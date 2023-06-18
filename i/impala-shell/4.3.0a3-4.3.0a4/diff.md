# Comparing `tmp/impala_shell-4.3.0a3.tar.gz` & `tmp/impala_shell-4.3.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/wenzhe/projects/impala/shell/dist/impala_shell-4.3.0a3.tar", last modified: Thu May 25 22:17:36 2023, max compression
+gzip compressed data, was "/home/wenzhe/projects/impala/shell/dist/impala_shell-4.3.0a4.tar", last modified: Sun Jun 18 06:08:08 2023, max compression
```

## Comparing `impala_shell-4.3.0a3.tar` & `impala_shell-4.3.0a4.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     3913 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/PKG-INFO
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    58107 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/LICENSE.txt
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/Exprs/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Exprs/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    59637 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Exprs/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Exprs/__init__.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     2157 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/shell_exceptions.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/Metrics/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Metrics/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     1755 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Metrics/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Metrics/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/ResourceProfile/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ResourceProfile/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     4395 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ResourceProfile/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ResourceProfile/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/fb303/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/fb303/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      961 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/fb303/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       53 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/fb303/__init__.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    69618 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/fb303/FacebookService.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     1765 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/value_converter.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/Status/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Status/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     3396 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Status/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Status/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/SqlConstraints/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/SqlConstraints/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     4200 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/SqlConstraints/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/SqlConstraints/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/Partitions/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Partitions/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     3917 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Partitions/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Partitions/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/Descriptors/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Descriptors/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    32802 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Descriptors/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Descriptors/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/ImpalaInternalService/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      396 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ImpalaInternalService/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    38764 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ImpalaInternalService/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ImpalaInternalService/__init__.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     1433 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/compatibility.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     2393 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/impala_shell_config_defaults.py
--rwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)    70102 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/impala_client.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     2085 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/cookie_util.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      986 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/impala_build_version.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    17002 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ImpalaHttpClient.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/hive_metastore/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     1841 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/hive_metastore/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)  1141856 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/hive_metastore/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)  2099744 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/hive_metastore/ThriftHiveMetastore.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       57 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/hive_metastore/__init__.py
--rwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)    96419 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/impala_shell.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/BackendGflags/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/BackendGflags/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    83607 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/BackendGflags/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/BackendGflags/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/Frontend/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Frontend/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   257862 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Frontend/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Frontend/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/Zip/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Zip/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     3234 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Zip/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Zip/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/TCLIService/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     1055 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/TCLIService/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   136485 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/TCLIService/TCLIService.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   244075 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/TCLIService/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       49 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/TCLIService/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/PlanNodes/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/PlanNodes/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   171160 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/PlanNodes/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/PlanNodes/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/JniCatalog/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      412 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/JniCatalog/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   255110 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/JniCatalog/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/JniCatalog/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/ImpalaService/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ImpalaService/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    51193 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ImpalaService/ImpalaHiveServer2Service.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    69461 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ImpalaService/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       79 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ImpalaService/__init__.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    47740 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ImpalaService/ImpalaService.py
--rwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)    21476 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/option_parser.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/Logging/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Logging/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     6111 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Logging/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Logging/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/DataSinks/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/DataSinks/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    37237 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/DataSinks/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/DataSinks/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/MetricDefs/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   127227 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/MetricDefs/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     5039 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/MetricDefs/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/MetricDefs/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/StatestoreService/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/StatestoreService/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     8032 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/StatestoreService/StatestoreService.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    52057 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/StatestoreService/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       79 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/StatestoreService/__init__.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    13898 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/StatestoreService/StatestoreSubscriber.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     9123 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/shell_output.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/CatalogObjects/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      398 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/CatalogObjects/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   204572 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/CatalogObjects/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/CatalogObjects/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/NetworkTest/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/NetworkTest/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     7640 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/NetworkTest/NetworkTestService.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     4553 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/NetworkTest/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       56 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/NetworkTest/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/CatalogService/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    57260 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/CatalogService/CatalogService.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      432 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/CatalogService/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   155237 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/CatalogService/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       52 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/CatalogService/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/parquet/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/parquet/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   184091 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/parquet/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/parquet/__init__.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     2072 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/ExecStats/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ExecStats/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    20911 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ExecStats/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ExecStats/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/LineageGraph/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/LineageGraph/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    17384 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/LineageGraph/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/LineageGraph/__init__.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     6399 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/thrift_printer.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/Planner/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Planner/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    23434 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Planner/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Planner/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/ExternalDataSource/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ExternalDataSource/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    36903 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ExternalDataSource/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ExternalDataSource/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/CatalogInternalService/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/CatalogInternalService/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     7882 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/CatalogInternalService/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/CatalogInternalService/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/Types/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Types/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    43325 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Types/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Types/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/beeswaxd/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/beeswaxd/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    27060 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/beeswaxd/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    82393 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/beeswaxd/BeeswaxService.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       52 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/beeswaxd/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/RuntimeProfile/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/RuntimeProfile/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    73406 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/RuntimeProfile/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/RuntimeProfile/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/Query/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      451 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Query/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   148375 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Query/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Query/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/ErrorCodes/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    12746 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ErrorCodes/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    18611 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ErrorCodes/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ErrorCodes/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/Data/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Data/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    19140 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Data/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Data/__init__.py
--rwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)     6552 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/TSSLSocketWithWildcardSAN.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/Results/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Results/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     6110 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Results/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Results/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell.egg-info/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     3913 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell.egg-info/PKG-INFO
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)        1 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell.egg-info/dependency_links.txt
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     5215 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell.egg-info/SOURCES.txt
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       78 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell.egg-info/entry_points.txt
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      164 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell.egg-info/requires.txt
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       13 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell.egg-info/top_level.txt
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     6129 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/setup.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)        7 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/version.txt
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     2442 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/README.md
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       97 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/MANIFEST.in
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      164 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/requirements.txt
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       38 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/setup.cfg
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     3913 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/PKG-INFO
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    58107 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/LICENSE.txt
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/Exprs/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Exprs/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    59637 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Exprs/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Exprs/__init__.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     2157 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/shell_exceptions.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/Metrics/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Metrics/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     1755 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Metrics/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Metrics/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/ResourceProfile/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/ResourceProfile/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     4395 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/ResourceProfile/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/ResourceProfile/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/fb303/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/fb303/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      961 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/fb303/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       53 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/fb303/__init__.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    69618 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/fb303/FacebookService.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     1765 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/value_converter.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/Status/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Status/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     3396 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Status/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Status/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/SqlConstraints/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/SqlConstraints/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     4200 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/SqlConstraints/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/SqlConstraints/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/Partitions/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Partitions/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     3917 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Partitions/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Partitions/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/Descriptors/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Descriptors/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    32802 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Descriptors/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Descriptors/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/ImpalaInternalService/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      396 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/ImpalaInternalService/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    38764 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/ImpalaInternalService/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/ImpalaInternalService/__init__.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     1433 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/compatibility.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     2393 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/impala_shell_config_defaults.py
+-rwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)    70102 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/impala_client.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     2085 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/cookie_util.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      986 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/impala_build_version.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    17002 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/ImpalaHttpClient.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/hive_metastore/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     1841 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/hive_metastore/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)  1141856 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/hive_metastore/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)  2099744 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/hive_metastore/ThriftHiveMetastore.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       57 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/hive_metastore/__init__.py
+-rwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)    96645 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/impala_shell.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/BackendGflags/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/BackendGflags/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    83607 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/BackendGflags/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/BackendGflags/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/Frontend/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Frontend/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   257862 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Frontend/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Frontend/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/Zip/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Zip/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     3234 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Zip/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Zip/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/TCLIService/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     1055 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/TCLIService/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   136485 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/TCLIService/TCLIService.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   244075 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/TCLIService/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       49 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/TCLIService/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/PlanNodes/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/PlanNodes/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   171160 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/PlanNodes/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/PlanNodes/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/JniCatalog/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      412 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/JniCatalog/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   255110 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/JniCatalog/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/JniCatalog/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/ImpalaService/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/ImpalaService/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    51193 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/ImpalaService/ImpalaHiveServer2Service.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    69557 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/ImpalaService/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       79 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/ImpalaService/__init__.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    47740 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/ImpalaService/ImpalaService.py
+-rwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)    21473 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/option_parser.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/Logging/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Logging/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     6111 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Logging/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Logging/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/DataSinks/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/DataSinks/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    39282 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/DataSinks/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/DataSinks/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/MetricDefs/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   127227 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/MetricDefs/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     5039 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/MetricDefs/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/MetricDefs/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/StatestoreService/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/StatestoreService/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     8032 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/StatestoreService/StatestoreService.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    52057 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/StatestoreService/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       79 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/StatestoreService/__init__.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    13898 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/StatestoreService/StatestoreSubscriber.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     9123 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/shell_output.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/CatalogObjects/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      398 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/CatalogObjects/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   204517 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/CatalogObjects/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/CatalogObjects/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/NetworkTest/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/NetworkTest/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     7640 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/NetworkTest/NetworkTestService.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     4553 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/NetworkTest/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       56 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/NetworkTest/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/CatalogService/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    57260 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/CatalogService/CatalogService.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      432 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/CatalogService/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   156749 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/CatalogService/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       52 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/CatalogService/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/parquet/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/parquet/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   184091 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/parquet/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/parquet/__init__.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     2072 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/ExecStats/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/ExecStats/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    20911 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/ExecStats/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/ExecStats/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/LineageGraph/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/LineageGraph/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    17384 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/LineageGraph/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/LineageGraph/__init__.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     6399 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/thrift_printer.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/Planner/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Planner/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    23434 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Planner/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Planner/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/ExternalDataSource/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/ExternalDataSource/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    36903 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/ExternalDataSource/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/ExternalDataSource/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/CatalogInternalService/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/CatalogInternalService/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     7882 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/CatalogInternalService/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/CatalogInternalService/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/Types/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Types/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    43538 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Types/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Types/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/beeswaxd/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/beeswaxd/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    27060 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/beeswaxd/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    82393 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/beeswaxd/BeeswaxService.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       52 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/beeswaxd/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/RuntimeProfile/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/RuntimeProfile/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    73406 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/RuntimeProfile/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/RuntimeProfile/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/Query/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      451 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Query/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   151624 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Query/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Query/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/ErrorCodes/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    12746 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/ErrorCodes/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    18611 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/ErrorCodes/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/ErrorCodes/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/Data/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Data/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    19140 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Data/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Data/__init__.py
+-rwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)     6552 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/TSSLSocketWithWildcardSAN.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell/Results/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Results/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     6110 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Results/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/impala_shell/Results/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell.egg-info/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     3913 2023-06-18 06:08:07.000000 impala_shell-4.3.0a4/impala_shell.egg-info/PKG-INFO
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)        1 2023-06-18 06:08:07.000000 impala_shell-4.3.0a4/impala_shell.egg-info/dependency_links.txt
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     5215 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/impala_shell.egg-info/SOURCES.txt
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       78 2023-06-18 06:08:07.000000 impala_shell-4.3.0a4/impala_shell.egg-info/entry_points.txt
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      164 2023-06-18 06:08:07.000000 impala_shell-4.3.0a4/impala_shell.egg-info/requires.txt
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       13 2023-06-18 06:08:07.000000 impala_shell-4.3.0a4/impala_shell.egg-info/top_level.txt
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     6129 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/setup.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)        7 2023-06-18 06:08:07.000000 impala_shell-4.3.0a4/version.txt
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     2442 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/README.md
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       97 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/MANIFEST.in
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      164 2023-06-18 06:08:06.000000 impala_shell-4.3.0a4/requirements.txt
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       38 2023-06-18 06:08:08.000000 impala_shell-4.3.0a4/setup.cfg
```

### Comparing `impala_shell-4.3.0a3/PKG-INFO` & `impala_shell-4.3.0a4/impala_shell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: impala_shell
-Version: 4.3.0a3
+Name: impala-shell
+Version: 4.3.0a4
 Summary: Impala Shell
 Home-page: https://impala.apache.org/
 Author: Impala Dev
 Author-email: dev@impala.apache.org
 License: Apache Software License
 Description: # Impala Interactive Shell
