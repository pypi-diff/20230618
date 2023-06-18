# Comparing `tmp/ovos-PHAL-plugin-pulseaudio-0.0.2a1.tar.gz` & `tmp/ovos-PHAL-plugin-pulseaudio-0.0.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-pulseaudio-0.0.2a1.tar", last modified: Fri Feb 24 20:15:49 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-pulseaudio-0.0.3a1.tar", last modified: Sun Jun 18 20:06:40 2023, max compression
```

## Comparing `ovos-PHAL-plugin-pulseaudio-0.0.2a1.tar` & `ovos-PHAL-plugin-pulseaudio-0.0.3a1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 20:15:48.999286 ovos-PHAL-plugin-pulseaudio-0.0.2a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-02-24 20:15:41.000000 ovos-PHAL-plugin-pulseaudio-0.0.2a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-24 20:15:41.000000 ovos-PHAL-plugin-pulseaudio-0.0.2a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-24 20:15:48.999286 ovos-PHAL-plugin-pulseaudio-0.0.2a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-02-24 20:15:41.000000 ovos-PHAL-plugin-pulseaudio-0.0.2a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 20:15:48.999286 ovos-PHAL-plugin-pulseaudio-0.0.2a1/ovos_PHAL_plugin_pulseaudio/
--rw-r--r--   0 runner    (1001) docker     (123)    10456 2023-02-24 20:15:41.000000 ovos-PHAL-plugin-pulseaudio-0.0.2a1/ovos_PHAL_plugin_pulseaudio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-02-24 20:15:43.000000 ovos-PHAL-plugin-pulseaudio-0.0.2a1/ovos_PHAL_plugin_pulseaudio/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 20:15:48.999286 ovos-PHAL-plugin-pulseaudio-0.0.2a1/ovos_PHAL_plugin_pulseaudio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-24 20:15:48.000000 ovos-PHAL-plugin-pulseaudio-0.0.2a1/ovos_PHAL_plugin_pulseaudio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-02-24 20:15:48.000000 ovos-PHAL-plugin-pulseaudio-0.0.2a1/ovos_PHAL_plugin_pulseaudio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 20:15:48.000000 ovos-PHAL-plugin-pulseaudio-0.0.2a1/ovos_PHAL_plugin_pulseaudio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-24 20:15:48.000000 ovos-PHAL-plugin-pulseaudio-0.0.2a1/ovos_PHAL_plugin_pulseaudio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-24 20:15:48.000000 ovos-PHAL-plugin-pulseaudio-0.0.2a1/ovos_PHAL_plugin_pulseaudio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-24 20:15:48.000000 ovos-PHAL-plugin-pulseaudio-0.0.2a1/ovos_PHAL_plugin_pulseaudio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 20:15:48.000000 ovos-PHAL-plugin-pulseaudio-0.0.2a1/ovos_PHAL_plugin_pulseaudio.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-24 20:15:41.000000 ovos-PHAL-plugin-pulseaudio-0.0.2a1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 20:15:48.999286 ovos-PHAL-plugin-pulseaudio-0.0.2a1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2796 2023-02-24 20:15:41.000000 ovos-PHAL-plugin-pulseaudio-0.0.2a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:06:40.687288 ovos-PHAL-plugin-pulseaudio-0.0.3a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-18 20:06:33.000000 ovos-PHAL-plugin-pulseaudio-0.0.3a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 20:06:33.000000 ovos-PHAL-plugin-pulseaudio-0.0.3a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-18 20:06:40.687288 ovos-PHAL-plugin-pulseaudio-0.0.3a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-18 20:06:33.000000 ovos-PHAL-plugin-pulseaudio-0.0.3a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:06:40.683288 ovos-PHAL-plugin-pulseaudio-0.0.3a1/ovos_PHAL_plugin_pulseaudio/
+-rw-r--r--   0 runner    (1001) docker     (123)    10453 2023-06-18 20:06:33.000000 ovos-PHAL-plugin-pulseaudio-0.0.3a1/ovos_PHAL_plugin_pulseaudio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-18 20:06:35.000000 ovos-PHAL-plugin-pulseaudio-0.0.3a1/ovos_PHAL_plugin_pulseaudio/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:06:40.687288 ovos-PHAL-plugin-pulseaudio-0.0.3a1/ovos_PHAL_plugin_pulseaudio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-18 20:06:40.000000 ovos-PHAL-plugin-pulseaudio-0.0.3a1/ovos_PHAL_plugin_pulseaudio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-18 20:06:40.000000 ovos-PHAL-plugin-pulseaudio-0.0.3a1/ovos_PHAL_plugin_pulseaudio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 20:06:40.000000 ovos-PHAL-plugin-pulseaudio-0.0.3a1/ovos_PHAL_plugin_pulseaudio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-18 20:06:40.000000 ovos-PHAL-plugin-pulseaudio-0.0.3a1/ovos_PHAL_plugin_pulseaudio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-18 20:06:40.000000 ovos-PHAL-plugin-pulseaudio-0.0.3a1/ovos_PHAL_plugin_pulseaudio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-18 20:06:40.000000 ovos-PHAL-plugin-pulseaudio-0.0.3a1/ovos_PHAL_plugin_pulseaudio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 20:06:40.000000 ovos-PHAL-plugin-pulseaudio-0.0.3a1/ovos_PHAL_plugin_pulseaudio.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-18 20:06:33.000000 ovos-PHAL-plugin-pulseaudio-0.0.3a1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 20:06:40.687288 ovos-PHAL-plugin-pulseaudio-0.0.3a1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2796 2023-06-18 20:06:33.000000 ovos-PHAL-plugin-pulseaudio-0.0.3a1/setup.py
```

### Comparing `ovos-PHAL-plugin-pulseaudio-0.0.2a1/LICENSE` & `ovos-PHAL-plugin-pulseaudio-0.0.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-pulseaudio-0.0.2a1/PKG-INFO` & `ovos-PHAL-plugin-pulseaudio-0.0.3a1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-pulseaudio
-Version: 0.0.2a1
+Version: 0.0.3a1
 Summary: A volume control plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-pulseaudio
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-pulseaudio-0.0.2a1/ovos_PHAL_plugin_pulseaudio/__init__.py` & `ovos-PHAL-plugin-pulseaudio-0.0.3a1/ovos_PHAL_plugin_pulseaudio/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import collections
 import re
 import subprocess
 from os.path import join, dirname
 
 from json_database import JsonConfigXDG
-from mycroft_bus_client import Message
+from ovos_bus_client import Message
 from ovos_plugin_manager.phal import PHALPlugin
 from ovos_utils.sound import play_audio
 from ovos_utils.system import find_executable, is_process_running
 
 
 class PulseAudioValidator:
     @staticmethod
```

### Comparing `ovos-PHAL-plugin-pulseaudio-0.0.2a1/ovos_PHAL_plugin_pulseaudio.egg-info/PKG-INFO` & `ovos-PHAL-plugin-pulseaudio-0.0.3a1/ovos_PHAL_plugin_pulseaudio.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-pulseaudio
-Version: 0.0.2a1
+Version: 0.0.3a1
 Summary: A volume control plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-pulseaudio
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-pulseaudio-0.0.2a1/setup.py` & `ovos-PHAL-plugin-pulseaudio-0.0.3a1/setup.py`

 * *Files identical despite different names*

