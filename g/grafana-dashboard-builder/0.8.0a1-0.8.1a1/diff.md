# Comparing `tmp/grafana-dashboard-builder-0.8.0a1.tar.gz` & `tmp/grafana-dashboard-builder-0.8.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grafana-dashboard-builder-0.8.0a1.tar", last modified: Sat Jun  4 18:10:22 2022, max compression
+gzip compressed data, was "grafana-dashboard-builder-0.8.1a1.tar", last modified: Sun Jun 18 19:46:33 2023, max compression
```

## Comparing `grafana-dashboard-builder-0.8.0a1.tar` & `grafana-dashboard-builder-0.8.1a1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 kuba      (1000) kuba      (1000)        0 2022-06-04 18:10:22.404060 grafana-dashboard-builder-0.8.0a1/
--rw-rw-r--   0 kuba      (1000) kuba      (1000)       40 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.0a1/AUTHORS
--rw-rw-r--   0 kuba      (1000) kuba      (1000)    11359 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.0a1/LICENSE
--rw-rw-r--   0 kuba      (1000) kuba      (1000)      135 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.0a1/NOTICE
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     1586 2022-06-04 18:10:22.404060 grafana-dashboard-builder-0.8.0a1/PKG-INFO
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     8844 2022-06-04 18:06:59.000000 grafana-dashboard-builder-0.8.0a1/README.md
-drwxrwxr-x   0 kuba      (1000) kuba      (1000)        0 2022-06-04 18:10:22.397060 grafana-dashboard-builder-0.8.0a1/bin/
--rwxrwxr-x   0 kuba      (1000) kuba      (1000)      824 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.0a1/bin/grafana_dashboard_builder.py
-drwxrwxr-x   0 kuba      (1000) kuba      (1000)        0 2022-06-04 18:10:22.398060 grafana-dashboard-builder-0.8.0a1/grafana_dashboard_builder.egg-info/
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     1586 2022-06-04 18:10:21.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboard_builder.egg-info/PKG-INFO
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     1213 2022-06-04 18:10:22.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboard_builder.egg-info/SOURCES.txt
--rw-rw-r--   0 kuba      (1000) kuba      (1000)        1 2022-06-04 18:10:21.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboard_builder.egg-info/dependency_links.txt
--rw-rw-r--   0 kuba      (1000) kuba      (1000)       74 2022-06-04 18:10:22.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboard_builder.egg-info/entry_points.txt
--rw-rw-r--   0 kuba      (1000) kuba      (1000)       48 2022-06-04 18:10:22.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboard_builder.egg-info/requires.txt
--rw-rw-r--   0 kuba      (1000) kuba      (1000)       19 2022-06-04 18:10:22.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboard_builder.egg-info/top_level.txt
-drwxrwxr-x   0 kuba      (1000) kuba      (1000)        0 2022-06-04 18:10:22.400060 grafana-dashboard-builder-0.8.0a1/grafana_dashboards/
--rw-rw-r--   0 kuba      (1000) kuba      (1000)      722 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboards/__init__.py
--rwxrwxr-x   0 kuba      (1000) kuba      (1000)     4467 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboards/cli.py
-drwxrwxr-x   0 kuba      (1000) kuba      (1000)        0 2022-06-04 18:10:22.401060 grafana-dashboard-builder-0.8.0a1/grafana_dashboards/client/
--rw-rw-r--   0 kuba      (1000) kuba      (1000)      722 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboards/client/__init__.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     4400 2022-06-04 18:06:59.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboards/client/connection.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     2093 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboards/client/elastic_search.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     3129 2022-06-04 18:06:59.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboards/client/grafana.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)      991 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboards/common.py
-drwxrwxr-x   0 kuba      (1000) kuba      (1000)        0 2022-06-04 18:10:22.404060 grafana-dashboard-builder-0.8.0a1/grafana_dashboards/components/
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     1132 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboards/components/__init__.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     1596 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboards/components/annotations.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     1881 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboards/components/axes.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     7070 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboards/components/base.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     2632 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboards/components/dashboards.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     2324 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboards/components/links.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)    13828 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboards/components/panels.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     1678 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboards/components/projects.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     1704 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboards/components/rows.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     2929 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboards/components/targets.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     6906 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboards/components/templates.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     1247 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboards/config.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     4028 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboards/context.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)      991 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboards/errors.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     3057 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboards/exporter.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     1450 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.0a1/grafana_dashboards/parser.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)       38 2022-06-04 18:10:22.404060 grafana-dashboard-builder-0.8.0a1/setup.cfg
--rwxrwxr-x   0 kuba      (1000) kuba      (1000)     3618 2022-06-04 18:06:59.000000 grafana-dashboard-builder-0.8.0a1/setup.py
+drwxr-xr-x   0 kuba      (1000) kuba      (1000)        0 2023-06-18 19:46:33.183141 grafana-dashboard-builder-0.8.1a1/
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)       40 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.1a1/AUTHORS
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)    11359 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.1a1/LICENSE
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)      135 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.1a1/NOTICE
+-rw-r--r--   0 kuba      (1000) kuba      (1000)     1587 2023-06-18 19:46:33.183141 grafana-dashboard-builder-0.8.1a1/PKG-INFO
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     8844 2022-06-04 18:06:59.000000 grafana-dashboard-builder-0.8.1a1/README.md
+drwxr-xr-x   0 kuba      (1000) kuba      (1000)        0 2023-06-18 19:46:33.181141 grafana-dashboard-builder-0.8.1a1/bin/
+-rwxrwxr-x   0 kuba      (1000) kuba      (1000)      824 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.1a1/bin/grafana_dashboard_builder.py
+drwxr-xr-x   0 kuba      (1000) kuba      (1000)        0 2023-06-18 19:46:33.182141 grafana-dashboard-builder-0.8.1a1/grafana_dashboard_builder.egg-info/
+-rw-r--r--   0 kuba      (1000) kuba      (1000)     1587 2023-06-18 19:46:33.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboard_builder.egg-info/PKG-INFO
+-rw-r--r--   0 kuba      (1000) kuba      (1000)     1213 2023-06-18 19:46:33.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboard_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 kuba      (1000) kuba      (1000)        1 2023-06-18 19:46:33.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboard_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 kuba      (1000) kuba      (1000)       74 2023-06-18 19:46:33.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboard_builder.egg-info/entry_points.txt
+-rw-r--r--   0 kuba      (1000) kuba      (1000)       48 2023-06-18 19:46:33.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboard_builder.egg-info/requires.txt
+-rw-r--r--   0 kuba      (1000) kuba      (1000)       19 2023-06-18 19:46:33.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboard_builder.egg-info/top_level.txt
+drwxr-xr-x   0 kuba      (1000) kuba      (1000)        0 2023-06-18 19:46:33.182141 grafana-dashboard-builder-0.8.1a1/grafana_dashboards/
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)      722 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboards/__init__.py
+-rwxrwxr-x   0 kuba      (1000) kuba      (1000)     4467 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboards/cli.py
+drwxr-xr-x   0 kuba      (1000) kuba      (1000)        0 2023-06-18 19:46:33.182141 grafana-dashboard-builder-0.8.1a1/grafana_dashboards/client/
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)      722 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboards/client/__init__.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     4400 2022-06-04 18:06:59.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboards/client/connection.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     2093 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboards/client/elastic_search.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     3129 2022-06-04 18:06:59.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboards/client/grafana.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)      991 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboards/common.py
+drwxr-xr-x   0 kuba      (1000) kuba      (1000)        0 2023-06-18 19:46:33.183141 grafana-dashboard-builder-0.8.1a1/grafana_dashboards/components/
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     1132 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboards/components/__init__.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     1596 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboards/components/annotations.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     1881 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboards/components/axes.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     7070 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboards/components/base.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     2632 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboards/components/dashboards.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     2324 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboards/components/links.py
+-rw-r--r--   0 kuba      (1000) kuba      (1000)    13889 2023-06-18 19:23:40.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboards/components/panels.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     1678 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboards/components/projects.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     1704 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboards/components/rows.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     2929 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboards/components/targets.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     6906 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboards/components/templates.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     1247 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboards/config.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     4028 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboards/context.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)      991 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboards/errors.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     3057 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboards/exporter.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     1450 2022-03-08 21:46:28.000000 grafana-dashboard-builder-0.8.1a1/grafana_dashboards/parser.py
+-rw-r--r--   0 kuba      (1000) kuba      (1000)       38 2023-06-18 19:46:33.183141 grafana-dashboard-builder-0.8.1a1/setup.cfg
+-rwxr-xr-x   0 kuba      (1000) kuba      (1000)     3619 2023-06-18 19:46:12.000000 grafana-dashboard-builder-0.8.1a1/setup.py
```

### Comparing `grafana-dashboard-builder-0.8.0a1/LICENSE` & `grafana-dashboard-builder-0.8.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `grafana-dashboard-builder-0.8.0a1/PKG-INFO` & `grafana-dashboard-builder-0.8.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grafana-dashboard-builder
-Version: 0.8.0a1
+Version: 0.8.1a1
 Summary: Generate Grafana dashboards with YAML
 Home-page: https://github.com/jakubplichta/grafana-dashboard-builder
 Author: Jakub Plichta
 Author-email: jakub.plichta@gmail.com
 License: Apache License, Version 2.0
 Keywords: grafana yaml graphite prometheus influxdb
 Classifier: Topic :: Utilities
@@ -12,19 +12,19 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 License-File: LICENSE
 License-File: NOTICE
 License-File: AUTHORS
 
 grafana-dashboard-builder is an open-source tool for easier creation of Grafana dashboards.
 It is written in Python and uses YAML descriptors for dashboard
```