```

### Comparing `impala_shell-4.3.0a3/LICENSE.txt` & `impala_shell-4.3.0a4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/Exprs/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/Exprs/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/shell_exceptions.py` & `impala_shell-4.3.0a4/impala_shell/shell_exceptions.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/Metrics/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/Metrics/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/ResourceProfile/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/ResourceProfile/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/fb303/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/fb303/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/fb303/FacebookService.py` & `impala_shell-4.3.0a4/impala_shell/fb303/FacebookService.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/value_converter.py` & `impala_shell-4.3.0a4/impala_shell/value_converter.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/Status/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/Status/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/SqlConstraints/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/SqlConstraints/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/Partitions/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/Partitions/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/Descriptors/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/Descriptors/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/ImpalaInternalService/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/ImpalaInternalService/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/compatibility.py` & `impala_shell-4.3.0a4/impala_shell/compatibility.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/impala_shell_config_defaults.py` & `impala_shell-4.3.0a4/impala_shell/impala_shell_config_defaults.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/impala_client.py` & `impala_shell-4.3.0a4/impala_shell/impala_client.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/cookie_util.py` & `impala_shell-4.3.0a4/impala_shell/cookie_util.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/impala_build_version.py` & `impala_shell-4.3.0a4/impala_shell/impala_build_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 def get_version():
-  return "4.3.0a3"
+  return "4.3.0a4"
 
 def get_git_hash():
-  return "ee300a1af09514af5650b0b14b90afc8d23d54b1"
+  return "06eb62d3efa1c94810c4276f90896fa62205a49b"
 
 def get_build_date():
-  return "Thu May 25 15:04:10 PDT 2023"
+  return "Sat Jun 17 22:34:59 PDT 2023"
```

### Comparing `impala_shell-4.3.0a3/impala_shell/ImpalaHttpClient.py` & `impala_shell-4.3.0a4/impala_shell/ImpalaHttpClient.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/hive_metastore/constants.py` & `impala_shell-4.3.0a4/impala_shell/hive_metastore/constants.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/hive_metastore/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/hive_metastore/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/hive_metastore/ThriftHiveMetastore.py` & `impala_shell-4.3.0a4/impala_shell/hive_metastore/ThriftHiveMetastore.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/impala_shell.py` & `impala_shell-4.3.0a4/impala_shell/impala_shell.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,14 +137,18 @@
   Status tells the caller that the command completed successfully.
   """
 
   # If not connected to an impalad, the server version is unknown.
   UNKNOWN_SERVER_VERSION = "Not Connected"
   PROMPT_FORMAT = "[{host}:{port}] {db}> "
   DISCONNECTED_PROMPT = "[Not connected] > "
+  # Message to display when the connection failed and it is reconnecting.
+  # This is used in some tests for verification that the session remained
+  # connected.
+  CONNECTION_LOST_MESSAGE = 'Connection lost, reconnecting...'
   # Message to display in shell when cancelling a query
   CANCELLATION_MESSAGE = ' Cancelling Query'
   # Number of times to attempt cancellation before giving up.
   CANCELLATION_TRIES = 3
   # Commands are terminated with the following delimiter.
   CMD_DELIM = ';'
   # Valid variable name pattern
@@ -722,15 +726,15 @@
       parsed_cmds[-1] += ImpalaShell.CMD_DELIM
       self.cmdqueue.extend(parsed_cmds)
       # If cmdqueue is populated, then commands are executed from the cmdqueue, and user
       # input is ignored. Send an empty string as the user input just to be safe.
       return str()
     # There is no need to reconnect if we are quitting.
     if not self.imp_client.is_connected() and not self._is_quit_command(args):
-      print("Connection lost, reconnecting...", file=sys.stderr)
+      print(ImpalaShell.CONNECTION_LOST_MESSAGE, file=sys.stderr)
       self._connect()
       self._validate_database(immediately=True)
     return args
 
   def onecmd(self, line):
     """Overridden to ensure the variable replacement is processed in interactive
        as well as non-interactive mode, since the precmd method would only work for
@@ -2246,17 +2250,14 @@
     if execute_queries_non_interactive_mode(options, query_options):
       return
     else:
       raise FatalShellException()
 
   intro = get_intro(options)
 
-  # Suppressing unwanted notifications from Thrift
-  logging.getLogger('thrift').addHandler(logging.NullHandler())
-
   with ImpalaShell(options, query_options) as shell:
     while shell.is_alive:
       try:
         try:
           shell.cmdloop(intro)
         except KeyboardInterrupt:
           print('^C', file=sys.stderr)
@@ -2287,12 +2288,14 @@
           # Interrupted system calls (e.g. because of cancellation) should be ignored.
           if e.errno != errno.EINTR: raise
       finally:
         intro = ''
 
 
 if __name__ == "__main__":
+  # Suppressing unwanted notifications from Thrift
+  logging.getLogger('thrift').addHandler(logging.NullHandler())
   try:
     impala_shell_main()
   except FatalShellException:
     # Ensure that fatal errors cause a clean exit with error.
     sys.exit(1)
```

### Comparing `impala_shell-4.3.0a3/impala_shell/BackendGflags/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/BackendGflags/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/Frontend/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/Frontend/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/Zip/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/Zip/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/TCLIService/constants.py` & `impala_shell-4.3.0a4/impala_shell/TCLIService/constants.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/TCLIService/TCLIService.py` & `impala_shell-4.3.0a4/impala_shell/TCLIService/TCLIService.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/TCLIService/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/TCLIService/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/PlanNodes/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/PlanNodes/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/JniCatalog/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/JniCatalog/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/ImpalaService/ImpalaHiveServer2Service.py` & `impala_shell-4.3.0a4/impala_shell/ImpalaService/ImpalaHiveServer2Service.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/ImpalaService/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/ImpalaService/ttypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,14 +178,15 @@
     CODEGEN_CACHE_MODE = 150
     STRINGIFY_MAP_KEYS = 151
     ENABLE_TRIVIAL_QUERY_FOR_ADMISSION = 152
     COMPUTE_PROCESSING_COST = 153
     PROCESSING_COST_MIN_THREADS = 154
     JOIN_SELECTIVITY_CORRELATION_FACTOR = 155
     MAX_FRAGMENT_INSTANCES_PER_NODE = 156
