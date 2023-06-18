# Comparing `tmp/oppoudpsdk-0.1.8.tar.gz` & `tmp/oppoudpsdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\oppoudpsdk-0.1.8.tar", last modified: Sun Jul 25 21:07:28 2021, max compression
+gzip compressed data, was "dist\oppoudpsdk-0.1.9.tar", last modified: Sun Jul 25 22:46:31 2021, max compression
```

## Comparing `oppoudpsdk-0.1.8.tar` & `oppoudpsdk-0.1.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2021-07-25 21:07:28.931810 oppoudpsdk-0.1.8/
--rw-rw-rw-   0        0        0     2173 2021-07-25 21:07:28.930811 oppoudpsdk-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1451 2021-07-04 20:29:40.000000 oppoudpsdk-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2021-07-25 21:07:28.854807 oppoudpsdk-0.1.8/oppoudpsdk/
--rw-rw-rw-   0        0        0      290 2021-07-25 21:07:12.000000 oppoudpsdk-0.1.8/oppoudpsdk/__init__.py
--rw-rw-rw-   0        0        0      948 2021-07-25 18:46:04.000000 oppoudpsdk-0.1.8/oppoudpsdk/async_helpers.py
--rw-rw-rw-   0        0        0    10328 2021-07-25 18:30:20.000000 oppoudpsdk-0.1.8/oppoudpsdk/client.py
--rw-rw-rw-   0        0        0     2809 2021-07-04 19:59:42.000000 oppoudpsdk-0.1.8/oppoudpsdk/codes.py
-drwxrwxrwx   0        0        0        0 2021-07-25 21:07:28.916808 oppoudpsdk-0.1.8/oppoudpsdk/command/
--rw-rw-rw-   0        0        0     1318 2021-07-01 20:02:24.000000 oppoudpsdk-0.1.8/oppoudpsdk/command/__init__.py
--rw-rw-rw-   0        0        0     1027 2021-07-25 20:37:48.000000 oppoudpsdk-0.1.8/oppoudpsdk/command/command.py
--rw-rw-rw-   0        0        0     2999 2021-07-06 14:35:01.000000 oppoudpsdk-0.1.8/oppoudpsdk/command/enums.py
--rw-rw-rw-   0        0        0      793 2021-07-02 20:23:37.000000 oppoudpsdk-0.1.8/oppoudpsdk/command/query_command.py
--rw-rw-rw-   0        0        0      412 2021-07-02 20:23:47.000000 oppoudpsdk-0.1.8/oppoudpsdk/command/remote_command.py
--rw-rw-rw-   0        0        0     4275 2021-07-25 20:38:54.000000 oppoudpsdk-0.1.8/oppoudpsdk/command/set_command.py
--rw-rw-rw-   0        0        0     3070 2021-07-04 20:02:27.000000 oppoudpsdk-0.1.8/oppoudpsdk/const.py
--rw-rw-rw-   0        0        0    12731 2021-07-25 20:43:24.000000 oppoudpsdk-0.1.8/oppoudpsdk/device.py
--rw-rw-rw-   0        0        0      913 2021-07-05 00:41:24.000000 oppoudpsdk-0.1.8/oppoudpsdk/exceptions.py
--rw-rw-rw-   0        0        0     2147 2021-06-26 20:16:54.000000 oppoudpsdk-0.1.8/oppoudpsdk/helpers.py
-drwxrwxrwx   0        0        0        0 2021-07-25 21:07:28.928807 oppoudpsdk-0.1.8/oppoudpsdk/response/
--rw-rw-rw-   0        0        0      859 2021-06-30 23:24:57.000000 oppoudpsdk-0.1.8/oppoudpsdk/response/__init__.py
--rw-rw-rw-   0        0        0     4510 2021-07-04 20:14:09.000000 oppoudpsdk-0.1.8/oppoudpsdk/response/enums.py
--rw-rw-rw-   0        0        0     8698 2021-07-25 18:13:49.000000 oppoudpsdk-0.1.8/oppoudpsdk/response/factory.py
--rw-rw-rw-   0        0        0     3375 2021-06-30 23:08:01.000000 oppoudpsdk-0.1.8/oppoudpsdk/response/mapping.py
--rw-rw-rw-   0        0        0     5965 2021-07-25 20:54:52.000000 oppoudpsdk-0.1.8/oppoudpsdk/response/mutator.py
--rw-rw-rw-   0        0        0     6925 2021-07-25 18:05:00.000000 oppoudpsdk-0.1.8/oppoudpsdk/response/response.py
--rw-rw-rw-   0        0        0      274 2021-07-02 20:16:04.000000 oppoudpsdk-0.1.8/oppoudpsdk/states.py
-drwxrwxrwx   0        0        0        0 2021-07-25 21:07:28.906806 oppoudpsdk-0.1.8/oppoudpsdk.egg-info/
--rw-rw-rw-   0        0        0     2173 2021-07-25 21:07:28.000000 oppoudpsdk-0.1.8/oppoudpsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      770 2021-07-25 21:07:28.000000 oppoudpsdk-0.1.8/oppoudpsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-07-25 21:07:28.000000 oppoudpsdk-0.1.8/oppoudpsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2021-07-25 21:07:28.000000 oppoudpsdk-0.1.8/oppoudpsdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2021-07-25 21:07:28.000000 oppoudpsdk-0.1.8/oppoudpsdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-07-25 21:07:28.932811 oppoudpsdk-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1313 2021-06-30 02:15:00.000000 oppoudpsdk-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-07-25 22:46:31.593870 oppoudpsdk-0.1.9/
+-rw-rw-rw-   0        0        0     2173 2021-07-25 22:46:31.592883 oppoudpsdk-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1451 2021-07-04 20:29:40.000000 oppoudpsdk-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2021-07-25 22:46:31.534873 oppoudpsdk-0.1.9/oppoudpsdk/
+-rw-rw-rw-   0        0        0      290 2021-07-25 22:45:58.000000 oppoudpsdk-0.1.9/oppoudpsdk/__init__.py
+-rw-rw-rw-   0        0        0      948 2021-07-25 18:46:04.000000 oppoudpsdk-0.1.9/oppoudpsdk/async_helpers.py
+-rw-rw-rw-   0        0        0    10511 2021-07-25 22:35:35.000000 oppoudpsdk-0.1.9/oppoudpsdk/client.py
+-rw-rw-rw-   0        0        0     2809 2021-07-04 19:59:42.000000 oppoudpsdk-0.1.9/oppoudpsdk/codes.py
+drwxrwxrwx   0        0        0        0 2021-07-25 22:46:31.579870 oppoudpsdk-0.1.9/oppoudpsdk/command/
+-rw-rw-rw-   0        0        0     1318 2021-07-01 20:02:24.000000 oppoudpsdk-0.1.9/oppoudpsdk/command/__init__.py
+-rw-rw-rw-   0        0        0     1027 2021-07-25 20:37:48.000000 oppoudpsdk-0.1.9/oppoudpsdk/command/command.py
+-rw-rw-rw-   0        0        0     2999 2021-07-06 14:35:01.000000 oppoudpsdk-0.1.9/oppoudpsdk/command/enums.py
+-rw-rw-rw-   0        0        0      793 2021-07-02 20:23:37.000000 oppoudpsdk-0.1.9/oppoudpsdk/command/query_command.py
+-rw-rw-rw-   0        0        0      412 2021-07-02 20:23:47.000000 oppoudpsdk-0.1.9/oppoudpsdk/command/remote_command.py
+-rw-rw-rw-   0        0        0     4275 2021-07-25 20:38:54.000000 oppoudpsdk-0.1.9/oppoudpsdk/command/set_command.py
+-rw-rw-rw-   0        0        0     3070 2021-07-04 20:02:27.000000 oppoudpsdk-0.1.9/oppoudpsdk/const.py
+-rw-rw-rw-   0        0        0    12447 2021-07-25 22:44:43.000000 oppoudpsdk-0.1.9/oppoudpsdk/device.py
+-rw-rw-rw-   0        0        0      913 2021-07-05 00:41:24.000000 oppoudpsdk-0.1.9/oppoudpsdk/exceptions.py
+-rw-rw-rw-   0        0        0     2147 2021-06-26 20:16:54.000000 oppoudpsdk-0.1.9/oppoudpsdk/helpers.py
+drwxrwxrwx   0        0        0        0 2021-07-25 22:46:31.590875 oppoudpsdk-0.1.9/oppoudpsdk/response/
+-rw-rw-rw-   0        0        0      859 2021-06-30 23:24:57.000000 oppoudpsdk-0.1.9/oppoudpsdk/response/__init__.py
+-rw-rw-rw-   0        0        0     4510 2021-07-04 20:14:09.000000 oppoudpsdk-0.1.9/oppoudpsdk/response/enums.py
+-rw-rw-rw-   0        0        0     8698 2021-07-25 18:13:49.000000 oppoudpsdk-0.1.9/oppoudpsdk/response/factory.py
+-rw-rw-rw-   0        0        0     3375 2021-06-30 23:08:01.000000 oppoudpsdk-0.1.9/oppoudpsdk/response/mapping.py
+-rw-rw-rw-   0        0        0     5965 2021-07-25 20:54:52.000000 oppoudpsdk-0.1.9/oppoudpsdk/response/mutator.py
+-rw-rw-rw-   0        0        0     6925 2021-07-25 18:05:00.000000 oppoudpsdk-0.1.9/oppoudpsdk/response/response.py
+-rw-rw-rw-   0        0        0      274 2021-07-02 20:16:04.000000 oppoudpsdk-0.1.9/oppoudpsdk/states.py
+drwxrwxrwx   0        0        0        0 2021-07-25 22:46:31.567871 oppoudpsdk-0.1.9/oppoudpsdk.egg-info/
+-rw-rw-rw-   0        0        0     2173 2021-07-25 22:46:31.000000 oppoudpsdk-0.1.9/oppoudpsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      770 2021-07-25 22:46:31.000000 oppoudpsdk-0.1.9/oppoudpsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-07-25 22:46:31.000000 oppoudpsdk-0.1.9/oppoudpsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2021-07-25 22:46:31.000000 oppoudpsdk-0.1.9/oppoudpsdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2021-07-25 22:46:31.000000 oppoudpsdk-0.1.9/oppoudpsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-07-25 22:46:31.593870 oppoudpsdk-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1313 2021-06-30 02:15:00.000000 oppoudpsdk-0.1.9/setup.py
```

### Comparing `oppoudpsdk-0.1.8/PKG-INFO` & `oppoudpsdk-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oppoudpsdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python SDK for Oppo UDP Devices
 Home-page: https://github.com/simbaja/oppoudpsdk
 Author: Jack Simbach
 Author-email: jack.simbach@gmail.com
 License: MIT
 Description: # oppoudpsdk
         Python SDK for Oppo UDP-20x media devices.
