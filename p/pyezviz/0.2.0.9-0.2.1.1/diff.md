# Comparing `tmp/pyezviz-0.2.0.9.tar.gz` & `tmp/pyezviz-0.2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyezviz-0.2.0.9.tar", last modified: Fri Jul  8 18:50:33 2022, max compression
+gzip compressed data, was "pyezviz-0.2.1.1.tar", last modified: Sun Jun 18 10:03:01 2023, max compression
```

## Comparing `pyezviz-0.2.0.9.tar` & `pyezviz-0.2.1.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 18:50:33.619938 pyezviz-0.2.0.9/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-07-08 18:50:26.000000 pyezviz-0.2.0.9/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-07-08 18:50:26.000000 pyezviz-0.2.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-07-08 18:50:33.619938 pyezviz-0.2.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4352 2022-07-08 18:50:26.000000 pyezviz-0.2.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 18:50:33.619938 pyezviz-0.2.0.9/pyezviz/
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-07-08 18:50:26.000000 pyezviz-0.2.0.9/pyezviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12195 2022-07-08 18:50:26.000000 pyezviz-0.2.0.9/pyezviz/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10377 2022-07-08 18:50:26.000000 pyezviz-0.2.0.9/pyezviz/camera.py
--rw-r--r--   0 runner    (1001) docker     (121)     5622 2022-07-08 18:50:26.000000 pyezviz-0.2.0.9/pyezviz/cas.py
--rw-r--r--   0 runner    (1001) docker     (121)    36211 2022-07-08 18:50:26.000000 pyezviz-0.2.0.9/pyezviz/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2187 2022-07-08 18:50:26.000000 pyezviz-0.2.0.9/pyezviz/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      608 2022-07-08 18:50:26.000000 pyezviz-0.2.0.9/pyezviz/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7248 2022-07-08 18:50:26.000000 pyezviz-0.2.0.9/pyezviz/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (121)     4901 2022-07-08 18:50:26.000000 pyezviz-0.2.0.9/pyezviz/test_cam_rtsp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1669 2022-07-08 18:50:26.000000 pyezviz-0.2.0.9/pyezviz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 18:50:33.619938 pyezviz-0.2.0.9/pyezviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-07-08 18:50:33.000000 pyezviz-0.2.0.9/pyezviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      421 2022-07-08 18:50:33.000000 pyezviz-0.2.0.9/pyezviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-08 18:50:33.000000 pyezviz-0.2.0.9/pyezviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-07-08 18:50:33.000000 pyezviz-0.2.0.9/pyezviz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-08 18:50:33.000000 pyezviz-0.2.0.9/pyezviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-07-08 18:50:33.000000 pyezviz-0.2.0.9/pyezviz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-08 18:50:33.619938 pyezviz-0.2.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      809 2022-07-08 18:50:26.000000 pyezviz-0.2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:03:01.527027 pyezviz-0.2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-18 10:03:01.527027 pyezviz-0.2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:03:01.523026 pyezviz-0.2.1.1/pyezviz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/pyezviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/pyezviz/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/pyezviz/api_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/pyezviz/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/pyezviz/cas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53667 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/pyezviz/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/pyezviz/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/pyezviz/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/pyezviz/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/pyezviz/test_cam_rtsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/pyezviz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:03:01.527027 pyezviz-0.2.1.1/pyezviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-18 10:03:01.000000 pyezviz-0.2.1.1/pyezviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-18 10:03:01.000000 pyezviz-0.2.1.1/pyezviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 10:03:01.000000 pyezviz-0.2.1.1/pyezviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-18 10:03:01.000000 pyezviz-0.2.1.1/pyezviz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-18 10:03:01.000000 pyezviz-0.2.1.1/pyezviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 10:03:01.000000 pyezviz-0.2.1.1/pyezviz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 10:03:01.527027 pyezviz-0.2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/setup.py
```

### Comparing `pyezviz-0.2.0.9/LICENSE.md` & `pyezviz-0.2.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.0.9/README.md` & `pyezviz-0.2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.0.9/pyezviz/__init__.py` & `pyezviz-0.2.1.1/pyezviz/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 """init pyezviz."""
 from .camera import EzvizCamera
 from .cas import EzvizCAS
 from .client import EzvizClient
-from .constants import DefenseModeType, DeviceCatagories, DeviceSwitchType, SoundMode
+from .constants import (
+    BatteryCameraWorkMode,
+    DefenseModeType,
+    DeviceCatagories,
+    DeviceSwitchType,
+    IntelligentDetectionMode,
+    MessageFilterType,
+    NightVisionMode,
+    SoundMode,
+    SupportExt,
+)
 from .exceptions import (
     AuthTestResultFailed,
     EzvizAuthTokenExpired,
     EzvizAuthVerificationCode,
     HTTPError,
     InvalidHost,
     InvalidURL,
@@ -24,12 +34,17 @@
     "InvalidHost",
     "AuthTestResultFailed",
     "EzvizAuthTokenExpired",
     "EzvizAuthVerificationCode",
     "EzvizCAS",
     "MQTTClient",
     "DefenseModeType",
+    "IntelligentDetectionMode",
+    "BatteryCameraWorkMode",
+    "NightVisionMode",
+    "MessageFilterType",
     "DeviceCatagories",
     "DeviceSwitchType",
+    "SupportExt",
     "SoundMode",
     "TestRTSPAuth",
 ]
```

### Comparing `pyezviz-0.2.0.9/pyezviz/__main__.py` & `pyezviz-0.2.1.1/pyezviz/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,16 @@
 from typing import Any
 
 import pandas
 
 from .camera import EzvizCamera
 from .client import EzvizClient
 from .constants import DefenseModeType
+from .exceptions import EzvizAuthVerificationCode
 from .mqtt import MQTTClient
-from .exceptions import (
-    EzvizAuthVerificationCode,
-)
 
 
 def main() -> Any:
     """Initiate arg parser."""
     parser = argparse.ArgumentParser(prog="pyezviz")
     parser.add_argument("-u", "--username", required=True, help="Ezviz username")
     parser.add_argument("-p", "--password", required=True, help="Ezviz Password")
@@ -265,14 +263,17 @@
             except Exception as exp:  # pylint: disable=broad-except
                 print(exp)
             finally:
                 client.close_session()
 
     elif args.action == "mqtt":
 
+        logging.basicConfig()
+        logging.getLogger().setLevel(logging.DEBUG)
+
         try:
             token = client.login()
             mqtt = MQTTClient(token)
             mqtt.start()
 
         except Exception as exp:  # pylint: disable=broad-except
             print(exp)
