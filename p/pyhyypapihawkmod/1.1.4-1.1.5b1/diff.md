# Comparing `tmp/pyhyypapihawkmod-1.1.4.tar.gz` & `tmp/pyhyypapihawkmod-1.1.5b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-1.1.4.tar", last modified: Sun Jun 18 10:38:22 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-1.1.5b1.tar", last modified: Sun Jun 18 18:54:39 2023, max compression
```

## Comparing `pyhyypapihawkmod-1.1.4.tar` & `pyhyypapihawkmod-1.1.5b1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 10:38:22.068194 pyhyypapihawkmod-1.1.4/
--rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.4/LICENSE.md
--rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      517 2023-06-18 10:38:22.066683 pyhyypapihawkmod-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2060 2023-06-18 10:36:49.000000 pyhyypapihawkmod-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 10:38:22.045209 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      429 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0     7697 2023-06-18 10:36:49.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    27687 2023-06-08 12:19:08.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     4005 2023-05-28 09:35:32.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-06-18 10:38:22.063686 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      517 2023-06-18 10:38:21.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-06-18 10:38:21.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 10:38:21.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-18 10:38:21.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-18 10:38:21.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 10:38:22.068194 pyhyypapihawkmod-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      921 2023-06-18 10:36:49.000000 pyhyypapihawkmod-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:54:39.944486 pyhyypapihawkmod-1.1.5b1/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.5b1/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.5b1/MANIFEST.in
+-rw-rw-rw-   0        0        0      519 2023-06-18 18:54:39.943485 pyhyypapihawkmod-1.1.5b1/PKG-INFO
+-rw-rw-rw-   0        0        0     2060 2023-06-18 17:23:40.000000 pyhyypapihawkmod-1.1.5b1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 18:54:39.932293 pyhyypapihawkmod-1.1.5b1/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      431 2023-06-18 18:50:51.000000 pyhyypapihawkmod-1.1.5b1/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.5b1/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0     8123 2023-06-18 18:50:47.000000 pyhyypapihawkmod-1.1.5b1/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.5b1/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.5b1/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    27687 2023-06-18 18:50:53.000000 pyhyypapihawkmod-1.1.5b1/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4005 2023-05-28 09:35:32.000000 pyhyypapihawkmod-1.1.5b1/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.5b1/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.5b1/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.5b1/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:54:39.941492 pyhyypapihawkmod-1.1.5b1/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      519 2023-06-18 18:54:39.000000 pyhyypapihawkmod-1.1.5b1/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-06-18 18:54:39.000000 pyhyypapihawkmod-1.1.5b1/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 18:54:39.000000 pyhyypapihawkmod-1.1.5b1/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-18 18:54:39.000000 pyhyypapihawkmod-1.1.5b1/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-18 18:54:39.000000 pyhyypapihawkmod-1.1.5b1/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 18:54:39.944486 pyhyypapihawkmod-1.1.5b1/setup.cfg
+-rw-rw-rw-   0        0        0      924 2023-06-18 18:51:58.000000 pyhyypapihawkmod-1.1.5b1/setup.py
```

### Comparing `pyhyypapihawkmod-1.1.4/LICENSE.md` & `pyhyypapihawkmod-1.1.5b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.4/PKG-INFO` & `pyhyypapihawkmod-1.1.5b1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.4
+Version: 1.1.5b1
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.4/README.md` & `pyhyypapihawkmod-1.1.5b1/README.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/alarm_info.py` & `pyhyypapihawkmod-1.1.5b1/pyhyypapihawkmod/alarm_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Alarm info for hass integration."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 from datetime import datetime
 from .constants import EventNumber
+import logging
 
 if TYPE_CHECKING:
     from .client import HyypClient
 
-
+_LOGGER = logging.getLogger(__name__)
 
 class HyypAlarmInfos:
     """Initialize Hyyp alarm objects."""
 
     def __init__(self, client: HyypClient) -> None:
         """init."""
         self._client = client
@@ -21,14 +22,25 @@
         self._notifications: dict = {}
         self._last_notification_check_timestamp = 0
 
     def _fetch_data(self) -> None:
         """Fetch data via client api."""
         self._sync_info = self._client.get_sync_info()
         self._state_info = self._client.get_state_info()
+        _LOGGER.debug("Sync Info:")
+        _LOGGER.debug("-----")
+        _LOGGER.debug(self._sync_info)
+        _LOGGER.debug("-----")
+        _LOGGER.debug("</Sync Info>")
+        
+        _LOGGER.debug("State Info:")
+        _LOGGER.debug("-----")
+        _LOGGER.debug(self._state_info)
+        _LOGGER.debug("-----")
+        _LOGGER.debug("</State Info>")
         
     def _fetch_notifications(self, site_id: int) -> dict[Any,Any]:
         """Fetch and cache site notifications."""
         self._notifications = self._client.site_notifications(site_id=site_id)
 
 
     def _last_notice(self) -> dict[Any, Any]:
```

### Comparing `pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-1.1.5b1/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-1.1.5b1/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-1.1.5b1/pyhyypapihawkmod/client.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-1.1.5b1/pyhyypapihawkmod/constants.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-1.1.5b1/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-1.1.5b1/pyhyypapihawkmod/push_receiver.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.4/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-1.1.5b1/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.4
+Version: 1.1.5b1
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.4/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-1.1.5b1/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.4/setup.py` & `pyhyypapihawkmod-1.1.5b1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="1.1.4",
+    version="1.1.5.b1",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
```

