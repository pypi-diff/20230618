# Comparing `tmp/ecowitt2mqtt-2023.6.0.tar.gz` & `tmp/ecowitt2mqtt-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecowitt2mqtt-2023.6.0.tar", max compression
+gzip compressed data, was "ecowitt2mqtt-2023.6.1.tar", max compression
```

## Comparing `ecowitt2mqtt-2023.6.0.tar` & `ecowitt2mqtt-2023.6.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1072 2023-06-17 17:57:01.588773 ecowitt2mqtt-2023.6.0/LICENSE
--rw-r--r--   0        0        0    31131 2023-06-17 17:57:01.588773 ecowitt2mqtt-2023.6.0/README.md
--rw-r--r--   0        0        0       39 2023-06-17 17:57:01.588773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/__init__.py
--rw-r--r--   0        0        0    13841 2023-06-17 17:57:01.588773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/__main__.py
--rw-r--r--   0        0        0       24 2023-06-17 17:57:01.588773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/backports/__init__.py
--rw-r--r--   0        0        0     1735 2023-06-17 17:57:01.588773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/backports/enum.py
--rw-r--r--   0        0        0    16441 2023-06-17 17:57:01.588773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/config.py
--rw-r--r--   0        0        0    10920 2023-06-17 17:57:01.588773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/const.py
--rw-r--r--   0        0        0     2308 2023-06-17 17:57:01.588773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/core.py
--rw-r--r--   0        0        0    12177 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/data.py
--rw-r--r--   0        0        0      107 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/errors.py
--rw-r--r--   0        0        0       22 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/__init__.py
--rw-r--r--   0        0        0     6598 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/__init__.py
--rw-r--r--   0        0        0     4891 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/battery.py
--rw-r--r--   0        0        0     2301 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/humidity.py
--rw-r--r--   0        0        0     2438 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/illuminance.py
--rw-r--r--   0        0        0     1018 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/leak.py
--rw-r--r--   0        0        0     2013 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/lightning.py
--rw-r--r--   0        0        0      744 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/pollution.py
--rw-r--r--   0        0        0     2737 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/precipitation.py
--rw-r--r--   0        0        0     1364 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/pressure.py
--rw-r--r--   0        0        0    21443 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/temperature.py
--rw-r--r--   0        0        0     1639 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/time.py
--rw-r--r--   0        0        0     4610 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/uv.py
--rw-r--r--   0        0        0     9593 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/wind.py
--rw-r--r--   0        0        0     2167 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/config_validation.py
--rw-r--r--   0        0        0     1665 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/device.py
--rw-r--r--   0        0        0     1800 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/publisher/__init__.py
--rw-r--r--   0        0        0      857 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/publisher/factory.py
--rw-r--r--   0        0        0    18157 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/publisher/hass.py
--rw-r--r--   0        0        0     1114 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/publisher/topic.py
--rw-r--r--   0        0        0     4973 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/server.py
--rw-r--r--   0        0        0      348 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/typing.py
--rw-r--r--   0        0        0     8058 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/runtime.py
--rw-r--r--   0        0        0     1414 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/util/__init__.py
--rw-r--r--   0        0        0     7934 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/util/meteo.py
--rw-r--r--   0        0        0    13191 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/util/unit_conversion.py
--rw-r--r--   0        0        0     4077 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/pyproject.toml
--rw-r--r--   0        0        0    32563 1970-01-01 00:00:00.000000 ecowitt2mqtt-2023.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/LICENSE
+-rw-r--r--   0        0        0    31131 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/README.md
+-rw-r--r--   0        0        0       39 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/__init__.py
+-rw-r--r--   0        0        0    13841 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/__main__.py
+-rw-r--r--   0        0        0       24 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/backports/__init__.py
+-rw-r--r--   0        0        0     1735 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/backports/enum.py
+-rw-r--r--   0        0        0    16441 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/config.py
+-rw-r--r--   0        0        0    10967 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/const.py
+-rw-r--r--   0        0        0     2308 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/core.py
+-rw-r--r--   0        0        0    12282 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/data.py
+-rw-r--r--   0        0        0      107 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/errors.py
+-rw-r--r--   0        0        0       22 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/__init__.py
+-rw-r--r--   0        0        0     6598 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/__init__.py
+-rw-r--r--   0        0        0     4891 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/battery.py
+-rw-r--r--   0        0        0     2301 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/humidity.py
+-rw-r--r--   0        0        0     2438 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/illuminance.py
+-rw-r--r--   0        0        0     1018 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/leak.py
+-rw-r--r--   0        0        0     2013 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/lightning.py
+-rw-r--r--   0        0        0      744 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/pollution.py
+-rw-r--r--   0        0        0     2737 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/precipitation.py
+-rw-r--r--   0        0        0     1364 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/pressure.py
+-rw-r--r--   0        0        0    21443 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/temperature.py
+-rw-r--r--   0        0        0     1639 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/time.py
+-rw-r--r--   0        0        0     4610 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/uv.py
+-rw-r--r--   0        0        0     9593 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/wind.py
+-rw-r--r--   0        0        0     2167 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/config_validation.py
+-rw-r--r--   0        0        0     1665 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/device.py
+-rw-r--r--   0        0        0     1800 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/publisher/__init__.py
+-rw-r--r--   0        0        0      857 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/publisher/factory.py
+-rw-r--r--   0        0        0    18330 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/publisher/hass.py
+-rw-r--r--   0        0        0     1114 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/publisher/topic.py
+-rw-r--r--   0        0        0     4973 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/server.py
+-rw-r--r--   0        0        0      348 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/typing.py
+-rw-r--r--   0        0        0     8058 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/runtime.py
+-rw-r--r--   0        0        0     1414 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/util/__init__.py
+-rw-r--r--   0        0        0     7934 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/util/meteo.py
+-rw-r--r--   0        0        0    13191 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/util/unit_conversion.py
+-rw-r--r--   0        0        0     4077 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/pyproject.toml
+-rw-r--r--   0        0        0    32563 1970-01-01 00:00:00.000000 ecowitt2mqtt-2023.6.1/PKG-INFO
```

### Comparing `ecowitt2mqtt-2023.6.0/LICENSE` & `ecowitt2mqtt-2023.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/README.md` & `ecowitt2mqtt-2023.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/__main__.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/__main__.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/backports/enum.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/backports/enum.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/config.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/config.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/const.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Define package constants."""
 import logging
 from typing import Final
 
 from ecowitt2mqtt.helpers.typing import UnitSystemType
 
-__version__ = "2023.06.0"
+__version__ = "2023.06.1"
 
 LOGGER = logging.getLogger(__package__)
 
 # Configuration keys:
 CONF_BATTERY_OVERRIDES: Final = "battery_override"
 CONF_CONFIG: Final = "config"
 CONF_DEFAULT_BATTERY_STRATEGY: Final = "default_battery_strategy"
@@ -93,14 +93,15 @@
 DATA_POINT_LIGHTNING_NUM: Final = "lightning_num"
 DATA_POINT_LIGHTNING_TIME: Final = "lightning_time"
 DATA_POINT_MONTHLY_RAIN: Final = "monthlyrain"
 DATA_POINT_RAIN_RATE: Final = "rainrate"
 DATA_POINT_RELATIVE_STRAIN_INDEX: Final = "relative_strain_index"
 DATA_POINT_RELATIVE_STRAIN_INDEX_PERCEPTION: Final = "relative_strain_index_perception"
 DATA_POINT_RUNTIME: Final = "runtime"
+DATA_POINT_R_RAIN_PIEZO: Final = "rrain_piezo"
 DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_1: Final = "safe_exposure_time_skin_type_1"
 DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_2: Final = "safe_exposure_time_skin_type_2"
 DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_3: Final = "safe_exposure_time_skin_type_3"
 DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_4: Final = "safe_exposure_time_skin_type_4"
 DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_5: Final = "safe_exposure_time_skin_type_5"
 DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_6: Final = "safe_exposure_time_skin_type_6"
 DATA_POINT_SIMMER_INDEX: Final = "simmerindex"
```

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/core.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/core.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/data.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     DATA_POINT_HUMIDITY,
     DATA_POINT_HUMIDITY_ABS,
     DATA_POINT_HUMIDITY_ABS_IN,
     DATA_POINT_INTERVAL,
     DATA_POINT_LIGHTNING,
     DATA_POINT_LIGHTNING_NUM,
     DATA_POINT_LIGHTNING_TIME,
+    DATA_POINT_R_RAIN_PIEZO,
     DATA_POINT_RAIN_RATE,
     DATA_POINT_RELATIVE_STRAIN_INDEX,
     DATA_POINT_RELATIVE_STRAIN_INDEX_PERCEPTION,
     DATA_POINT_RUNTIME,
     DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_1,
     DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_2,
     DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_3,
@@ -134,15 +135,15 @@
     DATA_POINT_GLOB_GUST: WindSpeedCalculator,
     DATA_POINT_GLOB_HUMIDITY: RelativeHumidityCalculator,
     DATA_POINT_GLOB_LEAK: LeakCalculator,
     DATA_POINT_GLOB_MOISTURE: RelativeHumidityCalculator,
     DATA_POINT_GLOB_PM10: PollutantCalculator,
     DATA_POINT_GLOB_PM25: PollutantCalculator,
     DATA_POINT_GLOB_RAIN: AccumulatedPrecipitationCalculator,
-    DATA_POINT_GLOB_RAIN_PIEZO: SimpleCalculator,
+    DATA_POINT_GLOB_RAIN_PIEZO: AccumulatedPrecipitationCalculator,
     DATA_POINT_GLOB_R_RAIN: PrecipitationRateCalculator,
     DATA_POINT_GLOB_TEMP: TemperatureCalculator,
     DATA_POINT_GLOB_TF: TemperatureCalculator,
     DATA_POINT_GLOB_VOLT: BatteryCalculator,
     DATA_POINT_GLOB_WETNESS: RelativeHumidityCalculator,
     DATA_POINT_GLOB_WIND: WindSpeedCalculator,
     DATA_POINT_GLOB_WINDDIR: WindDirCalculator,
@@ -157,14 +158,15 @@
     DATA_POINT_LIGHTNING: LightningStrikeDistanceCalculator,
     DATA_POINT_LIGHTNING_NUM: LightningStrikeCountCalculator,
     DATA_POINT_LIGHTNING_TIME: EpochCalculator,
     DATA_POINT_RAIN_RATE: PrecipitationRateCalculator,
     DATA_POINT_RELATIVE_STRAIN_INDEX: RsiCalculator,
     DATA_POINT_RELATIVE_STRAIN_INDEX_PERCEPTION: RsiPerceptionCalculator,
     DATA_POINT_RUNTIME: RuntimeCalculator,
+    DATA_POINT_R_RAIN_PIEZO: PrecipitationRateCalculator,
     DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_1: SafeExposureCalculator,
     DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_2: SafeExposureCalculator,
     DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_3: SafeExposureCalculator,
     DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_4: SafeExposureCalculator,
     DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_5: SafeExposureCalculator,
     DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_6: SafeExposureCalculator,
     DATA_POINT_SIMMER_INDEX: SimmerIndexCalculator,
```

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/__init__.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/__init__.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/battery.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/battery.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/humidity.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/humidity.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/illuminance.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/illuminance.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/leak.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/leak.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/lightning.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/lightning.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/pollution.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/pollution.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/precipitation.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/precipitation.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/pressure.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/pressure.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/temperature.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/temperature.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/time.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/time.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/uv.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/uv.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/wind.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/wind.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/config_validation.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/config_validation.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/device.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/device.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/publisher/__init__.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/publisher/__init__.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/publisher/factory.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/publisher/factory.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/publisher/hass.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/publisher/hass.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     DATA_POINT_HUMIDITY_ABS,
     DATA_POINT_HUMIDITY_ABS_IN,
     DATA_POINT_INTERVAL,
     DATA_POINT_LIGHTNING,
     DATA_POINT_LIGHTNING_NUM,
     DATA_POINT_LIGHTNING_TIME,
     DATA_POINT_MONTHLY_RAIN,
+    DATA_POINT_R_RAIN_PIEZO,
     DATA_POINT_RAIN_RATE,
     DATA_POINT_RELATIVE_STRAIN_INDEX,
     DATA_POINT_RELATIVE_STRAIN_INDEX_PERCEPTION,
     DATA_POINT_RUNTIME,
     DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_1,
     DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_2,
     DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_3,
@@ -238,15 +239,16 @@
         state_class=StateClass.MEASUREMENT,
     ),
     DATA_POINT_GLOB_RAIN: EntityDescription(
         icon="mdi:water",
         state_class=StateClass.MEASUREMENT,
     ),
     DATA_POINT_GLOB_RAIN_PIEZO: EntityDescription(
-        entity_category=EntityCategory.DIAGNOSTIC,
+        icon="mdi:water",
+        state_class=StateClass.MEASUREMENT,
     ),
     DATA_POINT_GLOB_TEMP: EntityDescription(
         device_class=DeviceClass.TEMPERATURE,
         state_class=StateClass.MEASUREMENT,
     ),
     DATA_POINT_GLOB_TF: EntityDescription(
         device_class=DeviceClass.TEMPERATURE,
@@ -301,14 +303,18 @@
     DATA_POINT_LIGHTNING_NUM: EntityDescription(
         icon="mdi:weather-lightning",
         state_class=StateClass.TOTAL,
     ),
     DATA_POINT_LIGHTNING_TIME: EntityDescription(
         device_class=DeviceClass.TIMESTAMP,
     ),
+    DATA_POINT_R_RAIN_PIEZO: EntityDescription(
+        icon="mdi:water",
+        state_class=StateClass.MEASUREMENT,
+    ),
     DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_1: EntityDescription(
         icon="mdi:timer",
         state_class=StateClass.MEASUREMENT,
     ),
     DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_2: EntityDescription(
         icon="mdi:timer",
         state_class=StateClass.MEASUREMENT,
```

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/publisher/topic.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/publisher/topic.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/server.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/server.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/runtime.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/runtime.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/util/__init__.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/util/meteo.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/util/meteo.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/util/unit_conversion.py` & `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/util/unit_conversion.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.0/pyproject.toml` & `ecowitt2mqtt-2023.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 warn_return_any = true
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
 [tool.poetry]
 name = "ecowitt2mqtt"
-version = "2023.06.0"
+version = "2023.06.1"
 description = "A small web server to send data from Ecowitt devices to an MQTT Broker"
 readme = "README.md"
 authors = ["Aaron Bach <bachya1208@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/bachya/ecowitt2mqtt"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `ecowitt2mqtt-2023.6.0/PKG-INFO` & `ecowitt2mqtt-2023.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecowitt2mqtt
-Version: 2023.6.0
+Version: 2023.6.1
 Summary: A small web server to send data from Ecowitt devices to an MQTT Broker
 Home-page: https://github.com/bachya/ecowitt2mqtt
 License: MIT
 Author: Aaron Bach
 Author-email: bachya1208@gmail.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ecowitt2mqtt Version: 2023.6.0 Summary: A small web
+Metadata-Version: 2.1 Name: ecowitt2mqtt Version: 2023.6.1 Summary: A small web
 server to send data from Ecowitt devices to an MQTT Broker Home-page: https://
 github.com/bachya/ecowitt2mqtt License: MIT Author: Aaron Bach Author-email:
 bachya1208@gmail.com Requires-Python: >=3.9.0,<4.0.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
```

