# Comparing `tmp/pulumi_cloudflare-5.4.0a1686761772.tar.gz` & `tmp/pulumi_cloudflare-5.5.0a1687050407.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_cloudflare-5.4.0a1686761772.tar", last modified: Wed Jun 14 17:01:15 2023, max compression
+gzip compressed data, was "pulumi_cloudflare-5.5.0a1687050407.tar", last modified: Sun Jun 18 01:12:18 2023, max compression
```

## Comparing `pulumi_cloudflare-5.4.0a1686761772.tar` & `pulumi_cloudflare-5.5.0a1687050407.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:01:15.079697 pulumi_cloudflare-5.4.0a1686761772/
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-06-14 17:01:15.079697 pulumi_cloudflare-5.4.0a1686761772/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:01:15.075697 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/
--rw-r--r--   0 runner    (1001) docker     (123)    22080 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   657682 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    58529 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/access_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    15370 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/access_ca_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    19346 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/access_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    25010 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/access_identity_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/access_keys_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    18013 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/access_mutual_tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    27944 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/access_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)    40874 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/access_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    21362 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/access_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/access_service_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/account.py
--rw-r--r--   0 runner    (1001) docker     (123)    13959 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/account_member.py
--rw-r--r--   0 runner    (1001) docker     (123)    22238 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/address_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    10574 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/api_shield.py
--rw-r--r--   0 runner    (1001) docker     (123)    18820 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/api_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/argo.py
--rw-r--r--   0 runner    (1001) docker     (123)    19083 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/authenticated_origin_pulls.py
--rw-r--r--   0 runner    (1001) docker     (123)    23674 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/authenticated_origin_pulls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/byo_ip_prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)    34746 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/certificate_pack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:01:15.079697 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    26966 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/custom_hostname.py
--rw-r--r--   0 runner    (1001) docker     (123)    10680 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/custom_hostname_fallback_origin.py
--rw-r--r--   0 runner    (1001) docker     (123)    15849 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/custom_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)    18178 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/custom_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    19675 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/device_dex_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13906 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/device_managed_networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/device_policy_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)    18270 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/device_posture_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    23563 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/device_posture_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    45257 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/device_settings_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/dlp_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/email_routing_address.py
--rw-r--r--   0 runner    (1001) docker     (123)    16326 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/email_routing_catch_all.py
--rw-r--r--   0 runner    (1001) docker     (123)    17902 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/email_routing_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    16142 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/email_routing_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/fallback_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    14429 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    22222 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/firewall_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_access_identity_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_account_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_api_token_permission_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_ip_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_load_balancer_pools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_origin_ca_root_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_rulesets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_zone.py
--rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_zone_dnssec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_zones.py
--rw-r--r--   0 runner    (1001) docker     (123)    29551 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/gre_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (123)    58563 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)    39524 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/ipsec_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (123)    13818 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    25280 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/list_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    80329 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)    42775 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/load_balancer_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    44865 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/load_balancer_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/logpull_retention.py
--rw-r--r--   0 runner    (1001) docker     (123)    42980 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/logpush_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    15765 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/logpush_ownership_challenge.py
--rw-r--r--   0 runner    (1001) docker     (123)    13974 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/magic_firewall_ruleset.py
--rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/managed_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)    23044 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/mtls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    43274 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/notification_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18763 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/notification_policy_webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    22053 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/origin_ca_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)   642232 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16229 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/page_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    12872 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/pages_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    31800 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/pages_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    22414 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/r2_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    29718 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/rate_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)    36107 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/record.py
--rw-r--r--   0 runner    (1001) docker     (123)    12793 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/regional_hostname.py
--rw-r--r--   0 runner    (1001) docker     (123)    25856 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/ruleset.py
--rw-r--r--   0 runner    (1001) docker     (123)    36939 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/spectrum_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/split_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (123)    21981 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/static_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    30020 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/teams_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    14549 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/teams_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    19086 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/teams_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/teams_proxy_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    28926 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/teams_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/tiered_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    11257 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/total_tls.py
--rw-r--r--   0 runner    (1001) docker     (123)    19389 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/tunnel.py
--rw-r--r--   0 runner    (1001) docker     (123)    16091 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/tunnel_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18141 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/tunnel_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/tunnel_virtual_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    20232 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/turnstile_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/url_normalization_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/user_agent_blocking_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    40753 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/waiting_room.py
--rw-r--r--   0 runner    (1001) docker     (123)    45501 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/waiting_room_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/waiting_room_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/waiting_room_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    15822 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/web3_hostname.py
--rw-r--r--   0 runner    (1001) docker     (123)    12221 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/worker_cron_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)    14968 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/worker_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/worker_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    40108 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/worker_script.py
--rw-r--r--   0 runner    (1001) docker     (123)    13379 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/workers_kv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/workers_kv_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    25022 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/zone.py
--rw-r--r--   0 runner    (1001) docker     (123)    34471 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/zone_cache_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)    18510 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/zone_dnssec.py
--rw-r--r--   0 runner    (1001) docker     (123)    19581 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/zone_lockdown.py
--rw-r--r--   0 runner    (1001) docker     (123)    15003 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/zone_settings_override.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:01:15.079697 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 17:01:15.079697 pulumi_cloudflare-5.4.0a1686761772/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-14 17:01:14.000000 pulumi_cloudflare-5.4.0a1686761772/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:12:18.447856 pulumi_cloudflare-5.5.0a1687050407/
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-06-18 01:12:18.447856 pulumi_cloudflare-5.5.0a1687050407/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:12:18.447856 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/
+-rw-r--r--   0 runner    (1001) docker     (123)    22080 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   657682 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58529 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/access_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15370 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/access_ca_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19346 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/access_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25010 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/access_identity_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/access_keys_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18013 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/access_mutual_tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27944 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/access_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40874 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/access_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21362 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/access_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/access_service_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13959 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/account_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22238 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/address_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10574 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/api_shield.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18820 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/api_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/argo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19083 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/authenticated_origin_pulls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23674 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/authenticated_origin_pulls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/byo_ip_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34746 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/certificate_pack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:12:18.447856 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26966 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/custom_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10680 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/custom_hostname_fallback_origin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15849 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/custom_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18178 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/custom_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19675 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/device_dex_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13906 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/device_managed_networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/device_policy_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18270 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/device_posture_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23563 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/device_posture_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45257 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/device_settings_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/dlp_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/email_routing_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16326 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/email_routing_catch_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17902 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/email_routing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16142 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/email_routing_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/fallback_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14429 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22222 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/firewall_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_access_identity_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_account_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_api_token_permission_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_ip_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_load_balancer_pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_origin_ca_root_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_rulesets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_zone_dnssec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_zones.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29551 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/gre_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58563 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39524 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/ipsec_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13818 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25280 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80329 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42775 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/load_balancer_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44865 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/load_balancer_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/logpull_retention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42980 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/logpush_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15765 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/logpush_ownership_challenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13974 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/magic_firewall_ruleset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/managed_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23044 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/mtls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43274 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/notification_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18763 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/notification_policy_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22053 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/origin_ca_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)   642232 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16229 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/page_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12872 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/pages_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31800 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/pages_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22414 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/r2_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29718 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/rate_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36107 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12793 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/regional_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25856 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/ruleset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36939 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/spectrum_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/split_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21981 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/static_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30020 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/teams_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14549 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/teams_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19086 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/teams_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/teams_proxy_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28926 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/teams_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/tiered_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11257 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/total_tls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19389 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16091 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/tunnel_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18141 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/tunnel_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/tunnel_virtual_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20232 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/turnstile_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/url_normalization_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/user_agent_blocking_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40753 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/waiting_room.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45501 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/waiting_room_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/waiting_room_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/waiting_room_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15822 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/web3_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12221 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/worker_cron_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14968 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/worker_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/worker_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40108 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/worker_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13379 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/workers_kv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/workers_kv_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25022 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34471 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/zone_cache_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18510 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/zone_dnssec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19581 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/zone_lockdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15003 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/zone_settings_override.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:12:18.447856 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 01:12:18.447856 pulumi_cloudflare-5.5.0a1687050407/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-18 01:12:18.000000 pulumi_cloudflare-5.5.0a1687050407/setup.py
```

### Comparing `pulumi_cloudflare-5.4.0a1686761772/PKG-INFO` & `pulumi_cloudflare-5.5.0a1687050407/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_cloudflare
-Version: 5.4.0a1686761772
+Version: 5.5.0a1687050407
 Summary: A Pulumi package for creating and managing Cloudflare cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-cloudflare
 Keywords: pulumi cloudflare
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_cloudflare-5.4.0a1686761772/README.md` & `pulumi_cloudflare-5.5.0a1687050407/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/__init__.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/_inputs.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/_utilities.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/access_application.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/access_application.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/access_ca_certificate.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/access_ca_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/access_group.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/access_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/access_identity_provider.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/access_identity_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/access_keys_configuration.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/access_keys_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/access_mutual_tls_certificate.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/access_mutual_tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/access_organization.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/access_organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/access_policy.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/access_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/access_rule.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/access_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/access_service_token.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/access_service_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/account.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/account.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/account_member.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/account_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/address_map.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/address_map.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/api_shield.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/api_shield.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/api_token.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/api_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/argo.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/argo.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/authenticated_origin_pulls.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/authenticated_origin_pulls.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/authenticated_origin_pulls_certificate.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/authenticated_origin_pulls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/byo_ip_prefix.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/byo_ip_prefix.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/certificate_pack.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/certificate_pack.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/config/vars.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/custom_hostname.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/custom_hostname.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/custom_hostname_fallback_origin.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/custom_hostname_fallback_origin.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/custom_pages.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/custom_pages.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/custom_ssl.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/custom_ssl.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/device_dex_test.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/device_dex_test.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/device_managed_networks.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/device_managed_networks.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/device_policy_certificates.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/device_policy_certificates.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/device_posture_integration.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/device_posture_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/device_posture_rule.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/device_posture_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/device_settings_policy.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/device_settings_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/dlp_profile.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/dlp_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/email_routing_address.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/email_routing_address.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/email_routing_catch_all.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/email_routing_catch_all.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/email_routing_rule.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/email_routing_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/email_routing_settings.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/email_routing_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/fallback_domain.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/fallback_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/filter.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/filter.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/firewall_rule.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/firewall_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_access_identity_provider.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_access_identity_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_account_roles.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_account_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_accounts.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_accounts.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_api_token_permission_groups.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_api_token_permission_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_devices.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_devices.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_ip_ranges.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_ip_ranges.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_list.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_lists.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_lists.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_load_balancer_pools.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_load_balancer_pools.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_origin_ca_root_certificate.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_origin_ca_root_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_record.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_rulesets.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_rulesets.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_zone.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_zone_dnssec.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_zone_dnssec.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/get_zones.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/get_zones.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/gre_tunnel.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/gre_tunnel.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/healthcheck.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/healthcheck.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/ipsec_tunnel.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/ipsec_tunnel.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/list.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/list.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/list_item.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/list_item.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/load_balancer.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/load_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/load_balancer_monitor.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/load_balancer_monitor.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/load_balancer_pool.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/load_balancer_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/logpull_retention.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/logpull_retention.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/logpush_job.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/logpush_job.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/logpush_ownership_challenge.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/logpush_ownership_challenge.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/magic_firewall_ruleset.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/magic_firewall_ruleset.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/managed_headers.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/managed_headers.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/mtls_certificate.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/mtls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/notification_policy.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/notification_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/notification_policy_webhooks.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/notification_policy_webhooks.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/origin_ca_certificate.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/origin_ca_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/outputs.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/page_rule.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/page_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/pages_domain.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/pages_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/pages_project.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/pages_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/provider.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/queue.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/queue.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/r2_bucket.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/r2_bucket.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/rate_limit.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/rate_limit.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/record.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/record.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/regional_hostname.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/regional_hostname.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/ruleset.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/ruleset.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/spectrum_application.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/spectrum_application.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/split_tunnel.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/split_tunnel.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/static_route.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/static_route.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/teams_account.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/teams_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/teams_list.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/teams_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/teams_location.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/teams_location.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/teams_proxy_endpoint.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/teams_proxy_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/teams_rule.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/teams_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/tiered_cache.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/tiered_cache.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/total_tls.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/total_tls.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/tunnel.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/tunnel.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/tunnel_config.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/tunnel_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/tunnel_route.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/tunnel_route.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/tunnel_virtual_network.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/tunnel_virtual_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/turnstile_widget.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/turnstile_widget.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/url_normalization_settings.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/url_normalization_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/user_agent_blocking_rule.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/user_agent_blocking_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/waiting_room.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/waiting_room.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/waiting_room_event.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/waiting_room_event.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/waiting_room_rules.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/waiting_room_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/waiting_room_settings.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/waiting_room_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/web3_hostname.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/web3_hostname.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/worker_cron_trigger.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/worker_cron_trigger.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/worker_domain.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/worker_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/worker_route.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/worker_route.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/worker_script.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/worker_script.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/workers_kv.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/workers_kv.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/workers_kv_namespace.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/workers_kv_namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/zone.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/zone_cache_variants.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/zone_cache_variants.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/zone_dnssec.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/zone_dnssec.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/zone_lockdown.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/zone_lockdown.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare/zone_settings_override.py` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare/zone_settings_override.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare.egg-info/PKG-INFO` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-cloudflare
-Version: 5.4.0a1686761772
+Version: 5.5.0a1687050407
 Summary: A Pulumi package for creating and managing Cloudflare cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-cloudflare
 Keywords: pulumi cloudflare
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_cloudflare-5.4.0a1686761772/pulumi_cloudflare.egg-info/SOURCES.txt` & `pulumi_cloudflare-5.5.0a1687050407/pulumi_cloudflare.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_cloudflare-5.4.0a1686761772/setup.py` & `pulumi_cloudflare-5.5.0a1687050407/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "5.4.0a1686761772"
-PLUGIN_VERSION = "5.4.0-alpha.1686761772+07e5d0a4"
+VERSION = "5.5.0a1687050407"
+PLUGIN_VERSION = "5.5.0-alpha.1687050407+ed805cb6"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'cloudflare', PLUGIN_VERSION])
         except OSError as error:
```

