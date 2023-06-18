# Comparing `tmp/pulumi_pagerduty-3.9.0a1678231019.tar.gz` & `tmp/pulumi_pagerduty-3.9.0a1678824312.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_pagerduty-3.9.0a1678231019.tar", last modified: Tue Mar  7 23:22:49 2023, max compression
+gzip compressed data, was "pulumi_pagerduty-3.9.0a1678824312.tar", last modified: Tue Mar 14 20:10:10 2023, max compression
```

## Comparing `pulumi_pagerduty-3.9.0a1678231019.tar` & `pulumi_pagerduty-3.9.0a1678824312.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 23:22:49.866200 pulumi_pagerduty-3.9.0a1678231019/
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-03-07 23:22:49.866200 pulumi_pagerduty-3.9.0a1678231019/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 23:22:49.866200 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/
--rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   248614 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/addon.py
--rw-r--r--   0 runner    (1001) docker     (123)    29736 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/automation_actions_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/automation_actions_action_service_association.py
--rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/automation_actions_action_team_association.py
--rw-r--r--   0 runner    (1001) docker     (123)    21581 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/automation_actions_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/automation_actions_runner_team_association.py
--rw-r--r--   0 runner    (1001) docker     (123)    18940 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/business_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    13703 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/business_service_subscriber.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 23:22:49.866200 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/custom_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    11286 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/custom_field_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/custom_field_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/custom_field_schema_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    16332 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/custom_field_schema_field_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/escalation_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14752 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/event_orchestration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17341 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/event_orchestration_router.py
--rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/event_orchestration_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    17913 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/event_orchestration_unrouted.py
--rw-r--r--   0 runner    (1001) docker     (123)    21924 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/event_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    24053 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    31642 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/extension_service_now.py
--rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_automation_actions_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_automation_actions_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_business_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_custom_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_custom_field_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_escalation_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_event_orchestration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_event_orchestrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_extension_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_incident_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_ruleset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_service_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_user_contact_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_vendor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13737 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/incident_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    19447 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/incident_workflow_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/maintenance_window.py
--rw-r--r--   0 runner    (1001) docker     (123)   221220 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37707 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/response_play.py
--rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/ruleset.py
--rw-r--r--   0 runner    (1001) docker     (123)    24333 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/ruleset_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    23490 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    58415 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    10517 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/service_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)    27229 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/service_event_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    45313 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/service_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    25784 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/slack_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/tag_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/team.py
--rw-r--r--   0 runner    (1001) docker     (123)    12532 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/team_membership.py
--rw-r--r--   0 runner    (1001) docker     (123)    31254 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    20992 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/user_contact_method.py
--rw-r--r--   0 runner    (1001) docker     (123)    17613 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/user_notification_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    27122 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/webhook_subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 23:22:49.866200 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 23:22:49.866200 pulumi_pagerduty-3.9.0a1678231019/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-03-07 23:22:49.000000 pulumi_pagerduty-3.9.0a1678231019/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:10:10.953976 pulumi_pagerduty-3.9.0a1678824312/
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-03-14 20:10:10.953976 pulumi_pagerduty-3.9.0a1678824312/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:10:10.949976 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/
+-rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   249671 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/addon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29736 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/automation_actions_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/automation_actions_action_service_association.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/automation_actions_action_team_association.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21581 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/automation_actions_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/automation_actions_runner_team_association.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18940 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/business_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13703 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/business_service_subscriber.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:10:10.953976 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11286 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/custom_field_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/custom_field_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/custom_field_schema_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17574 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/custom_field_schema_field_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/escalation_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14752 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/event_orchestration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17341 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/event_orchestration_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16495 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/event_orchestration_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17913 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/event_orchestration_unrouted.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21924 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/event_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24053 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31642 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/extension_service_now.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_automation_actions_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_automation_actions_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_business_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_custom_field_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_escalation_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_event_orchestration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_event_orchestrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_extension_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_incident_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_ruleset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_service_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_user_contact_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_vendor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13573 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/incident_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19283 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/incident_workflow_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)   222908 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37707 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/response_play.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/ruleset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24333 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/ruleset_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23490 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58415 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10517 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/service_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27229 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/service_event_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45313 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/service_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25784 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/slack_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/tag_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12532 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/team_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31254 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20992 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/user_contact_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17613 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/user_notification_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27122 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/webhook_subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:10:10.953976 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 20:10:10.953976 pulumi_pagerduty-3.9.0a1678824312/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-03-14 20:10:10.000000 pulumi_pagerduty-3.9.0a1678824312/setup.py
```

### Comparing `pulumi_pagerduty-3.9.0a1678231019/PKG-INFO` & `pulumi_pagerduty-3.9.0a1678824312/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_pagerduty
-Version: 3.9.0a1678231019
+Version: 3.9.0a1678824312
 Summary: A Pulumi package for creating and managing pagerduty cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-pagerduty
 Keywords: pulumi pagerduty
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_pagerduty-3.9.0a1678231019/README.md` & `pulumi_pagerduty-3.9.0a1678824312/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/__init__.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/_inputs.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,27 +122,31 @@
 
 @pulumi.input_type
 class AutomationActionsActionActionDataReferenceArgs:
     def __init__(__self__, *,
                  invocation_command: Optional[pulumi.Input[str]] = None,
                  process_automation_job_arguments: Optional[pulumi.Input[str]] = None,
                  process_automation_job_id: Optional[pulumi.Input[str]] = None,
+                 process_automation_node_filter: Optional[pulumi.Input[str]] = None,
                  script: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] invocation_command: The command to execute the script with.
         :param pulumi.Input[str] process_automation_job_arguments: The arguments to pass to the Process Automation job execution.
         :param pulumi.Input[str] process_automation_job_id: The ID of the Process Automation job to execute.
