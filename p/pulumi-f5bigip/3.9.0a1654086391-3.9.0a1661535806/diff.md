# Comparing `tmp/pulumi_f5bigip-3.9.0a1654086391.tar.gz` & `tmp/pulumi_f5bigip-3.9.0a1661535806.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulumi_f5bigip-3.9.0a1654086391.tar", last modified: Wed Jun  1 12:31:54 2022, max compression
+gzip compressed data, was "pulumi_f5bigip-3.9.0a1661535806.tar", last modified: Fri Aug 26 17:47:31 2022, max compression
```

## Comparing `pulumi_f5bigip-3.9.0a1654086391.tar` & `pulumi_f5bigip-3.9.0a1661535806.tar`

### file list

```diff
@@ -1,109 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/
--rw-r--r--   0 runner    (1001) docker     (121)     3711 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2877 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/
--rw-r--r--   0 runner    (1001) docker     (121)    10150 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     7667 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)    31936 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/as3.py
--rw-r--r--   0 runner    (1001) docker     (121)    24534 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/big_iq_as3.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/cm/
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/cm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/cm/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    12397 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/cm/device.py
--rw-r--r--   0 runner    (1001) docker     (121)    27223 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/cm/device_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     1734 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/cm/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    11042 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/command.py
--rw-r--r--   0 runner    (1001) docker     (121)    45840 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/common_license_manage_big_iq.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/config/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1922 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (121)    24050 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/do.py
--rw-r--r--   0 runner    (1001) docker     (121)    10202 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/event_service_discovery.py
--rw-r--r--   0 runner    (1001) docker     (121)    11273 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/fast_application.py
--rw-r--r--   0 runner    (1001) docker     (121)     9781 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/fast_template.py
--rw-r--r--   0 runner    (1001) docker     (121)    35168 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ipsec_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)    14501 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ipsec_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/
--rw-r--r--   0 runner    (1001) docker     (121)     1224 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   159339 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    17826 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/data_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     5294 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/get_data_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     4111 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/get_irule.py
--rw-r--r--   0 runner    (1001) docker     (121)    10986 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/get_monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)     9077 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/get_node.py
--rw-r--r--   0 runner    (1001) docker     (121)     6848 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/get_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3934 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/get_pool.py
--rw-r--r--   0 runner    (1001) docker     (121)     7090 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/i_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)    61668 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)    26735 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/node.py
--rw-r--r--   0 runner    (1001) docker     (121)   112571 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    46657 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/persistence_profile_cookie.py
--rw-r--r--   0 runner    (1001) docker     (121)    30659 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/persistence_profile_dst_addr.py
--rw-r--r--   0 runner    (1001) docker     (121)    33464 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/persistence_profile_src_addr.py
--rw-r--r--   0 runner    (1001) docker     (121)    25631 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/persistence_profile_ssl.py
--rw-r--r--   0 runner    (1001) docker     (121)    18180 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/policy.py
--rw-r--r--   0 runner    (1001) docker     (121)    30295 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/pool.py
--rw-r--r--   0 runner    (1001) docker     (121)    30265 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/pool_attachment.py
--rw-r--r--   0 runner    (1001) docker     (121)   140736 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/profile_client_ssl.py
--rw-r--r--   0 runner    (1001) docker     (121)    40889 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/profile_fast_http.py
--rw-r--r--   0 runner    (1001) docker     (121)    38499 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/profile_fast_l4.py
--rw-r--r--   0 runner    (1001) docker     (121)    46457 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/profile_ftp.py
--rw-r--r--   0 runner    (1001) docker     (121)    76666 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/profile_http.py
--rw-r--r--   0 runner    (1001) docker     (121)    41454 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/profile_http2.py
--rw-r--r--   0 runner    (1001) docker     (121)    22994 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/profile_http_compress.py
--rw-r--r--   0 runner    (1001) docker     (121)    33968 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/profile_one_connect.py
--rw-r--r--   0 runner    (1001) docker     (121)   133163 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/profile_server_ssl.py
--rw-r--r--   0 runner    (1001) docker     (121)    32825 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/profile_tcp.py
--rw-r--r--   0 runner    (1001) docker     (121)    31378 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/snat.py
--rw-r--r--   0 runner    (1001) docker     (121)     8835 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/snat_pool.py
--rw-r--r--   0 runner    (1001) docker     (121)    23125 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/virtual_address.py
--rw-r--r--   0 runner    (1001) docker     (121)    68016 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/virtual_server.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/net/
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1826 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/net/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1494 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/net/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    13817 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/net/route.py
--rw-r--r--   0 runner    (1001) docker     (121)    17525 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/net/self_ip.py
--rw-r--r--   0 runner    (1001) docker     (121)    10997 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/net/vlan.py
--rw-r--r--   0 runner    (1001) docker     (121)    79878 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/net_ike_peer.py
--rw-r--r--   0 runner    (1001) docker     (121)    38494 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/net_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1144 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    12098 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ssl/
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1363 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ssl/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    11736 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ssl/certificate.py
--rw-r--r--   0 runner    (1001) docker     (121)     4398 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ssl/get_certificate.py
--rw-r--r--   0 runner    (1001) docker     (121)     9798 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ssl/get_v_wan_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    17695 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ssl/get_waf_entity_parameter.py
--rw-r--r--   0 runner    (1001) docker     (121)    10821 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ssl/get_waf_entity_url.py
--rw-r--r--   0 runner    (1001) docker     (121)     6359 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ssl/get_waf_pb_suggestions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3799 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ssl/get_waf_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     7941 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ssl/get_waf_signatures.py
--rw-r--r--   0 runner    (1001) docker     (121)    11710 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ssl/key.py
--rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ssl/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/sys/
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/sys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6232 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/sys/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     7909 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/sys/big_ip_license.py
--rw-r--r--   0 runner    (1001) docker     (121)    12922 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/sys/dns.py
--rw-r--r--   0 runner    (1001) docker     (121)    39768 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/sys/i_app.py
--rw-r--r--   0 runner    (1001) docker     (121)    10382 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/sys/ntp.py
--rw-r--r--   0 runner    (1001) docker     (121)     4871 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/sys/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    22297 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/sys/provision.py
--rw-r--r--   0 runner    (1001) docker     (121)    11215 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/sys/snmp.py
--rw-r--r--   0 runner    (1001) docker     (121)    32698 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/sys/snmp_traps.py
--rw-r--r--   0 runner    (1001) docker     (121)    31225 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/traffic_selector.py
--rw-r--r--   0 runner    (1001) docker     (121)    59669 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/waf_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3711 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3225 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2129 2022-06-01 12:31:53.000000 pulumi_f5bigip-3.9.0a1654086391/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 17:47:31.786108 pulumi_f5bigip-3.9.0a1661535806/
+-rw-r--r--   0 runner    (1001) docker     (121)     3220 2022-08-26 17:47:31.782107 pulumi_f5bigip-3.9.0a1661535806/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2877 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 17:47:31.770107 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/
+-rw-r--r--   0 runner    (1001) docker     (121)    10720 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30319 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8081 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31885 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/as3.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24483 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/big_iq_as3.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 17:47:31.774108 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/cm/
+-rw-r--r--   0 runner    (1001) docker     (121)      364 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/cm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1501 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/cm/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12346 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/cm/device.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27172 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/cm/device_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1746 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/cm/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10991 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/command.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45789 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/common_license_manage_big_iq.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 17:47:31.774108 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/config/
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1934 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23999 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/do.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10151 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/event_service_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11222 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/fast_application.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34640 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/fast_http_app.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40810 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/fast_https_app.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36205 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/fast_tcp_app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9730 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/fast_template.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35117 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ipsec_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14450 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ipsec_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 17:47:31.778108 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/
+-rw-r--r--   0 runner    (1001) docker     (121)     1224 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   160050 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17775 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/data_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5253 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/get_data_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4070 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/get_irule.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10945 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/get_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9036 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/get_node.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6807 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/get_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3893 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/get_pool.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7039 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/i_rule.py
+-rw-r--r--   0 runner    (1001) docker     (121)    62015 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26716 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/node.py
+-rw-r--r--   0 runner    (1001) docker     (121)   113119 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46606 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/persistence_profile_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30608 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/persistence_profile_dst_addr.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33413 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/persistence_profile_src_addr.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25580 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/persistence_profile_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18221 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30230 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/pool.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30218 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/pool_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (121)   140685 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/profile_client_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40838 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/profile_fast_http.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38448 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/profile_fast_l4.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46406 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/profile_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    76615 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/profile_http.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41403 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/profile_http2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22943 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/profile_http_compress.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33917 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/profile_one_connect.py
+-rw-r--r--   0 runner    (1001) docker     (121)   133112 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/profile_server_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32774 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/profile_tcp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31327 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/snat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8784 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/snat_pool.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23074 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/virtual_address.py
+-rw-r--r--   0 runner    (1001) docker     (121)    68047 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/virtual_server.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 17:47:31.782107 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/net/
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1838 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/net/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/net/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13766 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/net/route.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18975 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/net/self_ip.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10946 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/net/vlan.py
+-rw-r--r--   0 runner    (1001) docker     (121)    79827 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/net_ike_peer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38443 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/net_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28259 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12047 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 17:47:31.782107 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ssl/
+-rw-r--r--   0 runner    (1001) docker     (121)      599 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1375 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ssl/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11685 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ssl/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4357 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ssl/get_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9757 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ssl/get_v_wan_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17654 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ssl/get_waf_entity_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10780 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ssl/get_waf_entity_url.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6318 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ssl/get_waf_pb_suggestions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3758 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ssl/get_waf_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9953 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ssl/get_waf_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11659 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ssl/key.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ssl/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 17:47:31.782107 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/sys/
+-rw-r--r--   0 runner    (1001) docker     (121)      474 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/sys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6244 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/sys/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7858 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/sys/big_ip_license.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12871 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/sys/dns.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39717 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/sys/i_app.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10331 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/sys/ntp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4883 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/sys/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22246 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/sys/provision.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11164 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/sys/snmp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32647 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/sys/snmp_traps.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31174 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/traffic_selector.py
+-rw-r--r--   0 runner    (1001) docker     (121)    77249 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/waf_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 17:47:31.774108 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3220 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3321 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 17:47:31.786108 pulumi_f5bigip-3.9.0a1661535806/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2129 2022-08-26 17:47:31.000000 pulumi_f5bigip-3.9.0a1661535806/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/PKG-INFO` & `pulumi_f5bigip-3.9.0a1661535806/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,71 +1,73 @@
 Metadata-Version: 2.1
 Name: pulumi_f5bigip
-Version: 3.9.0a1654086391
+Version: 3.9.0a1661535806
 Summary: A Pulumi package for creating and managing F5 BigIP resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-f5bigip
