# Comparing `tmp/lakefs-client-0.98.0.tar.gz` & `tmp/lakefs-client-0.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lakefs-client-0.98.0.tar", last modified: Wed Apr  5 11:29:14 2023, max compression
+gzip compressed data, was "lakefs-client-0.99.0.tar", last modified: Wed Apr 19 12:26:03 2023, max compression
```

## Comparing `lakefs-client-0.98.0.tar` & `lakefs-client-0.99.0.tar`

### file list

```diff
@@ -1,240 +1,240 @@
-drwxr-xr-x   0     1001      122        0 2023-04-05 11:29:14.235569 lakefs-client-0.98.0/
--rw-r--r--   0     1001      122    23958 2023-04-05 11:29:14.235569 lakefs-client-0.98.0/PKG-INFO
--rw-r--r--   0     1001      122    23621 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/README.md
-drwxr-xr-x   0     1001      122        0 2023-04-05 11:29:14.211570 lakefs-client-0.98.0/lakefs_client/
--rw-r--r--   0     1001      122      706 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/__init__.py
-drwxr-xr-x   0     1001      122        0 2023-04-05 11:29:14.211570 lakefs-client-0.98.0/lakefs_client/api/
--rw-r--r--   0     1001      122      217 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/api/__init__.py
--rw-r--r--   0     1001      122    20697 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/api/actions_api.py
--rw-r--r--   0     1001      122   149645 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/api/auth_api.py
--rw-r--r--   0     1001      122    39812 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/api/branches_api.py
--rw-r--r--   0     1001      122    15812 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/api/commits_api.py
--rw-r--r--   0     1001      122    24307 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/api/config_api.py
--rw-r--r--   0     1001      122    10159 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/api/experimental_api.py
--rw-r--r--   0     1001      122     4339 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/api/health_check_api.py
--rw-r--r--   0     1001      122    10487 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/api/import_api.py
--rw-r--r--   0     1001      122    14540 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/api/metadata_api.py
--rw-r--r--   0     1001      122    54238 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/api/objects_api.py
--rw-r--r--   0     1001      122    10154 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/api/otf_diff_api.py
--rw-r--r--   0     1001      122    32626 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/api/refs_api.py
--rw-r--r--   0     1001      122    32139 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/api/repositories_api.py
--rw-r--r--   0     1001      122    23822 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/api/retention_api.py
--rw-r--r--   0     1001      122    16709 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/api/staging_api.py
--rw-r--r--   0     1001      122     5165 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/api/statistics_api.py
--rw-r--r--   0     1001      122    19140 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/api/tags_api.py
--rw-r--r--   0     1001      122     5534 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/api/templates_api.py
--rw-r--r--   0     1001      122    36801 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/api_client.py
-drwxr-xr-x   0     1001      122        0 2023-04-05 11:29:14.211570 lakefs-client-0.98.0/lakefs_client/apis/
--rw-r--r--   0     1001      122     1393 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/apis/__init__.py
--rw-r--r--   0     1001      122     2784 2023-04-05 11:28:47.000000 lakefs-client-0.98.0/lakefs_client/client.py
--rw-r--r--   0     1001      122    18528 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/configuration.py
--rw-r--r--   0     1001      122     5035 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/exceptions.py
-drwxr-xr-x   0     1001      122        0 2023-04-05 11:29:14.223569 lakefs-client-0.98.0/lakefs_client/model/
--rw-r--r--   0     1001      122      348 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/model/__init__.py
--rw-r--r--   0     1001      122    11898 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/access_key_credentials.py
--rw-r--r--   0     1001      122    12186 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/acl.py
--rw-r--r--   0     1001      122    12568 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/action_run.py
--rw-r--r--   0     1001      122    11638 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/action_run_list.py
--rw-r--r--   0     1001      122    11286 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/auth_capabilities.py
--rw-r--r--   0     1001      122    11470 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/authentication_token.py
--rw-r--r--   0     1001      122    11260 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/branch_creation.py
--rw-r--r--   0     1001      122    11295 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/branch_protection_rule.py
--rw-r--r--   0     1001      122    11718 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/cherry_pick_creation.py
--rw-r--r--   0     1001      122    11848 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/comm_prefs_input.py
--rw-r--r--   0     1001      122    12549 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/commit.py
--rw-r--r--   0     1001      122    11635 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/commit_creation.py
--rw-r--r--   0     1001      122    11607 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/commit_list.py
--rw-r--r--   0     1001      122    11471 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/credentials.py
--rw-r--r--   0     1001      122    11657 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/credentials_list.py
--rw-r--r--   0     1001      122    11834 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/credentials_with_secret.py
--rw-r--r--   0     1001      122    11181 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/current_user.py
--rw-r--r--   0     1001      122    12102 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/diff.py
--rw-r--r--   0     1001      122    11587 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/diff_list.py
--rw-r--r--   0     1001      122    11048 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/diff_properties.py
--rw-r--r--   0     1001      122    11124 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/error.py
--rw-r--r--   0     1001      122    11412 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/error_no_acl.py
--rw-r--r--   0     1001      122    12082 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/find_merge_base_result.py
--rw-r--r--   0     1001      122    11080 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/forgot_password_request.py
--rw-r--r--   0     1001      122    11249 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/garbage_collection_config.py
--rw-r--r--   0     1001      122    11192 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/garbage_collection_prepare_request.py
--rw-r--r--   0     1001      122    12236 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/garbage_collection_prepare_response.py
--rw-r--r--   0     1001      122    11424 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/garbage_collection_rule.py
--rw-r--r--   0     1001      122    11773 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/garbage_collection_rules.py
--rw-r--r--   0     1001      122    11332 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/group.py
--rw-r--r--   0     1001      122    11023 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/group_creation.py
--rw-r--r--   0     1001      122    11597 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/group_list.py
--rw-r--r--   0     1001      122    12339 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/hook_run.py
--rw-r--r--   0     1001      122    11618 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/hook_run_list.py
--rw-r--r--   0     1001      122    12130 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/import_pagination.py
--rw-r--r--   0     1001      122    11627 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/ingest_range_creation_response.py
--rw-r--r--   0     1001      122    11078 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/inline_object1.py
--rw-r--r--   0     1001      122    13582 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/login_config.py
--rw-r--r--   0     1001      122    11486 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/login_information.py
--rw-r--r--   0     1001      122    11938 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/merge.py
--rw-r--r--   0     1001      122    11529 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/merge_result.py
--rw-r--r--   0     1001      122    11967 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/merge_result_summary.py
--rw-r--r--   0     1001      122    11353 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/meta_range_creation.py
--rw-r--r--   0     1001      122    11095 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/meta_range_creation_response.py
--rw-r--r--   0     1001      122    11154 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/next_step.py
--rw-r--r--   0     1001      122    11499 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/object_copy_creation.py
--rw-r--r--   0     1001      122    11721 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/object_error.py
--rw-r--r--   0     1001      122    11271 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/object_error_list.py
--rw-r--r--   0     1001      122    12610 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/object_stage_creation.py
--rw-r--r--   0     1001      122    13598 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/object_stats.py
--rw-r--r--   0     1001      122    11658 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/object_stats_list.py
--rw-r--r--   0     1001      122    10783 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/object_user_metadata.py
--rw-r--r--   0     1001      122    12651 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/otf_diff_entry.py
--rw-r--r--   0     1001      122    11620 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/otf_diff_list.py
--rw-r--r--   0     1001      122    11212 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/otf_diffs.py
--rw-r--r--   0     1001      122    12264 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/pagination.py
--rw-r--r--   0     1001      122    11047 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/path_list.py
--rw-r--r--   0     1001      122    11764 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/policy.py
--rw-r--r--   0     1001      122    11607 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/policy_list.py
--rw-r--r--   0     1001      122    11115 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/prepare_gc_uncommitted_request.py
--rw-r--r--   0     1001      122    11841 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/prepare_gc_uncommitted_response.py
--rw-r--r--   0     1001      122    12236 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/range_metadata.py
--rw-r--r--   0     1001      122    11238 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/ref.py
--rw-r--r--   0     1001      122    11577 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/ref_list.py
--rw-r--r--   0     1001      122    11949 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/refs_dump.py
--rw-r--r--   0     1001      122    12148 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/repository.py
--rw-r--r--   0     1001      122    12102 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/repository_creation.py
--rw-r--r--   0     1001      122    11647 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/repository_list.py
--rw-r--r--   0     1001      122    11363 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/reset_creation.py
--rw-r--r--   0     1001      122    11616 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/revert_creation.py
--rw-r--r--   0     1001      122    11580 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/setup.py
--rw-r--r--   0     1001      122    11584 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/lakefs_client/model/setup_state.py
--rw-r--r--   0     1001      122    12850 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/model/stage_range_creation.py
--rw-r--r--   0     1001      122    11870 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/model/staging_location.py
--rw-r--r--   0     1001      122    12443 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/model/staging_metadata.py
--rw-r--r--   0     1001      122    11661 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/model/statement.py
--rw-r--r--   0     1001      122    11918 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/model/stats_event.py
--rw-r--r--   0     1001      122    11264 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/model/stats_events_list.py
--rw-r--r--   0     1001      122    13414 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/model/storage_config.py
--rw-r--r--   0     1001      122    11080 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/model/storage_uri.py
--rw-r--r--   0     1001      122    11196 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/model/tag_creation.py
--rw-r--r--   0     1001      122    11120 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/model/underlying_object_properties.py
--rw-r--r--   0     1001      122    11760 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/model/update_password_by_token.py
--rw-r--r--   0     1001      122    11138 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/model/update_token.py
--rw-r--r--   0     1001      122    11909 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/model/user.py
--rw-r--r--   0     1001      122    11410 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/model/user_creation.py
--rw-r--r--   0     1001      122    11587 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/model/user_list.py
--rw-r--r--   0     1001      122    11715 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/model/version_config.py
--rw-r--r--   0     1001      122    81856 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/model_utils.py
-drwxr-xr-x   0     1001      122        0 2023-04-05 11:29:14.223569 lakefs-client-0.98.0/lakefs_client/models/
--rw-r--r--   0     1001      122     5899 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/models/__init__.py
--rw-r--r--   0     1001      122    12638 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/lakefs_client/rest.py
-drwxr-xr-x   0     1001      122        0 2023-04-05 11:29:14.211570 lakefs-client-0.98.0/lakefs_client.egg-info/
--rw-r--r--   0     1001      122    23958 2023-04-05 11:29:14.000000 lakefs-client-0.98.0/lakefs_client.egg-info/PKG-INFO
--rw-r--r--   0     1001      122     7588 2023-04-05 11:29:14.000000 lakefs-client-0.98.0/lakefs_client.egg-info/SOURCES.txt
--rw-r--r--   0     1001      122        1 2023-04-05 11:29:14.000000 lakefs-client-0.98.0/lakefs_client.egg-info/dependency_links.txt
--rw-r--r--   0     1001      122       32 2023-04-05 11:29:14.000000 lakefs-client-0.98.0/lakefs_client.egg-info/requires.txt
--rw-r--r--   0     1001      122       14 2023-04-05 11:29:14.000000 lakefs-client-0.98.0/lakefs_client.egg-info/top_level.txt
--rw-r--r--   0     1001      122       69 2023-04-05 11:29:14.235569 lakefs-client-0.98.0/setup.cfg
--rw-r--r--   0     1001      122     1095 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/setup.py
-drwxr-xr-x   0     1001      122        0 2023-04-05 11:29:14.235569 lakefs-client-0.98.0/test/
--rw-r--r--   0     1001      122      768 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_access_key_credentials.py
--rw-r--r--   0     1001      122      647 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_acl.py
--rw-r--r--   0     1001      122      690 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_action_run.py
--rw-r--r--   0     1001      122      898 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_action_run_list.py
--rw-r--r--   0     1001      122     1091 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_actions_api.py
--rw-r--r--   0     1001      122     5486 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_auth_api.py
--rw-r--r--   0     1001      122      739 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_auth_capabilities.py
--rw-r--r--   0     1001      122      760 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_authentication_token.py
--rw-r--r--   0     1001      122      725 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_branch_creation.py
--rw-r--r--   0     1001      122      768 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_branch_protection_rule.py
--rw-r--r--   0     1001      122     1637 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_branches_api.py
--rw-r--r--   0     1001      122      754 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_cherry_pick_creation.py
--rw-r--r--   0     1001      122      726 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_comm_prefs_input.py
--rw-r--r--   0     1001      122      668 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_commit.py
--rw-r--r--   0     1001      122      725 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_commit_creation.py
--rw-r--r--   0     1001      122      863 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_commit_list.py
--rw-r--r--   0     1001      122     1007 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_commits_api.py
--rw-r--r--   0     1001      122     1362 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_config_api.py
--rw-r--r--   0     1001      122      703 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_credentials.py
--rw-r--r--   0     1001      122      918 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_credentials_list.py
--rw-r--r--   0     1001      122      775 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_credentials_with_secret.py
--rw-r--r--   0     1001      122      771 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_current_user.py
--rw-r--r--   0     1001      122      654 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_diff.py
--rw-r--r--   0     1001      122      841 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_diff_list.py
--rw-r--r--   0     1001      122      725 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_diff_properties.py
--rw-r--r--   0     1001      122      661 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_error.py
--rw-r--r--   0     1001      122      698 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_error_no_acl.py
--rw-r--r--   0     1001      122      850 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_experimental_api.py
--rw-r--r--   0     1001      122      762 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_find_merge_base_result.py
--rw-r--r--   0     1001      122      775 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_forgot_password_request.py
--rw-r--r--   0     1001      122      789 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_garbage_collection_config.py
--rw-r--r--   0     1001      122      846 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_garbage_collection_prepare_request.py
--rw-r--r--   0     1001      122      853 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_garbage_collection_prepare_response.py
--rw-r--r--   0     1001      122      775 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_garbage_collection_rule.py
--rw-r--r--   0     1001      122      919 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_garbage_collection_rules.py
--rw-r--r--   0     1001      122      661 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_group.py
--rw-r--r--   0     1001      122      718 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_group_creation.py
--rw-r--r--   0     1001      122      852 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_group_list.py
--rw-r--r--   0     1001      122      651 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_health_check_api.py
--rw-r--r--   0     1001      122      676 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_hook_run.py
--rw-r--r--   0     1001      122      876 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_hook_run_list.py
--rw-r--r--   0     1001      122      877 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_import_api.py
--rw-r--r--   0     1001      122      739 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_import_pagination.py
--rw-r--r--   0     1001      122     1038 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_ingest_range_creation_response.py
--rw-r--r--   0     1001      122      718 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_inline_object1.py
--rw-r--r--   0     1001      122      704 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_login_config.py
--rw-r--r--   0     1001      122      739 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_login_information.py
--rw-r--r--   0     1001      122      661 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_merge.py
--rw-r--r--   0     1001      122      829 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_merge_result.py
--rw-r--r--   0     1001      122      754 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_merge_result_summary.py
--rw-r--r--   0     1001      122      851 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_meta_range_creation.py
--rw-r--r--   0     1001      122      804 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_meta_range_creation_response.py
--rw-r--r--   0     1001      122     1027 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_metadata_api.py
--rw-r--r--   0     1001      122      683 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_next_step.py
--rw-r--r--   0     1001      122      754 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_object_copy_creation.py
--rw-r--r--   0     1001      122      704 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_object_error.py
--rw-r--r--   0     1001      122      829 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_object_error_list.py
--rw-r--r--   0     1001      122      886 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_object_stage_creation.py
--rw-r--r--   0     1001      122      829 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_object_stats.py
--rw-r--r--   0     1001      122      920 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_object_stats_list.py
--rw-r--r--   0     1001      122      754 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_object_user_metadata.py
--rw-r--r--   0     1001      122     2080 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_objects_api.py
--rw-r--r--   0     1001      122      826 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_otf_diff_api.py
--rw-r--r--   0     1001      122      712 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_otf_diff_entry.py
--rw-r--r--   0     1001      122      806 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_otf_diff_list.py
--rw-r--r--   0     1001      122      791 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_otf_diffs.py
--rw-r--r--   0     1001      122      696 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_pagination.py
--rw-r--r--   0     1001      122      683 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_path_list.py
--rw-r--r--   0     1001      122      755 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_policy.py
--rw-r--r--   0     1001      122      863 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_policy_list.py
--rw-r--r--   0     1001      122      818 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_prepare_gc_uncommitted_request.py
--rw-r--r--   0     1001      122      825 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_prepare_gc_uncommitted_response.py
--rw-r--r--   0     1001      122      718 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_range_metadata.py
--rw-r--r--   0     1001      122      647 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_ref.py
--rw-r--r--   0     1001      122      830 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_ref_list.py
--rw-r--r--   0     1001      122     1525 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_refs_api.py
--rw-r--r--   0     1001      122      683 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_refs_dump.py
--rw-r--r--   0     1001      122     1582 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_repositories_api.py
--rw-r--r--   0     1001      122      696 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_repository.py
--rw-r--r--   0     1001      122      753 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_repository_creation.py
--rw-r--r--   0     1001      122      907 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_repository_list.py
--rw-r--r--   0     1001      122      718 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_reset_creation.py
--rw-r--r--   0     1001      122     1398 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_retention_api.py
--rw-r--r--   0     1001      122      725 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_revert_creation.py
--rw-r--r--   0     1001      122      794 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_setup.py
--rw-r--r--   0     1001      122      793 2023-04-05 11:28:58.000000 lakefs-client-0.98.0/test/test_setup_state.py
--rw-r--r--   0     1001      122      754 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_stage_range_creation.py
--rw-r--r--   0     1001      122     1103 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_staging_api.py
--rw-r--r--   0     1001      122      732 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_staging_location.py
--rw-r--r--   0     1001      122      844 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_staging_metadata.py
--rw-r--r--   0     1001      122      689 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_statement.py
--rw-r--r--   0     1001      122      741 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_statistics_api.py
--rw-r--r--   0     1001      122      697 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_stats_event.py
--rw-r--r--   0     1001      122      825 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_stats_events_list.py
--rw-r--r--   0     1001      122      718 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_storage_config.py
--rw-r--r--   0     1001      122      697 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_storage_uri.py
--rw-r--r--   0     1001      122      704 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_tag_creation.py
--rw-r--r--   0     1001      122     1013 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_tags_api.py
--rw-r--r--   0     1001      122      646 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_templates_api.py
--rw-r--r--   0     1001      122      810 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_underlying_object_properties.py
--rw-r--r--   0     1001      122      776 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_update_password_by_token.py
--rw-r--r--   0     1001      122      704 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_update_token.py
--rw-r--r--   0     1001      122      654 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_user.py
--rw-r--r--   0     1001      122      711 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_user_creation.py
--rw-r--r--   0     1001      122      841 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_user_list.py
--rw-r--r--   0     1001      122      718 2023-04-05 11:28:59.000000 lakefs-client-0.98.0/test/test_version_config.py
+drwxr-xr-x   0     1001      122        0 2023-04-19 12:26:03.274401 lakefs-client-0.99.0/
+-rw-r--r--   0     1001      122    23958 2023-04-19 12:26:03.274401 lakefs-client-0.99.0/PKG-INFO
+-rw-r--r--   0     1001      122    23621 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/README.md
+drwxr-xr-x   0     1001      122        0 2023-04-19 12:26:03.226401 lakefs-client-0.99.0/lakefs_client/
+-rw-r--r--   0     1001      122      706 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/lakefs_client/__init__.py
+drwxr-xr-x   0     1001      122        0 2023-04-19 12:26:03.234401 lakefs-client-0.99.0/lakefs_client/api/
+-rw-r--r--   0     1001      122      217 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/lakefs_client/api/__init__.py
+-rw-r--r--   0     1001      122    20697 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/api/actions_api.py
+-rw-r--r--   0     1001      122   149645 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/api/auth_api.py
+-rw-r--r--   0     1001      122    39812 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/api/branches_api.py
+-rw-r--r--   0     1001      122    15812 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/api/commits_api.py
+-rw-r--r--   0     1001      122    24307 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/api/config_api.py
+-rw-r--r--   0     1001      122    10159 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/lakefs_client/api/experimental_api.py
+-rw-r--r--   0     1001      122     4339 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/lakefs_client/api/health_check_api.py
+-rw-r--r--   0     1001      122    10487 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/lakefs_client/api/import_api.py
+-rw-r--r--   0     1001      122    14540 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/lakefs_client/api/metadata_api.py
+-rw-r--r--   0     1001      122    54238 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/lakefs_client/api/objects_api.py
+-rw-r--r--   0     1001      122    10154 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/lakefs_client/api/otf_diff_api.py
+-rw-r--r--   0     1001      122    32626 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/lakefs_client/api/refs_api.py
+-rw-r--r--   0     1001      122    32139 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/lakefs_client/api/repositories_api.py
+-rw-r--r--   0     1001      122    23822 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/lakefs_client/api/retention_api.py
+-rw-r--r--   0     1001      122    16709 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/lakefs_client/api/staging_api.py
+-rw-r--r--   0     1001      122     5165 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/lakefs_client/api/statistics_api.py
+-rw-r--r--   0     1001      122    19140 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/lakefs_client/api/tags_api.py
+-rw-r--r--   0     1001      122     5534 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/lakefs_client/api/templates_api.py
+-rw-r--r--   0     1001      122    36801 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/lakefs_client/api_client.py
+drwxr-xr-x   0     1001      122        0 2023-04-19 12:26:03.234401 lakefs-client-0.99.0/lakefs_client/apis/
+-rw-r--r--   0     1001      122     1393 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/lakefs_client/apis/__init__.py
+-rw-r--r--   0     1001      122     2784 2023-04-19 12:25:15.000000 lakefs-client-0.99.0/lakefs_client/client.py
+-rw-r--r--   0     1001      122    18528 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/lakefs_client/configuration.py
+-rw-r--r--   0     1001      122     5035 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/lakefs_client/exceptions.py
+drwxr-xr-x   0     1001      122        0 2023-04-19 12:26:03.258401 lakefs-client-0.99.0/lakefs_client/model/
+-rw-r--r--   0     1001      122      348 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/lakefs_client/model/__init__.py
+-rw-r--r--   0     1001      122    11898 2023-04-19 12:25:27.000000 lakefs-client-0.99.0/lakefs_client/model/access_key_credentials.py
+-rw-r--r--   0     1001      122    11283 2023-04-19 12:25:27.000000 lakefs-client-0.99.0/lakefs_client/model/acl.py
+-rw-r--r--   0     1001      122    12568 2023-04-19 12:25:27.000000 lakefs-client-0.99.0/lakefs_client/model/action_run.py
+-rw-r--r--   0     1001      122    11638 2023-04-19 12:25:27.000000 lakefs-client-0.99.0/lakefs_client/model/action_run_list.py
+-rw-r--r--   0     1001      122    11286 2023-04-19 12:25:27.000000 lakefs-client-0.99.0/lakefs_client/model/auth_capabilities.py
+-rw-r--r--   0     1001      122    11470 2023-04-19 12:25:27.000000 lakefs-client-0.99.0/lakefs_client/model/authentication_token.py
+-rw-r--r--   0     1001      122    11260 2023-04-19 12:25:27.000000 lakefs-client-0.99.0/lakefs_client/model/branch_creation.py
+-rw-r--r--   0     1001      122    11295 2023-04-19 12:25:27.000000 lakefs-client-0.99.0/lakefs_client/model/branch_protection_rule.py
+-rw-r--r--   0     1001      122    11718 2023-04-19 12:25:27.000000 lakefs-client-0.99.0/lakefs_client/model/cherry_pick_creation.py
+-rw-r--r--   0     1001      122    11848 2023-04-19 12:25:27.000000 lakefs-client-0.99.0/lakefs_client/model/comm_prefs_input.py
+-rw-r--r--   0     1001      122    12549 2023-04-19 12:25:27.000000 lakefs-client-0.99.0/lakefs_client/model/commit.py
+-rw-r--r--   0     1001      122    11635 2023-04-19 12:25:27.000000 lakefs-client-0.99.0/lakefs_client/model/commit_creation.py
+-rw-r--r--   0     1001      122    11607 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/commit_list.py
+-rw-r--r--   0     1001      122    11471 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/credentials.py
+-rw-r--r--   0     1001      122    11657 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/credentials_list.py
+-rw-r--r--   0     1001      122    11834 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/credentials_with_secret.py
+-rw-r--r--   0     1001      122    11181 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/current_user.py
+-rw-r--r--   0     1001      122    12102 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/diff.py
+-rw-r--r--   0     1001      122    11587 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/diff_list.py
+-rw-r--r--   0     1001      122    11048 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/diff_properties.py
+-rw-r--r--   0     1001      122    11124 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/error.py
+-rw-r--r--   0     1001      122    11412 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/error_no_acl.py
+-rw-r--r--   0     1001      122    12082 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/find_merge_base_result.py
+-rw-r--r--   0     1001      122    11080 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/forgot_password_request.py
+-rw-r--r--   0     1001      122    11249 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/garbage_collection_config.py
+-rw-r--r--   0     1001      122    11192 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/garbage_collection_prepare_request.py
+-rw-r--r--   0     1001      122    12236 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/garbage_collection_prepare_response.py
+-rw-r--r--   0     1001      122    11424 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/garbage_collection_rule.py
+-rw-r--r--   0     1001      122    11773 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/garbage_collection_rules.py
+-rw-r--r--   0     1001      122    11332 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/group.py
+-rw-r--r--   0     1001      122    11023 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/group_creation.py
+-rw-r--r--   0     1001      122    11597 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/group_list.py
+-rw-r--r--   0     1001      122    12339 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/hook_run.py
+-rw-r--r--   0     1001      122    11618 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/hook_run_list.py
+-rw-r--r--   0     1001      122    12130 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/import_pagination.py
+-rw-r--r--   0     1001      122    11627 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/ingest_range_creation_response.py
+-rw-r--r--   0     1001      122    11078 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/inline_object1.py
+-rw-r--r--   0     1001      122    13582 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/login_config.py
+-rw-r--r--   0     1001      122    11486 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/login_information.py
+-rw-r--r--   0     1001      122    11938 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/merge.py
+-rw-r--r--   0     1001      122    11529 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/merge_result.py
+-rw-r--r--   0     1001      122    11967 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/merge_result_summary.py
+-rw-r--r--   0     1001      122    11353 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/meta_range_creation.py
+-rw-r--r--   0     1001      122    11095 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/meta_range_creation_response.py
+-rw-r--r--   0     1001      122    11154 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/next_step.py
+-rw-r--r--   0     1001      122    11499 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/object_copy_creation.py
+-rw-r--r--   0     1001      122    11721 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/object_error.py
+-rw-r--r--   0     1001      122    11271 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/object_error_list.py
+-rw-r--r--   0     1001      122    12610 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/object_stage_creation.py
+-rw-r--r--   0     1001      122    13598 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/object_stats.py
+-rw-r--r--   0     1001      122    11658 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/object_stats_list.py
+-rw-r--r--   0     1001      122    10783 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/object_user_metadata.py
+-rw-r--r--   0     1001      122    12651 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/otf_diff_entry.py
+-rw-r--r--   0     1001      122    11620 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/otf_diff_list.py
+-rw-r--r--   0     1001      122    11212 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/otf_diffs.py
+-rw-r--r--   0     1001      122    12264 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/pagination.py
+-rw-r--r--   0     1001      122    11047 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/path_list.py
+-rw-r--r--   0     1001      122    11764 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/policy.py
+-rw-r--r--   0     1001      122    11607 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/policy_list.py
+-rw-r--r--   0     1001      122    11115 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/prepare_gc_uncommitted_request.py
+-rw-r--r--   0     1001      122    11841 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/prepare_gc_uncommitted_response.py
+-rw-r--r--   0     1001      122    12236 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/range_metadata.py
+-rw-r--r--   0     1001      122    11238 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/ref.py
+-rw-r--r--   0     1001      122    11577 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/ref_list.py
+-rw-r--r--   0     1001      122    11949 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/refs_dump.py
+-rw-r--r--   0     1001      122    12148 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/repository.py
+-rw-r--r--   0     1001      122    12102 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/repository_creation.py
+-rw-r--r--   0     1001      122    11647 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/repository_list.py
+-rw-r--r--   0     1001      122    11363 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/reset_creation.py
+-rw-r--r--   0     1001      122    11616 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/revert_creation.py
+-rw-r--r--   0     1001      122    11580 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/setup.py
+-rw-r--r--   0     1001      122    11584 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/setup_state.py
+-rw-r--r--   0     1001      122    12850 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/stage_range_creation.py
+-rw-r--r--   0     1001      122    11870 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/staging_location.py
+-rw-r--r--   0     1001      122    12443 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/staging_metadata.py
+-rw-r--r--   0     1001      122    11661 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/statement.py
+-rw-r--r--   0     1001      122    11918 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/stats_event.py
+-rw-r--r--   0     1001      122    11264 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/stats_events_list.py
+-rw-r--r--   0     1001      122    13414 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/storage_config.py
+-rw-r--r--   0     1001      122    11080 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/storage_uri.py
+-rw-r--r--   0     1001      122    11196 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/tag_creation.py
+-rw-r--r--   0     1001      122    11120 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/underlying_object_properties.py
+-rw-r--r--   0     1001      122    11760 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/update_password_by_token.py
+-rw-r--r--   0     1001      122    11138 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/update_token.py
+-rw-r--r--   0     1001      122    11909 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/user.py
+-rw-r--r--   0     1001      122    11410 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/user_creation.py
+-rw-r--r--   0     1001      122    11587 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/user_list.py
+-rw-r--r--   0     1001      122    11715 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/lakefs_client/model/version_config.py
+-rw-r--r--   0     1001      122    81856 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/lakefs_client/model_utils.py
+drwxr-xr-x   0     1001      122        0 2023-04-19 12:26:03.258401 lakefs-client-0.99.0/lakefs_client/models/
+-rw-r--r--   0     1001      122     5899 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/lakefs_client/models/__init__.py
+-rw-r--r--   0     1001      122    12638 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/lakefs_client/rest.py
+drwxr-xr-x   0     1001      122        0 2023-04-19 12:26:03.230401 lakefs-client-0.99.0/lakefs_client.egg-info/
+-rw-r--r--   0     1001      122    23958 2023-04-19 12:26:03.000000 lakefs-client-0.99.0/lakefs_client.egg-info/PKG-INFO
+-rw-r--r--   0     1001      122     7588 2023-04-19 12:26:03.000000 lakefs-client-0.99.0/lakefs_client.egg-info/SOURCES.txt
+-rw-r--r--   0     1001      122        1 2023-04-19 12:26:03.000000 lakefs-client-0.99.0/lakefs_client.egg-info/dependency_links.txt
+-rw-r--r--   0     1001      122       32 2023-04-19 12:26:03.000000 lakefs-client-0.99.0/lakefs_client.egg-info/requires.txt
+-rw-r--r--   0     1001      122       14 2023-04-19 12:26:03.000000 lakefs-client-0.99.0/lakefs_client.egg-info/top_level.txt
+-rw-r--r--   0     1001      122       69 2023-04-19 12:26:03.274401 lakefs-client-0.99.0/setup.cfg
+-rw-r--r--   0     1001      122     1095 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/setup.py
+drwxr-xr-x   0     1001      122        0 2023-04-19 12:26:03.274401 lakefs-client-0.99.0/test/
+-rw-r--r--   0     1001      122      768 2023-04-19 12:25:27.000000 lakefs-client-0.99.0/test/test_access_key_credentials.py
+-rw-r--r--   0     1001      122      647 2023-04-19 12:25:27.000000 lakefs-client-0.99.0/test/test_acl.py
+-rw-r--r--   0     1001      122      690 2023-04-19 12:25:27.000000 lakefs-client-0.99.0/test/test_action_run.py
+-rw-r--r--   0     1001      122      898 2023-04-19 12:25:27.000000 lakefs-client-0.99.0/test/test_action_run_list.py
+-rw-r--r--   0     1001      122     1091 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_actions_api.py
+-rw-r--r--   0     1001      122     5486 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_auth_api.py
+-rw-r--r--   0     1001      122      739 2023-04-19 12:25:27.000000 lakefs-client-0.99.0/test/test_auth_capabilities.py
+-rw-r--r--   0     1001      122      760 2023-04-19 12:25:27.000000 lakefs-client-0.99.0/test/test_authentication_token.py
+-rw-r--r--   0     1001      122      725 2023-04-19 12:25:27.000000 lakefs-client-0.99.0/test/test_branch_creation.py
+-rw-r--r--   0     1001      122      768 2023-04-19 12:25:27.000000 lakefs-client-0.99.0/test/test_branch_protection_rule.py
+-rw-r--r--   0     1001      122     1637 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_branches_api.py
+-rw-r--r--   0     1001      122      754 2023-04-19 12:25:27.000000 lakefs-client-0.99.0/test/test_cherry_pick_creation.py
+-rw-r--r--   0     1001      122      726 2023-04-19 12:25:27.000000 lakefs-client-0.99.0/test/test_comm_prefs_input.py
+-rw-r--r--   0     1001      122      668 2023-04-19 12:25:27.000000 lakefs-client-0.99.0/test/test_commit.py
+-rw-r--r--   0     1001      122      725 2023-04-19 12:25:27.000000 lakefs-client-0.99.0/test/test_commit_creation.py
+-rw-r--r--   0     1001      122      863 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_commit_list.py
+-rw-r--r--   0     1001      122     1007 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_commits_api.py
+-rw-r--r--   0     1001      122     1362 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_config_api.py
+-rw-r--r--   0     1001      122      703 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_credentials.py
+-rw-r--r--   0     1001      122      918 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_credentials_list.py
+-rw-r--r--   0     1001      122      775 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_credentials_with_secret.py
+-rw-r--r--   0     1001      122      771 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_current_user.py
+-rw-r--r--   0     1001      122      654 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_diff.py
+-rw-r--r--   0     1001      122      841 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_diff_list.py
+-rw-r--r--   0     1001      122      725 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_diff_properties.py
+-rw-r--r--   0     1001      122      661 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_error.py
+-rw-r--r--   0     1001      122      698 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_error_no_acl.py
+-rw-r--r--   0     1001      122      850 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/test/test_experimental_api.py
+-rw-r--r--   0     1001      122      762 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_find_merge_base_result.py
+-rw-r--r--   0     1001      122      775 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_forgot_password_request.py
+-rw-r--r--   0     1001      122      789 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_garbage_collection_config.py
+-rw-r--r--   0     1001      122      846 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_garbage_collection_prepare_request.py
+-rw-r--r--   0     1001      122      853 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_garbage_collection_prepare_response.py
+-rw-r--r--   0     1001      122      775 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_garbage_collection_rule.py
+-rw-r--r--   0     1001      122      919 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_garbage_collection_rules.py
+-rw-r--r--   0     1001      122      661 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_group.py
+-rw-r--r--   0     1001      122      718 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_group_creation.py
+-rw-r--r--   0     1001      122      852 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_group_list.py
+-rw-r--r--   0     1001      122      651 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/test/test_health_check_api.py
+-rw-r--r--   0     1001      122      676 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_hook_run.py
+-rw-r--r--   0     1001      122      876 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_hook_run_list.py
+-rw-r--r--   0     1001      122      877 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/test/test_import_api.py
+-rw-r--r--   0     1001      122      739 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_import_pagination.py
+-rw-r--r--   0     1001      122     1038 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_ingest_range_creation_response.py
+-rw-r--r--   0     1001      122      718 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_inline_object1.py
+-rw-r--r--   0     1001      122      704 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_login_config.py
+-rw-r--r--   0     1001      122      739 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_login_information.py
+-rw-r--r--   0     1001      122      661 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_merge.py
+-rw-r--r--   0     1001      122      829 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_merge_result.py
+-rw-r--r--   0     1001      122      754 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_merge_result_summary.py
+-rw-r--r--   0     1001      122      851 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_meta_range_creation.py
+-rw-r--r--   0     1001      122      804 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_meta_range_creation_response.py
+-rw-r--r--   0     1001      122     1027 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/test/test_metadata_api.py
+-rw-r--r--   0     1001      122      683 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_next_step.py
+-rw-r--r--   0     1001      122      754 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_object_copy_creation.py
+-rw-r--r--   0     1001      122      704 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_object_error.py
+-rw-r--r--   0     1001      122      829 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_object_error_list.py
+-rw-r--r--   0     1001      122      886 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_object_stage_creation.py
+-rw-r--r--   0     1001      122      829 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_object_stats.py
+-rw-r--r--   0     1001      122      920 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_object_stats_list.py
+-rw-r--r--   0     1001      122      754 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_object_user_metadata.py
+-rw-r--r--   0     1001      122     2080 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/test/test_objects_api.py
+-rw-r--r--   0     1001      122      826 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/test/test_otf_diff_api.py
+-rw-r--r--   0     1001      122      712 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_otf_diff_entry.py
+-rw-r--r--   0     1001      122      806 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_otf_diff_list.py
+-rw-r--r--   0     1001      122      791 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_otf_diffs.py
+-rw-r--r--   0     1001      122      696 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_pagination.py
+-rw-r--r--   0     1001      122      683 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_path_list.py
+-rw-r--r--   0     1001      122      755 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_policy.py
+-rw-r--r--   0     1001      122      863 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_policy_list.py
+-rw-r--r--   0     1001      122      818 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_prepare_gc_uncommitted_request.py
+-rw-r--r--   0     1001      122      825 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_prepare_gc_uncommitted_response.py
+-rw-r--r--   0     1001      122      718 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_range_metadata.py
+-rw-r--r--   0     1001      122      647 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_ref.py
+-rw-r--r--   0     1001      122      830 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_ref_list.py
+-rw-r--r--   0     1001      122     1525 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/test/test_refs_api.py
+-rw-r--r--   0     1001      122      683 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_refs_dump.py
+-rw-r--r--   0     1001      122     1582 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/test/test_repositories_api.py
+-rw-r--r--   0     1001      122      696 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_repository.py
+-rw-r--r--   0     1001      122      753 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_repository_creation.py
+-rw-r--r--   0     1001      122      907 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_repository_list.py
+-rw-r--r--   0     1001      122      718 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_reset_creation.py
+-rw-r--r--   0     1001      122     1398 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/test/test_retention_api.py
+-rw-r--r--   0     1001      122      725 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_revert_creation.py
+-rw-r--r--   0     1001      122      794 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_setup.py
+-rw-r--r--   0     1001      122      793 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_setup_state.py
+-rw-r--r--   0     1001      122      754 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_stage_range_creation.py
+-rw-r--r--   0     1001      122     1103 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/test/test_staging_api.py
+-rw-r--r--   0     1001      122      732 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_staging_location.py
+-rw-r--r--   0     1001      122      844 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_staging_metadata.py
+-rw-r--r--   0     1001      122      689 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_statement.py
+-rw-r--r--   0     1001      122      741 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/test/test_statistics_api.py
+-rw-r--r--   0     1001      122      697 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_stats_event.py
+-rw-r--r--   0     1001      122      825 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_stats_events_list.py
+-rw-r--r--   0     1001      122      718 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_storage_config.py
+-rw-r--r--   0     1001      122      697 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_storage_uri.py
+-rw-r--r--   0     1001      122      704 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_tag_creation.py
+-rw-r--r--   0     1001      122     1013 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/test/test_tags_api.py
+-rw-r--r--   0     1001      122      646 2023-04-19 12:25:29.000000 lakefs-client-0.99.0/test/test_templates_api.py
+-rw-r--r--   0     1001      122      810 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_underlying_object_properties.py
+-rw-r--r--   0     1001      122      776 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_update_password_by_token.py
+-rw-r--r--   0     1001      122      704 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_update_token.py
+-rw-r--r--   0     1001      122      654 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_user.py
+-rw-r--r--   0     1001      122      711 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_user_creation.py
+-rw-r--r--   0     1001      122      841 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_user_list.py
+-rw-r--r--   0     1001      122      718 2023-04-19 12:25:28.000000 lakefs-client-0.99.0/test/test_version_config.py
```

### Comparing `lakefs-client-0.98.0/PKG-INFO` & `lakefs-client-0.99.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakefs-client
-Version: 0.98.0
+Version: 0.99.0
 Summary: lakeFS API
 Home-page: https://github.com/treeverse/lakeFS/tree/master/clients/python
 Author: Treeverse
 Author-email: services@treeverse.io
 License: Apache 2.0
 Keywords: OpenAPI,OpenAPI-Generator,lakeFS API
 Requires-Python: >=3.6
