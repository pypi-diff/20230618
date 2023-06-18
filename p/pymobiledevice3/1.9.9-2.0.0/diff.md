# Comparing `tmp/pymobiledevice3-1.9.9.tar.gz` & `tmp/pymobiledevice3-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymobiledevice3-1.9.9.tar", last modified: Mon Aug  9 09:47:42 2021, max compression
+gzip compressed data, was "pymobiledevice3-2.0.0.tar", last modified: Sun Jun 18 13:43:25 2023, max compression
```

## Comparing `pymobiledevice3-1.9.9.tar` & `pymobiledevice3-2.0.0.tar`

### file list

```diff
@@ -1,114 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:42.795218 pymobiledevice3-1.9.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2021-08-09 09:47:32.000000 pymobiledevice3-1.9.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    16368 2021-08-09 09:47:42.791217 pymobiledevice3-1.9.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13258 2021-08-09 09:47:32.000000 pymobiledevice3-1.9.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:42.779218 pymobiledevice3-1.9.9/pymobiledevice3/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1872 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5315 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/ca.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:42.783218 pymobiledevice3-1.9.9/pymobiledevice3/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1972 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/afc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1571 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     4874 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/backup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1272 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/cli_common.py
--rw-r--r--   0 runner    (1001) docker     (121)     1395 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/crash.py
--rw-r--r--   0 runner    (1001) docker     (121)    27492 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/developer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2683 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (121)      679 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/list_devices.py
--rw-r--r--   0 runner    (1001) docker     (121)     1857 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/lockdown.py
--rw-r--r--   0 runner    (1001) docker     (121)     3820 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/mounter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1416 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/notification.py
--rw-r--r--   0 runner    (1001) docker     (121)     1695 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/pcap.py
--rw-r--r--   0 runner    (1001) docker     (121)      719 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/power_assertion.py
--rw-r--r--   0 runner    (1001) docker     (121)      998 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/processes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/profile.py
--rw-r--r--   0 runner    (1001) docker     (121)      998 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/provision.py
--rw-r--r--   0 runner    (1001) docker     (121)     2295 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/restore.py
--rw-r--r--   0 runner    (1001) docker     (121)     1755 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/springboard.py
--rw-r--r--   0 runner    (1001) docker     (121)     4661 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/syslog.py
--rw-r--r--   0 runner    (1001) docker     (121)     1678 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3223 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/irecv.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11356 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/lockdown.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:42.783218 pymobiledevice3-1.9.9/pymobiledevice3/resources/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)  1023280 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/resources/dsc_uuid_map.json
--rw-r--r--   0 runner    (1001) docker     (121)     2520 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/resources/dsc_uuid_map.py
--rw-r--r--   0 runner    (1001) docker     (121)     1794 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/resources/firmware_notifications.py
--rw-r--r--   0 runner    (1001) docker     (121)    20970 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/resources/notifications.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:42.787217 pymobiledevice3-1.9.9/pymobiledevice3/restore/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/restore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2979 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/restore/img4.py
--rw-r--r--   0 runner    (1001) docker     (121)    16208 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/restore/restore.py
--rw-r--r--   0 runner    (1001) docker     (121)     9471 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/restore/tss.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3905 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/service_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:42.787217 pymobiledevice3-1.9.9/pymobiledevice3/services/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5807 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/accessibilityaudit.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    20621 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/afc.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      593 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/debugserver_applist.py
--rw-r--r--   0 runner    (1001) docker     (121)     7341 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/device_link.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5608 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/diagnostics.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1433 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dtfetchsymbols.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:42.787217 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      744 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/dvt_secure_socket_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:42.791217 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8570 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/activity_trace_tap.py
--rw-r--r--   0 runner    (1001) docker     (121)      666 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/application_listing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/condition_inducer.py
--rw-r--r--   0 runner    (1001) docker     (121)    26146 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/core_profile_session_tap.py
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/device_info.py
--rw-r--r--   0 runner    (1001) docker     (121)      892 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/energy_monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)      588 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/graphics.py
--rw-r--r--   0 runner    (1001) docker     (121)     2547 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/network_monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)      829 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/notifications.py
--rw-r--r--   0 runner    (1001) docker     (121)     1406 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/process_control.py
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/sysmontap.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1406 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/file_relay.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      985 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/house_arrest.py
--rw-r--r--   0 runner    (1001) docker     (121)     6130 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/installation_proxy.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1483 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/misagent.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1809 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/mobile_config.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2895 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/mobile_image_mounter.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12675 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/mobilebackup2.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      977 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/notification_proxy.py
--rw-r--r--   0 runner    (1001) docker     (121)     4011 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/os_trace.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8856 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/pcapd.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      819 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/power_assertion.py
--rw-r--r--   0 runner    (1001) docker     (121)      629 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/preboard.py
--rw-r--r--   0 runner    (1001) docker     (121)    12701 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/remote_server.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1317 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/screenshot.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1732 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/simulate_location.py
--rw-r--r--   0 runner    (1001) docker     (121)     1551 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/springboard.py
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/syslog.py
--rw-r--r--   0 runner    (1001) docker     (121)     4148 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/tcp_forwarder.py
--rw-r--r--   0 runner    (1001) docker     (121)     8865 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/usbmux.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:42.783218 pymobiledevice3-1.9.9/pymobiledevice3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16368 2021-08-09 09:47:42.000000 pymobiledevice3-1.9.9/pymobiledevice3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3772 2021-08-09 09:47:42.000000 pymobiledevice3-1.9.9/pymobiledevice3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-09 09:47:42.000000 pymobiledevice3-1.9.9/pymobiledevice3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-08-09 09:47:42.000000 pymobiledevice3-1.9.9/pymobiledevice3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      149 2021-08-09 09:47:42.000000 pymobiledevice3-1.9.9/pymobiledevice3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-08-09 09:47:42.000000 pymobiledevice3-1.9.9/pymobiledevice3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      149 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-09 09:47:42.795218 pymobiledevice3-1.9.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1636 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:42.791217 pymobiledevice3-1.9.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:42.791217 pymobiledevice3-1.9.9/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      358 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/tests/cli/test_mounter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:42.791217 pymobiledevice3-1.9.9/tests/services/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/tests/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      212 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/tests/services/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:42.791217 pymobiledevice3-1.9.9/tests/services/instruments/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/tests/services/instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      777 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/tests/services/instruments/test_core_profile_session.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/tests/services/test_afc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4321 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/tests/services/test_dvt_secure_socket_proxy.py
--rw-r--r--   0 runner    (1001) docker     (121)      645 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/tests/services/test_pcapd.py
--rw-r--r--   0 runner    (1001) docker     (121)      440 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/tests/services/test_screenshotr_relay.py
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/tests/services/test_springboard_services_relay.py
--rw-r--r--   0 runner    (1001) docker     (121)      979 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/tests/services/test_syslog_relay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:25.944023 pymobiledevice3-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    57629 2023-06-18 13:43:25.944023 pymobiledevice3-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:25.916023 pymobiledevice3-2.0.0/pymobiledevice3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/bonjour.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1420 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/ca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:25.928023 pymobiledevice3-2.0.0/pymobiledevice3/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/afc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/amfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/bonjour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/cli_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/companion_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/crash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34760 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/developer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/lockdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9726 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/mounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/pcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/power_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/provision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/springboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/syslog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/cli/webinspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/irecv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32198 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/irecv_devices.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27360 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/lockdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/pair_records.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:25.932023 pymobiledevice3-2.0.0/pymobiledevice3/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1023280 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/resources/dsc_uuid_map.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/resources/dsc_uuid_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/resources/firmware_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25467 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/resources/notifications.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:25.936023 pymobiledevice3-2.0.0/pymobiledevice3/resources/webinspector/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/resources/webinspector/element_attribute.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/resources/webinspector/element_clear.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/resources/webinspector/enter_fullscreen.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/resources/webinspector/find_nodes.js
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/resources/webinspector/focus.js
+-rw-r--r--   0 runner    (1001) docker     (123)    42234 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/resources/webinspector/get_attribute.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43072 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/resources/webinspector/is_displayed.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/resources/webinspector/is_editable.js
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/resources/webinspector/is_enabled.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:25.936023 pymobiledevice3-2.0.0/pymobiledevice3/restore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/restore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/restore/asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/restore/base_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/restore/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/restore/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/restore/fdr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/restore/ftab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16315 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/restore/recovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49812 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/restore/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/restore/restore_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/restore/restored_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29015 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/restore/tss.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6768 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/service_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:25.940023 pymobiledevice3-2.0.0/pymobiledevice3/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/accessibilityaudit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31043 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/afc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/amfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/base_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/companion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/crash_reports.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/debugserver_applist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1153 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/device_arbitration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/device_link.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6154 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/diagnostics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1441 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dtfetchsymbols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:25.940023 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/dvt_secure_socket_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:25.940023 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/activity_trace_tap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/application_listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/condition_inducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27895 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/core_profile_session_tap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/device_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/energy_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/network_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/process_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/sysmontap.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/file_relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/heartbeat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/house_arrest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/installation_proxy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1894 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/misagent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3379 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/mobile_activation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3322 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/mobile_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10734 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/mobile_image_mounter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16752 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/mobilebackup2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1544 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/notification_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/os_trace.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9223 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/pcapd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/power_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/preboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/remote_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1270 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/screenshot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1790 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/simulate_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/springboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/syslog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:25.944023 pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/automation_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/cdp_screencast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/cdp_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32080 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/cdp_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/inspector_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/selenium_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/session_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/web_protocol/switch_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14217 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/services/webinspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/tcp_forwarder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pymobiledevice3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:25.920023 pymobiledevice3-2.0.0/pymobiledevice3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    57629 2023-06-18 13:43:25.000000 pymobiledevice3-2.0.0/pymobiledevice3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-06-18 13:43:25.000000 pymobiledevice3-2.0.0/pymobiledevice3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 13:43:25.000000 pymobiledevice3-2.0.0/pymobiledevice3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-18 13:43:25.000000 pymobiledevice3-2.0.0/pymobiledevice3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-18 13:43:25.000000 pymobiledevice3-2.0.0/pymobiledevice3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-18 13:43:25.000000 pymobiledevice3-2.0.0/pymobiledevice3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 13:43:25.944023 pymobiledevice3-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:43:25.944023 pymobiledevice3-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-18 13:43:08.000000 pymobiledevice3-2.0.0/tests/test_utils.py
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/cli/afc.py` & `pymobiledevice3-2.0.0/pymobiledevice3/cli/afc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import posixpath
-
 import click
 
 from pymobiledevice3.cli.cli_common import Command
+from pymobiledevice3.lockdown import LockdownClient
 from pymobiledevice3.services.afc import AfcService, AfcShell
 
 
 @click.group()
 def cli():
     """ apps cli """
     pass
@@ -15,49 +14,42 @@
 @cli.group()
 def afc():
     """ FileSystem utils """
     pass
 
 
 @afc.command('shell', cls=Command)
-def afc_shell(lockdown):
+def afc_shell(lockdown: LockdownClient):
     """ open an AFC shell rooted at /var/mobile/Media """
     AfcShell(lockdown=lockdown, service_name='com.apple.afc').cmdloop()
 
 
 @afc.command('pull', cls=Command)
 @click.argument('remote_file', type=click.Path(exists=False))
 @click.argument('local_file', type=click.File('wb'))
-def afc_pull(lockdown, remote_file, local_file):
+def afc_pull(lockdown: LockdownClient, remote_file, local_file):
     """ pull remote file from /var/mobile/Media """
     local_file.write(AfcService(lockdown=lockdown).get_file_contents(remote_file))
 
 
 @afc.command('push', cls=Command)
 @click.argument('local_file', type=click.File('rb'))
 @click.argument('remote_file', type=click.Path(exists=False))
-def afc_push(lockdown, local_file, remote_file):
+def afc_push(lockdown: LockdownClient, local_file, remote_file):
     """ push local file into /var/mobile/Media """
     AfcService(lockdown=lockdown).set_file_contents(remote_file, local_file.read())
 
 
-def show_dirlist(afc, dirname, recursive=False):
-    for filename in afc.listdir(dirname):
-        filename = posixpath.join(dirname, filename)
-        print(filename)
-        if recursive and afc.isdir(filename):
-            show_dirlist(afc, filename, recursive=recursive)
-
-
 @afc.command('ls', cls=Command)
 @click.argument('remote_file', type=click.Path(exists=False))
 @click.option('-r', '--recursive', is_flag=True)
-def afc_ls(lockdown, remote_file, recursive):
+def afc_ls(lockdown: LockdownClient, remote_file, recursive):
     """ perform a dirlist rooted at /var/mobile/Media """
-    show_dirlist(AfcService(lockdown=lockdown), remote_file, recursive=recursive)
+    for path in AfcService(lockdown=lockdown).dirlist(remote_file, -1 if recursive else 1):
+        print(path)
 
 
 @afc.command('rm', cls=Command)
 @click.argument('remote_file', type=click.Path(exists=False))
-def afc_rm(lockdown, remote_file):
+def afc_rm(lockdown: LockdownClient, remote_file):
     """ remove a file rooted at /var/mobile/Media """
     AfcService(lockdown=lockdown).rm(remote_file)
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/cli/apps.py` & `pymobiledevice3-2.0.0/pymobiledevice3/cli/apps.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import click
 
 from pymobiledevice3.cli.cli_common import Command, print_json
+from pymobiledevice3.lockdown import LockdownClient
 from pymobiledevice3.services.house_arrest import HouseArrestService
 from pymobiledevice3.services.installation_proxy import InstallationProxyService
 
 
 @click.group()
 def cli():
     """ apps cli """
@@ -17,36 +18,39 @@
     pass
 
 
 @apps.command('list', cls=Command)
 @click.option('--color/--no-color', default=True)
 @click.option('-u', '--user', is_flag=True, help='include user apps')
 @click.option('-s', '--system', is_flag=True, help='include system apps')
-def apps_list(lockdown, color, user, system):
+@click.option('--hidden', is_flag=True, help='include hidden apps')
+def apps_list(lockdown: LockdownClient, color, user, system, hidden):
     """ list installed apps """
     app_types = []
     if user:
         app_types.append('User')
     if system:
         app_types.append('System')
+    if hidden:
+        app_types.append('Hidden')
     print_json(InstallationProxyService(lockdown=lockdown).get_apps(app_types), colored=color)
 
 
 @apps.command('uninstall', cls=Command)
 @click.argument('bundle_id')
-def uninstall(lockdown, bundle_id):
+def uninstall(lockdown: LockdownClient, bundle_id):
     """ uninstall app by given bundle_id """
     InstallationProxyService(lockdown=lockdown).uninstall(bundle_id)
 
 
 @apps.command('install', cls=Command)
 @click.argument('ipa_path', type=click.Path(exists=True))
-def install(lockdown, ipa_path):
+def install(lockdown: LockdownClient, ipa_path):
     """ install given .ipa """
     InstallationProxyService(lockdown=lockdown).install_from_local(ipa_path)
 
 
 @apps.command('afc', cls=Command)
 @click.argument('bundle_id')
-def afc(lockdown, bundle_id):
+def afc(lockdown: LockdownClient, bundle_id):
     """ open an AFC shell for given bundle_id, assuming its profile is installed """
     HouseArrestService(lockdown=lockdown).shell(bundle_id)
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/cli/backup.py` & `pymobiledevice3-2.0.0/pymobiledevice3/cli/backup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 import logging
 
-from tqdm import tqdm
 import click
+from tqdm import tqdm
 
 from pymobiledevice3.cli.cli_common import Command
-from pymobiledevice3.services.mobilebackup2 import Mobilebackup2Service
 from pymobiledevice3.lockdown import LockdownClient
+from pymobiledevice3.services.mobilebackup2 import Mobilebackup2Service
+
+source_option = click.option('--source', default='', help='The UDID of the source device.')
+password_option = click.option('-p', '--password', default='', help='Backup password.')
+backup_directory_arg = click.argument('backup-directory', type=click.Path(exists=True, file_okay=False))
+backup_directory_option = click.option('-b', '--backup-directory', type=click.Path(exists=True, file_okay=False),
+                                       default='.')
+
+logger = logging.getLogger(__name__)
 
 
 @click.group()
 def cli():
     """ backup cli """
     pass
 
@@ -17,104 +25,148 @@
 @cli.group()
 def backup2():
     """ backup utils """
     pass
 
 
 @backup2.command(cls=Command)
-@click.argument('backup-directory', type=click.Path(exists=True, file_okay=False))
-@click.option('--full', is_flag=True)
+@click.argument('backup-directory', type=click.Path(file_okay=False))
+@click.option('--full', is_flag=True, help=('Whether to do a full backup.'
+                                            ' If full is True, any previous backup attempts will be discarded.'))
 def backup(lockdown: LockdownClient, backup_directory, full):
+    """
+    Backup device.
+
+    All backup data will be written to BACKUP_DIRECTORY, under a directory named with the device's udid.
+    """
     backup_client = Mobilebackup2Service(lockdown)
-    with tqdm(total=100) as pbar:
+    with tqdm(total=100, dynamic_ncols=True) as pbar:
         def update_bar(percentage):
             pbar.n = percentage
             pbar.refresh()
 
         backup_client.backup(full=full, backup_directory=backup_directory, progress_callback=update_bar)
 
 
 @backup2.command(cls=Command)
-@click.argument('backup-directory', type=click.Path(exists=True, file_okay=False))
-@click.option('--system/--no-system', default=False)
-@click.option('--reboot/--no-reboot', default=True)
-@click.option('--copy/--no-copy', default=True)
-@click.option('--settings/--no-settings', default=True)
-@click.option('--remove/--no-remove', default=False)
-@click.option('-p', '--password', type=click.STRING, default='')
-def restore(lockdown: LockdownClient, backup_directory, system, reboot, copy, settings, remove, password):
+@backup_directory_arg
+@click.option('--system/--no-system', default=False, help='Restore system files.')
+@click.option('--reboot/--no-reboot', default=True, help='Reboot the device when done.')
+@click.option('--copy/--no-copy', default=True, help='Create a copy of backup folder before restoring.')
+@click.option('--settings/--no-settings', default=True, help='Restore device settings.')
+@click.option('--remove/--no-remove', default=False, help='Remove items which aren\'t being restored.')
+@password_option
+@source_option
+def restore(lockdown: LockdownClient, backup_directory, system, reboot, copy, settings, remove, password, source):
+    """
+    Restore a backup to a device.
+
+    The backup will be restored from a directory with the device udid under BACKUP_DIRECTORY.
+    """
     backup_client = Mobilebackup2Service(lockdown)
-    with tqdm(total=100) as pbar:
+    with tqdm(total=100, dynamic_ncols=True) as pbar:
         def update_bar(percentage):
             pbar.n = percentage
             pbar.refresh()
 
         backup_client.restore(backup_directory=backup_directory, progress_callback=update_bar, system=system,
-                              reboot=reboot, copy=copy, settings=settings, remove=remove, password=password)
+                              reboot=reboot, copy=copy, settings=settings, remove=remove, password=password,
+                              source=source)
 
 
 @backup2.command(cls=Command)
-@click.argument('backup-directory', type=click.Path(exists=True, file_okay=False))
-def info(lockdown: LockdownClient, backup_directory):
+@backup_directory_arg
+@source_option
+def info(lockdown: LockdownClient, backup_directory, source):
+    """
+    Print information about a backup.
+    """
     backup_client = Mobilebackup2Service(lockdown)
-    print(backup_client.info(backup_directory=backup_directory))
+    print(backup_client.info(backup_directory=backup_directory, source=source))
 
 
 @backup2.command('list', cls=Command)
-@click.argument('backup-directory', type=click.Path(exists=True, file_okay=False))
-def list_(lockdown: LockdownClient, backup_directory):
+@backup_directory_arg
+@source_option
+def list_(lockdown: LockdownClient, backup_directory, source):
+    """
+    List all file in the backup in a CSV format.
+    """
     backup_client = Mobilebackup2Service(lockdown)
-    print(backup_client.list(backup_directory=backup_directory))
+    print(backup_client.list(backup_directory=backup_directory, source=source))
 
 
 @backup2.command(cls=Command)
-@click.argument('backup-directory', type=click.Path(exists=True, file_okay=False))
-@click.option('-p', '--password', type=click.STRING, default='')
-def unback(lockdown: LockdownClient, backup_directory, password):
+@backup_directory_arg
+@password_option
+@source_option
+def unback(lockdown: LockdownClient, backup_directory, password, source):
+    """
+    Convert all files in the backup to the correct directory hierarchy.
+    """
     backup_client = Mobilebackup2Service(lockdown)
-    backup_client.unback(backup_directory=backup_directory, password=password)
+    backup_client.unback(backup_directory=backup_directory, password=password, source=source)
 
 
 @backup2.command(cls=Command)
-@click.argument('domain-name', type=click.STRING)
-@click.argument('relative-path', type=click.STRING)
-@click.argument('backup-directory', type=click.Path(exists=True, file_okay=False))
-@click.option('-p', '--password', type=click.STRING, default='')
-def extract(lockdown: LockdownClient, domain_name, relative_path, backup_directory, password):
+@click.argument('domain-name')
+@click.argument('relative-path')
+@backup_directory_arg
+@password_option
+@source_option
+def extract(lockdown: LockdownClient, domain_name, relative_path, backup_directory, password, source):
+    """
+    Extract a file from the backup.
+
+    The file that belongs to the domain DOMAIN_NAME and located on the device in the path RELATIVE_PATH,
+    will be extracted to the BACKUP_DIRECTORY.
+    """
     backup_client = Mobilebackup2Service(lockdown)
-    backup_client.extract(domain_name, relative_path, backup_directory=backup_directory, password=password)
+    backup_client.extract(domain_name, relative_path, backup_directory=backup_directory, password=password,
+                          source=source)
 
 
 @backup2.command(cls=Command)
-@click.argument('on', type=click.BOOL)
-@click.argument('password', type=click.STRING)
-@click.argument('backup-directory', type=click.Path(exists=True, file_okay=False))
-def encryption(lockdown: LockdownClient, backup_directory, on, password):
-    will_encrypt = lockdown.get_value('com.apple.mobile.backup', 'WillEncrypt')
-    if will_encrypt == on:
-        logging.error('Encryption already ' + ('on!' if on else 'off!'))
-        return
+@click.argument('mode', type=click.Choice(['on', 'off'], case_sensitive=False))
+@click.argument('password')
+@backup_directory_option
+def encryption(lockdown: LockdownClient, backup_directory, mode, password):
+    """
+    Set backup encryption on / off.
+
+    When on, PASSWORD will be the new backup password.
+    When off, PASSWORD is the current backup password.
+    """
     backup_client = Mobilebackup2Service(lockdown)
-    if on:
+    should_encrypt = mode.lower() == 'on'
+    if should_encrypt == backup_client.will_encrypt:
+        logger.error('Encryption already ' + ('on!' if should_encrypt else 'off!'))
+        return
+    if should_encrypt:
         backup_client.change_password(backup_directory, new=password)
     else:
         backup_client.change_password(backup_directory, old=password)
 
 
 @backup2.command(cls=Command)
-@click.argument('old-password', type=click.STRING)
-@click.argument('new-password', type=click.STRING)
-@click.argument('backup-directory', type=click.Path(exists=True, file_okay=False))
+@click.argument('old-password')
+@click.argument('new-password')
+@backup_directory_option
 def change_password(lockdown: LockdownClient, old_password, new_password, backup_directory):
-    will_encrypt = lockdown.get_value('com.apple.mobile.backup', 'WillEncrypt')
-    if not will_encrypt:
-        logging.error('Encryption is not turned on!')
-        return
+    """
+    Change the backup password.
+    """
     backup_client = Mobilebackup2Service(lockdown)
+    if not backup_client.will_encrypt:
+        logger.error('Encryption is not turned on!')
+        return
     backup_client.change_password(backup_directory, old=old_password, new=new_password)
 
 
 @backup2.command(cls=Command)
-@click.argument('backup-directory', type=click.Path(exists=True, file_okay=False))
+@backup_directory_arg
 def erase_device(lockdown: LockdownClient, backup_directory):
+    """
+    Erase all data on the device.
+    """
     backup_client = Mobilebackup2Service(lockdown)
     backup_client.erase_device(backup_directory)
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/cli/developer.py` & `pymobiledevice3-2.0.0/pymobiledevice3/cli/developer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,58 @@
 # flake8: noqa: C901
 import json
 import logging
 import os
 import posixpath
 import shlex
+import signal
+import time
 from collections import namedtuple
 from dataclasses import asdict
+from datetime import datetime
+from pathlib import Path
+from typing import List
 
 import click
+from click.exceptions import MissingParameter, UsageError
 from pykdebugparser.pykdebugparser import PyKdebugParser
+from termcolor import colored
+
 import pymobiledevice3
-from pymobiledevice3.cli.cli_common import print_json, Command, default_json_encoder
-from pymobiledevice3.exceptions import DvtDirListError
+from pymobiledevice3.cli.cli_common import BASED_INT, Command, default_json_encoder, print_json, wait_return
+from pymobiledevice3.exceptions import DeviceAlreadyInUseError, DvtDirListError, ExtractingStackshotError, \
+    UnrecognizedSelectorError
 from pymobiledevice3.lockdown import LockdownClient
+from pymobiledevice3.services.accessibilityaudit import AccessibilityAudit
 from pymobiledevice3.services.debugserver_applist import DebugServerAppList
+from pymobiledevice3.services.device_arbitration import DtDeviceArbitration
+from pymobiledevice3.services.dtfetchsymbols import DtFetchSymbols
 from pymobiledevice3.services.dvt.dvt_secure_socket_proxy import DvtSecureSocketProxyService
 from pymobiledevice3.services.dvt.instruments.activity_trace_tap import ActivityTraceTap, decode_message_format
 from pymobiledevice3.services.dvt.instruments.application_listing import ApplicationListing
 from pymobiledevice3.services.dvt.instruments.condition_inducer import ConditionInducer
 from pymobiledevice3.services.dvt.instruments.core_profile_session_tap import CoreProfileSessionTap
 from pymobiledevice3.services.dvt.instruments.device_info import DeviceInfo
 from pymobiledevice3.services.dvt.instruments.energy_monitor import EnergyMonitor
 from pymobiledevice3.services.dvt.instruments.graphics import Graphics
-from pymobiledevice3.services.dvt.instruments.network_monitor import NetworkMonitor, ConnectionDetectionEvent
+from pymobiledevice3.services.dvt.instruments.network_monitor import ConnectionDetectionEvent, NetworkMonitor
 from pymobiledevice3.services.dvt.instruments.notifications import Notifications
 from pymobiledevice3.services.dvt.instruments.process_control import ProcessControl
+from pymobiledevice3.services.dvt.instruments.screenshot import Screenshot
 from pymobiledevice3.services.dvt.instruments.sysmontap import Sysmontap
-from pymobiledevice3.services.accessibilityaudit import AccessibilityAudit
 from pymobiledevice3.services.os_trace import OsTraceService
 from pymobiledevice3.services.remote_server import RemoteServer
 from pymobiledevice3.services.screenshot import ScreenshotService
-from pymobiledevice3.services.dtfetchsymbols import DtFetchSymbols
 from pymobiledevice3.services.simulate_location import DtSimulateLocation
-from termcolor import colored
 from pymobiledevice3.tcp_forwarder import TcpForwarder
 
-
-def wait_return():
-    input('> Hit RETURN to exit')
+BSC_SUBCLASS = 0x40c
+BSC_CLASS = 0x4
+VFS_AND_TRACES_SET = {0x03010000, 0x07ff0000}
+logger = logging.getLogger(__name__)
 
 
 @click.group()
 def cli():
     """ developer cli """
     pass
 
