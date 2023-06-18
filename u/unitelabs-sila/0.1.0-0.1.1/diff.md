# Comparing `tmp/unitelabs_sila-0.1.0.tar.gz` & `tmp/unitelabs_sila-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitelabs_sila-0.1.0.tar", max compression
+gzip compressed data, was "unitelabs_sila-0.1.1.tar", max compression
```

## Comparing `unitelabs_sila-0.1.0.tar` & `unitelabs_sila-0.1.1.tar`

### file list

```diff
@@ -1,117 +1,117 @@
--rw-r--r--   0        0        0     1069 2023-06-08 22:13:58.281937 unitelabs_sila-0.1.0/LICENSE
--rw-r--r--   0        0        0     2127 2023-06-14 06:12:15.664226 unitelabs_sila-0.1.0/README.md
--rw-r--r--   0        0        0     1945 2023-06-14 06:50:29.251606 unitelabs_sila-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      106 2023-06-14 07:16:21.186838 unitelabs_sila-0.1.0/src/sila/__init__.py
--rw-r--r--   0        0        0      146 2023-06-08 22:13:58.442811 unitelabs_sila-0.1.0/src/sila/cloud_connector/__init__.py
--rw-r--r--   0        0        0    15437 2023-06-11 21:57:12.510011 unitelabs_sila-0.1.0/src/sila/cloud_connector/cloud_server_endpoint.py
--rw-r--r--   0        0        0    10246 2023-06-10 15:36:21.353326 unitelabs_sila-0.1.0/src/sila/cloud_connector/messages.py
--rw-r--r--   0        0        0      592 2023-06-10 15:37:02.130746 unitelabs_sila-0.1.0/src/sila/commands/__init__.py
--rw-r--r--   0        0        0      946 2023-06-11 21:57:12.510981 unitelabs_sila-0.1.0/src/sila/commands/command.py
--rw-r--r--   0        0        0     1147 2023-06-11 21:57:12.512348 unitelabs_sila-0.1.0/src/sila/commands/command_confirmation.py
--rw-r--r--   0        0        0     4583 2023-06-11 21:57:12.516356 unitelabs_sila-0.1.0/src/sila/commands/command_execution.py
--rw-r--r--   0        0        0     3046 2023-06-11 21:57:12.517685 unitelabs_sila-0.1.0/src/sila/commands/command_execution_info.py
--rw-r--r--   0        0        0      453 2023-06-11 21:57:12.518337 unitelabs_sila-0.1.0/src/sila/commands/command_execution_uuid.py
--rw-r--r--   0        0        0      616 2023-06-11 21:57:12.521234 unitelabs_sila-0.1.0/src/sila/commands/observable_command.py
--rw-r--r--   0        0        0      390 2023-06-11 21:57:12.522401 unitelabs_sila-0.1.0/src/sila/commands/unobservable_command.py
--rw-r--r--   0        0        0     1231 2023-06-13 17:34:19.443118 unitelabs_sila-0.1.0/src/sila/constraints/__init__.py
--rw-r--r--   0        0        0      625 2023-06-11 21:57:12.523714 unitelabs_sila-0.1.0/src/sila/constraints/allowed_types.py
--rw-r--r--   0        0        0      478 2023-06-14 05:05:30.931848 unitelabs_sila-0.1.0/src/sila/constraints/constraint.py
--rw-r--r--   0        0        0      921 2023-06-08 08:41:46.740250 unitelabs_sila-0.1.0/src/sila/constraints/content_type.py
--rw-r--r--   0        0        0      889 2023-06-03 09:51:05.606924 unitelabs_sila-0.1.0/src/sila/constraints/element_count.py
--rw-r--r--   0        0        0     1555 2023-06-14 05:05:30.932520 unitelabs_sila-0.1.0/src/sila/constraints/fully_qualified_identifier.py
--rw-r--r--   0        0        0      934 2023-06-11 21:57:12.525011 unitelabs_sila-0.1.0/src/sila/constraints/length.py
--rw-r--r--   0        0        0      904 2023-06-03 09:51:05.610073 unitelabs_sila-0.1.0/src/sila/constraints/maximal_element_count.py
--rw-r--r--   0        0        0      888 2023-06-03 09:55:31.158596 unitelabs_sila-0.1.0/src/sila/constraints/maximal_exclusive.py
--rw-r--r--   0        0        0      907 2023-06-03 09:55:36.776856 unitelabs_sila-0.1.0/src/sila/constraints/maximal_inclusive.py
--rw-r--r--   0        0        0      985 2023-06-14 05:03:54.580670 unitelabs_sila-0.1.0/src/sila/constraints/maximal_length.py
--rw-r--r--   0        0        0      899 2023-06-03 09:51:05.614671 unitelabs_sila-0.1.0/src/sila/constraints/minimal_element_count.py
--rw-r--r--   0        0        0      893 2023-06-03 09:55:34.058872 unitelabs_sila-0.1.0/src/sila/constraints/minimal_exclusive.py
--rw-r--r--   0        0        0      909 2023-06-03 09:55:38.301758 unitelabs_sila-0.1.0/src/sila/constraints/minimal_inclusive.py
--rw-r--r--   0        0        0      994 2023-06-03 09:51:05.622353 unitelabs_sila-0.1.0/src/sila/constraints/minimal_length.py
--rw-r--r--   0        0        0      623 2023-06-14 05:05:30.933163 unitelabs_sila-0.1.0/src/sila/constraints/pattern.py
--rw-r--r--   0        0        0      665 2023-06-08 08:53:44.725620 unitelabs_sila-0.1.0/src/sila/constraints/schema.py
--rw-r--r--   0        0        0      726 2023-06-03 09:55:39.422718 unitelabs_sila-0.1.0/src/sila/constraints/set.py
--rw-r--r--   0        0        0     1602 2023-06-08 08:29:13.185856 unitelabs_sila-0.1.0/src/sila/constraints/unit.py
--rw-r--r--   0        0        0      144 2023-06-11 21:57:12.526082 unitelabs_sila-0.1.0/src/sila/core/__init__.py
--rw-r--r--   0        0        0     2770 2023-06-11 21:57:12.526764 unitelabs_sila-0.1.0/src/sila/core/feature.py
--rw-r--r--   0        0        0     1709 2023-06-11 21:57:12.527474 unitelabs_sila-0.1.0/src/sila/core/handler.py
--rw-r--r--   0        0        0     2971 2023-06-14 05:05:30.933915 unitelabs_sila-0.1.0/src/sila/core/server.py
--rw-r--r--   0        0        0      769 2023-06-13 15:55:13.097999 unitelabs_sila-0.1.0/src/sila/data_types/__init__.py
--rw-r--r--   0        0        0     1102 2023-06-04 19:54:04.417061 unitelabs_sila-0.1.0/src/sila/data_types/any.py
--rw-r--r--   0        0        0     1053 2023-06-07 19:30:07.082139 unitelabs_sila-0.1.0/src/sila/data_types/basic_type.py
--rw-r--r--   0        0        0     1354 2023-06-04 20:29:24.951615 unitelabs_sila-0.1.0/src/sila/data_types/binary.py
--rw-r--r--   0        0        0      771 2023-06-04 19:48:34.281597 unitelabs_sila-0.1.0/src/sila/data_types/boolean.py
--rw-r--r--   0        0        0     1336 2023-06-07 19:30:18.487002 unitelabs_sila-0.1.0/src/sila/data_types/constrained.py
--rw-r--r--   0        0        0      867 2023-06-07 19:30:26.689597 unitelabs_sila-0.1.0/src/sila/data_types/data_type.py
--rw-r--r--   0        0        0     2077 2023-06-09 11:21:36.627376 unitelabs_sila-0.1.0/src/sila/data_types/data_type_definition.py
--rw-r--r--   0        0        0     1965 2023-06-04 19:47:40.030909 unitelabs_sila-0.1.0/src/sila/data_types/date.py
--rw-r--r--   0        0        0     1130 2023-06-04 19:46:07.096305 unitelabs_sila-0.1.0/src/sila/data_types/duration.py
--rw-r--r--   0        0        0      743 2023-06-05 10:53:18.827154 unitelabs_sila-0.1.0/src/sila/data_types/integer.py
--rw-r--r--   0        0        0     1286 2023-06-07 19:30:34.932708 unitelabs_sila-0.1.0/src/sila/data_types/list.py
--rw-r--r--   0        0        0      760 2023-06-04 19:38:15.675710 unitelabs_sila-0.1.0/src/sila/data_types/real.py
--rw-r--r--   0        0        0     1147 2023-06-08 22:12:52.848122 unitelabs_sila-0.1.0/src/sila/data_types/string.py
--rw-r--r--   0        0        0     4271 2023-06-09 10:45:44.390563 unitelabs_sila-0.1.0/src/sila/data_types/structure.py
--rw-r--r--   0        0        0     1948 2023-06-04 19:45:25.161612 unitelabs_sila-0.1.0/src/sila/data_types/time.py
--rw-r--r--   0        0        0     2533 2023-06-04 19:44:26.791814 unitelabs_sila-0.1.0/src/sila/data_types/timestamp.py
--rw-r--r--   0        0        0     1250 2023-06-04 19:42:37.697579 unitelabs_sila-0.1.0/src/sila/data_types/timezone.py
--rw-r--r--   0        0        0      659 2023-06-04 19:42:08.651066 unitelabs_sila-0.1.0/src/sila/data_types/void.py
--rw-r--r--   0        0        0      164 2023-06-08 20:52:53.907366 unitelabs_sila-0.1.0/src/sila/datetime/__init__.py
--rw-r--r--   0        0        0     2262 2023-06-08 22:13:58.286982 unitelabs_sila-0.1.0/src/sila/datetime/date.py
--rw-r--r--   0        0        0       64 2023-06-08 22:13:58.443800 unitelabs_sila-0.1.0/src/sila/discovery/__init__.py
--rw-r--r--   0        0        0     1785 2023-06-08 22:13:58.444125 unitelabs_sila-0.1.0/src/sila/discovery/broadcaster.py
--rw-r--r--   0        0        0      446 2023-06-05 20:09:27.499133 unitelabs_sila-0.1.0/src/sila/errors/__init__.py
--rw-r--r--   0        0        0     2508 2023-06-05 20:11:46.397290 unitelabs_sila-0.1.0/src/sila/errors/defined_execution_error.py
--rw-r--r--   0        0        0     2005 2023-06-05 20:08:43.148208 unitelabs_sila-0.1.0/src/sila/errors/framework_error.py
--rw-r--r--   0        0        0     1808 2023-06-05 20:10:27.279204 unitelabs_sila-0.1.0/src/sila/errors/sila_error.py
--rw-r--r--   0        0        0      647 2023-06-05 20:10:05.335814 unitelabs_sila-0.1.0/src/sila/errors/sila_exception.py
--rw-r--r--   0        0        0      908 2023-06-05 20:10:02.365590 unitelabs_sila-0.1.0/src/sila/errors/undefined_execution_error.py
--rw-r--r--   0        0        0     1282 2023-06-05 20:09:59.865569 unitelabs_sila-0.1.0/src/sila/errors/validation_error.py
--rw-r--r--   0        0        0      941 2023-06-09 06:33:45.337996 unitelabs_sila-0.1.0/src/sila/fdl_parser/__init__.py
--rw-r--r--   0        0        0     1684 2023-06-08 11:09:33.254085 unitelabs_sila-0.1.0/src/sila/fdl_parser/serialize_command.py
--rw-r--r--   0        0        0     5095 2023-06-08 22:13:58.338287 unitelabs_sila-0.1.0/src/sila/fdl_parser/serialize_constraint.py
--rw-r--r--   0        0        0     3182 2023-06-08 10:47:41.040745 unitelabs_sila-0.1.0/src/sila/fdl_parser/serialize_data_type.py
--rw-r--r--   0        0        0      752 2023-06-09 06:36:56.248348 unitelabs_sila-0.1.0/src/sila/fdl_parser/serialize_data_type_definition.py
--rw-r--r--   0        0        0      586 2023-06-08 10:46:24.525760 unitelabs_sila-0.1.0/src/sila/fdl_parser/serialize_defined_execution_error.py
--rw-r--r--   0        0        0      418 2023-06-08 09:45:35.011949 unitelabs_sila-0.1.0/src/sila/fdl_parser/serialize_defined_execution_error_list.py
--rw-r--r--   0        0        0      245 2023-06-09 18:55:45.433970 unitelabs_sila-0.1.0/src/sila/fdl_parser/serialize_description.py
--rw-r--r--   0        0        0     2442 2023-06-09 06:45:11.260470 unitelabs_sila-0.1.0/src/sila/fdl_parser/serialize_feature.py
--rw-r--r--   0        0        0      852 2023-06-08 22:13:58.339752 unitelabs_sila-0.1.0/src/sila/fdl_parser/serialize_metadata.py
--rw-r--r--   0        0        0      944 2023-06-08 11:09:39.444072 unitelabs_sila-0.1.0/src/sila/fdl_parser/serialize_property.py
--rw-r--r--   0        0        0      760 2023-06-08 10:43:45.918520 unitelabs_sila-0.1.0/src/sila/fdl_parser/serialize_sila_element.py
--rw-r--r--   0        0        0     1211 2023-06-04 15:05:41.890867 unitelabs_sila-0.1.0/src/sila/identifiers/__init__.py
--rw-r--r--   0        0        0      921 2023-06-05 16:09:47.952981 unitelabs_sila-0.1.0/src/sila/identifiers/command_identifier.py
--rw-r--r--   0        0        0     1010 2023-06-05 16:09:56.289383 unitelabs_sila-0.1.0/src/sila/identifiers/command_parameter_identifier.py
--rw-r--r--   0        0        0      997 2023-06-05 16:10:04.394751 unitelabs_sila-0.1.0/src/sila/identifiers/command_response_identifier.py
--rw-r--r--   0        0        0     1037 2023-06-05 16:10:14.088142 unitelabs_sila-0.1.0/src/sila/identifiers/custom_data_type_identifier.py
--rw-r--r--   0        0        0     1139 2023-06-05 16:10:21.623765 unitelabs_sila-0.1.0/src/sila/identifiers/defined_execution_error_identifier.py
--rw-r--r--   0        0        0     1543 2023-06-05 16:10:28.377507 unitelabs_sila-0.1.0/src/sila/identifiers/feature_identifier.py
--rw-r--r--   0        0        0      929 2023-06-05 20:26:49.403019 unitelabs_sila-0.1.0/src/sila/identifiers/identifier.py
--rw-r--r--   0        0        0     1177 2023-06-05 16:10:35.608508 unitelabs_sila-0.1.0/src/sila/identifiers/intermediate_command_response_identifier.py
--rw-r--r--   0        0        0      923 2023-06-05 16:10:42.048691 unitelabs_sila-0.1.0/src/sila/identifiers/metadata_identifier.py
--rw-r--r--   0        0        0      925 2023-06-05 16:10:48.185705 unitelabs_sila-0.1.0/src/sila/identifiers/property_identifier.py
--rw-r--r--   0        0        0       55 2023-06-08 22:13:58.340262 unitelabs_sila-0.1.0/src/sila/metadata/__init__.py
--rw-r--r--   0        0        0     2850 2023-06-08 22:13:58.340758 unitelabs_sila-0.1.0/src/sila/metadata/metadata.py
--rw-r--r--   0        0        0      224 2023-06-05 14:34:27.247039 unitelabs_sila-0.1.0/src/sila/properties/__init__.py
--rw-r--r--   0        0        0      395 2023-06-05 18:28:34.990277 unitelabs_sila-0.1.0/src/sila/properties/observable_property.py
--rw-r--r--   0        0        0     1313 2023-06-05 18:39:52.745622 unitelabs_sila-0.1.0/src/sila/properties/property.py
--rw-r--r--   0        0        0      389 2023-06-05 18:29:02.534670 unitelabs_sila-0.1.0/src/sila/properties/unobservable_property.py
--rw-r--r--   0        0        0      550 2023-06-05 05:48:33.521128 unitelabs_sila-0.1.0/src/sila/protobuf/__init__.py
--rw-r--r--   0        0        0      441 2023-06-03 09:48:32.882854 unitelabs_sila-0.1.0/src/sila/protobuf/decode_error.py
--rw-r--r--   0        0        0        0 2023-06-12 07:48:23.932059 unitelabs_sila-0.1.0/src/sila/py.typed
--rw-r--r--   0        0        0      670 2023-06-08 22:13:58.341251 unitelabs_sila-0.1.0/src/sila/server/__init__.py
--rw-r--r--   0        0        0     1832 2023-06-09 08:20:59.706922 unitelabs_sila-0.1.0/src/sila/server/feature.py
--rw-r--r--   0        0        0      862 2023-06-07 10:04:20.415702 unitelabs_sila-0.1.0/src/sila/server/handler.py
--rw-r--r--   0        0        0     1347 2023-06-12 08:58:29.013915 unitelabs_sila-0.1.0/src/sila/server/metadata.py
--rw-r--r--   0        0        0     8143 2023-06-11 10:59:07.585836 unitelabs_sila-0.1.0/src/sila/server/observable_command.py
--rw-r--r--   0        0        0     2889 2023-06-08 22:13:58.343109 unitelabs_sila-0.1.0/src/sila/server/observable_property.py
--rw-r--r--   0        0        0     8181 2023-06-14 05:05:30.934576 unitelabs_sila-0.1.0/src/sila/server/server.py
--rw-r--r--   0        0        0     2468 2023-06-08 22:13:58.343791 unitelabs_sila-0.1.0/src/sila/server/unobservable_command.py
--rw-r--r--   0        0        0     2602 2023-06-08 22:13:58.344296 unitelabs_sila-0.1.0/src/sila/server/unobservable_property.py
--rw-r--r--   0        0        0      222 2023-06-14 05:05:30.935366 unitelabs_sila-0.1.0/src/sila/validators/__init__.py
--rw-r--r--   0        0        0      963 2023-06-14 05:05:30.935791 unitelabs_sila-0.1.0/src/sila/validators/display_name.py
--rw-r--r--   0        0        0     1192 2023-06-14 05:05:30.936233 unitelabs_sila-0.1.0/src/sila/validators/domain.py
--rw-r--r--   0        0        0     1335 2023-06-14 05:05:30.936778 unitelabs_sila-0.1.0/src/sila/validators/identifier.py
--rw-r--r--   0        0        0     1129 2023-06-14 05:05:30.937160 unitelabs_sila-0.1.0/src/sila/validators/uuid.py
--rw-r--r--   0        0        0     1347 2023-06-14 05:05:30.937529 unitelabs_sila-0.1.0/src/sila/validators/validator.py
--rw-r--r--   0        0        0     2901 2023-06-14 05:05:30.937980 unitelabs_sila-0.1.0/src/sila/validators/version.py
--rw-r--r--   0        0        0     3558 1970-01-01 00:00:00.000000 unitelabs_sila-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-08 22:13:58.281937 unitelabs_sila-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2038 2023-06-14 08:42:29.964140 unitelabs_sila-0.1.1/README.md
+-rw-r--r--   0        0        0     1945 2023-06-18 10:00:10.921604 unitelabs_sila-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      106 2023-06-14 07:16:21.186838 unitelabs_sila-0.1.1/src/sila/__init__.py
+-rw-r--r--   0        0        0      146 2023-06-08 22:13:58.442811 unitelabs_sila-0.1.1/src/sila/cloud_connector/__init__.py
+-rw-r--r--   0        0        0    17225 2023-06-16 16:19:03.239630 unitelabs_sila-0.1.1/src/sila/cloud_connector/cloud_server_endpoint.py
+-rw-r--r--   0        0        0    10246 2023-06-10 15:36:21.353326 unitelabs_sila-0.1.1/src/sila/cloud_connector/messages.py
+-rw-r--r--   0        0        0      592 2023-06-10 15:37:02.130746 unitelabs_sila-0.1.1/src/sila/commands/__init__.py
+-rw-r--r--   0        0        0      946 2023-06-16 13:18:07.658640 unitelabs_sila-0.1.1/src/sila/commands/command.py
+-rw-r--r--   0        0        0     1147 2023-06-11 21:57:12.512348 unitelabs_sila-0.1.1/src/sila/commands/command_confirmation.py
+-rw-r--r--   0        0        0     4709 2023-06-16 16:19:20.467543 unitelabs_sila-0.1.1/src/sila/commands/command_execution.py
+-rw-r--r--   0        0        0     3046 2023-06-11 21:57:12.517685 unitelabs_sila-0.1.1/src/sila/commands/command_execution_info.py
+-rw-r--r--   0        0        0      453 2023-06-11 21:57:12.518337 unitelabs_sila-0.1.1/src/sila/commands/command_execution_uuid.py
+-rw-r--r--   0        0        0      616 2023-06-11 21:57:12.521234 unitelabs_sila-0.1.1/src/sila/commands/observable_command.py
+-rw-r--r--   0        0        0      390 2023-06-11 21:57:12.522401 unitelabs_sila-0.1.1/src/sila/commands/unobservable_command.py
+-rw-r--r--   0        0        0     1231 2023-06-13 17:34:19.443118 unitelabs_sila-0.1.1/src/sila/constraints/__init__.py
+-rw-r--r--   0        0        0      625 2023-06-11 21:57:12.523714 unitelabs_sila-0.1.1/src/sila/constraints/allowed_types.py
+-rw-r--r--   0        0        0      478 2023-06-14 05:05:30.931848 unitelabs_sila-0.1.1/src/sila/constraints/constraint.py
+-rw-r--r--   0        0        0      921 2023-06-08 08:41:46.740250 unitelabs_sila-0.1.1/src/sila/constraints/content_type.py
+-rw-r--r--   0        0        0      889 2023-06-03 09:51:05.606924 unitelabs_sila-0.1.1/src/sila/constraints/element_count.py
+-rw-r--r--   0        0        0     1555 2023-06-16 13:19:36.970594 unitelabs_sila-0.1.1/src/sila/constraints/fully_qualified_identifier.py
+-rw-r--r--   0        0        0      934 2023-06-11 21:57:12.525011 unitelabs_sila-0.1.1/src/sila/constraints/length.py
+-rw-r--r--   0        0        0      904 2023-06-03 09:51:05.610073 unitelabs_sila-0.1.1/src/sila/constraints/maximal_element_count.py
+-rw-r--r--   0        0        0      888 2023-06-03 09:55:31.158596 unitelabs_sila-0.1.1/src/sila/constraints/maximal_exclusive.py
+-rw-r--r--   0        0        0      907 2023-06-03 09:55:36.776856 unitelabs_sila-0.1.1/src/sila/constraints/maximal_inclusive.py
+-rw-r--r--   0        0        0      985 2023-06-14 05:03:54.580670 unitelabs_sila-0.1.1/src/sila/constraints/maximal_length.py
+-rw-r--r--   0        0        0      899 2023-06-03 09:51:05.614671 unitelabs_sila-0.1.1/src/sila/constraints/minimal_element_count.py
+-rw-r--r--   0        0        0      893 2023-06-03 09:55:34.058872 unitelabs_sila-0.1.1/src/sila/constraints/minimal_exclusive.py
+-rw-r--r--   0        0        0      909 2023-06-03 09:55:38.301758 unitelabs_sila-0.1.1/src/sila/constraints/minimal_inclusive.py
+-rw-r--r--   0        0        0      994 2023-06-03 09:51:05.622353 unitelabs_sila-0.1.1/src/sila/constraints/minimal_length.py
+-rw-r--r--   0        0        0      623 2023-06-14 05:05:30.933163 unitelabs_sila-0.1.1/src/sila/constraints/pattern.py
+-rw-r--r--   0        0        0      665 2023-06-08 08:53:44.725620 unitelabs_sila-0.1.1/src/sila/constraints/schema.py
+-rw-r--r--   0        0        0      726 2023-06-03 09:55:39.422718 unitelabs_sila-0.1.1/src/sila/constraints/set.py
+-rw-r--r--   0        0        0     1602 2023-06-08 08:29:13.185856 unitelabs_sila-0.1.1/src/sila/constraints/unit.py
+-rw-r--r--   0        0        0      144 2023-06-11 21:57:12.526082 unitelabs_sila-0.1.1/src/sila/core/__init__.py
+-rw-r--r--   0        0        0     3851 2023-06-16 16:35:01.561541 unitelabs_sila-0.1.1/src/sila/core/feature.py
+-rw-r--r--   0        0        0     1709 2023-06-11 21:57:12.527474 unitelabs_sila-0.1.1/src/sila/core/handler.py
+-rw-r--r--   0        0        0     2971 2023-06-14 05:05:30.933915 unitelabs_sila-0.1.1/src/sila/core/server.py
+-rw-r--r--   0        0        0      769 2023-06-13 15:55:13.097999 unitelabs_sila-0.1.1/src/sila/data_types/__init__.py
+-rw-r--r--   0        0        0     1102 2023-06-04 19:54:04.417061 unitelabs_sila-0.1.1/src/sila/data_types/any.py
+-rw-r--r--   0        0        0     1053 2023-06-07 19:30:07.082139 unitelabs_sila-0.1.1/src/sila/data_types/basic_type.py
+-rw-r--r--   0        0        0     1354 2023-06-04 20:29:24.951615 unitelabs_sila-0.1.1/src/sila/data_types/binary.py
+-rw-r--r--   0        0        0      771 2023-06-04 19:48:34.281597 unitelabs_sila-0.1.1/src/sila/data_types/boolean.py
+-rw-r--r--   0        0        0     1336 2023-06-07 19:30:18.487002 unitelabs_sila-0.1.1/src/sila/data_types/constrained.py
+-rw-r--r--   0        0        0      867 2023-06-07 19:30:26.689597 unitelabs_sila-0.1.1/src/sila/data_types/data_type.py
+-rw-r--r--   0        0        0     2644 2023-06-16 10:08:28.352141 unitelabs_sila-0.1.1/src/sila/data_types/data_type_definition.py
+-rw-r--r--   0        0        0     1965 2023-06-04 19:47:40.030909 unitelabs_sila-0.1.1/src/sila/data_types/date.py
+-rw-r--r--   0        0        0     1130 2023-06-04 19:46:07.096305 unitelabs_sila-0.1.1/src/sila/data_types/duration.py
+-rw-r--r--   0        0        0      743 2023-06-05 10:53:18.827154 unitelabs_sila-0.1.1/src/sila/data_types/integer.py
+-rw-r--r--   0        0        0     1286 2023-06-07 19:30:34.932708 unitelabs_sila-0.1.1/src/sila/data_types/list.py
+-rw-r--r--   0        0        0      760 2023-06-04 19:38:15.675710 unitelabs_sila-0.1.1/src/sila/data_types/real.py
+-rw-r--r--   0        0        0     1147 2023-06-08 22:12:52.848122 unitelabs_sila-0.1.1/src/sila/data_types/string.py
+-rw-r--r--   0        0        0     4271 2023-06-09 10:45:44.390563 unitelabs_sila-0.1.1/src/sila/data_types/structure.py
+-rw-r--r--   0        0        0     1948 2023-06-04 19:45:25.161612 unitelabs_sila-0.1.1/src/sila/data_types/time.py
+-rw-r--r--   0        0        0     2533 2023-06-04 19:44:26.791814 unitelabs_sila-0.1.1/src/sila/data_types/timestamp.py
+-rw-r--r--   0        0        0     1250 2023-06-04 19:42:37.697579 unitelabs_sila-0.1.1/src/sila/data_types/timezone.py
+-rw-r--r--   0        0        0      659 2023-06-04 19:42:08.651066 unitelabs_sila-0.1.1/src/sila/data_types/void.py
+-rw-r--r--   0        0        0      164 2023-06-08 20:52:53.907366 unitelabs_sila-0.1.1/src/sila/datetime/__init__.py
+-rw-r--r--   0        0        0     2262 2023-06-08 22:13:58.286982 unitelabs_sila-0.1.1/src/sila/datetime/date.py
+-rw-r--r--   0        0        0       64 2023-06-08 22:13:58.443800 unitelabs_sila-0.1.1/src/sila/discovery/__init__.py
+-rw-r--r--   0        0        0     1785 2023-06-08 22:13:58.444125 unitelabs_sila-0.1.1/src/sila/discovery/broadcaster.py
+-rw-r--r--   0        0        0      446 2023-06-05 20:09:27.499133 unitelabs_sila-0.1.1/src/sila/errors/__init__.py
+-rw-r--r--   0        0        0     2508 2023-06-16 10:02:45.842808 unitelabs_sila-0.1.1/src/sila/errors/defined_execution_error.py
+-rw-r--r--   0        0        0     2005 2023-06-05 20:08:43.148208 unitelabs_sila-0.1.1/src/sila/errors/framework_error.py
+-rw-r--r--   0        0        0     1808 2023-06-05 20:10:27.279204 unitelabs_sila-0.1.1/src/sila/errors/sila_error.py
+-rw-r--r--   0        0        0      647 2023-06-05 20:10:05.335814 unitelabs_sila-0.1.1/src/sila/errors/sila_exception.py
+-rw-r--r--   0        0        0      908 2023-06-05 20:10:02.365590 unitelabs_sila-0.1.1/src/sila/errors/undefined_execution_error.py
+-rw-r--r--   0        0        0     1282 2023-06-05 20:09:59.865569 unitelabs_sila-0.1.1/src/sila/errors/validation_error.py
+-rw-r--r--   0        0        0      941 2023-06-09 06:33:45.337996 unitelabs_sila-0.1.1/src/sila/fdl_parser/__init__.py
+-rw-r--r--   0        0        0     1684 2023-06-08 11:09:33.254085 unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_command.py
+-rw-r--r--   0        0        0     5095 2023-06-08 22:13:58.338287 unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_constraint.py
+-rw-r--r--   0        0        0     3182 2023-06-08 10:47:41.040745 unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_data_type.py
+-rw-r--r--   0        0        0      752 2023-06-09 06:36:56.248348 unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_data_type_definition.py
+-rw-r--r--   0        0        0      586 2023-06-08 10:46:24.525760 unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_defined_execution_error.py
+-rw-r--r--   0        0        0      418 2023-06-08 09:45:35.011949 unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_defined_execution_error_list.py
+-rw-r--r--   0        0        0      245 2023-06-09 18:55:45.433970 unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_description.py
+-rw-r--r--   0        0        0     2496 2023-06-16 13:37:39.864064 unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_feature.py
+-rw-r--r--   0        0        0      852 2023-06-08 22:13:58.339752 unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_metadata.py
+-rw-r--r--   0        0        0      944 2023-06-08 11:09:39.444072 unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_property.py
+-rw-r--r--   0        0        0      760 2023-06-08 10:43:45.918520 unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_sila_element.py
+-rw-r--r--   0        0        0     1211 2023-06-04 15:05:41.890867 unitelabs_sila-0.1.1/src/sila/identifiers/__init__.py
+-rw-r--r--   0        0        0      921 2023-06-16 10:01:09.883882 unitelabs_sila-0.1.1/src/sila/identifiers/command_identifier.py
+-rw-r--r--   0        0        0     1010 2023-06-16 10:01:09.885217 unitelabs_sila-0.1.1/src/sila/identifiers/command_parameter_identifier.py
+-rw-r--r--   0        0        0      997 2023-06-16 10:01:09.885723 unitelabs_sila-0.1.1/src/sila/identifiers/command_response_identifier.py
+-rw-r--r--   0        0        0     1037 2023-06-16 10:01:09.886355 unitelabs_sila-0.1.1/src/sila/identifiers/custom_data_type_identifier.py
+-rw-r--r--   0        0        0     1139 2023-06-16 10:01:09.887826 unitelabs_sila-0.1.1/src/sila/identifiers/defined_execution_error_identifier.py
+-rw-r--r--   0        0        0     1696 2023-06-16 13:21:37.926999 unitelabs_sila-0.1.1/src/sila/identifiers/feature_identifier.py
+-rw-r--r--   0        0        0     1009 2023-06-16 10:39:35.807691 unitelabs_sila-0.1.1/src/sila/identifiers/identifier.py
+-rw-r--r--   0        0        0     1177 2023-06-16 10:01:09.902704 unitelabs_sila-0.1.1/src/sila/identifiers/intermediate_command_response_identifier.py
+-rw-r--r--   0        0        0      923 2023-06-16 10:39:06.952069 unitelabs_sila-0.1.1/src/sila/identifiers/metadata_identifier.py
+-rw-r--r--   0        0        0      925 2023-06-16 10:01:09.904485 unitelabs_sila-0.1.1/src/sila/identifiers/property_identifier.py
+-rw-r--r--   0        0        0       55 2023-06-08 22:13:58.340262 unitelabs_sila-0.1.1/src/sila/metadata/__init__.py
+-rw-r--r--   0        0        0     2850 2023-06-16 10:01:44.723784 unitelabs_sila-0.1.1/src/sila/metadata/metadata.py
+-rw-r--r--   0        0        0      224 2023-06-05 14:34:27.247039 unitelabs_sila-0.1.1/src/sila/properties/__init__.py
+-rw-r--r--   0        0        0      395 2023-06-05 18:28:34.990277 unitelabs_sila-0.1.1/src/sila/properties/observable_property.py
+-rw-r--r--   0        0        0     1313 2023-06-16 10:01:53.702668 unitelabs_sila-0.1.1/src/sila/properties/property.py
+-rw-r--r--   0        0        0      389 2023-06-05 18:29:02.534670 unitelabs_sila-0.1.1/src/sila/properties/unobservable_property.py
+-rw-r--r--   0        0        0      550 2023-06-05 05:48:33.521128 unitelabs_sila-0.1.1/src/sila/protobuf/__init__.py
+-rw-r--r--   0        0        0      441 2023-06-03 09:48:32.882854 unitelabs_sila-0.1.1/src/sila/protobuf/decode_error.py
+-rw-r--r--   0        0        0        0 2023-06-12 07:48:23.932059 unitelabs_sila-0.1.1/src/sila/py.typed
+-rw-r--r--   0        0        0      670 2023-06-08 22:13:58.341251 unitelabs_sila-0.1.1/src/sila/server/__init__.py
+-rw-r--r--   0        0        0     1913 2023-06-16 10:38:43.335380 unitelabs_sila-0.1.1/src/sila/server/feature.py
+-rw-r--r--   0        0        0      862 2023-06-07 10:04:20.415702 unitelabs_sila-0.1.1/src/sila/server/handler.py
+-rw-r--r--   0        0        0     1374 2023-06-15 20:32:32.072752 unitelabs_sila-0.1.1/src/sila/server/metadata.py
+-rw-r--r--   0        0        0     8240 2023-06-16 08:24:39.138382 unitelabs_sila-0.1.1/src/sila/server/observable_command.py
+-rw-r--r--   0        0        0     2925 2023-06-15 20:28:56.560208 unitelabs_sila-0.1.1/src/sila/server/observable_property.py
+-rw-r--r--   0        0        0     5302 2023-06-16 16:25:47.002998 unitelabs_sila-0.1.1/src/sila/server/server.py
+-rw-r--r--   0        0        0     2504 2023-06-16 13:26:00.125295 unitelabs_sila-0.1.1/src/sila/server/unobservable_command.py
+-rw-r--r--   0        0        0     2638 2023-06-15 20:29:13.265509 unitelabs_sila-0.1.1/src/sila/server/unobservable_property.py
+-rw-r--r--   0        0        0      222 2023-06-14 05:05:30.935366 unitelabs_sila-0.1.1/src/sila/validators/__init__.py
+-rw-r--r--   0        0        0      963 2023-06-14 05:05:30.935791 unitelabs_sila-0.1.1/src/sila/validators/display_name.py
+-rw-r--r--   0        0        0     1192 2023-06-14 05:05:30.936233 unitelabs_sila-0.1.1/src/sila/validators/domain.py
+-rw-r--r--   0        0        0     1335 2023-06-14 05:05:30.936778 unitelabs_sila-0.1.1/src/sila/validators/identifier.py
+-rw-r--r--   0        0        0     1129 2023-06-14 05:05:30.937160 unitelabs_sila-0.1.1/src/sila/validators/uuid.py
+-rw-r--r--   0        0        0     1347 2023-06-14 05:05:30.937529 unitelabs_sila-0.1.1/src/sila/validators/validator.py
+-rw-r--r--   0        0        0     2901 2023-06-14 05:05:30.937980 unitelabs_sila-0.1.1/src/sila/validators/version.py
+-rw-r--r--   0        0        0     3469 1970-01-01 00:00:00.000000 unitelabs_sila-0.1.1/PKG-INFO
```

### Comparing `unitelabs_sila-0.1.0/LICENSE` & `unitelabs_sila-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/README.md` & `unitelabs_sila-0.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 ![pipeline](https://gitlab.com/unitelabs/integrations/sila2/sila-python/badges/main/pipeline.svg?ignore_skipped=true)
 ![coverage](https://gitlab.com/unitelabs/integrations/sila2/sila-python/badges/main/coverage.svg?job=test)
-![release](https://gitlab.com/unitelabs/integrations/sila2/sila-python/badges/release.svg)
 ![license](https://img.shields.io/gitlab/license/unitelabs/integrations/sila2/sila-python)
 
 # SiLA
 
 This repository is an un-opinionated library that provides you with all means to develop a SiLA 2 1.1 compliant python
 application. It adheres to the [SiLA 2 specification](https://sila2.gitlab.io/sila_base/) and is used by the [UniteLabs 
 Connector Framework](https://gitlab.com/unitelabs/connector-framework/) to enable rapid development of cloud-native SiLA 
@@ -23,15 +22,15 @@
 $ poetry run connector start
 ```
 
 You can also manually create a new project from scratch and install the library with pip. In this case, of course,
 you'll be responsible for creating the project boilerplate files yourself.
 
 ```
-pip install unitelabs-sila
+$ pip install unitelabs-sila
 ```
 
 ## Documentation
 
 🧱🚧🏗️ This is still work in progress 🧱🚧🏗️  
 
 ## Contribute
```

### Comparing `unitelabs_sila-0.1.0/pyproject.toml` & `unitelabs_sila-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unitelabs-sila"
-version = "0.1.0"
+version = "0.1.1"
 description = "An un-opinionated SiLA 2 library."
 license = "MIT"
 authors = ["UniteLabs AG <developers+sila@unitelabs.ch>"]
 readme = "README.md"
 homepage = "https://sila-standard.com"
 repository = "https://gitlab.com/unitelabs/integrations/sila2/sila-python"
 documentation = "https://gitlab.com/unitelabs/integrations/sila2/sila-python/-/tree/main/docs/"
```

### Comparing `unitelabs_sila-0.1.0/src/sila/cloud_connector/cloud_server_endpoint.py` & `unitelabs_sila-0.1.1/src/sila/cloud_connector/cloud_server_endpoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import weakref
 
 import grpc
 import grpc.aio
 import grpc.experimental
 
 from sila import commands, errors
-from sila.server import Server
+from sila.server import ObservableCommand, ObservableProperty, Server, UnobservableCommand, UnobservableProperty
 
 from . import messages
 
 
 class CloudServerEndpointConfig(typing.TypedDict, total=False):
     endpoint: str
     secure: bool
@@ -51,15 +51,15 @@
 class CloudServerEndpoint:
     """gRPC client for SiLA cloud connectivity"""
 
     def __init__(self, server: Server, config: CloudServerEndpointConfig | None = None):
         self.__config = config or {}
         self._channel: typing.Optional[grpc.aio.Channel] = None
         self.responses = Responses(self.logger)
-        self.server = weakref.proxy(server)
+        self.server: Server = weakref.proxy(server)
         self.subscriptions: dict[str, asyncio.Task] = {}
 
     async def start(self):
         """Starts this client."""
         address = self.__config.get("endpoint", "localhost:5000")
         self.logger.info("Starting cloud server endpoint on address '%s'...", address)
 
@@ -196,15 +196,20 @@
         if client_message.cancelObservablePropertySubscription is not None:
             asyncio.create_task(self.cancelObservablePropertySubscription(client_message.requestUUID))
 
     async def unobservable_command_execution(
         self, request_uuid: str, identifier: str, parameters: bytes, metadata: dict
     ):
         try:
-            unobservable_command = self.server.get_unobservable_command(identifier)
+            feature = self.server.get_feature(identifier=identifier)
+            unobservable_command = feature.get_command(identifier=identifier)
+
+            if not isinstance(unobservable_command, UnobservableCommand):
+                raise ValueError()
+
             responses = await unobservable_command.execute(parameters, metadata)
             message = messages.SiLAServerMessage(
                 requestUUID=request_uuid,
                 unobservableCommandResponse=messages.UnobservableCommandResponse(response=responses),
             )
             await self.responses.put(message)
         except errors.SiLAException as error:
@@ -214,15 +219,20 @@
             )
             await self.responses.put(message)
 
     async def observable_command_initiation(
         self, request_uuid: str, identifier: str, parameters: bytes, metadata: dict
     ):
         try:
-            observable_command = self.server.get_observable_command(identifier)
+            feature = self.server.get_feature(identifier=identifier)
+            observable_command = feature.get_command(identifier=identifier)
+
+            if not isinstance(observable_command, ObservableCommand):
+                raise ValueError()
+
             command_confirmation = await observable_command.initiate_command(parameters, metadata)
             message = messages.SiLAServerMessage(
                 requestUUID=request_uuid,
                 observableCommandConfirmation=messages.ObservableCommandConfirmation(
                     commandConfirmation=command_confirmation
                 ),
             )
@@ -233,25 +243,32 @@
             )
             await self.responses.put(message)
 
     async def observable_command_execution_info_subscription(
         self, request_uuid: str, command_execution_uuid: commands.CommandExecutionUUID
     ):
         try:
-            command_execution = self.server.get_command_execution(command_execution_uuid.value)
-            observable_command = command_execution.command
+            command_execution = self.server.get_command_execution(command_execution_uuid=command_execution_uuid.value)
+
+            feature = self.server.get_feature(identifier=str(command_execution.identifier))
+            observable_command = feature.get_command(identifier=str(command_execution.identifier))
+
+            if not isinstance(observable_command, ObservableCommand):
+                raise ValueError()
 
             if current_task := asyncio.current_task():
                 self.subscriptions[request_uuid + "_info"] = current_task
 
-            async for responses in observable_command.subscribe_status(command_execution.uuid):
+            async for responses in observable_command.subscribe_status(command_execution.command_execution_uuid):
                 message = messages.SiLAServerMessage(
                     requestUUID=request_uuid,
                     observableCommandExecutionInfo=messages.ObservableCommandExecutionInfo(
-                        commandExecutionUUID=commands.CommandExecutionUUID(value=command_execution.uuid),
+                        commandExecutionUUID=commands.CommandExecutionUUID(
+                            value=command_execution.command_execution_uuid
+                        ),
                         executionInfo=responses,
                     ),
                 )
                 await self.responses.put(message)
         except errors.SiLAException as error:
             message = messages.SiLAServerMessage(
                 requestUUID=request_uuid,
@@ -263,25 +280,32 @@
         if request_uuid + "_info" in self.subscriptions:
             self.subscriptions.pop(request_uuid + "_info").cancel()
 
     async def observable_command_intermediate_response_subscription(
         self, request_uuid: str, command_execution_uuid: commands.CommandExecutionUUID
     ):
         try:
-            command_execution = self.server.get_command_execution(command_execution_uuid.value)
-            observable_command = command_execution.command
+            command_execution = self.server.get_command_execution(command_execution_uuid=command_execution_uuid.value)
+
+            feature = self.server.get_feature(identifier=str(command_execution.identifier))
+            observable_command = feature.get_command(identifier=str(command_execution.identifier))
+
+            if not isinstance(observable_command, ObservableCommand):
+                raise ValueError()
 
             if current_task := asyncio.current_task():
                 self.subscriptions[request_uuid + "_intermediate"] = current_task
 
-            async for responses in observable_command.subscribe_intermediate(command_execution.uuid):
+            async for responses in observable_command.subscribe_intermediate(command_execution.command_execution_uuid):
                 message = messages.SiLAServerMessage(
                     requestUUID=request_uuid,
                     observableCommandIntermediateResponse=messages.ObservableCommandIntermediateResponse(
-                        commandExecutionUUID=commands.CommandExecutionUUID(value=command_execution.uuid),
+                        commandExecutionUUID=commands.CommandExecutionUUID(
+                            value=command_execution.command_execution_uuid
+                        ),
                         response=responses,
                     ),
                 )
                 await self.responses.put(message)
         except errors.SiLAException as error:
             message = messages.SiLAServerMessage(
                 requestUUID=request_uuid,
@@ -293,51 +317,66 @@
         if request_uuid + "_intermediate" in self.subscriptions:
             self.subscriptions.pop(request_uuid + "_intermediate").cancel()
 
     async def observable_command_get_response(
         self, request_uuid: str, command_execution_uuid: commands.CommandExecutionUUID
     ):
         try:
-            command_execution = self.server.get_command_execution(command_execution_uuid.value)
-            observable_command = command_execution.command
-            response = await observable_command.get_result(command_execution.uuid)
+            command_execution = self.server.get_command_execution(command_execution_uuid=command_execution_uuid.value)
+
+            feature = self.server.get_feature(identifier=str(command_execution.identifier))
+            observable_command = feature.get_command(identifier=str(command_execution.identifier))
+
+            if not isinstance(observable_command, ObservableCommand):
+                raise ValueError()
+
+            response = await observable_command.get_result(command_execution.command_execution_uuid)
 
             message = messages.SiLAServerMessage(
                 requestUUID=request_uuid,
                 observableCommandResponse=messages.ObservableCommandResponse(
-                    commandExecutionUUID=commands.CommandExecutionUUID(value=command_execution.uuid),
+                    commandExecutionUUID=commands.CommandExecutionUUID(value=command_execution.command_execution_uuid),
                     response=response,
                 ),
             )
             await self.responses.put(message)
         except errors.SiLAException as error:
             message = messages.SiLAServerMessage(
                 requestUUID=request_uuid,
                 commandError=errors.SiLAError.from_exception(error),
             )
             await self.responses.put(message)
 
     async def unobservable_property_read(self, request_uuid: str, identifier: str, metadata: dict):
         try:
-            unobservable_property = self.server.get_unobservable_property(identifier)
+            feature = self.server.get_feature(identifier=identifier)
+            unobservable_property = feature.get_property(identifier=identifier)
+
+            if not isinstance(unobservable_property, UnobservableProperty):
+                raise ValueError()
+
             responses = await unobservable_property.execute(metadata)
             message = messages.SiLAServerMessage(
                 requestUUID=request_uuid, unobservablePropertyValue=messages.UnobservablePropertyValue(value=responses)
             )
             await self.responses.put(message)
         except errors.SiLAException as error:
             message = messages.SiLAServerMessage(
                 requestUUID=request_uuid,
                 propertyError=errors.SiLAError.from_exception(error),
             )
             await self.responses.put(message)
 
     async def observable_property_subscription(self, request_uuid: str, identifier: str, metadata: dict):
         try:
-            observable_property = self.server.get_observable_property(identifier)
+            feature = self.server.get_feature(identifier=identifier)
+            observable_property = feature.get_property(identifier=identifier)
+
+            if not isinstance(observable_property, ObservableProperty):
+                raise ValueError()
 
             if current_task := asyncio.current_task():
                 self.subscriptions[request_uuid] = current_task
 
             async for responses in observable_property.execute(metadata):
                 message = messages.SiLAServerMessage(
                     requestUUID=request_uuid,
```

### Comparing `unitelabs_sila-0.1.0/src/sila/cloud_connector/messages.py` & `unitelabs_sila-0.1.1/src/sila/cloud_connector/messages.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/commands/__init__.py` & `unitelabs_sila-0.1.1/src/sila/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/commands/command.py` & `unitelabs_sila-0.1.1/src/sila/commands/command.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/commands/command_confirmation.py` & `unitelabs_sila-0.1.1/src/sila/commands/command_confirmation.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/commands/command_execution.py` & `unitelabs_sila-0.1.1/src/sila/commands/command_execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from __future__ import annotations
 
 import asyncio
 import dataclasses
 import typing
 import uuid
 
-from sila import data_types, datetime, errors
+from sila import data_types, datetime, errors, identifiers
 
 from .command_confirmation import CommandConfirmation
 from .command_execution_info import CommandExecutionInfo, CommandExecutionStatus
 from .command_execution_uuid import CommandExecutionUUID
 
 
 @dataclasses.dataclass
 class CommandExecution:
+    identifier: identifiers.FullyQualifiedCommandIdentifier
+    """The command's fully qualified identifier."""
+
     executable: typing.Callable
     """The function to call when the execution should run."""
 
     task: typing.Optional[asyncio.Task] = None
 
     command_execution_uuid: str = dataclasses.field(default_factory=lambda: str(uuid.uuid4()))
     """A Command Execution UUID is the UUID of a Command execution."""
```

### Comparing `unitelabs_sila-0.1.0/src/sila/commands/command_execution_info.py` & `unitelabs_sila-0.1.1/src/sila/commands/command_execution_info.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/commands/observable_command.py` & `unitelabs_sila-0.1.1/src/sila/commands/observable_command.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/constraints/__init__.py` & `unitelabs_sila-0.1.1/src/sila/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/constraints/allowed_types.py` & `unitelabs_sila-0.1.1/src/sila/constraints/allowed_types.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/constraints/content_type.py` & `unitelabs_sila-0.1.1/src/sila/constraints/content_type.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/constraints/element_count.py` & `unitelabs_sila-0.1.1/src/sila/constraints/element_count.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/constraints/fully_qualified_identifier.py` & `unitelabs_sila-0.1.1/src/sila/constraints/fully_qualified_identifier.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/constraints/length.py` & `unitelabs_sila-0.1.1/src/sila/constraints/length.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/constraints/maximal_element_count.py` & `unitelabs_sila-0.1.1/src/sila/constraints/maximal_element_count.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/constraints/maximal_exclusive.py` & `unitelabs_sila-0.1.1/src/sila/constraints/maximal_exclusive.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/constraints/maximal_inclusive.py` & `unitelabs_sila-0.1.1/src/sila/constraints/maximal_inclusive.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/constraints/maximal_length.py` & `unitelabs_sila-0.1.1/src/sila/constraints/maximal_length.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/constraints/minimal_element_count.py` & `unitelabs_sila-0.1.1/src/sila/constraints/minimal_element_count.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/constraints/minimal_exclusive.py` & `unitelabs_sila-0.1.1/src/sila/constraints/minimal_exclusive.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/constraints/minimal_inclusive.py` & `unitelabs_sila-0.1.1/src/sila/constraints/minimal_inclusive.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/constraints/minimal_length.py` & `unitelabs_sila-0.1.1/src/sila/constraints/minimal_length.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/constraints/pattern.py` & `unitelabs_sila-0.1.1/src/sila/constraints/pattern.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/constraints/schema.py` & `unitelabs_sila-0.1.1/src/sila/constraints/schema.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/constraints/set.py` & `unitelabs_sila-0.1.1/src/sila/constraints/set.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/constraints/unit.py` & `unitelabs_sila-0.1.1/src/sila/constraints/unit.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/core/feature.py` & `unitelabs_sila-0.1.1/src/sila/metadata/metadata.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,71 @@
 from __future__ import annotations
 
 import dataclasses
 import typing
 
-from sila import identifiers, validators
+from sila import data_types, errors, identifiers, protobuf
 
 if typing.TYPE_CHECKING:
-    from sila import commands, data_types, metadata, properties
+    from sila import core
 
 
 @dataclasses.dataclass
-class Feature:
+class Metadata:
     """
-    Each feature describes a specific behavior of a SiLA server (e.g. the ability to measure a spectrum, to register a
-    sample in a LIMS, control heating, etc.). Features are implemented by a SiLA server and used by a SiLA client. The
-    SiLA service feature must be implemented by each SiLA server. The SiLA service feature offers basic information
-    about the SiLA server and about all other features the SiLA server implements.
+    SiLA Client Metadata is information that a SiLA Server expects to receive from a SiLA Client when executing a
+    Command or reading or subscribing to a Property. If expected SiLA Client Metadata is not received, a Invalid
+    Metadata Framework Error must be issued. This must be checked before parameter validation. Each SiLA Client Metadata
+    has a specific Metadata Identifier and a SiLA Data Type. Metadata is intended for small pieces of data, and
+    transmission might fail for values larger than 1 KB.
     """
 
-    locale: str = dataclasses.field(repr=False, default="en-us")
-    sila2_version: str = dataclasses.field(repr=False, default="1.1")
-    version: str = dataclasses.field(repr=False, default="1.0")
-    maturity_level: str = dataclasses.field(repr=False, default="Draft")
-    originator: str = dataclasses.field(repr=False, default="ch.unitelabs")
-    category: str = dataclasses.field(repr=False, default="core")
+    @dataclasses.dataclass
+    class AffectedByResponse(protobuf.BaseMessage):
+        affected_calls: typing.Annotated[list[data_types.String.Message], protobuf.Field(1)] = dataclasses.field(
+            default_factory=list
+        )
 
-    identifier: validators.Identifier = validators.Identifier()
+    identifier: str = dataclasses.field(default="")
     """
-    A feature identifier is the identifier of a feature. Each feature must have a feature identifier. All features
-    sharing the scope of the same originator and category must have unique feature identifiers. Uniqueness must be
-    checked without taking lower and upper case into account.
+    A Metadata Identifier is the Identifier of a SiLA Client Metadata. A Metadata Identifier must be unique within the
+    scope of a Feature. Uniqueness must be checked without taking lower and upper case into account.
     """
 
-    display_name: validators.DisplayName = validators.DisplayName()
-    """Human readable name of the SiLA feature."""
-
-    description: str = dataclasses.field(repr=False, default="")
-    """
-    A feature description is the description of a feature. A feature description must describe the behaviors /
-    capabilities the feature models in human readable form and with as many details as possible.
-    """
+    display_name: str = dataclasses.field(default="")
+    """A Metadata Display Name is the Display Name of a SiLA Client Metadata."""
 
-    commands: list[commands.Command] = dataclasses.field(repr=False, default_factory=list)
+    description: str = dataclasses.field(default="")
+    """The Metadata Description is the Description of a SiLA Client Metadata."""
 
-    properties: list[properties.Property] = dataclasses.field(repr=False, default_factory=list)
+    data_type: dataclasses.InitVar[data_types.DataType] = data_types.Void()
+    """A Metadata Data Type is the SiLA Data Type of a SiLA Client Metadata."""
 
-    metadata: list[metadata.Metadata] = dataclasses.field(repr=False, default_factory=list)
+    errors: list[errors.DefinedExecutionError] = dataclasses.field(repr=False, default_factory=list)
 
-    data_type_definitions: list[data_types.DataTypeDefinition] = dataclasses.field(repr=False, default_factory=list)
+    feature: core.Feature | None = dataclasses.field(repr=False, default=None)
+    """The SiLA feature this error was registered with."""
 
-    @property
-    def fully_qualified_identifier(self) -> identifiers.FullyQualifiedIdentifier:
-        return identifiers.FullyQualifiedFeatureIdentifier(
-            self.originator, self.category, self.identifier, self.version.rpartition(".")[0]
+    def __post_init__(self, data_type: data_types.DataType):
+        self.message = data_types.Structure(
+            elements=[
+                data_types.Structure.Element(
+                    identifier=self.identifier,
+                    display_name=self.display_name,
+                    description=self.description,
+                    data_type=data_type,
+                )
+            ]
         )
 
-    def __eq__(self, other) -> bool:
-        return (
-            hasattr(other, "fully_qualified_identifier")
-            and getattr(other, "fully_qualified_identifier") == self.fully_qualified_identifier
+    @property
+    def fully_qualified_identifier(self) -> identifiers.FullyQualifiedMetadataIdentifier:
+        """
+        The Fully Qualified Metadata Identifier of this SiLA Metadata.
+        """
+        if self.feature is None:
+            raise UnboundLocalError()
+
+        feature_identifier = self.feature.fully_qualified_identifier
+        return identifiers.FullyQualifiedMetadataIdentifier(
+            **dataclasses.asdict(feature_identifier), metadata=self.identifier
         )
```

### Comparing `unitelabs_sila-0.1.0/src/sila/core/handler.py` & `unitelabs_sila-0.1.1/src/sila/core/handler.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/core/server.py` & `unitelabs_sila-0.1.1/src/sila/core/server.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/data_types/__init__.py` & `unitelabs_sila-0.1.1/src/sila/data_types/__init__.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/data_types/any.py` & `unitelabs_sila-0.1.1/src/sila/data_types/any.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/data_types/basic_type.py` & `unitelabs_sila-0.1.1/src/sila/data_types/basic_type.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/data_types/binary.py` & `unitelabs_sila-0.1.1/src/sila/data_types/binary.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/data_types/boolean.py` & `unitelabs_sila-0.1.1/src/sila/data_types/boolean.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/data_types/constrained.py` & `unitelabs_sila-0.1.1/src/sila/data_types/constrained.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/data_types/data_type.py` & `unitelabs_sila-0.1.1/src/sila/data_types/data_type.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/data_types/data_type_definition.py` & `unitelabs_sila-0.1.1/src/sila/data_types/data_type_definition.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import dataclasses
 import typing
 import weakref
 
-from sila import core
+from sila import core, identifiers
 
 from .data_type import DataType
 from .structure import Structure
 from .void import Void
 
 if typing.TYPE_CHECKING:
     from sila.core.feature import Feature
@@ -50,16 +50,29 @@
             return self.message.elements[0].data_type.encode(value.get(self.identifier, None), field_number=1)
 
         return self.message.encode(value, field_number=None)
 
     def decode(self, data: bytes) -> dict:
         return self.message.decode(data)
 
+    @property
+    def fully_qualified_identifier(self) -> identifiers.FullyQualifiedCustomDataTypeIdentifier:
+        """
+        The Fully Qualified Custom Data Type Identifier of this SiLA Custom Data Type.
+        """
+        if self.feature is None:
+            raise UnboundLocalError()
+
+        feature_identifier = self.feature.fully_qualified_identifier
+        return identifiers.FullyQualifiedCustomDataTypeIdentifier(
+            **dataclasses.asdict(feature_identifier), custom_data_type=self.identifier
+        )
+
     def add_to_feature(self, feature: Feature):
         """
         Registers this data type definition with a SiLA feature.
 
         Args:
             feature: The SiLA feature to add this data type definition to.
         """
         self.feature = weakref.proxy(feature)
-        feature.data_type_definitions.append(self)
+        feature.data_type_definitions[self.fully_qualified_identifier] = self
```

### Comparing `unitelabs_sila-0.1.0/src/sila/data_types/date.py` & `unitelabs_sila-0.1.1/src/sila/data_types/date.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/data_types/duration.py` & `unitelabs_sila-0.1.1/src/sila/data_types/duration.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/data_types/integer.py` & `unitelabs_sila-0.1.1/src/sila/data_types/integer.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/data_types/list.py` & `unitelabs_sila-0.1.1/src/sila/data_types/list.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/data_types/real.py` & `unitelabs_sila-0.1.1/src/sila/data_types/real.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/data_types/string.py` & `unitelabs_sila-0.1.1/src/sila/data_types/string.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/data_types/structure.py` & `unitelabs_sila-0.1.1/src/sila/data_types/structure.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/data_types/time.py` & `unitelabs_sila-0.1.1/src/sila/data_types/time.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/data_types/timestamp.py` & `unitelabs_sila-0.1.1/src/sila/data_types/timestamp.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/data_types/timezone.py` & `unitelabs_sila-0.1.1/src/sila/data_types/timezone.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/data_types/void.py` & `unitelabs_sila-0.1.1/src/sila/data_types/void.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/datetime/date.py` & `unitelabs_sila-0.1.1/src/sila/datetime/date.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/discovery/broadcaster.py` & `unitelabs_sila-0.1.1/src/sila/discovery/broadcaster.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/errors/defined_execution_error.py` & `unitelabs_sila-0.1.1/src/sila/errors/defined_execution_error.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/errors/framework_error.py` & `unitelabs_sila-0.1.1/src/sila/errors/framework_error.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/errors/sila_error.py` & `unitelabs_sila-0.1.1/src/sila/errors/sila_error.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/errors/sila_exception.py` & `unitelabs_sila-0.1.1/src/sila/errors/sila_exception.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/errors/undefined_execution_error.py` & `unitelabs_sila-0.1.1/src/sila/errors/undefined_execution_error.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/errors/validation_error.py` & `unitelabs_sila-0.1.1/src/sila/errors/validation_error.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/fdl_parser/__init__.py` & `unitelabs_sila-0.1.1/src/sila/fdl_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/fdl_parser/serialize_command.py` & `unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_command.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/fdl_parser/serialize_constraint.py` & `unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_constraint.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/fdl_parser/serialize_data_type.py` & `unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_data_type.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/fdl_parser/serialize_data_type_definition.py` & `unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_data_type_definition.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/fdl_parser/serialize_defined_execution_error.py` & `unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_defined_execution_error.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/fdl_parser/serialize_feature.py` & `unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_feature.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 from .serialize_defined_execution_error import serialize_defined_execution_error
 from .serialize_description import serialize_description
 from .serialize_metadata import serialize_metadata
 from .serialize_property import serialize_property
 
 
 def serialize_feature(feature: core.Feature) -> str:
-    defined_execution_errors = list(
-        {
-            error.identifier: error for handler in feature.commands + feature.properties for error in handler.errors
-        }.values()
-    )
+    defined_execution_errors = {
+        error.identifier: error
+        for handler in list(feature.commands.values()) + list(feature.properties.values())
+        for error in handler.errors
+    }
 
     return (
         '<?xml version="1.0" encoding="utf-8" ?>\n'
         + f'<Feature Locale="{ feature.locale }" SiLA2Version="{feature.sila2_version}" FeatureVersion="{feature.version}" MaturityLevel="{feature.maturity_level}" Originator="{feature.originator}" Category="{feature.category}"\n'
         + '         xmlns="http://www.sila-standard.org"\n'
         + '         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"\n'
         + '         xsi:schemaLocation="http://www.sila-standard.org https://gitlab.com/SiLA2/sila_base/raw/master/schema/FeatureDefinition.xsd">'
@@ -28,26 +28,26 @@
                 f"""
                 <Identifier>{ feature.identifier }</Identifier>
                 <DisplayName>{ feature.display_name }</DisplayName>
                 """
             )
             + serialize_description(feature.description)
             + "\n"
-            + "\n".join(serialize_command(command) for command in feature.commands)
+            + "\n".join(serialize_command(command) for command in feature.commands.values())
             + ("\n" if feature.commands else "")
-            + "\n".join(serialize_property(property_) for property_ in feature.properties)
+            + "\n".join(serialize_property(property_) for property_ in feature.properties.values())
             + ("\n" if feature.properties else "")
-            + "\n".join(serialize_metadata(metadata) for metadata in feature.metadata)
+            + "\n".join(serialize_metadata(metadata) for metadata in feature.metadata.values())
             + ("\n" if feature.metadata else "")
             + "\n".join(
                 serialize_defined_execution_error(defined_execution_error)
-                for defined_execution_error in defined_execution_errors
+                for defined_execution_error in defined_execution_errors.values()
             )
             + ("\n" if defined_execution_errors else "")
             + "\n".join(
                 serialize_data_type_definition(data_type_definition)
-                for data_type_definition in feature.data_type_definitions
+                for data_type_definition in feature.data_type_definitions.values()
             ),
             "  ",
         )
         + "</Feature>"
     )
```

### Comparing `unitelabs_sila-0.1.0/src/sila/fdl_parser/serialize_metadata.py` & `unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_metadata.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/fdl_parser/serialize_property.py` & `unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_property.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/fdl_parser/serialize_sila_element.py` & `unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_sila_element.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/identifiers/__init__.py` & `unitelabs_sila-0.1.1/src/sila/identifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/identifiers/command_identifier.py` & `unitelabs_sila-0.1.1/src/sila/identifiers/command_identifier.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/identifiers/command_parameter_identifier.py` & `unitelabs_sila-0.1.1/src/sila/identifiers/command_parameter_identifier.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/identifiers/command_response_identifier.py` & `unitelabs_sila-0.1.1/src/sila/identifiers/command_response_identifier.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/identifiers/custom_data_type_identifier.py` & `unitelabs_sila-0.1.1/src/sila/identifiers/custom_data_type_identifier.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/identifiers/defined_execution_error_identifier.py` & `unitelabs_sila-0.1.1/src/sila/identifiers/defined_execution_error_identifier.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/identifiers/feature_identifier.py` & `unitelabs_sila-0.1.1/src/sila/identifiers/feature_identifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,21 +21,26 @@
     def __post_init__(self):
         if len(str(self)) > 2048:
             raise ValueError("A fully qualified identifier must not exceed 2048 characters in length.")
 
     @classmethod
     def parse(cls, identifier: str) -> FullyQualifiedFeatureIdentifier:
         try:
-            originator, category, feature, version = identifier.split("/")
+            originator, category, feature, version, *_ = identifier.split("/")
         except AttributeError as error:
             raise ValueError("Received malformed identifier") from error
 
         if not version.startswith("v"):
             raise ValueError("Major version in fully qualified identifiers must be prefixed with 'v', e.g. 'v1'.")
         version = version[1:]
 
         return FullyQualifiedFeatureIdentifier(
             originator=originator, category=category, feature=feature, version=version
         )
 
-    def __repr__(self) -> str:
+    @property
+    def feature_identifier(self) -> str:
+        """The fully qualified feature identifier."""
         return f"{self.originator}/{self.category}/{self.feature}/v{self.version}"
+
+    def __repr__(self) -> str:
+        return self.feature_identifier
```

### Comparing `unitelabs_sila-0.1.0/src/sila/identifiers/identifier.py` & `unitelabs_sila-0.1.1/src/sila/identifiers/identifier.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,9 +23,12 @@
         Returns:
             The fully qualified identifier.
 
         Raises:
             ValueError: Raised if the provided identifier is malformed.
         """
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
         return str(self).lower() == str(other).lower()
+
+    def __hash__(self) -> int:
+        return hash(repr(self))
```

### Comparing `unitelabs_sila-0.1.0/src/sila/identifiers/intermediate_command_response_identifier.py` & `unitelabs_sila-0.1.1/src/sila/identifiers/intermediate_command_response_identifier.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/identifiers/metadata_identifier.py` & `unitelabs_sila-0.1.1/src/sila/identifiers/metadata_identifier.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/identifiers/property_identifier.py` & `unitelabs_sila-0.1.1/src/sila/identifiers/property_identifier.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/properties/property.py` & `unitelabs_sila-0.1.1/src/sila/properties/property.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/protobuf/__init__.py` & `unitelabs_sila-0.1.1/src/sila/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/server/__init__.py` & `unitelabs_sila-0.1.1/src/sila/server/__init__.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/server/feature.py` & `unitelabs_sila-0.1.1/src/sila/server/feature.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,42 +2,45 @@
 
 import dataclasses
 import typing
 import weakref
 
 import grpc
 
-from sila import core
+from sila import core, identifiers
 
 from .handler import Handler
 from .metadata import Metadata
 
 if typing.TYPE_CHECKING:
-    from .server import Server
     from sila.data_types import DataTypeDefinition
 
+    from .server import Server
+
 
 @dataclasses.dataclass
 class Feature(core.Feature):
-    metadata: list[Metadata] = dataclasses.field(repr=False, default_factory=list)
+    metadata: dict[identifiers.FullyQualifiedMetadataIdentifier, Metadata] = dataclasses.field(
+        init=False, repr=False, default_factory=dict
+    )
 
     handlers: dict[str, grpc.RpcMethodHandler] = dataclasses.field(init=False, repr=False, default_factory=dict)
     """A dictionary that maps method names to corresponding RpcMethodHandler."""
 
     server: Server | None = dataclasses.field(init=False, repr=False, default=None)
     """The SiLA server this feature was registered with."""
 
     def add_to_server(self, server: Server) -> None:
         """
         Registers this feature as RPC handler with a SiLA server.
 
         Args:
             server: The SiLA server to add this feature to.
         """
-        server.features[str(self.fully_qualified_identifier)] = self
+        server.features[self.fully_qualified_identifier] = self
         self.server = weakref.proxy(server)
 
         service = ".".join(
             (
                 "sila2",
                 self.originator,
                 self.category,
```

### Comparing `unitelabs_sila-0.1.0/src/sila/server/handler.py` & `unitelabs_sila-0.1.1/src/sila/server/handler.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/server/metadata.py` & `unitelabs_sila-0.1.1/src/sila/server/metadata.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,11 +41,11 @@
         """
         Registers this metadata as RPC handler with a SiLA feature.
 
         Args:
             feature: The SiLA feature to add this metadata to.
         """
         self.feature = weakref.proxy(feature)
-        feature.metadata.append(self)
+        feature.metadata[self.fully_qualified_identifier] = self
         feature.handlers[f"Get_FCPAffectedByMetadata_{self.identifier}"] = grpc.unary_unary_rpc_method_handler(
             self.execute
         )
```

### Comparing `unitelabs_sila-0.1.0/src/sila/server/observable_command.py` & `unitelabs_sila-0.1.1/src/sila/server/observable_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,29 +18,30 @@
 class ObservableCommand(commands.ObservableCommand, Handler):
     async def initiate_command(self, message: bytes, metadata: dict) -> commands.CommandConfirmation:
         if self.feature is None or self.feature.server is None:
             raise RuntimeError("Cannot initiate unbound command.")
 
         try:
             for feature in self.feature.server.features.values():
-                for interceptor in feature.metadata:
+                for interceptor in feature.metadata.values():
                     interceptor.intercept(self, metadata)
         except errors.DefinedExecutionError as error:
             raise errors.FrameworkError(
                 error_type=errors.FrameworkError.Type.INVALID_METADATA, message=error.description
             )
         try:
             parameters = self.parameters.decode(message)
         except protobuf.MessageDecodeError as error:
             raise errors.ValidationError(
                 parameter=f"{self.fully_qualified_identifier}/Parameter/{error.field}", message=error.msg
             )
         try:
             command_execution = commands.CommandExecution(
-                executable=functools.partial(self.execute, parameters=parameters)
+                identifier=self.fully_qualified_identifier,
+                executable=functools.partial(self.execute, parameters=parameters),
             )
             self.feature.server.add_command_execution(command_execution)
             command_execution.run()
 
             return command_execution.command_confirmation
         except errors.DefinedExecutionError as error:
             error.feature = self.feature
@@ -154,15 +155,15 @@
         except errors.SiLAException as error:
             command_execution.raise_exception(error)
         except Exception as error:  # pylint: disable=broad-exception-caught
             command_execution.raise_exception(errors.UndefinedExecutionError(str(error)))
 
     def add_to_feature(self, feature):
         super().add_to_feature(feature=feature)
-        feature.commands.append(self)
+        feature.commands[self.fully_qualified_identifier] = self
 
         feature.handlers[f"{self.identifier}"] = grpc.unary_unary_rpc_method_handler(
             self.initiate_rpc_method_handler, response_serializer=bytes
         )
 
         feature.handlers[f"{self.identifier}_Info"] = grpc.unary_stream_rpc_method_handler(
             self.subscribe_status,
```

### Comparing `unitelabs_sila-0.1.0/src/sila/server/observable_property.py` & `unitelabs_sila-0.1.1/src/sila/server/observable_property.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 class ObservableProperty(properties.ObservableProperty, Handler):
     async def execute(self, metadata: dict) -> AsyncIterator[bytes]:
         if self.feature is None or self.feature.server is None:
             raise RuntimeError("Cannot execute unbound property.")
 
         try:
             for feature in self.feature.server.features.values():
-                for interceptor in feature.metadata:
+                for interceptor in feature.metadata.values():
                     interceptor.intercept(self, metadata)
         except errors.DefinedExecutionError as error:
             raise errors.FrameworkError(
                 error_type=errors.FrameworkError.Type.INVALID_METADATA, message=error.description
             )
         try:
             responses = self.function()
@@ -69,9 +69,9 @@
         except errors.SiLAException as error:
             exception = errors.SiLAError.from_exception(error)
             details = base64.standard_b64encode(bytes(exception)).decode("ascii")
             await context.abort(code=grpc.StatusCode.ABORTED, details=details)
 
     def add_to_feature(self, feature):
         super().add_to_feature(feature=feature)
-        feature.properties.append(self)
+        feature.properties[self.fully_qualified_identifier] = self
         feature.handlers[f"Subscribe_{self.identifier}"] = grpc.unary_stream_rpc_method_handler(self.rpc_method_handler)
```

### Comparing `unitelabs_sila-0.1.0/src/sila/server/unobservable_command.py` & `unitelabs_sila-0.1.1/src/sila/server/unobservable_command.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 class UnobservableCommand(commands.UnobservableCommand, Handler):
     async def execute(self, message: bytes = b"", metadata: dict | None = None) -> bytes:
         if self.feature is None or self.feature.server is None:
             raise RuntimeError("Cannot execute unbound command.")
 
         try:
             for feature in self.feature.server.features.values():
-                for interceptor in feature.metadata:
+                for interceptor in feature.metadata.values():
                     interceptor.intercept(self, metadata or {})
         except errors.DefinedExecutionError as error:
             raise errors.FrameworkError(
                 error_type=errors.FrameworkError.Type.INVALID_METADATA, message=error.description
             )
         try:
             parameters = self.parameters.decode(message)
@@ -54,9 +54,9 @@
         except errors.SiLAException as error:
             exception = errors.SiLAError.from_exception(error)
             details = base64.standard_b64encode(bytes(exception)).decode("ascii")
             await context.abort(code=grpc.StatusCode.ABORTED, details=details)
 
     def add_to_feature(self, feature):
         super().add_to_feature(feature=feature)
-        feature.commands.append(self)
+        feature.commands[self.fully_qualified_identifier] = self
         feature.handlers[self.identifier] = grpc.unary_unary_rpc_method_handler(self.rpc_method_handler)
```

### Comparing `unitelabs_sila-0.1.0/src/sila/server/unobservable_property.py` & `unitelabs_sila-0.1.1/src/sila/server/unobservable_property.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 class UnobservableProperty(properties.UnobservableProperty, Handler):
     async def execute(self, metadata: dict) -> bytes:
         if self.feature is None or self.feature.server is None:
             raise RuntimeError("Cannot execute unbound property.")
 
         try:
             for feature in self.feature.server.features.values():
-                for interceptor in feature.metadata:
+                for interceptor in feature.metadata.values():
                     interceptor.intercept(self, metadata)
         except errors.DefinedExecutionError as error:
             raise errors.FrameworkError(
                 error_type=errors.FrameworkError.Type.INVALID_METADATA, message=error.description
             )
         try:
             responses = self.function()
@@ -62,9 +62,9 @@
         except errors.SiLAException as error:
             exception = errors.SiLAError.from_exception(error)
             details = base64.standard_b64encode(bytes(exception)).decode("ascii")
             await context.abort(code=grpc.StatusCode.ABORTED, details=details)
 
     def add_to_feature(self, feature):
         super().add_to_feature(feature=feature)
-        feature.properties.append(self)
+        feature.properties[self.fully_qualified_identifier] = self
         feature.handlers[f"Get_{self.identifier}"] = grpc.unary_unary_rpc_method_handler(self.rpc_method_handler)
```

### Comparing `unitelabs_sila-0.1.0/src/sila/validators/display_name.py` & `unitelabs_sila-0.1.1/src/sila/validators/display_name.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/validators/domain.py` & `unitelabs_sila-0.1.1/src/sila/validators/domain.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/validators/identifier.py` & `unitelabs_sila-0.1.1/src/sila/validators/identifier.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/validators/uuid.py` & `unitelabs_sila-0.1.1/src/sila/validators/uuid.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/validators/validator.py` & `unitelabs_sila-0.1.1/src/sila/validators/validator.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/src/sila/validators/version.py` & `unitelabs_sila-0.1.1/src/sila/validators/version.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.0/PKG-INFO` & `unitelabs_sila-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitelabs-sila
-Version: 0.1.0
+Version: 0.1.1
 Summary: An un-opinionated SiLA 2 library.
 Home-page: https://sila-standard.com
 License: MIT
 Keywords: SiLA 2,laboratory,automation,connectivity
 Author: UniteLabs AG
 Author-email: developers+sila@unitelabs.ch
 Requires-Python: >=3.9,<4.0
@@ -28,15 +28,14 @@
 Project-URL: Bug Tracker, https://gitlab.com/unitelabs/integrations/sila2/sila-python/-/issues
 Project-URL: Documentation, https://gitlab.com/unitelabs/integrations/sila2/sila-python/-/tree/main/docs/
 Project-URL: Repository, https://gitlab.com/unitelabs/integrations/sila2/sila-python
 Description-Content-Type: text/markdown
 
 ![pipeline](https://gitlab.com/unitelabs/integrations/sila2/sila-python/badges/main/pipeline.svg?ignore_skipped=true)
 ![coverage](https://gitlab.com/unitelabs/integrations/sila2/sila-python/badges/main/coverage.svg?job=test)
-![release](https://gitlab.com/unitelabs/integrations/sila2/sila-python/badges/release.svg)
 ![license](https://img.shields.io/gitlab/license/unitelabs/integrations/sila2/sila-python)
 
 # SiLA
 
 This repository is an un-opinionated library that provides you with all means to develop a SiLA 2 1.1 compliant python
 application. It adheres to the [SiLA 2 specification](https://sila2.gitlab.io/sila_base/) and is used by the [UniteLabs 
 Connector Framework](https://gitlab.com/unitelabs/connector-framework/) to enable rapid development of cloud-native SiLA 
@@ -55,15 +54,15 @@
 $ poetry run connector start
 ```
 
 You can also manually create a new project from scratch and install the library with pip. In this case, of course,
 you'll be responsible for creating the project boilerplate files yourself.
 
 ```
-pip install unitelabs-sila
+$ pip install unitelabs-sila
 ```
 
 ## Documentation
 
 🧱🚧🏗️ This is still work in progress 🧱🚧🏗️  
 
 ## Contribute
```