-Description: [![Actions Status](https://github.com/pulumi/pulumi-f5bigip/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-f5bigip/actions)
-        [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
-        [![NPM version](https://badge.fury.io/js/%40pulumi%2Ff5bigip.svg)](https://www.npmjs.com/package/@pulumi/f5bigip)
-        [![Python version](https://badge.fury.io/py/pulumi-f5bigip.svg)](https://pypi.org/project/pulumi-f5bigip)
-        [![NuGet version](https://badge.fury.io/nu/pulumi.f5bigip.svg)](https://badge.fury.io/nu/pulumi.f5bigip)
-        [![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-f5bigip/sdk/v3/go)](https://pkg.go.dev/github.com/pulumi/pulumi-f5bigip/sdk/v3/go)
-        [![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumi.svg)](https://github.com/pulumi/pulumi-f5bigip/blob/master/LICENSE)
-        
-        # F5 BigIP Provider
-        
-        This provider allows management of F5 BigIP resources using Pulumi. This provider uses the iControlREST API to
-        perform management tasks, so it will need to be installed and enabled on your F5 device before proceeding.
-        
-        ## Installing
-        
-        This package is available in many languages in the standard packaging formats.
-        
-        ### Node.js (Java/TypeScript)
-        
-        To use from JavaScript or TypeScript in Node.js, install using either `npm`:
-        
-            $ npm install @pulumi/f5bigip
-        
-        or `yarn`:
-        
-            $ yarn add @pulumi/f5bigip
-        
-        ### Python
-        
-        To use from Python, install using `pip`:
-        
-            $ pip install pulumi_f5bigip
-        
-        ### Go
-        
-        To use from Go, use `go get` to grab the latest version of the library
-        
-            $ go get github.com/pulumi/pulumi-f5bigip/sdk/v3
-            
-        ### .NET
-        
-        To use from .NET, install using `dotnet add package`:
-        
-            $ dotnet add package Pulumi.F5bigip
-            
-        ## Configuration
-        
-        The following configuration points are available:
-        
-        - `f5bigip:address` - Domain name/IP of the BigIP. May be set via the `BIGIP_HOST` environment variable.
-        - `f5bigip:port` - Management Port to connect to BigIP.
-        - `f5bigip:username` - Username with API access to the BigIP. May be set via the `BIGIP_USER` environment variable.
-        - `f5bigip:password` - Password for API access to the BigIP. May be set via the `BIGIP_PASSWORD` environment variable.
-        - `f5bigip:tokenAuth` - Enable to use an external authentication source (LDAP, TACACS, etc). May be set via the `BIGIP_TOKEN_AUTH` environment variable.
-        - `f5bigip:tokenAuth` - Enable to use an external authentication source (LDAP, TACACS, etc). May be set via the `BIGIP_TOKEN_AUTH` environment variable.
-        - `f5bigip:loginRef` - Login reference for token authentication (see BIG-IP REST docs for details) May be set via the `BIGIP_LOGIN_REF` environment variable.
-        
-        ## Reference
-        
-        For further information, please visit [the F5bigip provider docs](https://www.pulumi.com/docs/intro/cloud-providers/f5bigip) or for detailed reference documentation, please visit [the API docs](https://www.pulumi.com/docs/reference/pkg/f5bigip).
-        
 Keywords: pulumi f5 bigip
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+
+[![Actions Status](https://github.com/pulumi/pulumi-f5bigip/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-f5bigip/actions)
+[![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
+[![NPM version](https://badge.fury.io/js/%40pulumi%2Ff5bigip.svg)](https://www.npmjs.com/package/@pulumi/f5bigip)
+[![Python version](https://badge.fury.io/py/pulumi-f5bigip.svg)](https://pypi.org/project/pulumi-f5bigip)
+[![NuGet version](https://badge.fury.io/nu/pulumi.f5bigip.svg)](https://badge.fury.io/nu/pulumi.f5bigip)
+[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-f5bigip/sdk/v3/go)](https://pkg.go.dev/github.com/pulumi/pulumi-f5bigip/sdk/v3/go)
+[![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumi.svg)](https://github.com/pulumi/pulumi-f5bigip/blob/master/LICENSE)
+
+# F5 BigIP Provider
+
+This provider allows management of F5 BigIP resources using Pulumi. This provider uses the iControlREST API to
+perform management tasks, so it will need to be installed and enabled on your F5 device before proceeding.
+
+## Installing
+
+This package is available in many languages in the standard packaging formats.
+
+### Node.js (Java/TypeScript)
+
+To use from JavaScript or TypeScript in Node.js, install using either `npm`:
+
+    $ npm install @pulumi/f5bigip
+
+or `yarn`:
+
+    $ yarn add @pulumi/f5bigip
+
+### Python
+
+To use from Python, install using `pip`:
+
+    $ pip install pulumi_f5bigip
+
+### Go
+
+To use from Go, use `go get` to grab the latest version of the library
+
+    $ go get github.com/pulumi/pulumi-f5bigip/sdk/v3
+    
+### .NET
+
+To use from .NET, install using `dotnet add package`:
+
+    $ dotnet add package Pulumi.F5bigip
+    
+## Configuration
+
+The following configuration points are available:
+
+- `f5bigip:address` - Domain name/IP of the BigIP. May be set via the `BIGIP_HOST` environment variable.
+- `f5bigip:port` - Management Port to connect to BigIP.
+- `f5bigip:username` - Username with API access to the BigIP. May be set via the `BIGIP_USER` environment variable.
+- `f5bigip:password` - Password for API access to the BigIP. May be set via the `BIGIP_PASSWORD` environment variable.
+- `f5bigip:tokenAuth` - Enable to use an external authentication source (LDAP, TACACS, etc). May be set via the `BIGIP_TOKEN_AUTH` environment variable.
+- `f5bigip:tokenAuth` - Enable to use an external authentication source (LDAP, TACACS, etc). May be set via the `BIGIP_TOKEN_AUTH` environment variable.
+- `f5bigip:loginRef` - Login reference for token authentication (see BIG-IP REST docs for details) May be set via the `BIGIP_LOGIN_REF` environment variable.
+
+## Reference
+
+For further information, please visit [the F5bigip provider docs](https://www.pulumi.com/docs/intro/cloud-providers/f5bigip) or for detailed reference documentation, please visit [the API docs](https://www.pulumi.com/docs/reference/pkg/f5bigip).
+
+
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/README.md` & `pulumi_f5bigip-3.9.0a1661535806/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/__init__.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 from .as3 import *
 from .big_iq_as3 import *
 from .command import *
 from .common_license_manage_big_iq import *
 from .do import *
 from .event_service_discovery import *
 from .fast_application import *
+from .fast_http_app import *
+from .fast_https_app import *
+from .fast_tcp_app import *
 from .fast_template import *
 from .ipsec_policy import *
 from .ipsec_profile import *
 from .net_ike_peer import *
 from .net_tunnel import *
 from .provider import *
 from .traffic_selector import *
@@ -118,14 +121,38 @@
   "fqn": "pulumi_f5bigip",
   "classes": {
    "f5bigip:index/fastApplication:FastApplication": "FastApplication"
   }
  },
  {
   "pkg": "f5bigip",
+  "mod": "index/fastHttpApp",
+  "fqn": "pulumi_f5bigip",
+  "classes": {
+   "f5bigip:index/fastHttpApp:FastHttpApp": "FastHttpApp"
+  }
+ },
+ {
+  "pkg": "f5bigip",
+  "mod": "index/fastHttpsApp",
+  "fqn": "pulumi_f5bigip",
+  "classes": {
+   "f5bigip:index/fastHttpsApp:FastHttpsApp": "FastHttpsApp"
+  }
+ },
+ {
+  "pkg": "f5bigip",
+  "mod": "index/fastTcpApp",
+  "fqn": "pulumi_f5bigip",
+  "classes": {
+   "f5bigip:index/fastTcpApp:FastTcpApp": "FastTcpApp"
+  }
+ },
+ {
+  "pkg": "f5bigip",
   "mod": "index/fastTemplate",
   "fqn": "pulumi_f5bigip",
   "classes": {
    "f5bigip:index/fastTemplate:FastTemplate": "FastTemplate"
   }
  },
  {
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/_inputs.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/cm/_inputs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,50 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from . import _utilities
+from .. import _utilities
 
 __all__ = [
-    'EventServiceDiscoveryNodeArgs',
+    'DeviceGroupDeviceArgs',
 ]
 
 @pulumi.input_type
-class EventServiceDiscoveryNodeArgs:
+class DeviceGroupDeviceArgs:
     def __init__(__self__, *,
-                 id: Optional[pulumi.Input[str]] = None,
-                 ip: Optional[pulumi.Input[str]] = None,
-                 port: Optional[pulumi.Input[int]] = None):
-        if id is not None:
-            pulumi.set(__self__, "id", id)
-        if ip is not None:
-            pulumi.set(__self__, "ip", ip)
-        if port is not None:
-            pulumi.set(__self__, "port", port)
+                 name: Optional[pulumi.Input[str]] = None,
+                 set_sync_leader: Optional[pulumi.Input[bool]] = None):
+        """
+        :param pulumi.Input[str] name: Is the name of the device Group
+        """
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if set_sync_leader is not None:
+            pulumi.set(__self__, "set_sync_leader", set_sync_leader)
 
     @property
     @pulumi.getter
-    def id(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "id")
-
-    @id.setter
-    def id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "id", value)
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Is the name of the device Group
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter
-    def ip(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "ip")
-
-    @ip.setter
-    def ip(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "ip", value)
-
-    @property
-    @pulumi.getter
-    def port(self) -> Optional[pulumi.Input[int]]:
-        return pulumi.get(self, "port")
-
-    @port.setter
-    def port(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "port", value)
+    @pulumi.getter(name="setSyncLeader")
+    def set_sync_leader(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "set_sync_leader")
+
+    @set_sync_leader.setter
+    def set_sync_leader(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "set_sync_leader", value)
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/_utilities.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/_utilities.py`

 * *Files 7% similar despite different names*

```diff
@@ -94,14 +94,25 @@
 _version = _get_semver_version()
 _version_str = str(_version)
 
 
 def get_version():
     return _version_str
 
+def get_resource_opts_defaults() -> pulumi.ResourceOptions:
+    return pulumi.ResourceOptions(
+        version=get_version(),
+        plugin_download_url=get_plugin_download_url(),
+    )
+
+def get_invoke_opts_defaults() -> pulumi.InvokeOptions:
+    return pulumi.InvokeOptions(
+        version=get_version(),
+        plugin_download_url=get_plugin_download_url(),
+    )
 
 def get_resource_args_opts(resource_args_type, resource_options_type, *args, **kwargs):
     """
     Return the resource args and options given the *args and **kwargs of a resource's
     __init__ method.
     """
 
@@ -230,7 +241,10 @@
             'args': args_list,
             'kwargs': bound_args.kwargs
         }).apply(lambda resolved_args: func(*resolved_args['args'],
                                             opts=opts,
                                             **resolved_args['kwargs']))
 
     return (lambda _: lifted_func)
+
+def get_plugin_download_url():
+	return None
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/as3.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/as3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['As3Args', 'As3']
@@ -1222,20 +1223,17 @@
                  as3_json: Optional[pulumi.Input[str]] = None,
                  ignore_metadata: Optional[pulumi.Input[bool]] = None,
                  task_id: Optional[pulumi.Input[str]] = None,
                  tenant_filter: Optional[pulumi.Input[str]] = None,
                  tenant_list: Optional[pulumi.Input[str]] = None,
                  tenant_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = As3Args.__new__(As3Args)
 
             __props__.__dict__["application_list"] = application_list
             __props__.__dict__["as3_json"] = as3_json
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/big_iq_as3.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/big_iq_as3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['BigIqAs3Args', 'BigIqAs3']
@@ -402,20 +403,17 @@
                  bigiq_password: Optional[pulumi.Input[str]] = None,
                  bigiq_port: Optional[pulumi.Input[str]] = None,
                  bigiq_token_auth: Optional[pulumi.Input[bool]] = None,
                  bigiq_user: Optional[pulumi.Input[str]] = None,
                  ignore_metadata: Optional[pulumi.Input[bool]] = None,
                  tenant_list: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = BigIqAs3Args.__new__(BigIqAs3Args)
 
             if as3_json is None and not opts.urn:
                 raise TypeError("Missing required property 'as3_json'")
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/cm/device.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/cm/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['DeviceArgs', 'Device']
@@ -225,20 +226,17 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  configsync_ip: Optional[pulumi.Input[str]] = None,
                  mirror_ip: Optional[pulumi.Input[str]] = None,
                  mirror_secondary_ip: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = DeviceArgs.__new__(DeviceArgs)
 
             if configsync_ip is None and not opts.urn:
                 raise TypeError("Missing required property 'configsync_ip'")
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/cm/device_group.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/cm/device_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -453,20 +454,17 @@
                  incremental_config: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  network_failover: Optional[pulumi.Input[str]] = None,
                  partition: Optional[pulumi.Input[str]] = None,
                  save_on_auto_sync: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = DeviceGroupArgs.__new__(DeviceGroupArgs)
 
             __props__.__dict__["auto_sync"] = auto_sync
             __props__.__dict__["description"] = description
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/cm/outputs.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/cm/outputs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/command.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['CommandArgs', 'Command']
@@ -180,20 +181,17 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  command_results: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  commands: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  when: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = CommandArgs.__new__(CommandArgs)
 
             __props__.__dict__["command_results"] = command_results
             if commands is None and not opts.urn:
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/common_license_manage_big_iq.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/common_license_manage_big_iq.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['CommonLicenseManageBigIqArgs', 'CommonLicenseManageBigIq']
@@ -722,20 +723,17 @@
                  license_poolname: Optional[pulumi.Input[str]] = None,
                  mac_address: Optional[pulumi.Input[str]] = None,
                  skukeyword1: Optional[pulumi.Input[str]] = None,
                  skukeyword2: Optional[pulumi.Input[str]] = None,
                  tenant: Optional[pulumi.Input[str]] = None,
                  unit_of_measure: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = CommonLicenseManageBigIqArgs.__new__(CommonLicenseManageBigIqArgs)
 
             if assignment_type is None and not opts.urn:
                 raise TypeError("Missing required property 'assignment_type'")
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/config/vars.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/config/vars.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 import types
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/do.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/do.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['DoArgs', 'Do']
@@ -388,20 +389,17 @@
                  bigip_port: Optional[pulumi.Input[str]] = None,
                  bigip_token_auth: Optional[pulumi.Input[bool]] = None,
                  bigip_user: Optional[pulumi.Input[str]] = None,
                  do_json: Optional[pulumi.Input[str]] = None,
                  tenant_name: Optional[pulumi.Input[str]] = None,
                  timeout: Optional[pulumi.Input[int]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = DoArgs.__new__(DoArgs)
 
             __props__.__dict__["bigip_address"] = bigip_address
             __props__.__dict__["bigip_password"] = bigip_password
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/event_service_discovery.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/event_service_discovery.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
@@ -170,20 +171,17 @@
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  nodes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['EventServiceDiscoveryNodeArgs']]]]] = None,
                  taskid: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = EventServiceDiscoveryArgs.__new__(EventServiceDiscoveryArgs)
 
             __props__.__dict__["nodes"] = nodes
             if taskid is None and not opts.urn:
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/fast_application.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/fast_application.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['FastApplicationArgs', 'FastApplication']
@@ -182,20 +183,17 @@
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  fast_json: Optional[pulumi.Input[str]] = None,
                  template: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = FastApplicationArgs.__new__(FastApplicationArgs)
 
             if fast_json is None and not opts.urn:
                 raise TypeError("Missing required property 'fast_json'")
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/fast_template.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/fast_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['FastTemplateArgs', 'FastTemplate']
@@ -164,20 +165,17 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  md5_hash: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  source: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = FastTemplateArgs.__new__(FastTemplateArgs)
 
             if md5_hash is None and not opts.urn:
                 raise TypeError("Missing required property 'md5_hash'")
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ipsec_policy.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ipsec_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['IpsecPolicyArgs', 'IpsecPolicy']
@@ -535,20 +536,17 @@
                  mode: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  perfect_forward_secrecy: Optional[pulumi.Input[str]] = None,
                  protocol: Optional[pulumi.Input[str]] = None,
                  tunnel_local_address: Optional[pulumi.Input[str]] = None,
                  tunnel_remote_address: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = IpsecPolicyArgs.__new__(IpsecPolicyArgs)
 
             __props__.__dict__["auth_algorithm"] = auth_algorithm
             __props__.__dict__["description"] = description
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ipsec_profile.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ipsec_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['IpsecProfileArgs', 'IpsecProfile']
@@ -222,20 +223,17 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  parent_profile: Optional[pulumi.Input[str]] = None,
                  traffic_selector: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = IpsecProfileArgs.__new__(IpsecProfileArgs)
 
             __props__.__dict__["description"] = description
             if name is None and not opts.urn:
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/__init__.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/_inputs.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -290,14 +291,15 @@
                  value: Optional[pulumi.Input[str]] = None,
                  virtual: Optional[pulumi.Input[str]] = None,
                  vlan: Optional[pulumi.Input[str]] = None,
                  vlan_id: Optional[pulumi.Input[int]] = None,
                  wam: Optional[pulumi.Input[bool]] = None,
                  write: Optional[pulumi.Input[bool]] = None):
         """
+        :param pulumi.Input[bool] connection: This action is set to `true` by default, it needs to be explicitly set to `false` for actions it conflicts with.
         :param pulumi.Input[bool] forward: This action will affect forwarding.
         :param pulumi.Input[str] pool: This action will direct the stream to this pool.
         """
         if app_service is not None:
             pulumi.set(__self__, "app_service", app_service)
         if application is not None:
             pulumi.set(__self__, "application", application)
@@ -604,14 +606,17 @@
     @compress.setter
     def compress(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "compress", value)
 
     @property
     @pulumi.getter
     def connection(self) -> Optional[pulumi.Input[bool]]:
+        """
+        This action is set to `true` by default, it needs to be explicitly set to `false` for actions it conflicts with.
+        """
         return pulumi.get(self, "connection")
 
     @connection.setter
     def connection(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "connection", value)
 
     @property
@@ -1470,14 +1475,15 @@
                  country_name: Optional[pulumi.Input[bool]] = None,
                  cpu_usage: Optional[pulumi.Input[bool]] = None,
                  device_make: Optional[pulumi.Input[bool]] = None,
                  device_model: Optional[pulumi.Input[bool]] = None,
                  domain: Optional[pulumi.Input[bool]] = None,
                  ends_with: Optional[pulumi.Input[bool]] = None,
                  equals: Optional[pulumi.Input[bool]] = None,
+                 exists: Optional[pulumi.Input[bool]] = None,
                  expiry: Optional[pulumi.Input[bool]] = None,
                  extension: Optional[pulumi.Input[bool]] = None,
                  external: Optional[pulumi.Input[bool]] = None,
                  geoip: Optional[pulumi.Input[bool]] = None,
                  greater: Optional[pulumi.Input[bool]] = None,
                  greater_or_equal: Optional[pulumi.Input[bool]] = None,
                  host: Optional[pulumi.Input[bool]] = None,
@@ -1582,14 +1588,16 @@
             pulumi.set(__self__, "device_model", device_model)
         if domain is not None:
             pulumi.set(__self__, "domain", domain)
         if ends_with is not None:
             pulumi.set(__self__, "ends_with", ends_with)
         if equals is not None:
             pulumi.set(__self__, "equals", equals)
+        if exists is not None:
+            pulumi.set(__self__, "exists", exists)
         if expiry is not None:
             pulumi.set(__self__, "expiry", expiry)
         if extension is not None:
             pulumi.set(__self__, "extension", extension)
         if external is not None:
             pulumi.set(__self__, "external", external)
         if geoip is not None:
@@ -1919,14 +1927,23 @@
 
     @equals.setter
     def equals(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "equals", value)
 
     @property
     @pulumi.getter
+    def exists(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "exists")
+
+    @exists.setter
+    def exists(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "exists", value)
+
+    @property
+    @pulumi.getter
     def expiry(self) -> Optional[pulumi.Input[bool]]:
         return pulumi.get(self, "expiry")
 
     @expiry.setter
     def expiry(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "expiry", value)
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/data_group.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/data_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -243,20 +244,17 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  internal: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  records: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DataGroupRecordArgs']]]]] = None,
                  records_src: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = DataGroupArgs.__new__(DataGroupArgs)
 
             __props__.__dict__["internal"] = internal
             if name is None and not opts.urn:
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/get_data_group.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/get_data_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -112,18 +113,15 @@
     :param str type: The Data Group type (string, ip, integer)"
     """
     __args__ = dict()
     __args__['name'] = name
     __args__['partition'] = partition
     __args__['records'] = records
     __args__['type'] = type
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('f5bigip:ltm/getDataGroup:getDataGroup', __args__, opts=opts, typ=GetDataGroupResult).value
 
     return AwaitableGetDataGroupResult(
         id=__ret__.id,
         name=__ret__.name,
         partition=__ret__.partition,
         records=__ret__.records,
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/get_irule.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/get_irule.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -99,18 +100,15 @@
 
     :param str name: Name of the irule
     :param str partition: partition of the ltm irule
     """
     __args__ = dict()
     __args__['name'] = name
     __args__['partition'] = partition
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('f5bigip:ltm/getIrule:getIrule', __args__, opts=opts, typ=GetIruleResult).value
 
     return AwaitableGetIruleResult(
         id=__ret__.id,
         irule=__ret__.irule,
         name=__ret__.name,
         partition=__ret__.partition)
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/get_monitor.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/get_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -248,18 +249,15 @@
 
     :param str name: Name of the ltm monitor
     :param str partition: partition of the ltm monitor
     """
     __args__ = dict()
     __args__['name'] = name
     __args__['partition'] = partition
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('f5bigip:ltm/getMonitor:getMonitor', __args__, opts=opts, typ=GetMonitorResult).value
 
     return AwaitableGetMonitorResult(
         adaptive=__ret__.adaptive,
         adaptive_limit=__ret__.adaptive_limit,
         database=__ret__.database,
         defaults_from=__ret__.defaults_from,
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/get_node.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/get_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -209,18 +210,15 @@
     __args__ = dict()
     __args__['address'] = address
     __args__['description'] = description
     __args__['fqdn'] = fqdn
     __args__['fullPath'] = full_path
     __args__['name'] = name
     __args__['partition'] = partition
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('f5bigip:ltm/getNode:getNode', __args__, opts=opts, typ=GetNodeResult).value
 
     return AwaitableGetNodeResult(
         address=__ret__.address,
         connection_limit=__ret__.connection_limit,
         description=__ret__.description,
         dynamic_ratio=__ret__.dynamic_ratio,
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/get_policy.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/get_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -144,18 +145,15 @@
     __args__ = dict()
     __args__['controls'] = controls
     __args__['name'] = name
     __args__['publishedCopy'] = published_copy
     __args__['requires'] = requires
     __args__['rules'] = rules
     __args__['strategy'] = strategy
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('f5bigip:ltm/getPolicy:getPolicy', __args__, opts=opts, typ=GetPolicyResult).value
 
     return AwaitableGetPolicyResult(
         controls=__ret__.controls,
         id=__ret__.id,
         name=__ret__.name,
         published_copy=__ret__.published_copy,
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/get_pool.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/get_pool.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -92,18 +93,15 @@
 
     :param str name: Name of the ltm monitor
     :param str partition: partition of the ltm monitor
     """
     __args__ = dict()
     __args__['name'] = name
     __args__['partition'] = partition
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('f5bigip:ltm/getPool:getPool', __args__, opts=opts, typ=GetPoolResult).value
 
     return AwaitableGetPoolResult(
         full_path=__ret__.full_path,
         id=__ret__.id,
         name=__ret__.name,
         partition=__ret__.partition)
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/i_rule.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/i_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['IRuleArgs', 'IRule']
@@ -131,20 +132,17 @@
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  irule: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = IRuleArgs.__new__(IRuleArgs)
 
             if irule is None and not opts.urn:
                 raise TypeError("Missing required property 'irule'")
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/monitor.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['MonitorArgs', 'Monitor']
@@ -42,15 +43,15 @@
         :param pulumi.Input[str] parent: Parent monitor for the system to use for setting initial values for the new monitor.
         :param pulumi.Input[str] adaptive: Specifies whether adaptive response time monitoring is enabled for this monitor. The default is `disabled`.
         :param pulumi.Input[int] adaptive_limit: Specifies the absolute number of milliseconds that may not be exceeded by a monitor probe, regardless of Allowed Divergence.
         :param pulumi.Input[str] compatibility: Specifies, when enabled, that the SSL options setting (in OpenSSL) is set to ALL. Accepts 'enabled' or 'disabled' values, the default value is 'enabled'.
         :param pulumi.Input[str] database: Specifies the database in which the user is created
         :param pulumi.Input[str] destination: Specify an alias address for monitoring
         :param pulumi.Input[str] filename: Specifies the full path and file name of the file that the system attempts to download. The health check is successful if the system can download the file.
-        :param pulumi.Input[int] interval: Specifies, in seconds, the frequency at which the system issues the monitor check when either the resource is down or the status of the resource is unknown. The default is `5`
+        :param pulumi.Input[int] interval: Specifies, in seconds, the frequency at which the system issues the monitor check when either the resource is down or the status of the resource is unknown,value of `interval` should be always less than `timeout`. Default is `5`.
         :param pulumi.Input[int] ip_dscp: Displays the differentiated services code point (DSCP).The default is `0 (zero)`.
         :param pulumi.Input[str] manual_resume: Specifies whether the system automatically changes the status of a resource to Enabled at the next successful monitor check.
         :param pulumi.Input[str] mode: Specifies the data transfer process (DTP) mode. The default value is passive. The options are passive (Specifies that the monitor sends a data transfer request to the FTP server. When the FTP server receives the request, the FTP server then initiates and establishes the data connection.) and active (Specifies that the monitor initiates and establishes the data connection with the FTP server.).
         :param pulumi.Input[str] password: Specifies the password if the monitored target requires authentication
         :param pulumi.Input[str] receive: Specifies the regular expression representing the text string that the monitor looks for in the returned resource.
         :param pulumi.Input[str] receive_disable: The system marks the node or pool member disabled when its response matches Receive Disable String but not Receive String.
         :param pulumi.Input[str] reverse: Instructs the system to mark the target resource down when the test is successful.
@@ -203,15 +204,15 @@
     def filename(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "filename", value)
 
     @property
     @pulumi.getter
     def interval(self) -> Optional[pulumi.Input[int]]:
         """
-        Specifies, in seconds, the frequency at which the system issues the monitor check when either the resource is down or the status of the resource is unknown. The default is `5`
+        Specifies, in seconds, the frequency at which the system issues the monitor check when either the resource is down or the status of the resource is unknown,value of `interval` should be always less than `timeout`. Default is `5`.
         """
         return pulumi.get(self, "interval")
 
     @interval.setter
     def interval(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "interval", value)
 
@@ -414,15 +415,15 @@
         Input properties used for looking up and filtering Monitor resources.
         :param pulumi.Input[str] adaptive: Specifies whether adaptive response time monitoring is enabled for this monitor. The default is `disabled`.
         :param pulumi.Input[int] adaptive_limit: Specifies the absolute number of milliseconds that may not be exceeded by a monitor probe, regardless of Allowed Divergence.
         :param pulumi.Input[str] compatibility: Specifies, when enabled, that the SSL options setting (in OpenSSL) is set to ALL. Accepts 'enabled' or 'disabled' values, the default value is 'enabled'.
         :param pulumi.Input[str] database: Specifies the database in which the user is created
         :param pulumi.Input[str] destination: Specify an alias address for monitoring
         :param pulumi.Input[str] filename: Specifies the full path and file name of the file that the system attempts to download. The health check is successful if the system can download the file.
-        :param pulumi.Input[int] interval: Specifies, in seconds, the frequency at which the system issues the monitor check when either the resource is down or the status of the resource is unknown. The default is `5`
+        :param pulumi.Input[int] interval: Specifies, in seconds, the frequency at which the system issues the monitor check when either the resource is down or the status of the resource is unknown,value of `interval` should be always less than `timeout`. Default is `5`.
         :param pulumi.Input[int] ip_dscp: Displays the differentiated services code point (DSCP).The default is `0 (zero)`.
         :param pulumi.Input[str] manual_resume: Specifies whether the system automatically changes the status of a resource to Enabled at the next successful monitor check.
         :param pulumi.Input[str] mode: Specifies the data transfer process (DTP) mode. The default value is passive. The options are passive (Specifies that the monitor sends a data transfer request to the FTP server. When the FTP server receives the request, the FTP server then initiates and establishes the data connection.) and active (Specifies that the monitor initiates and establishes the data connection with the FTP server.).
         :param pulumi.Input[str] name: Specifies the Name of the LTM Monitor.Name of Monitor should be full path,full path is the combination of the `partition + monitor name`,For ex:`/Common/test-ltm-monitor`.
         :param pulumi.Input[str] parent: Parent monitor for the system to use for setting initial values for the new monitor.
         :param pulumi.Input[str] password: Specifies the password if the monitored target requires authentication
         :param pulumi.Input[str] receive: Specifies the regular expression representing the text string that the monitor looks for in the returned resource.
@@ -555,15 +556,15 @@
     def filename(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "filename", value)
 
     @property
     @pulumi.getter
     def interval(self) -> Optional[pulumi.Input[int]]:
         """
-        Specifies, in seconds, the frequency at which the system issues the monitor check when either the resource is down or the status of the resource is unknown. The default is `5`
+        Specifies, in seconds, the frequency at which the system issues the monitor check when either the resource is down or the status of the resource is unknown,value of `interval` should be always less than `timeout`. Default is `5`.
         """
         return pulumi.get(self, "interval")
 
     @interval.setter
     def interval(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "interval", value)
 
@@ -788,40 +789,40 @@
                  transparent: Optional[pulumi.Input[str]] = None,
                  up_interval: Optional[pulumi.Input[int]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         `ltm.Monitor` Configures a custom monitor for use by health checks.
 
-        For resources should be named with their "full path". The full path is the combination of the partition + name of the resource. For example /Common/my-pool.
+        For resources should be named with their `full path`. The full path is the combination of the `partition + name` of the resource. For example `/Common/test-monitor`.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_f5bigip as f5bigip
 
         monitor = f5bigip.ltm.Monitor("monitor",
             destination="1.2.3.4:1234",
-            interval=999,
+            interval=998,
             name="/Common/terraform_monitor",
             parent="/Common/http",
             send=\"\"\"GET /some/path
 
         \"\"\",
             timeout=999)
         test_https_monitor = f5bigip.ltm.Monitor("test-https-monitor",
             interval=999,
             name="/Common/terraform_monitor",
             parent="/Common/http",
             send=\"\"\"GET /some/path
 
         \"\"\",
             ssl_profile="/Common/serverssl",
-            timeout=999)
+            timeout=1000)
         test_ftp_monitor = f5bigip.ltm.Monitor("test-ftp-monitor",
             destination="*:8008",
             filename="somefile",
             interval=5,
             name="/Common/ftp-test",
             parent="/Common/ftp",
             time_until_up=0,
@@ -841,15 +842,15 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] adaptive: Specifies whether adaptive response time monitoring is enabled for this monitor. The default is `disabled`.
         :param pulumi.Input[int] adaptive_limit: Specifies the absolute number of milliseconds that may not be exceeded by a monitor probe, regardless of Allowed Divergence.
         :param pulumi.Input[str] compatibility: Specifies, when enabled, that the SSL options setting (in OpenSSL) is set to ALL. Accepts 'enabled' or 'disabled' values, the default value is 'enabled'.
         :param pulumi.Input[str] database: Specifies the database in which the user is created
         :param pulumi.Input[str] destination: Specify an alias address for monitoring
         :param pulumi.Input[str] filename: Specifies the full path and file name of the file that the system attempts to download. The health check is successful if the system can download the file.
-        :param pulumi.Input[int] interval: Specifies, in seconds, the frequency at which the system issues the monitor check when either the resource is down or the status of the resource is unknown. The default is `5`
+        :param pulumi.Input[int] interval: Specifies, in seconds, the frequency at which the system issues the monitor check when either the resource is down or the status of the resource is unknown,value of `interval` should be always less than `timeout`. Default is `5`.
         :param pulumi.Input[int] ip_dscp: Displays the differentiated services code point (DSCP).The default is `0 (zero)`.
         :param pulumi.Input[str] manual_resume: Specifies whether the system automatically changes the status of a resource to Enabled at the next successful monitor check.
         :param pulumi.Input[str] mode: Specifies the data transfer process (DTP) mode. The default value is passive. The options are passive (Specifies that the monitor sends a data transfer request to the FTP server. When the FTP server receives the request, the FTP server then initiates and establishes the data connection.) and active (Specifies that the monitor initiates and establishes the data connection with the FTP server.).
         :param pulumi.Input[str] name: Specifies the Name of the LTM Monitor.Name of Monitor should be full path,full path is the combination of the `partition + monitor name`,For ex:`/Common/test-ltm-monitor`.
         :param pulumi.Input[str] parent: Parent monitor for the system to use for setting initial values for the new monitor.
         :param pulumi.Input[str] password: Specifies the password if the monitored target requires authentication
         :param pulumi.Input[str] receive: Specifies the regular expression representing the text string that the monitor looks for in the returned resource.
@@ -868,40 +869,40 @@
     def __init__(__self__,
                  resource_name: str,
                  args: MonitorArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         `ltm.Monitor` Configures a custom monitor for use by health checks.
 
-        For resources should be named with their "full path". The full path is the combination of the partition + name of the resource. For example /Common/my-pool.
+        For resources should be named with their `full path`. The full path is the combination of the `partition + name` of the resource. For example `/Common/test-monitor`.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_f5bigip as f5bigip
 
         monitor = f5bigip.ltm.Monitor("monitor",
             destination="1.2.3.4:1234",
-            interval=999,
+            interval=998,
             name="/Common/terraform_monitor",
             parent="/Common/http",
             send=\"\"\"GET /some/path
 
         \"\"\",
             timeout=999)
         test_https_monitor = f5bigip.ltm.Monitor("test-https-monitor",
             interval=999,
             name="/Common/terraform_monitor",
             parent="/Common/http",
             send=\"\"\"GET /some/path
 
         \"\"\",
             ssl_profile="/Common/serverssl",
-            timeout=999)
+            timeout=1000)
         test_ftp_monitor = f5bigip.ltm.Monitor("test-ftp-monitor",
             destination="*:8008",
             filename="somefile",
             interval=5,
             name="/Common/ftp-test",
             parent="/Common/ftp",
             time_until_up=0,
@@ -952,20 +953,17 @@
                  ssl_profile: Optional[pulumi.Input[str]] = None,
                  time_until_up: Optional[pulumi.Input[int]] = None,
                  timeout: Optional[pulumi.Input[int]] = None,
                  transparent: Optional[pulumi.Input[str]] = None,
                  up_interval: Optional[pulumi.Input[int]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = MonitorArgs.__new__(MonitorArgs)
 
             __props__.__dict__["adaptive"] = adaptive
             __props__.__dict__["adaptive_limit"] = adaptive_limit
@@ -1036,15 +1034,15 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] adaptive: Specifies whether adaptive response time monitoring is enabled for this monitor. The default is `disabled`.
         :param pulumi.Input[int] adaptive_limit: Specifies the absolute number of milliseconds that may not be exceeded by a monitor probe, regardless of Allowed Divergence.
         :param pulumi.Input[str] compatibility: Specifies, when enabled, that the SSL options setting (in OpenSSL) is set to ALL. Accepts 'enabled' or 'disabled' values, the default value is 'enabled'.
         :param pulumi.Input[str] database: Specifies the database in which the user is created
         :param pulumi.Input[str] destination: Specify an alias address for monitoring
         :param pulumi.Input[str] filename: Specifies the full path and file name of the file that the system attempts to download. The health check is successful if the system can download the file.
-        :param pulumi.Input[int] interval: Specifies, in seconds, the frequency at which the system issues the monitor check when either the resource is down or the status of the resource is unknown. The default is `5`
+        :param pulumi.Input[int] interval: Specifies, in seconds, the frequency at which the system issues the monitor check when either the resource is down or the status of the resource is unknown,value of `interval` should be always less than `timeout`. Default is `5`.
         :param pulumi.Input[int] ip_dscp: Displays the differentiated services code point (DSCP).The default is `0 (zero)`.
         :param pulumi.Input[str] manual_resume: Specifies whether the system automatically changes the status of a resource to Enabled at the next successful monitor check.
         :param pulumi.Input[str] mode: Specifies the data transfer process (DTP) mode. The default value is passive. The options are passive (Specifies that the monitor sends a data transfer request to the FTP server. When the FTP server receives the request, the FTP server then initiates and establishes the data connection.) and active (Specifies that the monitor initiates and establishes the data connection with the FTP server.).
         :param pulumi.Input[str] name: Specifies the Name of the LTM Monitor.Name of Monitor should be full path,full path is the combination of the `partition + monitor name`,For ex:`/Common/test-ltm-monitor`.
         :param pulumi.Input[str] parent: Parent monitor for the system to use for setting initial values for the new monitor.
         :param pulumi.Input[str] password: Specifies the password if the monitored target requires authentication
         :param pulumi.Input[str] receive: Specifies the regular expression representing the text string that the monitor looks for in the returned resource.
@@ -1135,15 +1133,15 @@
         """
         return pulumi.get(self, "filename")
 
     @property
     @pulumi.getter
     def interval(self) -> pulumi.Output[int]:
         """
-        Specifies, in seconds, the frequency at which the system issues the monitor check when either the resource is down or the status of the resource is unknown. The default is `5`
+        Specifies, in seconds, the frequency at which the system issues the monitor check when either the resource is down or the status of the resource is unknown,value of `interval` should be always less than `timeout`. Default is `5`.
         """
         return pulumi.get(self, "interval")
 
     @property
     @pulumi.getter(name="ipDscp")
     def ip_dscp(self) -> pulumi.Output[int]:
         """
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/node.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -386,15 +387,16 @@
                  ratio: Optional[pulumi.Input[int]] = None,
                  session: Optional[pulumi.Input[str]] = None,
                  state: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         `ltm.Node` Manages a node configuration
 
-        For resources should be named with their "full path".The full path is the combination of the partition + name of the resource( example: /Common/my-node ) or partition + Direcroty + nameof the resource ( example: /Common/test/my-node ).When including directory in fullpath we have to make sure it is created in the given partition before using it.
+        For resources should be named with their `full path`.The full path is the combination of the `partition + name` of the resource( example: `/Common/my-node` ) or `partition + Direcroty + name` of the resource ( example: `/Common/test/my-node` ).
+        When including directory in `full path` we have to make sure it is created in the given partition before using it.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_f5bigip as f5bigip
 
@@ -430,15 +432,16 @@
     def __init__(__self__,
                  resource_name: str,
                  args: NodeArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         `ltm.Node` Manages a node configuration
 
-        For resources should be named with their "full path".The full path is the combination of the partition + name of the resource( example: /Common/my-node ) or partition + Direcroty + nameof the resource ( example: /Common/test/my-node ).When including directory in fullpath we have to make sure it is created in the given partition before using it.
+        For resources should be named with their `full path`.The full path is the combination of the `partition + name` of the resource( example: `/Common/my-node` ) or `partition + Direcroty + name` of the resource ( example: `/Common/test/my-node` ).
+        When including directory in `full path` we have to make sure it is created in the given partition before using it.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_f5bigip as f5bigip
 
@@ -479,20 +482,17 @@
                  monitor: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  rate_limit: Optional[pulumi.Input[str]] = None,
                  ratio: Optional[pulumi.Input[int]] = None,
                  session: Optional[pulumi.Input[str]] = None,
                  state: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = NodeArgs.__new__(NodeArgs)
 
             if address is None and not opts.urn:
                 raise TypeError("Missing required property 'address'")
@@ -640,13 +640,13 @@
         """
         Enables or disables the node for new sessions. The default value is user-enabled.
         """
         return pulumi.get(self, "session")
 
     @property
     @pulumi.getter
-    def state(self) -> pulumi.Output[Optional[str]]:
+    def state(self) -> pulumi.Output[str]:
         """
         Default is "user-up" you can set to "user-down" if you want to disable
         """
         return pulumi.get(self, "state")
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/outputs.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 
@@ -349,14 +350,15 @@
                  value: Optional[str] = None,
                  virtual: Optional[str] = None,
                  vlan: Optional[str] = None,
                  vlan_id: Optional[int] = None,
                  wam: Optional[bool] = None,
                  write: Optional[bool] = None):
         """
+        :param bool connection: This action is set to `true` by default, it needs to be explicitly set to `false` for actions it conflicts with.
         :param bool forward: This action will affect forwarding.
         :param str pool: This action will direct the stream to this pool.
         """
         if app_service is not None:
             pulumi.set(__self__, "app_service", app_service)
         if application is not None:
             pulumi.set(__self__, "application", application)
@@ -619,14 +621,17 @@
     @pulumi.getter
     def compress(self) -> Optional[bool]:
         return pulumi.get(self, "compress")
 
     @property
     @pulumi.getter
     def connection(self) -> Optional[bool]:
+        """
+        This action is set to `true` by default, it needs to be explicitly set to `false` for actions it conflicts with.
+        """
         return pulumi.get(self, "connection")
 
     @property
     @pulumi.getter
     def content(self) -> Optional[str]:
         return pulumi.get(self, "content")
 
@@ -1218,14 +1223,15 @@
                  country_name: Optional[bool] = None,
                  cpu_usage: Optional[bool] = None,
                  device_make: Optional[bool] = None,
                  device_model: Optional[bool] = None,
                  domain: Optional[bool] = None,
                  ends_with: Optional[bool] = None,
                  equals: Optional[bool] = None,
+                 exists: Optional[bool] = None,
                  expiry: Optional[bool] = None,
                  extension: Optional[bool] = None,
                  external: Optional[bool] = None,
                  geoip: Optional[bool] = None,
                  greater: Optional[bool] = None,
                  greater_or_equal: Optional[bool] = None,
                  host: Optional[bool] = None,
@@ -1330,14 +1336,16 @@
             pulumi.set(__self__, "device_model", device_model)
         if domain is not None:
             pulumi.set(__self__, "domain", domain)
         if ends_with is not None:
             pulumi.set(__self__, "ends_with", ends_with)
         if equals is not None:
             pulumi.set(__self__, "equals", equals)
+        if exists is not None:
+            pulumi.set(__self__, "exists", exists)
         if expiry is not None:
             pulumi.set(__self__, "expiry", expiry)
         if extension is not None:
             pulumi.set(__self__, "extension", extension)
         if external is not None:
             pulumi.set(__self__, "external", external)
         if geoip is not None:
@@ -1579,14 +1587,19 @@
     @property
     @pulumi.getter
     def equals(self) -> Optional[bool]:
         return pulumi.get(self, "equals")
 
     @property
     @pulumi.getter
+    def exists(self) -> Optional[bool]:
+        return pulumi.get(self, "exists")
+
+    @property
+    @pulumi.getter
     def expiry(self) -> Optional[bool]:
         return pulumi.get(self, "expiry")
 
     @property
     @pulumi.getter
     def extension(self) -> Optional[bool]:
         return pulumi.get(self, "extension")
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/persistence_profile_cookie.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/persistence_profile_cookie.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['PersistenceProfileCookieArgs', 'PersistenceProfileCookie']
@@ -801,20 +802,17 @@
                  match_across_virtuals: Optional[pulumi.Input[str]] = None,
                  method: Optional[pulumi.Input[str]] = None,
                  mirror: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  override_conn_limit: Optional[pulumi.Input[str]] = None,
                  timeout: Optional[pulumi.Input[int]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PersistenceProfileCookieArgs.__new__(PersistenceProfileCookieArgs)
 
             __props__.__dict__["always_send"] = always_send
             __props__.__dict__["app_service"] = app_service
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/persistence_profile_dst_addr.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/persistence_profile_dst_addr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['PersistenceProfileDstAddrArgs', 'PersistenceProfileDstAddr']
@@ -517,20 +518,17 @@
                  match_across_services: Optional[pulumi.Input[str]] = None,
                  match_across_virtuals: Optional[pulumi.Input[str]] = None,
                  mirror: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  override_conn_limit: Optional[pulumi.Input[str]] = None,
                  timeout: Optional[pulumi.Input[int]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PersistenceProfileDstAddrArgs.__new__(PersistenceProfileDstAddrArgs)
 
             __props__.__dict__["app_service"] = app_service
             if defaults_from is None and not opts.urn:
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/persistence_profile_src_addr.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/persistence_profile_src_addr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['PersistenceProfileSrcAddrArgs', 'PersistenceProfileSrcAddr']
@@ -566,20 +567,17 @@
                  match_across_services: Optional[pulumi.Input[str]] = None,
                  match_across_virtuals: Optional[pulumi.Input[str]] = None,
                  mirror: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  override_conn_limit: Optional[pulumi.Input[str]] = None,
                  timeout: Optional[pulumi.Input[int]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PersistenceProfileSrcAddrArgs.__new__(PersistenceProfileSrcAddrArgs)
 
             __props__.__dict__["app_service"] = app_service
             if defaults_from is None and not opts.urn:
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/persistence_profile_ssl.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/persistence_profile_ssl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['PersistenceProfileSslArgs', 'PersistenceProfileSsl']
@@ -438,20 +439,17 @@
                  match_across_services: Optional[pulumi.Input[str]] = None,
                  match_across_virtuals: Optional[pulumi.Input[str]] = None,
                  mirror: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  override_conn_limit: Optional[pulumi.Input[str]] = None,
                  timeout: Optional[pulumi.Input[int]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PersistenceProfileSslArgs.__new__(PersistenceProfileSslArgs)
 
             __props__.__dict__["app_service"] = app_service
             if defaults_from is None and not opts.urn:
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/policy.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -230,15 +231,15 @@
                  requires: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  rules: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PolicyRuleArgs']]]]] = None,
                  strategy: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         `ltm.Policy` Configures ltm policies to manage traffic assigned to a virtual server
 
-        For resources should be named with their "full path". The full path is the combination of the partition + name of the resource. For example /Common/my-pool.
+        For resources should be named with their `full path`. The full path is the combination of the `partition + name` of the resource. For example `/Common/test-policy`.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_f5bigip as f5bigip
 
@@ -252,14 +253,15 @@
             strategy="first-match",
             requires=["http"],
             controls=["forwarding"],
             rules=[f5bigip.ltm.PolicyRuleArgs(
                 name="rule6",
                 actions=[f5bigip.ltm.PolicyRuleActionArgs(
                     forward=True,
+                    connection=False,
                     pool=mypool.name,
                 )],
             )],
             opts=pulumi.ResourceOptions(depends_on=[mypool]))
         ```
 
         :param str resource_name: The name of the resource.
@@ -276,15 +278,15 @@
     def __init__(__self__,
                  resource_name: str,
                  args: PolicyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         `ltm.Policy` Configures ltm policies to manage traffic assigned to a virtual server
 
-        For resources should be named with their "full path". The full path is the combination of the partition + name of the resource. For example /Common/my-pool.
+        For resources should be named with their `full path`. The full path is the combination of the `partition + name` of the resource. For example `/Common/test-policy`.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_f5bigip as f5bigip
 
@@ -298,14 +300,15 @@
             strategy="first-match",
             requires=["http"],
             controls=["forwarding"],
             rules=[f5bigip.ltm.PolicyRuleArgs(
                 name="rule6",
                 actions=[f5bigip.ltm.PolicyRuleActionArgs(
                     forward=True,
+                    connection=False,
                     pool=mypool.name,
                 )],
             )],
             opts=pulumi.ResourceOptions(depends_on=[mypool]))
         ```
 
         :param str resource_name: The name of the resource.
@@ -326,20 +329,17 @@
                  controls: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  published_copy: Optional[pulumi.Input[str]] = None,
                  requires: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  rules: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PolicyRuleArgs']]]]] = None,
                  strategy: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PolicyArgs.__new__(PolicyArgs)
 
             __props__.__dict__["controls"] = controls
             if name is None and not opts.urn:
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/pool.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['PoolArgs', 'Pool']
@@ -21,15 +22,15 @@
                  minimum_active_members: Optional[pulumi.Input[int]] = None,
                  monitors: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  reselect_tries: Optional[pulumi.Input[int]] = None,
                  service_down_action: Optional[pulumi.Input[str]] = None,
                  slow_ramp_time: Optional[pulumi.Input[int]] = None):
         """
         The set of arguments for constructing a Pool resource.
-        :param pulumi.Input[str] name: Name of the pool,it should be "full path".The full path is the combination of the partition + name of the pool.(For example `/Common/my-pool`)
+        :param pulumi.Input[str] name: Name of the pool,it should be `full path`.The full path is the combination of the `partition + name` of the pool.(For example `/Common/my-pool`)
         :param pulumi.Input[str] allow_nat: Specifies whether NATs are automatically enabled or disabled for any connections using this pool, [ Default : `yes`, Possible Values `yes` or `no`].
         :param pulumi.Input[str] allow_snat: Specifies whether SNATs are automatically enabled or disabled for any connections using this pool,[ Default : `yes`, Possible Values `yes` or `no`].
         :param pulumi.Input[str] description: Specifies descriptive text that identifies the pool.
         :param pulumi.Input[str] load_balancing_mode: Specifies the load balancing method. The default is Round Robin.
         :param pulumi.Input[int] minimum_active_members: Specifies whether the system load balances traffic according to the priority number assigned to the pool member,Default Value is `0` meaning `disabled`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] monitors: List of monitor names to associate with the pool
         :param pulumi.Input[int] reselect_tries: Specifies the number of times the system tries to contact a new pool member after a passive failure.
@@ -56,15 +57,15 @@
         if slow_ramp_time is not None:
             pulumi.set(__self__, "slow_ramp_time", slow_ramp_time)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
         """
-        Name of the pool,it should be "full path".The full path is the combination of the partition + name of the pool.(For example `/Common/my-pool`)
+        Name of the pool,it should be `full path`.The full path is the combination of the `partition + name` of the pool.(For example `/Common/my-pool`)
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
@@ -194,15 +195,15 @@
         Input properties used for looking up and filtering Pool resources.
         :param pulumi.Input[str] allow_nat: Specifies whether NATs are automatically enabled or disabled for any connections using this pool, [ Default : `yes`, Possible Values `yes` or `no`].
         :param pulumi.Input[str] allow_snat: Specifies whether SNATs are automatically enabled or disabled for any connections using this pool,[ Default : `yes`, Possible Values `yes` or `no`].
         :param pulumi.Input[str] description: Specifies descriptive text that identifies the pool.
         :param pulumi.Input[str] load_balancing_mode: Specifies the load balancing method. The default is Round Robin.
         :param pulumi.Input[int] minimum_active_members: Specifies whether the system load balances traffic according to the priority number assigned to the pool member,Default Value is `0` meaning `disabled`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] monitors: List of monitor names to associate with the pool
-        :param pulumi.Input[str] name: Name of the pool,it should be "full path".The full path is the combination of the partition + name of the pool.(For example `/Common/my-pool`)
+        :param pulumi.Input[str] name: Name of the pool,it should be `full path`.The full path is the combination of the `partition + name` of the pool.(For example `/Common/my-pool`)
         :param pulumi.Input[int] reselect_tries: Specifies the number of times the system tries to contact a new pool member after a passive failure.
         :param pulumi.Input[str] service_down_action: Specifies how the system should respond when the target pool member becomes unavailable. The default is `None`, Possible values: `[none, reset, reselect, drop]`.
         :param pulumi.Input[int] slow_ramp_time: Specifies the duration during which the system sends less traffic to a newly-enabled pool member.
         """
         if allow_nat is not None:
             pulumi.set(__self__, "allow_nat", allow_nat)
         if allow_snat is not None:
@@ -296,15 +297,15 @@
     def monitors(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "monitors", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the pool,it should be "full path".The full path is the combination of the partition + name of the pool.(For example `/Common/my-pool`)
+        Name of the pool,it should be `full path`.The full path is the combination of the `partition + name` of the pool.(For example `/Common/my-pool`)
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -360,15 +361,16 @@
                  reselect_tries: Optional[pulumi.Input[int]] = None,
                  service_down_action: Optional[pulumi.Input[str]] = None,
                  slow_ramp_time: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         `ltm.Pool` Manages F5 BIG-IP LTM pools via iControl REST API.
 
-        Resources should be named with their "full path". The full path is the combination of the partition + name (example: /Common/my-pool ) or  partition + directory + name of the resource  (example: /Common/test/my-pool )
+        For resources should be named with their `full path`. The full path is the combination of the `partition + name` of the resource or  `partition + directory + name`.
+        For example `/Common/my-pool`.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_f5bigip as f5bigip
 
@@ -386,29 +388,30 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] allow_nat: Specifies whether NATs are automatically enabled or disabled for any connections using this pool, [ Default : `yes`, Possible Values `yes` or `no`].
         :param pulumi.Input[str] allow_snat: Specifies whether SNATs are automatically enabled or disabled for any connections using this pool,[ Default : `yes`, Possible Values `yes` or `no`].
         :param pulumi.Input[str] description: Specifies descriptive text that identifies the pool.
         :param pulumi.Input[str] load_balancing_mode: Specifies the load balancing method. The default is Round Robin.
         :param pulumi.Input[int] minimum_active_members: Specifies whether the system load balances traffic according to the priority number assigned to the pool member,Default Value is `0` meaning `disabled`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] monitors: List of monitor names to associate with the pool
-        :param pulumi.Input[str] name: Name of the pool,it should be "full path".The full path is the combination of the partition + name of the pool.(For example `/Common/my-pool`)
+        :param pulumi.Input[str] name: Name of the pool,it should be `full path`.The full path is the combination of the `partition + name` of the pool.(For example `/Common/my-pool`)
         :param pulumi.Input[int] reselect_tries: Specifies the number of times the system tries to contact a new pool member after a passive failure.
         :param pulumi.Input[str] service_down_action: Specifies how the system should respond when the target pool member becomes unavailable. The default is `None`, Possible values: `[none, reset, reselect, drop]`.
         :param pulumi.Input[int] slow_ramp_time: Specifies the duration during which the system sends less traffic to a newly-enabled pool member.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: PoolArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         `ltm.Pool` Manages F5 BIG-IP LTM pools via iControl REST API.
 
-        Resources should be named with their "full path". The full path is the combination of the partition + name (example: /Common/my-pool ) or  partition + directory + name of the resource  (example: /Common/test/my-pool )
+        For resources should be named with their `full path`. The full path is the combination of the `partition + name` of the resource or  `partition + directory + name`.
+        For example `/Common/my-pool`.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_f5bigip as f5bigip
 
@@ -444,20 +447,17 @@
                  minimum_active_members: Optional[pulumi.Input[int]] = None,
                  monitors: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  reselect_tries: Optional[pulumi.Input[int]] = None,
                  service_down_action: Optional[pulumi.Input[str]] = None,
                  slow_ramp_time: Optional[pulumi.Input[int]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PoolArgs.__new__(PoolArgs)
 
             __props__.__dict__["allow_nat"] = allow_nat
             __props__.__dict__["allow_snat"] = allow_snat
@@ -500,15 +500,15 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] allow_nat: Specifies whether NATs are automatically enabled or disabled for any connections using this pool, [ Default : `yes`, Possible Values `yes` or `no`].
         :param pulumi.Input[str] allow_snat: Specifies whether SNATs are automatically enabled or disabled for any connections using this pool,[ Default : `yes`, Possible Values `yes` or `no`].
         :param pulumi.Input[str] description: Specifies descriptive text that identifies the pool.
         :param pulumi.Input[str] load_balancing_mode: Specifies the load balancing method. The default is Round Robin.
         :param pulumi.Input[int] minimum_active_members: Specifies whether the system load balances traffic according to the priority number assigned to the pool member,Default Value is `0` meaning `disabled`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] monitors: List of monitor names to associate with the pool
-        :param pulumi.Input[str] name: Name of the pool,it should be "full path".The full path is the combination of the partition + name of the pool.(For example `/Common/my-pool`)
+        :param pulumi.Input[str] name: Name of the pool,it should be `full path`.The full path is the combination of the `partition + name` of the pool.(For example `/Common/my-pool`)
         :param pulumi.Input[int] reselect_tries: Specifies the number of times the system tries to contact a new pool member after a passive failure.
         :param pulumi.Input[str] service_down_action: Specifies how the system should respond when the target pool member becomes unavailable. The default is `None`, Possible values: `[none, reset, reselect, drop]`.
         :param pulumi.Input[int] slow_ramp_time: Specifies the duration during which the system sends less traffic to a newly-enabled pool member.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _PoolState.__new__(_PoolState)
@@ -573,15 +573,15 @@
         """
         return pulumi.get(self, "monitors")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        Name of the pool,it should be "full path".The full path is the combination of the partition + name of the pool.(For example `/Common/my-pool`)
+        Name of the pool,it should be `full path`.The full path is the combination of the `partition + name` of the pool.(For example `/Common/my-pool`)
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="reselectTries")
     def reselect_tries(self) -> pulumi.Output[int]:
         """
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/pool_attachment.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/pool_attachment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['PoolAttachmentArgs', 'PoolAttachment']
@@ -305,15 +306,15 @@
         ```python
         import pulumi
         import pulumi_f5bigip as f5bigip
 
         monitor = f5bigip.ltm.Monitor("monitor",
             name="/Common/terraform_monitor",
             parent="/Common/http",
-            send="GET /some/path\n",
+            send="GET /some/path\\n",
             timeout=999,
             interval=998)
         pool = f5bigip.ltm.Pool("pool",
             name="/Common/terraform-pool",
             load_balancing_mode="round-robin",
             monitors=[monitor.name],
             allow_snat="yes",
@@ -327,15 +328,15 @@
         ```python
         import pulumi
         import pulumi_f5bigip as f5bigip
 
         monitor = f5bigip.ltm.Monitor("monitor",
             name="/Common/terraform_monitor",
             parent="/Common/http",
-            send="GET /some/path\n",
+            send="GET /some/path\\n",
             timeout=999,
             interval=998)
         pool = f5bigip.ltm.Pool("pool",
             name="/Common/terraform-pool",
             load_balancing_mode="round-robin",
             monitors=[monitor.name],
             allow_snat="yes",
@@ -376,15 +377,15 @@
         ```python
         import pulumi
         import pulumi_f5bigip as f5bigip
 
         monitor = f5bigip.ltm.Monitor("monitor",
             name="/Common/terraform_monitor",
             parent="/Common/http",
-            send="GET /some/path\n",
+            send="GET /some/path\\n",
             timeout=999,
             interval=998)
         pool = f5bigip.ltm.Pool("pool",
             name="/Common/terraform-pool",
             load_balancing_mode="round-robin",
             monitors=[monitor.name],
             allow_snat="yes",
@@ -398,15 +399,15 @@
         ```python
         import pulumi
         import pulumi_f5bigip as f5bigip
 
         monitor = f5bigip.ltm.Monitor("monitor",
             name="/Common/terraform_monitor",
             parent="/Common/http",
-            send="GET /some/path\n",
+            send="GET /some/path\\n",
             timeout=999,
             interval=998)
         pool = f5bigip.ltm.Pool("pool",
             name="/Common/terraform-pool",
             load_balancing_mode="round-robin",
             monitors=[monitor.name],
             allow_snat="yes",
@@ -439,20 +440,17 @@
                  dynamic_ratio: Optional[pulumi.Input[int]] = None,
                  fqdn_autopopulate: Optional[pulumi.Input[str]] = None,
                  node: Optional[pulumi.Input[str]] = None,
                  pool: Optional[pulumi.Input[str]] = None,
                  priority_group: Optional[pulumi.Input[int]] = None,
                  ratio: Optional[pulumi.Input[int]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PoolAttachmentArgs.__new__(PoolAttachmentArgs)
 
             __props__.__dict__["connection_limit"] = connection_limit
             __props__.__dict__["connection_rate_limit"] = connection_rate_limit
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/profile_client_ssl.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/profile_client_ssl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -2036,20 +2037,17 @@
                  ssl_forward_proxy: Optional[pulumi.Input[str]] = None,
                  ssl_forward_proxy_bypass: Optional[pulumi.Input[str]] = None,
                  ssl_sign_hash: Optional[pulumi.Input[str]] = None,
                  strict_resume: Optional[pulumi.Input[str]] = None,
                  tm_options: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  unclean_shutdown: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProfileClientSslArgs.__new__(ProfileClientSslArgs)
 
             __props__.__dict__["alert_timeout"] = alert_timeout
             __props__.__dict__["allow_non_ssl"] = allow_non_ssl
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/profile_fast_http.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/profile_fast_http.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['ProfileFastHttpArgs', 'ProfileFastHttp']
@@ -487,20 +488,17 @@
                  connpoolidle_timeoutoverride: Optional[pulumi.Input[int]] = None,
                  defaults_from: Optional[pulumi.Input[str]] = None,
                  forcehttp10response: Optional[pulumi.Input[str]] = None,
                  idle_timeout: Optional[pulumi.Input[int]] = None,
                  maxheader_size: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProfileFastHttpArgs.__new__(ProfileFastHttpArgs)
 
             __props__.__dict__["connpool_maxreuse"] = connpool_maxreuse
             __props__.__dict__["connpool_maxsize"] = connpool_maxsize
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/profile_fast_l4.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/profile_fast_l4.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['ProfileFastL4Args', 'ProfileFastL4']
@@ -464,20 +465,17 @@
                  idle_timeout: Optional[pulumi.Input[str]] = None,
                  iptos_toclient: Optional[pulumi.Input[str]] = None,
                  iptos_toserver: Optional[pulumi.Input[str]] = None,
                  keepalive_interval: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  partition: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProfileFastL4Args.__new__(ProfileFastL4Args)
 
             __props__.__dict__["client_timeout"] = client_timeout
             __props__.__dict__["defaults_from"] = defaults_from
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/profile_ftp.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/profile_ftp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['ProfileFtpArgs', 'ProfileFtp']
@@ -720,20 +721,17 @@
                  log_publisher: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  partition: Optional[pulumi.Input[str]] = None,
                  port: Optional[pulumi.Input[int]] = None,
                  security: Optional[pulumi.Input[str]] = None,
                  translate_extended: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProfileFtpArgs.__new__(ProfileFtpArgs)
 
             __props__.__dict__["allow_active_mode"] = allow_active_mode
             __props__.__dict__["allow_ftps"] = allow_ftps
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/profile_http.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/profile_http.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['ProfileHttpArgs', 'ProfileHttp']
@@ -1067,20 +1068,17 @@
                  server_agent_name: Optional[pulumi.Input[str]] = None,
                  tm_partition: Optional[pulumi.Input[str]] = None,
                  via_host_name: Optional[pulumi.Input[str]] = None,
                  via_request: Optional[pulumi.Input[str]] = None,
                  via_response: Optional[pulumi.Input[str]] = None,
                  xff_alternative_names: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProfileHttpArgs.__new__(ProfileHttpArgs)
 
             __props__.__dict__["accept_xff"] = accept_xff
             __props__.__dict__["app_service"] = app_service
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/profile_http2.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/profile_http2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['ProfileHttp2Args', 'ProfileHttp2']
@@ -565,20 +566,17 @@
                  include_content_length: Optional[pulumi.Input[str]] = None,
                  insert_header: Optional[pulumi.Input[str]] = None,
                  insert_header_name: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  receive_window: Optional[pulumi.Input[int]] = None,
                  write_size: Optional[pulumi.Input[int]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProfileHttp2Args.__new__(ProfileHttp2Args)
 
             __props__.__dict__["activation_modes"] = activation_modes
             __props__.__dict__["concurrent_streams_per_connection"] = concurrent_streams_per_connection
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/profile_http_compress.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/profile_http_compress.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['ProfileHttpCompressArgs', 'ProfileHttpCompress']
@@ -308,20 +309,17 @@
                  content_type_excludes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  content_type_includes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  defaults_from: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  uri_excludes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  uri_includes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProfileHttpCompressArgs.__new__(ProfileHttpCompressArgs)
 
             __props__.__dict__["content_type_excludes"] = content_type_excludes
             __props__.__dict__["content_type_includes"] = content_type_includes
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/profile_one_connect.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/profile_one_connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['ProfileOneConnectArgs', 'ProfileOneConnect']
@@ -446,20 +447,17 @@
                  max_reuse: Optional[pulumi.Input[int]] = None,
                  max_size: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  partition: Optional[pulumi.Input[str]] = None,
                  share_pools: Optional[pulumi.Input[str]] = None,
                  source_mask: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProfileOneConnectArgs.__new__(ProfileOneConnectArgs)
 
             __props__.__dict__["defaults_from"] = defaults_from
             __props__.__dict__["idle_timeout_override"] = idle_timeout_override
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/profile_server_ssl.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/profile_server_ssl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['ProfileServerSslArgs', 'ProfileServerSsl']
@@ -1873,20 +1874,17 @@
                  ssl_forward_proxy_bypass: Optional[pulumi.Input[str]] = None,
                  ssl_sign_hash: Optional[pulumi.Input[str]] = None,
                  strict_resume: Optional[pulumi.Input[str]] = None,
                  tm_options: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  unclean_shutdown: Optional[pulumi.Input[str]] = None,
                  untrusted_cert_response_control: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProfileServerSslArgs.__new__(ProfileServerSslArgs)
 
             __props__.__dict__["alert_timeout"] = alert_timeout
             __props__.__dict__["authenticate"] = authenticate
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/profile_tcp.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/profile_tcp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['ProfileTcpArgs', 'ProfileTcp']
@@ -446,20 +447,17 @@
                  finwait2timeout: Optional[pulumi.Input[int]] = None,
                  finwait_timeout: Optional[pulumi.Input[int]] = None,
                  idle_timeout: Optional[pulumi.Input[int]] = None,
                  keepalive_interval: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  partition: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProfileTcpArgs.__new__(ProfileTcpArgs)
 
             __props__.__dict__["close_wait_timeout"] = close_wait_timeout
             __props__.__dict__["defaults_from"] = defaults_from
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/snat.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/snat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -482,20 +483,17 @@
                  partition: Optional[pulumi.Input[str]] = None,
                  snatpool: Optional[pulumi.Input[str]] = None,
                  sourceport: Optional[pulumi.Input[str]] = None,
                  translation: Optional[pulumi.Input[str]] = None,
                  vlans: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  vlansdisabled: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = SnatArgs.__new__(SnatArgs)
 
             __props__.__dict__["autolasthop"] = autolasthop
             __props__.__dict__["full_path"] = full_path
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/snat_pool.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/snat_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['SnatPoolArgs', 'SnatPool']
@@ -159,20 +160,17 @@
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  members: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = SnatPoolArgs.__new__(SnatPoolArgs)
 
             if members is None and not opts.urn:
                 raise TypeError("Missing required property 'members'")
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/virtual_address.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/virtual_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['VirtualAddressArgs', 'VirtualAddress']
@@ -364,20 +365,17 @@
                  auto_delete: Optional[pulumi.Input[bool]] = None,
                  conn_limit: Optional[pulumi.Input[int]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  icmp_echo: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  traffic_group: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = VirtualAddressArgs.__new__(VirtualAddressArgs)
 
             __props__.__dict__["advertize_route"] = advertize_route
             __props__.__dict__["arp"] = arp
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ltm/virtual_server.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ltm/virtual_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['VirtualServerArgs', 'VirtualServer']
@@ -833,15 +834,16 @@
                  translate_port: Optional[pulumi.Input[str]] = None,
                  vlans: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  vlans_enabled: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         `ltm.VirtualServer` Configures Virtual Server
 
-        For resources should be named with their "full path". The full path is the combination of the partition + name of the resource (example: /Common/my-pool ) or partition + directory + name of the resource (example: /Common/test/my-pool ).When including directory in fullpath we have to make sure it is created in the given partition before using it.
+        For resources should be named with their `full path`. The full path is the combination of the `partition + name` of the resource (example: `/Common/test-virtualserver` ) or `partition + directory + name` of the resource (example: `/Common/test/test-virtualserver` ).
+        When including directory in `fullpath` we have to make sure it is created in the given partition before using it.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_f5bigip as f5bigip
 
@@ -908,15 +910,16 @@
     def __init__(__self__,
                  resource_name: str,
                  args: VirtualServerArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         `ltm.VirtualServer` Configures Virtual Server
 
-        For resources should be named with their "full path". The full path is the combination of the partition + name of the resource (example: /Common/my-pool ) or partition + directory + name of the resource (example: /Common/test/my-pool ).When including directory in fullpath we have to make sure it is created in the given partition before using it.
+        For resources should be named with their `full path`. The full path is the combination of the `partition + name` of the resource (example: `/Common/test-virtualserver` ) or `partition + directory + name` of the resource (example: `/Common/test/test-virtualserver` ).
+        When including directory in `fullpath` we have to make sure it is created in the given partition before using it.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_f5bigip as f5bigip
 
@@ -989,20 +992,17 @@
                  source_address_translation: Optional[pulumi.Input[str]] = None,
                  state: Optional[pulumi.Input[str]] = None,
                  translate_address: Optional[pulumi.Input[str]] = None,
                  translate_port: Optional[pulumi.Input[str]] = None,
                  vlans: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  vlans_enabled: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = VirtualServerArgs.__new__(VirtualServerArgs)
 
             __props__.__dict__["client_profiles"] = client_profiles
             __props__.__dict__["default_persistence_profile"] = default_persistence_profile
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/net/_inputs.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/net/_inputs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/net/outputs.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/net/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/net/route.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/net/route.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['RouteArgs', 'Route']
@@ -260,20 +261,17 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  gw: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  network: Optional[pulumi.Input[str]] = None,
                  reject: Optional[pulumi.Input[bool]] = None,
                  tunnel_ref: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RouteArgs.__new__(RouteArgs)
 
             __props__.__dict__["gw"] = gw
             if name is None and not opts.urn:
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/net/self_ip.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/net/self_ip.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['SelfIpArgs', 'SelfIp']
@@ -16,15 +17,15 @@
                  ip: pulumi.Input[str],
                  name: pulumi.Input[str],
                  vlan: pulumi.Input[str],
                  port_lockdowns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  traffic_group: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a SelfIp resource.
-        :param pulumi.Input[str] ip: The Self IP's address and netmask.
+        :param pulumi.Input[str] ip: The Self IP's address and netmask. The IP address could also contain the route domain, e.g. `10.12.13.14%4/24`.
         :param pulumi.Input[str] name: Name of the selfip
         :param pulumi.Input[str] vlan: Specifies the VLAN for which you are setting a self IP address. This setting must be provided when a self IP is created.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] port_lockdowns: Specifies the port lockdown, defaults to `Allow None` if not specified.
         :param pulumi.Input[str] traffic_group: Specifies the traffic group, defaults to `traffic-group-local-only` if not specified.
         """
         pulumi.set(__self__, "ip", ip)
         pulumi.set(__self__, "name", name)
@@ -34,15 +35,15 @@
         if traffic_group is not None:
             pulumi.set(__self__, "traffic_group", traffic_group)
 
     @property
     @pulumi.getter
     def ip(self) -> pulumi.Input[str]:
         """
-        The Self IP's address and netmask.
+        The Self IP's address and netmask. The IP address could also contain the route domain, e.g. `10.12.13.14%4/24`.
         """
         return pulumi.get(self, "ip")
 
     @ip.setter
     def ip(self, value: pulumi.Input[str]):
         pulumi.set(self, "ip", value)
 
@@ -101,15 +102,15 @@
                  ip: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  port_lockdowns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  traffic_group: Optional[pulumi.Input[str]] = None,
                  vlan: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering SelfIp resources.
-        :param pulumi.Input[str] ip: The Self IP's address and netmask.
+        :param pulumi.Input[str] ip: The Self IP's address and netmask. The IP address could also contain the route domain, e.g. `10.12.13.14%4/24`.
         :param pulumi.Input[str] name: Name of the selfip
         :param pulumi.Input[Sequence[pulumi.Input[str]]] port_lockdowns: Specifies the port lockdown, defaults to `Allow None` if not specified.
         :param pulumi.Input[str] traffic_group: Specifies the traffic group, defaults to `traffic-group-local-only` if not specified.
         :param pulumi.Input[str] vlan: Specifies the VLAN for which you are setting a self IP address. This setting must be provided when a self IP is created.
         """
         if ip is not None:
             pulumi.set(__self__, "ip", ip)
@@ -122,15 +123,15 @@
         if vlan is not None:
             pulumi.set(__self__, "vlan", vlan)
 
     @property
     @pulumi.getter
     def ip(self) -> Optional[pulumi.Input[str]]:
         """
-        The Self IP's address and netmask.
+        The Self IP's address and netmask. The IP address could also contain the route domain, e.g. `10.12.13.14%4/24`.
         """
         return pulumi.get(self, "ip")
 
     @ip.setter
     def ip(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ip", value)
 
@@ -246,18 +247,32 @@
             name="/Common/internalselfIP",
             ip="11.1.1.1/24",
             vlan="/Common/internal",
             traffic_group="traffic-group-1",
             port_lockdowns=["none"],
             opts=pulumi.ResourceOptions(depends_on=[bigip_net_vlan["vlan1"]]))
         ```
+        ### Example usage with route domain embedded in the `ip`
+
+        ```python
+        import pulumi
+        import pulumi_f5bigip as f5bigip
+
+        selfip1 = f5bigip.net.SelfIp("selfip1",
+            name="/Common/internalselfIP",
+            ip="11.1.1.1%4/24",
+            vlan="/Common/internal",
+            traffic_group="traffic-group-1",
+            port_lockdowns=["none"],
+            opts=pulumi.ResourceOptions(depends_on=[bigip_net_vlan["vlan1"]]))
+        ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] ip: The Self IP's address and netmask.
+        :param pulumi.Input[str] ip: The Self IP's address and netmask. The IP address could also contain the route domain, e.g. `10.12.13.14%4/24`.
         :param pulumi.Input[str] name: Name of the selfip
         :param pulumi.Input[Sequence[pulumi.Input[str]]] port_lockdowns: Specifies the port lockdown, defaults to `Allow None` if not specified.
         :param pulumi.Input[str] traffic_group: Specifies the traffic group, defaults to `traffic-group-local-only` if not specified.
         :param pulumi.Input[str] vlan: Specifies the VLAN for which you are setting a self IP address. This setting must be provided when a self IP is created.
         """
         ...
     @overload
@@ -317,14 +332,28 @@
             name="/Common/internalselfIP",
             ip="11.1.1.1/24",
             vlan="/Common/internal",
             traffic_group="traffic-group-1",
             port_lockdowns=["none"],
             opts=pulumi.ResourceOptions(depends_on=[bigip_net_vlan["vlan1"]]))
         ```
+        ### Example usage with route domain embedded in the `ip`
+
+        ```python
+        import pulumi
+        import pulumi_f5bigip as f5bigip
+
+        selfip1 = f5bigip.net.SelfIp("selfip1",
+            name="/Common/internalselfIP",
+            ip="11.1.1.1%4/24",
+            vlan="/Common/internal",
+            traffic_group="traffic-group-1",
+            port_lockdowns=["none"],
+            opts=pulumi.ResourceOptions(depends_on=[bigip_net_vlan["vlan1"]]))
+        ```
 
         :param str resource_name: The name of the resource.
         :param SelfIpArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
@@ -339,20 +368,17 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  ip: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  port_lockdowns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  traffic_group: Optional[pulumi.Input[str]] = None,
                  vlan: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = SelfIpArgs.__new__(SelfIpArgs)
 
             if ip is None and not opts.urn:
                 raise TypeError("Missing required property 'ip'")
@@ -383,15 +409,15 @@
         """
         Get an existing SelfIp resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] ip: The Self IP's address and netmask.
+        :param pulumi.Input[str] ip: The Self IP's address and netmask. The IP address could also contain the route domain, e.g. `10.12.13.14%4/24`.
         :param pulumi.Input[str] name: Name of the selfip
         :param pulumi.Input[Sequence[pulumi.Input[str]]] port_lockdowns: Specifies the port lockdown, defaults to `Allow None` if not specified.
         :param pulumi.Input[str] traffic_group: Specifies the traffic group, defaults to `traffic-group-local-only` if not specified.
         :param pulumi.Input[str] vlan: Specifies the VLAN for which you are setting a self IP address. This setting must be provided when a self IP is created.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
@@ -404,15 +430,15 @@
         __props__.__dict__["vlan"] = vlan
         return SelfIp(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def ip(self) -> pulumi.Output[str]:
         """
-        The Self IP's address and netmask.
+        The Self IP's address and netmask. The IP address could also contain the route domain, e.g. `10.12.13.14%4/24`.
         """
         return pulumi.get(self, "ip")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/net/vlan.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/net/vlan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -199,20 +200,17 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  interfaces: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VlanInterfaceArgs']]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  tag: Optional[pulumi.Input[int]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = VlanArgs.__new__(VlanArgs)
 
             __props__.__dict__["interfaces"] = interfaces
             if name is None and not opts.urn:
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/net_ike_peer.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/net_ike_peer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['NetIkePeerArgs', 'NetIkePeer']
@@ -1247,20 +1248,17 @@
                  remote_address: Optional[pulumi.Input[str]] = None,
                  replay_window_size: Optional[pulumi.Input[int]] = None,
                  state: Optional[pulumi.Input[str]] = None,
                  traffic_selectors: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  verify_cert: Optional[pulumi.Input[str]] = None,
                  versions: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = NetIkePeerArgs.__new__(NetIkePeerArgs)
 
             __props__.__dict__["app_service"] = app_service
             __props__.__dict__["ca_cert_file"] = ca_cert_file
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/net_tunnel.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/net_tunnel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['NetTunnelArgs', 'NetTunnel']
@@ -675,20 +676,17 @@
                  remote_address: Optional[pulumi.Input[str]] = None,
                  secondary_address: Optional[pulumi.Input[str]] = None,
                  tos: Optional[pulumi.Input[str]] = None,
                  traffic_group: Optional[pulumi.Input[str]] = None,
                  transparent: Optional[pulumi.Input[str]] = None,
                  use_pmtu: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = NetTunnelArgs.__new__(NetTunnelArgs)
 
             __props__.__dict__["app_service"] = app_service
             __props__.__dict__["auto_last_hop"] = auto_last_hop
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/provider.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['ProviderArgs', 'Provider']
@@ -209,20 +210,17 @@
                  password: Optional[pulumi.Input[str]] = None,
                  port: Optional[pulumi.Input[str]] = None,
                  teem_disable: Optional[pulumi.Input[bool]] = None,
                  token_auth: Optional[pulumi.Input[bool]] = None,
                  token_value: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProviderArgs.__new__(ProviderArgs)
 
             __props__.__dict__["address"] = address
             __props__.__dict__["login_ref"] = login_ref
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ssl/__init__.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ssl/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ssl/_inputs.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ssl/_inputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ssl/certificate.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ssl/certificate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['CertificateArgs', 'Certificate']
@@ -223,20 +224,17 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  content: Optional[pulumi.Input[str]] = None,
                  full_path: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  partition: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = CertificateArgs.__new__(CertificateArgs)
 
             if content is None and not opts.urn:
                 raise TypeError("Missing required property 'content'")
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ssl/get_certificate.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ssl/get_certificate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -96,18 +97,15 @@
 
     :param str name: Name of the ssl_certificate
     :param str partition: partition of the ltm ssl_certificate
     """
     __args__ = dict()
     __args__['name'] = name
     __args__['partition'] = partition
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('f5bigip:ssl/getCertificate:getCertificate', __args__, opts=opts, typ=GetCertificateResult).value
 
     return AwaitableGetCertificateResult(
         certificate=__ret__.certificate,
         id=__ret__.id,
         name=__ret__.name,
         partition=__ret__.partition)
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ssl/get_v_wan_config.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ssl/get_v_wan_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -166,18 +167,15 @@
     :param str azure_vwan_resourcegroup: Name of the Azure vWAN resource group
     :param str azure_vwan_vpnsite: Name of the Azure vWAN VPN site from which configuration to be download
     """
     __args__ = dict()
     __args__['azureVwanName'] = azure_vwan_name
     __args__['azureVwanResourcegroup'] = azure_vwan_resourcegroup
     __args__['azureVwanVpnsite'] = azure_vwan_vpnsite
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('f5bigip:ssl/getVWanConfig:getVWanConfig', __args__, opts=opts, typ=GetVWanConfigResult).value
 
     return AwaitableGetVWanConfigResult(
         azure_vwan_name=__ret__.azure_vwan_name,
         azure_vwan_resourcegroup=__ret__.azure_vwan_resourcegroup,
         azure_vwan_vpnsite=__ret__.azure_vwan_vpnsite,
         bigip_gw_ip=__ret__.bigip_gw_ip,
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ssl/get_waf_entity_parameter.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ssl/get_waf_entity_parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -286,18 +287,15 @@
     __args__['name'] = name
     __args__['parameterLocation'] = parameter_location
     __args__['performStaging'] = perform_staging
     __args__['sensitiveParameter'] = sensitive_parameter
     __args__['signatureOverridesDisables'] = signature_overrides_disables
     __args__['type'] = type
     __args__['valueType'] = value_type
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('f5bigip:ssl/getWafEntityParameter:getWafEntityParameter', __args__, opts=opts, typ=GetWafEntityParameterResult).value
 
     return AwaitableGetWafEntityParameterResult(
         allow_empty_type=__ret__.allow_empty_type,
         allow_repeated_parameter_name=__ret__.allow_repeated_parameter_name,
         attack_signatures_check=__ret__.attack_signatures_check,
         check_max_value_length=__ret__.check_max_value_length,
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ssl/get_waf_entity_url.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ssl/get_waf_entity_url.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -183,18 +184,15 @@
     __args__['method'] = method
     __args__['methodOverrides'] = method_overrides
     __args__['name'] = name
     __args__['performStaging'] = perform_staging
     __args__['protocol'] = protocol
     __args__['signatureOverridesDisables'] = signature_overrides_disables
     __args__['type'] = type
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('f5bigip:ssl/getWafEntityUrl:getWafEntityUrl', __args__, opts=opts, typ=GetWafEntityUrlResult).value
 
     return AwaitableGetWafEntityUrlResult(
         description=__ret__.description,
         id=__ret__.id,
         json=__ret__.json,
         method=__ret__.method,
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ssl/get_waf_pb_suggestions.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ssl/get_waf_pb_suggestions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -120,18 +121,15 @@
     :param str policy_name: WAF policy name from which PB suggestions should be exported.
     """
     __args__ = dict()
     __args__['minimumLearningScore'] = minimum_learning_score
     __args__['partition'] = partition
     __args__['policyId'] = policy_id
     __args__['policyName'] = policy_name
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('f5bigip:ssl/getWafPbSuggestions:getWafPbSuggestions', __args__, opts=opts, typ=GetWafPbSuggestionsResult).value
 
     return AwaitableGetWafPbSuggestionsResult(
         id=__ret__.id,
         json=__ret__.json,
         minimum_learning_score=__ret__.minimum_learning_score,
         partition=__ret__.partition,
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ssl/get_waf_policy.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ssl/get_waf_policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -82,18 +83,15 @@
 
     :param str policy_id: ID of the WAF policy deployed in the BIG-IP.
     :param str policy_json: Exported WAF policy JSON
     """
     __args__ = dict()
     __args__['policyId'] = policy_id
     __args__['policyJson'] = policy_json
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('f5bigip:ssl/getWafPolicy:getWafPolicy', __args__, opts=opts, typ=GetWafPolicyResult).value
 
     return AwaitableGetWafPolicyResult(
         id=__ret__.id,
         policy_id=__ret__.policy_id,
         policy_json=__ret__.policy_json)
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ssl/get_waf_signatures.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ssl/get_waf_signatures.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -16,73 +17,100 @@
 ]
 
 @pulumi.output_type
 class GetWafSignaturesResult:
     """
     A collection of values returned by getWafSignatures.
     """
-    def __init__(__self__, accuracy=None, description=None, id=None, name=None, risk=None, signature_id=None, system_signature_id=None, type=None):
+    def __init__(__self__, accuracy=None, description=None, enabled=None, id=None, json=None, name=None, perform_staging=None, risk=None, signature_id=None, system_signature_id=None, tag=None, type=None):
         if accuracy and not isinstance(accuracy, str):
             raise TypeError("Expected argument 'accuracy' to be a str")
         pulumi.set(__self__, "accuracy", accuracy)
         if description and not isinstance(description, str):
             raise TypeError("Expected argument 'description' to be a str")
         pulumi.set(__self__, "description", description)
+        if enabled and not isinstance(enabled, bool):
+            raise TypeError("Expected argument 'enabled' to be a bool")
+        pulumi.set(__self__, "enabled", enabled)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
+        if json and not isinstance(json, str):
+            raise TypeError("Expected argument 'json' to be a str")
+        pulumi.set(__self__, "json", json)
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
+        if perform_staging and not isinstance(perform_staging, bool):
+            raise TypeError("Expected argument 'perform_staging' to be a bool")
+        pulumi.set(__self__, "perform_staging", perform_staging)
         if risk and not isinstance(risk, str):
             raise TypeError("Expected argument 'risk' to be a str")
         pulumi.set(__self__, "risk", risk)
         if signature_id and not isinstance(signature_id, int):
             raise TypeError("Expected argument 'signature_id' to be a int")
         pulumi.set(__self__, "signature_id", signature_id)
         if system_signature_id and not isinstance(system_signature_id, str):
             raise TypeError("Expected argument 'system_signature_id' to be a str")
         pulumi.set(__self__, "system_signature_id", system_signature_id)
+        if tag and not isinstance(tag, str):
+            raise TypeError("Expected argument 'tag' to be a str")
+        pulumi.set(__self__, "tag", tag)
         if type and not isinstance(type, str):
             raise TypeError("Expected argument 'type' to be a str")
         pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
     def accuracy(self) -> str:
         """
         The relative detection accuracy of the signature.
         """
         return pulumi.get(self, "accuracy")
 
     @property
     @pulumi.getter
-    def description(self) -> str:
+    def description(self) -> Optional[str]:
         """
         Description of the signature.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
+    def enabled(self) -> Optional[bool]:
+        return pulumi.get(self, "enabled")
+
+    @property
+    @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
+    def json(self) -> str:
+        return pulumi.get(self, "json")
+
+    @property
+    @pulumi.getter
     def name(self) -> str:
         """
         Name of the signature as configured on the system.
         """
         return pulumi.get(self, "name")
 
     @property
+    @pulumi.getter(name="performStaging")
+    def perform_staging(self) -> Optional[bool]:
+        return pulumi.get(self, "perform_staging")
+
+    @property
     @pulumi.getter
     def risk(self) -> str:
         """
         The relative risk level of the attack that matches this signature.
         """
         return pulumi.get(self, "risk")
 
@@ -100,14 +128,19 @@
         """
         System generated ID of the signature.
         """
         return pulumi.get(self, "system_signature_id")
 
     @property
     @pulumi.getter
+    def tag(self) -> str:
+        return pulumi.get(self, "tag")
+
+    @property
+    @pulumi.getter
     def type(self) -> str:
         """
         Type of the signature.
         """
         return pulumi.get(self, "type")
 
 
@@ -115,28 +148,35 @@
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetWafSignaturesResult(
             accuracy=self.accuracy,
             description=self.description,
+            enabled=self.enabled,
             id=self.id,
+            json=self.json,
             name=self.name,
+            perform_staging=self.perform_staging,
             risk=self.risk,
             signature_id=self.signature_id,
             system_signature_id=self.system_signature_id,
+            tag=self.tag,
             type=self.type)
 
 
 def get_waf_signatures(accuracy: Optional[str] = None,
                        description: Optional[str] = None,
+                       enabled: Optional[bool] = None,
                        name: Optional[str] = None,
+                       perform_staging: Optional[bool] = None,
                        risk: Optional[str] = None,
                        signature_id: Optional[int] = None,
                        system_signature_id: Optional[str] = None,
+                       tag: Optional[str] = None,
                        type: Optional[str] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetWafSignaturesResult:
     """
     Use this data source (`ssl.get_waf_signatures`) to get the details of attack signatures available on BIG-IP WAF
 
     ## Example Usage
 
@@ -155,43 +195,50 @@
     :param int signature_id: ID of the signature in the BIG-IP WAF database.
     :param str system_signature_id: System generated ID of the signature.
     :param str type: Type of the signature.
     """
     __args__ = dict()
     __args__['accuracy'] = accuracy
     __args__['description'] = description
+    __args__['enabled'] = enabled
     __args__['name'] = name
+    __args__['performStaging'] = perform_staging
     __args__['risk'] = risk
     __args__['signatureId'] = signature_id
     __args__['systemSignatureId'] = system_signature_id
+    __args__['tag'] = tag
     __args__['type'] = type
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('f5bigip:ssl/getWafSignatures:getWafSignatures', __args__, opts=opts, typ=GetWafSignaturesResult).value
 
     return AwaitableGetWafSignaturesResult(
         accuracy=__ret__.accuracy,
         description=__ret__.description,
+        enabled=__ret__.enabled,
         id=__ret__.id,
+        json=__ret__.json,
         name=__ret__.name,
+        perform_staging=__ret__.perform_staging,
         risk=__ret__.risk,
         signature_id=__ret__.signature_id,
         system_signature_id=__ret__.system_signature_id,
+        tag=__ret__.tag,
         type=__ret__.type)
 
 
 @_utilities.lift_output_func(get_waf_signatures)
 def get_waf_signatures_output(accuracy: Optional[pulumi.Input[Optional[str]]] = None,
                               description: Optional[pulumi.Input[Optional[str]]] = None,
+                              enabled: Optional[pulumi.Input[Optional[bool]]] = None,
                               name: Optional[pulumi.Input[Optional[str]]] = None,
+                              perform_staging: Optional[pulumi.Input[Optional[bool]]] = None,
                               risk: Optional[pulumi.Input[Optional[str]]] = None,
                               signature_id: Optional[pulumi.Input[int]] = None,
                               system_signature_id: Optional[pulumi.Input[Optional[str]]] = None,
+                              tag: Optional[pulumi.Input[Optional[str]]] = None,
                               type: Optional[pulumi.Input[Optional[str]]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetWafSignaturesResult]:
     """
     Use this data source (`ssl.get_waf_signatures`) to get the details of attack signatures available on BIG-IP WAF
 
     ## Example Usage
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ssl/key.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ssl/key.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['KeyArgs', 'Key']
@@ -223,20 +224,17 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  content: Optional[pulumi.Input[str]] = None,
                  full_path: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  partition: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = KeyArgs.__new__(KeyArgs)
 
             if content is None and not opts.urn:
                 raise TypeError("Missing required property 'content'")
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/ssl/outputs.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/ssl/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/sys/_inputs.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/sys/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/sys/big_ip_license.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/sys/big_ip_license.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['BigIpLicenseArgs', 'BigIpLicense']
@@ -125,20 +126,17 @@
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  command: Optional[pulumi.Input[str]] = None,
                  registration_key: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = BigIpLicenseArgs.__new__(BigIpLicenseArgs)
 
             if command is None and not opts.urn:
                 raise TypeError("Missing required property 'command'")
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/sys/dns.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/sys/dns.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['DnsArgs', 'Dns']
@@ -224,20 +225,17 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  name_servers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  number_of_dots: Optional[pulumi.Input[int]] = None,
                  searches: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = DnsArgs.__new__(DnsArgs)
 
             if description is None and not opts.urn:
                 raise TypeError("Missing required property 'description'")
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/sys/i_app.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/sys/i_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
@@ -682,20 +683,17 @@
                  tables: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IAppTableArgs']]]]] = None,
                  template: Optional[pulumi.Input[str]] = None,
                  template_modified: Optional[pulumi.Input[str]] = None,
                  template_prerequisite_errors: Optional[pulumi.Input[str]] = None,
                  traffic_group: Optional[pulumi.Input[str]] = None,
                  variables: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IAppVariableArgs']]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = IAppArgs.__new__(IAppArgs)
 
             __props__.__dict__["description"] = description
             __props__.__dict__["devicegroup"] = devicegroup
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/sys/ntp.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/sys/ntp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['NtpArgs', 'Ntp']
@@ -189,20 +190,17 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  servers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  timezone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = NtpArgs.__new__(NtpArgs)
 
             if description is None and not opts.urn:
                 raise TypeError("Missing required property 'description'")
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/sys/outputs.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/sys/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/sys/provision.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/sys/provision.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['ProvisionArgs', 'Provision']
@@ -402,20 +403,17 @@
                  cpu_ratio: Optional[pulumi.Input[int]] = None,
                  disk_ratio: Optional[pulumi.Input[int]] = None,
                  full_path: Optional[pulumi.Input[str]] = None,
                  level: Optional[pulumi.Input[str]] = None,
                  memory_ratio: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProvisionArgs.__new__(ProvisionArgs)
 
             __props__.__dict__["cpu_ratio"] = cpu_ratio
             __props__.__dict__["disk_ratio"] = disk_ratio
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/sys/snmp.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/sys/snmp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['SnmpArgs', 'Snmp']
@@ -186,20 +187,17 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  allowedaddresses: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  sys_contact: Optional[pulumi.Input[str]] = None,
                  sys_location: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = SnmpArgs.__new__(SnmpArgs)
 
             __props__.__dict__["allowedaddresses"] = allowedaddresses
             __props__.__dict__["sys_contact"] = sys_contact
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/sys/snmp_traps.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/sys/snmp_traps.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['SnmpTrapsArgs', 'SnmpTraps']
@@ -575,20 +576,17 @@
                  privacy_password: Optional[pulumi.Input[str]] = None,
                  privacy_password_encrypted: Optional[pulumi.Input[str]] = None,
                  privacy_protocol: Optional[pulumi.Input[str]] = None,
                  security_level: Optional[pulumi.Input[str]] = None,
                  security_name: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = SnmpTrapsArgs.__new__(SnmpTrapsArgs)
 
             __props__.__dict__["auth_passwordencrypted"] = auth_passwordencrypted
             __props__.__dict__["auth_protocol"] = auth_protocol
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/traffic_selector.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/traffic_selector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['TrafficSelectorArgs', 'TrafficSelector']
@@ -439,20 +440,17 @@
                  ip_protocol: Optional[pulumi.Input[int]] = None,
                  ipsec_policy: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  order: Optional[pulumi.Input[int]] = None,
                  source_address: Optional[pulumi.Input[str]] = None,
                  source_port: Optional[pulumi.Input[int]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = TrafficSelectorArgs.__new__(TrafficSelectorArgs)
 
             __props__.__dict__["description"] = description
             if destination_address is None and not opts.urn:
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip/waf_policy.py` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip/waf_policy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,103 +1,133 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
+from . import outputs
+from ._inputs import *
 
 __all__ = ['WafPolicyArgs', 'WafPolicy']
 
 @pulumi.input_type
 class WafPolicyArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  template_name: pulumi.Input[str],
                  application_language: Optional[pulumi.Input[str]] = None,
                  case_insensitive: Optional[pulumi.Input[bool]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  enable_passivemode: Optional[pulumi.Input[bool]] = None,
                  enforcement_mode: Optional[pulumi.Input[str]] = None,
+                 file_types: Optional[pulumi.Input[Sequence[pulumi.Input['WafPolicyFileTypeArgs']]]] = None,
+                 graphql_profiles: Optional[pulumi.Input[Sequence[pulumi.Input['WafPolicyGraphqlProfileArgs']]]] = None,
                  modifications: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 open_api_files: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  parameters: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 partition: Optional[pulumi.Input[str]] = None,
+                 policy_builders: Optional[pulumi.Input[Sequence[pulumi.Input['WafPolicyPolicyBuilderArgs']]]] = None,
                  policy_export_json: Optional[pulumi.Input[str]] = None,
                  policy_id: Optional[pulumi.Input[str]] = None,
                  policy_import_json: Optional[pulumi.Input[str]] = None,
                  protocol_independent: Optional[pulumi.Input[bool]] = None,
                  server_technologies: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  signature_sets: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  signatures: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 signatures_settings: Optional[pulumi.Input[Sequence[pulumi.Input['WafPolicySignaturesSettingArgs']]]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  urls: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a WafPolicy resource.
-        :param pulumi.Input[str] name: The unique user-given name of the policy. Policy names cannot contain spaces or special characters. Allowed characters are a-z, A-Z, 0-9, dot, dash (-), colon (:) and underscore (_). It will be `fullpath`, ex: `/Common/policy1`
+        :param pulumi.Input[str] name: The unique user-given name of the policy. Policy names cannot contain spaces or special characters. Allowed characters are a-z, A-Z, 0-9, dot, dash (-), colon (:) and underscore (_).
         :param pulumi.Input[str] template_name: Specifies the name of the template used for the policy creation.
         :param pulumi.Input[str] application_language: The character encoding for the web application. The character encoding determines how the policy processes the character sets. The default is `utf-8`
         :param pulumi.Input[bool] case_insensitive: Specifies whether the security policy treats microservice URLs, file types, URLs, and parameters as case sensitive or not. When this setting is enabled, the system stores these security policy elements in lowercase in the security policy configuration
         :param pulumi.Input[str] description: Specifies the description of the policy.
         :param pulumi.Input[bool] enable_passivemode: Passive Mode allows the policy to be associated with a Performance L4 Virtual Server (using a FastL4 profile). With FastL4, traffic is analyzed but is not modified in any way.
         :param pulumi.Input[str] enforcement_mode: How the system processes a request that triggers a security policy violation
+        :param pulumi.Input[Sequence[pulumi.Input['WafPolicyFileTypeArgs']]] file_types: `file_types` takes list of file-types options to be used for policy builder.
+               See file types below for more details.
+        :param pulumi.Input[Sequence[pulumi.Input['WafPolicyGraphqlProfileArgs']]] graphql_profiles: `graphql_profiles` takes list of graphql profile options to be used for policy builder.
+               See graphql profiles below for more details.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] modifications: the modifications section includes actions that modify the declarative policy as it is defined in the adjustments
                section. The modifications section is updated manually, with the changes generally driven by the learning suggestions
                provided by the BIG-IP.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] open_api_files: This section defines the Link for open api files on the policy.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] parameters: This section defines parameters that the security policy permits in requests.
+        :param pulumi.Input[str] partition: Specifies the partition of the policy. Default is `Common`
+        :param pulumi.Input[Sequence[pulumi.Input['WafPolicyPolicyBuilderArgs']]] policy_builders: `policy_builder` block will provide `learning_mode` options to be used for policy builder.
+               See policy builder below for more details.
         :param pulumi.Input[str] policy_export_json: Exported WAF policy deployed on BIGIP.
         :param pulumi.Input[str] policy_id: The id of the A.WAF Policy as it would be calculated on the BIG-IP.
-        :param pulumi.Input[str] policy_import_json: The payload of the WAF Policy to be used for IMPORT on to BIGIP
+        :param pulumi.Input[str] policy_import_json: The payload of the WAF Policy to be used for IMPORT on to BIG-IP.
         :param pulumi.Input[bool] protocol_independent: When creating a security policy, you can determine whether a security policy differentiates between HTTP and HTTPS URLs. If enabled, the security policy differentiates between HTTP and HTTPS URLs. If disabled, the security policy configures URLs without specifying a specific protocol. This is useful for applications that behave the same for HTTP and HTTPS, and it keeps the security policy from including the same URL twice.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] server_technologies: The server technology is a server-side application, framework, web server or operating system type that is configured in the policy in order to adapt the policy to the checks needed for the respective technology.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] signature_sets: Defines behavior when signatures found within a signature-set are detected in a request. Settings are culmulative, so if a signature is found in any set with block enabled, that signature will have block enabled.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] signatures: This section defines the properties of a signature on the policy.
-        :param pulumi.Input[str] type: The type of policy you want to create. The default policy type is Security.
+        :param pulumi.Input[Sequence[pulumi.Input['WafPolicySignaturesSettingArgs']]] signatures_settings: bulk signature setting
+        :param pulumi.Input[str] type: The type of policy you want to create. The default policy type is `security`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] urls: In a security policy, you can manually specify the HTTP URLs that are allowed (or disallowed) in traffic to the web application being protected. If you are using automatic policy building (and the policy includes learning URLs), the system can determine which URLs to add, based on legitimate traffic.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "template_name", template_name)
         if application_language is not None:
             pulumi.set(__self__, "application_language", application_language)
         if case_insensitive is not None:
             pulumi.set(__self__, "case_insensitive", case_insensitive)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if enable_passivemode is not None:
             pulumi.set(__self__, "enable_passivemode", enable_passivemode)
         if enforcement_mode is not None:
             pulumi.set(__self__, "enforcement_mode", enforcement_mode)
+        if file_types is not None:
+            pulumi.set(__self__, "file_types", file_types)
+        if graphql_profiles is not None:
+            pulumi.set(__self__, "graphql_profiles", graphql_profiles)
         if modifications is not None:
             pulumi.set(__self__, "modifications", modifications)
+        if open_api_files is not None:
+            pulumi.set(__self__, "open_api_files", open_api_files)
         if parameters is not None:
             pulumi.set(__self__, "parameters", parameters)
+        if partition is not None:
+            pulumi.set(__self__, "partition", partition)
+        if policy_builders is not None:
+            pulumi.set(__self__, "policy_builders", policy_builders)
         if policy_export_json is not None:
             pulumi.set(__self__, "policy_export_json", policy_export_json)
         if policy_id is not None:
             pulumi.set(__self__, "policy_id", policy_id)
         if policy_import_json is not None:
             pulumi.set(__self__, "policy_import_json", policy_import_json)
         if protocol_independent is not None:
             pulumi.set(__self__, "protocol_independent", protocol_independent)
         if server_technologies is not None:
             pulumi.set(__self__, "server_technologies", server_technologies)
         if signature_sets is not None:
             pulumi.set(__self__, "signature_sets", signature_sets)
         if signatures is not None:
             pulumi.set(__self__, "signatures", signatures)
+        if signatures_settings is not None:
+            pulumi.set(__self__, "signatures_settings", signatures_settings)
         if type is not None:
             pulumi.set(__self__, "type", type)
         if urls is not None:
             pulumi.set(__self__, "urls", urls)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
         """
-        The unique user-given name of the policy. Policy names cannot contain spaces or special characters. Allowed characters are a-z, A-Z, 0-9, dot, dash (-), colon (:) and underscore (_). It will be `fullpath`, ex: `/Common/policy1`
+        The unique user-given name of the policy. Policy names cannot contain spaces or special characters. Allowed characters are a-z, A-Z, 0-9, dot, dash (-), colon (:) and underscore (_).
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
@@ -170,40 +200,103 @@
         return pulumi.get(self, "enforcement_mode")
 
     @enforcement_mode.setter
     def enforcement_mode(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "enforcement_mode", value)
 
     @property
+    @pulumi.getter(name="fileTypes")
+    def file_types(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['WafPolicyFileTypeArgs']]]]:
+        """
+        `file_types` takes list of file-types options to be used for policy builder.
+        See file types below for more details.
+        """
+        return pulumi.get(self, "file_types")
+
+    @file_types.setter
+    def file_types(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['WafPolicyFileTypeArgs']]]]):
+        pulumi.set(self, "file_types", value)
+
+    @property
+    @pulumi.getter(name="graphqlProfiles")
+    def graphql_profiles(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['WafPolicyGraphqlProfileArgs']]]]:
+        """
+        `graphql_profiles` takes list of graphql profile options to be used for policy builder.
+        See graphql profiles below for more details.
+        """
+        return pulumi.get(self, "graphql_profiles")
+
+    @graphql_profiles.setter
+    def graphql_profiles(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['WafPolicyGraphqlProfileArgs']]]]):
+        pulumi.set(self, "graphql_profiles", value)
+
+    @property
     @pulumi.getter
     def modifications(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         the modifications section includes actions that modify the declarative policy as it is defined in the adjustments
         section. The modifications section is updated manually, with the changes generally driven by the learning suggestions
         provided by the BIG-IP.
         """
         return pulumi.get(self, "modifications")
 
     @modifications.setter
     def modifications(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "modifications", value)
 
     @property
+    @pulumi.getter(name="openApiFiles")
+    def open_api_files(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        This section defines the Link for open api files on the policy.
+        """
+        return pulumi.get(self, "open_api_files")
+
+    @open_api_files.setter
+    def open_api_files(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "open_api_files", value)
+
+    @property
     @pulumi.getter
     def parameters(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         This section defines parameters that the security policy permits in requests.
         """
         return pulumi.get(self, "parameters")
 
     @parameters.setter
     def parameters(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "parameters", value)
 
     @property
+    @pulumi.getter
+    def partition(self) -> Optional[pulumi.Input[str]]:
+        """
+        Specifies the partition of the policy. Default is `Common`
+        """
+        return pulumi.get(self, "partition")
+
+    @partition.setter
+    def partition(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "partition", value)
+
+    @property
+    @pulumi.getter(name="policyBuilders")
+    def policy_builders(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['WafPolicyPolicyBuilderArgs']]]]:
+        """
+        `policy_builder` block will provide `learning_mode` options to be used for policy builder.
+        See policy builder below for more details.
+        """
+        return pulumi.get(self, "policy_builders")
+
+    @policy_builders.setter
+    def policy_builders(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['WafPolicyPolicyBuilderArgs']]]]):
+        pulumi.set(self, "policy_builders", value)
+
+    @property
     @pulumi.getter(name="policyExportJson")
     def policy_export_json(self) -> Optional[pulumi.Input[str]]:
         """
         Exported WAF policy deployed on BIGIP.
         """
         return pulumi.get(self, "policy_export_json")
 
@@ -223,15 +316,15 @@
     def policy_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "policy_id", value)
 
     @property
     @pulumi.getter(name="policyImportJson")
     def policy_import_json(self) -> Optional[pulumi.Input[str]]:
         """
-        The payload of the WAF Policy to be used for IMPORT on to BIGIP
+        The payload of the WAF Policy to be used for IMPORT on to BIG-IP.
         """
         return pulumi.get(self, "policy_import_json")
 
     @policy_import_json.setter
     def policy_import_json(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "policy_import_json", value)
 
@@ -280,18 +373,30 @@
         return pulumi.get(self, "signatures")
 
     @signatures.setter
     def signatures(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "signatures", value)
 
     @property
+    @pulumi.getter(name="signaturesSettings")
+    def signatures_settings(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['WafPolicySignaturesSettingArgs']]]]:
+        """
+        bulk signature setting
+        """
+        return pulumi.get(self, "signatures_settings")
+
+    @signatures_settings.setter
+    def signatures_settings(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['WafPolicySignaturesSettingArgs']]]]):
+        pulumi.set(self, "signatures_settings", value)
+
+    @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        The type of policy you want to create. The default policy type is Security.
+        The type of policy you want to create. The default policy type is `security`.
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -312,80 +417,107 @@
 class _WafPolicyState:
     def __init__(__self__, *,
                  application_language: Optional[pulumi.Input[str]] = None,
                  case_insensitive: Optional[pulumi.Input[bool]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  enable_passivemode: Optional[pulumi.Input[bool]] = None,
                  enforcement_mode: Optional[pulumi.Input[str]] = None,
+                 file_types: Optional[pulumi.Input[Sequence[pulumi.Input['WafPolicyFileTypeArgs']]]] = None,
+                 graphql_profiles: Optional[pulumi.Input[Sequence[pulumi.Input['WafPolicyGraphqlProfileArgs']]]] = None,
                  modifications: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
+                 open_api_files: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  parameters: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 partition: Optional[pulumi.Input[str]] = None,
+                 policy_builders: Optional[pulumi.Input[Sequence[pulumi.Input['WafPolicyPolicyBuilderArgs']]]] = None,
                  policy_export_json: Optional[pulumi.Input[str]] = None,
                  policy_id: Optional[pulumi.Input[str]] = None,
                  policy_import_json: Optional[pulumi.Input[str]] = None,
                  protocol_independent: Optional[pulumi.Input[bool]] = None,
                  server_technologies: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  signature_sets: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  signatures: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 signatures_settings: Optional[pulumi.Input[Sequence[pulumi.Input['WafPolicySignaturesSettingArgs']]]] = None,
                  template_name: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  urls: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering WafPolicy resources.
         :param pulumi.Input[str] application_language: The character encoding for the web application. The character encoding determines how the policy processes the character sets. The default is `utf-8`
         :param pulumi.Input[bool] case_insensitive: Specifies whether the security policy treats microservice URLs, file types, URLs, and parameters as case sensitive or not. When this setting is enabled, the system stores these security policy elements in lowercase in the security policy configuration
         :param pulumi.Input[str] description: Specifies the description of the policy.
         :param pulumi.Input[bool] enable_passivemode: Passive Mode allows the policy to be associated with a Performance L4 Virtual Server (using a FastL4 profile). With FastL4, traffic is analyzed but is not modified in any way.
         :param pulumi.Input[str] enforcement_mode: How the system processes a request that triggers a security policy violation
+        :param pulumi.Input[Sequence[pulumi.Input['WafPolicyFileTypeArgs']]] file_types: `file_types` takes list of file-types options to be used for policy builder.
+               See file types below for more details.
+        :param pulumi.Input[Sequence[pulumi.Input['WafPolicyGraphqlProfileArgs']]] graphql_profiles: `graphql_profiles` takes list of graphql profile options to be used for policy builder.
+               See graphql profiles below for more details.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] modifications: the modifications section includes actions that modify the declarative policy as it is defined in the adjustments
                section. The modifications section is updated manually, with the changes generally driven by the learning suggestions
                provided by the BIG-IP.
-        :param pulumi.Input[str] name: The unique user-given name of the policy. Policy names cannot contain spaces or special characters. Allowed characters are a-z, A-Z, 0-9, dot, dash (-), colon (:) and underscore (_). It will be `fullpath`, ex: `/Common/policy1`
+        :param pulumi.Input[str] name: The unique user-given name of the policy. Policy names cannot contain spaces or special characters. Allowed characters are a-z, A-Z, 0-9, dot, dash (-), colon (:) and underscore (_).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] open_api_files: This section defines the Link for open api files on the policy.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] parameters: This section defines parameters that the security policy permits in requests.
+        :param pulumi.Input[str] partition: Specifies the partition of the policy. Default is `Common`
+        :param pulumi.Input[Sequence[pulumi.Input['WafPolicyPolicyBuilderArgs']]] policy_builders: `policy_builder` block will provide `learning_mode` options to be used for policy builder.
+               See policy builder below for more details.
         :param pulumi.Input[str] policy_export_json: Exported WAF policy deployed on BIGIP.
         :param pulumi.Input[str] policy_id: The id of the A.WAF Policy as it would be calculated on the BIG-IP.