+    MAX_SORT_RUN_SIZE = 157
 
     _VALUES_TO_NAMES = {
         0: "ABORT_ON_ERROR",
         1: "MAX_ERRORS",
         2: "DISABLE_CODEGEN",
         3: "BATCH_SIZE",
         4: "MEM_LIMIT",
@@ -337,14 +338,15 @@
         150: "CODEGEN_CACHE_MODE",
         151: "STRINGIFY_MAP_KEYS",
         152: "ENABLE_TRIVIAL_QUERY_FOR_ADMISSION",
         153: "COMPUTE_PROCESSING_COST",
         154: "PROCESSING_COST_MIN_THREADS",
         155: "JOIN_SELECTIVITY_CORRELATION_FACTOR",
         156: "MAX_FRAGMENT_INSTANCES_PER_NODE",
+        157: "MAX_SORT_RUN_SIZE",
     }
 
     _NAMES_TO_VALUES = {
         "ABORT_ON_ERROR": 0,
         "MAX_ERRORS": 1,
         "DISABLE_CODEGEN": 2,
         "BATCH_SIZE": 3,
@@ -497,14 +499,15 @@
         "CODEGEN_CACHE_MODE": 150,
         "STRINGIFY_MAP_KEYS": 151,
         "ENABLE_TRIVIAL_QUERY_FOR_ADMISSION": 152,
         "COMPUTE_PROCESSING_COST": 153,
         "PROCESSING_COST_MIN_THREADS": 154,
         "JOIN_SELECTIVITY_CORRELATION_FACTOR": 155,
         "MAX_FRAGMENT_INSTANCES_PER_NODE": 156,
+        "MAX_SORT_RUN_SIZE": 157,
     }
 
 
 class TDmlResult(object):
     """
     Attributes:
      - rows_modified
```

### Comparing `impala_shell-4.3.0a3/impala_shell/ImpalaService/ImpalaService.py` & `impala_shell-4.3.0a4/impala_shell/ImpalaService/ImpalaService.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/option_parser.py` & `impala_shell-4.3.0a4/impala_shell/option_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,23 +316,23 @@
   parser.add_option("--http_path", dest="http_path", default="cliservice",
                     help="Default http path on the coordinator to connect to. The final "
                     "connection URL looks like <http(s)>://<coordinator-host>:<port>/"
                     "<http_path>. While the coordinator server implementation does not "
                     "enforce any http path for the incoming requests, deployments could "
                     "still put it behind a loadbalancer that can expect the traffic at a "
                     "certain path.")
-  parser.add_option("--fetch_size", type="int", dest="fetch_size", default=10240,
+  parser.add_option("--fetch_size", type="int", dest="fetch_size", default=8192,
                     help="The fetch size when fetching rows from the Impala coordinator. "
                     "The fetch size controls how many rows a single fetch RPC request "
                     "(RPC from the Impala shell to the Impala coordinator) reads at a "
                     "time. This option is most effective when result spooling is enabled "
                     "('spool_query_results'=true). When result spooling is enabled "
                     "values over the batch_size are honored. When result spooling is "
                     "disabled, values over the batch_size have no affect. By default, "
-                    "the fetch_size is set to 10240 which is equivalent to 10 row "
+                    "the fetch_size is set to 8192 which is equivalent to 8 row "
                     "batches (assuming the default batch size). Note that if result "
                     "spooling is disabled only a single row batch can be fetched at a "
                     "time regardless of the specified fetch_size.")
   parser.add_option("--http_cookie_names", dest="http_cookie_names",
                     default="impala.auth,impala.session.id",
                     help="A comma-separated list of HTTP cookie names that are supported "
                     "by the impala-shell. If a cookie with one of these names is "
```

### Comparing `impala_shell-4.3.0a3/impala_shell/Logging/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/Logging/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/DataSinks/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/DataSinks/ttypes.py`

 * *Files 3% similar despite different names*

```diff
@@ -356,14 +356,54 @@
     def __eq__(self, other):
         return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not (self == other)
 
 
+class TIcebergDeleteSink(object):
+
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('TIcebergDeleteSink')
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
 class TKuduTableSink(object):
     """
     Attributes:
      - referenced_columns
      - ignore_not_found_or_duplicate
      - kudu_txn_token
 
@@ -645,24 +685,26 @@
     """
     Attributes:
      - target_table_id
      - type
      - action
      - hdfs_table_sink
      - kudu_table_sink
+     - iceberg_delete_sink
 
     """
 
 
-    def __init__(self, target_table_id=None, type=None, action=None, hdfs_table_sink=None, kudu_table_sink=None,):
+    def __init__(self, target_table_id=None, type=None, action=None, hdfs_table_sink=None, kudu_table_sink=None, iceberg_delete_sink=None,):
         self.target_table_id = target_table_id
         self.type = type
         self.action = action
         self.hdfs_table_sink = hdfs_table_sink
         self.kudu_table_sink = kudu_table_sink
+        self.iceberg_delete_sink = iceberg_delete_sink
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
@@ -692,14 +734,20 @@
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.STRUCT:
                     self.kudu_table_sink = TKuduTableSink()
                     self.kudu_table_sink.read(iprot)
                 else:
                     iprot.skip(ftype)
+            elif fid == 6:
+                if ftype == TType.STRUCT:
+                    self.iceberg_delete_sink = TIcebergDeleteSink()
+                    self.iceberg_delete_sink.read(iprot)
+                else:
+                    iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
@@ -722,14 +770,18 @@
             oprot.writeFieldBegin('hdfs_table_sink', TType.STRUCT, 4)
             self.hdfs_table_sink.write(oprot)
             oprot.writeFieldEnd()
         if self.kudu_table_sink is not None:
             oprot.writeFieldBegin('kudu_table_sink', TType.STRUCT, 5)
             self.kudu_table_sink.write(oprot)
             oprot.writeFieldEnd()
+        if self.iceberg_delete_sink is not None:
+            oprot.writeFieldBegin('iceberg_delete_sink', TType.STRUCT, 6)
+            self.iceberg_delete_sink.write(oprot)
+            oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.target_table_id is None:
             raise TProtocolException(message='Required field target_table_id is unset!')
         if self.type is None:
@@ -927,14 +979,17 @@
     (6, TType.I64, 'write_id', None, None, ),  # 6
     (7, TType.I32, 'sorting_order', None, None, ),  # 7
     (8, TType.BOOL, 'is_result_sink', None, False, ),  # 8
     (9, TType.STRING, 'external_output_dir', None, None, ),  # 9
     (10, TType.I32, 'external_output_partition_depth', None, None, ),  # 10
     (11, TType.MAP, 'parquet_bloom_filter_col_info', (TType.STRING, None, TType.I64, None, False), None, ),  # 11
 )
+all_structs.append(TIcebergDeleteSink)
+TIcebergDeleteSink.thrift_spec = (
+)
 all_structs.append(TKuduTableSink)
 TKuduTableSink.thrift_spec = (
     None,  # 0
     (1, TType.LIST, 'referenced_columns', (TType.I32, None, False), None, ),  # 1
     (2, TType.BOOL, 'ignore_not_found_or_duplicate', None, None, ),  # 2
     (3, TType.STRING, 'kudu_txn_token', 'BINARY', None, ),  # 3
 )
@@ -957,14 +1012,15 @@
 TTableSink.thrift_spec = (
     None,  # 0
     (1, TType.I32, 'target_table_id', None, None, ),  # 1
     (2, TType.I32, 'type', None, None, ),  # 2
     (3, TType.I32, 'action', None, None, ),  # 3
     (4, TType.STRUCT, 'hdfs_table_sink', [THdfsTableSink, None], None, ),  # 4
     (5, TType.STRUCT, 'kudu_table_sink', [TKuduTableSink, None], None, ),  # 5
+    (6, TType.STRUCT, 'iceberg_delete_sink', [TIcebergDeleteSink, None], None, ),  # 6
 )
 all_structs.append(TDataSink)
 TDataSink.thrift_spec = (
     None,  # 0
     (1, TType.I32, 'type', None, None, ),  # 1
     (2, TType.STRUCT, 'stream_sink', [TDataStreamSink, None], None, ),  # 2
     (3, TType.STRUCT, 'table_sink', [TTableSink, None], None, ),  # 3
```

### Comparing `impala_shell-4.3.0a3/impala_shell/MetricDefs/constants.py` & `impala_shell-4.3.0a4/impala_shell/MetricDefs/constants.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/MetricDefs/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/MetricDefs/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/StatestoreService/StatestoreService.py` & `impala_shell-4.3.0a4/impala_shell/StatestoreService/StatestoreService.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/StatestoreService/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/StatestoreService/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/StatestoreService/StatestoreSubscriber.py` & `impala_shell-4.3.0a4/impala_shell/StatestoreService/StatestoreSubscriber.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/shell_output.py` & `impala_shell-4.3.0a4/impala_shell/shell_output.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/CatalogObjects/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/CatalogObjects/ttypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -3505,36 +3505,36 @@
     def __ne__(self, other):
         return not (self == other)
 
 
 class TIcebergPartitionSpec(object):
     """
     Attributes:
-     - partition_id
+     - spec_id
      - partition_fields
 
     """
 
 
-    def __init__(self, partition_id=None, partition_fields=None,):
-        self.partition_id = partition_id
+    def __init__(self, spec_id=None, partition_fields=None,):
+        self.spec_id = spec_id
         self.partition_fields = partition_fields
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.I32:
-                    self.partition_id = iprot.readI32()
+                    self.spec_id = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.partition_fields = []
                     (_etype184, _size181) = iprot.readListBegin()
                     for _i185 in range(_size181):
@@ -3550,31 +3550,31 @@
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('TIcebergPartitionSpec')
-        if self.partition_id is not None:
-            oprot.writeFieldBegin('partition_id', TType.I32, 1)
-            oprot.writeI32(self.partition_id)
+        if self.spec_id is not None:
+            oprot.writeFieldBegin('spec_id', TType.I32, 1)
+            oprot.writeI32(self.spec_id)
             oprot.writeFieldEnd()
         if self.partition_fields is not None:
             oprot.writeFieldBegin('partition_fields', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.partition_fields))
             for iter187 in self.partition_fields:
                 iter187.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
-        if self.partition_id is None:
-            raise TProtocolException(message='Required field partition_id is unset!')
+        if self.spec_id is None:
+            raise TProtocolException(message='Required field spec_id is unset!')
         return
 
     def __repr__(self):
         L = ['%s=%r' % (key, value)
              for key, value in self.__dict__.items()]
         return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
 