```

### Comparing `pyezviz-0.2.0.9/pyezviz/camera.py` & `pyezviz-0.2.1.1/pyezviz/camera.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """pyezviz camera api."""
 from __future__ import annotations
 
 import datetime
 from typing import TYPE_CHECKING, Any
 
-from .constants import DeviceCatagories, DeviceSwitchType, SoundMode
+from .constants import DeviceSwitchType, SoundMode
 from .exceptions import PyEzvizError
 
 if TYPE_CHECKING:
     from .client import EzvizClient
 
 
 class EzvizCamera:
@@ -29,35 +29,14 @@
         )
         self._last_alarm: dict[str, Any] = {}
         self._switch: dict[int, bool] = {
             switch["type"]: switch["enable"]
             for switch in self._device.get("SWITCH", {})
         }
 
-    def _detection_sensibility(self) -> Any:
-        """Load detection sensitivity."""
-        result = "Unknown"
-
-        if self._switch.get(DeviceSwitchType.AUTO_SLEEP.value) is not True:
-            if (
-                self._device["deviceInfos"]["deviceCategory"]
-                == DeviceCatagories.BATTERY_CAMERA_DEVICE_CATEGORY.value
-            ):
-                result = self._client.get_detection_sensibility(
-                    self._serial,
-                    "3",
-                )
-            else:
-                result = self._client.get_detection_sensibility(self._serial)
-
-        if self._switch.get(DeviceSwitchType.AUTO_SLEEP.value) is True:
-            result = "Hibernate"
-
-        return result
-
     def _alarm_list(self) -> None:
         """Get last alarm info for this camera's self._serial."""
         _alarmlist = self._client.get_alarminfo(self._serial)
 
         if _alarmlist["page"].get("totalResults") > 0:
             self._last_alarm = _alarmlist["alarms"][0]
             return self._motion_trigger()
@@ -131,44 +110,65 @@
             "audio": self._switch.get(DeviceSwitchType.SOUND.value),
             "ir_led": self._switch.get(DeviceSwitchType.INFRARED_LIGHT.value),
             "state_led": self._switch.get(DeviceSwitchType.LIGHT.value),
             "upgrade_percent": self._device["STATUS"].get("upgradeProcess"),
             "upgrade_in_progress": bool(
                 self._device["STATUS"].get("upgradeStatus") == 0
             ),
+            "latest_firmware_info": self._device["UPGRADE"].get("upgradePackageInfo"),
             "follow_move": self._switch.get(DeviceSwitchType.MOBILE_TRACKING.value),
             "alarm_notify": bool(self._device["STATUS"].get("globalStatus")),
             "alarm_schedules_enabled": self._is_alarm_schedules_enabled(),
             "alarm_sound_mod": SoundMode(
-                self._device["STATUS"].get("alarmSoundMode")
+                self._device["STATUS"].get("alarmSoundMode", -1)
             ).name,
             "encrypted": bool(self._device["STATUS"].get("isEncrypt")),
+            "encrypted_pwd_hash": self._device["STATUS"].get("encryptPwd"),
             "local_ip": self._local_ip(),
             "wan_ip": self._device["CONNECTION"].get("netIp"),
             "mac_address": self._device["deviceInfos"].get("mac"),
             "local_rtsp_port": self._device["CONNECTION"].get("localRtspPort", "554")
             if self._device["CONNECTION"].get("localRtspPort", "554") != 0
             else "554",
             "supported_channels": self._device["deviceInfos"].get("channelNumber"),
-            "detection_sensibility": self._detection_sensibility(),
             "battery_level": self._device["STATUS"]
             .get("optionals", {})
             .get("powerRemaining"),
+            "battery_camera_work_mode": self._device["STATUS"]
+            .get("optionals", {})
+            .get("batteryCameraWorkMode"),
+            "Alarm_DetectHumanCar": self._device["STATUS"]
+            .get("optionals", {})
+            .get("Alarm_DetectHumanCar"),
+            "NightVision_Model": self._device["STATUS"]
+            .get("optionals", {})
+            .get("NightVision_Model"),
             "PIR_Status": self._device["STATUS"].get("pirStatus"),
             "Motion_Trigger": self._alarmmotiontrigger.get("alarm_trigger_active"),
             "Seconds_Last_Trigger": self._alarmmotiontrigger.get("timepassed"),
             "last_alarm_time": self._last_alarm.get("alarmStartTimeStr"),
             "last_alarm_pic": self._last_alarm.get(
                 "picUrl",
                 "https://eustatics.ezvizlife.com/ovs_mall/web/img/index/EZVIZ_logo.png?ver=3007907502",
             ),
             "last_alarm_type_code": self._last_alarm.get("alarmType", "0000"),
             "last_alarm_type_name": self._last_alarm.get("sampleName", "NoAlarm"),
+            "alarm_light_luminance": int(
+                "".join(
+                    filter(
+                        str.isdigit,
+                        self._device["STATUS"]
+                        .get("optionals", {})
+                        .get("Alarm_Light", "0"),
+                    )
+                )
+            ),  # extract the value from the string and cater for the case where the value is not set.
             "wifiInfos": self._device.get("WIFI"),
             "switches": self._switch,
+            "supportExt": self._device["deviceInfos"]["supportExt"],
         }
 
     def move(self, direction: str, speed: int = 5) -> bool:
         """Move camera."""
         if direction not in ["right", "left", "down", "up"]:
             raise PyEzvizError(f"Invalid direction: {direction} ")
```

### Comparing `pyezviz-0.2.0.9/pyezviz/cas.py` & `pyezviz-0.2.1.1/pyezviz/cas.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.0.9/pyezviz/client.py` & `pyezviz-0.2.1.1/pyezviz/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,73 @@
 """Ezviz API."""
 from __future__ import annotations
 
+from datetime import datetime
 import hashlib
+import json
 import logging
 from typing import Any
+import urllib.parse
 from uuid import uuid4
 
 import requests
 
