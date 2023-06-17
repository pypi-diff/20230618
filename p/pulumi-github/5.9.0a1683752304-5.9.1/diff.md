# Comparing `tmp/pulumi_github-5.9.0a1683752304.tar.gz` & `tmp/pulumi_github-5.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_github-5.9.0a1683752304.tar", last modified: Wed May 10 21:12:33 2023, max compression
+gzip compressed data, was "pulumi_github-5.9.1.tar", last modified: Tue May 23 19:12:43 2023, max compression
```

## Comparing `pulumi_github-5.9.0a1683752304.tar` & `pulumi_github-5.9.1.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:12:33.662678 pulumi_github-5.9.0a1683752304/
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-10 21:12:33.662678 pulumi_github-5.9.0a1683752304/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:12:33.662678 pulumi_github-5.9.0a1683752304/pulumi_github/
--rw-r--r--   0 runner    (1001) docker     (123)    15525 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63092 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    19178 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/actions_environment_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    16013 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/actions_environment_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/actions_organization_oidc_subject_claim_customization_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    20745 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/actions_organization_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22394 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/actions_organization_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/actions_organization_secret_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/actions_organization_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/actions_repository_access_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/actions_repository_oidc_subject_claim_customization_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    16292 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/actions_repository_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25998 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/actions_runner_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    15530 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/actions_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/actions_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/app_installation_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)    11169 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/app_installation_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16865 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/branch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/branch_default.py
--rw-r--r--   0 runner    (1001) docker     (123)    44058 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/branch_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    31972 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/branch_protection_v3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:12:33.662678 pulumi_github-5.9.0a1683752304/pulumi_github/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    18662 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/dependabot_organization_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/dependabot_organization_secret_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/dependabot_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/emu_group_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    14654 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/enterprise_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_actions_environment_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_actions_environment_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_actions_organization_oidc_subject_claim_customization_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_actions_organization_public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_actions_organization_registration_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_actions_organization_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_actions_organization_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_actions_public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_actions_registration_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_actions_repository_oidc_subject_claim_customization_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_actions_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_actions_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_branch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_branch_protection_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_collaborators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_dependabot_organization_public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_dependabot_organization_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_dependabot_public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_dependabot_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_enterprise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_external_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_github_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    14508 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_ip_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_issue_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_membership.py
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_organization_ip_allow_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_organization_team_sync_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_organization_teams.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_organization_webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_release.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)    20628 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_repository_branches.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_repository_deploy_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_repository_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_repository_milestone.py
--rw-r--r--   0 runner    (1001) docker     (123)    11966 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_repository_pull_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_repository_pull_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_repository_teams.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_repository_webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_ssh_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    20918 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/issue.py
--rw-r--r--   0 runner    (1001) docker     (123)    13277 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/issue_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/membership.py
--rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/organization_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/organization_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/organization_security_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    79808 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/organization_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    15058 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/organization_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)   104294 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15743 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/project_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/project_column.py
--rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28755 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/release.py
--rw-r--r--   0 runner    (1001) docker     (123)   107291 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16391 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/repository_autolink_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    21061 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/repository_collaborator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/repository_collaborators.py
--rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/repository_deploy_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    17882 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/repository_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    27314 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/repository_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/repository_milestone.py
--rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/repository_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    28682 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/repository_pull_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/repository_tag_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    17190 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/repository_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    22399 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/team.py
--rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/team_members.py
--rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/team_membership.py
--rw-r--r--   0 runner    (1001) docker     (123)    15499 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/team_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/team_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10810 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/team_sync_group_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/user_gpg_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/user_invitation_accepter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github/user_ssh_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:12:33.662678 pulumi_github-5.9.0a1683752304/pulumi_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/pulumi_github.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 21:12:33.662678 pulumi_github-5.9.0a1683752304/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-10 21:12:33.000000 pulumi_github-5.9.0a1683752304/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:12:43.600196 pulumi_github-5.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-23 19:12:43.600196 pulumi_github-5.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:12:43.596196 pulumi_github-5.9.1/pulumi_github/
+-rw-r--r--   0 runner    (1001) docker     (123)    15525 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63272 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19178 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/actions_environment_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16013 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/actions_environment_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/actions_organization_oidc_subject_claim_customization_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20745 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/actions_organization_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22394 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/actions_organization_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/actions_organization_secret_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/actions_organization_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/actions_repository_access_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/actions_repository_oidc_subject_claim_customization_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16270 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/actions_repository_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25998 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/actions_runner_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15530 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/actions_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/actions_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/app_installation_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11169 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/app_installation_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16865 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/branch_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44058 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/branch_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31972 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/branch_protection_v3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:12:43.600196 pulumi_github-5.9.1/pulumi_github/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18662 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/dependabot_organization_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/dependabot_organization_secret_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/dependabot_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/emu_group_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14654 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/enterprise_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_actions_environment_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_actions_environment_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_actions_organization_oidc_subject_claim_customization_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_actions_organization_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_actions_organization_registration_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_actions_organization_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_actions_organization_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_actions_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_actions_registration_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_actions_repository_oidc_subject_claim_customization_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_actions_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_actions_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_branch_protection_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_collaborators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_dependabot_organization_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_dependabot_organization_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_dependabot_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_dependabot_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_external_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_github_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14508 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_ip_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_issue_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_organization_ip_allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_organization_team_sync_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_organization_teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_organization_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_release.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20628 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_repository_branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_repository_deploy_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_repository_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_repository_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11966 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_repository_pull_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_repository_pull_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_repository_teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_repository_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_ssh_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20918 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13277 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/issue_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/organization_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/organization_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/organization_security_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79808 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/organization_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15058 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/organization_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104474 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17035 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/project_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/project_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28755 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/release.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107291 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16391 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/repository_autolink_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21061 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/repository_collaborator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/repository_collaborators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14270 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/repository_deploy_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17882 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/repository_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27314 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/repository_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/repository_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/repository_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28682 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/repository_pull_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/repository_tag_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17190 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/repository_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22399 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/team_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13443 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/team_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15499 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/team_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/team_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/team_sync_group_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/user_gpg_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/user_invitation_accepter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github/user_ssh_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:12:43.600196 pulumi_github-5.9.1/pulumi_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/pulumi_github.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 19:12:43.600196 pulumi_github-5.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-23 19:12:43.000000 pulumi_github-5.9.1/setup.py
```

### Comparing `pulumi_github-5.9.0a1683752304/PKG-INFO` & `pulumi_github-5.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_github
-Version: 5.9.0a1683752304
+Version: 5.9.1
 Summary: A Pulumi package for creating and managing github cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-github
 Keywords: pulumi github
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_github-5.9.0a1683752304/README.md` & `pulumi_github-5.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/__init__.py` & `pulumi_github-5.9.1/pulumi_github/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/_inputs.py` & `pulumi_github-5.9.1/pulumi_github/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -580,14 +580,16 @@
 class BranchProtectionV3RestrictionsArgs:
     def __init__(__self__, *,
                  apps: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  teams: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  users: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[Sequence[pulumi.Input[str]]] apps: The list of app slugs with push access.
+               
+               `restrictions` is only available for organization-owned repositories.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] teams: The list of team slugs with push access.
                Always use `slug` of the team, **not** its name. Each team already **has** to have access to the repository.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] users: The list of user logins with push access.
         """
         if apps is not None:
             pulumi.set(__self__, "apps", apps)
         if teams is not None:
@@ -596,14 +598,16 @@
             pulumi.set(__self__, "users", users)
 
     @property
     @pulumi.getter
     def apps(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         The list of app slugs with push access.
+
+        `restrictions` is only available for organization-owned repositories.
         """
         return pulumi.get(self, "apps")
 
     @apps.setter
     def apps(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "apps", value)