@@ -58,95 +69,109 @@
     """
     pass
 
 
 @developer.command('shell', cls=Command)
 @click.argument('service')
 @click.option('-r', '--remove-ssl-context', is_flag=True)
-def developer_shell(lockdown, service, remove_ssl_context):
+def developer_shell(lockdown: LockdownClient, service, remove_ssl_context):
     """ Launch developer shell. """
     with RemoteServer(lockdown, service, remove_ssl_context) as service:
         service.shell()
 
 
 @developer.group()
 def dvt():
     """ dvt operations """
     pass
 
 
 @dvt.command('proclist', cls=Command)
 @click.option('--color/--no-color', default=True)
-def proclist(lockdown, color):
+def proclist(lockdown: LockdownClient, color):
     """ show process list """
     with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
         processes = DeviceInfo(dvt).proclist()
         for process in processes:
             if 'startDate' in process:
                 process['startDate'] = str(process['startDate'])
 
         print_json(processes, colored=color)
 
 
 @dvt.command('applist', cls=Command)
 @click.option('--color/--no-color', default=True)
-def applist(lockdown, color):
+def applist(lockdown: LockdownClient, color):
     """ show application list """
     with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
         apps = ApplicationListing(dvt).applist()
         print_json(apps, colored=color)
 
 
+@dvt.command('signal', cls=Command)
+@click.argument('pid', type=click.INT)
+@click.argument('sig', type=click.INT, required=False)
+@click.option('-s', '--signal-name', type=click.Choice([s.name for s in signal.Signals]))
+def send_signal(lockdown, pid, sig, signal_name):
+    """ Send SIGNAL to process by its PID """
+    if not sig and not signal_name:
+        raise MissingParameter(param_type='argument|option', param_hint='\'SIG|SIGNAL-NAME\'')
+    if sig and signal_name:
+        raise UsageError(message='Cannot give SIG and SIGNAL-NAME together')
+    sig = sig or signal.Signals[signal_name].value
+    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+        ProcessControl(dvt).signal(pid, sig)
+
+
 @dvt.command('kill', cls=Command)
 @click.argument('pid', type=click.INT)
-def kill(lockdown, pid):
+def kill(lockdown: LockdownClient, pid):
     """ Kill a process by its pid. """
     with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
         ProcessControl(dvt).kill(pid)
 
 
 @dvt.command('pkill', cls=Command)
 @click.argument('expression')
-def pkill(lockdown, expression):
+def pkill(lockdown: LockdownClient, expression):
     """ kill all processes containing `expression` in their name. """
     processes = OsTraceService(lockdown=lockdown).get_pid_list()['Payload']
     if len(processes) == 0:
         # no point at trying to use DvtSecureSocketProxyService if no processes
         # were matched
         return
 
     with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
         process_control = ProcessControl(dvt)
         for pid, process_info in processes.items():
             process_name = process_info['ProcessName']
             if expression in process_name:
-                logging.info(f'killing {process_name}({pid})')
+                logger.info(f'killing {process_name}({pid})')
                 process_control.kill(pid)
 
 
 @dvt.command('launch', cls=Command)
 @click.argument('arguments', type=click.STRING)
-@click.option('--kill-existing/--no-kill-existing', default=True)
-@click.option('--suspended', is_flag=True)
-def launch(lockdown: LockdownClient, arguments: str, kill_existing: bool, suspended: bool):
-    """
-    Launch a process.
-    :param lockdown: Lockdown client.
-    :param arguments: Arguments of process to launch, the first argument is the bundle id.
-    :param kill_existing: Whether to kill an existing instance of this process.
-    :param suspended: Same as WaitForDebugger.
-    """
+@click.option('--kill-existing/--no-kill-existing', default=True,
+              help='Whether to kill an existing instance of this process')
+@click.option('--suspended', is_flag=True, help='Same as WaitForDebugger')
+@click.option('--env', multiple=True, type=click.Tuple((str, str)),
+              help='Environment variables to pass to process given as a list of key value')
+def launch(lockdown: LockdownClient, arguments: str, kill_existing: bool, suspended: bool, env: tuple):
+    """ Launch a process. """
     with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
         parsed_arguments = shlex.split(arguments)
-        pid = ProcessControl(dvt).launch(parsed_arguments[0], parsed_arguments[1:], kill_existing, suspended)
+        pid = ProcessControl(dvt).launch(bundle_id=parsed_arguments[0], arguments=parsed_arguments[1:],
+                                         kill_existing=kill_existing, start_suspended=suspended,
+                                         environment=dict(env))
         print(f'Process launched with pid {pid}')
 
 
 @dvt.command('shell', cls=Command)
-def dvt_shell(lockdown):
+def dvt_shell(lockdown: LockdownClient):
     """ Launch developer shell. """
     with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
         dvt.shell()
 
 
 def show_dirlist(device_info: DeviceInfo, dirname, recursive=False):
     try:
@@ -158,87 +183,99 @@
         filename = posixpath.join(dirname, filename)
         print(filename)
         if recursive:
             show_dirlist(device_info, filename, recursive=recursive)
 
 
 @dvt.command('ls', cls=Command)
-@click.argument('path', type=click.Path(exists=False))
+@click.argument('path', type=click.Path(exists=False, readable=False))
 @click.option('-r', '--recursive', is_flag=True)
-def ls(lockdown, path, recursive):
+def ls(lockdown: LockdownClient, path, recursive):
     """ List directory. """
     with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
         show_dirlist(DeviceInfo(dvt), path, recursive=recursive)
 
 
 @dvt.command('device-information', cls=Command)
 @click.option('--color/--no-color', default=True)
-def device_information(lockdown, color):
+def device_information(lockdown: LockdownClient, color):
     """ Print system information. """
     with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
         device_info = DeviceInfo(dvt)
-        print_json({
-            'system': device_info.system_information(),
+        info = {
             'hardware': device_info.hardware_information(),
             'network': device_info.network_information(),
-        }, colored=color)
+            'kernel-name': device_info.mach_kernel_name(),
+            'kpep-database': device_info.kpep_database(),
+        }
+        try:
+            info['system'] = device_info.system_information()
+        except UnrecognizedSelectorError:
+            pass
+        print_json(info, colored=color)
 
 
 @dvt.command('netstat', cls=Command)
-def netstat(lockdown):
+def netstat(lockdown: LockdownClient):
     """ Print information about current network activity. """
     with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
         with NetworkMonitor(dvt) as monitor:
             for event in monitor:
                 if isinstance(event, ConnectionDetectionEvent):
-                    logging.info(
+                    logger.info(
                         f'Connection detected: {event.local_address.data.address}:{event.local_address.port} -> '
                         f'{event.remote_address.data.address}:{event.remote_address.port}')
 
 
+@dvt.command('screenshot', cls=Command)
+@click.argument('out', type=click.File('wb'))
+def screenshot(lockdown: LockdownClient, out):
+    """ get device screenshot """
+    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+        out.write(Screenshot(dvt).get_screenshot())
+
+
 @dvt.group('sysmon')
 def sysmon():
     """ System monitor options. """
 
 
 @sysmon.group('process')
 def sysmon_process():
     """ Process monitor options. """
 
 
 @sysmon_process.command('monitor', cls=Command)
 @click.argument('threshold', type=click.FLOAT)
-def sysmon_process_monitor(lockdown, threshold):
+def sysmon_process_monitor(lockdown: LockdownClient, threshold):
     """ monitor all most consuming processes by given cpuUsage threshold. """
 
     Process = namedtuple('process', 'pid name cpuUsage')
 
     with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
         with Sysmontap(dvt) as sysmon:
             for process_snapshot in sysmon.iter_processes():
                 entries = []
                 for process in process_snapshot:
                     if (process['cpuUsage'] is not None) and (process['cpuUsage'] >= threshold):
                         entries.append(Process(pid=process['pid'], name=process['name'], cpuUsage=process['cpuUsage']))
 
-                logging.info(entries)
+                logger.info(entries)
 
 
 @sysmon_process.command('single', cls=Command)
-@click.option('-f', '--fields', help='show only given field names splitted by ",".')
 @click.option('-a', '--attributes', multiple=True,
               help='filter processes by given attribute value given as key=value')
-def sysmon_process_single(lockdown, fields, attributes):
+@click.option('--color/--no-color', default=True)
+def sysmon_process_single(lockdown: LockdownClient, attributes: List[str], color: bool):
     """ show a single snapshot of currently running processes. """
 
-    if fields is not None:
-        fields = fields.split(',')
-
     count = 0
 
+    result = []
     with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
         device_info = DeviceInfo(dvt)
 
         with Sysmontap(dvt) as sysmon:
             for process_snapshot in sysmon.iter_processes():
                 count += 1
 
@@ -256,27 +293,24 @@
                                 break
 
                     if skip:
                         continue
 
                     # adding "artificially" the execName field
                     process['execName'] = device_info.execname_for_pid(process['pid'])
-
-                    print(f'{process["name"]} ({process["pid"]})')
-                    for name, value in process.items():
-                        if (fields is None) or (name in fields):
-                            print(f'\t{name}: {value}')
+                    result.append(process)
 
                 # exit after single snapshot
-                return
+                break
+    print_json(result, colored=color)
 
 
 @sysmon.command('system', cls=Command)
 @click.option('-f', '--fields', help='field names splitted by ",".')
-def sysmon_system(lockdown, fields):
+def sysmon_system(lockdown: LockdownClient, fields):
     """ show current system stats. """
 
     if fields is not None:
         fields = fields.split(',')
 
     with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
         sysmontap = Sysmontap(dvt)
@@ -293,44 +327,58 @@
 
 
 @dvt.group('core-profile-session')
 def core_profile_session():
     """ Core profile session options. """
 
 
-def parse_filters(filters):
-    if not filters:
+bsc_filter = click.option('--bsc/--no-bsc', default=False, help='Whether to print BSC events or not.')
+class_filter = click.option('-cf', '--class-filters', multiple=True, type=BASED_INT,
+                            help='Events class filter. Omit for all.')
+subclass_filter = click.option('-sf', '--subclass-filters', multiple=True, type=BASED_INT,
+                               help='Events subclass filter. Omit for all.')
+
+
+def parse_filters(subclasses: List[int], classes: List[int]):
+    if not subclasses and not classes:
         return None
     parsed = set()
-    for filter_ in filters:
-        print(filter_)
-        if filter_.lower() == 'bsc':
-            parsed |= {0x03010000, 0x040c0000, 0x07ff0000}  # VFS_LOOKUP, BSC operations, TRACE
-        else:
-            parsed.add(int(filter_, 16) << 16)
-
+    for subclass in subclasses:
+        if subclass == BSC_SUBCLASS:
+            parsed |= VFS_AND_TRACES_SET
+        parsed.add(subclass << 16)
+    for class_ in classes:
+        if class_ == BSC_CLASS:
+            parsed |= VFS_AND_TRACES_SET
+        parsed.add((class_ << 24) | 0x00ff0000)
     return parsed
 
 
 @core_profile_session.command('live', cls=Command)
 @click.option('-c', '--count', type=click.INT, default=-1, help='Number of events to print. Omit to endless sniff.')
-@click.option('-f', '--filters', multiple=True, help='Events filter. Omit for all.')
-@click.option('--pid', type=click.INT, default=None, help='Process ID to filter. Omit for all.')
+@bsc_filter
+@class_filter
+@subclass_filter
 @click.option('--tid', type=click.INT, default=None, help='Thread ID to filter. Omit for all.')
 @click.option('--timestamp/--no-timestamp', default=True, help='Whether to print timestamp or not.')
 @click.option('--event-name/--no-event-name', default=True, help='Whether to print event name or not.')
 @click.option('--func-qual/--no-func-qual', default=True, help='Whether to print function qualifier or not.')
 @click.option('--show-tid/--no-show-tid', default=True, help='Whether to print thread id or not.')
 @click.option('--process-name/--no-process-name', default=True, help='Whether to print process name or not.')
 @click.option('--args/--no-args', default=True, help='Whether to print event arguments or not.')
-def live_profile_session(lockdown, count, filters, pid, tid, timestamp, event_name, func_qual,
-                         show_tid, process_name, args):
+def live_profile_session(lockdown: LockdownClient, count, bsc, class_filters, subclass_filters, tid, timestamp,
+                         event_name, func_qual, show_tid, process_name, args):
     """ Print kevents received from the device in real time. """
-    filters = parse_filters(filters)
+
     parser = PyKdebugParser()
+    parser.filter_class = class_filters
+    if bsc:
+        subclass_filters = list(subclass_filters) + [BSC_SUBCLASS]
+    parser.filter_subclass = subclass_filters
+    filters = parse_filters(subclass_filters, class_filters)
     parser.filter_tid = tid
     parser.show_timestamp = timestamp
     parser.show_name = event_name
     parser.show_func_qual = func_qual
     parser.show_tid = show_tid
     parser.show_process = process_name
     parser.show_args = args
@@ -349,57 +397,74 @@
                 i += 1
                 if i == count:
                     break
 
 
 @core_profile_session.command('save', cls=Command)
 @click.argument('out', type=click.File('wb'))
-@click.option('-f', '--filters', multiple=True, help='Events filter. Omit for all.')
-def save_profile_session(lockdown, out, filters):
+@bsc_filter
+@class_filter
+@subclass_filter
+def save_profile_session(lockdown: LockdownClient, out, bsc, class_filters, subclass_filters):
     """ Dump core profiling information. """
-    filters = parse_filters(filters)
+    if bsc:
+        subclass_filters = list(subclass_filters) + [BSC_SUBCLASS]
+    filters = parse_filters(subclass_filters, class_filters)
     with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
         with CoreProfileSessionTap(dvt, {}, filters) as tap:
             tap.dump(out)
 
 
 @core_profile_session.command('stackshot', cls=Command)
 @click.option('--out', type=click.File('w'), default=None)
 @click.option('--color/--no-color', default=True)
-def stackshot(lockdown, out, color):
+def stackshot(lockdown: LockdownClient, out, color):
     """ Dump stackshot information. """
     with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
         with CoreProfileSessionTap(dvt, {}) as tap:
-            data = tap.get_stackshot()
+            try:
+                data = tap.get_stackshot()
+            except ExtractingStackshotError:
+                logger.error(f'Extracting stackshot failed')
+                return
+
             if out is not None:
                 json.dump(data, out, indent=4, default=default_json_encoder)
             else:
                 print_json(data, colored=color)
 
 
 @core_profile_session.command('parse-live', cls=Command)
 @click.option('-c', '--count', type=click.INT, default=-1, help='Number of events to print. Omit to endless sniff.')
-@click.option('--pid', type=click.INT, default=None, help='Process ID to filter. Omit for all.')
 @click.option('--tid', type=click.INT, default=None, help='Thread ID to filter. Omit for all.')
 @click.option('--show-tid/--no-show-tid', default=False, help='Whether to print thread id or not.')
-@click.option('-f', '--filters', multiple=True, help='Events filter. Omit for all.')
+@bsc_filter
+@class_filter
+@subclass_filter
+@click.option('--process', default=None, help='Process ID / name to filter. Omit for all.')
 @click.option('--color/--no-color', default=True)
-def parse_live_profile_session(lockdown, count, pid, tid, show_tid, filters, color):
+def parse_live_profile_session(lockdown: LockdownClient, count, tid, show_tid, bsc, class_filters, subclass_filters,
+                               process, color):
     """ Print traces (syscalls, thread events, etc.) received from the device in real time. """
     with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
-        filters = parse_filters(filters)
         print('Receiving time information')
         time_config = CoreProfileSessionTap.get_time_config(dvt)
         parser = PyKdebugParser()
+        parser.filter_class = list(class_filters)
+        if bsc:
+            subclass_filters = list(subclass_filters) + [BSC_SUBCLASS]
+        parser.filter_subclass = subclass_filters
+        filters = parse_filters(subclass_filters, class_filters)
         parser.numer = time_config['numer']
         parser.denom = time_config['denom']
         parser.mach_absolute_time = time_config['mach_absolute_time']
         parser.usecs_since_epoch = time_config['usecs_since_epoch']
         parser.timezone = time_config['timezone']
         parser.filter_tid = tid
+        parser.filter_process = process
         parser.color = color
         parser.show_tid = show_tid
 
         with CoreProfileSessionTap(dvt, time_config, filters) as tap:
             if show_tid:
                 print('{:^32}|{:^11}|{:^33}|   Event'.format('Time', 'Thread', 'Process'))
             else:
@@ -433,15 +498,15 @@
 
 @core_profile_session.command('callstacks-live', cls=Command)
 @click.option('-c', '--count', type=click.INT, default=-1, help='Number of events to print. Omit to endless sniff.')
 @click.option('--process', default=None, help='Process to filter. Omit for all.')
 @click.option('--tid', type=click.INT, default=None, help='Thread ID to filter. Omit for all.')
 @click.option('--show-tid/--no-show-tid', default=False, help='Whether to print thread id or not.')
 @click.option('--color/--no-color', default=True)
-def callstacks_live_profile_session(lockdown, count, process, tid, show_tid, color):
+def callstacks_live_profile_session(lockdown: LockdownClient, count, process, tid, show_tid, color):
     """ Print callstacks received from the device in real time. """
     with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
         print('Receiving time information')
         time_config = CoreProfileSessionTap.get_time_config(dvt)
         parser = PyKdebugParser()
         parser.numer = time_config['numer']
         parser.denom = time_config['denom']
@@ -464,260 +529,378 @@
                 i += 1
                 if i == count:
                     break
 
 
 @dvt.command('trace-codes', cls=Command)
 @click.option('--color/--no-color', default=True)
-def trace_codes(lockdown, color):
-    """ Print system information. """
+def dvt_trace_codes(lockdown: LockdownClient, color):
+    """ Print KDebug trace codes. """
     with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
         device_info = DeviceInfo(dvt)
         print_json({hex(k): v for k, v in device_info.trace_codes().items()}, colored=color)
 
 
+@dvt.command('name-for-uid', cls=Command)
+@click.argument('uid', type=click.INT)
+def dvt_name_for_uid(lockdown: LockdownClient, uid):
+    """ Print the assiciated username for the given uid. """
+    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+        device_info = DeviceInfo(dvt)
+        print(device_info.name_for_uid(uid))
+
+
+@dvt.command('name-for-gid', cls=Command)
+@click.argument('gid', type=click.INT)
+def dvt_name_for_gid(lockdown: LockdownClient, gid):
+    """ Print the assiciated group name for the given gid. """
+    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+        device_info = DeviceInfo(dvt)
+        print(device_info.name_for_gid(gid))
+
+
 @dvt.command('oslog', cls=Command)
 @click.option('--color/--no-color', default=True)
 @click.option('--pid', type=click.INT)
-def dvt_oslog(lockdown, color, pid):
+def dvt_oslog(lockdown: LockdownClient, color, pid):
     """ oslog. """
     with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
         with ActivityTraceTap(dvt) as tap:
             for message in tap:
                 message_pid = message.process
-                message_type = message.message_type
+                # without message_type maybe signpost have event_type
+                message_type = message.message_type if hasattr(message, 'message_type') else message.event_type \
+                    if hasattr(message, 'event_type') else 'unknown'
                 sender_image_path = message.sender_image_path
                 image_name = os.path.basename(sender_image_path)
                 subsystem = message.subsystem
                 category = message.category
+                timestamp = datetime.now()
 
                 if pid is not None and message_pid != pid:
                     continue
 
-                try:
-                    formatted_message = decode_message_format(message.message).decode()
-                except Exception:
-                    print('error decoding')
+                if message.message:
+                    formatted_message = decode_message_format(message.message)
+                else:
+                    formatted_message = message.name
 
                 if color:
+                    timestamp = colored(str(timestamp), attrs=['bold'])
                     message_pid = colored(str(message_pid), 'magenta')
                     subsystem = colored(subsystem, 'green')
                     category = colored(category, 'green')
                     image_name = colored(image_name, 'yellow')
                     message_type = colored(message_type, 'cyan')
 
-                print(f'[{subsystem}][{category}][{message_pid}][{image_name}] <{message_type}>: {formatted_message}')
+                print(f'[{timestamp}][{subsystem}][{category}][{message_pid}][{image_name}] '
+                      f'<{message_type}>: {formatted_message}')
 
 
 @dvt.command('energy', cls=Command)
 @click.argument('pid-list', nargs=-1)
-def dvt_energy(lockdown, pid_list):
+def dvt_energy(lockdown: LockdownClient, pid_list):
     """ energy monitoring for given pid list. """
 
     if len(pid_list) == 0:
-        logging.error('pid_list must not be empty')
+        logger.error('pid_list must not be empty')
         return
 
     pid_list = [int(pid) for pid in pid_list]
 
     with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
         with EnergyMonitor(dvt, pid_list) as energy_monitor:
             for telemetry in energy_monitor:
-                logging.info(telemetry)
+                logger.info(telemetry)
 
 
 @dvt.command('notifications', cls=Command)
-def dvt_notifications(lockdown):
+def dvt_notifications(lockdown: LockdownClient):
     """ monitor memory and app notifications """
     with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
         with Notifications(dvt) as notifications:
             for notification in notifications:
-                logging.info(notification)
+                logger.info(notification)
 
 
 @dvt.command('graphics', cls=Command)
-def dvt_notifications(lockdown):
+def dvt_notifications(lockdown: LockdownClient):
     """ monitor graphics statistics """
     with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
         with Graphics(dvt) as graphics:
             for stats in graphics:
-                logging.info(stats)
+                logger.info(stats)
+
+
+@developer.group('fetch-symbols')
+def fetch_symbols():
+    """ fetch-symbols options. """
+    pass
 
 
-@developer.command('fetch-symbols', cls=Command)
+@fetch_symbols.command('list', cls=Command)
+@click.option('--color/--no-color', default=True)
+def fetch_symbols_list(lockdown: LockdownClient, color: bool):
+    """ list of files to be downloaded """
+    print_json(DtFetchSymbols(lockdown).list_files(), colored=color)
+
+
+@fetch_symbols.command('download', cls=Command)
 @click.argument('out', type=click.Path(dir_okay=True, file_okay=False))
-def developer_fetch_symbols(lockdown, out):
+def fetch_symbols_download(lockdown: LockdownClient, out):
     """ download the linker and dyld cache to a specified directory """
     fetch_symbols = DtFetchSymbols(lockdown)
     files = fetch_symbols.list_files()
+    out = Path(out)
 
     if not os.path.exists(out):
         os.makedirs(out)
 
-    for i, filename in enumerate(files):
-        filename = os.path.join(out, os.path.basename(filename))
-        with open(filename, 'wb') as f:
-            logging.info(f'writing to: {filename}')
+    downloaded_files = set()
+
+    for i, file in enumerate(files):
+        if file.startswith('/'):
+            # trim root to allow relative download
+            file = file[1:]
+        file = out / file
+
+        if file not in downloaded_files:
+            # first time the file was seen in list, means we can safely remove any old copy if any
+            file.unlink(missing_ok=True)
+
+        downloaded_files.add(file)
+        file.parent.mkdir(parents=True, exist_ok=True)
+        with open(file, 'ab') as f:
+            # same file may appear twice, so we'll need to append data into it
+            logger.info(f'writing to: {file}')
             fetch_symbols.get_file(i, f)
 
 
 @developer.group('simulate-location')
 def simulate_location():
     """ simulate-location options. """
     pass
 
 
 @simulate_location.command('clear', cls=Command)
-def simulate_location_clear(lockdown):
+def simulate_location_clear(lockdown: LockdownClient):
     """ clear simulated location """
     DtSimulateLocation(lockdown).clear()
 
 
 @simulate_location.command('set', cls=Command)
 @click.argument('latitude', type=click.FLOAT)
 @click.argument('longitude', type=click.FLOAT)
-def simulate_location_set(lockdown, latitude, longitude):
+def simulate_location_set(lockdown: LockdownClient, latitude, longitude):
     """
     set a simulated location.
     try:
         ... set -- 40.690008 -74.045843 for liberty island
     """
     DtSimulateLocation(lockdown).set(latitude, longitude)
 
 
 @simulate_location.command('play', cls=Command)
 @click.argument('filename', type=click.Path(exists=True, file_okay=True, dir_okay=False))
 @click.option('--disable-sleep', is_flag=True, default=False)
-def simulate_location_play(lockdown, filename, disable_sleep):
+def simulate_location_play(lockdown: LockdownClient, filename, disable_sleep):
     """
     play a .gpx file
     """
     DtSimulateLocation(lockdown).play_gpx_file(filename, disable_sleep=disable_sleep)
 
 
 @developer.group('accessibility')
 def accessibility():
     """ accessibility options. """
     pass
 
 
 @accessibility.command('capabilities', cls=Command)
-def accessibility_capabilities(lockdown):
+def accessibility_capabilities(lockdown: LockdownClient):
     """ display accessibility capabilities """
-    print_json(AccessibilityAudit(lockdown).device_capabilities())
+    print_json(AccessibilityAudit(lockdown).capabilities)
 
 
 @accessibility.group('settings')
 def accessibility_settings():
     """ accessibility settings. """
     pass
 
 
 @accessibility_settings.command('show', cls=Command)
-def accessibility_settings_show(lockdown):
+def accessibility_settings_show(lockdown: LockdownClient):
     """ show current settings """
-    for setting in AccessibilityAudit(lockdown).get_current_settings():
+    for setting in AccessibilityAudit(lockdown).settings:
         print(setting)
 
 
 @accessibility_settings.command('set', cls=Command)
-@click.argument('setting', type=click.Choice(
-    ['INVERT_COLORS', 'INCREASE_CONTRAST', 'REDUCE_TRANSPARENCY', 'REDUCE_MOTION', 'FONT_SIZE']))
-@click.argument('value', type=click.INT)
-def accessibility_settings_set(lockdown, setting, value):
-    """ show current settings """
+@click.argument('setting')
+@click.argument('value')
+def accessibility_settings_set(lockdown: LockdownClient, setting, value):
+    """
+    change current settings
+
+    in order to list all available use the "show" command
+    """
     service = AccessibilityAudit(lockdown)
-    service.set_setting(setting, value)
+    service.set_setting(setting, eval(value))
     wait_return()
 
 
 @accessibility.command('shell', cls=Command)
-def accessibility_shell(lockdown):
+def accessibility_shell(lockdown: LockdownClient):
     """ start and ipython accessibility shell """
     AccessibilityAudit(lockdown).shell()
 
 
 @accessibility.command('notifications', cls=Command)
-@click.option('-c', '--cycle-focus', is_flag=True)
-def accessibility_notifications(lockdown, cycle_focus):
+def accessibility_notifications(lockdown: LockdownClient):
     """ show notifications """
 
-    def callback(name, data):
-        if name in ('hostAppStateChanged:',
-                    'hostInspectorCurrentElementChanged:',):
-            for focus_item in data:
-                logging.info(focus_item)
-
-            if name == 'hostInspectorCurrentElementChanged:':
-                if cycle_focus:
-                    service.move_focus_next()
+    service = AccessibilityAudit(lockdown)
+    for event in service.iter_events():
+        if event.name in ('hostAppStateChanged:',
+                          'hostInspectorCurrentElementChanged:',):
+            for focus_item in event.data:
+                logger.info(focus_item)
+
+
+@accessibility.command('list-items', cls=Command)
+def accessibility_list_items(lockdown: LockdownClient):
+    """ list items available in currently shown menu """
 
     service = AccessibilityAudit(lockdown)
-    service.register_notifications_callback(callback)
-    if cycle_focus:
+    iterator = service.iter_events()
+
+    # every focus change is expected publish a "hostInspectorCurrentElementChanged:"
+    service.move_focus_next()
+
+    first_item = None
+
+    for event in iterator:
+        if event.name != 'hostInspectorCurrentElementChanged:':
+            # ignore any other events
+            continue
+
+        # each such event should contain exactly one element that became in focus
+        current_item = event.data[0]
+
+        if first_item is None:
+            first_item = current_item
+        else:
+            if first_item.caption == current_item.caption:
+                return
+
+        print(f'{current_item.caption}: {current_item.element.identifier}')
         service.move_focus_next()
-    service.listen_for_notifications()
 
 
 @developer.group('condition')
 def condition():
     """ condition inducer options. """
     pass
 
 
 @condition.command('list', cls=Command)
-def condition_list(lockdown):
+def condition_list(lockdown: LockdownClient):
     """ list all available conditions """
     with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
         print_json(ConditionInducer(dvt).list())
 
 
 @condition.command('clear', cls=Command)
-def condition_clear(lockdown):
+def condition_clear(lockdown: LockdownClient):
     """ clear current condition """
     with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
         ConditionInducer(dvt).clear()
 
 
 @condition.command('set', cls=Command)
 @click.argument('profile_identifier')
-def condition_set(lockdown, profile_identifier):
+def condition_set(lockdown: LockdownClient, profile_identifier):
     """ set a specific condition """
     with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
         ConditionInducer(dvt).set(profile_identifier)
         wait_return()
 
 
 @developer.command(cls=Command)
 @click.argument('out', type=click.File('wb'))
-def screenshot(lockdown, out):
+def screenshot(lockdown: LockdownClient, out):
     """ take a screenshot in PNG format """
     out.write(ScreenshotService(lockdown=lockdown).take_screenshot())
 
 
 @developer.group('debugserver')
 def debugserver():
     """ debugserver options. """
     pass
 
 
 @debugserver.command('applist', cls=Command)
-def debugserver_applist(lockdown):
+def debugserver_applist(lockdown: LockdownClient):
     """ get applist xml """
     print_json(DebugServerAppList(lockdown).get())
 
 
 @debugserver.command('start-server', cls=Command)
 @click.argument('local_port', type=click.INT)
-def debugserver_shell(lockdown, local_port):
+def debugserver_start_server(lockdown: LockdownClient, local_port):
     """
     start a debugserver at remote listening on a given port locally.
 
     Please note the connection must be done soon afterwards using your own lldb client.
     This can be done using the following commands within lldb shell:
 
-    - platform select remote-ios
+    (lldb) platform select remote-ios
 
-    - platform connect connect://localhost:<local_port>
+    (lldb) platform connect connect://localhost:<local_port>
     """
     attr = lockdown.get_service_connection_attributes('com.apple.debugserver.DVTSecureSocketProxy')
-    TcpForwarder(lockdown, local_port, attr['Port'], attr.get('EnableServiceSSL', False)).start()
+    TcpForwarder(local_port, attr['Port'], serial=lockdown.identifier,
+                 enable_ssl=attr.get('EnableServiceSSL', False)).start()
+
+
+@developer.group('arbitration')
+def arbitration():
+    """ arbitration options. """
+    pass
+
+
+@arbitration.command('version', cls=Command)
+@click.option('--color/--no-color', default=True)
+def version(lockdown: LockdownClient, color):
+    """ get arbitration version """
+    with DtDeviceArbitration(lockdown) as device_arbitration:
+        print_json(device_arbitration.version, colored=color)
+
+
+@arbitration.command('check-in', cls=Command)
+@click.argument('hostname')
+@click.option('-f', '--force', default=False, is_flag=True)
+def check_in(lockdown: LockdownClient, hostname, force):
+    """ owner check-in """
+    with DtDeviceArbitration(lockdown) as device_arbitration:
+        try:
+            device_arbitration.check_in(hostname, force=force)
+            wait_return()
+        except DeviceAlreadyInUseError as e:
+            logger.error(e.message)
+
+
+@arbitration.command('check-out', cls=Command)
+def check_out(lockdown: LockdownClient):
+    """ owner check-out """
+    with DtDeviceArbitration(lockdown) as device_arbitration:
+        device_arbitration.check_out()
+
+
+@dvt.command('har', cls=Command)
+def dvt_har(lockdown: LockdownClient):
+    """ enable har-logging """
+    with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
+        print('> Press Ctrl-C to abort')
+        with ActivityTraceTap(dvt, enable_http_archive_logging=True) as tap:
+            while True:
+                tap.channel.receive_message()
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/cli/diagnostics.py` & `pymobiledevice3-2.0.0/pymobiledevice3/cli/diagnostics.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,91 +1,96 @@
 import logging
 import time
-from pprint import pprint
 
 import click
+
 from pymobiledevice3.cli.cli_common import Command, print_json
+from pymobiledevice3.lockdown import LockdownClient
 from pymobiledevice3.services.diagnostics import DiagnosticsService
 
+logger = logging.getLogger(__name__)
+
 
 @click.group()
 def cli():
     """ apps cli """
     pass
 
 
 @cli.group()
 def diagnostics():
     """ diagnostics options """
     pass
 
 
 @diagnostics.command('restart', cls=Command)
-def diagnostics_restart(lockdown):
+def diagnostics_restart(lockdown: LockdownClient):
     """ restart device """
     DiagnosticsService(lockdown=lockdown).restart()
 
 
 @diagnostics.command('shutdown', cls=Command)
-def diagnostics_shutdown(lockdown):
+def diagnostics_shutdown(lockdown: LockdownClient):
     """ shutdown device """
     DiagnosticsService(lockdown=lockdown).shutdown()
 
 
 @diagnostics.command('sleep', cls=Command)
-def diagnostics_sleep(lockdown):
+def diagnostics_sleep(lockdown: LockdownClient):
     """ put device into sleep """
     DiagnosticsService(lockdown=lockdown).sleep()
 
 
 @diagnostics.command('info', cls=Command)
 @click.option('--color/--no-color', default=True)
-def diagnostics_info(lockdown, color):
+def diagnostics_info(lockdown: LockdownClient, color):
     """ get diagnostics info """
     print_json(DiagnosticsService(lockdown=lockdown).info(), colored=color)
 
 
 @diagnostics.command('ioregistry', cls=Command)
 @click.option('--plane')
 @click.option('--name')
 @click.option('--ioclass')
-def diagnostics_ioregistry(lockdown, plane, name, ioclass):
+@click.option('--color/--no-color', default=True)
+def diagnostics_ioregistry(lockdown: LockdownClient, plane, name, ioclass, color):
     """ get ioregistry info """
-    pprint(DiagnosticsService(lockdown=lockdown).ioregistry(plane=plane, name=name, ioclass=ioclass))
+    print_json(DiagnosticsService(lockdown=lockdown).ioregistry(plane=plane, name=name, ioclass=ioclass), colored=color)
 
 
 @diagnostics.command('mg', cls=Command)
 @click.argument('keys', nargs=-1, default=None)
-def diagnostics_mg(lockdown, keys):
+@click.option('--color/--no-color', default=True)
+def diagnostics_mg(lockdown: LockdownClient, keys, color):
     """ get MobileGestalt key values from given list. If empty, return all known. """
-    pprint(DiagnosticsService(lockdown=lockdown).mobilegestalt(keys=keys))
+    print_json(DiagnosticsService(lockdown=lockdown).mobilegestalt(keys=keys), colored=color)
 
 
 @diagnostics.group('battery')
 def diagnostics_battery():
     """ battery options """
     pass
 
 
 @diagnostics_battery.command('single', cls=Command)
 @click.option('--color/--no-color', default=True)
-def diagnostics_battery_single(lockdown, color):
+def diagnostics_battery_single(lockdown: LockdownClient, color):
     """ get single snapshot of battery data """
     raw_info = DiagnosticsService(lockdown=lockdown).get_battery()
     print_json(raw_info, colored=color)
 
 
 @diagnostics_battery.command('monitor', cls=Command)
-def diagnostics_battery_monitor(lockdown):
+def diagnostics_battery_monitor(lockdown: LockdownClient):
     """ monitor battery usage """
     diagnostics = DiagnosticsService(lockdown=lockdown)
     while True:
         raw_info = diagnostics.get_battery()
         info = {
             'InstantAmperage': raw_info.get('InstantAmperage'),
             'Temperature': raw_info.get('Temperature'),
             'Voltage': raw_info.get('Voltage'),
             'IsCharging': raw_info.get('IsCharging'),
             'CurrentCapacity': raw_info.get('CurrentCapacity'),
         }
-        logging.info(info)
+        logger.info(info)
         time.sleep(1)
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/cli/pcap.py` & `pymobiledevice3-2.0.0/pymobiledevice3/cli/pcap.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 from datetime import datetime
+from typing import IO
 
 import click
-from pygments import highlight, lexers, formatters
-import hexdump
+from pygments import formatters, highlight, lexers
 
-from pymobiledevice3.cli.cli_common import Command
+from pymobiledevice3.cli.cli_common import Command, print_hex
+from pymobiledevice3.lockdown import LockdownClient
 from pymobiledevice3.services.pcapd import PcapdService
 
 
 @click.group()
 def cli():
     """ apps cli """
     pass
 
 
+def print_packet_header(packet, color: bool):
+    date = datetime.fromtimestamp(packet.seconds + (packet.microseconds / 1000000))
+    data = (
+        f'{date}: '
+        f'Process {packet.comm} ({packet.pid}), '
+        f'Interface: {packet.interface_name} ({packet.interface_type.name}), '
+        f'Family: {packet.protocol_family.name}'
+    )
+    if not color:
+        print(data)
+    else:
+        print(highlight(data, lexers.HspecLexer(), formatters.TerminalTrueColorFormatter(style='native')), end='')
+
+
+def print_packet(packet, color: bool):
+    """ Return the packet so it can be chained in a generator """
+    print_packet_header(packet, color)
+    print_hex(packet.data, color)
+    return packet
+
+
 @cli.command(cls=Command)
 @click.argument('out', type=click.File('wb'), required=False)
 @click.option('-c', '--count', type=click.INT, default=-1, help='Number of packets to sniff. Omit to endless sniff.')
 @click.option('--process', default=None, help='Process to filter. Omit for all.')
 @click.option('--color/--no-color', default=True)
-def pcap(lockdown, out, count, process, color):
+def pcap(lockdown: LockdownClient, out: IO, count: int, process: str, color: bool):
     """ sniff device traffic """
     service = PcapdService(lockdown=lockdown)
     packets_generator = service.watch(packets_count=count, process=process)
+
     if out is not None:
-        service.write_to_pcap(out, packets_generator)
+        packets_generator_with_print = map(lambda p: print_packet(p, color), packets_generator)
+        service.write_to_pcap(out, packets_generator_with_print)
         return
 
-    formatter = formatters.TerminalTrueColorFormatter(style='native')
-
     for packet in packets_generator:
-        date = datetime.fromtimestamp(packet.seconds + (packet.microseconds / 1000000))
-        data = (
-            f'{date}: '
-            f'Process {packet.comm} ({packet.pid}), '
-            f'Interface: {packet.interface_name} ({packet.interface_type.name}), '
-            f'Family: {packet.protocol_family.name}'
-        )
-        if not color:
-            print(data)
-        else:
-            print(highlight(data, lexers.HspecLexer(), formatter), end='')
-        hex_dump = hexdump.hexdump(packet.data, result='return')
-        if color:
-            print(hex_dump, end='\n\n')
-        else:
-            print(highlight(hex_dump, lexers.HexdumpLexer(), formatter))
+        print_packet(packet, color)
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/cli/processes.py` & `pymobiledevice3-2.0.0/pymobiledevice3/cli/processes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-import click
 import logging
 
+import click
+
 from pymobiledevice3.cli.cli_common import Command, print_json
+from pymobiledevice3.lockdown import LockdownClient
 from pymobiledevice3.services.os_trace import OsTraceService
 
+logger = logging.getLogger(__name__)
+
 
 @click.group()
 def cli():
     """ apps cli """
     pass
 
 
@@ -15,21 +19,21 @@
 def processes():
     """ processes cli """
     pass
 
 
 @processes.command('ps', cls=Command)
 @click.option('--color/--no-color', default=True)
-def processes_ps(lockdown, color):
+def processes_ps(lockdown: LockdownClient, color):
     """ show process list """
     print_json(OsTraceService(lockdown=lockdown).get_pid_list().get('Payload'), colored=color)
 
 
 @processes.command('pgrep', cls=Command)
 @click.argument('expression')
-def processes_pgrep(lockdown, expression):
+def processes_pgrep(lockdown: LockdownClient, expression):
     """ try to match processes pid by given expression (like pgrep) """
     processes_list = OsTraceService(lockdown=lockdown).get_pid_list().get('Payload')
     for pid, process_info in processes_list.items():
         process_name = process_info.get('ProcessName')
         if expression in process_name:
-            logging.info(f'{pid} {process_name}')
+            logger.info(f'{pid} {process_name}')
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/cli/springboard.py` & `pymobiledevice3-2.0.0/pymobiledevice3/cli/springboard.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-import IPython
 import click
+import IPython
 
 from pymobiledevice3.cli.cli_common import Command, print_json
+from pymobiledevice3.lockdown import LockdownClient
 from pymobiledevice3.services.springboard import SpringBoardServicesService
 
 SHELL_USAGE = '''
-Use `service` to access the service features 
+Use `service` to access the service features
 '''
 
 
 @click.group()
 def cli():
     """ apps cli """
     pass
@@ -25,42 +26,42 @@
 def state():
     """ icons state options """
     pass
 
 
 @state.command('get', cls=Command)
 @click.option('--color/--no-color', default=True)
-def state_get(lockdown, color):
+def state_get(lockdown: LockdownClient, color):
     """ get icon state """
     print_json(SpringBoardServicesService(lockdown=lockdown).get_icon_state(), colored=color)
 
 
 @springboard.command('shell', cls=Command)
-def springboard_shell(lockdown):
+def springboard_shell(lockdown: LockdownClient):
     """ open a shell to communicate with SpringBoardServicesService """
     service = SpringBoardServicesService(lockdown=lockdown)
     IPython.embed(
         header=SHELL_USAGE,
         user_ns={
             'service': service,
         })
 
 
 @springboard.command('icon', cls=Command)
 @click.argument('bundle_id')
 @click.argument('out', type=click.File('wb'))
-def springboard_icon(lockdown, bundle_id, out):
+def springboard_icon(lockdown: LockdownClient, bundle_id, out):
     """ get application's icon """
     out.write(SpringBoardServicesService(lockdown=lockdown).get_icon_pngdata(bundle_id))
 
 
 @springboard.command('orientation', cls=Command)
