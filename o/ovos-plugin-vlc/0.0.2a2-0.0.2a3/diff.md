# Comparing `tmp/ovos_plugin_vlc-0.0.2a2-py3-none-any.whl.zip` & `tmp/ovos_plugin_vlc-0.0.2a3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 8313 bytes, number of entries: 8
--rw-r--r--  2.0 unx     8437 b- defN 22-Aug-05 12:07 ovos_plugin_vlc/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 22-Aug-05 12:07 ovos_plugin_vlc/version.py
--rw-r--r--  2.0 unx    11349 b- defN 22-Aug-05 12:07 ovos_plugin_vlc-0.0.2a2.dist-info/LICENSE
--rw-r--r--  2.0 unx      350 b- defN 22-Aug-05 12:07 ovos_plugin_vlc-0.0.2a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Aug-05 12:07 ovos_plugin_vlc-0.0.2a2.dist-info/WHEEL
--rw-r--r--  2.0 unx      147 b- defN 22-Aug-05 12:07 ovos_plugin_vlc-0.0.2a2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       16 b- defN 22-Aug-05 12:07 ovos_plugin_vlc-0.0.2a2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      708 b- defN 22-Aug-05 12:07 ovos_plugin_vlc-0.0.2a2.dist-info/RECORD
-8 files, 21276 bytes uncompressed, 7059 bytes compressed:  66.8%
+Zip file size: 8308 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     8434 b- defN 23-Jun-18 20:05 ovos_plugin_vlc/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Jun-18 20:05 ovos_plugin_vlc/version.py
+-rw-r--r--  2.0 unx    11349 b- defN 23-Jun-18 20:05 ovos_plugin_vlc-0.0.2a3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      350 b- defN 23-Jun-18 20:05 ovos_plugin_vlc-0.0.2a3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-18 20:05 ovos_plugin_vlc-0.0.2a3.dist-info/WHEEL
+-rw-r--r--  2.0 unx      147 b- defN 23-Jun-18 20:05 ovos_plugin_vlc-0.0.2a3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-18 20:05 ovos_plugin_vlc-0.0.2a3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      708 b- defN 23-Jun-18 20:05 ovos_plugin_vlc-0.0.2a3.dist-info/RECORD
+8 files, 21273 bytes uncompressed, 7054 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: ovos_plugin_vlc/__init__.py
 Comment: 
 
 Filename: ovos_plugin_vlc/version.py
 Comment: 
 
-Filename: ovos_plugin_vlc-0.0.2a2.dist-info/LICENSE
+Filename: ovos_plugin_vlc-0.0.2a3.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_plugin_vlc-0.0.2a2.dist-info/METADATA
+Filename: ovos_plugin_vlc-0.0.2a3.dist-info/METADATA
 Comment: 
 
-Filename: ovos_plugin_vlc-0.0.2a2.dist-info/WHEEL
+Filename: ovos_plugin_vlc-0.0.2a3.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_plugin_vlc-0.0.2a2.dist-info/entry_points.txt
+Filename: ovos_plugin_vlc-0.0.2a3.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_plugin_vlc-0.0.2a2.dist-info/top_level.txt
+Filename: ovos_plugin_vlc-0.0.2a3.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_plugin_vlc-0.0.2a2.dist-info/RECORD
+Filename: ovos_plugin_vlc-0.0.2a3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_plugin_vlc/__init__.py

```diff
@@ -1,10 +1,10 @@
 from ovos_plugin_manager.templates.audio import AudioBackend
 from ovos_utils.log import LOG
-from mycroft_bus_client.message import Message
+from ovos_bus_client.message import Message
 from ovos_plugin_common_play.ocp.status import TrackState, \
     MediaState, PlayerState
 import vlc
 import time
 
 
 VLCAudioPluginConfig = {
```

## ovos_plugin_vlc/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 2
-VERSION_ALPHA = 2
+VERSION_ALPHA = 3
 # END_VERSION_BLOCK
```

## Comparing `ovos_plugin_vlc-0.0.2a2.dist-info/LICENSE` & `ovos_plugin_vlc-0.0.2a3.dist-info/LICENSE`

 * *Files identical despite different names*

