# Comparing `tmp/aioshelly-5.3.2.tar.gz` & `tmp/aioshelly-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioshelly-5.3.2.tar", last modified: Wed Apr 19 12:17:23 2023, max compression
+gzip compressed data, was "aioshelly-5.4.0.tar", last modified: Sun Jun 18 21:28:41 2023, max compression
```

## Comparing `aioshelly-5.3.2.tar` & `aioshelly-5.4.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:17:23.101659 aioshelly-5.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-19 12:17:06.000000 aioshelly-5.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-19 12:17:06.000000 aioshelly-5.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-19 12:17:23.101659 aioshelly-5.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-19 12:17:06.000000 aioshelly-5.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:17:23.101659 aioshelly-5.3.2/aioshelly/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:17:23.101659 aioshelly-5.3.2/aioshelly/ble/
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/ble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/ble/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:17:23.101659 aioshelly-5.3.2/aioshelly/block_device/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/block_device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/block_device/coap.py
--rw-r--r--   0 runner    (1001) docker     (123)    16966 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/block_device/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/json.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:17:23.101659 aioshelly-5.3.2/aioshelly/rpc_device/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/rpc_device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/rpc_device/device.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/rpc_device/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    16453 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/rpc_device/wsrpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:17:23.101659 aioshelly-5.3.2/aioshelly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-19 12:17:23.000000 aioshelly-5.3.2/aioshelly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-19 12:17:23.000000 aioshelly-5.3.2/aioshelly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:17:23.000000 aioshelly-5.3.2/aioshelly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-19 12:17:23.000000 aioshelly-5.3.2/aioshelly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 12:17:23.000000 aioshelly-5.3.2/aioshelly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:17:23.000000 aioshelly-5.3.2/aioshelly.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-19 12:17:06.000000 aioshelly-5.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-19 12:17:23.105659 aioshelly-5.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-19 12:17:06.000000 aioshelly-5.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:28:41.918056 aioshelly-5.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-06-18 21:28:33.000000 aioshelly-5.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-18 21:28:33.000000 aioshelly-5.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-06-18 21:28:41.918056 aioshelly-5.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-18 21:28:33.000000 aioshelly-5.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:28:41.918056 aioshelly-5.4.0/aioshelly/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-18 21:28:33.000000 aioshelly-5.4.0/aioshelly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:28:41.918056 aioshelly-5.4.0/aioshelly/ble/
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-06-18 21:28:33.000000 aioshelly-5.4.0/aioshelly/ble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-18 21:28:33.000000 aioshelly-5.4.0/aioshelly/ble/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:28:41.918056 aioshelly-5.4.0/aioshelly/block_device/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-18 21:28:33.000000 aioshelly-5.4.0/aioshelly/block_device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-06-18 21:28:33.000000 aioshelly-5.4.0/aioshelly/block_device/coap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16966 2023-06-18 21:28:33.000000 aioshelly-5.4.0/aioshelly/block_device/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-18 21:28:33.000000 aioshelly-5.4.0/aioshelly/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-18 21:28:33.000000 aioshelly-5.4.0/aioshelly/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-18 21:28:33.000000 aioshelly-5.4.0/aioshelly/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-18 21:28:33.000000 aioshelly-5.4.0/aioshelly/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 21:28:33.000000 aioshelly-5.4.0/aioshelly/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:28:41.918056 aioshelly-5.4.0/aioshelly/rpc_device/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-18 21:28:33.000000 aioshelly-5.4.0/aioshelly/rpc_device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-06-18 21:28:33.000000 aioshelly-5.4.0/aioshelly/rpc_device/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-18 21:28:33.000000 aioshelly-5.4.0/aioshelly/rpc_device/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16453 2023-06-18 21:28:33.000000 aioshelly-5.4.0/aioshelly/rpc_device/wsrpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:28:41.918056 aioshelly-5.4.0/aioshelly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-06-18 21:28:41.000000 aioshelly-5.4.0/aioshelly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-18 21:28:41.000000 aioshelly-5.4.0/aioshelly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 21:28:41.000000 aioshelly-5.4.0/aioshelly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-18 21:28:41.000000 aioshelly-5.4.0/aioshelly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-18 21:28:41.000000 aioshelly-5.4.0/aioshelly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 21:28:41.000000 aioshelly-5.4.0/aioshelly.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-18 21:28:33.000000 aioshelly-5.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-18 21:28:41.922056 aioshelly-5.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-18 21:28:33.000000 aioshelly-5.4.0/setup.py
```

### Comparing `aioshelly-5.3.2/LICENSE` & `aioshelly-5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aioshelly-5.3.2/PKG-INFO` & `aioshelly-5.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioshelly
-Version: 5.3.2
+Version: 5.4.0
 Summary: Asynchronous library to control Shelly devices.
 Home-page: https://github.com/home-assistant-libs/aioshelly
 Author: Paulus Schoutsen
 Author-email: paulus@home-assistant.io
 License: Apache License 2.0
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `aioshelly-5.3.2/README.md` & `aioshelly-5.4.0/README.md`

 * *Files identical despite different names*

