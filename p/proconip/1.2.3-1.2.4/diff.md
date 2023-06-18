# Comparing `tmp/proconip-1.2.3.tar.gz` & `tmp/proconip-1.2.4.tar.gz`

## Comparing `proconip-1.2.3.tar` & `proconip-1.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 proconip-1.2.3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 proconip-1.2.3/CONTRIBUTING.md
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 proconip-1.2.3/SECURITY.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 proconip-1.2.3/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 proconip-1.2.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 proconip-1.2.3/.github/workflows/unittest.yml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 proconip-1.2.3/src/requirements.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 proconip-1.2.3/src/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.2.3/src/proconip/__init__.py
--rw-r--r--   0        0        0     8268 2020-02-02 00:00:00.000000 proconip-1.2.3/src/proconip/api.py
--rw-r--r--   0        0        0    23557 2020-02-02 00:00:00.000000 proconip-1.2.3/src/proconip/definitions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.2.3/tests/__init__.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 proconip-1.2.3/tests/helper.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 proconip-1.2.3/tests/requirements.txt
--rw-r--r--   0        0        0    12006 2020-02-02 00:00:00.000000 proconip-1.2.3/tests/test_definitions.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 proconip-1.2.3/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 proconip-1.2.3/LICENSE
--rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 proconip-1.2.3/README.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 proconip-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 proconip-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 proconip-1.2.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 proconip-1.2.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 proconip-1.2.4/SECURITY.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 proconip-1.2.4/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 proconip-1.2.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 proconip-1.2.4/.github/workflows/unittest.yml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 proconip-1.2.4/src/requirements.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 proconip-1.2.4/src/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.2.4/src/proconip/__init__.py
+-rw-r--r--   0        0        0    10016 2020-02-02 00:00:00.000000 proconip-1.2.4/src/proconip/api.py
+-rw-r--r--   0        0        0    23557 2020-02-02 00:00:00.000000 proconip-1.2.4/src/proconip/definitions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.2.4/tests/__init__.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 proconip-1.2.4/tests/helper.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 proconip-1.2.4/tests/requirements.txt
+-rw-r--r--   0        0        0    12006 2020-02-02 00:00:00.000000 proconip-1.2.4/tests/test_definitions.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 proconip-1.2.4/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 proconip-1.2.4/LICENSE
+-rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 proconip-1.2.4/README.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 proconip-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 proconip-1.2.4/PKG-INFO
```

### Comparing `proconip-1.2.3/CODE_OF_CONDUCT.md` & `proconip-1.2.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `proconip-1.2.3/CONTRIBUTING.md` & `proconip-1.2.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `proconip-1.2.3/.github/workflows/pylint.yml` & `proconip-1.2.4/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `proconip-1.2.3/.github/workflows/python-publish.yml` & `proconip-1.2.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `proconip-1.2.3/.github/workflows/unittest.yml` & `proconip-1.2.4/.github/workflows/unittest.yml`

 * *Files identical despite different names*

### Comparing `proconip-1.2.3/src/proconip/api.py` & `proconip-1.2.4/src/proconip/api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,196 +1,328 @@
 """GetState class to get data from the GetState.csv interface."""
-
-from aiohttp import BasicAuth, ClientSession
+import asyncio
+import socket
+import async_timeout
+
+from aiohttp import (
+    BasicAuth,
+    ClientError,
+    ClientSession,
+)
 from yarl import URL
 
 from .definitions import (
     API_PATH_GET_STATE,
     API_PATH_USRCFG,
     API_PATH_COMMAND,
     BadRelayException,
     ConfigObject,
     DosageTarget,
     GetStateData,
     Relay,
 )
 
 
-async def async_get_raw_state(client_session: ClientSession, config: ConfigObject) -> str:
+async def async_get_raw_state(
+    client_session: ClientSession,
+    config: ConfigObject,
+) -> str:
     """Get raw data (csv string) from the GetState.csv interface."""
     url = URL(config.base_url).with_path(API_PATH_GET_STATE)