@@ -5305,15 +5305,15 @@
     (3, TType.STRING, 'orig_field_name', None, None, ),  # 3
     (4, TType.STRING, 'field_name', None, None, ),  # 4
     (5, TType.STRUCT, 'transform', [TIcebergPartitionTransform, None], None, ),  # 5
 )
 all_structs.append(TIcebergPartitionSpec)
 TIcebergPartitionSpec.thrift_spec = (
     None,  # 0
-    (1, TType.I32, 'partition_id', None, None, ),  # 1
+    (1, TType.I32, 'spec_id', None, None, ),  # 1
     (2, TType.LIST, 'partition_fields', (TType.STRUCT, [TIcebergPartitionField, None], False), None, ),  # 2
 )
 all_structs.append(TIcebergPartitionStats)
 TIcebergPartitionStats.thrift_spec = (
     None,  # 0
     (1, TType.I64, 'num_files', None, None, ),  # 1
     (2, TType.I64, 'num_rows', None, None, ),  # 2
```

### Comparing `impala_shell-4.3.0a3/impala_shell/NetworkTest/NetworkTestService.py` & `impala_shell-4.3.0a4/impala_shell/NetworkTest/NetworkTestService.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/NetworkTest/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/NetworkTest/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/CatalogService/CatalogService.py` & `impala_shell-4.3.0a4/impala_shell/CatalogService/CatalogService.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/CatalogService/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/CatalogService/ttypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -855,52 +855,71 @@
     def __ne__(self, other):
         return not (self == other)
 
 
 class TIcebergOperationParam(object):
     """
     Attributes:
+     - operation
      - spec_id
      - iceberg_data_files_fb
+     - iceberg_delete_files_fb
      - is_overwrite
      - initial_snapshot_id
 
     """
 
 
-    def __init__(self, spec_id=None, iceberg_data_files_fb=None, is_overwrite=False, initial_snapshot_id=None,):
+    def __init__(self, operation=None, spec_id=None, iceberg_data_files_fb=None, iceberg_delete_files_fb=None, is_overwrite=False, initial_snapshot_id=None,):
+        self.operation = operation
         self.spec_id = spec_id
         self.iceberg_data_files_fb = iceberg_data_files_fb
+        self.iceberg_delete_files_fb = iceberg_delete_files_fb
         self.is_overwrite = is_overwrite
         self.initial_snapshot_id = initial_snapshot_id
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
-            if fid == 1:
+            if fid == 5:
+                if ftype == TType.I32:
+                    self.operation = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 1:
                 if ftype == TType.I32:
                     self.spec_id = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.iceberg_data_files_fb = []
                     (_etype17, _size14) = iprot.readListBegin()
                     for _i18 in range(_size14):
                         _elem19 = iprot.readBinary()
                         self.iceberg_data_files_fb.append(_elem19)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
+            elif fid == 6:
+                if ftype == TType.LIST:
+                    self.iceberg_delete_files_fb = []
+                    (_etype23, _size20) = iprot.readListBegin()
+                    for _i24 in range(_size20):
+                        _elem25 = iprot.readBinary()
+                        self.iceberg_delete_files_fb.append(_elem25)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.BOOL:
                     self.is_overwrite = iprot.readBool()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.I64:
@@ -920,32 +939,43 @@
         if self.spec_id is not None:
             oprot.writeFieldBegin('spec_id', TType.I32, 1)
             oprot.writeI32(self.spec_id)
             oprot.writeFieldEnd()
         if self.iceberg_data_files_fb is not None:
             oprot.writeFieldBegin('iceberg_data_files_fb', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.iceberg_data_files_fb))
-            for iter20 in self.iceberg_data_files_fb:
-                oprot.writeBinary(iter20)
+            for iter26 in self.iceberg_data_files_fb:
+                oprot.writeBinary(iter26)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.is_overwrite is not None:
             oprot.writeFieldBegin('is_overwrite', TType.BOOL, 3)
             oprot.writeBool(self.is_overwrite)
             oprot.writeFieldEnd()
         if self.initial_snapshot_id is not None:
             oprot.writeFieldBegin('initial_snapshot_id', TType.I64, 4)
             oprot.writeI64(self.initial_snapshot_id)
             oprot.writeFieldEnd()
+        if self.operation is not None:
+            oprot.writeFieldBegin('operation', TType.I32, 5)
+            oprot.writeI32(self.operation)
+            oprot.writeFieldEnd()
+        if self.iceberg_delete_files_fb is not None:
+            oprot.writeFieldBegin('iceberg_delete_files_fb', TType.LIST, 6)
+            oprot.writeListBegin(TType.STRING, len(self.iceberg_delete_files_fb))
+            for iter27 in self.iceberg_delete_files_fb:
+                oprot.writeBinary(iter27)
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
-        if self.iceberg_data_files_fb is None:
-            raise TProtocolException(message='Required field iceberg_data_files_fb is unset!')
+        if self.operation is None:
+            raise TProtocolException(message='Required field operation is unset!')
         if self.is_overwrite is None:
             raise TProtocolException(message='Required field is_overwrite is unset!')
         return
 
     def __repr__(self):
         L = ['%s=%r' % (key, value)
              for key, value in self.__dict__.items()]
@@ -977,18 +1007,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.files = []
-                    (_etype24, _size21) = iprot.readListBegin()
-                    for _i25 in range(_size21):
-                        _elem26 = iprot.readString()
-                        self.files.append(_elem26)
+                    (_etype31, _size28) = iprot.readListBegin()
+                    for _i32 in range(_size28):
+                        _elem33 = iprot.readString()
+                        self.files.append(_elem33)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -997,16 +1027,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('TUpdatedPartition')
         if self.files is not None:
             oprot.writeFieldBegin('files', TType.LIST, 1)
             oprot.writeListBegin(TType.STRING, len(self.files))
-            for iter27 in self.files:
-                oprot.writeString(iter27)
+            for iter34 in self.files:
+                oprot.writeString(iter34)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.files is None:
@@ -1090,20 +1120,20 @@
                 if ftype == TType.STRING:
                     self.db_name = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.MAP:
                     self.updated_partitions = {}
-                    (_ktype29, _vtype30, _size28) = iprot.readMapBegin()
-                    for _i32 in range(_size28):
-                        _key33 = iprot.readString()
-                        _val34 = TUpdatedPartition()
-                        _val34.read(iprot)
-                        self.updated_partitions[_key33] = _val34
+                    (_ktype36, _vtype37, _size35) = iprot.readMapBegin()
+                    for _i39 in range(_size35):
+                        _key40 = iprot.readString()
+                        _val41 = TUpdatedPartition()
+                        _val41.read(iprot)
+                        self.updated_partitions[_key40] = _val41
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 7:
                 if ftype == TType.BOOL:
                     self.is_overwrite = iprot.readBool()
                 else:
@@ -1158,17 +1188,17 @@
         if self.db_name is not None:
             oprot.writeFieldBegin('db_name', TType.STRING, 5)
             oprot.writeString(self.db_name)
             oprot.writeFieldEnd()
         if self.updated_partitions is not None:
             oprot.writeFieldBegin('updated_partitions', TType.MAP, 6)
             oprot.writeMapBegin(TType.STRING, TType.STRUCT, len(self.updated_partitions))
-            for kiter35, viter36 in self.updated_partitions.items():
-                oprot.writeString(kiter35)
-                viter36.write(oprot)
+            for kiter42, viter43 in self.updated_partitions.items():
+                oprot.writeString(kiter42)
+                viter43.write(oprot)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.is_overwrite is not None:
             oprot.writeFieldBegin('is_overwrite', TType.BOOL, 7)
             oprot.writeBool(self.is_overwrite)
             oprot.writeFieldEnd()
         if self.transaction_id is not None:
@@ -1336,19 +1366,19 @@
                     self.table_name = CatalogObjects.ttypes.TTableName()
                     self.table_name.read(iprot)
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.LIST:
                     self.partition_spec = []
-                    (_etype40, _size37) = iprot.readListBegin()
-                    for _i41 in range(_size37):
-                        _elem42 = CatalogObjects.ttypes.TPartitionKeyValue()
-                        _elem42.read(iprot)
-                        self.partition_spec.append(_elem42)
+                    (_etype47, _size44) = iprot.readListBegin()
+                    for _i48 in range(_size44):
+                        _elem49 = CatalogObjects.ttypes.TPartitionKeyValue()
+                        _elem49.read(iprot)
+                        self.partition_spec.append(_elem49)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.STRING:
                     self.db_name = iprot.readString()
                 else:
@@ -1398,16 +1428,16 @@
         if self.table_name is not None:
             oprot.writeFieldBegin('table_name', TType.STRUCT, 4)
             self.table_name.write(oprot)
             oprot.writeFieldEnd()
         if self.partition_spec is not None:
             oprot.writeFieldBegin('partition_spec', TType.LIST, 5)
             oprot.writeListBegin(TType.STRUCT, len(self.partition_spec))
-            for iter43 in self.partition_spec:
-                iter43.write(oprot)
+            for iter50 in self.partition_spec:
+                iter50.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.db_name is not None:
             oprot.writeFieldBegin('db_name', TType.STRING, 6)
             oprot.writeString(self.db_name)
             oprot.writeFieldEnd()
         if self.sync_ddl is not None:
@@ -1619,19 +1649,19 @@
                     self.status = Status.ttypes.TStatus()
                     self.status.read(iprot)
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.functions = []
-                    (_etype47, _size44) = iprot.readListBegin()
-                    for _i48 in range(_size44):
-                        _elem49 = Types.ttypes.TFunction()
-                        _elem49.read(iprot)
-                        self.functions.append(_elem49)
+                    (_etype54, _size51) = iprot.readListBegin()
+                    for _i55 in range(_size51):
+                        _elem56 = Types.ttypes.TFunction()
+                        _elem56.read(iprot)
+                        self.functions.append(_elem56)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -1644,16 +1674,16 @@
         if self.status is not None:
             oprot.writeFieldBegin('status', TType.STRUCT, 1)
             self.status.write(oprot)
             oprot.writeFieldEnd()
         if self.functions is not None:
             oprot.writeFieldBegin('functions', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.functions))
-            for iter50 in self.functions:
-                iter50.write(oprot)
+            for iter57 in self.functions:
+                iter57.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -1746,18 +1776,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.db_names = []
-                    (_etype54, _size51) = iprot.readListBegin()
-                    for _i55 in range(_size51):
-                        _elem56 = iprot.readString()
-                        self.db_names.append(_elem56)
+                    (_etype61, _size58) = iprot.readListBegin()
+                    for _i62 in range(_size58):
+                        _elem63 = iprot.readString()
+                        self.db_names.append(_elem63)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -1766,16 +1796,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('TPartialCatalogInfo')
         if self.db_names is not None:
             oprot.writeFieldBegin('db_names', TType.LIST, 1)
             oprot.writeListBegin(TType.STRING, len(self.db_names))
-            for iter57 in self.db_names:
-                oprot.writeString(iter57)
+            for iter64 in self.db_names:
+                oprot.writeString(iter64)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -1840,18 +1870,18 @@
                 if ftype == TType.BOOL:
                     self.want_hms_table = iprot.readBool()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.partition_ids = []
-                    (_etype61, _size58) = iprot.readListBegin()
-                    for _i62 in range(_size58):
-                        _elem63 = iprot.readI64()
-                        self.partition_ids.append(_elem63)
+                    (_etype68, _size65) = iprot.readListBegin()
+                    for _i69 in range(_size65):
+                        _elem70 = iprot.readI64()
+                        self.partition_ids.append(_elem70)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.BOOL:
                     self.want_partition_names = iprot.readBool()
                 else:
@@ -1865,18 +1895,18 @@
                 if ftype == TType.BOOL:
                     self.want_partition_files = iprot.readBool()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.LIST:
                     self.want_stats_for_column_names = []
-                    (_etype67, _size64) = iprot.readListBegin()
-                    for _i68 in range(_size64):
-                        _elem69 = iprot.readString()
-                        self.want_stats_for_column_names.append(_elem69)
+                    (_etype74, _size71) = iprot.readListBegin()
+                    for _i75 in range(_size71):
+                        _elem76 = iprot.readString()
+                        self.want_stats_for_column_names.append(_elem76)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 7:
                 if ftype == TType.BOOL:
                     self.want_partition_stats = iprot.readBool()
                 else:
@@ -1925,16 +1955,16 @@
         if self.want_hms_table is not None:
             oprot.writeFieldBegin('want_hms_table', TType.BOOL, 1)
             oprot.writeBool(self.want_hms_table)
             oprot.writeFieldEnd()
         if self.partition_ids is not None:
             oprot.writeFieldBegin('partition_ids', TType.LIST, 2)
             oprot.writeListBegin(TType.I64, len(self.partition_ids))
-            for iter70 in self.partition_ids:
-                oprot.writeI64(iter70)
+            for iter77 in self.partition_ids:
+                oprot.writeI64(iter77)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.want_partition_names is not None:
             oprot.writeFieldBegin('want_partition_names', TType.BOOL, 3)
             oprot.writeBool(self.want_partition_names)
             oprot.writeFieldEnd()
         if self.want_partition_metadata is not None:
@@ -1944,16 +1974,16 @@
         if self.want_partition_files is not None:
             oprot.writeFieldBegin('want_partition_files', TType.BOOL, 5)
             oprot.writeBool(self.want_partition_files)
             oprot.writeFieldEnd()
         if self.want_stats_for_column_names is not None:
             oprot.writeFieldBegin('want_stats_for_column_names', TType.LIST, 6)
             oprot.writeListBegin(TType.STRING, len(self.want_stats_for_column_names))
-            for iter71 in self.want_stats_for_column_names:
-                oprot.writeString(iter71)
+            for iter78 in self.want_stats_for_column_names:
+                oprot.writeString(iter78)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.want_partition_stats is not None:
             oprot.writeFieldBegin('want_partition_stats', TType.BOOL, 7)
             oprot.writeBool(self.want_partition_stats)
             oprot.writeFieldEnd()
         if self.want_table_constraints is not None:
@@ -2059,41 +2089,41 @@
                     self.hms_partition = hive_metastore.ttypes.Partition()
                     self.hms_partition.read(iprot)
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.LIST:
                     self.file_descriptors = []
-                    (_etype75, _size72) = iprot.readListBegin()
-                    for _i76 in range(_size72):
-                        _elem77 = CatalogObjects.ttypes.THdfsFileDesc()
-                        _elem77.read(iprot)
-                        self.file_descriptors.append(_elem77)
+                    (_etype82, _size79) = iprot.readListBegin()
+                    for _i83 in range(_size79):
+                        _elem84 = CatalogObjects.ttypes.THdfsFileDesc()
+                        _elem84.read(iprot)
+                        self.file_descriptors.append(_elem84)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 8:
                 if ftype == TType.LIST:
                     self.insert_file_descriptors = []
-                    (_etype81, _size78) = iprot.readListBegin()
-                    for _i82 in range(_size78):
-                        _elem83 = CatalogObjects.ttypes.THdfsFileDesc()
-                        _elem83.read(iprot)
-                        self.insert_file_descriptors.append(_elem83)
+                    (_etype88, _size85) = iprot.readListBegin()
+                    for _i89 in range(_size85):
+                        _elem90 = CatalogObjects.ttypes.THdfsFileDesc()
+                        _elem90.read(iprot)
+                        self.insert_file_descriptors.append(_elem90)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 9:
                 if ftype == TType.LIST:
                     self.delete_file_descriptors = []
-                    (_etype87, _size84) = iprot.readListBegin()
-                    for _i88 in range(_size84):
-                        _elem89 = CatalogObjects.ttypes.THdfsFileDesc()
-                        _elem89.read(iprot)
-                        self.delete_file_descriptors.append(_elem89)
+                    (_etype94, _size91) = iprot.readListBegin()
+                    for _i95 in range(_size91):
+                        _elem96 = CatalogObjects.ttypes.THdfsFileDesc()
+                        _elem96.read(iprot)
+                        self.delete_file_descriptors.append(_elem96)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 14:
                 if ftype == TType.I64:
                     self.last_compaction_id = iprot.readI64()
                 else:
@@ -2112,19 +2142,19 @@
                 if ftype == TType.BOOL:
                     self.is_marked_cached = iprot.readBool()
                 else:
                     iprot.skip(ftype)
             elif fid == 10:
                 if ftype == TType.MAP:
                     self.hms_parameters = {}
-                    (_ktype91, _vtype92, _size90) = iprot.readMapBegin()
-                    for _i94 in range(_size90):
-                        _key95 = iprot.readString()
-                        _val96 = iprot.readString()
-                        self.hms_parameters[_key95] = _val96
+                    (_ktype98, _vtype99, _size97) = iprot.readMapBegin()
+                    for _i101 in range(_size97):
+                        _key102 = iprot.readString()
+                        _val103 = iprot.readString()
+                        self.hms_parameters[_key102] = _val103
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 11:
                 if ftype == TType.I64:
                     self.write_id = iprot.readI64()
                 else:
@@ -2162,16 +2192,16 @@
         if self.hms_partition is not None:
             oprot.writeFieldBegin('hms_partition', TType.STRUCT, 3)
             self.hms_partition.write(oprot)
             oprot.writeFieldEnd()
         if self.file_descriptors is not None:
             oprot.writeFieldBegin('file_descriptors', TType.LIST, 4)
             oprot.writeListBegin(TType.STRUCT, len(self.file_descriptors))
-            for iter97 in self.file_descriptors:
-                iter97.write(oprot)
+            for iter104 in self.file_descriptors:
+                iter104.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.partition_stats is not None:
             oprot.writeFieldBegin('partition_stats', TType.STRING, 5)
             oprot.writeBinary(self.partition_stats)
             oprot.writeFieldEnd()
         if self.has_incremental_stats is not None:
@@ -2181,31 +2211,31 @@
         if self.is_marked_cached is not None:
             oprot.writeFieldBegin('is_marked_cached', TType.BOOL, 7)
             oprot.writeBool(self.is_marked_cached)
             oprot.writeFieldEnd()
         if self.insert_file_descriptors is not None:
             oprot.writeFieldBegin('insert_file_descriptors', TType.LIST, 8)
             oprot.writeListBegin(TType.STRUCT, len(self.insert_file_descriptors))
-            for iter98 in self.insert_file_descriptors:
-                iter98.write(oprot)
+            for iter105 in self.insert_file_descriptors:
+                iter105.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.delete_file_descriptors is not None:
             oprot.writeFieldBegin('delete_file_descriptors', TType.LIST, 9)
             oprot.writeListBegin(TType.STRUCT, len(self.delete_file_descriptors))
-            for iter99 in self.delete_file_descriptors:
-                iter99.write(oprot)
+            for iter106 in self.delete_file_descriptors:
+                iter106.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.hms_parameters is not None:
             oprot.writeFieldBegin('hms_parameters', TType.MAP, 10)
             oprot.writeMapBegin(TType.STRING, TType.STRING, len(self.hms_parameters))
-            for kiter100, viter101 in self.hms_parameters.items():
-                oprot.writeString(kiter100)
-                oprot.writeString(viter101)
+            for kiter107, viter108 in self.hms_parameters.items():
+                oprot.writeString(kiter107)
+                oprot.writeString(viter108)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.write_id is not None:
             oprot.writeFieldBegin('write_id', TType.I64, 11)
             oprot.writeI64(self.write_id)
             oprot.writeFieldEnd()
         if self.hdfs_storage_descriptor is not None:
@@ -2285,57 +2315,57 @@
                     self.hms_table = hive_metastore.ttypes.Table()
                     self.hms_table.read(iprot)
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.partitions = []
-                    (_etype105, _size102) = iprot.readListBegin()
-                    for _i106 in range(_size102):
-                        _elem107 = TPartialPartitionInfo()
-                        _elem107.read(iprot)
-                        self.partitions.append(_elem107)
+                    (_etype112, _size109) = iprot.readListBegin()
+                    for _i113 in range(_size109):
+                        _elem114 = TPartialPartitionInfo()
+                        _elem114.read(iprot)
+                        self.partitions.append(_elem114)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.column_stats = []
-                    (_etype111, _size108) = iprot.readListBegin()
-                    for _i112 in range(_size108):
-                        _elem113 = hive_metastore.ttypes.ColumnStatisticsObj()
-                        _elem113.read(iprot)
-                        self.column_stats.append(_elem113)
+                    (_etype118, _size115) = iprot.readListBegin()
+                    for _i119 in range(_size115):
+                        _elem120 = hive_metastore.ttypes.ColumnStatisticsObj()
+                        _elem120.read(iprot)
+                        self.column_stats.append(_elem120)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.LIST:
                     self.virtual_columns = []
-                    (_etype117, _size114) = iprot.readListBegin()
-                    for _i118 in range(_size114):
-                        _elem119 = CatalogObjects.ttypes.TColumn()
-                        _elem119.read(iprot)
-                        self.virtual_columns.append(_elem119)
+                    (_etype124, _size121) = iprot.readListBegin()
+                    for _i125 in range(_size121):
+                        _elem126 = CatalogObjects.ttypes.TColumn()
+                        _elem126.read(iprot)
+                        self.virtual_columns.append(_elem126)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.I64:
                     self.storage_metadata_load_time_ns = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 8:
                 if ftype == TType.LIST:
                     self.network_addresses = []