+        :param pulumi.Input[str] process_automation_node_filter: The expression that filters on which nodes a Process Automation Job executes [Learn more](https://docs.rundeck.com/docs/manual/05-nodes.html#node-filtering).
         :param pulumi.Input[str] script: Body of the script to be executed on the Runner. Max length is 16777215 characters.
         """
         if invocation_command is not None:
             pulumi.set(__self__, "invocation_command", invocation_command)
         if process_automation_job_arguments is not None:
             pulumi.set(__self__, "process_automation_job_arguments", process_automation_job_arguments)
         if process_automation_job_id is not None:
             pulumi.set(__self__, "process_automation_job_id", process_automation_job_id)
+        if process_automation_node_filter is not None:
+            pulumi.set(__self__, "process_automation_node_filter", process_automation_node_filter)
         if script is not None:
             pulumi.set(__self__, "script", script)
 
     @property
     @pulumi.getter(name="invocationCommand")
     def invocation_command(self) -> Optional[pulumi.Input[str]]:
         """
@@ -175,14 +179,26 @@
         return pulumi.get(self, "process_automation_job_id")
 
     @process_automation_job_id.setter
     def process_automation_job_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "process_automation_job_id", value)
 
     @property
+    @pulumi.getter(name="processAutomationNodeFilter")
+    def process_automation_node_filter(self) -> Optional[pulumi.Input[str]]:
+        """
+        The expression that filters on which nodes a Process Automation Job executes [Learn more](https://docs.rundeck.com/docs/manual/05-nodes.html#node-filtering).
+        """
+        return pulumi.get(self, "process_automation_node_filter")
+
+    @process_automation_node_filter.setter
+    def process_automation_node_filter(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "process_automation_node_filter", value)
+
+    @property
     @pulumi.getter
     def script(self) -> Optional[pulumi.Input[str]]:
         """
         Body of the script to be executed on the Runner. Max length is 16777215 characters.
         """
         return pulumi.get(self, "script")
