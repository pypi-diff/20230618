# Comparing `tmp/unitelabs_connector_framework-0.1.0.tar.gz` & `tmp/unitelabs_connector_framework-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitelabs_connector_framework-0.1.0.tar", max compression
+gzip compressed data, was "unitelabs_connector_framework-0.1.1.tar", max compression
```

## Comparing `unitelabs_connector_framework-0.1.0.tar` & `unitelabs_connector_framework-0.1.1.tar`

### file list

```diff
@@ -1,64 +1,68 @@
--rw-r--r--   0        0        0     1069 2023-06-11 17:51:12.165815 unitelabs_connector_framework-0.1.0/LICENSE
--rw-r--r--   0        0        0     3027 2023-06-14 08:43:30.504479 unitelabs_connector_framework-0.1.0/README.md
--rw-r--r--   0        0        0     2061 2023-06-14 09:33:37.670004 unitelabs_connector_framework-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      168 2023-06-14 09:28:37.005175 unitelabs_connector_framework-0.1.0/src/unitelabs/__init__.py
--rw-r--r--   0        0        0     1235 2023-06-10 08:57:12.994027 unitelabs_connector_framework-0.1.0/src/unitelabs/cli.py
--rw-r--r--   0        0        0      454 2023-06-10 08:19:00.892129 unitelabs_connector_framework-0.1.0/src/unitelabs/config.py
--rw-r--r--   0        0        0     1648 2023-06-10 09:14:45.123602 unitelabs_connector_framework-0.1.0/src/unitelabs/connector.py
--rw-r--r--   0        0        0     4429 2023-06-08 12:21:47.568189 unitelabs_connector_framework-0.1.0/src/unitelabs/features/core/lock_controller/LockController-v2_0.proto
--rw-r--r--   0        0        0     5518 2023-06-08 12:21:47.572050 unitelabs_connector_framework-0.1.0/src/unitelabs/features/core/lock_controller/LockController-v2_0.sila.xml
--rw-r--r--   0        0        0      321 2023-06-08 12:21:47.573953 unitelabs_connector_framework-0.1.0/src/unitelabs/features/core/lock_controller/__init__.py
--rw-r--r--   0        0        0     3755 2023-06-14 09:35:35.940054 unitelabs_connector_framework-0.1.0/src/unitelabs/features/core/lock_controller/lock_controller.py
--rw-r--r--   0        0        0     3375 2023-06-10 08:57:13.031414 unitelabs_connector_framework-0.1.0/src/unitelabs/features/core/lock_controller/lock_controller_base.py
--rw-r--r--   0        0        0     7109 2023-06-08 12:01:08.346706 unitelabs_connector_framework-0.1.0/src/unitelabs/features/core/sila_service/SiLAService-v1_0.proto
--rw-r--r--   0        0        0     7902 2023-06-08 11:43:41.586033 unitelabs_connector_framework-0.1.0/src/unitelabs/features/core/sila_service/SiLAService-v1_0.sila.xml
--rw-r--r--   0        0        0      111 2023-06-08 12:01:41.537455 unitelabs_connector_framework-0.1.0/src/unitelabs/features/core/sila_service/__init__.py
--rw-r--r--   0        0        0     5626 2023-06-11 10:26:41.921309 unitelabs_connector_framework-0.1.0/src/unitelabs/features/core/sila_service/sila_service.py
--rw-r--r--   0        0        0    14833 2023-06-09 11:02:35.803576 unitelabs_connector_framework-0.1.0/src/unitelabs/features/robot/labware_transfer_manipulator_controller/LabwareTransferManipulatorController-v1_0.proto
--rw-r--r--   0        0        0    15654 2023-06-08 18:31:02.343015 unitelabs_connector_framework-0.1.0/src/unitelabs/features/robot/labware_transfer_manipulator_controller/LabwareTransferManipulatorController-v1_0.sila.xml
--rw-r--r--   0        0        0      407 2023-06-14 09:34:31.175200 unitelabs_connector_framework-0.1.0/src/unitelabs/features/robot/labware_transfer_manipulator_controller/__init__.py
--rw-r--r--   0        0        0    11116 2023-06-14 09:34:39.277307 unitelabs_connector_framework-0.1.0/src/unitelabs/features/robot/labware_transfer_manipulator_controller/labware_transfer_manipulator_controller_base.py
--rw-r--r--   0        0        0     8041 2023-06-08 15:58:40.585326 unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/basic_data_types_test/BasicDataTypesTest-v1_0.proto
--rw-r--r--   0        0        0     8279 2023-06-08 15:58:37.034762 unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/basic_data_types_test/BasicDataTypesTest-v1_0.sila.xml
--rw-r--r--   0        0        0       88 2023-06-08 15:56:50.422431 unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/basic_data_types_test/__init__.py
--rw-r--r--   0        0        0     5190 2023-06-11 10:29:43.300577 unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/basic_data_types_test/basic_data_types_test.py
--rw-r--r--   0        0        0     2891 2023-06-03 08:08:38.591011 unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/observable_command_test/ObservableCommandTest-v1_0.proto
--rw-r--r--   0        0        0     2846 2023-06-10 09:38:31.720888 unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/observable_command_test/ObservableCommandTest-v1_0.sila.xml
--rw-r--r--   0        0        0       96 2023-05-07 08:13:10.387701 unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/observable_command_test/__init__.py
--rw-r--r--   0        0        0     2383 2023-06-11 10:54:49.863161 unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/observable_command_test/observable_command_test.py
--rw-r--r--   0        0        0     2146 2023-06-10 08:52:51.902499 unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/observable_property_test/ObservablePropertyTest-v1_0.proto
--rw-r--r--   0        0        0     1820 2023-06-10 08:52:10.669356 unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/observable_property_test/ObservablePropertyTest-v1_0.sila.xml
--rw-r--r--   0        0        0       99 2023-06-10 08:56:35.314045 unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/observable_property_test/__init__.py
--rw-r--r--   0        0        0     1625 2023-06-10 09:22:10.087811 unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/observable_property_test/observable_property_test.py
--rw-r--r--   0        0        0     3147 2023-06-08 15:10:15.841233 unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/unobservable_command_test/UnobservableCommandTest-v1_0.proto
--rw-r--r--   0        0        0     4090 2023-06-08 15:12:39.575863 unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/unobservable_command_test/UnobservableCommandTest-v1_0.sila.xml
--rw-r--r--   0        0        0      102 2023-06-08 15:57:00.405056 unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/unobservable_command_test/__init__.py
--rw-r--r--   0        0        0     2006 2023-06-11 10:22:39.326761 unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/unobservable_command_test/unobservable_command_test.py
--rw-r--r--   0        0        0     1465 2023-06-08 14:12:11.083908 unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/unobservable_property_test/UnobservablePropertyTest-v1_0.proto
--rw-r--r--   0        0        0     1250 2023-06-08 14:13:49.773291 unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/unobservable_property_test/UnobservablePropertyTest-v1_0.sila.xml
--rw-r--r--   0        0        0      105 2023-06-08 14:14:24.590503 unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/unobservable_property_test/__init__.py
--rw-r--r--   0        0        0      725 2023-06-10 08:57:12.994633 unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/unobservable_property_test/unobservable_property_test.py
--rw-r--r--   0        0        0     4157 2023-06-03 08:14:35.038359 unitelabs_connector_framework-0.1.0/src/unitelabs/features/weighing/weighing_service/WeighingService-v1_0.proto
--rw-r--r--   0        0        0     8446 2023-05-07 08:33:49.313366 unitelabs_connector_framework-0.1.0/src/unitelabs/features/weighing/weighing_service/WeighingService-v1_0.sila.xml
--rw-r--r--   0        0        0       85 2023-06-03 08:14:35.038563 unitelabs_connector_framework-0.1.0/src/unitelabs/features/weighing/weighing_service/__init__.py
--rw-r--r--   0        0        0     2839 2023-06-11 10:28:57.427186 unitelabs_connector_framework-0.1.0/src/unitelabs/features/weighing/weighing_service/weighing_service.py
--rw-r--r--   0        0        0      541 2023-06-06 19:24:50.656991 unitelabs_connector_framework-0.1.0/src/unitelabs/logging.py
--rw-r--r--   0        0        0        0 2023-06-12 08:59:43.667279 unitelabs_connector_framework-0.1.0/src/unitelabs/py.typed
--rw-r--r--   0        0        0     1121 2023-06-11 10:27:23.555778 unitelabs_connector_framework-0.1.0/src/unitelabs/sila/__init__.py
--rw-r--r--   0        0        0        0 2023-06-11 09:33:36.508770 unitelabs_connector_framework-0.1.0/src/unitelabs/sila/commands/__init__.py
--rw-r--r--   0        0        0      425 2023-06-11 09:59:16.304398 unitelabs_connector_framework-0.1.0/src/unitelabs/sila/commands/intermediate.py
--rw-r--r--   0        0        0     1188 2023-06-11 10:57:11.616229 unitelabs_connector_framework-0.1.0/src/unitelabs/sila/commands/intermediate_response.py
--rw-r--r--   0        0        0     1455 2023-06-11 10:57:13.280572 unitelabs_connector_framework-0.1.0/src/unitelabs/sila/commands/response.py
--rw-r--r--   0        0        0      698 2023-06-11 09:59:11.555574 unitelabs_connector_framework-0.1.0/src/unitelabs/sila/commands/status.py
--rw-r--r--   0        0        0      704 2023-06-09 10:50:39.626785 unitelabs_connector_framework-0.1.0/src/unitelabs/sila/data_type_definition.py
--rw-r--r--   0        0        0      651 2023-06-07 12:03:48.878896 unitelabs_connector_framework-0.1.0/src/unitelabs/sila/defined_execution_error.py
--rw-r--r--   0        0        0     1249 2023-06-09 08:43:40.105340 unitelabs_connector_framework-0.1.0/src/unitelabs/sila/feature.py
--rw-r--r--   0        0        0      675 2023-06-08 14:06:19.120898 unitelabs_connector_framework-0.1.0/src/unitelabs/sila/metadata.py
--rw-r--r--   0        0        0     5027 2023-06-14 09:35:17.579080 unitelabs_connector_framework-0.1.0/src/unitelabs/sila/observable_command.py
--rw-r--r--   0        0        0     1516 2023-06-10 08:48:26.073694 unitelabs_connector_framework-0.1.0/src/unitelabs/sila/observable_property.py
--rw-r--r--   0        0        0     3486 2023-06-09 08:24:50.416452 unitelabs_connector_framework-0.1.0/src/unitelabs/sila/parser.py
--rw-r--r--   0        0        0     3940 2023-06-11 10:31:42.067642 unitelabs_connector_framework-0.1.0/src/unitelabs/sila/unobservable_command.py
--rw-r--r--   0        0        0     1377 2023-06-07 12:04:17.401494 unitelabs_connector_framework-0.1.0/src/unitelabs/sila/unobservable_property.py
--rw-r--r--   0        0        0     2314 2023-06-06 20:10:09.131560 unitelabs_connector_framework-0.1.0/src/unitelabs/sila/utils.py
--rw-r--r--   0        0        0      307 2023-04-04 16:41:46.514608 unitelabs_connector_framework-0.1.0/src/unitelabs/utils.py
--rw-r--r--   0        0        0     4487 1970-01-01 00:00:00.000000 unitelabs_connector_framework-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-11 17:51:12.165815 unitelabs_connector_framework-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3026 2023-06-18 10:34:53.733054 unitelabs_connector_framework-0.1.1/README.md
+-rw-r--r--   0        0        0     2061 2023-06-18 10:34:53.742212 unitelabs_connector_framework-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-06-14 09:28:37.005175 unitelabs_connector_framework-0.1.1/src/unitelabs/__init__.py
+-rw-r--r--   0        0        0     1235 2023-06-10 08:57:12.994027 unitelabs_connector_framework-0.1.1/src/unitelabs/cli.py
+-rw-r--r--   0        0        0      454 2023-06-10 08:19:00.892129 unitelabs_connector_framework-0.1.1/src/unitelabs/config.py
+-rw-r--r--   0        0        0     1751 2023-06-18 10:34:53.743165 unitelabs_connector_framework-0.1.1/src/unitelabs/connector.py
+-rw-r--r--   0        0        0     4429 2023-06-08 12:21:47.568189 unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/lock_controller/LockController-v2_0.proto
+-rw-r--r--   0        0        0     5518 2023-06-08 12:21:47.572050 unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/lock_controller/LockController-v2_0.sila.xml
+-rw-r--r--   0        0        0      321 2023-06-08 12:21:47.573953 unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/lock_controller/__init__.py
+-rw-r--r--   0        0        0     3755 2023-06-14 09:35:35.940054 unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/lock_controller/lock_controller.py
+-rw-r--r--   0        0        0     3375 2023-06-10 08:57:13.031414 unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/lock_controller/lock_controller_base.py
+-rw-r--r--   0        0        0     7109 2023-06-08 12:01:08.346706 unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/sila_service/SiLAService-v1_0.proto
+-rw-r--r--   0        0        0     7902 2023-06-08 11:43:41.586033 unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/sila_service/SiLAService-v1_0.sila.xml
+-rw-r--r--   0        0        0      111 2023-06-08 12:01:41.537455 unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/sila_service/__init__.py
+-rw-r--r--   0        0        0     5936 2023-06-18 10:26:38.076224 unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/sila_service/sila_service.py
+-rw-r--r--   0        0        0       93 2023-06-18 10:34:53.743616 unitelabs_connector_framework-0.1.1/src/unitelabs/features/examples/greeting_provider/__init__.py
+-rw-r--r--   0        0        0     1029 2023-06-18 10:34:53.744341 unitelabs_connector_framework-0.1.1/src/unitelabs/features/examples/greeting_provider/greeting_provider_base.py
+-rw-r--r--   0        0        0       84 2023-06-18 10:34:53.744719 unitelabs_connector_framework-0.1.1/src/unitelabs/features/examples/timer_provider/__init__.py
+-rw-r--r--   0        0        0     1838 2023-06-18 10:34:53.745303 unitelabs_connector_framework-0.1.1/src/unitelabs/features/examples/timer_provider/timer_provider_base.py
+-rw-r--r--   0        0        0    14833 2023-06-09 11:02:35.803576 unitelabs_connector_framework-0.1.1/src/unitelabs/features/robot/labware_transfer_manipulator_controller/LabwareTransferManipulatorController-v1_0.proto
+-rw-r--r--   0        0        0    15654 2023-06-08 18:31:02.343015 unitelabs_connector_framework-0.1.1/src/unitelabs/features/robot/labware_transfer_manipulator_controller/LabwareTransferManipulatorController-v1_0.sila.xml
+-rw-r--r--   0        0        0      407 2023-06-14 09:34:31.175200 unitelabs_connector_framework-0.1.1/src/unitelabs/features/robot/labware_transfer_manipulator_controller/__init__.py
+-rw-r--r--   0        0        0    11116 2023-06-14 09:34:39.277307 unitelabs_connector_framework-0.1.1/src/unitelabs/features/robot/labware_transfer_manipulator_controller/labware_transfer_manipulator_controller_base.py
+-rw-r--r--   0        0        0     8041 2023-06-08 15:58:40.585326 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/basic_data_types_test/BasicDataTypesTest-v1_0.proto
+-rw-r--r--   0        0        0     8279 2023-06-08 15:58:37.034762 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/basic_data_types_test/BasicDataTypesTest-v1_0.sila.xml
+-rw-r--r--   0        0        0       88 2023-06-08 15:56:50.422431 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/basic_data_types_test/__init__.py
+-rw-r--r--   0        0        0     5190 2023-06-11 10:29:43.300577 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/basic_data_types_test/basic_data_types_test.py
+-rw-r--r--   0        0        0     2891 2023-06-03 08:08:38.591011 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/observable_command_test/ObservableCommandTest-v1_0.proto
+-rw-r--r--   0        0        0     2846 2023-06-10 09:38:31.720888 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/observable_command_test/ObservableCommandTest-v1_0.sila.xml
+-rw-r--r--   0        0        0       96 2023-05-07 08:13:10.387701 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/observable_command_test/__init__.py
+-rw-r--r--   0        0        0     2383 2023-06-11 10:54:49.863161 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/observable_command_test/observable_command_test.py
+-rw-r--r--   0        0        0     2146 2023-06-10 08:52:51.902499 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/observable_property_test/ObservablePropertyTest-v1_0.proto
+-rw-r--r--   0        0        0     1820 2023-06-10 08:52:10.669356 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/observable_property_test/ObservablePropertyTest-v1_0.sila.xml
+-rw-r--r--   0        0        0       99 2023-06-10 08:56:35.314045 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/observable_property_test/__init__.py
+-rw-r--r--   0        0        0     1625 2023-06-10 09:22:10.087811 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/observable_property_test/observable_property_test.py
+-rw-r--r--   0        0        0     3147 2023-06-08 15:10:15.841233 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/unobservable_command_test/UnobservableCommandTest-v1_0.proto
+-rw-r--r--   0        0        0     4090 2023-06-08 15:12:39.575863 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/unobservable_command_test/UnobservableCommandTest-v1_0.sila.xml
+-rw-r--r--   0        0        0      102 2023-06-08 15:57:00.405056 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/unobservable_command_test/__init__.py
+-rw-r--r--   0        0        0     2006 2023-06-11 10:22:39.326761 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/unobservable_command_test/unobservable_command_test.py
+-rw-r--r--   0        0        0     1465 2023-06-08 14:12:11.083908 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/unobservable_property_test/UnobservablePropertyTest-v1_0.proto
+-rw-r--r--   0        0        0     1250 2023-06-08 14:13:49.773291 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/unobservable_property_test/UnobservablePropertyTest-v1_0.sila.xml
+-rw-r--r--   0        0        0      105 2023-06-08 14:14:24.590503 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/unobservable_property_test/__init__.py
+-rw-r--r--   0        0        0      725 2023-06-10 08:57:12.994633 unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/unobservable_property_test/unobservable_property_test.py
+-rw-r--r--   0        0        0     4157 2023-06-03 08:14:35.038359 unitelabs_connector_framework-0.1.1/src/unitelabs/features/weighing/weighing_service/WeighingService-v1_0.proto
+-rw-r--r--   0        0        0     8446 2023-05-07 08:33:49.313366 unitelabs_connector_framework-0.1.1/src/unitelabs/features/weighing/weighing_service/WeighingService-v1_0.sila.xml
+-rw-r--r--   0        0        0       85 2023-06-03 08:14:35.038563 unitelabs_connector_framework-0.1.1/src/unitelabs/features/weighing/weighing_service/__init__.py
+-rw-r--r--   0        0        0     2839 2023-06-11 10:28:57.427186 unitelabs_connector_framework-0.1.1/src/unitelabs/features/weighing/weighing_service/weighing_service.py
+-rw-r--r--   0        0        0      541 2023-06-06 19:24:50.656991 unitelabs_connector_framework-0.1.1/src/unitelabs/logging.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:59:43.667279 unitelabs_connector_framework-0.1.1/src/unitelabs/py.typed
+-rw-r--r--   0        0        0     1121 2023-06-11 10:27:23.555778 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-11 09:33:36.508770 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/commands/__init__.py
+-rw-r--r--   0        0        0      425 2023-06-11 09:59:16.304398 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/commands/intermediate.py
+-rw-r--r--   0        0        0     1188 2023-06-11 10:57:11.616229 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/commands/intermediate_response.py
+-rw-r--r--   0        0        0     1455 2023-06-11 10:57:13.280572 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/commands/response.py
+-rw-r--r--   0        0        0      698 2023-06-11 09:59:11.555574 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/commands/status.py
+-rw-r--r--   0        0        0      704 2023-06-09 10:50:39.626785 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/data_type_definition.py
+-rw-r--r--   0        0        0      651 2023-06-07 12:03:48.878896 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/defined_execution_error.py
+-rw-r--r--   0        0        0     1249 2023-06-09 08:43:40.105340 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/feature.py
+-rw-r--r--   0        0        0      675 2023-06-08 14:06:19.120898 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/metadata.py
+-rw-r--r--   0        0        0     5027 2023-06-14 09:35:17.579080 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/observable_command.py
+-rw-r--r--   0        0        0     1516 2023-06-10 08:48:26.073694 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/observable_property.py
+-rw-r--r--   0        0        0     3486 2023-06-09 08:24:50.416452 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/parser.py
+-rw-r--r--   0        0        0     3940 2023-06-11 10:31:42.067642 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/unobservable_command.py
+-rw-r--r--   0        0        0     1377 2023-06-07 12:04:17.401494 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/unobservable_property.py
+-rw-r--r--   0        0        0     2314 2023-06-06 20:10:09.131560 unitelabs_connector_framework-0.1.1/src/unitelabs/sila/utils.py
+-rw-r--r--   0        0        0      307 2023-04-04 16:41:46.514608 unitelabs_connector_framework-0.1.1/src/unitelabs/utils.py
+-rw-r--r--   0        0        0     4486 1970-01-01 00:00:00.000000 unitelabs_connector_framework-0.1.1/PKG-INFO
```

### Comparing `unitelabs_connector_framework-0.1.0/LICENSE` & `unitelabs_connector_framework-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/README.md` & `unitelabs_connector_framework-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 ```
 $ pip install unitelabs-connector-framework
 ```
 
 ## Documentation
 
