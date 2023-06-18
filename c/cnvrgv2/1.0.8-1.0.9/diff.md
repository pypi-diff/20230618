# Comparing `tmp/cnvrgv2-1.0.8.tar.gz` & `tmp/cnvrgv2-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnvrgv2-1.0.8.tar", last modified: Mon Apr  4 07:40:04 2022, max compression
+gzip compressed data, was "cnvrgv2-1.0.9.tar", last modified: Mon Apr 11 13:20:01 2022, max compression
```

## Comparing `cnvrgv2-1.0.8.tar` & `cnvrgv2-1.0.9.tar`

### file list

```diff
@@ -1,187 +1,200 @@
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.770773 cnvrgv2-1.0.8/
--rw-r--r--   0 leah       (501) staff       (20)       66 2022-03-01 15:06:52.000000 cnvrgv2-1.0.8/MANIFEST.in
--rw-r--r--   0 leah       (501) staff       (20)      269 2022-04-04 07:40:04.770447 cnvrgv2-1.0.8/PKG-INFO
--rw-r--r--   0 leah       (501) staff       (20)     2080 2021-09-07 11:10:42.000000 cnvrgv2-1.0.8/README.md
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.695161 cnvrgv2-1.0.8/cnvrgv2/
--rw-r--r--   0 leah       (501) staff       (20)      322 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)       22 2022-04-04 07:39:40.000000 cnvrgv2-1.0.8/cnvrgv2/_version.py
--rw-r--r--   0 leah       (501) staff       (20)     1508 2021-04-08 09:17:55.000000 cnvrgv2-1.0.8/cnvrgv2/async.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.698687 cnvrgv2-1.0.8/cnvrgv2/cli/
--rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-08 09:17:55.000000 cnvrgv2-1.0.8/cnvrgv2/cli/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)     1985 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/cli/cli.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.699742 cnvrgv2-1.0.8/cnvrgv2/cli/logger/
--rw-r--r--   0 leah       (501) staff       (20)        0 2021-09-07 11:10:42.000000 cnvrgv2-1.0.8/cnvrgv2/cli/logger/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)     2190 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/cli/logger/logger.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.700643 cnvrgv2-1.0.8/cnvrgv2/cli/modules/
--rw-r--r--   0 leah       (501) staff       (20)        0 2021-09-07 11:10:42.000000 cnvrgv2-1.0.8/cnvrgv2/cli/modules/__init__.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.701841 cnvrgv2-1.0.8/cnvrgv2/cli/modules/config/
--rw-r--r--   0 leah       (501) staff       (20)       27 2021-09-07 11:10:42.000000 cnvrgv2-1.0.8/cnvrgv2/cli/modules/config/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)     1362 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/cli/modules/config/config.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.703064 cnvrgv2-1.0.8/cnvrgv2/cli/modules/dataset/
--rw-r--r--   0 leah       (501) staff       (20)        0 2021-09-07 11:10:42.000000 cnvrgv2-1.0.8/cnvrgv2/cli/modules/dataset/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)     3124 2022-04-04 07:39:09.000000 cnvrgv2-1.0.8/cnvrgv2/cli/modules/dataset/dataset.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.704855 cnvrgv2-1.0.8/cnvrgv2/cli/modules/project/
--rw-r--r--   0 leah       (501) staff       (20)        0 2021-09-07 11:10:42.000000 cnvrgv2-1.0.8/cnvrgv2/cli/modules/project/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)     2536 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/cli/modules/project/experiment.py
--rw-r--r--   0 leah       (501) staff       (20)     4782 2022-04-04 07:39:09.000000 cnvrgv2-1.0.8/cnvrgv2/cli/modules/project/project.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.705504 cnvrgv2-1.0.8/cnvrgv2/cli/modules/ssh/
--rw-r--r--   0 leah       (501) staff       (20)        0 2021-09-07 11:10:42.000000 cnvrgv2-1.0.8/cnvrgv2/cli/modules/ssh/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)     2099 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/cli/modules/ssh/ssh.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.706673 cnvrgv2-1.0.8/cnvrgv2/cli/modules/users/
--rw-r--r--   0 leah       (501) staff       (20)        0 2021-09-07 11:10:42.000000 cnvrgv2-1.0.8/cnvrgv2/cli/modules/users/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)     2769 2021-12-13 12:57:10.000000 cnvrgv2-1.0.8/cnvrgv2/cli/modules/users/users.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.709546 cnvrgv2-1.0.8/cnvrgv2/cli/utils/
--rw-r--r--   0 leah       (501) staff       (20)        0 2021-09-07 11:10:42.000000 cnvrgv2-1.0.8/cnvrgv2/cli/utils/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)     1979 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/cli/utils/decorators.py
--rw-r--r--   0 leah       (501) staff       (20)     6083 2022-04-04 07:39:09.000000 cnvrgv2-1.0.8/cnvrgv2/cli/utils/messages.py
--rw-r--r--   0 leah       (501) staff       (20)     1283 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/cli/utils/progress_bar_utils.py
--rw-r--r--   0 leah       (501) staff       (20)      309 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/cli/utils/validators.py
--rw-r--r--   0 leah       (501) staff       (20)     4945 2022-01-20 13:24:21.000000 cnvrgv2-1.0.8/cnvrgv2/cnvrg.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.712640 cnvrgv2-1.0.8/cnvrgv2/config/
--rw-r--r--   0 leah       (501) staff       (20)      100 2021-09-07 11:10:42.000000 cnvrgv2-1.0.8/cnvrgv2/config/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)    10846 2022-04-04 07:39:09.000000 cnvrgv2-1.0.8/cnvrgv2/config/config.py
--rw-r--r--   0 leah       (501) staff       (20)     6593 2022-04-04 07:39:09.000000 cnvrgv2-1.0.8/cnvrgv2/config/error_messages.py
--rw-r--r--   0 leah       (501) staff       (20)     4465 2022-04-04 07:39:09.000000 cnvrgv2-1.0.8/cnvrgv2/config/routes.py
--rw-r--r--   0 leah       (501) staff       (20)    11083 2021-12-13 12:57:10.000000 cnvrgv2-1.0.8/cnvrgv2/context.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.719155 cnvrgv2-1.0.8/cnvrgv2/data/
--rw-r--r--   0 leah       (501) staff       (20)      396 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/data/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)     3549 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/data/artifacts_downloader.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.720658 cnvrgv2-1.0.8/cnvrgv2/data/clients/
--rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-08 09:17:55.000000 cnvrgv2-1.0.8/cnvrgv2/data/clients/__init__.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.721551 cnvrgv2-1.0.8/cnvrgv2/data/clients/azure/
--rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-08 09:17:55.000000 cnvrgv2-1.0.8/cnvrgv2/data/clients/azure/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)     3259 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/data/clients/azure/client.py
--rw-r--r--   0 leah       (501) staff       (20)     2024 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/data/clients/base_storage_client.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.722636 cnvrgv2-1.0.8/cnvrgv2/data/clients/gcp/
--rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-08 09:17:55.000000 cnvrgv2-1.0.8/cnvrgv2/data/clients/gcp/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)     3444 2022-03-01 15:06:52.000000 cnvrgv2-1.0.8/cnvrgv2/data/clients/gcp/client.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.723522 cnvrgv2-1.0.8/cnvrgv2/data/clients/minio/
--rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-08 09:17:55.000000 cnvrgv2-1.0.8/cnvrgv2/data/clients/minio/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)     1979 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/data/clients/minio/client.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.724360 cnvrgv2-1.0.8/cnvrgv2/data/clients/s3/
--rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-08 09:17:55.000000 cnvrgv2-1.0.8/cnvrgv2/data/clients/s3/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)     1988 2021-11-03 14:03:29.000000 cnvrgv2-1.0.8/cnvrgv2/data/clients/s3/client.py
--rw-r--r--   0 leah       (501) staff       (20)     1765 2021-11-10 12:25:57.000000 cnvrgv2-1.0.8/cnvrgv2/data/clients/storage_client_factory.py
--rw-r--r--   0 leah       (501) staff       (20)     7486 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/data/data_loader.py
--rw-r--r--   0 leah       (501) staff       (20)     2949 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/data/file_compare.py
--rw-r--r--   0 leah       (501) staff       (20)     3000 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/data/file_downloader.py
--rw-r--r--   0 leah       (501) staff       (20)     2939 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/data/file_uploader.py
--rw-r--r--   0 leah       (501) staff       (20)     3598 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/data/local_file_deleter.py
--rw-r--r--   0 leah       (501) staff       (20)     9063 2022-03-01 15:06:52.000000 cnvrgv2-1.0.8/cnvrgv2/data/local_files_handler.py
--rw-r--r--   0 leah       (501) staff       (20)     7592 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/data/remote_file_deleter.py
--rw-r--r--   0 leah       (501) staff       (20)     7767 2022-04-04 07:39:09.000000 cnvrgv2-1.0.8/cnvrgv2/data/remote_files_handler.py
--rw-r--r--   0 leah       (501) staff       (20)     1610 2021-09-07 11:10:42.000000 cnvrgv2-1.0.8/cnvrgv2/errors.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.729248 cnvrgv2-1.0.8/cnvrgv2/modules/
--rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-08 09:17:55.000000 cnvrgv2-1.0.8/cnvrgv2/modules/__init__.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.731787 cnvrgv2-1.0.8/cnvrgv2/modules/base/
--rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-08 09:17:55.000000 cnvrgv2-1.0.8/cnvrgv2/modules/base/__init__.py
--rwxr-xr-x   0 leah       (501) staff       (20)    22452 2022-04-04 07:39:09.000000 cnvrgv2-1.0.8/cnvrgv2/modules/base/data_owner.py
--rw-r--r--   0 leah       (501) staff       (20)     2848 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/base/dynamic_attributes.py
--rw-r--r--   0 leah       (501) staff       (20)     6843 2021-12-13 12:57:10.000000 cnvrgv2-1.0.8/cnvrgv2/modules/base/workflow_instance_base.py
--rw-r--r--   0 leah       (501) staff       (20)     4610 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/base/workflows_base.py
--rw-r--r--   0 leah       (501) staff       (20)     2554 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/commit.py
--rw-r--r--   0 leah       (501) staff       (20)     3292 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/dataset.py
--rw-r--r--   0 leah       (501) staff       (20)     3497 2021-11-03 14:03:29.000000 cnvrgv2-1.0.8/cnvrgv2/modules/datasets_client.py
--rw-r--r--   0 leah       (501) staff       (20)      479 2021-11-03 14:03:29.000000 cnvrgv2-1.0.8/cnvrgv2/modules/file.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.734205 cnvrgv2-1.0.8/cnvrgv2/modules/flows/
--rw-r--r--   0 leah       (501) staff       (20)        0 2021-09-07 11:10:42.000000 cnvrgv2-1.0.8/cnvrgv2/modules/flows/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)     5590 2021-12-13 12:57:10.000000 cnvrgv2-1.0.8/cnvrgv2/modules/flows/flow.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.735921 cnvrgv2-1.0.8/cnvrgv2/modules/flows/flow_version/
--rw-r--r--   0 leah       (501) staff       (20)        0 2021-09-07 11:10:42.000000 cnvrgv2-1.0.8/cnvrgv2/modules/flows/flow_version/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)     2422 2021-11-03 14:03:29.000000 cnvrgv2-1.0.8/cnvrgv2/modules/flows/flow_version/flow_version.py
--rw-r--r--   0 leah       (501) staff       (20)     1449 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/flows/flow_version/flow_versions_client.py
--rw-r--r--   0 leah       (501) staff       (20)     3462 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/flows/flows_client.py
--rw-r--r--   0 leah       (501) staff       (20)      379 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/folder.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.737778 cnvrgv2-1.0.8/cnvrgv2/modules/images/
--rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-11 20:18:38.000000 cnvrgv2-1.0.8/cnvrgv2/modules/images/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)      826 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/images/image.py
--rw-r--r--   0 leah       (501) staff       (20)     2011 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/images/images_client.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.739780 cnvrgv2-1.0.8/cnvrgv2/modules/organization/
--rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-08 09:17:55.000000 cnvrgv2-1.0.8/cnvrgv2/modules/organization/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)     2003 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/organization/organization_settings.py
--rw-r--r--   0 leah       (501) staff       (20)     1491 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/organization/organizations_client.py
--rw-r--r--   0 leah       (501) staff       (20)     2454 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/project.py
--rw-r--r--   0 leah       (501) staff       (20)     4196 2022-04-04 07:39:09.000000 cnvrgv2-1.0.8/cnvrgv2/modules/project_settings.py
--rw-r--r--   0 leah       (501) staff       (20)     2821 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/projects_client.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.741252 cnvrgv2-1.0.8/cnvrgv2/modules/queries/
--rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-11 20:18:38.000000 cnvrgv2-1.0.8/cnvrgv2/modules/queries/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)     2451 2021-11-03 14:03:29.000000 cnvrgv2-1.0.8/cnvrgv2/modules/queries/queries_client.py
--rw-r--r--   0 leah       (501) staff       (20)     1053 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/queries/query.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.745716 cnvrgv2-1.0.8/cnvrgv2/modules/resources/
--rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-08 09:17:55.000000 cnvrgv2-1.0.8/cnvrgv2/modules/resources/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)     3067 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/resources/_machine.py
--rw-r--r--   0 leah       (501) staff       (20)     4009 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/resources/_machines_client.py
--rw-r--r--   0 leah       (501) staff       (20)     1625 2021-11-03 14:03:29.000000 cnvrgv2-1.0.8/cnvrgv2/modules/resources/_spark_driver.py
--rw-r--r--   0 leah       (501) staff       (20)     1475 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/resources/_spark_drivers_client.py
--rw-r--r--   0 leah       (501) staff       (20)     1565 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/resources/cluster.py
--rw-r--r--   0 leah       (501) staff       (20)     1424 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/resources/clusters_client.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.748015 cnvrgv2-1.0.8/cnvrgv2/modules/resources/templates/
--rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-08 09:17:55.000000 cnvrgv2-1.0.8/cnvrgv2/modules/resources/templates/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)     4431 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/resources/templates/kube_template.py
--rw-r--r--   0 leah       (501) staff       (20)     4998 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/resources/templates/kube_templates_client.py
--rw-r--r--   0 leah       (501) staff       (20)     3465 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/resources/templates/spark_template.py
--rw-r--r--   0 leah       (501) staff       (20)     3868 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/resources/templates/spark_templates_client.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.749182 cnvrgv2-1.0.8/cnvrgv2/modules/ssh/
--rw-r--r--   0 leah       (501) staff       (20)        0 2021-09-07 11:10:42.000000 cnvrgv2-1.0.8/cnvrgv2/modules/ssh/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)     1394 2021-11-03 14:03:29.000000 cnvrgv2-1.0.8/cnvrgv2/modules/ssh/ssh.py
--rw-r--r--   0 leah       (501) staff       (20)      273 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/ssh/ssh_client.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.750481 cnvrgv2-1.0.8/cnvrgv2/modules/users/
--rw-r--r--   0 leah       (501) staff       (20)       45 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/users/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)     2782 2021-11-03 14:03:29.000000 cnvrgv2-1.0.8/cnvrgv2/modules/users/user.py
--rw-r--r--   0 leah       (501) staff       (20)     3152 2021-11-03 14:03:29.000000 cnvrgv2-1.0.8/cnvrgv2/modules/users/users_client.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.751598 cnvrgv2-1.0.8/cnvrgv2/modules/volumes/
--rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-11 20:18:38.000000 cnvrgv2-1.0.8/cnvrgv2/modules/volumes/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)     1090 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/volumes/volume.py
--rw-r--r--   0 leah       (501) staff       (20)     2766 2021-11-03 14:03:29.000000 cnvrgv2-1.0.8/cnvrgv2/modules/volumes/volumes_client.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.752618 cnvrgv2-1.0.8/cnvrgv2/modules/workflows/
--rw-r--r--   0 leah       (501) staff       (20)      646 2021-11-03 14:03:29.000000 cnvrgv2-1.0.8/cnvrgv2/modules/workflows/__init__.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.754732 cnvrgv2-1.0.8/cnvrgv2/modules/workflows/endpoint/
--rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-11 20:18:38.000000 cnvrgv2-1.0.8/cnvrgv2/modules/workflows/endpoint/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)    14240 2022-03-01 15:06:52.000000 cnvrgv2-1.0.8/cnvrgv2/modules/workflows/endpoint/endpoint.py
--rw-r--r--   0 leah       (501) staff       (20)      669 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/workflows/endpoint/endpoint_rule.py
--rw-r--r--   0 leah       (501) staff       (20)     2861 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/workflows/endpoint/endpoints_client.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.756313 cnvrgv2-1.0.8/cnvrgv2/modules/workflows/experiment/
--rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-11 20:18:38.000000 cnvrgv2-1.0.8/cnvrgv2/modules/workflows/experiment/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)    12782 2022-03-01 15:06:52.000000 cnvrgv2-1.0.8/cnvrgv2/modules/workflows/experiment/experiment.py
--rw-r--r--   0 leah       (501) staff       (20)     9291 2022-01-20 13:24:21.000000 cnvrgv2-1.0.8/cnvrgv2/modules/workflows/experiment/experiments_client.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.757968 cnvrgv2-1.0.8/cnvrgv2/modules/workflows/webapp/
--rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-11 20:18:38.000000 cnvrgv2-1.0.8/cnvrgv2/modules/workflows/webapp/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)     1720 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/workflows/webapp/webapp.py
--rw-r--r--   0 leah       (501) staff       (20)     2130 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/workflows/webapp/webapps_client.py
--rw-r--r--   0 leah       (501) staff       (20)     1601 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/workflows/workflow_utils.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.759913 cnvrgv2-1.0.8/cnvrgv2/modules/workflows/workspace/
--rw-r--r--   0 leah       (501) staff       (20)       48 2021-11-03 14:03:29.000000 cnvrgv2-1.0.8/cnvrgv2/modules/workflows/workspace/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)     4812 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/modules/workflows/workspace/workspace.py
--rw-r--r--   0 leah       (501) staff       (20)     2315 2021-11-03 14:03:29.000000 cnvrgv2-1.0.8/cnvrgv2/modules/workflows/workspace/workspaces_client.py
--rw-r--r--   0 leah       (501) staff       (20)     6369 2021-12-13 12:57:10.000000 cnvrgv2-1.0.8/cnvrgv2/proxy.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.768164 cnvrgv2-1.0.8/cnvrgv2/utils/
--rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-08 09:17:55.000000 cnvrgv2-1.0.8/cnvrgv2/utils/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)     1850 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/utils/api_list_generator.py
--rw-r--r--   0 leah       (501) staff       (20)     7330 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/utils/chart_utils.py
--rw-r--r--   0 leah       (501) staff       (20)     1217 2021-09-07 11:10:42.000000 cnvrgv2-1.0.8/cnvrgv2/utils/converters.py
--rw-r--r--   0 leah       (501) staff       (20)     2775 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/utils/cron.py
--rw-r--r--   0 leah       (501) staff       (20)      177 2021-04-11 20:18:38.000000 cnvrgv2-1.0.8/cnvrgv2/utils/env_helper.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.769067 cnvrgv2-1.0.8/cnvrgv2/utils/files/
--rw-r--r--   0 leah       (501) staff       (20)      186 2022-03-01 15:06:52.000000 cnvrgv2-1.0.8/cnvrgv2/utils/files/.cnvrgignore
--rw-r--r--   0 leah       (501) staff       (20)        0 2022-03-01 15:06:52.000000 cnvrgv2-1.0.8/cnvrgv2/utils/files/__init__.py
--rw-r--r--   0 leah       (501) staff       (20)      738 2021-09-07 11:10:42.000000 cnvrgv2-1.0.8/cnvrgv2/utils/filter_utils.py
--rw-r--r--   0 leah       (501) staff       (20)     1533 2021-04-11 20:18:38.000000 cnvrgv2-1.0.8/cnvrgv2/utils/json_api_format.py
--rw-r--r--   0 leah       (501) staff       (20)     1888 2021-04-11 20:18:38.000000 cnvrgv2-1.0.8/cnvrgv2/utils/log_utils.py
--rw-r--r--   0 leah       (501) staff       (20)     1043 2021-11-03 14:03:28.000000 cnvrgv2-1.0.8/cnvrgv2/utils/retry.py
--rw-r--r--   0 leah       (501) staff       (20)     7044 2022-03-06 10:51:53.000000 cnvrgv2-1.0.8/cnvrgv2/utils/storage_utils.py
--rw-r--r--   0 leah       (501) staff       (20)      573 2021-04-08 09:17:55.000000 cnvrgv2-1.0.8/cnvrgv2/utils/suppress_exceptions.py
--rw-r--r--   0 leah       (501) staff       (20)     1251 2021-09-07 11:10:42.000000 cnvrgv2-1.0.8/cnvrgv2/utils/url_utils.py
--rw-r--r--   0 leah       (501) staff       (20)     3918 2022-04-04 07:39:09.000000 cnvrgv2-1.0.8/cnvrgv2/utils/validators.py
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.697950 cnvrgv2-1.0.8/cnvrgv2.egg-info/
--rw-r--r--   0 leah       (501) staff       (20)      269 2022-04-04 07:40:04.000000 cnvrgv2-1.0.8/cnvrgv2.egg-info/PKG-INFO
--rw-r--r--   0 leah       (501) staff       (20)     5158 2022-04-04 07:40:04.000000 cnvrgv2-1.0.8/cnvrgv2.egg-info/SOURCES.txt
--rw-r--r--   0 leah       (501) staff       (20)        1 2022-04-04 07:40:04.000000 cnvrgv2-1.0.8/cnvrgv2.egg-info/dependency_links.txt
--rw-r--r--   0 leah       (501) staff       (20)       80 2022-04-04 07:40:04.000000 cnvrgv2-1.0.8/cnvrgv2.egg-info/entry_points.txt
--rw-r--r--   0 leah       (501) staff       (20)      741 2022-04-04 07:40:04.000000 cnvrgv2-1.0.8/cnvrgv2.egg-info/requires.txt
--rw-r--r--   0 leah       (501) staff       (20)       17 2022-04-04 07:40:04.000000 cnvrgv2-1.0.8/cnvrgv2.egg-info/top_level.txt
-drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-04 07:40:04.769557 cnvrgv2-1.0.8/examples/
--rw-r--r--   0 leah       (501) staff       (20)        0 2022-01-20 13:24:21.000000 cnvrgv2-1.0.8/examples/__init__.py
--rwxr-xr-x   0 leah       (501) staff       (20)    10630 2022-03-01 15:06:52.000000 cnvrgv2-1.0.8/examples/create_load_cluster.py
--rw-r--r--   0 leah       (501) staff       (20)      469 2022-03-06 10:51:53.000000 cnvrgv2-1.0.8/requirements.txt
--rw-r--r--   0 leah       (501) staff       (20)       38 2022-04-04 07:40:04.770866 cnvrgv2-1.0.8/setup.cfg
--rw-r--r--   0 leah       (501) staff       (20)     1219 2022-03-06 10:51:53.000000 cnvrgv2-1.0.8/setup.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.994216 cnvrgv2-1.0.9/
+-rw-r--r--   0 leah       (501) staff       (20)       66 2022-03-01 15:06:52.000000 cnvrgv2-1.0.9/MANIFEST.in
+-rw-r--r--   0 leah       (501) staff       (20)      269 2022-04-11 13:20:01.993806 cnvrgv2-1.0.9/PKG-INFO
+-rw-r--r--   0 leah       (501) staff       (20)     2080 2021-09-07 11:10:42.000000 cnvrgv2-1.0.9/README.md
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.931378 cnvrgv2-1.0.9/cnvrgv2/
+-rw-r--r--   0 leah       (501) staff       (20)      322 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)       22 2022-04-11 13:19:33.000000 cnvrgv2-1.0.9/cnvrgv2/_version.py
+-rw-r--r--   0 leah       (501) staff       (20)     1508 2021-04-08 09:17:55.000000 cnvrgv2-1.0.9/cnvrgv2/async.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.934822 cnvrgv2-1.0.9/cnvrgv2/cli/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-08 09:17:55.000000 cnvrgv2-1.0.9/cnvrgv2/cli/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)     2088 2022-04-11 13:19:18.000000 cnvrgv2-1.0.9/cnvrgv2/cli/cli.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.935501 cnvrgv2-1.0.9/cnvrgv2/cli/logger/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2021-09-07 11:10:42.000000 cnvrgv2-1.0.9/cnvrgv2/cli/logger/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)     2190 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/cli/logger/logger.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.935954 cnvrgv2-1.0.9/cnvrgv2/cli/modules/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2021-09-07 11:10:42.000000 cnvrgv2-1.0.9/cnvrgv2/cli/modules/__init__.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.936618 cnvrgv2-1.0.9/cnvrgv2/cli/modules/config/
+-rw-r--r--   0 leah       (501) staff       (20)       27 2021-09-07 11:10:42.000000 cnvrgv2-1.0.9/cnvrgv2/cli/modules/config/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)     1362 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/cli/modules/config/config.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.937621 cnvrgv2-1.0.9/cnvrgv2/cli/modules/dataset/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2021-09-07 11:10:42.000000 cnvrgv2-1.0.9/cnvrgv2/cli/modules/dataset/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)     3124 2022-04-04 07:39:09.000000 cnvrgv2-1.0.9/cnvrgv2/cli/modules/dataset/dataset.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.938372 cnvrgv2-1.0.9/cnvrgv2/cli/modules/libraries/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2022-04-11 13:19:18.000000 cnvrgv2-1.0.9/cnvrgv2/cli/modules/libraries/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)     1021 2022-04-11 13:19:18.000000 cnvrgv2-1.0.9/cnvrgv2/cli/modules/libraries/library.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.939577 cnvrgv2-1.0.9/cnvrgv2/cli/modules/project/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2021-09-07 11:10:42.000000 cnvrgv2-1.0.9/cnvrgv2/cli/modules/project/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)     2536 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/cli/modules/project/experiment.py
+-rw-r--r--   0 leah       (501) staff       (20)     4782 2022-04-04 07:39:09.000000 cnvrgv2-1.0.9/cnvrgv2/cli/modules/project/project.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.940287 cnvrgv2-1.0.9/cnvrgv2/cli/modules/ssh/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2021-09-07 11:10:42.000000 cnvrgv2-1.0.9/cnvrgv2/cli/modules/ssh/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)     2099 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/cli/modules/ssh/ssh.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.941207 cnvrgv2-1.0.9/cnvrgv2/cli/modules/users/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2021-09-07 11:10:42.000000 cnvrgv2-1.0.9/cnvrgv2/cli/modules/users/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)     2769 2021-12-13 12:57:10.000000 cnvrgv2-1.0.9/cnvrgv2/cli/modules/users/users.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.943085 cnvrgv2-1.0.9/cnvrgv2/cli/utils/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2021-09-07 11:10:42.000000 cnvrgv2-1.0.9/cnvrgv2/cli/utils/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)     1979 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/cli/utils/decorators.py
+-rw-r--r--   0 leah       (501) staff       (20)     6434 2022-04-11 13:19:18.000000 cnvrgv2-1.0.9/cnvrgv2/cli/utils/messages.py
+-rw-r--r--   0 leah       (501) staff       (20)     1283 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/cli/utils/progress_bar_utils.py
+-rw-r--r--   0 leah       (501) staff       (20)      309 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/cli/utils/validators.py
+-rw-r--r--   0 leah       (501) staff       (20)     5115 2022-04-11 13:19:18.000000 cnvrgv2-1.0.9/cnvrgv2/cnvrg.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.944790 cnvrgv2-1.0.9/cnvrgv2/config/
+-rw-r--r--   0 leah       (501) staff       (20)      100 2021-09-07 11:10:42.000000 cnvrgv2-1.0.9/cnvrgv2/config/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)    11340 2022-04-11 13:19:18.000000 cnvrgv2-1.0.9/cnvrgv2/config/config.py
+-rw-r--r--   0 leah       (501) staff       (20)     6688 2022-04-11 13:19:18.000000 cnvrgv2-1.0.9/cnvrgv2/config/error_messages.py
+-rw-r--r--   0 leah       (501) staff       (20)     4749 2022-04-11 13:19:18.000000 cnvrgv2-1.0.9/cnvrgv2/config/routes.py
+-rw-r--r--   0 leah       (501) staff       (20)    11488 2022-04-11 13:19:18.000000 cnvrgv2-1.0.9/cnvrgv2/context.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.948716 cnvrgv2-1.0.9/cnvrgv2/data/
+-rw-r--r--   0 leah       (501) staff       (20)      396 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/data/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)     3549 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/data/artifacts_downloader.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.949869 cnvrgv2-1.0.9/cnvrgv2/data/clients/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-08 09:17:55.000000 cnvrgv2-1.0.9/cnvrgv2/data/clients/__init__.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.950465 cnvrgv2-1.0.9/cnvrgv2/data/clients/azure/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-08 09:17:55.000000 cnvrgv2-1.0.9/cnvrgv2/data/clients/azure/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)     3259 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/data/clients/azure/client.py
+-rw-r--r--   0 leah       (501) staff       (20)     2024 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/data/clients/base_storage_client.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.951148 cnvrgv2-1.0.9/cnvrgv2/data/clients/gcp/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-08 09:17:55.000000 cnvrgv2-1.0.9/cnvrgv2/data/clients/gcp/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)     3444 2022-03-01 15:06:52.000000 cnvrgv2-1.0.9/cnvrgv2/data/clients/gcp/client.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.951753 cnvrgv2-1.0.9/cnvrgv2/data/clients/minio/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-08 09:17:55.000000 cnvrgv2-1.0.9/cnvrgv2/data/clients/minio/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)     1979 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/data/clients/minio/client.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.952406 cnvrgv2-1.0.9/cnvrgv2/data/clients/s3/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-08 09:17:55.000000 cnvrgv2-1.0.9/cnvrgv2/data/clients/s3/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)     1988 2021-11-03 14:03:29.000000 cnvrgv2-1.0.9/cnvrgv2/data/clients/s3/client.py
+-rw-r--r--   0 leah       (501) staff       (20)     1765 2021-11-10 12:25:57.000000 cnvrgv2-1.0.9/cnvrgv2/data/clients/storage_client_factory.py
+-rw-r--r--   0 leah       (501) staff       (20)     7486 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/data/data_loader.py
+-rw-r--r--   0 leah       (501) staff       (20)     2949 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/data/file_compare.py
+-rw-r--r--   0 leah       (501) staff       (20)     3000 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/data/file_downloader.py
+-rw-r--r--   0 leah       (501) staff       (20)     2939 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/data/file_uploader.py
+-rw-r--r--   0 leah       (501) staff       (20)     3598 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/data/local_file_deleter.py
+-rw-r--r--   0 leah       (501) staff       (20)     9063 2022-03-01 15:06:52.000000 cnvrgv2-1.0.9/cnvrgv2/data/local_files_handler.py
+-rw-r--r--   0 leah       (501) staff       (20)     7592 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/data/remote_file_deleter.py
+-rw-r--r--   0 leah       (501) staff       (20)     7767 2022-04-04 07:39:09.000000 cnvrgv2-1.0.9/cnvrgv2/data/remote_files_handler.py
+-rw-r--r--   0 leah       (501) staff       (20)     1610 2021-09-07 11:10:42.000000 cnvrgv2-1.0.9/cnvrgv2/errors.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.955495 cnvrgv2-1.0.9/cnvrgv2/modules/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-08 09:17:55.000000 cnvrgv2-1.0.9/cnvrgv2/modules/__init__.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.957917 cnvrgv2-1.0.9/cnvrgv2/modules/base/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-08 09:17:55.000000 cnvrgv2-1.0.9/cnvrgv2/modules/base/__init__.py
+-rwxr-xr-x   0 leah       (501) staff       (20)    22452 2022-04-04 07:39:09.000000 cnvrgv2-1.0.9/cnvrgv2/modules/base/data_owner.py
+-rw-r--r--   0 leah       (501) staff       (20)     2848 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/base/dynamic_attributes.py
+-rw-r--r--   0 leah       (501) staff       (20)     6843 2021-12-13 12:57:10.000000 cnvrgv2-1.0.9/cnvrgv2/modules/base/workflow_instance_base.py
+-rw-r--r--   0 leah       (501) staff       (20)     4610 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/base/workflows_base.py
+-rw-r--r--   0 leah       (501) staff       (20)     2554 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/commit.py
+-rw-r--r--   0 leah       (501) staff       (20)     3292 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/dataset.py
+-rw-r--r--   0 leah       (501) staff       (20)     3497 2021-11-03 14:03:29.000000 cnvrgv2-1.0.9/cnvrgv2/modules/datasets_client.py
+-rw-r--r--   0 leah       (501) staff       (20)      479 2021-11-03 14:03:29.000000 cnvrgv2-1.0.9/cnvrgv2/modules/file.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.959155 cnvrgv2-1.0.9/cnvrgv2/modules/flows/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2021-09-07 11:10:42.000000 cnvrgv2-1.0.9/cnvrgv2/modules/flows/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)     5590 2021-12-13 12:57:10.000000 cnvrgv2-1.0.9/cnvrgv2/modules/flows/flow.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.960708 cnvrgv2-1.0.9/cnvrgv2/modules/flows/flow_version/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2021-09-07 11:10:42.000000 cnvrgv2-1.0.9/cnvrgv2/modules/flows/flow_version/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)     2422 2021-11-03 14:03:29.000000 cnvrgv2-1.0.9/cnvrgv2/modules/flows/flow_version/flow_version.py
+-rw-r--r--   0 leah       (501) staff       (20)     1449 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/flows/flow_version/flow_versions_client.py
+-rw-r--r--   0 leah       (501) staff       (20)     3462 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/flows/flows_client.py
+-rw-r--r--   0 leah       (501) staff       (20)      379 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/folder.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.961954 cnvrgv2-1.0.9/cnvrgv2/modules/images/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-11 20:18:38.000000 cnvrgv2-1.0.9/cnvrgv2/modules/images/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)      826 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/images/image.py
+-rw-r--r--   0 leah       (501) staff       (20)     2011 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/images/images_client.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.962476 cnvrgv2-1.0.9/cnvrgv2/modules/libhub/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2022-04-11 13:19:18.000000 cnvrgv2-1.0.9/cnvrgv2/modules/libhub/__init__.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.964584 cnvrgv2-1.0.9/cnvrgv2/modules/libhub/libraries/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2022-04-11 13:19:18.000000 cnvrgv2-1.0.9/cnvrgv2/modules/libhub/libraries/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)     1671 2022-04-11 13:19:18.000000 cnvrgv2-1.0.9/cnvrgv2/modules/libhub/libraries/libraries_client.py
+-rw-r--r--   0 leah       (501) staff       (20)     1253 2022-04-11 13:19:18.000000 cnvrgv2-1.0.9/cnvrgv2/modules/libhub/libraries/library.py
+-rw-r--r--   0 leah       (501) staff       (20)     3242 2022-04-11 13:19:18.000000 cnvrgv2-1.0.9/cnvrgv2/modules/libhub/libraries/library_version.py
+-rw-r--r--   0 leah       (501) staff       (20)     1491 2022-04-11 13:19:18.000000 cnvrgv2-1.0.9/cnvrgv2/modules/libhub/libraries/library_versions_client.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.966562 cnvrgv2-1.0.9/cnvrgv2/modules/organization/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-08 09:17:55.000000 cnvrgv2-1.0.9/cnvrgv2/modules/organization/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)     2003 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/organization/organization_settings.py
+-rw-r--r--   0 leah       (501) staff       (20)     1491 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/organization/organizations_client.py
+-rw-r--r--   0 leah       (501) staff       (20)     2454 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/project.py
+-rw-r--r--   0 leah       (501) staff       (20)     4196 2022-04-04 07:39:09.000000 cnvrgv2-1.0.9/cnvrgv2/modules/project_settings.py
+-rw-r--r--   0 leah       (501) staff       (20)     2821 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/projects_client.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.968426 cnvrgv2-1.0.9/cnvrgv2/modules/queries/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-11 20:18:38.000000 cnvrgv2-1.0.9/cnvrgv2/modules/queries/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)     2451 2021-11-03 14:03:29.000000 cnvrgv2-1.0.9/cnvrgv2/modules/queries/queries_client.py
+-rw-r--r--   0 leah       (501) staff       (20)     1053 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/queries/query.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.972364 cnvrgv2-1.0.9/cnvrgv2/modules/resources/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-08 09:17:55.000000 cnvrgv2-1.0.9/cnvrgv2/modules/resources/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)     3067 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/resources/_machine.py
+-rw-r--r--   0 leah       (501) staff       (20)     4009 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/resources/_machines_client.py
+-rw-r--r--   0 leah       (501) staff       (20)     1625 2021-11-03 14:03:29.000000 cnvrgv2-1.0.9/cnvrgv2/modules/resources/_spark_driver.py
+-rw-r--r--   0 leah       (501) staff       (20)     1475 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/resources/_spark_drivers_client.py
+-rw-r--r--   0 leah       (501) staff       (20)     1565 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/resources/cluster.py
+-rw-r--r--   0 leah       (501) staff       (20)     1424 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/resources/clusters_client.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.974520 cnvrgv2-1.0.9/cnvrgv2/modules/resources/templates/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-08 09:17:55.000000 cnvrgv2-1.0.9/cnvrgv2/modules/resources/templates/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)     4431 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/resources/templates/kube_template.py
+-rw-r--r--   0 leah       (501) staff       (20)     4998 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/resources/templates/kube_templates_client.py
+-rw-r--r--   0 leah       (501) staff       (20)     3465 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/resources/templates/spark_template.py
+-rw-r--r--   0 leah       (501) staff       (20)     3868 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/resources/templates/spark_templates_client.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.976141 cnvrgv2-1.0.9/cnvrgv2/modules/ssh/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2021-09-07 11:10:42.000000 cnvrgv2-1.0.9/cnvrgv2/modules/ssh/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)     1394 2021-11-03 14:03:29.000000 cnvrgv2-1.0.9/cnvrgv2/modules/ssh/ssh.py
+-rw-r--r--   0 leah       (501) staff       (20)      273 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/ssh/ssh_client.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.977583 cnvrgv2-1.0.9/cnvrgv2/modules/users/
+-rw-r--r--   0 leah       (501) staff       (20)       45 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/users/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)     2813 2022-04-11 13:19:18.000000 cnvrgv2-1.0.9/cnvrgv2/modules/users/user.py
+-rw-r--r--   0 leah       (501) staff       (20)     3238 2022-04-11 13:19:18.000000 cnvrgv2-1.0.9/cnvrgv2/modules/users/users_client.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.978859 cnvrgv2-1.0.9/cnvrgv2/modules/volumes/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-11 20:18:38.000000 cnvrgv2-1.0.9/cnvrgv2/modules/volumes/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)     1090 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/volumes/volume.py
+-rw-r--r--   0 leah       (501) staff       (20)     2766 2021-11-03 14:03:29.000000 cnvrgv2-1.0.9/cnvrgv2/modules/volumes/volumes_client.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.979685 cnvrgv2-1.0.9/cnvrgv2/modules/workflows/
+-rw-r--r--   0 leah       (501) staff       (20)      646 2021-11-03 14:03:29.000000 cnvrgv2-1.0.9/cnvrgv2/modules/workflows/__init__.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.981302 cnvrgv2-1.0.9/cnvrgv2/modules/workflows/endpoint/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-11 20:18:38.000000 cnvrgv2-1.0.9/cnvrgv2/modules/workflows/endpoint/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)    14240 2022-03-01 15:06:52.000000 cnvrgv2-1.0.9/cnvrgv2/modules/workflows/endpoint/endpoint.py
+-rw-r--r--   0 leah       (501) staff       (20)      669 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/workflows/endpoint/endpoint_rule.py
+-rw-r--r--   0 leah       (501) staff       (20)     2861 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/workflows/endpoint/endpoints_client.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.982453 cnvrgv2-1.0.9/cnvrgv2/modules/workflows/experiment/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-11 20:18:38.000000 cnvrgv2-1.0.9/cnvrgv2/modules/workflows/experiment/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)    12782 2022-03-01 15:06:52.000000 cnvrgv2-1.0.9/cnvrgv2/modules/workflows/experiment/experiment.py
+-rw-r--r--   0 leah       (501) staff       (20)     9291 2022-01-20 13:24:21.000000 cnvrgv2-1.0.9/cnvrgv2/modules/workflows/experiment/experiments_client.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.983777 cnvrgv2-1.0.9/cnvrgv2/modules/workflows/webapp/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-11 20:18:38.000000 cnvrgv2-1.0.9/cnvrgv2/modules/workflows/webapp/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)     1720 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/workflows/webapp/webapp.py
+-rw-r--r--   0 leah       (501) staff       (20)     2130 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/workflows/webapp/webapps_client.py
+-rw-r--r--   0 leah       (501) staff       (20)     1601 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/workflows/workflow_utils.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.985131 cnvrgv2-1.0.9/cnvrgv2/modules/workflows/workspace/
+-rw-r--r--   0 leah       (501) staff       (20)       48 2021-11-03 14:03:29.000000 cnvrgv2-1.0.9/cnvrgv2/modules/workflows/workspace/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)     4812 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/modules/workflows/workspace/workspace.py
+-rw-r--r--   0 leah       (501) staff       (20)     2315 2021-11-03 14:03:29.000000 cnvrgv2-1.0.9/cnvrgv2/modules/workflows/workspace/workspaces_client.py
+-rw-r--r--   0 leah       (501) staff       (20)     6559 2022-04-11 13:19:18.000000 cnvrgv2-1.0.9/cnvrgv2/proxy.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.985523 cnvrgv2-1.0.9/cnvrgv2/tryoutes/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2022-04-11 13:19:18.000000 cnvrgv2-1.0.9/cnvrgv2/tryoutes/__init__.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.991016 cnvrgv2-1.0.9/cnvrgv2/utils/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2021-04-08 09:17:55.000000 cnvrgv2-1.0.9/cnvrgv2/utils/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)     1850 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/utils/api_list_generator.py
+-rw-r--r--   0 leah       (501) staff       (20)     7330 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/utils/chart_utils.py
+-rw-r--r--   0 leah       (501) staff       (20)     1217 2021-09-07 11:10:42.000000 cnvrgv2-1.0.9/cnvrgv2/utils/converters.py
+-rw-r--r--   0 leah       (501) staff       (20)     2775 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/utils/cron.py
+-rw-r--r--   0 leah       (501) staff       (20)      177 2021-04-11 20:18:38.000000 cnvrgv2-1.0.9/cnvrgv2/utils/env_helper.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.992419 cnvrgv2-1.0.9/cnvrgv2/utils/files/
+-rw-r--r--   0 leah       (501) staff       (20)      186 2022-03-01 15:06:52.000000 cnvrgv2-1.0.9/cnvrgv2/utils/files/.cnvrgignore
+-rw-r--r--   0 leah       (501) staff       (20)        0 2022-03-01 15:06:52.000000 cnvrgv2-1.0.9/cnvrgv2/utils/files/__init__.py
+-rw-r--r--   0 leah       (501) staff       (20)      738 2021-09-07 11:10:42.000000 cnvrgv2-1.0.9/cnvrgv2/utils/filter_utils.py
+-rw-r--r--   0 leah       (501) staff       (20)     1533 2021-04-11 20:18:38.000000 cnvrgv2-1.0.9/cnvrgv2/utils/json_api_format.py
+-rw-r--r--   0 leah       (501) staff       (20)     1888 2021-04-11 20:18:38.000000 cnvrgv2-1.0.9/cnvrgv2/utils/log_utils.py
+-rw-r--r--   0 leah       (501) staff       (20)     1043 2021-11-03 14:03:28.000000 cnvrgv2-1.0.9/cnvrgv2/utils/retry.py
+-rw-r--r--   0 leah       (501) staff       (20)     7044 2022-03-06 10:51:53.000000 cnvrgv2-1.0.9/cnvrgv2/utils/storage_utils.py
+-rw-r--r--   0 leah       (501) staff       (20)      573 2021-04-08 09:17:55.000000 cnvrgv2-1.0.9/cnvrgv2/utils/suppress_exceptions.py
+-rw-r--r--   0 leah       (501) staff       (20)     1251 2021-09-07 11:10:42.000000 cnvrgv2-1.0.9/cnvrgv2/utils/url_utils.py
+-rw-r--r--   0 leah       (501) staff       (20)     3918 2022-04-04 07:39:09.000000 cnvrgv2-1.0.9/cnvrgv2/utils/validators.py
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.934172 cnvrgv2-1.0.9/cnvrgv2.egg-info/
+-rw-r--r--   0 leah       (501) staff       (20)      269 2022-04-11 13:20:01.000000 cnvrgv2-1.0.9/cnvrgv2.egg-info/PKG-INFO
+-rw-r--r--   0 leah       (501) staff       (20)     5559 2022-04-11 13:20:01.000000 cnvrgv2-1.0.9/cnvrgv2.egg-info/SOURCES.txt
+-rw-r--r--   0 leah       (501) staff       (20)        1 2022-04-11 13:20:01.000000 cnvrgv2-1.0.9/cnvrgv2.egg-info/dependency_links.txt
+-rw-r--r--   0 leah       (501) staff       (20)       80 2022-04-11 13:20:01.000000 cnvrgv2-1.0.9/cnvrgv2.egg-info/entry_points.txt
+-rw-r--r--   0 leah       (501) staff       (20)      747 2022-04-11 13:20:01.000000 cnvrgv2-1.0.9/cnvrgv2.egg-info/requires.txt
+-rw-r--r--   0 leah       (501) staff       (20)       17 2022-04-11 13:20:01.000000 cnvrgv2-1.0.9/cnvrgv2.egg-info/top_level.txt
+drwxr-xr-x   0 leah       (501) staff       (20)        0 2022-04-11 13:20:01.993271 cnvrgv2-1.0.9/examples/
+-rw-r--r--   0 leah       (501) staff       (20)        0 2022-01-20 13:24:21.000000 cnvrgv2-1.0.9/examples/__init__.py
+-rwxr-xr-x   0 leah       (501) staff       (20)    10630 2022-03-01 15:06:52.000000 cnvrgv2-1.0.9/examples/create_load_cluster.py
+-rw-r--r--   0 leah       (501) staff       (20)      474 2022-04-11 13:19:18.000000 cnvrgv2-1.0.9/requirements.txt
+-rw-r--r--   0 leah       (501) staff       (20)       38 2022-04-11 13:20:01.994375 cnvrgv2-1.0.9/setup.cfg
+-rw-r--r--   0 leah       (501) staff       (20)     1220 2022-04-11 13:19:18.000000 cnvrgv2-1.0.9/setup.py
```

### Comparing `cnvrgv2-1.0.8/README.md` & `cnvrgv2-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/async.py` & `cnvrgv2-1.0.9/cnvrgv2/async.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/cli/cli.py` & `cnvrgv2-1.0.9/cnvrgv2/cli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from cnvrgv2.cli.modules.config import config
 from cnvrgv2.cli.modules.ssh.ssh import ssh_group
 from cnvrgv2.cli.utils import messages
 from cnvrgv2.cli.modules.users import users
 from cnvrgv2.cli.logger.logger import CnvrgLogger
 from cnvrgv2.cli.modules.project.project import project_group
