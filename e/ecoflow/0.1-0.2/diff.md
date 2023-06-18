# Comparing `tmp/ecoflow-0.1.tar.gz` & `tmp/ecoflow-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoflow-0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ecoflow-0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ecoflow-0.1.tar` & `ecoflow-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      817 2023-06-17 19:22:08.674424 ecoflow-0.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      704 2023-06-17 19:22:08.674424 ecoflow-0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0       36 2023-06-17 19:22:08.674424 ecoflow-0.1/.gitignore
--rw-r--r--   0        0        0     1081 2023-06-17 19:22:08.674424 ecoflow-0.1/LICENSE
--rw-r--r--   0        0        0     2009 2023-06-17 19:22:08.674424 ecoflow-0.1/README.md
--rw-r--r--   0        0        0      137 2023-06-17 19:22:08.674424 ecoflow-0.1/ecoflow/__init__.py
--rw-r--r--   0        0        0      847 2023-06-17 19:22:08.674424 ecoflow-0.1/ecoflow/common.py
--rw-r--r--   0        0        0     4868 2023-06-17 19:22:08.674424 ecoflow-0.1/ecoflow/delta2.py
--rw-r--r--   0        0        0      567 2023-06-17 19:22:08.674424 ecoflow-0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-17 19:22:08.674424 ecoflow-0.1/tests/__init__.py
--rw-r--r--   0        0        0     4415 2023-06-17 19:22:08.674424 ecoflow-0.1/tests/test_delta2.py
--rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 ecoflow-0.1/PKG-INFO
+-rw-r--r--   0        0        0      817 2023-06-18 08:16:47.908569 ecoflow-0.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      704 2023-06-18 08:16:47.908569 ecoflow-0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0       36 2023-06-18 08:16:47.908569 ecoflow-0.2/.gitignore
+-rw-r--r--   0        0        0     1081 2023-06-18 08:16:47.908569 ecoflow-0.2/LICENSE
+-rw-r--r--   0        0        0     2012 2023-06-18 08:16:47.908569 ecoflow-0.2/README.md
+-rw-r--r--   0        0        0      137 2023-06-18 08:16:47.908569 ecoflow-0.2/ecoflow/__init__.py
+-rw-r--r--   0        0        0      847 2023-06-18 08:16:47.908569 ecoflow-0.2/ecoflow/common.py
+-rw-r--r--   0        0        0     5017 2023-06-18 08:16:47.908569 ecoflow-0.2/ecoflow/delta2.py
+-rw-r--r--   0        0        0      567 2023-06-18 08:16:47.908569 ecoflow-0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-18 08:16:47.908569 ecoflow-0.2/tests/__init__.py
+-rw-r--r--   0        0        0     5128 2023-06-18 08:16:47.908569 ecoflow-0.2/tests/test_delta2.py
+-rw-r--r--   0        0        0     2511 1970-01-01 00:00:00.000000 ecoflow-0.2/PKG-INFO
```

### Comparing `ecoflow-0.1/.github/workflows/publish.yml` & `ecoflow-0.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ecoflow-0.1/.github/workflows/test.yml` & `ecoflow-0.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ecoflow-0.1/LICENSE` & `ecoflow-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ecoflow-0.1/README.md` & `ecoflow-0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,34 +23,31 @@
 ## Usage
 
 ```
 import asyncio
 import bleak
 from ecoflow import Delta2, OutputCircuit
 
-
 async def main():
     mac = "00:00:00:00:00:01"
     ble_client = bleak.BleakClient(mac, timeout=15)
     async with Delta2(ble_client) as dev:
         await dev.turn_on_circuit(OutputCircuit.USB)
         await dev.turn_off_circuit(OutputCircuit.AC)
 
         await dev.start_state_stream(print_state)
         await asyncio.sleep(40)
         await dev.stop_state_stream()
 
-
-def print_state(data):
+async def print_state(data):
     print("state update...")
     for k, v in data.items():
         print(f"{k} = {v}")
     print("-"*20)
 
-
 asyncio.run(main())
 ```
 
 Note to understand the example completely one may need to refer to:
 
 - bleak https://github.com/hbldh/bleak
 - Python asyncio https://realpython.com/async-io-python/
