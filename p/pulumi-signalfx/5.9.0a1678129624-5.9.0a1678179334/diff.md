# Comparing `tmp/pulumi_signalfx-5.9.0a1678129624.tar.gz` & `tmp/pulumi_signalfx-5.9.0a1678179334.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_signalfx-5.9.0a1678129624.tar", last modified: Mon Mar  6 19:17:34 2023, max compression
+gzip compressed data, was "pulumi_signalfx-5.9.0a1678179334.tar", last modified: Tue Mar  7 09:00:07 2023, max compression
```

## Comparing `pulumi_signalfx-5.9.0a1678129624.tar` & `pulumi_signalfx-5.9.0a1678179334.tar`

### file list

```diff
@@ -1,85 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:17:34.903772 pulumi_signalfx-5.9.0a1678129624/
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-03-06 19:17:34.899773 pulumi_signalfx-5.9.0a1678129624/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:17:34.895773 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/
--rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   130493 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    19485 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/alert_muting_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:17:34.895773 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/aws/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19473 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/aws/external_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/aws/get_services.py
--rw-r--r--   0 runner    (1001) docker     (123)    80393 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/aws/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/aws/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/aws/token_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:17:34.899773 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/azure/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/azure/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/azure/get_services.py
--rw-r--r--   0 runner    (1001) docker     (123)    55951 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/azure/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/azure/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:17:34.899773 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    60438 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    34779 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/dashboard_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    23028 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/data_link.py
--rw-r--r--   0 runner    (1001) docker     (123)    62286 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/detector.py
--rw-r--r--   0 runner    (1001) docker     (123)    17671 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/event_feed_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:17:34.899773 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/gcp/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/gcp/get_services.py
--rw-r--r--   0 runner    (1001) docker     (123)    34418 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/gcp/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/gcp/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/get_aws_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/get_azure_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/get_dimension_values.py
--rw-r--r--   0 runner    (1001) docker     (123)    42295 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/heatmap_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:17:34.899773 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/jira/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/jira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32032 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/jira/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    62121 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/list_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:17:34.899773 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/logs/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/logs/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28303 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/logs/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:17:34.899773 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/opsgenie/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/opsgenie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/opsgenie/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    22917 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/org_token.py
--rw-r--r--   0 runner    (1001) docker     (123)   118495 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:17:34.899773 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/pagerduty/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/pagerduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/pagerduty/get_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10115 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/pagerduty/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:17:34.899773 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/servicenow/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/servicenow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27661 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/servicenow/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    40263 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/single_value_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:17:34.899773 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/slack/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/slack/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    31617 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/table_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)    27565 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/team.py
--rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/text_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)    78926 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/time_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:17:34.899773 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/victorops/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/victorops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10136 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/victorops/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/webhook_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:17:34.895773 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 19:17:34.903772 pulumi_signalfx-5.9.0a1678129624/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-03-06 19:17:34.000000 pulumi_signalfx-5.9.0a1678129624/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:07.055112 pulumi_signalfx-5.9.0a1678179334/
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-03-07 09:00:07.055112 pulumi_signalfx-5.9.0a1678179334/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:07.047111 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/
+-rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   139415 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19485 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/alert_muting_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:07.051112 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/aws/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19473 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/aws/external_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/aws/get_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80393 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/aws/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/aws/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/aws/token_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:07.051112 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/azure/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/azure/get_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55951 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/azure/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/azure/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:07.051112 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60438 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34779 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/dashboard_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23028 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/data_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62286 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17671 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/event_feed_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:07.051112 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/gcp/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/gcp/get_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34418 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/gcp/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/gcp/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/get_aws_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/get_azure_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/get_dimension_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42295 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/heatmap_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:07.051112 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/jira/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/jira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32032 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/jira/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62121 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/list_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:07.051112 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/logs/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/logs/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28303 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/logs/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17643 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/metric_ruleset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:07.051112 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/opsgenie/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/opsgenie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/opsgenie/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22917 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/org_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)   126160 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:07.051112 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/pagerduty/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/pagerduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/pagerduty/get_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10115 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/pagerduty/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11666 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:07.051112 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/servicenow/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/servicenow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27661 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/servicenow/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40263 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/single_value_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:07.055112 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/slack/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31617 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/table_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27565 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/text_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78926 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/time_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:07.055112 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/victorops/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/victorops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10136 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/victorops/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/webhook_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:07.051112 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-03-07 09:00:07.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-03-07 09:00:07.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 09:00:07.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 09:00:07.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-07 09:00:07.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-07 09:00:07.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 09:00:07.055112 pulumi_signalfx-5.9.0a1678179334/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/setup.py
```

### Comparing `pulumi_signalfx-5.9.0a1678129624/PKG-INFO` & `pulumi_signalfx-5.9.0a1678179334/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_signalfx
-Version: 5.9.0a1678129624
+Version: 5.9.0a1678179334
 Summary: A Pulumi package for creating and managing SignalFx resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-signalfx
 Keywords: pulumi signalfx
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_signalfx-5.9.0a1678129624/README.md` & `pulumi_signalfx-5.9.0a1678179334/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/__init__.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from .detector import *
 from .event_feed_chart import *
 from .get_aws_services import *
 from .get_azure_services import *
 from .get_dimension_values import *
 from .heatmap_chart import *
 from .list_chart import *