```

### Comparing `oppoudpsdk-0.1.8/README.md` & `oppoudpsdk-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `oppoudpsdk-0.1.8/oppoudpsdk/async_helpers.py` & `oppoudpsdk-0.1.9/oppoudpsdk/async_helpers.py`

 * *Files identical despite different names*

### Comparing `oppoudpsdk-0.1.8/oppoudpsdk/client.py` & `oppoudpsdk-0.1.9/oppoudpsdk/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,14 +220,20 @@
       self._writer.close()
       await self._writer.wait_closed()
 
   def _initialize_device(self):
     """Initializes the device (gets power status, and triggers a future initialization)"""
     async def _async_initialize_device():   
       await self.async_send_command(OppoQueryCommand(OppoQueryCode.QPW))
+
+      #force an update if we are on...
+      if self.device.power_status == PowerStatus.ON:
+        await self.device.async_request_update()
+
+      #indicate we're ready to go
       await self.async_event(EVENT_READY, self)
     
     asyncio.ensure_future(_async_initialize_device())
 
   async def _send_command(self, command: OppoCommand):
     """Sends a command to the client (internal)"""
     _LOGGER.debug(f'Sending command: {command}')
```

### Comparing `oppoudpsdk-0.1.8/oppoudpsdk/codes.py` & `oppoudpsdk-0.1.9/oppoudpsdk/codes.py`

 * *Files identical despite different names*

### Comparing `oppoudpsdk-0.1.8/oppoudpsdk/command/__init__.py` & `oppoudpsdk-0.1.9/oppoudpsdk/command/__init__.py`

 * *Files identical despite different names*

### Comparing `oppoudpsdk-0.1.8/oppoudpsdk/command/command.py` & `oppoudpsdk-0.1.9/oppoudpsdk/command/command.py`

 * *Files identical despite different names*

### Comparing `oppoudpsdk-0.1.8/oppoudpsdk/command/enums.py` & `oppoudpsdk-0.1.9/oppoudpsdk/command/enums.py`

 * *Files identical despite different names*

### Comparing `oppoudpsdk-0.1.8/oppoudpsdk/command/query_command.py` & `oppoudpsdk-0.1.9/oppoudpsdk/command/query_command.py`

 * *Files identical despite different names*

### Comparing `oppoudpsdk-0.1.8/oppoudpsdk/command/set_command.py` & `oppoudpsdk-0.1.9/oppoudpsdk/command/set_command.py`

 * *Files identical despite different names*

### Comparing `oppoudpsdk-0.1.8/oppoudpsdk/const.py` & `oppoudpsdk-0.1.9/oppoudpsdk/const.py`

 * *Files identical despite different names*

### Comparing `oppoudpsdk-0.1.8/oppoudpsdk/device.py` & `oppoudpsdk-0.1.9/oppoudpsdk/device.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,15 +88,15 @@
   async def async_request_update(self):
     """Request the device to send a full state update"""
     try:
       #async with self._update_lock:
         #disable individual state events since we're doing a bunch at once
       self._state_events_enabled = False
       await self._client.async_event(EVENT_DEVICE_STATE_UPDATING, self)
