# Comparing `tmp/airflow_provider_anomaly_detection-0.0.8.tar.gz` & `tmp/airflow_provider_anomaly_detection-0.0.9.tar.gz`

## Comparing `airflow_provider_anomaly_detection-0.0.8.tar` & `airflow_provider_anomaly_detection-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,34 @@
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/.astro-registry.yaml
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/Makefile
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/requirements-dev.txt
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/requirements.txt
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/__init__.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/utils.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/example_dags/README.md
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/example_dags/__init__.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/example_dags/anomaly-detection-dag/README.md
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/example_dags/anomaly-detection-dag/__init__.py
--rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/example_dags/anomaly-detection-dag/anomaly-detection-dag.py
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/example_dags/anomaly-detection-dag/config/defaults.yaml
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/example_dags/anomaly-detection-dag/config/metrics_daily.yaml
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/example_dags/anomaly-detection-dag/config/metrics_hourly.yaml
--rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/example_dags/anomaly-detection-dag/sql/alert_status.sql
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/example_dags/anomaly-detection-dag/sql/preprocess.sql
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/example_dags/anomaly-detection-dag/sql/metrics/metrics_daily.sql
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/example_dags/anomaly-detection-dag/sql/metrics/metrics_hourly.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/operators/__init__.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/operators/metric_batch_alert_operator.py
--rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/operators/metric_batch_email_notify_operator.py
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/operators/metric_batch_ingest_operator.py
--rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/operators/metric_batch_score_operator.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/operators/metric_batch_train_operator.py
--rw-r--r--   0        0        0   222811 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/img/alert-chart-example.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/tests/operators/__init__.py
--rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/LICENSE
--rw-r--r--   0        0        0     5089 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/README.md
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/.astro-registry.yaml
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/Dockerfile
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/Makefile
+-rw-r--r--   0        0        0    10801 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/docker-compose.yaml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/requirements-dev.txt
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/requirements.txt
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/__init__.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/utils.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/example_dags/README.md
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/example_dags/__init__.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/example_dags/anomaly-detection-dag/README.md
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/example_dags/anomaly-detection-dag/__init__.py
+-rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/example_dags/anomaly-detection-dag/anomaly-detection-dag.py
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/example_dags/anomaly-detection-dag/config/defaults.yaml
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/example_dags/anomaly-detection-dag/config/metrics_daily.yaml
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/example_dags/anomaly-detection-dag/config/metrics_hourly.yaml
+-rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/example_dags/anomaly-detection-dag/sql/alert_status.sql
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/example_dags/anomaly-detection-dag/sql/preprocess.sql
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/example_dags/anomaly-detection-dag/sql/metrics/metrics_daily.sql
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/example_dags/anomaly-detection-dag/sql/metrics/metrics_hourly.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/operators/__init__.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/operators/metric_batch_alert_operator.py
+-rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/operators/metric_batch_email_notify_operator.py
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/operators/metric_batch_ingest_operator.py
+-rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/operators/metric_batch_score_operator.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/operators/metric_batch_train_operator.py
+-rw-r--r--   0        0        0   222811 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/img/alert-chart-example.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/tests/operators/__init__.py
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/LICENSE
+-rw-r--r--   0        0        0     5385 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/README.md
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5836 2020-02-02 00:00:00.000000 airflow_provider_anomaly_detection-0.0.9/PKG-INFO
```

### Comparing `airflow_provider_anomaly_detection-0.0.8/.astro-registry.yaml` & `airflow_provider_anomaly_detection-0.0.9/.astro-registry.yaml`

 * *Files identical despite different names*

### Comparing `airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/utils.py` & `airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 import yaml
 
 # TODO: clean these up they are horrible
 
 def get_metric_batch_configs(config_dir):
-    metric_batch_configs = [f'{config_dir}/{f}' for f in os.listdir(config_dir)]
+    metric_batch_configs = [f'{config_dir}{f}' for f in os.listdir(config_dir)]
     metric_batch_configs = [f for f in metric_batch_configs if f.endswith('.yaml') and not f.endswith('defaults.yaml')]
     return metric_batch_configs
 
 
 def get_metric_batch_config_defaults(config_dir):
-    metric_batch_configs_defaults = [f'{config_dir}/{f}' for f in os.listdir(config_dir)]
+    metric_batch_configs_defaults = [f'{config_dir}{f}' for f in os.listdir(config_dir)]
     metric_batch_configs_defaults = [f for f in metric_batch_configs_defaults if f.endswith('defaults.yaml')]
     for metric_batch_config_file in metric_batch_configs_defaults:
         with open(metric_batch_config_file) as yaml_file:
             metric_batch_config_defaults = yaml.safe_load(yaml_file)
     return metric_batch_config_defaults
