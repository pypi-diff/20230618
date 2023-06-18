# Comparing `tmp/bthome_ble-2.8.0.tar.gz` & `tmp/bthome_ble-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bthome_ble-2.8.0.tar", max compression
+gzip compressed data, was "bthome_ble-2.9.0.tar", max compression
```

## Comparing `bthome_ble-2.8.0.tar` & `bthome_ble-2.9.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-03-05 19:12:03.836197 bthome_ble-2.8.0/LICENSE
--rw-r--r--   0        0        0     3675 2023-03-05 19:12:03.836197 bthome_ble-2.8.0/README.md
--rw-r--r--   0        0        0     2379 2023-03-05 19:12:04.592209 bthome_ble-2.8.0/pyproject.toml
--rw-r--r--   0        0        0      610 2023-03-05 19:12:04.552209 bthome_ble-2.8.0/src/bthome_ble/__init__.py
--rw-r--r--   0        0        0     3588 2023-03-05 19:12:03.836197 bthome_ble-2.8.0/src/bthome_ble/bthome_v1_encryption.py
--rw-r--r--   0        0        0     3739 2023-03-05 19:12:03.836197 bthome_ble-2.8.0/src/bthome_ble/bthome_v2_encryption.py
--rw-r--r--   0        0        0     9886 2023-03-05 19:12:03.836197 bthome_ble-2.8.0/src/bthome_ble/const.py
--rw-r--r--   0        0        0      649 2023-03-05 19:12:03.836197 bthome_ble-2.8.0/src/bthome_ble/event.py
--rw-r--r--   0        0        0    20586 2023-03-05 19:12:03.836197 bthome_ble-2.8.0/src/bthome_ble/parser.py
--rw-r--r--   0        0        0        0 2023-03-05 19:12:03.836197 bthome_ble-2.8.0/src/bthome_ble/py.typed
--rw-r--r--   0        0        0     5129 1970-01-01 00:00:00.000000 bthome_ble-2.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-03-12 18:06:38.418232 bthome_ble-2.9.0/LICENSE
+-rw-r--r--   0        0        0     3675 2023-03-12 18:06:38.418232 bthome_ble-2.9.0/README.md
+-rw-r--r--   0        0        0     2379 2023-03-12 18:06:39.210245 bthome_ble-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0      610 2023-03-12 18:06:39.174244 bthome_ble-2.9.0/src/bthome_ble/__init__.py
+-rw-r--r--   0        0        0     3588 2023-03-12 18:06:38.418232 bthome_ble-2.9.0/src/bthome_ble/bthome_v1_encryption.py
+-rw-r--r--   0        0        0     3739 2023-03-12 18:06:38.418232 bthome_ble-2.9.0/src/bthome_ble/bthome_v2_encryption.py
+-rw-r--r--   0        0        0    10015 2023-03-12 18:06:38.418232 bthome_ble-2.9.0/src/bthome_ble/const.py
+-rw-r--r--   0        0        0      649 2023-03-12 18:06:38.418232 bthome_ble-2.9.0/src/bthome_ble/event.py
+-rw-r--r--   0        0        0    20586 2023-03-12 18:06:38.418232 bthome_ble-2.9.0/src/bthome_ble/parser.py
+-rw-r--r--   0        0        0        0 2023-03-12 18:06:38.418232 bthome_ble-2.9.0/src/bthome_ble/py.typed
+-rw-r--r--   0        0        0     5129 1970-01-01 00:00:00.000000 bthome_ble-2.9.0/PKG-INFO
```

### Comparing `bthome_ble-2.8.0/LICENSE` & `bthome_ble-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bthome_ble-2.8.0/README.md` & `bthome_ble-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `bthome_ble-2.8.0/pyproject.toml` & `bthome_ble-2.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bthome-ble"
-version = "2.8.0"
+version = "2.9.0"
 description = "BThome BLE support"
 authors = ["Ernst Klamer <e.klamer@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bluetooth-devices/bthome-ble"
 documentation = "https://bthome-ble.readthedocs.io"
 classifiers = [
@@ -27,15 +27,15 @@
 
 # Documentation Dependencies
 Sphinx = {version = "^5.0", optional = true}
 sphinx-rtd-theme = {version = "^1.0", optional = true}
 myst-parser = {version = "^0.18", optional = true}
 bluetooth-sensor-state-data = ">=1.6.1"
 pycryptodomex = ">=3.15.0"
-sensor-state-data = ">=2.13.0"
+sensor-state-data = ">=2.14.0"
 bluetooth-data-tools = ">=0.1.2"
 
 [tool.poetry.extras]
 docs = [
     "myst-parser",
     "sphinx",
     "sphinx-rtd-theme",
```