+from cnvrgv2.cli.modules.libraries.library import library_group
 from cnvrgv2.cli.modules.dataset.dataset import dataset_group
 from cnvrgv2.cli.modules.project.experiment import experiment_group
 
 """
 To avoid issues reading unicode chars from stdin or writing to stdout, we need to ensure that the
 python3 runtime is correctly configured, if not, we try to force to utf-8.
 """
@@ -45,11 +46,12 @@
         click.echo(messages.CLI_UNEXPECTED_ERROR.format(str(e)), err=True)
 
 
 entry_point.add_command(users.login)
 entry_point.add_command(users.logout)
 entry_point.add_command(CnvrgLogger.set_logs_keep_duration)
 entry_point.add_command(project_group)
+entry_point.add_command(library_group)
 entry_point.add_command(experiment_group)
 entry_point.add_command(dataset_group)
 entry_point.add_command(ssh_group)
 entry_point.add_command(config)
```

### Comparing `cnvrgv2-1.0.8/cnvrgv2/cli/logger/logger.py` & `cnvrgv2-1.0.9/cnvrgv2/cli/logger/logger.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/cli/modules/config/config.py` & `cnvrgv2-1.0.9/cnvrgv2/cli/modules/config/config.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/cli/modules/dataset/dataset.py` & `cnvrgv2-1.0.9/cnvrgv2/cli/modules/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/cli/modules/project/experiment.py` & `cnvrgv2-1.0.9/cnvrgv2/cli/modules/project/experiment.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/cli/modules/project/project.py` & `cnvrgv2-1.0.9/cnvrgv2/cli/modules/project/project.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/cli/modules/ssh/ssh.py` & `cnvrgv2-1.0.9/cnvrgv2/cli/modules/ssh/ssh.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/cli/modules/users/users.py` & `cnvrgv2-1.0.9/cnvrgv2/cli/modules/users/users.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/cli/utils/decorators.py` & `cnvrgv2-1.0.9/cnvrgv2/cli/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/cli/utils/messages.py` & `cnvrgv2-1.0.9/cnvrgv2/cli/utils/messages.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,20 @@
 PROJECT_HELP_CREATE = "Name for the new project"
 PROJECT_CREATE_FOLDER_NOT_EMPTY = "Warning! You're about to associate a non empty folder with the new project." \
                                   "\r\nContinue?"
 PROJECT_CREATING_PROJECT = "Creating new project {0}"
 PROJECT_CREATE_SUCCESS = "Successfully created project {0}"
 PROJECT_DOWNLOAD_HELP_COMMIT = "Sha1 of the commit to download"
 