-        :param pulumi.Input[str] policy_import_json: The payload of the WAF Policy to be used for IMPORT on to BIGIP
+        :param pulumi.Input[str] policy_import_json: The payload of the WAF Policy to be used for IMPORT on to BIG-IP.
         :param pulumi.Input[bool] protocol_independent: When creating a security policy, you can determine whether a security policy differentiates between HTTP and HTTPS URLs. If enabled, the security policy differentiates between HTTP and HTTPS URLs. If disabled, the security policy configures URLs without specifying a specific protocol. This is useful for applications that behave the same for HTTP and HTTPS, and it keeps the security policy from including the same URL twice.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] server_technologies: The server technology is a server-side application, framework, web server or operating system type that is configured in the policy in order to adapt the policy to the checks needed for the respective technology.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] signature_sets: Defines behavior when signatures found within a signature-set are detected in a request. Settings are culmulative, so if a signature is found in any set with block enabled, that signature will have block enabled.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] signatures: This section defines the properties of a signature on the policy.
+        :param pulumi.Input[Sequence[pulumi.Input['WafPolicySignaturesSettingArgs']]] signatures_settings: bulk signature setting
         :param pulumi.Input[str] template_name: Specifies the name of the template used for the policy creation.
-        :param pulumi.Input[str] type: The type of policy you want to create. The default policy type is Security.
+        :param pulumi.Input[str] type: The type of policy you want to create. The default policy type is `security`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] urls: In a security policy, you can manually specify the HTTP URLs that are allowed (or disallowed) in traffic to the web application being protected. If you are using automatic policy building (and the policy includes learning URLs), the system can determine which URLs to add, based on legitimate traffic.
         """
         if application_language is not None:
             pulumi.set(__self__, "application_language", application_language)
         if case_insensitive is not None:
             pulumi.set(__self__, "case_insensitive", case_insensitive)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if enable_passivemode is not None:
             pulumi.set(__self__, "enable_passivemode", enable_passivemode)
         if enforcement_mode is not None:
             pulumi.set(__self__, "enforcement_mode", enforcement_mode)
+        if file_types is not None:
+            pulumi.set(__self__, "file_types", file_types)
+        if graphql_profiles is not None:
+            pulumi.set(__self__, "graphql_profiles", graphql_profiles)
         if modifications is not None:
             pulumi.set(__self__, "modifications", modifications)
         if name is not None:
             pulumi.set(__self__, "name", name)
+        if open_api_files is not None:
+            pulumi.set(__self__, "open_api_files", open_api_files)
         if parameters is not None:
             pulumi.set(__self__, "parameters", parameters)
+        if partition is not None:
+            pulumi.set(__self__, "partition", partition)
+        if policy_builders is not None:
+            pulumi.set(__self__, "policy_builders", policy_builders)
         if policy_export_json is not None:
             pulumi.set(__self__, "policy_export_json", policy_export_json)
         if policy_id is not None:
             pulumi.set(__self__, "policy_id", policy_id)
         if policy_import_json is not None:
             pulumi.set(__self__, "policy_import_json", policy_import_json)
         if protocol_independent is not None:
             pulumi.set(__self__, "protocol_independent", protocol_independent)
         if server_technologies is not None:
             pulumi.set(__self__, "server_technologies", server_technologies)
         if signature_sets is not None:
             pulumi.set(__self__, "signature_sets", signature_sets)
         if signatures is not None:
             pulumi.set(__self__, "signatures", signatures)
+        if signatures_settings is not None:
+            pulumi.set(__self__, "signatures_settings", signatures_settings)
         if template_name is not None:
             pulumi.set(__self__, "template_name", template_name)
         if type is not None:
             pulumi.set(__self__, "type", type)
         if urls is not None:
             pulumi.set(__self__, "urls", urls)
 
@@ -446,14 +578,40 @@
         return pulumi.get(self, "enforcement_mode")
 
     @enforcement_mode.setter
     def enforcement_mode(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "enforcement_mode", value)
 
     @property
+    @pulumi.getter(name="fileTypes")
+    def file_types(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['WafPolicyFileTypeArgs']]]]:
+        """
+        `file_types` takes list of file-types options to be used for policy builder.
+        See file types below for more details.
+        """
+        return pulumi.get(self, "file_types")
+
+    @file_types.setter
+    def file_types(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['WafPolicyFileTypeArgs']]]]):
+        pulumi.set(self, "file_types", value)
+
+    @property
+    @pulumi.getter(name="graphqlProfiles")
+    def graphql_profiles(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['WafPolicyGraphqlProfileArgs']]]]:
+        """
+        `graphql_profiles` takes list of graphql profile options to be used for policy builder.
+        See graphql profiles below for more details.
+        """
+        return pulumi.get(self, "graphql_profiles")
+
+    @graphql_profiles.setter
+    def graphql_profiles(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['WafPolicyGraphqlProfileArgs']]]]):
+        pulumi.set(self, "graphql_profiles", value)
+
+    @property
     @pulumi.getter
     def modifications(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         the modifications section includes actions that modify the declarative policy as it is defined in the adjustments
         section. The modifications section is updated manually, with the changes generally driven by the learning suggestions
         provided by the BIG-IP.
         """