```

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/_utilities.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/addon.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/addon.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/automation_actions_action.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/automation_actions_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/automation_actions_action_service_association.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/automation_actions_action_service_association.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/automation_actions_action_team_association.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/automation_actions_action_team_association.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/automation_actions_runner.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/automation_actions_runner.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/automation_actions_runner_team_association.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/automation_actions_runner_team_association.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/business_service.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/business_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/business_service_subscriber.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/business_service_subscriber.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/config/vars.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/custom_field.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/custom_field.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/custom_field_option.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/custom_field_option.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/custom_field_schema.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/custom_field_schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/custom_field_schema_assignment.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/custom_field_schema_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/custom_field_schema_field_configuration.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/custom_field_schema_field_configuration.py`

 * *Files 7% similar despite different names*

```diff
@@ -230,14 +230,32 @@
                  schema: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         A [Custom Field Configuration](https://support.pagerduty.com/docs/custom-fields#associate-schemas-with-services) is a declaration of a specific Custom Field in a specific Custom Field Schema.
 
         > The Custom Fields feature is currently available in Early Access.
 
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_pagerduty as pagerduty
+
+        cs_impact = pagerduty.CustomField("csImpact", datatype="string")
+        my_schema = pagerduty.CustomFieldSchema("mySchema",
+            title="My Schema",
+            description="Fields used on incidents")
+        first_field_configuration = pagerduty.CustomFieldSchemaFieldConfiguration("firstFieldConfiguration",
+            schema=my_schema.id,
+            field=cs_impact.id,
+            required=True,
+            default_value="none",
+            default_value_datatype="string")
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] default_value: The default value for the field.
         :param pulumi.Input[str] default_value_datatype: The datatype of the default value.
         :param pulumi.Input[bool] default_value_multi_value: Whether or not the default value is multi-valued.
         :param pulumi.Input[str] field: The ID of the field.
         :param pulumi.Input[bool] required: True if the field is required
@@ -250,14 +268,32 @@
                  args: CustomFieldSchemaFieldConfigurationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         A [Custom Field Configuration](https://support.pagerduty.com/docs/custom-fields#associate-schemas-with-services) is a declaration of a specific Custom Field in a specific Custom Field Schema.
 
         > The Custom Fields feature is currently available in Early Access.
 
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_pagerduty as pagerduty
+
+        cs_impact = pagerduty.CustomField("csImpact", datatype="string")
+        my_schema = pagerduty.CustomFieldSchema("mySchema",
+            title="My Schema",
+            description="Fields used on incidents")
+        first_field_configuration = pagerduty.CustomFieldSchemaFieldConfiguration("firstFieldConfiguration",
+            schema=my_schema.id,
+            field=cs_impact.id,
+            required=True,
+            default_value="none",
+            default_value_datatype="string")
+        ```
+
         :param str resource_name: The name of the resource.
         :param CustomFieldSchemaFieldConfigurationArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(CustomFieldSchemaFieldConfigurationArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/escalation_policy.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/escalation_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/event_orchestration.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/event_orchestration.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/event_orchestration_router.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/event_orchestration_router.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/event_orchestration_service.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/event_orchestration_service.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,24 +14,28 @@
 __all__ = ['EventOrchestrationServiceArgs', 'EventOrchestrationService']
 
 @pulumi.input_type
 class EventOrchestrationServiceArgs:
     def __init__(__self__, *,
                  catch_all: pulumi.Input['EventOrchestrationServiceCatchAllArgs'],
                  service: pulumi.Input[str],
-                 sets: pulumi.Input[Sequence[pulumi.Input['EventOrchestrationServiceSetArgs']]]):
+                 sets: pulumi.Input[Sequence[pulumi.Input['EventOrchestrationServiceSetArgs']]],
+                 enable_event_orchestration_for_service: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a EventOrchestrationService resource.
         :param pulumi.Input['EventOrchestrationServiceCatchAllArgs'] catch_all: the `catch_all` actions will be applied if an Event reaches the end of any set without matching any rules in that set.
         :param pulumi.Input[str] service: ID of the Service to which this Service Orchestration belongs to.
         :param pulumi.Input[Sequence[pulumi.Input['EventOrchestrationServiceSetArgs']]] sets: A Service Orchestration must contain at least a "start" set, but can contain any number of additional sets that are routed to by other rules to form a directional graph.
+        :param pulumi.Input[bool] enable_event_orchestration_for_service: Opt-in/out for switching the Service to [Service Orchestrations](https://support.pagerduty.com/docs/event-orchestration#service-orchestrations).
         """
         pulumi.set(__self__, "catch_all", catch_all)
         pulumi.set(__self__, "service", service)
         pulumi.set(__self__, "sets", sets)
+        if enable_event_orchestration_for_service is not None:
+            pulumi.set(__self__, "enable_event_orchestration_for_service", enable_event_orchestration_for_service)
 
     @property
     @pulumi.getter(name="catchAll")
     def catch_all(self) -> pulumi.Input['EventOrchestrationServiceCatchAllArgs']:
         """
         the `catch_all` actions will be applied if an Event reaches the end of any set without matching any rules in that set.
         """
@@ -61,29 +65,45 @@
         """
         return pulumi.get(self, "sets")
 
     @sets.setter
     def sets(self, value: pulumi.Input[Sequence[pulumi.Input['EventOrchestrationServiceSetArgs']]]):
         pulumi.set(self, "sets", value)
 
+    @property
+    @pulumi.getter(name="enableEventOrchestrationForService")
+    def enable_event_orchestration_for_service(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Opt-in/out for switching the Service to [Service Orchestrations](https://support.pagerduty.com/docs/event-orchestration#service-orchestrations).
+        """
+        return pulumi.get(self, "enable_event_orchestration_for_service")
+
+    @enable_event_orchestration_for_service.setter
+    def enable_event_orchestration_for_service(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "enable_event_orchestration_for_service", value)
+
 
 @pulumi.input_type
 class _EventOrchestrationServiceState:
     def __init__(__self__, *,
                  catch_all: Optional[pulumi.Input['EventOrchestrationServiceCatchAllArgs']] = None,
+                 enable_event_orchestration_for_service: Optional[pulumi.Input[bool]] = None,
                  service: Optional[pulumi.Input[str]] = None,
                  sets: Optional[pulumi.Input[Sequence[pulumi.Input['EventOrchestrationServiceSetArgs']]]] = None):
         """
         Input properties used for looking up and filtering EventOrchestrationService resources.
         :param pulumi.Input['EventOrchestrationServiceCatchAllArgs'] catch_all: the `catch_all` actions will be applied if an Event reaches the end of any set without matching any rules in that set.
+        :param pulumi.Input[bool] enable_event_orchestration_for_service: Opt-in/out for switching the Service to [Service Orchestrations](https://support.pagerduty.com/docs/event-orchestration#service-orchestrations).
         :param pulumi.Input[str] service: ID of the Service to which this Service Orchestration belongs to.
         :param pulumi.Input[Sequence[pulumi.Input['EventOrchestrationServiceSetArgs']]] sets: A Service Orchestration must contain at least a "start" set, but can contain any number of additional sets that are routed to by other rules to form a directional graph.
         """
         if catch_all is not None:
             pulumi.set(__self__, "catch_all", catch_all)
+        if enable_event_orchestration_for_service is not None:
+            pulumi.set(__self__, "enable_event_orchestration_for_service", enable_event_orchestration_for_service)
         if service is not None:
             pulumi.set(__self__, "service", service)
         if sets is not None:
             pulumi.set(__self__, "sets", sets)
 
     @property
     @pulumi.getter(name="catchAll")
@@ -94,14 +114,26 @@
         return pulumi.get(self, "catch_all")
 
     @catch_all.setter
     def catch_all(self, value: Optional[pulumi.Input['EventOrchestrationServiceCatchAllArgs']]):
         pulumi.set(self, "catch_all", value)
 
     @property
+    @pulumi.getter(name="enableEventOrchestrationForService")
+    def enable_event_orchestration_for_service(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Opt-in/out for switching the Service to [Service Orchestrations](https://support.pagerduty.com/docs/event-orchestration#service-orchestrations).
+        """
+        return pulumi.get(self, "enable_event_orchestration_for_service")
+
+    @enable_event_orchestration_for_service.setter
+    def enable_event_orchestration_for_service(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "enable_event_orchestration_for_service", value)
+
+    @property
     @pulumi.getter
     def service(self) -> Optional[pulumi.Input[str]]:
         """
         ID of the Service to which this Service Orchestration belongs to.
         """
         return pulumi.get(self, "service")
 
@@ -124,14 +156,15 @@
 
 class EventOrchestrationService(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  catch_all: Optional[pulumi.Input[pulumi.InputType['EventOrchestrationServiceCatchAllArgs']]] = None,
+                 enable_event_orchestration_for_service: Optional[pulumi.Input[bool]] = None,
                  service: Optional[pulumi.Input[str]] = None,
                  sets: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['EventOrchestrationServiceSetArgs']]]]] = None,
                  __props__=None):
         """
         ## Import
 
         Service Orchestration can be imported using the `id` of the Service, e.g.
@@ -139,14 +172,15 @@
         ```sh
          $ pulumi import pagerduty:index/eventOrchestrationService:EventOrchestrationService service PFEODA7
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['EventOrchestrationServiceCatchAllArgs']] catch_all: the `catch_all` actions will be applied if an Event reaches the end of any set without matching any rules in that set.
+        :param pulumi.Input[bool] enable_event_orchestration_for_service: Opt-in/out for switching the Service to [Service Orchestrations](https://support.pagerduty.com/docs/event-orchestration#service-orchestrations).
         :param pulumi.Input[str] service: ID of the Service to which this Service Orchestration belongs to.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['EventOrchestrationServiceSetArgs']]]] sets: A Service Orchestration must contain at least a "start" set, but can contain any number of additional sets that are routed to by other rules to form a directional graph.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -173,28 +207,30 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  catch_all: Optional[pulumi.Input[pulumi.InputType['EventOrchestrationServiceCatchAllArgs']]] = None,
+                 enable_event_orchestration_for_service: Optional[pulumi.Input[bool]] = None,
                  service: Optional[pulumi.Input[str]] = None,
                  sets: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['EventOrchestrationServiceSetArgs']]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = EventOrchestrationServiceArgs.__new__(EventOrchestrationServiceArgs)
 
             if catch_all is None and not opts.urn:
                 raise TypeError("Missing required property 'catch_all'")
             __props__.__dict__["catch_all"] = catch_all
+            __props__.__dict__["enable_event_orchestration_for_service"] = enable_event_orchestration_for_service
             if service is None and not opts.urn:
                 raise TypeError("Missing required property 'service'")
             __props__.__dict__["service"] = service
             if sets is None and not opts.urn:
                 raise TypeError("Missing required property 'sets'")
             __props__.__dict__["sets"] = sets
         super(EventOrchestrationService, __self__).__init__(
@@ -204,45 +240,56 @@
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             catch_all: Optional[pulumi.Input[pulumi.InputType['EventOrchestrationServiceCatchAllArgs']]] = None,
+            enable_event_orchestration_for_service: Optional[pulumi.Input[bool]] = None,
             service: Optional[pulumi.Input[str]] = None,
             sets: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['EventOrchestrationServiceSetArgs']]]]] = None) -> 'EventOrchestrationService':
         """
         Get an existing EventOrchestrationService resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['EventOrchestrationServiceCatchAllArgs']] catch_all: the `catch_all` actions will be applied if an Event reaches the end of any set without matching any rules in that set.
