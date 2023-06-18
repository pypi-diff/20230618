# Comparing `tmp/data_ecosystem_services-202306.0.8.tar.gz` & `tmp/data_ecosystem_services-202306.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_ecosystem_services-202306.0.8.tar", max compression
+gzip compressed data, was "data_ecosystem_services-202306.0.9.tar", max compression
```

## Comparing `data_ecosystem_services-202306.0.8.tar` & `data_ecosystem_services-202306.0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      857 2023-06-15 18:09:23.812189 data_ecosystem_services-202306.0.8/data_ecosystem_services/__main__.py
--rw-r--r--   0        0        0      973 2023-06-15 18:09:23.812189 data_ecosystem_services-202306.0.8/data_ecosystem_services/admin_service/__init__.py
--rw-r--r--   0        0        0     6323 2023-06-15 18:09:23.812189 data_ecosystem_services-202306.0.8/data_ecosystem_services/admin_service/environment_logging.py
--rw-r--r--   0        0        0     6901 2023-06-15 18:09:23.812189 data_ecosystem_services-202306.0.8/data_ecosystem_services/admin_service/environment_tracing.py
--rw-r--r--   0        0        0     1081 2023-06-15 18:09:23.812189 data_ecosystem_services-202306.0.8/data_ecosystem_services/alation_service/__init__.py
--rw-r--r--   0        0        0     1871 2023-06-15 18:09:23.812189 data_ecosystem_services-202306.0.8/data_ecosystem_services/alation_service/customfieldsendpoint.py
--rw-r--r--   0        0        0     2319 2023-06-15 18:09:23.812189 data_ecosystem_services-202306.0.8/data_ecosystem_services/alation_service/datasource.py
--rw-r--r--   0        0        0     1808 2023-06-15 18:09:23.812189 data_ecosystem_services-202306.0.8/data_ecosystem_services/alation_service/endpoint.py
--rw-r--r--   0        0        0     1666 2023-06-15 18:09:23.812189 data_ecosystem_services-202306.0.8/data_ecosystem_services/alation_service/idfinderendpoint.py
--rw-r--r--   0        0        0    12151 2023-06-15 18:09:23.812189 data_ecosystem_services-202306.0.8/data_ecosystem_services/alation_service/manifest.py
--rw-r--r--   0        0        0    17715 2023-06-15 18:09:23.812189 data_ecosystem_services-202306.0.8/data_ecosystem_services/alation_service/schema.py
--rw-r--r--   0        0        0     1224 2023-06-15 18:09:23.812189 data_ecosystem_services-202306.0.8/data_ecosystem_services/alation_service/tagsendpoint.py
--rw-r--r--   0        0        0    12309 2023-06-15 18:09:23.812189 data_ecosystem_services-202306.0.8/data_ecosystem_services/alation_service/tokenendpoint.py
--rw-r--r--   0        0        0      971 2023-06-15 18:09:23.812189 data_ecosystem_services-202306.0.8/data_ecosystem_services/az_storage_service/__init__.py
--rw-r--r--   0        0        0      750 2023-06-15 18:09:23.812189 data_ecosystem_services-202306.0.8/data_ecosystem_services/az_storage_service/az_storage_queue.py
--rw-r--r--   0        0        0      908 2023-06-15 18:09:23.816189 data_ecosystem_services-202306.0.8/data_ecosystem_services/security_service/__init__.py
--rw-r--r--   0        0        0    14614 2023-06-15 18:09:23.816189 data_ecosystem_services-202306.0.8/data_ecosystem_services/security_service/security_core.py
--rw-r--r--   0        0        0     1115 2023-06-15 18:09:23.816189 data_ecosystem_services-202306.0.8/data_ecosystem_services/self_service/__init__.py
--rw-r--r--   0        0        0    41371 2023-06-15 18:09:23.816189 data_ecosystem_services-202306.0.8/data_ecosystem_services/self_service/dataset_metadata.py
--rw-r--r--   0        0        0    32805 2023-06-15 18:09:23.816189 data_ecosystem_services-202306.0.8/data_ecosystem_services/self_service/environment_metadata.py
--rw-r--r--   0        0        0    36036 2023-06-15 18:09:23.816189 data_ecosystem_services-202306.0.8/data_ecosystem_services/self_service/job_metadata.py
--rw-r--r--   0        0        0     2250 2023-06-15 18:09:23.816189 data_ecosystem_services-202306.0.8/data_ecosystem_services/self_service/logging_metadata.py
--rw-r--r--   0        0        0    22304 2023-06-15 18:09:23.816189 data_ecosystem_services-202306.0.8/data_ecosystem_services/self_service/pipeline_metadata.py
--rw-r--r--   0        0        0     1538 2023-06-15 18:09:23.816189 data_ecosystem_services-202306.0.8/data_ecosystem_services/tech_environment_service/__init__.py
--rw-r--r--   0        0        0    33723 2023-06-15 18:09:23.816189 data_ecosystem_services-202306.0.8/data_ecosystem_services/tech_environment_service/dataset_convert.py
--rw-r--r--   0        0        0     8716 2023-06-15 18:09:23.816189 data_ecosystem_services-202306.0.8/data_ecosystem_services/tech_environment_service/dataset_core.py
--rw-r--r--   0        0        0    24955 2023-06-15 18:09:23.816189 data_ecosystem_services-202306.0.8/data_ecosystem_services/tech_environment_service/dataset_crud.py
--rw-r--r--   0        0        0     3777 2023-06-15 18:09:23.816189 data_ecosystem_services-202306.0.8/data_ecosystem_services/tech_environment_service/dataset_extract.py
--rw-r--r--   0        0        0     1997 2023-06-15 18:09:23.816189 data_ecosystem_services-202306.0.8/data_ecosystem_services/tech_environment_service/environment_core.py
--rw-r--r--   0        0        0    27546 2023-06-15 18:09:23.816189 data_ecosystem_services-202306.0.8/data_ecosystem_services/tech_environment_service/environment_file.py
--rw-r--r--   0        0        0     4589 2023-06-15 18:09:23.816189 data_ecosystem_services-202306.0.8/data_ecosystem_services/tech_environment_service/environment_spark.py
--rw-r--r--   0        0        0     4648 2023-06-15 18:09:23.816189 data_ecosystem_services-202306.0.8/data_ecosystem_services/tech_environment_service/job_core.py
--rw-r--r--   0        0        0    17224 2023-06-15 18:09:23.816189 data_ecosystem_services-202306.0.8/data_ecosystem_services/tech_environment_service/repo_core.py
--rw-r--r--   0        0        0    11357 2023-06-15 18:09:23.816189 data_ecosystem_services-202306.0.8/license.md
--rw-r--r--   0        0        0     3495 2023-06-15 18:12:35.854105 data_ecosystem_services-202306.0.8/pyproject.toml
--rw-r--r--   0        0        0    52126 2023-06-15 18:09:23.816189 data_ecosystem_services-202306.0.8/readme.md
--rw-r--r--   0        0        0      126 2023-06-15 18:09:23.816189 data_ecosystem_services-202306.0.8/setup.cfg
--rw-r--r--   0        0        0      127 2023-06-15 18:09:23.816189 data_ecosystem_services-202306.0.8/setup.py
--rw-r--r--   0        0        0    55057 1970-01-01 00:00:00.000000 data_ecosystem_services-202306.0.8/PKG-INFO
+-rw-r--r--   0        0        0      857 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/__main__.py
+-rw-r--r--   0        0        0      973 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/admin_service/__init__.py
+-rw-r--r--   0        0        0     6323 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/admin_service/environment_logging.py
+-rw-r--r--   0        0        0     6901 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/admin_service/environment_tracing.py
+-rw-r--r--   0        0        0     1130 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/__init__.py
+-rw-r--r--   0        0        0     1871 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/customfieldsendpoint.py
+-rw-r--r--   0        0        0     2319 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/datasource.py
+-rw-r--r--   0        0        0     1808 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/endpoint.py
+-rw-r--r--   0        0        0     1666 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/idfinderendpoint.py
+-rw-r--r--   0        0        0    12151 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/manifest.py
+-rw-r--r--   0        0        0    17906 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/schema.py
+-rw-r--r--   0        0        0     1224 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/tagsendpoint.py
+-rw-r--r--   0        0        0    12309 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/tokenendpoint.py
+-rw-r--r--   0        0        0      971 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/az_storage_service/__init__.py
+-rw-r--r--   0        0        0      920 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/az_storage_service/az_storage_queue.py
+-rw-r--r--   0        0        0      908 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/security_service/__init__.py
+-rw-r--r--   0        0        0    14614 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/security_service/security_core.py
+-rw-r--r--   0        0        0     1115 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/self_service/__init__.py
+-rw-r--r--   0        0        0    41371 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/self_service/dataset_metadata.py
+-rw-r--r--   0        0        0    32805 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/data_ecosystem_services/self_service/environment_metadata.py
+-rw-r--r--   0        0        0    36036 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/data_ecosystem_services/self_service/job_metadata.py
+-rw-r--r--   0        0        0     2250 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/data_ecosystem_services/self_service/logging_metadata.py
+-rw-r--r--   0        0        0    22304 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/data_ecosystem_services/self_service/pipeline_metadata.py
+-rw-r--r--   0        0        0     1538 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/__init__.py
+-rw-r--r--   0        0        0    33723 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/dataset_convert.py
+-rw-r--r--   0        0        0     8716 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/dataset_core.py
+-rw-r--r--   0        0        0    24955 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/dataset_crud.py
+-rw-r--r--   0        0        0     3777 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/dataset_extract.py
+-rw-r--r--   0        0        0     1997 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/environment_core.py
+-rw-r--r--   0        0        0    27546 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/environment_file.py
+-rw-r--r--   0        0        0     4589 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/environment_spark.py
+-rw-r--r--   0        0        0     4648 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/job_core.py
+-rw-r--r--   0        0        0    17224 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/repo_core.py
+-rw-r--r--   0        0        0    11357 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/license.md
+-rw-r--r--   0        0        0     3495 2023-06-16 11:57:40.714613 data_ecosystem_services-202306.0.9/pyproject.toml
+-rw-r--r--   0        0        0    52126 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/readme.md
+-rw-r--r--   0        0        0      126 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/setup.cfg
+-rw-r--r--   0        0        0      127 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/setup.py
+-rw-r--r--   0        0        0    55057 1970-01-01 00:00:00.000000 data_ecosystem_services-202306.0.9/PKG-INFO
```

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/__main__.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/__main__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/admin_service/__init__.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/admin_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/admin_service/environment_logging.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/admin_service/environment_logging.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/admin_service/environment_tracing.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/admin_service/environment_tracing.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/alation_service/__init__.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,9 +17,9 @@
     print("non windows")
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../../..")))
 
 from ..admin_service import environment_logging
 from ..admin_service import environment_tracing
-
+from ..az_storage_service import az_storage_queue
 __all__ = ["endpoint", "customfieldsendpoint", "tokenendpoint", "manifest", "tagsendpoint", "idfinderendpoint", "datasource", "schema"]
```

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/alation_service/customfieldsendpoint.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/customfieldsendpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/alation_service/datasource.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/datasource.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/alation_service/endpoint.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/endpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/alation_service/idfinderendpoint.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/idfinderendpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/alation_service/manifest.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/manifest.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/alation_service/schema.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from opentelemetry import trace
 
 from .tokenendpoint import TokenEndpoint
 from .customfieldsendpoint import CustomFieldsEndpoint
 from .tagsendpoint import TagsEndpoint
 from .idfinderendpoint import IdFinderEndpoint
 