-    result = await client_session.get(url,
-                                      auth=BasicAuth(config.username,
-                                                     password=config.password))
-    if result.status in [401, 403]:
-        raise BadCredentialsException
-    if result.status != 200:
-        raise BadStatusCodeException(f"Unexpected status code: {result.status}")
-    return await result.text()
-
-
-async def async_get_state(client_session: ClientSession, config: ConfigObject) -> GetStateData:
+    try:
+        async with async_timeout.timeout(10):
+            response = await client_session.get(
+                url,
+                auth=BasicAuth(
+                    config.username,
+                    password=config.password
+                ),
+            )
+            if response.status in (401, 403):
+                raise BadCredentialsException("Invalid credentials")
+            response.raise_for_status()
+            return await response.text()
+    except asyncio.TimeoutError as exception:
+        raise ProconipApiException(
+            "Timeout error fetching data",
+        ) from exception
+    except (ClientError, socket.gaierror) as exception:
+        raise ProconipApiException(
+            "Error fetching data",
+        ) from exception
+    except Exception as exception:  # pylint: disable=broad-except
+        raise BadStatusCodeException(
+            "Unexpected response",
+        ) from exception
+
+
+async def async_get_state(
+    client_session: ClientSession,
+    config: ConfigObject,
+) -> GetStateData:
     """Get structured data from the GetState.csv interface."""
     raw_data = await async_get_raw_state(client_session, config)
     structured_data = GetStateData(raw_data)
     return structured_data
 
 
 class GetState:
     """GetState class to get data from the GetState.csv interface."""
-    def __init__(self, client_session: ClientSession, config: ConfigObject):
+    def __init__(
+        self,
+        client_session: ClientSession,
+        config: ConfigObject
+    ):
         self.client_session = client_session
         self.config = config
 
-    async def async_get_raw_state(self) -> str:
+    async def async_get_raw_state(
+        self,
+    ) -> str:
         """Get raw data (csv string) from the GetState.csv interface."""
-        return await async_get_raw_state(self.client_session, self.config)
-
-    async def async_get_state(self) -> GetStateData:
+        return await async_get_raw_state(
+            self.client_session,
+            self.config
+        )
+
+    async def async_get_state(
+        self,
+    ) -> GetStateData:
         """Get structured data from the GetState.csv interface."""
-        return await async_get_state(self.client_session, self.config)
+        return await async_get_state(
+            self.client_session,
+            self.config
+        )
+
+
+async def async_post_usrcfg_cgi(
+    client_session: ClientSession,
+    config: ConfigObject,
+    payload: str,
+) -> str:
+    """Send post request to the /usrcfg.cgi endpoint."""
+    url = URL(config.base_url).with_path(API_PATH_USRCFG)
+    try:
+        async with async_timeout.timeout(10):
+            response = await client_session.post(
+                url=url,
+                data=payload,
+                auth=BasicAuth(
+                    login=config.username,
+                    password=config.password,
+                ),
+            )
+            response.raise_for_status()
+            return await response.text()
+    except asyncio.TimeoutError as exception:
+        raise ProconipApiException(
+            "Timeout error fetching data",
+        ) from exception
+    except (ClientError, socket.gaierror) as exception:
+        raise ProconipApiException(
+            "Error fetching data",
+        ) from exception
+    except Exception as exception:  # pylint: disable=broad-except
+        raise BadStatusCodeException(
+            "Unexpected response",
+        ) from exception
 
 
 async def async_switch_on(
         client_session: ClientSession,
         config: ConfigObject,
         current_state: GetStateData,
-        relay: Relay) -> None:
+        relay: Relay,
+) -> str:
     """Switch on a relay using the usrcfg.cgi interface."""
     if current_state.is_dosage_relay(relay):
-        raise BadRelayException
+        raise BadRelayException(
+            "Cannot permanently switch on a dosage relay",
+        )
     bit_state = current_state.determine_overall_relay_bit_state()
     relay_bit_mask = relay.get_bit_mask()
     bit_state[0] |= relay_bit_mask
     bit_state[1] |= relay_bit_mask
-    url = URL(config.base_url).with_path(API_PATH_USRCFG)
-    result = await client_session.post(url,
-                                       data=f"ENA={bit_state[0]},{bit_state[1]}&MANUAL=1",
-                                       auth=BasicAuth(config.username,
-                                                      password=config.password))
-    if result.status in [401, 403]:
-        raise BadCredentialsException
-    if result.status != 200:
-        raise BadStatusCodeException(f"Unexpected status code: {result.status}")
+    return await async_post_usrcfg_cgi(
+        client_session=client_session,
+        config=config,
+        payload=f"ENA={bit_state[0]},{bit_state[1]}&MANUAL=1"
+    )
 
 
 async def async_switch_off(
         client_session: ClientSession,
         config: ConfigObject,
         current_state: GetStateData,
-        relay: Relay) -> None:
+        relay: Relay,
+) -> str:
     """Switch on a relay using the usrcfg.cgi interface."""
     bit_state = current_state.determine_overall_relay_bit_state()
     relay_bit_mask = relay.get_bit_mask()
     bit_state[0] |= relay_bit_mask
     bit_state[1] &= ~relay_bit_mask