+from .api_endpoints import (
+    API_ENDPOINT_ALARM_SOUND,
+    API_ENDPOINT_ALARMINFO_GET,
+    API_ENDPOINT_CAM_ENCRYPTKEY,
+    API_ENDPOINT_CANCEL_ALARM,
+    API_ENDPOINT_CREATE_PANORAMIC,
+    API_ENDPOINT_DETECTION_SENSIBILITY,
+    API_ENDPOINT_DETECTION_SENSIBILITY_GET,
+    API_ENDPOINT_DEVCONFIG_BY_KEY,
+    API_ENDPOINT_DEVICES,
+    API_ENDPOINT_DO_NOT_DISTURB,
+    API_ENDPOINT_GROUP_DEFENCE_MODE,
+    API_ENDPOINT_LOGIN,
+    API_ENDPOINT_LOGOUT,
+    API_ENDPOINT_PAGELIST,
+    API_ENDPOINT_PANORAMIC_DEVICES_OPERATION,
+    API_ENDPOINT_PTZCONTROL,
+    API_ENDPOINT_REFRESH_SESSION_ID,
+    API_ENDPOINT_RETURN_PANORAMIC,
+    API_ENDPOINT_SEND_CODE,
+    API_ENDPOINT_SERVER_INFO,
+    API_ENDPOINT_SET_DEFENCE_SCHEDULE,
+    API_ENDPOINT_SET_LUMINANCE,
+    API_ENDPOINT_SWITCH_DEFENCE_MODE,
+    API_ENDPOINT_SWITCH_SOUND_ALARM,
+    API_ENDPOINT_SWITCH_STATUS,
+    API_ENDPOINT_UNIFIEDMSG_LIST_GET,
+    API_ENDPOINT_UPGRADE_DEVICE,
+    API_ENDPOINT_USER_ID,
+    API_ENDPOINT_V3_ALARMS,
+    API_ENDPOINT_VIDEO_ENCRYPT,
+)
 from .camera import EzvizCamera
 from .cas import EzvizCAS
 from .constants import (
     DEFAULT_TIMEOUT,
     FEATURE_CODE,
     MAX_RETRIES,
     REQUEST_HEADER,
     DefenseModeType,
     DeviceCatagories,
+    MessageFilterType,
 )
 from .exceptions import (
     EzvizAuthTokenExpired,
     EzvizAuthVerificationCode,
     HTTPError,
     InvalidURL,
     PyEzvizError,
 )
 
 _LOGGER = logging.getLogger(__name__)
 
-API_ENDPOINT_CLOUDDEVICES = "/api/cloud/v2/cloudDevices/getAll"
-API_ENDPOINT_PAGELIST = "/v3/userdevices/v1/resources/pagelist"
-API_ENDPOINT_DEVICES = "/v3/devices/"
-API_ENDPOINT_LOGIN = "/v3/users/login/v5"
-API_ENDPOINT_REFRESH_SESSION_ID = "/v3/apigateway/login"
-API_ENDPOINT_SWITCH_STATUS = "/switchStatus"
-API_ENDPOINT_PTZCONTROL = "/ptzControl"
-API_ENDPOINT_ALARM_SOUND = "/alarm/sound"
-API_ENDPOINT_DETECTION_SENSIBILITY = "/api/device/configAlgorithm"
-API_ENDPOINT_DETECTION_SENSIBILITY_GET = "/api/device/queryAlgorithmConfig"
-API_ENDPOINT_ALARMINFO_GET = "/v3/alarms/v2/advanced"
-API_ENDPOINT_SET_DEFENCE_SCHEDULE = "/api/device/defence/plan2"
-API_ENDPOINT_SWITCH_DEFENCE_MODE = "/v3/userdevices/v1/group/switchDefenceMode"
-API_ENDPOINT_SWITCH_SOUND_ALARM = "/sendAlarm"
-API_ENDPOINT_SERVER_INFO = "/v3/configurations/system/info"
-API_ENDPOINT_LOGOUT = "/v3/users/logout/v2"
-API_ENDPOINT_PANORAMIC_DEVICES_OPERATION = "/v3/panoramicDevices/operation"
-API_ENDPOINT_UPGRADE_DEVICE = "/v3/upgrades/v1/devices/"
-API_ENDPOINT_SEND_CODE = "/v3/sms/nologin/checkcode"
-
-API_ENDPOINT_V3_ALARMS = "/v3/alarms/"
-API_ENDPOINT_DO_NOT_DISTURB = "/1/nodisturb"
-
 
 class EzvizClient:
     """Initialize api client object."""
 
     def __init__(
         self,
         account: str | None = None,
@@ -64,17 +77,17 @@
         token: dict | None = None,
     ) -> None:
         """Initialize the client object."""
         self.account = account
         self.password = (
             hashlib.md5(password.encode("utf-8")).hexdigest() if password else None
         )  # Ezviz API sends md5 of password
-        self._session = None
-        self.close_session()
-        self._session.headers["sessionId"] = token.get("session_id") if token else None
+        self._session = requests.session()
+        self._session.headers.update(REQUEST_HEADER)
+        self._session.headers["sessionId"] = token["session_id"] if token else None
         self._token = token or {
             "session_id": None,
             "rf_session_id": None,
             "username": None,
             "api_url": url,
         }
         self._timeout = timeout
@@ -189,15 +202,15 @@
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
-        if json_output.get("meta").get("code") != 200:
+        if json_output["meta"].get("code") != 200:
             raise PyEzvizError(
                 f"Could not request MFA code: Got {req.status_code} : {req.text})"
             )
 
         return True
 
     def get_service_urls(self) -> Any:
@@ -229,15 +242,15 @@
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
-        if json_output.get("meta").get("code") != 200:
+        if json_output["meta"].get("code") != 200:
             raise PyEzvizError(f"Error getting Service URLs: {json_output['meta']}")
 
         service_urls = json_output["systemConfigInfo"]
         service_urls["sysConf"] = service_urls["sysConf"].split("|")
 
         return service_urls
 
@@ -279,15 +292,15 @@
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
-        if json_output.get("meta").get("code") != 200:
+        if json_output["meta"].get("code") != 200:
             # session is wrong, need to relogin
             self.login()
             logging.info(
                 "Json request error, relogging (max retries: %s)", str(max_retries)
             )
             return self._api_get_pagelist(page_filter, json_key, max_retries + 1)
 
@@ -303,16 +316,16 @@
                 "Impossible to load the devices, here is the returned response: %s",
                 str(req.text),
             )
             return self._api_get_pagelist(page_filter, json_key, max_retries + 1)
 
         return json_result
 