```

### Comparing `airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/example_dags/__init__.py` & `airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/example_dags/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/example_dags/anomaly-detection-dag/README.md` & `airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/example_dags/anomaly-detection-dag/README.md`

 * *Files identical despite different names*

### Comparing `airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/example_dags/anomaly-detection-dag/__init__.py` & `airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/example_dags/anomaly-detection-dag/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/example_dags/anomaly-detection-dag/anomaly-detection-dag.py` & `airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/example_dags/anomaly-detection-dag/anomaly-detection-dag.py`

 * *Files identical despite different names*

### Comparing `airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/example_dags/anomaly-detection-dag/config/defaults.yaml` & `airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/example_dags/anomaly-detection-dag/config/defaults.yaml`

 * *Files identical despite different names*

### Comparing `airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/example_dags/anomaly-detection-dag/config/metrics_daily.yaml` & `airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/example_dags/anomaly-detection-dag/config/metrics_daily.yaml`

 * *Files identical despite different names*

### Comparing `airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/example_dags/anomaly-detection-dag/config/metrics_hourly.yaml` & `airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/example_dags/anomaly-detection-dag/config/metrics_hourly.yaml`

 * *Files identical despite different names*

### Comparing `airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/example_dags/anomaly-detection-dag/sql/alert_status.sql` & `airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/example_dags/anomaly-detection-dag/sql/alert_status.sql`

 * *Files identical despite different names*

### Comparing `airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/example_dags/anomaly-detection-dag/sql/preprocess.sql` & `airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/example_dags/anomaly-detection-dag/sql/preprocess.sql`

 * *Files identical despite different names*

### Comparing `airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/example_dags/anomaly-detection-dag/sql/metrics/metrics_daily.sql` & `airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/example_dags/anomaly-detection-dag/sql/metrics/metrics_daily.sql`

 * *Files identical despite different names*

### Comparing `airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/example_dags/anomaly-detection-dag/sql/metrics/metrics_hourly.sql` & `airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/example_dags/anomaly-detection-dag/sql/metrics/metrics_hourly.sql`

 * *Files identical despite different names*

### Comparing `airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/operators/metric_batch_alert_operator.py` & `airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/operators/metric_batch_alert_operator.py`

 * *Files identical despite different names*

### Comparing `airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/operators/metric_batch_email_notify_operator.py` & `airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/operators/metric_batch_email_notify_operator.py`

 * *Files identical despite different names*

### Comparing `airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/operators/metric_batch_ingest_operator.py` & `airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/operators/metric_batch_ingest_operator.py`

 * *Files identical despite different names*

### Comparing `airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/operators/metric_batch_score_operator.py` & `airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/operators/metric_batch_score_operator.py`

 * *Files identical despite different names*

### Comparing `airflow_provider_anomaly_detection-0.0.8/airflow_anomaly_detection/operators/metric_batch_train_operator.py` & `airflow_provider_anomaly_detection-0.0.9/airflow_anomaly_detection/operators/metric_batch_train_operator.py`

 * *Files identical despite different names*

### Comparing `airflow_provider_anomaly_detection-0.0.8/img/alert-chart-example.png` & `airflow_provider_anomaly_detection-0.0.9/img/alert-chart-example.png`

 * *Files identical despite different names*

### Comparing `airflow_provider_anomaly_detection-0.0.8/.gitignore` & `airflow_provider_anomaly_detection-0.0.9/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -136,7 +136,11 @@
 
 # pytype static type analyzer
 .pytype/
 
 # Cython debug symbols
 cython_debug/
 