-                    (_etype123, _size120) = iprot.readListBegin()
-                    for _i124 in range(_size120):
-                        _elem125 = Types.ttypes.TNetworkAddress()
-                        _elem125.read(iprot)
-                        self.network_addresses.append(_elem125)
+                    (_etype130, _size127) = iprot.readListBegin()
+                    for _i131 in range(_size127):
+                        _elem132 = Types.ttypes.TNetworkAddress()
+                        _elem132.read(iprot)
+                        self.network_addresses.append(_elem132)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 9:
                 if ftype == TType.STRUCT:
                     self.sql_constraints = SqlConstraints.ttypes.TSqlConstraints()
                     self.sql_constraints.read(iprot)
@@ -2351,18 +2381,18 @@
                 if ftype == TType.BOOL:
                     self.is_marked_cached = iprot.readBool()
                 else:
                     iprot.skip(ftype)
             elif fid == 12:
                 if ftype == TType.LIST:
                     self.partition_prefixes = []
-                    (_etype129, _size126) = iprot.readListBegin()
-                    for _i130 in range(_size126):
-                        _elem131 = iprot.readString()
-                        self.partition_prefixes.append(_elem131)
+                    (_etype136, _size133) = iprot.readListBegin()
+                    for _i137 in range(_size133):
+                        _elem138 = iprot.readString()
+                        self.partition_prefixes.append(_elem138)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 13:
                 if ftype == TType.STRUCT:
                     self.iceberg_table = CatalogObjects.ttypes.TIcebergTable()
                     self.iceberg_table.read(iprot)
@@ -2381,41 +2411,41 @@
         if self.hms_table is not None:
             oprot.writeFieldBegin('hms_table', TType.STRUCT, 1)
             self.hms_table.write(oprot)
             oprot.writeFieldEnd()
         if self.partitions is not None:
             oprot.writeFieldBegin('partitions', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.partitions))
-            for iter132 in self.partitions:
-                iter132.write(oprot)
+            for iter139 in self.partitions:
+                iter139.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.column_stats is not None:
             oprot.writeFieldBegin('column_stats', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.column_stats))
-            for iter133 in self.column_stats:
-                iter133.write(oprot)
+            for iter140 in self.column_stats:
+                iter140.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.virtual_columns is not None:
             oprot.writeFieldBegin('virtual_columns', TType.LIST, 4)
             oprot.writeListBegin(TType.STRUCT, len(self.virtual_columns))
-            for iter134 in self.virtual_columns:
-                iter134.write(oprot)
+            for iter141 in self.virtual_columns:
+                iter141.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.storage_metadata_load_time_ns is not None:
             oprot.writeFieldBegin('storage_metadata_load_time_ns', TType.I64, 5)
             oprot.writeI64(self.storage_metadata_load_time_ns)
             oprot.writeFieldEnd()
         if self.network_addresses is not None:
             oprot.writeFieldBegin('network_addresses', TType.LIST, 8)
             oprot.writeListBegin(TType.STRUCT, len(self.network_addresses))
-            for iter135 in self.network_addresses:
-                iter135.write(oprot)
+            for iter142 in self.network_addresses:
+                iter142.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.sql_constraints is not None:
             oprot.writeFieldBegin('sql_constraints', TType.STRUCT, 9)
             self.sql_constraints.write(oprot)
             oprot.writeFieldEnd()
         if self.valid_write_ids is not None:
@@ -2425,16 +2455,16 @@
         if self.is_marked_cached is not None:
             oprot.writeFieldBegin('is_marked_cached', TType.BOOL, 11)
             oprot.writeBool(self.is_marked_cached)
             oprot.writeFieldEnd()
         if self.partition_prefixes is not None:
             oprot.writeFieldBegin('partition_prefixes', TType.LIST, 12)
             oprot.writeListBegin(TType.STRING, len(self.partition_prefixes))
-            for iter136 in self.partition_prefixes:
-                oprot.writeString(iter136)
+            for iter143 in self.partition_prefixes:
+                oprot.writeString(iter143)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.iceberg_table is not None:
             oprot.writeFieldBegin('iceberg_table', TType.STRUCT, 13)
             self.iceberg_table.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -2655,29 +2685,29 @@
                     self.hms_database = hive_metastore.ttypes.Database()
                     self.hms_database.read(iprot)
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.brief_meta_of_tables = []
-                    (_etype140, _size137) = iprot.readListBegin()
-                    for _i141 in range(_size137):
-                        _elem142 = TBriefTableMeta()
-                        _elem142.read(iprot)
-                        self.brief_meta_of_tables.append(_elem142)
+                    (_etype147, _size144) = iprot.readListBegin()
+                    for _i148 in range(_size144):
+                        _elem149 = TBriefTableMeta()
+                        _elem149.read(iprot)
+                        self.brief_meta_of_tables.append(_elem149)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.function_names = []
-                    (_etype146, _size143) = iprot.readListBegin()
-                    for _i147 in range(_size143):
-                        _elem148 = iprot.readString()
-                        self.function_names.append(_elem148)
+                    (_etype153, _size150) = iprot.readListBegin()
+                    for _i154 in range(_size150):
+                        _elem155 = iprot.readString()
+                        self.function_names.append(_elem155)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -2690,23 +2720,23 @@
         if self.hms_database is not None:
             oprot.writeFieldBegin('hms_database', TType.STRUCT, 1)
             self.hms_database.write(oprot)
             oprot.writeFieldEnd()
         if self.brief_meta_of_tables is not None:
             oprot.writeFieldBegin('brief_meta_of_tables', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.brief_meta_of_tables))
-            for iter149 in self.brief_meta_of_tables:
-                iter149.write(oprot)
+            for iter156 in self.brief_meta_of_tables:
+                iter156.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.function_names is not None:
             oprot.writeFieldBegin('function_names', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.function_names))
-            for iter150 in self.function_names:
-                oprot.writeString(iter150)
+            for iter157 in self.function_names:
+                oprot.writeString(iter157)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -2897,19 +2927,19 @@
                     self.catalog_info = TPartialCatalogInfo()
                     self.catalog_info.read(iprot)
                 else:
                     iprot.skip(ftype)
             elif fid == 7:
                 if ftype == TType.LIST:
                     self.functions = []
-                    (_etype154, _size151) = iprot.readListBegin()
-                    for _i155 in range(_size151):
-                        _elem156 = Types.ttypes.TFunction()
-                        _elem156.read(iprot)
-                        self.functions.append(_elem156)
+                    (_etype161, _size158) = iprot.readListBegin()
+                    for _i162 in range(_size158):
+                        _elem163 = Types.ttypes.TFunction()
+                        _elem163.read(iprot)
+                        self.functions.append(_elem163)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -2942,16 +2972,16 @@
         if self.catalog_info is not None:
             oprot.writeFieldBegin('catalog_info', TType.STRUCT, 6)
             self.catalog_info.write(oprot)
             oprot.writeFieldEnd()
         if self.functions is not None:
             oprot.writeFieldBegin('functions', TType.LIST, 7)
             oprot.writeListBegin(TType.STRUCT, len(self.functions))
-            for iter157 in self.functions:
-                iter157.write(oprot)
+            for iter164 in self.functions:
+                iter164.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -3236,19 +3266,19 @@
                     self.status = Status.ttypes.TStatus()
                     self.status.read(iprot)
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.MAP:
                     self.partition_stats = {}
-                    (_ktype159, _vtype160, _size158) = iprot.readMapBegin()
-                    for _i162 in range(_size158):
-                        _key163 = iprot.readString()
-                        _val164 = iprot.readBinary()
-                        self.partition_stats[_key163] = _val164
+                    (_ktype166, _vtype167, _size165) = iprot.readMapBegin()
+                    for _i169 in range(_size165):
+                        _key170 = iprot.readString()
+                        _val171 = iprot.readBinary()
+                        self.partition_stats[_key170] = _val171
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -3261,17 +3291,17 @@
         if self.status is not None:
             oprot.writeFieldBegin('status', TType.STRUCT, 1)
             self.status.write(oprot)
             oprot.writeFieldEnd()
         if self.partition_stats is not None:
             oprot.writeFieldBegin('partition_stats', TType.MAP, 2)
             oprot.writeMapBegin(TType.STRING, TType.STRING, len(self.partition_stats))
-            for kiter165, viter166 in self.partition_stats.items():
-                oprot.writeString(kiter165)
-                oprot.writeBinary(viter166)
+            for kiter172, viter173 in self.partition_stats.items():
+                oprot.writeString(kiter172)
+                oprot.writeBinary(viter173)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -3322,19 +3352,19 @@
                     self.header = TCatalogServiceRequestHeader()
                     self.header.read(iprot)
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.object_descs = []
-                    (_etype170, _size167) = iprot.readListBegin()
-                    for _i171 in range(_size167):
-                        _elem172 = CatalogObjects.ttypes.TCatalogObject()
-                        _elem172.read(iprot)
-                        self.object_descs.append(_elem172)
+                    (_etype177, _size174) = iprot.readListBegin()
+                    for _i178 in range(_size174):
+                        _elem179 = CatalogObjects.ttypes.TCatalogObject()
+                        _elem179.read(iprot)
+                        self.object_descs.append(_elem179)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -3351,16 +3381,16 @@
         if self.header is not None:
             oprot.writeFieldBegin('header', TType.STRUCT, 2)
             self.header.write(oprot)
             oprot.writeFieldEnd()
         if self.object_descs is not None:
             oprot.writeFieldBegin('object_descs', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.object_descs))
-            for iter173 in self.object_descs:
-                iter173.write(oprot)
+            for iter180 in self.object_descs:
+                iter180.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.protocol_version is None:
@@ -3533,19 +3563,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.usages = []
-                    (_etype177, _size174) = iprot.readListBegin()
-                    for _i178 in range(_size174):
-                        _elem179 = TTableUsage()
-                        _elem179.read(iprot)
-                        self.usages.append(_elem179)
+                    (_etype184, _size181) = iprot.readListBegin()
+                    for _i185 in range(_size181):
+                        _elem186 = TTableUsage()
+                        _elem186.read(iprot)
+                        self.usages.append(_elem186)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -3554,16 +3584,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('TUpdateTableUsageRequest')
         if self.usages is not None:
             oprot.writeFieldBegin('usages', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.usages))