+        :param pulumi.Input[bool] enable_event_orchestration_for_service: Opt-in/out for switching the Service to [Service Orchestrations](https://support.pagerduty.com/docs/event-orchestration#service-orchestrations).
         :param pulumi.Input[str] service: ID of the Service to which this Service Orchestration belongs to.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['EventOrchestrationServiceSetArgs']]]] sets: A Service Orchestration must contain at least a "start" set, but can contain any number of additional sets that are routed to by other rules to form a directional graph.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _EventOrchestrationServiceState.__new__(_EventOrchestrationServiceState)
 
         __props__.__dict__["catch_all"] = catch_all
+        __props__.__dict__["enable_event_orchestration_for_service"] = enable_event_orchestration_for_service
         __props__.__dict__["service"] = service
         __props__.__dict__["sets"] = sets
         return EventOrchestrationService(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="catchAll")
     def catch_all(self) -> pulumi.Output['outputs.EventOrchestrationServiceCatchAll']:
         """
         the `catch_all` actions will be applied if an Event reaches the end of any set without matching any rules in that set.
         """
         return pulumi.get(self, "catch_all")
 
     @property
+    @pulumi.getter(name="enableEventOrchestrationForService")
+    def enable_event_orchestration_for_service(self) -> pulumi.Output[Optional[bool]]:
+        """
+        Opt-in/out for switching the Service to [Service Orchestrations](https://support.pagerduty.com/docs/event-orchestration#service-orchestrations).
+        """
+        return pulumi.get(self, "enable_event_orchestration_for_service")
+
+    @property
     @pulumi.getter
     def service(self) -> pulumi.Output[str]:
         """
         ID of the Service to which this Service Orchestration belongs to.
         """
         return pulumi.get(self, "service")