```

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/_utilities.py` & `pulumi_github-5.9.1/pulumi_github/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/actions_environment_secret.py` & `pulumi_github-5.9.1/pulumi_github/actions_environment_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/actions_environment_variable.py` & `pulumi_github-5.9.1/pulumi_github/actions_environment_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/actions_organization_oidc_subject_claim_customization_template.py` & `pulumi_github-5.9.1/pulumi_github/actions_organization_oidc_subject_claim_customization_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/actions_organization_permissions.py` & `pulumi_github-5.9.1/pulumi_github/actions_organization_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/actions_organization_secret.py` & `pulumi_github-5.9.1/pulumi_github/actions_organization_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/actions_organization_secret_repositories.py` & `pulumi_github-5.9.1/pulumi_github/actions_organization_secret_repositories.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/actions_organization_variable.py` & `pulumi_github-5.9.1/pulumi_github/actions_organization_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/actions_repository_access_level.py` & `pulumi_github-5.9.1/pulumi_github/actions_repository_access_level.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/actions_repository_oidc_subject_claim_customization_template.py` & `pulumi_github-5.9.1/pulumi_github/actions_repository_oidc_subject_claim_customization_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/actions_repository_permissions.py` & `pulumi_github-5.9.1/pulumi_github/actions_repository_permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,15 @@
         ```
 
         ## Import
 
         This resource can be imported using the name of the GitHub repository
 
         ```sh
-         $ pulumi import github:index/actionsRepositoryPermissions:ActionsRepositoryPermissions test <github_repository_name>
+         $ pulumi import github:index/actionsRepositoryPermissions:ActionsRepositoryPermissions test my-repository
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] allowed_actions: The permissions policy that controls the actions that are allowed to run. Can be one of: `all`, `local_only`, or `selected`.
         :param pulumi.Input[pulumi.InputType['ActionsRepositoryPermissionsAllowedActionsConfigArgs']] allowed_actions_config: Sets the actions that are allowed in an repository. Only available when `allowed_actions` = `selected`. See Allowed Actions Config below for details.
         :param pulumi.Input[bool] enabled: Should GitHub actions be enabled on this repository?
@@ -236,15 +236,15 @@
         ```
 
         ## Import
 
         This resource can be imported using the name of the GitHub repository
 
         ```sh
-         $ pulumi import github:index/actionsRepositoryPermissions:ActionsRepositoryPermissions test <github_repository_name>
+         $ pulumi import github:index/actionsRepositoryPermissions:ActionsRepositoryPermissions test my-repository
         ```
 
         :param str resource_name: The name of the resource.
         :param ActionsRepositoryPermissionsArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/actions_runner_group.py` & `pulumi_github-5.9.1/pulumi_github/actions_runner_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/actions_secret.py` & `pulumi_github-5.9.1/pulumi_github/actions_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/actions_variable.py` & `pulumi_github-5.9.1/pulumi_github/actions_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/app_installation_repositories.py` & `pulumi_github-5.9.1/pulumi_github/app_installation_repository.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,226 +5,272 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['AppInstallationRepositoriesArgs', 'AppInstallationRepositories']
+__all__ = ['AppInstallationRepositoryArgs', 'AppInstallationRepository']
 
 @pulumi.input_type
-class AppInstallationRepositoriesArgs:
+class AppInstallationRepositoryArgs:
     def __init__(__self__, *,
                  installation_id: pulumi.Input[str],
-                 selected_repositories: pulumi.Input[Sequence[pulumi.Input[str]]]):
+                 repository: pulumi.Input[str]):
         """
-        The set of arguments for constructing a AppInstallationRepositories resource.
+        The set of arguments for constructing a AppInstallationRepository resource.
         :param pulumi.Input[str] installation_id: The GitHub app installation id.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] selected_repositories: A list of repository names to install the app on.
+        :param pulumi.Input[str] repository: The repository to install the app on.
         """
         pulumi.set(__self__, "installation_id", installation_id)
-        pulumi.set(__self__, "selected_repositories", selected_repositories)
+        pulumi.set(__self__, "repository", repository)
 
     @property
     @pulumi.getter(name="installationId")
     def installation_id(self) -> pulumi.Input[str]:
         """
         The GitHub app installation id.
         """
         return pulumi.get(self, "installation_id")
 
     @installation_id.setter
     def installation_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "installation_id", value)
 
     @property