### Comparing `grafana-dashboard-builder-0.8.0a1/README.md` & `grafana-dashboard-builder-0.8.1a1/README.md`

 * *Files identical despite different names*

### Comparing `grafana-dashboard-builder-0.8.0a1/bin/grafana_dashboard_builder.py` & `grafana-dashboard-builder-0.8.1a1/bin/grafana_dashboard_builder.py`

 * *Files identical despite different names*

### Comparing `grafana-dashboard-builder-0.8.0a1/grafana_dashboard_builder.egg-info/PKG-INFO` & `grafana-dashboard-builder-0.8.1a1/grafana_dashboard_builder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grafana-dashboard-builder
-Version: 0.8.0a1
+Version: 0.8.1a1
 Summary: Generate Grafana dashboards with YAML
 Home-page: https://github.com/jakubplichta/grafana-dashboard-builder
 Author: Jakub Plichta
 Author-email: jakub.plichta@gmail.com
 License: Apache License, Version 2.0
 Keywords: grafana yaml graphite prometheus influxdb
 Classifier: Topic :: Utilities
@@ -12,19 +12,19 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 License-File: LICENSE
 License-File: NOTICE
 License-File: AUTHORS
 
 grafana-dashboard-builder is an open-source tool for easier creation of Grafana dashboards.
 It is written in Python and uses YAML descriptors for dashboard