-Start by then exploring the UniteLabs Connector Framework [documentation](docs/01_intro.md), dive into the
+Start by then exploring the UniteLabs Connector Framework [documentation](docs/0.index.md), dive into the
 [core concepts](docs/3.concepts/1.feature.md), and try our [tutorials](docs/2.tutorial/index.md) for some hands-on learning.
 
 ## Contribute
 
 There are many ways to contribute to this project and our vision of freely and readily available interfaces for laboratory systems.
 
 - Check out our [contribution guidelines](docs/6.community/1.contributing.md) to help us improve this project
```

### Comparing `unitelabs_connector_framework-0.1.0/pyproject.toml` & `unitelabs_connector_framework-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unitelabs-connector-framework"
-version = "0.1.0"
+version = "0.1.1"
 description = "A framework to build connectors based on the SiLA 2 standard specification."
 license = "MIT"
 authors = ["UniteLabs AG <developers+connector@unitelabs.ch>"]
 readme = "README.md"
 homepage = "https://unitelabs.ch"
 repository = "https://gitlab.com/unitelabs/connector-framework"
 documentation = "https://gitlab.com/unitelabs/connector-framework/-/tree/main/docs/"
@@ -32,15 +32,15 @@
 [tool.poetry.scripts]
 connector = 'unitelabs.cli:cli'
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = "8.1.3"
 pydantic = { version = "1.10.9", extras = ["dotenv"] }