+# LIBRARIES
+LIBRARY_PROMPT_CLONE = "Please enter library name to clone"
+LIBRARY_VERSION_PROMPT_CLONE = "Please enter library version name to clone (default = \"latest\")"
+LIBRARY_CLONE_SKIP = "Library {0} is already cloned, skipping action"
+LIBRARY_CLONE_SUCCESS = "Successfully cloned project: {0}"
+
 
 # EXPERIMENT
 EXPERIMENT_PROMPT_TITLE = "Please enter a title for the experiment"
 EXPERIMENT_HELP_TITLE = "Name of the experiment"
 EXPERIMENT_HELP_TEMPLATES = "Comma separated list of template names"
 EXPERIMENT_HELP_LOCAL = "Boolean. Run the experiment locally"
 EXPERIMENT_PROMPT_COMMAND = "Please enter a command to run as experiment"
@@ -86,14 +92,15 @@
 EXPERIMENT_HELP_GIT_BRANCH = "The branch to pull files from for the experiment, in case project is git project"
 EXPERIMENT_HELP_GIT_COMMIT = "The commit to pull files from for the experiment, in case project is git project"
 EXPERIMENT_CREATE_SUCCESS = "Experiment {0} created successfully. \r\nExperiment is available at: {1}"
 
 # LOGS
 LOG_START_COMMAND = "Starting command {0}. Options: {1}"
 LOG_CLONING_PROJECT = "Cloning project: {0}"