-            for iter180 in self.usages:
-                iter180.write(oprot)
+            for iter187 in self.usages:
+                iter187.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.usages is None:
@@ -3705,14 +3735,16 @@
 all_structs.append(TIcebergOperationParam)
 TIcebergOperationParam.thrift_spec = (
     None,  # 0
     (1, TType.I32, 'spec_id', None, None, ),  # 1
     (2, TType.LIST, 'iceberg_data_files_fb', (TType.STRING, 'BINARY', False), None, ),  # 2
     (3, TType.BOOL, 'is_overwrite', None, False, ),  # 3
     (4, TType.I64, 'initial_snapshot_id', None, None, ),  # 4
+    (5, TType.I32, 'operation', None, None, ),  # 5
+    (6, TType.LIST, 'iceberg_delete_files_fb', (TType.STRING, 'BINARY', False), None, ),  # 6
 )
 all_structs.append(TUpdatedPartition)
 TUpdatedPartition.thrift_spec = (
     None,  # 0
     (1, TType.LIST, 'files', (TType.STRING, None, False), None, ),  # 1
 )
 all_structs.append(TUpdateCatalogRequest)
```

### Comparing `impala_shell-4.3.0a3/impala_shell/parquet/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/parquet/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/__init__.py` & `impala_shell-4.3.0a4/impala_shell/__init__.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/ExecStats/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/ExecStats/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/LineageGraph/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/LineageGraph/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/thrift_printer.py` & `impala_shell-4.3.0a4/impala_shell/thrift_printer.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/Planner/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/Planner/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/ExternalDataSource/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/ExternalDataSource/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/CatalogInternalService/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/CatalogInternalService/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/Types/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/Types/ttypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,14 +128,29 @@
         "LOAD": 4,
         "SET": 5,
         "ADMIN_FN": 6,
         "TESTCASE": 7,
     }
 
 
