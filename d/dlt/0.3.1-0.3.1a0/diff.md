# Comparing `tmp/dlt-0.3.1.tar.gz` & `tmp/dlt-0.3.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlt-0.3.1.tar", max compression
+gzip compressed data, was "dlt-0.3.1a0.tar", max compression
```

## Comparing `dlt-0.3.1.tar` & `dlt-0.3.1a0.tar`

### file list

```diff
@@ -1,214 +1,214 @@
--rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.3.1/LICENSE.txt
--rw-r--r--   0        0        0     4144 2023-06-16 15:10:31.799722 dlt-0.3.1/README.md
--rw-r--r--   0        0        0     1708 2023-06-16 15:10:31.839722 dlt-0.3.1/dlt/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 21:17:44.388805 dlt-0.3.1/dlt/cli/__init__.py
--rw-r--r--   0        0        0    17123 2023-06-16 15:21:55.039722 dlt-0.3.1/dlt/cli/_dlt.py
--rw-r--r--   0        0        0     3886 2023-05-29 14:13:02.418979 dlt-0.3.1/dlt/cli/config_toml_writer.py
--rw-r--r--   0        0        0    15046 2023-06-16 15:10:31.899721 dlt-0.3.1/dlt/cli/deploy_command.py
--rw-r--r--   0        0        0    14843 2023-06-16 15:10:31.939721 dlt-0.3.1/dlt/cli/deploy_command_helpers.py
--rw-r--r--   0        0        0     1853 2023-04-30 21:17:44.388805 dlt-0.3.1/dlt/cli/echo.py
--rw-r--r--   0        0        0      435 2023-06-07 10:42:04.941010 dlt-0.3.1/dlt/cli/exceptions.py
--rw-r--r--   0        0        0    18756 2023-06-07 10:42:04.941010 dlt-0.3.1/dlt/cli/init_command.py
--rw-r--r--   0        0        0    10503 2023-06-15 19:21:49.026312 dlt-0.3.1/dlt/cli/pipeline_command.py
--rw-r--r--   0        0        0     9588 2023-06-16 15:21:55.039722 dlt-0.3.1/dlt/cli/pipeline_files.py
--rw-r--r--   0        0        0     4505 2023-05-24 16:38:22.528779 dlt-0.3.1/dlt/cli/source_detection.py
--rw-r--r--   0        0        0     1899 2023-05-23 16:25:33.987923 dlt-0.3.1/dlt/cli/telemetry_command.py
--rw-r--r--   0        0        0     3753 2023-05-29 18:11:09.008705 dlt-0.3.1/dlt/cli/utils.py
--rw-r--r--   0        0        0      307 2023-03-23 14:48:32.551618 dlt-0.3.1/dlt/common/__init__.py
--rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.3.1/dlt/common/arithmetics.py
--rw-r--r--   0        0        0      442 2023-05-29 14:13:02.418979 dlt-0.3.1/dlt/common/configuration/__init__.py
--rw-r--r--   0        0        0     5078 2023-05-24 16:38:22.528779 dlt-0.3.1/dlt/common/configuration/accessors.py
--rw-r--r--   0        0        0     3469 2023-06-03 16:59:51.259756 dlt-0.3.1/dlt/common/configuration/container.py
--rw-r--r--   0        0        0     6741 2023-05-29 14:13:02.418979 dlt-0.3.1/dlt/common/configuration/exceptions.py
--rw-r--r--   0        0        0     7912 2023-04-22 20:26:30.632198 dlt-0.3.1/dlt/common/configuration/inject.py
--rw-r--r--   0        0        0     1791 2023-05-14 20:33:31.539348 dlt-0.3.1/dlt/common/configuration/paths.py
--rw-r--r--   0        0        0      344 2023-06-16 15:10:31.959721 dlt-0.3.1/dlt/common/configuration/providers/__init__.py
--rw-r--r--   0        0        0      664 2023-05-29 14:13:02.418979 dlt-0.3.1/dlt/common/configuration/providers/airflow.py
--rw-r--r--   0        0        0     1116 2023-05-07 23:03:04.659469 dlt-0.3.1/dlt/common/configuration/providers/context.py
--rw-r--r--   0        0        0     1335 2023-05-07 23:03:04.659469 dlt-0.3.1/dlt/common/configuration/providers/dictionary.py
--rw-r--r--   0        0        0     1981 2023-05-07 23:03:04.659469 dlt-0.3.1/dlt/common/configuration/providers/environ.py
--rw-r--r--   0        0        0     3662 2023-05-29 14:13:02.418979 dlt-0.3.1/dlt/common/configuration/providers/google_secrets.py
--rw-r--r--   0        0        0     1306 2023-05-24 16:38:22.538779 dlt-0.3.1/dlt/common/configuration/providers/provider.py
--rw-r--r--   0        0        0    12880 2023-06-16 15:10:31.999722 dlt-0.3.1/dlt/common/configuration/providers/toml.py
--rw-r--r--   0        0        0    18788 2023-06-07 08:32:53.261010 dlt-0.3.1/dlt/common/configuration/resolve.py
--rw-r--r--   0        0        0      971 2023-05-29 14:13:02.418979 dlt-0.3.1/dlt/common/configuration/specs/__init__.py
--rw-r--r--   0        0        0     1817 2023-05-07 23:03:04.659469 dlt-0.3.1/dlt/common/configuration/specs/api_credentials.py
--rw-r--r--   0        0        0     2109 2023-05-29 14:13:02.418979 dlt-0.3.1/dlt/common/configuration/specs/aws_credentials.py
--rw-r--r--   0        0        0    14214 2023-05-29 14:13:02.418979 dlt-0.3.1/dlt/common/configuration/specs/base_configuration.py
--rw-r--r--   0        0        0     5483 2023-05-29 14:13:02.418979 dlt-0.3.1/dlt/common/configuration/specs/config_providers_context.py
--rw-r--r--   0        0        0     3387 2023-06-07 08:32:53.261010 dlt-0.3.1/dlt/common/configuration/specs/config_section_context.py
--rw-r--r--   0        0        0     1818 2023-05-24 16:38:22.538779 dlt-0.3.1/dlt/common/configuration/specs/connection_string_credentials.py
--rw-r--r--   0        0        0     2125 2023-04-24 18:26:21.111453 dlt-0.3.1/dlt/common/configuration/specs/exceptions.py
--rw-r--r--   0        0        0    12725 2023-05-07 23:03:04.669469 dlt-0.3.1/dlt/common/configuration/specs/gcp_credentials.py
--rw-r--r--   0        0        0      725 2023-05-07 23:03:04.669469 dlt-0.3.1/dlt/common/configuration/specs/known_sections.py
--rw-r--r--   0        0        0     2455 2023-04-30 21:17:44.388805 dlt-0.3.1/dlt/common/configuration/specs/run_configuration.py
--rw-r--r--   0        0        0     6036 2023-05-29 14:13:02.418979 dlt-0.3.1/dlt/common/configuration/utils.py
--rw-r--r--   0        0        0      142 2023-03-23 14:48:32.551618 dlt-0.3.1/dlt/common/data_types/__init__.py
--rw-r--r--   0        0        0     6306 2023-03-23 14:48:32.551618 dlt-0.3.1/dlt/common/data_types/type_helpers.py
--rw-r--r--   0        0        0      214 2023-03-23 14:48:32.551618 dlt-0.3.1/dlt/common/data_types/typing.py
--rw-r--r--   0        0        0      260 2023-03-23 14:48:20.701618 dlt-0.3.1/dlt/common/data_writers/__init__.py
--rw-r--r--   0        0        0     6201 2023-06-16 15:21:55.039722 dlt-0.3.1/dlt/common/data_writers/buffered.py
--rw-r--r--   0        0        0     2400 2023-06-16 15:10:32.009722 dlt-0.3.1/dlt/common/data_writers/escape.py
--rw-r--r--   0        0        0      962 2023-03-23 14:48:32.551618 dlt-0.3.1/dlt/common/data_writers/exceptions.py
--rw-r--r--   0        0        0     5672 2023-06-16 15:21:55.039722 dlt-0.3.1/dlt/common/data_writers/writers.py
--rw-r--r--   0        0        0      189 2023-05-29 18:11:09.008705 dlt-0.3.1/dlt/common/destination/__init__.py
--rw-r--r--   0        0        0     2228 2023-06-16 15:10:32.029722 dlt-0.3.1/dlt/common/destination/capabilities.py
--rw-r--r--   0        0        0    11099 2023-05-29 18:11:09.008705 dlt-0.3.1/dlt/common/destination/reference.py
--rw-r--r--   0        0        0     6465 2023-06-08 07:50:27.863474 dlt-0.3.1/dlt/common/exceptions.py
--rw-r--r--   0        0        0     4954 2023-03-23 14:48:32.551618 dlt-0.3.1/dlt/common/git.py
--rw-r--r--   0        0        0     5253 2023-05-14 20:33:31.539348 dlt-0.3.1/dlt/common/json/__init__.py
--rw-r--r--   0        0        0     1802 2023-04-10 08:12:53.769595 dlt-0.3.1/dlt/common/json/_orjson.py
--rw-r--r--   0        0        0     2939 2023-04-10 08:12:53.769595 dlt-0.3.1/dlt/common/json/_simplejson.py
--rw-r--r--   0        0        0     1536 2023-04-29 12:58:55.943219 dlt-0.3.1/dlt/common/jsonpath.py
--rw-r--r--   0        0        0      232 2023-03-23 14:48:32.551618 dlt-0.3.1/dlt/common/normalizers/__init__.py
--rw-r--r--   0        0        0     1197 2023-05-07 23:03:04.669469 dlt-0.3.1/dlt/common/normalizers/configuration.py
--rw-r--r--   0        0        0      472 2023-03-23 14:48:32.551618 dlt-0.3.1/dlt/common/normalizers/exceptions.py
--rw-r--r--   0        0        0     1644 2023-04-06 15:27:24.759561 dlt-0.3.1/dlt/common/normalizers/json/__init__.py
--rw-r--r--   0        0        0    13382 2023-05-14 20:33:31.539348 dlt-0.3.1/dlt/common/normalizers/json/relational.py
--rw-r--r--   0        0        0       64 2023-03-23 14:48:32.551618 dlt-0.3.1/dlt/common/normalizers/naming/__init__.py
--rw-r--r--   0        0        0      807 2023-03-23 14:48:32.551618 dlt-0.3.1/dlt/common/normalizers/naming/direct.py
--rw-r--r--   0        0        0     1069 2023-03-23 14:48:32.551618 dlt-0.3.1/dlt/common/normalizers/naming/duck_case.py
--rw-r--r--   0        0        0      792 2023-03-23 14:48:32.551618 dlt-0.3.1/dlt/common/normalizers/naming/exceptions.py
--rw-r--r--   0        0        0     3753 2023-04-05 08:03:40.638919 dlt-0.3.1/dlt/common/normalizers/naming/naming.py
--rw-r--r--   0        0        0     3002 2023-03-23 14:48:32.551618 dlt-0.3.1/dlt/common/normalizers/naming/snake_case.py
--rw-r--r--   0        0        0      358 2023-04-02 09:09:15.855769 dlt-0.3.1/dlt/common/normalizers/typing.py
--rw-r--r--   0        0        0     2337 2023-04-06 15:27:24.759561 dlt-0.3.1/dlt/common/normalizers/utils.py
--rw-r--r--   0        0        0      451 2023-03-23 14:48:32.551618 dlt-0.3.1/dlt/common/pendulum.py
--rw-r--r--   0        0        0    18949 2023-06-07 08:32:53.261010 dlt-0.3.1/dlt/common/pipeline.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.551618 dlt-0.3.1/dlt/common/reflection/__init__.py
--rw-r--r--   0        0        0      374 2023-03-23 14:48:32.551618 dlt-0.3.1/dlt/common/reflection/function_visitor.py
--rw-r--r--   0        0        0     4891 2023-04-09 16:39:04.593180 dlt-0.3.1/dlt/common/reflection/spec.py
--rw-r--r--   0        0        0     5069 2023-04-24 18:26:21.111453 dlt-0.3.1/dlt/common/reflection/utils.py
--rw-r--r--   0        0        0      174 2023-04-30 21:17:44.388805 dlt-0.3.1/dlt/common/runners/__init__.py
--rw-r--r--   0        0        0      705 2023-05-24 16:38:22.538779 dlt-0.3.1/dlt/common/runners/configuration.py
--rw-r--r--   0        0        0     2635 2023-05-14 11:08:47.420838 dlt-0.3.1/dlt/common/runners/pool_runner.py
--rw-r--r--   0        0        0     4046 2023-03-23 14:48:32.561618 dlt-0.3.1/dlt/common/runners/runnable.py
--rw-r--r--   0        0        0     3145 2023-03-23 14:48:32.561618 dlt-0.3.1/dlt/common/runners/stdout.py
--rw-r--r--   0        0        0     2137 2023-03-23 14:48:32.561618 dlt-0.3.1/dlt/common/runners/synth_pickle.py
--rw-r--r--   0        0        0      105 2023-04-30 21:17:44.388805 dlt-0.3.1/dlt/common/runners/typing.py
--rw-r--r--   0        0        0     5590 2023-05-07 23:03:04.669469 dlt-0.3.1/dlt/common/runners/venv.py
--rw-r--r--   0        0        0       36 2023-04-30 21:17:44.398805 dlt-0.3.1/dlt/common/runtime/__init__.py
--rw-r--r--   0        0        0    13923 2023-06-07 08:32:53.261010 dlt-0.3.1/dlt/common/runtime/collector.py
--rw-r--r--   0        0        0     4501 2023-05-14 20:33:31.539348 dlt-0.3.1/dlt/common/runtime/exec_info.py
--rw-r--r--   0        0        0      647 2023-04-30 21:17:44.398805 dlt-0.3.1/dlt/common/runtime/init.py
--rw-r--r--   0        0        0     4002 2023-04-30 21:17:44.398805 dlt-0.3.1/dlt/common/runtime/logger.py
--rw-r--r--   0        0        0     2052 2023-04-30 21:17:44.398805 dlt-0.3.1/dlt/common/runtime/prometheus.py
--rw-r--r--   0        0        0     7170 2023-05-14 20:33:31.539348 dlt-0.3.1/dlt/common/runtime/segment.py
--rw-r--r--   0        0        0     2493 2023-04-30 21:17:44.398805 dlt-0.3.1/dlt/common/runtime/sentry.py
--rw-r--r--   0        0        0     2027 2023-04-30 21:17:44.398805 dlt-0.3.1/dlt/common/runtime/signals.py
--rw-r--r--   0        0        0      616 2023-04-03 18:50:36.893525 dlt-0.3.1/dlt/common/runtime/slack.py
--rw-r--r--   0        0        0      720 2023-04-30 21:17:44.398805 dlt-0.3.1/dlt/common/runtime/telemetry.py
--rw-r--r--   0        0        0      387 2023-04-03 18:50:36.893525 dlt-0.3.1/dlt/common/schema/__init__.py
--rw-r--r--   0        0        0     1927 2023-03-23 14:48:32.561618 dlt-0.3.1/dlt/common/schema/detections.py
--rw-r--r--   0        0        0     2974 2023-03-23 14:48:32.561618 dlt-0.3.1/dlt/common/schema/exceptions.py
--rw-r--r--   0        0        0    25164 2023-05-29 14:13:02.418979 dlt-0.3.1/dlt/common/schema/schema.py
--rw-r--r--   0        0        0     3004 2023-04-22 20:26:30.632198 dlt-0.3.1/dlt/common/schema/typing.py
--rw-r--r--   0        0        0    23080 2023-06-07 08:32:53.261010 dlt-0.3.1/dlt/common/schema/utils.py
--rw-r--r--   0        0        0     1467 2023-05-24 16:38:22.538779 dlt-0.3.1/dlt/common/source.py
--rw-r--r--   0        0        0      554 2023-05-24 16:38:22.538779 dlt-0.3.1/dlt/common/storages/__init__.py
--rw-r--r--   0        0        0     1649 2023-05-24 16:38:22.538779 dlt-0.3.1/dlt/common/storages/configuration.py
--rw-r--r--   0        0        0     1906 2023-03-23 14:48:32.561618 dlt-0.3.1/dlt/common/storages/data_item_storage.py
--rw-r--r--   0        0        0     3107 2023-06-07 08:32:53.261010 dlt-0.3.1/dlt/common/storages/exceptions.py
--rw-r--r--   0        0        0    11872 2023-06-16 15:21:55.039722 dlt-0.3.1/dlt/common/storages/file_storage.py
--rw-r--r--   0        0        0     2690 2023-05-24 16:38:22.538779 dlt-0.3.1/dlt/common/storages/live_schema_storage.py
--rw-r--r--   0        0        0    21812 2023-05-24 16:38:22.538779 dlt-0.3.1/dlt/common/storages/load_storage.py
--rw-r--r--   0        0        0     2409 2023-05-24 16:38:22.538779 dlt-0.3.1/dlt/common/storages/normalize_storage.py
--rw-r--r--   0        0        0     8600 2023-06-07 08:32:53.261010 dlt-0.3.1/dlt/common/storages/schema_storage.py
--rw-r--r--   0        0        0     9486 2023-06-08 07:50:27.863474 dlt-0.3.1/dlt/common/storages/transactional_file.py
--rw-r--r--   0        0        0     2525 2023-04-24 18:26:21.111453 dlt-0.3.1/dlt/common/storages/versioned_storage.py
--rw-r--r--   0        0        0     2634 2023-05-07 23:03:04.669469 dlt-0.3.1/dlt/common/time.py
--rw-r--r--   0        0        0     4736 2023-04-03 18:50:36.893525 dlt-0.3.1/dlt/common/typing.py
--rw-r--r--   0        0        0    14285 2023-06-16 15:10:32.029722 dlt-0.3.1/dlt/common/utils.py
--rw-r--r--   0        0        0     3686 2023-03-23 14:48:32.561618 dlt-0.3.1/dlt/common/validation.py
--rw-r--r--   0        0        0     1185 2023-03-23 14:48:32.561618 dlt-0.3.1/dlt/common/wei.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.561618 dlt-0.3.1/dlt/destinations/__init__.py
--rw-r--r--   0        0        0      437 2023-03-23 14:48:32.561618 dlt-0.3.1/dlt/destinations/bigquery/README.md
--rw-r--r--   0        0        0     1813 2023-06-15 19:21:49.026312 dlt-0.3.1/dlt/destinations/bigquery/__init__.py
--rw-r--r--   0        0        0    12370 2023-06-16 15:10:32.029722 dlt-0.3.1/dlt/destinations/bigquery/bigquery.py
--rw-r--r--   0        0        0      386 2023-05-07 23:03:04.669469 dlt-0.3.1/dlt/destinations/bigquery/configuration.py
--rw-r--r--   0        0        0    10342 2023-05-07 23:03:04.669469 dlt-0.3.1/dlt/destinations/bigquery/sql_client.py
--rw-r--r--   0        0        0     1935 2023-04-05 08:03:40.638919 dlt-0.3.1/dlt/destinations/duckdb/__init__.py
--rw-r--r--   0        0        0     7207 2023-05-29 14:13:02.418979 dlt-0.3.1/dlt/destinations/duckdb/configuration.py
--rw-r--r--   0        0        0     2754 2023-03-23 14:48:32.561618 dlt-0.3.1/dlt/destinations/duckdb/duck.py
--rw-r--r--   0        0        0     6936 2023-04-21 22:25:54.789942 dlt-0.3.1/dlt/destinations/duckdb/sql_client.py
--rw-r--r--   0        0        0     1671 2023-03-23 14:48:32.561618 dlt-0.3.1/dlt/destinations/dummy/__init__.py
--rw-r--r--   0        0        0      736 2023-04-03 18:50:36.893525 dlt-0.3.1/dlt/destinations/dummy/configuration.py
--rw-r--r--   0        0        0     4989 2023-05-29 14:13:02.418979 dlt-0.3.1/dlt/destinations/dummy/dummy.py
--rw-r--r--   0        0        0     4159 2023-04-05 08:03:40.638919 dlt-0.3.1/dlt/destinations/exceptions.py
--rw-r--r--   0        0        0     1270 2023-06-18 19:46:54.773803 dlt-0.3.1/dlt/destinations/filesystem/__init__.py
--rw-r--r--   0        0        0     2253 2023-05-29 14:13:02.418979 dlt-0.3.1/dlt/destinations/filesystem/configuration.py
--rw-r--r--   0        0        0     4935 2023-05-29 14:13:02.418979 dlt-0.3.1/dlt/destinations/filesystem/filesystem.py
--rw-r--r--   0        0        0     1419 2023-05-29 14:13:02.418979 dlt-0.3.1/dlt/destinations/filesystem/filesystem_client.py
--rw-r--r--   0        0        0     5028 2023-06-16 15:21:55.039722 dlt-0.3.1/dlt/destinations/insert_job_client.py
--rw-r--r--   0        0        0    15662 2023-06-16 15:21:55.039722 dlt-0.3.1/dlt/destinations/job_client_impl.py
--rw-r--r--   0        0        0     1303 2023-04-05 08:03:40.638919 dlt-0.3.1/dlt/destinations/job_impl.py
--rw-r--r--   0        0        0      251 2023-03-23 14:48:32.561618 dlt-0.3.1/dlt/destinations/postgres/README.md
--rw-r--r--   0        0        0     1934 2023-04-05 08:03:40.638919 dlt-0.3.1/dlt/destinations/postgres/__init__.py
--rw-r--r--   0        0        0     1316 2023-05-29 18:11:09.008705 dlt-0.3.1/dlt/destinations/postgres/configuration.py
--rw-r--r--   0        0        0     3025 2023-03-23 14:48:32.561618 dlt-0.3.1/dlt/destinations/postgres/postgres.py
--rw-r--r--   0        0        0     6074 2023-05-07 23:03:04.669469 dlt-0.3.1/dlt/destinations/postgres/sql_client.py
--rw-r--r--   0        0        0     1159 2023-04-03 18:50:36.893525 dlt-0.3.1/dlt/destinations/redshift/README.md
--rw-r--r--   0        0        0     1905 2023-04-05 08:03:40.638919 dlt-0.3.1/dlt/destinations/redshift/__init__.py
--rw-r--r--   0        0        0      570 2023-05-07 23:03:04.669469 dlt-0.3.1/dlt/destinations/redshift/configuration.py
--rw-r--r--   0        0        0     3761 2023-03-23 14:48:32.561618 dlt-0.3.1/dlt/destinations/redshift/redshift.py
--rw-r--r--   0        0        0     7117 2023-06-16 15:10:32.029722 dlt-0.3.1/dlt/destinations/sql_client.py
--rw-r--r--   0        0        0    10090 2023-05-28 13:56:42.341452 dlt-0.3.1/dlt/destinations/sql_merge_job.py
--rw-r--r--   0        0        0     1931 2023-04-24 18:26:21.111453 dlt-0.3.1/dlt/destinations/typing.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.1/dlt/extract/__init__.py
--rw-r--r--   0        0        0    26516 2023-06-07 08:32:53.261010 dlt-0.3.1/dlt/extract/decorators.py
--rw-r--r--   0        0        0    12995 2023-06-07 08:32:53.261010 dlt-0.3.1/dlt/extract/exceptions.py
--rw-r--r--   0        0        0     8312 2023-06-16 15:10:32.159721 dlt-0.3.1/dlt/extract/extract.py
--rw-r--r--   0        0        0    14954 2023-05-24 16:38:22.538779 dlt-0.3.1/dlt/extract/incremental.py
--rw-r--r--   0        0        0    35387 2023-06-18 19:50:10.233803 dlt-0.3.1/dlt/extract/pipe.py
--rw-r--r--   0        0        0     9683 2023-05-24 16:38:22.538779 dlt-0.3.1/dlt/extract/schema.py
--rw-r--r--   0        0        0    38391 2023-06-16 15:10:32.259722 dlt-0.3.1/dlt/extract/source.py
--rw-r--r--   0        0        0     4308 2023-05-24 16:38:22.538779 dlt-0.3.1/dlt/extract/typing.py
--rw-r--r--   0        0        0      593 2023-04-06 20:38:35.239561 dlt-0.3.1/dlt/extract/utils.py
--rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.3.1/dlt/helpers/__init__.py
--rw-r--r--   0        0        0    13783 2023-05-28 13:56:42.341452 dlt-0.3.1/dlt/helpers/airflow_helper.py
--rw-r--r--   0        0        0     2907 2023-03-23 14:48:32.561618 dlt-0.3.1/dlt/helpers/dbt/__init__.py
--rw-r--r--   0        0        0     1220 2023-03-23 14:48:32.561618 dlt-0.3.1/dlt/helpers/dbt/configuration.py
--rw-r--r--   0        0        0     6137 2023-03-23 14:48:32.561618 dlt-0.3.1/dlt/helpers/dbt/dbt_utils.py
--rw-r--r--   0        0        0      758 2023-03-23 14:48:32.561618 dlt-0.3.1/dlt/helpers/dbt/exceptions.py
--rw-r--r--   0        0        0     3583 2023-03-23 14:48:32.561618 dlt-0.3.1/dlt/helpers/dbt/profiles.yml
--rw-r--r--   0        0        0    13032 2023-04-30 21:17:44.398805 dlt-0.3.1/dlt/helpers/dbt/runner.py
--rw-r--r--   0        0        0     2490 2023-05-29 14:13:02.438979 dlt-0.3.1/dlt/helpers/pandas_helper.py
--rw-r--r--   0        0        0     1035 2023-06-15 19:21:49.026312 dlt-0.3.1/dlt/helpers/parquet.py
--rw-r--r--   0        0        0    13378 2023-05-29 14:13:02.438979 dlt-0.3.1/dlt/helpers/streamlit_helper.py
--rw-r--r--   0        0        0       31 2023-03-23 14:48:32.571618 dlt-0.3.1/dlt/load/__init__.py
--rw-r--r--   0        0        0     1005 2023-05-24 16:38:22.538779 dlt-0.3.1/dlt/load/configuration.py
--rw-r--r--   0        0        0     1993 2023-04-05 08:03:40.638919 dlt-0.3.1/dlt/load/exceptions.py
--rw-r--r--   0        0        0    19925 2023-06-08 14:19:13.923473 dlt-0.3.1/dlt/load/load.py
--rw-r--r--   0        0        0       32 2023-03-23 14:48:32.571618 dlt-0.3.1/dlt/normalize/__init__.py
--rw-r--r--   0        0        0     1101 2023-05-24 16:38:22.538779 dlt-0.3.1/dlt/normalize/configuration.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.1/dlt/normalize/exceptions.py
--rw-r--r--   0        0        0    16538 2023-06-15 19:21:49.026312 dlt-0.3.1/dlt/normalize/normalize.py
--rw-r--r--   0        0        0    13083 2023-06-16 15:10:32.279722 dlt-0.3.1/dlt/pipeline/__init__.py
--rw-r--r--   0        0        0     1858 2023-06-15 19:21:49.026312 dlt-0.3.1/dlt/pipeline/configuration.py
--rw-r--r--   0        0        0      379 2023-05-24 16:38:22.538779 dlt-0.3.1/dlt/pipeline/current.py
--rw-r--r--   0        0        0     4829 2023-03-23 14:48:32.571618 dlt-0.3.1/dlt/pipeline/dbt.py
--rw-r--r--   0        0        0     3100 2023-05-28 13:56:42.341452 dlt-0.3.1/dlt/pipeline/exceptions.py
--rw-r--r--   0        0        0     8733 2023-06-07 08:32:53.271010 dlt-0.3.1/dlt/pipeline/helpers.py
--rw-r--r--   0        0        0      122 2023-04-06 15:27:24.759561 dlt-0.3.1/dlt/pipeline/mark.py
--rw-r--r--   0        0        0    59020 2023-06-15 19:21:58.236312 dlt-0.3.1/dlt/pipeline/pipeline.py
--rw-r--r--   0        0        0      985 2023-04-30 21:17:44.398805 dlt-0.3.1/dlt/pipeline/progress.py
--rw-r--r--   0        0        0     4186 2023-06-07 08:32:53.271010 dlt-0.3.1/dlt/pipeline/state_sync.py
--rw-r--r--   0        0        0     7990 2023-06-16 15:21:55.039722 dlt-0.3.1/dlt/pipeline/trace.py
--rw-r--r--   0        0        0     4625 2023-05-29 18:11:09.018705 dlt-0.3.1/dlt/pipeline/track.py
--rw-r--r--   0        0        0       91 2023-03-23 14:48:32.571618 dlt-0.3.1/dlt/pipeline/typing.py
--rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.3.1/dlt/py.typed
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.3.1/dlt/reflection/__init__.py
--rw-r--r--   0        0        0      563 2023-03-23 14:48:32.571618 dlt-0.3.1/dlt/reflection/names.py
--rw-r--r--   0        0        0     5617 2023-05-07 23:03:04.669469 dlt-0.3.1/dlt/reflection/script_inspector.py
--rw-r--r--   0        0        0     6186 2023-03-23 14:48:32.571618 dlt-0.3.1/dlt/reflection/script_visitor.py
--rw-r--r--   0        0        0      124 2023-05-07 23:03:04.669469 dlt-0.3.1/dlt/sources/__init__.py
--rw-r--r--   0        0        0      320 2023-05-07 23:03:04.669469 dlt-0.3.1/dlt/sources/credentials.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.3.1/dlt/sources/helpers/__init__.py
--rw-r--r--   0        0        0      574 2023-03-23 14:48:37.261618 dlt-0.3.1/dlt/sources/helpers/requests/__init__.py
--rw-r--r--   0        0        0     9243 2023-05-29 14:13:02.418979 dlt-0.3.1/dlt/sources/helpers/requests/retry.py
--rw-r--r--   0        0        0     1336 2023-03-23 14:48:32.571618 dlt-0.3.1/dlt/sources/helpers/requests/session.py
--rw-r--r--   0        0        0      679 2023-04-06 15:27:24.759561 dlt-0.3.1/dlt/sources/helpers/transform.py
--rw-r--r--   0        0        0     1125 2023-04-22 20:26:30.632198 dlt-0.3.1/dlt/version.py
--rw-r--r--   0        0        0     4276 2023-06-18 19:51:09.063803 dlt-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     7559 1970-01-01 00:00:00.000000 dlt-0.3.1/setup.py
--rw-r--r--   0        0        0     7557 1970-01-01 00:00:00.000000 dlt-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.3.1a0/LICENSE.txt
+-rw-r--r--   0        0        0     4131 2023-06-07 10:42:04.941010 dlt-0.3.1a0/README.md
+-rw-r--r--   0        0        0     1711 2023-04-30 21:17:44.388805 dlt-0.3.1a0/dlt/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 21:17:44.388805 dlt-0.3.1a0/dlt/cli/__init__.py
+-rw-r--r--   0        0        0    16723 2023-06-07 10:42:04.941010 dlt-0.3.1a0/dlt/cli/_dlt.py
+-rw-r--r--   0        0        0     3886 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/cli/config_toml_writer.py
+-rw-r--r--   0        0        0    14636 2023-05-29 18:11:09.008705 dlt-0.3.1a0/dlt/cli/deploy_command.py
+-rw-r--r--   0        0        0    14722 2023-05-29 18:11:09.008705 dlt-0.3.1a0/dlt/cli/deploy_command_helpers.py
+-rw-r--r--   0        0        0     1853 2023-04-30 21:17:44.388805 dlt-0.3.1a0/dlt/cli/echo.py
+-rw-r--r--   0        0        0      435 2023-06-07 10:42:04.941010 dlt-0.3.1a0/dlt/cli/exceptions.py
+-rw-r--r--   0        0        0    18756 2023-06-07 10:42:04.941010 dlt-0.3.1a0/dlt/cli/init_command.py
+-rw-r--r--   0        0        0    10503 2023-05-28 13:56:42.331452 dlt-0.3.1a0/dlt/cli/pipeline_command.py
+-rw-r--r--   0        0        0     9588 2023-06-07 10:42:04.941010 dlt-0.3.1a0/dlt/cli/pipeline_files.py
+-rw-r--r--   0        0        0     4505 2023-05-24 16:38:22.528779 dlt-0.3.1a0/dlt/cli/source_detection.py
+-rw-r--r--   0        0        0     1899 2023-05-23 16:25:33.987923 dlt-0.3.1a0/dlt/cli/telemetry_command.py
+-rw-r--r--   0        0        0     3753 2023-05-29 18:11:09.008705 dlt-0.3.1a0/dlt/cli/utils.py
+-rw-r--r--   0        0        0      307 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/__init__.py
+-rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.3.1a0/dlt/common/arithmetics.py
+-rw-r--r--   0        0        0      442 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/__init__.py
+-rw-r--r--   0        0        0     5078 2023-05-24 16:38:22.528779 dlt-0.3.1a0/dlt/common/configuration/accessors.py
+-rw-r--r--   0        0        0     3469 2023-06-03 16:59:51.259756 dlt-0.3.1a0/dlt/common/configuration/container.py
+-rw-r--r--   0        0        0     6741 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/exceptions.py
+-rw-r--r--   0        0        0     7912 2023-04-22 20:26:30.632198 dlt-0.3.1a0/dlt/common/configuration/inject.py
+-rw-r--r--   0        0        0     1791 2023-05-14 20:33:31.539348 dlt-0.3.1a0/dlt/common/configuration/paths.py
+-rw-r--r--   0        0        0      306 2023-05-07 23:03:04.659469 dlt-0.3.1a0/dlt/common/configuration/providers/__init__.py
+-rw-r--r--   0        0        0      664 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/providers/airflow.py
+-rw-r--r--   0        0        0     1116 2023-05-07 23:03:04.659469 dlt-0.3.1a0/dlt/common/configuration/providers/context.py
+-rw-r--r--   0        0        0     1335 2023-05-07 23:03:04.659469 dlt-0.3.1a0/dlt/common/configuration/providers/dictionary.py
+-rw-r--r--   0        0        0     1981 2023-05-07 23:03:04.659469 dlt-0.3.1a0/dlt/common/configuration/providers/environ.py
+-rw-r--r--   0        0        0     3662 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/providers/google_secrets.py
+-rw-r--r--   0        0        0     1306 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/common/configuration/providers/provider.py
+-rw-r--r--   0        0        0    12390 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/providers/toml.py
+-rw-r--r--   0        0        0    18788 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/common/configuration/resolve.py
+-rw-r--r--   0        0        0      971 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/specs/__init__.py
+-rw-r--r--   0        0        0     1817 2023-05-07 23:03:04.659469 dlt-0.3.1a0/dlt/common/configuration/specs/api_credentials.py
+-rw-r--r--   0        0        0     2109 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/specs/aws_credentials.py
+-rw-r--r--   0        0        0    14214 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/specs/base_configuration.py
+-rw-r--r--   0        0        0     5483 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/specs/config_providers_context.py
+-rw-r--r--   0        0        0     3387 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/common/configuration/specs/config_section_context.py
+-rw-r--r--   0        0        0     1818 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/common/configuration/specs/connection_string_credentials.py
+-rw-r--r--   0        0        0     2125 2023-04-24 18:26:21.111453 dlt-0.3.1a0/dlt/common/configuration/specs/exceptions.py
+-rw-r--r--   0        0        0    12725 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/common/configuration/specs/gcp_credentials.py
+-rw-r--r--   0        0        0      725 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/common/configuration/specs/known_sections.py
+-rw-r--r--   0        0        0     2455 2023-04-30 21:17:44.388805 dlt-0.3.1a0/dlt/common/configuration/specs/run_configuration.py
+-rw-r--r--   0        0        0     6036 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/utils.py
+-rw-r--r--   0        0        0      142 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/data_types/__init__.py
+-rw-r--r--   0        0        0     6306 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/data_types/type_helpers.py
+-rw-r--r--   0        0        0      214 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/data_types/typing.py
+-rw-r--r--   0        0        0      260 2023-03-23 14:48:20.701618 dlt-0.3.1a0/dlt/common/data_writers/__init__.py
+-rw-r--r--   0        0        0     5893 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/common/data_writers/buffered.py
+-rw-r--r--   0        0        0     2400 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/data_writers/escape.py
+-rw-r--r--   0        0        0      962 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/data_writers/exceptions.py
+-rw-r--r--   0        0        0     5159 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/data_writers/writers.py
+-rw-r--r--   0        0        0      189 2023-05-29 18:11:09.008705 dlt-0.3.1a0/dlt/common/destination/__init__.py
+-rw-r--r--   0        0        0     2228 2023-06-13 23:16:30.618251 dlt-0.3.1a0/dlt/common/destination/capabilities.py
+-rw-r--r--   0        0        0    11099 2023-05-29 18:11:09.008705 dlt-0.3.1a0/dlt/common/destination/reference.py
+-rw-r--r--   0        0        0     6465 2023-06-08 07:50:27.863474 dlt-0.3.1a0/dlt/common/exceptions.py
+-rw-r--r--   0        0        0     4954 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/git.py
+-rw-r--r--   0        0        0     5253 2023-05-14 20:33:31.539348 dlt-0.3.1a0/dlt/common/json/__init__.py
+-rw-r--r--   0        0        0     1802 2023-04-10 08:12:53.769595 dlt-0.3.1a0/dlt/common/json/_orjson.py
+-rw-r--r--   0        0        0     2939 2023-04-10 08:12:53.769595 dlt-0.3.1a0/dlt/common/json/_simplejson.py
+-rw-r--r--   0        0        0     1536 2023-04-29 12:58:55.943219 dlt-0.3.1a0/dlt/common/jsonpath.py
+-rw-r--r--   0        0        0      232 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/normalizers/__init__.py
+-rw-r--r--   0        0        0     1197 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/common/normalizers/configuration.py
+-rw-r--r--   0        0        0      472 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/normalizers/exceptions.py
+-rw-r--r--   0        0        0     1644 2023-04-06 15:27:24.759561 dlt-0.3.1a0/dlt/common/normalizers/json/__init__.py
+-rw-r--r--   0        0        0    13382 2023-05-14 20:33:31.539348 dlt-0.3.1a0/dlt/common/normalizers/json/relational.py
+-rw-r--r--   0        0        0       64 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/normalizers/naming/__init__.py
+-rw-r--r--   0        0        0      807 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/normalizers/naming/direct.py
+-rw-r--r--   0        0        0     1069 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/normalizers/naming/duck_case.py
+-rw-r--r--   0        0        0      792 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/normalizers/naming/exceptions.py
+-rw-r--r--   0        0        0     3753 2023-04-05 08:03:40.638919 dlt-0.3.1a0/dlt/common/normalizers/naming/naming.py
+-rw-r--r--   0        0        0     3002 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/normalizers/naming/snake_case.py
+-rw-r--r--   0        0        0      358 2023-04-02 09:09:15.855769 dlt-0.3.1a0/dlt/common/normalizers/typing.py
+-rw-r--r--   0        0        0     2337 2023-04-06 15:27:24.759561 dlt-0.3.1a0/dlt/common/normalizers/utils.py
+-rw-r--r--   0        0        0      451 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/pendulum.py
+-rw-r--r--   0        0        0    18949 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/common/pipeline.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/reflection/__init__.py
+-rw-r--r--   0        0        0      374 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/reflection/function_visitor.py
+-rw-r--r--   0        0        0     4891 2023-04-09 16:39:04.593180 dlt-0.3.1a0/dlt/common/reflection/spec.py
+-rw-r--r--   0        0        0     5069 2023-04-24 18:26:21.111453 dlt-0.3.1a0/dlt/common/reflection/utils.py
+-rw-r--r--   0        0        0      174 2023-04-30 21:17:44.388805 dlt-0.3.1a0/dlt/common/runners/__init__.py
+-rw-r--r--   0        0        0      705 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/common/runners/configuration.py
+-rw-r--r--   0        0        0     2635 2023-05-14 11:08:47.420838 dlt-0.3.1a0/dlt/common/runners/pool_runner.py
+-rw-r--r--   0        0        0     4046 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/common/runners/runnable.py
+-rw-r--r--   0        0        0     3145 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/common/runners/stdout.py
+-rw-r--r--   0        0        0     2137 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/common/runners/synth_pickle.py
+-rw-r--r--   0        0        0      105 2023-04-30 21:17:44.388805 dlt-0.3.1a0/dlt/common/runners/typing.py
+-rw-r--r--   0        0        0     5590 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/common/runners/venv.py
+-rw-r--r--   0        0        0       36 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/common/runtime/__init__.py
+-rw-r--r--   0        0        0    13923 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/common/runtime/collector.py
+-rw-r--r--   0        0        0     4501 2023-05-14 20:33:31.539348 dlt-0.3.1a0/dlt/common/runtime/exec_info.py
+-rw-r--r--   0        0        0      647 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/common/runtime/init.py
+-rw-r--r--   0        0        0     4002 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/common/runtime/logger.py
+-rw-r--r--   0        0        0     2052 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/common/runtime/prometheus.py
+-rw-r--r--   0        0        0     7170 2023-05-14 20:33:31.539348 dlt-0.3.1a0/dlt/common/runtime/segment.py
+-rw-r--r--   0        0        0     2493 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/common/runtime/sentry.py
+-rw-r--r--   0        0        0     2027 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/common/runtime/signals.py
+-rw-r--r--   0        0        0      616 2023-04-03 18:50:36.893525 dlt-0.3.1a0/dlt/common/runtime/slack.py
+-rw-r--r--   0        0        0      720 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/common/runtime/telemetry.py
+-rw-r--r--   0        0        0      387 2023-04-03 18:50:36.893525 dlt-0.3.1a0/dlt/common/schema/__init__.py
+-rw-r--r--   0        0        0     1927 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/common/schema/detections.py
+-rw-r--r--   0        0        0     2974 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/common/schema/exceptions.py
+-rw-r--r--   0        0        0    25164 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/schema/schema.py
+-rw-r--r--   0        0        0     3004 2023-04-22 20:26:30.632198 dlt-0.3.1a0/dlt/common/schema/typing.py
+-rw-r--r--   0        0        0    23080 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/common/schema/utils.py
+-rw-r--r--   0        0        0     1467 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/common/source.py
+-rw-r--r--   0        0        0      554 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/common/storages/__init__.py
+-rw-r--r--   0        0        0     1649 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/common/storages/configuration.py
+-rw-r--r--   0        0        0     1906 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/common/storages/data_item_storage.py
+-rw-r--r--   0        0        0     3107 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/common/storages/exceptions.py
+-rw-r--r--   0        0        0    10891 2023-05-14 20:33:31.539348 dlt-0.3.1a0/dlt/common/storages/file_storage.py
+-rw-r--r--   0        0        0     2690 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/common/storages/live_schema_storage.py
+-rw-r--r--   0        0        0    21812 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/common/storages/load_storage.py
+-rw-r--r--   0        0        0     2409 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/common/storages/normalize_storage.py
+-rw-r--r--   0        0        0     8600 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/common/storages/schema_storage.py
+-rw-r--r--   0        0        0     9486 2023-06-08 07:50:27.863474 dlt-0.3.1a0/dlt/common/storages/transactional_file.py
+-rw-r--r--   0        0        0     2525 2023-04-24 18:26:21.111453 dlt-0.3.1a0/dlt/common/storages/versioned_storage.py
+-rw-r--r--   0        0        0     2634 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/common/time.py
+-rw-r--r--   0        0        0     4736 2023-04-03 18:50:36.893525 dlt-0.3.1a0/dlt/common/typing.py
+-rw-r--r--   0        0        0    14285 2023-06-13 23:16:30.618251 dlt-0.3.1a0/dlt/common/utils.py
+-rw-r--r--   0        0        0     3686 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/common/validation.py
+-rw-r--r--   0        0        0     1185 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/common/wei.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/destinations/__init__.py
+-rw-r--r--   0        0        0      437 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/destinations/bigquery/README.md
+-rw-r--r--   0        0        0     1813 2023-04-05 08:03:40.638919 dlt-0.3.1a0/dlt/destinations/bigquery/__init__.py
+-rw-r--r--   0        0        0    12370 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/destinations/bigquery/bigquery.py
+-rw-r--r--   0        0        0      386 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/destinations/bigquery/configuration.py
+-rw-r--r--   0        0        0    10342 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/destinations/bigquery/sql_client.py
+-rw-r--r--   0        0        0     1935 2023-04-05 08:03:40.638919 dlt-0.3.1a0/dlt/destinations/duckdb/__init__.py
+-rw-r--r--   0        0        0     7207 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/destinations/duckdb/configuration.py
+-rw-r--r--   0        0        0     2754 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/destinations/duckdb/duck.py
+-rw-r--r--   0        0        0     6936 2023-04-21 22:25:54.789942 dlt-0.3.1a0/dlt/destinations/duckdb/sql_client.py
+-rw-r--r--   0        0        0     1671 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/destinations/dummy/__init__.py
+-rw-r--r--   0        0        0      736 2023-04-03 18:50:36.893525 dlt-0.3.1a0/dlt/destinations/dummy/configuration.py
+-rw-r--r--   0        0        0     4989 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/destinations/dummy/dummy.py
+-rw-r--r--   0        0        0     4159 2023-04-05 08:03:40.638919 dlt-0.3.1a0/dlt/destinations/exceptions.py
+-rw-r--r--   0        0        0     1270 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/destinations/filesystem/__init__.py
+-rw-r--r--   0        0        0     2253 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/destinations/filesystem/configuration.py
+-rw-r--r--   0        0        0     4935 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/destinations/filesystem/filesystem.py
+-rw-r--r--   0        0        0     1419 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/destinations/filesystem/filesystem_client.py
+-rw-r--r--   0        0        0     5005 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/destinations/insert_job_client.py
+-rw-r--r--   0        0        0    15639 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/destinations/job_client_impl.py
+-rw-r--r--   0        0        0     1303 2023-04-05 08:03:40.638919 dlt-0.3.1a0/dlt/destinations/job_impl.py
+-rw-r--r--   0        0        0      251 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/destinations/postgres/README.md
+-rw-r--r--   0        0        0     1934 2023-04-05 08:03:40.638919 dlt-0.3.1a0/dlt/destinations/postgres/__init__.py
+-rw-r--r--   0        0        0     1316 2023-05-29 18:11:09.008705 dlt-0.3.1a0/dlt/destinations/postgres/configuration.py
+-rw-r--r--   0        0        0     3025 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/destinations/postgres/postgres.py
+-rw-r--r--   0        0        0     6074 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/destinations/postgres/sql_client.py
+-rw-r--r--   0        0        0     1159 2023-04-03 18:50:36.893525 dlt-0.3.1a0/dlt/destinations/redshift/README.md
+-rw-r--r--   0        0        0     1905 2023-04-05 08:03:40.638919 dlt-0.3.1a0/dlt/destinations/redshift/__init__.py
+-rw-r--r--   0        0        0      570 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/destinations/redshift/configuration.py
+-rw-r--r--   0        0        0     3761 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/destinations/redshift/redshift.py
+-rw-r--r--   0        0        0     7117 2023-05-28 13:56:42.341452 dlt-0.3.1a0/dlt/destinations/sql_client.py
+-rw-r--r--   0        0        0    10090 2023-05-28 13:56:42.341452 dlt-0.3.1a0/dlt/destinations/sql_merge_job.py
+-rw-r--r--   0        0        0     1931 2023-04-24 18:26:21.111453 dlt-0.3.1a0/dlt/destinations/typing.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.1a0/dlt/extract/__init__.py
+-rw-r--r--   0        0        0    26516 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/extract/decorators.py
+-rw-r--r--   0        0        0    12995 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/extract/exceptions.py
+-rw-r--r--   0        0        0     8312 2023-06-13 20:43:40.978251 dlt-0.3.1a0/dlt/extract/extract.py
+-rw-r--r--   0        0        0    14954 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/extract/incremental.py
+-rw-r--r--   0        0        0    32327 2023-06-13 20:43:40.978251 dlt-0.3.1a0/dlt/extract/pipe.py
+-rw-r--r--   0        0        0     9683 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/extract/schema.py
+-rw-r--r--   0        0        0    38391 2023-06-13 20:43:40.978251 dlt-0.3.1a0/dlt/extract/source.py
+-rw-r--r--   0        0        0     4308 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/extract/typing.py
+-rw-r--r--   0        0        0      593 2023-04-06 20:38:35.239561 dlt-0.3.1a0/dlt/extract/utils.py
+-rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.3.1a0/dlt/helpers/__init__.py
+-rw-r--r--   0        0        0    13783 2023-05-28 13:56:42.341452 dlt-0.3.1a0/dlt/helpers/airflow_helper.py
+-rw-r--r--   0        0        0     2907 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/helpers/dbt/__init__.py
+-rw-r--r--   0        0        0     1220 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/helpers/dbt/configuration.py
+-rw-r--r--   0        0        0     6137 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/helpers/dbt/dbt_utils.py
+-rw-r--r--   0        0        0      758 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/helpers/dbt/exceptions.py
+-rw-r--r--   0        0        0     3583 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/helpers/dbt/profiles.yml
+-rw-r--r--   0        0        0    13032 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/helpers/dbt/runner.py
+-rw-r--r--   0        0        0     2490 2023-05-29 14:13:02.438979 dlt-0.3.1a0/dlt/helpers/pandas_helper.py
+-rw-r--r--   0        0        0     1035 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/helpers/parquet.py
+-rw-r--r--   0        0        0    13378 2023-05-29 14:13:02.438979 dlt-0.3.1a0/dlt/helpers/streamlit_helper.py
+-rw-r--r--   0        0        0       31 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/load/__init__.py
+-rw-r--r--   0        0        0     1005 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/load/configuration.py
+-rw-r--r--   0        0        0     1993 2023-04-05 08:03:40.638919 dlt-0.3.1a0/dlt/load/exceptions.py
+-rw-r--r--   0        0        0    19925 2023-06-08 14:19:13.923473 dlt-0.3.1a0/dlt/load/load.py
+-rw-r--r--   0        0        0       32 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/normalize/__init__.py
+-rw-r--r--   0        0        0     1101 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/normalize/configuration.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.1a0/dlt/normalize/exceptions.py
+-rw-r--r--   0        0        0    16538 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/normalize/normalize.py
+-rw-r--r--   0        0        0    13081 2023-05-28 13:56:42.341452 dlt-0.3.1a0/dlt/pipeline/__init__.py
+-rw-r--r--   0        0        0     1858 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/pipeline/configuration.py
+-rw-r--r--   0        0        0      379 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/pipeline/current.py
+-rw-r--r--   0        0        0     4829 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/pipeline/dbt.py
+-rw-r--r--   0        0        0     3100 2023-05-28 13:56:42.341452 dlt-0.3.1a0/dlt/pipeline/exceptions.py
+-rw-r--r--   0        0        0     8733 2023-06-07 08:32:53.271010 dlt-0.3.1a0/dlt/pipeline/helpers.py
+-rw-r--r--   0        0        0      122 2023-04-06 15:27:24.759561 dlt-0.3.1a0/dlt/pipeline/mark.py
+-rw-r--r--   0        0        0    59020 2023-06-07 08:32:53.271010 dlt-0.3.1a0/dlt/pipeline/pipeline.py
+-rw-r--r--   0        0        0      985 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/pipeline/progress.py
+-rw-r--r--   0        0        0     4186 2023-06-07 08:32:53.271010 dlt-0.3.1a0/dlt/pipeline/state_sync.py
+-rw-r--r--   0        0        0     7990 2023-04-03 18:50:36.903525 dlt-0.3.1a0/dlt/pipeline/trace.py
+-rw-r--r--   0        0        0     4625 2023-05-29 18:11:09.018705 dlt-0.3.1a0/dlt/pipeline/track.py
+-rw-r--r--   0        0        0       91 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/pipeline/typing.py
+-rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.3.1a0/dlt/py.typed
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/reflection/__init__.py
+-rw-r--r--   0        0        0      563 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/reflection/names.py
+-rw-r--r--   0        0        0     5617 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/reflection/script_inspector.py
+-rw-r--r--   0        0        0     6186 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/reflection/script_visitor.py
+-rw-r--r--   0        0        0      124 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/sources/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/sources/credentials.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/sources/helpers/__init__.py
+-rw-r--r--   0        0        0      574 2023-03-23 14:48:37.261618 dlt-0.3.1a0/dlt/sources/helpers/requests/__init__.py
+-rw-r--r--   0        0        0     9243 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/sources/helpers/requests/retry.py
+-rw-r--r--   0        0        0     1336 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/sources/helpers/requests/session.py
+-rw-r--r--   0        0        0      679 2023-04-06 15:27:24.759561 dlt-0.3.1a0/dlt/sources/helpers/transform.py
+-rw-r--r--   0        0        0     1125 2023-04-22 20:26:30.632198 dlt-0.3.1a0/dlt/version.py
+-rw-r--r--   0        0        0     4278 2023-06-13 23:16:43.718251 dlt-0.3.1a0/pyproject.toml
+-rw-r--r--   0        0        0     7548 1970-01-01 00:00:00.000000 dlt-0.3.1a0/setup.py
+-rw-r--r--   0        0        0     7546 1970-01-01 00:00:00.000000 dlt-0.3.1a0/PKG-INFO
```

### Comparing `dlt-0.3.1/LICENSE.txt` & `dlt-0.3.1a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/README.md` & `dlt-0.3.1a0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 - **Versatile Usage:** Suitable for ad-hoc exploration to advanced loading infrastructures.
 - **Start in Seconds with CLI:** Powerful CLI for managing, deploying and inspecting local pipelines.
 - **Incremental Loading:** Load only new or changed data and avoid loading old records again.
 - **Open Source:** Free and Apache 2.0 Licensed.
 
 ## Ready to use Sources and Destinations
 
