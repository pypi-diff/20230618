# Comparing `tmp/aiovantage-0.2.0.tar.gz` & `tmp/aiovantage-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiovantage-0.2.0.tar", last modified: Sat Jun 17 06:34:47 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `aiovantage-0.2.0.tar` & `aiovantage-0.2.1.tar`

### file list

```diff
@@ -1,161 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.867621 aiovantage-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.843620 aiovantage-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.847620 aiovantage-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-17 06:34:36.000000 aiovantage-0.2.0/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-17 06:34:36.000000 aiovantage-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-17 06:34:36.000000 aiovantage-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-17 06:34:47.867621 aiovantage-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-17 06:34:36.000000 aiovantage-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.847620 aiovantage-0.2.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.847620 aiovantage-0.2.0/examples/areas/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/areas/dump_areas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.847620 aiovantage-0.2.0/examples/blind_groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/blind_groups/dump_blind_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.847620 aiovantage-0.2.0/examples/blinds/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/blinds/dump_blinds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/blinds/monitor_blinds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.847620 aiovantage-0.2.0/examples/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/buttons/dump_buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/buttons/monitor_buttons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.847620 aiovantage-0.2.0/examples/command_client/
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/command_client/event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/command_client/status_load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.851620 aiovantage-0.2.0/examples/config_client/
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/config_client/dump_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/config_client/get_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.851620 aiovantage-0.2.0/examples/dry_contacts/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/dry_contacts/dump_dry_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/dry_contacts/monitor_dry_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/dump_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.851620 aiovantage-0.2.0/examples/gmem/
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/gmem/dump_gmem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/gmem/monitor_gmem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/gmem/set_gmem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.851620 aiovantage-0.2.0/examples/load_groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/load_groups/dump_load_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.851620 aiovantage-0.2.0/examples/loads/
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/loads/control_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/loads/dump_loads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/loads/monitor_loads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/loads/poll_on_loads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/loads/toggle_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/monitor_all.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.851620 aiovantage-0.2.0/examples/omni_sensors/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/omni_sensors/dump_omni_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/omni_sensors/monitor_omni_sensors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.851620 aiovantage-0.2.0/examples/rgb_loads/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/rgb_loads/dump_rgb_loads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/rgb_loads/monitor_rgb_loads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.851620 aiovantage-0.2.0/examples/stations/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/stations/dump_stations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.851620 aiovantage-0.2.0/examples/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/tasks/dump_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/tasks/run_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-17 06:34:36.000000 aiovantage-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 06:34:47.867621 aiovantage-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.847620 aiovantage-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.851620 aiovantage-0.2.0/src/aiovantage/
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.855621 aiovantage-0.2.0/src/aiovantage/command_client/
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    30612 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.855621 aiovantage-0.2.0/src/aiovantage/command_client/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/interfaces/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/interfaces/blind.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/interfaces/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/interfaces/color_temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/interfaces/gmem.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/interfaces/introspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/interfaces/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/interfaces/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/interfaces/rgb_load.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/interfaces/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/interfaces/task.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/ssl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.855621 aiovantage-0.2.0/src/aiovantage/config_client/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.855621 aiovantage-0.2.0/src/aiovantage/config_client/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/methods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.859621 aiovantage-0.2.0/src/aiovantage/config_client/methods/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/methods/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/methods/configuration/close_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/methods/configuration/get_filter_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/methods/configuration/get_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/methods/configuration/object_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/methods/configuration/open_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.859621 aiovantage-0.2.0/src/aiovantage/config_client/methods/introspection/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/methods/introspection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/methods/introspection/get_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.859621 aiovantage-0.2.0/src/aiovantage/config_client/methods/login/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/methods/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/methods/login/login.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.863621 aiovantage-0.2.0/src/aiovantage/config_client/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/anemo_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/area.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/blind.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/blind_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/button.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/dc_power_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/ddg_color_load.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/dg_color_load.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/dimmer.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/dry_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/dual_relay_station.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/eq_ctrl.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/eq_ux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/gmem.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/keypad.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/light_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/load.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/load_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/location_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/master.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/omni_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/power_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/pwm_power_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/qis_blind.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/qube_blind.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/relay_blind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/rgb_load.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/scene_point_relay.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/station_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/station_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/system_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/task.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/urtsi_2_group_child.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/urtsi_2_shade_child.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/xml_dataclass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.867621 aiovantage-0.2.0/src/aiovantage/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/areas.py
--rw-r--r--   0 runner    (1001) docker     (123)    10048 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/blind_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/blinds.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/dry_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/gmem.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/load_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/loads.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/masters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/omni_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/rgb_loads.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/stations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.851620 aiovantage-0.2.0/src/aiovantage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-17 06:34:47.000000 aiovantage-0.2.0/src/aiovantage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-17 06:34:47.000000 aiovantage-0.2.0/src/aiovantage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 06:34:47.000000 aiovantage-0.2.0/src/aiovantage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-17 06:34:47.000000 aiovantage-0.2.0/src/aiovantage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-17 06:34:47.000000 aiovantage-0.2.0/src/aiovantage.egg-info/top_level.txt
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aiovantage-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 aiovantage-0.2.1/TODO
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 aiovantage-0.2.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 aiovantage-0.2.1/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 aiovantage-0.2.1/.vscode/settings.json
+-rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/dump_system.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/monitor_all.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/areas/dump_areas.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/blind_groups/dump_blind_groups.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/blinds/dump_blinds.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/blinds/monitor_blinds.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/buttons/dump_buttons.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/buttons/monitor_buttons.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/command_client/event_log.py
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/command_client/status_load.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/config_client/dump_objects.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/config_client/get_version.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/dry_contacts/dump_dry_contacts.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/dry_contacts/monitor_dry_contacts.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/gmem/dump_gmem.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/gmem/monitor_gmem.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/gmem/set_gmem.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/load_groups/dump_load_groups.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/loads/control_load.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/loads/dump_loads.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/loads/monitor_loads.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/loads/poll_on_loads.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/loads/toggle_load.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/omni_sensors/dump_omni_sensors.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/omni_sensors/monitor_omni_sensors.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/rgb_loads/dump_rgb_loads.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/rgb_loads/monitor_rgb_loads.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/stations/dump_stations.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/tasks/dump_tasks.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/tasks/run_task.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/__about__.py
+-rw-r--r--   0        0        0     7158 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/__init__.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/events.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/py.typed
+-rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/query.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/README.md
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/__init__.py
+-rw-r--r--   0        0        0    18949 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/client.py
+-rw-r--r--   0        0        0    10260 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/connection.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/errors.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/events.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/response.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/utils.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/interfaces/__init__.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/interfaces/base.py
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/interfaces/blind.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/interfaces/button.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/interfaces/color_temperature.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/interfaces/gmem.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/interfaces/introspection.py
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/interfaces/load.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/interfaces/object.py
+-rw-r--r--   0        0        0     8960 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/interfaces/rgb_load.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/interfaces/sensor.py
+-rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/interfaces/task.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/README.md
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/__init__.py
+-rw-r--r--   0        0        0     8118 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/client.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/errors.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/helpers.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/xml_dataclass.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/methods/__init__.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/methods/types.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/methods/configuration/__init__.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/methods/configuration/close_filter.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/methods/configuration/get_filter_results.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/methods/configuration/get_object.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/methods/configuration/open_filter.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/methods/introspection/__init__.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/methods/introspection/get_version.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/methods/login/__init__.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/methods/login/login.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/__init__.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/anemo_sensor.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/area.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/blind.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/blind_group.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/button.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/dc_power_profile.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/ddg_color_load.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/dg_color_load.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/dimmer.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/dry_contact.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/dual_relay_station.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/eq_ctrl.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/eq_ux.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/gmem.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/keypad.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/light_sensor.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/load.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/load_group.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/location_object.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/master.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/omni_sensor.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/power_profile.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/pwm_power_profile.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/qis_blind.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/qube_blind.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/relay_blind.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/rgb_load.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/scene_point_relay.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/sensor.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/station_bus.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/station_object.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/system_object.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/task.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/temperature.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/urtsi_2_group.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/urtsi_2_shade.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/__init__.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/areas.py
+-rw-r--r--   0        0        0    10205 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/base.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/blind_groups.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/blinds.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/buttons.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/dry_contacts.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/gmem.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/load_groups.py
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/loads.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/masters.py
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/omni_sensors.py
+-rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/rgb_loads.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/stations.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/tasks.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 aiovantage-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 aiovantage-0.2.1/README.md
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 aiovantage-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 aiovantage-0.2.1/PKG-INFO
```

### Comparing `aiovantage-0.2.0/LICENSE` & `aiovantage-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.0/PKG-INFO` & `aiovantage-0.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: aiovantage
-Version: 0.2.0
-Summary: Python module to talk to Vantage InFusion controllers.
+Version: 0.2.1
+Summary: Interact with and control Vantage InFusion home automation controllers.
+Project-URL: Documentation, https://github.com/loopj/aiovantage#readme
+Project-URL: Issues, https://github.com/loopj/aiovantage/issues
+Project-URL: Source, https://github.com/loopj/aiovantage
 Author-email: James Smith <james@loopj.com>