@@ -12,15 +12,15 @@
 
 # lakefs-client
 lakeFS HTTP API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 0.1.0
-- Package version: 0.98.0
+- Package version: 0.99.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python >= 3.6
 
 ## Installation & Usage
```

### Comparing `lakefs-client-0.98.0/README.md` & `lakefs-client-0.99.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lakefs-client
 lakeFS HTTP API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 0.1.0
-- Package version: 0.98.0
+- Package version: 0.99.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python >= 3.6
 
 ## Installation & Usage
```

### Comparing `lakefs-client-0.98.0/lakefs_client/__init__.py` & `lakefs-client-0.99.0/lakefs_client/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The version of the OpenAPI document: 0.1.0
     Contact: services@treeverse.io
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.98.0"
+__version__ = "0.99.0"
 
 # import ApiClient
 from lakefs_client.api_client import ApiClient
 
 # import Configuration
 from lakefs_client.configuration import Configuration
```

### Comparing `lakefs-client-0.98.0/lakefs_client/api/actions_api.py` & `lakefs-client-0.99.0/lakefs_client/api/actions_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/api/auth_api.py` & `lakefs-client-0.99.0/lakefs_client/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/api/branches_api.py` & `lakefs-client-0.99.0/lakefs_client/api/branches_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/api/commits_api.py` & `lakefs-client-0.99.0/lakefs_client/api/commits_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/api/config_api.py` & `lakefs-client-0.99.0/lakefs_client/api/config_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/api/experimental_api.py` & `lakefs-client-0.99.0/lakefs_client/api/experimental_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/api/health_check_api.py` & `lakefs-client-0.99.0/lakefs_client/api/health_check_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/api/import_api.py` & `lakefs-client-0.99.0/lakefs_client/api/import_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/api/metadata_api.py` & `lakefs-client-0.99.0/lakefs_client/api/metadata_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/api/objects_api.py` & `lakefs-client-0.99.0/lakefs_client/api/objects_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/api/otf_diff_api.py` & `lakefs-client-0.99.0/lakefs_client/api/otf_diff_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/api/refs_api.py` & `lakefs-client-0.99.0/lakefs_client/api/refs_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/api/repositories_api.py` & `lakefs-client-0.99.0/lakefs_client/api/repositories_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/api/retention_api.py` & `lakefs-client-0.99.0/lakefs_client/api/retention_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/api/staging_api.py` & `lakefs-client-0.99.0/lakefs_client/api/staging_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/api/statistics_api.py` & `lakefs-client-0.99.0/lakefs_client/api/statistics_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/api/tags_api.py` & `lakefs-client-0.99.0/lakefs_client/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/api/templates_api.py` & `lakefs-client-0.99.0/lakefs_client/api/templates_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/api_client.py` & `lakefs-client-0.99.0/lakefs_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'lakefs-python-sdk/0.98.0'
+        self.user_agent = 'lakefs-python-sdk/0.99.0'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lakefs-client-0.98.0/lakefs_client/apis/__init__.py` & `lakefs-client-0.99.0/lakefs_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/client.py` & `lakefs-client-0.99.0/lakefs_client/client.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/configuration.py` & `lakefs-client-0.99.0/lakefs_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -452,15 +452,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.1.0\n"\
-               "SDK Package Version: 0.98.0".\
+               "SDK Package Version: 0.99.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lakefs-client-0.98.0/lakefs_client/exceptions.py` & `lakefs-client-0.99.0/lakefs_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/access_key_credentials.py` & `lakefs-client-0.99.0/lakefs_client/model/access_key_credentials.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/acl.py` & `lakefs-client-0.99.0/lakefs_client/model/acl.py`

 * *Files 7% similar despite different names*

```diff
@@ -79,27 +79,23 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'permission': (str,),  # noqa: E501
-            'all_repositories': (bool,),  # noqa: E501
-            'repositories': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'permission': 'permission',  # noqa: E501
-        'all_repositories': 'all_repositories',  # noqa: E501
-        'repositories': 'repositories',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -138,16 +134,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            all_repositories (bool): If true, this ACL applies to all repositories, including those added in future.  Permission \"Admin\" allows changing ACLs, so this is necessarily true for that permission. . [optional]  # noqa: E501
-            repositories ([str]): Apply this ACL only to these repositories.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -225,16 +219,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            all_repositories (bool): If true, this ACL applies to all repositories, including those added in future.  Permission \"Admin\" allows changing ACLs, so this is necessarily true for that permission. . [optional]  # noqa: E501
-            repositories ([str]): Apply this ACL only to these repositories.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `lakefs-client-0.98.0/lakefs_client/model/action_run.py` & `lakefs-client-0.99.0/lakefs_client/model/action_run.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/action_run_list.py` & `lakefs-client-0.99.0/lakefs_client/model/action_run_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/auth_capabilities.py` & `lakefs-client-0.99.0/lakefs_client/model/auth_capabilities.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/authentication_token.py` & `lakefs-client-0.99.0/lakefs_client/model/authentication_token.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/branch_creation.py` & `lakefs-client-0.99.0/lakefs_client/model/branch_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/branch_protection_rule.py` & `lakefs-client-0.99.0/lakefs_client/model/branch_protection_rule.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/cherry_pick_creation.py` & `lakefs-client-0.99.0/lakefs_client/model/cherry_pick_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/comm_prefs_input.py` & `lakefs-client-0.99.0/lakefs_client/model/comm_prefs_input.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/commit.py` & `lakefs-client-0.99.0/lakefs_client/model/commit.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/commit_creation.py` & `lakefs-client-0.99.0/lakefs_client/model/commit_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/commit_list.py` & `lakefs-client-0.99.0/lakefs_client/model/commit_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/credentials.py` & `lakefs-client-0.99.0/lakefs_client/model/credentials.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/credentials_list.py` & `lakefs-client-0.99.0/lakefs_client/model/credentials_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/credentials_with_secret.py` & `lakefs-client-0.99.0/lakefs_client/model/credentials_with_secret.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/current_user.py` & `lakefs-client-0.99.0/lakefs_client/model/current_user.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/diff.py` & `lakefs-client-0.99.0/lakefs_client/model/diff.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/diff_list.py` & `lakefs-client-0.99.0/lakefs_client/model/diff_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/diff_properties.py` & `lakefs-client-0.99.0/lakefs_client/model/diff_properties.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/error.py` & `lakefs-client-0.99.0/lakefs_client/model/error.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/error_no_acl.py` & `lakefs-client-0.99.0/lakefs_client/model/error_no_acl.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/find_merge_base_result.py` & `lakefs-client-0.99.0/lakefs_client/model/find_merge_base_result.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/forgot_password_request.py` & `lakefs-client-0.99.0/lakefs_client/model/forgot_password_request.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/garbage_collection_config.py` & `lakefs-client-0.99.0/lakefs_client/model/garbage_collection_config.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/garbage_collection_prepare_request.py` & `lakefs-client-0.99.0/lakefs_client/model/garbage_collection_prepare_request.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/garbage_collection_prepare_response.py` & `lakefs-client-0.99.0/lakefs_client/model/garbage_collection_prepare_response.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/garbage_collection_rule.py` & `lakefs-client-0.99.0/lakefs_client/model/garbage_collection_rule.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/garbage_collection_rules.py` & `lakefs-client-0.99.0/lakefs_client/model/garbage_collection_rules.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/group.py` & `lakefs-client-0.99.0/lakefs_client/model/group.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/group_creation.py` & `lakefs-client-0.99.0/lakefs_client/model/group_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/group_list.py` & `lakefs-client-0.99.0/lakefs_client/model/group_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/hook_run.py` & `lakefs-client-0.99.0/lakefs_client/model/hook_run.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/hook_run_list.py` & `lakefs-client-0.99.0/lakefs_client/model/hook_run_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/import_pagination.py` & `lakefs-client-0.99.0/lakefs_client/model/import_pagination.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/ingest_range_creation_response.py` & `lakefs-client-0.99.0/lakefs_client/model/ingest_range_creation_response.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/inline_object1.py` & `lakefs-client-0.99.0/lakefs_client/model/inline_object1.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/login_config.py` & `lakefs-client-0.99.0/lakefs_client/model/login_config.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/login_information.py` & `lakefs-client-0.99.0/lakefs_client/model/login_information.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/merge.py` & `lakefs-client-0.99.0/lakefs_client/model/merge.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/merge_result.py` & `lakefs-client-0.99.0/lakefs_client/model/merge_result.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/merge_result_summary.py` & `lakefs-client-0.99.0/lakefs_client/model/merge_result_summary.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/meta_range_creation.py` & `lakefs-client-0.99.0/lakefs_client/model/meta_range_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/meta_range_creation_response.py` & `lakefs-client-0.99.0/lakefs_client/model/meta_range_creation_response.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/next_step.py` & `lakefs-client-0.99.0/lakefs_client/model/next_step.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/object_copy_creation.py` & `lakefs-client-0.99.0/lakefs_client/model/object_copy_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/object_error.py` & `lakefs-client-0.99.0/lakefs_client/model/object_error.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/object_error_list.py` & `lakefs-client-0.99.0/lakefs_client/model/object_error_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/object_stage_creation.py` & `lakefs-client-0.99.0/lakefs_client/model/object_stage_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/object_stats.py` & `lakefs-client-0.99.0/lakefs_client/model/object_stats.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/object_stats_list.py` & `lakefs-client-0.99.0/lakefs_client/model/object_stats_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/object_user_metadata.py` & `lakefs-client-0.99.0/lakefs_client/model/object_user_metadata.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/otf_diff_entry.py` & `lakefs-client-0.99.0/lakefs_client/model/otf_diff_entry.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/otf_diff_list.py` & `lakefs-client-0.99.0/lakefs_client/model/otf_diff_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/otf_diffs.py` & `lakefs-client-0.99.0/lakefs_client/model/otf_diffs.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/pagination.py` & `lakefs-client-0.99.0/lakefs_client/model/pagination.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/path_list.py` & `lakefs-client-0.99.0/lakefs_client/model/path_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/policy.py` & `lakefs-client-0.99.0/lakefs_client/model/policy.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/policy_list.py` & `lakefs-client-0.99.0/lakefs_client/model/policy_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/prepare_gc_uncommitted_request.py` & `lakefs-client-0.99.0/lakefs_client/model/prepare_gc_uncommitted_request.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/prepare_gc_uncommitted_response.py` & `lakefs-client-0.99.0/lakefs_client/model/prepare_gc_uncommitted_response.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/range_metadata.py` & `lakefs-client-0.99.0/lakefs_client/model/range_metadata.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/ref.py` & `lakefs-client-0.99.0/lakefs_client/model/ref.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/ref_list.py` & `lakefs-client-0.99.0/lakefs_client/model/ref_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/refs_dump.py` & `lakefs-client-0.99.0/lakefs_client/model/refs_dump.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/repository.py` & `lakefs-client-0.99.0/lakefs_client/model/repository.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/repository_creation.py` & `lakefs-client-0.99.0/lakefs_client/model/repository_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/repository_list.py` & `lakefs-client-0.99.0/lakefs_client/model/repository_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/reset_creation.py` & `lakefs-client-0.99.0/lakefs_client/model/reset_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/revert_creation.py` & `lakefs-client-0.99.0/lakefs_client/model/revert_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/setup.py` & `lakefs-client-0.99.0/lakefs_client/model/setup.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/setup_state.py` & `lakefs-client-0.99.0/lakefs_client/model/setup_state.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/stage_range_creation.py` & `lakefs-client-0.99.0/lakefs_client/model/stage_range_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/staging_location.py` & `lakefs-client-0.99.0/lakefs_client/model/staging_location.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/staging_metadata.py` & `lakefs-client-0.99.0/lakefs_client/model/staging_metadata.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/statement.py` & `lakefs-client-0.99.0/lakefs_client/model/statement.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/stats_event.py` & `lakefs-client-0.99.0/lakefs_client/model/stats_event.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/stats_events_list.py` & `lakefs-client-0.99.0/lakefs_client/model/stats_events_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/storage_config.py` & `lakefs-client-0.99.0/lakefs_client/model/storage_config.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/storage_uri.py` & `lakefs-client-0.99.0/lakefs_client/model/storage_uri.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/tag_creation.py` & `lakefs-client-0.99.0/lakefs_client/model/tag_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/underlying_object_properties.py` & `lakefs-client-0.99.0/lakefs_client/model/underlying_object_properties.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/update_password_by_token.py` & `lakefs-client-0.99.0/lakefs_client/model/update_password_by_token.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/update_token.py` & `lakefs-client-0.99.0/lakefs_client/model/update_token.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/user.py` & `lakefs-client-0.99.0/lakefs_client/model/user.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/user_creation.py` & `lakefs-client-0.99.0/lakefs_client/model/user_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/user_list.py` & `lakefs-client-0.99.0/lakefs_client/model/user_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model/version_config.py` & `lakefs-client-0.99.0/lakefs_client/model/version_config.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/model_utils.py` & `lakefs-client-0.99.0/lakefs_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/models/__init__.py` & `lakefs-client-0.99.0/lakefs_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client/rest.py` & `lakefs-client-0.99.0/lakefs_client/rest.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/lakefs_client.egg-info/PKG-INFO` & `lakefs-client-0.99.0/lakefs_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakefs-client
-Version: 0.98.0
+Version: 0.99.0
 Summary: lakeFS API
 Home-page: https://github.com/treeverse/lakeFS/tree/master/clients/python
 Author: Treeverse
 Author-email: services@treeverse.io
 License: Apache 2.0
 Keywords: OpenAPI,OpenAPI-Generator,lakeFS API
 Requires-Python: >=3.6
@@ -12,15 +12,15 @@
 
 # lakefs-client
 lakeFS HTTP API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 0.1.0
-- Package version: 0.98.0
+- Package version: 0.99.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python >= 3.6
 
 ## Installation & Usage
```