+LOG_CLONING_LIBRARY = "Cloning library: {0}=={1}"
 LOG_CLONING_DATASET = "Cloning dataset: {0}"
 
 # SSH
 SSH_HELP_PORT = "Port to bind on host"
 SSH_HELP_USERNAME = "Username to login in container, default will be image default user"
 SSH_HELP_PASSWORD = "Password for login"
 SSH_HELP_KUBECTL = "Full path to kubeconfig file, otherwise default will be used"
```

### Comparing `cnvrgv2-1.0.8/cnvrgv2/cli/utils/progress_bar_utils.py` & `cnvrgv2-1.0.9/cnvrgv2/cli/utils/progress_bar_utils.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/cnvrg.py` & `cnvrgv2-1.0.9/cnvrgv2/cnvrg.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from cnvrgv2.errors import CnvrgError, CnvrgArgumentsError
 from cnvrgv2.context import Context, SCOPE
 from cnvrgv2.modules.images.images_client import ImagesClient
 from cnvrgv2.modules.ssh.ssh_client import SshClient
 from cnvrgv2.modules.users.users_client import UsersClient
 from cnvrgv2.modules.users.user import User, ROLES
 from cnvrgv2.modules.projects_client import ProjectsClient
+from cnvrgv2.modules.libhub.libraries.libraries_client import LibrariesClient
 from cnvrgv2.modules.datasets_client import DatasetsClient
 from cnvrgv2.modules.resources.clusters_client import ClustersClient
 from cnvrgv2.modules.organization.organization_settings import OrganizationSettings
 from cnvrgv2.proxy import Proxy, HTTP
 from cnvrgv2.utils.json_api_format import JAF
 from cnvrgv2.utils.validators import validate_email, validate_user_role
 
