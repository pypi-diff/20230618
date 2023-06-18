# Comparing `tmp/SenseLink-2.1.0.tar.gz` & `tmp/SenseLink-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SenseLink-2.1.0.tar", last modified: Sat May  6 20:20:36 2023, max compression
+gzip compressed data, was "SenseLink-2.2.0.tar", last modified: Sat Jun 17 23:59:54 2023, max compression
```

## Comparing `SenseLink-2.1.0.tar` & `SenseLink-2.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:20:36.299939 SenseLink-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-06 20:20:23.000000 SenseLink-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-05-06 20:20:36.299939 SenseLink-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-05-06 20:20:23.000000 SenseLink-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:20:36.295939 SenseLink-2.1.0/SenseLink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-05-06 20:20:36.000000 SenseLink-2.1.0/SenseLink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-06 20:20:36.000000 SenseLink-2.1.0/SenseLink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 20:20:36.000000 SenseLink-2.1.0/SenseLink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-06 20:20:36.000000 SenseLink-2.1.0/SenseLink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 20:20:36.000000 SenseLink-2.1.0/SenseLink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-06 20:20:23.000000 SenseLink-2.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:20:36.295939 SenseLink-2.1.0/senselink/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-06 20:20:23.000000 SenseLink-2.1.0/senselink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-06 20:20:23.000000 SenseLink-2.1.0/senselink/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-06 20:20:23.000000 SenseLink-2.1.0/senselink/data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:20:36.295939 SenseLink-2.1.0/senselink/homeassistant/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-06 20:20:23.000000 SenseLink-2.1.0/senselink/homeassistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-06 20:20:23.000000 SenseLink-2.1.0/senselink/homeassistant/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-05-06 20:20:23.000000 SenseLink-2.1.0/senselink/homeassistant/ha_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-05-06 20:20:23.000000 SenseLink-2.1.0/senselink/homeassistant/ha_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:20:36.299939 SenseLink-2.1.0/senselink/mqtt/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-06 20:20:23.000000 SenseLink-2.1.0/senselink/mqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-06 20:20:23.000000 SenseLink-2.1.0/senselink/mqtt/mqtt_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-05-06 20:20:23.000000 SenseLink-2.1.0/senselink/mqtt/mqtt_data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-06 20:20:23.000000 SenseLink-2.1.0/senselink/mqtt/mqtt_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-05-06 20:20:23.000000 SenseLink-2.1.0/senselink/plug_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    12260 2023-05-06 20:20:23.000000 SenseLink-2.1.0/senselink/senselink.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-06 20:20:23.000000 SenseLink-2.1.0/senselink/tplink_encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 20:20:36.299939 SenseLink-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-06 20:20:23.000000 SenseLink-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:59:54.331796 SenseLink-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-17 23:59:41.000000 SenseLink-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-06-17 23:59:54.331796 SenseLink-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-06-17 23:59:41.000000 SenseLink-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:59:54.331796 SenseLink-2.2.0/SenseLink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-06-17 23:59:54.000000 SenseLink-2.2.0/SenseLink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-17 23:59:54.000000 SenseLink-2.2.0/SenseLink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 23:59:54.000000 SenseLink-2.2.0/SenseLink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-17 23:59:54.000000 SenseLink-2.2.0/SenseLink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-17 23:59:54.000000 SenseLink-2.2.0/SenseLink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-17 23:59:41.000000 SenseLink-2.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:59:54.331796 SenseLink-2.2.0/senselink/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-17 23:59:41.000000 SenseLink-2.2.0/senselink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-17 23:59:41.000000 SenseLink-2.2.0/senselink/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-17 23:59:41.000000 SenseLink-2.2.0/senselink/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-06-17 23:59:41.000000 SenseLink-2.2.0/senselink/data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:59:54.331796 SenseLink-2.2.0/senselink/homeassistant/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 23:59:41.000000 SenseLink-2.2.0/senselink/homeassistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-06-17 23:59:41.000000 SenseLink-2.2.0/senselink/homeassistant/ha_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-06-17 23:59:41.000000 SenseLink-2.2.0/senselink/homeassistant/ha_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:59:54.331796 SenseLink-2.2.0/senselink/mqtt/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-17 23:59:41.000000 SenseLink-2.2.0/senselink/mqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-17 23:59:41.000000 SenseLink-2.2.0/senselink/mqtt/mqtt_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-06-17 23:59:41.000000 SenseLink-2.2.0/senselink/mqtt/mqtt_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-17 23:59:41.000000 SenseLink-2.2.0/senselink/mqtt/mqtt_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-06-17 23:59:41.000000 SenseLink-2.2.0/senselink/plug_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11669 2023-06-17 23:59:41.000000 SenseLink-2.2.0/senselink/senselink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-17 23:59:41.000000 SenseLink-2.2.0/senselink/tplink_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 23:59:54.331796 SenseLink-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-17 23:59:41.000000 SenseLink-2.2.0/setup.py
```

### Comparing `SenseLink-2.1.0/LICENSE` & `SenseLink-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SenseLink-2.1.0/PKG-INFO` & `SenseLink-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SenseLink
-Version: 2.1.0
+Version: 2.2.0
 Summary: A tool to create virtual smart plugs and inform a Sense Home Energy Monitor about usage in your home
 Home-page: https://github.com/cbpowell/SenseLink
 Author: Charles Powell
 Author-email: cbpowell@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `SenseLink-2.1.0/README.md` & `SenseLink-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `SenseLink-2.1.0/SenseLink.egg-info/PKG-INFO` & `SenseLink-2.2.0/SenseLink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SenseLink