+class TIcebergOperation(object):
+    INSERT = 0
+    DELETE = 1
+
+    _VALUES_TO_NAMES = {
+        0: "INSERT",
+        1: "DELETE",
+    }
+
+    _NAMES_TO_VALUES = {
+        "INSERT": 0,
+        "DELETE": 1,
+    }
+
+
 class TExplainLevel(object):
     MINIMAL = 0
     STANDARD = 1
     EXTENDED = 2
     VERBOSE = 3
 
     _VALUES_TO_NAMES = {
```

### Comparing `impala_shell-4.3.0a3/impala_shell/beeswaxd/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/beeswaxd/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/beeswaxd/BeeswaxService.py` & `impala_shell-4.3.0a4/impala_shell/beeswaxd/BeeswaxService.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/RuntimeProfile/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/RuntimeProfile/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/Query/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/Query/ttypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,22 +363,23 @@
      - codegen_cache_mode
      - stringify_map_keys
      - enable_trivial_query_for_admission
      - compute_processing_cost
      - processing_cost_min_threads
      - join_selectivity_correlation_factor
      - max_fragment_instances_per_node
+     - max_sort_run_size
 
     """
 
 
     def __init__(self, abort_on_error=False, max_errors=100, disable_codegen=False, batch_size=0, num_nodes=0, max_scan_range_length=0, num_scanner_threads=0, debug_action="", mem_limit=0, compression_codec=None, hbase_caching=0, hbase_cache_blocks=False, parquet_file_size=0, explain_level=1, sync_ddl=False, request_pool=None, disable_outermost_topn=False, query_timeout_s=0, buffer_pool_limit=None, appx_count_distinct=False, disable_unsafe_spills=False, exec_single_node_rows_threshold=100, optimize_partition_key_scans=False, replica_preference=0, schedule_random_replica=False, disable_streaming_preaggregations=False, runtime_filter_mode=2, runtime_bloom_filter_size=1048576, runtime_filter_wait_time_ms=0, disable_row_runtime_filtering=False, max_num_runtime_filters=10, parquet_annotate_strings_utf8=False, parquet_fallback_schema_resolution=0, mt_dop=None, s3_skip_insert_staging=True, runtime_filter_min_size=1048576, runtime_filter_max_size=16777216, prefetch_mode=1, strict_mode=False, scratch_limit=-1, enable_expr_rewrites=True, decimal_v2=True, parquet_dictionary_filtering=True, parquet_array_resolution=0, parquet_read_statistics=True, default_join_distribution_mode=0, disable_codegen_rows_threshold=50000, default_spillable_buffer_size=2097152, min_spillable_buffer_size=65536, max_row_size=524288, idle_session_timeout=None, compute_stats_min_sample_size=1073741824, exec_time_limit_s=0, shuffle_distinct_exprs=True, max_mem_estimate_for_admission=0, thread_reservation_limit=3000, thread_reservation_aggregate_limit=0, kudu_read_mode=0, allow_erasure_coded_files=True, timezone="", scan_bytes_limit=0, cpu_limit_s=0, topn_bytes_limit=536870912, client_identifier=None, resource_trace_ratio=float(0), num_remote_executor_candidates=3, num_rows_produced_limit=0, planner_testcase_mode=False, default_file_format=0, parquet_timestamp_type=0, parquet_read_page_index=True, parquet_write_page_index=True, parquet_page_row_count_limit=None, disable_hdfs_num_rows_estimate=False, default_hints_insert_statement=None, spool_query_results=True, default_transactional_type=0, statement_expression_limit=250000, max_statement_length_bytes=16777216, disable_data_cache=False, max_result_spooling_mem=104857600, max_spilled_result_spooling_mem=1073741824, disable_hbase_num_rows_estimate=False, fetch_rows_timeout_ms=10000, now_string="", parquet_object_store_split_size=268435456, mem_limit_executors=0, broadcast_bytes_limit=34359738368, preagg_bytes_limit=-1, enable_cnf_rewrites=True, max_cnf_exprs=200, kudu_snapshot_read_timestamp_micros=0, retry_failed_queries=False, enabled_runtime_filter_types=set((
         0,
         1,
-    )), async_codegen=False, enable_distinct_semi_join_optimization=True, sort_run_bytes_limit=-1, max_fs_writers=0, refresh_updated_hms_partitions=False, spool_all_results_for_retries=True, runtime_filter_error_rate=None, use_local_tz_for_unix_timestamp_conversions=False, convert_legacy_hive_parquet_utc_timestamps=False, enable_outer_join_to_inner_transformation=False, targeted_kudu_scan_range_length=-1, report_skew_limit=1.0000000000000000, optimize_simple_limit=False, use_dop_for_costing=True, broadcast_to_partition_factor=1.0000000000000000, join_rows_produced_limit=0, utf8_mode=False, analytic_rank_pushdown_threshold=1000, minmax_filter_threshold=0.0000000000000000, minmax_filtering_level=1, compute_column_minmax_stats=False, show_column_minmax_stats=False, default_ndv_scale=2, kudu_replica_selection=1, delete_stats_in_truncate=True, parquet_bloom_filtering=True, minmax_filter_sorted_columns=True, minmax_filter_fast_code_path=1, enable_kudu_transaction=False, minmax_filter_partition_columns=True, parquet_bloom_filter_write=1, orc_read_statistics=True, enable_async_ddl_execution=True, enable_async_load_data_execution=True, parquet_late_materialization_threshold=20, parquet_dictionary_runtime_filter_entry_limit=1024, abort_java_udf_on_exception=False, orc_async_read=True, runtime_in_list_filter_entry_limit=1024, enable_replan=True, test_replan=False, lock_max_wait_time_s=300, orc_schema_resolution=0, expand_complex_types=False, fallback_db_for_functions=None, disable_codegen_cache=False, codegen_cache_mode=0, stringify_map_keys=False, enable_trivial_query_for_admission=True, compute_processing_cost=False, processing_cost_min_threads=1, join_selectivity_correlation_factor=0.0000000000000000, max_fragment_instances_per_node=128,):
+    )), async_codegen=False, enable_distinct_semi_join_optimization=True, sort_run_bytes_limit=-1, max_fs_writers=0, refresh_updated_hms_partitions=False, spool_all_results_for_retries=True, runtime_filter_error_rate=None, use_local_tz_for_unix_timestamp_conversions=False, convert_legacy_hive_parquet_utc_timestamps=False, enable_outer_join_to_inner_transformation=False, targeted_kudu_scan_range_length=-1, report_skew_limit=1.0000000000000000, optimize_simple_limit=False, use_dop_for_costing=True, broadcast_to_partition_factor=1.0000000000000000, join_rows_produced_limit=0, utf8_mode=False, analytic_rank_pushdown_threshold=1000, minmax_filter_threshold=0.0000000000000000, minmax_filtering_level=1, compute_column_minmax_stats=False, show_column_minmax_stats=False, default_ndv_scale=2, kudu_replica_selection=1, delete_stats_in_truncate=True, parquet_bloom_filtering=True, minmax_filter_sorted_columns=True, minmax_filter_fast_code_path=1, enable_kudu_transaction=False, minmax_filter_partition_columns=True, parquet_bloom_filter_write=1, orc_read_statistics=True, enable_async_ddl_execution=True, enable_async_load_data_execution=True, parquet_late_materialization_threshold=20, parquet_dictionary_runtime_filter_entry_limit=1024, abort_java_udf_on_exception=False, orc_async_read=True, runtime_in_list_filter_entry_limit=1024, enable_replan=True, test_replan=False, lock_max_wait_time_s=300, orc_schema_resolution=0, expand_complex_types=False, fallback_db_for_functions=None, disable_codegen_cache=False, codegen_cache_mode=0, stringify_map_keys=False, enable_trivial_query_for_admission=True, compute_processing_cost=False, processing_cost_min_threads=1, join_selectivity_correlation_factor=0.0000000000000000, max_fragment_instances_per_node=128, max_sort_run_size=0,):
         self.abort_on_error = abort_on_error
         self.max_errors = max_errors
         self.disable_codegen = disable_codegen
         self.batch_size = batch_size
         self.num_nodes = num_nodes
         self.max_scan_range_length = max_scan_range_length
         self.num_scanner_threads = num_scanner_threads
@@ -523,14 +524,15 @@
         self.codegen_cache_mode = codegen_cache_mode
         self.stringify_map_keys = stringify_map_keys
         self.enable_trivial_query_for_admission = enable_trivial_query_for_admission
         self.compute_processing_cost = compute_processing_cost
         self.processing_cost_min_threads = processing_cost_min_threads
         self.join_selectivity_correlation_factor = join_selectivity_correlation_factor
         self.max_fragment_instances_per_node = max_fragment_instances_per_node
+        self.max_sort_run_size = max_sort_run_size
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
@@ -1274,14 +1276,19 @@
                 else:
                     iprot.skip(ftype)
             elif fid == 157:
                 if ftype == TType.I32:
                     self.max_fragment_instances_per_node = iprot.readI32()
                 else:
                     iprot.skip(ftype)
+            elif fid == 158:
+                if ftype == TType.I32:
+                    self.max_sort_run_size = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
@@ -1875,14 +1882,18 @@
             oprot.writeFieldBegin('join_selectivity_correlation_factor', TType.DOUBLE, 156)
             oprot.writeDouble(self.join_selectivity_correlation_factor)
             oprot.writeFieldEnd()
         if self.max_fragment_instances_per_node is not None:
             oprot.writeFieldBegin('max_fragment_instances_per_node', TType.I32, 157)
             oprot.writeI32(self.max_fragment_instances_per_node)
             oprot.writeFieldEnd()
+        if self.max_sort_run_size is not None:
+            oprot.writeFieldBegin('max_sort_run_size', TType.I32, 158)
+            oprot.writeI32(self.max_sort_run_size)
+            oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
 
     def __repr__(self):
@@ -2635,42 +2646,121 @@
     def __eq__(self, other):
         return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not (self == other)
 
 
+class TIcebergDmlFinalizeParams(object):
+    """
+    Attributes:
+     - operation
+     - spec_id
+     - initial_snapshot_id
+
+    """
+
+
+    def __init__(self, operation=None, spec_id=None, initial_snapshot_id=None,):
+        self.operation = operation
+        self.spec_id = spec_id
+        self.initial_snapshot_id = initial_snapshot_id
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.I32:
+                    self.operation = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.I32:
+                    self.spec_id = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.I64:
+                    self.initial_snapshot_id = iprot.readI64()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('TIcebergDmlFinalizeParams')
+        if self.operation is not None:
+            oprot.writeFieldBegin('operation', TType.I32, 1)
+            oprot.writeI32(self.operation)
+            oprot.writeFieldEnd()
+        if self.spec_id is not None:
+            oprot.writeFieldBegin('spec_id', TType.I32, 2)
+            oprot.writeI32(self.spec_id)
+            oprot.writeFieldEnd()
+        if self.initial_snapshot_id is not None:
+            oprot.writeFieldBegin('initial_snapshot_id', TType.I64, 3)
+            oprot.writeI64(self.initial_snapshot_id)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        if self.operation is None:
+            raise TProtocolException(message='Required field operation is unset!')
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
 class TFinalizeParams(object):
     """
     Attributes:
      - is_overwrite
      - hdfs_base_dir
      - table_name
      - table_db
      - staging_dir
      - table_id
      - transaction_id
      - write_id
-     - spec_id
-     - initial_snapshot_id
+     - iceberg_params
 
     """
 
 
-    def __init__(self, is_overwrite=None, hdfs_base_dir=None, table_name=None, table_db=None, staging_dir=None, table_id=None, transaction_id=None, write_id=None, spec_id=None, initial_snapshot_id=None,):
+    def __init__(self, is_overwrite=None, hdfs_base_dir=None, table_name=None, table_db=None, staging_dir=None, table_id=None, transaction_id=None, write_id=None, iceberg_params=None,):
         self.is_overwrite = is_overwrite
         self.hdfs_base_dir = hdfs_base_dir
         self.table_name = table_name
         self.table_db = table_db
         self.staging_dir = staging_dir
         self.table_id = table_id
         self.transaction_id = transaction_id
         self.write_id = write_id
-        self.spec_id = spec_id
-        self.initial_snapshot_id = initial_snapshot_id
+        self.iceberg_params = iceberg_params
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
@@ -2714,21 +2804,17 @@
                     iprot.skip(ftype)
             elif fid == 8:
                 if ftype == TType.I64:
                     self.write_id = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 9:
-                if ftype == TType.I32:
-                    self.spec_id = iprot.readI32()
-                else:
-                    iprot.skip(ftype)
-            elif fid == 10:
-                if ftype == TType.I64:
-                    self.initial_snapshot_id = iprot.readI64()
+                if ftype == TType.STRUCT:
+                    self.iceberg_params = TIcebergDmlFinalizeParams()
+                    self.iceberg_params.read(iprot)
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
@@ -2765,21 +2851,17 @@
             oprot.writeFieldBegin('transaction_id', TType.I64, 7)
             oprot.writeI64(self.transaction_id)
             oprot.writeFieldEnd()
         if self.write_id is not None:
             oprot.writeFieldBegin('write_id', TType.I64, 8)
             oprot.writeI64(self.write_id)
             oprot.writeFieldEnd()
-        if self.spec_id is not None:
-            oprot.writeFieldBegin('spec_id', TType.I32, 9)
-            oprot.writeI32(self.spec_id)
-            oprot.writeFieldEnd()
-        if self.initial_snapshot_id is not None:
-            oprot.writeFieldBegin('initial_snapshot_id', TType.I64, 10)
-            oprot.writeI64(self.initial_snapshot_id)
+        if self.iceberg_params is not None:
+            oprot.writeFieldBegin('iceberg_params', TType.STRUCT, 9)
+            self.iceberg_params.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.is_overwrite is None:
             raise TProtocolException(message='Required field is_overwrite is unset!')
@@ -3188,14 +3270,15 @@
     (151, TType.I32, 'codegen_cache_mode', None, 0, ),  # 151
     (152, TType.BOOL, 'stringify_map_keys', None, False, ),  # 152
     (153, TType.BOOL, 'enable_trivial_query_for_admission', None, True, ),  # 153
     (154, TType.BOOL, 'compute_processing_cost', None, False, ),  # 154
     (155, TType.I32, 'processing_cost_min_threads', None, 1, ),  # 155
     (156, TType.DOUBLE, 'join_selectivity_correlation_factor', None, 0.0000000000000000, ),  # 156
     (157, TType.I32, 'max_fragment_instances_per_node', None, 128, ),  # 157
+    (158, TType.I32, 'max_sort_run_size', None, 0, ),  # 158
 )
 all_structs.append(TClientRequest)
 TClientRequest.thrift_spec = (
     None,  # 0
     (1, TType.STRING, 'stmt', None, None, ),  # 1
     (2, TType.STRUCT, 'query_options', [TQueryOptions, None], None, ),  # 2
     (3, TType.STRING, 'redacted_stmt', None, None, ),  # 3
@@ -3247,27 +3330,33 @@
 )
 all_structs.append(TPlanExecInfo)
 TPlanExecInfo.thrift_spec = (
     None,  # 0
     (1, TType.LIST, 'fragments', (TType.STRUCT, [Planner.ttypes.TPlanFragment, None], False), None, ),  # 1
     (2, TType.MAP, 'per_node_scan_ranges', (TType.I32, None, TType.STRUCT, [Planner.ttypes.TScanRangeSpec, None], False), None, ),  # 2
 )
+all_structs.append(TIcebergDmlFinalizeParams)
+TIcebergDmlFinalizeParams.thrift_spec = (
+    None,  # 0
+    (1, TType.I32, 'operation', None, None, ),  # 1
+    (2, TType.I32, 'spec_id', None, None, ),  # 2
+    (3, TType.I64, 'initial_snapshot_id', None, None, ),  # 3
+)
 all_structs.append(TFinalizeParams)
 TFinalizeParams.thrift_spec = (
     None,  # 0
     (1, TType.BOOL, 'is_overwrite', None, None, ),  # 1
     (2, TType.STRING, 'hdfs_base_dir', None, None, ),  # 2
     (3, TType.STRING, 'table_name', None, None, ),  # 3
     (4, TType.STRING, 'table_db', None, None, ),  # 4
     (5, TType.STRING, 'staging_dir', None, None, ),  # 5
     (6, TType.I64, 'table_id', None, None, ),  # 6
     (7, TType.I64, 'transaction_id', None, None, ),  # 7
     (8, TType.I64, 'write_id', None, None, ),  # 8
-    (9, TType.I32, 'spec_id', None, None, ),  # 9
-    (10, TType.I64, 'initial_snapshot_id', None, None, ),  # 10
+    (9, TType.STRUCT, 'iceberg_params', [TIcebergDmlFinalizeParams, None], None, ),  # 9
 )
 all_structs.append(TQueryExecRequest)
 TQueryExecRequest.thrift_spec = (
     None,  # 0
     (1, TType.LIST, 'plan_exec_info', (TType.STRUCT, [TPlanExecInfo, None], False), None, ),  # 1
     (2, TType.STRUCT, 'result_set_metadata', [Results.ttypes.TResultSetMetadata, None], None, ),  # 2
     (3, TType.STRUCT, 'finalize_params', [TFinalizeParams, None], None, ),  # 3
```

### Comparing `impala_shell-4.3.0a3/impala_shell/ErrorCodes/constants.py` & `impala_shell-4.3.0a4/impala_shell/ErrorCodes/constants.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/ErrorCodes/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/ErrorCodes/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/Data/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/Data/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/TSSLSocketWithWildcardSAN.py` & `impala_shell-4.3.0a4/impala_shell/TSSLSocketWithWildcardSAN.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell/Results/ttypes.py` & `impala_shell-4.3.0a4/impala_shell/Results/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/impala_shell.egg-info/PKG-INFO` & `impala_shell-4.3.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: impala-shell
-Version: 4.3.0a3
+Name: impala_shell
+Version: 4.3.0a4
 Summary: Impala Shell
 Home-page: https://impala.apache.org/
 Author: Impala Dev
 Author-email: dev@impala.apache.org
 License: Apache Software License
 Description: # Impala Interactive Shell
```

### Comparing `impala_shell-4.3.0a3/impala_shell.egg-info/SOURCES.txt` & `impala_shell-4.3.0a4/impala_shell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/setup.py` & `impala_shell-4.3.0a4/setup.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a3/README.md` & `impala_shell-4.3.0a4/README.md`

 * *Files identical despite different names*