+from .metric_ruleset import *
 from .org_token import *
 from .provider import *
 from .single_value_chart import *
 from .table_chart import *
 from .team import *
 from .text_chart import *
 from .time_chart import *
@@ -169,14 +170,22 @@
   "fqn": "pulumi_signalfx",
   "classes": {
    "signalfx:index/listChart:ListChart": "ListChart"
   }
  },
  {
   "pkg": "signalfx",
+  "mod": "index/metricRuleset",
+  "fqn": "pulumi_signalfx",
+  "classes": {
+   "signalfx:index/metricRuleset:MetricRuleset": "MetricRuleset"
+  }
+ },
+ {
+  "pkg": "signalfx",
   "mod": "index/orgToken",
   "fqn": "pulumi_signalfx",
   "classes": {
    "signalfx:index/orgToken:OrgToken": "OrgToken"
   }
  },
  {
```

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/_inputs.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/_inputs.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,19 @@
     'DetectorRuleArgs',
     'DetectorVizOptionArgs',
     'HeatmapChartColorRangeArgs',
     'HeatmapChartColorScaleArgs',
     'ListChartColorScaleArgs',
     'ListChartLegendOptionsFieldArgs',
     'ListChartVizOptionArgs',
+    'MetricRulesetAggregationRuleArgs',
+    'MetricRulesetAggregationRuleAggregatorArgs',
+    'MetricRulesetAggregationRuleMatcherArgs',
+    'MetricRulesetAggregationRuleMatcherFilterArgs',
+    'MetricRulesetRoutingRuleArgs',
     'OrgTokenDpmLimitsArgs',
     'OrgTokenHostOrUsageLimitsArgs',
     'SingleValueChartColorScaleArgs',
     'SingleValueChartVizOptionArgs',
     'TableChartVizOptionArgs',
     'TimeChartAxisLeftArgs',
     'TimeChartAxisLeftWatermarkArgs',
@@ -2024,14 +2029,257 @@
 
     @value_unit.setter
     def value_unit(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "value_unit", value)
 
 
 @pulumi.input_type
+class MetricRulesetAggregationRuleArgs:
+    def __init__(__self__, *,
+                 aggregators: pulumi.Input[Sequence[pulumi.Input['MetricRulesetAggregationRuleAggregatorArgs']]],
+                 enabled: pulumi.Input[bool],
+                 matchers: pulumi.Input[Sequence[pulumi.Input['MetricRulesetAggregationRuleMatcherArgs']]],
+                 name: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[Sequence[pulumi.Input['MetricRulesetAggregationRuleAggregatorArgs']]] aggregators: Aggregator object
+        :param pulumi.Input[bool] enabled: When false, this rule will not generate aggregated MTSs
+        :param pulumi.Input[Sequence[pulumi.Input['MetricRulesetAggregationRuleMatcherArgs']]] matchers: Matcher object
+        """
+        pulumi.set(__self__, "aggregators", aggregators)
+        pulumi.set(__self__, "enabled", enabled)
+        pulumi.set(__self__, "matchers", matchers)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+
+    @property
+    @pulumi.getter
+    def aggregators(self) -> pulumi.Input[Sequence[pulumi.Input['MetricRulesetAggregationRuleAggregatorArgs']]]:
+        """
+        Aggregator object
+        """
+        return pulumi.get(self, "aggregators")
+
+    @aggregators.setter
+    def aggregators(self, value: pulumi.Input[Sequence[pulumi.Input['MetricRulesetAggregationRuleAggregatorArgs']]]):
+        pulumi.set(self, "aggregators", value)
+
+    @property
+    @pulumi.getter
+    def enabled(self) -> pulumi.Input[bool]:
+        """
+        When false, this rule will not generate aggregated MTSs
+        """
+        return pulumi.get(self, "enabled")
+
+    @enabled.setter
+    def enabled(self, value: pulumi.Input[bool]):
+        pulumi.set(self, "enabled", value)
+
+    @property
+    @pulumi.getter
+    def matchers(self) -> pulumi.Input[Sequence[pulumi.Input['MetricRulesetAggregationRuleMatcherArgs']]]:
+        """
+        Matcher object
+        """
+        return pulumi.get(self, "matchers")
+
+    @matchers.setter
+    def matchers(self, value: pulumi.Input[Sequence[pulumi.Input['MetricRulesetAggregationRuleMatcherArgs']]]):
+        pulumi.set(self, "matchers", value)
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
+
+@pulumi.input_type
+class MetricRulesetAggregationRuleAggregatorArgs:
+    def __init__(__self__, *,
+                 dimensions: pulumi.Input[Sequence[pulumi.Input[str]]],
+                 drop_dimensions: pulumi.Input[bool],
+                 output_name: pulumi.Input[str],
+                 type: pulumi.Input[str]):
+        """
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] dimensions: List of dimensions to either be kept or dropped in the new aggregated MTSs
+        :param pulumi.Input[bool] drop_dimensions: when true, the specified dimensions will be dropped from the aggregated MTSs
+        :param pulumi.Input[str] output_name: name of the new aggregated metric
+        :param pulumi.Input[str] type: Type of aggregator. Must always be "rollup"
+        """
+        pulumi.set(__self__, "dimensions", dimensions)
+        pulumi.set(__self__, "drop_dimensions", drop_dimensions)
+        pulumi.set(__self__, "output_name", output_name)
+        pulumi.set(__self__, "type", type)
+
+    @property
+    @pulumi.getter
+    def dimensions(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
+        """
+        List of dimensions to either be kept or dropped in the new aggregated MTSs
+        """
+        return pulumi.get(self, "dimensions")
+
+    @dimensions.setter
+    def dimensions(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(self, "dimensions", value)
+
+    @property
+    @pulumi.getter(name="dropDimensions")
+    def drop_dimensions(self) -> pulumi.Input[bool]:
+        """
+        when true, the specified dimensions will be dropped from the aggregated MTSs
+        """
+        return pulumi.get(self, "drop_dimensions")
+
+    @drop_dimensions.setter
+    def drop_dimensions(self, value: pulumi.Input[bool]):
+        pulumi.set(self, "drop_dimensions", value)
+
+    @property
+    @pulumi.getter(name="outputName")
+    def output_name(self) -> pulumi.Input[str]:
+        """
+        name of the new aggregated metric
+        """
+        return pulumi.get(self, "output_name")
+
+    @output_name.setter
+    def output_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "output_name", value)
+
+    @property
+    @pulumi.getter
+    def type(self) -> pulumi.Input[str]:
+        """
+        Type of aggregator. Must always be "rollup"
+        """
+        return pulumi.get(self, "type")
+
+    @type.setter
+    def type(self, value: pulumi.Input[str]):
+        pulumi.set(self, "type", value)
+
+
+@pulumi.input_type
+class MetricRulesetAggregationRuleMatcherArgs:
+    def __init__(__self__, *,
+                 type: pulumi.Input[str],
+                 filters: Optional[pulumi.Input[Sequence[pulumi.Input['MetricRulesetAggregationRuleMatcherFilterArgs']]]] = None):
+        """
+        :param pulumi.Input[str] type: Type of aggregator. Must always be "rollup"
+        :param pulumi.Input[Sequence[pulumi.Input['MetricRulesetAggregationRuleMatcherFilterArgs']]] filters: List of filters to filter the set of input MTSs
+        """
+        pulumi.set(__self__, "type", type)
+        if filters is not None:
+            pulumi.set(__self__, "filters", filters)
+
+    @property
+    @pulumi.getter
+    def type(self) -> pulumi.Input[str]:
+        """
+        Type of aggregator. Must always be "rollup"
+        """
+        return pulumi.get(self, "type")
+
+    @type.setter
+    def type(self, value: pulumi.Input[str]):
+        pulumi.set(self, "type", value)
+
+    @property
+    @pulumi.getter
+    def filters(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['MetricRulesetAggregationRuleMatcherFilterArgs']]]]:
+        """
+        List of filters to filter the set of input MTSs
+        """
+        return pulumi.get(self, "filters")
+
+    @filters.setter
+    def filters(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['MetricRulesetAggregationRuleMatcherFilterArgs']]]]):
+        pulumi.set(self, "filters", value)
+
+
+@pulumi.input_type
+class MetricRulesetAggregationRuleMatcherFilterArgs:
+    def __init__(__self__, *,
+                 not_: pulumi.Input[bool],
+                 property: pulumi.Input[str],
+                 property_values: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        """
+        :param pulumi.Input[bool] not_: When true, this filter will match all values not matching the property_values
+        :param pulumi.Input[str] property: Name of the dimension
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] property_values: Value of the dimension
+        """
+        pulumi.set(__self__, "not_", not_)
+        pulumi.set(__self__, "property", property)
+        pulumi.set(__self__, "property_values", property_values)
+
+    @property
+    @pulumi.getter(name="not")
+    def not_(self) -> pulumi.Input[bool]:
+        """
+        When true, this filter will match all values not matching the property_values
+        """
+        return pulumi.get(self, "not_")
+
+    @not_.setter
+    def not_(self, value: pulumi.Input[bool]):
+        pulumi.set(self, "not_", value)
+
+    @property
+    @pulumi.getter(name="propertyValues")
+    def property_values(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
+        """
+        Value of the dimension
+        """
+        return pulumi.get(self, "property_values")
+
+    @property_values.setter
+    def property_values(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(self, "property_values", value)
+
+    @property
+    @pulumi.getter
+    def property(self) -> pulumi.Input[str]:
+        """
+        Name of the dimension
+        """
+        return pulumi.get(self, "property")
+
+    @property.setter
+    def property(self, value: pulumi.Input[str]):
+        pulumi.set(self, "property", value)
+
+
+@pulumi.input_type
+class MetricRulesetRoutingRuleArgs:
+    def __init__(__self__, *,
+                 destination: pulumi.Input[str]):
+        """
+        :param pulumi.Input[str] destination: end destination of the input metric
+        """
+        pulumi.set(__self__, "destination", destination)
+
+    @property
+    @pulumi.getter
+    def destination(self) -> pulumi.Input[str]:
+        """
+        end destination of the input metric
+        """
+        return pulumi.get(self, "destination")
+
+    @destination.setter
+    def destination(self, value: pulumi.Input[str]):
+        pulumi.set(self, "destination", value)
+
+
+@pulumi.input_type
 class OrgTokenDpmLimitsArgs:
     def __init__(__self__, *,
                  dpm_limit: pulumi.Input[int],
                  dpm_notification_threshold: Optional[pulumi.Input[int]] = None):
         """
         :param pulumi.Input[int] dpm_limit: The datapoints per minute (dpm) limit for this token. If you exceed this limit, SignalFx sends out an alert.
         :param pulumi.Input[int] dpm_notification_threshold: DPM level at which SignalFx sends the notification for this token. If you don't specify a notification, SignalFx sends the generic notification.
```

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/_utilities.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/alert_muting_rule.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/alert_muting_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/aws/_inputs.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/aws/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/aws/external_integration.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/aws/external_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/aws/get_services.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/aws/get_services.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/aws/integration.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/aws/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/aws/outputs.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/aws/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/aws/token_integration.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/aws/token_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/azure/_inputs.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/azure/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/azure/get_services.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/azure/get_services.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/azure/integration.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/azure/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/azure/outputs.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/azure/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/config/vars.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/config/vars.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,13 +33,34 @@
     def custom_app_url(self) -> Optional[str]:
         """
         Application URL for your SignalFx org, often customized for organizations using SSO
         """
         return __config__.get('customAppUrl')
 
     @property
+    def retry_max_attempts(self) -> Optional[int]:
+        """
+        Max retries for a single HTTP call. Defaults to 4
+        """
+        return __config__.get_int('retryMaxAttempts')
+
+    @property
+    def retry_wait_max_seconds(self) -> Optional[int]:
+        """
+        Maximum retry wait for a single HTTP call in seconds. Defaults to 30
+        """
+        return __config__.get_int('retryWaitMaxSeconds')
+
+    @property
+    def retry_wait_min_seconds(self) -> Optional[int]:
+        """
+        Minimum retry wait for a single HTTP call in seconds. Defaults to 1
+        """
+        return __config__.get_int('retryWaitMinSeconds')
+
+    @property
     def timeout_seconds(self) -> Optional[int]:
         """
         Timeout duration for a single HTTP call in seconds. Defaults to 120
         """
         return __config__.get_int('timeoutSeconds')
```

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/dashboard.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/dashboard_group.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/dashboard_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/data_link.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/data_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/detector.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/detector.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/event_feed_chart.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/event_feed_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/gcp/_inputs.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/gcp/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/gcp/get_services.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/gcp/get_services.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/gcp/integration.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/gcp/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/gcp/outputs.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/gcp/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/get_aws_services.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/get_aws_services.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/get_azure_services.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/get_azure_services.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/get_dimension_values.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/get_dimension_values.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/heatmap_chart.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/heatmap_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/jira/integration.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/jira/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/list_chart.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/list_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/logs/_inputs.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/logs/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/logs/outputs.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/logs/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/logs/view.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/logs/view.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/opsgenie/integration.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/opsgenie/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/org_token.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/org_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/outputs.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,19 @@
     'DetectorRule',
     'DetectorVizOption',
     'HeatmapChartColorRange',
     'HeatmapChartColorScale',
     'ListChartColorScale',
     'ListChartLegendOptionsField',
     'ListChartVizOption',
+    'MetricRulesetAggregationRule',
+    'MetricRulesetAggregationRuleAggregator',
+    'MetricRulesetAggregationRuleMatcher',
+    'MetricRulesetAggregationRuleMatcherFilter',
+    'MetricRulesetRoutingRule',
     'OrgTokenDpmLimits',
     'OrgTokenHostOrUsageLimits',
     'SingleValueChartColorScale',
     'SingleValueChartVizOption',
     'TableChartVizOption',
     'TimeChartAxisLeft',
     'TimeChartAxisLeftWatermark',
@@ -1904,14 +1909,239 @@
         """
         A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gigibyte, Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
         """
         return pulumi.get(self, "value_unit")
 
 
 @pulumi.output_type
+class MetricRulesetAggregationRule(dict):
+    def __init__(__self__, *,
+                 aggregators: Sequence['outputs.MetricRulesetAggregationRuleAggregator'],
+                 enabled: bool,
+                 matchers: Sequence['outputs.MetricRulesetAggregationRuleMatcher'],
+                 name: Optional[str] = None):
+        """
+        :param Sequence['MetricRulesetAggregationRuleAggregatorArgs'] aggregators: Aggregator object
+        :param bool enabled: When false, this rule will not generate aggregated MTSs
+        :param Sequence['MetricRulesetAggregationRuleMatcherArgs'] matchers: Matcher object
+        """
+        pulumi.set(__self__, "aggregators", aggregators)
+        pulumi.set(__self__, "enabled", enabled)
+        pulumi.set(__self__, "matchers", matchers)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+
+    @property
+    @pulumi.getter
+    def aggregators(self) -> Sequence['outputs.MetricRulesetAggregationRuleAggregator']:
+        """
+        Aggregator object
+        """
+        return pulumi.get(self, "aggregators")
+
+    @property
+    @pulumi.getter
+    def enabled(self) -> bool:
+        """
+        When false, this rule will not generate aggregated MTSs
+        """
+        return pulumi.get(self, "enabled")
+
+    @property
+    @pulumi.getter
+    def matchers(self) -> Sequence['outputs.MetricRulesetAggregationRuleMatcher']:
+        """
+        Matcher object
+        """
+        return pulumi.get(self, "matchers")
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[str]:
+        return pulumi.get(self, "name")
+
+
+@pulumi.output_type
+class MetricRulesetAggregationRuleAggregator(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "dropDimensions":
+            suggest = "drop_dimensions"
+        elif key == "outputName":
+            suggest = "output_name"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in MetricRulesetAggregationRuleAggregator. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        MetricRulesetAggregationRuleAggregator.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        MetricRulesetAggregationRuleAggregator.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 dimensions: Sequence[str],
+                 drop_dimensions: bool,
+                 output_name: str,
+                 type: str):
+        """
+        :param Sequence[str] dimensions: List of dimensions to either be kept or dropped in the new aggregated MTSs
+        :param bool drop_dimensions: when true, the specified dimensions will be dropped from the aggregated MTSs
+        :param str output_name: name of the new aggregated metric
+        :param str type: Type of aggregator. Must always be "rollup"
+        """
+        pulumi.set(__self__, "dimensions", dimensions)
+        pulumi.set(__self__, "drop_dimensions", drop_dimensions)
+        pulumi.set(__self__, "output_name", output_name)
+        pulumi.set(__self__, "type", type)
+
+    @property
+    @pulumi.getter
+    def dimensions(self) -> Sequence[str]:
+        """
+        List of dimensions to either be kept or dropped in the new aggregated MTSs
+        """
+        return pulumi.get(self, "dimensions")
+
+    @property
+    @pulumi.getter(name="dropDimensions")
+    def drop_dimensions(self) -> bool:
+        """
+        when true, the specified dimensions will be dropped from the aggregated MTSs
+        """
+        return pulumi.get(self, "drop_dimensions")
+
+    @property
+    @pulumi.getter(name="outputName")
+    def output_name(self) -> str:
+        """
+        name of the new aggregated metric
+        """
+        return pulumi.get(self, "output_name")
+
+    @property
+    @pulumi.getter
+    def type(self) -> str:
+        """
+        Type of aggregator. Must always be "rollup"
+        """
+        return pulumi.get(self, "type")
+
+
+@pulumi.output_type
+class MetricRulesetAggregationRuleMatcher(dict):
+    def __init__(__self__, *,
+                 type: str,
+                 filters: Optional[Sequence['outputs.MetricRulesetAggregationRuleMatcherFilter']] = None):
+        """
+        :param str type: Type of aggregator. Must always be "rollup"
+        :param Sequence['MetricRulesetAggregationRuleMatcherFilterArgs'] filters: List of filters to filter the set of input MTSs
+        """
+        pulumi.set(__self__, "type", type)
+        if filters is not None:
+            pulumi.set(__self__, "filters", filters)
+
+    @property
+    @pulumi.getter
+    def type(self) -> str:
+        """
+        Type of aggregator. Must always be "rollup"
+        """
+        return pulumi.get(self, "type")
+
+    @property
+    @pulumi.getter
+    def filters(self) -> Optional[Sequence['outputs.MetricRulesetAggregationRuleMatcherFilter']]:
+        """
+        List of filters to filter the set of input MTSs
+        """
+        return pulumi.get(self, "filters")
+
+
+@pulumi.output_type
+class MetricRulesetAggregationRuleMatcherFilter(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "not":
+            suggest = "not_"
+        elif key == "propertyValues":
+            suggest = "property_values"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in MetricRulesetAggregationRuleMatcherFilter. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        MetricRulesetAggregationRuleMatcherFilter.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        MetricRulesetAggregationRuleMatcherFilter.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 not_: bool,
+                 property: str,
+                 property_values: Sequence[str]):
+        """
+        :param bool not_: When true, this filter will match all values not matching the property_values
+        :param str property: Name of the dimension
+        :param Sequence[str] property_values: Value of the dimension
+        """
+        pulumi.set(__self__, "not_", not_)
+        pulumi.set(__self__, "property", property)
+        pulumi.set(__self__, "property_values", property_values)
+
+    @property
+    @pulumi.getter(name="not")
+    def not_(self) -> bool:
+        """
+        When true, this filter will match all values not matching the property_values
+        """
+        return pulumi.get(self, "not_")
+
+    @property
+    @pulumi.getter(name="propertyValues")
+    def property_values(self) -> Sequence[str]:
+        """
+        Value of the dimension
+        """
+        return pulumi.get(self, "property_values")
+
+    @property
+    @pulumi.getter
+    def property(self) -> str:
+        """
+        Name of the dimension
+        """
+        return pulumi.get(self, "property")
+
+
+@pulumi.output_type
+class MetricRulesetRoutingRule(dict):
+    def __init__(__self__, *,
+                 destination: str):
+        """
+        :param str destination: end destination of the input metric
+        """
+        pulumi.set(__self__, "destination", destination)
+
+    @property
+    @pulumi.getter
+    def destination(self) -> str:
+        """
+        end destination of the input metric
+        """
+        return pulumi.get(self, "destination")
+
+
+@pulumi.output_type
 class OrgTokenDpmLimits(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "dpmLimit":
             suggest = "dpm_limit"
         elif key == "dpmNotificationThreshold":
```

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/pagerduty/get_integration.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/pagerduty/get_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/pagerduty/integration.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/pagerduty/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/servicenow/integration.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/servicenow/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/single_value_chart.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/single_value_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/slack/integration.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/slack/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/table_chart.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/table_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/team.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/text_chart.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/text_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/time_chart.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/time_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/victorops/integration.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/victorops/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx/webhook_integration.py` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/webhook_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx.egg-info/PKG-INFO` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-signalfx
-Version: 5.9.0a1678129624
+Version: 5.9.0a1678179334
 Summary: A Pulumi package for creating and managing SignalFx resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-signalfx
 Keywords: pulumi signalfx
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_signalfx-5.9.0a1678129624/pulumi_signalfx.egg-info/SOURCES.txt` & `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 pulumi_signalfx/detector.py
 pulumi_signalfx/event_feed_chart.py
 pulumi_signalfx/get_aws_services.py
 pulumi_signalfx/get_azure_services.py
 pulumi_signalfx/get_dimension_values.py
 pulumi_signalfx/heatmap_chart.py
 pulumi_signalfx/list_chart.py
+pulumi_signalfx/metric_ruleset.py
 pulumi_signalfx/org_token.py
 pulumi_signalfx/outputs.py
 pulumi_signalfx/provider.py
 pulumi_signalfx/pulumi-plugin.json
 pulumi_signalfx/py.typed
 pulumi_signalfx/single_value_chart.py
 pulumi_signalfx/table_chart.py
```

### Comparing `pulumi_signalfx-5.9.0a1678129624/setup.py` & `pulumi_signalfx-5.9.0a1678179334/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "5.9.0a1678129624"
-PLUGIN_VERSION = "5.9.0-alpha.1678129624+3b3b5684"
+VERSION = "5.9.0a1678179334"
+PLUGIN_VERSION = "5.9.0-alpha.1678179334+e6d600fc"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'signalfx', PLUGIN_VERSION])
         except OSError as error:
```