@@ -35,15 +36,15 @@
         self._organization = organization or self._context.organization
 
     def me(self):
         """
         Retrieves information about the current user
         @return: A dictionary representing the current logged in user
         """
-        users_client = UsersClient(self._context.domain, self._context.token)
+        users_client = UsersClient(self._context.domain, self._context.token, is_capi=self._context.is_capi)
         return users_client.me()
 
     def is_admin(self):
         """
         @return: Returns if the logged user is an admin in the current organization or not
         """
         user_membership = next(membership for membership in self.me().roles
@@ -94,15 +95,15 @@
         if not validate_user_role(role):
             raise CnvrgArgumentsError(FAULTY_VALUE.format(role))
 
         if not validate_email(email):
             raise CnvrgArgumentsError(FAULTY_VALUE.format(email))
 
         # TODO fix workaround
-        organization = self._organization if self._organization is str else self._organization['organization']
+        organization = self._organization if isinstance(self._organization, str) else self._organization['organization']
         self._proxy.call_api(
             route=routes.ORGANIZATION_USERS.format(organization),
             http_method=HTTP.POST,
             payload=JAF.serialize(type="users", attributes={"email": email, "role": role})
         )
 
     def revoke_user(self, email):
@@ -123,14 +124,15 @@
         """
         Sets up the clients that are exposed to the user.
         @return: None
         """
         try:
             self.projects = ProjectsClient(self)
             self.datasets = DatasetsClient(self)
+            self.libraries = LibrariesClient(self)
             self.images = ImagesClient(self)
             self.settings = OrganizationSettings(self)
             self.clusters = ClustersClient(self)
             self.ssh = SshClient(self)
 
         except CnvrgError:
             # TODO: How to handle exceptions
```

### Comparing `cnvrgv2-1.0.8/cnvrgv2/config/config.py` & `cnvrgv2-1.0.9/cnvrgv2/config/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,30 +30,35 @@
         "version": float
     }
 
     local_config_attributes = {
         "git": bool,
         "commit_sha1": str,
         "project_slug": str,
+        "library_slug": str,
         "dataset_slug": str,
     }
 
     def __init__(self):