-unitelabs-sila = "0.1.0"
+unitelabs-sila = "0.1.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
 isort = "5.12.0"
 pylint = "2.17.4"
 pytest = "7.3.1"
 pytest-asyncio = "0.21.0"
```

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/cli.py` & `unitelabs_connector_framework-0.1.1/src/unitelabs/cli.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/connector.py` & `unitelabs_connector_framework-0.1.1/src/unitelabs/connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,28 +13,30 @@
 class Connector:
     """Main app"""
 
     def __init__(self, config: typing.Optional[dict] = None):
         self.__config = Config.parse_obj(config or {})
 
         self._sila_server = server.Server(config=self.config.sila_server)
+        self.logger.info(self._sila_server)
         self._broadcaster = discovery.Broadcaster(self._sila_server)
         self._cloud_server_endpoint = cloud_connector.CloudServerEndpoint(
             self._sila_server, self.config.cloud_server_endpoint
         )
 
         self.register(SiLAService())
 
     def register(self, feature: server.Feature):
         """Register a new feature to this driver"""
+        self.logger.debug("Added feature: %s", feature)
         self._sila_server.add_feature(feature)
 
     async def start(self):
         """Start running this driver"""
-        self.logger.info("Starting driver...")
+        self.logger.info("Starting connector...")
 
         await asyncio.gather(
             asyncio.create_task(self._sila_server.start()),
             asyncio.create_task(self._broadcaster.start()),
             asyncio.create_task(self._cloud_server_endpoint.start()),
         )
```

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/features/core/lock_controller/LockController-v2_0.proto` & `unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/lock_controller/LockController-v2_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/features/core/lock_controller/LockController-v2_0.sila.xml` & `unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/lock_controller/LockController-v2_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/features/core/lock_controller/lock_controller.py` & `unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/lock_controller/lock_controller.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/features/core/lock_controller/lock_controller_base.py` & `unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/lock_controller/lock_controller_base.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/features/core/sila_service/SiLAService-v1_0.proto` & `unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/sila_service/SiLAService-v1_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/features/core/sila_service/SiLAService-v1_0.sila.xml` & `unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/sila_service/SiLAService-v1_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/features/core/sila_service/sila_service.py` & `unitelabs_connector_framework-0.1.1/src/unitelabs/features/core/sila_service/sila_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,19 +47,22 @@
         """
         Get the Feature Definition of an implemented Feature by its fully qualified Feature Identifier.
         This command has no preconditions and no further dependencies and can be called at any time.
 
         .. parameter:: The fully qualified Feature identifier for which the Feature definition shall be retrieved.
         .. return:: The Feature definition in XML format (according to the Feature Definition Schema).
         """