-def springboard_orientation(lockdown):
+def springboard_orientation(lockdown: LockdownClient):
     """ get screen orientation """
     print(SpringBoardServicesService(lockdown=lockdown).get_interface_orientation())
 
 
 @springboard.command('wallpaper', cls=Command)
 @click.argument('out', type=click.File('wb'))
-def springboard_wallpaper(lockdown, out):
+def springboard_wallpaper(lockdown: LockdownClient, out):
     """ get wallpapaer """
     out.write(SpringBoardServicesService(lockdown=lockdown).get_wallpaper_pngdata())
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/cli/syslog.py` & `pymobiledevice3-2.0.0/pymobiledevice3/cli/syslog.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 import logging
 import os
+import posixpath
+import re
 
 import click
 from termcolor import colored
 
 from pymobiledevice3.cli.cli_common import Command
+from pymobiledevice3.lockdown import LockdownClient
 from pymobiledevice3.services.os_trace import OsTraceService
 from pymobiledevice3.services.syslog import SyslogService
 
+logger = logging.getLogger(__name__)
+
 
 @click.group()
 def cli():
-    """ apps cli """
+    """ syslog cli """
     pass
 
 
 @cli.group()
 def syslog():
     """ syslog options """
     pass
 
 
 @syslog.command('live-old', cls=Command)
-def syslog_live_old(lockdown):
+def syslog_live_old(lockdown: LockdownClient):
     """ view live syslog lines in raw bytes form from old relay """
     for line in SyslogService(lockdown=lockdown).watch():
         print(line)
 
 
 def format_line(color, pid, syslog_entry, include_label):
     log_level_colors = {
@@ -36,17 +41,17 @@
         'Warning': 'yellow',
     }
 
     syslog_pid = syslog_entry.pid
     timestamp = syslog_entry.timestamp
     level = syslog_entry.level
     filename = syslog_entry.filename
-    image_name = os.path.basename(syslog_entry.image_name)
+    image_name = posixpath.basename(syslog_entry.image_name)
     message = syslog_entry.message
-    process_name = os.path.basename(filename)
+    process_name = posixpath.basename(filename)
     label = ''
 
     if (pid != -1) and (syslog_pid != pid):
         return None
 
     if syslog_entry.label is not None:
         label = f'[{syslog_entry.label.subsystem}][{syslog_entry.label.category}]'
@@ -75,21 +80,37 @@
     return line
 
 
 @syslog.command('live', cls=Command)
 @click.option('-o', '--out', type=click.File('wt'), help='log file')
 @click.option('--color/--no-color', default=True, help='disable colors')
 @click.option('--pid', type=click.INT, default=-1, help='pid to filter. -1 for all')
+@click.option('-pn', '--process-name', help='process name to filter')
 @click.option('-m', '--match', multiple=True, help='match expression')
 @click.option('-mi', '--match-insensitive', multiple=True, help='insensitive match expression')
 @click.option('include_label', '--label', is_flag=True, help='should include label')
-def syslog_live(lockdown, out, color, pid, match, match_insensitive, include_label):
+@click.option('-e', '--regex', multiple=True, help='filter only lines matching given regex')
+@click.option('-ei', '--insensitive-regex', multiple=True, help='filter only lines matching given regex (insensitive)')
+def syslog_live(lockdown: LockdownClient, out, color, pid, process_name, match, match_insensitive, include_label, regex,
+                insensitive_regex):
     """ view live syslog lines """
 
+    match_regex = [re.compile(f'.*({r}).*') for r in regex]
+    match_regex += [re.compile(f'.*({r}).*', re.IGNORECASE) for r in insensitive_regex]
+
+    def replace(m):
+        if len(m.groups()):
+            return line.replace(m.group(1), colored(m.group(1), attrs=['bold', 'underline']))
+        return None
+
     for syslog_entry in OsTraceService(lockdown=lockdown).syslog(pid=pid):
+        if process_name:
+            if posixpath.basename(syslog_entry.filename) != process_name:
+                continue
+
         line = format_line(color, pid, syslog_entry, include_label)
 
         skip = False
 
         if match is not None:
             for m in match:
                 match_line = line
@@ -107,37 +128,49 @@
                 if m not in line.lower():
                     skip = True
                     break
                 else:
                     if color:
                         start = line.lower().index(m)
                         end = start + len(m)
-                        line = line[:start] + colored(m, attrs=['bold', 'underline']) + line[end:]
+                        line = line[:start] + colored(line[start:end], attrs=['bold', 'underline']) + line[end:]
+
+        if match_regex:
+            skip = True
+            for r in match_regex:
+                if not r.findall(line):
+                    continue
+
+                line = re.sub(r, replace, line)
+                skip = False
 
         if skip:
             continue
 
-        print(line)
+        print(line, flush=True)
 
         if out:
-            out.write(line)
+            print(line, file=out, flush=True)
 
 
 @syslog.command('collect', cls=Command)
 @click.argument('out', type=click.Path(exists=False, dir_okay=True, file_okay=True))
-def syslog_collect(lockdown, out):
+@click.option('--size-limit', type=click.INT)
+@click.option('--age-limit', type=click.INT)
+@click.option('--start-time', type=click.INT)
+def syslog_collect(lockdown: LockdownClient, out, size_limit, age_limit, start_time):
     """
     Collect the system logs into a .logarchive that can be viewed later with tools such as log or Console.
     If the filename doesn't exist, system_logs.logarchive will be created in the given directory.
     """
 
     if os.path.isdir(out):
         out = os.path.join(out, 'system_logs.logarchive')
 
     if not os.path.exists(out):
         os.makedirs(out)
 
     if not out.endswith('.logarchive'):
-        logging.warning('given out path doesn\'t end with a .logarchive - consider renaming to be able to view'
-                        'the file with the likes of the Console.app and the `log show` utilities')
+        logger.warning('given out path doesn\'t end with a .logarchive - consider renaming to be able to view '
+                       'the file with the likes of the Console.app and the `log show` utilities')
 