### Comparing `aioshelly-5.3.2/aioshelly/ble/__init__.py` & `aioshelly-5.4.0/aioshelly/ble/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Shelly Gen2 BLE support."""
 from __future__ import annotations
 
 import logging
-from base64 import b64decode
+from binascii import a2b_base64
 from typing import Any
 
 from bluetooth_data_tools import BLEGAPAdvertisement, parse_advertisement_data
 
 from ..exceptions import RpcCallError
 from ..rpc_device import RpcDevice
 from .const import (
@@ -95,15 +95,18 @@
     rssi: int = data[2]
     advertisement_data_b64: str = data[3]
     scan_response_b64: str = data[4]
     return (
         address.upper(),
         rssi,
         parse_advertisement_data(
-            (b64decode(advertisement_data_b64), b64decode(scan_response_b64))
+            (
+                a2b_base64(advertisement_data_b64.encode("ascii")),
+                a2b_base64(scan_response_b64.encode("ascii")),
+            )
         ),
     )
 
 
 async def async_ensure_ble_enabled(device: RpcDevice) -> bool:
     """Ensure BLE is enabled.
```

### Comparing `aioshelly-5.3.2/aioshelly/ble/const.py` & `aioshelly-5.4.0/aioshelly/ble/const.py`

 * *Files identical despite different names*

### Comparing `aioshelly-5.3.2/aioshelly/block_device/coap.py` & `aioshelly-5.4.0/aioshelly/block_device/coap.py`

 * *Files identical despite different names*

### Comparing `aioshelly-5.3.2/aioshelly/block_device/device.py` & `aioshelly-5.4.0/aioshelly/block_device/device.py`

 * *Files identical despite different names*

### Comparing `aioshelly-5.3.2/aioshelly/common.py` & `aioshelly-5.4.0/aioshelly/common.py`

 * *Files identical despite different names*

### Comparing `aioshelly-5.3.2/aioshelly/const.py` & `aioshelly-5.4.0/aioshelly/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,29 +53,32 @@
     "SHSW-L": "Shelly 1L",
     "SHSW-PM": "Shelly 1PM",
     "SHTRV-01": "Shelly Valve",
     "SHUNI-1": "Shelly UNI",
     "SHVIN-1": "Shelly Vintage",
     "SHWT-1": "Shelly Flood",
     # Gen2 RPC based models
+    "SAWD-0A1XX10EU1": "Shelly Wall Display",
     "SNPL-00110IT": "Shelly Plus Plug IT",
     "SNPL-00112EU": "Shelly Plus Plug S",
     "SNPL-00112UK": "Shelly Plus Plug UK",
     "SNPL-00116US": "Shelly Plus Plug US",
     "SNSN-0013A": "Shelly Plus H&T",
     "SNSN-0031Z": "Shelly Plus Smoke",
     "SNSN-0D24X": "Shelly Plus I4DC",
     "SNSW-001P15UL": "Shelly Plus 1PM UL",
     "SNSW-001P16EU": "Shelly Plus 1PM",
     "SNSW-001X15UL": "Shelly Plus 1 UL",
     "SNSW-001X16EU": "Shelly Plus 1",
     "SNSW-0024X": "Shelly Plus I4",
     "SNSW-002P16EU": "Shelly Plus 2PM",
     "SNSW-102P16EU": "Shelly Plus 2PM",
+    "SPEM-002CEBEU50": "Shelly Pro EM",
     "SPEM-003CEBEU": "Shelly Pro 3EM",
+    "SPSH-002PE16EU": "Shelly Pro Dual Cover PM",
     "SPSW-001PE16EU": "Shelly Pro 1PM",
     "SPSW-001XE16EU": "Shelly Pro 1",
     "SPSW-002PE16EU": "Shelly Pro 2PM",
     "SPSW-002XE16EU": "Shelly Pro 2",
     "SPSW-003XE16EU": "Shelly Pro 3",
     "SPSW-004PE16EU": "Shelly Pro 4PM",
     "SPSW-101PE16EU": "Shelly Pro 1PM",
```

### Comparing `aioshelly-5.3.2/aioshelly/exceptions.py` & `aioshelly-5.4.0/aioshelly/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioshelly-5.3.2/aioshelly/json.py` & `aioshelly-5.4.0/aioshelly/json.py`

 * *Files identical despite different names*

### Comparing `aioshelly-5.3.2/aioshelly/rpc_device/device.py` & `aioshelly-5.4.0/aioshelly/rpc_device/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,22 @@
     DeviceConnectionError,
     InvalidAuthError,
     NotInitialized,
     RpcCallError,
     ShellyError,
     WrongShellyGen,
 )
-from .models import ShellyBLEConfig, ShellyBLESetConfig, ShellyScript, ShellyScriptCode
+from .models import (
+    ShellyBLEConfig,
+    ShellyBLESetConfig,
+    ShellyScript,
+    ShellyScriptCode,
+    ShellyWsConfig,
+    ShellyWsSetConfig,
+)
 from .wsrpc import WsRPC, WsServer
 
 _LOGGER = logging.getLogger(__name__)
 
 
 def mergedicts(dict1: dict, dict2: dict) -> dict:
     """Deep dicts merge."""
@@ -255,14 +262,49 @@
             ),
         )
 
     async def ble_getconfig(self) -> ShellyBLEConfig:
         """Get the BLE config with BLE.GetConfig."""
         return cast(ShellyBLEConfig, await self.call_rpc("BLE.GetConfig"))
 
+    async def ws_setconfig(
+        self, enable: bool, server: str, ssl_ca: str = "*"
+    ) -> ShellyWsSetConfig:
+        """Set the outbound websocket config."""
+        return cast(
+            ShellyWsSetConfig,
+            await self.call_rpc(
+                "Ws.SetConfig",
+                {"config": {"enable": enable, "server": server, "ssl_ca": ssl_ca}},
+            ),
+        )
+
+    async def ws_getconfig(self) -> ShellyWsConfig:
+        """Get the outbound websocket config."""
+        return cast(ShellyWsConfig, await self.call_rpc("Ws.GetConfig"))
+
+    async def update_outbound_websocket(self, server: str) -> bool:
+        """Update the outbound websocket (if needed).
+
+        Returns True if the device was restarted.
+
+        Raises RpcCallError if set failed.
+        """
+        ws_config = await self.ws_getconfig()
+        if ws_config["enable"] and ws_config["server"] == server:
+            return False
+        ws_enable = await self.ws_setconfig(enable=True, server=server)
+        if not ws_enable["restart_required"]:
+            return False
+        _LOGGER.info(
+            "Outbound websocket enabled, restarting device %s", self.ip_address
+        )
+        await self.trigger_reboot(3500)
+        return True
+
     @property
     def requires_auth(self) -> bool:
         """Device check for authentication."""
         if "auth_en" not in self.shelly:
             raise WrongShellyGen
 
         return bool(self.shelly["auth_en"])
```

### Comparing `aioshelly-5.3.2/aioshelly/rpc_device/models.py` & `aioshelly-5.4.0/aioshelly/rpc_device/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,7 +32,21 @@
     rpc: ShellyBLERpcConfig
 
 
 class ShellyBLESetConfig(TypedDict, total=False):
     """Shelly BLE Set Config."""
 
     restart_required: bool
+
+
+class ShellyWsConfig(TypedDict, total=False):
+    """Shelly Outbound Websocket Config."""
+
+    enable: bool
+    server: str | None
+    ssl_ca: str
+
+
+class ShellyWsSetConfig(TypedDict, total=False):
+    """Shelly Outbound Websocket Set Config."""
+
+    restart_required: bool
```

### Comparing `aioshelly-5.3.2/aioshelly/rpc_device/wsrpc.py` & `aioshelly-5.4.0/aioshelly/rpc_device/wsrpc.py`

 * *Files identical despite different names*

### Comparing `aioshelly-5.3.2/aioshelly.egg-info/PKG-INFO` & `aioshelly-5.4.0/aioshelly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioshelly
-Version: 5.3.2
+Version: 5.4.0
 Summary: Asynchronous library to control Shelly devices.
 Home-page: https://github.com/home-assistant-libs/aioshelly
 Author: Paulus Schoutsen
 Author-email: paulus@home-assistant.io
 License: Apache License 2.0
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `aioshelly-5.3.2/aioshelly.egg-info/SOURCES.txt` & `aioshelly-5.4.0/aioshelly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioshelly-5.3.2/setup.py` & `aioshelly-5.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Setup module for aioshelly."""
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "5.3.2"
+VERSION = "5.4.0"
 
 
 setup(
     name="aioshelly",
     version=VERSION,
     license="Apache License 2.0",
     url="https://github.com/home-assistant-libs/aioshelly",
```

