# Comparing `tmp/reolink_aio-0.7.0.tar.gz` & `tmp/reolink_aio-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reolink_aio-0.7.0.tar", last modified: Fri Jun 16 16:48:53 2023, max compression
+gzip compressed data, was "reolink_aio-0.7.1.tar", last modified: Sun Jun 18 09:46:36 2023, max compression
```

## Comparing `reolink_aio-0.7.0.tar` & `reolink_aio-0.7.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 16:48:53.737388 reolink_aio-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-06-16 16:48:43.000000 reolink_aio-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     4571 2023-06-16 16:48:53.737388 reolink_aio-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3763 2023-06-16 16:48:43.000000 reolink_aio-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 16:48:53.733388 reolink_aio-0.7.0/reolink_aio/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-16 16:48:43.000000 reolink_aio-0.7.0/reolink_aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   190984 2023-06-16 16:48:43.000000 reolink_aio-0.7.0/reolink_aio/api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1046 2023-06-16 16:48:43.000000 reolink_aio-0.7.0/reolink_aio/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-06-16 16:48:43.000000 reolink_aio-0.7.0/reolink_aio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     9403 2023-06-16 16:48:43.000000 reolink_aio-0.7.0/reolink_aio/software_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     7930 2023-06-16 16:48:43.000000 reolink_aio-0.7.0/reolink_aio/templates.py
--rw-r--r--   0 runner    (1001) docker     (122)    15190 2023-06-16 16:48:43.000000 reolink_aio-0.7.0/reolink_aio/typings.py
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-06-16 16:48:43.000000 reolink_aio-0.7.0/reolink_aio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 16:48:53.737388 reolink_aio-0.7.0/reolink_aio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4571 2023-06-16 16:48:53.000000 reolink_aio-0.7.0/reolink_aio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      439 2023-06-16 16:48:53.000000 reolink_aio-0.7.0/reolink_aio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 16:48:53.000000 reolink_aio-0.7.0/reolink_aio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 16:48:53.000000 reolink_aio-0.7.0/reolink_aio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-06-16 16:48:53.000000 reolink_aio-0.7.0/reolink_aio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-16 16:48:53.000000 reolink_aio-0.7.0/reolink_aio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 16:48:53.737388 reolink_aio-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1380 2023-06-16 16:48:43.000000 reolink_aio-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 16:48:53.737388 reolink_aio-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    15443 2023-06-16 16:48:43.000000 reolink_aio-0.7.0/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 09:46:36.853476 reolink_aio-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-06-18 09:46:24.000000 reolink_aio-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4571 2023-06-18 09:46:36.853476 reolink_aio-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3763 2023-06-18 09:46:24.000000 reolink_aio-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 09:46:36.853476 reolink_aio-0.7.1/reolink_aio/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-18 09:46:24.000000 reolink_aio-0.7.1/reolink_aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   192151 2023-06-18 09:46:24.000000 reolink_aio-0.7.1/reolink_aio/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1046 2023-06-18 09:46:24.000000 reolink_aio-0.7.1/reolink_aio/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-06-18 09:46:24.000000 reolink_aio-0.7.1/reolink_aio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9403 2023-06-18 09:46:24.000000 reolink_aio-0.7.1/reolink_aio/software_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7935 2023-06-18 09:46:24.000000 reolink_aio-0.7.1/reolink_aio/templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15190 2023-06-18 09:46:24.000000 reolink_aio-0.7.1/reolink_aio/typings.py
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-06-18 09:46:24.000000 reolink_aio-0.7.1/reolink_aio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 09:46:36.853476 reolink_aio-0.7.1/reolink_aio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4571 2023-06-18 09:46:36.000000 reolink_aio-0.7.1/reolink_aio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      439 2023-06-18 09:46:36.000000 reolink_aio-0.7.1/reolink_aio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-18 09:46:36.000000 reolink_aio-0.7.1/reolink_aio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-18 09:46:36.000000 reolink_aio-0.7.1/reolink_aio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-06-18 09:46:36.000000 reolink_aio-0.7.1/reolink_aio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-18 09:46:36.000000 reolink_aio-0.7.1/reolink_aio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-18 09:46:36.853476 reolink_aio-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1380 2023-06-18 09:46:24.000000 reolink_aio-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 09:46:36.853476 reolink_aio-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    15443 2023-06-18 09:46:24.000000 reolink_aio-0.7.1/tests/test.py
```

### Comparing `reolink_aio-0.7.0/LICENSE` & `reolink_aio-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.0/PKG-INFO` & `reolink_aio-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reolink_aio
-Version: 0.7.0
+Version: 0.7.1
 Summary: Reolink NVR/cameras API package
 Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG
 Author-email: starkiller.og@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reolink_aio Version: 0.7.0 Summary: Reolink NVR/