-        features: dict[str, sila.Feature] = getattr(self.server, "features", {})
-        if feature_identifier not in features:
+        identifier = sila.identifiers.FullyQualifiedFeatureIdentifier.parse(feature_identifier)
+        features: dict[sila.identifiers.FullyQualifiedFeatureIdentifier, sila.Feature] = getattr(
+            self.server, "features", {}
+        )
+        if identifier not in features:
             raise UnimplementedFeature()
 
-        feature = features[feature_identifier]
+        feature = features[identifier]
 
         return fdl_parser.serialize_feature(feature=feature)
 
     @sila.UnobservableCommand()
     def set_server_name(self, server_name: typing.Annotated[str, sila.constraints.MaximalLength(255)]) -> None:
         """
         Sets a human readable name to the Server Name Property.Command has no preconditions and
@@ -133,8 +136,11 @@
     ) -> list[
         typing.Annotated[str, sila.constraints.FullyQualifiedIdentifier(sila.constraints.Identifier.FEATURE_IDENTIFIER)]
     ]:
         """
         Returns a list of fully qualified Feature identifiers of all implemented Features of this SiLA Server.
         This list SHOULD remain the same throughout the lifetime of the SiLA Server.
         """
-        return list(getattr(self.server, "features").keys())
+        features: dict[sila.identifiers.FullyQualifiedFeatureIdentifier, sila.Feature] = getattr(
+            self.server, "features", {}
+        )
+        return [str(feature_identifier) for feature_identifier in features]
```

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/features/robot/labware_transfer_manipulator_controller/LabwareTransferManipulatorController-v1_0.proto` & `unitelabs_connector_framework-0.1.1/src/unitelabs/features/robot/labware_transfer_manipulator_controller/LabwareTransferManipulatorController-v1_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/features/robot/labware_transfer_manipulator_controller/LabwareTransferManipulatorController-v1_0.sila.xml` & `unitelabs_connector_framework-0.1.1/src/unitelabs/features/robot/labware_transfer_manipulator_controller/LabwareTransferManipulatorController-v1_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/features/robot/labware_transfer_manipulator_controller/labware_transfer_manipulator_controller_base.py` & `unitelabs_connector_framework-0.1.1/src/unitelabs/features/robot/labware_transfer_manipulator_controller/labware_transfer_manipulator_controller_base.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/basic_data_types_test/BasicDataTypesTest-v1_0.proto` & `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/basic_data_types_test/BasicDataTypesTest-v1_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/basic_data_types_test/BasicDataTypesTest-v1_0.sila.xml` & `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/basic_data_types_test/BasicDataTypesTest-v1_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/basic_data_types_test/basic_data_types_test.py` & `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/basic_data_types_test/basic_data_types_test.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/observable_command_test/ObservableCommandTest-v1_0.proto` & `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/observable_command_test/ObservableCommandTest-v1_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/observable_command_test/ObservableCommandTest-v1_0.sila.xml` & `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/observable_command_test/ObservableCommandTest-v1_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/observable_command_test/observable_command_test.py` & `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/observable_command_test/observable_command_test.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/observable_property_test/ObservablePropertyTest-v1_0.proto` & `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/observable_property_test/ObservablePropertyTest-v1_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/observable_property_test/ObservablePropertyTest-v1_0.sila.xml` & `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/observable_property_test/ObservablePropertyTest-v1_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/observable_property_test/observable_property_test.py` & `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/observable_property_test/observable_property_test.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/unobservable_command_test/UnobservableCommandTest-v1_0.proto` & `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/unobservable_command_test/UnobservableCommandTest-v1_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/unobservable_command_test/UnobservableCommandTest-v1_0.sila.xml` & `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/unobservable_command_test/UnobservableCommandTest-v1_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/unobservable_command_test/unobservable_command_test.py` & `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/unobservable_command_test/unobservable_command_test.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/unobservable_property_test/UnobservablePropertyTest-v1_0.proto` & `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/unobservable_property_test/UnobservablePropertyTest-v1_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/unobservable_property_test/UnobservablePropertyTest-v1_0.sila.xml` & `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/unobservable_property_test/UnobservablePropertyTest-v1_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/features/test/unobservable_property_test/unobservable_property_test.py` & `unitelabs_connector_framework-0.1.1/src/unitelabs/features/test/unobservable_property_test/unobservable_property_test.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/features/weighing/weighing_service/WeighingService-v1_0.proto` & `unitelabs_connector_framework-0.1.1/src/unitelabs/features/weighing/weighing_service/WeighingService-v1_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/features/weighing/weighing_service/WeighingService-v1_0.sila.xml` & `unitelabs_connector_framework-0.1.1/src/unitelabs/features/weighing/weighing_service/WeighingService-v1_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/features/weighing/weighing_service/weighing_service.py` & `unitelabs_connector_framework-0.1.1/src/unitelabs/features/weighing/weighing_service/weighing_service.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/logging.py` & `unitelabs_connector_framework-0.1.1/src/unitelabs/logging.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/sila/__init__.py` & `unitelabs_connector_framework-0.1.1/src/unitelabs/sila/__init__.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/sila/commands/intermediate_response.py` & `unitelabs_connector_framework-0.1.1/src/unitelabs/sila/commands/intermediate_response.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/sila/commands/response.py` & `unitelabs_connector_framework-0.1.1/src/unitelabs/sila/commands/response.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/sila/commands/status.py` & `unitelabs_connector_framework-0.1.1/src/unitelabs/sila/commands/status.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/sila/data_type_definition.py` & `unitelabs_connector_framework-0.1.1/src/unitelabs/sila/data_type_definition.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/sila/defined_execution_error.py` & `unitelabs_connector_framework-0.1.1/src/unitelabs/sila/defined_execution_error.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/sila/feature.py` & `unitelabs_connector_framework-0.1.1/src/unitelabs/sila/feature.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/sila/metadata.py` & `unitelabs_connector_framework-0.1.1/src/unitelabs/sila/metadata.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/sila/observable_command.py` & `unitelabs_connector_framework-0.1.1/src/unitelabs/sila/observable_command.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/sila/observable_property.py` & `unitelabs_connector_framework-0.1.1/src/unitelabs/sila/observable_property.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/sila/parser.py` & `unitelabs_connector_framework-0.1.1/src/unitelabs/sila/parser.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/sila/unobservable_command.py` & `unitelabs_connector_framework-0.1.1/src/unitelabs/sila/unobservable_command.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/sila/unobservable_property.py` & `unitelabs_connector_framework-0.1.1/src/unitelabs/sila/unobservable_property.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/src/unitelabs/sila/utils.py` & `unitelabs_connector_framework-0.1.1/src/unitelabs/sila/utils.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.0/PKG-INFO` & `unitelabs_connector_framework-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitelabs-connector-framework
-Version: 0.1.0
+Version: 0.1.1
 Summary: A framework to build connectors based on the SiLA 2 standard specification.
 Home-page: https://unitelabs.ch
 License: MIT
 Keywords: SiLA 2,laboratory,automation,connectivity
 Author: UniteLabs AG
 Author-email: developers+connector@unitelabs.ch
 Requires-Python: >=3.9,<4.0
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: click (==8.1.3)
 Requires-Dist: pydantic[dotenv] (==1.10.9)
-Requires-Dist: unitelabs-sila (==0.1.0)
+Requires-Dist: unitelabs-sila (==0.1.1)
 Project-URL: Bug Tracker, https://gitlab.com/unitelabs/connector-framework/-/issues
 Project-URL: Documentation, https://gitlab.com/unitelabs/connector-framework/-/tree/main/docs/
 Project-URL: Repository, https://gitlab.com/unitelabs/connector-framework
 Description-Content-Type: text/markdown
 
 # UniteLabs Connector Framework
 
@@ -59,15 +59,15 @@
 
 ```
 $ pip install unitelabs-connector-framework
 ```
 
 ## Documentation
 
-Start by then exploring the UniteLabs Connector Framework [documentation](docs/01_intro.md), dive into the
+Start by then exploring the UniteLabs Connector Framework [documentation](docs/0.index.md), dive into the
 [core concepts](docs/3.concepts/1.feature.md), and try our [tutorials](docs/2.tutorial/index.md) for some hands-on learning.
 
 ## Contribute
 
 There are many ways to contribute to this project and our vision of freely and readily available interfaces for laboratory systems.
 
 - Check out our [contribution guidelines](docs/6.community/1.contributing.md) to help us improve this project
```