+        self.is_capi = None
         self.local_config = {}
         self.global_config = {}
         if self.local_cnvrg_path:
             self.root = str(Path(self.local_cnvrg_path).parent)
         else:
             self.root = ""
 
         # Support legacy config files
         self._load_legacy_config()
 
         if self.global_config_exists:
             global_config = yaml.safe_load(open(self.global_config_file_path, "r")) or {}
+            if global_config.get("token"):
+                self.is_capi = True
+
             for key in Config.global_config_attributes.keys():
                 default = False if Config.global_config_attributes[key] == bool else None
                 self.global_config[key] = global_config.get(key, default) or self.global_config.get(key, default)
 
         if self.local_config_exists:
             local_config = yaml.safe_load(open(self.local_config_file_path, "r")) or {}
             for key in Config.local_config_attributes.keys():
@@ -102,39 +107,45 @@
 
         legacy_global_config_exists = os.path.exists(legacy_global_config_file_path)
         legacy_netrc_exists = os.path.exists(LEGACY_NETRC_PATH)
 
         legacy_idx_exists = os.path.exists(legacy_idx_file_path)
         legacy_config_exists = os.path.exists(legacy_config_file_path)
 
+        organization = None
         # We want to try and load legacy config file BEFORE the new config file so we can override if needed
         if legacy_global_config_exists:
-            legacy_global_config = yaml.safe_load(open(legacy_global_config_file_path, "r"))
+            legacy_global_config = yaml.safe_load(open(legacy_global_config_file_path, "r")) or {}
+            organization = legacy_global_config.get(":owner", None) or legacy_global_config.get("owner", None)
             api = legacy_global_config.get(":api", None) or legacy_global_config.get("api", None)
             uri = urllib.parse.urlparse(api)
-            self.domain = '{uri.scheme}://{uri.hostname}/'.format(uri=uri)
+            self.domain = '{uri.scheme}://{uri.netloc}/'.format(uri=uri)
 
         if legacy_netrc_exists:
             netrc_file = netrc.netrc()
             authTokens = netrc_file.authenticators("cnvrg.io")
             # 0 is login, 1 is account, 2 is password
             self.user = authTokens[0]
             self.token = authTokens[2]
+            self.is_capi = False
 
         if legacy_config_exists:
-            legacy_config = yaml.safe_load(open(legacy_config_file_path, "r"))
-            self.organization = legacy_config.get(":owner", None) or legacy_config.get("owner", None)
+            legacy_config = yaml.safe_load(open(legacy_config_file_path, "r")) or {}
+            organization = legacy_config.get(":owner", None) or legacy_config.get("owner", None) or organization
             self.project_slug = legacy_config.get("project_slug", None) or legacy_config.get(":project_slug", None)
+            self.library_slug = legacy_config.get("project_slug", None) or legacy_config.get(":library_slug", None)
             self.dataset_slug = legacy_config.get("dataset_slug", None) or legacy_config.get(":dataset_slug", None)
             self.git = legacy_config.get(":git", False) or legacy_config.get("git", False)
 
         if legacy_idx_exists:
-            legacy_idx_config = yaml.safe_load(open(legacy_idx_file_path, "r"))
+            legacy_idx_config = yaml.safe_load(open(legacy_idx_file_path, "r")) or {}
             self.commit_sha1 = legacy_idx_config.get(":commit", None) or legacy_idx_config.get("commit", None)
 
+        self.organization = organization
+
     def __getattr__(self, name):
         """
         Returns an attribute value from the local/global config attributes
         @param name: Name of the attribute to return
         @return: The value of the given attribute
         """
         is_global = name in Config.global_config_attributes.keys()
```

### Comparing `cnvrgv2-1.0.8/cnvrgv2/config/error_messages.py` & `cnvrgv2-1.0.9/cnvrgv2/config/error_messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,17 @@
 # COMMIT
 COMMIT_FAULTY_SHA1 = "Commit sha1 must be a string"
 
 # PROJECT
 PROJECT_GET_FAULTY_SLUG = "Cannot get project with empty slug or a non string slug"
 PROJECT_CREATE_FAULTY_NAME = "Cannot create project with empty/non-string name"
 
+# LIBRARY
+LIBRARY_GET_FAULTY_SLUG = "Cannot get library with empty slug or a non string slug"
+
 # DATASET
 DATASET_GET_FAULTY_SLUG = "Cannot get dataset with empty slug or a non string slug"
 DATASET_CREATE_FAULTY_NAME = "Cannot create dataset with empty/non-string name"
 DATASET_CREATE_FAULTY_CATEGORY = "Cannot create dataset with empty/non-string category"
 DATASET_CREATE_FAULTY_CATEGORY_VALUE = "Dataset category must be one of [general, images, audio, video, text, tabular]"
 NOT_A_DATASET_LIST_OBJECT = "datasets must be a list of datasets objects"
 NOT_A_DATASET_OBJECT = "dataset parameter missing or not a dataset object"