```

### Comparing `grafana-dashboard-builder-0.8.0a1/grafana_dashboard_builder.egg-info/SOURCES.txt` & `grafana-dashboard-builder-0.8.1a1/grafana_dashboard_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grafana-dashboard-builder-0.8.0a1/grafana_dashboards/__init__.py` & `grafana-dashboard-builder-0.8.1a1/grafana_dashboards/__init__.py`

 * *Files identical despite different names*

### Comparing `grafana-dashboard-builder-0.8.0a1/grafana_dashboards/cli.py` & `grafana-dashboard-builder-0.8.1a1/grafana_dashboards/cli.py`

 * *Files identical despite different names*

### Comparing `grafana-dashboard-builder-0.8.0a1/grafana_dashboards/client/__init__.py` & `grafana-dashboard-builder-0.8.1a1/grafana_dashboards/client/__init__.py`

 * *Files identical despite different names*

### Comparing `grafana-dashboard-builder-0.8.0a1/grafana_dashboards/client/connection.py` & `grafana-dashboard-builder-0.8.1a1/grafana_dashboards/client/connection.py`

 * *Files identical despite different names*

### Comparing `grafana-dashboard-builder-0.8.0a1/grafana_dashboards/client/elastic_search.py` & `grafana-dashboard-builder-0.8.1a1/grafana_dashboards/client/elastic_search.py`

 * *Files identical despite different names*

### Comparing `grafana-dashboard-builder-0.8.0a1/grafana_dashboards/client/grafana.py` & `grafana-dashboard-builder-0.8.1a1/grafana_dashboards/client/grafana.py`

 * *Files identical despite different names*

### Comparing `grafana-dashboard-builder-0.8.0a1/grafana_dashboards/common.py` & `grafana-dashboard-builder-0.8.1a1/grafana_dashboards/common.py`

 * *Files identical despite different names*

### Comparing `grafana-dashboard-builder-0.8.0a1/grafana_dashboards/components/__init__.py` & `grafana-dashboard-builder-0.8.1a1/grafana_dashboards/components/__init__.py`

 * *Files identical despite different names*

### Comparing `grafana-dashboard-builder-0.8.0a1/grafana_dashboards/components/annotations.py` & `grafana-dashboard-builder-0.8.1a1/grafana_dashboards/components/annotations.py`

 * *Files identical despite different names*

### Comparing `grafana-dashboard-builder-0.8.0a1/grafana_dashboards/components/axes.py` & `grafana-dashboard-builder-0.8.1a1/grafana_dashboards/components/axes.py`

 * *Files identical despite different names*

### Comparing `grafana-dashboard-builder-0.8.0a1/grafana_dashboards/components/base.py` & `grafana-dashboard-builder-0.8.1a1/grafana_dashboards/components/base.py`

 * *Files identical despite different names*

### Comparing `grafana-dashboard-builder-0.8.0a1/grafana_dashboards/components/dashboards.py` & `grafana-dashboard-builder-0.8.1a1/grafana_dashboards/components/dashboards.py`

 * *Files identical despite different names*

### Comparing `grafana-dashboard-builder-0.8.0a1/grafana_dashboards/components/links.py` & `grafana-dashboard-builder-0.8.1a1/grafana_dashboards/components/links.py`

 * *Files identical despite different names*

### Comparing `grafana-dashboard-builder-0.8.0a1/grafana_dashboards/components/panels.py` & `grafana-dashboard-builder-0.8.1a1/grafana_dashboards/components/panels.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,14 +77,15 @@
                 'hideZero': self.data['legend'].get('hideZero', False),
                 'sideWidth': self.data['legend'].get('sideWidth', None)
             }
         if 'tooltip' in self.data:
             panel_json['tooltip'] = {
                 'value_type': self.data['tooltip'].get('value_type', 'individual'),
                 'shared': self.data['tooltip'].get('shared', False),
+                'sort': self.data['tooltip'].get('sort', 0),
             }
         if 'seriesOverrides' in self.data:
             overrides = []
             for override in self.data['seriesOverrides']:
                 for alias, settings in override.items():
                     to_add = {'alias': alias}
                     to_add.update(settings)
