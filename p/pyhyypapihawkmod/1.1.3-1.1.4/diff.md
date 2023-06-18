# Comparing `tmp/pyhyypapihawkmod-1.1.3.tar.gz` & `tmp/pyhyypapihawkmod-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-1.1.3.tar", last modified: Wed Jun 14 05:46:18 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-1.1.4.tar", last modified: Sun Jun 18 10:38:22 2023, max compression
```

## Comparing `pyhyypapihawkmod-1.1.3.tar` & `pyhyypapihawkmod-1.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 05:46:18.589983 pyhyypapihawkmod-1.1.3/
--rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.3/LICENSE.md
--rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      517 2023-06-14 05:46:18.588956 pyhyypapihawkmod-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1917 2023-06-14 05:43:17.000000 pyhyypapihawkmod-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 05:46:18.572353 pyhyypapihawkmod-1.1.3/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      429 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.3/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.3/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0     7652 2023-06-14 05:42:00.000000 pyhyypapihawkmod-1.1.3/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.3/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.3/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    27687 2023-06-08 12:19:08.000000 pyhyypapihawkmod-1.1.3/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     4005 2023-05-28 09:35:32.000000 pyhyypapihawkmod-1.1.3/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.3/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.3/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.3/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-06-14 05:46:18.586900 pyhyypapihawkmod-1.1.3/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      517 2023-06-14 05:46:18.000000 pyhyypapihawkmod-1.1.3/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-06-14 05:46:18.000000 pyhyypapihawkmod-1.1.3/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 05:46:18.000000 pyhyypapihawkmod-1.1.3/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-14 05:46:18.000000 pyhyypapihawkmod-1.1.3/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-14 05:46:18.000000 pyhyypapihawkmod-1.1.3/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 05:46:18.589983 pyhyypapihawkmod-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      921 2023-06-14 05:42:31.000000 pyhyypapihawkmod-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 10:38:22.068194 pyhyypapihawkmod-1.1.4/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.4/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      517 2023-06-18 10:38:22.066683 pyhyypapihawkmod-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2060 2023-06-18 10:36:49.000000 pyhyypapihawkmod-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 10:38:22.045209 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      429 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0     7697 2023-06-18 10:36:49.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    27687 2023-06-08 12:19:08.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4005 2023-05-28 09:35:32.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-06-18 10:38:22.063686 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      517 2023-06-18 10:38:21.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-06-18 10:38:21.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 10:38:21.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-18 10:38:21.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-18 10:38:21.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 10:38:22.068194 pyhyypapihawkmod-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      921 2023-06-18 10:36:49.000000 pyhyypapihawkmod-1.1.4/setup.py
```

### Comparing `pyhyypapihawkmod-1.1.3/LICENSE.md` & `pyhyypapihawkmod-1.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.3/PKG-INFO` & `pyhyypapihawkmod-1.1.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.3
+Version: 1.1.4
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.3/README.md` & `pyhyypapihawkmod-1.1.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -45,16 +45,19 @@
 - CLI usage. (GCF client is there, just needs some more automation.)
 - Capture panic api...for obvious reasons.
 - What zone caused arm/arm stay not to work. - Looks like GCM/Firebase push messages. Added GCM client...just run main program and register GCF code in function called register gcf. It works.
 
 
 Changelog 
 
+1.1.4
+- Bugfix: When no "triggers" exist a blank key is now returned instead of nothing. This caused a KeyError in home assistant.
+
 1.1.3
-- Fixes a bug when calling notifications
+- Bugfix: Fixes a bug when calling notifications
 
 1.1.2
 - Changed the way notifications are cached
 - Changed the last notification timestamp from a global variable to a class variable
 
 1.1.1
 - Bugfix: Missing variable to timeout
```

### Comparing `pyhyypapihawkmod-1.1.3/pyhyypapihawkmod/alarm_info.py` & `pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/alarm_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,14 +119,15 @@
 
             # Add last site notification.
             _last_notice = self._last_notice()
             site_ids[site]["lastNoticeTime"] = _last_notice["lastNoticeTime"]
             site_ids[site]["lastNoticeName"] = _last_notice["lastNoticeName"]
 
             # Add triggers (PGM / Automations in APP)
+            site_ids[site]["triggers"] = {}
             for trigger_id in trigger_ids:
                 if trigger_id not in site_ids[site]["triggerIds"]:
                     continue
                 else:
                     site_ids[site]["triggers"] = {
                         key: value
                         for (key, value) in trigger_ids.items()
```

### Comparing `pyhyypapihawkmod-1.1.3/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.3/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.3/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/client.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.3/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/constants.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.3/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.3/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/push_receiver.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.3/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-1.1.4/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.3
+Version: 1.1.4
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.3/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-1.1.4/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.3/setup.py` & `pyhyypapihawkmod-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="1.1.3",
+    version="1.1.4",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
```