-    @pulumi.getter(name="selectedRepositories")
-    def selected_repositories(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
+    @pulumi.getter
+    def repository(self) -> pulumi.Input[str]:
         """
-        A list of repository names to install the app on.
+        The repository to install the app on.
         """
-        return pulumi.get(self, "selected_repositories")
+        return pulumi.get(self, "repository")
 
-    @selected_repositories.setter
-    def selected_repositories(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        pulumi.set(self, "selected_repositories", value)
+    @repository.setter
+    def repository(self, value: pulumi.Input[str]):
+        pulumi.set(self, "repository", value)
 
 
 @pulumi.input_type
-class _AppInstallationRepositoriesState:
+class _AppInstallationRepositoryState:
     def __init__(__self__, *,
                  installation_id: Optional[pulumi.Input[str]] = None,
-                 selected_repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
+                 repo_id: Optional[pulumi.Input[int]] = None,
+                 repository: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering AppInstallationRepositories resources.
+        Input properties used for looking up and filtering AppInstallationRepository resources.
         :param pulumi.Input[str] installation_id: The GitHub app installation id.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] selected_repositories: A list of repository names to install the app on.
+        :param pulumi.Input[str] repository: The repository to install the app on.
         """
         if installation_id is not None:
             pulumi.set(__self__, "installation_id", installation_id)
-        if selected_repositories is not None:
-            pulumi.set(__self__, "selected_repositories", selected_repositories)
+        if repo_id is not None:
+            pulumi.set(__self__, "repo_id", repo_id)
+        if repository is not None:
+            pulumi.set(__self__, "repository", repository)
 
     @property
     @pulumi.getter(name="installationId")
     def installation_id(self) -> Optional[pulumi.Input[str]]:
         """
         The GitHub app installation id.
         """
         return pulumi.get(self, "installation_id")
 
     @installation_id.setter
     def installation_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "installation_id", value)
 
     @property
-    @pulumi.getter(name="selectedRepositories")
-    def selected_repositories(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter(name="repoId")
+    def repo_id(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "repo_id")
+
+    @repo_id.setter
+    def repo_id(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "repo_id", value)
+
+    @property
+    @pulumi.getter
+    def repository(self) -> Optional[pulumi.Input[str]]:
         """
-        A list of repository names to install the app on.
+        The repository to install the app on.
         """
-        return pulumi.get(self, "selected_repositories")
+        return pulumi.get(self, "repository")
 
-    @selected_repositories.setter
-    def selected_repositories(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "selected_repositories", value)
+    @repository.setter
+    def repository(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "repository", value)
 
 
-class AppInstallationRepositories(pulumi.CustomResource):
+class AppInstallationRepository(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  installation_id: Optional[pulumi.Input[str]] = None,
-                 selected_repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 repository: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         > **Note**: This resource is not compatible with the GitHub App Installation authentication method.
 
         This resource manages relationships between app installations and repositories
         in your GitHub organization.
 
-        Creating this resource installs a particular app on multiple repositories.
+        Creating this resource installs a particular app on a particular repository.
 
-        The app installation and the repositories must all belong to the same
+        The app installation and the repository must both belong to the same
         organization on GitHub. Note: you can review your organization's installations
         by the following the instructions at this
         [link](https://docs.github.com/en/github/setting-up-and-managing-organizations-and-teams/reviewing-your-organizations-installed-integrations).
 
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_github as github
+
+        # Create a repository.
+        some_repo = github.Repository("someRepo")
+        some_app_repo = github.AppInstallationRepository("someAppRepo",
+            installation_id="1234567",
+            repository=some_repo.name)
+        ```
+
         ## Import
 
-        GitHub App Installation Repositories can be imported using an ID made up of `installation_id`, e.g.
+        GitHub App Installation Repository can be imported using an ID made up of `installation_id:repository`, e.g.
 
         ```sh
-         $ pulumi import github:index/appInstallationRepositories:AppInstallationRepositories some_app_repos 1234567
+         $ pulumi import github:index/appInstallationRepository:AppInstallationRepository terraform_repo 1234567:terraform
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] installation_id: The GitHub app installation id.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] selected_repositories: A list of repository names to install the app on.
+        :param pulumi.Input[str] repository: The repository to install the app on.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: AppInstallationRepositoriesArgs,
+                 args: AppInstallationRepositoryArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         > **Note**: This resource is not compatible with the GitHub App Installation authentication method.
 
         This resource manages relationships between app installations and repositories
         in your GitHub organization.
 
-        Creating this resource installs a particular app on multiple repositories.
+        Creating this resource installs a particular app on a particular repository.
 
-        The app installation and the repositories must all belong to the same
+        The app installation and the repository must both belong to the same
         organization on GitHub. Note: you can review your organization's installations
         by the following the instructions at this
         [link](https://docs.github.com/en/github/setting-up-and-managing-organizations-and-teams/reviewing-your-organizations-installed-integrations).
 
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_github as github
+
+        # Create a repository.
+        some_repo = github.Repository("someRepo")
+        some_app_repo = github.AppInstallationRepository("someAppRepo",
+            installation_id="1234567",
+            repository=some_repo.name)
+        ```
+
         ## Import
 
-        GitHub App Installation Repositories can be imported using an ID made up of `installation_id`, e.g.
+        GitHub App Installation Repository can be imported using an ID made up of `installation_id:repository`, e.g.
 
         ```sh
-         $ pulumi import github:index/appInstallationRepositories:AppInstallationRepositories some_app_repos 1234567
+         $ pulumi import github:index/appInstallationRepository:AppInstallationRepository terraform_repo 1234567:terraform
         ```
 
         :param str resource_name: The name of the resource.
-        :param AppInstallationRepositoriesArgs args: The arguments to use to populate this resource's properties.
+        :param AppInstallationRepositoryArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(AppInstallationRepositoriesArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(AppInstallationRepositoryArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  installation_id: Optional[pulumi.Input[str]] = None,
-                 selected_repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 repository: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = AppInstallationRepositoriesArgs.__new__(AppInstallationRepositoriesArgs)
+            __props__ = AppInstallationRepositoryArgs.__new__(AppInstallationRepositoryArgs)
 
             if installation_id is None and not opts.urn:
                 raise TypeError("Missing required property 'installation_id'")
             __props__.__dict__["installation_id"] = installation_id
-            if selected_repositories is None and not opts.urn:
-                raise TypeError("Missing required property 'selected_repositories'")
-            __props__.__dict__["selected_repositories"] = selected_repositories
-        super(AppInstallationRepositories, __self__).__init__(
-            'github:index/appInstallationRepositories:AppInstallationRepositories',
+            if repository is None and not opts.urn:
+                raise TypeError("Missing required property 'repository'")
+            __props__.__dict__["repository"] = repository
+            __props__.__dict__["repo_id"] = None
+        super(AppInstallationRepository, __self__).__init__(
+            'github:index/appInstallationRepository:AppInstallationRepository',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             installation_id: Optional[pulumi.Input[str]] = None,
-            selected_repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'AppInstallationRepositories':
+            repo_id: Optional[pulumi.Input[int]] = None,
+            repository: Optional[pulumi.Input[str]] = None) -> 'AppInstallationRepository':
         """
-        Get an existing AppInstallationRepositories resource's state with the given name, id, and optional extra
+        Get an existing AppInstallationRepository resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] installation_id: The GitHub app installation id.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] selected_repositories: A list of repository names to install the app on.
+        :param pulumi.Input[str] repository: The repository to install the app on.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _AppInstallationRepositoriesState.__new__(_AppInstallationRepositoriesState)
+        __props__ = _AppInstallationRepositoryState.__new__(_AppInstallationRepositoryState)
 
         __props__.__dict__["installation_id"] = installation_id