-    OsTraceService(lockdown=lockdown).collect(out)
+    OsTraceService(lockdown=lockdown).collect(out, size_limit=size_limit, age_limit=age_limit, start_time=start_time)
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/resources/dsc_uuid_map.json` & `pymobiledevice3-2.0.0/pymobiledevice3/resources/dsc_uuid_map.json`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/resources/dsc_uuid_map.py` & `pymobiledevice3-2.0.0/pymobiledevice3/resources/dsc_uuid_map.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 MAGIC = b'\x0b\x10\x00\x00'
 DYLD_MAGIC = b'dyld_v1'
 MAP_FILENAME = os.path.join(os.path.dirname(__file__), 'dsc_uuid_map.json')
 PARTITIONS = ('/System', '/usr', '/Applications', '/private')
 DYLD_UUID_OFFSET = 0x58
 UUID_SIZE = 0x10
 
+logger = logging.getLogger(__name__)
+
 
 def get_dsc_map(dsc_uuid):
     with open(MAP_FILENAME, 'r') as f:
         uuid_map = json.load(f)
 
     return uuid_map.get(dsc_uuid)
 
@@ -50,17 +52,17 @@
     if not dsc.startswith(DYLD_MAGIC):
         logging.error('invalid dsc file')
         return
 
     dsc_uuid = str(UUID(bytes=dsc[DYLD_UUID_OFFSET:DYLD_UUID_OFFSET + UUID_SIZE]))
 
     if dsc_uuid in uuid_map:
-        logging.warning(f'dsc {dsc_uuid} is already found in dsc_uuid_map')
+        logger.warning(f'dsc {dsc_uuid} is already found in dsc_uuid_map')
         if not force:
-            logging.info('exiting. use --force to force update')
+            logger.info('exiting. use --force to force update')
             return
     else:
         uuid_map[dsc_uuid] = {str(dyld_uuid): '/usr/lib/dyld'}
 
     for i in range(0, len(dsc) - 4, 4):
         # we can assume MAGIC is always aligned to 4
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/resources/firmware_notifications.py` & `pymobiledevice3-2.0.0/pymobiledevice3/resources/firmware_notifications.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/resources/notifications.txt` & `pymobiledevice3-2.0.0/pymobiledevice3/resources/notifications.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,462 +1,550 @@
 
-com.apple.awdd.anonymity
-com.apple.softwareupdateservicesd.activity.autoInstallEnd
-com.apple.spotlightui.prefschanged
-com.apple.duetexpertd.ATXMMAppPredictor.WiredAudioDeviceConnectedAnchor
-com.apple.awd.launch.nfcd
-com.apple.security.publickeynotavailable
-com.apple.bookmarks.BookmarksFileChanged
-com.apple.awd.launch.wifi
+com.apple.networkextension.app-paths-changed
+com.apple.ap.adprivacyd.iTunesActiveStorefrontDidChangeNotification
+com.apple.ManagedConfiguration.profileListChanged
+com.apple.mobileslideshow.ICPLStateChanged
+EKNotificationCountChangedExternallyNotification
+com.apple.tv.updateAppVisibility
+com.apple.bluetooth.connection
 com.apple.duetexpertd.ATXAnchorModel.invalidate.ChargerConnectedAnchor
-com.apple.timezonesync.idslaunchnotification
-com.apple.AirTunes.DACP.nextitem
-com.apple.healthlite.SleepSessionEndRequest
-com.apple.softwareupdateservicesd.activity.installAlert
-AppleDatePreferencesChangedNotification
-com.apple.MusicLibrary.importFinished-/var/mobile/Media/iTunes_Control/iTunes/MediaLibrary.sqlitedb
-com.apple.locationd.vehicle.disconnected
-com.apple.locationd.vehicle.exit
-com.apple.mobile.lockdown.activation_state
-com.apple.cddcommunicator.batteryChanged
-com.apple.duetexpertd.prefschanged
-com.apple.duetbm.internalSettingsChanged
-com.apple.voiceservices.trigger.asset-force-update
-com.apple.mobile.disk_image_mounted
-com.apple.SafariShared.Assistant.reload_plugin
-com.apple.coreduetd.knowledgebase.launch.duetexpertd
-kVMVoicemailTranscriptionTaskTranscribeAllVoicemails
-com.apple.touchsetupd.launch
-ConnectedGymPreferencesChangedNotification
-com.apple.calendar.database.preference.notification.kCalPreferredDaysToSyncKey
-MISProvisioningProfileInstalled
+com.apple.LaunchServices.ApplicationsChanged
 kCalEventOccurrenceCacheChangedNotification
-__ABDataBaseChangedByOtherProcessNotification
-com.apple.locationd.vehicular.changed.toVehicular
-com.apple.ap.adprivacyd.iTunesActiveAccountDidChangeNotification
-com.apple.duetexpertd.ATXScreenUnlockUpdateSource
-com.apple.appletv.backgroundstate
-com.apple.cloudd.pcsIdentityUpdate-com.apple.ProactivePredictionsBackup
-com.apple.ap.adprivacyd.canceltasks
-com.apple.AirTunes.DACP.volumeup
-com.apple.AOSNotification.FMIPStateDidChange
-com.apple.duetexpertd.ATXMMAppPredictor.IdleTimeEndAnchor
-com.apple.system.powersources.percent
-com.apple.TVRemoteCore.connectionRequested
-com.apple.GeoServices.navigation.started
-com.apple.mobiletimerd.resttest
-com.apple.MobileAsset.TimeZoneUpdate.ma.new-asset-installed
-com.apple.duetexpertd.ATXAnchorModel.invalidate.IdleTimeEndAnchor
-com.apple.duetexpertd.ATXAnchorModel.invalidate.CarPlayConnectedAnchor
-com.apple.system.logging.power_button_notification
-com.apple.homed.user-cloud-share.repair.wake.com.apple.applemediaservices.multiuser
-com.apple.nanoregistry.devicedidunpair
-com.apple.networkserviceproxy.reset
-com.apple.voicetrigger.enablePolicyChanged
-com.apple.duetexpertd.ms.nowplayingplay
-com.apple.siri.cloud.synch.changed
-com.apple.appstored.PodcastSubEntitlementsCacheUpdated
-com.apple.softwareupdateservicesd.activity.autoDownload
-com.apple.coreduetd.remoteDeviceChange
-com.apple.locationd.appreset
 com.apple.MobileAsset.ProactiveEventTrackerAssets.ma.new-asset-installed
-com.apple.duetexpertd.ATXMMAppPredictor.CarPlayDisconnectedAnchor
-com.apple.springboard.pluggedin
-com.apple.language.changed
-com.apple.assistant.sync_data_changed
-com.apple.assistant.sync_needed
-com.apple.AirTunes.DACP.shuffletoggle
-com.apple.system.powersources.criticallevel
-com.apple.MobileAsset.VoiceServices.VoiceResources.ma.new-asset-installed
-com.apple.CallHistoryPluginHelper.launchnotification
-com.apple.dataaccess.checkHolidayCalendarAccount
+com.apple.family.family_updated
+com.apple.mobilecal.invitationalertschanged
+com.apple.LoginKit.isLoggedIn
+com.apple.ams.privateListeningChanged
+com.apple.coreaudio.RoutingConfiguration
+com.apple.siri.ShortcutsCloudKitAccountAddedNotification
+com.apple.security.publickeyavailable
+com.apple.springboard.finishedstartup
+com.apple.AirTunes.DACP.play
+com.apple.softwareupdate.autoinstall.startInstall
+com.apple.ProtectedCloudStorage.updatedKeys
+com.apple.nanomusic.sync.defaults
+kAFPreferencesDidChangeDarwinNotification
+com.apple.siri.koa.donate
+com.apple.softwareupdateservicesd.activity.splatAutoScan
+com.apple.AirTunes.DACP.volumedown
 com.apple.appstored.ActivitySubEntitlementsCacheUpdated
-com.apple.ProtectedCloudStorage.test.mobileBackupStateChange
-com.apple.MobileAsset.VoiceTriggerAssetsWatch.ma.cached-metadata-updated
-com.apple.LaunchServices.applicationUnregistered
-com.apple.nanoregistry.watchdidbecomeactive
-com.apple.softwareupdateservicesd.activity.autoDownloadEnd
-com.apple.sleepd.diagnostics
-SBApplicationNotificationStateChanged
-com.apple.assistant.siri_settings_did_change
+com.apple.tv.appRemoved
+com.apple.mobilecal.preference.notification.weekStart
+com.apple.mobileipod.keeplocalstatechanged
+com.apple.accessibility.cache.invert.colors
+com.apple.duetexpertd.ATXAnchorModel.invalidate.BluetoothConnectedAnchor
+CNContactStoreMeContactDidChangeNotification
 com.apple.duetexpertd.ms.carplaydisconnect
-com.apple.system.thermalpressurelevel
-EKFeatureSetDidChangeNotification
-com.apple.mobile.lockdown.device_name_changed
-com.apple.triald.wake
-com.apple.bluetooth.connection
-com.apple.ap.adprivacyd.deviceKnowledge
-com.apple.idscredentials.idslaunchnotification
-com.apple.networkextension.nehelper-init
-com.apple.idsremoteurlconnection.idslaunchnotification
-com.apple.rapport.CompanionLinkDeviceAdded
-com.apple.imautomatichistorydeletionagent.prefchange
-com.apple.dataaccess.ping
-com.apple.cddcommunicator.thermalChanged
-com.apple.softwareupdate.autoinstall.startInstall
+com.apple.duetexpertd.ATXScreenUnlockUpdateSource
+com.apple.mobile.lockdown.activation_state
+com.apple.kvs.store-did-change.com.apple.iBooks
+com.apple.eventkit.preference.notification.UnselectedCalendarIdentifiersForFocusMode
+com.apple.security.cloudkeychain.forceupdate
+com.apple.datamigrator.migrationDidFinish
+com.apple.assistant.app_vocabulary
+com.apple.voicetrigger.enablePolicyChanged
+com.apple.duetexpertd.ATXAnchorModel.ChargerConnectedAnchor
+com.apple.security.view-ready.SE-PTC
+com.apple.MobileAsset.VoiceTriggerAssetsIPad.ma.cached-metadata-updated
+com.apple.duetexpertd.ms.nowplayingplay
+com.apple.security.octagon.peer-changed
+com.apple.softwareupdateservicesd.SUCoreConfigScheduledScan
+com.apple.ManagedConfiguration.webContentFilterChanged
+AppleKeyboardsPreferencesChangedNotification
+com.apple.mobile.keybagd.first_unlock
+com.apple.carkit.capabilities-changed
+com.apple.NanoPhotos.Library.changed
+SUPreferencesChangedNotification
+com.apple.kvs.store-did-change.com.apple.cloudsettings.keyboard
+com.apple.security.octagon.joined-with-bottle
+com.apple.EscrowSecurityAlert.server
+com.apple.telephonyutilities.callservicesd.fakeoutgoingmessage
+com.apple.duetexpertd.donationmonitor.intent
+com.apple.MediaRemote.nowPlayingActivePlayersIsPlayingDidChange
+com.apple.kvs.store-did-change.com.apple.sleepd
+com.apple.duetexpertd.mm.bluetoothconnected
 com.apple.security.view-change.PCS
-com.apple.suggestions.prepareForQuery
-com.apple.ams.provision-biometrics
-CKAccountChangedNotification
-com.apple.StoreServices.StorefrontChanged
-com.apple.carkit.carplay-attached
-com.apple.homed.televisionAccessoryAdded
-NewOperatorNotification
-com.apple.atc.xpc.runkeeplocaltask
+com.apple.trial.NamespaceUpdate.SIRI_VALUE_INFERENCE_CONTACT_RESOLUTION
+com.apple.cloud.quota.simulate.vfs.almostfull
 com.apple.dmd.iCloudAccount.didChange
-com.apple.mobiletimerd.reset
-com.apple.proactive.PersonalizationPortrait.namedEntitiesDidChangeMeaningfully
-com.apple.voiceservices.notification.voice-update
-com.apple.system.powersources.source
-com.apple.MobileAsset.SpeechEndpointAssets.cached-metadata-updated
-com.apple.telephonyutilities.callservicesd.fakeoutgoingmessage
+com.apple.system.batterysavermode.first_time
+com.apple.idscredentials.idslaunchnotification
+com.apple.triald.wake
+com.apple.system.lowpowermode.auto_disabled
+com.apple.UsageTrackingAgent.registration.application
+com.apple.system.batterysavermode
+com.apple.MobileAsset.VoiceServices.VoiceResources.new-asset-installed
+com.apple.MobileAsset.VoiceTriggerHSAssetsIPad.ma.new-asset-installed
+AppleDatePreferencesChangedNotification
 com.apple.duetexpertd.updateDefaultsDueToRelevantHomeScreenConfigUpdate
-com.apple.SensorKit.messagesUsageReport
-com.apple.MobileAsset.VoiceServices.GryphonVoice.ma.new-asset-installed
-com.apple.mobiletimerd.goodmorningtest
-com.apple.icloudpairing.idslaunchnotification
-com.apple.MobileAsset.AppleKeyServicesCRL.new-asset-installed
+com.apple.homed.AppleTVAccessoryAdded
+com.apple.photostream.idslaunchnotification
+SLSharedWithYouSettingHasChanged
+com.apple.MobileAsset.VoiceTriggerAssetsMarsh.ma.new-asset-installed
+com.apple.duetexpertd.ATXMMAppPredictor.WiredAudioDeviceDisconnectedAnchor
+com.apple.pasteboard.notify.changed
+com.apple.system.config.network_change
+com.apple.ProtectedCloudStorage.mobileBackupStateChange
+com.apple.corerecents.iCloudAccountChanged
+com.apple.duetexpertd.donationmonitor.activity
+com.apple.idsremoteurlconnection.idslaunchnotification
+com.apple.security.octagon.trust-status-change
+com.apple.icloud.searchparty.accessoryDidPair
+MISProvisioningProfileInstalled
+com.apple.ap.adprivacyd.iTunesActiveAccountDidChangeNotification
+com.apple.cloud.quota.simulate.vfs.notfull
+com.apple.softwareupdateservicesd.activity.installAlert
+com.apple.MobileAsset.VoiceTriggerAssets.ma.new-asset-installed
+com.apple.assistant.sync_needed
+com.apple.spotlightui.prefschanged
+com.apple.assistant.sync_homekit_now
+com.apple.AirTunes.DACP.pause
+com.apple.StoreServices.StorefrontChanged
 com.apple.smartcharging.defaultschanged
-com.apple.proactive.PersonalizationPortrait.namedEntitiesInvalidated
-com.apple.appstored.iCloudSubEntitlementsCacheUpdated
+com.apple.AirTunes.DACP.volumeup
+com.apple.MobileAsset.VoiceTriggerHSAssetsWatch.ma.cached-metadata-updated
+com.apple.mobileipod.displayvalueschanged
+com.apple.coreduetd.remoteDeviceChange
+com.apple.powerui.smartcharge
+com.apple.MobileAsset.VoiceServices.VoiceResources.ma.new-asset-installed
+com.apple.MobileAsset.VoiceTriggerHSAssetsIPad.ma.cached-metadata-updated
+com.apple.MusicLibrary.importFinished-/var/mobile/Media/iTunes_Control/iTunes/MediaLibrary.sqlitedb
+com.apple.mobiletimerd.chargetest
+com.apple.powermanagement.idlesleeppreventers
+com.apple.duetexpertd.clientModelRefreshBlendingLayer
+com.apple.nanoregistry.paireddevicedidchangeversion
+com.apple.duetexpertd.feedbackavailable
+com.apple.contacts.clientDidDisplayFavorites
+com.apple.appstored.NewsSubEntitlementsCacheUpdated
 com.apple.coreduetd.nearbydeviceschanged
-com.apple.telephonyutilities.callservicesd.fakeincomingmessage
-com.apple.siri.preheat.quiet
-com.apple.locationd.authorization
-com.apple.media.podcasts.siri_data_changed
+com.apple.networkextension.apps-changed
+AppleLanguagePreferencesChangedNotification
+CalSyncClientBeginningMultiSave
+com.apple.nanoregistry.devicedidpair
+com.apple.sleepd.ids.test
+com.apple.voiceservices.notification.voice-update
+com.apple.ProximityControl.LockScreenDiscovery
+com.apple.accessibility.cache.enhance.background.contrast
+com.apple.tv.TVWidgetExtension.Register
+com.apple.siri.cloud.synch.changed
+com.apple.system.lowpowermode
 com.apple.rapport.prefsChanged
-com.apple.mobilecal.preference.notification.calendarsExcludedFromNotifications
-com.apple.MobileAsset.VoiceServices.VoiceResources.new-asset-installed
-com.apple.chatkit.groups.siri_data_changed
-com.apple.hangtracerd.htse_state_changed
-com.apple.nanoregistry.paireddevicedidchangecapabilities
-com.apple.sockpuppet.applications.updated
-com.apple.idstransfers.idslaunchnotification
-com.apple.duetexpertd.ATXAnchorModel.invalidate.BluetoothConnectedAnchor
 kKeepAppsUpToDateEnabledChangedNotification
-com.apple.aggregated.addaily.logging
-com.apple.voicemail.changed
-com.apple.iokit.hid.displayStatus
-com.apple.ProtectedCloudStorage.rollIfAged
-com.apple.security.secureobjectsync.holdlock
-com.apple.duetexpertd.ATXMMAppPredictor.BluetoothConnectedAnchor
-com.apple.UsageTrackingAgent.registration.now-playing
-com.apple.photostream.idslaunchnotification
-com.apple.appstored.AppStoreSubEntitlementsCacheUpdated
+com.apple.powermanagement.restartpreventers
 com.apple.shortcuts.daemon-wakeup-request
-com.apple.AirTunes.DACP.pause
-com.apple.corespotlight.developer.ReindexAllItems
+com.apple.jett.switch.environmentChange.idms.complete
+com.apple.kvs.store-did-change.com.apple.cloudsettings.international
 com.apple.telephonyutilities.callservicesdaemon.voicemailcallended
-com.apple.mobilecal.invitationalertschanged
-VMStoreSetTokenNotification
-kFZVCAppBundleIdentifierLaunchNotification
-com.apple.cmfsyncagent.storedidchangeexternally
-kFZACAppBundleIdentifierLaunchNotification
-CalSyncClientFinishedMultiSave
-com.apple.duetexpertd.clientModelRefreshBlendingLayer
-com.apple.mobileslideshow.PLNotificationKeepOriginalsChanged
-com.apple.datamigrator.datamigrationcompletecontinuerestore
-com.apple.duetexpertd.defaultsChanged
-com.apple.nanomusic.sync.defaults
-com.apple.siri.ShortcutsCloudKitAccountAddedNotification
-CKIdentityUpdateNotification
-com.apple.GeoServices.PreferencesSync.SettingsChanged
-dmf.policy.monitor.app
-com.apple.system.timezone
-com.apple.MediaRemote.nowPlayingApplicationIsPlayingDidChange
-AppleNumberPreferencesChangedNotification
-com.apple.DuetHeuristic-BM.shutdowsoon
-com.apple.AirTunes.DACP.devicevolumechanged
-com.apple.duetexpertd.ms.nowplayingpause
-com.apple.voicemail.ReloadService
-com.apple.managedconfiguration.allowpasscodemodificationchanged
-com.apple.system.clock_set
-com.apple.nanoregistry.devicedidpair
-com.apple.ProtectedCloudStorage.rollBackupDisabled
 com.apple.nanophotos.prefs.LibraryCollectionTargetMapData-changed
-com.apple.powerui.requiredFullCharge
-com.apple.MobileAsset.ProactiveEventTrackerAssets.ma.cached-metadata-updated
-com.apple.SensorKit.visits
+com.apple.AirTunes.DACP.device-prevent-playback
+com.apple.appletv.backgroundstate
+com.apple.duetexpertd.ATXMMAppPredictor.CarPlayDisconnectedAnchor
+com.apple.nearfield.handoff.terminal
 com.apple.icloud.fmip.lostmode.enable
-com.apple.bluetooth.pairing
-com.apple.MobileAsset.VoiceServicesVocalizerVoice.ma.cached-metadata-updated
-com.apple.ProtectedCloudStorage.rollNow
-com.apple.LaunchServices.ApplicationsChanged
-com.apple.security.publickeyavailable
-INVoocabularyChangedNotification
+com.apple.AOSNotification.FMIPStateDidChange
+com.apple.navd.backgroundCommute.startPredicting
+com.apple.system.clock_set
+com.apple.ProtectedCloudStorage.rollBackupDisabled
+com.apple.accessibility.cache.reduce.motion
+com.apple.mobile.storage_unmounted
+com.apple.ap.aes
+com.apple.kvs.store-did-change.com.apple.cloudsettings.controlcenter
 com.apple.itunesstored.accountschanged
-com.apple.duetexpertd.ATXMMAppPredictor.BluetoothDisconnectedAnchor
-com.apple.duetexpertd.feedbackavailable
-com.apple.MobileAsset.SpeechEndpointAssets.ma.cached-metadata-updated
+com.apple.siri.inference.coreduet-context
+com.apple.mobileipod.noncontentspropertieschanged
+com.apple.bookmarks.BookmarksFileChanged
+com.apple.locationd.vehicle.exit
+com.apple.mobilemail.afc.poll
+com.apple.locationd.vehicle.disconnected
+com.apple.cmfsyncagent.kvstorechange
+com.apple.SafariShared.Assistant.reload_plugin
+RTLocationsOfInterestDidChangeNotification
+com.apple.ttsasset.NewAssetNotification
+com.apple.ap.adprivacyd.deviceKnowledge
 com.apple.purplebuddy.setupdone
-com.apple.ContinuityKeyBoard.enabled
-com.apple.cddcommunicator.pluginChanged
-com.apple.datamigrator.migrationDidFinish
-com.apple.MobileAsset.VoiceTriggerAssetsMarsh.ma.new-asset-installed
-com.apple.networkextension.app-paths-changed
-CNContactStoreMeContactDidChangeNotification
-com.apple.voicetrigger.XPCRestarted
-com.apple.duetexpertd.dockAppListCacheUpdate
-com.apple.ManagedConfiguration.webContentFilterChanged
-com.apple.softwareupdateservicesd.activity.delayEndScan
-com.apple.mobileipod-prefsChanged
-com.apple.ap.adprivacyd.iTunesActiveStorefrontDidChangeNotification
-com.apple.pex.connections.focalappchanged
-com.apple.Preferences.ChangedRestrictionsEnabledStateNotification
-com.apple.ManagedConfiguration.profileListChanged
-com.apple.AppleMediaServices.deviceOffersChanged
-com.apple.security.cloudkeychain.forceupdate
-com.apple.proactive.queries.databaseChange
-com.apple.system.hostname
-com.apple.pairedsync.syncDidComplete
-com.apple.thermalmonitor.ageAwareMitigationsEnabled
-com.apple.duetexpertd.ms.carplayconnect
-com.apple.geoservices.siri_data_changed
-com.apple.EscrowSecurityAlert.record
-com.apple.mobileslideshow.ICPLStateChanged
-com.apple.assistant.speech-capture.finished
-com.apple.homed.user-cloud-share.wake.com.apple.mediaservicesbroker.container
-com.apple.voicemail.VVVerifierCheckpointDictionaryChanged
-com.apple.bluetooth.WirelessSplitterOn
-com.apple.OTACrashCopier.SubmissionPreferenceChanged
-com.apple.MobileAsset.VoiceTriggerAssets.ma.cached-metadata-updated
-com.apple.homed.speakersConfiguredChanged
-com.apple.MobileAsset.VoiceTriggerAssets.ma.new-asset-installed
-com.apple.powermanagement.restartpreventers
-com.apple.tv.updateAppVisibility
-com.apple.duetexpertd.mm.audiodisconnect
-com.apple.Carousel.wristStateChanged
-FMFMeDeviceChangedNotification
-com.apple.VideosUI.UpNextRequestDidFinishNotification
-com.apple.voicetrigger.EarlyDetect
-com.apple.MobileAsset.TimeZoneUpdate.ma.cached-metadata-updated
-com.apple.parsecd.queries.clearData
-com.apple.SensorKit.deviceUsageReport
-com.apple.pushproxy.idslaunchnotification
-com.apple.security.tick
 HKHealthDaemonActiveWorkoutServersDidUpdateNotification
-com.apple.homed.user-cloud-share.wake.com.apple.siri.data
-com.apple.proactive.information.source.weather
-com.apple.duetexpertd.donationmonitor.intent
-VVMessageWaitingFallbackNotification
-com.apple.powermanagement.systemsleeppreventers
-com.apple.voicetrigger.PHSProfileModified
-ACDAccountStoreDidChangeNotification
-com.apple.icloud.searchparty.selfbeaconchanged
-com.apple.mobile.keybagd.first_unlock
+com.apple.MobileAsset.VoiceTriggerAssets.ma.cached-metadata-updated
+com.apple.ap.adprivacyd.reconcile
+com.apple.icloud.findmydeviced.findkit.magSafe.removed
+com.apple.siri.ShortcutsCloudKitAccountModifiedNotification
+com.apple.pairedsync.syncDidComplete
+kFZVCAppBundleIdentifierLaunchNotification
+com.apple.parsecd.bag
+com.apple.appstored.TVSubEntitlementsCacheUpdated
+com.apple.symptoms.materialLinkQualityChange
+com.apple.MobileAsset.VoiceTriggerAssets.new-asset-installed
+com.apple.MobileAsset.VoiceServicesVocalizerVoice.ma.cached-metadata-updated
+com.apple.duetexpertd.ATXAnchorModel.invalidate.CarPlayConnectedAnchor
+com.apple.navd.wakeUpForHypothesisUpdate
 com.apple.duetexpertd.mm.bluetoothdisconnect
-com.apple.MobileAsset.VoiceTriggerAssetsIPad.ma.new-asset-installed
-com.apple.corespotlight.developer.ReindexAllItemsWithIdentifiers
-com.apple.fitness.FitnessAppInstalled
+com.apple.duetexpertd.ATXMMAppPredictor.IdleTimeEndAnchor
+com.apple.mobilecal.timezonechanged
+com.apple.proactive.information.source.weather
+com.apple.MobileAsset.VoiceTriggerAssets.cached-metadata-updated
+com.apple.duetexpertd.ATXMMAppPredictor.BluetoothConnectedAnchor
+com.apple.voicetrigger.RemoteDarwin.ConnectionChanged
+com.apple.kvs.store-did-change.com.apple.cloudsettings.displays
+com.apple.mobileipod-prefsChanged
+com.apple.CallHistoryPluginHelper.launchnotification
+com.apple.exchangesyncd.ping
 com.apple.homehubd.endpointDeactivated
-logging tasks have changed
-com.apple.commcenter.InternationalRoamingEDGE.changed
-com.apple.nanoregistry.paireddevicedidchangeversion
-com.apple.remindd.nano_preferences_sync
-com.apple.UsageTrackingAgent.registration.application
-com.apple.screensharing.idslaunchnotification
-com.apple.MobileSoftwareUpdate.OSVersionChanged
-com.apple.softwareupdateservicesd.SUCoreConfigScheduledScan
-com.apple.nearfield.handoff.terminal
-SignificantTimeChangeNotification
-FMFFollowersChangedNotification
-com.apple.itunesstored.autodownloaddefaultschange
-com.apple.family.family_updated
-com.apple.da.tasking_changed
-com.apple.MobileAsset.SecureElementServiceAssets.ma.cached-metadata-updated
-com.apple.managedconfiguration.restrictionchanged
-com.apple.parsec-fbf.FLUploadImmediately
-com.apple.assistant.app_vocabulary
-com.apple.cloud.quota.simulate.vfs.almostfull
-com.apple.system.powermanagement.uservisiblepowerevent
-com.apple.cloud.quota.simulate.vfs.notfull
-com.apple.duetexpertd.ATXAnchorModel.invalidate.WiredAudioDeviceConnectedAnchor
+com.apple.wcd.wake-up
+com.apple.media.entities.siri_data_changed
+kFZACAppBundleIdentifierLaunchNotification
+com.apple.voicemail.changed
 PCPreferencesDidChangeNotification
-com.apple.bluetooth.accessory-authentication.success
-com.apple.homed.user-cloud-share.wake.com.apple.applemediaservices.multiuser
-AppleLanguagePreferencesChangedNotification
-com.apple.duetexpertd.appchangeprediction
-com.apple.siri.inference.coreduet-context
-com.apple.homed.user-cloud-share.wake.com.apple.siri.zonesharing
-com.apple.MobileAsset.CoreTextAssets.ma.new-asset-installed
-com.apple.GeoServices.countryCodeChanged
+CSLDisableWristDetectionChangedNotification
+com.apple.MobileAsset.TimeZoneUpdate.ma.new-asset-installed
+com.apple.springboard.lockstate
+com.apple.homed.televisionAccessoryAdded
+com.apple.locationd.vehicular.changed.toVehicular
+com.apple.duetexpertd.ms.nowplayingpause
+com.apple.mobileslideshow.PLNotificationKeepOriginalsChanged
+com.apple.voicetrigger.XPCRestarted
+com.apple.duetexpertd.ATXAnchorModel.invalidate.WiredAudioDeviceConnectedAnchor
+com.apple.assistant.sync_data_changed
+EKFeatureSetDidChangeNotification
+com.apple.MobileAsset.VoiceTriggerAssetsIPad.ma.new-asset-installed
+com.apple.system.powersources.criticallevel
+com.apple.tcc.access.changed
+com.apple.locationd.appreset
+com.apple.coreaudio.borealisTrigger
+logging tasks have changed
+com.apple.proactive.PersonalizationPortrait.namedEntitiesDidChangeMeaningfully
+com.apple.kvs.store-did-change.com.apple.cloudsettings.appearance
+com.apple.mobiletimerd.resttest
+com.apple.suggestions.settingsChanged
 com.apple.VideosUI.PlayHistoryUpdatedNotification
-com.apple.callhistorysync.idslaunchnotification
-com.apple.ManagedConfiguration.managedAppsChanged
-com.apple.ProtectedCloudStorage.updatedKeys
-com.apple.calendar.database.preference.notification.suggestEventLocations
-com.apple.powermanagement.idlesleeppreventers
-MFNanoMailImportantBridgeSettingHasChangedDarwinNotification
-com.apple.locationd/Prefs
-com.apple.mobiletimerd.bedtimetest
-com.apple.mobileipod.displayvalueschanged
-com.apple.UsageTrackingAgent.registration.video
-com.apple.MCX._managementStatusChangedForDomains
-com.apple.AirTunes.DACP.volumedown
+com.apple.thermalmonitor.ageAwareMitigationsEnabled
+com.apple.media.podcasts.siri_data_changed
+com.apple.voicemail.ReloadService
+com.apple.duetexpertd.ATXMMAppPredictor.WiredAudioDeviceConnectedAnchor
 com.apple.mobiletimerd.waketest
-com.apple.appstored.NewsSubEntitlementsCacheUpdated
+com.apple.AirTunes.DACP.shuffletoggle
+com.apple.MediaRemote.lockScreenControlsDidChange
+CNContactStoreDidChangeNotification
+com.apple.accessibility.cache.darken.system.colors.enabled
+com.apple.AirTunes.DACP.devicevolume
+com.apple.softwareupdateservicesd.activity.autoDownload
+com.apple.da.tasking_changed
+com.apple.fairplayd.resync-fpkeybag
+com.apple.SensorKit.deviceUsageReport
+com.apple.isp.backcamerapower
+com.apple.homed.user-cloud-share.wake.com.apple.siri.zonesharing
+com.apple.ProtectedCloudStorage.test.mobileBackupStateChange
+com.apple.triald.new-experiment
+com.apple.private.SensorKit.pedometer.stridecalibration
 com.apple.duetexpertd.homeScreenPageConfigCacheUpdate
-kCalBirthdayDefaultAlarmChangedNote
-com.apple.system.config.network_change
-com.apple.duetexpertd.ATXAnchorModel.BluetoothConnectedAnchor
+com.apple.homed.user-cloud-share.wake.com.apple.siri.data
+com.apple.UsageTrackingAgent.registration.now-playing
 com.apple.system.powermanagement.poweradapter
-com.apple.springboard.hasBlankedScreen
-com.apple.nfcacd.multitag.state.change
+com.apple.MobileAsset.VoiceServices.CustomVoice.ma.new-asset-installed
+com.apple.homed.user-cloud-share.wake.com.apple.applemediaservices.multiuser
+SBApplicationNotificationStateChanged
+com.apple.kvs.store-did-change.com.apple.cloudsettings.pencil
+com.apple.managedconfiguration.managedorginfochanged
+com.apple.callhistory.RecentsClearedNotification
+com.apple.wirelessproximity.launch
+MFNanoMailImportantBridgeSettingHasChangedDarwinNotification
 com.apple.mobiletimerd.wakeuptest
-kAFPreferencesDidChangeDarwinNotification
-com.apple.duetexpertd.ATXAnchorModel.ChargerConnectedAnchor
-com.apple.audio.AOP.enable
-com.apple.system.powermanagement.useractivity2
-com.apple.Music-AllowsCellularDataDownloads
-com.apple.security.itembackup
-com.apple.mobiletimerd.chargetest
-com.apple.isp.backcamerapower
-com.apple.MediaRemote.nowPlayingActivePlayersIsPlayingDidChange
-com.apple.itunescloudd.artworkDownloadsDidCompleteNotification
-com.apple.duetexpertd.ATXAnchorModel.CarPlayConnectedAnchor
-com.apple.duetexpertd.appclipprediction
-com.apple.symptoms.materialLinkQualityChange
-com.apple.siri.ShortcutsCloudKitAccountModifiedNotification
-com.apple.powermanagement.systempowerstate
-com.apple.security.secureobjectsync.circlechanged
-com.apple.mobiletimerd.diagnostics
-com.apple.corerecents.iCloudAccountChanged
-com.apple.proactive.queries.clearData
-com.apple.AirTunes.DACP.previtem
-com.apple.videos.migrationCompleted
-com.apple.cmfsyncagent.kvstorechange
-com.apple.mobilecal.timezonechanged
-com.apple.system.thermalpressurelevel.cold
-com.apple.MobileAsset.CoreTextAssets.ma.cached-metadata-updated
+NewOperatorNotification
+com.apple.MobileAsset.VoiceTriggerHSAssets.ma.cached-metadata-updated
+com.apple.siri.cloud.storage.deleted
+com.apple.commcenter.InternationalRoamingEDGE.changed
 com.apple.alarm.label.siri_data_changed
-com.apple.coreduet.idslaunchnotification
-com.apple.mobileipod.noncontentspropertieschanged
-kFaceTimeChangedNotification
-com.apple.MobileAsset.VoiceTriggerAssets.new-asset-installed
-com.apple.duetexpertd.mm.bluetoothconnected
-com.apple.trial.NamespaceUpdate.SIRI_VALUE_INFERENCE_CONTACT_RESOLUTION
-com.apple.UsageTrackingAgent.registration.web-domain
-com.apple.coremedia.carplayisconnected
-com.apple.powerlog.batteryServiceNotification
-com.apple.mobileipod.keeplocalstatechanged
+com.apple.idstransfers.idslaunchnotification
+com.apple.MobileAsset.AppleKeyServicesCRL.new-asset-installed
+com.apple.aggregated.addaily.logging
+com.apple.springboard.pluggedin
+com.apple.managedconfiguration.restrictionchanged
 com.apple.SensorKit.als
-AppleTimePreferencesChangedNotification
-CalSyncClientBeginningMultiSave
-com.apple.welcomemat.finalizeMigratableApps
-com.apple.reminder.list.name.siri_data_changed
-com.apple.duet.expertcenter.appRefresh
-com.apple.LoginKit.isLoggedIn
-NoteContextDarwinNotificationWithLoggedChanges
-com.apple.duetexpertd.donationmonitor.activity
-com.apple.LaunchServices.applicationRegistered
-com.apple.private.SensorKit.pedometer.stridecalibration
-com.apple.security.secureobjectsync.viewschanged
+com.apple.powerlog.batteryServiceNotification
+com.apple.system.logging.power_button_notification
+com.apple.ManagedConfiguration.managedAppsChanged
+com.apple.bluetooth.WirelessSplitterOn
+com.apple.accessibility.component-change
+com.apple.MobileAsset.Font7.ma.cached-metadata-updated
+com.apple.appstored.AppStoreSubEntitlementsCacheUpdated
+com.apple.itunesstored.autodownloaddefaultschange
+com.apple.managedconfiguration.effectivesettingschanged
+com.apple.mobileipod.librarychanged
+com.apple.mobiletimerd.bedtimetest
+com.apple.MobileAsset.CoreTextAssets.ma.new-asset-installed
+com.apple.atc.xpc.runkeeplocaltask
+com.apple.coremedia.carplayisconnected
+com.apple.dataaccess.checkHolidayCalendarAccount
+com.apple.MediaRemote.nowPlayingApplicationIsPlayingDidChange
+com.apple.imautomatichistorydeletionagent.prefchange
+com.apple.proactive.queries.databaseChange
+__ABDataBaseChangedByOtherProcessNotification
+com.apple.pushproxy.idslaunchnotification
+com.apple.isp.frontcamerapower
+com.apple.security.view-change.SE-PTC
 FMFDataUpdateCompleteNotification
-com.apple.MobileAsset.SecureElementServiceAssets.ma.new-asset-installed
-com.apple.softwareupdateservicesd.activity.autoInstallUnlock
-com.apple.remotemanagement.accountsChanged
-MISProvisioningProfileRemoved
-com.apple.softwareupdateservicesd.activity.autoScan
-FMFDevicesChangedNotification
-com.apple.homed.AppleTVAccessoryAdded
-com.apple.exchangesyncd.ping
-com.apple.BiometricKit.passcodeGracePeriodChanged
-com.apple.sleep.sync.SleepScheduleDidChange
-com.apple.security.octagon.trust-status-change
-com.apple.sbd.kvstorechange
-AFLanguageCodeDidChangeDarwinNotification
-com.apple.callhistory.RecentsClearedNotification
-com.apple.coreduet.client-needs-help.coreduetd
-com.apple.dmd.budget.didChange
-com.apple.security.cloudkeychainproxy.kvstorechange3
-com.apple.AirTunes.DACP.devicevolume
-com.apple.purplebuddy.setupexited
+AppleTimePreferencesChangedNotification
+com.apple.spotlight.SyndicatedContentRefreshed
+com.apple.duetexpertd.dockAppListCacheUpdate
+com.apple.geoservices.siri_data_changed
+com.apple.cmfsyncagent.storedidchangeexternally
+com.apple.system.powersources.timeremaining
+com.apple.MobileAsset.SpeechEndpointAssets.ma.cached-metadata-updated
+com.apple.icloud.searchparty.selfbeaconchanged
+com.apple.homed.user-cloud-share.wake.com.apple.applemediaservices.multiuser.qa
+com.apple.AirTunes.DACP.previtem
+com.apple.trial.NamespaceUpdate.SIRI_UNDERSTANDING_ASR_ASSISTANT
+com.apple.accessories.connection.MFi4AccessoryDisconnected
+com.apple.ManagedConfiguration.webContentFilterTypeChanged
+com.apple.voicemail.VVVerifierCheckpointDictionaryChanged
+com.apple.UsageTrackingAgent.registration.video
+com.apple.carkit.carplay-attached
+com.apple.itunescloudd.artworkDownloadsDidCompleteNotification
+com.apple.sleepd.cloudkit.reset
+com.apple.SoftwareUpdate.SUPreferencesChanged
+com.apple.managedconfiguration.passcodechanged
+com.apple.springboard.hasBlankedScreen
+com.apple.softwareupdateservicesd.activity.autoInstallEnd
+com.apple.cloudrecents.kvstorechange
+com.apple.softwareupdateservicesd.activity.presentBanner
+com.apple.awd.launch.nfcd
 com.apple.cddcommunicator.nwchanged
-com.apple.parsecd.bag
-com.apple.VideosUI.StoreAcquisitionCrossProcessNotification
-com.apple.AirTunes.DACP.device-prevent-playback
-com.apple.ams.privateListeningChanged
-com.apple.triald.new-experiment
+com.apple.proactive.PersonalizationPortrait.namedEntitiesInvalidated
+com.apple.assistant.sync_homekit_urgent
+com.apple.duetexpertd.appclipprediction
+com.apple.sockpuppet.applications.updated
+com.apple.mobile.lockdown.device_name_changed
+CKIdentityUpdateNotification
+com.apple.videos.migrationCompleted
 com.apple.homed.multi-user-status-changed
-com.apple.suggestions.settingsChanged
-com.apple.contacts.clientDidDisplayFavorites
-com.apple.duetexpertd.ATXAnchorModel.WiredAudioDeviceConnectedAnchor
+com.apple.MobileAsset.ProactiveEventTrackerAssets.ma.cached-metadata-updated
+com.apple.ap.adprivacyd.launch
+com.apple.AirTunes.DACP.mutetoggle
+com.apple.ap.adprivacyd.canceltasks
+com.apple.TVRemoteCore.connectionRequested
+com.apple.system.lowpowermode.first_time
+com.apple.MobileAsset.CoreTextAssets.ma.cached-metadata-updated
+com.apple.duetexpertd.mm.audiodisconnect
+com.apple.hangtracerd.htse_state_changed
+com.apple.sleep.sync.SleepScheduleDidChange
+com.apple.powerui.requiredFullCharge
+com.apple.DuetHeuristic-BM.shutdowsoon
+com.apple.datamigrator.datamigrationcompletecontinuerestore
+NanoLifestylePreferencesChangedNotification
+com.apple.icloud.findmydeviced.findkit.magSafe.added
+com.apple.homekit.sync-data-cache-updated
+com.apple.assistant.siri_settings_did_change
+com.apple.proactive.queries.clearData
+com.apple.corespotlight.developer.ReindexAllItemsWithIdentifiers
+com.apple.corespotlight.developer.ReindexAllItems
+com.apple.cddcommunicator.pluginChanged
+com.apple.language.changed
+com.apple.rapport.CompanionLinkDeviceAdded
+com.apple.voicetrigger.EarlyDetect
+com.apple.voiceservices.trigger.asset-force-update
+MPStoreClientTokenDidChangeNotification
 com.apple.VideoSubscriberAccount.DidRegisterSubscription
-com.apple.pasteboard.notify.changed
-com.apple.system.batterysavermode
-com.apple.EscrowSecurityAlert.server
-com.apple.MobileAsset.VoiceTriggerAssetsMarsh.ma.cached-metadata-updated
-com.apple.MediaRemote.nowPlayingInfoDidChange
-com.apple.media.entities.siri_data_changed
-com.apple.softwareupdateservicesd.activity.emergencyAutoScan
-com.apple.wirelessproximity.launch
-com.apple.MobileAsset.VoiceTriggerAssets.cached-metadata-updated
-NewCarrierNotification
-com.apple.homehubd.endpointActivated
-com.apple.ProtectedCloudStorage.mobileBackupStateChange
-BYSetupAssistantFinishedDarwinNotification
-com.apple.ap.adprivacyd.reconcile
-com.apple.mobileipod.librarychanged
-com.apple.managedconfiguration.passcodechanged
-EKNotificationCountChangedExternallyNotification
-com.apple.MobileAsset.VoiceTriggerAssetsWatch.ma.new-asset-installed
-com.apple.icloud.fmip.siri_data_changed
-com.apple.MobileAsset.VoiceTriggerAssetsIPad.ma.cached-metadata-updated
-com.apple.carkit.capabilities-changed
-com.apple.mobileme.fmf1.allowFindMyFriendsModification
-com.apple.trial.NamespaceUpdate.FREEZER_POLICIES
-com.apple.Sharing.prefsChanged
+com.apple.kvs.store-did-change.com.apple.cloudsettings.mouse
+com.apple.MobileAsset.VoiceTriggerAssetsWatch.new-asset-installed
+ConnectedGymPreferencesChangedNotification
+_CalDatabaseChangedNotification
+com.apple.powermanagement.systemsleeppreventers
+com.apple.MobileAsset.EmbeddedSpeech.ma.new-asset-installed
+com.apple.OTACrashCopier.SubmissionPreferenceChanged
+com.apple.duetexpertd.ms.carplayconnect
+com.apple.SensorKit.messagesUsageReport
+com.apple.sleep.sync.SleepRecordDidChange
+com.apple.healthlite.SleepSessionEndRequest
+com.apple.welcomemat.finalizeMigratableApps
+com.apple.Carousel.wristStateChanged
+com.apple.networkserviceproxy.reset
+ACDAccountStoreDidChangeNotification
+com.apple.EscrowSecurityAlert.reset
+CalSyncClientFinishedMultiSave
+com.apple.mobiletimerd.reset
 com.apple.mobileipod.libraryimportdidfinish
+com.apple.security.publickeynotavailable
+com.apple.Music-AllowsCellularDataDownloads
+com.apple.siri.preheat.quiet
+com.apple.AirTunes.DACP.nextitem
+com.apple.duetbm.internalSettingsChanged
+com.apple.parsecd.queries.clearData
 com.apple.duetexpertd.ATXMMAppPredictor.CarPlayConnectedAnchor
+MISProvisioningProfileRemoved
+com.apple.siri.power.PowerContextPolicy.updated
+com.apple.bluetooth.accessory-authentication.success
+com.apple.dmd.budget.didChange
+com.apple.icloud.fmip.siri_data_changed
+com.apple.SensorKit.visits
+NoteContextDarwinNotificationWithLoggedChanges
+com.apple.mobile.keybagd.lock_status
+com.apple.healthlite.SleepDetectedActivity
 com.apple.locationd.vehicle.connected
-com.apple.navd.wakeUpForHypothesisUpdate
-com.apple.ap.adprivacyd.launch
-com.apple.NanoPhotos.Library.changed
-com.apple.softwareupdateservicesd.activity.presentBanner
-com.apple.bluetooth.daemonStarted
+com.apple.mobiletimerd.goodmorningtest
+com.apple.UsageTrackingAgent.registration.web-domain
+com.apple.assistant.speech-capture.finished
+com.apple.awd.launch.wifi
+com.apple.duetexpertd.ATXAnchorModel.WiredAudioDeviceConnectedAnchor
+com.apple.devicemanagementclient.longLivedTokenChanged
+com.apple.VideosUI.UpNextRequestDidFinishNotification
+com.apple.MobileAsset.TTSAXResourceModelAssets.ma.new-asset-installed
 com.apple.system.batterysavermode.auto_disabled
-com.apple.assistant.sync_homekit_now
-com.apple.EscrowSecurityAlert.reset
-com.apple.navd.backgroundCommute.startPredicting
-com.apple.cloudrecents.kvstorechange
-com.apple.springboard.lockstate
-com.apple.powerui.smartcharge
-com.apple.Preferences.ResetPrivacyWarningsNotification
-com.apple.tv.appRemoved
+com.apple.MCX._managementStatusChangedForDomains
+com.apple.softwareupdateservicesd.activity.autoDownloadEnd
+com.apple.coreduet.client-needs-help.coreduetd
+com.apple.fitness.FitnessAppInstalled
+NewCarrierNotification
+com.apple.duetexpertd.ATXAnchorModel.IdleTimeEndAnchor
+com.apple.softwareupdateservicesd.activity.autoInstallUnlock
+com.apple.icloud.findmydeviced.localActivationLockInfoChanged
+com.apple.calendar.database.preference.notification.kCalPreferredDaysToSyncKey
+com.apple.accessibility.cache.enhance.text.legibility
+com.apple.security.cloudkeychainproxy.kvstorechange3
+com.apple.MobileAsset.TimeZoneUpdate.ma.cached-metadata-updated
+com.apple.softwareupdateservicesd.activity.delayEndScan
+com.apple.trial.NamespaceUpdate.FREEZER_POLICIES
+com.apple.ams.provision-biometrics
+com.apple.cddcommunicator.batteryChanged
+com.apple.icloud.findmydeviced.findkit.magSafe.detach
+com.apple.powermanagement.systempowerstate
+com.apple.icloud.FindMy.addMagSafeAccessory
 com.apple.GeoServices.navigation.stopped
-com.apple.siri.cloud.storage.deleted
-com.apple.duetexpertd.ATXMMAppPredictor.WiredAudioDeviceDisconnectedAnchor
-com.apple.mobilecal.preference.notification.weekStart
-MPStoreClientTokenDidChangeNotification
-com.apple.isp.frontcamerapower
+kVMVoicemailTranscriptionTaskTranscribeAllVoicemails
+com.apple.BiometricKit.passcodeGracePeriodChanged
+INVoocabularyChangedNotification
+com.apple.SynthesisProvider.updatedVoices
+com.apple.security.tick
+com.apple.security.secureobjectsync.circlechanged
+com.apple.security.itembackup
+com.apple.Preferences.ChangedRestrictionsEnabledStateNotification
+com.apple.parsec-fbf.FLUploadImmediately
+com.apple.cddcommunicator.thermalChanged
+com.apple.system.thermalpressurelevel.cold
+AppleNumberPreferencesChangedNotification
+com.apple.kvs.store-did-change.com.apple.cloudsettings.sound
+com.apple.stockholm.se.mfd
+com.apple.security.secureobjectsync.viewschanged
+SignificantTimeChangeNotification
+com.apple.softwareupdateservicesd.activity.emergencyAutoScan
+com.apple.dataaccess.ping
+com.apple.MobileSoftwareUpdate.OSVersionChanged
+kCalBirthdayDefaultAlarmChangedNote
+com.apple.system.timezone
+com.apple.calendar.database.preference.notification.suggestEventLocations
+com.apple.duetexpertd.ATXAnchorModel.invalidate.IdleTimeEndAnchor
+com.apple.homehubd.endpointActivated
+com.apple.system.powersources.percent
+com.apple.duetexpertd.appchangeprediction
+com.apple.system.thermalpressurelevel
+com.apple.timezonesync.idslaunchnotification
+com.apple.MobileAsset.VoiceTriggerHSAssetsWatch.ma.new-asset-installed
+com.apple.mobilecal.preference.notification.calendarsExcludedFromNotifications
+com.apple.system.powersources.source
+com.apple.duetexpertd.ATXMMAppPredictor.BluetoothDisconnectedAnchor
+com.apple.reminder.list.name.siri_data_changed
+com.apple.managedconfiguration.allowpasscodemodificationchanged
+com.apple.nanoregistry.devicedidunpair
+com.apple.homed.user-cloud-share.wake.com.apple.mediaservicesbroker.container
+com.apple.MobileAsset.VoiceServices.GryphonVoice.ma.new-asset-installed
+com.apple.awdd.anonymity
+com.apple.appstored.iCloudSubEntitlementsCacheUpdated
+SLSharedWithYouAppSettingHasChanged
+com.apple.nanoregistry.paireddevicedidchangecapabilities
 com.apple.SensorKit.phoneUsageReport
-com.apple.mobilemail.afc.poll
-com.apple.wcd.wake-up
-com.apple.duetexpertd.ATXAnchorModel.IdleTimeEndAnchor
-_CalDatabaseChangedNotification
-com.apple.appstored.TVSubEntitlementsCacheUpdated
-com.apple.siri.client.state.DynamiteClientState.siri_data_changed
-com.apple.managedconfiguration.effectivesettingschanged
-com.apple.AirTunes.DACP.play
-com.apple.appstored.MusicSubEntitlementsCacheUpdated
-com.apple.healthlite.SleepDetectedActivity
-com.apple.coreaudio.speechDetectionVAD.created
-com.apple.springboard.finishedstartup
-CNFavoritesChangedExternallyNotification
-com.apple.AirTunes.DACP.mutetoggle
+com.apple.LaunchServices.applicationRegistered
 com.apple.AirTunes.DACP.repeatadv
-com.apple.tv.TVWidgetExtension.Register
-com.apple.networkextension.apps-changed
-com.apple.homed.user-cloud-share.wake.com.apple.applemediaservices.multiuser.qa
-com.apple.MobileAsset.VoiceTriggerAssetsWatch.new-asset-installed
-com.apple.ManagedConfiguration.webContentFilterTypeChanged
-com.apple.mobile.keybagd.lock_status
-com.apple.managedconfiguration.managedorginfochanged
-CNContactStoreDidChangeNotification
-com.apple.tcc.access.changed
+com.apple.audio.AOP.enable
+com.apple.locationd/Prefs
+security.mac.amfi.developer_mode_status.changed
+com.apple.MobileAsset.SpeechEndpointAssets.cached-metadata-updated
+com.apple.siri.inference.biome-context
+com.apple.sbd.kvstorechange
+com.apple.system.powermanagement.useractivity2
+com.apple.coreaudio.speechDetectionVAD.created
+com.apple.ProtectedCloudStorage.rollIfAged
+com.apple.MediaRemote.nowPlayingInfoDidChange
+com.apple.locationd.authorization
+com.apple.GeoServices.navigation.started
+com.apple.MobileAsset.SecureElementServiceAssets.ma.new-asset-installed
+com.apple.softwareupdateservicesd.activity.autoScan
+com.apple.kvs.store-did-change.com.apple.cloudsettings.trackpad
+com.apple.purplebuddy.setupexited
+com.apple.remindd.nano_preferences_sync
+com.apple.voicetrigger.RemoteDarwin.EarlyDetect
 com.apple.itunesstored.invalidatebags
-com.apple.coreaudio.RoutingConfiguration
-AppleKeyboardsPreferencesChangedNotification
-com.apple.MobileAsset.EmbeddedSpeech.ma.new-asset-installed
-com.apple.coreaudio.borealisTrigger
-com.apple.system.batterysavermode.first_time
-com.apple.fairplayd.resync-fpkeybag
+com.apple.EscrowSecurityAlert.record
+com.apple.ContinuityKeyBoard.enabled
+com.apple.iokit.hid.displayStatus
+com.apple.system.powermanagement.uservisiblepowerevent
+com.apple.nanoregistry.watchdidbecomeactive
+com.apple.softwareupdateservicesd.activity.rollbackReboot
+FMFFollowersChangedNotification
+FMFMeDeviceChangedNotification
+com.apple.MobileAsset.SecureElementServiceAssets.ma.cached-metadata-updated
+com.apple.duetexpertd.ATXAnchorModel.BluetoothConnectedAnchor
+com.apple.security.secureobjectsync.holdlock
+com.apple.pex.connections.focalappchanged
+com.apple.Sharing.prefsChanged
+com.apple.system.hostname
+com.apple.appstored.PodcastSubEntitlementsCacheUpdated
+com.apple.kvs.store-did-change.com.apple.cloudsettings.gamecontroller
+com.apple.MobileAsset.VoiceTriggerAssetsWatch.ma.new-asset-installed
+com.apple.callhistorysync.idslaunchnotification
+com.apple.icloud.findmydeviced.findkit.magSafe.attach
+SPSpotlightRecentsCacheDidChange
+com.apple.screensharing.idslaunchnotification
+com.apple.mobileme.fmf1.allowFindMyFriendsModification
+com.apple.chatkit.groups.siri_data_changed
+com.apple.GeoServices.countryCodeChanged
+com.apple.MobileAsset.VoiceTriggerAssetsWatch.ma.cached-metadata-updated
+com.apple.remotemanagement.accountsChanged
+com.apple.duetexpertd.defaultsChanged
+com.apple.AirTunes.DACP.devicevolumechanged
+com.apple.accessibility.cache.differentiate.without.color
+com.apple.mobiletimerd.diagnostics
+com.apple.ProtectedCloudStorage.rollNow
+com.apple.sleepd.diagnostics
+com.apple.touchsetupd.launch
+com.apple.trial.NamespaceUpdate.SIRI_DICTATION_ASSETS
+com.apple.cloudd.pcsIdentityUpdate-com.apple.ProactivePredictionsBackup
+com.apple.trial.NamespaceUpdate.NETWORK_SERVICE_PROXY_CONFIG_UPDATE
+BYSetupAssistantFinishedDarwinNotification
+com.apple.siri.client.state.DynamiteClientState.siri_data_changed
+com.apple.Preferences.ResetPrivacyWarningsNotification
+kFaceTimeChangedNotification
+FMFDevicesChangedNotification
+VVMessageWaitingFallbackNotification
+CKAccountChangedNotification
+com.apple.MobileAsset.VoiceTriggerAssetsMarsh.ma.cached-metadata-updated
+com.apple.coreduetd.knowledgebase.launch.duetexpertd
+com.apple.MobileBackup.backgroundCellularAccessChanged
+com.apple.homed.user-cloud-share.repair.wake.com.apple.applemediaservices.multiuser
+com.apple.suggestions.prepareForQuery
+AFLanguageCodeDidChangeDarwinNotification
+com.apple.networkextension.nehelper-init
+com.apple.GeoServices.PreferencesSync.SettingsChanged
+com.apple.homed.speakersConfiguredChanged
+ApplePreferredContentSizeCategoryChangedNotification
+dmf.policy.monitor.app
+com.apple.voicetrigger.PHSProfileModified
+com.apple.duet.expertcenter.appRefresh
+com.apple.duetexpertd.ATXAnchorModel.CarPlayConnectedAnchor
+com.apple.icloudpairing.idslaunchnotification
+com.apple.accessories.connection.passedMFi4Auth
+com.apple.bluetooth.daemonStarted
+CNFavoritesChangedExternallyNotification
+VMStoreSetTokenNotification
+com.apple.spotlight.SyndicatedContentDeleted
+com.apple.coreduet.idslaunchnotification
+com.apple.appstored.MusicSubEntitlementsCacheUpdated
+com.apple.trial.NamespaceUpdate.SIRI_TEXT_TO_SPEECH
+com.apple.MobileAsset.VoiceTriggerHSAssets.ma.new-asset-installed
+com.apple.CloudSubscriptionFeature.Changed
+com.apple.bluetooth.pairing
+com.apple.telephonyutilities.callservicesd.fakeincomingmessage
+com.apple.mobile.disk_image_mounted
+com.apple.kvs.store-did-change.com.apple.cloudsettings.desktop
+com.apple.sleep.sync.SleepSettingsDidChange
+com.apple.nfcacd.multitag.state.change
+com.apple.VideosUI.StoreAcquisitionCrossProcessNotification
+com.apple.duetexpertd.prefschanged
+com.apple.kvs.store-did-change.com.apple.cloudsettings.general
+com.apple.LaunchServices.applicationUnregistered
+com.apple.AppleMediaServices.deviceOffersChanged
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/restore/restore.py` & `pymobiledevice3-2.0.0/pymobiledevice3/restore/recovery.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,460 +1,470 @@
+import hashlib
 import logging
-import plistlib
 import time
-import zipfile
-from io import BytesIO
+import typing
+from zipfile import ZipFile
 
-import asn1
 from usb import USBError
 
 from pymobiledevice3.exceptions import PyMobileDevice3Exception
-from pymobiledevice3.irecv import IRecv
+from pymobiledevice3.irecv import IRecv, Mode
 from pymobiledevice3.lockdown import LockdownClient
+from pymobiledevice3.restore.base_restore import BaseRestore, Behavior
+from pymobiledevice3.restore.consts import lpol_file
+from pymobiledevice3.restore.device import Device
 from pymobiledevice3.restore.tss import TSSRequest
-from pymobiledevice3.services.preboard import PreboardService
 
-
-class RestoreService:
-    def __init__(self, lockdown: LockdownClient, ipsw: BytesIO, tss=None):
-        self.ipsw = zipfile.ZipFile(ipsw)
-        self.tss = tss
-
-        self._lockdown = lockdown
-        self.hardware_model = self._lockdown.all_values['HardwareModel'].lower()
-        self.ecid = self._lockdown.all_values['UniqueChipID']
-        self.build_version = self._lockdown.all_values['BuildVersion']
-        self.build_major = int(self.build_version[:2])
-        self.is_image4_supported = self._lockdown.get_value(key='Image4Supported')
-
-        if not self.is_image4_supported:
-            raise NotImplementedError('is_image4_supported is False')
-
-        logging.info(f'connected device: <ecid: {self.ecid} chipset: {self.hardware_model} build: {self.build_version} '
-                     f'image4-support: {self.is_image4_supported}>')
-
-        self.build_identity = None
-
-        logging.debug('scanning BuildManifest.plist for the correct BuildIdentity')
-        self.build_manifest = plistlib.loads(self.ipsw.read('BuildManifest.plist'))
-        for build_identity in self.build_manifest['BuildIdentities']:
-            device_class = build_identity['Info']['DeviceClass'].lower()
-            restore_behavior = build_identity['Info']['RestoreBehavior']
-            logging.debug(f'iterating: class: {device_class} behavior: {restore_behavior}')
-            if (device_class == self.hardware_model) and (restore_behavior == 'Update'):
-                self.build_identity = build_identity
-                break
-
-        if self.build_identity is None:
-            raise PyMobileDevice3Exception('failed to find the correct BuildIdentity from the BuildManifest.plist')
-
-        self.irecv = None  # type: IRecv
-
-    def reconnect(self):
-        logging.debug('Waiting for device to reconnect in Recovery mode...')
-        self.irecv = IRecv(ecid=self.ecid)
+RESTORE_VARIANT_ERASE_INSTALL = 'Erase Install (IPSW)'
+RESTORE_VARIANT_UPGRADE_INSTALL = 'Upgrade Install (IPSW)'
+RESTORE_VARIANT_MACOS_RECOVERY_OS = 'macOS Customer'
+
+
+class Recovery(BaseRestore):
+    def __init__(self, ipsw: ZipFile, device: Device, tss: typing.Mapping = None, behavior: Behavior = Behavior.Update):
+        super().__init__(ipsw, device, tss, behavior, logger=logging.getLogger(__name__))
+        self.tss_localpolicy = None
+        self.tss_recoveryos_root_ticket = None
+        self.restore_boot_args = None
+
+    def reconnect_irecv(self, is_recovery=None):
+        self.logger.debug('waiting for device to reconnect...')
+        self.device.irecv = IRecv(ecid=self.device.ecid, is_recovery=is_recovery)
+        self.logger.debug(f'connected mode: {self.device.irecv.mode}')
 
     def get_preboard_manifest(self):
         overrides = {
             '@APTicket': True,
             'ApProductionMode': 0,
             'ApSecurityDomain': 0,
         }
 
         parameters = {
             'ApProductionMode': False,
             'ApSecurityMode': False,
             'ApSupportsImg4': True,
         }
 
-        keys_to_copy = ('UniqueBuildID', 'ApChipID', 'ApBoardID', 'ApSecurityDomain', 'Ap,OSLongVersion', 'BMU,BoardID',
-                        'BMU,ChipID', 'BbChipID', 'BbProvisioningManifestKeyHash', 'BbActivationManifestKeyHash',
-                        'BbCalibrationManifestKeyHash', 'BbFactoryActivationManifestKeyHash', 'BbFDRSecurityKeyHash',
-                        'BbSkeyId', 'SE,ChipID', 'Savage,ChipID', 'Savage,PatchEpoch', 'Yonkers,BoardID',
-                        'Yonkers,ChipID', 'Yonkers,PatchEpoch', 'Rap,BoardID', 'Rap,ChipID', 'Rap,SecurityDomain',
-                        'eUICC,ChipID', 'PearlCertificationRootPub', 'Manifest',)
-        for k in keys_to_copy:
-            try:
-                v = self.build_identity[k]
-                if isinstance(v, str) and v.startswith('0x'):
-                    v = int(v, 16)
-                parameters[k] = v
-            except KeyError:
-                pass
+        self.build_identity.populate_tss_request_parameters(parameters)
 
         tss = TSSRequest()
-        tss.add_common_flags(parameters, overrides)
+        tss.add_common_tags(parameters, overrides)
 
         parameters['_OnlyFWComponents'] = True
 
         tss.add_ap_tags(parameters)
 
-        return tss.img4_create_local_manifest()
-
-    def normal_handle_create_stashbag(self, manifest):
-        preboard = PreboardService(self._lockdown)
-        return preboard.create_stashbag(manifest)
-
-    def get_ap_nonce(self):
-        return self._lockdown.get_value(key='ApNonce')
-
-    def get_sep_nonce(self):
-        return self._lockdown.get_value(key='SEPNonce')
-
-    def tss_parameters_add_from_manifest(self, parameters):
-        keys_to_copy = (
-            'UniqueBuildID', 'Ap,OSLongVersion', 'ApChipID', 'ApBoardID', 'ApSecurityDomain',
-            'BMU,BoardID', 'BMU,ChipID', 'BbChipID', 'BbProvisioningManifestKeyHash', 'BbActivationManifestKeyHash',
-            'BbCalibrationManifestKeyHash', 'BbFactoryActivationManifestKeyHash', 'BbFDRSecurityKeyHash', 'BbSkeyId',
-            'SE,ChipID', 'Savage,ChipID', 'Savage,PatchEpoch', 'Yonkers,BoardID', 'Yonkers,ChipID',
-            'Yonkers,PatchEpoch', 'Rap,BoardID', 'Rap,ChipID', 'Rap,SecurityDomain', 'eUICC,ChipID',
-            'PearlCertificationRootPub', 'Manifest')
-
-        for k in keys_to_copy:
-            try:
-                v = self.build_identity[k]
-                if isinstance(v, str) and v.startswith('0x'):
-                    v = int(v, 16)
-                parameters[k] = v
-            except KeyError:
-                pass
-
-    def get_preflight_info(self):
-        return self._lockdown.get_value(key='FirmwarePreflightInfo')
+        return tss.img4_create_local_manifest(build_identity=self.build_identity)
 
     def get_tss_response(self):
         # populate parameters
         parameters = dict()
 
-        parameters['ApECID'] = self.ecid
-        if self.ap_nonce is not None:
-            parameters['ApNonce'] = self.ap_nonce
+        parameters['ApECID'] = self.device.ecid
+        if self.device.ap_nonce is not None:
+            parameters['ApNonce'] = self.device.ap_nonce
 
-        sep_nonce = self.get_sep_nonce()
-        if sep_nonce is not None:
-            parameters['ApSepNonce'] = sep_nonce
+        if self.device.sep_nonce is not None:
+            parameters['ApSepNonce'] = self.device.sep_nonce
 
         parameters['ApProductionMode'] = True
 
-        if self.is_image4_supported:
+        if self.device.is_image4_supported:
             parameters['ApSecurityMode'] = True
             parameters['ApSupportsImg4'] = True
         else:
             parameters['ApSupportsImg4'] = False
 
-        self.tss_parameters_add_from_manifest(parameters)
+        self.build_identity.populate_tss_request_parameters(parameters)
 
         tss = TSSRequest()
-        tss.add_common_flags(parameters)
+        tss.add_common_tags(parameters)
         tss.add_ap_tags(parameters)
 
         # add personalized parameters
-        if self.is_image4_supported:
+        if self.device.is_image4_supported:
             tss.add_ap_img4_tags(parameters)
         else:
             tss.add_ap_img3_tags(parameters)
 
-        # normal mode; request baseband ticket aswell
-        pinfo = self.get_preflight_info()
-        if pinfo:
-            logging.debug('adding preflight info')
-
-            node = pinfo.get('Nonce')
-            if node is not None:
-                parameters['BbNonce'] = node
-
-            node = pinfo.get('ChipID')
-            if node is not None:
-                parameters['BbChipID'] = node
-
-            node = pinfo.get('CertID')
-            if node is not None:
-                parameters['BbGoldCertId'] = node
-
-            node = pinfo.get('ChipSerialNo')
-            if node is not None:
-                parameters['BbSNUM'] = node
-
-            tss.add_baseband_tags(parameters)
-
-            euiccchipid = pinfo.get('EUICCChipID')
-            if euiccchipid:
-                logging.debug('adding EUICCChipID info')
-                parameters['eUICC,ChipID'] = euiccchipid
-
-                if euiccchipid >= 5:
-                    node = pinfo.get('EUICCCSN')
-                    if node is not None:
-                        parameters['eUICC,EID'] = node
-
-                    node = pinfo.get('EUICCCertIdentifier')
-                    if node is not None:
-                        parameters['eUICC,RootKeyIdentifier'] = node
-
-                    node = pinfo.get('EUICCGoldNonce')
-                    if node is not None:
-                        parameters['EUICCGoldNonce'] = node
-
-                    node = pinfo.get('EUICCMainNonce')
-                    if node is not None:
-                        parameters['EUICCMainNonce'] = node
+        # normal mode; request baseband ticket as well
+        if self.device.lockdown is not None:
+            pinfo = self.device.preflight_info
+            if pinfo:
+                self.logger.debug('adding preflight info')
+
+                node = pinfo.get('Nonce')
+                if node is not None:
+                    parameters['BbNonce'] = node
+
+                node = pinfo.get('ChipID')
+                if node is not None:
+                    parameters['BbChipID'] = node
+
+                node = pinfo.get('CertID')
+                if node is not None:
+                    parameters['BbGoldCertId'] = node
+
+                node = pinfo.get('ChipSerialNo')
+                if node is not None:
+                    parameters['BbSNUM'] = node
+
+                tss.add_baseband_tags(parameters)
+
+                euiccchipid = pinfo.get('EUICCChipID')
+                if euiccchipid:
+                    self.logger.debug('adding EUICCChipID info')
+                    parameters['eUICC,ChipID'] = euiccchipid
+
+                    if euiccchipid >= 5:
+                        node = pinfo.get('EUICCCSN')
+                        if node is not None:
+                            parameters['eUICC,EID'] = node
+
+                        node = pinfo.get('EUICCCertIdentifier')
+                        if node is not None:
+                            parameters['eUICC,RootKeyIdentifier'] = node
+
+                        node = pinfo.get('EUICCGoldNonce')
+                        if node is not None:
+                            parameters['EUICCGoldNonce'] = node
+
+                        node = pinfo.get('EUICCMainNonce')
+                        if node is not None:
+                            parameters['EUICCMainNonce'] = node
 
-                    tss.add_vinyl_tags(parameters)
+                        tss.add_vinyl_tags(parameters)
 
         # send request and grab response
-        return tss.request_send()
+        return tss.send_receive()
 
-    def fetch_tss_record(self):
-        stashbag_commit_required = False
-        if self._lockdown.all_values['HasSiDP']:
-            logging.info('Checking if device requires stashbag...')
-            manifest = self.get_preboard_manifest()
-
-            logging.debug('creating stashbag...')
-            response = self.normal_handle_create_stashbag(manifest)
-
-            if not response.get('Skip', False):
-                raise NotImplementedError('requiring stashbag not yet supported')
-
-        if self.build_major > 8:
-            self.ap_nonce = self.get_ap_nonce()
-            if self.ap_nonce is None:
-                # the first nonce request with older firmware releases can fail and it's OK
-                logging.info('NOTE: Unable to get nonce from device')
+    def get_local_policy_tss_response(self):
+        # populate parameters
+        parameters = {
+            'ApECID': self.device.ecid,
+            'Ap,LocalBoot': False,
+            'ApProductionMode': True,
+        }
 
-        self.tss = self.get_tss_response()
+        if self.device.ap_nonce:
+            parameters['ApNonce'] = self.device.ap_nonce
 
-        if self.build_major >= 20:
-            raise NotImplementedError('not yet supported')
+        sep_nonce = self.device.sep_nonce
 
-        if stashbag_commit_required:
-            raise NotImplementedError('requiring stashbag not yet supported')
+        if sep_nonce:
+            parameters['ApSepNonce'] = sep_nonce
 
-        return self.tss
+        if self.device.is_image4_supported:
+            parameters['ApSecurityMode'] = True
+            parameters['ApSupportsImg4'] = True
+        else:
+            parameters['ApSupportsImg4'] = False
+
+        self.build_identity.populate_tss_request_parameters(parameters)
 
-    def tss_response_get_path_by_entry(self, component):
-        node = self.tss.get(component)
-        if node is not None:
-            return node.get('Path')
-
-        return None
-
-    def build_identity_get_component_path(self, component):
-        return self.build_identity['Manifest'][component]['Info']['Path']
-
-    def tss_response_get_ap_img4_ticket(self):
-        return self.tss.get('ApImg4Ticket')
-
-    def img4_stitch_component(self, name, data, blob):
-        logging.info(f'Personalizing IMG4 component {name}...')
-
-        # first we need check if we have to change the tag for the given component
-        decoder = asn1.Decoder()
-        decoder.start(data)
-        decoder.enter()
-
-        decoder.read()
-        tag, value = decoder.read()
-
-        component_name_tag = {
-            'RestoreKernelCache': b'rkrn',
-            'RestoreDeviceTree': b'rdtr',
-            'RestoreSEP': b'rsep',
-            'RestoreLogo': b'rlgo',
-            'RestoreTrustCache': b'rtsc',
-            'RestoreDCP': b'rdcp',
-            'Ap,RestoreTMU': b'rtmu',
-            'Ap,RestoreCIO': b'rcio',
-            'Ap,DCP2': b'dcp2',
+        # Add Ap,LocalPolicy
+        lpol = {
+            'Digest': hashlib.sha384(lpol_file).digest(),
+            'Trusted': True,
         }
 
-        logging.debug(f'tag: {tag} {value}')
-        if name in component_name_tag:
-            logging.debug('Tag found')
-            data = data.replace(value.encode(), component_name_tag[name], 1)
+        parameters['Ap,LocalPolicy'] = lpol
 
-        # create element header for the "IMG4" magic
-        encoder = asn1.Encoder()
-        encoder.start()
+        # Add Ap,NextStageIM4MHash
+        # Get previous TSS ticket
+        ticket = self.tss.ap_img4_ticket
+        # Hash it and add it as Ap,NextStageIM4MHash
+        parameters['Ap,NextStageIM4MHash'] = hashlib.sha384(ticket).digest()
 
-        encoder.enter(asn1.Numbers.Sequence)
+        # create basic request
+        request = TSSRequest()
+
+        # add common tags from manifest
+        request.add_local_policy_tags(parameters)
+
+        return request.send_receive()
+
+    def get_recoveryos_root_ticket_tss_response(self):
+        # populate parameters
+        parameters = {
+            'ApECID': self.device.ecid,
+            'Ap,LocalBoot': False,
+            'ApProductionMode': True,
+        }
 
-        # create element header for the "IMG4" magic
-        encoder.write(b'IMG4', asn1.Numbers.IA5String)
+        if self.device.ap_nonce:
+            parameters['ApNonce'] = self.device.ap_nonce
 
-        decoder = asn1.Decoder()
-        decoder.start(data)
-        encoder.write(decoder.read()[1], nr=asn1.Numbers.Sequence, typ=asn1.Types.Constructed)
+        sep_nonce = self.device.sep_nonce
 
-        encoder.enter(0, cls=asn1.Classes.Context)
+        if sep_nonce:
+            parameters['ApSepNonce'] = sep_nonce
 
-        decoder = asn1.Decoder()
-        decoder.start(blob)
-        encoder.write(decoder.read()[1], nr=asn1.Numbers.Sequence, typ=asn1.Types.Constructed)
+        if self.device.is_image4_supported:
+            parameters['ApSecurityMode'] = True
+            parameters['ApSupportsImg4'] = True
+        else:
+            parameters['ApSupportsImg4'] = False
 
-        encoder.leave()
+        self.build_identity.populate_tss_request_parameters(parameters)
 
-        encoder.leave()
+        # create basic request
+        # Adds @HostPlatformInfo, @VersionInfo, @UUID
+        request = TSSRequest()
 
-        return encoder.output()
+        # add common tags from manifest
+        # Adds Ap,OSLongVersion, AppNonce, @ApImg4Ticket
+        request.add_ap_img4_tags(parameters)
 
-    def personalize_component(self, name, data):
-        blob = self.tss_response_get_ap_img4_ticket()
+        # add AP tags from manifest
+        request.add_common_tags(parameters)
 
-        # stitch ApImg4Ticket into IMG4 file
-        return self.img4_stitch_component(name, data, blob)
+        # add AP tags from manifest
+        # Fills digests & co
+        request.add_ap_recovery_tags(parameters)
 
-    def recovery_send_component(self, name):
-        logging.info(f'Sending {name}...')
-        path = None
-        if self.tss:
-            path = self.tss_response_get_path_by_entry(name)
+        return request.send_receive()
 
-        if path is None:
-            logging.debug(f'NOTE: No path for component {name} in TSS, will fetch from build_identity')
+    def fetch_tss_record(self):
+        if self.ipsw.build_manifest.build_major > 8:
+            if self.device.ap_nonce is None:
+                # the first nonce request with older firmware releases can fail, and it's OK
+                self.logger.info('NOTE: Unable to get nonce from device')
 
-        path = self.build_identity_get_component_path(name)
-        logging.debug(f'Sending a patched version of: {path}')
+        self.tss = self.get_tss_response()
 
-        data = self.ipsw.read(path)
-        signed_data = self.personalize_component(name, data)
+        if self.macos_variant:
+            self.tss_localpolicy = self.get_local_policy_tss_response()
+            self.tss_recoveryos_root_ticket = self.get_recoveryos_root_ticket_tss_response()
 
-        self.irecv.send_buffer(signed_data)
+        return self.tss
 
-    def recovery_send_component_and_command(self, name, command):
-        self.recovery_send_component(name)
-        self.irecv.send_command(command)
+    def send_component(self, name: str):
+        # Use a specific TSS ticket for the Ap,LocalPolicy component
+        data = None
+        tss = self.tss
+        if name == 'Ap,LocalPolicy':
+            tss = self.tss_localpolicy
+            # If Ap,LocalPolicy => Inject an empty policy
+            data = lpol_file
+
+        data = self.build_identity.get_component(name, tss=tss, data=data).personalized_data
+        self.logger.info(f'Sending {name} ({len(data)} bytes)...')
+        self.device.irecv.send_buffer(data)
+
+    def send_component_and_command(self, name, command):
+        self.send_component(name)
+        self.device.irecv.send_command(command)
 
-    def recovery_send_ibec(self):
+    def send_ibec(self):
         component = 'iBEC'
-        self.recovery_send_component(component)
-        self.irecv.send_command('go')
-        self.irecv.ctrl_transfer(0x21, 1)
+        self.send_component(component)
+        self.device.irecv.send_command('go', b_request=1)
+        self.device.irecv.ctrl_transfer(0x21, 1)
 
-    def recovery_send_applelogo(self):
+    def send_applelogo(self, allow_missing=True):
         component = 'RestoreLogo'
-        self.recovery_send_component(component)
-        self.irecv.send_command('setpicture 4')
-        self.irecv.send_command('bgcolor 0 0 0')
 
-    def recovery_send_loaded_by_iboot(self):
+        if not self.build_identity.has_component(component):
+            if allow_missing:
+                logging.warning(f'build_identity has no {component}')
+                return
+            else:
+                raise PyMobileDevice3Exception(f'missing component: {component}')
+
+        self.send_component(component)
+        self.device.irecv.send_command('setpicture 4')
+        self.device.irecv.send_command('bgcolor 0 0 0')
+
+    def send_loaded_by_iboot(self):
         manifest = self.build_identity['Manifest']
         for key, node in manifest.items():
             iboot = node['Info'].get('IsLoadedByiBoot', False)
             iboot_stg1 = node['Info'].get('IsLoadedByiBootStage1', False)
 
             assert isinstance(iboot, bool)
             assert isinstance(iboot_stg1, bool)
 
             if iboot and not iboot_stg1:
-                logging.debug(f'{key} is loaded by iBoot')
-                self.recovery_send_component_and_command(key, 'firmware')
+                self.logger.debug(f'{key} is loaded by iBoot')
+                self.send_component_and_command(key, 'firmware')
 
-    def recovery_send_ramdisk(self):
+    def send_iboot_stage1_components(self):
+        manifest = self.build_identity['Manifest']
+        for key, node in manifest.items():
+            iboot = node['Info'].get('IsLoadedByiBoot', False)
+            iboot_stg1 = node['Info'].get('IsLoadedByiBootStage1', False)
+
+            assert isinstance(iboot, bool)
+            assert isinstance(iboot_stg1, bool)
+
+            if iboot and iboot_stg1:
+                self.logger.debug(f'{key} is loaded by iBoot Stage 1')
+                self.send_component_and_command(key, 'firmware')
+
+    def send_ramdisk(self):
         component = 'RestoreRamDisk'
-        ramdisk_size = self.irecv.getenv('ramdisk-size')
-        logging.info(f'ramdisk-size: {ramdisk_size}')
+        ramdisk_size = self.device.irecv.getenv('ramdisk-size')
+        self.logger.info(f'ramdisk-size: {ramdisk_size}')
 
-        self.recovery_send_component(component)
-        ramdisk_delay = self.irecv.getenv('ramdisk-delay')
-        logging.info(f'ramdisk-delay: {ramdisk_delay}')
+        self.send_component(component)
+        ramdisk_delay = self.device.irecv.getenv('ramdisk-delay')
+        self.logger.info(f'ramdisk-delay: {ramdisk_delay}')
 
-        self.irecv.send_command('ramdisk')
+        self.device.irecv.send_command('ramdisk')
 
         time.sleep(2)
 
-    def recovery_send_kernelcache(self):
+    def send_kernelcache(self):
         component = 'RestoreKernelCache'
 
-        self.recovery_send_component(component)
+        self.send_component(component)
         try:
-            self.irecv.ctrl_transfer(0x21, 1)
+            self.device.irecv.ctrl_transfer(0x21, 1)
         except USBError:
             pass
 
         if self.restore_boot_args:
-            self.irecv.send_command(f'setenv boot-args {self.restore_boot_args}')
+            self.device.irecv.send_command(f'setenv boot-args {self.restore_boot_args}')
 
         try:
-            self.irecv.send_command('bootx')
+            self.device.irecv.send_command('bootx', b_request=1)
         except USBError:
             pass
 
-    def recovery_set_autoboot(self, enable: bool):
-        self.irecv.set_autoboot(enable)
+    def set_autoboot(self, enable: bool):
+        self.device.irecv.set_autoboot(enable)
 
-    def recovery_enter_restore(self):
-        if self.build_major >= 8:
+    def enter_restore(self):
+        if self.ipsw.build_manifest.build_major >= 8:
             self.restore_boot_args = 'rd=md0 nand-enable-reformat=1 -progress'
-        elif self.build_major >= 20:
+        elif self.macos_variant:
             self.restore_boot_args = 'rd=md0 nand-enable-reformat=1 -progress -restore'
 
         # upload data to make device boot restore mode
 
         # Recovery Mode Environment:
-        build_version = self.irecv.getenv('build-version')
-        logging.info(f'iBoot build-version={build_version}')
+        build_version = None
+        while not build_version:
+            self.logger.debug('build-version not yet supported. reconnecting...')
+            time.sleep(1)
+
+            # sometimes we manage to connect before iBEC actually started running
+            build_version = self.device.irecv.getenv('build-version')
+            self.reconnect_irecv()
 
-        build_style = self.irecv.getenv('build-style')
-        logging.info(f'iBoot build-style={build_style}')
+        self.logger.info(f'iBoot build-version={build_version}')
 
-        radio_error = self.irecv.getenv('radio-error')
+        build_style = self.device.irecv.getenv('build-style')
+        self.logger.info(f'iBoot build-style={build_style}')
+
+        radio_error = self.device.irecv.getenv('radio-error')
         if radio_error:
             radio_error = int(radio_error)
-            logging.info(f'radio-error: {radio_error}')
-            radio_error_string = self.irecv.getenv('radio-error-string')
+            self.logger.info(f'radio-error: {radio_error}')
+            radio_error_string = self.device.irecv.getenv('radio-error-string')
             if radio_error_string:
-                logging.info(f'radio-error-string: {radio_error_string}')
+                self.logger.info(f'radio-error-string: {radio_error_string}')
 
-        self.recovery_set_autoboot(False)
+        self.set_autoboot(False)
 
         # send logo and show it
-        self.recovery_send_applelogo()
+        self.send_applelogo()
 
         # send components loaded by iBoot
-        self.recovery_send_loaded_by_iboot()
+        self.send_loaded_by_iboot()
 
         # send ramdisk and run it
-        self.recovery_send_ramdisk()
+        self.send_ramdisk()
 
         # send devicetree and load it
-        self.recovery_send_component_and_command('RestoreDeviceTree', 'devicetree')
+        self.send_component_and_command('RestoreDeviceTree', 'devicetree')
 
-        if 'RestoreSEP' in self.build_identity['Manifest']:
+        if self.build_identity.has_component('RestoreSEP'):
             # send rsepfirmware and load it
-            self.recovery_send_component_and_command('RestoreSEP', 'rsepfirmware')
+            self.send_component_and_command('RestoreSEP', 'rsepfirmware')
+
+        self.send_kernelcache()
+
+    def dfu_enter_recovery(self):
+        self.send_component('iBSS')
+        self.reconnect_irecv(is_recovery=True)
+
+        if self.build_identity.build_manifest.build_major > 8:
+            old_nonce = self.device.irecv.ap_nonce
 
-        self.recovery_send_kernelcache()
+            # reconnect
+            self.reconnect_irecv()
+            nonce = self.device.irecv.ap_nonce
+
+            if old_nonce != nonce:
+                # Welcome iOS5. We have to re-request the TSS with our nonce.
+                self.tss = self.get_tss_response()
+
+            self.device.irecv.set_configuration(1)
+
+            # Now, before sending iBEC, we must send necessary firmwares on new versions.
+            if self.macos_variant:
+                # Without this empty policy file & its special signature, iBEC won't start.
+                self.send_component_and_command('Ap,LocalPolicy', 'lpolrestore')
+                self.send_iboot_stage1_components()
+                self.device.irecv.set_autoboot(False)
+                self.device.irecv.send_command('setenvnp boot-args rd=md0 nand-enable-reformat=1 -progress -restore')
+                self.send_applelogo(allow_missing=False)
+
+            # send iBEC
+            self.send_component('iBEC')
+
+            if self.device.irecv and self.device.irecv.mode.is_recovery:
+                time.sleep(1)
+                self.device.irecv.send_command('go', b_request=1)
+
+                if self.build_identity.build_manifest.build_major < 20:
+                    self.device.irecv.ctrl_transfer(0x21, 1, timeout=5000)
+
+        self.logger.debug('Waiting for device to disconnect...')
+        time.sleep(10)
+
+        self.logger.debug('Waiting for device to reconnect in recovery mode...')
+        self.reconnect_irecv(is_recovery=True)
 
     def boot_ramdisk(self):
         if self.tss is None:
-            logging.info('fetching TSS record')
+            self.logger.info('fetching TSS record')
             self.fetch_tss_record()
 
-        logging.info('going into Recovery')
-        self._lockdown.enter_recovery()
-        self.reconnect()
-        ecid = self.irecv.device_info['ECID']
-        logging.debug(f'ECID: {ecid}')
+        if self.device.irecv:
+            if self.device.irecv.mode == Mode.DFU_MODE:
+                # device is currently in DFU mode, place it into recovery mode
+                self.dfu_enter_recovery()
+            elif self.device.irecv.mode.is_recovery:
+                # now we load the iBEC
+                try:
+                    self.send_ibec()
+                except USBError:
+                    pass
+
+                self.reconnect_irecv()
+        elif self.device.lockdown:
+            # normal mode
+            self.logger.info('going into Recovery')
+
+            # in case lockdown has disconnected while waiting for a ticket
+            self.device.lockdown = LockdownClient(serial=self.device.lockdown.udid)
+            self.device.lockdown.enter_recovery()
+
+            self.device.lockdown = None
+            self.device.irecv = IRecv(self.device.ecid)
+            self.reconnect_irecv()
 
-        logging.info('device booted into recovery')
+            # now we load the iBEC
+            try:
+                self.send_ibec()
+            except USBError:
+                pass
 
-        # now we load the iBEC
-        try:
-            self.recovery_send_ibec()
-        except USBError:
-            pass
+            self.reconnect_irecv()
 
-        self.reconnect()
+        self.logger.info('device booted into recovery')
 
         # now finally do the magic to put the device into restore mode
-        self.recovery_enter_restore()
-
-    def restore_device(self):
-        # TODO: implement
-        raise NotImplementedError('restore_device not yet implemented')
-
-    def upgrade(self):
-        self.boot_ramdisk()
-
-        # device is finally in restore mode, let's do this
-        self.restore_device()
+        self.enter_restore()
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/service_connection.py` & `pymobiledevice3-2.0.0/pymobiledevice3/cli/cli_common.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,127 +1,128 @@
-from re import sub
-import plistlib
+import datetime
+import json
 import logging
-import struct
-import ssl
+import os
+import uuid
 
-import IPython
-from pygments import highlight, lexers, formatters
+import click
+import coloredlogs
+import hexdump
+import inquirer
+from inquirer.themes import GreenPassion
+from pygments import formatters, highlight, lexers
 
-from pymobiledevice3 import usbmux
-from pymobiledevice3.exceptions import ConnectionFailedError, PyMobileDevice3Exception
+from pymobiledevice3.exceptions import NoDeviceSelectedError
+from pymobiledevice3.lockdown import LockdownClient, create_using_usbmux
+from pymobiledevice3.usbmux import select_devices_by_connection_type
 
-SHELL_USAGE = """
-# This shell allows you to communicate directly with every service layer behind the lockdownd daemon.
 
-# For example, you can do the following:
-client.send_plist({"Command": "DoSomething"})
+def default_json_encoder(obj):
+    if isinstance(obj, bytes):
+        return f'<{obj.hex()}>'
+    if isinstance(obj, datetime.datetime):
+        return str(obj)
+    if isinstance(obj, uuid.UUID):
+        return str(obj)
+    raise TypeError()
 
-# and view the reply
-print(client.recv_plist())
 
-# or just send raw message
-client.send(b"hello")
+def print_json(buf, colored=True, default=default_json_encoder):
+    formatted_json = json.dumps(buf, sort_keys=True, indent=4, default=default)
+    if colored:
+        colorful_json = highlight(formatted_json, lexers.JsonLexer(),
+                                  formatters.TerminalTrueColorFormatter(style='stata-dark'))
+        print(colorful_json)
+    else:
+        print(formatted_json)
 
-# and view the result
-print(client.recvall(20))
-"""
 
+def print_hex(data, colored=True):
+    hex_dump = hexdump.hexdump(data, result='return')
+    if colored:
+        print(highlight(hex_dump, lexers.HexdumpLexer(), formatters.TerminalTrueColorFormatter(style='native')))
+    else:
+        print(hex_dump, end='\n\n')
 
-class ServiceConnection(object):
-    def __init__(self, socket):
-        self.logger = logging.getLogger(__name__)
-        self.socket = socket
+
+def set_verbosity(ctx, param, value):
+    coloredlogs.set_level(logging.INFO - (value * 10))
+
+
+def wait_return():
+    input('> Hit RETURN to exit')
+
+
+UDID_ENV_VAR = 'PYMOBILEDEVICE3_UDID'
+
+
+class DeviceInfo:
+    def __init__(self, lockdown_client: LockdownClient):
+        self.lockdown_client = lockdown_client
+        self.product_version = self.lockdown_client.product_version
+        self.serial = self.lockdown_client.identifier
+        self.display_name = self.lockdown_client.display_name
+
+    def __str__(self):
+        if self.display_name is None:
+            return f'Unknown device, ios version: {self.product_version}, serial: {self.serial}'
+        else:
+            return f'{self.display_name}, ios version: {self.product_version}, serial: {self.serial}'
+
+
+class Command(click.Command):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.params[:0] = [
+            click.Option(('lockdown', '--udid'), envvar=UDID_ENV_VAR, callback=self.udid,
+                         help=f'Device unique identifier. You may pass {UDID_ENV_VAR} environment variable to pass this'
+                              f' option as well'),
+            click.Option(('verbosity', '-v', '--verbose'), count=True, callback=set_verbosity, expose_value=False),
+        ]
 
     @staticmethod
-    def create(udid, port):
-        mux = usbmux.USBMux()
-        mux.process()
-        target_device = None
-
-        while target_device is None:
-            mux.process()
-            for connected_device in mux.devices:
-                if connected_device.serial == udid:
-                    target_device = connected_device
-                    break
+    def udid(ctx, param, value):
+        if '_PYMOBILEDEVICE3_COMPLETE' in os.environ:
+            # prevent lockdown connection establishment when in autocomplete mode
+            return
 
+        if value is not None:
+            return create_using_usbmux(serial=value)
+
+        devices = select_devices_by_connection_type(connection_type='USB')
+        if len(devices) <= 1:
+            return create_using_usbmux()
+
+        devices_options = []
+        for device in devices:
+            lockdown_client = create_using_usbmux(serial=device.serial)
+            device_info = DeviceInfo(lockdown_client)
+            devices_options.append(device_info)
+
+        device_question = [inquirer.List('device', message='choose device', choices=devices_options, carousel=True)]
         try:
-            socket = mux.connect(target_device, port)
-        except usbmux.MuxException:
-            raise ConnectionFailedError(f'Connection to device port {port} failed')
-
-        return ServiceConnection(socket)
-
-    def setblocking(self, blocking: bool):
-        self.socket.setblocking(blocking)
-
-    def close(self):
-        self.socket.close()
-
-    def recv(self, length=4096):
-        """ socket.recv() normal behavior. attempt to receive a single chunk """
-        return self.socket.recv(length)
-
-    def sendall(self, data):
-        self.socket.sendall(data)
-
-    def send_recv_plist(self, data):
-        self.send_plist(data)
-        return self.recv_plist()
-
-    def recvall(self, size):
-        data = b''
-        while len(data) < size:
-            chunk = self.recv(size - len(data))
-            if chunk is None or len(chunk) == 0:
-                raise ConnectionAbortedError()
-            data += chunk
-        return data
-
-    def recv_prefixed(self, endianity='>'):
-        """ receive a data block prefixed with a u32 length field """
-        size = self.recvall(4)
-        if not size or len(size) != 4:
-            return
-        size = struct.unpack(endianity + 'L', size)[0]
-        return self.recvall(size)
+            result = inquirer.prompt(device_question, theme=GreenPassion(), raise_keyboard_interrupt=True)
+            return result['device'].lockdown_client
+        except KeyboardInterrupt as e:
+            raise NoDeviceSelectedError from e
 
-    def send_prefixed(self, data):
-        """ send a data block prefixed with a u32 length field """
-        if isinstance(data, str):
-            data = data.encode()
-        hdr = struct.pack('>L', len(data))
-        msg = b''.join([hdr, data])
-        return self.sendall(msg)
-
-    def recv_plist(self):
-        payload = self.recv_prefixed()
-        if not payload:
+
+class CommandWithoutAutopair(Command):
+    @staticmethod
+    def udid(ctx, param, value):
+        if '_PYMOBILEDEVICE3_COMPLETE' in os.environ:
+            # prevent lockdown connection establishment when in autocomplete mode
             return
-        bplist_header = b'bplist00'
-        xml_header = b'<?xml'
-        if payload.startswith(bplist_header):
-            return plistlib.loads(payload)
-        elif payload.startswith(xml_header):
-            # HAX lockdown HardwarePlatform with null bytes
-            payload = sub(r'[^\w<>\/ \-_0-9\"\'\\=\.\?\!\+]+', '', payload.decode('utf-8')).encode('utf-8')
-            return plistlib.loads(payload)
-        else:
-            raise PyMobileDevice3Exception(f'recv_plist invalid data: {payload[:100].hex()}')
+        return create_using_usbmux(serial=value, autopair=False)
+
+
+class BasedIntParamType(click.ParamType):
+    name = 'based int'
+
+    def convert(self, value, param, ctx):
+        try:
+            return int(value, 0)
+        except ValueError:
+            self.fail(f'{value!r} is not a valid int.', param, ctx)
+
 
-    def send_plist(self, d):
-        payload = plistlib.dumps(d)
-        message = struct.pack(">L", len(payload))
-        return self.sendall(message + payload)
-
-    def ssl_start(self, keyfile, certfile):
-        context = ssl.SSLContext(ssl.PROTOCOL_TLSv1)
-        context.load_cert_chain(certfile, keyfile)
-        self.socket = context.wrap_socket(self.socket)
-
-    def shell(self):
-        IPython.embed(
-            header=highlight(SHELL_USAGE, lexers.PythonLexer(), formatters.TerminalTrueColorFormatter(style='native')),
-            user_ns={
-                'client': self,
-            })
+BASED_INT = BasedIntParamType()
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/services/accessibilityaudit.py` & `pymobiledevice3-2.0.0/pymobiledevice3/services/accessibilityaudit.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,49 @@
+import typing
+from dataclasses import dataclass
+from enum import Enum
+
+from packaging.version import Version
+
 from pymobiledevice3.lockdown import LockdownClient
-from pymobiledevice3.services.remote_server import RemoteServer, MessageAux
+from pymobiledevice3.services.remote_server import MessageAux, RemoteServer
 
 
 class SerializedObject:
-    def __init__(self, fields: dict):
+    def __init__(self, fields: typing.Mapping):
         self._fields = fields
 
 
 class AXAuditInspectorFocus_v1(SerializedObject):
     def __init__(self, fields):
         super().__init__(fields)
 
+    @property
+    def caption(self) -> str:
+        return self._fields.get('CaptionTextValue_v1')
+
+    @property
+    def element(self) -> bytes:
+        return self._fields.get('ElementValue_v1')
+
     def __str__(self):
-        return f'<Focused Element: {self._fields.get("CaptionTextValue_v1")}>'
+        return f'<Focused ElementCaption: {self.caption}>'
 
 
 class AXAuditElement_v1(SerializedObject):
     def __init__(self, fields):
         super().__init__(fields)
 
+    @property
+    def identifier(self) -> bytes:
+        return self._fields['PlatformElementValue_v1'].NSdata
+
+    def __repr__(self):
+        return f'<Element: {self.identifier}>'
+
 
 class AXAuditInspectorSection_v1(SerializedObject):
     def __init__(self, fields):
         super().__init__(fields)
 
 
 class AXAuditElementAttribute_v1(SerializedObject):
@@ -35,31 +56,46 @@
 
     def __init__(self, fields):
         super().__init__(fields)
         for k in self.FIELDS:
             if k not in self._fields:
                 self._fields[k] = None
 
-    def __str__(self):
-        return f'<AXAuditDeviceSetting_v1 {self._fields["IdentiifierValue_v1"]} = ' \
-               f'{self._fields["CurrentValueNumber_v1"]}>'
+    @property
+    def key(self) -> str:
+        return self._fields['IdentiifierValue_v1']
+
+    @property
+    def value(self) -> typing.Any:
+        return self._fields['CurrentValueNumber_v1']
+
+    def __str__(self) -> str:
+        return f'<AXAuditDeviceSetting_v1 {self.key} = {self.value}>'
 
 
 SERIALIZABLE_OBJECTS = {
     'AXAuditDeviceSetting_v1': AXAuditDeviceSetting_v1,
     'AXAuditInspectorFocus_v1': AXAuditInspectorFocus_v1,
     'AXAuditElement_v1': AXAuditElement_v1,
     'AXAuditInspectorSection_v1': AXAuditInspectorSection_v1,
     'AXAuditElementAttribute_v1': AXAuditElementAttribute_v1,
 }
 
-DIRECTION_PREV = 3
-DIRECTION_NEXT = 4
-DIRECTION_FIRST = 5
-DIRECTION_LAST = 6
+
+@dataclass
+class Event:
+    name: str
+    data: SerializedObject
+
+
+class Direction(Enum):
+    Previous = 3
+    Next = 4
+    First = 5
+    Last = 6
 
 
 def deserialize_object(d):
     if not isinstance(d, dict):
         if isinstance(d, list):
             return [deserialize_object(x) for x in d]
         return d
@@ -79,95 +115,145 @@
 
 class AccessibilityAudit(RemoteServer):
     SERVICE_NAME = 'com.apple.accessibility.axAuditDaemon.remoteserver'
 
     def __init__(self, lockdown: LockdownClient):
         super().__init__(lockdown, self.SERVICE_NAME, remove_ssl_context=True)
 
-        self._callback = None
-
-        self.broadcast.deviceSetAppMonitoringEnabled_(MessageAux().append_obj(True))
-        self.recv_response()
+        # flush previously received messages
+        self.recv_plist()
+        if Version(lockdown.product_version) >= Version('15.0'):
+            self.recv_plist()
 
-        self.broadcast.deviceInspectorSetMonitoredEventType_(MessageAux().append_obj(0))
-        self.recv_response()
+    @property
+    def capabilities(self) -> typing.List[str]:
+        self.broadcast.deviceCapabilities()
+        return self.recv_plist()[0]
 
-        self.broadcast.deviceInspectorShowVisuals_(MessageAux().append_obj(1))
-        self.recv_response()
+    @property
+    def settings(self) -> typing.List[AXAuditDeviceSetting_v1]:
+        self.broadcast.deviceAccessibilitySettings()
+        return deserialize_object(self.recv_plist()[0])
 
-        self.broadcast.deviceInspectorShowIgnoredElements_(MessageAux().append_obj(1))
-        self.recv_response()
+    def perform_handshake(self) -> None:
+        # this service acts differently from others, requiring no handshake
+        pass
 
-    def register_notifications_callback(self, callback):
-        self._callback = callback
+    def set_app_monitoring_enabled(self, value: bool) -> None:
+        self.broadcast.deviceSetAppMonitoringEnabled_(MessageAux().append_obj(value), expects_reply=False)
 
-    def listen_for_notifications(self):
-        if self._callback is not None:
-            while True:
-                notification = self.recv_plist()
-                if notification[1] is None:
-                    continue
-                data = [x['value'] for x in notification[1]]
-                self._callback(notification[0], deserialize_object(data))
+    def set_monitored_event_type(self, event_type: int = None) -> None:
+        if event_type is None:
+            event_type = 0
+        self.broadcast.deviceInspectorSetMonitoredEventType_(MessageAux().append_obj(event_type), expects_reply=False)
 
-    def recv_response(self):
-        plist = self.recv_plist()
+    def set_show_ignored_elements(self, value: bool) -> None:
+        self.broadcast.deviceInspectorShowIgnoredElements_(MessageAux().append_obj(int(value)), expects_reply=False)
 
-        while plist[1] is not None:
-            # skip notifications, but report them if exists
-            if self._callback is not None:
-                self._callback(plist[0], deserialize_object(plist[1]))
+    def set_show_visuals(self, value: bool) -> None:
+        self.broadcast.deviceInspectorShowVisuals_(MessageAux().append_obj(int(value)), expects_reply=False)
 
-            plist = self.recv_plist()
+    def iter_events(self, app_monitoring_enabled=True, monitored_event_type: int = None) -> \
+            typing.Generator[Event, None, None]:
 
-        return plist
+        self.set_app_monitoring_enabled(app_monitoring_enabled)
+        self.set_monitored_event_type(monitored_event_type)
 
-    def kaki(self):
         while True:
-            print(self.recv_plist())
-
-    def device_capabilities(self):
-        self.broadcast.deviceCapabilities()
-        return self.recv_response()[0]
+            message = self.recv_plist()
+            if message[1] is None:
+                continue
+            data = [x['value'] for x in message[1]]
+            yield Event(name=message[0], data=deserialize_object(data))
+
+    def move_focus_next(self) -> None:
+        self.move_focus(Direction.Next)
+
+    def perform_press(self, element: bytes) -> None:
+        """ simulate click (can be used only for processes with task_for_pid-allow """
+        element = {
+            'ObjectType': 'AXAuditElement_v1',
+            'Value': {
+                'ObjectType': 'passthrough',
+                'Value': {
+                    'PlatformElementValue_v1': {
+                        'ObjectType': 'passthrough'
+                    },
+                    'Value': element,
+                }
+            }
+        }
 
-    def get_current_settings(self):
-        self.broadcast.deviceAccessibilitySettings()
-        return deserialize_object(self.recv_response()[0])
+        action = {
+            'ObjectType': 'AXAuditElementAttribute_v1',
+            'Value': {
+                'ObjectType': 'passthrough',
+                'Value': {
+                    'AttributeNameValue_v1': {
+                        'ObjectType': 'passthrough',
+                        'Value': 'AXAction-2010',
+                    },
+                    'DisplayAsTree_v1': {
+                        'ObjectType': 'passthrough',
+                        'Value': 0,
+                    },
+                    'HumanReadableNameValue_v1': {
+                        'ObjectType': 'passthrough',
+                        'Value': 'Activate',
+                    },
+                    'IsInternal_v1': {
+                        'ObjectType': 'passthrough',
+                        'Value': 0,
+                    },
+                    'PerformsActionValue_v1': {
+                        'ObjectType': 'passthrough',
+                        'Value': 1,
+                    },
+                    'SettableValue_v1': {
+                        'ObjectType': 'passthrough',
+                        'Value': 0,
+                    },
+                    'ValueTypeValue_v1': {
+                        'ObjectType': 'passthrough',
+                        'Value': 1,
+                    },
+                }
+            }
+        }
 
-    def move_focus_next(self):
-        self.move_focus(DIRECTION_NEXT)
+        self.broadcast.deviceElement_performAction_withValue_(
+            MessageAux().append_obj(element).append_obj(action).append_obj(0), expects_reply=False)
 
-    def move_focus(self, direction):
+    def move_focus(self, direction: Direction) -> None:
         options = {
             'ObjectType': 'passthrough',
             'Value': {
                 'allowNonAX': {
                     'ObjectType': 'passthrough',
                     'Value': 0,
                 },
                 'direction': {
                     'ObjectType': 'passthrough',
-                    'Value': direction,
+                    'Value': direction.value,
                 },
                 'includeContainers': {
                     'ObjectType': 'passthrough',
                     'Value': 1,
                 }
             }
         }
 
-        self.broadcast.deviceInspectorMoveWithOptions_(MessageAux().append_obj(options))
-        self.recv_response()
+        self.broadcast.deviceInspectorMoveWithOptions_(MessageAux().append_obj(options), expects_reply=False)
 
-    def set_setting(self, name, value):
+    def set_setting(self, name: str, value: typing.Any) -> None:
         setting = {'ObjectType': 'AXAuditDeviceSetting_v1',
                    'Value': {'ObjectType': 'passthrough',
                              'Value': {'CurrentValueNumber_v1': {'ObjectType': 'passthrough',
                                                                  'Value': True},
                                        'EnabledValue_v1': {'ObjectType': 'passthrough', 'Value': True},
                                        'IdentiifierValue_v1': {'ObjectType': 'passthrough',
                                                                'Value': name},
                                        'SettingTypeValue_v1': {'ObjectType': 'passthrough', 'Value': 3},
                                        'SliderTickMarksValue_v1': {'ObjectType': 'passthrough', 'Value': 0}}}}
         self.broadcast.deviceUpdateAccessibilitySetting_withValue_(
-            MessageAux().append_obj(setting).append_obj({'ObjectType': 'passthrough', 'Value': value}))
-        self.recv_response()
+            MessageAux().append_obj(setting).append_obj({'ObjectType': 'passthrough', 'Value': value}),
+            expects_reply=False)
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/services/device_link.py` & `pymobiledevice3-2.0.0/pymobiledevice3/services/device_link.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-import datetime
 import ctypes
+import datetime
 import shutil
-import os
 import struct
 from pathlib import Path
 
 from pymobiledevice3.exceptions import PyMobileDevice3Exception
 
 SIZE_FORMAT = '>I'
 CODE_FORMAT = '>B'
@@ -108,37 +107,33 @@
                 'DLFileType': ftype,
                 'DLFileSize': file.stat().st_size,
                 'DLFileModificationDate': datetime.datetime.utcfromtimestamp(file.stat().st_mtime - APPLE_EPOCH)
             }
         self.status_response(0, status_dict=data)
 
     def upload_files(self, message):
-        real_size = 0
         while True:
             device_name = self._prefixed_recv()
             if not device_name:
                 break
             file_name = self._prefixed_recv()
             size, = struct.unpack(SIZE_FORMAT, self.service.recvall(struct.calcsize(SIZE_FORMAT)))
             code, = struct.unpack(CODE_FORMAT, self.service.recvall(struct.calcsize(CODE_FORMAT)))
             size -= struct.calcsize(CODE_FORMAT)
-            data = b''
-            while size and code == CODE_FILE_DATA:
-                real_size += size
-                data += self.service.recvall(size)
-                size, = struct.unpack(SIZE_FORMAT, self.service.recvall(struct.calcsize(SIZE_FORMAT)))
-                code, = struct.unpack(CODE_FORMAT, self.service.recvall(struct.calcsize(CODE_FORMAT)))
-                size -= struct.calcsize(CODE_FORMAT)
+            with open(self.root_path / file_name, 'wb') as fd:
+                while size and code == CODE_FILE_DATA:
+                    fd.write(self.service.recvall(size))
+                    size, = struct.unpack(SIZE_FORMAT, self.service.recvall(struct.calcsize(SIZE_FORMAT)))
+                    code, = struct.unpack(CODE_FORMAT, self.service.recvall(struct.calcsize(CODE_FORMAT)))
+                    size -= struct.calcsize(CODE_FORMAT)
             assert code == CODE_SUCCESS
-            (self.root_path / file_name).write_bytes(data)
         self.status_response(0)
 
     def get_free_disk_space(self, message):
-        vfs = os.statvfs(self.root_path)
-        freespace = vfs.f_bavail * vfs.f_bsize
+        freespace = shutil.disk_usage(self.root_path).free
         self.status_response(0, status_dict=freespace)
 
     def move_items(self, message):
         for src, dst in message[1].items():
             dest = self.root_path / dst
             dest.parent.mkdir(parents=True, exist_ok=True)
             shutil.move(self.root_path / src, dest)
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/services/diagnostics.py` & `pymobiledevice3-2.0.0/pymobiledevice3/services/diagnostics.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,12 @@
-from pymobiledevice3.exceptions import PyMobileDevice3Exception
-from pymobiledevice3.lockdown import LockdownClient
+from typing import List, Mapping, Optional
 
-Requests = """Goodbye
-All
-GasGauge
-WiFi
-Shutdown
-Restart
-MobileGestalt
-Sleep
-NAND
-IORegistry
-Obliterate
-"""
+from pymobiledevice3.exceptions import ConnectionFailedError, PyMobileDevice3Exception
+from pymobiledevice3.lockdown import LockdownClient
+from pymobiledevice3.services.base_service import BaseService
 
 MobileGestaltKeys = ['BasebandKeyHashInformation',
                      'BasebandFirmwareManifestData',
                      'DieId',
                      'SerialNumber',
                      'UniqueChipID',
                      'WifiAddress',
@@ -93,57 +83,64 @@
                      'RegionalBehaviorNoWiFi',
                      'RegionalBehaviorChinaBrick',
                      'RegionalBehaviorNoVOIP',
                      'RegionalBehaviorAll',
                      'ApNonce']
 
 
-class DiagnosticsService(object):
-    SERVICE_NAME = 'com.apple.mobile.diagnostics_relay'
+class DiagnosticsService(BaseService):
+    """
+    Provides an API to:
+    * Query MobileGestalt & IORegistry keys.
+    * Reboot, shutdown or put the device in sleep mode.
+    """
+    SERVICE_NAME_NEW = 'com.apple.mobile.diagnostics_relay'
+    SERVICE_NAME_OLD = 'com.apple.iosdiagnostics.relay'
 
     def __init__(self, lockdown: LockdownClient):
-        self.lockdown = lockdown
-        self.service = self.lockdown.start_service(self.SERVICE_NAME)
-        self.packet_num = 0
+        try:
+            service = lockdown.start_service(self.SERVICE_NAME_NEW)
+            service_name = self.SERVICE_NAME_NEW
+        except ConnectionFailedError:
+            service = lockdown.start_service(self.SERVICE_NAME_OLD)
+            service_name = self.SERVICE_NAME_OLD
 
-    def mobilegestalt(self, keys=None):
+        super().__init__(lockdown, service_name, service=service)
+
+    def mobilegestalt(self, keys: List[str] = None) -> Mapping:
         if keys is None or len(keys) == 0:
             keys = MobileGestaltKeys
-        self.service.send_plist({'Request': 'MobileGestalt',
-                                 'MobileGestaltKeys': keys})
+        resp = self.service.send_recv_plist({'Request': 'MobileGestalt', 'MobileGestaltKeys': keys})
 
-        res = self.service.recv_plist()
-        d = res.get('Diagnostics')
-        if d:
-            return d.get('MobileGestalt')
-        return None
+        if (resp['Status'] != 'Success') or (resp['Diagnostics']['MobileGestalt']['Status'] != 'Success'):
+            raise PyMobileDevice3Exception('failed to query MobileGestalt')
 
-    def action(self, action):
-        self.service.send_plist({'Request': action})
-        response = self.service.recv_plist()
-        if response.get('Status', None) is None:
-            raise PyMobileDevice3Exception(f'got invalid response: {response}')
+        resp['Diagnostics']['MobileGestalt'].pop('Status')
+
+        return resp['Diagnostics']['MobileGestalt']
+
+    def action(self, action: str) -> Optional[Mapping]:
+        response = self.service.send_recv_plist({'Request': action})
+        if response['Status'] != 'Success':
+            raise PyMobileDevice3Exception(f'failed to perform action: {action}')
+        return response.get('Diagnostics')
 
     def restart(self):
         self.action('Restart')
 
     def shutdown(self):
         self.action('Shutdown')
 
     def sleep(self):
         self.action('Sleep')
 
-    def info(self, diag_type='All'):
-        self.service.send_plist({'Request': diag_type})
-        res = self.service.recv_plist()
-        if res:
-            return res.get('Diagnostics')
-        return None
+    def info(self, diag_type: str = 'All') -> Mapping:
+        return self.action(diag_type)
 
-    def ioregistry(self, plane=None, name=None, ioclass=None):
+    def ioregistry(self, plane: str = None, name: str = None, ioclass: str = None):
         d = {}
 
         if plane:
             d['CurrentPlane'] = plane
 
         if name:
             d['EntryName'] = name
@@ -158,9 +155,9 @@
             raise PyMobileDevice3Exception(f'got invalid response: {response}')
 
         dd = response.get('Diagnostics')
         if dd:
             return dd.get('IORegistry')
         return None
 
-    def get_battery(self):
+    def get_battery(self) -> Mapping:
         return self.ioregistry(ioclass='IOPMPowerSource')
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/services/dtfetchsymbols.py` & `pymobiledevice3-2.0.0/pymobiledevice3/services/dtfetchsymbols.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import struct
-from io import BytesIO
+import typing
 
 from pymobiledevice3.exceptions import PyMobileDevice3Exception
 from pymobiledevice3.lockdown import LockdownClient
 
 
 class DtFetchSymbols(object):
     SERVICE_NAME = 'com.apple.dt.fetchsymbols'
@@ -12,24 +12,24 @@
     CMD_LIST_FILES_PLIST = struct.pack('>I', 0x30303030)
     CMD_GET_FILE = struct.pack('>I', 1)
 
     def __init__(self, lockdown: LockdownClient):
         self.logger = logging.getLogger(__name__)
         self.lockdown = lockdown
 
-    def list_files(self) -> bytes:
+    def list_files(self) -> typing.List[str]:
         service = self._start_command(self.CMD_LIST_FILES_PLIST)
         return service.recv_plist().get('files')
 
-    def get_file(self, fileno: int, stream: BytesIO):
+    def get_file(self, fileno: int, stream: typing.IO):
         service = self._start_command(self.CMD_GET_FILE)
         service.sendall(struct.pack('>I', fileno))
 
         size = struct.unpack('>Q', service.recvall(8))[0]
-        logging.debug(f'file size: {size}')
+        self.logger.debug(f'file size: {size}')
 
         received = 0
         while received < size:
             buf = service.recv(min(size - received, self.MAX_CHUNK))
             stream.write(buf)
             received += len(buf)
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/dvt_secure_socket_proxy.py` & `pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/dvt_secure_socket_proxy.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from distutils.version import LooseVersion
+from packaging.version import Version
 
 from pymobiledevice3.lockdown import LockdownClient
 from pymobiledevice3.services.remote_server import RemoteServer
 
 
 class DvtSecureSocketProxyService(RemoteServer):
     SERVICE_NAME = 'com.apple.instruments.remoteserver.DVTSecureSocketProxy'
     OLD_SERVICE_NAME = 'com.apple.instruments.remoteserver'
 
     def __init__(self, lockdown: LockdownClient):
-        if LooseVersion(lockdown.ios_version) >= LooseVersion('14.0'):
+        if Version(lockdown.product_version) >= Version('14.0'):
             service_name = self.SERVICE_NAME
             remove_ssl_context = False
         else:
             service_name = self.OLD_SERVICE_NAME
             remove_ssl_context = True
 
         super().__init__(lockdown, service_name, remove_ssl_context=remove_ssl_context)
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/activity_trace_tap.py` & `pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/activity_trace_tap.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,64 +34,69 @@
         return s
 
     if s[-1] == 0:
         s = s[:-1]
     return s
 
 
-def decode_message_format(message):
-    s = b''
+def decode_message_format(message) -> str:
+    s = ''
     for type_, data in message:
-        data = ignored_null(data)
+        if data:
+            data = ignored_null(data)
         type_ = decode_str(type_)
 
         if type_ == 'address':
             type_ = 'uint64-hex'
 
-        if type_ == 'narrative-text':
-            s += ignored_null(data)
-        elif type_ == 'string':
-            s += ignored_null(data)
+        if type_ in ('narrative-text', 'string'):
+            if data is None:
+                s += '<None>'
+            else:
+                s += data.decode()
         elif type_.startswith('uint64'):
             uint64 = struct.unpack('<Q', data.ljust(8, b'\x00'))[0]
             if 'hex' in type_:
                 uint64 = hex(uint64)[2:]
                 if 'lowercase' in type_:
                     uint64 = uint64.lower()
-            s += str(uint64).encode()
+            s += str(uint64)
         elif 'decimal' in type_:
             uint64 = struct.unpack('<Q', data.ljust(8, b'\x00'))[0]
-            s += str(uint64).encode()
-        elif type_ == 'data':
-            s += b''.join(data).hex().encode()
+            s += str(uint64)
+        elif type_ in ('data', 'uuid'):
+            if data is not None:
+                s += b''.join(data).hex()
         else:
-            s += data
+            # by default, make sure the data can be concatenated
+            s += str(data)
     return s
 
 
 class ActivityTraceTap(Tap):
     IDENTIFIER = 'com.apple.instruments.server.services.activitytracetap'
 
-    def __init__(self, dvt):
+    def __init__(self, dvt, enable_http_archive_logging=False):
         # TODO:
         #   reverse: [DTOSLogLoader _handleRecord:], DTTableRowEncoder::*
         #   to understand each row's structure.
 
         config = {
             'bm': 0,  # buffer mode
             'combineDataScope': 0,
             'machTimebaseDenom': 3,
             'machTimebaseNumer': 125,
             'onlySignposts': 0,
-            'pidToInjectCombineDYLIB': "-1",
-            'predicate': "(messageType == info OR messageType == debug OR messageType == default OR "
-                         "messageType == error OR messageType == fault)",
-            # 'signpostsAndLogs': 1,
-            'signpostsAndLogs': 0,
-            'targetPID': "-3",
+            'pidToInjectCombineDYLIB': '-1',
+            'predicate': '(messageType == info OR messageType == debug OR messageType == default OR '
+                         'messageType == error OR messageType == fault)',
+            'signpostsAndLogs': 1,
+            'trackPidToExecNameMapping': True,
+            'enableHTTPArchiveLogging': enable_http_archive_logging,
+            'targetPID': -3,  # all Process
             'trackExpiredPIDs': 1,
             'ur': 500,
         }
 
         super().__init__(dvt, self.IDENTIFIER, config)
 
         self.stack = []
@@ -99,15 +104,15 @@
         self.background = 0
         self.tables = []
 
     def _get_next_message(self):
         message = b''
         while message.startswith(b'bplist') or len(message) == 0:
             # ignore heartbeat messages
-            message = self._channel.receive_message()
+            message = self.channel.receive_message()
         self._set_current_message(message)
 
     def _set_current_message(self, message):
         self._message = BytesIO(message)
 
     def _seek_relative(self, offset):
         self._message.seek(offset, os.SEEK_CUR)
@@ -133,20 +138,22 @@
         bit_count = 0
         while word >> 14 != 0b11:
             # not end word
             imm = (imm << 14) | (word & 0x3fff)
             word = self._read_word()
             count += 1
             bit_count += 14
+
         imm = (imm << 14) | (word & 0x3fff)
         bit_count += 14
 
         imm <<= (8 - bit_count % 8)
+        bit_count += 8 - bit_count % 8
 
-        result = imm.to_bytes(math.ceil(len(bin(imm)[2:]) / 8), 'big')
+        result = imm.to_bytes(math.ceil(bit_count / 8), 'big')
         self.stack.append(result)
 
         return result
 
     def _handle_table_reset(self, word):
         """ start new table vector """
         self.generation += 1
@@ -179,22 +186,21 @@
                       unknown0=table_raw.unknown0, unknown2=table_raw.unknown2)
 
         self.stack = self.stack[:-distance]
         self.tables.append(table)
 
     def _handle_debug(self, word):
         """ pop last pushed item from stack """
-        # TODO: fix asserts
-        # debug_id = word & 0xff
-        # item = self.stack[-1]
-        #
-        # reference = int.from_bytes(item, byteorder='little')
-        #
-        # assert reference == len(self.stack) - 1, f'assert debug {debug_id} got reference: {hex(reference)} instead of:' \
-        #                                          f'{len(self.stack) - 1}  {item}'
+        debug_id = word & 0xff
+        item = self.stack[-1]
+
+        reference = int.from_bytes(item, byteorder='little')
+
+        assert reference == len(self.stack) - 1, \
+            f'assert debug {debug_id} got reference: {hex(reference)} instead of: {len(self.stack) - 1}  {item}'
         self.stack = self.stack[:-1]
 
     def _handle_copy(self, word):
         """ copy item at distance from stack """
         distance = word & 0xff
         if distance != 0xff:
             item = self.stack[-distance - 1]
@@ -209,39 +215,37 @@
     def _handle_end_row(self, word):
         """ flush current row """
         generation = word & 0xff
         columns = self.tables[generation].columns
         row = self.stack[-len(columns):]
         self.stack = self.stack[:-len(columns)]
 
-        try:
-            Message = dataclasses.make_dataclass('message', [c.replace('-', '_') for c in columns])
-            message = Message(*row)
-            message.process = struct.unpack('<I', message.process[0].ljust(4, b'\x00'))[0]
-            message.thread = struct.unpack('<I', message.thread[0].ljust(4, b'\x00'))[0]
-
-            string_fields = ('message_type', 'format_string', 'subsystem', 'category', 'sender_image_path')
-            for f in string_fields:
-                if hasattr(message, f):
-                    setattr(message, f, decode_str(getattr(message, f)))
-
-            if hasattr(message, 'message'):
-                return message
-        except Exception:
-            # TODO: remove this when reference parsing is fixed
-            print('ERROR')
+        Message = dataclasses.make_dataclass('message', [c.replace('-', '_') for c in columns])
+        message = Message(*row)
+        message.process = 0 if message.process is None else struct.unpack('<I', message.process[0].ljust(4, b'\x00'))[0]
+        message.thread = struct.unpack('<I', message.thread[0].ljust(4, b'\x00'))[0]
+
+        string_fields = ('message_type', 'format_string', 'subsystem', 'category', 'sender_image_path',
+                         'event_type', 'name')
+        for f in string_fields:
+            if hasattr(message, f):
+                v = getattr(message, f)
+                setattr(message, f, decode_str(v) if v else v)
+
+        if hasattr(message, 'message'):
+            return message
 
     def _handle_placeholder_count(self, word):
         """ remove `count` last items from stack """
         count = word & 0xff
         if count > 0:
             self.stack = self.stack[:-count]
 
     def _handle_convert_mach_continuous(self, word):
-        """ push an item and pop it. effictively do nothing """
+        """ push an item and pop it. effectively do nothing """
         pass
 
     def _parse(self):
         word = self._read_word()
 
         operations = {
             CMD_TABLE_RESET: self._handle_table_reset,
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/application_listing.py` & `pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/application_listing.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/condition_inducer.py` & `pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/condition_inducer.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,25 +4,28 @@
 from pymobiledevice3.services.remote_server import MessageAux
 
 
 class ConditionInducer:
     IDENTIFIER = 'com.apple.instruments.server.services.ConditionInducer'
 
     def __init__(self, dvt):
+        self.logger = logging.getLogger(__name__)
         self._channel = dvt.make_channel(self.IDENTIFIER)
 
     def list(self) -> list:
         self._channel.availableConditionInducers()
         return self._channel.receive_plist()
 
     def set(self, profile_identifier):
         for group in self.list():
             for profile in group.get('profiles'):
                 if profile_identifier == profile.get('identifier'):
-                    logging.info(profile.get('description'))
+                    self.logger.info(profile.get('description'))
                     self._channel.enableConditionWithIdentifier_profileIdentifier_(
                         MessageAux().append_obj(group.get('identifier')).append_obj(profile.get('identifier')))
+                    # wait for response which may be a raised NSError
+                    self._channel.receive_plist()
                     return
         raise PyMobileDevice3Exception('Invalid profile identifier')
 
     def clear(self):
         self._channel.disableActiveCondition()
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/core_profile_session_tap.py` & `pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/core_profile_session_tap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+import time
 import typing
 import uuid
-from datetime import timezone, timedelta
+from datetime import timedelta, timezone
 from io import BytesIO
 
-from construct import Struct, Int32ul, Int64ul, FixedSized, GreedyRange, GreedyBytes, Enum, Switch, Padding, Padded, \
-    LazyBound, CString, Computed, Array, this, Byte, Int16ul, Pass, Bytes
+from construct import Array, Byte, Bytes, Computed, CString, Enum, FixedSized, GreedyBytes, GreedyRange, GreedyString, \
+    Int16ul, Int32ul, Int64ul, LazyBound, Padded, Padding, Pass, Struct, Switch, this
+from pykdebugparser.kd_buf_parser import RAW_VERSION2_BYTES
 
+from pymobiledevice3.exceptions import ExtractingStackshotError
 from pymobiledevice3.resources.dsc_uuid_map import get_dsc_map
 from pymobiledevice3.services.dvt.dvt_secure_socket_proxy import DvtSecureSocketProxyService
 from pymobiledevice3.services.dvt.instruments.device_info import DeviceInfo
 from pymobiledevice3.services.remote_server import Tap
 
 kcdata_types = {
     'KCDATA_TYPE_INVALID': 0x0,
@@ -95,14 +98,16 @@
     'STACKSHOT_KCTYPE_LATENCY_INFO': 0x92b,
     'STACKSHOT_KCTYPE_LATENCY_INFO_TASK': 0x92c,
     'STACKSHOT_KCTYPE_LATENCY_INFO_THREAD': 0x92d,
     'STACKSHOT_KCTYPE_LOADINFO64_TEXT_EXEC': 0x92e,
 
     'STACKSHOT_KCTYPE_TASK_DELTA_SNAPSHOT': 0x940,
     'STACKSHOT_KCTYPE_THREAD_DELTA_SNAPSHOT': 0x941,
+    'STACKSHOT_KCTYPE_UNKNOWN_0x942': 0x942,
+    'STACKSHOT_KCTYPE_UNKNOWN_0x943': 0x943,
 
     'KCDATA_TYPE_BUFFER_END': 0xF19158ED,
 
     'TASK_CRASHINFO_EXTMODINFO': 0x801,
     'TASK_CRASHINFO_BSDINFOWITHUNIQID': 0x802,
     'TASK_CRASHINFO_TASKDYLD_INFO': 0x803,
     'TASK_CRASHINFO_UUID': 0x804,
@@ -175,14 +180,15 @@
     kcdata_types_enum.STACKSHOT_KCTYPE_USER_STACKLR64: 'user_stack_frames',
     kcdata_types_enum.STACKSHOT_KCTYPE_JETSAM_COALITION_SNAPSHOT: 'jetsam_coalition_snapshot',
     kcdata_types_enum.STACKSHOT_KCTYPE_DONATING_PIDS: 'donating_pids',
     kcdata_types_enum.STACKSHOT_KCTYPE_THREAD_DISPATCH_QUEUE_LABEL: 'dispatch_queue_label',
     kcdata_types_enum.KCDATA_BUFFER_BEGIN_STACKSHOT: 'kcdata_stackshot',
     kcdata_types_enum.STACKSHOT_KCTYPE_STACKSHOT_FAULT_STATS: 'stackshot_fault_stats',
     kcdata_types_enum.STACKSHOT_KCTYPE_STACKSHOT_DURATION: 'stackshot_duration',
+    kcdata_types_enum.STACKSHOT_KCTYPE_LOADINFO64_TEXT_EXEC: 'dyld_load_info_text_exec',
 }
 
 predefined_name_substruct = 'name' / Computed(lambda ctx: predefined_names[ctx._.type])
 
 uint32_desc = Struct(
     'name' / Padded(32, CString('utf8')),
     'obj' / Int32ul,
@@ -212,21 +218,39 @@
     'obj' / Struct(
         'imageLoadAddress' / Int64ul,
         '_imageUUID' / Bytes(16),
         'imageUUID' / Computed(lambda ctx: uuid.UUID(bytes=ctx._imageUUID)),
         'imageSlidBaseAddress' / Int64ul,
     ),
 )
+
+thread_group_snapshot_trace_v2 = Struct(
+    'tgs_id' / Int64ul,
+    '_tgs_name' / FixedSized(16, GreedyString('utf8')),
+    'tgs_name' / Computed(lambda ctx: ctx._tgs_name.strip('\x00')),
+    'tgs_flags' / Int64ul,
+)
+
+thread_group_snapshot_trace_v3 = Struct(
+    'tgs_id' / Int64ul,
+    '_tgs_name' / FixedSized(16, GreedyString('utf8')),
+    'tgs_flags' / Int64ul,
+    '_tgs_name_cont' / FixedSized(16, GreedyString('utf8')),
+    'tgs_name' / Computed(lambda ctx: ctx._tgs_name.strip('\x00') + ctx._tgs_name_cont.strip('\x00')),
+)
+
 thread_group_snapshot = Struct(
     predefined_name_substruct,
-    'obj' / Struct(
-        'tgs_id' / Int64ul,
-        'tgs_name' / Padded(16, CString('utf8')),
-        'tgs_flags' / Int64ul
-    ),
+    'obj' / Switch(
+        lambda ctx: ctx._._.size // ctx._.count,
+        {
+            thread_group_snapshot_trace_v2.sizeof(): thread_group_snapshot_trace_v2,
+            thread_group_snapshot_trace_v3.sizeof(): thread_group_snapshot_trace_v3,
+        }
+    )
 )
 type_array_pad0 = Struct(
     'flags_type' / Computed(lambda ctx: (ctx._.flags >> 32) & 0xffffffff),
     'type' / Computed(lambda ctx: kcdata_types_enum.decmapping[ctx.flags_type]),
     'count' / Computed(lambda ctx: ctx._.flags & 0xffffffff),
     'name' / Computed(lambda ctx: predefined_names[ctx.type]),
     'obj' / Array(this.count, LazyBound(lambda: Switch(
@@ -269,15 +293,15 @@
         kcdata_types_structures,
         default=GreedyBytes
     ))),
     Padding(0xc),
 )
 type_container_begin = Struct(
     'obj' / kcdata_types_enum,
-    'name' / Computed(lambda ctx: predefined_names[ctx.obj]),
+    'name' / Computed(lambda ctx: predefined_names.get(ctx.obj, 'unknown')),
     'unique_id' / Computed(lambda ctx: ctx._.flags),
 )
 kernelcache_load_info = Struct(
     predefined_name_substruct,
     'obj' / Struct(
         'imageLoadAddress' / Int64ul,
         '_imageUUID' / Bytes(16),
@@ -405,14 +429,23 @@
     predefined_name_substruct,
     'obj' / Struct(
         'stackshot_duration' / Int64ul,
         'stackshot_duration_outer' / Int64ul,
     )
 )
 
+loadinfo64_text_exec = Struct(
+    predefined_name_substruct,
+    'obj' / Struct(
+        'imageLoadAddress' / Int64ul,
+        '_imageUUID' / Bytes(16),
+        'imageUUID' / Computed(lambda ctx: uuid.UUID(bytes=ctx._imageUUID)),
+    ),
+)
+
 kcdata_types_structures = {
     kcdata_types_enum.KCDATA_TYPE_UINT32_DESC: uint32_desc,
     kcdata_types_enum.KCDATA_TYPE_UINT64_DESC: uint64_desc,
     kcdata_types_enum.STACKSHOT_KCTYPE_JETSAM_LEVEL: jetsam_level,
     kcdata_types_enum.STACKSHOT_KCTYPE_THREAD_POLICY_VERSION: thread_policy_version,
     kcdata_types_enum.STACKSHOT_KCTYPE_KERN_PAGE_SIZE: kernel_page_size,
     kcdata_types_enum.STACKSHOT_KCTYPE_OSVERSION: osversion,
@@ -443,14 +476,15 @@
     kcdata_types_enum.STACKSHOT_KCTYPE_DONATING_PIDS: donating_pids,
     kcdata_types_enum.STACKSHOT_KCTYPE_THREAD_DISPATCH_QUEUE_LABEL: dispatch_queue_label,
     kcdata_types_enum.STACKSHOT_KCTYPE_STACKSHOT_FAULT_STATS: stackshot_fault_stats,
     kcdata_types_enum.KCDATA_BUFFER_BEGIN_STACKSHOT: Struct(predefined_name_substruct),
     kcdata_types_enum.KCDATA_TYPE_CONTAINER_END: Pass,
     kcdata_types_enum.KCDATA_TYPE_BUFFER_END: Pass,
     kcdata_types_enum.STACKSHOT_KCTYPE_STACKSHOT_DURATION: stackshot_duration,
+    kcdata_types_enum.STACKSHOT_KCTYPE_LOADINFO64_TEXT_EXEC: loadinfo64_text_exec,
 }
 
 kcdata_item = Struct(
     'type' / kcdata_types_enum,
     'size' / Int32ul,
     'flags' / Int64ul,
     'data' / FixedSized(lambda ctx: ctx.size, Switch(
@@ -490,15 +524,16 @@
             current_index = jsonify_parsed_stackshot(stackshot, root[item['data']['name']][item['data']['unique_id']],
                                                      current_index)
         elif item['type'] == kcdata_types_enum.KCDATA_TYPE_CONTAINER_END:
             return current_index
         elif item['type'] == kcdata_types_enum.KCDATA_TYPE_BUFFER_END:
             return
         else:
-            root[item['data']['name']] = item['data']['obj']
+            if isinstance(item['data'], dict):
+                root[item['data']['name']] = item['data']['obj']
 
 
 STACKSHOT_HEADER = Int32ul.build(int(kcdata_types_enum.KCDATA_BUFFER_BEGIN_STACKSHOT))
 
 
 class KdBufStream:
     def __init__(self, channel):
@@ -579,61 +614,70 @@
     def get_stackshot(self) -> typing.Mapping:
         """
         Get a stackshot from the tap.
         """
         if self.stack_shot is not None:
             # The stackshot is sent one per TAP creation, so we cache it.
             return self.stack_shot
-        data = self._channel.receive_message()
-        while not data.startswith(STACKSHOT_HEADER):
-            data = self._channel.receive_message()
+        data = self.channel.receive_message()
+        while not data.startswith(STACKSHOT_HEADER) and not data.startswith(RAW_VERSION2_BYTES):
+            data = self.channel.receive_message()
+
+        if data.startswith(RAW_VERSION2_BYTES):
+            raise ExtractingStackshotError()
+
         stackshot = self.parse_stackshot(data)
 
         dsc_map = get_dsc_map(str(stackshot['shared_cache_dyld_load_info']['imageUUID']))
 
         for pid, snapshot in stackshot['task_snapshots'].items():
             for loaded_image in snapshot.get('dyld_load_info', []):
                 image_uuid = str(loaded_image['imageUUID'])
                 if isinstance(dsc_map, dict) and image_uuid in dsc_map:
                     loaded_image['imagePath'] = dsc_map[image_uuid]
 
         self.stack_shot = stackshot
 
         return self.stack_shot
 
-    def dump(self, out: typing.BinaryIO):
+    def dump(self, out: typing.BinaryIO, timeout: int = None):
         """
         Dump data from core profile session to a file.
         :param out: File object to write data to.
+        :param timeout: Timeout for data dumping, in seconds.
         """
-        while True:
-            data = self._channel.receive_message()
+        start = time.time()
+        while timeout is None or time.time() <= start + timeout:
+            data = self.channel.receive_message()
             if data.startswith(STACKSHOT_HEADER) or data.startswith(b'bplist'):
                 # Skip not kernel trace data.
                 continue
             print(f'Receiving trace data ({len(data)}B)')
             out.write(data)
             out.flush()
 
     def get_kdbuf_stream(self):
         """
         Get kd_buf stream.
         """
-        return KdBufStream(self._channel)
+        return KdBufStream(self.channel)
 
     @staticmethod
     def parse_stackshot(data):
         parsed = kcdata.parse(data)
         # Required for removing streams from construct output.
         stackshot = clean(parsed)
         parsed_stack_shot = {}
         jsonify_parsed_stackshot(stackshot, parsed_stack_shot)
         return parsed_stack_shot[predefined_names[kcdata_types_enum.KCDATA_BUFFER_BEGIN_STACKSHOT]]
 
     @staticmethod
     def get_time_config(dvt):
-        mach_absolute_time, numer, denom, _ = DeviceInfo(dvt).mach_time_info()
+        time_info = DeviceInfo(dvt).mach_time_info()
+        mach_absolute_time = time_info[0]
+        numer = time_info[1]
+        denom = time_info[2]
         usecs_since_epoch = dvt.lockdown.get_value(key='TimeIntervalSince1970') * 1000000
         return dict(
             numer=numer, denom=denom, mach_absolute_time=mach_absolute_time, usecs_since_epoch=usecs_since_epoch,
             timezone=timezone(timedelta(seconds=dvt.lockdown.get_value(key='TimeZoneOffsetFromUTC')))
         )
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/device_info.py` & `pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/device_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import plistlib
+import typing
 from datetime import datetime
 
 from pymobiledevice3.exceptions import DvtDirListError
 from pymobiledevice3.services.remote_server import MessageAux
 
 
 class DeviceInfo:
@@ -51,14 +53,28 @@
 
     def network_information(self):
         return self.request_information('networkInformation')
 
     def mach_time_info(self):
         return self.request_information('machTimeInfo')
 
+    def mach_kernel_name(self) -> str:
+        return self.request_information('machKernelName')
+
+    def kpep_database(self) -> typing.Mapping:
+        return plistlib.loads(self.request_information('kpepDatabase'))
+
     def trace_codes(self):
         codes_file = self.request_information('traceCodesFile')
-        return {int(k, 16): v for k, v in map(lambda l: l.split(), codes_file.splitlines())}
+        return {int(k, 16): v for k, v in map(lambda line: line.split(), codes_file.splitlines())}
 
     def request_information(self, selector_name):
         self._channel[selector_name]()
         return self._channel.receive_plist()
+
+    def name_for_uid(self, uid: int) -> str:
+        self._channel.nameForUID_(MessageAux().append_obj(uid))
+        return self._channel.receive_plist()
+
+    def name_for_gid(self, gid: int) -> str:
+        self._channel.nameForGID_(MessageAux().append_obj(gid))
+        return self._channel.receive_plist()
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/energy_monitor.py` & `pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/energy_monitor.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/graphics.py` & `pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/graphics.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/network_monitor.py` & `pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/network_monitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import dataclasses
 import ipaddress
 import logging
 
-from construct import Struct, Int32ul, this, Adapter, Switch, Int8ul, Int16ub, Bytes
+from construct import Adapter, Bytes, Int8ul, Int16ub, Int32ul, Struct, Switch, this
 
 
 class IpAddressAdapter(Adapter):
     def _decode(self, obj, context, path):
         return ipaddress.ip_address(obj)
 
 
@@ -66,14 +66,15 @@
     unknown1: int
 
 
 class NetworkMonitor:
     IDENTIFIER = 'com.apple.instruments.server.services.networking'
 
     def __init__(self, dvt):
+        self.logger = logging.getLogger(__name__)
         self._channel = dvt.make_channel(self.IDENTIFIER)
 
     def __enter__(self):
         self._channel.startMonitoring(expects_reply=False)
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
@@ -93,9 +94,9 @@
             elif message[0] == MESSAGE_TYPE_CONNECTION_DETECTION:
                 event = ConnectionDetectionEvent(*message[1])
                 event.local_address = address_t.parse(event.local_address)
                 event.remote_address = address_t.parse(event.remote_address)
             elif message[0] == MESSAGE_TYPE_CONNECTION_UPDATE:
                 event = ConnectionUpdateEvent(*message[1])
             else:
-                logging.warning(f'unsupported event type: {message[0]}')
+                self.logger.warning(f'unsupported event type: {message[0]}')
             yield event
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/notifications.py` & `pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/notifications.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/sysmontap.py` & `pymobiledevice3-2.0.0/pymobiledevice3/services/dvt/instruments/sysmontap.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             'sampleInterval': 500000000
         }
 
         super().__init__(dvt, self.IDENTIFIER, config)
 
     def __iter__(self):
         while True:
-            for result in self._channel.receive_plist():
+            for result in self.channel.receive_plist():
                 yield result
 
     def iter_processes(self):
         for row in self:
             if 'Processes' not in row:
                 continue
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/services/file_relay.py` & `pymobiledevice3-2.0.0/pymobiledevice3/services/file_relay.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import logging
-
 from pymobiledevice3.lockdown import LockdownClient
+from pymobiledevice3.services.base_service import BaseService
 
 SRCFILES = '''Baseband
 CrashReporter
 MobileAsset
 VARFS
 HFSMeta
 Lockdown
@@ -19,21 +18,19 @@
 NANDDebugInfo
 SystemConfiguration
 Ubiquity
 tmp
 WirelessAutomation'''
 
 
-class FileRelayService(object):
+class FileRelayService(BaseService):
     SERVICE_NAME = 'com.apple.mobile.file_relay'
 
-    def __init__(self, lockdown: LockdownClient, ):
-        self.logger = logging.getLogger(__name__)
-        self.lockdown = lockdown
-        self.service = self.lockdown.start_service(self.SERVICE_NAME)
+    def __init__(self, lockdown: LockdownClient):
+        super().__init__(lockdown, self.SERVICE_NAME)
         self.packet_num = 0
 
     def stop_session(self):
         self.logger.info('Disconecting...')
         self.service.close()
 
     def request_sources(self, sources=None):
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/services/house_arrest.py` & `pymobiledevice3-2.0.0/pymobiledevice3/services/house_arrest.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,8 +21,8 @@
             return False
         else:
             return True
 
     def shell(self, application_id, cmd='VendContainer'):
         res = self.send_command(application_id, cmd)
         if res:
-            AfcShell(self.lockdown).cmdloop()
+            AfcShell(self.lockdown, afc_service=self).cmdloop()
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/services/misagent.py` & `pymobiledevice3-2.0.0/pymobiledevice3/services/screenshot.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,29 @@
-from io import BytesIO
-
 from pymobiledevice3.exceptions import PyMobileDevice3Exception
 from pymobiledevice3.lockdown import LockdownClient
+from pymobiledevice3.services.base_service import BaseService
 
 
-class MisagentService(object):
-    SERVICE_NAME = 'com.apple.misagent'
+class ScreenshotService(BaseService):
+    SERVICE_NAME = 'com.apple.mobile.screenshotr'
 
     def __init__(self, lockdown: LockdownClient):
-        self.lockdown = lockdown
-        self.service = self.lockdown.start_service(self.SERVICE_NAME)
+        super().__init__(lockdown, self.SERVICE_NAME, is_developer_service=True)
+
+        dl_message_version_exchange = self.service.recv_plist()
+        version_major = dl_message_version_exchange[1]
+        dl_message_device_ready = self.service.send_recv_plist(
+            ['DLMessageVersionExchange', 'DLVersionsOk', version_major])
+        if dl_message_device_ready[0] != 'DLMessageDeviceReady':
+            raise PyMobileDevice3Exception('Screenshotr didn\'t return ready state')
+
+    def take_screenshot(self) -> bytes:
+        self.service.send_plist(['DLMessageProcessMessage', {'MessageType': 'ScreenShotRequest'}])
+        response = self.service.recv_plist()
+
+        assert len(response) == 2
+        assert response[0] == 'DLMessageProcessMessage'
 
-    def install(self, plist: BytesIO):
-        response = self.service.send_recv_plist({'MessageType': 'Install',
-                                                 'Profile': plist.read(),
-                                                 'ProfileType': 'Provisioning'})
-        if response['Status']:
-            raise PyMobileDevice3Exception(f'invalid status: {response}')
-
-        return response
-
-    def remove(self, profile_id):
-        response = self.service.send_recv_plist({'MessageType': 'Remove',
-                                                 'ProfileID': profile_id,
-                                                 'ProfileType': 'Provisioning'})
-        if response['Status']:
-            raise PyMobileDevice3Exception(f'invalid status: {response}')
-
-        return response
-
-    def copy_all(self):
-        response = self.service.send_recv_plist({'MessageType': 'CopyAll',
-                                                 'ProfileType': 'Provisioning'})
-        if response['Status']:
-            raise PyMobileDevice3Exception(f'invalid status: {response}')
+        if response[1].get('MessageType') == 'ScreenShotReply':
+            return response[1]['ScreenShotData']
 
-        return response['Payload']
+        raise PyMobileDevice3Exception(f'invalid response: {response}')
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/services/mobilebackup2.py` & `pymobiledevice3-2.0.0/pymobiledevice3/services/mobilebackup2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python3
-import logging
-from pathlib import Path
+import plistlib
 import time
 import uuid
-import plistlib
+from contextlib import contextmanager, suppress
 from datetime import datetime
-from contextlib import contextmanager
+from pathlib import Path
 
+from pymobiledevice3.exceptions import AfcException, AfcFileNotFoundError, ConnectionTerminatedError, LockdownError, \
+    PyMobileDevice3Exception
 from pymobiledevice3.lockdown import LockdownClient
-from pymobiledevice3.exceptions import PyMobileDevice3Exception, AfcFileNotFoundError, AfcException
-from pymobiledevice3.services.afc import AfcService, AFC_LOCK_EX, afc_error_t, AFC_LOCK_UN
+from pymobiledevice3.services.afc import AFC_LOCK_EX, AFC_LOCK_UN, AfcService, afc_error_t
+from pymobiledevice3.services.base_service import BaseService
 from pymobiledevice3.services.device_link import DeviceLink
 from pymobiledevice3.services.installation_proxy import InstallationProxyService
 from pymobiledevice3.services.notification_proxy import NotificationProxyService
 from pymobiledevice3.services.springboard import SpringBoardServicesService
 
 SUPPORTED_VERSIONS = [2.0, 2.1]
 ITUNES_FILES = [
@@ -23,31 +24,42 @@
 ]
 NP_SYNC_WILL_START = 'com.apple.itunes-mobdev.syncWillStart'
 NP_SYNC_DID_START = 'com.apple.itunes-mobdev.syncDidStart'
 NP_SYNC_LOCK_REQUEST = 'com.apple.itunes-mobdev.syncLockRequest'
 NP_SYNC_DID_FINISH = 'com.apple.itunes-mobdev.syncDidFinish'
 
 
-class Mobilebackup2Service:
+class Mobilebackup2Service(BaseService):
     SERVICE_NAME = 'com.apple.mobilebackup2'
 
     def __init__(self, lockdown: LockdownClient):
-        self.logger = logging.getLogger(__name__)
-        self.lockdown = lockdown
-        self.service = self.lockdown.start_service(self.SERVICE_NAME)
+        super().__init__(lockdown, self.SERVICE_NAME)
 
-    def backup(self, full=True, backup_directory=Path('.'), progress_callback=lambda x: None):
+    @property
+    def will_encrypt(self):
+        try:
+            return self.lockdown.get_value('com.apple.mobile.backup', 'WillEncrypt')
+        except LockdownError:
+            return False
+
+    def backup(self, full: bool = True, backup_directory='.', progress_callback=lambda x: None) -> None:
+        """
+        Backup a device.
+        :param full: Whether to do a full backup. If full is True, any previous backup attempts will be discarded.
+        :param backup_directory: Directory to write backup to.
+        :param progress_callback: Function to be called as the backup progresses.
+        The function shall receive the percentage as a parameter.
+        """
         backup_directory = Path(backup_directory)
-        device_directory = backup_directory / self.lockdown.identifier
+        device_directory = backup_directory / self.lockdown.udid
         device_directory.mkdir(exist_ok=True, mode=0o755, parents=True)
 
-        with self.device_link(backup_directory) as dl:
-            notification_proxy = NotificationProxyService(self.lockdown)
-            afc = AfcService(self.lockdown)
-
+        with self.device_link(backup_directory) as dl, \
+                NotificationProxyService(self.lockdown) as notification_proxy, \
+                AfcService(self.lockdown) as afc:
             with self._backup_lock(afc, notification_proxy):
                 # Initialize Info.plist
                 info_plist = self.init_mobile_backup_factory_info(afc)
                 with open(device_directory / 'Info.plist', 'wb') as fd:
                     plistlib.dump(info_plist, fd)
 
                 # Initialize Status.plist file if doesn't exist.
@@ -65,31 +77,42 @@
 
                 # Create Manifest.plist if doesn't exist.
                 manifest_path = device_directory / 'Manifest.plist'
                 if full:
                     manifest_path.unlink(missing_ok=True)
                 (device_directory / 'Manifest.plist').touch()
 
-                dl.send_process_message({'MessageName': 'Backup', 'TargetIdentifier': self.lockdown.identifier})
+                dl.send_process_message({'MessageName': 'Backup', 'TargetIdentifier': self.lockdown.udid})
                 dl.dl_loop(progress_callback)
 
-    def restore(self, backup_directory=Path('.'), system=False, reboot=True, copy=True, settings=True, remove=False,
-                password='', progress_callback=lambda x: None):
+    def restore(self, backup_directory='.', system: bool = False, reboot: bool = True, copy: bool = True,
+                settings: bool = True, remove: bool = False, password: str = '', source: str = '',
+                progress_callback=lambda x: None):
+        """
+        Restore a previous backup to the device.
+        :param backup_directory: Path of the backup directory.
+        :param system: Whether to restore system files.
+        :param reboot: Reboot the device when done.
+        :param copy: Create a copy of backup folder before restoring.
+        :param settings: Restore device settings.
+        :param remove: Remove items which aren't being restored.
+        :param password: Password of the backup if it is encrypted.
+        :param source: Identifier of device to restore its backup.
+        :param progress_callback: Function to be called as the backup progresses.
+        The function shall receive the current percentage of the progress as a parameter.
+        """
         backup_directory = Path(backup_directory)
-        device_directory = backup_directory / self.lockdown.identifier
-        assert device_directory.exists()
-
-        with self.device_link(backup_directory) as dl:
-            notification_proxy = NotificationProxyService(self.lockdown)
-            afc = AfcService(self.lockdown)
+        source = source if source else self.lockdown.udid
+        self._assert_backup_exists(backup_directory, source)
 
+        with self.device_link(backup_directory) as dl, \
+                NotificationProxyService(self.lockdown) as notification_proxy, \
+                AfcService(self.lockdown) as afc:
             with self._backup_lock(afc, notification_proxy):
-                assert (device_directory / 'Info.plist').exists()
-                manifest_plist_path = device_directory / 'Manifest.plist'
-                assert manifest_plist_path.exists()
+                manifest_plist_path = backup_directory / source / 'Manifest.plist'
                 with open(manifest_plist_path, 'rb') as fd:
                     manifest = plistlib.load(fd)
                 is_encrypted = manifest.get('IsEncrypted', False)
                 options = {
                     'RestoreShouldReboot': reboot,
                     'RestoreDontCopyBackup': copy,
                     'RestorePreserveSettings': settings,
@@ -100,154 +123,201 @@
                     if password:
                         options['Password'] = password
                     else:
                         self.logger.error('Backup is encrypted, please supply password.')
                         return
                 dl.send_process_message({
                     'MessageName': 'Restore',
-                    'TargetIdentifier': self.lockdown.identifier,
-                    'SourceIdentifier': self.lockdown.identifier,
+                    'TargetIdentifier': self.lockdown.udid,
+                    'SourceIdentifier': source,
                     'Options': options,
                 })
                 dl.dl_loop(progress_callback)
 
-    def info(self, backup_directory=Path('.')):
-        with self.device_link(Path(backup_directory)) as dl:
-            dl.send_process_message({'MessageName': 'Info', 'TargetIdentifier': self.lockdown.identifier})
+    def info(self, backup_directory='.', source: str = '') -> str:
+        """
+        Get information about a backup.
+        :param backup_directory: Path of the backup directory.
+        :param source: Identifier of device to get info about its backup.
+        :return: Information about a backup.
+        """
+        backup_dir = Path(backup_directory)
+        self._assert_backup_exists(backup_dir, source if source else self.lockdown.udid)
+        with self.device_link(backup_dir) as dl:
+            message = {'MessageName': 'Info', 'TargetIdentifier': self.lockdown.udid}
+            if source:
+                message['SourceIdentifier'] = source
+            dl.send_process_message(message)
             result = dl.dl_loop()
         return result
 
-    def list(self, backup_directory=Path('.')):
-        with self.device_link(Path(backup_directory)) as dl:
+    def list(self, backup_directory='.', source: str = '') -> str:
+        """
+        List the files in the last backup.
+        :param backup_directory: Path of the backup directory.
+        :param source: Identifier of device to list its backup data.
+        :return: List of files and additional data about each file, all in a CSV format.
+        """
+        backup_dir = Path(backup_directory)
+        source = source if source else self.lockdown.udid
+        self._assert_backup_exists(backup_dir, source)
+        with self.device_link(backup_dir) as dl:
             dl.send_process_message({
-                'MessageName': 'List', 'TargetIdentifier': self.lockdown.identifier,
-                'SourceIdentifier': self.lockdown.identifier
+                'MessageName': 'List', 'TargetIdentifier': self.lockdown.udid, 'SourceIdentifier': source,
             })
             result = dl.dl_loop()
         return result
 
-    def unback(self, backup_directory=Path('.'), password=''):
-        device_directory = Path(backup_directory) / self.lockdown.identifier
-        assert (device_directory / 'Info.plist').exists()
-        assert (device_directory / 'Manifest.plist').exists()
-        with self.device_link(Path(backup_directory)) as dl:
-            message = {'MessageName': 'Unback', 'TargetIdentifier': self.lockdown.identifier}
+    def unback(self, backup_directory='.', password: str = '', source: str = '') -> None:
+        """
+        Unpack a complete backup to its device hierarchy.
+        :param backup_directory: Path of the backup directory.
+        :param password: Password of the backup if it is encrypted.
+        :param source: Identifier of device to unpack its backup.
+        """
+        backup_dir = Path(backup_directory)
+        self._assert_backup_exists(backup_dir, source if source else self.lockdown.udid)
+        with self.device_link(backup_dir) as dl:
+            message = {'MessageName': 'Unback', 'TargetIdentifier': self.lockdown.udid}
+            if source:
+                message['SourceIdentifier'] = source
             if password:
                 message['Password'] = password
             dl.send_process_message(message)
-            result = dl.dl_loop()
-        return result
+            dl.dl_loop()
 
-    def extract(self, domain_name, relative_path, backup_directory=Path('.'), password=''):
-        device_directory = backup_directory / self.lockdown.identifier
-        assert (device_directory / 'Info.plist').exists()
-        assert (device_directory / 'Manifest.plist').exists()
-        with self.device_link(Path(backup_directory)) as dl:
+    def extract(self, domain_name: str, relative_path: str, backup_directory='.', password: str = '',
+                source: str = '') -> None:
+        """
+        Extract a file from a previous backup.
+        :param domain_name: File's domain name, e.g., SystemPreferencesDomain or HomeDomain.
+        :param relative_path: File path.
+        :param backup_directory: Path of the backup directory.
+        :param password: Password of the last backup if it is encrypted.
+        :param source: Identifier of device to extract file from its backup.
+        """
+        backup_dir = Path(backup_directory)
+        self._assert_backup_exists(backup_dir, source if source else self.lockdown.udid)
+        with self.device_link(backup_dir) as dl:
             message = {
-                'MessageName': 'Extract', 'TargetIdentifier': self.lockdown.identifier, 'DomainName': domain_name,
+                'MessageName': 'Extract', 'TargetIdentifier': self.lockdown.udid, 'DomainName': domain_name,
                 'RelativePath': relative_path
             }
+            if source:
+                message['SourceIdentifier'] = source
             if password:
                 message['Password'] = password
             dl.send_process_message(message)
-            result = dl.dl_loop()
-        return result
+            dl.dl_loop()
 
-    def change_password(self, backup_directory=Path('.'), old='', new=''):
+    def change_password(self, backup_directory='.', old: str = '', new: str = '') -> None:
+        """
+        Change backup password.
+        :param backup_directory: Backups directory.
+        :param old: Previous password. Omit when enabling backup encryption.
+        :param new: New password. Omit when disabling backup encryption.
+        """
         with self.device_link(Path(backup_directory)) as dl:
-            message = {'MessageName': 'ChangePassword', 'TargetIdentifier': self.lockdown.identifier}
+            message = {'MessageName': 'ChangePassword', 'TargetIdentifier': self.lockdown.udid}
             if old:
                 message['OldPassword'] = old
             if new:
                 message['NewPassword'] = new
             dl.send_process_message(message)
             dl.dl_loop()
 
-    def erase_device(self, backup_directory=Path('.')):
-        with self.device_link(Path(backup_directory)) as dl:
-            dl.send_process_message({'MessageName': 'EraseDevice', 'TargetIdentifier': self.lockdown.identifier})
-            dl.dl_loop()
-
-    def version_exchange(self, dl: DeviceLink, local_versions=None):
+    def erase_device(self, backup_directory='.') -> None:
+        """
+        Erase the device.
+        """
+        with suppress(ConnectionTerminatedError):
+            with self.device_link(Path(backup_directory)) as dl:
+                dl.send_process_message({'MessageName': 'EraseDevice', 'TargetIdentifier': self.lockdown.udid})
+                dl.dl_loop()
+
+    def version_exchange(self, dl: DeviceLink, local_versions=None) -> None:
+        """
+        Exchange versions with the device and assert that the device supports our version of the protocol.
+        :param dl: Initialized device link.
+        :param local_versions: versions supported by us.
+        """
         if local_versions is None:
             local_versions = SUPPORTED_VERSIONS
         dl.send_process_message({
             'MessageName': 'Hello',
             'SupportedProtocolVersions': local_versions,
         })
         reply = dl.receive_message()
         assert reply[0] == 'DLMessageProcessMessage' and reply[1]['ErrorCode'] == 0
-        assert reply[1]['ProtocolVersion'] in SUPPORTED_VERSIONS
+        assert reply[1]['ProtocolVersion'] in local_versions
 
     def init_mobile_backup_factory_info(self, afc: AfcService):
-        ip = InstallationProxyService(self.lockdown)
-        sbs = SpringBoardServicesService(self.lockdown)
+        with InstallationProxyService(self.lockdown) as ip, SpringBoardServicesService(self.lockdown) as sbs:
+            root_node = self.lockdown.get_value()
+            itunes_settings = self.lockdown.get_value(domain='com.apple.iTunes')
+            min_itunes_version = self.lockdown.get_value('com.apple.mobile.iTunes', 'MinITunesVersion')
+            app_dict = {}
+            installed_apps = []
+            apps = ip.browse(options={'ApplicationType': 'User'},
+                             attributes=['CFBundleIdentifier', 'ApplicationSINF', 'iTunesMetadata'])
+            for app in apps:
+                bundle_id = app['CFBundleIdentifier']
+                if bundle_id:
+                    installed_apps.append(bundle_id)
+                    if app.get('iTunesMetadata', False) and app.get('ApplicationSINF', False):
+                        app_dict[bundle_id] = {
+                            'ApplicationSINF': app['ApplicationSINF'],
+                            'iTunesMetadata': app['iTunesMetadata'],
+                            'PlaceholderIcon': sbs.get_icon_pngdata(bundle_id),
+                        }
+
+            files = {}
+            for file in ITUNES_FILES:
+                try:
+                    data_buf = afc.get_file_contents('/iTunes_Control/iTunes/' + file)
+                except AfcFileNotFoundError:
+                    pass
+                else:
+                    files[file] = data_buf
+
+            ret = {
+                'iTunes Version': min_itunes_version if min_itunes_version else '10.0.1',
+                'iTunes Files': files,
+                'Unique Identifier': self.lockdown.udid.upper(),
+                'Target Type': 'Device',
+                'Target Identifier': root_node['UniqueDeviceID'],
+                'Serial Number': root_node['SerialNumber'],
+                'Product Version': root_node['ProductVersion'],
+                'Product Type': root_node['ProductType'],
+                'Installed Applications': installed_apps,
+                'GUID': uuid.uuid4().bytes,
+                'Display Name': root_node['DeviceName'],
+                'Device Name': root_node['DeviceName'],
+                'Build Version': root_node['BuildVersion'],
+                'Applications': app_dict,
+            }
 
-        root_node = self.lockdown.get_value()
-        itunes_settings = self.lockdown.get_value(domain='com.apple.iTunes')
-        min_itunes_version = self.lockdown.get_value('com.apple.mobile.iTunes', 'MinITunesVersion')
-        app_dict = {}
-        installed_apps = []
-        apps = ip.browse(options={'ApplicationType': 'User'},
-                         attributes=['CFBundleIdentifier', 'ApplicationSINF', 'iTunesMetadata'])
-        for app in apps:
-            bundle_id = app['CFBundleIdentifier']
-            if bundle_id:
-                installed_apps.append(bundle_id)
-                if app.get('iTunesMetadata', False) and app.get('ApplicationSINF', False):
-                    app_dict[bundle_id] = {
-                        'ApplicationSINF': app['ApplicationSINF'],
-                        'iTunesMetadata': app['iTunesMetadata'],
-                        'PlaceholderIcon': sbs.get_icon_pngdata(bundle_id),
-                    }
+            if 'IntegratedCircuitCardIdentity' in root_node:
+                ret['ICCID'] = root_node['IntegratedCircuitCardIdentity']
+            if 'InternationalMobileEquipmentIdentity' in root_node:
+                ret['IMEI'] = root_node['InternationalMobileEquipmentIdentity']
+            if 'MobileEquipmentIdentifier' in root_node:
+                ret['MEID'] = root_node['MobileEquipmentIdentifier']
+            if 'PhoneNumber' in root_node:
+                ret['Phone Number'] = root_node['PhoneNumber']
 
-        files = {}
-        for file in ITUNES_FILES:
             try:
-                data_buf = afc.get_file_contents('/iTunes_Control/iTunes/' + file)
+                data_buf = afc.get_file_contents('/Books/iBooksData2.plist')
             except AfcFileNotFoundError:
                 pass
             else:
-                files[file] = data_buf
-
-        ret = {
-            'iTunes Version': min_itunes_version if min_itunes_version else '10.0.1',
-            'iTunes Files': files,
-            'Unique Identifier': self.lockdown.identifier.upper(),
-            'Target Type': 'Device',
-            'Target Identifier': root_node['UniqueDeviceID'],
-            'Serial Number': root_node['SerialNumber'],
-            'Product Version': root_node['ProductVersion'],
-            'Product Type': root_node['ProductType'],
-            'Installed Applications': installed_apps,
-            'GUID': uuid.uuid4().bytes,
-            'Display Name': root_node['DeviceName'],
-            'Device Name': root_node['DeviceName'],
-            'Build Version': root_node['BuildVersion'],
-            'Applications': app_dict,
-        }
-
-        if 'IntegratedCircuitCardIdentity' in root_node:
-            ret['ICCID'] = root_node['IntegratedCircuitCardIdentity']
-        if 'InternationalMobileEquipmentIdentity' in root_node:
-            ret['IMEI'] = root_node['InternationalMobileEquipmentIdentity']
-        if 'MobileEquipmentIdentifier' in root_node:
-            ret['MEID'] = root_node['MobileEquipmentIdentifier']
-        if 'PhoneNumber' in root_node:
-            ret['Phone Number'] = root_node['PhoneNumber']
-
-        try:
-            data_buf = afc.get_file_contents('/Books/iBooksData2.plist')
-        except AfcFileNotFoundError:
-            pass
-        else:
-            ret['iBooks Data 2'] = data_buf
-        if itunes_settings:
-            ret['iTunes Settings'] = itunes_settings
-        return ret
+                ret['iBooks Data 2'] = data_buf
+            if itunes_settings:
+                ret['iTunes Settings'] = itunes_settings
+            return ret
 
     @contextmanager
     def _backup_lock(self, afc, notification_proxy):
         notification_proxy.notify_post(NP_SYNC_WILL_START)
         lockfile = afc.fopen('/com.apple.itunes.lock_sync', 'r+')
         if lockfile:
             notification_proxy.notify_post(NP_SYNC_LOCK_REQUEST)
@@ -269,14 +339,21 @@
         try:
             yield
         finally:
             afc.lock(lockfile, AFC_LOCK_UN)
             afc.fclose(lockfile)
             notification_proxy.notify_post(NP_SYNC_DID_FINISH)
 
+    @staticmethod
+    def _assert_backup_exists(backup_directory: Path, identifier: str):
+        device_directory = backup_directory / identifier
+        assert (device_directory / 'Info.plist').exists()
+        assert (device_directory / 'Manifest.plist').exists()
+        assert (device_directory / 'Status.plist').exists()
+
     @contextmanager
     def device_link(self, backup_directory):
         dl = DeviceLink(self.service, backup_directory)
         dl.version_exchange()
         self.version_exchange(dl)
         try:
             yield dl
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/services/os_trace.py` & `pymobiledevice3-2.0.0/pymobiledevice3/services/os_trace.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 #!/usr/bin/env python3
 import logging
 import plistlib
 import struct
 import tempfile
+import typing
 from datetime import datetime
-from io import BytesIO
 from tarfile import TarFile
 
-from construct import Struct, Bytes, Int32ul, Optional, Enum, Byte, Adapter, Int16ul, this, Computed, \
-    RepeatUntil
+from construct import Adapter, Byte, Bytes, Computed, Enum, Int16ul, Int32ul, Optional, RepeatUntil, Struct, this
+
 from pymobiledevice3.exceptions import PyMobileDevice3Exception
 from pymobiledevice3.lockdown import LockdownClient
+from pymobiledevice3.services.base_service import BaseService
+from pymobiledevice3.utils import try_decode
 
 CHUNK_SIZE = 4096
 TIME_FORMAT = '%H:%M:%S'
 SYSLOG_LINE_SPLITTER = '\n\x00'
 
 
 class TimestampAdapter(Adapter):
@@ -27,22 +29,14 @@
 
 timestamp_t = Struct(
     'seconds' / Int32ul,
     Bytes(4),
     'microseconds' / Int32ul
 )
 
-
-def try_decode(s):
-    try:
-        return s.decode('utf8')
-    except UnicodeDecodeError:
-        return s
-
-
 syslog_t = Struct(
     Bytes(9),
     'pid' / Int32ul,
     Bytes(42),
     'timestamp' / TimestampAdapter(timestamp_t),
     Bytes(1),
     'level' / Enum(Byte, Notice=0, Info=0x01, Debug=0x02, Error=0x10, Fault=0x11),
@@ -64,62 +58,79 @@
         'subsystem' / Computed(lambda ctx: try_decode(ctx._subsystem[:-1])),
         '_category' / Bytes(this._._category_size),
         'category' / Computed(lambda ctx: try_decode(ctx._category[:-1])),
     )),
 )
 
 
-class OsTraceService(object):
+class OsTraceService(BaseService):
+    """
+    Provides API for the following operations:
+    * Show process list (process name and pid)
+    * Stream syslog lines in binary form with optional filtering by pid.
+    * Get old stored syslog archive in PAX format (can be extracted using `pax -r < filename`).
+        * Archive contain the contents are the `/var/db/diagnostics` directory
+    """
     SERVICE_NAME = 'com.apple.os_trace_relay'
 
     def __init__(self, lockdown: LockdownClient):
+        super().__init__(lockdown, self.SERVICE_NAME)
         self.logger = logging.getLogger(__name__)
-        self.lockdown = lockdown
-        self.c = self.lockdown.start_service(self.SERVICE_NAME)
 
     def get_pid_list(self):
-        self.c.send_plist({'Request': 'PidList'})
+        self.service.send_plist({'Request': 'PidList'})
 
         # ignore first received unknown byte
-        self.c.recvall(1)
+        self.service.recvall(1)
 
-        response = self.c.recv_prefixed()
+        response = self.service.recv_prefixed()
         return plistlib.loads(response)
 
-    def create_archive(self, out: BytesIO):
-        self.c.send_plist({'Request': 'CreateArchive'})
+    def create_archive(self, out: typing.IO, size_limit: int = None, age_limit: int = None, start_time: int = None):
+        request = {'Request': 'CreateArchive'}
+
+        if size_limit is not None:
+            request.update({'SizeLimit': size_limit})
+
+        if age_limit is not None:
+            request.update({'AgeLimit': age_limit})
+
+        if start_time is not None:
+            request.update({'StartTime': start_time})
+
+        self.service.send_plist(request)
 
-        assert 1 == self.c.recvall(1)[0]
+        assert 1 == self.service.recvall(1)[0]
 
-        assert plistlib.loads(self.c.recv_prefixed()).get('Status') == 'RequestSuccessful', 'Invalid status'
+        assert plistlib.loads(self.service.recv_prefixed()).get('Status') == 'RequestSuccessful', 'Invalid status'
 
         while True:
             try:
-                assert 3 == self.c.recvall(1)[0], 'invalid magic'
+                assert 3 == self.service.recvall(1)[0], 'invalid magic'
             except ConnectionAbortedError:
                 break
-            out.write(self.c.recv_prefixed(endianity='<'))
+            out.write(self.service.recv_prefixed(endianity='<'))
 
-    def collect(self, out: str):
+    def collect(self, out: str, size_limit: int = None, age_limit: int = None, start_time: int = None):
         """
         Collect the system logs into a .logarchive that can be viewed later with tools such as log or Console.
         """
         with tempfile.NamedTemporaryFile() as tar:
-            self.create_archive(tar)
+            self.create_archive(tar, size_limit=size_limit, age_limit=age_limit, start_time=start_time)
             TarFile(tar.name).extractall(out)
 
     def syslog(self, pid=-1):
-        self.c.send_plist({'Request': 'StartActivity', 'MessageFilter': 65535, 'Pid': pid, 'StreamFlags': 60})
+        self.service.send_plist({'Request': 'StartActivity', 'MessageFilter': 65535, 'Pid': pid, 'StreamFlags': 60})
 
-        length_length, = struct.unpack('<I', self.c.recvall(4))
-        length = int(self.c.recvall(length_length)[::-1].hex(), 16)
-        response = plistlib.loads(self.c.recvall(length))
+        length_length, = struct.unpack('<I', self.service.recvall(4))
+        length = int(self.service.recvall(length_length)[::-1].hex(), 16)
+        response = plistlib.loads(self.service.recvall(length))
 
         if response.get('Status') != 'RequestSuccessful':
             raise PyMobileDevice3Exception(f'got invalid response: {response}')
 
         while True:
-            assert b'\x02' == self.c.recvall(1)
-            length, = struct.unpack('<I', self.c.recvall(4))
-            line = self.c.recvall(length)
+            assert b'\x02' == self.service.recvall(1)
+            length, = struct.unpack('<I', self.service.recvall(4))
+            line = self.service.recvall(length)
             entry = syslog_t.parse(line)
             yield entry
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/services/pcapd.py` & `pymobiledevice3-2.0.0/pymobiledevice3/services/pcapd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/env python3
 
-import logging
+import enum
 import socket
 import struct
-import enum
+from typing import Generator
 
-from construct import Struct, Int32ub, Int32ul, Bytes, Byte, this, Padding, Padded, CString
+from construct import Byte, Bytes, Container, CString, Int16ub, Int32ub, Int32ul, Padded, Seek, Struct, this
 
 from pymobiledevice3.lockdown import LockdownClient
+from pymobiledevice3.services.base_service import BaseService
 
 INTERFACE_NAMES = enum.Enum('InterfaceNames', names={
     'other': 1,
     'regular1822': 2,
     'hdh1822': 3,
     'ddnX25': 4,
     'rfc877x25': 5,
@@ -297,40 +298,44 @@
 ETHERNET_HEADER = b'\xBE\xEF' * 6 + b'\x08\x00'
 
 device_packet_struct = Struct(
     'header_length' / Int32ub,
     'header_version' / Byte,
     'packet_length' / Int32ub,
     'interface_type' / Byte,
-    Padding(2),
-    Padding(1),
+    'unit' / Int16ub,
+    'io' / Byte,
     'protocol_family' / Int32ub,
     'frame_pre_length' / Int32ub,
     'frame_post_length' / Int32ub,
     'interface_name' / Padded(16, CString('utf8')),
     'pid' / Int32ul,
     'comm' / Padded(17, CString('utf8')),
     'svc' / Int32ub,
     'epid' / Int32ul,
     'ecomm' / Padded(17, CString('utf8')),
     'seconds' / Int32ub,
     'microseconds' / Int32ub,
-    'data' / Bytes(this.packet_length)
+    Seek(this.header_length),
+    'data' / Bytes(this.packet_length),
 )
 
 
-class PcapdService:
+class PcapdService(BaseService):
+    """
+    Starting iOS 5, apple added a remote virtual interface (RVI) facility that allows mirroring networks traffic from
+    an iOS device. On macOS, the virtual interface can be enabled with the rvictl command. This script allows to use
+    this service on other systems.
+    """
     SERVICE_NAME = 'com.apple.pcapd'
 
     def __init__(self, lockdown: LockdownClient):
-        self.logger = logging.getLogger(__name__)
-        self.lockdown = lockdown
-        self.service = self.lockdown.start_service(self.SERVICE_NAME)
+        super().__init__(lockdown, self.SERVICE_NAME)
 
-    def watch(self, packets_count: int = -1, process: str = None):
+    def watch(self, packets_count: int = -1, process: str = None) -> Generator[Container, None, None]:
         packet_index = 0
         while packet_index != packets_count:
             d = self.service.recv_plist()
             if not d:
                 break
 
             packet = device_packet_struct.parse(d)
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/services/preboard.py` & `pymobiledevice3-2.0.0/pymobiledevice3/services/preboard.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 #!/usr/bin/env python3
-import logging
 
 from pymobiledevice3.lockdown import LockdownClient
+from pymobiledevice3.services.base_service import BaseService
 
 
-class PreboardService(object):
+class PreboardService(BaseService):
     SERVICE_NAME = 'com.apple.preboardservice_v2'
 
     def __init__(self, lockdown: LockdownClient):
-        self.logger = logging.getLogger(__name__)
-        self.lockdown = lockdown
-        self.c = self.lockdown.start_service(self.SERVICE_NAME)
+        super().__init__(lockdown, self.SERVICE_NAME)
 
     def create_stashbag(self, manifest):
-        return self.c.send_recv_plist({'Command': 'CreateStashbag', 'Manifest': manifest})
+        return self.service.send_recv_plist({'Command': 'CreateStashbag', 'Manifest': manifest})
 
     def commit(self, manifest):
-        return self.c.send_recv_plist({'Command': 'CommitStashbag', 'Manifest': manifest})
+        return self.service.send_recv_plist({'Command': 'CommitStashbag', 'Manifest': manifest})
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/services/remote_server.py` & `pymobiledevice3-2.0.0/pymobiledevice3/services/remote_server.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import io
-import logging
 import plistlib
+import typing
 from functools import partial
 from pprint import pprint
-from queue import Queue, Empty
+from queue import Empty, Queue
 
 import IPython
 from bpylist2 import archiver
-from construct import Struct, Default, Int64ul, Prefixed, GreedyRange, Select, Const, Int32ul, Switch, this, \
-    GreedyBytes, Adapter, Int16ul, Int32sl
-from pygments import highlight, lexers, formatters
+from construct import Adapter, Const, Default, GreedyBytes, GreedyRange, Int16ul, Int32sl, Int32ul, Int64ul, Prefixed, \
+    Select, Struct, Switch, this
+from pygments import formatters, highlight, lexers
 
-from pymobiledevice3.exceptions import DvtException
+from pymobiledevice3.exceptions import DvtException, UnrecognizedSelectorError
 from pymobiledevice3.lockdown import LockdownClient
+from pymobiledevice3.services.base_service import BaseService
 
 SHELL_USAGE = '''
 # This shell allows you to send messages to the DVTSecureSocketProxy and receive answers easily.
 # Generally speaking, each channel represents a group of actions.
 # Calling actions is done using a selector and auxiliary (parameters).
 # Receiving answers is done by getting a return value and seldom auxiliary (private / extra parameters).
 # To see the available channels, type the following:
@@ -111,22 +112,26 @@
     def decode_archive(archive_obj):
         return None
 
 
 class NSError:
     @staticmethod
     def decode_archive(archive_obj):
+        user_info = archive_obj.decode('NSUserInfo')
+        if user_info.get('NSLocalizedDescription', '').endswith(' - it does not respond to the selector'):
+            raise UnrecognizedSelectorError(user_info)
         raise DvtException(archive_obj.decode('NSUserInfo'))
 
 
 archiver.update_class_map({'DTSysmonTapMessage': DTTapMessage,
                            'DTTapHeartbeatMessage': DTTapMessage,
                            'DTTapStatusMessage': DTTapMessage,
                            'DTKTraceTapMessage': DTTapMessage,
                            'DTActivityTraceTapMessage': DTTapMessage,
+                           'DTTapMessage': DTTapMessage,
                            'NSNull': NSNull,
                            'NSError': NSError})
 
 
 class Channel(int):
     @classmethod
     def create(cls, value: int, service):
@@ -178,24 +183,66 @@
             self._stream_packet_data += chunk
             if mheader.fragmentId == mheader.fragmentCount - 1:
                 # last message
                 self._messages.put(self._stream_packet_data)
                 self._stream_packet_data = b''
 
 
-class RemoteServer(object):
+class RemoteServer(BaseService):
+    """
+    Wrapper to Apple's RemoteServer.
+    This server exports several ObjC objects allowing calling their respective selectors.
+    The `/Developer/Library/PrivateFrameworks/DVTInstrumentsFoundation.framework/DTServiceHub` service reads the
+    configuration stored from `[[NSUserDefaults standardUserDefaults] boolForKey:@"DTXConnectionTracer"]`
+    If the value is true, then `/tmp/DTServiceHub[PID].DTXConnection.RANDOM.log` is created and can be used to debug the
+    transport protocol.
+
+    For example:
+
+    ```
+    root@iPhone (/var/root)# tail -f /tmp/DTServiceHub[369].DTXConnection.qNjM2U.log
+    170.887982 x4 resuming [c0]: <DTXConnection 0x100d20670 : x4>
+    170.889120 x4   sent   [c0]: < DTXMessage 0x100d52b10 : i2.0 c0 dispatch:[_notifyOfPublishedCapabilities:<NSDictionary 0x100d0e1b0 | 92 key/value pairs>] >
+    170.889547 x4 received [c0]: < DTXMessage 0x100d0a550 : i1.0 c0 dispatch:[_notifyOfPublishedCapabilities:<NSDictionary 0x100d16a40 | 2 key/value pairs>] >
+    170.892101 x4 received [c0]: < DTXMessage 0x100d0a550 : i3.0e c0 dispatch:[_requestChannelWithCode:[1]identifier :"com.apple.instruments.server.services.deviceinfo"] >
+    170.892238 x4   sent   [c0]: < DTXMessage 0x100d61830 : i3.1 c0 >
+    170.892973 x4 received [c1f]: < DTXMessage 0x100d0a550 : i4.0e c1 dispatch:[runningProcesses] >
+    171.204957 x4   sent   [c1f]: < DTXMessage 0x100c557a0 : i4.1 c1 object:(__NSArrayM*)<NSArray 0x100c199d0 | 245 objects> { <NSDictionary 0x100c167c0 | 5 key/value pairs>, <NSDictionary 0x100d17970 | 5 key/value pairs>, <NSDictionary 0x100d17f40 | 5 key/value pairs>, <NSDictionary 0x100d61750 | 5 key/value pairs>, <NSDictionary 0x100c16760 | 5 key/value pairs>, ...  } >
+    171.213326 x4 received [c0]: < DTXMessage : kDTXInterruptionMessage >
+    171.213424 x4  handler [c0]: < DTXMessage : i1 kDTXInterruptionMessage >
+    171.213477 x4 received [c1f]: < DTXMessage : kDTXInterruptionMessage >
+    ```
+
+    For editing the configuration we can simply add the respected key into:
+    `/var/mobile/Library/Preferences/.GlobalPreferences.plist` and kill `cfprefsd`
+
+    The valid selectors for triggering can be found using the following Frida script the same way Troy Bowman used for
+    iterating all classes which implement the protocol `DTXAllowedRPC`:
+
+    ```shell
+    frida -U DTServiceHub
+    ```
+
+    ```javascript
+    for (var name in ObjC.protocols) {
+        var protocol = ObjC.protocols[name]
+        if ('DTXAllowedRPC' in protocol.protocols) {
+            console.log('@protocol', name)
+            console.log('  ' + Object.keys(protocol.methods).join('\n  '))
+        }
+    }
+    ```
+    """
     BROADCAST_CHANNEL = 0
     INSTRUMENTS_MESSAGE_TYPE = 2
     EXPECTS_REPLY_MASK = 0x1000
 
     def __init__(self, lockdown: LockdownClient, service_name, remove_ssl_context=True):
-        self.logger = logging.getLogger(__name__)
-        self.lockdown = lockdown
+        super().__init__(lockdown, service_name, is_developer_service=True)
 
-        self.service = self.lockdown.start_developer_service(service_name)
         if remove_ssl_context and hasattr(self.service.socket, '_sslobj'):
             self.service.socket._sslobj = None
 
         self.supported_identifiers = {}
         self.last_channel_code = 0
         self.cur_message = 0
         self.channel_cache = {}
@@ -266,15 +313,15 @@
         if data is not None:
             try:
                 data = archiver.unarchive(data)
             except archiver.MissingClassMapping as e:
                 pprint(plistlib.loads(data))
                 raise e
             except plistlib.InvalidFileException:
-                logging.warning(f'got an invalid plist: {data[:40]}')
+                self.logger.warning(f'got an invalid plist: {data[:40]}')
         return data, aux
 
     def recv_message(self, channel: int = BROADCAST_CHANNEL):
         packet_stream = self._recv_packet_fragments(channel)
         pheader = dtx_message_payload_header_struct.parse_stream(packet_stream)
 
         compression = (pheader.flags & 0xFF000) >> 12
@@ -318,34 +365,31 @@
 
                 self.channel_messages[received_channel_code].add_fragment(mheader, self.service.recvall(mheader.length))
 
     def __enter__(self):
         self.perform_handshake()
         return self
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        pass
-
 
 class Tap:
-    def __init__(self, dvt, channel_name: str, config: dict):
+    def __init__(self, dvt, channel_name: str, config: typing.Mapping):
         self._dvt = dvt
         self._channel_name = channel_name
-        self._channel = None
         self._config = config
+        self.channel = None
 
     def __enter__(self):
-        self._channel = self._dvt.make_channel(self._channel_name)
-        self._channel.setConfig_(MessageAux().append_obj(self._config), expects_reply=False)
-        self._channel.start(expects_reply=False)
+        self.channel = self._dvt.make_channel(self._channel_name)
+        self.channel.setConfig_(MessageAux().append_obj(self._config), expects_reply=False)
+        self.channel.start(expects_reply=False)
 
         # first message is just kind of an ack
-        self._channel.receive_plist()
+        self.channel.receive_plist()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        self._channel.stop(expects_reply=False)
+        self.channel.stop(expects_reply=False)
 
     def __iter__(self):
         while True:
-            for result in self._channel.receive_plist():
+            for result in self.channel.receive_plist():
                 yield result
```