```

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/event_orchestration_unrouted.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/event_orchestration_unrouted.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/event_rule.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/event_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/extension.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/extension.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/extension_service_now.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/extension_service_now.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_automation_actions_action.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_automation_actions_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_automation_actions_runner.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_automation_actions_runner.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_business_service.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_business_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_custom_field.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_custom_field.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_custom_field_schema.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_custom_field_schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_escalation_policy.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_escalation_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_event_orchestration.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_event_orchestration.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_event_orchestrations.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_event_orchestrations.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_extension_schema.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_extension_schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_incident_workflow.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_incident_workflow.py`

 * *Files 11% similar despite different names*

```diff
@@ -63,16 +63,14 @@
 
 
 def get_incident_workflow(name: Optional[str] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetIncidentWorkflowResult:
     """
     Use this data source to get information about a specific [Incident Workflow](https://support.pagerduty.com/docs/incident-workflows) so that you can create a trigger for it.
 
-    > The Incident Workflows feature is currently available in Early Access.
-
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_pagerduty as pagerduty
 
     my_workflow = pagerduty.get_incident_workflow(name="Some Workflow Name")
@@ -100,16 +98,14 @@
 
 @_utilities.lift_output_func(get_incident_workflow)
 def get_incident_workflow_output(name: Optional[pulumi.Input[str]] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetIncidentWorkflowResult]:
     """
     Use this data source to get information about a specific [Incident Workflow](https://support.pagerduty.com/docs/incident-workflows) so that you can create a trigger for it.
 
-    > The Incident Workflows feature is currently available in Early Access.
-
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_pagerduty as pagerduty
 
     my_workflow = pagerduty.get_incident_workflow(name="Some Workflow Name")
```

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_priority.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_priority.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_ruleset.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_ruleset.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_schedule.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_schedule.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_service.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_service_integration.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_service_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_tag.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_team.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_user.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_user_contact_method.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_user_contact_method.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_users.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/get_vendor.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/get_vendor.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/incident_workflow.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/incident_workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,16 +166,14 @@
                  name: Optional[pulumi.Input[str]] = None,
                  steps: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IncidentWorkflowStepArgs']]]]] = None,
                  team: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         An [Incident Workflow](https://support.pagerduty.com/docs/incident-workflows) is a series of steps which can be executed on an incident.
 
-        > The Incident Workflows feature is currently available in Early Access.
-
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_pagerduty as pagerduty
 
         my_first_workflow = pagerduty.IncidentWorkflow("myFirstWorkflow",
@@ -210,16 +208,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[IncidentWorkflowArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         An [Incident Workflow](https://support.pagerduty.com/docs/incident-workflows) is a series of steps which can be executed on an incident.
 
-        > The Incident Workflows feature is currently available in Early Access.
-
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_pagerduty as pagerduty
 
         my_first_workflow = pagerduty.IncidentWorkflow("myFirstWorkflow",
```

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/incident_workflow_trigger.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/incident_workflow_trigger.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,16 +194,14 @@
                  subscribed_to_all_services: Optional[pulumi.Input[bool]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  workflow: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         An [Incident Workflow Trigger](https://support.pagerduty.com/docs/incident-workflows#triggers) defines when and if an [Incident Workflow](https://support.pagerduty.com/docs/incident-workflows) will be triggered.
 
-        > The Incident Workflows feature is currently available in Early Access.
-
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_pagerduty as pagerduty
 
         my_first_workflow = pagerduty.IncidentWorkflow("myFirstWorkflow",
@@ -251,16 +249,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: IncidentWorkflowTriggerArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         An [Incident Workflow Trigger](https://support.pagerduty.com/docs/incident-workflows#triggers) defines when and if an [Incident Workflow](https://support.pagerduty.com/docs/incident-workflows) will be triggered.
 
-        > The Incident Workflows feature is currently available in Early Access.
-
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_pagerduty as pagerduty
 
         my_first_workflow = pagerduty.IncidentWorkflow("myFirstWorkflow",
```

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/maintenance_window.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/maintenance_window.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/outputs.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,14 +133,16 @@
         suggest = None
         if key == "invocationCommand":
             suggest = "invocation_command"
         elif key == "processAutomationJobArguments":
             suggest = "process_automation_job_arguments"
         elif key == "processAutomationJobId":
             suggest = "process_automation_job_id"
+        elif key == "processAutomationNodeFilter":
+            suggest = "process_automation_node_filter"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in AutomationActionsActionActionDataReference. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         AutomationActionsActionActionDataReference.__key_warning(key)
         return super().__getitem__(key)
@@ -149,27 +151,31 @@
         AutomationActionsActionActionDataReference.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  invocation_command: Optional[str] = None,
                  process_automation_job_arguments: Optional[str] = None,
                  process_automation_job_id: Optional[str] = None,
+                 process_automation_node_filter: Optional[str] = None,
                  script: Optional[str] = None):
         """
         :param str invocation_command: The command to execute the script with.
         :param str process_automation_job_arguments: The arguments to pass to the Process Automation job execution.
         :param str process_automation_job_id: The ID of the Process Automation job to execute.
+        :param str process_automation_node_filter: The expression that filters on which nodes a Process Automation Job executes [Learn more](https://docs.rundeck.com/docs/manual/05-nodes.html#node-filtering).
         :param str script: Body of the script to be executed on the Runner. Max length is 16777215 characters.
         """
         if invocation_command is not None:
             pulumi.set(__self__, "invocation_command", invocation_command)
         if process_automation_job_arguments is not None:
             pulumi.set(__self__, "process_automation_job_arguments", process_automation_job_arguments)
         if process_automation_job_id is not None:
             pulumi.set(__self__, "process_automation_job_id", process_automation_job_id)
+        if process_automation_node_filter is not None:
+            pulumi.set(__self__, "process_automation_node_filter", process_automation_node_filter)
         if script is not None:
             pulumi.set(__self__, "script", script)
 
     @property
     @pulumi.getter(name="invocationCommand")
     def invocation_command(self) -> Optional[str]:
         """
@@ -190,14 +196,22 @@
     def process_automation_job_id(self) -> Optional[str]:
         """
         The ID of the Process Automation job to execute.
         """
         return pulumi.get(self, "process_automation_job_id")
 
     @property
+    @pulumi.getter(name="processAutomationNodeFilter")
+    def process_automation_node_filter(self) -> Optional[str]:
+        """
+        The expression that filters on which nodes a Process Automation Job executes [Learn more](https://docs.rundeck.com/docs/manual/05-nodes.html#node-filtering).
+        """
+        return pulumi.get(self, "process_automation_node_filter")
+
+    @property
     @pulumi.getter
     def script(self) -> Optional[str]:
         """
         Body of the script to be executed on the Runner. Max length is 16777215 characters.
         """
         return pulumi.get(self, "script")
 
@@ -5210,24 +5224,27 @@
 
 @pulumi.output_type
 class GetAutomationActionsActionActionDataReferenceResult(dict):
     def __init__(__self__, *,
                  invocation_command: str,
                  process_automation_job_arguments: str,
                  process_automation_job_id: str,
+                 process_automation_node_filter: str,
                  script: str):
         """
         :param str invocation_command: (Optional) The command to execute the script with.
         :param str process_automation_job_arguments: (Optional) The arguments to pass to the Process Automation job execution.
         :param str process_automation_job_id: (Required for `process_automation` action_type) The ID of the Process Automation job to execute.
+        :param str process_automation_node_filter: (Optional) The expression that filters on which nodes a Process Automation Job executes [Learn more](https://docs.rundeck.com/docs/manual/05-nodes.html#node-filtering).
         :param str script: (Required for `script` action_type) Body of the script to be executed on the Runner. Max length is 16777215 characters.
         """
         pulumi.set(__self__, "invocation_command", invocation_command)
         pulumi.set(__self__, "process_automation_job_arguments", process_automation_job_arguments)
         pulumi.set(__self__, "process_automation_job_id", process_automation_job_id)
+        pulumi.set(__self__, "process_automation_node_filter", process_automation_node_filter)
         pulumi.set(__self__, "script", script)
 
     @property
     @pulumi.getter(name="invocationCommand")
     def invocation_command(self) -> str:
         """
         (Optional) The command to execute the script with.
@@ -5247,14 +5264,22 @@
     def process_automation_job_id(self) -> str:
         """
         (Required for `process_automation` action_type) The ID of the Process Automation job to execute.
         """
         return pulumi.get(self, "process_automation_job_id")
 
     @property
+    @pulumi.getter(name="processAutomationNodeFilter")
+    def process_automation_node_filter(self) -> str:
+        """
+        (Optional) The expression that filters on which nodes a Process Automation Job executes [Learn more](https://docs.rundeck.com/docs/manual/05-nodes.html#node-filtering).
+        """
+        return pulumi.get(self, "process_automation_node_filter")
+
+    @property
     @pulumi.getter
     def script(self) -> str:
         """
         (Required for `script` action_type) Body of the script to be executed on the Runner. Max length is 16777215 characters.
         """
         return pulumi.get(self, "script")
```

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/provider.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/response_play.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/response_play.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/ruleset.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/ruleset.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/ruleset_rule.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/ruleset_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/schedule.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/schedule.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/service.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/service.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/service_dependency.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/service_dependency.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/service_event_rule.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/service_event_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/service_integration.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/service_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/slack_connection.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/slack_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/tag.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/tag_assignment.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/tag_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/team.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/team_membership.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/team_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/user.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/user_contact_method.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/user_contact_method.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/user_notification_rule.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/user_notification_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty/webhook_subscription.py` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty/webhook_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty.egg-info/PKG-INFO` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-pagerduty
-Version: 3.9.0a1678231019
+Version: 3.9.0a1678824312
 Summary: A Pulumi package for creating and managing pagerduty cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-pagerduty
 Keywords: pulumi pagerduty
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_pagerduty-3.9.0a1678231019/pulumi_pagerduty.egg-info/SOURCES.txt` & `pulumi_pagerduty-3.9.0a1678824312/pulumi_pagerduty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-3.9.0a1678231019/setup.py` & `pulumi_pagerduty-3.9.0a1678824312/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.9.0a1678231019"
-PLUGIN_VERSION = "3.9.0-alpha.1678231019+93c08d80"
+VERSION = "3.9.0a1678824312"
+PLUGIN_VERSION = "3.9.0-alpha.1678824312+98ef1881"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'pagerduty', PLUGIN_VERSION])
         except OSError as error:
```