@@ -463,35 +621,72 @@
     def modifications(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "modifications", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The unique user-given name of the policy. Policy names cannot contain spaces or special characters. Allowed characters are a-z, A-Z, 0-9, dot, dash (-), colon (:) and underscore (_). It will be `fullpath`, ex: `/Common/policy1`
+        The unique user-given name of the policy. Policy names cannot contain spaces or special characters. Allowed characters are a-z, A-Z, 0-9, dot, dash (-), colon (:) and underscore (_).
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
+    @pulumi.getter(name="openApiFiles")
+    def open_api_files(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        This section defines the Link for open api files on the policy.
+        """
+        return pulumi.get(self, "open_api_files")
+
+    @open_api_files.setter
+    def open_api_files(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "open_api_files", value)
+
+    @property
     @pulumi.getter
     def parameters(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         This section defines parameters that the security policy permits in requests.
         """
         return pulumi.get(self, "parameters")
 
     @parameters.setter
     def parameters(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "parameters", value)
 
     @property
+    @pulumi.getter
+    def partition(self) -> Optional[pulumi.Input[str]]:
+        """
+        Specifies the partition of the policy. Default is `Common`
+        """
+        return pulumi.get(self, "partition")
+
+    @partition.setter
+    def partition(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "partition", value)
+
+    @property
+    @pulumi.getter(name="policyBuilders")
+    def policy_builders(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['WafPolicyPolicyBuilderArgs']]]]:
+        """
+        `policy_builder` block will provide `learning_mode` options to be used for policy builder.
+        See policy builder below for more details.
+        """
+        return pulumi.get(self, "policy_builders")
+
+    @policy_builders.setter
+    def policy_builders(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['WafPolicyPolicyBuilderArgs']]]]):
+        pulumi.set(self, "policy_builders", value)
+
+    @property
     @pulumi.getter(name="policyExportJson")
     def policy_export_json(self) -> Optional[pulumi.Input[str]]:
         """
         Exported WAF policy deployed on BIGIP.
         """
         return pulumi.get(self, "policy_export_json")
 
