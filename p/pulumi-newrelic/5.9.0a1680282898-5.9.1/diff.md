# Comparing `tmp/pulumi_newrelic-5.9.0a1680282898.tar.gz` & `tmp/pulumi_newrelic-5.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_newrelic-5.9.0a1680282898.tar", last modified: Fri Mar 31 17:21:01 2023, max compression
+gzip compressed data, was "pulumi_newrelic-5.9.1.tar", last modified: Mon Apr 24 23:46:42 2023, max compression
```

## Comparing `pulumi_newrelic-5.9.0a1680282898.tar` & `pulumi_newrelic-5.9.1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:21:01.573843 pulumi_newrelic-5.9.0a1680282898/
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-03-31 17:21:01.573843 pulumi_newrelic-5.9.0a1680282898/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:21:01.565843 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/
--rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   448850 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/account_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    19378 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/alert_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    42951 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/alert_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/alert_muting_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    21313 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/alert_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14505 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/alert_policy_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    20485 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/api_access_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/browser_application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:21:01.569843 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   168479 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/cloud/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60440 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/cloud/aws_govcloud_integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    18999 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/cloud/aws_govcloud_link_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    27596 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/cloud/aws_integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/cloud/aws_link_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    90078 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/cloud/azure_integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    16032 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/cloud/azure_link_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    74614 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/cloud/gcp_integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     9754 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/cloud/gcp_link_account.py
--rw-r--r--   0 runner    (1001) docker     (123)   188009 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/cloud/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:21:01.569843 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    20415 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/data_partition_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/entity_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    15870 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/events_to_metrics_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/get_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/get_alert_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/get_alert_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/get_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/get_cloud_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     9819 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/get_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/get_key_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/get_notification_destination.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/get_obfuscation_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/get_service_level_alert_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/get_test_grok_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    56153 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/infra_alert_condition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:21:01.569843 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/insights/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/insights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/insights/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10052 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/insights/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/insights/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22252 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/log_parsing_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    21098 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/notification_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    25645 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/notification_destination.py
--rw-r--r--   0 runner    (1001) docker     (123)    95474 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/nrql_alert_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)    15708 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/nrql_drop_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/obfuscation_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    17665 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/obfuscation_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    21572 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/one_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/one_dashboard_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    23116 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/one_dashboard_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)   442238 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:21:01.569843 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17030 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/plugins/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14922 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/plugins/application_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/plugins/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31618 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/plugins/workload.py
--rw-r--r--   0 runner    (1001) docker     (123)    18680 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26181 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/service_level.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:21:01.573843 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12981 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19963 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/alert_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)    29006 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/broken_links_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    31102 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/cert_check_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/get_private_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/get_secure_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)    56034 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    30779 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/multi_location_alert_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17171 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/private_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    45717 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/script_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15602 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/secure_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)    32106 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/step_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    41091 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:21:01.565843 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 17:21:01.573843 pulumi_newrelic-5.9.0a1680282898/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-03-31 17:21:01.000000 pulumi_newrelic-5.9.0a1680282898/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:46:42.411032 pulumi_newrelic-5.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-04-24 23:46:42.411032 pulumi_newrelic-5.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:46:42.403032 pulumi_newrelic-5.9.1/pulumi_newrelic/
+-rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   449006 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/account_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20354 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/alert_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42951 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/alert_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/alert_muting_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21313 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/alert_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14505 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/alert_policy_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21983 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/api_access_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/browser_application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:46:42.407032 pulumi_newrelic-5.9.1/pulumi_newrelic/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   168479 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/cloud/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60440 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/cloud/aws_govcloud_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18999 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/cloud/aws_govcloud_link_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27596 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/cloud/aws_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/cloud/aws_link_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90078 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/cloud/azure_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16032 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/cloud/azure_link_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74614 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/cloud/gcp_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9754 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/cloud/gcp_link_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)   188009 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/cloud/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:46:42.407032 pulumi_newrelic-5.9.1/pulumi_newrelic/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20415 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/data_partition_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/entity_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15870 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/events_to_metrics_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/get_alert_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/get_alert_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/get_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/get_cloud_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9819 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/get_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/get_key_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/get_notification_destination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/get_obfuscation_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/get_service_level_alert_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/get_test_grok_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56153 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/infra_alert_condition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:46:42.407032 pulumi_newrelic-5.9.1/pulumi_newrelic/insights/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/insights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/insights/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10052 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/insights/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/insights/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22252 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/log_parsing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21098 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/notification_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25645 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/notification_destination.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95474 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/nrql_alert_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15708 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/nrql_drop_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/obfuscation_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17665 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/obfuscation_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21572 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/one_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/one_dashboard_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23116 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/one_dashboard_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)   442394 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:46:42.407032 pulumi_newrelic-5.9.1/pulumi_newrelic/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17030 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/plugins/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14922 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/plugins/application_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/plugins/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31618 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/plugins/workload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18680 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26181 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/service_level.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:46:42.411032 pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12981 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19963 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/alert_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29006 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/broken_links_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31102 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/cert_check_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/get_private_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/get_secure_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56034 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30779 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/multi_location_alert_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17171 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/private_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45717 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/script_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15602 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/secure_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32106 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/step_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41091 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/pulumi_newrelic/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:46:42.407032 pulumi_newrelic-5.9.1/pulumi_newrelic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-04-24 23:46:42.000000 pulumi_newrelic-5.9.1/pulumi_newrelic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-04-24 23:46:42.000000 pulumi_newrelic-5.9.1/pulumi_newrelic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 23:46:42.000000 pulumi_newrelic-5.9.1/pulumi_newrelic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 23:46:42.000000 pulumi_newrelic-5.9.1/pulumi_newrelic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-24 23:46:42.000000 pulumi_newrelic-5.9.1/pulumi_newrelic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-24 23:46:42.000000 pulumi_newrelic-5.9.1/pulumi_newrelic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 23:46:42.411032 pulumi_newrelic-5.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-24 23:46:41.000000 pulumi_newrelic-5.9.1/setup.py
```

### Comparing `pulumi_newrelic-5.9.0a1680282898/PKG-INFO` & `pulumi_newrelic-5.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_newrelic
-Version: 5.9.0a1680282898
+Version: 5.9.1
 Summary: A Pulumi package for creating and managing New Relic resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-newrelic
 Keywords: pulumi new relic
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_newrelic-5.9.0a1680282898/README.md` & `pulumi_newrelic-5.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/__init__.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/_inputs.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,15 @@
         :param pulumi.Input[str] payload_type: Can either be `application/json` or `application/x-www-form-urlencoded`. The `payload_type` argument is _required_ if `payload` is set.
         :param pulumi.Input[str] recipients: Comma delimited list of email addresses.
         :param pulumi.Input[str] region: The data center region to store your data.  Valid values are `US` and `EU`.  Default is `US`.
         :param pulumi.Input[str] route_key: The route key for integrating with VictorOps.
         :param pulumi.Input[str] service_key: Specifies the service key for integrating with Pagerduty.
         :param pulumi.Input[str] tags: A set of tags for targeting notifications. Multiple values are comma separated.
         :param pulumi.Input[str] teams: A set of teams for targeting notifications. Multiple values are comma separated.