+
 from data_ecosystem_services.admin_service import (
     environment_tracing as pade_env_tracing,
     environment_logging as pade_env_logging
 )
 
 
 class Schema:
@@ -169,14 +170,17 @@
         logger_singleton = pade_env_logging.LoggerSingleton.instance()
         logger = logger_singleton.get_logger()
         tracer_singleton = pade_env_tracing.TracerSingleton.instance()
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("upload_schema_manifest"):
 
+            queue_name =  config.get("json_metadata_az_storage_queue_name")
+            storage_queue = AzureStorageQueue(connection_string='your_connection_string', queue_name=queue_name)
+
             schema_location = config.get("edc_schema_location")
             environment = config.get("environment")
             alation_user_id = config.get("edc_alation_user_id")
 
             logger.info('Validating the manifest file at {0} with schema'.format(
                 manifest_file))
             metadata = manifest.validateManifest(manifest_file)
```

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/alation_service/tagsendpoint.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/tagsendpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/alation_service/tokenendpoint.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/tokenendpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/az_storage_service/__init__.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/az_storage_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/security_service/__init__.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/security_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/security_service/security_core.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/security_service/security_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/self_service/__init__.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/self_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/self_service/dataset_metadata.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/self_service/dataset_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/self_service/environment_metadata.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/self_service/environment_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/self_service/job_metadata.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/self_service/job_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/self_service/logging_metadata.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/self_service/logging_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/self_service/pipeline_metadata.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/self_service/pipeline_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/tech_environment_service/__init__.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/tech_environment_service/dataset_convert.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/dataset_convert.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/tech_environment_service/dataset_core.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/dataset_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/tech_environment_service/dataset_crud.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/dataset_crud.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/tech_environment_service/dataset_extract.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/dataset_extract.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/tech_environment_service/environment_core.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/environment_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/tech_environment_service/environment_file.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/environment_file.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/tech_environment_service/environment_spark.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/environment_spark.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/tech_environment_service/job_core.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/job_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/data_ecosystem_services/tech_environment_service/repo_core.py` & `data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/repo_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/license.md` & `data_ecosystem_services-202306.0.9/license.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/pyproject.toml` & `data_ecosystem_services-202306.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [project.urls]
 "Homepage" = "https://test.pypi.org/project/data-ecosystem-services"
 "Documentation" = "https://gift.readthedocs.io"
 "Repository" = "https://github.com/cdcent/data-ecosystem-services"
 
 [tool.poetry]
 name="data_ecosystem_services"
-version="202306.0.8"
+version="202306.0.9"
 description="Program Agnostic Data Ecosystem (PADE) - Python Services"
 authors=["John Bowyer <zfi4@cdc.gov>"]
 readme = "readme.md"
 license="Apache"
 homepage="https://test.pypi.org/project/data-ecosystem-services"
 repository="https://github.com/cdcent/data-ecosystem-services"
 classifiers=[
```

### Comparing `data_ecosystem_services-202306.0.8/readme.md` & `data_ecosystem_services-202306.0.9/readme.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.8/PKG-INFO` & `data_ecosystem_services-202306.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-ecosystem-services
-Version: 202306.0.8
+Version: 202306.0.9
 Summary: Program Agnostic Data Ecosystem (PADE) - Python Services
 Home-page: https://test.pypi.org/project/data-ecosystem-services
 License: Apache
 Author: John Bowyer
 Author-email: zfi4@cdc.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

