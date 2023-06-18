# Comparing `tmp/pulumi_sumologic-0.9.0.tar.gz` & `tmp/pulumi_sumologic-0.9.1a1663799436.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_sumologic-0.9.0.tar", last modified: Wed Aug 17 17:25:23 2022, max compression
+gzip compressed data, was "pulumi_sumologic-0.9.1a1663799436.tar", last modified: Wed Sep 21 22:35:16 2022, max compression
```

## Comparing `pulumi_sumologic-0.9.0.tar` & `pulumi_sumologic-0.9.1a1663799436.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 17:25:23.472792 pulumi_sumologic-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     2922 2022-08-17 17:25:23.472792 pulumi_sumologic-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2578 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 17:25:23.472792 pulumi_sumologic-0.9.0/pulumi_sumologic/
--rw-r--r--   0 runner    (1001) docker     (121)    13721 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   622490 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     8081 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)    44626 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/aws_inventory_source.py
--rw-r--r--   0 runner    (1001) docker     (121)    44194 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/aws_xray_source.py
--rw-r--r--   0 runner    (1001) docker     (121)    33618 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/cloud_syslog_source.py
--rw-r--r--   0 runner    (1001) docker     (121)    13427 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/cloud_to_cloud_source.py
--rw-r--r--   0 runner    (1001) docker     (121)    46759 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/cloudfront_source.py
--rw-r--r--   0 runner    (1001) docker     (121)    46747 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/cloudtrail_source.py
--rw-r--r--   0 runner    (1001) docker     (121)    44977 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/cloudwatch_source.py
--rw-r--r--   0 runner    (1001) docker     (121)    16416 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/collector.py
--rw-r--r--   0 runner    (1001) docker     (121)     7571 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/collector_ingest_budget_assignment.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 17:25:23.472792 pulumi_sumologic-0.9.0/pulumi_sumologic/config/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (121)    25423 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/connection.py
--rw-r--r--   0 runner    (1001) docker     (121)    14632 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/content.py
--rw-r--r--   0 runner    (1001) docker     (121)    20370 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/content_permission.py
--rw-r--r--   0 runner    (1001) docker     (121)    42403 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/cse_aggregation_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)    33743 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/cse_chain_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)    11062 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/cse_custom_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    22865 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/cse_custom_insight.py
--rw-r--r--   0 runner    (1001) docker     (121)     9816 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/cse_entity_criticality_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    24501 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/cse_entity_entity_group_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     9092 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/cse_insights_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)    10963 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/cse_insights_resolution.py
--rw-r--r--   0 runner    (1001) docker     (121)     9195 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/cse_insights_status.py
--rw-r--r--   0 runner    (1001) docker     (121)    20928 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/cse_inventory_entity_group_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)    31168 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/cse_log_mapping.py
--rw-r--r--   0 runner    (1001) docker     (121)    19408 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/cse_match_list.py
--rw-r--r--   0 runner    (1001) docker     (121)    27798 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/cse_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)    12214 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/cse_network_block.py
--rw-r--r--   0 runner    (1001) docker     (121)    19471 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/cse_rule_tuning_expression.py
--rw-r--r--   0 runner    (1001) docker     (121)    35930 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/cse_threshold_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)    73692 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (121)    46123 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/elb_source.py
--rw-r--r--   0 runner    (1001) docker     (121)    11275 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/field.py
--rw-r--r--   0 runner    (1001) docker     (121)    14961 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/field_extraction_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)    11615 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/folder.py
--rw-r--r--   0 runner    (1001) docker     (121)    43776 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/gcp_metrics_source.py
--rw-r--r--   0 runner    (1001) docker     (121)    38497 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/gcp_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     4221 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/get_admin_recommended_folder.py
--rw-r--r--   0 runner    (1001) docker     (121)     2826 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/get_caller_identity.py
--rw-r--r--   0 runner    (1001) docker     (121)     5903 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/get_collector.py
--rw-r--r--   0 runner    (1001) docker     (121)     4983 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/get_cse_log_mapping_vendor_product.py
--rw-r--r--   0 runner    (1001) docker     (121)     4163 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/get_folder.py
--rw-r--r--   0 runner    (1001) docker     (121)     6803 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/get_http_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     1969 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/get_my_user_id.py
--rw-r--r--   0 runner    (1001) docker     (121)     3908 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/get_personal_folder.py
--rw-r--r--   0 runner    (1001) docker     (121)     5424 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/get_role.py
--rw-r--r--   0 runner    (1001) docker     (121)     5686 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/get_user.py
--rw-r--r--   0 runner    (1001) docker     (121)    11488 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (121)    40968 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/http_source.py
--rw-r--r--   0 runner    (1001) docker     (121)    20867 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/ingest_budget.py
--rw-r--r--   0 runner    (1001) docker     (121)    24169 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/ingest_budget_v2.py
--rw-r--r--   0 runner    (1001) docker     (121)    27766 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/installed_collector.py
--rw-r--r--   0 runner    (1001) docker     (121)    44871 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/kineis_log_source.py
--rw-r--r--   0 runner    (1001) docker     (121)    40601 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/kinesis_metrics_source.py
--rw-r--r--   0 runner    (1001) docker     (121)    20878 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/lookup_table.py
--rw-r--r--   0 runner    (1001) docker     (121)    45161 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/metadata_source.py
--rw-r--r--   0 runner    (1001) docker     (121)    89296 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)    34696 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/monitor_folder.py
--rw-r--r--   0 runner    (1001) docker     (121)   612741 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    27360 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/partition.py
--rw-r--r--   0 runner    (1001) docker     (121)    40432 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/password_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)    27264 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/policies.py
--rw-r--r--   0 runner    (1001) docker     (121)    44587 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/polling_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     7706 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    13962 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/role.py
--rw-r--r--   0 runner    (1001) docker     (121)    46193 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/s3_audit_source.py
--rw-r--r--   0 runner    (1001) docker     (121)    45733 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/s3_source.py
--rw-r--r--   0 runner    (1001) docker     (121)    53730 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/saml_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)    25428 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/scheduled_view.py
--rw-r--r--   0 runner    (1001) docker     (121)    35819 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/slo.py
--rw-r--r--   0 runner    (1001) docker     (121)    27195 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/slo_folder.py
--rw-r--r--   0 runner    (1001) docker     (121)     6449 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/subdomain.py
--rw-r--r--   0 runner    (1001) docker     (121)    14972 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/token.py
--rw-r--r--   0 runner    (1001) docker     (121)    17851 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic/user.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 17:25:23.472792 pulumi_sumologic-0.9.0/pulumi_sumologic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2922 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3096 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/pulumi_sumologic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-17 17:25:23.472792 pulumi_sumologic-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2114 2022-08-17 17:25:23.000000 pulumi_sumologic-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:35:16.507894 pulumi_sumologic-0.9.1a1663799436/
+-rw-r--r--   0 runner    (1001) docker     (121)     2933 2022-09-21 22:35:16.503894 pulumi_sumologic-0.9.1a1663799436/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2578 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:35:16.503894 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/
+-rw-r--r--   0 runner    (1001) docker     (121)    13721 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)  1328682 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8081 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44626 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/aws_inventory_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44194 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/aws_xray_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33618 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cloud_syslog_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13427 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cloud_to_cloud_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46759 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cloudfront_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46747 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cloudtrail_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44977 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cloudwatch_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16416 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/collector.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7571 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/collector_ingest_budget_assignment.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:35:16.503894 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/config/
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25423 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/connection.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14632 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/content.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20370 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/content_permission.py
+-rw-r--r--   0 runner    (1001) docker     (121)    42403 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_aggregation_rule.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33743 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_chain_rule.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11062 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_custom_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22865 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_custom_insight.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9816 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_entity_criticality_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24501 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_entity_entity_group_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9092 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_insights_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10963 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_insights_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9195 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_insights_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20928 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_inventory_entity_group_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31168 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_log_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19408 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_match_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27798 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_match_rule.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12214 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_network_block.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19471 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_rule_tuning_expression.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35930 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_threshold_rule.py
+-rw-r--r--   0 runner    (1001) docker     (121)    73692 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46123 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/elb_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11275 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/field.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14961 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/field_extraction_rule.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11615 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/folder.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43776 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/gcp_metrics_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38497 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/gcp_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4221 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/get_admin_recommended_folder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2826 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/get_caller_identity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5903 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/get_collector.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4983 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/get_cse_log_mapping_vendor_product.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4163 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/get_folder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6803 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/get_http_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1969 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/get_my_user_id.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3908 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/get_personal_folder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5424 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5686 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11488 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40968 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/http_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20867 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/ingest_budget.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24169 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/ingest_budget_v2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27766 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/installed_collector.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44871 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/kineis_log_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40601 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/kinesis_metrics_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20878 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/lookup_table.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45161 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/metadata_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)    89296 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34696 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/monitor_folder.py
+-rw-r--r--   0 runner    (1001) docker     (121)  1351717 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27360 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/partition.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40432 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/password_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27264 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/policies.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44587 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/polling_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7706 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    13962 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/role.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46193 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/s3_audit_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45733 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/s3_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)    53730 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/saml_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25428 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/scheduled_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35819 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/slo.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27195 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/slo_folder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6449 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/subdomain.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14972 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/token.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17851 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/user.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:35:16.503894 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2933 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3096 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 22:35:16.507894 pulumi_sumologic-0.9.1a1663799436/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2151 2022-09-21 22:35:16.000000 pulumi_sumologic-0.9.1a1663799436/setup.py
```

### Comparing `pulumi_sumologic-0.9.0/PKG-INFO` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi_sumologic
-Version: 0.9.0
+Name: pulumi-sumologic
+Version: 0.9.1a1663799436
 Summary: A Pulumi package for creating and managing sumologic cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-sumologic
 Keywords: pulumi sumologic
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_sumologic-0.9.0/README.md` & `pulumi_sumologic-0.9.1a1663799436/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/__init__.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/_utilities.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/aws_inventory_source.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/aws_inventory_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/aws_xray_source.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/aws_xray_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/cloud_syslog_source.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cloud_syslog_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/cloud_to_cloud_source.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cloud_to_cloud_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/cloudfront_source.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cloudfront_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/cloudtrail_source.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cloudtrail_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/cloudwatch_source.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cloudwatch_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/collector.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/collector.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/collector_ingest_budget_assignment.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/collector_ingest_budget_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/config/vars.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/connection.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/content.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/content.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/content_permission.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/content_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/cse_aggregation_rule.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_aggregation_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/cse_chain_rule.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_chain_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/cse_custom_entity_type.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_custom_entity_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/cse_custom_insight.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_custom_insight.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/cse_entity_criticality_config.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_entity_criticality_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/cse_entity_entity_group_configuration.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_entity_entity_group_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/cse_insights_configuration.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_insights_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/cse_insights_resolution.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_insights_resolution.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/cse_insights_status.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_insights_status.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/cse_inventory_entity_group_configuration.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_inventory_entity_group_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/cse_log_mapping.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_log_mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/cse_match_list.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_match_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/cse_match_rule.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_match_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/cse_network_block.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_network_block.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/cse_rule_tuning_expression.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_rule_tuning_expression.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/cse_threshold_rule.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/cse_threshold_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/dashboard.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/elb_source.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/elb_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/field.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/field.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/field_extraction_rule.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/field_extraction_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/folder.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/folder.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/gcp_metrics_source.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/gcp_metrics_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/gcp_source.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/gcp_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/get_admin_recommended_folder.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/get_admin_recommended_folder.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/get_caller_identity.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/get_caller_identity.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/get_collector.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/get_collector.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/get_cse_log_mapping_vendor_product.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/get_cse_log_mapping_vendor_product.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/get_folder.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/get_folder.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/get_http_source.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/get_http_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/get_my_user_id.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/get_my_user_id.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/get_personal_folder.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/get_personal_folder.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/get_role.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/get_user.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/hierarchy.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/hierarchy.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/http_source.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/http_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/ingest_budget.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/ingest_budget.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/ingest_budget_v2.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/ingest_budget_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/installed_collector.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/installed_collector.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/kineis_log_source.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/kineis_log_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/kinesis_metrics_source.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/kinesis_metrics_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/lookup_table.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/lookup_table.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/metadata_source.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/metadata_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/monitor.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/monitor.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/monitor_folder.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/monitor_folder.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/partition.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/partition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/password_policy.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/password_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/policies.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/polling_source.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/polling_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/provider.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/role.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/s3_audit_source.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/s3_audit_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/s3_source.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/s3_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/saml_configuration.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/saml_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/scheduled_view.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/scheduled_view.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/slo.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/slo.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/slo_folder.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/slo_folder.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/subdomain.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/subdomain.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/token.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/token.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic/user.py` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic.egg-info/PKG-INFO` & `pulumi_sumologic-0.9.1a1663799436/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi-sumologic
-Version: 0.9.0
+Name: pulumi_sumologic
+Version: 0.9.1a1663799436
 Summary: A Pulumi package for creating and managing sumologic cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-sumologic
 Keywords: pulumi sumologic
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_sumologic-0.9.0/pulumi_sumologic.egg-info/SOURCES.txt` & `pulumi_sumologic-0.9.1a1663799436/pulumi_sumologic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_sumologic-0.9.0/setup.py` & `pulumi_sumologic-0.9.1a1663799436/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.9.0"
-PLUGIN_VERSION = "0.9.0"
+VERSION = "0.9.1a1663799436"
+PLUGIN_VERSION = "0.9.1-alpha.1663799436+d9ba766f"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'sumologic', PLUGIN_VERSION])
         except OSError as error:
```

