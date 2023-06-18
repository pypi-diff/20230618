# Comparing `tmp/foursight_core-4.3.0.1b8.tar.gz` & `tmp/foursight_core-4.3.0.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_core-4.3.0.1b8.tar", max compression
+gzip compressed data, was "foursight_core-4.3.0.1b9.tar", max compression
```

## Comparing `foursight_core-4.3.0.1b8.tar` & `foursight_core-4.3.0.1b9.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1083 2023-06-16 21:21:32.521840 foursight_core-4.3.0.1b8/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-06-16 21:21:32.525840 foursight_core-4.3.0.1b8/foursight_core/__init__.py
--rw-r--r--   0        0        0     1901 2023-06-16 21:21:32.525840 foursight_core-4.3.0.1b8/foursight_core/abstract_connection.py
--rw-r--r--   0        0        0       69 2023-06-16 21:21:32.525840 foursight_core-4.3.0.1b8/foursight_core/app.py
--rw-r--r--   0        0        0   105657 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/app_utils.py
--rw-r--r--   0        0        0     2611 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/buckets.py
--rw-r--r--   0        0        0      638 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/check_schema.py
--rw-r--r--   0        0        0        3 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/check_setup.json
--rw-r--r--   0        0        0    22858 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/check_utils.py
--rw-r--r--   0        0        0      270 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/checks/__init__.py
--rw-r--r--   0        0        0     6115 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/checks/access_key_expiration_detection.py
--rw-r--r--   0        0        0     2899 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/checks/codebuild_checks.py
--rw-r--r--   0        0        0     3305 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/checks/ecs_checks.py
--rw-r--r--   0        0        0     4683 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/checks/ecs_recovery_check.py
--rw-r--r--   0        0        0        0 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/checks/helpers/__init__.py
--rw-r--r--   0        0        0      348 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/checks/helpers/confchecks.py
--rw-r--r--   0        0        0     3519 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/checks/helpers/sys_utils.py
--rw-r--r--   0        0        0     2055 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0     8375 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/checks/scaling_checks.py
--rw-r--r--   0        0        0     2658 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/checks/test_checks.py
--rw-r--r--   0        0        0    11929 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/decorators.py
--rw-r--r--   0        0        0    15050 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/deploy.py
--rw-r--r--   0        0        0     8302 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/environment.py
--rw-r--r--   0        0        0    11792 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/es_connection.py
--rw-r--r--   0        0        0     1176 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/exceptions.py
--rw-r--r--   0        0        0     5408 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/fs_connection.py
--rw-r--r--   0        0        0     8423 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/identity.py
--rw-r--r--   0        0        0     3082 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/mapping.json
--rw-r--r--   0        0        0     1014 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/package.py
--rw-r--r--   0        0        0    16912 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/react/api/auth.py
--rw-r--r--   0        0        0     6629 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/react/api/auth0_config.py
--rw-r--r--   0        0        0    22994 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/react/api/aws_network.py
--rw-r--r--   0        0        0     3093 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/react/api/aws_s3.py
--rw-r--r--   0        0        0     6116 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/react/api/aws_stacks.py
--rw-r--r--   0        0        0    28009 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/react/api/checks.py
--rw-r--r--   0        0        0    20464 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/react/api/cognito.py
--rw-r--r--   0        0        0     3952 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/react/api/cookie_utils.py
--rw-r--r--   0        0        0     6189 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/react/api/datetime_utils.py
--rw-r--r--   0        0        0     1841 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/react/api/encoding_utils.py
--rw-r--r--   0        0        0     3649 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/react/api/encryption.py
--rw-r--r--   0        0        0     4720 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/react/api/envs.py
--rw-r--r--   0        0        0     3196 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/react/api/gac.py
--rw-r--r--   0        0        0     3516 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/react/api/jwt_utils.py
--rw-r--r--   0        0        0     9466 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/react/api/misc_utils.py
--rw-r--r--   0        0        0     5250 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/react/api/portal_access_key_utils.py
--rw-r--r--   0        0        0    81643 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/react/api/react_api.py
--rw-r--r--   0        0        0    11210 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/react/api/react_api_base.py
--rw-r--r--   0        0        0     8025 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/react/api/react_route_decorator.py
--rw-r--r--   0        0        0    34216 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/react/api/react_routes.py
--rw-r--r--   0        0        0     4805 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/react/api/react_ui.py
--rw-r--r--   0        0        0      806 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/react/api/yaml_utils.py
--rw-r--r--   0        0        0      234 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/react/ui/asset-manifest.json
--rw-r--r--   0        0        0     1681 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/react/ui/index.html
--rw-r--r--   0        0        0        3 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/react/ui/manifest.json
--rw-r--r--   0        0        0    11735 2023-06-16 21:21:32.529840 foursight_core-4.3.0.1b8/foursight_core/react/ui/static/css/main.css
--rw-r--r--   0        0        0  1936472 2023-06-16 21:21:32.541840 foursight_core-4.3.0.1b8/foursight_core/react/ui/static/js/main.js
--rw-r--r--   0        0        0      597 2023-06-16 21:21:32.541840 foursight_core-4.3.0.1b8/foursight_core/route_prefixes.py
--rw-r--r--   0        0        0    10496 2023-06-16 21:21:32.541840 foursight_core-4.3.0.1b8/foursight_core/routes.py
--rw-r--r--   0        0        0    22481 2023-06-16 21:21:32.541840 foursight_core-4.3.0.1b8/foursight_core/run_result.py
--rw-r--r--   0        0        0     6389 2023-06-16 21:21:32.541840 foursight_core-4.3.0.1b8/foursight_core/s3_connection.py
--rw-r--r--   0        0        0     5282 2023-06-16 21:21:32.541840 foursight_core-4.3.0.1b8/foursight_core/schedule_decorator.py
--rw-r--r--   0        0        0     1402 2023-06-16 21:21:32.541840 foursight_core-4.3.0.1b8/foursight_core/scripts/decrypt_accounts_file.py
--rw-r--r--   0        0        0     1406 2023-06-16 21:21:32.541840 foursight_core-4.3.0.1b8/foursight_core/scripts/encrypt_accounts_file.py
--rw-r--r--   0        0        0     5886 2023-06-16 21:21:32.541840 foursight_core-4.3.0.1b8/foursight_core/sqs_utils.py
--rw-r--r--   0        0        0     1715 2023-06-16 21:21:32.541840 foursight_core-4.3.0.1b8/foursight_core/stage.py
--rw-r--r--   0        0        0     7763 2023-06-16 21:21:32.541840 foursight_core-4.3.0.1b8/foursight_core/templates/base.html
--rw-r--r--   0        0        0    20532 2023-06-16 21:21:32.541840 foursight_core-4.3.0.1b8/foursight_core/templates/header.html
--rw-r--r--   0        0        0     4090 2023-06-16 21:21:32.541840 foursight_core-4.3.0.1b8/foursight_core/templates/history.html
--rw-r--r--   0        0        0    19634 2023-06-16 21:21:32.541840 foursight_core-4.3.0.1b8/foursight_core/templates/info.html
--rw-r--r--   0        0        0     1297 2023-06-16 21:21:32.541840 foursight_core-4.3.0.1b8/foursight_core/templates/unused.html
--rw-r--r--   0        0        0     2259 2023-06-16 21:21:32.541840 foursight_core-4.3.0.1b8/foursight_core/templates/user.html
--rw-r--r--   0        0        0     1669 2023-06-16 21:21:32.541840 foursight_core-4.3.0.1b8/foursight_core/templates/users.html
--rw-r--r--   0        0        0      572 2023-06-16 21:21:32.541840 foursight_core-4.3.0.1b8/foursight_core/templates/view_checks.html
--rw-r--r--   0        0        0     2248 2023-06-16 21:21:32.541840 foursight_core-4.3.0.1b8/foursight_core/templates/view_groups.html
--rw-r--r--   0        0        0     1636 2023-06-16 21:21:32.545840 foursight_core-4.3.0.1b8/pyproject.toml
--rw-r--r--   0        0        0     1197 1970-01-01 00:00:00.000000 foursight_core-4.3.0.1b8/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-16 21:43:26.544503 foursight_core-4.3.0.1b9/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/__init__.py
+-rw-r--r--   0        0        0     1901 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/abstract_connection.py
+-rw-r--r--   0        0        0       69 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/app.py
+-rw-r--r--   0        0        0   105698 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/app_utils.py
+-rw-r--r--   0        0        0     2611 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/buckets.py
+-rw-r--r--   0        0        0      638 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/check_schema.py
+-rw-r--r--   0        0        0        3 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/check_setup.json
+-rw-r--r--   0        0        0    22858 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/check_utils.py
+-rw-r--r--   0        0        0      270 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/checks/__init__.py
+-rw-r--r--   0        0        0     6117 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/checks/access_key_expiration_detection.py
+-rw-r--r--   0        0        0     2899 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/checks/codebuild_checks.py
+-rw-r--r--   0        0        0     3305 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/checks/ecs_checks.py
+-rw-r--r--   0        0        0     4683 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/checks/ecs_recovery_check.py
+-rw-r--r--   0        0        0        0 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/checks/helpers/__init__.py
+-rw-r--r--   0        0        0      348 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0     3519 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/checks/helpers/sys_utils.py
+-rw-r--r--   0        0        0     2055 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0     8375 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/checks/scaling_checks.py
+-rw-r--r--   0        0        0     2658 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/checks/test_checks.py
+-rw-r--r--   0        0        0    11929 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/decorators.py
+-rw-r--r--   0        0        0    15050 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/deploy.py
+-rw-r--r--   0        0        0     8302 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/environment.py
+-rw-r--r--   0        0        0    11792 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/es_connection.py
+-rw-r--r--   0        0        0     1176 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/exceptions.py
+-rw-r--r--   0        0        0     5408 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/fs_connection.py
+-rw-r--r--   0        0        0     8423 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/identity.py
+-rw-r--r--   0        0        0     3082 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/mapping.json
+-rw-r--r--   0        0        0     1014 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/package.py
+-rw-r--r--   0        0        0    16912 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/react/api/auth.py
+-rw-r--r--   0        0        0     6629 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/react/api/auth0_config.py
+-rw-r--r--   0        0        0    22994 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/react/api/aws_network.py
+-rw-r--r--   0        0        0     3093 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/react/api/aws_s3.py
+-rw-r--r--   0        0        0     6116 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/react/api/aws_stacks.py
+-rw-r--r--   0        0        0    28009 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/react/api/checks.py
+-rw-r--r--   0        0        0    20464 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/react/api/cognito.py
+-rw-r--r--   0        0        0     3952 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/react/api/cookie_utils.py
+-rw-r--r--   0        0        0     6189 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/react/api/datetime_utils.py
+-rw-r--r--   0        0        0     1841 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/react/api/encoding_utils.py
+-rw-r--r--   0        0        0     3649 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/react/api/encryption.py
+-rw-r--r--   0        0        0     4720 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/react/api/envs.py
+-rw-r--r--   0        0        0     3196 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/react/api/gac.py
+-rw-r--r--   0        0        0     3516 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/react/api/jwt_utils.py
+-rw-r--r--   0        0        0     9466 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/react/api/misc_utils.py
+-rw-r--r--   0        0        0     5250 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/react/api/portal_access_key_utils.py
+-rw-r--r--   0        0        0    81643 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/react/api/react_api.py
+-rw-r--r--   0        0        0    11210 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/react/api/react_api_base.py
+-rw-r--r--   0        0        0     8025 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/react/api/react_route_decorator.py
+-rw-r--r--   0        0        0    34216 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/react/api/react_routes.py
+-rw-r--r--   0        0        0     4805 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/react/api/react_ui.py
+-rw-r--r--   0        0        0      806 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/react/api/yaml_utils.py
+-rw-r--r--   0        0        0      234 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/react/ui/asset-manifest.json
+-rw-r--r--   0        0        0     1681 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/react/ui/index.html
+-rw-r--r--   0        0        0        3 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/react/ui/manifest.json
+-rw-r--r--   0        0        0    11735 2023-06-16 21:43:26.552503 foursight_core-4.3.0.1b9/foursight_core/react/ui/static/css/main.css
+-rw-r--r--   0        0        0  1936472 2023-06-16 21:43:26.564504 foursight_core-4.3.0.1b9/foursight_core/react/ui/static/js/main.js
+-rw-r--r--   0        0        0      597 2023-06-16 21:43:26.564504 foursight_core-4.3.0.1b9/foursight_core/route_prefixes.py
+-rw-r--r--   0        0        0    10496 2023-06-16 21:43:26.564504 foursight_core-4.3.0.1b9/foursight_core/routes.py
+-rw-r--r--   0        0        0    22980 2023-06-16 21:43:26.564504 foursight_core-4.3.0.1b9/foursight_core/run_result.py
+-rw-r--r--   0        0        0     6389 2023-06-16 21:43:26.564504 foursight_core-4.3.0.1b9/foursight_core/s3_connection.py
+-rw-r--r--   0        0        0     5282 2023-06-16 21:43:26.564504 foursight_core-4.3.0.1b9/foursight_core/schedule_decorator.py
+-rw-r--r--   0        0        0     1402 2023-06-16 21:43:26.564504 foursight_core-4.3.0.1b9/foursight_core/scripts/decrypt_accounts_file.py
+-rw-r--r--   0        0        0     1406 2023-06-16 21:43:26.564504 foursight_core-4.3.0.1b9/foursight_core/scripts/encrypt_accounts_file.py
+-rw-r--r--   0        0        0     5886 2023-06-16 21:43:26.564504 foursight_core-4.3.0.1b9/foursight_core/sqs_utils.py
+-rw-r--r--   0        0        0     1715 2023-06-16 21:43:26.564504 foursight_core-4.3.0.1b9/foursight_core/stage.py
+-rw-r--r--   0        0        0     7763 2023-06-16 21:43:26.564504 foursight_core-4.3.0.1b9/foursight_core/templates/base.html
+-rw-r--r--   0        0        0    20532 2023-06-16 21:43:26.564504 foursight_core-4.3.0.1b9/foursight_core/templates/header.html
+-rw-r--r--   0        0        0     4090 2023-06-16 21:43:26.564504 foursight_core-4.3.0.1b9/foursight_core/templates/history.html
+-rw-r--r--   0        0        0    19634 2023-06-16 21:43:26.564504 foursight_core-4.3.0.1b9/foursight_core/templates/info.html
+-rw-r--r--   0        0        0     1297 2023-06-16 21:43:26.564504 foursight_core-4.3.0.1b9/foursight_core/templates/unused.html
+-rw-r--r--   0        0        0     2259 2023-06-16 21:43:26.564504 foursight_core-4.3.0.1b9/foursight_core/templates/user.html
+-rw-r--r--   0        0        0     1669 2023-06-16 21:43:26.564504 foursight_core-4.3.0.1b9/foursight_core/templates/users.html
+-rw-r--r--   0        0        0      572 2023-06-16 21:43:26.564504 foursight_core-4.3.0.1b9/foursight_core/templates/view_checks.html
+-rw-r--r--   0        0        0     2248 2023-06-16 21:43:26.564504 foursight_core-4.3.0.1b9/foursight_core/templates/view_groups.html
+-rw-r--r--   0        0        0     1636 2023-06-16 21:43:26.568503 foursight_core-4.3.0.1b9/pyproject.toml
+-rw-r--r--   0        0        0     1197 1970-01-01 00:00:00.000000 foursight_core-4.3.0.1b9/PKG-INFO
```

### Comparing `foursight_core-4.3.0.1b8/LICENSE.txt` & `foursight_core-4.3.0.1b9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/abstract_connection.py` & `foursight_core-4.3.0.1b9/foursight_core/abstract_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/app_utils.py` & `foursight_core-4.3.0.1b9/foursight_core/app_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2002,15 +2002,15 @@
                     logger.warning(f'-RUN-> Wrote action record: {rec_key}')
             run_result = self.check_handler.run_check_or_action(connection, run_name, run_kwargs)
             logger.warning('-RUN-> RESULT:  %s (uuid)' % str(run_result.get('uuid')))
             # invoke action if running a check and kwargs['queue_action'] matches stage
             stage = self.stage.get_stage()
             if run_result['type'] == 'check' and run_result['kwargs']['queue_action'] == stage:
                 # must also have check.action and check.allow_action set