-        __props__.__dict__["selected_repositories"] = selected_repositories
-        return AppInstallationRepositories(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["repo_id"] = repo_id
+        __props__.__dict__["repository"] = repository
+        return AppInstallationRepository(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="installationId")
     def installation_id(self) -> pulumi.Output[str]:
         """
         The GitHub app installation id.
         """
         return pulumi.get(self, "installation_id")
 
     @property
-    @pulumi.getter(name="selectedRepositories")
-    def selected_repositories(self) -> pulumi.Output[Sequence[str]]:
+    @pulumi.getter(name="repoId")
+    def repo_id(self) -> pulumi.Output[int]:
+        return pulumi.get(self, "repo_id")
+
+    @property
+    @pulumi.getter
+    def repository(self) -> pulumi.Output[str]:
         """
-        A list of repository names to install the app on.
+        The repository to install the app on.
         """
-        return pulumi.get(self, "selected_repositories")
+        return pulumi.get(self, "repository")
```

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/app_installation_repository.py` & `pulumi_github-5.9.1/pulumi_github/app_installation_repositories.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,272 +5,240 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['AppInstallationRepositoryArgs', 'AppInstallationRepository']
+__all__ = ['AppInstallationRepositoriesArgs', 'AppInstallationRepositories']
 
 @pulumi.input_type
-class AppInstallationRepositoryArgs:
+class AppInstallationRepositoriesArgs:
     def __init__(__self__, *,
                  installation_id: pulumi.Input[str],
-                 repository: pulumi.Input[str]):
+                 selected_repositories: pulumi.Input[Sequence[pulumi.Input[str]]]):
         """
-        The set of arguments for constructing a AppInstallationRepository resource.
+        The set of arguments for constructing a AppInstallationRepositories resource.
         :param pulumi.Input[str] installation_id: The GitHub app installation id.
-        :param pulumi.Input[str] repository: The repository to install the app on.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] selected_repositories: A list of repository names to install the app on.
+               
+               > **Note**: Due to how GitHub implements app installations, apps cannot be installed with no repositories selected. Therefore deleting this resource will leave one repository with the app installed. Manually uninstall the app or set the installation to all repositories via the GUI as after deleting this resource.
         """
         pulumi.set(__self__, "installation_id", installation_id)
-        pulumi.set(__self__, "repository", repository)
+        pulumi.set(__self__, "selected_repositories", selected_repositories)
 
     @property
     @pulumi.getter(name="installationId")
     def installation_id(self) -> pulumi.Input[str]:
         """
         The GitHub app installation id.
         """
         return pulumi.get(self, "installation_id")
 
     @installation_id.setter
     def installation_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "installation_id", value)
 
     @property
-    @pulumi.getter
-    def repository(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="selectedRepositories")
+    def selected_repositories(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        The repository to install the app on.
+        A list of repository names to install the app on.
+
+        > **Note**: Due to how GitHub implements app installations, apps cannot be installed with no repositories selected. Therefore deleting this resource will leave one repository with the app installed. Manually uninstall the app or set the installation to all repositories via the GUI as after deleting this resource.
         """
-        return pulumi.get(self, "repository")
+        return pulumi.get(self, "selected_repositories")
 
-    @repository.setter
-    def repository(self, value: pulumi.Input[str]):
-        pulumi.set(self, "repository", value)
+    @selected_repositories.setter
+    def selected_repositories(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(self, "selected_repositories", value)
 
 
 @pulumi.input_type
-class _AppInstallationRepositoryState:
+class _AppInstallationRepositoriesState:
     def __init__(__self__, *,
                  installation_id: Optional[pulumi.Input[str]] = None,
-                 repo_id: Optional[pulumi.Input[int]] = None,
-                 repository: Optional[pulumi.Input[str]] = None):
+                 selected_repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        Input properties used for looking up and filtering AppInstallationRepository resources.
+        Input properties used for looking up and filtering AppInstallationRepositories resources.
         :param pulumi.Input[str] installation_id: The GitHub app installation id.
-        :param pulumi.Input[str] repository: The repository to install the app on.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] selected_repositories: A list of repository names to install the app on.
+               
+               > **Note**: Due to how GitHub implements app installations, apps cannot be installed with no repositories selected. Therefore deleting this resource will leave one repository with the app installed. Manually uninstall the app or set the installation to all repositories via the GUI as after deleting this resource.
         """
         if installation_id is not None:
             pulumi.set(__self__, "installation_id", installation_id)
-        if repo_id is not None:
-            pulumi.set(__self__, "repo_id", repo_id)
-        if repository is not None:
-            pulumi.set(__self__, "repository", repository)
+        if selected_repositories is not None:
+            pulumi.set(__self__, "selected_repositories", selected_repositories)
 
     @property
     @pulumi.getter(name="installationId")
     def installation_id(self) -> Optional[pulumi.Input[str]]:
         """
         The GitHub app installation id.
         """
         return pulumi.get(self, "installation_id")
 
     @installation_id.setter
     def installation_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "installation_id", value)
 
     @property
-    @pulumi.getter(name="repoId")
-    def repo_id(self) -> Optional[pulumi.Input[int]]:
-        return pulumi.get(self, "repo_id")
-
-    @repo_id.setter
-    def repo_id(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "repo_id", value)
-
-    @property
-    @pulumi.getter
-    def repository(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="selectedRepositories")
+    def selected_repositories(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The repository to install the app on.
+        A list of repository names to install the app on.
+
+        > **Note**: Due to how GitHub implements app installations, apps cannot be installed with no repositories selected. Therefore deleting this resource will leave one repository with the app installed. Manually uninstall the app or set the installation to all repositories via the GUI as after deleting this resource.
         """
-        return pulumi.get(self, "repository")
+        return pulumi.get(self, "selected_repositories")
 
-    @repository.setter
-    def repository(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "repository", value)
+    @selected_repositories.setter
+    def selected_repositories(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "selected_repositories", value)
 
 
-class AppInstallationRepository(pulumi.CustomResource):
+class AppInstallationRepositories(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  installation_id: Optional[pulumi.Input[str]] = None,
-                 repository: Optional[pulumi.Input[str]] = None,
+                 selected_repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         > **Note**: This resource is not compatible with the GitHub App Installation authentication method.
 
         This resource manages relationships between app installations and repositories
         in your GitHub organization.
 
-        Creating this resource installs a particular app on a particular repository.
+        Creating this resource installs a particular app on multiple repositories.
 
-        The app installation and the repository must both belong to the same
+        The app installation and the repositories must all belong to the same
         organization on GitHub. Note: you can review your organization's installations
         by the following the instructions at this
         [link](https://docs.github.com/en/github/setting-up-and-managing-organizations-and-teams/reviewing-your-organizations-installed-integrations).
 
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import pulumi_github as github
-
-        # Create a repository.
-        some_repo = github.Repository("someRepo")
-        some_app_repo = github.AppInstallationRepository("someAppRepo",
-            installation_id="1234567",
-            repository=some_repo.name)
-        ```
-
         ## Import
 
-        GitHub App Installation Repository can be imported using an ID made up of `installation_id:repository`, e.g.
+        GitHub App Installation Repositories can be imported using an ID made up of `installation_id`, e.g.
 
         ```sh
-         $ pulumi import github:index/appInstallationRepository:AppInstallationRepository terraform_repo 1234567:terraform
+         $ pulumi import github:index/appInstallationRepositories:AppInstallationRepositories some_app_repos 1234567
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] installation_id: The GitHub app installation id.
-        :param pulumi.Input[str] repository: The repository to install the app on.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] selected_repositories: A list of repository names to install the app on.
+               
+               > **Note**: Due to how GitHub implements app installations, apps cannot be installed with no repositories selected. Therefore deleting this resource will leave one repository with the app installed. Manually uninstall the app or set the installation to all repositories via the GUI as after deleting this resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: AppInstallationRepositoryArgs,
+                 args: AppInstallationRepositoriesArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         > **Note**: This resource is not compatible with the GitHub App Installation authentication method.
 
         This resource manages relationships between app installations and repositories
         in your GitHub organization.
 
-        Creating this resource installs a particular app on a particular repository.
+        Creating this resource installs a particular app on multiple repositories.
 
-        The app installation and the repository must both belong to the same
+        The app installation and the repositories must all belong to the same
         organization on GitHub. Note: you can review your organization's installations
         by the following the instructions at this
         [link](https://docs.github.com/en/github/setting-up-and-managing-organizations-and-teams/reviewing-your-organizations-installed-integrations).
 
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import pulumi_github as github
-
-        # Create a repository.
-        some_repo = github.Repository("someRepo")
-        some_app_repo = github.AppInstallationRepository("someAppRepo",
-            installation_id="1234567",
-            repository=some_repo.name)
-        ```
-
         ## Import
 
-        GitHub App Installation Repository can be imported using an ID made up of `installation_id:repository`, e.g.
+        GitHub App Installation Repositories can be imported using an ID made up of `installation_id`, e.g.
 
         ```sh
-         $ pulumi import github:index/appInstallationRepository:AppInstallationRepository terraform_repo 1234567:terraform
+         $ pulumi import github:index/appInstallationRepositories:AppInstallationRepositories some_app_repos 1234567
         ```
 
         :param str resource_name: The name of the resource.
-        :param AppInstallationRepositoryArgs args: The arguments to use to populate this resource's properties.
+        :param AppInstallationRepositoriesArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(AppInstallationRepositoryArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(AppInstallationRepositoriesArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  installation_id: Optional[pulumi.Input[str]] = None,
-                 repository: Optional[pulumi.Input[str]] = None,
+                 selected_repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = AppInstallationRepositoryArgs.__new__(AppInstallationRepositoryArgs)
+            __props__ = AppInstallationRepositoriesArgs.__new__(AppInstallationRepositoriesArgs)
 
             if installation_id is None and not opts.urn:
                 raise TypeError("Missing required property 'installation_id'")
             __props__.__dict__["installation_id"] = installation_id
-            if repository is None and not opts.urn:
-                raise TypeError("Missing required property 'repository'")
-            __props__.__dict__["repository"] = repository
-            __props__.__dict__["repo_id"] = None
-        super(AppInstallationRepository, __self__).__init__(
-            'github:index/appInstallationRepository:AppInstallationRepository',
+            if selected_repositories is None and not opts.urn:
+                raise TypeError("Missing required property 'selected_repositories'")
+            __props__.__dict__["selected_repositories"] = selected_repositories
+        super(AppInstallationRepositories, __self__).__init__(
+            'github:index/appInstallationRepositories:AppInstallationRepositories',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             installation_id: Optional[pulumi.Input[str]] = None,
-            repo_id: Optional[pulumi.Input[int]] = None,
-            repository: Optional[pulumi.Input[str]] = None) -> 'AppInstallationRepository':
+            selected_repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'AppInstallationRepositories':
         """
-        Get an existing AppInstallationRepository resource's state with the given name, id, and optional extra
+        Get an existing AppInstallationRepositories resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] installation_id: The GitHub app installation id.
-        :param pulumi.Input[str] repository: The repository to install the app on.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] selected_repositories: A list of repository names to install the app on.
+               
+               > **Note**: Due to how GitHub implements app installations, apps cannot be installed with no repositories selected. Therefore deleting this resource will leave one repository with the app installed. Manually uninstall the app or set the installation to all repositories via the GUI as after deleting this resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _AppInstallationRepositoryState.__new__(_AppInstallationRepositoryState)
+        __props__ = _AppInstallationRepositoriesState.__new__(_AppInstallationRepositoriesState)
 
         __props__.__dict__["installation_id"] = installation_id
-        __props__.__dict__["repo_id"] = repo_id
-        __props__.__dict__["repository"] = repository
-        return AppInstallationRepository(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["selected_repositories"] = selected_repositories
+        return AppInstallationRepositories(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="installationId")
     def installation_id(self) -> pulumi.Output[str]:
         """
         The GitHub app installation id.
         """
         return pulumi.get(self, "installation_id")
 
     @property
-    @pulumi.getter(name="repoId")
-    def repo_id(self) -> pulumi.Output[int]:
-        return pulumi.get(self, "repo_id")
-
-    @property
-    @pulumi.getter
-    def repository(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="selectedRepositories")
+    def selected_repositories(self) -> pulumi.Output[Sequence[str]]:
         """
-        The repository to install the app on.
+        A list of repository names to install the app on.
+
+        > **Note**: Due to how GitHub implements app installations, apps cannot be installed with no repositories selected. Therefore deleting this resource will leave one repository with the app installed. Manually uninstall the app or set the installation to all repositories via the GUI as after deleting this resource.
         """
-        return pulumi.get(self, "repository")
+        return pulumi.get(self, "selected_repositories")
```

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/branch.py` & `pulumi_github-5.9.1/pulumi_github/branch.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/branch_default.py` & `pulumi_github-5.9.1/pulumi_github/branch_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/branch_protection.py` & `pulumi_github-5.9.1/pulumi_github/branch_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/branch_protection_v3.py` & `pulumi_github-5.9.1/pulumi_github/branch_protection_v3.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/config/outputs.py` & `pulumi_github-5.9.1/pulumi_github/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/config/vars.py` & `pulumi_github-5.9.1/pulumi_github/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/dependabot_organization_secret.py` & `pulumi_github-5.9.1/pulumi_github/dependabot_organization_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/dependabot_organization_secret_repositories.py` & `pulumi_github-5.9.1/pulumi_github/dependabot_organization_secret_repositories.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/dependabot_secret.py` & `pulumi_github-5.9.1/pulumi_github/dependabot_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/emu_group_mapping.py` & `pulumi_github-5.9.1/pulumi_github/emu_group_mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/enterprise_organization.py` & `pulumi_github-5.9.1/pulumi_github/enterprise_organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_actions_environment_secrets.py` & `pulumi_github-5.9.1/pulumi_github/get_actions_environment_secrets.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_actions_environment_variables.py` & `pulumi_github-5.9.1/pulumi_github/get_actions_environment_variables.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_actions_organization_oidc_subject_claim_customization_template.py` & `pulumi_github-5.9.1/pulumi_github/get_actions_organization_oidc_subject_claim_customization_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_actions_organization_public_key.py` & `pulumi_github-5.9.1/pulumi_github/get_actions_organization_public_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_actions_organization_registration_token.py` & `pulumi_github-5.9.1/pulumi_github/get_actions_organization_registration_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_actions_organization_secrets.py` & `pulumi_github-5.9.1/pulumi_github/get_actions_organization_secrets.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_actions_organization_variables.py` & `pulumi_github-5.9.1/pulumi_github/get_actions_organization_variables.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_actions_public_key.py` & `pulumi_github-5.9.1/pulumi_github/get_actions_public_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_actions_registration_token.py` & `pulumi_github-5.9.1/pulumi_github/get_actions_registration_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_actions_repository_oidc_subject_claim_customization_template.py` & `pulumi_github-5.9.1/pulumi_github/get_actions_repository_oidc_subject_claim_customization_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_actions_secrets.py` & `pulumi_github-5.9.1/pulumi_github/get_actions_secrets.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_actions_variables.py` & `pulumi_github-5.9.1/pulumi_github/get_actions_variables.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_branch.py` & `pulumi_github-5.9.1/pulumi_github/get_branch.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_branch_protection_rules.py` & `pulumi_github-5.9.1/pulumi_github/get_branch_protection_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_collaborators.py` & `pulumi_github-5.9.1/pulumi_github/get_collaborators.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_dependabot_organization_public_key.py` & `pulumi_github-5.9.1/pulumi_github/get_dependabot_organization_public_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_dependabot_organization_secrets.py` & `pulumi_github-5.9.1/pulumi_github/get_dependabot_organization_secrets.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_dependabot_public_key.py` & `pulumi_github-5.9.1/pulumi_github/get_dependabot_public_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_dependabot_secrets.py` & `pulumi_github-5.9.1/pulumi_github/get_dependabot_secrets.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_enterprise.py` & `pulumi_github-5.9.1/pulumi_github/get_enterprise.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_external_groups.py` & `pulumi_github-5.9.1/pulumi_github/get_external_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_github_app.py` & `pulumi_github-5.9.1/pulumi_github/get_github_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_ip_ranges.py` & `pulumi_github-5.9.1/pulumi_github/get_ip_ranges.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_issue_labels.py` & `pulumi_github-5.9.1/pulumi_github/get_issue_labels.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_membership.py` & `pulumi_github-5.9.1/pulumi_github/get_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_organization.py` & `pulumi_github-5.9.1/pulumi_github/get_organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_organization_ip_allow_list.py` & `pulumi_github-5.9.1/pulumi_github/get_organization_ip_allow_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_organization_team_sync_groups.py` & `pulumi_github-5.9.1/pulumi_github/get_organization_team_sync_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_organization_teams.py` & `pulumi_github-5.9.1/pulumi_github/get_organization_teams.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_organization_webhooks.py` & `pulumi_github-5.9.1/pulumi_github/get_organization_webhooks.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_ref.py` & `pulumi_github-5.9.1/pulumi_github/get_ref.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_release.py` & `pulumi_github-5.9.1/pulumi_github/get_release.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_repositories.py` & `pulumi_github-5.9.1/pulumi_github/get_repositories.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_repository.py` & `pulumi_github-5.9.1/pulumi_github/get_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_repository_branches.py` & `pulumi_github-5.9.1/pulumi_github/get_repository_branches.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_repository_deploy_keys.py` & `pulumi_github-5.9.1/pulumi_github/get_repository_deploy_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_repository_file.py` & `pulumi_github-5.9.1/pulumi_github/get_repository_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -165,15 +165,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_github as github
 
-    foo = github.get_repository_file(repository=github_repository["foo"]["name"],
+    foo = github.get_repository_file(repository=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         branch="main",
         file=".gitignore")
     ```
 
 
     :param str branch: Git branch. Defaults to the repository's default branch.
     :param str file: The path of the file to read.
@@ -211,15 +211,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_github as github
 
-    foo = github.get_repository_file(repository=github_repository["foo"]["name"],
+    foo = github.get_repository_file(repository=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         branch="main",
         file=".gitignore")
     ```
 
 
     :param str branch: Git branch. Defaults to the repository's default branch.
     :param str file: The path of the file to read.
```

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_repository_milestone.py` & `pulumi_github-5.9.1/pulumi_github/get_repository_milestone.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_repository_pull_request.py` & `pulumi_github-5.9.1/pulumi_github/get_repository_pull_request.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_repository_pull_requests.py` & `pulumi_github-5.9.1/pulumi_github/get_repository_pull_requests.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_repository_teams.py` & `pulumi_github-5.9.1/pulumi_github/get_repository_teams.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_repository_webhooks.py` & `pulumi_github-5.9.1/pulumi_github/get_repository_webhooks.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_ssh_keys.py` & `pulumi_github-5.9.1/pulumi_github/get_ssh_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_team.py` & `pulumi_github-5.9.1/pulumi_github/get_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_tree.py` & `pulumi_github-5.9.1/pulumi_github/get_tree.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_user.py` & `pulumi_github-5.9.1/pulumi_github/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/get_users.py` & `pulumi_github-5.9.1/pulumi_github/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/issue.py` & `pulumi_github-5.9.1/pulumi_github/issue.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/issue_label.py` & `pulumi_github-5.9.1/pulumi_github/issue_label.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/membership.py` & `pulumi_github-5.9.1/pulumi_github/membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/organization_block.py` & `pulumi_github-5.9.1/pulumi_github/organization_block.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/organization_project.py` & `pulumi_github-5.9.1/pulumi_github/organization_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/organization_security_manager.py` & `pulumi_github-5.9.1/pulumi_github/organization_security_manager.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/organization_settings.py` & `pulumi_github-5.9.1/pulumi_github/organization_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/organization_webhook.py` & `pulumi_github-5.9.1/pulumi_github/organization_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/outputs.py` & `pulumi_github-5.9.1/pulumi_github/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -611,14 +611,16 @@
 class BranchProtectionV3Restrictions(dict):
     def __init__(__self__, *,
                  apps: Optional[Sequence[str]] = None,
                  teams: Optional[Sequence[str]] = None,
                  users: Optional[Sequence[str]] = None):
         """
         :param Sequence[str] apps: The list of app slugs with push access.
+               
+               `restrictions` is only available for organization-owned repositories.
         :param Sequence[str] teams: The list of team slugs with push access.
                Always use `slug` of the team, **not** its name. Each team already **has** to have access to the repository.
         :param Sequence[str] users: The list of user logins with push access.
         """
         if apps is not None:
             pulumi.set(__self__, "apps", apps)
         if teams is not None:
@@ -627,14 +629,16 @@
             pulumi.set(__self__, "users", users)
 
     @property
     @pulumi.getter
     def apps(self) -> Optional[Sequence[str]]:
         """
         The list of app slugs with push access.
+
+        `restrictions` is only available for organization-owned repositories.
         """
         return pulumi.get(self, "apps")
 
     @property
     @pulumi.getter
     def teams(self) -> Optional[Sequence[str]]:
         """
```

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/project_card.py` & `pulumi_github-5.9.1/pulumi_github/project_card.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,17 @@
                  content_type: Optional[pulumi.Input[str]] = None,
                  note: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a ProjectCard resource.
         :param pulumi.Input[str] column_id: The ID of the card.
         :param pulumi.Input[int] content_id: `github_issue.issue_id`.
         :param pulumi.Input[str] content_type: Must be either `Issue` or `PullRequest`
+               
+               **Remarks:** You must either set the `note` attribute or both `content_id` and `content_type`.
+               See note example or issue example for more information.
         :param pulumi.Input[str] note: The note contents of the card. Markdown supported.
         """
         pulumi.set(__self__, "column_id", column_id)
         if content_id is not None:
             pulumi.set(__self__, "content_id", content_id)
         if content_type is not None:
             pulumi.set(__self__, "content_type", content_type)
@@ -58,14 +61,17 @@
         pulumi.set(self, "content_id", value)
 
     @property
     @pulumi.getter(name="contentType")
     def content_type(self) -> Optional[pulumi.Input[str]]:
         """
         Must be either `Issue` or `PullRequest`
+
+        **Remarks:** You must either set the `note` attribute or both `content_id` and `content_type`.
+        See note example or issue example for more information.
         """
         return pulumi.get(self, "content_type")
 
     @content_type.setter
     def content_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "content_type", value)
 
@@ -93,14 +99,17 @@
                  note: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering ProjectCard resources.
         :param pulumi.Input[int] card_id: The ID of the card.
         :param pulumi.Input[str] column_id: The ID of the card.
         :param pulumi.Input[int] content_id: `github_issue.issue_id`.
         :param pulumi.Input[str] content_type: Must be either `Issue` or `PullRequest`
+               
+               **Remarks:** You must either set the `note` attribute or both `content_id` and `content_type`.
+               See note example or issue example for more information.
         :param pulumi.Input[str] note: The note contents of the card. Markdown supported.
         """
         if card_id is not None:
             pulumi.set(__self__, "card_id", card_id)
         if column_id is not None:
             pulumi.set(__self__, "column_id", column_id)
         if content_id is not None:
@@ -149,14 +158,17 @@
         pulumi.set(self, "content_id", value)
 
     @property
     @pulumi.getter(name="contentType")
     def content_type(self) -> Optional[pulumi.Input[str]]:
         """
         Must be either `Issue` or `PullRequest`
+
+        **Remarks:** You must either set the `note` attribute or both `content_id` and `content_type`.
+        See note example or issue example for more information.
         """
         return pulumi.get(self, "content_type")
 
     @content_type.setter
     def content_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "content_type", value)
 
@@ -239,14 +251,17 @@
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] column_id: The ID of the card.
         :param pulumi.Input[int] content_id: `github_issue.issue_id`.
         :param pulumi.Input[str] content_type: Must be either `Issue` or `PullRequest`
+               
+               **Remarks:** You must either set the `note` attribute or both `content_id` and `content_type`.
+               See note example or issue example for more information.
         :param pulumi.Input[str] note: The note contents of the card. Markdown supported.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ProjectCardArgs,
@@ -356,14 +371,17 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] card_id: The ID of the card.
         :param pulumi.Input[str] column_id: The ID of the card.
         :param pulumi.Input[int] content_id: `github_issue.issue_id`.
         :param pulumi.Input[str] content_type: Must be either `Issue` or `PullRequest`
+               
+               **Remarks:** You must either set the `note` attribute or both `content_id` and `content_type`.
+               See note example or issue example for more information.
         :param pulumi.Input[str] note: The note contents of the card. Markdown supported.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ProjectCardState.__new__(_ProjectCardState)
 
         __props__.__dict__["card_id"] = card_id
@@ -399,14 +417,17 @@
         return pulumi.get(self, "content_id")
 
     @property
     @pulumi.getter(name="contentType")
     def content_type(self) -> pulumi.Output[Optional[str]]:
         """
         Must be either `Issue` or `PullRequest`
+
+        **Remarks:** You must either set the `note` attribute or both `content_id` and `content_type`.
+        See note example or issue example for more information.
         """
         return pulumi.get(self, "content_type")
 
     @property
     @pulumi.getter
     def etag(self) -> pulumi.Output[str]:
         return pulumi.get(self, "etag")
```

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/project_column.py` & `pulumi_github-5.9.1/pulumi_github/project_column.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/provider.py` & `pulumi_github-5.9.1/pulumi_github/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/release.py` & `pulumi_github-5.9.1/pulumi_github/release.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/repository.py` & `pulumi_github-5.9.1/pulumi_github/repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/repository_autolink_reference.py` & `pulumi_github-5.9.1/pulumi_github/repository_autolink_reference.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/repository_collaborator.py` & `pulumi_github-5.9.1/pulumi_github/repository_collaborator.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/repository_collaborators.py` & `pulumi_github-5.9.1/pulumi_github/repository_collaborators.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/repository_deploy_key.py` & `pulumi_github-5.9.1/pulumi_github/repository_deploy_key.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,16 @@
                  title: pulumi.Input[str],
                  read_only: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a RepositoryDeployKey resource.
         :param pulumi.Input[str] key: A SSH key.
         :param pulumi.Input[str] repository: Name of the GitHub repository.
         :param pulumi.Input[str] title: A title.
+               
+               Changing any of the fields forces re-creating the resource.
         :param pulumi.Input[bool] read_only: A boolean qualifying the key to be either read only or read/write.
         """
         pulumi.set(__self__, "key", key)
         pulumi.set(__self__, "repository", repository)
         pulumi.set(__self__, "title", title)
         if read_only is not None:
             pulumi.set(__self__, "read_only", read_only)
@@ -56,14 +58,16 @@
         pulumi.set(self, "repository", value)
 
     @property
     @pulumi.getter
     def title(self) -> pulumi.Input[str]:
         """
         A title.
+
+        Changing any of the fields forces re-creating the resource.
         """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: pulumi.Input[str]):
         pulumi.set(self, "title", value)
 
@@ -90,14 +94,16 @@
                  title: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering RepositoryDeployKey resources.
         :param pulumi.Input[str] key: A SSH key.
         :param pulumi.Input[bool] read_only: A boolean qualifying the key to be either read only or read/write.
         :param pulumi.Input[str] repository: Name of the GitHub repository.
         :param pulumi.Input[str] title: A title.
+               
+               Changing any of the fields forces re-creating the resource.
         """
         if etag is not None:
             pulumi.set(__self__, "etag", etag)
         if key is not None:
             pulumi.set(__self__, "key", key)
         if read_only is not None:
             pulumi.set(__self__, "read_only", read_only)
@@ -152,14 +158,16 @@
         pulumi.set(self, "repository", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
         """
         A title.
+
+        Changing any of the fields forces re-creating the resource.
         """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
@@ -210,14 +218,16 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] key: A SSH key.
         :param pulumi.Input[bool] read_only: A boolean qualifying the key to be either read only or read/write.
         :param pulumi.Input[str] repository: Name of the GitHub repository.
         :param pulumi.Input[str] title: A title.
+               
+               Changing any of the fields forces re-creating the resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: RepositoryDeployKeyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -316,14 +326,16 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] key: A SSH key.
         :param pulumi.Input[bool] read_only: A boolean qualifying the key to be either read only or read/write.
         :param pulumi.Input[str] repository: Name of the GitHub repository.
         :param pulumi.Input[str] title: A title.
+               
+               Changing any of the fields forces re-creating the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _RepositoryDeployKeyState.__new__(_RepositoryDeployKeyState)
 
         __props__.__dict__["etag"] = etag
         __props__.__dict__["key"] = key
@@ -362,10 +374,12 @@
         return pulumi.get(self, "repository")
 
     @property
     @pulumi.getter
     def title(self) -> pulumi.Output[str]:
         """
         A title.
+
+        Changing any of the fields forces re-creating the resource.
         """
         return pulumi.get(self, "title")
```

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/repository_environment.py` & `pulumi_github-5.9.1/pulumi_github/repository_environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/repository_file.py` & `pulumi_github-5.9.1/pulumi_github/repository_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/repository_milestone.py` & `pulumi_github-5.9.1/pulumi_github/repository_milestone.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/repository_project.py` & `pulumi_github-5.9.1/pulumi_github/repository_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/repository_pull_request.py` & `pulumi_github-5.9.1/pulumi_github/repository_pull_request.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/repository_tag_protection.py` & `pulumi_github-5.9.1/pulumi_github/repository_tag_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/repository_webhook.py` & `pulumi_github-5.9.1/pulumi_github/repository_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/team.py` & `pulumi_github-5.9.1/pulumi_github/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/team_members.py` & `pulumi_github-5.9.1/pulumi_github/team_members.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/team_membership.py` & `pulumi_github-5.9.1/pulumi_github/team_membership.py`

 * *Files 11% similar despite different names*

```diff
@@ -143,14 +143,25 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  role: Optional[pulumi.Input[str]] = None,
                  team_id: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
+        Provides a GitHub team membership resource.
+
+        This resource allows you to add/remove users from teams in your organization. When applied,
+        the user will be added to the team. If the user hasn't accepted their invitation to the
+        organization, they won't be part of the team until they do. When
+        destroyed, the user will be removed from the team.
+
+        > **Note** This resource is not compatible with `TeamMembers`. Use either `TeamMembers` or `TeamMembership`.
+
+        > **Note** Organization owners may not be set as "members" of a team; they may only be set as "maintainers". Attempting to set organization an owner to "member" of a may result in a `pulumi preview` diff that changes their status back to "maintainer".
+
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_github as github
 
         # Add a user to the organization
@@ -186,14 +197,25 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: TeamMembershipArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        Provides a GitHub team membership resource.
+
+        This resource allows you to add/remove users from teams in your organization. When applied,
+        the user will be added to the team. If the user hasn't accepted their invitation to the
+        organization, they won't be part of the team until they do. When
+        destroyed, the user will be removed from the team.
+
+        > **Note** This resource is not compatible with `TeamMembers`. Use either `TeamMembers` or `TeamMembership`.
+
+        > **Note** Organization owners may not be set as "members" of a team; they may only be set as "maintainers". Attempting to set organization an owner to "member" of a may result in a `pulumi preview` diff that changes their status back to "maintainer".
+
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_github as github
 
         # Add a user to the organization
```

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/team_repository.py` & `pulumi_github-5.9.1/pulumi_github/team_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/team_settings.py` & `pulumi_github-5.9.1/pulumi_github/team_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/team_sync_group_mapping.py` & `pulumi_github-5.9.1/pulumi_github/team_sync_group_mapping.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,16 @@
                  team_slug: pulumi.Input[str],
                  groups: Optional[pulumi.Input[Sequence[pulumi.Input['TeamSyncGroupMappingGroupArgs']]]] = None):
         """
         The set of arguments for constructing a TeamSyncGroupMapping resource.
         :param pulumi.Input[str] team_slug: Slug of the team
         :param pulumi.Input[Sequence[pulumi.Input['TeamSyncGroupMappingGroupArgs']]] groups: An Array of GitHub Identity Provider Groups (or empty []).  Each `group` block consists of the fields documented below.
                ___
+               
+               The `group` block consists of:
         """
         pulumi.set(__self__, "team_slug", team_slug)
         if groups is not None:
             pulumi.set(__self__, "groups", groups)
 
     @property
     @pulumi.getter(name="teamSlug")
@@ -42,14 +44,16 @@
 
     @property
     @pulumi.getter
     def groups(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['TeamSyncGroupMappingGroupArgs']]]]:
         """
         An Array of GitHub Identity Provider Groups (or empty []).  Each `group` block consists of the fields documented below.
         ___
+
+        The `group` block consists of:
         """
         return pulumi.get(self, "groups")
 
     @groups.setter
     def groups(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['TeamSyncGroupMappingGroupArgs']]]]):
         pulumi.set(self, "groups", value)
 
