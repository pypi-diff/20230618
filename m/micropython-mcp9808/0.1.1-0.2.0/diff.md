# Comparing `tmp/micropython-mcp9808-0.1.1.tar.gz` & `tmp/micropython-mcp9808-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-mcp9808-0.1.1.tar", last modified: Sun Jun 18 04:45:30 2023, max compression
+gzip compressed data, was "micropython-mcp9808-0.2.0.tar", last modified: Sun Jun 18 19:12:59 2023, max compression
```

## Comparing `micropython-mcp9808-0.1.1.tar` & `micropython-mcp9808-0.2.0.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:30.832149 micropython-mcp9808-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:30.828149 micropython-mcp9808-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:30.828149 micropython-mcp9808-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-18 04:45:15.000000 micropython-mcp9808-0.1.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-18 04:45:15.000000 micropython-mcp9808-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-18 04:45:15.000000 micropython-mcp9808-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-18 04:45:15.000000 micropython-mcp9808-0.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-18 04:45:15.000000 micropython-mcp9808-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-18 04:45:15.000000 micropython-mcp9808-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-18 04:45:30.832149 micropython-mcp9808-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-18 04:45:15.000000 micropython-mcp9808-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:30.828149 micropython-mcp9808-0.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:30.828149 micropython-mcp9808-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-18 04:45:15.000000 micropython-mcp9808-0.1.1/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-18 04:45:15.000000 micropython-mcp9808-0.1.1/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-18 04:45:15.000000 micropython-mcp9808-0.1.1/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-18 04:45:15.000000 micropython-mcp9808-0.1.1/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-18 04:45:15.000000 micropython-mcp9808-0.1.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-18 04:45:15.000000 micropython-mcp9808-0.1.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-18 04:45:15.000000 micropython-mcp9808-0.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-18 04:45:15.000000 micropython-mcp9808-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-18 04:45:15.000000 micropython-mcp9808-0.1.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-18 04:45:15.000000 micropython-mcp9808-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-18 04:45:15.000000 micropython-mcp9808-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:30.828149 micropython-mcp9808-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-18 04:45:23.000000 micropython-mcp9808-0.1.1/examples/mcp9808_hysteresis.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-18 04:45:23.000000 micropython-mcp9808-0.1.1/examples/mcp9808_power_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-18 04:45:23.000000 micropython-mcp9808-0.1.1/examples/mcp9808_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:15.000000 micropython-mcp9808-0.1.1/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:30.828149 micropython-mcp9808-0.1.1/micropython_mcp9808/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:23.000000 micropython-mcp9808-0.1.1/micropython_mcp9808/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-18 04:45:23.000000 micropython-mcp9808-0.1.1/micropython_mcp9808/i2c_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-06-18 04:45:23.000000 micropython-mcp9808-0.1.1/micropython_mcp9808/mcp9808.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:30.828149 micropython-mcp9808-0.1.1/micropython_mcp9808.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-18 04:45:30.000000 micropython-mcp9808-0.1.1/micropython_mcp9808.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-18 04:45:30.000000 micropython-mcp9808-0.1.1/micropython_mcp9808.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 04:45:30.000000 micropython-mcp9808-0.1.1/micropython_mcp9808.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-18 04:45:30.000000 micropython-mcp9808-0.1.1/micropython_mcp9808.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-18 04:45:30.000000 micropython-mcp9808-0.1.1/micropython_mcp9808.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-18 04:45:15.000000 micropython-mcp9808-0.1.1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-18 04:45:23.000000 micropython-mcp9808-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-18 04:45:15.000000 micropython-mcp9808-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 04:45:30.832149 micropython-mcp9808-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:12:59.570573 micropython-mcp9808-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:12:59.566573 micropython-mcp9808-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:12:59.566573 micropython-mcp9808-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-18 19:12:59.570573 micropython-mcp9808-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:12:59.570573 micropython-mcp9808-0.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:12:59.570573 micropython-mcp9808-0.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:12:59.570573 micropython-mcp9808-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-18 19:12:51.000000 micropython-mcp9808-0.2.0/examples/mcp9808_hysteresis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-18 19:12:51.000000 micropython-mcp9808-0.2.0/examples/mcp9808_power_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-18 19:12:51.000000 micropython-mcp9808-0.2.0/examples/mcp9808_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-18 19:12:51.000000 micropython-mcp9808-0.2.0/examples/mcp9808_temperature_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-18 19:12:51.000000 micropython-mcp9808-0.2.0/examples/mcp9808_temperature_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:12:59.570573 micropython-mcp9808-0.2.0/micropython_mcp9808/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 19:12:51.000000 micropython-mcp9808-0.2.0/micropython_mcp9808/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-18 19:12:51.000000 micropython-mcp9808-0.2.0/micropython_mcp9808/i2c_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10839 2023-06-18 19:12:51.000000 micropython-mcp9808-0.2.0/micropython_mcp9808/mcp9808.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:12:59.570573 micropython-mcp9808-0.2.0/micropython_mcp9808.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-18 19:12:59.000000 micropython-mcp9808-0.2.0/micropython_mcp9808.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-18 19:12:59.000000 micropython-mcp9808-0.2.0/micropython_mcp9808.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 19:12:59.000000 micropython-mcp9808-0.2.0/micropython_mcp9808.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-18 19:12:59.000000 micropython-mcp9808-0.2.0/micropython_mcp9808.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-18 19:12:59.000000 micropython-mcp9808-0.2.0/micropython_mcp9808.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-18 19:12:51.000000 micropython-mcp9808-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 19:12:59.570573 micropython-mcp9808-0.2.0/setup.cfg
```

### Comparing `micropython-mcp9808-0.1.1/.gitignore` & `micropython-mcp9808-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `micropython-mcp9808-0.1.1/.pre-commit-config.yaml` & `micropython-mcp9808-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `micropython-mcp9808-0.1.1/.pylintrc` & `micropython-mcp9808-0.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-mcp9808-0.1.1/LICENSE` & `micropython-mcp9808-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-mcp9808-0.1.1/PKG-INFO` & `micropython-mcp9808-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-mcp9808
-Version: 0.1.1
+Version: 0.2.0
 Summary: MicroPython Driver for the Microchip MCP9808 Temperature Sensor
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_MCP9808
 Keywords: sensor,micropython,mcp9808,temperature,microchip,mcp9808,temperature,micropython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `micropython-mcp9808-0.1.1/README.rst` & `micropython-mcp9808-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `micropython-mcp9808-0.1.1/docs/_static/Logo.png` & `micropython-mcp9808-0.2.0/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-mcp9808-0.1.1/docs/_static/favicon.ico` & `micropython-mcp9808-0.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `micropython-mcp9808-0.1.1/docs/conf.py` & `micropython-mcp9808-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `micropython-mcp9808-0.1.1/examples/mcp9808_hysteresis.py` & `micropython-mcp9808-0.2.0/examples/mcp9808_hysteresis.py`

 * *Files identical despite different names*

### Comparing `micropython-mcp9808-0.1.1/examples/mcp9808_power_mode.py` & `micropython-mcp9808-0.2.0/examples/mcp9808_power_mode.py`

 * *Files identical despite different names*

### Comparing `micropython-mcp9808-0.1.1/micropython_mcp9808/i2c_helpers.py` & `micropython-mcp9808-0.2.0/micropython_mcp9808/i2c_helpers.py`

 * *Files identical despite different names*

### Comparing `micropython-mcp9808-0.1.1/micropython_mcp9808/mcp9808.py` & `micropython-mcp9808-0.2.0/micropython_mcp9808/mcp9808.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,39 +11,54 @@
 
 
 * Author(s): Jose D. Montoya
 
 
 """
 
+from collections import namedtuple
 from micropython import const
 from micropython_mcp9808.i2c_helpers import CBits, RegisterStruct
 
 
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 __repo__ = "https://github.com/jposada202020/MicroPython_MCP9808.git"
 
 
 _CONFIG = const(0x01)
 _UPPER_TEMP = const(0x02)
-_LOWER_TEMP = const(0x02)
-_CRITICAL_TEMP = const(0x02)
+_LOWER_TEMP = const(0x03)
+_CRITICAL_TEMP = const(0x04)
 _TEMP = const(0x05)
 _REG_WHOAMI = const(0x07)
+_RESOLUTION = const(0x08)
 
 HYSTERESIS_0 = const(0b00)
 HYSTERESIS_1_5 = const(0b01)
 HYSTERESIS_3 = const(0b10)
 HYSTERESIS_6 = const(0b11)
 hysteresis_values = (HYSTERESIS_0, HYSTERESIS_1_5, HYSTERESIS_3, HYSTERESIS_6)
 
-CONTINUOUS = const(0b00)
+CONTINUOUS = const(0b0)
 SHUTDOWN = const(0b1)
 power_mode_values = (CONTINUOUS, SHUTDOWN)
 
+RESOLUTION_0_5_C = const(0b00)
+RESOLUTION_0_625_C = const(0b01)
+RESOLUTION_0_125_C = const(0b10)
+RESOLUTION_0_0625_C = const(0b11)
+temperature_resolution_values = (
+    RESOLUTION_0_5_C,
+    RESOLUTION_0_625_C,
+    RESOLUTION_0_125_C,
+    RESOLUTION_0_0625_C,
+)
+
+AlertStatus = namedtuple("AlertStatus", ["high_alert", "low_alert", "critical_alert"])
+
 
 class MCP9808:
     """Driver for the MCP9808 Sensor connected over I2C.
 
     :param ~machine.I2C i2c: The I2C bus the MCP9808 is connected to.
     :param int address: The I2C device address. Defaults to :const:`0x18`
 