### Comparing `pymobiledevice3-1.9.9/pymobiledevice3/services/springboard.py` & `pymobiledevice3-2.0.0/pymobiledevice3/services/springboard.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,45 @@
-import logging
+import typing
 from enum import IntEnum
 
 from pymobiledevice3.lockdown import LockdownClient
+from pymobiledevice3.services.base_service import BaseService
 
 
 class InterfaceOrientation(IntEnum):
     PORTRAIT = 1
     PORTRAIT_UPSIDE_DOWN = 2
     LANDSCAPE = 3
     LANDSCAPE_HOME_TO_LEFT = 4
 
 
-class SpringBoardServicesService(object):
+class SpringBoardServicesService(BaseService):
     SERVICE_NAME = 'com.apple.springboardservices'
 
     def __init__(self, lockdown: LockdownClient):
-        self.logger = logging.getLogger(__name__)
-        self.lockdown = lockdown
-        self.service = self.lockdown.start_service(self.SERVICE_NAME)
+        super().__init__(lockdown, self.SERVICE_NAME)
 
-    def get_icon_state(self, format_version='2'):
+    def get_icon_state(self, format_version: str = '2'):
         cmd = {'command': 'getIconState'}
         if format_version:
             cmd['formatVersion'] = format_version
 
         return self.service.send_recv_plist(cmd)
 
-    def set_icon_state(self, newstate=None):
+    def set_icon_state(self, newstate: typing.Mapping = None):
         if newstate is None:
             newstate = {}
         cmd = {'command': 'setIconState',
                'iconState': newstate}
 
         self.service.send_recv_plist(cmd)
 
-    def get_icon_pngdata(self, bid):
+    def get_icon_pngdata(self, bundle_id: str):
         cmd = {'command': 'getIconPNGData',
-               'bundleId': bid}
+               'bundleId': bundle_id}
 
         return self.service.send_recv_plist(cmd).get('pngData')
 
     def get_interface_orientation(self):
         cmd = {'command': 'getInterfaceOrientation'}
         self.service.send_plist(cmd)
         res = self.service.recv_plist()
```

