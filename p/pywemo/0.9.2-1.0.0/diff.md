# Comparing `tmp/pywemo-0.9.2.tar.gz` & `tmp/pywemo-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywemo-0.9.2.tar", max compression
+gzip compressed data, was "pywemo-1.0.0.tar", max compression
```

## Comparing `pywemo-0.9.2.tar` & `pywemo-1.0.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0     2831 2023-05-03 05:19:33.307345 pywemo-0.9.2/LICENSE
--rw-r--r--   0        0        0     7426 2023-05-03 05:19:33.307345 pywemo-0.9.2/README.rst
--rw-r--r--   0        0        0     3876 2023-05-03 05:19:33.307345 pywemo-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     1229 2023-05-03 05:19:33.307345 pywemo-0.9.2/pywemo/__init__.py
--rw-r--r--   0        0        0     2762 2023-05-03 05:19:33.307345 pywemo-0.9.2/pywemo/color.py
--rw-r--r--   0        0        0     6857 2023-05-03 05:19:33.307345 pywemo-0.9.2/pywemo/discovery.py
--rw-r--r--   0        0        0     2780 2023-05-03 05:19:33.307345 pywemo-0.9.2/pywemo/exceptions.py
--rw-r--r--   0        0        0     1468 2023-05-03 05:19:33.307345 pywemo-0.9.2/pywemo/ouimeaux_device/LICENSE
--rw-r--r--   0        0        0    26879 2023-05-03 05:19:33.307345 pywemo-0.9.2/pywemo/ouimeaux_device/__init__.py
--rw-r--r--   0        0        0       23 2023-05-03 05:19:33.307345 pywemo-0.9.2/pywemo/ouimeaux_device/api/__init__.py
--rw-r--r--   0        0        0     3382 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/api/attributes.py
--rw-r--r--   0        0        0     6691 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/api/db_orm.py
--rw-r--r--   0        0        0     6030 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/api/long_press.py
--rw-r--r--   0        0        0    14840 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/api/rules_db.py
--rw-r--r--   0        0        0    12468 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/api/service.py
--rw-r--r--   0        0        0      828 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/api/wemo_services.py
--rw-r--r--   0        0        0     6838 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/api/wemo_services.pyi
--rw-r--r--   0        0        0       60 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/api/xsd/__init__.py
--rw-r--r--   0        0        0   108170 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/api/xsd/device.py
--rw-r--r--   0        0        0     4305 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/api/xsd/device.xsd
--rw-r--r--   0        0        0   106749 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/api/xsd/service.py
--rw-r--r--   0        0        0     3526 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/api/xsd/service.xsd
--rw-r--r--   0        0        0     7086 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/api/xsd_types.py
--rw-r--r--   0        0        0    17494 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/bridge.py
--rw-r--r--   0        0        0     2707 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/coffeemaker.py
--rw-r--r--   0        0        0     4210 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/crockpot.py
--rw-r--r--   0        0        0     2652 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/dimmer.py
--rw-r--r--   0        0        0     6193 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/humidifier.py
--rw-r--r--   0        0        0     7068 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/insight.py
--rw-r--r--   0        0        0      328 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/lightswitch.py
--rw-r--r--   0        0        0     2320 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/maker.py
--rw-r--r--   0        0        0      141 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/motion.py
--rw-r--r--   0        0        0      157 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/outdoor_plug.py
--rw-r--r--   0        0        0      991 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/switch.py
--rw-r--r--   0        0        0        0 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/py.typed
--rw-r--r--   0        0        0    17280 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ssdp.py
--rw-r--r--   0        0        0    25195 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/subscribe.py
--rw-r--r--   0        0        0     5522 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/util.py
--rw-r--r--   0        0        0     8238 1970-01-01 00:00:00.000000 pywemo-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     2831 2023-06-17 22:27:32.227857 pywemo-1.0.0/LICENSE
+-rw-r--r--   0        0        0     7620 2023-06-17 22:27:32.227857 pywemo-1.0.0/README.rst
+-rw-r--r--   0        0        0     3140 2023-06-17 22:27:32.227857 pywemo-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2889 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/README.md
+-rw-r--r--   0        0        0     1254 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/__init__.py
+-rw-r--r--   0        0        0     2762 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/color.py
+-rw-r--r--   0        0        0     6709 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/discovery.py
+-rw-r--r--   0        0        0     2753 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/exceptions.py
+-rw-r--r--   0        0        0     1468 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/LICENSE
+-rw-r--r--   0        0        0    26370 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/__init__.py
+-rw-r--r--   0        0        0       23 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/api/__init__.py
+-rw-r--r--   0        0        0     4843 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/api/attributes.py
+-rw-r--r--   0        0        0     6733 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/api/db_orm.py
+-rw-r--r--   0        0        0     6059 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/api/long_press.py
+-rw-r--r--   0        0        0    14976 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/api/rules_db.py
+-rw-r--r--   0        0        0    12705 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/api/service.py
+-rw-r--r--   0        0        0      912 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/api/wemo_services.py
+-rw-r--r--   0        0        0     6838 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/api/wemo_services.pyi
+-rw-r--r--   0        0        0       60 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/api/xsd/__init__.py
+-rw-r--r--   0        0        0   126828 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/api/xsd/device.py
+-rw-r--r--   0        0        0     4305 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/api/xsd/device.xsd
+-rw-r--r--   0        0        0   122520 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/api/xsd/service.py
+-rw-r--r--   0        0        0     3526 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/api/xsd/service.xsd
+-rw-r--r--   0        0        0     7275 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/api/xsd_types.py
+-rw-r--r--   0        0        0    18975 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/bridge.py
+-rw-r--r--   0        0        0     2833 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/coffeemaker.py
+-rw-r--r--   0        0        0     4826 2023-06-17 22:27:32.231857 pywemo-1.0.0/pywemo/ouimeaux_device/crockpot.py
+-rw-r--r--   0        0        0     2250 2023-06-17 22:27:32.231857 pywemo-1.0.0/pywemo/ouimeaux_device/dimmer.py
+-rw-r--r--   0        0        0     6433 2023-06-17 22:27:32.231857 pywemo-1.0.0/pywemo/ouimeaux_device/humidifier.py
+-rw-r--r--   0        0        0     6125 2023-06-17 22:27:32.231857 pywemo-1.0.0/pywemo/ouimeaux_device/insight.py
+-rw-r--r--   0        0        0      328 2023-06-17 22:27:32.231857 pywemo-1.0.0/pywemo/ouimeaux_device/lightswitch.py
+-rw-r--r--   0        0        0     1645 2023-06-17 22:27:32.231857 pywemo-1.0.0/pywemo/ouimeaux_device/maker.py
+-rw-r--r--   0        0        0      141 2023-06-17 22:27:32.231857 pywemo-1.0.0/pywemo/ouimeaux_device/motion.py
+-rw-r--r--   0        0        0      157 2023-06-17 22:27:32.231857 pywemo-1.0.0/pywemo/ouimeaux_device/outdoor_plug.py
+-rw-r--r--   0        0        0     1023 2023-06-17 22:27:32.231857 pywemo-1.0.0/pywemo/ouimeaux_device/switch.py
+-rw-r--r--   0        0        0        0 2023-06-17 22:27:32.231857 pywemo-1.0.0/pywemo/py.typed
+-rw-r--r--   0        0        0    11845 2023-06-17 22:27:32.231857 pywemo-1.0.0/pywemo/ssdp.py
+-rw-r--r--   0        0        0    28195 2023-06-17 22:27:32.231857 pywemo-1.0.0/pywemo/subscribe.py
+-rw-r--r--   0        0        0     4417 2023-06-17 22:27:32.231857 pywemo-1.0.0/pywemo/util.py
+-rw-r--r--   0        0        0     8382 1970-01-01 00:00:00.000000 pywemo-1.0.0/PKG-INFO
```

### Comparing `pywemo-0.9.2/LICENSE` & `pywemo-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.2/README.rst` & `pywemo-1.0.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-pyWeMo |Build Badge| |PyPI Version Badge| |Coverage| |PyPI Downloads Badge|
-===========================================================================
+pyWeMo |Build Badge| |PyPI Version Badge| |Coverage| |PyPI Downloads Badge| |Docs Badge|
+========================================================================================
 Python 3 module to setup, discover and control WeMo devices.
 
 Dependencies
 ------------
 pyWeMo depends on Python packages: requests, ifaddr, lxml, urllib3
 
 How to use
@@ -150,7 +150,10 @@
     :alt: Latest PyPI version
 .. |Coverage| image:: https://coveralls.io/repos/github/pywemo/pywemo/badge.svg?branch=main
     :target: https://coveralls.io/github/pywemo/pywemo?branch=main
     :alt: Coveralls coverage
 .. |PyPI Downloads Badge| image:: https://img.shields.io/pypi/dm/pywemo
     :target: https://pypi.org/project/pywemo/
     :alt: Number of PyPI downloads
+.. |Docs Badge| image:: https://github.com/pywemo/pywemo/actions/workflows/docs.yml/badge.svg
+    :target: https://pywemo.github.io/pywemo/
+    :alt: API Documentation
```

### Comparing `pywemo-0.9.2/pywemo/__init__.py` & `pywemo-1.0.0/pywemo/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-"""Lightweight Python module to discover and control WeMo devices."""
+r"""Lightweight Python module to discover and control WeMo devices.
+.. include:: README.md
+"""
 # flake8: noqa F401
 
 from .discovery import (
     device_from_description,
     discover_devices,
     setup_url_for_address,
 )
```

### Comparing `pywemo-0.9.2/pywemo/color.py` & `pywemo-1.0.0/pywemo/color.py`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.2/pywemo/discovery.py` & `pywemo-1.0.0/pywemo/discovery.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Module to discover WeMo devices."""
 from __future__ import annotations
 
 import logging
-import warnings
 from ipaddress import ip_address
 from socket import gaierror, gethostbyname
 from typing import Any, Callable
 
 import requests
 
 from . import ssdp
@@ -40,86 +39,86 @@
     key = (uuid, method)
     if key in _uuid_seen:
         return
     _uuid_seen.add(key)
     method(*args, *kwargs)
 
 
-def discover_devices(debug: bool = False, **kwargs: Any) -> list[Device]:
+def discover_devices(*, debug: bool = False, **kwargs: Any) -> list[Device]:
     """Find WeMo devices on the local network."""
     devices = (
-        device_from_uuid_and_location(entry.udn, entry.location, debug)
+        device_from_uuid_and_location(entry.udn, entry.location, debug=debug)
         for entry in ssdp.scan(**kwargs)
     )
     return [d for d in devices if d is not None]
 
 
 def device_from_description(
-    description_url: str, mac: str = 'deprecated', debug: bool = False
+    description_url: str, *, debug: bool = False
 ) -> Device | None:
     """Return object representing WeMo device running at host, else None."""
-    if mac != 'deprecated':
-        warnings.warn(
-            "The mac argument to device_from_description is deprecated and "
-            "will be removed in a future release.",
-            DeprecationWarning,
-        )
     try:
         xml = requests.get(description_url, timeout=REQUESTS_TIMEOUT)
     except requests.RequestException:
         LOG.exception("Failed to fetch description %s", description_url)
         return None
 
     try:
         device = DeviceDescription.from_xml(xml.content)
     except PyWeMoException:
         LOG.exception("Failed to parse description %s", description_url)
         return None
 
-    return device_from_uuid_and_location(device.udn, description_url, debug)
+    return device_from_uuid_and_location(
+        device.udn, description_url, debug=debug
+    )
 
 
 def device_from_uuid_and_location(  # noqa: C901
-    uuid: str | None, location: str | None, debug: bool = False
+    # pylint: disable=too-many-branches,too-many-return-statements
+    uuid: str | None,
+    location: str | None,
+    *,
+    debug: bool = False,
 ) -> Device | None:
     """Determine device class based on the device uuid."""
     if not (uuid and location):
         return None
     try:
-        if uuid.startswith('uuid:Socket'):
+        if uuid.startswith("uuid:Socket"):
             return Switch(location)
-        if uuid.startswith('uuid:Lightswitch-1_0'):
+        if uuid.startswith("uuid:Lightswitch-1_0"):
             return LightSwitchLongPress(location)
-        if uuid.startswith('uuid:Lightswitch-2_0'):
+        if uuid.startswith("uuid:Lightswitch-2_0"):
             return LightSwitchLongPress(location)
-        if uuid.startswith('uuid:Lightswitch-3_0'):
+        if uuid.startswith("uuid:Lightswitch-3_0"):
             return LightSwitchLongPress(location)
-        if uuid.startswith('uuid:Lightswitch'):
+        if uuid.startswith("uuid:Lightswitch"):
             return LightSwitch(location)
-        if uuid.startswith('uuid:Dimmer-1_0'):
+        if uuid.startswith("uuid:Dimmer-1_0"):
             return DimmerLongPress(location)
-        if uuid.startswith('uuid:Dimmer-2_0'):
+        if uuid.startswith("uuid:Dimmer-2_0"):
             return DimmerV2(location)
-        if uuid.startswith('uuid:Dimmer'):
+        if uuid.startswith("uuid:Dimmer"):
             return Dimmer(location)
-        if uuid.startswith('uuid:Insight'):
+        if uuid.startswith("uuid:Insight"):
             return Insight(location)
-        if uuid.startswith('uuid:Sensor'):
+        if uuid.startswith("uuid:Sensor"):
             return Motion(location)
-        if uuid.startswith('uuid:Maker'):
+        if uuid.startswith("uuid:Maker"):
             return Maker(location)
-        if uuid.startswith('uuid:Bridge'):
+        if uuid.startswith("uuid:Bridge"):
             return Bridge(location)
-        if uuid.startswith('uuid:CoffeeMaker'):
+        if uuid.startswith("uuid:CoffeeMaker"):
             return CoffeeMaker(location)
-        if uuid.startswith('uuid:Crockpot'):
+        if uuid.startswith("uuid:Crockpot"):
             return CrockPot(location)
-        if uuid.startswith('uuid:Humidifier'):
+        if uuid.startswith("uuid:Humidifier"):
             return Humidifier(location)
-        if uuid.startswith('uuid:OutdoorPlug'):
+        if uuid.startswith("uuid:OutdoorPlug"):
             return OutdoorPlug(location)
     except (InvalidSchemaError, MissingServiceError) as err:
         _call_once_per_uuid(
             uuid,
             LOG.info,
             "pyWeMo encountered a non-WeMo device %s %s: %r",
             uuid,
@@ -129,27 +128,27 @@
         # Fall-through: Try UnsupportedDevice if debug is enabled.
     except PyWeMoException:
         _call_once_per_uuid(
             uuid, LOG.exception, "Device setup failed %s %s", uuid, location
         )
         # Fall-through: Try UnsupportedDevice if debug is enabled.
 
-    if uuid.startswith('uuid:') and debug:
+    if uuid.startswith("uuid:") and debug:
         # unsupported device, but if this function was called from
         # discover_devices then this should be a Belkin product and is probably
         # a WeMo product without a custom class yet.  So attempt to return a
         # basic object to allow manual interaction.
         try:
             device = UnsupportedDevice(location)
         except PyWeMoException:
             LOG.exception("Device setup failed %s %s", uuid, location)
         else:
             LOG.info(
-                'Device with %s is not supported by pywemo, returning '
-                'UnsupportedDevice object to allow manual interaction',
+                "Device with %s is not supported by pywemo, returning "
+                "UnsupportedDevice object to allow manual interaction",
                 uuid,
             )
             return device
 
     return None
 
 
@@ -158,21 +157,21 @@
     try:
         # The {host} must be resolved to an IP address; if this fails, this
         # will throw a socket.gaierror.
         host_address = gethostbyname(hostname)
 
         # Reset {host} to the resolved address.
         LOG.debug(
-            'Resolved hostname %s to IP address %s.', hostname, host_address
+            "Resolved hostname %s to IP address %s.", hostname, host_address
         )
         return host_address
 
     except gaierror:
         # The {host}-as-hostname did not resolve to an IP address.
-        LOG.debug('Could not resolve hostname %s to an IP address.', hostname)
+        LOG.debug("Could not resolve hostname %s to an IP address.", hostname)
         return hostname
 
 
 def setup_url_for_address(host: str, port: int | None = None) -> str | None:
     """Determine setup.xml url for a given host and port pair."""
     # Force hostnames into IP addresses
     try:
```

### Comparing `pywemo-0.9.2/pywemo/exceptions.py` & `pywemo-1.0.0/pywemo/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,32 +17,31 @@
 
     fault_code: str = ""
     fault_string: str = ""
     error_code: str = ""
     error_description: str = ""
 
     def __init__(
-        self, message: str = "", fault_element: et.Element | None = None
+        self, message: str = "", fault_element: et._Element | None = None
     ) -> None:
         """Initialize from a SOAP Fault lxml.etree Element."""
         details = ""
         if fault_element is not None:
             upnp_error_prefix = (
                 "detail"
                 "/{urn:schemas-upnp-org:control-1-0}UPnPError/"
                 "{urn:schemas-upnp-org:control-1-0}"
             )
-            self.fault_code = fault_element.findtext("faultcode") or ""
-            self.fault_string = fault_element.findtext("faultstring") or ""
-            self.error_code = (
-                fault_element.findtext(f"{upnp_error_prefix}errorCode") or ""
+            self.fault_code = fault_element.findtext("faultcode", "")
+            self.fault_string = fault_element.findtext("faultstring", "")
+            self.error_code = fault_element.findtext(
+                f"{upnp_error_prefix}errorCode", ""
             )
-            self.error_description = (
-                fault_element.findtext(f"{upnp_error_prefix}errorDescription")
-                or ""
+            self.error_description = fault_element.findtext(
+                f"{upnp_error_prefix}errorDescription", ""
             )
             details = (
                 f" SOAP Fault {self.fault_code}:{self.fault_string}, "
                 f"{self.error_code}:{self.error_description}"
             )
         super().__init__(f"{message}{details}")
```

### Comparing `pywemo-0.9.2/pywemo/ouimeaux_device/LICENSE` & `pywemo-1.0.0/pywemo/ouimeaux_device/LICENSE`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.2/pywemo/ouimeaux_device/__init__.py` & `pywemo-1.0.0/pywemo/ouimeaux_device/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from __future__ import annotations
 
 import base64
 import logging
 import subprocess
 import threading
 import time
-import warnings
 from typing import Any, Sequence
 
 import requests
 
 from ..exceptions import (
     ActionException,
     APNotFound,
@@ -40,53 +39,52 @@
 
 def probe_wemo(
     host: str,
     ports: Sequence[int] = PROBE_PORTS,
     probe_timeout: float = REQUESTS_TIMEOUT,
     match_udn: str | None = None,
 ) -> int | None:
-    """
-    Probe a host for the current port.
+    """Probe a host for the current port.
 
     This probes a host for known-to-be-possible ports and
     returns the one currently in use. If no port is discovered
     then it returns None.
     """
     for port in ports:
         try:
             response = requests.get(
-                f'http://{host}:{port}/setup.xml', timeout=probe_timeout
+                f"http://{host}:{port}/setup.xml", timeout=probe_timeout
             )
             try:
                 device = DeviceDescription.from_xml(response.content)
             except InvalidSchemaError:
                 continue
             if match_udn and match_udn != device.udn:
                 LOG.error(
-                    'Reconnected to a different WeMo. '
-                    'Expected %s / Received %s',
+                    "Reconnected to a different WeMo. "
+                    "Expected %s / Received %s",
                     match_udn,
                     device.udn,
                 )
                 continue
             return port
         except requests.exceptions.ConnectTimeout:
             # If we timed out connecting, then the wemo is gone,
             # no point in trying further.
             LOG.debug(
-                'Timed out connecting to %s on port %i, wemo is offline',
+                "Timed out connecting to %s on port %i, wemo is offline",
                 host,
                 port,
             )
             break
         except requests.exceptions.Timeout:
             # Apparently sometimes wemos get into a wedged state where
             # they still accept connections on an old port, but do not
             # respond. If that happens, we should keep searching.
-            LOG.debug('No response from %s on port %i, continuing', host, port)
+            LOG.debug("No response from %s on port %i, continuing", host, port)
             continue
         except requests.exceptions.ConnectionError:
             pass
     return None
 
 
 def probe_device(device: Device) -> int | None:
@@ -103,22 +101,16 @@
 
 
 class Device(DeviceDescription, RequiredServicesMixin, WeMoServiceTypesMixin):
     """Base object for WeMo devices."""
 
     EVENT_TYPE_BINARY_STATE = "BinaryState"
 
-    def __init__(self, url: str, mac: str = 'deprecated') -> None:
+    def __init__(self, url: str) -> None:
         """Create a WeMo device."""
-        if mac != 'deprecated':
-            warnings.warn(
-                "The mac argument to Device is deprecated and will be removed "
-                "in a future release.",
-                DeprecationWarning,
-            )
         self._state: int | None = None
         self.basic_state_params: dict[str, str] = {}
         self._reconnect_lock = threading.Lock()
         self.session = Session(url)
         xml = self.session.get(url).data
 
         try:
@@ -162,19 +154,19 @@
             LOG.error("Unable to reconnect with %s", self.name)
 
     def _reconnect_with_device_by_probing(self) -> bool:
         """Attempt to reconnect to the device on the existing port."""
         port = probe_device(self)
 
         if port is None:
-            LOG.error('Unable to re-probe wemo %s at %s', self, self.host)
+            LOG.error("Unable to re-probe wemo %s at %s", self, self.host)
             return False
 
-        LOG.info('Reconnected to wemo %s on port %i', self, port)
-        self.session.url = f'http://{self.host}:{port}/setup.xml'
+        LOG.info("Reconnected to wemo %s on port %i", self, port)
+        self.session.url = f"http://{self.host}:{port}/setup.xml"
         return True
 
     def reconnect_with_device(self) -> None:
         """Re-probe & scan network to rediscover a disconnected device."""
         # Avoid retrying from multiple threads
         # pylint: disable=consider-using-with
         if not self._reconnect_lock.acquire(blocking=False):
@@ -189,15 +181,15 @@
     def parse_basic_state(params: str) -> dict[str, str]:
         """Parse the basic state response from the device."""
         # The BinaryState `params` could have two different formats:
         #   1|1492338954|0|922|14195|1209600|0|940670|15213709|227088884
         #   1
         # In both formats, the first integer value indicates the state.
         # 0 if off, 1 if on,
-        return {'state': params.split('|')[0]}
+        return {"state": params.split("|")[0]}
 
     def update_binary_state(self) -> None:
         """Update the cached copy of the basic state response."""
         self.basic_state_params = self.basicevent.GetBinaryState() or {}
 
     def subscription_update(self, _type: str, _params: str) -> bool:
         """Update device state based on subscription event."""
@@ -219,15 +211,15 @@
     def get_state(self, force_update: bool = False) -> int:
         """Return 0 if off and 1 if on."""
         if force_update or self._state is None:
             self.update_binary_state()
 
             try:
                 self._state = int(
-                    self.basic_state_params.get('BinaryState', 0)
+                    self.basic_state_params.get("BinaryState", 0)
                 )
             except ValueError:
                 self._state = 0
 
         return self._state
 
     def get_service(self, name: str) -> Service:
@@ -241,36 +233,34 @@
         """Return list of services."""
         return list(self.services.keys())
 
     def explain(self) -> None:
         """Print information about the device and its actions."""
         for name, svc in self.services.items():
             print(name)
-            print('-' * len(name))
+            print("-" * len(name))
             for aname, action in svc.actions.items():
-                inputs = ', '.join(str(val) for val in action.args)
-                outputs = ', '.join(str(val) for val in action.returns)
+                inputs = ", ".join(str(val) for val in action.args)
+                outputs = ", ".join(str(val) for val in action.returns)
                 if len(action.returns) > 1:
-                    outputs = '(' + outputs + ')'
+                    outputs = "(" + outputs + ")"
                 if outputs:
-                    outputs = ' -> ' + outputs
+                    outputs = " -> " + outputs
                 print(f"  {aname}({inputs}){outputs}")
             print()
 
     def reset(self, data: bool, wifi: bool) -> str:
-        """
-        Reset Wemo device.
+        """Reset Wemo device.
 
-        Parameters
-        ----------
-        data : bool
+        Args:
+          data (bool):
             Set to True to reset the data ("Clear Personalized Info" in the
             Wemo app), which resets the device name and cleans the icon and
             rules.
-        wifi : bool
+          wifi (bool):
             Set to True to clear wifi information ("Change Wi-Fi" in the Wemo
             app), which does not clear the rules, name, etc.
 
         Notes
         -----
         Setting both to true is equivalent to a "Factory Restore" from the app.
 
@@ -278,166 +268,161 @@
         method is mainly for convenience or when physical access is not
         possible.
 
         From testing on a handful of devices, the Reset codes used in the
         ReSetup action below were consistent.  These could potentially change
         in a future firmware revision or may be different for other untested
         devices.
-
         """
         try:
             action = self.basicevent.ReSetup
         except AttributeError as exc:
             raise ResetException(
-                'Cannot reset device: ReSetup action not found'
+                "Cannot reset device: ReSetup action not found"
             ) from exc
 
         if data and wifi:
-            LOG.info('Clearing data and wifi (factory reset)')
+            LOG.info("Clearing data and wifi (factory reset)")
             result = action(Reset=2)
         elif data:
-            LOG.info('Clearing data (icon, rules, etc)')
+            LOG.info("Clearing data (icon, rules, etc)")
             result = action(Reset=1)
         elif wifi:
-            LOG.info('Clearing wifi information')
+            LOG.info("Clearing wifi information")
             result = action(Reset=5)
         else:
-            raise ResetException('no action requested')
+            raise ResetException("no action requested")
 
         try:
-            status = result['Reset'].strip().lower()
+            status = result["Reset"].strip().lower()
         except KeyError:
-            status = 'unknown'
+            status = "unknown"
 
-        if status == 'success':
-            LOG.info('reset successful')
+        if status == "success":
+            LOG.info("reset successful")
         else:
             # one test unit always returns "reset_remote" here instead of
             # "success", but it appears to still reset successfully
-            LOG.warning('result of reset (may be successful): %s', status)
+            LOG.warning("result of reset (may be successful): %s", status)
 
         return status
 
     def factory_reset(self) -> str:
         """Perform a full factory reset (convenience method)."""
         return self.reset(data=True, wifi=True)
 
     @staticmethod
     def encrypt_aes128(
         password: str, wemo_metadata: str, is_rtos: bool
     ) -> str:
-        """
-        Encrypt a password using OpenSSL.
+        """Encrypt a password using OpenSSL.
 
         Function borrows heavily from Vadim Kantorov's "wemosetup" script:
         https://github.com/vadimkantorov/wemosetup
         """
         if not password:
-            raise SetupException('password required for AES')
+            raise SetupException("password required for AES")
 
         # Wemo uses some meta information for salt and iv
         meta_info = MetaInfo.from_meta_info(wemo_metadata)
         keydata = (
             meta_info.mac[:6] + meta_info.serial_number + meta_info.mac[6:12]
         )
         if is_rtos:
-            keydata += 'b3{8t;80dIN{ra83eC1s?M70?683@2Yf'
+            keydata += "b3{8t;80dIN{ra83eC1s?M70?683@2Yf"
 
         salt, initialization_vector = keydata[:8], keydata[:16]
         if len(salt) != 8 or len(initialization_vector) != 16:
-            LOG.warning('device meta information may not be supported')
+            LOG.warning("device meta information may not be supported")
 
         # call OpenSSL to encrypt the data
         try:
             openssl = subprocess.run(
                 [
-                    'openssl',
-                    'enc',
-                    '-aes-128-cbc',
-                    '-md',
-                    'md5',
-                    '-S',
-                    salt.encode('utf-8').hex(),
-                    '-iv',
-                    initialization_vector.encode('utf-8').hex(),
-                    '-pass',
-                    'pass:' + keydata,
+                    "openssl",
+                    "enc",
+                    "-aes-128-cbc",
+                    "-md",
+                    "md5",
+                    "-S",
+                    salt.encode("utf-8").hex(),
+                    "-iv",
+                    initialization_vector.encode("utf-8").hex(),
+                    "-pass",
+                    "pass:" + keydata,
                 ],
                 check=True,
                 capture_output=True,
-                input=password.encode('utf-8'),
+                input=password.encode("utf-8"),
             )
         except FileNotFoundError as exc:
             raise SetupException(
-                'openssl command failed (openssl not installed / not on path?)'
+                "openssl command failed (openssl not installed / not on path?)"
             ) from exc
         except subprocess.CalledProcessError as exc:
-            raise SetupException('openssl command failed') from exc
+            raise SetupException("openssl command failed") from exc
 
         output = openssl.stdout
-        if output.startswith(b'Salted__'):
+        if output.startswith(b"Salted__"):
             # remove 16byte magic and salt prefix inserted by OpenSSL, which
             # is of the form "Salted__XXXXXXXX" before the actual password
             output = output[16:]
         encrypted_password = base64.b64encode(output).decode()
 
         # the last 4 digits that wemo expects is xxyy, where:
         #     xx: length of the encrypted password as hexadecimal
         #     yy: length of the original password as hexadecimal
-        n_encrypted = len(encrypted_password)
-        n_password = len(password)
-        LOG.debug('password length (before encryption): %s', n_password)
-        LOG.debug('password length (after encryption): %s', n_encrypted)
-        if n_encrypted > 255 or n_password > 255:
+        len_encrypted = len(encrypted_password)
+        len_original = len(password)
+        LOG.debug("password length (before encryption): %s", len_original)
+        LOG.debug("password length (after encryption): %s", len_encrypted)
+        if len_encrypted > 255 or len_original > 255:
             # untested, but over 255 characters would require >2 hex digits
             raise SetupException(
-                'Wemo requires the wifi password (including after encryption) '
-                'to be 255 or less characters, but found password of length '
-                f'{n_password} (and {n_encrypted} after encryption).'
+                "Wemo requires the wifi password (including after encryption) "
+                "to be 255 or less characters, but found password of length "
+                f"{len_original} (and {len_encrypted} after encryption)."
             )
 
         if not is_rtos:
-            encrypted_password += f'{n_encrypted:#04x}'[2:]
-            encrypted_password += f'{n_password:#04x}'[2:]
+            encrypted_password += f"{len_encrypted:#04x}"[2:]
+            encrypted_password += f"{len_original:#04x}"[2:]
         return encrypted_password
 
     def setup(self, *args: Any, **kwargs: Any) -> tuple[str, str]:
-        """
-        Connect Wemo to wifi network.
+        """Connect Wemo to wifi network.
 
         This function should be used and will capture several potential
         exceptions to indicate when the setup method won't work on a device.
 
-        Parameters
-        ----------
-        ssid : str
+        Args:
+          ssid (str):
             SSID to connect the device to.
-        password : str
+          password (str):
             Password for the indicated SSID.  This password will be encrypted
             with OpenSSL and then sent to the device.  To connect to an open,
             unsecured network, pass anything for the password as it will be
             ignored.
-        timeout : float, optional
+          timeout (float, optional):
             Number of seconds to wait and poll a device to see if it has
             successfully connected to the network.  The minimum value allows is
             15 seconds as devices sometimes take 10-15 seconds to connect.
-        connection_attempts : int, optional
+          connection_attempts (int, optional):
             Number of times to try connecting a debice to the network, if it
             has failed to connect within `timeout` seconds.
-        status_delay : float, optional
+          status_delay (float, optional):
             Number of seconds to delay between each called to the connection
             status of the device.  Generally should prefer this to be as short
             as possible, but not too quick to overload the device with
             requests.  It must be less than or equal to half of the `timeout`.
 
         Notes
         -----
         The timeout applies to each connection attempt, so the total wait time
-        will be approximately timeout * connection_attempts
-
+        will be approximately `timeout * connection_attempts`.
         """
         try:
             return self._setup(*args, **kwargs)
         except (UnknownService, AttributeError, KeyError) as exc:
             #    Exception       | Reason to catch it
             #    --------------------------------------------------------------
             #    UnknownService  | some devices or firmwares may not have the
@@ -445,219 +430,220 @@
             #    --------------------------------------------------------------
             #    AttributeError  | some devices or firmwares may not have the
             #                    | actions used
             #    --------------------------------------------------------------
             #    KeyError        | an expected result (return from an action)
             #                    | does not exist (e.g. ApList)
             #    --------------------------------------------------------------
-            raise SetupException(f'pywemo cannot setup {self}') from exc
+            raise SetupException(f"pywemo cannot setup {self}") from exc
         except ActionException as exc:
             #    Exception       | Reason to catch it
             #    --------------------------------------------------------------
             #    ActionException | one of the action calls never returned!  The
             #                    | device was not re-discovered.  It may have
             #                    | lost power (been unplugged).
             #    --------------------------------------------------------------
             raise SetupException(
-                f'pywemo lost device {self} and was unable to reconnect.  '
-                'Setup status is uncertain, re-probing and checking is '
-                'required.'
+                f"pywemo lost device {self} and was unable to reconnect.  "
+                "Setup status is uncertain, re-probing and checking is "
+                "required."
             ) from exc
 
     def _setup(  # noqa: C901
+        # pylint: disable=too-many-arguments,too-many-branches,too-many-locals
+        # pylint: disable=too-many-statements
         self,
         ssid: str,
         password: str,
         timeout: float = 20.0,
         connection_attempts: int = 1,
         status_delay: float = 1.0,
     ) -> tuple[str, str]:
-        """
-        Connect Wemo to wifi network.
+        """Connect Wemo to wifi network.
 
         See the setup method for details.
         """
         # a timeout of less than 20 is too short for many devices, so require
         # at least 20 seconds.
         timeout = max(timeout, 20.0)
         status_delay = min(status_delay, timeout / 2.0)
         connection_attempts = int(max(1, connection_attempts))
 
         # find all access points that the device can see, and select the one
         # matching the desired SSID
-        LOG.info('scanning for AP\'s...')
-        wifisetup = self.get_service('WiFiSetup')
-        access_points = wifisetup.GetApList()['ApList']
+        LOG.info("scanning for AP's...")
+        wifisetup = self.get_service("WiFiSetup")
+        access_points = wifisetup.GetApList()["ApList"]
 
         selected_ap = None
-        for access_point in access_points.split('\n')[1:]:
-            access_point = access_point.strip().rstrip(',')
-            if not access_point.strip() or '|' not in access_point:
+        for access_point in access_points.split("\n")[1:]:
+            access_point = access_point.strip().rstrip(",")
+            if not access_point.strip() or "|" not in access_point:
                 continue
-            LOG.debug('found AP: %s', access_point)
-            if access_point.startswith(f'{ssid}|'):
+            LOG.debug("found AP: %s", access_point)
+            if access_point.startswith(f"{ssid}|"):
                 selected_ap = access_point
-                LOG.info('selecting AP: %s', selected_ap)
+                LOG.info("selecting AP: %s", selected_ap)
                 break
 
         if selected_ap is None:
-            raise APNotFound(f'AP with SSID {ssid} not found.  Try again.')
+            raise APNotFound(f"AP with SSID {ssid} not found.  Try again.")
 
         # get some information about the access point
-        columns = selected_ap.split('|')
+        columns = selected_ap.split("|")
         channel = columns[1].strip()
-        auth_mode, encryption_method = columns[-1].strip().split('/')
-        LOG.debug('AP channel: %s', channel)
-        LOG.debug('AP authorization mode(s): %s', auth_mode)
-        LOG.debug('AP encryption method: %s', encryption_method)
+        auth_mode, encryption_method = columns[-1].strip().split("/")
+        LOG.debug("AP channel: %s", channel)
+        LOG.debug("AP authorization mode(s): %s", auth_mode)
+        LOG.debug("AP encryption method: %s", encryption_method)
 
         # check if the encryption type is supported by this script
-        supported_encryptions = {'NONE', 'AES'}
+        supported_encryptions = {"NONE", "AES"}
         if encryption_method not in supported_encryptions:
             raise SetupException(
-                f'Encryption {encryption_method} not currently supported.  '
+                f"Encryption {encryption_method} not currently supported.  "
                 f'Supported encryptions are: {",".join(supported_encryptions)}'
             )
 
         # try to connect the device to the selected network
-        if encryption_method == 'NONE':
-            LOG.debug('selected network has no encryption (password ignored)')
-            auth_mode = 'OPEN'
-            encrypted_password = ''
+        if encryption_method == "NONE":
+            LOG.debug("selected network has no encryption (password ignored)")
+            auth_mode = "OPEN"
+            encrypted_password = ""
         else:
             # get the meta information of the device and encrypt the password
-            meta_info = self.get_service('metainfo').GetMetaInfo()['MetaInfo']
-            is_rtos = self._config_any.get('rtos', '0') == '1'
+            meta_info = self.get_service("metainfo").GetMetaInfo()["MetaInfo"]
+            is_rtos = self._config_any.get("rtos", "0") == "1"
             encrypted_password = self.encrypt_aes128(
                 password, meta_info, is_rtos
             )
 
         # optionally make multiple connection attempts
         start_time = time.time()
 
         # status messages:
         #     0: still trying to connect to network
         #     1: successfully connected
         #     2: short password (Wemo requires at least 8 characters)
         #     3: performing handshake? (uncertain, but devices generally
         #        go to status 3 for a few moments before switching to
         #        successful status 1)
-        skip = {'1', '2'}
+        skip = {"1", "2"}
 
         for attempt in range(connection_attempts):
-            LOG.info('sending connection request (try %s)', attempt + 1)
+            LOG.info("sending connection request (try %s)", attempt + 1)
             # success rate is much higher if the ConnectHomeNetwork command is
             # sent twice (not sure why!)
-            for i in range(2):
+            for retry in range(2):
                 result = wifisetup.ConnectHomeNetwork(
                     ssid=ssid,
                     auth=auth_mode,
                     password=encrypted_password,
                     encrypt=encryption_method,
                     channel=channel,
                 )
                 try:
-                    status = result['PairingStatus']
+                    status = result["PairingStatus"]
                 except KeyError:
                     # print entire dictionary if PairingStatus doesn't exist
                     status = repr(result)
-                LOG.debug('pairing status (send %s): %s', i + 1, status)
-                if i == 0:
+                LOG.debug("pairing status (send %s): %s", retry + 1, status)
+                if retry == 0:
                     # only delay on the first call
                     time.sleep(0.10)
 
             timeout_start = time.time()
-            LOG.info('starting status checks (%s second timeout)', timeout)
-            status = ''
+            LOG.info("starting status checks (%s second timeout)", timeout)
+            status = ""
 
             # Make an initial, quicker check
             time.sleep(min(0.50, status_delay / 3.0))
-            status = wifisetup.GetNetworkStatus()['NetworkStatus']
-            LOG.debug('initial status check: %s', status)
+            status = wifisetup.GetNetworkStatus()["NetworkStatus"]
+            LOG.debug("initial status check: %s", status)
 
             while time.time() - timeout_start < timeout and status not in skip:
                 time.sleep(status_delay)
-                status = wifisetup.GetNetworkStatus()['NetworkStatus']
+                status = wifisetup.GetNetworkStatus()["NetworkStatus"]
                 LOG.debug(
-                    'network status after %.2f seconds: %s',
+                    "network status after %.2f seconds: %s",
                     time.time() - timeout_start,
                     status,
                 )
             if status in skip:
                 # skip any further attempts
                 break
 
         # status 3 usually (always?) occurs shortly before it switches to
         # status 1, so if the status is 3 here, then delay a few more seconds
         # to see if it switches to status 1.
-        if status == '3':
-            LOG.debug('delaying a little longer (status 3)...')
+        if status == "3":
+            LOG.debug("delaying a little longer (status 3)...")
             loops = 3  # 3 seconds with default status_delay
             while loops > 0 and status not in skip:
                 time.sleep(status_delay)
-                status = wifisetup.GetNetworkStatus()['NetworkStatus']
+                status = wifisetup.GetNetworkStatus()["NetworkStatus"]
                 loops -= 1
 
         try:
             result = wifisetup.CloseSetup()
         except AttributeError:
             # if CloseSetup doesn't exist, it may still work
-            result = {'status': 'CloseSetup action not available'}
+            result = {"status": "CloseSetup action not available"}
 
         try:
-            close_status = result['status']
+            close_status = result["status"]
         except KeyError:
             # print entire dictionary if status doesn't exist
             close_status = repr(result)
-        LOG.debug('network status: %s', status)
-        LOG.debug('close status: %s', close_status)
+        LOG.debug("network status: %s", status)
+        LOG.debug("close status: %s", close_status)
 
-        if status == '2':
+        if status == "2":
             # we could check the password length way earlier (start of the
             # function), but perhaps Wemo will change this requirement some
             # day to make it longer, so instead just use the status '2' return
             # code.
             raise ShortPassword(
-                'Password is too short (Wemo requires at least 8 characters).'
+                "Password is too short (Wemo requires at least 8 characters)."
             )
 
-        if status == '1' and close_status == 'success':
+        if status == "1" and close_status == "success":
             try:
                 self.basicevent.SetSetupDoneStatus()
             except AttributeError:
                 LOG.debug(
-                    'SetSetupDoneStatus not available (some devices do not '
-                    'have this method)'
+                    "SetSetupDoneStatus not available (some devices do not "
+                    "have this method)"
                 )
             LOG.info(
                 'Wemo device connected to "%s" in %.2f seconds (%s connection '
-                'attempts(s))',
+                "attempts(s))",
                 ssid,
                 time.time() - start_time,
                 attempt + 1,
             )
-        elif status == '1':
+        elif status == "1":
             LOG.warning(
                 'Wemo device likely connected to "%s", but should be verified '
                 '(CloseSetup returned "%s").',
                 ssid,
                 close_status,
             )
-        elif status == '3':
+        elif status == "3":
             raise SetupException(
                 f'Wemo device failed to connect to "{ssid}", but has status=3,'
-                'which usually precedes a successful connection.  Thus it may '
-                'still connect to the network shortly.  Otherwise, please try '
-                'again.'
+                "which usually precedes a successful connection.  Thus it may "
+                "still connect to the network shortly.  Otherwise, please try "
+                "again."
             )
         else:
             raise SetupException(
                 f'Wemo device failed to connect to "{ssid}".  It could be a '
-                'wrong password or Wemo device/firmware issue.  Please try '
-                'again.'
+                "wrong password or Wemo device/firmware issue.  Please try "
+                "again."
             )
 
         return status, close_status
 
     @classmethod
     def supports_long_press(cls) -> bool:
         """Return True of the device supports long press events."""
@@ -670,24 +656,14 @@
 
     @property
     def port(self) -> int:
         """TCP port for the device's UPnP web server."""
         return self.session.port
 
     @property
-    def serialnumber(self) -> str:
-        """Return the serial number of the device."""
-        warnings.warn(
-            "serialnumber is deprecated and will be removed in a future "
-            "release. Use serial_number instead.",
-            DeprecationWarning,
-        )
-        return self.serial_number
-
-    @property
     def device_type(self) -> str:
         """Return what kind of WeMo this device is."""
         return type(self).__name__
 
     def __repr__(self) -> str:
         """Return a string representation of the device."""
         return f'<WeMo {self.device_type} "{self.name}">'
```

### Comparing `pywemo-0.9.2/pywemo/ouimeaux_device/api/db_orm.py` & `pywemo-1.0.0/pywemo/ouimeaux_device/api/db_orm.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
     def sql_type(self):
         """Return the sqlite type name for this type."""
         if self.not_null:
             return f"{self._sql_type} NOT NULL".lstrip()
         return self._sql_type.lstrip()
 
 
-class PrimaryKey(SQLType):
+class PrimaryKey(SQLType):  # pylint: disable=too-few-public-methods
     """Class used to indicate the primary key field for a Row."""
 
     def __init__(self, *args, auto_increment=False, **kwargs):
         """Create a PrimaryKey instance."""
         super().__init__(*args, **kwargs)
         self.auto_increment = auto_increment
```

### Comparing `pywemo-0.9.2/pywemo/ouimeaux_device/api/long_press.py` & `pywemo-1.0.0/pywemo/ouimeaux_device/api/long_press.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         EndDate="07301982",
         State="1",
         Sync="NOSYNC",
     )
     rules_db.add_rule(new_rule)
     rules_db.add_rule_devices(
         RuleDevicesRow(
-            RuleID=new_rule.RuleID,
+            RuleID=new_rule.RuleID,  # pylint: disable=no-member
             DeviceID=device_udn,
             GroupID=0,
             DayID=-1,
             StartTime=60,
             RuleDuration=86340,
             StartAction=ActionType.TOGGLE.value,
             EndAction=-1.0,
```

### Comparing `pywemo-0.9.2/pywemo/ouimeaux_device/api/rules_db.py` & `pywemo-1.0.0/pywemo/ouimeaux_device/api/rules_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Access and manipulate the on-device rules sqlite database."""
 
 import base64
 import contextlib
 import io
 import logging
+import os
 import sqlite3
 import tempfile
 import zipfile
 from types import MappingProxyType
 from typing import FrozenSet, List, Mapping, Optional, Tuple
 
 from pywemo.exceptions import HTTPNotOkException, RulesDbQueryError
@@ -179,15 +180,15 @@
             RuleDevicesRow.select_all(cursor)
         )
         self._target_devices = _index_by_primary_key(
             TargetDevicesRow.select_all(cursor)
         )
 
     @property
-    def db(self) -> sqlite3.Connection:
+    def db(self) -> sqlite3.Connection:  # pylint: disable=invalid-name
         """Return the sqlite3 connection instance."""
         return self._db
 
     def cursor(self) -> sqlite3.Cursor:
         """Return a cursor for the underlying sqlite3 database."""
         return self.db.cursor()
 
@@ -368,25 +369,24 @@
     version = int(fetch["ruleDbVersion"])
     rule_db_url = fetch["ruleDbPath"]
     try:
         response = device.session.get(rule_db_url)
     except HTTPNotOkException:
         response = None
 
-    with tempfile.NamedTemporaryFile(
-        prefix="wemorules", suffix=".db"
-    ) as temp_db_file:
+    with tempfile.TemporaryDirectory(prefix="wemorules_") as temp_dir:
+        local_file_name = os.path.join(temp_dir, "rules.db")
         # Create a new db, or extract the current db.
         if response is None:
-            db_file_name = _create_empty_db(temp_db_file.name)
+            inner_file_name = _create_empty_db(local_file_name)
         else:
-            db_file_name = _unpack_db(response.content, temp_db_file)
+            inner_file_name = _unpack_db(response.content, local_file_name)
 
         # Open the DB.
-        conn = sqlite3.connect(temp_db_file.name)
+        conn = sqlite3.connect(local_file_name)
         try:
             conn.row_factory = sqlite3.Row
             try:
                 rules = RulesDb(
                     conn, default_udn=device.udn, device_name=device.name
                 )
                 yield rules
@@ -403,44 +403,44 @@
                 raise RulesDbQueryError(f"sqlite3 exception {err}") from err
 
             if rules.update_if_modified():
                 LOG.debug("Rules for %s updated. Storing rules.", device.name)
                 conn.commit()
                 conn.close()
                 conn = None
-                body = _pack_db(temp_db_file, db_file_name)
+                body = _pack_db(local_file_name, inner_file_name)
                 device.rules.StoreRules(
                     ruleDbVersion=version + 1,
                     processDb=1,
                     ruleDbBody="&lt;![CDATA[" + body + "]]&gt;",
                 )
         finally:
             if conn is not None:
                 conn.close()
 
 
-def _unpack_db(content, db_file):
+def _unpack_db(content, local_file_name):
     """Unpack the sqlite database from a .zip file content."""
     zip_contents = io.BytesIO(content)
     with zipfile.ZipFile(zip_contents) as zip_file:
         inner_file_name = zip_file.namelist()[0]
         with zip_file.open(inner_file_name) as zipped_db_file:
-            db_file.write(zipped_db_file.read())
-            db_file.flush()
+            with open(local_file_name, "w+b") as db_file:
+                db_file.write(zipped_db_file.read())
         return inner_file_name
     raise RuntimeError("Could not find database within zip file")
 
 
-def _pack_db(db_file, inner_file_name):
+def _pack_db(local_file_name, inner_file_name):
     """Pack the sqlite database as a base64(zipped(db))."""
     zip_contents = io.BytesIO()
     with zipfile.ZipFile(
         zip_contents, mode="w", compression=zipfile.ZIP_DEFLATED
     ) as zip_file:
-        zip_file.write(db_file.name, arcname=inner_file_name)
+        zip_file.write(local_file_name, arcname=inner_file_name)
     return base64.b64encode(zip_contents.getvalue()).decode("utf-8")
 
 
 def _index_by_primary_key(rows):
     """Return a dict of Rows indexed by the primary key."""
     result = {}
     for row in rows:
```

### Comparing `pywemo-0.9.2/pywemo/ouimeaux_device/api/service.py` & `pywemo-1.0.0/pywemo/ouimeaux_device/api/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,21 +63,21 @@
     response body and will raise an exception if fetching the response body
     takes longer than the timeout.
 
     Since much of pywemo is built atop the requests library, a `content`
     field on HTTPResponse is populated from the `data` field.
     """
 
-    # Retry strategy for requests that fail.
     retries: int | urllib3.Retry | None = urllib3.Retry(
-        total=6, backoff_factor=1.5, allowed_methods=['GET', 'POST']
+        total=6, backoff_factor=1.5, allowed_methods=["GET", "POST"]
     )
+    """Retry strategy for requests that fail."""
 
-    # Seconds that a request can be idle before retrying.
     timeout = 3.0
+    """Seconds that a request can be idle before retrying."""
 
     def __init__(
         self,
         url: str,
         retries: int | urllib3.Retry | None = None,
         timeout: float | None = None,
     ) -> None:
@@ -133,19 +133,19 @@
                 raise HTTPException(err) from err
             # For `requests` compatibility.
             response.content = response.data  # type: ignore
             return response
 
     def get(self, url: str, **kwargs: Any) -> urllib3.HTTPResponse:
         """HTTP GET request."""
-        return self.request('GET', url, **kwargs)
+        return self.request("GET", url, **kwargs)
 
     def post(self, url: str, **kwargs: Any) -> urllib3.HTTPResponse:
         """HTTP POST request."""
-        return self.request('POST', url, **kwargs)
+        return self.request("POST", url, **kwargs)
 
     def urljoin(self, path: str) -> str:
         """Build an absolute URL from a path."""
         return urljoin(self._url, path)
 
     @property
     def url(self) -> str:
@@ -171,34 +171,34 @@
         """Hostname associated with this session."""
         return self._host
 
 
 class Action:
     """Representation of an Action for a WeMo device."""
 
-    # A few actions take longer than the default timeout. Override the default
-    # timeout value for those actions.
     soap_action_timeout_override = {
         "urn:Belkin:service:bridge:1#AddDevice": 30,
         "urn:Belkin:service:bridge:1#OpenNetwork": 30,
         "urn:Belkin:service:WiFiSetup:1#GetApList": 10,
     }
+    """A few actions take longer than the default timeout. Override the default
+    timeout value for those actions."""
 
     max_rediscovery_attempts = 3
 
     def __init__(
         self, service: Service, action_config: ActionProperties
     ) -> None:
         """Create an instance of an Action."""
         self.name = action_config.name
         self.service = service
-        self.soap_action = f'{service.serviceType}#{self.name}'
+        self.soap_action = f"{service.serviceType}#{self.name}"
         self.headers = {
-            'Content-Type': 'text/xml',
-            'SOAPACTION': f'"{self.soap_action}"',
+            "Content-Type": "text/xml",
+            "SOAPACTION": f'"{self.soap_action}"',
         }
 
         self.args = [
             arg.name
             for arg in action_config.arguments
             if arg.direction.lower() != "out"
         ]
@@ -208,16 +208,16 @@
             if arg.direction.lower() == "out"
         ]
 
     def __call__(
         self, *, pywemo_timeout: float | None = None, **kwargs: Any
     ) -> dict[str, str]:
         """Representations a method or function call."""
-        arglist = '\n'.join(
-            f'<{arg}>{value}</{arg}>' for arg, value in kwargs.items()
+        arglist = "\n".join(
+            f"<{arg}>{value}</{arg}>" for arg, value in kwargs.items()
         )
         body = REQUEST_TEMPLATE.format(
             action=self.name, service=self.service.serviceType, args=arglist
         ).strip()
         timeout = pywemo_timeout or self.soap_action_timeout_override.get(
             self.soap_action
         )
@@ -239,27 +239,29 @@
                     session.host,
                     session.port,
                     err,
                     attempt,
                 )
                 last_exception = err
             else:
-                envelope = et.fromstring(response.data)
+                envelope = et.fromstring(
+                    response.data, parser=et.XMLParser(resolve_entities=False)
+                )
                 body_element = list(envelope)[0]
                 response_element = list(body_element)[0]
                 if (
                     response_element.tag
                     == "{http://schemas.xmlsoap.org/soap/envelope/}Fault"
                 ):
                     raise SOAPFault(
                         f"Error calling {self.soap_action}",
                         fault_element=response_element,
                     )
                 return {
-                    response_item.tag: response_item.text
+                    response_item.tag: response_item.text or ""
                     for response_item in response_element
                 }
 
             self.service.device.reconnect_with_device()
 
         msg = (
             f"Error communicating with {self.service.device.name} after "
@@ -272,19 +274,19 @@
         """Return a string representation of the Action."""
         return f"<Action {self.name}({', '.join(self.args)})>"
 
 
 class Service(WeMoAllActionsMixin):
     """Representation of a service for a WeMo device."""
 
-    def __init__(self, device: 'Device', service: ServiceProperties) -> None:
+    def __init__(self, device: "Device", service: ServiceProperties) -> None:
         """Create an instance of a Service."""
         self.device = device
         self._config = service
-        self.name = self.serviceType.split(':')[-2]
+        self.name = self.serviceType.split(":")[-2]
         self.actions = {}
 
         url = device.session.urljoin(service.description_url)
         xml = device.session.get(url).data
 
         try:
             scpd = ServiceDescription.from_xml(xml)
@@ -294,25 +296,25 @@
 
         for action in scpd.actions:
             act = Action(self, action)
             self.actions[act.name] = act
             setattr(self, act.name, act)
 
     @property
-    def controlURL(self) -> str:
+    def controlURL(self) -> str:  # pylint: disable=invalid-name
         """Get the controlURL for interacting with this Service."""
         return self.device.session.urljoin(self._config.control_url)
 
     @property
-    def eventSubURL(self) -> str:
+    def eventSubURL(self) -> str:  # pylint: disable=invalid-name
         """Get the eventSubURL for interacting with this Service."""
         return self.device.session.urljoin(self._config.event_subscription_url)
 
     @property
-    def serviceType(self) -> str:
+    def serviceType(self) -> str:  # pylint: disable=invalid-name
         """Get the type of this Service."""
         return self._config.service_type
 
     def __repr__(self) -> str:
         """Return a string representation of the Service."""
         return f"<Service {self.name}({', '.join(self.actions)})>"
 
@@ -321,15 +323,15 @@
 class RequiredService:
     """Specifies the service name and actions that are required for a class."""
 
     name: str
     actions: list[str]
 
 
-class RequiredServicesMixin:
+class RequiredServicesMixin:  # pylint: disable=too-few-public-methods
     """Provide and check for required services."""
 
     @property
     def _required_services(self) -> list[RequiredService]:
         return []
 
     def _check_required_services(self, services: Iterable[Service]) -> None:
```

### Comparing `pywemo-0.9.2/pywemo/ouimeaux_device/api/wemo_services.py` & `pywemo-1.0.0/pywemo/ouimeaux_device/api/wemo_services.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 
 mypy, however, uses the wemo_services.pyi stub typing file to find basic type
 information for the services and actions supported by WeMo devices. This type
 information is generated by scripts/generate_wemo_service.py.
 """
 
 
-class WeMoServiceTypesMixin:
+class WeMoServiceTypesMixin:  # pylint: disable=too-few-public-methods
     """Mixin for the Device base class.
 
     Provides type information for the service properties that are dynamically
     set at run-time via `setattr(self, service_name, Service(...))`.
     """
 
 
-class WeMoAllActionsMixin:
+class WeMoAllActionsMixin:  # pylint: disable=too-few-public-methods
     """Mixin for the Service base class.
 
     Provides type information for every known service action method. These
     methods are set as properties of the Service instance at run-time via
     `setattr(self, action_name, Action(...))`.
     """
```

### Comparing `pywemo-0.9.2/pywemo/ouimeaux_device/api/wemo_services.pyi` & `pywemo-1.0.0/pywemo/ouimeaux_device/api/wemo_services.pyi`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.2/pywemo/ouimeaux_device/api/xsd/device.py` & `pywemo-1.0.0/pywemo/ouimeaux_device/api/xsd/device.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
+# flake8: noqa
+# isort: skip_file
+# mypy: ignore-errors
+# pylint: skip-file
 
 #
-# Generated Sun Dec 27 17:49:26 2020 by generateDS.py version 2.37.11.
-# Python 3.8.5 (default, Jul 28 2020, 12:59:40)  [GCC 9.3.0]
+# Generated  by generateDS.py version 2.41.5.
+# Python [sys.version]
 #
 # Command line options:
+#   ('-f', '')
+#   ('--no-dates', '')
 #   ('-o', 'device.py')
 #
 # Command line arguments:
-#   device.xsd
+#   pywemo/ouimeaux_device/api/xsd/device.xsd
 #
 # Command line:
-#   generateDS -o "device.py" device.xsd
+#   generateDS.py -f --no-dates -o "device.py" pywemo/ouimeaux_device/api/xsd/device.xsd
 #
 # Current working directory (os.getcwd()):
-#   xsd
+#   pywemo
 #
 
 import sys
+
 try:
     ModulenotfoundExp_ = ModuleNotFoundError
 except NameError:
     ModulenotfoundExp_ = ImportError
 from itertools import zip_longest
 import os
 import re as re_
 import base64
 import datetime as datetime_
 import decimal as decimal_
-try:
-    from lxml import etree as etree_
-except ModulenotfoundExp_ :
-    from xml.etree import ElementTree as etree_
+from lxml import etree as etree_
 
 
 Validate_simpletypes_ = True
 SaveElementTreeNode = True
+TagNamePrefix = ""
 if sys.version_info.major == 2:
     BaseStrType_ = basestring
 else:
     BaseStrType_ = str
 
 
 def parsexml_(infile, parser=None, **kwargs):
@@ -56,26 +61,28 @@
         if isinstance(infile, os.PathLike):
             infile = os.path.join(infile)
     except AttributeError:
         pass
     doc = etree_.parse(infile, parser=parser, **kwargs)
     return doc
 
+
 def parsexmlstring_(instring, parser=None, **kwargs):
     if parser is None:
         # Use the lxml ElementTree compatible parser so that, e.g.,
         #   we ignore comments.
         try:
             parser = etree_.ETCompatXMLParser()
         except AttributeError:
             # fallback to xml.etree
             parser = etree_.XMLParser()
     element = etree_.fromstring(instring, parser=parser, **kwargs)
     return element
 
+
 #
 # Namespace prefix definition table (and other attributes, too)
 #
 # The module generatedsnamespaces, if it is importable, must contain
 # a dictionary named GeneratedsNamespaceDefs.  This Python dictionary
 # should map element type names (strings) to XML schema namespace prefix
 # definitions.  The export method for any class for which there is
@@ -91,48 +98,51 @@
 #         "ElementtypeA": "http://www.xxx.com/namespaceA",
 #         "ElementtypeB": "http://www.xxx.com/namespaceB",
 #     }
 #
 # Additionally, the generatedsnamespaces module can contain a python
 # dictionary named GenerateDSNamespaceTypePrefixes that associates element
 # types with the namespace prefixes that are to be added to the
-# "xsi:type" attribute value.  See the exportAttributes method of
+# "xsi:type" attribute value.  See the _exportAttributes method of
 # any generated element type and the generation of "xsi:type" for an
 # example of the use of this table.
 # An example table:
 #
 #     # File: generatedsnamespaces.py
 #
 #     GenerateDSNamespaceTypePrefixes = {
 #         "ElementtypeC": "aaa:",
 #         "ElementtypeD": "bbb:",
 #     }
 #
 
 try:
-    from generatedsnamespaces import GenerateDSNamespaceDefs as GenerateDSNamespaceDefs_
-except ModulenotfoundExp_ :
+    from generatedsnamespaces import (
+        GenerateDSNamespaceDefs as GenerateDSNamespaceDefs_,
+    )
+except ModulenotfoundExp_:
     GenerateDSNamespaceDefs_ = {}
 try:
-    from generatedsnamespaces import GenerateDSNamespaceTypePrefixes as GenerateDSNamespaceTypePrefixes_
-except ModulenotfoundExp_ :
+    from generatedsnamespaces import (
+        GenerateDSNamespaceTypePrefixes as GenerateDSNamespaceTypePrefixes_,
+    )
+except ModulenotfoundExp_:
     GenerateDSNamespaceTypePrefixes_ = {}
 
 #
 # You can replace the following class definition by defining an
 # importable module named "generatedscollector" containing a class
 # named "GdsCollector".  See the default class definition below for
 # clues about the possible content of that class.
 #
 try:
     from generatedscollector import GdsCollector as GdsCollector_
-except ModulenotfoundExp_ :
+except ModulenotfoundExp_:
 
     class GdsCollector_(object):
-
         def __init__(self, messages=None):
             if messages is None:
                 self.messages = []
             else:
                 self.messages = messages
 
         def add_message(self, msg):
@@ -155,514 +165,692 @@
 
 #
 # The super-class for enum types
 #
 
 try:
     from enum import Enum
-except ModulenotfoundExp_ :
+except ModulenotfoundExp_:
     Enum = object
 
 #
 # The root super-class for element type classes
 #
 # Calls to the methods in these classes are generated by generateDS.py.
 # You can replace these methods by re-implementing the following class
 #   in a module named generatedssuper.py.
 
 try:
     from generatedssuper import GeneratedsSuper
 except ModulenotfoundExp_ as exp:
+    try:
+        from generatedssupersuper import GeneratedsSuperSuper
+    except ModulenotfoundExp_ as exp:
+
+        class GeneratedsSuperSuper(object):
+            pass
 
-    class GeneratedsSuper(object):
+    class GeneratedsSuper(GeneratedsSuperSuper):
         __hash__ = object.__hash__
-        tzoff_pattern = re_.compile(r'(\+|-)((0\d|1[0-3]):[0-5]\d|14:00)$')
+        tzoff_pattern = re_.compile(r"(\+|-)((0\d|1[0-3]):[0-5]\d|14:00)$")
+
         class _FixedOffsetTZ(datetime_.tzinfo):
             def __init__(self, offset, name):
                 self.__offset = datetime_.timedelta(minutes=offset)
                 self.__name = name
+
             def utcoffset(self, dt):
                 return self.__offset
+
             def tzname(self, dt):
                 return self.__name
+
             def dst(self, dt):
                 return None
-        def gds_format_string(self, input_data, input_name=''):
+
+        def __str__(self):
+            settings = {
+                "str_pretty_print": True,
+                "str_indent_level": 0,
+                "str_namespaceprefix": "",
+                "str_name": self.__class__.__name__,
+                "str_namespacedefs": "",
+            }
+            for n in settings:
+                if hasattr(self, n):
+                    settings[n] = getattr(self, n)
+            if sys.version_info.major == 2:
+                from StringIO import StringIO
+            else:
+                from io import StringIO
+            output = StringIO()
+            self.export(
+                output,
+                settings["str_indent_level"],
+                pretty_print=settings["str_pretty_print"],
+                namespaceprefix_=settings["str_namespaceprefix"],
+                name_=settings["str_name"],
+                namespacedef_=settings["str_namespacedefs"],
+            )
+            strval = output.getvalue()
+            output.close()
+            return strval
+
+        def gds_format_string(self, input_data, input_name=""):
             return input_data
-        def gds_parse_string(self, input_data, node=None, input_name=''):
+
+        def gds_parse_string(self, input_data, node=None, input_name=""):
             return input_data
-        def gds_validate_string(self, input_data, node=None, input_name=''):
+
+        def gds_validate_string(self, input_data, node=None, input_name=""):
             if not input_data:
-                return ''
+                return ""
             else:
                 return input_data
-        def gds_format_base64(self, input_data, input_name=''):
-            return base64.b64encode(input_data)
-        def gds_validate_base64(self, input_data, node=None, input_name=''):
+
+        def gds_format_base64(self, input_data, input_name=""):
+            return base64.b64encode(input_data).decode("ascii")
+
+        def gds_validate_base64(self, input_data, node=None, input_name=""):
             return input_data
-        def gds_format_integer(self, input_data, input_name=''):
-            return '%d' % input_data
-        def gds_parse_integer(self, input_data, node=None, input_name=''):
+
+        def gds_format_integer(self, input_data, input_name=""):
+            return "%d" % int(input_data)
+
+        def gds_parse_integer(self, input_data, node=None, input_name=""):
             try:
                 ival = int(input_data)
             except (TypeError, ValueError) as exp:
-                raise_parse_error(node, 'Requires integer value: %s' % exp)
+                raise_parse_error(node, "Requires integer value: %s" % exp)
             return ival
-        def gds_validate_integer(self, input_data, node=None, input_name=''):
+
+        def gds_validate_integer(self, input_data, node=None, input_name=""):
             try:
                 value = int(input_data)
             except (TypeError, ValueError):
-                raise_parse_error(node, 'Requires integer value')
+                raise_parse_error(node, "Requires integer value")
             return value
-        def gds_format_integer_list(self, input_data, input_name=''):
-            if len(input_data) > 0 and not isinstance(input_data[0], BaseStrType_):
+
+        def gds_format_integer_list(self, input_data, input_name=""):
+            if len(input_data) > 0 and not isinstance(
+                input_data[0], BaseStrType_
+            ):
                 input_data = [str(s) for s in input_data]
-            return '%s' % ' '.join(input_data)
+            return "%s" % " ".join(input_data)
+
         def gds_validate_integer_list(
-                self, input_data, node=None, input_name=''):
+            self, input_data, node=None, input_name=""
+        ):
             values = input_data.split()
             for value in values:
                 try:
                     int(value)
                 except (TypeError, ValueError):
-                    raise_parse_error(node, 'Requires sequence of integer values')
+                    raise_parse_error(
+                        node, "Requires sequence of integer values"
+                    )
             return values
-        def gds_format_float(self, input_data, input_name=''):
-            return ('%.15f' % input_data).rstrip('0')
-        def gds_parse_float(self, input_data, node=None, input_name=''):
+
+        def gds_format_float(self, input_data, input_name=""):
+            value = ("%.15f" % float(input_data)).rstrip("0")
+            if value.endswith("."):
+                value += "0"
+            return value
+
+        def gds_parse_float(self, input_data, node=None, input_name=""):
             try:
                 fval_ = float(input_data)
             except (TypeError, ValueError) as exp:
-                raise_parse_error(node, 'Requires float or double value: %s' % exp)
+                raise_parse_error(
+                    node, "Requires float or double value: %s" % exp
+                )
             return fval_
-        def gds_validate_float(self, input_data, node=None, input_name=''):
+
+        def gds_validate_float(self, input_data, node=None, input_name=""):
             try:
                 value = float(input_data)
             except (TypeError, ValueError):
-                raise_parse_error(node, 'Requires float value')
+                raise_parse_error(node, "Requires float value")
             return value
-        def gds_format_float_list(self, input_data, input_name=''):
-            if len(input_data) > 0 and not isinstance(input_data[0], BaseStrType_):
+
+        def gds_format_float_list(self, input_data, input_name=""):
+            if len(input_data) > 0 and not isinstance(
+                input_data[0], BaseStrType_
+            ):
                 input_data = [str(s) for s in input_data]
-            return '%s' % ' '.join(input_data)
+            return "%s" % " ".join(input_data)
+
         def gds_validate_float_list(
-                self, input_data, node=None, input_name=''):
+            self, input_data, node=None, input_name=""
+        ):
             values = input_data.split()
             for value in values:
                 try:
                     float(value)
                 except (TypeError, ValueError):
-                    raise_parse_error(node, 'Requires sequence of float values')
+                    raise_parse_error(
+                        node, "Requires sequence of float values"
+                    )
             return values
-        def gds_format_decimal(self, input_data, input_name=''):
-            return_value = '%s' % input_data
-            if '.' in return_value:
-                return_value = return_value.rstrip('0')
-                if return_value.endswith('.'):
-                    return_value = return_value.rstrip('.')
+
+        def gds_format_decimal(self, input_data, input_name=""):
+            return_value = "%s" % input_data
+            if "." in return_value:
+                return_value = return_value.rstrip("0")
+                if return_value.endswith("."):
+                    return_value = return_value.rstrip(".")
             return return_value
-        def gds_parse_decimal(self, input_data, node=None, input_name=''):
+
+        def gds_parse_decimal(self, input_data, node=None, input_name=""):
             try:
                 decimal_value = decimal_.Decimal(input_data)
             except (TypeError, ValueError):
-                raise_parse_error(node, 'Requires decimal value')
+                raise_parse_error(node, "Requires decimal value")
             return decimal_value
-        def gds_validate_decimal(self, input_data, node=None, input_name=''):
+
+        def gds_validate_decimal(self, input_data, node=None, input_name=""):
             try:
                 value = decimal_.Decimal(input_data)
             except (TypeError, ValueError):
-                raise_parse_error(node, 'Requires decimal value')
+                raise_parse_error(node, "Requires decimal value")
             return value
-        def gds_format_decimal_list(self, input_data, input_name=''):
-            if len(input_data) > 0 and not isinstance(input_data[0], BaseStrType_):
+
+        def gds_format_decimal_list(self, input_data, input_name=""):
+            if len(input_data) > 0 and not isinstance(
+                input_data[0], BaseStrType_
+            ):
                 input_data = [str(s) for s in input_data]
-            return ' '.join([self.gds_format_decimal(item) for item in input_data])
+            return " ".join(
+                [self.gds_format_decimal(item) for item in input_data]
+            )
+
         def gds_validate_decimal_list(
-                self, input_data, node=None, input_name=''):
+            self, input_data, node=None, input_name=""
+        ):
             values = input_data.split()
             for value in values:
                 try:
                     decimal_.Decimal(value)
                 except (TypeError, ValueError):
-                    raise_parse_error(node, 'Requires sequence of decimal values')
+                    raise_parse_error(
+                        node, "Requires sequence of decimal values"
+                    )
             return values
-        def gds_format_double(self, input_data, input_name=''):
-            return '%s' % input_data
-        def gds_parse_double(self, input_data, node=None, input_name=''):
+
+        def gds_format_double(self, input_data, input_name=""):
+            return "%s" % input_data
+
+        def gds_parse_double(self, input_data, node=None, input_name=""):
             try:
                 fval_ = float(input_data)
             except (TypeError, ValueError) as exp:
-                raise_parse_error(node, 'Requires double or float value: %s' % exp)
+                raise_parse_error(
+                    node, "Requires double or float value: %s" % exp
+                )
             return fval_
-        def gds_validate_double(self, input_data, node=None, input_name=''):
+
+        def gds_validate_double(self, input_data, node=None, input_name=""):
             try:
                 value = float(input_data)
             except (TypeError, ValueError):
-                raise_parse_error(node, 'Requires double or float value')
+                raise_parse_error(node, "Requires double or float value")
             return value
-        def gds_format_double_list(self, input_data, input_name=''):
-            if len(input_data) > 0 and not isinstance(input_data[0], BaseStrType_):
+
+        def gds_format_double_list(self, input_data, input_name=""):
+            if len(input_data) > 0 and not isinstance(
+                input_data[0], BaseStrType_
+            ):
                 input_data = [str(s) for s in input_data]
-            return '%s' % ' '.join(input_data)
+            return "%s" % " ".join(input_data)
+
         def gds_validate_double_list(
-                self, input_data, node=None, input_name=''):
+            self, input_data, node=None, input_name=""
+        ):
             values = input_data.split()
             for value in values:
                 try:
                     float(value)
                 except (TypeError, ValueError):
                     raise_parse_error(
-                        node, 'Requires sequence of double or float values')
+                        node, "Requires sequence of double or float values"
+                    )
             return values
-        def gds_format_boolean(self, input_data, input_name=''):
-            return ('%s' % input_data).lower()
-        def gds_parse_boolean(self, input_data, node=None, input_name=''):
-            if input_data in ('true', '1'):
+
+        def gds_format_boolean(self, input_data, input_name=""):
+            return ("%s" % input_data).lower()
+
+        def gds_parse_boolean(self, input_data, node=None, input_name=""):
+            input_data = input_data.strip()
+            if input_data in ("true", "1"):
                 bval = True
-            elif input_data in ('false', '0'):
+            elif input_data in ("false", "0"):
                 bval = False
             else:
-                raise_parse_error(node, 'Requires boolean value')
+                raise_parse_error(node, "Requires boolean value")
             return bval
-        def gds_validate_boolean(self, input_data, node=None, input_name=''):
-            if input_data not in (True, 1, False, 0, ):
+
+        def gds_validate_boolean(self, input_data, node=None, input_name=""):
+            if input_data not in (
+                True,
+                1,
+                False,
+                0,
+            ):
                 raise_parse_error(
                     node,
-                    'Requires boolean value '
-                    '(one of True, 1, False, 0)')
+                    "Requires boolean value " "(one of True, 1, False, 0)",
+                )
             return input_data
-        def gds_format_boolean_list(self, input_data, input_name=''):
-            if len(input_data) > 0 and not isinstance(input_data[0], BaseStrType_):
+
+        def gds_format_boolean_list(self, input_data, input_name=""):
+            if len(input_data) > 0 and not isinstance(
+                input_data[0], BaseStrType_
+            ):
                 input_data = [str(s) for s in input_data]
-            return '%s' % ' '.join(input_data)
+            return "%s" % " ".join(input_data)
+
         def gds_validate_boolean_list(
-                self, input_data, node=None, input_name=''):
+            self, input_data, node=None, input_name=""
+        ):
             values = input_data.split()
             for value in values:
-                if value not in (True, 1, False, 0, ):
+                value = self.gds_parse_boolean(value, node, input_name)
+                if value not in (
+                    True,
+                    1,
+                    False,
+                    0,
+                ):
                     raise_parse_error(
                         node,
-                        'Requires sequence of boolean values '
-                        '(one of True, 1, False, 0)')
+                        "Requires sequence of boolean values "
+                        "(one of True, 1, False, 0)",
+                    )
             return values
-        def gds_validate_datetime(self, input_data, node=None, input_name=''):
+
+        def gds_validate_datetime(self, input_data, node=None, input_name=""):
             return input_data
-        def gds_format_datetime(self, input_data, input_name=''):
+
+        def gds_format_datetime(self, input_data, input_name=""):
             if input_data.microsecond == 0:
-                _svalue = '%04d-%02d-%02dT%02d:%02d:%02d' % (
+                _svalue = "%04d-%02d-%02dT%02d:%02d:%02d" % (
                     input_data.year,
                     input_data.month,
                     input_data.day,
                     input_data.hour,
                     input_data.minute,
                     input_data.second,
                 )
             else:
-                _svalue = '%04d-%02d-%02dT%02d:%02d:%02d.%s' % (
+                _svalue = "%04d-%02d-%02dT%02d:%02d:%02d.%s" % (
                     input_data.year,
                     input_data.month,
                     input_data.day,
                     input_data.hour,
                     input_data.minute,
                     input_data.second,
-                    ('%f' % (float(input_data.microsecond) / 1000000))[2:],
+                    ("%f" % (float(input_data.microsecond) / 1000000))[2:],
                 )
             if input_data.tzinfo is not None:
                 tzoff = input_data.tzinfo.utcoffset(input_data)
                 if tzoff is not None:
                     total_seconds = tzoff.seconds + (86400 * tzoff.days)
                     if total_seconds == 0:
-                        _svalue += 'Z'
+                        _svalue += "Z"
                     else:
                         if total_seconds < 0:
-                            _svalue += '-'
+                            _svalue += "-"
                             total_seconds *= -1
                         else:
-                            _svalue += '+'
+                            _svalue += "+"
                         hours = total_seconds // 3600
                         minutes = (total_seconds - (hours * 3600)) // 60
-                        _svalue += '{0:02d}:{1:02d}'.format(hours, minutes)
+                        _svalue += "{0:02d}:{1:02d}".format(hours, minutes)
             return _svalue
+
         @classmethod
         def gds_parse_datetime(cls, input_data):
             tz = None
-            if input_data[-1] == 'Z':
-                tz = GeneratedsSuper._FixedOffsetTZ(0, 'UTC')
+            if input_data[-1] == "Z":
+                tz = GeneratedsSuper._FixedOffsetTZ(0, "UTC")
                 input_data = input_data[:-1]
             else:
                 results = GeneratedsSuper.tzoff_pattern.search(input_data)
                 if results is not None:
-                    tzoff_parts = results.group(2).split(':')
+                    tzoff_parts = results.group(2).split(":")
                     tzoff = int(tzoff_parts[0]) * 60 + int(tzoff_parts[1])
-                    if results.group(1) == '-':
+                    if results.group(1) == "-":
                         tzoff *= -1
                     tz = GeneratedsSuper._FixedOffsetTZ(
-                        tzoff, results.group(0))
+                        tzoff, results.group(0)
+                    )
                     input_data = input_data[:-6]
-            time_parts = input_data.split('.')
+            time_parts = input_data.split(".")
             if len(time_parts) > 1:
-                micro_seconds = int(float('0.' + time_parts[1]) * 1000000)
-                input_data = '%s.%s' % (
-                    time_parts[0], "{}".format(micro_seconds).rjust(6, "0"), )
+                micro_seconds = int(float("0." + time_parts[1]) * 1000000)
+                input_data = "%s.%s" % (
+                    time_parts[0],
+                    "{}".format(micro_seconds).rjust(6, "0"),
+                )
                 dt = datetime_.datetime.strptime(
-                    input_data, '%Y-%m-%dT%H:%M:%S.%f')
+                    input_data, "%Y-%m-%dT%H:%M:%S.%f"
+                )
             else:
                 dt = datetime_.datetime.strptime(
-                    input_data, '%Y-%m-%dT%H:%M:%S')
+                    input_data, "%Y-%m-%dT%H:%M:%S"
+                )
             dt = dt.replace(tzinfo=tz)
             return dt
-        def gds_validate_date(self, input_data, node=None, input_name=''):
+
+        def gds_validate_date(self, input_data, node=None, input_name=""):
             return input_data
-        def gds_format_date(self, input_data, input_name=''):
-            _svalue = '%04d-%02d-%02d' % (
+
+        def gds_format_date(self, input_data, input_name=""):
+            _svalue = "%04d-%02d-%02d" % (
                 input_data.year,
                 input_data.month,
                 input_data.day,
             )
             try:
                 if input_data.tzinfo is not None:
                     tzoff = input_data.tzinfo.utcoffset(input_data)
                     if tzoff is not None:
                         total_seconds = tzoff.seconds + (86400 * tzoff.days)
                         if total_seconds == 0:
-                            _svalue += 'Z'
+                            _svalue += "Z"
                         else:
                             if total_seconds < 0:
-                                _svalue += '-'
+                                _svalue += "-"
                                 total_seconds *= -1
                             else:
-                                _svalue += '+'
+                                _svalue += "+"
                             hours = total_seconds // 3600
                             minutes = (total_seconds - (hours * 3600)) // 60
-                            _svalue += '{0:02d}:{1:02d}'.format(
-                                hours, minutes)
+                            _svalue += "{0:02d}:{1:02d}".format(hours, minutes)
             except AttributeError:
                 pass
             return _svalue
+
         @classmethod
         def gds_parse_date(cls, input_data):
             tz = None
-            if input_data[-1] == 'Z':
-                tz = GeneratedsSuper._FixedOffsetTZ(0, 'UTC')
+            if input_data[-1] == "Z":
+                tz = GeneratedsSuper._FixedOffsetTZ(0, "UTC")
                 input_data = input_data[:-1]
             else:
                 results = GeneratedsSuper.tzoff_pattern.search(input_data)
                 if results is not None:
-                    tzoff_parts = results.group(2).split(':')
+                    tzoff_parts = results.group(2).split(":")
                     tzoff = int(tzoff_parts[0]) * 60 + int(tzoff_parts[1])
-                    if results.group(1) == '-':
+                    if results.group(1) == "-":
                         tzoff *= -1
                     tz = GeneratedsSuper._FixedOffsetTZ(
-                        tzoff, results.group(0))
+                        tzoff, results.group(0)
+                    )
                     input_data = input_data[:-6]
-            dt = datetime_.datetime.strptime(input_data, '%Y-%m-%d')
+            dt = datetime_.datetime.strptime(input_data, "%Y-%m-%d")
             dt = dt.replace(tzinfo=tz)
             return dt.date()
-        def gds_validate_time(self, input_data, node=None, input_name=''):
+
+        def gds_validate_time(self, input_data, node=None, input_name=""):
             return input_data
-        def gds_format_time(self, input_data, input_name=''):
+
+        def gds_format_time(self, input_data, input_name=""):
             if input_data.microsecond == 0:
-                _svalue = '%02d:%02d:%02d' % (
+                _svalue = "%02d:%02d:%02d" % (
                     input_data.hour,
                     input_data.minute,
                     input_data.second,
                 )
             else:
-                _svalue = '%02d:%02d:%02d.%s' % (
+                _svalue = "%02d:%02d:%02d.%s" % (
                     input_data.hour,
                     input_data.minute,
                     input_data.second,
-                    ('%f' % (float(input_data.microsecond) / 1000000))[2:],
+                    ("%f" % (float(input_data.microsecond) / 1000000))[2:],
                 )
             if input_data.tzinfo is not None:
                 tzoff = input_data.tzinfo.utcoffset(input_data)
                 if tzoff is not None:
                     total_seconds = tzoff.seconds + (86400 * tzoff.days)
                     if total_seconds == 0:
-                        _svalue += 'Z'
+                        _svalue += "Z"
                     else:
                         if total_seconds < 0:
-                            _svalue += '-'
+                            _svalue += "-"
                             total_seconds *= -1
                         else:
-                            _svalue += '+'
+                            _svalue += "+"
                         hours = total_seconds // 3600
                         minutes = (total_seconds - (hours * 3600)) // 60
-                        _svalue += '{0:02d}:{1:02d}'.format(hours, minutes)
+                        _svalue += "{0:02d}:{1:02d}".format(hours, minutes)
             return _svalue
+
         def gds_validate_simple_patterns(self, patterns, target):
             # pat is a list of lists of strings/patterns.
             # The target value must match at least one of the patterns
             # in order for the test to succeed.
             found1 = True
+            target = str(target)
             for patterns1 in patterns:
                 found2 = False
                 for patterns2 in patterns1:
                     mo = re_.search(patterns2, target)
                     if mo is not None and len(mo.group(0)) == len(target):
                         found2 = True
                         break
                 if not found2:
                     found1 = False
                     break
             return found1
+
         @classmethod
         def gds_parse_time(cls, input_data):
             tz = None
-            if input_data[-1] == 'Z':
-                tz = GeneratedsSuper._FixedOffsetTZ(0, 'UTC')
+            if input_data[-1] == "Z":
+                tz = GeneratedsSuper._FixedOffsetTZ(0, "UTC")
                 input_data = input_data[:-1]
             else:
                 results = GeneratedsSuper.tzoff_pattern.search(input_data)
                 if results is not None:
-                    tzoff_parts = results.group(2).split(':')
+                    tzoff_parts = results.group(2).split(":")
                     tzoff = int(tzoff_parts[0]) * 60 + int(tzoff_parts[1])
-                    if results.group(1) == '-':
+                    if results.group(1) == "-":
                         tzoff *= -1
                     tz = GeneratedsSuper._FixedOffsetTZ(
-                        tzoff, results.group(0))
+                        tzoff, results.group(0)
+                    )
                     input_data = input_data[:-6]
-            if len(input_data.split('.')) > 1:
-                dt = datetime_.datetime.strptime(input_data, '%H:%M:%S.%f')
+            if len(input_data.split(".")) > 1:
+                dt = datetime_.datetime.strptime(input_data, "%H:%M:%S.%f")
             else:
-                dt = datetime_.datetime.strptime(input_data, '%H:%M:%S')
+                dt = datetime_.datetime.strptime(input_data, "%H:%M:%S")
             dt = dt.replace(tzinfo=tz)
             return dt.time()
+
         def gds_check_cardinality_(
-                self, value, input_name,
-                min_occurs=0, max_occurs=1, required=None):
+            self, value, input_name, min_occurs=0, max_occurs=1, required=None
+        ):
             if value is None:
                 length = 0
             elif isinstance(value, list):
                 length = len(value)
             else:
                 length = 1
-            if required is not None :
+            if required is not None:
                 if required and length < 1:
                     self.gds_collector_.add_message(
                         "Required value {}{} is missing".format(
-                            input_name, self.gds_get_node_lineno_()))
+                            input_name, self.gds_get_node_lineno_()
+                        )
+                    )
             if length < min_occurs:
                 self.gds_collector_.add_message(
                     "Number of values for {}{} is below "
                     "the minimum allowed, "
                     "expected at least {}, found {}".format(
-                        input_name, self.gds_get_node_lineno_(),
-                        min_occurs, length))
+                        input_name,
+                        self.gds_get_node_lineno_(),
+                        min_occurs,
+                        length,
+                    )
+                )
             elif length > max_occurs:
                 self.gds_collector_.add_message(
                     "Number of values for {}{} is above "
                     "the maximum allowed, "
                     "expected at most {}, found {}".format(
-                        input_name, self.gds_get_node_lineno_(),
-                        max_occurs, length))
+                        input_name,
+                        self.gds_get_node_lineno_(),
+                        max_occurs,
+                        length,
+                    )
+                )
+
         def gds_validate_builtin_ST_(
-                self, validator, value, input_name,
-                min_occurs=None, max_occurs=None, required=None):
+            self,
+            validator,
+            value,
+            input_name,
+            min_occurs=None,
+            max_occurs=None,
+            required=None,
+        ):
             if value is not None:
                 try:
                     validator(value, input_name=input_name)
                 except GDSParseError as parse_error:
                     self.gds_collector_.add_message(str(parse_error))
+
         def gds_validate_defined_ST_(
-                self, validator, value, input_name,
-                min_occurs=None, max_occurs=None, required=None):
+            self,
+            validator,
+            value,
+            input_name,
+            min_occurs=None,
+            max_occurs=None,
+            required=None,
+        ):
             if value is not None:
                 try:
                     validator(value)
                 except GDSParseError as parse_error:
                     self.gds_collector_.add_message(str(parse_error))
+
         def gds_str_lower(self, instring):
             return instring.lower()
+
         def get_path_(self, node):
             path_list = []
             self.get_path_list_(node, path_list)
             path_list.reverse()
-            path = '/'.join(path_list)
+            path = "/".join(path_list)
             return path
-        Tag_strip_pattern_ = re_.compile(r'\{.*\}')
+
+        Tag_strip_pattern_ = re_.compile(r"\{.*\}")
+
         def get_path_list_(self, node, path_list):
             if node is None:
                 return
-            tag = GeneratedsSuper.Tag_strip_pattern_.sub('', node.tag)
+            tag = GeneratedsSuper.Tag_strip_pattern_.sub("", node.tag)
             if tag:
                 path_list.append(tag)
             self.get_path_list_(node.getparent(), path_list)
+
         def get_class_obj_(self, node, default_class=None):
             class_obj1 = default_class
-            if 'xsi' in node.nsmap:
-                classname = node.get('{%s}type' % node.nsmap['xsi'])
+            if "xsi" in node.nsmap:
+                classname = node.get("{%s}type" % node.nsmap["xsi"])
                 if classname is not None:
-                    names = classname.split(':')
+                    names = classname.split(":")
                     if len(names) == 2:
                         classname = names[1]
                     class_obj2 = globals().get(classname)
                     if class_obj2 is not None:
                         class_obj1 = class_obj2
             return class_obj1
+
         def gds_build_any(self, node, type_name=None):
             # provide default value in case option --disable-xml is used.
             content = ""
             content = etree_.tostring(node, encoding="unicode")
             return content
+
         @classmethod
         def gds_reverse_node_mapping(cls, mapping):
             return dict(((v, k) for k, v in mapping.items()))
+
         @staticmethod
         def gds_encode(instring):
             if sys.version_info.major == 2:
                 if ExternalEncoding:
                     encoding = ExternalEncoding
                 else:
-                    encoding = 'utf-8'
+                    encoding = "utf-8"
                 return instring.encode(encoding)
             else:
                 return instring
+
         @staticmethod
         def convert_unicode(instring):
             if isinstance(instring, str):
                 result = quote_xml(instring)
             elif sys.version_info.major == 2 and isinstance(instring, unicode):
-                result = quote_xml(instring).encode('utf8')
+                result = quote_xml(instring).encode("utf8")
             else:
                 result = GeneratedsSuper.gds_encode(str(instring))
             return result
+
         def __eq__(self, other):
             def excl_select_objs_(obj):
-                return (obj[0] != 'parent_object_' and
-                        obj[0] != 'gds_collector_')
+                return (
+                    obj[0] != "parent_object_" and obj[0] != "gds_collector_"
+                )
+
             if type(self) != type(other):
                 return False
-            return all(x == y for x, y in zip_longest(
-                filter(excl_select_objs_, self.__dict__.items()),
-                filter(excl_select_objs_, other.__dict__.items())))
+            return all(
+                x == y
+                for x, y in zip_longest(
+                    filter(excl_select_objs_, self.__dict__.items()),
+                    filter(excl_select_objs_, other.__dict__.items()),
+                )
+            )
+
         def __ne__(self, other):
             return not self.__eq__(other)
+
         # Django ETL transform hooks.
         def gds_djo_etl_transform(self):
             pass
+
         def gds_djo_etl_transform_db_obj(self, dbobj):
             pass
+
         # SQLAlchemy ETL transform hooks.
         def gds_sqa_etl_transform(self):
             return 0, None
+
         def gds_sqa_etl_transform_db_obj(self, dbobj):
             pass
+
         def gds_get_node_lineno_(self):
-            if (hasattr(self, "gds_elementtree_node_") and
-                    self.gds_elementtree_node_ is not None):
-                return ' near line {}'.format(
-                    self.gds_elementtree_node_.sourceline)
+            if (
+                hasattr(self, "gds_elementtree_node_")
+                and self.gds_elementtree_node_ is not None
+            ):
+                return " near line {}".format(
+                    self.gds_elementtree_node_.sourceline
+                )
             else:
                 return ""
 
-
     def getSubclassFromModule_(module, class_):
-        '''Get the subclass of a class from a specific module.'''
-        name = class_.__name__ + 'Sub'
+        """Get the subclass of a class from a specific module."""
+        name = class_.__name__ + "Sub"
         if hasattr(module, name):
             return getattr(module, name)
         else:
             return None
 
 
 #
@@ -680,131 +868,145 @@
 # IPython shell:
 #    ipshell('<some message> -- Entering ipshell.\nHit Ctrl-D to exit')
 
 #
 # Globals
 #
 
-ExternalEncoding = ''
+ExternalEncoding = ""
 # Set this to false in order to deactivate during export, the use of
 # name space prefixes captured from the input document.
 UseCapturedNS_ = True
 CapturedNsmap_ = {}
-Tag_pattern_ = re_.compile(r'({.*})?(.*)')
+Tag_pattern_ = re_.compile(r"({.*})?(.*)")
 String_cleanup_pat_ = re_.compile(r"[\n\r\s]+")
-Namespace_extract_pat_ = re_.compile(r'{(.*)}(.*)')
+Namespace_extract_pat_ = re_.compile(r"{(.*)}(.*)")
 CDATA_pattern_ = re_.compile(r"<!\[CDATA\[.*?\]\]>", re_.DOTALL)
 
 # Change this to redirect the generated superclass module to use a
 # specific subclass module.
 CurrentSubclassModule_ = None
 
 #
 # Support/utility functions.
 #
 
 
 def showIndent(outfile, level, pretty_print=True):
     if pretty_print:
         for idx in range(level):
-            outfile.write('    ')
+            outfile.write("    ")
 
 
 def quote_xml(inStr):
     "Escape markup chars, but do not modify CDATA sections."
     if not inStr:
-        return ''
-    s1 = (isinstance(inStr, BaseStrType_) and inStr or '%s' % inStr)
-    s2 = ''
+        return ""
+    s1 = isinstance(inStr, BaseStrType_) and inStr or "%s" % inStr
+    s2 = ""
     pos = 0
     matchobjects = CDATA_pattern_.finditer(s1)
     for mo in matchobjects:
-        s3 = s1[pos:mo.start()]
+        s3 = s1[pos : mo.start()]
         s2 += quote_xml_aux(s3)
-        s2 += s1[mo.start():mo.end()]
+        s2 += s1[mo.start() : mo.end()]
         pos = mo.end()
     s3 = s1[pos:]
     s2 += quote_xml_aux(s3)
     return s2
 
 
 def quote_xml_aux(inStr):
-    s1 = inStr.replace('&', '&amp;')
-    s1 = s1.replace('<', '&lt;')
-    s1 = s1.replace('>', '&gt;')
+    s1 = inStr.replace("&", "&amp;")
+    s1 = s1.replace("<", "&lt;")
+    s1 = s1.replace(">", "&gt;")
     return s1
 
 
 def quote_attrib(inStr):
-    s1 = (isinstance(inStr, BaseStrType_) and inStr or '%s' % inStr)
-    s1 = s1.replace('&', '&amp;')
-    s1 = s1.replace('<', '&lt;')
-    s1 = s1.replace('>', '&gt;')
+    s1 = isinstance(inStr, BaseStrType_) and inStr or "%s" % inStr
+    s1 = s1.replace("&", "&amp;")
+    s1 = s1.replace("<", "&lt;")
+    s1 = s1.replace(">", "&gt;")
+    s1 = s1.replace("\n", "&#10;")
     if '"' in s1:
         if "'" in s1:
             s1 = '"%s"' % s1.replace('"', "&quot;")
         else:
             s1 = "'%s'" % s1
     else:
         s1 = '"%s"' % s1
     return s1
 
 
 def quote_python(inStr):
     s1 = inStr
     if s1.find("'") == -1:
-        if s1.find('\n') == -1:
+        if s1.find("\n") == -1:
             return "'%s'" % s1
         else:
             return "'''%s'''" % s1
     else:
         if s1.find('"') != -1:
             s1 = s1.replace('"', '\\"')
-        if s1.find('\n') == -1:
+        if s1.find("\n") == -1:
             return '"%s"' % s1
         else:
             return '"""%s"""' % s1
 
 
 def get_all_text_(node):
     if node.text is not None:
         text = node.text
     else:
-        text = ''
+        text = ""
     for child in node:
         if child.tail is not None:
             text += child.tail
     return text
 
 
 def find_attr_value_(attr_name, node):
     attrs = node.attrib
-    attr_parts = attr_name.split(':')
+    attr_parts = attr_name.split(":")
     value = None
     if len(attr_parts) == 1:
         value = attrs.get(attr_name)
     elif len(attr_parts) == 2:
         prefix, name = attr_parts
-        namespace = node.nsmap.get(prefix)
+        if prefix == "xml":
+            namespace = "http://www.w3.org/XML/1998/namespace"
+        else:
+            namespace = node.nsmap.get(prefix)
         if namespace is not None:
-            value = attrs.get('{%s}%s' % (namespace, name, ))
+            value = attrs.get(
+                "{%s}%s"
+                % (
+                    namespace,
+                    name,
+                )
+            )
     return value
 
 
 def encode_str_2_3(instr):
     return instr
 
 
 class GDSParseError(Exception):
     pass
 
 
 def raise_parse_error(node, msg):
     if node is not None:
-        msg = '%s (element %s/line %d)' % (msg, node.tag, node.sourceline, )
+        msg = "%s (element %s/line %d)" % (
+            msg,
+            node.tag,
+            node.sourceline,
+        )
     raise GDSParseError(msg)
 
 
 class MixedContainer:
     # Constants for category:
     CategoryNone = 0
     CategoryText = 1
@@ -816,440 +1018,750 @@
     TypeString = 2
     TypeInteger = 3
     TypeFloat = 4
     TypeDecimal = 5
     TypeDouble = 6
     TypeBoolean = 7
     TypeBase64 = 8
+
     def __init__(self, category, content_type, name, value):
         self.category = category
         self.content_type = content_type
         self.name = name
         self.value = value
+
     def getCategory(self):
         return self.category
+
     def getContenttype(self, content_type):
         return self.content_type
+
     def getValue(self):
         return self.value
+
     def getName(self):
         return self.name
-    def export(self, outfile, level, name, namespace,
-               pretty_print=True):
+
+    def export(self, outfile, level, name, namespace, pretty_print=True):
         if self.category == MixedContainer.CategoryText:
             # Prevent exporting empty content as empty lines.
             if self.value.strip():
                 outfile.write(self.value)
         elif self.category == MixedContainer.CategorySimple:
             self.exportSimple(outfile, level, name)
-        else:    # category == MixedContainer.CategoryComplex
+        else:  # category == MixedContainer.CategoryComplex
             self.value.export(
-                outfile, level, namespace, name_=name,
-                pretty_print=pretty_print)
+                outfile,
+                level,
+                namespace,
+                name_=name,
+                pretty_print=pretty_print,
+            )
+
     def exportSimple(self, outfile, level, name):
         if self.content_type == MixedContainer.TypeString:
-            outfile.write('<%s>%s</%s>' % (
-                self.name, self.value, self.name))
-        elif self.content_type == MixedContainer.TypeInteger or \
-                self.content_type == MixedContainer.TypeBoolean:
-            outfile.write('<%s>%d</%s>' % (
-                self.name, self.value, self.name))
-        elif self.content_type == MixedContainer.TypeFloat or \
-                self.content_type == MixedContainer.TypeDecimal:
-            outfile.write('<%s>%f</%s>' % (
-                self.name, self.value, self.name))
+            outfile.write("<%s>%s</%s>" % (self.name, self.value, self.name))
+        elif (
+            self.content_type == MixedContainer.TypeInteger
+            or self.content_type == MixedContainer.TypeBoolean
+        ):
+            outfile.write("<%s>%d</%s>" % (self.name, self.value, self.name))
+        elif (
+            self.content_type == MixedContainer.TypeFloat
+            or self.content_type == MixedContainer.TypeDecimal
+        ):
+            outfile.write("<%s>%f</%s>" % (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeDouble:
-            outfile.write('<%s>%g</%s>' % (
-                self.name, self.value, self.name))
+            outfile.write("<%s>%g</%s>" % (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeBase64:
-            outfile.write('<%s>%s</%s>' % (
-                self.name,
-                base64.b64encode(self.value),
-                self.name))
-    def to_etree(self, element, mapping_=None, nsmap_=None):
+            outfile.write(
+                "<%s>%s</%s>"
+                % (self.name, base64.b64encode(self.value), self.name)
+            )
+
+    def to_etree(
+        self, element, mapping_=None, reverse_mapping_=None, nsmap_=None
+    ):
         if self.category == MixedContainer.CategoryText:
             # Prevent exporting empty content as empty lines.
             if self.value.strip():
                 if len(element) > 0:
                     if element[-1].tail is None:
                         element[-1].tail = self.value
                     else:
                         element[-1].tail += self.value
                 else:
                     if element.text is None:
                         element.text = self.value
                     else:
                         element.text += self.value
         elif self.category == MixedContainer.CategorySimple:
-            subelement = etree_.SubElement(
-                element, '%s' % self.name)
+            subelement = etree_.SubElement(element, "%s" % self.name)
             subelement.text = self.to_etree_simple()
-        else:    # category == MixedContainer.CategoryComplex
+        else:  # category == MixedContainer.CategoryComplex
             self.value.to_etree(element)
-    def to_etree_simple(self, mapping_=None, nsmap_=None):
+
+    def to_etree_simple(
+        self, mapping_=None, reverse_mapping_=None, nsmap_=None
+    ):
         if self.content_type == MixedContainer.TypeString:
             text = self.value
-        elif (self.content_type == MixedContainer.TypeInteger or
-                self.content_type == MixedContainer.TypeBoolean):
-            text = '%d' % self.value
-        elif (self.content_type == MixedContainer.TypeFloat or
-                self.content_type == MixedContainer.TypeDecimal):
-            text = '%f' % self.value
+        elif (
+            self.content_type == MixedContainer.TypeInteger
+            or self.content_type == MixedContainer.TypeBoolean
+        ):
+            text = "%d" % self.value
+        elif (
+            self.content_type == MixedContainer.TypeFloat
+            or self.content_type == MixedContainer.TypeDecimal
+        ):
+            text = "%f" % self.value
         elif self.content_type == MixedContainer.TypeDouble:
-            text = '%g' % self.value
+            text = "%g" % self.value
         elif self.content_type == MixedContainer.TypeBase64:
-            text = '%s' % base64.b64encode(self.value)
+            text = "%s" % base64.b64encode(self.value)
         return text
+
     def exportLiteral(self, outfile, level, name):
         if self.category == MixedContainer.CategoryText:
             showIndent(outfile, level)
             outfile.write(
-                'model_.MixedContainer(%d, %d, "%s", "%s"),\n' % (
-                    self.category, self.content_type,
-                    self.name, self.value))
+                'model_.MixedContainer(%d, %d, "%s", "%s"),\n'
+                % (self.category, self.content_type, self.name, self.value)
+            )
         elif self.category == MixedContainer.CategorySimple:
             showIndent(outfile, level)
             outfile.write(
-                'model_.MixedContainer(%d, %d, "%s", "%s"),\n' % (
-                    self.category, self.content_type,
-                    self.name, self.value))
-        else:    # category == MixedContainer.CategoryComplex
+                'model_.MixedContainer(%d, %d, "%s", "%s"),\n'
+                % (self.category, self.content_type, self.name, self.value)
+            )
+        else:  # category == MixedContainer.CategoryComplex
             showIndent(outfile, level)
             outfile.write(
-                'model_.MixedContainer(%d, %d, "%s",\n' % (
-                    self.category, self.content_type, self.name,))
+                'model_.MixedContainer(%d, %d, "%s",\n'
+                % (
+                    self.category,
+                    self.content_type,
+                    self.name,
+                )
+            )
             self.value.exportLiteral(outfile, level + 1)
             showIndent(outfile, level)
-            outfile.write(')\n')
+            outfile.write(")\n")
 
 
 class MemberSpec_(object):
-    def __init__(self, name='', data_type='', container=0,
-            optional=0, child_attrs=None, choice=None):
+    def __init__(
+        self,
+        name="",
+        data_type="",
+        container=0,
+        optional=0,
+        child_attrs=None,
+        choice=None,
+    ):
         self.name = name
         self.data_type = data_type
         self.container = container
         self.child_attrs = child_attrs
         self.choice = choice
         self.optional = optional
-    def set_name(self, name): self.name = name
-    def get_name(self): return self.name
-    def set_data_type(self, data_type): self.data_type = data_type
-    def get_data_type_chain(self): return self.data_type
+
+    def set_name(self, name):
+        self.name = name
+
+    def get_name(self):
+        return self.name
+
+    def set_data_type(self, data_type):
+        self.data_type = data_type
+
+    def get_data_type_chain(self):
+        return self.data_type
+
     def get_data_type(self):
         if isinstance(self.data_type, list):
             if len(self.data_type) > 0:
                 return self.data_type[-1]
             else:
-                return 'xs:string'
+                return "xs:string"
         else:
             return self.data_type
-    def set_container(self, container): self.container = container
-    def get_container(self): return self.container
-    def set_child_attrs(self, child_attrs): self.child_attrs = child_attrs
-    def get_child_attrs(self): return self.child_attrs
-    def set_choice(self, choice): self.choice = choice
-    def get_choice(self): return self.choice
-    def set_optional(self, optional): self.optional = optional
-    def get_optional(self): return self.optional
+
+    def set_container(self, container):
+        self.container = container
+
+    def get_container(self):
+        return self.container
+
+    def set_child_attrs(self, child_attrs):
+        self.child_attrs = child_attrs
+
+    def get_child_attrs(self):
+        return self.child_attrs
+
+    def set_choice(self, choice):
+        self.choice = choice
+
+    def get_choice(self):
+        return self.choice
+
+    def set_optional(self, optional):
+        self.optional = optional
+
+    def get_optional(self):
+        return self.optional
 
 
 def _cast(typ, value):
     if typ is None or value is None:
         return value
     return typ(value)
 
+
 #
 # Data representation classes.
 #
 
 
 class root(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, specVersion=None, URLBase=None, device=None, gds_collector_=None, **kwargs_):
+
+    def __init__(
+        self,
+        specVersion=None,
+        URLBase=None,
+        device=None,
+        gds_collector_=None,
+        **kwargs_
+    ):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
-        self.parent_object_ = kwargs_.get('parent_object_')
+        self.parent_object_ = kwargs_.get("parent_object_")
         self.ns_prefix_ = None
         self.specVersion = specVersion
         self.specVersion_nsprefix_ = None
         self.URLBase = URLBase
         self.URLBase_nsprefix_ = None
         self.device = device
         self.device_nsprefix_ = None
         self.anyAttributes_ = {}
+
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
-            subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, root)
+            subclass = getSubclassFromModule_(CurrentSubclassModule_, root)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
         if root.subclass:
             return root.subclass(*args_, **kwargs_)
         else:
             return root(*args_, **kwargs_)
+
     factory = staticmethod(factory)
+
     def get_ns_prefix_(self):
         return self.ns_prefix_
+
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
+
     def get_specVersion(self):
         return self.specVersion
+
     def set_specVersion(self, specVersion):
         self.specVersion = specVersion
+
     def get_URLBase(self):
         return self.URLBase
+
     def set_URLBase(self, URLBase):
         self.URLBase = URLBase
+
     def get_device(self):
         return self.device
+
     def set_device(self, device):
         self.device = device
-    def get_anyAttributes_(self): return self.anyAttributes_
-    def set_anyAttributes_(self, anyAttributes_): self.anyAttributes_ = anyAttributes_
-    def hasContent_(self):
+
+    def get_anyAttributes_(self):
+        return self.anyAttributes_
+
+    def set_anyAttributes_(self, anyAttributes_):
+        self.anyAttributes_ = anyAttributes_
+
+    def has__content(self):
         if (
-            self.specVersion is not None or
-            self.URLBase is not None or
-            self.device is not None
+            self.specVersion is not None
+            or self.URLBase is not None
+            or self.device is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ', name_='root', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('root')
+
+    def export(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ',
+        name_="root",
+        pretty_print=True,
+    ):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get("root")
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'root':
+            eol_ = ""
+        if self.original_tagname_ is not None and name_ == "root":
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
-            namespaceprefix_ = self.ns_prefix_ + ':'
+            namespaceprefix_ = self.ns_prefix_ + ":"
         showIndent(outfile, level, pretty_print)
-        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        outfile.write(
+            "<%s%s%s"
+            % (
+                namespaceprefix_,
+                name_,
+                namespacedef_ and " " + namespacedef_ or "",
+            )
+        )
         already_processed = set()
-        self.exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='root')
-        if self.hasContent_():
-            outfile.write('>%s' % (eol_, ))
-            self.exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='root', pretty_print=pretty_print)
+        self._exportAttributes(
+            outfile, level, already_processed, namespaceprefix_, name_="root"
+        )
+        if self.has__content():
+            outfile.write(">%s" % (eol_,))
+            self._exportChildren(
+                outfile,
+                level + 1,
+                namespaceprefix_,
+                namespacedef_,
+                name_="root",
+                pretty_print=pretty_print,
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+            outfile.write("</%s%s>%s" % (namespaceprefix_, name_, eol_))
         else:
-            outfile.write('/>%s' % (eol_, ))
-    def exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='root'):
+            outfile.write("/>%s" % (eol_,))
+
+    def _exportAttributes(
+        self,
+        outfile,
+        level,
+        already_processed,
+        namespaceprefix_="",
+        name_="root",
+    ):
         unique_counter = 0
         for name, value in self.anyAttributes_.items():
-            xsinamespaceprefix = 'xsi'
-            xsinamespace1 = 'http://www.w3.org/2001/XMLSchema-instance'
-            xsinamespace2 = '{%s}' % (xsinamespace1, )
+            xsinamespaceprefix = "xsi"
+            xsinamespace1 = "http://www.w3.org/2001/XMLSchema-instance"
+            xsinamespace2 = "{%s}" % (xsinamespace1,)
             if name.startswith(xsinamespace2):
-                name1 = name[len(xsinamespace2):]
-                name2 = '%s:%s' % (xsinamespaceprefix, name1, )
+                name1 = name[len(xsinamespace2) :]
+                name2 = "%s:%s" % (
+                    xsinamespaceprefix,
+                    name1,
+                )
                 if name2 not in already_processed:
                     already_processed.add(name2)
-                    outfile.write(' %s=%s' % (name2, quote_attrib(value), ))
+                    outfile.write(
+                        " %s=%s"
+                        % (
+                            name2,
+                            quote_attrib(value),
+                        )
+                    )
             else:
                 mo = re_.match(Namespace_extract_pat_, name)
                 if mo is not None:
                     namespace, name = mo.group(1, 2)
                     if name not in already_processed:
                         already_processed.add(name)
-                        if namespace == 'http://www.w3.org/XML/1998/namespace':
-                            outfile.write(' %s=%s' % (
-                                name, quote_attrib(value), ))
+                        if namespace == "http://www.w3.org/XML/1998/namespace":
+                            outfile.write(
+                                " %s=%s"
+                                % (
+                                    name,
+                                    quote_attrib(value),
+                                )
+                            )
                         else:
                             unique_counter += 1
-                            outfile.write(' xmlns:%d="%s"' % (
-                                unique_counter, namespace, ))
-                            outfile.write(' %d:%s=%s' % (
-                                unique_counter, name, quote_attrib(value), ))
+                            outfile.write(
+                                ' xmlns:%d="%s"'
+                                % (
+                                    unique_counter,
+                                    namespace,
+                                )
+                            )
+                            outfile.write(
+                                " %d:%s=%s"
+                                % (
+                                    unique_counter,
+                                    name,
+                                    quote_attrib(value),
+                                )
+                            )
                 else:
                     if name not in already_processed:
                         already_processed.add(name)
-                        outfile.write(' %s=%s' % (
-                            name, quote_attrib(value), ))
+                        outfile.write(
+                            " %s=%s"
+                            % (
+                                name,
+                                quote_attrib(value),
+                            )
+                        )
         pass
-    def exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ', name_='root', fromsubclass_=False, pretty_print=True):
+
+    def _exportChildren(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ',
+        name_="root",
+        fromsubclass_=False,
+        pretty_print=True,
+    ):
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
+            eol_ = ""
         if self.specVersion is not None:
-            namespaceprefix_ = self.specVersion_nsprefix_ + ':' if (UseCapturedNS_ and self.specVersion_nsprefix_) else ''
-            self.specVersion.export(outfile, level, namespaceprefix_, namespacedef_='', name_='specVersion', pretty_print=pretty_print)
+            namespaceprefix_ = (
+                self.specVersion_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.specVersion_nsprefix_)
+                else ""
+            )
+            self.specVersion.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="specVersion",
+                pretty_print=pretty_print,
+            )
         if self.URLBase is not None:
-            namespaceprefix_ = self.URLBase_nsprefix_ + ':' if (UseCapturedNS_ and self.URLBase_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.URLBase_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.URLBase_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%sURLBase>%s</%sURLBase>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.URLBase), input_name='URLBase')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%sURLBase>%s</%sURLBase>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(self.URLBase), input_name="URLBase"
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.device is not None:
-            namespaceprefix_ = self.device_nsprefix_ + ':' if (UseCapturedNS_ and self.device_nsprefix_) else ''
-            self.device.export(outfile, level, namespaceprefix_, namespacedef_='', name_='device', pretty_print=pretty_print)
+            namespaceprefix_ = (
+                self.device_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.device_nsprefix_)
+                else ""
+            )
+            self.device.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="device",
+                pretty_print=pretty_print,
+            )
+
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
-        self.buildAttributes(node, node.attrib, already_processed)
+        self._buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
-            self.buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+            self._buildChildren(
+                child, node, nodeName_, gds_collector_=gds_collector_
+            )
         return self
-    def buildAttributes(self, node, attrs, already_processed):
+
+    def _buildAttributes(self, node, attrs, already_processed):
         self.anyAttributes_ = {}
         for name, value in attrs.items():
             if name not in already_processed:
                 self.anyAttributes_[name] = value
-    def buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
-        if nodeName_ == 'specVersion':
+
+    def _buildChildren(
+        self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
+    ):
+        if nodeName_ == "specVersion":
             obj_ = SpecVersionType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.specVersion = obj_
-            obj_.original_tagname_ = 'specVersion'
-        elif nodeName_ == 'URLBase':
+            obj_.original_tagname_ = "specVersion"
+        elif nodeName_ == "URLBase":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'URLBase')
-            value_ = self.gds_validate_string(value_, node, 'URLBase')
+            value_ = self.gds_parse_string(value_, node, "URLBase")
+            value_ = self.gds_validate_string(value_, node, "URLBase")
             self.URLBase = value_
             self.URLBase_nsprefix_ = child_.prefix
-        elif nodeName_ == 'device':
+        elif nodeName_ == "device":
             obj_ = DeviceType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.device = obj_
-            obj_.original_tagname_ = 'device'
+            obj_.original_tagname_ = "device"
+
+
 # end class root
 
 
 class SpecVersionType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
+
     def __init__(self, major=None, minor=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
-        self.parent_object_ = kwargs_.get('parent_object_')
+        self.parent_object_ = kwargs_.get("parent_object_")
         self.ns_prefix_ = None
         self.major = major
         self.major_nsprefix_ = None
         self.minor = minor
         self.minor_nsprefix_ = None
+
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, SpecVersionType)
+                CurrentSubclassModule_, SpecVersionType
+            )
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
         if SpecVersionType.subclass:
             return SpecVersionType.subclass(*args_, **kwargs_)
         else:
             return SpecVersionType(*args_, **kwargs_)
+
     factory = staticmethod(factory)
+
     def get_ns_prefix_(self):
         return self.ns_prefix_
+
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
+
     def get_major(self):
         return self.major
+
     def set_major(self, major):
         self.major = major
+
     def get_minor(self):
         return self.minor
+
     def set_minor(self, minor):
         self.minor = minor
-    def hasContent_(self):
-        if (
-            self.major is not None or
-            self.minor is not None
-        ):
+
+    def has__content(self):
+        if self.major is not None or self.minor is not None:
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ', name_='SpecVersionType', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('SpecVersionType')
+
+    def export(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ',
+        name_="SpecVersionType",
+        pretty_print=True,
+    ):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get("SpecVersionType")
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'SpecVersionType':
+            eol_ = ""
+        if self.original_tagname_ is not None and name_ == "SpecVersionType":
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
-            namespaceprefix_ = self.ns_prefix_ + ':'
+            namespaceprefix_ = self.ns_prefix_ + ":"
         showIndent(outfile, level, pretty_print)
-        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        outfile.write(
+            "<%s%s%s"
+            % (
+                namespaceprefix_,
+                name_,
+                namespacedef_ and " " + namespacedef_ or "",
+            )
+        )
         already_processed = set()
-        self.exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SpecVersionType')
-        if self.hasContent_():
-            outfile.write('>%s' % (eol_, ))
-            self.exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SpecVersionType', pretty_print=pretty_print)
+        self._exportAttributes(
+            outfile,
+            level,
+            already_processed,
+            namespaceprefix_,
+            name_="SpecVersionType",
+        )
+        if self.has__content():
+            outfile.write(">%s" % (eol_,))
+            self._exportChildren(
+                outfile,
+                level + 1,
+                namespaceprefix_,
+                namespacedef_,
+                name_="SpecVersionType",
+                pretty_print=pretty_print,
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+            outfile.write("</%s%s>%s" % (namespaceprefix_, name_, eol_))
         else:
-            outfile.write('/>%s' % (eol_, ))
-    def exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SpecVersionType'):
+            outfile.write("/>%s" % (eol_,))
+
+    def _exportAttributes(
+        self,
+        outfile,
+        level,
+        already_processed,
+        namespaceprefix_="",
+        name_="SpecVersionType",
+    ):
         pass
-    def exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ', name_='SpecVersionType', fromsubclass_=False, pretty_print=True):
+
+    def _exportChildren(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ',
+        name_="SpecVersionType",
+        fromsubclass_=False,
+        pretty_print=True,
+    ):
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
+            eol_ = ""
         if self.major is not None:
-            namespaceprefix_ = self.major_nsprefix_ + ':' if (UseCapturedNS_ and self.major_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.major_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.major_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%smajor>%s</%smajor>%s' % (namespaceprefix_ , self.gds_format_integer(self.major, input_name='major'), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%smajor>%s</%smajor>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_format_integer(self.major, input_name="major"),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.minor is not None:
-            namespaceprefix_ = self.minor_nsprefix_ + ':' if (UseCapturedNS_ and self.minor_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.minor_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.minor_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%sminor>%s</%sminor>%s' % (namespaceprefix_ , self.gds_format_integer(self.minor, input_name='minor'), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%sminor>%s</%sminor>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_format_integer(self.minor, input_name="minor"),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
+
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
-        self.buildAttributes(node, node.attrib, already_processed)
+        self._buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
-            self.buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+            self._buildChildren(
+                child, node, nodeName_, gds_collector_=gds_collector_
+            )
         return self
-    def buildAttributes(self, node, attrs, already_processed):
+
+    def _buildAttributes(self, node, attrs, already_processed):
         pass
-    def buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
-        if nodeName_ == 'major' and child_.text:
+
+    def _buildChildren(
+        self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
+    ):
+        if nodeName_ == "major" and child_.text:
             sval_ = child_.text
-            ival_ = self.gds_parse_integer(sval_, node, 'major')
-            ival_ = self.gds_validate_integer(ival_, node, 'major')
+            ival_ = self.gds_parse_integer(sval_, node, "major")
+            ival_ = self.gds_validate_integer(ival_, node, "major")
             self.major = ival_
             self.major_nsprefix_ = child_.prefix
-        elif nodeName_ == 'minor' and child_.text:
+        elif nodeName_ == "minor" and child_.text:
             sval_ = child_.text
-            ival_ = self.gds_parse_integer(sval_, node, 'minor')
-            ival_ = self.gds_validate_integer(ival_, node, 'minor')
+            ival_ = self.gds_parse_integer(sval_, node, "minor")
+            ival_ = self.gds_validate_integer(ival_, node, "minor")
             self.minor = ival_
             self.minor_nsprefix_ = child_.prefix
+
+
 # end class SpecVersionType
 
 
 class DeviceType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, deviceType=None, friendlyName=None, manufacturer=None, manufacturerURL=None, modelDescription=None, modelName=None, modelNumber=None, modelURL=None, serialNumber=None, UDN=None, macAddress=None, UPC=None, iconList=None, serviceList=None, deviceList=None, presentationURL=None, anytypeobjs_=None, gds_collector_=None, **kwargs_):
+
+    def __init__(
+        self,
+        deviceType=None,
+        friendlyName=None,
+        manufacturer=None,
+        manufacturerURL=None,
+        modelDescription=None,
+        modelName=None,
+        modelNumber=None,
+        modelURL=None,
+        serialNumber=None,
+        UDN=None,
+        macAddress=None,
+        UPC=None,
+        iconList=None,
+        serviceList=None,
+        deviceList=None,
+        presentationURL=None,
+        anytypeobjs_=None,
+        gds_collector_=None,
+        **kwargs_
+    ):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
-        self.parent_object_ = kwargs_.get('parent_object_')
+        self.parent_object_ = kwargs_.get("parent_object_")
         self.ns_prefix_ = None
         self.deviceType = deviceType
         self.deviceType_nsprefix_ = None
         self.friendlyName = friendlyName
         self.friendlyName_nsprefix_ = None
         self.manufacturer = manufacturer
         self.manufacturer_nsprefix_ = None
@@ -1279,1163 +1791,2092 @@
         self.deviceList_nsprefix_ = None
         self.presentationURL = presentationURL
         self.presentationURL_nsprefix_ = None
         if anytypeobjs_ is None:
             self.anytypeobjs_ = []
         else:
             self.anytypeobjs_ = anytypeobjs_
+
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, DeviceType)
+                CurrentSubclassModule_, DeviceType
+            )
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
         if DeviceType.subclass:
             return DeviceType.subclass(*args_, **kwargs_)
         else:
             return DeviceType(*args_, **kwargs_)
+
     factory = staticmethod(factory)
+
     def get_ns_prefix_(self):
         return self.ns_prefix_
+
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
+
     def get_deviceType(self):
         return self.deviceType
+
     def set_deviceType(self, deviceType):
         self.deviceType = deviceType
+
     def get_friendlyName(self):
         return self.friendlyName
+
     def set_friendlyName(self, friendlyName):
         self.friendlyName = friendlyName
+
     def get_manufacturer(self):
         return self.manufacturer
+
     def set_manufacturer(self, manufacturer):
         self.manufacturer = manufacturer
+
     def get_manufacturerURL(self):
         return self.manufacturerURL
+
     def set_manufacturerURL(self, manufacturerURL):
         self.manufacturerURL = manufacturerURL
+
     def get_modelDescription(self):
         return self.modelDescription
+
     def set_modelDescription(self, modelDescription):
         self.modelDescription = modelDescription
+
     def get_modelName(self):
         return self.modelName
+
     def set_modelName(self, modelName):
         self.modelName = modelName
+
     def get_modelNumber(self):
         return self.modelNumber
+
     def set_modelNumber(self, modelNumber):
         self.modelNumber = modelNumber
+
     def get_modelURL(self):
         return self.modelURL
+
     def set_modelURL(self, modelURL):
         self.modelURL = modelURL
+
     def get_serialNumber(self):
         return self.serialNumber
+
     def set_serialNumber(self, serialNumber):
         self.serialNumber = serialNumber
+
     def get_UDN(self):
         return self.UDN
+
     def set_UDN(self, UDN):
         self.UDN = UDN
+
     def get_macAddress(self):
         return self.macAddress
+
     def set_macAddress(self, macAddress):
         self.macAddress = macAddress
+
     def get_UPC(self):
         return self.UPC
+
     def set_UPC(self, UPC):
         self.UPC = UPC
+
     def get_iconList(self):
         return self.iconList
+
     def set_iconList(self, iconList):
         self.iconList = iconList
+
     def get_serviceList(self):
         return self.serviceList
+
     def set_serviceList(self, serviceList):
         self.serviceList = serviceList
+
     def get_deviceList(self):
         return self.deviceList
+
     def set_deviceList(self, deviceList):
         self.deviceList = deviceList
+
     def get_presentationURL(self):
         return self.presentationURL
+
     def set_presentationURL(self, presentationURL):
         self.presentationURL = presentationURL
-    def get_anytypeobjs_(self): return self.anytypeobjs_
-    def set_anytypeobjs_(self, anytypeobjs_): self.anytypeobjs_ = anytypeobjs_
-    def add_anytypeobjs_(self, value): self.anytypeobjs_.append(value)
-    def insert_anytypeobjs_(self, index, value): self._anytypeobjs_[index] = value
-    def hasContent_(self):
+
+    def get_anytypeobjs_(self):
+        return self.anytypeobjs_
+
+    def set_anytypeobjs_(self, anytypeobjs_):
+        self.anytypeobjs_ = anytypeobjs_
+
+    def add_anytypeobjs_(self, value):
+        self.anytypeobjs_.append(value)
+
+    def insert_anytypeobjs_(self, index, value):
+        self._anytypeobjs_[index] = value
+
+    def has__content(self):
         if (
-            self.deviceType is not None or
-            self.friendlyName is not None or
-            self.manufacturer is not None or
-            self.manufacturerURL is not None or
-            self.modelDescription is not None or
-            self.modelName is not None or
-            self.modelNumber is not None or
-            self.modelURL is not None or
-            self.serialNumber is not None or
-            self.UDN is not None or
-            self.macAddress is not None or
-            self.UPC is not None or
-            self.iconList is not None or
-            self.serviceList is not None or
-            self.deviceList is not None or
-            self.presentationURL is not None or
-            self.anytypeobjs_
+            self.deviceType is not None
+            or self.friendlyName is not None
+            or self.manufacturer is not None
+            or self.manufacturerURL is not None
+            or self.modelDescription is not None
+            or self.modelName is not None
+            or self.modelNumber is not None
+            or self.modelURL is not None
+            or self.serialNumber is not None
+            or self.UDN is not None
+            or self.macAddress is not None
+            or self.UPC is not None
+            or self.iconList is not None
+            or self.serviceList is not None
+            or self.deviceList is not None
+            or self.presentationURL is not None
+            or self.anytypeobjs_
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ', name_='DeviceType', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('DeviceType')
+
+    def export(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ',
+        name_="DeviceType",
+        pretty_print=True,
+    ):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get("DeviceType")
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'DeviceType':
+            eol_ = ""
+        if self.original_tagname_ is not None and name_ == "DeviceType":
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
-            namespaceprefix_ = self.ns_prefix_ + ':'
+            namespaceprefix_ = self.ns_prefix_ + ":"
         showIndent(outfile, level, pretty_print)
-        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        outfile.write(
+            "<%s%s%s"
+            % (
+                namespaceprefix_,
+                name_,
+                namespacedef_ and " " + namespacedef_ or "",
+            )
+        )
         already_processed = set()
-        self.exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DeviceType')
-        if self.hasContent_():
-            outfile.write('>%s' % (eol_, ))
-            self.exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DeviceType', pretty_print=pretty_print)
+        self._exportAttributes(
+            outfile,
+            level,
+            already_processed,
+            namespaceprefix_,
+            name_="DeviceType",
+        )
+        if self.has__content():
+            outfile.write(">%s" % (eol_,))
+            self._exportChildren(
+                outfile,
+                level + 1,
+                namespaceprefix_,
+                namespacedef_,
+                name_="DeviceType",
+                pretty_print=pretty_print,
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+            outfile.write("</%s%s>%s" % (namespaceprefix_, name_, eol_))
         else:
-            outfile.write('/>%s' % (eol_, ))
-    def exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DeviceType'):
+            outfile.write("/>%s" % (eol_,))
+
+    def _exportAttributes(
+        self,
+        outfile,
+        level,
+        already_processed,
+        namespaceprefix_="",
+        name_="DeviceType",
+    ):
         pass
-    def exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ', name_='DeviceType', fromsubclass_=False, pretty_print=True):
+
+    def _exportChildren(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ',
+        name_="DeviceType",
+        fromsubclass_=False,
+        pretty_print=True,
+    ):
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
+            eol_ = ""
         if self.deviceType is not None:
-            namespaceprefix_ = self.deviceType_nsprefix_ + ':' if (UseCapturedNS_ and self.deviceType_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.deviceType_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.deviceType_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%sdeviceType>%s</%sdeviceType>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.deviceType), input_name='deviceType')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%sdeviceType>%s</%sdeviceType>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(self.deviceType), input_name="deviceType"
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.friendlyName is not None:
-            namespaceprefix_ = self.friendlyName_nsprefix_ + ':' if (UseCapturedNS_ and self.friendlyName_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.friendlyName_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.friendlyName_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%sfriendlyName>%s</%sfriendlyName>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.friendlyName), input_name='friendlyName')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%sfriendlyName>%s</%sfriendlyName>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(self.friendlyName),
+                            input_name="friendlyName",
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.manufacturer is not None:
-            namespaceprefix_ = self.manufacturer_nsprefix_ + ':' if (UseCapturedNS_ and self.manufacturer_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.manufacturer_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.manufacturer_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%smanufacturer>%s</%smanufacturer>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.manufacturer), input_name='manufacturer')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%smanufacturer>%s</%smanufacturer>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(self.manufacturer),
+                            input_name="manufacturer",
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.manufacturerURL is not None:
-            namespaceprefix_ = self.manufacturerURL_nsprefix_ + ':' if (UseCapturedNS_ and self.manufacturerURL_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.manufacturerURL_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.manufacturerURL_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%smanufacturerURL>%s</%smanufacturerURL>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.manufacturerURL), input_name='manufacturerURL')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%smanufacturerURL>%s</%smanufacturerURL>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(self.manufacturerURL),
+                            input_name="manufacturerURL",
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.modelDescription is not None:
-            namespaceprefix_ = self.modelDescription_nsprefix_ + ':' if (UseCapturedNS_ and self.modelDescription_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.modelDescription_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.modelDescription_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%smodelDescription>%s</%smodelDescription>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.modelDescription), input_name='modelDescription')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%smodelDescription>%s</%smodelDescription>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(self.modelDescription),
+                            input_name="modelDescription",
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.modelName is not None:
-            namespaceprefix_ = self.modelName_nsprefix_ + ':' if (UseCapturedNS_ and self.modelName_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.modelName_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.modelName_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%smodelName>%s</%smodelName>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.modelName), input_name='modelName')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%smodelName>%s</%smodelName>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(self.modelName), input_name="modelName"
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.modelNumber is not None:
-            namespaceprefix_ = self.modelNumber_nsprefix_ + ':' if (UseCapturedNS_ and self.modelNumber_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.modelNumber_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.modelNumber_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%smodelNumber>%s</%smodelNumber>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.modelNumber), input_name='modelNumber')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%smodelNumber>%s</%smodelNumber>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(self.modelNumber),
+                            input_name="modelNumber",
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.modelURL is not None:
-            namespaceprefix_ = self.modelURL_nsprefix_ + ':' if (UseCapturedNS_ and self.modelURL_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.modelURL_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.modelURL_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%smodelURL>%s</%smodelURL>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.modelURL), input_name='modelURL')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%smodelURL>%s</%smodelURL>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(self.modelURL), input_name="modelURL"
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.serialNumber is not None:
-            namespaceprefix_ = self.serialNumber_nsprefix_ + ':' if (UseCapturedNS_ and self.serialNumber_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.serialNumber_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.serialNumber_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%sserialNumber>%s</%sserialNumber>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.serialNumber), input_name='serialNumber')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%sserialNumber>%s</%sserialNumber>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(self.serialNumber),
+                            input_name="serialNumber",
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.UDN is not None:
-            namespaceprefix_ = self.UDN_nsprefix_ + ':' if (UseCapturedNS_ and self.UDN_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.UDN_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.UDN_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%sUDN>%s</%sUDN>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.UDN), input_name='UDN')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%sUDN>%s</%sUDN>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(self.UDN), input_name="UDN"
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.macAddress is not None:
-            namespaceprefix_ = self.macAddress_nsprefix_ + ':' if (UseCapturedNS_ and self.macAddress_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.macAddress_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.macAddress_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%smacAddress>%s</%smacAddress>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.macAddress), input_name='macAddress')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%smacAddress>%s</%smacAddress>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(self.macAddress), input_name="macAddress"
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.UPC is not None:
-            namespaceprefix_ = self.UPC_nsprefix_ + ':' if (UseCapturedNS_ and self.UPC_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.UPC_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.UPC_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%sUPC>%s</%sUPC>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.UPC), input_name='UPC')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%sUPC>%s</%sUPC>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(self.UPC), input_name="UPC"
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.iconList is not None:
-            namespaceprefix_ = self.iconList_nsprefix_ + ':' if (UseCapturedNS_ and self.iconList_nsprefix_) else ''
-            self.iconList.export(outfile, level, namespaceprefix_, namespacedef_='', name_='iconList', pretty_print=pretty_print)
+            namespaceprefix_ = (
+                self.iconList_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.iconList_nsprefix_)
+                else ""
+            )
+            self.iconList.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="iconList",
+                pretty_print=pretty_print,
+            )
         if self.serviceList is not None:
-            namespaceprefix_ = self.serviceList_nsprefix_ + ':' if (UseCapturedNS_ and self.serviceList_nsprefix_) else ''
-            self.serviceList.export(outfile, level, namespaceprefix_, namespacedef_='', name_='serviceList', pretty_print=pretty_print)
+            namespaceprefix_ = (
+                self.serviceList_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.serviceList_nsprefix_)
+                else ""
+            )
+            self.serviceList.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="serviceList",
+                pretty_print=pretty_print,
+            )
         if self.deviceList is not None:
-            namespaceprefix_ = self.deviceList_nsprefix_ + ':' if (UseCapturedNS_ and self.deviceList_nsprefix_) else ''
-            self.deviceList.export(outfile, level, namespaceprefix_, namespacedef_='', name_='deviceList', pretty_print=pretty_print)
+            namespaceprefix_ = (
+                self.deviceList_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.deviceList_nsprefix_)
+                else ""
+            )
+            self.deviceList.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="deviceList",
+                pretty_print=pretty_print,
+            )
         if self.presentationURL is not None:
-            namespaceprefix_ = self.presentationURL_nsprefix_ + ':' if (UseCapturedNS_ and self.presentationURL_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.presentationURL_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.presentationURL_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%spresentationURL>%s</%spresentationURL>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.presentationURL), input_name='presentationURL')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%spresentationURL>%s</%spresentationURL>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(self.presentationURL),
+                            input_name="presentationURL",
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if not fromsubclass_:
             for obj_ in self.anytypeobjs_:
                 showIndent(outfile, level, pretty_print)
-                outfile.write(obj_)
-                outfile.write('\n')
+                outfile.write(str(obj_))
+                outfile.write("\n")
+
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
-        self.buildAttributes(node, node.attrib, already_processed)
+        self._buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
-            self.buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+            self._buildChildren(
+                child, node, nodeName_, gds_collector_=gds_collector_
+            )
         return self
-    def buildAttributes(self, node, attrs, already_processed):
+
+    def _buildAttributes(self, node, attrs, already_processed):
         pass
-    def buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
-        if nodeName_ == 'deviceType':
+
+    def _buildChildren(
+        self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
+    ):
+        if nodeName_ == "deviceType":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'deviceType')
-            value_ = self.gds_validate_string(value_, node, 'deviceType')
+            value_ = self.gds_parse_string(value_, node, "deviceType")
+            value_ = self.gds_validate_string(value_, node, "deviceType")
             self.deviceType = value_
             self.deviceType_nsprefix_ = child_.prefix
-        elif nodeName_ == 'friendlyName':
+        elif nodeName_ == "friendlyName":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'friendlyName')
-            value_ = self.gds_validate_string(value_, node, 'friendlyName')
+            value_ = self.gds_parse_string(value_, node, "friendlyName")
+            value_ = self.gds_validate_string(value_, node, "friendlyName")
             self.friendlyName = value_
             self.friendlyName_nsprefix_ = child_.prefix
-        elif nodeName_ == 'manufacturer':
+        elif nodeName_ == "manufacturer":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'manufacturer')
-            value_ = self.gds_validate_string(value_, node, 'manufacturer')
+            value_ = self.gds_parse_string(value_, node, "manufacturer")
+            value_ = self.gds_validate_string(value_, node, "manufacturer")
             self.manufacturer = value_
             self.manufacturer_nsprefix_ = child_.prefix
-        elif nodeName_ == 'manufacturerURL':
+        elif nodeName_ == "manufacturerURL":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'manufacturerURL')
-            value_ = self.gds_validate_string(value_, node, 'manufacturerURL')
+            value_ = self.gds_parse_string(value_, node, "manufacturerURL")
+            value_ = self.gds_validate_string(value_, node, "manufacturerURL")
             self.manufacturerURL = value_
             self.manufacturerURL_nsprefix_ = child_.prefix
-        elif nodeName_ == 'modelDescription':
+        elif nodeName_ == "modelDescription":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'modelDescription')
-            value_ = self.gds_validate_string(value_, node, 'modelDescription')
+            value_ = self.gds_parse_string(value_, node, "modelDescription")
+            value_ = self.gds_validate_string(value_, node, "modelDescription")
             self.modelDescription = value_
             self.modelDescription_nsprefix_ = child_.prefix
-        elif nodeName_ == 'modelName':
+        elif nodeName_ == "modelName":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'modelName')
-            value_ = self.gds_validate_string(value_, node, 'modelName')
+            value_ = self.gds_parse_string(value_, node, "modelName")
+            value_ = self.gds_validate_string(value_, node, "modelName")
             self.modelName = value_
             self.modelName_nsprefix_ = child_.prefix
-        elif nodeName_ == 'modelNumber':
+        elif nodeName_ == "modelNumber":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'modelNumber')
-            value_ = self.gds_validate_string(value_, node, 'modelNumber')
+            value_ = self.gds_parse_string(value_, node, "modelNumber")
+            value_ = self.gds_validate_string(value_, node, "modelNumber")
             self.modelNumber = value_
             self.modelNumber_nsprefix_ = child_.prefix
-        elif nodeName_ == 'modelURL':
+        elif nodeName_ == "modelURL":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'modelURL')
-            value_ = self.gds_validate_string(value_, node, 'modelURL')
+            value_ = self.gds_parse_string(value_, node, "modelURL")
+            value_ = self.gds_validate_string(value_, node, "modelURL")
             self.modelURL = value_
             self.modelURL_nsprefix_ = child_.prefix
-        elif nodeName_ == 'serialNumber':
+        elif nodeName_ == "serialNumber":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'serialNumber')
-            value_ = self.gds_validate_string(value_, node, 'serialNumber')
+            value_ = self.gds_parse_string(value_, node, "serialNumber")
+            value_ = self.gds_validate_string(value_, node, "serialNumber")
             self.serialNumber = value_
             self.serialNumber_nsprefix_ = child_.prefix
-        elif nodeName_ == 'UDN':
+        elif nodeName_ == "UDN":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'UDN')
-            value_ = self.gds_validate_string(value_, node, 'UDN')
+            value_ = self.gds_parse_string(value_, node, "UDN")
+            value_ = self.gds_validate_string(value_, node, "UDN")
             self.UDN = value_
             self.UDN_nsprefix_ = child_.prefix
-        elif nodeName_ == 'macAddress':
+        elif nodeName_ == "macAddress":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'macAddress')
-            value_ = self.gds_validate_string(value_, node, 'macAddress')
+            value_ = self.gds_parse_string(value_, node, "macAddress")
+            value_ = self.gds_validate_string(value_, node, "macAddress")
             self.macAddress = value_
             self.macAddress_nsprefix_ = child_.prefix
-        elif nodeName_ == 'UPC':
+        elif nodeName_ == "UPC":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'UPC')
-            value_ = self.gds_validate_string(value_, node, 'UPC')
+            value_ = self.gds_parse_string(value_, node, "UPC")
+            value_ = self.gds_validate_string(value_, node, "UPC")
             self.UPC = value_
             self.UPC_nsprefix_ = child_.prefix
-        elif nodeName_ == 'iconList':
+        elif nodeName_ == "iconList":
             obj_ = IconListType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.iconList = obj_
-            obj_.original_tagname_ = 'iconList'
-        elif nodeName_ == 'serviceList':
+            obj_.original_tagname_ = "iconList"
+        elif nodeName_ == "serviceList":
             obj_ = ServiceListType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.serviceList = obj_
-            obj_.original_tagname_ = 'serviceList'
-        elif nodeName_ == 'deviceList':
+            obj_.original_tagname_ = "serviceList"
+        elif nodeName_ == "deviceList":
             obj_ = DeviceListType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.deviceList = obj_
-            obj_.original_tagname_ = 'deviceList'
-        elif nodeName_ == 'presentationURL':
+            obj_.original_tagname_ = "deviceList"
+        elif nodeName_ == "presentationURL":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'presentationURL')
-            value_ = self.gds_validate_string(value_, node, 'presentationURL')
+            value_ = self.gds_parse_string(value_, node, "presentationURL")
+            value_ = self.gds_validate_string(value_, node, "presentationURL")
             self.presentationURL = value_
             self.presentationURL_nsprefix_ = child_.prefix
         else:
-            content_ = self.gds_build_any(child_, 'DeviceType')
-            self.add_anytypeobjs_(content_)
+            content_ = self.gds_build_any(child_, "DeviceType")
+            self.anytypeobjs_.append(content_)
+
+
 # end class DeviceType
 
 
 class IconListType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
+
     def __init__(self, icon=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
-        self.parent_object_ = kwargs_.get('parent_object_')
+        self.parent_object_ = kwargs_.get("parent_object_")
         self.ns_prefix_ = None
         if icon is None:
             self.icon = []
         else:
             self.icon = icon
         self.icon_nsprefix_ = None
+
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, IconListType)
+                CurrentSubclassModule_, IconListType
+            )
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
         if IconListType.subclass:
             return IconListType.subclass(*args_, **kwargs_)
         else:
             return IconListType(*args_, **kwargs_)
+
     factory = staticmethod(factory)
+
     def get_ns_prefix_(self):
         return self.ns_prefix_
+
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
+
     def get_icon(self):
         return self.icon
+
     def set_icon(self, icon):
         self.icon = icon
+
     def add_icon(self, value):
         self.icon.append(value)
+
     def insert_icon_at(self, index, value):
         self.icon.insert(index, value)
+
     def replace_icon_at(self, index, value):
         self.icon[index] = value
-    def hasContent_(self):
-        if (
-            self.icon
-        ):
+
+    def has__content(self):
+        if self.icon:
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ', name_='IconListType', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('IconListType')
+
+    def export(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ',
+        name_="IconListType",
+        pretty_print=True,
+    ):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get("IconListType")
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'IconListType':
+            eol_ = ""
+        if self.original_tagname_ is not None and name_ == "IconListType":
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
-            namespaceprefix_ = self.ns_prefix_ + ':'
+            namespaceprefix_ = self.ns_prefix_ + ":"
         showIndent(outfile, level, pretty_print)
-        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        outfile.write(
+            "<%s%s%s"
+            % (
+                namespaceprefix_,
+                name_,
+                namespacedef_ and " " + namespacedef_ or "",
+            )
+        )
         already_processed = set()
-        self.exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IconListType')
-        if self.hasContent_():
-            outfile.write('>%s' % (eol_, ))
-            self.exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IconListType', pretty_print=pretty_print)
+        self._exportAttributes(
+            outfile,
+            level,
+            already_processed,
+            namespaceprefix_,
+            name_="IconListType",
+        )
+        if self.has__content():
+            outfile.write(">%s" % (eol_,))
+            self._exportChildren(
+                outfile,
+                level + 1,
+                namespaceprefix_,
+                namespacedef_,
+                name_="IconListType",
+                pretty_print=pretty_print,
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+            outfile.write("</%s%s>%s" % (namespaceprefix_, name_, eol_))
         else:
-            outfile.write('/>%s' % (eol_, ))
-    def exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IconListType'):
+            outfile.write("/>%s" % (eol_,))
+
+    def _exportAttributes(
+        self,
+        outfile,
+        level,
+        already_processed,
+        namespaceprefix_="",
+        name_="IconListType",
+    ):
         pass
-    def exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ', name_='IconListType', fromsubclass_=False, pretty_print=True):
+
+    def _exportChildren(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ',
+        name_="IconListType",
+        fromsubclass_=False,
+        pretty_print=True,
+    ):
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
+            eol_ = ""
         for icon_ in self.icon:
-            namespaceprefix_ = self.icon_nsprefix_ + ':' if (UseCapturedNS_ and self.icon_nsprefix_) else ''
-            icon_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='icon', pretty_print=pretty_print)
+            namespaceprefix_ = (
+                self.icon_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.icon_nsprefix_)
+                else ""
+            )
+            icon_.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="icon",
+                pretty_print=pretty_print,
+            )
+
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
-        self.buildAttributes(node, node.attrib, already_processed)
+        self._buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
-            self.buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+            self._buildChildren(
+                child, node, nodeName_, gds_collector_=gds_collector_
+            )
         return self
-    def buildAttributes(self, node, attrs, already_processed):
+
+    def _buildAttributes(self, node, attrs, already_processed):
         pass
-    def buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
-        if nodeName_ == 'icon':
+
+    def _buildChildren(
+        self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
+    ):
+        if nodeName_ == "icon":
             obj_ = iconType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.icon.append(obj_)
-            obj_.original_tagname_ = 'icon'
+            obj_.original_tagname_ = "icon"
+
+
 # end class IconListType
 
 
 class ServiceListType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
+
     def __init__(self, service=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
-        self.parent_object_ = kwargs_.get('parent_object_')
+        self.parent_object_ = kwargs_.get("parent_object_")
         self.ns_prefix_ = None
         if service is None:
             self.service = []
         else:
             self.service = service
         self.service_nsprefix_ = None
+
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, ServiceListType)
+                CurrentSubclassModule_, ServiceListType
+            )
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
         if ServiceListType.subclass:
             return ServiceListType.subclass(*args_, **kwargs_)
         else:
             return ServiceListType(*args_, **kwargs_)
+
     factory = staticmethod(factory)
+
     def get_ns_prefix_(self):
         return self.ns_prefix_
+
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
+
     def get_service(self):
         return self.service
+
     def set_service(self, service):
         self.service = service
+
     def add_service(self, value):
         self.service.append(value)
+
     def insert_service_at(self, index, value):
         self.service.insert(index, value)
+
     def replace_service_at(self, index, value):
         self.service[index] = value
-    def hasContent_(self):
-        if (
-            self.service
-        ):
+
+    def has__content(self):
+        if self.service:
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ', name_='ServiceListType', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('ServiceListType')
+
+    def export(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ',
+        name_="ServiceListType",
+        pretty_print=True,
+    ):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get("ServiceListType")
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'ServiceListType':
+            eol_ = ""
+        if self.original_tagname_ is not None and name_ == "ServiceListType":
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
-            namespaceprefix_ = self.ns_prefix_ + ':'
+            namespaceprefix_ = self.ns_prefix_ + ":"
         showIndent(outfile, level, pretty_print)
-        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        outfile.write(
+            "<%s%s%s"
+            % (
+                namespaceprefix_,
+                name_,
+                namespacedef_ and " " + namespacedef_ or "",
+            )
+        )
         already_processed = set()
-        self.exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ServiceListType')
-        if self.hasContent_():
-            outfile.write('>%s' % (eol_, ))
-            self.exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ServiceListType', pretty_print=pretty_print)
+        self._exportAttributes(
+            outfile,
+            level,
+            already_processed,
+            namespaceprefix_,
+            name_="ServiceListType",
+        )
+        if self.has__content():
+            outfile.write(">%s" % (eol_,))
+            self._exportChildren(
+                outfile,
+                level + 1,
+                namespaceprefix_,
+                namespacedef_,
+                name_="ServiceListType",
+                pretty_print=pretty_print,
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+            outfile.write("</%s%s>%s" % (namespaceprefix_, name_, eol_))
         else:
-            outfile.write('/>%s' % (eol_, ))
-    def exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ServiceListType'):
+            outfile.write("/>%s" % (eol_,))
+
+    def _exportAttributes(
+        self,
+        outfile,
+        level,
+        already_processed,
+        namespaceprefix_="",
+        name_="ServiceListType",
+    ):
         pass
-    def exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ', name_='ServiceListType', fromsubclass_=False, pretty_print=True):
+
+    def _exportChildren(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ',
+        name_="ServiceListType",
+        fromsubclass_=False,
+        pretty_print=True,
+    ):
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
+            eol_ = ""
         for service_ in self.service:
-            namespaceprefix_ = self.service_nsprefix_ + ':' if (UseCapturedNS_ and self.service_nsprefix_) else ''
-            service_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='service', pretty_print=pretty_print)
+            namespaceprefix_ = (
+                self.service_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.service_nsprefix_)
+                else ""
+            )
+            service_.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="service",
+                pretty_print=pretty_print,
+            )
+
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
-        self.buildAttributes(node, node.attrib, already_processed)
+        self._buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
-            self.buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+            self._buildChildren(
+                child, node, nodeName_, gds_collector_=gds_collector_
+            )
         return self
-    def buildAttributes(self, node, attrs, already_processed):
+
+    def _buildAttributes(self, node, attrs, already_processed):
         pass
-    def buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
-        if nodeName_ == 'service':
+
+    def _buildChildren(
+        self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
+    ):
+        if nodeName_ == "service":
             obj_ = serviceType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.service.append(obj_)
-            obj_.original_tagname_ = 'service'
+            obj_.original_tagname_ = "service"
+
+
 # end class ServiceListType
 
 
 class DeviceListType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
+
     def __init__(self, device=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
-        self.parent_object_ = kwargs_.get('parent_object_')
+        self.parent_object_ = kwargs_.get("parent_object_")
         self.ns_prefix_ = None
         if device is None:
             self.device = []
         else:
             self.device = device
         self.device_nsprefix_ = None
+
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, DeviceListType)
+                CurrentSubclassModule_, DeviceListType
+            )
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
         if DeviceListType.subclass:
             return DeviceListType.subclass(*args_, **kwargs_)
         else:
             return DeviceListType(*args_, **kwargs_)
+
     factory = staticmethod(factory)
+
     def get_ns_prefix_(self):
         return self.ns_prefix_
+
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
+
     def get_device(self):
         return self.device
+
     def set_device(self, device):
         self.device = device
+
     def add_device(self, value):
         self.device.append(value)
+
     def insert_device_at(self, index, value):
         self.device.insert(index, value)
+
     def replace_device_at(self, index, value):
         self.device[index] = value
-    def hasContent_(self):
-        if (
-            self.device
-        ):
+
+    def has__content(self):
+        if self.device:
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ', name_='DeviceListType', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('DeviceListType')
+
+    def export(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ',
+        name_="DeviceListType",
+        pretty_print=True,
+    ):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get("DeviceListType")
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'DeviceListType':
+            eol_ = ""
+        if self.original_tagname_ is not None and name_ == "DeviceListType":
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
-            namespaceprefix_ = self.ns_prefix_ + ':'
+            namespaceprefix_ = self.ns_prefix_ + ":"
         showIndent(outfile, level, pretty_print)
-        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        outfile.write(
+            "<%s%s%s"
+            % (
+                namespaceprefix_,
+                name_,
+                namespacedef_ and " " + namespacedef_ or "",
+            )
+        )
         already_processed = set()
-        self.exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DeviceListType')
-        if self.hasContent_():
-            outfile.write('>%s' % (eol_, ))
-            self.exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DeviceListType', pretty_print=pretty_print)
+        self._exportAttributes(
+            outfile,
+            level,
+            already_processed,
+            namespaceprefix_,
+            name_="DeviceListType",
+        )
+        if self.has__content():
+            outfile.write(">%s" % (eol_,))
+            self._exportChildren(
+                outfile,
+                level + 1,
+                namespaceprefix_,
+                namespacedef_,
+                name_="DeviceListType",
+                pretty_print=pretty_print,
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+            outfile.write("</%s%s>%s" % (namespaceprefix_, name_, eol_))
         else:
-            outfile.write('/>%s' % (eol_, ))
-    def exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DeviceListType'):
+            outfile.write("/>%s" % (eol_,))
+
+    def _exportAttributes(
+        self,
+        outfile,
+        level,
+        already_processed,
+        namespaceprefix_="",
+        name_="DeviceListType",
+    ):
         pass
-    def exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ', name_='DeviceListType', fromsubclass_=False, pretty_print=True):
+
+    def _exportChildren(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ',
+        name_="DeviceListType",
+        fromsubclass_=False,
+        pretty_print=True,
+    ):
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
+            eol_ = ""
         for device_ in self.device:
-            namespaceprefix_ = self.device_nsprefix_ + ':' if (UseCapturedNS_ and self.device_nsprefix_) else ''
-            device_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='device', pretty_print=pretty_print)
+            namespaceprefix_ = (
+                self.device_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.device_nsprefix_)
+                else ""
+            )
+            device_.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="device",
+                pretty_print=pretty_print,
+            )
+
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
-        self.buildAttributes(node, node.attrib, already_processed)
+        self._buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
-            self.buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+            self._buildChildren(
+                child, node, nodeName_, gds_collector_=gds_collector_
+            )
         return self
-    def buildAttributes(self, node, attrs, already_processed):
+
+    def _buildAttributes(self, node, attrs, already_processed):
         pass
-    def buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
-        if nodeName_ == 'device':
+
+    def _buildChildren(
+        self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
+    ):
+        if nodeName_ == "device":
             obj_ = DeviceType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.device.append(obj_)
-            obj_.original_tagname_ = 'device'
+            obj_.original_tagname_ = "device"
+
+
 # end class DeviceListType
 
 
 class iconType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, mimetype=None, width=None, height=None, depth=None, url=None, gds_collector_=None, **kwargs_):
+
+    def __init__(
+        self,
+        mimetype=None,
+        width=None,
+        height=None,
+        depth=None,
+        url=None,
+        gds_collector_=None,
+        **kwargs_
+    ):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
-        self.parent_object_ = kwargs_.get('parent_object_')
+        self.parent_object_ = kwargs_.get("parent_object_")
         self.ns_prefix_ = None
         self.mimetype = mimetype
         self.mimetype_nsprefix_ = None
         self.width = width
         self.width_nsprefix_ = None
         self.height = height
         self.height_nsprefix_ = None
         self.depth = depth
         self.depth_nsprefix_ = None
         self.url = url
         self.url_nsprefix_ = None
+
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
-            subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, iconType)
+            subclass = getSubclassFromModule_(CurrentSubclassModule_, iconType)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
         if iconType.subclass:
             return iconType.subclass(*args_, **kwargs_)
         else:
             return iconType(*args_, **kwargs_)
+
     factory = staticmethod(factory)
+
     def get_ns_prefix_(self):
         return self.ns_prefix_
+
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
+
     def get_mimetype(self):
         return self.mimetype
+
     def set_mimetype(self, mimetype):
         self.mimetype = mimetype
+
     def get_width(self):
         return self.width
+
     def set_width(self, width):
         self.width = width
+
     def get_height(self):
         return self.height
+
     def set_height(self, height):
         self.height = height
+
     def get_depth(self):
         return self.depth
+
     def set_depth(self, depth):
         self.depth = depth
+
     def get_url(self):
         return self.url
+
     def set_url(self, url):
         self.url = url
-    def hasContent_(self):
+
+    def has__content(self):
         if (
-            self.mimetype is not None or
-            self.width is not None or
-            self.height is not None or
-            self.depth is not None or
-            self.url is not None
+            self.mimetype is not None
+            or self.width is not None
+            or self.height is not None
+            or self.depth is not None
+            or self.url is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ', name_='iconType', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('iconType')
+
+    def export(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ',
+        name_="iconType",
+        pretty_print=True,
+    ):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get("iconType")
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'iconType':
+            eol_ = ""
+        if self.original_tagname_ is not None and name_ == "iconType":
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
-            namespaceprefix_ = self.ns_prefix_ + ':'
+            namespaceprefix_ = self.ns_prefix_ + ":"
         showIndent(outfile, level, pretty_print)
-        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        outfile.write(
+            "<%s%s%s"
+            % (
+                namespaceprefix_,
+                name_,
+                namespacedef_ and " " + namespacedef_ or "",
+            )
+        )
         already_processed = set()
-        self.exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='iconType')
-        if self.hasContent_():
-            outfile.write('>%s' % (eol_, ))
-            self.exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='iconType', pretty_print=pretty_print)
+        self._exportAttributes(
+            outfile,
+            level,
+            already_processed,
+            namespaceprefix_,
+            name_="iconType",
+        )
+        if self.has__content():
+            outfile.write(">%s" % (eol_,))
+            self._exportChildren(
+                outfile,
+                level + 1,
+                namespaceprefix_,
+                namespacedef_,
+                name_="iconType",
+                pretty_print=pretty_print,
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+            outfile.write("</%s%s>%s" % (namespaceprefix_, name_, eol_))
         else:
-            outfile.write('/>%s' % (eol_, ))
-    def exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='iconType'):
+            outfile.write("/>%s" % (eol_,))
+
+    def _exportAttributes(
+        self,
+        outfile,
+        level,
+        already_processed,
+        namespaceprefix_="",
+        name_="iconType",
+    ):
         pass
-    def exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ', name_='iconType', fromsubclass_=False, pretty_print=True):
+
+    def _exportChildren(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ',
+        name_="iconType",
+        fromsubclass_=False,
+        pretty_print=True,
+    ):
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
+            eol_ = ""
         if self.mimetype is not None:
-            namespaceprefix_ = self.mimetype_nsprefix_ + ':' if (UseCapturedNS_ and self.mimetype_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.mimetype_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.mimetype_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%smimetype>%s</%smimetype>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.mimetype), input_name='mimetype')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%smimetype>%s</%smimetype>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(self.mimetype), input_name="mimetype"
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.width is not None:
-            namespaceprefix_ = self.width_nsprefix_ + ':' if (UseCapturedNS_ and self.width_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.width_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.width_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%swidth>%s</%swidth>%s' % (namespaceprefix_ , self.gds_format_integer(self.width, input_name='width'), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%swidth>%s</%swidth>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_format_integer(self.width, input_name="width"),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.height is not None:
-            namespaceprefix_ = self.height_nsprefix_ + ':' if (UseCapturedNS_ and self.height_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.height_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.height_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%sheight>%s</%sheight>%s' % (namespaceprefix_ , self.gds_format_integer(self.height, input_name='height'), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%sheight>%s</%sheight>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_format_integer(self.height, input_name="height"),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.depth is not None:
-            namespaceprefix_ = self.depth_nsprefix_ + ':' if (UseCapturedNS_ and self.depth_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.depth_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.depth_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%sdepth>%s</%sdepth>%s' % (namespaceprefix_ , self.gds_format_integer(self.depth, input_name='depth'), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%sdepth>%s</%sdepth>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_format_integer(self.depth, input_name="depth"),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.url is not None:
-            namespaceprefix_ = self.url_nsprefix_ + ':' if (UseCapturedNS_ and self.url_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.url_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.url_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%surl>%s</%surl>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.url), input_name='url')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%surl>%s</%surl>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(self.url), input_name="url"
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
+
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
-        self.buildAttributes(node, node.attrib, already_processed)
+        self._buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
-            self.buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+            self._buildChildren(
+                child, node, nodeName_, gds_collector_=gds_collector_
+            )
         return self
-    def buildAttributes(self, node, attrs, already_processed):
+
+    def _buildAttributes(self, node, attrs, already_processed):
         pass
-    def buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
-        if nodeName_ == 'mimetype':
+
+    def _buildChildren(
+        self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
+    ):
+        if nodeName_ == "mimetype":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'mimetype')
-            value_ = self.gds_validate_string(value_, node, 'mimetype')
+            value_ = self.gds_parse_string(value_, node, "mimetype")
+            value_ = self.gds_validate_string(value_, node, "mimetype")
             self.mimetype = value_
             self.mimetype_nsprefix_ = child_.prefix
-        elif nodeName_ == 'width' and child_.text:
+        elif nodeName_ == "width" and child_.text:
             sval_ = child_.text
-            ival_ = self.gds_parse_integer(sval_, node, 'width')
-            ival_ = self.gds_validate_integer(ival_, node, 'width')
+            ival_ = self.gds_parse_integer(sval_, node, "width")
+            ival_ = self.gds_validate_integer(ival_, node, "width")
             self.width = ival_
             self.width_nsprefix_ = child_.prefix
-        elif nodeName_ == 'height' and child_.text:
+        elif nodeName_ == "height" and child_.text:
             sval_ = child_.text
-            ival_ = self.gds_parse_integer(sval_, node, 'height')
-            ival_ = self.gds_validate_integer(ival_, node, 'height')
+            ival_ = self.gds_parse_integer(sval_, node, "height")
+            ival_ = self.gds_validate_integer(ival_, node, "height")
             self.height = ival_
             self.height_nsprefix_ = child_.prefix
-        elif nodeName_ == 'depth' and child_.text:
+        elif nodeName_ == "depth" and child_.text:
             sval_ = child_.text
-            ival_ = self.gds_parse_integer(sval_, node, 'depth')
-            ival_ = self.gds_validate_integer(ival_, node, 'depth')
+            ival_ = self.gds_parse_integer(sval_, node, "depth")
+            ival_ = self.gds_validate_integer(ival_, node, "depth")
             self.depth = ival_
             self.depth_nsprefix_ = child_.prefix
-        elif nodeName_ == 'url':
+        elif nodeName_ == "url":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'url')
-            value_ = self.gds_validate_string(value_, node, 'url')
+            value_ = self.gds_parse_string(value_, node, "url")
+            value_ = self.gds_validate_string(value_, node, "url")
             self.url = value_
             self.url_nsprefix_ = child_.prefix
+
+
 # end class iconType
 
 
 class serviceType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, serviceType_member=None, serviceId=None, SCPDURL=None, controlURL=None, eventSubURL=None, gds_collector_=None, **kwargs_):
+
+    def __init__(
+        self,
+        serviceType_member=None,
+        serviceId=None,
+        SCPDURL=None,
+        controlURL=None,
+        eventSubURL=None,
+        gds_collector_=None,
+        **kwargs_
+    ):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
-        self.parent_object_ = kwargs_.get('parent_object_')
+        self.parent_object_ = kwargs_.get("parent_object_")
         self.ns_prefix_ = None
         self.serviceType = serviceType_member
         self.serviceType_nsprefix_ = None
         self.serviceId = serviceId
         self.serviceId_nsprefix_ = None
         self.SCPDURL = SCPDURL
         self.SCPDURL_nsprefix_ = None
         self.controlURL = controlURL
         self.controlURL_nsprefix_ = None
         self.eventSubURL = eventSubURL
         self.eventSubURL_nsprefix_ = None
+
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, serviceType)
+                CurrentSubclassModule_, serviceType
+            )
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
         if serviceType.subclass:
             return serviceType.subclass(*args_, **kwargs_)
         else:
             return serviceType(*args_, **kwargs_)
+
     factory = staticmethod(factory)
+
     def get_ns_prefix_(self):
         return self.ns_prefix_
+
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
+
     def get_serviceType(self):
         return self.serviceType
+
     def set_serviceType(self, serviceType):
         self.serviceType = serviceType
+
     def get_serviceId(self):
         return self.serviceId
+
     def set_serviceId(self, serviceId):
         self.serviceId = serviceId
+
     def get_SCPDURL(self):
         return self.SCPDURL
+
     def set_SCPDURL(self, SCPDURL):
         self.SCPDURL = SCPDURL
+
     def get_controlURL(self):
         return self.controlURL
+
     def set_controlURL(self, controlURL):
         self.controlURL = controlURL
+
     def get_eventSubURL(self):
         return self.eventSubURL
+
     def set_eventSubURL(self, eventSubURL):
         self.eventSubURL = eventSubURL
-    def hasContent_(self):
+
+    def has__content(self):
         if (
-            self.serviceType is not None or
-            self.serviceId is not None or
-            self.SCPDURL is not None or
-            self.controlURL is not None or
-            self.eventSubURL is not None
+            self.serviceType is not None
+            or self.serviceId is not None
+            or self.SCPDURL is not None
+            or self.controlURL is not None
+            or self.eventSubURL is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ', name_='serviceType', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('serviceType')
+
+    def export(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ',
+        name_="serviceType",
+        pretty_print=True,
+    ):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get("serviceType")
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'serviceType':
+            eol_ = ""
+        if self.original_tagname_ is not None and name_ == "serviceType":
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
-            namespaceprefix_ = self.ns_prefix_ + ':'
+            namespaceprefix_ = self.ns_prefix_ + ":"
         showIndent(outfile, level, pretty_print)
-        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        outfile.write(
+            "<%s%s%s"
+            % (
+                namespaceprefix_,
+                name_,
+                namespacedef_ and " " + namespacedef_ or "",
+            )
+        )
         already_processed = set()
-        self.exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='serviceType')
-        if self.hasContent_():
-            outfile.write('>%s' % (eol_, ))
-            self.exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='serviceType', pretty_print=pretty_print)
+        self._exportAttributes(
+            outfile,
+            level,
+            already_processed,
+            namespaceprefix_,
+            name_="serviceType",
+        )
+        if self.has__content():
+            outfile.write(">%s" % (eol_,))
+            self._exportChildren(
+                outfile,
+                level + 1,
+                namespaceprefix_,
+                namespacedef_,
+                name_="serviceType",
+                pretty_print=pretty_print,
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+            outfile.write("</%s%s>%s" % (namespaceprefix_, name_, eol_))
         else:
-            outfile.write('/>%s' % (eol_, ))
-    def exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='serviceType'):
+            outfile.write("/>%s" % (eol_,))
+
+    def _exportAttributes(
+        self,
+        outfile,
+        level,
+        already_processed,
+        namespaceprefix_="",
+        name_="serviceType",
+    ):
         pass
-    def exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ', name_='serviceType', fromsubclass_=False, pretty_print=True):
+
+    def _exportChildren(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0" xmlns:None="urn:schemas-upnp-org:device-1-0" ',
+        name_="serviceType",
+        fromsubclass_=False,
+        pretty_print=True,
+    ):
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
+            eol_ = ""
         if self.serviceType is not None:
-            namespaceprefix_ = self.serviceType_nsprefix_ + ':' if (UseCapturedNS_ and self.serviceType_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.serviceType_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.serviceType_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%sserviceType>%s</%sserviceType>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.serviceType), input_name='serviceType')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%sserviceType>%s</%sserviceType>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(self.serviceType),
+                            input_name="serviceType",
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.serviceId is not None:
-            namespaceprefix_ = self.serviceId_nsprefix_ + ':' if (UseCapturedNS_ and self.serviceId_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.serviceId_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.serviceId_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%sserviceId>%s</%sserviceId>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.serviceId), input_name='serviceId')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%sserviceId>%s</%sserviceId>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(self.serviceId), input_name="serviceId"
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.SCPDURL is not None:
-            namespaceprefix_ = self.SCPDURL_nsprefix_ + ':' if (UseCapturedNS_ and self.SCPDURL_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.SCPDURL_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.SCPDURL_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%sSCPDURL>%s</%sSCPDURL>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.SCPDURL), input_name='SCPDURL')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%sSCPDURL>%s</%sSCPDURL>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(self.SCPDURL), input_name="SCPDURL"
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.controlURL is not None:
-            namespaceprefix_ = self.controlURL_nsprefix_ + ':' if (UseCapturedNS_ and self.controlURL_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.controlURL_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.controlURL_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%scontrolURL>%s</%scontrolURL>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.controlURL), input_name='controlURL')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%scontrolURL>%s</%scontrolURL>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(self.controlURL), input_name="controlURL"
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.eventSubURL is not None:
-            namespaceprefix_ = self.eventSubURL_nsprefix_ + ':' if (UseCapturedNS_ and self.eventSubURL_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.eventSubURL_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.eventSubURL_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%seventSubURL>%s</%seventSubURL>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.eventSubURL), input_name='eventSubURL')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%seventSubURL>%s</%seventSubURL>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(self.eventSubURL),
+                            input_name="eventSubURL",
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
+
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
-        self.buildAttributes(node, node.attrib, already_processed)
+        self._buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
-            self.buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+            self._buildChildren(
+                child, node, nodeName_, gds_collector_=gds_collector_
+            )
         return self
-    def buildAttributes(self, node, attrs, already_processed):
+
+    def _buildAttributes(self, node, attrs, already_processed):
         pass
-    def buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
-        if nodeName_ == 'serviceType':
+
+    def _buildChildren(
+        self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
+    ):
+        if nodeName_ == "serviceType":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'serviceType')
-            value_ = self.gds_validate_string(value_, node, 'serviceType')
+            value_ = self.gds_parse_string(value_, node, "serviceType")
+            value_ = self.gds_validate_string(value_, node, "serviceType")
             self.serviceType = value_
             self.serviceType_nsprefix_ = child_.prefix
-        elif nodeName_ == 'serviceId':
+        elif nodeName_ == "serviceId":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'serviceId')
-            value_ = self.gds_validate_string(value_, node, 'serviceId')
+            value_ = self.gds_parse_string(value_, node, "serviceId")
+            value_ = self.gds_validate_string(value_, node, "serviceId")
             self.serviceId = value_
             self.serviceId_nsprefix_ = child_.prefix
-        elif nodeName_ == 'SCPDURL':
+        elif nodeName_ == "SCPDURL":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'SCPDURL')
-            value_ = self.gds_validate_string(value_, node, 'SCPDURL')
+            value_ = self.gds_parse_string(value_, node, "SCPDURL")
+            value_ = self.gds_validate_string(value_, node, "SCPDURL")
             self.SCPDURL = value_
             self.SCPDURL_nsprefix_ = child_.prefix
-        elif nodeName_ == 'controlURL':
+        elif nodeName_ == "controlURL":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'controlURL')
-            value_ = self.gds_validate_string(value_, node, 'controlURL')
+            value_ = self.gds_parse_string(value_, node, "controlURL")
+            value_ = self.gds_validate_string(value_, node, "controlURL")
             self.controlURL = value_
             self.controlURL_nsprefix_ = child_.prefix
-        elif nodeName_ == 'eventSubURL':
+        elif nodeName_ == "eventSubURL":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'eventSubURL')
-            value_ = self.gds_validate_string(value_, node, 'eventSubURL')
+            value_ = self.gds_parse_string(value_, node, "eventSubURL")
+            value_ = self.gds_validate_string(value_, node, "eventSubURL")
             self.eventSubURL = value_
             self.eventSubURL_nsprefix_ = child_.prefix
+
+
 # end class serviceType
 
 
-GDSClassesMapping = {
-}
+GDSClassesMapping = {}
 
 
 USAGE_TEXT = """
 Usage: python <Parser>.py [ -s ] <in_xml_file>
 """
 
 
 def usage():
     print(USAGE_TEXT)
     sys.exit(1)
 
 
 def get_root_tag(node):
     tag = Tag_pattern_.match(node.tag).groups()[-1]
-    rootClass = GDSClassesMapping.get(tag)
+    prefix_tag = TagNamePrefix + tag
+    rootClass = GDSClassesMapping.get(prefix_tag)
     if rootClass is None:
-        rootClass = globals().get(tag)
+        rootClass = globals().get(prefix_tag)
     return tag, rootClass
 
 
 def get_required_ns_prefix_defs(rootNode):
-    '''Get all name space prefix definitions required in this XML doc.
+    """Get all name space prefix definitions required in this XML doc.
     Return a dictionary of definitions and a char string of definitions.
-    '''
+    """
     nsmap = {
         prefix: uri
         for node in rootNode.iter()
         for (prefix, uri) in node.nsmap.items()
         if prefix is not None
     }
-    namespacedefs = ' '.join([
-        'xmlns:{}="{}"'.format(prefix, uri)
-        for prefix, uri in nsmap.items()
-    ])
+    namespacedefs = " ".join(
+        ['xmlns:{}="{}"'.format(prefix, uri) for prefix, uri in nsmap.items()]
+    )
     return nsmap, namespacedefs
 
 
 def parse(inFileName, silence=False, print_warnings=True):
     global CapturedNsmap_
     gds_collector = GdsCollector_()
     parser = None
     doc = parsexml_(inFileName, parser)
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
-        rootTag = 'root'
+        rootTag = "root"
         rootClass = root
     rootObj = rootClass.factory()
     rootObj.build(rootNode, gds_collector_=gds_collector)
     CapturedNsmap_, namespacedefs = get_required_ns_prefix_defs(rootNode)
     if not SaveElementTreeNode:
         doc = None
         rootNode = None
     if not silence:
         sys.stdout.write('<?xml version="1.0" ?>\n')
         rootObj.export(
-            sys.stdout, 0, name_=rootTag,
+            sys.stdout,
+            0,
+            name_=rootTag,
             namespacedef_=namespacedefs,
-            pretty_print=True)
+            pretty_print=True,
+        )
     if print_warnings and len(gds_collector.get_messages()) > 0:
-        separator = ('-' * 50) + '\n'
+        separator = ("-" * 50) + "\n"
         sys.stderr.write(separator)
-        sys.stderr.write('----- Warnings -- count: {} -----\n'.format(
-            len(gds_collector.get_messages()), ))
+        sys.stderr.write(
+            "----- Warnings -- count: {} -----\n".format(
+                len(gds_collector.get_messages()),
+            )
+        )
         gds_collector.write_messages(sys.stderr)
         sys.stderr.write(separator)
     return rootObj
 
 
-def parseEtree(inFileName, silence=False, print_warnings=True,
-               mapping=None, nsmap=None):
+def parseEtree(
+    inFileName,
+    silence=False,
+    print_warnings=True,
+    mapping=None,
+    reverse_mapping=None,
+    nsmap=None,
+):
     parser = None
     doc = parsexml_(inFileName, parser)
     gds_collector = GdsCollector_()
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
-        rootTag = 'root'
+        rootTag = "root"
         rootClass = root
     rootObj = rootClass.factory()
     rootObj.build(rootNode, gds_collector_=gds_collector)
-    # Enable Python to collect the space used by the DOM.
     if mapping is None:
         mapping = {}
+    if reverse_mapping is None:
+        reverse_mapping = {}
     rootElement = rootObj.to_etree(
-        None, name_=rootTag, mapping_=mapping, nsmap_=nsmap)
-    reverse_mapping = rootObj.gds_reverse_node_mapping(mapping)
+        None,
+        name_=rootTag,
+        mapping_=mapping,
+        reverse_mapping_=reverse_mapping,
+        nsmap_=nsmap,
+    )
+    reverse_node_mapping = rootObj.gds_reverse_node_mapping(mapping)
+    # Enable Python to collect the space used by the DOM.
     if not SaveElementTreeNode:
         doc = None
         rootNode = None
     if not silence:
         content = etree_.tostring(
-            rootElement, pretty_print=True,
-            xml_declaration=True, encoding="utf-8")
+            rootElement,
+            pretty_print=True,
+            xml_declaration=True,
+            encoding="utf-8",
+        )
         sys.stdout.write(str(content))
-        sys.stdout.write('\n')
+        sys.stdout.write("\n")
     if print_warnings and len(gds_collector.get_messages()) > 0:
-        separator = ('-' * 50) + '\n'
+        separator = ("-" * 50) + "\n"
         sys.stderr.write(separator)
-        sys.stderr.write('----- Warnings -- count: {} -----\n'.format(
-            len(gds_collector.get_messages()), ))
+        sys.stderr.write(
+            "----- Warnings -- count: {} -----\n".format(
+                len(gds_collector.get_messages()),
+            )
+        )
         gds_collector.write_messages(sys.stderr)
         sys.stderr.write(separator)
-    return rootObj, rootElement, mapping, reverse_mapping
+    return rootObj, rootElement, mapping, reverse_node_mapping
 
 
 def parseString(inString, silence=False, print_warnings=True):
-    '''Parse a string, create the object tree, and export it.
+    """Parse a string, create the object tree, and export it.
 
     Arguments:
     - inString -- A string.  This XML fragment should not start
       with an XML declaration containing an encoding.
     - silence -- A boolean.  If False, export the object.
     Returns -- The root object in the tree.
-    '''
+    """
     parser = None
-    rootNode= parsexmlstring_(inString, parser)
+    rootNode = parsexmlstring_(inString, parser)
     gds_collector = GdsCollector_()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
-        rootTag = 'root'
+        rootTag = "root"
         rootClass = root
     rootObj = rootClass.factory()
     rootObj.build(rootNode, gds_collector_=gds_collector)
     if not SaveElementTreeNode:
         rootNode = None
     if not silence:
         sys.stdout.write('<?xml version="1.0" ?>\n')
         rootObj.export(
-            sys.stdout, 0, name_=rootTag,
-            namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0"')
+            sys.stdout,
+            0,
+            name_=rootTag,
+            namespacedef_='xmlns:tns="urn:schemas-upnp-org:device-1-0"',
+        )
     if print_warnings and len(gds_collector.get_messages()) > 0:
-        separator = ('-' * 50) + '\n'
+        separator = ("-" * 50) + "\n"
         sys.stderr.write(separator)
-        sys.stderr.write('----- Warnings -- count: {} -----\n'.format(
-            len(gds_collector.get_messages()), ))
+        sys.stderr.write(
+            "----- Warnings -- count: {} -----\n".format(
+                len(gds_collector.get_messages()),
+            )
+        )
         gds_collector.write_messages(sys.stderr)
         sys.stderr.write(separator)
     return rootObj
 
 
 def parseLiteral(inFileName, silence=False, print_warnings=True):
     parser = None
     doc = parsexml_(inFileName, parser)
     gds_collector = GdsCollector_()
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
-        rootTag = 'root'
+        rootTag = "root"
         rootClass = root
     rootObj = rootClass.factory()
     rootObj.build(rootNode, gds_collector_=gds_collector)
     # Enable Python to collect the space used by the DOM.
     if not SaveElementTreeNode:
         doc = None
         rootNode = None
     if not silence:
-        sys.stdout.write('#from device import *\n\n')
-        sys.stdout.write('import device as model_\n\n')
-        sys.stdout.write('rootObj = model_.rootClass(\n')
+        sys.stdout.write("#from device import *\n\n")
+        sys.stdout.write("import device as model_\n\n")
+        sys.stdout.write("rootObj = model_.rootClass(\n")
         rootObj.exportLiteral(sys.stdout, 0, name_=rootTag)
-        sys.stdout.write(')\n')
+        sys.stdout.write(")\n")
     if print_warnings and len(gds_collector.get_messages()) > 0:
-        separator = ('-' * 50) + '\n'
+        separator = ("-" * 50) + "\n"
         sys.stderr.write(separator)
-        sys.stderr.write('----- Warnings -- count: {} -----\n'.format(
-            len(gds_collector.get_messages()), ))
+        sys.stderr.write(
+            "----- Warnings -- count: {} -----\n".format(
+                len(gds_collector.get_messages()),
+            )
+        )
         gds_collector.write_messages(sys.stderr)
         sys.stderr.write(separator)
     return rootObj
 
 
 def main():
     args = sys.argv[1:]
     if len(args) == 1:
         parse(args[0])
     else:
         usage()
 
 
-if __name__ == '__main__':
-    #import pdb; pdb.set_trace()
+if __name__ == "__main__":
+    # import pdb; pdb.set_trace()
     main()
 
-RenameMappings_ = {
-}
+RenameMappings_ = {}
 
 #
 # Mapping of namespaces to types defined in them
 # and the file in which each is defined.
 # simpleTypes are marked "ST" and complexTypes "CT".
-NamespaceToDefMappings_ = {'urn:schemas-upnp-org:device-1-0': [('SpecVersionType', 'device.xsd', 'CT'),
-                                     ('DeviceType', 'device.xsd', 'CT'),
-                                     ('IconListType', 'device.xsd', 'CT'),
-                                     ('ServiceListType', 'device.xsd', 'CT'),
-                                     ('DeviceListType', 'device.xsd', 'CT')]}
+NamespaceToDefMappings_ = {
+    "urn:schemas-upnp-org:device-1-0": [
+        ("SpecVersionType", "pywemo/ouimeaux_device/api/xsd/device.xsd", "CT"),
+        ("DeviceType", "pywemo/ouimeaux_device/api/xsd/device.xsd", "CT"),
+        ("IconListType", "pywemo/ouimeaux_device/api/xsd/device.xsd", "CT"),
+        ("ServiceListType", "pywemo/ouimeaux_device/api/xsd/device.xsd", "CT"),
+        ("DeviceListType", "pywemo/ouimeaux_device/api/xsd/device.xsd", "CT"),
+    ]
+}
 
 __all__ = [
     "DeviceListType",
     "DeviceType",
     "IconListType",
     "ServiceListType",
     "SpecVersionType",
     "iconType",
     "root",
-    "serviceType"
+    "serviceType",
 ]
```

### Comparing `pywemo-0.9.2/pywemo/ouimeaux_device/api/xsd/device.xsd` & `pywemo-1.0.0/pywemo/ouimeaux_device/api/xsd/device.xsd`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.2/pywemo/ouimeaux_device/api/xsd/service.py` & `pywemo-1.0.0/pywemo/ouimeaux_device/api/xsd/service.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
+# flake8: noqa
+# isort: skip_file
+# mypy: ignore-errors
+# pylint: skip-file
 
 #
-# Generated Sun Dec 27 17:49:35 2020 by generateDS.py version 2.37.11.
-# Python 3.8.5 (default, Jul 28 2020, 12:59:40)  [GCC 9.3.0]
+# Generated  by generateDS.py version 2.41.5.
+# Python [sys.version]
 #
 # Command line options:
+#   ('-f', '')
+#   ('--no-dates', '')
 #   ('-o', 'service.py')
 #
 # Command line arguments:
-#   service.xsd
+#   pywemo/ouimeaux_device/api/xsd/service.xsd
 #
 # Command line:
-#   generateDS -o "service.py" service.xsd
+#   generateDS.py -f --no-dates -o "service.py" pywemo/ouimeaux_device/api/xsd/service.xsd
 #
 # Current working directory (os.getcwd()):
-#   xsd
+#   pywemo
 #
 
 import sys
+
 try:
     ModulenotfoundExp_ = ModuleNotFoundError
 except NameError:
     ModulenotfoundExp_ = ImportError
 from itertools import zip_longest
 import os
 import re as re_
 import base64
 import datetime as datetime_
 import decimal as decimal_
-try:
-    from lxml import etree as etree_
-except ModulenotfoundExp_ :
-    from xml.etree import ElementTree as etree_
+from lxml import etree as etree_
 
 
 Validate_simpletypes_ = True
 SaveElementTreeNode = True
+TagNamePrefix = ""
 if sys.version_info.major == 2:
     BaseStrType_ = basestring
 else:
     BaseStrType_ = str
 
 
 def parsexml_(infile, parser=None, **kwargs):
@@ -56,26 +61,28 @@
         if isinstance(infile, os.PathLike):
             infile = os.path.join(infile)
     except AttributeError:
         pass
     doc = etree_.parse(infile, parser=parser, **kwargs)
     return doc
 
+
 def parsexmlstring_(instring, parser=None, **kwargs):
     if parser is None:
         # Use the lxml ElementTree compatible parser so that, e.g.,
         #   we ignore comments.
         try:
             parser = etree_.ETCompatXMLParser()
         except AttributeError:
             # fallback to xml.etree
             parser = etree_.XMLParser()
     element = etree_.fromstring(instring, parser=parser, **kwargs)
     return element
 
+
 #
 # Namespace prefix definition table (and other attributes, too)
 #
 # The module generatedsnamespaces, if it is importable, must contain
 # a dictionary named GeneratedsNamespaceDefs.  This Python dictionary
 # should map element type names (strings) to XML schema namespace prefix
 # definitions.  The export method for any class for which there is
@@ -91,48 +98,51 @@
 #         "ElementtypeA": "http://www.xxx.com/namespaceA",
 #         "ElementtypeB": "http://www.xxx.com/namespaceB",
 #     }
 #
 # Additionally, the generatedsnamespaces module can contain a python
 # dictionary named GenerateDSNamespaceTypePrefixes that associates element
 # types with the namespace prefixes that are to be added to the
-# "xsi:type" attribute value.  See the exportAttributes method of
+# "xsi:type" attribute value.  See the _exportAttributes method of
 # any generated element type and the generation of "xsi:type" for an
 # example of the use of this table.
 # An example table:
 #
 #     # File: generatedsnamespaces.py
 #
 #     GenerateDSNamespaceTypePrefixes = {
 #         "ElementtypeC": "aaa:",
 #         "ElementtypeD": "bbb:",
 #     }
 #
 
 try:
-    from generatedsnamespaces import GenerateDSNamespaceDefs as GenerateDSNamespaceDefs_
-except ModulenotfoundExp_ :
+    from generatedsnamespaces import (
+        GenerateDSNamespaceDefs as GenerateDSNamespaceDefs_,
+    )
+except ModulenotfoundExp_:
     GenerateDSNamespaceDefs_ = {}
 try:
-    from generatedsnamespaces import GenerateDSNamespaceTypePrefixes as GenerateDSNamespaceTypePrefixes_
-except ModulenotfoundExp_ :
+    from generatedsnamespaces import (
+        GenerateDSNamespaceTypePrefixes as GenerateDSNamespaceTypePrefixes_,
+    )
+except ModulenotfoundExp_:
     GenerateDSNamespaceTypePrefixes_ = {}
 
 #
 # You can replace the following class definition by defining an
 # importable module named "generatedscollector" containing a class
 # named "GdsCollector".  See the default class definition below for
 # clues about the possible content of that class.
 #
 try:
     from generatedscollector import GdsCollector as GdsCollector_
-except ModulenotfoundExp_ :
+except ModulenotfoundExp_:
 
     class GdsCollector_(object):
-
         def __init__(self, messages=None):
             if messages is None:
                 self.messages = []
             else:
                 self.messages = messages
 
         def add_message(self, msg):
@@ -155,514 +165,692 @@
 
 #
 # The super-class for enum types
 #
 
 try:
     from enum import Enum
-except ModulenotfoundExp_ :
+except ModulenotfoundExp_:
     Enum = object
 
 #
 # The root super-class for element type classes
 #
 # Calls to the methods in these classes are generated by generateDS.py.
 # You can replace these methods by re-implementing the following class
 #   in a module named generatedssuper.py.
 
 try:
     from generatedssuper import GeneratedsSuper
 except ModulenotfoundExp_ as exp:
+    try:
+        from generatedssupersuper import GeneratedsSuperSuper
+    except ModulenotfoundExp_ as exp:
+
+        class GeneratedsSuperSuper(object):
+            pass
 
-    class GeneratedsSuper(object):
+    class GeneratedsSuper(GeneratedsSuperSuper):
         __hash__ = object.__hash__
-        tzoff_pattern = re_.compile(r'(\+|-)((0\d|1[0-3]):[0-5]\d|14:00)$')
+        tzoff_pattern = re_.compile(r"(\+|-)((0\d|1[0-3]):[0-5]\d|14:00)$")
+
         class _FixedOffsetTZ(datetime_.tzinfo):
             def __init__(self, offset, name):
                 self.__offset = datetime_.timedelta(minutes=offset)
                 self.__name = name
+
             def utcoffset(self, dt):
                 return self.__offset
+
             def tzname(self, dt):
                 return self.__name
+
             def dst(self, dt):
                 return None
-        def gds_format_string(self, input_data, input_name=''):
+
+        def __str__(self):
+            settings = {
+                "str_pretty_print": True,
+                "str_indent_level": 0,
+                "str_namespaceprefix": "",
+                "str_name": self.__class__.__name__,
+                "str_namespacedefs": "",
+            }
+            for n in settings:
+                if hasattr(self, n):
+                    settings[n] = getattr(self, n)
+            if sys.version_info.major == 2:
+                from StringIO import StringIO
+            else:
+                from io import StringIO
+            output = StringIO()
+            self.export(
+                output,
+                settings["str_indent_level"],
+                pretty_print=settings["str_pretty_print"],
+                namespaceprefix_=settings["str_namespaceprefix"],
+                name_=settings["str_name"],
+                namespacedef_=settings["str_namespacedefs"],
+            )
+            strval = output.getvalue()
+            output.close()
+            return strval
+
+        def gds_format_string(self, input_data, input_name=""):
             return input_data
-        def gds_parse_string(self, input_data, node=None, input_name=''):
+
+        def gds_parse_string(self, input_data, node=None, input_name=""):
             return input_data
-        def gds_validate_string(self, input_data, node=None, input_name=''):
+
+        def gds_validate_string(self, input_data, node=None, input_name=""):
             if not input_data:
-                return ''
+                return ""
             else:
                 return input_data
-        def gds_format_base64(self, input_data, input_name=''):
-            return base64.b64encode(input_data)
-        def gds_validate_base64(self, input_data, node=None, input_name=''):
+
+        def gds_format_base64(self, input_data, input_name=""):
+            return base64.b64encode(input_data).decode("ascii")
+
+        def gds_validate_base64(self, input_data, node=None, input_name=""):
             return input_data
-        def gds_format_integer(self, input_data, input_name=''):
-            return '%d' % input_data
-        def gds_parse_integer(self, input_data, node=None, input_name=''):
+
+        def gds_format_integer(self, input_data, input_name=""):
+            return "%d" % int(input_data)
+
+        def gds_parse_integer(self, input_data, node=None, input_name=""):
             try:
                 ival = int(input_data)
             except (TypeError, ValueError) as exp:
-                raise_parse_error(node, 'Requires integer value: %s' % exp)
+                raise_parse_error(node, "Requires integer value: %s" % exp)
             return ival
-        def gds_validate_integer(self, input_data, node=None, input_name=''):
+
+        def gds_validate_integer(self, input_data, node=None, input_name=""):
             try:
                 value = int(input_data)
             except (TypeError, ValueError):
-                raise_parse_error(node, 'Requires integer value')
+                raise_parse_error(node, "Requires integer value")
             return value
-        def gds_format_integer_list(self, input_data, input_name=''):
-            if len(input_data) > 0 and not isinstance(input_data[0], BaseStrType_):
+
+        def gds_format_integer_list(self, input_data, input_name=""):
+            if len(input_data) > 0 and not isinstance(
+                input_data[0], BaseStrType_
+            ):
                 input_data = [str(s) for s in input_data]
-            return '%s' % ' '.join(input_data)
+            return "%s" % " ".join(input_data)
+
         def gds_validate_integer_list(
-                self, input_data, node=None, input_name=''):
+            self, input_data, node=None, input_name=""
+        ):
             values = input_data.split()
             for value in values:
                 try:
                     int(value)
                 except (TypeError, ValueError):
-                    raise_parse_error(node, 'Requires sequence of integer values')
+                    raise_parse_error(
+                        node, "Requires sequence of integer values"
+                    )
             return values
-        def gds_format_float(self, input_data, input_name=''):
-            return ('%.15f' % input_data).rstrip('0')
-        def gds_parse_float(self, input_data, node=None, input_name=''):
+
+        def gds_format_float(self, input_data, input_name=""):
+            value = ("%.15f" % float(input_data)).rstrip("0")
+            if value.endswith("."):
+                value += "0"
+            return value
+
+        def gds_parse_float(self, input_data, node=None, input_name=""):
             try:
                 fval_ = float(input_data)
             except (TypeError, ValueError) as exp:
-                raise_parse_error(node, 'Requires float or double value: %s' % exp)
+                raise_parse_error(
+                    node, "Requires float or double value: %s" % exp
+                )
             return fval_
-        def gds_validate_float(self, input_data, node=None, input_name=''):
+
+        def gds_validate_float(self, input_data, node=None, input_name=""):
             try:
                 value = float(input_data)
             except (TypeError, ValueError):
-                raise_parse_error(node, 'Requires float value')
+                raise_parse_error(node, "Requires float value")
             return value
-        def gds_format_float_list(self, input_data, input_name=''):
-            if len(input_data) > 0 and not isinstance(input_data[0], BaseStrType_):
+
+        def gds_format_float_list(self, input_data, input_name=""):
+            if len(input_data) > 0 and not isinstance(
+                input_data[0], BaseStrType_
+            ):
                 input_data = [str(s) for s in input_data]
-            return '%s' % ' '.join(input_data)
+            return "%s" % " ".join(input_data)
+
         def gds_validate_float_list(
-                self, input_data, node=None, input_name=''):
+            self, input_data, node=None, input_name=""
+        ):
             values = input_data.split()
             for value in values:
                 try:
                     float(value)
                 except (TypeError, ValueError):
-                    raise_parse_error(node, 'Requires sequence of float values')
+                    raise_parse_error(
+                        node, "Requires sequence of float values"
+                    )
             return values
-        def gds_format_decimal(self, input_data, input_name=''):
-            return_value = '%s' % input_data
-            if '.' in return_value:
-                return_value = return_value.rstrip('0')
-                if return_value.endswith('.'):
-                    return_value = return_value.rstrip('.')
+
+        def gds_format_decimal(self, input_data, input_name=""):
+            return_value = "%s" % input_data
+            if "." in return_value:
+                return_value = return_value.rstrip("0")
+                if return_value.endswith("."):
+                    return_value = return_value.rstrip(".")
             return return_value
-        def gds_parse_decimal(self, input_data, node=None, input_name=''):
+
+        def gds_parse_decimal(self, input_data, node=None, input_name=""):
             try:
                 decimal_value = decimal_.Decimal(input_data)
             except (TypeError, ValueError):
-                raise_parse_error(node, 'Requires decimal value')
+                raise_parse_error(node, "Requires decimal value")
             return decimal_value
-        def gds_validate_decimal(self, input_data, node=None, input_name=''):
+
+        def gds_validate_decimal(self, input_data, node=None, input_name=""):
             try:
                 value = decimal_.Decimal(input_data)
             except (TypeError, ValueError):
-                raise_parse_error(node, 'Requires decimal value')
+                raise_parse_error(node, "Requires decimal value")
             return value
-        def gds_format_decimal_list(self, input_data, input_name=''):
-            if len(input_data) > 0 and not isinstance(input_data[0], BaseStrType_):
+
+        def gds_format_decimal_list(self, input_data, input_name=""):
+            if len(input_data) > 0 and not isinstance(
+                input_data[0], BaseStrType_
+            ):
                 input_data = [str(s) for s in input_data]
-            return ' '.join([self.gds_format_decimal(item) for item in input_data])
+            return " ".join(
+                [self.gds_format_decimal(item) for item in input_data]
+            )
+
         def gds_validate_decimal_list(
-                self, input_data, node=None, input_name=''):
+            self, input_data, node=None, input_name=""
+        ):
             values = input_data.split()
             for value in values:
                 try:
                     decimal_.Decimal(value)
                 except (TypeError, ValueError):
-                    raise_parse_error(node, 'Requires sequence of decimal values')
+                    raise_parse_error(
+                        node, "Requires sequence of decimal values"
+                    )
             return values
-        def gds_format_double(self, input_data, input_name=''):
-            return '%s' % input_data
-        def gds_parse_double(self, input_data, node=None, input_name=''):
+
+        def gds_format_double(self, input_data, input_name=""):
+            return "%s" % input_data
+
+        def gds_parse_double(self, input_data, node=None, input_name=""):
             try:
                 fval_ = float(input_data)
             except (TypeError, ValueError) as exp:
-                raise_parse_error(node, 'Requires double or float value: %s' % exp)
+                raise_parse_error(
+                    node, "Requires double or float value: %s" % exp
+                )
             return fval_
-        def gds_validate_double(self, input_data, node=None, input_name=''):
+
+        def gds_validate_double(self, input_data, node=None, input_name=""):
             try:
                 value = float(input_data)
             except (TypeError, ValueError):
-                raise_parse_error(node, 'Requires double or float value')
+                raise_parse_error(node, "Requires double or float value")
             return value
-        def gds_format_double_list(self, input_data, input_name=''):
-            if len(input_data) > 0 and not isinstance(input_data[0], BaseStrType_):
+
+        def gds_format_double_list(self, input_data, input_name=""):
+            if len(input_data) > 0 and not isinstance(
+                input_data[0], BaseStrType_
+            ):
                 input_data = [str(s) for s in input_data]
-            return '%s' % ' '.join(input_data)
+            return "%s" % " ".join(input_data)
+
         def gds_validate_double_list(
-                self, input_data, node=None, input_name=''):
+            self, input_data, node=None, input_name=""
+        ):
             values = input_data.split()
             for value in values:
                 try:
                     float(value)
                 except (TypeError, ValueError):
                     raise_parse_error(
-                        node, 'Requires sequence of double or float values')
+                        node, "Requires sequence of double or float values"
+                    )
             return values
-        def gds_format_boolean(self, input_data, input_name=''):
-            return ('%s' % input_data).lower()
-        def gds_parse_boolean(self, input_data, node=None, input_name=''):
-            if input_data in ('true', '1'):
+
+        def gds_format_boolean(self, input_data, input_name=""):
+            return ("%s" % input_data).lower()
+
+        def gds_parse_boolean(self, input_data, node=None, input_name=""):
+            input_data = input_data.strip()
+            if input_data in ("true", "1"):
                 bval = True
-            elif input_data in ('false', '0'):
+            elif input_data in ("false", "0"):
                 bval = False
             else:
-                raise_parse_error(node, 'Requires boolean value')
+                raise_parse_error(node, "Requires boolean value")
             return bval
-        def gds_validate_boolean(self, input_data, node=None, input_name=''):
-            if input_data not in (True, 1, False, 0, ):
+
+        def gds_validate_boolean(self, input_data, node=None, input_name=""):
+            if input_data not in (
+                True,
+                1,
+                False,
+                0,
+            ):
                 raise_parse_error(
                     node,
-                    'Requires boolean value '
-                    '(one of True, 1, False, 0)')
+                    "Requires boolean value " "(one of True, 1, False, 0)",
+                )
             return input_data
-        def gds_format_boolean_list(self, input_data, input_name=''):
-            if len(input_data) > 0 and not isinstance(input_data[0], BaseStrType_):
+
+        def gds_format_boolean_list(self, input_data, input_name=""):
+            if len(input_data) > 0 and not isinstance(
+                input_data[0], BaseStrType_
+            ):
                 input_data = [str(s) for s in input_data]
-            return '%s' % ' '.join(input_data)
+            return "%s" % " ".join(input_data)
+
         def gds_validate_boolean_list(
-                self, input_data, node=None, input_name=''):
+            self, input_data, node=None, input_name=""
+        ):
             values = input_data.split()
             for value in values:
-                if value not in (True, 1, False, 0, ):
+                value = self.gds_parse_boolean(value, node, input_name)
+                if value not in (
+                    True,
+                    1,
+                    False,
+                    0,
+                ):
                     raise_parse_error(
                         node,
-                        'Requires sequence of boolean values '
-                        '(one of True, 1, False, 0)')
+                        "Requires sequence of boolean values "
+                        "(one of True, 1, False, 0)",
+                    )
             return values
-        def gds_validate_datetime(self, input_data, node=None, input_name=''):
+
+        def gds_validate_datetime(self, input_data, node=None, input_name=""):
             return input_data
-        def gds_format_datetime(self, input_data, input_name=''):
+
+        def gds_format_datetime(self, input_data, input_name=""):
             if input_data.microsecond == 0:
-                _svalue = '%04d-%02d-%02dT%02d:%02d:%02d' % (
+                _svalue = "%04d-%02d-%02dT%02d:%02d:%02d" % (
                     input_data.year,
                     input_data.month,
                     input_data.day,
                     input_data.hour,
                     input_data.minute,
                     input_data.second,
                 )
             else:
-                _svalue = '%04d-%02d-%02dT%02d:%02d:%02d.%s' % (
+                _svalue = "%04d-%02d-%02dT%02d:%02d:%02d.%s" % (
                     input_data.year,
                     input_data.month,
                     input_data.day,
                     input_data.hour,
                     input_data.minute,
                     input_data.second,
-                    ('%f' % (float(input_data.microsecond) / 1000000))[2:],
+                    ("%f" % (float(input_data.microsecond) / 1000000))[2:],
                 )
             if input_data.tzinfo is not None:
                 tzoff = input_data.tzinfo.utcoffset(input_data)
                 if tzoff is not None:
                     total_seconds = tzoff.seconds + (86400 * tzoff.days)
                     if total_seconds == 0:
-                        _svalue += 'Z'
+                        _svalue += "Z"
                     else:
                         if total_seconds < 0:
-                            _svalue += '-'
+                            _svalue += "-"
                             total_seconds *= -1
                         else:
-                            _svalue += '+'
+                            _svalue += "+"
                         hours = total_seconds // 3600
                         minutes = (total_seconds - (hours * 3600)) // 60
-                        _svalue += '{0:02d}:{1:02d}'.format(hours, minutes)
+                        _svalue += "{0:02d}:{1:02d}".format(hours, minutes)
             return _svalue
+
         @classmethod
         def gds_parse_datetime(cls, input_data):
             tz = None
-            if input_data[-1] == 'Z':
-                tz = GeneratedsSuper._FixedOffsetTZ(0, 'UTC')
+            if input_data[-1] == "Z":
+                tz = GeneratedsSuper._FixedOffsetTZ(0, "UTC")
                 input_data = input_data[:-1]
             else:
                 results = GeneratedsSuper.tzoff_pattern.search(input_data)
                 if results is not None:
-                    tzoff_parts = results.group(2).split(':')
+                    tzoff_parts = results.group(2).split(":")
                     tzoff = int(tzoff_parts[0]) * 60 + int(tzoff_parts[1])
-                    if results.group(1) == '-':
+                    if results.group(1) == "-":
                         tzoff *= -1
                     tz = GeneratedsSuper._FixedOffsetTZ(
-                        tzoff, results.group(0))
+                        tzoff, results.group(0)
+                    )
                     input_data = input_data[:-6]
-            time_parts = input_data.split('.')
+            time_parts = input_data.split(".")
             if len(time_parts) > 1:
-                micro_seconds = int(float('0.' + time_parts[1]) * 1000000)
-                input_data = '%s.%s' % (
-                    time_parts[0], "{}".format(micro_seconds).rjust(6, "0"), )
+                micro_seconds = int(float("0." + time_parts[1]) * 1000000)
+                input_data = "%s.%s" % (
+                    time_parts[0],
+                    "{}".format(micro_seconds).rjust(6, "0"),
+                )
                 dt = datetime_.datetime.strptime(
-                    input_data, '%Y-%m-%dT%H:%M:%S.%f')
+                    input_data, "%Y-%m-%dT%H:%M:%S.%f"
+                )
             else:
                 dt = datetime_.datetime.strptime(
-                    input_data, '%Y-%m-%dT%H:%M:%S')
+                    input_data, "%Y-%m-%dT%H:%M:%S"
+                )
             dt = dt.replace(tzinfo=tz)
             return dt
-        def gds_validate_date(self, input_data, node=None, input_name=''):
+
+        def gds_validate_date(self, input_data, node=None, input_name=""):
             return input_data
-        def gds_format_date(self, input_data, input_name=''):
-            _svalue = '%04d-%02d-%02d' % (
+
+        def gds_format_date(self, input_data, input_name=""):
+            _svalue = "%04d-%02d-%02d" % (
                 input_data.year,
                 input_data.month,
                 input_data.day,
             )
             try:
                 if input_data.tzinfo is not None:
                     tzoff = input_data.tzinfo.utcoffset(input_data)
                     if tzoff is not None:
                         total_seconds = tzoff.seconds + (86400 * tzoff.days)
                         if total_seconds == 0:
-                            _svalue += 'Z'
+                            _svalue += "Z"
                         else:
                             if total_seconds < 0:
-                                _svalue += '-'
+                                _svalue += "-"
                                 total_seconds *= -1
                             else:
-                                _svalue += '+'
+                                _svalue += "+"
                             hours = total_seconds // 3600
                             minutes = (total_seconds - (hours * 3600)) // 60
-                            _svalue += '{0:02d}:{1:02d}'.format(
-                                hours, minutes)
+                            _svalue += "{0:02d}:{1:02d}".format(hours, minutes)
             except AttributeError:
                 pass
             return _svalue
+
         @classmethod
         def gds_parse_date(cls, input_data):
             tz = None
-            if input_data[-1] == 'Z':
-                tz = GeneratedsSuper._FixedOffsetTZ(0, 'UTC')
+            if input_data[-1] == "Z":
+                tz = GeneratedsSuper._FixedOffsetTZ(0, "UTC")
                 input_data = input_data[:-1]
             else:
                 results = GeneratedsSuper.tzoff_pattern.search(input_data)
                 if results is not None:
-                    tzoff_parts = results.group(2).split(':')
+                    tzoff_parts = results.group(2).split(":")
                     tzoff = int(tzoff_parts[0]) * 60 + int(tzoff_parts[1])
-                    if results.group(1) == '-':
+                    if results.group(1) == "-":
                         tzoff *= -1
                     tz = GeneratedsSuper._FixedOffsetTZ(
-                        tzoff, results.group(0))
+                        tzoff, results.group(0)
+                    )
                     input_data = input_data[:-6]
-            dt = datetime_.datetime.strptime(input_data, '%Y-%m-%d')
+            dt = datetime_.datetime.strptime(input_data, "%Y-%m-%d")
             dt = dt.replace(tzinfo=tz)
             return dt.date()
-        def gds_validate_time(self, input_data, node=None, input_name=''):
+
+        def gds_validate_time(self, input_data, node=None, input_name=""):
             return input_data
-        def gds_format_time(self, input_data, input_name=''):
+
+        def gds_format_time(self, input_data, input_name=""):
             if input_data.microsecond == 0:
-                _svalue = '%02d:%02d:%02d' % (
+                _svalue = "%02d:%02d:%02d" % (
                     input_data.hour,
                     input_data.minute,
                     input_data.second,
                 )
             else:
-                _svalue = '%02d:%02d:%02d.%s' % (
+                _svalue = "%02d:%02d:%02d.%s" % (
                     input_data.hour,
                     input_data.minute,
                     input_data.second,
-                    ('%f' % (float(input_data.microsecond) / 1000000))[2:],
+                    ("%f" % (float(input_data.microsecond) / 1000000))[2:],
                 )
             if input_data.tzinfo is not None:
                 tzoff = input_data.tzinfo.utcoffset(input_data)
                 if tzoff is not None:
                     total_seconds = tzoff.seconds + (86400 * tzoff.days)
                     if total_seconds == 0:
-                        _svalue += 'Z'
+                        _svalue += "Z"
                     else:
                         if total_seconds < 0:
-                            _svalue += '-'
+                            _svalue += "-"
                             total_seconds *= -1
                         else:
-                            _svalue += '+'
+                            _svalue += "+"
                         hours = total_seconds // 3600
                         minutes = (total_seconds - (hours * 3600)) // 60
-                        _svalue += '{0:02d}:{1:02d}'.format(hours, minutes)
+                        _svalue += "{0:02d}:{1:02d}".format(hours, minutes)
             return _svalue
+
         def gds_validate_simple_patterns(self, patterns, target):
             # pat is a list of lists of strings/patterns.
             # The target value must match at least one of the patterns
             # in order for the test to succeed.
             found1 = True
+            target = str(target)
             for patterns1 in patterns:
                 found2 = False
                 for patterns2 in patterns1:
                     mo = re_.search(patterns2, target)
                     if mo is not None and len(mo.group(0)) == len(target):
                         found2 = True
                         break
                 if not found2:
                     found1 = False
                     break
             return found1
+
         @classmethod
         def gds_parse_time(cls, input_data):
             tz = None
-            if input_data[-1] == 'Z':
-                tz = GeneratedsSuper._FixedOffsetTZ(0, 'UTC')
+            if input_data[-1] == "Z":
+                tz = GeneratedsSuper._FixedOffsetTZ(0, "UTC")
                 input_data = input_data[:-1]
             else:
                 results = GeneratedsSuper.tzoff_pattern.search(input_data)
                 if results is not None:
-                    tzoff_parts = results.group(2).split(':')
+                    tzoff_parts = results.group(2).split(":")
                     tzoff = int(tzoff_parts[0]) * 60 + int(tzoff_parts[1])
-                    if results.group(1) == '-':
+                    if results.group(1) == "-":
                         tzoff *= -1
                     tz = GeneratedsSuper._FixedOffsetTZ(
-                        tzoff, results.group(0))
+                        tzoff, results.group(0)
+                    )
                     input_data = input_data[:-6]
-            if len(input_data.split('.')) > 1:
-                dt = datetime_.datetime.strptime(input_data, '%H:%M:%S.%f')
+            if len(input_data.split(".")) > 1:
+                dt = datetime_.datetime.strptime(input_data, "%H:%M:%S.%f")
             else:
-                dt = datetime_.datetime.strptime(input_data, '%H:%M:%S')
+                dt = datetime_.datetime.strptime(input_data, "%H:%M:%S")
             dt = dt.replace(tzinfo=tz)
             return dt.time()
+
         def gds_check_cardinality_(
-                self, value, input_name,
-                min_occurs=0, max_occurs=1, required=None):
+            self, value, input_name, min_occurs=0, max_occurs=1, required=None
+        ):
             if value is None:
                 length = 0
             elif isinstance(value, list):
                 length = len(value)
             else:
                 length = 1
-            if required is not None :
+            if required is not None:
                 if required and length < 1:
                     self.gds_collector_.add_message(
                         "Required value {}{} is missing".format(
-                            input_name, self.gds_get_node_lineno_()))
+                            input_name, self.gds_get_node_lineno_()
+                        )
+                    )
             if length < min_occurs:
                 self.gds_collector_.add_message(
                     "Number of values for {}{} is below "
                     "the minimum allowed, "
                     "expected at least {}, found {}".format(
-                        input_name, self.gds_get_node_lineno_(),
-                        min_occurs, length))
+                        input_name,
+                        self.gds_get_node_lineno_(),
+                        min_occurs,
+                        length,
+                    )
+                )
             elif length > max_occurs:
                 self.gds_collector_.add_message(
                     "Number of values for {}{} is above "
                     "the maximum allowed, "
                     "expected at most {}, found {}".format(
-                        input_name, self.gds_get_node_lineno_(),
-                        max_occurs, length))
+                        input_name,
+                        self.gds_get_node_lineno_(),
+                        max_occurs,
+                        length,
+                    )
+                )
+
         def gds_validate_builtin_ST_(
-                self, validator, value, input_name,
-                min_occurs=None, max_occurs=None, required=None):
+            self,
+            validator,
+            value,
+            input_name,
+            min_occurs=None,
+            max_occurs=None,
+            required=None,
+        ):
             if value is not None:
                 try:
                     validator(value, input_name=input_name)
                 except GDSParseError as parse_error:
                     self.gds_collector_.add_message(str(parse_error))
+
         def gds_validate_defined_ST_(
-                self, validator, value, input_name,
-                min_occurs=None, max_occurs=None, required=None):
+            self,
+            validator,
+            value,
+            input_name,
+            min_occurs=None,
+            max_occurs=None,
+            required=None,
+        ):
             if value is not None:
                 try:
                     validator(value)
                 except GDSParseError as parse_error:
                     self.gds_collector_.add_message(str(parse_error))
+
         def gds_str_lower(self, instring):
             return instring.lower()
+
         def get_path_(self, node):
             path_list = []
             self.get_path_list_(node, path_list)
             path_list.reverse()
-            path = '/'.join(path_list)
+            path = "/".join(path_list)
             return path
-        Tag_strip_pattern_ = re_.compile(r'\{.*\}')
+
+        Tag_strip_pattern_ = re_.compile(r"\{.*\}")
+
         def get_path_list_(self, node, path_list):
             if node is None:
                 return
-            tag = GeneratedsSuper.Tag_strip_pattern_.sub('', node.tag)
+            tag = GeneratedsSuper.Tag_strip_pattern_.sub("", node.tag)
             if tag:
                 path_list.append(tag)
             self.get_path_list_(node.getparent(), path_list)
+
         def get_class_obj_(self, node, default_class=None):
             class_obj1 = default_class
-            if 'xsi' in node.nsmap:
-                classname = node.get('{%s}type' % node.nsmap['xsi'])
+            if "xsi" in node.nsmap:
+                classname = node.get("{%s}type" % node.nsmap["xsi"])
                 if classname is not None:
-                    names = classname.split(':')
+                    names = classname.split(":")
                     if len(names) == 2:
                         classname = names[1]
                     class_obj2 = globals().get(classname)
                     if class_obj2 is not None:
                         class_obj1 = class_obj2
             return class_obj1
+
         def gds_build_any(self, node, type_name=None):
             # provide default value in case option --disable-xml is used.
             content = ""
             content = etree_.tostring(node, encoding="unicode")
             return content
+
         @classmethod
         def gds_reverse_node_mapping(cls, mapping):
             return dict(((v, k) for k, v in mapping.items()))
+
         @staticmethod
         def gds_encode(instring):
             if sys.version_info.major == 2:
                 if ExternalEncoding:
                     encoding = ExternalEncoding
                 else:
-                    encoding = 'utf-8'
+                    encoding = "utf-8"
                 return instring.encode(encoding)
             else:
                 return instring
+
         @staticmethod
         def convert_unicode(instring):
             if isinstance(instring, str):
                 result = quote_xml(instring)
             elif sys.version_info.major == 2 and isinstance(instring, unicode):
-                result = quote_xml(instring).encode('utf8')
+                result = quote_xml(instring).encode("utf8")
             else:
                 result = GeneratedsSuper.gds_encode(str(instring))
             return result
+
         def __eq__(self, other):
             def excl_select_objs_(obj):
-                return (obj[0] != 'parent_object_' and
-                        obj[0] != 'gds_collector_')
+                return (
+                    obj[0] != "parent_object_" and obj[0] != "gds_collector_"
+                )
+
             if type(self) != type(other):
                 return False
-            return all(x == y for x, y in zip_longest(
-                filter(excl_select_objs_, self.__dict__.items()),
-                filter(excl_select_objs_, other.__dict__.items())))
+            return all(
+                x == y
+                for x, y in zip_longest(
+                    filter(excl_select_objs_, self.__dict__.items()),
+                    filter(excl_select_objs_, other.__dict__.items()),
+                )
+            )
+
         def __ne__(self, other):
             return not self.__eq__(other)
+
         # Django ETL transform hooks.
         def gds_djo_etl_transform(self):
             pass
+
         def gds_djo_etl_transform_db_obj(self, dbobj):
             pass
+
         # SQLAlchemy ETL transform hooks.
         def gds_sqa_etl_transform(self):
             return 0, None
+
         def gds_sqa_etl_transform_db_obj(self, dbobj):
             pass
+
         def gds_get_node_lineno_(self):
-            if (hasattr(self, "gds_elementtree_node_") and
-                    self.gds_elementtree_node_ is not None):
-                return ' near line {}'.format(
-                    self.gds_elementtree_node_.sourceline)
+            if (
+                hasattr(self, "gds_elementtree_node_")
+                and self.gds_elementtree_node_ is not None
+            ):
+                return " near line {}".format(
+                    self.gds_elementtree_node_.sourceline
+                )
             else:
                 return ""
 
-
     def getSubclassFromModule_(module, class_):
-        '''Get the subclass of a class from a specific module.'''
-        name = class_.__name__ + 'Sub'
+        """Get the subclass of a class from a specific module."""
+        name = class_.__name__ + "Sub"
         if hasattr(module, name):
             return getattr(module, name)
         else:
             return None
 
 
 #
@@ -680,131 +868,145 @@
 # IPython shell:
 #    ipshell('<some message> -- Entering ipshell.\nHit Ctrl-D to exit')
 
 #
 # Globals
 #
 
-ExternalEncoding = ''
+ExternalEncoding = ""
 # Set this to false in order to deactivate during export, the use of
 # name space prefixes captured from the input document.
 UseCapturedNS_ = True
 CapturedNsmap_ = {}
-Tag_pattern_ = re_.compile(r'({.*})?(.*)')
+Tag_pattern_ = re_.compile(r"({.*})?(.*)")
 String_cleanup_pat_ = re_.compile(r"[\n\r\s]+")
-Namespace_extract_pat_ = re_.compile(r'{(.*)}(.*)')
+Namespace_extract_pat_ = re_.compile(r"{(.*)}(.*)")
 CDATA_pattern_ = re_.compile(r"<!\[CDATA\[.*?\]\]>", re_.DOTALL)
 
 # Change this to redirect the generated superclass module to use a
 # specific subclass module.
 CurrentSubclassModule_ = None
 
 #
 # Support/utility functions.
 #
 
 
 def showIndent(outfile, level, pretty_print=True):
     if pretty_print:
         for idx in range(level):
-            outfile.write('    ')
+            outfile.write("    ")
 
 
 def quote_xml(inStr):
     "Escape markup chars, but do not modify CDATA sections."
     if not inStr:
-        return ''
-    s1 = (isinstance(inStr, BaseStrType_) and inStr or '%s' % inStr)
-    s2 = ''
+        return ""
+    s1 = isinstance(inStr, BaseStrType_) and inStr or "%s" % inStr
+    s2 = ""
     pos = 0
     matchobjects = CDATA_pattern_.finditer(s1)
     for mo in matchobjects:
-        s3 = s1[pos:mo.start()]
+        s3 = s1[pos : mo.start()]
         s2 += quote_xml_aux(s3)
-        s2 += s1[mo.start():mo.end()]
+        s2 += s1[mo.start() : mo.end()]
         pos = mo.end()
     s3 = s1[pos:]
     s2 += quote_xml_aux(s3)
     return s2
 
 
 def quote_xml_aux(inStr):
-    s1 = inStr.replace('&', '&amp;')
-    s1 = s1.replace('<', '&lt;')
-    s1 = s1.replace('>', '&gt;')
+    s1 = inStr.replace("&", "&amp;")
+    s1 = s1.replace("<", "&lt;")
+    s1 = s1.replace(">", "&gt;")
     return s1
 
 
 def quote_attrib(inStr):
-    s1 = (isinstance(inStr, BaseStrType_) and inStr or '%s' % inStr)
-    s1 = s1.replace('&', '&amp;')
-    s1 = s1.replace('<', '&lt;')
-    s1 = s1.replace('>', '&gt;')
+    s1 = isinstance(inStr, BaseStrType_) and inStr or "%s" % inStr
+    s1 = s1.replace("&", "&amp;")
+    s1 = s1.replace("<", "&lt;")
+    s1 = s1.replace(">", "&gt;")
+    s1 = s1.replace("\n", "&#10;")
     if '"' in s1:
         if "'" in s1:
             s1 = '"%s"' % s1.replace('"', "&quot;")
         else:
             s1 = "'%s'" % s1
     else:
         s1 = '"%s"' % s1
     return s1
 
 
 def quote_python(inStr):
     s1 = inStr
     if s1.find("'") == -1:
-        if s1.find('\n') == -1:
+        if s1.find("\n") == -1:
             return "'%s'" % s1
         else:
             return "'''%s'''" % s1
     else:
         if s1.find('"') != -1:
             s1 = s1.replace('"', '\\"')
-        if s1.find('\n') == -1:
+        if s1.find("\n") == -1:
             return '"%s"' % s1
         else:
             return '"""%s"""' % s1
 
 
 def get_all_text_(node):
     if node.text is not None:
         text = node.text
     else:
-        text = ''
+        text = ""
     for child in node:
         if child.tail is not None:
             text += child.tail
     return text
 
 
 def find_attr_value_(attr_name, node):
     attrs = node.attrib
-    attr_parts = attr_name.split(':')
+    attr_parts = attr_name.split(":")
     value = None
     if len(attr_parts) == 1:
         value = attrs.get(attr_name)
     elif len(attr_parts) == 2:
         prefix, name = attr_parts
-        namespace = node.nsmap.get(prefix)
+        if prefix == "xml":
+            namespace = "http://www.w3.org/XML/1998/namespace"
+        else:
+            namespace = node.nsmap.get(prefix)
         if namespace is not None:
-            value = attrs.get('{%s}%s' % (namespace, name, ))
+            value = attrs.get(
+                "{%s}%s"
+                % (
+                    namespace,
+                    name,
+                )
+            )
     return value
 
 
 def encode_str_2_3(instr):
     return instr
 
 
 class GDSParseError(Exception):
     pass
 
 
 def raise_parse_error(node, msg):
     if node is not None:
-        msg = '%s (element %s/line %d)' % (msg, node.tag, node.sourceline, )
+        msg = "%s (element %s/line %d)" % (
+            msg,
+            node.tag,
+            node.sourceline,
+        )
     raise GDSParseError(msg)
 
 
 class MixedContainer:
     # Constants for category:
     CategoryNone = 0
     CategoryText = 1
@@ -816,1648 +1018,2849 @@
     TypeString = 2
     TypeInteger = 3
     TypeFloat = 4
     TypeDecimal = 5
     TypeDouble = 6
     TypeBoolean = 7
     TypeBase64 = 8
+
     def __init__(self, category, content_type, name, value):
         self.category = category
         self.content_type = content_type
         self.name = name
         self.value = value
+
     def getCategory(self):
         return self.category
+
     def getContenttype(self, content_type):
         return self.content_type
+
     def getValue(self):
         return self.value
+
     def getName(self):
         return self.name
-    def export(self, outfile, level, name, namespace,
-               pretty_print=True):
+
+    def export(self, outfile, level, name, namespace, pretty_print=True):
         if self.category == MixedContainer.CategoryText:
             # Prevent exporting empty content as empty lines.
             if self.value.strip():
                 outfile.write(self.value)
         elif self.category == MixedContainer.CategorySimple:
             self.exportSimple(outfile, level, name)
-        else:    # category == MixedContainer.CategoryComplex
+        else:  # category == MixedContainer.CategoryComplex
             self.value.export(
-                outfile, level, namespace, name_=name,
-                pretty_print=pretty_print)
+                outfile,
+                level,
+                namespace,
+                name_=name,
+                pretty_print=pretty_print,
+            )
+
     def exportSimple(self, outfile, level, name):
         if self.content_type == MixedContainer.TypeString:
-            outfile.write('<%s>%s</%s>' % (
-                self.name, self.value, self.name))
-        elif self.content_type == MixedContainer.TypeInteger or \
-                self.content_type == MixedContainer.TypeBoolean:
-            outfile.write('<%s>%d</%s>' % (
-                self.name, self.value, self.name))
-        elif self.content_type == MixedContainer.TypeFloat or \
-                self.content_type == MixedContainer.TypeDecimal:
-            outfile.write('<%s>%f</%s>' % (
-                self.name, self.value, self.name))
+            outfile.write("<%s>%s</%s>" % (self.name, self.value, self.name))
+        elif (
+            self.content_type == MixedContainer.TypeInteger
+            or self.content_type == MixedContainer.TypeBoolean
+        ):
+            outfile.write("<%s>%d</%s>" % (self.name, self.value, self.name))
+        elif (
+            self.content_type == MixedContainer.TypeFloat
+            or self.content_type == MixedContainer.TypeDecimal
+        ):
+            outfile.write("<%s>%f</%s>" % (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeDouble:
-            outfile.write('<%s>%g</%s>' % (
-                self.name, self.value, self.name))
+            outfile.write("<%s>%g</%s>" % (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeBase64:
-            outfile.write('<%s>%s</%s>' % (
-                self.name,
-                base64.b64encode(self.value),
-                self.name))
-    def to_etree(self, element, mapping_=None, nsmap_=None):
+            outfile.write(
+                "<%s>%s</%s>"
+                % (self.name, base64.b64encode(self.value), self.name)
+            )
+
+    def to_etree(
+        self, element, mapping_=None, reverse_mapping_=None, nsmap_=None
+    ):
         if self.category == MixedContainer.CategoryText:
             # Prevent exporting empty content as empty lines.
             if self.value.strip():
                 if len(element) > 0:
                     if element[-1].tail is None:
                         element[-1].tail = self.value
                     else:
                         element[-1].tail += self.value
                 else:
                     if element.text is None:
                         element.text = self.value
                     else:
                         element.text += self.value
         elif self.category == MixedContainer.CategorySimple:
-            subelement = etree_.SubElement(
-                element, '%s' % self.name)
+            subelement = etree_.SubElement(element, "%s" % self.name)
             subelement.text = self.to_etree_simple()
-        else:    # category == MixedContainer.CategoryComplex
+        else:  # category == MixedContainer.CategoryComplex
             self.value.to_etree(element)
-    def to_etree_simple(self, mapping_=None, nsmap_=None):
+
+    def to_etree_simple(
+        self, mapping_=None, reverse_mapping_=None, nsmap_=None
+    ):
         if self.content_type == MixedContainer.TypeString:
             text = self.value
-        elif (self.content_type == MixedContainer.TypeInteger or
-                self.content_type == MixedContainer.TypeBoolean):
-            text = '%d' % self.value
-        elif (self.content_type == MixedContainer.TypeFloat or
-                self.content_type == MixedContainer.TypeDecimal):
-            text = '%f' % self.value
+        elif (
+            self.content_type == MixedContainer.TypeInteger
+            or self.content_type == MixedContainer.TypeBoolean
+        ):
+            text = "%d" % self.value
+        elif (
+            self.content_type == MixedContainer.TypeFloat
+            or self.content_type == MixedContainer.TypeDecimal
+        ):
+            text = "%f" % self.value
         elif self.content_type == MixedContainer.TypeDouble:
-            text = '%g' % self.value
+            text = "%g" % self.value
         elif self.content_type == MixedContainer.TypeBase64:
-            text = '%s' % base64.b64encode(self.value)
+            text = "%s" % base64.b64encode(self.value)
         return text
+
     def exportLiteral(self, outfile, level, name):
         if self.category == MixedContainer.CategoryText:
             showIndent(outfile, level)
             outfile.write(
-                'model_.MixedContainer(%d, %d, "%s", "%s"),\n' % (
-                    self.category, self.content_type,
-                    self.name, self.value))
+                'model_.MixedContainer(%d, %d, "%s", "%s"),\n'
+                % (self.category, self.content_type, self.name, self.value)
+            )
         elif self.category == MixedContainer.CategorySimple:
             showIndent(outfile, level)
             outfile.write(
-                'model_.MixedContainer(%d, %d, "%s", "%s"),\n' % (
-                    self.category, self.content_type,
-                    self.name, self.value))
-        else:    # category == MixedContainer.CategoryComplex
+                'model_.MixedContainer(%d, %d, "%s", "%s"),\n'
+                % (self.category, self.content_type, self.name, self.value)
+            )
+        else:  # category == MixedContainer.CategoryComplex
             showIndent(outfile, level)
             outfile.write(
-                'model_.MixedContainer(%d, %d, "%s",\n' % (
-                    self.category, self.content_type, self.name,))
+                'model_.MixedContainer(%d, %d, "%s",\n'
+                % (
+                    self.category,
+                    self.content_type,
+                    self.name,
+                )
+            )
             self.value.exportLiteral(outfile, level + 1)
             showIndent(outfile, level)
-            outfile.write(')\n')
+            outfile.write(")\n")
 
 
 class MemberSpec_(object):
-    def __init__(self, name='', data_type='', container=0,
-            optional=0, child_attrs=None, choice=None):
+    def __init__(
+        self,
+        name="",
+        data_type="",
+        container=0,
+        optional=0,
+        child_attrs=None,
+        choice=None,
+    ):
         self.name = name
         self.data_type = data_type
         self.container = container
         self.child_attrs = child_attrs
         self.choice = choice
         self.optional = optional
-    def set_name(self, name): self.name = name
-    def get_name(self): return self.name
-    def set_data_type(self, data_type): self.data_type = data_type
-    def get_data_type_chain(self): return self.data_type
+
+    def set_name(self, name):
+        self.name = name
+
+    def get_name(self):
+        return self.name
+
+    def set_data_type(self, data_type):
+        self.data_type = data_type
+
+    def get_data_type_chain(self):
+        return self.data_type
+
     def get_data_type(self):
         if isinstance(self.data_type, list):
             if len(self.data_type) > 0:
                 return self.data_type[-1]
             else:
-                return 'xs:string'
+                return "xs:string"
         else:
             return self.data_type
-    def set_container(self, container): self.container = container
-    def get_container(self): return self.container
-    def set_child_attrs(self, child_attrs): self.child_attrs = child_attrs
-    def get_child_attrs(self): return self.child_attrs
-    def set_choice(self, choice): self.choice = choice
-    def get_choice(self): return self.choice
-    def set_optional(self, optional): self.optional = optional
-    def get_optional(self): return self.optional
+
+    def set_container(self, container):
+        self.container = container
+
+    def get_container(self):
+        return self.container
+
+    def set_child_attrs(self, child_attrs):
+        self.child_attrs = child_attrs
+
+    def get_child_attrs(self):
+        return self.child_attrs
+
+    def set_choice(self, choice):
+        self.choice = choice
+
+    def get_choice(self):
+        return self.choice
+
+    def set_optional(self, optional):
+        self.optional = optional
+
+    def get_optional(self):
+        return self.optional
 
 
 def _cast(typ, value):
     if typ is None or value is None:
         return value
     return typ(value)
 
+
 #
 # Data representation classes.
 #
 
 
 class scpd(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, specVersion=None, actionList=None, serviceStateTable=None, gds_collector_=None, **kwargs_):
+
+    def __init__(
+        self,
+        specVersion=None,
+        actionList=None,
+        serviceStateTable=None,
+        gds_collector_=None,
+        **kwargs_
+    ):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
-        self.parent_object_ = kwargs_.get('parent_object_')
+        self.parent_object_ = kwargs_.get("parent_object_")
         self.ns_prefix_ = None
         self.specVersion = specVersion
         self.specVersion_nsprefix_ = None
         self.actionList = actionList
         self.actionList_nsprefix_ = None
         self.serviceStateTable = serviceStateTable
         self.serviceStateTable_nsprefix_ = None
+
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
-            subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, scpd)
+            subclass = getSubclassFromModule_(CurrentSubclassModule_, scpd)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
         if scpd.subclass:
             return scpd.subclass(*args_, **kwargs_)
         else:
             return scpd(*args_, **kwargs_)
+
     factory = staticmethod(factory)
+
     def get_ns_prefix_(self):
         return self.ns_prefix_
+
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
+
     def get_specVersion(self):
         return self.specVersion
+
     def set_specVersion(self, specVersion):
         self.specVersion = specVersion
+
     def get_actionList(self):
         return self.actionList
+
     def set_actionList(self, actionList):
         self.actionList = actionList
+
     def get_serviceStateTable(self):
         return self.serviceStateTable
+
     def set_serviceStateTable(self, serviceStateTable):
         self.serviceStateTable = serviceStateTable
-    def hasContent_(self):
+
+    def has__content(self):
         if (
-            self.specVersion is not None or
-            self.actionList is not None or
-            self.serviceStateTable is not None
+            self.specVersion is not None
+            or self.actionList is not None
+            or self.serviceStateTable is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ', name_='scpd', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('scpd')
+
+    def export(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ',
+        name_="scpd",
+        pretty_print=True,
+    ):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get("scpd")
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'scpd':
+            eol_ = ""
+        if self.original_tagname_ is not None and name_ == "scpd":
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
-            namespaceprefix_ = self.ns_prefix_ + ':'
+            namespaceprefix_ = self.ns_prefix_ + ":"
         showIndent(outfile, level, pretty_print)
-        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        outfile.write(
+            "<%s%s%s"
+            % (
+                namespaceprefix_,
+                name_,
+                namespacedef_ and " " + namespacedef_ or "",
+            )
+        )
         already_processed = set()
-        self.exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='scpd')
-        if self.hasContent_():
-            outfile.write('>%s' % (eol_, ))
-            self.exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='scpd', pretty_print=pretty_print)
+        self._exportAttributes(
+            outfile, level, already_processed, namespaceprefix_, name_="scpd"
+        )
+        if self.has__content():
+            outfile.write(">%s" % (eol_,))
+            self._exportChildren(
+                outfile,
+                level + 1,
+                namespaceprefix_,
+                namespacedef_,
+                name_="scpd",
+                pretty_print=pretty_print,
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+            outfile.write("</%s%s>%s" % (namespaceprefix_, name_, eol_))
         else:
-            outfile.write('/>%s' % (eol_, ))
-    def exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='scpd'):
-        pass
-    def exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ', name_='scpd', fromsubclass_=False, pretty_print=True):
+            outfile.write("/>%s" % (eol_,))
+
+    def _exportAttributes(
+        self,
+        outfile,
+        level,
+        already_processed,
+        namespaceprefix_="",
+        name_="scpd",
+    ):
+        pass
+
+    def _exportChildren(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ',
+        name_="scpd",
+        fromsubclass_=False,
+        pretty_print=True,
+    ):
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
+            eol_ = ""
         if self.specVersion is not None:
-            namespaceprefix_ = self.specVersion_nsprefix_ + ':' if (UseCapturedNS_ and self.specVersion_nsprefix_) else ''
-            self.specVersion.export(outfile, level, namespaceprefix_, namespacedef_='', name_='specVersion', pretty_print=pretty_print)
+            namespaceprefix_ = (
+                self.specVersion_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.specVersion_nsprefix_)
+                else ""
+            )
+            self.specVersion.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="specVersion",
+                pretty_print=pretty_print,
+            )
         if self.actionList is not None:
-            namespaceprefix_ = self.actionList_nsprefix_ + ':' if (UseCapturedNS_ and self.actionList_nsprefix_) else ''
-            self.actionList.export(outfile, level, namespaceprefix_, namespacedef_='', name_='actionList', pretty_print=pretty_print)
+            namespaceprefix_ = (
+                self.actionList_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.actionList_nsprefix_)
+                else ""
+            )
+            self.actionList.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="actionList",
+                pretty_print=pretty_print,
+            )
         if self.serviceStateTable is not None:
-            namespaceprefix_ = self.serviceStateTable_nsprefix_ + ':' if (UseCapturedNS_ and self.serviceStateTable_nsprefix_) else ''
-            self.serviceStateTable.export(outfile, level, namespaceprefix_, namespacedef_='', name_='serviceStateTable', pretty_print=pretty_print)
+            namespaceprefix_ = (
+                self.serviceStateTable_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.serviceStateTable_nsprefix_)
+                else ""
+            )
+            self.serviceStateTable.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="serviceStateTable",
+                pretty_print=pretty_print,
+            )
+
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
-        self.buildAttributes(node, node.attrib, already_processed)
+        self._buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
-            self.buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+            self._buildChildren(
+                child, node, nodeName_, gds_collector_=gds_collector_
+            )
         return self
-    def buildAttributes(self, node, attrs, already_processed):
+
+    def _buildAttributes(self, node, attrs, already_processed):
         pass
-    def buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
-        if nodeName_ == 'specVersion':
+
+    def _buildChildren(
+        self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
+    ):
+        if nodeName_ == "specVersion":
             obj_ = SpecVersionType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.specVersion = obj_
-            obj_.original_tagname_ = 'specVersion'
-        elif nodeName_ == 'actionList':
+            obj_.original_tagname_ = "specVersion"
+        elif nodeName_ == "actionList":
             obj_ = ActionListType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.actionList = obj_
-            obj_.original_tagname_ = 'actionList'
-        elif nodeName_ == 'serviceStateTable':
+            obj_.original_tagname_ = "actionList"
+        elif nodeName_ == "serviceStateTable":
             obj_ = ServiceStateTableType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.serviceStateTable = obj_
-            obj_.original_tagname_ = 'serviceStateTable'
+            obj_.original_tagname_ = "serviceStateTable"
+
+
 # end class scpd
 
 
 class SpecVersionType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
+
     def __init__(self, major=None, minor=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
-        self.parent_object_ = kwargs_.get('parent_object_')
+        self.parent_object_ = kwargs_.get("parent_object_")
         self.ns_prefix_ = None
         self.major = major
         self.major_nsprefix_ = None
         self.minor = minor
         self.minor_nsprefix_ = None
+
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, SpecVersionType)
+                CurrentSubclassModule_, SpecVersionType
+            )
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
         if SpecVersionType.subclass:
             return SpecVersionType.subclass(*args_, **kwargs_)
         else:
             return SpecVersionType(*args_, **kwargs_)
+
     factory = staticmethod(factory)
+
     def get_ns_prefix_(self):
         return self.ns_prefix_
+
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
+
     def get_major(self):
         return self.major
+
     def set_major(self, major):
         self.major = major
+
     def get_minor(self):
         return self.minor
+
     def set_minor(self, minor):
         self.minor = minor
-    def hasContent_(self):
-        if (
-            self.major is not None or
-            self.minor is not None
-        ):
+
+    def has__content(self):
+        if self.major is not None or self.minor is not None:
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ', name_='SpecVersionType', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('SpecVersionType')
+
+    def export(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ',
+        name_="SpecVersionType",
+        pretty_print=True,
+    ):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get("SpecVersionType")
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'SpecVersionType':
+            eol_ = ""
+        if self.original_tagname_ is not None and name_ == "SpecVersionType":
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
-            namespaceprefix_ = self.ns_prefix_ + ':'
+            namespaceprefix_ = self.ns_prefix_ + ":"
         showIndent(outfile, level, pretty_print)
-        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        outfile.write(
+            "<%s%s%s"
+            % (
+                namespaceprefix_,
+                name_,
+                namespacedef_ and " " + namespacedef_ or "",
+            )
+        )
         already_processed = set()
-        self.exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SpecVersionType')
-        if self.hasContent_():
-            outfile.write('>%s' % (eol_, ))
-            self.exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SpecVersionType', pretty_print=pretty_print)
+        self._exportAttributes(
+            outfile,
+            level,
+            already_processed,
+            namespaceprefix_,
+            name_="SpecVersionType",
+        )
+        if self.has__content():
+            outfile.write(">%s" % (eol_,))
+            self._exportChildren(
+                outfile,
+                level + 1,
+                namespaceprefix_,
+                namespacedef_,
+                name_="SpecVersionType",
+                pretty_print=pretty_print,
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+            outfile.write("</%s%s>%s" % (namespaceprefix_, name_, eol_))
         else:
-            outfile.write('/>%s' % (eol_, ))
-    def exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SpecVersionType'):
-        pass
-    def exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ', name_='SpecVersionType', fromsubclass_=False, pretty_print=True):
+            outfile.write("/>%s" % (eol_,))
+
+    def _exportAttributes(
+        self,
+        outfile,
+        level,
+        already_processed,
+        namespaceprefix_="",
+        name_="SpecVersionType",
+    ):
+        pass
+
+    def _exportChildren(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ',
+        name_="SpecVersionType",
+        fromsubclass_=False,
+        pretty_print=True,
+    ):
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
+            eol_ = ""
         if self.major is not None:
-            namespaceprefix_ = self.major_nsprefix_ + ':' if (UseCapturedNS_ and self.major_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.major_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.major_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%smajor>%s</%smajor>%s' % (namespaceprefix_ , self.gds_format_integer(self.major, input_name='major'), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%smajor>%s</%smajor>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_format_integer(self.major, input_name="major"),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.minor is not None:
-            namespaceprefix_ = self.minor_nsprefix_ + ':' if (UseCapturedNS_ and self.minor_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.minor_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.minor_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%sminor>%s</%sminor>%s' % (namespaceprefix_ , self.gds_format_integer(self.minor, input_name='minor'), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%sminor>%s</%sminor>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_format_integer(self.minor, input_name="minor"),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
+
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
-        self.buildAttributes(node, node.attrib, already_processed)
+        self._buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
-            self.buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+            self._buildChildren(
+                child, node, nodeName_, gds_collector_=gds_collector_
+            )
         return self
-    def buildAttributes(self, node, attrs, already_processed):
+
+    def _buildAttributes(self, node, attrs, already_processed):
         pass
-    def buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
-        if nodeName_ == 'major' and child_.text:
+
+    def _buildChildren(
+        self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
+    ):
+        if nodeName_ == "major" and child_.text:
             sval_ = child_.text
-            ival_ = self.gds_parse_integer(sval_, node, 'major')
-            ival_ = self.gds_validate_integer(ival_, node, 'major')
+            ival_ = self.gds_parse_integer(sval_, node, "major")
+            ival_ = self.gds_validate_integer(ival_, node, "major")
             self.major = ival_
             self.major_nsprefix_ = child_.prefix
-        elif nodeName_ == 'minor' and child_.text:
+        elif nodeName_ == "minor" and child_.text:
             sval_ = child_.text
-            ival_ = self.gds_parse_integer(sval_, node, 'minor')
-            ival_ = self.gds_validate_integer(ival_, node, 'minor')
+            ival_ = self.gds_parse_integer(sval_, node, "minor")
+            ival_ = self.gds_validate_integer(ival_, node, "minor")
             self.minor = ival_
             self.minor_nsprefix_ = child_.prefix
+
+
 # end class SpecVersionType
 
 
 class ActionListType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
+
     def __init__(self, action=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
-        self.parent_object_ = kwargs_.get('parent_object_')
+        self.parent_object_ = kwargs_.get("parent_object_")
         self.ns_prefix_ = None
         if action is None:
             self.action = []
         else:
             self.action = action
         self.action_nsprefix_ = None
+
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, ActionListType)
+                CurrentSubclassModule_, ActionListType
+            )
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
         if ActionListType.subclass:
             return ActionListType.subclass(*args_, **kwargs_)
         else:
             return ActionListType(*args_, **kwargs_)
+
     factory = staticmethod(factory)
+
     def get_ns_prefix_(self):
         return self.ns_prefix_
+
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
+
     def get_action(self):
         return self.action
+
     def set_action(self, action):
         self.action = action
+
     def add_action(self, value):
         self.action.append(value)
+
     def insert_action_at(self, index, value):
         self.action.insert(index, value)
+
     def replace_action_at(self, index, value):
         self.action[index] = value
-    def hasContent_(self):
-        if (
-            self.action
-        ):
+
+    def has__content(self):
+        if self.action:
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ', name_='ActionListType', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('ActionListType')
+
+    def export(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ',
+        name_="ActionListType",
+        pretty_print=True,
+    ):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get("ActionListType")
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'ActionListType':
+            eol_ = ""
+        if self.original_tagname_ is not None and name_ == "ActionListType":
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
-            namespaceprefix_ = self.ns_prefix_ + ':'
+            namespaceprefix_ = self.ns_prefix_ + ":"
         showIndent(outfile, level, pretty_print)
-        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        outfile.write(
+            "<%s%s%s"
+            % (
+                namespaceprefix_,
+                name_,
+                namespacedef_ and " " + namespacedef_ or "",
+            )
+        )
         already_processed = set()
-        self.exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ActionListType')
-        if self.hasContent_():
-            outfile.write('>%s' % (eol_, ))
-            self.exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ActionListType', pretty_print=pretty_print)
+        self._exportAttributes(
+            outfile,
+            level,
+            already_processed,
+            namespaceprefix_,
+            name_="ActionListType",
+        )
+        if self.has__content():
+            outfile.write(">%s" % (eol_,))
+            self._exportChildren(
+                outfile,
+                level + 1,
+                namespaceprefix_,
+                namespacedef_,
+                name_="ActionListType",
+                pretty_print=pretty_print,
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+            outfile.write("</%s%s>%s" % (namespaceprefix_, name_, eol_))
         else:
-            outfile.write('/>%s' % (eol_, ))
-    def exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ActionListType'):
-        pass
-    def exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ', name_='ActionListType', fromsubclass_=False, pretty_print=True):
+            outfile.write("/>%s" % (eol_,))
+
+    def _exportAttributes(
+        self,
+        outfile,
+        level,
+        already_processed,
+        namespaceprefix_="",
+        name_="ActionListType",
+    ):
+        pass
+
+    def _exportChildren(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ',
+        name_="ActionListType",
+        fromsubclass_=False,
+        pretty_print=True,
+    ):
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
+            eol_ = ""
         for action_ in self.action:
-            namespaceprefix_ = self.action_nsprefix_ + ':' if (UseCapturedNS_ and self.action_nsprefix_) else ''
-            action_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='action', pretty_print=pretty_print)
+            namespaceprefix_ = (
+                self.action_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.action_nsprefix_)
+                else ""
+            )
+            action_.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="action",
+                pretty_print=pretty_print,
+            )
+
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
-        self.buildAttributes(node, node.attrib, already_processed)
+        self._buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
-            self.buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+            self._buildChildren(
+                child, node, nodeName_, gds_collector_=gds_collector_
+            )
         return self
-    def buildAttributes(self, node, attrs, already_processed):
+
+    def _buildAttributes(self, node, attrs, already_processed):
         pass
-    def buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
-        if nodeName_ == 'action':
+
+    def _buildChildren(
+        self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
+    ):
+        if nodeName_ == "action":
             obj_ = ActionType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.action.append(obj_)
-            obj_.original_tagname_ = 'action'
+            obj_.original_tagname_ = "action"
+
+
 # end class ActionListType
 
 
 class ActionType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, name=None, argumentList=None, gds_collector_=None, **kwargs_):
+
+    def __init__(
+        self, name=None, argumentList=None, gds_collector_=None, **kwargs_
+    ):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
-        self.parent_object_ = kwargs_.get('parent_object_')
+        self.parent_object_ = kwargs_.get("parent_object_")
         self.ns_prefix_ = None
         self.name = name
         self.name_nsprefix_ = None
         self.argumentList = argumentList
         self.argumentList_nsprefix_ = None
+
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, ActionType)
+                CurrentSubclassModule_, ActionType
+            )
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
         if ActionType.subclass:
             return ActionType.subclass(*args_, **kwargs_)
         else:
             return ActionType(*args_, **kwargs_)
+
     factory = staticmethod(factory)
+
     def get_ns_prefix_(self):
         return self.ns_prefix_
+
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
+
     def get_name(self):
         return self.name
+
     def set_name(self, name):
         self.name = name
+
     def get_argumentList(self):
         return self.argumentList
+
     def set_argumentList(self, argumentList):
         self.argumentList = argumentList
-    def hasContent_(self):
-        if (
-            self.name is not None or
-            self.argumentList is not None
-        ):
+
+    def has__content(self):
+        if self.name is not None or self.argumentList is not None:
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ', name_='ActionType', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('ActionType')
+
+    def export(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ',
+        name_="ActionType",
+        pretty_print=True,
+    ):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get("ActionType")
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'ActionType':
+            eol_ = ""
+        if self.original_tagname_ is not None and name_ == "ActionType":
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
-            namespaceprefix_ = self.ns_prefix_ + ':'
+            namespaceprefix_ = self.ns_prefix_ + ":"
         showIndent(outfile, level, pretty_print)
-        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        outfile.write(
+            "<%s%s%s"
+            % (
+                namespaceprefix_,
+                name_,
+                namespacedef_ and " " + namespacedef_ or "",
+            )
+        )
         already_processed = set()
-        self.exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ActionType')
-        if self.hasContent_():
-            outfile.write('>%s' % (eol_, ))
-            self.exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ActionType', pretty_print=pretty_print)
+        self._exportAttributes(
+            outfile,
+            level,
+            already_processed,
+            namespaceprefix_,
+            name_="ActionType",
+        )
+        if self.has__content():
+            outfile.write(">%s" % (eol_,))
+            self._exportChildren(
+                outfile,
+                level + 1,
+                namespaceprefix_,
+                namespacedef_,
+                name_="ActionType",
+                pretty_print=pretty_print,
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+            outfile.write("</%s%s>%s" % (namespaceprefix_, name_, eol_))
         else:
-            outfile.write('/>%s' % (eol_, ))
-    def exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ActionType'):
-        pass
-    def exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ', name_='ActionType', fromsubclass_=False, pretty_print=True):
+            outfile.write("/>%s" % (eol_,))
+
+    def _exportAttributes(
+        self,
+        outfile,
+        level,
+        already_processed,
+        namespaceprefix_="",
+        name_="ActionType",
+    ):
+        pass
+
+    def _exportChildren(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ',
+        name_="ActionType",
+        fromsubclass_=False,
+        pretty_print=True,
+    ):
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
+            eol_ = ""
         if self.name is not None:
-            namespaceprefix_ = self.name_nsprefix_ + ':' if (UseCapturedNS_ and self.name_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.name_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.name_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%sname>%s</%sname>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.name), input_name='name')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%sname>%s</%sname>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(self.name), input_name="name"
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.argumentList is not None:
-            namespaceprefix_ = self.argumentList_nsprefix_ + ':' if (UseCapturedNS_ and self.argumentList_nsprefix_) else ''
-            self.argumentList.export(outfile, level, namespaceprefix_, namespacedef_='', name_='argumentList', pretty_print=pretty_print)
+            namespaceprefix_ = (
+                self.argumentList_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.argumentList_nsprefix_)
+                else ""
+            )
+            self.argumentList.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="argumentList",
+                pretty_print=pretty_print,
+            )
+
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
-        self.buildAttributes(node, node.attrib, already_processed)
+        self._buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
-            self.buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+            self._buildChildren(
+                child, node, nodeName_, gds_collector_=gds_collector_
+            )
         return self
-    def buildAttributes(self, node, attrs, already_processed):
+
+    def _buildAttributes(self, node, attrs, already_processed):
         pass
-    def buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
-        if nodeName_ == 'name':
+
+    def _buildChildren(
+        self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
+    ):
+        if nodeName_ == "name":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'name')
-            value_ = self.gds_validate_string(value_, node, 'name')
+            value_ = self.gds_parse_string(value_, node, "name")
+            value_ = self.gds_validate_string(value_, node, "name")
             self.name = value_
             self.name_nsprefix_ = child_.prefix
-        elif nodeName_ == 'argumentList':
+        elif nodeName_ == "argumentList":
             obj_ = ArgumentListType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.argumentList = obj_
-            obj_.original_tagname_ = 'argumentList'
+            obj_.original_tagname_ = "argumentList"
+
+
 # end class ActionType
 
 
 class ArgumentListType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
+
     def __init__(self, argument=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
-        self.parent_object_ = kwargs_.get('parent_object_')
+        self.parent_object_ = kwargs_.get("parent_object_")
         self.ns_prefix_ = None
         if argument is None:
             self.argument = []
         else:
             self.argument = argument
         self.argument_nsprefix_ = None
+
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, ArgumentListType)
+                CurrentSubclassModule_, ArgumentListType
+            )
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
         if ArgumentListType.subclass:
             return ArgumentListType.subclass(*args_, **kwargs_)
         else:
             return ArgumentListType(*args_, **kwargs_)
+
     factory = staticmethod(factory)
+
     def get_ns_prefix_(self):
         return self.ns_prefix_
+
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
+
     def get_argument(self):
         return self.argument
+
     def set_argument(self, argument):
         self.argument = argument
+
     def add_argument(self, value):
         self.argument.append(value)
+
     def insert_argument_at(self, index, value):
         self.argument.insert(index, value)
+
     def replace_argument_at(self, index, value):
         self.argument[index] = value
-    def hasContent_(self):
-        if (
-            self.argument
-        ):
+
+    def has__content(self):
+        if self.argument:
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ', name_='ArgumentListType', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('ArgumentListType')
+
+    def export(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ',
+        name_="ArgumentListType",
+        pretty_print=True,
+    ):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get("ArgumentListType")
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'ArgumentListType':
+            eol_ = ""
+        if self.original_tagname_ is not None and name_ == "ArgumentListType":
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
-            namespaceprefix_ = self.ns_prefix_ + ':'
+            namespaceprefix_ = self.ns_prefix_ + ":"
         showIndent(outfile, level, pretty_print)
-        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        outfile.write(
+            "<%s%s%s"
+            % (
+                namespaceprefix_,
+                name_,
+                namespacedef_ and " " + namespacedef_ or "",
+            )
+        )
         already_processed = set()
-        self.exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ArgumentListType')
-        if self.hasContent_():
-            outfile.write('>%s' % (eol_, ))
-            self.exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ArgumentListType', pretty_print=pretty_print)
+        self._exportAttributes(
+            outfile,
+            level,
+            already_processed,
+            namespaceprefix_,
+            name_="ArgumentListType",
+        )
+        if self.has__content():
+            outfile.write(">%s" % (eol_,))
+            self._exportChildren(
+                outfile,
+                level + 1,
+                namespaceprefix_,
+                namespacedef_,
+                name_="ArgumentListType",
+                pretty_print=pretty_print,
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+            outfile.write("</%s%s>%s" % (namespaceprefix_, name_, eol_))
         else:
-            outfile.write('/>%s' % (eol_, ))
-    def exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ArgumentListType'):
-        pass
-    def exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ', name_='ArgumentListType', fromsubclass_=False, pretty_print=True):
+            outfile.write("/>%s" % (eol_,))
+
+    def _exportAttributes(
+        self,
+        outfile,
+        level,
+        already_processed,
+        namespaceprefix_="",
+        name_="ArgumentListType",
+    ):
+        pass
+
+    def _exportChildren(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ',
+        name_="ArgumentListType",
+        fromsubclass_=False,
+        pretty_print=True,
+    ):
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
+            eol_ = ""
         for argument_ in self.argument:
-            namespaceprefix_ = self.argument_nsprefix_ + ':' if (UseCapturedNS_ and self.argument_nsprefix_) else ''
-            argument_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='argument', pretty_print=pretty_print)
+            namespaceprefix_ = (
+                self.argument_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.argument_nsprefix_)
+                else ""
+            )
+            argument_.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="argument",
+                pretty_print=pretty_print,
+            )
+
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
-        self.buildAttributes(node, node.attrib, already_processed)
+        self._buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
-            self.buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+            self._buildChildren(
+                child, node, nodeName_, gds_collector_=gds_collector_
+            )
         return self
-    def buildAttributes(self, node, attrs, already_processed):
+
+    def _buildAttributes(self, node, attrs, already_processed):
         pass
-    def buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
-        if nodeName_ == 'argument':
+
+    def _buildChildren(
+        self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
+    ):
+        if nodeName_ == "argument":
             obj_ = ArgumentType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.argument.append(obj_)
-            obj_.original_tagname_ = 'argument'
+            obj_.original_tagname_ = "argument"
+
+
 # end class ArgumentListType
 
 
 class ArgumentType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, name=None, direction=None, relatedStateVariable=None, retval=None, gds_collector_=None, **kwargs_):
+
+    def __init__(
+        self,
+        name=None,
+        direction=None,
+        relatedStateVariable=None,
+        retval=None,
+        gds_collector_=None,
+        **kwargs_
+    ):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
-        self.parent_object_ = kwargs_.get('parent_object_')
+        self.parent_object_ = kwargs_.get("parent_object_")
         self.ns_prefix_ = None
         self.name = name
         self.name_nsprefix_ = None
         self.direction = direction
         self.direction_nsprefix_ = None
         self.relatedStateVariable = relatedStateVariable
         self.relatedStateVariable_nsprefix_ = None
         self.retval = retval
         self.retval_nsprefix_ = None
+
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, ArgumentType)
+                CurrentSubclassModule_, ArgumentType
+            )
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
         if ArgumentType.subclass:
             return ArgumentType.subclass(*args_, **kwargs_)
         else:
             return ArgumentType(*args_, **kwargs_)
+
     factory = staticmethod(factory)
+
     def get_ns_prefix_(self):
         return self.ns_prefix_
+
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
+
     def get_name(self):
         return self.name
+
     def set_name(self, name):
         self.name = name
+
     def get_direction(self):
         return self.direction
+
     def set_direction(self, direction):
         self.direction = direction
+
     def get_relatedStateVariable(self):
         return self.relatedStateVariable
+
     def set_relatedStateVariable(self, relatedStateVariable):
         self.relatedStateVariable = relatedStateVariable
+
     def get_retval(self):
         return self.retval
+
     def set_retval(self, retval):
         self.retval = retval
-    def hasContent_(self):
+
+    def has__content(self):
         if (
-            self.name is not None or
-            self.direction is not None or
-            self.relatedStateVariable is not None or
-            self.retval is not None
+            self.name is not None
+            or self.direction is not None
+            or self.relatedStateVariable is not None
+            or self.retval is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ', name_='ArgumentType', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('ArgumentType')
+
+    def export(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ',
+        name_="ArgumentType",
+        pretty_print=True,
+    ):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get("ArgumentType")
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'ArgumentType':
+            eol_ = ""
+        if self.original_tagname_ is not None and name_ == "ArgumentType":
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
-            namespaceprefix_ = self.ns_prefix_ + ':'
+            namespaceprefix_ = self.ns_prefix_ + ":"
         showIndent(outfile, level, pretty_print)
-        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        outfile.write(
+            "<%s%s%s"
+            % (
+                namespaceprefix_,
+                name_,
+                namespacedef_ and " " + namespacedef_ or "",
+            )
+        )
         already_processed = set()
-        self.exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ArgumentType')
-        if self.hasContent_():
-            outfile.write('>%s' % (eol_, ))
-            self.exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ArgumentType', pretty_print=pretty_print)
+        self._exportAttributes(
+            outfile,
+            level,
+            already_processed,
+            namespaceprefix_,
+            name_="ArgumentType",
+        )
+        if self.has__content():
+            outfile.write(">%s" % (eol_,))
+            self._exportChildren(
+                outfile,
+                level + 1,
+                namespaceprefix_,
+                namespacedef_,
+                name_="ArgumentType",
+                pretty_print=pretty_print,
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+            outfile.write("</%s%s>%s" % (namespaceprefix_, name_, eol_))
         else:
-            outfile.write('/>%s' % (eol_, ))
-    def exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ArgumentType'):
-        pass
-    def exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ', name_='ArgumentType', fromsubclass_=False, pretty_print=True):
+            outfile.write("/>%s" % (eol_,))
+
+    def _exportAttributes(
+        self,
+        outfile,
+        level,
+        already_processed,
+        namespaceprefix_="",
+        name_="ArgumentType",
+    ):
+        pass
+
+    def _exportChildren(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ',
+        name_="ArgumentType",
+        fromsubclass_=False,
+        pretty_print=True,
+    ):
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
+            eol_ = ""
         if self.name is not None:
-            namespaceprefix_ = self.name_nsprefix_ + ':' if (UseCapturedNS_ and self.name_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.name_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.name_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%sname>%s</%sname>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.name), input_name='name')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%sname>%s</%sname>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(self.name), input_name="name"
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.direction is not None:
-            namespaceprefix_ = self.direction_nsprefix_ + ':' if (UseCapturedNS_ and self.direction_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.direction_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.direction_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%sdirection>%s</%sdirection>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.direction), input_name='direction')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%sdirection>%s</%sdirection>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(self.direction), input_name="direction"
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.relatedStateVariable is not None:
-            namespaceprefix_ = self.relatedStateVariable_nsprefix_ + ':' if (UseCapturedNS_ and self.relatedStateVariable_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.relatedStateVariable_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.relatedStateVariable_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%srelatedStateVariable>%s</%srelatedStateVariable>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.relatedStateVariable), input_name='relatedStateVariable')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%srelatedStateVariable>%s</%srelatedStateVariable>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(self.relatedStateVariable),
+                            input_name="relatedStateVariable",
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.retval is not None:
-            namespaceprefix_ = self.retval_nsprefix_ + ':' if (UseCapturedNS_ and self.retval_nsprefix_) else ''
-            self.retval.export(outfile, level, namespaceprefix_, namespacedef_='', name_='retval', pretty_print=pretty_print)
+            namespaceprefix_ = (
+                self.retval_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.retval_nsprefix_)
+                else ""
+            )
+            self.retval.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="retval",
+                pretty_print=pretty_print,
+            )
+
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
-        self.buildAttributes(node, node.attrib, already_processed)
+        self._buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
-            self.buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+            self._buildChildren(
+                child, node, nodeName_, gds_collector_=gds_collector_
+            )
         return self
-    def buildAttributes(self, node, attrs, already_processed):
+
+    def _buildAttributes(self, node, attrs, already_processed):
         pass
-    def buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
-        if nodeName_ == 'name':
+
+    def _buildChildren(
+        self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
+    ):
+        if nodeName_ == "name":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'name')
-            value_ = self.gds_validate_string(value_, node, 'name')
+            value_ = self.gds_parse_string(value_, node, "name")
+            value_ = self.gds_validate_string(value_, node, "name")
             self.name = value_
             self.name_nsprefix_ = child_.prefix
-        elif nodeName_ == 'direction':
+        elif nodeName_ == "direction":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'direction')
-            value_ = self.gds_validate_string(value_, node, 'direction')
+            value_ = self.gds_parse_string(value_, node, "direction")
+            value_ = self.gds_validate_string(value_, node, "direction")
             self.direction = value_
             self.direction_nsprefix_ = child_.prefix
-        elif nodeName_ == 'relatedStateVariable':
+        elif nodeName_ == "relatedStateVariable":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'relatedStateVariable')
-            value_ = self.gds_validate_string(value_, node, 'relatedStateVariable')
+            value_ = self.gds_parse_string(
+                value_, node, "relatedStateVariable"
+            )
+            value_ = self.gds_validate_string(
+                value_, node, "relatedStateVariable"
+            )
             self.relatedStateVariable = value_
             self.relatedStateVariable_nsprefix_ = child_.prefix
-        elif nodeName_ == 'retval':
+        elif nodeName_ == "retval":
             obj_ = retvalType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.retval = obj_
-            obj_.original_tagname_ = 'retval'
+            obj_.original_tagname_ = "retval"
+
+
 # end class ArgumentType
 
 
 class ServiceStateTableType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
+
     def __init__(self, stateVariable=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
-        self.parent_object_ = kwargs_.get('parent_object_')
+        self.parent_object_ = kwargs_.get("parent_object_")
         self.ns_prefix_ = None
         if stateVariable is None:
             self.stateVariable = []
         else:
             self.stateVariable = stateVariable
         self.stateVariable_nsprefix_ = None
+
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, ServiceStateTableType)
+                CurrentSubclassModule_, ServiceStateTableType
+            )
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
         if ServiceStateTableType.subclass:
             return ServiceStateTableType.subclass(*args_, **kwargs_)
         else:
             return ServiceStateTableType(*args_, **kwargs_)
+
     factory = staticmethod(factory)
+
     def get_ns_prefix_(self):
         return self.ns_prefix_
+
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
+
     def get_stateVariable(self):
         return self.stateVariable
+
     def set_stateVariable(self, stateVariable):
         self.stateVariable = stateVariable
+
     def add_stateVariable(self, value):
         self.stateVariable.append(value)
+
     def insert_stateVariable_at(self, index, value):
         self.stateVariable.insert(index, value)
+
     def replace_stateVariable_at(self, index, value):
         self.stateVariable[index] = value
-    def hasContent_(self):
-        if (
-            self.stateVariable
-        ):
+
+    def has__content(self):
+        if self.stateVariable:
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ', name_='ServiceStateTableType', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('ServiceStateTableType')
+
+    def export(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ',
+        name_="ServiceStateTableType",
+        pretty_print=True,
+    ):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get(
+            "ServiceStateTableType"
+        )
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'ServiceStateTableType':
+            eol_ = ""
+        if (
+            self.original_tagname_ is not None
+            and name_ == "ServiceStateTableType"
+        ):
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
-            namespaceprefix_ = self.ns_prefix_ + ':'
+            namespaceprefix_ = self.ns_prefix_ + ":"
         showIndent(outfile, level, pretty_print)
-        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        outfile.write(
+            "<%s%s%s"
+            % (
+                namespaceprefix_,
+                name_,
+                namespacedef_ and " " + namespacedef_ or "",
+            )
+        )
         already_processed = set()
-        self.exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ServiceStateTableType')
-        if self.hasContent_():
-            outfile.write('>%s' % (eol_, ))
-            self.exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ServiceStateTableType', pretty_print=pretty_print)
+        self._exportAttributes(
+            outfile,
+            level,
+            already_processed,
+            namespaceprefix_,
+            name_="ServiceStateTableType",
+        )
+        if self.has__content():
+            outfile.write(">%s" % (eol_,))
+            self._exportChildren(
+                outfile,
+                level + 1,
+                namespaceprefix_,
+                namespacedef_,
+                name_="ServiceStateTableType",
+                pretty_print=pretty_print,
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+            outfile.write("</%s%s>%s" % (namespaceprefix_, name_, eol_))
         else:
-            outfile.write('/>%s' % (eol_, ))
-    def exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ServiceStateTableType'):
-        pass
-    def exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ', name_='ServiceStateTableType', fromsubclass_=False, pretty_print=True):
+            outfile.write("/>%s" % (eol_,))
+
+    def _exportAttributes(
+        self,
+        outfile,
+        level,
+        already_processed,
+        namespaceprefix_="",
+        name_="ServiceStateTableType",
+    ):
+        pass
+
+    def _exportChildren(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ',
+        name_="ServiceStateTableType",
+        fromsubclass_=False,
+        pretty_print=True,
+    ):
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
+            eol_ = ""
         for stateVariable_ in self.stateVariable:
-            namespaceprefix_ = self.stateVariable_nsprefix_ + ':' if (UseCapturedNS_ and self.stateVariable_nsprefix_) else ''
-            stateVariable_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='stateVariable', pretty_print=pretty_print)
+            namespaceprefix_ = (
+                self.stateVariable_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.stateVariable_nsprefix_)
+                else ""
+            )
+            stateVariable_.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="stateVariable",
+                pretty_print=pretty_print,
+            )
+
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
-        self.buildAttributes(node, node.attrib, already_processed)
+        self._buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
-            self.buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+            self._buildChildren(
+                child, node, nodeName_, gds_collector_=gds_collector_
+            )
         return self
-    def buildAttributes(self, node, attrs, already_processed):
+
+    def _buildAttributes(self, node, attrs, already_processed):
         pass
-    def buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
-        if nodeName_ == 'stateVariable':
+
+    def _buildChildren(
+        self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
+    ):
+        if nodeName_ == "stateVariable":
             obj_ = StateVariableType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.stateVariable.append(obj_)
-            obj_.original_tagname_ = 'stateVariable'
+            obj_.original_tagname_ = "stateVariable"
+
+
 # end class ServiceStateTableType
 
 
 class StateVariableType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, sendEvents='yes', name=None, dataType=None, defaultValue=None, allowedValueList=None, allowedValueRange=None, gds_collector_=None, **kwargs_):
+
+    def __init__(
+        self,
+        sendEvents="yes",
+        name=None,
+        dataType=None,
+        defaultValue=None,
+        allowedValueList=None,
+        allowedValueRange=None,
+        gds_collector_=None,
+        **kwargs_
+    ):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
-        self.parent_object_ = kwargs_.get('parent_object_')
+        self.parent_object_ = kwargs_.get("parent_object_")
         self.ns_prefix_ = None
         self.sendEvents = _cast(None, sendEvents)
         self.sendEvents_nsprefix_ = None
         self.name = name
         self.name_nsprefix_ = None
         self.dataType = dataType
         self.dataType_nsprefix_ = None
         self.defaultValue = defaultValue
         self.defaultValue_nsprefix_ = None
         self.allowedValueList = allowedValueList
         self.allowedValueList_nsprefix_ = None
         self.allowedValueRange = allowedValueRange
         self.allowedValueRange_nsprefix_ = None
+
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, StateVariableType)
+                CurrentSubclassModule_, StateVariableType
+            )
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
         if StateVariableType.subclass:
             return StateVariableType.subclass(*args_, **kwargs_)
         else:
             return StateVariableType(*args_, **kwargs_)
+
     factory = staticmethod(factory)
+
     def get_ns_prefix_(self):
         return self.ns_prefix_
+
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
+
     def get_name(self):
         return self.name
+
     def set_name(self, name):
         self.name = name
+
     def get_dataType(self):
         return self.dataType
+
     def set_dataType(self, dataType):
         self.dataType = dataType
+
     def get_defaultValue(self):
         return self.defaultValue
+
     def set_defaultValue(self, defaultValue):
         self.defaultValue = defaultValue
+
     def get_allowedValueList(self):
         return self.allowedValueList
+
     def set_allowedValueList(self, allowedValueList):
         self.allowedValueList = allowedValueList
+
     def get_allowedValueRange(self):
         return self.allowedValueRange
+
     def set_allowedValueRange(self, allowedValueRange):
         self.allowedValueRange = allowedValueRange
+
     def get_sendEvents(self):
         return self.sendEvents
+
     def set_sendEvents(self, sendEvents):
         self.sendEvents = sendEvents
-    def hasContent_(self):
+
+    def has__content(self):
         if (
-            self.name is not None or
-            self.dataType is not None or
-            self.defaultValue is not None or
-            self.allowedValueList is not None or
-            self.allowedValueRange is not None
+            self.name is not None
+            or self.dataType is not None
+            or self.defaultValue is not None
+            or self.allowedValueList is not None
+            or self.allowedValueRange is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ', name_='StateVariableType', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('StateVariableType')
+
+    def export(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ',
+        name_="StateVariableType",
+        pretty_print=True,
+    ):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get("StateVariableType")
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'StateVariableType':
+            eol_ = ""
+        if self.original_tagname_ is not None and name_ == "StateVariableType":
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
-            namespaceprefix_ = self.ns_prefix_ + ':'
+            namespaceprefix_ = self.ns_prefix_ + ":"
         showIndent(outfile, level, pretty_print)
-        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        outfile.write(
+            "<%s%s%s"
+            % (
+                namespaceprefix_,
+                name_,
+                namespacedef_ and " " + namespacedef_ or "",
+            )
+        )
         already_processed = set()
-        self.exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='StateVariableType')
-        if self.hasContent_():
-            outfile.write('>%s' % (eol_, ))
-            self.exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='StateVariableType', pretty_print=pretty_print)
+        self._exportAttributes(
+            outfile,
+            level,
+            already_processed,
+            namespaceprefix_,
+            name_="StateVariableType",
+        )
+        if self.has__content():
+            outfile.write(">%s" % (eol_,))
+            self._exportChildren(
+                outfile,
+                level + 1,
+                namespaceprefix_,
+                namespacedef_,
+                name_="StateVariableType",
+                pretty_print=pretty_print,
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+            outfile.write("</%s%s>%s" % (namespaceprefix_, name_, eol_))
         else:
-            outfile.write('/>%s' % (eol_, ))
-    def exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='StateVariableType'):
-        if self.sendEvents != "yes" and 'sendEvents' not in already_processed:
-            already_processed.add('sendEvents')
-            outfile.write(' sendEvents=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.sendEvents), input_name='sendEvents')), ))
-    def exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ', name_='StateVariableType', fromsubclass_=False, pretty_print=True):
+            outfile.write("/>%s" % (eol_,))
+
+    def _exportAttributes(
+        self,
+        outfile,
+        level,
+        already_processed,
+        namespaceprefix_="",
+        name_="StateVariableType",
+    ):
+        if self.sendEvents != "yes" and "sendEvents" not in already_processed:
+            already_processed.add("sendEvents")
+            outfile.write(
+                " sendEvents=%s"
+                % (
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_attrib(self.sendEvents),
+                            input_name="sendEvents",
+                        )
+                    ),
+                )
+            )
+
+    def _exportChildren(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ',
+        name_="StateVariableType",
+        fromsubclass_=False,
+        pretty_print=True,
+    ):
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
+            eol_ = ""
         if self.name is not None:
-            namespaceprefix_ = self.name_nsprefix_ + ':' if (UseCapturedNS_ and self.name_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.name_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.name_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%sname>%s</%sname>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.name), input_name='name')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%sname>%s</%sname>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(self.name), input_name="name"
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.dataType is not None:
-            namespaceprefix_ = self.dataType_nsprefix_ + ':' if (UseCapturedNS_ and self.dataType_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.dataType_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.dataType_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%sdataType>%s</%sdataType>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.dataType), input_name='dataType')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%sdataType>%s</%sdataType>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(self.dataType), input_name="dataType"
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.defaultValue is not None:
-            namespaceprefix_ = self.defaultValue_nsprefix_ + ':' if (UseCapturedNS_ and self.defaultValue_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.defaultValue_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.defaultValue_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%sdefaultValue>%s</%sdefaultValue>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.defaultValue), input_name='defaultValue')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%sdefaultValue>%s</%sdefaultValue>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(self.defaultValue),
+                            input_name="defaultValue",
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.allowedValueList is not None:
-            namespaceprefix_ = self.allowedValueList_nsprefix_ + ':' if (UseCapturedNS_ and self.allowedValueList_nsprefix_) else ''
-            self.allowedValueList.export(outfile, level, namespaceprefix_, namespacedef_='', name_='allowedValueList', pretty_print=pretty_print)
+            namespaceprefix_ = (
+                self.allowedValueList_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.allowedValueList_nsprefix_)
+                else ""
+            )
+            self.allowedValueList.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="allowedValueList",
+                pretty_print=pretty_print,
+            )
         if self.allowedValueRange is not None:
-            namespaceprefix_ = self.allowedValueRange_nsprefix_ + ':' if (UseCapturedNS_ and self.allowedValueRange_nsprefix_) else ''
-            self.allowedValueRange.export(outfile, level, namespaceprefix_, namespacedef_='', name_='allowedValueRange', pretty_print=pretty_print)
+            namespaceprefix_ = (
+                self.allowedValueRange_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.allowedValueRange_nsprefix_)
+                else ""
+            )
+            self.allowedValueRange.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="allowedValueRange",
+                pretty_print=pretty_print,
+            )
+
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
-        self.buildAttributes(node, node.attrib, already_processed)
+        self._buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
-            self.buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+            self._buildChildren(
+                child, node, nodeName_, gds_collector_=gds_collector_
+            )
         return self
-    def buildAttributes(self, node, attrs, already_processed):
-        value = find_attr_value_('sendEvents', node)
-        if value is not None and 'sendEvents' not in already_processed:
-            already_processed.add('sendEvents')
+
+    def _buildAttributes(self, node, attrs, already_processed):
+        value = find_attr_value_("sendEvents", node)
+        if value is not None and "sendEvents" not in already_processed:
+            already_processed.add("sendEvents")
             self.sendEvents = value
-    def buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
-        if nodeName_ == 'name':
+
+    def _buildChildren(
+        self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
+    ):
+        if nodeName_ == "name":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'name')
-            value_ = self.gds_validate_string(value_, node, 'name')
+            value_ = self.gds_parse_string(value_, node, "name")
+            value_ = self.gds_validate_string(value_, node, "name")
             self.name = value_
             self.name_nsprefix_ = child_.prefix
-        elif nodeName_ == 'dataType':
+        elif nodeName_ == "dataType":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'dataType')
-            value_ = self.gds_validate_string(value_, node, 'dataType')
+            value_ = self.gds_parse_string(value_, node, "dataType")
+            value_ = self.gds_validate_string(value_, node, "dataType")
             self.dataType = value_
             self.dataType_nsprefix_ = child_.prefix
-        elif nodeName_ == 'defaultValue':
+        elif nodeName_ == "defaultValue":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'defaultValue')
-            value_ = self.gds_validate_string(value_, node, 'defaultValue')
+            value_ = self.gds_parse_string(value_, node, "defaultValue")
+            value_ = self.gds_validate_string(value_, node, "defaultValue")
             self.defaultValue = value_
             self.defaultValue_nsprefix_ = child_.prefix
-        elif nodeName_ == 'allowedValueList':
+        elif nodeName_ == "allowedValueList":
             obj_ = AllowedValueListType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.allowedValueList = obj_
-            obj_.original_tagname_ = 'allowedValueList'
-        elif nodeName_ == 'allowedValueRange':
+            obj_.original_tagname_ = "allowedValueList"
+        elif nodeName_ == "allowedValueRange":
             obj_ = AllowedValueRangeType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.allowedValueRange = obj_
-            obj_.original_tagname_ = 'allowedValueRange'
+            obj_.original_tagname_ = "allowedValueRange"
+
+
 # end class StateVariableType
 
 
 class AllowedValueListType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
+
     def __init__(self, allowedValue=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
-        self.parent_object_ = kwargs_.get('parent_object_')
+        self.parent_object_ = kwargs_.get("parent_object_")
         self.ns_prefix_ = None
         if allowedValue is None:
             self.allowedValue = []
         else:
             self.allowedValue = allowedValue
         self.allowedValue_nsprefix_ = None
+
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, AllowedValueListType)
+                CurrentSubclassModule_, AllowedValueListType
+            )
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
         if AllowedValueListType.subclass:
             return AllowedValueListType.subclass(*args_, **kwargs_)
         else:
             return AllowedValueListType(*args_, **kwargs_)
+
     factory = staticmethod(factory)
+
     def get_ns_prefix_(self):
         return self.ns_prefix_
+
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
+
     def get_allowedValue(self):
         return self.allowedValue
+
     def set_allowedValue(self, allowedValue):
         self.allowedValue = allowedValue
+
     def add_allowedValue(self, value):
         self.allowedValue.append(value)
+
     def insert_allowedValue_at(self, index, value):
         self.allowedValue.insert(index, value)
+
     def replace_allowedValue_at(self, index, value):
         self.allowedValue[index] = value
-    def hasContent_(self):
-        if (
-            self.allowedValue
-        ):
+
+    def has__content(self):
+        if self.allowedValue:
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ', name_='AllowedValueListType', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('AllowedValueListType')
+
+    def export(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ',
+        name_="AllowedValueListType",
+        pretty_print=True,
+    ):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get("AllowedValueListType")
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'AllowedValueListType':
+            eol_ = ""
+        if (
+            self.original_tagname_ is not None
+            and name_ == "AllowedValueListType"
+        ):
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
-            namespaceprefix_ = self.ns_prefix_ + ':'
+            namespaceprefix_ = self.ns_prefix_ + ":"
         showIndent(outfile, level, pretty_print)
-        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        outfile.write(
+            "<%s%s%s"
+            % (
+                namespaceprefix_,
+                name_,
+                namespacedef_ and " " + namespacedef_ or "",
+            )
+        )
         already_processed = set()
-        self.exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='AllowedValueListType')
-        if self.hasContent_():
-            outfile.write('>%s' % (eol_, ))
-            self.exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='AllowedValueListType', pretty_print=pretty_print)
+        self._exportAttributes(
+            outfile,
+            level,
+            already_processed,
+            namespaceprefix_,
+            name_="AllowedValueListType",
+        )
+        if self.has__content():
+            outfile.write(">%s" % (eol_,))
+            self._exportChildren(
+                outfile,
+                level + 1,
+                namespaceprefix_,
+                namespacedef_,
+                name_="AllowedValueListType",
+                pretty_print=pretty_print,
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+            outfile.write("</%s%s>%s" % (namespaceprefix_, name_, eol_))
         else:
-            outfile.write('/>%s' % (eol_, ))
-    def exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='AllowedValueListType'):
-        pass
-    def exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ', name_='AllowedValueListType', fromsubclass_=False, pretty_print=True):
+            outfile.write("/>%s" % (eol_,))
+
+    def _exportAttributes(
+        self,
+        outfile,
+        level,
+        already_processed,
+        namespaceprefix_="",
+        name_="AllowedValueListType",
+    ):
+        pass
+
+    def _exportChildren(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ',
+        name_="AllowedValueListType",
+        fromsubclass_=False,
+        pretty_print=True,
+    ):
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
+            eol_ = ""
         for allowedValue_ in self.allowedValue:
-            namespaceprefix_ = self.allowedValue_nsprefix_ + ':' if (UseCapturedNS_ and self.allowedValue_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.allowedValue_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.allowedValue_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%sallowedValue>%s</%sallowedValue>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(allowedValue_), input_name='allowedValue')), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%sallowedValue>%s</%sallowedValue>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_xml(allowedValue_), input_name="allowedValue"
+                        )
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
+
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
-        self.buildAttributes(node, node.attrib, already_processed)
+        self._buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
-            self.buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+            self._buildChildren(
+                child, node, nodeName_, gds_collector_=gds_collector_
+            )
         return self
-    def buildAttributes(self, node, attrs, already_processed):
+
+    def _buildAttributes(self, node, attrs, already_processed):
         pass
-    def buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
-        if nodeName_ == 'allowedValue':
+
+    def _buildChildren(
+        self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
+    ):
+        if nodeName_ == "allowedValue":
             value_ = child_.text
-            value_ = self.gds_parse_string(value_, node, 'allowedValue')
-            value_ = self.gds_validate_string(value_, node, 'allowedValue')
+            value_ = self.gds_parse_string(value_, node, "allowedValue")
+            value_ = self.gds_validate_string(value_, node, "allowedValue")
             self.allowedValue.append(value_)
             self.allowedValue_nsprefix_ = child_.prefix
+
+
 # end class AllowedValueListType
 
 
 class AllowedValueRangeType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, minimum=None, maximum=None, step=None, gds_collector_=None, **kwargs_):
+
+    def __init__(
+        self,
+        minimum=None,
+        maximum=None,
+        step=None,
+        gds_collector_=None,
+        **kwargs_
+    ):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
-        self.parent_object_ = kwargs_.get('parent_object_')
+        self.parent_object_ = kwargs_.get("parent_object_")
         self.ns_prefix_ = None
         self.minimum = minimum
         self.minimum_nsprefix_ = None
         self.maximum = maximum
         self.maximum_nsprefix_ = None
         self.step = step
         self.step_nsprefix_ = None
+
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, AllowedValueRangeType)
+                CurrentSubclassModule_, AllowedValueRangeType
+            )
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
         if AllowedValueRangeType.subclass:
             return AllowedValueRangeType.subclass(*args_, **kwargs_)
         else:
             return AllowedValueRangeType(*args_, **kwargs_)
+
     factory = staticmethod(factory)
+
     def get_ns_prefix_(self):
         return self.ns_prefix_
+
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
+
     def get_minimum(self):
         return self.minimum
+
     def set_minimum(self, minimum):
         self.minimum = minimum
+
     def get_maximum(self):
         return self.maximum
+
     def set_maximum(self, maximum):
         self.maximum = maximum
+
     def get_step(self):
         return self.step
+
     def set_step(self, step):
         self.step = step
-    def hasContent_(self):
+
+    def has__content(self):
         if (
-            self.minimum is not None or
-            self.maximum is not None or
-            self.step is not None
+            self.minimum is not None
+            or self.maximum is not None
+            or self.step is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ', name_='AllowedValueRangeType', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('AllowedValueRangeType')
+
+    def export(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ',
+        name_="AllowedValueRangeType",
+        pretty_print=True,
+    ):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get(
+            "AllowedValueRangeType"
+        )
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'AllowedValueRangeType':
+            eol_ = ""
+        if (
+            self.original_tagname_ is not None
+            and name_ == "AllowedValueRangeType"
+        ):
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
-            namespaceprefix_ = self.ns_prefix_ + ':'
+            namespaceprefix_ = self.ns_prefix_ + ":"
         showIndent(outfile, level, pretty_print)
-        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        outfile.write(
+            "<%s%s%s"
+            % (
+                namespaceprefix_,
+                name_,
+                namespacedef_ and " " + namespacedef_ or "",
+            )
+        )
         already_processed = set()
-        self.exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='AllowedValueRangeType')
-        if self.hasContent_():
-            outfile.write('>%s' % (eol_, ))
-            self.exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='AllowedValueRangeType', pretty_print=pretty_print)
+        self._exportAttributes(
+            outfile,
+            level,
+            already_processed,
+            namespaceprefix_,
+            name_="AllowedValueRangeType",
+        )
+        if self.has__content():
+            outfile.write(">%s" % (eol_,))
+            self._exportChildren(
+                outfile,
+                level + 1,
+                namespaceprefix_,
+                namespacedef_,
+                name_="AllowedValueRangeType",
+                pretty_print=pretty_print,
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+            outfile.write("</%s%s>%s" % (namespaceprefix_, name_, eol_))
         else:
-            outfile.write('/>%s' % (eol_, ))
-    def exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='AllowedValueRangeType'):
-        pass
-    def exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ', name_='AllowedValueRangeType', fromsubclass_=False, pretty_print=True):
+            outfile.write("/>%s" % (eol_,))
+
+    def _exportAttributes(
+        self,
+        outfile,
+        level,
+        already_processed,
+        namespaceprefix_="",
+        name_="AllowedValueRangeType",
+    ):
+        pass
+
+    def _exportChildren(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="urn:schemas-upnp-org:service-1-0" ',
+        name_="AllowedValueRangeType",
+        fromsubclass_=False,
+        pretty_print=True,
+    ):
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
+            eol_ = ""
         if self.minimum is not None:
-            namespaceprefix_ = self.minimum_nsprefix_ + ':' if (UseCapturedNS_ and self.minimum_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.minimum_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.minimum_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%sminimum>%s</%sminimum>%s' % (namespaceprefix_ , self.gds_format_decimal(self.minimum, input_name='minimum'), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%sminimum>%s</%sminimum>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_format_decimal(
+                        self.minimum, input_name="minimum"
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.maximum is not None:
-            namespaceprefix_ = self.maximum_nsprefix_ + ':' if (UseCapturedNS_ and self.maximum_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.maximum_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.maximum_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%smaximum>%s</%smaximum>%s' % (namespaceprefix_ , self.gds_format_decimal(self.maximum, input_name='maximum'), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%smaximum>%s</%smaximum>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_format_decimal(
+                        self.maximum, input_name="maximum"
+                    ),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
         if self.step is not None:
-            namespaceprefix_ = self.step_nsprefix_ + ':' if (UseCapturedNS_ and self.step_nsprefix_) else ''
+            namespaceprefix_ = (
+                self.step_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.step_nsprefix_)
+                else ""
+            )
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%sstep>%s</%sstep>%s' % (namespaceprefix_ , self.gds_format_decimal(self.step, input_name='step'), namespaceprefix_ , eol_))
+            outfile.write(
+                "<%sstep>%s</%sstep>%s"
+                % (
+                    namespaceprefix_,
+                    self.gds_format_decimal(self.step, input_name="step"),
+                    namespaceprefix_,
+                    eol_,
+                )
+            )
+
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
-        self.buildAttributes(node, node.attrib, already_processed)
+        self._buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
-            self.buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+            self._buildChildren(
+                child, node, nodeName_, gds_collector_=gds_collector_
+            )
         return self
-    def buildAttributes(self, node, attrs, already_processed):
+
+    def _buildAttributes(self, node, attrs, already_processed):
         pass
-    def buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
-        if nodeName_ == 'minimum' and child_.text:
+
+    def _buildChildren(
+        self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
+    ):
+        if nodeName_ == "minimum" and child_.text:
             sval_ = child_.text
-            fval_ = self.gds_parse_decimal(sval_, node, 'minimum')
-            fval_ = self.gds_validate_decimal(fval_, node, 'minimum')
+            fval_ = self.gds_parse_decimal(sval_, node, "minimum")
+            fval_ = self.gds_validate_decimal(fval_, node, "minimum")
             self.minimum = fval_
             self.minimum_nsprefix_ = child_.prefix
-        elif nodeName_ == 'maximum' and child_.text:
+        elif nodeName_ == "maximum" and child_.text:
             sval_ = child_.text
-            fval_ = self.gds_parse_decimal(sval_, node, 'maximum')
-            fval_ = self.gds_validate_decimal(fval_, node, 'maximum')
+            fval_ = self.gds_parse_decimal(sval_, node, "maximum")
+            fval_ = self.gds_validate_decimal(fval_, node, "maximum")
             self.maximum = fval_
             self.maximum_nsprefix_ = child_.prefix
-        elif nodeName_ == 'step' and child_.text:
+        elif nodeName_ == "step" and child_.text:
             sval_ = child_.text
-            fval_ = self.gds_parse_decimal(sval_, node, 'step')
-            fval_ = self.gds_validate_decimal(fval_, node, 'step')
+            fval_ = self.gds_parse_decimal(sval_, node, "step")
+            fval_ = self.gds_validate_decimal(fval_, node, "step")
             self.step = fval_
             self.step_nsprefix_ = child_.prefix
+
+
 # end class AllowedValueRangeType
 
 
 class retvalType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
+
     def __init__(self, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
-        self.parent_object_ = kwargs_.get('parent_object_')
+        self.parent_object_ = kwargs_.get("parent_object_")
         self.ns_prefix_ = None
+
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, retvalType)
+                CurrentSubclassModule_, retvalType
+            )
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
         if retvalType.subclass:
             return retvalType.subclass(*args_, **kwargs_)
         else:
             return retvalType(*args_, **kwargs_)
+
     factory = staticmethod(factory)
+
     def get_ns_prefix_(self):
         return self.ns_prefix_
+
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def hasContent_(self):
-        if (
 
-        ):
+    def has__content(self):
+        if ():
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='retvalType', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('retvalType')
+
+    def export(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_="",
+        name_="retvalType",
+        pretty_print=True,
+    ):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get("retvalType")
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
-            eol_ = '\n'
+            eol_ = "\n"
         else:
-            eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'retvalType':
+            eol_ = ""
+        if self.original_tagname_ is not None and name_ == "retvalType":
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
-            namespaceprefix_ = self.ns_prefix_ + ':'
+            namespaceprefix_ = self.ns_prefix_ + ":"
         showIndent(outfile, level, pretty_print)
-        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        outfile.write(
+            "<%s%s%s"
+            % (
+                namespaceprefix_,
+                name_,
+                namespacedef_ and " " + namespacedef_ or "",
+            )
+        )
         already_processed = set()
-        self.exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='retvalType')
-        if self.hasContent_():
-            outfile.write('>%s' % (eol_, ))
-            self.exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='retvalType', pretty_print=pretty_print)
-            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+        self._exportAttributes(
+            outfile,
+            level,
+            already_processed,
+            namespaceprefix_,
+            name_="retvalType",
+        )
+        if self.has__content():
+            outfile.write(">%s" % (eol_,))
+            self._exportChildren(
+                outfile,
+                level + 1,
+                namespaceprefix_,
+                namespacedef_,
+                name_="retvalType",
+                pretty_print=pretty_print,
+            )
+            outfile.write("</%s%s>%s" % (namespaceprefix_, name_, eol_))
         else:
-            outfile.write('/>%s' % (eol_, ))
-    def exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='retvalType'):
-        pass
-    def exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='retvalType', fromsubclass_=False, pretty_print=True):
+            outfile.write("/>%s" % (eol_,))
+
+    def _exportAttributes(
+        self,
+        outfile,
+        level,
+        already_processed,
+        namespaceprefix_="",
+        name_="retvalType",
+    ):
+        pass
+
+    def _exportChildren(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_="",
+        name_="retvalType",
+        fromsubclass_=False,
+        pretty_print=True,
+    ):
         pass
+
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
-        self.buildAttributes(node, node.attrib, already_processed)
+        self._buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
-            self.buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+            self._buildChildren(
+                child, node, nodeName_, gds_collector_=gds_collector_
+            )
         return self
-    def buildAttributes(self, node, attrs, already_processed):
+
+    def _buildAttributes(self, node, attrs, already_processed):
         pass
-    def buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
+
+    def _buildChildren(
+        self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
+    ):
         pass
+
+
 # end class retvalType
 
 
-GDSClassesMapping = {
-}
+GDSClassesMapping = {}
 
 
 USAGE_TEXT = """
 Usage: python <Parser>.py [ -s ] <in_xml_file>
 """
 
 
 def usage():
     print(USAGE_TEXT)
     sys.exit(1)
 
 
 def get_root_tag(node):
     tag = Tag_pattern_.match(node.tag).groups()[-1]
-    rootClass = GDSClassesMapping.get(tag)
+    prefix_tag = TagNamePrefix + tag
+    rootClass = GDSClassesMapping.get(prefix_tag)
     if rootClass is None:
-        rootClass = globals().get(tag)
+        rootClass = globals().get(prefix_tag)
     return tag, rootClass
 
 
 def get_required_ns_prefix_defs(rootNode):
-    '''Get all name space prefix definitions required in this XML doc.
+    """Get all name space prefix definitions required in this XML doc.
     Return a dictionary of definitions and a char string of definitions.
-    '''
+    """
     nsmap = {
         prefix: uri
         for node in rootNode.iter()
         for (prefix, uri) in node.nsmap.items()
         if prefix is not None
     }
-    namespacedefs = ' '.join([
-        'xmlns:{}="{}"'.format(prefix, uri)
-        for prefix, uri in nsmap.items()
-    ])
+    namespacedefs = " ".join(
+        ['xmlns:{}="{}"'.format(prefix, uri) for prefix, uri in nsmap.items()]
+    )
     return nsmap, namespacedefs
 
 
 def parse(inFileName, silence=False, print_warnings=True):
     global CapturedNsmap_
     gds_collector = GdsCollector_()
     parser = None
     doc = parsexml_(inFileName, parser)
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
-        rootTag = 'scpd'
+        rootTag = "scpd"
         rootClass = scpd
     rootObj = rootClass.factory()
     rootObj.build(rootNode, gds_collector_=gds_collector)
     CapturedNsmap_, namespacedefs = get_required_ns_prefix_defs(rootNode)
     if not SaveElementTreeNode:
         doc = None
         rootNode = None
     if not silence:
         sys.stdout.write('<?xml version="1.0" ?>\n')
         rootObj.export(
-            sys.stdout, 0, name_=rootTag,
+            sys.stdout,
+            0,
+            name_=rootTag,
             namespacedef_=namespacedefs,
-            pretty_print=True)
+            pretty_print=True,
+        )
     if print_warnings and len(gds_collector.get_messages()) > 0:
-        separator = ('-' * 50) + '\n'
+        separator = ("-" * 50) + "\n"
         sys.stderr.write(separator)
-        sys.stderr.write('----- Warnings -- count: {} -----\n'.format(
-            len(gds_collector.get_messages()), ))
+        sys.stderr.write(
+            "----- Warnings -- count: {} -----\n".format(
+                len(gds_collector.get_messages()),
+            )
+        )
         gds_collector.write_messages(sys.stderr)
         sys.stderr.write(separator)
     return rootObj
 
 
-def parseEtree(inFileName, silence=False, print_warnings=True,
-               mapping=None, nsmap=None):
+def parseEtree(
+    inFileName,
+    silence=False,
+    print_warnings=True,
+    mapping=None,
+    reverse_mapping=None,
+    nsmap=None,
+):
     parser = None
     doc = parsexml_(inFileName, parser)
     gds_collector = GdsCollector_()
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
-        rootTag = 'scpd'
+        rootTag = "scpd"
         rootClass = scpd
     rootObj = rootClass.factory()
     rootObj.build(rootNode, gds_collector_=gds_collector)
-    # Enable Python to collect the space used by the DOM.
     if mapping is None:
         mapping = {}
+    if reverse_mapping is None:
+        reverse_mapping = {}
     rootElement = rootObj.to_etree(
-        None, name_=rootTag, mapping_=mapping, nsmap_=nsmap)
-    reverse_mapping = rootObj.gds_reverse_node_mapping(mapping)
+        None,
+        name_=rootTag,
+        mapping_=mapping,
+        reverse_mapping_=reverse_mapping,
+        nsmap_=nsmap,
+    )
+    reverse_node_mapping = rootObj.gds_reverse_node_mapping(mapping)
+    # Enable Python to collect the space used by the DOM.
     if not SaveElementTreeNode:
         doc = None
         rootNode = None
     if not silence:
         content = etree_.tostring(
-            rootElement, pretty_print=True,
-            xml_declaration=True, encoding="utf-8")
+            rootElement,
+            pretty_print=True,
+            xml_declaration=True,
+            encoding="utf-8",
+        )
         sys.stdout.write(str(content))
-        sys.stdout.write('\n')
+        sys.stdout.write("\n")
     if print_warnings and len(gds_collector.get_messages()) > 0:
-        separator = ('-' * 50) + '\n'
+        separator = ("-" * 50) + "\n"
         sys.stderr.write(separator)
-        sys.stderr.write('----- Warnings -- count: {} -----\n'.format(
-            len(gds_collector.get_messages()), ))
+        sys.stderr.write(
+            "----- Warnings -- count: {} -----\n".format(
+                len(gds_collector.get_messages()),
+            )
+        )
         gds_collector.write_messages(sys.stderr)
         sys.stderr.write(separator)
-    return rootObj, rootElement, mapping, reverse_mapping
+    return rootObj, rootElement, mapping, reverse_node_mapping
 
 
 def parseString(inString, silence=False, print_warnings=True):
-    '''Parse a string, create the object tree, and export it.
+    """Parse a string, create the object tree, and export it.
 
     Arguments:
     - inString -- A string.  This XML fragment should not start
       with an XML declaration containing an encoding.
     - silence -- A boolean.  If False, export the object.
     Returns -- The root object in the tree.
-    '''
+    """
     parser = None
-    rootNode= parsexmlstring_(inString, parser)
+    rootNode = parsexmlstring_(inString, parser)
     gds_collector = GdsCollector_()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
-        rootTag = 'scpd'
+        rootTag = "scpd"
         rootClass = scpd
     rootObj = rootClass.factory()
     rootObj.build(rootNode, gds_collector_=gds_collector)
     if not SaveElementTreeNode:
         rootNode = None
     if not silence:
         sys.stdout.write('<?xml version="1.0" ?>\n')
-        rootObj.export(
-            sys.stdout, 0, name_=rootTag,
-            namespacedef_='')
+        rootObj.export(sys.stdout, 0, name_=rootTag, namespacedef_="")
     if print_warnings and len(gds_collector.get_messages()) > 0:
-        separator = ('-' * 50) + '\n'
+        separator = ("-" * 50) + "\n"
         sys.stderr.write(separator)
-        sys.stderr.write('----- Warnings -- count: {} -----\n'.format(
-            len(gds_collector.get_messages()), ))
+        sys.stderr.write(
+            "----- Warnings -- count: {} -----\n".format(
+                len(gds_collector.get_messages()),
+            )
+        )
         gds_collector.write_messages(sys.stderr)
         sys.stderr.write(separator)
     return rootObj
 
 
 def parseLiteral(inFileName, silence=False, print_warnings=True):
     parser = None
     doc = parsexml_(inFileName, parser)
     gds_collector = GdsCollector_()
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
-        rootTag = 'scpd'
+        rootTag = "scpd"
         rootClass = scpd
     rootObj = rootClass.factory()
     rootObj.build(rootNode, gds_collector_=gds_collector)
     # Enable Python to collect the space used by the DOM.
     if not SaveElementTreeNode:
         doc = None
         rootNode = None
     if not silence:
-        sys.stdout.write('#from service import *\n\n')
-        sys.stdout.write('import service as model_\n\n')
-        sys.stdout.write('rootObj = model_.rootClass(\n')
+        sys.stdout.write("#from service import *\n\n")
+        sys.stdout.write("import service as model_\n\n")
+        sys.stdout.write("rootObj = model_.rootClass(\n")
         rootObj.exportLiteral(sys.stdout, 0, name_=rootTag)
-        sys.stdout.write(')\n')
+        sys.stdout.write(")\n")
     if print_warnings and len(gds_collector.get_messages()) > 0:
-        separator = ('-' * 50) + '\n'
+        separator = ("-" * 50) + "\n"
         sys.stderr.write(separator)
-        sys.stderr.write('----- Warnings -- count: {} -----\n'.format(
-            len(gds_collector.get_messages()), ))
+        sys.stderr.write(
+            "----- Warnings -- count: {} -----\n".format(
+                len(gds_collector.get_messages()),
+            )
+        )
         gds_collector.write_messages(sys.stderr)
         sys.stderr.write(separator)
     return rootObj
 
 
 def main():
     args = sys.argv[1:]
     if len(args) == 1:
         parse(args[0])
     else:
         usage()
 
 
-if __name__ == '__main__':
-    #import pdb; pdb.set_trace()
+if __name__ == "__main__":
+    # import pdb; pdb.set_trace()
     main()
 
-RenameMappings_ = {
-}
+RenameMappings_ = {}
 
 #
 # Mapping of namespaces to types defined in them
 # and the file in which each is defined.
 # simpleTypes are marked "ST" and complexTypes "CT".
-NamespaceToDefMappings_ = {'urn:schemas-upnp-org:service-1-0': [('SpecVersionType', 'service.xsd', 'CT'),
-                                      ('ActionListType', 'service.xsd', 'CT'),
-                                      ('ActionType', 'service.xsd', 'CT'),
-                                      ('ArgumentListType', 'service.xsd', 'CT'),
-                                      ('ArgumentType', 'service.xsd', 'CT'),
-                                      ('ServiceStateTableType',
-                                       'service.xsd',
-                                       'CT'),
-                                      ('StateVariableType',
-                                       'service.xsd',
-                                       'CT'),
-                                      ('AllowedValueListType',
-                                       'service.xsd',
-                                       'CT'),
-                                      ('AllowedValueRangeType',
-                                       'service.xsd',
-                                       'CT')]}
+NamespaceToDefMappings_ = {
+    "urn:schemas-upnp-org:service-1-0": [
+        (
+            "SpecVersionType",
+            "pywemo/ouimeaux_device/api/xsd/service.xsd",
+            "CT",
+        ),
+        ("ActionListType", "pywemo/ouimeaux_device/api/xsd/service.xsd", "CT"),
+        ("ActionType", "pywemo/ouimeaux_device/api/xsd/service.xsd", "CT"),
+        (
+            "ArgumentListType",
+            "pywemo/ouimeaux_device/api/xsd/service.xsd",
+            "CT",
+        ),
+        ("ArgumentType", "pywemo/ouimeaux_device/api/xsd/service.xsd", "CT"),
+        (
+            "ServiceStateTableType",
+            "pywemo/ouimeaux_device/api/xsd/service.xsd",
+            "CT",
+        ),
+        (
+            "StateVariableType",
+            "pywemo/ouimeaux_device/api/xsd/service.xsd",
+            "CT",
+        ),
+        (
+            "AllowedValueListType",
+            "pywemo/ouimeaux_device/api/xsd/service.xsd",
+            "CT",
+        ),
+        (
+            "AllowedValueRangeType",
+            "pywemo/ouimeaux_device/api/xsd/service.xsd",
+            "CT",
+        ),
+    ]
+}
 
 __all__ = [
     "ActionListType",
     "ActionType",
     "AllowedValueListType",
     "AllowedValueRangeType",
     "ArgumentListType",
     "ArgumentType",
     "ServiceStateTableType",
     "SpecVersionType",
     "StateVariableType",
     "retvalType",
-    "scpd"
+    "scpd",
 ]
```

### Comparing `pywemo-0.9.2/pywemo/ouimeaux_device/api/xsd/service.xsd` & `pywemo-1.0.0/pywemo/ouimeaux_device/api/xsd/service.xsd`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.2/pywemo/ouimeaux_device/api/xsd_types.py` & `pywemo-1.0.0/pywemo/ouimeaux_device/api/xsd_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 fields of the dataclass instances are fully populated and valid. Any parsing
 or validation issues will result in InvalidSchemaError being raised.
 """
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass
-from typing import Any
+from typing import Any, Dict, List
 
 from lxml import etree as et
 
 from pywemo.exceptions import InvalidSchemaError
 
 from .xsd import device as device_parser
 from .xsd import service as service_parser
@@ -118,28 +118,28 @@
             description_url=_get_element_text(service, "SCPDURL"),
             control_url=_get_element_text(service, "controlURL"),
             event_subscription_url=_get_element_text(service, "eventSubURL"),
         )
 
 
 @dataclass(frozen=True)
-class DeviceDescription:
+class DeviceDescription:  # pylint: disable=too-many-instance-attributes
     """Device properties from the DeviceType xsd type."""
 
     firmware_version: str
     name: str
     mac: str
     manufacturer: str
     model: str
     model_name: str
     serial_number: str
     udn: str
-    _config_any: dict[str, str]
+    _config_any: Dict[str, str]
     _device_type: str
-    _services: list[ServiceProperties]
+    _services: List[ServiceProperties]
 
     @staticmethod
     def dict_from_xml(setup_xml_content: bytes) -> dict[str, Any]:
         """Parse and validate the DeviceType xsd type."""
         try:
             root = device_parser.parseString(  # type: ignore
                 setup_xml_content, silence=True, print_warnings=False
@@ -153,15 +153,20 @@
         manufacturer = _get_element_text(device, "manufacturer")
         if manufacturer != "Belkin International Inc.":
             raise InvalidSchemaError(
                 f"Unexpected manufacturer: {manufacturer}"
             )
 
         if device.anytypeobjs_:
-            xs_any = (et.fromstring(extra) for extra in device.anytypeobjs_)
+            xs_any = (
+                et.fromstring(
+                    extra, parser=et.XMLParser(resolve_entities=False)
+                )
+                for extra in device.anytypeobjs_
+            )
             config_any = {
                 et.QName(tag).localname: tag.text.strip()
                 for tag in xs_any
                 if tag.text and tag.text.strip()
             }
         else:
             config_any = {}
```

### Comparing `pywemo-0.9.2/pywemo/ouimeaux_device/bridge.py` & `pywemo-1.0.0/pywemo/ouimeaux_device/bridge.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,308 +1,365 @@
 """Representation of a WeMo Bridge (Link) device."""
 from __future__ import annotations
 
 import io
-import sys
 import time
+import warnings
 from html import escape
-from typing import Any
+from typing import Any, Iterable, TypedDict
 
 from lxml import etree as et
 
 from ..color import ColorXY, get_profiles, limit_to_gamut
+from ..exceptions import InvalidSchemaError
 from . import Device
 from .api.service import RequiredService
 
 CAPABILITY_ID2NAME = dict(
     (
-        ('10006', "onoff"),
-        ('10008', "levelcontrol"),
-        ('30008', "sleepfader"),
-        ('30009', "levelcontrol_move"),
-        ('3000A', "levelcontrol_stop"),
-        ('10300', "colorcontrol"),
-        ('30301', "colortemperature"),
+        ("10006", "onoff"),
+        ("10008", "levelcontrol"),
+        ("30008", "sleepfader"),
+        ("30009", "levelcontrol_move"),
+        ("3000A", "levelcontrol_stop"),
+        ("10300", "colorcontrol"),
+        ("30301", "colortemperature"),
     )
 )
 CAPABILITY_NAME2ID = dict(
     (val, cap) for cap, val in CAPABILITY_ID2NAME.items()
 )
 
 # acceptable values for 'onoff'
 OFF = 0
 ON = 1
 TOGGLE = 2
 
 
+def _warn_rename(old: str, new: str, stacklevel: int = 3) -> None:
+    warnings.warn(
+        f"{old} is deprecated and will be removed in a future release. "
+        f"Use {new} instead",
+        DeprecationWarning,
+        stacklevel=stacklevel,
+    )
+
+
 def limit(value: int, min_val: int, max_val: int) -> int:
     """Return a value clipped to the range [min_val, max_val]."""
     return max(min_val, min(value, max_val))
 
 
 class Bridge(Device):
     """Representation of a WeMo Bridge (Link) device."""
 
-    Lights: dict[str, Light] = {}
-    Groups: dict[str, Group] = {}
+    lights: dict[str, Light]
+    groups: dict[str, Group]
 
     EVENT_TYPE_STATUS_CHANGE = "StatusChange"
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         """Create a WeMo Bridge (Link) device."""
         super().__init__(*args, **kwargs)
+        self.lights = {}
+        self.groups = {}
         self.bridge_update()
 
     def __repr__(self) -> str:
         """Return a string representation of the device."""
         return (
-            '<WeMo Bridge "{name}", Lights: {lights}, ' + 'Groups: {groups}>'
+            '<WeMo Bridge "{name}", Lights: {lights}, ' + "Groups: {groups}>"
         ).format(
-            name=self.name, lights=len(self.Lights), groups=len(self.Groups)
+            name=self.name, lights=len(self.lights), groups=len(self.groups)
         )
 
     @property
     def _required_services(self) -> list[RequiredService]:
         return super()._required_services + [
             RequiredService(name="basicevent", actions=["GetMacAddr"]),
             RequiredService(
                 name="bridge",
                 actions=["GetDeviceStatus", "SetDeviceStatus"],
             ),
         ]
 
+    @property
+    def Lights(self) -> dict[str, Light]:  # pylint: disable=invalid-name
+        """Deprecated method for accessing .lights."""
+        _warn_rename("Lights", "lights")
+        return self.lights
+
+    @property
+    def Groups(self) -> dict[str, Group]:  # pylint: disable=invalid-name
+        """Deprecated method for accessing .groups."""
+        _warn_rename("Groups", "groups")
+        return self.groups
+
     def bridge_update(
         self, force_update: bool = True
     ) -> tuple[dict[str, Light], dict[str, Group]]:
         """Get updated status information for the bridge and its lights."""
-        if force_update or self.Lights is None or self.Groups is None:
-            plugin_udn = self.basicevent.GetMacAddr().get('PluginUDN')
+        if force_update or self.lights is None or self.groups is None:
+            plugin_udn = self.basicevent.GetMacAddr().get("PluginUDN")
 
-            if hasattr(self.bridge, 'GetEndDevicesWithStatus'):
+            if hasattr(self.bridge, "GetEndDevicesWithStatus"):
                 end_devices = self.bridge.GetEndDevicesWithStatus(
-                    DevUDN=plugin_udn, ReqListType='PAIRED_LIST'
+                    DevUDN=plugin_udn, ReqListType="PAIRED_LIST"
                 )
             else:
                 end_devices = self.bridge.GetEndDevices(
-                    DevUDN=plugin_udn, ReqListType='PAIRED_LIST'
+                    DevUDN=plugin_udn, ReqListType="PAIRED_LIST"
                 )
 
-            end_devices_xml = end_devices.get('DeviceLists')
-            if not end_devices_xml:
-                return self.Lights, self.Groups
-
-            end_device_list = et.fromstring(end_devices_xml.encode('utf-8'))
-
-            for light in end_device_list.iter('DeviceInfo'):
-                uniqueID = light.find('DeviceID').text
-                if uniqueID in self.Lights:
-                    self.Lights[uniqueID].update_state(light)
+            if not (end_devices_xml := end_devices.get("DeviceLists")):
+                return self.lights, self.groups
+
+            end_device_list = et.fromstring(
+                end_devices_xml.encode("utf-8"),
+                parser=et.XMLParser(resolve_entities=False),
+            )
+
+            for light in end_device_list.iter("DeviceInfo"):
+                if not (device_id := light.findtext("DeviceID")):
+                    raise InvalidSchemaError(
+                        f"DeviceID missing: {et.tostring(light).decode()}"
+                    )
+                if device_id in self.lights:
+                    self.lights[device_id].update_state(light)
                 else:
-                    self.Lights[uniqueID] = Light(self, light)
+                    self.lights[device_id] = Light(self, light)
 
-            for group in end_device_list.iter('GroupInfo'):
-                uniqueID = group.find('GroupID').text
-                if uniqueID in self.Groups:
-                    self.Groups[uniqueID].update_state(group)
+            for group in end_device_list.iter("GroupInfo"):
+                if not (group_id := group.findtext("GroupID")):
+                    raise InvalidSchemaError(
+                        f"GroupID missing: {et.tostring(group).decode()}"
+                    )
+                if group_id in self.groups:
+                    self.groups[group_id].update_state(group)
                 else:
-                    self.Groups[uniqueID] = Group(self, group)
+                    self.groups[group_id] = Group(self, group)
 
-        return self.Lights, self.Groups
+        return self.lights, self.groups
 
     def get_state(self, force_update: bool = False) -> int:
         """Update the state of the Bridge device."""
         state = super().get_state(force_update)
         self.bridge_update(force_update)
         return state
 
     def subscription_update(self, _type: str, _param: str) -> bool:
         """Update the bridge attributes due to a subscription update event."""
         if _type == self.EVENT_TYPE_STATUS_CHANGE and _param:
-            state_event = et.fromstring(_param.encode('utf8'))
-            key = state_event.findtext('DeviceID')
-            if not key:
+            try:
+                state_event = et.fromstring(
+                    _param.encode("utf8"),
+                    parser=et.XMLParser(resolve_entities=False),
+                )
+            except et.XMLSyntaxError:
+                return False
+            if not (key := state_event.findtext("DeviceID")):
                 return False
-            if key in self.Lights:
-                return self.Lights[key].subscription_update(state_event)
+            if key in self.lights:
+                return self.lights[key].subscription_update(state_event)
 
-            if key in self.Groups:
-                return self.Groups[key].subscription_update(state_event)
+            if key in self.groups:
+                return self.groups[key].subscription_update(state_event)
 
             return False
         return super().subscription_update(_type, _param)
 
-    def bridge_getdevicestatus(self, deviceid: str) -> et.Element | None:
+    def bridge_getdevicestatus(self, deviceid: str) -> et._Element | None:
         """Return the list of device statuses for the bridge's lights."""
         status_list = self.bridge.GetDeviceStatus(DeviceIDs=deviceid)
-        device_status_list_xml = status_list.get('DeviceStatusList')
+        device_status_list_xml = status_list.get("DeviceStatusList")
         if not device_status_list_xml:
             return None
         device_status_list = et.fromstring(
-            device_status_list_xml.encode('utf-8')
+            device_status_list_xml.encode("utf-8"),
+            parser=et.XMLParser(resolve_entities=False),
         )
 
-        return device_status_list.find('DeviceStatus')
+        return device_status_list.find("DeviceStatus")
 
     def bridge_setdevicestatus(
         self, isgroup: str, deviceid: str, capids: list[str], values: list[str]
     ) -> dict[str, str]:
         """Set the status of the bridge's lights."""
-        req = et.Element('DeviceStatus')
-        et.SubElement(req, 'IsGroupAction').text = isgroup
-        et.SubElement(req, 'DeviceID', available="YES").text = deviceid
-        et.SubElement(req, 'CapabilityID').text = ','.join(capids)
-        et.SubElement(req, 'CapabilityValue').text = ','.join(values)
+        req = et.Element("DeviceStatus")
+        et.SubElement(req, "IsGroupAction").text = isgroup
+        et.SubElement(req, "DeviceID", available="YES").text = deviceid
+        et.SubElement(req, "CapabilityID").text = ",".join(capids)
+        et.SubElement(req, "CapabilityValue").text = ",".join(values)
 
         buf = io.BytesIO()
-        et.ElementTree(req).write(buf, encoding='UTF-8', xml_declaration=True)
+        et.ElementTree(req).write(buf, encoding="UTF-8", xml_declaration=True)
         send_state = escape(buf.getvalue().decode(), quote=True)
 
         return self.bridge.SetDeviceStatus(DeviceStatusList=send_state)
 
 
-if sys.version_info >= (3, 8):
-    # Remove pylint disable when Python 3.7 support is removed.
-    from typing import TypedDict  # pylint: disable=no-name-in-module
-
-    class DeviceState(TypedDict, total=False):
-        """LinkedDevice state dictionary type."""
-
-        available: bool
-        onoff: int
-        level: int
-        temperature_mireds: int
-        temperature_kelvin: int
-        color_xy: ColorXY
-
-else:
-    from typing import Dict, Union
+class DeviceState(TypedDict, total=False):
+    """LinkedDevice state dictionary type."""
 
-    DeviceState = Dict[str, Union[ColorXY, bool, int]]
+    available: bool
+    onoff: int
+    level: int
+    temperature_mireds: int
+    temperature_kelvin: int
+    color_xy: ColorXY
 
 
-class LinkedDevice:
+class LinkedDevice:  # pylint: disable=too-many-instance-attributes
     """Representation of a device connected to the bridge."""
 
-    def __init__(self, bridge: Bridge, info: et.Element) -> None:
+    _NAME_TAG: str
+    _CAPABILITIES_TAGS: tuple[str, ...]
+    _VALUES_TAGS: tuple[str, ...]
+
+    def __init__(self, bridge: Bridge, info: et._Element) -> None:
         """Create a Linked Device."""
-        self.bridge = bridge
-        self.host = self.bridge.host
-        self.port = self.bridge.port
-        self.name = ''
+        self.bridge: Bridge = bridge
+        self.host: str = self.bridge.host
+        self.port: int = self.bridge.port
+        self.name: str = ""
         self.state: DeviceState = {}
-        self.capabilities: list[str] = []
-        self._values: list[str] = []
+        self.capabilities: Iterable[str] = tuple()
         self.update_state(info)
         self._last_err: dict[str, str] = {}
-        self.mac = self.bridge.mac
-        self.serialnumber = self.bridge.serial_number
-        self.uniqueID = ''
+        self.mac: str = self.bridge.mac
+        self.serial_number: str = self.bridge.serial_number
+        self.uniqueID: str = ""  # pylint: disable=invalid-name
 
     def get_state(self, force_update: bool = False) -> DeviceState:
         """Return the status of the device."""
         if force_update:
             self.bridge.bridge_update()
         return self.state
 
-    def update_state(self, status: Any) -> None:
-        """
-        Set the device state based on capabilities and values.
-
-        Subclasses should parse status into self.capabilities and
-        self._values and then call this to populate self.state.
-        """
-        status = {}
-        for capability, value in zip(self.capabilities, self._values):
+    def update_state(self, status: et._Element) -> None:
+        """Fetch the capabilities and values then update the device state."""
+        if name := status.findtext(self._NAME_TAG, ""):
+            self.name = name
+
+        def get_first_text(tags: Iterable[str]) -> str | None:
+            candidates = (status.findtext(tag) for tag in tags)
+            return next(filter(bool, candidates), None)
+
+        if capabilities := get_first_text(self._CAPABILITIES_TAGS):
+            self.capabilities = tuple(
+                CAPABILITY_ID2NAME.get(c, c) for c in capabilities.split(",")
+            )
+            if current_state := get_first_text(self._VALUES_TAGS):
+                self._update_values(
+                    zip(self.capabilities, current_state.split(","))
+                )
+
+    def _update_values(self, values: Iterable[tuple[str, str]]) -> None:
+        """Set the device state based on capabilities and values."""
+        status: dict[str, tuple[int, ...] | None] = {}
+        for capability, value in values:
+            if capability not in CAPABILITY_NAME2ID:
+                continue  # Ignore unsupported capabilities.
             if not value:
                 status[capability] = None
-            elif ':' in value:
+                continue
+            try:
                 status[capability] = tuple(
-                    int(round(float(v))) for v in value.split(':')
+                    int(round(float(v))) for v in value.split(":")
                 )
-            else:
-                status[capability] = int(round(float(value)))
+            except ValueError as err:
+                raise ValueError(
+                    f"Invalid value for {capability}: {repr(value)}"
+                ) from err
 
         # unreachable devices have empty strings for all capability values
-        if status.get('onoff') is None:
-            self.state['available'] = False
-            self.state['onoff'] = 0
-            return
-
-        self.state['available'] = True
-        self.state['onoff'] = status['onoff']
-
-        if status.get('levelcontrol') is not None:
-            self.state['level'] = status['levelcontrol'][0]
-
-        if status.get('colortemperature') is not None:
-            temperature = status['colortemperature'][0]
-            self.state['temperature_mireds'] = temperature
-            self.state['temperature_kelvin'] = int(1000000 / temperature)
-
-        if status.get('colorcontrol') is not None:
-            colorx, colory = status['colorcontrol'][:2]
-            colorx, colory = colorx / 65535.0, colory / 65535.0
-            self.state['color_xy'] = colorx, colory
+        if (on_off := status.get("onoff", ("Missing",))) is None:
+            self.state["available"] = False
+            self.state["onoff"] = 0
+        elif isinstance(on_off[0], int):
+            self.state["available"] = True
+            self.state["onoff"] = on_off[0]
+
+        if (level_control := status.get("levelcontrol")) is not None:
+            self.state["level"] = level_control[0]
+
+        if (color_temperature := status.get("colortemperature")) is not None:
+            temperature = color_temperature[0]
+            if temperature <= 0:
+                raise ValueError(
+                    f"Invalid value for color temperature: {temperature}"
+                )
+            self.state["temperature_mireds"] = temperature
+            self.state["temperature_kelvin"] = int(1000000 / temperature)
+
+        if (color_control := status.get("colorcontrol")) is not None:
+            if len(color_control) < 2:
+                raise ValueError(
+                    f"Too few values for colorcontrol: {repr(color_control)}"
+                )
+            color_x, color_y = float(color_control[0]), float(color_control[1])
+            color_x, color_y = color_x / 65535.0, color_y / 65535.0
+            self.state["color_xy"] = color_x, color_y
 
-    def subscription_update(self, state_event: et.Element) -> bool:
+    def subscription_update(self, state_event: et._Element) -> bool:
         """Update the light values due to a subscription update event."""
-        device_id = state_event.find('DeviceID')
-        if device_id.get('available', 'YES').upper() == 'YES':
-            capability = state_event.findtext('CapabilityId')
-            value = state_event.findtext('Value')
+        if (
+            device_id := state_event.find("DeviceID")
+        ) is None or device_id.get("available", "YES").upper() == "YES":
+            capability = state_event.findtext("CapabilityId")
+            value = state_event.findtext("Value")
         else:
-            capability = CAPABILITY_NAME2ID.get('onoff')
-            value = ''  # Use an empty string to indicate an unreachable device
+            capability = CAPABILITY_NAME2ID.get("onoff")
+            value = ""  # Use an empty string to indicate an unreachable device
 
         if capability is None or value is None:
             return False
+
         name = CAPABILITY_ID2NAME.get(capability, capability)
-        # Update only the capability/value pair that changed.
-        try:
-            index = self.capabilities.index(name)
-        except ValueError:
+        if name not in self.capabilities:
             # Should't receive updates for capabilities that were not
             # originally present.
             return False
-        self._values[index] = value
 
-        # Don't call the subclass. It expects to have a list of all the
-        # capability/value pairs. The subscription_update only receives a
-        # single capability/value pair.
-        LinkedDevice.update_state(self, {})
+        try:
+            self._update_values([(name, value)])
+        except ValueError:
+            return False
         return True
 
     def _setdevicestatus(self, **kwargs: Any) -> LinkedDevice:
         """Ask the bridge to set the device status."""
-        isgroup = 'YES' if isinstance(self, Group) else 'NO'
+        isgroup = "YES" if isinstance(self, Group) else "NO"
 
         capids = []
         values = []
         for cap, val in kwargs.items():
             capids.append(CAPABILITY_NAME2ID[cap])
 
             if not isinstance(val, (list, tuple)):
                 val = (val,)
-            values.append(':'.join(str(v) for v in val))
+            values.append(":".join(str(v) for v in val))
 
         self._last_err = self.bridge.bridge_setdevicestatus(
             isgroup, self.uniqueID, capids, values
         )
         return self
 
-    def turn_on(
+    def turn_on(  # pylint: disable=unused-argument
         self,
         level: int | None = None,
         transition: int = 0,
         force_update: bool = False,
     ) -> LinkedDevice:
         """Turn on the device."""
         return self._setdevicestatus(onoff=ON)
 
-    def turn_off(self, transition: int = 0) -> LinkedDevice:
+    def turn_off(  # pylint: disable=unused-argument
+        self, transition: int = 0
+    ) -> LinkedDevice:
         """Turn off the device."""
         return self._setdevicestatus(onoff=OFF)
 
     def toggle(self) -> LinkedDevice:
         """Toggle the device from on to off or off to on."""
         return self._setdevicestatus(onoff=TOGGLE)
 
@@ -312,75 +369,58 @@
         return type(self).__name__
 
     def __repr__(self) -> str:
         """Return a string representation of the device."""
         return f'<{self.device_type.upper()} "{self.name}">'
 
 
-class Light(LinkedDevice):
+class Light(LinkedDevice):  # pylint: disable=too-many-instance-attributes
     """Representation of a Light connected to the Bridge."""
 
-    def __init__(self, bridge: Bridge, info: et.Element) -> None:
+    _NAME_TAG = "FriendlyName"
+    _CAPABILITIES_TAGS = ("CapabilityIDs", "CapabilityID")
+    _VALUES_TAGS = ("CurrentState", "CapabilityValue")
+
+    def __init__(self, bridge: Bridge, info: et._Element) -> None:
         """Create a Light device."""
         super().__init__(bridge, info)
 
-        self.device_index = info.findtext('DeviceIndex')
-        self.uniqueID = info.findtext('DeviceID')
-        self.iconvalue = info.findtext('IconVersion')
-        self.firmware = info.findtext('FirmwareVersion')
-        self.manufacturer = info.findtext('Manufacturer')
-        self.model = info.findtext('ModelCode')
-        self.certified = info.findtext('WeMoCertified')
+        self.device_index: str = info.findtext("DeviceIndex", "")
+        self.uniqueID: str = info.findtext("DeviceID", "")
+        self.iconvalue: str = info.findtext("IconVersion", "")
+        self.firmware: str = info.findtext("FirmwareVersion", "")
+        self.manufacturer: str = info.findtext("Manufacturer", "")
+        self.model: str = info.findtext("ModelCode", "")
+        self.certified: str = info.findtext("WeMoCertified", "")
 
         self.temperature_range, self.gamut = get_profiles(self.model)
         self._pending: dict[str, Any] = {}
 
     def _queuedevicestatus(self, queue: bool = False, **kwargs: Any) -> Light:
         """Queue an update to the device."""
         if kwargs:
             self._pending.update(kwargs)
         if not queue:
             self._setdevicestatus(**self._pending)
             self._pending = {}
 
         return self
 
-    def update_state(self, status: et.Element) -> None:
-        """Update the device state."""
-        if status.tag == 'DeviceInfo':
-            self.name = status.findtext('FriendlyName')
-
-        capabilities = status.findtext('CapabilityIDs') or status.findtext(
-            'CapabilityID'
-        )
-        currentstate = status.findtext('CurrentState') or status.findtext(
-            'CapabilityValue'
-        )
-
-        if capabilities is not None:
-            self.capabilities = [
-                CAPABILITY_ID2NAME.get(c, c) for c in capabilities.split(',')
-            ]
-        if currentstate is not None:
-            self._values = currentstate.split(',')
-
-        super().update_state(status)
-
     def turn_on(
         self,
         level: int | None = None,
         transition: int = 0,
         force_update: bool = False,
     ) -> Light:
         """Turn on the light."""
         transition_time = limit(int(transition * 10), 0, 65535)
 
         if level == 0:
             return self.turn_off(transition)
-        if 'levelcontrol' in self.capabilities:
+        if "levelcontrol" in self.capabilities:
             # Work around observed fw bugs.
             # - When we set a new brightness level but the bulb is off, it
             #   first turns on at the old brightness and then fades to the new
             #   setting. So we have to force the saved brightness to 0 first.
             # - When we turn a bulb on with levelcontrol the onoff state
             #   doesn't update.
             # - After turning off a bulb with sleepfader, it fails to turn back
@@ -388,27 +428,27 @@
             self.get_state(force_update=force_update)
             # A freshly power cycled bridge has no record of the bulb
             # brightness, so default to full on if the client didn't request
             # a level and we have no record
             if level is None:
                 level = self.state.get("level", 255)
 
-            if self.state['onoff'] == 0:
+            if self.state["onoff"] == 0:
                 self._setdevicestatus(levelcontrol=(0, 0), onoff=ON)
 
             level = limit(int(level), 0, 255)
             return self._queuedevicestatus(
                 levelcontrol=(level, transition_time)
             )
 
         return self._queuedevicestatus(onoff=ON)
 
     def turn_off(self, transition: int = 0) -> Light:
         """Turn off the light."""
-        if transition and 'sleepfader' in self.capabilities:
+        if transition and "sleepfader" in self.capabilities:
             # Sleepfader control did not turn off bulb when fadetime was 0
             transition_time = limit(int(transition * 10), 1, 65535)
             reference = int(time.time())
             return self._queuedevicestatus(
                 sleepfader=(transition_time, reference)
             )
 
@@ -440,43 +480,27 @@
         colory = limit(int(colorxy[1] * 65535), 0, 65535)
         return self._queuedevicestatus(
             colorcontrol=(colorx, colory, transition_time), queue=delay
         )
 
     def start_ramp(self, ramp_up: bool, rate: int) -> Light:
         """Start ramping the brightness up or down."""
-        up_down = '1' if ramp_up else '0'
+        up_down = "1" if ramp_up else "0"
         rate = limit(int(rate), 0, 255)
         return self._queuedevicestatus(levelcontrol_move=(up_down, rate))
 
     def stop_ramp(self) -> LinkedDevice:
         """Start ramping the brightness up or down."""
-        return self._setdevicestatus(levelcontrol_stop='')
+        return self._setdevicestatus(levelcontrol_stop="")
 
 
 class Group(LinkedDevice):
     """Representation of a Group of lights connected to the Bridge."""
 
-    def __init__(self, bridge: Bridge, info: et.Element) -> None:
+    _NAME_TAG = "GroupName"
+    _CAPABILITIES_TAGS = ("GroupCapabilityIDs", "CapabilityID")
+    _VALUES_TAGS = ("GroupCapabilityValues", "CapabilityValue")
+
+    def __init__(self, bridge: Bridge, info: et._Element) -> None:
         """Create a Group device."""
         super().__init__(bridge, info)
-        self.uniqueID = info.findtext('GroupID')
-
-    def update_state(self, status: et.Element) -> None:
-        """Update the device state."""
-        if status.tag == 'GroupInfo':
-            self.name = status.findtext('GroupName')
-
-        capabilities = status.findtext(
-            'GroupCapabilityIDs'
-        ) or status.findtext('CapabilityID')
-        currentstate = status.findtext(
-            'GroupCapabilityValues'
-        ) or status.findtext('CapabilityValue')
-
-        if capabilities is not None:
-            self.capabilities = [
-                CAPABILITY_ID2NAME.get(c, c) for c in capabilities.split(',')
-            ]
-        if currentstate is not None:
-            self._values = currentstate.split(',')
-        super().update_state(status)
+        self.uniqueID: str = info.findtext("GroupID", "")
```

### Comparing `pywemo-0.9.2/pywemo/ouimeaux_device/coffeemaker.py` & `pywemo-1.0.0/pywemo/ouimeaux_device/coffeemaker.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Representation of a WeMo CoffeeMaker device."""
 from __future__ import annotations
 
 from enum import IntEnum
-from typing import Any
+from typing import Any, TypedDict
 
 from .api.attributes import AttributeDevice
 
 _UNKNOWN = -1
 
 
 # These enums were derived from the
@@ -42,23 +42,28 @@
     CoffeeMakerMode.Brewed: "Brewed",
     CoffeeMakerMode.CleaningBrewing: "CleaningBrewing",
     CoffeeMakerMode.CleaningSoaking: "CleaningSoaking",
     CoffeeMakerMode.BrewFailCarafeRemoved: "BrewFailCarafeRemoved",
 }
 
 
+class _Attributes(TypedDict, total=False):
+    Mode: int
+
+
 class CoffeeMaker(AttributeDevice):
     """Representation of a WeMo CoffeeMaker device."""
 
     _state_property = "mode"  # Required by AttributeDevice.
+    _attributes: _Attributes  # Required by AttributeDevice.
 
     @property
     def mode(self) -> CoffeeMakerMode:
         """Return the mode of the device."""
-        return CoffeeMakerMode(int(self._attributes.get("Mode", _UNKNOWN)))
+        return CoffeeMakerMode(self._attributes.get("Mode", _UNKNOWN))
 
     @property
     def mode_string(self) -> str:
         """Return the mode of the device as a string."""
         return MODE_NAMES.get(self.mode, "Unknown")
 
     def get_state(self, force_update: bool = False) -> int:
```

### Comparing `pywemo-0.9.2/pywemo/ouimeaux_device/crockpot.py` & `pywemo-1.0.0/pywemo/ouimeaux_device/crockpot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """Representation of a WeMo CrockPot device."""
 from __future__ import annotations
 
+import logging
 from enum import IntEnum
-from typing import Any
+from typing import Any, TypedDict
 
 from .api.service import RequiredService
 from .switch import Switch
 
 _UNKNOWN = -1
 
+LOG = logging.getLogger(__name__)
+
 
 # These enums were derived from the CrockPot.basicevent.GetCrockpotState()
 # service call. Thus these names/values were not chosen randomly and the
 # numbers have meaning.
 class CrockPotMode(IntEnum):
     """Modes for the CrockPot."""
 
@@ -32,25 +35,35 @@
     CrockPotMode.Off: "Turned Off",
     CrockPotMode.Warm: "Warm",
     CrockPotMode.Low: "Low",
     CrockPotMode.High: "High",
 }
 
 
+class _Attributes(TypedDict, total=False):
+    """CrockPot state dictionary type."""
+
+    cookedTime: int
+    mode: int
+    time: int
+
+
 class CrockPot(Switch):
     """WeMo Crockpot."""
 
     EVENT_TYPE_COOKED_TIME = "cookedTime"
     EVENT_TYPE_MODE = "mode"
     EVENT_TYPE_TIME = "time"
 
+    _attributes: _Attributes
+
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         """Create a WeMo CrockPot device."""
         super().__init__(*args, **kwargs)
-        self._attributes: dict[str, str] = {}
+        self._attributes = {}
         self.get_state(True)
 
     @property
     def _required_services(self) -> list[RequiredService]:
         return super()._required_services + [
             RequiredService(
                 name="basicevent",
@@ -59,55 +72,63 @@
         ]
 
     def update_attributes(self) -> None:
         """Request state from device."""
         state_attributes = self.basicevent.GetCrockpotState()
 
         # Only update our state on complete updates from the device
-        if all(
-            state_attributes.get(attr) is not None
-            for attr in ("cookedTime", "mode", "time")
-        ):
-            self._attributes = state_attributes
+        try:
+            self._attributes = {
+                "cookedTime": int(state_attributes["cookedTime"]),
+                "mode": int(state_attributes["mode"]),
+                "time": int(state_attributes["time"]),
+            }
+        except KeyError as err:
+            LOG.error("Missing expected state attribute: %r", err)
+        except ValueError as err:
+            LOG.error("Invalid state value: %r", err)
+        else:
             self._state = self.mode
 
     def subscription_update(self, _type: str, _params: str) -> bool:
         """Handle reports from device."""
-        if _type == self.EVENT_TYPE_MODE:
-            self._attributes['mode'] = _params
-            self._state = self.mode
-            return True
-        if _type == self.EVENT_TYPE_TIME:
-            self._attributes['time'] = _params
-            return True
-        if _type == self.EVENT_TYPE_COOKED_TIME:
-            self._attributes['cookedTime'] = _params
-            return True
-
+        try:
+            if _type == self.EVENT_TYPE_MODE:
+                self._attributes["mode"] = int(_params)
+                self._state = self.mode
+                return True
+            if _type == self.EVENT_TYPE_TIME:
+                self._attributes["time"] = int(_params)
+                return True
+            if _type == self.EVENT_TYPE_COOKED_TIME:
+                self._attributes["cookedTime"] = int(_params)
+                return True
+        except ValueError as err:
+            LOG.error("Invalid value for %s: %r", _type, err)
         return super().subscription_update(_type, _params)
 
     @property
     def mode(self) -> CrockPotMode:
         """Return the mode of the device."""
-        return CrockPotMode(int(self._attributes.get('mode', _UNKNOWN)))
+        return CrockPotMode(self._attributes.get("mode", _UNKNOWN))
 
     @property
     def mode_string(self) -> str:
         """Return the mode of the device as a string."""
         return MODE_NAMES.get(self.mode, "Unknown")
 
     @property
     def remaining_time(self) -> int:
         """Return the remaining time in minutes."""
-        return int(self._attributes.get('time', 0))
+        return self._attributes.get("time", 0)
 
     @property
     def cooked_time(self) -> int:
         """Return the cooked time in minutes."""
-        return int(self._attributes.get('cookedTime', 0))
+        return self._attributes.get("cookedTime", 0)
 
     def get_state(self, force_update: bool = False) -> int:
         """Return 0 if off and 1 if on."""
         # The base implementation using GetBinaryState doesn't work for
         # CrockPot (always returns 0) so use mode instead.
         if force_update or self._attributes.get("mode") is None:
             self.update_attributes()
```

### Comparing `pywemo-0.9.2/pywemo/ouimeaux_device/dimmer.py` & `pywemo-1.0.0/pywemo/ouimeaux_device/dimmer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """Representation of a WeMo Dimmer device."""
 from __future__ import annotations
 
-import warnings
-
 from .api.long_press import LongPressMixin
 from .api.service import RequiredService
 from .switch import Switch
 
 
 class Dimmer(Switch):
     """Representation of a WeMo Dimmer device."""
@@ -23,23 +21,14 @@
         """Get brightness from device."""
         self.get_state(force_update)
         assert self._brightness is not None
         return self._brightness
 
     def set_brightness(self, brightness: int) -> None:
         """Set the brightness of this device to an integer between 1-100."""
-        if not isinstance(brightness, int):
-            warnings.warn(  # type: ignore[unreachable]
-                "The brightness argument to Dimmer.set_brightness must be an "
-                "int. Support for non-int values will be dropped in a future "
-                "pyWeMo release.",
-                DeprecationWarning,
-            )
-            brightness = int(brightness)
-
         # WeMo only supports values between 1-100. WeMo will ignore a 0
         # brightness value. If 0 is requested, then turn the light off instead.
         if brightness:
             self.basicevent.SetBinaryState(
                 BinaryState=1, brightness=brightness
             )
             self._state = 1
```

### Comparing `pywemo-0.9.2/pywemo/ouimeaux_device/humidifier.py` & `pywemo-1.0.0/pywemo/ouimeaux_device/humidifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Representation of a WeMo Humidifier device."""
 from __future__ import annotations
 
 from enum import IntEnum
-from typing import Any
+from typing import Any, TypedDict
 
 from .api.attributes import AttributeDevice
 
 _UNKNOWN = -1
 
 
 # These enums were derived from Humidifier.deviceevent.GetAttributeList() and
@@ -77,73 +77,84 @@
     WaterLevel.Low: "Low",
     WaterLevel.Good: "Good",
 }
 
 FILTER_LIFE_MAX = 60480
 
 
+class _Attributes(TypedDict, total=False):
+    FanMode: int
+    DesiredHumidity: int
+    CurrentHumidity: float
+    NoWater: int
+    WaterAdvise: int
+    FilterLife: float
+    ExpiredFilterTime: int
+
+
 class Humidifier(AttributeDevice):
     """Representation of a WeMo Humidifier device."""
 
     _state_property = "fan_mode"  # Required by AttributeDevice.
+    _attributes: _Attributes  # Required by AttributeDevice.
 
     @property
     def fan_mode(self) -> FanMode:
         """Return the FanMode setting (as an int index of the IntEnum)."""
-        return FanMode(int(self._attributes.get("FanMode", _UNKNOWN)))
+        return FanMode(self._attributes.get("FanMode", _UNKNOWN))
 
     @property
     def fan_mode_string(self) -> str:
         """Return the FanMode setting as a string.
 
         (Off, Low, Medium, High, Maximum).
         """
         return FAN_MODE_NAMES.get(self.fan_mode, "Unknown")
 
     @property
     def desired_humidity(self) -> DesiredHumidity:
         """Return the desired humidity (as an int index of the IntEnum)."""
         return DesiredHumidity(
-            int(self._attributes.get("DesiredHumidity", _UNKNOWN))
+            self._attributes.get("DesiredHumidity", _UNKNOWN)
         )
 
     @property
     def desired_humidity_percent(self) -> str:
         """Return the desired humidity in percent (string)."""
         return DESIRED_HUMIDITY_NAMES.get(self.desired_humidity, "Unknown")
 
     @property
     def current_humidity_percent(self) -> float:
         """Return the observed relative humidity in percent (float)."""
-        return float(self._attributes.get("CurrentHumidity", 0.0))
+        return self._attributes.get("CurrentHumidity", 0.0)
 
     @property
     def water_level(self) -> WaterLevel:
         """Return 0 if water level is Empty, 1 if Low, and 2 if Good."""
-        if self._attributes.get("NoWater") == "1":
+        if self._attributes.get("NoWater") == 1:
             return WaterLevel.Empty
-        if self._attributes.get("WaterAdvise") == "1":
+        if self._attributes.get("WaterAdvise") == 1:
             return WaterLevel.Low
         return WaterLevel.Good
 
     @property
     def water_level_string(self) -> str:
         """Return Empty, Low, or Good depending on the water level."""
         return WATER_LEVEL_NAMES.get(self.water_level, "Unknown")
 
     @property
     def filter_life_percent(self) -> float:
         """Return the percentage (float) of filter life remaining."""
-        filter_life = float(self._attributes.get("FilterLife", 0.0))
+        filter_life = self._attributes.get("FilterLife", 0.0)
         return round(filter_life / float(FILTER_LIFE_MAX) * 100.0, 2)
 
     @property
     def filter_expired(self) -> bool:
         """Return False if filter is OK, or True if it needs to be changed."""
-        return bool(int(self._attributes.get("ExpiredFilterTime", 0)))
+        return bool(self._attributes.get("ExpiredFilterTime", 0))
 
     def get_state(self, force_update: bool = False) -> int:
         """Return 0 if off and 1 if on."""
         # The base implementation using GetBinaryState
         # doesn't work for Humidifier (always returns 0)
         # so use fan mode instead.
         # Consider the Humidifier to be "on" if it's not off.
```

### Comparing `pywemo-0.9.2/pywemo/ouimeaux_device/insight.py` & `pywemo-1.0.0/pywemo/ouimeaux_device/insight.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """Representation of a WeMo Insight device."""
 from __future__ import annotations
 
 import logging
-import sys
-import warnings
 from datetime import datetime
 from enum import IntEnum
-from typing import Any
+from typing import Any, TypedDict
 
 from .api.service import RequiredService
 from .switch import Switch
 
 LOG = logging.getLogger(__name__)
 
 
@@ -23,36 +21,27 @@
     STANDBY = 8
 
     @classmethod
     def _missing_(cls, value: Any) -> StandbyState:
         return cls._UNKNOWN
 
 
-if sys.version_info >= (3, 8):
-    # Remove pylint disable when Python 3.7 support is removed.
-    from typing import TypedDict  # pylint: disable=no-name-in-module
-
-    class InsightParams(TypedDict):
-        """Energy related parameters for Insight devices."""
-
-        state: str
-        lastchange: datetime
-        onfor: int
-        ontoday: int
-        ontotal: int
-        todaymw: int
-        totalmw: int
-        currentpower: int
-        wifipower: int
-        powerthreshold: int
+class InsightParams(TypedDict):
+    """Energy related parameters for Insight devices."""
 
-else:
-    from typing import Dict, Union
-
-    InsightParams = Dict[str, Union[str, datetime, int]]
+    state: str
+    lastchange: datetime
+    onfor: int
+    ontoday: int
+    ontotal: int
+    todaymw: int
+    totalmw: int
+    currentpower: int
+    wifipower: int
+    powerthreshold: int
 
 
 class Insight(Switch):
     """Representation of a WeMo Insight device."""
 
     EVENT_TYPE_INSIGHT_PARAMS = "InsightParams"
     insight_params: InsightParams
@@ -66,23 +55,31 @@
     def _required_services(self) -> list[RequiredService]:
         return super()._required_services + [
             RequiredService(name="insight", actions=["GetInsightParams"]),
         ]
 
     def update_insight_params(self) -> None:
         """Get and parse the device attributes."""
-        params = self.insight.GetInsightParams().get('InsightParams')
+        params = self.insight.GetInsightParams().get("InsightParams")
         assert params
         self.insight_params = self.parse_insight_params(params)
 
     def subscription_update(self, _type: str, _params: str) -> bool:
         """Update the device attributes due to a subscription update event."""
         LOG.debug("subscription_update %s %s", _type, _params)
         if _type == self.EVENT_TYPE_INSIGHT_PARAMS:
-            self.insight_params = self.parse_insight_params(_params)
+            try:
+                self.insight_params = self.parse_insight_params(_params)
+            except ValueError:
+                LOG.error(
+                    "Unexpected %s value `%s` for device %s.",
+                    self.EVENT_TYPE_INSIGHT_PARAMS,
+                    _params,
+                    self.name,
+                )
             return True
         updated = super().subscription_update(_type, _params)
         if _type == self.EVENT_TYPE_BINARY_STATE and updated:
             # Special case: When an Insight device turns off, it also stops
             # sending InsightParams updates. Return False in this case to
             # indicate that the current state of the device hasn't been fully
             # updated.
@@ -100,26 +97,26 @@
             ontotal,  # seconds
             _timeperiod,
             wifipower,  # wifi rssi signal strength
             currentmw,
             todaymw,
             totalmw,
             powerthreshold,
-        ) = params.split('|')
+        ) = params.split("|")
         return {
-            'state': state,
-            'lastchange': datetime.fromtimestamp(int(lastchange)),
-            'onfor': int(onfor),
-            'ontoday': int(ontoday),
-            'ontotal': int(ontotal),
-            'todaymw': int(float(todaymw)),
-            'totalmw': int(float(totalmw)),
-            'currentpower': int(float(currentmw)),
-            'wifipower': int(float(wifipower)),
-            'powerthreshold': int(float(powerthreshold)),
+            "state": state,
+            "lastchange": datetime.fromtimestamp(int(lastchange)),
+            "onfor": int(onfor),
+            "ontoday": int(ontoday),
+            "ontotal": int(ontotal),
+            "todaymw": int(float(todaymw)),
+            "totalmw": int(float(totalmw)),
+            "currentpower": int(float(currentmw)),
+            "wifipower": int(float(wifipower)),
+            "powerthreshold": int(float(powerthreshold)),
         }
 
     def get_state(self, force_update: bool = False) -> int:
         """Return the device state."""
         if force_update or self._state is None:
             self.update_insight_params()
 
@@ -129,88 +126,66 @@
         """Set the state of this device to on or off."""
         super().set_state(state)
         self.get_state(force_update=True)  # Refresh the insight params.
 
     @property
     def today_kwh(self) -> float:
         """Return the number of kWh consumed today."""
-        return float(self.insight_params['todaymw']) * 1.6666667e-8
+        return float(self.insight_params["todaymw"]) * 1.6666667e-8
 
     @property
     def total_kwh(self) -> float:
         """Return the total kWh consumed for the device."""
-        return float(self.insight_params['totalmw']) * 1.6666667e-8
+        return float(self.insight_params["totalmw"]) * 1.6666667e-8
 
     @property
     def current_power(self) -> int:
         """Return the current power usage in mW."""
-        return self.insight_params['currentpower']
+        return self.insight_params["currentpower"]
 
     @property
     def current_power_watts(self) -> float:
         """Return the current power usage in Watts."""
         return float(self.current_power) / 1000.0
 
     @property
     def wifi_power(self) -> int:
         """Return the current rssi wifi signal."""
-        return self.insight_params['wifipower']
+        return self.insight_params["wifipower"]
 
     @property
     def threshold_power(self) -> int:
         """Return the threshold power in mW.
 
         Above this the device is on, below it is standby.
         """
-        return self.insight_params['powerthreshold']
+        return self.insight_params["powerthreshold"]
 
     @property
     def threshold_power_watts(self) -> float:
         """Return the threshold power in watts."""
         return float(self.threshold_power) / 1000.0
 
     @property
     def today_on_time(self) -> int:
         """Return the number of seconds the device has been on today."""
-        return self.insight_params['ontoday']
-
-    @property
-    def today_standby_time(self) -> int:
-        """Return how long the device has been in standby today."""
-        warnings.warn(
-            "The Insight.today_standby_time property should not be used and "
-            "will be removed in a future version of pyWeMo. Switch to using "
-            "the Insight.today_on_time property instead.",
-            DeprecationWarning,
-        )
-        return self.insight_params['ontoday']
+        return self.insight_params["ontoday"]
 
     @property
     def total_on_time(self) -> int:
         """Return the number of seconds the device has been on."""
-        return self.insight_params['ontotal']
+        return self.insight_params["ontotal"]
 
     @property
     def on_for(self) -> int:
         """Return the number of seconds the device was last on for."""
-        return self.insight_params['onfor']
+        return self.insight_params["onfor"]
 
     @property
     def last_change(self) -> datetime:
         """Return the last change datetime."""
-        return self.insight_params['lastchange']
+        return self.insight_params["lastchange"]
 
     @property
     def standby_state(self) -> StandbyState:
         """Return the standby state of the device."""
-        return StandbyState(int(self.insight_params['state']))
-
-    @property
-    def get_standby_state(self) -> str:
-        """Return the standby state of the device."""
-        warnings.warn(
-            "The Insight.get_standby_state property should not be used and "
-            "will be removed in a future version of pyWeMo. Switch to using "
-            "the Insight.standby_state property instead.",
-            DeprecationWarning,
-        )
-        return self.standby_state.name.lower()
+        return StandbyState(int(self.insight_params["state"]))
```

### Comparing `pywemo-0.9.2/pywemo/ouimeaux_device/switch.py` & `pywemo-1.0.0/pywemo/ouimeaux_device/switch.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,14 @@
         self.basicevent.SetBinaryState(BinaryState=int(state))
         self._state = int(state)
 
     def off(self) -> None:
         """Turn this device off. If already off, will return "Error"."""
         self.set_state(0)
 
-    def on(self) -> None:
+    def on(self) -> None:  # pylint: disable=invalid-name
         """Turn this device on. If already on, will return "Error"."""
         self.set_state(1)
 
     def toggle(self) -> None:
         """Toggle the switch's state."""
         self.set_state(not self.get_state())
```

### Comparing `pywemo-0.9.2/pywemo/ssdp.py` & `pywemo-1.0.0/pywemo/ssdp.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,267 +2,95 @@
 from __future__ import annotations
 
 import logging
 import re
 import select
 import socket
 import threading
-import warnings
 from datetime import datetime, timedelta
-from typing import Any
-
-import requests
-from lxml import etree as et
 
 from .ouimeaux_device.api.long_press import VIRTUAL_DEVICE_UDN
-from .ouimeaux_device.api.service import REQUESTS_TIMEOUT
-from .util import etree_to_dict, get_callback_address, interface_addresses
+from .util import get_callback_address, interface_addresses
 
 DISCOVER_TIMEOUT = 5
 
 LOG = logging.getLogger(__name__)
 
-RESPONSE_REGEX = re.compile(r'\n(.*)\: (.*)\r')
+RESPONSE_REGEX = re.compile(r"\n(.*)\: (.*)\r")
 
 MIN_TIME_BETWEEN_SCANS = timedelta(seconds=59)
 
 MULTICAST_GROUP = "239.255.255.250"
 MULTICAST_PORT = 1900
 
 # Wemo specific urn:
 ST = "urn:Belkin:service:basicevent:1"
-VIRTUAL_DEVICE_USN = f'{VIRTUAL_DEVICE_UDN}::{ST}'
+VIRTUAL_DEVICE_USN = f"{VIRTUAL_DEVICE_UDN}::{ST}"
 
 SSDP_REPLY = f"""HTTP/1.1 200 OK
 CACHE-CONTROL: max-age=86400
 EXT:
 LOCATION: http://%s/setup.xml
 OPT: "http://schemas.upnp.org/upnp/1/0/"; ns=01
 ST: {ST}
 USN: {VIRTUAL_DEVICE_USN}
 
 """  # Newline characters at the the end of SSDP_REPLY are intentional.
-SSDP_REPLY = SSDP_REPLY.replace('\n', '\r\n')
+SSDP_REPLY = SSDP_REPLY.replace("\n", "\r\n")
 
 SSDP_NOTIFY = f"""NOTIFY * HTTP/1.1
 HOST: {MULTICAST_GROUP}:{MULTICAST_PORT}
 CACHE-CONTROL: max-age=1800
 LOCATION: http://%s/setup.xml
 SERVER: Unspecified, UPnP/1.0, Unspecified
 NT: {ST}
 NTS: ssdp:alive
 USN: {VIRTUAL_DEVICE_USN}
 
 """  # Newline characters at the the end of SSDP_NOTIFY are intentional.
-SSDP_NOTIFY = SSDP_NOTIFY.replace('\n', '\r\n')
+SSDP_NOTIFY = SSDP_NOTIFY.replace("\n", "\r\n")
 
 EXPECTED_ST_HEADER = ("ST: " + ST).encode("UTF-8")
 EXPECTED_MAN_HEADER = b'MAN: "ssdp:discover"'
 
 
-class SSDP:
-    """Controls the scanning of uPnP devices and services and caches output."""
-
-    def __init__(self) -> None:
-        """Create SSDP object."""
-        self.entries: list[UPNPEntry] = []
-        self.last_scan: datetime | None = None
-        self._lock = threading.RLock()
-        warnings.warn(
-            "pywemo.ssdp.SSDP is unused within pywemo and will be removed in "
-            "a future release.",
-            DeprecationWarning,
-        )
-
-    def scan(self) -> None:
-        """Scan the network."""
-        with self._lock:
-            self.update()
-
-    def all(self) -> list[UPNPEntry]:
-        """
-        Return all found entries.
-
-        Will scan for entries if not scanned recently.
-        """
-        with self._lock:
-            self.update()
-
-            return list(self.entries)
-
-    def find_by_st(self, st: str) -> list[UPNPEntry]:
-        """Return a list of entries that match the ST."""
-        with self._lock:
-            self.update()
-
-            return [entry for entry in self.entries if entry.st == st]
-
-    def find_by_device_description(
-        self, values: dict[str, Any]
-    ) -> list[UPNPEntry]:
-        """
-        Return a list of entries that match the description.
-
-        Pass in a dict with values to match against the device tag in the
-        description.
-        """
-        with self._lock:
-            self.update()
-
-            return [
-                entry
-                for entry in self.entries
-                if entry.match_device_description(values)
-            ]
-
-    def update(self, force_update: bool = False) -> None:
-        """Scan for new uPnP devices and services."""
-        with self._lock:
-            if (
-                self.last_scan is None
-                or force_update
-                or datetime.now() - self.last_scan > MIN_TIME_BETWEEN_SCANS
-            ):
-                self.remove_expired()
-
-                self.entries.extend(
-                    entry
-                    for entry in scan() + scan(ST)
-                    if entry not in self.entries
-                )
-
-                self.last_scan = datetime.now()
-
-    def remove_expired(self) -> None:
-        """Filter out expired entries."""
-        with self._lock:
-            self.entries = [
-                entry for entry in self.entries if not entry.is_expired
-            ]
-
-
 class UPNPEntry:
     """Found uPnP entry."""
 
-    # Use functools.cached_property if Python < 3.8 support is dropped.
-    _description: dict[str, Any] | None = None
-
     def __init__(self, values: dict[str, str]) -> None:
         """Create a UPNPEntry object."""
         self.values = values
         self._created = datetime.now()
         self._expires: datetime | None = None
 
-        if 'cache-control' in self.values:
-            cache_seconds = int(self.values['cache-control'].split('=')[1])
+        if "cache-control" in self.values:
+            cache_seconds = int(self.values["cache-control"].split("=")[1])
 
             self._expires = self._created + timedelta(seconds=cache_seconds)
 
     @property
-    def created(self) -> datetime:
-        """Return timestamp for when this entry was created."""
-        warnings.warn(
-            "pywemo.ssdp.UPNPEntry.created is unused within pywemo and "
-            "will be removed in a future release.",
-            DeprecationWarning,
-        )
-        return self._created
-
-    @property
-    def expires(self) -> datetime | None:
-        """Return timestamp for when this entry expires."""
-        warnings.warn(
-            "pywemo.ssdp.UPNPEntry.expires is unused within pywemo and "
-            "will be removed in a future release.",
-            DeprecationWarning,
-        )
-        return self._expires
-
-    @property
-    def is_expired(self) -> bool:
-        """Return whether the entry is expired or not."""
-        warnings.warn(
-            "pywemo.ssdp.UPNPEntry.is_expired is unused within pywemo and "
-            "will be removed in a future release.",
-            DeprecationWarning,
-        )
-        return self.expires is not None and datetime.now() > self.expires
-
-    @property
-    def st(self) -> str | None:
+    def st(self) -> str | None:  # pylint: disable=invalid-name
         """Return ST value."""
-        return self.values.get('st')
+        return self.values.get("st")
 
     @property
     def location(self) -> str | None:
         """Return location value."""
-        return self.values.get('location')
+        return self.values.get("location")
 
     @property
     def usn(self) -> str | None:
         """Return unique service name."""
-        return self.values.get('usn')
+        return self.values.get("usn")
 
     @property
     def udn(self) -> str:
         """Return unique device name."""
-        usn = self.usn or ''
-        return usn.split('::')[0]
-
-    @property
-    def description(self) -> dict[str, Any]:
-        """Return the description from the uPnP entry."""
-        # The description property may be referenced multiple times. Cache the
-        # description to avoid needing to fetch it each time the property is
-        # accessed.
-        if self._description is not None:
-            return self._description
-        self._description = {}
-        warnings.warn(
-            "pywemo.ssdp.UPNPEntry.description is unused within pywemo and "
-            "will be removed in a future release.",
-            DeprecationWarning,
-        )
-
-        url = self.location
-        if not url:
-            return {}
-
-        try:
-            for _ in range(3):
-                try:
-                    xml = requests.get(url, timeout=REQUESTS_TIMEOUT).content
-                    tree = et.fromstring(xml or b'')
-                    root: dict[str, Any] = etree_to_dict(tree).get('root', {})
-                    self._description = root
-                    break
-                except requests.RequestException:
-                    LOG.warning("Error fetching description at %s", url)
-
-        except et.ParseError:
-            # There used to be a log message here to record an error about
-            # malformed XML, but this only happens on non-WeMo devices
-            # and can be safely ignored.
-            pass
-
-        return self._description
-
-    def match_device_description(self, values: dict[str, Any]) -> bool:
-        """
-        Fetch description and match against it.
-
-        Values should only contain lowercase keys.
-        """
-        warnings.warn(
-            "pywemo.ssdp.UPNPEntry.match_device_description is unused within "
-            "pywemo and will be removed in a future release.",
-            DeprecationWarning,
-        )
-        device = self.description.get('device', {})
-        return all(val == device.get(key) for key, val in values.items())
+        usn = self.usn or ""
+        return usn.split("::")[0]
 
     @classmethod
     def from_response(cls, response: str) -> UPNPEntry:
         """Create a uPnP entry from a response."""
         return UPNPEntry(
             {
                 key.lower(): item
@@ -277,41 +105,41 @@
 
     def __eq__(self, other: object) -> bool:
         """Equality operator."""
         return isinstance(other, type(self)) and self._key == other._key
 
     def __hash__(self) -> int:
         """Generate hash of instance."""
-        return hash(('UPNPEntry', self._key))
+        return hash(("UPNPEntry", self._key))
 
     def __repr__(self) -> str:
         """Return the string representation of the object."""
-        st = self.st or ''
-        location = self.location or ''
-        udn = self.udn or ''
+        st = self.st or ""  # pylint: disable=invalid-name
+        location = self.location or ""
+        udn = self.udn or ""
         return f"<UPNPEntry {st} - {location} - {udn}>"
 
 
 def build_ssdp_request(ssdp_st: str, ssdp_mx: int) -> bytes:
     """Build the standard request to send during SSDP discovery."""
     return "\r\n".join(
         [
-            'M-SEARCH * HTTP/1.1',
-            f'ST: {ssdp_st}',
-            f'MX: {ssdp_mx}',
+            "M-SEARCH * HTTP/1.1",
+            f"ST: {ssdp_st}",
+            f"MX: {ssdp_mx}",
             'MAN: "ssdp:discover"',
-            f'HOST: {MULTICAST_GROUP}:{MULTICAST_PORT}',
-            '',
-            '',
+            f"HOST: {MULTICAST_GROUP}:{MULTICAST_PORT}",
+            "",
+            "",
         ]
-    ).encode('ascii')
+    ).encode("ascii")
 
 
-def scan(
-    st: str = ST,
+def scan(  # pylint: disable=too-many-branches,too-many-locals
+    st: str = ST,  # pylint: disable=invalid-name
     timeout: float = DISCOVER_TIMEOUT,
     max_entries: int | None = None,
     match_udn: str | None = None,
 ) -> list[UPNPEntry]:
     """
     Send a message over the network to discover upnp devices.
 
@@ -325,40 +153,40 @@
 
     calc_now = datetime.now
 
     ssdp_request = build_ssdp_request(st, ssdp_mx=1)
     sockets = []
     try:
         for addr in interface_addresses():
-            s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+            sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
             try:
-                s.bind((addr, 0))
-                s.sendto(ssdp_request, ssdp_target)
-                sockets.append(s)
+                sock.bind((addr, 0))
+                sock.sendto(ssdp_request, ssdp_target)
+                sockets.append(sock)
             except OSError:
                 pass
             finally:
-                if s not in sockets:
-                    s.close()
+                if sock not in sockets:
+                    sock.close()
 
         start = calc_now()
         while sockets:
             time_diff = calc_now() - start
 
             seconds_left = max(timeout - time_diff.seconds, 0)
 
             ready = select.select(sockets, [], [], min(1, seconds_left))[0]
             if not ready:
                 # Only check for timeout when there are no more results. Exit
                 # if the time has expired, or probe again if there is more
                 # time remaining.
                 if seconds_left <= 0:
                     return entries
-                for s in sockets:
-                    s.sendto(ssdp_request, ssdp_target)
+                for sock in sockets:
+                    sock.sendto(ssdp_request, ssdp_target)
 
             for sock in ready:
                 response = sock.recv(1024).decode("UTF-8", "replace")
 
                 entry = UPNPEntry.from_response(response)
                 if entry.usn == VIRTUAL_DEVICE_USN:
                     continue  # Don't return the virtual device.
@@ -372,16 +200,16 @@
 
                     # Return if we've found the max number of devices
                     if max_entries and len(entries) == max_entries:
                         return entries
     except OSError:
         LOG.exception("Socket error while discovering SSDP devices")
     finally:
-        for s in sockets:
-            s.close()
+        for sock in sockets:
+            sock.close()
 
     return entries
 
 
 class DiscoveryResponder:
     """Inform Wemo devices of the pywemo virtual Wemo device.
 
@@ -495,15 +323,15 @@
 
     def start(self) -> None:
         """Start the server."""
         self._exit.clear()
         self._thread_exception = None
         self._thread = threading.Thread(
             target=self.respond_to_discovery,
-            name='Wemo DiscoveryResponder Thread',
+            name="Wemo DiscoveryResponder Thread",
         )
         self._thread.start()
 
     def stop(self) -> None:
         """Stop the server."""
         if self._thread:
             self._exit.set()
```

### Comparing `pywemo-0.9.2/pywemo/subscribe.py` & `pywemo-1.0.0/pywemo/subscribe.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,40 @@
-"""Module to listen for wemo events."""
+"""Module to listen for WeMo events.
+
+Example usage:
+
+```python
+import pywemo
+# The SubscriptionRegistry maintains push subscriptions to each endpoint
+# of a device.
+registry = pywemo.SubscriptionRegistry()
+registry.start()
+
+device = ... # See example of discovering devices in the pywemo module.
+
+# Start subscribing to push notifications of state changes.
+registry.register(device)
+
+def push_notification(device, event, params):
+    '''Notify device of state change and get new device state.'''
+    processed_update = device.subscription_update(event, params)
+    state = device.get_state(force_update=not processed_update)
+    print(f"Device state: {state}")
+
+# Register a callback to receive state push notifications.
+registry.on(device, None, push_notification)
+
+# Do some work.
+# time.sleep(60)
+
+# Stop the registry
+registry.unregister(device)
+registry.stop()
+```
+"""
 from __future__ import annotations
 
 import collections
 import logging
 import os
 import sched
 import threading
@@ -25,16 +57,16 @@
 # Subscription event types.
 EVENT_TYPE_BINARY_STATE = "BinaryState"
 EVENT_TYPE_INSIGHT_PARAMS = "InsightParams"
 EVENT_TYPE_LONG_PRESS = "LongPress"
 
 LOG = logging.getLogger(__name__)
 NS = "{urn:schemas-upnp-org:event-1-0}"
-RESPONSE_SUCCESS = '<html><body><h1>200 OK</h1></body></html>'
-RESPONSE_NOT_FOUND = '<html><body><h1>404 Not Found</h1></body></html>'
+RESPONSE_SUCCESS = "<html><body><h1>200 OK</h1></body></html>"
+RESPONSE_NOT_FOUND = "<html><body><h1>404 Not Found</h1></body></html>"
 SUBSCRIPTION_RETRY = 60
 
 VIRTUAL_SETUP_XML = f"""<?xml version="1.0"?>
 <root xmlns="urn:Belkin:device-1-0">
   <specVersion>
     <major>1</major>
     <minor>0</minor>
@@ -60,48 +92,86 @@
         <eventSubURL>/upnp/event/basicevent1</eventSubURL>
         <SCPDURL>/eventservice.xml</SCPDURL>
       </service>
     </serviceList>
 </device>
 </root>"""
 
+SOAP_ACTION_RESPONSE = {
+    '"urn:Belkin:service:basicevent:1#GetBinaryState"': """<s:Envelope
+  xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"
+  s:encodingStyle="http://schemas.xmlsoap.org/soap/encoding/">
+<s:Body>
+  <u:GetBinaryStateResponse xmlns:u="urn:Belkin:service:basicevent:1">
+  <BinaryState>0</BinaryState>
+  </u:GetBinaryStateResponse>
+</s:Body></s:Envelope>""",
+    '"urn:Belkin:service:basicevent:1#SetBinaryState"': """<s:Envelope
+  xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"
+  s:encodingStyle="http://schemas.xmlsoap.org/soap/encoding/">
+<s:Body>
+  <u:SetBinaryStateResponse xmlns:u="urn:Belkin:service:basicevent:1">
+    <BinaryState>0</BinaryState>
+  </u:SetBinaryStateResponse>
+</s:Body></s:Envelope>""",
+}
+
+ERROR_SOAP_ACTION_RESPONSE = """<?xml version='1.0' encoding='UTF-8'?>
+<s:Envelope
+  xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"
+  s:encodingStyle="http://schemas.xmlsoap.org/soap/encoding/">
+<s:Body>
+  <s:Fault>
+    <faultcode>SOAP-ENV:Server</faultcode>
+    <faultstring>Unknown Action</faultstring>
+    <detail>The requested SOAP action is not handled by pyWeMo</detail>
+  </s:Fault>
+</s:Body>
+</s:Envelope>"""
+
 
 class Subscription:
     """Subscription to a single UPnP service endpoint."""
 
-    # Scheduler Event used to periodically maintain the subscription.
     scheduler_event: sched.Event | None = None
+    """Scheduler Event used to periodically maintain the subscription."""
 
-    # Controls whether or not the subscription will continue to be periodically
-    # scheduled by the Scheduler. Set to False when the device us unregistered.
     scheduler_active: bool = True
+    """
+    Controls whether or not the subscription will continue to be periodically
+    scheduled by the Scheduler. Set to False when the device us unregistered.
+    """
 
-    # Time that the subscription will expire, or 0.0 if not subscribed.
-    # time.time() value.
     expiration_time: float = 0.0
+    """Time that the subscription will expire, or 0.0 if not subscribed.
+    time.time() value.
+    """
 
-    # Has a notification event been received for this subscription?
     event_received: bool = False
+    """Has a notification event been received for this subscription?"""
 
-    # Subscription Identifier (SID) used to maintain/refresh the subscription.
-    # `None` when the subscription is not active.
     subscription_id: str | None = None
+    """Subscription Identifier (SID) used to maintain/refresh the subscription.
+    `None` when the subscription is not active.
+    """
 
-    # Request that the device keep the subscription active for this number of
-    # seconds.
     default_timeout_seconds: int = 300
+    """
+    Request that the device keep the subscription active for this number of
+    seconds.
+    """
 
-    # WeMo device instance.
     device: Device
+    """WeMo device instance."""
 
-    # HTTP port used by devices to send event notifications.
     callback_port: int
+    """HTTP port used by devices to send event notifications."""
 
-    # Name of the subscription endpoint service.
     service_name: str
+    """Name of the subscription endpoint service."""
 
     def __init__(
         self, device: Device, callback_port: int, service_name: str
     ) -> None:
         """Initialize a new subscription."""
         self.device = device
         self.callback_port = callback_port
@@ -152,57 +222,56 @@
     def _subscribe(self) -> requests.Response:
         """Start/renew a subscription with a UPnP SUBSCRIBE request.
 
         Will renew an existing subscription if one exists, otherwise a new
         subscription will be created.
         """
         if self.subscription_id:  # Renew existing subscription.
-            headers = {'SID': self.subscription_id}
+            headers = {"SID": self.subscription_id}
         else:  # Start a new subscription.
             callback_address = get_callback_address(
                 host=self.device.host,
                 port=self.callback_port,
             )
 
-            callback = f'<http://{callback_address}{self.path}>'
-            headers = {'CALLBACK': callback, 'NT': 'upnp:event'}
-        headers['TIMEOUT'] = f'Second-{self.default_timeout_seconds}'
+            callback = f"<http://{callback_address}{self.path}>"
+            headers = {"CALLBACK": callback, "NT": "upnp:event"}
+        headers["TIMEOUT"] = f"Second-{self.default_timeout_seconds}"
         return requests.request(
-            method='SUBSCRIBE',
+            method="SUBSCRIBE",
             url=self.url,
             headers=headers,
             timeout=REQUESTS_TIMEOUT,
         )
 
     def _unsubscribe(self) -> None:
         """Remove the subscription on the WeMo with a UPnP UNSUBSCRIBE request.
 
         Only sends the UNSUBSCRIBE message if there is an existing
         subscription. Does nothing if there is no subscription.
         """
         if self.subscription_id:
             requests.request(
-                method='UNSUBSCRIBE',
+                method="UNSUBSCRIBE",
                 url=self.url,
-                headers={'SID': self.subscription_id},
+                headers={"SID": self.subscription_id},
                 timeout=REQUESTS_TIMEOUT,
             )
             self.subscription_id = None
 
     def _update_subscription(self, headers: MutableMapping[str, str]) -> int:
         """Update UPnP subscription parameters from SUBSCRIBE response headers.
 
         Returns:
             The duration of the subscription in seconds.
         """
-        self.subscription_id = headers.get('SID', self.subscription_id)
-        timeout_header = headers.get('TIMEOUT', None)
-        if timeout_header:
+        self.subscription_id = headers.get("SID", self.subscription_id)
+        if timeout_header := headers.get("TIMEOUT", None):
             timeout = min(
-                int(timeout_header.replace('Second-', '')),
+                int(timeout_header.replace("Second-", "")),
                 self.default_timeout_seconds,
             )
         else:
             timeout = self.default_timeout_seconds
         self.expiration_time = timeout + time.time()
         return timeout
 
@@ -218,15 +287,15 @@
     def url(self) -> str:
         """URL for the UPnP subscription endoint."""
         return self.device.services[self.service_name].eventSubURL
 
     @property
     def path(self) -> str:
         """Path for the callback to disambiguate multiple subscriptions."""
-        return f'/sub/{self.service_name}'
+        return f"/sub/{self.service_name}"
 
     @property
     def is_subscribed(self) -> bool:
         """Return True if the subscription is active, False otherwise.
 
         Verifies that the subscription is within its expected lifetime and that
         at least one event notification has been received.
@@ -242,26 +311,26 @@
     """ThreadingHTTPServer with an 'outer' attribute."""
 
     outer: SubscriptionRegistry
 
 
 def _start_server(port: int | None) -> HTTPServer:
     """Find a valid open port and start the HTTP server."""
-    requested_port = port or os.getenv('PYWEMO_HTTP_SERVER_PORT')
+    requested_port = port or os.getenv("PYWEMO_HTTP_SERVER_PORT")
     if requested_port is not None:
         start_port = int(requested_port)
         ports_to_check = 1
     else:
         start_port = 8989
         ports_to_check = 128
 
-    for i in range(0, ports_to_check):
-        port = start_port + i
+    for offset in range(0, ports_to_check):
+        port = start_port + offset
         try:
-            return HTTPServer(('', port), RequestHandler)
+            return HTTPServer(("", port), RequestHandler)
         except OSError as error:
             last_error = error
     raise last_error
 
 
 def _cancel_events(
     scheduler: sched.scheduler, subscriptions: Iterable[Subscription]
@@ -322,35 +391,40 @@
       method to update the BinaryState of the virtual device. This doesn't
       actually update any state, rather the virtual device then delivers the
       event notification to any event listeners configured to receive events
       from the pywemo SubscriptionRegistry. The event type for a long press
       action is EVENT_TYPE_LONG_PRESS.
     """
 
-    # Do not wait for more than 10 seconds for any request to complete.
     timeout = 10
+    """Do not wait for more than 10 seconds for any request to complete."""
+
     server: HTTPServer
+    server_version = f"{BaseHTTPRequestHandler.server_version} UPnP/1.0"
 
     def do_NOTIFY(self) -> None:  # pylint: disable=invalid-name
         """Handle subscription responses received from devices."""
         sender_ip, _ = self.client_address
         outer = self.server.outer
-        device = outer.devices.get(sender_ip)
-        if device is None:
+        if (device := outer.devices.get(sender_ip)) is None:
             LOG.warning(
-                'Received %s event for unregistered device %s',
+                "Received %s event for unregistered device %s",
                 self.path,
                 sender_ip,
             )
         else:
             doc = self._get_xml_from_http_body()
-            for propnode in doc.findall(f'./{NS}property'):
+            for propnode in doc.findall(f"./{NS}property"):
                 for property_ in list(propnode):
-                    text = property_.text
-                    outer.event(device, property_.tag, text, path=self.path)
+                    outer.event(
+                        device,
+                        property_.tag,
+                        property_.text or "",
+                        path=self.path,
+                    )
 
         self._send_response(200, RESPONSE_SUCCESS)
 
     def do_GET(self) -> None:  # pylint: disable=invalid-name
         """Handle GET requests for a Virtual WeMo device."""
         if self.path.endswith("/setup.xml"):
             self._send_response(
@@ -360,88 +434,103 @@
             self._send_response(404, RESPONSE_NOT_FOUND)
 
     def do_POST(self) -> None:  # pylint: disable=invalid-name
         """Handle POST requests for a Virtual WeMo device."""
         if self.path.endswith("/upnp/control/basicevent1"):
             sender_ip, _ = self.client_address
             outer = self.server.outer
-            device = outer.devices.get(sender_ip)
-            if device is None:
+            if (device := outer.devices.get(sender_ip)) is None:
                 LOG.warning(
-                    'Received event for unregistered device %s', sender_ip
+                    "Received event for unregistered device %s", sender_ip
                 )
             else:
                 doc = self._get_xml_from_http_body()
-                binary_state = doc.find('.//BinaryState')
-                if binary_state is not None:
-                    text = binary_state.text
-                    outer.event(device, EVENT_TYPE_LONG_PRESS, text)
-            self._send_response(200, RESPONSE_SUCCESS)
+                if binary_state := doc.findtext(".//BinaryState"):
+                    outer.event(device, EVENT_TYPE_LONG_PRESS, binary_state)
+            action = self.headers.get("SOAPACTION", "")
+            response = SOAP_ACTION_RESPONSE.get(
+                action, ERROR_SOAP_ACTION_RESPONSE
+            )
+            self._send_response(
+                200, response, content_type='text/xml; charset="utf-8"'
+            )
         else:
             self._send_response(404, RESPONSE_NOT_FOUND)
 
     def do_SUBSCRIBE(self) -> None:  # pylint: disable=invalid-name
         """Handle SUBSCRIBE requests for a Virtual WeMo device."""
         if self.path.endswith("/upnp/event/basicevent1"):
             self.send_response(200)
             self.send_header("CONTENT-LENGTH", "0")
             self.send_header("TIMEOUT", "Second-1801")
             # Using a randomly generated valid UUID (uuid.uuid4()).
             self.send_header(
                 "SID", "uuid:a74b23d5-34b9-4f71-9f87-bed24353f304"
             )
-            self.send_header('Connection', 'close')
+            self.send_header("Connection", "close")
+            self.end_headers()
+        else:
+            self._send_response(404, RESPONSE_NOT_FOUND)
+
+    def do_UNSUBSCRIBE(self) -> None:  # pylint: disable=invalid-name
+        """Handle UNSUBSCRIBE requests for a Virtual WeMo device."""
+        if self.path.endswith("/upnp/event/basicevent1"):
+            self.send_response(200)
+            self.send_header("CONTENT-LENGTH", "0")
+            self.send_header("Connection", "close")
             self.end_headers()
         else:
             self._send_response(404, RESPONSE_NOT_FOUND)
 
     def _send_response(
         self, code: int, body: str, *, content_type: str = "text/html"
     ) -> None:
         self.send_response(code)
-        self.send_header('Content-Type', content_type)
-        self.send_header('Content-Length', str(len(body)))
-        self.send_header('Connection', 'close')
+        self.send_header("Content-Type", content_type)
+        self.send_header("Content-Length", str(len(body)))
+        self.send_header("Connection", "close")
         self.end_headers()
         if body:
             self.wfile.write(body.encode("UTF-8"))
 
-    def _get_xml_from_http_body(self) -> et.Element:
+    def _get_xml_from_http_body(self) -> et._Element:
         """Build the element tree root from the body of the http request."""
-        content_len = int(self.headers.get('content-length', 0))
+        content_len = int(self.headers.get("content-length", 0))
         data = self.rfile.read(content_len)
         # trim garbage from end, if any
         data = data.strip()
-        return et.fromstring(data)
+        return et.fromstring(data, parser=et.XMLParser(resolve_entities=False))
 
     # pylint: disable=redefined-builtin
     def log_message(self, format: str, *args: Any) -> None:
         """Disable error logging."""
         return
 
 
 SubscriberCallback = Callable[[Device, str, str], Any]
 
 
-class SubscriptionRegistry:
+class SubscriptionRegistry:  # pylint: disable=too-many-instance-attributes
     """Holds device subscriptions and callbacks for wemo events."""
 
-    # Potential service endpoints for subscriptions. A Subscription will be
-    # created for each entry as long as the service is supported by the device.
     subscription_service_names: Iterable[str] = (
-        'basicevent',
-        'bridge',
-        'insight',
+        "basicevent",
+        "bridge",
+        "insight",
     )
+    """Potential service endpoints for subscriptions.
+    A Subscription will be created for each entry as long as the service is
+    supported by the device.
+    """
 
     def __init__(self, requested_port: int | None = None) -> None:
         """Create the subscription registry object."""
         self.devices: dict[str, Device] = {}
         self._callbacks: dict[
-            Device, list[tuple[str, SubscriberCallback]]
+            Device, list[tuple[str | None, SubscriberCallback]]
         ] = collections.defaultdict(list)
         self._exiting = False
 
         self._event_thread: threading.Thread | None = None
         self._event_thread_cond = threading.Condition()
         self._subscriptions: dict[Device, list[Subscription]] = {}
 
@@ -543,38 +632,41 @@
 
     def event(
         self, device: Device, type_: str, value: str, path: str | None = None
     ) -> None:
         """Execute the callback for a received event."""
         LOG.debug(
             "Received %s event from %s(%s) - %s %s",
-            path or 'an',
+            path or "an",
             device,
             device.host,
             type_,
             value,
         )
         if path:
             # Update the event_received property for the subscription.
             for subscription in self._subscriptions.get(device, []):
                 if subscription.path == path:
                     subscription.event_received = True
                     break
             else:
                 LOG.warning(
-                    'Received unexpected subscription path (%s) for device %s',
+                    "Received unexpected subscription path (%s) for device %s",
                     path,
                     device,
                 )
         for type_filter, callback in self._callbacks.get(device, ()):
             if type_filter is None or type_ == type_filter:
                 callback(device, type_, value)
 
-    def on(
-        self, device: Device, type_filter: str, callback: SubscriberCallback
+    def on(  # pylint: disable=invalid-name
+        self,
+        device: Device,
+        type_filter: str | None,
+        callback: SubscriberCallback,
     ) -> None:
         """Add an event callback for a device."""
         self._callbacks[device].append((type_filter, callback))
 
     def is_subscribed(self, device: Device) -> bool:
         """Return True if all of the device's subscriptions are active."""
         if isinstance(device, Insight) and device.get_state() == 0:
@@ -594,24 +686,24 @@
         )
 
     def start(self) -> None:
         """Start the subscription registry."""
         self._httpd = _start_server(self._requested_port)
         if self._httpd is None:
             raise SubscriptionRegistryFailed(
-                'Unable to bind a port for listening'
+                "Unable to bind a port for listening"
             )
         self._http_thread = threading.Thread(
-            target=self._run_http_server, name='Wemo HTTP Thread'
+            target=self._run_http_server, name="Wemo HTTP Thread"
         )
         self._http_thread.daemon = True
         self._http_thread.start()
 
         self._event_thread = threading.Thread(
-            target=self._run_event_loop, name='Wemo Events Thread'
+            target=self._run_event_loop, name="Wemo Events Thread"
         )
         self._event_thread.daemon = True
         self._event_thread.start()
 
     def stop(self) -> None:
         """Shutdown the HTTP server."""
         assert self._httpd
@@ -638,14 +730,15 @@
     def _run_http_server(self) -> None:
         """Start the HTTP server."""
         assert self._httpd
         self._httpd.allow_reuse_address = True
         self._httpd.outer = self
         LOG.info("Listening on port %d", self.port)
         self._httpd.serve_forever()
+        self._httpd.server_close()
 
     def _run_event_loop(self) -> None:
         """Run the event thread loop."""
         while not self._exiting:
             with self._event_thread_cond:
                 while not self._exiting and self._sched.empty():
                     self._event_thread_cond.wait(10)
```

### Comparing `pywemo-0.9.2/pywemo/util.py` & `pywemo-1.0.0/pywemo/util.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,16 @@
 """Miscellaneous utility functions."""
 from __future__ import annotations
 
 import os
 import socket
-import warnings
-from collections import defaultdict
 from dataclasses import dataclass
 from datetime import datetime, timedelta
-from typing import Any, cast
 
 import ifaddr
-from lxml import etree as et
-
-
-# Taken from http://stackoverflow.com/a/10077069
-def etree_to_dict(tree: et.Element) -> dict[str, Any]:
-    """Split a tree into a dict."""
-    warnings.warn(
-        "pywemo.util.etree_to_dict is unused within pywemo and will be "
-        "removed in a future release.",
-        DeprecationWarning,
-    )
-    # strip namespace
-    tag_name = tree.tag[tree.tag.find("}") + 1 :]
-
-    tree_dict: dict[str, Any] = {tag_name: {} if tree.attrib else None}
-    children = list(tree)
-    if children:
-        default_dict = defaultdict(list)
-        for dict_children in map(etree_to_dict, children):
-            for key, value in dict_children.items():
-                default_dict[key].append(value)
-        tree_dict = {
-            tag_name: {
-                key: value[0] if len(value) == 1 else value
-                for key, value in default_dict.items()
-            }
-        }
-    if tree.attrib:
-        tree_dict[tag_name].update(
-            ('@' + key, value) for key, value in tree.attrib.items()
-        )
-    if tree.text:
-        text = tree.text.strip()
-        if children or tree.attrib:
-            if text:
-                tree_dict[tag_name]['#text'] = text
-        else:
-            tree_dict[tag_name] = text
-    return tree_dict
 
 
 def interface_addresses() -> list[str]:
     """
     Return local address for broadcast/multicast.
 
     Return local address of any network associated with a local interface
@@ -60,32 +18,32 @@
     """
     addresses = []
 
     for iface in ifaddr.get_adapters():
         for addr in iface.ips:
             if not (addr.is_IPv4 and isinstance(addr.ip, str)):
                 continue
-            if addr.ip == '127.0.0.1':
+            if addr.ip == "127.0.0.1":
                 continue
 
             addresses.append(addr.ip)
 
     return addresses
 
 
 def get_callback_address(host: str, port: int) -> str | None:
     """Return IP address & port used by devices to send event notifications."""
-    pywemo_callback_address = os.getenv('PYWEMO_CALLBACK_ADDRESS')
+    pywemo_callback_address = os.getenv("PYWEMO_CALLBACK_ADDRESS")
     if pywemo_callback_address is not None:
         return pywemo_callback_address
 
     sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     try:
         sock.connect((host, 9))
-        return f'{cast(str, sock.getsockname()[0])}:{port}'
+        return f"{sock.getsockname()[0]}:{port}"
     except OSError:
         return None
     finally:
         del sock
 
 
 def signal_strength_to_dbm(value: dict[str, str] | str) -> int:
@@ -129,22 +87,24 @@
     access_point_ssid: str
     model_name: str
 
     @classmethod
     def from_meta_info(cls, value: dict[str, str] | str) -> MetaInfo:
         """Initialize from metainfo.GetMetaInfo() output."""
         info_str = value["MetaInfo"] if isinstance(value, dict) else value
+        if not info_str.isprintable():
+            raise ValueError("Invalid characters found in MetaInfo")
         values = info_str.split("|")
         if len(values) < 6:
             raise ValueError(f"Could not unpack MetaInfo: {info_str}")
         return cls(*values[:6])
 
 
 @dataclass
-class ExtMetaInfo:
+class ExtMetaInfo:  # pylint: disable=too-many-instance-attributes
     """Parsed output of the metainfo.GetExtMetaInfo() Action."""
 
     current_client_state: int
     ice_running: int
     nat_initialized: int
     last_auth_value: int
     uptime: timedelta
@@ -154,14 +114,16 @@
     remote_access_enabled: bool
     model_name: str
 
     @classmethod
     def from_ext_meta_info(cls, value: dict[str, str] | str) -> ExtMetaInfo:
         """Initialize from metainfo.GetExtMetaInfo() output."""
         info_str = value["ExtMetaInfo"] if isinstance(value, dict) else value
+        if not info_str.isprintable():
+            raise ValueError("Invalid characters found in ExtMetaInfo")
         values = info_str.split("|")
         if not len(values) > 9:
             raise ValueError(f"Could not unpack ExtMetaInfo: {info_str}")
 
         hours, minutes, seconds = (int(v) for v in values[4].split(":"))
         return cls(
             current_client_state=int(values[0]),
```

### Comparing `pywemo-0.9.2/PKG-INFO` & `pywemo-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: pywemo
-Version: 0.9.2
+Version: 1.0.0
 Summary: Lightweight Python module to discover and control WeMo devices
 Home-page: https://github.com/pywemo/pywemo
 License: MIT
 Keywords: wemo,api
 Author: Eric Severance
 Author-email: pywemo@esev.com
-Requires-Python: >=3.7.2,<4.0.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ifaddr (>=0.1.0)
 Requires-Dist: lxml (>=4.6,<5.0)
 Requires-Dist: requests (>=2.0)
 Requires-Dist: urllib3 (>=1.26.0)
 Project-URL: Repository, https://github.com/pywemo/pywemo
 Description-Content-Type: text/x-rst
 
-pyWeMo |Build Badge| |PyPI Version Badge| |Coverage| |PyPI Downloads Badge|
-===========================================================================
+pyWeMo |Build Badge| |PyPI Version Badge| |Coverage| |PyPI Downloads Badge| |Docs Badge|
+========================================================================================
 Python 3 module to setup, discover and control WeMo devices.
 
 Dependencies
 ------------
 pyWeMo depends on Python packages: requests, ifaddr, lxml, urllib3
 
 How to use
@@ -173,8 +172,11 @@
     :alt: Latest PyPI version
 .. |Coverage| image:: https://coveralls.io/repos/github/pywemo/pywemo/badge.svg?branch=main
     :target: https://coveralls.io/github/pywemo/pywemo?branch=main
     :alt: Coveralls coverage
 .. |PyPI Downloads Badge| image:: https://img.shields.io/pypi/dm/pywemo
     :target: https://pypi.org/project/pywemo/
     :alt: Number of PyPI downloads
+.. |Docs Badge| image:: https://github.com/pywemo/pywemo/actions/workflows/docs.yml/badge.svg
+    :target: https://pywemo.github.io/pywemo/
+    :alt: API Documentation
```