-      #await self._client.async_send_command(OppoSetVerboseModeCommand(SetVerboseMode.OFF))
+      await self._client.async_send_command(OppoSetVerboseModeCommand(SetVerboseMode.VERBOSE))
       await self._client.async_send_command(OppoQueryCommand(OppoQueryCode.QVM))
       await self._client.async_send_command(OppoQueryCommand(OppoQueryCode.QPW))
       await self._client.async_send_command(OppoQueryCommand(OppoQueryCode.QVR))
       await self._client.async_send_command(OppoQueryCommand(OppoQueryCode.QVL))
       await self._client.async_send_command(OppoQueryCommand(OppoQueryCode.QHD))
       await self._client.async_send_command(OppoQueryCommand(OppoQueryCode.QPL))
       await self._client.async_send_command(OppoQueryCommand(OppoQueryCode.QDT))
@@ -108,15 +108,14 @@
       await self._client.async_send_command(OppoQueryCommand(OppoQueryCode.QAR))
       await self._client.async_send_command(OppoQueryCdCommand())
 
       #request media-related updates
       await self.async_request_media_update(False)
     finally:
       #re-enable state events and send the updated event
-      #await self._client.async_send_command(OppoSetVerboseModeCommand(SetVerboseMode.VERBOSE))
       self._state_events_enabled = True
       await self._client.async_event(EVENT_DEVICE_STATE_UPDATED, self)
 
   async def async_request_media_update(self, suspend_events: bool = True):
     try:
       if self.is_playing:
         if suspend_events:
@@ -150,27 +149,25 @@
 
   async def async_request_position_update(self):
     """Requests a playback position update"""
     try:
       #async with self._update_lock:      
       self._state_events_enabled = False
       await self._client.async_event(EVENT_DEVICE_STATE_UPDATING, self)
-      #await self._client.async_send_command(OppoSetVerboseModeCommand(SetVerboseMode.OFF))
       await self._client.async_send_command(OppoQueryCommand(OppoQueryCode.QTK))
       await self._client.async_send_command(OppoQueryCommand(OppoQueryCode.QCH))
       await self._client.async_send_command(OppoQueryCommand(OppoQueryCode.QTE))
       await self._client.async_send_command(OppoQueryCommand(OppoQueryCode.QTR))
       await self._client.async_send_command(OppoQueryCommand(OppoQueryCode.QCE))
       await self._client.async_send_command(OppoQueryCommand(OppoQueryCode.QCR))
       await self._client.async_send_command(OppoQueryCommand(OppoQueryCode.QEL))
       await self._client.async_send_command(OppoQueryCommand(OppoQueryCode.QRE))
       self._calculate_duration()
       
     finally:
-      #await self._client.async_send_command(OppoSetVerboseModeCommand(SetVerboseMode.VERBOSE))
       self._state_events_enabled = True
       await self._client.async_event(EVENT_DEVICE_STATE_UPDATED, self)
 
   async def async_send_command(self, code: OppoRemoteCodeType):
     """Sends a remote command to the device"""
     await self._client.async_send_command(OppoRemoteCommand(code))