+# airflow docker related
+logs
+dags
+plugins
```

### Comparing `airflow_provider_anomaly_detection-0.0.8/LICENSE` & `airflow_provider_anomaly_detection-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow_provider_anomaly_detection-0.0.8/README.md` & `airflow_provider_anomaly_detection-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 Example output of an alert. Horizontal bar chart used to show metric values over time. 
 Smoothed anomaly score is shown as a `%` and any flagged anomalies are marked with `*`.
 
 ### Alert Text (ascii art yay!)
 
 ```
-🤷 [some_metric_last1h] looks anomalous (2023-01-25 16:00:00) 🤷
+🔥 [some_metric_last1h] looks anomalous (2023-01-25 16:00:00) 🔥
 ```
 ```
 some_metric_last1h (2023-01-24 15:30:00 to 2023-01-25 16:00:00)
                                                                                        
 t=0   ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~             2,742.00    72% 2023-01-25 16:00:00
 t=-1  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~       3,165.00  * 81% 2023-01-25 15:30:00
 t=-2  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~  3,448.00  * 95% 2023-01-25 15:15:00
@@ -68,19 +68,28 @@
 ## Getting Started
 
 Check out the [example dag](https://github.com/andrewm4894/airflow-provider-anomaly-detection/tree/main/airflow_anomaly_detection/example_dags/anomaly-detection-dag/) to get started.
 
 ### Prerequisites
 
 * Currently only Google BiqQuery is supported as a data source. The plan is to add Snowflake next and then probably Redshift. PR's to add other data sources are very welcome (some refactoring probably needed).
+* Requirements are listed in [requirements.txt](requirements.txt).
 
 ### Installation
 
 Install from [PyPI](https://pypi.org/project/airflow-provider-anomaly-detection/) as usual.
 
 ```bash
 pip install airflow-provider-anomaly-detection
 ```
 
 ### Configuration
 
 See the example configuration files in the [example dag](https://github.com/andrewm4894/airflow-provider-anomaly-detection/tree/main/airflow_anomaly_detection/example_dags/anomaly-detection-dag/config/) folder. You can use a `defaults.yaml` or specific `<metric-batch>.yaml` for each metric batch if needed.
+
+### Docker
+
+YOu can use the docker compose file to spin up an airflow instance with the provider installed and the example dag available. This is useful for quickly trying it out locally.
+
+```bash
+docker-compose up
+```
```

### Comparing `airflow_provider_anomaly_detection-0.0.8/pyproject.toml` & `airflow_provider_anomaly_detection-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "airflow-provider-anomaly-detection"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="andrewm4894", email="andrewm4894@gmail.com" },
 ]
 description = "An airflow provider for anomaly detection."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `airflow_provider_anomaly_detection-0.0.8/PKG-INFO` & `airflow_provider_anomaly_detection-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-provider-anomaly-detection
-Version: 0.0.8
+Version: 0.0.9
 Summary: An airflow provider for anomaly detection.
 Project-URL: Homepage, https://github.com/andrewm4894/airflow-provider-anomaly-detection
 Project-URL: Bug Tracker, https://github.com/andrewm4894/airflow-provider-anomaly-detection/issues
 Author-email: andrewm4894 <andrewm4894@gmail.com>
 License-File: LICENSE
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
@@ -24,15 +24,15 @@
 
 Example output of an alert. Horizontal bar chart used to show metric values over time. 
 Smoothed anomaly score is shown as a `%` and any flagged anomalies are marked with `*`.
 
 ### Alert Text (ascii art yay!)
 
 ```
-🤷 [some_metric_last1h] looks anomalous (2023-01-25 16:00:00) 🤷
+🔥 [some_metric_last1h] looks anomalous (2023-01-25 16:00:00) 🔥
 ```
 ```
 some_metric_last1h (2023-01-24 15:30:00 to 2023-01-25 16:00:00)
                                                                                        
 t=0   ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~             2,742.00    72% 2023-01-25 16:00:00
 t=-1  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~       3,165.00  * 81% 2023-01-25 15:30:00
 t=-2  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~  3,448.00  * 95% 2023-01-25 15:15:00
@@ -81,19 +81,28 @@
 ## Getting Started
 
 Check out the [example dag](https://github.com/andrewm4894/airflow-provider-anomaly-detection/tree/main/airflow_anomaly_detection/example_dags/anomaly-detection-dag/) to get started.
 
 ### Prerequisites
 
 * Currently only Google BiqQuery is supported as a data source. The plan is to add Snowflake next and then probably Redshift. PR's to add other data sources are very welcome (some refactoring probably needed).
+* Requirements are listed in [requirements.txt](requirements.txt).
 
 ### Installation
 
 Install from [PyPI](https://pypi.org/project/airflow-provider-anomaly-detection/) as usual.
 
 ```bash
 pip install airflow-provider-anomaly-detection
 ```
 
 ### Configuration
 
 See the example configuration files in the [example dag](https://github.com/andrewm4894/airflow-provider-anomaly-detection/tree/main/airflow_anomaly_detection/example_dags/anomaly-detection-dag/config/) folder. You can use a `defaults.yaml` or specific `<metric-batch>.yaml` for each metric batch if needed.
+
+### Docker
+
+YOu can use the docker compose file to spin up an airflow instance with the provider installed and the example dag available. This is useful for quickly trying it out locally.
+
+```bash
+docker-compose up
+```
```