-Version: 2.1.0
+Version: 2.2.0
 Summary: A tool to create virtual smart plugs and inform a Sense Home Energy Monitor about usage in your home
 Home-page: https://github.com/cbpowell/SenseLink
 Author: Charles Powell
 Author-email: cbpowell@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `SenseLink-2.1.0/SenseLink.egg-info/SOURCES.txt` & `SenseLink-2.2.0/SenseLink.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 SenseLink.egg-info/PKG-INFO
 SenseLink.egg-info/SOURCES.txt
 SenseLink.egg-info/dependency_links.txt
 SenseLink.egg-info/requires.txt
 SenseLink.egg-info/top_level.txt
 senselink/__init__.py
 senselink/__main__.py
+senselink/common.py
 senselink/data_source.py
 senselink/plug_instance.py
 senselink/senselink.py
 senselink/tplink_encryption.py
 senselink/homeassistant/__init__.py
-senselink/homeassistant/common.py
 senselink/homeassistant/ha_controller.py
 senselink/homeassistant/ha_data_source.py
 senselink/mqtt/__init__.py
 senselink/mqtt/mqtt_controller.py
 senselink/mqtt/mqtt_data_source.py
 senselink/mqtt/mqtt_listener.py
```

### Comparing `SenseLink-2.1.0/senselink/__main__.py` & `SenseLink-2.2.0/senselink/__main__.py`

 * *Files identical despite different names*

### Comparing `SenseLink-2.1.0/senselink/data_source.py` & `SenseLink-2.2.0/senselink/data_source.py`

 * *Files identical despite different names*

### Comparing `SenseLink-2.1.0/senselink/homeassistant/ha_controller.py` & `SenseLink-2.2.0/senselink/homeassistant/ha_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import websockets
 import json
 from socket import gaierror
-from .common import *
+from senselink.common import *
 
 
 class HAController:
     ws = None
     event_rq_id = 1
     bulk_rq_id = 2
     data_sources = []
```

### Comparing `SenseLink-2.1.0/senselink/homeassistant/ha_data_source.py` & `SenseLink-2.2.0/senselink/homeassistant/ha_data_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright 2022, Charles Powell
 from math import isclose
 
 from senselink.data_source import DataSource
-from .common import *
 from .ha_controller import *
 
 # Independently set WS logger
 wslogger = logging.getLogger('websockets')
 wslogger.setLevel(logging.WARNING)
```

### Comparing `SenseLink-2.1.0/senselink/mqtt/mqtt_controller.py` & `SenseLink-2.2.0/senselink/mqtt/mqtt_controller.py`

 * *Files identical despite different names*

### Comparing `SenseLink-2.1.0/senselink/mqtt/mqtt_data_source.py` & `SenseLink-2.2.0/senselink/mqtt/mqtt_data_source.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Copyright 2022, Charles Powell
 import logging
 import asyncio
+import json
 from math import isclose
+from senselink.common import *
 from senselink.data_source import DataSource
 from .mqtt_controller import MQTTController
 from .mqtt_listener import MQTTListener
 
 
 class MQTTSource(DataSource):
     # Primary output property
@@ -59,14 +61,24 @@
         self.state = False
 
     @property
     def power(self):
         return self._power
 
     def update_power(self, value, timeout=True):
+        if self.power_topic_keypath is not None:
+            logging.debug(f'Extracting power from JSON message, at key path {self.power_topic_keypath}')
+            # Extract value from (assumed) JSON message at keypath
+            message = json.loads(value)
+            # Overwrite value variable with what is extracted from JSON
+            value = safekey(message, self.power_topic_keypath)
+            if value is None:
+                logging.warning(f'Update on power topic failed to find value at power keypath ({self.power_topic_keypath})')
+                return
+
         try:
             fval = float(value)
         except ValueError:
             logging.warning(f'Failed to convert power value ("{value}") for {self.identifier} to float, ignoring')
             return
 
         # Reset previous timer