@@ -511,15 +706,15 @@
     def policy_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "policy_id", value)
 
     @property
     @pulumi.getter(name="policyImportJson")
     def policy_import_json(self) -> Optional[pulumi.Input[str]]:
         """
-        The payload of the WAF Policy to be used for IMPORT on to BIGIP
+        The payload of the WAF Policy to be used for IMPORT on to BIG-IP.
         """
         return pulumi.get(self, "policy_import_json")
 
     @policy_import_json.setter
     def policy_import_json(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "policy_import_json", value)
 
@@ -568,14 +763,26 @@
         return pulumi.get(self, "signatures")
 
     @signatures.setter
     def signatures(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "signatures", value)
 
     @property
+    @pulumi.getter(name="signaturesSettings")
+    def signatures_settings(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['WafPolicySignaturesSettingArgs']]]]:
+        """
+        bulk signature setting
+        """
+        return pulumi.get(self, "signatures_settings")
+
+    @signatures_settings.setter
+    def signatures_settings(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['WafPolicySignaturesSettingArgs']]]]):
+        pulumi.set(self, "signatures_settings", value)
+
+    @property
     @pulumi.getter(name="templateName")
     def template_name(self) -> Optional[pulumi.Input[str]]:
         """
         Specifies the name of the template used for the policy creation.
         """
         return pulumi.get(self, "template_name")
 