```

### Comparing `oppoudpsdk-0.1.8/oppoudpsdk/exceptions.py` & `oppoudpsdk-0.1.9/oppoudpsdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `oppoudpsdk-0.1.8/oppoudpsdk/helpers.py` & `oppoudpsdk-0.1.9/oppoudpsdk/helpers.py`

 * *Files identical despite different names*

### Comparing `oppoudpsdk-0.1.8/oppoudpsdk/response/__init__.py` & `oppoudpsdk-0.1.9/oppoudpsdk/response/__init__.py`

 * *Files identical despite different names*

### Comparing `oppoudpsdk-0.1.8/oppoudpsdk/response/enums.py` & `oppoudpsdk-0.1.9/oppoudpsdk/response/enums.py`

 * *Files identical despite different names*

### Comparing `oppoudpsdk-0.1.8/oppoudpsdk/response/factory.py` & `oppoudpsdk-0.1.9/oppoudpsdk/response/factory.py`

 * *Files identical despite different names*

### Comparing `oppoudpsdk-0.1.8/oppoudpsdk/response/mapping.py` & `oppoudpsdk-0.1.9/oppoudpsdk/response/mapping.py`

 * *Files identical despite different names*

### Comparing `oppoudpsdk-0.1.8/oppoudpsdk/response/mutator.py` & `oppoudpsdk-0.1.9/oppoudpsdk/response/mutator.py`

 * *Files identical despite different names*

### Comparing `oppoudpsdk-0.1.8/oppoudpsdk/response/response.py` & `oppoudpsdk-0.1.9/oppoudpsdk/response/response.py`

 * *Files identical despite different names*

### Comparing `oppoudpsdk-0.1.8/oppoudpsdk.egg-info/PKG-INFO` & `oppoudpsdk-0.1.9/oppoudpsdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oppoudpsdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python SDK for Oppo UDP Devices
 Home-page: https://github.com/simbaja/oppoudpsdk
 Author: Jack Simbach
 Author-email: jack.simbach@gmail.com
 License: MIT
 Description: # oppoudpsdk
         Python SDK for Oppo UDP-20x media devices.
```

### Comparing `oppoudpsdk-0.1.8/oppoudpsdk.egg-info/SOURCES.txt` & `oppoudpsdk-0.1.9/oppoudpsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oppoudpsdk-0.1.8/setup.py` & `oppoudpsdk-0.1.9/setup.py`

 * *Files identical despite different names*

