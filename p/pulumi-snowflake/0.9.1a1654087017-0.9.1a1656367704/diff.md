# Comparing `tmp/pulumi_snowflake-0.9.1a1654087017.tar.gz` & `tmp/pulumi_snowflake-0.9.1a1656367704.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulumi_snowflake-0.9.1a1654087017.tar", last modified: Wed Jun  1 12:43:37 2022, max compression
+gzip compressed data, was "dist/pulumi_snowflake-0.9.1a1656367704.tar", last modified: Mon Jun 27 22:11:59 2022, max compression
```

## Comparing `pulumi_snowflake-0.9.1a1654087017.tar` & `pulumi_snowflake-0.9.1a1656367704.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/
--rw-r--r--   0 runner    (1001) docker     (121)     5543 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4513 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/
--rw-r--r--   0 runner    (1001) docker     (121)    13165 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27618 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     7667 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)    14436 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/account_grant.py
--rw-r--r--   0 runner    (1001) docker     (121)    31439 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/api_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/config/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5156 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (121)    23035 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/database.py
--rw-r--r--   0 runner    (1001) docker     (121)    18850 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/database_grant.py
--rw-r--r--   0 runner    (1001) docker     (121)    44403 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/external_function.py
--rw-r--r--   0 runner    (1001) docker     (121)    47010 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/external_oauth_integration.py
--rw-r--r--   0 runner    (1001) docker     (121)    37801 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/external_table.py
--rw-r--r--   0 runner    (1001) docker     (121)    29228 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/external_table_grant.py
--rw-r--r--   0 runner    (1001) docker     (121)    92493 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/file_format.py
--rw-r--r--   0 runner    (1001) docker     (121)    26362 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/file_format_grant.py
--rw-r--r--   0 runner    (1001) docker     (121)    30810 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/function.py
--rw-r--r--   0 runner    (1001) docker     (121)    35603 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/function_grant.py
--rw-r--r--   0 runner    (1001) docker     (121)     2995 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_current_account.py
--rw-r--r--   0 runner    (1001) docker     (121)     5694 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_database.py
--rw-r--r--   0 runner    (1001) docker     (121)     2201 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_databases.py
--rw-r--r--   0 runner    (1001) docker     (121)     4019 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_external_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3902 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_external_tables.py
--rw-r--r--   0 runner    (1001) docker     (121)     3785 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_file_formats.py
--rw-r--r--   0 runner    (1001) docker     (121)     3666 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3940 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_masking_policies.py
--rw-r--r--   0 runner    (1001) docker     (121)     4019 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_materialized_views.py
--rw-r--r--   0 runner    (1001) docker     (121)     3514 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_pipes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3704 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_procedures.py
--rw-r--r--   0 runner    (1001) docker     (121)     2447 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_resource_monitors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2837 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_role.py
--rw-r--r--   0 runner    (1001) docker     (121)     4041 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_row_access_policies.py
--rw-r--r--   0 runner    (1001) docker     (121)     3042 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_schemas.py
--rw-r--r--   0 runner    (1001) docker     (121)     3666 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_sequences.py
--rw-r--r--   0 runner    (1001) docker     (121)     3552 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_stages.py
--rw-r--r--   0 runner    (1001) docker     (121)     2537 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_storage_integrations.py
--rw-r--r--   0 runner    (1001) docker     (121)     3590 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_streams.py
--rw-r--r--   0 runner    (1001) docker     (121)     3764 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_system_generate_scim_access_token.py
--rw-r--r--   0 runner    (1001) docker     (121)     3600 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_system_get_aws_sns_iam_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     4054 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_system_get_private_link_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2992 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_system_get_snowflake_platform_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     3552 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_tables.py
--rw-r--r--   0 runner    (1001) docker     (121)     3514 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     2954 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_users.py
--rw-r--r--   0 runner    (1001) docker     (121)     3514 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_views.py
--rw-r--r--   0 runner    (1001) docker     (121)     2233 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_warehouses.py
--rw-r--r--   0 runner    (1001) docker     (121)    16954 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/integration_grant.py
--rw-r--r--   0 runner    (1001) docker     (121)    19399 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/managed_account.py
--rw-r--r--   0 runner    (1001) docker     (121)    19480 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/masking_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)    20781 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/masking_policy_grant.py
--rw-r--r--   0 runner    (1001) docker     (121)    22629 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/materialized_view.py
--rw-r--r--   0 runner    (1001) docker     (121)    29573 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/materialized_view_grant.py
--rw-r--r--   0 runner    (1001) docker     (121)    14822 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/network_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)    16345 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/network_policy_attachment.py
--rw-r--r--   0 runner    (1001) docker     (121)    40801 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/notification_integration.py
--rw-r--r--   0 runner    (1001) docker     (121)    27378 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/oauth_integration.py
--rw-r--r--   0 runner    (1001) docker     (121)    44342 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    24592 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/pipe.py
--rw-r--r--   0 runner    (1001) docker     (121)    24680 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/pipe_grant.py
--rw-r--r--   0 runner    (1001) docker     (121)    27784 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/procedure.py
--rw-r--r--   0 runner    (1001) docker     (121)    35327 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/procedure_grant.py
--rw-r--r--   0 runner    (1001) docker     (121)    29244 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    29397 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/resource_monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)    16022 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/resource_monitor_grant.py
--rw-r--r--   0 runner    (1001) docker     (121)     8813 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/role.py
--rw-r--r--   0 runner    (1001) docker     (121)    14211 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/role_grants.py
--rw-r--r--   0 runner    (1001) docker     (121)    11315 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/role_ownership_grant.py
--rw-r--r--   0 runner    (1001) docker     (121)    20320 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/row_access_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)    22355 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/row_access_policy_grant.py
--rw-r--r--   0 runner    (1001) docker     (121)    66872 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/saml_integration.py
--rw-r--r--   0 runner    (1001) docker     (121)    22086 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)    25150 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/schema_grant.py
--rw-r--r--   0 runner    (1001) docker     (121)    17649 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/scim_integration.py
--rw-r--r--   0 runner    (1001) docker     (121)    16640 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/sequence.py
--rw-r--r--   0 runner    (1001) docker     (121)    26042 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/sequence_grant.py
--rw-r--r--   0 runner    (1001) docker     (121)    10175 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/share.py
--rw-r--r--   0 runner    (1001) docker     (121)    32752 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/stage.py
--rw-r--r--   0 runner    (1001) docker     (121)    24426 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/stage_grant.py
--rw-r--r--   0 runner    (1001) docker     (121)    31316 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/storage_integration.py
--rw-r--r--   0 runner    (1001) docker     (121)    20907 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/stream.py
--rw-r--r--   0 runner    (1001) docker     (121)    25806 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/stream_grant.py
--rw-r--r--   0 runner    (1001) docker     (121)    32621 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/table.py
--rw-r--r--   0 runner    (1001) docker     (121)    27961 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/table_grant.py
--rw-r--r--   0 runner    (1001) docker     (121)    11014 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/tag.py
--rw-r--r--   0 runner    (1001) docker     (121)    41211 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/task.py
--rw-r--r--   0 runner    (1001) docker     (121)    25580 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/task_grant.py
--rw-r--r--   0 runner    (1001) docker     (121)    42025 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/user.py
--rw-r--r--   0 runner    (1001) docker     (121)    11315 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/user_ownership_grant.py
--rw-r--r--   0 runner    (1001) docker     (121)    11413 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/user_public_keys.py
--rw-r--r--   0 runner    (1001) docker     (121)    20632 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/view.py
--rw-r--r--   0 runner    (1001) docker     (121)    28046 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/view_grant.py
--rw-r--r--   0 runner    (1001) docker     (121)    42938 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/warehouse.py
--rw-r--r--   0 runner    (1001) docker     (121)    16637 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/warehouse_grant.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5543 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3564 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2151 2022-06-01 12:43:37.000000 pulumi_snowflake-0.9.1a1654087017/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 22:11:59.000000 pulumi_snowflake-0.9.1a1656367704/
+-rw-r--r--   0 runner    (1001) docker     (121)     5543 2022-06-27 22:11:59.000000 pulumi_snowflake-0.9.1a1656367704/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4513 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 22:11:59.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/
+-rw-r--r--   0 runner    (1001) docker     (121)    13165 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27618 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7667 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14436 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/account_grant.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31439 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/api_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 22:11:59.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/config/
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5156 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23035 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/database.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18850 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/database_grant.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44403 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/external_function.py
+-rw-r--r--   0 runner    (1001) docker     (121)    47010 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/external_oauth_integration.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37801 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/external_table.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29228 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/external_table_grant.py
+-rw-r--r--   0 runner    (1001) docker     (121)    92493 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/file_format.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26362 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/file_format_grant.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30810 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/function.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35113 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/function_grant.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2995 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_current_account.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5694 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_database.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2201 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_databases.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4019 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_external_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3902 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_external_tables.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3785 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_file_formats.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3666 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3940 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_masking_policies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4019 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_materialized_views.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3514 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_pipes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3704 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_procedures.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2447 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_resource_monitors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2837 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4041 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_row_access_policies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3042 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3666 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_sequences.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3552 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_stages.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2537 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_storage_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3590 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_streams.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3764 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_system_generate_scim_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3600 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_system_get_aws_sns_iam_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4054 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_system_get_private_link_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2992 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_system_get_snowflake_platform_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3552 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_tables.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3514 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2954 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3514 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_views.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2233 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_warehouses.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16954 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/integration_grant.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19399 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/managed_account.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19480 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/masking_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20781 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/masking_policy_grant.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22629 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/materialized_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29573 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/materialized_view_grant.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14822 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/network_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16345 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/network_policy_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40801 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/notification_integration.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27378 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/oauth_integration.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44659 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24592 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24680 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/pipe_grant.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29735 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/procedure.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34837 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/procedure_grant.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29244 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    29397 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/resource_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16022 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/resource_monitor_grant.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8813 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/role.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14211 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/role_grants.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11315 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/role_ownership_grant.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20320 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/row_access_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22355 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/row_access_policy_grant.py
+-rw-r--r--   0 runner    (1001) docker     (121)    66872 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/saml_integration.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22086 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25150 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/schema_grant.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17649 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/scim_integration.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16640 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26042 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/sequence_grant.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10175 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/share.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32752 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/stage.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24426 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/stage_grant.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31316 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/storage_integration.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20907 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/stream.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25806 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/stream_grant.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32621 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/table.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27961 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/table_grant.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14298 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/tag.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41211 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/task.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25580 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/task_grant.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43750 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/user.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11315 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/user_ownership_grant.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11413 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/user_public_keys.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20632 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/view.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28046 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/view_grant.py
+-rw-r--r--   0 runner    (1001) docker     (121)    42938 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16637 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/warehouse_grant.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 22:11:59.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5543 2022-06-27 22:11:59.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3564 2022-06-27 22:11:59.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-27 22:11:59.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-27 22:11:59.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-27 22:11:59.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-27 22:11:59.000000 pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-27 22:11:59.000000 pulumi_snowflake-0.9.1a1656367704/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2151 2022-06-27 22:11:58.000000 pulumi_snowflake-0.9.1a1656367704/setup.py
```

### Comparing `pulumi_snowflake-0.9.1a1654087017/PKG-INFO` & `pulumi_snowflake-0.9.1a1656367704/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_snowflake
-Version: 0.9.1a1654087017
+Version: 0.9.1a1656367704
 Summary: A Pulumi package for creating and managing snowflake cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-snowflake
 Description: [![Actions Status](https://github.com/pulumi/pulumi-snowflake/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-snowflake/actions)
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
         [![NPM version](https://badge.fury.io/js/%40pulumi%2Fsnowflake.svg)](https://www.npmjs.com/package/@pulumi/snowflake)
```

### Comparing `pulumi_snowflake-0.9.1a1654087017/README.md` & `pulumi_snowflake-0.9.1a1656367704/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/__init__.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/_inputs.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/_utilities.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/account_grant.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/account_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/api_integration.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/api_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/config/vars.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/database.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/database.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/database_grant.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/database_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/external_function.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/external_function.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/external_oauth_integration.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/external_oauth_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/external_table.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/external_table.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/external_table_grant.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/external_table_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/file_format.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/file_format.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/file_format_grant.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/file_format_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/function.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/function.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/function_grant.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/function_grant.py`

 * *Files 2% similar despite different names*

```diff
@@ -411,35 +411,39 @@
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_snowflake as snowflake
 
         grant = snowflake.FunctionGrant("grant",
-            database_name="db",
-            schema_name="schema",
-            function_name="function",
             arguments=[
                 snowflake.FunctionGrantArgumentArgs(
-                    %!v(PANIC=Format method: interface conversion: model.Expression is *model.TemplateExpression, not *model.LiteralValueExpression),
-                    snowflake.FunctionGrantArgumentArgs(
-                        %!v(PANIC=Format method: interface conversion: model.Expression is *model.TemplateExpression, not *model.LiteralValueExpression),
-                    ],
-                    return_type="string",
-                    privilege="USAGE",
-                    roles=[
-                        "role1",
-                        "role2",
-                    ],
-                    shares=[
-                        "share1",
-                        "share2",
-                    ],
-                    on_future=False,
-                    with_grant_option=False)
+                    name="a",
+                    type="array",
+                ),
+                snowflake.FunctionGrantArgumentArgs(
+                    name="b",
+                    type="string",
+                ),
+            ],
+            database_name="db",
+            function_name="function",
+            on_future=False,
+            privilege="USAGE",
+            return_type="string",
+            roles=[
+                "role1",
+                "role2",
+            ],
+            schema_name="schema",
+            shares=[
+                "share1",
+                "share2",
+            ],
+            with_grant_option=False)
         ```
 
         ## Import
 
         # format is database name | schema name | function signature | privilege | true/false for with_grant_option
 
         ```sh
@@ -473,35 +477,39 @@
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_snowflake as snowflake
 
         grant = snowflake.FunctionGrant("grant",
-            database_name="db",
-            schema_name="schema",
-            function_name="function",
             arguments=[
                 snowflake.FunctionGrantArgumentArgs(
-                    %!v(PANIC=Format method: interface conversion: model.Expression is *model.TemplateExpression, not *model.LiteralValueExpression),
-                    snowflake.FunctionGrantArgumentArgs(
-                        %!v(PANIC=Format method: interface conversion: model.Expression is *model.TemplateExpression, not *model.LiteralValueExpression),
-                    ],
-                    return_type="string",
-                    privilege="USAGE",
-                    roles=[
-                        "role1",
-                        "role2",
-                    ],
-                    shares=[
-                        "share1",
-                        "share2",
-                    ],
-                    on_future=False,
-                    with_grant_option=False)
+                    name="a",
+                    type="array",
+                ),
+                snowflake.FunctionGrantArgumentArgs(
+                    name="b",
+                    type="string",
+                ),
+            ],
+            database_name="db",
+            function_name="function",
+            on_future=False,
+            privilege="USAGE",
+            return_type="string",
+            roles=[
+                "role1",
+                "role2",
+            ],
+            schema_name="schema",
+            shares=[
+                "share1",
+                "share2",
+            ],
+            with_grant_option=False)
         ```
 
         ## Import
 
         # format is database name | schema name | function signature | privilege | true/false for with_grant_option
 
         ```sh
```

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_current_account.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_current_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_database.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_databases.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_databases.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_external_functions.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_external_functions.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_external_tables.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_external_tables.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_file_formats.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_file_formats.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_functions.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_functions.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_masking_policies.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_masking_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_materialized_views.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_materialized_views.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_pipes.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_pipes.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_procedures.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_procedures.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_resource_monitors.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_resource_monitors.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_role.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_row_access_policies.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_row_access_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_schemas.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_schemas.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_sequences.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_sequences.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_stages.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_stages.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_storage_integrations.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_storage_integrations.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_streams.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_streams.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_system_generate_scim_access_token.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_system_generate_scim_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_system_get_aws_sns_iam_policy.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_system_get_aws_sns_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_system_get_private_link_config.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_system_get_private_link_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_system_get_snowflake_platform_info.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_system_get_snowflake_platform_info.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_tables.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_tables.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_tasks.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_tasks.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_users.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_views.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_views.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/get_warehouses.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/get_warehouses.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/integration_grant.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/integration_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/managed_account.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/managed_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/masking_policy.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/masking_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/masking_policy_grant.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/masking_policy_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/materialized_view.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/materialized_view.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/materialized_view_grant.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/materialized_view_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/network_policy.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/network_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/network_policy_attachment.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/network_policy_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/notification_integration.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/notification_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/oauth_integration.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/oauth_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/outputs.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1467,26 +1467,28 @@
 
 @pulumi.output_type
 class GetUsersUserResult(dict):
     def __init__(__self__, *,
                  comment: str,
                  default_namespace: str,
                  default_role: str,
+                 default_secondary_roles: Sequence[str],
                  default_warehouse: str,
                  disabled: bool,
                  display_name: str,
                  email: str,
                  first_name: str,
                  has_rsa_public_key: bool,
                  last_name: str,
                  login_name: str,
                  name: str):
         pulumi.set(__self__, "comment", comment)
         pulumi.set(__self__, "default_namespace", default_namespace)
         pulumi.set(__self__, "default_role", default_role)
+        pulumi.set(__self__, "default_secondary_roles", default_secondary_roles)
         pulumi.set(__self__, "default_warehouse", default_warehouse)
         pulumi.set(__self__, "disabled", disabled)
         pulumi.set(__self__, "display_name", display_name)
         pulumi.set(__self__, "email", email)
         pulumi.set(__self__, "first_name", first_name)
         pulumi.set(__self__, "has_rsa_public_key", has_rsa_public_key)
         pulumi.set(__self__, "last_name", last_name)
@@ -1505,14 +1507,19 @@
 
     @property
     @pulumi.getter(name="defaultRole")
     def default_role(self) -> str:
         return pulumi.get(self, "default_role")
 
     @property
+    @pulumi.getter(name="defaultSecondaryRoles")
+    def default_secondary_roles(self) -> Sequence[str]:
+        return pulumi.get(self, "default_secondary_roles")
+
+    @property
     @pulumi.getter(name="defaultWarehouse")
     def default_warehouse(self) -> str:
         return pulumi.get(self, "default_warehouse")
 
     @property
     @pulumi.getter
     def disabled(self) -> bool:
```

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/pipe.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/pipe.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/pipe_grant.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/pipe_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/procedure.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/procedure.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,26 +18,28 @@
                  database: pulumi.Input[str],
                  return_type: pulumi.Input[str],
                  schema: pulumi.Input[str],
                  statement: pulumi.Input[str],
                  arguments: Optional[pulumi.Input[Sequence[pulumi.Input['ProcedureArgumentArgs']]]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  execute_as: Optional[pulumi.Input[str]] = None,
+                 language: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  null_input_behavior: Optional[pulumi.Input[str]] = None,
                  return_behavior: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Procedure resource.
         :param pulumi.Input[str] database: The database in which to create the procedure. Don't use the | character.
         :param pulumi.Input[str] return_type: The return type of the procedure
         :param pulumi.Input[str] schema: The schema in which to create the procedure. Don't use the | character.
         :param pulumi.Input[str] statement: Specifies the javascript code used to create the procedure.
         :param pulumi.Input[Sequence[pulumi.Input['ProcedureArgumentArgs']]] arguments: List of the arguments for the procedure
         :param pulumi.Input[str] comment: Specifies a comment for the procedure.
         :param pulumi.Input[str] execute_as: Sets execute context - see caller's rights and owner's rights
+        :param pulumi.Input[str] language: Specifies the language of the stored procedure code.
         :param pulumi.Input[str] name: Specifies the identifier for the procedure; does not have to be unique for the schema in which the procedure is created.
                Don't use the | character.
         :param pulumi.Input[str] null_input_behavior: Specifies the behavior of the procedure when called with null inputs.
         :param pulumi.Input[str] return_behavior: Specifies the behavior of the function when returning results
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "return_type", return_type)
@@ -45,14 +47,16 @@
         pulumi.set(__self__, "statement", statement)
         if arguments is not None:
             pulumi.set(__self__, "arguments", arguments)
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
         if execute_as is not None:
             pulumi.set(__self__, "execute_as", execute_as)
+        if language is not None:
+            pulumi.set(__self__, "language", language)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if null_input_behavior is not None:
             pulumi.set(__self__, "null_input_behavior", null_input_behavior)
         if return_behavior is not None:
             pulumi.set(__self__, "return_behavior", return_behavior)
 
@@ -138,14 +142,26 @@
 
     @execute_as.setter
     def execute_as(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "execute_as", value)
 
     @property
     @pulumi.getter
+    def language(self) -> Optional[pulumi.Input[str]]:
+        """
+        Specifies the language of the stored procedure code.
+        """
+        return pulumi.get(self, "language")
+
+    @language.setter
+    def language(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "language", value)
+
+    @property
+    @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         Specifies the identifier for the procedure; does not have to be unique for the schema in which the procedure is created.
         Don't use the | character.
         """
         return pulumi.get(self, "name")
 
@@ -181,26 +197,28 @@
 @pulumi.input_type
 class _ProcedureState:
     def __init__(__self__, *,
                  arguments: Optional[pulumi.Input[Sequence[pulumi.Input['ProcedureArgumentArgs']]]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  database: Optional[pulumi.Input[str]] = None,
                  execute_as: Optional[pulumi.Input[str]] = None,
+                 language: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  null_input_behavior: Optional[pulumi.Input[str]] = None,
                  return_behavior: Optional[pulumi.Input[str]] = None,
                  return_type: Optional[pulumi.Input[str]] = None,
                  schema: Optional[pulumi.Input[str]] = None,
                  statement: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Procedure resources.
         :param pulumi.Input[Sequence[pulumi.Input['ProcedureArgumentArgs']]] arguments: List of the arguments for the procedure
         :param pulumi.Input[str] comment: Specifies a comment for the procedure.
         :param pulumi.Input[str] database: The database in which to create the procedure. Don't use the | character.
         :param pulumi.Input[str] execute_as: Sets execute context - see caller's rights and owner's rights
+        :param pulumi.Input[str] language: Specifies the language of the stored procedure code.
         :param pulumi.Input[str] name: Specifies the identifier for the procedure; does not have to be unique for the schema in which the procedure is created.
                Don't use the | character.
         :param pulumi.Input[str] null_input_behavior: Specifies the behavior of the procedure when called with null inputs.
         :param pulumi.Input[str] return_behavior: Specifies the behavior of the function when returning results
         :param pulumi.Input[str] return_type: The return type of the procedure
         :param pulumi.Input[str] schema: The schema in which to create the procedure. Don't use the | character.
         :param pulumi.Input[str] statement: Specifies the javascript code used to create the procedure.
@@ -209,14 +227,16 @@
             pulumi.set(__self__, "arguments", arguments)
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if execute_as is not None:
             pulumi.set(__self__, "execute_as", execute_as)
+        if language is not None:
+            pulumi.set(__self__, "language", language)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if null_input_behavior is not None:
             pulumi.set(__self__, "null_input_behavior", null_input_behavior)
         if return_behavior is not None:
             pulumi.set(__self__, "return_behavior", return_behavior)
         if return_type is not None:
@@ -272,14 +292,26 @@
 
     @execute_as.setter
     def execute_as(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "execute_as", value)
 
     @property
     @pulumi.getter
+    def language(self) -> Optional[pulumi.Input[str]]:
+        """
+        Specifies the language of the stored procedure code.
+        """
+        return pulumi.get(self, "language")
+
+    @language.setter
+    def language(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "language", value)
+
+    @property
+    @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         Specifies the identifier for the procedure; does not have to be unique for the schema in which the procedure is created.
         Don't use the | character.
         """
         return pulumi.get(self, "name")
 
@@ -353,14 +385,15 @@
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  arguments: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProcedureArgumentArgs']]]]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  database: Optional[pulumi.Input[str]] = None,
                  execute_as: Optional[pulumi.Input[str]] = None,
+                 language: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  null_input_behavior: Optional[pulumi.Input[str]] = None,
                  return_behavior: Optional[pulumi.Input[str]] = None,
                  return_type: Optional[pulumi.Input[str]] = None,
                  schema: Optional[pulumi.Input[str]] = None,
                  statement: Optional[pulumi.Input[str]] = None,
                  __props__=None):
@@ -374,14 +407,15 @@
         db = snowflake.Schema("db", data_retention_days=1)
         schema = snowflake.Schema("schema",
             database=snowflake_database["db"]["name"],
             data_retention_days=1)
         proc = snowflake.Procedure("proc",
             database=snowflake_database["db"]["name"],
             schema=schema.name,
+            language="JAVASCRIPT",
             arguments=[
                 snowflake.ProcedureArgumentArgs(
                     name="arg1",
                     type="varchar",
                 ),
                 snowflake.ProcedureArgumentArgs(
                     name="arg2",
@@ -408,14 +442,15 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProcedureArgumentArgs']]]] arguments: List of the arguments for the procedure
         :param pulumi.Input[str] comment: Specifies a comment for the procedure.
         :param pulumi.Input[str] database: The database in which to create the procedure. Don't use the | character.
         :param pulumi.Input[str] execute_as: Sets execute context - see caller's rights and owner's rights
+        :param pulumi.Input[str] language: Specifies the language of the stored procedure code.
         :param pulumi.Input[str] name: Specifies the identifier for the procedure; does not have to be unique for the schema in which the procedure is created.
                Don't use the | character.
         :param pulumi.Input[str] null_input_behavior: Specifies the behavior of the procedure when called with null inputs.
         :param pulumi.Input[str] return_behavior: Specifies the behavior of the function when returning results
         :param pulumi.Input[str] return_type: The return type of the procedure
         :param pulumi.Input[str] schema: The schema in which to create the procedure. Don't use the | character.
         :param pulumi.Input[str] statement: Specifies the javascript code used to create the procedure.
@@ -436,14 +471,15 @@
         db = snowflake.Schema("db", data_retention_days=1)
         schema = snowflake.Schema("schema",
             database=snowflake_database["db"]["name"],
             data_retention_days=1)
         proc = snowflake.Procedure("proc",
             database=snowflake_database["db"]["name"],
             schema=schema.name,
+            language="JAVASCRIPT",
             arguments=[
                 snowflake.ProcedureArgumentArgs(
                     name="arg1",
                     type="varchar",
                 ),
                 snowflake.ProcedureArgumentArgs(
                     name="arg2",
@@ -483,14 +519,15 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  arguments: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProcedureArgumentArgs']]]]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  database: Optional[pulumi.Input[str]] = None,
                  execute_as: Optional[pulumi.Input[str]] = None,
+                 language: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  null_input_behavior: Optional[pulumi.Input[str]] = None,
                  return_behavior: Optional[pulumi.Input[str]] = None,
                  return_type: Optional[pulumi.Input[str]] = None,
                  schema: Optional[pulumi.Input[str]] = None,
                  statement: Optional[pulumi.Input[str]] = None,
                  __props__=None):
@@ -507,14 +544,15 @@
 
             __props__.__dict__["arguments"] = arguments
             __props__.__dict__["comment"] = comment
             if database is None and not opts.urn:
                 raise TypeError("Missing required property 'database'")
             __props__.__dict__["database"] = database
             __props__.__dict__["execute_as"] = execute_as
+            __props__.__dict__["language"] = language
             __props__.__dict__["name"] = name
             __props__.__dict__["null_input_behavior"] = null_input_behavior
             __props__.__dict__["return_behavior"] = return_behavior
             if return_type is None and not opts.urn:
                 raise TypeError("Missing required property 'return_type'")
             __props__.__dict__["return_type"] = return_type
             if schema is None and not opts.urn:
@@ -533,14 +571,15 @@
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             arguments: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProcedureArgumentArgs']]]]] = None,
             comment: Optional[pulumi.Input[str]] = None,
             database: Optional[pulumi.Input[str]] = None,
             execute_as: Optional[pulumi.Input[str]] = None,
+            language: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
             null_input_behavior: Optional[pulumi.Input[str]] = None,
             return_behavior: Optional[pulumi.Input[str]] = None,
             return_type: Optional[pulumi.Input[str]] = None,
             schema: Optional[pulumi.Input[str]] = None,
             statement: Optional[pulumi.Input[str]] = None) -> 'Procedure':
         """
@@ -550,14 +589,15 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProcedureArgumentArgs']]]] arguments: List of the arguments for the procedure
         :param pulumi.Input[str] comment: Specifies a comment for the procedure.
         :param pulumi.Input[str] database: The database in which to create the procedure. Don't use the | character.
         :param pulumi.Input[str] execute_as: Sets execute context - see caller's rights and owner's rights
+        :param pulumi.Input[str] language: Specifies the language of the stored procedure code.
         :param pulumi.Input[str] name: Specifies the identifier for the procedure; does not have to be unique for the schema in which the procedure is created.
                Don't use the | character.
         :param pulumi.Input[str] null_input_behavior: Specifies the behavior of the procedure when called with null inputs.
         :param pulumi.Input[str] return_behavior: Specifies the behavior of the function when returning results
         :param pulumi.Input[str] return_type: The return type of the procedure
         :param pulumi.Input[str] schema: The schema in which to create the procedure. Don't use the | character.
         :param pulumi.Input[str] statement: Specifies the javascript code used to create the procedure.
@@ -566,14 +606,15 @@
 
         __props__ = _ProcedureState.__new__(_ProcedureState)
 
         __props__.__dict__["arguments"] = arguments
         __props__.__dict__["comment"] = comment
         __props__.__dict__["database"] = database
         __props__.__dict__["execute_as"] = execute_as
+        __props__.__dict__["language"] = language
         __props__.__dict__["name"] = name
         __props__.__dict__["null_input_behavior"] = null_input_behavior
         __props__.__dict__["return_behavior"] = return_behavior
         __props__.__dict__["return_type"] = return_type
         __props__.__dict__["schema"] = schema
         __props__.__dict__["statement"] = statement
         return Procedure(resource_name, opts=opts, __props__=__props__)
@@ -608,14 +649,22 @@
         """
         Sets execute context - see caller's rights and owner's rights
         """
         return pulumi.get(self, "execute_as")
 
     @property
     @pulumi.getter
+    def language(self) -> pulumi.Output[Optional[str]]:
+        """
+        Specifies the language of the stored procedure code.
+        """
+        return pulumi.get(self, "language")
+
+    @property
+    @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
         Specifies the identifier for the procedure; does not have to be unique for the schema in which the procedure is created.
         Don't use the | character.
         """
         return pulumi.get(self, "name")
```

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/procedure_grant.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/procedure_grant.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,35 +411,39 @@
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_snowflake as snowflake
 
         grant = snowflake.ProcedureGrant("grant",
-            database_name="db",
-            schema_name="schema",
-            procedure_name="procedure",
             arguments=[
                 snowflake.ProcedureGrantArgumentArgs(
-                    %!v(PANIC=Format method: interface conversion: model.Expression is *model.TemplateExpression, not *model.LiteralValueExpression),
-                    snowflake.ProcedureGrantArgumentArgs(
-                        %!v(PANIC=Format method: interface conversion: model.Expression is *model.TemplateExpression, not *model.LiteralValueExpression),
-                    ],
-                    return_type="string",
-                    privilege="select",
-                    roles=[
-                        "role1",
-                        "role2",
-                    ],
-                    shares=[
-                        "share1",
-                        "share2",
-                    ],
-                    on_future=False,
-                    with_grant_option=False)
+                    name="a",
+                    type="array",
+                ),
+                snowflake.ProcedureGrantArgumentArgs(
+                    name="b",
+                    type="string",
+                ),
+            ],
+            database_name="db",
+            on_future=False,
+            privilege="select",
+            procedure_name="procedure",
+            return_type="string",
+            roles=[
+                "role1",
+                "role2",
+            ],
+            schema_name="schema",
+            shares=[
+                "share1",
+                "share2",
+            ],
+            with_grant_option=False)
         ```
 
         ## Import
 
         # format is database name | schema name | procedure signature | privilege | true/false for with_grant_option
 
         ```sh
@@ -473,35 +477,39 @@
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_snowflake as snowflake
 
         grant = snowflake.ProcedureGrant("grant",
-            database_name="db",
-            schema_name="schema",
-            procedure_name="procedure",
             arguments=[
                 snowflake.ProcedureGrantArgumentArgs(
-                    %!v(PANIC=Format method: interface conversion: model.Expression is *model.TemplateExpression, not *model.LiteralValueExpression),
-                    snowflake.ProcedureGrantArgumentArgs(
-                        %!v(PANIC=Format method: interface conversion: model.Expression is *model.TemplateExpression, not *model.LiteralValueExpression),
-                    ],
-                    return_type="string",
-                    privilege="select",
-                    roles=[
-                        "role1",
-                        "role2",
-                    ],
-                    shares=[
-                        "share1",
-                        "share2",
-                    ],
-                    on_future=False,
-                    with_grant_option=False)
+                    name="a",
+                    type="array",
+                ),
+                snowflake.ProcedureGrantArgumentArgs(
+                    name="b",
+                    type="string",
+                ),
+            ],
+            database_name="db",
+            on_future=False,
+            privilege="select",
+            procedure_name="procedure",
+            return_type="string",
+            roles=[
+                "role1",
+                "role2",
+            ],
+            schema_name="schema",
+            shares=[
+                "share1",
+                "share2",
+            ],
+            with_grant_option=False)
         ```
 
         ## Import
 
         # format is database name | schema name | procedure signature | privilege | true/false for with_grant_option
 
         ```sh
```

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/provider.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/resource_monitor.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/resource_monitor.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/resource_monitor_grant.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/resource_monitor_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/role.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/role_grants.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/role_grants.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/role_ownership_grant.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/role_ownership_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/row_access_policy.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/row_access_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/row_access_policy_grant.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/row_access_policy_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/saml_integration.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/saml_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/schema.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/schema_grant.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/schema_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/scim_integration.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/scim_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/sequence.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/sequence.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/sequence_grant.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/sequence_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/share.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/share.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/stage.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/stage.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/stage_grant.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/stage_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/storage_integration.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/storage_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/stream.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/stream.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/stream_grant.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/stream_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/table.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/table.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/table_grant.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/table_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/tag.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/tag.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,25 +11,29 @@
 __all__ = ['TagArgs', 'Tag']
 
 @pulumi.input_type
 class TagArgs:
     def __init__(__self__, *,
                  database: pulumi.Input[str],
                  schema: pulumi.Input[str],
+                 allowed_values: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Tag resource.
         :param pulumi.Input[str] database: The database in which to create the tag.
         :param pulumi.Input[str] schema: The schema in which to create the tag.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_values: List of allowed values for the tag.
         :param pulumi.Input[str] comment: Specifies a comment for the tag.
         :param pulumi.Input[str] name: Specifies the identifier for the tag; must be unique for the database in which the tag is created.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "schema", schema)
+        if allowed_values is not None:
+            pulumi.set(__self__, "allowed_values", allowed_values)
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
@@ -52,14 +56,26 @@
         return pulumi.get(self, "schema")
 
     @schema.setter
     def schema(self, value: pulumi.Input[str]):
         pulumi.set(self, "schema", value)
 
     @property
+    @pulumi.getter(name="allowedValues")
+    def allowed_values(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        List of allowed values for the tag.
+        """
+        return pulumi.get(self, "allowed_values")
+
+    @allowed_values.setter
+    def allowed_values(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "allowed_values", value)
+
+    @property
     @pulumi.getter
     def comment(self) -> Optional[pulumi.Input[str]]:
         """
         Specifies a comment for the tag.
         """
         return pulumi.get(self, "comment")
 
@@ -79,35 +95,51 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
 
 @pulumi.input_type
 class _TagState:
     def __init__(__self__, *,
+                 allowed_values: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  database: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  schema: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Tag resources.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_values: List of allowed values for the tag.
         :param pulumi.Input[str] comment: Specifies a comment for the tag.
         :param pulumi.Input[str] database: The database in which to create the tag.
         :param pulumi.Input[str] name: Specifies the identifier for the tag; must be unique for the database in which the tag is created.
         :param pulumi.Input[str] schema: The schema in which to create the tag.
         """
+        if allowed_values is not None:
+            pulumi.set(__self__, "allowed_values", allowed_values)
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if schema is not None:
             pulumi.set(__self__, "schema", schema)
 
     @property
+    @pulumi.getter(name="allowedValues")
+    def allowed_values(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        List of allowed values for the tag.
+        """
+        return pulumi.get(self, "allowed_values")
+
+    @allowed_values.setter
+    def allowed_values(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "allowed_values", value)
+
+    @property
     @pulumi.getter
     def comment(self) -> Optional[pulumi.Input[str]]:
         """
         Specifies a comment for the tag.
         """
         return pulumi.get(self, "comment")
 
@@ -153,36 +185,84 @@
 
 
 class Tag(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 allowed_values: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  database: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  schema: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a Tag resource with the given unique name, props, and options.
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_snowflake as snowflake
+
+        test_tag = snowflake.Tag("testTag",
+            allowed_values=[
+                "foo",
+                "bar",
+            ],
+            comment="test comment",
+            database="test_db",
+            schema="test_schema")
+        ```
+
+        ## Import
+
+        # format is database name | schema name | tag name
+
+        ```sh
+         $ pulumi import snowflake:index/tag:Tag example 'dbName|schemaName|tagName'
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_values: List of allowed values for the tag.
         :param pulumi.Input[str] comment: Specifies a comment for the tag.
         :param pulumi.Input[str] database: The database in which to create the tag.
         :param pulumi.Input[str] name: Specifies the identifier for the tag; must be unique for the database in which the tag is created.
         :param pulumi.Input[str] schema: The schema in which to create the tag.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: TagArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a Tag resource with the given unique name, props, and options.
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_snowflake as snowflake
+
+        test_tag = snowflake.Tag("testTag",
+            allowed_values=[
+                "foo",
+                "bar",
+            ],
+            comment="test comment",
+            database="test_db",
+            schema="test_schema")
+        ```
+
+        ## Import
+
+        # format is database name | schema name | tag name
+
+        ```sh
+         $ pulumi import snowflake:index/tag:Tag example 'dbName|schemaName|tagName'
+        ```
+
         :param str resource_name: The name of the resource.
         :param TagArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(TagArgs, pulumi.ResourceOptions, *args, **kwargs)
@@ -190,14 +270,15 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 allowed_values: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  database: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  schema: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
@@ -206,14 +287,15 @@
         if opts.version is None:
             opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = TagArgs.__new__(TagArgs)
 
+            __props__.__dict__["allowed_values"] = allowed_values
             __props__.__dict__["comment"] = comment
             if database is None and not opts.urn:
                 raise TypeError("Missing required property 'database'")
             __props__.__dict__["database"] = database
             __props__.__dict__["name"] = name
             if schema is None and not opts.urn:
                 raise TypeError("Missing required property 'schema'")
@@ -224,41 +306,52 @@
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
+            allowed_values: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             comment: Optional[pulumi.Input[str]] = None,
             database: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
             schema: Optional[pulumi.Input[str]] = None) -> 'Tag':
         """
         Get an existing Tag resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_values: List of allowed values for the tag.
         :param pulumi.Input[str] comment: Specifies a comment for the tag.
         :param pulumi.Input[str] database: The database in which to create the tag.
         :param pulumi.Input[str] name: Specifies the identifier for the tag; must be unique for the database in which the tag is created.
         :param pulumi.Input[str] schema: The schema in which to create the tag.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _TagState.__new__(_TagState)
 
+        __props__.__dict__["allowed_values"] = allowed_values
         __props__.__dict__["comment"] = comment
         __props__.__dict__["database"] = database
         __props__.__dict__["name"] = name
         __props__.__dict__["schema"] = schema
         return Tag(resource_name, opts=opts, __props__=__props__)
 
     @property
+    @pulumi.getter(name="allowedValues")
+    def allowed_values(self) -> pulumi.Output[Optional[Sequence[str]]]:
+        """
+        List of allowed values for the tag.
+        """
+        return pulumi.get(self, "allowed_values")
+
+    @property
     @pulumi.getter
     def comment(self) -> pulumi.Output[Optional[str]]:
         """
         Specifies a comment for the tag.
         """
         return pulumi.get(self, "comment")
```

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/task.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/task.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/task_grant.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/task_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/user.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 @pulumi.input_type
 class UserArgs:
     def __init__(__self__, *,
                  comment: Optional[pulumi.Input[str]] = None,
                  default_namespace: Optional[pulumi.Input[str]] = None,
                  default_role: Optional[pulumi.Input[str]] = None,
+                 default_secondary_roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  default_warehouse: Optional[pulumi.Input[str]] = None,
                  disabled: Optional[pulumi.Input[bool]] = None,
                  display_name: Optional[pulumi.Input[str]] = None,
                  email: Optional[pulumi.Input[str]] = None,
                  first_name: Optional[pulumi.Input[str]] = None,
                  last_name: Optional[pulumi.Input[str]] = None,
                  login_name: Optional[pulumi.Input[str]] = None,
@@ -32,14 +33,15 @@
                  rsa_public_key2: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input['UserTagArgs']]]] = None):
         """
         The set of arguments for constructing a User resource.
         :param pulumi.Input[str] default_namespace: Specifies the namespace (database only or database and schema) that is active by default for the user’s session upon
                login.
         :param pulumi.Input[str] default_role: Specifies the role that is active by default for the user’s session upon login.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] default_secondary_roles: Specifies the set of secondary roles that are active for the user’s session upon login.
         :param pulumi.Input[str] default_warehouse: Specifies the virtual warehouse that is active by default for the user’s session upon login.
         :param pulumi.Input[str] display_name: Name displayed for the user in the Snowflake web interface.
         :param pulumi.Input[str] email: Email address for the user.
         :param pulumi.Input[str] first_name: First name of the user.
         :param pulumi.Input[str] last_name: Last name of the user.
         :param pulumi.Input[str] login_name: The name users use to log in. If not supplied, snowflake will use name instead.
         :param pulumi.Input[bool] must_change_password: Specifies whether the user is forced to change their password on next login (including their first/initial login) into
@@ -54,14 +56,16 @@
         """
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
         if default_namespace is not None:
             pulumi.set(__self__, "default_namespace", default_namespace)
         if default_role is not None:
             pulumi.set(__self__, "default_role", default_role)
+        if default_secondary_roles is not None:
+            pulumi.set(__self__, "default_secondary_roles", default_secondary_roles)
         if default_warehouse is not None:
             pulumi.set(__self__, "default_warehouse", default_warehouse)
         if disabled is not None:
             pulumi.set(__self__, "disabled", disabled)
         if display_name is not None:
             pulumi.set(__self__, "display_name", display_name)
         if email is not None:
@@ -116,14 +120,26 @@
         return pulumi.get(self, "default_role")
 
     @default_role.setter
     def default_role(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_role", value)
 
     @property
+    @pulumi.getter(name="defaultSecondaryRoles")
+    def default_secondary_roles(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Specifies the set of secondary roles that are active for the user’s session upon login.
+        """
+        return pulumi.get(self, "default_secondary_roles")
+
+    @default_secondary_roles.setter
+    def default_secondary_roles(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "default_secondary_roles", value)
+
+    @property
     @pulumi.getter(name="defaultWarehouse")
     def default_warehouse(self) -> Optional[pulumi.Input[str]]:
         """
         Specifies the virtual warehouse that is active by default for the user’s session upon login.
         """
         return pulumi.get(self, "default_warehouse")
 
@@ -278,14 +294,15 @@
 
 @pulumi.input_type
 class _UserState:
     def __init__(__self__, *,
                  comment: Optional[pulumi.Input[str]] = None,
                  default_namespace: Optional[pulumi.Input[str]] = None,
                  default_role: Optional[pulumi.Input[str]] = None,
+                 default_secondary_roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  default_warehouse: Optional[pulumi.Input[str]] = None,
                  disabled: Optional[pulumi.Input[bool]] = None,
                  display_name: Optional[pulumi.Input[str]] = None,
                  email: Optional[pulumi.Input[str]] = None,
                  first_name: Optional[pulumi.Input[str]] = None,
                  has_rsa_public_key: Optional[pulumi.Input[bool]] = None,
                  last_name: Optional[pulumi.Input[str]] = None,
@@ -297,14 +314,15 @@
                  rsa_public_key2: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input['UserTagArgs']]]] = None):
         """
         Input properties used for looking up and filtering User resources.
         :param pulumi.Input[str] default_namespace: Specifies the namespace (database only or database and schema) that is active by default for the user’s session upon
                login.
         :param pulumi.Input[str] default_role: Specifies the role that is active by default for the user’s session upon login.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] default_secondary_roles: Specifies the set of secondary roles that are active for the user’s session upon login.
         :param pulumi.Input[str] default_warehouse: Specifies the virtual warehouse that is active by default for the user’s session upon login.
         :param pulumi.Input[str] display_name: Name displayed for the user in the Snowflake web interface.
         :param pulumi.Input[str] email: Email address for the user.
         :param pulumi.Input[str] first_name: First name of the user.
         :param pulumi.Input[bool] has_rsa_public_key: Will be true if user as an RSA key set.
         :param pulumi.Input[str] last_name: Last name of the user.
         :param pulumi.Input[str] login_name: The name users use to log in. If not supplied, snowflake will use name instead.
@@ -320,14 +338,16 @@
         """
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
         if default_namespace is not None:
             pulumi.set(__self__, "default_namespace", default_namespace)
         if default_role is not None:
             pulumi.set(__self__, "default_role", default_role)
+        if default_secondary_roles is not None:
+            pulumi.set(__self__, "default_secondary_roles", default_secondary_roles)
         if default_warehouse is not None:
             pulumi.set(__self__, "default_warehouse", default_warehouse)
         if disabled is not None:
             pulumi.set(__self__, "disabled", disabled)
         if display_name is not None:
             pulumi.set(__self__, "display_name", display_name)
         if email is not None:
@@ -384,14 +404,26 @@
         return pulumi.get(self, "default_role")
 
     @default_role.setter
     def default_role(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_role", value)
 
     @property
+    @pulumi.getter(name="defaultSecondaryRoles")
+    def default_secondary_roles(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Specifies the set of secondary roles that are active for the user’s session upon login.
+        """
+        return pulumi.get(self, "default_secondary_roles")
+
+    @default_secondary_roles.setter
+    def default_secondary_roles(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "default_secondary_roles", value)
+
+    @property
     @pulumi.getter(name="defaultWarehouse")
     def default_warehouse(self) -> Optional[pulumi.Input[str]]:
         """
         Specifies the virtual warehouse that is active by default for the user’s session upon login.
         """
         return pulumi.get(self, "default_warehouse")
 
@@ -560,14 +592,15 @@
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  default_namespace: Optional[pulumi.Input[str]] = None,
                  default_role: Optional[pulumi.Input[str]] = None,
+                 default_secondary_roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  default_warehouse: Optional[pulumi.Input[str]] = None,
                  disabled: Optional[pulumi.Input[bool]] = None,
                  display_name: Optional[pulumi.Input[str]] = None,
                  email: Optional[pulumi.Input[str]] = None,
                  first_name: Optional[pulumi.Input[str]] = None,
                  last_name: Optional[pulumi.Input[str]] = None,
                  login_name: Optional[pulumi.Input[str]] = None,
@@ -575,47 +608,26 @@
                  name: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  rsa_public_key: Optional[pulumi.Input[str]] = None,
                  rsa_public_key2: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserTagArgs']]]]] = None,
                  __props__=None):
         """
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import pulumi_snowflake as snowflake
-
-        user = snowflake.User("user",
-            comment="A user of snowflake.",
-            default_role="role1",
-            default_warehouse="warehouse",
-            disabled=False,
-            display_name="Snowflake User",
-            email="user@snowflake.example",
-            first_name="Snowflake",
-            last_name="User",
-            login_name="snowflake_user",
-            must_change_password=False,
-            password="secret",
-            rsa_public_key="...",
-            rsa_public_key2="...")
-        ```
-
         ## Import
 
         ```sh
          $ pulumi import snowflake:index/user:User example userName
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] default_namespace: Specifies the namespace (database only or database and schema) that is active by default for the user’s session upon
                login.
         :param pulumi.Input[str] default_role: Specifies the role that is active by default for the user’s session upon login.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] default_secondary_roles: Specifies the set of secondary roles that are active for the user’s session upon login.
         :param pulumi.Input[str] default_warehouse: Specifies the virtual warehouse that is active by default for the user’s session upon login.
         :param pulumi.Input[str] display_name: Name displayed for the user in the Snowflake web interface.
         :param pulumi.Input[str] email: Email address for the user.
         :param pulumi.Input[str] first_name: First name of the user.
         :param pulumi.Input[str] last_name: Last name of the user.
         :param pulumi.Input[str] login_name: The name users use to log in. If not supplied, snowflake will use name instead.
         :param pulumi.Input[bool] must_change_password: Specifies whether the user is forced to change their password on next login (including their first/initial login) into
@@ -631,36 +643,14 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[UserArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import pulumi_snowflake as snowflake
-
-        user = snowflake.User("user",
-            comment="A user of snowflake.",
-            default_role="role1",
-            default_warehouse="warehouse",
-            disabled=False,
-            display_name="Snowflake User",
-            email="user@snowflake.example",
-            first_name="Snowflake",
-            last_name="User",
-            login_name="snowflake_user",
-            must_change_password=False,
-            password="secret",
-            rsa_public_key="...",
-            rsa_public_key2="...")
-        ```
-
         ## Import
 
         ```sh
          $ pulumi import snowflake:index/user:User example userName
         ```
 
         :param str resource_name: The name of the resource.
@@ -677,14 +667,15 @@
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  default_namespace: Optional[pulumi.Input[str]] = None,
                  default_role: Optional[pulumi.Input[str]] = None,
+                 default_secondary_roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  default_warehouse: Optional[pulumi.Input[str]] = None,
                  disabled: Optional[pulumi.Input[bool]] = None,
                  display_name: Optional[pulumi.Input[str]] = None,
                  email: Optional[pulumi.Input[str]] = None,
                  first_name: Optional[pulumi.Input[str]] = None,
                  last_name: Optional[pulumi.Input[str]] = None,
                  login_name: Optional[pulumi.Input[str]] = None,
@@ -705,14 +696,15 @@
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = UserArgs.__new__(UserArgs)
 
             __props__.__dict__["comment"] = comment
             __props__.__dict__["default_namespace"] = default_namespace
             __props__.__dict__["default_role"] = default_role
+            __props__.__dict__["default_secondary_roles"] = default_secondary_roles
             __props__.__dict__["default_warehouse"] = default_warehouse
             __props__.__dict__["disabled"] = disabled
             __props__.__dict__["display_name"] = display_name
             __props__.__dict__["email"] = email
             __props__.__dict__["first_name"] = first_name
             __props__.__dict__["last_name"] = last_name
             __props__.__dict__["login_name"] = login_name
@@ -732,14 +724,15 @@
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             comment: Optional[pulumi.Input[str]] = None,
             default_namespace: Optional[pulumi.Input[str]] = None,
             default_role: Optional[pulumi.Input[str]] = None,
+            default_secondary_roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             default_warehouse: Optional[pulumi.Input[str]] = None,
             disabled: Optional[pulumi.Input[bool]] = None,
             display_name: Optional[pulumi.Input[str]] = None,
             email: Optional[pulumi.Input[str]] = None,
             first_name: Optional[pulumi.Input[str]] = None,
             has_rsa_public_key: Optional[pulumi.Input[bool]] = None,
             last_name: Optional[pulumi.Input[str]] = None,
@@ -756,14 +749,15 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] default_namespace: Specifies the namespace (database only or database and schema) that is active by default for the user’s session upon
                login.
         :param pulumi.Input[str] default_role: Specifies the role that is active by default for the user’s session upon login.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] default_secondary_roles: Specifies the set of secondary roles that are active for the user’s session upon login.
         :param pulumi.Input[str] default_warehouse: Specifies the virtual warehouse that is active by default for the user’s session upon login.
         :param pulumi.Input[str] display_name: Name displayed for the user in the Snowflake web interface.
         :param pulumi.Input[str] email: Email address for the user.
         :param pulumi.Input[str] first_name: First name of the user.
         :param pulumi.Input[bool] has_rsa_public_key: Will be true if user as an RSA key set.
         :param pulumi.Input[str] last_name: Last name of the user.
         :param pulumi.Input[str] login_name: The name users use to log in. If not supplied, snowflake will use name instead.
@@ -780,14 +774,15 @@
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _UserState.__new__(_UserState)
 
         __props__.__dict__["comment"] = comment
         __props__.__dict__["default_namespace"] = default_namespace
         __props__.__dict__["default_role"] = default_role
+        __props__.__dict__["default_secondary_roles"] = default_secondary_roles
         __props__.__dict__["default_warehouse"] = default_warehouse
         __props__.__dict__["disabled"] = disabled
         __props__.__dict__["display_name"] = display_name
         __props__.__dict__["email"] = email
         __props__.__dict__["first_name"] = first_name
         __props__.__dict__["has_rsa_public_key"] = has_rsa_public_key
         __props__.__dict__["last_name"] = last_name
@@ -819,14 +814,22 @@
     def default_role(self) -> pulumi.Output[str]:
         """
         Specifies the role that is active by default for the user’s session upon login.
         """
         return pulumi.get(self, "default_role")
 
     @property
+    @pulumi.getter(name="defaultSecondaryRoles")
+    def default_secondary_roles(self) -> pulumi.Output[Optional[Sequence[str]]]:
+        """
+        Specifies the set of secondary roles that are active for the user’s session upon login.
+        """
+        return pulumi.get(self, "default_secondary_roles")
+
+    @property
     @pulumi.getter(name="defaultWarehouse")
     def default_warehouse(self) -> pulumi.Output[Optional[str]]:
         """
         Specifies the virtual warehouse that is active by default for the user’s session upon login.
         """
         return pulumi.get(self, "default_warehouse")
```

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/user_ownership_grant.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/user_ownership_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/user_public_keys.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/user_public_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/view.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/view.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/view_grant.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/view_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/warehouse.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/warehouse.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake/warehouse_grant.py` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake/warehouse_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake.egg-info/PKG-INFO` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-snowflake
-Version: 0.9.1a1654087017
+Version: 0.9.1a1656367704
 Summary: A Pulumi package for creating and managing snowflake cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-snowflake
 Description: [![Actions Status](https://github.com/pulumi/pulumi-snowflake/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-snowflake/actions)
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
         [![NPM version](https://badge.fury.io/js/%40pulumi%2Fsnowflake.svg)](https://www.npmjs.com/package/@pulumi/snowflake)
```

### Comparing `pulumi_snowflake-0.9.1a1654087017/pulumi_snowflake.egg-info/SOURCES.txt` & `pulumi_snowflake-0.9.1a1656367704/pulumi_snowflake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_snowflake-0.9.1a1654087017/setup.py` & `pulumi_snowflake-0.9.1a1656367704/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.9.1a1654087017"
-PLUGIN_VERSION = "0.9.1-alpha.1654087017+9ad5a5ba"
+VERSION = "0.9.1a1656367704"
+PLUGIN_VERSION = "0.9.1-alpha.1656367704+dcdc5621"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'snowflake', PLUGIN_VERSION])
         except OSError as error:
```