@@ -583,15 +790,15 @@
     def template_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "template_name", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        The type of policy you want to create. The default policy type is Security.
+        The type of policy you want to create. The default policy type is `security`.
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -614,24 +821,30 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  application_language: Optional[pulumi.Input[str]] = None,
                  case_insensitive: Optional[pulumi.Input[bool]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  enable_passivemode: Optional[pulumi.Input[bool]] = None,
                  enforcement_mode: Optional[pulumi.Input[str]] = None,
+                 file_types: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['WafPolicyFileTypeArgs']]]]] = None,
+                 graphql_profiles: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['WafPolicyGraphqlProfileArgs']]]]] = None,
                  modifications: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
+                 open_api_files: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  parameters: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 partition: Optional[pulumi.Input[str]] = None,
+                 policy_builders: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['WafPolicyPolicyBuilderArgs']]]]] = None,
                  policy_export_json: Optional[pulumi.Input[str]] = None,
                  policy_id: Optional[pulumi.Input[str]] = None,
                  policy_import_json: Optional[pulumi.Input[str]] = None,
                  protocol_independent: Optional[pulumi.Input[bool]] = None,
                  server_technologies: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  signature_sets: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  signatures: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 signatures_settings: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['WafPolicySignaturesSettingArgs']]]]] = None,
                  template_name: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  urls: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         `WafPolicy` Manages a WAF Policy resource with its adjustments and modifications on a BIG-IP.
         It outputs an up-to-date WAF Policy in a JSON format