```

### Comparing `grafana-dashboard-builder-0.8.0a1/grafana_dashboards/components/projects.py` & `grafana-dashboard-builder-0.8.1a1/grafana_dashboards/components/projects.py`

 * *Files identical despite different names*

### Comparing `grafana-dashboard-builder-0.8.0a1/grafana_dashboards/components/rows.py` & `grafana-dashboard-builder-0.8.1a1/grafana_dashboards/components/rows.py`

 * *Files identical despite different names*

### Comparing `grafana-dashboard-builder-0.8.0a1/grafana_dashboards/components/targets.py` & `grafana-dashboard-builder-0.8.1a1/grafana_dashboards/components/targets.py`

 * *Files identical despite different names*

### Comparing `grafana-dashboard-builder-0.8.0a1/grafana_dashboards/components/templates.py` & `grafana-dashboard-builder-0.8.1a1/grafana_dashboards/components/templates.py`

 * *Files identical despite different names*

### Comparing `grafana-dashboard-builder-0.8.0a1/grafana_dashboards/config.py` & `grafana-dashboard-builder-0.8.1a1/grafana_dashboards/config.py`

 * *Files identical despite different names*

### Comparing `grafana-dashboard-builder-0.8.0a1/grafana_dashboards/context.py` & `grafana-dashboard-builder-0.8.1a1/grafana_dashboards/context.py`

 * *Files identical despite different names*

### Comparing `grafana-dashboard-builder-0.8.0a1/grafana_dashboards/errors.py` & `grafana-dashboard-builder-0.8.1a1/grafana_dashboards/errors.py`

 * *Files identical despite different names*

### Comparing `grafana-dashboard-builder-0.8.0a1/grafana_dashboards/exporter.py` & `grafana-dashboard-builder-0.8.1a1/grafana_dashboards/exporter.py`

 * *Files identical despite different names*

### Comparing `grafana-dashboard-builder-0.8.0a1/grafana_dashboards/parser.py` & `grafana-dashboard-builder-0.8.1a1/grafana_dashboards/parser.py`

 * *Files identical despite different names*

### Comparing `grafana-dashboard-builder-0.8.0a1/setup.py` & `grafana-dashboard-builder-0.8.1a1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             args = shlex.split(self.tox_args)
         errno = tox.cmdline(args=args)
         sys.exit(errno)
 
 
 params = {
     'name': 'grafana-dashboard-builder',
-    'version': '0.8.0a1',
+    'version': '0.8.1a1',
     'packages': [
         'grafana_dashboards',
         'grafana_dashboards.client',
         'grafana_dashboards.components'
     ],
     'scripts': [
         'bin/grafana_dashboard_builder.py'
@@ -69,19 +69,19 @@
         'Intended Audience :: Developers',
         'Intended Audience :: Information Technology',
         'Intended Audience :: System Administrators',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     'keywords': 'grafana yaml graphite prometheus influxdb',
     'cmdclass': {'test': Tox},
     'tests_require': ['tox', 'mock'],
     'install_requires': ['PyYAML>=5.3', 'argparse', 'requests-kerberos', 'requests'],
     'python_requires': '>=3.6',
     'entry_points': {
```