-    url = URL(config.base_url).with_path(API_PATH_USRCFG)
-    result = await client_session.post(url,
-                                       data=f"ENA={bit_state[0]},{bit_state[1]}&MANUAL=1",
-                                       auth=BasicAuth(config.username,
-                                                      password=config.password))
-    if result.status in [401, 403]:
-        raise BadCredentialsException
-    if result.status != 200:
-        raise BadStatusCodeException(f"Unexpected status code: {result.status}")
+    return await async_post_usrcfg_cgi(
+        client_session=client_session,
+        config=config,
+        payload=f"ENA={bit_state[0]},{bit_state[1]}&MANUAL=1",
+    )
 
 
 async def async_set_auto_mode(
         client_session: ClientSession,
         config: ConfigObject,
         current_state: GetStateData,
-        relay: Relay) -> None:
+        relay: Relay,
+) -> str:
     """Switch a relay to auto mode using the usrcfg.cgi interface."""
     bit_state = current_state.determine_overall_relay_bit_state()
     relay_bit_mask = relay.get_bit_mask()
     bit_state[0] &= ~relay_bit_mask
     bit_state[1] &= ~relay_bit_mask
-    url = URL(config.base_url).with_path(API_PATH_USRCFG)
-    result = await client_session.post(url,
-                                       data=f"ENA={bit_state[0]},{bit_state[1]}&MANUAL=1",
-                                       auth=BasicAuth(config.username,
-                                                      password=config.password))
-    if result.status in [401, 403]:
-        raise BadCredentialsException
-    if result.status != 200:
-        raise BadStatusCodeException(f"Unexpected status code: {result.status}")
+    return await async_post_usrcfg_cgi(
+        client_session=client_session,
+        config=config,
+        payload=f"ENA={bit_state[0]},{bit_state[1]}&MANUAL=1",
+    )
 
 
 class RelaySwitch:
     """RelaySwitch class to set relay states via usrcfg.cgi interface."""
-    def __init__(self, client_session: ClientSession, config: ConfigObject):
+    def __init__(
+        self,
+        client_session: ClientSession,
+        config: ConfigObject,
+    ):
         self.client_session = client_session
         self.config = config
 
-    async def async_switch_on(self, current_state: GetStateData, relay_id: int) -> None:
+    async def async_switch_on(
+        self,
+        current_state: GetStateData,
+        relay_id: int,
+    ) -> str:
         """Set relay with given id to manual on."""
-        await async_switch_on(self.client_session,
-                              self.config,
-                              current_state,
-                              current_state.get_relay(relay_id))
+        return await async_switch_on(
+            client_session=self.client_session,
+            config=self.config,
+            current_state=current_state,
+            relay=current_state.get_relay(relay_id),
+        )
 
-    async def async_switch_off(self, current_state: GetStateData, relay_id: int) -> None:
+    async def async_switch_off(
+        self,
+        current_state: GetStateData,
+        relay_id: int,
+    ) -> str:
         """Set relay with given id to manual off."""
-        await async_switch_off(self.client_session,
-                               self.config,
-                               current_state,
-                               current_state.get_relay(relay_id))
+        return await async_switch_off(
+            client_session=self.client_session,
+            config=self.config,
+            current_state=current_state,
+            relay=current_state.get_relay(relay_id),
+        )
 
-    async def async_set_auto_mode(self, current_state: GetStateData, relay_id: int) -> None:
+    async def async_set_auto_mode(
+        self,
+        current_state: GetStateData,
+        relay_id: int,
+    ) -> str:
         """Set relay with given id to use auto mode."""
-        await async_set_auto_mode(self.client_session,
-                                  self.config,
-                                  current_state,
-                                  current_state.get_relay(relay_id))
+        return await async_set_auto_mode(
+            client_session=self.client_session,
+            config=self.config,
+            current_state=current_state,
+            relay=current_state.get_relay(relay_id),
+        )
 
 
 async def async_start_dosage(
-        client_session: ClientSession,
-        config: ConfigObject,
-        dosage_target: DosageTarget,
-        dosage_duration: int) -> None:
+    client_session: ClientSession,
+    config: ConfigObject,
+    dosage_target: DosageTarget,
+    dosage_duration: int,
+) -> str:
     """Start manual dosage for given target and duration."""