### Comparing `bthome_ble-2.8.0/src/bthome_ble/__init__.py` & `bthome_ble-2.9.0/src/bthome_ble/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     SensorUpdate,
     SensorValue,
     Units,
 )
 
 from .parser import BTHomeBluetoothDeviceData
 
-__version__ = "2.8.0"
+__version__ = "2.9.0"
 
 __all__ = [
     "BinarySensorDeviceClass",
     "BTHomeBluetoothDeviceData",
     "DeviceClass",
     "DeviceKey",
     "SensorDescription",
```

### Comparing `bthome_ble-2.8.0/src/bthome_ble/bthome_v1_encryption.py` & `bthome_ble-2.9.0/src/bthome_ble/bthome_v1_encryption.py`

 * *Files identical despite different names*

### Comparing `bthome_ble-2.8.0/src/bthome_ble/bthome_v2_encryption.py` & `bthome_ble-2.9.0/src/bthome_ble/bthome_v2_encryption.py`

 * *Files identical despite different names*

### Comparing `bthome_ble-2.8.0/src/bthome_ble/const.py` & `bthome_ble-2.9.0/src/bthome_ble/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -333,8 +333,13 @@
         factor=0.001,
     ),
     0x4E: MeasTypes(
         meas_format=SensorLibrary.VOLUME__VOLUME_LITERS,
         data_length=4,
         factor=0.001,
     ),
+    0x4F: MeasTypes(
+        meas_format=SensorLibrary.WATER__VOLUME_LITERS,
+        data_length=4,
+        factor=0.001,
+    ),
 }
```

### Comparing `bthome_ble-2.8.0/src/bthome_ble/event.py` & `bthome_ble-2.9.0/src/bthome_ble/event.py`

 * *Files identical despite different names*

### Comparing `bthome_ble-2.8.0/src/bthome_ble/parser.py` & `bthome_ble-2.9.0/src/bthome_ble/parser.py`

 * *Files identical despite different names*

### Comparing `bthome_ble-2.8.0/PKG-INFO` & `bthome_ble-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bthome-ble
-Version: 2.8.0
+Version: 2.9.0
 Summary: BThome BLE support
 Home-page: https://github.com/bluetooth-devices/bthome-ble
 License: MIT
 Author: Ernst Klamer
 Author-email: e.klamer@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -19,15 +19,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: docs
 Requires-Dist: Sphinx (>=5.0,<6.0) ; extra == "docs"
 Requires-Dist: bluetooth-data-tools (>=0.1.2)
 Requires-Dist: bluetooth-sensor-state-data (>=1.6.1)
 Requires-Dist: myst-parser (>=0.18,<0.19) ; extra == "docs"
 Requires-Dist: pycryptodomex (>=3.15.0)
-Requires-Dist: sensor-state-data (>=2.13.0)
+Requires-Dist: sensor-state-data (>=2.14.0)
 Requires-Dist: sphinx-rtd-theme (>=1.0,<2.0) ; extra == "docs"
 Project-URL: Bug Tracker, https://github.com/bluetooth-devices/bthome-ble/issues
 Project-URL: Changelog, https://github.com/bluetooth-devices/bthome-ble/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://bthome-ble.readthedocs.io
 Project-URL: Repository, https://github.com/bluetooth-devices/bthome-ble
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: bthome-ble Version: 2.8.0 Summary: BThome BLE
+Metadata-Version: 2.1 Name: bthome-ble Version: 2.9.0 Summary: BThome BLE
 support Home-page: https://github.com/bluetooth-devices/bthome-ble License: MIT
 Author: Ernst Klamer Author-email: e.klamer@gmail.com Requires-Python:
 >=3.9,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Software Development :: Libraries Provides-Extra: docs Requires-Dist:
 Sphinx (>=5.0,<6.0) ; extra == "docs" Requires-Dist: bluetooth-data-tools
 (>=0.1.2) Requires-Dist: bluetooth-sensor-state-data (>=1.6.1) Requires-Dist:
 myst-parser (>=0.18,<0.19) ; extra == "docs" Requires-Dist: pycryptodomex
-(>=3.15.0) Requires-Dist: sensor-state-data (>=2.13.0) Requires-Dist: sphinx-
+(>=3.15.0) Requires-Dist: sensor-state-data (>=2.14.0) Requires-Dist: sphinx-
 rtd-theme (>=1.0,<2.0) ; extra == "docs" Project-URL: Bug Tracker, https://
 github.com/bluetooth-devices/bthome-ble/issues Project-URL: Changelog, https://
 github.com/bluetooth-devices/bthome-ble/blob/main/CHANGELOG.md Project-URL:
 Documentation, https://bthome-ble.readthedocs.io Project-URL: Repository,
 https://github.com/bluetooth-devices/bthome-ble Description-Content-Type: text/
 markdown # BTHome BLE
          [CI_Status] [Documentation_Status] [Test_coverage_percentage]
```