-License: MIT
+License-Expression: MIT
+License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
+Requires-Dist: typing-extensions<5.0,>=4.6.3
+Requires-Dist: xsdata==23.5
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # aiovantage
 
 aiovantage is a Python library for interacting with and controlling Vantage InFusion home automation controllers.
 
 Uses a "controller" pattern inspired heavily by the [aiohue](https://github.com/home-assistant-libs/aiohue) library.
 
@@ -43,30 +48,30 @@
 - Alternatively, eager-fetch objects with `controller.initialize`.
 
 
 ## Supported objects types
 
 The following interfaces/controllers are currently supported.
 
-| Type          | Description           | Controller                | Examples
-| ------------- | --------------------- | ------------------------- | --------
-| Area          | Rooms, etc            | `vantage.areas`           | [Examples](examples/areas)
-| Blind         | Shades, blinds        | `vantage.blinds`          | [Examples](examples/blinds)
-| BlindGroups   | Groups of blinds      | `vantage.blind_groups`    | [Examples](examples/blind_groups)
-| Buttons       | Keypad buttons        | `vantage.buttons`         | [Examples](examples/buttons)
-| DryContacts   | Motion sensors, etc   | `vantage.dry_contacts`    | [Examples](examples/dry_contacts)
-| GMem          | Vantage variables     | `vantage.gmem`            | [Examples](examples/gmem)
-| Load          | Lights, relays, etc   | `vantage.loads`           | [Examples](examples/loads)
-| LoadGroup     | Groups of loads       | `vantage.load_groups`     | [Examples](examples/load_groups)
-| OmniSensor    | Power, current, etc   | `vantage.omni_sensors`    | [Examples](examples/omni_sensors)
-| RGBLoad       | RGB lights            | `vantage.rgb_loads`       | [Examples](examples/rgb_loads)
-| Stations      | Keypads, etc          | `vantage.stations`        | [Examples](examples/stations)
-| Tasks         | Vantage tasks         | `vantage.tasks`           | [Examples](examples/tasks)
+| Type          | Description           | Controller                | Examples                          |
+| ------------- | --------------------- | ------------------------- | --------------------------------- |
+| Area          | Rooms, etc            | `vantage.areas`           | [Examples](examples/areas)        |
+| Blind         | Shades, blinds        | `vantage.blinds`          | [Examples](examples/blinds)       |
+| BlindGroups   | Groups of blinds      | `vantage.blind_groups`    | [Examples](examples/blind_groups) |
+| Buttons       | Keypad buttons        | `vantage.buttons`         | [Examples](examples/buttons)      |
+| DryContacts   | Motion sensors, etc   | `vantage.dry_contacts`    | [Examples](examples/dry_contacts) |
+| GMem          | Vantage variables     | `vantage.gmem`            | [Examples](examples/gmem)         |
+| Load          | Lights, relays, etc   | `vantage.loads`           | [Examples](examples/loads)        |
+| LoadGroup     | Groups of loads       | `vantage.load_groups`     | [Examples](examples/load_groups)  |
+| OmniSensor    | Power, current, etc   | `vantage.omni_sensors`    | [Examples](examples/omni_sensors) |
+| RGBLoad       | RGB lights            | `vantage.rgb_loads`       | [Examples](examples/rgb_loads)    |
+| Stations      | Keypads, etc          | `vantage.stations`        | [Examples](examples/stations)     |
+| Tasks         | Vantage tasks         | `vantage.tasks`           | [Examples](examples/tasks)        |
 
 If you have an object that you expect to show up in one of these controllers, but it is missing, please let me know in an issue.
 
 
 ## Installation
 
 ```shell
 pip3 install aiovantage
-```
+```
```

### Comparing `aiovantage-0.2.0/README.md` & `aiovantage-0.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -28,28 +28,28 @@
 - Alternatively, eager-fetch objects with `controller.initialize`.
 
 
 ## Supported objects types
 
 The following interfaces/controllers are currently supported.
 
-| Type          | Description           | Controller                | Examples
-| ------------- | --------------------- | ------------------------- | --------
-| Area          | Rooms, etc            | `vantage.areas`           | [Examples](examples/areas)
-| Blind         | Shades, blinds        | `vantage.blinds`          | [Examples](examples/blinds)
-| BlindGroups   | Groups of blinds      | `vantage.blind_groups`    | [Examples](examples/blind_groups)
-| Buttons       | Keypad buttons        | `vantage.buttons`         | [Examples](examples/buttons)
-| DryContacts   | Motion sensors, etc   | `vantage.dry_contacts`    | [Examples](examples/dry_contacts)
-| GMem          | Vantage variables     | `vantage.gmem`            | [Examples](examples/gmem)
-| Load          | Lights, relays, etc   | `vantage.loads`           | [Examples](examples/loads)
-| LoadGroup     | Groups of loads       | `vantage.load_groups`     | [Examples](examples/load_groups)
-| OmniSensor    | Power, current, etc   | `vantage.omni_sensors`    | [Examples](examples/omni_sensors)
-| RGBLoad       | RGB lights            | `vantage.rgb_loads`       | [Examples](examples/rgb_loads)
-| Stations      | Keypads, etc          | `vantage.stations`        | [Examples](examples/stations)
-| Tasks         | Vantage tasks         | `vantage.tasks`           | [Examples](examples/tasks)
+| Type          | Description           | Controller                | Examples                          |
+| ------------- | --------------------- | ------------------------- | --------------------------------- |
+| Area          | Rooms, etc            | `vantage.areas`           | [Examples](examples/areas)        |
+| Blind         | Shades, blinds        | `vantage.blinds`          | [Examples](examples/blinds)       |
+| BlindGroups   | Groups of blinds      | `vantage.blind_groups`    | [Examples](examples/blind_groups) |
+| Buttons       | Keypad buttons        | `vantage.buttons`         | [Examples](examples/buttons)      |
+| DryContacts   | Motion sensors, etc   | `vantage.dry_contacts`    | [Examples](examples/dry_contacts) |
+| GMem          | Vantage variables     | `vantage.gmem`            | [Examples](examples/gmem)         |
+| Load          | Lights, relays, etc   | `vantage.loads`           | [Examples](examples/loads)        |
+| LoadGroup     | Groups of loads       | `vantage.load_groups`     | [Examples](examples/load_groups)  |
+| OmniSensor    | Power, current, etc   | `vantage.omni_sensors`    | [Examples](examples/omni_sensors) |
+| RGBLoad       | RGB lights            | `vantage.rgb_loads`       | [Examples](examples/rgb_loads)    |
+| Stations      | Keypads, etc          | `vantage.stations`        | [Examples](examples/stations)     |
+| Tasks         | Vantage tasks         | `vantage.tasks`           | [Examples](examples/tasks)        |
 
 If you have an object that you expect to show up in one of these controllers, but it is missing, please let me know in an issue.
 
 
 ## Installation
 
 ```shell
```

### Comparing `aiovantage-0.2.0/examples/areas/dump_areas.py` & `aiovantage-0.2.1/examples/areas/dump_areas.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-"""
-Prints out the id and name of each area in the Vantage controller.
-"""
+"""Prints out the id and name of each area in the Vantage controller."""
 
 import argparse
 import asyncio
+import contextlib
 import logging
 
 from aiovantage import Vantage
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
 async def main() -> None:
+    """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
     # Connect to the Vantage controller and print out the name and level of each load
     async with Vantage(args.host, args.username, args.password) as vantage:
         async for area in vantage.areas:
             print(f"[{area.id}] '{area.name}'")
 
 
-try:
+with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
-except KeyboardInterrupt:
-    pass
```

### Comparing `aiovantage-0.2.0/examples/blind_groups/dump_blind_groups.py` & `aiovantage-0.2.1/examples/tasks/dump_tasks.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-"""
-Prints out the id, name, and members of each blind group in the Vantage controller.
-"""
+"""Prints out the id, name, and running state of each task in the Vantage controller."""
 
 import argparse
 import asyncio
+import contextlib
 import logging
 
 from aiovantage import Vantage
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
 async def main() -> None:
+    """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
-    # Connect to the Vantage controller and print out details of each blind group
+    # Connect to the Vantage controller and print out the name and value of each GMem
     async with Vantage(args.host, args.username, args.password) as vantage:
-        async for blind_group in vantage.blind_groups:
-            print(f"[{blind_group.id}] '{blind_group.name}' {blind_group.blind_ids}")
+        async for task in vantage.tasks:
+            print(f"[{task.id}] '{task.name}' is_running={task.is_running}")
 
 
-try:
+with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
-except KeyboardInterrupt:
-    pass
```

### Comparing `aiovantage-0.2.0/examples/blinds/dump_blinds.py` & `aiovantage-0.2.1/examples/dry_contacts/dump_dry_contacts.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-"""
-Prints out the id and name of each blind in the Vantage controller.
-"""
+"""Prints out the id and name of each dry contact in the Vantage controller."""
 
 import argparse
 import asyncio
+import contextlib
 import logging
 
 from aiovantage import Vantage
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
 async def main() -> None:
+    """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
-    # Connect to the Vantage controller and print out the name and level of each load
+    # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
-        async for blind in vantage.blinds:
-            print(f"[{blind.id}] '{blind.name}'")
+        # Print some details about each dry contact
+        async for dry_contact in vantage.dry_contacts:
+            print(f"[{dry_contact.id}] name='{dry_contact.name}' ")
 
 
-try:
+with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
-except KeyboardInterrupt:
-    pass
```

### Comparing `aiovantage-0.2.0/examples/blinds/monitor_blinds.py` & `aiovantage-0.2.1/examples/blind_groups/dump_blind_groups.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,33 @@
-"""
-Fetch all blinds from the Vantage controller, and print out any state changes.
-"""
+"""Prints out the id, name and members of each blind group in the Vantage controller."""
 
 import argparse
 import asyncio
+import contextlib
 import logging
-from typing import Any, Dict
 
-from aiovantage import Vantage, VantageEvent
-from aiovantage.config_client.objects import SystemObject
+from aiovantage import Vantage
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
-def callback(event: VantageEvent, obj: SystemObject, data: Dict[str, Any]) -> None:
-    if event == VantageEvent.OBJECT_ADDED:
-        print(f"[Blind added] '{obj.name}' ({obj.id})")
-
-    elif event == VantageEvent.OBJECT_UPDATED:
-        print(f"[Blind updated] '{obj.name}' ({obj.id})")
-        for attr in data.get("attrs_changed", []):
-            print(f"    {attr} = {getattr(obj, attr)}")
-
-
 async def main() -> None:
+    """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
+    # Connect to the Vantage controller and print out details of each blind group
     async with Vantage(args.host, args.username, args.password) as vantage:
-        # Subscribe to updates for all loads
-        vantage.blinds.subscribe(callback)
-
-        # Fetch all known loads from the controller
-        await vantage.blinds.initialize()
-
-        # Keep running for a while
-        await asyncio.sleep(3600)
+        async for blind_group in vantage.blind_groups:
+            print(f"[{blind_group.id}] '{blind_group.name}'")
+            async for blind in vantage.blind_groups.blinds(blind_group.id):
+                print(f"    [{blind.id}] '{blind.name}'")
 
 
-try:
+with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
-except KeyboardInterrupt:
-    pass
```

### Comparing `aiovantage-0.2.0/examples/buttons/dump_buttons.py` & `aiovantage-0.2.1/examples/buttons/dump_buttons.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-"""
-Prints out the id, name, and labels of each button in the Vantage controller.
-"""
+"""Prints out the id, name, and labels of each button in the Vantage controller."""
 
 import argparse
 import asyncio
+import contextlib
 import logging
 
 from aiovantage import Vantage
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
 async def main() -> None:
+    """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
     # Connect to the Vantage controller and print out the name and level of each load
     async with Vantage(args.host, args.username, args.password) as vantage:
         async for button in vantage.buttons:
             print(
                 f"[{button.id}] name='{button.name}' "
                 f"text1='{button.text1}' text2='{button.text2}'"
             )
 
 
-try:
+with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
-except KeyboardInterrupt:
-    pass
```

### Comparing `aiovantage-0.2.0/examples/buttons/monitor_buttons.py` & `aiovantage-0.2.1/examples/load_groups/dump_load_groups.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,32 @@
-"""
-Fetch all buttons from the Vantage controller, and print out any state changes.
-"""
+"""Prints out the id, name, and members of each load group in the Vantage controller."""
 
 import argparse
 import asyncio
+import contextlib
 import logging
-from typing import Any, Dict
 
-from aiovantage import Vantage, VantageEvent
-from aiovantage.config_client.objects import Button
+from aiovantage import Vantage
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
-def callback(event: VantageEvent, obj: Button, data: Dict[str, Any]) -> None:
-    if event == VantageEvent.OBJECT_ADDED:
-        print(f"[Button added] '{obj.name}' ({obj.id})")
-
-    elif event == VantageEvent.OBJECT_UPDATED:
-        print(f"[Button updated] '{obj.name}' ({obj.id})")
-        for attr in data.get("attrs_changed", []):
-            print(f"    {attr} = {getattr(obj, attr)}")
-
-
 async def main() -> None:
+    """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
+    # Connect to the Vantage controller and print out the name and level of each load
     async with Vantage(args.host, args.username, args.password) as vantage:
-        # Subscribe to updates for all buttons
-        vantage.buttons.subscribe(callback)
-
-        # Fetch all known loads from the controller
-        await vantage.buttons.initialize()
-
-        # Keep running for a while
-        await asyncio.sleep(3600)
+        async for load_group in vantage.load_groups:
+            print(load_group)
+            print(f"[{load_group.id}] '{load_group.name}' {load_group.load_ids}")
 
 
-try:
+with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
-except KeyboardInterrupt:
-    pass
```

### Comparing `aiovantage-0.2.0/examples/command_client/event_log.py` & `aiovantage-0.2.1/examples/stations/dump_stations.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,30 @@
+"""Prints out the id and name of each station in the Vantage controller."""
+
 import argparse
 import asyncio
+import contextlib
 import logging
 
-from aiovantage.command_client import CommandClient, Event, EventType
+from aiovantage import Vantage
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
-# Define callback function for Host Command events
-def command_client_callback(event: Event) -> None:
-    if event["tag"] == EventType.EVENT_LOG:
-        print(event["log"])
-    elif event["tag"] == EventType.CONNECTED:
-        print("Connected and monitoring for log events...")
-
-
 async def main() -> None:
+    """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
-    # Create a Host Command client
-    async with CommandClient(args.host, args.username, args.password) as client:
-        # Subscribe to connection events
-        client.subscribe(command_client_callback, EventType.CONNECTED)
-
-        # Subscribe to system log events
-        await client.subscribe_event_log(command_client_callback, "SYSTEM")
-
-        # Keep running for a while
-        await asyncio.sleep(3600)
+    async with Vantage(args.host, args.username, args.password) as vantage:
+        async for station in vantage.stations:
+            print(f"[{station.id}] '{station.name}'")
 
 
-try:
+with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
-except KeyboardInterrupt:
-    pass
```

### Comparing `aiovantage-0.2.0/examples/command_client/status_load.py` & `aiovantage-0.2.1/examples/command_client/status_load.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,39 @@
+"""Use a CommandClient to subscribe to status updates for LOAD objects."""
+
 import argparse
 import asyncio
+import contextlib
 import logging
 
 from aiovantage.command_client import CommandClient, Event, EventType
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
-# Define callback function for command client events
 def command_client_callback(event: Event) -> None:
+    """Print out the status update for each event."""
     if event["tag"] == EventType.STATUS:
         print(f"[{event['status_type']}] id: {event['id']}, args: {event['args']}")
     elif event["tag"] == EventType.CONNECTED:
         print("Connected and monitoring for status updates...")
     elif event["tag"] == EventType.DISCONNECTED:
         print("Disconnected")
     elif event["tag"] == EventType.RECONNECTED:
         print("Reconnected")
 
 
 async def main() -> None:
+    """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
     # Create a Host Command client
     async with CommandClient(args.host, args.username, args.password) as client:
         # Subscribe to connection events
         client.subscribe(
@@ -40,11 +44,9 @@
         # Subscribe to status updates for LOAD objects (STATUS LOAD)
         await client.subscribe_status(command_client_callback, "LOAD")
 
         # Keep running for a while
         await asyncio.sleep(3600)
 
 
-try:
+with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
-except KeyboardInterrupt:
-    pass
```

### Comparing `aiovantage-0.2.0/examples/config_client/dump_objects.py` & `aiovantage-0.2.1/examples/config_client/dump_objects.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,46 @@
+"""Example of using the get_objects helper to dump all objects of a given type."""
+
 import argparse
 import asyncio
+import contextlib
 import logging
 
 from aiovantage.config_client import ConfigClient
 from aiovantage.config_client.helpers import get_objects
 
-
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
 async def main() -> None:
+    """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
     async with ConfigClient(args.host, args.username, args.password) as client:
         # Dump all Areas using the get_objects helper
         print("# Vantage Areas")
-        async for area in get_objects(client, type="Area"):
+        async for area in get_objects(client, types="Area"):
             print(area)
         print()
 
         # Dump all Loads using the get_objects helper
         print("# Vantage Loads")
-        async for load in get_objects(client, type="Load"):
+        async for load in get_objects(client, types="Load"):
             print(load)
         print()
 
         # Dump some StationObjects using the get_objects helper
         print("# Vantage Stations")
-        async for station in get_objects(client, type=("Keypad", "EqCtrl")):
+        async for station in get_objects(client, types=("Keypad", "EqCtrl")):
             print(station)
         print()
 
 
-try:
+with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
-except KeyboardInterrupt:
-    pass
```

### Comparing `aiovantage-0.2.0/examples/config_client/get_version.py` & `aiovantage-0.2.1/examples/config_client/get_version.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,31 @@
+"""Example of using the ConfigClient to get the Vantage version."""
 import argparse
 import asyncio
+import contextlib
 import logging
 
 from aiovantage.config_client import ConfigClient
 from aiovantage.config_client.methods.introspection import GetVersion
 
-
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
 async def main() -> None:
+    """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
     async with ConfigClient(args.host, args.username, args.password) as client:
         # Simple RPC request without any params (IIntrospection.GetVersion)
         version = await client.request(GetVersion)
         print(version)
 
 
-try:
+with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
-except KeyboardInterrupt:
-    pass
```

### Comparing `aiovantage-0.2.0/examples/dry_contacts/dump_dry_contacts.py` & `aiovantage-0.2.1/examples/gmem/dump_gmem.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,31 @@
-"""
-Prints out the id and name of each dry contact in the Vantage controller.
-"""
+"""Prints out the id, name, and value of each variable in the Vantage controller."""
 
 import argparse
 import asyncio
+import contextlib
 import logging
 
 from aiovantage import Vantage
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
 async def main() -> None:
+    """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
-    # Connect to the Vantage controller
+    # Connect to the Vantage controller and print out the name and value of each GMem
     async with Vantage(args.host, args.username, args.password) as vantage:
-        # Print some details about each dry contact
-        async for dry_contact in vantage.dry_contacts:
-            print(f"[{dry_contact.id}] name='{dry_contact.name}' ")
+        async for gmem in vantage.gmem:
+            print(f"[{gmem.id}] '{gmem.name}' = {repr(gmem.value)}")
 
 
-try:
+with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
-except KeyboardInterrupt:
-    pass
```

### Comparing `aiovantage-0.2.0/examples/dry_contacts/monitor_dry_contacts.py` & `aiovantage-0.2.1/examples/dry_contacts/monitor_dry_contacts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-"""
-Fetch all dry contacts from the Vantage controller, and print out any state changes.
-"""
+"""Fetch all dry contacts from the Vantage controller, and print any state changes."""
 
 import argparse
 import asyncio
+import contextlib
 import logging
 from typing import Any, Dict
 
 from aiovantage import Vantage, VantageEvent
 from aiovantage.config_client.objects import DryContact
 
 # Grab connection info from command line arguments
@@ -16,35 +15,35 @@
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
 def callback(event: VantageEvent, obj: DryContact, data: Dict[str, Any]) -> None:
+    """Print out any state changes."""
     if event == VantageEvent.OBJECT_ADDED:
         print(f"[DryContact added] '{obj.name}' ({obj.id})")
 
     elif event == VantageEvent.OBJECT_UPDATED:
         print(f"[DryContact updated] '{obj.name}' ({obj.id})")
         for attr in data.get("attrs_changed", []):
             print(f"    {attr} = {getattr(obj, attr)}")
 
 
 async def main() -> None:
+    """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
     async with Vantage(args.host, args.username, args.password) as vantage:
         # Subscribe to updates for all buttons
         vantage.dry_contacts.subscribe(callback)
 
         # Fetch all known loads from the controller
         await vantage.dry_contacts.initialize()
 
         # Keep running for a while
         await asyncio.sleep(3600)
 
 
-try:
+with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
-except KeyboardInterrupt:
-    pass
```

### Comparing `aiovantage-0.2.0/examples/dump_system.py` & `aiovantage-0.2.1/examples/dump_system.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-"""
-Print a tree of all the areas, loads, stations, and dry contacts in the
-Vantage system.
-"""
+"""Print a tree of objects in the Vantage system."""
 
 import argparse
 import asyncio
+import contextlib
 import logging
 from typing import Optional
 
 from aiovantage import Vantage
 from aiovantage.config_client.objects import Area, Load
 
-
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
@@ -26,32 +23,36 @@
 RED = "\033[31m"
 GREEN = "\033[32m"
 YELLOW = "\033[33m"
 CYAN = "\033[36m"
 
 
 def colorize(text: str, color: str) -> str:
+    """Return text wrapped in the given ANSI color code."""
     return f"{color}{text}{RESET}"
 
 
 def print_indented(text: str, indent_level: int) -> None:
+    """Print text indented by the given number of levels."""
     indent = indent_level * "    "
     print(f"{indent}{text}")
 
 
 def load_state(load: Load) -> str:
+    """Return a string describing the state of a load."""
     if not load.level:
         return colorize("(OFF)", RED)
     elif load.level == 100:
         return colorize("(ON)", GREEN)
     else:
         return colorize(f"({load.level}%)", GREEN)
 
 
 def print_area(vantage: Vantage, area: Optional[Area], indent: int = 0) -> None:
+    """Recursively print an area and all its children."""
     if area is None:
         return
 
     # Print the area name
     print_indented(colorize(area.name, CYAN), indent)
 
     # Print loads in this area, if any
@@ -90,23 +91,22 @@
     child_areas = vantage.areas.filter(area_id=area.id)
     if child_areas:
         for child_area in child_areas:
             print_area(vantage, child_area, indent + 1)
 
 
 async def main() -> None:
+    """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
     # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
         # Preload all the objects we want to dump
         await vantage.initialize()
 
         # Recursively print the root area and all its children
         print_area(vantage, vantage.areas.root)
 
 
-try:
+with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
-except KeyboardInterrupt:
-    pass
```

### Comparing `aiovantage-0.2.0/examples/gmem/dump_gmem.py` & `aiovantage-0.2.1/examples/blinds/dump_blinds.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-"""
-Prints out the id, name, and value of each variable in the Vantage controller.
-"""
+"""Prints out the id and name of each blind in the Vantage controller."""
 
 import argparse
 import asyncio
+import contextlib
 import logging
 
 from aiovantage import Vantage
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
 async def main() -> None:
+    """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
-    # Connect to the Vantage controller and print out the name and value of each GMem
+    # Connect to the Vantage controller and print out the name and level of each load
     async with Vantage(args.host, args.username, args.password) as vantage:
-        async for gmem in vantage.gmem:
-            print(f"[{gmem.id}] '{gmem.name}' = {repr(gmem.value)}")
+        async for blind in vantage.blinds:
+            print(f"[{blind.id}] '{blind.name}'")
 
 
-try:
+with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
-except KeyboardInterrupt:
-    pass
```

### Comparing `aiovantage-0.2.0/examples/gmem/monitor_gmem.py` & `aiovantage-0.2.1/examples/blinds/monitor_blinds.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,49 @@
-"""
-Fetch all variables from the Vantage controller, and print out any state changes.
-"""
+"""Fetch all blinds from the Vantage controller, and print out any state changes."""
 
 import argparse
 import asyncio
+import contextlib
 import logging
 from typing import Any, Dict
 
 from aiovantage import Vantage, VantageEvent
-from aiovantage.config_client.objects import GMem
+from aiovantage.config_client.objects import SystemObject
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
-def callback(event: VantageEvent, obj: GMem, data: Dict[str, Any]) -> None:
+def callback(event: VantageEvent, obj: SystemObject, data: Dict[str, Any]) -> None:
+    """Print out any state changes."""
     if event == VantageEvent.OBJECT_ADDED:
-        print(f"[GMem added] '{obj.name}' ({obj.id})")
+        print(f"[Blind added] '{obj.name}' ({obj.id})")
 
     elif event == VantageEvent.OBJECT_UPDATED:
-        print(f"[GMem updated] '{obj.name}' ({obj.id})")
+        print(f"[Blind updated] '{obj.name}' ({obj.id})")
         for attr in data.get("attrs_changed", []):
-            print(f"    {attr} = {repr(getattr(obj, attr))}")
+            print(f"    {attr} = {getattr(obj, attr)}")
 
 
 async def main() -> None:
+    """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
     async with Vantage(args.host, args.username, args.password) as vantage:
-        # Subscribe to updates for all GMem objects
-        vantage.gmem.subscribe(callback)
+        # Subscribe to updates for all loads
+        vantage.blinds.subscribe(callback)
 
-        # Fetch all known GMem objects from the controller
-        await vantage.gmem.initialize()
+        # Fetch all known loads from the controller
+        await vantage.blinds.initialize()
 
         # Keep running for a while
         await asyncio.sleep(3600)
 
 
-try:
+with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
-except KeyboardInterrupt:
-    pass
```

### Comparing `aiovantage-0.2.0/examples/gmem/set_gmem.py` & `aiovantage-0.2.1/examples/gmem/set_gmem.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-"""
-Set the value of a variable on the Vantage controller.
-"""
+"""Set the value of a variable on the Vantage controller."""
 
 import argparse
 import asyncio
+import contextlib
 import logging
 
 from aiovantage import Vantage
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
@@ -16,14 +15,15 @@
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
 async def main() -> None:
+    """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
     # Connect to the Vantage controller and print out the name and value of each GMem
     async with Vantage(args.host, args.username, args.password) as vantage:
         # Look up the object by id
         try:
@@ -53,11 +53,9 @@
                 return
 
         # Set the value
         print(f"Setting '{gmem.name}' (id = {gmem.id}) to '{args.value}'")
         await vantage.gmem.set_value(gmem_id, args.value)
 
 
-try:
+with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
-except KeyboardInterrupt:
-    pass
```

### Comparing `aiovantage-0.2.0/examples/load_groups/dump_load_groups.py` & `aiovantage-0.2.1/examples/loads/toggle_load.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,46 @@
-"""
-Prints out the id, name, and members of each load group in the Vantage controller.
-"""
+"""Toggle a load on or off by ID."""
 
 import argparse
 import asyncio
+import contextlib
 import logging
 
 from aiovantage import Vantage
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
+parser.add_argument("id", help="load id to toggle")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
 async def main() -> None:
+    """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
-    # Connect to the Vantage controller and print out the name and level of each load
+    # Connect to the Vantage controller and print out the name and value of each GMem
     async with Vantage(args.host, args.username, args.password) as vantage:
-        async for load_group in vantage.load_groups:
-            print(load_group)
-            print(f"[{load_group.id}] '{load_group.name}' {load_group.load_ids}")
+        try:
+            load_id = int(args.id)
+        except ValueError:
+            print("Invalid load id")
+            return
+
+        load = await vantage.loads.aget(load_id)
+        if load is None:
+            print("Load not found")
+            return
+
+        print(f"Toggling {load.name} (id = {load.id})")
+        if load.is_on:
+            await vantage.loads.turn_off(load.id)
+        else:
+            await vantage.loads.turn_on(load.id)
 
 
-try:
+with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
-except KeyboardInterrupt:
-    pass
```

### Comparing `aiovantage-0.2.0/examples/loads/control_load.py` & `aiovantage-0.2.1/examples/loads/control_load.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,56 @@
-"""
-Print a list of loads and allow the user to control them with the keyboard.
-"""
+"""Print a list of loads and allow the user to control them with the keyboard."""
 
 import argparse
 import asyncio
 import logging
 import sys
 import termios
 import tty
-from contextlib import contextmanager
+from contextlib import contextmanager, suppress
 from typing import Iterator, Optional
 
 from aiovantage import Vantage
 
-
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
 def parse_keypress() -> Optional[str]:
-    # Rudimentary keypress parser
-
-    c = sys.stdin.read(1)
-    if c == "\x1b":
+    """Rudimentary keypress parser."""
+    char = sys.stdin.read(1)
+    if char == "\x1b":
         seq = sys.stdin.read(2)
         if seq == "[A":
             return "KEY_UP"
-        elif seq == "[B":
+        if seq == "[B":
             return "KEY_DOWN"
-        else:
-            return None
-    else:
-        return c
+        return None
 
+    return char
 
-@contextmanager
-def cbreak_mode(fd: int) -> Iterator[None]:
-    # Context manager to read terminal input character by character
 
-    old_attrs = termios.tcgetattr(fd)
+@contextmanager
+def cbreak_mode(descriptor: int) -> Iterator[None]:
+    """Context manager to read terminal input character by character."""
+    old_attrs = termios.tcgetattr(descriptor)
     try:
-        tty.setcbreak(fd)
+        tty.setcbreak(descriptor)
         yield
     finally:
-        termios.tcsetattr(fd, termios.TCSADRAIN, old_attrs)
+        termios.tcsetattr(descriptor, termios.TCSADRAIN, old_attrs)
 
 
 async def main() -> None:
+    """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
     async with Vantage(args.host, args.username, args.password) as vantage:
         # Print out the available loads
         print("Load ID  Name")
         print("-------  ----")
@@ -107,11 +102,9 @@
                         await vantage.loads.turn_on(load.id)
                         print(f"Turned '{load.name}' load on")
 
                 elif key == "q":
                     break
 
 
-try:
+with suppress(KeyboardInterrupt):
     asyncio.run(main())
-except KeyboardInterrupt:
-    pass
```

### Comparing `aiovantage-0.2.0/examples/loads/dump_loads.py` & `aiovantage-0.2.1/examples/loads/dump_loads.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-"""
-Prints out the id, name, and level of each load in the Vantage controller.
-"""
+"""Prints out the id, name, and level of each load in the Vantage controller."""
 
 import argparse
 import asyncio
+import contextlib
 import logging
 
 from aiovantage import Vantage
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
 async def main() -> None:
+    """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
     # Connect to the Vantage controller and print out the name and level of each load
     async with Vantage(args.host, args.username, args.password) as vantage:
         async for load in vantage.loads:
             print(f"[{load.id}] '{load.name}' level={load.level}%")
 
 
-try:
+with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
-except KeyboardInterrupt:
-    pass
```

### Comparing `aiovantage-0.2.0/examples/loads/monitor_loads.py` & `aiovantage-0.2.1/examples/loads/monitor_loads.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-"""
-Fetch all loads from the Vantage controller, and print out any state changes.
-"""
+"""Fetch all loads from the Vantage controller, and print out any state changes."""
 
 import argparse
 import asyncio
+import contextlib
 import logging
 from typing import Any, Dict
 
 from aiovantage import Vantage, VantageEvent
 from aiovantage.config_client.objects import Load
 
 # Grab connection info from command line arguments
@@ -16,35 +15,35 @@
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
 def callback(event: VantageEvent, obj: Load, data: Dict[str, Any]) -> None:
+    """Print out any state changes."""
     if event == VantageEvent.OBJECT_ADDED:
         print(f"[Load added] '{obj.name}' ({obj.id})")
 
     elif event == VantageEvent.OBJECT_UPDATED:
         print(f"[Load updated] '{obj.name}' ({obj.id})")
         for attr in data.get("attrs_changed", []):
             print(f"    {attr} = {getattr(obj, attr)}")
 
 
 async def main() -> None:
+    """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
     async with Vantage(args.host, args.username, args.password) as vantage:
         # Subscribe to updates for all loads
         vantage.loads.subscribe(callback)
 
         # Fetch all known loads from the controller
         await vantage.loads.initialize()
 
         # Keep running for a while
         await asyncio.sleep(3600)
 
 
-try:
+with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
-except KeyboardInterrupt:
-    pass
```

### Comparing `aiovantage-0.2.0/examples/loads/poll_on_loads.py` & `aiovantage-0.2.1/examples/loads/poll_on_loads.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-"""
-Print a list of all loads that are currently on every 5 seconds.
-"""
+"""Print a list of all loads that are currently on every 5 seconds."""
 
 import argparse
 import asyncio
+import contextlib
 import logging
 
 from aiovantage import Vantage
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
 async def main() -> None:
+    """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
     async with Vantage(args.host, args.username, args.password) as vantage:
         # Preload the loads from the controller
         await vantage.loads.initialize()
 
@@ -32,11 +32,9 @@
             for load in on_loads:
                 print(f"- {load.name}")
             print()
 
             await asyncio.sleep(5)
 
 
-try:
+with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
-except KeyboardInterrupt:
-    pass
```

### Comparing `aiovantage-0.2.0/examples/monitor_all.py` & `aiovantage-0.2.1/examples/buttons/monitor_buttons.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,49 @@
-"""
-Fetch all objects from the Vantage controller, and print out any state changes.
-"""
+"""Fetch all buttons from the Vantage controller, and print out any state changes."""
 
 import argparse
 import asyncio
+import contextlib
 import logging
 from typing import Any, Dict
 
 from aiovantage import Vantage, VantageEvent
-from aiovantage.config_client.objects import SystemObject
+from aiovantage.config_client.objects import Button
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
-def callback(event: VantageEvent, obj: SystemObject, data: Dict[str, Any]) -> None:
-    object_type = type(obj).__name__
-
+def callback(event: VantageEvent, obj: Button, data: Dict[str, Any]) -> None:
+    """Print out any state changes."""
     if event == VantageEvent.OBJECT_ADDED:
-        print(f"[{object_type} added] '{obj.name}' ({obj.id})")
+        print(f"[Button added] '{obj.name}' ({obj.id})")
+
     elif event == VantageEvent.OBJECT_UPDATED:
-        print(f"[{object_type} updated] '{obj.name}' ({obj.id})")
+        print(f"[Button updated] '{obj.name}' ({obj.id})")
         for attr in data.get("attrs_changed", []):
             print(f"    {attr} = {getattr(obj, attr)}")
 
 
 async def main() -> None:
+    """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
     async with Vantage(args.host, args.username, args.password) as vantage:
-        # Subscribe to updates for all objects
-        vantage.subscribe(callback)
+        # Subscribe to updates for all buttons
+        vantage.buttons.subscribe(callback)
 
-        # Fetch all known objects from the controller
-        await vantage.initialize()
+        # Fetch all known loads from the controller
+        await vantage.buttons.initialize()
 
         # Keep running for a while
         await asyncio.sleep(3600)
 
 
-try:
+with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
-except KeyboardInterrupt:
-    pass
```

### Comparing `aiovantage-0.2.0/examples/omni_sensors/dump_omni_sensors.py` & `aiovantage-0.2.1/examples/omni_sensors/dump_omni_sensors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,32 @@
-"""
-Prints out the id, name, and level of each omni sensor in the Vantage controller.
-"""
+"""Prints out the id, name, and level of each omni sensor in the Vantage controller."""
 
 import argparse
 import asyncio
+import contextlib
 import logging
 
 from aiovantage import Vantage
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
 async def main() -> None:
+    """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
     # Connect to the Vantage controller and print out the name and level of each load
     async with Vantage(args.host, args.username, args.password) as vantage:
         async for omni_sensor in vantage.omni_sensors:
             level = f"{omni_sensor.level}" if omni_sensor.level is not None else "?"
             print(f"[{omni_sensor.id}] '{omni_sensor.name}' = {level}")
 
 
-try:
+with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
-except KeyboardInterrupt:
-    pass
```

### Comparing `aiovantage-0.2.0/examples/omni_sensors/monitor_omni_sensors.py` & `aiovantage-0.2.1/examples/rgb_loads/monitor_rgb_loads.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,48 @@
-"""
-Fetch all omni sensors from the Vantage controller, and print out any state changes.
-"""
+"""Fetch all RGB loads from the Vantage controller, and print out any state changes."""
 
 import argparse
 import asyncio
+import contextlib
 import logging
 from typing import Any, Dict
 
 from aiovantage import Vantage, VantageEvent
-from aiovantage.config_client.objects import OmniSensor
+from aiovantage.config_client.objects import RGBLoad
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
-def callback(event: VantageEvent, obj: OmniSensor, data: Dict[str, Any]) -> None:
+def callback(event: VantageEvent, obj: RGBLoad, data: Dict[str, Any]) -> None:
+    """Print out any state changes."""
     if event == VantageEvent.OBJECT_ADDED:
-        print(f"[Sensor added] '{obj.name}' ({obj.id})")
-
+        print(f"[RGBLoad added] '{obj.name}' ({obj.id})")
     elif event == VantageEvent.OBJECT_UPDATED:
-        print(f"[Sensor updated] '{obj.name}' ({obj.id})")
+        print(f"[RGBLoad updated] '{obj.name}' ({obj.id})")
         for attr in data.get("attrs_changed", []):
             print(f"    {attr} = {getattr(obj, attr)}")
 
 
 async def main() -> None:
+    """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
     async with Vantage(args.host, args.username, args.password) as vantage:
-        # Subscribe to updates for all sensors
-        vantage.omni_sensors.subscribe(callback)
+        # Subscribe to RGB load updates
+        vantage.rgb_loads.subscribe(callback)
 
-        # Fetch all known sensors from the controller
-        await vantage.omni_sensors.initialize()
+        # Fetch all known RGB loads from the controller
+        await vantage.rgb_loads.initialize()
 
         # Keep running for a while
         await asyncio.sleep(3600)
 
 
-try:
+with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
-except KeyboardInterrupt:
-    pass
```

### Comparing `aiovantage-0.2.0/examples/rgb_loads/dump_rgb_loads.py` & `aiovantage-0.2.1/examples/rgb_loads/dump_rgb_loads.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-"""
-Prints out the id and name of each RGB load in the Vantage controller.
-"""
+"""Prints out the id and name of each RGB load in the Vantage controller."""
 
 import argparse
 import asyncio
+import contextlib
 import logging
 
 from aiovantage import Vantage
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
 async def main() -> None:
+    """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
     # Connect to the Vantage controller and print out the name and level of each load
     async with Vantage(args.host, args.username, args.password) as vantage:
         async for rgb_load in vantage.rgb_loads:
             print(
                 f"[{rgb_load.id}] '{rgb_load.name}' "
                 f"is {'ON' if rgb_load.is_on else 'OFF'}"
             )
 
 
-try:
+with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
-except KeyboardInterrupt:
-    pass
```

### Comparing `aiovantage-0.2.0/examples/rgb_loads/monitor_rgb_loads.py` & `aiovantage-0.2.1/examples/omni_sensors/monitor_omni_sensors.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-"""
-Fetch all RGB loads from the Vantage controller, and print out any state changes.
-"""
+"""Fetch all omni sensors from the Vantage controller, and print any state changes."""
 
 import argparse
 import asyncio
+import contextlib
 import logging
 from typing import Any, Dict
 
 from aiovantage import Vantage, VantageEvent
-from aiovantage.config_client.objects import RGBLoad
+from aiovantage.config_client.objects import OmniSensor
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
-def callback(event: VantageEvent, obj: RGBLoad, data: Dict[str, Any]) -> None:
+def callback(event: VantageEvent, obj: OmniSensor, data: Dict[str, Any]) -> None:
+    """Print out any state changes."""
     if event == VantageEvent.OBJECT_ADDED:
-        print(f"[RGBLoad added] '{obj.name}' ({obj.id})")
+        print(f"[Sensor added] '{obj.name}' ({obj.id})")
+
     elif event == VantageEvent.OBJECT_UPDATED:
-        print(f"[RGBLoad updated] '{obj.name}' ({obj.id})")
+        print(f"[Sensor updated] '{obj.name}' ({obj.id})")
         for attr in data.get("attrs_changed", []):
             print(f"    {attr} = {getattr(obj, attr)}")
 
 
 async def main() -> None:
+    """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
     async with Vantage(args.host, args.username, args.password) as vantage:
-        # Subscribe to RGB load updates
-        vantage.rgb_loads.subscribe(callback)
+        # Subscribe to updates for all sensors
+        vantage.omni_sensors.subscribe(callback)
 
-        # Fetch all known RGB loads from the controller
-        await vantage.rgb_loads.initialize()
+        # Fetch all known sensors from the controller
+        await vantage.omni_sensors.initialize()
 
         # Keep running for a while
         await asyncio.sleep(3600)
 
 
-try:
+with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
-except KeyboardInterrupt:
-    pass
```

### Comparing `aiovantage-0.2.0/src/aiovantage/__init__.py` & `aiovantage-0.2.1/src/aiovantage/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,29 @@
+"""Interact with and control Vantage InFusion home automation controllers."""
+
 __all__ = ["Vantage", "VantageEvent"]
 
 import asyncio
 from types import TracebackType
 from typing import Callable, Optional, Type
 
 from typing_extensions import Self
 
 from aiovantage.command_client import CommandClient
 from aiovantage.config_client import ConfigClient
 from aiovantage.config_client.objects import SystemObject
 from aiovantage.controllers.areas import AreasController
 from aiovantage.controllers.base import EventCallback
-from aiovantage.controllers.blinds import BlindsController
 from aiovantage.controllers.blind_groups import BlindGroupsController
+from aiovantage.controllers.blinds import BlindsController
 from aiovantage.controllers.buttons import ButtonsController
 from aiovantage.controllers.dry_contacts import DryContactsController
 from aiovantage.controllers.gmem import GMemController
-from aiovantage.controllers.loads import LoadsController
 from aiovantage.controllers.load_groups import LoadGroupsController
+from aiovantage.controllers.loads import LoadsController
 from aiovantage.controllers.masters import MastersController
 from aiovantage.controllers.omni_sensors import OmniSensorsController
 from aiovantage.controllers.rgb_loads import RGBLoadsController
 from aiovantage.controllers.stations import StationsController
 from aiovantage.controllers.tasks import TasksController
 
 from .events import VantageEvent
@@ -63,24 +65,25 @@
         self._masters = MastersController(self)
         self._rgb_loads = RGBLoadsController(self)
         self._omni_sensors = OmniSensorsController(self)
         self._stations = StationsController(self)
         self._tasks = TasksController(self)
 
     async def __aenter__(self) -> Self:
+        """Return context manager."""
         return self
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> None:
+        """Exit context manager."""
         await self.close()
-
         if exc_val:
             raise exc_val
 
     @property
     def config_client(self) -> ConfigClient:
         """Return the config client."""
         return self._config_client
@@ -176,16 +179,15 @@
             self._rgb_loads.initialize(),
             self._omni_sensors.initialize(),
             self._stations.initialize(),
             self._tasks.initialize(),
         )
 
     def subscribe(self, callback: EventCallback[SystemObject]) -> Callable[[], None]:
-        """
-        Subscribe to state changes for all objects.
+        """Subscribe to state changes for all objects.
 
         Returns:
             A function to unsubscribe.
         """
 
         unsubscribes = [
             self.areas.subscribe(callback),
```

### Comparing `aiovantage-0.2.0/src/aiovantage/command_client/README.md` & `aiovantage-0.2.1/src/aiovantage/command_client/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -57,16 +57,16 @@
     await client.command("LOAD", 118, 100)
 ```
 
 
 ### Subscribe to load events
 
 ```python
-from aiovantage.command_client import CommandClient
+from aiovantage.command_client import CommandClient, Event, EventType
 
 def callback(event: Event) -> None:
     assert event["tag"] == EventType.STATUS
-    print(f"Load {event["id"]} changed state")
+    print(f"Load {event['id']} changed state")
 
 client = CommandClient("10.2.0.103")
 await client.subscribe_status(callback, "LOAD")
 ```
```

### Comparing `aiovantage-0.2.0/src/aiovantage/command_client/errors.py` & `aiovantage-0.2.1/src/aiovantage/command_client/errors.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,44 @@
+"""Command client exceptions."""
+
 import asyncio
 
 
 class ClientError(Exception):
-    pass
+    """Base exception for command client."""
 
 
 class ClientConnectionError(ClientError):
-    pass
+    """Exception for command client connection errors."""
 
 
 class ClientTimeoutError(asyncio.TimeoutError, ClientConnectionError):
-    pass
+    """Exception for command client connection errors caused by timeouts."""
 
 
 class CommandError(ClientError):
+    """Base exception for errors returned by the Host Command service."""
+
     @classmethod
     def from_string(cls, message: str) -> "CommandError":
+        """Create a CommandError from a string returned by the Host Command service."""
         tag, error_message = message.split(" ", 1)
         _, _, error_code_str = tag.split(":")
         error_code = int(error_code_str)
 
-        exc: Exception
+        exc: CommandError
         if error_code == 21:
             exc = LoginRequiredError(error_message)
         elif error_code == 23:
             exc = LoginFailedError(error_message)
         else:
             exc = CommandError(f"{error_message} (Error code {error_code})")
+
         return exc
 
 
 class LoginRequiredError(CommandError):
-    pass
+    """Login is required to perform this command."""
 
 
 class LoginFailedError(CommandError):
-    pass
+    """Login failed."""
```

### Comparing `aiovantage-0.2.0/src/aiovantage/command_client/helpers.py` & `aiovantage-0.2.1/src/aiovantage/command_client/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,34 @@
+"""Utility functions for the Host Command service client."""
+
 import re
 from decimal import Decimal
+from ssl import CERT_NONE, PROTOCOL_TLS_CLIENT, SSLContext
 from typing import Sequence, Union
 
 TOKEN_PATTERN = re.compile(r'"([^""]*(?:""[^""]*)*)"|(\{.*?\})|(\S+)')
 
 
-def tokenize_response(string: str) -> Sequence[str]:
+def create_ssl_context() -> SSLContext:
+    """SSL context that doesn't verify hostname or certificate.
+
+    We don't have a local issuer certificate to check against, and we'll most likely be
+    connecting to an IP address, so we can't check the hostname.
     """
-    Tokenize a response from the Host Command service, handling quoted strings and
-    byte arrays (in curly braces) as single tokens.
+
+    context = SSLContext(PROTOCOL_TLS_CLIENT)
+    context.check_hostname = False
+    context.verify_mode = CERT_NONE
+    return context
+
+
+def tokenize_response(string: str) -> Sequence[str]:
+    """Tokenize a response from the Host Command service.
+
+    Handles quoted strings and byte arrays (in curly braces) as single tokens.
 
     Args:
         string: The response string to tokenize.
 
     Returns:
         A list of string tokens.
     """
@@ -29,17 +45,18 @@
 
     return tokens
 
 
 def encode_params(
     *params: Union[str, int, float, Decimal, bool], force_quotes: bool = False
 ) -> str:
-    """
-    Encode a list of parameters, converting all params to strings, wrapping strings in
-    double quote, and escaping double quotes in strings.
+    """Encode a list of parameters for sending to the Host Command service.
+
+    Converts all params to strings, wraps strings in double quotes, and escapes
+    double quotes.
 
     Args:
         params: The parameters to encode.
         force_quotes: Whether to force string params to be wrapped in double quotes.
 
     Returns:
         The encoded parameters, joined by spaces.
@@ -55,10 +72,10 @@
             else:
                 encoded_params.append(value)
         elif isinstance(value, bool):
             encoded_params.append(str(int(value)))
         elif isinstance(value, (int, float, Decimal)):
             encoded_params.append(str(value))
         else:
-            raise ValueError(f"Invalid value type: {type(value)}")
+            raise TypeError(f"Invalid value type: {type(value)}")
 
     return " ".join(encoded_params)
```

### Comparing `aiovantage-0.2.0/src/aiovantage/command_client/interfaces/__init__.py` & `aiovantage-0.2.1/src/aiovantage/command_client/interfaces/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Comand client object interfaces."""
+
 from .blind import BlindInterface
 from .button import ButtonInterface
 from .color_temperature import ColorTemperatureInterface
 from .gmem import GMemInterface
 from .introspection import IntrospectionInterface
 from .load import LoadInterface
 from .object import ObjectInterface
```

### Comparing `aiovantage-0.2.0/src/aiovantage/command_client/interfaces/blind.py` & `aiovantage-0.2.1/src/aiovantage/command_client/interfaces/blind.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,121 +1,123 @@
+"""Interface for querying and controlling blinds."""
+
 from collections import namedtuple
 from decimal import Decimal
 from typing import Sequence
 
 from .base import Interface
 
 
 class BlindInterface(Interface):
+    """Interface for querying and controlling blinds."""
+
     BlindState = namedtuple(
         "BlindState",
         ["is_moving", "start_pos", "end_pos", "transition_time", "start_time"],
     )
 
-    async def open(self, id: int) -> None:
-        """
-        Open a blind.
+    async def open(self, vid: int) -> None:
+        """Open a blind.
 
         Args:
-            id: The ID of the blind.
+            vid: The Vantage ID of the blind.
         """
 
         # INVOKE <id> Blind.Open
         # -> R:INVOKE <id> <rcode> Blind.Open
-        await self.invoke(id, "Blind.Open")
+        await self.invoke(vid, "Blind.Open")
 
-    async def close(self, id: int) -> None:
-        """
-        Close a blind.
+    async def close(self, vid: int) -> None:
+        """Close a blind.
 
         Args:
-            id: The ID of the blind.
+            vid: The Vantage ID of the blind.
         """
 
         # INVOKE <id> Blind.Close
         # -> R:INVOKE <id> <rcode> Blind.Close
-        await self.invoke(id, "Blind.Close")
+        await self.invoke(vid, "Blind.Close")
 
-    async def stop(self, id: int) -> None:
-        """
-        Stop a blind.
+    async def stop(self, vid: int) -> None:
+        """Stop a blind.
 
         Args:
-            id: The ID of the blind.
+            vid: The Vantage ID of the blind.
         """
 
         # INVOKE <id> Blind.Stop
         # -> R:INVOKE <id> <rcode> Blind.Stop
-        await self.invoke(id, "Blind.Stop")
+        await self.invoke(vid, "Blind.Stop")
 
-    async def get_position(self, id: int) -> Decimal:
-        """
-        Get the position of a blind.
+    async def get_position(self, vid: int) -> Decimal:
+        """Get the position of a blind.
 
         Args:
-            id: The ID of the blind.
+            vid: The Vantage ID of the blind.
 
         Returns:
             The position of the blind, as a percentage.
         """
 
         # INVOKE <id> Blind.GetPosition
         # -> R:INVOKE <id> <position (0-100.000)> Blind.GetPosition
-        response = await self.invoke(id, "Blind.GetPosition")
+        response = await self.invoke(vid, "Blind.GetPosition")
         position = Decimal(response.args[1])
 
         return position
 
-    async def set_position(self, id: int, position: float) -> None:
-        """
-        Set the position of a blind.
+    async def set_position(self, vid: int, position: float) -> None:
+        """Set the position of a blind.
 
         Args:
-            id: The ID of the blind.
+            vid: The Vantage ID of the blind.
             position: The position to set the blind to, as a percentage.
         """
 
         # INVOKE <id> Blind.SetPosition <position>
         # -> R:INVOKE <id> <rcode> Blind.SetPosition <position>
-        await self.invoke(id, "Blind.SetPosition", position)
+        await self.invoke(vid, "Blind.SetPosition", position)
 
     @classmethod
     def parse_blind_status(cls, args: Sequence[str]) -> Decimal:
-        """
-        Parse a simple "S:BLIND" event.
+        """Parse a simple 'S:BLIND' event.
 
         Args:
             args: The arguments of the event.
 
         Returns:
             The position of the blind, as a percentage.
         """
 
         # STATUS BLIND
         # -> S:BLIND <id> <position (0-100.000)>
         return Decimal(args[0])
 
     @classmethod
     def parse_get_position_status(cls, args: Sequence[str]) -> Decimal:
+        """Parse a 'Blind.GetPosition' event."""
+
         # ELLOG STATUS ON
         # -> EL: <id> Blind.GetPosition <position (0-100000)>
 
         # ADDSTATUS <id>
         # -> S:STATUS <id> Blind.GetPosition <position (0-100000)>
         position = Decimal(args[0]) / 1000
 
         return position
 
     @classmethod
     def parse_get_state_status(cls, args: Sequence[str]) -> BlindState:
+        """Parse a 'Blind.GetBlindState' event."""
+
         # ADDSTATUS <id>
-        # -> S:STATUS <id> Blind.GetBlindState <moving> <start> <end> <transitionTime> <startTime> # noqa
+        # -> S:STATUS <id> Blind.GetBlindState <moving> <start> <end> <transitionTime> <startTime>
 
         # ELLOG STATUSEX ON
-        # -> EL: <id> Blind.GetBlindState <moving> <start> <end> <transitionTime> <startTime> # noqa
+        # -> EL: <id> Blind.GetBlindState <moving> <start> <end> <transitionTime> <startTime>
         return cls.BlindState(
             # Is the blind currently moving?
             is_moving=bool(int(args[0])),
             # Position the blind is moving from (as a percentage)
             start_pos=Decimal(args[1]) / 1000,
             # Position the blind is moving to (as a percentage)
             end_pos=Decimal(args[2]) / 1000,
```

### Comparing `aiovantage-0.2.0/src/aiovantage/command_client/interfaces/button.py` & `aiovantage-0.2.1/src/aiovantage/command_client/interfaces/button.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,105 +1,102 @@
+"""Interface for querying and controlling buttons."""
+
 from typing import Sequence
 
 from .base import Interface
 
 
 class ButtonInterface(Interface):
-    async def get_state(self, id: int) -> bool:
-        """
-        Get the state of a button.
+    """Interface for querying and controlling buttons."""
+
+    async def get_state(self, vid: int) -> bool:
+        """Get the state of a button.
 
         Args:
-            id: The ID of the button.
+            vid: The Vantage ID of the button.
 
         Returns:
             The pressed state of the button, True if pressed, False if not.
         """
 
         # INVOKE <id> Button.GetState
         # -> R:INVOKE <id> <state (Up/Down)> Button.GetState
-        response = await self.invoke(id, "Button.GetState")
+        response = await self.invoke(vid, "Button.GetState")
         state = response.args[1]
         if state == "Up":
             return False
-        elif state == "Down":
+        if state == "Down":
             return True
-        else:
-            raise ValueError(f"Invalid button state name: {state}")
 
-    async def set_state(self, id: int, pressed: bool) -> None:
-        """
-        Set the state of a button.
+        raise ValueError(f"Invalid button state name: {state}")
+
+    async def set_state(self, vid: int, pressed: bool) -> None:
+        """Set the state of a button.
 
         Args:
-            id: The ID of the button.
-            state: The state to set the button to, either a State.UP or State.DOWN.
+            vid: The Vantage ID of the button.
+            pressed: The state to set the button to, either a State.UP or State.DOWN.
         """
 
         # INVOKE <id> Button.SetState <state (0/1/Up/Down)>
         # -> R:INVOKE <id> Button.SetState <state (Up/Down)>
-        await self.invoke(id, "Button.SetState", pressed)
+        await self.invoke(vid, "Button.SetState", pressed)
 
-    async def press(self, id: int) -> None:
-        """
-        Press a button.
+    async def press(self, vid: int) -> None:
+        """Press a button.
 
         Args:
-            id: The ID of the button.
+            vid: The Vantage ID of the button.
         """
 
-        await self.set_state(id, True)
+        await self.set_state(vid, True)
 
-    async def release(self, id: int) -> None:
-        """
-        Release a button.
+    async def release(self, vid: int) -> None:
+        """Release a button.
 
         Args:
-            id: The ID of the button.
+            vid: The Vantage ID of the button.
         """
 
-        await self.set_state(id, False)
+        await self.set_state(vid, False)
 
-    async def press_and_release(self, id: int) -> None:
-        """
-        Press and release a button.
+    async def press_and_release(self, vid: int) -> None:
+        """Press and release a button.
 
         Args:
-            id: The ID of the button.
+            vid: The Vantage ID of the button.
         """
 
-        await self.press(id)
-        await self.release(id)
+        await self.press(vid)
+        await self.release(vid)
 
     @classmethod
     def parse_btn_status(cls, args: Sequence[str]) -> bool:
-        """
-        Parse a simple "S:BTN" event.
+        """Parse a simple 'S:BTN' event.
 
         Args:
             args: The arguments of the event.
 
         Returns:
             The state of the button, either a State.UP or State.DOWN.
         """
 
         # STATUS BTN
         # -> S:BTN <id> <state (PRESS/RELEASE)>
         state = args[0]
         if state == "RELEASE":
             return False
-        elif state == "PRESS":
+        if state == "PRESS":
             return True
-        else:
-            raise ValueError(f"Invalid button state name: {state}")
+
+        raise ValueError(f"Invalid button state name: {state}")
 
     @classmethod
     def parse_get_state_status(cls, args: Sequence[str]) -> bool:
-        """
-        Parse a "Button.GetState" event.
+        """Parse a 'Button.GetState' event.
 
         Args:
             args: The arguments of the event.
 
         Returns:
             The state of the button, either a State.UP or State.DOWN.
         """
```

### Comparing `aiovantage-0.2.0/src/aiovantage/command_client/interfaces/color_temperature.py` & `aiovantage-0.2.1/src/aiovantage/command_client/interfaces/color_temperature.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,53 @@
+"""Interface for querying and controlling color temperature."""
+
 from typing import Sequence
 
 from .base import Interface
 
 
 class ColorTemperatureInterface(Interface):
-    async def get_color_temp(self, id: int) -> int:
-        """
-        Get the color temperature of a light.
+    """Interface for querying and controlling color temperature."""
+
+    async def get_color_temp(self, vid: int) -> int:
+        """Get the color temperature of a light.
 
         Args:
-            id: The ID of the light.
+            vid: The Vantage ID of the light.
 
         Returns:
             The color temperature of the light, in Kelvin.
         """
 
         # INVOKE <id> ColorTemperature.Get
         # -> R:INVOKE <id> <temp> ColorTemperature.Get
-        response = await self.invoke(id, "ColorTemperature.Get")
+        response = await self.invoke(vid, "ColorTemperature.Get")
         color_temp = int(response.args[1])
 
         return color_temp
 
-    async def set_color_temp(self, id: int, temp: int, transition: int = 0) -> None:
-        """
-        Set the color temperature of a light.
+    async def set_color_temp(self, vid: int, temp: int, transition: int = 0) -> None:
+        """Set the color temperature of a light.
 
         Args:
-            id: The ID of the light.
+            vid: The Vantage ID of the light.
             temp: The color temperature to set the light to, in Kelvin.
             transition: The time in seconds to transition to the new color
         """
 
         # Ensure the temperature is an integer
         temp = int(temp)
 
         # INVOKE <id> ColorTemperature.Set <temp> <seconds>
         # -> R:INVOKE <id> <rcode> ColorTemperature.Set <temp>
-        await self.invoke(id, "ColorTemperature.Set", temp, transition)
+        await self.invoke(vid, "ColorTemperature.Set", temp, transition)
 
     @classmethod
     def parse_get_status(cls, args: Sequence[str]) -> int:
-        """
-        Parse a "ColorTemperature.Get" event.
+        """Parse a 'ColorTemperature.Get' event.
 
         Args:
             args: The arguments of the event.
 
         Returns:
             The color temperature, in Kelvin.
         """
```

### Comparing `aiovantage-0.2.0/src/aiovantage/command_client/interfaces/gmem.py` & `aiovantage-0.2.1/src/aiovantage/command_client/interfaces/gmem.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,49 @@
+"""Interface for querying and controlling variables."""
+
 from typing import Sequence, Union
 
 from .base import Interface
 
 
 class GMemInterface(Interface):
-    async def get_value(self, id: int) -> str:
-        """
-        Get the value of a variable.
+    """Interface for querying and controlling variables."""
+
+    async def get_value(self, vid: int) -> str:
+        """Get the value of a variable.
 
         Args:
-            id: The variable ID.
+            vid: The Vantage ID of the variable.
 
         Returns:
             The value of the variable, as a raw string.
         """
 
         # GETVARIABLE {id}
         # -> R:GETVARIABLE {id} {value}
-        response = await self.command_client.command("GETVARIABLE", id)
+        response = await self.command_client.command("GETVARIABLE", vid)
         value = response.args[1]
 
         return value
 
-    async def set_value(self, id: int, value: Union[int, str, bool]) -> None:
-        """
-        Set the value of a variable.
+    async def set_value(self, vid: int, value: Union[int, str, bool]) -> None:
+        """Set the value of a variable.
 
         Args:
-            id: The variable ID.
+            vid: The Vantage ID of the variable.
             value: The value to set, either a bool, int, or str.
         """
 
         # SETVARIABLE {id} {value}
         # -> R:SETVARIABLE {id} {value}
-        await self.command_client.command("VARIABLE", id, value, force_quotes=True)
+        await self.command_client.command("VARIABLE", vid, value, force_quotes=True)
 
     @classmethod
     def parse_variable_status(cls, args: Sequence[str]) -> str:
-        """
-        Parse a simple "S:VARIABLE" event.
+        """Parse a simple 'S:VARIABLE' event.
 
         Args:
             args: The arguments of the event.
 
         Returns:
             The level of the load.
         """
```

### Comparing `aiovantage-0.2.0/src/aiovantage/command_client/interfaces/load.py` & `aiovantage-0.2.1/src/aiovantage/command_client/interfaces/load.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,120 +1,128 @@
+"""Interface for querying and controlling loads."""
+
 from enum import Enum
 from typing import Sequence
 
 from .base import Interface
 
 
 class LoadInterface(Interface):
+    """Interface for querying and controlling loads."""
+
     class RampType(Enum):
+        """The type of ramp to perform."""
+
         STOP = 2
         OPPOSITE = 3
         DOWN = 4
         UP = 5
         FIXED = 6
         VARIABLE = 7
         ADJUST = 8
 
-    async def turn_on(self, id: int, transition: float = 0, level: float = 100) -> None:
-        """
-        Turn on a load.
+    async def turn_on(
+        self, vid: int, transition: float = 0, level: float = 100
+    ) -> None:
+        """Turn on a load.
 
         Args:
-            id: The ID of the load.
+            vid: The Vantage ID of the load.
+            transition: The time in seconds to transition to the new level.
+            level: The level to set the load to (0-100).
         """
 
         if transition:
-            await self.ramp(id, level, transition)
+            await self.ramp(vid, level, transition)
         else:
-            await self.set_level(id, level)
+            await self.set_level(vid, level)
 
-    async def turn_off(self, id: int, transition: float = 0) -> None:
-        """
-        Turn off a load.
+    async def turn_off(self, vid: int, transition: float = 0) -> None:
+        """Turn off a load.
 
         Args:
-            id: The ID of the load.
+            vid: The Vantage ID of the load.
+            transition: The time in seconds to ramp the load down.
         """
 
         if transition:
-            await self.ramp(id, 0, transition)
+            await self.ramp(vid, 0, transition)
         else:
-            await self.set_level(id, 0)
+            await self.set_level(vid, 0)
 
-    async def get_level(self, id: int) -> float:
-        """
-        Get the level of a load.
+    async def get_level(self, vid: int) -> float:
+        """Get the level of a load.
 
         Args:
-            id: The ID of the load.
+            vid: The Vantage ID of the load.
 
         Returns:
             The level of the load, as a percentage (0-100).
         """
 
         # INVOKE <id> Load.GetLevel
         # -> R:INVOKE <id> <level (0-100)> Load.GetLevel
-        response = await self.invoke(id, "Load.GetLevel")
+        response = await self.invoke(vid, "Load.GetLevel")
         level = float(response.args[1])
 
         return level
 
-    async def set_level(self, id: int, level: float) -> None:
-        """
-        Set the level of a load.
+    async def set_level(self, vid: int, level: float) -> None:
+        """Set the level of a load.
 
         Args:
-            id: The ID of the load.
+            vid: The Vantage ID of the load.
             level: The level to set the load to (0-100).
         """
 
         # Clamp level to 0-100
         level = max(min(level, 100), 0)
 
         # INVOKE <id> Load.SetLevel <level (0-100)>
         # -> R:INVOKE <id> <rcode> Load.SetLevel <level (0-100)>
-        await self.invoke(id, "Load.SetLevel", level)
+        await self.invoke(vid, "Load.SetLevel", level)
 
     async def ramp(
-        self, id: int, level: float, seconds: float, type: RampType = RampType.FIXED
+        self,
+        vid: int,
+        level: float,
+        seconds: float,
+        ramp_type: RampType = RampType.FIXED,
     ) -> None:
-        """
-        Ramp a load to a level over a number of seconds.
+        """Ramp a load to a level over a number of seconds.
 
         Args:
-            id: The ID of the load.
+            vid: The Vantage ID of the load.
             level: The level to ramp the load to (0-100).
             seconds: The number of seconds to ramp the load over.
-            type: The type of ramp to perform.
+            ramp_type: The type of ramp to perform.
         """
 
         # INVOKE <id> Load.Ramp <type> <seconds> <level>
         # -> R:INVOKE <id> <rcode> Load.Ramp <type> <seconds> <level>
-        await self.invoke(id, "Load.Ramp", type.value, seconds, level)
+        await self.invoke(vid, "Load.Ramp", ramp_type.value, seconds, level)
 
     @classmethod
     def parse_load_status(cls, args: Sequence[str]) -> float:
-        """
-        Parse a simple "S:LOAD" event.
+        """Parse a simple 'S:LOAD' event.
 
         Args:
             args: The arguments of the event.
 
         Returns:
             The level of the load.
         """
 
         # STATUS LOAD
         # -> S:LOAD <id> <level (0-100)>
         return float(args[0])
 
     @classmethod
     def parse_get_level_status(cls, args: Sequence[str]) -> float:
-        """
-        Parse a "Load.GetLevel" event.
+        """Parse a 'Load.GetLevel' event.
 
         Args:
             args: The arguments of the event.
 
         Returns:
             The level of the load.
         """
```

### Comparing `aiovantage-0.2.0/src/aiovantage/command_client/interfaces/rgb_load.py` & `aiovantage-0.2.1/src/aiovantage/command_client/interfaces/rgb_load.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,257 +1,255 @@
+"""Interface for querying and controlling RGB loads."""
+
 import struct
 from typing import Sequence, Tuple
 
 from .base import Interface
 
 
 class RGBLoadInterface(Interface):
-    async def get_rgb(self, id: int) -> Tuple[int, ...]:
-        """
-        Get the RGB color of a load from the controller.
+    """Interface for querying and controlling RGB loads."""
+
+    async def get_rgb(self, vid: int) -> Tuple[int, ...]:
+        """Get the RGB color of a load from the controller.
 
         Args:
-            id: The ID of the load.
+            vid: The Vantage ID of the RGB load.
 
         Returns:
             The value of the RGB color as a tuple of (red, green, blue).
         """
 
-        return (await self.get_color(id))[:3]
+        return (await self.get_color(vid))[:3]
 
-    async def get_rgbw(self, id: int) -> Tuple[int, ...]:
-        """
-        Get the RGBW color of a load from the controller.
+    async def get_rgbw(self, vid: int) -> Tuple[int, ...]:
+        """Get the RGBW color of a load from the controller.
 
         Args:
-            id: The ID of the load.
+            vid: The Vantage ID of the RGB load.
 
         Returns:
             The value of the RGBW color as a tuple of (red, green, blue, white).
         """
 
-        return tuple([await self.get_rgb_channel(id, channel) for channel in range(4)])
+        return tuple([await self.get_rgb_channel(vid, channel) for channel in range(4)])
 
-    async def get_hsl(self, id: int) -> Tuple[int, ...]:
-        """
-        Get the HSL color of a load from the controller.
+    async def get_hsl(self, vid: int) -> Tuple[int, ...]:
+        """Get the HSL color of a load from the controller.
 
         Args:
-            id: The ID of the load.
+            vid: The Vantage ID of the RGB load.
 
         Returns:
             The value of the HSL color as a tuple of (hue, saturation, lightness).
         """
 
         return tuple(
-            [await self.get_hsl_attribute(id, attribute) for attribute in range(3)]
+            [await self.get_hsl_attribute(vid, attribute) for attribute in range(3)]
         )
 
-    async def get_color(self, id: int) -> Tuple[int, ...]:
-        """
-        Get the RGB/RGBW color of a load from the controller.
+    async def get_color(self, vid: int) -> Tuple[int, ...]:
+        """Get the RGB/RGBW color of a load from the controller.
 
         Args:
-            id: The ID of the load.
+            vid: The Vantage ID of the RGB load.
 
         Returns:
             The value of the RGB/RGBW color as a bytearray.
         """
 
         # INVOKE <id> RGBLoad.GetColor
         # -> R:INVOKE <id> <color> RGBLoad.GetColor
-        response = await self.invoke(id, "RGBLoad.GetColor")
+        response = await self.invoke(vid, "RGBLoad.GetColor")
         color = int(response.args[1])
 
         return tuple(struct.pack(">i", color))
 
-    async def get_rgb_channel(self, id: int, channel: int) -> int:
-        """
-        Get a single RGB color channel of a load from the controller.
+    async def get_rgb_channel(self, vid: int, channel: int) -> int:
+        """Get a single RGB color channel of a load from the controller.
 
         Args:
-            id: The ID of the load.
+            vid: The Vantage ID of the RGB load.
             channel: The channel to get the color of.
 
         Returns:
             The value of the RGB channel, 0-255.
         """
 
         # INVOKE <id> RGBLoad.GetRGB <channel>
         # -> R:INVOKE <id> <value> RGBLoad.GetRGB <channel>
-        response = await self.invoke(id, "RGBLoad.GetRGB", channel)
+        response = await self.invoke(vid, "RGBLoad.GetRGB", channel)
         color = int(response.args[1])
 
         return color
 
-    async def get_rgbw_channel(self, id: int, channel: int) -> int:
-        """
-        Get a single RGBW color channel of a load from the controller.
+    async def get_rgbw_channel(self, vid: int, channel: int) -> int:
+        """Get a single RGBW color channel of a load from the controller.
 
         Args:
-            id: The ID of the load.
+            vid: The Vantage ID of the RGB load.
             channel: The channel to get the color of.
 
         Returns:
             The value of the RGBW channel, 0-255.
         """
 
         # INVOKE <id> RGBLoad.GetRGB <channel>
         # -> R:INVOKE <id> <value> RGBLoad.GetRGB <channel>
-        response = await self.invoke(id, "RGBLoad.GetRGBW", channel)
+        response = await self.invoke(vid, "RGBLoad.GetRGBW", channel)
         color = int(response.args[1])
 
         return color
 
-    async def get_hsl_attribute(self, id: int, attribute: int) -> int:
-        """
-        Get a single HSL color attribute of a load from the controller.
+    async def get_hsl_attribute(self, vid: int, attribute: int) -> int:
+        """Get a single HSL color attribute of a load from the controller.
 
         Args:
-            id: The ID of the load.
+            vid: The Vantage ID of the RGB load.
             attribute: The attribute to get the value of.
 
         Returns:
             The value of the HSL attribute, 0-360 for hue, 0-100 for saturation and
             lightness.
         """
 
         # INVOKE <id> RGBLoad.GetHSL <channel>
         # -> R:INVOKE <id> <value> RGBLoad.GetHSL <channel>
-        response = await self.invoke(id, "RGBLoad.GetHSL", attribute)
+        response = await self.invoke(vid, "RGBLoad.GetHSL", attribute)
         color = int(response.args[1])
 
         return color
 
-    async def set_rgb(self, id: int, red: int, green: int, blue: int) -> None:
-        """
-        Set the color of an RGB load.
+    async def set_rgb(self, vid: int, red: int, green: int, blue: int) -> None:
+        """Set the color of an RGB load.
 
         Args:
-            id: The ID of the load.
+            vid: The Vantage ID of the RGB load.
             red: The red value of the color, (0-255)
             green: The green value of the color, (0-255)
             blue: The blue value of the color, (0-255)
         """
 
         # Clamp levels to 0-255, ensure they're integers
         red = int(max(min(red, 255), 0))
         green = int(max(min(green, 255), 0))
         blue = int(max(min(blue, 255), 0))
 
         # INVOKE <id> RGBLoad.SetRGB <red> <green> <blue>
         # -> R:INVOKE <id> <rcode> RGBLoad.SetRGB <red> <green> <blue>
-        await self.invoke(id, "RGBLoad.SetRGB", red, green, blue)
+        await self.invoke(vid, "RGBLoad.SetRGB", red, green, blue)
 
     async def set_rgbw(
-        self, id: int, red: int, green: int, blue: int, white: int
+        self, vid: int, red: int, green: int, blue: int, white: int
     ) -> None:
-        """
-        Set the color of an RGBW load.
+        """Set the color of an RGBW load.
 
         Args:
-            id: The ID of the load.
+            vid: The Vantage ID of the RGB load.
             red: The red value of the color, (0-255)
             green: The green value of the color, (0-255)
             blue: The blue value of the color, (0-255)
             white: The white value of the color, (0-255)
         """
 
         # Clamp levels to 0-255
         red = int(max(min(red, 255), 0))
         green = int(max(min(green, 255), 0))
         blue = int(max(min(blue, 255), 0))
         white = int(max(min(white, 255), 0))
 
         # INVOKE <id> RGBLoad.SetRGBW <red> <green> <blue> <white>
         # -> R:INVOKE <id> <rcode> RGBLoad.SetRGBW <red> <green> <blue> <white>
-        await self.invoke(id, "RGBLoad.SetRGBW", red, green, blue, white)
+        await self.invoke(vid, "RGBLoad.SetRGBW", red, green, blue, white)
 
-    async def set_hsl(self, id: int, hue: int, saturation: int, lightness: int) -> None:
-        """
-        Set the color of an HSL load.
+    async def set_hsl(
+        self, vid: int, hue: int, saturation: int, lightness: int
+    ) -> None:
+        """Set the color of an HSL load.
 
         Args:
-            id: The ID of the load.
+            vid: The Vantage ID of the RGB load.
             hue: The hue value of the color, in degrees (0-360).
             saturation: The saturation value of the color, in percent (0-100).
             lightness: The lightness value of the color, in percent (0-100).
         """
 
         # Clamp levels to 0-360, 0-100, ensure they're integers
         hue = int(max(min(hue, 360), 0))
         saturation = int(max(min(saturation, 100), 0))
         lightness = int(max(min(lightness, 100), 0))
 
         # INVOKE <id> RGBLoad.SetHSL <hue> <saturation> <lightness>
         # -> R:INVOKE <id> <rcode> RGBLoad.SetHSL <hue> <saturation> <lightness>
-        await self.invoke(id, "RGBLoad.SetHSL", hue, saturation, lightness)
+        await self.invoke(vid, "RGBLoad.SetHSL", hue, saturation, lightness)
 
     async def dissolve_rgb(
-        self, id: int, red: int, green: int, blue: int, seconds: int
+        self, vid: int, red: int, green: int, blue: int, seconds: int
     ) -> None:
-        """
-        Transition the color of an RGB load over a number of seconds.
+        """Transition the color of an RGB load over a number of seconds.
 
         Args:
-            id: The ID of the load.
+            vid: The Vantage ID of the RGB load.
             red: The new red value of the color, (0-255)
             green: The new green value of the color, (0-255)
             blue: The new blue value of the color, (0-255)
             seconds: The number of seconds the transition should take.
         """
 
         # Clamp levels to 0-255, ensure they're integers
         red = int(max(min(red, 255), 0))
         green = int(max(min(green, 255), 0))
         blue = int(max(min(blue, 255), 0))
 
         # INVOKE <id> RGBLoad.DissolveRGB <red> <green> <blue>
         # -> R:INVOKE <id> <rcode> RGBLoad.DissolveRGB <red> <green> <blue>
-        await self.invoke(id, "RGBLoad.DissolveRGB", red, green, blue, seconds)
+        await self.invoke(vid, "RGBLoad.DissolveRGB", red, green, blue, seconds)
 
     async def dissolve_hsl(
-        self, id: int, hue: int, saturation: int, lightness: int, seconds: int
+        self, vid: int, hue: int, saturation: int, lightness: int, seconds: int
     ) -> None:
-        """
-        Transition the color of an HSL load over a number of seconds.
+        """Transition the color of an HSL load over a number of seconds.
 
         Args:
-            id: The ID of the load.
+            vid: The Vantage ID of the RGB load.
             hue: The new hue value of the color, in degrees (0-360).
             saturation: The new saturation value of the color, in percent (0-100).
             lightness: The new lightness value of the color, in percent (0-100).
             seconds: The number of seconds the transition should take.
         """
 
         # Clamp levels to 0-360, 0-100, ensure they're integers
         hue = int(max(min(hue, 360), 0))
         saturation = int(max(min(saturation, 100), 0))
         lightness = int(max(min(lightness, 100), 0))
 
         # INVOKE <id> RGBLoad.DissolveHSL <hue> <saturation> <lightness>
         # -> R:INVOKE <id> <rcode> RGBLoad.DissolveHSL <hue> <saturation> <lightness>
         await self.invoke(
-            id, "RGBLoad.DissolveHSL", hue, saturation, lightness, seconds
+            vid, "RGBLoad.DissolveHSL", hue, saturation, lightness, seconds
         )
 
     @classmethod
     def parse_color_channel_status(cls, args: Sequence[str]) -> Tuple[int, int]:
+        """Parse an 'RGBLoad.GetRGB' event."""
+
         # ELLOG STATUSEX ON
         # -> EL: <id> RGBLoad.GetRGB <value> <channel>
 
         # STATUS ADD <id>
         # -> S:STATUS <id> RGBLoad.GetRGB <value> <channel>
         value = int(args[0])
         channel = int(args[1])
 
-        return (channel, value)
+        return channel, value
 
     @classmethod
     def parse_get_color_status(cls, args: Sequence[str]) -> bytearray:
+        """Parse an 'RGBLoad.GetColor' event."""
+
         # ELLOG STATUS ON
         # -> EL: <id> RGBLoad.GetColor <color>
 
         # STATUS ADD <id>
         # -> S:STATUS <id> RGBLoad.GetColor <color>
         color = int(args[0])
```

### Comparing `aiovantage-0.2.0/src/aiovantage/command_client/interfaces/sensor.py` & `aiovantage-0.2.1/src/aiovantage/command_client/interfaces/sensor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,34 @@
+"""Interface for querying and controlling sensors."""
+
 from typing import Sequence
 
 from .base import Interface
 
 
 class SensorInterface(Interface):
-    async def get_level(self, id: int) -> int:
-        """
-        Get the level of a sensor.
+    """Interface for querying and controlling sensors."""
+
+    async def get_level(self, vid: int) -> int:
+        """Get the level of a sensor.
 
         Args:
-            id: The ID of the sensor.
+            vid: The Vantage ID of the sensor.
         """
 
         # INVOKE <id> Sensor.GetLevel
         # -> R:INVOKE <id> <level (0-100)> Sensor.GetLevel
-        response = await self.invoke(id, "Sensor.GetLevel")
+        response = await self.invoke(vid, "Sensor.GetLevel")
         level = int(response.args[1])
 
         return level
 
     @classmethod
     def parse_get_level_status(cls, args: Sequence[str]) -> int:
-        """
-        Parse a "Sensor.GetLevel" event.
+        """Parse a 'Sensor.GetLevel' event.
 
         Args:
             args: The arguments of the event.
 
         Returns:
             The level of the sensor.
         """
```

### Comparing `aiovantage-0.2.0/src/aiovantage/command_client/interfaces/task.py` & `aiovantage-0.2.1/src/aiovantage/command_client/interfaces/task.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,85 @@
+"""Interface for querying and controlling tasks."""
+
 from typing import Sequence
 
 from .base import Interface
 
 
 class TaskInterface(Interface):
-    async def is_running(self, id: int) -> bool:
-        """
-        Get the running state of a task.
+    """Interface for querying and controlling tasks."""
+
+    async def is_running(self, vid: int) -> bool:
+        """Get the running state of a task.
 
         Args:
-            id: The ID of the task.
+            vid: The Vantage ID of the task.
         """
 
         # INVOKE <id> Task.IsRunning
         # -> R:INVOKE <id> <running (0/1)> Task.IsRunning
-        response = await self.invoke(id, "Task.IsRunning")
+        response = await self.invoke(vid, "Task.IsRunning")
         is_running = bool(int(response.args[1]))
 
         return is_running
 
-    async def get_state(self, id: int) -> bool:
-        """
-        Get the state of a task.
+    async def get_state(self, vid: int) -> bool:
+        """Get the state of a task.
 
         Args:
-            id: The ID of the task.
+            vid: The Vantage ID of the task.
         """
 
         # INVOKE <id> Task.GetState
         # -> R:INVOKE <id> <state (0/1)> Task.GetState
-        response = await self.invoke(id, "Task.GetState")
+        response = await self.invoke(vid, "Task.GetState")
         task_state = bool(int(response.args[1]))
 
         return task_state
 
-    async def start(self, id: int) -> None:
-        """
-        Start a task.
+    async def start(self, vid: int) -> None:
+        """Start a task.
 
         Args:
-            id: The ID of the task.
+            vid: The Vantage ID of the task.
         """
 
         # INVOKE <id> Task.Start <source> <event> <param1> <param2>
         # -> R:INVOKE <id> <rcode (0/1)> Task.Start <source> <event> <param1> <param2>
-        await self.invoke(id, "Task.Start")
+        await self.invoke(vid, "Task.Start")
 
-    async def stop(self, id: int) -> None:
-        """
-        Stop a running task.
+    async def stop(self, vid: int) -> None:
+        """Stop a running task.
 
         Args:
-            id: The ID of the task.
+            vid: The Vantage ID of the task.
         """
 
         # INVOKE <id> Task.Stop
         # -> R:INVOKE <id> <rcode> Task.Stop
-        await self.invoke(id, "Task.Stop")
+        await self.invoke(vid, "Task.Stop")
 
     @classmethod
     def parse_task_status(cls, args: Sequence[str]) -> bool:
-        """
-        Parse a simple "S:TASK" event.
+        """Parse a simple 'S:TASK' event.
 
         Args:
             args: The arguments of the event.
 
         Returns:
             The state of the task.
         """
 
         # STATUS TASK
         # -> S:TASK <id> <state (0/1)>
         return bool(int(args[0]))
 
     @classmethod
     def parse_get_state_status(cls, args: Sequence[str]) -> bool:
-        """
-        Parse a "Task.GetState" event.
+        """Parse a 'Task.GetState' event.
 
         Args:
             args: The arguments of the event.
 
         Returns:
             The state of the task.
         """
@@ -91,16 +89,15 @@
 
         # STATUS ADD <id>
         # -> S:STATUS <id> Task.GetState <state (0/1)>
         return bool(int(args[0]))
 
     @classmethod
     def parse_is_running_status(cls, args: Sequence[str]) -> bool:
-        """
-        Parse a "Task.IsRunning" event.
+        """Parse a 'Task.IsRunning' event.
 
         Args:
             args: The arguments of the event.
 
         Returns:
             The running state of the task.
         """
```

### Comparing `aiovantage-0.2.0/src/aiovantage/config_client/README.md` & `aiovantage-0.2.1/src/aiovantage/config_client/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 ### Lookup objects by type, using a helper
 
 ```python
 from aiovantage.config_client import ConfigClient
 from aiovantage.config_client.helpers import get_objects
 
 async with ConfigClient("hostname") as client:
-    loads = get_objects(client, type=["Load", "Button"])
+    loads = get_objects(client, types=["Load", "Button"])
 ```
 
 ### Lookup objects by id, using a helper
 
 ```python
 from aiovantage.config_client import ConfigClient
 from aiovantage.config_client.helpers import get_objects_by_id
```

### Comparing `aiovantage-0.2.0/src/aiovantage/config_client/__init__.py` & `aiovantage-0.2.1/src/aiovantage/config_client/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,33 @@
-"""
-This module provides a client for the Vantage Application Communication Interface (ACI)
-service.
-
-The ACI service is an XML-based RPC service that Design Center uses to communicate
-with Vantage InFusion Controllers. There are a number of "interfaces" exposed, each
-with one or more "methods".
-
-This service allows you to query the "configuration" of a Vantage system, for
-example fetching a list of all the objects, getting a backup of the Design Center
-XML, etc.
-
-The service is exposed on port 2010 (SSL) by default, and on port 2001 (non-SSL) if
-this port has been opened by the firewall on the controller.
-
-The service is discoverable via mDNS as `_aci._tcp.local` and/or
-`_secure_aci._tcp.local`.
-"""
-
-__all__ = ["ConfigClient"]
+"""Client for the Vantage Application Communication Interface (ACI) service."""
 
 import asyncio
 import logging
 import ssl
-import xml.etree.ElementTree as ET
 from types import TracebackType
 from typing import Any, Optional, Tuple, Type, Union
+from xml.etree import ElementTree
 
 from typing_extensions import Self
 from xsdata.formats.dataclass.parsers import XmlParser
 from xsdata.formats.dataclass.parsers.config import ParserConfig
 from xsdata.formats.dataclass.parsers.handlers import XmlEventHandler
 from xsdata.formats.dataclass.serializers import XmlSerializer
 from xsdata.formats.dataclass.serializers.config import SerializerConfig
 
 from .errors import ClientConnectionError, ClientTimeoutError
-from .methods import CallType, Method, ReturnType
+from .methods import Call, Method, Return
 from .methods.login import Login
 
 # Type alias for connections
 Connection = Tuple[asyncio.StreamReader, asyncio.StreamWriter]
 
 
 class ConfigClient:
-    """
-    Client to communicate with the Vantage InFusion "Application Communication
-    Interface" (ACI) service.
+    """Client for the Vantage Application Communication Interface (ACI) service.
 
     This client handles connecting to the ACI service, authenticating, and the
     serialization/deserialization of XML requests and responses.
     """
 
     def __init__(
         self,
@@ -57,16 +36,15 @@
         password: Optional[str] = None,
         *,
         use_ssl: Union[ssl.SSLContext, bool] = True,
         port: Optional[int] = None,
         conn_timeout: float = 5,
         read_timeout: float = 60,
     ):
-        """
-        Initialize the ConfigClient instance.
+        """Initialize the ConfigClient instance.
 
         Args:
             host: The hostname or IP address of the ACI service.
             username: The username to use when authenticating with the ACI service.
             password: The password to use when authenticating with the ACI service.
             use_ssl: Whether to use SSL when connecting to the ACI service.
             port: The port to use when connecting to the ACI service.
@@ -107,45 +85,43 @@
         )
 
         self._serializer = XmlSerializer(
             config=SerializerConfig(xml_declaration=False),
         )
 
     async def __aenter__(self) -> Self:
+        """Return context manager."""
         return self
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> None:
+        """Exit context manager."""
         self.close()
-
         if exc_val:
             raise exc_val
 
     def close(self) -> None:
-        """
-        Close any open connections to the ACI service.
-        """
+        """Close any open connections to the ACI service."""
 
         # Check if connection is already closed
         if self._connection is None or self._connection[1].is_closing():
             return
 
         # Close the connection
         _, writer = self._connection
         writer.close()
 
         self._logger.debug("Connection closed")
 
     async def raw_request(self, interface: str, payload: str) -> str:
-        """
-        Send a plaintext request to the ACI service.
+        """Send a plaintext request to the ACI service.
 
         Args:
             interface: The interface to send the request to
             payload: The request payload string to send
 
         Returns:
             The response payload string
@@ -171,39 +147,60 @@
                 raise ClientTimeoutError from err
             except (OSError, asyncio.IncompleteReadError) as err:
                 raise ClientConnectionError from err
 
             return data.decode()
 
     async def request(
-        self, method: Type[Method[CallType, ReturnType]], params: Any = None
-    ) -> ReturnType:
-        """
-        Marshall a request, send it to the ACI service, and yield a parsed object.
+        self, method_cls: Type[Method[Call, Return]], params: Any = None
+    ) -> Return:
+        """Marshall a request, send it to the ACI service, and yield a parsed object.
 
         Args:
-            method: The method class to use
+            method_cls: The method class to use
             params: The parameters instance to pass to the method
 
         Returns:
             The parsed response object
         """
 
-        request = self._marshall_request(method, params)
+        # Build the method object
+        method = method_cls()
+        method.call = params
+
+        # Render the method object to XML with xsdata
+        request = self._serializer.render(method)
         self._logger.debug(request)
 
         response = await self.raw_request(method.interface, request)
         self._logger.debug(response)
 
-        return self._unmarshall_response(method, response)
+        # Parse the XML doc
+        tree = ElementTree.fromstring(response)
+
+        # Extract the method element from XML doc
+        method_el = tree.find(f"{method_cls.__name__}")
+        if method_el is None:
+            raise ValueError(
+                f"Response from {method_cls.interface} did not contain a "
+                f"<{method_cls.__name__}> element"
+            )
+
+        # Parse the method element with xsdata
+        method = self._parser.parse(method_el, method_cls)
+        if not method.return_value:
+            raise TypeError(
+                f"Response from {method_cls.interface}.{method_cls.__name__}"
+                f"did not contain a return value"
+            )
+
+        return method.return_value
 
     async def _get_connection(self) -> Connection:
-        """
-        Get a connection to the ACI service, authenticating if necessary.
-        """
+        """Get a connection to the ACI service, authenticating if necessary."""
 
         # If we already have a connection, return it
         if self._connection is not None and not self._connection[1].is_closing():
             return self._connection
 
         try:
             # Otherwise, open a new connection
@@ -225,52 +222,14 @@
         except asyncio.TimeoutError as err:
             raise ClientTimeoutError from err
         except OSError as err:
             raise ClientConnectionError from err
 
         return connection
 
-    def _marshall_request(
-        self, method_cls: Type[Method[CallType, ReturnType]], params: Any
-    ) -> str:
-        # Serialize the request to XML using xsdata
-
-        # Build the method object
-        method = method_cls()
-        method.call = params
-
-        # Render the method object to XML with xsdata
-        return self._serializer.render(method)
-
-    def _unmarshall_response(
-        self, method_cls: Type[Method[CallType, ReturnType]], response_str: str
-    ) -> ReturnType:
-        # Deserialize the response from XML using xsdata
-
-        # Parse the XML doc
-        tree = ET.fromstring(response_str)
-
-        # Extract the method element from XML doc
-        method_el = tree.find(f"{method_cls.__name__}")
-        if method_el is None:
-            raise ValueError(
-                f"Response from {method_cls.interface} did not contain a "
-                f"<{method_cls.__name__}> element"
-            )
-
-        # Parse the method element with xsdata
-        method = self._parser.parse(method_el, method_cls)
-        if method.return_value is None or method.return_value == "":
-            raise TypeError(
-                f"Response from {method_cls.interface}.{method_cls.__name__}"
-                f"did not contain a return value"
-            )
-
-        return method.return_value
-
     async def _login(self) -> None:
         # Authenticate if necessary
 
         if self._username is None or self._password is None:
             return
 
         params = Login.Params(user=self._username, password=self._password)
```

### Comparing `aiovantage-0.2.0/src/aiovantage/config_client/methods/configuration/get_filter_results.py` & `aiovantage-0.2.1/src/aiovantage/config_client/methods/configuration/get_filter_results.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,32 @@
+"""IConfiguration.GetFilterResults method definition."""
+
 from dataclasses import dataclass
 from typing import ClassVar, List, Optional
 
+from aiovantage.config_client.methods.types import ObjectChoice
 from aiovantage.config_client.xml_dataclass import xml_element
 
-from .object_choice import ObjectChoice
-
 
 @dataclass
 class GetFilterResults:
+    """IConfiguration.GetFilterResults method definition."""
+
     interface: ClassVar[str] = "IConfiguration"
     call: Optional["GetFilterResults.Params"] = xml_element("call", default=None)
     return_value: Optional["GetFilterResults.Return"] = xml_element(
         "return", default=None
     )
 
     @dataclass
     class Params:
+        """IConfiguration.GetFilterResults method parameters."""
+
         h_filter: int = xml_element("hFilter")
         count: int = xml_element("Count", default=50)
         whole_object: bool = xml_element("WholeObject", default=True)
 
     @dataclass
     class Return:
+        """IConfiguration.GetFilterResults method return value."""
+
         objects: List[ObjectChoice] = xml_element("Object", default_factory=list)
```

### Comparing `aiovantage-0.2.0/src/aiovantage/config_client/methods/configuration/get_object.py` & `aiovantage-0.2.1/src/aiovantage/config_client/methods/configuration/get_object.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,28 @@
+"""IConfiguration.GetObject method definition."""
+
 from dataclasses import dataclass
 from typing import ClassVar, List, Optional
 
+from aiovantage.config_client.methods.types import ObjectChoice
 from aiovantage.config_client.xml_dataclass import xml_element
 
-from .object_choice import ObjectChoice
-
 
 @dataclass
 class GetObject:
+    """IConfiguration.GetObject method definition."""
+
     interface: ClassVar[str] = "IConfiguration"
     call: Optional["GetObject.Params"] = xml_element("call", default=None)
     return_value: Optional["GetObject.Return"] = xml_element("return", default=None)
 
     @dataclass
     class Params:
+        """IConfiguration.GetObject method parameters."""
+
         vids: List[int] = xml_element("VID")
 
     @dataclass
     class Return:
+        """IConfiguration.GetObject method return value."""
+
         objects: List[ObjectChoice] = xml_element("Object", default_factory=list)
```

### Comparing `aiovantage-0.2.0/src/aiovantage/config_client/methods/introspection/get_version.py` & `aiovantage-0.2.1/src/aiovantage/config_client/methods/introspection/get_version.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,23 @@
+"""IIntrospection.GetVersion method definition."""
+
 from dataclasses import dataclass
 from typing import ClassVar, Optional
 
 from aiovantage.config_client.xml_dataclass import xml_element
 
 
 @dataclass
 class GetVersion:
+    """IIntrospection.GetVersion method definition."""
+
     interface: ClassVar[str] = "IIntrospection"
     call: Optional[object] = None
     return_value: Optional["GetVersion.Return"] = xml_element("return", default=None)
 
     @dataclass
     class Return:
+        """IIntrospection.GetVersion method return value."""
+
         kernel: Optional[str] = xml_element("kernel", default=None)
         rootfs: Optional[str] = xml_element("rootfs", default=None)
         app: Optional[str] = xml_element("app", default=None)
```

### Comparing `aiovantage-0.2.0/src/aiovantage/config_client/objects/button.py` & `aiovantage-0.2.1/src/aiovantage/config_client/objects/button.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,35 @@
+"""Button object."""
+
 from dataclasses import dataclass
 
 from aiovantage.config_client.xml_dataclass import xml_element
 
 from .system_object import SystemObject
 
 
 @dataclass
 class Button(SystemObject):
+    """Button object."""
+
     parent_id: int = xml_element("Parent")
     text1: str = xml_element("Text1")
     text2: str = xml_element("Text2")
     up_task_id: int = xml_element("Up")
     down_task_id: int = xml_element("Down")
     hold_task_id: int = xml_element("Hold")
 
     @property
     def has_task(self) -> bool:
+        """Return True if button has a task assigned."""
         return any(
             task_id != 0
             for task_id in (
                 self.up_task_id,
                 self.down_task_id,
                 self.hold_task_id,
             )
         )
 
     def __post_init__(self) -> None:
+        """Post init."""
         self.pressed: bool = False
```

### Comparing `aiovantage-0.2.0/src/aiovantage/config_client/objects/gmem.py` & `aiovantage-0.2.1/src/aiovantage/config_client/objects/gmem.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,68 @@
+"""GMem (variable) object."""
+
 from dataclasses import dataclass
 from typing import Union
 
 from aiovantage.config_client.xml_dataclass import xml_attribute, xml_element, xml_text
 
 from .system_object import SystemObject
 
 
 @dataclass
 class GMem(SystemObject):
+    """GMem (variable) object."""
+
     @dataclass
     class Tag:
+        """GMem tag."""
+
         type: str = xml_text()
         object: bool = xml_attribute("object", default=False)
 
     @dataclass
     class Data:
+        """GMem data."""
+
         fixed: bool = xml_attribute("Fixed", default=False)
 
     data: Data = xml_element("data")
     persistent: bool = xml_element("Persistent")
     tag: Tag = xml_element("Tag")
 
     def __post_init__(self) -> None:
+        """Post init."""
         self.value: Union[int, str, bool, None] = None
 
     @property
     def is_bool(self) -> bool:
+        """Return True if GMem is boolean type."""
         return self.tag.type == "bool"
 
     @property
     def is_str(self) -> bool:
+        """Return True if GMem is string type."""
         return self.tag.type == "Text"
 
     @property
     def is_int(self) -> bool:
+        """Return True if GMem is integer type."""
         return self.tag.type in (
             "Delay",
             "DeviceUnits",
             "Level",
             "Load",
             "Number",
             "Seconds",
             "Task",
             "DegC",
         )
 
     @property
     def is_object_id(self) -> bool:
+        """Return True if GMem is a pointer to an object."""
         return self.tag.object
 
     @property
     def is_fixed(self) -> bool:
+        """Return True if GMem is a fixed point number."""
         return self.data.fixed
```

### Comparing `aiovantage-0.2.0/src/aiovantage/config_client/objects/omni_sensor.py` & `aiovantage-0.2.1/src/aiovantage/config_client/methods/configuration/open_filter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,29 @@
-from dataclasses import dataclass
+"""IConfiguration.OpenFilter method definition."""
 
-from aiovantage.config_client.xml_dataclass import xml_attribute, xml_element
+from dataclasses import dataclass
+from typing import ClassVar, List, Optional
 
-from .sensor import Sensor
+from aiovantage.config_client.xml_dataclass import xml_element
 
 
 @dataclass
-class OmniSensor(Sensor):
+class OpenFilter:
+    """IConfiguration.OpenFilter method definition."""
+
+    interface: ClassVar[str] = "IConfiguration"
+    call: Optional["Params"] = xml_element("call", default=None)
+    return_value: Optional[int] = xml_element("return", default=None)
+
+    # @dataclass
+    # class Filter:
+    #     # TODO: Try using a wrapper
+    #     object_type: List[str] = xml_element("ObjectType")
+
     @dataclass
-    class GetMethodType:
-        @dataclass
-        class Formula:
-            return_type: str = xml_attribute("ReturnType")
-            level_type: str = xml_attribute("LevelType")
-
-        formula: Formula = xml_element("Formula")
-        method: str = xml_element("Method")
-        method_hw: str = xml_element("MethodHW")
-
-    get: GetMethodType = xml_element("Get")
-    parent_id: int = xml_element("Parent")
-
-    @property
-    def is_current_sensor(self) -> bool:
-        return self.model == "Current"
-
-    @property
-    def is_power_sensor(self) -> bool:
-        return self.model == "Power"
-
-    @property
-    def is_temperature_sensor(self) -> bool:
-        return self.model == "Temperature"
+    class Params:
+        """IConfiguration.OpenFilter method parameters."""
+
+        object_types: Optional[List[str]] = xml_element(
+            "ObjectType", wrapper="Objects", default=None
+        )
+        xpath: Optional[str] = xml_element("XPath", default=None)
```

### Comparing `aiovantage-0.2.0/src/aiovantage/config_client/objects/rgb_load.py` & `aiovantage-0.2.1/src/aiovantage/config_client/objects/rgb_load.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,60 +1,59 @@
+"""RGB load object."""
+
 from dataclasses import dataclass
 from enum import Enum
 from typing import Optional, Tuple
 
 from aiovantage.config_client.xml_dataclass import xml_element
 
 from .location_object import LocationObject
 
 # This isn't strictly a Vantage object type, but this helps us avoid
 # code duplication in RGBLoad-like objects.
 
 
 @dataclass
 class RGBLoad(LocationObject):
+    """RGB load object."""
+
     class ColorType(Enum):
+        """Color type."""
+
         RGB = "RGB"
         RGBW = "RGBW"
         HSL = "HSL"
         HSIC = "HSIC"
         CCT = "CCT"
         COLOR_CHANNEL = "Color Channel"
 
     color_type: ColorType = xml_element("ColorType")
     min_temp: int = xml_element("MinTemp")
     max_temp: int = xml_element("MaxTemp")
 
     def __post_init__(self) -> None:
+        """Post init."""
+
         self.hsl: Optional[Tuple[int, int, int]] = None
         self.rgb: Optional[Tuple[int, int, int]] = None
         self.rgbw: Optional[Tuple[int, int, int, int]] = None
         self.level: Optional[int] = None
         self.color_temp: Optional[int] = None
 
     @property
     def is_on(self) -> bool:
-        """
-        Return whether the load is on.
-        """
-
+        """Return True if the load is on."""
         return bool(self.level)
 
     @property
     def is_rgb(self) -> bool:
-        """
-        Return whether the load is an RGB load.
-        """
-
+        """Return True if the load is an RGB(W) load."""
         return self.color_type in (
             RGBLoad.ColorType.RGB,
             RGBLoad.ColorType.RGBW,
             RGBLoad.ColorType.HSL,
         )
 
     @property
     def is_cct(self) -> bool:
-        """
-        Return whether the load is a CCT load.
-        """
-
+        """Return True if the load is a CCT load."""
         return self.color_type == RGBLoad.ColorType.CCT
```

### Comparing `aiovantage-0.2.0/src/aiovantage/config_client/xml_dataclass.py` & `aiovantage-0.2.1/src/aiovantage/config_client/xml_dataclass.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,36 @@
+"""Helper functions for XML dataclasses."""
+
 from dataclasses import field
 from typing import Any, Type
 
 
 def xml_attribute(name: str, **kwargs: Any) -> Any:
+    """Create a dataclass field for an XML attribute."""
     metadata = {}
     metadata.update(kwargs.pop("metadata", {}))
     metadata.update({"name": name, "type": "Attribute"})
 
     return field(metadata=metadata, **kwargs)
 
 
 def xml_element(name: str, **kwargs: Any) -> Any:
+    """Create a dataclass field for an XML element."""
     metadata = {}
     metadata.update(kwargs.pop("metadata", {}))
     metadata.update({"name": name, "type": "Element"})
 
+    if "wrapper" in kwargs:
+        metadata.update({"wrapper": kwargs.pop("wrapper")})
+
     return field(metadata=metadata, **kwargs)
 
 
 def xml_text(**kwargs: Any) -> Any:
+    """Create a dataclass field for an XML text node."""
     metadata = {}
     metadata.update(kwargs.pop("metadata", {}))
     metadata.update({"type": "Text"})
 
     return field(metadata=metadata, **kwargs)
```

### Comparing `aiovantage-0.2.0/src/aiovantage/controllers/base.py` & `aiovantage-0.2.1/src/aiovantage/controllers/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Base controller for Vantage objects."""
+
 import asyncio
 import logging
 from abc import abstractmethod
 from inspect import iscoroutinefunction
 from typing import (
     TYPE_CHECKING,
     Any,
@@ -14,101 +16,102 @@
     Tuple,
     TypeVar,
     Union,
     cast,
 )
 
 from aiovantage.command_client import CommandClient, Event, EventType
-from aiovantage.command_client.helpers import tokenize_response
+from aiovantage.command_client.utils import tokenize_response
 from aiovantage.config_client import ConfigClient
 from aiovantage.config_client.helpers import get_objects
 from aiovantage.config_client.objects import SystemObject
 from aiovantage.events import VantageEvent
 from aiovantage.query import QuerySet
 
 if TYPE_CHECKING:
     from aiovantage import Vantage
 
-T = TypeVar("T", bound="SystemObject")
+T = TypeVar("T", bound=SystemObject)
 
 
 # Types for callbacks for event subscriptions
 EventCallback = Callable[[VantageEvent, T, Dict[str, Any]], None]
 EventSubscription = Tuple[EventCallback[T], Optional[Iterable[VantageEvent]]]
 
 
 class BaseController(QuerySet[T]):
+    """Base controller for Vantage objects."""
+
     # The Vantage object types that this controller handles
     vantage_types: Tuple[str, ...]
 
     def __init__(self, vantage: "Vantage") -> None:
+        """Initialize instance."""
         self._vantage = vantage
         self._items: Dict[int, T] = {}
         self._logger = logging.getLogger(__package__)
         self._subscriptions: List[EventSubscription[T]] = []
         self._id_subscriptions: Dict[int, List[EventSubscription[T]]] = {}
         self._initialized = False
 
         QuerySet.__init__(self, self._items, self.initialize)
 
-    def __getitem__(self, id: int) -> T:
-        return self._items[id]
+        self.__post_init__()
+
+    def __post_init__(self) -> None:
+        """Post initialization hook."""
 
-    def __contains__(self, id: int) -> bool:
-        return id in self._items
+    def __getitem__(self, vid: int) -> T:
+        """Return the object with the given Vantage ID."""
+        return self._items[vid]
+
+    def __contains__(self, vid: int) -> bool:
+        """Return True if the object with the given Vantage ID exists."""
+        return vid in self._items
 
     @property
     def config_client(self) -> ConfigClient:
-        return self._vantage._config_client
+        """Return the config client instance."""
+        return self._vantage.config_client
 
     @property
     def command_client(self) -> CommandClient:
-        return self._vantage._command_client
+        """Return the command client instance."""
+        return self._vantage.command_client
 
     async def initialize(self) -> None:
-        """
-        Initialize a stateless controller by populating the objects it manages.
-        """
-
-        # TODO: Allow reinitalization
+        """Initialize a stateless controller by populating the objects it manages."""
 
         if self._initialized:
             return
 
         await self.fetch_objects()
 
         self._initialized = True
 
     async def fetch_objects(self) -> None:
-        """
-        Fetch all objects managed by this controller.
-        """
-
-        # TODO: Allow re-fetching objects
-        # - fire OBJECT_ADDED events for new objects
-        # - fire OBJECT_REMOVED events for removed objects
+        """Fetch all objects managed by this controller."""
 
-        async for obj in get_objects(self.config_client, type=self.vantage_types):
+        async for obj in get_objects(self.config_client, types=self.vantage_types):
             self._items[obj.id] = cast(T, obj)
             self.emit(VantageEvent.OBJECT_ADDED, cast(T, obj))
 
-        self._logger.info(f"{self.__class__.__name__} fetched objects")
+        self._logger.info("%s fetched objects", self.__class__.__name__)
 
     def subscribe(
         self,
         callback: EventCallback[T],
         id_filter: Union[int, Tuple[int], None] = None,
         event_filter: Union[VantageEvent, Tuple[VantageEvent], None] = None,
     ) -> Callable[[], None]:
-        """
-        Subscribe to status changes for objects managed by this controller.
+        """Subscribe to status changes for objects managed by this controller.
 
         Args:
             callback: The callback to call when an object changes.
-            id_filter: The object IDs to subscribe to, all objects if None.
+            id_filter: The Vantage IDs to subscribe to, all objects if None.
             event_filter: The event types to subscribe to, all events if None.
 
         Returns:
             A function to unsubscribe from the callback.
         """
 
         # Handle single ID filter
@@ -122,87 +125,86 @@
         # Create the subscription
         subscription = (callback, event_filter)
 
         # Add the subscription to the list of subscriptions
         if id_filter is None:
             self._subscriptions.append(subscription)
         else:
-            for id in id_filter:
-                if id not in self._id_subscriptions:
-                    self._id_subscriptions[id] = []
-                self._id_subscriptions[id].append(subscription)
+            for vid in id_filter:
+                if vid not in self._id_subscriptions:
+                    self._id_subscriptions[vid] = []
+                self._id_subscriptions[vid].append(subscription)
 
         # Return a function to unsubscribe
         def unsubscribe() -> None:
             if id_filter is None:
                 self._subscriptions.remove(subscription)
             else:
-                for id in id_filter:  # type: ignore[union-attr]
-                    if id not in self._id_subscriptions:
+                for vid in id_filter:  # type: ignore[union-attr]
+                    if vid not in self._id_subscriptions:
                         continue
-                    self._id_subscriptions[id].remove(subscription)
+                    self._id_subscriptions[vid].remove(subscription)
 
         return unsubscribe
 
     def emit(
         self,
         event_type: VantageEvent,
         obj: T,
-        user_data: Optional[Dict[str, Any]] = None,
+        data: Optional[Dict[str, Any]] = None,
     ) -> None:
-        """
-        Emit an event to subscribers of this controller.
+        """Emit an event to subscribers of this controller.
 
         Args:
             event_type: The type of event to emit.
             obj: The object that the event relates to.
-            user_data: User data to pass to the callback.
+            data: Data to pass to the callback.
         """
 
-        if user_data is None:
-            user_data = {}
+        if data is None:
+            data = {}
 
         # Grab a list of subscribers that care about this object
         subscribers = self._subscriptions + self._id_subscriptions.get(obj.id, [])
         for callback, event_filter in subscribers:
             if event_filter is not None and event_type not in event_filter:
                 continue
 
             if iscoroutinefunction(callback):
-                asyncio.create_task(callback(event_type, obj, user_data))
+                asyncio.create_task(callback(event_type, obj, data))  # noqa: RUF006
             else:
-                callback(event_type, obj, user_data)
+                callback(event_type, obj, data)
 
 
 class StatefulController(BaseController[T]):
+    """Base controller for Vantage objects that have state."""
+
     # Which Vantage status types this controller handles, if any
     status_types: Optional[Tuple[str, ...]] = None
 
     # Should we subscribe to status updates from the event log?
     event_log_status: bool = False
 
     # Which status methods this controller handles from the event log
     event_log_status_methods: Optional[Tuple[str, ...]] = None
 
     @abstractmethod
-    async def fetch_object_state(self, id: int) -> None:
-        ...
+    async def fetch_object_state(self, vid: int) -> None:
+        """Fetch the initial state of an object."""
 
     @abstractmethod
-    def handle_object_update(self, id: int, status: str, args: Sequence[str]) -> None:
-        ...
+    def handle_object_update(self, vid: int, status: str, args: Sequence[str]) -> None:
+        """Handle state changes for an object."""
 
     async def initialize(self) -> None:
-        """
-        Initialize a stateful controller by populating the objects it manages, fetching
-        their initial state, and subscribing to state updates.
-        """
+        """Initialize a stateful controller.
 
-        # TODO: Allow reinitalization
-        # TODO: Allow initializing without subscribing to object state updates
+        Populates the objects it manages, fetches their initial state, and subscribes
+        to state updates.
+        """
 
         if self._initialized:
             return
 
         await self.fetch_objects()
         await self.fetch_full_state()
         await self.subscribe_to_updates()
@@ -210,30 +212,24 @@
         self.command_client.subscribe(
             self._handle_command_client_event, EventType.RECONNECTED
         )
 
         self._initialized = True
 
     async def fetch_full_state(self) -> None:
-        """
-        Fetch the full state of all objects managed by this controller.
-        """
+        """Fetch the full state of all objects managed by this controller."""
 
         await asyncio.gather(
             *[self.fetch_object_state(obj.id) for obj in self._items.values()]
         )
 
-        self._logger.info(f"{self.__class__.__name__} fetched full state")
+        self._logger.info("%s fetched full state", self.__class__.__name__)
 
     async def subscribe_to_updates(self) -> None:
-        """
-        Subscribe to state updates for objects managed by this controller.
-        """
-
-        # TODO: Handle unsubscribe
+        """Subscribe to state updates for objects managed by this controller."""
 
         if not self._items:
             return
 
         # Subscribe to object state updates from the event log
         if self.event_log_status:
             await self.command_client.subscribe_event_log(
@@ -242,39 +238,38 @@
 
         # Subscribe to "STATUS {type}" updates, if this controller cares about them
         if self.status_types:
             await self.command_client.subscribe_status(
                 self._handle_command_client_event, self.status_types
             )
 
-        self._logger.info(f"{self.__class__.__name__} subscribed to updates")
+        self._logger.info("%s subscribed to updates", self.__class__.__name__)
 
-    def update_state(self, id: int, state: Dict[str, Any]) -> None:
-        """
-        Update the state of an object and notify subscribers if it changed
+    def update_state(self, vid: int, state: Dict[str, Any]) -> None:
+        """Update the state of an object and notify subscribers if it changed.
 
         Args:
-            id: The ID of the object to update.
+            vid: The Vantage ID of the object to update.
             state: A dictionary of attributes to update.
         """
 
         # Get the object, skip if it doesn't exist
-        obj = self.get(id)
+        obj = self.get(vid)
         if obj is None:
             return
 
         # Check if any of the attributes changed and update them
         attrs_changed = []
         for key, value in state.items():
             try:
                 if getattr(obj, key) != value:
                     setattr(obj, key, value)
                     attrs_changed.append(key)
             except AttributeError:
-                self._logger.warn(f"Object '{obj.id}' has no attribute '{key}'")
+                self._logger.warning("Object '%d' has no attribute '%s'", obj.id, key)
 
         # Notify subscribers if any attributes changed
         if len(attrs_changed) > 0:
             self.emit(
                 VantageEvent.OBJECT_UPDATED,
                 obj,
                 {"attrs_changed": attrs_changed},
@@ -282,15 +277,15 @@
 
     async def _handle_command_client_event(self, event: Event) -> None:
         # Handle status update events from the command client
 
         if event["tag"] == EventType.STATUS:
             # Handle "STATUS {type}" events
 
-            if event["id"] not in self._items.keys():
+            if event["id"] not in self._items:
                 return
 
             self.handle_object_update(event["id"], event["status_type"], event["args"])
 
         elif event["tag"] == EventType.EVENT_LOG:
             # Handle event log events
 
@@ -298,19 +293,19 @@
             id_str, method, *args = tokenize_response(event["log"])
             if (
                 self.event_log_status_methods
                 and method not in self.event_log_status_methods
             ):
                 return
 
-            id = int(id_str)
-            if id not in self._items.keys():
+            vid = int(id_str)
+            if vid not in self._items:
                 return
 
             # Pass the event to the controller
-            self.handle_object_update(id, method, args)
+            self.handle_object_update(vid, method, args)
 
         elif event["tag"] == EventType.RECONNECTED:
             # Handle reconnect events
 
             # Fetch the full state
             await self.fetch_full_state()
```

### Comparing `aiovantage-0.2.0/src/aiovantage/controllers/blind_groups.py` & `aiovantage-0.2.1/src/aiovantage/controllers/blind_groups.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,27 @@
+"""Controller holding and managing Vantage blind groups."""
+
 from aiovantage.command_client.interfaces import BlindInterface
 from aiovantage.config_client.objects import Blind, BlindGroup
 from aiovantage.query import QuerySet
 
 from .base import BaseController
 
 
 class BlindGroupsController(BaseController[BlindGroup], BlindInterface):
+    """Controller holding and managing Vantage blind groups."""
+
     # Fetch the following object types from Vantage
     vantage_types = ("BlindGroup", "Somfy.URTSI_2_Group_CHILD")
 
-    def blinds(self, id: int) -> QuerySet[Blind]:
+    def blinds(self, vid: int) -> QuerySet[Blind]:
         """Return a queryset of all blinds in this blind group."""
 
-        blind_group = self[id]
+        blind_group = self[vid]
         if blind_group.blind_ids is not None:
             # Some blind groups have a list of blind ids, use that to filter
             return self._vantage.blinds.filter(
-                lambda blind: blind.id in blind_group.blind_ids  # type: ignore
+                lambda blind: blind.id in blind_group.blind_ids  # type: ignore[operator]
             )
-        else:
-            # Otherwise, use the parent_id to filter
-            return self._vantage.blinds.filter(parent_id=blind_group.id)
+
+        # Otherwise, use the parent_id to filter
+        return self._vantage.blinds.filter(parent_id=blind_group.id)
```

### Comparing `aiovantage-0.2.0/src/aiovantage/controllers/blinds.py` & `aiovantage-0.2.1/src/aiovantage/controllers/blinds.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,41 @@
+"""Controller holding and managing Vantage blinds."""
+
 from typing import Any, Dict, Sequence
 
 from typing_extensions import override
 
 from aiovantage.command_client.interfaces import BlindInterface
 from aiovantage.config_client.objects import Blind
 
 from .base import StatefulController
 
 
 class BlindsController(StatefulController[Blind], BlindInterface):
+    """Controller holding and managing Vantage blinds."""
+
     # Fetch the following object types from Vantage
     vantage_types = ("QISBlind", "QubeBlind", "RelayBlind", "Somfy.URTSI_2_Shade_CHILD")
 
     # Subscribe to status updates from the event log for the following methods
     event_log_status = True
     event_log_status_methods = ("Blind.GetPosition",)
 
     @override
-    async def fetch_object_state(self, id: int) -> None:
-        # Fetch initial state of a Blind.
+    async def fetch_object_state(self, vid: int) -> None:
+        """Fetch the initial state of a blind."""
 
-        state: Dict[str, Any] = {}
-        state["position"] = await BlindInterface.get_position(self, id)
+        state: Dict[str, Any] = {
+            "position": await BlindInterface.get_position(self, vid)
+        }
 
-        self.update_state(id, state)
+        self.update_state(vid, state)
 
     @override
-    def handle_object_update(self, id: int, status: str, args: Sequence[str]) -> None:
-        # Handle state changes for a Blind.
+    def handle_object_update(self, vid: int, status: str, args: Sequence[str]) -> None:
+        """Handle state changes for a blind."""
 
         state: Dict[str, Any] = {}
         if status == "Blind.GetPosition":
             state["position"] = BlindInterface.parse_get_position_status(args)
 
-        self.update_state(id, state)
+        self.update_state(vid, state)
```

### Comparing `aiovantage-0.2.0/src/aiovantage/controllers/buttons.py` & `aiovantage-0.2.1/src/aiovantage/controllers/buttons.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,34 @@
+"""Controller holding and managing Vantage buttons."""
+
 from typing import Any, Dict, Sequence
 
 from typing_extensions import override
 
 from aiovantage.command_client.interfaces import ButtonInterface
 from aiovantage.config_client.objects import Button
 
 from .base import StatefulController
 
 
 class ButtonsController(StatefulController[Button], ButtonInterface):
+    """Controller holding and managing Vantage buttons."""
+
     # Fetch the following object types from Vantage
     vantage_types = ("Button",)
 
     # Get status updates from "STATUS BTN"
     status_types = ("BTN",)
 
     @override
-    async def fetch_object_state(self, id: int) -> None:
-        pass  # Buttons are momentary, skip fetching initial state.
+    async def fetch_object_state(self, vid: int) -> None:
+        """Fetch the initial state of a button."""
 
     @override
-    def handle_object_update(self, id: int, status: str, args: Sequence[str]) -> None:
-        # Handle state changes for a Button object.
+    def handle_object_update(self, vid: int, status: str, args: Sequence[str]) -> None:
+        """Handle state changes for a button."""
 
         state: Dict[str, Any] = {}
         if status == "BTN":
             state["pressed"] = ButtonInterface.parse_btn_status(args)
 
-        self.update_state(id, state)
+        self.update_state(vid, state)
```

### Comparing `aiovantage-0.2.0/src/aiovantage/controllers/loads.py` & `aiovantage-0.2.1/src/aiovantage/controllers/loads.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,48 @@
+"""Controller holding and managing Vantage loads."""
+
 from typing import Any, Dict, Sequence
 
 from typing_extensions import override
 
 from aiovantage.command_client.interfaces import LoadInterface
 from aiovantage.config_client.objects import Load
 from aiovantage.query import QuerySet
 
 from .base import StatefulController
 
 
 class LoadsController(StatefulController[Load], LoadInterface):
+    """Controller holding and managing Vantage loads."""
+
     # Fetch the following object types from Vantage
     vantage_types = ("Load",)
 
     # Get status updates from "STATUS LOAD"
     status_types = ("LOAD",)
 
     @override
-    async def fetch_object_state(self, id: int) -> None:
-        # Fetch initial state of a Load.
+    async def fetch_object_state(self, vid: int) -> None:
+        """Fetch the initial state of a load."""
 
-        state: Dict[str, Any] = {}
-        state["level"] = await LoadInterface.get_level(self, id)
+        state: Dict[str, Any] = {
+            "level": await LoadInterface.get_level(self, vid),
+        }
 
-        self.update_state(id, state)
+        self.update_state(vid, state)
 
     @override
-    def handle_object_update(self, id: int, status: str, args: Sequence[str]) -> None:
-        # Handle state changes for a Load.
+    def handle_object_update(self, vid: int, status: str, args: Sequence[str]) -> None:
+        """Handle state changes for a load."""
 
         state: Dict[str, Any] = {}
         if status == "LOAD":
             state["level"] = LoadInterface.parse_load_status(args)
 
-        self.update_state(id, state)
+        self.update_state(vid, state)
 
     @property
     def on(self) -> QuerySet[Load]:
         """Return a queryset of all loads that are turned on."""
 
         return self.filter(lambda load: load.is_on)
```

### Comparing `aiovantage-0.2.0/src/aiovantage/controllers/omni_sensors.py` & `aiovantage-0.2.1/src/aiovantage/controllers/omni_sensors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,64 +1,70 @@
+"""Controller holding and managing Vantage omni sensors."""
+
 from decimal import Decimal
 from typing import Any, Dict, Sequence, Union
 
 from typing_extensions import override
 
 from aiovantage.config_client.objects import OmniSensor
 from aiovantage.controllers.base import StatefulController
 
 
 class OmniSensorsController(StatefulController[OmniSensor]):
+    """Controller holding and managing Vantage omni sensors."""
+
     # Fetch the following object types from Vantage
     vantage_types = ("OmniSensor",)
 
     # Subscribe to status updates from the event log
     event_log_status = True
 
     @override
-    async def fetch_object_state(self, id: int) -> None:
-        # Fetch initial state of an OmniSensor.
+    async def fetch_object_state(self, vid: int) -> None:
+        """Fetch the initial state of an omni sensor."""
 
-        state: Dict[str, Any] = {}
-        state["level"] = await self.get_level(id)
+        state: Dict[str, Any] = {
+            "level": await self.get_level(vid),
+        }
 
-        self.update_state(id, state)
+        self.update_state(vid, state)
 
     @override
-    def handle_object_update(self, id: int, method: str, args: Sequence[str]) -> None:
-        # Handle state changes for an OmniSensor.
+    def handle_object_update(self, vid: int, status: str, args: Sequence[str]) -> None:
+        """Handle state changes for an omni sensor."""
 
-        omni_sensor: OmniSensor = self[id]
-        if method != omni_sensor.get.method:
+        omni_sensor: OmniSensor = self[vid]
+        if status != omni_sensor.get.method:
             return
 
-        state: Dict[str, Any] = {}
-        state["level"] = self.parse_get_level_status(omni_sensor, args)
+        state: Dict[str, Any] = {
+            "level": self.parse_get_level_status(omni_sensor, args),
+        }
 
-        self.update_state(id, state)
+        self.update_state(vid, state)
 
-    async def get_level(self, id: int, cached: bool = False) -> Union[int, Decimal]:
-        """
-        Get the level of an OmniSensor.
+    async def get_level(self, vid: int, cached: bool = False) -> Union[int, Decimal]:
+        """Get the level of an OmniSensor.
 
         Args:
-            id: The ID of the sensor.
+            vid: The ID of the sensor.
+            cached: Whether to use the cached value or fetch a new one.
 
         Returns:
             The level of the sensor.
         """
 
-        omni_sensor: OmniSensor = self[id]
+        omni_sensor: OmniSensor = self[vid]
 
         # Figure out which get method to use, hardware or software (cached)
         method = omni_sensor.get.method if cached else omni_sensor.get.method_hw
 
         # INVOKE <id> <method>
         # -> R:INVOKE <id> <value> <method>
-        response = await self.command_client.command("INVOKE", id, method)
+        response = await self.command_client.command("INVOKE", vid, method)
 
         # Convert the level to the correct type
         if omni_sensor.get.formula.return_type == "fixed":
             level = Decimal(response.args[1])
             if omni_sensor.get.formula.level_type == "fixed":
                 return level
             else:
@@ -70,15 +76,15 @@
             else:
                 return int(level)
 
     @classmethod
     def parse_get_level_status(
         cls, omni_sensor: OmniSensor, args: Sequence[str]
     ) -> Union[int, Decimal]:
-        # Parse an OmniSensor "GetLevel" event, eg. "PowerSensor.GetPower"
+        """Parse an OmniSensor 'GetLevel' event, eg. 'PowerSensor.GetPower'."""
 
         # ELLOG STATUS ON
         # -> EL: <id> <method> <value>
         # STATUS ADD <id>
         # -> S:STATUS <id> <method> <value>
         level = Decimal(args[0]) / 1000
         if omni_sensor.get.formula.level_type == "fixed":
```

### Comparing `aiovantage-0.2.0/src/aiovantage/controllers/rgb_loads.py` & `aiovantage-0.2.1/src/aiovantage/controllers/rgb_loads.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Controller holding and managing Vantage RGB loads."""
+
 from typing import Any, Dict, List, Optional, Sequence, Tuple
 
 from typing_extensions import override
 
 from aiovantage.command_client.interfaces import (
     ColorTemperatureInterface,
     LoadInterface,
@@ -15,107 +17,110 @@
 
 class RGBLoadsController(
     StatefulController[RGBLoad],
     LoadInterface,
     RGBLoadInterface,
     ColorTemperatureInterface,
 ):
+    """Controller holding and managing Vantage RGB loads."""
+
     # Fetch the following object types from Vantage
     vantage_types = ("Vantage.DGColorLoad", "Vantage.DDGColorLoad")
 
     # Subscribe to status updates from the event log for the following methods
     event_log_status = True
     event_log_status_methods = (
         "RGBLoad.GetHSL",
         "RGBLoad.GetRGB",
         "RGBLoad.GetRGBW",
         "ColorTemperature.Get",
         "Load.GetLevel",
     )
 
-    async def initialize(self) -> None:
+    def __post_init__(self) -> None:
+        """Post initialization hook."""
         self._temp_color_map: Dict[int, List[int]] = {}
-        return await super().initialize()
 
     @override
-    async def fetch_object_state(self, id: int) -> None:
-        # Fetch initial state of an RGBLoad.
+    async def fetch_object_state(self, vid: int) -> None:
+        """Fetch the initial state of an RGB load."""
 
-        rgb_load: RGBLoad = self[id]
-        state: Dict[str, Any] = {}
-        state["level"] = await LoadInterface.get_level(self, id)
+        state: Dict[str, Any] = {
+            "level": await LoadInterface.get_level(self, vid),
+        }
 
+        rgb_load: RGBLoad = self[vid]
         if rgb_load.is_rgb:
-            state["hsl"] = await RGBLoadInterface.get_hsl(self, id)
-            state["rgb"] = await RGBLoadInterface.get_rgb(self, id)
-            state["rgbw"] = await RGBLoadInterface.get_rgbw(self, id)
+            state["hsl"] = await RGBLoadInterface.get_hsl(self, vid)
+            state["rgb"] = await RGBLoadInterface.get_rgb(self, vid)
+            state["rgbw"] = await RGBLoadInterface.get_rgbw(self, vid)
 
         if rgb_load.is_cct:
             state["color_temp"] = await ColorTemperatureInterface.get_color_temp(
-                self, id
+                self, vid
             )
 
-        self.update_state(id, state)
+        self.update_state(vid, state)
 
     @override
-    def handle_object_update(self, id: int, method: str, args: Sequence[str]) -> None:
-        # Handle state changes for an RGBLoad.
+    def handle_object_update(self, vid: int, status: str, args: Sequence[str]) -> None:
+        """Handle state changes for an RGB load."""
 
-        rgb_load: RGBLoad = self[id]
+        rgb_load: RGBLoad = self[vid]
         state: Dict[str, Any] = {}
-        if method == "Load.GetLevel":
+        if status == "Load.GetLevel":
             state["level"] = LoadInterface.parse_get_level_status(args)
 
-        elif method == "RGBLoad.GetHSL" and rgb_load.is_rgb:
+        elif status == "RGBLoad.GetHSL" and rgb_load.is_rgb:
             channel, value = RGBLoadInterface.parse_color_channel_status(args)
-            if hsl := self._build_color_from_channels(id, channel, value, 3):
+            if hsl := self._build_color_from_channels(vid, channel, value, 3):
                 state["hsl"] = hsl
 
-        elif method == "RGBLoad.GetRGB" and rgb_load.is_rgb:
+        elif status == "RGBLoad.GetRGB" and rgb_load.is_rgb:
             channel, value = RGBLoadInterface.parse_color_channel_status(args)
-            if rgb := self._build_color_from_channels(id, channel, value, 3):
+            if rgb := self._build_color_from_channels(vid, channel, value, 3):
                 state["rgb"] = rgb
 
-        elif method == "RGBLoad.GetRGBW" and rgb_load.is_rgb:
+        elif status == "RGBLoad.GetRGBW" and rgb_load.is_rgb:
             channel, value = RGBLoadInterface.parse_color_channel_status(args)
-            if rgbw := self._build_color_from_channels(id, channel, value, 4):
+            if rgbw := self._build_color_from_channels(vid, channel, value, 4):
                 state["rgbw"] = rgbw
 
-        elif method == "ColorTemperature.Get" and rgb_load.is_cct:
+        elif status == "ColorTemperature.Get" and rgb_load.is_cct:
             state["color_temp"] = ColorTemperatureInterface.parse_get_status(args)
 
-        self.update_state(id, state)
+        self.update_state(vid, state)
 
     @property
     def on(self) -> QuerySet[RGBLoad]:
         """Return a queryset of all RGB loads that are turned on."""
 
         return self.filter(lambda load: load.is_on)
 
     @property
     def off(self) -> QuerySet[RGBLoad]:
         """Return a queryset of all RGB loads that are turned off."""
 
         return self.filter(lambda load: not load.is_on)
 
     def _build_color_from_channels(
-        self, id: int, channel: int, value: int, num_channels: int
+        self, vid: int, channel: int, value: int, num_channels: int
     ) -> Optional[Tuple[int, ...]]:
         # Build a color from a series of channel value events. We need to store
         # partially constructed colors in memory, since updates come separately for
         # each channel.
 
         # Ignore updates for channels we don't care about
         if channel < 0 or channel >= num_channels:
             return None
 
         # Store the channel value in the temp color map
-        self._temp_color_map.setdefault(id, num_channels * [0])
-        self._temp_color_map[id][channel] = value
+        self._temp_color_map.setdefault(vid, num_channels * [0])
+        self._temp_color_map[vid][channel] = value
 
         # If we have all the channels, build and return the color
         if channel == num_channels - 1:
-            color = tuple(self._temp_color_map[id])
-            del self._temp_color_map[id]
+            color = tuple(self._temp_color_map[vid])
+            del self._temp_color_map[vid]
             return color
 
         return None
```

### Comparing `aiovantage-0.2.0/src/aiovantage/controllers/tasks.py` & `aiovantage-0.2.1/src/aiovantage/controllers/tasks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,45 @@
+"""Controller holding and managing Vantage tasks."""
+
 from typing import Any, Dict, Sequence
 
 from typing_extensions import override
 
 from aiovantage.command_client.interfaces import TaskInterface
 from aiovantage.config_client.objects import Task
 
 from .base import StatefulController
 
 
 class TasksController(StatefulController[Task], TaskInterface):
+    """Controller holding and managing Vantage tasks."""
+
     # Fetch the following object types from Vantage
     vantage_types = ("Task",)
 
     # Subscribe to status updates from the event log for the following methods
     event_log_status = True
     event_log_status_methods = ("Task.IsRunning", "Task.GetState")
 
     @override
-    async def fetch_object_state(self, id: int) -> None:
-        # Fetch initial state of a Task.
+    async def fetch_object_state(self, vid: int) -> None:
+        """Fetch the initial state of a task."""
 
-        state: Dict[str, Any] = {}
-        state["is_running"] = await TaskInterface.is_running(self, id)
-        state["state"] = await TaskInterface.get_state(self, id)
+        state: Dict[str, Any] = {
+            "is_running": await TaskInterface.is_running(self, vid),
+            "state": await TaskInterface.get_state(self, vid),
+        }
 
-        self.update_state(id, state)
+        self.update_state(vid, state)
 
     @override
-    def handle_object_update(self, id: int, method: str, args: Sequence[str]) -> None:
-        # Handle state changes for a Task.
+    def handle_object_update(self, vid: int, status: str, args: Sequence[str]) -> None:
+        """Handle state changes for a task."""
 
         state: Dict[str, Any] = {}
-        if method == "Task.IsRunning":
+        if status == "Task.IsRunning":
             state["is_running"] = TaskInterface.parse_is_running_status(args)
 
-        elif method == "Task.GetState":
+        elif status == "Task.GetState":
             state["state"] = TaskInterface.parse_get_state_status(args)
 
-        self.update_state(id, state)
+        self.update_state(vid, state)
```