@@ -652,15 +865,16 @@
             type="explicit",
             data_type="alpha-numeric",
             perform_staging=True)
         u_rl = f5bigip.ssl.get_waf_entity_url(name="URL1",
             protocol="http")
         u_rl2 = f5bigip.ssl.get_waf_entity_url(name="URL2")
         test_awaf = f5bigip.WafPolicy("test-awaf",
-            name="/Common/testpolicyravi",
+            name="testpolicyravi",
+            partition="Common",
             template_name="POLICY_TEMPLATE_RAPID_DEPLOYMENT",
             application_language="utf-8",
             enforcement_mode="blocking",
             server_technologies=[
                 "MySQL",
                 "Unix/Linux",
                 "MongoDB",
@@ -686,28 +900,37 @@
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] application_language: The character encoding for the web application. The character encoding determines how the policy processes the character sets. The default is `utf-8`
         :param pulumi.Input[bool] case_insensitive: Specifies whether the security policy treats microservice URLs, file types, URLs, and parameters as case sensitive or not. When this setting is enabled, the system stores these security policy elements in lowercase in the security policy configuration
         :param pulumi.Input[str] description: Specifies the description of the policy.
         :param pulumi.Input[bool] enable_passivemode: Passive Mode allows the policy to be associated with a Performance L4 Virtual Server (using a FastL4 profile). With FastL4, traffic is analyzed but is not modified in any way.
         :param pulumi.Input[str] enforcement_mode: How the system processes a request that triggers a security policy violation
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['WafPolicyFileTypeArgs']]]] file_types: `file_types` takes list of file-types options to be used for policy builder.
+               See file types below for more details.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['WafPolicyGraphqlProfileArgs']]]] graphql_profiles: `graphql_profiles` takes list of graphql profile options to be used for policy builder.
+               See graphql profiles below for more details.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] modifications: the modifications section includes actions that modify the declarative policy as it is defined in the adjustments
                section. The modifications section is updated manually, with the changes generally driven by the learning suggestions
                provided by the BIG-IP.
-        :param pulumi.Input[str] name: The unique user-given name of the policy. Policy names cannot contain spaces or special characters. Allowed characters are a-z, A-Z, 0-9, dot, dash (-), colon (:) and underscore (_). It will be `fullpath`, ex: `/Common/policy1`
+        :param pulumi.Input[str] name: The unique user-given name of the policy. Policy names cannot contain spaces or special characters. Allowed characters are a-z, A-Z, 0-9, dot, dash (-), colon (:) and underscore (_).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] open_api_files: This section defines the Link for open api files on the policy.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] parameters: This section defines parameters that the security policy permits in requests.
+        :param pulumi.Input[str] partition: Specifies the partition of the policy. Default is `Common`
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['WafPolicyPolicyBuilderArgs']]]] policy_builders: `policy_builder` block will provide `learning_mode` options to be used for policy builder.
+               See policy builder below for more details.
         :param pulumi.Input[str] policy_export_json: Exported WAF policy deployed on BIGIP.
         :param pulumi.Input[str] policy_id: The id of the A.WAF Policy as it would be calculated on the BIG-IP.
-        :param pulumi.Input[str] policy_import_json: The payload of the WAF Policy to be used for IMPORT on to BIGIP
+        :param pulumi.Input[str] policy_import_json: The payload of the WAF Policy to be used for IMPORT on to BIG-IP.
         :param pulumi.Input[bool] protocol_independent: When creating a security policy, you can determine whether a security policy differentiates between HTTP and HTTPS URLs. If enabled, the security policy differentiates between HTTP and HTTPS URLs. If disabled, the security policy configures URLs without specifying a specific protocol. This is useful for applications that behave the same for HTTP and HTTPS, and it keeps the security policy from including the same URL twice.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] server_technologies: The server technology is a server-side application, framework, web server or operating system type that is configured in the policy in order to adapt the policy to the checks needed for the respective technology.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] signature_sets: Defines behavior when signatures found within a signature-set are detected in a request. Settings are culmulative, so if a signature is found in any set with block enabled, that signature will have block enabled.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] signatures: This section defines the properties of a signature on the policy.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['WafPolicySignaturesSettingArgs']]]] signatures_settings: bulk signature setting
         :param pulumi.Input[str] template_name: Specifies the name of the template used for the policy creation.
-        :param pulumi.Input[str] type: The type of policy you want to create. The default policy type is Security.
+        :param pulumi.Input[str] type: The type of policy you want to create. The default policy type is `security`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] urls: In a security policy, you can manually specify the HTTP URLs that are allowed (or disallowed) in traffic to the web application being protected. If you are using automatic policy building (and the policy includes learning URLs), the system can determine which URLs to add, based on legitimate traffic.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: WafPolicyArgs,
@@ -732,15 +955,16 @@
             type="explicit",
             data_type="alpha-numeric",
             perform_staging=True)
         u_rl = f5bigip.ssl.get_waf_entity_url(name="URL1",
             protocol="http")
         u_rl2 = f5bigip.ssl.get_waf_entity_url(name="URL2")
         test_awaf = f5bigip.WafPolicy("test-awaf",
-            name="/Common/testpolicyravi",
+            name="testpolicyravi",
+            partition="Common",
             template_name="POLICY_TEMPLATE_RAPID_DEPLOYMENT",
             application_language="utf-8",
             enforcement_mode="blocking",
             server_technologies=[
                 "MySQL",
                 "Unix/Linux",
                 "MongoDB",
@@ -779,56 +1003,65 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  application_language: Optional[pulumi.Input[str]] = None,
                  case_insensitive: Optional[pulumi.Input[bool]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  enable_passivemode: Optional[pulumi.Input[bool]] = None,
                  enforcement_mode: Optional[pulumi.Input[str]] = None,
+                 file_types: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['WafPolicyFileTypeArgs']]]]] = None,
+                 graphql_profiles: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['WafPolicyGraphqlProfileArgs']]]]] = None,
                  modifications: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
+                 open_api_files: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  parameters: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 partition: Optional[pulumi.Input[str]] = None,
+                 policy_builders: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['WafPolicyPolicyBuilderArgs']]]]] = None,
                  policy_export_json: Optional[pulumi.Input[str]] = None,
                  policy_id: Optional[pulumi.Input[str]] = None,
                  policy_import_json: Optional[pulumi.Input[str]] = None,
                  protocol_independent: Optional[pulumi.Input[bool]] = None,
                  server_technologies: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  signature_sets: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  signatures: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 signatures_settings: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['WafPolicySignaturesSettingArgs']]]]] = None,
                  template_name: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  urls: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = WafPolicyArgs.__new__(WafPolicyArgs)
 
             __props__.__dict__["application_language"] = application_language
             __props__.__dict__["case_insensitive"] = case_insensitive
             __props__.__dict__["description"] = description
             __props__.__dict__["enable_passivemode"] = enable_passivemode
             __props__.__dict__["enforcement_mode"] = enforcement_mode
+            __props__.__dict__["file_types"] = file_types
+            __props__.__dict__["graphql_profiles"] = graphql_profiles
             __props__.__dict__["modifications"] = modifications
             if name is None and not opts.urn:
                 raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
+            __props__.__dict__["open_api_files"] = open_api_files
             __props__.__dict__["parameters"] = parameters