+Metadata-Version: 2.1 Name: reolink_aio Version: 0.7.1 Summary: Reolink NVR/
 cameras API package Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG Author-email: starkiller.og@gmail.com License: MIT
 Platform: any Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier: Topic
 :: Software Development :: Libraries Classifier: Topic :: Home Automation
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `reolink_aio-0.7.0/README.md` & `reolink_aio-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.0/reolink_aio/api.py` & `reolink_aio-0.7.1/reolink_aio/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,16 @@
 MANUFACTURER = "Reolink"
 DEFAULT_STREAM = "sub"
 DEFAULT_PROTOCOL = "rtmp"
 DEFAULT_TIMEOUT = 60
 RETRY_ATTEMPTS = 3
 MAX_CHUNK_ITEMS = 40
 DEFAULT_RTMP_AUTH_METHOD = "PASSWORD"
-SUBSCRIPTION_TERMINATION_TIME = 15
+SUBSCRIPTION_TERMINATION_TIME = 15  # minutes
+LONG_POLL_TIMEOUT = 5  # minutes
 
 MOTION_DETECTION_TYPE = "motion"
 FACE_DETECTION_TYPE = "face"
 PERSON_DETECTION_TYPE = "person"
 VEHICLE_DETECTION_TYPE = "vehicle"
 PET_DETECTION_TYPE = "pet"
 VISITOR_DETECTION_TYPE = "visitor"
@@ -889,14 +890,17 @@
 
         if self.api_version("upgrade") >= 2:
             self._capabilities["Host"].append("update")
 
         if self.api_version("wifi") > 0:
             self._capabilities["Host"].append("wifi")
 
+        if self.api_version("reboot") > 0:
+            self._capabilities["Host"].append("reboot")
+
         # Channel capabilities
         for channel in self._channels:
             self._capabilities[channel] = []
 
             if self.is_nvr and self.api_version("supportAutoTrackStream", channel) > 0:
                 self._capabilities[channel].append("autotrack_stream")
 
@@ -1719,14 +1723,27 @@
             raise NoDataError(f"Host: {self._host}:{self._port}: error obtaining update progress response") from err
 
         if json_data[0]["code"] != 0:
             return False
 
         return json_data[0]["value"]["Status"]["Persent"]
 
+    async def reboot(self) -> None:
+        """Reboot the camera."""
+        if not self.supported(None, "reboot"):
+            raise NotSupportedError(f"Reboot: not supported by {self.nvr_name}")
+
+        body = [{"cmd": "Reboot"}]
+        json_data = await self.send(body, expected_response_type="json")
+
+        if json_data[0]["code"] != 0 or json_data[0].get("value", {}).get("rspCode", -1) != 200:
+            rspCode = json_data[0].get("value", json_data[0]["error"])["rspCode"]
+            detail = json_data[0].get("value", json_data[0]["error"]).get("detail", "")
+            raise ApiError(f"Reboot: API returned error code {json_data[0]['code']}, response code {rspCode}/{detail}")
+
     async def get_snapshot(self, channel: int, stream: Optional[str] = None) -> bytes | None:
         """Get the still image."""
         if channel not in self._stream_channels:
             return None
 
         if stream is None:
             stream = "main"
@@ -3809,15 +3826,15 @@
             "UsernameToken": str(uuid.uuid4()),
             "Username": self._username,
             "PasswordDigest": digest_pwd.decode("utf8"),
             "Nonce": nonce.decode("utf8"),
             "Created": time_created,
         }
 
-    async def subscription_send(self, headers, data) -> str:
+    async def subscription_send(self, headers, data, timeout: aiohttp.ClientTimeout | None = None) -> str:
         """Send subscription data to the camera."""
         if self._subscribe_url is None:
             await self.get_state("GetNetPort")
 
         if self._subscribe_url is None:
             raise NotSupportedError(f"subscription_send: failed to retrieve subscribe_url from {self._host}:{self._port}")
 
@@ -3827,21 +3844,25 @@
             self._port,
             data,
         )
 
         if self._aiohttp_session.closed:
             self._aiohttp_session = self._get_aiohttp_session()
 
+        if timeout is None:
+            timeout = self._timeout
+
         try:
             async with self._send_mutex:
                 response = await self._aiohttp_session.post(
                     url=self._subscribe_url,
                     data=data,
                     headers=headers,
                     allow_redirects=False,
+                    timeout=timeout,
                 )
 
             response_text = await response.text()
             _LOGGER.debug(
                 "Host %s:%s: subscription got response status: %s. Payload:\n%s\n",
                 self._host,
                 self._port,
@@ -4012,22 +4033,27 @@
         if not self.subscribed(SubType.long_poll):
             raise SubscriptionError(f"Host {self._host}:{self._port}: failed to request pull point message, not yet subscribed")
 
         headers = templates.HEADERS
         headers.update(templates.PULLMESSAGE_ACTION)
         template = templates.PULLMESSAGE_XML
 
-        parameters = {"To": self._subscription_manager_url[SubType.long_poll]}
+        parameters = {
+            "To": self._subscription_manager_url[SubType.long_poll],
+            "Timeout": f"PT{LONG_POLL_TIMEOUT}M",
+        }
         parameters.update(await self.get_digest())
 
         xml = template.format(**parameters)
         _LOGGER.debug("Reolink %s requesting ONVIF pull point message", self.nvr_name)
 
+        timeout = aiohttp.ClientTimeout(total=LONG_POLL_TIMEOUT * 60 + 30, connect=self.timeout)
+
         try:
-            response = await self.subscription_send(headers, xml)
+            response = await self.subscription_send(headers, xml, timeout)
         except ReolinkError as err:
             raise SubscriptionError(f"Failed to request pull point message: {str(err)}") from err
 
         root = XML.fromstring(response)
         if root.find(".//{http://docs.oasis-open.org/wsn/b-2}NotificationMessage") is None:
             _LOGGER.debug("Reolink %s received ONVIF pull point message without event", self.nvr_name)
             return []
```