@@ -53,38 +68,43 @@
 
     Here is an example of using the :class:`MCP9808` class.
     First you will need to import the libraries to use the sensor
 
     .. code-block:: python
 
         from machine import Pin, I2C
-        import mcp9808
+        from micropython_mcp9808 import mcp9808
 
     Once this is done you can define your `machine.I2C` object and define your sensor object
 
     .. code-block:: python
 
-        i2c = I2C(sda=Pin28), scl=Pin(3))
-        mcp9808 = mcp9808.MCP9808(i2c)
+        i2c = I2C(1, sda=Pin(2), scl=Pin(3))
+        mcp = mcp9808.MCP9808(i2c)
 
     Now you have access to the attributes
 
     .. code-block:: python
 
+        temp = mcp.temperature
+
     """
 
     _device_id = RegisterStruct(_REG_WHOAMI, "B")
     _config = RegisterStruct(_CONFIG, "H")
 
     _hysteresis = CBits(2, _CONFIG, 9, 2, False)
     _power_mode = CBits(1, _CONFIG, 8, 2, False)
+
     _temperature_data = CBits(13, _TEMP, 0, 2, False)
-    _temperature_upper = CBits(11, _UPPER_TEMP, 2, 2, False)
-    _temperature_lower = CBits(11, _LOWER_TEMP, 2, 2, False)
-    _temperature_critical = CBits(11, _CRITICAL_TEMP, 2, 2, False)
+    _temperature_resolution = CBits(2, _RESOLUTION, 0)
+
+    critical_alert = CBits(1, _TEMP, 7, register_width=1)
+    high_alert = CBits(1, _TEMP, 6, register_width=1)
+    low_alert = CBits(1, _TEMP, 5, register_width=1)
 
     def __init__(self, i2c, address: int = 0x18) -> None:
         self._i2c = i2c
         self._address = address
 
         if self._device_id != 0x04:
             raise RuntimeError("Failed to find MCP9808")
@@ -139,45 +159,53 @@
     @power_mode.setter
     def power_mode(self, value: int) -> None:
         if value not in power_mode_values:
             raise ValueError("Value must be a valid power_mode setting")
         self._power_mode = value
 
     @property
-    def temperature(self) -> float:
+    def temperature(self):
         """
         Temperature in Celsius
         """
-        return self._convert_temperature(self._temperature_data)
+        data = bytearray(2)
+        self._i2c.readfrom_mem_into(self._address, _TEMP, data)
+
+        return self._convert_temperature(data)
 
     @staticmethod
-    def _convert_temperature(temp: int) -> float:
+    def _convert_temperature(temp: bytearray) -> float:
 
-        high_byte = temp >> 8
-        low_byte = temp & 0xFF
-        if high_byte & 0x10 == 0x10:
-            high_byte = high_byte & 0x0F
-            return 256 - (high_byte * 16 + low_byte / 16.0)
-        return high_byte * 16 + low_byte / 16.0
+        temp[0] = temp[0] & 0x1F
+        if temp[0] & 0x10 == 0x10:
+            temp[0] = temp[0] & 0x0F
+            return (temp[0] * 16 + temp[1] / 16.0) - 256
+        return temp[0] * 16 + temp[1] / 16.0
 
     @property
     def temperature_upper(self) -> float:
         """
         Upper temperature in Celsius
         """
-        return self._convert_temperature(self._temperature_upper)
+        return self._get_temperature(_UPPER_TEMP)
 
     @temperature_upper.setter
     def temperature_upper(self, value: int) -> None:
         if not isinstance(value, int):
             raise ValueError("Temperature must be an int value")
-        self._temperature_upper = self._limit_temperatures(value)
+        self._limit_temperatures(value, _UPPER_TEMP)
 
-    @staticmethod
-    def _limit_temperatures(temp: int) -> int:
+    def _get_temperature(self, register_address):
+
+        data = bytearray(2)
+        self._i2c.readfrom_mem_into(self._address, register_address, data)
+
+        return self._convert_temperature(data)
+
+    def _limit_temperatures(self, temp: int, register_address):
         """Internal function to setup limit temperature
         :param int temp: temperature limit
         """
 
         if temp < 0:
             negative = True
             temp = abs(temp)
@@ -186,36 +214,108 @@
 
         high_byte = temp >> 4
         if negative:
             high_byte = high_byte | 0x10
 
         low_byte = (temp & 0x0F) << 4
 
-        value = high_byte << 8 | low_byte
-
-        return value
+        self._i2c.writeto_mem(
+            self._address, register_address, bytes([high_byte, low_byte])
+        )
 
     @property
     def temperature_lower(self) -> float:
         """
         Lower temperature in Celsius
         """
-        return self._convert_temperature(self._temperature_lower)
+        return self._get_temperature(_LOWER_TEMP)
 
     @temperature_lower.setter
     def temperature_lower(self, value: int) -> None:
         if not isinstance(value, int):
             raise ValueError("Temperature must be an int value")
-        self._temperature_lower = self._limit_temperatures(value)
+        self._limit_temperatures(value, _LOWER_TEMP)
 
     @property
     def temperature_critical(self) -> float:
         """
         Critical temperature in Celsius
         """
-        return self._convert_temperature(self._temperature_critical)
+        return self._get_temperature(_CRITICAL_TEMP)
 
     @temperature_critical.setter
     def temperature_critical(self, value: int) -> None:
         if not isinstance(value, int):
             raise ValueError("Temperature must be an int value")
-        self._temperature_critical = self._limit_temperatures(value)
+        self._limit_temperatures(value, _CRITICAL_TEMP)
+
+    @property
+    def alert_status(self):
+        """The current triggered status of the high and low temperature alerts as a AlertStatus
+        named tuple with attributes for the triggered status of each alert.
+
+        .. code-block :: python
+
+            import time
+            from machine import Pin, I2C
+            from micropython_mcp9808 import mcp9808
+
+            i2c = I2C(1, sda=Pin(2), scl=Pin(3))  # Correct I2C pins for RP2040
+            mcp = mcp9808.MCP9808(i2c)
+
+            mcp.temperature_lower = 20
+            mcp.temperature_upper = 23
+            mcp.temperature_critical = 30
+
+            print("High limit: {}".format(mcp.temperature_upper))
+            print("Low limit: {}".format(mcp.temperature_lower))
+            print("Critical limit: {}".format(mcp.temperature_critical))
+
+            while True:
+                print("Temperature: {:.2f}C".format(mcp.temperature))
+                alert_status = tmp.alert_status
+                if alert_status.high_alert:
+                    print("Temperature above high set limit!")
+                if alert_status.low_alert:
+                    print("Temperature below low set limit!")
+                if alert_status.critical_alert:
+                    print("Temperature above critical set limit!")
+                time.sleep(1)
+
+        """
+
+        return AlertStatus(
+            high_alert=self.high_alert,
+            low_alert=self.low_alert,
+            critical_alert=self.critical_alert,
+        )
+
+    @property
+    def temperature_resolution(self) -> str:
+        """
+        Sensor temperature_resolution
+
+        +------------------------------------------+---------------------------+
+        | Mode                                     | Value                     |
+        +==========================================+===========================+
+        | :py:const:`mcp9808.RESOLUTION_0_5_C`     | :py:const:`0b00` 0.5°C    |
+        +------------------------------------------+---------------------------+
+        | :py:const:`mcp9808.RESOLUTION_0_625_C`   | :py:const:`0b01` 0.25°C   |
+        +------------------------------------------+---------------------------+
+        | :py:const:`mcp9808.RESOLUTION_0_125_C`   | :py:const:`0b10` 0.125°C  |
+        +------------------------------------------+---------------------------+
+        | :py:const:`mcp9808.RESOLUTION_0_0625_C`  | :py:const:`0b11` 0.0625°C |
+        +------------------------------------------+---------------------------+
+        """
+        values = (
+            "RESOLUTION_0_5_C",
+            "RESOLUTION_0_625_C",
+            "RESOLUTION_0_125_C",
+            "RESOLUTION_0_0625_C",
+        )
+        return values[self._temperature_resolution]
+
+    @temperature_resolution.setter
+    def temperature_resolution(self, value: int) -> None:
+        if value not in temperature_resolution_values:
+            raise ValueError("Value must be a valid temperature_resolution setting")
+        self._temperature_resolution = value
```

### Comparing `micropython-mcp9808-0.1.1/micropython_mcp9808.egg-info/PKG-INFO` & `micropython-mcp9808-0.2.0/micropython_mcp9808.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-mcp9808
-Version: 0.1.1
+Version: 0.2.0
 Summary: MicroPython Driver for the Microchip MCP9808 Temperature Sensor
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_MCP9808
 Keywords: sensor,micropython,mcp9808,temperature,microchip,mcp9808,temperature,micropython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `micropython-mcp9808-0.1.1/micropython_mcp9808.egg-info/SOURCES.txt` & `micropython-mcp9808-0.2.0/micropython_mcp9808.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 docs/_static/extra_css.css
 docs/_static/extra_css.css.license
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/mcp9808_hysteresis.py
 examples/mcp9808_power_mode.py
 examples/mcp9808_simpletest.py
+examples/mcp9808_temperature_limits.py
+examples/mcp9808_temperature_resolution.py
 micropython_mcp9808/__init__.py
 micropython_mcp9808/i2c_helpers.py
 micropython_mcp9808/mcp9808.py
 micropython_mcp9808.egg-info/PKG-INFO
 micropython_mcp9808.egg-info/SOURCES.txt
 micropython_mcp9808.egg-info/dependency_links.txt
 micropython_mcp9808.egg-info/requires.txt
```

### Comparing `micropython-mcp9808-0.1.1/pyproject.toml` & `micropython-mcp9808-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-mcp9808"
 description = "MicroPython Driver for the Microchip MCP9808 Temperature Sensor"
-version = "0.1.1"
+version = "0.2.0"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_MCP9808"}
 keywords = [
     "sensor",
```

