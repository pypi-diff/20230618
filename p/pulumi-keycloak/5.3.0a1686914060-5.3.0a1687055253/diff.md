# Comparing `tmp/pulumi_keycloak-5.3.0a1686914060.tar.gz` & `tmp/pulumi_keycloak-5.3.0a1687055253.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_keycloak-5.3.0a1686914060.tar", last modified: Fri Jun 16 11:19:08 2023, max compression
+gzip compressed data, was "pulumi_keycloak-5.3.0a1687055253.tar", last modified: Sun Jun 18 02:34:58 2023, max compression
```

## Comparing `pulumi_keycloak-5.3.0a1686914060.tar` & `pulumi_keycloak-5.3.0a1687055253.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:19:08.732838 pulumi_keycloak-5.3.0a1686914060/
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-16 11:19:08.732838 pulumi_keycloak-5.3.0a1686914060/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:19:08.720838 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/
--rw-r--r--   0 runner    (1001) docker     (123)    20526 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   102617 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    27739 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/attribute_importer_identity_provider_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21933 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/attribute_to_role_identity_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:19:08.720838 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24520 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/authentication/bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)    16713 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/authentication/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)    15432 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/authentication/execution_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/authentication/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    23130 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/authentication/subflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:19:08.720838 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    18978 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/custom_identity_provider_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    29602 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/custom_user_federation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/default_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/default_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    23092 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/generic_client_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    22211 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/generic_client_role_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    23868 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/generic_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21773 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/generic_role_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/get_authentication_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/get_authentication_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    26196 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/get_client_description_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    37193 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/get_realm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/get_realm_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/get_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/get_user_realm_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/group_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)    18691 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/group_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18844 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/group_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    16923 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/hardcoded_attribute_identity_provider_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12330 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/hardcoded_role_identity_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    24404 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/identity_provider_token_exchange_scope_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:19:08.724838 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/ldap/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/ldap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/ldap/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20564 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/ldap/full_name_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    57296 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/ldap/group_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    18399 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/ldap/hardcoded_attribute_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11925 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/ldap/hardcoded_group_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    19079 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/ldap/hardcoded_role_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    14278 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/ldap/msad_lds_user_account_control_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    17667 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/ldap/msad_user_account_control_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/ldap/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46485 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/ldap/role_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    31107 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/ldap/user_attribute_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    85992 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/ldap/user_federation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:19:08.724838 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/oidc/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69494 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/oidc/google_identity_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    82330 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/oidc/identity_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:19:08.728839 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18351 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29325 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/audience_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    17901 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/audience_resolve_protocol_mappter.py
--rw-r--r--   0 runner    (1001) docker     (123)   146214 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13673 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_aggregate_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18086 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_authorization_permission.py
--rw-r--r--   0 runner    (1001) docker     (123)    17909 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_authorization_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_authorization_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    12598 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_default_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_group_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14315 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_js_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_optional_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)    23020 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21830 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14933 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_role_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    20270 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_service_account_realm_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    15794 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_service_account_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    27525 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_time_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13479 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_user_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/full_name_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    30167 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/get_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/get_client_authorization_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/get_client_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/get_client_service_account_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    29689 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/group_membership_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    32107 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/hardcoded_claim_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    19846 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/hardcoded_role_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21973 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34832 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/script_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    37290 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/user_attribute_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    38593 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/user_client_role_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    33237 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/user_property_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    35135 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/user_realm_role_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    30199 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/user_session_note_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    94592 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16755 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   157967 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/realm.py
--rw-r--r--   0 runner    (1001) docker     (123)    25046 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/realm_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    18172 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/realm_keystore_aes_generated.py
--rw-r--r--   0 runner    (1001) docker     (123)    17421 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/realm_keystore_ecdsa_generated.py
--rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/realm_keystore_hmac_generated.py
--rw-r--r--   0 runner    (1001) docker     (123)    25062 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/realm_keystore_java_generated.py
--rw-r--r--   0 runner    (1001) docker     (123)    19806 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/realm_keystore_rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)    18943 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/realm_keystore_rsa_generated.py
--rw-r--r--   0 runner    (1001) docker     (123)    18132 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/realm_user_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    17148 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/required_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    23764 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:19:08.732838 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/saml/
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/saml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/saml/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    99872 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/saml/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/saml/client_default_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/saml/client_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    23628 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/saml/get_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/saml/get_client_installation_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)   103281 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/saml/identity_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/saml/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28175 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/saml/script_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    25945 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/saml/user_attribute_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    25910 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/saml/user_property_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    27809 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    16660 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/user_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    16648 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/user_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    20139 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/user_template_importer_identity_provider_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    19558 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/users_permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:19:08.720838 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 11:19:08.732838 pulumi_keycloak-5.3.0a1686914060/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-16 11:19:08.000000 pulumi_keycloak-5.3.0a1686914060/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:34:58.438357 pulumi_keycloak-5.3.0a1687055253/
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-18 02:34:58.438357 pulumi_keycloak-5.3.0a1687055253/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:34:58.422357 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/
+-rw-r--r--   0 runner    (1001) docker     (123)    20526 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102617 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27739 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/attribute_importer_identity_provider_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21933 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/attribute_to_role_identity_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:34:58.426357 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24520 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/authentication/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16713 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/authentication/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15432 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/authentication/execution_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/authentication/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23130 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/authentication/subflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:34:58.426357 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18978 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/custom_identity_provider_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29602 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/custom_user_federation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/default_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/default_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23092 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/generic_client_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22211 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/generic_client_role_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23868 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/generic_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21773 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/generic_role_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/get_authentication_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/get_authentication_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26196 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/get_client_description_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37193 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/get_realm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/get_realm_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/get_user_realm_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/group_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18691 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/group_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18844 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/group_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16923 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/hardcoded_attribute_identity_provider_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12330 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/hardcoded_role_identity_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24404 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/identity_provider_token_exchange_scope_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:34:58.430357 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/ldap/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/ldap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/ldap/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20564 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/ldap/full_name_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57296 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/ldap/group_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18399 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/ldap/hardcoded_attribute_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11925 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/ldap/hardcoded_group_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19079 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/ldap/hardcoded_role_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14278 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/ldap/msad_lds_user_account_control_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17667 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/ldap/msad_user_account_control_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/ldap/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46485 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/ldap/role_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31107 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/ldap/user_attribute_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85992 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/ldap/user_federation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:34:58.430357 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/oidc/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69494 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/oidc/google_identity_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82330 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/oidc/identity_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:34:58.434357 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18351 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29325 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/audience_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17901 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/audience_resolve_protocol_mappter.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146214 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13673 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_aggregate_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18086 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_authorization_permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17909 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_authorization_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_authorization_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12598 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_default_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_group_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14315 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_js_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_optional_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23020 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21830 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14933 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_role_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20270 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_service_account_realm_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15794 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_service_account_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27525 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_time_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13479 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_user_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/full_name_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30167 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/get_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/get_client_authorization_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/get_client_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/get_client_service_account_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29689 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/group_membership_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32107 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/hardcoded_claim_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19846 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/hardcoded_role_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21973 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34832 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/script_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37290 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/user_attribute_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38593 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/user_client_role_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33237 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/user_property_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35135 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/user_realm_role_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30199 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/user_session_note_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94592 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16755 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   157967 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/realm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25046 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/realm_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18172 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/realm_keystore_aes_generated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17421 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/realm_keystore_ecdsa_generated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/realm_keystore_hmac_generated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25062 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/realm_keystore_java_generated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19806 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/realm_keystore_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18943 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/realm_keystore_rsa_generated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18132 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/realm_user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17148 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/required_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23764 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:34:58.438357 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/saml/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/saml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/saml/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99872 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/saml/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/saml/client_default_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/saml/client_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23628 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/saml/get_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/saml/get_client_installation_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103281 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/saml/identity_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/saml/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28175 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/saml/script_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25945 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/saml/user_attribute_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25910 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/saml/user_property_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27809 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16660 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16648 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/user_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20139 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/user_template_importer_identity_provider_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19558 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/users_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:34:58.422357 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-18 02:34:58.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-18 02:34:58.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:34:58.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:34:58.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-18 02:34:58.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-18 02:34:58.000000 pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 02:34:58.438357 pulumi_keycloak-5.3.0a1687055253/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-18 02:34:57.000000 pulumi_keycloak-5.3.0a1687055253/setup.py
```

### Comparing `pulumi_keycloak-5.3.0a1686914060/PKG-INFO` & `pulumi_keycloak-5.3.0a1687055253/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_keycloak
-Version: 5.3.0a1686914060
+Version: 5.3.0a1687055253
 Summary: A Pulumi package for creating and managing keycloak cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-keycloak
 Keywords: pulumi keycloak
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_keycloak-5.3.0a1686914060/README.md` & `pulumi_keycloak-5.3.0a1687055253/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/__init__.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/_inputs.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/_utilities.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/attribute_importer_identity_provider_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/attribute_importer_identity_provider_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/attribute_to_role_identity_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/attribute_to_role_identity_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/authentication/bindings.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/authentication/bindings.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/authentication/execution.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/authentication/execution.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/authentication/execution_config.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/authentication/execution_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/authentication/flow.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/authentication/flow.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/authentication/subflow.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/authentication/subflow.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/config/vars.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/custom_identity_provider_mapping.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/custom_identity_provider_mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/custom_user_federation.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/custom_user_federation.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/default_groups.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/default_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/default_roles.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/default_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/generic_client_protocol_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/generic_client_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/generic_client_role_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/generic_client_role_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/generic_protocol_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/generic_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/generic_role_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/generic_role_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/get_authentication_execution.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/get_authentication_execution.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/get_authentication_flow.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/get_authentication_flow.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/get_client_description_converter.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/get_client_description_converter.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/get_group.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/get_realm.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/get_realm.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/get_realm_keys.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/get_realm_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/get_role.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/get_user.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/get_user_realm_roles.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/get_user_realm_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/group.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/group_memberships.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/group_memberships.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/group_permissions.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/group_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/group_roles.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/group_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/hardcoded_attribute_identity_provider_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/hardcoded_attribute_identity_provider_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/hardcoded_role_identity_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/hardcoded_role_identity_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/identity_provider_token_exchange_scope_permission.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/identity_provider_token_exchange_scope_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/ldap/__init__.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/ldap/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/ldap/_inputs.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/ldap/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/ldap/full_name_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/ldap/full_name_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/ldap/group_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/ldap/group_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/ldap/hardcoded_attribute_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/ldap/hardcoded_attribute_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/ldap/hardcoded_group_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/ldap/hardcoded_group_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/ldap/hardcoded_role_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/ldap/hardcoded_role_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/ldap/msad_lds_user_account_control_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/ldap/msad_lds_user_account_control_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/ldap/msad_user_account_control_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/ldap/msad_user_account_control_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/ldap/outputs.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/ldap/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/ldap/role_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/ldap/role_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/ldap/user_attribute_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/ldap/user_attribute_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/ldap/user_federation.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/ldap/user_federation.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/oidc/google_identity_provider.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/oidc/google_identity_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/oidc/identity_provider.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/oidc/identity_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/__init__.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/_inputs.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/audience_protocol_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/audience_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/audience_resolve_protocol_mappter.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/audience_resolve_protocol_mappter.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_aggregate_policy.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_aggregate_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_authorization_permission.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_authorization_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_authorization_resource.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_authorization_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_authorization_scope.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_authorization_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_default_scopes.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_default_scopes.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_group_policy.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_group_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_js_policy.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_js_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_optional_scopes.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_optional_scopes.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_permissions.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_policy.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_role_policy.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_role_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_scope.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_service_account_realm_role.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_service_account_realm_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_service_account_role.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_service_account_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_time_policy.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_time_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/client_user_policy.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/client_user_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/full_name_protocol_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/full_name_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/get_client.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/get_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/get_client_authorization_policy.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/get_client_authorization_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/get_client_scope.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/get_client_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/get_client_service_account_user.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/get_client_service_account_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/group_membership_protocol_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/group_membership_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/hardcoded_claim_protocol_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/hardcoded_claim_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/hardcoded_role_protocol_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/hardcoded_role_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/outputs.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/script_protocol_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/script_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/user_attribute_protocol_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/user_attribute_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/user_client_role_protocol_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/user_client_role_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/user_property_protocol_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/user_property_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/user_realm_role_protocol_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/user_realm_role_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/openid/user_session_note_protocol_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/openid/user_session_note_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/outputs.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/provider.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/realm.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/realm.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/realm_events.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/realm_events.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/realm_keystore_aes_generated.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/realm_keystore_aes_generated.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/realm_keystore_ecdsa_generated.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/realm_keystore_ecdsa_generated.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/realm_keystore_hmac_generated.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/realm_keystore_hmac_generated.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/realm_keystore_java_generated.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/realm_keystore_java_generated.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/realm_keystore_rsa.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/realm_keystore_rsa.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/realm_keystore_rsa_generated.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/realm_keystore_rsa_generated.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/realm_user_profile.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/realm_user_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/required_action.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/required_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/role.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/saml/__init__.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/saml/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/saml/_inputs.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/saml/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/saml/client.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/saml/client.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/saml/client_default_scope.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/saml/client_default_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/saml/client_scope.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/saml/client_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/saml/get_client.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/saml/get_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/saml/get_client_installation_provider.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/saml/get_client_installation_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/saml/identity_provider.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/saml/identity_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/saml/outputs.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/saml/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/saml/script_protocol_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/saml/script_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/saml/user_attribute_protocol_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/saml/user_attribute_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/saml/user_property_protocol_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/saml/user_property_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/user.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/user_groups.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/user_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/user_roles.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/user_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/user_template_importer_identity_provider_mapper.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/user_template_importer_identity_provider_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak/users_permissions.py` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak/users_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak.egg-info/PKG-INFO` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-keycloak
-Version: 5.3.0a1686914060
+Version: 5.3.0a1687055253
 Summary: A Pulumi package for creating and managing keycloak cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-keycloak
 Keywords: pulumi keycloak
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_keycloak-5.3.0a1686914060/pulumi_keycloak.egg-info/SOURCES.txt` & `pulumi_keycloak-5.3.0a1687055253/pulumi_keycloak.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.3.0a1686914060/setup.py` & `pulumi_keycloak-5.3.0a1687055253/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "5.3.0a1686914060"
-PLUGIN_VERSION = "5.3.0-alpha.1686914060+b09005da"
+VERSION = "5.3.0a1687055253"
+PLUGIN_VERSION = "5.3.0-alpha.1687055253+ab79fede"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'keycloak', PLUGIN_VERSION])
         except OSError as error:
```