### Comparing `reolink_aio-0.7.0/reolink_aio/enums.py` & `reolink_aio-0.7.1/reolink_aio/enums.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.0/reolink_aio/exceptions.py` & `reolink_aio-0.7.1/reolink_aio/exceptions.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.0/reolink_aio/software_version.py` & `reolink_aio-0.7.1/reolink_aio/software_version.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.0/reolink_aio/templates.py` & `reolink_aio-0.7.1/reolink_aio/templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,13 +118,13 @@
                     <wsse:Nonce EncodingType="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-soap-message-security-1.0#Base64Binary">{Nonce}</wsse:Nonce>
                     <wsu:Created>{Created}</wsu:Created>
                 </wsse:UsernameToken>
             </wsse:Security>
         </soap:Header>
         <soap:Body>
             <wsdl:PullMessages>
-                <wsdl:Timeout>PT1M</wsdl:Timeout>
+                <wsdl:Timeout>{Timeout}</wsdl:Timeout>
                 <wsdl:MessageLimit>100</wsdl:MessageLimit>
             </wsdl:PullMessages>
         </soap:Body>
     </soap:Envelope>
 """
```

### Comparing `reolink_aio-0.7.0/reolink_aio/typings.py` & `reolink_aio-0.7.1/reolink_aio/typings.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.0/reolink_aio/utils.py` & `reolink_aio-0.7.1/reolink_aio/utils.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.0/reolink_aio.egg-info/PKG-INFO` & `reolink_aio-0.7.1/reolink_aio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reolink-aio
-Version: 0.7.0
+Version: 0.7.1
 Summary: Reolink NVR/cameras API package
 Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG
 Author-email: starkiller.og@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reolink-aio Version: 0.7.0 Summary: Reolink NVR/
+Metadata-Version: 2.1 Name: reolink-aio Version: 0.7.1 Summary: Reolink NVR/
 cameras API package Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG Author-email: starkiller.og@gmail.com License: MIT
 Platform: any Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier: Topic
 :: Software Development :: Libraries Classifier: Topic :: Home Automation
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `reolink_aio-0.7.0/setup.py` & `reolink_aio-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(name='reolink_aio',
-      version='0.7.0',
+      version='0.7.1',
       description='Reolink NVR/cameras API package',
       long_description=README,
       long_description_content_type="text/markdown",
       url='https://github.com/starkillerOG/reolink_aio',
       author='starkillerOG',
       author_email='starkiller.og@gmail.com',
       license='MIT',
```

### Comparing `reolink_aio-0.7.0/tests/test.py` & `reolink_aio-0.7.1/tests/test.py`

 * *Files identical despite different names*