@@ -60,14 +64,16 @@
                  etag: Optional[pulumi.Input[str]] = None,
                  groups: Optional[pulumi.Input[Sequence[pulumi.Input['TeamSyncGroupMappingGroupArgs']]]] = None,
                  team_slug: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering TeamSyncGroupMapping resources.
         :param pulumi.Input[Sequence[pulumi.Input['TeamSyncGroupMappingGroupArgs']]] groups: An Array of GitHub Identity Provider Groups (or empty []).  Each `group` block consists of the fields documented below.
                ___
+               
+               The `group` block consists of:
         :param pulumi.Input[str] team_slug: Slug of the team
         """
         if etag is not None:
             pulumi.set(__self__, "etag", etag)
         if groups is not None:
             pulumi.set(__self__, "groups", groups)
         if team_slug is not None:
@@ -84,14 +90,16 @@
 
     @property
     @pulumi.getter
     def groups(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['TeamSyncGroupMappingGroupArgs']]]]:
         """
         An Array of GitHub Identity Provider Groups (or empty []).  Each `group` block consists of the fields documented below.
         ___
+
+        The `group` block consists of:
         """
         return pulumi.get(self, "groups")
 
     @groups.setter
     def groups(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['TeamSyncGroupMappingGroupArgs']]]]):
         pulumi.set(self, "groups", value)
 
@@ -131,14 +139,16 @@
          $ pulumi import github:index/teamSyncGroupMapping:TeamSyncGroupMapping example some_team
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TeamSyncGroupMappingGroupArgs']]]] groups: An Array of GitHub Identity Provider Groups (or empty []).  Each `group` block consists of the fields documented below.
                ___
+               
+               The `group` block consists of:
         :param pulumi.Input[str] team_slug: Slug of the team
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: TeamSyncGroupMappingArgs,
@@ -207,14 +217,16 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TeamSyncGroupMappingGroupArgs']]]] groups: An Array of GitHub Identity Provider Groups (or empty []).  Each `group` block consists of the fields documented below.
                ___
+               
+               The `group` block consists of:
         :param pulumi.Input[str] team_slug: Slug of the team
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _TeamSyncGroupMappingState.__new__(_TeamSyncGroupMappingState)
 
         __props__.__dict__["etag"] = etag
@@ -229,14 +241,16 @@
 
     @property
     @pulumi.getter
     def groups(self) -> pulumi.Output[Optional[Sequence['outputs.TeamSyncGroupMappingGroup']]]:
         """
         An Array of GitHub Identity Provider Groups (or empty []).  Each `group` block consists of the fields documented below.
         ___
+
+        The `group` block consists of:
         """
         return pulumi.get(self, "groups")
 
     @property
     @pulumi.getter(name="teamSlug")
     def team_slug(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/user_gpg_key.py` & `pulumi_github-5.9.1/pulumi_github/user_gpg_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/user_invitation_accepter.py` & `pulumi_github-5.9.1/pulumi_github/user_invitation_accepter.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github/user_ssh_key.py` & `pulumi_github-5.9.1/pulumi_github/user_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github.egg-info/PKG-INFO` & `pulumi_github-5.9.1/pulumi_github.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-github
-Version: 5.9.0a1683752304
+Version: 5.9.1
 Summary: A Pulumi package for creating and managing github cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-github
 Keywords: pulumi github
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_github-5.9.0a1683752304/pulumi_github.egg-info/SOURCES.txt` & `pulumi_github-5.9.1/pulumi_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.9.0a1683752304/setup.py` & `pulumi_github-5.9.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "5.9.0a1683752304"
-PLUGIN_VERSION = "5.9.0-alpha.1683752304+c5de6232"
+VERSION = "5.9.1"
+PLUGIN_VERSION = "5.9.1"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'github', PLUGIN_VERSION])
         except OSError as error:
```

