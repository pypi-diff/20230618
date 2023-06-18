# Comparing `tmp/pulumi_datadog-4.9.0a1650908051.tar.gz` & `tmp/pulumi_datadog-4.9.0a1653604828.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulumi_datadog-4.9.0a1650908051.tar", last modified: Mon Apr 25 17:43:07 2022, max compression
+gzip compressed data, was "dist/pulumi_datadog-4.9.0a1653604828.tar", last modified: Thu May 26 22:44:11 2022, max compression
```

## Comparing `pulumi_datadog-4.9.0a1650908051.tar` & `pulumi_datadog-4.9.0a1653604828.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 17:43:07.000000 pulumi_datadog-4.9.0a1650908051/
--rw-r--r--   0 runner    (1001) docker     (121)     3294 2022-04-25 17:43:07.000000 pulumi_datadog-4.9.0a1650908051/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2462 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 17:43:07.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/
--rw-r--r--   0 runner    (1001) docker     (121)    10870 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)  2477234 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     7667 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)     6876 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/api_key.py
--rw-r--r--   0 runner    (1001) docker     (121)     7220 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/application_key.py
--rw-r--r--   0 runner    (1001) docker     (121)    10317 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/authn_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 17:43:07.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/aws/
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    39847 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/aws/integration.py
--rw-r--r--   0 runner    (1001) docker     (121)    10341 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/aws/integration_lambda_arn.py
--rw-r--r--   0 runner    (1001) docker     (121)    11184 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/aws/integration_log_collection.py
--rw-r--r--   0 runner    (1001) docker     (121)    12394 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/aws/integration_tag_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 17:43:07.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/azure/
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17159 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/azure/integration.py
--rw-r--r--   0 runner    (1001) docker     (121)    14108 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/child_organization.py
--rw-r--r--   0 runner    (1001) docker     (121)    12506 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/cloud_workload_security_agent_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 17:43:07.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/config/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2094 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (121)    98537 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (121)    47367 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/dashboard_json.py
--rw-r--r--   0 runner    (1001) docker     (121)    12899 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/dashboard_list.py
--rw-r--r--   0 runner    (1001) docker     (121)    30124 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/downtime.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 17:43:07.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/gcp/
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21022 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/gcp/integration.py
--rw-r--r--   0 runner    (1001) docker     (121)     3386 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_api_key.py
--rw-r--r--   0 runner    (1001) docker     (121)     3650 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_application_key.py
--rw-r--r--   0 runner    (1001) docker     (121)     2783 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_cloud_workload_security_agent_rules.py
--rw-r--r--   0 runner    (1001) docker     (121)     4027 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (121)     4466 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_dashboard_list.py
--rw-r--r--   0 runner    (1001) docker     (121)    11387 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_ip_ranges.py
--rw-r--r--   0 runner    (1001) docker     (121)     2430 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_logs_indexes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2611 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_logs_indexes_order.py
--rw-r--r--   0 runner    (1001) docker     (121)    19060 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)     5466 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_monitors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2423 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_permissions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3792 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_role.py
--rw-r--r--   0 runner    (1001) docker     (121)     3378 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (121)     3095 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_security_monitoring_filters.py
--rw-r--r--   0 runner    (1001) docker     (121)     7390 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_security_monitoring_rules.py
--rw-r--r--   0 runner    (1001) docker     (121)     6760 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_service_level_objective.py
--rw-r--r--   0 runner    (1001) docker     (121)     6410 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_service_level_objectives.py
--rw-r--r--   0 runner    (1001) docker     (121)     3578 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_synthetics_global_variable.py
--rw-r--r--   0 runner    (1001) docker     (121)     2357 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_synthetics_locations.py
--rw-r--r--   0 runner    (1001) docker     (121)     3952 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_synthetics_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3379 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_user.py
--rw-r--r--   0 runner    (1001) docker     (121)    20978 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/logs_archive.py
--rw-r--r--   0 runner    (1001) docker     (121)     9157 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/logs_archive_order.py
--rw-r--r--   0 runner    (1001) docker     (121)    26974 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/logs_custom_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)    20719 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/logs_index.py
--rw-r--r--   0 runner    (1001) docker     (121)     9552 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/logs_index_order.py
--rw-r--r--   0 runner    (1001) docker     (121)     7845 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/logs_integration_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)    15200 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/logs_metric.py
--rw-r--r--   0 runner    (1001) docker     (121)    11539 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/logs_pipeline_order.py
--rw-r--r--   0 runner    (1001) docker     (121)    17610 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/metric_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)    20996 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/metric_tag_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)    89036 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)    10010 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/monitor_json.py
--rw-r--r--   0 runner    (1001) docker     (121)    10872 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/organization_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)  2190032 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 17:43:07.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/pagerduty/
--rw-r--r--   0 runner    (1001) docker     (121)      326 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/pagerduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11738 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/pagerduty/integration.py
--rw-r--r--   0 runner    (1001) docker     (121)     9667 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/pagerduty/service_object.py
--rw-r--r--   0 runner    (1001) docker     (121)    12185 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    10763 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/role.py
--rw-r--r--   0 runner    (1001) docker     (121)    13013 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/security_monitoring_default_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)    17777 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/security_monitoring_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)    29084 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/security_monitoring_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)    33638 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/service_level_objective.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 17:43:07.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/slack/
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2724 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/slack/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    11228 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/slack/channel.py
--rw-r--r--   0 runner    (1001) docker     (121)     2062 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/slack/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    24275 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/slo_correction.py
--rw-r--r--   0 runner    (1001) docker     (121)    22883 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/synthetics_global_variable.py
--rw-r--r--   0 runner    (1001) docker     (121)    12580 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/synthetics_private_location.py
--rw-r--r--   0 runner    (1001) docker     (121)    81780 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/synthetics_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    16317 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/user.py
--rw-r--r--   0 runner    (1001) docker     (121)    14010 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/webhook.py
--rw-r--r--   0 runner    (1001) docker     (121)    10542 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog/webhook_custom_variable.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 17:43:07.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3294 2022-04-25 17:43:07.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3102 2022-04-25 17:43:07.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-25 17:43:07.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-25 17:43:07.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-04-25 17:43:07.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-04-25 17:43:07.000000 pulumi_datadog-4.9.0a1650908051/pulumi_datadog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-25 17:43:07.000000 pulumi_datadog-4.9.0a1650908051/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2127 2022-04-25 17:43:06.000000 pulumi_datadog-4.9.0a1650908051/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/
+-rw-r--r--   0 runner    (1001) docker     (121)     3294 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2462 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/
+-rw-r--r--   0 runner    (1001) docker     (121)    10870 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)  2414008 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7667 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6876 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7220 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/application_key.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10317 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/authn_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/aws/
+-rw-r--r--   0 runner    (1001) docker     (121)      414 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40351 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/aws/integration.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10341 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/aws/integration_lambda_arn.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11352 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/aws/integration_log_collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11750 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/aws/integration_tag_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/azure/
+-rw-r--r--   0 runner    (1001) docker     (121)      296 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17327 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/azure/integration.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14108 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/child_organization.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12506 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/cloud_workload_security_agent_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/config/
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2114 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (121)    97389 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (121)    47367 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/dashboard_json.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12899 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/dashboard_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33168 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/downtime.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/gcp/
+-rw-r--r--   0 runner    (1001) docker     (121)      296 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21106 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/gcp/integration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3078 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3286 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_application_key.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2730 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_cloud_workload_security_agent_rules.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3630 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4259 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_dashboard_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9425 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_ip_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2377 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_logs_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2340 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_logs_indexes_order.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15684 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4480 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_monitors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2339 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3472 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3136 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2990 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_security_monitoring_filters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7390 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_security_monitoring_rules.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5536 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_service_level_objective.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5486 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_service_level_objectives.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3145 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_synthetics_global_variable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2251 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_synthetics_locations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3548 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_synthetics_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3082 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23887 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/logs_archive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9325 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/logs_archive_order.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26974 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/logs_custom_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20803 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/logs_index.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9636 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/logs_index_order.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7845 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/logs_integration_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15200 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/logs_metric.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11777 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/logs_pipeline_order.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17743 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/metric_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20835 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/metric_tag_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)    93812 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10010 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/monitor_json.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10872 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/organization_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)  2131533 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/pagerduty/
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/pagerduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11738 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/pagerduty/integration.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11781 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/pagerduty/service_object.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12245 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    10763 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/role.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13013 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/security_monitoring_default_rule.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17602 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/security_monitoring_filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29084 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/security_monitoring_rule.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33708 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/service_level_objective.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/slack/
+-rw-r--r--   0 runner    (1001) docker     (121)      337 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2059 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/slack/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11228 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/slack/channel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/slack/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23722 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/slo_correction.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22883 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/synthetics_global_variable.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14989 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/synthetics_private_location.py
+-rw-r--r--   0 runner    (1001) docker     (121)    79204 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/synthetics_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16317 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/user.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13779 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10542 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog/webhook_custom_variable.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3294 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3102 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/pulumi_datadog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2127 2022-05-26 22:44:11.000000 pulumi_datadog-4.9.0a1653604828/setup.py
```

### Comparing `pulumi_datadog-4.9.0a1650908051/PKG-INFO` & `pulumi_datadog-4.9.0a1653604828/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_datadog
-Version: 4.9.0a1650908051
+Version: 4.9.0a1653604828
 Summary: A Pulumi package for creating and managing Datadog resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-datadog
 Description: [![Actions Status](https://github.com/pulumi/pulumi-datadog/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-datadog/actions)
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
         [![NPM version](https://badge.fury.io/js/%40pulumi%2Fdatadog.svg)](https://www.npmjs.com/package/@pulumi/datadog)
```

### Comparing `pulumi_datadog-4.9.0a1650908051/README.md` & `pulumi_datadog-4.9.0a1653604828/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/__init__.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/_inputs.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -378,14 +378,16 @@
     'DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionRequestRumQueryGroupBySortQueryArgs',
     'DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionRequestRumQueryMultiComputeArgs',
     'DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionRequestSecurityQueryArgs',
     'DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionRequestSecurityQueryComputeQueryArgs',
     'DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionRequestSecurityQueryGroupByArgs',
     'DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionRequestSecurityQueryGroupBySortQueryArgs',
     'DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionRequestSecurityQueryMultiComputeArgs',
+    'DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionTimeseriesBackgroundArgs',
+    'DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionTimeseriesBackgroundYaxisArgs',
     'DashboardWidgetGroupDefinitionWidgetScatterplotDefinitionArgs',
     'DashboardWidgetGroupDefinitionWidgetScatterplotDefinitionCustomLinkArgs',
     'DashboardWidgetGroupDefinitionWidgetScatterplotDefinitionRequestArgs',
     'DashboardWidgetGroupDefinitionWidgetScatterplotDefinitionRequestScatterplotTableArgs',
     'DashboardWidgetGroupDefinitionWidgetScatterplotDefinitionRequestScatterplotTableFormulaArgs',
     'DashboardWidgetGroupDefinitionWidgetScatterplotDefinitionRequestScatterplotTableQueryArgs',
     'DashboardWidgetGroupDefinitionWidgetScatterplotDefinitionRequestScatterplotTableQueryApmDependencyStatsQueryArgs',
@@ -769,14 +771,16 @@
     'DashboardWidgetQueryValueDefinitionRequestRumQueryGroupBySortQueryArgs',
     'DashboardWidgetQueryValueDefinitionRequestRumQueryMultiComputeArgs',
     'DashboardWidgetQueryValueDefinitionRequestSecurityQueryArgs',
     'DashboardWidgetQueryValueDefinitionRequestSecurityQueryComputeQueryArgs',
     'DashboardWidgetQueryValueDefinitionRequestSecurityQueryGroupByArgs',
     'DashboardWidgetQueryValueDefinitionRequestSecurityQueryGroupBySortQueryArgs',
     'DashboardWidgetQueryValueDefinitionRequestSecurityQueryMultiComputeArgs',
+    'DashboardWidgetQueryValueDefinitionTimeseriesBackgroundArgs',
+    'DashboardWidgetQueryValueDefinitionTimeseriesBackgroundYaxisArgs',
     'DashboardWidgetScatterplotDefinitionArgs',
     'DashboardWidgetScatterplotDefinitionCustomLinkArgs',
     'DashboardWidgetScatterplotDefinitionRequestArgs',
     'DashboardWidgetScatterplotDefinitionRequestScatterplotTableArgs',
     'DashboardWidgetScatterplotDefinitionRequestScatterplotTableFormulaArgs',
     'DashboardWidgetScatterplotDefinitionRequestScatterplotTableQueryArgs',
     'DashboardWidgetScatterplotDefinitionRequestScatterplotTableQueryApmDependencyStatsQueryArgs',
@@ -1060,21 +1064,23 @@
     'RolePermissionArgs',
     'SecurityMonitoringDefaultRuleCaseArgs',
     'SecurityMonitoringDefaultRuleFilterArgs',
     'SecurityMonitoringFilterExclusionFilterArgs',
     'SecurityMonitoringRuleCaseArgs',
     'SecurityMonitoringRuleFilterArgs',
     'SecurityMonitoringRuleOptionsArgs',
+    'SecurityMonitoringRuleOptionsImpossibleTravelOptionsArgs',
     'SecurityMonitoringRuleOptionsNewValueOptionsArgs',
     'SecurityMonitoringRuleQueryArgs',
     'SecurityMonitoringRuleQueryAgentRuleArgs',
     'ServiceLevelObjectiveQueryArgs',
     'ServiceLevelObjectiveThresholdArgs',
     'SyntheticsGlobalVariableParseTestOptionsArgs',
     'SyntheticsGlobalVariableParseTestOptionsParserArgs',
+    'SyntheticsPrivateLocationMetadataArgs',
     'SyntheticsTestApiStepArgs',
     'SyntheticsTestApiStepAssertionArgs',
     'SyntheticsTestApiStepAssertionTargetjsonpathArgs',
     'SyntheticsTestApiStepExtractedValueArgs',
     'SyntheticsTestApiStepExtractedValueParserArgs',
     'SyntheticsTestApiStepRequestBasicauthArgs',
     'SyntheticsTestApiStepRequestClientCertificateArgs',
@@ -1104,17 +1110,14 @@
 ]
 
 @pulumi.input_type
 class ChildOrganizationApiKeyArgs:
     def __init__(__self__, *,
                  key: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] name: Name for Child Organization after creation.
-        """
         if key is not None:
             pulumi.set(__self__, "key", key)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
@@ -1124,33 +1127,27 @@
     @key.setter
     def key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
-        """
-        Name for Child Organization after creation.
-        """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
 
 @pulumi.input_type
 class ChildOrganizationApplicationKeyArgs:
     def __init__(__self__, *,
                  hash: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  owner: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] name: Name for Child Organization after creation.
-        """
         if hash is not None:
             pulumi.set(__self__, "hash", hash)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if owner is not None:
             pulumi.set(__self__, "owner", owner)
 
@@ -1162,17 +1159,14 @@
     @hash.setter
     def hash(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "hash", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
-        """
-        Name for Child Organization after creation.
-        """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
@@ -1392,17 +1386,14 @@
 
 @pulumi.input_type
 class ChildOrganizationUserArgs:
     def __init__(__self__, *,
                  access_role: Optional[pulumi.Input[str]] = None,
                  email: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] name: Name for Child Organization after creation.
-        """
         if access_role is not None:
             pulumi.set(__self__, "access_role", access_role)
         if email is not None:
             pulumi.set(__self__, "email", email)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
@@ -1423,189 +1414,142 @@
     @email.setter
     def email(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "email", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
-        """
-        Name for Child Organization after creation.
-        """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
 
 @pulumi.input_type
 class DashboardListDashItemArgs:
     def __init__(__self__, *,
                  dash_id: pulumi.Input[str],
                  type: pulumi.Input[str]):
-        """
-        :param pulumi.Input[str] dash_id: The ID of the dashboard to add
-        :param pulumi.Input[str] type: The type of this dashboard. Valid values are `custom_timeboard`, `custom_screenboard`, `integration_screenboard`, `integration_timeboard`, `host_timeboard`.
-        """
         pulumi.set(__self__, "dash_id", dash_id)
         pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter(name="dashId")
     def dash_id(self) -> pulumi.Input[str]:
-        """
-        The ID of the dashboard to add
-        """
         return pulumi.get(self, "dash_id")
 
     @dash_id.setter
     def dash_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "dash_id", value)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
-        """
-        The type of this dashboard. Valid values are `custom_timeboard`, `custom_screenboard`, `integration_screenboard`, `integration_timeboard`, `host_timeboard`.
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
 
 @pulumi.input_type
 class DashboardTemplateVariableArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  available_values: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  default: Optional[pulumi.Input[str]] = None,
                  prefix: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] name: The name of the variable.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] available_values: The list of values that the template variable drop-down is be limited to
-        :param pulumi.Input[str] default: The default value for the template variable on dashboard load.
-        :param pulumi.Input[str] prefix: The tag prefix associated with the variable. Only tags with this prefix appear in the variable dropdown.
-        """
         pulumi.set(__self__, "name", name)
         if available_values is not None:
             pulumi.set(__self__, "available_values", available_values)
         if default is not None:
             pulumi.set(__self__, "default", default)
         if prefix is not None:
             pulumi.set(__self__, "prefix", prefix)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
-        """
-        The name of the variable.
-        """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="availableValues")
     def available_values(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        The list of values that the template variable drop-down is be limited to
-        """
         return pulumi.get(self, "available_values")
 
     @available_values.setter
     def available_values(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "available_values", value)
 
     @property
     @pulumi.getter
     def default(self) -> Optional[pulumi.Input[str]]:
-        """
-        The default value for the template variable on dashboard load.
-        """
         return pulumi.get(self, "default")
 
     @default.setter
     def default(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default", value)
 
     @property
     @pulumi.getter
     def prefix(self) -> Optional[pulumi.Input[str]]:
-        """
-        The tag prefix associated with the variable. Only tags with this prefix appear in the variable dropdown.
-        """
         return pulumi.get(self, "prefix")
 
     @prefix.setter
     def prefix(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "prefix", value)
 
 
 @pulumi.input_type
 class DashboardTemplateVariablePresetArgs:
     def __init__(__self__, *,
                  name: Optional[pulumi.Input[str]] = None,
                  template_variables: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardTemplateVariablePresetTemplateVariableArgs']]]] = None):
-        """
-        :param pulumi.Input[str] name: The name of the preset.
-        :param pulumi.Input[Sequence[pulumi.Input['DashboardTemplateVariablePresetTemplateVariableArgs']]] template_variables: The template variable names and assumed values under the given preset
-        """
         if name is not None:
             pulumi.set(__self__, "name", name)
         if template_variables is not None:
             pulumi.set(__self__, "template_variables", template_variables)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
-        """
-        The name of the preset.
-        """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="templateVariables")
     def template_variables(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['DashboardTemplateVariablePresetTemplateVariableArgs']]]]:
-        """
-        The template variable names and assumed values under the given preset
-        """
         return pulumi.get(self, "template_variables")
 
     @template_variables.setter
     def template_variables(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardTemplateVariablePresetTemplateVariableArgs']]]]):
         pulumi.set(self, "template_variables", value)
 
 
 @pulumi.input_type
 class DashboardTemplateVariablePresetTemplateVariableArgs:
     def __init__(__self__, *,
                  name: Optional[pulumi.Input[str]] = None,
                  value: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] name: The name of the variable.
-        """
         if name is not None:
             pulumi.set(__self__, "name", name)
         if value is not None:
             pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
-        """
-        The name of the variable.
-        """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
@@ -1646,45 +1590,14 @@
                  servicemap_definition: Optional[pulumi.Input['DashboardWidgetServicemapDefinitionArgs']] = None,
                  sunburst_definition: Optional[pulumi.Input['DashboardWidgetSunburstDefinitionArgs']] = None,
                  timeseries_definition: Optional[pulumi.Input['DashboardWidgetTimeseriesDefinitionArgs']] = None,
                  toplist_definition: Optional[pulumi.Input['DashboardWidgetToplistDefinitionArgs']] = None,
                  trace_service_definition: Optional[pulumi.Input['DashboardWidgetTraceServiceDefinitionArgs']] = None,
                  treemap_definition: Optional[pulumi.Input['DashboardWidgetTreemapDefinitionArgs']] = None,
                  widget_layout: Optional[pulumi.Input['DashboardWidgetWidgetLayoutArgs']] = None):
-        """
-        :param pulumi.Input['DashboardWidgetAlertGraphDefinitionArgs'] alert_graph_definition: The definition for a Alert Graph widget.
-        :param pulumi.Input['DashboardWidgetAlertValueDefinitionArgs'] alert_value_definition: The definition for a Alert Value widget.
-        :param pulumi.Input['DashboardWidgetChangeDefinitionArgs'] change_definition: The definition for a Change widget.
-        :param pulumi.Input['DashboardWidgetCheckStatusDefinitionArgs'] check_status_definition: The definition for a Check Status widget.
-        :param pulumi.Input['DashboardWidgetDistributionDefinitionArgs'] distribution_definition: The definition for a Distribution widget.
-        :param pulumi.Input['DashboardWidgetEventStreamDefinitionArgs'] event_stream_definition: The definition for a Event Stream widget.
-        :param pulumi.Input['DashboardWidgetEventTimelineDefinitionArgs'] event_timeline_definition: The definition for a Event Timeline widget.
-        :param pulumi.Input['DashboardWidgetFreeTextDefinitionArgs'] free_text_definition: The definition for a Free Text widget.
-        :param pulumi.Input['DashboardWidgetGeomapDefinitionArgs'] geomap_definition: The definition for a Geomap widget.
-        :param pulumi.Input['DashboardWidgetGroupDefinitionArgs'] group_definition: The definition for a Group widget.
-        :param pulumi.Input['DashboardWidgetHeatmapDefinitionArgs'] heatmap_definition: The definition for a Heatmap widget.
-        :param pulumi.Input['DashboardWidgetHostmapDefinitionArgs'] hostmap_definition: The definition for a Hostmap widget.
-        :param pulumi.Input[int] id: The ID of the widget.
-        :param pulumi.Input['DashboardWidgetIframeDefinitionArgs'] iframe_definition: The definition for an Iframe widget.
-        :param pulumi.Input['DashboardWidgetImageDefinitionArgs'] image_definition: The definition for an Image widget
-        :param pulumi.Input['DashboardWidgetLogStreamDefinitionArgs'] log_stream_definition: The definition for an Log Stream widget.
-        :param pulumi.Input['DashboardWidgetManageStatusDefinitionArgs'] manage_status_definition: The definition for an Manage Status widget.
-        :param pulumi.Input['DashboardWidgetNoteDefinitionArgs'] note_definition: The definition for a Note widget.
-        :param pulumi.Input['DashboardWidgetQueryTableDefinitionArgs'] query_table_definition: The definition for a Query Table widget.
-        :param pulumi.Input['DashboardWidgetQueryValueDefinitionArgs'] query_value_definition: The definition for a Query Value widget.
-        :param pulumi.Input['DashboardWidgetScatterplotDefinitionArgs'] scatterplot_definition: The definition for a Scatterplot widget.
-        :param pulumi.Input['DashboardWidgetServiceLevelObjectiveDefinitionArgs'] service_level_objective_definition: The definition for a Service Level Objective widget.
-        :param pulumi.Input['DashboardWidgetServicemapDefinitionArgs'] servicemap_definition: The definition for a Service Map widget.
-        :param pulumi.Input['DashboardWidgetSunburstDefinitionArgs'] sunburst_definition: The definition for a Sunburst widget.
-        :param pulumi.Input['DashboardWidgetTimeseriesDefinitionArgs'] timeseries_definition: The definition for a Timeseries widget.
-        :param pulumi.Input['DashboardWidgetToplistDefinitionArgs'] toplist_definition: The definition for a Toplist widget.
-        :param pulumi.Input['DashboardWidgetTraceServiceDefinitionArgs'] trace_service_definition: The definition for a Trace Service widget.
-        :param pulumi.Input['DashboardWidgetTreemapDefinitionArgs'] treemap_definition: The definition for a Treemap widget.
-        :param pulumi.Input['DashboardWidgetWidgetLayoutArgs'] widget_layout: The layout of the widget on a 'free' dashboard.
-        """
         if alert_graph_definition is not None:
             pulumi.set(__self__, "alert_graph_definition", alert_graph_definition)
         if alert_value_definition is not None:
             pulumi.set(__self__, "alert_value_definition", alert_value_definition)
         if change_definition is not None:
             pulumi.set(__self__, "change_definition", change_definition)
         if check_status_definition is not None:
@@ -1739,353 +1652,266 @@
             pulumi.set(__self__, "treemap_definition", treemap_definition)
         if widget_layout is not None:
             pulumi.set(__self__, "widget_layout", widget_layout)
 
     @property
     @pulumi.getter(name="alertGraphDefinition")
     def alert_graph_definition(self) -> Optional[pulumi.Input['DashboardWidgetAlertGraphDefinitionArgs']]:
-        """
-        The definition for a Alert Graph widget.
-        """
         return pulumi.get(self, "alert_graph_definition")
 
     @alert_graph_definition.setter
     def alert_graph_definition(self, value: Optional[pulumi.Input['DashboardWidgetAlertGraphDefinitionArgs']]):
         pulumi.set(self, "alert_graph_definition", value)
 
     @property
     @pulumi.getter(name="alertValueDefinition")
     def alert_value_definition(self) -> Optional[pulumi.Input['DashboardWidgetAlertValueDefinitionArgs']]:
-        """
-        The definition for a Alert Value widget.
-        """
         return pulumi.get(self, "alert_value_definition")
 
     @alert_value_definition.setter
     def alert_value_definition(self, value: Optional[pulumi.Input['DashboardWidgetAlertValueDefinitionArgs']]):
         pulumi.set(self, "alert_value_definition", value)
 
     @property
     @pulumi.getter(name="changeDefinition")
     def change_definition(self) -> Optional[pulumi.Input['DashboardWidgetChangeDefinitionArgs']]:
-        """
-        The definition for a Change widget.
-        """
         return pulumi.get(self, "change_definition")
 
     @change_definition.setter
     def change_definition(self, value: Optional[pulumi.Input['DashboardWidgetChangeDefinitionArgs']]):
         pulumi.set(self, "change_definition", value)
 
     @property
     @pulumi.getter(name="checkStatusDefinition")
     def check_status_definition(self) -> Optional[pulumi.Input['DashboardWidgetCheckStatusDefinitionArgs']]:
-        """
-        The definition for a Check Status widget.
-        """
         return pulumi.get(self, "check_status_definition")
 
     @check_status_definition.setter
     def check_status_definition(self, value: Optional[pulumi.Input['DashboardWidgetCheckStatusDefinitionArgs']]):
         pulumi.set(self, "check_status_definition", value)
 
     @property
     @pulumi.getter(name="distributionDefinition")
     def distribution_definition(self) -> Optional[pulumi.Input['DashboardWidgetDistributionDefinitionArgs']]:
-        """
-        The definition for a Distribution widget.
-        """
         return pulumi.get(self, "distribution_definition")
 
     @distribution_definition.setter
     def distribution_definition(self, value: Optional[pulumi.Input['DashboardWidgetDistributionDefinitionArgs']]):
         pulumi.set(self, "distribution_definition", value)
 
     @property
     @pulumi.getter(name="eventStreamDefinition")
     def event_stream_definition(self) -> Optional[pulumi.Input['DashboardWidgetEventStreamDefinitionArgs']]:
-        """
-        The definition for a Event Stream widget.
-        """
         return pulumi.get(self, "event_stream_definition")
 
     @event_stream_definition.setter
     def event_stream_definition(self, value: Optional[pulumi.Input['DashboardWidgetEventStreamDefinitionArgs']]):
         pulumi.set(self, "event_stream_definition", value)
 
     @property
     @pulumi.getter(name="eventTimelineDefinition")
     def event_timeline_definition(self) -> Optional[pulumi.Input['DashboardWidgetEventTimelineDefinitionArgs']]:
-        """
-        The definition for a Event Timeline widget.
-        """
         return pulumi.get(self, "event_timeline_definition")
 
     @event_timeline_definition.setter
     def event_timeline_definition(self, value: Optional[pulumi.Input['DashboardWidgetEventTimelineDefinitionArgs']]):
         pulumi.set(self, "event_timeline_definition", value)
 
     @property
     @pulumi.getter(name="freeTextDefinition")
     def free_text_definition(self) -> Optional[pulumi.Input['DashboardWidgetFreeTextDefinitionArgs']]:
-        """
-        The definition for a Free Text widget.
-        """
         return pulumi.get(self, "free_text_definition")
 
     @free_text_definition.setter
     def free_text_definition(self, value: Optional[pulumi.Input['DashboardWidgetFreeTextDefinitionArgs']]):
         pulumi.set(self, "free_text_definition", value)
 
     @property
     @pulumi.getter(name="geomapDefinition")
     def geomap_definition(self) -> Optional[pulumi.Input['DashboardWidgetGeomapDefinitionArgs']]:
-        """
-        The definition for a Geomap widget.
-        """
         return pulumi.get(self, "geomap_definition")
 
     @geomap_definition.setter
     def geomap_definition(self, value: Optional[pulumi.Input['DashboardWidgetGeomapDefinitionArgs']]):
         pulumi.set(self, "geomap_definition", value)
 
     @property
     @pulumi.getter(name="groupDefinition")
     def group_definition(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionArgs']]:
-        """
-        The definition for a Group widget.
-        """
         return pulumi.get(self, "group_definition")
 
     @group_definition.setter
     def group_definition(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionArgs']]):
         pulumi.set(self, "group_definition", value)
 
     @property
     @pulumi.getter(name="heatmapDefinition")
     def heatmap_definition(self) -> Optional[pulumi.Input['DashboardWidgetHeatmapDefinitionArgs']]:
-        """
-        The definition for a Heatmap widget.
-        """
         return pulumi.get(self, "heatmap_definition")
 
     @heatmap_definition.setter
     def heatmap_definition(self, value: Optional[pulumi.Input['DashboardWidgetHeatmapDefinitionArgs']]):
         pulumi.set(self, "heatmap_definition", value)
 
     @property
     @pulumi.getter(name="hostmapDefinition")
     def hostmap_definition(self) -> Optional[pulumi.Input['DashboardWidgetHostmapDefinitionArgs']]:
-        """
-        The definition for a Hostmap widget.
-        """
         return pulumi.get(self, "hostmap_definition")
 
     @hostmap_definition.setter
     def hostmap_definition(self, value: Optional[pulumi.Input['DashboardWidgetHostmapDefinitionArgs']]):
         pulumi.set(self, "hostmap_definition", value)
 
     @property
     @pulumi.getter
     def id(self) -> Optional[pulumi.Input[int]]:
-        """
-        The ID of the widget.
-        """
         return pulumi.get(self, "id")
 
     @id.setter
     def id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "id", value)
 
     @property
     @pulumi.getter(name="iframeDefinition")
     def iframe_definition(self) -> Optional[pulumi.Input['DashboardWidgetIframeDefinitionArgs']]:
-        """
-        The definition for an Iframe widget.
-        """
         return pulumi.get(self, "iframe_definition")
 
     @iframe_definition.setter
     def iframe_definition(self, value: Optional[pulumi.Input['DashboardWidgetIframeDefinitionArgs']]):
         pulumi.set(self, "iframe_definition", value)
 
     @property
     @pulumi.getter(name="imageDefinition")
     def image_definition(self) -> Optional[pulumi.Input['DashboardWidgetImageDefinitionArgs']]:
-        """
-        The definition for an Image widget
-        """
         return pulumi.get(self, "image_definition")
 
     @image_definition.setter
     def image_definition(self, value: Optional[pulumi.Input['DashboardWidgetImageDefinitionArgs']]):
         pulumi.set(self, "image_definition", value)
 
     @property
     @pulumi.getter(name="logStreamDefinition")
     def log_stream_definition(self) -> Optional[pulumi.Input['DashboardWidgetLogStreamDefinitionArgs']]:
-        """
-        The definition for an Log Stream widget.
-        """
         return pulumi.get(self, "log_stream_definition")
 
     @log_stream_definition.setter
     def log_stream_definition(self, value: Optional[pulumi.Input['DashboardWidgetLogStreamDefinitionArgs']]):
         pulumi.set(self, "log_stream_definition", value)
 
     @property
     @pulumi.getter(name="manageStatusDefinition")
     def manage_status_definition(self) -> Optional[pulumi.Input['DashboardWidgetManageStatusDefinitionArgs']]:
-        """
-        The definition for an Manage Status widget.
-        """
         return pulumi.get(self, "manage_status_definition")
 
     @manage_status_definition.setter
     def manage_status_definition(self, value: Optional[pulumi.Input['DashboardWidgetManageStatusDefinitionArgs']]):
         pulumi.set(self, "manage_status_definition", value)
 
     @property
     @pulumi.getter(name="noteDefinition")
     def note_definition(self) -> Optional[pulumi.Input['DashboardWidgetNoteDefinitionArgs']]:
-        """
-        The definition for a Note widget.
-        """
         return pulumi.get(self, "note_definition")
 
     @note_definition.setter
     def note_definition(self, value: Optional[pulumi.Input['DashboardWidgetNoteDefinitionArgs']]):
         pulumi.set(self, "note_definition", value)
 
     @property
     @pulumi.getter(name="queryTableDefinition")
     def query_table_definition(self) -> Optional[pulumi.Input['DashboardWidgetQueryTableDefinitionArgs']]:
-        """
-        The definition for a Query Table widget.
-        """
         return pulumi.get(self, "query_table_definition")
 
     @query_table_definition.setter
     def query_table_definition(self, value: Optional[pulumi.Input['DashboardWidgetQueryTableDefinitionArgs']]):
         pulumi.set(self, "query_table_definition", value)
 
     @property
     @pulumi.getter(name="queryValueDefinition")
     def query_value_definition(self) -> Optional[pulumi.Input['DashboardWidgetQueryValueDefinitionArgs']]:
-        """
-        The definition for a Query Value widget.
-        """
         return pulumi.get(self, "query_value_definition")
 
     @query_value_definition.setter
     def query_value_definition(self, value: Optional[pulumi.Input['DashboardWidgetQueryValueDefinitionArgs']]):
         pulumi.set(self, "query_value_definition", value)
 
     @property
     @pulumi.getter(name="scatterplotDefinition")
     def scatterplot_definition(self) -> Optional[pulumi.Input['DashboardWidgetScatterplotDefinitionArgs']]:
-        """
-        The definition for a Scatterplot widget.
-        """
         return pulumi.get(self, "scatterplot_definition")
 
     @scatterplot_definition.setter
     def scatterplot_definition(self, value: Optional[pulumi.Input['DashboardWidgetScatterplotDefinitionArgs']]):
         pulumi.set(self, "scatterplot_definition", value)
 
     @property
     @pulumi.getter(name="serviceLevelObjectiveDefinition")
     def service_level_objective_definition(self) -> Optional[pulumi.Input['DashboardWidgetServiceLevelObjectiveDefinitionArgs']]:
-        """
-        The definition for a Service Level Objective widget.
-        """
         return pulumi.get(self, "service_level_objective_definition")
 
     @service_level_objective_definition.setter
     def service_level_objective_definition(self, value: Optional[pulumi.Input['DashboardWidgetServiceLevelObjectiveDefinitionArgs']]):
         pulumi.set(self, "service_level_objective_definition", value)
 
     @property
     @pulumi.getter(name="servicemapDefinition")
     def servicemap_definition(self) -> Optional[pulumi.Input['DashboardWidgetServicemapDefinitionArgs']]:
-        """
-        The definition for a Service Map widget.
-        """
         return pulumi.get(self, "servicemap_definition")
 
     @servicemap_definition.setter
     def servicemap_definition(self, value: Optional[pulumi.Input['DashboardWidgetServicemapDefinitionArgs']]):
         pulumi.set(self, "servicemap_definition", value)
 
     @property
     @pulumi.getter(name="sunburstDefinition")
     def sunburst_definition(self) -> Optional[pulumi.Input['DashboardWidgetSunburstDefinitionArgs']]:
-        """
-        The definition for a Sunburst widget.
-        """
         return pulumi.get(self, "sunburst_definition")
 
     @sunburst_definition.setter
     def sunburst_definition(self, value: Optional[pulumi.Input['DashboardWidgetSunburstDefinitionArgs']]):
         pulumi.set(self, "sunburst_definition", value)
 
     @property
     @pulumi.getter(name="timeseriesDefinition")
     def timeseries_definition(self) -> Optional[pulumi.Input['DashboardWidgetTimeseriesDefinitionArgs']]:
-        """
-        The definition for a Timeseries widget.
-        """
         return pulumi.get(self, "timeseries_definition")
 
     @timeseries_definition.setter
     def timeseries_definition(self, value: Optional[pulumi.Input['DashboardWidgetTimeseriesDefinitionArgs']]):
         pulumi.set(self, "timeseries_definition", value)
 
     @property
     @pulumi.getter(name="toplistDefinition")
     def toplist_definition(self) -> Optional[pulumi.Input['DashboardWidgetToplistDefinitionArgs']]:
-        """
-        The definition for a Toplist widget.
-        """
         return pulumi.get(self, "toplist_definition")
 
     @toplist_definition.setter
     def toplist_definition(self, value: Optional[pulumi.Input['DashboardWidgetToplistDefinitionArgs']]):
         pulumi.set(self, "toplist_definition", value)
 
     @property
     @pulumi.getter(name="traceServiceDefinition")
     def trace_service_definition(self) -> Optional[pulumi.Input['DashboardWidgetTraceServiceDefinitionArgs']]:
-        """
-        The definition for a Trace Service widget.
-        """
         return pulumi.get(self, "trace_service_definition")
 
     @trace_service_definition.setter
     def trace_service_definition(self, value: Optional[pulumi.Input['DashboardWidgetTraceServiceDefinitionArgs']]):
         pulumi.set(self, "trace_service_definition", value)
 
     @property
     @pulumi.getter(name="treemapDefinition")
     def treemap_definition(self) -> Optional[pulumi.Input['DashboardWidgetTreemapDefinitionArgs']]:
-        """
-        The definition for a Treemap widget.
-        """
         return pulumi.get(self, "treemap_definition")
 
     @treemap_definition.setter
     def treemap_definition(self, value: Optional[pulumi.Input['DashboardWidgetTreemapDefinitionArgs']]):
         pulumi.set(self, "treemap_definition", value)
 
     @property
     @pulumi.getter(name="widgetLayout")
     def widget_layout(self) -> Optional[pulumi.Input['DashboardWidgetWidgetLayoutArgs']]:
-        """
-        The layout of the widget on a 'free' dashboard.
-        """
         return pulumi.get(self, "widget_layout")
 
     @widget_layout.setter
     def widget_layout(self, value: Optional[pulumi.Input['DashboardWidgetWidgetLayoutArgs']]):
         pulumi.set(self, "widget_layout", value)
 
 
@@ -2094,17 +1920,14 @@
     def __init__(__self__, *,
                  alert_id: pulumi.Input[str],
                  viz_type: pulumi.Input[str],
                  live_span: Optional[pulumi.Input[str]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         pulumi.set(__self__, "alert_id", alert_id)
         pulumi.set(__self__, "viz_type", viz_type)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if title is not None:
             pulumi.set(__self__, "title", title)
         if title_align is not None:
@@ -2138,17 +1961,14 @@
     @live_span.setter
     def live_span(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "live_span", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -2176,17 +1996,14 @@
                  alert_id: pulumi.Input[str],
                  precision: Optional[pulumi.Input[int]] = None,
                  text_align: Optional[pulumi.Input[str]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None,
                  unit: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         pulumi.set(__self__, "alert_id", alert_id)
         if precision is not None:
             pulumi.set(__self__, "precision", precision)
         if text_align is not None:
             pulumi.set(__self__, "text_align", text_align)
         if title is not None:
             pulumi.set(__self__, "title", title)
@@ -2223,17 +2040,14 @@
     @text_align.setter
     def text_align(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "text_align", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -2269,17 +2083,14 @@
     def __init__(__self__, *,
                  custom_links: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetChangeDefinitionCustomLinkArgs']]]] = None,
                  live_span: Optional[pulumi.Input[str]] = None,
                  requests: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetChangeDefinitionRequestArgs']]]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if requests is not None:
             pulumi.set(__self__, "requests", requests)
         if title is not None:
@@ -2315,17 +2126,14 @@
     @requests.setter
     def requests(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetChangeDefinitionRequestArgs']]]]):
         pulumi.set(self, "requests", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -4406,17 +4214,14 @@
                  group: Optional[pulumi.Input[str]] = None,
                  group_bies: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  live_span: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         pulumi.set(__self__, "check", check)
         pulumi.set(__self__, "grouping", grouping)
         if group is not None:
             pulumi.set(__self__, "group", group)
         if group_bies is not None:
             pulumi.set(__self__, "group_bies", group_bies)
         if live_span is not None:
@@ -4483,17 +4288,14 @@
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -4521,17 +4323,14 @@
                  legend_size: Optional[pulumi.Input[str]] = None,
                  live_span: Optional[pulumi.Input[str]] = None,
                  requests: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetDistributionDefinitionRequestArgs']]]] = None,
                  show_legend: Optional[pulumi.Input[bool]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         if legend_size is not None:
             pulumi.set(__self__, "legend_size", legend_size)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if requests is not None:
             pulumi.set(__self__, "requests", requests)
         if show_legend is not None:
@@ -4578,17 +4377,14 @@
     @show_legend.setter
     def show_legend(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "show_legend", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -5818,17 +5614,14 @@
                  query: pulumi.Input[str],
                  event_size: Optional[pulumi.Input[str]] = None,
                  live_span: Optional[pulumi.Input[str]] = None,
                  tags_execution: Optional[pulumi.Input[str]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         pulumi.set(__self__, "query", query)
         if event_size is not None:
             pulumi.set(__self__, "event_size", event_size)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if tags_execution is not None:
             pulumi.set(__self__, "tags_execution", tags_execution)
@@ -5874,17 +5667,14 @@
     @tags_execution.setter
     def tags_execution(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "tags_execution", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -5911,17 +5701,14 @@
     def __init__(__self__, *,
                  query: pulumi.Input[str],
                  live_span: Optional[pulumi.Input[str]] = None,
                  tags_execution: Optional[pulumi.Input[str]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         pulumi.set(__self__, "query", query)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if tags_execution is not None:
             pulumi.set(__self__, "tags_execution", tags_execution)
         if title is not None:
             pulumi.set(__self__, "title", title)
@@ -5956,17 +5743,14 @@
     @tags_execution.setter
     def tags_execution(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "tags_execution", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -6047,17 +5831,14 @@
                  custom_links: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGeomapDefinitionCustomLinkArgs']]]] = None,
                  live_span: Optional[pulumi.Input[str]] = None,
                  requests: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGeomapDefinitionRequestArgs']]]] = None,
                  style: Optional[pulumi.Input['DashboardWidgetGeomapDefinitionStyleArgs']] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         pulumi.set(__self__, "view", view)
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if requests is not None:
             pulumi.set(__self__, "requests", requests)
@@ -6114,17 +5895,14 @@
     @style.setter
     def style(self, value: Optional[pulumi.Input['DashboardWidgetGeomapDefinitionStyleArgs']]):
         pulumi.set(self, "style", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -7637,48 +7415,37 @@
     def __init__(__self__, *,
                  layout_type: pulumi.Input[str],
                  widgets: pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGroupDefinitionWidgetArgs']]],
                  background_color: Optional[pulumi.Input[str]] = None,
                  banner_img: Optional[pulumi.Input[str]] = None,
                  show_title: Optional[pulumi.Input[bool]] = None,
                  title: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] layout_type: The layout type of the dashboard. Valid values are `ordered`, `free`.
-        :param pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGroupDefinitionWidgetArgs']]] widgets: The list of widgets to display on the dashboard.
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         pulumi.set(__self__, "layout_type", layout_type)
         pulumi.set(__self__, "widgets", widgets)
         if background_color is not None:
             pulumi.set(__self__, "background_color", background_color)
         if banner_img is not None:
             pulumi.set(__self__, "banner_img", banner_img)
         if show_title is not None:
             pulumi.set(__self__, "show_title", show_title)
         if title is not None:
             pulumi.set(__self__, "title", title)
 
     @property
     @pulumi.getter(name="layoutType")
     def layout_type(self) -> pulumi.Input[str]:
-        """
-        The layout type of the dashboard. Valid values are `ordered`, `free`.
-        """
         return pulumi.get(self, "layout_type")
 
     @layout_type.setter
     def layout_type(self, value: pulumi.Input[str]):
         pulumi.set(self, "layout_type", value)
 
     @property
     @pulumi.getter
     def widgets(self) -> pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGroupDefinitionWidgetArgs']]]:
-        """
-        The list of widgets to display on the dashboard.
-        """
         return pulumi.get(self, "widgets")
 
     @widgets.setter
     def widgets(self, value: pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGroupDefinitionWidgetArgs']]]):
         pulumi.set(self, "widgets", value)
 
     @property
@@ -7707,17 +7474,14 @@
     @show_title.setter
     def show_title(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "show_title", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
 
@@ -7748,44 +7512,14 @@
                  servicemap_definition: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetServicemapDefinitionArgs']] = None,
                  sunburst_definition: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetSunburstDefinitionArgs']] = None,
                  timeseries_definition: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetTimeseriesDefinitionArgs']] = None,
                  toplist_definition: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetToplistDefinitionArgs']] = None,
                  trace_service_definition: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetTraceServiceDefinitionArgs']] = None,
                  treemap_definition: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetTreemapDefinitionArgs']] = None,
                  widget_layout: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetWidgetLayoutArgs']] = None):
-        """
-        :param pulumi.Input['DashboardWidgetGroupDefinitionWidgetAlertGraphDefinitionArgs'] alert_graph_definition: The definition for a Alert Graph widget.
-        :param pulumi.Input['DashboardWidgetGroupDefinitionWidgetAlertValueDefinitionArgs'] alert_value_definition: The definition for a Alert Value widget.
-        :param pulumi.Input['DashboardWidgetGroupDefinitionWidgetChangeDefinitionArgs'] change_definition: The definition for a Change widget.
-        :param pulumi.Input['DashboardWidgetGroupDefinitionWidgetCheckStatusDefinitionArgs'] check_status_definition: The definition for a Check Status widget.
-        :param pulumi.Input['DashboardWidgetGroupDefinitionWidgetDistributionDefinitionArgs'] distribution_definition: The definition for a Distribution widget.
-        :param pulumi.Input['DashboardWidgetGroupDefinitionWidgetEventStreamDefinitionArgs'] event_stream_definition: The definition for a Event Stream widget.
-        :param pulumi.Input['DashboardWidgetGroupDefinitionWidgetEventTimelineDefinitionArgs'] event_timeline_definition: The definition for a Event Timeline widget.
-        :param pulumi.Input['DashboardWidgetGroupDefinitionWidgetFreeTextDefinitionArgs'] free_text_definition: The definition for a Free Text widget.
-        :param pulumi.Input['DashboardWidgetGroupDefinitionWidgetGeomapDefinitionArgs'] geomap_definition: The definition for a Geomap widget.
-        :param pulumi.Input['DashboardWidgetGroupDefinitionWidgetHeatmapDefinitionArgs'] heatmap_definition: The definition for a Heatmap widget.
-        :param pulumi.Input['DashboardWidgetGroupDefinitionWidgetHostmapDefinitionArgs'] hostmap_definition: The definition for a Hostmap widget.
-        :param pulumi.Input[int] id: The ID of the widget.
-        :param pulumi.Input['DashboardWidgetGroupDefinitionWidgetIframeDefinitionArgs'] iframe_definition: The definition for an Iframe widget.
-        :param pulumi.Input['DashboardWidgetGroupDefinitionWidgetImageDefinitionArgs'] image_definition: The definition for an Image widget
-        :param pulumi.Input['DashboardWidgetGroupDefinitionWidgetLogStreamDefinitionArgs'] log_stream_definition: The definition for an Log Stream widget.
-        :param pulumi.Input['DashboardWidgetGroupDefinitionWidgetManageStatusDefinitionArgs'] manage_status_definition: The definition for an Manage Status widget.
-        :param pulumi.Input['DashboardWidgetGroupDefinitionWidgetNoteDefinitionArgs'] note_definition: The definition for a Note widget.
-        :param pulumi.Input['DashboardWidgetGroupDefinitionWidgetQueryTableDefinitionArgs'] query_table_definition: The definition for a Query Table widget.
-        :param pulumi.Input['DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionArgs'] query_value_definition: The definition for a Query Value widget.
-        :param pulumi.Input['DashboardWidgetGroupDefinitionWidgetScatterplotDefinitionArgs'] scatterplot_definition: The definition for a Scatterplot widget.
-        :param pulumi.Input['DashboardWidgetGroupDefinitionWidgetServiceLevelObjectiveDefinitionArgs'] service_level_objective_definition: The definition for a Service Level Objective widget.
-        :param pulumi.Input['DashboardWidgetGroupDefinitionWidgetServicemapDefinitionArgs'] servicemap_definition: The definition for a Service Map widget.
-        :param pulumi.Input['DashboardWidgetGroupDefinitionWidgetSunburstDefinitionArgs'] sunburst_definition: The definition for a Sunburst widget.
-        :param pulumi.Input['DashboardWidgetGroupDefinitionWidgetTimeseriesDefinitionArgs'] timeseries_definition: The definition for a Timeseries widget.
-        :param pulumi.Input['DashboardWidgetGroupDefinitionWidgetToplistDefinitionArgs'] toplist_definition: The definition for a Toplist widget.
-        :param pulumi.Input['DashboardWidgetGroupDefinitionWidgetTraceServiceDefinitionArgs'] trace_service_definition: The definition for a Trace Service widget.
-        :param pulumi.Input['DashboardWidgetGroupDefinitionWidgetTreemapDefinitionArgs'] treemap_definition: The definition for a Treemap widget.
-        :param pulumi.Input['DashboardWidgetGroupDefinitionWidgetWidgetLayoutArgs'] widget_layout: The layout of the widget on a 'free' dashboard.
-        """
         if alert_graph_definition is not None:
             pulumi.set(__self__, "alert_graph_definition", alert_graph_definition)
         if alert_value_definition is not None:
             pulumi.set(__self__, "alert_value_definition", alert_value_definition)
         if change_definition is not None:
             pulumi.set(__self__, "change_definition", change_definition)
         if check_status_definition is not None:
@@ -7838,341 +7572,257 @@
             pulumi.set(__self__, "treemap_definition", treemap_definition)
         if widget_layout is not None:
             pulumi.set(__self__, "widget_layout", widget_layout)
 
     @property
     @pulumi.getter(name="alertGraphDefinition")
     def alert_graph_definition(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetAlertGraphDefinitionArgs']]:
-        """
-        The definition for a Alert Graph widget.
-        """
         return pulumi.get(self, "alert_graph_definition")
 
     @alert_graph_definition.setter
     def alert_graph_definition(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetAlertGraphDefinitionArgs']]):
         pulumi.set(self, "alert_graph_definition", value)
 
     @property
     @pulumi.getter(name="alertValueDefinition")
     def alert_value_definition(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetAlertValueDefinitionArgs']]:
-        """
-        The definition for a Alert Value widget.
-        """
         return pulumi.get(self, "alert_value_definition")
 
     @alert_value_definition.setter
     def alert_value_definition(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetAlertValueDefinitionArgs']]):
         pulumi.set(self, "alert_value_definition", value)
 
     @property
     @pulumi.getter(name="changeDefinition")
     def change_definition(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetChangeDefinitionArgs']]:
-        """
-        The definition for a Change widget.
-        """
         return pulumi.get(self, "change_definition")
 
     @change_definition.setter
     def change_definition(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetChangeDefinitionArgs']]):
         pulumi.set(self, "change_definition", value)
 
     @property
     @pulumi.getter(name="checkStatusDefinition")
     def check_status_definition(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetCheckStatusDefinitionArgs']]:
-        """
-        The definition for a Check Status widget.
-        """
         return pulumi.get(self, "check_status_definition")
 
     @check_status_definition.setter
     def check_status_definition(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetCheckStatusDefinitionArgs']]):
         pulumi.set(self, "check_status_definition", value)
 
     @property
     @pulumi.getter(name="distributionDefinition")
     def distribution_definition(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetDistributionDefinitionArgs']]:
-        """
-        The definition for a Distribution widget.
-        """
         return pulumi.get(self, "distribution_definition")
 
     @distribution_definition.setter
     def distribution_definition(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetDistributionDefinitionArgs']]):
         pulumi.set(self, "distribution_definition", value)
 
     @property
     @pulumi.getter(name="eventStreamDefinition")
     def event_stream_definition(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetEventStreamDefinitionArgs']]:
-        """
-        The definition for a Event Stream widget.
-        """
         return pulumi.get(self, "event_stream_definition")
 
     @event_stream_definition.setter
     def event_stream_definition(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetEventStreamDefinitionArgs']]):
         pulumi.set(self, "event_stream_definition", value)
 
     @property
     @pulumi.getter(name="eventTimelineDefinition")
     def event_timeline_definition(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetEventTimelineDefinitionArgs']]:
-        """
-        The definition for a Event Timeline widget.
-        """
         return pulumi.get(self, "event_timeline_definition")
 
     @event_timeline_definition.setter
     def event_timeline_definition(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetEventTimelineDefinitionArgs']]):
         pulumi.set(self, "event_timeline_definition", value)
 
     @property
     @pulumi.getter(name="freeTextDefinition")
     def free_text_definition(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetFreeTextDefinitionArgs']]:
-        """
-        The definition for a Free Text widget.
-        """
         return pulumi.get(self, "free_text_definition")
 
     @free_text_definition.setter
     def free_text_definition(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetFreeTextDefinitionArgs']]):
         pulumi.set(self, "free_text_definition", value)
 
     @property
     @pulumi.getter(name="geomapDefinition")
     def geomap_definition(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetGeomapDefinitionArgs']]:
-        """
-        The definition for a Geomap widget.
-        """
         return pulumi.get(self, "geomap_definition")
 
     @geomap_definition.setter
     def geomap_definition(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetGeomapDefinitionArgs']]):
         pulumi.set(self, "geomap_definition", value)
 
     @property
     @pulumi.getter(name="heatmapDefinition")
     def heatmap_definition(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetHeatmapDefinitionArgs']]:
-        """
-        The definition for a Heatmap widget.
-        """
         return pulumi.get(self, "heatmap_definition")
 
     @heatmap_definition.setter
     def heatmap_definition(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetHeatmapDefinitionArgs']]):
         pulumi.set(self, "heatmap_definition", value)
 
     @property
     @pulumi.getter(name="hostmapDefinition")
     def hostmap_definition(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetHostmapDefinitionArgs']]:
-        """
-        The definition for a Hostmap widget.
-        """
         return pulumi.get(self, "hostmap_definition")
 
     @hostmap_definition.setter
     def hostmap_definition(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetHostmapDefinitionArgs']]):
         pulumi.set(self, "hostmap_definition", value)
 
     @property
     @pulumi.getter
     def id(self) -> Optional[pulumi.Input[int]]:
-        """
-        The ID of the widget.
-        """
         return pulumi.get(self, "id")
 
     @id.setter
     def id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "id", value)
 
     @property
     @pulumi.getter(name="iframeDefinition")
     def iframe_definition(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetIframeDefinitionArgs']]:
-        """
-        The definition for an Iframe widget.
-        """
         return pulumi.get(self, "iframe_definition")
 
     @iframe_definition.setter
     def iframe_definition(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetIframeDefinitionArgs']]):
         pulumi.set(self, "iframe_definition", value)
 
     @property
     @pulumi.getter(name="imageDefinition")
     def image_definition(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetImageDefinitionArgs']]:
-        """
-        The definition for an Image widget
-        """
         return pulumi.get(self, "image_definition")
 
     @image_definition.setter
     def image_definition(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetImageDefinitionArgs']]):
         pulumi.set(self, "image_definition", value)
 
     @property
     @pulumi.getter(name="logStreamDefinition")
     def log_stream_definition(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetLogStreamDefinitionArgs']]:
-        """
-        The definition for an Log Stream widget.
-        """
         return pulumi.get(self, "log_stream_definition")
 
     @log_stream_definition.setter
     def log_stream_definition(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetLogStreamDefinitionArgs']]):
         pulumi.set(self, "log_stream_definition", value)
 
     @property
     @pulumi.getter(name="manageStatusDefinition")
     def manage_status_definition(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetManageStatusDefinitionArgs']]:
-        """
-        The definition for an Manage Status widget.
-        """
         return pulumi.get(self, "manage_status_definition")
 
     @manage_status_definition.setter
     def manage_status_definition(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetManageStatusDefinitionArgs']]):
         pulumi.set(self, "manage_status_definition", value)
 
     @property
     @pulumi.getter(name="noteDefinition")
     def note_definition(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetNoteDefinitionArgs']]:
-        """
-        The definition for a Note widget.
-        """
         return pulumi.get(self, "note_definition")
 
     @note_definition.setter
     def note_definition(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetNoteDefinitionArgs']]):
         pulumi.set(self, "note_definition", value)
 
     @property
     @pulumi.getter(name="queryTableDefinition")
     def query_table_definition(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetQueryTableDefinitionArgs']]:
-        """
-        The definition for a Query Table widget.
-        """
         return pulumi.get(self, "query_table_definition")
 
     @query_table_definition.setter
     def query_table_definition(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetQueryTableDefinitionArgs']]):
         pulumi.set(self, "query_table_definition", value)
 
     @property
     @pulumi.getter(name="queryValueDefinition")
     def query_value_definition(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionArgs']]:
-        """
-        The definition for a Query Value widget.
-        """
         return pulumi.get(self, "query_value_definition")
 
     @query_value_definition.setter
     def query_value_definition(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionArgs']]):
         pulumi.set(self, "query_value_definition", value)
 
     @property
     @pulumi.getter(name="scatterplotDefinition")
     def scatterplot_definition(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetScatterplotDefinitionArgs']]:
-        """
-        The definition for a Scatterplot widget.
-        """
         return pulumi.get(self, "scatterplot_definition")
 
     @scatterplot_definition.setter
     def scatterplot_definition(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetScatterplotDefinitionArgs']]):
         pulumi.set(self, "scatterplot_definition", value)
 
     @property
     @pulumi.getter(name="serviceLevelObjectiveDefinition")
     def service_level_objective_definition(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetServiceLevelObjectiveDefinitionArgs']]:
-        """
-        The definition for a Service Level Objective widget.
-        """
         return pulumi.get(self, "service_level_objective_definition")
 
     @service_level_objective_definition.setter
     def service_level_objective_definition(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetServiceLevelObjectiveDefinitionArgs']]):
         pulumi.set(self, "service_level_objective_definition", value)
 
     @property
     @pulumi.getter(name="servicemapDefinition")
     def servicemap_definition(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetServicemapDefinitionArgs']]:
-        """
-        The definition for a Service Map widget.
-        """
         return pulumi.get(self, "servicemap_definition")
 
     @servicemap_definition.setter
     def servicemap_definition(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetServicemapDefinitionArgs']]):
         pulumi.set(self, "servicemap_definition", value)
 
     @property
     @pulumi.getter(name="sunburstDefinition")
     def sunburst_definition(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetSunburstDefinitionArgs']]:
-        """
-        The definition for a Sunburst widget.
-        """
         return pulumi.get(self, "sunburst_definition")
 
     @sunburst_definition.setter
     def sunburst_definition(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetSunburstDefinitionArgs']]):
         pulumi.set(self, "sunburst_definition", value)
 
     @property
     @pulumi.getter(name="timeseriesDefinition")
     def timeseries_definition(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetTimeseriesDefinitionArgs']]:
-        """
-        The definition for a Timeseries widget.
-        """
         return pulumi.get(self, "timeseries_definition")
 
     @timeseries_definition.setter
     def timeseries_definition(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetTimeseriesDefinitionArgs']]):
         pulumi.set(self, "timeseries_definition", value)
 
     @property
     @pulumi.getter(name="toplistDefinition")
     def toplist_definition(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetToplistDefinitionArgs']]:
-        """
-        The definition for a Toplist widget.
-        """
         return pulumi.get(self, "toplist_definition")
 
     @toplist_definition.setter
     def toplist_definition(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetToplistDefinitionArgs']]):
         pulumi.set(self, "toplist_definition", value)
 
     @property
     @pulumi.getter(name="traceServiceDefinition")
     def trace_service_definition(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetTraceServiceDefinitionArgs']]:
-        """
-        The definition for a Trace Service widget.
-        """
         return pulumi.get(self, "trace_service_definition")
 
     @trace_service_definition.setter
     def trace_service_definition(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetTraceServiceDefinitionArgs']]):
         pulumi.set(self, "trace_service_definition", value)
 
     @property
     @pulumi.getter(name="treemapDefinition")
     def treemap_definition(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetTreemapDefinitionArgs']]:
-        """
-        The definition for a Treemap widget.
-        """
         return pulumi.get(self, "treemap_definition")
 
     @treemap_definition.setter
     def treemap_definition(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetTreemapDefinitionArgs']]):
         pulumi.set(self, "treemap_definition", value)
 
     @property
     @pulumi.getter(name="widgetLayout")
     def widget_layout(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetWidgetLayoutArgs']]:
-        """
-        The layout of the widget on a 'free' dashboard.
-        """
         return pulumi.get(self, "widget_layout")
 
     @widget_layout.setter
     def widget_layout(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetWidgetLayoutArgs']]):
         pulumi.set(self, "widget_layout", value)
 
 
@@ -8181,17 +7831,14 @@
     def __init__(__self__, *,
                  alert_id: pulumi.Input[str],
                  viz_type: pulumi.Input[str],
                  live_span: Optional[pulumi.Input[str]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         pulumi.set(__self__, "alert_id", alert_id)
         pulumi.set(__self__, "viz_type", viz_type)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if title is not None:
             pulumi.set(__self__, "title", title)
         if title_align is not None:
@@ -8225,17 +7872,14 @@
     @live_span.setter
     def live_span(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "live_span", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -8263,17 +7907,14 @@
                  alert_id: pulumi.Input[str],
                  precision: Optional[pulumi.Input[int]] = None,
                  text_align: Optional[pulumi.Input[str]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None,
                  unit: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         pulumi.set(__self__, "alert_id", alert_id)
         if precision is not None:
             pulumi.set(__self__, "precision", precision)
         if text_align is not None:
             pulumi.set(__self__, "text_align", text_align)
         if title is not None:
             pulumi.set(__self__, "title", title)
@@ -8310,17 +7951,14 @@
     @text_align.setter
     def text_align(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "text_align", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -8356,17 +7994,14 @@
     def __init__(__self__, *,
                  custom_links: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGroupDefinitionWidgetChangeDefinitionCustomLinkArgs']]]] = None,
                  live_span: Optional[pulumi.Input[str]] = None,
                  requests: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGroupDefinitionWidgetChangeDefinitionRequestArgs']]]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if requests is not None:
             pulumi.set(__self__, "requests", requests)
         if title is not None:
@@ -8402,17 +8037,14 @@
     @requests.setter
     def requests(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGroupDefinitionWidgetChangeDefinitionRequestArgs']]]]):
         pulumi.set(self, "requests", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -10493,17 +10125,14 @@
                  group: Optional[pulumi.Input[str]] = None,
                  group_bies: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  live_span: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         pulumi.set(__self__, "check", check)
         pulumi.set(__self__, "grouping", grouping)
         if group is not None:
             pulumi.set(__self__, "group", group)
         if group_bies is not None:
             pulumi.set(__self__, "group_bies", group_bies)
         if live_span is not None:
@@ -10570,17 +10199,14 @@
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -10608,17 +10234,14 @@
                  legend_size: Optional[pulumi.Input[str]] = None,
                  live_span: Optional[pulumi.Input[str]] = None,
                  requests: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGroupDefinitionWidgetDistributionDefinitionRequestArgs']]]] = None,
                  show_legend: Optional[pulumi.Input[bool]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         if legend_size is not None:
             pulumi.set(__self__, "legend_size", legend_size)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if requests is not None:
             pulumi.set(__self__, "requests", requests)
         if show_legend is not None:
@@ -10665,17 +10288,14 @@
     @show_legend.setter
     def show_legend(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "show_legend", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -11905,17 +11525,14 @@
                  query: pulumi.Input[str],
                  event_size: Optional[pulumi.Input[str]] = None,
                  live_span: Optional[pulumi.Input[str]] = None,
                  tags_execution: Optional[pulumi.Input[str]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         pulumi.set(__self__, "query", query)
         if event_size is not None:
             pulumi.set(__self__, "event_size", event_size)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if tags_execution is not None:
             pulumi.set(__self__, "tags_execution", tags_execution)
@@ -11961,17 +11578,14 @@
     @tags_execution.setter
     def tags_execution(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "tags_execution", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -11998,17 +11612,14 @@
     def __init__(__self__, *,
                  query: pulumi.Input[str],
                  live_span: Optional[pulumi.Input[str]] = None,
                  tags_execution: Optional[pulumi.Input[str]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         pulumi.set(__self__, "query", query)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if tags_execution is not None:
             pulumi.set(__self__, "tags_execution", tags_execution)
         if title is not None:
             pulumi.set(__self__, "title", title)
@@ -12043,17 +11654,14 @@
     @tags_execution.setter
     def tags_execution(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "tags_execution", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -12134,17 +11742,14 @@
                  custom_links: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGroupDefinitionWidgetGeomapDefinitionCustomLinkArgs']]]] = None,
                  live_span: Optional[pulumi.Input[str]] = None,
                  requests: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGroupDefinitionWidgetGeomapDefinitionRequestArgs']]]] = None,
                  style: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetGeomapDefinitionStyleArgs']] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         pulumi.set(__self__, "view", view)
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if requests is not None:
             pulumi.set(__self__, "requests", requests)
@@ -12201,17 +11806,14 @@
     @style.setter
     def style(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetGeomapDefinitionStyleArgs']]):
         pulumi.set(self, "style", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -13728,17 +13330,14 @@
                  live_span: Optional[pulumi.Input[str]] = None,
                  requests: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGroupDefinitionWidgetHeatmapDefinitionRequestArgs']]]] = None,
                  show_legend: Optional[pulumi.Input[bool]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None,
                  yaxis: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetHeatmapDefinitionYaxisArgs']] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if events is not None:
             pulumi.set(__self__, "events", events)
         if legend_size is not None:
             pulumi.set(__self__, "legend_size", legend_size)
         if live_span is not None:
@@ -13809,17 +13408,14 @@
     @show_legend.setter
     def show_legend(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "show_legend", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -15060,17 +14656,14 @@
                  node_type: Optional[pulumi.Input[str]] = None,
                  request: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetHostmapDefinitionRequestArgs']] = None,
                  scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  style: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetHostmapDefinitionStyleArgs']] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if groups is not None:
             pulumi.set(__self__, "groups", groups)
         if no_group_hosts is not None:
             pulumi.set(__self__, "no_group_hosts", no_group_hosts)
         if no_metric_hosts is not None:
@@ -15161,17 +14754,14 @@
     @style.setter
     def style(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetHostmapDefinitionStyleArgs']]):
         pulumi.set(self, "style", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -17378,25 +16968,19 @@
         pulumi.set(self, "palette_flip", value)
 
 
 @pulumi.input_type
 class DashboardWidgetGroupDefinitionWidgetIframeDefinitionArgs:
     def __init__(__self__, *,
                  url: pulumi.Input[str]):
-        """
-        :param pulumi.Input[str] url: The URL of the dashboard.
-        """
         pulumi.set(__self__, "url", url)
 
     @property
     @pulumi.getter
     def url(self) -> pulumi.Input[str]:
-        """
-        The URL of the dashboard.
-        """
         return pulumi.get(self, "url")
 
     @url.setter
     def url(self, value: pulumi.Input[str]):
         pulumi.set(self, "url", value)
 
 
@@ -17407,17 +16991,14 @@
                  has_background: Optional[pulumi.Input[bool]] = None,
                  has_border: Optional[pulumi.Input[bool]] = None,
                  horizontal_align: Optional[pulumi.Input[str]] = None,
                  margin: Optional[pulumi.Input[str]] = None,
                  sizing: Optional[pulumi.Input[str]] = None,
                  url_dark_theme: Optional[pulumi.Input[str]] = None,
                  vertical_align: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] url: The URL of the dashboard.
-        """
         pulumi.set(__self__, "url", url)
         if has_background is not None:
             pulumi.set(__self__, "has_background", has_background)
         if has_border is not None:
             pulumi.set(__self__, "has_border", has_border)
         if horizontal_align is not None:
             pulumi.set(__self__, "horizontal_align", horizontal_align)
@@ -17429,17 +17010,14 @@
             pulumi.set(__self__, "url_dark_theme", url_dark_theme)
         if vertical_align is not None:
             pulumi.set(__self__, "vertical_align", vertical_align)
 
     @property
     @pulumi.getter
     def url(self) -> pulumi.Input[str]:
-        """
-        The URL of the dashboard.
-        """
         return pulumi.get(self, "url")
 
     @url.setter
     def url(self, value: pulumi.Input[str]):
         pulumi.set(self, "url", value)
 
     @property
@@ -17516,17 +17094,14 @@
                  query: Optional[pulumi.Input[str]] = None,
                  show_date_column: Optional[pulumi.Input[bool]] = None,
                  show_message_column: Optional[pulumi.Input[bool]] = None,
                  sort: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetLogStreamDefinitionSortArgs']] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         if columns is not None:
             pulumi.set(__self__, "columns", columns)
         if indexes is not None:
             pulumi.set(__self__, "indexes", indexes)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if message_display is not None:
@@ -17617,17 +17192,14 @@
     @sort.setter
     def sort(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetLogStreamDefinitionSortArgs']]):
         pulumi.set(self, "sort", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -17685,17 +17257,14 @@
                  hide_zero_counts: Optional[pulumi.Input[bool]] = None,
                  show_last_triggered: Optional[pulumi.Input[bool]] = None,
                  sort: Optional[pulumi.Input[str]] = None,
                  summary_type: Optional[pulumi.Input[str]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         pulumi.set(__self__, "query", query)
         if color_preference is not None:
             pulumi.set(__self__, "color_preference", color_preference)
         if display_format is not None:
             pulumi.set(__self__, "display_format", display_format)
         if hide_zero_counts is not None:
             pulumi.set(__self__, "hide_zero_counts", hide_zero_counts)
@@ -17774,17 +17343,14 @@
     @summary_type.setter
     def summary_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "summary_type", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -17924,17 +17490,14 @@
                  custom_links: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGroupDefinitionWidgetQueryTableDefinitionCustomLinkArgs']]]] = None,
                  has_search_bar: Optional[pulumi.Input[str]] = None,
                  live_span: Optional[pulumi.Input[str]] = None,
                  requests: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGroupDefinitionWidgetQueryTableDefinitionRequestArgs']]]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if has_search_bar is not None:
             pulumi.set(__self__, "has_search_bar", has_search_bar)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if requests is not None:
@@ -17981,17 +17544,14 @@
     @requests.setter
     def requests(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGroupDefinitionWidgetQueryTableDefinitionRequestArgs']]]]):
         pulumi.set(self, "requests", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -20328,34 +19888,34 @@
                  autoscale: Optional[pulumi.Input[bool]] = None,
                  custom_links: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionCustomLinkArgs']]]] = None,
                  custom_unit: Optional[pulumi.Input[str]] = None,
                  live_span: Optional[pulumi.Input[str]] = None,
                  precision: Optional[pulumi.Input[int]] = None,
                  requests: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionRequestArgs']]]] = None,
                  text_align: Optional[pulumi.Input[str]] = None,
+                 timeseries_background: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionTimeseriesBackgroundArgs']] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         if autoscale is not None:
             pulumi.set(__self__, "autoscale", autoscale)
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if custom_unit is not None:
             pulumi.set(__self__, "custom_unit", custom_unit)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if precision is not None:
             pulumi.set(__self__, "precision", precision)
         if requests is not None:
             pulumi.set(__self__, "requests", requests)
         if text_align is not None:
             pulumi.set(__self__, "text_align", text_align)
+        if timeseries_background is not None:
+            pulumi.set(__self__, "timeseries_background", timeseries_background)
         if title is not None:
             pulumi.set(__self__, "title", title)
         if title_align is not None:
             pulumi.set(__self__, "title_align", title_align)
         if title_size is not None:
             pulumi.set(__self__, "title_size", title_size)
 
@@ -20419,19 +19979,25 @@
         return pulumi.get(self, "text_align")
 
     @text_align.setter
     def text_align(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "text_align", value)
 
     @property
+    @pulumi.getter(name="timeseriesBackground")
+    def timeseries_background(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionTimeseriesBackgroundArgs']]:
+        return pulumi.get(self, "timeseries_background")
+
+    @timeseries_background.setter
+    def timeseries_background(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionTimeseriesBackgroundArgs']]):
+        pulumi.set(self, "timeseries_background", value)
+
+    @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -22799,28 +22365,118 @@
 
     @interval.setter
     def interval(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "interval", value)
 
 
 @pulumi.input_type
+class DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionTimeseriesBackgroundArgs:
+    def __init__(__self__, *,
+                 type: pulumi.Input[str],
+                 yaxis: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionTimeseriesBackgroundYaxisArgs']] = None):
+        pulumi.set(__self__, "type", type)
+        if yaxis is not None:
+            pulumi.set(__self__, "yaxis", yaxis)
+
+    @property
+    @pulumi.getter
+    def type(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "type")
+
+    @type.setter
+    def type(self, value: pulumi.Input[str]):
+        pulumi.set(self, "type", value)
+
+    @property
+    @pulumi.getter
+    def yaxis(self) -> Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionTimeseriesBackgroundYaxisArgs']]:
+        return pulumi.get(self, "yaxis")
+
+    @yaxis.setter
+    def yaxis(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionTimeseriesBackgroundYaxisArgs']]):
+        pulumi.set(self, "yaxis", value)
+
+
+@pulumi.input_type
+class DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionTimeseriesBackgroundYaxisArgs:
+    def __init__(__self__, *,
+                 include_zero: Optional[pulumi.Input[bool]] = None,
+                 label: Optional[pulumi.Input[str]] = None,
+                 max: Optional[pulumi.Input[str]] = None,
+                 min: Optional[pulumi.Input[str]] = None,
+                 scale: Optional[pulumi.Input[str]] = None):
+        if include_zero is not None:
+            pulumi.set(__self__, "include_zero", include_zero)
+        if label is not None:
+            pulumi.set(__self__, "label", label)
+        if max is not None:
+            pulumi.set(__self__, "max", max)
+        if min is not None:
+            pulumi.set(__self__, "min", min)
+        if scale is not None:
+            pulumi.set(__self__, "scale", scale)
+
+    @property
+    @pulumi.getter(name="includeZero")
+    def include_zero(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "include_zero")
+
+    @include_zero.setter
+    def include_zero(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "include_zero", value)
+
+    @property
+    @pulumi.getter
+    def label(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "label")
+
+    @label.setter
+    def label(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "label", value)
+
+    @property
+    @pulumi.getter
+    def max(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "max")
+
+    @max.setter
+    def max(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "max", value)
+
+    @property
+    @pulumi.getter
+    def min(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "min")
+
+    @min.setter
+    def min(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "min", value)
+
+    @property
+    @pulumi.getter
+    def scale(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "scale")
+
+    @scale.setter
+    def scale(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "scale", value)
+
+
+@pulumi.input_type
 class DashboardWidgetGroupDefinitionWidgetScatterplotDefinitionArgs:
     def __init__(__self__, *,
                  color_by_groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  custom_links: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGroupDefinitionWidgetScatterplotDefinitionCustomLinkArgs']]]] = None,
                  live_span: Optional[pulumi.Input[str]] = None,
                  request: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetScatterplotDefinitionRequestArgs']] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None,
                  xaxis: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetScatterplotDefinitionXaxisArgs']] = None,
                  yaxis: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetScatterplotDefinitionYaxisArgs']] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         if color_by_groups is not None:
             pulumi.set(__self__, "color_by_groups", color_by_groups)
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if request is not None:
@@ -22871,17 +22527,14 @@
     @request.setter
     def request(self, value: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetScatterplotDefinitionRequestArgs']]):
         pulumi.set(self, "request", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -25969,17 +25622,14 @@
                  view_mode: pulumi.Input[str],
                  view_type: pulumi.Input[str],
                  global_time_target: Optional[pulumi.Input[str]] = None,
                  show_error_budget: Optional[pulumi.Input[bool]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         pulumi.set(__self__, "slo_id", slo_id)
         pulumi.set(__self__, "time_windows", time_windows)
         pulumi.set(__self__, "view_mode", view_mode)
         pulumi.set(__self__, "view_type", view_type)
         if global_time_target is not None:
             pulumi.set(__self__, "global_time_target", global_time_target)
         if show_error_budget is not None:
@@ -26044,17 +25694,14 @@
     @show_error_budget.setter
     def show_error_budget(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "show_error_budget", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -26081,17 +25728,14 @@
     def __init__(__self__, *,
                  filters: pulumi.Input[Sequence[pulumi.Input[str]]],
                  service: pulumi.Input[str],
                  custom_links: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGroupDefinitionWidgetServicemapDefinitionCustomLinkArgs']]]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         pulumi.set(__self__, "filters", filters)
         pulumi.set(__self__, "service", service)
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if title is not None:
             pulumi.set(__self__, "title", title)
         if title_align is not None:
@@ -26125,17 +25769,14 @@
     @custom_links.setter
     def custom_links(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGroupDefinitionWidgetServicemapDefinitionCustomLinkArgs']]]]):
         pulumi.set(self, "custom_links", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -26218,17 +25859,14 @@
                  legend_inline: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetSunburstDefinitionLegendInlineArgs']] = None,
                  legend_table: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetSunburstDefinitionLegendTableArgs']] = None,
                  live_span: Optional[pulumi.Input[str]] = None,
                  requests: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGroupDefinitionWidgetSunburstDefinitionRequestArgs']]]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if hide_total is not None:
             pulumi.set(__self__, "hide_total", hide_total)
         if legend_inline is not None:
             pulumi.set(__self__, "legend_inline", legend_inline)
         if legend_table is not None:
@@ -26297,17 +25935,14 @@
     @requests.setter
     def requests(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGroupDefinitionWidgetSunburstDefinitionRequestArgs']]]]):
         pulumi.set(self, "requests", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -28849,17 +28484,14 @@
                  requests: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGroupDefinitionWidgetTimeseriesDefinitionRequestArgs']]]] = None,
                  right_yaxis: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetTimeseriesDefinitionRightYaxisArgs']] = None,
                  show_legend: Optional[pulumi.Input[bool]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None,
                  yaxis: Optional[pulumi.Input['DashboardWidgetGroupDefinitionWidgetTimeseriesDefinitionYaxisArgs']] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if events is not None:
             pulumi.set(__self__, "events", events)
         if legend_columns is not None:
             pulumi.set(__self__, "legend_columns", legend_columns)
         if legend_layout is not None:
@@ -28974,17 +28606,14 @@
     @show_legend.setter
     def show_legend(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "show_legend", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -31786,17 +31415,14 @@
     def __init__(__self__, *,
                  custom_links: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGroupDefinitionWidgetToplistDefinitionCustomLinkArgs']]]] = None,
                  live_span: Optional[pulumi.Input[str]] = None,
                  requests: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGroupDefinitionWidgetToplistDefinitionRequestArgs']]]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if requests is not None:
             pulumi.set(__self__, "requests", requests)
         if title is not None:
@@ -31832,17 +31458,14 @@
     @requests.setter
     def requests(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGroupDefinitionWidgetToplistDefinitionRequestArgs']]]]):
         pulumi.set(self, "requests", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -34244,17 +33867,14 @@
                  show_hits: Optional[pulumi.Input[bool]] = None,
                  show_latency: Optional[pulumi.Input[bool]] = None,
                  show_resource_list: Optional[pulumi.Input[bool]] = None,
                  size_format: Optional[pulumi.Input[str]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         pulumi.set(__self__, "env", env)
         pulumi.set(__self__, "service", service)
         pulumi.set(__self__, "span_name", span_name)
         if display_format is not None:
             pulumi.set(__self__, "display_format", display_format)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
@@ -34386,17 +34006,14 @@
     @size_format.setter
     def size_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "size_format", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -34419,17 +34036,14 @@
 
 
 @pulumi.input_type
 class DashboardWidgetGroupDefinitionWidgetTreemapDefinitionArgs:
     def __init__(__self__, *,
                  requests: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGroupDefinitionWidgetTreemapDefinitionRequestArgs']]]] = None,
                  title: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         if requests is not None:
             pulumi.set(__self__, "requests", requests)
         if title is not None:
             pulumi.set(__self__, "title", title)
 
     @property
     @pulumi.getter
@@ -34439,17 +34053,14 @@
     @requests.setter
     def requests(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetGroupDefinitionWidgetTreemapDefinitionRequestArgs']]]]):
         pulumi.set(self, "requests", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
 
@@ -35429,17 +35040,14 @@
                  live_span: Optional[pulumi.Input[str]] = None,
                  requests: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetHeatmapDefinitionRequestArgs']]]] = None,
                  show_legend: Optional[pulumi.Input[bool]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None,
                  yaxis: Optional[pulumi.Input['DashboardWidgetHeatmapDefinitionYaxisArgs']] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if events is not None:
             pulumi.set(__self__, "events", events)
         if legend_size is not None:
             pulumi.set(__self__, "legend_size", legend_size)
         if live_span is not None:
@@ -35510,17 +35118,14 @@
     @show_legend.setter
     def show_legend(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "show_legend", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -36761,17 +36366,14 @@
                  node_type: Optional[pulumi.Input[str]] = None,
                  request: Optional[pulumi.Input['DashboardWidgetHostmapDefinitionRequestArgs']] = None,
                  scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  style: Optional[pulumi.Input['DashboardWidgetHostmapDefinitionStyleArgs']] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if groups is not None:
             pulumi.set(__self__, "groups", groups)
         if no_group_hosts is not None:
             pulumi.set(__self__, "no_group_hosts", no_group_hosts)
         if no_metric_hosts is not None:
@@ -36862,17 +36464,14 @@
     @style.setter
     def style(self, value: Optional[pulumi.Input['DashboardWidgetHostmapDefinitionStyleArgs']]):
         pulumi.set(self, "style", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -39079,25 +38678,19 @@
         pulumi.set(self, "palette_flip", value)
 
 
 @pulumi.input_type
 class DashboardWidgetIframeDefinitionArgs:
     def __init__(__self__, *,
                  url: pulumi.Input[str]):
-        """
-        :param pulumi.Input[str] url: The URL of the dashboard.
-        """
         pulumi.set(__self__, "url", url)
 
     @property
     @pulumi.getter
     def url(self) -> pulumi.Input[str]:
-        """
-        The URL of the dashboard.
-        """
         return pulumi.get(self, "url")
 
     @url.setter
     def url(self, value: pulumi.Input[str]):
         pulumi.set(self, "url", value)
 
 
@@ -39108,17 +38701,14 @@
                  has_background: Optional[pulumi.Input[bool]] = None,
                  has_border: Optional[pulumi.Input[bool]] = None,
                  horizontal_align: Optional[pulumi.Input[str]] = None,
                  margin: Optional[pulumi.Input[str]] = None,
                  sizing: Optional[pulumi.Input[str]] = None,
                  url_dark_theme: Optional[pulumi.Input[str]] = None,
                  vertical_align: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] url: The URL of the dashboard.
-        """
         pulumi.set(__self__, "url", url)
         if has_background is not None:
             pulumi.set(__self__, "has_background", has_background)
         if has_border is not None:
             pulumi.set(__self__, "has_border", has_border)
         if horizontal_align is not None:
             pulumi.set(__self__, "horizontal_align", horizontal_align)
@@ -39130,17 +38720,14 @@
             pulumi.set(__self__, "url_dark_theme", url_dark_theme)
         if vertical_align is not None:
             pulumi.set(__self__, "vertical_align", vertical_align)
 
     @property
     @pulumi.getter
     def url(self) -> pulumi.Input[str]:
-        """
-        The URL of the dashboard.
-        """
         return pulumi.get(self, "url")
 
     @url.setter
     def url(self, value: pulumi.Input[str]):
         pulumi.set(self, "url", value)
 
     @property
@@ -39217,17 +38804,14 @@
                  query: Optional[pulumi.Input[str]] = None,
                  show_date_column: Optional[pulumi.Input[bool]] = None,
                  show_message_column: Optional[pulumi.Input[bool]] = None,
                  sort: Optional[pulumi.Input['DashboardWidgetLogStreamDefinitionSortArgs']] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         if columns is not None:
             pulumi.set(__self__, "columns", columns)
         if indexes is not None:
             pulumi.set(__self__, "indexes", indexes)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if message_display is not None:
@@ -39318,17 +38902,14 @@
     @sort.setter
     def sort(self, value: Optional[pulumi.Input['DashboardWidgetLogStreamDefinitionSortArgs']]):
         pulumi.set(self, "sort", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -39386,17 +38967,14 @@
                  hide_zero_counts: Optional[pulumi.Input[bool]] = None,
                  show_last_triggered: Optional[pulumi.Input[bool]] = None,
                  sort: Optional[pulumi.Input[str]] = None,
                  summary_type: Optional[pulumi.Input[str]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         pulumi.set(__self__, "query", query)
         if color_preference is not None:
             pulumi.set(__self__, "color_preference", color_preference)
         if display_format is not None:
             pulumi.set(__self__, "display_format", display_format)
         if hide_zero_counts is not None:
             pulumi.set(__self__, "hide_zero_counts", hide_zero_counts)
@@ -39475,17 +39053,14 @@
     @summary_type.setter
     def summary_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "summary_type", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -39625,17 +39200,14 @@
                  custom_links: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetQueryTableDefinitionCustomLinkArgs']]]] = None,
                  has_search_bar: Optional[pulumi.Input[str]] = None,
                  live_span: Optional[pulumi.Input[str]] = None,
                  requests: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetQueryTableDefinitionRequestArgs']]]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if has_search_bar is not None:
             pulumi.set(__self__, "has_search_bar", has_search_bar)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if requests is not None:
@@ -39682,17 +39254,14 @@
     @requests.setter
     def requests(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetQueryTableDefinitionRequestArgs']]]]):
         pulumi.set(self, "requests", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -42029,34 +41598,34 @@
                  autoscale: Optional[pulumi.Input[bool]] = None,
                  custom_links: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetQueryValueDefinitionCustomLinkArgs']]]] = None,
                  custom_unit: Optional[pulumi.Input[str]] = None,
                  live_span: Optional[pulumi.Input[str]] = None,
                  precision: Optional[pulumi.Input[int]] = None,
                  requests: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetQueryValueDefinitionRequestArgs']]]] = None,
                  text_align: Optional[pulumi.Input[str]] = None,
+                 timeseries_background: Optional[pulumi.Input['DashboardWidgetQueryValueDefinitionTimeseriesBackgroundArgs']] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         if autoscale is not None:
             pulumi.set(__self__, "autoscale", autoscale)
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if custom_unit is not None:
             pulumi.set(__self__, "custom_unit", custom_unit)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if precision is not None:
             pulumi.set(__self__, "precision", precision)
         if requests is not None:
             pulumi.set(__self__, "requests", requests)
         if text_align is not None:
             pulumi.set(__self__, "text_align", text_align)
+        if timeseries_background is not None:
+            pulumi.set(__self__, "timeseries_background", timeseries_background)
         if title is not None:
             pulumi.set(__self__, "title", title)
         if title_align is not None:
             pulumi.set(__self__, "title_align", title_align)
         if title_size is not None:
             pulumi.set(__self__, "title_size", title_size)
 
@@ -42120,19 +41689,25 @@
         return pulumi.get(self, "text_align")
 
     @text_align.setter
     def text_align(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "text_align", value)
 
     @property
+    @pulumi.getter(name="timeseriesBackground")
+    def timeseries_background(self) -> Optional[pulumi.Input['DashboardWidgetQueryValueDefinitionTimeseriesBackgroundArgs']]:
+        return pulumi.get(self, "timeseries_background")
+
+    @timeseries_background.setter
+    def timeseries_background(self, value: Optional[pulumi.Input['DashboardWidgetQueryValueDefinitionTimeseriesBackgroundArgs']]):
+        pulumi.set(self, "timeseries_background", value)
+
+    @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -44500,28 +44075,118 @@
 
     @interval.setter
     def interval(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "interval", value)
 
 
 @pulumi.input_type
+class DashboardWidgetQueryValueDefinitionTimeseriesBackgroundArgs:
+    def __init__(__self__, *,
+                 type: pulumi.Input[str],
+                 yaxis: Optional[pulumi.Input['DashboardWidgetQueryValueDefinitionTimeseriesBackgroundYaxisArgs']] = None):
+        pulumi.set(__self__, "type", type)
+        if yaxis is not None:
+            pulumi.set(__self__, "yaxis", yaxis)
+
+    @property
+    @pulumi.getter
+    def type(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "type")
+
+    @type.setter
+    def type(self, value: pulumi.Input[str]):
+        pulumi.set(self, "type", value)
+
+    @property
+    @pulumi.getter
+    def yaxis(self) -> Optional[pulumi.Input['DashboardWidgetQueryValueDefinitionTimeseriesBackgroundYaxisArgs']]:
+        return pulumi.get(self, "yaxis")
+
+    @yaxis.setter
+    def yaxis(self, value: Optional[pulumi.Input['DashboardWidgetQueryValueDefinitionTimeseriesBackgroundYaxisArgs']]):
+        pulumi.set(self, "yaxis", value)
+
+
+@pulumi.input_type
+class DashboardWidgetQueryValueDefinitionTimeseriesBackgroundYaxisArgs:
+    def __init__(__self__, *,
+                 include_zero: Optional[pulumi.Input[bool]] = None,
+                 label: Optional[pulumi.Input[str]] = None,
+                 max: Optional[pulumi.Input[str]] = None,
+                 min: Optional[pulumi.Input[str]] = None,
+                 scale: Optional[pulumi.Input[str]] = None):
+        if include_zero is not None:
+            pulumi.set(__self__, "include_zero", include_zero)
+        if label is not None:
+            pulumi.set(__self__, "label", label)
+        if max is not None:
+            pulumi.set(__self__, "max", max)
+        if min is not None:
+            pulumi.set(__self__, "min", min)
+        if scale is not None:
+            pulumi.set(__self__, "scale", scale)
+
+    @property
+    @pulumi.getter(name="includeZero")
+    def include_zero(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "include_zero")
+
+    @include_zero.setter
+    def include_zero(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "include_zero", value)
+
+    @property
+    @pulumi.getter
+    def label(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "label")
+
+    @label.setter
+    def label(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "label", value)
+
+    @property
+    @pulumi.getter
+    def max(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "max")
+
+    @max.setter
+    def max(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "max", value)
+
+    @property
+    @pulumi.getter
+    def min(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "min")
+
+    @min.setter
+    def min(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "min", value)
+
+    @property
+    @pulumi.getter
+    def scale(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "scale")
+
+    @scale.setter
+    def scale(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "scale", value)
+
+
+@pulumi.input_type
 class DashboardWidgetScatterplotDefinitionArgs:
     def __init__(__self__, *,
                  color_by_groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  custom_links: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetScatterplotDefinitionCustomLinkArgs']]]] = None,
                  live_span: Optional[pulumi.Input[str]] = None,
                  request: Optional[pulumi.Input['DashboardWidgetScatterplotDefinitionRequestArgs']] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None,
                  xaxis: Optional[pulumi.Input['DashboardWidgetScatterplotDefinitionXaxisArgs']] = None,
                  yaxis: Optional[pulumi.Input['DashboardWidgetScatterplotDefinitionYaxisArgs']] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         if color_by_groups is not None:
             pulumi.set(__self__, "color_by_groups", color_by_groups)
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if request is not None:
@@ -44572,17 +44237,14 @@
     @request.setter
     def request(self, value: Optional[pulumi.Input['DashboardWidgetScatterplotDefinitionRequestArgs']]):
         pulumi.set(self, "request", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -47670,17 +47332,14 @@
                  view_mode: pulumi.Input[str],
                  view_type: pulumi.Input[str],
                  global_time_target: Optional[pulumi.Input[str]] = None,
                  show_error_budget: Optional[pulumi.Input[bool]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         pulumi.set(__self__, "slo_id", slo_id)
         pulumi.set(__self__, "time_windows", time_windows)
         pulumi.set(__self__, "view_mode", view_mode)
         pulumi.set(__self__, "view_type", view_type)
         if global_time_target is not None:
             pulumi.set(__self__, "global_time_target", global_time_target)
         if show_error_budget is not None:
@@ -47745,17 +47404,14 @@
     @show_error_budget.setter
     def show_error_budget(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "show_error_budget", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -47782,17 +47438,14 @@
     def __init__(__self__, *,
                  filters: pulumi.Input[Sequence[pulumi.Input[str]]],
                  service: pulumi.Input[str],
                  custom_links: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetServicemapDefinitionCustomLinkArgs']]]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         pulumi.set(__self__, "filters", filters)
         pulumi.set(__self__, "service", service)
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if title is not None:
             pulumi.set(__self__, "title", title)
         if title_align is not None:
@@ -47826,17 +47479,14 @@
     @custom_links.setter
     def custom_links(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetServicemapDefinitionCustomLinkArgs']]]]):
         pulumi.set(self, "custom_links", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -47919,17 +47569,14 @@
                  legend_inline: Optional[pulumi.Input['DashboardWidgetSunburstDefinitionLegendInlineArgs']] = None,
                  legend_table: Optional[pulumi.Input['DashboardWidgetSunburstDefinitionLegendTableArgs']] = None,
                  live_span: Optional[pulumi.Input[str]] = None,
                  requests: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetSunburstDefinitionRequestArgs']]]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if hide_total is not None:
             pulumi.set(__self__, "hide_total", hide_total)
         if legend_inline is not None:
             pulumi.set(__self__, "legend_inline", legend_inline)
         if legend_table is not None:
@@ -47998,17 +47645,14 @@
     @requests.setter
     def requests(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetSunburstDefinitionRequestArgs']]]]):
         pulumi.set(self, "requests", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -50550,17 +50194,14 @@
                  requests: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetTimeseriesDefinitionRequestArgs']]]] = None,
                  right_yaxis: Optional[pulumi.Input['DashboardWidgetTimeseriesDefinitionRightYaxisArgs']] = None,
                  show_legend: Optional[pulumi.Input[bool]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None,
                  yaxis: Optional[pulumi.Input['DashboardWidgetTimeseriesDefinitionYaxisArgs']] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if events is not None:
             pulumi.set(__self__, "events", events)
         if legend_columns is not None:
             pulumi.set(__self__, "legend_columns", legend_columns)
         if legend_layout is not None:
@@ -50675,17 +50316,14 @@
     @show_legend.setter
     def show_legend(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "show_legend", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -53487,17 +53125,14 @@
     def __init__(__self__, *,
                  custom_links: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetToplistDefinitionCustomLinkArgs']]]] = None,
                  live_span: Optional[pulumi.Input[str]] = None,
                  requests: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetToplistDefinitionRequestArgs']]]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if requests is not None:
             pulumi.set(__self__, "requests", requests)
         if title is not None:
@@ -53533,17 +53168,14 @@
     @requests.setter
     def requests(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetToplistDefinitionRequestArgs']]]]):
         pulumi.set(self, "requests", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -55945,17 +55577,14 @@
                  show_hits: Optional[pulumi.Input[bool]] = None,
                  show_latency: Optional[pulumi.Input[bool]] = None,
                  show_resource_list: Optional[pulumi.Input[bool]] = None,
                  size_format: Optional[pulumi.Input[str]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  title_align: Optional[pulumi.Input[str]] = None,
                  title_size: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         pulumi.set(__self__, "env", env)
         pulumi.set(__self__, "service", service)
         pulumi.set(__self__, "span_name", span_name)
         if display_format is not None:
             pulumi.set(__self__, "display_format", display_format)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
@@ -56087,17 +55716,14 @@
     @size_format.setter
     def size_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "size_format", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
@@ -56120,17 +55746,14 @@
 
 
 @pulumi.input_type
 class DashboardWidgetTreemapDefinitionArgs:
     def __init__(__self__, *,
                  requests: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetTreemapDefinitionRequestArgs']]]] = None,
                  title: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] title: The title of the dashboard.
-        """
         if requests is not None:
             pulumi.set(__self__, "requests", requests)
         if title is not None:
             pulumi.set(__self__, "title", title)
 
     @property
     @pulumi.getter
@@ -56140,17 +55763,14 @@
     @requests.setter
     def requests(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetTreemapDefinitionRequestArgs']]]]):
         pulumi.set(self, "requests", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
 
@@ -57126,22 +56746,14 @@
     def __init__(__self__, *,
                  type: pulumi.Input[str],
                  period: Optional[pulumi.Input[int]] = None,
                  rrule: Optional[pulumi.Input[str]] = None,
                  until_date: Optional[pulumi.Input[int]] = None,
                  until_occurrences: Optional[pulumi.Input[int]] = None,
                  week_days: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
-        """
-        :param pulumi.Input[str] type: One of `days`, `weeks`, `months`, or `years`
-        :param pulumi.Input[int] period: How often to repeat as an integer. For example to repeat every 3 days, select a `type` of `days` and a `period` of `3`.
-        :param pulumi.Input[str] rrule: The RRULE standard for defining recurring events. For example, to have a recurring event on the first day of each month, use `FREQ=MONTHLY;INTERVAL=1`. Most common rrule options from the iCalendar Spec are supported. Attributes specifying the duration in RRULE are not supported (for example, `DTSTART`, `DTEND`, `DURATION`).
-        :param pulumi.Input[int] until_date: The date at which the recurrence should end as a POSIX timestamp. `until_occurrences` and `until_date` are mutually exclusive.
-        :param pulumi.Input[int] until_occurrences: How many times the downtime will be rescheduled. `until_occurrences` and `until_date` are mutually exclusive.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] week_days: A list of week days to repeat on. Choose from: `Mon`, `Tue`, `Wed`, `Thu`, `Fri`, `Sat` or `Sun`. Only applicable when `type` is `weeks`. First letter must be capitalized.
-        """
         pulumi.set(__self__, "type", type)
         if period is not None:
             pulumi.set(__self__, "period", period)
         if rrule is not None:
             pulumi.set(__self__, "rrule", rrule)
         if until_date is not None:
             pulumi.set(__self__, "until_date", until_date)
@@ -57149,77 +56761,59 @@
             pulumi.set(__self__, "until_occurrences", until_occurrences)
         if week_days is not None:
             pulumi.set(__self__, "week_days", week_days)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
-        """
-        One of `days`, `weeks`, `months`, or `years`
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def period(self) -> Optional[pulumi.Input[int]]:
-        """
-        How often to repeat as an integer. For example to repeat every 3 days, select a `type` of `days` and a `period` of `3`.
-        """
         return pulumi.get(self, "period")
 
     @period.setter
     def period(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "period", value)
 
     @property
     @pulumi.getter
     def rrule(self) -> Optional[pulumi.Input[str]]:
-        """
-        The RRULE standard for defining recurring events. For example, to have a recurring event on the first day of each month, use `FREQ=MONTHLY;INTERVAL=1`. Most common rrule options from the iCalendar Spec are supported. Attributes specifying the duration in RRULE are not supported (for example, `DTSTART`, `DTEND`, `DURATION`).
-        """
         return pulumi.get(self, "rrule")
 
     @rrule.setter
     def rrule(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "rrule", value)
 
     @property
     @pulumi.getter(name="untilDate")
     def until_date(self) -> Optional[pulumi.Input[int]]:
-        """
-        The date at which the recurrence should end as a POSIX timestamp. `until_occurrences` and `until_date` are mutually exclusive.
-        """
         return pulumi.get(self, "until_date")
 
     @until_date.setter
     def until_date(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "until_date", value)
 
     @property
     @pulumi.getter(name="untilOccurrences")
     def until_occurrences(self) -> Optional[pulumi.Input[int]]:
-        """
-        How many times the downtime will be rescheduled. `until_occurrences` and `until_date` are mutually exclusive.
-        """
         return pulumi.get(self, "until_occurrences")
 
     @until_occurrences.setter
     def until_occurrences(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "until_occurrences", value)
 
     @property
     @pulumi.getter(name="weekDays")
     def week_days(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        A list of week days to repeat on. Choose from: `Mon`, `Tue`, `Wed`, `Thu`, `Fri`, `Sat` or `Sun`. Only applicable when `type` is `weeks`. First letter must be capitalized.
-        """
         return pulumi.get(self, "week_days")
 
     @week_days.setter
     def week_days(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "week_days", value)
 
 
@@ -57227,238 +56821,174 @@
 class LogsArchiveAzureArchiveArgs:
     def __init__(__self__, *,
                  client_id: pulumi.Input[str],
                  container: pulumi.Input[str],
                  storage_account: pulumi.Input[str],
                  tenant_id: pulumi.Input[str],
                  path: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] client_id: Your client id.
-        :param pulumi.Input[str] container: The container where the archive will be stored.
-        :param pulumi.Input[str] storage_account: The associated storage account.
-        :param pulumi.Input[str] tenant_id: Your tenant id.
-        :param pulumi.Input[str] path: The path where the archive will be stored.
-        """
         pulumi.set(__self__, "client_id", client_id)
         pulumi.set(__self__, "container", container)
         pulumi.set(__self__, "storage_account", storage_account)
         pulumi.set(__self__, "tenant_id", tenant_id)
         if path is not None:
             pulumi.set(__self__, "path", path)
 
     @property
     @pulumi.getter(name="clientId")
     def client_id(self) -> pulumi.Input[str]:
-        """
-        Your client id.
-        """
         return pulumi.get(self, "client_id")
 
     @client_id.setter
     def client_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "client_id", value)
 
     @property
     @pulumi.getter
     def container(self) -> pulumi.Input[str]:
-        """
-        The container where the archive will be stored.
-        """
         return pulumi.get(self, "container")
 
     @container.setter
     def container(self, value: pulumi.Input[str]):
         pulumi.set(self, "container", value)
 
     @property
     @pulumi.getter(name="storageAccount")
     def storage_account(self) -> pulumi.Input[str]:
-        """
-        The associated storage account.
-        """
         return pulumi.get(self, "storage_account")
 
     @storage_account.setter
     def storage_account(self, value: pulumi.Input[str]):
         pulumi.set(self, "storage_account", value)
 
     @property
     @pulumi.getter(name="tenantId")
     def tenant_id(self) -> pulumi.Input[str]:
-        """
-        Your tenant id.
-        """
         return pulumi.get(self, "tenant_id")
 
     @tenant_id.setter
     def tenant_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "tenant_id", value)
 
     @property
     @pulumi.getter
     def path(self) -> Optional[pulumi.Input[str]]:
-        """
-        The path where the archive will be stored.
-        """
         return pulumi.get(self, "path")
 
     @path.setter
     def path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "path", value)
 
 
 @pulumi.input_type
 class LogsArchiveGcsArchiveArgs:
     def __init__(__self__, *,
                  bucket: pulumi.Input[str],
                  client_email: pulumi.Input[str],
                  path: pulumi.Input[str],
                  project_id: pulumi.Input[str]):
-        """
-        :param pulumi.Input[str] bucket: Name of your GCS bucket.
-        :param pulumi.Input[str] client_email: Your client email.
-        :param pulumi.Input[str] path: Path where the archive will be stored.
-        :param pulumi.Input[str] project_id: Your project id.
-        """
         pulumi.set(__self__, "bucket", bucket)
         pulumi.set(__self__, "client_email", client_email)
         pulumi.set(__self__, "path", path)
         pulumi.set(__self__, "project_id", project_id)
 
     @property
     @pulumi.getter
     def bucket(self) -> pulumi.Input[str]:
-        """
-        Name of your GCS bucket.
-        """
         return pulumi.get(self, "bucket")
 
     @bucket.setter
     def bucket(self, value: pulumi.Input[str]):
         pulumi.set(self, "bucket", value)
 
     @property
     @pulumi.getter(name="clientEmail")
     def client_email(self) -> pulumi.Input[str]:
-        """
-        Your client email.
-        """
         return pulumi.get(self, "client_email")
 
     @client_email.setter
     def client_email(self, value: pulumi.Input[str]):
         pulumi.set(self, "client_email", value)
 
     @property
     @pulumi.getter
     def path(self) -> pulumi.Input[str]:
-        """
-        Path where the archive will be stored.
-        """
         return pulumi.get(self, "path")
 
     @path.setter
     def path(self, value: pulumi.Input[str]):
         pulumi.set(self, "path", value)
 
     @property
     @pulumi.getter(name="projectId")
     def project_id(self) -> pulumi.Input[str]:
-        """
-        Your project id.
-        """
         return pulumi.get(self, "project_id")
 
     @project_id.setter
     def project_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "project_id", value)
 
 
 @pulumi.input_type
 class LogsArchiveS3ArchiveArgs:
     def __init__(__self__, *,
                  account_id: pulumi.Input[str],
                  bucket: pulumi.Input[str],
                  path: pulumi.Input[str],
                  role_name: pulumi.Input[str]):
-        """
-        :param pulumi.Input[str] account_id: Your AWS account id.
-        :param pulumi.Input[str] bucket: Name of your s3 bucket.
-        :param pulumi.Input[str] path: Path where the archive will be stored.
-        :param pulumi.Input[str] role_name: Your AWS role name
-        """
         pulumi.set(__self__, "account_id", account_id)
         pulumi.set(__self__, "bucket", bucket)
         pulumi.set(__self__, "path", path)
         pulumi.set(__self__, "role_name", role_name)
 
     @property
     @pulumi.getter(name="accountId")
     def account_id(self) -> pulumi.Input[str]:
-        """
-        Your AWS account id.
-        """
         return pulumi.get(self, "account_id")
 
     @account_id.setter
     def account_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "account_id", value)
 
     @property
     @pulumi.getter
     def bucket(self) -> pulumi.Input[str]:
-        """
-        Name of your s3 bucket.
-        """
         return pulumi.get(self, "bucket")
 
     @bucket.setter
     def bucket(self, value: pulumi.Input[str]):
         pulumi.set(self, "bucket", value)
 
     @property
     @pulumi.getter
     def path(self) -> pulumi.Input[str]:
-        """
-        Path where the archive will be stored.
-        """
         return pulumi.get(self, "path")
 
     @path.setter
     def path(self, value: pulumi.Input[str]):
         pulumi.set(self, "path", value)
 
     @property
     @pulumi.getter(name="roleName")
     def role_name(self) -> pulumi.Input[str]:
-        """
-        Your AWS role name
-        """
         return pulumi.get(self, "role_name")
 
     @role_name.setter
     def role_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "role_name", value)
 
 
 @pulumi.input_type
 class LogsCustomPipelineFilterArgs:
     def __init__(__self__, *,
                  query: pulumi.Input[str]):
-        """
-        :param pulumi.Input[str] query: Filter criteria of the category.
-        """
         pulumi.set(__self__, "query", query)
 
     @property
     @pulumi.getter
     def query(self) -> pulumi.Input[str]:
-        """
-        Filter criteria of the category.
-        """
         return pulumi.get(self, "query")
 
     @query.setter
     def query(self, value: pulumi.Input[str]):
         pulumi.set(self, "query", value)
 
 
@@ -57476,30 +57006,14 @@
                  pipeline: Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineArgs']] = None,
                  service_remapper: Optional[pulumi.Input['LogsCustomPipelineProcessorServiceRemapperArgs']] = None,
                  status_remapper: Optional[pulumi.Input['LogsCustomPipelineProcessorStatusRemapperArgs']] = None,
                  string_builder_processor: Optional[pulumi.Input['LogsCustomPipelineProcessorStringBuilderProcessorArgs']] = None,
                  trace_id_remapper: Optional[pulumi.Input['LogsCustomPipelineProcessorTraceIdRemapperArgs']] = None,
                  url_parser: Optional[pulumi.Input['LogsCustomPipelineProcessorUrlParserArgs']] = None,
                  user_agent_parser: Optional[pulumi.Input['LogsCustomPipelineProcessorUserAgentParserArgs']] = None):
-        """
-        :param pulumi.Input['LogsCustomPipelineProcessorArithmeticProcessorArgs'] arithmetic_processor: Arithmetic Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#arithmetic-processor)
-        :param pulumi.Input['LogsCustomPipelineProcessorAttributeRemapperArgs'] attribute_remapper: Attribute Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#remapper)
-        :param pulumi.Input['LogsCustomPipelineProcessorCategoryProcessorArgs'] category_processor: Category Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#category-processor)
-        :param pulumi.Input['LogsCustomPipelineProcessorDateRemapperArgs'] date_remapper: Date Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#log-date-remapper)
-        :param pulumi.Input['LogsCustomPipelineProcessorGeoIpParserArgs'] geo_ip_parser: Date GeoIP Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#geoip-parser)
-        :param pulumi.Input['LogsCustomPipelineProcessorGrokParserArgs'] grok_parser: Grok Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#grok-parser)
-        :param pulumi.Input['LogsCustomPipelineProcessorLookupProcessorArgs'] lookup_processor: Lookup Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#lookup-processor)
-        :param pulumi.Input['LogsCustomPipelineProcessorMessageRemapperArgs'] message_remapper: Message Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#log-message-remapper)
-        :param pulumi.Input['LogsCustomPipelineProcessorServiceRemapperArgs'] service_remapper: Service Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#service-remapper)
-        :param pulumi.Input['LogsCustomPipelineProcessorStatusRemapperArgs'] status_remapper: Status Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#log-status-remapper)
-        :param pulumi.Input['LogsCustomPipelineProcessorStringBuilderProcessorArgs'] string_builder_processor: String Builder Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#string-builder-processor)
-        :param pulumi.Input['LogsCustomPipelineProcessorTraceIdRemapperArgs'] trace_id_remapper: Trace ID Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#trace-remapper)
-        :param pulumi.Input['LogsCustomPipelineProcessorUrlParserArgs'] url_parser: URL Parser Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#url-parser)
-        :param pulumi.Input['LogsCustomPipelineProcessorUserAgentParserArgs'] user_agent_parser: User-Agent Parser Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#user-agent-parser)
-        """
         if arithmetic_processor is not None:
             pulumi.set(__self__, "arithmetic_processor", arithmetic_processor)
         if attribute_remapper is not None:
             pulumi.set(__self__, "attribute_remapper", attribute_remapper)
         if category_processor is not None:
             pulumi.set(__self__, "category_processor", category_processor)
         if date_remapper is not None:
@@ -57526,101 +57040,77 @@
             pulumi.set(__self__, "url_parser", url_parser)
         if user_agent_parser is not None:
             pulumi.set(__self__, "user_agent_parser", user_agent_parser)
 
     @property
     @pulumi.getter(name="arithmeticProcessor")
     def arithmetic_processor(self) -> Optional[pulumi.Input['LogsCustomPipelineProcessorArithmeticProcessorArgs']]:
-        """
-        Arithmetic Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#arithmetic-processor)
-        """
         return pulumi.get(self, "arithmetic_processor")
 
     @arithmetic_processor.setter
     def arithmetic_processor(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorArithmeticProcessorArgs']]):
         pulumi.set(self, "arithmetic_processor", value)
 
     @property
     @pulumi.getter(name="attributeRemapper")
     def attribute_remapper(self) -> Optional[pulumi.Input['LogsCustomPipelineProcessorAttributeRemapperArgs']]:
-        """
-        Attribute Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#remapper)
-        """
         return pulumi.get(self, "attribute_remapper")
 
     @attribute_remapper.setter
     def attribute_remapper(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorAttributeRemapperArgs']]):
         pulumi.set(self, "attribute_remapper", value)
 
     @property
     @pulumi.getter(name="categoryProcessor")
     def category_processor(self) -> Optional[pulumi.Input['LogsCustomPipelineProcessorCategoryProcessorArgs']]:
-        """
-        Category Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#category-processor)
-        """
         return pulumi.get(self, "category_processor")
 
     @category_processor.setter
     def category_processor(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorCategoryProcessorArgs']]):
         pulumi.set(self, "category_processor", value)
 
     @property
     @pulumi.getter(name="dateRemapper")
     def date_remapper(self) -> Optional[pulumi.Input['LogsCustomPipelineProcessorDateRemapperArgs']]:
-        """
-        Date Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#log-date-remapper)
-        """
         return pulumi.get(self, "date_remapper")
 
     @date_remapper.setter
     def date_remapper(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorDateRemapperArgs']]):
         pulumi.set(self, "date_remapper", value)
 
     @property
     @pulumi.getter(name="geoIpParser")
     def geo_ip_parser(self) -> Optional[pulumi.Input['LogsCustomPipelineProcessorGeoIpParserArgs']]:
-        """
-        Date GeoIP Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#geoip-parser)
-        """
         return pulumi.get(self, "geo_ip_parser")
 
     @geo_ip_parser.setter
     def geo_ip_parser(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorGeoIpParserArgs']]):
         pulumi.set(self, "geo_ip_parser", value)
 
     @property
     @pulumi.getter(name="grokParser")
     def grok_parser(self) -> Optional[pulumi.Input['LogsCustomPipelineProcessorGrokParserArgs']]:
-        """
-        Grok Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#grok-parser)
-        """
         return pulumi.get(self, "grok_parser")
 
     @grok_parser.setter
     def grok_parser(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorGrokParserArgs']]):
         pulumi.set(self, "grok_parser", value)
 
     @property
     @pulumi.getter(name="lookupProcessor")
     def lookup_processor(self) -> Optional[pulumi.Input['LogsCustomPipelineProcessorLookupProcessorArgs']]:
-        """
-        Lookup Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#lookup-processor)
-        """
         return pulumi.get(self, "lookup_processor")
 
     @lookup_processor.setter
     def lookup_processor(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorLookupProcessorArgs']]):
         pulumi.set(self, "lookup_processor", value)
 
     @property
     @pulumi.getter(name="messageRemapper")
     def message_remapper(self) -> Optional[pulumi.Input['LogsCustomPipelineProcessorMessageRemapperArgs']]:
-        """
-        Message Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#log-message-remapper)
-        """
         return pulumi.get(self, "message_remapper")
 
     @message_remapper.setter
     def message_remapper(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorMessageRemapperArgs']]):
         pulumi.set(self, "message_remapper", value)
 
     @property
@@ -57631,77 +57121,59 @@
     @pipeline.setter
     def pipeline(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineArgs']]):
         pulumi.set(self, "pipeline", value)
 
     @property
     @pulumi.getter(name="serviceRemapper")
     def service_remapper(self) -> Optional[pulumi.Input['LogsCustomPipelineProcessorServiceRemapperArgs']]:
-        """
-        Service Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#service-remapper)
-        """
         return pulumi.get(self, "service_remapper")
 
     @service_remapper.setter
     def service_remapper(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorServiceRemapperArgs']]):
         pulumi.set(self, "service_remapper", value)
 
     @property
     @pulumi.getter(name="statusRemapper")
     def status_remapper(self) -> Optional[pulumi.Input['LogsCustomPipelineProcessorStatusRemapperArgs']]:
-        """
-        Status Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#log-status-remapper)
-        """
         return pulumi.get(self, "status_remapper")
 
     @status_remapper.setter
     def status_remapper(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorStatusRemapperArgs']]):
         pulumi.set(self, "status_remapper", value)
 
     @property
     @pulumi.getter(name="stringBuilderProcessor")
     def string_builder_processor(self) -> Optional[pulumi.Input['LogsCustomPipelineProcessorStringBuilderProcessorArgs']]:
-        """
-        String Builder Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#string-builder-processor)
-        """
         return pulumi.get(self, "string_builder_processor")
 
     @string_builder_processor.setter
     def string_builder_processor(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorStringBuilderProcessorArgs']]):
         pulumi.set(self, "string_builder_processor", value)
 
     @property
     @pulumi.getter(name="traceIdRemapper")
     def trace_id_remapper(self) -> Optional[pulumi.Input['LogsCustomPipelineProcessorTraceIdRemapperArgs']]:
-        """
-        Trace ID Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#trace-remapper)
-        """
         return pulumi.get(self, "trace_id_remapper")
 
     @trace_id_remapper.setter
     def trace_id_remapper(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorTraceIdRemapperArgs']]):
         pulumi.set(self, "trace_id_remapper", value)
 
     @property
     @pulumi.getter(name="urlParser")
     def url_parser(self) -> Optional[pulumi.Input['LogsCustomPipelineProcessorUrlParserArgs']]:
-        """
-        URL Parser Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#url-parser)
-        """
         return pulumi.get(self, "url_parser")
 
     @url_parser.setter
     def url_parser(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorUrlParserArgs']]):
         pulumi.set(self, "url_parser", value)
 
     @property
     @pulumi.getter(name="userAgentParser")
     def user_agent_parser(self) -> Optional[pulumi.Input['LogsCustomPipelineProcessorUserAgentParserArgs']]:
-        """
-        User-Agent Parser Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#user-agent-parser)
-        """
         return pulumi.get(self, "user_agent_parser")
 
     @user_agent_parser.setter
     def user_agent_parser(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorUserAgentParserArgs']]):
         pulumi.set(self, "user_agent_parser", value)
 
 
@@ -57955,25 +57427,19 @@
         pulumi.set(self, "name", value)
 
 
 @pulumi.input_type
 class LogsCustomPipelineProcessorCategoryProcessorCategoryFilterArgs:
     def __init__(__self__, *,
                  query: pulumi.Input[str]):
-        """
-        :param pulumi.Input[str] query: Filter criteria of the category.
-        """
         pulumi.set(__self__, "query", query)
 
     @property
     @pulumi.getter
     def query(self) -> pulumi.Input[str]:
-        """
-        Filter criteria of the category.
-        """
         return pulumi.get(self, "query")
 
     @query.setter
     def query(self, value: pulumi.Input[str]):
         pulumi.set(self, "query", value)
 
 
@@ -58323,25 +57789,19 @@
         pulumi.set(self, "processors", value)
 
 
 @pulumi.input_type
 class LogsCustomPipelineProcessorPipelineFilterArgs:
     def __init__(__self__, *,
                  query: pulumi.Input[str]):
-        """
-        :param pulumi.Input[str] query: Filter criteria of the category.
-        """
         pulumi.set(__self__, "query", query)
 
     @property
     @pulumi.getter
     def query(self) -> pulumi.Input[str]:
-        """
-        Filter criteria of the category.
-        """
         return pulumi.get(self, "query")
 
     @query.setter
     def query(self, value: pulumi.Input[str]):
         pulumi.set(self, "query", value)
 
 
@@ -58358,30 +57818,14 @@
                  message_remapper: Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorMessageRemapperArgs']] = None,
                  service_remapper: Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorServiceRemapperArgs']] = None,
                  status_remapper: Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorStatusRemapperArgs']] = None,
                  string_builder_processor: Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorStringBuilderProcessorArgs']] = None,
                  trace_id_remapper: Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorTraceIdRemapperArgs']] = None,
                  url_parser: Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorUrlParserArgs']] = None,
                  user_agent_parser: Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorUserAgentParserArgs']] = None):
-        """
-        :param pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorArithmeticProcessorArgs'] arithmetic_processor: Arithmetic Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#arithmetic-processor)
-        :param pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorAttributeRemapperArgs'] attribute_remapper: Attribute Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#remapper)
-        :param pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorCategoryProcessorArgs'] category_processor: Category Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#category-processor)
-        :param pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorDateRemapperArgs'] date_remapper: Date Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#log-date-remapper)
-        :param pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorGeoIpParserArgs'] geo_ip_parser: Date GeoIP Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#geoip-parser)
-        :param pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorGrokParserArgs'] grok_parser: Grok Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#grok-parser)
-        :param pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorLookupProcessorArgs'] lookup_processor: Lookup Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#lookup-processor)
-        :param pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorMessageRemapperArgs'] message_remapper: Message Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#log-message-remapper)
-        :param pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorServiceRemapperArgs'] service_remapper: Service Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#service-remapper)
-        :param pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorStatusRemapperArgs'] status_remapper: Status Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#log-status-remapper)
-        :param pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorStringBuilderProcessorArgs'] string_builder_processor: String Builder Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#string-builder-processor)
-        :param pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorTraceIdRemapperArgs'] trace_id_remapper: Trace ID Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#trace-remapper)
-        :param pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorUrlParserArgs'] url_parser: URL Parser Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#url-parser)
-        :param pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorUserAgentParserArgs'] user_agent_parser: User-Agent Parser Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#user-agent-parser)
-        """
         if arithmetic_processor is not None:
             pulumi.set(__self__, "arithmetic_processor", arithmetic_processor)
         if attribute_remapper is not None:
             pulumi.set(__self__, "attribute_remapper", attribute_remapper)
         if category_processor is not None:
             pulumi.set(__self__, "category_processor", category_processor)
         if date_remapper is not None:
@@ -58406,173 +57850,131 @@
             pulumi.set(__self__, "url_parser", url_parser)
         if user_agent_parser is not None:
             pulumi.set(__self__, "user_agent_parser", user_agent_parser)
 
     @property
     @pulumi.getter(name="arithmeticProcessor")
     def arithmetic_processor(self) -> Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorArithmeticProcessorArgs']]:
-        """
-        Arithmetic Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#arithmetic-processor)
-        """
         return pulumi.get(self, "arithmetic_processor")
 
     @arithmetic_processor.setter
     def arithmetic_processor(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorArithmeticProcessorArgs']]):
         pulumi.set(self, "arithmetic_processor", value)
 
     @property
     @pulumi.getter(name="attributeRemapper")
     def attribute_remapper(self) -> Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorAttributeRemapperArgs']]:
-        """
-        Attribute Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#remapper)
-        """
         return pulumi.get(self, "attribute_remapper")
 
     @attribute_remapper.setter
     def attribute_remapper(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorAttributeRemapperArgs']]):
         pulumi.set(self, "attribute_remapper", value)
 
     @property
     @pulumi.getter(name="categoryProcessor")
     def category_processor(self) -> Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorCategoryProcessorArgs']]:
-        """
-        Category Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#category-processor)
-        """
         return pulumi.get(self, "category_processor")
 
     @category_processor.setter
     def category_processor(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorCategoryProcessorArgs']]):
         pulumi.set(self, "category_processor", value)
 
     @property
     @pulumi.getter(name="dateRemapper")
     def date_remapper(self) -> Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorDateRemapperArgs']]:
-        """
-        Date Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#log-date-remapper)
-        """
         return pulumi.get(self, "date_remapper")
 
     @date_remapper.setter
     def date_remapper(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorDateRemapperArgs']]):
         pulumi.set(self, "date_remapper", value)
 
     @property
     @pulumi.getter(name="geoIpParser")
     def geo_ip_parser(self) -> Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorGeoIpParserArgs']]:
-        """
-        Date GeoIP Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#geoip-parser)
-        """
         return pulumi.get(self, "geo_ip_parser")
 
     @geo_ip_parser.setter
     def geo_ip_parser(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorGeoIpParserArgs']]):
         pulumi.set(self, "geo_ip_parser", value)
 
     @property
     @pulumi.getter(name="grokParser")
     def grok_parser(self) -> Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorGrokParserArgs']]:
-        """
-        Grok Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#grok-parser)
-        """
         return pulumi.get(self, "grok_parser")
 
     @grok_parser.setter
     def grok_parser(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorGrokParserArgs']]):
         pulumi.set(self, "grok_parser", value)
 
     @property
     @pulumi.getter(name="lookupProcessor")
     def lookup_processor(self) -> Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorLookupProcessorArgs']]:
-        """
-        Lookup Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#lookup-processor)
-        """
         return pulumi.get(self, "lookup_processor")
 
     @lookup_processor.setter
     def lookup_processor(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorLookupProcessorArgs']]):
         pulumi.set(self, "lookup_processor", value)
 
     @property
     @pulumi.getter(name="messageRemapper")
     def message_remapper(self) -> Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorMessageRemapperArgs']]:
-        """
-        Message Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#log-message-remapper)
-        """
         return pulumi.get(self, "message_remapper")
 
     @message_remapper.setter
     def message_remapper(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorMessageRemapperArgs']]):
         pulumi.set(self, "message_remapper", value)
 
     @property
     @pulumi.getter(name="serviceRemapper")
     def service_remapper(self) -> Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorServiceRemapperArgs']]:
-        """
-        Service Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#service-remapper)
-        """
         return pulumi.get(self, "service_remapper")
 
     @service_remapper.setter
     def service_remapper(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorServiceRemapperArgs']]):
         pulumi.set(self, "service_remapper", value)
 
     @property
     @pulumi.getter(name="statusRemapper")
     def status_remapper(self) -> Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorStatusRemapperArgs']]:
-        """
-        Status Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#log-status-remapper)
-        """
         return pulumi.get(self, "status_remapper")
 
     @status_remapper.setter
     def status_remapper(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorStatusRemapperArgs']]):
         pulumi.set(self, "status_remapper", value)
 
     @property
     @pulumi.getter(name="stringBuilderProcessor")
     def string_builder_processor(self) -> Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorStringBuilderProcessorArgs']]:
-        """
-        String Builder Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#string-builder-processor)
-        """
         return pulumi.get(self, "string_builder_processor")
 
     @string_builder_processor.setter
     def string_builder_processor(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorStringBuilderProcessorArgs']]):
         pulumi.set(self, "string_builder_processor", value)
 
     @property
     @pulumi.getter(name="traceIdRemapper")
     def trace_id_remapper(self) -> Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorTraceIdRemapperArgs']]:
-        """
-        Trace ID Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#trace-remapper)
-        """
         return pulumi.get(self, "trace_id_remapper")
 
     @trace_id_remapper.setter
     def trace_id_remapper(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorTraceIdRemapperArgs']]):
         pulumi.set(self, "trace_id_remapper", value)
 
     @property
     @pulumi.getter(name="urlParser")
     def url_parser(self) -> Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorUrlParserArgs']]:
-        """
-        URL Parser Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#url-parser)
-        """
         return pulumi.get(self, "url_parser")
 
     @url_parser.setter
     def url_parser(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorUrlParserArgs']]):
         pulumi.set(self, "url_parser", value)
 
     @property
     @pulumi.getter(name="userAgentParser")
     def user_agent_parser(self) -> Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorUserAgentParserArgs']]:
-        """
-        User-Agent Parser Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#user-agent-parser)
-        """
         return pulumi.get(self, "user_agent_parser")
 
     @user_agent_parser.setter
     def user_agent_parser(self, value: Optional[pulumi.Input['LogsCustomPipelineProcessorPipelineProcessorUserAgentParserArgs']]):
         pulumi.set(self, "user_agent_parser", value)
 
 
@@ -58826,25 +58228,19 @@
         pulumi.set(self, "name", value)
 
 
 @pulumi.input_type
 class LogsCustomPipelineProcessorPipelineProcessorCategoryProcessorCategoryFilterArgs:
     def __init__(__self__, *,
                  query: pulumi.Input[str]):
-        """
-        :param pulumi.Input[str] query: Filter criteria of the category.
-        """
         pulumi.set(__self__, "query", query)
 
     @property
     @pulumi.getter
     def query(self) -> pulumi.Input[str]:
-        """
-        Filter criteria of the category.
-        """
         return pulumi.get(self, "query")
 
     @query.setter
     def query(self, value: pulumi.Input[str]):
         pulumi.set(self, "query", value)
 
 
@@ -59763,82 +59159,62 @@
 
 @pulumi.input_type
 class LogsIndexExclusionFilterArgs:
     def __init__(__self__, *,
                  filters: Optional[pulumi.Input[Sequence[pulumi.Input['LogsIndexExclusionFilterFilterArgs']]]] = None,
                  is_enabled: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[Sequence[pulumi.Input['LogsIndexExclusionFilterFilterArgs']]] filters: Logs filter
-        :param pulumi.Input[bool] is_enabled: A boolean stating if the exclusion is active or not.
-        :param pulumi.Input[str] name: The name of the exclusion filter.
-        """
         if filters is not None:
             pulumi.set(__self__, "filters", filters)
         if is_enabled is not None:
             pulumi.set(__self__, "is_enabled", is_enabled)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def filters(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['LogsIndexExclusionFilterFilterArgs']]]]:
-        """
-        Logs filter
-        """
         return pulumi.get(self, "filters")
 
     @filters.setter
     def filters(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['LogsIndexExclusionFilterFilterArgs']]]]):
         pulumi.set(self, "filters", value)
 
     @property
     @pulumi.getter(name="isEnabled")
     def is_enabled(self) -> Optional[pulumi.Input[bool]]:
-        """
-        A boolean stating if the exclusion is active or not.
-        """
         return pulumi.get(self, "is_enabled")
 
     @is_enabled.setter
     def is_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "is_enabled", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
-        """
-        The name of the exclusion filter.
-        """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
 
 @pulumi.input_type
 class LogsIndexExclusionFilterFilterArgs:
     def __init__(__self__, *,
                  query: Optional[pulumi.Input[str]] = None,
                  sample_rate: Optional[pulumi.Input[float]] = None):
-        """
-        :param pulumi.Input[str] query: Logs filter criteria. Only logs matching this filter criteria are considered for this index.
-        """
         if query is not None:
             pulumi.set(__self__, "query", query)
         if sample_rate is not None:
             pulumi.set(__self__, "sample_rate", sample_rate)
 
     @property
     @pulumi.getter
     def query(self) -> Optional[pulumi.Input[str]]:
-        """
-        Logs filter criteria. Only logs matching this filter criteria are considered for this index.
-        """
         return pulumi.get(self, "query")
 
     @query.setter
     def query(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "query", value)
 
     @property
@@ -59851,198 +59227,146 @@
         pulumi.set(self, "sample_rate", value)
 
 
 @pulumi.input_type
 class LogsIndexFilterArgs:
     def __init__(__self__, *,
                  query: pulumi.Input[str]):
-        """
-        :param pulumi.Input[str] query: Logs filter criteria. Only logs matching this filter criteria are considered for this index.
-        """
         pulumi.set(__self__, "query", query)
 
     @property
     @pulumi.getter
     def query(self) -> pulumi.Input[str]:
-        """
-        Logs filter criteria. Only logs matching this filter criteria are considered for this index.
-        """
         return pulumi.get(self, "query")
 
     @query.setter
     def query(self, value: pulumi.Input[str]):
         pulumi.set(self, "query", value)
 
 
 @pulumi.input_type
 class LogsMetricComputeArgs:
     def __init__(__self__, *,
                  aggregation_type: pulumi.Input[str],
                  path: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] aggregation_type: The type of aggregation to use. This field can't be updated after creation. Valid values are `count`, `distribution`.
-        :param pulumi.Input[str] path: The path to the value the log-based metric will aggregate on (only used if the aggregation type is a "distribution"). This field can't be updated after creation.
-        """
         pulumi.set(__self__, "aggregation_type", aggregation_type)
         if path is not None:
             pulumi.set(__self__, "path", path)
 
     @property
     @pulumi.getter(name="aggregationType")
     def aggregation_type(self) -> pulumi.Input[str]:
-        """
-        The type of aggregation to use. This field can't be updated after creation. Valid values are `count`, `distribution`.
-        """
         return pulumi.get(self, "aggregation_type")
 
     @aggregation_type.setter
     def aggregation_type(self, value: pulumi.Input[str]):
         pulumi.set(self, "aggregation_type", value)
 
     @property
     @pulumi.getter
     def path(self) -> Optional[pulumi.Input[str]]:
-        """
-        The path to the value the log-based metric will aggregate on (only used if the aggregation type is a "distribution"). This field can't be updated after creation.
-        """
         return pulumi.get(self, "path")
 
     @path.setter
     def path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "path", value)
 
 
 @pulumi.input_type
 class LogsMetricFilterArgs:
     def __init__(__self__, *,
                  query: pulumi.Input[str]):
-        """
-        :param pulumi.Input[str] query: The search query - following the log search syntax.
-        """
         pulumi.set(__self__, "query", query)
 
     @property
     @pulumi.getter
     def query(self) -> pulumi.Input[str]:
-        """
-        The search query - following the log search syntax.
-        """
         return pulumi.get(self, "query")
 
     @query.setter
     def query(self, value: pulumi.Input[str]):
         pulumi.set(self, "query", value)
 
 
 @pulumi.input_type
 class LogsMetricGroupByArgs:
     def __init__(__self__, *,
                  path: pulumi.Input[str],
                  tag_name: pulumi.Input[str]):
-        """
-        :param pulumi.Input[str] path: The path to the value the log-based metric will be aggregated over.
-        :param pulumi.Input[str] tag_name: Name of the tag that gets created.
-        """
         pulumi.set(__self__, "path", path)
         pulumi.set(__self__, "tag_name", tag_name)
 
     @property
     @pulumi.getter
     def path(self) -> pulumi.Input[str]:
-        """
-        The path to the value the log-based metric will be aggregated over.
-        """
         return pulumi.get(self, "path")
 
     @path.setter
     def path(self, value: pulumi.Input[str]):
         pulumi.set(self, "path", value)
 
     @property
     @pulumi.getter(name="tagName")
     def tag_name(self) -> pulumi.Input[str]:
-        """
-        Name of the tag that gets created.
-        """
         return pulumi.get(self, "tag_name")
 
     @tag_name.setter
     def tag_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "tag_name", value)
 
 
 @pulumi.input_type
 class MetricTagConfigurationAggregationArgs:
     def __init__(__self__, *,
                  space: pulumi.Input[str],
                  time: pulumi.Input[str]):
-        """
-        :param pulumi.Input[str] space: A space aggregation for use in query. Valid values are `avg`, `max`, `min`, `sum`.
-        :param pulumi.Input[str] time: A time aggregation for use in query. Valid values are `avg`, `count`, `max`, `min`, `sum`.
-        """
         pulumi.set(__self__, "space", space)
         pulumi.set(__self__, "time", time)
 
     @property
     @pulumi.getter
     def space(self) -> pulumi.Input[str]:
-        """
-        A space aggregation for use in query. Valid values are `avg`, `max`, `min`, `sum`.
-        """
         return pulumi.get(self, "space")
 
     @space.setter
     def space(self, value: pulumi.Input[str]):
         pulumi.set(self, "space", value)
 
     @property
     @pulumi.getter
     def time(self) -> pulumi.Input[str]:
-        """
-        A time aggregation for use in query. Valid values are `avg`, `count`, `max`, `min`, `sum`.
-        """
         return pulumi.get(self, "time")
 
     @time.setter
     def time(self, value: pulumi.Input[str]):
         pulumi.set(self, "time", value)
 
 
 @pulumi.input_type
 class MonitorMonitorThresholdWindowsArgs:
     def __init__(__self__, *,
                  recovery_window: Optional[pulumi.Input[str]] = None,
                  trigger_window: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] recovery_window: Describes how long an anomalous metric must be normal before the alert recovers.
-        :param pulumi.Input[str] trigger_window: Describes how long a metric must be anomalous before an alert triggers.
-        """
         if recovery_window is not None:
             pulumi.set(__self__, "recovery_window", recovery_window)
         if trigger_window is not None:
             pulumi.set(__self__, "trigger_window", trigger_window)
 
     @property
     @pulumi.getter(name="recoveryWindow")
     def recovery_window(self) -> Optional[pulumi.Input[str]]:
-        """
-        Describes how long an anomalous metric must be normal before the alert recovers.
-        """
         return pulumi.get(self, "recovery_window")
 
     @recovery_window.setter
     def recovery_window(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "recovery_window", value)
 
     @property
     @pulumi.getter(name="triggerWindow")
     def trigger_window(self) -> Optional[pulumi.Input[str]]:
-        """
-        Describes how long a metric must be anomalous before an alert triggers.
-        """
         return pulumi.get(self, "trigger_window")
 
     @trigger_window.setter
     def trigger_window(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "trigger_window", value)
 
 
@@ -60051,22 +59375,14 @@
     def __init__(__self__, *,
                  critical: Optional[pulumi.Input[str]] = None,
                  critical_recovery: Optional[pulumi.Input[str]] = None,
                  ok: Optional[pulumi.Input[str]] = None,
                  unknown: Optional[pulumi.Input[str]] = None,
                  warning: Optional[pulumi.Input[str]] = None,
                  warning_recovery: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] critical: The monitor `CRITICAL` threshold. Must be a number.
-        :param pulumi.Input[str] critical_recovery: The monitor `CRITICAL` recovery threshold. Must be a number.
-        :param pulumi.Input[str] ok: The monitor `OK` threshold. Must be a number.
-        :param pulumi.Input[str] unknown: The monitor `UNKNOWN` threshold. Must be a number.
-        :param pulumi.Input[str] warning: The monitor `WARNING` threshold. Must be a number.
-        :param pulumi.Input[str] warning_recovery: The monitor `WARNING` recovery threshold. Must be a number.
-        """
         if critical is not None:
             pulumi.set(__self__, "critical", critical)
         if critical_recovery is not None:
             pulumi.set(__self__, "critical_recovery", critical_recovery)
         if ok is not None:
             pulumi.set(__self__, "ok", ok)
         if unknown is not None:
@@ -60075,77 +59391,59 @@
             pulumi.set(__self__, "warning", warning)
         if warning_recovery is not None:
             pulumi.set(__self__, "warning_recovery", warning_recovery)
 
     @property
     @pulumi.getter
     def critical(self) -> Optional[pulumi.Input[str]]:
-        """
-        The monitor `CRITICAL` threshold. Must be a number.
-        """
         return pulumi.get(self, "critical")
 
     @critical.setter
     def critical(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "critical", value)
 
     @property
     @pulumi.getter(name="criticalRecovery")
     def critical_recovery(self) -> Optional[pulumi.Input[str]]:
-        """
-        The monitor `CRITICAL` recovery threshold. Must be a number.
-        """
         return pulumi.get(self, "critical_recovery")
 
     @critical_recovery.setter
     def critical_recovery(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "critical_recovery", value)
 
     @property
     @pulumi.getter
     def ok(self) -> Optional[pulumi.Input[str]]:
-        """
-        The monitor `OK` threshold. Must be a number.
-        """
         return pulumi.get(self, "ok")
 
     @ok.setter
     def ok(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ok", value)
 
     @property
     @pulumi.getter
     def unknown(self) -> Optional[pulumi.Input[str]]:
-        """
-        The monitor `UNKNOWN` threshold. Must be a number.
-        """
         return pulumi.get(self, "unknown")
 
     @unknown.setter
     def unknown(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "unknown", value)
 
     @property
     @pulumi.getter
     def warning(self) -> Optional[pulumi.Input[str]]:
-        """
-        The monitor `WARNING` threshold. Must be a number.
-        """
         return pulumi.get(self, "warning")
 
     @warning.setter
     def warning(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "warning", value)
 
     @property
     @pulumi.getter(name="warningRecovery")
     def warning_recovery(self) -> Optional[pulumi.Input[str]]:
-        """
-        The monitor `WARNING` recovery threshold. Must be a number.
-        """
         return pulumi.get(self, "warning_recovery")
 
     @warning_recovery.setter
     def warning_recovery(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "warning_recovery", value)
 
 
@@ -60158,26 +59456,14 @@
                  saml_strict_mode: pulumi.Input['OrganizationSettingsSettingsSamlStrictModeArgs'],
                  private_widget_share: Optional[pulumi.Input[bool]] = None,
                  saml_autocreate_access_role: Optional[pulumi.Input[str]] = None,
                  saml_can_be_enabled: Optional[pulumi.Input[bool]] = None,
                  saml_idp_endpoint: Optional[pulumi.Input[str]] = None,
                  saml_idp_metadata_uploaded: Optional[pulumi.Input[bool]] = None,
                  saml_login_url: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input['OrganizationSettingsSettingsSamlArgs'] saml: SAML properties
-        :param pulumi.Input['OrganizationSettingsSettingsSamlAutocreateUsersDomainsArgs'] saml_autocreate_users_domains: List of domains where the SAML automated user creation is enabled.
-        :param pulumi.Input['OrganizationSettingsSettingsSamlIdpInitiatedLoginArgs'] saml_idp_initiated_login: Whether or not a SAML identity provider metadata file was provided to the Datadog organization.
-        :param pulumi.Input['OrganizationSettingsSettingsSamlStrictModeArgs'] saml_strict_mode: Whether or not the SAML strict mode is enabled. If true, all users must log in with SAML.
-        :param pulumi.Input[bool] private_widget_share: Whether or not the organization users can share widgets outside of Datadog.
-        :param pulumi.Input[str] saml_autocreate_access_role: The access role of the user. Options are `st` (standard user), `adm` (admin user), or `ro` (read-only user). Allowed enum values: `st`, `adm` , `ro`, `ERROR`
-        :param pulumi.Input[bool] saml_can_be_enabled: Whether or not SAML can be enabled for this organization.
-        :param pulumi.Input[str] saml_idp_endpoint: Identity provider endpoint for SAML authentication.
-        :param pulumi.Input[bool] saml_idp_metadata_uploaded: Whether or not a SAML identity provider metadata file was provided to the Datadog organization.
-        :param pulumi.Input[str] saml_login_url: URL for SAML logging.
-        """
         pulumi.set(__self__, "saml", saml)
         pulumi.set(__self__, "saml_autocreate_users_domains", saml_autocreate_users_domains)
         pulumi.set(__self__, "saml_idp_initiated_login", saml_idp_initiated_login)
         pulumi.set(__self__, "saml_strict_mode", saml_strict_mode)
         if private_widget_share is not None:
             pulumi.set(__self__, "private_widget_share", private_widget_share)
         if saml_autocreate_access_role is not None:
@@ -60190,125 +59476,95 @@
             pulumi.set(__self__, "saml_idp_metadata_uploaded", saml_idp_metadata_uploaded)
         if saml_login_url is not None:
             pulumi.set(__self__, "saml_login_url", saml_login_url)
 
     @property
     @pulumi.getter
     def saml(self) -> pulumi.Input['OrganizationSettingsSettingsSamlArgs']:
-        """
-        SAML properties
-        """
         return pulumi.get(self, "saml")
 
     @saml.setter
     def saml(self, value: pulumi.Input['OrganizationSettingsSettingsSamlArgs']):
         pulumi.set(self, "saml", value)
 
     @property
     @pulumi.getter(name="samlAutocreateUsersDomains")
     def saml_autocreate_users_domains(self) -> pulumi.Input['OrganizationSettingsSettingsSamlAutocreateUsersDomainsArgs']:
-        """
-        List of domains where the SAML automated user creation is enabled.
-        """
         return pulumi.get(self, "saml_autocreate_users_domains")
 
     @saml_autocreate_users_domains.setter
     def saml_autocreate_users_domains(self, value: pulumi.Input['OrganizationSettingsSettingsSamlAutocreateUsersDomainsArgs']):
         pulumi.set(self, "saml_autocreate_users_domains", value)
 
     @property
     @pulumi.getter(name="samlIdpInitiatedLogin")
     def saml_idp_initiated_login(self) -> pulumi.Input['OrganizationSettingsSettingsSamlIdpInitiatedLoginArgs']:
-        """
-        Whether or not a SAML identity provider metadata file was provided to the Datadog organization.
-        """
         return pulumi.get(self, "saml_idp_initiated_login")
 
     @saml_idp_initiated_login.setter
     def saml_idp_initiated_login(self, value: pulumi.Input['OrganizationSettingsSettingsSamlIdpInitiatedLoginArgs']):
         pulumi.set(self, "saml_idp_initiated_login", value)
 
     @property
     @pulumi.getter(name="samlStrictMode")
     def saml_strict_mode(self) -> pulumi.Input['OrganizationSettingsSettingsSamlStrictModeArgs']:
-        """
-        Whether or not the SAML strict mode is enabled. If true, all users must log in with SAML.
-        """
         return pulumi.get(self, "saml_strict_mode")
 
     @saml_strict_mode.setter
     def saml_strict_mode(self, value: pulumi.Input['OrganizationSettingsSettingsSamlStrictModeArgs']):
         pulumi.set(self, "saml_strict_mode", value)
 
     @property
     @pulumi.getter(name="privateWidgetShare")
     def private_widget_share(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Whether or not the organization users can share widgets outside of Datadog.
-        """
         return pulumi.get(self, "private_widget_share")
 
     @private_widget_share.setter
     def private_widget_share(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "private_widget_share", value)
 
     @property
     @pulumi.getter(name="samlAutocreateAccessRole")
     def saml_autocreate_access_role(self) -> Optional[pulumi.Input[str]]:
-        """
-        The access role of the user. Options are `st` (standard user), `adm` (admin user), or `ro` (read-only user). Allowed enum values: `st`, `adm` , `ro`, `ERROR`
-        """
         return pulumi.get(self, "saml_autocreate_access_role")
 
     @saml_autocreate_access_role.setter
     def saml_autocreate_access_role(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "saml_autocreate_access_role", value)
 
     @property
     @pulumi.getter(name="samlCanBeEnabled")
     def saml_can_be_enabled(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Whether or not SAML can be enabled for this organization.
-        """
         return pulumi.get(self, "saml_can_be_enabled")
 
     @saml_can_be_enabled.setter
     def saml_can_be_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "saml_can_be_enabled", value)
 
     @property
     @pulumi.getter(name="samlIdpEndpoint")
     def saml_idp_endpoint(self) -> Optional[pulumi.Input[str]]:
-        """
-        Identity provider endpoint for SAML authentication.
-        """
         return pulumi.get(self, "saml_idp_endpoint")
 
     @saml_idp_endpoint.setter
     def saml_idp_endpoint(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "saml_idp_endpoint", value)
 
     @property
     @pulumi.getter(name="samlIdpMetadataUploaded")
     def saml_idp_metadata_uploaded(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Whether or not a SAML identity provider metadata file was provided to the Datadog organization.
-        """
         return pulumi.get(self, "saml_idp_metadata_uploaded")
 
     @saml_idp_metadata_uploaded.setter
     def saml_idp_metadata_uploaded(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "saml_idp_metadata_uploaded", value)
 
     @property
     @pulumi.getter(name="samlLoginUrl")
     def saml_login_url(self) -> Optional[pulumi.Input[str]]:
-        """
-        URL for SAML logging.
-        """
         return pulumi.get(self, "saml_login_url")
 
     @saml_login_url.setter
     def saml_login_url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "saml_login_url", value)
 
 
@@ -60393,40 +59649,30 @@
 
 
 @pulumi.input_type
 class RolePermissionArgs:
     def __init__(__self__, *,
                  id: pulumi.Input[str],
                  name: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] id: ID of the permission to assign.
-        :param pulumi.Input[str] name: Name of the permission.
-        """
         pulumi.set(__self__, "id", id)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def id(self) -> pulumi.Input[str]:
-        """
-        ID of the permission to assign.
-        """
         return pulumi.get(self, "id")
 
     @id.setter
     def id(self, value: pulumi.Input[str]):
         pulumi.set(self, "id", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
-        """
-        Name of the permission.
-        """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
 
@@ -60485,39 +59731,29 @@
 
 
 @pulumi.input_type
 class SecurityMonitoringFilterExclusionFilterArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  query: pulumi.Input[str]):
-        """
-        :param pulumi.Input[str] name: Exclusion filter name.
-        :param pulumi.Input[str] query: Exclusion filter query. Logs that match this query are excluded from the security filter.
-        """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "query", query)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
-        """
-        Exclusion filter name.
-        """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def query(self) -> pulumi.Input[str]:
-        """
-        Exclusion filter query. Logs that match this query are excluded from the security filter.
-        """
         return pulumi.get(self, "query")
 
     @query.setter
     def query(self, value: pulumi.Input[str]):
         pulumi.set(self, "query", value)
 
 
@@ -60615,21 +59851,24 @@
 @pulumi.input_type
 class SecurityMonitoringRuleOptionsArgs:
     def __init__(__self__, *,
                  keep_alive: pulumi.Input[int],
                  max_signal_duration: pulumi.Input[int],
                  detection_method: Optional[pulumi.Input[str]] = None,
                  evaluation_window: Optional[pulumi.Input[int]] = None,
+                 impossible_travel_options: Optional[pulumi.Input['SecurityMonitoringRuleOptionsImpossibleTravelOptionsArgs']] = None,
                  new_value_options: Optional[pulumi.Input['SecurityMonitoringRuleOptionsNewValueOptionsArgs']] = None):
         pulumi.set(__self__, "keep_alive", keep_alive)
         pulumi.set(__self__, "max_signal_duration", max_signal_duration)
         if detection_method is not None:
             pulumi.set(__self__, "detection_method", detection_method)
         if evaluation_window is not None:
             pulumi.set(__self__, "evaluation_window", evaluation_window)
+        if impossible_travel_options is not None:
+            pulumi.set(__self__, "impossible_travel_options", impossible_travel_options)
         if new_value_options is not None:
             pulumi.set(__self__, "new_value_options", new_value_options)
 
     @property
     @pulumi.getter(name="keepAlive")
     def keep_alive(self) -> pulumi.Input[int]:
         return pulumi.get(self, "keep_alive")
@@ -60662,24 +59901,50 @@
         return pulumi.get(self, "evaluation_window")
 
     @evaluation_window.setter
     def evaluation_window(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "evaluation_window", value)
 
     @property
+    @pulumi.getter(name="impossibleTravelOptions")
+    def impossible_travel_options(self) -> Optional[pulumi.Input['SecurityMonitoringRuleOptionsImpossibleTravelOptionsArgs']]:
+        return pulumi.get(self, "impossible_travel_options")
+
+    @impossible_travel_options.setter
+    def impossible_travel_options(self, value: Optional[pulumi.Input['SecurityMonitoringRuleOptionsImpossibleTravelOptionsArgs']]):
+        pulumi.set(self, "impossible_travel_options", value)
+
+    @property
     @pulumi.getter(name="newValueOptions")
     def new_value_options(self) -> Optional[pulumi.Input['SecurityMonitoringRuleOptionsNewValueOptionsArgs']]:
         return pulumi.get(self, "new_value_options")
 
     @new_value_options.setter
     def new_value_options(self, value: Optional[pulumi.Input['SecurityMonitoringRuleOptionsNewValueOptionsArgs']]):
         pulumi.set(self, "new_value_options", value)
 
 
 @pulumi.input_type
+class SecurityMonitoringRuleOptionsImpossibleTravelOptionsArgs:
+    def __init__(__self__, *,
+                 baseline_user_locations: Optional[pulumi.Input[bool]] = None):
+        if baseline_user_locations is not None:
+            pulumi.set(__self__, "baseline_user_locations", baseline_user_locations)
+
+    @property
+    @pulumi.getter(name="baselineUserLocations")
+    def baseline_user_locations(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "baseline_user_locations")
+
+    @baseline_user_locations.setter
+    def baseline_user_locations(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "baseline_user_locations", value)
+
+
+@pulumi.input_type
 class SecurityMonitoringRuleOptionsNewValueOptionsArgs:
     def __init__(__self__, *,
                  forget_after: pulumi.Input[int],
                  learning_duration: pulumi.Input[int]):
         pulumi.set(__self__, "forget_after", forget_after)
         pulumi.set(__self__, "learning_duration", learning_duration)
 
@@ -60831,39 +60096,29 @@
 
 
 @pulumi.input_type
 class ServiceLevelObjectiveQueryArgs:
     def __init__(__self__, *,
                  denominator: pulumi.Input[str],
                  numerator: pulumi.Input[str]):
-        """
-        :param pulumi.Input[str] denominator: The sum of the `total` events.
-        :param pulumi.Input[str] numerator: The sum of all the `good` events.
-        """
         pulumi.set(__self__, "denominator", denominator)
         pulumi.set(__self__, "numerator", numerator)
 
     @property
     @pulumi.getter
     def denominator(self) -> pulumi.Input[str]:
-        """
-        The sum of the `total` events.
-        """
         return pulumi.get(self, "denominator")
 
     @denominator.setter
     def denominator(self, value: pulumi.Input[str]):
         pulumi.set(self, "denominator", value)
 
     @property
     @pulumi.getter
     def numerator(self) -> pulumi.Input[str]:
-        """
-        The sum of all the `good` events.
-        """
         return pulumi.get(self, "numerator")
 
     @numerator.setter
     def numerator(self, value: pulumi.Input[str]):
         pulumi.set(self, "numerator", value)
 
 
@@ -60871,101 +60126,75 @@
 class ServiceLevelObjectiveThresholdArgs:
     def __init__(__self__, *,
                  target: pulumi.Input[float],
                  timeframe: pulumi.Input[str],
                  target_display: Optional[pulumi.Input[str]] = None,
                  warning: Optional[pulumi.Input[float]] = None,
                  warning_display: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[float] target: The objective's target in`[0,100]`.
-        :param pulumi.Input[str] timeframe: The time frame for the objective. The mapping from these types to the types found in the Datadog Web UI can be found in the Datadog API documentation page. Valid values are `7d`, `30d`, `90d`, `custom`.
-        :param pulumi.Input[str] target_display: A string representation of the target that indicates its precision. It uses trailing zeros to show significant decimal places (e.g. `98.00`).
-        :param pulumi.Input[float] warning: The objective's warning value in `[0,100]`. This must be greater than the target value.
-        :param pulumi.Input[str] warning_display: A string representation of the warning target (see the description of the target_display field for details).
-        """
         pulumi.set(__self__, "target", target)
         pulumi.set(__self__, "timeframe", timeframe)
         if target_display is not None:
             pulumi.set(__self__, "target_display", target_display)
         if warning is not None:
             pulumi.set(__self__, "warning", warning)
         if warning_display is not None:
             pulumi.set(__self__, "warning_display", warning_display)
 
     @property
     @pulumi.getter
     def target(self) -> pulumi.Input[float]:
-        """
-        The objective's target in`[0,100]`.
-        """
         return pulumi.get(self, "target")
 
     @target.setter
     def target(self, value: pulumi.Input[float]):
         pulumi.set(self, "target", value)
 
     @property
     @pulumi.getter
     def timeframe(self) -> pulumi.Input[str]:
-        """
-        The time frame for the objective. The mapping from these types to the types found in the Datadog Web UI can be found in the Datadog API documentation page. Valid values are `7d`, `30d`, `90d`, `custom`.
-        """
         return pulumi.get(self, "timeframe")
 
     @timeframe.setter
     def timeframe(self, value: pulumi.Input[str]):
         pulumi.set(self, "timeframe", value)
 
     @property
     @pulumi.getter(name="targetDisplay")
     def target_display(self) -> Optional[pulumi.Input[str]]:
-        """
-        A string representation of the target that indicates its precision. It uses trailing zeros to show significant decimal places (e.g. `98.00`).
-        """
         return pulumi.get(self, "target_display")
 
     @target_display.setter
     def target_display(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "target_display", value)
 
     @property
     @pulumi.getter
     def warning(self) -> Optional[pulumi.Input[float]]:
-        """
-        The objective's warning value in `[0,100]`. This must be greater than the target value.
-        """
         return pulumi.get(self, "warning")
 
     @warning.setter
     def warning(self, value: Optional[pulumi.Input[float]]):
         pulumi.set(self, "warning", value)
 
     @property
     @pulumi.getter(name="warningDisplay")
     def warning_display(self) -> Optional[pulumi.Input[str]]:
-        """
-        A string representation of the warning target (see the description of the target_display field for details).
-        """
         return pulumi.get(self, "warning_display")
 
     @warning_display.setter
     def warning_display(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "warning_display", value)
 
 
 @pulumi.input_type
 class SyntheticsGlobalVariableParseTestOptionsArgs:
     def __init__(__self__, *,
                  parser: pulumi.Input['SyntheticsGlobalVariableParseTestOptionsParserArgs'],
                  type: pulumi.Input[str],
                  field: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] type: Defines the source to use to extract the value. Valid values are `http_body`, `http_header`.
-        :param pulumi.Input[str] field: Required when type = `http_header`. Defines the header to use to extract the value
-        """
         pulumi.set(__self__, "parser", parser)
         pulumi.set(__self__, "type", type)
         if field is not None:
             pulumi.set(__self__, "field", field)
 
     @property
     @pulumi.getter
@@ -60975,44 +60204,35 @@
     @parser.setter
     def parser(self, value: pulumi.Input['SyntheticsGlobalVariableParseTestOptionsParserArgs']):
         pulumi.set(self, "parser", value)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
-        """
-        Defines the source to use to extract the value. Valid values are `http_body`, `http_header`.
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def field(self) -> Optional[pulumi.Input[str]]:
-        """
-        Required when type = `http_header`. Defines the header to use to extract the value
-        """
         return pulumi.get(self, "field")
 
     @field.setter
     def field(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "field", value)
 
 
 @pulumi.input_type
 class SyntheticsGlobalVariableParseTestOptionsParserArgs:
     def __init__(__self__, *,
                  type: pulumi.Input[str],
                  value: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] value: The value of the global variable.
-        """
         pulumi.set(__self__, "type", type)
         if value is not None:
             pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
@@ -61021,25 +60241,39 @@
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def value(self) -> Optional[pulumi.Input[str]]:
-        """
-        The value of the global variable.
-        """
         return pulumi.get(self, "value")
 
     @value.setter
     def value(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "value", value)
 
 
 @pulumi.input_type
+class SyntheticsPrivateLocationMetadataArgs:
+    def __init__(__self__, *,
+                 restricted_roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
+        if restricted_roles is not None:
+            pulumi.set(__self__, "restricted_roles", restricted_roles)
+
+    @property
+    @pulumi.getter(name="restrictedRoles")
+    def restricted_roles(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        return pulumi.get(self, "restricted_roles")
+
+    @restricted_roles.setter
+    def restricted_roles(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "restricted_roles", value)
+
+
+@pulumi.input_type
 class SyntheticsTestApiStepArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  allow_failure: Optional[pulumi.Input[bool]] = None,
                  assertions: Optional[pulumi.Input[Sequence[pulumi.Input['SyntheticsTestApiStepAssertionArgs']]]] = None,
                  extracted_values: Optional[pulumi.Input[Sequence[pulumi.Input['SyntheticsTestApiStepExtractedValueArgs']]]] = None,
                  is_critical: Optional[pulumi.Input[bool]] = None,
@@ -61047,28 +60281,14 @@
                  request_client_certificate: Optional[pulumi.Input['SyntheticsTestApiStepRequestClientCertificateArgs']] = None,
                  request_definition: Optional[pulumi.Input['SyntheticsTestApiStepRequestDefinitionArgs']] = None,
                  request_headers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  request_proxy: Optional[pulumi.Input['SyntheticsTestApiStepRequestProxyArgs']] = None,
                  request_query: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  retry: Optional[pulumi.Input['SyntheticsTestApiStepRetryArgs']] = None,
                  subtype: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] name: The name of the step.
-        :param pulumi.Input[bool] allow_failure: Determines whether or not to continue with test if this step fails.
-        :param pulumi.Input[Sequence[pulumi.Input['SyntheticsTestApiStepAssertionArgs']]] assertions: Assertions used for the test. Multiple `assertion` blocks are allowed with the structure below.
-        :param pulumi.Input[Sequence[pulumi.Input['SyntheticsTestApiStepExtractedValueArgs']]] extracted_values: Values to parse and save as variables from the response.
-        :param pulumi.Input[bool] is_critical: Determines whether or not to consider the entire test as failed if this step fails. Can be used only if `allow_failure` is `true`.
-        :param pulumi.Input['SyntheticsTestApiStepRequestBasicauthArgs'] request_basicauth: The HTTP basic authentication credentials. Exactly one nested block is allowed with the structure below.
-        :param pulumi.Input['SyntheticsTestApiStepRequestClientCertificateArgs'] request_client_certificate: Client certificate to use when performing the test request. Exactly one nested block is allowed with the structure below.
-        :param pulumi.Input['SyntheticsTestApiStepRequestDefinitionArgs'] request_definition: The request for the api step.
-        :param pulumi.Input[Mapping[str, Any]] request_headers: Header name and value map.
-        :param pulumi.Input['SyntheticsTestApiStepRequestProxyArgs'] request_proxy: The proxy to perform the test.
-        :param pulumi.Input[Mapping[str, Any]] request_query: Query arguments name and value map.
-        :param pulumi.Input[str] subtype: The subtype of the Synthetic multistep API test step. Valid values are `http`.
-        """
         pulumi.set(__self__, "name", name)
         if allow_failure is not None:
             pulumi.set(__self__, "allow_failure", allow_failure)
         if assertions is not None:
             pulumi.set(__self__, "assertions", assertions)
         if extracted_values is not None:
             pulumi.set(__self__, "extracted_values", extracted_values)
@@ -61090,137 +60310,104 @@
             pulumi.set(__self__, "retry", retry)
         if subtype is not None:
             pulumi.set(__self__, "subtype", subtype)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
-        """
-        The name of the step.
-        """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="allowFailure")
     def allow_failure(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Determines whether or not to continue with test if this step fails.
-        """
         return pulumi.get(self, "allow_failure")
 
     @allow_failure.setter
     def allow_failure(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "allow_failure", value)
 
     @property
     @pulumi.getter
     def assertions(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['SyntheticsTestApiStepAssertionArgs']]]]:
-        """
-        Assertions used for the test. Multiple `assertion` blocks are allowed with the structure below.
-        """
         return pulumi.get(self, "assertions")
 
     @assertions.setter
     def assertions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SyntheticsTestApiStepAssertionArgs']]]]):
         pulumi.set(self, "assertions", value)
 
     @property
     @pulumi.getter(name="extractedValues")
     def extracted_values(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['SyntheticsTestApiStepExtractedValueArgs']]]]:
-        """
-        Values to parse and save as variables from the response.
-        """
         return pulumi.get(self, "extracted_values")
 
     @extracted_values.setter
     def extracted_values(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SyntheticsTestApiStepExtractedValueArgs']]]]):
         pulumi.set(self, "extracted_values", value)
 
     @property
     @pulumi.getter(name="isCritical")
     def is_critical(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Determines whether or not to consider the entire test as failed if this step fails. Can be used only if `allow_failure` is `true`.
-        """
         return pulumi.get(self, "is_critical")
 
     @is_critical.setter
     def is_critical(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "is_critical", value)
 
     @property
     @pulumi.getter(name="requestBasicauth")
     def request_basicauth(self) -> Optional[pulumi.Input['SyntheticsTestApiStepRequestBasicauthArgs']]:
-        """
-        The HTTP basic authentication credentials. Exactly one nested block is allowed with the structure below.
-        """
         return pulumi.get(self, "request_basicauth")
 
     @request_basicauth.setter
     def request_basicauth(self, value: Optional[pulumi.Input['SyntheticsTestApiStepRequestBasicauthArgs']]):
         pulumi.set(self, "request_basicauth", value)
 
     @property
     @pulumi.getter(name="requestClientCertificate")
     def request_client_certificate(self) -> Optional[pulumi.Input['SyntheticsTestApiStepRequestClientCertificateArgs']]:
-        """
-        Client certificate to use when performing the test request. Exactly one nested block is allowed with the structure below.
-        """
         return pulumi.get(self, "request_client_certificate")
 
     @request_client_certificate.setter
     def request_client_certificate(self, value: Optional[pulumi.Input['SyntheticsTestApiStepRequestClientCertificateArgs']]):
         pulumi.set(self, "request_client_certificate", value)
 
     @property
     @pulumi.getter(name="requestDefinition")
     def request_definition(self) -> Optional[pulumi.Input['SyntheticsTestApiStepRequestDefinitionArgs']]:
-        """
-        The request for the api step.
-        """
         return pulumi.get(self, "request_definition")
 
     @request_definition.setter
     def request_definition(self, value: Optional[pulumi.Input['SyntheticsTestApiStepRequestDefinitionArgs']]):
         pulumi.set(self, "request_definition", value)
 
     @property
     @pulumi.getter(name="requestHeaders")
     def request_headers(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
-        """
-        Header name and value map.
-        """
         return pulumi.get(self, "request_headers")
 
     @request_headers.setter
     def request_headers(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "request_headers", value)
 
     @property
     @pulumi.getter(name="requestProxy")
     def request_proxy(self) -> Optional[pulumi.Input['SyntheticsTestApiStepRequestProxyArgs']]:
-        """
-        The proxy to perform the test.
-        """
         return pulumi.get(self, "request_proxy")
 
     @request_proxy.setter
     def request_proxy(self, value: Optional[pulumi.Input['SyntheticsTestApiStepRequestProxyArgs']]):
         pulumi.set(self, "request_proxy", value)
 
     @property
     @pulumi.getter(name="requestQuery")
     def request_query(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
-        """
-        Query arguments name and value map.
-        """
         return pulumi.get(self, "request_query")
 
     @request_query.setter
     def request_query(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "request_query", value)
 
     @property
@@ -61231,17 +60418,14 @@
     @retry.setter
     def retry(self, value: Optional[pulumi.Input['SyntheticsTestApiStepRetryArgs']]):
         pulumi.set(self, "retry", value)
 
     @property
     @pulumi.getter
     def subtype(self) -> Optional[pulumi.Input[str]]:
-        """
-        The subtype of the Synthetic multistep API test step. Valid values are `http`.
-        """
         return pulumi.get(self, "subtype")
 
     @subtype.setter
     def subtype(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "subtype", value)
 
 
@@ -61249,84 +60433,62 @@
 class SyntheticsTestApiStepAssertionArgs:
     def __init__(__self__, *,
                  operator: pulumi.Input[str],
                  type: pulumi.Input[str],
                  property: Optional[pulumi.Input[str]] = None,
                  target: Optional[pulumi.Input[str]] = None,
                  targetjsonpath: Optional[pulumi.Input['SyntheticsTestApiStepAssertionTargetjsonpathArgs']] = None):
-        """
-        :param pulumi.Input[str] operator: Assertion operator. **Note** Only some combinations of `type` and `operator` are valid (please refer to [Datadog documentation](https://docs.datadoghq.com/api/latest/synthetics/#create-a-test)).
-        :param pulumi.Input[str] type: Type of assertion. **Note** Only some combinations of `type` and `operator` are valid (please refer to [Datadog documentation](https://docs.datadoghq.com/api/latest/synthetics/#create-a-test)). Valid values are `body`, `header`, `statusCode`, `certificate`, `responseTime`, `property`, `recordEvery`, `recordSome`, `tlsVersion`, `minTlsVersion`, `latency`, `packetLossPercentage`, `packetsReceived`, `networkHop`, `receivedMessage`.
-        :param pulumi.Input[str] property: If assertion type is `header`, this is the header name.
-        :param pulumi.Input[str] target: Expected value. Depends on the assertion type, refer to [Datadog documentation](https://docs.datadoghq.com/api/latest/synthetics/#create-a-test) for details.
-        :param pulumi.Input['SyntheticsTestApiStepAssertionTargetjsonpathArgs'] targetjsonpath: Expected structure if `operator` is `validatesJSONPath`. Exactly one nested block is allowed with the structure below.
-        """
         pulumi.set(__self__, "operator", operator)
         pulumi.set(__self__, "type", type)
         if property is not None:
             pulumi.set(__self__, "property", property)
         if target is not None:
             pulumi.set(__self__, "target", target)
         if targetjsonpath is not None:
             pulumi.set(__self__, "targetjsonpath", targetjsonpath)
 
     @property
     @pulumi.getter
     def operator(self) -> pulumi.Input[str]:
-        """
-        Assertion operator. **Note** Only some combinations of `type` and `operator` are valid (please refer to [Datadog documentation](https://docs.datadoghq.com/api/latest/synthetics/#create-a-test)).
-        """
         return pulumi.get(self, "operator")
 
     @operator.setter
     def operator(self, value: pulumi.Input[str]):
         pulumi.set(self, "operator", value)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
-        """
-        Type of assertion. **Note** Only some combinations of `type` and `operator` are valid (please refer to [Datadog documentation](https://docs.datadoghq.com/api/latest/synthetics/#create-a-test)). Valid values are `body`, `header`, `statusCode`, `certificate`, `responseTime`, `property`, `recordEvery`, `recordSome`, `tlsVersion`, `minTlsVersion`, `latency`, `packetLossPercentage`, `packetsReceived`, `networkHop`, `receivedMessage`.
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def target(self) -> Optional[pulumi.Input[str]]:
-        """
-        Expected value. Depends on the assertion type, refer to [Datadog documentation](https://docs.datadoghq.com/api/latest/synthetics/#create-a-test) for details.
-        """
         return pulumi.get(self, "target")
 
     @target.setter
     def target(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "target", value)
 
     @property
     @pulumi.getter
     def targetjsonpath(self) -> Optional[pulumi.Input['SyntheticsTestApiStepAssertionTargetjsonpathArgs']]:
-        """
-        Expected structure if `operator` is `validatesJSONPath`. Exactly one nested block is allowed with the structure below.
-        """
         return pulumi.get(self, "targetjsonpath")
 
     @targetjsonpath.setter
     def targetjsonpath(self, value: Optional[pulumi.Input['SyntheticsTestApiStepAssertionTargetjsonpathArgs']]):
         pulumi.set(self, "targetjsonpath", value)
 
     @property
     @pulumi.getter
     def property(self) -> Optional[pulumi.Input[str]]:
-        """
-        If assertion type is `header`, this is the header name.
-        """
         return pulumi.get(self, "property")
 
     @property.setter
     def property(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "property", value)
 
 
@@ -61371,30 +60533,23 @@
 @pulumi.input_type
 class SyntheticsTestApiStepExtractedValueArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  parser: pulumi.Input['SyntheticsTestApiStepExtractedValueParserArgs'],
                  type: pulumi.Input[str],
                  field: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] name: Name of Datadog synthetics test.
-        :param pulumi.Input[str] type: Synthetics test type. Valid values are `api`, `browser`.
-        """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "parser", parser)
         pulumi.set(__self__, "type", type)
         if field is not None:
             pulumi.set(__self__, "field", field)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
-        """
-        Name of Datadog synthetics test.
-        """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
@@ -61405,17 +60560,14 @@
     @parser.setter
     def parser(self, value: pulumi.Input['SyntheticsTestApiStepExtractedValueParserArgs']):
         pulumi.set(self, "parser", value)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
-        """
-        Synthetics test type. Valid values are `api`, `browser`.
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
@@ -61429,27 +60581,21 @@
 
 
 @pulumi.input_type
 class SyntheticsTestApiStepExtractedValueParserArgs:
     def __init__(__self__, *,
                  type: pulumi.Input[str],
                  value: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] type: Synthetics test type. Valid values are `api`, `browser`.
-        """
         pulumi.set(__self__, "type", type)
         if value is not None:
             pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
-        """
-        Synthetics test type. Valid values are `api`, `browser`.
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
@@ -61471,26 +60617,14 @@
                  region: Optional[pulumi.Input[str]] = None,
                  secret_key: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  session_token: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  workstation: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] access_key: Access key for `SIGV4` authentication.
-        :param pulumi.Input[str] domain: Domain for `ntlm` authentication.
-        :param pulumi.Input[str] password: Password for authentication.
-        :param pulumi.Input[str] region: Region for `SIGV4` authentication.
-        :param pulumi.Input[str] secret_key: Secret key for `SIGV4` authentication.
-        :param pulumi.Input[str] service_name: Service name for `SIGV4` authentication.
-        :param pulumi.Input[str] session_token: Session token for `SIGV4` authentication.
-        :param pulumi.Input[str] type: Type of basic authentication to use when performing the test.
-        :param pulumi.Input[str] username: Username for authentication.
-        :param pulumi.Input[str] workstation: Workstation for `ntlm` authentication.
-        """
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if domain is not None:
             pulumi.set(__self__, "domain", domain)
         if password is not None:
             pulumi.set(__self__, "password", password)
         if region is not None:
@@ -61507,125 +60641,95 @@
             pulumi.set(__self__, "username", username)
         if workstation is not None:
             pulumi.set(__self__, "workstation", workstation)
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[pulumi.Input[str]]:
-        """
-        Access key for `SIGV4` authentication.
-        """
         return pulumi.get(self, "access_key")
 
     @access_key.setter
     def access_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "access_key", value)
 
     @property
     @pulumi.getter
     def domain(self) -> Optional[pulumi.Input[str]]:
-        """
-        Domain for `ntlm` authentication.
-        """
         return pulumi.get(self, "domain")
 
     @domain.setter
     def domain(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "domain", value)
 
     @property
     @pulumi.getter
     def password(self) -> Optional[pulumi.Input[str]]:
-        """
-        Password for authentication.
-        """
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "password", value)
 
     @property
     @pulumi.getter
     def region(self) -> Optional[pulumi.Input[str]]:
-        """
-        Region for `SIGV4` authentication.
-        """
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
     @property
     @pulumi.getter(name="secretKey")
     def secret_key(self) -> Optional[pulumi.Input[str]]:
-        """
-        Secret key for `SIGV4` authentication.
-        """
         return pulumi.get(self, "secret_key")
 
     @secret_key.setter
     def secret_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_key", value)
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        Service name for `SIGV4` authentication.
-        """
         return pulumi.get(self, "service_name")
 
     @service_name.setter
     def service_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_name", value)
 
     @property
     @pulumi.getter(name="sessionToken")
     def session_token(self) -> Optional[pulumi.Input[str]]:
-        """
-        Session token for `SIGV4` authentication.
-        """
         return pulumi.get(self, "session_token")
 
     @session_token.setter
     def session_token(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "session_token", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
-        """
-        Type of basic authentication to use when performing the test.
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def username(self) -> Optional[pulumi.Input[str]]:
-        """
-        Username for authentication.
-        """
         return pulumi.get(self, "username")
 
     @username.setter
     def username(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "username", value)
 
     @property
     @pulumi.getter
     def workstation(self) -> Optional[pulumi.Input[str]]:
-        """
-        Workstation for `ntlm` authentication.
-        """
         return pulumi.get(self, "workstation")
 
     @workstation.setter
     def workstation(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "workstation", value)
 
 
@@ -61726,29 +60830,14 @@
                  no_saving_response_body: Optional[pulumi.Input[bool]] = None,
                  number_of_packets: Optional[pulumi.Input[int]] = None,
                  port: Optional[pulumi.Input[int]] = None,
                  servername: Optional[pulumi.Input[str]] = None,
                  should_track_hops: Optional[pulumi.Input[bool]] = None,
                  timeout: Optional[pulumi.Input[int]] = None,
                  url: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] body: The request body.
-        :param pulumi.Input[str] dns_server: DNS server to use for DNS tests (`subtype = "dns"`).
-        :param pulumi.Input[int] dns_server_port: DNS server port to use for DNS tests.
-        :param pulumi.Input[str] host: Host name to perform the test with.
-        :param pulumi.Input[str] message: For UDP and websocket tests, message to send with the request.
-        :param pulumi.Input[str] method: The HTTP method. Valid values are `GET`, `POST`, `PATCH`, `PUT`, `DELETE`, `HEAD`, `OPTIONS`.
-        :param pulumi.Input[bool] no_saving_response_body: Determines whether or not to save the response body.
-        :param pulumi.Input[int] number_of_packets: Number of pings to use per test for ICMP tests (`subtype = "icmp"`) between 0 and 10.
-        :param pulumi.Input[int] port: Port to use when performing the test.
-        :param pulumi.Input[str] servername: For SSL tests, it specifies on which server you want to initiate the TLS handshake, allowing the server to present one of multiple possible certificates on the same IP address and TCP port number.
-        :param pulumi.Input[bool] should_track_hops: This will turn on a traceroute probe to discover all gateways along the path to the host destination. For ICMP tests (`subtype = "icmp"`).
-        :param pulumi.Input[int] timeout: Timeout in seconds for the test. Defaults to `60`.
-        :param pulumi.Input[str] url: The URL to send the request to.
-        """
         if allow_insecure is not None:
             pulumi.set(__self__, "allow_insecure", allow_insecure)
         if body is not None:
             pulumi.set(__self__, "body", body)
         if dns_server is not None:
             pulumi.set(__self__, "dns_server", dns_server)
         if dns_server_port is not None:
@@ -61784,41 +60873,32 @@
     @allow_insecure.setter
     def allow_insecure(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "allow_insecure", value)
 
     @property
     @pulumi.getter
     def body(self) -> Optional[pulumi.Input[str]]:
-        """
-        The request body.
-        """
         return pulumi.get(self, "body")
 
     @body.setter
     def body(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "body", value)
 
     @property
     @pulumi.getter(name="dnsServer")
     def dns_server(self) -> Optional[pulumi.Input[str]]:
-        """
-        DNS server to use for DNS tests (`subtype = "dns"`).
-        """
         return pulumi.get(self, "dns_server")
 
     @dns_server.setter
     def dns_server(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "dns_server", value)
 
     @property
     @pulumi.getter(name="dnsServerPort")
     def dns_server_port(self) -> Optional[pulumi.Input[int]]:
-        """
-        DNS server port to use for DNS tests.
-        """
         return pulumi.get(self, "dns_server_port")
 
     @dns_server_port.setter
     def dns_server_port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "dns_server_port", value)
 
     @property
@@ -61829,163 +60909,123 @@
     @follow_redirects.setter
     def follow_redirects(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "follow_redirects", value)
 
     @property
     @pulumi.getter
     def host(self) -> Optional[pulumi.Input[str]]:
-        """
-        Host name to perform the test with.
-        """
         return pulumi.get(self, "host")
 
     @host.setter
     def host(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "host", value)
 
     @property
     @pulumi.getter
     def message(self) -> Optional[pulumi.Input[str]]:
-        """
-        For UDP and websocket tests, message to send with the request.
-        """
         return pulumi.get(self, "message")
 
     @message.setter
     def message(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "message", value)
 
     @property
     @pulumi.getter
     def method(self) -> Optional[pulumi.Input[str]]:
-        """
-        The HTTP method. Valid values are `GET`, `POST`, `PATCH`, `PUT`, `DELETE`, `HEAD`, `OPTIONS`.
-        """
         return pulumi.get(self, "method")
 
     @method.setter
     def method(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "method", value)
 
     @property
     @pulumi.getter(name="noSavingResponseBody")
     def no_saving_response_body(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Determines whether or not to save the response body.
-        """
         return pulumi.get(self, "no_saving_response_body")
 
     @no_saving_response_body.setter
     def no_saving_response_body(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "no_saving_response_body", value)
 
     @property
     @pulumi.getter(name="numberOfPackets")
     def number_of_packets(self) -> Optional[pulumi.Input[int]]:
-        """
-        Number of pings to use per test for ICMP tests (`subtype = "icmp"`) between 0 and 10.
-        """
         return pulumi.get(self, "number_of_packets")
 
     @number_of_packets.setter
     def number_of_packets(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "number_of_packets", value)
 
     @property
     @pulumi.getter
     def port(self) -> Optional[pulumi.Input[int]]:
-        """
-        Port to use when performing the test.
-        """
         return pulumi.get(self, "port")
 
     @port.setter
     def port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "port", value)
 
     @property
     @pulumi.getter
     def servername(self) -> Optional[pulumi.Input[str]]:
-        """
-        For SSL tests, it specifies on which server you want to initiate the TLS handshake, allowing the server to present one of multiple possible certificates on the same IP address and TCP port number.
-        """
         return pulumi.get(self, "servername")
 
     @servername.setter
     def servername(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "servername", value)
 
     @property
     @pulumi.getter(name="shouldTrackHops")
     def should_track_hops(self) -> Optional[pulumi.Input[bool]]:
-        """
-        This will turn on a traceroute probe to discover all gateways along the path to the host destination. For ICMP tests (`subtype = "icmp"`).
-        """
         return pulumi.get(self, "should_track_hops")
 
     @should_track_hops.setter
     def should_track_hops(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "should_track_hops", value)
 
     @property
     @pulumi.getter
     def timeout(self) -> Optional[pulumi.Input[int]]:
-        """
-        Timeout in seconds for the test. Defaults to `60`.
-        """
         return pulumi.get(self, "timeout")
 
     @timeout.setter
     def timeout(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "timeout", value)
 
     @property
     @pulumi.getter
     def url(self) -> Optional[pulumi.Input[str]]:
-        """
-        The URL to send the request to.
-        """
         return pulumi.get(self, "url")
 
     @url.setter
     def url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "url", value)
 
 
 @pulumi.input_type
 class SyntheticsTestApiStepRequestProxyArgs:
     def __init__(__self__, *,
                  url: pulumi.Input[str],
                  headers: Optional[pulumi.Input[Mapping[str, Any]]] = None):
-        """
-        :param pulumi.Input[str] url: URL of the proxy to perform the test.
-        :param pulumi.Input[Mapping[str, Any]] headers: Header name and value map.
-        """
         pulumi.set(__self__, "url", url)
         if headers is not None:
             pulumi.set(__self__, "headers", headers)
 
     @property
     @pulumi.getter
     def url(self) -> pulumi.Input[str]:
-        """
-        URL of the proxy to perform the test.
-        """
         return pulumi.get(self, "url")
 
     @url.setter
     def url(self, value: pulumi.Input[str]):
         pulumi.set(self, "url", value)
 
     @property
     @pulumi.getter
     def headers(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
-        """
-        Header name and value map.
-        """
         return pulumi.get(self, "headers")
 
     @headers.setter
     def headers(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "headers", value)
 
 
@@ -62022,84 +61062,62 @@
 class SyntheticsTestAssertionArgs:
     def __init__(__self__, *,
                  operator: pulumi.Input[str],
                  type: pulumi.Input[str],
                  property: Optional[pulumi.Input[str]] = None,
                  target: Optional[pulumi.Input[str]] = None,
                  targetjsonpath: Optional[pulumi.Input['SyntheticsTestAssertionTargetjsonpathArgs']] = None):
-        """
-        :param pulumi.Input[str] operator: Assertion operator. **Note** Only some combinations of `type` and `operator` are valid (please refer to [Datadog documentation](https://docs.datadoghq.com/api/latest/synthetics/#create-a-test)).
-        :param pulumi.Input[str] type: Type of assertion. **Note** Only some combinations of `type` and `operator` are valid (please refer to [Datadog documentation](https://docs.datadoghq.com/api/latest/synthetics/#create-a-test)). Valid values are `body`, `header`, `statusCode`, `certificate`, `responseTime`, `property`, `recordEvery`, `recordSome`, `tlsVersion`, `minTlsVersion`, `latency`, `packetLossPercentage`, `packetsReceived`, `networkHop`, `receivedMessage`.
-        :param pulumi.Input[str] property: If assertion type is `header`, this is the header name.
-        :param pulumi.Input[str] target: Expected value. Depends on the assertion type, refer to [Datadog documentation](https://docs.datadoghq.com/api/latest/synthetics/#create-a-test) for details.
-        :param pulumi.Input['SyntheticsTestAssertionTargetjsonpathArgs'] targetjsonpath: Expected structure if `operator` is `validatesJSONPath`. Exactly one nested block is allowed with the structure below.
-        """
         pulumi.set(__self__, "operator", operator)
         pulumi.set(__self__, "type", type)
         if property is not None:
             pulumi.set(__self__, "property", property)
         if target is not None:
             pulumi.set(__self__, "target", target)
         if targetjsonpath is not None:
             pulumi.set(__self__, "targetjsonpath", targetjsonpath)
 
     @property
     @pulumi.getter
     def operator(self) -> pulumi.Input[str]:
-        """
-        Assertion operator. **Note** Only some combinations of `type` and `operator` are valid (please refer to [Datadog documentation](https://docs.datadoghq.com/api/latest/synthetics/#create-a-test)).
-        """
         return pulumi.get(self, "operator")
 
     @operator.setter
     def operator(self, value: pulumi.Input[str]):
         pulumi.set(self, "operator", value)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
-        """
-        Type of assertion. **Note** Only some combinations of `type` and `operator` are valid (please refer to [Datadog documentation](https://docs.datadoghq.com/api/latest/synthetics/#create-a-test)). Valid values are `body`, `header`, `statusCode`, `certificate`, `responseTime`, `property`, `recordEvery`, `recordSome`, `tlsVersion`, `minTlsVersion`, `latency`, `packetLossPercentage`, `packetsReceived`, `networkHop`, `receivedMessage`.
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def target(self) -> Optional[pulumi.Input[str]]:
-        """
-        Expected value. Depends on the assertion type, refer to [Datadog documentation](https://docs.datadoghq.com/api/latest/synthetics/#create-a-test) for details.
-        """
         return pulumi.get(self, "target")
 
     @target.setter
     def target(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "target", value)
 
     @property
     @pulumi.getter
     def targetjsonpath(self) -> Optional[pulumi.Input['SyntheticsTestAssertionTargetjsonpathArgs']]:
-        """
-        Expected structure if `operator` is `validatesJSONPath`. Exactly one nested block is allowed with the structure below.
-        """
         return pulumi.get(self, "targetjsonpath")
 
     @targetjsonpath.setter
     def targetjsonpath(self, value: Optional[pulumi.Input['SyntheticsTestAssertionTargetjsonpathArgs']]):
         pulumi.set(self, "targetjsonpath", value)
 
     @property
     @pulumi.getter
     def property(self) -> Optional[pulumi.Input[str]]:
-        """
-        If assertion type is `header`, this is the header name.
-        """
         return pulumi.get(self, "property")
 
     @property.setter
     def property(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "property", value)
 
 
@@ -62147,23 +61165,14 @@
                  name: pulumi.Input[str],
                  params: pulumi.Input['SyntheticsTestBrowserStepParamsArgs'],
                  type: pulumi.Input[str],
                  allow_failure: Optional[pulumi.Input[bool]] = None,
                  force_element_update: Optional[pulumi.Input[bool]] = None,
                  is_critical: Optional[pulumi.Input[bool]] = None,
                  timeout: Optional[pulumi.Input[int]] = None):
-        """
-        :param pulumi.Input[str] name: Name of the step.
-        :param pulumi.Input['SyntheticsTestBrowserStepParamsArgs'] params: Parameters for the step.
-        :param pulumi.Input[str] type: Type of the step. Valid values are `assertCurrentUrl`, `assertElementAttribute`, `assertElementContent`, `assertElementPresent`, `assertEmail`, `assertFileDownload`, `assertFromJavascript`, `assertPageContains`, `assertPageLacks`, `click`, `extractFromJavascript`, `extractVariable`, `goToEmailLink`, `goToUrl`, `goToUrlAndMeasureTti`, `hover`, `playSubTest`, `pressKey`, `refresh`, `runApiTest`, `scroll`, `selectOption`, `typeText`, `uploadFiles`, `wait`.
-        :param pulumi.Input[bool] allow_failure: Determines if the step should be allowed to fail.
-        :param pulumi.Input[bool] force_element_update: Force update of the "element" parameter for the step
-        :param pulumi.Input[bool] is_critical: Determines whether or not to consider the entire test as failed if this step fails. Can be used only if `allow_failure` is `true`.
-        :param pulumi.Input[int] timeout: Used to override the default timeout of a step.
-        """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "params", params)
         pulumi.set(__self__, "type", type)
         if allow_failure is not None:
             pulumi.set(__self__, "allow_failure", allow_failure)
         if force_element_update is not None:
             pulumi.set(__self__, "force_element_update", force_element_update)
@@ -62171,89 +61180,68 @@
             pulumi.set(__self__, "is_critical", is_critical)
         if timeout is not None:
             pulumi.set(__self__, "timeout", timeout)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
-        """
-        Name of the step.
-        """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def params(self) -> pulumi.Input['SyntheticsTestBrowserStepParamsArgs']:
-        """
-        Parameters for the step.
-        """
         return pulumi.get(self, "params")
 
     @params.setter
     def params(self, value: pulumi.Input['SyntheticsTestBrowserStepParamsArgs']):
         pulumi.set(self, "params", value)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
-        """
-        Type of the step. Valid values are `assertCurrentUrl`, `assertElementAttribute`, `assertElementContent`, `assertElementPresent`, `assertEmail`, `assertFileDownload`, `assertFromJavascript`, `assertPageContains`, `assertPageLacks`, `click`, `extractFromJavascript`, `extractVariable`, `goToEmailLink`, `goToUrl`, `goToUrlAndMeasureTti`, `hover`, `playSubTest`, `pressKey`, `refresh`, `runApiTest`, `scroll`, `selectOption`, `typeText`, `uploadFiles`, `wait`.
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter(name="allowFailure")
     def allow_failure(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Determines if the step should be allowed to fail.
-        """
         return pulumi.get(self, "allow_failure")
 
     @allow_failure.setter
     def allow_failure(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "allow_failure", value)
 
     @property
     @pulumi.getter(name="forceElementUpdate")
     def force_element_update(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Force update of the "element" parameter for the step
-        """
         return pulumi.get(self, "force_element_update")
 
     @force_element_update.setter
     def force_element_update(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "force_element_update", value)
 
     @property
     @pulumi.getter(name="isCritical")
     def is_critical(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Determines whether or not to consider the entire test as failed if this step fails. Can be used only if `allow_failure` is `true`.
-        """
         return pulumi.get(self, "is_critical")
 
     @is_critical.setter
     def is_critical(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "is_critical", value)
 
     @property
     @pulumi.getter
     def timeout(self) -> Optional[pulumi.Input[int]]:
-        """
-        Used to override the default timeout of a step.
-        """
         return pulumi.get(self, "timeout")
 
     @timeout.setter
     def timeout(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "timeout", value)
 
 
@@ -62519,17 +61507,14 @@
 
 
 @pulumi.input_type
 class SyntheticsTestBrowserStepParamsElementUserLocatorValueArgs:
     def __init__(__self__, *,
                  value: pulumi.Input[str],
                  type: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] type: Synthetics test type. Valid values are `api`, `browser`.
-        """
         pulumi.set(__self__, "value", value)
         if type is not None:
             pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
     def value(self) -> pulumi.Input[str]:
@@ -62538,32 +61523,26 @@
     @value.setter
     def value(self, value: pulumi.Input[str]):
         pulumi.set(self, "value", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
-        """
-        Synthetics test type. Valid values are `api`, `browser`.
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
 
 @pulumi.input_type
 class SyntheticsTestBrowserStepParamsVariableArgs:
     def __init__(__self__, *,
                  example: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] name: Name of Datadog synthetics test.
-        """
         if example is not None:
             pulumi.set(__self__, "example", example)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
@@ -62573,17 +61552,14 @@
     @example.setter
     def example(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "example", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
-        """
-        Name of Datadog synthetics test.
-        """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
 
@@ -62591,84 +61567,62 @@
 class SyntheticsTestBrowserVariableArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  type: pulumi.Input[str],
                  example: Optional[pulumi.Input[str]] = None,
                  id: Optional[pulumi.Input[str]] = None,
                  pattern: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] name: Name of the variable.
-        :param pulumi.Input[str] type: Type of browser test variable. Valid values are `element`, `email`, `global`, `javascript`, `text`.
-        :param pulumi.Input[str] example: Example for the variable.
-        :param pulumi.Input[str] id: ID of the global variable to use. This is actually only used (and required) in the case of using a variable of type `global`.
-        :param pulumi.Input[str] pattern: Pattern of the variable.
-        """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "type", type)
         if example is not None:
             pulumi.set(__self__, "example", example)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if pattern is not None:
             pulumi.set(__self__, "pattern", pattern)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
-        """
-        Name of the variable.
-        """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
-        """
-        Type of browser test variable. Valid values are `element`, `email`, `global`, `javascript`, `text`.
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def example(self) -> Optional[pulumi.Input[str]]:
-        """
-        Example for the variable.
-        """
         return pulumi.get(self, "example")
 
     @example.setter
     def example(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "example", value)
 
     @property
     @pulumi.getter
     def id(self) -> Optional[pulumi.Input[str]]:
-        """
-        ID of the global variable to use. This is actually only used (and required) in the case of using a variable of type `global`.
-        """
         return pulumi.get(self, "id")
 
     @id.setter
     def id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "id", value)
 
     @property
     @pulumi.getter
     def pattern(self) -> Optional[pulumi.Input[str]]:
-        """
-        Pattern of the variable.
-        """
         return pulumi.get(self, "pattern")
 
     @pattern.setter
     def pattern(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "pattern", value)
 
 
@@ -62676,84 +61630,62 @@
 class SyntheticsTestConfigVariableArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  type: pulumi.Input[str],
                  example: Optional[pulumi.Input[str]] = None,
                  id: Optional[pulumi.Input[str]] = None,
                  pattern: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] name: Name of the variable.
-        :param pulumi.Input[str] type: Type of test configuration variable. Valid values are `global`, `text`.
-        :param pulumi.Input[str] example: Example for the variable.
-        :param pulumi.Input[str] id: When type = `global`, ID of the global variable to use.
-        :param pulumi.Input[str] pattern: Pattern of the variable.
-        """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "type", type)
         if example is not None:
             pulumi.set(__self__, "example", example)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if pattern is not None:
             pulumi.set(__self__, "pattern", pattern)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
-        """
-        Name of the variable.
-        """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
-        """
-        Type of test configuration variable. Valid values are `global`, `text`.
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def example(self) -> Optional[pulumi.Input[str]]:
-        """
-        Example for the variable.
-        """
         return pulumi.get(self, "example")
 
     @example.setter
     def example(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "example", value)
 
     @property
     @pulumi.getter
     def id(self) -> Optional[pulumi.Input[str]]:
-        """
-        When type = `global`, ID of the global variable to use.
-        """
         return pulumi.get(self, "id")
 
     @id.setter
     def id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "id", value)
 
     @property
     @pulumi.getter
     def pattern(self) -> Optional[pulumi.Input[str]]:
-        """
-        Pattern of the variable.
-        """
         return pulumi.get(self, "pattern")
 
     @pattern.setter
     def pattern(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "pattern", value)
 
 
@@ -62767,26 +61699,16 @@
                  follow_redirects: Optional[pulumi.Input[bool]] = None,
                  min_failure_duration: Optional[pulumi.Input[int]] = None,
                  min_location_failed: Optional[pulumi.Input[int]] = None,
                  monitor_name: Optional[pulumi.Input[str]] = None,
                  monitor_options: Optional[pulumi.Input['SyntheticsTestOptionsListMonitorOptionsArgs']] = None,
                  monitor_priority: Optional[pulumi.Input[int]] = None,
                  no_screenshot: Optional[pulumi.Input[bool]] = None,
+                 restricted_roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  retry: Optional[pulumi.Input['SyntheticsTestOptionsListRetryArgs']] = None):
-        """
-        :param pulumi.Input[int] tick_every: How often the test should run (in seconds).
-        :param pulumi.Input[bool] accept_self_signed: For SSL test, whether or not the test should allow self signed certificates.
-        :param pulumi.Input[bool] allow_insecure: Allows loading insecure content for an HTTP test.
-        :param pulumi.Input[bool] check_certificate_revocation: For SSL test, whether or not the test should fail on revoked certificate in stapled OCSP.
-        :param pulumi.Input[bool] follow_redirects: Determines whether or not the API HTTP test should follow redirects.
-        :param pulumi.Input[int] min_failure_duration: Minimum amount of time in failure required to trigger an alert. Default is `0`.
-        :param pulumi.Input[int] min_location_failed: Minimum number of locations in failure required to trigger an alert. Default is `1`.
-        :param pulumi.Input[str] monitor_name: The monitor name is used for the alert title as well as for all monitor dashboard widgets and SLOs.
-        :param pulumi.Input[bool] no_screenshot: Prevents saving screenshots of the steps.
-        """
         pulumi.set(__self__, "tick_every", tick_every)
         if accept_self_signed is not None:
             pulumi.set(__self__, "accept_self_signed", accept_self_signed)
         if allow_insecure is not None:
             pulumi.set(__self__, "allow_insecure", allow_insecure)
         if check_certificate_revocation is not None:
             pulumi.set(__self__, "check_certificate_revocation", check_certificate_revocation)
@@ -62800,107 +61722,85 @@
             pulumi.set(__self__, "monitor_name", monitor_name)
         if monitor_options is not None:
             pulumi.set(__self__, "monitor_options", monitor_options)
         if monitor_priority is not None:
             pulumi.set(__self__, "monitor_priority", monitor_priority)
         if no_screenshot is not None:
             pulumi.set(__self__, "no_screenshot", no_screenshot)
+        if restricted_roles is not None:
+            pulumi.set(__self__, "restricted_roles", restricted_roles)
         if retry is not None:
             pulumi.set(__self__, "retry", retry)
 
     @property
     @pulumi.getter(name="tickEvery")
     def tick_every(self) -> pulumi.Input[int]:
-        """
-        How often the test should run (in seconds).
-        """
         return pulumi.get(self, "tick_every")
 
     @tick_every.setter
     def tick_every(self, value: pulumi.Input[int]):
         pulumi.set(self, "tick_every", value)
 
     @property
     @pulumi.getter(name="acceptSelfSigned")
     def accept_self_signed(self) -> Optional[pulumi.Input[bool]]:
-        """
-        For SSL test, whether or not the test should allow self signed certificates.
-        """
         return pulumi.get(self, "accept_self_signed")
 
     @accept_self_signed.setter
     def accept_self_signed(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "accept_self_signed", value)
 
     @property
     @pulumi.getter(name="allowInsecure")
     def allow_insecure(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Allows loading insecure content for an HTTP test.
-        """
         return pulumi.get(self, "allow_insecure")
 
     @allow_insecure.setter
     def allow_insecure(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "allow_insecure", value)
 
     @property
     @pulumi.getter(name="checkCertificateRevocation")
     def check_certificate_revocation(self) -> Optional[pulumi.Input[bool]]:
-        """
-        For SSL test, whether or not the test should fail on revoked certificate in stapled OCSP.
-        """
         return pulumi.get(self, "check_certificate_revocation")
 
     @check_certificate_revocation.setter
     def check_certificate_revocation(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "check_certificate_revocation", value)
 
     @property
     @pulumi.getter(name="followRedirects")
     def follow_redirects(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Determines whether or not the API HTTP test should follow redirects.
-        """
         return pulumi.get(self, "follow_redirects")
 
     @follow_redirects.setter
     def follow_redirects(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "follow_redirects", value)
 
     @property
     @pulumi.getter(name="minFailureDuration")
     def min_failure_duration(self) -> Optional[pulumi.Input[int]]:
-        """
-        Minimum amount of time in failure required to trigger an alert. Default is `0`.
-        """
         return pulumi.get(self, "min_failure_duration")
 
     @min_failure_duration.setter
     def min_failure_duration(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "min_failure_duration", value)
 
     @property
     @pulumi.getter(name="minLocationFailed")
     def min_location_failed(self) -> Optional[pulumi.Input[int]]:
-        """
-        Minimum number of locations in failure required to trigger an alert. Default is `1`.
-        """
         return pulumi.get(self, "min_location_failed")
 
     @min_location_failed.setter
     def min_location_failed(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "min_location_failed", value)
 
     @property
     @pulumi.getter(name="monitorName")
     def monitor_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        The monitor name is used for the alert title as well as for all monitor dashboard widgets and SLOs.
-        """
         return pulumi.get(self, "monitor_name")
 
     @monitor_name.setter
     def monitor_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "monitor_name", value)
 
     @property
@@ -62920,24 +61820,30 @@
     @monitor_priority.setter
     def monitor_priority(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "monitor_priority", value)
 
     @property
     @pulumi.getter(name="noScreenshot")
     def no_screenshot(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Prevents saving screenshots of the steps.
-        """
         return pulumi.get(self, "no_screenshot")
 
     @no_screenshot.setter
     def no_screenshot(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "no_screenshot", value)
 
     @property
+    @pulumi.getter(name="restrictedRoles")
+    def restricted_roles(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        return pulumi.get(self, "restricted_roles")
+
+    @restricted_roles.setter
+    def restricted_roles(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "restricted_roles", value)
+
+    @property
     @pulumi.getter
     def retry(self) -> Optional[pulumi.Input['SyntheticsTestOptionsListRetryArgs']]:
         return pulumi.get(self, "retry")
 
     @retry.setter
     def retry(self, value: Optional[pulumi.Input['SyntheticsTestOptionsListRetryArgs']]):
         pulumi.set(self, "retry", value)
@@ -62998,26 +61904,14 @@
                  region: Optional[pulumi.Input[str]] = None,
                  secret_key: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  session_token: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  workstation: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] access_key: Access key for `SIGV4` authentication.
-        :param pulumi.Input[str] domain: Domain for `ntlm` authentication.
-        :param pulumi.Input[str] password: Password for authentication.
-        :param pulumi.Input[str] region: Region for `SIGV4` authentication.
-        :param pulumi.Input[str] secret_key: Secret key for `SIGV4` authentication.
-        :param pulumi.Input[str] service_name: Service name for `SIGV4` authentication.
-        :param pulumi.Input[str] session_token: Session token for `SIGV4` authentication.
-        :param pulumi.Input[str] type: Type of basic authentication to use when performing the test.
-        :param pulumi.Input[str] username: Username for authentication.
-        :param pulumi.Input[str] workstation: Workstation for `ntlm` authentication.
-        """
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if domain is not None:
             pulumi.set(__self__, "domain", domain)
         if password is not None:
             pulumi.set(__self__, "password", password)
         if region is not None:
@@ -63034,125 +61928,95 @@
             pulumi.set(__self__, "username", username)
         if workstation is not None:
             pulumi.set(__self__, "workstation", workstation)
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[pulumi.Input[str]]:
-        """
-        Access key for `SIGV4` authentication.
-        """
         return pulumi.get(self, "access_key")
 
     @access_key.setter
     def access_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "access_key", value)
 
     @property
     @pulumi.getter
     def domain(self) -> Optional[pulumi.Input[str]]:
-        """
-        Domain for `ntlm` authentication.
-        """
         return pulumi.get(self, "domain")
 
     @domain.setter
     def domain(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "domain", value)
 
     @property
     @pulumi.getter
     def password(self) -> Optional[pulumi.Input[str]]:
-        """
-        Password for authentication.
-        """
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "password", value)
 
     @property
     @pulumi.getter
     def region(self) -> Optional[pulumi.Input[str]]:
-        """
-        Region for `SIGV4` authentication.
-        """
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
     @property
     @pulumi.getter(name="secretKey")
     def secret_key(self) -> Optional[pulumi.Input[str]]:
-        """
-        Secret key for `SIGV4` authentication.
-        """
         return pulumi.get(self, "secret_key")
 
     @secret_key.setter
     def secret_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_key", value)
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        Service name for `SIGV4` authentication.
-        """
         return pulumi.get(self, "service_name")
 
     @service_name.setter
     def service_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_name", value)
 
     @property
     @pulumi.getter(name="sessionToken")
     def session_token(self) -> Optional[pulumi.Input[str]]:
-        """
-        Session token for `SIGV4` authentication.
-        """
         return pulumi.get(self, "session_token")
 
     @session_token.setter
     def session_token(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "session_token", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
-        """
-        Type of basic authentication to use when performing the test.
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def username(self) -> Optional[pulumi.Input[str]]:
-        """
-        Username for authentication.
-        """
         return pulumi.get(self, "username")
 
     @username.setter
     def username(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "username", value)
 
     @property
     @pulumi.getter
     def workstation(self) -> Optional[pulumi.Input[str]]:
-        """
-        Workstation for `ntlm` authentication.
-        """
         return pulumi.get(self, "workstation")
 
     @workstation.setter
     def workstation(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "workstation", value)
 
 
@@ -63251,29 +62115,14 @@
                  no_saving_response_body: Optional[pulumi.Input[bool]] = None,
                  number_of_packets: Optional[pulumi.Input[int]] = None,
                  port: Optional[pulumi.Input[int]] = None,
                  servername: Optional[pulumi.Input[str]] = None,
                  should_track_hops: Optional[pulumi.Input[bool]] = None,
                  timeout: Optional[pulumi.Input[int]] = None,
                  url: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] body: The request body.
-        :param pulumi.Input[str] dns_server: DNS server to use for DNS tests (`subtype = "dns"`).
-        :param pulumi.Input[int] dns_server_port: DNS server port to use for DNS tests.
-        :param pulumi.Input[str] host: Host name to perform the test with.
-        :param pulumi.Input[str] message: For UDP and websocket tests, message to send with the request.
-        :param pulumi.Input[str] method: The HTTP method. Valid values are `GET`, `POST`, `PATCH`, `PUT`, `DELETE`, `HEAD`, `OPTIONS`.
-        :param pulumi.Input[bool] no_saving_response_body: Determines whether or not to save the response body.
-        :param pulumi.Input[int] number_of_packets: Number of pings to use per test for ICMP tests (`subtype = "icmp"`) between 0 and 10.
-        :param pulumi.Input[int] port: Port to use when performing the test.
-        :param pulumi.Input[str] servername: For SSL tests, it specifies on which server you want to initiate the TLS handshake, allowing the server to present one of multiple possible certificates on the same IP address and TCP port number.
-        :param pulumi.Input[bool] should_track_hops: This will turn on a traceroute probe to discover all gateways along the path to the host destination. For ICMP tests (`subtype = "icmp"`).
-        :param pulumi.Input[int] timeout: Timeout in seconds for the test. Defaults to `60`.
-        :param pulumi.Input[str] url: The URL to send the request to.
-        """
         if body is not None:
             pulumi.set(__self__, "body", body)
         if dns_server is not None:
             pulumi.set(__self__, "dns_server", dns_server)
         if dns_server_port is not None:
             pulumi.set(__self__, "dns_server_port", dns_server_port)
         if host is not None:
@@ -63296,199 +62145,150 @@
             pulumi.set(__self__, "timeout", timeout)
         if url is not None:
             pulumi.set(__self__, "url", url)
 
     @property
     @pulumi.getter
     def body(self) -> Optional[pulumi.Input[str]]:
-        """
-        The request body.
-        """
         return pulumi.get(self, "body")
 
     @body.setter
     def body(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "body", value)
 
     @property
     @pulumi.getter(name="dnsServer")
     def dns_server(self) -> Optional[pulumi.Input[str]]:
-        """
-        DNS server to use for DNS tests (`subtype = "dns"`).
-        """
         return pulumi.get(self, "dns_server")
 
     @dns_server.setter
     def dns_server(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "dns_server", value)
 
     @property
     @pulumi.getter(name="dnsServerPort")
     def dns_server_port(self) -> Optional[pulumi.Input[int]]:
-        """
-        DNS server port to use for DNS tests.
-        """
         return pulumi.get(self, "dns_server_port")
 
     @dns_server_port.setter
     def dns_server_port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "dns_server_port", value)
 
     @property
     @pulumi.getter
     def host(self) -> Optional[pulumi.Input[str]]:
-        """
-        Host name to perform the test with.
-        """
         return pulumi.get(self, "host")
 
     @host.setter
     def host(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "host", value)
 
     @property
     @pulumi.getter
     def message(self) -> Optional[pulumi.Input[str]]:
-        """
-        For UDP and websocket tests, message to send with the request.
-        """
         return pulumi.get(self, "message")
 
     @message.setter
     def message(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "message", value)
 
     @property
     @pulumi.getter
     def method(self) -> Optional[pulumi.Input[str]]:
-        """
-        The HTTP method. Valid values are `GET`, `POST`, `PATCH`, `PUT`, `DELETE`, `HEAD`, `OPTIONS`.
-        """
         return pulumi.get(self, "method")
 
     @method.setter
     def method(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "method", value)
 
     @property
     @pulumi.getter(name="noSavingResponseBody")
     def no_saving_response_body(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Determines whether or not to save the response body.
-        """
         return pulumi.get(self, "no_saving_response_body")
 
     @no_saving_response_body.setter
     def no_saving_response_body(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "no_saving_response_body", value)
 
     @property
     @pulumi.getter(name="numberOfPackets")
     def number_of_packets(self) -> Optional[pulumi.Input[int]]:
-        """
-        Number of pings to use per test for ICMP tests (`subtype = "icmp"`) between 0 and 10.
-        """
         return pulumi.get(self, "number_of_packets")
 
     @number_of_packets.setter
     def number_of_packets(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "number_of_packets", value)
 
     @property
     @pulumi.getter
     def port(self) -> Optional[pulumi.Input[int]]:
-        """
-        Port to use when performing the test.
-        """
         return pulumi.get(self, "port")
 
     @port.setter
     def port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "port", value)
 
     @property
     @pulumi.getter
     def servername(self) -> Optional[pulumi.Input[str]]:
-        """
-        For SSL tests, it specifies on which server you want to initiate the TLS handshake, allowing the server to present one of multiple possible certificates on the same IP address and TCP port number.
-        """
         return pulumi.get(self, "servername")
 
     @servername.setter
     def servername(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "servername", value)
 
     @property
     @pulumi.getter(name="shouldTrackHops")
     def should_track_hops(self) -> Optional[pulumi.Input[bool]]:
-        """
-        This will turn on a traceroute probe to discover all gateways along the path to the host destination. For ICMP tests (`subtype = "icmp"`).
-        """
         return pulumi.get(self, "should_track_hops")
 
     @should_track_hops.setter
     def should_track_hops(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "should_track_hops", value)
 
     @property
     @pulumi.getter
     def timeout(self) -> Optional[pulumi.Input[int]]:
-        """
-        Timeout in seconds for the test. Defaults to `60`.
-        """
         return pulumi.get(self, "timeout")
 
     @timeout.setter
     def timeout(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "timeout", value)
 
     @property
     @pulumi.getter
     def url(self) -> Optional[pulumi.Input[str]]:
-        """
-        The URL to send the request to.
-        """
         return pulumi.get(self, "url")
 
     @url.setter
     def url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "url", value)
 
 
 @pulumi.input_type
 class SyntheticsTestRequestProxyArgs:
     def __init__(__self__, *,
                  url: pulumi.Input[str],
                  headers: Optional[pulumi.Input[Mapping[str, Any]]] = None):
-        """
-        :param pulumi.Input[str] url: URL of the proxy to perform the test.
-        :param pulumi.Input[Mapping[str, Any]] headers: Header name and value map.
-        """
         pulumi.set(__self__, "url", url)
         if headers is not None:
             pulumi.set(__self__, "headers", headers)
 
     @property
     @pulumi.getter
     def url(self) -> pulumi.Input[str]:
-        """
-        URL of the proxy to perform the test.
-        """
         return pulumi.get(self, "url")
 
     @url.setter
     def url(self, value: pulumi.Input[str]):
         pulumi.set(self, "url", value)
 
     @property
     @pulumi.getter
     def headers(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
-        """
-        Header name and value map.
-        """
         return pulumi.get(self, "headers")
 
     @headers.setter
     def headers(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "headers", value)
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/_utilities.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/api_key.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/api_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/application_key.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/application_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/authn_mapping.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/authn_mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/aws/integration.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/aws/integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,24 @@
                  resource_collection_enabled: Optional[pulumi.Input[str]] = None,
                  role_name: Optional[pulumi.Input[str]] = None,
                  secret_access_key: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Integration resource.
         :param pulumi.Input[str] access_key_id: Your AWS access key ID. Only required if your AWS account is a GovCloud or China account.
         :param pulumi.Input[str] account_id: Your AWS Account ID without dashes.
-        :param pulumi.Input[Mapping[str, Any]] account_specific_namespace_rules: Enables or disables metric collection for specific AWS namespaces for this AWS account only. A list of namespaces can be found at the [available namespace rules API endpoint](https://docs.datadoghq.com/api/v1/aws-integration/#list-namespace-rules).
-        :param pulumi.Input[str] cspm_resource_collection_enabled: Whether Datadog collects cloud security posture management resources from your AWS account. This includes additional resources not covered under the general resource_collection.
+        :param pulumi.Input[Mapping[str, Any]] account_specific_namespace_rules: Enables or disables metric collection for specific AWS namespaces for this AWS account only. A list of namespaces can be
+               found at the [available namespace rules API
+               endpoint](https://docs.datadoghq.com/api/v1/aws-integration/#list-namespace-rules).
+        :param pulumi.Input[str] cspm_resource_collection_enabled: Whether Datadog collects cloud security posture management resources from your AWS account. This includes additional
+               resources not covered under the general resource_collection.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] excluded_regions: An array of AWS regions to exclude from metrics collection.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] filter_tags: Array of EC2 tags (in the form `key:value`) defines a filter that Datadog uses when collecting metrics from EC2. Wildcards, such as `?` (for single characters) and `*` (for multiple characters) can also be used. Only hosts that match one of the defined tags will be imported into Datadog. The rest will be ignored. Host matching a given tag can also be excluded by adding `!` before the tag. e.x. `env:production,instance-type:c1.*,!region:us-east-1`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] filter_tags: Array of EC2 tags (in the form `key:value`) defines a filter that Datadog uses when collecting metrics from EC2.
+               Wildcards, such as `?` (for single characters) and `*` (for multiple characters) can also be used. Only hosts that match
+               one of the defined tags will be imported into Datadog. The rest will be ignored. Host matching a given tag can also be
+               excluded by adding `!` before the tag. e.x. `env:production,instance-type:c1.*,!region:us-east-1`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] host_tags: Array of tags (in the form `key:value`) to add to all hosts and metrics reporting through this integration.
         :param pulumi.Input[str] metrics_collection_enabled: Whether Datadog collects metrics for this AWS account.
         :param pulumi.Input[str] resource_collection_enabled: Whether Datadog collects a standard set of resources from your AWS account.
         :param pulumi.Input[str] role_name: Your Datadog role delegation name.
         :param pulumi.Input[str] secret_access_key: Your AWS secret access key. Only required if your AWS account is a GovCloud or China account.
         """
         if access_key_id is not None:
@@ -85,27 +91,30 @@
     def account_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "account_id", value)
 
     @property
     @pulumi.getter(name="accountSpecificNamespaceRules")
     def account_specific_namespace_rules(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
-        Enables or disables metric collection for specific AWS namespaces for this AWS account only. A list of namespaces can be found at the [available namespace rules API endpoint](https://docs.datadoghq.com/api/v1/aws-integration/#list-namespace-rules).
+        Enables or disables metric collection for specific AWS namespaces for this AWS account only. A list of namespaces can be
+        found at the [available namespace rules API
+        endpoint](https://docs.datadoghq.com/api/v1/aws-integration/#list-namespace-rules).
         """
         return pulumi.get(self, "account_specific_namespace_rules")
 
     @account_specific_namespace_rules.setter
     def account_specific_namespace_rules(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "account_specific_namespace_rules", value)
 
     @property
     @pulumi.getter(name="cspmResourceCollectionEnabled")
     def cspm_resource_collection_enabled(self) -> Optional[pulumi.Input[str]]:
         """
-        Whether Datadog collects cloud security posture management resources from your AWS account. This includes additional resources not covered under the general resource_collection.
+        Whether Datadog collects cloud security posture management resources from your AWS account. This includes additional
+        resources not covered under the general resource_collection.
         """
         return pulumi.get(self, "cspm_resource_collection_enabled")
 
     @cspm_resource_collection_enabled.setter
     def cspm_resource_collection_enabled(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cspm_resource_collection_enabled", value)
 
@@ -121,15 +130,18 @@
     def excluded_regions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "excluded_regions", value)
 
     @property
     @pulumi.getter(name="filterTags")
     def filter_tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Array of EC2 tags (in the form `key:value`) defines a filter that Datadog uses when collecting metrics from EC2. Wildcards, such as `?` (for single characters) and `*` (for multiple characters) can also be used. Only hosts that match one of the defined tags will be imported into Datadog. The rest will be ignored. Host matching a given tag can also be excluded by adding `!` before the tag. e.x. `env:production,instance-type:c1.*,!region:us-east-1`.
+        Array of EC2 tags (in the form `key:value`) defines a filter that Datadog uses when collecting metrics from EC2.
+        Wildcards, such as `?` (for single characters) and `*` (for multiple characters) can also be used. Only hosts that match
+        one of the defined tags will be imported into Datadog. The rest will be ignored. Host matching a given tag can also be
+        excluded by adding `!` before the tag. e.x. `env:production,instance-type:c1.*,!region:us-east-1`.
         """
         return pulumi.get(self, "filter_tags")
 
     @filter_tags.setter
     def filter_tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "filter_tags", value)
 
@@ -209,20 +221,26 @@
                  resource_collection_enabled: Optional[pulumi.Input[str]] = None,
                  role_name: Optional[pulumi.Input[str]] = None,
                  secret_access_key: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Integration resources.
         :param pulumi.Input[str] access_key_id: Your AWS access key ID. Only required if your AWS account is a GovCloud or China account.
         :param pulumi.Input[str] account_id: Your AWS Account ID without dashes.
-        :param pulumi.Input[Mapping[str, Any]] account_specific_namespace_rules: Enables or disables metric collection for specific AWS namespaces for this AWS account only. A list of namespaces can be found at the [available namespace rules API endpoint](https://docs.datadoghq.com/api/v1/aws-integration/#list-namespace-rules).
-        :param pulumi.Input[str] cspm_resource_collection_enabled: Whether Datadog collects cloud security posture management resources from your AWS account. This includes additional resources not covered under the general resource_collection.
+        :param pulumi.Input[Mapping[str, Any]] account_specific_namespace_rules: Enables or disables metric collection for specific AWS namespaces for this AWS account only. A list of namespaces can be
+               found at the [available namespace rules API
+               endpoint](https://docs.datadoghq.com/api/v1/aws-integration/#list-namespace-rules).
+        :param pulumi.Input[str] cspm_resource_collection_enabled: Whether Datadog collects cloud security posture management resources from your AWS account. This includes additional
+               resources not covered under the general resource_collection.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] excluded_regions: An array of AWS regions to exclude from metrics collection.
         :param pulumi.Input[str] external_id: AWS External ID. **NOTE** This provider will not be able to detect changes made to the `external_id` field from outside
                Terraform.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] filter_tags: Array of EC2 tags (in the form `key:value`) defines a filter that Datadog uses when collecting metrics from EC2. Wildcards, such as `?` (for single characters) and `*` (for multiple characters) can also be used. Only hosts that match one of the defined tags will be imported into Datadog. The rest will be ignored. Host matching a given tag can also be excluded by adding `!` before the tag. e.x. `env:production,instance-type:c1.*,!region:us-east-1`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] filter_tags: Array of EC2 tags (in the form `key:value`) defines a filter that Datadog uses when collecting metrics from EC2.
+               Wildcards, such as `?` (for single characters) and `*` (for multiple characters) can also be used. Only hosts that match
+               one of the defined tags will be imported into Datadog. The rest will be ignored. Host matching a given tag can also be
+               excluded by adding `!` before the tag. e.x. `env:production,instance-type:c1.*,!region:us-east-1`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] host_tags: Array of tags (in the form `key:value`) to add to all hosts and metrics reporting through this integration.
         :param pulumi.Input[str] metrics_collection_enabled: Whether Datadog collects metrics for this AWS account.
         :param pulumi.Input[str] resource_collection_enabled: Whether Datadog collects a standard set of resources from your AWS account.
         :param pulumi.Input[str] role_name: Your Datadog role delegation name.
         :param pulumi.Input[str] secret_access_key: Your AWS secret access key. Only required if your AWS account is a GovCloud or China account.
         """
         if access_key_id is not None:
@@ -274,27 +292,30 @@
     def account_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "account_id", value)
 
     @property
     @pulumi.getter(name="accountSpecificNamespaceRules")
     def account_specific_namespace_rules(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
-        Enables or disables metric collection for specific AWS namespaces for this AWS account only. A list of namespaces can be found at the [available namespace rules API endpoint](https://docs.datadoghq.com/api/v1/aws-integration/#list-namespace-rules).
+        Enables or disables metric collection for specific AWS namespaces for this AWS account only. A list of namespaces can be
+        found at the [available namespace rules API
+        endpoint](https://docs.datadoghq.com/api/v1/aws-integration/#list-namespace-rules).
         """
         return pulumi.get(self, "account_specific_namespace_rules")
 
     @account_specific_namespace_rules.setter
     def account_specific_namespace_rules(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "account_specific_namespace_rules", value)
 
     @property
     @pulumi.getter(name="cspmResourceCollectionEnabled")
     def cspm_resource_collection_enabled(self) -> Optional[pulumi.Input[str]]:
         """
-        Whether Datadog collects cloud security posture management resources from your AWS account. This includes additional resources not covered under the general resource_collection.
+        Whether Datadog collects cloud security posture management resources from your AWS account. This includes additional
+        resources not covered under the general resource_collection.
         """
         return pulumi.get(self, "cspm_resource_collection_enabled")
 
     @cspm_resource_collection_enabled.setter
     def cspm_resource_collection_enabled(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cspm_resource_collection_enabled", value)
 
@@ -323,15 +344,18 @@
     def external_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "external_id", value)
 
     @property
     @pulumi.getter(name="filterTags")
     def filter_tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Array of EC2 tags (in the form `key:value`) defines a filter that Datadog uses when collecting metrics from EC2. Wildcards, such as `?` (for single characters) and `*` (for multiple characters) can also be used. Only hosts that match one of the defined tags will be imported into Datadog. The rest will be ignored. Host matching a given tag can also be excluded by adding `!` before the tag. e.x. `env:production,instance-type:c1.*,!region:us-east-1`.
+        Array of EC2 tags (in the form `key:value`) defines a filter that Datadog uses when collecting metrics from EC2.
+        Wildcards, such as `?` (for single characters) and `*` (for multiple characters) can also be used. Only hosts that match
+        one of the defined tags will be imported into Datadog. The rest will be ignored. Host matching a given tag can also be
+        excluded by adding `!` before the tag. e.x. `env:production,instance-type:c1.*,!region:us-east-1`.
         """
         return pulumi.get(self, "filter_tags")
 
     @filter_tags.setter
     def filter_tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "filter_tags", value)
 
@@ -449,18 +473,24 @@
          $ pulumi import datadog:aws/integration:Integration EXTERNAL_ID=${external_id} datadog_integration_aws.test ${account_id}:${role_name}
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access_key_id: Your AWS access key ID. Only required if your AWS account is a GovCloud or China account.
         :param pulumi.Input[str] account_id: Your AWS Account ID without dashes.
-        :param pulumi.Input[Mapping[str, Any]] account_specific_namespace_rules: Enables or disables metric collection for specific AWS namespaces for this AWS account only. A list of namespaces can be found at the [available namespace rules API endpoint](https://docs.datadoghq.com/api/v1/aws-integration/#list-namespace-rules).
-        :param pulumi.Input[str] cspm_resource_collection_enabled: Whether Datadog collects cloud security posture management resources from your AWS account. This includes additional resources not covered under the general resource_collection.
+        :param pulumi.Input[Mapping[str, Any]] account_specific_namespace_rules: Enables or disables metric collection for specific AWS namespaces for this AWS account only. A list of namespaces can be
+               found at the [available namespace rules API
+               endpoint](https://docs.datadoghq.com/api/v1/aws-integration/#list-namespace-rules).
+        :param pulumi.Input[str] cspm_resource_collection_enabled: Whether Datadog collects cloud security posture management resources from your AWS account. This includes additional
+               resources not covered under the general resource_collection.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] excluded_regions: An array of AWS regions to exclude from metrics collection.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] filter_tags: Array of EC2 tags (in the form `key:value`) defines a filter that Datadog uses when collecting metrics from EC2. Wildcards, such as `?` (for single characters) and `*` (for multiple characters) can also be used. Only hosts that match one of the defined tags will be imported into Datadog. The rest will be ignored. Host matching a given tag can also be excluded by adding `!` before the tag. e.x. `env:production,instance-type:c1.*,!region:us-east-1`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] filter_tags: Array of EC2 tags (in the form `key:value`) defines a filter that Datadog uses when collecting metrics from EC2.
+               Wildcards, such as `?` (for single characters) and `*` (for multiple characters) can also be used. Only hosts that match
+               one of the defined tags will be imported into Datadog. The rest will be ignored. Host matching a given tag can also be
+               excluded by adding `!` before the tag. e.x. `env:production,instance-type:c1.*,!region:us-east-1`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] host_tags: Array of tags (in the form `key:value`) to add to all hosts and metrics reporting through this integration.
         :param pulumi.Input[str] metrics_collection_enabled: Whether Datadog collects metrics for this AWS account.
         :param pulumi.Input[str] resource_collection_enabled: Whether Datadog collects a standard set of resources from your AWS account.
         :param pulumi.Input[str] role_name: Your Datadog role delegation name.
         :param pulumi.Input[str] secret_access_key: Your AWS secret access key. Only required if your AWS account is a GovCloud or China account.
         """
         ...
@@ -582,20 +612,26 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access_key_id: Your AWS access key ID. Only required if your AWS account is a GovCloud or China account.
         :param pulumi.Input[str] account_id: Your AWS Account ID without dashes.
-        :param pulumi.Input[Mapping[str, Any]] account_specific_namespace_rules: Enables or disables metric collection for specific AWS namespaces for this AWS account only. A list of namespaces can be found at the [available namespace rules API endpoint](https://docs.datadoghq.com/api/v1/aws-integration/#list-namespace-rules).
-        :param pulumi.Input[str] cspm_resource_collection_enabled: Whether Datadog collects cloud security posture management resources from your AWS account. This includes additional resources not covered under the general resource_collection.
+        :param pulumi.Input[Mapping[str, Any]] account_specific_namespace_rules: Enables or disables metric collection for specific AWS namespaces for this AWS account only. A list of namespaces can be
+               found at the [available namespace rules API
+               endpoint](https://docs.datadoghq.com/api/v1/aws-integration/#list-namespace-rules).
+        :param pulumi.Input[str] cspm_resource_collection_enabled: Whether Datadog collects cloud security posture management resources from your AWS account. This includes additional
+               resources not covered under the general resource_collection.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] excluded_regions: An array of AWS regions to exclude from metrics collection.
         :param pulumi.Input[str] external_id: AWS External ID. **NOTE** This provider will not be able to detect changes made to the `external_id` field from outside
                Terraform.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] filter_tags: Array of EC2 tags (in the form `key:value`) defines a filter that Datadog uses when collecting metrics from EC2. Wildcards, such as `?` (for single characters) and `*` (for multiple characters) can also be used. Only hosts that match one of the defined tags will be imported into Datadog. The rest will be ignored. Host matching a given tag can also be excluded by adding `!` before the tag. e.x. `env:production,instance-type:c1.*,!region:us-east-1`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] filter_tags: Array of EC2 tags (in the form `key:value`) defines a filter that Datadog uses when collecting metrics from EC2.
+               Wildcards, such as `?` (for single characters) and `*` (for multiple characters) can also be used. Only hosts that match
+               one of the defined tags will be imported into Datadog. The rest will be ignored. Host matching a given tag can also be
+               excluded by adding `!` before the tag. e.x. `env:production,instance-type:c1.*,!region:us-east-1`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] host_tags: Array of tags (in the form `key:value`) to add to all hosts and metrics reporting through this integration.
         :param pulumi.Input[str] metrics_collection_enabled: Whether Datadog collects metrics for this AWS account.
         :param pulumi.Input[str] resource_collection_enabled: Whether Datadog collects a standard set of resources from your AWS account.
         :param pulumi.Input[str] role_name: Your Datadog role delegation name.
         :param pulumi.Input[str] secret_access_key: Your AWS secret access key. Only required if your AWS account is a GovCloud or China account.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
@@ -632,23 +668,26 @@
         """
         return pulumi.get(self, "account_id")
 
     @property
     @pulumi.getter(name="accountSpecificNamespaceRules")
     def account_specific_namespace_rules(self) -> pulumi.Output[Optional[Mapping[str, Any]]]:
         """
-        Enables or disables metric collection for specific AWS namespaces for this AWS account only. A list of namespaces can be found at the [available namespace rules API endpoint](https://docs.datadoghq.com/api/v1/aws-integration/#list-namespace-rules).
+        Enables or disables metric collection for specific AWS namespaces for this AWS account only. A list of namespaces can be
+        found at the [available namespace rules API
+        endpoint](https://docs.datadoghq.com/api/v1/aws-integration/#list-namespace-rules).
         """
         return pulumi.get(self, "account_specific_namespace_rules")
 
     @property
     @pulumi.getter(name="cspmResourceCollectionEnabled")
     def cspm_resource_collection_enabled(self) -> pulumi.Output[str]:
         """
-        Whether Datadog collects cloud security posture management resources from your AWS account. This includes additional resources not covered under the general resource_collection.
+        Whether Datadog collects cloud security posture management resources from your AWS account. This includes additional
+        resources not covered under the general resource_collection.
         """
         return pulumi.get(self, "cspm_resource_collection_enabled")
 
     @property
     @pulumi.getter(name="excludedRegions")
     def excluded_regions(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
@@ -665,15 +704,18 @@
         """
         return pulumi.get(self, "external_id")
 
     @property
     @pulumi.getter(name="filterTags")
     def filter_tags(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        Array of EC2 tags (in the form `key:value`) defines a filter that Datadog uses when collecting metrics from EC2. Wildcards, such as `?` (for single characters) and `*` (for multiple characters) can also be used. Only hosts that match one of the defined tags will be imported into Datadog. The rest will be ignored. Host matching a given tag can also be excluded by adding `!` before the tag. e.x. `env:production,instance-type:c1.*,!region:us-east-1`.
+        Array of EC2 tags (in the form `key:value`) defines a filter that Datadog uses when collecting metrics from EC2.
+        Wildcards, such as `?` (for single characters) and `*` (for multiple characters) can also be used. Only hosts that match
+        one of the defined tags will be imported into Datadog. The rest will be ignored. Host matching a given tag can also be
+        excluded by adding `!` before the tag. e.x. `env:production,instance-type:c1.*,!region:us-east-1`.
         """
         return pulumi.get(self, "filter_tags")
 
     @property
     @pulumi.getter(name="hostTags")
     def host_tags(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/aws/integration_lambda_arn.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/aws/integration_lambda_arn.py`

 * *Files identical despite different names*

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/aws/integration_log_collection.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/aws/integration_log_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 class IntegrationLogCollectionArgs:
     def __init__(__self__, *,
                  account_id: pulumi.Input[str],
                  services: pulumi.Input[Sequence[pulumi.Input[str]]]):
         """
         The set of arguments for constructing a IntegrationLogCollection resource.
         :param pulumi.Input[str] account_id: Your AWS Account ID without dashes. If your account is a GovCloud or China account, specify the `access_key_id` here.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: A list of services to collect logs from. See the [api docs](https://docs.datadoghq.com/api/v1/aws-logs-integration/#get-list-of-aws-log-ready-services) for more details on which services are supported.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: A list of services to collect logs from. See the [api
+               docs](https://docs.datadoghq.com/api/v1/aws-logs-integration/#get-list-of-aws-log-ready-services) for more details on
+               which services are supported.
         """
         pulumi.set(__self__, "account_id", account_id)
         pulumi.set(__self__, "services", services)
 
     @property
     @pulumi.getter(name="accountId")
     def account_id(self) -> pulumi.Input[str]:
@@ -35,15 +37,17 @@
     def account_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "account_id", value)
 
     @property
     @pulumi.getter
     def services(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        A list of services to collect logs from. See the [api docs](https://docs.datadoghq.com/api/v1/aws-logs-integration/#get-list-of-aws-log-ready-services) for more details on which services are supported.
+        A list of services to collect logs from. See the [api
+        docs](https://docs.datadoghq.com/api/v1/aws-logs-integration/#get-list-of-aws-log-ready-services) for more details on
+        which services are supported.
         """
         return pulumi.get(self, "services")
 
     @services.setter
     def services(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "services", value)
 
@@ -52,15 +56,17 @@
 class _IntegrationLogCollectionState:
     def __init__(__self__, *,
                  account_id: Optional[pulumi.Input[str]] = None,
                  services: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering IntegrationLogCollection resources.
         :param pulumi.Input[str] account_id: Your AWS Account ID without dashes. If your account is a GovCloud or China account, specify the `access_key_id` here.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: A list of services to collect logs from. See the [api docs](https://docs.datadoghq.com/api/v1/aws-logs-integration/#get-list-of-aws-log-ready-services) for more details on which services are supported.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: A list of services to collect logs from. See the [api
+               docs](https://docs.datadoghq.com/api/v1/aws-logs-integration/#get-list-of-aws-log-ready-services) for more details on
+               which services are supported.
         """
         if account_id is not None:
             pulumi.set(__self__, "account_id", account_id)
         if services is not None:
             pulumi.set(__self__, "services", services)
 
     @property
@@ -75,15 +81,17 @@
     def account_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "account_id", value)
 
     @property
     @pulumi.getter
     def services(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of services to collect logs from. See the [api docs](https://docs.datadoghq.com/api/v1/aws-logs-integration/#get-list-of-aws-log-ready-services) for more details on which services are supported.
+        A list of services to collect logs from. See the [api
+        docs](https://docs.datadoghq.com/api/v1/aws-logs-integration/#get-list-of-aws-log-ready-services) for more details on
+        which services are supported.
         """
         return pulumi.get(self, "services")
 
     @services.setter
     def services(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "services", value)
 
@@ -118,15 +126,17 @@
         ```sh
          $ pulumi import datadog:aws/integrationLogCollection:IntegrationLogCollection test 1234567890
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] account_id: Your AWS Account ID without dashes. If your account is a GovCloud or China account, specify the `access_key_id` here.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: A list of services to collect logs from. See the [api docs](https://docs.datadoghq.com/api/v1/aws-logs-integration/#get-list-of-aws-log-ready-services) for more details on which services are supported.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: A list of services to collect logs from. See the [api
+               docs](https://docs.datadoghq.com/api/v1/aws-logs-integration/#get-list-of-aws-log-ready-services) for more details on
+               which services are supported.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: IntegrationLogCollectionArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -204,15 +214,17 @@
         Get an existing IntegrationLogCollection resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] account_id: Your AWS Account ID without dashes. If your account is a GovCloud or China account, specify the `access_key_id` here.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: A list of services to collect logs from. See the [api docs](https://docs.datadoghq.com/api/v1/aws-logs-integration/#get-list-of-aws-log-ready-services) for more details on which services are supported.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: A list of services to collect logs from. See the [api
+               docs](https://docs.datadoghq.com/api/v1/aws-logs-integration/#get-list-of-aws-log-ready-services) for more details on
+               which services are supported.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _IntegrationLogCollectionState.__new__(_IntegrationLogCollectionState)
 
         __props__.__dict__["account_id"] = account_id
         __props__.__dict__["services"] = services
@@ -226,11 +238,13 @@
         """
         return pulumi.get(self, "account_id")
 
     @property
     @pulumi.getter
     def services(self) -> pulumi.Output[Sequence[str]]:
         """
-        A list of services to collect logs from. See the [api docs](https://docs.datadoghq.com/api/v1/aws-logs-integration/#get-list-of-aws-log-ready-services) for more details on which services are supported.
+        A list of services to collect logs from. See the [api
+        docs](https://docs.datadoghq.com/api/v1/aws-logs-integration/#get-list-of-aws-log-ready-services) for more details on
+        which services are supported.
         """
         return pulumi.get(self, "services")
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/aws/integration_tag_filter.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/aws/integration_tag_filter.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def __init__(__self__, *,
                  account_id: pulumi.Input[str],
                  namespace: pulumi.Input[str],
                  tag_filter_str: pulumi.Input[str]):
         """
         The set of arguments for constructing a IntegrationTagFilter resource.
         :param pulumi.Input[str] account_id: Your AWS Account ID without dashes. If your account is a GovCloud or China account, specify the `access_key_id` here.
-        :param pulumi.Input[str] namespace: The namespace associated with the tag filter entry. Valid values are `elb`, `application_elb`, `sqs`, `rds`, `custom`, `network_elb`, `lambda`.
+        :param pulumi.Input[str] namespace: The namespace associated with the tag filter entry.
         :param pulumi.Input[str] tag_filter_str: The tag filter string.
         """
         pulumi.set(__self__, "account_id", account_id)
         pulumi.set(__self__, "namespace", namespace)
         pulumi.set(__self__, "tag_filter_str", tag_filter_str)
 
     @property
@@ -38,15 +38,15 @@
     def account_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "account_id", value)
 
     @property
     @pulumi.getter
     def namespace(self) -> pulumi.Input[str]:
         """
-        The namespace associated with the tag filter entry. Valid values are `elb`, `application_elb`, `sqs`, `rds`, `custom`, `network_elb`, `lambda`.
+        The namespace associated with the tag filter entry.
         """
         return pulumi.get(self, "namespace")
 
     @namespace.setter
     def namespace(self, value: pulumi.Input[str]):
         pulumi.set(self, "namespace", value)
 
@@ -68,15 +68,15 @@
     def __init__(__self__, *,
                  account_id: Optional[pulumi.Input[str]] = None,
                  namespace: Optional[pulumi.Input[str]] = None,
                  tag_filter_str: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering IntegrationTagFilter resources.
         :param pulumi.Input[str] account_id: Your AWS Account ID without dashes. If your account is a GovCloud or China account, specify the `access_key_id` here.
-        :param pulumi.Input[str] namespace: The namespace associated with the tag filter entry. Valid values are `elb`, `application_elb`, `sqs`, `rds`, `custom`, `network_elb`, `lambda`.
+        :param pulumi.Input[str] namespace: The namespace associated with the tag filter entry.
         :param pulumi.Input[str] tag_filter_str: The tag filter string.
         """
         if account_id is not None:
             pulumi.set(__self__, "account_id", account_id)
         if namespace is not None:
             pulumi.set(__self__, "namespace", namespace)
         if tag_filter_str is not None:
@@ -94,15 +94,15 @@
     def account_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "account_id", value)
 
     @property
     @pulumi.getter
     def namespace(self) -> Optional[pulumi.Input[str]]:
         """
-        The namespace associated with the tag filter entry. Valid values are `elb`, `application_elb`, `sqs`, `rds`, `custom`, `network_elb`, `lambda`.
+        The namespace associated with the tag filter entry.
         """
         return pulumi.get(self, "namespace")
 
     @namespace.setter
     def namespace(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "namespace", value)
 
@@ -151,15 +151,15 @@
         ```sh
          $ pulumi import datadog:aws/integrationTagFilter:IntegrationTagFilter foo ${account_id}:${namespace}
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] account_id: Your AWS Account ID without dashes. If your account is a GovCloud or China account, specify the `access_key_id` here.
-        :param pulumi.Input[str] namespace: The namespace associated with the tag filter entry. Valid values are `elb`, `application_elb`, `sqs`, `rds`, `custom`, `network_elb`, `lambda`.
+        :param pulumi.Input[str] namespace: The namespace associated with the tag filter entry.
         :param pulumi.Input[str] tag_filter_str: The tag filter string.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: IntegrationTagFilterArgs,
@@ -244,15 +244,15 @@
         Get an existing IntegrationTagFilter resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] account_id: Your AWS Account ID without dashes. If your account is a GovCloud or China account, specify the `access_key_id` here.
-        :param pulumi.Input[str] namespace: The namespace associated with the tag filter entry. Valid values are `elb`, `application_elb`, `sqs`, `rds`, `custom`, `network_elb`, `lambda`.
+        :param pulumi.Input[str] namespace: The namespace associated with the tag filter entry.
         :param pulumi.Input[str] tag_filter_str: The tag filter string.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _IntegrationTagFilterState.__new__(_IntegrationTagFilterState)
 
         __props__.__dict__["account_id"] = account_id
@@ -268,15 +268,15 @@
         """
         return pulumi.get(self, "account_id")
 
     @property
     @pulumi.getter
     def namespace(self) -> pulumi.Output[str]:
         """
-        The namespace associated with the tag filter entry. Valid values are `elb`, `application_elb`, `sqs`, `rds`, `custom`, `network_elb`, `lambda`.
+        The namespace associated with the tag filter entry.
         """
         return pulumi.get(self, "namespace")
 
     @property
     @pulumi.getter(name="tagFilterStr")
     def tag_filter_str(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/azure/integration.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/azure/integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,17 @@
                  host_filters: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Integration resource.
         :param pulumi.Input[str] client_id: Your Azure web application ID.
         :param pulumi.Input[str] client_secret: (Required for Initial Creation) Your Azure web application secret key.
         :param pulumi.Input[str] tenant_name: Your Azure Active Directory ID.
         :param pulumi.Input[bool] automute: Silence monitors for expected Azure VM shutdowns.
-        :param pulumi.Input[str] host_filters: String of host tag(s) (in the form `key:value,key:value`) defines a filter that Datadog will use when collecting metrics from Azure. Limit the Azure instances that are pulled into Datadog by using tags. Only hosts that match one of the defined tags are imported into Datadog. e.x. `env:production,deploymentgroup:red`
+        :param pulumi.Input[str] host_filters: String of host tag(s) (in the form `key:value,key:value`) defines a filter that Datadog will use when collecting metrics
+               from Azure. Limit the Azure instances that are pulled into Datadog by using tags. Only hosts that match one of the
+               defined tags are imported into Datadog. e.x. `env:production,deploymentgroup:red`
         """
         pulumi.set(__self__, "client_id", client_id)
         pulumi.set(__self__, "client_secret", client_secret)
         pulumi.set(__self__, "tenant_name", tenant_name)
         if automute is not None:
             pulumi.set(__self__, "automute", automute)
         if host_filters is not None:
@@ -82,15 +84,17 @@
     def automute(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "automute", value)
 
     @property
     @pulumi.getter(name="hostFilters")
     def host_filters(self) -> Optional[pulumi.Input[str]]:
         """
-        String of host tag(s) (in the form `key:value,key:value`) defines a filter that Datadog will use when collecting metrics from Azure. Limit the Azure instances that are pulled into Datadog by using tags. Only hosts that match one of the defined tags are imported into Datadog. e.x. `env:production,deploymentgroup:red`
+        String of host tag(s) (in the form `key:value,key:value`) defines a filter that Datadog will use when collecting metrics
+        from Azure. Limit the Azure instances that are pulled into Datadog by using tags. Only hosts that match one of the
+        defined tags are imported into Datadog. e.x. `env:production,deploymentgroup:red`
         """
         return pulumi.get(self, "host_filters")
 
     @host_filters.setter
     def host_filters(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "host_filters", value)
 
@@ -104,15 +108,17 @@
                  host_filters: Optional[pulumi.Input[str]] = None,
                  tenant_name: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Integration resources.
         :param pulumi.Input[bool] automute: Silence monitors for expected Azure VM shutdowns.
         :param pulumi.Input[str] client_id: Your Azure web application ID.
         :param pulumi.Input[str] client_secret: (Required for Initial Creation) Your Azure web application secret key.
-        :param pulumi.Input[str] host_filters: String of host tag(s) (in the form `key:value,key:value`) defines a filter that Datadog will use when collecting metrics from Azure. Limit the Azure instances that are pulled into Datadog by using tags. Only hosts that match one of the defined tags are imported into Datadog. e.x. `env:production,deploymentgroup:red`
+        :param pulumi.Input[str] host_filters: String of host tag(s) (in the form `key:value,key:value`) defines a filter that Datadog will use when collecting metrics
+               from Azure. Limit the Azure instances that are pulled into Datadog by using tags. Only hosts that match one of the
+               defined tags are imported into Datadog. e.x. `env:production,deploymentgroup:red`
         :param pulumi.Input[str] tenant_name: Your Azure Active Directory ID.
         """
         if automute is not None:
             pulumi.set(__self__, "automute", automute)
         if client_id is not None:
             pulumi.set(__self__, "client_id", client_id)
         if client_secret is not None:
@@ -158,15 +164,17 @@
     def client_secret(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "client_secret", value)
 
     @property
     @pulumi.getter(name="hostFilters")
     def host_filters(self) -> Optional[pulumi.Input[str]]:
         """
-        String of host tag(s) (in the form `key:value,key:value`) defines a filter that Datadog will use when collecting metrics from Azure. Limit the Azure instances that are pulled into Datadog by using tags. Only hosts that match one of the defined tags are imported into Datadog. e.x. `env:production,deploymentgroup:red`
+        String of host tag(s) (in the form `key:value,key:value`) defines a filter that Datadog will use when collecting metrics
+        from Azure. Limit the Azure instances that are pulled into Datadog by using tags. Only hosts that match one of the
+        defined tags are imported into Datadog. e.x. `env:production,deploymentgroup:red`
         """
         return pulumi.get(self, "host_filters")
 
     @host_filters.setter
     def host_filters(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "host_filters", value)
 
@@ -220,15 +228,17 @@
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] automute: Silence monitors for expected Azure VM shutdowns.
         :param pulumi.Input[str] client_id: Your Azure web application ID.
         :param pulumi.Input[str] client_secret: (Required for Initial Creation) Your Azure web application secret key.
-        :param pulumi.Input[str] host_filters: String of host tag(s) (in the form `key:value,key:value`) defines a filter that Datadog will use when collecting metrics from Azure. Limit the Azure instances that are pulled into Datadog by using tags. Only hosts that match one of the defined tags are imported into Datadog. e.x. `env:production,deploymentgroup:red`
+        :param pulumi.Input[str] host_filters: String of host tag(s) (in the form `key:value,key:value`) defines a filter that Datadog will use when collecting metrics
+               from Azure. Limit the Azure instances that are pulled into Datadog by using tags. Only hosts that match one of the
+               defined tags are imported into Datadog. e.x. `env:production,deploymentgroup:red`
         :param pulumi.Input[str] tenant_name: Your Azure Active Directory ID.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: IntegrationArgs,
@@ -322,15 +332,17 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] automute: Silence monitors for expected Azure VM shutdowns.
         :param pulumi.Input[str] client_id: Your Azure web application ID.
         :param pulumi.Input[str] client_secret: (Required for Initial Creation) Your Azure web application secret key.
-        :param pulumi.Input[str] host_filters: String of host tag(s) (in the form `key:value,key:value`) defines a filter that Datadog will use when collecting metrics from Azure. Limit the Azure instances that are pulled into Datadog by using tags. Only hosts that match one of the defined tags are imported into Datadog. e.x. `env:production,deploymentgroup:red`
+        :param pulumi.Input[str] host_filters: String of host tag(s) (in the form `key:value,key:value`) defines a filter that Datadog will use when collecting metrics
+               from Azure. Limit the Azure instances that are pulled into Datadog by using tags. Only hosts that match one of the
+               defined tags are imported into Datadog. e.x. `env:production,deploymentgroup:red`
         :param pulumi.Input[str] tenant_name: Your Azure Active Directory ID.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _IntegrationState.__new__(_IntegrationState)
 
         __props__.__dict__["automute"] = automute
@@ -364,15 +376,17 @@
         """
         return pulumi.get(self, "client_secret")
 
     @property
     @pulumi.getter(name="hostFilters")
     def host_filters(self) -> pulumi.Output[Optional[str]]:
         """
-        String of host tag(s) (in the form `key:value,key:value`) defines a filter that Datadog will use when collecting metrics from Azure. Limit the Azure instances that are pulled into Datadog by using tags. Only hosts that match one of the defined tags are imported into Datadog. e.x. `env:production,deploymentgroup:red`
+        String of host tag(s) (in the form `key:value,key:value`) defines a filter that Datadog will use when collecting metrics
+        from Azure. Limit the Azure instances that are pulled into Datadog by using tags. Only hosts that match one of the
+        defined tags are imported into Datadog. e.x. `env:production,deploymentgroup:red`
         """
         return pulumi.get(self, "host_filters")
 
     @property
     @pulumi.getter(name="tenantName")
     def tenant_name(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/child_organization.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/child_organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/cloud_workload_security_agent_rule.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/cloud_workload_security_agent_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/config/vars.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/config/vars.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         (Required unless validate is false) Datadog APP key. This can also be set via the DD_APP_KEY environment variable.
         """
         return __config__.get('appKey')
 
     @property
     def http_client_retry_enabled(self) -> Optional[bool]:
         """
-        Enables request retries on HTTP status codes 429 and 5xx.
+        Enables request retries on HTTP status codes 429 and 5xx. Defaults to `true`.
         """
         return __config__.get_bool('httpClientRetryEnabled')
 
     @property
     def http_client_retry_timeout(self) -> Optional[int]:
         """
         The HTTP request retry timeout period.
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/dashboard.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,21 +25,22 @@
                  restricted_roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  template_variable_presets: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardTemplateVariablePresetArgs']]]] = None,
                  template_variables: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardTemplateVariableArgs']]]] = None,
                  url: Optional[pulumi.Input[str]] = None,
                  widgets: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetArgs']]]] = None):
         """
         The set of arguments for constructing a Dashboard resource.
-        :param pulumi.Input[str] layout_type: The layout type of the dashboard. Valid values are `ordered`, `free`.
+        :param pulumi.Input[str] layout_type: The layout type of the dashboard.
         :param pulumi.Input[str] title: The title of the dashboard.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] dashboard_lists: A list of dashboard lists this dashboard belongs to.
         :param pulumi.Input[str] description: The description of the dashboard.
-        :param pulumi.Input[bool] is_read_only: Whether this dashboard is read-only. **Deprecated.** Prefer using `restricted_roles` to define which roles are required to edit the dashboard.
+        :param pulumi.Input[bool] is_read_only: Whether this dashboard is read-only.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] notify_lists: The list of handles for the users to notify when changes are made to this dashboard.
-        :param pulumi.Input[str] reflow_type: The reflow type of a new dashboard layout. Set this only when layout type is `ordered`. If set to `fixed`, the dashboard expects all widgets to have a layout, and if it's set to `auto`, widgets should not have layouts. Valid values are `auto`, `fixed`.
+        :param pulumi.Input[str] reflow_type: The reflow type of a new dashboard layout. Set this only when layout type is `ordered`. If set to `fixed`, the dashboard
+               expects all widgets to have a layout, and if it's set to `auto`, widgets should not have layouts.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] restricted_roles: UUIDs of roles whose associated users are authorized to edit the dashboard.
         :param pulumi.Input[Sequence[pulumi.Input['DashboardTemplateVariablePresetArgs']]] template_variable_presets: The list of selectable template variable presets for this dashboard.
         :param pulumi.Input[Sequence[pulumi.Input['DashboardTemplateVariableArgs']]] template_variables: The list of template variables for this dashboard.
         :param pulumi.Input[str] url: The URL of the dashboard.
         :param pulumi.Input[Sequence[pulumi.Input['DashboardWidgetArgs']]] widgets: The list of widgets to display on the dashboard.
         """
         pulumi.set(__self__, "layout_type", layout_type)
@@ -68,15 +69,15 @@
         if widgets is not None:
             pulumi.set(__self__, "widgets", widgets)
 
     @property
     @pulumi.getter(name="layoutType")
     def layout_type(self) -> pulumi.Input[str]:
         """
-        The layout type of the dashboard. Valid values are `ordered`, `free`.
+        The layout type of the dashboard.
         """
         return pulumi.get(self, "layout_type")
 
     @layout_type.setter
     def layout_type(self, value: pulumi.Input[str]):
         pulumi.set(self, "layout_type", value)
 
@@ -116,15 +117,15 @@
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter(name="isReadOnly")
     def is_read_only(self) -> Optional[pulumi.Input[bool]]:
         """
-        Whether this dashboard is read-only. **Deprecated.** Prefer using `restricted_roles` to define which roles are required to edit the dashboard.
+        Whether this dashboard is read-only.
         """
         return pulumi.get(self, "is_read_only")
 
     @is_read_only.setter
     def is_read_only(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "is_read_only", value)
 
@@ -140,15 +141,16 @@
     def notify_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "notify_lists", value)
 
     @property
     @pulumi.getter(name="reflowType")
     def reflow_type(self) -> Optional[pulumi.Input[str]]:
         """
-        The reflow type of a new dashboard layout. Set this only when layout type is `ordered`. If set to `fixed`, the dashboard expects all widgets to have a layout, and if it's set to `auto`, widgets should not have layouts. Valid values are `auto`, `fixed`.
+        The reflow type of a new dashboard layout. Set this only when layout type is `ordered`. If set to `fixed`, the dashboard
+        expects all widgets to have a layout, and if it's set to `auto`, widgets should not have layouts.
         """
         return pulumi.get(self, "reflow_type")
 
     @reflow_type.setter
     def reflow_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "reflow_type", value)
 
@@ -230,18 +232,19 @@
                  url: Optional[pulumi.Input[str]] = None,
                  widgets: Optional[pulumi.Input[Sequence[pulumi.Input['DashboardWidgetArgs']]]] = None):
         """
         Input properties used for looking up and filtering Dashboard resources.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] dashboard_lists: A list of dashboard lists this dashboard belongs to.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] dashboard_lists_removeds: A list of dashboard lists this dashboard should be removed from. Internal only.
         :param pulumi.Input[str] description: The description of the dashboard.
-        :param pulumi.Input[bool] is_read_only: Whether this dashboard is read-only. **Deprecated.** Prefer using `restricted_roles` to define which roles are required to edit the dashboard.
-        :param pulumi.Input[str] layout_type: The layout type of the dashboard. Valid values are `ordered`, `free`.
+        :param pulumi.Input[bool] is_read_only: Whether this dashboard is read-only.
+        :param pulumi.Input[str] layout_type: The layout type of the dashboard.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] notify_lists: The list of handles for the users to notify when changes are made to this dashboard.
-        :param pulumi.Input[str] reflow_type: The reflow type of a new dashboard layout. Set this only when layout type is `ordered`. If set to `fixed`, the dashboard expects all widgets to have a layout, and if it's set to `auto`, widgets should not have layouts. Valid values are `auto`, `fixed`.
+        :param pulumi.Input[str] reflow_type: The reflow type of a new dashboard layout. Set this only when layout type is `ordered`. If set to `fixed`, the dashboard
+               expects all widgets to have a layout, and if it's set to `auto`, widgets should not have layouts.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] restricted_roles: UUIDs of roles whose associated users are authorized to edit the dashboard.
         :param pulumi.Input[Sequence[pulumi.Input['DashboardTemplateVariablePresetArgs']]] template_variable_presets: The list of selectable template variable presets for this dashboard.
         :param pulumi.Input[Sequence[pulumi.Input['DashboardTemplateVariableArgs']]] template_variables: The list of template variables for this dashboard.
         :param pulumi.Input[str] title: The title of the dashboard.
         :param pulumi.Input[str] url: The URL of the dashboard.
         :param pulumi.Input[Sequence[pulumi.Input['DashboardWidgetArgs']]] widgets: The list of widgets to display on the dashboard.
         """
@@ -311,27 +314,27 @@
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter(name="isReadOnly")
     def is_read_only(self) -> Optional[pulumi.Input[bool]]:
         """
-        Whether this dashboard is read-only. **Deprecated.** Prefer using `restricted_roles` to define which roles are required to edit the dashboard.
+        Whether this dashboard is read-only.
         """
         return pulumi.get(self, "is_read_only")
 
     @is_read_only.setter
     def is_read_only(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "is_read_only", value)
 
     @property
     @pulumi.getter(name="layoutType")
     def layout_type(self) -> Optional[pulumi.Input[str]]:
         """
-        The layout type of the dashboard. Valid values are `ordered`, `free`.
+        The layout type of the dashboard.
         """
         return pulumi.get(self, "layout_type")
 
     @layout_type.setter
     def layout_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "layout_type", value)
 
@@ -347,15 +350,16 @@
     def notify_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "notify_lists", value)
 
     @property
     @pulumi.getter(name="reflowType")
     def reflow_type(self) -> Optional[pulumi.Input[str]]:
         """
-        The reflow type of a new dashboard layout. Set this only when layout type is `ordered`. If set to `fixed`, the dashboard expects all widgets to have a layout, and if it's set to `auto`, widgets should not have layouts. Valid values are `auto`, `fixed`.
+        The reflow type of a new dashboard layout. Set this only when layout type is `ordered`. If set to `fixed`, the dashboard
+        expects all widgets to have a layout, and if it's set to `auto`, widgets should not have layouts.
         """
         return pulumi.get(self, "reflow_type")
 
     @reflow_type.setter
     def reflow_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "reflow_type", value)
 
@@ -1151,18 +1155,19 @@
          $ pulumi import datadog:index/dashboard:Dashboard my_service_dashboard sv7-gyh-kas
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] dashboard_lists: A list of dashboard lists this dashboard belongs to.
         :param pulumi.Input[str] description: The description of the dashboard.
-        :param pulumi.Input[bool] is_read_only: Whether this dashboard is read-only. **Deprecated.** Prefer using `restricted_roles` to define which roles are required to edit the dashboard.
-        :param pulumi.Input[str] layout_type: The layout type of the dashboard. Valid values are `ordered`, `free`.
+        :param pulumi.Input[bool] is_read_only: Whether this dashboard is read-only.
+        :param pulumi.Input[str] layout_type: The layout type of the dashboard.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] notify_lists: The list of handles for the users to notify when changes are made to this dashboard.
-        :param pulumi.Input[str] reflow_type: The reflow type of a new dashboard layout. Set this only when layout type is `ordered`. If set to `fixed`, the dashboard expects all widgets to have a layout, and if it's set to `auto`, widgets should not have layouts. Valid values are `auto`, `fixed`.
+        :param pulumi.Input[str] reflow_type: The reflow type of a new dashboard layout. Set this only when layout type is `ordered`. If set to `fixed`, the dashboard
+               expects all widgets to have a layout, and if it's set to `auto`, widgets should not have layouts.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] restricted_roles: UUIDs of roles whose associated users are authorized to edit the dashboard.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DashboardTemplateVariablePresetArgs']]]] template_variable_presets: The list of selectable template variable presets for this dashboard.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DashboardTemplateVariableArgs']]]] template_variables: The list of template variables for this dashboard.
         :param pulumi.Input[str] title: The title of the dashboard.
         :param pulumi.Input[str] url: The URL of the dashboard.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DashboardWidgetArgs']]]] widgets: The list of widgets to display on the dashboard.
         """
@@ -1961,18 +1966,19 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] dashboard_lists: A list of dashboard lists this dashboard belongs to.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] dashboard_lists_removeds: A list of dashboard lists this dashboard should be removed from. Internal only.
         :param pulumi.Input[str] description: The description of the dashboard.
-        :param pulumi.Input[bool] is_read_only: Whether this dashboard is read-only. **Deprecated.** Prefer using `restricted_roles` to define which roles are required to edit the dashboard.
-        :param pulumi.Input[str] layout_type: The layout type of the dashboard. Valid values are `ordered`, `free`.
+        :param pulumi.Input[bool] is_read_only: Whether this dashboard is read-only.
+        :param pulumi.Input[str] layout_type: The layout type of the dashboard.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] notify_lists: The list of handles for the users to notify when changes are made to this dashboard.
-        :param pulumi.Input[str] reflow_type: The reflow type of a new dashboard layout. Set this only when layout type is `ordered`. If set to `fixed`, the dashboard expects all widgets to have a layout, and if it's set to `auto`, widgets should not have layouts. Valid values are `auto`, `fixed`.
+        :param pulumi.Input[str] reflow_type: The reflow type of a new dashboard layout. Set this only when layout type is `ordered`. If set to `fixed`, the dashboard
+               expects all widgets to have a layout, and if it's set to `auto`, widgets should not have layouts.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] restricted_roles: UUIDs of roles whose associated users are authorized to edit the dashboard.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DashboardTemplateVariablePresetArgs']]]] template_variable_presets: The list of selectable template variable presets for this dashboard.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DashboardTemplateVariableArgs']]]] template_variables: The list of template variables for this dashboard.
         :param pulumi.Input[str] title: The title of the dashboard.
         :param pulumi.Input[str] url: The URL of the dashboard.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DashboardWidgetArgs']]]] widgets: The list of widgets to display on the dashboard.
         """
@@ -2019,23 +2025,23 @@
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter(name="isReadOnly")
     def is_read_only(self) -> pulumi.Output[Optional[bool]]:
         """
-        Whether this dashboard is read-only. **Deprecated.** Prefer using `restricted_roles` to define which roles are required to edit the dashboard.
+        Whether this dashboard is read-only.
         """
         return pulumi.get(self, "is_read_only")
 
     @property
     @pulumi.getter(name="layoutType")
     def layout_type(self) -> pulumi.Output[str]:
         """
-        The layout type of the dashboard. Valid values are `ordered`, `free`.
+        The layout type of the dashboard.
         """
         return pulumi.get(self, "layout_type")
 
     @property
     @pulumi.getter(name="notifyLists")
     def notify_lists(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
@@ -2043,15 +2049,16 @@
         """
         return pulumi.get(self, "notify_lists")
 
     @property
     @pulumi.getter(name="reflowType")
     def reflow_type(self) -> pulumi.Output[Optional[str]]:
         """
-        The reflow type of a new dashboard layout. Set this only when layout type is `ordered`. If set to `fixed`, the dashboard expects all widgets to have a layout, and if it's set to `auto`, widgets should not have layouts. Valid values are `auto`, `fixed`.
+        The reflow type of a new dashboard layout. Set this only when layout type is `ordered`. If set to `fixed`, the dashboard
+        expects all widgets to have a layout, and if it's set to `auto`, widgets should not have layouts.
         """
         return pulumi.get(self, "reflow_type")
 
     @property
     @pulumi.getter(name="restrictedRoles")
     def restricted_roles(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/dashboard_json.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/dashboard_json.py`

 * *Files identical despite different names*

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/dashboard_list.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/dashboard_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/downtime.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/downtime.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,26 +17,29 @@
     def __init__(__self__, *,
                  scopes: pulumi.Input[Sequence[pulumi.Input[str]]],
                  end: Optional[pulumi.Input[int]] = None,
                  end_date: Optional[pulumi.Input[str]] = None,
                  message: Optional[pulumi.Input[str]] = None,
                  monitor_id: Optional[pulumi.Input[int]] = None,
                  monitor_tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 mute_first_recovery_notification: Optional[pulumi.Input[bool]] = None,
                  recurrence: Optional[pulumi.Input['DowntimeRecurrenceArgs']] = None,
                  start: Optional[pulumi.Input[int]] = None,
                  start_date: Optional[pulumi.Input[str]] = None,
                  timezone: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Downtime resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: specify the group scope to which this downtime applies. For everything use '*'
         :param pulumi.Input[int] end: Optionally specify an end date when this downtime should expire
         :param pulumi.Input[str] end_date: String representing date and time to end the downtime in RFC3339 format.
         :param pulumi.Input[str] message: An optional message to provide when creating the downtime, can include notification handles
         :param pulumi.Input[int] monitor_id: When specified, this downtime will only apply to this monitor
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] monitor_tags: A list of monitor tags (up to 32) to base the scheduled downtime on. Only monitors that have all selected tags are silenced
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] monitor_tags: A list of monitor tags (up to 32) to base the scheduled downtime on. Only monitors that have all selected tags are
+               silenced
+        :param pulumi.Input[bool] mute_first_recovery_notification: When true the first recovery notification during the downtime will be muted
         :param pulumi.Input['DowntimeRecurrenceArgs'] recurrence: Optional recurring schedule for this downtime
         :param pulumi.Input[int] start: Specify when this downtime should start
         :param pulumi.Input[str] start_date: String representing date and time to start the downtime in RFC3339 format.
         :param pulumi.Input[str] timezone: The timezone for the downtime, default UTC
         """
         pulumi.set(__self__, "scopes", scopes)
         if end is not None:
@@ -45,14 +48,16 @@
             pulumi.set(__self__, "end_date", end_date)
         if message is not None:
             pulumi.set(__self__, "message", message)
         if monitor_id is not None:
             pulumi.set(__self__, "monitor_id", monitor_id)
         if monitor_tags is not None:
             pulumi.set(__self__, "monitor_tags", monitor_tags)
+        if mute_first_recovery_notification is not None:
+            pulumi.set(__self__, "mute_first_recovery_notification", mute_first_recovery_notification)
         if recurrence is not None:
             pulumi.set(__self__, "recurrence", recurrence)
         if start is not None:
             pulumi.set(__self__, "start", start)
         if start_date is not None:
             pulumi.set(__self__, "start_date", start_date)
         if timezone is not None:
@@ -118,23 +123,36 @@
     def monitor_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "monitor_id", value)
 
     @property
     @pulumi.getter(name="monitorTags")
     def monitor_tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of monitor tags (up to 32) to base the scheduled downtime on. Only monitors that have all selected tags are silenced
+        A list of monitor tags (up to 32) to base the scheduled downtime on. Only monitors that have all selected tags are
+        silenced
         """
         return pulumi.get(self, "monitor_tags")
 
     @monitor_tags.setter
     def monitor_tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "monitor_tags", value)
 
     @property
+    @pulumi.getter(name="muteFirstRecoveryNotification")
+    def mute_first_recovery_notification(self) -> Optional[pulumi.Input[bool]]:
+        """
+        When true the first recovery notification during the downtime will be muted
+        """
+        return pulumi.get(self, "mute_first_recovery_notification")
+
+    @mute_first_recovery_notification.setter
+    def mute_first_recovery_notification(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "mute_first_recovery_notification", value)
+
+    @property
     @pulumi.getter
     def recurrence(self) -> Optional[pulumi.Input['DowntimeRecurrenceArgs']]:
         """
         Optional recurring schedule for this downtime
         """
         return pulumi.get(self, "recurrence")
 
@@ -186,29 +204,33 @@
                  active_child_id: Optional[pulumi.Input[int]] = None,
                  disabled: Optional[pulumi.Input[bool]] = None,
                  end: Optional[pulumi.Input[int]] = None,
                  end_date: Optional[pulumi.Input[str]] = None,
                  message: Optional[pulumi.Input[str]] = None,
                  monitor_id: Optional[pulumi.Input[int]] = None,
                  monitor_tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 mute_first_recovery_notification: Optional[pulumi.Input[bool]] = None,
                  recurrence: Optional[pulumi.Input['DowntimeRecurrenceArgs']] = None,
                  scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  start: Optional[pulumi.Input[int]] = None,
                  start_date: Optional[pulumi.Input[str]] = None,
                  timezone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Downtime resources.
         :param pulumi.Input[bool] active: When true indicates this downtime is being actively applied
-        :param pulumi.Input[int] active_child_id: The id corresponding to the downtime object definition of the active child for the original parent recurring downtime. This field will only exist on recurring downtimes.
+        :param pulumi.Input[int] active_child_id: The id corresponding to the downtime object definition of the active child for the original parent recurring downtime.
+               This field will only exist on recurring downtimes.
         :param pulumi.Input[bool] disabled: When true indicates this downtime is not being applied
         :param pulumi.Input[int] end: Optionally specify an end date when this downtime should expire
         :param pulumi.Input[str] end_date: String representing date and time to end the downtime in RFC3339 format.
         :param pulumi.Input[str] message: An optional message to provide when creating the downtime, can include notification handles
         :param pulumi.Input[int] monitor_id: When specified, this downtime will only apply to this monitor
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] monitor_tags: A list of monitor tags (up to 32) to base the scheduled downtime on. Only monitors that have all selected tags are silenced
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] monitor_tags: A list of monitor tags (up to 32) to base the scheduled downtime on. Only monitors that have all selected tags are
+               silenced
+        :param pulumi.Input[bool] mute_first_recovery_notification: When true the first recovery notification during the downtime will be muted
         :param pulumi.Input['DowntimeRecurrenceArgs'] recurrence: Optional recurring schedule for this downtime
         :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: specify the group scope to which this downtime applies. For everything use '*'
         :param pulumi.Input[int] start: Specify when this downtime should start
         :param pulumi.Input[str] start_date: String representing date and time to start the downtime in RFC3339 format.
         :param pulumi.Input[str] timezone: The timezone for the downtime, default UTC
         """
         if active is not None:
@@ -223,14 +245,16 @@
             pulumi.set(__self__, "end_date", end_date)
         if message is not None:
             pulumi.set(__self__, "message", message)
         if monitor_id is not None:
             pulumi.set(__self__, "monitor_id", monitor_id)
         if monitor_tags is not None:
             pulumi.set(__self__, "monitor_tags", monitor_tags)
+        if mute_first_recovery_notification is not None:
+            pulumi.set(__self__, "mute_first_recovery_notification", mute_first_recovery_notification)
         if recurrence is not None:
             pulumi.set(__self__, "recurrence", recurrence)
         if scopes is not None:
             pulumi.set(__self__, "scopes", scopes)
         if start is not None:
             pulumi.set(__self__, "start", start)
         if start_date is not None:
@@ -250,15 +274,16 @@
     def active(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "active", value)
 
     @property
     @pulumi.getter(name="activeChildId")
     def active_child_id(self) -> Optional[pulumi.Input[int]]:
         """
-        The id corresponding to the downtime object definition of the active child for the original parent recurring downtime. This field will only exist on recurring downtimes.
+        The id corresponding to the downtime object definition of the active child for the original parent recurring downtime.
+        This field will only exist on recurring downtimes.
         """
         return pulumi.get(self, "active_child_id")
 
     @active_child_id.setter
     def active_child_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "active_child_id", value)
 
@@ -322,23 +347,36 @@
     def monitor_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "monitor_id", value)
 
     @property
     @pulumi.getter(name="monitorTags")
     def monitor_tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of monitor tags (up to 32) to base the scheduled downtime on. Only monitors that have all selected tags are silenced
+        A list of monitor tags (up to 32) to base the scheduled downtime on. Only monitors that have all selected tags are
+        silenced
         """
         return pulumi.get(self, "monitor_tags")
 
     @monitor_tags.setter
     def monitor_tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "monitor_tags", value)
 
     @property
+    @pulumi.getter(name="muteFirstRecoveryNotification")
+    def mute_first_recovery_notification(self) -> Optional[pulumi.Input[bool]]:
+        """
+        When true the first recovery notification during the downtime will be muted
+        """
+        return pulumi.get(self, "mute_first_recovery_notification")
+
+    @mute_first_recovery_notification.setter
+    def mute_first_recovery_notification(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "mute_first_recovery_notification", value)
+
+    @property
     @pulumi.getter
     def recurrence(self) -> Optional[pulumi.Input['DowntimeRecurrenceArgs']]:
         """
         Optional recurring schedule for this downtime
         """
         return pulumi.get(self, "recurrence")
 
@@ -401,14 +439,15 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  end: Optional[pulumi.Input[int]] = None,
                  end_date: Optional[pulumi.Input[str]] = None,
                  message: Optional[pulumi.Input[str]] = None,
                  monitor_id: Optional[pulumi.Input[int]] = None,
                  monitor_tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 mute_first_recovery_notification: Optional[pulumi.Input[bool]] = None,
                  recurrence: Optional[pulumi.Input[pulumi.InputType['DowntimeRecurrenceArgs']]] = None,
                  scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  start: Optional[pulumi.Input[int]] = None,
                  start_date: Optional[pulumi.Input[str]] = None,
                  timezone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
@@ -440,15 +479,17 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] end: Optionally specify an end date when this downtime should expire
         :param pulumi.Input[str] end_date: String representing date and time to end the downtime in RFC3339 format.
         :param pulumi.Input[str] message: An optional message to provide when creating the downtime, can include notification handles
         :param pulumi.Input[int] monitor_id: When specified, this downtime will only apply to this monitor
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] monitor_tags: A list of monitor tags (up to 32) to base the scheduled downtime on. Only monitors that have all selected tags are silenced
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] monitor_tags: A list of monitor tags (up to 32) to base the scheduled downtime on. Only monitors that have all selected tags are
+               silenced
+        :param pulumi.Input[bool] mute_first_recovery_notification: When true the first recovery notification during the downtime will be muted
         :param pulumi.Input[pulumi.InputType['DowntimeRecurrenceArgs']] recurrence: Optional recurring schedule for this downtime
         :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: specify the group scope to which this downtime applies. For everything use '*'
         :param pulumi.Input[int] start: Specify when this downtime should start
         :param pulumi.Input[str] start_date: String representing date and time to start the downtime in RFC3339 format.
         :param pulumi.Input[str] timezone: The timezone for the downtime, default UTC
         """
         ...
@@ -500,14 +541,15 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  end: Optional[pulumi.Input[int]] = None,
                  end_date: Optional[pulumi.Input[str]] = None,
                  message: Optional[pulumi.Input[str]] = None,
                  monitor_id: Optional[pulumi.Input[int]] = None,
                  monitor_tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 mute_first_recovery_notification: Optional[pulumi.Input[bool]] = None,
                  recurrence: Optional[pulumi.Input[pulumi.InputType['DowntimeRecurrenceArgs']]] = None,
                  scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  start: Optional[pulumi.Input[int]] = None,
                  start_date: Optional[pulumi.Input[str]] = None,
                  timezone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         if opts is None:
@@ -522,14 +564,15 @@
             __props__ = DowntimeArgs.__new__(DowntimeArgs)
 
             __props__.__dict__["end"] = end
             __props__.__dict__["end_date"] = end_date
             __props__.__dict__["message"] = message
             __props__.__dict__["monitor_id"] = monitor_id
             __props__.__dict__["monitor_tags"] = monitor_tags
+            __props__.__dict__["mute_first_recovery_notification"] = mute_first_recovery_notification
             __props__.__dict__["recurrence"] = recurrence
             if scopes is None and not opts.urn:
                 raise TypeError("Missing required property 'scopes'")
             __props__.__dict__["scopes"] = scopes
             __props__.__dict__["start"] = start
             __props__.__dict__["start_date"] = start_date
             __props__.__dict__["timezone"] = timezone
@@ -550,34 +593,38 @@
             active_child_id: Optional[pulumi.Input[int]] = None,
             disabled: Optional[pulumi.Input[bool]] = None,
             end: Optional[pulumi.Input[int]] = None,
             end_date: Optional[pulumi.Input[str]] = None,
             message: Optional[pulumi.Input[str]] = None,
             monitor_id: Optional[pulumi.Input[int]] = None,
             monitor_tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            mute_first_recovery_notification: Optional[pulumi.Input[bool]] = None,
             recurrence: Optional[pulumi.Input[pulumi.InputType['DowntimeRecurrenceArgs']]] = None,
             scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             start: Optional[pulumi.Input[int]] = None,
             start_date: Optional[pulumi.Input[str]] = None,
             timezone: Optional[pulumi.Input[str]] = None) -> 'Downtime':
         """
         Get an existing Downtime resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] active: When true indicates this downtime is being actively applied
-        :param pulumi.Input[int] active_child_id: The id corresponding to the downtime object definition of the active child for the original parent recurring downtime. This field will only exist on recurring downtimes.
+        :param pulumi.Input[int] active_child_id: The id corresponding to the downtime object definition of the active child for the original parent recurring downtime.
+               This field will only exist on recurring downtimes.
         :param pulumi.Input[bool] disabled: When true indicates this downtime is not being applied
         :param pulumi.Input[int] end: Optionally specify an end date when this downtime should expire
         :param pulumi.Input[str] end_date: String representing date and time to end the downtime in RFC3339 format.
         :param pulumi.Input[str] message: An optional message to provide when creating the downtime, can include notification handles
         :param pulumi.Input[int] monitor_id: When specified, this downtime will only apply to this monitor
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] monitor_tags: A list of monitor tags (up to 32) to base the scheduled downtime on. Only monitors that have all selected tags are silenced
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] monitor_tags: A list of monitor tags (up to 32) to base the scheduled downtime on. Only monitors that have all selected tags are
+               silenced
+        :param pulumi.Input[bool] mute_first_recovery_notification: When true the first recovery notification during the downtime will be muted
         :param pulumi.Input[pulumi.InputType['DowntimeRecurrenceArgs']] recurrence: Optional recurring schedule for this downtime
         :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: specify the group scope to which this downtime applies. For everything use '*'
         :param pulumi.Input[int] start: Specify when this downtime should start
         :param pulumi.Input[str] start_date: String representing date and time to start the downtime in RFC3339 format.
         :param pulumi.Input[str] timezone: The timezone for the downtime, default UTC
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
@@ -588,14 +635,15 @@
         __props__.__dict__["active_child_id"] = active_child_id
         __props__.__dict__["disabled"] = disabled
         __props__.__dict__["end"] = end
         __props__.__dict__["end_date"] = end_date
         __props__.__dict__["message"] = message
         __props__.__dict__["monitor_id"] = monitor_id
         __props__.__dict__["monitor_tags"] = monitor_tags
+        __props__.__dict__["mute_first_recovery_notification"] = mute_first_recovery_notification
         __props__.__dict__["recurrence"] = recurrence
         __props__.__dict__["scopes"] = scopes
         __props__.__dict__["start"] = start
         __props__.__dict__["start_date"] = start_date
         __props__.__dict__["timezone"] = timezone
         return Downtime(resource_name, opts=opts, __props__=__props__)
 
@@ -607,15 +655,16 @@
         """
         return pulumi.get(self, "active")
 
     @property
     @pulumi.getter(name="activeChildId")
     def active_child_id(self) -> pulumi.Output[int]:
         """
-        The id corresponding to the downtime object definition of the active child for the original parent recurring downtime. This field will only exist on recurring downtimes.
+        The id corresponding to the downtime object definition of the active child for the original parent recurring downtime.
+        This field will only exist on recurring downtimes.
         """
         return pulumi.get(self, "active_child_id")
 
     @property
     @pulumi.getter
     def disabled(self) -> pulumi.Output[bool]:
         """
@@ -655,19 +704,28 @@
         """
         return pulumi.get(self, "monitor_id")
 
     @property
     @pulumi.getter(name="monitorTags")
     def monitor_tags(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of monitor tags (up to 32) to base the scheduled downtime on. Only monitors that have all selected tags are silenced
+        A list of monitor tags (up to 32) to base the scheduled downtime on. Only monitors that have all selected tags are
+        silenced
         """
         return pulumi.get(self, "monitor_tags")
 
     @property
+    @pulumi.getter(name="muteFirstRecoveryNotification")
+    def mute_first_recovery_notification(self) -> pulumi.Output[Optional[bool]]:
+        """
+        When true the first recovery notification during the downtime will be muted
+        """
+        return pulumi.get(self, "mute_first_recovery_notification")
+
+    @property
     @pulumi.getter
     def recurrence(self) -> pulumi.Output[Optional['outputs.DowntimeRecurrence']]:
         """
         Optional recurring schedule for this downtime
         """
         return pulumi.get(self, "recurrence")
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/gcp/integration.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/gcp/integration.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,16 @@
         The set of arguments for constructing a Integration resource.
         :param pulumi.Input[str] client_email: Your email found in your JSON service account key.
         :param pulumi.Input[str] client_id: Your ID found in your JSON service account key.
         :param pulumi.Input[str] private_key: Your private key name found in your JSON service account key.
         :param pulumi.Input[str] private_key_id: Your private key ID found in your JSON service account key.
         :param pulumi.Input[str] project_id: Your Google Cloud project ID found in your JSON service account key.
         :param pulumi.Input[bool] automute: Silence monitors for expected GCE instance shutdowns.
-        :param pulumi.Input[str] host_filters: Limit the GCE instances that are pulled into Datadog by using tags. Only hosts that match one of the defined tags are imported into Datadog.
+        :param pulumi.Input[str] host_filters: Limit the GCE instances that are pulled into Datadog by using tags. Only hosts that match one of the defined tags are
+               imported into Datadog.
         """
         pulumi.set(__self__, "client_email", client_email)
         pulumi.set(__self__, "client_id", client_id)
         pulumi.set(__self__, "private_key", private_key)
         pulumi.set(__self__, "private_key_id", private_key_id)
         pulumi.set(__self__, "project_id", project_id)
         if automute is not None:
@@ -112,15 +113,16 @@
     def automute(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "automute", value)
 
     @property
     @pulumi.getter(name="hostFilters")
     def host_filters(self) -> Optional[pulumi.Input[str]]:
         """
-        Limit the GCE instances that are pulled into Datadog by using tags. Only hosts that match one of the defined tags are imported into Datadog.
+        Limit the GCE instances that are pulled into Datadog by using tags. Only hosts that match one of the defined tags are
+        imported into Datadog.
         """
         return pulumi.get(self, "host_filters")
 
     @host_filters.setter
     def host_filters(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "host_filters", value)
 
@@ -136,15 +138,16 @@
                  private_key_id: Optional[pulumi.Input[str]] = None,
                  project_id: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Integration resources.
         :param pulumi.Input[bool] automute: Silence monitors for expected GCE instance shutdowns.
         :param pulumi.Input[str] client_email: Your email found in your JSON service account key.
         :param pulumi.Input[str] client_id: Your ID found in your JSON service account key.
-        :param pulumi.Input[str] host_filters: Limit the GCE instances that are pulled into Datadog by using tags. Only hosts that match one of the defined tags are imported into Datadog.
+        :param pulumi.Input[str] host_filters: Limit the GCE instances that are pulled into Datadog by using tags. Only hosts that match one of the defined tags are
+               imported into Datadog.
         :param pulumi.Input[str] private_key: Your private key name found in your JSON service account key.
         :param pulumi.Input[str] private_key_id: Your private key ID found in your JSON service account key.
         :param pulumi.Input[str] project_id: Your Google Cloud project ID found in your JSON service account key.
         """
         if automute is not None:
             pulumi.set(__self__, "automute", automute)
         if client_email is not None:
@@ -196,15 +199,16 @@
     def client_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "client_id", value)
 
     @property
     @pulumi.getter(name="hostFilters")
     def host_filters(self) -> Optional[pulumi.Input[str]]:
         """
-        Limit the GCE instances that are pulled into Datadog by using tags. Only hosts that match one of the defined tags are imported into Datadog.
+        Limit the GCE instances that are pulled into Datadog by using tags. Only hosts that match one of the defined tags are
+        imported into Datadog.
         """
         return pulumi.get(self, "host_filters")
 
     @host_filters.setter
     def host_filters(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "host_filters", value)
 
@@ -290,15 +294,16 @@
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] automute: Silence monitors for expected GCE instance shutdowns.
         :param pulumi.Input[str] client_email: Your email found in your JSON service account key.
         :param pulumi.Input[str] client_id: Your ID found in your JSON service account key.
-        :param pulumi.Input[str] host_filters: Limit the GCE instances that are pulled into Datadog by using tags. Only hosts that match one of the defined tags are imported into Datadog.
+        :param pulumi.Input[str] host_filters: Limit the GCE instances that are pulled into Datadog by using tags. Only hosts that match one of the defined tags are
+               imported into Datadog.
         :param pulumi.Input[str] private_key: Your private key name found in your JSON service account key.
         :param pulumi.Input[str] private_key_id: Your private key ID found in your JSON service account key.
         :param pulumi.Input[str] project_id: Your Google Cloud project ID found in your JSON service account key.
         """
         ...
     @overload
     def __init__(__self__,
@@ -410,15 +415,16 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] automute: Silence monitors for expected GCE instance shutdowns.
         :param pulumi.Input[str] client_email: Your email found in your JSON service account key.
         :param pulumi.Input[str] client_id: Your ID found in your JSON service account key.
-        :param pulumi.Input[str] host_filters: Limit the GCE instances that are pulled into Datadog by using tags. Only hosts that match one of the defined tags are imported into Datadog.
+        :param pulumi.Input[str] host_filters: Limit the GCE instances that are pulled into Datadog by using tags. Only hosts that match one of the defined tags are
+               imported into Datadog.
         :param pulumi.Input[str] private_key: Your private key name found in your JSON service account key.
         :param pulumi.Input[str] private_key_id: Your private key ID found in your JSON service account key.
         :param pulumi.Input[str] project_id: Your Google Cloud project ID found in your JSON service account key.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _IntegrationState.__new__(_IntegrationState)
@@ -456,15 +462,16 @@
         """
         return pulumi.get(self, "client_id")
 
     @property
     @pulumi.getter(name="hostFilters")
     def host_filters(self) -> pulumi.Output[Optional[str]]:
         """
-        Limit the GCE instances that are pulled into Datadog by using tags. Only hosts that match one of the defined tags are imported into Datadog.
+        Limit the GCE instances that are pulled into Datadog by using tags. Only hosts that match one of the defined tags are
+        imported into Datadog.
         """
         return pulumi.get(self, "host_filters")
 
     @property
     @pulumi.getter(name="privateKey")
     def private_key(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_api_key.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_api_key.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,33 +30,24 @@
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
-        """
-        Id for API Key.
-        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def key(self) -> str:
-        """
-        The value of the API Key.
-        """
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
-        """
-        Name for API Key.
-        """
         return pulumi.get(self, "name")
 
 
 class AwaitableGetApiKeyResult(GetApiKeyResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -77,18 +68,14 @@
 
     ```python
     import pulumi
     import pulumi_datadog as datadog
 
     foo = datadog.get_api_key(name="foo-application")
     ```
-
-
-    :param str id: Id for API Key.
-    :param str name: Name for API Key.
     """
     __args__ = dict()
     __args__['id'] = id
     __args__['name'] = name
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
@@ -112,13 +99,9 @@
 
     ```python
     import pulumi
     import pulumi_datadog as datadog
 
     foo = datadog.get_api_key(name="foo-application")
     ```
-
-
-    :param str id: Id for API Key.
-    :param str name: Name for API Key.
     """
     ...
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_application_key.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_application_key.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,33 +30,24 @@
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
-        """
-        Id for Application Key.
-        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def key(self) -> str:
-        """
-        The value of the Application Key.
-        """
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
-        """
-        Name for Application Key.
-        """
         return pulumi.get(self, "name")
 
 
 class AwaitableGetApplicationKeyResult(GetApplicationKeyResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -77,18 +68,14 @@
 
     ```python
     import pulumi
     import pulumi_datadog as datadog
 
     foo = datadog.get_application_key(name="foo-application")
     ```
-
-
-    :param str id: Id for Application Key.
-    :param str name: Name for Application Key.
     """
     __args__ = dict()
     __args__['id'] = id
     __args__['name'] = name
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
@@ -112,13 +99,9 @@
 
     ```python
     import pulumi
     import pulumi_datadog as datadog
 
     foo = datadog.get_application_key(name="foo-application")
     ```
-
-
-    :param str id: Id for Application Key.
-    :param str name: Name for Application Key.
     """
     ...
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_cloud_workload_security_agent_rules.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_cloud_workload_security_agent_rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,17 +27,14 @@
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
 
     @property
     @pulumi.getter(name="agentRules")
     def agent_rules(self) -> Sequence['outputs.GetCloudWorkloadSecurityAgentRulesAgentRuleResult']:
-        """
-        List of Agent rules.
-        """
         return pulumi.get(self, "agent_rules")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_dashboard.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_dashboard.py`

 * *Files 25% similar despite different names*

```diff
@@ -41,33 +41,24 @@
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> str:
-        """
-        The dashboard name to search for. Must only match one dashboard.
-        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def title(self) -> str:
-        """
-        The name of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter
     def url(self) -> str:
-        """
-        The URL to a specific dashboard.
-        """
         return pulumi.get(self, "url")
 
 
 class AwaitableGetDashboardResult(GetDashboardResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -88,17 +79,14 @@
 
     ```python
     import pulumi
     import pulumi_datadog as datadog
 
     test = datadog.get_dashboard(name="My super dashboard")
     ```
-
-
-    :param str name: The dashboard name to search for. Must only match one dashboard.
     """
     __args__ = dict()
     __args__['name'] = name
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
@@ -121,12 +109,9 @@
 
     ```python
     import pulumi
     import pulumi_datadog as datadog
 
     test = datadog.get_dashboard(name="My super dashboard")
     ```
-
-
-    :param str name: The dashboard name to search for. Must only match one dashboard.
     """
     ...
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_dashboard_list.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_dashboard_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,17 +35,14 @@
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> str:
-        """
-        A dashboard list name to limit the search.
-        """
         return pulumi.get(self, "name")
 
 
 class AwaitableGetDashboardListResult(GetDashboardListResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -79,17 +76,14 @@
                 alert_id="1234",
                 live_span="1h",
                 title="Widget Title",
                 viz_type="timeseries",
             ),
         )])
     ```
-
-
-    :param str name: A dashboard list name to limit the search.
     """
     __args__ = dict()
     __args__['name'] = name
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
@@ -125,12 +119,9 @@
                 alert_id="1234",
                 live_span="1h",
                 title="Widget Title",
                 viz_type="timeseries",
             ),
         )])
     ```
-
-
-    :param str name: A dashboard list name to limit the search.
     """
     ...
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_ip_ranges.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_ip_ranges.py`

 * *Files 18% similar despite different names*

```diff
@@ -71,145 +71,97 @@
         if webhooks_ipv6s and not isinstance(webhooks_ipv6s, list):
             raise TypeError("Expected argument 'webhooks_ipv6s' to be a list")
         pulumi.set(__self__, "webhooks_ipv6s", webhooks_ipv6s)
 
     @property
     @pulumi.getter(name="agentsIpv4s")
     def agents_ipv4s(self) -> Sequence[str]:
-        """
-        An Array of IPv4 addresses in CIDR format specifying the A records for the Agent endpoint.
-        """
         return pulumi.get(self, "agents_ipv4s")
 
     @property
     @pulumi.getter(name="agentsIpv6s")
     def agents_ipv6s(self) -> Sequence[str]:
-        """
-        An Array of IPv6 addresses in CIDR format specifying the A records for the Agent endpoint.
-        """
         return pulumi.get(self, "agents_ipv6s")
 
     @property
     @pulumi.getter(name="apiIpv4s")
     def api_ipv4s(self) -> Sequence[str]:
-        """
-        An Array of IPv4 addresses in CIDR format specifying the A records for the API endpoint.
-        """
         return pulumi.get(self, "api_ipv4s")
 
     @property
     @pulumi.getter(name="apiIpv6s")
     def api_ipv6s(self) -> Sequence[str]:
-        """
-        An Array of IPv6 addresses in CIDR format specifying the A records for the API endpoint.
-        """
         return pulumi.get(self, "api_ipv6s")
 
     @property
     @pulumi.getter(name="apmIpv4s")
     def apm_ipv4s(self) -> Sequence[str]:
-        """
-        An Array of IPv4 addresses in CIDR format specifying the A records for the APM endpoint.
-        """
         return pulumi.get(self, "apm_ipv4s")
 
     @property
     @pulumi.getter(name="apmIpv6s")
     def apm_ipv6s(self) -> Sequence[str]:
-        """
-        An Array of IPv6 addresses in CIDR format specifying the A records for the APM endpoint.
-        """
         return pulumi.get(self, "apm_ipv6s")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="logsIpv4s")
     def logs_ipv4s(self) -> Sequence[str]:
-        """
-        An Array of IPv4 addresses in CIDR format specifying the A records for the Logs endpoint.
-        """
         return pulumi.get(self, "logs_ipv4s")
 
     @property
     @pulumi.getter(name="logsIpv6s")
     def logs_ipv6s(self) -> Sequence[str]:
-        """
-        An Array of IPv6 addresses in CIDR format specifying the A records for the Logs endpoint.
-        """
         return pulumi.get(self, "logs_ipv6s")
 
     @property
     @pulumi.getter(name="processIpv4s")
     def process_ipv4s(self) -> Sequence[str]:
-        """
-        An Array of IPv4 addresses in CIDR format specifying the A records for the Process endpoint.
-        """
         return pulumi.get(self, "process_ipv4s")
 
     @property
     @pulumi.getter(name="processIpv6s")
     def process_ipv6s(self) -> Sequence[str]:
-        """
-        An Array of IPv6 addresses in CIDR format specifying the A records for the Process endpoint.
-        """
         return pulumi.get(self, "process_ipv6s")
 
     @property
     @pulumi.getter(name="syntheticsIpv4ByLocation")
     def synthetics_ipv4_by_location(self) -> Mapping[str, Any]:
-        """
-        A map of IPv4 prefixes (string of concatenated IPs, delimited by ',') by location.
-        """
         return pulumi.get(self, "synthetics_ipv4_by_location")
 
     @property
     @pulumi.getter(name="syntheticsIpv4s")
     def synthetics_ipv4s(self) -> Sequence[str]:
-        """
-        An Array of IPv4 addresses in CIDR format specifying the A records for the Synthetics endpoint.
-        """
         return pulumi.get(self, "synthetics_ipv4s")
 
     @property
     @pulumi.getter(name="syntheticsIpv6ByLocation")
     def synthetics_ipv6_by_location(self) -> Mapping[str, Any]:
-        """
-        A map of IPv6 prefixes (string of concatenated IPs, delimited by ',') by location.
-        """
         return pulumi.get(self, "synthetics_ipv6_by_location")
 
     @property
     @pulumi.getter(name="syntheticsIpv6s")
     def synthetics_ipv6s(self) -> Sequence[str]:
-        """
-        An Array of IPv6 addresses in CIDR format specifying the A records for the Synthetics endpoint.
-        """
         return pulumi.get(self, "synthetics_ipv6s")
 
     @property
     @pulumi.getter(name="webhooksIpv4s")
     def webhooks_ipv4s(self) -> Sequence[str]:
-        """
-        An Array of IPv4 addresses in CIDR format specifying the A records for the Webhooks endpoint.
-        """
         return pulumi.get(self, "webhooks_ipv4s")
 
     @property
     @pulumi.getter(name="webhooksIpv6s")
     def webhooks_ipv6s(self) -> Sequence[str]:
-        """
-        An Array of IPv6 addresses in CIDR format specifying the A records for the Webhooks endpoint.
-        """
         return pulumi.get(self, "webhooks_ipv6s")
 
 
 class AwaitableGetIpRangesResult(GetIpRangesResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_logs_indexes.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_logs_indexes.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,17 +35,14 @@
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="logsIndexes")
     def logs_indexes(self) -> Sequence['outputs.GetLogsIndexesLogsIndexResult']:
-        """
-        List of logs indexes
-        """
         return pulumi.get(self, "logs_indexes")
 
 
 class AwaitableGetLogsIndexesResult(GetLogsIndexesResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_logs_indexes_order.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_logs_indexes_order.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,17 +34,14 @@
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="indexNames")
     def index_names(self) -> Sequence[str]:
-        """
-        Array of strings identifying by their name(s) the index(es) of your organization. Logs are tested against the query filter of each index one by one, following the order of the array. Logs are eventually stored in the first matching index.
-        """
         return pulumi.get(self, "index_names")
 
 
 class AwaitableGetLogsIndexesOrderResult(GetLogsIndexesOrderResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_monitor.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_monitor.py`

 * *Files 24% similar despite different names*

```diff
@@ -106,230 +106,152 @@
         if type and not isinstance(type, str):
             raise TypeError("Expected argument 'type' to be a str")
         pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter(name="enableLogsSample")
     def enable_logs_sample(self) -> bool:
-        """
-        Whether or not a list of log values which triggered the alert is included. This is only used by log monitors.
-        """
         return pulumi.get(self, "enable_logs_sample")
 
     @property
     @pulumi.getter(name="escalationMessage")
     def escalation_message(self) -> str:
-        """
-        Message included with a re-notification for this monitor.
-        """
         return pulumi.get(self, "escalation_message")
 
     @property
     @pulumi.getter(name="evaluationDelay")
     def evaluation_delay(self) -> int:
-        """
-        Time (in seconds) for which evaluation is delayed. This is only used by metric monitors.
-        """
         return pulumi.get(self, "evaluation_delay")
 
     @property
     @pulumi.getter(name="groupbySimpleMonitor")
     def groupby_simple_monitor(self) -> bool:
-        """
-        Whether or not to trigger one alert if any source breaches a threshold.
-        """
         return pulumi.get(self, "groupby_simple_monitor")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="includeTags")
     def include_tags(self) -> bool:
-        """
-        Whether or not notifications from the monitor automatically inserts its triggering tags into the title.
-        """
         return pulumi.get(self, "include_tags")
 
     @property
     @pulumi.getter
     def locked(self) -> bool:
-        """
-        Whether or not changes to the monitor are restricted to the creator or admins.
-        """
         return pulumi.get(self, "locked")
 
     @property
     @pulumi.getter
     def message(self) -> str:
-        """
-        Message included with notifications for this monitor
-        """
         return pulumi.get(self, "message")
 
     @property
     @pulumi.getter(name="monitorTagsFilters")
     def monitor_tags_filters(self) -> Optional[Sequence[str]]:
-        """
-        A list of monitor tags to limit the search. This filters on the tags set on the monitor itself.
-        """
         return pulumi.get(self, "monitor_tags_filters")
 
     @property
     @pulumi.getter(name="monitorThresholdWindows")
     def monitor_threshold_windows(self) -> Sequence['outputs.GetMonitorMonitorThresholdWindowResult']:
-        """
-        Mapping containing `recovery_window` and `trigger_window` values, e.g. `last_15m`. This is only used by anomaly monitors.
-        """
         return pulumi.get(self, "monitor_threshold_windows")
 
     @property
     @pulumi.getter(name="monitorThresholds")
     def monitor_thresholds(self) -> Sequence['outputs.GetMonitorMonitorThresholdResult']:
-        """
-        Alert thresholds of the monitor.
-        """
         return pulumi.get(self, "monitor_thresholds")
 
     @property
     @pulumi.getter
     def name(self) -> str:
-        """
-        Name of the monitor
-        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="nameFilter")
     def name_filter(self) -> Optional[str]:
-        """
-        A monitor name to limit the search.
-        """
         return pulumi.get(self, "name_filter")
 
     @property
     @pulumi.getter(name="newGroupDelay")
     def new_group_delay(self) -> int:
-        """
-        Time (in seconds) to skip evaluations for new groups.
-        """
         return pulumi.get(self, "new_group_delay")
 
     @property
     @pulumi.getter(name="newHostDelay")
     def new_host_delay(self) -> int:
-        """
-        Time (in seconds) allowing a host to boot and applications to fully start before starting the evaluation of monitor results.
-        """
         return pulumi.get(self, "new_host_delay")
 
     @property
     @pulumi.getter(name="noDataTimeframe")
     def no_data_timeframe(self) -> int:
-        """
-        The number of minutes before the monitor notifies when data stops reporting.
-        """
         return pulumi.get(self, "no_data_timeframe")
 
     @property
     @pulumi.getter(name="notifyAudit")
     def notify_audit(self) -> bool:
-        """
-        Whether or not tagged users are notified on changes to the monitor.
-        """
         return pulumi.get(self, "notify_audit")
 
     @property
     @pulumi.getter(name="notifyNoData")
     def notify_no_data(self) -> bool:
-        """
-        Whether or not this monitor notifies when data stops reporting.
-        """
         return pulumi.get(self, "notify_no_data")
 
     @property
     @pulumi.getter
     def query(self) -> str:
-        """
-        Query of the monitor.
-        """
         return pulumi.get(self, "query")
 
     @property
     @pulumi.getter(name="renotifyInterval")
     def renotify_interval(self) -> int:
-        """
-        The number of minutes after the last notification before the monitor re-notifies on the current status.
-        """
         return pulumi.get(self, "renotify_interval")
 
     @property
     @pulumi.getter(name="renotifyOccurrences")
     def renotify_occurrences(self) -> int:
-        """
-        The number of re-notification messages that should be sent on the current status.
-        """
         return pulumi.get(self, "renotify_occurrences")
 
     @property
     @pulumi.getter(name="renotifyStatuses")
     def renotify_statuses(self) -> Sequence[str]:
-        """
-        The types of statuses for which re-notification messages should be sent. Valid values are `alert`, `warn`, `no data`.
-        """
         return pulumi.get(self, "renotify_statuses")
 
     @property
     @pulumi.getter(name="requireFullWindow")
     def require_full_window(self) -> bool:
-        """
-        Whether or not the monitor needs a full window of data before it is evaluated.
-        """
         return pulumi.get(self, "require_full_window")
 
     @property
     @pulumi.getter(name="restrictedRoles")
     def restricted_roles(self) -> Sequence[str]:
         return pulumi.get(self, "restricted_roles")
 
     @property
     @pulumi.getter
     def tags(self) -> Sequence[str]:
-        """
-        List of tags associated with the monitor.
-        """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tagsFilters")
     def tags_filters(self) -> Optional[Sequence[str]]:
-        """
-        A list of tags to limit the search. This filters on the monitor scope.
-        """
         return pulumi.get(self, "tags_filters")
 
     @property
     @pulumi.getter(name="timeoutH")
     def timeout_h(self) -> int:
-        """
-        Number of hours of the monitor not reporting data before it automatically resolves from a triggered state.
-        """
         return pulumi.get(self, "timeout_h")
 
     @property
     @pulumi.getter
     def type(self) -> str:
-        """
-        Type of the monitor.
-        """
         return pulumi.get(self, "type")
 
 
 class AwaitableGetMonitorResult(GetMonitorResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -377,19 +299,14 @@
     ```python
     import pulumi
     import pulumi_datadog as datadog
 
     test = datadog.get_monitor(monitor_tags_filters=["foo:bar"],
         name_filter="My awesome monitor")
     ```
-
-
-    :param Sequence[str] monitor_tags_filters: A list of monitor tags to limit the search. This filters on the tags set on the monitor itself.
-    :param str name_filter: A monitor name to limit the search.
-    :param Sequence[str] tags_filters: A list of tags to limit the search. This filters on the monitor scope.
     """
     __args__ = dict()
     __args__['monitorTagsFilters'] = monitor_tags_filters
     __args__['nameFilter'] = name_filter
     __args__['tagsFilters'] = tags_filters
     if opts is None:
         opts = pulumi.InvokeOptions()
@@ -441,14 +358,9 @@
     ```python
     import pulumi
     import pulumi_datadog as datadog
 
     test = datadog.get_monitor(monitor_tags_filters=["foo:bar"],
         name_filter="My awesome monitor")
     ```
-
-
-    :param Sequence[str] monitor_tags_filters: A list of monitor tags to limit the search. This filters on the tags set on the monitor itself.
-    :param str name_filter: A monitor name to limit the search.
-    :param Sequence[str] tags_filters: A list of tags to limit the search. This filters on the monitor scope.
     """
     ...
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_monitors.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_monitors.py`

 * *Files 21% similar despite different names*

```diff
@@ -45,41 +45,29 @@
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="monitorTagsFilters")
     def monitor_tags_filters(self) -> Optional[Sequence[str]]:
-        """
-        A list of monitor tags to limit the search. This filters on the tags set on the monitor itself.
-        """
         return pulumi.get(self, "monitor_tags_filters")
 
     @property
     @pulumi.getter
     def monitors(self) -> Sequence['outputs.GetMonitorsMonitorResult']:
-        """
-        List of monitors
-        """
         return pulumi.get(self, "monitors")
 
     @property
     @pulumi.getter(name="nameFilter")
     def name_filter(self) -> Optional[str]:
-        """
-        A monitor name to limit the search.
-        """
         return pulumi.get(self, "name_filter")
 
     @property
     @pulumi.getter(name="tagsFilters")
     def tags_filters(self) -> Optional[Sequence[str]]:
-        """
-        A list of tags to limit the search. This filters on the monitor scope.
-        """
         return pulumi.get(self, "tags_filters")
 
 
 class AwaitableGetMonitorsResult(GetMonitorsResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -94,19 +82,14 @@
 
 def get_monitors(monitor_tags_filters: Optional[Sequence[str]] = None,
                  name_filter: Optional[str] = None,
                  tags_filters: Optional[Sequence[str]] = None,
                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetMonitorsResult:
     """
     Use this data source to list several existing monitors for use in other resources.
-
-
-    :param Sequence[str] monitor_tags_filters: A list of monitor tags to limit the search. This filters on the tags set on the monitor itself.
-    :param str name_filter: A monitor name to limit the search.
-    :param Sequence[str] tags_filters: A list of tags to limit the search. This filters on the monitor scope.
     """
     __args__ = dict()
     __args__['monitorTagsFilters'] = monitor_tags_filters
     __args__['nameFilter'] = name_filter
     __args__['tagsFilters'] = tags_filters
     if opts is None:
         opts = pulumi.InvokeOptions()
@@ -125,14 +108,9 @@
 @_utilities.lift_output_func(get_monitors)
 def get_monitors_output(monitor_tags_filters: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                         name_filter: Optional[pulumi.Input[Optional[str]]] = None,
                         tags_filters: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetMonitorsResult]:
     """
     Use this data source to list several existing monitors for use in other resources.
-
-
-    :param Sequence[str] monitor_tags_filters: A list of monitor tags to limit the search. This filters on the tags set on the monitor itself.
-    :param str name_filter: A monitor name to limit the search.
-    :param Sequence[str] tags_filters: A list of tags to limit the search. This filters on the monitor scope.
     """
     ...
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_permissions.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_permissions.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,17 +34,14 @@
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def permissions(self) -> Mapping[str, str]:
-        """
-        Map of permissions names to their corresponding ID.
-        """
         return pulumi.get(self, "permissions")
 
 
 class AwaitableGetPermissionsResult(GetPermissionsResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_role.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_role.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,41 +33,32 @@
         if user_count and not isinstance(user_count, int):
             raise TypeError("Expected argument 'user_count' to be a int")
         pulumi.set(__self__, "user_count", user_count)
 
     @property
     @pulumi.getter
     def filter(self) -> str:
-        """
-        A string on which to filter the roles.
-        """
         return pulumi.get(self, "filter")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> str:
-        """
-        Name of the role.
-        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="userCount")
     def user_count(self) -> int:
-        """
-        Number of users assigned to this role.
-        """
         return pulumi.get(self, "user_count")
 
 
 class AwaitableGetRoleResult(GetRoleResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -88,17 +79,14 @@
 
     ```python
     import pulumi
     import pulumi_datadog as datadog
 
     test = datadog.get_role(filter="Datadog Standard Role")
     ```
-
-
-    :param str filter: A string on which to filter the roles.
     """
     __args__ = dict()
     __args__['filter'] = filter
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
@@ -121,12 +109,9 @@
 
     ```python
     import pulumi
     import pulumi_datadog as datadog
 
     test = datadog.get_role(filter="Datadog Standard Role")
     ```
-
-
-    :param str filter: A string on which to filter the roles.
     """
     ...
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_roles.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_roles.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,33 +31,27 @@
         if roles and not isinstance(roles, list):
             raise TypeError("Expected argument 'roles' to be a list")
         pulumi.set(__self__, "roles", roles)
 
     @property
     @pulumi.getter
     def filter(self) -> Optional[str]:
-        """
-        Filter all roles by the given string.
-        """
         return pulumi.get(self, "filter")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def roles(self) -> Sequence['outputs.GetRolesRoleResult']:
-        """
-        List of Roles
-        """
         return pulumi.get(self, "roles")
 
 
 class AwaitableGetRolesResult(GetRolesResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -77,17 +71,14 @@
 
     ```python
     import pulumi
     import pulumi_datadog as datadog
 
     foo = datadog.get_roles(filter="Datadog")
     ```
-
-
-    :param str filter: Filter all roles by the given string.
     """
     __args__ = dict()
     __args__['filter'] = filter
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
@@ -109,12 +100,9 @@
 
     ```python
     import pulumi
     import pulumi_datadog as datadog
 
     foo = datadog.get_roles(filter="Datadog")
     ```
-
-
-    :param str filter: Filter all roles by the given string.
     """
     ...
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_security_monitoring_filters.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_security_monitoring_filters.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,25 +30,19 @@
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
 
     @property
     @pulumi.getter
     def filters(self) -> Sequence['outputs.GetSecurityMonitoringFiltersFilterResult']:
-        """
-        List of filters.
-        """
         return pulumi.get(self, "filters")
 
     @property
     @pulumi.getter(name="filtersIds")
     def filters_ids(self) -> Sequence[str]:
-        """
-        List of IDs of filters.
-        """
         return pulumi.get(self, "filters_ids")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_security_monitoring_rules.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_security_monitoring_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_service_level_objective.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_service_level_objective.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,57 +39,39 @@
         if type and not isinstance(type, str):
             raise TypeError("Expected argument 'type' to be a str")
         pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
-        """
-        A SLO ID to limit the search.
-        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="metricsQuery")
     def metrics_query(self) -> Optional[str]:
-        """
-        Filter results based on SLO numerator and denominator.
-        """
         return pulumi.get(self, "metrics_query")
 
     @property
     @pulumi.getter
     def name(self) -> str:
-        """
-        Name of the Datadog service level objective
-        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="nameQuery")
     def name_query(self) -> Optional[str]:
-        """
-        Filter results based on SLO names.
-        """
         return pulumi.get(self, "name_query")
 
     @property
     @pulumi.getter(name="tagsQuery")
     def tags_query(self) -> Optional[str]:
-        """
-        Filter results based on a single SLO tag.
-        """
         return pulumi.get(self, "tags_query")
 
     @property
     @pulumi.getter
     def type(self) -> str:
-        """
-        The type of the service level objective. The mapping from these types to the types found in the Datadog Web UI can be found in the Datadog API [documentation page](https://docs.datadoghq.com/api/v1/service-level-objectives/#create-a-slo-object). Available values are: `metric` and `monitor`.
-        """
         return pulumi.get(self, "type")
 
 
 class AwaitableGetServiceLevelObjectiveResult(GetServiceLevelObjectiveResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -117,20 +99,14 @@
     import pulumi
     import pulumi_datadog as datadog
 
     test = datadog.get_service_level_objective(name_query="My test SLO",
         tags_query="foo:bar")
     api_slo = datadog.get_service_level_objective(id=data["terraform_remote_state"]["api"]["outputs"]["slo"])
     ```
-
-
-    :param str id: A SLO ID to limit the search.
-    :param str metrics_query: Filter results based on SLO numerator and denominator.
-    :param str name_query: Filter results based on SLO names.
-    :param str tags_query: Filter results based on a single SLO tag.
     """
     __args__ = dict()
     __args__['id'] = id
     __args__['metricsQuery'] = metrics_query
     __args__['nameQuery'] = name_query
     __args__['tagsQuery'] = tags_query
     if opts is None:
@@ -163,15 +139,9 @@
     import pulumi
     import pulumi_datadog as datadog
 
     test = datadog.get_service_level_objective(name_query="My test SLO",
         tags_query="foo:bar")
     api_slo = datadog.get_service_level_objective(id=data["terraform_remote_state"]["api"]["outputs"]["slo"])
     ```
-
-
-    :param str id: A SLO ID to limit the search.
-    :param str metrics_query: Filter results based on SLO numerator and denominator.
-    :param str name_query: Filter results based on SLO names.
-    :param str tags_query: Filter results based on a single SLO tag.
     """
     ...
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_service_level_objectives.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_service_level_objectives.py`

 * *Files 27% similar despite different names*

```diff
@@ -48,49 +48,34 @@
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def ids(self) -> Optional[Sequence[str]]:
-        """
-        An array of SLO IDs to limit the search.
-        """
         return pulumi.get(self, "ids")
 
     @property
     @pulumi.getter(name="metricsQuery")
     def metrics_query(self) -> Optional[str]:
-        """
-        Filter results based on SLO numerator and denominator.
-        """
         return pulumi.get(self, "metrics_query")
 
     @property
     @pulumi.getter(name="nameQuery")
     def name_query(self) -> Optional[str]:
-        """
-        Filter results based on SLO names.
-        """
         return pulumi.get(self, "name_query")
 
     @property
     @pulumi.getter
     def slos(self) -> Sequence['outputs.GetServiceLevelObjectivesSloResult']:
-        """
-        List of SLOs
-        """
         return pulumi.get(self, "slos")
 
     @property
     @pulumi.getter(name="tagsQuery")
     def tags_query(self) -> Optional[str]:
-        """
-        Filter results based on a single SLO tag.
-        """
         return pulumi.get(self, "tags_query")
 
 
 class AwaitableGetServiceLevelObjectivesResult(GetServiceLevelObjectivesResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -116,20 +101,14 @@
 
     ```python
     import pulumi
     import pulumi_datadog as datadog
 
     ft_foo_slos = datadog.get_service_level_objectives(tags_query="owner:ft-foo")
     ```
-
-
-    :param Sequence[str] ids: An array of SLO IDs to limit the search.
-    :param str metrics_query: Filter results based on SLO numerator and denominator.
-    :param str name_query: Filter results based on SLO names.
-    :param str tags_query: Filter results based on a single SLO tag.
     """
     __args__ = dict()
     __args__['ids'] = ids
     __args__['metricsQuery'] = metrics_query
     __args__['nameQuery'] = name_query
     __args__['tagsQuery'] = tags_query
     if opts is None:
@@ -160,15 +139,9 @@
 
     ```python
     import pulumi
     import pulumi_datadog as datadog
 
     ft_foo_slos = datadog.get_service_level_objectives(tags_query="owner:ft-foo")
     ```
-
-
-    :param Sequence[str] ids: An array of SLO IDs to limit the search.
-    :param str metrics_query: Filter results based on SLO numerator and denominator.
-    :param str name_query: Filter results based on SLO names.
-    :param str tags_query: Filter results based on a single SLO tag.
     """
     ...
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_synthetics_global_variable.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_synthetics_global_variable.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,25 +38,19 @@
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> str:
-        """
-        The synthetics global variable name to search for. Must only match one global variable.
-        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def tags(self) -> Sequence[str]:
-        """
-        A list of tags assigned to the Synthetics global variable.
-        """
         return pulumi.get(self, "tags")
 
 
 class AwaitableGetSyntheticsGlobalVariableResult(GetSyntheticsGlobalVariableResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -67,17 +61,14 @@
             tags=self.tags)
 
 
 def get_synthetics_global_variable(name: Optional[str] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetSyntheticsGlobalVariableResult:
     """
     Use this data source to retrieve a Datadog Synthetics global variable (to be used in Synthetics tests).
-
-
-    :param str name: The synthetics global variable name to search for. Must only match one global variable.
     """
     __args__ = dict()
     __args__['name'] = name
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
@@ -90,12 +81,9 @@
 
 
 @_utilities.lift_output_func(get_synthetics_global_variable)
 def get_synthetics_global_variable_output(name: Optional[pulumi.Input[str]] = None,
                                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSyntheticsGlobalVariableResult]:
     """
     Use this data source to retrieve a Datadog Synthetics global variable (to be used in Synthetics tests).
-
-
-    :param str name: The synthetics global variable name to search for. Must only match one global variable.
     """
     ...
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_synthetics_locations.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_synthetics_locations.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,17 +34,14 @@
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def locations(self) -> Mapping[str, Any]:
-        """
-        A map of available Synthetics location IDs to names for Synthetics tests.
-        """
         return pulumi.get(self, "locations")
 
 
 class AwaitableGetSyntheticsLocationsResult(GetSyntheticsLocationsResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_synthetics_test.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_synthetics_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -44,41 +44,29 @@
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> str:
-        """
-        The name of the synthetic test.
-        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def tags(self) -> Sequence[str]:
-        """
-        A list of tags assigned to the synthetic test.
-        """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="testId")
     def test_id(self) -> str:
-        """
-        The synthetic test id to search for
-        """
         return pulumi.get(self, "test_id")
 
     @property
     @pulumi.getter
     def url(self) -> str:
-        """
-        The start URL of the synthetic test.
-        """
         return pulumi.get(self, "url")
 
 
 class AwaitableGetSyntheticsTestResult(GetSyntheticsTestResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -91,17 +79,14 @@
             url=self.url)
 
 
 def get_synthetics_test(test_id: Optional[str] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetSyntheticsTestResult:
     """
     Use this data source to retrieve a Datadog Synthetic Test.
-
-
-    :param str test_id: The synthetic test id to search for
     """
     __args__ = dict()
     __args__['testId'] = test_id
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
@@ -116,12 +101,9 @@
 
 
 @_utilities.lift_output_func(get_synthetics_test)
 def get_synthetics_test_output(test_id: Optional[pulumi.Input[str]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSyntheticsTestResult]:
     """
     Use this data source to retrieve a Datadog Synthetic Test.
-
-
-    :param str test_id: The synthetic test id to search for
     """
     ...
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/get_user.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/get_user.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,41 +33,32 @@
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def email(self) -> str:
-        """
-        Email of the user.
-        """
         return pulumi.get(self, "email")
 
     @property
     @pulumi.getter
     def filter(self) -> str:
-        """
-        Filter all users by the given string.
-        """
         return pulumi.get(self, "filter")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> str:
-        """
-        Name of the user.
-        """
         return pulumi.get(self, "name")
 
 
 class AwaitableGetUserResult(GetUserResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -79,17 +70,14 @@
             name=self.name)
 
 
 def get_user(filter: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetUserResult:
     """
     Use this data source to retrieve information about an existing user to use it in an other resources.
-
-
-    :param str filter: Filter all users by the given string.
     """
     __args__ = dict()
     __args__['filter'] = filter
     if opts is None:
         opts = pulumi.InvokeOptions()
     if opts.version is None:
         opts.version = _utilities.get_version()
@@ -103,12 +91,9 @@
 
 
 @_utilities.lift_output_func(get_user)
 def get_user_output(filter: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUserResult]:
     """
     Use this data source to retrieve information about an existing user to use it in an other resources.
-
-
-    :param str filter: Filter all users by the given string.
     """
     ...
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/logs_archive.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/logs_archive.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,34 +16,39 @@
 class LogsArchiveArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  query: pulumi.Input[str],
                  azure_archive: Optional[pulumi.Input['LogsArchiveAzureArchiveArgs']] = None,
                  gcs_archive: Optional[pulumi.Input['LogsArchiveGcsArchiveArgs']] = None,
                  include_tags: Optional[pulumi.Input[bool]] = None,
+                 rehydration_max_scan_size_in_gb: Optional[pulumi.Input[int]] = None,
                  rehydration_tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  s3_archive: Optional[pulumi.Input['LogsArchiveS3ArchiveArgs']] = None):
         """
         The set of arguments for constructing a LogsArchive resource.
         :param pulumi.Input[str] name: Your archive name.
         :param pulumi.Input[str] query: The archive query/filter. Logs matching this query are included in the archive.
         :param pulumi.Input['LogsArchiveAzureArchiveArgs'] azure_archive: Definition of an azure archive.
         :param pulumi.Input['LogsArchiveGcsArchiveArgs'] gcs_archive: Definition of a GCS archive.
-        :param pulumi.Input[bool] include_tags: To store the tags in the archive, set the value `true`. If it is set to `false`, the tags will be dropped when the logs are sent to the archive.
+        :param pulumi.Input[bool] include_tags: To store the tags in the archive, set the value `true`. If it is set to `false`, the tags will be dropped when the logs
+               are sent to the archive.
+        :param pulumi.Input[int] rehydration_max_scan_size_in_gb: To limit the rehydration scan size for the archive, set a value in GB.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] rehydration_tags: An array of tags to add to rehydrated logs from an archive.
         :param pulumi.Input['LogsArchiveS3ArchiveArgs'] s3_archive: Definition of an s3 archive.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "query", query)
         if azure_archive is not None:
             pulumi.set(__self__, "azure_archive", azure_archive)
         if gcs_archive is not None:
             pulumi.set(__self__, "gcs_archive", gcs_archive)
         if include_tags is not None:
             pulumi.set(__self__, "include_tags", include_tags)
+        if rehydration_max_scan_size_in_gb is not None:
+            pulumi.set(__self__, "rehydration_max_scan_size_in_gb", rehydration_max_scan_size_in_gb)
         if rehydration_tags is not None:
             pulumi.set(__self__, "rehydration_tags", rehydration_tags)
         if s3_archive is not None:
             pulumi.set(__self__, "s3_archive", s3_archive)
 
     @property
     @pulumi.getter
@@ -93,23 +98,36 @@
     def gcs_archive(self, value: Optional[pulumi.Input['LogsArchiveGcsArchiveArgs']]):
         pulumi.set(self, "gcs_archive", value)
 
     @property
     @pulumi.getter(name="includeTags")
     def include_tags(self) -> Optional[pulumi.Input[bool]]:
         """
-        To store the tags in the archive, set the value `true`. If it is set to `false`, the tags will be dropped when the logs are sent to the archive.
+        To store the tags in the archive, set the value `true`. If it is set to `false`, the tags will be dropped when the logs
+        are sent to the archive.
         """
         return pulumi.get(self, "include_tags")
 
     @include_tags.setter
     def include_tags(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "include_tags", value)
 
     @property
+    @pulumi.getter(name="rehydrationMaxScanSizeInGb")
+    def rehydration_max_scan_size_in_gb(self) -> Optional[pulumi.Input[int]]:
+        """
+        To limit the rehydration scan size for the archive, set a value in GB.
+        """
+        return pulumi.get(self, "rehydration_max_scan_size_in_gb")
+
+    @rehydration_max_scan_size_in_gb.setter
+    def rehydration_max_scan_size_in_gb(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "rehydration_max_scan_size_in_gb", value)
+
+    @property
     @pulumi.getter(name="rehydrationTags")
     def rehydration_tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         An array of tags to add to rehydrated logs from an archive.
         """
         return pulumi.get(self, "rehydration_tags")
 
@@ -134,36 +152,41 @@
 class _LogsArchiveState:
     def __init__(__self__, *,
                  azure_archive: Optional[pulumi.Input['LogsArchiveAzureArchiveArgs']] = None,
                  gcs_archive: Optional[pulumi.Input['LogsArchiveGcsArchiveArgs']] = None,
                  include_tags: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  query: Optional[pulumi.Input[str]] = None,
+                 rehydration_max_scan_size_in_gb: Optional[pulumi.Input[int]] = None,
                  rehydration_tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  s3_archive: Optional[pulumi.Input['LogsArchiveS3ArchiveArgs']] = None):
         """
         Input properties used for looking up and filtering LogsArchive resources.
         :param pulumi.Input['LogsArchiveAzureArchiveArgs'] azure_archive: Definition of an azure archive.
         :param pulumi.Input['LogsArchiveGcsArchiveArgs'] gcs_archive: Definition of a GCS archive.
-        :param pulumi.Input[bool] include_tags: To store the tags in the archive, set the value `true`. If it is set to `false`, the tags will be dropped when the logs are sent to the archive.
+        :param pulumi.Input[bool] include_tags: To store the tags in the archive, set the value `true`. If it is set to `false`, the tags will be dropped when the logs
+               are sent to the archive.
         :param pulumi.Input[str] name: Your archive name.
         :param pulumi.Input[str] query: The archive query/filter. Logs matching this query are included in the archive.
+        :param pulumi.Input[int] rehydration_max_scan_size_in_gb: To limit the rehydration scan size for the archive, set a value in GB.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] rehydration_tags: An array of tags to add to rehydrated logs from an archive.
         :param pulumi.Input['LogsArchiveS3ArchiveArgs'] s3_archive: Definition of an s3 archive.
         """
         if azure_archive is not None:
             pulumi.set(__self__, "azure_archive", azure_archive)
         if gcs_archive is not None:
             pulumi.set(__self__, "gcs_archive", gcs_archive)
         if include_tags is not None:
             pulumi.set(__self__, "include_tags", include_tags)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if query is not None:
             pulumi.set(__self__, "query", query)
+        if rehydration_max_scan_size_in_gb is not None:
+            pulumi.set(__self__, "rehydration_max_scan_size_in_gb", rehydration_max_scan_size_in_gb)
         if rehydration_tags is not None:
             pulumi.set(__self__, "rehydration_tags", rehydration_tags)
         if s3_archive is not None:
             pulumi.set(__self__, "s3_archive", s3_archive)
 
     @property
     @pulumi.getter(name="azureArchive")
@@ -189,15 +212,16 @@
     def gcs_archive(self, value: Optional[pulumi.Input['LogsArchiveGcsArchiveArgs']]):
         pulumi.set(self, "gcs_archive", value)
 
     @property
     @pulumi.getter(name="includeTags")
     def include_tags(self) -> Optional[pulumi.Input[bool]]:
         """
-        To store the tags in the archive, set the value `true`. If it is set to `false`, the tags will be dropped when the logs are sent to the archive.
+        To store the tags in the archive, set the value `true`. If it is set to `false`, the tags will be dropped when the logs
+        are sent to the archive.
         """
         return pulumi.get(self, "include_tags")
 
     @include_tags.setter
     def include_tags(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "include_tags", value)
 
@@ -222,14 +246,26 @@
         return pulumi.get(self, "query")
 
     @query.setter
     def query(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "query", value)
 
     @property
+    @pulumi.getter(name="rehydrationMaxScanSizeInGb")
+    def rehydration_max_scan_size_in_gb(self) -> Optional[pulumi.Input[int]]:
+        """
+        To limit the rehydration scan size for the archive, set a value in GB.
+        """
+        return pulumi.get(self, "rehydration_max_scan_size_in_gb")
+
+    @rehydration_max_scan_size_in_gb.setter
+    def rehydration_max_scan_size_in_gb(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "rehydration_max_scan_size_in_gb", value)
+
+    @property
     @pulumi.getter(name="rehydrationTags")
     def rehydration_tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         An array of tags to add to rehydrated logs from an archive.
         """
         return pulumi.get(self, "rehydration_tags")
 
@@ -256,14 +292,15 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  azure_archive: Optional[pulumi.Input[pulumi.InputType['LogsArchiveAzureArchiveArgs']]] = None,
                  gcs_archive: Optional[pulumi.Input[pulumi.InputType['LogsArchiveGcsArchiveArgs']]] = None,
                  include_tags: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  query: Optional[pulumi.Input[str]] = None,
+                 rehydration_max_scan_size_in_gb: Optional[pulumi.Input[int]] = None,
                  rehydration_tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  s3_archive: Optional[pulumi.Input[pulumi.InputType['LogsArchiveS3ArchiveArgs']]] = None,
                  __props__=None):
         """
         Provides a Datadog Logs Archive API resource, which is used to create and manage Datadog logs archives.
 
         ## Example Usage
@@ -289,17 +326,19 @@
          $ pulumi import datadog:index/logsArchive:LogsArchive my_s3_archive 1Aabc2_dfQPLnXy3HlfK4hi
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['LogsArchiveAzureArchiveArgs']] azure_archive: Definition of an azure archive.
         :param pulumi.Input[pulumi.InputType['LogsArchiveGcsArchiveArgs']] gcs_archive: Definition of a GCS archive.
-        :param pulumi.Input[bool] include_tags: To store the tags in the archive, set the value `true`. If it is set to `false`, the tags will be dropped when the logs are sent to the archive.
+        :param pulumi.Input[bool] include_tags: To store the tags in the archive, set the value `true`. If it is set to `false`, the tags will be dropped when the logs
+               are sent to the archive.
         :param pulumi.Input[str] name: Your archive name.
         :param pulumi.Input[str] query: The archive query/filter. Logs matching this query are included in the archive.
+        :param pulumi.Input[int] rehydration_max_scan_size_in_gb: To limit the rehydration scan size for the archive, set a value in GB.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] rehydration_tags: An array of tags to add to rehydrated logs from an archive.
         :param pulumi.Input[pulumi.InputType['LogsArchiveS3ArchiveArgs']] s3_archive: Definition of an s3 archive.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -347,14 +386,15 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  azure_archive: Optional[pulumi.Input[pulumi.InputType['LogsArchiveAzureArchiveArgs']]] = None,
                  gcs_archive: Optional[pulumi.Input[pulumi.InputType['LogsArchiveGcsArchiveArgs']]] = None,
                  include_tags: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  query: Optional[pulumi.Input[str]] = None,
+                 rehydration_max_scan_size_in_gb: Optional[pulumi.Input[int]] = None,
                  rehydration_tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  s3_archive: Optional[pulumi.Input[pulumi.InputType['LogsArchiveS3ArchiveArgs']]] = None,
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
@@ -370,14 +410,15 @@
             __props__.__dict__["include_tags"] = include_tags
             if name is None and not opts.urn:
                 raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
             if query is None and not opts.urn:
                 raise TypeError("Missing required property 'query'")
             __props__.__dict__["query"] = query
+            __props__.__dict__["rehydration_max_scan_size_in_gb"] = rehydration_max_scan_size_in_gb
             __props__.__dict__["rehydration_tags"] = rehydration_tags
             __props__.__dict__["s3_archive"] = s3_archive
         super(LogsArchive, __self__).__init__(
             'datadog:index/logsArchive:LogsArchive',
             resource_name,
             __props__,
             opts)
@@ -387,40 +428,44 @@
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             azure_archive: Optional[pulumi.Input[pulumi.InputType['LogsArchiveAzureArchiveArgs']]] = None,
             gcs_archive: Optional[pulumi.Input[pulumi.InputType['LogsArchiveGcsArchiveArgs']]] = None,
             include_tags: Optional[pulumi.Input[bool]] = None,
             name: Optional[pulumi.Input[str]] = None,
             query: Optional[pulumi.Input[str]] = None,
+            rehydration_max_scan_size_in_gb: Optional[pulumi.Input[int]] = None,
             rehydration_tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             s3_archive: Optional[pulumi.Input[pulumi.InputType['LogsArchiveS3ArchiveArgs']]] = None) -> 'LogsArchive':
         """
         Get an existing LogsArchive resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['LogsArchiveAzureArchiveArgs']] azure_archive: Definition of an azure archive.
         :param pulumi.Input[pulumi.InputType['LogsArchiveGcsArchiveArgs']] gcs_archive: Definition of a GCS archive.
-        :param pulumi.Input[bool] include_tags: To store the tags in the archive, set the value `true`. If it is set to `false`, the tags will be dropped when the logs are sent to the archive.
+        :param pulumi.Input[bool] include_tags: To store the tags in the archive, set the value `true`. If it is set to `false`, the tags will be dropped when the logs
+               are sent to the archive.
         :param pulumi.Input[str] name: Your archive name.
         :param pulumi.Input[str] query: The archive query/filter. Logs matching this query are included in the archive.
+        :param pulumi.Input[int] rehydration_max_scan_size_in_gb: To limit the rehydration scan size for the archive, set a value in GB.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] rehydration_tags: An array of tags to add to rehydrated logs from an archive.
         :param pulumi.Input[pulumi.InputType['LogsArchiveS3ArchiveArgs']] s3_archive: Definition of an s3 archive.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _LogsArchiveState.__new__(_LogsArchiveState)
 
         __props__.__dict__["azure_archive"] = azure_archive
         __props__.__dict__["gcs_archive"] = gcs_archive
         __props__.__dict__["include_tags"] = include_tags
         __props__.__dict__["name"] = name
         __props__.__dict__["query"] = query
+        __props__.__dict__["rehydration_max_scan_size_in_gb"] = rehydration_max_scan_size_in_gb
         __props__.__dict__["rehydration_tags"] = rehydration_tags
         __props__.__dict__["s3_archive"] = s3_archive
         return LogsArchive(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="azureArchive")
     def azure_archive(self) -> pulumi.Output[Optional['outputs.LogsArchiveAzureArchive']]:
@@ -437,15 +482,16 @@
         """
         return pulumi.get(self, "gcs_archive")
 
     @property
     @pulumi.getter(name="includeTags")
     def include_tags(self) -> pulumi.Output[Optional[bool]]:
         """
-        To store the tags in the archive, set the value `true`. If it is set to `false`, the tags will be dropped when the logs are sent to the archive.
+        To store the tags in the archive, set the value `true`. If it is set to `false`, the tags will be dropped when the logs
+        are sent to the archive.
         """
         return pulumi.get(self, "include_tags")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
@@ -458,14 +504,22 @@
     def query(self) -> pulumi.Output[str]:
         """
         The archive query/filter. Logs matching this query are included in the archive.
         """
         return pulumi.get(self, "query")
 
     @property
+    @pulumi.getter(name="rehydrationMaxScanSizeInGb")
+    def rehydration_max_scan_size_in_gb(self) -> pulumi.Output[Optional[int]]:
+        """
+        To limit the rehydration scan size for the archive, set a value in GB.
+        """
+        return pulumi.get(self, "rehydration_max_scan_size_in_gb")
+
+    @property
     @pulumi.getter(name="rehydrationTags")
     def rehydration_tags(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         An array of tags to add to rehydrated logs from an archive.
         """
         return pulumi.get(self, "rehydration_tags")
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/logs_archive_order.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/logs_archive_order.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,48 +12,56 @@
 
 @pulumi.input_type
 class LogsArchiveOrderArgs:
     def __init__(__self__, *,
                  archive_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a LogsArchiveOrder resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] archive_ids: The archive IDs list. The order of archive IDs in this attribute defines the overall archive order for logs. If `archive_ids` is empty or not specified, it will import the actual archive order, and create the resource. Otherwise, it will try to update the order.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] archive_ids: The archive IDs list. The order of archive IDs in this attribute defines the overall archive order for logs. If
+               `archive_ids` is empty or not specified, it will import the actual archive order, and create the resource. Otherwise, it
+               will try to update the order.
         """
         if archive_ids is not None:
             pulumi.set(__self__, "archive_ids", archive_ids)
 
     @property
     @pulumi.getter(name="archiveIds")
     def archive_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The archive IDs list. The order of archive IDs in this attribute defines the overall archive order for logs. If `archive_ids` is empty or not specified, it will import the actual archive order, and create the resource. Otherwise, it will try to update the order.
+        The archive IDs list. The order of archive IDs in this attribute defines the overall archive order for logs. If
+        `archive_ids` is empty or not specified, it will import the actual archive order, and create the resource. Otherwise, it
+        will try to update the order.
         """
         return pulumi.get(self, "archive_ids")
 
     @archive_ids.setter
     def archive_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "archive_ids", value)
 
 
 @pulumi.input_type
 class _LogsArchiveOrderState:
     def __init__(__self__, *,
                  archive_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering LogsArchiveOrder resources.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] archive_ids: The archive IDs list. The order of archive IDs in this attribute defines the overall archive order for logs. If `archive_ids` is empty or not specified, it will import the actual archive order, and create the resource. Otherwise, it will try to update the order.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] archive_ids: The archive IDs list. The order of archive IDs in this attribute defines the overall archive order for logs. If
+               `archive_ids` is empty or not specified, it will import the actual archive order, and create the resource. Otherwise, it
+               will try to update the order.
         """
         if archive_ids is not None:
             pulumi.set(__self__, "archive_ids", archive_ids)
 
     @property
     @pulumi.getter(name="archiveIds")
     def archive_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The archive IDs list. The order of archive IDs in this attribute defines the overall archive order for logs. If `archive_ids` is empty or not specified, it will import the actual archive order, and create the resource. Otherwise, it will try to update the order.
+        The archive IDs list. The order of archive IDs in this attribute defines the overall archive order for logs. If
+        `archive_ids` is empty or not specified, it will import the actual archive order, and create the resource. Otherwise, it
+        will try to update the order.
         """
         return pulumi.get(self, "archive_ids")
 
     @archive_ids.setter
     def archive_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "archive_ids", value)
 
@@ -86,15 +94,17 @@
 
         ```sh
          $ pulumi import datadog:index/logsArchiveOrder:LogsArchiveOrder name> archiveOrderID
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] archive_ids: The archive IDs list. The order of archive IDs in this attribute defines the overall archive order for logs. If `archive_ids` is empty or not specified, it will import the actual archive order, and create the resource. Otherwise, it will try to update the order.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] archive_ids: The archive IDs list. The order of archive IDs in this attribute defines the overall archive order for logs. If
+               `archive_ids` is empty or not specified, it will import the actual archive order, and create the resource. Otherwise, it
+               will try to update the order.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[LogsArchiveOrderArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -164,24 +174,28 @@
         """
         Get an existing LogsArchiveOrder resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] archive_ids: The archive IDs list. The order of archive IDs in this attribute defines the overall archive order for logs. If `archive_ids` is empty or not specified, it will import the actual archive order, and create the resource. Otherwise, it will try to update the order.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] archive_ids: The archive IDs list. The order of archive IDs in this attribute defines the overall archive order for logs. If
+               `archive_ids` is empty or not specified, it will import the actual archive order, and create the resource. Otherwise, it
+               will try to update the order.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _LogsArchiveOrderState.__new__(_LogsArchiveOrderState)
 
         __props__.__dict__["archive_ids"] = archive_ids
         return LogsArchiveOrder(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="archiveIds")
     def archive_ids(self) -> pulumi.Output[Sequence[str]]:
         """
-        The archive IDs list. The order of archive IDs in this attribute defines the overall archive order for logs. If `archive_ids` is empty or not specified, it will import the actual archive order, and create the resource. Otherwise, it will try to update the order.
+        The archive IDs list. The order of archive IDs in this attribute defines the overall archive order for logs. If
+        `archive_ids` is empty or not specified, it will import the actual archive order, and create the resource. Otherwise, it
+        will try to update the order.
         """
         return pulumi.get(self, "archive_ids")
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/logs_custom_pipeline.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/logs_custom_pipeline.py`

 * *Files identical despite different names*

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/logs_index.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/logs_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,16 @@
                  exclusion_filters: Optional[pulumi.Input[Sequence[pulumi.Input['LogsIndexExclusionFilterArgs']]]] = None,
                  retention_days: Optional[pulumi.Input[int]] = None):
         """
         The set of arguments for constructing a LogsIndex resource.
         :param pulumi.Input[Sequence[pulumi.Input['LogsIndexFilterArgs']]] filters: Logs filter
         :param pulumi.Input[str] name: The name of the index.
         :param pulumi.Input[int] daily_limit: The number of log events you can send in this index per day before you are rate-limited.
-        :param pulumi.Input[bool] disable_daily_limit: If true, sets the daily*limit value to null and the index is not limited on a daily basis (any specified daily*limit value in the request is ignored). If false or omitted, the index's current daily_limit is maintained.
+        :param pulumi.Input[bool] disable_daily_limit: If true, sets the daily_limit value to null and the index is not limited on a daily basis (any specified daily_limit
+               value in the request is ignored). If false or omitted, the index's current daily_limit is maintained.
         :param pulumi.Input[Sequence[pulumi.Input['LogsIndexExclusionFilterArgs']]] exclusion_filters: List of exclusion filters.
         :param pulumi.Input[int] retention_days: The number of days before logs are deleted from this index.
         """
         pulumi.set(__self__, "filters", filters)
         pulumi.set(__self__, "name", name)
         if daily_limit is not None:
             pulumi.set(__self__, "daily_limit", daily_limit)
@@ -77,15 +78,16 @@
     def daily_limit(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "daily_limit", value)
 
     @property
     @pulumi.getter(name="disableDailyLimit")
     def disable_daily_limit(self) -> Optional[pulumi.Input[bool]]:
         """
-        If true, sets the daily*limit value to null and the index is not limited on a daily basis (any specified daily*limit value in the request is ignored). If false or omitted, the index's current daily_limit is maintained.
+        If true, sets the daily_limit value to null and the index is not limited on a daily basis (any specified daily_limit
+        value in the request is ignored). If false or omitted, the index's current daily_limit is maintained.
         """
         return pulumi.get(self, "disable_daily_limit")
 
     @disable_daily_limit.setter
     def disable_daily_limit(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "disable_daily_limit", value)
 
@@ -122,15 +124,16 @@
                  exclusion_filters: Optional[pulumi.Input[Sequence[pulumi.Input['LogsIndexExclusionFilterArgs']]]] = None,
                  filters: Optional[pulumi.Input[Sequence[pulumi.Input['LogsIndexFilterArgs']]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  retention_days: Optional[pulumi.Input[int]] = None):
         """
         Input properties used for looking up and filtering LogsIndex resources.
         :param pulumi.Input[int] daily_limit: The number of log events you can send in this index per day before you are rate-limited.
-        :param pulumi.Input[bool] disable_daily_limit: If true, sets the daily*limit value to null and the index is not limited on a daily basis (any specified daily*limit value in the request is ignored). If false or omitted, the index's current daily_limit is maintained.
+        :param pulumi.Input[bool] disable_daily_limit: If true, sets the daily_limit value to null and the index is not limited on a daily basis (any specified daily_limit
+               value in the request is ignored). If false or omitted, the index's current daily_limit is maintained.
         :param pulumi.Input[Sequence[pulumi.Input['LogsIndexExclusionFilterArgs']]] exclusion_filters: List of exclusion filters.
         :param pulumi.Input[Sequence[pulumi.Input['LogsIndexFilterArgs']]] filters: Logs filter
         :param pulumi.Input[str] name: The name of the index.
         :param pulumi.Input[int] retention_days: The number of days before logs are deleted from this index.
         """
         if daily_limit is not None:
             pulumi.set(__self__, "daily_limit", daily_limit)
@@ -157,15 +160,16 @@
     def daily_limit(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "daily_limit", value)
 
     @property
     @pulumi.getter(name="disableDailyLimit")
     def disable_daily_limit(self) -> Optional[pulumi.Input[bool]]:
         """
-        If true, sets the daily*limit value to null and the index is not limited on a daily basis (any specified daily*limit value in the request is ignored). If false or omitted, the index's current daily_limit is maintained.
+        If true, sets the daily_limit value to null and the index is not limited on a daily basis (any specified daily_limit
+        value in the request is ignored). If false or omitted, the index's current daily_limit is maintained.
         """
         return pulumi.get(self, "disable_daily_limit")
 
     @disable_daily_limit.setter
     def disable_daily_limit(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "disable_daily_limit", value)
 
@@ -269,15 +273,16 @@
         ```sh
          $ pulumi import datadog:index/logsIndex:LogsIndex name> <indexName>
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] daily_limit: The number of log events you can send in this index per day before you are rate-limited.
-        :param pulumi.Input[bool] disable_daily_limit: If true, sets the daily*limit value to null and the index is not limited on a daily basis (any specified daily*limit value in the request is ignored). If false or omitted, the index's current daily_limit is maintained.
+        :param pulumi.Input[bool] disable_daily_limit: If true, sets the daily_limit value to null and the index is not limited on a daily basis (any specified daily_limit
+               value in the request is ignored). If false or omitted, the index's current daily_limit is maintained.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['LogsIndexExclusionFilterArgs']]]] exclusion_filters: List of exclusion filters.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['LogsIndexFilterArgs']]]] filters: Logs filter
         :param pulumi.Input[str] name: The name of the index.
         :param pulumi.Input[int] retention_days: The number of days before logs are deleted from this index.
         """
         ...
     @overload
@@ -388,15 +393,16 @@
         Get an existing LogsIndex resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] daily_limit: The number of log events you can send in this index per day before you are rate-limited.
-        :param pulumi.Input[bool] disable_daily_limit: If true, sets the daily*limit value to null and the index is not limited on a daily basis (any specified daily*limit value in the request is ignored). If false or omitted, the index's current daily_limit is maintained.
+        :param pulumi.Input[bool] disable_daily_limit: If true, sets the daily_limit value to null and the index is not limited on a daily basis (any specified daily_limit
+               value in the request is ignored). If false or omitted, the index's current daily_limit is maintained.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['LogsIndexExclusionFilterArgs']]]] exclusion_filters: List of exclusion filters.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['LogsIndexFilterArgs']]]] filters: Logs filter
         :param pulumi.Input[str] name: The name of the index.
         :param pulumi.Input[int] retention_days: The number of days before logs are deleted from this index.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
@@ -418,15 +424,16 @@
         """
         return pulumi.get(self, "daily_limit")
 
     @property
     @pulumi.getter(name="disableDailyLimit")
     def disable_daily_limit(self) -> pulumi.Output[bool]:
         """
-        If true, sets the daily*limit value to null and the index is not limited on a daily basis (any specified daily*limit value in the request is ignored). If false or omitted, the index's current daily_limit is maintained.
+        If true, sets the daily_limit value to null and the index is not limited on a daily basis (any specified daily_limit
+        value in the request is ignored). If false or omitted, the index's current daily_limit is maintained.
         """
         return pulumi.get(self, "disable_daily_limit")
 
     @property
     @pulumi.getter(name="exclusionFilters")
     def exclusion_filters(self) -> pulumi.Output[Optional[Sequence['outputs.LogsIndexExclusionFilter']]]:
         """
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/logs_index_order.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/logs_index_order.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,25 +13,27 @@
 @pulumi.input_type
 class LogsIndexOrderArgs:
     def __init__(__self__, *,
                  indexes: pulumi.Input[Sequence[pulumi.Input[str]]],
                  name: pulumi.Input[str]):
         """
         The set of arguments for constructing a LogsIndexOrder resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] indexes: The index resource list. Logs are tested against the query filter of each index one by one following the order of the list.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] indexes: The index resource list. Logs are tested against the query filter of each index one by one following the order of the
+               list.
         :param pulumi.Input[str] name: The unique name of the index order resource.
         """
         pulumi.set(__self__, "indexes", indexes)
         pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def indexes(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        The index resource list. Logs are tested against the query filter of each index one by one following the order of the list.
+        The index resource list. Logs are tested against the query filter of each index one by one following the order of the
+        list.
         """
         return pulumi.get(self, "indexes")
 
     @indexes.setter
     def indexes(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "indexes", value)
 
@@ -51,27 +53,29 @@
 @pulumi.input_type
 class _LogsIndexOrderState:
     def __init__(__self__, *,
                  indexes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering LogsIndexOrder resources.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] indexes: The index resource list. Logs are tested against the query filter of each index one by one following the order of the list.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] indexes: The index resource list. Logs are tested against the query filter of each index one by one following the order of the
+               list.
         :param pulumi.Input[str] name: The unique name of the index order resource.
         """
         if indexes is not None:
             pulumi.set(__self__, "indexes", indexes)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def indexes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The index resource list. Logs are tested against the query filter of each index one by one following the order of the list.
+        The index resource list. Logs are tested against the query filter of each index one by one following the order of the
+        list.
         """
         return pulumi.get(self, "indexes")
 
     @indexes.setter
     def indexes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "indexes", value)
 
@@ -116,15 +120,16 @@
 
         ```sh
          $ pulumi import datadog:index/logsIndexOrder:LogsIndexOrder name> <name>
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] indexes: The index resource list. Logs are tested against the query filter of each index one by one following the order of the list.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] indexes: The index resource list. Logs are tested against the query filter of each index one by one following the order of the
+               list.
         :param pulumi.Input[str] name: The unique name of the index order resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: LogsIndexOrderArgs,
@@ -201,30 +206,32 @@
         """
         Get an existing LogsIndexOrder resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] indexes: The index resource list. Logs are tested against the query filter of each index one by one following the order of the list.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] indexes: The index resource list. Logs are tested against the query filter of each index one by one following the order of the
+               list.
         :param pulumi.Input[str] name: The unique name of the index order resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _LogsIndexOrderState.__new__(_LogsIndexOrderState)
 
         __props__.__dict__["indexes"] = indexes
         __props__.__dict__["name"] = name
         return LogsIndexOrder(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def indexes(self) -> pulumi.Output[Sequence[str]]:
         """
-        The index resource list. Logs are tested against the query filter of each index one by one following the order of the list.
+        The index resource list. Logs are tested against the query filter of each index one by one following the order of the
+        list.
         """
         return pulumi.get(self, "indexes")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/logs_integration_pipeline.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/logs_integration_pipeline.py`

 * *Files identical despite different names*

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/logs_metric.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/logs_metric.py`

 * *Files identical despite different names*

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/logs_pipeline_order.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/logs_pipeline_order.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,25 +13,29 @@
 @pulumi.input_type
 class LogsPipelineOrderArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  pipelines: pulumi.Input[Sequence[pulumi.Input[str]]]):
         """
         The set of arguments for constructing a LogsPipelineOrder resource.
-        :param pulumi.Input[str] name: The name attribute in the resource `LogsPipelineOrder` needs to be unique. It's recommended to use the same value as the resource name. No related field is available in [Logs Pipeline API](https://docs.datadoghq.com/api/v1/logs-pipelines/#get-pipeline-order).
+        :param pulumi.Input[str] name: The name attribute in the resource `datadog_logs_pipeline_order` needs to be unique. It's recommended to use the same
+               value as the resource name. No related field is available in [Logs Pipeline
+               API](https://docs.datadoghq.com/api/v1/logs-pipelines/#get-pipeline-order).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] pipelines: The pipeline IDs list. The order of pipeline IDs in this attribute defines the overall pipeline order for logs.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "pipelines", pipelines)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
         """
-        The name attribute in the resource `LogsPipelineOrder` needs to be unique. It's recommended to use the same value as the resource name. No related field is available in [Logs Pipeline API](https://docs.datadoghq.com/api/v1/logs-pipelines/#get-pipeline-order).
+        The name attribute in the resource `datadog_logs_pipeline_order` needs to be unique. It's recommended to use the same
+        value as the resource name. No related field is available in [Logs Pipeline
+        API](https://docs.datadoghq.com/api/v1/logs-pipelines/#get-pipeline-order).
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
@@ -51,27 +55,31 @@
 @pulumi.input_type
 class _LogsPipelineOrderState:
     def __init__(__self__, *,
                  name: Optional[pulumi.Input[str]] = None,
                  pipelines: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering LogsPipelineOrder resources.
-        :param pulumi.Input[str] name: The name attribute in the resource `LogsPipelineOrder` needs to be unique. It's recommended to use the same value as the resource name. No related field is available in [Logs Pipeline API](https://docs.datadoghq.com/api/v1/logs-pipelines/#get-pipeline-order).
+        :param pulumi.Input[str] name: The name attribute in the resource `datadog_logs_pipeline_order` needs to be unique. It's recommended to use the same
+               value as the resource name. No related field is available in [Logs Pipeline
+               API](https://docs.datadoghq.com/api/v1/logs-pipelines/#get-pipeline-order).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] pipelines: The pipeline IDs list. The order of pipeline IDs in this attribute defines the overall pipeline order for logs.
         """
         if name is not None:
             pulumi.set(__self__, "name", name)
         if pipelines is not None:
             pulumi.set(__self__, "pipelines", pipelines)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The name attribute in the resource `LogsPipelineOrder` needs to be unique. It's recommended to use the same value as the resource name. No related field is available in [Logs Pipeline API](https://docs.datadoghq.com/api/v1/logs-pipelines/#get-pipeline-order).
+        The name attribute in the resource `datadog_logs_pipeline_order` needs to be unique. It's recommended to use the same
+        value as the resource name. No related field is available in [Logs Pipeline
+        API](https://docs.datadoghq.com/api/v1/logs-pipelines/#get-pipeline-order).
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -119,15 +127,17 @@
 
         ```sh
          $ pulumi import datadog:index/logsPipelineOrder:LogsPipelineOrder name> <name>
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] name: The name attribute in the resource `LogsPipelineOrder` needs to be unique. It's recommended to use the same value as the resource name. No related field is available in [Logs Pipeline API](https://docs.datadoghq.com/api/v1/logs-pipelines/#get-pipeline-order).
+        :param pulumi.Input[str] name: The name attribute in the resource `datadog_logs_pipeline_order` needs to be unique. It's recommended to use the same
+               value as the resource name. No related field is available in [Logs Pipeline
+               API](https://docs.datadoghq.com/api/v1/logs-pipelines/#get-pipeline-order).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] pipelines: The pipeline IDs list. The order of pipeline IDs in this attribute defines the overall pipeline order for logs.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: LogsPipelineOrderArgs,
@@ -207,30 +217,34 @@
         """
         Get an existing LogsPipelineOrder resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] name: The name attribute in the resource `LogsPipelineOrder` needs to be unique. It's recommended to use the same value as the resource name. No related field is available in [Logs Pipeline API](https://docs.datadoghq.com/api/v1/logs-pipelines/#get-pipeline-order).
+        :param pulumi.Input[str] name: The name attribute in the resource `datadog_logs_pipeline_order` needs to be unique. It's recommended to use the same
+               value as the resource name. No related field is available in [Logs Pipeline
+               API](https://docs.datadoghq.com/api/v1/logs-pipelines/#get-pipeline-order).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] pipelines: The pipeline IDs list. The order of pipeline IDs in this attribute defines the overall pipeline order for logs.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _LogsPipelineOrderState.__new__(_LogsPipelineOrderState)
 
         __props__.__dict__["name"] = name
         __props__.__dict__["pipelines"] = pipelines
         return LogsPipelineOrder(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        The name attribute in the resource `LogsPipelineOrder` needs to be unique. It's recommended to use the same value as the resource name. No related field is available in [Logs Pipeline API](https://docs.datadoghq.com/api/v1/logs-pipelines/#get-pipeline-order).
+        The name attribute in the resource `datadog_logs_pipeline_order` needs to be unique. It's recommended to use the same
+        value as the resource name. No related field is available in [Logs Pipeline
+        API](https://docs.datadoghq.com/api/v1/logs-pipelines/#get-pipeline-order).
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def pipelines(self) -> pulumi.Output[Sequence[str]]:
         """
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/metric_metadata.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/metric_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         """
         The set of arguments for constructing a MetricMetadata resource.
         :param pulumi.Input[str] metric: The name of the metric.
         :param pulumi.Input[str] description: A description of the metric.
         :param pulumi.Input[str] per_unit: Per unit of the metric such as `second` in `bytes per second`.
         :param pulumi.Input[str] short_name: A short name of the metric.
         :param pulumi.Input[int] statsd_interval: If applicable, statsd flush interval in seconds for the metric.
-        :param pulumi.Input[str] type: Type of the metric.
+        :param pulumi.Input[str] type: Metric type such as `gauge` or `rate`.
         :param pulumi.Input[str] unit: Primary unit of the metric such as `byte` or `operation`.
         """
         pulumi.set(__self__, "metric", metric)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if per_unit is not None:
             pulumi.set(__self__, "per_unit", per_unit)
@@ -104,15 +104,15 @@
     def statsd_interval(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "statsd_interval", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        Type of the metric.
+        Metric type such as `gauge` or `rate`.
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -142,15 +142,15 @@
         """
         Input properties used for looking up and filtering MetricMetadata resources.
         :param pulumi.Input[str] description: A description of the metric.
         :param pulumi.Input[str] metric: The name of the metric.
         :param pulumi.Input[str] per_unit: Per unit of the metric such as `second` in `bytes per second`.
         :param pulumi.Input[str] short_name: A short name of the metric.
         :param pulumi.Input[int] statsd_interval: If applicable, statsd flush interval in seconds for the metric.
-        :param pulumi.Input[str] type: Type of the metric.
+        :param pulumi.Input[str] type: Metric type such as `gauge` or `rate`.
         :param pulumi.Input[str] unit: Primary unit of the metric such as `byte` or `operation`.
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if metric is not None:
             pulumi.set(__self__, "metric", metric)
         if per_unit is not None:
@@ -224,15 +224,15 @@
     def statsd_interval(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "statsd_interval", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        Type of the metric.
+        Metric type such as `gauge` or `rate`.
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -283,15 +283,15 @@
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A description of the metric.
         :param pulumi.Input[str] metric: The name of the metric.
         :param pulumi.Input[str] per_unit: Per unit of the metric such as `second` in `bytes per second`.
         :param pulumi.Input[str] short_name: A short name of the metric.
         :param pulumi.Input[int] statsd_interval: If applicable, statsd flush interval in seconds for the metric.
-        :param pulumi.Input[str] type: Type of the metric.
+        :param pulumi.Input[str] type: Metric type such as `gauge` or `rate`.
         :param pulumi.Input[str] unit: Primary unit of the metric such as `byte` or `operation`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: MetricMetadataArgs,
@@ -382,15 +382,15 @@
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A description of the metric.
         :param pulumi.Input[str] metric: The name of the metric.
         :param pulumi.Input[str] per_unit: Per unit of the metric such as `second` in `bytes per second`.
         :param pulumi.Input[str] short_name: A short name of the metric.
         :param pulumi.Input[int] statsd_interval: If applicable, statsd flush interval in seconds for the metric.
-        :param pulumi.Input[str] type: Type of the metric.
+        :param pulumi.Input[str] type: Metric type such as `gauge` or `rate`.
         :param pulumi.Input[str] unit: Primary unit of the metric such as `byte` or `operation`.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _MetricMetadataState.__new__(_MetricMetadataState)
 
         __props__.__dict__["description"] = description
@@ -442,15 +442,15 @@
         """
         return pulumi.get(self, "statsd_interval")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[Optional[str]]:
         """
-        Type of the metric.
+        Metric type such as `gauge` or `rate`.
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def unit(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/metric_tag_configuration.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/metric_tag_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,21 @@
                  metric_type: pulumi.Input[str],
                  tags: pulumi.Input[Sequence[pulumi.Input[str]]],
                  aggregations: Optional[pulumi.Input[Sequence[pulumi.Input['MetricTagConfigurationAggregationArgs']]]] = None,
                  include_percentiles: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a MetricTagConfiguration resource.
         :param pulumi.Input[str] metric_name: The metric name for this resource.
-        :param pulumi.Input[str] metric_type: The metric's type. This field can't be updated after creation. Valid values are `gauge`, `count`, `rate`, `distribution`.
+        :param pulumi.Input[str] metric_type: The metric's type. This field can't be updated after creation.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tag keys that will be queryable for your metric.
-        :param pulumi.Input[Sequence[pulumi.Input['MetricTagConfigurationAggregationArgs']]] aggregations: A list of queryable aggregation combinations for a count, rate, or gauge metric. By default, count and rate metrics require the (time: sum, space: sum) aggregation and gauge metrics require the (time: avg, space: avg) aggregation. Can only be applied to metrics that have a `metric_type` of count, rate, or gauge.
-        :param pulumi.Input[bool] include_percentiles: Toggle to include/exclude percentiles for a distribution metric. Defaults to false. Can only be applied to metrics that have a `metric_type` of distribution.
+        :param pulumi.Input[Sequence[pulumi.Input['MetricTagConfigurationAggregationArgs']]] aggregations: A list of queryable aggregation combinations for a count, rate, or gauge metric. By default, count and rate metrics
+               require the (time: sum, space: sum) aggregation and gauge metrics require the (time: avg, space: avg) aggregation. Can
+               only be applied to metrics that have a `metric_type` of count, rate, or gauge.
+        :param pulumi.Input[bool] include_percentiles: Toggle to include/exclude percentiles for a distribution metric. Defaults to false. Can only be applied to metrics that
+               have a `metric_type` of distribution.
         """
         pulumi.set(__self__, "metric_name", metric_name)
         pulumi.set(__self__, "metric_type", metric_type)
         pulumi.set(__self__, "tags", tags)
         if aggregations is not None:
             pulumi.set(__self__, "aggregations", aggregations)
         if include_percentiles is not None:
@@ -48,15 +51,15 @@
     def metric_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "metric_name", value)
 
     @property
     @pulumi.getter(name="metricType")
     def metric_type(self) -> pulumi.Input[str]:
         """
-        The metric's type. This field can't be updated after creation. Valid values are `gauge`, `count`, `rate`, `distribution`.
+        The metric's type. This field can't be updated after creation.
         """
         return pulumi.get(self, "metric_type")
 
     @metric_type.setter
     def metric_type(self, value: pulumi.Input[str]):
         pulumi.set(self, "metric_type", value)
 
@@ -72,27 +75,30 @@
     def tags(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "tags", value)
 
     @property
     @pulumi.getter
     def aggregations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['MetricTagConfigurationAggregationArgs']]]]:
         """
-        A list of queryable aggregation combinations for a count, rate, or gauge metric. By default, count and rate metrics require the (time: sum, space: sum) aggregation and gauge metrics require the (time: avg, space: avg) aggregation. Can only be applied to metrics that have a `metric_type` of count, rate, or gauge.
+        A list of queryable aggregation combinations for a count, rate, or gauge metric. By default, count and rate metrics
+        require the (time: sum, space: sum) aggregation and gauge metrics require the (time: avg, space: avg) aggregation. Can
+        only be applied to metrics that have a `metric_type` of count, rate, or gauge.
         """
         return pulumi.get(self, "aggregations")
 
     @aggregations.setter
     def aggregations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['MetricTagConfigurationAggregationArgs']]]]):
         pulumi.set(self, "aggregations", value)
 
     @property
     @pulumi.getter(name="includePercentiles")
     def include_percentiles(self) -> Optional[pulumi.Input[bool]]:
         """
-        Toggle to include/exclude percentiles for a distribution metric. Defaults to false. Can only be applied to metrics that have a `metric_type` of distribution.
+        Toggle to include/exclude percentiles for a distribution metric. Defaults to false. Can only be applied to metrics that
+        have a `metric_type` of distribution.
         """
         return pulumi.get(self, "include_percentiles")
 
     @include_percentiles.setter
     def include_percentiles(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "include_percentiles", value)
 
@@ -103,18 +109,21 @@
                  aggregations: Optional[pulumi.Input[Sequence[pulumi.Input['MetricTagConfigurationAggregationArgs']]]] = None,
                  include_percentiles: Optional[pulumi.Input[bool]] = None,
                  metric_name: Optional[pulumi.Input[str]] = None,
                  metric_type: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering MetricTagConfiguration resources.
-        :param pulumi.Input[Sequence[pulumi.Input['MetricTagConfigurationAggregationArgs']]] aggregations: A list of queryable aggregation combinations for a count, rate, or gauge metric. By default, count and rate metrics require the (time: sum, space: sum) aggregation and gauge metrics require the (time: avg, space: avg) aggregation. Can only be applied to metrics that have a `metric_type` of count, rate, or gauge.
-        :param pulumi.Input[bool] include_percentiles: Toggle to include/exclude percentiles for a distribution metric. Defaults to false. Can only be applied to metrics that have a `metric_type` of distribution.
+        :param pulumi.Input[Sequence[pulumi.Input['MetricTagConfigurationAggregationArgs']]] aggregations: A list of queryable aggregation combinations for a count, rate, or gauge metric. By default, count and rate metrics
+               require the (time: sum, space: sum) aggregation and gauge metrics require the (time: avg, space: avg) aggregation. Can
+               only be applied to metrics that have a `metric_type` of count, rate, or gauge.
+        :param pulumi.Input[bool] include_percentiles: Toggle to include/exclude percentiles for a distribution metric. Defaults to false. Can only be applied to metrics that
+               have a `metric_type` of distribution.
         :param pulumi.Input[str] metric_name: The metric name for this resource.
-        :param pulumi.Input[str] metric_type: The metric's type. This field can't be updated after creation. Valid values are `gauge`, `count`, `rate`, `distribution`.
+        :param pulumi.Input[str] metric_type: The metric's type. This field can't be updated after creation.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tag keys that will be queryable for your metric.
         """
         if aggregations is not None:
             pulumi.set(__self__, "aggregations", aggregations)
         if include_percentiles is not None:
             pulumi.set(__self__, "include_percentiles", include_percentiles)
         if metric_name is not None:
@@ -124,27 +133,30 @@
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def aggregations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['MetricTagConfigurationAggregationArgs']]]]:
         """
-        A list of queryable aggregation combinations for a count, rate, or gauge metric. By default, count and rate metrics require the (time: sum, space: sum) aggregation and gauge metrics require the (time: avg, space: avg) aggregation. Can only be applied to metrics that have a `metric_type` of count, rate, or gauge.
+        A list of queryable aggregation combinations for a count, rate, or gauge metric. By default, count and rate metrics
+        require the (time: sum, space: sum) aggregation and gauge metrics require the (time: avg, space: avg) aggregation. Can
+        only be applied to metrics that have a `metric_type` of count, rate, or gauge.
         """
         return pulumi.get(self, "aggregations")
 
     @aggregations.setter
     def aggregations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['MetricTagConfigurationAggregationArgs']]]]):
         pulumi.set(self, "aggregations", value)
 
     @property
     @pulumi.getter(name="includePercentiles")
     def include_percentiles(self) -> Optional[pulumi.Input[bool]]:
         """
-        Toggle to include/exclude percentiles for a distribution metric. Defaults to false. Can only be applied to metrics that have a `metric_type` of distribution.
+        Toggle to include/exclude percentiles for a distribution metric. Defaults to false. Can only be applied to metrics that
+        have a `metric_type` of distribution.
         """
         return pulumi.get(self, "include_percentiles")
 
     @include_percentiles.setter
     def include_percentiles(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "include_percentiles", value)
 
@@ -160,15 +172,15 @@
     def metric_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "metric_name", value)
 
     @property
     @pulumi.getter(name="metricType")
     def metric_type(self) -> Optional[pulumi.Input[str]]:
         """
-        The metric's type. This field can't be updated after creation. Valid values are `gauge`, `count`, `rate`, `distribution`.
+        The metric's type. This field can't be updated after creation.
         """
         return pulumi.get(self, "metric_type")
 
     @metric_type.setter
     def metric_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "metric_type", value)
 
@@ -232,18 +244,21 @@
                 "sport",
                 "datacenter",
             ])
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['MetricTagConfigurationAggregationArgs']]]] aggregations: A list of queryable aggregation combinations for a count, rate, or gauge metric. By default, count and rate metrics require the (time: sum, space: sum) aggregation and gauge metrics require the (time: avg, space: avg) aggregation. Can only be applied to metrics that have a `metric_type` of count, rate, or gauge.
-        :param pulumi.Input[bool] include_percentiles: Toggle to include/exclude percentiles for a distribution metric. Defaults to false. Can only be applied to metrics that have a `metric_type` of distribution.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['MetricTagConfigurationAggregationArgs']]]] aggregations: A list of queryable aggregation combinations for a count, rate, or gauge metric. By default, count and rate metrics
+               require the (time: sum, space: sum) aggregation and gauge metrics require the (time: avg, space: avg) aggregation. Can
+               only be applied to metrics that have a `metric_type` of count, rate, or gauge.
+        :param pulumi.Input[bool] include_percentiles: Toggle to include/exclude percentiles for a distribution metric. Defaults to false. Can only be applied to metrics that
+               have a `metric_type` of distribution.
         :param pulumi.Input[str] metric_name: The metric name for this resource.
-        :param pulumi.Input[str] metric_type: The metric's type. This field can't be updated after creation. Valid values are `gauge`, `count`, `rate`, `distribution`.
+        :param pulumi.Input[str] metric_type: The metric's type. This field can't be updated after creation.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tag keys that will be queryable for your metric.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: MetricTagConfigurationArgs,
@@ -347,18 +362,21 @@
         """
         Get an existing MetricTagConfiguration resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['MetricTagConfigurationAggregationArgs']]]] aggregations: A list of queryable aggregation combinations for a count, rate, or gauge metric. By default, count and rate metrics require the (time: sum, space: sum) aggregation and gauge metrics require the (time: avg, space: avg) aggregation. Can only be applied to metrics that have a `metric_type` of count, rate, or gauge.
-        :param pulumi.Input[bool] include_percentiles: Toggle to include/exclude percentiles for a distribution metric. Defaults to false. Can only be applied to metrics that have a `metric_type` of distribution.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['MetricTagConfigurationAggregationArgs']]]] aggregations: A list of queryable aggregation combinations for a count, rate, or gauge metric. By default, count and rate metrics
+               require the (time: sum, space: sum) aggregation and gauge metrics require the (time: avg, space: avg) aggregation. Can
+               only be applied to metrics that have a `metric_type` of count, rate, or gauge.
+        :param pulumi.Input[bool] include_percentiles: Toggle to include/exclude percentiles for a distribution metric. Defaults to false. Can only be applied to metrics that
+               have a `metric_type` of distribution.
         :param pulumi.Input[str] metric_name: The metric name for this resource.
-        :param pulumi.Input[str] metric_type: The metric's type. This field can't be updated after creation. Valid values are `gauge`, `count`, `rate`, `distribution`.
+        :param pulumi.Input[str] metric_type: The metric's type. This field can't be updated after creation.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tag keys that will be queryable for your metric.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _MetricTagConfigurationState.__new__(_MetricTagConfigurationState)
 
         __props__.__dict__["aggregations"] = aggregations
@@ -368,23 +386,26 @@
         __props__.__dict__["tags"] = tags
         return MetricTagConfiguration(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def aggregations(self) -> pulumi.Output[Sequence['outputs.MetricTagConfigurationAggregation']]:
         """
-        A list of queryable aggregation combinations for a count, rate, or gauge metric. By default, count and rate metrics require the (time: sum, space: sum) aggregation and gauge metrics require the (time: avg, space: avg) aggregation. Can only be applied to metrics that have a `metric_type` of count, rate, or gauge.
+        A list of queryable aggregation combinations for a count, rate, or gauge metric. By default, count and rate metrics
+        require the (time: sum, space: sum) aggregation and gauge metrics require the (time: avg, space: avg) aggregation. Can
+        only be applied to metrics that have a `metric_type` of count, rate, or gauge.
         """
         return pulumi.get(self, "aggregations")
 
     @property
     @pulumi.getter(name="includePercentiles")
     def include_percentiles(self) -> pulumi.Output[Optional[bool]]:
         """
-        Toggle to include/exclude percentiles for a distribution metric. Defaults to false. Can only be applied to metrics that have a `metric_type` of distribution.
+        Toggle to include/exclude percentiles for a distribution metric. Defaults to false. Can only be applied to metrics that
+        have a `metric_type` of distribution.
         """
         return pulumi.get(self, "include_percentiles")
 
     @property
     @pulumi.getter(name="metricName")
     def metric_name(self) -> pulumi.Output[str]:
         """
@@ -392,15 +413,15 @@
         """
         return pulumi.get(self, "metric_name")
 
     @property
     @pulumi.getter(name="metricType")
     def metric_type(self) -> pulumi.Output[str]:
         """
-        The metric's type. This field can't be updated after creation. Valid values are `gauge`, `count`, `rate`, `distribution`.
+        The metric's type. This field can't be updated after creation.
         """
         return pulumi.get(self, "metric_type")
 
     @property
     @pulumi.getter
     def tags(self) -> pulumi.Output[Sequence[str]]:
         """
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/monitor.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/monitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,16 @@
                  require_full_window: Optional[pulumi.Input[bool]] = None,
                  restricted_roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  timeout_h: Optional[pulumi.Input[int]] = None,
                  validate: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Monitor resource.
-        :param pulumi.Input[str] message: A message to include with notifications for this monitor.
+        :param pulumi.Input[str] message: A message to include with notifications for this monitor. Email notifications can be sent to specific users by using the
+               same `@username` notation as events.
         :param pulumi.Input[str] name: Name of Datadog monitor.
         :param pulumi.Input[str] query: The monitor query to notify on. Note this is not the same query you see in the UI and the syntax is different depending
                on the monitor type, please see the [API Reference](https://docs.datadoghq.com/api/v1/monitors/#create-a-monitor) for
                details. `terraform plan` will validate query contents unless `validate` is set to `false`. **Note:** APM latency data
                is now available as Distribution Metrics. Existing monitors have been migrated automatically but all terraformed
                monitors can still use the existing metrics. We strongly recommend updating monitor definitions to query the new
                metrics. To learn more, or to see examples of how to update your terraform definitions to utilize the new distribution
@@ -87,17 +88,22 @@
         :param pulumi.Input[int] renotify_interval: The number of minutes after the last notification before a monitor will re-notify on the current status. It will only
                re-notify if it's not resolved.
         :param pulumi.Input[int] renotify_occurrences: The number of re-notification messages that should be sent on the current status.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] renotify_statuses: The types of statuses for which re-notification messages should be sent.
         :param pulumi.Input[bool] require_full_window: A boolean indicating whether this monitor needs a full window of data before it's evaluated. We highly recommend you set
                this to `false` for sparse metrics, otherwise some evaluations will be skipped. Default: `true` for `on average`, `at
                all times` and `in total` aggregation. `false` otherwise.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] restricted_roles: A list of unique role identifiers to define which roles are allowed to edit the monitor. Editing a monitor includes any
+               updates to the monitor configuration, monitor deletion, and muting of the monitor for any amount of time. Roles unique
+               identifiers can be pulled from the [Roles API](https://docs.datadoghq.com/api/latest/roles/#list-roles) in the `data.id`
+               field.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to associate with your monitor. This can help you categorize and filter monitors in the manage monitors
                page of the UI. Note: it's not currently possible to filter by these tags when querying via the API
-        :param pulumi.Input[int] timeout_h: The number of hours of the monitor not reporting data before it will automatically resolve from a triggered state.
+        :param pulumi.Input[int] timeout_h: The number of hours of the monitor not reporting data before it automatically resolves from a triggered state. The
+               minimum allowed value is 0 hours. The maximum allowed value is 24 hours.
         :param pulumi.Input[bool] validate: If set to `false`, skip the validation call done during plan.
         """
         pulumi.set(__self__, "message", message)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "query", query)
         pulumi.set(__self__, "type", type)
         if enable_logs_sample is not None:
@@ -109,14 +115,17 @@
         if force_delete is not None:
             pulumi.set(__self__, "force_delete", force_delete)
         if groupby_simple_monitor is not None:
             pulumi.set(__self__, "groupby_simple_monitor", groupby_simple_monitor)
         if include_tags is not None:
             pulumi.set(__self__, "include_tags", include_tags)
         if locked is not None:
+            warnings.warn("""Use `restricted_roles`.""", DeprecationWarning)
+            pulumi.log.warn("""locked is deprecated: Use `restricted_roles`.""")
+        if locked is not None:
             pulumi.set(__self__, "locked", locked)
         if monitor_threshold_windows is not None:
             pulumi.set(__self__, "monitor_threshold_windows", monitor_threshold_windows)
         if monitor_thresholds is not None:
             pulumi.set(__self__, "monitor_thresholds", monitor_thresholds)
         if new_group_delay is not None:
             pulumi.set(__self__, "new_group_delay", new_group_delay)
@@ -150,15 +159,16 @@
         if validate is not None:
             pulumi.set(__self__, "validate", validate)
 
     @property
     @pulumi.getter
     def message(self) -> pulumi.Input[str]:
         """
-        A message to include with notifications for this monitor.
+        A message to include with notifications for this monitor. Email notifications can be sent to specific users by using the
+        same `@username` notation as events.
         """
         return pulumi.get(self, "message")
 
     @message.setter
     def message(self, value: pulumi.Input[str]):
         pulumi.set(self, "message", value)
 
@@ -449,14 +459,20 @@
     @require_full_window.setter
     def require_full_window(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "require_full_window", value)
 
     @property
     @pulumi.getter(name="restrictedRoles")
     def restricted_roles(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        A list of unique role identifiers to define which roles are allowed to edit the monitor. Editing a monitor includes any
+        updates to the monitor configuration, monitor deletion, and muting of the monitor for any amount of time. Roles unique
+        identifiers can be pulled from the [Roles API](https://docs.datadoghq.com/api/latest/roles/#list-roles) in the `data.id`
+        field.
+        """
         return pulumi.get(self, "restricted_roles")
 
     @restricted_roles.setter
     def restricted_roles(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "restricted_roles", value)
 
     @property
@@ -472,15 +488,16 @@
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
     @property
     @pulumi.getter(name="timeoutH")
     def timeout_h(self) -> Optional[pulumi.Input[int]]:
         """
-        The number of hours of the monitor not reporting data before it will automatically resolve from a triggered state.
+        The number of hours of the monitor not reporting data before it automatically resolves from a triggered state. The
+        minimum allowed value is 0 hours. The maximum allowed value is 24 hours.
         """
         return pulumi.get(self, "timeout_h")
 
     @timeout_h.setter
     def timeout_h(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "timeout_h", value)
 
@@ -539,15 +556,16 @@
         :param pulumi.Input[bool] force_delete: A boolean indicating whether this monitor can be deleted even if it’s referenced by other resources (e.g. SLO,
                composite monitor).
         :param pulumi.Input[bool] groupby_simple_monitor: Whether or not to trigger one alert if any source breaches a threshold. This is only used by log monitors. Defaults to
                `false`.
         :param pulumi.Input[bool] include_tags: A boolean indicating whether notifications from this monitor automatically insert its triggering tags into the title.
                Defaults to `true`.
         :param pulumi.Input[bool] locked: A boolean indicating whether changes to this monitor should be restricted to the creator or admins. Defaults to `false`.
-        :param pulumi.Input[str] message: A message to include with notifications for this monitor.
+        :param pulumi.Input[str] message: A message to include with notifications for this monitor. Email notifications can be sent to specific users by using the
+               same `@username` notation as events.
         :param pulumi.Input['MonitorMonitorThresholdWindowsArgs'] monitor_threshold_windows: A mapping containing `recovery_window` and `trigger_window` values, e.g. `last_15m` . Can only be used for, and are
                required for, anomaly monitors.
         :param pulumi.Input['MonitorMonitorThresholdsArgs'] monitor_thresholds: Alert thresholds of the monitor.
         :param pulumi.Input[str] name: Name of Datadog monitor.
         :param pulumi.Input[int] new_group_delay: The time (in seconds) to skip evaluations for new groups. `new_group_delay` overrides `new_host_delay` if it is set to a
                nonzero value.
         :param pulumi.Input[int] new_host_delay: **Deprecated**. See `new_group_delay`. Time (in seconds) to allow a host to boot and applications to fully start before
@@ -569,17 +587,22 @@
         :param pulumi.Input[int] renotify_interval: The number of minutes after the last notification before a monitor will re-notify on the current status. It will only
                re-notify if it's not resolved.
         :param pulumi.Input[int] renotify_occurrences: The number of re-notification messages that should be sent on the current status.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] renotify_statuses: The types of statuses for which re-notification messages should be sent.
         :param pulumi.Input[bool] require_full_window: A boolean indicating whether this monitor needs a full window of data before it's evaluated. We highly recommend you set
                this to `false` for sparse metrics, otherwise some evaluations will be skipped. Default: `true` for `on average`, `at
                all times` and `in total` aggregation. `false` otherwise.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] restricted_roles: A list of unique role identifiers to define which roles are allowed to edit the monitor. Editing a monitor includes any
+               updates to the monitor configuration, monitor deletion, and muting of the monitor for any amount of time. Roles unique
+               identifiers can be pulled from the [Roles API](https://docs.datadoghq.com/api/latest/roles/#list-roles) in the `data.id`
+               field.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to associate with your monitor. This can help you categorize and filter monitors in the manage monitors
                page of the UI. Note: it's not currently possible to filter by these tags when querying via the API
-        :param pulumi.Input[int] timeout_h: The number of hours of the monitor not reporting data before it will automatically resolve from a triggered state.
+        :param pulumi.Input[int] timeout_h: The number of hours of the monitor not reporting data before it automatically resolves from a triggered state. The
+               minimum allowed value is 0 hours. The maximum allowed value is 24 hours.
         :param pulumi.Input[str] type: The type of the monitor. The mapping from these types to the types found in the Datadog Web UI can be found in the
                Datadog API [documentation page](https://docs.datadoghq.com/api/v1/monitors/#create-a-monitor). Note: The monitor type
                cannot be changed after a monitor is created.
         :param pulumi.Input[bool] validate: If set to `false`, skip the validation call done during plan.
         """
         if enable_logs_sample is not None:
             pulumi.set(__self__, "enable_logs_sample", enable_logs_sample)
@@ -590,14 +613,17 @@
         if force_delete is not None:
             pulumi.set(__self__, "force_delete", force_delete)
         if groupby_simple_monitor is not None:
             pulumi.set(__self__, "groupby_simple_monitor", groupby_simple_monitor)
         if include_tags is not None:
             pulumi.set(__self__, "include_tags", include_tags)
         if locked is not None:
+            warnings.warn("""Use `restricted_roles`.""", DeprecationWarning)
+            pulumi.log.warn("""locked is deprecated: Use `restricted_roles`.""")
+        if locked is not None:
             pulumi.set(__self__, "locked", locked)
         if message is not None:
             pulumi.set(__self__, "message", message)
         if monitor_threshold_windows is not None:
             pulumi.set(__self__, "monitor_threshold_windows", monitor_threshold_windows)
         if monitor_thresholds is not None:
             pulumi.set(__self__, "monitor_thresholds", monitor_thresholds)
@@ -730,15 +756,16 @@
     def locked(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "locked", value)
 
     @property
     @pulumi.getter
     def message(self) -> Optional[pulumi.Input[str]]:
         """
-        A message to include with notifications for this monitor.
+        A message to include with notifications for this monitor. Email notifications can be sent to specific users by using the
+        same `@username` notation as events.
         """
         return pulumi.get(self, "message")
 
     @message.setter
     def message(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "message", value)
 
@@ -924,14 +951,20 @@
     @require_full_window.setter
     def require_full_window(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "require_full_window", value)
 
     @property
     @pulumi.getter(name="restrictedRoles")
     def restricted_roles(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        A list of unique role identifiers to define which roles are allowed to edit the monitor. Editing a monitor includes any
+        updates to the monitor configuration, monitor deletion, and muting of the monitor for any amount of time. Roles unique
+        identifiers can be pulled from the [Roles API](https://docs.datadoghq.com/api/latest/roles/#list-roles) in the `data.id`
+        field.
+        """
         return pulumi.get(self, "restricted_roles")
 
     @restricted_roles.setter
     def restricted_roles(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "restricted_roles", value)
 
     @property
@@ -947,15 +980,16 @@
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
     @property
     @pulumi.getter(name="timeoutH")
     def timeout_h(self) -> Optional[pulumi.Input[int]]:
         """
-        The number of hours of the monitor not reporting data before it will automatically resolve from a triggered state.
+        The number of hours of the monitor not reporting data before it automatically resolves from a triggered state. The
+        minimum allowed value is 0 hours. The maximum allowed value is 24 hours.
         """
         return pulumi.get(self, "timeout_h")
 
     @timeout_h.setter
     def timeout_h(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "timeout_h", value)
 
@@ -1024,33 +1058,27 @@
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_datadog as datadog
 
-        # Create a new Datadog monitor
         foo = datadog.Monitor("foo",
             escalation_message="Escalation message @pagerduty",
             include_tags=True,
             message="Monitor triggered. Notify: @hipchat-channel",
             monitor_thresholds=datadog.MonitorMonitorThresholdsArgs(
                 critical="4",
-                critical_recovery="3",
                 warning="2",
-                warning_recovery="1",
             ),
             name="Name for monitor foo",
-            notify_audit=False,
-            notify_no_data=False,
             query="avg(last_1h):avg:aws.ec2.cpu{environment:foo,host:foo} by {host} > 4",
-            renotify_interval=60,
             tags=[
                 "foo:bar",
-                "baz",
+                "team:fooBar",
             ],
             type="metric alert")
         ```
 
         ## Import
 
         ```sh
@@ -1069,15 +1097,16 @@
         :param pulumi.Input[bool] force_delete: A boolean indicating whether this monitor can be deleted even if it’s referenced by other resources (e.g. SLO,
                composite monitor).
         :param pulumi.Input[bool] groupby_simple_monitor: Whether or not to trigger one alert if any source breaches a threshold. This is only used by log monitors. Defaults to
                `false`.
         :param pulumi.Input[bool] include_tags: A boolean indicating whether notifications from this monitor automatically insert its triggering tags into the title.
                Defaults to `true`.
         :param pulumi.Input[bool] locked: A boolean indicating whether changes to this monitor should be restricted to the creator or admins. Defaults to `false`.
-        :param pulumi.Input[str] message: A message to include with notifications for this monitor.
+        :param pulumi.Input[str] message: A message to include with notifications for this monitor. Email notifications can be sent to specific users by using the
+               same `@username` notation as events.
         :param pulumi.Input[pulumi.InputType['MonitorMonitorThresholdWindowsArgs']] monitor_threshold_windows: A mapping containing `recovery_window` and `trigger_window` values, e.g. `last_15m` . Can only be used for, and are
                required for, anomaly monitors.
         :param pulumi.Input[pulumi.InputType['MonitorMonitorThresholdsArgs']] monitor_thresholds: Alert thresholds of the monitor.
         :param pulumi.Input[str] name: Name of Datadog monitor.
         :param pulumi.Input[int] new_group_delay: The time (in seconds) to skip evaluations for new groups. `new_group_delay` overrides `new_host_delay` if it is set to a
                nonzero value.
         :param pulumi.Input[int] new_host_delay: **Deprecated**. See `new_group_delay`. Time (in seconds) to allow a host to boot and applications to fully start before
@@ -1099,17 +1128,22 @@
         :param pulumi.Input[int] renotify_interval: The number of minutes after the last notification before a monitor will re-notify on the current status. It will only
                re-notify if it's not resolved.
         :param pulumi.Input[int] renotify_occurrences: The number of re-notification messages that should be sent on the current status.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] renotify_statuses: The types of statuses for which re-notification messages should be sent.
         :param pulumi.Input[bool] require_full_window: A boolean indicating whether this monitor needs a full window of data before it's evaluated. We highly recommend you set
                this to `false` for sparse metrics, otherwise some evaluations will be skipped. Default: `true` for `on average`, `at
                all times` and `in total` aggregation. `false` otherwise.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] restricted_roles: A list of unique role identifiers to define which roles are allowed to edit the monitor. Editing a monitor includes any
+               updates to the monitor configuration, monitor deletion, and muting of the monitor for any amount of time. Roles unique
+               identifiers can be pulled from the [Roles API](https://docs.datadoghq.com/api/latest/roles/#list-roles) in the `data.id`
+               field.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to associate with your monitor. This can help you categorize and filter monitors in the manage monitors
                page of the UI. Note: it's not currently possible to filter by these tags when querying via the API
-        :param pulumi.Input[int] timeout_h: The number of hours of the monitor not reporting data before it will automatically resolve from a triggered state.
+        :param pulumi.Input[int] timeout_h: The number of hours of the monitor not reporting data before it automatically resolves from a triggered state. The
+               minimum allowed value is 0 hours. The maximum allowed value is 24 hours.
         :param pulumi.Input[str] type: The type of the monitor. The mapping from these types to the types found in the Datadog Web UI can be found in the
                Datadog API [documentation page](https://docs.datadoghq.com/api/v1/monitors/#create-a-monitor). Note: The monitor type
                cannot be changed after a monitor is created.
         :param pulumi.Input[bool] validate: If set to `false`, skip the validation call done during plan.
         """
         ...
     @overload
@@ -1122,33 +1156,27 @@
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_datadog as datadog
 
-        # Create a new Datadog monitor
         foo = datadog.Monitor("foo",
             escalation_message="Escalation message @pagerduty",
             include_tags=True,
             message="Monitor triggered. Notify: @hipchat-channel",
             monitor_thresholds=datadog.MonitorMonitorThresholdsArgs(
                 critical="4",
-                critical_recovery="3",
                 warning="2",
-                warning_recovery="1",
             ),
             name="Name for monitor foo",
-            notify_audit=False,
-            notify_no_data=False,
             query="avg(last_1h):avg:aws.ec2.cpu{environment:foo,host:foo} by {host} > 4",
-            renotify_interval=60,
             tags=[
                 "foo:bar",
-                "baz",
+                "team:fooBar",
             ],
             type="metric alert")
         ```
 
         ## Import
 
         ```sh
@@ -1211,14 +1239,17 @@
 
             __props__.__dict__["enable_logs_sample"] = enable_logs_sample
             __props__.__dict__["escalation_message"] = escalation_message
             __props__.__dict__["evaluation_delay"] = evaluation_delay
             __props__.__dict__["force_delete"] = force_delete
             __props__.__dict__["groupby_simple_monitor"] = groupby_simple_monitor
             __props__.__dict__["include_tags"] = include_tags
+            if locked is not None and not opts.urn:
+                warnings.warn("""Use `restricted_roles`.""", DeprecationWarning)
+                pulumi.log.warn("""locked is deprecated: Use `restricted_roles`.""")
             __props__.__dict__["locked"] = locked
             if message is None and not opts.urn:
                 raise TypeError("Missing required property 'message'")
             __props__.__dict__["message"] = message
             __props__.__dict__["monitor_threshold_windows"] = monitor_threshold_windows
             __props__.__dict__["monitor_thresholds"] = monitor_thresholds
             if name is None and not opts.urn:
@@ -1301,15 +1332,16 @@
         :param pulumi.Input[bool] force_delete: A boolean indicating whether this monitor can be deleted even if it’s referenced by other resources (e.g. SLO,
                composite monitor).
         :param pulumi.Input[bool] groupby_simple_monitor: Whether or not to trigger one alert if any source breaches a threshold. This is only used by log monitors. Defaults to
                `false`.
         :param pulumi.Input[bool] include_tags: A boolean indicating whether notifications from this monitor automatically insert its triggering tags into the title.
                Defaults to `true`.
         :param pulumi.Input[bool] locked: A boolean indicating whether changes to this monitor should be restricted to the creator or admins. Defaults to `false`.
-        :param pulumi.Input[str] message: A message to include with notifications for this monitor.
+        :param pulumi.Input[str] message: A message to include with notifications for this monitor. Email notifications can be sent to specific users by using the
+               same `@username` notation as events.
         :param pulumi.Input[pulumi.InputType['MonitorMonitorThresholdWindowsArgs']] monitor_threshold_windows: A mapping containing `recovery_window` and `trigger_window` values, e.g. `last_15m` . Can only be used for, and are
                required for, anomaly monitors.
         :param pulumi.Input[pulumi.InputType['MonitorMonitorThresholdsArgs']] monitor_thresholds: Alert thresholds of the monitor.
         :param pulumi.Input[str] name: Name of Datadog monitor.
         :param pulumi.Input[int] new_group_delay: The time (in seconds) to skip evaluations for new groups. `new_group_delay` overrides `new_host_delay` if it is set to a
                nonzero value.
         :param pulumi.Input[int] new_host_delay: **Deprecated**. See `new_group_delay`. Time (in seconds) to allow a host to boot and applications to fully start before
@@ -1331,17 +1363,22 @@
         :param pulumi.Input[int] renotify_interval: The number of minutes after the last notification before a monitor will re-notify on the current status. It will only
                re-notify if it's not resolved.
         :param pulumi.Input[int] renotify_occurrences: The number of re-notification messages that should be sent on the current status.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] renotify_statuses: The types of statuses for which re-notification messages should be sent.
         :param pulumi.Input[bool] require_full_window: A boolean indicating whether this monitor needs a full window of data before it's evaluated. We highly recommend you set
                this to `false` for sparse metrics, otherwise some evaluations will be skipped. Default: `true` for `on average`, `at
                all times` and `in total` aggregation. `false` otherwise.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] restricted_roles: A list of unique role identifiers to define which roles are allowed to edit the monitor. Editing a monitor includes any
+               updates to the monitor configuration, monitor deletion, and muting of the monitor for any amount of time. Roles unique
+               identifiers can be pulled from the [Roles API](https://docs.datadoghq.com/api/latest/roles/#list-roles) in the `data.id`
+               field.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to associate with your monitor. This can help you categorize and filter monitors in the manage monitors
                page of the UI. Note: it's not currently possible to filter by these tags when querying via the API
-        :param pulumi.Input[int] timeout_h: The number of hours of the monitor not reporting data before it will automatically resolve from a triggered state.
+        :param pulumi.Input[int] timeout_h: The number of hours of the monitor not reporting data before it automatically resolves from a triggered state. The
+               minimum allowed value is 0 hours. The maximum allowed value is 24 hours.
         :param pulumi.Input[str] type: The type of the monitor. The mapping from these types to the types found in the Datadog Web UI can be found in the
                Datadog API [documentation page](https://docs.datadoghq.com/api/v1/monitors/#create-a-monitor). Note: The monitor type
                cannot be changed after a monitor is created.
         :param pulumi.Input[bool] validate: If set to `false`, skip the validation call done during plan.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
@@ -1439,15 +1476,16 @@
         """
         return pulumi.get(self, "locked")
 
     @property
     @pulumi.getter
     def message(self) -> pulumi.Output[str]:
         """
-        A message to include with notifications for this monitor.
+        A message to include with notifications for this monitor. Email notifications can be sent to specific users by using the
+        same `@username` notation as events.
         """
         return pulumi.get(self, "message")
 
     @property
     @pulumi.getter(name="monitorThresholdWindows")
     def monitor_threshold_windows(self) -> pulumi.Output[Optional['outputs.MonitorMonitorThresholdWindows']]:
         """
@@ -1573,14 +1611,20 @@
         all times` and `in total` aggregation. `false` otherwise.
         """
         return pulumi.get(self, "require_full_window")
 
     @property
     @pulumi.getter(name="restrictedRoles")
     def restricted_roles(self) -> pulumi.Output[Optional[Sequence[str]]]:
+        """
+        A list of unique role identifiers to define which roles are allowed to edit the monitor. Editing a monitor includes any
+        updates to the monitor configuration, monitor deletion, and muting of the monitor for any amount of time. Roles unique
+        identifiers can be pulled from the [Roles API](https://docs.datadoghq.com/api/latest/roles/#list-roles) in the `data.id`
+        field.
+        """
         return pulumi.get(self, "restricted_roles")
 
     @property
     @pulumi.getter
     def tags(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         A list of tags to associate with your monitor. This can help you categorize and filter monitors in the manage monitors
@@ -1588,15 +1632,16 @@
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="timeoutH")
     def timeout_h(self) -> pulumi.Output[Optional[int]]:
         """
-        The number of hours of the monitor not reporting data before it will automatically resolve from a triggered state.
+        The number of hours of the monitor not reporting data before it automatically resolves from a triggered state. The
+        minimum allowed value is 0 hours. The maximum allowed value is 24 hours.
         """
         return pulumi.get(self, "timeout_h")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/monitor_json.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/monitor_json.py`

 * *Files identical despite different names*

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/organization_settings.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/organization_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/outputs.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,14 +379,16 @@
     'DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionRequestRumQueryGroupBySortQuery',
     'DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionRequestRumQueryMultiCompute',
     'DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionRequestSecurityQuery',
     'DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionRequestSecurityQueryComputeQuery',
     'DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionRequestSecurityQueryGroupBy',
     'DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionRequestSecurityQueryGroupBySortQuery',
     'DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionRequestSecurityQueryMultiCompute',
+    'DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionTimeseriesBackground',
+    'DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionTimeseriesBackgroundYaxis',
     'DashboardWidgetGroupDefinitionWidgetScatterplotDefinition',
     'DashboardWidgetGroupDefinitionWidgetScatterplotDefinitionCustomLink',
     'DashboardWidgetGroupDefinitionWidgetScatterplotDefinitionRequest',
     'DashboardWidgetGroupDefinitionWidgetScatterplotDefinitionRequestScatterplotTable',
     'DashboardWidgetGroupDefinitionWidgetScatterplotDefinitionRequestScatterplotTableFormula',
     'DashboardWidgetGroupDefinitionWidgetScatterplotDefinitionRequestScatterplotTableQuery',
     'DashboardWidgetGroupDefinitionWidgetScatterplotDefinitionRequestScatterplotTableQueryApmDependencyStatsQuery',
@@ -770,14 +772,16 @@
     'DashboardWidgetQueryValueDefinitionRequestRumQueryGroupBySortQuery',
     'DashboardWidgetQueryValueDefinitionRequestRumQueryMultiCompute',
     'DashboardWidgetQueryValueDefinitionRequestSecurityQuery',
     'DashboardWidgetQueryValueDefinitionRequestSecurityQueryComputeQuery',
     'DashboardWidgetQueryValueDefinitionRequestSecurityQueryGroupBy',
     'DashboardWidgetQueryValueDefinitionRequestSecurityQueryGroupBySortQuery',
     'DashboardWidgetQueryValueDefinitionRequestSecurityQueryMultiCompute',
+    'DashboardWidgetQueryValueDefinitionTimeseriesBackground',
+    'DashboardWidgetQueryValueDefinitionTimeseriesBackgroundYaxis',
     'DashboardWidgetScatterplotDefinition',
     'DashboardWidgetScatterplotDefinitionCustomLink',
     'DashboardWidgetScatterplotDefinitionRequest',
     'DashboardWidgetScatterplotDefinitionRequestScatterplotTable',
     'DashboardWidgetScatterplotDefinitionRequestScatterplotTableFormula',
     'DashboardWidgetScatterplotDefinitionRequestScatterplotTableQuery',
     'DashboardWidgetScatterplotDefinitionRequestScatterplotTableQueryApmDependencyStatsQuery',
@@ -1061,21 +1065,23 @@
     'RolePermission',
     'SecurityMonitoringDefaultRuleCase',
     'SecurityMonitoringDefaultRuleFilter',
     'SecurityMonitoringFilterExclusionFilter',
     'SecurityMonitoringRuleCase',
     'SecurityMonitoringRuleFilter',
     'SecurityMonitoringRuleOptions',
+    'SecurityMonitoringRuleOptionsImpossibleTravelOptions',
     'SecurityMonitoringRuleOptionsNewValueOptions',
     'SecurityMonitoringRuleQuery',
     'SecurityMonitoringRuleQueryAgentRule',
     'ServiceLevelObjectiveQuery',
     'ServiceLevelObjectiveThreshold',
     'SyntheticsGlobalVariableParseTestOptions',
     'SyntheticsGlobalVariableParseTestOptionsParser',
+    'SyntheticsPrivateLocationMetadata',
     'SyntheticsTestApiStep',
     'SyntheticsTestApiStepAssertion',
     'SyntheticsTestApiStepAssertionTargetjsonpath',
     'SyntheticsTestApiStepExtractedValue',
     'SyntheticsTestApiStepExtractedValueParser',
     'SyntheticsTestApiStepRequestBasicauth',
     'SyntheticsTestApiStepRequestClientCertificate',
@@ -1113,56 +1119,48 @@
     'GetRolesRoleResult',
     'GetSecurityMonitoringFiltersFilterResult',
     'GetSecurityMonitoringFiltersFilterExclusionFilterResult',
     'GetSecurityMonitoringRulesRuleResult',
     'GetSecurityMonitoringRulesRuleCaseResult',
     'GetSecurityMonitoringRulesRuleFilterResult',
     'GetSecurityMonitoringRulesRuleOptionsResult',
+    'GetSecurityMonitoringRulesRuleOptionsImpossibleTravelOptionsResult',
     'GetSecurityMonitoringRulesRuleOptionsNewValueOptionsResult',
     'GetSecurityMonitoringRulesRuleQueryResult',
     'GetSecurityMonitoringRulesRuleQueryAgentRuleResult',
     'GetServiceLevelObjectivesSloResult',
 ]
 
 @pulumi.output_type
 class ChildOrganizationApiKey(dict):
     def __init__(__self__, *,
                  key: Optional[str] = None,
                  name: Optional[str] = None):
-        """
-        :param str name: Name for Child Organization after creation.
-        """
         if key is not None:
             pulumi.set(__self__, "key", key)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def key(self) -> Optional[str]:
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
-        """
-        Name for Child Organization after creation.
-        """
         return pulumi.get(self, "name")
 
 
 @pulumi.output_type
 class ChildOrganizationApplicationKey(dict):
     def __init__(__self__, *,
                  hash: Optional[str] = None,
                  name: Optional[str] = None,
                  owner: Optional[str] = None):
-        """
-        :param str name: Name for Child Organization after creation.
-        """
         if hash is not None:
             pulumi.set(__self__, "hash", hash)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if owner is not None:
             pulumi.set(__self__, "owner", owner)
 
@@ -1170,17 +1168,14 @@
     @pulumi.getter
     def hash(self) -> Optional[str]:
         return pulumi.get(self, "hash")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
-        """
-        Name for Child Organization after creation.
-        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def owner(self) -> Optional[str]:
         return pulumi.get(self, "owner")
 
@@ -1382,17 +1377,14 @@
         ChildOrganizationUser.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  access_role: Optional[str] = None,
                  email: Optional[str] = None,
                  name: Optional[str] = None):
-        """
-        :param str name: Name for Child Organization after creation.
-        """
         if access_role is not None:
             pulumi.set(__self__, "access_role", access_role)
         if email is not None:
             pulumi.set(__self__, "email", email)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
@@ -1405,17 +1397,14 @@
     @pulumi.getter
     def email(self) -> Optional[str]:
         return pulumi.get(self, "email")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
-        """
-        Name for Child Organization after creation.
-        """
         return pulumi.get(self, "name")
 
 
 @pulumi.output_type
 class DashboardListDashItem(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -1433,35 +1422,25 @@
     def get(self, key: str, default = None) -> Any:
         DashboardListDashItem.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  dash_id: str,
                  type: str):
-        """
-        :param str dash_id: The ID of the dashboard to add
-        :param str type: The type of this dashboard. Valid values are `custom_timeboard`, `custom_screenboard`, `integration_screenboard`, `integration_timeboard`, `host_timeboard`.
-        """
         pulumi.set(__self__, "dash_id", dash_id)
         pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter(name="dashId")
     def dash_id(self) -> str:
-        """
-        The ID of the dashboard to add
-        """
         return pulumi.get(self, "dash_id")
 
     @property
     @pulumi.getter
     def type(self) -> str:
-        """
-        The type of this dashboard. Valid values are `custom_timeboard`, `custom_screenboard`, `integration_screenboard`, `integration_timeboard`, `host_timeboard`.
-        """
         return pulumi.get(self, "type")
 
 
 @pulumi.output_type
 class DashboardTemplateVariable(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -1481,58 +1460,40 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  name: str,
                  available_values: Optional[Sequence[str]] = None,
                  default: Optional[str] = None,
                  prefix: Optional[str] = None):
-        """
-        :param str name: The name of the variable.
-        :param Sequence[str] available_values: The list of values that the template variable drop-down is be limited to
-        :param str default: The default value for the template variable on dashboard load.
-        :param str prefix: The tag prefix associated with the variable. Only tags with this prefix appear in the variable dropdown.
-        """
         pulumi.set(__self__, "name", name)
         if available_values is not None:
             pulumi.set(__self__, "available_values", available_values)
         if default is not None:
             pulumi.set(__self__, "default", default)
         if prefix is not None:
             pulumi.set(__self__, "prefix", prefix)
 
     @property
     @pulumi.getter
     def name(self) -> str:
-        """
-        The name of the variable.
-        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="availableValues")
     def available_values(self) -> Optional[Sequence[str]]:
-        """
-        The list of values that the template variable drop-down is be limited to
-        """
         return pulumi.get(self, "available_values")
 
     @property
     @pulumi.getter
     def default(self) -> Optional[str]:
-        """
-        The default value for the template variable on dashboard load.
-        """
         return pulumi.get(self, "default")
 
     @property
     @pulumi.getter
     def prefix(self) -> Optional[str]:
-        """
-        The tag prefix associated with the variable. Only tags with this prefix appear in the variable dropdown.
-        """
         return pulumi.get(self, "prefix")
 
 
 @pulumi.output_type
 class DashboardTemplateVariablePreset(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -1550,59 +1511,43 @@
     def get(self, key: str, default = None) -> Any:
         DashboardTemplateVariablePreset.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  name: Optional[str] = None,
                  template_variables: Optional[Sequence['outputs.DashboardTemplateVariablePresetTemplateVariable']] = None):
-        """
-        :param str name: The name of the preset.
-        :param Sequence['DashboardTemplateVariablePresetTemplateVariableArgs'] template_variables: The template variable names and assumed values under the given preset
-        """
         if name is not None:
             pulumi.set(__self__, "name", name)
         if template_variables is not None:
             pulumi.set(__self__, "template_variables", template_variables)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
-        """
-        The name of the preset.
-        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="templateVariables")
     def template_variables(self) -> Optional[Sequence['outputs.DashboardTemplateVariablePresetTemplateVariable']]:
-        """
-        The template variable names and assumed values under the given preset
-        """
         return pulumi.get(self, "template_variables")
 
 
 @pulumi.output_type
 class DashboardTemplateVariablePresetTemplateVariable(dict):
     def __init__(__self__, *,
                  name: Optional[str] = None,
                  value: Optional[str] = None):
-        """
-        :param str name: The name of the variable.
-        """
         if name is not None:
             pulumi.set(__self__, "name", name)
         if value is not None:
             pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
-        """
-        The name of the variable.
-        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def value(self) -> Optional[str]:
         return pulumi.get(self, "value")
 
@@ -1706,45 +1651,14 @@
                  servicemap_definition: Optional['outputs.DashboardWidgetServicemapDefinition'] = None,
                  sunburst_definition: Optional['outputs.DashboardWidgetSunburstDefinition'] = None,
                  timeseries_definition: Optional['outputs.DashboardWidgetTimeseriesDefinition'] = None,
                  toplist_definition: Optional['outputs.DashboardWidgetToplistDefinition'] = None,
                  trace_service_definition: Optional['outputs.DashboardWidgetTraceServiceDefinition'] = None,
                  treemap_definition: Optional['outputs.DashboardWidgetTreemapDefinition'] = None,
                  widget_layout: Optional['outputs.DashboardWidgetWidgetLayout'] = None):
-        """
-        :param 'DashboardWidgetAlertGraphDefinitionArgs' alert_graph_definition: The definition for a Alert Graph widget.
-        :param 'DashboardWidgetAlertValueDefinitionArgs' alert_value_definition: The definition for a Alert Value widget.
-        :param 'DashboardWidgetChangeDefinitionArgs' change_definition: The definition for a Change widget.
-        :param 'DashboardWidgetCheckStatusDefinitionArgs' check_status_definition: The definition for a Check Status widget.
-        :param 'DashboardWidgetDistributionDefinitionArgs' distribution_definition: The definition for a Distribution widget.
-        :param 'DashboardWidgetEventStreamDefinitionArgs' event_stream_definition: The definition for a Event Stream widget.
-        :param 'DashboardWidgetEventTimelineDefinitionArgs' event_timeline_definition: The definition for a Event Timeline widget.
-        :param 'DashboardWidgetFreeTextDefinitionArgs' free_text_definition: The definition for a Free Text widget.
-        :param 'DashboardWidgetGeomapDefinitionArgs' geomap_definition: The definition for a Geomap widget.
-        :param 'DashboardWidgetGroupDefinitionArgs' group_definition: The definition for a Group widget.
-        :param 'DashboardWidgetHeatmapDefinitionArgs' heatmap_definition: The definition for a Heatmap widget.
-        :param 'DashboardWidgetHostmapDefinitionArgs' hostmap_definition: The definition for a Hostmap widget.
-        :param int id: The ID of the widget.
-        :param 'DashboardWidgetIframeDefinitionArgs' iframe_definition: The definition for an Iframe widget.
-        :param 'DashboardWidgetImageDefinitionArgs' image_definition: The definition for an Image widget
-        :param 'DashboardWidgetLogStreamDefinitionArgs' log_stream_definition: The definition for an Log Stream widget.
-        :param 'DashboardWidgetManageStatusDefinitionArgs' manage_status_definition: The definition for an Manage Status widget.
-        :param 'DashboardWidgetNoteDefinitionArgs' note_definition: The definition for a Note widget.
-        :param 'DashboardWidgetQueryTableDefinitionArgs' query_table_definition: The definition for a Query Table widget.
-        :param 'DashboardWidgetQueryValueDefinitionArgs' query_value_definition: The definition for a Query Value widget.
-        :param 'DashboardWidgetScatterplotDefinitionArgs' scatterplot_definition: The definition for a Scatterplot widget.
-        :param 'DashboardWidgetServiceLevelObjectiveDefinitionArgs' service_level_objective_definition: The definition for a Service Level Objective widget.
-        :param 'DashboardWidgetServicemapDefinitionArgs' servicemap_definition: The definition for a Service Map widget.
-        :param 'DashboardWidgetSunburstDefinitionArgs' sunburst_definition: The definition for a Sunburst widget.
-        :param 'DashboardWidgetTimeseriesDefinitionArgs' timeseries_definition: The definition for a Timeseries widget.
-        :param 'DashboardWidgetToplistDefinitionArgs' toplist_definition: The definition for a Toplist widget.
-        :param 'DashboardWidgetTraceServiceDefinitionArgs' trace_service_definition: The definition for a Trace Service widget.
-        :param 'DashboardWidgetTreemapDefinitionArgs' treemap_definition: The definition for a Treemap widget.
-        :param 'DashboardWidgetWidgetLayoutArgs' widget_layout: The layout of the widget on a 'free' dashboard.
-        """
         if alert_graph_definition is not None:
             pulumi.set(__self__, "alert_graph_definition", alert_graph_definition)
         if alert_value_definition is not None:
             pulumi.set(__self__, "alert_value_definition", alert_value_definition)
         if change_definition is not None:
             pulumi.set(__self__, "change_definition", change_definition)
         if check_status_definition is not None:
@@ -1799,241 +1713,154 @@
             pulumi.set(__self__, "treemap_definition", treemap_definition)
         if widget_layout is not None:
             pulumi.set(__self__, "widget_layout", widget_layout)
 
     @property
     @pulumi.getter(name="alertGraphDefinition")
     def alert_graph_definition(self) -> Optional['outputs.DashboardWidgetAlertGraphDefinition']:
-        """
-        The definition for a Alert Graph widget.
-        """
         return pulumi.get(self, "alert_graph_definition")
 
     @property
     @pulumi.getter(name="alertValueDefinition")
     def alert_value_definition(self) -> Optional['outputs.DashboardWidgetAlertValueDefinition']:
-        """
-        The definition for a Alert Value widget.
-        """
         return pulumi.get(self, "alert_value_definition")
 
     @property
     @pulumi.getter(name="changeDefinition")
     def change_definition(self) -> Optional['outputs.DashboardWidgetChangeDefinition']:
-        """
-        The definition for a Change widget.
-        """
         return pulumi.get(self, "change_definition")
 
     @property
     @pulumi.getter(name="checkStatusDefinition")
     def check_status_definition(self) -> Optional['outputs.DashboardWidgetCheckStatusDefinition']:
-        """
-        The definition for a Check Status widget.
-        """
         return pulumi.get(self, "check_status_definition")
 
     @property
     @pulumi.getter(name="distributionDefinition")
     def distribution_definition(self) -> Optional['outputs.DashboardWidgetDistributionDefinition']:
-        """
-        The definition for a Distribution widget.
-        """
         return pulumi.get(self, "distribution_definition")
 
     @property
     @pulumi.getter(name="eventStreamDefinition")
     def event_stream_definition(self) -> Optional['outputs.DashboardWidgetEventStreamDefinition']:
-        """
-        The definition for a Event Stream widget.
-        """
         return pulumi.get(self, "event_stream_definition")
 
     @property
     @pulumi.getter(name="eventTimelineDefinition")
     def event_timeline_definition(self) -> Optional['outputs.DashboardWidgetEventTimelineDefinition']:
-        """
-        The definition for a Event Timeline widget.
-        """
         return pulumi.get(self, "event_timeline_definition")
 
     @property
     @pulumi.getter(name="freeTextDefinition")
     def free_text_definition(self) -> Optional['outputs.DashboardWidgetFreeTextDefinition']:
-        """
-        The definition for a Free Text widget.
-        """
         return pulumi.get(self, "free_text_definition")
 
     @property
     @pulumi.getter(name="geomapDefinition")
     def geomap_definition(self) -> Optional['outputs.DashboardWidgetGeomapDefinition']:
-        """
-        The definition for a Geomap widget.
-        """
         return pulumi.get(self, "geomap_definition")
 
     @property
     @pulumi.getter(name="groupDefinition")
     def group_definition(self) -> Optional['outputs.DashboardWidgetGroupDefinition']:
-        """
-        The definition for a Group widget.
-        """
         return pulumi.get(self, "group_definition")
 
     @property
     @pulumi.getter(name="heatmapDefinition")
     def heatmap_definition(self) -> Optional['outputs.DashboardWidgetHeatmapDefinition']:
-        """
-        The definition for a Heatmap widget.
-        """
         return pulumi.get(self, "heatmap_definition")
 
     @property
     @pulumi.getter(name="hostmapDefinition")
     def hostmap_definition(self) -> Optional['outputs.DashboardWidgetHostmapDefinition']:
-        """
-        The definition for a Hostmap widget.
-        """
         return pulumi.get(self, "hostmap_definition")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[int]:
-        """
-        The ID of the widget.
-        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="iframeDefinition")
     def iframe_definition(self) -> Optional['outputs.DashboardWidgetIframeDefinition']:
-        """
-        The definition for an Iframe widget.
-        """
         return pulumi.get(self, "iframe_definition")
 
     @property
     @pulumi.getter(name="imageDefinition")
     def image_definition(self) -> Optional['outputs.DashboardWidgetImageDefinition']:
-        """
-        The definition for an Image widget
-        """
         return pulumi.get(self, "image_definition")
 
     @property
     @pulumi.getter(name="logStreamDefinition")
     def log_stream_definition(self) -> Optional['outputs.DashboardWidgetLogStreamDefinition']:
-        """
-        The definition for an Log Stream widget.
-        """
         return pulumi.get(self, "log_stream_definition")
 
     @property
     @pulumi.getter(name="manageStatusDefinition")
     def manage_status_definition(self) -> Optional['outputs.DashboardWidgetManageStatusDefinition']:
-        """
-        The definition for an Manage Status widget.
-        """
         return pulumi.get(self, "manage_status_definition")
 
     @property
     @pulumi.getter(name="noteDefinition")
     def note_definition(self) -> Optional['outputs.DashboardWidgetNoteDefinition']:
-        """
-        The definition for a Note widget.
-        """
         return pulumi.get(self, "note_definition")
 
     @property
     @pulumi.getter(name="queryTableDefinition")
     def query_table_definition(self) -> Optional['outputs.DashboardWidgetQueryTableDefinition']:
-        """
-        The definition for a Query Table widget.
-        """
         return pulumi.get(self, "query_table_definition")
 
     @property
     @pulumi.getter(name="queryValueDefinition")
     def query_value_definition(self) -> Optional['outputs.DashboardWidgetQueryValueDefinition']:
-        """
-        The definition for a Query Value widget.
-        """
         return pulumi.get(self, "query_value_definition")
 
     @property
     @pulumi.getter(name="scatterplotDefinition")
     def scatterplot_definition(self) -> Optional['outputs.DashboardWidgetScatterplotDefinition']:
-        """
-        The definition for a Scatterplot widget.
-        """
         return pulumi.get(self, "scatterplot_definition")
 
     @property
     @pulumi.getter(name="serviceLevelObjectiveDefinition")
     def service_level_objective_definition(self) -> Optional['outputs.DashboardWidgetServiceLevelObjectiveDefinition']:
-        """
-        The definition for a Service Level Objective widget.
-        """
         return pulumi.get(self, "service_level_objective_definition")
 
     @property
     @pulumi.getter(name="servicemapDefinition")
     def servicemap_definition(self) -> Optional['outputs.DashboardWidgetServicemapDefinition']:
-        """
-        The definition for a Service Map widget.
-        """
         return pulumi.get(self, "servicemap_definition")
 
     @property
     @pulumi.getter(name="sunburstDefinition")
     def sunburst_definition(self) -> Optional['outputs.DashboardWidgetSunburstDefinition']:
-        """
-        The definition for a Sunburst widget.
-        """
         return pulumi.get(self, "sunburst_definition")
 
     @property
     @pulumi.getter(name="timeseriesDefinition")
     def timeseries_definition(self) -> Optional['outputs.DashboardWidgetTimeseriesDefinition']:
-        """
-        The definition for a Timeseries widget.
-        """
         return pulumi.get(self, "timeseries_definition")
 
     @property
     @pulumi.getter(name="toplistDefinition")
     def toplist_definition(self) -> Optional['outputs.DashboardWidgetToplistDefinition']:
-        """
-        The definition for a Toplist widget.
-        """
         return pulumi.get(self, "toplist_definition")
 
     @property
     @pulumi.getter(name="traceServiceDefinition")
     def trace_service_definition(self) -> Optional['outputs.DashboardWidgetTraceServiceDefinition']:
-        """
-        The definition for a Trace Service widget.
-        """
         return pulumi.get(self, "trace_service_definition")
 
     @property
     @pulumi.getter(name="treemapDefinition")
     def treemap_definition(self) -> Optional['outputs.DashboardWidgetTreemapDefinition']:
-        """
-        The definition for a Treemap widget.
-        """
         return pulumi.get(self, "treemap_definition")
 
     @property
     @pulumi.getter(name="widgetLayout")
     def widget_layout(self) -> Optional['outputs.DashboardWidgetWidgetLayout']:
-        """
-        The layout of the widget on a 'free' dashboard.
-        """
         return pulumi.get(self, "widget_layout")
 
 
 @pulumi.output_type
 class DashboardWidgetAlertGraphDefinition(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -2063,17 +1890,14 @@
     def __init__(__self__, *,
                  alert_id: str,
                  viz_type: str,
                  live_span: Optional[str] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         pulumi.set(__self__, "alert_id", alert_id)
         pulumi.set(__self__, "viz_type", viz_type)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if title is not None:
             pulumi.set(__self__, "title", title)
         if title_align is not None:
@@ -2095,17 +1919,14 @@
     @pulumi.getter(name="liveSpan")
     def live_span(self) -> Optional[str]:
         return pulumi.get(self, "live_span")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -2144,17 +1965,14 @@
                  alert_id: str,
                  precision: Optional[int] = None,
                  text_align: Optional[str] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None,
                  unit: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         pulumi.set(__self__, "alert_id", alert_id)
         if precision is not None:
             pulumi.set(__self__, "precision", precision)
         if text_align is not None:
             pulumi.set(__self__, "text_align", text_align)
         if title is not None:
             pulumi.set(__self__, "title", title)
@@ -2179,17 +1997,14 @@
     @pulumi.getter(name="textAlign")
     def text_align(self) -> Optional[str]:
         return pulumi.get(self, "text_align")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -2232,17 +2047,14 @@
     def __init__(__self__, *,
                  custom_links: Optional[Sequence['outputs.DashboardWidgetChangeDefinitionCustomLink']] = None,
                  live_span: Optional[str] = None,
                  requests: Optional[Sequence['outputs.DashboardWidgetChangeDefinitionRequest']] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if requests is not None:
             pulumi.set(__self__, "requests", requests)
         if title is not None:
@@ -2266,17 +2078,14 @@
     @pulumi.getter
     def requests(self) -> Optional[Sequence['outputs.DashboardWidgetChangeDefinitionRequest']]:
         return pulumi.get(self, "requests")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -4145,17 +3954,14 @@
                  group: Optional[str] = None,
                  group_bies: Optional[Sequence[str]] = None,
                  live_span: Optional[str] = None,
                  tags: Optional[Sequence[str]] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         pulumi.set(__self__, "check", check)
         pulumi.set(__self__, "grouping", grouping)
         if group is not None:
             pulumi.set(__self__, "group", group)
         if group_bies is not None:
             pulumi.set(__self__, "group_bies", group_bies)
         if live_span is not None:
@@ -4198,17 +4004,14 @@
     @pulumi.getter
     def tags(self) -> Optional[Sequence[str]]:
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -4249,17 +4052,14 @@
                  legend_size: Optional[str] = None,
                  live_span: Optional[str] = None,
                  requests: Optional[Sequence['outputs.DashboardWidgetDistributionDefinitionRequest']] = None,
                  show_legend: Optional[bool] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         if legend_size is not None:
             pulumi.set(__self__, "legend_size", legend_size)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if requests is not None:
             pulumi.set(__self__, "requests", requests)
         if show_legend is not None:
@@ -4290,17 +4090,14 @@
     @pulumi.getter(name="showLegend")
     def show_legend(self) -> Optional[bool]:
         return pulumi.get(self, "show_legend")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -5417,17 +5214,14 @@
                  query: str,
                  event_size: Optional[str] = None,
                  live_span: Optional[str] = None,
                  tags_execution: Optional[str] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         pulumi.set(__self__, "query", query)
         if event_size is not None:
             pulumi.set(__self__, "event_size", event_size)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if tags_execution is not None:
             pulumi.set(__self__, "tags_execution", tags_execution)
@@ -5457,17 +5251,14 @@
     @pulumi.getter(name="tagsExecution")
     def tags_execution(self) -> Optional[str]:
         return pulumi.get(self, "tags_execution")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -5505,17 +5296,14 @@
     def __init__(__self__, *,
                  query: str,
                  live_span: Optional[str] = None,
                  tags_execution: Optional[str] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         pulumi.set(__self__, "query", query)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if tags_execution is not None:
             pulumi.set(__self__, "tags_execution", tags_execution)
         if title is not None:
             pulumi.set(__self__, "title", title)
@@ -5538,17 +5326,14 @@
     @pulumi.getter(name="tagsExecution")
     def tags_execution(self) -> Optional[str]:
         return pulumi.get(self, "tags_execution")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -5643,17 +5428,14 @@
                  custom_links: Optional[Sequence['outputs.DashboardWidgetGeomapDefinitionCustomLink']] = None,
                  live_span: Optional[str] = None,
                  requests: Optional[Sequence['outputs.DashboardWidgetGeomapDefinitionRequest']] = None,
                  style: Optional['outputs.DashboardWidgetGeomapDefinitionStyle'] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         pulumi.set(__self__, "view", view)
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if requests is not None:
             pulumi.set(__self__, "requests", requests)
@@ -5690,17 +5472,14 @@
     @pulumi.getter
     def style(self) -> Optional['outputs.DashboardWidgetGeomapDefinitionStyle']:
         return pulumi.get(self, "style")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -7077,44 +6856,33 @@
     def __init__(__self__, *,
                  layout_type: str,
                  widgets: Sequence['outputs.DashboardWidgetGroupDefinitionWidget'],
                  background_color: Optional[str] = None,
                  banner_img: Optional[str] = None,
                  show_title: Optional[bool] = None,
                  title: Optional[str] = None):
-        """
-        :param str layout_type: The layout type of the dashboard. Valid values are `ordered`, `free`.
-        :param Sequence['DashboardWidgetGroupDefinitionWidgetArgs'] widgets: The list of widgets to display on the dashboard.
-        :param str title: The title of the dashboard.
-        """
         pulumi.set(__self__, "layout_type", layout_type)
         pulumi.set(__self__, "widgets", widgets)
         if background_color is not None:
             pulumi.set(__self__, "background_color", background_color)
         if banner_img is not None:
             pulumi.set(__self__, "banner_img", banner_img)
         if show_title is not None:
             pulumi.set(__self__, "show_title", show_title)
         if title is not None:
             pulumi.set(__self__, "title", title)
 
     @property
     @pulumi.getter(name="layoutType")
     def layout_type(self) -> str:
-        """
-        The layout type of the dashboard. Valid values are `ordered`, `free`.
-        """
         return pulumi.get(self, "layout_type")
 
     @property
     @pulumi.getter
     def widgets(self) -> Sequence['outputs.DashboardWidgetGroupDefinitionWidget']:
-        """
-        The list of widgets to display on the dashboard.
-        """
         return pulumi.get(self, "widgets")
 
     @property
     @pulumi.getter(name="backgroundColor")
     def background_color(self) -> Optional[str]:
         return pulumi.get(self, "background_color")
 
@@ -7127,17 +6895,14 @@
     @pulumi.getter(name="showTitle")
     def show_title(self) -> Optional[bool]:
         return pulumi.get(self, "show_title")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
 
 @pulumi.output_type
 class DashboardWidgetGroupDefinitionWidget(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -7233,44 +6998,14 @@
                  servicemap_definition: Optional['outputs.DashboardWidgetGroupDefinitionWidgetServicemapDefinition'] = None,
                  sunburst_definition: Optional['outputs.DashboardWidgetGroupDefinitionWidgetSunburstDefinition'] = None,
                  timeseries_definition: Optional['outputs.DashboardWidgetGroupDefinitionWidgetTimeseriesDefinition'] = None,
                  toplist_definition: Optional['outputs.DashboardWidgetGroupDefinitionWidgetToplistDefinition'] = None,
                  trace_service_definition: Optional['outputs.DashboardWidgetGroupDefinitionWidgetTraceServiceDefinition'] = None,
                  treemap_definition: Optional['outputs.DashboardWidgetGroupDefinitionWidgetTreemapDefinition'] = None,
                  widget_layout: Optional['outputs.DashboardWidgetGroupDefinitionWidgetWidgetLayout'] = None):
-        """
-        :param 'DashboardWidgetGroupDefinitionWidgetAlertGraphDefinitionArgs' alert_graph_definition: The definition for a Alert Graph widget.
-        :param 'DashboardWidgetGroupDefinitionWidgetAlertValueDefinitionArgs' alert_value_definition: The definition for a Alert Value widget.
-        :param 'DashboardWidgetGroupDefinitionWidgetChangeDefinitionArgs' change_definition: The definition for a Change widget.
-        :param 'DashboardWidgetGroupDefinitionWidgetCheckStatusDefinitionArgs' check_status_definition: The definition for a Check Status widget.
-        :param 'DashboardWidgetGroupDefinitionWidgetDistributionDefinitionArgs' distribution_definition: The definition for a Distribution widget.
-        :param 'DashboardWidgetGroupDefinitionWidgetEventStreamDefinitionArgs' event_stream_definition: The definition for a Event Stream widget.
-        :param 'DashboardWidgetGroupDefinitionWidgetEventTimelineDefinitionArgs' event_timeline_definition: The definition for a Event Timeline widget.
-        :param 'DashboardWidgetGroupDefinitionWidgetFreeTextDefinitionArgs' free_text_definition: The definition for a Free Text widget.
-        :param 'DashboardWidgetGroupDefinitionWidgetGeomapDefinitionArgs' geomap_definition: The definition for a Geomap widget.
-        :param 'DashboardWidgetGroupDefinitionWidgetHeatmapDefinitionArgs' heatmap_definition: The definition for a Heatmap widget.
-        :param 'DashboardWidgetGroupDefinitionWidgetHostmapDefinitionArgs' hostmap_definition: The definition for a Hostmap widget.
-        :param int id: The ID of the widget.
-        :param 'DashboardWidgetGroupDefinitionWidgetIframeDefinitionArgs' iframe_definition: The definition for an Iframe widget.
-        :param 'DashboardWidgetGroupDefinitionWidgetImageDefinitionArgs' image_definition: The definition for an Image widget
-        :param 'DashboardWidgetGroupDefinitionWidgetLogStreamDefinitionArgs' log_stream_definition: The definition for an Log Stream widget.
-        :param 'DashboardWidgetGroupDefinitionWidgetManageStatusDefinitionArgs' manage_status_definition: The definition for an Manage Status widget.
-        :param 'DashboardWidgetGroupDefinitionWidgetNoteDefinitionArgs' note_definition: The definition for a Note widget.
-        :param 'DashboardWidgetGroupDefinitionWidgetQueryTableDefinitionArgs' query_table_definition: The definition for a Query Table widget.
-        :param 'DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionArgs' query_value_definition: The definition for a Query Value widget.
-        :param 'DashboardWidgetGroupDefinitionWidgetScatterplotDefinitionArgs' scatterplot_definition: The definition for a Scatterplot widget.
-        :param 'DashboardWidgetGroupDefinitionWidgetServiceLevelObjectiveDefinitionArgs' service_level_objective_definition: The definition for a Service Level Objective widget.
-        :param 'DashboardWidgetGroupDefinitionWidgetServicemapDefinitionArgs' servicemap_definition: The definition for a Service Map widget.
-        :param 'DashboardWidgetGroupDefinitionWidgetSunburstDefinitionArgs' sunburst_definition: The definition for a Sunburst widget.
-        :param 'DashboardWidgetGroupDefinitionWidgetTimeseriesDefinitionArgs' timeseries_definition: The definition for a Timeseries widget.
-        :param 'DashboardWidgetGroupDefinitionWidgetToplistDefinitionArgs' toplist_definition: The definition for a Toplist widget.
-        :param 'DashboardWidgetGroupDefinitionWidgetTraceServiceDefinitionArgs' trace_service_definition: The definition for a Trace Service widget.
-        :param 'DashboardWidgetGroupDefinitionWidgetTreemapDefinitionArgs' treemap_definition: The definition for a Treemap widget.
-        :param 'DashboardWidgetGroupDefinitionWidgetWidgetLayoutArgs' widget_layout: The layout of the widget on a 'free' dashboard.
-        """
         if alert_graph_definition is not None:
             pulumi.set(__self__, "alert_graph_definition", alert_graph_definition)
         if alert_value_definition is not None:
             pulumi.set(__self__, "alert_value_definition", alert_value_definition)
         if change_definition is not None:
             pulumi.set(__self__, "change_definition", change_definition)
         if check_status_definition is not None:
@@ -7323,233 +7058,149 @@
             pulumi.set(__self__, "treemap_definition", treemap_definition)
         if widget_layout is not None:
             pulumi.set(__self__, "widget_layout", widget_layout)
 
     @property
     @pulumi.getter(name="alertGraphDefinition")
     def alert_graph_definition(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetAlertGraphDefinition']:
-        """
-        The definition for a Alert Graph widget.
-        """
         return pulumi.get(self, "alert_graph_definition")
 
     @property
     @pulumi.getter(name="alertValueDefinition")
     def alert_value_definition(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetAlertValueDefinition']:
-        """
-        The definition for a Alert Value widget.
-        """
         return pulumi.get(self, "alert_value_definition")
 
     @property
     @pulumi.getter(name="changeDefinition")
     def change_definition(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetChangeDefinition']:
-        """
-        The definition for a Change widget.
-        """
         return pulumi.get(self, "change_definition")
 
     @property
     @pulumi.getter(name="checkStatusDefinition")
     def check_status_definition(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetCheckStatusDefinition']:
-        """
-        The definition for a Check Status widget.
-        """
         return pulumi.get(self, "check_status_definition")
 
     @property
     @pulumi.getter(name="distributionDefinition")
     def distribution_definition(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetDistributionDefinition']:
-        """
-        The definition for a Distribution widget.
-        """
         return pulumi.get(self, "distribution_definition")
 
     @property
     @pulumi.getter(name="eventStreamDefinition")
     def event_stream_definition(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetEventStreamDefinition']:
-        """
-        The definition for a Event Stream widget.
-        """
         return pulumi.get(self, "event_stream_definition")
 
     @property
     @pulumi.getter(name="eventTimelineDefinition")
     def event_timeline_definition(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetEventTimelineDefinition']:
-        """
-        The definition for a Event Timeline widget.
-        """
         return pulumi.get(self, "event_timeline_definition")
 
     @property
     @pulumi.getter(name="freeTextDefinition")
     def free_text_definition(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetFreeTextDefinition']:
-        """
-        The definition for a Free Text widget.
-        """
         return pulumi.get(self, "free_text_definition")
 
     @property
     @pulumi.getter(name="geomapDefinition")
     def geomap_definition(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetGeomapDefinition']:
-        """
-        The definition for a Geomap widget.
-        """
         return pulumi.get(self, "geomap_definition")
 
     @property
     @pulumi.getter(name="heatmapDefinition")
     def heatmap_definition(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetHeatmapDefinition']:
-        """
-        The definition for a Heatmap widget.
-        """
         return pulumi.get(self, "heatmap_definition")
 
     @property
     @pulumi.getter(name="hostmapDefinition")
     def hostmap_definition(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetHostmapDefinition']:
-        """
-        The definition for a Hostmap widget.
-        """
         return pulumi.get(self, "hostmap_definition")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[int]:
-        """
-        The ID of the widget.
-        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="iframeDefinition")
     def iframe_definition(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetIframeDefinition']:
-        """
-        The definition for an Iframe widget.
-        """
         return pulumi.get(self, "iframe_definition")
 
     @property
     @pulumi.getter(name="imageDefinition")
     def image_definition(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetImageDefinition']:
-        """
-        The definition for an Image widget
-        """
         return pulumi.get(self, "image_definition")
 
     @property
     @pulumi.getter(name="logStreamDefinition")
     def log_stream_definition(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetLogStreamDefinition']:
-        """
-        The definition for an Log Stream widget.
-        """
         return pulumi.get(self, "log_stream_definition")
 
     @property
     @pulumi.getter(name="manageStatusDefinition")
     def manage_status_definition(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetManageStatusDefinition']:
-        """
-        The definition for an Manage Status widget.
-        """
         return pulumi.get(self, "manage_status_definition")
 
     @property
     @pulumi.getter(name="noteDefinition")
     def note_definition(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetNoteDefinition']:
-        """
-        The definition for a Note widget.
-        """
         return pulumi.get(self, "note_definition")
 
     @property
     @pulumi.getter(name="queryTableDefinition")
     def query_table_definition(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetQueryTableDefinition']:
-        """
-        The definition for a Query Table widget.
-        """
         return pulumi.get(self, "query_table_definition")
 
     @property
     @pulumi.getter(name="queryValueDefinition")
     def query_value_definition(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetQueryValueDefinition']:
-        """
-        The definition for a Query Value widget.
-        """
         return pulumi.get(self, "query_value_definition")
 
     @property
     @pulumi.getter(name="scatterplotDefinition")
     def scatterplot_definition(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetScatterplotDefinition']:
-        """
-        The definition for a Scatterplot widget.
-        """
         return pulumi.get(self, "scatterplot_definition")
 
     @property
     @pulumi.getter(name="serviceLevelObjectiveDefinition")
     def service_level_objective_definition(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetServiceLevelObjectiveDefinition']:
-        """
-        The definition for a Service Level Objective widget.
-        """
         return pulumi.get(self, "service_level_objective_definition")
 
     @property
     @pulumi.getter(name="servicemapDefinition")
     def servicemap_definition(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetServicemapDefinition']:
-        """
-        The definition for a Service Map widget.
-        """
         return pulumi.get(self, "servicemap_definition")
 
     @property
     @pulumi.getter(name="sunburstDefinition")
     def sunburst_definition(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetSunburstDefinition']:
-        """
-        The definition for a Sunburst widget.
-        """
         return pulumi.get(self, "sunburst_definition")
 
     @property
     @pulumi.getter(name="timeseriesDefinition")
     def timeseries_definition(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetTimeseriesDefinition']:
-        """
-        The definition for a Timeseries widget.
-        """
         return pulumi.get(self, "timeseries_definition")
 
     @property
     @pulumi.getter(name="toplistDefinition")
     def toplist_definition(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetToplistDefinition']:
-        """
-        The definition for a Toplist widget.
-        """
         return pulumi.get(self, "toplist_definition")
 
     @property
     @pulumi.getter(name="traceServiceDefinition")
     def trace_service_definition(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetTraceServiceDefinition']:
-        """
-        The definition for a Trace Service widget.
-        """
         return pulumi.get(self, "trace_service_definition")
 
     @property
     @pulumi.getter(name="treemapDefinition")
     def treemap_definition(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetTreemapDefinition']:
-        """
-        The definition for a Treemap widget.
-        """
         return pulumi.get(self, "treemap_definition")
 
     @property
     @pulumi.getter(name="widgetLayout")
     def widget_layout(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetWidgetLayout']:
-        """
-        The layout of the widget on a 'free' dashboard.
-        """
         return pulumi.get(self, "widget_layout")
 
 
 @pulumi.output_type
 class DashboardWidgetGroupDefinitionWidgetAlertGraphDefinition(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -7579,17 +7230,14 @@
     def __init__(__self__, *,
                  alert_id: str,
                  viz_type: str,
                  live_span: Optional[str] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         pulumi.set(__self__, "alert_id", alert_id)
         pulumi.set(__self__, "viz_type", viz_type)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if title is not None:
             pulumi.set(__self__, "title", title)
         if title_align is not None:
@@ -7611,17 +7259,14 @@
     @pulumi.getter(name="liveSpan")
     def live_span(self) -> Optional[str]:
         return pulumi.get(self, "live_span")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -7660,17 +7305,14 @@
                  alert_id: str,
                  precision: Optional[int] = None,
                  text_align: Optional[str] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None,
                  unit: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         pulumi.set(__self__, "alert_id", alert_id)
         if precision is not None:
             pulumi.set(__self__, "precision", precision)
         if text_align is not None:
             pulumi.set(__self__, "text_align", text_align)
         if title is not None:
             pulumi.set(__self__, "title", title)
@@ -7695,17 +7337,14 @@
     @pulumi.getter(name="textAlign")
     def text_align(self) -> Optional[str]:
         return pulumi.get(self, "text_align")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -7748,17 +7387,14 @@
     def __init__(__self__, *,
                  custom_links: Optional[Sequence['outputs.DashboardWidgetGroupDefinitionWidgetChangeDefinitionCustomLink']] = None,
                  live_span: Optional[str] = None,
                  requests: Optional[Sequence['outputs.DashboardWidgetGroupDefinitionWidgetChangeDefinitionRequest']] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if requests is not None:
             pulumi.set(__self__, "requests", requests)
         if title is not None:
@@ -7782,17 +7418,14 @@
     @pulumi.getter
     def requests(self) -> Optional[Sequence['outputs.DashboardWidgetGroupDefinitionWidgetChangeDefinitionRequest']]:
         return pulumi.get(self, "requests")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -9661,17 +9294,14 @@
                  group: Optional[str] = None,
                  group_bies: Optional[Sequence[str]] = None,
                  live_span: Optional[str] = None,
                  tags: Optional[Sequence[str]] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         pulumi.set(__self__, "check", check)
         pulumi.set(__self__, "grouping", grouping)
         if group is not None:
             pulumi.set(__self__, "group", group)
         if group_bies is not None:
             pulumi.set(__self__, "group_bies", group_bies)
         if live_span is not None:
@@ -9714,17 +9344,14 @@
     @pulumi.getter
     def tags(self) -> Optional[Sequence[str]]:
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -9765,17 +9392,14 @@
                  legend_size: Optional[str] = None,
                  live_span: Optional[str] = None,
                  requests: Optional[Sequence['outputs.DashboardWidgetGroupDefinitionWidgetDistributionDefinitionRequest']] = None,
                  show_legend: Optional[bool] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         if legend_size is not None:
             pulumi.set(__self__, "legend_size", legend_size)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if requests is not None:
             pulumi.set(__self__, "requests", requests)
         if show_legend is not None:
@@ -9806,17 +9430,14 @@
     @pulumi.getter(name="showLegend")
     def show_legend(self) -> Optional[bool]:
         return pulumi.get(self, "show_legend")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -10933,17 +10554,14 @@
                  query: str,
                  event_size: Optional[str] = None,
                  live_span: Optional[str] = None,
                  tags_execution: Optional[str] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         pulumi.set(__self__, "query", query)
         if event_size is not None:
             pulumi.set(__self__, "event_size", event_size)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if tags_execution is not None:
             pulumi.set(__self__, "tags_execution", tags_execution)
@@ -10973,17 +10591,14 @@
     @pulumi.getter(name="tagsExecution")
     def tags_execution(self) -> Optional[str]:
         return pulumi.get(self, "tags_execution")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -11021,17 +10636,14 @@
     def __init__(__self__, *,
                  query: str,
                  live_span: Optional[str] = None,
                  tags_execution: Optional[str] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         pulumi.set(__self__, "query", query)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if tags_execution is not None:
             pulumi.set(__self__, "tags_execution", tags_execution)
         if title is not None:
             pulumi.set(__self__, "title", title)
@@ -11054,17 +10666,14 @@
     @pulumi.getter(name="tagsExecution")
     def tags_execution(self) -> Optional[str]:
         return pulumi.get(self, "tags_execution")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -11159,17 +10768,14 @@
                  custom_links: Optional[Sequence['outputs.DashboardWidgetGroupDefinitionWidgetGeomapDefinitionCustomLink']] = None,
                  live_span: Optional[str] = None,
                  requests: Optional[Sequence['outputs.DashboardWidgetGroupDefinitionWidgetGeomapDefinitionRequest']] = None,
                  style: Optional['outputs.DashboardWidgetGroupDefinitionWidgetGeomapDefinitionStyle'] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         pulumi.set(__self__, "view", view)
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if requests is not None:
             pulumi.set(__self__, "requests", requests)
@@ -11206,17 +10812,14 @@
     @pulumi.getter
     def style(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetGeomapDefinitionStyle']:
         return pulumi.get(self, "style")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -12601,17 +12204,14 @@
                  live_span: Optional[str] = None,
                  requests: Optional[Sequence['outputs.DashboardWidgetGroupDefinitionWidgetHeatmapDefinitionRequest']] = None,
                  show_legend: Optional[bool] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None,
                  yaxis: Optional['outputs.DashboardWidgetGroupDefinitionWidgetHeatmapDefinitionYaxis'] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if events is not None:
             pulumi.set(__self__, "events", events)
         if legend_size is not None:
             pulumi.set(__self__, "legend_size", legend_size)
         if live_span is not None:
@@ -12658,17 +12258,14 @@
     @pulumi.getter(name="showLegend")
     def show_legend(self) -> Optional[bool]:
         return pulumi.get(self, "show_legend")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -13813,17 +13410,14 @@
                  node_type: Optional[str] = None,
                  request: Optional['outputs.DashboardWidgetGroupDefinitionWidgetHostmapDefinitionRequest'] = None,
                  scopes: Optional[Sequence[str]] = None,
                  style: Optional['outputs.DashboardWidgetGroupDefinitionWidgetHostmapDefinitionStyle'] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if groups is not None:
             pulumi.set(__self__, "groups", groups)
         if no_group_hosts is not None:
             pulumi.set(__self__, "no_group_hosts", no_group_hosts)
         if no_metric_hosts is not None:
@@ -13882,17 +13476,14 @@
     @pulumi.getter
     def style(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetHostmapDefinitionStyle']:
         return pulumi.get(self, "style")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -15871,25 +15462,19 @@
         return pulumi.get(self, "palette_flip")
 
 
 @pulumi.output_type
 class DashboardWidgetGroupDefinitionWidgetIframeDefinition(dict):
     def __init__(__self__, *,
                  url: str):
-        """
-        :param str url: The URL of the dashboard.
-        """
         pulumi.set(__self__, "url", url)
 
     @property
     @pulumi.getter
     def url(self) -> str:
-        """
-        The URL of the dashboard.
-        """
         return pulumi.get(self, "url")
 
 
 @pulumi.output_type
 class DashboardWidgetGroupDefinitionWidgetImageDefinition(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -15921,17 +15506,14 @@
                  has_background: Optional[bool] = None,
                  has_border: Optional[bool] = None,
                  horizontal_align: Optional[str] = None,
                  margin: Optional[str] = None,
                  sizing: Optional[str] = None,
                  url_dark_theme: Optional[str] = None,
                  vertical_align: Optional[str] = None):
-        """
-        :param str url: The URL of the dashboard.
-        """
         pulumi.set(__self__, "url", url)
         if has_background is not None:
             pulumi.set(__self__, "has_background", has_background)
         if has_border is not None:
             pulumi.set(__self__, "has_border", has_border)
         if horizontal_align is not None:
             pulumi.set(__self__, "horizontal_align", horizontal_align)
@@ -15943,17 +15525,14 @@
             pulumi.set(__self__, "url_dark_theme", url_dark_theme)
         if vertical_align is not None:
             pulumi.set(__self__, "vertical_align", vertical_align)
 
     @property
     @pulumi.getter
     def url(self) -> str:
-        """
-        The URL of the dashboard.
-        """
         return pulumi.get(self, "url")
 
     @property
     @pulumi.getter(name="hasBackground")
     def has_background(self) -> Optional[bool]:
         return pulumi.get(self, "has_background")
 
@@ -16025,17 +15604,14 @@
                  query: Optional[str] = None,
                  show_date_column: Optional[bool] = None,
                  show_message_column: Optional[bool] = None,
                  sort: Optional['outputs.DashboardWidgetGroupDefinitionWidgetLogStreamDefinitionSort'] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         if columns is not None:
             pulumi.set(__self__, "columns", columns)
         if indexes is not None:
             pulumi.set(__self__, "indexes", indexes)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if message_display is not None:
@@ -16094,17 +15670,14 @@
     @pulumi.getter
     def sort(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetLogStreamDefinitionSort']:
         return pulumi.get(self, "sort")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -16171,17 +15744,14 @@
                  hide_zero_counts: Optional[bool] = None,
                  show_last_triggered: Optional[bool] = None,
                  sort: Optional[str] = None,
                  summary_type: Optional[str] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         pulumi.set(__self__, "query", query)
         if color_preference is not None:
             pulumi.set(__self__, "color_preference", color_preference)
         if display_format is not None:
             pulumi.set(__self__, "display_format", display_format)
         if hide_zero_counts is not None:
             pulumi.set(__self__, "hide_zero_counts", hide_zero_counts)
@@ -16232,17 +15802,14 @@
     @pulumi.getter(name="summaryType")
     def summary_type(self) -> Optional[str]:
         return pulumi.get(self, "summary_type")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -16390,17 +15957,14 @@
                  custom_links: Optional[Sequence['outputs.DashboardWidgetGroupDefinitionWidgetQueryTableDefinitionCustomLink']] = None,
                  has_search_bar: Optional[str] = None,
                  live_span: Optional[str] = None,
                  requests: Optional[Sequence['outputs.DashboardWidgetGroupDefinitionWidgetQueryTableDefinitionRequest']] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if has_search_bar is not None:
             pulumi.set(__self__, "has_search_bar", has_search_bar)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if requests is not None:
@@ -16431,17 +15995,14 @@
     @pulumi.getter
     def requests(self) -> Optional[Sequence['outputs.DashboardWidgetGroupDefinitionWidgetQueryTableDefinitionRequest']]:
         return pulumi.get(self, "requests")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -18515,14 +18076,16 @@
             suggest = "custom_links"
         elif key == "customUnit":
             suggest = "custom_unit"
         elif key == "liveSpan":
             suggest = "live_span"
         elif key == "textAlign":
             suggest = "text_align"
+        elif key == "timeseriesBackground":
+            suggest = "timeseries_background"
         elif key == "titleAlign":
             suggest = "title_align"
         elif key == "titleSize":
             suggest = "title_size"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in DashboardWidgetGroupDefinitionWidgetQueryValueDefinition. Access the value via the '{suggest}' property getter instead.")
@@ -18539,34 +18102,34 @@
                  autoscale: Optional[bool] = None,
                  custom_links: Optional[Sequence['outputs.DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionCustomLink']] = None,
                  custom_unit: Optional[str] = None,
                  live_span: Optional[str] = None,
                  precision: Optional[int] = None,
                  requests: Optional[Sequence['outputs.DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionRequest']] = None,
                  text_align: Optional[str] = None,
+                 timeseries_background: Optional['outputs.DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionTimeseriesBackground'] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         if autoscale is not None:
             pulumi.set(__self__, "autoscale", autoscale)
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if custom_unit is not None:
             pulumi.set(__self__, "custom_unit", custom_unit)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if precision is not None:
             pulumi.set(__self__, "precision", precision)
         if requests is not None:
             pulumi.set(__self__, "requests", requests)
         if text_align is not None:
             pulumi.set(__self__, "text_align", text_align)
+        if timeseries_background is not None:
+            pulumi.set(__self__, "timeseries_background", timeseries_background)
         if title is not None:
             pulumi.set(__self__, "title", title)
         if title_align is not None:
             pulumi.set(__self__, "title_align", title_align)
         if title_size is not None:
             pulumi.set(__self__, "title_size", title_size)
 
@@ -18602,19 +18165,21 @@
 
     @property
     @pulumi.getter(name="textAlign")
     def text_align(self) -> Optional[str]:
         return pulumi.get(self, "text_align")
 
     @property
+    @pulumi.getter(name="timeseriesBackground")
+    def timeseries_background(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionTimeseriesBackground']:
+        return pulumi.get(self, "timeseries_background")
+
+    @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -20710,14 +20275,96 @@
     @property
     @pulumi.getter
     def interval(self) -> Optional[int]:
         return pulumi.get(self, "interval")
 
 
 @pulumi.output_type
+class DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionTimeseriesBackground(dict):
+    def __init__(__self__, *,
+                 type: str,
+                 yaxis: Optional['outputs.DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionTimeseriesBackgroundYaxis'] = None):
+        pulumi.set(__self__, "type", type)
+        if yaxis is not None:
+            pulumi.set(__self__, "yaxis", yaxis)
+
+    @property
+    @pulumi.getter
+    def type(self) -> str:
+        return pulumi.get(self, "type")
+
+    @property
+    @pulumi.getter
+    def yaxis(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionTimeseriesBackgroundYaxis']:
+        return pulumi.get(self, "yaxis")
+
+
+@pulumi.output_type
+class DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionTimeseriesBackgroundYaxis(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "includeZero":
+            suggest = "include_zero"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionTimeseriesBackgroundYaxis. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionTimeseriesBackgroundYaxis.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        DashboardWidgetGroupDefinitionWidgetQueryValueDefinitionTimeseriesBackgroundYaxis.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 include_zero: Optional[bool] = None,
+                 label: Optional[str] = None,
+                 max: Optional[str] = None,
+                 min: Optional[str] = None,
+                 scale: Optional[str] = None):
+        if include_zero is not None:
+            pulumi.set(__self__, "include_zero", include_zero)
+        if label is not None:
+            pulumi.set(__self__, "label", label)
+        if max is not None:
+            pulumi.set(__self__, "max", max)
+        if min is not None:
+            pulumi.set(__self__, "min", min)
+        if scale is not None:
+            pulumi.set(__self__, "scale", scale)
+
+    @property
+    @pulumi.getter(name="includeZero")
+    def include_zero(self) -> Optional[bool]:
+        return pulumi.get(self, "include_zero")
+
+    @property
+    @pulumi.getter
+    def label(self) -> Optional[str]:
+        return pulumi.get(self, "label")
+
+    @property
+    @pulumi.getter
+    def max(self) -> Optional[str]:
+        return pulumi.get(self, "max")
+
+    @property
+    @pulumi.getter
+    def min(self) -> Optional[str]:
+        return pulumi.get(self, "min")
+
+    @property
+    @pulumi.getter
+    def scale(self) -> Optional[str]:
+        return pulumi.get(self, "scale")
+
+
+@pulumi.output_type
 class DashboardWidgetGroupDefinitionWidgetScatterplotDefinition(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "colorByGroups":
             suggest = "color_by_groups"
         elif key == "customLinks":
@@ -20746,17 +20393,14 @@
                  live_span: Optional[str] = None,
                  request: Optional['outputs.DashboardWidgetGroupDefinitionWidgetScatterplotDefinitionRequest'] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None,
                  xaxis: Optional['outputs.DashboardWidgetGroupDefinitionWidgetScatterplotDefinitionXaxis'] = None,
                  yaxis: Optional['outputs.DashboardWidgetGroupDefinitionWidgetScatterplotDefinitionYaxis'] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         if color_by_groups is not None:
             pulumi.set(__self__, "color_by_groups", color_by_groups)
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if request is not None:
@@ -20791,17 +20435,14 @@
     @pulumi.getter
     def request(self) -> Optional['outputs.DashboardWidgetGroupDefinitionWidgetScatterplotDefinitionRequest']:
         return pulumi.get(self, "request")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -23597,17 +23238,14 @@
                  view_mode: str,
                  view_type: str,
                  global_time_target: Optional[str] = None,
                  show_error_budget: Optional[bool] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         pulumi.set(__self__, "slo_id", slo_id)
         pulumi.set(__self__, "time_windows", time_windows)
         pulumi.set(__self__, "view_mode", view_mode)
         pulumi.set(__self__, "view_type", view_type)
         if global_time_target is not None:
             pulumi.set(__self__, "global_time_target", global_time_target)
         if show_error_budget is not None:
@@ -23648,17 +23286,14 @@
     @pulumi.getter(name="showErrorBudget")
     def show_error_budget(self) -> Optional[bool]:
         return pulumi.get(self, "show_error_budget")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -23694,17 +23329,14 @@
     def __init__(__self__, *,
                  filters: Sequence[str],
                  service: str,
                  custom_links: Optional[Sequence['outputs.DashboardWidgetGroupDefinitionWidgetServicemapDefinitionCustomLink']] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         pulumi.set(__self__, "filters", filters)
         pulumi.set(__self__, "service", service)
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if title is not None:
             pulumi.set(__self__, "title", title)
         if title_align is not None:
@@ -23726,17 +23358,14 @@
     @pulumi.getter(name="customLinks")
     def custom_links(self) -> Optional[Sequence['outputs.DashboardWidgetGroupDefinitionWidgetServicemapDefinitionCustomLink']]:
         return pulumi.get(self, "custom_links")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -23839,17 +23468,14 @@
                  legend_inline: Optional['outputs.DashboardWidgetGroupDefinitionWidgetSunburstDefinitionLegendInline'] = None,
                  legend_table: Optional['outputs.DashboardWidgetGroupDefinitionWidgetSunburstDefinitionLegendTable'] = None,
                  live_span: Optional[str] = None,
                  requests: Optional[Sequence['outputs.DashboardWidgetGroupDefinitionWidgetSunburstDefinitionRequest']] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if hide_total is not None:
             pulumi.set(__self__, "hide_total", hide_total)
         if legend_inline is not None:
             pulumi.set(__self__, "legend_inline", legend_inline)
         if legend_table is not None:
@@ -23894,17 +23520,14 @@
     @pulumi.getter
     def requests(self) -> Optional[Sequence['outputs.DashboardWidgetGroupDefinitionWidgetSunburstDefinitionRequest']]:
         return pulumi.get(self, "requests")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -26199,17 +25822,14 @@
                  requests: Optional[Sequence['outputs.DashboardWidgetGroupDefinitionWidgetTimeseriesDefinitionRequest']] = None,
                  right_yaxis: Optional['outputs.DashboardWidgetGroupDefinitionWidgetTimeseriesDefinitionRightYaxis'] = None,
                  show_legend: Optional[bool] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None,
                  yaxis: Optional['outputs.DashboardWidgetGroupDefinitionWidgetTimeseriesDefinitionYaxis'] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if events is not None:
             pulumi.set(__self__, "events", events)
         if legend_columns is not None:
             pulumi.set(__self__, "legend_columns", legend_columns)
         if legend_layout is not None:
@@ -26284,17 +25904,14 @@
     @pulumi.getter(name="showLegend")
     def show_legend(self) -> Optional[bool]:
         return pulumi.get(self, "show_legend")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -28844,17 +28461,14 @@
     def __init__(__self__, *,
                  custom_links: Optional[Sequence['outputs.DashboardWidgetGroupDefinitionWidgetToplistDefinitionCustomLink']] = None,
                  live_span: Optional[str] = None,
                  requests: Optional[Sequence['outputs.DashboardWidgetGroupDefinitionWidgetToplistDefinitionRequest']] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if requests is not None:
             pulumi.set(__self__, "requests", requests)
         if title is not None:
@@ -28878,17 +28492,14 @@
     @pulumi.getter
     def requests(self) -> Optional[Sequence['outputs.DashboardWidgetGroupDefinitionWidgetToplistDefinitionRequest']]:
         return pulumi.get(self, "requests")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -31053,17 +30664,14 @@
                  show_hits: Optional[bool] = None,
                  show_latency: Optional[bool] = None,
                  show_resource_list: Optional[bool] = None,
                  size_format: Optional[str] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         pulumi.set(__self__, "env", env)
         pulumi.set(__self__, "service", service)
         pulumi.set(__self__, "span_name", span_name)
         if display_format is not None:
             pulumi.set(__self__, "display_format", display_format)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
@@ -31147,17 +30755,14 @@
     @pulumi.getter(name="sizeFormat")
     def size_format(self) -> Optional[str]:
         return pulumi.get(self, "size_format")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -31168,33 +30773,27 @@
 
 
 @pulumi.output_type
 class DashboardWidgetGroupDefinitionWidgetTreemapDefinition(dict):
     def __init__(__self__, *,
                  requests: Optional[Sequence['outputs.DashboardWidgetGroupDefinitionWidgetTreemapDefinitionRequest']] = None,
                  title: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         if requests is not None:
             pulumi.set(__self__, "requests", requests)
         if title is not None:
             pulumi.set(__self__, "title", title)
 
     @property
     @pulumi.getter
     def requests(self) -> Optional[Sequence['outputs.DashboardWidgetGroupDefinitionWidgetTreemapDefinitionRequest']]:
         return pulumi.get(self, "requests")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
 
 @pulumi.output_type
 class DashboardWidgetGroupDefinitionWidgetTreemapDefinitionRequest(dict):
     def __init__(__self__, *,
                  formulas: Optional[Sequence['outputs.DashboardWidgetGroupDefinitionWidgetTreemapDefinitionRequestFormula']] = None,
@@ -32088,17 +31687,14 @@
                  live_span: Optional[str] = None,
                  requests: Optional[Sequence['outputs.DashboardWidgetHeatmapDefinitionRequest']] = None,
                  show_legend: Optional[bool] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None,
                  yaxis: Optional['outputs.DashboardWidgetHeatmapDefinitionYaxis'] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if events is not None:
             pulumi.set(__self__, "events", events)
         if legend_size is not None:
             pulumi.set(__self__, "legend_size", legend_size)
         if live_span is not None:
@@ -32145,17 +31741,14 @@
     @pulumi.getter(name="showLegend")
     def show_legend(self) -> Optional[bool]:
         return pulumi.get(self, "show_legend")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -33300,17 +32893,14 @@
                  node_type: Optional[str] = None,
                  request: Optional['outputs.DashboardWidgetHostmapDefinitionRequest'] = None,
                  scopes: Optional[Sequence[str]] = None,
                  style: Optional['outputs.DashboardWidgetHostmapDefinitionStyle'] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if groups is not None:
             pulumi.set(__self__, "groups", groups)
         if no_group_hosts is not None:
             pulumi.set(__self__, "no_group_hosts", no_group_hosts)
         if no_metric_hosts is not None:
@@ -33369,17 +32959,14 @@
     @pulumi.getter
     def style(self) -> Optional['outputs.DashboardWidgetHostmapDefinitionStyle']:
         return pulumi.get(self, "style")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -35358,25 +34945,19 @@
         return pulumi.get(self, "palette_flip")
 
 
 @pulumi.output_type
 class DashboardWidgetIframeDefinition(dict):
     def __init__(__self__, *,
                  url: str):
-        """
-        :param str url: The URL of the dashboard.
-        """
         pulumi.set(__self__, "url", url)
 
     @property
     @pulumi.getter
     def url(self) -> str:
-        """
-        The URL of the dashboard.
-        """
         return pulumi.get(self, "url")
 
 
 @pulumi.output_type
 class DashboardWidgetImageDefinition(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -35408,17 +34989,14 @@
                  has_background: Optional[bool] = None,
                  has_border: Optional[bool] = None,
                  horizontal_align: Optional[str] = None,
                  margin: Optional[str] = None,
                  sizing: Optional[str] = None,
                  url_dark_theme: Optional[str] = None,
                  vertical_align: Optional[str] = None):
-        """
-        :param str url: The URL of the dashboard.
-        """
         pulumi.set(__self__, "url", url)
         if has_background is not None:
             pulumi.set(__self__, "has_background", has_background)
         if has_border is not None:
             pulumi.set(__self__, "has_border", has_border)
         if horizontal_align is not None:
             pulumi.set(__self__, "horizontal_align", horizontal_align)
@@ -35430,17 +35008,14 @@
             pulumi.set(__self__, "url_dark_theme", url_dark_theme)
         if vertical_align is not None:
             pulumi.set(__self__, "vertical_align", vertical_align)
 
     @property
     @pulumi.getter
     def url(self) -> str:
-        """
-        The URL of the dashboard.
-        """
         return pulumi.get(self, "url")
 
     @property
     @pulumi.getter(name="hasBackground")
     def has_background(self) -> Optional[bool]:
         return pulumi.get(self, "has_background")
 
@@ -35512,17 +35087,14 @@
                  query: Optional[str] = None,
                  show_date_column: Optional[bool] = None,
                  show_message_column: Optional[bool] = None,
                  sort: Optional['outputs.DashboardWidgetLogStreamDefinitionSort'] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         if columns is not None:
             pulumi.set(__self__, "columns", columns)
         if indexes is not None:
             pulumi.set(__self__, "indexes", indexes)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if message_display is not None:
@@ -35581,17 +35153,14 @@
     @pulumi.getter
     def sort(self) -> Optional['outputs.DashboardWidgetLogStreamDefinitionSort']:
         return pulumi.get(self, "sort")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -35658,17 +35227,14 @@
                  hide_zero_counts: Optional[bool] = None,
                  show_last_triggered: Optional[bool] = None,
                  sort: Optional[str] = None,
                  summary_type: Optional[str] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         pulumi.set(__self__, "query", query)
         if color_preference is not None:
             pulumi.set(__self__, "color_preference", color_preference)
         if display_format is not None:
             pulumi.set(__self__, "display_format", display_format)
         if hide_zero_counts is not None:
             pulumi.set(__self__, "hide_zero_counts", hide_zero_counts)
@@ -35719,17 +35285,14 @@
     @pulumi.getter(name="summaryType")
     def summary_type(self) -> Optional[str]:
         return pulumi.get(self, "summary_type")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -35877,17 +35440,14 @@
                  custom_links: Optional[Sequence['outputs.DashboardWidgetQueryTableDefinitionCustomLink']] = None,
                  has_search_bar: Optional[str] = None,
                  live_span: Optional[str] = None,
                  requests: Optional[Sequence['outputs.DashboardWidgetQueryTableDefinitionRequest']] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if has_search_bar is not None:
             pulumi.set(__self__, "has_search_bar", has_search_bar)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if requests is not None:
@@ -35918,17 +35478,14 @@
     @pulumi.getter
     def requests(self) -> Optional[Sequence['outputs.DashboardWidgetQueryTableDefinitionRequest']]:
         return pulumi.get(self, "requests")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -38002,14 +37559,16 @@
             suggest = "custom_links"
         elif key == "customUnit":
             suggest = "custom_unit"
         elif key == "liveSpan":
             suggest = "live_span"
         elif key == "textAlign":
             suggest = "text_align"
+        elif key == "timeseriesBackground":
+            suggest = "timeseries_background"
         elif key == "titleAlign":
             suggest = "title_align"
         elif key == "titleSize":
             suggest = "title_size"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in DashboardWidgetQueryValueDefinition. Access the value via the '{suggest}' property getter instead.")
@@ -38026,34 +37585,34 @@
                  autoscale: Optional[bool] = None,
                  custom_links: Optional[Sequence['outputs.DashboardWidgetQueryValueDefinitionCustomLink']] = None,
                  custom_unit: Optional[str] = None,
                  live_span: Optional[str] = None,
                  precision: Optional[int] = None,
                  requests: Optional[Sequence['outputs.DashboardWidgetQueryValueDefinitionRequest']] = None,
                  text_align: Optional[str] = None,
+                 timeseries_background: Optional['outputs.DashboardWidgetQueryValueDefinitionTimeseriesBackground'] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         if autoscale is not None:
             pulumi.set(__self__, "autoscale", autoscale)
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if custom_unit is not None:
             pulumi.set(__self__, "custom_unit", custom_unit)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if precision is not None:
             pulumi.set(__self__, "precision", precision)
         if requests is not None:
             pulumi.set(__self__, "requests", requests)
         if text_align is not None:
             pulumi.set(__self__, "text_align", text_align)
+        if timeseries_background is not None:
+            pulumi.set(__self__, "timeseries_background", timeseries_background)
         if title is not None:
             pulumi.set(__self__, "title", title)
         if title_align is not None:
             pulumi.set(__self__, "title_align", title_align)
         if title_size is not None:
             pulumi.set(__self__, "title_size", title_size)
 
@@ -38089,19 +37648,21 @@
 
     @property
     @pulumi.getter(name="textAlign")
     def text_align(self) -> Optional[str]:
         return pulumi.get(self, "text_align")
 
     @property
+    @pulumi.getter(name="timeseriesBackground")
+    def timeseries_background(self) -> Optional['outputs.DashboardWidgetQueryValueDefinitionTimeseriesBackground']:
+        return pulumi.get(self, "timeseries_background")
+
+    @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -40197,14 +39758,96 @@
     @property
     @pulumi.getter
     def interval(self) -> Optional[int]:
         return pulumi.get(self, "interval")
 
 
 @pulumi.output_type
+class DashboardWidgetQueryValueDefinitionTimeseriesBackground(dict):
+    def __init__(__self__, *,
+                 type: str,
+                 yaxis: Optional['outputs.DashboardWidgetQueryValueDefinitionTimeseriesBackgroundYaxis'] = None):
+        pulumi.set(__self__, "type", type)
+        if yaxis is not None:
+            pulumi.set(__self__, "yaxis", yaxis)
+
+    @property
+    @pulumi.getter
+    def type(self) -> str:
+        return pulumi.get(self, "type")
+
+    @property
+    @pulumi.getter
+    def yaxis(self) -> Optional['outputs.DashboardWidgetQueryValueDefinitionTimeseriesBackgroundYaxis']:
+        return pulumi.get(self, "yaxis")
+
+
+@pulumi.output_type
+class DashboardWidgetQueryValueDefinitionTimeseriesBackgroundYaxis(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "includeZero":
+            suggest = "include_zero"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in DashboardWidgetQueryValueDefinitionTimeseriesBackgroundYaxis. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        DashboardWidgetQueryValueDefinitionTimeseriesBackgroundYaxis.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        DashboardWidgetQueryValueDefinitionTimeseriesBackgroundYaxis.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 include_zero: Optional[bool] = None,
+                 label: Optional[str] = None,
+                 max: Optional[str] = None,
+                 min: Optional[str] = None,
+                 scale: Optional[str] = None):
+        if include_zero is not None:
+            pulumi.set(__self__, "include_zero", include_zero)
+        if label is not None:
+            pulumi.set(__self__, "label", label)
+        if max is not None:
+            pulumi.set(__self__, "max", max)
+        if min is not None:
+            pulumi.set(__self__, "min", min)
+        if scale is not None:
+            pulumi.set(__self__, "scale", scale)
+
+    @property
+    @pulumi.getter(name="includeZero")
+    def include_zero(self) -> Optional[bool]:
+        return pulumi.get(self, "include_zero")
+
+    @property
+    @pulumi.getter
+    def label(self) -> Optional[str]:
+        return pulumi.get(self, "label")
+
+    @property
+    @pulumi.getter
+    def max(self) -> Optional[str]:
+        return pulumi.get(self, "max")
+
+    @property
+    @pulumi.getter
+    def min(self) -> Optional[str]:
+        return pulumi.get(self, "min")
+
+    @property
+    @pulumi.getter
+    def scale(self) -> Optional[str]:
+        return pulumi.get(self, "scale")
+
+
+@pulumi.output_type
 class DashboardWidgetScatterplotDefinition(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "colorByGroups":
             suggest = "color_by_groups"
         elif key == "customLinks":
@@ -40233,17 +39876,14 @@
                  live_span: Optional[str] = None,
                  request: Optional['outputs.DashboardWidgetScatterplotDefinitionRequest'] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None,
                  xaxis: Optional['outputs.DashboardWidgetScatterplotDefinitionXaxis'] = None,
                  yaxis: Optional['outputs.DashboardWidgetScatterplotDefinitionYaxis'] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         if color_by_groups is not None:
             pulumi.set(__self__, "color_by_groups", color_by_groups)
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if request is not None:
@@ -40278,17 +39918,14 @@
     @pulumi.getter
     def request(self) -> Optional['outputs.DashboardWidgetScatterplotDefinitionRequest']:
         return pulumi.get(self, "request")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -43084,17 +42721,14 @@
                  view_mode: str,
                  view_type: str,
                  global_time_target: Optional[str] = None,
                  show_error_budget: Optional[bool] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         pulumi.set(__self__, "slo_id", slo_id)
         pulumi.set(__self__, "time_windows", time_windows)
         pulumi.set(__self__, "view_mode", view_mode)
         pulumi.set(__self__, "view_type", view_type)
         if global_time_target is not None:
             pulumi.set(__self__, "global_time_target", global_time_target)
         if show_error_budget is not None:
@@ -43135,17 +42769,14 @@
     @pulumi.getter(name="showErrorBudget")
     def show_error_budget(self) -> Optional[bool]:
         return pulumi.get(self, "show_error_budget")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -43181,17 +42812,14 @@
     def __init__(__self__, *,
                  filters: Sequence[str],
                  service: str,
                  custom_links: Optional[Sequence['outputs.DashboardWidgetServicemapDefinitionCustomLink']] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         pulumi.set(__self__, "filters", filters)
         pulumi.set(__self__, "service", service)
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if title is not None:
             pulumi.set(__self__, "title", title)
         if title_align is not None:
@@ -43213,17 +42841,14 @@
     @pulumi.getter(name="customLinks")
     def custom_links(self) -> Optional[Sequence['outputs.DashboardWidgetServicemapDefinitionCustomLink']]:
         return pulumi.get(self, "custom_links")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -43326,17 +42951,14 @@
                  legend_inline: Optional['outputs.DashboardWidgetSunburstDefinitionLegendInline'] = None,
                  legend_table: Optional['outputs.DashboardWidgetSunburstDefinitionLegendTable'] = None,
                  live_span: Optional[str] = None,
                  requests: Optional[Sequence['outputs.DashboardWidgetSunburstDefinitionRequest']] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if hide_total is not None:
             pulumi.set(__self__, "hide_total", hide_total)
         if legend_inline is not None:
             pulumi.set(__self__, "legend_inline", legend_inline)
         if legend_table is not None:
@@ -43381,17 +43003,14 @@
     @pulumi.getter
     def requests(self) -> Optional[Sequence['outputs.DashboardWidgetSunburstDefinitionRequest']]:
         return pulumi.get(self, "requests")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -45686,17 +45305,14 @@
                  requests: Optional[Sequence['outputs.DashboardWidgetTimeseriesDefinitionRequest']] = None,
                  right_yaxis: Optional['outputs.DashboardWidgetTimeseriesDefinitionRightYaxis'] = None,
                  show_legend: Optional[bool] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None,
                  yaxis: Optional['outputs.DashboardWidgetTimeseriesDefinitionYaxis'] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if events is not None:
             pulumi.set(__self__, "events", events)
         if legend_columns is not None:
             pulumi.set(__self__, "legend_columns", legend_columns)
         if legend_layout is not None:
@@ -45771,17 +45387,14 @@
     @pulumi.getter(name="showLegend")
     def show_legend(self) -> Optional[bool]:
         return pulumi.get(self, "show_legend")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -48331,17 +47944,14 @@
     def __init__(__self__, *,
                  custom_links: Optional[Sequence['outputs.DashboardWidgetToplistDefinitionCustomLink']] = None,
                  live_span: Optional[str] = None,
                  requests: Optional[Sequence['outputs.DashboardWidgetToplistDefinitionRequest']] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         if custom_links is not None:
             pulumi.set(__self__, "custom_links", custom_links)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
         if requests is not None:
             pulumi.set(__self__, "requests", requests)
         if title is not None:
@@ -48365,17 +47975,14 @@
     @pulumi.getter
     def requests(self) -> Optional[Sequence['outputs.DashboardWidgetToplistDefinitionRequest']]:
         return pulumi.get(self, "requests")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -50540,17 +50147,14 @@
                  show_hits: Optional[bool] = None,
                  show_latency: Optional[bool] = None,
                  show_resource_list: Optional[bool] = None,
                  size_format: Optional[str] = None,
                  title: Optional[str] = None,
                  title_align: Optional[str] = None,
                  title_size: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         pulumi.set(__self__, "env", env)
         pulumi.set(__self__, "service", service)
         pulumi.set(__self__, "span_name", span_name)
         if display_format is not None:
             pulumi.set(__self__, "display_format", display_format)
         if live_span is not None:
             pulumi.set(__self__, "live_span", live_span)
@@ -50634,17 +50238,14 @@
     @pulumi.getter(name="sizeFormat")
     def size_format(self) -> Optional[str]:
         return pulumi.get(self, "size_format")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="titleAlign")
     def title_align(self) -> Optional[str]:
         return pulumi.get(self, "title_align")
 
@@ -50655,33 +50256,27 @@
 
 
 @pulumi.output_type
 class DashboardWidgetTreemapDefinition(dict):
     def __init__(__self__, *,
                  requests: Optional[Sequence['outputs.DashboardWidgetTreemapDefinitionRequest']] = None,
                  title: Optional[str] = None):
-        """
-        :param str title: The title of the dashboard.
-        """
         if requests is not None:
             pulumi.set(__self__, "requests", requests)
         if title is not None:
             pulumi.set(__self__, "title", title)
 
     @property
     @pulumi.getter
     def requests(self) -> Optional[Sequence['outputs.DashboardWidgetTreemapDefinitionRequest']]:
         return pulumi.get(self, "requests")
 
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
-        """
-        The title of the dashboard.
-        """
         return pulumi.get(self, "title")
 
 
 @pulumi.output_type
 class DashboardWidgetTreemapDefinitionRequest(dict):
     def __init__(__self__, *,
                  formulas: Optional[Sequence['outputs.DashboardWidgetTreemapDefinitionRequestFormula']] = None,
@@ -51565,22 +51160,14 @@
     def __init__(__self__, *,
                  type: str,
                  period: Optional[int] = None,
                  rrule: Optional[str] = None,
                  until_date: Optional[int] = None,
                  until_occurrences: Optional[int] = None,
                  week_days: Optional[Sequence[str]] = None):
-        """
-        :param str type: One of `days`, `weeks`, `months`, or `years`
-        :param int period: How often to repeat as an integer. For example to repeat every 3 days, select a `type` of `days` and a `period` of `3`.
-        :param str rrule: The RRULE standard for defining recurring events. For example, to have a recurring event on the first day of each month, use `FREQ=MONTHLY;INTERVAL=1`. Most common rrule options from the iCalendar Spec are supported. Attributes specifying the duration in RRULE are not supported (for example, `DTSTART`, `DTEND`, `DURATION`).
-        :param int until_date: The date at which the recurrence should end as a POSIX timestamp. `until_occurrences` and `until_date` are mutually exclusive.
-        :param int until_occurrences: How many times the downtime will be rescheduled. `until_occurrences` and `until_date` are mutually exclusive.
-        :param Sequence[str] week_days: A list of week days to repeat on. Choose from: `Mon`, `Tue`, `Wed`, `Thu`, `Fri`, `Sat` or `Sun`. Only applicable when `type` is `weeks`. First letter must be capitalized.
-        """
         pulumi.set(__self__, "type", type)
         if period is not None:
             pulumi.set(__self__, "period", period)
         if rrule is not None:
             pulumi.set(__self__, "rrule", rrule)
         if until_date is not None:
             pulumi.set(__self__, "until_date", until_date)
@@ -51588,57 +51175,39 @@
             pulumi.set(__self__, "until_occurrences", until_occurrences)
         if week_days is not None:
             pulumi.set(__self__, "week_days", week_days)
 
     @property
     @pulumi.getter
     def type(self) -> str:
-        """
-        One of `days`, `weeks`, `months`, or `years`
-        """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def period(self) -> Optional[int]:
-        """
-        How often to repeat as an integer. For example to repeat every 3 days, select a `type` of `days` and a `period` of `3`.
-        """
         return pulumi.get(self, "period")
 
     @property
     @pulumi.getter
     def rrule(self) -> Optional[str]:
-        """
-        The RRULE standard for defining recurring events. For example, to have a recurring event on the first day of each month, use `FREQ=MONTHLY;INTERVAL=1`. Most common rrule options from the iCalendar Spec are supported. Attributes specifying the duration in RRULE are not supported (for example, `DTSTART`, `DTEND`, `DURATION`).
-        """
         return pulumi.get(self, "rrule")
 
     @property
     @pulumi.getter(name="untilDate")
     def until_date(self) -> Optional[int]:
-        """
-        The date at which the recurrence should end as a POSIX timestamp. `until_occurrences` and `until_date` are mutually exclusive.
-        """
         return pulumi.get(self, "until_date")
 
     @property
     @pulumi.getter(name="untilOccurrences")
     def until_occurrences(self) -> Optional[int]:
-        """
-        How many times the downtime will be rescheduled. `until_occurrences` and `until_date` are mutually exclusive.
-        """
         return pulumi.get(self, "until_occurrences")
 
     @property
     @pulumi.getter(name="weekDays")
     def week_days(self) -> Optional[Sequence[str]]:
-        """
-        A list of week days to repeat on. Choose from: `Mon`, `Tue`, `Wed`, `Thu`, `Fri`, `Sat` or `Sun`. Only applicable when `type` is `weeks`. First letter must be capitalized.
-        """
         return pulumi.get(self, "week_days")
 
 
 @pulumi.output_type
 class LogsArchiveAzureArchive(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -51663,66 +51232,44 @@
 
     def __init__(__self__, *,
                  client_id: str,
                  container: str,
                  storage_account: str,
                  tenant_id: str,
                  path: Optional[str] = None):
-        """
-        :param str client_id: Your client id.
-        :param str container: The container where the archive will be stored.
-        :param str storage_account: The associated storage account.
-        :param str tenant_id: Your tenant id.
-        :param str path: The path where the archive will be stored.
-        """
         pulumi.set(__self__, "client_id", client_id)
         pulumi.set(__self__, "container", container)
         pulumi.set(__self__, "storage_account", storage_account)
         pulumi.set(__self__, "tenant_id", tenant_id)
         if path is not None:
             pulumi.set(__self__, "path", path)
 
     @property
     @pulumi.getter(name="clientId")
     def client_id(self) -> str:
-        """
-        Your client id.
-        """
         return pulumi.get(self, "client_id")
 
     @property
     @pulumi.getter
     def container(self) -> str:
-        """
-        The container where the archive will be stored.
-        """
         return pulumi.get(self, "container")
 
     @property
     @pulumi.getter(name="storageAccount")
     def storage_account(self) -> str:
-        """
-        The associated storage account.
-        """
         return pulumi.get(self, "storage_account")
 
     @property
     @pulumi.getter(name="tenantId")
     def tenant_id(self) -> str:
-        """
-        Your tenant id.
-        """
         return pulumi.get(self, "tenant_id")
 
     @property
     @pulumi.getter
     def path(self) -> Optional[str]:
-        """
-        The path where the archive will be stored.
-        """
         return pulumi.get(self, "path")
 
 
 @pulumi.output_type
 class LogsArchiveGcsArchive(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -51744,55 +51291,37 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  bucket: str,
                  client_email: str,
                  path: str,
                  project_id: str):
-        """
-        :param str bucket: Name of your GCS bucket.
-        :param str client_email: Your client email.
-        :param str path: Path where the archive will be stored.
-        :param str project_id: Your project id.
-        """
         pulumi.set(__self__, "bucket", bucket)
         pulumi.set(__self__, "client_email", client_email)
         pulumi.set(__self__, "path", path)
         pulumi.set(__self__, "project_id", project_id)
 
     @property
     @pulumi.getter
     def bucket(self) -> str:
-        """
-        Name of your GCS bucket.
-        """
         return pulumi.get(self, "bucket")
 
     @property
     @pulumi.getter(name="clientEmail")
     def client_email(self) -> str:
-        """
-        Your client email.
-        """
         return pulumi.get(self, "client_email")
 
     @property
     @pulumi.getter
     def path(self) -> str:
-        """
-        Path where the archive will be stored.
-        """
         return pulumi.get(self, "path")
 
     @property
     @pulumi.getter(name="projectId")
     def project_id(self) -> str:
-        """
-        Your project id.
-        """
         return pulumi.get(self, "project_id")
 
 
 @pulumi.output_type
 class LogsArchiveS3Archive(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -51814,73 +51343,49 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  account_id: str,
                  bucket: str,
                  path: str,
                  role_name: str):
-        """
-        :param str account_id: Your AWS account id.
-        :param str bucket: Name of your s3 bucket.
-        :param str path: Path where the archive will be stored.
-        :param str role_name: Your AWS role name
-        """
         pulumi.set(__self__, "account_id", account_id)
         pulumi.set(__self__, "bucket", bucket)
         pulumi.set(__self__, "path", path)
         pulumi.set(__self__, "role_name", role_name)
 
     @property
     @pulumi.getter(name="accountId")
     def account_id(self) -> str:
-        """
-        Your AWS account id.
-        """
         return pulumi.get(self, "account_id")
 
     @property
     @pulumi.getter
     def bucket(self) -> str:
-        """
-        Name of your s3 bucket.
-        """
         return pulumi.get(self, "bucket")
 
     @property
     @pulumi.getter
     def path(self) -> str:
-        """
-        Path where the archive will be stored.
-        """
         return pulumi.get(self, "path")
 
     @property
     @pulumi.getter(name="roleName")
     def role_name(self) -> str:
-        """
-        Your AWS role name
-        """
         return pulumi.get(self, "role_name")
 
 
 @pulumi.output_type
 class LogsCustomPipelineFilter(dict):
     def __init__(__self__, *,
                  query: str):
-        """
-        :param str query: Filter criteria of the category.
-        """
         pulumi.set(__self__, "query", query)
 
     @property
     @pulumi.getter
     def query(self) -> str:
-        """
-        Filter criteria of the category.
-        """
         return pulumi.get(self, "query")
 
 
 @pulumi.output_type
 class LogsCustomPipelineProcessor(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -51937,30 +51442,14 @@
                  pipeline: Optional['outputs.LogsCustomPipelineProcessorPipeline'] = None,
                  service_remapper: Optional['outputs.LogsCustomPipelineProcessorServiceRemapper'] = None,
                  status_remapper: Optional['outputs.LogsCustomPipelineProcessorStatusRemapper'] = None,
                  string_builder_processor: Optional['outputs.LogsCustomPipelineProcessorStringBuilderProcessor'] = None,
                  trace_id_remapper: Optional['outputs.LogsCustomPipelineProcessorTraceIdRemapper'] = None,
                  url_parser: Optional['outputs.LogsCustomPipelineProcessorUrlParser'] = None,
                  user_agent_parser: Optional['outputs.LogsCustomPipelineProcessorUserAgentParser'] = None):
-        """
-        :param 'LogsCustomPipelineProcessorArithmeticProcessorArgs' arithmetic_processor: Arithmetic Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#arithmetic-processor)
-        :param 'LogsCustomPipelineProcessorAttributeRemapperArgs' attribute_remapper: Attribute Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#remapper)
-        :param 'LogsCustomPipelineProcessorCategoryProcessorArgs' category_processor: Category Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#category-processor)
-        :param 'LogsCustomPipelineProcessorDateRemapperArgs' date_remapper: Date Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#log-date-remapper)
-        :param 'LogsCustomPipelineProcessorGeoIpParserArgs' geo_ip_parser: Date GeoIP Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#geoip-parser)
-        :param 'LogsCustomPipelineProcessorGrokParserArgs' grok_parser: Grok Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#grok-parser)
-        :param 'LogsCustomPipelineProcessorLookupProcessorArgs' lookup_processor: Lookup Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#lookup-processor)
-        :param 'LogsCustomPipelineProcessorMessageRemapperArgs' message_remapper: Message Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#log-message-remapper)
-        :param 'LogsCustomPipelineProcessorServiceRemapperArgs' service_remapper: Service Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#service-remapper)
-        :param 'LogsCustomPipelineProcessorStatusRemapperArgs' status_remapper: Status Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#log-status-remapper)
-        :param 'LogsCustomPipelineProcessorStringBuilderProcessorArgs' string_builder_processor: String Builder Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#string-builder-processor)
-        :param 'LogsCustomPipelineProcessorTraceIdRemapperArgs' trace_id_remapper: Trace ID Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#trace-remapper)
-        :param 'LogsCustomPipelineProcessorUrlParserArgs' url_parser: URL Parser Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#url-parser)
-        :param 'LogsCustomPipelineProcessorUserAgentParserArgs' user_agent_parser: User-Agent Parser Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#user-agent-parser)
-        """
         if arithmetic_processor is not None:
             pulumi.set(__self__, "arithmetic_processor", arithmetic_processor)
         if attribute_remapper is not None:
             pulumi.set(__self__, "attribute_remapper", attribute_remapper)
         if category_processor is not None:
             pulumi.set(__self__, "category_processor", category_processor)
         if date_remapper is not None:
@@ -51987,126 +51476,84 @@
             pulumi.set(__self__, "url_parser", url_parser)
         if user_agent_parser is not None:
             pulumi.set(__self__, "user_agent_parser", user_agent_parser)
 
     @property
     @pulumi.getter(name="arithmeticProcessor")
     def arithmetic_processor(self) -> Optional['outputs.LogsCustomPipelineProcessorArithmeticProcessor']:
-        """
-        Arithmetic Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#arithmetic-processor)
-        """
         return pulumi.get(self, "arithmetic_processor")
 
     @property
     @pulumi.getter(name="attributeRemapper")
     def attribute_remapper(self) -> Optional['outputs.LogsCustomPipelineProcessorAttributeRemapper']:
-        """
-        Attribute Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#remapper)
-        """
         return pulumi.get(self, "attribute_remapper")
 
     @property
     @pulumi.getter(name="categoryProcessor")
     def category_processor(self) -> Optional['outputs.LogsCustomPipelineProcessorCategoryProcessor']:
-        """
-        Category Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#category-processor)
-        """
         return pulumi.get(self, "category_processor")
 
     @property
     @pulumi.getter(name="dateRemapper")
     def date_remapper(self) -> Optional['outputs.LogsCustomPipelineProcessorDateRemapper']:
-        """
-        Date Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#log-date-remapper)
-        """
         return pulumi.get(self, "date_remapper")
 
     @property
     @pulumi.getter(name="geoIpParser")
     def geo_ip_parser(self) -> Optional['outputs.LogsCustomPipelineProcessorGeoIpParser']:
-        """
-        Date GeoIP Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#geoip-parser)
-        """
         return pulumi.get(self, "geo_ip_parser")
 
     @property
     @pulumi.getter(name="grokParser")
     def grok_parser(self) -> Optional['outputs.LogsCustomPipelineProcessorGrokParser']:
-        """
-        Grok Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#grok-parser)
-        """
         return pulumi.get(self, "grok_parser")
 
     @property
     @pulumi.getter(name="lookupProcessor")
     def lookup_processor(self) -> Optional['outputs.LogsCustomPipelineProcessorLookupProcessor']:
-        """
-        Lookup Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#lookup-processor)
-        """
         return pulumi.get(self, "lookup_processor")
 
     @property
     @pulumi.getter(name="messageRemapper")
     def message_remapper(self) -> Optional['outputs.LogsCustomPipelineProcessorMessageRemapper']:
-        """
-        Message Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#log-message-remapper)
-        """
         return pulumi.get(self, "message_remapper")
 
     @property
     @pulumi.getter
     def pipeline(self) -> Optional['outputs.LogsCustomPipelineProcessorPipeline']:
         return pulumi.get(self, "pipeline")
 
     @property
     @pulumi.getter(name="serviceRemapper")
     def service_remapper(self) -> Optional['outputs.LogsCustomPipelineProcessorServiceRemapper']:
-        """
-        Service Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#service-remapper)
-        """
         return pulumi.get(self, "service_remapper")
 
     @property
     @pulumi.getter(name="statusRemapper")
     def status_remapper(self) -> Optional['outputs.LogsCustomPipelineProcessorStatusRemapper']:
-        """
-        Status Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#log-status-remapper)
-        """
         return pulumi.get(self, "status_remapper")
 
     @property
     @pulumi.getter(name="stringBuilderProcessor")
     def string_builder_processor(self) -> Optional['outputs.LogsCustomPipelineProcessorStringBuilderProcessor']:
-        """
-        String Builder Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#string-builder-processor)
-        """
         return pulumi.get(self, "string_builder_processor")
 
     @property
     @pulumi.getter(name="traceIdRemapper")
     def trace_id_remapper(self) -> Optional['outputs.LogsCustomPipelineProcessorTraceIdRemapper']:
-        """
-        Trace ID Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#trace-remapper)
-        """
         return pulumi.get(self, "trace_id_remapper")
 
     @property
     @pulumi.getter(name="urlParser")
     def url_parser(self) -> Optional['outputs.LogsCustomPipelineProcessorUrlParser']:
-        """
-        URL Parser Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#url-parser)
-        """
         return pulumi.get(self, "url_parser")
 
     @property
     @pulumi.getter(name="userAgentParser")
     def user_agent_parser(self) -> Optional['outputs.LogsCustomPipelineProcessorUserAgentParser']:
-        """
-        User-Agent Parser Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#user-agent-parser)
-        """
         return pulumi.get(self, "user_agent_parser")
 
 
 @pulumi.output_type
 class LogsCustomPipelineProcessorArithmeticProcessor(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -52339,25 +51786,19 @@
         return pulumi.get(self, "name")
 
 
 @pulumi.output_type
 class LogsCustomPipelineProcessorCategoryProcessorCategoryFilter(dict):
     def __init__(__self__, *,
                  query: str):
-        """
-        :param str query: Filter criteria of the category.
-        """
         pulumi.set(__self__, "query", query)
 
     @property
     @pulumi.getter
     def query(self) -> str:
-        """
-        Filter criteria of the category.
-        """
         return pulumi.get(self, "query")
 
 
 @pulumi.output_type
 class LogsCustomPipelineProcessorDateRemapper(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -52720,25 +52161,19 @@
         return pulumi.get(self, "processors")
 
 
 @pulumi.output_type
 class LogsCustomPipelineProcessorPipelineFilter(dict):
     def __init__(__self__, *,
                  query: str):
-        """
-        :param str query: Filter criteria of the category.
-        """
         pulumi.set(__self__, "query", query)
 
     @property
     @pulumi.getter
     def query(self) -> str:
-        """
-        Filter criteria of the category.
-        """
         return pulumi.get(self, "query")
 
 
 @pulumi.output_type
 class LogsCustomPipelineProcessorPipelineProcessor(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -52794,30 +52229,14 @@
                  message_remapper: Optional['outputs.LogsCustomPipelineProcessorPipelineProcessorMessageRemapper'] = None,
                  service_remapper: Optional['outputs.LogsCustomPipelineProcessorPipelineProcessorServiceRemapper'] = None,
                  status_remapper: Optional['outputs.LogsCustomPipelineProcessorPipelineProcessorStatusRemapper'] = None,
                  string_builder_processor: Optional['outputs.LogsCustomPipelineProcessorPipelineProcessorStringBuilderProcessor'] = None,
                  trace_id_remapper: Optional['outputs.LogsCustomPipelineProcessorPipelineProcessorTraceIdRemapper'] = None,
                  url_parser: Optional['outputs.LogsCustomPipelineProcessorPipelineProcessorUrlParser'] = None,
                  user_agent_parser: Optional['outputs.LogsCustomPipelineProcessorPipelineProcessorUserAgentParser'] = None):
-        """
-        :param 'LogsCustomPipelineProcessorPipelineProcessorArithmeticProcessorArgs' arithmetic_processor: Arithmetic Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#arithmetic-processor)
-        :param 'LogsCustomPipelineProcessorPipelineProcessorAttributeRemapperArgs' attribute_remapper: Attribute Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#remapper)
-        :param 'LogsCustomPipelineProcessorPipelineProcessorCategoryProcessorArgs' category_processor: Category Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#category-processor)
-        :param 'LogsCustomPipelineProcessorPipelineProcessorDateRemapperArgs' date_remapper: Date Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#log-date-remapper)
-        :param 'LogsCustomPipelineProcessorPipelineProcessorGeoIpParserArgs' geo_ip_parser: Date GeoIP Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#geoip-parser)
-        :param 'LogsCustomPipelineProcessorPipelineProcessorGrokParserArgs' grok_parser: Grok Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#grok-parser)
-        :param 'LogsCustomPipelineProcessorPipelineProcessorLookupProcessorArgs' lookup_processor: Lookup Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#lookup-processor)
-        :param 'LogsCustomPipelineProcessorPipelineProcessorMessageRemapperArgs' message_remapper: Message Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#log-message-remapper)
-        :param 'LogsCustomPipelineProcessorPipelineProcessorServiceRemapperArgs' service_remapper: Service Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#service-remapper)
-        :param 'LogsCustomPipelineProcessorPipelineProcessorStatusRemapperArgs' status_remapper: Status Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#log-status-remapper)
-        :param 'LogsCustomPipelineProcessorPipelineProcessorStringBuilderProcessorArgs' string_builder_processor: String Builder Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#string-builder-processor)
-        :param 'LogsCustomPipelineProcessorPipelineProcessorTraceIdRemapperArgs' trace_id_remapper: Trace ID Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#trace-remapper)
-        :param 'LogsCustomPipelineProcessorPipelineProcessorUrlParserArgs' url_parser: URL Parser Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#url-parser)
-        :param 'LogsCustomPipelineProcessorPipelineProcessorUserAgentParserArgs' user_agent_parser: User-Agent Parser Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#user-agent-parser)
-        """
         if arithmetic_processor is not None:
             pulumi.set(__self__, "arithmetic_processor", arithmetic_processor)
         if attribute_remapper is not None:
             pulumi.set(__self__, "attribute_remapper", attribute_remapper)
         if category_processor is not None:
             pulumi.set(__self__, "category_processor", category_processor)
         if date_remapper is not None:
@@ -52842,121 +52261,79 @@
             pulumi.set(__self__, "url_parser", url_parser)
         if user_agent_parser is not None:
             pulumi.set(__self__, "user_agent_parser", user_agent_parser)
 
     @property
     @pulumi.getter(name="arithmeticProcessor")
     def arithmetic_processor(self) -> Optional['outputs.LogsCustomPipelineProcessorPipelineProcessorArithmeticProcessor']:
-        """
-        Arithmetic Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#arithmetic-processor)
-        """
         return pulumi.get(self, "arithmetic_processor")
 
     @property
     @pulumi.getter(name="attributeRemapper")
     def attribute_remapper(self) -> Optional['outputs.LogsCustomPipelineProcessorPipelineProcessorAttributeRemapper']:
-        """
-        Attribute Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#remapper)
-        """
         return pulumi.get(self, "attribute_remapper")
 
     @property
     @pulumi.getter(name="categoryProcessor")
     def category_processor(self) -> Optional['outputs.LogsCustomPipelineProcessorPipelineProcessorCategoryProcessor']:
-        """
-        Category Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#category-processor)
-        """
         return pulumi.get(self, "category_processor")
 
     @property
     @pulumi.getter(name="dateRemapper")
     def date_remapper(self) -> Optional['outputs.LogsCustomPipelineProcessorPipelineProcessorDateRemapper']:
-        """
-        Date Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#log-date-remapper)
-        """
         return pulumi.get(self, "date_remapper")
 
     @property
     @pulumi.getter(name="geoIpParser")
     def geo_ip_parser(self) -> Optional['outputs.LogsCustomPipelineProcessorPipelineProcessorGeoIpParser']:
-        """
-        Date GeoIP Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#geoip-parser)
-        """
         return pulumi.get(self, "geo_ip_parser")
 
     @property
     @pulumi.getter(name="grokParser")
     def grok_parser(self) -> Optional['outputs.LogsCustomPipelineProcessorPipelineProcessorGrokParser']:
-        """
-        Grok Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#grok-parser)
-        """
         return pulumi.get(self, "grok_parser")
 
     @property
     @pulumi.getter(name="lookupProcessor")
     def lookup_processor(self) -> Optional['outputs.LogsCustomPipelineProcessorPipelineProcessorLookupProcessor']:
-        """
-        Lookup Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#lookup-processor)
-        """
         return pulumi.get(self, "lookup_processor")
 
     @property
     @pulumi.getter(name="messageRemapper")
     def message_remapper(self) -> Optional['outputs.LogsCustomPipelineProcessorPipelineProcessorMessageRemapper']:
-        """
-        Message Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#log-message-remapper)
-        """
         return pulumi.get(self, "message_remapper")
 
     @property
     @pulumi.getter(name="serviceRemapper")
     def service_remapper(self) -> Optional['outputs.LogsCustomPipelineProcessorPipelineProcessorServiceRemapper']:
-        """
-        Service Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#service-remapper)
-        """
         return pulumi.get(self, "service_remapper")
 
     @property
     @pulumi.getter(name="statusRemapper")
     def status_remapper(self) -> Optional['outputs.LogsCustomPipelineProcessorPipelineProcessorStatusRemapper']:
-        """
-        Status Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#log-status-remapper)
-        """
         return pulumi.get(self, "status_remapper")
 
     @property
     @pulumi.getter(name="stringBuilderProcessor")
     def string_builder_processor(self) -> Optional['outputs.LogsCustomPipelineProcessorPipelineProcessorStringBuilderProcessor']:
-        """
-        String Builder Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#string-builder-processor)
-        """
         return pulumi.get(self, "string_builder_processor")
 
     @property
     @pulumi.getter(name="traceIdRemapper")
     def trace_id_remapper(self) -> Optional['outputs.LogsCustomPipelineProcessorPipelineProcessorTraceIdRemapper']:
-        """
-        Trace ID Remapper Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#trace-remapper)
-        """
         return pulumi.get(self, "trace_id_remapper")
 
     @property
     @pulumi.getter(name="urlParser")
     def url_parser(self) -> Optional['outputs.LogsCustomPipelineProcessorPipelineProcessorUrlParser']:
-        """
-        URL Parser Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#url-parser)
-        """
         return pulumi.get(self, "url_parser")
 
     @property
     @pulumi.getter(name="userAgentParser")
     def user_agent_parser(self) -> Optional['outputs.LogsCustomPipelineProcessorPipelineProcessorUserAgentParser']:
-        """
-        User-Agent Parser Processor. More information can be found in the [official docs](https://docs.datadoghq.com/logs/processing/processors/?tab=ui#user-agent-parser)
-        """
         return pulumi.get(self, "user_agent_parser")
 
 
 @pulumi.output_type
 class LogsCustomPipelineProcessorPipelineProcessorArithmeticProcessor(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -53189,25 +52566,19 @@
         return pulumi.get(self, "name")
 
 
 @pulumi.output_type
 class LogsCustomPipelineProcessorPipelineProcessorCategoryProcessorCategoryFilter(dict):
     def __init__(__self__, *,
                  query: str):
-        """
-        :param str query: Filter criteria of the category.
-        """
         pulumi.set(__self__, "query", query)
 
     @property
     @pulumi.getter
     def query(self) -> str:
-        """
-        Filter criteria of the category.
-        """
         return pulumi.get(self, "query")
 
 
 @pulumi.output_type
 class LogsCustomPipelineProcessorPipelineProcessorDateRemapper(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -54179,48 +53550,34 @@
         LogsIndexExclusionFilter.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  filters: Optional[Sequence['outputs.LogsIndexExclusionFilterFilter']] = None,
                  is_enabled: Optional[bool] = None,
                  name: Optional[str] = None):
-        """
-        :param Sequence['LogsIndexExclusionFilterFilterArgs'] filters: Logs filter
-        :param bool is_enabled: A boolean stating if the exclusion is active or not.
-        :param str name: The name of the exclusion filter.
-        """
         if filters is not None:
             pulumi.set(__self__, "filters", filters)
         if is_enabled is not None:
             pulumi.set(__self__, "is_enabled", is_enabled)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def filters(self) -> Optional[Sequence['outputs.LogsIndexExclusionFilterFilter']]:
-        """
-        Logs filter
-        """
         return pulumi.get(self, "filters")
 
     @property
     @pulumi.getter(name="isEnabled")
     def is_enabled(self) -> Optional[bool]:
-        """
-        A boolean stating if the exclusion is active or not.
-        """
         return pulumi.get(self, "is_enabled")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
-        """
-        The name of the exclusion filter.
-        """
         return pulumi.get(self, "name")
 
 
 @pulumi.output_type
 class LogsIndexExclusionFilterFilter(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -54238,51 +53595,39 @@
     def get(self, key: str, default = None) -> Any:
         LogsIndexExclusionFilterFilter.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  query: Optional[str] = None,
                  sample_rate: Optional[float] = None):
-        """
-        :param str query: Logs filter criteria. Only logs matching this filter criteria are considered for this index.
-        """
         if query is not None:
             pulumi.set(__self__, "query", query)
         if sample_rate is not None:
             pulumi.set(__self__, "sample_rate", sample_rate)
 
     @property
     @pulumi.getter
     def query(self) -> Optional[str]:
-        """
-        Logs filter criteria. Only logs matching this filter criteria are considered for this index.
-        """
         return pulumi.get(self, "query")
 
     @property
     @pulumi.getter(name="sampleRate")
     def sample_rate(self) -> Optional[float]:
         return pulumi.get(self, "sample_rate")
 
 
 @pulumi.output_type
 class LogsIndexFilter(dict):
     def __init__(__self__, *,
                  query: str):
-        """
-        :param str query: Logs filter criteria. Only logs matching this filter criteria are considered for this index.
-        """
         pulumi.set(__self__, "query", query)
 
     @property
     @pulumi.getter
     def query(self) -> str:
-        """
-        Logs filter criteria. Only logs matching this filter criteria are considered for this index.
-        """
         return pulumi.get(self, "query")
 
 
 @pulumi.output_type
 class LogsMetricCompute(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -54300,54 +53645,38 @@
     def get(self, key: str, default = None) -> Any:
         LogsMetricCompute.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  aggregation_type: str,
                  path: Optional[str] = None):
-        """
-        :param str aggregation_type: The type of aggregation to use. This field can't be updated after creation. Valid values are `count`, `distribution`.
-        :param str path: The path to the value the log-based metric will aggregate on (only used if the aggregation type is a "distribution"). This field can't be updated after creation.
-        """
         pulumi.set(__self__, "aggregation_type", aggregation_type)
         if path is not None:
             pulumi.set(__self__, "path", path)
 
     @property
     @pulumi.getter(name="aggregationType")
     def aggregation_type(self) -> str:
-        """
-        The type of aggregation to use. This field can't be updated after creation. Valid values are `count`, `distribution`.
-        """
         return pulumi.get(self, "aggregation_type")
 
     @property
     @pulumi.getter
     def path(self) -> Optional[str]:
-        """
-        The path to the value the log-based metric will aggregate on (only used if the aggregation type is a "distribution"). This field can't be updated after creation.
-        """
         return pulumi.get(self, "path")
 
 
 @pulumi.output_type
 class LogsMetricFilter(dict):
     def __init__(__self__, *,
                  query: str):
-        """
-        :param str query: The search query - following the log search syntax.
-        """
         pulumi.set(__self__, "query", query)
 
     @property
     @pulumi.getter
     def query(self) -> str:
-        """
-        The search query - following the log search syntax.
-        """
         return pulumi.get(self, "query")
 
 
 @pulumi.output_type
 class LogsMetricGroupBy(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -54365,64 +53694,44 @@
     def get(self, key: str, default = None) -> Any:
         LogsMetricGroupBy.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  path: str,
                  tag_name: str):
-        """
-        :param str path: The path to the value the log-based metric will be aggregated over.
-        :param str tag_name: Name of the tag that gets created.
-        """
         pulumi.set(__self__, "path", path)
         pulumi.set(__self__, "tag_name", tag_name)
 
     @property
     @pulumi.getter
     def path(self) -> str:
-        """
-        The path to the value the log-based metric will be aggregated over.
-        """
         return pulumi.get(self, "path")
 
     @property
     @pulumi.getter(name="tagName")
     def tag_name(self) -> str:
-        """
-        Name of the tag that gets created.
-        """
         return pulumi.get(self, "tag_name")
 
 
 @pulumi.output_type
 class MetricTagConfigurationAggregation(dict):
     def __init__(__self__, *,
                  space: str,
                  time: str):
-        """
-        :param str space: A space aggregation for use in query. Valid values are `avg`, `max`, `min`, `sum`.
-        :param str time: A time aggregation for use in query. Valid values are `avg`, `count`, `max`, `min`, `sum`.
-        """
         pulumi.set(__self__, "space", space)
         pulumi.set(__self__, "time", time)
 
     @property
     @pulumi.getter
     def space(self) -> str:
-        """
-        A space aggregation for use in query. Valid values are `avg`, `max`, `min`, `sum`.
-        """
         return pulumi.get(self, "space")
 
     @property
     @pulumi.getter
     def time(self) -> str:
-        """
-        A time aggregation for use in query. Valid values are `avg`, `count`, `max`, `min`, `sum`.
-        """
         return pulumi.get(self, "time")
 
 
 @pulumi.output_type
 class MonitorMonitorThresholdWindows(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -54442,37 +53751,27 @@
     def get(self, key: str, default = None) -> Any:
         MonitorMonitorThresholdWindows.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  recovery_window: Optional[str] = None,
                  trigger_window: Optional[str] = None):
-        """
-        :param str recovery_window: Describes how long an anomalous metric must be normal before the alert recovers.
-        :param str trigger_window: Describes how long a metric must be anomalous before an alert triggers.
-        """
         if recovery_window is not None:
             pulumi.set(__self__, "recovery_window", recovery_window)
         if trigger_window is not None:
             pulumi.set(__self__, "trigger_window", trigger_window)
 
     @property
     @pulumi.getter(name="recoveryWindow")
     def recovery_window(self) -> Optional[str]:
-        """
-        Describes how long an anomalous metric must be normal before the alert recovers.
-        """
         return pulumi.get(self, "recovery_window")
 
     @property
     @pulumi.getter(name="triggerWindow")
     def trigger_window(self) -> Optional[str]:
-        """
-        Describes how long a metric must be anomalous before an alert triggers.
-        """
         return pulumi.get(self, "trigger_window")
 
 
 @pulumi.output_type
 class MonitorMonitorThresholds(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -54496,22 +53795,14 @@
     def __init__(__self__, *,
                  critical: Optional[str] = None,
                  critical_recovery: Optional[str] = None,
                  ok: Optional[str] = None,
                  unknown: Optional[str] = None,
                  warning: Optional[str] = None,
                  warning_recovery: Optional[str] = None):
-        """
-        :param str critical: The monitor `CRITICAL` threshold. Must be a number.
-        :param str critical_recovery: The monitor `CRITICAL` recovery threshold. Must be a number.
-        :param str ok: The monitor `OK` threshold. Must be a number.
-        :param str unknown: The monitor `UNKNOWN` threshold. Must be a number.
-        :param str warning: The monitor `WARNING` threshold. Must be a number.
-        :param str warning_recovery: The monitor `WARNING` recovery threshold. Must be a number.
-        """
         if critical is not None:
             pulumi.set(__self__, "critical", critical)
         if critical_recovery is not None:
             pulumi.set(__self__, "critical_recovery", critical_recovery)
         if ok is not None:
             pulumi.set(__self__, "ok", ok)
         if unknown is not None:
@@ -54520,57 +53811,39 @@
             pulumi.set(__self__, "warning", warning)
         if warning_recovery is not None:
             pulumi.set(__self__, "warning_recovery", warning_recovery)
 
     @property
     @pulumi.getter
     def critical(self) -> Optional[str]:
-        """
-        The monitor `CRITICAL` threshold. Must be a number.
-        """
         return pulumi.get(self, "critical")
 
     @property
     @pulumi.getter(name="criticalRecovery")
     def critical_recovery(self) -> Optional[str]:
-        """
-        The monitor `CRITICAL` recovery threshold. Must be a number.
-        """
         return pulumi.get(self, "critical_recovery")
 
     @property
     @pulumi.getter
     def ok(self) -> Optional[str]:
-        """
-        The monitor `OK` threshold. Must be a number.
-        """
         return pulumi.get(self, "ok")
 
     @property
     @pulumi.getter
     def unknown(self) -> Optional[str]:
-        """
-        The monitor `UNKNOWN` threshold. Must be a number.
-        """
         return pulumi.get(self, "unknown")
 
     @property
     @pulumi.getter
     def warning(self) -> Optional[str]:
-        """
-        The monitor `WARNING` threshold. Must be a number.
-        """
         return pulumi.get(self, "warning")
 
     @property
     @pulumi.getter(name="warningRecovery")
     def warning_recovery(self) -> Optional[str]:
-        """
-        The monitor `WARNING` recovery threshold. Must be a number.
-        """
         return pulumi.get(self, "warning_recovery")
 
 
 @pulumi.output_type
 class OrganizationSettingsSettings(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -54612,26 +53885,14 @@
                  saml_strict_mode: 'outputs.OrganizationSettingsSettingsSamlStrictMode',
                  private_widget_share: Optional[bool] = None,
                  saml_autocreate_access_role: Optional[str] = None,
                  saml_can_be_enabled: Optional[bool] = None,
                  saml_idp_endpoint: Optional[str] = None,
                  saml_idp_metadata_uploaded: Optional[bool] = None,
                  saml_login_url: Optional[str] = None):
-        """
-        :param 'OrganizationSettingsSettingsSamlArgs' saml: SAML properties
-        :param 'OrganizationSettingsSettingsSamlAutocreateUsersDomainsArgs' saml_autocreate_users_domains: List of domains where the SAML automated user creation is enabled.
-        :param 'OrganizationSettingsSettingsSamlIdpInitiatedLoginArgs' saml_idp_initiated_login: Whether or not a SAML identity provider metadata file was provided to the Datadog organization.
-        :param 'OrganizationSettingsSettingsSamlStrictModeArgs' saml_strict_mode: Whether or not the SAML strict mode is enabled. If true, all users must log in with SAML.
-        :param bool private_widget_share: Whether or not the organization users can share widgets outside of Datadog.
-        :param str saml_autocreate_access_role: The access role of the user. Options are `st` (standard user), `adm` (admin user), or `ro` (read-only user). Allowed enum values: `st`, `adm` , `ro`, `ERROR`
-        :param bool saml_can_be_enabled: Whether or not SAML can be enabled for this organization.
-        :param str saml_idp_endpoint: Identity provider endpoint for SAML authentication.
-        :param bool saml_idp_metadata_uploaded: Whether or not a SAML identity provider metadata file was provided to the Datadog organization.
-        :param str saml_login_url: URL for SAML logging.
-        """
         pulumi.set(__self__, "saml", saml)
         pulumi.set(__self__, "saml_autocreate_users_domains", saml_autocreate_users_domains)
         pulumi.set(__self__, "saml_idp_initiated_login", saml_idp_initiated_login)
         pulumi.set(__self__, "saml_strict_mode", saml_strict_mode)
         if private_widget_share is not None:
             pulumi.set(__self__, "private_widget_share", private_widget_share)
         if saml_autocreate_access_role is not None:
@@ -54644,89 +53905,59 @@
             pulumi.set(__self__, "saml_idp_metadata_uploaded", saml_idp_metadata_uploaded)
         if saml_login_url is not None:
             pulumi.set(__self__, "saml_login_url", saml_login_url)
 
     @property
     @pulumi.getter
     def saml(self) -> 'outputs.OrganizationSettingsSettingsSaml':
-        """
-        SAML properties
-        """
         return pulumi.get(self, "saml")
 
     @property
     @pulumi.getter(name="samlAutocreateUsersDomains")
     def saml_autocreate_users_domains(self) -> 'outputs.OrganizationSettingsSettingsSamlAutocreateUsersDomains':
-        """
-        List of domains where the SAML automated user creation is enabled.
-        """
         return pulumi.get(self, "saml_autocreate_users_domains")
 
     @property
     @pulumi.getter(name="samlIdpInitiatedLogin")
     def saml_idp_initiated_login(self) -> 'outputs.OrganizationSettingsSettingsSamlIdpInitiatedLogin':
-        """
-        Whether or not a SAML identity provider metadata file was provided to the Datadog organization.
-        """
         return pulumi.get(self, "saml_idp_initiated_login")
 
     @property
     @pulumi.getter(name="samlStrictMode")
     def saml_strict_mode(self) -> 'outputs.OrganizationSettingsSettingsSamlStrictMode':
-        """
-        Whether or not the SAML strict mode is enabled. If true, all users must log in with SAML.
-        """
         return pulumi.get(self, "saml_strict_mode")
 
     @property
     @pulumi.getter(name="privateWidgetShare")
     def private_widget_share(self) -> Optional[bool]:
-        """
-        Whether or not the organization users can share widgets outside of Datadog.
-        """
         return pulumi.get(self, "private_widget_share")
 
     @property
     @pulumi.getter(name="samlAutocreateAccessRole")
     def saml_autocreate_access_role(self) -> Optional[str]:
-        """
-        The access role of the user. Options are `st` (standard user), `adm` (admin user), or `ro` (read-only user). Allowed enum values: `st`, `adm` , `ro`, `ERROR`
-        """
         return pulumi.get(self, "saml_autocreate_access_role")
 
     @property
     @pulumi.getter(name="samlCanBeEnabled")
     def saml_can_be_enabled(self) -> Optional[bool]:
-        """
-        Whether or not SAML can be enabled for this organization.
-        """
         return pulumi.get(self, "saml_can_be_enabled")
 
     @property
     @pulumi.getter(name="samlIdpEndpoint")
     def saml_idp_endpoint(self) -> Optional[str]:
-        """
-        Identity provider endpoint for SAML authentication.
-        """
         return pulumi.get(self, "saml_idp_endpoint")
 
     @property
     @pulumi.getter(name="samlIdpMetadataUploaded")
     def saml_idp_metadata_uploaded(self) -> Optional[bool]:
-        """
-        Whether or not a SAML identity provider metadata file was provided to the Datadog organization.
-        """
         return pulumi.get(self, "saml_idp_metadata_uploaded")
 
     @property
     @pulumi.getter(name="samlLoginUrl")
     def saml_login_url(self) -> Optional[str]:
-        """
-        URL for SAML logging.
-        """
         return pulumi.get(self, "saml_login_url")
 
 
 @pulumi.output_type
 class OrganizationSettingsSettingsSaml(dict):
     def __init__(__self__, *,
                  enabled: Optional[bool] = None):
@@ -54787,36 +54018,26 @@
 
 
 @pulumi.output_type
 class RolePermission(dict):
     def __init__(__self__, *,
                  id: str,
                  name: Optional[str] = None):
-        """
-        :param str id: ID of the permission to assign.
-        :param str name: Name of the permission.
-        """
         pulumi.set(__self__, "id", id)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def id(self) -> str:
-        """
-        ID of the permission to assign.
-        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
-        """
-        Name of the permission.
-        """
         return pulumi.get(self, "name")
 
 
 @pulumi.output_type
 class SecurityMonitoringDefaultRuleCase(dict):
     def __init__(__self__, *,
                  notifications: Sequence[str],
@@ -54855,35 +54076,25 @@
 
 
 @pulumi.output_type
 class SecurityMonitoringFilterExclusionFilter(dict):
     def __init__(__self__, *,
                  name: str,
                  query: str):
-        """
-        :param str name: Exclusion filter name.
-        :param str query: Exclusion filter query. Logs that match this query are excluded from the security filter.
-        """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "query", query)
 
     @property
     @pulumi.getter
     def name(self) -> str:
-        """
-        Exclusion filter name.
-        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def query(self) -> str:
-        """
-        Exclusion filter query. Logs that match this query are excluded from the security filter.
-        """
         return pulumi.get(self, "query")
 
 
 @pulumi.output_type
 class SecurityMonitoringRuleCase(dict):
     def __init__(__self__, *,
                  status: str,
@@ -54959,14 +54170,16 @@
             suggest = "keep_alive"
         elif key == "maxSignalDuration":
             suggest = "max_signal_duration"
         elif key == "detectionMethod":
             suggest = "detection_method"
         elif key == "evaluationWindow":
             suggest = "evaluation_window"
+        elif key == "impossibleTravelOptions":
+            suggest = "impossible_travel_options"
         elif key == "newValueOptions":
             suggest = "new_value_options"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in SecurityMonitoringRuleOptions. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
@@ -54978,21 +54191,24 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  keep_alive: int,
                  max_signal_duration: int,
                  detection_method: Optional[str] = None,
                  evaluation_window: Optional[int] = None,
+                 impossible_travel_options: Optional['outputs.SecurityMonitoringRuleOptionsImpossibleTravelOptions'] = None,
                  new_value_options: Optional['outputs.SecurityMonitoringRuleOptionsNewValueOptions'] = None):
         pulumi.set(__self__, "keep_alive", keep_alive)
         pulumi.set(__self__, "max_signal_duration", max_signal_duration)
         if detection_method is not None:
             pulumi.set(__self__, "detection_method", detection_method)
         if evaluation_window is not None:
             pulumi.set(__self__, "evaluation_window", evaluation_window)
+        if impossible_travel_options is not None:
+            pulumi.set(__self__, "impossible_travel_options", impossible_travel_options)
         if new_value_options is not None:
             pulumi.set(__self__, "new_value_options", new_value_options)
 
     @property
     @pulumi.getter(name="keepAlive")
     def keep_alive(self) -> int:
         return pulumi.get(self, "keep_alive")
@@ -55009,20 +54225,55 @@
 
     @property
     @pulumi.getter(name="evaluationWindow")
     def evaluation_window(self) -> Optional[int]:
         return pulumi.get(self, "evaluation_window")
 
     @property
+    @pulumi.getter(name="impossibleTravelOptions")
+    def impossible_travel_options(self) -> Optional['outputs.SecurityMonitoringRuleOptionsImpossibleTravelOptions']:
+        return pulumi.get(self, "impossible_travel_options")
+
+    @property
     @pulumi.getter(name="newValueOptions")
     def new_value_options(self) -> Optional['outputs.SecurityMonitoringRuleOptionsNewValueOptions']:
         return pulumi.get(self, "new_value_options")
 
 
 @pulumi.output_type
+class SecurityMonitoringRuleOptionsImpossibleTravelOptions(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "baselineUserLocations":
+            suggest = "baseline_user_locations"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in SecurityMonitoringRuleOptionsImpossibleTravelOptions. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        SecurityMonitoringRuleOptionsImpossibleTravelOptions.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        SecurityMonitoringRuleOptionsImpossibleTravelOptions.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 baseline_user_locations: Optional[bool] = None):
+        if baseline_user_locations is not None:
+            pulumi.set(__self__, "baseline_user_locations", baseline_user_locations)
+
+    @property
+    @pulumi.getter(name="baselineUserLocations")
+    def baseline_user_locations(self) -> Optional[bool]:
+        return pulumi.get(self, "baseline_user_locations")
+
+
+@pulumi.output_type
 class SecurityMonitoringRuleOptionsNewValueOptions(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "forgetAfter":
             suggest = "forget_after"
         elif key == "learningDuration":
@@ -55184,35 +54435,25 @@
 
 
 @pulumi.output_type
 class ServiceLevelObjectiveQuery(dict):
     def __init__(__self__, *,
                  denominator: str,
                  numerator: str):
-        """
-        :param str denominator: The sum of the `total` events.
-        :param str numerator: The sum of all the `good` events.
-        """
         pulumi.set(__self__, "denominator", denominator)
         pulumi.set(__self__, "numerator", numerator)
 
     @property
     @pulumi.getter
     def denominator(self) -> str:
-        """
-        The sum of the `total` events.
-        """
         return pulumi.get(self, "denominator")
 
     @property
     @pulumi.getter
     def numerator(self) -> str:
-        """
-        The sum of all the `good` events.
-        """
         return pulumi.get(self, "numerator")
 
 
 @pulumi.output_type
 class ServiceLevelObjectiveThreshold(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -55235,135 +54476,127 @@
 
     def __init__(__self__, *,
                  target: float,
                  timeframe: str,
                  target_display: Optional[str] = None,
                  warning: Optional[float] = None,
                  warning_display: Optional[str] = None):
-        """
-        :param float target: The objective's target in`[0,100]`.
-        :param str timeframe: The time frame for the objective. The mapping from these types to the types found in the Datadog Web UI can be found in the Datadog API documentation page. Valid values are `7d`, `30d`, `90d`, `custom`.
-        :param str target_display: A string representation of the target that indicates its precision. It uses trailing zeros to show significant decimal places (e.g. `98.00`).
-        :param float warning: The objective's warning value in `[0,100]`. This must be greater than the target value.
-        :param str warning_display: A string representation of the warning target (see the description of the target_display field for details).
-        """
         pulumi.set(__self__, "target", target)
         pulumi.set(__self__, "timeframe", timeframe)
         if target_display is not None:
             pulumi.set(__self__, "target_display", target_display)
         if warning is not None:
             pulumi.set(__self__, "warning", warning)
         if warning_display is not None:
             pulumi.set(__self__, "warning_display", warning_display)
 
     @property
     @pulumi.getter
     def target(self) -> float:
-        """
-        The objective's target in`[0,100]`.
-        """
         return pulumi.get(self, "target")
 
     @property
     @pulumi.getter
     def timeframe(self) -> str:
-        """
-        The time frame for the objective. The mapping from these types to the types found in the Datadog Web UI can be found in the Datadog API documentation page. Valid values are `7d`, `30d`, `90d`, `custom`.
-        """
         return pulumi.get(self, "timeframe")
 
     @property
     @pulumi.getter(name="targetDisplay")
     def target_display(self) -> Optional[str]:
-        """
-        A string representation of the target that indicates its precision. It uses trailing zeros to show significant decimal places (e.g. `98.00`).
-        """
         return pulumi.get(self, "target_display")
 
     @property
     @pulumi.getter
     def warning(self) -> Optional[float]:
-        """
-        The objective's warning value in `[0,100]`. This must be greater than the target value.
-        """
         return pulumi.get(self, "warning")
 
     @property
     @pulumi.getter(name="warningDisplay")
     def warning_display(self) -> Optional[str]:
-        """
-        A string representation of the warning target (see the description of the target_display field for details).
-        """
         return pulumi.get(self, "warning_display")
 
 
 @pulumi.output_type
 class SyntheticsGlobalVariableParseTestOptions(dict):
     def __init__(__self__, *,
                  parser: 'outputs.SyntheticsGlobalVariableParseTestOptionsParser',
                  type: str,
                  field: Optional[str] = None):
-        """
-        :param str type: Defines the source to use to extract the value. Valid values are `http_body`, `http_header`.
-        :param str field: Required when type = `http_header`. Defines the header to use to extract the value
-        """
         pulumi.set(__self__, "parser", parser)
         pulumi.set(__self__, "type", type)
         if field is not None:
             pulumi.set(__self__, "field", field)
 
     @property
     @pulumi.getter
     def parser(self) -> 'outputs.SyntheticsGlobalVariableParseTestOptionsParser':
         return pulumi.get(self, "parser")
 
     @property
     @pulumi.getter
     def type(self) -> str:
-        """
-        Defines the source to use to extract the value. Valid values are `http_body`, `http_header`.
-        """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def field(self) -> Optional[str]:
-        """
-        Required when type = `http_header`. Defines the header to use to extract the value
-        """
         return pulumi.get(self, "field")
 
 
 @pulumi.output_type
 class SyntheticsGlobalVariableParseTestOptionsParser(dict):
     def __init__(__self__, *,
                  type: str,
                  value: Optional[str] = None):
-        """
-        :param str value: The value of the global variable.
-        """
         pulumi.set(__self__, "type", type)
         if value is not None:
             pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def type(self) -> str:
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def value(self) -> Optional[str]:
-        """
-        The value of the global variable.
-        """
         return pulumi.get(self, "value")
 
 
 @pulumi.output_type
+class SyntheticsPrivateLocationMetadata(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "restrictedRoles":
+            suggest = "restricted_roles"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in SyntheticsPrivateLocationMetadata. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        SyntheticsPrivateLocationMetadata.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        SyntheticsPrivateLocationMetadata.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 restricted_roles: Optional[Sequence[str]] = None):
+        if restricted_roles is not None:
+            pulumi.set(__self__, "restricted_roles", restricted_roles)
+
+    @property
+    @pulumi.getter(name="restrictedRoles")
+    def restricted_roles(self) -> Optional[Sequence[str]]:
+        return pulumi.get(self, "restricted_roles")
+
+
+@pulumi.output_type
 class SyntheticsTestApiStep(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "allowFailure":
             suggest = "allow_failure"
         elif key == "extractedValues":
@@ -55404,28 +54637,14 @@
                  request_client_certificate: Optional['outputs.SyntheticsTestApiStepRequestClientCertificate'] = None,
                  request_definition: Optional['outputs.SyntheticsTestApiStepRequestDefinition'] = None,
                  request_headers: Optional[Mapping[str, Any]] = None,
                  request_proxy: Optional['outputs.SyntheticsTestApiStepRequestProxy'] = None,
                  request_query: Optional[Mapping[str, Any]] = None,
                  retry: Optional['outputs.SyntheticsTestApiStepRetry'] = None,
                  subtype: Optional[str] = None):
-        """
-        :param str name: The name of the step.
-        :param bool allow_failure: Determines whether or not to continue with test if this step fails.
-        :param Sequence['SyntheticsTestApiStepAssertionArgs'] assertions: Assertions used for the test. Multiple `assertion` blocks are allowed with the structure below.
-        :param Sequence['SyntheticsTestApiStepExtractedValueArgs'] extracted_values: Values to parse and save as variables from the response.
-        :param bool is_critical: Determines whether or not to consider the entire test as failed if this step fails. Can be used only if `allow_failure` is `true`.
-        :param 'SyntheticsTestApiStepRequestBasicauthArgs' request_basicauth: The HTTP basic authentication credentials. Exactly one nested block is allowed with the structure below.
-        :param 'SyntheticsTestApiStepRequestClientCertificateArgs' request_client_certificate: Client certificate to use when performing the test request. Exactly one nested block is allowed with the structure below.
-        :param 'SyntheticsTestApiStepRequestDefinitionArgs' request_definition: The request for the api step.
-        :param Mapping[str, Any] request_headers: Header name and value map.
-        :param 'SyntheticsTestApiStepRequestProxyArgs' request_proxy: The proxy to perform the test.
-        :param Mapping[str, Any] request_query: Query arguments name and value map.
-        :param str subtype: The subtype of the Synthetic multistep API test step. Valid values are `http`.
-        """
         pulumi.set(__self__, "name", name)
         if allow_failure is not None:
             pulumi.set(__self__, "allow_failure", allow_failure)
         if assertions is not None:
             pulumi.set(__self__, "assertions", assertions)
         if extracted_values is not None:
             pulumi.set(__self__, "extracted_values", extracted_values)
@@ -55447,175 +54666,117 @@
             pulumi.set(__self__, "retry", retry)
         if subtype is not None:
             pulumi.set(__self__, "subtype", subtype)
 
     @property
     @pulumi.getter
     def name(self) -> str:
-        """
-        The name of the step.
-        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="allowFailure")
     def allow_failure(self) -> Optional[bool]:
-        """
-        Determines whether or not to continue with test if this step fails.
-        """
         return pulumi.get(self, "allow_failure")
 
     @property
     @pulumi.getter
     def assertions(self) -> Optional[Sequence['outputs.SyntheticsTestApiStepAssertion']]:
-        """
-        Assertions used for the test. Multiple `assertion` blocks are allowed with the structure below.
-        """
         return pulumi.get(self, "assertions")
 
     @property
     @pulumi.getter(name="extractedValues")
     def extracted_values(self) -> Optional[Sequence['outputs.SyntheticsTestApiStepExtractedValue']]:
-        """
-        Values to parse and save as variables from the response.
-        """
         return pulumi.get(self, "extracted_values")
 
     @property
     @pulumi.getter(name="isCritical")
     def is_critical(self) -> Optional[bool]:
-        """
-        Determines whether or not to consider the entire test as failed if this step fails. Can be used only if `allow_failure` is `true`.
-        """
         return pulumi.get(self, "is_critical")
 
     @property
     @pulumi.getter(name="requestBasicauth")
     def request_basicauth(self) -> Optional['outputs.SyntheticsTestApiStepRequestBasicauth']:
-        """
-        The HTTP basic authentication credentials. Exactly one nested block is allowed with the structure below.
-        """
         return pulumi.get(self, "request_basicauth")
 
     @property
     @pulumi.getter(name="requestClientCertificate")
     def request_client_certificate(self) -> Optional['outputs.SyntheticsTestApiStepRequestClientCertificate']:
-        """
-        Client certificate to use when performing the test request. Exactly one nested block is allowed with the structure below.
-        """
         return pulumi.get(self, "request_client_certificate")
 
     @property
     @pulumi.getter(name="requestDefinition")
     def request_definition(self) -> Optional['outputs.SyntheticsTestApiStepRequestDefinition']:
-        """
-        The request for the api step.
-        """
         return pulumi.get(self, "request_definition")
 
     @property
     @pulumi.getter(name="requestHeaders")
     def request_headers(self) -> Optional[Mapping[str, Any]]:
-        """
-        Header name and value map.
-        """
         return pulumi.get(self, "request_headers")
 
     @property
     @pulumi.getter(name="requestProxy")
     def request_proxy(self) -> Optional['outputs.SyntheticsTestApiStepRequestProxy']:
-        """
-        The proxy to perform the test.
-        """
         return pulumi.get(self, "request_proxy")
 
     @property
     @pulumi.getter(name="requestQuery")
     def request_query(self) -> Optional[Mapping[str, Any]]:
-        """
-        Query arguments name and value map.
-        """
         return pulumi.get(self, "request_query")
 
     @property
     @pulumi.getter
     def retry(self) -> Optional['outputs.SyntheticsTestApiStepRetry']:
         return pulumi.get(self, "retry")
 
     @property
     @pulumi.getter
     def subtype(self) -> Optional[str]:
-        """
-        The subtype of the Synthetic multistep API test step. Valid values are `http`.
-        """
         return pulumi.get(self, "subtype")
 
 
 @pulumi.output_type
 class SyntheticsTestApiStepAssertion(dict):
     def __init__(__self__, *,
                  operator: str,
                  type: str,
                  property: Optional[str] = None,
                  target: Optional[str] = None,
                  targetjsonpath: Optional['outputs.SyntheticsTestApiStepAssertionTargetjsonpath'] = None):
-        """
-        :param str operator: Assertion operator. **Note** Only some combinations of `type` and `operator` are valid (please refer to [Datadog documentation](https://docs.datadoghq.com/api/latest/synthetics/#create-a-test)).
-        :param str type: Type of assertion. **Note** Only some combinations of `type` and `operator` are valid (please refer to [Datadog documentation](https://docs.datadoghq.com/api/latest/synthetics/#create-a-test)). Valid values are `body`, `header`, `statusCode`, `certificate`, `responseTime`, `property`, `recordEvery`, `recordSome`, `tlsVersion`, `minTlsVersion`, `latency`, `packetLossPercentage`, `packetsReceived`, `networkHop`, `receivedMessage`.
-        :param str property: If assertion type is `header`, this is the header name.
-        :param str target: Expected value. Depends on the assertion type, refer to [Datadog documentation](https://docs.datadoghq.com/api/latest/synthetics/#create-a-test) for details.
-        :param 'SyntheticsTestApiStepAssertionTargetjsonpathArgs' targetjsonpath: Expected structure if `operator` is `validatesJSONPath`. Exactly one nested block is allowed with the structure below.
-        """
         pulumi.set(__self__, "operator", operator)
         pulumi.set(__self__, "type", type)
         if property is not None:
             pulumi.set(__self__, "property", property)
         if target is not None:
             pulumi.set(__self__, "target", target)
         if targetjsonpath is not None:
             pulumi.set(__self__, "targetjsonpath", targetjsonpath)
 
     @property
     @pulumi.getter
     def operator(self) -> str:
-        """
-        Assertion operator. **Note** Only some combinations of `type` and `operator` are valid (please refer to [Datadog documentation](https://docs.datadoghq.com/api/latest/synthetics/#create-a-test)).
-        """
         return pulumi.get(self, "operator")
 
     @property
     @pulumi.getter
     def type(self) -> str:
-        """
-        Type of assertion. **Note** Only some combinations of `type` and `operator` are valid (please refer to [Datadog documentation](https://docs.datadoghq.com/api/latest/synthetics/#create-a-test)). Valid values are `body`, `header`, `statusCode`, `certificate`, `responseTime`, `property`, `recordEvery`, `recordSome`, `tlsVersion`, `minTlsVersion`, `latency`, `packetLossPercentage`, `packetsReceived`, `networkHop`, `receivedMessage`.
-        """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def target(self) -> Optional[str]:
-        """
-        Expected value. Depends on the assertion type, refer to [Datadog documentation](https://docs.datadoghq.com/api/latest/synthetics/#create-a-test) for details.
-        """
         return pulumi.get(self, "target")
 
     @property
     @pulumi.getter
     def targetjsonpath(self) -> Optional['outputs.SyntheticsTestApiStepAssertionTargetjsonpath']:
-        """
-        Expected structure if `operator` is `validatesJSONPath`. Exactly one nested block is allowed with the structure below.
-        """
         return pulumi.get(self, "targetjsonpath")
 
     @property
     @pulumi.getter
     def property(self) -> Optional[str]:
-        """
-        If assertion type is `header`, this is the header name.
-        """
         return pulumi.get(self, "property")
 
 
 @pulumi.output_type
 class SyntheticsTestApiStepAssertionTargetjsonpath(dict):
     def __init__(__self__, *,
                  jsonpath: str,
@@ -55644,69 +54805,53 @@
 @pulumi.output_type
 class SyntheticsTestApiStepExtractedValue(dict):
     def __init__(__self__, *,
                  name: str,
                  parser: 'outputs.SyntheticsTestApiStepExtractedValueParser',
                  type: str,
                  field: Optional[str] = None):
-        """
-        :param str name: Name of Datadog synthetics test.
-        :param str type: Synthetics test type. Valid values are `api`, `browser`.
-        """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "parser", parser)
         pulumi.set(__self__, "type", type)
         if field is not None:
             pulumi.set(__self__, "field", field)
 
     @property
     @pulumi.getter
     def name(self) -> str:
-        """
-        Name of Datadog synthetics test.
-        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def parser(self) -> 'outputs.SyntheticsTestApiStepExtractedValueParser':
         return pulumi.get(self, "parser")
 
     @property
     @pulumi.getter
     def type(self) -> str:
-        """
-        Synthetics test type. Valid values are `api`, `browser`.
-        """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def field(self) -> Optional[str]:
         return pulumi.get(self, "field")
 
 
 @pulumi.output_type
 class SyntheticsTestApiStepExtractedValueParser(dict):
     def __init__(__self__, *,
                  type: str,
                  value: Optional[str] = None):
-        """
-        :param str type: Synthetics test type. Valid values are `api`, `browser`.
-        """
         pulumi.set(__self__, "type", type)
         if value is not None:
             pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def type(self) -> str:
-        """
-        Synthetics test type. Valid values are `api`, `browser`.
-        """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def value(self) -> Optional[str]:
         return pulumi.get(self, "value")
 
@@ -55743,26 +54888,14 @@
                  region: Optional[str] = None,
                  secret_key: Optional[str] = None,
                  service_name: Optional[str] = None,
                  session_token: Optional[str] = None,
                  type: Optional[str] = None,
                  username: Optional[str] = None,
                  workstation: Optional[str] = None):
-        """
-        :param str access_key: Access key for `SIGV4` authentication.
-        :param str domain: Domain for `ntlm` authentication.
-        :param str password: Password for authentication.
-        :param str region: Region for `SIGV4` authentication.
-        :param str secret_key: Secret key for `SIGV4` authentication.
-        :param str service_name: Service name for `SIGV4` authentication.
-        :param str session_token: Session token for `SIGV4` authentication.
-        :param str type: Type of basic authentication to use when performing the test.
-        :param str username: Username for authentication.
-        :param str workstation: Workstation for `ntlm` authentication.
-        """
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if domain is not None:
             pulumi.set(__self__, "domain", domain)
         if password is not None:
             pulumi.set(__self__, "password", password)
         if region is not None:
@@ -55779,89 +54912,59 @@
             pulumi.set(__self__, "username", username)
         if workstation is not None:
             pulumi.set(__self__, "workstation", workstation)
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
-        """
-        Access key for `SIGV4` authentication.
-        """
         return pulumi.get(self, "access_key")
 
     @property
     @pulumi.getter
     def domain(self) -> Optional[str]:
-        """
-        Domain for `ntlm` authentication.
-        """
         return pulumi.get(self, "domain")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
-        """
-        Password for authentication.
-        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def region(self) -> Optional[str]:
-        """
-        Region for `SIGV4` authentication.
-        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="secretKey")
     def secret_key(self) -> Optional[str]:
-        """
-        Secret key for `SIGV4` authentication.
-        """
         return pulumi.get(self, "secret_key")
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> Optional[str]:
-        """
-        Service name for `SIGV4` authentication.
-        """
         return pulumi.get(self, "service_name")
 
     @property
     @pulumi.getter(name="sessionToken")
     def session_token(self) -> Optional[str]:
-        """
-        Session token for `SIGV4` authentication.
-        """
         return pulumi.get(self, "session_token")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
-        """
-        Type of basic authentication to use when performing the test.
-        """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
-        """
-        Username for authentication.
-        """
         return pulumi.get(self, "username")
 
     @property
     @pulumi.getter
     def workstation(self) -> Optional[str]:
-        """
-        Workstation for `ntlm` authentication.
-        """
         return pulumi.get(self, "workstation")
 
 
 @pulumi.output_type
 class SyntheticsTestApiStepRequestClientCertificate(dict):
     def __init__(__self__, *,
                  cert: 'outputs.SyntheticsTestApiStepRequestClientCertificateCert',
@@ -55963,29 +55066,14 @@
                  no_saving_response_body: Optional[bool] = None,
                  number_of_packets: Optional[int] = None,
                  port: Optional[int] = None,
                  servername: Optional[str] = None,
                  should_track_hops: Optional[bool] = None,
                  timeout: Optional[int] = None,
                  url: Optional[str] = None):
-        """
-        :param str body: The request body.
-        :param str dns_server: DNS server to use for DNS tests (`subtype = "dns"`).
-        :param int dns_server_port: DNS server port to use for DNS tests.
-        :param str host: Host name to perform the test with.
-        :param str message: For UDP and websocket tests, message to send with the request.
-        :param str method: The HTTP method. Valid values are `GET`, `POST`, `PATCH`, `PUT`, `DELETE`, `HEAD`, `OPTIONS`.
-        :param bool no_saving_response_body: Determines whether or not to save the response body.
-        :param int number_of_packets: Number of pings to use per test for ICMP tests (`subtype = "icmp"`) between 0 and 10.
-        :param int port: Port to use when performing the test.
-        :param str servername: For SSL tests, it specifies on which server you want to initiate the TLS handshake, allowing the server to present one of multiple possible certificates on the same IP address and TCP port number.
-        :param bool should_track_hops: This will turn on a traceroute probe to discover all gateways along the path to the host destination. For ICMP tests (`subtype = "icmp"`).
-        :param int timeout: Timeout in seconds for the test. Defaults to `60`.
-        :param str url: The URL to send the request to.
-        """
         if allow_insecure is not None:
             pulumi.set(__self__, "allow_insecure", allow_insecure)
         if body is not None:
             pulumi.set(__self__, "body", body)
         if dns_server is not None:
             pulumi.set(__self__, "dns_server", dns_server)
         if dns_server_port is not None:
@@ -56017,148 +55105,99 @@
     @pulumi.getter(name="allowInsecure")
     def allow_insecure(self) -> Optional[bool]:
         return pulumi.get(self, "allow_insecure")
 
     @property
     @pulumi.getter
     def body(self) -> Optional[str]:
-        """
-        The request body.
-        """
         return pulumi.get(self, "body")
 
     @property
     @pulumi.getter(name="dnsServer")
     def dns_server(self) -> Optional[str]:
-        """
-        DNS server to use for DNS tests (`subtype = "dns"`).
-        """
         return pulumi.get(self, "dns_server")
 
     @property
     @pulumi.getter(name="dnsServerPort")
     def dns_server_port(self) -> Optional[int]:
-        """
-        DNS server port to use for DNS tests.
-        """
         return pulumi.get(self, "dns_server_port")
 
     @property
     @pulumi.getter(name="followRedirects")
     def follow_redirects(self) -> Optional[bool]:
         return pulumi.get(self, "follow_redirects")
 
     @property
     @pulumi.getter
     def host(self) -> Optional[str]:
-        """
-        Host name to perform the test with.
-        """
         return pulumi.get(self, "host")
 
     @property
     @pulumi.getter
     def message(self) -> Optional[str]:
-        """
-        For UDP and websocket tests, message to send with the request.
-        """
         return pulumi.get(self, "message")
 
     @property
     @pulumi.getter
     def method(self) -> Optional[str]:
-        """
-        The HTTP method. Valid values are `GET`, `POST`, `PATCH`, `PUT`, `DELETE`, `HEAD`, `OPTIONS`.
-        """
         return pulumi.get(self, "method")
 
     @property
     @pulumi.getter(name="noSavingResponseBody")
     def no_saving_response_body(self) -> Optional[bool]:
-        """
-        Determines whether or not to save the response body.
-        """
         return pulumi.get(self, "no_saving_response_body")
 
     @property
     @pulumi.getter(name="numberOfPackets")
     def number_of_packets(self) -> Optional[int]:
-        """
-        Number of pings to use per test for ICMP tests (`subtype = "icmp"`) between 0 and 10.
-        """
         return pulumi.get(self, "number_of_packets")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
-        """
-        Port to use when performing the test.
-        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter
     def servername(self) -> Optional[str]:
-        """
-        For SSL tests, it specifies on which server you want to initiate the TLS handshake, allowing the server to present one of multiple possible certificates on the same IP address and TCP port number.
-        """
         return pulumi.get(self, "servername")
 
     @property
     @pulumi.getter(name="shouldTrackHops")
     def should_track_hops(self) -> Optional[bool]:
-        """
-        This will turn on a traceroute probe to discover all gateways along the path to the host destination. For ICMP tests (`subtype = "icmp"`).
-        """
         return pulumi.get(self, "should_track_hops")
 
     @property
     @pulumi.getter
     def timeout(self) -> Optional[int]:
-        """
-        Timeout in seconds for the test. Defaults to `60`.
-        """
         return pulumi.get(self, "timeout")
 
     @property
     @pulumi.getter
     def url(self) -> Optional[str]:
-        """
-        The URL to send the request to.
-        """
         return pulumi.get(self, "url")
 
 
 @pulumi.output_type
 class SyntheticsTestApiStepRequestProxy(dict):
     def __init__(__self__, *,
                  url: str,
                  headers: Optional[Mapping[str, Any]] = None):
-        """
-        :param str url: URL of the proxy to perform the test.
-        :param Mapping[str, Any] headers: Header name and value map.
-        """
         pulumi.set(__self__, "url", url)
         if headers is not None:
             pulumi.set(__self__, "headers", headers)
 
     @property
     @pulumi.getter
     def url(self) -> str:
-        """
-        URL of the proxy to perform the test.
-        """
         return pulumi.get(self, "url")
 
     @property
     @pulumi.getter
     def headers(self) -> Optional[Mapping[str, Any]]:
-        """
-        Header name and value map.
-        """
         return pulumi.get(self, "headers")
 
 
 @pulumi.output_type
 class SyntheticsTestApiStepRetry(dict):
     def __init__(__self__, *,
                  count: Optional[int] = None,
@@ -56183,68 +55222,46 @@
 class SyntheticsTestAssertion(dict):
     def __init__(__self__, *,
                  operator: str,
                  type: str,
                  property: Optional[str] = None,
                  target: Optional[str] = None,
                  targetjsonpath: Optional['outputs.SyntheticsTestAssertionTargetjsonpath'] = None):
-        """
-        :param str operator: Assertion operator. **Note** Only some combinations of `type` and `operator` are valid (please refer to [Datadog documentation](https://docs.datadoghq.com/api/latest/synthetics/#create-a-test)).
-        :param str type: Type of assertion. **Note** Only some combinations of `type` and `operator` are valid (please refer to [Datadog documentation](https://docs.datadoghq.com/api/latest/synthetics/#create-a-test)). Valid values are `body`, `header`, `statusCode`, `certificate`, `responseTime`, `property`, `recordEvery`, `recordSome`, `tlsVersion`, `minTlsVersion`, `latency`, `packetLossPercentage`, `packetsReceived`, `networkHop`, `receivedMessage`.
-        :param str property: If assertion type is `header`, this is the header name.
-        :param str target: Expected value. Depends on the assertion type, refer to [Datadog documentation](https://docs.datadoghq.com/api/latest/synthetics/#create-a-test) for details.
-        :param 'SyntheticsTestAssertionTargetjsonpathArgs' targetjsonpath: Expected structure if `operator` is `validatesJSONPath`. Exactly one nested block is allowed with the structure below.
-        """
         pulumi.set(__self__, "operator", operator)
         pulumi.set(__self__, "type", type)
         if property is not None:
             pulumi.set(__self__, "property", property)
         if target is not None:
             pulumi.set(__self__, "target", target)
         if targetjsonpath is not None:
             pulumi.set(__self__, "targetjsonpath", targetjsonpath)
 
     @property
     @pulumi.getter
     def operator(self) -> str:
-        """
-        Assertion operator. **Note** Only some combinations of `type` and `operator` are valid (please refer to [Datadog documentation](https://docs.datadoghq.com/api/latest/synthetics/#create-a-test)).
-        """
         return pulumi.get(self, "operator")
 
     @property
     @pulumi.getter
     def type(self) -> str:
-        """
-        Type of assertion. **Note** Only some combinations of `type` and `operator` are valid (please refer to [Datadog documentation](https://docs.datadoghq.com/api/latest/synthetics/#create-a-test)). Valid values are `body`, `header`, `statusCode`, `certificate`, `responseTime`, `property`, `recordEvery`, `recordSome`, `tlsVersion`, `minTlsVersion`, `latency`, `packetLossPercentage`, `packetsReceived`, `networkHop`, `receivedMessage`.
-        """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def target(self) -> Optional[str]:
-        """
-        Expected value. Depends on the assertion type, refer to [Datadog documentation](https://docs.datadoghq.com/api/latest/synthetics/#create-a-test) for details.
-        """
         return pulumi.get(self, "target")
 
     @property
     @pulumi.getter
     def targetjsonpath(self) -> Optional['outputs.SyntheticsTestAssertionTargetjsonpath']:
-        """
-        Expected structure if `operator` is `validatesJSONPath`. Exactly one nested block is allowed with the structure below.
-        """
         return pulumi.get(self, "targetjsonpath")
 
     @property
     @pulumi.getter
     def property(self) -> Optional[str]:
-        """
-        If assertion type is `header`, this is the header name.
-        """
         return pulumi.get(self, "property")
 
 
 @pulumi.output_type
 class SyntheticsTestAssertionTargetjsonpath(dict):
     def __init__(__self__, *,
                  jsonpath: str,
@@ -56297,23 +55314,14 @@
                  name: str,
                  params: 'outputs.SyntheticsTestBrowserStepParams',
                  type: str,
                  allow_failure: Optional[bool] = None,
                  force_element_update: Optional[bool] = None,
                  is_critical: Optional[bool] = None,
                  timeout: Optional[int] = None):
-        """
-        :param str name: Name of the step.
-        :param 'SyntheticsTestBrowserStepParamsArgs' params: Parameters for the step.
-        :param str type: Type of the step. Valid values are `assertCurrentUrl`, `assertElementAttribute`, `assertElementContent`, `assertElementPresent`, `assertEmail`, `assertFileDownload`, `assertFromJavascript`, `assertPageContains`, `assertPageLacks`, `click`, `extractFromJavascript`, `extractVariable`, `goToEmailLink`, `goToUrl`, `goToUrlAndMeasureTti`, `hover`, `playSubTest`, `pressKey`, `refresh`, `runApiTest`, `scroll`, `selectOption`, `typeText`, `uploadFiles`, `wait`.
-        :param bool allow_failure: Determines if the step should be allowed to fail.
-        :param bool force_element_update: Force update of the "element" parameter for the step
-        :param bool is_critical: Determines whether or not to consider the entire test as failed if this step fails. Can be used only if `allow_failure` is `true`.
-        :param int timeout: Used to override the default timeout of a step.
-        """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "params", params)
         pulumi.set(__self__, "type", type)
         if allow_failure is not None:
             pulumi.set(__self__, "allow_failure", allow_failure)
         if force_element_update is not None:
             pulumi.set(__self__, "force_element_update", force_element_update)
@@ -56321,65 +55329,44 @@
             pulumi.set(__self__, "is_critical", is_critical)
         if timeout is not None:
             pulumi.set(__self__, "timeout", timeout)
 
     @property
     @pulumi.getter
     def name(self) -> str:
-        """
-        Name of the step.
-        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def params(self) -> 'outputs.SyntheticsTestBrowserStepParams':
-        """
-        Parameters for the step.
-        """
         return pulumi.get(self, "params")
 
     @property
     @pulumi.getter
     def type(self) -> str:
-        """
-        Type of the step. Valid values are `assertCurrentUrl`, `assertElementAttribute`, `assertElementContent`, `assertElementPresent`, `assertEmail`, `assertFileDownload`, `assertFromJavascript`, `assertPageContains`, `assertPageLacks`, `click`, `extractFromJavascript`, `extractVariable`, `goToEmailLink`, `goToUrl`, `goToUrlAndMeasureTti`, `hover`, `playSubTest`, `pressKey`, `refresh`, `runApiTest`, `scroll`, `selectOption`, `typeText`, `uploadFiles`, `wait`.
-        """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter(name="allowFailure")
     def allow_failure(self) -> Optional[bool]:
-        """
-        Determines if the step should be allowed to fail.
-        """
         return pulumi.get(self, "allow_failure")
 
     @property
     @pulumi.getter(name="forceElementUpdate")
     def force_element_update(self) -> Optional[bool]:
-        """
-        Force update of the "element" parameter for the step
-        """
         return pulumi.get(self, "force_element_update")
 
     @property
     @pulumi.getter(name="isCritical")
     def is_critical(self) -> Optional[bool]:
-        """
-        Determines whether or not to consider the entire test as failed if this step fails. Can be used only if `allow_failure` is `true`.
-        """
         return pulumi.get(self, "is_critical")
 
     @property
     @pulumi.getter
     def timeout(self) -> Optional[int]:
-        """
-        Used to override the default timeout of a step.
-        """
         return pulumi.get(self, "timeout")
 
 
 @pulumi.output_type
 class SyntheticsTestBrowserStepParams(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -56599,189 +55586,133 @@
 
 
 @pulumi.output_type
 class SyntheticsTestBrowserStepParamsElementUserLocatorValue(dict):
     def __init__(__self__, *,
                  value: str,
                  type: Optional[str] = None):
-        """
-        :param str type: Synthetics test type. Valid values are `api`, `browser`.
-        """
         pulumi.set(__self__, "value", value)
         if type is not None:
             pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
     def value(self) -> str:
         return pulumi.get(self, "value")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
-        """
-        Synthetics test type. Valid values are `api`, `browser`.
-        """
         return pulumi.get(self, "type")
 
 
 @pulumi.output_type
 class SyntheticsTestBrowserStepParamsVariable(dict):
     def __init__(__self__, *,
                  example: Optional[str] = None,
                  name: Optional[str] = None):
-        """
-        :param str name: Name of Datadog synthetics test.
-        """
         if example is not None:
             pulumi.set(__self__, "example", example)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def example(self) -> Optional[str]:
         return pulumi.get(self, "example")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
-        """
-        Name of Datadog synthetics test.
-        """
         return pulumi.get(self, "name")
 
 
 @pulumi.output_type
 class SyntheticsTestBrowserVariable(dict):
     def __init__(__self__, *,
                  name: str,
                  type: str,
                  example: Optional[str] = None,
                  id: Optional[str] = None,
                  pattern: Optional[str] = None):
-        """
-        :param str name: Name of the variable.
-        :param str type: Type of browser test variable. Valid values are `element`, `email`, `global`, `javascript`, `text`.
-        :param str example: Example for the variable.
-        :param str id: ID of the global variable to use. This is actually only used (and required) in the case of using a variable of type `global`.
-        :param str pattern: Pattern of the variable.
-        """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "type", type)
         if example is not None:
             pulumi.set(__self__, "example", example)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if pattern is not None:
             pulumi.set(__self__, "pattern", pattern)
 
     @property
     @pulumi.getter
     def name(self) -> str:
-        """
-        Name of the variable.
-        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def type(self) -> str:
-        """
-        Type of browser test variable. Valid values are `element`, `email`, `global`, `javascript`, `text`.
-        """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def example(self) -> Optional[str]:
-        """
-        Example for the variable.
-        """
         return pulumi.get(self, "example")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
-        """
-        ID of the global variable to use. This is actually only used (and required) in the case of using a variable of type `global`.
-        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def pattern(self) -> Optional[str]:
-        """
-        Pattern of the variable.
-        """
         return pulumi.get(self, "pattern")
 
 
 @pulumi.output_type
 class SyntheticsTestConfigVariable(dict):
     def __init__(__self__, *,
                  name: str,
                  type: str,
                  example: Optional[str] = None,
                  id: Optional[str] = None,
                  pattern: Optional[str] = None):
-        """
-        :param str name: Name of the variable.
-        :param str type: Type of test configuration variable. Valid values are `global`, `text`.
-        :param str example: Example for the variable.
-        :param str id: When type = `global`, ID of the global variable to use.
-        :param str pattern: Pattern of the variable.
-        """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "type", type)
         if example is not None:
             pulumi.set(__self__, "example", example)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if pattern is not None:
             pulumi.set(__self__, "pattern", pattern)
 
     @property
     @pulumi.getter
     def name(self) -> str:
-        """
-        Name of the variable.
-        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def type(self) -> str:
-        """
-        Type of test configuration variable. Valid values are `global`, `text`.
-        """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def example(self) -> Optional[str]:
-        """
-        Example for the variable.
-        """
         return pulumi.get(self, "example")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
-        """
-        When type = `global`, ID of the global variable to use.
-        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def pattern(self) -> Optional[str]:
-        """
-        Pattern of the variable.
-        """
         return pulumi.get(self, "pattern")
 
 
 @pulumi.output_type
 class SyntheticsTestOptionsList(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -56804,14 +55735,16 @@
             suggest = "monitor_name"
         elif key == "monitorOptions":
             suggest = "monitor_options"
         elif key == "monitorPriority":
             suggest = "monitor_priority"
         elif key == "noScreenshot":
             suggest = "no_screenshot"
+        elif key == "restrictedRoles":
+            suggest = "restricted_roles"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in SyntheticsTestOptionsList. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         SyntheticsTestOptionsList.__key_warning(key)
         return super().__getitem__(key)
@@ -56828,26 +55761,16 @@
                  follow_redirects: Optional[bool] = None,
                  min_failure_duration: Optional[int] = None,
                  min_location_failed: Optional[int] = None,
                  monitor_name: Optional[str] = None,
                  monitor_options: Optional['outputs.SyntheticsTestOptionsListMonitorOptions'] = None,
                  monitor_priority: Optional[int] = None,
                  no_screenshot: Optional[bool] = None,
+                 restricted_roles: Optional[Sequence[str]] = None,
                  retry: Optional['outputs.SyntheticsTestOptionsListRetry'] = None):
-        """
-        :param int tick_every: How often the test should run (in seconds).
-        :param bool accept_self_signed: For SSL test, whether or not the test should allow self signed certificates.
-        :param bool allow_insecure: Allows loading insecure content for an HTTP test.
-        :param bool check_certificate_revocation: For SSL test, whether or not the test should fail on revoked certificate in stapled OCSP.
-        :param bool follow_redirects: Determines whether or not the API HTTP test should follow redirects.
-        :param int min_failure_duration: Minimum amount of time in failure required to trigger an alert. Default is `0`.
-        :param int min_location_failed: Minimum number of locations in failure required to trigger an alert. Default is `1`.
-        :param str monitor_name: The monitor name is used for the alert title as well as for all monitor dashboard widgets and SLOs.
-        :param bool no_screenshot: Prevents saving screenshots of the steps.
-        """
         pulumi.set(__self__, "tick_every", tick_every)
         if accept_self_signed is not None:
             pulumi.set(__self__, "accept_self_signed", accept_self_signed)
         if allow_insecure is not None:
             pulumi.set(__self__, "allow_insecure", allow_insecure)
         if check_certificate_revocation is not None:
             pulumi.set(__self__, "check_certificate_revocation", check_certificate_revocation)
@@ -56861,79 +55784,57 @@
             pulumi.set(__self__, "monitor_name", monitor_name)
         if monitor_options is not None:
             pulumi.set(__self__, "monitor_options", monitor_options)
         if monitor_priority is not None:
             pulumi.set(__self__, "monitor_priority", monitor_priority)
         if no_screenshot is not None:
             pulumi.set(__self__, "no_screenshot", no_screenshot)
+        if restricted_roles is not None:
+            pulumi.set(__self__, "restricted_roles", restricted_roles)
         if retry is not None:
             pulumi.set(__self__, "retry", retry)
 
     @property
     @pulumi.getter(name="tickEvery")
     def tick_every(self) -> int:
-        """
-        How often the test should run (in seconds).
-        """
         return pulumi.get(self, "tick_every")
 
     @property
     @pulumi.getter(name="acceptSelfSigned")
     def accept_self_signed(self) -> Optional[bool]:
-        """
-        For SSL test, whether or not the test should allow self signed certificates.
-        """
         return pulumi.get(self, "accept_self_signed")
 
     @property
     @pulumi.getter(name="allowInsecure")
     def allow_insecure(self) -> Optional[bool]:
-        """
-        Allows loading insecure content for an HTTP test.
-        """
         return pulumi.get(self, "allow_insecure")
 
     @property
     @pulumi.getter(name="checkCertificateRevocation")
     def check_certificate_revocation(self) -> Optional[bool]:
-        """
-        For SSL test, whether or not the test should fail on revoked certificate in stapled OCSP.
-        """
         return pulumi.get(self, "check_certificate_revocation")
 
     @property
     @pulumi.getter(name="followRedirects")
     def follow_redirects(self) -> Optional[bool]:
-        """
-        Determines whether or not the API HTTP test should follow redirects.
-        """
         return pulumi.get(self, "follow_redirects")
 
     @property
     @pulumi.getter(name="minFailureDuration")
     def min_failure_duration(self) -> Optional[int]:
-        """
-        Minimum amount of time in failure required to trigger an alert. Default is `0`.
-        """
         return pulumi.get(self, "min_failure_duration")
 
     @property
     @pulumi.getter(name="minLocationFailed")
     def min_location_failed(self) -> Optional[int]:
-        """
-        Minimum number of locations in failure required to trigger an alert. Default is `1`.
-        """
         return pulumi.get(self, "min_location_failed")
 
     @property
     @pulumi.getter(name="monitorName")
     def monitor_name(self) -> Optional[str]:
-        """
-        The monitor name is used for the alert title as well as for all monitor dashboard widgets and SLOs.
-        """
         return pulumi.get(self, "monitor_name")
 
     @property
     @pulumi.getter(name="monitorOptions")
     def monitor_options(self) -> Optional['outputs.SyntheticsTestOptionsListMonitorOptions']:
         return pulumi.get(self, "monitor_options")
 
@@ -56941,20 +55842,22 @@
     @pulumi.getter(name="monitorPriority")
     def monitor_priority(self) -> Optional[int]:
         return pulumi.get(self, "monitor_priority")
 
     @property
     @pulumi.getter(name="noScreenshot")
     def no_screenshot(self) -> Optional[bool]:
-        """
-        Prevents saving screenshots of the steps.
-        """
         return pulumi.get(self, "no_screenshot")
 
     @property
+    @pulumi.getter(name="restrictedRoles")
+    def restricted_roles(self) -> Optional[Sequence[str]]:
+        return pulumi.get(self, "restricted_roles")
+
+    @property
     @pulumi.getter
     def retry(self) -> Optional['outputs.SyntheticsTestOptionsListRetry']:
         return pulumi.get(self, "retry")
 
 
 @pulumi.output_type
 class SyntheticsTestOptionsListMonitorOptions(dict):
@@ -57039,26 +55942,14 @@
                  region: Optional[str] = None,
                  secret_key: Optional[str] = None,
                  service_name: Optional[str] = None,
                  session_token: Optional[str] = None,
                  type: Optional[str] = None,
                  username: Optional[str] = None,
                  workstation: Optional[str] = None):
-        """
-        :param str access_key: Access key for `SIGV4` authentication.
-        :param str domain: Domain for `ntlm` authentication.
-        :param str password: Password for authentication.
-        :param str region: Region for `SIGV4` authentication.
-        :param str secret_key: Secret key for `SIGV4` authentication.
-        :param str service_name: Service name for `SIGV4` authentication.
-        :param str session_token: Session token for `SIGV4` authentication.
-        :param str type: Type of basic authentication to use when performing the test.
-        :param str username: Username for authentication.
-        :param str workstation: Workstation for `ntlm` authentication.
-        """
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if domain is not None:
             pulumi.set(__self__, "domain", domain)
         if password is not None:
             pulumi.set(__self__, "password", password)
         if region is not None:
@@ -57075,89 +55966,59 @@
             pulumi.set(__self__, "username", username)
         if workstation is not None:
             pulumi.set(__self__, "workstation", workstation)
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
-        """
-        Access key for `SIGV4` authentication.
-        """
         return pulumi.get(self, "access_key")
 
     @property
     @pulumi.getter
     def domain(self) -> Optional[str]:
-        """
-        Domain for `ntlm` authentication.
-        """
         return pulumi.get(self, "domain")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
-        """
-        Password for authentication.
-        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def region(self) -> Optional[str]:
-        """
-        Region for `SIGV4` authentication.
-        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="secretKey")
     def secret_key(self) -> Optional[str]:
-        """
-        Secret key for `SIGV4` authentication.
-        """
         return pulumi.get(self, "secret_key")
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> Optional[str]:
-        """
-        Service name for `SIGV4` authentication.
-        """
         return pulumi.get(self, "service_name")
 
     @property
     @pulumi.getter(name="sessionToken")
     def session_token(self) -> Optional[str]:
-        """
-        Session token for `SIGV4` authentication.
-        """
         return pulumi.get(self, "session_token")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
-        """
-        Type of basic authentication to use when performing the test.
-        """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
-        """
-        Username for authentication.
-        """
         return pulumi.get(self, "username")
 
     @property
     @pulumi.getter
     def workstation(self) -> Optional[str]:
-        """
-        Workstation for `ntlm` authentication.
-        """
         return pulumi.get(self, "workstation")
 
 
 @pulumi.output_type
 class SyntheticsTestRequestClientCertificate(dict):
     def __init__(__self__, *,
                  cert: 'outputs.SyntheticsTestRequestClientCertificateCert',
@@ -57253,29 +56114,14 @@
                  no_saving_response_body: Optional[bool] = None,
                  number_of_packets: Optional[int] = None,
                  port: Optional[int] = None,
                  servername: Optional[str] = None,
                  should_track_hops: Optional[bool] = None,
                  timeout: Optional[int] = None,
                  url: Optional[str] = None):
-        """
-        :param str body: The request body.
-        :param str dns_server: DNS server to use for DNS tests (`subtype = "dns"`).
-        :param int dns_server_port: DNS server port to use for DNS tests.
-        :param str host: Host name to perform the test with.
-        :param str message: For UDP and websocket tests, message to send with the request.
-        :param str method: The HTTP method. Valid values are `GET`, `POST`, `PATCH`, `PUT`, `DELETE`, `HEAD`, `OPTIONS`.
-        :param bool no_saving_response_body: Determines whether or not to save the response body.
-        :param int number_of_packets: Number of pings to use per test for ICMP tests (`subtype = "icmp"`) between 0 and 10.
-        :param int port: Port to use when performing the test.
-        :param str servername: For SSL tests, it specifies on which server you want to initiate the TLS handshake, allowing the server to present one of multiple possible certificates on the same IP address and TCP port number.
-        :param bool should_track_hops: This will turn on a traceroute probe to discover all gateways along the path to the host destination. For ICMP tests (`subtype = "icmp"`).
-        :param int timeout: Timeout in seconds for the test. Defaults to `60`.
-        :param str url: The URL to send the request to.
-        """
         if body is not None:
             pulumi.set(__self__, "body", body)
         if dns_server is not None:
             pulumi.set(__self__, "dns_server", dns_server)
         if dns_server_port is not None:
             pulumi.set(__self__, "dns_server_port", dns_server_port)
         if host is not None:
@@ -57298,157 +56144,105 @@
             pulumi.set(__self__, "timeout", timeout)
         if url is not None:
             pulumi.set(__self__, "url", url)
 
     @property
     @pulumi.getter
     def body(self) -> Optional[str]:
-        """
-        The request body.
-        """
         return pulumi.get(self, "body")
 
     @property
     @pulumi.getter(name="dnsServer")
     def dns_server(self) -> Optional[str]:
-        """
-        DNS server to use for DNS tests (`subtype = "dns"`).
-        """
         return pulumi.get(self, "dns_server")
 
     @property
     @pulumi.getter(name="dnsServerPort")
     def dns_server_port(self) -> Optional[int]:
-        """
-        DNS server port to use for DNS tests.
-        """
         return pulumi.get(self, "dns_server_port")
 
     @property
     @pulumi.getter
     def host(self) -> Optional[str]:
-        """
-        Host name to perform the test with.
-        """
         return pulumi.get(self, "host")
 
     @property
     @pulumi.getter
     def message(self) -> Optional[str]:
-        """
-        For UDP and websocket tests, message to send with the request.
-        """
         return pulumi.get(self, "message")
 
     @property
     @pulumi.getter
     def method(self) -> Optional[str]:
-        """
-        The HTTP method. Valid values are `GET`, `POST`, `PATCH`, `PUT`, `DELETE`, `HEAD`, `OPTIONS`.
-        """
         return pulumi.get(self, "method")
 
     @property
     @pulumi.getter(name="noSavingResponseBody")
     def no_saving_response_body(self) -> Optional[bool]:
-        """
-        Determines whether or not to save the response body.
-        """
         return pulumi.get(self, "no_saving_response_body")
 
     @property
     @pulumi.getter(name="numberOfPackets")
     def number_of_packets(self) -> Optional[int]:
-        """
-        Number of pings to use per test for ICMP tests (`subtype = "icmp"`) between 0 and 10.
-        """
         return pulumi.get(self, "number_of_packets")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
-        """
-        Port to use when performing the test.
-        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter
     def servername(self) -> Optional[str]:
-        """
-        For SSL tests, it specifies on which server you want to initiate the TLS handshake, allowing the server to present one of multiple possible certificates on the same IP address and TCP port number.
-        """
         return pulumi.get(self, "servername")
 
     @property
     @pulumi.getter(name="shouldTrackHops")
     def should_track_hops(self) -> Optional[bool]:
-        """
-        This will turn on a traceroute probe to discover all gateways along the path to the host destination. For ICMP tests (`subtype = "icmp"`).
-        """
         return pulumi.get(self, "should_track_hops")
 
     @property
     @pulumi.getter
     def timeout(self) -> Optional[int]:
-        """
-        Timeout in seconds for the test. Defaults to `60`.
-        """
         return pulumi.get(self, "timeout")
 
     @property
     @pulumi.getter
     def url(self) -> Optional[str]:
-        """
-        The URL to send the request to.
-        """
         return pulumi.get(self, "url")
 
 
 @pulumi.output_type
 class SyntheticsTestRequestProxy(dict):
     def __init__(__self__, *,
                  url: str,
                  headers: Optional[Mapping[str, Any]] = None):
-        """
-        :param str url: URL of the proxy to perform the test.
-        :param Mapping[str, Any] headers: Header name and value map.
-        """
         pulumi.set(__self__, "url", url)
         if headers is not None:
             pulumi.set(__self__, "headers", headers)
 
     @property
     @pulumi.getter
     def url(self) -> str:
-        """
-        URL of the proxy to perform the test.
-        """
         return pulumi.get(self, "url")
 
     @property
     @pulumi.getter
     def headers(self) -> Optional[Mapping[str, Any]]:
-        """
-        Header name and value map.
-        """
         return pulumi.get(self, "headers")
 
 
 @pulumi.output_type
 class GetCloudWorkloadSecurityAgentRulesAgentRuleResult(dict):
     def __init__(__self__, *,
                  description: str,
                  enabled: bool,
                  expression: str,
                  id: str,
                  name: str):
-        """
-        :param str id: The ID of this resource.
-        """
         pulumi.set(__self__, "description", description)
         pulumi.set(__self__, "enabled", enabled)
         pulumi.set(__self__, "expression", expression)
         pulumi.set(__self__, "id", id)
         pulumi.set(__self__, "name", name)
 
     @property
@@ -57465,17 +56259,14 @@
     @pulumi.getter
     def expression(self) -> str:
         return pulumi.get(self, "expression")
 
     @property
     @pulumi.getter
     def id(self) -> str:
-        """
-        The ID of this resource.
-        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         return pulumi.get(self, "name")
 
@@ -57646,27 +56437,21 @@
 
 @pulumi.output_type
 class GetMonitorsMonitorResult(dict):
     def __init__(__self__, *,
                  id: int,
                  name: str,
                  type: str):
-        """
-        :param int id: The ID of this resource.
-        """
         pulumi.set(__self__, "id", id)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
     def id(self) -> int:
-        """
-        The ID of this resource.
-        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         return pulumi.get(self, "name")
 
@@ -57678,27 +56463,21 @@
 
 @pulumi.output_type
 class GetRolesRoleResult(dict):
     def __init__(__self__, *,
                  id: str,
                  name: str,
                  user_count: int):
-        """
-        :param str id: The ID of this resource.
-        """
         pulumi.set(__self__, "id", id)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "user_count", user_count)
 
     @property
     @pulumi.getter
     def id(self) -> str:
-        """
-        The ID of this resource.
-        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         return pulumi.get(self, "name")
 
@@ -57915,21 +56694,24 @@
 @pulumi.output_type
 class GetSecurityMonitoringRulesRuleOptionsResult(dict):
     def __init__(__self__, *,
                  keep_alive: int,
                  max_signal_duration: int,
                  detection_method: Optional[str] = None,
                  evaluation_window: Optional[int] = None,
+                 impossible_travel_options: Optional['outputs.GetSecurityMonitoringRulesRuleOptionsImpossibleTravelOptionsResult'] = None,
                  new_value_options: Optional['outputs.GetSecurityMonitoringRulesRuleOptionsNewValueOptionsResult'] = None):
         pulumi.set(__self__, "keep_alive", keep_alive)
         pulumi.set(__self__, "max_signal_duration", max_signal_duration)
         if detection_method is not None:
             pulumi.set(__self__, "detection_method", detection_method)
         if evaluation_window is not None:
             pulumi.set(__self__, "evaluation_window", evaluation_window)
+        if impossible_travel_options is not None:
+            pulumi.set(__self__, "impossible_travel_options", impossible_travel_options)
         if new_value_options is not None:
             pulumi.set(__self__, "new_value_options", new_value_options)
 
     @property
     @pulumi.getter(name="keepAlive")
     def keep_alive(self) -> int:
         return pulumi.get(self, "keep_alive")
@@ -57946,20 +56728,38 @@
 
     @property
     @pulumi.getter(name="evaluationWindow")
     def evaluation_window(self) -> Optional[int]:
         return pulumi.get(self, "evaluation_window")
 
     @property
+    @pulumi.getter(name="impossibleTravelOptions")
+    def impossible_travel_options(self) -> Optional['outputs.GetSecurityMonitoringRulesRuleOptionsImpossibleTravelOptionsResult']:
+        return pulumi.get(self, "impossible_travel_options")
+
+    @property
     @pulumi.getter(name="newValueOptions")
     def new_value_options(self) -> Optional['outputs.GetSecurityMonitoringRulesRuleOptionsNewValueOptionsResult']:
         return pulumi.get(self, "new_value_options")
 
 
 @pulumi.output_type
+class GetSecurityMonitoringRulesRuleOptionsImpossibleTravelOptionsResult(dict):
+    def __init__(__self__, *,
+                 baseline_user_locations: Optional[bool] = None):
+        if baseline_user_locations is not None:
+            pulumi.set(__self__, "baseline_user_locations", baseline_user_locations)
+
+    @property
+    @pulumi.getter(name="baselineUserLocations")
+    def baseline_user_locations(self) -> Optional[bool]:
+        return pulumi.get(self, "baseline_user_locations")
+
+
+@pulumi.output_type
 class GetSecurityMonitoringRulesRuleOptionsNewValueOptionsResult(dict):
     def __init__(__self__, *,
                  forget_after: int,
                  learning_duration: int):
         pulumi.set(__self__, "forget_after", forget_after)
         pulumi.set(__self__, "learning_duration", learning_duration)
 
@@ -58055,27 +56855,21 @@
 
 @pulumi.output_type
 class GetServiceLevelObjectivesSloResult(dict):
     def __init__(__self__, *,
                  id: str,
                  name: str,
                  type: str):
-        """
-        :param str id: The ID of this resource.
-        """
         pulumi.set(__self__, "id", id)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
     def id(self) -> str:
-        """
-        The ID of this resource.
-        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         return pulumi.get(self, "name")
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/pagerduty/integration.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/pagerduty/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/pagerduty/service_object.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/pagerduty/service_object.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,25 +13,31 @@
 @pulumi.input_type
 class ServiceObjectArgs:
     def __init__(__self__, *,
                  service_key: pulumi.Input[str],
                  service_name: pulumi.Input[str]):
         """
         The set of arguments for constructing a ServiceObject resource.
-        :param pulumi.Input[str] service_key: Your Service name associated service key in PagerDuty. Note: Since the Datadog API never returns service keys, it is impossible to detect drifts.
+        :param pulumi.Input[str] service_key: Your Service name associated service key in PagerDuty. Note: Since the Datadog API never returns service keys, it is
+               impossible to detect [drifts](https://www.hashicorp.com/blog/detecting-and-managing-drift-with-terraform). The best way
+               to solve a drift is to manually mark the Service Object resource with [terraform
+               taint](https://www.terraform.io/docs/commands/taint.html) to have it destroyed and recreated.
         :param pulumi.Input[str] service_name: Your Service name in PagerDuty.
         """
         pulumi.set(__self__, "service_key", service_key)
         pulumi.set(__self__, "service_name", service_name)
 
     @property
     @pulumi.getter(name="serviceKey")
     def service_key(self) -> pulumi.Input[str]:
         """
-        Your Service name associated service key in PagerDuty. Note: Since the Datadog API never returns service keys, it is impossible to detect drifts.
+        Your Service name associated service key in PagerDuty. Note: Since the Datadog API never returns service keys, it is
+        impossible to detect [drifts](https://www.hashicorp.com/blog/detecting-and-managing-drift-with-terraform). The best way
+        to solve a drift is to manually mark the Service Object resource with [terraform
+        taint](https://www.terraform.io/docs/commands/taint.html) to have it destroyed and recreated.
         """
         return pulumi.get(self, "service_key")
 
     @service_key.setter
     def service_key(self, value: pulumi.Input[str]):
         pulumi.set(self, "service_key", value)
 
@@ -51,27 +57,33 @@
 @pulumi.input_type
 class _ServiceObjectState:
     def __init__(__self__, *,
                  service_key: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering ServiceObject resources.
-        :param pulumi.Input[str] service_key: Your Service name associated service key in PagerDuty. Note: Since the Datadog API never returns service keys, it is impossible to detect drifts.
+        :param pulumi.Input[str] service_key: Your Service name associated service key in PagerDuty. Note: Since the Datadog API never returns service keys, it is
+               impossible to detect [drifts](https://www.hashicorp.com/blog/detecting-and-managing-drift-with-terraform). The best way
+               to solve a drift is to manually mark the Service Object resource with [terraform
+               taint](https://www.terraform.io/docs/commands/taint.html) to have it destroyed and recreated.
         :param pulumi.Input[str] service_name: Your Service name in PagerDuty.
         """
         if service_key is not None:
             pulumi.set(__self__, "service_key", service_key)
         if service_name is not None:
             pulumi.set(__self__, "service_name", service_name)
 
     @property
     @pulumi.getter(name="serviceKey")
     def service_key(self) -> Optional[pulumi.Input[str]]:
         """
-        Your Service name associated service key in PagerDuty. Note: Since the Datadog API never returns service keys, it is impossible to detect drifts.
+        Your Service name associated service key in PagerDuty. Note: Since the Datadog API never returns service keys, it is
+        impossible to detect [drifts](https://www.hashicorp.com/blog/detecting-and-managing-drift-with-terraform). The best way
+        to solve a drift is to manually mark the Service Object resource with [terraform
+        taint](https://www.terraform.io/docs/commands/taint.html) to have it destroyed and recreated.
         """
         return pulumi.get(self, "service_key")
 
     @service_key.setter
     def service_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_key", value)
 
@@ -111,15 +123,18 @@
         testing_bar = datadog.pagerduty.ServiceObject("testingBar",
             service_key="54321098765432109876",
             service_name="testing_bar")
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] service_key: Your Service name associated service key in PagerDuty. Note: Since the Datadog API never returns service keys, it is impossible to detect drifts.
+        :param pulumi.Input[str] service_key: Your Service name associated service key in PagerDuty. Note: Since the Datadog API never returns service keys, it is
+               impossible to detect [drifts](https://www.hashicorp.com/blog/detecting-and-managing-drift-with-terraform). The best way
+               to solve a drift is to manually mark the Service Object resource with [terraform
+               taint](https://www.terraform.io/docs/commands/taint.html) to have it destroyed and recreated.
         :param pulumi.Input[str] service_name: Your Service name in PagerDuty.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ServiceObjectArgs,
@@ -191,30 +206,36 @@
         """
         Get an existing ServiceObject resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] service_key: Your Service name associated service key in PagerDuty. Note: Since the Datadog API never returns service keys, it is impossible to detect drifts.
+        :param pulumi.Input[str] service_key: Your Service name associated service key in PagerDuty. Note: Since the Datadog API never returns service keys, it is
+               impossible to detect [drifts](https://www.hashicorp.com/blog/detecting-and-managing-drift-with-terraform). The best way
+               to solve a drift is to manually mark the Service Object resource with [terraform
+               taint](https://www.terraform.io/docs/commands/taint.html) to have it destroyed and recreated.
         :param pulumi.Input[str] service_name: Your Service name in PagerDuty.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ServiceObjectState.__new__(_ServiceObjectState)
 
         __props__.__dict__["service_key"] = service_key
         __props__.__dict__["service_name"] = service_name
         return ServiceObject(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="serviceKey")
     def service_key(self) -> pulumi.Output[str]:
         """
-        Your Service name associated service key in PagerDuty. Note: Since the Datadog API never returns service keys, it is impossible to detect drifts.
+        Your Service name associated service key in PagerDuty. Note: Since the Datadog API never returns service keys, it is
+        impossible to detect [drifts](https://www.hashicorp.com/blog/detecting-and-managing-drift-with-terraform). The best way
+        to solve a drift is to manually mark the Service Object resource with [terraform
+        taint](https://www.terraform.io/docs/commands/taint.html) to have it destroyed and recreated.
         """
         return pulumi.get(self, "service_key")
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/provider.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         """
         The set of arguments for constructing a Provider resource.
         :param pulumi.Input[str] api_key: (Required unless validate is false) Datadog API key. This can also be set via the DD_API_KEY environment variable.
         :param pulumi.Input[str] api_url: The API URL. This can also be set via the DD_HOST environment variable. Note that this URL must not end with the /api/
                path. For example, https://api.datadoghq.com/ is a correct value, while https://api.datadoghq.com/api/ is not. And if
                you're working with "EU" version of Datadog, use https://api.datadoghq.eu/.
         :param pulumi.Input[str] app_key: (Required unless validate is false) Datadog APP key. This can also be set via the DD_APP_KEY environment variable.
-        :param pulumi.Input[bool] http_client_retry_enabled: Enables request retries on HTTP status codes 429 and 5xx.
+        :param pulumi.Input[bool] http_client_retry_enabled: Enables request retries on HTTP status codes 429 and 5xx. Defaults to `true`.
         :param pulumi.Input[int] http_client_retry_timeout: The HTTP request retry timeout period.
         :param pulumi.Input[bool] validate: Enables validation of the provided API and APP keys during provider initialization. Default is true. When false, api_key
                and app_key won't be checked.
         """
         if api_key is not None:
             pulumi.set(__self__, "api_key", api_key)
         if api_url is not None:
@@ -82,15 +82,15 @@
     def app_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "app_key", value)
 
     @property
     @pulumi.getter(name="httpClientRetryEnabled")
     def http_client_retry_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enables request retries on HTTP status codes 429 and 5xx.
+        Enables request retries on HTTP status codes 429 and 5xx. Defaults to `true`.
         """
         return pulumi.get(self, "http_client_retry_enabled")
 
     @http_client_retry_enabled.setter
     def http_client_retry_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "http_client_retry_enabled", value)
 
@@ -141,15 +141,15 @@
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] api_key: (Required unless validate is false) Datadog API key. This can also be set via the DD_API_KEY environment variable.
         :param pulumi.Input[str] api_url: The API URL. This can also be set via the DD_HOST environment variable. Note that this URL must not end with the /api/
                path. For example, https://api.datadoghq.com/ is a correct value, while https://api.datadoghq.com/api/ is not. And if
                you're working with "EU" version of Datadog, use https://api.datadoghq.eu/.
         :param pulumi.Input[str] app_key: (Required unless validate is false) Datadog APP key. This can also be set via the DD_APP_KEY environment variable.
-        :param pulumi.Input[bool] http_client_retry_enabled: Enables request retries on HTTP status codes 429 and 5xx.
+        :param pulumi.Input[bool] http_client_retry_enabled: Enables request retries on HTTP status codes 429 and 5xx. Defaults to `true`.
         :param pulumi.Input[int] http_client_retry_timeout: The HTTP request retry timeout period.
         :param pulumi.Input[bool] validate: Enables validation of the provided API and APP keys during provider initialization. Default is true. When false, api_key
                and app_key won't be checked.
         """
         ...
     @overload
     def __init__(__self__,
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/role.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/security_monitoring_default_rule.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/security_monitoring_default_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/security_monitoring_filter.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/security_monitoring_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                  filtered_data_type: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a SecurityMonitoringFilter resource.
         :param pulumi.Input[bool] is_enabled: Whether the security filter is enabled.
         :param pulumi.Input[str] name: The name of the security filter.
         :param pulumi.Input[str] query: The query of the security filter.
         :param pulumi.Input[Sequence[pulumi.Input['SecurityMonitoringFilterExclusionFilterArgs']]] exclusion_filters: Exclusion filters to exclude some logs from the security filter.
-        :param pulumi.Input[str] filtered_data_type: The filtered data type. Valid values are `logs`.
+        :param pulumi.Input[str] filtered_data_type: The filtered data type.
         """
         pulumi.set(__self__, "is_enabled", is_enabled)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "query", query)
         if exclusion_filters is not None:
             pulumi.set(__self__, "exclusion_filters", exclusion_filters)
         if filtered_data_type is not None:
@@ -84,15 +84,15 @@
     def exclusion_filters(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SecurityMonitoringFilterExclusionFilterArgs']]]]):
         pulumi.set(self, "exclusion_filters", value)
 
     @property
     @pulumi.getter(name="filteredDataType")
     def filtered_data_type(self) -> Optional[pulumi.Input[str]]:
         """
-        The filtered data type. Valid values are `logs`.
+        The filtered data type.
         """
         return pulumi.get(self, "filtered_data_type")
 
     @filtered_data_type.setter
     def filtered_data_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "filtered_data_type", value)
 
@@ -105,15 +105,15 @@
                  is_enabled: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  query: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[int]] = None):
         """
         Input properties used for looking up and filtering SecurityMonitoringFilter resources.
         :param pulumi.Input[Sequence[pulumi.Input['SecurityMonitoringFilterExclusionFilterArgs']]] exclusion_filters: Exclusion filters to exclude some logs from the security filter.
-        :param pulumi.Input[str] filtered_data_type: The filtered data type. Valid values are `logs`.
+        :param pulumi.Input[str] filtered_data_type: The filtered data type.
         :param pulumi.Input[bool] is_enabled: Whether the security filter is enabled.
         :param pulumi.Input[str] name: The name of the security filter.
         :param pulumi.Input[str] query: The query of the security filter.
         :param pulumi.Input[int] version: The version of the security filter.
         """
         if exclusion_filters is not None:
             pulumi.set(__self__, "exclusion_filters", exclusion_filters)
@@ -140,15 +140,15 @@
     def exclusion_filters(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SecurityMonitoringFilterExclusionFilterArgs']]]]):
         pulumi.set(self, "exclusion_filters", value)
 
     @property
     @pulumi.getter(name="filteredDataType")
     def filtered_data_type(self) -> Optional[pulumi.Input[str]]:
         """
-        The filtered data type. Valid values are `logs`.
+        The filtered data type.
         """
         return pulumi.get(self, "filtered_data_type")
 
     @filtered_data_type.setter
     def filtered_data_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "filtered_data_type", value)
 
@@ -244,15 +244,15 @@
         ```sh
          $ pulumi import datadog:index/securityMonitoringFilter:SecurityMonitoringFilter my_filter m0o-hto-lkb
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SecurityMonitoringFilterExclusionFilterArgs']]]] exclusion_filters: Exclusion filters to exclude some logs from the security filter.
-        :param pulumi.Input[str] filtered_data_type: The filtered data type. Valid values are `logs`.
+        :param pulumi.Input[str] filtered_data_type: The filtered data type.
         :param pulumi.Input[bool] is_enabled: Whether the security filter is enabled.
         :param pulumi.Input[str] name: The name of the security filter.
         :param pulumi.Input[str] query: The query of the security filter.
         """
         ...
     @overload
     def __init__(__self__,
@@ -356,15 +356,15 @@
         Get an existing SecurityMonitoringFilter resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SecurityMonitoringFilterExclusionFilterArgs']]]] exclusion_filters: Exclusion filters to exclude some logs from the security filter.
-        :param pulumi.Input[str] filtered_data_type: The filtered data type. Valid values are `logs`.
+        :param pulumi.Input[str] filtered_data_type: The filtered data type.
         :param pulumi.Input[bool] is_enabled: Whether the security filter is enabled.
         :param pulumi.Input[str] name: The name of the security filter.
         :param pulumi.Input[str] query: The query of the security filter.
         :param pulumi.Input[int] version: The version of the security filter.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
@@ -386,15 +386,15 @@
         """
         return pulumi.get(self, "exclusion_filters")
 
     @property
     @pulumi.getter(name="filteredDataType")
     def filtered_data_type(self) -> pulumi.Output[Optional[str]]:
         """
-        The filtered data type. Valid values are `logs`.
+        The filtered data type.
         """
         return pulumi.get(self, "filtered_data_type")
 
     @property
     @pulumi.getter(name="isEnabled")
     def is_enabled(self) -> pulumi.Output[bool]:
         """
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/security_monitoring_rule.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/security_monitoring_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/service_level_objective.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/service_level_objective.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,21 +25,25 @@
                  query: Optional[pulumi.Input['ServiceLevelObjectiveQueryArgs']] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  validate: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a ServiceLevelObjective resource.
         :param pulumi.Input[str] name: Name of Datadog service level objective
         :param pulumi.Input[Sequence[pulumi.Input['ServiceLevelObjectiveThresholdArgs']]] thresholds: A list of thresholds and targets that define the service level objectives from the provided SLIs.
-        :param pulumi.Input[str] type: The type of the service level objective. The mapping from these types to the types found in the Datadog Web UI can be found in the Datadog API [documentation page](https://docs.datadoghq.com/api/v1/service-level-objectives/#create-a-slo-object). Valid values are `metric`, `monitor`.
+        :param pulumi.Input[str] type: The type of the service level objective. The mapping from these types to the types found in the Datadog Web UI can be
+               found in the Datadog API [documentation
+               page](https://docs.datadoghq.com/api/v1/service-level-objectives/#create-a-slo-object).
         :param pulumi.Input[str] description: A description of this service level objective.
         :param pulumi.Input[bool] force_delete: A boolean indicating whether this monitor can be deleted even if it’s referenced by other resources (e.g. dashboards).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: A static set of groups to filter monitor-based SLOs
         :param pulumi.Input[Sequence[pulumi.Input[int]]] monitor_ids: A static set of monitor IDs to use as part of the SLO
         :param pulumi.Input['ServiceLevelObjectiveQueryArgs'] query: The metric query of good / total events
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to associate with your service level objective. This can help you categorize and filter service level objectives in the service level objectives page of the UI. Note: it's not currently possible to filter by these tags when querying via the API
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to associate with your service level objective. This can help you categorize and filter service level
+               objectives in the service level objectives page of the UI. Note: it's not currently possible to filter by these tags
+               when querying via the API
         :param pulumi.Input[bool] validate: Whether or not to validate the SLO.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "thresholds", thresholds)
         pulumi.set(__self__, "type", type)
         if description is not None:
             pulumi.set(__self__, "description", description)
@@ -80,15 +84,17 @@
     def thresholds(self, value: pulumi.Input[Sequence[pulumi.Input['ServiceLevelObjectiveThresholdArgs']]]):
         pulumi.set(self, "thresholds", value)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
         """
-        The type of the service level objective. The mapping from these types to the types found in the Datadog Web UI can be found in the Datadog API [documentation page](https://docs.datadoghq.com/api/v1/service-level-objectives/#create-a-slo-object). Valid values are `metric`, `monitor`.
+        The type of the service level objective. The mapping from these types to the types found in the Datadog Web UI can be
+        found in the Datadog API [documentation
+        page](https://docs.datadoghq.com/api/v1/service-level-objectives/#create-a-slo-object).
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
@@ -152,15 +158,17 @@
     def query(self, value: Optional[pulumi.Input['ServiceLevelObjectiveQueryArgs']]):
         pulumi.set(self, "query", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of tags to associate with your service level objective. This can help you categorize and filter service level objectives in the service level objectives page of the UI. Note: it's not currently possible to filter by these tags when querying via the API
+        A list of tags to associate with your service level objective. This can help you categorize and filter service level
+        objectives in the service level objectives page of the UI. Note: it's not currently possible to filter by these tags
+        when querying via the API
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
@@ -194,17 +202,21 @@
         Input properties used for looking up and filtering ServiceLevelObjective resources.
         :param pulumi.Input[str] description: A description of this service level objective.
         :param pulumi.Input[bool] force_delete: A boolean indicating whether this monitor can be deleted even if it’s referenced by other resources (e.g. dashboards).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: A static set of groups to filter monitor-based SLOs
         :param pulumi.Input[Sequence[pulumi.Input[int]]] monitor_ids: A static set of monitor IDs to use as part of the SLO
         :param pulumi.Input[str] name: Name of Datadog service level objective
         :param pulumi.Input['ServiceLevelObjectiveQueryArgs'] query: The metric query of good / total events
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to associate with your service level objective. This can help you categorize and filter service level objectives in the service level objectives page of the UI. Note: it's not currently possible to filter by these tags when querying via the API
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to associate with your service level objective. This can help you categorize and filter service level
+               objectives in the service level objectives page of the UI. Note: it's not currently possible to filter by these tags
+               when querying via the API
         :param pulumi.Input[Sequence[pulumi.Input['ServiceLevelObjectiveThresholdArgs']]] thresholds: A list of thresholds and targets that define the service level objectives from the provided SLIs.
-        :param pulumi.Input[str] type: The type of the service level objective. The mapping from these types to the types found in the Datadog Web UI can be found in the Datadog API [documentation page](https://docs.datadoghq.com/api/v1/service-level-objectives/#create-a-slo-object). Valid values are `metric`, `monitor`.
+        :param pulumi.Input[str] type: The type of the service level objective. The mapping from these types to the types found in the Datadog Web UI can be
+               found in the Datadog API [documentation
+               page](https://docs.datadoghq.com/api/v1/service-level-objectives/#create-a-slo-object).
         :param pulumi.Input[bool] validate: Whether or not to validate the SLO.
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if force_delete is not None:
             pulumi.set(__self__, "force_delete", force_delete)
         if groups is not None:
@@ -296,15 +308,17 @@
     def query(self, value: Optional[pulumi.Input['ServiceLevelObjectiveQueryArgs']]):
         pulumi.set(self, "query", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of tags to associate with your service level objective. This can help you categorize and filter service level objectives in the service level objectives page of the UI. Note: it's not currently possible to filter by these tags when querying via the API
+        A list of tags to associate with your service level objective. This can help you categorize and filter service level
+        objectives in the service level objectives page of the UI. Note: it's not currently possible to filter by these tags
+        when querying via the API
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
@@ -320,15 +334,17 @@
     def thresholds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceLevelObjectiveThresholdArgs']]]]):
         pulumi.set(self, "thresholds", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        The type of the service level objective. The mapping from these types to the types found in the Datadog Web UI can be found in the Datadog API [documentation page](https://docs.datadoghq.com/api/v1/service-level-objectives/#create-a-slo-object). Valid values are `metric`, `monitor`.
+        The type of the service level objective. The mapping from these types to the types found in the Datadog Web UI can be
+        found in the Datadog API [documentation
+        page](https://docs.datadoghq.com/api/v1/service-level-objectives/#create-a-slo-object).
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -441,17 +457,21 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A description of this service level objective.
         :param pulumi.Input[bool] force_delete: A boolean indicating whether this monitor can be deleted even if it’s referenced by other resources (e.g. dashboards).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: A static set of groups to filter monitor-based SLOs
         :param pulumi.Input[Sequence[pulumi.Input[int]]] monitor_ids: A static set of monitor IDs to use as part of the SLO
         :param pulumi.Input[str] name: Name of Datadog service level objective
         :param pulumi.Input[pulumi.InputType['ServiceLevelObjectiveQueryArgs']] query: The metric query of good / total events
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to associate with your service level objective. This can help you categorize and filter service level objectives in the service level objectives page of the UI. Note: it's not currently possible to filter by these tags when querying via the API
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to associate with your service level objective. This can help you categorize and filter service level
+               objectives in the service level objectives page of the UI. Note: it's not currently possible to filter by these tags
+               when querying via the API
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceLevelObjectiveThresholdArgs']]]] thresholds: A list of thresholds and targets that define the service level objectives from the provided SLIs.
-        :param pulumi.Input[str] type: The type of the service level objective. The mapping from these types to the types found in the Datadog Web UI can be found in the Datadog API [documentation page](https://docs.datadoghq.com/api/v1/service-level-objectives/#create-a-slo-object). Valid values are `metric`, `monitor`.
+        :param pulumi.Input[str] type: The type of the service level objective. The mapping from these types to the types found in the Datadog Web UI can be
+               found in the Datadog API [documentation
+               page](https://docs.datadoghq.com/api/v1/service-level-objectives/#create-a-slo-object).
         :param pulumi.Input[bool] validate: Whether or not to validate the SLO.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ServiceLevelObjectiveArgs,
@@ -614,17 +634,21 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A description of this service level objective.
         :param pulumi.Input[bool] force_delete: A boolean indicating whether this monitor can be deleted even if it’s referenced by other resources (e.g. dashboards).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: A static set of groups to filter monitor-based SLOs
         :param pulumi.Input[Sequence[pulumi.Input[int]]] monitor_ids: A static set of monitor IDs to use as part of the SLO
         :param pulumi.Input[str] name: Name of Datadog service level objective
         :param pulumi.Input[pulumi.InputType['ServiceLevelObjectiveQueryArgs']] query: The metric query of good / total events
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to associate with your service level objective. This can help you categorize and filter service level objectives in the service level objectives page of the UI. Note: it's not currently possible to filter by these tags when querying via the API
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to associate with your service level objective. This can help you categorize and filter service level
+               objectives in the service level objectives page of the UI. Note: it's not currently possible to filter by these tags
+               when querying via the API
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceLevelObjectiveThresholdArgs']]]] thresholds: A list of thresholds and targets that define the service level objectives from the provided SLIs.
-        :param pulumi.Input[str] type: The type of the service level objective. The mapping from these types to the types found in the Datadog Web UI can be found in the Datadog API [documentation page](https://docs.datadoghq.com/api/v1/service-level-objectives/#create-a-slo-object). Valid values are `metric`, `monitor`.
+        :param pulumi.Input[str] type: The type of the service level objective. The mapping from these types to the types found in the Datadog Web UI can be
+               found in the Datadog API [documentation
+               page](https://docs.datadoghq.com/api/v1/service-level-objectives/#create-a-slo-object).
         :param pulumi.Input[bool] validate: Whether or not to validate the SLO.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ServiceLevelObjectiveState.__new__(_ServiceLevelObjectiveState)
 
         __props__.__dict__["description"] = description
@@ -687,15 +711,17 @@
         """
         return pulumi.get(self, "query")
 
     @property
     @pulumi.getter
     def tags(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of tags to associate with your service level objective. This can help you categorize and filter service level objectives in the service level objectives page of the UI. Note: it's not currently possible to filter by these tags when querying via the API
+        A list of tags to associate with your service level objective. This can help you categorize and filter service level
+        objectives in the service level objectives page of the UI. Note: it's not currently possible to filter by these tags
+        when querying via the API
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def thresholds(self) -> pulumi.Output[Sequence['outputs.ServiceLevelObjectiveThreshold']]:
         """
@@ -703,15 +729,17 @@
         """
         return pulumi.get(self, "thresholds")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[str]:
         """
-        The type of the service level objective. The mapping from these types to the types found in the Datadog Web UI can be found in the Datadog API [documentation page](https://docs.datadoghq.com/api/v1/service-level-objectives/#create-a-slo-object). Valid values are `metric`, `monitor`.
+        The type of the service level objective. The mapping from these types to the types found in the Datadog Web UI can be
+        found in the Datadog API [documentation
+        page](https://docs.datadoghq.com/api/v1/service-level-objectives/#create-a-slo-object).
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def validate(self) -> pulumi.Output[Optional[bool]]:
         """
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/slack/_inputs.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/slack/outputs.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,81 +5,47 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
-    'ChannelDisplayArgs',
+    'ChannelDisplay',
 ]
 
-@pulumi.input_type
-class ChannelDisplayArgs:
+@pulumi.output_type
+class ChannelDisplay(dict):
     def __init__(__self__, *,
-                 message: Optional[pulumi.Input[bool]] = None,
-                 notified: Optional[pulumi.Input[bool]] = None,
-                 snapshot: Optional[pulumi.Input[bool]] = None,
-                 tags: Optional[pulumi.Input[bool]] = None):
-        """
-        :param pulumi.Input[bool] message: Show the main body of the alert event.
-        :param pulumi.Input[bool] notified: Show the list of @-handles in the alert event.
-        :param pulumi.Input[bool] snapshot: Show the alert event's snapshot image.
-        :param pulumi.Input[bool] tags: Show the scopes on which the monitor alerted.
-        """
+                 message: Optional[bool] = None,
+                 notified: Optional[bool] = None,
+                 snapshot: Optional[bool] = None,
+                 tags: Optional[bool] = None):
         if message is not None:
             pulumi.set(__self__, "message", message)
         if notified is not None:
             pulumi.set(__self__, "notified", notified)
         if snapshot is not None:
             pulumi.set(__self__, "snapshot", snapshot)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
-    def message(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Show the main body of the alert event.
-        """
+    def message(self) -> Optional[bool]:
         return pulumi.get(self, "message")
 
-    @message.setter
-    def message(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "message", value)
-
     @property
     @pulumi.getter
-    def notified(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Show the list of @-handles in the alert event.
-        """
+    def notified(self) -> Optional[bool]:
         return pulumi.get(self, "notified")
 
-    @notified.setter
-    def notified(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "notified", value)
-
     @property
     @pulumi.getter
-    def snapshot(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Show the alert event's snapshot image.
-        """
+    def snapshot(self) -> Optional[bool]:
         return pulumi.get(self, "snapshot")
 
-    @snapshot.setter
-    def snapshot(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "snapshot", value)
-
     @property
     @pulumi.getter
-    def tags(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Show the scopes on which the monitor alerted.
-        """
+    def tags(self) -> Optional[bool]:
         return pulumi.get(self, "tags")
 
-    @tags.setter
-    def tags(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "tags", value)
-
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/slack/channel.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/slack/channel.py`

 * *Files identical despite different names*

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/slo_correction.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/slo_correction.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,21 +19,22 @@
                  description: Optional[pulumi.Input[str]] = None,
                  duration: Optional[pulumi.Input[int]] = None,
                  end: Optional[pulumi.Input[int]] = None,
                  rrule: Optional[pulumi.Input[str]] = None,
                  timezone: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a SloCorrection resource.
-        :param pulumi.Input[str] category: Category the SLO correction belongs to. Valid values are `Scheduled Maintenance`, `Outside Business Hours`, `Deployment`, `Other`.
+        :param pulumi.Input[str] category: Category the SLO correction belongs to.
         :param pulumi.Input[str] slo_id: ID of the SLO that this correction will be applied to.
         :param pulumi.Input[int] start: Starting time of the correction in epoch seconds.
         :param pulumi.Input[str] description: Description of the correction being made.
         :param pulumi.Input[int] duration: Length of time in seconds for a specified `rrule` recurring SLO correction (required if specifying `rrule`)
         :param pulumi.Input[int] end: Ending time of the correction in epoch seconds. Required for one time corrections, but optional if `rrule` is specified
-        :param pulumi.Input[str] rrule: Recurrence rules as defined in the iCalendar RFC 5545. Supported rules for SLO corrections are `FREQ`, `INTERVAL`, `COUNT` and `UNTIL`.
+        :param pulumi.Input[str] rrule: Recurrence rules as defined in the iCalendar RFC 5545. Supported rules for SLO corrections are `FREQ`, `INTERVAL`,
+               `COUNT` and `UNTIL`.
         :param pulumi.Input[str] timezone: The timezone to display in the UI for the correction times (defaults to "UTC")
         """
         pulumi.set(__self__, "category", category)
         pulumi.set(__self__, "slo_id", slo_id)
         pulumi.set(__self__, "start", start)
         if description is not None:
             pulumi.set(__self__, "description", description)
@@ -46,15 +47,15 @@
         if timezone is not None:
             pulumi.set(__self__, "timezone", timezone)
 
     @property
     @pulumi.getter
     def category(self) -> pulumi.Input[str]:
         """
-        Category the SLO correction belongs to. Valid values are `Scheduled Maintenance`, `Outside Business Hours`, `Deployment`, `Other`.
+        Category the SLO correction belongs to.
         """
         return pulumi.get(self, "category")
 
     @category.setter
     def category(self, value: pulumi.Input[str]):
         pulumi.set(self, "category", value)
 
@@ -118,15 +119,16 @@
     def end(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "end", value)
 
     @property
     @pulumi.getter
     def rrule(self) -> Optional[pulumi.Input[str]]:
         """
-        Recurrence rules as defined in the iCalendar RFC 5545. Supported rules for SLO corrections are `FREQ`, `INTERVAL`, `COUNT` and `UNTIL`.
+        Recurrence rules as defined in the iCalendar RFC 5545. Supported rules for SLO corrections are `FREQ`, `INTERVAL`,
+        `COUNT` and `UNTIL`.
         """
         return pulumi.get(self, "rrule")
 
     @rrule.setter
     def rrule(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "rrule", value)
 
@@ -152,19 +154,20 @@
                  end: Optional[pulumi.Input[int]] = None,
                  rrule: Optional[pulumi.Input[str]] = None,
                  slo_id: Optional[pulumi.Input[str]] = None,
                  start: Optional[pulumi.Input[int]] = None,
                  timezone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering SloCorrection resources.
-        :param pulumi.Input[str] category: Category the SLO correction belongs to. Valid values are `Scheduled Maintenance`, `Outside Business Hours`, `Deployment`, `Other`.
+        :param pulumi.Input[str] category: Category the SLO correction belongs to.
         :param pulumi.Input[str] description: Description of the correction being made.
         :param pulumi.Input[int] duration: Length of time in seconds for a specified `rrule` recurring SLO correction (required if specifying `rrule`)
         :param pulumi.Input[int] end: Ending time of the correction in epoch seconds. Required for one time corrections, but optional if `rrule` is specified
-        :param pulumi.Input[str] rrule: Recurrence rules as defined in the iCalendar RFC 5545. Supported rules for SLO corrections are `FREQ`, `INTERVAL`, `COUNT` and `UNTIL`.
+        :param pulumi.Input[str] rrule: Recurrence rules as defined in the iCalendar RFC 5545. Supported rules for SLO corrections are `FREQ`, `INTERVAL`,
+               `COUNT` and `UNTIL`.
         :param pulumi.Input[str] slo_id: ID of the SLO that this correction will be applied to.
         :param pulumi.Input[int] start: Starting time of the correction in epoch seconds.
         :param pulumi.Input[str] timezone: The timezone to display in the UI for the correction times (defaults to "UTC")
         """
         if category is not None:
             pulumi.set(__self__, "category", category)
         if description is not None:
@@ -182,15 +185,15 @@
         if timezone is not None:
             pulumi.set(__self__, "timezone", timezone)
 
     @property
     @pulumi.getter
     def category(self) -> Optional[pulumi.Input[str]]:
         """
-        Category the SLO correction belongs to. Valid values are `Scheduled Maintenance`, `Outside Business Hours`, `Deployment`, `Other`.
+        Category the SLO correction belongs to.
         """
         return pulumi.get(self, "category")
 
     @category.setter
     def category(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "category", value)
 
@@ -230,15 +233,16 @@
     def end(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "end", value)
 
     @property
     @pulumi.getter
     def rrule(self) -> Optional[pulumi.Input[str]]:
         """
-        Recurrence rules as defined in the iCalendar RFC 5545. Supported rules for SLO corrections are `FREQ`, `INTERVAL`, `COUNT` and `UNTIL`.
+        Recurrence rules as defined in the iCalendar RFC 5545. Supported rules for SLO corrections are `FREQ`, `INTERVAL`,
+        `COUNT` and `UNTIL`.
         """
         return pulumi.get(self, "rrule")
 
     @rrule.setter
     def rrule(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "rrule", value)
 
@@ -338,19 +342,20 @@
 
         ```sh
          $ pulumi import datadog:index/sloCorrection:SloCorrection testing_slo_correction 11111111-3fee-11eb-8a13-77cd9f15119e
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] category: Category the SLO correction belongs to. Valid values are `Scheduled Maintenance`, `Outside Business Hours`, `Deployment`, `Other`.
+        :param pulumi.Input[str] category: Category the SLO correction belongs to.
         :param pulumi.Input[str] description: Description of the correction being made.
         :param pulumi.Input[int] duration: Length of time in seconds for a specified `rrule` recurring SLO correction (required if specifying `rrule`)
         :param pulumi.Input[int] end: Ending time of the correction in epoch seconds. Required for one time corrections, but optional if `rrule` is specified
-        :param pulumi.Input[str] rrule: Recurrence rules as defined in the iCalendar RFC 5545. Supported rules for SLO corrections are `FREQ`, `INTERVAL`, `COUNT` and `UNTIL`.
+        :param pulumi.Input[str] rrule: Recurrence rules as defined in the iCalendar RFC 5545. Supported rules for SLO corrections are `FREQ`, `INTERVAL`,
+               `COUNT` and `UNTIL`.
         :param pulumi.Input[str] slo_id: ID of the SLO that this correction will be applied to.
         :param pulumi.Input[int] start: Starting time of the correction in epoch seconds.
         :param pulumi.Input[str] timezone: The timezone to display in the UI for the correction times (defaults to "UTC")
         """
         ...
     @overload
     def __init__(__self__,
@@ -474,19 +479,20 @@
         """
         Get an existing SloCorrection resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] category: Category the SLO correction belongs to. Valid values are `Scheduled Maintenance`, `Outside Business Hours`, `Deployment`, `Other`.
+        :param pulumi.Input[str] category: Category the SLO correction belongs to.
         :param pulumi.Input[str] description: Description of the correction being made.
         :param pulumi.Input[int] duration: Length of time in seconds for a specified `rrule` recurring SLO correction (required if specifying `rrule`)
         :param pulumi.Input[int] end: Ending time of the correction in epoch seconds. Required for one time corrections, but optional if `rrule` is specified
-        :param pulumi.Input[str] rrule: Recurrence rules as defined in the iCalendar RFC 5545. Supported rules for SLO corrections are `FREQ`, `INTERVAL`, `COUNT` and `UNTIL`.
+        :param pulumi.Input[str] rrule: Recurrence rules as defined in the iCalendar RFC 5545. Supported rules for SLO corrections are `FREQ`, `INTERVAL`,
+               `COUNT` and `UNTIL`.
         :param pulumi.Input[str] slo_id: ID of the SLO that this correction will be applied to.
         :param pulumi.Input[int] start: Starting time of the correction in epoch seconds.
         :param pulumi.Input[str] timezone: The timezone to display in the UI for the correction times (defaults to "UTC")
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SloCorrectionState.__new__(_SloCorrectionState)
@@ -501,15 +507,15 @@
         __props__.__dict__["timezone"] = timezone
         return SloCorrection(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def category(self) -> pulumi.Output[str]:
         """
-        Category the SLO correction belongs to. Valid values are `Scheduled Maintenance`, `Outside Business Hours`, `Deployment`, `Other`.
+        Category the SLO correction belongs to.
         """
         return pulumi.get(self, "category")
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[Optional[str]]:
         """
@@ -533,15 +539,16 @@
         """
         return pulumi.get(self, "end")
 
     @property
     @pulumi.getter
     def rrule(self) -> pulumi.Output[Optional[str]]:
         """
-        Recurrence rules as defined in the iCalendar RFC 5545. Supported rules for SLO corrections are `FREQ`, `INTERVAL`, `COUNT` and `UNTIL`.
+        Recurrence rules as defined in the iCalendar RFC 5545. Supported rules for SLO corrections are `FREQ`, `INTERVAL`,
+        `COUNT` and `UNTIL`.
         """
         return pulumi.get(self, "rrule")
 
     @property
     @pulumi.getter(name="sloId")
     def slo_id(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/synthetics_global_variable.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/synthetics_global_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/synthetics_private_location.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/synthetics_private_location.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,32 +3,38 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
+from . import outputs
+from ._inputs import *
 
 __all__ = ['SyntheticsPrivateLocationArgs', 'SyntheticsPrivateLocation']
 
 @pulumi.input_type
 class SyntheticsPrivateLocationArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  description: Optional[pulumi.Input[str]] = None,
+                 metadata: Optional[pulumi.Input['SyntheticsPrivateLocationMetadataArgs']] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a SyntheticsPrivateLocation resource.
         :param pulumi.Input[str] name: Synthetics private location name.
         :param pulumi.Input[str] description: Description of the private location.
+        :param pulumi.Input['SyntheticsPrivateLocationMetadataArgs'] metadata: The private location metadata
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to associate with your synthetics private location.
         """
         pulumi.set(__self__, "name", name)
         if description is not None:
             pulumi.set(__self__, "description", description)
+        if metadata is not None:
+            pulumi.set(__self__, "metadata", metadata)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
         """
@@ -50,14 +56,26 @@
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
+    def metadata(self) -> Optional[pulumi.Input['SyntheticsPrivateLocationMetadataArgs']]:
+        """
+        The private location metadata
+        """
+        return pulumi.get(self, "metadata")
+
+    @metadata.setter
+    def metadata(self, value: Optional[pulumi.Input['SyntheticsPrivateLocationMetadataArgs']]):
+        pulumi.set(self, "metadata", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         A list of tags to associate with your synthetics private location.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -66,37 +84,43 @@
 
 
 @pulumi.input_type
 class _SyntheticsPrivateLocationState:
     def __init__(__self__, *,
                  config: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
+                 metadata: Optional[pulumi.Input['SyntheticsPrivateLocationMetadataArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering SyntheticsPrivateLocation resources.
-        :param pulumi.Input[str] config: Configuration skeleton for the private location. See installation instructions of the private location on how to use this configuration.
+        :param pulumi.Input[str] config: Configuration skeleton for the private location. See installation instructions of the private location on how to use
+               this configuration.
         :param pulumi.Input[str] description: Description of the private location.
+        :param pulumi.Input['SyntheticsPrivateLocationMetadataArgs'] metadata: The private location metadata
         :param pulumi.Input[str] name: Synthetics private location name.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to associate with your synthetics private location.
         """
         if config is not None:
             pulumi.set(__self__, "config", config)
         if description is not None:
             pulumi.set(__self__, "description", description)
+        if metadata is not None:
+            pulumi.set(__self__, "metadata", metadata)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def config(self) -> Optional[pulumi.Input[str]]:
         """
-        Configuration skeleton for the private location. See installation instructions of the private location on how to use this configuration.
+        Configuration skeleton for the private location. See installation instructions of the private location on how to use
+        this configuration.
         """
         return pulumi.get(self, "config")
 
     @config.setter
     def config(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "config", value)
 
@@ -110,14 +134,26 @@
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
+    def metadata(self) -> Optional[pulumi.Input['SyntheticsPrivateLocationMetadataArgs']]:
+        """
+        The private location metadata
+        """
+        return pulumi.get(self, "metadata")
+
+    @metadata.setter
+    def metadata(self, value: Optional[pulumi.Input['SyntheticsPrivateLocationMetadataArgs']]):
+        pulumi.set(self, "metadata", value)
+
+    @property
+    @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         Synthetics private location name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
@@ -139,14 +175,15 @@
 
 class SyntheticsPrivateLocation(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
+                 metadata: Optional[pulumi.Input[pulumi.InputType['SyntheticsPrivateLocationMetadataArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         Provides a Datadog synthetics private location resource. This can be used to create and manage Datadog synthetics private locations.
 
         ## Example Usage
@@ -171,14 +208,15 @@
         ```sh
          $ pulumi import datadog:index/syntheticsPrivateLocation:SyntheticsPrivateLocation bar pl:private-location-name-abcdef123456
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: Description of the private location.
+        :param pulumi.Input[pulumi.InputType['SyntheticsPrivateLocationMetadataArgs']] metadata: The private location metadata
         :param pulumi.Input[str] name: Synthetics private location name.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to associate with your synthetics private location.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -222,14 +260,15 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
+                 metadata: Optional[pulumi.Input[pulumi.InputType['SyntheticsPrivateLocationMetadataArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
@@ -237,14 +276,15 @@
             opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = SyntheticsPrivateLocationArgs.__new__(SyntheticsPrivateLocationArgs)
 
             __props__.__dict__["description"] = description
+            __props__.__dict__["metadata"] = metadata
             if name is None and not opts.urn:
                 raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
             __props__.__dict__["tags"] = tags
             __props__.__dict__["config"] = None
         super(SyntheticsPrivateLocation, __self__).__init__(
             'datadog:index/syntheticsPrivateLocation:SyntheticsPrivateLocation',
@@ -254,56 +294,69 @@
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             config: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
+            metadata: Optional[pulumi.Input[pulumi.InputType['SyntheticsPrivateLocationMetadataArgs']]] = None,
             name: Optional[pulumi.Input[str]] = None,
             tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'SyntheticsPrivateLocation':
         """
         Get an existing SyntheticsPrivateLocation resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] config: Configuration skeleton for the private location. See installation instructions of the private location on how to use this configuration.
+        :param pulumi.Input[str] config: Configuration skeleton for the private location. See installation instructions of the private location on how to use
+               this configuration.
         :param pulumi.Input[str] description: Description of the private location.
+        :param pulumi.Input[pulumi.InputType['SyntheticsPrivateLocationMetadataArgs']] metadata: The private location metadata
         :param pulumi.Input[str] name: Synthetics private location name.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to associate with your synthetics private location.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SyntheticsPrivateLocationState.__new__(_SyntheticsPrivateLocationState)
 
         __props__.__dict__["config"] = config
         __props__.__dict__["description"] = description
+        __props__.__dict__["metadata"] = metadata
         __props__.__dict__["name"] = name
         __props__.__dict__["tags"] = tags
         return SyntheticsPrivateLocation(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def config(self) -> pulumi.Output[str]:
         """
-        Configuration skeleton for the private location. See installation instructions of the private location on how to use this configuration.
+        Configuration skeleton for the private location. See installation instructions of the private location on how to use
+        this configuration.
         """
         return pulumi.get(self, "config")
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[Optional[str]]:
         """
         Description of the private location.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
+    def metadata(self) -> pulumi.Output[Optional['outputs.SyntheticsPrivateLocationMetadata']]:
+        """
+        The private location metadata
+        """
+        return pulumi.get(self, "metadata")
+
+    @property
+    @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
         Synthetics private location name.
         """
         return pulumi.get(self, "name")
 
     @property
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/synthetics_test.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/synthetics_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,34 +34,40 @@
                  request_proxy: Optional[pulumi.Input['SyntheticsTestRequestProxyArgs']] = None,
                  request_query: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  set_cookie: Optional[pulumi.Input[str]] = None,
                  subtype: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a SyntheticsTest resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] locations: Array of locations used to run the test. Refer to [Datadog documentation](https://docs.datadoghq.com/synthetics/api_test/#request) for available locations (e.g. `aws:eu-central-1`).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] locations: Array of locations used to run the test. Refer to [Datadog
+               documentation](https://docs.datadoghq.com/synthetics/api_test/#request) for available locations (e.g.
+               `aws:eu-central-1`).
         :param pulumi.Input[str] name: Name of Datadog synthetics test.
-        :param pulumi.Input[str] status: Define whether you want to start (`live`) or pause (`paused`) a Synthetic test. Valid values are `live`, `paused`.
-        :param pulumi.Input[str] type: Synthetics test type. Valid values are `api`, `browser`.
+        :param pulumi.Input[str] status: Define whether you want to start (`live`) or pause (`paused`) a Synthetic test.
+        :param pulumi.Input[str] type: Synthetics test type.
         :param pulumi.Input[Sequence[pulumi.Input['SyntheticsTestApiStepArgs']]] api_steps: Steps for multistep api tests
         :param pulumi.Input[Sequence[pulumi.Input['SyntheticsTestAssertionArgs']]] assertions: Assertions used for the test. Multiple `assertion` blocks are allowed with the structure below.
         :param pulumi.Input[Sequence[pulumi.Input['SyntheticsTestBrowserStepArgs']]] browser_steps: Steps for browser tests.
         :param pulumi.Input[Sequence[pulumi.Input['SyntheticsTestBrowserVariableArgs']]] browser_variables: Variables used for a browser test steps. Multiple `variable` blocks are allowed with the structure below.
         :param pulumi.Input[Sequence[pulumi.Input['SyntheticsTestConfigVariableArgs']]] config_variables: Variables used for the test configuration. Multiple `config_variable` blocks are allowed with the structure below.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] device_ids: Required if `type = "browser"`. Array with the different device IDs used to run the test. Valid values are `laptop_large`, `tablet`, `mobile_small`, `chrome.laptop_large`, `chrome.tablet`, `chrome.mobile_small`, `firefox.laptop_large`, `firefox.tablet`, `firefox.mobile_small`, `edge.laptop_large`, `edge.tablet`, `edge.mobile_small`.
-        :param pulumi.Input[str] message: A message to include with notifications for this synthetics test. Email notifications can be sent to specific users by using the same `@username` notation as events.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] device_ids: Required if `type = "browser"`. Array with the different device IDs used to run the test.
+        :param pulumi.Input[str] message: A message to include with notifications for this synthetics test. Email notifications can be sent to specific users by
+               using the same `@username` notation as events.
         :param pulumi.Input['SyntheticsTestRequestBasicauthArgs'] request_basicauth: The HTTP basic authentication credentials. Exactly one nested block is allowed with the structure below.
-        :param pulumi.Input['SyntheticsTestRequestClientCertificateArgs'] request_client_certificate: Client certificate to use when performing the test request. Exactly one nested block is allowed with the structure below.
+        :param pulumi.Input['SyntheticsTestRequestClientCertificateArgs'] request_client_certificate: Client certificate to use when performing the test request. Exactly one nested block is allowed with the structure
+               below.
         :param pulumi.Input['SyntheticsTestRequestDefinitionArgs'] request_definition: Required if `type = "api"`. The synthetics test request.
         :param pulumi.Input[Mapping[str, Any]] request_headers: Header name and value map.
         :param pulumi.Input['SyntheticsTestRequestProxyArgs'] request_proxy: The proxy to perform the test.
         :param pulumi.Input[Mapping[str, Any]] request_query: Query arguments name and value map.
-        :param pulumi.Input[str] set_cookie: Cookies to be used for a browser test request, using the [Set-Cookie](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Set-Cookie) syntax.
-        :param pulumi.Input[str] subtype: The subtype of the Synthetic API test. Defaults to `http`. Valid values are `http`, `ssl`, `tcp`, `dns`, `multi`, `icmp`, `udp`, `websocket`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to associate with your synthetics test. This can help you categorize and filter tests in the manage synthetics page of the UI. Default is an empty list (`[]`).
+        :param pulumi.Input[str] set_cookie: Cookies to be used for a browser test request, using the
+               [Set-Cookie](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Set-Cookie) syntax.
+        :param pulumi.Input[str] subtype: The subtype of the Synthetic API test. Defaults to `http`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to associate with your synthetics test. This can help you categorize and filter tests in the manage
+               synthetics page of the UI. Default is an empty list (`[]`).
         """
         pulumi.set(__self__, "locations", locations)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "status", status)
         pulumi.set(__self__, "type", type)
         if api_steps is not None:
             pulumi.set(__self__, "api_steps", api_steps)
@@ -98,15 +104,17 @@
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def locations(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        Array of locations used to run the test. Refer to [Datadog documentation](https://docs.datadoghq.com/synthetics/api_test/#request) for available locations (e.g. `aws:eu-central-1`).
+        Array of locations used to run the test. Refer to [Datadog
+        documentation](https://docs.datadoghq.com/synthetics/api_test/#request) for available locations (e.g.
+        `aws:eu-central-1`).
         """
         return pulumi.get(self, "locations")
 
     @locations.setter
     def locations(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "locations", value)
 
@@ -122,27 +130,27 @@
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def status(self) -> pulumi.Input[str]:
         """
-        Define whether you want to start (`live`) or pause (`paused`) a Synthetic test. Valid values are `live`, `paused`.
+        Define whether you want to start (`live`) or pause (`paused`) a Synthetic test.
         """
         return pulumi.get(self, "status")
 
     @status.setter
     def status(self, value: pulumi.Input[str]):
         pulumi.set(self, "status", value)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
         """
-        Synthetics test type. Valid values are `api`, `browser`.
+        Synthetics test type.
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
@@ -206,27 +214,28 @@
     def config_variables(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SyntheticsTestConfigVariableArgs']]]]):
         pulumi.set(self, "config_variables", value)
 
     @property
     @pulumi.getter(name="deviceIds")
     def device_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Required if `type = "browser"`. Array with the different device IDs used to run the test. Valid values are `laptop_large`, `tablet`, `mobile_small`, `chrome.laptop_large`, `chrome.tablet`, `chrome.mobile_small`, `firefox.laptop_large`, `firefox.tablet`, `firefox.mobile_small`, `edge.laptop_large`, `edge.tablet`, `edge.mobile_small`.
+        Required if `type = "browser"`. Array with the different device IDs used to run the test.
         """
         return pulumi.get(self, "device_ids")
 
     @device_ids.setter
     def device_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "device_ids", value)
 
     @property
     @pulumi.getter
     def message(self) -> Optional[pulumi.Input[str]]:
         """
-        A message to include with notifications for this synthetics test. Email notifications can be sent to specific users by using the same `@username` notation as events.
+        A message to include with notifications for this synthetics test. Email notifications can be sent to specific users by
+        using the same `@username` notation as events.
         """
         return pulumi.get(self, "message")
 
     @message.setter
     def message(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "message", value)
 
@@ -251,15 +260,16 @@
     def request_basicauth(self, value: Optional[pulumi.Input['SyntheticsTestRequestBasicauthArgs']]):
         pulumi.set(self, "request_basicauth", value)
 
     @property
     @pulumi.getter(name="requestClientCertificate")
     def request_client_certificate(self) -> Optional[pulumi.Input['SyntheticsTestRequestClientCertificateArgs']]:
         """
-        Client certificate to use when performing the test request. Exactly one nested block is allowed with the structure below.
+        Client certificate to use when performing the test request. Exactly one nested block is allowed with the structure
+        below.
         """
         return pulumi.get(self, "request_client_certificate")
 
     @request_client_certificate.setter
     def request_client_certificate(self, value: Optional[pulumi.Input['SyntheticsTestRequestClientCertificateArgs']]):
         pulumi.set(self, "request_client_certificate", value)
 
@@ -311,39 +321,41 @@
     def request_query(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "request_query", value)
 
     @property
     @pulumi.getter(name="setCookie")
     def set_cookie(self) -> Optional[pulumi.Input[str]]:
         """
-        Cookies to be used for a browser test request, using the [Set-Cookie](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Set-Cookie) syntax.
+        Cookies to be used for a browser test request, using the
+        [Set-Cookie](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Set-Cookie) syntax.
         """
         return pulumi.get(self, "set_cookie")
 
     @set_cookie.setter
     def set_cookie(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "set_cookie", value)
 
     @property
     @pulumi.getter
     def subtype(self) -> Optional[pulumi.Input[str]]:
         """
-        The subtype of the Synthetic API test. Defaults to `http`. Valid values are `http`, `ssl`, `tcp`, `dns`, `multi`, `icmp`, `udp`, `websocket`.
+        The subtype of the Synthetic API test. Defaults to `http`.
         """
         return pulumi.get(self, "subtype")
 
     @subtype.setter
     def subtype(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "subtype", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of tags to associate with your synthetics test. This can help you categorize and filter tests in the manage synthetics page of the UI. Default is an empty list (`[]`).
+        A list of tags to associate with your synthetics test. This can help you categorize and filter tests in the manage
+        synthetics page of the UI. Default is an empty list (`[]`).
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
@@ -376,30 +388,36 @@
         """
         Input properties used for looking up and filtering SyntheticsTest resources.
         :param pulumi.Input[Sequence[pulumi.Input['SyntheticsTestApiStepArgs']]] api_steps: Steps for multistep api tests
         :param pulumi.Input[Sequence[pulumi.Input['SyntheticsTestAssertionArgs']]] assertions: Assertions used for the test. Multiple `assertion` blocks are allowed with the structure below.
         :param pulumi.Input[Sequence[pulumi.Input['SyntheticsTestBrowserStepArgs']]] browser_steps: Steps for browser tests.
         :param pulumi.Input[Sequence[pulumi.Input['SyntheticsTestBrowserVariableArgs']]] browser_variables: Variables used for a browser test steps. Multiple `variable` blocks are allowed with the structure below.
         :param pulumi.Input[Sequence[pulumi.Input['SyntheticsTestConfigVariableArgs']]] config_variables: Variables used for the test configuration. Multiple `config_variable` blocks are allowed with the structure below.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] device_ids: Required if `type = "browser"`. Array with the different device IDs used to run the test. Valid values are `laptop_large`, `tablet`, `mobile_small`, `chrome.laptop_large`, `chrome.tablet`, `chrome.mobile_small`, `firefox.laptop_large`, `firefox.tablet`, `firefox.mobile_small`, `edge.laptop_large`, `edge.tablet`, `edge.mobile_small`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] locations: Array of locations used to run the test. Refer to [Datadog documentation](https://docs.datadoghq.com/synthetics/api_test/#request) for available locations (e.g. `aws:eu-central-1`).
-        :param pulumi.Input[str] message: A message to include with notifications for this synthetics test. Email notifications can be sent to specific users by using the same `@username` notation as events.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] device_ids: Required if `type = "browser"`. Array with the different device IDs used to run the test.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] locations: Array of locations used to run the test. Refer to [Datadog
+               documentation](https://docs.datadoghq.com/synthetics/api_test/#request) for available locations (e.g.
+               `aws:eu-central-1`).
+        :param pulumi.Input[str] message: A message to include with notifications for this synthetics test. Email notifications can be sent to specific users by
+               using the same `@username` notation as events.
         :param pulumi.Input[int] monitor_id: ID of the monitor associated with the Datadog synthetics test.
         :param pulumi.Input[str] name: Name of Datadog synthetics test.
         :param pulumi.Input['SyntheticsTestRequestBasicauthArgs'] request_basicauth: The HTTP basic authentication credentials. Exactly one nested block is allowed with the structure below.
-        :param pulumi.Input['SyntheticsTestRequestClientCertificateArgs'] request_client_certificate: Client certificate to use when performing the test request. Exactly one nested block is allowed with the structure below.
+        :param pulumi.Input['SyntheticsTestRequestClientCertificateArgs'] request_client_certificate: Client certificate to use when performing the test request. Exactly one nested block is allowed with the structure
+               below.
         :param pulumi.Input['SyntheticsTestRequestDefinitionArgs'] request_definition: Required if `type = "api"`. The synthetics test request.
         :param pulumi.Input[Mapping[str, Any]] request_headers: Header name and value map.
         :param pulumi.Input['SyntheticsTestRequestProxyArgs'] request_proxy: The proxy to perform the test.
         :param pulumi.Input[Mapping[str, Any]] request_query: Query arguments name and value map.
-        :param pulumi.Input[str] set_cookie: Cookies to be used for a browser test request, using the [Set-Cookie](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Set-Cookie) syntax.
-        :param pulumi.Input[str] status: Define whether you want to start (`live`) or pause (`paused`) a Synthetic test. Valid values are `live`, `paused`.
-        :param pulumi.Input[str] subtype: The subtype of the Synthetic API test. Defaults to `http`. Valid values are `http`, `ssl`, `tcp`, `dns`, `multi`, `icmp`, `udp`, `websocket`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to associate with your synthetics test. This can help you categorize and filter tests in the manage synthetics page of the UI. Default is an empty list (`[]`).
-        :param pulumi.Input[str] type: Synthetics test type. Valid values are `api`, `browser`.
+        :param pulumi.Input[str] set_cookie: Cookies to be used for a browser test request, using the
+               [Set-Cookie](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Set-Cookie) syntax.
+        :param pulumi.Input[str] status: Define whether you want to start (`live`) or pause (`paused`) a Synthetic test.
+        :param pulumi.Input[str] subtype: The subtype of the Synthetic API test. Defaults to `http`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to associate with your synthetics test. This can help you categorize and filter tests in the manage
+               synthetics page of the UI. Default is an empty list (`[]`).
+        :param pulumi.Input[str] type: Synthetics test type.
         """
         if api_steps is not None:
             pulumi.set(__self__, "api_steps", api_steps)
         if assertions is not None:
             pulumi.set(__self__, "assertions", assertions)
         if browser_steps is not None:
             pulumi.set(__self__, "browser_steps", browser_steps)
@@ -502,39 +520,42 @@
     def config_variables(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SyntheticsTestConfigVariableArgs']]]]):
         pulumi.set(self, "config_variables", value)
 
     @property
     @pulumi.getter(name="deviceIds")
     def device_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Required if `type = "browser"`. Array with the different device IDs used to run the test. Valid values are `laptop_large`, `tablet`, `mobile_small`, `chrome.laptop_large`, `chrome.tablet`, `chrome.mobile_small`, `firefox.laptop_large`, `firefox.tablet`, `firefox.mobile_small`, `edge.laptop_large`, `edge.tablet`, `edge.mobile_small`.
+        Required if `type = "browser"`. Array with the different device IDs used to run the test.
         """
         return pulumi.get(self, "device_ids")
 
     @device_ids.setter
     def device_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "device_ids", value)
 
     @property
     @pulumi.getter
     def locations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Array of locations used to run the test. Refer to [Datadog documentation](https://docs.datadoghq.com/synthetics/api_test/#request) for available locations (e.g. `aws:eu-central-1`).
+        Array of locations used to run the test. Refer to [Datadog
+        documentation](https://docs.datadoghq.com/synthetics/api_test/#request) for available locations (e.g.
+        `aws:eu-central-1`).
         """
         return pulumi.get(self, "locations")
 
     @locations.setter
     def locations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "locations", value)
 
     @property
     @pulumi.getter
     def message(self) -> Optional[pulumi.Input[str]]:
         """
-        A message to include with notifications for this synthetics test. Email notifications can be sent to specific users by using the same `@username` notation as events.
+        A message to include with notifications for this synthetics test. Email notifications can be sent to specific users by
+        using the same `@username` notation as events.
         """
         return pulumi.get(self, "message")
 
     @message.setter
     def message(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "message", value)
 
@@ -583,15 +604,16 @@
     def request_basicauth(self, value: Optional[pulumi.Input['SyntheticsTestRequestBasicauthArgs']]):
         pulumi.set(self, "request_basicauth", value)
 
     @property
     @pulumi.getter(name="requestClientCertificate")
     def request_client_certificate(self) -> Optional[pulumi.Input['SyntheticsTestRequestClientCertificateArgs']]:
         """
-        Client certificate to use when performing the test request. Exactly one nested block is allowed with the structure below.
+        Client certificate to use when performing the test request. Exactly one nested block is allowed with the structure
+        below.
         """
         return pulumi.get(self, "request_client_certificate")
 
     @request_client_certificate.setter
     def request_client_certificate(self, value: Optional[pulumi.Input['SyntheticsTestRequestClientCertificateArgs']]):
         pulumi.set(self, "request_client_certificate", value)
 
@@ -643,63 +665,65 @@
     def request_query(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "request_query", value)
 
     @property
     @pulumi.getter(name="setCookie")
     def set_cookie(self) -> Optional[pulumi.Input[str]]:
         """
-        Cookies to be used for a browser test request, using the [Set-Cookie](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Set-Cookie) syntax.
+        Cookies to be used for a browser test request, using the
+        [Set-Cookie](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Set-Cookie) syntax.
         """
         return pulumi.get(self, "set_cookie")
 
     @set_cookie.setter
     def set_cookie(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "set_cookie", value)
 
     @property
     @pulumi.getter
     def status(self) -> Optional[pulumi.Input[str]]:
         """
-        Define whether you want to start (`live`) or pause (`paused`) a Synthetic test. Valid values are `live`, `paused`.
+        Define whether you want to start (`live`) or pause (`paused`) a Synthetic test.
         """
         return pulumi.get(self, "status")
 
     @status.setter
     def status(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "status", value)
 
     @property
     @pulumi.getter
     def subtype(self) -> Optional[pulumi.Input[str]]:
         """
-        The subtype of the Synthetic API test. Defaults to `http`. Valid values are `http`, `ssl`, `tcp`, `dns`, `multi`, `icmp`, `udp`, `websocket`.
+        The subtype of the Synthetic API test. Defaults to `http`.
         """
         return pulumi.get(self, "subtype")
 
     @subtype.setter
     def subtype(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "subtype", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of tags to associate with your synthetics test. This can help you categorize and filter tests in the manage synthetics page of the UI. Default is an empty list (`[]`).
+        A list of tags to associate with your synthetics test. This can help you categorize and filter tests in the manage
+        synthetics page of the UI. Default is an empty list (`[]`).
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        Synthetics test type. Valid values are `api`, `browser`.
+        Synthetics test type.
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -745,20 +769,14 @@
         import pulumi
         ```
 
         to
 
         ```python
         import pulumi
-
-        config_variable = {
-            "name": "LOCAL_VAR",
-            "id": [your_global_variable_id],
-            "type": "global",
-        }
         ```
 
         which you can now use in your request definition:
         ```python
         import pulumi
         ```
 
@@ -777,15 +795,15 @@
                 type="statusCode",
             )],
             locations=["aws:eu-central-1"],
             message="Notify @pagerduty",
             name="An API test on example.org",
             options_list=datadog.SyntheticsTestOptionsListArgs(
                 monitor_options=datadog.SyntheticsTestOptionsListMonitorOptionsArgs(
-                    renotify_interval=100,
+                    renotify_interval=120,
                 ),
                 retry=datadog.SyntheticsTestOptionsListRetryArgs(
                     count=2,
                     interval=300,
                 ),
                 tick_every=900,
             ),
@@ -991,29 +1009,35 @@
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SyntheticsTestApiStepArgs']]]] api_steps: Steps for multistep api tests
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SyntheticsTestAssertionArgs']]]] assertions: Assertions used for the test. Multiple `assertion` blocks are allowed with the structure below.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SyntheticsTestBrowserStepArgs']]]] browser_steps: Steps for browser tests.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SyntheticsTestBrowserVariableArgs']]]] browser_variables: Variables used for a browser test steps. Multiple `variable` blocks are allowed with the structure below.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SyntheticsTestConfigVariableArgs']]]] config_variables: Variables used for the test configuration. Multiple `config_variable` blocks are allowed with the structure below.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] device_ids: Required if `type = "browser"`. Array with the different device IDs used to run the test. Valid values are `laptop_large`, `tablet`, `mobile_small`, `chrome.laptop_large`, `chrome.tablet`, `chrome.mobile_small`, `firefox.laptop_large`, `firefox.tablet`, `firefox.mobile_small`, `edge.laptop_large`, `edge.tablet`, `edge.mobile_small`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] locations: Array of locations used to run the test. Refer to [Datadog documentation](https://docs.datadoghq.com/synthetics/api_test/#request) for available locations (e.g. `aws:eu-central-1`).
-        :param pulumi.Input[str] message: A message to include with notifications for this synthetics test. Email notifications can be sent to specific users by using the same `@username` notation as events.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] device_ids: Required if `type = "browser"`. Array with the different device IDs used to run the test.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] locations: Array of locations used to run the test. Refer to [Datadog
+               documentation](https://docs.datadoghq.com/synthetics/api_test/#request) for available locations (e.g.
+               `aws:eu-central-1`).
+        :param pulumi.Input[str] message: A message to include with notifications for this synthetics test. Email notifications can be sent to specific users by
+               using the same `@username` notation as events.
         :param pulumi.Input[str] name: Name of Datadog synthetics test.
         :param pulumi.Input[pulumi.InputType['SyntheticsTestRequestBasicauthArgs']] request_basicauth: The HTTP basic authentication credentials. Exactly one nested block is allowed with the structure below.
-        :param pulumi.Input[pulumi.InputType['SyntheticsTestRequestClientCertificateArgs']] request_client_certificate: Client certificate to use when performing the test request. Exactly one nested block is allowed with the structure below.
+        :param pulumi.Input[pulumi.InputType['SyntheticsTestRequestClientCertificateArgs']] request_client_certificate: Client certificate to use when performing the test request. Exactly one nested block is allowed with the structure
+               below.
         :param pulumi.Input[pulumi.InputType['SyntheticsTestRequestDefinitionArgs']] request_definition: Required if `type = "api"`. The synthetics test request.
         :param pulumi.Input[Mapping[str, Any]] request_headers: Header name and value map.
         :param pulumi.Input[pulumi.InputType['SyntheticsTestRequestProxyArgs']] request_proxy: The proxy to perform the test.
         :param pulumi.Input[Mapping[str, Any]] request_query: Query arguments name and value map.
-        :param pulumi.Input[str] set_cookie: Cookies to be used for a browser test request, using the [Set-Cookie](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Set-Cookie) syntax.
-        :param pulumi.Input[str] status: Define whether you want to start (`live`) or pause (`paused`) a Synthetic test. Valid values are `live`, `paused`.
-        :param pulumi.Input[str] subtype: The subtype of the Synthetic API test. Defaults to `http`. Valid values are `http`, `ssl`, `tcp`, `dns`, `multi`, `icmp`, `udp`, `websocket`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to associate with your synthetics test. This can help you categorize and filter tests in the manage synthetics page of the UI. Default is an empty list (`[]`).
-        :param pulumi.Input[str] type: Synthetics test type. Valid values are `api`, `browser`.
+        :param pulumi.Input[str] set_cookie: Cookies to be used for a browser test request, using the
+               [Set-Cookie](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Set-Cookie) syntax.
+        :param pulumi.Input[str] status: Define whether you want to start (`live`) or pause (`paused`) a Synthetic test.
+        :param pulumi.Input[str] subtype: The subtype of the Synthetic API test. Defaults to `http`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to associate with your synthetics test. This can help you categorize and filter tests in the manage
+               synthetics page of the UI. Default is an empty list (`[]`).
+        :param pulumi.Input[str] type: Synthetics test type.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: SyntheticsTestArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -1031,20 +1055,14 @@
         import pulumi
         ```
 
         to
 
         ```python
         import pulumi
-
-        config_variable = {
-            "name": "LOCAL_VAR",
-            "id": [your_global_variable_id],
-            "type": "global",
-        }
         ```
 
         which you can now use in your request definition:
         ```python
         import pulumi
         ```
 
@@ -1063,15 +1081,15 @@
                 type="statusCode",
             )],
             locations=["aws:eu-central-1"],
             message="Notify @pagerduty",
             name="An API test on example.org",
             options_list=datadog.SyntheticsTestOptionsListArgs(
                 monitor_options=datadog.SyntheticsTestOptionsListMonitorOptionsArgs(
-                    renotify_interval=100,
+                    renotify_interval=120,
                 ),
                 retry=datadog.SyntheticsTestOptionsListRetryArgs(
                     count=2,
                     interval=300,
                 ),
                 tick_every=900,
             ),
@@ -1392,30 +1410,36 @@
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SyntheticsTestApiStepArgs']]]] api_steps: Steps for multistep api tests
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SyntheticsTestAssertionArgs']]]] assertions: Assertions used for the test. Multiple `assertion` blocks are allowed with the structure below.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SyntheticsTestBrowserStepArgs']]]] browser_steps: Steps for browser tests.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SyntheticsTestBrowserVariableArgs']]]] browser_variables: Variables used for a browser test steps. Multiple `variable` blocks are allowed with the structure below.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SyntheticsTestConfigVariableArgs']]]] config_variables: Variables used for the test configuration. Multiple `config_variable` blocks are allowed with the structure below.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] device_ids: Required if `type = "browser"`. Array with the different device IDs used to run the test. Valid values are `laptop_large`, `tablet`, `mobile_small`, `chrome.laptop_large`, `chrome.tablet`, `chrome.mobile_small`, `firefox.laptop_large`, `firefox.tablet`, `firefox.mobile_small`, `edge.laptop_large`, `edge.tablet`, `edge.mobile_small`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] locations: Array of locations used to run the test. Refer to [Datadog documentation](https://docs.datadoghq.com/synthetics/api_test/#request) for available locations (e.g. `aws:eu-central-1`).
-        :param pulumi.Input[str] message: A message to include with notifications for this synthetics test. Email notifications can be sent to specific users by using the same `@username` notation as events.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] device_ids: Required if `type = "browser"`. Array with the different device IDs used to run the test.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] locations: Array of locations used to run the test. Refer to [Datadog
+               documentation](https://docs.datadoghq.com/synthetics/api_test/#request) for available locations (e.g.
+               `aws:eu-central-1`).
+        :param pulumi.Input[str] message: A message to include with notifications for this synthetics test. Email notifications can be sent to specific users by
+               using the same `@username` notation as events.
         :param pulumi.Input[int] monitor_id: ID of the monitor associated with the Datadog synthetics test.
         :param pulumi.Input[str] name: Name of Datadog synthetics test.
         :param pulumi.Input[pulumi.InputType['SyntheticsTestRequestBasicauthArgs']] request_basicauth: The HTTP basic authentication credentials. Exactly one nested block is allowed with the structure below.
-        :param pulumi.Input[pulumi.InputType['SyntheticsTestRequestClientCertificateArgs']] request_client_certificate: Client certificate to use when performing the test request. Exactly one nested block is allowed with the structure below.
+        :param pulumi.Input[pulumi.InputType['SyntheticsTestRequestClientCertificateArgs']] request_client_certificate: Client certificate to use when performing the test request. Exactly one nested block is allowed with the structure
+               below.
         :param pulumi.Input[pulumi.InputType['SyntheticsTestRequestDefinitionArgs']] request_definition: Required if `type = "api"`. The synthetics test request.
         :param pulumi.Input[Mapping[str, Any]] request_headers: Header name and value map.
         :param pulumi.Input[pulumi.InputType['SyntheticsTestRequestProxyArgs']] request_proxy: The proxy to perform the test.
         :param pulumi.Input[Mapping[str, Any]] request_query: Query arguments name and value map.
-        :param pulumi.Input[str] set_cookie: Cookies to be used for a browser test request, using the [Set-Cookie](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Set-Cookie) syntax.
-        :param pulumi.Input[str] status: Define whether you want to start (`live`) or pause (`paused`) a Synthetic test. Valid values are `live`, `paused`.
-        :param pulumi.Input[str] subtype: The subtype of the Synthetic API test. Defaults to `http`. Valid values are `http`, `ssl`, `tcp`, `dns`, `multi`, `icmp`, `udp`, `websocket`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to associate with your synthetics test. This can help you categorize and filter tests in the manage synthetics page of the UI. Default is an empty list (`[]`).
-        :param pulumi.Input[str] type: Synthetics test type. Valid values are `api`, `browser`.
+        :param pulumi.Input[str] set_cookie: Cookies to be used for a browser test request, using the
+               [Set-Cookie](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Set-Cookie) syntax.
+        :param pulumi.Input[str] status: Define whether you want to start (`live`) or pause (`paused`) a Synthetic test.
+        :param pulumi.Input[str] subtype: The subtype of the Synthetic API test. Defaults to `http`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to associate with your synthetics test. This can help you categorize and filter tests in the manage
+               synthetics page of the UI. Default is an empty list (`[]`).
+        :param pulumi.Input[str] type: Synthetics test type.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SyntheticsTestState.__new__(_SyntheticsTestState)
 
         __props__.__dict__["api_steps"] = api_steps
         __props__.__dict__["assertions"] = assertions
@@ -1481,31 +1505,34 @@
         """
         return pulumi.get(self, "config_variables")
 
     @property
     @pulumi.getter(name="deviceIds")
     def device_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        Required if `type = "browser"`. Array with the different device IDs used to run the test. Valid values are `laptop_large`, `tablet`, `mobile_small`, `chrome.laptop_large`, `chrome.tablet`, `chrome.mobile_small`, `firefox.laptop_large`, `firefox.tablet`, `firefox.mobile_small`, `edge.laptop_large`, `edge.tablet`, `edge.mobile_small`.
+        Required if `type = "browser"`. Array with the different device IDs used to run the test.
         """
         return pulumi.get(self, "device_ids")
 
     @property
     @pulumi.getter
     def locations(self) -> pulumi.Output[Sequence[str]]:
         """
-        Array of locations used to run the test. Refer to [Datadog documentation](https://docs.datadoghq.com/synthetics/api_test/#request) for available locations (e.g. `aws:eu-central-1`).
+        Array of locations used to run the test. Refer to [Datadog
+        documentation](https://docs.datadoghq.com/synthetics/api_test/#request) for available locations (e.g.
+        `aws:eu-central-1`).
         """
         return pulumi.get(self, "locations")
 
     @property
     @pulumi.getter
     def message(self) -> pulumi.Output[Optional[str]]:
         """
-        A message to include with notifications for this synthetics test. Email notifications can be sent to specific users by using the same `@username` notation as events.
+        A message to include with notifications for this synthetics test. Email notifications can be sent to specific users by
+        using the same `@username` notation as events.
         """
         return pulumi.get(self, "message")
 
     @property
     @pulumi.getter(name="monitorId")
     def monitor_id(self) -> pulumi.Output[int]:
         """
@@ -1534,15 +1561,16 @@
         """
         return pulumi.get(self, "request_basicauth")
 
     @property
     @pulumi.getter(name="requestClientCertificate")
     def request_client_certificate(self) -> pulumi.Output[Optional['outputs.SyntheticsTestRequestClientCertificate']]:
         """
-        Client certificate to use when performing the test request. Exactly one nested block is allowed with the structure below.
+        Client certificate to use when performing the test request. Exactly one nested block is allowed with the structure
+        below.
         """
         return pulumi.get(self, "request_client_certificate")
 
     @property
     @pulumi.getter(name="requestDefinition")
     def request_definition(self) -> pulumi.Output[Optional['outputs.SyntheticsTestRequestDefinition']]:
         """
@@ -1574,43 +1602,45 @@
         """
         return pulumi.get(self, "request_query")
 
     @property
     @pulumi.getter(name="setCookie")
     def set_cookie(self) -> pulumi.Output[Optional[str]]:
         """
-        Cookies to be used for a browser test request, using the [Set-Cookie](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Set-Cookie) syntax.
+        Cookies to be used for a browser test request, using the
+        [Set-Cookie](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Set-Cookie) syntax.
         """
         return pulumi.get(self, "set_cookie")
 
     @property
     @pulumi.getter
     def status(self) -> pulumi.Output[str]:
         """
-        Define whether you want to start (`live`) or pause (`paused`) a Synthetic test. Valid values are `live`, `paused`.
+        Define whether you want to start (`live`) or pause (`paused`) a Synthetic test.
         """
         return pulumi.get(self, "status")
 
     @property
     @pulumi.getter
     def subtype(self) -> pulumi.Output[Optional[str]]:
         """
-        The subtype of the Synthetic API test. Defaults to `http`. Valid values are `http`, `ssl`, `tcp`, `dns`, `multi`, `icmp`, `udp`, `websocket`.
+        The subtype of the Synthetic API test. Defaults to `http`.
         """
         return pulumi.get(self, "subtype")
 
     @property
     @pulumi.getter
     def tags(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of tags to associate with your synthetics test. This can help you categorize and filter tests in the manage synthetics page of the UI. Default is an empty list (`[]`).
+        A list of tags to associate with your synthetics test. This can help you categorize and filter tests in the manage
+        synthetics page of the UI. Default is an empty list (`[]`).
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[str]:
         """
-        Synthetics test type. Valid values are `api`, `browser`.
+        Synthetics test type.
         """
         return pulumi.get(self, "type")
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/user.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/webhook.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/webhook.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
                  encode_as: Optional[pulumi.Input[str]] = None,
                  payload: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Webhook resource.
         :param pulumi.Input[str] name: The name of the webhook. It corresponds with `<WEBHOOK_NAME>`.
         :param pulumi.Input[str] url: The URL of the webhook.
         :param pulumi.Input[str] custom_headers: The headers attached to the webhook.
-        :param pulumi.Input[str] encode_as: Encoding type. Valid values are `json`, `form`.
+        :param pulumi.Input[str] encode_as: Encoding type.
         :param pulumi.Input[str] payload: The payload of the webhook.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "url", url)
         if custom_headers is not None:
             pulumi.set(__self__, "custom_headers", custom_headers)
         if encode_as is not None:
@@ -71,15 +71,15 @@
     def custom_headers(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "custom_headers", value)
 
     @property
     @pulumi.getter(name="encodeAs")
     def encode_as(self) -> Optional[pulumi.Input[str]]:
         """
-        Encoding type. Valid values are `json`, `form`.
+        Encoding type.
         """
         return pulumi.get(self, "encode_as")
 
     @encode_as.setter
     def encode_as(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "encode_as", value)
 
@@ -103,15 +103,15 @@
                  encode_as: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  payload: Optional[pulumi.Input[str]] = None,
                  url: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Webhook resources.
         :param pulumi.Input[str] custom_headers: The headers attached to the webhook.
-        :param pulumi.Input[str] encode_as: Encoding type. Valid values are `json`, `form`.
+        :param pulumi.Input[str] encode_as: Encoding type.
         :param pulumi.Input[str] name: The name of the webhook. It corresponds with `<WEBHOOK_NAME>`.
         :param pulumi.Input[str] payload: The payload of the webhook.
         :param pulumi.Input[str] url: The URL of the webhook.
         """
         if custom_headers is not None:
             pulumi.set(__self__, "custom_headers", custom_headers)
         if encode_as is not None:
@@ -135,15 +135,15 @@
     def custom_headers(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "custom_headers", value)
 
     @property
     @pulumi.getter(name="encodeAs")
     def encode_as(self) -> Optional[pulumi.Input[str]]:
         """
-        Encoding type. Valid values are `json`, `form`.
+        Encoding type.
         """
         return pulumi.get(self, "encode_as")
 
     @encode_as.setter
     def encode_as(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "encode_as", value)
 
@@ -223,15 +223,15 @@
         ```sh
          $ pulumi import datadog:index/webhook:Webhook foo example-webhook
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] custom_headers: The headers attached to the webhook.
-        :param pulumi.Input[str] encode_as: Encoding type. Valid values are `json`, `form`.
+        :param pulumi.Input[str] encode_as: Encoding type.
         :param pulumi.Input[str] name: The name of the webhook. It corresponds with `<WEBHOOK_NAME>`.
         :param pulumi.Input[str] payload: The payload of the webhook.
         :param pulumi.Input[str] url: The URL of the webhook.
         """
         ...
     @overload
     def __init__(__self__,
@@ -327,15 +327,15 @@
         Get an existing Webhook resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] custom_headers: The headers attached to the webhook.
-        :param pulumi.Input[str] encode_as: Encoding type. Valid values are `json`, `form`.
+        :param pulumi.Input[str] encode_as: Encoding type.
         :param pulumi.Input[str] name: The name of the webhook. It corresponds with `<WEBHOOK_NAME>`.
         :param pulumi.Input[str] payload: The payload of the webhook.
         :param pulumi.Input[str] url: The URL of the webhook.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _WebhookState.__new__(_WebhookState)
@@ -355,15 +355,15 @@
         """
         return pulumi.get(self, "custom_headers")
 
     @property
     @pulumi.getter(name="encodeAs")
     def encode_as(self) -> pulumi.Output[str]:
         """
-        Encoding type. Valid values are `json`, `form`.
+        Encoding type.
         """
         return pulumi.get(self, "encode_as")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog/webhook_custom_variable.py` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog/webhook_custom_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog.egg-info/PKG-INFO` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-datadog
-Version: 4.9.0a1650908051
+Version: 4.9.0a1653604828
 Summary: A Pulumi package for creating and managing Datadog resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-datadog
 Description: [![Actions Status](https://github.com/pulumi/pulumi-datadog/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-datadog/actions)
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
         [![NPM version](https://badge.fury.io/js/%40pulumi%2Fdatadog.svg)](https://www.npmjs.com/package/@pulumi/datadog)
```

### Comparing `pulumi_datadog-4.9.0a1650908051/pulumi_datadog.egg-info/SOURCES.txt` & `pulumi_datadog-4.9.0a1653604828/pulumi_datadog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_datadog-4.9.0a1650908051/setup.py` & `pulumi_datadog-4.9.0a1653604828/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "4.9.0a1650908051"
-PLUGIN_VERSION = "4.9.0-alpha.1650908051+9ee9dac4"
+VERSION = "4.9.0a1653604828"
+PLUGIN_VERSION = "4.9.0-alpha.1653604828+5135f5e5"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'datadog', PLUGIN_VERSION])
         except OSError as error:
```