-Explore ready to use sources (e.g. Google Sheets) in the [Verified Sources docs](https://dlthub.com/docs/dlt-ecosystem/verified-sources) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/dlt-ecosystem/destinations).
+Explore ready to use sources (e.g. Google Sheets) in the [Verified Sources docs](https://dlthub.com/docs/verified-sources/chess) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/destinations/bigquery).
 
 ## Documentation
 
 For detailed usage and configuration, please refer to the [official documentation](https://dlthub.com/docs).
 
 ## Examples
```

### Comparing `dlt-0.3.1/dlt/__init__.py` & `dlt-0.3.1a0/dlt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     $ dlt pipeline dlt_magnus_games show
 
 
 Or start with our pipeline template with sample chess.com data loaded to bigquery
 
     $ dlt init chess duckdb
 
-For more detailed info, see https://dlthub.com/docs/walkthroughs
+For more detailed info, see https://dlthub.com/docs/getting-started
 """
 
 from dlt.version import __version__
 from dlt.common.configuration.accessors import config, secrets
 from dlt.common.typing import TSecretValue as _TSecretValue
 from dlt.common.configuration.specs import CredentialsConfiguration as _CredentialsConfiguration
 from dlt.common.pipeline import source_state as state
```

### Comparing `dlt-0.3.1/dlt/cli/_dlt.py` & `dlt-0.3.1a0/dlt/cli/_dlt.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from dlt.common.schema import Schema
 from dlt.common.typing import DictStrAny
 from dlt.common.runners import Venv
 
 import dlt.cli.echo as fmt
 from dlt.cli import utils
 from dlt.cli.init_command import init_command, list_verified_sources_command, DLT_INIT_DOCS_URL, DEFAULT_VERIFIED_SOURCES_REPO
-from dlt.cli.deploy_command import PipelineWasNotRun, deploy_command, DLT_DEPLOY_DOCS_URL, DeploymentMethods, COMMAND_DEPLOY_REPO_LOCATION, SecretFormats
+from dlt.cli.deploy_command import PipelineWasNotRun, deploy_command, DLT_DEPLOY_DOCS_URL, DeploymentMethods, COMMAND_DEPLOY_REPO_LOCATION
 from dlt.cli.pipeline_command import pipeline_command, DLT_PIPELINE_COMMAND_DOCS_URL
 from dlt.cli.telemetry_command import DLT_TELEMETRY_DOCS_URL, change_telemetry_status_command, telemetry_status_command
 from dlt.pipeline.exceptions import CannotRestorePipelineException
 
 
 @utils.track_command("init", False, "source_name", "destination_name")
 def init_command_wrapper(source_name: str, destination_name: str, use_generic_template: bool, repo_location: str, branch: str) -> int:
@@ -38,52 +38,58 @@
         click.secho(str(ex), err=True, fg="red")
         fmt.note("Please refer to %s for further assistance" % fmt.bold(DLT_INIT_DOCS_URL))
         return -1
     return 0
 
 
 @utils.track_command("deploy", False, "deployment_method")
-def deploy_command_wrapper(pipeline_script_path: str, deployment_method: str, repo_location: str, branch: Optional[str] = None, **kwargs: Any
-) -> int:
+def deploy_command_wrapper(
+    pipeline_script_path: str,
+    deployment_method: str,
+    schedule: Optional[str],
+    run_on_push: bool,
+    run_on_dispatch: bool,
+    repo_location: str,
+    branch: Optional[str]) -> int:
     try:
         utils.ensure_git_command("deploy")
     except Exception as ex:
         click.secho(str(ex), err=True, fg="red")
         return -1
 
     from git import InvalidGitRepositoryError, NoSuchPathError
     try:
-        deploy_command(pipeline_script_path=pipeline_script_path, deployment_method=deployment_method, repo_location=repo_location, branch=branch, **kwargs)
+        deploy_command(pipeline_script_path, deployment_method, schedule, run_on_push, run_on_dispatch, repo_location, branch)
     except (CannotRestorePipelineException, PipelineWasNotRun) as ex:
         click.secho(str(ex), err=True, fg="red")
         fmt.note("You must run the pipeline locally successfully at least once in order to deploy it.")
         fmt.note("Please refer to %s for further assistance" % fmt.bold(DLT_DEPLOY_DOCS_URL))
-        return -2
+        return -1
     except InvalidGitRepositoryError:
         click.secho(
             "No git repository found for pipeline script %s." % fmt.bold(pipeline_script_path),
             err=True,
             fg="red"
         )
         fmt.note("If you do not have a repository yet, you can do either of:")
         fmt.note("- Run the following command to initialize new repository: %s" % fmt.bold("git init"))
         fmt.note("- Add your local code to Github as described here: %s" % fmt.bold("https://docs.github.com/en/get-started/importing-your-projects-to-github/importing-source-code-to-github/adding-locally-hosted-code-to-github"))
         fmt.note("Please refer to %s for further assistance" % fmt.bold(DLT_DEPLOY_DOCS_URL))
-        return -3
+        return -1
     except NoSuchPathError as path_ex:
         click.secho(
             "The pipeline script does not exist\n%s" % str(path_ex),
             err=True,
             fg="red"
         )
-        return -4
+        return -1
     except Exception as ex:
         click.secho(str(ex), err=True, fg="red")
         fmt.note("Please refer to %s for further assistance" % fmt.bold(DLT_DEPLOY_DOCS_URL))
-        return -5
+        return -1
         # TODO: display stack trace if with debug flag
     return 0
 
 
 @utils.track_command("pipeline", True, "operation")
 def pipeline_command_wrapper(
         operation: str, pipeline_name: str, pipelines_dir: str, verbosity: int, **command_kwargs: Any
@@ -98,15 +104,15 @@
     except Exception as ex:
         click.secho(str(ex), err=True, fg="red")
         return 1
 
 
 @utils.track_command("schema", False, "operation")
 def schema_command_wrapper(file_path: str, format_: str, remove_defaults: bool) -> int:
-    with open(file_path, "rb") as f:
+    with open(file_path, "br") as f:
         if os.path.splitext(file_path)[1][1:] == "json":
             schema_dict: DictStrAny = json.load(f)
         else:
             schema_dict = yaml.safe_load(f)
     s = Schema.from_dict(schema_dict)
     if format_ == "json":
         schema_str = json.dumps(s.to_dict(remove_defaults=remove_defaults), pretty=True)
@@ -186,30 +192,27 @@
     init_cmd.add_argument("--list-verified-sources", "-l",  default=False, action="store_true", help="List available verified sources")
     init_cmd.add_argument("source", nargs='?', help="Name of data source for which to create a pipeline. Adds existing verified source or creates a new pipeline template if verified source for your data source is not yet implemented.")
     init_cmd.add_argument("destination", nargs='?', help="Name of a destination ie. bigquery or redshift")
     init_cmd.add_argument("--location", default=DEFAULT_VERIFIED_SOURCES_REPO, help="Advanced. Uses a specific url or local path to verified sources repository.")
     init_cmd.add_argument("--branch", default=None, help="Advanced. Uses specific branch of the init repository to fetch the template.")
     init_cmd.add_argument("--generic", default=False, action="store_true", help="When present uses a generic template with all the dlt loading code present will be used. Otherwise a debug template is used that can be immediately run to get familiar with the dlt sources.")
 
-    # deploy
     deploy_cmd = subparsers.add_parser("deploy", help="Creates a deployment package for a selected pipeline script")
     deploy_cmd.add_argument("pipeline_script_path", metavar="pipeline-script-path", help="Path to a pipeline script")
+    deploy_cmd.add_argument(
+        "deployment_method",
+        metavar="deployment-method",
+        choices=list(map(lambda value: value.value, DeploymentMethods.__members__.values())),
+        default=DeploymentMethods.github_actions.value,
+        help="Deployment method: %s" % ", ".join(map(lambda value: value.value, DeploymentMethods.__members__.values())))
     deploy_cmd.add_argument("--schedule", required=False, help="A schedule with which to run the pipeline, in cron format. Example: '*/30 * * * *' will run the pipeline every 30 minutes.")
+    deploy_cmd.add_argument("--run-manually", default=True, action="store_true", help="Allows the pipeline to be run manually form Github Actions UI.")
+    deploy_cmd.add_argument("--run-on-push", default=False, action="store_true", help="Runs the pipeline with every push to the repository.")
     deploy_cmd.add_argument("--location", default=COMMAND_DEPLOY_REPO_LOCATION, help="Advanced. Uses a specific url or local path to pipelines repository.")
     deploy_cmd.add_argument("--branch", default=None, help="Advanced. Uses specific branch of the deploy repository to fetch the template.")
-    deploy_sub_parsers = deploy_cmd.add_subparsers(dest="deployment_method")
-
-    # deploy github actions
-    deploy_github_cmd = deploy_sub_parsers.add_parser(DeploymentMethods.github_actions.value, help="Deploys the pipeline to Github Actions")
-    deploy_github_cmd.add_argument("--run-manually", default=True, action="store_true", help="Allows the pipeline to be run manually form Github Actions UI.")
-    deploy_github_cmd.add_argument("--run-on-push", default=False, action="store_true", help="Runs the pipeline with every push to the repository.")
-
-    # deploy airflow composer
-    deploy_airflow_cmd = deploy_sub_parsers.add_parser(DeploymentMethods.airflow_composer.value, help="Deploys the pipeline to Airflow")
-    deploy_airflow_cmd.add_argument("--secrets-format", default=SecretFormats.env, choices=[v.value for v in SecretFormats], required=False, help="Format of the secrets")
 
     schema = subparsers.add_parser("schema", help="Shows, converts and upgrades schemas")
     schema.add_argument("file", help="Schema file name, in yaml or json format, will autodetect based on extension")
     schema.add_argument("--format", choices=["json", "yaml"], default="yaml", help="Display schema in this format")
     schema.add_argument("--remove-defaults", action="store_true", help="Does not show default hint values")
 
     pipe_cmd = subparsers.add_parser("pipeline", help="Operations on pipelines that were ran locally")
@@ -278,22 +281,15 @@
         else:
             if not args.source or not args.destination:
                 init_cmd.print_usage()
                 return -1
             else:
                 return init_command_wrapper(args.source, args.destination, args.generic, args.location, args.branch)
     elif args.command == "deploy":
-        deploy_args = vars(args)
-        return deploy_command_wrapper(
-            pipeline_script_path=deploy_args.pop("pipeline_script_path"),
-            deployment_method=deploy_args.pop("deployment_method"),
-            repo_location=deploy_args.pop("location"),
-            branch=deploy_args.pop("branch"),
-            **deploy_args
-        )
+        return deploy_command_wrapper(args.pipeline_script_path, args.deployment_method, args.schedule, args.run_on_push, args.run_manually, args.location, args.branch)
     elif args.command == "telemetry":
         return telemetry_status_command_wrapper()
     else:
         print_help(parser)
         return -1
```

### Comparing `dlt-0.3.1/dlt/cli/config_toml_writer.py` & `dlt-0.3.1a0/dlt/cli/config_toml_writer.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/cli/deploy_command.py` & `dlt-0.3.1a0/dlt/cli/deploy_command.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,60 +1,75 @@
 import os
-from typing import Optional, Any, Type
+from typing import Optional, Any
 import yaml
 from enum import Enum
 from importlib.metadata import version as pkg_version
 
-from dlt.common.configuration.providers import SECRETS_TOML, SECRETS_TOML_KEY, StringTomlProvider
+from dlt.common.configuration.providers import SECRETS_TOML
 from dlt.common.configuration.paths import make_dlt_settings_path
 from dlt.common.configuration.utils import serialize_value
 from dlt.common.git import is_dirty
 
 from dlt.cli import utils
 from dlt.cli import echo as fmt
-from dlt.cli.deploy_command_helpers import (PipelineWasNotRun, BaseDeployment, ask_files_overwrite, generate_pip_freeze, github_origin_to_url, serialize_templated_yaml,
-                                            wrap_template_str)
+from dlt.cli.deploy_command_helpers import (BaseDeployment, ask_files_overwrite, generate_pip_freeze, github_origin_to_url, serialize_templated_yaml,
+                                            wrap_template_str, PipelineWasNotRun)
 
 from dlt.version import DLT_PKG_NAME
 
 from dlt.common.destination.reference import DestinationReference
 
 REQUIREMENTS_GITHUB_ACTION = "requirements_github_action.txt"
 DLT_DEPLOY_DOCS_URL = "https://dlthub.com/docs/walkthroughs/deploy-a-pipeline"
-DLT_AIRFLOW_GCP_DOCS_URL = "https://dlthub.com/docs/walkthroughs/deploy-a-pipeline/deploy-with-airflow-composer"
+DLT_AIRFLOW_GCP_DOCS_URL = "https://dlthub.com/docs/running-in-production/orchestrators/airflow-gcp-cloud-composer"
 AIRFLOW_GETTING_STARTED = "https://airflow.apache.org/docs/apache-airflow/stable/start.html"
 AIRFLOW_DAG_TEMPLATE_SCRIPT = "dag_template.py"
 AIRFLOW_CLOUDBUILD_YAML = "cloudbuild.yaml"
 COMMAND_REPO_LOCATION = "https://github.com/dlt-hub/dlt-%s-template.git"
 COMMAND_DEPLOY_REPO_LOCATION = COMMAND_REPO_LOCATION % "deploy"
 
 
 class DeploymentMethods(Enum):
     github_actions = "github-action"
     airflow_composer = "airflow-composer"
 
 
-class SecretFormats(Enum):
-    env = "env"
-    toml = "toml"
-
-
-def deploy_command(pipeline_script_path: str, deployment_method: str, repo_location: str, branch: Optional[str] = None, **kwargs: Any
+def deploy_command(
+    pipeline_script_path: str,
+    deployment_method: str,
+    schedule: Optional[str],
+    run_on_push: bool,
+    run_on_dispatch: bool,
+    repo_location: str,
+    branch: Optional[str] = None,
 ) -> None:
-
     # get current repo local folder
-    deployment_class: Type[BaseDeployment] = None
+    deployment_obj: BaseDeployment = None
     if deployment_method == DeploymentMethods.github_actions.value:
-        deployment_class = GithubActionDeployment
+        deployment_obj = GithubActionDeployment(
+            pipeline_script_path=pipeline_script_path,
+            schedule=schedule,
+            run_on_push=run_on_push,
+            run_on_dispatch=run_on_dispatch,
+            repo_location=repo_location,
+            branch=branch
+        )
     elif deployment_method == DeploymentMethods.airflow_composer.value:
-        deployment_class = AirflowDeployment
+        deployment_obj = AirflowDeployment(
+            pipeline_script_path=pipeline_script_path,
+            schedule=schedule,
+            run_on_push=run_on_push,
+            run_on_dispatch=run_on_dispatch,
+            repo_location=repo_location,
+            branch=branch
+        )
     else:
         raise ValueError(f"Deployment method '{deployment_method}' is not supported. Only {', '.join([m.value for m in DeploymentMethods])} are available.'")
 
-    deployment_class(pipeline_script_path=pipeline_script_path, location=repo_location, branch=branch, **kwargs).run_deployment()
+    deployment_obj.run_deployment()
 
 
 class GithubActionDeployment(BaseDeployment):
     def _generate_workflow(self, *args: Optional[Any]) -> None:
         self.deployment_method = DeploymentMethods.github_actions.value
         if self.schedule_description is None:
             raise ValueError(
@@ -229,36 +244,23 @@
         ))
         fmt.echo("2. Set _BUCKET_NAME up in %s/%s file. " % (
             fmt.bold(utils.AIRFLOW_BUILD_FOLDER), fmt.bold(AIRFLOW_CLOUDBUILD_YAML),
         ))
         if len(self.secret_envs) == 0 and len(self.envs) == 0:
             fmt.echo("3. Your pipeline does not seem to need any secrets.")
         else:
-            if self.secrets_format == SecretFormats.env.value:
-                fmt.echo("3. Add the following secret values (typically stored in %s): \n%s\n%s\nin ENVIRONMENT VARIABLES using Google Composer UI" % (
-                    fmt.bold(make_dlt_settings_path(SECRETS_TOML)),
-                    fmt.bold("\n".join(self.env_prov.get_key_name(s_v.key, *s_v.sections) for s_v in self.secret_envs)),
-                    fmt.bold("\n".join(self.env_prov.get_key_name(v.key, *v.sections) for v in self.envs)),
-                ))
-                fmt.echo()
-                # if fmt.confirm("Do you want to list the environment variables in the format suitable for Airflow?", default=True):
-                self._echo_secrets()
-                self._echo_envs()
-            elif self.secrets_format == SecretFormats.toml.value:
-                # build toml
-                fmt.echo(f"3. Add the following toml-string in the Google Composer UI as the {SECRETS_TOML_KEY} variable.")
-                fmt.echo()
-                toml_provider = StringTomlProvider("")
-                for s_v in self.secret_envs:
-                    toml_provider.set_value(s_v.key, s_v.value, None, *s_v.sections)
-                for s_v in self.envs:
-                    toml_provider.set_value(s_v.key, s_v.value, None, *s_v.sections)
-                fmt.echo(toml_provider.dumps())
-            else:
-                raise ValueError(self.secrets_format)
+            fmt.echo("3. Add the following secret values (typically stored in %s): \n%s\n%s\nin ENVIRONMENT VARIABLES using Google Composer UI" % (
+                fmt.bold(make_dlt_settings_path(SECRETS_TOML)),
+                fmt.bold("\n".join(self.env_prov.get_key_name(s_v.key, *s_v.sections) for s_v in self.secret_envs)),
+                fmt.bold("\n".join(self.env_prov.get_key_name(v.key, *v.sections) for v in self.envs)),
+            ))
+            fmt.echo()
+            # if fmt.confirm("Do you want to list the environment variables in the format suitable for Airflow?", default=True):
+            self._echo_secrets()
+            self._echo_envs()
 
         fmt.echo("4. Add dlt package below using Google Composer UI.")
         fmt.echo(fmt.bold(self.artifacts["requirements_txt"]))
         fmt.note("You may need to add more packages ie. when your source requires additional dependencies")
         fmt.echo("5. Commit and push the pipeline files to github:")
         fmt.echo("a. Add stage deployment files to commit. Use your Git UI or the following command")
```

### Comparing `dlt-0.3.1/dlt/cli/deploy_command_helpers.py` & `dlt-0.3.1a0/dlt/cli/deploy_command_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,29 +33,26 @@
 GITHUB_URL = "https://github.com/"
 
 
 class BaseDeployment(abc.ABC):
     def __init__(
         self,
         pipeline_script_path: str,
-        location: str,
         schedule: Optional[str],
-        run_on_push: bool = False,
-        run_on_dispatch: bool = False,
-        branch: Optional[str] = None,
-        secrets_format: Optional[str] = None,
-        **_kwargs: Any
+        run_on_push: bool,
+        run_on_dispatch: bool,
+        repo_location: str,
+        branch: Optional[str] = None
     ):
         self.pipeline_script_path = pipeline_script_path
         self.schedule = schedule
         self.run_on_push = run_on_push
         self.run_on_dispatch = run_on_dispatch
-        self.repo_location = location
+        self.repo_location = repo_location
         self.branch = branch
-        self.secrets_format = secrets_format
 
         self.pipelines_dir: Optional[str] = None
         self.pipeline_name: Optional[str] = None
 
         self.deployment_method: str
         self.repo: Repo
         self.repo_storage: FileStorage
```

### Comparing `dlt-0.3.1/dlt/cli/echo.py` & `dlt-0.3.1a0/dlt/cli/echo.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/cli/init_command.py` & `dlt-0.3.1a0/dlt/cli/init_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/cli/pipeline_command.py` & `dlt-0.3.1a0/dlt/cli/pipeline_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/cli/pipeline_files.py` & `dlt-0.3.1a0/dlt/cli/pipeline_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
             posix_file = posixpath.join(*Path(posix_file).parts)
             try:
                 blob_sha3 = tree.join(posix_file).hexsha
             except KeyError:
                 # if directory is dirty and we do not have git sha
                 blob_sha3 = None
 
-            with open(os.path.join(repo_path, file), "rb") as f:
+            with open(os.path.join(repo_path, file), "br") as f:
                 file_blob = f.read()
             files_sha[file] = {
                 "commit_sha": commit_sha,
                 "git_sha": blob_sha3,
                 "sha3_256":  hashlib.sha3_256(file_blob).hexdigest()
             }
 
@@ -221,15 +221,15 @@
     dest_storage: FileStorage
 ) -> Tuple[List[str], List[str]]:
     """Use files index from .sources to identify modified files via sha3 content hash"""
 
     conflict_modified: List[str] = []
 
     def is_file_modified(file: str, entry: TVerifiedSourceFileEntry) -> bool:
-        with dest_storage.open_file(file, "rb") as f:
+        with dest_storage.open_file(file, "br") as f:
             file_blob = f.read()
         # file exists but was not changed
         return hashlib.sha3_256(file_blob).hexdigest() != entry["sha3_256"]
 
     for file, entry in remote_new.items():
         if dest_storage.has_file(file):
             # if incoming file is different from local
```

### Comparing `dlt-0.3.1/dlt/cli/source_detection.py` & `dlt-0.3.1a0/dlt/cli/source_detection.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/cli/telemetry_command.py` & `dlt-0.3.1a0/dlt/cli/telemetry_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/cli/utils.py` & `dlt-0.3.1a0/dlt/cli/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/arithmetics.py` & `dlt-0.3.1a0/dlt/common/arithmetics.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/configuration/accessors.py` & `dlt-0.3.1a0/dlt/common/configuration/accessors.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/configuration/container.py` & `dlt-0.3.1a0/dlt/common/configuration/container.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/configuration/exceptions.py` & `dlt-0.3.1a0/dlt/common/configuration/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/configuration/inject.py` & `dlt-0.3.1a0/dlt/common/configuration/inject.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/configuration/paths.py` & `dlt-0.3.1a0/dlt/common/configuration/paths.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/configuration/providers/airflow.py` & `dlt-0.3.1a0/dlt/common/configuration/providers/airflow.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/configuration/providers/context.py` & `dlt-0.3.1a0/dlt/common/configuration/providers/context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/configuration/providers/dictionary.py` & `dlt-0.3.1a0/dlt/common/configuration/providers/dictionary.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/configuration/providers/environ.py` & `dlt-0.3.1a0/dlt/common/configuration/providers/environ.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/configuration/providers/google_secrets.py` & `dlt-0.3.1a0/dlt/common/configuration/providers/google_secrets.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/configuration/providers/provider.py` & `dlt-0.3.1a0/dlt/common/configuration/providers/provider.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/configuration/providers/toml.py` & `dlt-0.3.1a0/dlt/common/configuration/providers/toml.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,35 +80,14 @@
         return True
 
     @property
     def is_empty(self) -> bool:
         return len(self._toml.body) == 0
 
 
-class StringTomlProvider(BaseTomlProvider):
-
-    def __init__(self, toml_string: str) -> None:
-        super().__init__(StringTomlProvider.loads(toml_string))
-
-    def dumps(self) -> str:
-        return tomlkit.dumps(self._toml)
-
-    @staticmethod
-    def loads(toml_string: str) -> tomlkit.TOMLDocument:
-        return tomlkit.parse(toml_string)
-
-    @property
-    def supports_secrets(self) -> bool:
-        return True
-
-    @property
-    def name(self) -> str:
-        return "memory"
-
-
 class VaultTomlProvider(BaseTomlProvider):
     """A toml-backed Vault abstract config provider.
 
     This provider allows implementation of providers that store secrets in external vaults: like Hashicorp, Google Secrets or Airflow Metadata.
     The basic working principle is obtain config and secrets values from Vault keys and reconstitute a `secrets.toml` like document that is then used
     as a cache.
```

### Comparing `dlt-0.3.1/dlt/common/configuration/resolve.py` & `dlt-0.3.1a0/dlt/common/configuration/resolve.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/configuration/specs/__init__.py` & `dlt-0.3.1a0/dlt/common/configuration/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/configuration/specs/api_credentials.py` & `dlt-0.3.1a0/dlt/common/configuration/specs/api_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/configuration/specs/aws_credentials.py` & `dlt-0.3.1a0/dlt/common/configuration/specs/aws_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/configuration/specs/base_configuration.py` & `dlt-0.3.1a0/dlt/common/configuration/specs/base_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/configuration/specs/config_providers_context.py` & `dlt-0.3.1a0/dlt/common/configuration/specs/config_providers_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/configuration/specs/config_section_context.py` & `dlt-0.3.1a0/dlt/common/configuration/specs/config_section_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/configuration/specs/connection_string_credentials.py` & `dlt-0.3.1a0/dlt/common/configuration/specs/connection_string_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/configuration/specs/exceptions.py` & `dlt-0.3.1a0/dlt/common/configuration/specs/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/configuration/specs/gcp_credentials.py` & `dlt-0.3.1a0/dlt/common/configuration/specs/gcp_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/configuration/specs/known_sections.py` & `dlt-0.3.1a0/dlt/common/configuration/specs/known_sections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/configuration/specs/run_configuration.py` & `dlt-0.3.1a0/dlt/common/configuration/specs/run_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/configuration/utils.py` & `dlt-0.3.1a0/dlt/common/configuration/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/data_types/type_helpers.py` & `dlt-0.3.1a0/dlt/common/data_types/type_helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/data_writers/buffered.py` & `dlt-0.3.1a0/dlt/common/data_writers/buffered.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import gzip
 from typing import List, IO, Any, Optional, Type
 
 from dlt.common.utils import uniq_id
 from dlt.common.typing import TDataItem, TDataItems
 from dlt.common.data_writers import TLoaderFileFormat
 from dlt.common.data_writers.exceptions import BufferedDataWriterClosed, DestinationCapabilitiesRequired, InvalidFileNameTemplateException
 from dlt.common.data_writers.writers import DataWriter
@@ -15,46 +14,42 @@
 class BufferedDataWriter:
 
     @configspec
     class BufferedDataWriterConfiguration(BaseConfiguration):
         buffer_max_items: int = 5000
         file_max_items: Optional[int] = None
         file_max_bytes: Optional[int] = None
-        disable_compression: bool = False
         _caps: Optional[DestinationCapabilitiesContext] = None
 
         __section__ = known_sections.DATA_WRITER
 
 
     @with_config(spec=BufferedDataWriterConfiguration)
     def __init__(
         self,
         file_format: TLoaderFileFormat,
         file_name_template: str,
         *,
         buffer_max_items: int = 5000,
         file_max_items: int = None,
         file_max_bytes: int = None,
-        disable_compression: bool = False,
         _caps: DestinationCapabilitiesContext = None
     ):
         self.file_format = file_format
         self._file_format_spec = DataWriter.data_format_from_file_format(self.file_format)
         if self._file_format_spec.requires_destination_capabilities and not _caps:
             raise DestinationCapabilitiesRequired(file_format)
         self._caps = _caps
         # validate if template has correct placeholders
         self.file_name_template = file_name_template
         self.closed_files: List[str] = []  # all fully processed files
         # buffered items must be less than max items in file
         self.buffer_max_items = min(buffer_max_items, file_max_items or buffer_max_items)
         self.file_max_bytes = file_max_bytes
         self.file_max_items = file_max_items
-        # the open function is either gzip.open or open
-        self.open = gzip.open if self._file_format_spec.supports_compression and not disable_compression else open
 
         self._current_columns: TTableSchemaColumns = None
         self._file_name: str = None
         self._buffered_items: List[TDataItem] = []
         self._writer: DataWriter = None
         self._file: IO[Any] = None
         self._closed = False
@@ -111,17 +106,17 @@
 
     def _flush_items(self) -> None:
         if len(self._buffered_items) > 0:
             # we only open a writer when there are any items in the buffer and first flush is requested
             if not self._writer:
                 # create new writer and write header
                 if self._file_format_spec.is_binary_format:
-                    self._file = self.open(self._file_name, "wb") # type: ignore
+                    self._file = open(self._file_name, "wb")
                 else:
-                    self._file = self.open(self._file_name, "wt", encoding="utf-8") # type: ignore
+                    self._file = open(self._file_name, "wt", encoding="utf-8")
                 self._writer = DataWriter.from_file_format(self.file_format, self._file, caps=self._caps)
                 self._writer.write_header(self._current_columns)
             # write buffer
             self._writer.write_data(self._buffered_items)
             self._buffered_items.clear()
 
     def _flush_and_close_file(self) -> None:
```

### Comparing `dlt-0.3.1/dlt/common/data_writers/escape.py` & `dlt-0.3.1a0/dlt/common/data_writers/escape.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/data_writers/exceptions.py` & `dlt-0.3.1a0/dlt/common/data_writers/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/data_writers/writers.py` & `dlt-0.3.1a0/dlt/common/data_writers/writers.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 @dataclass
 class TFileFormatSpec:
     file_format: TLoaderFileFormat
     file_extension: str
     is_binary_format: bool
     supports_schema_changes: bool
     requires_destination_capabilities: bool = False
-    supports_compression: bool = False
 
 
 class DataWriter(abc.ABC):
     def __init__(self, f: IO[Any], caps: DestinationCapabilitiesContext = None) -> None:
         self._f = f
         self._caps = caps
         self.items_count = 0
@@ -83,42 +82,30 @@
             self._f.write(b"\n")
 
     def write_footer(self) -> None:
         pass
 
     @classmethod
     def data_format(cls) -> TFileFormatSpec:
-        return TFileFormatSpec(
-            "jsonl",
-            file_extension="jsonl",
-            is_binary_format=True,
-            supports_schema_changes=True,
-            supports_compression=True,
-        )
+        return TFileFormatSpec("jsonl", "jsonl", True, True)
 
 
 class JsonlListPUAEncodeWriter(JsonlWriter):
 
     def write_data(self, rows: Sequence[Any]) -> None:
         # skip JsonlWriter when calling super
         super(JsonlWriter, self).write_data(rows)
         # write all rows as one list which will require to write just one line
         # encode types with PUA characters
         json.typed_dump(rows, self._f)
         self._f.write(b"\n")
 
     @classmethod
     def data_format(cls) -> TFileFormatSpec:
-        return TFileFormatSpec(
-            "puae-jsonl",
-            file_extension="jsonl",
-            is_binary_format=True,
-            supports_schema_changes=True,
-            supports_compression=True,
-        )
+        return TFileFormatSpec("puae-jsonl", "jsonl", True, True)
 
 
 class InsertValuesWriter(DataWriter):
 
     def __init__(self, f: IO[Any], caps: DestinationCapabilitiesContext = None) -> None:
         super().__init__(f, caps)
         self._chunks_written = 0
@@ -161,15 +148,8 @@
 
     def write_footer(self) -> None:
         assert self._chunks_written > 0
         self._f.write(";")
 
     @classmethod
     def data_format(cls) -> TFileFormatSpec:
-        return TFileFormatSpec(
-            "insert_values",
-            file_extension="insert_values",
-            is_binary_format=False,
-            supports_schema_changes=False,
-            supports_compression=True,
-            requires_destination_capabilities=True,
-        )
+        return TFileFormatSpec("insert_values", "insert_values", False, False, requires_destination_capabilities=True)
```

### Comparing `dlt-0.3.1/dlt/common/destination/capabilities.py` & `dlt-0.3.1a0/dlt/common/destination/capabilities.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/destination/reference.py` & `dlt-0.3.1a0/dlt/common/destination/reference.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/exceptions.py` & `dlt-0.3.1a0/dlt/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/git.py` & `dlt-0.3.1a0/dlt/common/git.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/json/__init__.py` & `dlt-0.3.1a0/dlt/common/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/json/_orjson.py` & `dlt-0.3.1a0/dlt/common/json/_orjson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/json/_simplejson.py` & `dlt-0.3.1a0/dlt/common/json/_simplejson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/jsonpath.py` & `dlt-0.3.1a0/dlt/common/jsonpath.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/normalizers/configuration.py` & `dlt-0.3.1a0/dlt/common/normalizers/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/normalizers/json/__init__.py` & `dlt-0.3.1a0/dlt/common/normalizers/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/normalizers/json/relational.py` & `dlt-0.3.1a0/dlt/common/normalizers/json/relational.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/normalizers/naming/direct.py` & `dlt-0.3.1a0/dlt/common/normalizers/naming/direct.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/normalizers/naming/duck_case.py` & `dlt-0.3.1a0/dlt/common/normalizers/naming/duck_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/normalizers/naming/exceptions.py` & `dlt-0.3.1a0/dlt/common/normalizers/naming/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/normalizers/naming/naming.py` & `dlt-0.3.1a0/dlt/common/normalizers/naming/naming.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/normalizers/naming/snake_case.py` & `dlt-0.3.1a0/dlt/common/normalizers/naming/snake_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/normalizers/utils.py` & `dlt-0.3.1a0/dlt/common/normalizers/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/pipeline.py` & `dlt-0.3.1a0/dlt/common/pipeline.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/reflection/spec.py` & `dlt-0.3.1a0/dlt/common/reflection/spec.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/reflection/utils.py` & `dlt-0.3.1a0/dlt/common/reflection/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/runners/configuration.py` & `dlt-0.3.1a0/dlt/common/runners/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/runners/pool_runner.py` & `dlt-0.3.1a0/dlt/common/runners/pool_runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/runners/runnable.py` & `dlt-0.3.1a0/dlt/common/runners/runnable.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/runners/stdout.py` & `dlt-0.3.1a0/dlt/common/runners/stdout.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/runners/synth_pickle.py` & `dlt-0.3.1a0/dlt/common/runners/synth_pickle.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/runners/venv.py` & `dlt-0.3.1a0/dlt/common/runners/venv.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/runtime/collector.py` & `dlt-0.3.1a0/dlt/common/runtime/collector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/runtime/exec_info.py` & `dlt-0.3.1a0/dlt/common/runtime/exec_info.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/runtime/init.py` & `dlt-0.3.1a0/dlt/common/runtime/init.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/runtime/logger.py` & `dlt-0.3.1a0/dlt/common/runtime/logger.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/runtime/prometheus.py` & `dlt-0.3.1a0/dlt/common/runtime/prometheus.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/runtime/segment.py` & `dlt-0.3.1a0/dlt/common/runtime/segment.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/runtime/sentry.py` & `dlt-0.3.1a0/dlt/common/runtime/sentry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/runtime/signals.py` & `dlt-0.3.1a0/dlt/common/runtime/signals.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/runtime/slack.py` & `dlt-0.3.1a0/dlt/common/runtime/slack.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/runtime/telemetry.py` & `dlt-0.3.1a0/dlt/common/runtime/telemetry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/schema/detections.py` & `dlt-0.3.1a0/dlt/common/schema/detections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/schema/exceptions.py` & `dlt-0.3.1a0/dlt/common/schema/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/schema/schema.py` & `dlt-0.3.1a0/dlt/common/schema/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/schema/typing.py` & `dlt-0.3.1a0/dlt/common/schema/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/schema/utils.py` & `dlt-0.3.1a0/dlt/common/schema/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/source.py` & `dlt-0.3.1a0/dlt/common/source.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/storages/__init__.py` & `dlt-0.3.1a0/dlt/common/storages/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/storages/configuration.py` & `dlt-0.3.1a0/dlt/common/storages/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/storages/data_item_storage.py` & `dlt-0.3.1a0/dlt/common/storages/data_item_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/storages/exceptions.py` & `dlt-0.3.1a0/dlt/common/storages/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/storages/file_storage.py` & `dlt-0.3.1a0/dlt/common/storages/file_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-import gzip
 import os
 import re
 import stat
 import errno
 import tempfile
 import shutil
 import pathvalidate
-from typing import IO, Any, Optional, List, cast
+from typing import IO, Any, List
 from dlt.common.typing import AnyFun
 
 from dlt.common.utils import encoding_for_mode, uniq_id
 
 
 FILE_COMPONENT_INVALID_CHARACTERS = re.compile(r"[.%{}]")
 
@@ -88,16 +87,14 @@
                 os.rmdir(folder_path)
         else:
             raise NotADirectoryError(folder_path)
 
     def open_file(self, relative_path: str, mode: str = "r") -> IO[Any]:
         if "b" not in mode and "t" not in mode:
             mode = mode + self.file_type
-        if "r" in mode:
-            return FileStorage.open_zipsafe_ro(self.make_full_path(relative_path), mode)
         return open(self.make_full_path(relative_path), mode, encoding=encoding_for_mode(mode))
 
     def open_temp(self, delete: bool = False, mode: str = "w", file_type: str = None) -> IO[Any]:
         mode = mode + file_type or self.file_type
         return tempfile.NamedTemporaryFile(dir=self.storage_path, mode=mode, delete=delete, encoding=encoding_for_mode(mode))
 
     def has_file(self, relative_path: str) -> bool:
@@ -250,23 +247,7 @@
     def rmtree_del_ro(action: AnyFun, name: str, exc: Any) -> Any:
         if action is os.unlink or action is os.remove or action is os.rmdir:
             os.chmod(name, stat.S_IWRITE)
             if os.path.isdir(name):
                 os.rmdir(name)
             else:
                 os.remove(name)
-
-    @staticmethod
-    def open_zipsafe_ro(path: str, mode: str = "r", **kwargs: Any) -> IO[Any]:
-        """Opens a file using gzip.open if it is a gzip file, otherwise uses open."""
-        assert "r" in mode, "FileStorage.open_zipsafe_ro only supports read modes"
-        encoding = kwargs.pop("encoding", encoding_for_mode(mode))
-        origmode = str(mode)
-        try:
-            if encoding is not None and mode == "r":
-                mode += "t"  # gzip requires text mode explicitly to use encoding
-            f = gzip.open(path, mode, encoding=encoding, **kwargs)
-            # Force gzip to read the first few bytes and check the magic number
-            f.read(2), f.seek(0)
-            return cast(IO[Any], f)
-        except (gzip.BadGzipFile, OSError):
-            return open(path, origmode, encoding=encoding, **kwargs)
```

### Comparing `dlt-0.3.1/dlt/common/storages/live_schema_storage.py` & `dlt-0.3.1a0/dlt/common/storages/live_schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/storages/load_storage.py` & `dlt-0.3.1a0/dlt/common/storages/load_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/storages/normalize_storage.py` & `dlt-0.3.1a0/dlt/common/storages/normalize_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/storages/schema_storage.py` & `dlt-0.3.1a0/dlt/common/storages/schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/storages/transactional_file.py` & `dlt-0.3.1a0/dlt/common/storages/transactional_file.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/storages/versioned_storage.py` & `dlt-0.3.1a0/dlt/common/storages/versioned_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/time.py` & `dlt-0.3.1a0/dlt/common/time.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/typing.py` & `dlt-0.3.1a0/dlt/common/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/utils.py` & `dlt-0.3.1a0/dlt/common/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/validation.py` & `dlt-0.3.1a0/dlt/common/validation.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/common/wei.py` & `dlt-0.3.1a0/dlt/common/wei.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/destinations/bigquery/__init__.py` & `dlt-0.3.1a0/dlt/destinations/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/destinations/bigquery/bigquery.py` & `dlt-0.3.1a0/dlt/destinations/bigquery/bigquery.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/destinations/bigquery/sql_client.py` & `dlt-0.3.1a0/dlt/destinations/bigquery/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/destinations/duckdb/__init__.py` & `dlt-0.3.1a0/dlt/destinations/duckdb/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/destinations/duckdb/configuration.py` & `dlt-0.3.1a0/dlt/destinations/duckdb/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/destinations/duckdb/duck.py` & `dlt-0.3.1a0/dlt/destinations/duckdb/duck.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/destinations/duckdb/sql_client.py` & `dlt-0.3.1a0/dlt/destinations/duckdb/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/destinations/dummy/__init__.py` & `dlt-0.3.1a0/dlt/destinations/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/destinations/dummy/configuration.py` & `dlt-0.3.1a0/dlt/destinations/dummy/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/destinations/dummy/dummy.py` & `dlt-0.3.1a0/dlt/destinations/dummy/dummy.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/destinations/exceptions.py` & `dlt-0.3.1a0/dlt/destinations/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/destinations/filesystem/__init__.py` & `dlt-0.3.1a0/dlt/destinations/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/destinations/filesystem/configuration.py` & `dlt-0.3.1a0/dlt/destinations/filesystem/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/destinations/filesystem/filesystem.py` & `dlt-0.3.1a0/dlt/destinations/filesystem/filesystem.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/destinations/filesystem/filesystem_client.py` & `dlt-0.3.1a0/dlt/destinations/filesystem/filesystem_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/destinations/insert_job_client.py` & `dlt-0.3.1a0/dlt/destinations/insert_job_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     def exception(self) -> str:
         # this part of code should be never reached
         raise NotImplementedError()
 
     def _insert(self, qualified_table_name: str, write_disposition: TWriteDisposition, file_path: str) -> Iterator[List[str]]:
         # WARNING: maximum redshift statement is 16MB https://docs.aws.amazon.com/redshift/latest/dg/c_redshift-sql.html
         # the procedure below will split the inserts into max_query_length // 2 packs
-        with FileStorage.open_zipsafe_ro(file_path, "r", encoding="utf-8") as f:
+        with open(file_path, "r", encoding="utf-8") as f:
             header = f.readline()
             values_mark = f.readline()
             # properly formatted file has a values marker at the beginning
             assert values_mark == "VALUES\n"
 
             insert_sql = []
             if write_disposition == "replace":
```

### Comparing `dlt-0.3.1/dlt/destinations/job_client_impl.py` & `dlt-0.3.1a0/dlt/destinations/job_client_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 class SqlLoadJob(LoadJob):
     """A job executing sql statement, without followup trait"""
 
     def __init__(self, file_path: str, sql_client: SqlClientBase[Any]) -> None:
         super().__init__(FileStorage.get_file_name_from_file_path(file_path))
         # execute immediately if client present
-        with FileStorage.open_zipsafe_ro(file_path, "r", encoding="utf-8") as f:
+        with open(file_path, "r", encoding="utf-8") as f:
             sql = f.read()
         with sql_client.begin_transaction():
             sql_client.execute_sql(sql)
 
     def state(self) -> TLoadJobState:
         # this job is always done
         return "completed"
```

### Comparing `dlt-0.3.1/dlt/destinations/job_impl.py` & `dlt-0.3.1a0/dlt/destinations/job_impl.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/destinations/postgres/__init__.py` & `dlt-0.3.1a0/dlt/destinations/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/destinations/postgres/configuration.py` & `dlt-0.3.1a0/dlt/destinations/postgres/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/destinations/postgres/postgres.py` & `dlt-0.3.1a0/dlt/destinations/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/destinations/postgres/sql_client.py` & `dlt-0.3.1a0/dlt/destinations/postgres/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/destinations/redshift/README.md` & `dlt-0.3.1a0/dlt/destinations/redshift/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/destinations/redshift/__init__.py` & `dlt-0.3.1a0/dlt/destinations/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/destinations/redshift/configuration.py` & `dlt-0.3.1a0/dlt/destinations/redshift/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/destinations/redshift/redshift.py` & `dlt-0.3.1a0/dlt/destinations/redshift/redshift.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/destinations/sql_client.py` & `dlt-0.3.1a0/dlt/destinations/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/destinations/sql_merge_job.py` & `dlt-0.3.1a0/dlt/destinations/sql_merge_job.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/destinations/typing.py` & `dlt-0.3.1a0/dlt/destinations/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/extract/decorators.py` & `dlt-0.3.1a0/dlt/extract/decorators.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/extract/exceptions.py` & `dlt-0.3.1a0/dlt/extract/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/extract/extract.py` & `dlt-0.3.1a0/dlt/extract/extract.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/extract/incremental.py` & `dlt-0.3.1a0/dlt/extract/incremental.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/extract/pipe.py` & `dlt-0.3.1a0/dlt/extract/pipe.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import types
 import asyncio
 import makefun
 from asyncio import Future
 from concurrent.futures import ThreadPoolExecutor
 from copy import copy
 from threading import Thread
-from typing import Any, ContextManager, Optional, Sequence, Union, Callable, Iterable, Iterator, List, NamedTuple, Awaitable, Tuple, Type, TYPE_CHECKING, Literal
+from typing import Any, ContextManager, Optional, Sequence, Union, Callable, Iterable, Iterator, List, NamedTuple, Awaitable, Tuple, Type, TYPE_CHECKING
 
 from dlt.common import sleep
 from dlt.common.configuration import configspec
 from dlt.common.configuration.inject import with_config
 from dlt.common.configuration.specs import BaseConfiguration, ContainerInjectableContext
 from dlt.common.configuration.container import Container
 from dlt.common.exceptions import PipelineException
@@ -61,16 +61,14 @@
     Iterable[TPipedDataItems],
     Iterator[TPipedDataItems],
     Callable[[TDataItems, Optional[Any]], TPipedDataItems],
     Callable[[TDataItems, Optional[Any]], Iterator[TPipedDataItems]],
     Callable[[TDataItems, Optional[Any]], Iterator[ResolvablePipeItem]]
 ]
 
-TPipeNextItemMode = Union[Literal["fifo"], Literal["round_robin"]]
-
 
 class ForkPipe:
     def __init__(self, pipe: "Pipe", step: int = -1, copy_on_fork: bool = False) -> None:
         """A transformer that forks the `pipe` and sends the data items to forks added via `add_pipe` method."""
         self._pipes: List[Tuple["Pipe", int]] = []
         self.copy_on_fork = copy_on_fork
         """If true, the data items going to a forked pipe will be copied"""
@@ -422,70 +420,62 @@
 
     @configspec
     class PipeIteratorConfiguration(BaseConfiguration):
         max_parallel_items: int = 20
         workers: int = 5
         futures_poll_interval: float = 0.01
         copy_on_fork: bool = False
-        next_item_mode: str = "fifo"
 
         __section__ = "extract"
 
-    def __init__(self, max_parallel_items: int, workers: int, futures_poll_interval: float, next_item_mode: TPipeNextItemMode) -> None:
+    def __init__(self, max_parallel_items: int, workers: int, futures_poll_interval: float) -> None:
         self.max_parallel_items = max_parallel_items
         self.workers = workers
         self.futures_poll_interval = futures_poll_interval
 
-        self._round_robin_index: int = -1
-        self._initial_sources_count: int = 0
         self._async_pool: asyncio.AbstractEventLoop = None
         self._async_pool_thread: Thread = None
         self._thread_pool: ThreadPoolExecutor = None
         self._sources: List[SourcePipeItem] = []
         self._futures: List[FuturePipeItem] = []
-        self._next_item_mode = next_item_mode
 
     @classmethod
     @with_config(spec=PipeIteratorConfiguration)
-    def from_pipe(cls, pipe: Pipe, *, max_parallel_items: int = 20, workers: int = 5, futures_poll_interval: float = 0.01, next_item_mode: TPipeNextItemMode = "fifo") -> "PipeIterator":
+    def from_pipe(cls, pipe: Pipe, *, max_parallel_items: int = 20, workers: int = 5, futures_poll_interval: float = 0.01) -> "PipeIterator":
         # join all dependent pipes
         if pipe.parent:
             pipe = pipe.full_pipe()
         # clone pipe to allow multiple iterations on pipe based on iterables/callables
         pipe = pipe._clone()
         # head must be iterator
         pipe.evaluate_gen()
         assert isinstance(pipe.gen, Iterator)
         # create extractor
-        extract = cls(max_parallel_items, workers, futures_poll_interval, next_item_mode)
+        extract = cls(max_parallel_items, workers, futures_poll_interval)
         # add as first source
         extract._sources.append(SourcePipeItem(pipe.gen, 0, pipe, None))
-        cls._initial_sources_count = 1
         return extract
 
     @classmethod
     @with_config(spec=PipeIteratorConfiguration)
     def from_pipes(
         cls,
         pipes: Sequence[Pipe],
         yield_parents: bool = True,
         *,
         max_parallel_items: int = 20,
         workers: int = 5,
         futures_poll_interval: float = 0.01,
-        copy_on_fork: bool = False,
-        next_item_mode: TPipeNextItemMode = "fifo"
+        copy_on_fork: bool = False
     ) -> "PipeIterator":
-
         # print(f"max_parallel_items: {max_parallel_items} workers: {workers}")
-        extract = cls(max_parallel_items, workers, futures_poll_interval, next_item_mode)
+        extract = cls(max_parallel_items, workers, futures_poll_interval)
         # clone all pipes before iterating (recursively) as we will fork them (this add steps) and evaluate gens
         pipes = PipeIterator.clone_pipes(pipes)
 
-
         def _fork_pipeline(pipe: Pipe) -> None:
             if pipe.parent:
                 # fork the parent pipe
                 pipe.evaluate_gen()
                 pipe.parent.fork(pipe, copy_on_fork=copy_on_fork)
                 # make the parent yield by sending a clone of item to itself with position at the end
                 if yield_parents and pipe.parent in pipes:
@@ -496,22 +486,17 @@
                 # head of independent pipe must be iterator
                 pipe.evaluate_gen()
                 assert isinstance(pipe.gen, Iterator)
                 # add every head as source only once
                 if not any(i.pipe == pipe for i in extract._sources):
                     extract._sources.append(SourcePipeItem(pipe.gen, 0, pipe, None))
 
-        # reverse pipes for current mode, as we start processing from the back
-        if next_item_mode == "fifo":
-            pipes.reverse()
-        for pipe in pipes:
+        for pipe in reversed(pipes):
             _fork_pipeline(pipe)
 
-        extract._initial_sources_count = len(extract._sources)
-
         return extract
 
     def __next__(self) -> PipeItem:
         pipe_item: Union[ResolvablePipeItem, SourcePipeItem] = None
         # __next__ should call itself to remove the `while` loop and continue clauses but that may lead to stack overflows: there's no tail recursion opt in python
         # https://stackoverflow.com/questions/13591970/does-python-optimize-tail-recursion (see Y combinator on how it could be emulated)
         while True:
@@ -678,90 +663,46 @@
         item = future.result()
         if isinstance(item, DataItemWithMeta):
             return ResolvablePipeItem(item.data, step, pipe, item.meta)
         else:
             return ResolvablePipeItem(item, step, pipe, meta)
 
     def _get_source_item(self) -> ResolvablePipeItem:
-        if self._next_item_mode == "fifo":
-            return self._get_source_item_current()
-        elif self._next_item_mode == "round_robin":
-            return self._get_source_item_round_robin()
-
-    def _get_source_item_current(self) -> ResolvablePipeItem:
         # no more sources to iterate
         if len(self._sources) == 0:
             return None
-        try:
-            # get items from last added iterator, this makes the overall Pipe as close to FIFO as possible
-            gen, step, pipe, meta = self._sources[-1]
-            # print(f"got {pipe.name} {pipe._pipe_id}")
-            # register current pipe name during the execution of gen
-            set_current_pipe_name(pipe.name)
-            item = next(gen)
-            # full pipe item may be returned, this is used by ForkPipe step
-            # to redirect execution of an item to another pipe
-            if isinstance(item, ResolvablePipeItem):
-                return item
-            else:
-                # keep the item assigned step and pipe when creating resolvable item
-                if isinstance(item, DataItemWithMeta):
-                    return ResolvablePipeItem(item.data, step, pipe, item.meta)
-                else:
-                    return ResolvablePipeItem(item, step, pipe, meta)
-        except StopIteration:
-            # remove empty iterator and try another source
-            self._sources.pop()
-            return self._get_source_item()
-        except (PipelineException, ExtractorException, DltSourceException, PipeException):
-            raise
-        except Exception as ex:
-            raise ResourceExtractionError(pipe.name, gen, str(ex), "generator") from ex
 
-    def _get_source_item_round_robin(self) -> ResolvablePipeItem:
-        # no more sources to iterate
-        sources_count = len(self._sources)
-        if sources_count == 0:
-            return None
-        # if there are currently more sources than added initially, we need to process the new ones first
-        if sources_count > self._initial_sources_count:
-            return self._get_source_item_current()
+        # get items from last added iterator, this makes the overall Pipe as close to FIFO as possible
+        gen, step, pipe, meta = self._sources[-1]
+        # print(f"got {pipe.name} {pipe._pipe_id}")
+        # register current pipe name during the execution of gen
+        set_current_pipe_name(pipe.name)
         try:
-            # get items from last added iterator, this makes the overall Pipe as close to FIFO as possible
-            self._round_robin_index = (self._round_robin_index + 1) % sources_count
-            gen, step, pipe, meta = self._sources[self._round_robin_index]
-            # print(f"got {pipe.name} {pipe._pipe_id}")
-            # register current pipe name during the execution of gen
-            set_current_pipe_name(pipe.name)
             item = next(gen)
             # full pipe item may be returned, this is used by ForkPipe step
             # to redirect execution of an item to another pipe
             if isinstance(item, ResolvablePipeItem):
                 return item
             else:
                 # keep the item assigned step and pipe when creating resolvable item
                 if isinstance(item, DataItemWithMeta):
                     return ResolvablePipeItem(item.data, step, pipe, item.meta)
                 else:
                     return ResolvablePipeItem(item, step, pipe, meta)
         except StopIteration:
             # remove empty iterator and try another source
-            self._sources.pop(self._round_robin_index)
-            # we need to decrease the index to keep the round robin order
-            self._round_robin_index -= 1
-            # since in this case we have popped an initial source, we need to decrease the initial sources count
-            self._initial_sources_count -= 1
+            self._sources.pop()
             return self._get_source_item()
         except (PipelineException, ExtractorException, DltSourceException, PipeException):
             raise
         except Exception as ex:
             raise ResourceExtractionError(pipe.name, gen, str(ex), "generator") from ex
 
     @staticmethod
-    def clone_pipes(pipes: Sequence[Pipe]) -> List[Pipe]:
+    def clone_pipes(pipes: Sequence[Pipe]) -> Sequence[Pipe]:
         """This will clone pipes and fix the parent/dependent references"""
         cloned_pipes = [p._clone() for p in pipes]
         cloned_pairs = {id(p): c for p, c in zip(pipes, cloned_pipes)}
 
         for clone in cloned_pipes:
             while True:
                 if not clone.parent:
```

### Comparing `dlt-0.3.1/dlt/extract/schema.py` & `dlt-0.3.1a0/dlt/extract/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/extract/source.py` & `dlt-0.3.1a0/dlt/extract/source.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/extract/typing.py` & `dlt-0.3.1a0/dlt/extract/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/extract/utils.py` & `dlt-0.3.1a0/dlt/extract/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/helpers/airflow_helper.py` & `dlt-0.3.1a0/dlt/helpers/airflow_helper.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/helpers/dbt/__init__.py` & `dlt-0.3.1a0/dlt/helpers/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/helpers/dbt/configuration.py` & `dlt-0.3.1a0/dlt/helpers/dbt/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/helpers/dbt/dbt_utils.py` & `dlt-0.3.1a0/dlt/helpers/dbt/dbt_utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/helpers/dbt/exceptions.py` & `dlt-0.3.1a0/dlt/helpers/dbt/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/helpers/dbt/profiles.yml` & `dlt-0.3.1a0/dlt/helpers/dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/helpers/dbt/runner.py` & `dlt-0.3.1a0/dlt/helpers/dbt/runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/helpers/pandas_helper.py` & `dlt-0.3.1a0/dlt/helpers/pandas_helper.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/helpers/parquet.py` & `dlt-0.3.1a0/dlt/helpers/parquet.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/helpers/streamlit_helper.py` & `dlt-0.3.1a0/dlt/helpers/streamlit_helper.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/load/configuration.py` & `dlt-0.3.1a0/dlt/load/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/load/exceptions.py` & `dlt-0.3.1a0/dlt/load/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/load/load.py` & `dlt-0.3.1a0/dlt/load/load.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/normalize/configuration.py` & `dlt-0.3.1a0/dlt/normalize/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/normalize/normalize.py` & `dlt-0.3.1a0/dlt/normalize/normalize.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/pipeline/__init__.py` & `dlt-0.3.1a0/dlt/pipeline/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 
     ### Summary
     The `pipeline` functions allows you to pass the destination name to which the data should be loaded, the name of the dataset and several other options that govern loading of the data.
     The created `Pipeline` object lets you load the data from any source with `run` method or to have more granular control over the loading process with `extract`, `normalize` and `load` methods.
 
     Please refer to the following doc pages
     - Write your first pipeline walkthrough: https://dlthub.com/docs/walkthroughs/create-a-pipeline
-    - Pipeline architecture and data loading steps: https://dlthub.com/docs/reference
-    - List of supported destinations: https://dlthub.com/docs/dlt-ecosystem/destinations
+    - Pipeline architecture and data loading steps: https://dlthub.com/docs/architecture
+    - List of supported destinations: https://dlthub.com/docs/destinations/bigquery
 
     ### Args:
         pipeline_name (str, optional): A name of the pipeline that will be used to identify it in monitoring events and to restore its state and data schemas on subsequent runs.
         Defaults to the file name of pipeline script with `dlt_` prefix added.
 
         pipelines_dir (str, optional): A working directory in which pipeline state and temporary files will be stored. Defaults to user home directory: `~/dlt/pipelines/`.
```

### Comparing `dlt-0.3.1/dlt/pipeline/configuration.py` & `dlt-0.3.1a0/dlt/pipeline/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/pipeline/dbt.py` & `dlt-0.3.1a0/dlt/pipeline/dbt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/pipeline/exceptions.py` & `dlt-0.3.1a0/dlt/pipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/pipeline/helpers.py` & `dlt-0.3.1a0/dlt/pipeline/helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/pipeline/pipeline.py` & `dlt-0.3.1a0/dlt/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/pipeline/progress.py` & `dlt-0.3.1a0/dlt/pipeline/progress.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/pipeline/state_sync.py` & `dlt-0.3.1a0/dlt/pipeline/state_sync.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/pipeline/trace.py` & `dlt-0.3.1a0/dlt/pipeline/trace.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,12 +203,12 @@
 def save_trace(trace_path: str, trace: PipelineTrace) -> None:
     with open(os.path.join(trace_path, TRACE_FILE_NAME), mode="bw") as f:
         f.write(pickle.dumps(trace))
 
 
 def load_trace(trace_path: str) -> PipelineTrace:
     try:
-        with open(os.path.join(trace_path, TRACE_FILE_NAME), mode="rb") as f:
+        with open(os.path.join(trace_path, TRACE_FILE_NAME), mode="br") as f:
             return pickle.load(f)  # type: ignore
     except (AttributeError, FileNotFoundError):
         # on incompatible pickling / file not found return no trace
         return None
```

### Comparing `dlt-0.3.1/dlt/pipeline/track.py` & `dlt-0.3.1a0/dlt/pipeline/track.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/reflection/names.py` & `dlt-0.3.1a0/dlt/reflection/names.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/reflection/script_inspector.py` & `dlt-0.3.1a0/dlt/reflection/script_inspector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/reflection/script_visitor.py` & `dlt-0.3.1a0/dlt/reflection/script_visitor.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/sources/helpers/requests/__init__.py` & `dlt-0.3.1a0/dlt/sources/helpers/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/sources/helpers/requests/retry.py` & `dlt-0.3.1a0/dlt/sources/helpers/requests/retry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/sources/helpers/requests/session.py` & `dlt-0.3.1a0/dlt/sources/helpers/requests/session.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/sources/helpers/transform.py` & `dlt-0.3.1a0/dlt/sources/helpers/transform.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/dlt/version.py` & `dlt-0.3.1a0/dlt/version.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1/pyproject.toml` & `dlt-0.3.1a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dlt"
-version = "0.3.1"
+version = "0.3.1a0"
 description = "DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run."
 authors = ["dltHub Inc. <services@dlthub.com>"]
 maintainers = [ "Marcin Rudolf <marcin@dlthub.com>", "Adrian Brudaru <adrian@dlthub.com>", "Ty Dunn <ty@dlthub.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/dlt-hub"
 repository = "https://github.com/dlt-hub/dlt"
```

### Comparing `dlt-0.3.1/setup.py` & `dlt-0.3.1a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,17 +96,17 @@
  's3': ['s3fs>=2023.5.0,<2024.0.0', 'boto3>=1.26']}
 
 entry_points = \
 {'console_scripts': ['dlt = dlt.cli._dlt:_main']}
 
 setup_kwargs = {
     'name': 'dlt',
-    'version': '0.3.1',
+    'version': '0.3.1a0',
     'description': 'DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.',
-    'long_description': '<h1 align="center">\n    <strong>data load tool (dlt) — the open-source Python library for data loading</strong>\n</h1>\n<p align="center">\nBe it a Google Colab notebook, AWS Lambda function, an Airflow DAG, your local laptop,<br/>or a GPT-4 assisted development playground—<strong>dlt</strong> can be dropped in anywhere.\n</p>\n\n<div align="center">\n  <a target="_blank" href="https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g" style="background:none">\n    <img src="https://img.shields.io/badge/slack-join-dlt.svg?labelColor=191937&color=6F6FF7&logo=slack" />\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/v/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/pyversions/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n</div>\n\n## Installation\n\ndlt supports Python 3.8+.\n\n```bash\npip install dlt\n```\n\n## Quick Start\n\nLoad chess game data from chess.com API and save it in DuckDB:\n\n```python\nimport dlt\nfrom chess import chess # a utility function that grabs data from the chess.com API\n\n# create a dlt pipeline that will load chess game data to the DuckDB destination\npipeline = dlt.pipeline(\n    pipeline_name=\'chess_pipeline\',\n    destination=\'duckdb\',\n    dataset_name=\'games_data\'\n)\n\n# use chess.com API to grab data about a few players\ndata = chess([\'magnuscarlsen\', \'rpragchess\'], start_month=\'2022/11\', end_month=\'2022/12\')\n\n# extract, normalize, and load the data\npipeline.run(data)\n```\n\nTry it out in our **[Colab Demo](https://colab.research.google.com/drive/1NfSB1DpwbbHX9_t5vlalBTf13utwpMGx?usp=sharing)**\n\n## Features\n\n- **Automatic Schema:** Data structure inspection and schema creation for the destination.\n- **Data Normalization:** Consistent and verified data before loading.\n- **Seamless Integration:** Colab, AWS Lambda, Airflow, and local environments.\n- **Scalable:** Adapts to growing data needs in production.\n- **Easy Maintenance:** Clear data pipeline structure for updates.\n- **Rapid Exploration:** Quickly explore and gain insights from new data sources.\n- **Versatile Usage:** Suitable for ad-hoc exploration to advanced loading infrastructures.\n- **Start in Seconds with CLI:** Powerful CLI for managing, deploying and inspecting local pipelines.\n- **Incremental Loading:** Load only new or changed data and avoid loading old records again.\n- **Open Source:** Free and Apache 2.0 Licensed.\n\n## Ready to use Sources and Destinations\n\nExplore ready to use sources (e.g. Google Sheets) in the [Verified Sources docs](https://dlthub.com/docs/dlt-ecosystem/verified-sources) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/dlt-ecosystem/destinations).\n\n## Documentation\n\nFor detailed usage and configuration, please refer to the [official documentation](https://dlthub.com/docs).\n\n## Examples\n\nYou can find examples for various use cases in the [examples](docs/examples) folder.\n\n## Get Involved\n\nThe dlt project is quickly growing, and we\'re excited to have you join our community! Here\'s how you can get involved:\n\n- **Connect with the Community**: Join other dlt users and contributors on our [Slack](https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g)\n- **Report issues and suggest features**: Please use the [GitHub Issues](https://github.com/dlt-hub/dlt/issues) to report bugs or suggest new features. Before creating a new issue, make sure to search the tracker for possible duplicates and add a comment if you find one.\n- **Contribute Verified Sources**: Contribute your custom sources to the [dlt-hub/verified-sources](https://github.com/dlt-hub/verified-sources) to help other folks in handling their data tasks.\n- **Contribute code**: Check out our [contributing guidelines](CONTRIBUTING.md) for information on how to make a pull request.\n- **Improve documentation**: Help us enhance the dlt documentation.\n\n## License\n\nDLT is released under the [Apache 2.0 License](LICENSE.txt).\n',
+    'long_description': '<h1 align="center">\n    <strong>data load tool (dlt) — the open-source Python library for data loading</strong>\n</h1>\n<p align="center">\nBe it a Google Colab notebook, AWS Lambda function, an Airflow DAG, your local laptop,<br/>or a GPT-4 assisted development playground—<strong>dlt</strong> can be dropped in anywhere.\n</p>\n\n<div align="center">\n  <a target="_blank" href="https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g" style="background:none">\n    <img src="https://img.shields.io/badge/slack-join-dlt.svg?labelColor=191937&color=6F6FF7&logo=slack" />\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/v/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/pyversions/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n</div>\n\n## Installation\n\ndlt supports Python 3.8+.\n\n```bash\npip install dlt\n```\n\n## Quick Start\n\nLoad chess game data from chess.com API and save it in DuckDB:\n\n```python\nimport dlt\nfrom chess import chess # a utility function that grabs data from the chess.com API\n\n# create a dlt pipeline that will load chess game data to the DuckDB destination\npipeline = dlt.pipeline(\n    pipeline_name=\'chess_pipeline\',\n    destination=\'duckdb\',\n    dataset_name=\'games_data\'\n)\n\n# use chess.com API to grab data about a few players\ndata = chess([\'magnuscarlsen\', \'rpragchess\'], start_month=\'2022/11\', end_month=\'2022/12\')\n\n# extract, normalize, and load the data\npipeline.run(data)\n```\n\nTry it out in our **[Colab Demo](https://colab.research.google.com/drive/1NfSB1DpwbbHX9_t5vlalBTf13utwpMGx?usp=sharing)**\n\n## Features\n\n- **Automatic Schema:** Data structure inspection and schema creation for the destination.\n- **Data Normalization:** Consistent and verified data before loading.\n- **Seamless Integration:** Colab, AWS Lambda, Airflow, and local environments.\n- **Scalable:** Adapts to growing data needs in production.\n- **Easy Maintenance:** Clear data pipeline structure for updates.\n- **Rapid Exploration:** Quickly explore and gain insights from new data sources.\n- **Versatile Usage:** Suitable for ad-hoc exploration to advanced loading infrastructures.\n- **Start in Seconds with CLI:** Powerful CLI for managing, deploying and inspecting local pipelines.\n- **Incremental Loading:** Load only new or changed data and avoid loading old records again.\n- **Open Source:** Free and Apache 2.0 Licensed.\n\n## Ready to use Sources and Destinations\n\nExplore ready to use sources (e.g. Google Sheets) in the [Verified Sources docs](https://dlthub.com/docs/verified-sources/chess) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/destinations/bigquery).\n\n## Documentation\n\nFor detailed usage and configuration, please refer to the [official documentation](https://dlthub.com/docs).\n\n## Examples\n\nYou can find examples for various use cases in the [examples](docs/examples) folder.\n\n## Get Involved\n\nThe dlt project is quickly growing, and we\'re excited to have you join our community! Here\'s how you can get involved:\n\n- **Connect with the Community**: Join other dlt users and contributors on our [Slack](https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g)\n- **Report issues and suggest features**: Please use the [GitHub Issues](https://github.com/dlt-hub/dlt/issues) to report bugs or suggest new features. Before creating a new issue, make sure to search the tracker for possible duplicates and add a comment if you find one.\n- **Contribute Verified Sources**: Contribute your custom sources to the [dlt-hub/verified-sources](https://github.com/dlt-hub/verified-sources) to help other folks in handling their data tasks.\n- **Contribute code**: Check out our [contributing guidelines](CONTRIBUTING.md) for information on how to make a pull request.\n- **Improve documentation**: Help us enhance the dlt documentation.\n\n## License\n\nDLT is released under the [Apache 2.0 License](LICENSE.txt).\n',
     'author': 'dltHub Inc.',
     'author_email': 'services@dlthub.com',
     'maintainer': 'Marcin Rudolf',
     'maintainer_email': 'marcin@dlthub.com',
     'url': 'https://github.com/dlt-hub',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `dlt-0.3.1/PKG-INFO` & `dlt-0.3.1a0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlt
-Version: 0.3.1
+Version: 0.3.1a0
 Summary: DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.
 Home-page: https://github.com/dlt-hub
 License: Apache-2.0
 Keywords: etl
 Author: dltHub Inc.
 Author-email: services@dlthub.com
 Maintainer: Marcin Rudolf
@@ -139,15 +139,15 @@
 - **Versatile Usage:** Suitable for ad-hoc exploration to advanced loading infrastructures.
 - **Start in Seconds with CLI:** Powerful CLI for managing, deploying and inspecting local pipelines.
 - **Incremental Loading:** Load only new or changed data and avoid loading old records again.
 - **Open Source:** Free and Apache 2.0 Licensed.
 
 ## Ready to use Sources and Destinations
 
-Explore ready to use sources (e.g. Google Sheets) in the [Verified Sources docs](https://dlthub.com/docs/dlt-ecosystem/verified-sources) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/dlt-ecosystem/destinations).
+Explore ready to use sources (e.g. Google Sheets) in the [Verified Sources docs](https://dlthub.com/docs/verified-sources/chess) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/destinations/bigquery).
 
 ## Documentation
 
 For detailed usage and configuration, please refer to the [official documentation](https://dlthub.com/docs).
 
 ## Examples
```

