# Comparing `tmp/homeassistant-historical-sensor-0.1.0a0.tar.gz` & `tmp/homeassistant-historical-sensor-1.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homeassistant-historical-sensor-0.1.0a0.tar", last modified: Sun Jun 18 15:29:39 2023, max compression
+gzip compressed data, was "homeassistant-historical-sensor-1.0.0a0.tar", last modified: Sun Jun 18 15:36:02 2023, max compression
```

## Comparing `homeassistant-historical-sensor-0.1.0a0.tar` & `homeassistant-historical-sensor-1.0.0a0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:29:39.022164 homeassistant-historical-sensor-0.1.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-18 15:29:39.022164 homeassistant-historical-sensor-0.1.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-18 15:29:27.000000 homeassistant-historical-sensor-0.1.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:29:39.018164 homeassistant-historical-sensor-0.1.0a0/homeassistant_historical_sensor/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-18 15:29:27.000000 homeassistant-historical-sensor-0.1.0a0/homeassistant_historical_sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-18 15:29:27.000000 homeassistant-historical-sensor-0.1.0a0/homeassistant_historical_sensor/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-06-18 15:29:27.000000 homeassistant-historical-sensor-0.1.0a0/homeassistant_historical_sensor/recorderutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    13737 2023-06-18 15:29:27.000000 homeassistant-historical-sensor-0.1.0a0/homeassistant_historical_sensor/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-18 15:29:27.000000 homeassistant-historical-sensor-0.1.0a0/homeassistant_historical_sensor/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:29:39.018164 homeassistant-historical-sensor-0.1.0a0/homeassistant_historical_sensor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-18 15:29:39.000000 homeassistant-historical-sensor-0.1.0a0/homeassistant_historical_sensor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-18 15:29:39.000000 homeassistant-historical-sensor-0.1.0a0/homeassistant_historical_sensor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 15:29:39.000000 homeassistant-historical-sensor-0.1.0a0/homeassistant_historical_sensor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-18 15:29:39.000000 homeassistant-historical-sensor-0.1.0a0/homeassistant_historical_sensor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-18 15:29:27.000000 homeassistant-historical-sensor-0.1.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-18 15:29:39.022164 homeassistant-historical-sensor-0.1.0a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:36:02.220721 homeassistant-historical-sensor-1.0.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-18 15:36:02.220721 homeassistant-historical-sensor-1.0.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-18 15:35:51.000000 homeassistant-historical-sensor-1.0.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:36:02.220721 homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-18 15:35:51.000000 homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-18 15:35:51.000000 homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-06-18 15:35:51.000000 homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor/recorderutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13737 2023-06-18 15:35:51.000000 homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-18 15:35:51.000000 homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:36:02.220721 homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-18 15:36:02.000000 homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-18 15:36:02.000000 homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 15:36:02.000000 homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-18 15:36:02.000000 homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-18 15:35:51.000000 homeassistant-historical-sensor-1.0.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-18 15:36:02.224722 homeassistant-historical-sensor-1.0.0a0/setup.cfg
```

### Comparing `homeassistant-historical-sensor-0.1.0a0/PKG-INFO` & `homeassistant-historical-sensor-1.0.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeassistant-historical-sensor
-Version: 0.1.0a0
+Version: 1.0.0a0
 Summary: Historical sensors for HomeAssistant
 Home-page: https://github.com/ldotlopez/ha-historical-sensor
 Author: Luis López
 Author-email: luis@cuarentaydos.com
 Project-URL: Repository, https://github.com/ldotlopez/ha-historical-sensor/
 Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-historical-sensor/issues
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 0.1.0a0
+Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 1.0.0a0
 Summary: Historical sensors for HomeAssistant Home-page: https://github.com/
 ldotlopez/ha-historical-sensor Author: Luis LÃ³pez Author-email:
 luis@cuarentaydos.com Project-URL: Repository, https://github.com/ldotlopez/ha-
 historical-sensor/ Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-
 historical-sensor/issues Requires-Python: >=3.9 Description-Content-Type: text/
 markdown # Historical sensors for Home Assistant ![](icon-64.png)  ![GitHub
 Release (latest SemVer including pre-releases)](https://img.shields.io/github/
```

### Comparing `homeassistant-historical-sensor-0.1.0a0/README.md` & `homeassistant-historical-sensor-1.0.0a0/README.md`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-0.1.0a0/homeassistant_historical_sensor/__init__.py` & `homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-0.1.0a0/homeassistant_historical_sensor/patches.py` & `homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor/patches.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-0.1.0a0/homeassistant_historical_sensor/recorderutil.py` & `homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor/recorderutil.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-0.1.0a0/homeassistant_historical_sensor/sensor.py` & `homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor/sensor.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-0.1.0a0/homeassistant_historical_sensor/state.py` & `homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor/state.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-0.1.0a0/homeassistant_historical_sensor.egg-info/PKG-INFO` & `homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeassistant-historical-sensor
-Version: 0.1.0a0
+Version: 1.0.0a0
 Summary: Historical sensors for HomeAssistant
 Home-page: https://github.com/ldotlopez/ha-historical-sensor
 Author: Luis López
 Author-email: luis@cuarentaydos.com
 Project-URL: Repository, https://github.com/ldotlopez/ha-historical-sensor/
 Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-historical-sensor/issues
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 0.1.0a0
+Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 1.0.0a0
 Summary: Historical sensors for HomeAssistant Home-page: https://github.com/
 ldotlopez/ha-historical-sensor Author: Luis LÃ³pez Author-email:
 luis@cuarentaydos.com Project-URL: Repository, https://github.com/ldotlopez/ha-
 historical-sensor/ Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-
 historical-sensor/issues Requires-Python: >=3.9 Description-Content-Type: text/
 markdown # Historical sensors for Home Assistant ![](icon-64.png)  ![GitHub
 Release (latest SemVer including pre-releases)](https://img.shields.io/github/
```

### Comparing `homeassistant-historical-sensor-0.1.0a0/setup.cfg` & `homeassistant-historical-sensor-1.0.0a0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = homeassistant-historical-sensor
-version = 0.1.0a0
+version = 1.0.0a0
 author = Luis López
 author_email = luis@cuarentaydos.com
 description = Historical sensors for HomeAssistant
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ldotlopez/ha-historical-sensor
 project_urls =
```