@@ -87,14 +99,25 @@
 
     async def power_handler(self, value):
         logging.debug(f'Power topic update for {self.identifier}: {value}')
         self.update_power(value)
 
     async def state_handler(self, value):
         logging.debug(f'State topic update for {self.identifier}: {value}')
+
+        if self.state_topic_keypath is not None:
+            logging.debug(f'Extracting state from JSON message, at key path {self.state_topic_keypath}')
+            # Extract value from (assumed) JSON message at keypath
+            message = json.loads(value)
+            # Overwrite value variable with what is extracted from JSON
+            value = safekey(message, self.state_topic_keypath)
+            if value is None:
+                logging.warning(f'Update on state topic failed to find value at state keypath ({self.state_topic_keypath})')
+                return
+
         # Act immediate if state is being set to off
         if value == self.off_state_value:
             # Device is off
             self.state = False
             self.update_power(self.off_usage)
             logging.debug(f'State set to OFF for {self.identifier}')
         elif value == self.on_state_value:
@@ -119,14 +142,25 @@
                     logging.debug(f'State update is numeric and no power_topic defined, using as power value')
                     self.update_power(fstate)
             except ValueError:
                 logging.debug(f'State update ("{value}") is non-numeric and does not match on/off values, ignoring')
 
     async def attribute_handler(self, value):
         logging.debug(f'Attribute topic update for {self.identifier}: {value}')
+
+        if self.attribute_topic_keypath is not None:
+            logging.debug(f'Extracting attribute value from JSON message, at key path {self.attribute_topic_keypath}')
+            # Extract value from (assumed) JSON message at keypath
+            message = json.loads(value)
+            # Overwrite value variable with what is extracted from JSON
+            value = safekey(message, self.attribute_topic_keypath)
+            if value is None:
+                logging.warning(f'Update on attribute topic failed to find value at attribute keypath ({self.attribute_topic_keypath})')
+                return
+
         # Get attribute value and scale to provided values
         try:
             attribute_value = float(value)
         except ValueError:
             logging.warning(f'Non-float value ("{value}") received for attribute update, unable to update!')
             self._power = self.off_usage
             self.state = False
```

### Comparing `SenseLink-2.1.0/senselink/plug_instance.py` & `SenseLink-2.2.0/senselink/plug_instance.py`

 * *Files identical despite different names*

### Comparing `SenseLink-2.1.0/senselink/senselink.py` & `SenseLink-2.2.0/senselink/senselink.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import yaml
 import asyncio
 import argparse
 import logging
 import dpath.util
 import json
 
+from .common import *
 from .data_source import *
 from .plug_instance import *
 from .tplink_encryption import *
 
 from senselink.mqtt import *
 from senselink.homeassistant import *
 
@@ -18,38 +19,14 @@
 MUTABLE_KEY = 'mutable'
 HASS_KEY = 'hass'
 MQTT_KEY = 'mqtt'
 AGG_KEY = 'aggregate'
 PLUGS_KEY = 'plugs'
 
 
-# Check if a multi-layer key exists
-def keys_exist(element, *keys):
-    if not isinstance(element, dict):
-        raise AttributeError('keys_exists() expects dict as first argument.')
-    if len(keys) == 0:
-        raise AttributeError('keys_exists() expects at least two arguments, one given.')
-
-    _element = element
-    for key in keys:
-        try:
-            _element = _element[key]
-        except KeyError:
-            return False
-    return True
-
-
-def safekey(d, keypath, default=None):
-    try:
-        val = dpath.util.get(d, keypath)
-        return val
-    except KeyError:
-        return default
-
-
 class SenseLinkProtocol(asyncio.DatagramProtocol):
     transport = None
     target = None
 
     def __init__(self, instances, finished):
         self._instances = instances
         self.should_respond = True
```

### Comparing `SenseLink-2.1.0/senselink/tplink_encryption.py` & `SenseLink-2.2.0/senselink/tplink_encryption.py`

 * *Files identical despite different names*

### Comparing `SenseLink-2.1.0/setup.py` & `SenseLink-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='SenseLink',
-    version='2.1.0',
+    version='2.2.0',
     description='A tool to create virtual smart plugs and inform a Sense Home Energy Monitor about usage in your home',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/cbpowell/SenseLink',
     author='Charles Powell',
     author_email='cbpowell@gmail.com',
     license='MIT',
```