+            __props__.__dict__["partition"] = partition
+            __props__.__dict__["policy_builders"] = policy_builders
             __props__.__dict__["policy_export_json"] = policy_export_json
             __props__.__dict__["policy_id"] = policy_id
             __props__.__dict__["policy_import_json"] = policy_import_json
             __props__.__dict__["protocol_independent"] = protocol_independent
             __props__.__dict__["server_technologies"] = server_technologies
             __props__.__dict__["signature_sets"] = signature_sets
             __props__.__dict__["signatures"] = signatures
+            __props__.__dict__["signatures_settings"] = signatures_settings
             if template_name is None and not opts.urn:
                 raise TypeError("Missing required property 'template_name'")
             __props__.__dict__["template_name"] = template_name
             __props__.__dict__["type"] = type
             __props__.__dict__["urls"] = urls
         super(WafPolicy, __self__).__init__(
             'f5bigip:index/wafPolicy:WafPolicy',
@@ -841,24 +1074,30 @@
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             application_language: Optional[pulumi.Input[str]] = None,
             case_insensitive: Optional[pulumi.Input[bool]] = None,
             description: Optional[pulumi.Input[str]] = None,
             enable_passivemode: Optional[pulumi.Input[bool]] = None,
             enforcement_mode: Optional[pulumi.Input[str]] = None,
+            file_types: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['WafPolicyFileTypeArgs']]]]] = None,
+            graphql_profiles: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['WafPolicyGraphqlProfileArgs']]]]] = None,
             modifications: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             name: Optional[pulumi.Input[str]] = None,
+            open_api_files: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             parameters: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            partition: Optional[pulumi.Input[str]] = None,
+            policy_builders: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['WafPolicyPolicyBuilderArgs']]]]] = None,
             policy_export_json: Optional[pulumi.Input[str]] = None,
             policy_id: Optional[pulumi.Input[str]] = None,
             policy_import_json: Optional[pulumi.Input[str]] = None,
             protocol_independent: Optional[pulumi.Input[bool]] = None,
             server_technologies: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             signature_sets: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             signatures: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            signatures_settings: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['WafPolicySignaturesSettingArgs']]]]] = None,
             template_name: Optional[pulumi.Input[str]] = None,
             type: Optional[pulumi.Input[str]] = None,
             urls: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'WafPolicy':
         """
         Get an existing WafPolicy resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
@@ -866,49 +1105,64 @@
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] application_language: The character encoding for the web application. The character encoding determines how the policy processes the character sets. The default is `utf-8`
         :param pulumi.Input[bool] case_insensitive: Specifies whether the security policy treats microservice URLs, file types, URLs, and parameters as case sensitive or not. When this setting is enabled, the system stores these security policy elements in lowercase in the security policy configuration
         :param pulumi.Input[str] description: Specifies the description of the policy.
         :param pulumi.Input[bool] enable_passivemode: Passive Mode allows the policy to be associated with a Performance L4 Virtual Server (using a FastL4 profile). With FastL4, traffic is analyzed but is not modified in any way.
         :param pulumi.Input[str] enforcement_mode: How the system processes a request that triggers a security policy violation
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['WafPolicyFileTypeArgs']]]] file_types: `file_types` takes list of file-types options to be used for policy builder.
+               See file types below for more details.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['WafPolicyGraphqlProfileArgs']]]] graphql_profiles: `graphql_profiles` takes list of graphql profile options to be used for policy builder.
+               See graphql profiles below for more details.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] modifications: the modifications section includes actions that modify the declarative policy as it is defined in the adjustments
                section. The modifications section is updated manually, with the changes generally driven by the learning suggestions
                provided by the BIG-IP.
-        :param pulumi.Input[str] name: The unique user-given name of the policy. Policy names cannot contain spaces or special characters. Allowed characters are a-z, A-Z, 0-9, dot, dash (-), colon (:) and underscore (_). It will be `fullpath`, ex: `/Common/policy1`
+        :param pulumi.Input[str] name: The unique user-given name of the policy. Policy names cannot contain spaces or special characters. Allowed characters are a-z, A-Z, 0-9, dot, dash (-), colon (:) and underscore (_).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] open_api_files: This section defines the Link for open api files on the policy.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] parameters: This section defines parameters that the security policy permits in requests.
+        :param pulumi.Input[str] partition: Specifies the partition of the policy. Default is `Common`
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['WafPolicyPolicyBuilderArgs']]]] policy_builders: `policy_builder` block will provide `learning_mode` options to be used for policy builder.
+               See policy builder below for more details.
         :param pulumi.Input[str] policy_export_json: Exported WAF policy deployed on BIGIP.
         :param pulumi.Input[str] policy_id: The id of the A.WAF Policy as it would be calculated on the BIG-IP.
-        :param pulumi.Input[str] policy_import_json: The payload of the WAF Policy to be used for IMPORT on to BIGIP
+        :param pulumi.Input[str] policy_import_json: The payload of the WAF Policy to be used for IMPORT on to BIG-IP.
         :param pulumi.Input[bool] protocol_independent: When creating a security policy, you can determine whether a security policy differentiates between HTTP and HTTPS URLs. If enabled, the security policy differentiates between HTTP and HTTPS URLs. If disabled, the security policy configures URLs without specifying a specific protocol. This is useful for applications that behave the same for HTTP and HTTPS, and it keeps the security policy from including the same URL twice.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] server_technologies: The server technology is a server-side application, framework, web server or operating system type that is configured in the policy in order to adapt the policy to the checks needed for the respective technology.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] signature_sets: Defines behavior when signatures found within a signature-set are detected in a request. Settings are culmulative, so if a signature is found in any set with block enabled, that signature will have block enabled.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] signatures: This section defines the properties of a signature on the policy.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['WafPolicySignaturesSettingArgs']]]] signatures_settings: bulk signature setting
         :param pulumi.Input[str] template_name: Specifies the name of the template used for the policy creation.
-        :param pulumi.Input[str] type: The type of policy you want to create. The default policy type is Security.
+        :param pulumi.Input[str] type: The type of policy you want to create. The default policy type is `security`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] urls: In a security policy, you can manually specify the HTTP URLs that are allowed (or disallowed) in traffic to the web application being protected. If you are using automatic policy building (and the policy includes learning URLs), the system can determine which URLs to add, based on legitimate traffic.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _WafPolicyState.__new__(_WafPolicyState)
 
         __props__.__dict__["application_language"] = application_language
         __props__.__dict__["case_insensitive"] = case_insensitive
         __props__.__dict__["description"] = description
         __props__.__dict__["enable_passivemode"] = enable_passivemode
         __props__.__dict__["enforcement_mode"] = enforcement_mode
+        __props__.__dict__["file_types"] = file_types
+        __props__.__dict__["graphql_profiles"] = graphql_profiles
         __props__.__dict__["modifications"] = modifications
         __props__.__dict__["name"] = name
+        __props__.__dict__["open_api_files"] = open_api_files
         __props__.__dict__["parameters"] = parameters
+        __props__.__dict__["partition"] = partition
+        __props__.__dict__["policy_builders"] = policy_builders
         __props__.__dict__["policy_export_json"] = policy_export_json
         __props__.__dict__["policy_id"] = policy_id
         __props__.__dict__["policy_import_json"] = policy_import_json
         __props__.__dict__["protocol_independent"] = protocol_independent
         __props__.__dict__["server_technologies"] = server_technologies
         __props__.__dict__["signature_sets"] = signature_sets
         __props__.__dict__["signatures"] = signatures
+        __props__.__dict__["signatures_settings"] = signatures_settings
         __props__.__dict__["template_name"] = template_name
         __props__.__dict__["type"] = type
         __props__.__dict__["urls"] = urls
         return WafPolicy(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="applicationLanguage")
@@ -947,40 +1201,83 @@
     def enforcement_mode(self) -> pulumi.Output[Optional[str]]:
         """
         How the system processes a request that triggers a security policy violation
         """
         return pulumi.get(self, "enforcement_mode")
 
     @property
+    @pulumi.getter(name="fileTypes")
+    def file_types(self) -> pulumi.Output[Optional[Sequence['outputs.WafPolicyFileType']]]:
+        """
+        `file_types` takes list of file-types options to be used for policy builder.
+        See file types below for more details.
+        """
+        return pulumi.get(self, "file_types")
+
+    @property
+    @pulumi.getter(name="graphqlProfiles")
+    def graphql_profiles(self) -> pulumi.Output[Optional[Sequence['outputs.WafPolicyGraphqlProfile']]]:
+        """
+        `graphql_profiles` takes list of graphql profile options to be used for policy builder.
+        See graphql profiles below for more details.
+        """
+        return pulumi.get(self, "graphql_profiles")
+
+    @property
     @pulumi.getter
     def modifications(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         the modifications section includes actions that modify the declarative policy as it is defined in the adjustments
         section. The modifications section is updated manually, with the changes generally driven by the learning suggestions
         provided by the BIG-IP.
         """
         return pulumi.get(self, "modifications")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        The unique user-given name of the policy. Policy names cannot contain spaces or special characters. Allowed characters are a-z, A-Z, 0-9, dot, dash (-), colon (:) and underscore (_). It will be `fullpath`, ex: `/Common/policy1`
+        The unique user-given name of the policy. Policy names cannot contain spaces or special characters. Allowed characters are a-z, A-Z, 0-9, dot, dash (-), colon (:) and underscore (_).
         """
         return pulumi.get(self, "name")
 
     @property
+    @pulumi.getter(name="openApiFiles")
+    def open_api_files(self) -> pulumi.Output[Optional[Sequence[str]]]:
+        """
+        This section defines the Link for open api files on the policy.
+        """
+        return pulumi.get(self, "open_api_files")
+
+    @property
     @pulumi.getter
     def parameters(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         This section defines parameters that the security policy permits in requests.
         """
         return pulumi.get(self, "parameters")
 
     @property
+    @pulumi.getter
+    def partition(self) -> pulumi.Output[Optional[str]]:
+        """
+        Specifies the partition of the policy. Default is `Common`
+        """
+        return pulumi.get(self, "partition")
+
+    @property
+    @pulumi.getter(name="policyBuilders")
+    def policy_builders(self) -> pulumi.Output[Optional[Sequence['outputs.WafPolicyPolicyBuilder']]]:
+        """
+        `policy_builder` block will provide `learning_mode` options to be used for policy builder.
+        See policy builder below for more details.
+        """
+        return pulumi.get(self, "policy_builders")
+
+    @property
     @pulumi.getter(name="policyExportJson")
     def policy_export_json(self) -> pulumi.Output[str]:
         """
         Exported WAF policy deployed on BIGIP.
         """
         return pulumi.get(self, "policy_export_json")
 
@@ -992,15 +1289,15 @@
         """
         return pulumi.get(self, "policy_id")
 
     @property
     @pulumi.getter(name="policyImportJson")
     def policy_import_json(self) -> pulumi.Output[Optional[str]]:
         """
-        The payload of the WAF Policy to be used for IMPORT on to BIGIP
+        The payload of the WAF Policy to be used for IMPORT on to BIG-IP.
         """
         return pulumi.get(self, "policy_import_json")
 
     @property
     @pulumi.getter(name="protocolIndependent")
     def protocol_independent(self) -> pulumi.Output[Optional[bool]]:
         """
@@ -1029,26 +1326,34 @@
     def signatures(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         This section defines the properties of a signature on the policy.
         """
         return pulumi.get(self, "signatures")
 
     @property
+    @pulumi.getter(name="signaturesSettings")
+    def signatures_settings(self) -> pulumi.Output[Optional[Sequence['outputs.WafPolicySignaturesSetting']]]:
+        """
+        bulk signature setting
+        """
+        return pulumi.get(self, "signatures_settings")
+
+    @property
     @pulumi.getter(name="templateName")
     def template_name(self) -> pulumi.Output[str]:
         """
         Specifies the name of the template used for the policy creation.
         """
         return pulumi.get(self, "template_name")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[Optional[str]]:
         """
-        The type of policy you want to create. The default policy type is Security.
+        The type of policy you want to create. The default policy type is `security`.
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def urls(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip.egg-info/PKG-INFO` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,73 @@
 Metadata-Version: 2.1
 Name: pulumi-f5bigip
-Version: 3.9.0a1654086391
+Version: 3.9.0a1661535806
 Summary: A Pulumi package for creating and managing F5 BigIP resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-f5bigip
-Description: [![Actions Status](https://github.com/pulumi/pulumi-f5bigip/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-f5bigip/actions)
-        [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
-        [![NPM version](https://badge.fury.io/js/%40pulumi%2Ff5bigip.svg)](https://www.npmjs.com/package/@pulumi/f5bigip)
-        [![Python version](https://badge.fury.io/py/pulumi-f5bigip.svg)](https://pypi.org/project/pulumi-f5bigip)
-        [![NuGet version](https://badge.fury.io/nu/pulumi.f5bigip.svg)](https://badge.fury.io/nu/pulumi.f5bigip)
-        [![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-f5bigip/sdk/v3/go)](https://pkg.go.dev/github.com/pulumi/pulumi-f5bigip/sdk/v3/go)
-        [![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumi.svg)](https://github.com/pulumi/pulumi-f5bigip/blob/master/LICENSE)
-        
-        # F5 BigIP Provider
-        
-        This provider allows management of F5 BigIP resources using Pulumi. This provider uses the iControlREST API to
-        perform management tasks, so it will need to be installed and enabled on your F5 device before proceeding.
-        
-        ## Installing
-        
-        This package is available in many languages in the standard packaging formats.
-        
-        ### Node.js (Java/TypeScript)
-        
-        To use from JavaScript or TypeScript in Node.js, install using either `npm`:
-        
-            $ npm install @pulumi/f5bigip
-        
-        or `yarn`:
-        
-            $ yarn add @pulumi/f5bigip
-        
-        ### Python
-        
-        To use from Python, install using `pip`:
-        
-            $ pip install pulumi_f5bigip
-        
-        ### Go
-        
-        To use from Go, use `go get` to grab the latest version of the library
-        
-            $ go get github.com/pulumi/pulumi-f5bigip/sdk/v3
-            
-        ### .NET
-        
-        To use from .NET, install using `dotnet add package`:
-        
-            $ dotnet add package Pulumi.F5bigip
-            
-        ## Configuration
-        
-        The following configuration points are available:
-        
-        - `f5bigip:address` - Domain name/IP of the BigIP. May be set via the `BIGIP_HOST` environment variable.
-        - `f5bigip:port` - Management Port to connect to BigIP.
-        - `f5bigip:username` - Username with API access to the BigIP. May be set via the `BIGIP_USER` environment variable.
-        - `f5bigip:password` - Password for API access to the BigIP. May be set via the `BIGIP_PASSWORD` environment variable.
-        - `f5bigip:tokenAuth` - Enable to use an external authentication source (LDAP, TACACS, etc). May be set via the `BIGIP_TOKEN_AUTH` environment variable.
-        - `f5bigip:tokenAuth` - Enable to use an external authentication source (LDAP, TACACS, etc). May be set via the `BIGIP_TOKEN_AUTH` environment variable.
-        - `f5bigip:loginRef` - Login reference for token authentication (see BIG-IP REST docs for details) May be set via the `BIGIP_LOGIN_REF` environment variable.
-        
-        ## Reference
-        
-        For further information, please visit [the F5bigip provider docs](https://www.pulumi.com/docs/intro/cloud-providers/f5bigip) or for detailed reference documentation, please visit [the API docs](https://www.pulumi.com/docs/reference/pkg/f5bigip).
-        
 Keywords: pulumi f5 bigip
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+
+[![Actions Status](https://github.com/pulumi/pulumi-f5bigip/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-f5bigip/actions)
+[![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
+[![NPM version](https://badge.fury.io/js/%40pulumi%2Ff5bigip.svg)](https://www.npmjs.com/package/@pulumi/f5bigip)
+[![Python version](https://badge.fury.io/py/pulumi-f5bigip.svg)](https://pypi.org/project/pulumi-f5bigip)
+[![NuGet version](https://badge.fury.io/nu/pulumi.f5bigip.svg)](https://badge.fury.io/nu/pulumi.f5bigip)
+[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-f5bigip/sdk/v3/go)](https://pkg.go.dev/github.com/pulumi/pulumi-f5bigip/sdk/v3/go)
+[![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumi.svg)](https://github.com/pulumi/pulumi-f5bigip/blob/master/LICENSE)
+
+# F5 BigIP Provider
+
+This provider allows management of F5 BigIP resources using Pulumi. This provider uses the iControlREST API to
+perform management tasks, so it will need to be installed and enabled on your F5 device before proceeding.
+
+## Installing
+
+This package is available in many languages in the standard packaging formats.
+
+### Node.js (Java/TypeScript)
+
+To use from JavaScript or TypeScript in Node.js, install using either `npm`:
+
+    $ npm install @pulumi/f5bigip
+
+or `yarn`:
+
+    $ yarn add @pulumi/f5bigip
+
+### Python
+
+To use from Python, install using `pip`:
+
+    $ pip install pulumi_f5bigip
+
+### Go
+
+To use from Go, use `go get` to grab the latest version of the library
+
+    $ go get github.com/pulumi/pulumi-f5bigip/sdk/v3
+    
+### .NET
+
+To use from .NET, install using `dotnet add package`:
+
+    $ dotnet add package Pulumi.F5bigip
+    
+## Configuration
+
+The following configuration points are available:
+
+- `f5bigip:address` - Domain name/IP of the BigIP. May be set via the `BIGIP_HOST` environment variable.
+- `f5bigip:port` - Management Port to connect to BigIP.
+- `f5bigip:username` - Username with API access to the BigIP. May be set via the `BIGIP_USER` environment variable.
+- `f5bigip:password` - Password for API access to the BigIP. May be set via the `BIGIP_PASSWORD` environment variable.
+- `f5bigip:tokenAuth` - Enable to use an external authentication source (LDAP, TACACS, etc). May be set via the `BIGIP_TOKEN_AUTH` environment variable.
+- `f5bigip:tokenAuth` - Enable to use an external authentication source (LDAP, TACACS, etc). May be set via the `BIGIP_TOKEN_AUTH` environment variable.
+- `f5bigip:loginRef` - Login reference for token authentication (see BIG-IP REST docs for details) May be set via the `BIGIP_LOGIN_REF` environment variable.
+
+## Reference
+
+For further information, please visit [the F5bigip provider docs](https://www.pulumi.com/docs/intro/cloud-providers/f5bigip) or for detailed reference documentation, please visit [the API docs](https://www.pulumi.com/docs/reference/pkg/f5bigip).
+
+
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/pulumi_f5bigip.egg-info/SOURCES.txt` & `pulumi_f5bigip-3.9.0a1661535806/pulumi_f5bigip.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 pulumi_f5bigip/as3.py
 pulumi_f5bigip/big_iq_as3.py
 pulumi_f5bigip/command.py
 pulumi_f5bigip/common_license_manage_big_iq.py
 pulumi_f5bigip/do.py
 pulumi_f5bigip/event_service_discovery.py
 pulumi_f5bigip/fast_application.py
+pulumi_f5bigip/fast_http_app.py
+pulumi_f5bigip/fast_https_app.py
+pulumi_f5bigip/fast_tcp_app.py
 pulumi_f5bigip/fast_template.py
 pulumi_f5bigip/ipsec_policy.py
 pulumi_f5bigip/ipsec_profile.py
 pulumi_f5bigip/net_ike_peer.py
 pulumi_f5bigip/net_tunnel.py
 pulumi_f5bigip/outputs.py
 pulumi_f5bigip/provider.py
```

### Comparing `pulumi_f5bigip-3.9.0a1654086391/setup.py` & `pulumi_f5bigip-3.9.0a1661535806/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.9.0a1654086391"
-PLUGIN_VERSION = "3.9.0-alpha.1654086391+eb30d238"
+VERSION = "3.9.0a1661535806"
+PLUGIN_VERSION = "3.9.0-alpha.1661535806+c5d753e3"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'f5bigip', PLUGIN_VERSION])
         except OSError as error:
```