```

### Comparing `ecoflow-0.1/ecoflow/common.py` & `ecoflow-0.2/ecoflow/common.py`

 * *Files identical despite different names*

### Comparing `ecoflow-0.1/ecoflow/delta2.py` & `ecoflow-0.2/ecoflow/delta2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Delta 2 power station API
 """
 
 import logging
+import asyncio
 import struct
 from collections import namedtuple
 
 from .common import OutputCircuit
 from .common import StateField as SF
 from .common import BleConnectionMixin
 
@@ -90,26 +91,29 @@
         }
 
     def parse(self, _char, data):
         """
         Receive state notification data as raw bytes and parses into a dict with state fields
         """
         pages = self._split_pages(bytes(data))
-        state_fleids = {}
+        state_fields = {}
         for page in pages:
             page_code = self._page_code(page)
             try:
                 parser = self.page_parsers.get(page_code, self._nop_parser)
                 parsed_page = parser(page)
             except:
                 LOGGER.exception("could not parse a page %s. Data: %s", page_code, page)
                 parsed_page = {}
-            state_fleids.update(parsed_page)
+            state_fields.update(parsed_page)
 
-        self.callback(state_fleids)
+        if asyncio.iscoroutinefunction(self.callback):
+            asyncio.create_task(self.callback(state_fields))
+        else:
+            self.callback(state_fields)
 
     def _split_pages(self, data):
         pages = []
         unsplit = data
         while unsplit:
             unsplit, page_start, page_data = unsplit.rpartition(self.PAGE_HEADER)
             pages.append(page_start + page_data)
```

### Comparing `ecoflow-0.1/pyproject.toml` & `ecoflow-0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ecoflow-0.1/tests/test_delta2.py` & `ecoflow-0.2/tests/test_delta2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import asyncio
 from unittest.mock import AsyncMock
 import struct
 import pytest
 import bleak
 from ecoflow import Delta2
 from ecoflow.common import StateField, OutputCircuit
 
+STATE_CHAR_HANDLE = 0x2b
 
 @pytest.fixture
 def ble_client():
     client = AsyncMock()
     client.mock_add_spec(bleak.BleakClient, spec_set=True)
     return client
 
@@ -65,15 +67,14 @@
 
     await dev.turn_off_circuit(OutputCircuit.USB)
     ble_client.write_gatt_char.assert_called_with(0x29, exp_pkt_off)
 
 
 @pytest.mark.asyncio
 async def test_state_notifications(ble_client: AsyncMock):
-    STATE_CHAR_HANDLE = 0x2b
     state_data = {}
     def save_state_data_cb(data):
         nonlocal state_data
         state_data = data
     
     dev = Delta2(ble_client)
     src = FakeNotificationsSource()
@@ -115,14 +116,35 @@
     src.send(STATE_CHAR_HANDLE, page_0x5e)
     assert state_data[StateField.CHARGE_SPEED] == charge_speed
 
     await dev.stop_state_stream()
     ble_client.stop_notify.assert_called_with(STATE_CHAR_HANDLE)
 
 
+@pytest.mark.asyncio
+async def test_state_notifications_async_cb(ble_client: AsyncMock):
+    q = asyncio.Queue()
+    async def save_state_data_cb(data):
+        await q.put(data)
+    
+    dev = Delta2(ble_client)
+    src = FakeNotificationsSource()
+    ble_client.start_notify.side_effect = src.register
+
+    await dev.start_state_stream(save_state_data_cb)
+    ble_client.start_notify.assert_called_with(STATE_CHAR_HANDLE, src.send)
+
+    page_0x85 = [0xaa, 0x2, 0x85] + [0]*150
+    charge_level = 55
+    page_0x85[30] = charge_level
+
+    src.send(STATE_CHAR_HANDLE, page_0x85)
+    state_data = await asyncio.wait_for(q.get(), timeout=2)
+    assert state_data[StateField.CHARGE_LEVEL] == charge_level
+
 class FakeNotificationsSource:
     """
     Convenience object allowing tests to simulate BLE messages receival
     """
     def __init__(self) -> None:
         def nop():
             pass
```

### Comparing `ecoflow-0.1/PKG-INFO` & `ecoflow-0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoflow
-Version: 0.1
+Version: 0.2
 Summary: Python API for managing Ecoflow power stations
 Author-email: Anton Ptashnik <iavtomator@gmail.com>
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: bleak >=0.20.2
 Requires-Dist: pytest >= 7.3.0 ; extra == "test"
@@ -37,34 +37,31 @@
 ## Usage
 
 ```
 import asyncio
 import bleak
 from ecoflow import Delta2, OutputCircuit
 
-
 async def main():
     mac = "00:00:00:00:00:01"
     ble_client = bleak.BleakClient(mac, timeout=15)
     async with Delta2(ble_client) as dev:
         await dev.turn_on_circuit(OutputCircuit.USB)
         await dev.turn_off_circuit(OutputCircuit.AC)
 
         await dev.start_state_stream(print_state)
         await asyncio.sleep(40)
         await dev.stop_state_stream()
 
-
-def print_state(data):
+async def print_state(data):
     print("state update...")
     for k, v in data.items():
         print(f"{k} = {v}")
     print("-"*20)
 
-
 asyncio.run(main())
 ```
 
 Note to understand the example completely one may need to refer to:
 
 - bleak https://github.com/hbldh/bleak
 - Python asyncio https://realpython.com/async-io-python/
```