-        :param pulumi.Input[str] url: [Slack Webhook URL](https://slack.com/intl/en-es/help/articles/115005265063-Incoming-webhooks-for-Slack).
+        :param pulumi.Input[str] url: [Slack Webhook URL](https://api.slack.com/messaging/webhooks#create_a_webhook).
         """
         if api_key is not None:
             pulumi.set(__self__, "api_key", api_key)
         if auth_password is not None:
             pulumi.set(__self__, "auth_password", auth_password)
         if auth_type is not None:
             pulumi.set(__self__, "auth_type", auth_type)
@@ -480,15 +480,15 @@
     def teams(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "teams", value)
 
     @property
     @pulumi.getter
     def url(self) -> Optional[pulumi.Input[str]]:
         """
-        [Slack Webhook URL](https://slack.com/intl/en-es/help/articles/115005265063-Incoming-webhooks-for-Slack).
+        [Slack Webhook URL](https://api.slack.com/messaging/webhooks#create_a_webhook).
         """
         return pulumi.get(self, "url")
 
     @url.setter
     def url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "url", value)
 
@@ -8967,15 +8967,15 @@
                  items: Optional[pulumi.Input[Sequence[pulumi.Input['OneDashboardVariableItemArgs']]]] = None,
                  nrql_query: Optional[pulumi.Input['OneDashboardVariableNrqlQueryArgs']] = None):
         """
         :param pulumi.Input[str] name: The title of the dashboard.
         :param pulumi.Input[str] replacement_strategy: (Optional) Indicates the strategy to apply when replacing a variable in a NRQL query. One of `default`, `identifier`, `number` or `string`.
         :param pulumi.Input[str] title: (Optional) A human-friendly display string for this value.
         :param pulumi.Input[str] type: (Required) Specifies the data type of the variable and where its possible values may come from. One of `enum`, `nrql` or `string`
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] default_values: (Optional) A list of default values for this variable.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] default_values: (Optional) A list of default values for this variable. To select **all** default values, the appropriate value to be used with this argument would be `["*"]`.
         :param pulumi.Input[bool] is_multi_selection: (Optional) Indicates whether this variable supports multiple selection or not. Only applies to variables of type `nrql` or `enum`.
         :param pulumi.Input[Sequence[pulumi.Input['OneDashboardVariableItemArgs']]] items: (Optional) List of possible values for variables of type `enum`. See Nested item blocks below for details.
         :param pulumi.Input['OneDashboardVariableNrqlQueryArgs'] nrql_query: (Optional) Configuration for variables of type `nrql`. See Nested nrql\\_query blocks for details.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "replacement_strategy", replacement_strategy)
         pulumi.set(__self__, "title", title)
@@ -9037,15 +9037,15 @@
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter(name="defaultValues")
     def default_values(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        (Optional) A list of default values for this variable.
+        (Optional) A list of default values for this variable. To select **all** default values, the appropriate value to be used with this argument would be `["*"]`.
         """
         return pulumi.get(self, "default_values")
 
     @default_values.setter
     def default_values(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "default_values", value)
```

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/_utilities.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/account_management.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/account_management.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/alert_channel.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/alert_channel.py`

 * *Files 5% similar despite different names*

```diff
@@ -191,14 +191,16 @@
             config=newrelic.AlertChannelConfigArgs(
                 channel="example-alerts-channel",
                 url="https://hooks.slack.com/services/XXXXXXX/XXXXXXX/XXXXXXXXXX",
             ),
             type="slack")
         ```
 
+        > **NOTE:** For instructions on setting up Webhooks with Slack, please visit the article linked under the argument `slack` in the aforementioned configuration, or [this article](https://docs.newrelic.com/docs/alerts-applied-intelligence/new-relic-alerts/alert-notifications/notification-channels-control-where-send-alerts/#slack) in New Relic's docs for additional details on setting up the `New Relic Alerts` Slack application, and subsequently using the generated Webhook URL.
+
         ### OpsGenie
         ```python
         import pulumi
         import pulumi_newrelic as newrelic
 
         foo = newrelic.AlertChannel("foo",
             config=newrelic.AlertChannelConfigArgs(
@@ -323,14 +325,16 @@
             config=newrelic.AlertChannelConfigArgs(
                 channel="example-alerts-channel",
                 url="https://hooks.slack.com/services/XXXXXXX/XXXXXXX/XXXXXXXXXX",
             ),
             type="slack")
         ```
 
+        > **NOTE:** For instructions on setting up Webhooks with Slack, please visit the article linked under the argument `slack` in the aforementioned configuration, or [this article](https://docs.newrelic.com/docs/alerts-applied-intelligence/new-relic-alerts/alert-notifications/notification-channels-control-where-send-alerts/#slack) in New Relic's docs for additional details on setting up the `New Relic Alerts` Slack application, and subsequently using the generated Webhook URL.
+
         ### OpsGenie
         ```python
         import pulumi
         import pulumi_newrelic as newrelic
 
         foo = newrelic.AlertChannel("foo",
             config=newrelic.AlertChannelConfigArgs(
```

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/alert_condition.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/alert_condition.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/alert_muting_rule.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/alert_muting_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/alert_policy.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/alert_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/alert_policy_channel.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/alert_policy_channel.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/api_access_key.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/api_access_key.py`

 * *Files 7% similar despite different names*

```diff
@@ -269,14 +269,16 @@
         foobar = newrelic.ApiAccessKey("foobar",
             account_id=1234567,
             ingest_type="LICENSE",
             key_type="INGEST",
             notes="To be used with service X")
         ```
 
+        > **WARNING:** Creating 'Ingest - License' and 'Ingest - Browser' keys using this resource is restricted to 'core' or 'full platform' New Relic user accounts. If you've signed up as a 'basic' user with New Relic, or have been added as a 'basic' user to your organization on New Relic, you would not be able to use your account to create 'Ingest' keys. If you see the message `"You do not have permission to create this key"` in the response of the API called by this resource, it could be owing to the aforementioned. For more insights into user account types on New Relic and associated privileges, please check out this [page](https://docs.newrelic.com/docs/accounts/accounts-billing/new-relic-one-user-management/user-type/#api-access).
+
         ## Import
 
         Existing API access keys can be imported using a composite ID of `<api_access_key_id>:<key_type>`. `<key_type>` will be either `INGEST` or `USER`. For example
 
         ```sh
          $ pulumi import newrelic:index/apiAccessKey:ApiAccessKey foobar "1234567:INGEST"
         ```
@@ -320,14 +322,16 @@
         foobar = newrelic.ApiAccessKey("foobar",
             account_id=1234567,
             ingest_type="LICENSE",
             key_type="INGEST",
             notes="To be used with service X")
         ```
 
+        > **WARNING:** Creating 'Ingest - License' and 'Ingest - Browser' keys using this resource is restricted to 'core' or 'full platform' New Relic user accounts. If you've signed up as a 'basic' user with New Relic, or have been added as a 'basic' user to your organization on New Relic, you would not be able to use your account to create 'Ingest' keys. If you see the message `"You do not have permission to create this key"` in the response of the API called by this resource, it could be owing to the aforementioned. For more insights into user account types on New Relic and associated privileges, please check out this [page](https://docs.newrelic.com/docs/accounts/accounts-billing/new-relic-one-user-management/user-type/#api-access).
+
         ## Import
 
         Existing API access keys can be imported using a composite ID of `<api_access_key_id>:<key_type>`. `<key_type>` will be either `INGEST` or `USER`. For example
 
         ```sh
          $ pulumi import newrelic:index/apiAccessKey:ApiAccessKey foobar "1234567:INGEST"
         ```
```

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/browser_application.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/browser_application.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/cloud/__init__.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/cloud/_inputs.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/cloud/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/cloud/aws_govcloud_integrations.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/cloud/aws_govcloud_integrations.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/cloud/aws_govcloud_link_account.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/cloud/aws_govcloud_link_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/cloud/aws_integrations.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/cloud/aws_integrations.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/cloud/aws_link_account.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/cloud/aws_link_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/cloud/azure_integrations.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/cloud/azure_integrations.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/cloud/azure_link_account.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/cloud/azure_link_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/cloud/gcp_integrations.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/cloud/gcp_integrations.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/cloud/gcp_link_account.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/cloud/gcp_link_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/cloud/outputs.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/cloud/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/config/vars.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/data_partition_rule.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/data_partition_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/entity_tags.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/entity_tags.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/events_to_metrics_rule.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/events_to_metrics_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/get_account.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/get_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/get_alert_channel.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/get_alert_channel.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/get_alert_policy.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/get_alert_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/get_application.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/get_application.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/get_cloud_account.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/get_cloud_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/get_entity.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/get_entity.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/get_key_transaction.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/get_key_transaction.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/get_notification_destination.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/get_notification_destination.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/get_obfuscation_expression.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/get_obfuscation_expression.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/get_service_level_alert_helper.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/get_service_level_alert_helper.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/get_test_grok_pattern.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/get_test_grok_pattern.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/infra_alert_condition.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/infra_alert_condition.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/insights/_inputs.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/insights/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/insights/event.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/insights/event.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/insights/outputs.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/insights/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/log_parsing_rule.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/log_parsing_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/notification_channel.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/notification_channel.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/notification_destination.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/notification_destination.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/nrql_alert_condition.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/nrql_alert_condition.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/nrql_drop_rule.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/nrql_drop_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/obfuscation_expression.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/obfuscation_expression.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/obfuscation_rule.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/obfuscation_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/one_dashboard.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/one_dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/one_dashboard_json.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/one_dashboard_json.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/one_dashboard_raw.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/one_dashboard_raw.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/outputs.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,15 @@
         :param str payload_type: Can either be `application/json` or `application/x-www-form-urlencoded`. The `payload_type` argument is _required_ if `payload` is set.
         :param str recipients: Comma delimited list of email addresses.
         :param str region: The data center region to store your data.  Valid values are `US` and `EU`.  Default is `US`.
         :param str route_key: The route key for integrating with VictorOps.
         :param str service_key: Specifies the service key for integrating with Pagerduty.
         :param str tags: A set of tags for targeting notifications. Multiple values are comma separated.
         :param str teams: A set of teams for targeting notifications. Multiple values are comma separated.
-        :param str url: [Slack Webhook URL](https://slack.com/intl/en-es/help/articles/115005265063-Incoming-webhooks-for-Slack).
+        :param str url: [Slack Webhook URL](https://api.slack.com/messaging/webhooks#create_a_webhook).
         """
         if api_key is not None:
             pulumi.set(__self__, "api_key", api_key)
         if auth_password is not None:
             pulumi.set(__self__, "auth_password", auth_password)
         if auth_type is not None:
             pulumi.set(__self__, "auth_type", auth_type)
@@ -448,15 +448,15 @@
         """
         return pulumi.get(self, "teams")
 
     @property
     @pulumi.getter
     def url(self) -> Optional[str]:
         """
-        [Slack Webhook URL](https://slack.com/intl/en-es/help/articles/115005265063-Incoming-webhooks-for-Slack).
+        [Slack Webhook URL](https://api.slack.com/messaging/webhooks#create_a_webhook).
         """
         return pulumi.get(self, "url")
 
     @property
     @pulumi.getter(name="userId")
     def user_id(self) -> Optional[str]:
         return pulumi.get(self, "user_id")
@@ -9296,15 +9296,15 @@
                  items: Optional[Sequence['outputs.OneDashboardVariableItem']] = None,
                  nrql_query: Optional['outputs.OneDashboardVariableNrqlQuery'] = None):
         """
         :param str name: The title of the dashboard.
         :param str replacement_strategy: (Optional) Indicates the strategy to apply when replacing a variable in a NRQL query. One of `default`, `identifier`, `number` or `string`.
         :param str title: (Optional) A human-friendly display string for this value.
         :param str type: (Required) Specifies the data type of the variable and where its possible values may come from. One of `enum`, `nrql` or `string`
-        :param Sequence[str] default_values: (Optional) A list of default values for this variable.
+        :param Sequence[str] default_values: (Optional) A list of default values for this variable. To select **all** default values, the appropriate value to be used with this argument would be `["*"]`.
         :param bool is_multi_selection: (Optional) Indicates whether this variable supports multiple selection or not. Only applies to variables of type `nrql` or `enum`.
         :param Sequence['OneDashboardVariableItemArgs'] items: (Optional) List of possible values for variables of type `enum`. See Nested item blocks below for details.
         :param 'OneDashboardVariableNrqlQueryArgs' nrql_query: (Optional) Configuration for variables of type `nrql`. See Nested nrql\\_query blocks for details.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "replacement_strategy", replacement_strategy)
         pulumi.set(__self__, "title", title)
@@ -9350,15 +9350,15 @@
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter(name="defaultValues")
     def default_values(self) -> Optional[Sequence[str]]:
         """
-        (Optional) A list of default values for this variable.
+        (Optional) A list of default values for this variable. To select **all** default values, the appropriate value to be used with this argument would be `["*"]`.
         """
         return pulumi.get(self, "default_values")
 
     @property
     @pulumi.getter(name="isMultiSelection")
     def is_multi_selection(self) -> Optional[bool]:
         """
```

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/plugins/_inputs.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/plugins/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/plugins/application_settings.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/plugins/application_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/plugins/outputs.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/plugins/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/plugins/workload.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/plugins/workload.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/provider.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/service_level.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/service_level.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/__init__.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/_inputs.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/alert_condition.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/alert_condition.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/broken_links_monitor.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/broken_links_monitor.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/cert_check_monitor.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/cert_check_monitor.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/get_private_location.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/get_private_location.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/get_secure_credential.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/get_secure_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/monitor.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/monitor.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/multi_location_alert_condition.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/multi_location_alert_condition.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/outputs.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/private_location.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/private_location.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/script_monitor.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/script_monitor.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/secure_credential.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/secure_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/synthetics/step_monitor.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/synthetics/step_monitor.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic/workflow.py` & `pulumi_newrelic-5.9.1/pulumi_newrelic/workflow.py`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic.egg-info/PKG-INFO` & `pulumi_newrelic-5.9.1/pulumi_newrelic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-newrelic
-Version: 5.9.0a1680282898
+Version: 5.9.1
 Summary: A Pulumi package for creating and managing New Relic resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-newrelic
 Keywords: pulumi new relic
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_newrelic-5.9.0a1680282898/pulumi_newrelic.egg-info/SOURCES.txt` & `pulumi_newrelic-5.9.1/pulumi_newrelic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_newrelic-5.9.0a1680282898/setup.py` & `pulumi_newrelic-5.9.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "5.9.0a1680282898"
-PLUGIN_VERSION = "5.9.0-alpha.1680282898+b0d47700"
+VERSION = "5.9.1"
+PLUGIN_VERSION = "5.9.1"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'newrelic', PLUGIN_VERSION])
         except OSError as error:
```