### Comparing `lakefs-client-0.98.0/lakefs_client.egg-info/SOURCES.txt` & `lakefs-client-0.99.0/lakefs_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/setup.py` & `lakefs-client-0.99.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "lakefs-client"
-VERSION = "0.98.0"
+VERSION = "0.99.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `lakefs-client-0.98.0/test/test_access_key_credentials.py` & `lakefs-client-0.99.0/test/test_access_key_credentials.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_acl.py` & `lakefs-client-0.99.0/test/test_acl.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_action_run.py` & `lakefs-client-0.99.0/test/test_action_run.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_action_run_list.py` & `lakefs-client-0.99.0/test/test_action_run_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_actions_api.py` & `lakefs-client-0.99.0/test/test_actions_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_auth_api.py` & `lakefs-client-0.99.0/test/test_auth_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_auth_capabilities.py` & `lakefs-client-0.99.0/test/test_auth_capabilities.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_authentication_token.py` & `lakefs-client-0.99.0/test/test_authentication_token.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_branch_creation.py` & `lakefs-client-0.99.0/test/test_branch_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_branch_protection_rule.py` & `lakefs-client-0.99.0/test/test_branch_protection_rule.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_branches_api.py` & `lakefs-client-0.99.0/test/test_branches_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_cherry_pick_creation.py` & `lakefs-client-0.99.0/test/test_cherry_pick_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_comm_prefs_input.py` & `lakefs-client-0.99.0/test/test_comm_prefs_input.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_commit.py` & `lakefs-client-0.99.0/test/test_commit.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_commit_creation.py` & `lakefs-client-0.99.0/test/test_commit_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_commit_list.py` & `lakefs-client-0.99.0/test/test_commit_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_commits_api.py` & `lakefs-client-0.99.0/test/test_commits_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_config_api.py` & `lakefs-client-0.99.0/test/test_config_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_credentials.py` & `lakefs-client-0.99.0/test/test_credentials.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_credentials_list.py` & `lakefs-client-0.99.0/test/test_credentials_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_credentials_with_secret.py` & `lakefs-client-0.99.0/test/test_credentials_with_secret.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_current_user.py` & `lakefs-client-0.99.0/test/test_current_user.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_diff.py` & `lakefs-client-0.99.0/test/test_diff.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_diff_list.py` & `lakefs-client-0.99.0/test/test_diff_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_diff_properties.py` & `lakefs-client-0.99.0/test/test_diff_properties.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_error.py` & `lakefs-client-0.99.0/test/test_error.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_error_no_acl.py` & `lakefs-client-0.99.0/test/test_error_no_acl.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_experimental_api.py` & `lakefs-client-0.99.0/test/test_experimental_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_find_merge_base_result.py` & `lakefs-client-0.99.0/test/test_find_merge_base_result.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_forgot_password_request.py` & `lakefs-client-0.99.0/test/test_forgot_password_request.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_garbage_collection_config.py` & `lakefs-client-0.99.0/test/test_garbage_collection_config.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_garbage_collection_prepare_request.py` & `lakefs-client-0.99.0/test/test_garbage_collection_prepare_request.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_garbage_collection_prepare_response.py` & `lakefs-client-0.99.0/test/test_garbage_collection_prepare_response.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_garbage_collection_rule.py` & `lakefs-client-0.99.0/test/test_garbage_collection_rule.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_garbage_collection_rules.py` & `lakefs-client-0.99.0/test/test_garbage_collection_rules.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_group.py` & `lakefs-client-0.99.0/test/test_group.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_group_creation.py` & `lakefs-client-0.99.0/test/test_group_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_group_list.py` & `lakefs-client-0.99.0/test/test_group_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_health_check_api.py` & `lakefs-client-0.99.0/test/test_health_check_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_hook_run.py` & `lakefs-client-0.99.0/test/test_hook_run.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_hook_run_list.py` & `lakefs-client-0.99.0/test/test_hook_run_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_import_api.py` & `lakefs-client-0.99.0/test/test_import_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_import_pagination.py` & `lakefs-client-0.99.0/test/test_import_pagination.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_ingest_range_creation_response.py` & `lakefs-client-0.99.0/test/test_ingest_range_creation_response.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_inline_object1.py` & `lakefs-client-0.99.0/test/test_inline_object1.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_login_config.py` & `lakefs-client-0.99.0/test/test_login_config.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_login_information.py` & `lakefs-client-0.99.0/test/test_login_information.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_merge.py` & `lakefs-client-0.99.0/test/test_merge.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_merge_result.py` & `lakefs-client-0.99.0/test/test_merge_result.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_merge_result_summary.py` & `lakefs-client-0.99.0/test/test_merge_result_summary.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_meta_range_creation.py` & `lakefs-client-0.99.0/test/test_meta_range_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_meta_range_creation_response.py` & `lakefs-client-0.99.0/test/test_meta_range_creation_response.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_metadata_api.py` & `lakefs-client-0.99.0/test/test_metadata_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_next_step.py` & `lakefs-client-0.99.0/test/test_next_step.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_object_copy_creation.py` & `lakefs-client-0.99.0/test/test_object_copy_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_object_error.py` & `lakefs-client-0.99.0/test/test_object_error.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_object_error_list.py` & `lakefs-client-0.99.0/test/test_object_error_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_object_stage_creation.py` & `lakefs-client-0.99.0/test/test_object_stage_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_object_stats.py` & `lakefs-client-0.99.0/test/test_object_stats.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_object_stats_list.py` & `lakefs-client-0.99.0/test/test_object_stats_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_object_user_metadata.py` & `lakefs-client-0.99.0/test/test_object_user_metadata.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_objects_api.py` & `lakefs-client-0.99.0/test/test_objects_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_otf_diff_api.py` & `lakefs-client-0.99.0/test/test_otf_diff_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_otf_diff_entry.py` & `lakefs-client-0.99.0/test/test_otf_diff_entry.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_otf_diff_list.py` & `lakefs-client-0.99.0/test/test_otf_diff_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_otf_diffs.py` & `lakefs-client-0.99.0/test/test_otf_diffs.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_pagination.py` & `lakefs-client-0.99.0/test/test_pagination.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_path_list.py` & `lakefs-client-0.99.0/test/test_path_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_policy.py` & `lakefs-client-0.99.0/test/test_policy.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_policy_list.py` & `lakefs-client-0.99.0/test/test_policy_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_prepare_gc_uncommitted_request.py` & `lakefs-client-0.99.0/test/test_prepare_gc_uncommitted_request.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_prepare_gc_uncommitted_response.py` & `lakefs-client-0.99.0/test/test_prepare_gc_uncommitted_response.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_range_metadata.py` & `lakefs-client-0.99.0/test/test_range_metadata.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_ref.py` & `lakefs-client-0.99.0/test/test_ref.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_ref_list.py` & `lakefs-client-0.99.0/test/test_ref_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_refs_api.py` & `lakefs-client-0.99.0/test/test_refs_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_refs_dump.py` & `lakefs-client-0.99.0/test/test_refs_dump.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_repositories_api.py` & `lakefs-client-0.99.0/test/test_repositories_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_repository.py` & `lakefs-client-0.99.0/test/test_repository.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_repository_creation.py` & `lakefs-client-0.99.0/test/test_repository_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_repository_list.py` & `lakefs-client-0.99.0/test/test_repository_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_reset_creation.py` & `lakefs-client-0.99.0/test/test_reset_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_retention_api.py` & `lakefs-client-0.99.0/test/test_retention_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_revert_creation.py` & `lakefs-client-0.99.0/test/test_revert_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_setup.py` & `lakefs-client-0.99.0/test/test_setup.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_setup_state.py` & `lakefs-client-0.99.0/test/test_setup_state.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_stage_range_creation.py` & `lakefs-client-0.99.0/test/test_stage_range_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_staging_api.py` & `lakefs-client-0.99.0/test/test_staging_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_staging_location.py` & `lakefs-client-0.99.0/test/test_staging_location.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_staging_metadata.py` & `lakefs-client-0.99.0/test/test_staging_metadata.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_statement.py` & `lakefs-client-0.99.0/test/test_statement.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_statistics_api.py` & `lakefs-client-0.99.0/test/test_statistics_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_stats_event.py` & `lakefs-client-0.99.0/test/test_stats_event.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_stats_events_list.py` & `lakefs-client-0.99.0/test/test_stats_events_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_storage_config.py` & `lakefs-client-0.99.0/test/test_storage_config.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_storage_uri.py` & `lakefs-client-0.99.0/test/test_storage_uri.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_tag_creation.py` & `lakefs-client-0.99.0/test/test_tag_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_tags_api.py` & `lakefs-client-0.99.0/test/test_tags_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_templates_api.py` & `lakefs-client-0.99.0/test/test_templates_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_underlying_object_properties.py` & `lakefs-client-0.99.0/test/test_underlying_object_properties.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_update_password_by_token.py` & `lakefs-client-0.99.0/test/test_update_password_by_token.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_update_token.py` & `lakefs-client-0.99.0/test/test_update_token.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_user.py` & `lakefs-client-0.99.0/test/test_user.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_user_creation.py` & `lakefs-client-0.99.0/test/test_user_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_user_list.py` & `lakefs-client-0.99.0/test/test_user_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-0.98.0/test/test_version_config.py` & `lakefs-client-0.99.0/test/test_version_config.py`

 * *Files identical despite different names*