```

### Comparing `cnvrgv2-1.0.8/cnvrgv2/config/routes.py` & `cnvrgv2-1.0.9/cnvrgv2/config/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,22 @@
 PROJECT_DELETE_SECRET = "delete_secrets"
 PROJECT_UPDATE_SECRET = "update_secrets"
 
 # DATASET
 DATASETS_BASE = "v2/{0}/datasets/"
 DATASET_BASE = "v2/{0}/datasets/{1}"
 
+# LIBHUB
+LIBHUB_BASE = "v2/libhub/"
+LIBRARIES_BASE = "v2/{0}/libhub/libraries/"
+LIBRARY_BASE = "v2/{0}/libhub/libraries/{1}/"
+USE_LIBRARY_SUFFIX = "use"
+LIBRARY_VERSIONS_BASE = "v2/{0}/libhub/libraries/{1}/versions/"
+LIBRARY_VERSION_BASE = "v2/{0}/libhub/libraries/{1}/versions/{2}"
+
 # COMMIT
 COMMITS_BASE = "v2/{0}/datasets/{1}/commits/"
 COMMIT_BASE = "v2/{0}/datasets/{1}/commits/{2}"
 COMMIT_REMOVE_FILES = "commits/{0}/remove_files?page[size]=1000&sort=id"
 
 # QUERIES
 QUERY_BASE = "v2/{0}/datasets/{1}/queries/{2}"
```

### Comparing `cnvrgv2-1.0.8/cnvrgv2/context.py` & `cnvrgv2-1.0.9/cnvrgv2/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,22 @@
         "key": "volume",
         "dependencies": ["project", "organization", "user"]
     }
     DATASET = {
         "key": "dataset",
         "dependencies": ["organization", "user"]
     }
+    LIBRARY = {
+        "key": "library",
+        "dependencies": ["organization", "user"]
+    }
+    LIBRARY_VERSION = {
+        "key": "library_version",
+        "dependencies": ["library", "organization", "user"]
+    }
     COMMIT = {
         "key": "commit",
         "dependencies": ["dataset", "organization", "user"]
     }
     QUERY = {
         "key": "query",
         "dependencies": ["dataset", "organization", "user"]
@@ -80,19 +88,20 @@
         for attr in dir(cls):
             if not callable(getattr(cls, attr)) and not attr.startswith("__"):
                 scopes.append(getattr(cls, attr)["key"])
         return scopes
 
 
 class Context:
-    def __init__(self, context=None, domain=None, user=None, password=None, organization=None, token=None):
+    def __init__(self, context=None, domain=None, user=None, password=None, organization=None, token=None, is_capi=True):
         # Set the credentials variables:
         self.token = None
         self.domain = None
         self.user = None
+        self.is_capi = is_capi
 
         # Set scope variables:
         for scope in SCOPE.scopes():
             setattr(self, scope, None)
 
         # If a context is passed, perform a deep copy and return
         if context:
@@ -105,15 +114,15 @@
 
         # If a domain is passed, init a blank Cnvrg client
         if domain:
             self.domain = domain
 
             # Attempt to authenticate using the credentials if they were passed
             if user:
-                self._authenticate(domain, user, password, token)
+                self._authenticate(domain, user, password, token, is_capi)
         else:
             self._load_credentials()
 
         # Override organization if it was explicitly passed
         if organization:
             self.organization = organization
 
@@ -165,14 +174,15 @@
         """
         Performs a deep copy of the supplied context into the current one
         @param context: The source context
         @param organization: Organization name to override
         @return: None
         """
         self.token = context.token
+        self.is_capi = context.is_capi
         self.domain = context.domain
         self.user = context.user
 
         for scope in SCOPE.scopes():
             target_attr = getattr(context, scope, None)
             setattr(self, scope, target_attr)
 
@@ -193,24 +203,24 @@
                 error_msg = error_messages.CONTEXT_SCOPE_BAD_DEPENDENCIES.format(scope["key"], dependency)
                 raise CnvrgError(error_msg)
             else:
                 scope_dict[dependency] = dependency_slug
 
         return scope_dict
 
-    def _authenticate(self, domain, user, password, user_token=None):
+    def _authenticate(self, domain, user, password, user_token=None, is_capi=True):
         """
         Performs authentication against Cnvrg and retrieves the auth token
         @param domain: Cnvrg app domain
         @param user: Email with which the user was registered
         @param password: Password with which the user was registered
         @param user_token: user authentication token instead of password
         @return: None
         """
-        auth = UsersClient(domain=domain, token=user_token)
+        auth = UsersClient(domain=domain, token=user_token, is_capi=is_capi)
 
         if password is None:
             password = ""
 
         # Will raise an exception if login did not succeed
         token, organization = auth.login(user=user, password=password)
 
@@ -284,14 +294,15 @@
         # Context variables
         organization = config.organization
 
         if not all([token, domain, user, organization]):
             return False
 
         self.token = token
+        self.is_capi = config.is_capi
         self.domain = domain
         self.user = user
         self.organization = organization
 
         if config.project_slug:
             self.project = config.project_slug
         if config.dataset_slug:
@@ -322,15 +333,15 @@
         if self.dataset:
             context["dataset_slug"] = self.dataset
 
         return context
 
     def ensure_organization_exist(self, name):
         try:
-            proxy = Proxy(domain=self.domain, token=self.token)
+            proxy = Proxy(domain=self.domain, token=self.token, is_capi=self.is_capi)
             organization_route = routes.ORGANIZATION_BASE.format(name)
 
             proxy.call_api(route=organization_route, http_method=HTTP.GET)
 
         except CnvrgHttpError as e:
             if e.status_code == requests.codes.not_found:
                 raise CnvrgArgumentsError(error_messages.ORGANIZATION_DOESNT_EXIST)
```

### Comparing `cnvrgv2-1.0.8/cnvrgv2/data/artifacts_downloader.py` & `cnvrgv2-1.0.9/cnvrgv2/data/artifacts_downloader.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/data/clients/azure/client.py` & `cnvrgv2-1.0.9/cnvrgv2/data/clients/azure/client.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/data/clients/base_storage_client.py` & `cnvrgv2-1.0.9/cnvrgv2/data/clients/base_storage_client.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/data/clients/gcp/client.py` & `cnvrgv2-1.0.9/cnvrgv2/data/clients/gcp/client.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/data/clients/minio/client.py` & `cnvrgv2-1.0.9/cnvrgv2/data/clients/minio/client.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/data/clients/s3/client.py` & `cnvrgv2-1.0.9/cnvrgv2/data/clients/s3/client.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/data/clients/storage_client_factory.py` & `cnvrgv2-1.0.9/cnvrgv2/data/clients/storage_client_factory.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/data/data_loader.py` & `cnvrgv2-1.0.9/cnvrgv2/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/data/file_compare.py` & `cnvrgv2-1.0.9/cnvrgv2/data/file_compare.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/data/file_downloader.py` & `cnvrgv2-1.0.9/cnvrgv2/data/file_downloader.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/data/file_uploader.py` & `cnvrgv2-1.0.9/cnvrgv2/data/file_uploader.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/data/local_file_deleter.py` & `cnvrgv2-1.0.9/cnvrgv2/data/local_file_deleter.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/data/local_files_handler.py` & `cnvrgv2-1.0.9/cnvrgv2/data/local_files_handler.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/data/remote_file_deleter.py` & `cnvrgv2-1.0.9/cnvrgv2/data/remote_file_deleter.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/data/remote_files_handler.py` & `cnvrgv2-1.0.9/cnvrgv2/data/remote_files_handler.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/errors.py` & `cnvrgv2-1.0.9/cnvrgv2/errors.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/base/data_owner.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/base/data_owner.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/base/dynamic_attributes.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/base/dynamic_attributes.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/base/workflow_instance_base.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/base/workflow_instance_base.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/base/workflows_base.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/base/workflows_base.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/commit.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/commit.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/dataset.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/dataset.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/datasets_client.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/datasets_client.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/flows/flow.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/flows/flow.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/flows/flow_version/flow_version.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/flows/flow_version/flow_version.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/flows/flow_version/flow_versions_client.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/flows/flow_version/flow_versions_client.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/flows/flows_client.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/flows/flows_client.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/images/image.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/images/image.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/images/images_client.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/images/images_client.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/organization/organization_settings.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/organization/organization_settings.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/organization/organizations_client.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/organization/organizations_client.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/project.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/project.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/project_settings.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/project_settings.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/projects_client.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/projects_client.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/queries/queries_client.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/queries/queries_client.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/queries/query.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/queries/query.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/resources/_machine.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/resources/_machine.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/resources/_machines_client.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/resources/_machines_client.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/resources/_spark_driver.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/resources/_spark_driver.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/resources/_spark_drivers_client.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/resources/_spark_drivers_client.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/resources/cluster.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/resources/cluster.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/resources/clusters_client.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/resources/clusters_client.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/resources/templates/kube_template.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/resources/templates/kube_template.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/resources/templates/kube_templates_client.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/resources/templates/kube_templates_client.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/resources/templates/spark_template.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/resources/templates/spark_template.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/resources/templates/spark_templates_client.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/resources/templates/spark_templates_client.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/ssh/ssh.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/ssh/ssh.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/users/user.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/users/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,16 @@
         "git_access_token": str,
         "default_homepage": str,
         "vscode_settings": str,
         "roles": list,
         "organizations": list
     }
 
-    def __init__(self, domain, token, attributes=None):
-        self._proxy = Proxy(domain=domain, token=token)
+    def __init__(self, domain, token, is_capi=True, attributes=None):
+        self._proxy = Proxy(domain=domain, token=token, is_capi=is_capi)
         if attributes:
             self._email = attributes["email"]
             attributes["icon"] = None
             attributes["vscode_settings"] = None
 
         self._token = token
         self._route = routes.USER_CURRENT