-    url = URL(config.base_url)\
-        .with_path(API_PATH_COMMAND)\
-        .with_query(f"MAN_DOSAGE={dosage_target},{dosage_duration}")
-    result = await client_session.get(url, auth=BasicAuth(config.username,
-                                                          password=config.password))
-    if result.status in [401, 403]:
-        raise BadCredentialsException
-    if result.status != 200:
-        raise BadStatusCodeException(f"Unexpected status code: {result.status}")
+    query = f"MAN_DOSAGE={dosage_target},{dosage_duration}"
+    url = URL(config.base_url).with_path(API_PATH_COMMAND).with_query(query)
+    try:
+        async with async_timeout.timeout(10):
+            response = await client_session.get(
+                url=url,
+                auth=BasicAuth(
+                    login=config.username,
+                    password=config.password,
+                ),
+            )
+            response.raise_for_status()
+            return await response.text()
+    except asyncio.TimeoutError as exception:
+        raise ProconipApiException(
+            "Timeout error fetching data",
+        ) from exception
+    except (ClientError, socket.gaierror) as exception:
+        raise ProconipApiException(
+            "Error fetching data",
+        ) from exception
+    except Exception as exception:  # pylint: disable=broad-except
+        raise BadStatusCodeException(
+            "Unexpected response",
+        ) from exception
 
 
 class DosageControl:
     """DosageControl class to start manual dosage via Command.htm endpoint."""
-    def __init__(self, client_session: ClientSession, config: ConfigObject):
+    def __init__(
+        self,
+        client_session: ClientSession,
+        config: ConfigObject,
+    ):
         self.client_session = client_session
         self.config = config
 
-    async def async_chlorine_dosage(self, dosage_duration: int) -> None:
+    async def async_chlorine_dosage(
+        self,
+        dosage_duration: int,
+    ) -> str:
         """Start manual chlorine dosage."""
-        await async_start_dosage(self.client_session,
-                                 self.config,
-                                 DosageTarget.CHLORINE,
-                                 dosage_duration)
-
-    async def async_ph_minus_dosage(self, dosage_duration: int) -> None:
+        return await async_start_dosage(
+            client_session=self.client_session,
+            config=self.config,
+            dosage_target=DosageTarget.CHLORINE,
+            dosage_duration=dosage_duration,
+        )
+
+    async def async_ph_minus_dosage(
+        self,
+        dosage_duration: int,
+    ) -> str:
         """Start manual pH minus dosage."""
-        await async_start_dosage(self.client_session,
-                                 self.config,
-                                 DosageTarget.PH_MINUS,
-                                 dosage_duration)
-
-    async def async_ph_plus_dosage(self, dosage_duration: int) -> None:
+        return await async_start_dosage(
+            client_session=self.client_session,
+            config=self.config,
+            dosage_target=DosageTarget.PH_MINUS,
+            dosage_duration=dosage_duration
+        )
+
+    async def async_ph_plus_dosage(
+        self,
+        dosage_duration: int,
+    ) -> None:
         """Start manual pH plus dosage."""
-        await async_start_dosage(self.client_session,
-                                 self.config,
-                                 DosageTarget.PH_PLUS,
-                                 dosage_duration)
+        await async_start_dosage(
+            client_session=self.client_session,
+            config=self.config,
+            dosage_target=DosageTarget.PH_PLUS,
+            dosage_duration=dosage_duration
+        )
+
+
+class ProconipApiException(Exception):
+    """Exception to raise when an api call fails."""
 
 
-class BadCredentialsException(Exception):
+class BadCredentialsException(ProconipApiException):
     """Exception to raise when we get an 401 Unauthorized or 403 Forbidden response."""
 
 
-class BadStatusCodeException(Exception):
+class BadStatusCodeException(ProconipApiException):
     """Exception to raise when we get an unknown response code."""
```

### Comparing `proconip-1.2.3/src/proconip/definitions.py` & `proconip-1.2.4/src/proconip/definitions.py`

 * *Files identical despite different names*

### Comparing `proconip-1.2.3/tests/helper.py` & `proconip-1.2.4/tests/helper.py`

 * *Files identical despite different names*

### Comparing `proconip-1.2.3/tests/test_definitions.py` & `proconip-1.2.4/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `proconip-1.2.3/.gitignore` & `proconip-1.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `proconip-1.2.3/LICENSE` & `proconip-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `proconip-1.2.3/README.md` & `proconip-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `proconip-1.2.3/pyproject.toml` & `proconip-1.2.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "proconip"
-version = "1.2.3"
+version = "1.2.4"
 authors = [
   { name="Yannic Labonte", email="yannic.labonte@gmail.com" },
 ]
 description = "Library for basic interaction with the Procon.IP pool controller unit."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `proconip-1.2.3/PKG-INFO` & `proconip-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proconip
-Version: 1.2.3
+Version: 1.2.4
 Summary: Library for basic interaction with the Procon.IP pool controller unit.
 Project-URL: Homepage, https://github.com/ylabonte/proconip-pypi
 Project-URL: Bug Tracker, https://github.com/ylabonte/proconip-pypi/issues
 Author-email: Yannic Labonte <yannic.labonte@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