-                if run_result['allow_action'] and run_result['action']:
+                if run_result['allow_action'] and run_result['action'] and not run_result.get('prevent_action'):
                     action_params = {'check_name': run_result['name'],
                                      'called_by': run_result['kwargs']['uuid']}
                     try:
                         self.queue_action(run_env, run_result['action'],
                                           params=action_params, uuid=run_uuid)
                     except Exception as exc:
                         logger.warning('-RUN-> Could not queue action %s on stage %s with kwargs: %s. Error: %s'
```

### Comparing `foursight_core-4.3.0.1b8/foursight_core/buckets.py` & `foursight_core-4.3.0.1b9/foursight_core/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/check_schema.py` & `foursight_core-4.3.0.1b9/foursight_core/check_schema.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/check_utils.py` & `foursight_core-4.3.0.1b9/foursight_core/check_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/checks/access_key_expiration_detection.py` & `foursight_core-4.3.0.1b9/foursight_core/checks/access_key_expiration_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,21 +43,21 @@
         check.brief_output = check.full_output = check.summary
         return check
     elif now > three_weeks_to_expiration:
         check.status = 'WARN'
         check.summary = (f'Application access keys will expire in less than 21 days! Please run'
                          f' the deployment action soon')
         check.brief_output = check.full_output = check.summary
-        check.allow_action = False
+        check.prevent_action = True
         return check
     else:
         check.status = 'PASS'
         check.summary = (f'Application access keys expiration is more than 3 weeks away. All good.'
                          f' Expiration date: {expiration_date}')
-        check.allow_action = False
+        check.prevent_action = True
         return check
 
 
 @action_function()
 def refresh_access_keys(connection, **kwargs):
     """ Triggers a refresh of the 3 admin keys, previously run through the portal """
     action = ActionResult(connection, 'refresh_access_keys')
```

### Comparing `foursight_core-4.3.0.1b8/foursight_core/checks/codebuild_checks.py` & `foursight_core-4.3.0.1b9/foursight_core/checks/codebuild_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/checks/ecs_checks.py` & `foursight_core-4.3.0.1b9/foursight_core/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/checks/ecs_recovery_check.py` & `foursight_core-4.3.0.1b9/foursight_core/checks/ecs_recovery_check.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/checks/helpers/sys_utils.py` & `foursight_core-4.3.0.1b9/foursight_core/checks/helpers/sys_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/checks/helpers/wrangler_utils.py` & `foursight_core-4.3.0.1b9/foursight_core/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/checks/scaling_checks.py` & `foursight_core-4.3.0.1b9/foursight_core/checks/scaling_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/checks/test_checks.py` & `foursight_core-4.3.0.1b9/foursight_core/checks/test_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/decorators.py` & `foursight_core-4.3.0.1b9/foursight_core/decorators.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/deploy.py` & `foursight_core-4.3.0.1b9/foursight_core/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/environment.py` & `foursight_core-4.3.0.1b9/foursight_core/environment.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/es_connection.py` & `foursight_core-4.3.0.1b9/foursight_core/es_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/exceptions.py` & `foursight_core-4.3.0.1b9/foursight_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/fs_connection.py` & `foursight_core-4.3.0.1b9/foursight_core/fs_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/identity.py` & `foursight_core-4.3.0.1b9/foursight_core/identity.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/mapping.json` & `foursight_core-4.3.0.1b9/foursight_core/mapping.json`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/package.py` & `foursight_core-4.3.0.1b9/foursight_core/package.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/react/api/auth.py` & `foursight_core-4.3.0.1b9/foursight_core/react/api/auth.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/react/api/auth0_config.py` & `foursight_core-4.3.0.1b9/foursight_core/react/api/auth0_config.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/react/api/aws_network.py` & `foursight_core-4.3.0.1b9/foursight_core/react/api/aws_network.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/react/api/aws_s3.py` & `foursight_core-4.3.0.1b9/foursight_core/react/api/aws_s3.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/react/api/aws_stacks.py` & `foursight_core-4.3.0.1b9/foursight_core/react/api/aws_stacks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/react/api/checks.py` & `foursight_core-4.3.0.1b9/foursight_core/react/api/checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/react/api/cognito.py` & `foursight_core-4.3.0.1b9/foursight_core/react/api/cognito.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/react/api/cookie_utils.py` & `foursight_core-4.3.0.1b9/foursight_core/react/api/cookie_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/react/api/datetime_utils.py` & `foursight_core-4.3.0.1b9/foursight_core/react/api/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/react/api/encoding_utils.py` & `foursight_core-4.3.0.1b9/foursight_core/react/api/encoding_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/react/api/encryption.py` & `foursight_core-4.3.0.1b9/foursight_core/react/api/encryption.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/react/api/envs.py` & `foursight_core-4.3.0.1b9/foursight_core/react/api/envs.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/react/api/gac.py` & `foursight_core-4.3.0.1b9/foursight_core/react/api/gac.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/react/api/jwt_utils.py` & `foursight_core-4.3.0.1b9/foursight_core/react/api/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/react/api/misc_utils.py` & `foursight_core-4.3.0.1b9/foursight_core/react/api/misc_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/react/api/portal_access_key_utils.py` & `foursight_core-4.3.0.1b9/foursight_core/react/api/portal_access_key_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/react/api/react_api.py` & `foursight_core-4.3.0.1b9/foursight_core/react/api/react_api.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/react/api/react_api_base.py` & `foursight_core-4.3.0.1b9/foursight_core/react/api/react_api_base.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/react/api/react_route_decorator.py` & `foursight_core-4.3.0.1b9/foursight_core/react/api/react_route_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/react/api/react_routes.py` & `foursight_core-4.3.0.1b9/foursight_core/react/api/react_routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/react/api/react_ui.py` & `foursight_core-4.3.0.1b9/foursight_core/react/api/react_ui.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/react/api/yaml_utils.py` & `foursight_core-4.3.0.1b9/foursight_core/react/api/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/react/ui/index.html` & `foursight_core-4.3.0.1b9/foursight_core/react/ui/index.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/react/ui/static/css/main.css` & `foursight_core-4.3.0.1b9/foursight_core/react/ui/static/css/main.css`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/react/ui/static/js/main.js` & `foursight_core-4.3.0.1b9/foursight_core/react/ui/static/js/main.js`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/route_prefixes.py` & `foursight_core-4.3.0.1b9/foursight_core/route_prefixes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/routes.py` & `foursight_core-4.3.0.1b9/foursight_core/routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/run_result.py` & `foursight_core-4.3.0.1b9/foursight_core/run_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -367,14 +367,19 @@
         self.full_output = None
         # admin output is only seen by admins on the UI
         self.admin_output = None
         self.ff_link = ''
         # self.action_name is the function name of the action to link to check
         self.action = ''
         self.allow_action = False  # by default do not allow the action to be run
+        # Added prevent_action to allow the allow_action flag to be True, so action *may* *always*
+        # be run, but does not automatically run after check; this came up with the access_key_status
+        # check, where we always want to allow the action to be manually run, but want to prevent it from
+        # running after the check run, unless it is expiring soon; see: access_key_expiration_detection.
+        self.prevent_action = False
         self.action_message = 'Are you sure you want to run this action?'
 
     def format_result(self, uuid):
         # use summary as description if descrip is missing
         if self.summary and not self.description:
             use_description = self.summary
         else:
@@ -387,14 +392,15 @@
             'uuid': uuid,
             'brief_output': self.brief_output,
             'full_output': self.full_output,
             'admin_output': self.admin_output,
             'ff_link': self.ff_link,
             'action': self.action,
             'allow_action': self.allow_action,
+            'prevent_action': self.prevent_action,
             'action_message': self.action_message,
             'kwargs': self.kwargs,
             'type': 'check'
         }
 
     def validate(self):
         """
```

### Comparing `foursight_core-4.3.0.1b8/foursight_core/s3_connection.py` & `foursight_core-4.3.0.1b9/foursight_core/s3_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/schedule_decorator.py` & `foursight_core-4.3.0.1b9/foursight_core/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/scripts/decrypt_accounts_file.py` & `foursight_core-4.3.0.1b9/foursight_core/scripts/decrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/scripts/encrypt_accounts_file.py` & `foursight_core-4.3.0.1b9/foursight_core/scripts/encrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/sqs_utils.py` & `foursight_core-4.3.0.1b9/foursight_core/sqs_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/stage.py` & `foursight_core-4.3.0.1b9/foursight_core/stage.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/templates/base.html` & `foursight_core-4.3.0.1b9/foursight_core/templates/base.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/templates/header.html` & `foursight_core-4.3.0.1b9/foursight_core/templates/header.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/templates/history.html` & `foursight_core-4.3.0.1b9/foursight_core/templates/history.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/templates/info.html` & `foursight_core-4.3.0.1b9/foursight_core/templates/info.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/templates/unused.html` & `foursight_core-4.3.0.1b9/foursight_core/templates/unused.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/templates/user.html` & `foursight_core-4.3.0.1b9/foursight_core/templates/user.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/templates/users.html` & `foursight_core-4.3.0.1b9/foursight_core/templates/users.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/templates/view_checks.html` & `foursight_core-4.3.0.1b9/foursight_core/templates/view_checks.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/foursight_core/templates/view_groups.html` & `foursight_core-4.3.0.1b9/foursight_core/templates/view_groups.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b8/pyproject.toml` & `foursight_core-4.3.0.1b9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight-core"
-version = "4.3.0.1b8"  # TODO: To become 4.4.0
+version = "4.3.0.1b9"  # TODO: To become 4.4.0
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "foursight_core" },
   { include = "checks", from = "foursight_core" },
   { include = "helpers", from = "foursight_core/checks" }
```

### Comparing `foursight_core-4.3.0.1b8/PKG-INFO` & `foursight_core-4.3.0.1b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-core
-Version: 4.3.0.1b8
+Version: 4.3.0.1b9
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