-    def get_alarminfo(self, serial: str, limit: int = 1, max_retries: int = 0) -> Any:
-        """Get data from alarm info API."""
+    def get_alarminfo(self, serial: str, limit: int = 1, max_retries: int = 0) -> dict:
+        """Get data from alarm info API for camera serial."""
         if max_retries > MAX_RETRIES:
             raise PyEzvizError("Can't gather proper data. Max retries exceeded.")
 
         params: dict[str, int | str] = {
             "deviceSerials": serial,
             "queryType": -1,
             "limit": limit,
@@ -336,24 +349,92 @@
 
             raise HTTPError from err
 
         if req.text == "":
             raise PyEzvizError("No data")
 
         try:
-            json_output = req.json()
+            json_output: dict = req.json()
 
         except ValueError as err:
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
+        if json_output["meta"].get("code") != 200:
+            raise PyEzvizError(
+                f"Could not get data from alarm api: Got {json_output['meta']})"
+            )
+
+        return json_output
+
+    def get_device_messages_list(
+        self,
+        serials: str | None = None,
+        s_type: int = MessageFilterType.FILTER_TYPE_ALL_ALARM.value,
+        limit: int | None = 20,  # 50 is the max even if you set it higher
+        date: str = datetime.today().strftime("%Y%m%d"),
+        end_time: str | None = None,
+        tags: str = "ALL",
+        max_retries: int = 0,
+    ) -> dict:
+        """Get data from Unified message list API."""
+        if max_retries > MAX_RETRIES:
+            raise PyEzvizError("Can't gather proper data. Max retries exceeded.")
+
+        params: dict[str, int | str | None] = {
+            "serials:": serials,
+            "stype": s_type,
+            "limit": limit,
+            "date": date,
+            "endTime": end_time,
+            "tags": tags,
+        }
+
+        try:
+            req = self._session.get(
+                "https://" + self._token["api_url"] + API_ENDPOINT_UNIFIEDMSG_LIST_GET,
+                params=params,
+                timeout=self._timeout,
+            )
+
+            req.raise_for_status()
+
+        except requests.HTTPError as err:
+            if err.response.status_code == 401:
+                # session is wrong, need to relogin
+                self.login()
+                return self.get_device_messages_list(
+                    serials, s_type, limit, date, end_time, tags, max_retries + 1
+                )
+
+            raise HTTPError from err
+
+        if req.text == "":
+            raise PyEzvizError("No data")
+
+        try:
+            json_output: dict = req.json()
+
+        except ValueError as err:
+            raise PyEzvizError(
+                "Impossible to decode response: "
+                + str(err)
+                + "\nResponse was: "
+                + str(req.text)
+            ) from err
+
+        if json_output["meta"].get("code") != 200:
+            raise PyEzvizError(
+                f"Could not get unified message list: Got {json_output['meta']})"
+            )
+
         return json_output
 
     def _switch_status(
         self, serial: str, status_type: int, enable: int, max_retries: int = 0
     ) -> bool:
         """Switch status on a device."""
         if max_retries > MAX_RETRIES:
@@ -394,17 +475,96 @@
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
-        if json_output.get("meta").get("code") != 200:
+        if json_output["meta"].get("code") != 200:
+            raise PyEzvizError(f"Could not set the switch: Got {json_output})")
+
+        return True
+
+    def set_battery_camera_work_mode(self, serial: str, value: int) -> bool:
+        """Set battery camera work mode."""
+        return self.set_device_config_by_key(serial, value, key="batteryCameraWorkMode")
+
+    def set_detection_mode(self, serial: str, value: int) -> bool:
+        """Set detection mode."""
+        return self.set_device_config_by_key(
+            serial, value=f'{{"type":{value}}}', key="Alarm_DetectHumanCar"
+        )
+
+    def set_night_vision_mode(
+        self, serial: str, mode: int, luminance: int = 100
+    ) -> bool:
+        """Set night vision mode."""
+        return self.set_device_config_by_key(
+            serial,
+            value=f'{{"graphicType":{mode},"luminance":{luminance}}}',
+            key="NightVision_Model",
+        )
+
+    def set_device_config_by_key(
+        self,
+        serial: str,
+        value: Any,
+        key: str = "batteryCameraWorkMode",
+        max_retries: int = 0,
+    ) -> bool:
+        """Change value on device by setting key."""
+        if max_retries > MAX_RETRIES:
+            raise PyEzvizError("Can't gather proper data. Max retries exceeded.")
+
+        params = {"key": key, "value": value}
+        params_str = urllib.parse.urlencode(
+            params, safe="}{:"
+        )  # not encode curly braces and colon
+
+        full_url = f'https://{self._token["api_url"]}{API_ENDPOINT_DEVCONFIG_BY_KEY}{serial}/1/op'
+
+        # EZVIZ api request needs {}: in the url, but requests lib doesn't allow it
+        # so we need to manually prepare it
+        req_prep = requests.Request(
+            method="PUT", url=full_url, headers=self._session.headers
+        ).prepare()
+        req_prep.url = full_url + "?" + params_str
+
+        try:
+            req = self._session.send(
+                request=req_prep,
+                timeout=self._timeout,
+            )
+
+            req.raise_for_status()
+
+        except requests.HTTPError as err:
+            if err.response.status_code == 401:
+                # session is wrong, need to relogin
+                self.login()
+                return self.set_device_config_by_key(
+                    serial, value, key, max_retries + 1
+                )
+
+            raise HTTPError from err
+
+        try:
+            json_output = req.json()
+
+        except ValueError as err:
+            raise PyEzvizError(
+                "Impossible to decode response: "
+                + str(err)
+                + "\nResponse was: "
+                + str(req.text)
+            ) from err
+
+        if json_output["meta"].get("code") != 200:
             raise PyEzvizError(
-                f"Could not set the switch: Got {req.status_code} : {req.text})"
+                f"Could not set camera work mode: Got {json_output['meta']})"
             )
 
         return True
 
     def upgrade_device(self, serial: str, max_retries: int = 0) -> bool:
         """Upgrade device firmware."""
         if max_retries > MAX_RETRIES:
@@ -437,15 +597,15 @@
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
-        if json_output.get("meta").get("code") != 200:
+        if json_output["meta"].get("code") != 200:
             raise PyEzvizError(
                 f"Could not initiate firmare upgrade: Got {req.status_code} : {req.text})"
             )
 
         return True
 
     def sound_alarm(self, serial: str, enable: int = 1, max_retries: int = 0) -> bool:
@@ -484,21 +644,221 @@
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
-        if json_output.get("meta").get("code") != 200:
+        if json_output["meta"].get("code") != 200:
             raise PyEzvizError(
                 f"Could not set the alarm sound: Got {req.status_code} : {req.text})"
             )
 
         return True
 
+    def get_user_id(self, max_retries: int = 0) -> Any:
+        """Get Ezviz userid, used by restricted api endpoints."""
+
+        if max_retries > MAX_RETRIES:
+            raise PyEzvizError("Can't gather proper data. Max retries exceeded.")
+
+        try:
+            req = self._session.get(
+                f"https://{self._token['api_url']}{API_ENDPOINT_USER_ID}",
+                timeout=self._timeout,
+            )
+            req.raise_for_status()
+
+        except requests.HTTPError as err:
+            if err.response.status_code == 401:
+                # session is wrong, need to relogin
+                self.login()
+                return self.get_user_id(max_retries + 1)
+
+            raise HTTPError from err
+
+        try:
+            json_output = req.json()
+
+        except ValueError as err:
+            raise PyEzvizError(
+                "Impossible to decode response: "
+                + str(err)
+                + "\nResponse was: "
+                + str(req.text)
+            ) from err
+
+        if json_output["meta"].get("code") != 200:
+            raise PyEzvizError(
+                f"Could not set video encryption: Got {json_output['meta']})"
+            )
+
+        return json_output["deviceTokenInfo"]
+
+    def set_video_enc(
+        self,
+        serial: str,
+        enable: int = 1,
+        camera_verification_code: str | None = None,
+        new_password: str | None = None,
+        old_password: str | None = None,
+        max_retries: int = 0,
+    ) -> bool:
+        """Enable or Disable video encryption."""
+        if max_retries > MAX_RETRIES:
+            raise PyEzvizError("Can't gather proper data. Max retries exceeded.")
+
+        device_token_info = self.get_user_id()
+        cookies = {
+            "clientType": "3",
+            "clientVersion": "5.12.1.0517",
+            "userId": device_token_info["userId"],
+            "ASG_DisplayName": "home",
+            "C_SS": self._session.headers["sessionId"],
+            "lang": "en_US",
+        }
+
+        try:
+            req = self._session.put(
+                "https://"
+                + self._token["api_url"]
+                + API_ENDPOINT_DEVICES
+                + API_ENDPOINT_VIDEO_ENCRYPT,
+                data={
+                    "deviceSerial": serial,
+                    "isEncrypt": enable,
+                    "oldPassword": old_password,
+                    "password": new_password,
+                    "featureCode": FEATURE_CODE,
+                    "validateCode": camera_verification_code,
+                    "msgType": -1,
+                },
+                cookies=cookies,
+                timeout=self._timeout,
+            )
+
+            req.raise_for_status()
+
+        except requests.HTTPError as err:
+            if err.response.status_code == 401:
+                # session is wrong, need to relogin
+                self.login()
+                return self.set_video_enc(
+                    serial,
+                    enable,
+                    camera_verification_code,
+                    new_password,
+                    old_password,
+                    max_retries + 1,
+                )
+
+            raise HTTPError from err
+
+        try:
+            json_output = req.json()
+
+        except ValueError as err:
+            raise PyEzvizError(
+                "Impossible to decode response: "
+                + str(err)
+                + "\nResponse was: "
+                + str(req.text)
+            ) from err
+
+        if json_output["meta"].get("code") != 200:
+            raise PyEzvizError(
+                f"Could not set video encryption: Got {json_output['meta']})"
+            )
+
+        return True
+
+    def get_group_defence_mode(self, max_retries: int = 0) -> Any:
+        """Get group arm status. The alarm arm/disarm concept on 1st page of app."""
+
+        if max_retries > MAX_RETRIES:
+            raise PyEzvizError("Can't gather proper data. Max retries exceeded.")
+
+        try:
+            req = self._session.get(
+                "https://" + self._token["api_url"] + API_ENDPOINT_GROUP_DEFENCE_MODE,
+                params={
+                    "groupId": -1,
+                },
+                timeout=self._timeout,
+            )
+
+            req.raise_for_status()
+
+        except requests.HTTPError as err:
+            if err.response.status_code == 401:
+                # session is wrong, need to relogin
+                self.login()
+                return self.get_group_defence_mode(max_retries + 1)
+
+            raise HTTPError from err
+
+        try:
+            json_output = req.json()
+
+        except ValueError as err:
+            raise PyEzvizError(
+                "Impossible to decode response: "
+                + str(err)
+                + "\nResponse was: "
+                + str(req.text)
+            ) from err
+
+        if json_output["meta"].get("code") != 200:
+            raise PyEzvizError(
+                f"Could not get group defence status: Got {json_output['meta']})"
+            )
+
+        return json_output["mode"]
+
+    # Not tested
+    def cancel_alarm_device(self, serial: str, max_retries: int = 0) -> bool:
+        """Cacnel alarm on an Alarm device."""
+        if max_retries > MAX_RETRIES:
+            raise PyEzvizError("Can't gather proper data. Max retries exceeded.")
+
+        try:
+            req = self._session.post(
+                "https://" + self._token["api_url"] + API_ENDPOINT_CANCEL_ALARM,
+                data={"subSerial": serial},
+                timeout=self._timeout,
+            )
+
+            req.raise_for_status()
+
+        except requests.HTTPError as err:
+            if err.response.status_code == 401:
+                # session is wrong, need to relogin
+                self.login()
+                return self.sound_alarm(serial, max_retries + 1)
+
+            raise HTTPError from err
+
+        try:
+            json_output = req.json()
+
+        except ValueError as err:
+            raise PyEzvizError(
+                "Impossible to decode response: "
+                + str(err)
+                + "\nResponse was: "
+                + str(req.text)
+            ) from err
+
+        if json_output["meta"].get("code") != 200:
+            raise PyEzvizError(
+                f"Could not cancel alarm siren: Got {req.status_code} : {req.text})"
+            )
+
+        return True
+
     def load_cameras(self) -> dict[Any, Any]:
         """Load and return all cameras objects."""
 
         devices = self.get_device_infos()
         supported_categories = [
             DeviceCatagories.COMMON_DEVICE_CATEGORY.value,
             DeviceCatagories.CAMERA_DEVICE_CATEGORY.value,
@@ -531,15 +891,15 @@
         result: dict[str, Any] = {}
         _res_id = "NONE"
 
         for device in devices["deviceInfos"]:
             _serial = device["deviceSerial"]
             _res_id_list = {
                 item
-                for item in devices.get("CLOUD", {}).keys()
+                for item in devices.get("CLOUD", {})
                 if devices["CLOUD"][item].get("deviceSerial") == _serial
             }
             _res_id = _res_id_list.pop() if len(_res_id_list) else "NONE"
 
             result[_serial] = {
                 "CLOUD": {_res_id: devices.get("CLOUD", {}).get(_res_id, {})},
                 "VTM": {_res_id: devices.get("VTM", {}).get(_res_id, {})},
@@ -563,14 +923,18 @@
                     item
                     for item in devices.get("resourceInfos")
                     if item.get("deviceSerial") == _serial
                 ],  # Could be more than one
                 "WIFI": devices.get("WIFI", {}).get(_serial, {}),
                 "deviceInfos": device,
             }
+            # Nested keys are still encoded as JSON strings
+            result[_serial]["deviceInfos"]["supportExt"] = json.loads(
+                result[_serial]["deviceInfos"]["supportExt"]
+            )
 
         if not serial:
             return result
 
         return result.get(serial, {})
 
     def ptz_control(
@@ -603,14 +967,152 @@
             req.raise_for_status()
 
         except requests.HTTPError as err:
             raise HTTPError from err
 
         return req.text
 
+    def get_cam_key(
+        self, serial: str, smscode: int | None = None, max_retries: int = 0
+    ) -> Any:
+        """Get Camera encryption key."""
+
+        if max_retries > MAX_RETRIES:
+            raise PyEzvizError("Can't gather proper data. Max retries exceeded.")
+
+        try:
+            req = self._session.post(
+                "https://" + self._token["api_url"] + API_ENDPOINT_CAM_ENCRYPTKEY,
+                data={
+                    "checkcode": smscode,
+                    "serial": serial,
+                    "clientNo": "web_site",
+                    "clientType": 3,
+                    "netType": "WIFI",
+                    "featureCode": FEATURE_CODE,
+                    "sessionId": self._token["session_id"],
+                },
+                timeout=self._timeout,
+            )
+
+            req.raise_for_status()
+
+        except requests.HTTPError as err:
+            if err.response.status_code == 401:
+                # session is wrong, need to relogin
+                self.login()
+                return self.get_cam_key(serial, smscode, max_retries + 1)
+
+            raise HTTPError from err
+
+        try:
+            json_output = req.json()
+
+        except ValueError as err:
+            raise PyEzvizError(
+                "Impossible to decode response: "
+                + str(err)
+                + "\nResponse was: "
+                + str(req.text)
+            ) from err
+
+        if json_output.get("resultCode") == "20002":
+            raise PyEzvizError(
+                f"MFA code required: Got {req.status_code} : {req.text})"
+            )
+
+        if json_output.get("resultCode") != "0":
+            raise PyEzvizError(
+                f"Could not get camera encryption key: Got {req.status_code} : {req.text})"
+            )
+
+        return json_output
+
+    def create_panoramic(self, serial: str, max_retries: int = 0) -> Any:
+        """Create panoramic image."""
+
+        if max_retries > MAX_RETRIES:
+            raise PyEzvizError("Can't gather proper data. Max retries exceeded.")
+
+        try:
+            req = self._session.post(
+                "https://" + self._token["api_url"] + API_ENDPOINT_CREATE_PANORAMIC,
+                data={"deviceSerial": serial},
+                timeout=self._timeout,
+            )
+
+            req.raise_for_status()
+
+        except requests.HTTPError as err:
+            if err.response.status_code == 401:
+                # session is wrong, need to relogin
+                self.login()
+                return self.create_panoramic(serial, max_retries + 1)
+
+            raise HTTPError from err
+
+        try:
+            json_output = req.json()
+
+        except ValueError as err:
+            raise PyEzvizError(
+                "Impossible to decode response: "
+                + str(err)
+                + "\nResponse was: "
+                + str(req.text)
+            ) from err
+
+        if json_output.get("resultCode") != "0":
+            raise PyEzvizError(
+                f"Could not send command to create panoramic photo: Got {req.status_code} : {req.text})"
+            )
+
+        return json_output
+
+    def return_panoramic(self, serial: str, max_retries: int = 0) -> Any:
+        """Return panoramic image url list."""
+
+        if max_retries > MAX_RETRIES:
+            raise PyEzvizError("Can't gather proper data. Max retries exceeded.")
+
+        try:
+            req = self._session.post(
+                "https://" + self._token["api_url"] + API_ENDPOINT_RETURN_PANORAMIC,
+                data={"deviceSerial": serial},
+                timeout=self._timeout,
+            )
+
+            req.raise_for_status()
+
+        except requests.HTTPError as err:
+            if err.response.status_code == 401:
+                # session is wrong, need to relogin
+                self.login()
+                return self.return_panoramic(serial, max_retries + 1)
+
+            raise HTTPError from err
+
+        try:
+            json_output = req.json()
+
+        except ValueError as err:
+            raise PyEzvizError(
+                "Impossible to decode response: "
+                + str(err)
+                + "\nResponse was: "
+                + str(req.text)
+            ) from err
+
+        if json_output.get("resultCode") != "0":
+            raise PyEzvizError(
+                f"Could retrieve panoramic photo: Got {req.status_code} : {req.text})"
+            )
+
+        return json_output
+
     def ptz_control_coordinates(
         self, serial: str, x_axis: float, y_axis: float
     ) -> bool:
         """PTZ Coordinate Move."""
         if 0 < x_axis > 1:
             raise PyEzvizError(
                 f"Invalid X coordinate: {x_axis}: Should be between 0 and 1 inclusive"
@@ -668,15 +1170,14 @@
                     "Impossible to decode response: "
                     + str(err)
                     + "\nResponse was: "
                     + str(req.text)
                 ) from err
 
             if json_result["meta"].get("code") == 200:
-
                 self._session.headers["sessionId"] = json_result["sessionInfo"][
                     "sessionId"
                 ]
                 self._token["session_id"] = str(json_result["sessionInfo"]["sessionId"])
                 self._token["rf_session_id"] = str(
                     json_result["sessionInfo"]["refreshSessionId"]
                 )
@@ -831,64 +1332,122 @@
             raise PyEzvizError(
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
-        if json_output.get("meta").get("code") != 200:
+        if json_output["meta"].get("code") != 200:
             raise PyEzvizError(
                 f"Could not set defence mode: Got {req.status_code} : {req.text})"
             )
 
         return True
 
     def do_not_disturb(
         self,
         serial: str,
         enable: int = 1,
+        channelno: int = 1,
         max_retries: int = 0,
     ) -> bool | str:
         """Set do not disturb on camera with spesified serial."""
         if max_retries > MAX_RETRIES:
             raise PyEzvizError("Can't gather proper data. Max retries exceeded.")
 
         try:
             req = self._session.put(
                 "https://"
                 + self._token["api_url"]
                 + API_ENDPOINT_V3_ALARMS
                 + serial
+                + "/"
+                + channelno
                 + API_ENDPOINT_DO_NOT_DISTURB,
-                data={"enable": enable, "channelNo": "1", "deviceSerial": serial},
+                data={"enable": enable, "channelNo": channelno, "deviceSerial": serial},
                 timeout=self._timeout,
             )
             req.raise_for_status()
 
         except requests.HTTPError as err:
             if err.response.status_code == 401:
                 # session is wrong, need to re-log-in
                 self.login()
                 return self.do_not_disturb(serial, enable, max_retries + 1)
 
             raise HTTPError from err
 
         try:
-            response_json = req.json()
+            json_output = req.json()
 
         except ValueError as err:
             raise PyEzvizError("Could not decode response:" + str(err)) from err
 
-        if response_json.get("meta").get("code") != 200:
+        if json_output["meta"].get("code") != 200:
             raise PyEzvizError(
                 f"Could not set defence mode: Got {req.status_code} : {req.text})"
             )
 
         return True
 
+    def set_floodlight_brightness(
+        self,
+        serial: str,
+        luminance: int = 50,
+        channelno: str = "1",
+        max_retries: int = 0,
+    ) -> bool | str:
+        """Set brightness on camera with adjustable light."""
+        if max_retries > MAX_RETRIES:
+            raise PyEzvizError("Can't gather proper data. Max retries exceeded.")
+
+        if luminance not in range(1, 100):
+            raise PyEzvizError(
+                "Range of luminance is 1-100, got " + str(luminance) + "."
+            )
+
+        try:
+            req = self._session.post(
+                "https://"
+                + self._token["api_url"]
+                + API_ENDPOINT_SET_LUMINANCE
+                + "/"
+                + serial
+                + "/"
+                + channelno,
+                data={
+                    "luminance": luminance,
+                },
+                timeout=self._timeout,
+            )
+
+            req.raise_for_status()
+
+        except requests.HTTPError as err:
+            if err.response.status_code == 401:
+                # session is wrong, need to re-log-in
+                self.login()
+                return self.set_floodlight_brightness(
+                    serial, luminance, channelno, max_retries + 1
+                )
+
+            raise HTTPError from err
+
+        try:
+            response_json = req.json()
+
+        except ValueError as err:
+            raise PyEzvizError("Could not decode response:" + str(err)) from err
+
+        if response_json["meta"]["code"] != 200:
+            _LOGGER.error(response_json)
+            return False
+
+        return True
+
     def detection_sensibility(
         self,
         serial: str,
         sensibility: int = 3,
         type_value: int = 3,
         max_retries: int = 0,
     ) -> bool | str:
@@ -971,22 +1530,22 @@
         try:
             response_json = req.json()
 
         except ValueError as err:
             raise PyEzvizError("Could not decode response:" + str(err)) from err
 
         if response_json["resultCode"] != "0":
-            return "Unknown"
+            return None
 
         if response_json["algorithmConfig"]["algorithmList"]:
             for idx in response_json["algorithmConfig"]["algorithmList"]:
                 if idx["type"] == type_value:
                     return idx["value"]
 
-        return "Unknown"
+        return None
 
     # soundtype: 0 = normal, 1 = intensive, 2 = disabled ... don't ask me why...
     def alarm_sound(
         self, serial: str, sound_type: int, enable: int = 1, max_retries: int = 0
     ) -> bool:
         """Enable alarm sound by API."""
         if max_retries > MAX_RETRIES:
@@ -1030,17 +1589,18 @@
         return self._switch_status(serial, status_type, enable)
 
     def _get_page_list(self) -> Any:
         """Get ezviz device info broken down in sections."""
         return self._api_get_pagelist(
             page_filter="CLOUD, TIME_PLAN, CONNECTION, SWITCH,"
             "STATUS, WIFI, NODISTURB, KMS,"
-            "P2P, TIME_PLAN, CHANNEL, VTM,"
-            "DETECTOR, FEATURE, CUSTOM_TAG, UPGRADE,"
-            "VIDEO_QUALITY, QOS, PRODUCTS_INFO, FEATURE_INFO",
+            "P2P, TIME_PLAN, CHANNEL, VTM, DETECTOR,"
+            "FEATURE, CUSTOM_TAG, UPGRADE, VIDEO_QUALITY,"
+            "QOS, PRODUCTS_INFO, SIM_CARD, MULTI_UPGRADE_EXT,"
+            "FEATURE_INFO",
             json_key=None,
         )
 
     def get_device(self) -> Any:
         """Get ezviz devices filter."""
         return self._api_get_pagelist(page_filter="CLOUD", json_key="deviceInfos")
```

### Comparing `pyezviz-0.2.0.9/pyezviz/exceptions.py` & `pyezviz-0.2.1.1/pyezviz/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.0.9/pyezviz/mqtt.py` & `pyezviz-0.2.1.1/pyezviz/mqtt.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,90 +1,109 @@
 """Ezviz cloud MQTT client for push messages."""
+from __future__ import annotations
 
 import base64
 import json
+import logging
 import threading
 import time
+from typing import Any
 
 import paho.mqtt.client as mqtt
 import requests
 
-from .constants import DEFAULT_TIMEOUT, FEATURE_CODE
+from .api_endpoints import (
+    API_ENDPOINT_REGISTER_MQTT,
+    API_ENDPOINT_START_MQTT,
+    API_ENDPOINT_STOP_MQTT,
+)
+from .constants import (
+    APP_SECRET,
+    DEFAULT_TIMEOUT,
+    FEATURE_CODE,
+    MQTT_APP_KEY,
+    REQUEST_HEADER,
+)
 from .exceptions import HTTPError, InvalidURL, PyEzvizError
 
-API_ENDPOINT_SERVER_INFO = "/v3/configurations/system/info"
-API_ENDPOINT_REGISTER_MQTT = "/v1/getClientId"
-API_ENDPOINT_START_MQTT = "/api/push/start"
-API_ENDPOINT_STOP_MQTT = "/api/push/stop"
-
-
-MQTT_APP_KEY = "4c6b3cc2-b5eb-4813-a592-612c1374c1fe"
-APP_SECRET = "17454517-cc1c-42b3-a845-99b4a15dd3e6"
+_LOGGER = logging.getLogger(__name__)
 
 
 class MQTTClient(threading.Thread):
     """Open MQTT connection to ezviz cloud."""
 
     def __init__(
         self,
-        token,
-        timeout=DEFAULT_TIMEOUT,
-    ):
+        token: dict,
+        timeout: int = DEFAULT_TIMEOUT,
+    ) -> None:
         """Initialize the client object."""
         threading.Thread.__init__(self)
-        self._session = None
+        self._session = requests.session()
+        self._session.headers.update(REQUEST_HEADER)
         self._token = token or {
             "session_id": None,
             "rf_session_id": None,
             "username": None,
             "api_url": "apiieu.ezvizlife.com",
         }
         self._timeout = timeout
         self._stop_event = threading.Event()
         self._mqtt_data = {
             "mqtt_clientid": None,
             "ticket": None,
             "push_url": token["service_urls"]["pushAddr"],
         }
+        self.mqtt_client = None
+        self.rcv_message: dict[Any, Any] = {}
 
-    def on_subscribe(self, client, userdata, mid, granted_qos):
+    def on_subscribe(
+        self, client: Any, userdata: Any, mid: Any, granted_qos: Any
+    ) -> None:
         """On MQTT message subscribe."""
         # pylint: disable=unused-argument
-        print("Subscribed: " + str(mid) + " " + str(granted_qos))
+        _LOGGER.info("Subscribed: %s %s", mid, granted_qos)
 
-    def on_connect(self, client, userdata, flags, return_code):
+    def on_connect(
+        self, client: Any, userdata: Any, flags: Any, return_code: Any
+    ) -> None:
         """On MQTT connect."""
         # pylint: disable=unused-argument
         if return_code == 0:
-            print("connected OK Returned code=", return_code)
+            _LOGGER.info("Connected OK with return code %s", return_code)
         else:
-            print("Bad connection Returned code=", return_code)
+            _LOGGER.info("Connection Error with Return code %s", return_code)
             client.reconnect()
 
-    def on_message(self, client, userdata, msg):
+    def on_message(self, client: Any, userdata: Any, msg: Any) -> None:
         """On MQTT message receive."""
         # pylint: disable=unused-argument
-        mqtt_message = json.loads(msg.payload)
+        try:
+            mqtt_message = json.loads(msg.payload)
+
+        except ValueError as err:
+            self.stop()
+            raise PyEzvizError(
+                "Impossible to decode mqtt message: " + str(err)
+            ) from err
+
         mqtt_message["ext"] = mqtt_message["ext"].split(",")
 
-        # Print payload message
-        decoded_message = {
-            mqtt_message["ext"][2]: {
-                "id": mqtt_message["id"],
-                "alert": mqtt_message["alert"],
-                "time": mqtt_message["ext"][1],
-                "alert type": mqtt_message["ext"][4],
-                "image": mqtt_message["ext"][16]
-                if len(mqtt_message["ext"]) > 16
-                else None,
-            }
+        # Format payload message and keep latest device message.
+        self.rcv_message[mqtt_message["ext"][2]] = {
+            "id": mqtt_message["id"],
+            "alert": mqtt_message["alert"],
+            "time": mqtt_message["ext"][1],
+            "alert type": mqtt_message["ext"][4],
+            "image": mqtt_message["ext"][16] if len(mqtt_message["ext"]) > 16 else None,
         }
-        print(decoded_message)
 
-    def _mqtt(self):
+        _LOGGER.debug(self.rcv_message, exc_info=True)
+
+    def _mqtt(self) -> mqtt.Client:
         """Receive MQTT messages from ezviz server."""
 
         ezviz_mqtt_client = mqtt.Client(
             client_id=self._mqtt_data["mqtt_clientid"], protocol=4, transport="tcp"
         )
         ezviz_mqtt_client.on_connect = self.on_connect
         ezviz_mqtt_client.on_subscribe = self.on_subscribe
@@ -95,19 +114,21 @@
         ezviz_mqtt_client.subscribe(
             f"{MQTT_APP_KEY}/ticket/{self._mqtt_data['ticket']}", qos=2
         )
 
         ezviz_mqtt_client.loop_start()
         return ezviz_mqtt_client
 
-    def _register_ezviz_push(self):
+    def _register_ezviz_push(self) -> None:
         """Register for push messages."""
 
-        auth_seq = base64.b64encode(f"{MQTT_APP_KEY}:{APP_SECRET}".encode("ascii"))
-        auth_seq = "Basic " + auth_seq.decode()
+        auth_seq = (
+            "Basic "
+            + base64.b64encode(f"{MQTT_APP_KEY}:{APP_SECRET}".encode("ascii")).decode()
+        )
 
         payload = {
             "appKey": MQTT_APP_KEY,
             "clientType": "5",
             "mac": FEATURE_CODE,
             "token": "123456",
             "version": "v1.3.0",
@@ -139,38 +160,38 @@
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         self._mqtt_data["mqtt_clientid"] = json_result["data"]["clientId"]
 
-    def run(self):
-        """Represent the thread's activity, should not be used directly."""
+    def run(self) -> None:
+        """Start mqtt thread."""
 
-        if self._session is None:
-            self._session = requests.session()
-            self._session.headers.update(
-                {"User-Agent": "okhttp/3.12.1"}
-            )  # Android generic user agent.
+        if self._token.get("username") is None:
+            self._stop_event.set()
+            raise PyEzvizError(
+                "Ezviz internal username is required. Call EzvizClient login without token."
+            )
 
         self._register_ezviz_push()
         self._start_ezviz_push()
-        self._mqtt()
+        self.mqtt_client = self._mqtt()
+
+    def start(self) -> None:
+        """Start mqtt thread as application. Set logging first to see messages."""
+        self.run()
 
         try:
             while not self._stop_event.is_set():
                 time.sleep(1)
         except KeyboardInterrupt:
             self.stop()
 
-    def start(self):
-        """Start mqtt thread."""
-        super().start()
-
-    def stop(self):
+    def stop(self) -> None:
         """Stop push notifications."""
 
         payload = {
             "appKey": MQTT_APP_KEY,
             "clientId": self._mqtt_data["mqtt_clientid"],
             "clientType": 5,
             "sessionId": self._token["session_id"],
@@ -188,17 +209,19 @@
 
         except requests.ConnectionError as err:
             raise InvalidURL("A Invalid URL or Proxy error occured") from err
 
         except requests.HTTPError as err:
             raise HTTPError from err
 
-        self._stop_event.set()
+        finally:
+            self._stop_event.set()
+            self.mqtt_client.loop_stop()
 
-    def _start_ezviz_push(self):
+    def _start_ezviz_push(self) -> None:
         """Send start for push messages to ezviz api."""
 
         payload = {
             "appKey": MQTT_APP_KEY,
             "clientId": self._mqtt_data["mqtt_clientid"],
             "clientType": 5,
             "sessionId": self._token["session_id"],
```

### Comparing `pyezviz-0.2.0.9/pyezviz/test_cam_rtsp.py` & `pyezviz-0.2.1.1/pyezviz/test_cam_rtsp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Test camera RTSP authentication."""
 import base64
 import hashlib
 import socket
 
-from pyezviz.exceptions import AuthTestResultFailed, InvalidHost
+from .exceptions import AuthTestResultFailed, InvalidHost
 
 
 def genmsg_describe(url, seq, user_agent, auth_seq):
     """Generate RTSP describe message."""
     msg_ret = "DESCRIBE " + url + " RTSP/1.0\r\n"
     msg_ret += "CSeq: " + str(seq) + "\r\n"
     msg_ret += "Authorization: " + auth_seq + "\r\n"
```

### Comparing `pyezviz-0.2.0.9/pyezviz/utils.py` & `pyezviz-0.2.1.1/pyezviz/utils.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.0.9/setup.py` & `pyezviz-0.2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyezviz',
-    version="0.2.0.9",
+    version="0.2.1.1",
     license='Apache Software License 2.0',
     author='Pierre Ourdouille',
     author_email='baqs@users.github.com',
     description='Pilot your Ezviz cameras',
     long_description="Pilot your Ezviz cameras with this module. Please view readme on github",
     url='http://github.com/baqs/pyEzviz/',
     packages=setuptools.find_packages(),
```