```

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/users/users_client.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/users/users_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 from cnvrgv2.errors import CnvrgArgumentsError
 from cnvrgv2.config import routes, error_messages
 from cnvrgv2.config.error_messages import FAULTY_VALUE
 from cnvrgv2.utils.validators import validate_url, validate_email, validate_username
 
 
 class UsersClient:
-    def __init__(self, domain, token=None):
+    def __init__(self, domain, token=None, is_capi=True):
         if not validate_url(domain):
             raise CnvrgArgumentsError(error_messages.INVALID_URL)
 
         self._domain = domain
         self._token = token
-        self._proxy = Proxy(domain=domain, token=token)
+        self._is_capi = is_capi
+        self._proxy = Proxy(domain=domain, token=token, is_capi=is_capi)
 
     def login(self, user, password):
         """
         Authenticates the user with the given username/password
         @param user: The users Email
         @param password: the users password
         @raise CnvrgHttpError: If the user data is incorrect
@@ -88,8 +89,8 @@
             raise CnvrgArgumentsError(error_messages.CONTEXT_CANT_SAVE)
 
         response = self._proxy.call_api(
             route=routes.USER_CURRENT,
             http_method=HTTP.GET
         )
 
-        return User(domain=self._domain, token=self._token, attributes=response.attributes)
+        return User(domain=self._domain, token=self._token, is_capi=self._is_capi, attributes=response.attributes)
```

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/volumes/volume.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/volumes/volume.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/volumes/volumes_client.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/volumes/volumes_client.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/workflows/__init__.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/workflows/endpoint/endpoint.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/workflows/endpoint/endpoint.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/workflows/endpoint/endpoint_rule.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/workflows/endpoint/endpoint_rule.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/workflows/endpoint/endpoints_client.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/workflows/endpoint/endpoints_client.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/workflows/experiment/experiment.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/workflows/experiment/experiment.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/workflows/experiment/experiments_client.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/workflows/experiment/experiments_client.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/workflows/webapp/webapp.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/workflows/webapp/webapp.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/workflows/webapp/webapps_client.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/workflows/webapp/webapps_client.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/workflows/workflow_utils.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/workflows/workflow_utils.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/workflows/workspace/workspace.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/workflows/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/modules/workflows/workspace/workspaces_client.py` & `cnvrgv2-1.0.9/cnvrgv2/modules/workflows/workspace/workspaces_client.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/proxy.py` & `cnvrgv2-1.0.9/cnvrgv2/proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,22 +15,24 @@
     POST = "POST"
     PUT = "PUT"
     DELETE = "DELETE"
     OPTIONS = "OPTIONS"
 
 
 class Proxy:
-    def __init__(self, context=None, domain=None, token=None):
+    def __init__(self, context=None, domain=None, token=None, is_capi=True):
         # Those are using for User/Org clients that do not have context
         self._domain = domain
         self._token = token
+        self._is_capi = is_capi
 
         if context:
             self._domain = context.domain
             self._token = context.token
+            self._is_capi = context.is_capi
 
     def call_api(self, route, http_method, payload=None, files_list=None, headers=None):
         """
         The main function controlling access to the Cnvrg API
         @param route: the partial url of the api resource to access
         @param http_method: get/post/put/delete
         @param payload: params to send along with the api request
@@ -97,15 +99,19 @@
         # Copy the headers so we wont change the original input
         full_headers = dict(headers)
 
         # If it's a file, we'll let requests lib complete the Content-Type (multipart/form-data)
         if not is_file:
             full_headers['Content-Type'] = "application/json"
         full_headers['User-Agent'] = "cnvrg/{version}".format(version=__version__)
-        full_headers['Authorization'] = "CAPI {jwt}".format(jwt=self._token)
+        if self._is_capi:
+            full_headers['Authorization'] = "CAPI {capi}".format(capi=self._token)
+        else:
+            full_headers['Auth-Token'] = self._token
+
         full_headers['Source'] = "sdk_v2"
         return full_headers
 
     def _parse_response(self, response):
         """
         This function handles the response from the api, decodes the json and returns the appropriate object
         @param response: Response object to handle
```

### Comparing `cnvrgv2-1.0.8/cnvrgv2/utils/api_list_generator.py` & `cnvrgv2-1.0.9/cnvrgv2/utils/api_list_generator.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/utils/chart_utils.py` & `cnvrgv2-1.0.9/cnvrgv2/utils/chart_utils.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/utils/converters.py` & `cnvrgv2-1.0.9/cnvrgv2/utils/converters.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/utils/cron.py` & `cnvrgv2-1.0.9/cnvrgv2/utils/cron.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/utils/filter_utils.py` & `cnvrgv2-1.0.9/cnvrgv2/utils/filter_utils.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/utils/json_api_format.py` & `cnvrgv2-1.0.9/cnvrgv2/utils/json_api_format.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/utils/log_utils.py` & `cnvrgv2-1.0.9/cnvrgv2/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/utils/retry.py` & `cnvrgv2-1.0.9/cnvrgv2/utils/retry.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/utils/storage_utils.py` & `cnvrgv2-1.0.9/cnvrgv2/utils/storage_utils.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/utils/suppress_exceptions.py` & `cnvrgv2-1.0.9/cnvrgv2/utils/suppress_exceptions.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/utils/url_utils.py` & `cnvrgv2-1.0.9/cnvrgv2/utils/url_utils.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2/utils/validators.py` & `cnvrgv2-1.0.9/cnvrgv2/utils/validators.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/cnvrgv2.egg-info/SOURCES.txt` & `cnvrgv2-1.0.9/cnvrgv2.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 cnvrgv2/cli/logger/__init__.py
 cnvrgv2/cli/logger/logger.py
 cnvrgv2/cli/modules/__init__.py
 cnvrgv2/cli/modules/config/__init__.py
 cnvrgv2/cli/modules/config/config.py
 cnvrgv2/cli/modules/dataset/__init__.py
 cnvrgv2/cli/modules/dataset/dataset.py
+cnvrgv2/cli/modules/libraries/__init__.py
+cnvrgv2/cli/modules/libraries/library.py
 cnvrgv2/cli/modules/project/__init__.py
 cnvrgv2/cli/modules/project/experiment.py
 cnvrgv2/cli/modules/project/project.py
 cnvrgv2/cli/modules/ssh/__init__.py
 cnvrgv2/cli/modules/ssh/ssh.py
 cnvrgv2/cli/modules/users/__init__.py
 cnvrgv2/cli/modules/users/users.py
@@ -80,14 +82,20 @@
 cnvrgv2/modules/flows/flows_client.py
 cnvrgv2/modules/flows/flow_version/__init__.py
 cnvrgv2/modules/flows/flow_version/flow_version.py
 cnvrgv2/modules/flows/flow_version/flow_versions_client.py
 cnvrgv2/modules/images/__init__.py
 cnvrgv2/modules/images/image.py
 cnvrgv2/modules/images/images_client.py
+cnvrgv2/modules/libhub/__init__.py
+cnvrgv2/modules/libhub/libraries/__init__.py
+cnvrgv2/modules/libhub/libraries/libraries_client.py
+cnvrgv2/modules/libhub/libraries/library.py
+cnvrgv2/modules/libhub/libraries/library_version.py
+cnvrgv2/modules/libhub/libraries/library_versions_client.py
 cnvrgv2/modules/organization/__init__.py
 cnvrgv2/modules/organization/organization_settings.py
 cnvrgv2/modules/organization/organizations_client.py
 cnvrgv2/modules/queries/__init__.py
 cnvrgv2/modules/queries/queries_client.py
 cnvrgv2/modules/queries/query.py
 cnvrgv2/modules/resources/__init__.py
@@ -122,14 +130,15 @@
 cnvrgv2/modules/workflows/experiment/experiments_client.py
 cnvrgv2/modules/workflows/webapp/__init__.py
 cnvrgv2/modules/workflows/webapp/webapp.py
 cnvrgv2/modules/workflows/webapp/webapps_client.py
 cnvrgv2/modules/workflows/workspace/__init__.py
 cnvrgv2/modules/workflows/workspace/workspace.py
 cnvrgv2/modules/workflows/workspace/workspaces_client.py
+cnvrgv2/tryoutes/__init__.py
 cnvrgv2/utils/__init__.py
 cnvrgv2/utils/api_list_generator.py
 cnvrgv2/utils/chart_utils.py
 cnvrgv2/utils/converters.py
 cnvrgv2/utils/cron.py
 cnvrgv2/utils/env_helper.py
 cnvrgv2/utils/filter_utils.py
```

### Comparing `cnvrgv2-1.0.8/cnvrgv2.egg-info/requires.txt` & `cnvrgv2-1.0.9/cnvrgv2.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 oauthlib>=3.1.0
 progress==1.5
 protobuf>=3.17.2
 pyaml>=20.4.0
 pyasn1>=0.4.8
 pyasn1-modules>=0.2.8
 pycparser>=2.20
-pycrypto>=2.6.1
+pycryptodome==3.14.1
 python-dateutil>=2.8.1
 pytz>=2021.1
 PyYAML>=5.3.1
 requests==2.23.0
 requests-oauthlib==1.3.0
 rsa>=4.7.2
 s3transfer>=0.3.7
 six>=1.15.0
 urllib3>=1.25.11
 
 [azure]
 azure-core>=1.10.0
-azure-storage-blob>=12.6.0
+azure-storage-blob>=12.10.0
 
 [dev]
 pytest
 pytest-mock
 
 [google]
 google-api-core>=1.23.0
```

### Comparing `cnvrgv2-1.0.8/examples/create_load_cluster.py` & `cnvrgv2-1.0.9/examples/create_load_cluster.py`

 * *Files identical despite different names*

### Comparing `cnvrgv2-1.0.8/setup.py` & `cnvrgv2-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     extras_require={
         'dev': [
             'pytest',
             'pytest-mock'
         ],
         'azure': [
             'azure-core>=1.10.0',
-            'azure-storage-blob>=12.6.0'
+            'azure-storage-blob>=12.10.0'
         ],
         'google': [
             'google-api-core>=1.23.0',
             'google-cloud-core>=1.4.4',
             'google-cloud-storage>=1.32.0',
             'google-auth>=1.23.0',
             'google-crc32c>=1.0.0',
```

