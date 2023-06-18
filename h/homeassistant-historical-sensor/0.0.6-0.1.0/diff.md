# Comparing `tmp/homeassistant-historical-sensor-0.0.6.tar.gz` & `tmp/homeassistant-historical-sensor-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homeassistant-historical-sensor-0.0.6.tar", last modified: Fri Jun 16 17:49:08 2023, max compression
+gzip compressed data, was "homeassistant-historical-sensor-0.1.0.tar", last modified: Sun Jun 18 09:42:11 2023, max compression
```

## Comparing `homeassistant-historical-sensor-0.0.6.tar` & `homeassistant-historical-sensor-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:08.788144 homeassistant-historical-sensor-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-16 17:49:08.788144 homeassistant-historical-sensor-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-16 17:48:57.000000 homeassistant-historical-sensor-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:08.788144 homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor/
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-16 17:48:57.000000 homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-16 17:48:57.000000 homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)    14167 2023-06-16 17:48:57.000000 homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-16 17:48:57.000000 homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-16 17:48:57.000000 homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:08.788144 homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-16 17:49:08.000000 homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-16 17:49:08.000000 homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:49:08.000000 homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 17:49:08.000000 homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-16 17:48:57.000000 homeassistant-historical-sensor-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-16 17:49:08.788144 homeassistant-historical-sensor-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:42:11.587929 homeassistant-historical-sensor-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-18 09:42:11.587929 homeassistant-historical-sensor-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-18 09:41:55.000000 homeassistant-historical-sensor-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:42:11.587929 homeassistant-historical-sensor-0.1.0/homeassistant_historical_sensor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-18 09:41:55.000000 homeassistant-historical-sensor-0.1.0/homeassistant_historical_sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-18 09:41:55.000000 homeassistant-historical-sensor-0.1.0/homeassistant_historical_sensor/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-06-18 09:41:55.000000 homeassistant-historical-sensor-0.1.0/homeassistant_historical_sensor/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-18 09:41:55.000000 homeassistant-historical-sensor-0.1.0/homeassistant_historical_sensor/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-18 09:41:55.000000 homeassistant-historical-sensor-0.1.0/homeassistant_historical_sensor/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:42:11.587929 homeassistant-historical-sensor-0.1.0/homeassistant_historical_sensor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-18 09:42:11.000000 homeassistant-historical-sensor-0.1.0/homeassistant_historical_sensor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-18 09:42:11.000000 homeassistant-historical-sensor-0.1.0/homeassistant_historical_sensor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 09:42:11.000000 homeassistant-historical-sensor-0.1.0/homeassistant_historical_sensor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-18 09:42:11.000000 homeassistant-historical-sensor-0.1.0/homeassistant_historical_sensor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-18 09:41:55.000000 homeassistant-historical-sensor-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-18 09:42:11.591929 homeassistant-historical-sensor-0.1.0/setup.cfg
```

### Comparing `homeassistant-historical-sensor-0.0.6/PKG-INFO` & `homeassistant-historical-sensor-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeassistant-historical-sensor
-Version: 0.0.6
+Version: 0.1.0
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
-Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 0.0.6
+Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 0.1.0
 Summary: Historical sensors for HomeAssistant Home-page: https://github.com/
 ldotlopez/ha-historical-sensor Author: Luis LÃ³pez Author-email:
 luis@cuarentaydos.com Project-URL: Repository, https://github.com/ldotlopez/ha-
 historical-sensor/ Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-
 historical-sensor/issues Requires-Python: >=3.9 Description-Content-Type: text/
 markdown # Historical sensors for Home Assistant ![](icon-64.png)  ![GitHub
 Release (latest SemVer including pre-releases)](https://img.shields.io/github/
```

### Comparing `homeassistant-historical-sensor-0.0.6/README.md` & `homeassistant-historical-sensor-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor/__init__.py` & `homeassistant-historical-sensor-0.1.0/homeassistant_historical_sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor/patches.py` & `homeassistant-historical-sensor-0.1.0/homeassistant_historical_sensor/patches.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor/sensor.py` & `homeassistant-historical-sensor-0.1.0/homeassistant_historical_sensor/sensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -344,18 +344,15 @@
             statistic_id=self.statatistic_id,
             unit_of_measurement=self.unit_of_measurement,
         )
 
         return metadata
 
     async def async_calculate_statistic_data(
-        self,
-        hist_states: List[HistoricalState],
-        *,
-        latest: Optional[StatisticsRow] = None,
+        self, hist_states: List[HistoricalState], *, latest: Optional[dict]
     ) -> List[StatisticData]:
         raise NotImplementedError()
 
 
 class PollUpdateMixin(HistoricalSensor):
     """PollUpdateMixin for simulate poll update model
```

### Comparing `homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor/state.py` & `homeassistant-historical-sensor-0.1.0/homeassistant_historical_sensor/state.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor/util.py` & `homeassistant-historical-sensor-0.1.0/homeassistant_historical_sensor/util.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor.egg-info/PKG-INFO` & `homeassistant-historical-sensor-0.1.0/homeassistant_historical_sensor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeassistant-historical-sensor
-Version: 0.0.6
+Version: 0.1.0
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
-Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 0.0.6
+Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 0.1.0
 Summary: Historical sensors for HomeAssistant Home-page: https://github.com/
 ldotlopez/ha-historical-sensor Author: Luis LÃ³pez Author-email:
 luis@cuarentaydos.com Project-URL: Repository, https://github.com/ldotlopez/ha-
 historical-sensor/ Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-
 historical-sensor/issues Requires-Python: >=3.9 Description-Content-Type: text/
 markdown # Historical sensors for Home Assistant ![](icon-64.png)  ![GitHub
 Release (latest SemVer including pre-releases)](https://img.shields.io/github/
```

### Comparing `homeassistant-historical-sensor-0.0.6/setup.cfg` & `homeassistant-historical-sensor-0.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = homeassistant-historical-sensor
-version = 0.0.6
+version = 0.1.0
 author = Luis López
 author_email = luis@cuarentaydos.com
 description = Historical sensors for HomeAssistant
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ldotlopez/ha-historical-sensor
 project_urls =
```

