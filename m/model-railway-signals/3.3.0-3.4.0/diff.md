# Comparing `tmp/model-railway-signals-3.3.0.tar.gz` & `tmp/model-railway-signals-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/model-railway-signals-3.3.0.tar", last modified: Sat Apr 22 16:49:21 2023, max compression
+gzip compressed data, was "dist/model-railway-signals-3.4.0.tar", last modified: Sun Jun 18 15:02:23 2023, max compression
```

## Comparing `model-railway-signals-3.3.0.tar` & `model-railway-signals-3.4.0.tar`

### file list

```diff
@@ -1,74 +1,80 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-22 16:49:21.000000 model-railway-signals-3.3.0/
--rw-r--r--   0 pi        (1000) pi        (1000)      127 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/MANIFEST.in
--rw-r--r--   0 pi        (1000) pi        (1000)     5715 2023-04-22 16:49:21.000000 model-railway-signals-3.3.0/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     4435 2023-04-22 16:44:27.000000 model-railway-signals-3.3.0/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-22 16:49:21.000000 model-railway-signals-3.3.0/model_railway_signals/
--rw-r--r--   0 pi        (1000) pi        (1000)     6599 2023-04-06 13:44:14.000000 model-railway-signals-3.3.0/model_railway_signals/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)      325 2023-03-25 09:50:18.000000 model-railway-signals-3.3.0/model_railway_signals/__main__.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-22 16:49:21.000000 model-railway-signals-3.3.0/model_railway_signals/editor/
--rw-r--r--   0 pi        (1000) pi        (1000)        0 2023-03-25 09:50:18.000000 model-railway-signals-3.3.0/model_railway_signals/editor/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)    42645 2023-04-21 13:57:37.000000 model-railway-signals-3.3.0/model_railway_signals/editor/common.py
--rw-r--r--   0 pi        (1000) pi        (1000)    17653 2023-04-22 13:10:39.000000 model-railway-signals-3.3.0/model_railway_signals/editor/configure_instrument.py
--rw-r--r--   0 pi        (1000) pi        (1000)    20790 2023-04-21 14:01:49.000000 model-railway-signals-3.3.0/model_railway_signals/editor/configure_point.py
--rw-r--r--   0 pi        (1000) pi        (1000)    21713 2023-04-06 17:26:45.000000 model-railway-signals-3.3.0/model_railway_signals/editor/configure_section.py
--rw-r--r--   0 pi        (1000) pi        (1000)    58487 2023-04-06 17:00:22.000000 model-railway-signals-3.3.0/model_railway_signals/editor/configure_signal.py
--rw-r--r--   0 pi        (1000) pi        (1000)    53376 2023-04-09 07:33:17.000000 model-railway-signals-3.3.0/model_railway_signals/editor/configure_signal_tab1.py
--rw-r--r--   0 pi        (1000) pi        (1000)    21575 2023-04-06 17:18:07.000000 model-railway-signals-3.3.0/model_railway_signals/editor/configure_signal_tab2.py
--rw-r--r--   0 pi        (1000) pi        (1000)    34207 2023-04-06 17:10:41.000000 model-railway-signals-3.3.0/model_railway_signals/editor/configure_signal_tab3.py
--rw-r--r--   0 pi        (1000) pi        (1000)    19118 2023-04-22 16:13:13.000000 model-railway-signals-3.3.0/model_railway_signals/editor/editor.py
--rw-r--r--   0 pi        (1000) pi        (1000)    18788 2023-04-10 08:10:14.000000 model-railway-signals-3.3.0/model_railway_signals/editor/menubar_windows.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-22 16:49:21.000000 model-railway-signals-3.3.0/model_railway_signals/editor/objects/
--rw-r--r--   0 pi        (1000) pi        (1000)     5501 2023-04-06 13:44:14.000000 model-railway-signals-3.3.0/model_railway_signals/editor/objects/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)    32108 2023-04-10 08:57:59.000000 model-railway-signals-3.3.0/model_railway_signals/editor/objects/objects.py
--rw-r--r--   0 pi        (1000) pi        (1000)     9563 2023-04-06 13:44:14.000000 model-railway-signals-3.3.0/model_railway_signals/editor/objects/objects_common.py
--rw-r--r--   0 pi        (1000) pi        (1000)    13272 2023-04-22 11:59:29.000000 model-railway-signals-3.3.0/model_railway_signals/editor/objects/objects_instruments.py
--rw-r--r--   0 pi        (1000) pi        (1000)     7428 2023-04-06 13:44:14.000000 model-railway-signals-3.3.0/model_railway_signals/editor/objects/objects_lines.py
--rw-r--r--   0 pi        (1000) pi        (1000)    20303 2023-04-06 13:44:14.000000 model-railway-signals-3.3.0/model_railway_signals/editor/objects/objects_points.py
--rw-r--r--   0 pi        (1000) pi        (1000)    19032 2023-04-06 13:44:14.000000 model-railway-signals-3.3.0/model_railway_signals/editor/objects/objects_sections.py
--rw-r--r--   0 pi        (1000) pi        (1000)    50499 2023-04-06 16:20:27.000000 model-railway-signals-3.3.0/model_railway_signals/editor/objects/objects_signals.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-22 16:49:21.000000 model-railway-signals-3.3.0/model_railway_signals/editor/resources/
--rw-r--r--   0 pi        (1000) pi        (1000)        0 2023-03-25 09:50:18.000000 model-railway-signals-3.3.0/model_railway_signals/editor/resources/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)      644 2023-03-25 09:50:18.000000 model-railway-signals-3.3.0/model_railway_signals/editor/resources/block_instrument.png
--rw-r--r--   0 pi        (1000) pi        (1000)      284 2023-03-25 09:50:18.000000 model-railway-signals-3.3.0/model_railway_signals/editor/resources/colour_light.png
--rw-r--r--   0 pi        (1000) pi        (1000)      295 2023-03-25 09:50:18.000000 model-railway-signals-3.3.0/model_railway_signals/editor/resources/ground_disc.png
--rw-r--r--   0 pi        (1000) pi        (1000)      277 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/editor/resources/ground_position.png
--rw-r--r--   0 pi        (1000) pi        (1000)      247 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/editor/resources/left_hand_point.png
--rw-r--r--   0 pi        (1000) pi        (1000)      170 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/editor/resources/line.png
--rw-r--r--   0 pi        (1000) pi        (1000)      246 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/editor/resources/right_hand_point.png
--rw-r--r--   0 pi        (1000) pi        (1000)      208 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/editor/resources/semaphore.png
--rw-r--r--   0 pi        (1000) pi        (1000)      670 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/editor/resources/track_section.png
--rw-r--r--   0 pi        (1000) pi        (1000)    53684 2023-04-22 14:12:59.000000 model-railway-signals-3.3.0/model_railway_signals/editor/run_layout.py
--rw-r--r--   0 pi        (1000) pi        (1000)    40127 2023-04-22 16:11:15.000000 model-railway-signals-3.3.0/model_railway_signals/editor/schematic.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6955 2023-04-22 16:45:15.000000 model-railway-signals-3.3.0/model_railway_signals/editor/settings.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-22 16:49:21.000000 model-railway-signals-3.3.0/model_railway_signals/library/
--rw-r--r--   0 pi        (1000) pi        (1000)        0 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/library/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)    49745 2023-04-21 15:00:53.000000 model-railway-signals-3.3.0/model_railway_signals/library/block_instruments.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6542 2023-04-06 13:44:14.000000 model-railway-signals-3.3.0/model_railway_signals/library/common.py
--rw-r--r--   0 pi        (1000) pi        (1000)    43683 2023-04-06 13:44:14.000000 model-railway-signals-3.3.0/model_railway_signals/library/dcc_control.py
--rw-r--r--   0 pi        (1000) pi        (1000)    23375 2023-04-21 13:14:12.000000 model-railway-signals-3.3.0/model_railway_signals/library/file_interface.py
--rw-r--r--   0 pi        (1000) pi        (1000)    18681 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/library/mqtt_interface.py
--rw-r--r--   0 pi        (1000) pi        (1000)    31806 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/library/pi_sprog_interface.py
--rw-r--r--   0 pi        (1000) pi        (1000)    26355 2023-04-06 17:38:56.000000 model-railway-signals-3.3.0/model_railway_signals/library/points.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-22 16:49:21.000000 model-railway-signals-3.3.0/model_railway_signals/library/resources/
--rw-r--r--   0 pi        (1000) pi        (1000)        0 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/library/resources/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)    80808 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/library/resources/bell-ring-01.wav
--rw-r--r--   0 pi        (1000) pi        (1000)    80808 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/library/resources/bell-ring-02.wav
--rw-r--r--   0 pi        (1000) pi        (1000)    80808 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/library/resources/bell-ring-03.wav
--rw-r--r--   0 pi        (1000) pi        (1000)    80808 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/library/resources/bell-ring-04.wav
--rw-r--r--   0 pi        (1000) pi        (1000)    30722 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/library/resources/telegraph-key-01.wav
--rw-r--r--   0 pi        (1000) pi        (1000)    52852 2023-04-06 15:39:47.000000 model-railway-signals-3.3.0/model_railway_signals/library/signals.py
--rw-r--r--   0 pi        (1000) pi        (1000)    46658 2023-04-06 15:40:23.000000 model-railway-signals-3.3.0/model_railway_signals/library/signals_colour_lights.py
--rw-r--r--   0 pi        (1000) pi        (1000)    37138 2023-04-06 15:56:51.000000 model-railway-signals-3.3.0/model_railway_signals/library/signals_common.py
--rw-r--r--   0 pi        (1000) pi        (1000)     7412 2023-04-06 16:06:14.000000 model-railway-signals-3.3.0/model_railway_signals/library/signals_ground_disc.py
--rw-r--r--   0 pi        (1000) pi        (1000)     9805 2023-04-06 16:04:36.000000 model-railway-signals-3.3.0/model_railway_signals/library/signals_ground_position.py
--rw-r--r--   0 pi        (1000) pi        (1000)    55615 2023-04-06 16:07:03.000000 model-railway-signals-3.3.0/model_railway_signals/library/signals_semaphores.py
--rw-r--r--   0 pi        (1000) pi        (1000)    25918 2023-04-06 15:44:18.000000 model-railway-signals-3.3.0/model_railway_signals/library/track_sections.py
--rw-r--r--   0 pi        (1000) pi        (1000)    13806 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/library/track_sensors.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-22 16:49:21.000000 model-railway-signals-3.3.0/model_railway_signals.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     5715 2023-04-22 16:49:18.000000 model-railway-signals-3.3.0/model_railway_signals.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     3077 2023-04-22 16:49:18.000000 model-railway-signals-3.3.0/model_railway_signals.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-04-22 16:49:18.000000 model-railway-signals-3.3.0/model_railway_signals.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       19 2023-04-22 16:49:18.000000 model-railway-signals-3.3.0/model_railway_signals.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       22 2023-04-22 16:49:18.000000 model-railway-signals-3.3.0/model_railway_signals.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-04-22 16:49:21.000000 model-railway-signals-3.3.0/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      979 2023-04-22 16:44:43.000000 model-railway-signals-3.3.0/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-18 15:02:23.000000 model-railway-signals-3.4.0/
+-rw-r--r--   0 pi        (1000) pi        (1000)      127 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/MANIFEST.in
+-rw-r--r--   0 pi        (1000) pi        (1000)     6386 2023-06-18 15:02:23.000000 model-railway-signals-3.4.0/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)     5042 2023-06-18 14:44:25.000000 model-railway-signals-3.4.0/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-18 15:02:23.000000 model-railway-signals-3.4.0/model_railway_signals/
+-rw-r--r--   0 pi        (1000) pi        (1000)     6829 2023-06-13 19:27:26.000000 model-railway-signals-3.4.0/model_railway_signals/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      325 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/__main__.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-18 15:02:23.000000 model-railway-signals-3.4.0/model_railway_signals/editor/
+-rw-r--r--   0 pi        (1000) pi        (1000)        0 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/editor/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    49919 2023-05-17 19:17:06.000000 model-railway-signals-3.4.0/model_railway_signals/editor/common.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    17917 2023-06-12 20:31:04.000000 model-railway-signals-3.4.0/model_railway_signals/editor/configure_instrument.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    10609 2023-06-18 14:35:52.000000 model-railway-signals-3.4.0/model_railway_signals/editor/configure_line.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    21296 2023-05-17 19:02:06.000000 model-railway-signals-3.4.0/model_railway_signals/editor/configure_point.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    22142 2023-06-04 18:46:34.000000 model-railway-signals-3.4.0/model_railway_signals/editor/configure_section.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    58536 2023-05-17 19:02:52.000000 model-railway-signals-3.4.0/model_railway_signals/editor/configure_signal.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    53376 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/editor/configure_signal_tab1.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    21732 2023-05-17 18:48:48.000000 model-railway-signals-3.4.0/model_railway_signals/editor/configure_signal_tab2.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    34207 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/editor/configure_signal_tab3.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    21192 2023-06-18 13:48:39.000000 model-railway-signals-3.4.0/model_railway_signals/editor/editor.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    22191 2023-06-18 14:03:21.000000 model-railway-signals-3.4.0/model_railway_signals/editor/menubar_windows.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-18 15:02:23.000000 model-railway-signals-3.4.0/model_railway_signals/editor/objects/
+-rw-r--r--   0 pi        (1000) pi        (1000)     6067 2023-04-30 08:41:38.000000 model-railway-signals-3.4.0/model_railway_signals/editor/objects/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    32300 2023-06-17 07:57:59.000000 model-railway-signals-3.4.0/model_railway_signals/editor/objects/objects.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     9959 2023-05-03 18:46:06.000000 model-railway-signals-3.4.0/model_railway_signals/editor/objects/objects_common.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    13178 2023-05-17 19:28:08.000000 model-railway-signals-3.4.0/model_railway_signals/editor/objects/objects_instruments.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    13260 2023-05-17 19:28:02.000000 model-railway-signals-3.4.0/model_railway_signals/editor/objects/objects_lines.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    20191 2023-05-03 18:38:12.000000 model-railway-signals-3.4.0/model_railway_signals/editor/objects/objects_points.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    18889 2023-04-30 05:47:14.000000 model-railway-signals-3.4.0/model_railway_signals/editor/objects/objects_sections.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    50424 2023-06-13 19:24:44.000000 model-railway-signals-3.4.0/model_railway_signals/editor/objects/objects_signals.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-18 15:02:23.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/
+-rw-r--r--   0 pi        (1000) pi        (1000)        0 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2900 2023-05-03 17:52:46.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/arrow1.png
+-rw-r--r--   0 pi        (1000) pi        (1000)     2914 2023-05-03 17:54:08.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/arrow2.png
+-rw-r--r--   0 pi        (1000) pi        (1000)     2927 2023-05-03 17:55:10.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/arrow3.png
+-rw-r--r--   0 pi        (1000) pi        (1000)     2933 2023-05-03 17:55:54.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/arrow4.png
+-rw-r--r--   0 pi        (1000) pi        (1000)      284 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/colourlight.png
+-rw-r--r--   0 pi        (1000) pi        (1000)     2858 2023-04-30 16:09:28.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/endstop.png
+-rw-r--r--   0 pi        (1000) pi        (1000)      295 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/grounddisc.png
+-rw-r--r--   0 pi        (1000) pi        (1000)      277 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/groundpos.png
+-rw-r--r--   0 pi        (1000) pi        (1000)      644 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/instrument.png
+-rw-r--r--   0 pi        (1000) pi        (1000)      247 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/lhpoint.png
+-rw-r--r--   0 pi        (1000) pi        (1000)      170 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/line.png
+-rw-r--r--   0 pi        (1000) pi        (1000)      246 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/rhpoint.png
+-rw-r--r--   0 pi        (1000) pi        (1000)      670 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/section.png
+-rw-r--r--   0 pi        (1000) pi        (1000)      208 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/semaphore.png
+-rw-r--r--   0 pi        (1000) pi        (1000)    55559 2023-05-23 20:06:32.000000 model-railway-signals-3.4.0/model_railway_signals/editor/run_layout.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    42689 2023-06-17 07:57:38.000000 model-railway-signals-3.4.0/model_railway_signals/editor/schematic.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     9149 2023-06-18 14:04:31.000000 model-railway-signals-3.4.0/model_railway_signals/editor/settings.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-18 15:02:23.000000 model-railway-signals-3.4.0/model_railway_signals/library/
+-rw-r--r--   0 pi        (1000) pi        (1000)        0 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/library/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    56398 2023-06-04 19:20:01.000000 model-railway-signals-3.4.0/model_railway_signals/library/block_instruments.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     6481 2023-05-17 20:19:26.000000 model-railway-signals-3.4.0/model_railway_signals/library/common.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    43946 2023-06-04 19:34:10.000000 model-railway-signals-3.4.0/model_railway_signals/library/dcc_control.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    23696 2023-05-17 20:22:42.000000 model-railway-signals-3.4.0/model_railway_signals/library/file_interface.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    20005 2023-06-14 19:04:40.000000 model-railway-signals-3.4.0/model_railway_signals/library/mqtt_interface.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    31597 2023-05-17 20:24:20.000000 model-railway-signals-3.4.0/model_railway_signals/library/pi_sprog_interface.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    26152 2023-05-17 20:25:20.000000 model-railway-signals-3.4.0/model_railway_signals/library/points.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-18 15:02:23.000000 model-railway-signals-3.4.0/model_railway_signals/library/resources/
+-rw-r--r--   0 pi        (1000) pi        (1000)        0 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/library/resources/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    80808 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/library/resources/bell-ring-01.wav
+-rw-r--r--   0 pi        (1000) pi        (1000)    80808 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/library/resources/bell-ring-02.wav
+-rw-r--r--   0 pi        (1000) pi        (1000)    80808 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/library/resources/bell-ring-03.wav
+-rw-r--r--   0 pi        (1000) pi        (1000)    80808 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/library/resources/bell-ring-04.wav
+-rw-r--r--   0 pi        (1000) pi        (1000)    30722 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/library/resources/telegraph-key-01.wav
+-rw-r--r--   0 pi        (1000) pi        (1000)    50923 2023-06-04 19:13:19.000000 model-railway-signals-3.4.0/model_railway_signals/library/signals.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    46806 2023-06-14 19:51:48.000000 model-railway-signals-3.4.0/model_railway_signals/library/signals_colour_lights.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    39299 2023-06-14 20:26:52.000000 model-railway-signals-3.4.0/model_railway_signals/library/signals_common.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     7712 2023-06-14 19:16:38.000000 model-railway-signals-3.4.0/model_railway_signals/library/signals_ground_disc.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    10104 2023-06-14 19:16:30.000000 model-railway-signals-3.4.0/model_railway_signals/library/signals_ground_position.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    55797 2023-06-14 19:51:58.000000 model-railway-signals-3.4.0/model_railway_signals/library/signals_semaphores.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    27709 2023-06-04 19:12:12.000000 model-railway-signals-3.4.0/model_railway_signals/library/track_sections.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    13717 2023-05-17 20:33:06.000000 model-railway-signals-3.4.0/model_railway_signals/library/track_sensors.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-18 15:02:23.000000 model-railway-signals-3.4.0/model_railway_signals.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     6386 2023-06-18 15:02:20.000000 model-railway-signals-3.4.0/model_railway_signals.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)     3338 2023-06-18 15:02:20.000000 model-railway-signals-3.4.0/model_railway_signals.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-06-18 15:02:20.000000 model-railway-signals-3.4.0/model_railway_signals.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       19 2023-06-18 15:02:20.000000 model-railway-signals-3.4.0/model_railway_signals.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       22 2023-06-18 15:02:20.000000 model-railway-signals-3.4.0/model_railway_signals.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-06-18 15:02:23.000000 model-railway-signals-3.4.0/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      979 2023-06-18 14:04:57.000000 model-railway-signals-3.4.0/setup.py
```

### Comparing `model-railway-signals-3.3.0/PKG-INFO` & `model-railway-signals-3.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,50 @@
 Metadata-Version: 2.1
 Name: model-railway-signals
-Version: 3.3.0
+Version: 3.4.0
 Summary: Create your own DCC model railway signalling scheme
 Home-page: https://github.com/johnrm174/model-railway-signalling
 Author: johnrm174
 Author-email: johnrm17418@gmail.com
 License: GNU GENERAL PUBLIC LICENSE Version 2, June 1991
 Description: # model-railway-signalling
         
         A DCC model railway signalling system written in Python. Primarily intended for the Raspberry Pi, but 
         will also run on other platforms (albeit without some of the Raspberry-Pi specific interfacing functions). 
-        Most types of colour light signals, semaphore signals, and ground signals are supported.
+        * Enables schematics to be created with signals, points, track occupancy sections and block instruments
+        * Most types of colour light signals, semaphore signals, and ground signals are supported.
         * Interfaces with the Pi-SPROG DCC command station to drive the signals and points out on the layout
         * Uses the Raspberry Pi GPIO inputs to provide train detection in support of signalling automation
+        * Incorporates MQTT networking to allow multiple signalling applications to be linked for larger layouts
         
         ## Layout editor
         
-        From Release 3.0.0, the schematic editor application enables automated and interlocked layout signalling 
-        schemes to be designed and configured without the need to write any code. Note that the editor is in
+        The schematic editor application enables automated and interlocked layout signalling schemes to be
+        designed and configured via the UI without the need to write any code. Note that the editor is in
         active development so any comments and suggestions for future features are welcome.
         
-        What's supported in Release 3.3.0:
-        * Draw your layout schematic with lines, points, signals and track occupancy sections
-        * Define the DCC command sequences to drive the signals and points out on the layout
-        * Configure the signals and points to implement protototypical interlocking schemes
+        What's currently supported by the Editor:
+        * Draw your schematic with lines, points, signals, track occupancy sections and block instruments
+        * Define the DCC command sequences needed to drive the signals and points out on the layout
+        * Configure the signals, points and block instruments for protototypical interlocking
         * Configure GPIO sensors and track sections to provide a 'mimic' display of the layout
-        * Automation of signals as trains traverse the routes that have been configured
-        * Save and load your layout schematic and state between running sessions
-        * Block instruments - with interlocking of starting signals
-        * Popup error messages when things go wrong (reduced reliance on logs)
+        * Configure a level of automation for the signals as trains traverse the layout
+        
+        What's New in Release 3.4.0:
+        * Point and line colour selections - to enable colour coding of routes
+        * Line end-style selections - end-stops and arrow styles can now be specified
+        * Enhanced error/warning reporting via popups - reduced reliance on logs
+        * Layout 'info' function (under Help) allows you to add notes for your layout
+        * Fixed issue when selecting objects if Canvas is scrolled within the main window
+        * Various window geometry improvements to keep key UI elements visible on resizing
+        * Track section occupancy logic corrected for passing shunt-ahead ground signals
         
         What's coming soon:
         * MQTT networking (for linking layouts)
-        * Application documentation
+        * Better pplication documentation
         
         Any bug reports and feedback you may have would be gratefully appreciated - specifically:
         * What aspects are intuitive? What aspects aren't?
         * What aspects do you particularly like?
         * What aspects particularly irritate you?
         
         There are some example layout files in the 'configuration_examples' folder.
```

### Comparing `model-railway-signals-3.3.0/README.md` & `model-railway-signals-3.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 # model-railway-signalling
 
 A DCC model railway signalling system written in Python. Primarily intended for the Raspberry Pi, but 
 will also run on other platforms (albeit without some of the Raspberry-Pi specific interfacing functions). 
-Most types of colour light signals, semaphore signals, and ground signals are supported.
+* Enables schematics to be created with signals, points, track occupancy sections and block instruments
+* Most types of colour light signals, semaphore signals, and ground signals are supported.
 * Interfaces with the Pi-SPROG DCC command station to drive the signals and points out on the layout
 * Uses the Raspberry Pi GPIO inputs to provide train detection in support of signalling automation
+* Incorporates MQTT networking to allow multiple signalling applications to be linked for larger layouts
 
 ## Layout editor
 
-From Release 3.0.0, the schematic editor application enables automated and interlocked layout signalling 
-schemes to be designed and configured without the need to write any code. Note that the editor is in
+The schematic editor application enables automated and interlocked layout signalling schemes to be
+designed and configured via the UI without the need to write any code. Note that the editor is in
 active development so any comments and suggestions for future features are welcome.
 
-What's supported in Release 3.3.0:
-* Draw your layout schematic with lines, points, signals and track occupancy sections
-* Define the DCC command sequences to drive the signals and points out on the layout
-* Configure the signals and points to implement protototypical interlocking schemes
+What's currently supported by the Editor:
+* Draw your schematic with lines, points, signals, track occupancy sections and block instruments
+* Define the DCC command sequences needed to drive the signals and points out on the layout
+* Configure the signals, points and block instruments for protototypical interlocking
 * Configure GPIO sensors and track sections to provide a 'mimic' display of the layout
-* Automation of signals as trains traverse the routes that have been configured
-* Save and load your layout schematic and state between running sessions
-* Block instruments - with interlocking of starting signals
-* Popup error messages when things go wrong (reduced reliance on logs)
+* Configure a level of automation for the signals as trains traverse the layout
+
+What's New in Release 3.4.0:
+* Point and line colour selections - to enable colour coding of routes
+* Line end-style selections - end-stops and arrow styles can now be specified
+* Enhanced error/warning reporting via popups - reduced reliance on logs
+* Layout 'info' function (under Help) allows you to add notes for your layout
+* Fixed issue when selecting objects if Canvas is scrolled within the main window
+* Various window geometry improvements to keep key UI elements visible on resizing
+* Track section occupancy logic corrected for passing shunt-ahead ground signals
 
 What's coming soon:
 * MQTT networking (for linking layouts)
-* Application documentation
+* Better pplication documentation
 
 Any bug reports and feedback you may have would be gratefully appreciated - specifically:
 * What aspects are intuitive? What aspects aren't?
 * What aspects do you particularly like?
 * What aspects particularly irritate you?
 
 There are some example layout files in the 'configuration_examples' folder.
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/__init__.py` & `model-railway-signals-3.4.0/model_railway_signals/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,14 +76,16 @@
 from .library.mqtt_interface import configure_networking
 
 from .library.file_interface import load_layout_state
 
 from .library.block_instruments import block_callback_type
 from .library.block_instruments import create_block_instrument
 from .library.block_instruments import block_section_ahead_clear
+from .library.block_instruments import subscribe_to_instrument_updates
+from .library.block_instruments import set_instruments_to_publish_state
 
 from .editor.editor import run_editor
 
 __all__ = [
       # Public point types
         'point_type',
         'point_callback_type',
@@ -161,11 +163,13 @@
       # Public File load/save functions
         'load_layout_state',
       # public block instrument types
         'block_callback_type',
       # Public block instrument functions
         'create_block_instrument',
         'block_section_ahead_clear',
+        'subscribe_to_instrument_updates',
+        'set_instruments_to_publish_state',
       # Public function to run editor
         'run_editor'
            ]
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/editor/common.py` & `model-railway-signals-3.4.0/model_railway_signals/editor/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 #------------------------------------------------------------------------------------
 # These are common classes used across multiple UI Elements
 #
-# Provides the following base classes for use across the editor UI
+# Provides the following 'primitive' classes for use across the editor UI
 #    CreateToolTip(widget,tool_tip)
-#    check_box(entry)
-#    state_box(entry)
-#    entry_box(entry)
+#    check_box(Tk.Checkbutton)
+#    state_box(Tk.Checkbutton)
+#    entry_box(Tk.Entry)
 #    integer_entry_box(entry_box)
 #    dcc_entry_box(integer_entry_box)
 #    int_item_id_entry_box (integer_entry_box)
 #    str_item_id_entry_box(entry_box)
-#    object_id_selection(integer_entry_box)
+#    scrollable_text_frame(Tk.Frame)
+#
+# Provides the following 'compound' UI elements for the application
+#    object_id_selection(Tk.integer_entry_box)
 #    dcc_command_entry() - combines dcc_entry_box and state_box
 #    signal_route_selections() - combines int_item_id_entry_box and 5 state_boxes
 #    selection_buttons() - combines 5 RadioButtons
+#    colour_selection() - Allows the colour of an item to be changed
 #    window_controls() - apply/ok/reset/cancel
 #------------------------------------------------------------------------------------
 
 import tkinter as Tk
+from tkinter import colorchooser
 
 #------------------------------------------------------------------------------------
 # Class to create a tooltip for a tkinter widget - Acknowledgements to Stack Overflow
 # https://stackoverflow.com/questions/3221956/how-do-i-display-tooltips-in-tkinter
+#
 # Class instance elements intended for external use are:
 #     "text" - to change the tooltip text (e.g. to show error messages)
 #------------------------------------------------------------------------------------
 
 class CreateToolTip():
     def __init__(self, widget, text:str='widget info'):
         self.waittime = 500     #miliseconds
@@ -72,22 +78,26 @@
         
     def hidetip(self):
         tw = self.tw
         self.tw= None
         if tw: tw.destroy()
 
 #------------------------------------------------------------------------------------
-# Base class for a generic Checkbox - Builds on the tkinter checkbutton class.
+# Base class for a generic check_box - Builds on the tkinter checkbutton class.
+# Note the responsibility of the instantiating func/class to 'pack' the check_box.
+#
 # Additional class methods provided are:
-#    "set_value" - will set the CB state (bool)
+#    "set_value" - will set the check_box state (bool)
 #    "get_value" - will return the state (False if disabled) (bool)
-#    "disable" - disables/blanks the CB (i.e. sets it to False)
-#    "enable"  enables/loads the CB (with the last state)
-#    "enable1"/"enable2"/"disable1"/"disable2" - as above but provides an
-#        AND function where both flags need to be set to enable the CB
+#    "disable/disable1/disable2" - disables/blanks the check_box
+#    "enable/enable1/enable2"  enables/loads the check_box (with the last state)
+#
+# Note that check_box is created as 'enabled' - the individual functions provide
+# an AND function where all three flags need to be 'enabled' to enable the 
+# check_box. Any of the 3 flags can be 'disabled' to disable the check_box.
 #------------------------------------------------------------------------------------
 
 class check_box(Tk.Checkbutton):
     def __init__(self, parent_frame, label:str, tool_tip:str, width:int=None, callback=None):
         # Create the local instance configuration variables
         # 'selection' is the current CB state and 'state' is the last entered state
         # 'enabled' is the flag to track whether the checkbox is enabled or not
@@ -151,23 +161,27 @@
             self.selection.set(new_value)
 
     def get_value(self):
         # Will always return False if disabled
         return (self.selection.get())
 
 #------------------------------------------------------------------------------------
-# Base class for a generic State Box (like a check box but with labels for off/on 
+# Base class for a generic state_box (like a check box but with labels for off/on 
 # and blank when disabled) - Builds on the tkinter checkbutton class.
+# Note the responsibility of the instantiating func/class to 'pack' the state_box.
+#
 # Additional class methods provided are:
-#    "set_value" - will set the CB state (bool)
+#    "set_value" - will set the state_box state (bool)
 #    "get_value" - will return the current state (False if disabled) (bool)
-#    "disable" - disables/blanks the CB (i.e. sets it to False)
-#    "enable"  enables/loads the CB (with the last state)
-#    "enable1"/"enable2"/"disable1"/"disable2" - as above but provides an
-#        AND function where both flags need to be set to enable the CB
+#    "disable/disable1/disable2" - disables/blanks the state_box
+#    "enable/enable1/enable2"  enables/loads the state_box (with the last state)
+#
+# Note that state_box is created as 'enabled' - the individual functions provide
+# an AND function where all three flags need to be 'enabled' to enable the 
+# state_box. Any of the 3 flags can be 'disabled' to disable the state_box.
 #------------------------------------------------------------------------------------
 
 class state_box(Tk.Checkbutton):
     def __init__(self, parent_frame, label_off:str, label_on:str, tool_tip:str,
                          width:int=None, callback=None, read_only:bool=False):
         # Create the local instance configuration variables
         # 'selection' is the current CB state and 'state' is the last entered state
@@ -245,29 +259,35 @@
         self.update_cb_state()
         
     def get_value(self,):
         # Will always return False if disabled
         return (self.selection.get())
 
 #------------------------------------------------------------------------------------
-# Common Base Class for a generic "Entry box" - Builds on the tkinter Entry class.
+# Common Base Class for a generic entry_box - Builds on the tkinter Entry class.
+# This will accept any string value to be entered/displayed with no validation.
+# Note the responsibility of the instantiating func/class to 'pack' the entry_box.
+#
 # Additional class methods provided are:
-#    "set_value" - set the initial value of the entry box (string) 
-#    "get_value" - get the last "validated" value of the entry box (string) 
-#    "get_initial_value" - get the initial value of the entry box (string)
+#    "set_value" - set the initial value of the entry_box (string) 
+#    "get_value" - get the last "validated" value of the entry_box (string) 
+#    "get_initial_value" - get the initial value of the entry_box (string)
 #    "validate" - This gets overridden by the child class function
-#    "disable" - disables/blanks the entry box
-#    "enable"  enables/loads the entry box (with the last value)
-#    "enable1"/"enable2"/"disable1"/"disable2" - as above but provides an
-#        AND function where both flags need to be set to enable the EB
+#    "disable/disable1/disable2" - disables/blanks the entry_box
+#    "enable/enable1/enable2"  enables/loads the entry_box (with the last state)
+#
+# Note that entry_box is created as 'enabled' - the individual functions provide
+# an AND function where all three flags need to be 'enabled' to enable the 
+# entry_box. Any of the 3 flags can be 'disabled' to disable the entry_box.
+#
 # Class methods/objects intended for use by child classes that inherit:
 #    "set_validation_status" - to be called following external validation
-#    "TT.text" - The tooltip for the entry box (to change the tooltip text)
-#    "entry" - is the current entry box value (may or may not be valid)
-#    "value" - is the last validated value of the entry box
+#    "TT.text" - The tooltip for the entry_box (to change the tooltip text)
+#    "entry" - is the current entry_box value (may or may not be valid)
+#    "value" - is the last validated value of the entry_box
 #------------------------------------------------------------------------------------
 
 class entry_box(Tk.Entry):
     def __init__(self, parent_frame, width:int, tool_tip:str, callback=None):
         # Create the local instance configuration variables
         # 'entry' is the current EB value and 'value' is the last entered value
         # 'enabled' is the flag to track whether the checkbox is enabled or not
@@ -357,28 +377,37 @@
         if self.enabled0 and self.enabled1 and self.enabled2: return(self.value)
         else: return("")
 
     def get_initial_value(self):
         return(self.initial_value)
 
 #------------------------------------------------------------------------------------
-# Common Class for an "Integer Entry box" - builds on the Entry Box class (above)
+# Common Class for an integer_entry_box - builds on the entry_box class (above).
+# This will only allow valid integers (within the defined range) to be entered.
+# Note the responsibility of the instantiating func/class to 'pack' the entry_box.
+#
 # Public class instance methods inherited from the base Entry Box class are:
-#    "disable" - disables/blanks the entry box 
-#    "enable"  enables/loads the entry box (with the last value)
+#    "disable/disable1/disable2" - disables/blanks the entry_box
+#    "enable/enable1/enable2"  enables/loads the entry_box (with the last state)
+#
+# Note that entry_box is created as 'enabled' - the individual functions provide
+# an AND function where all three flags need to be 'enabled' to enable the 
+# entry_box. Any of the 3 flags can be 'disabled' to disable the entry_box.
+#
 # Public class instance methods overridden by this class are
-#    "set_value" - set the initial value of the entry box (int) 
-#    "get_value" - get the last "validated" value of the entry box (int) 
-#    "get_initial_value" - get the initial value of the entry box (int) 
-#    "validate" - Validates an integer, within range and whether empty 
+#    "set_value" - set the initial value of the entry_box (int) 
+#    "get_value" - get the last "validated" value of the entry_box (int) 
+#    "get_initial_value" - get the initial value of the entry_box (int) 
+#    "validate" - Validates an integer, within range and whether empty
+#
 # Class methods/objects intended for use by child classes that inherit:
 #    "set_validation_status" - to be called following external validation
-#    "TT.text" - The tooltip for the entry box (to change the tooltip text)
-#    "entry" - is the current entry box value (may or may not be valid)
-#    "value" - is the last validated value of the entry box
+#    "TT.text" - The tooltip for the entry_box (to change the tooltip text)
+#    "entry" - is the current entry_box value (may or may not be valid)
+#    "value" - is the last validated value of the entry_box
 #------------------------------------------------------------------------------------
 
 class integer_entry_box(entry_box):
     def __init__(self, parent_frame, width:int, min_value:int, max_value:int,
                        tool_tip:str, callback=None, allow_empty:bool=True):
         # Store the local instance configuration variables
         self.empty_allowed = allow_empty
@@ -422,42 +451,48 @@
         else: return(int(super().get_value()))
 
     def get_initial_value(self):
         if super().get_initial_value() == "": return(0)
         else: return(int(super().get_initial_value()))
 
 #------------------------------------------------------------------------------------
-# Common class for a DCC address entry box - builds on the Integer Entry Box class
-# Public class instance methods inherited from the base Entry Box class are:
-#    "disable" - disables/blanks the entry box 
-#    "enable"  enables/loads the entry box (with the last value)
-#    "set_value" - set the initial value of the entry box (int) 
-#    "get_value" - get the last "validated" value of the entry box (int) 
+# Common class for a DCC address entry box - builds on the integer_entry_box class
+# Adds additional validation to ensure the DCC Address is within the valid range.
+# Note the responsibility of the instantiating func/class to 'pack' the entry_box.
+#
+# Public class instance methods inherited from the base entry_box class are:
+#    "disable" - disables/blanks the entry_box 
+#    "enable"  enables/loads the entry_box (with the last value)
+#    "set_value" - set the initial value of the entry_box (int) 
+#    "get_value" - get the last "validated" value of the entry_box (int) 
 #    "validate" - Validates an integer, within range and whether empty 
 #------------------------------------------------------------------------------------
 
 class dcc_entry_box (integer_entry_box):
     def __init__(self, parent_frame, callback=None,
             tool_tip:str="Enter a DCC address (1-2047) or leave blank"):
         # Call the common base class init function to create the EB
         super().__init__(parent_frame, width=4 , min_value=1, max_value=2047,
                             tool_tip=tool_tip, callback=callback)
 
 #------------------------------------------------------------------------------------
-# Common class for an Item-specific Integer entry box - builds on the Integer Entry Box
+# Common class for an int_item_id_entry_box - builds on the integer_entry_box
 # These classes are for entering local signal/point/instrument/section IDs (integers)
 # They do not accept remote Signal or Instrument IDs (where the ID can be an int or str)
 # The class uses the 'exists_function' to check that the item exists on the schematic
 # If a 'current_id_function' is specified then this function is also used to validate
 # that the entered ID is not the same as the current ID of the item.
-# Public class instance methods inherited from the base Integer Entry Box are:
-#    "disable" - disables/blanks the entry box 
-#    "enable"  enables/loads the entry box (with the last value)
-#    "set_value" - set the initial value of the entry box (int) 
-#    "get_value" - get the last "validated" value of the entry box (int) 
+# Note the responsibility of the instantiating func/class to 'pack' the entry_box.
+#
+# Public class instance methods inherited from the base integer_entry_box are:
+#    "disable" - disables/blanks the entry_box 
+#    "enable"  enables/loads the entry_box (with the last value)
+#    "set_value" - set the initial value of the entry_box (int) 
+#    "get_value" - get the last "validated" value of the entry_box (int)
+#
 # Public class instance methods overridden by this class are
 #    "validate" - Validation as described above 
 #------------------------------------------------------------------------------------
 
 class int_item_id_entry_box (integer_entry_box):
     def __init__(self, parent_frame, tool_tip:str, callback=None, allow_empty=True,
                             exists_function=None, current_id_function=None):
@@ -481,24 +516,27 @@
                 if self.entry.get() == str(self.current_id_function()):
                     self.TT.text = "Entered ID is the same as the current Item ID"
                     valid = False
         if update_validation_status: self.set_validation_status(valid)
         return(valid)
 
 #------------------------------------------------------------------------------------
-# Common class for an Item-specific String entry box - builds on the common Entry Box
-# These classes are for entering LOCAL or REMOTE signal or instrument IDs (where the ID
-# can be an int or str). The class uses the 'exists_function' to check that the item exists
-# on the schematic. If a 'current_id_function' is specified then this function is also used
+# Common class for a str_item_id_entry_box - builds on the common entry_box class.
+# These classes are for entering LOCAL or REMOTE item IDs (where the ID can be an int
+# or str). The class uses the 'exists_function' to check that the item exists on the
+# schematic. If a 'current_id_function' is specified then this function is also used
 # to validate that the entered ID is not the same as the current ID of the item.
-# Public class instance methods inherited from the base Entry Box class are:
-#    "disable" - disables/blanks the entry box 
-#    "enable"  enables/loads the entry box (with the last value)
-#    "set_value" - set the initial value of the entry box (str) 
-#    "get_value" - get the last "validated" value of the entry box (str) 
+# Note the responsibility of the instantiating func/class to 'pack' the entry_box.
+#
+# Public class instance methods inherited from the base entry_box class are:
+#    "disable" - disables/blanks the entry_box 
+#    "enable"  enables/loads the entry_box (with the last value)
+#    "set_value" - set the initial value of the entry_box (str) 
+#    "get_value" - get the last "validated" value of the entry_box (str)
+#
 # Public class instance methods overridden by this class are
 #    "validate" - Validation as described above 
 #------------------------------------------------------------------------------------
 
 class str_item_id_entry_box (entry_box):
     def __init__(self, parent_frame, tool_tip:str, callback=None,
                  exists_function = None, current_id_function=None):
@@ -542,25 +580,108 @@
             if self.entry.get() == str(self.current_id_function()):
                 self.TT.text = "Entered ID is the same as the current Item ID"
                 valid = False
         if update_validation_status: self.set_validation_status(valid)
         return(valid)
 
 #------------------------------------------------------------------------------------
-# Common Class for an "Object ID" Entry Frame - builds on the Integer Entry Box class
-# This is used across all object edit windows for displaying / changing the item ID
-# Public class instance methods inherited from the base Integer Entry Box are:
-#    "disable" - disables/blanks the entry box 
-#    "enable"  enables/loads the entry box (with the last value)
-#    "set_value" - set the initial value of the entry box (int) 
-#    "get_value" - get the last "validated" value of the entry box (int) 
-#    "get_initial_value" - get the initial value of the entry box (int)
+# Class for a scrollable_text_frame - can be editable (e.g. entering layout info)
+# or non-editable (e.g. displaying a list of warnings)- can also be configured
+# to re-size automatically (within the specified limits) as text is entered.
+# The text box will 'fit' to the content unless max or min dimentions are
+# specified for the width and/or height - then the scrollbars can be used.
+# Note the responsibility of the instantiating func/class to 'pack' the entry_box.
+#
+# Public class instance methods provided by this class are
+#    "set_value" - will set the current value (str)
+#    "get_value" - will return the current value (str)
+#------------------------------------------------------------------------------------
+
+class scrollable_text_frame(Tk.Frame):
+    def __init__(self, parent_window, max_height:int=None, min_height:int=None, editable:bool=False,
+                 max_width:int=None, min_width:int=None, auto_resize:bool=False):
+        # Store the parameters we need
+        self.min_height = min_height
+        self.max_height = max_height
+        self.min_width = min_width
+        self.max_width = max_width
+        self.editable = editable
+        self.auto_resize = auto_resize
+        self.text=""
+        # Create a frame for the text widget and scrollbars
+        super().__init__(parent_window)
+        # Create a subframe for the text and scrollbars
+        self.subframe = Tk.Frame(self)
+        self.subframe.pack(fill=Tk.BOTH, expand=True)
+        # Create the text widget and vertical scrollbars in the subframe
+        self.text_box = Tk.Text(self.subframe, wrap=Tk.NONE)
+        self.text_box.insert(Tk.END,self.text)
+        hbar = Tk.Scrollbar(self.subframe, orient=Tk.HORIZONTAL)
+        hbar.pack(side=Tk.BOTTOM, fill=Tk.X)
+        hbar.config(command=self.text_box.xview)
+        vbar = Tk.Scrollbar(self.subframe, orient=Tk.VERTICAL)
+        vbar.pack(side=Tk.RIGHT, fill=Tk.Y)
+        vbar.config(command=self.text_box.yview)
+        self.text_box.config(xscrollcommand=hbar.set, yscrollcommand=vbar.set)
+        self.text_box.pack(side=Tk.LEFT, expand=True, fill=Tk.BOTH)
+        # configure the window for editable or non-editable
+        if not self.editable: self.text_box.config(state="disabled")
+        # Set up the callback for auto re-size (if specified)
+        if self.auto_resize: self.text_box.bind("<Key>", self.resize_text_box)
+        # Set the initial size for the text box
+        self.resize_text_box()
+
+    def resize_text_box(self, event=None):
+        # Calculate the height and width of the text
+        self.text = self.text_box.get("1.0",Tk.END)
+        list_of_lines = self.text.splitlines()
+        number_of_lines = len(list_of_lines)
+        max_line_length = 0
+        for line in list_of_lines:
+            if len(line) > max_line_length: max_line_length = len(line)
+        # Apply the specified size constraints
+        if self.min_height is not None and number_of_lines < self.min_height:
+            number_of_lines = self.min_height
+        if self.max_height is not None and number_of_lines > self.max_height:
+            number_of_lines = self.max_height
+        if self.min_width is not None and max_line_length < self.min_width:
+            max_line_length = self.min_width
+        if self.max_width is not None and max_line_length > self.max_width:
+            max_line_length = self.max_width
+        # re-size the text box
+        self.text_box.config(height=number_of_lines+1, width=max_line_length+1)
+        
+    def set_value(self, text:str):
+        self.text = text
+        if not self.editable: self.text_box.config(state="normal")
+        self.text_box.delete("1.0",Tk.END)
+        self.text_box.insert(Tk.INSERT, self.text)
+        if not self.editable: self.text_box.config(state="disabled")
+        self.resize_text_box()
+    
+    def get_value(self):
+        self.text = self.text_box.get("1.0",Tk.END)
+        return(self.text)
+    
+#------------------------------------------------------------------------------------
+# Compound UI element for an object_id_selection LabelFrame - uses the integer_entry_box.
+# This is used across all object windows for displaying / changing the item ID.
+# Note the responsibility of the instantiating func/class to 'pack' the Frame of
+# the UI element - i.e. '<class_instance>.frame.pack()'
+#
+# Public class instance methods inherited from the base integer_entry_box are:
+#    "disable" - disables/blanks the entry_box 
+#    "enable"  enables/loads the entry_box (with the last value)
+#    "set_value" - set the initial value of the entry_box (int) 
+#    "get_value" - get the last "validated" value of the entry_box (int) 
+#    "get_initial_value" - get the initial value of the entry_box (int)
+#
 # Public class instance methods overridden by this class are
 #    "validate" - Validates that the entered Item ID is "free" (and can therefore be
-#               assigned to this item) or is being changed back to the initial value
+#               assigned to this item) or is being changed back to the initial value.
 #------------------------------------------------------------------------------------
 
 class object_id_selection(integer_entry_box):
     def __init__(self, parent_frame, label:str, exists_function):
         # This is the function to call to see if the object already exists
         self.exists_function = exists_function
         # Create a Label Frame for the UI element
@@ -583,32 +704,37 @@
             if self.exists_function(new_id) and new_id != current_id:
                 self.TT.text = "ID already assigned"
                 valid = False
         self.set_validation_status(valid)
         return(valid)
 
 #------------------------------------------------------------------------------------
-# Common class for a DCC command (address + command logic) entry element box
-# Uses the dcc_entry_box and state_box classes from above
+# Compound UI element for a dcc_command_entry (address + command logic).
+# Uses the common dcc_entry_box and state_box classes. Note that the state_box
+# is only enabled when a valid DCC address has been entered into the entry_box.
+# This is used across all object windows for displaying / changing the item ID.
+# Note the responsibility of the instantiating func/class to 'pack' the Frame of
+# the UI element - i.e. '<class_instance>.frame.pack()'
+#
 # Public class instance methods provided by this class are
-#    "validate" - validate the current entry box value and return True/false
+#    "validate" - validate the current entry_box value and return True/false
 #    "set_value" - will set the current value [address:int, state:bool]
 #    "get_value" - will return the last "valid" value [address:int, state:bool]
-#    "disable" - disables/blanks the entry box (and associated state button)
-#    "enable"  enables/loads the entry box (and associated state button)
+#    "disable" - disables/blanks the entry_box (and associated state button)
+#    "enable"  enables/loads the entry_box (and associated state button)
 #------------------------------------------------------------------------------------
 
 class dcc_command_entry():
     def __init__(self, parent_frame):
         # create a frame to pack the two elements into
         self.frame = Tk.Frame(parent_frame)
         # Create the address entry box and the associated dcc state box
-        self.EB = dcc_entry_box(parent_frame, callback=self.eb_updated)
+        self.EB = dcc_entry_box(self.frame, callback=self.eb_updated)
         self.EB.pack(side=Tk.LEFT)
-        self.CB = state_box(parent_frame, label_off="OFF", label_on="ON",
+        self.CB = state_box(self.frame, label_off="OFF", label_on="ON",
                     width=4, tool_tip="Set the DCC logic for the command")
         self.CB.pack(side=Tk.LEFT)
     
     def eb_updated(self):
         if self.EB.entry.get() == "":
             self.CB.disable()
         else: self.CB.enable()
@@ -633,143 +759,117 @@
     def get_value(self):
         # Returns a 2 element list of [DCC_Address, DCC_State]
         # When disabled (or empty) will always return [0, False]
         # When invalid will return [last valid address, current state]
         return([self.EB.get_value(), self.CB.get_value()])
 
 #------------------------------------------------------------------------------------
-# Common class for a route selection element (route selection CBs)
-# Public class instance methods provided by this class are
-#    "set_values" - Sets the route selection CBs 
-#    "get_values" - Gets route selection CBs 
-#    "enable" - Enables/loads the route selection CBs 
-#    "disable" - Disables/blanks the route selection CBs 
-#------------------------------------------------------------------------------------
-
-class route_selections():
-    def __init__(self, parent_frame, tool_tip:str, read_only=False, callback=None):
-        # create the UI Elements for each of the possible route selections
-        self.main = state_box(parent_frame, label_off="MAIN", label_on="MAIN",
-                width=5, tool_tip=tool_tip, read_only=read_only, callback=callback)
-        self.main.pack(side=Tk.LEFT)
-        self.lh1 = state_box(parent_frame, label_off="LH1", label_on="LH1",
-                width=4, tool_tip=tool_tip, read_only=read_only, callback=callback)
-        self.lh1.pack(side=Tk.LEFT)
-        self.lh2 = state_box(parent_frame, label_off="LH2", label_on="LH2",
-                width=4, tool_tip=tool_tip, read_only=read_only, callback=callback)
-        self.lh2.pack(side=Tk.LEFT)
-        self.rh1 = state_box(parent_frame, label_off="RH1", label_on="RH1",
-                width=4, tool_tip=tool_tip, read_only=read_only, callback=callback)
-        self.rh1.pack(side=Tk.LEFT)
-        self.rh2 = state_box(parent_frame, label_off="RH2", label_on="RH2",
-                width=4, tool_tip=tool_tip, read_only=read_only, callback=callback)
-        self.rh2.pack(side=Tk.LEFT)
-
-    def enable(self):
-        self.main.enable()
-        self.lh1.enable()
-        self.lh2.enable()
-        self.rh1.enable()
-        self.rh2.enable()
-
-    def disable(self):
-        self.main.disable()
-        self.lh1.disable()
-        self.lh2.disable()
-        self.rh1.disable()
-        self.rh2.disable()
-
-    def set_values(self, routes:[bool,bool,bool,bool,bool]):
-        # A 'Route' comprises a list of route selections [main, lh1, lh2, rh1, rh2]
-        # Where each route selection is a boolean value (True or False)
-        self.main.set_value(routes[0])
-        self.lh1.set_value(routes[1])
-        self.lh2.set_value(routes[2])
-        self.rh1.set_value(routes[3])
-        self.rh2.set_value(routes[4])
-
-    def get_values(self):
-        # A 'Route' comprises a list of route selections [main, lh1, lh2, rh1, rh2]
-        # Where each route selection is a boolean value (True or False)
-        return ( [ self.main.get_value(),
-                   self.lh1.get_value(),
-                   self.lh2.get_value(),
-                   self.rh1.get_value(),
-                   self.rh2.get_value() ])
-
-#------------------------------------------------------------------------------------
-# Class for a signal route selection element (Sig ID EB + route selection CBs)
-# Used by the signals and points interlocking tabs (read only for points tab)
-# Inherits from the common route_selections class (above)
+# Compound UI Element for a signal route selections (Sig ID EB + route selection CBs)
+# Note the responsibility of the instantiating func/class to 'pack' the Frame of
+# the UI element - i.e. '<class_instance>.frame.pack()'
+#
 # Public class instance methods provided by this class are
 #    "validate" - Checks whether the entry is a valid Item Id 
 #    "set_values" - Sets the EB value and all route selection CBs 
 #    "get_values" - Gets the EB value and all route selection CBs 
 #    "enable" - Enables/loads the EB value and all route selection CBs 
 #    "disable" - Disables/blanks EB value and all route selection CBs 
 #------------------------------------------------------------------------------------
 
-class signal_route_selections(route_selections):
+class signal_route_selections():
     def __init__(self, parent_frame, tool_tip:str, exists_function=None,
                   current_id_function=None, read_only:bool=False):
         self.read_only = read_only
-        # Create a fFrame to hold all the elements
+        # Create a Frame to hold all the elements
         self.frame = Tk.Frame(parent_frame)
         # Call the common base class init function to create the EB
         self.EB = int_item_id_entry_box(self.frame, tool_tip=tool_tip, callback=self.eb_updated,
                     exists_function=exists_function, current_id_function=current_id_function)
         self.EB.pack(side=Tk.LEFT)
         # Disable the EB (we don't use the disable method as we want to display the value_
         if self.read_only: self.EB.configure(state="disabled")
         # Create the UI Elements for each of the possible route selections
-        super().__init__(self.frame, tool_tip, read_only)
+        self.main = state_box(self.frame, label_off="MAIN", label_on="MAIN",
+                width=5, tool_tip=tool_tip, read_only=read_only)
+        self.main.pack(side=Tk.LEFT)
+        self.lh1 = state_box(self.frame, label_off="LH1", label_on="LH1",
+                width=4, tool_tip=tool_tip, read_only=read_only)
+        self.lh1.pack(side=Tk.LEFT)
+        self.lh2 = state_box(self.frame, label_off="LH2", label_on="LH2",
+                width=4, tool_tip=tool_tip, read_only=read_only)
+        self.lh2.pack(side=Tk.LEFT)
+        self.rh1 = state_box(self.frame, label_off="RH1", label_on="RH1",
+                width=4, tool_tip=tool_tip, read_only=read_only)
+        self.rh1.pack(side=Tk.LEFT)
+        self.rh2 = state_box(self.frame, label_off="RH2", label_on="RH2",
+                width=4, tool_tip=tool_tip, read_only=read_only)
+        self.rh2.pack(side=Tk.LEFT)
 
     def eb_updated(self):
         # Enable/disable the checkboxes depending on the EB state
         if not self.read_only:
             if self.EB.entry.get() == "":
-                super().disable()
+                self.main.disable()
+                self.lh1.disable()
+                self.lh2.disable()
+                self.rh1.disable()
+                self.rh2.disable()
             else:
-                super().enable()
+                self.main.enable()
+                self.lh1.enable()
+                self.lh2.enable()
+                self.rh1.enable()
+                self.rh2.enable()
     
     def validate(self):
         return(self.EB.validate())
     
     def enable(self):
         self.EB.enable()
         self.eb_updated()
         
     def disable(self):
         self.EB.disable()
         self.eb_updated()
-        
+
     def set_values(self, signal:[int,[bool,bool,bool,bool,bool]]):
         # Each signal comprises [sig_id, [main, lh1, lh2, rh1, rh2]]
         # Where each route element is a boolean value (True or False)
         self.EB.set_value(signal[0])
-        super().set_values(signal[1])
+        self.main.set_value(signal[1][0])
+        self.lh1.set_value(signal[1][1])
+        self.lh2.set_value(signal[1][2])
+        self.rh1.set_value(signal[1][3])
+        self.rh2.set_value(signal[1][4])
         self.eb_updated()
 
     def get_values(self):
         # each signal comprises [sig_id, [main, lh1, lh2, rh1, rh2]]
         # Where each route element is a boolean value (True or False)
-        return ( [ self.EB.get_value(), super().get_values() ])
+        return ( [ self.EB.get_value(), [ self.main.get_value(),
+                                          self.lh1.get_value(),
+                                          self.lh2.get_value(),
+                                          self.rh1.get_value(),
+                                          self.rh2.get_value() ] ])
 
 #------------------------------------------------------------------------------------
-# Class for a signal route interlocking frame - uses multiple instances of the
-# signal_route_selection_element which are created when "set_values" is called
+# Compound UI Element for a signal route interlocking LabelFrame - creates a variable
+# number of instances of the signal_route_selection_element when "set_values" is called
+# (according to the length of the supplied list).Note that this is a 'read-only' element.
+# Note the responsibility of the instantiating func/class to 'pack' the Frame of
+# the UI element - i.e. '<class_instance>.frame.pack()'
+#
 # Public class instance methods provided by this class are:
 #    "set_values" - Populates the list of interlocked signals and their routes
 #------------------------------------------------------------------------------------
 
 class signal_route_interlocking_frame():
     def __init__(self, parent_frame):
         # Create the Label Frame for the Signal Interlocking List 
         self.frame = Tk.LabelFrame(parent_frame, text="Interlocking with signals")
-        self.frame.pack(padx=2, pady=2, fill='x')
         # These are the lists that hold the references to the subframes and subclasses
         self.sigelements = []
         self.subframe = None
 
     def set_values(self, sig_interlocking_frame:[[int,[bool,bool,bool,bool,bool]],]):
         # If the lists are not empty (case of "reloading" the config) then destroy
         # all the UI elements and create them again (the list may have changed)
@@ -787,17 +887,21 @@
                 self.sigelements[-1].frame.pack()
                 self.sigelements[-1].set_values (sig_interlocking_routes)
         else:
             self.label = Tk.Label(self.subframe, text="No interlocked signals")
             self.label.pack()
 
 #------------------------------------------------------------------------------------
-# Class for a frame containing up to 5 radio buttons
+# Compound UI Element for a LabelFrame containing up to 5 radio buttons
+# Note the responsibility of the instantiating func/class to 'pack' the Frame of
+# the UI element - i.e. '<class_instance>.frame.pack()'
+#
 # Class instance elements to use externally are:
 #    "B1" to "B5 - to access the button widgets (i.e. for reconfiguration)
+#
 # Class instance functions to use externally are:
 #    "set_value" - will set the current value (integer 1-5)
 #    "get_value" - will return the last "valid" value (integer 1-5)
 #------------------------------------------------------------------------------------
 
 class selection_buttons():
     def __init__(self, parent_frame, label:str, tool_tip:str, callback=None, 
@@ -844,27 +948,67 @@
     def set_value(self, value:int):
         self.value.set(value)
 
     def get_value(self):
         return(self.value.get())
 
 #------------------------------------------------------------------------------------
-# Class for the common Apply/OK/Reset/Cancel Buttons - will make external callbacks
+# Compound UI Element for Colour selection
+# Note the responsibility of the instantiating func/class to 'pack' the Frame of
+# the UI element - i.e. '<class_instance>.frame.pack()'
+#
+# Class instance functions to use externally are:
+#    "set_value" - will set the current value (colour code string)
+#    "get_value" - will return the last "valid" value (colour code string)
+#------------------------------------------------------------------------------------
+
+class colour_selection():
+    def __init__(self, parent_frame):
+        # Variable to hold the currently selected colour:
+        self.colour ='black'
+        # Create a frame to hold the tkinter widgets
+        # The parent class is responsible for packing the frame
+        self.frame = Tk.LabelFrame(parent_frame,text="Colour")
+        # Create a sub frame for the UI elements to centre them
+        self.subframe = Tk.Frame(self.frame)
+        self.subframe.pack()
+        self.label2 = Tk.Label(self.subframe, width=3, bg=self.colour)
+        self.label2.pack(side=Tk.LEFT, padx=2, pady=2)
+        self.TT2 = CreateToolTip(self.label2, "Currently selected colour")
+        self.B1 = Tk.Button(self.subframe, text="Change", command=self.update)
+        self.B1.pack(side=Tk.LEFT, padx=2, pady=2)
+        self.TT2 = CreateToolTip(self.B1, "Open colour chooser dialog")
+        
+    def update(self):
+        colour_code = colorchooser.askcolor(parent=self.frame, title ="Select Colour")
+        self.colour = colour_code[1]
+        self.label2.config(bg=self.colour)
+        
+    def get_value(self):
+        return(self.colour)
+        
+    def set_value(self,colour:str):
+        self.colour = colour
+        self.label2.config(bg=self.colour)
+
+#------------------------------------------------------------------------------------
+# Compound UI element for the Apply/OK/Reset/Cancel Buttons - will make callbacks
 # to the specified "load_callback" and "save_callback" functions as appropriate 
+# Note the responsibility of the instantiating func/class to 'pack' the Frame of
+# the UI element - i.e. '<class_instance>.frame.pack()'
 #------------------------------------------------------------------------------------
 
 class window_controls():
     def __init__(self, parent_window, parent_object, load_callback, save_callback):
         # Create the class instance variables
         self.window = parent_window
         self.save_callback = save_callback
         self.load_callback = load_callback
         self.parent_object = parent_object
         self.frame = Tk.Frame(self.window)
-        self.frame.pack(padx=2, pady=2)
         # Create the buttons and tooltips
         self.B1 = Tk.Button (self.frame, text = "Ok",command=self.ok)
         self.B1.pack(side=Tk.LEFT, padx=2, pady=2)
         self.TT1 = CreateToolTip(self.B1, "Apply selections and close window")
         self.B2 = Tk.Button (self.frame, text = "Apply",command=self.apply)
         self.B2.pack(side=Tk.LEFT, padx=2, pady=2)
         self.TT2 = CreateToolTip(self.B2, "Apply selections")
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/editor/configure_instrument.py` & `model-railway-signals-3.4.0/model_railway_signals/editor/configure_instrument.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 #------------------------------------------------------------------------------------
 #
 # External API functions intended for use by other editor modules:
 #    edit_instrument - Open the edit block instrument top level window
 #
 # Makes the following external API calls to other editor modules:
 #    objects.update_object(obj_id,new_obj) - Update the configuration on save
-#    objects.instrument_exists(item_id) - To see if a specified instrument ID exists
 #
 # Accesses the following external editor objects directly:
 #    objects.signal_index - To iterate through all the signal objects
 #    objects.schematic_objects - To load/save the object configuration
 #
+# Makes the following external API calls to library modules:
+#    block_instruments.instrument_exists(id) - To see if the instrument exists
+#
 # Inherits the following common editor base classes (from common):
 #    common.str_item_id_entry_box
 #    common.entry_box
 #    common.create_tool_tip
 #    common.object_id_selection
 #    common.selection_buttons
 #    common.signal_route_interlocking_frame
@@ -31,19 +33,21 @@
 
 import tkinter as Tk
 from tkinter import ttk
 
 from . import common
 from . import objects
 
+from ..library import block_instruments
+
 # We can only use audio for the block instruments if 'simpleaudio' is installed
 # Although this package is supported across different platforms, for Windows
 # it has a dependency on Visual C++ 14.0. As this is quite a faff to install I
 # haven't made audio a hard and fast dependency for the 'model_railway_signals'
-# pack age as a whole - its up to the user to install if required
+# package as a whole - its up to the user to install if required
 
 def is_simpleaudio_installed():
     global simpleaudio
     try:
         import simpleaudio
         return (True)
     except Exception: pass
@@ -70,15 +74,15 @@
         for route_index, signal_route in enumerate(signal_routes):
             # Test to see if the signal route is configured to be interlocked with this instrument
             # Note that Both of the values we are comparing are integers
             if signal_route[2] == instrument_id:
                 signal_interlocked_by_instrument = True
                 interlocked_routes[route_index] = True
         if signal_interlocked_by_instrument:
-            list_of_interlocked_signals.append([instrument_id,interlocked_routes])
+            list_of_interlocked_signals.append([signal_id,interlocked_routes])
     return(list_of_interlocked_signals)
 
 #------------------------------------------------------------------------------------
 # Function to load the initial UI state when the Edit window is created
 # Also called to re-load the UI state on an "Apply" (i.e. after the save)
 #------------------------------------------------------------------------------------
  
@@ -153,18 +157,15 @@
 #    "validate" - Validates the instrument exists and not the current inst_id
 #------------------------------------------------------------------------------------
 
 class linked_to_selection(common.str_item_id_entry_box):
     def __init__(self, parent_frame, parent_object):
         # These are the functions used to validate that the entered ID
         # exists on the schematic and is different to the current ID
-        ######################################################################################################
-        ## Note that the exists function will need to change when the application supports remote instruments
-        ######################################################################################################
-        exists_function = objects.instrument_exists
+        exists_function = block_instruments.instrument_exists
         current_id_function = parent_object.instid.get_value
         # Create the Label Frame for the "also switch" entry box
         self.frame = Tk.LabelFrame(parent_frame, text="Block section")
         # Call the common base class init function to create the EB
         self.label1 = Tk.Label(self.frame,text="Linked block instrument:")
         self.label1.pack(side=Tk.LEFT, padx=2, pady=2)
         super().__init__(self.frame, tool_tip = "Enter the ID of the linked instrument "+
@@ -206,25 +207,29 @@
         
     def load(self):
         # Use the library resources folder for the initial path for the file dialog
         # But the user can navigate away and use another sound file from somewhere else
         with importlib.resources.path ('model_railway_signals.library', 'resources') as initial_path:
             filename = Tk.filedialog.askopenfilename(title='Select Audio File', initialdir = initial_path,
                     filetypes=(('audio files','*.wav'),('all files','*.*')), parent=self.frame)
-        # Try loading/playing the selected file - with an error popup if it fails
-        if filename != () and filename != "":
-            try:
-                simpleaudio.WaveObject.from_wave_file(filename).play()
-            except:
-                Tk.messagebox.showerror(parent=self.frame, title="Load Error",
-                            message="Error loading audio file '"+str(filename)+"'")
-            else:
-                # Set the filename entry to the name of the current file (split from the dir path)
-                self.set_value(os.path.split(filename)[1])
-                self.full_filename = filename
+            # Try loading/playing the selected file - with an error popup if it fails
+            if filename != () and filename != "":
+                try:
+                    simpleaudio.WaveObject.from_wave_file(filename).play()
+                except:
+                    Tk.messagebox.showerror(parent=self.frame, title="Load Error",
+                                message="Error loading audio file '"+str(filename)+"'")
+                else:
+                    # Set the filename entry to the name of the current file (split from the dir path)
+                    self.set_value(os.path.split(filename)[1])
+                    # If a resources file has been chosen then strip off the path to aid cross-platform
+                    # transfer of layout files (where the path to the resource folder may be different)
+                    if os.path.split(filename)[0] == str(initial_path):
+                        filename = os.path.split(filename)[1]
+                    self.full_filename = filename
 
 #------------------------------------------------------------------------------------
 # Class for the Sound file selections element - uses 2 instances of the element above)
 # Class instance methods provided by this class are:
 #    "set_values" - will set the fully qualified audio filenames (bell, key)
 #    "get_values" - will return the fully qualified audio filenames (bell, key)
 #------------------------------------------------------------------------------------
@@ -254,19 +259,19 @@
 #------------------------------------------------------------------------------------
 
 class instrument_configuration_tab():
     def __init__(self, parent_tab):
         # Create a Frame to hold the Inst ID and Inst Type Selections
         self.frame = Tk.Frame(parent_tab)
         self.frame.pack(padx=2, pady=2, fill='x')
-        # Create the UI Element for Point ID selection
+        # Create the UI Element for Inst ID selection
         self.instid = common.object_id_selection(self.frame, "Inst ID",
-                                exists_function = objects.instrument_exists) 
+                        exists_function = block_instruments.instrument_exists) 
         self.instid.frame.pack(side=Tk.LEFT, padx=2, pady=2, fill='y')
-        # Create the UI Element for Point Type selection
+        # Create the UI Element for Inst Type selection
         self.insttype = common.selection_buttons(self.frame, "Point type",
                     "Select block Instrument Type", None, "Single line", "Double Line")
         self.insttype.frame.pack(padx=2, pady=2, fill='x')
         self.linkedto = linked_to_selection(parent_tab, self)
         self.linkedto.frame.pack(padx=2, pady=2, fill='x')
         self.sounds = sound_file_selections(parent_tab)
         self.sounds.frame.pack(padx=2, pady=2, fill='x')
@@ -274,14 +279,15 @@
 #------------------------------------------------------------------------------------
 # Top level Class for the Block Instrument Interlocking Tab
 #------------------------------------------------------------------------------------
 
 class instrument_interlocking_tab():
     def __init__(self, parent_tab):
         self.signals = common.signal_route_interlocking_frame(parent_tab)
+        self.signals.frame.pack(padx=2, pady=2, fill='x')
 
 #####################################################################################
 # Top level Class for the Edit Block Instrument window
 #####################################################################################
 
 class edit_instrument():
     def __init__(self, root, object_id):
@@ -301,14 +307,15 @@
         self.tab2 = Tk.Frame(self.tabs)
         self.tabs.add(self.tab2, text="Interlocking")
         self.tabs.pack()
         self.config = instrument_configuration_tab(self.tab1)
         self.locking = instrument_interlocking_tab(self.tab2)
         # Create the common Apply/OK/Reset/Cancel buttons for the window
         self.controls = common.window_controls(self.window, self, load_state, save_state)
+        self.controls.frame.pack(padx=2, pady=2)
         # Create the Validation error message (this gets packed/unpacked on apply/save)
         self.validation_error = Tk.Label(self.window, text="Errors on Form need correcting", fg="red")
         # load the initial UI state
         load_state(self)
 
     def tab_changed(self,event):
         # Focus on the top level window to remove focus from the first entry box
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/editor/configure_point.py` & `model-railway-signals-3.4.0/model_railway_signals/editor/configure_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 #    common.int_item_id_entry_box
 #    common.check_box
 #    common.dcc_entry_box
 #    common.object_id_selection
 #    common.selection_buttons
 #    common.signal_route_interlocking_frame
 #    common.signal_route_selections
+#    common.colour_selector
 #    common.window_controls
 #
 #------------------------------------------------------------------------------------
 
 import copy
 
 import tkinter as Tk
@@ -63,14 +64,15 @@
         # Label the edit window with the Point ID
         point.window.title("Point "+str(objects.schematic_objects[object_id]["itemid"]))
         # Set the Initial UI state from the current object settings
         point.config.pointid.set_value(objects.schematic_objects[object_id]["itemid"])
         point.config.alsoswitch.set_value(objects.schematic_objects[object_id]["alsoswitch"])
         point.config.alsoswitch.set_switched_with(switched_with_point(object_id))
         point.config.pointtype.set_value(objects.schematic_objects[object_id]["itemtype"])
+        point.config.colour.set_value(objects.schematic_objects[object_id]["colour"])
         # These are the general settings for the point
         auto = objects.schematic_objects[object_id]["automatic"]
         rev = objects.schematic_objects[object_id]["reverse"]
         fpl = objects.schematic_objects[object_id]["hasfpl"]
         if objects.schematic_objects[object_id]["orientation"] == 180: rot = True
         else:rot = False
         point.config.settings.set_values(rot, rev, auto, fpl)
@@ -98,14 +100,15 @@
              point.config.settings.validate() and point.config.dccsettings.validate()):
         # Copy the original point Configuration (elements get overwritten as required)
         new_object_configuration = copy.deepcopy(objects.schematic_objects[object_id])
         # Update the point coniguration elements from the current user selections
         new_object_configuration["itemid"] = point.config.pointid.get_value()
         new_object_configuration["itemtype"] = point.config.pointtype.get_value()
         new_object_configuration["alsoswitch"] = point.config.alsoswitch.get_value()
+        new_object_configuration["colour"] = point.config.colour.get_value()
         # These are the general settings
         rot, rev, auto, fpl = point.config.settings.get_values()
         new_object_configuration["reverse"] = rev
         new_object_configuration["automatic"] = auto
         new_object_configuration["hasfpl"] = fpl
         if rot: new_object_configuration["orientation"] = 180
         else: new_object_configuration["orientation"] = 0
@@ -305,25 +308,28 @@
     
 #------------------------------------------------------------------------------------
 # Top level Class for the Point Configuration Tab
 #------------------------------------------------------------------------------------
 
 class point_configuration_tab():
     def __init__(self, parent_tab):
-        # Create a Frame to hold the Point ID and Point Type Selections
+        # Create a Frame to hold the Point ID, Point Type and point colour Selections
         self.frame = Tk.Frame(parent_tab)
         self.frame.pack(padx=2, pady=2, fill='x')
         # Create the UI Element for Point ID selection
         self.pointid = common.object_id_selection(self.frame, "Point ID",
                                 exists_function = objects.point_exists) 
         self.pointid.frame.pack(side=Tk.LEFT, padx=2, pady=2, fill='y')
         # Create the UI Element for Point Type selection
         self.pointtype = common.selection_buttons(self.frame, "Point type",
                                       "Select Point Type", None, "RH", "LH")
-        self.pointtype.frame.pack(padx=2, pady=2, fill='x')
+        self.pointtype.frame.pack(side=Tk.LEFT, padx=2, pady=2, fill='y')
+        # Create the Point colour selection element
+        self.colour = common.colour_selection(self.frame)
+        self.colour.frame.pack(side=Tk.LEFT,padx=2, pady=2, fill='y')
         # Create the UI element for the general settings
         # Note that the class needs the parent object (to reference siblings)
         self.settings = general_settings(parent_tab, self)
         self.settings.frame.pack(padx=2, pady=2, fill='x')
         # Create the UI element for the "Also Switch" entry 
         # Note that the class needs the parent object (to reference siblings)
         self.alsoswitch = also_switch_selection(parent_tab, self)
@@ -335,14 +341,15 @@
 #------------------------------------------------------------------------------------
 # Top level Class for the Point Interlocking Tab
 #------------------------------------------------------------------------------------
 
 class point_interlocking_tab():
     def __init__(self, parent_tab):
         self.signals = common.signal_route_interlocking_frame(parent_tab)
+        self.signals.frame.pack(padx=2, pady=2, fill='x')
 
 #####################################################################################
 # Top level Class for the Edit Point window
 #####################################################################################
 
 class edit_point():
     def __init__(self, root, object_id):
@@ -362,14 +369,15 @@
         self.tab2 = Tk.Frame(self.tabs)
         self.tabs.add(self.tab2, text="Interlocking")
         self.tabs.pack()
         self.config = point_configuration_tab(self.tab1)
         self.locking = point_interlocking_tab(self.tab2)
         # Create the common Apply/OK/Reset/Cancel buttons for the window
         self.controls = common.window_controls(self.window, self, load_state, save_state)
+        self.controls.frame.pack(padx=2, pady=2)
         # Create the Validation error message (this gets packed/unpacked on apply/save)
         self.validation_error = Tk.Label(self.window, text="Errors on Form need correcting", fg="red")
         # load the initial UI state
         load_state(self)
 
     def tab_changed(self,event):
         # Focus on the top level window to remove focus from the first entry box
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/editor/configure_section.py` & `model-railway-signals-3.4.0/model_railway_signals/editor/configure_section.py`

 * *Files 2% similar despite different names*

```diff
@@ -335,44 +335,51 @@
 #------------------------------------------------------------------------------------
 # Class for the main Track Section configuration tab
 #------------------------------------------------------------------------------------
 
 class section_automation_tab():
     def __init__(self, parent_tab):
         self.behind = signal_route_frame (parent_tab, label="Signals behind section")
+        self.behind.frame.pack(padx=2, pady=2, fill='x')
         self.ahead = signal_route_frame (parent_tab, label="Signals ahead of section")
+        self.ahead.frame.pack(padx=2, pady=2, fill='x')
 
 #####################################################################################
 # Top level Class for the Edit Section window
 #####################################################################################
 
 class edit_section():
     def __init__(self, root, object_id):
         # This is the UUID for the object being edited
         self.object_id = object_id
         # Creatre the basic Top Level window
         self.window = Tk.Toplevel(root)
         self.window.attributes('-topmost',True)
+        # Create a frame to hold all UI elements (so they don't expand on window resize
+        # to provide consistent behavior with the other configure object popup windows)
+        self.main_frame = Tk.Frame(self.window)
+        self.main_frame.pack()
         # Create the Notebook (for the tabs) 
-        self.tabs = ttk.Notebook(self.window)
+        self.tabs = ttk.Notebook(self.main_frame)
         # When you change tabs tkinter focuses on the first entry box - we don't want this
         # So we bind the tab changed event to a function which will focus on something else 
         self.tabs.bind ('<<NotebookTabChanged>>', self.tab_changed)
         # Create the Window tabs
         self.tab1 = Tk.Frame(self.tabs)
         self.tabs.add(self.tab1, text="Configration")
         self.tab2 = Tk.Frame(self.tabs)
         self.tabs.add(self.tab2, text="Automation")
         self.tabs.pack(fill='x')
         self.config = section_configuration_tab(self.tab1)
         self.automation = section_automation_tab(self.tab2)        
         # Create the common Apply/OK/Reset/Cancel buttons for the window
-        self.controls = common.window_controls(self.window, self, load_state, save_state)
+        self.controls = common.window_controls(self.main_frame, self, load_state, save_state)
+        self.controls.frame.pack(padx=2, pady=2)
         # Create the Validation error message (this gets packed/unpacked on apply/save)
-        self.validation_error = Tk.Label(self.window, text="Errors on Form need correcting", fg="red")
+        self.validation_error = Tk.Label(self.main_frame, text="Errors on Form need correcting", fg="red")
         # load the initial UI state
         load_state(self)
 
     def tab_changed(self,event):
         # Focus on the top level window to remove focus from the first entry box
         # THIS IS STILL NOT WORKING AS IT LEAVES THE ENTRY BOX HIGHLIGHTED
         # self.window.focus()
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/editor/configure_signal.py` & `model-railway-signals-3.4.0/model_railway_signals/editor/configure_signal.py`

 * *Files 1% similar despite different names*

```diff
@@ -881,14 +881,15 @@
                 self.sub_routes_updated, self.dist_routes_updated)
         # The interlocking tab needs the parent object so the sig_id can be accessed for validation
         self.locking = configure_signal_tab2.signal_interlocking_tab(self.tab2, self)
         # The automation tab needs the parent object so the sig_id can be accessed for validation
         self.automation = configure_signal_tab3.signal_automation_tab(self.tab3, self)
         # Create the common Apply/OK/Reset/Cancel buttons for the window
         self.controls = common.window_controls(self.window, self, load_state, save_state)
+        self.controls.frame.pack(padx=2, pady=2)
         # Create the Validation error message (this gets packed/unpacked on apply/save)
         self.validation_error = Tk.Label(self.window, text="Errors on Form need correcting", fg="red")
         # load the initial UI state
         load_state(self)
         
     def tab_changed(self,event):
         # Focus on the top level window to remove focus from the first entry box
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/editor/configure_signal_tab1.py` & `model-railway-signals-3.4.0/model_railway_signals/editor/configure_signal_tab1.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.3.0/model_railway_signals/editor/configure_signal_tab2.py` & `model-railway-signals-3.4.0/model_railway_signals/editor/configure_signal_tab2.py`

 * *Files 4% similar despite different names*

```diff
@@ -274,29 +274,32 @@
         # These are the functions used to validate that the entered signal ID
         # exists on the schematic and is different to the current signal ID
         exists_function = objects.signal_exists
         current_id_function = parent_object.config.sigid.get_value
         # Create the Label Frame for the UI element (packed/unpacked on enable/disable) 
         self.frame = Tk.LabelFrame(parent_frame, text=label+" - interlocking with conflicting signals")
         self.frame.pack(padx=2, pady=2, fill='x')
-        self.frame.grid_columnconfigure(0, weight=1)
-        self.frame.grid_columnconfigure(1, weight=1)
+        # create two frames - each frame will hold two conflicting signals
+        self.subframe1 = Tk.Frame(self.frame)
+        self.subframe1.pack()
+        self.subframe2 = Tk.Frame(self.frame)
+        self.subframe2.pack()
         tool_tip = "Specify any signals/routes that would conflict with this signal route"
-        self.sig1 = common.signal_route_selections(self.frame, read_only=False, tool_tip = tool_tip,
+        self.sig1 = common.signal_route_selections(self.subframe1, read_only=False, tool_tip = tool_tip,
                     exists_function=exists_function, current_id_function=current_id_function)
-        self.sig1.frame.grid(row=0, column=0)
-        self.sig2 = common.signal_route_selections(self.frame, read_only=False, tool_tip = tool_tip,
+        self.sig1.frame.pack(side=Tk.LEFT, padx=5)
+        self.sig2 = common.signal_route_selections(self.subframe1, read_only=False, tool_tip = tool_tip,
                     exists_function=exists_function, current_id_function=current_id_function)
-        self.sig2.frame.grid(row=0, column=1)
-        self.sig3 = common.signal_route_selections(self.frame, read_only=False, tool_tip = tool_tip,
+        self.sig2.frame.pack(side=Tk.LEFT, padx=5)
+        self.sig3 = common.signal_route_selections(self.subframe2, read_only=False, tool_tip = tool_tip,
                     exists_function=exists_function, current_id_function=current_id_function)
-        self.sig3.frame.grid(row=1, column=0)
-        self.sig4 = common.signal_route_selections(self.frame, read_only=False, tool_tip = tool_tip,
+        self.sig3.frame.pack(side=Tk.LEFT, padx=5)
+        self.sig4 = common.signal_route_selections(self.subframe2, read_only=False, tool_tip = tool_tip,
                     exists_function=exists_function, current_id_function=current_id_function)
-        self.sig4.frame.grid(row=1, column=1)
+        self.sig4.frame.pack(side=Tk.LEFT, padx=5)
 
     def validate(self):
         # Validate all conflicting signal entries
         return ( self.sig1.validate and
                  self.sig2.validate and
                  self.sig3.validate and
                  self.sig4.validate )
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/editor/configure_signal_tab3.py` & `model-railway-signals-3.4.0/model_railway_signals/editor/configure_signal_tab3.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.3.0/model_railway_signals/editor/editor.py` & `model-railway-signals-3.4.0/model_railway_signals/editor/editor.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 #
 # Makes the following external API calls to other editor modules:
 #    objects.save_schematic_state() - Save the state following save or load
 #    objects.set_all(new_objects) - Set the dict of objects following a load
 #    objects.get_all() - Retrieve the dict of objects for saving to file
 #    objects.reset_objects() - Reset the schematic back to its default state
 #    schematic.initialise(root, callback, width, height, grid) - Create the canvas
-#    schematic.select_all_objects() - For selecting all objects prior to deletion
-#    schematic.delete_selected_objects() - For deleting all objects (on new/load)
+#    schematic.delete_all_objects() - For deleting all objects (on new/load)
 #    schematic.update_canvas() - For updating the canvas following reload/resizing
 #    schematic.enable_editing() - On mode toggle or load (if file is in edit mode)
 #    schematic.disable_editing() - On mode toggle or load (if file is in run mode)
 #    settings.get_all() - Get all settings (for save)
 #    settings.set_all() - Set all settings (following load)
 #    settings.get_canvas() - Get default/loaded canvas settings (for resizing)
 #    settings.get_version() - Get the Application version (for the Arg Parser)
 #    settings.get_general() - Get the current filename and editor mode
 #    settings.set_general() - Set the filename and editor mode
 #    settings.get_logging() - Set the default log level
 #    settings.get_sprog() - to get the initial SPROG settings
 #    settings.restore_defaults() - Following user selection of "new"
+#    common.scrollable_text_box - to display a list of warnings on file load
 #
 # Makes the following external API calls to library modules:
 #    library_common.find_root_window (widget) - To set the root window
 #    library_common.on_closing (ask_to_save_state) - To shutdown gracefully
 #    file_interface.load_schematic - To load all settings and objects
 #    file_interface.save_schematic - To save all settings and objects
 #    file_interface.purge_loaded_state_information - Called following a re-load
@@ -41,14 +41,15 @@
 #------------------------------------------------------------------------------------
 
 import os
 import tkinter as Tk
 import logging
 from argparse import ArgumentParser
 
+from . import common
 from . import objects
 from . import settings
 from . import schematic
 from . import menubar_windows
 from ..library import file_interface
 from ..library import pi_sprog_interface
 from ..library import common as library_common
@@ -98,25 +99,27 @@
         self.settings_menu.add_command(label =" SPROG...", command=lambda:menubar_windows.edit_sprog_settings(self.root, self))
         self.settings_menu.add_command(label =" Logging...", command=lambda:menubar_windows.edit_logging_settings(self.root))
         self.mainmenubar.add_cascade(label = "Settings  ", menu=self.settings_menu)
         # Create the various menubar items for the Help Dropdown
         self.help_menu = Tk.Menu(self.mainmenubar,tearoff=False)
         self.help_menu.add_command(label =" Help...", command=lambda:menubar_windows.display_help(self.root))
         self.help_menu.add_command(label =" About...", command=lambda:menubar_windows.display_about(self.root))
+        self.help_menu.add_command(label =" Info...", command=lambda:menubar_windows.edit_layout_info(self.root))
         self.mainmenubar.add_cascade(label = "Help  ", menu=self.help_menu)
         # Flag to track whether the new configuration has been saved or not
         # Used to enforce a "save as" dialog on the initial save of a new layout
         self.file_has_been_saved = False
         # initialise the schematic editor
         width, height, grid = settings.get_canvas()
         schematic.initialise(self.root, self.handle_canvas_event, width, height, grid)
         # Initialise the editor configuration at startup
         self.initialise_editor()
         # Parse the command line arguments to get the filename (and load it)
-        parser = ArgumentParser(description =  "Model railway signalling "+settings.get_version())
+        # The version is the third parameter provided by 'get_general'
+        parser = ArgumentParser(description =  "Model railway signalling "+settings.get_general()[2])
         parser.add_argument("-f","--file",dest="filename",help="schematic file to load on startup",metavar="FILE")
         args = parser.parse_args()
         if args.filename is not None: self.load_schematic(args.filename)
         
     # Common initialisation function (called on editor start or layout load or new layout)
     def initialise_editor(self):
         # Set the root window label to the name of the current file (split from the dir path)
@@ -221,21 +224,16 @@
         return()
                 
     def new_schematic(self, ask_for_confirm:bool=True):
         # Note that 'confirmation' is defaulted to 'True' for normal use (i.e. when this function
         # is called as a result of a menubar selection) to enforce the confirmation dialog. If
         if not ask_for_confirm or Tk.messagebox.askokcancel(parent=self.root, title="New Schematic",
                 message="Are you sure you want to discard all changes and create a new blank schematic"):
-            # We use the schematic functions to delete all existing objects to
-            # ensure they are also deselected and removed from the clibboard 
-            schematic.select_all_objects()
-            schematic.delete_selected_objects()
-            # Belt and braces delete of all canvas objects as I've seen issues when
-            # running the system tests (probably because I'm not using the mainloop)
-            schematic.canvas.delete("all")
+            # Delete all existing objects
+            schematic.delete_all_objects()
             # Restore the default settings and update the editor config
             settings.restore_defaults()
             # Re-initialise the editor for the new settings to take effect
             self.initialise_editor()
             # Re-size the canvas to reflect the new schematic size
             width, height, grid = settings.get_canvas()
             schematic.update_canvas(width, height, grid)
@@ -262,56 +260,93 @@
             self.file_has_been_saved = True
         return()
 
     def load_schematic(self, filename=None):
         # Note that 'filename' is defaulted to 'None' for normal use (i.e. when this function
         # is called as a result of a menubar selection) to enforce the file selection dialog. If
         # a filename is specified (system_test_harness use case) then the dialogue is surpressed
-        global logging
+
         # Call the library function to load the base configuration file
         # the 'file_loaded' will be the name of the file loaded or None (if not loaded)
         file_loaded, layout_state = file_interface.load_schematic(filename)
         if file_loaded is not None:
             # Do some basic validation that the file has the elements we need
             if "settings" in layout_state.keys() and "objects" in layout_state.keys():
-                # We use the schematic functions to delete all existing objects to
-                # ensure they are also deselected and removed from the clibboard 
-                schematic.select_all_objects()
-                schematic.delete_selected_objects()
-                # Belt and braces delete of all canvas objects as I've seen issues when
-                # running the system tests (probably because I'm not using the mainloop)
-                schematic.canvas.delete("all")
-                # Store the newly loaded settings
-                settings.set_all(layout_state["settings"])
+                # Delete all existing objects
+                schematic.delete_all_objects()
+                # Create an empty list for any warning messages generated by the load
+                # Messages could be generated by settings.set_all or objects.set_all
+                warning_messages = []
+                # Store the newly loaded settings (getting any warnings)
+                warning_messages = settings.set_all(layout_state["settings"])
                 # Set the filename to reflect that actual name of the loaded file
                 settings.set_general(filename=file_loaded)
                 # Re-size the canvas to reflect the new schematic size
                 width, height, grid = settings.get_canvas()
                 schematic.update_canvas(width, height, grid)
                 # Re-initailise the editor with the new configuration
                 self.initialise_editor()
                 # Create the loaded layout objects then purge the loaded state information
-                objects.set_all(layout_state["objects"])
+                warning_messages.extend(objects.set_all(layout_state["objects"]))
                 # Purge the loaded state (to stope it being erroneously inherited
                 # when items are deleted and then new items created with the same IDs)
                 file_interface.purge_loaded_state_information()
                 # Set the flag so we don't enforce a "save as" on next save
                 self.file_has_been_saved = True
+                # Generate a popup window to display any warning messages:
+                if warning_messages != []:
+                    warning_text=""
+                    for warning_message in warning_messages:
+                        warning_text = warning_text + warning_message + "\n"
+                    self.load_warnings_window(self.root,warning_text)
             else:
                 logging.error("LOAD LAYOUT - Selected file does not contain all required elements")
                 Tk.messagebox.showerror(parent=self.root, title="Load Error", 
                     message="File does not contain\nall required elements")
         return()
+    
+#------------------------------------------------------------------------------------
+# Class for the window to display any file load warning messages  
+#------------------------------------------------------------------------------------
 
+    class load_warnings_window():
+        def __init__(self, root_window, warning_text):
+            self.root_window = root_window
+            # Create the top level window for the file load warnings
+            winx = self.root_window.winfo_rootx() + 250
+            winy = self.root_window.winfo_rooty() + 20
+            self.window = Tk.Toplevel(self.root_window)
+            self.window.geometry(f'+{winx}+{winy}')
+            self.window.title("Load Layout File")
+            self.window.attributes('-topmost',True)
+            # Create an overall warning label
+            label_text = ("Layout file generated by a different version of the application\n"+
+                            "Check reported warnings and re-save as a new layout file")
+            self.label = Tk.Label(self.window, font="Helvetica 12 bold", text=label_text)
+            # Create the srollable textbox to display the warnings. We only specify
+            # the max height (in case the list of warnings is extremely long) leaving
+            # the width to auto-scale to the maximum width of the warnings
+            self.text = common.scrollable_text_frame(self.window, max_height=25)
+            self.text.set_value(warning_text)
+            # Create the ok/close button and tooltip
+            self.B1 = Tk.Button (self.window, text = "Ok / Close", command=self.ok)
+            self.TT1 = common.CreateToolTip(self.B1, "Close window")
+            # Pack the OK button and labels First - so they remain visible on re-sizing
+            self.B1.pack(padx=5, pady=5, side=Tk.BOTTOM)
+            self.label.pack(padx=2, pady=2, side=Tk.TOP)
+            self.text.pack(padx=2, pady=2, fill=Tk.BOTH, expand=True)
+            
+        def ok(self):
+            self.window.destroy()
+        
 #------------------------------------------------------------------------------------
 # This is where the code begins  
 #------------------------------------------------------------------------------------
 
 def run_editor():
-    global logging
     # Create the Main Root Window
     root = Tk.Tk()
     # Create the menubar and editor canvas (canvas size will be set on creation)
     main_window_menubar = main_menubar(root)
     # Use the signals Lib function to find/store the root window reference
     # And then re-bind the close window event to the editor quit function
     library_common.find_root_window(main_window_menubar.mainmenubar)
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/editor/menubar_windows.py` & `model-railway-signals-3.4.0/model_railway_signals/editor/menubar_windows.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 #------------------------------------------------------------------------------------
 # This module contains all the functions for the menubar selection windows
 # 
 # Classes (pop up windows) called from the main editor module menubar selections
 #    display_help(root)
 #    display_about(root)
+#    edit_layout_info()
 #    edit_mqtt_settings(root)
 #    edit_sprog_settings(root)
 #    edit_logging_settings(root)
 #    edit_canvas_settings(root)
 #    ######### MORE COMING #####################
 #
 # Makes the following external API calls to other editor modules:
 #    schematic.update_canvas() - For updating the canvas following reload/resizing
 #    settings.get_canvas() - Get the current settings (for editing)
 #    settings.set_canvas(width,height,grid) - Save the new settings
 #    settings.get_logging() - Get the current settings (for editing)
 #    settings.set_logging(level) - Save the new settings
+#    settings.get_general() - Get the current settings (for info/editing)
+#    settings.set_general() - Save the new settings (layout info)
 #    settings.get_sprog() - Get the current settings (for editing)
 #    settings.set_sprog(params) - Save the new settings
-#    settings_get_version() - For the 'About' Window
 #
 # Uses the following common editor UI elements:
 #    common.selection_buttons
 #    common.check_box
 #    common.entry_box
 #    common.integer_entry_box
 #    common.window_controls
 #    common.CreateToolTip
-#
+#    common.scrollable_text_box
 #------------------------------------------------------------------------------------
 
 import tkinter as Tk
 import logging
 import webbrowser
 
 from . import common
 from . import settings
 from . import schematic
 
 #------------------------------------------------------------------------------------
-# Class for the "Help" window
+# Class for the "Help" window - Uses the common.scrollable_text_box
+# Note the packing order to keep the button visible during window re-sizing
 #------------------------------------------------------------------------------------
 
 help_text = """
 Application documentation is still on the 'ToDo' list, but in the meantime here is some
 basic guidance and top tips for creating your layout signalling system:
 
 1) Save your progress - The editor is still in active development so may still contain
@@ -77,124 +80,171 @@
 1) File - All the functions you would expect
 2) Mode - Selects the schematic editor mode (Edit Mode or Run Mode)
 3) SPROG - Opens the serial port and connects to the SPROG
 4) DCC Power - Toggle the DCC bus supply (SPROG must be initialised)
 5) Settings-Canvas - Change the display size of the schematic
 6) Settings-Logging - Set the log level for running the layout
 7) Settings-SPROG - Configure the serial port and SPROG behavior
+8) Help-Info - Add notes to document your layout configuration
 
 Schematic object configuration
 
 1) Double click on the object to open the object's configuration window
 2) Use the hover-over Tooltips to get more information on the selections 
 """
 
 class display_help():
     def __init__(self, root_window):
         self.root_window = root_window
-        # Create the top level window for the canvas settings
+        # Create the top level window for application help
         winx = self.root_window.winfo_rootx() + 250
-        winy = self.root_window.winfo_rooty() + 50
+        winy = self.root_window.winfo_rooty() + 20
         self.window = Tk.Toplevel(self.root_window)
         self.window.geometry(f'+{winx}+{winy}')
         self.window.title("Application Help")
         self.window.attributes('-topmost',True)
-        self.label1 = Tk.Label(self.window, text=help_text, justify=Tk.LEFT)
-        self.label1.pack(padx=5, pady=5)
-        # Create the close button and tooltip
-        self.B1 = Tk.Button (self.window, text = "Ok / Close",command=self.ok)
-        self.B1.pack(padx=2, pady=2)
+        # Create the srollable textbox to display the help text. We only specify
+        # the max height (in case the help text grows in the future) leaving
+        # the width to auto-scale to the maximum width of the help text
+        self.text = common.scrollable_text_frame(self.window, max_height=25)
+        self.text.set_value(help_text)
+        # Create the ok/close button and tooltip
+        self.B1 = Tk.Button (self.window, text = "Ok / Close", command=self.ok)
         self.TT1 = common.CreateToolTip(self.B1, "Close window")
+        # Pack the OK button First - so it remains visible on re-sizing
+        self.B1.pack(padx=5, pady=5, side=Tk.BOTTOM)
+        self.text.pack(padx=2, pady=2, fill=Tk.BOTH, expand=True)
         
     def ok(self):
         self.window.destroy()
-        
+
 #------------------------------------------------------------------------------------
-# Class for the "About" window
+# Class for the "About" window- uses a hyperlink to go to the github repo
 #------------------------------------------------------------------------------------
 
+# The version is the third parameter provided by 'get_general'
 about_text = """
-Model Railway Signals ("""+settings.get_version()+""")
+Model Railway Signals ("""+settings.get_general()[2]+""")
 
 An application for designing and developing fully interlocked and automated model railway
 signalling systems with DCC control of signals and points via the SPROG Command Station.
 
-From release 3.0.0 this software is released under the GNU General Public License
-Version 2, June 1991 meaning you are free to use, share or adapt the software as you like
+This software is released under the GNU General Public License Version 2, June 1991 
+meaning you are free to use, share or adapt the software as you like
 but must ensure those same rights are passed on to all recipients.
 
 For more information visit: """
 
 class display_about():
     def __init__(self, root_window):
-        text2 = "https://github.com/johnrm174/model-railway-signalling"
         self.root_window = root_window
-        # Create the top level window for the canvas settings
+        # Create the top level window for application about
         winx = self.root_window.winfo_rootx() + 250
-        winy = self.root_window.winfo_rooty() + 50
+        winy = self.root_window.winfo_rooty() + 20
         self.window = Tk.Toplevel(self.root_window)
         self.window.geometry(f'+{winx}+{winy}')
         self.window.title("Application Info")
         self.window.attributes('-topmost',True)
         self.label1 = Tk.Label(self.window, text=about_text)
         self.label1.pack(padx=5, pady=5)
-        self.label2 = Tk.Label(self.window, text=text2, fg="blue", cursor="hand2")
+        hyperlink = "https://github.com/johnrm174/model-railway-signalling"
+        self.label2 = Tk.Label(self.window, text=hyperlink, fg="blue", cursor="hand2")
         self.label2.pack(padx=5, pady=5)
-        self.label2.bind("<Button-1>", lambda e:self.callback())
+        self.label2.bind("<Button-1>", self.callback)
         # Create the close button and tooltip
         self.B1 = Tk.Button (self.window, text = "Ok / Close",command=self.ok)
         self.B1.pack(padx=2, pady=2)
         self.TT1 = common.CreateToolTip(self.B1, "Close window")
         
     def ok(self):
         self.window.destroy()
 
-    def callback(self):
+    def callback(self,event):
         webbrowser.open_new_tab("https://github.com/johnrm174/model-railway-signalling")
 
 #------------------------------------------------------------------------------------
-# Class for the "About" window
+# Class for the Edit Layout Information window
+#------------------------------------------------------------------------------------
+
+class edit_layout_info():
+    def __init__(self, root_window):
+        self.root_window = root_window
+        # Create the top level window for application help
+        winx = self.root_window.winfo_rootx() + 250
+        winy = self.root_window.winfo_rooty() + 20
+        self.window = Tk.Toplevel(self.root_window)
+        self.window.geometry(f'+{winx}+{winy}')
+        self.window.title("Layout Information")
+        self.window.attributes('-topmost',True)
+        # Create the srollable textbox to display the text. We specify
+        # the max height/width (in case the text grows in the future) and also
+        # the min height/width (to give the user something to start with)
+        self.text = common.scrollable_text_frame(self.window, max_height=30,max_width=100,
+                min_height=10, min_width=40, editable=True, auto_resize=True)
+        # Create the common Apply/OK/Reset/Cancel buttons for the window
+        self.controls = common.window_controls(self.window, self,
+                                self.load_state, self.save_state)
+        # We need to pack the window buttons at the bottom and then pack the text
+        # frame - so the buttons remain visible if the user re-sizes the window
+        self.controls.frame.pack(side=Tk.BOTTOM, padx=2, pady=2)
+        self.text.pack(padx=2, pady=2, fill=Tk.BOTH, expand=True)
+        # Load the initial UI state
+        self.load_state()
+        
+    def load_state(self, parent_object=None):
+        # Parent object is passed by the callback - not used here
+        # The version is the forth parameter provided by 'get_general'
+        self.text.set_value(settings.get_general()[3])
+        
+    def save_state(self, parent_object, close_window:bool):
+        # Parent object is passed by the callback - not used here
+        settings.set_general(info=self.text.get_value())
+        if close_window: self.window.destroy()
+
+#------------------------------------------------------------------------------------
+# Class for the MQTT configuration window
 #------------------------------------------------------------------------------------
 
 class edit_mqtt_settings():
     def __init__(self, root_window):
         text1 = ("Coming Soon")
         self.root_window = root_window
-        # Create the top level window for the canvas settings
-        winx = self.root_window.winfo_rootx() + 250
-        winy = self.root_window.winfo_rooty() + 50
+        # Create the top level window for the MQTT Settings
+        winx = self.root_window.winfo_rootx() + 200
+        winy = self.root_window.winfo_rooty() + 20
         self.window = Tk.Toplevel(self.root_window)
         self.window.geometry(f'+{winx}+{winy}')
         self.window.title("MQTT")
         self.window.attributes('-topmost',True)
         self.label1 = Tk.Label(self.window, text=text1, wraplength=400)
         self.label1.pack(padx=2, pady=2)
         # Create the common Apply/OK/Reset/Cancel buttons for the window
-        common.window_controls(self.window, self, self.load_state, self.save_state)
+        self.controls = common.window_controls(self.window, self, self.load_state, self.save_state)
+        self.controls.frame.pack(padx=2, pady=2)
 
     def load_state(self, parent_object=None):
         # Parent object is passed by the callback - not used here
         pass
         
     def save_state(self, parent_object, close_window:bool):
         # Parent object is passed by the callback - not used here
         if close_window: self.window.destroy()
 
 #------------------------------------------------------------------------------------
-# Class for the SPROG settings selection toolbar window. Note the function also takee
-# in the menubar object so it can call the function to update the menubar sprog status
+# Class for the SPROG settings selection toolbar window. Note the function also takes
+# in a callback object so it can call the function to update the menubar sprog status
 #------------------------------------------------------------------------------------
 
 class edit_sprog_settings():
     def __init__(self, root_window, mb_object):
         self.root_window = root_window
         self.mb_object = mb_object
-        # Create the top level window for the canvas settings
+        # Create the top level window for the SPROG configuration
         winx = self.root_window.winfo_rootx() + 200
-        winy = self.root_window.winfo_rooty() + 50
+        winy = self.root_window.winfo_rooty() + 20
         self.window = Tk.Toplevel(self.root_window)
         self.window.geometry(f'+{winx}+{winy}')
         self.window.title("SPROG DCC")
         self.window.attributes('-topmost',True)
         # Create the Serial Port and baud rate UI elements 
         self.frame1 = Tk.Frame(self.window)
         self.frame1.pack()
@@ -204,14 +254,16 @@
                         "the serial port to use for communicating with the SPROG")
         self.port.pack(side=Tk.LEFT, padx=2, pady=2)
         self.label2 = Tk.Label(self.frame1, text="Baud:")
         self.label2.pack(side=Tk.LEFT, padx=2, pady=2)
         self.options = ['300','600','1200','1800','2400','4800','9600','19200','38400','57600','115200']
         self.baud_selection = Tk.StringVar(self.window, "")
         self.baud = Tk.OptionMenu(self.frame1, self.baud_selection, *self.options)
+        menu_width = len(max(self.options, key=len))
+        self.baud.config(width=menu_width)
         common.CreateToolTip(self.baud, "Select the baud rate to use for the serial port")
         self.baud.pack(side=Tk.LEFT, padx=2, pady=2)
         # Create the remaining UI elements
         self.debug = common.check_box(self.window, label="Enhanced SPROG debug logging", width=28, 
             tool_tip="Select to enable enhanced debug logging (Layout log level must also be set to 'debug')")
         self.debug.pack(padx=2, pady=2)
         self.startup = common.check_box(self.window, label="Initialise SPROG on layout load", width=28, 
@@ -226,19 +278,21 @@
         self.B1.pack(padx=2, pady=2)
         self.TT1 = common.CreateToolTip(self.B1, "Will configure/open the specified serial port and request "+
                         "the command station status to confirm a connection to the SPROG has been established")
         # Create the Status Label
         self.status = Tk.Label(self.window, text="")
         self.status.pack(padx=2, pady=2)
         # Create the common Apply/OK/Reset/Cancel buttons for the window
-        common.window_controls(self.window, self, self.load_state, self.save_state)
+        self.controls = common.window_controls(self.window, self, self.load_state, self.save_state)
+        self.controls.frame.pack(padx=2, pady=2)
         # Load the initial UI state
         self.load_state()
 
     def selection_changed(self):
+        # If connect on startup is selected then enable the DCC power on startup selection
         if self.startup.get_value(): self.power.enable()
         else: self.power.disable()
 
     def test_connectivity(self):
         # Validate the port to "accept" the current value (by focusing out)
         self.port.validate()
         self.B1.focus()
@@ -263,14 +317,15 @@
         # Parent object is passed by the callback - not used here
         port, baud, debug, startup, power = settings.get_sprog()
         self.port.set_value(port)
         self.baud_selection.set(str(baud))
         self.debug.set_value(debug)
         self.startup.set_value(startup)
         self.power.set_value(power)
+        self.selection_changed()
         
     def save_state(self, parent_object, close_window:bool):
         # Parent object is passed by the callback - not used here
         baud = int(self.baud_selection.get())
         port = self.port.get_value()
         debug = self.debug.get_value()
         startup = self.startup.get_value()
@@ -282,28 +337,29 @@
 #------------------------------------------------------------------------------------
 # Class for the Logging Level selection toolbar window
 #------------------------------------------------------------------------------------
 
 class edit_logging_settings():
     def __init__(self, root_window):
         self.root_window = root_window
-        # Create the top level window for the canvas settings
+        # Create the top level window for the Logging Configuration
         winx = self.root_window.winfo_rootx() + 200
-        winy = self.root_window.winfo_rooty() + 50
+        winy = self.root_window.winfo_rooty() + 20
         self.window = Tk.Toplevel(self.root_window)
         self.window.geometry(f'+{winx}+{winy}')
         self.window.title("Logging")
         self.window.attributes('-topmost',True)
         # Create the logging Level selections element
         self.log_level = common.selection_buttons (self.window, label="Layout Log Level",
                                             b1="Error", b2="Warning", b3="Info", b4="Debug",
                                             tool_tip="Set the logging level for running the layout")
         self.log_level.frame.pack()
         # Create the common Apply/OK/Reset/Cancel buttons for the window
-        common.window_controls(self.window, self, self.load_state, self.save_state)
+        self.controls = common.window_controls(self.window, self, self.load_state, self.save_state)
+        self.controls.frame.pack(padx=2, pady=2)
         # Load the initial UI state
         self.load_state()
 
     def load_state(self, parent_object=None):
         # Parent object is passed by the callback - not used here
         self.log_level.set_value(settings.get_logging())
         
@@ -322,16 +378,16 @@
 # Class for the Canvas configuration toolbar window
 #------------------------------------------------------------------------------------
 
 class edit_canvas_settings():
     def __init__(self, root_window):
         self.root_window = root_window
         # Create the top level window for the canvas settings
-        winx = self.root_window.winfo_rootx() + 150
-        winy = self.root_window.winfo_rooty() + 50
+        winx = self.root_window.winfo_rootx() + 200
+        winy = self.root_window.winfo_rooty() + 20
         self.window = Tk.Toplevel(self.root_window)
         self.window.geometry(f'+{winx}+{winy}')
         self.window.title("Canvas")
         self.window.attributes('-topmost',True)
         # Create the entry box elements for the width and height
         # Pack the elements as a grid to get an aligned layout
         self.frame = Tk.Frame(self.window)
@@ -345,15 +401,16 @@
         self.width.grid(row=0, column=1)
         self.label2 = Tk.Label(self.frame, text="Canvas height:")
         self.label2.grid(row=1, column=0)
         self.height = common.integer_entry_box(self.frame, width=5, min_value=200, max_value=2000,
                         allow_empty=False, tool_tip="Enter height in pixels (200-2000)")
         self.height.grid(row=1, column=1)
         # Create the common Apply/OK/Reset/Cancel buttons for the window
-        common.window_controls(self.window, self, self.load_state, self.save_state)
+        self.controls = common.window_controls(self.window, self, self.load_state, self.save_state)
+        self.controls.frame.pack(padx=2, pady=2)
         # Load the initial UI state
         self.load_state()
 
     def load_state(self, parent_object=None):
         # Parent object is passed by the callback - not used here
         width, height, grid = settings.get_canvas()
         self.width.set_value(width)
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/editor/objects/__init__.py` & `model-railway-signals-3.4.0/model_railway_signals/editor/objects/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 #------------------------------------------------------------------------------------
 # These are the Public API functions for the Objects sub-package
 #------------------------------------------------------------------------------------
 #
-#    Externalised API functions intended for use by other editor modules:
+# Externalised API functions intended for use by other editor modules:
 #    initialise (canvas,x,y,grid) - Initialise the objects package and set defaults
 #    update_canvas(x,y,grid) - update the attributes (on load and re-size)
 #    signal(item_id:int) - helper function to find the object Id by Item ID
 #    point(item_id:int) - helper function to find the object Id by Item ID
 #    section(item_id:int) - helper function to find the object Id by Item ID
 #    instrument(item_id:int) - helper function to find the object Id by Item ID
+#    line(item_id:int) - helper function to find the object Id by Item ID
 #    signal_exists(item_id:int) - Common function to see if a given item exists
 #    point_exists(item_id:int) - Common function to see if a given item exists
 #    section_exists(item_id:int) - Common function to see if a given item exists
 #    instrument_exists(item_id:int) - Common function to see if a given item exists
+#    line_exists (item_id:int) - Common function to see if a given item exists
 #    save_schematic_state(reset_pointer:bool) - save a snapshot of the schematic objects
 #         (reset_pointer=True will clear the undo buffer (deleting the undo history)
 #    set_all(new_objects) - Creates a new dictionary of objects (following a load)
 #    get_all() - returns the current dictionary of objects (for saving to file)
 #    undo() / redo() - Undo and re-do functions as you would expect
 #    create_object(obj_type, item_type, item_subtype) - create a new object on the canvas
 #    delete_objects([object_IDs]) - Delete the selected objects from the canvas
@@ -24,14 +26,16 @@
 #    move_objects([object_IDs]) - Finalises the move of selected objects
 #    copy_objects([object_IDs]) - Copy the selected objects to the clipboard
 #    paste_objects() - Paste Clipboard objects onto the canvas (returns list of new IDs)
 #    update_object(object_ID, new_object) - update the config of an existing object
 #    enable_editing() - Call when 'Edit' Mode is selected (from Schematic Module)
 #    disable_editing() - Call when 'Run' Mode is selected (from Schematic Module)
 #    reset_objects() - resets all points, signals, instruments and sections to default state
+#    get_endstop_offsets(x1,y1,x2,y2)- used by the schematics module to get the offsets
+#        for line 'end stops' so they can be moved with the line ends during editing
 #
 # Objects intended to be accessed directly by other editor modules:
 #    object_type - Enumeration type for the supported objects
 #    schematic_objects - For accessing/editing the configuration of an object
 #    signal_index - for iterating through all the signal objects
 #    point_index - for iterating through all the point objects
 #    instrument_index - for iterating through all the instrument objects
@@ -63,25 +67,30 @@
 from .objects import reset_objects
 from .objects_common import initialise
 from .objects_common import update_canvas
 from .objects_common import signal 
 from .objects_common import point 
 from .objects_common import section
 from .objects_common import instrument
+from .objects_common import line
 from .objects_common import signal_exists
 from .objects_common import point_exists
 from .objects_common import section_exists
 from .objects_common import instrument_exists
+from .objects_common import line_exists
 
 from .objects_common import object_type
 from .objects_common import schematic_objects 
 from .objects_common import signal_index 
 from .objects_common import point_index 
 from .objects_common import section_index 
 from .objects_common import instrument_index
+from .objects_common import line_index
+
+from .objects_lines import get_endstop_offsets
 
 # The following code does nothing apart from suppressing
 # the spurious pyflakes warnings for unused imports
 
 assert set_all
 assert get_all
 assert undo
@@ -99,19 +108,23 @@
 assert reset_objects
 assert initialise
 assert update_canvas
 assert signal 
 assert point 
 assert section
 assert instrument
+assert line
 assert signal_exists
 assert point_exists
 assert section_exists
 assert instrument_exists
+assert line_exists
 assert object_type
+assert get_endstop_offsets
 assert type(schematic_objects) 
 assert type(signal_index)
 assert type(point_index)
 assert type(section_index)
 assert type(instrument_index)
+assert type(line_index)
 
-##########################################################################################################################
+##########################################################################################################################
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/editor/objects/objects.py` & `model-railway-signals-3.4.0/model_railway_signals/editor/objects/objects.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 #    objects_instruments.update_instrument(obj_id,new_obj) - Update the configuration of an existing instrument object
 #    objects_instruments.paste_instrument(object) - Paste a copy of an object to create a new one (returns new object_id)
 #    objects_instruments.delete_instrument_object(object_id) - Soft delete the drawing object (prior to recreating))
 #    objects_instruments.redraw_instrument_object(object_id) - Redraw the object on the canvas following an update
 #    objects_instruments.default_instrument_object - The dictionary of default values for the object
 #    objects_lines.create_line() - Create a default object on the schematic
 #    objects_lines.delete_line(object_id) - Hard Delete an object when deleted from the schematic
+#    objects_lines.update_line(obj_id,new_obj) - Update the configuration of an existing line object
 #    objects_lines.paste_line(object) - Paste a copy of an object to create a new one (returns new object_id)
 #    objects_lines.delete_line_object(object_id) - Soft delete the drawing object (prior to recreating))
 #    objects_lines.redraw_line_object(object_id) - Redraw the object on the canvas following an update
 #    objects_lines.default_line_object - The dictionary of default values for the object
 #    objects_points.create_point(type) - Create a default object on the schematic
 #    objects_points.delete_point(obj_id) - Hard Delete an object when deleted from the schematic
 #    objects_points.update_point(obj_id,new_obj) - Update the configuration of an existing point object
@@ -60,16 +61,14 @@
 #    objects_signals.default_signal_object - The dictionary of default values for the object
 #
 #------------------------------------------------------------------------------------
 
 import copy 
 import logging
 
-import tkinter as Tk
-
 from . import objects_common
 from . import objects_signals
 from . import objects_points
 from . import objects_lines
 from . import objects_sections
 from . import objects_instruments
 
@@ -102,35 +101,39 @@
             objects_signals.redraw_signal_object(object_id)
         elif this_object_type == objects_common.object_type.point:
             objects_points.redraw_point_object(object_id)
         elif this_object_type == objects_common.object_type.section:
             objects_sections.redraw_section_object(object_id)
         elif this_object_type == objects_common.object_type.instrument:
             objects_instruments.redraw_instrument_object(object_id)
+    # Ensure all track sections are brought forward on the schematic (in front of any lines)
+    bring_track_sections_to_the_front()
     return()
 
 #------------------------------------------------------------------------------------
 # Internal function to reset all item-specific indexes from the main schematic_objects
 # dictionary - called following item load and as part of undo/redo. Note that for
 # both of these cases, all existing entries will have been deleted when all schematic
 # objects were selected then deleted as part of the undo/redo or load layout
 #------------------------------------------------------------------------------------
 
 def reset_all_schematic_indexes():
     for object_id in objects_common.schematic_objects:
         this_object_type = objects_common.schematic_objects[object_id]["item"]
-        this_object_id = objects_common.schematic_objects[object_id]["itemid"]
+        this_object_item_id = objects_common.schematic_objects[object_id]["itemid"]
         if this_object_type == objects_common.object_type.signal:                
-            objects_common.signal_index[str(this_object_id)] = object_id
+            objects_common.signal_index[str(this_object_item_id)] = object_id
         elif this_object_type == objects_common.object_type.point:
-            objects_common.point_index[str(this_object_id)] = object_id
+            objects_common.point_index[str(this_object_item_id)] = object_id
         elif this_object_type == objects_common.object_type.section:
-            objects_common.section_index[str(this_object_id)] = object_id
+            objects_common.section_index[str(this_object_item_id)] = object_id
         elif this_object_type == objects_common.object_type.instrument:
-            objects_common.instrument_index[str(this_object_id)] = object_id
+            objects_common.instrument_index[str(this_object_item_id)] = object_id
+        elif this_object_type == objects_common.object_type.line:
+            objects_common.line_index[str(this_object_item_id)] = object_id
     return()
 
 #------------------------------------------------------------------------------------
 # Undo and redo functions - the 'save_schematic_state' function should be called after
 # every change the schematic or a change to any object on the schematic to take a snapshot
 # and add this to the undo buffer. 'undo' and 'redo' then work as you'd expect
 # 'restore_schematic_state' is the internal function used by 'undo' and 'redo'
@@ -185,16 +188,14 @@
     snapshot_objects = undo_buffer[undo_pointer]
     for object_id in snapshot_objects:
         objects_common.schematic_objects[object_id] = copy.deepcopy(snapshot_objects[object_id])
     # Set the seperate schematic dictionary indexes from the restored schematic objects dict
     reset_all_schematic_indexes()
     # Re-draw all objects, ensuring a new bbox is created for each object
     redraw_all_objects(create_new_bbox=True)
-    # Ensure all track sections are brought forward on the schematic (in front of any lines)
-    bring_track_sections_to_the_front()
     # Recalculate instrument interlocking tables as a 'belt and braces' measure (on the 
     # basis they would have successfully been restored with the rest of the snapshot)
     objects_points.reset_point_interlocking_tables()
     return()
 
 #------------------------------------------------------------------------------------
 # Functions to Enable and disable editing 
@@ -263,23 +264,25 @@
 # Function to update the configuration of an existing schematic object and re-draw it
 # in its new configuration (delete the drawing objects then re-draw in the new configuration)
 #------------------------------------------------------------------------------------
 
 def update_object(object_id, new_object):
     type_of_object = objects_common.schematic_objects[object_id]["item"]
     if type_of_object == objects_common.object_type.line:
-        pass
+        objects_lines.update_line(object_id, new_object)
     elif type_of_object == objects_common.object_type.signal:
         objects_signals.update_signal(object_id, new_object)
     elif type_of_object == objects_common.object_type.point:
         objects_points.update_point(object_id, new_object)
     elif type_of_object == objects_common.object_type.section:
         objects_sections.update_section(object_id, new_object)
     elif type_of_object == objects_common.object_type.instrument:
         objects_instruments.update_instrument(object_id, new_object)
+    # Ensure all track sections are brought forward on the schematic (in front of any lines)
+    bring_track_sections_to_the_front()
     # save the current state (for undo/redo)
     save_schematic_state()
     # Process any layout changes (interlocking, signal ahead etc)
     # that might be dependent on the object configuration change
     run_layout.initialise_layout()
     return()
 
@@ -433,17 +436,21 @@
 #------------------------------------------------------------------------------------
 # Function to set (re-create) all schematic objects (following a file load)
 # Note that there is a dependancy that the main schematic objects dict is empty
 # i.e. any legacy objects existing prior to the load will have been deleted first
 #------------------------------------------------------------------------------------
 
 def set_all(new_objects):
-    global logging
-    # List of error messages to report
-    warning_messages = ""
+    ##################################################################################
+    ### Handle breaking change of lines having Item IDs from Release 3.4.0 onwards ###
+    one_up_line_id = 1
+    ### Handle breaking change of lines having Item IDs from Release 3.4.0 onwards ###
+    ##################################################################################
+    # List of warning messages to report
+    warning_messages = []
     # For each loaded object, create a new default object of the same type
     # and then copy across each element in turn. This is defensive programming
     # to populate the objects gracefully whilst handling changes to an object
     # structre (e.g. new element introduced since the file was last saved)
     for object_id in new_objects:
         # Get the item id of the new object - for error reporting
         # The 'item' and 'itemid' elements are MANDATORY for all objects 
@@ -458,81 +465,68 @@
             default_object = objects_points.default_point_object
         elif new_object_type == objects_common.object_type.section:
             default_object = objects_sections.default_section_object
         elif new_object_type == objects_common.object_type.instrument:
             default_object = objects_instruments.default_instrument_object
         else:
             default_object = {}
-            logging.warning("LOAD LAYOUT - "+new_object_type+" "+item_id+" - Unrecognised object type: '"+new_object_type+"'")
-            warning_messages += (new_object_type+" "+item_id+" - Unrecognised object type - DISCARDED\n")
+            warning_message = (new_object_type+" "+str(item_id)+
+                            " - Unrecognised object type - DISCARDED")
+            logging.warning("LOAD LAYOUT - "+warning_message)
+            warning_messages.append(warning_message)
         # Populate each element at a time and report any elements not recognised
         if default_object != {}:
             objects_common.schematic_objects[object_id] = copy.deepcopy(default_object)
             for element in new_objects[object_id]:
                 if element not in default_object.keys():
-                    logging.warning("LOAD LAYOUT - "+new_object_type+" "+item_id+" - Unexpected element: '"+element+"'")
-                    warning_messages += (new_object_type+" "+item_id+" - Unexpected element: '"+element+"'\n")
+                    warning_message = (new_object_type+" "+str(item_id)+
+                            " - Unexpected element: '"+element+"' - DISCARDED")
+                    logging.warning("LOAD LAYOUT - "+warning_message)
+                    warning_messages.append(warning_message)
+                ##################################################################################
+                ### Handle breaking change of lines having Item IDs from Release 3.4.0 onwards ###
+                elif (new_object_type == objects_common.object_type.line and
+                          element == "itemid" and new_objects[object_id][element] is None):                    
+                    item_id = one_up_line_id
+                    objects_common.schematic_objects[object_id][element] = one_up_line_id
+                    warning_message = (new_object_type+
+                            " ? - Missing Item ID - assigning default ID '"+str(item_id)+"'")
+                    logging.warning("LOAD LAYOUT - "+warning_message)
+                    warning_messages.append(warning_message)
+                    one_up_line_id = one_up_line_id + 1
+                ### Handle breaking change of lines having Item IDs from Release 3.4.0 onwards ###
+                ##################################################################################
                 else:
                     objects_common.schematic_objects[object_id][element] = new_objects[object_id][element]        
             # Now report any elements missing from the new object - intended to provide a
             # level of backward capability (able to load old config files into an extended config)
             for element in default_object:
                 if element not in new_objects[object_id].keys():
-                    logging.warning("LOAD LAYOUT - "+new_object_type+" "+item_id+" - Missing element: '"+element+"'")
-                    warning_messages += (new_object_type+" "+item_id+" - Missing element: '"+element+"'\n")
-                    #############################################################################################
-                    # Set any mandatory elements - to prevent the application from breaking
-                    # When loading files saved by old versions of the application (this specifically
-                    # for the block instrument type breaking change from Release 3.2.0 to 3.3.0
-                    if element == "itemtype": objects_common.schematic_objects[object_id][element] = 1
-                    #############################################################################################
-    # Report the error messages
-    if warning_messages != "": display_warnings(warning_messages)
+                    default_value = objects_common.schematic_objects[object_id][element]
+                    warning_message = (new_object_type+" "+str(item_id)+" - Missing element: '"
+                            +element+"' - Asigning default values: "+str(default_value))
+                    logging.warning("LOAD LAYOUT - "+warning_message)
+                    warning_messages.append(warning_message)
     # Reset the signal/point/section/instrument indexes
     reset_all_schematic_indexes()
     # Redraw (re-create) all items on the schematic with a new bbox
     redraw_all_objects(create_new_bbox=True)
     # Ensure all track sections are in front of any lines
     bring_track_sections_to_the_front()
     # Recalculate point interlocking tables as a 'belt and braces' measure (on the 
     # basis they would have successfully been loaded with the rest of the configuration)
     objects_points.reset_point_interlocking_tables()
     # Initialise the layout (interlocking changes, signal aspects etc)
     run_layout.initialise_layout()    
     # save the current state (for undo/redo) - deleting all previous history
     save_schematic_state(reset_pointer=True)
-    return()
+    # Return the list of warning messages (for display to the user)
+    return(warning_messages)
 
 #------------------------------------------------------------------------------------
 # Function get the current objects dictionary (for saving to file)
 #------------------------------------------------------------------------------------
 
 def get_all():
     return(objects_common.schematic_objects)
 
-#------------------------------------------------------------------------------------
-# Internal Function to generate a popup window to display load errors
-#------------------------------------------------------------------------------------
-
-class display_warnings():
-    def __init__(self, warnings:str):
-        # Create the top level window for the canvas settings
-        winx = objects_common.canvas.winfo_rootx() + 250
-        winy = objects_common.canvas.winfo_rooty() + 50
-        self.window = Tk.Toplevel(objects_common.canvas)
-        self.window.geometry(f'+{winx}+{winy}')
-        self.window.title("Load Warnings")
-        self.window.attributes('-topmost',True)
-        self.label1 = Tk.Label(self.window, font="Helvetica 12 bold", text=
-                    "WARNING - Layout file generated by a different\n"+
-                    "version of the application - Check configuration")
-        self.label1.pack(padx=2, pady=2)
-        self.label2 = Tk.Label(self.window, text=warnings, justify=Tk.LEFT)
-        self.label2.pack(padx=2, pady=2)
-        # Create the close button 
-        self.B1 = Tk.Button (self.window, text = "Ok / Close",command=self.ok)
-        self.B1.pack(padx=2, pady=2)
-
-    def ok(self):
-        self.window.destroy()
-
 ####################################################################################
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/editor/objects/objects_common.py` & `model-railway-signals-3.4.0/model_railway_signals/editor/objects/objects_common.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,26 +8,29 @@
 #    set_bbox - Common function to create/update the boundary box for a schematic object
 #    find_initial_canvas_position - common function to return the next 'free' position (x,y)
 #    new_item_id - Common function - common function to return the next 'free' item ID
 #    signal_exists (item_id:int) - Common function to see if a given item exists
 #    point_exists (item_id:int) - Common function to see if a given item exists
 #    section_exists (item_id:int) - Common function to see if a given item exists
 #    instrument_exists (item_id:int) - Common function to see if a given item exists
+#    line_exists (item_id:int) - Common function to see if a given item exists
 #    signal(item_id:int) - helper function to find the object Id by Item ID
 #    point(item_id:int) - helper function to find the object Id by Item ID
 #    section(item_id:int) - helper function to find the object Id by Item ID
 #    instrument(item_id:int) - helper function to find the object Id by Item ID
+#    line(item_id:int) - helper function to find the object Id by Item ID
 #
 # Objects intended to be accessed directly by other editor modules:
 #    object_type - Enumeration type for the supported objects
 #    schematic_objects - for accessing/editing the configuration of an object
 #    signal_index - for iterating through all the signal objects
 #    point_index - for iterating through all the point objects
 #    instrument_index - for iterating through all the instrument objects
 #    section_index - for iterating through all the section objects
+#    line_index - for iterating through all the line objects
 #    canvas_width, canvas_height, canvas_grid - for creating/pasting objects
 #    canvas - global reference to the Tkinter drawing object
 #
 # Makes the following external API calls to other editor modules:
 #    run_layout.initialise(canvas) - Initialise the run_layout module with the canvas reference
 #
 #------------------------------------------------------------------------------------
@@ -59,32 +62,35 @@
 # object_id to be indexed by the item_id (unique only for each object_type)
 #------------------------------------------------------------------------------------
 
 signal_index:dict={}
 point_index:dict={}
 instrument_index:dict={}
 section_index:dict={}
+line_index:dict={}
 
 #------------------------------------------------------------------------------------
 # Helper functions to get the main dictionary index (the object_id) from the item_id
 #------------------------------------------------------------------------------------
 
 def signal(ID:int): return (signal_index[str(ID)])
 def point(ID:int): return (point_index[str(ID)])
 def instrument(ID:int): return (instrument_index[str(ID)])
 def section(ID:int): return (section_index[str(ID)])
+def line(ID:int): return (line_index[str(ID)])
 
 #------------------------------------------------------------------------------------
 # Simple functions to test if a particular item_id already exists (for an item_type)
 #------------------------------------------------------------------------------------
 
 def signal_exists(ID:int): return (str(ID) in signal_index.keys())
 def point_exists(ID:int): return (str(ID) in point_index.keys())
 def instrument_exists(ID:int): return (str(ID) in instrument_index.keys())
 def section_exists(ID:int): return (str(ID) in section_index.keys())
+def line_exists(ID:int): return (str(ID) in line_index.keys())
 
 #------------------------------------------------------------------------------------
 # Common parameters for a Default Layout Object (i.e. state at creation)
 # These elements are common to all schematic layout objects and are primarily
 # used to support the schematic editor functions (move, select, etc)
 #------------------------------------------------------------------------------------
 
@@ -100,21 +106,23 @@
 # Function to set the required defaults for the Objects package at application start
 # The Tkinter Canvas Object and default canvas attributes (dimentions and grid size)
 # are saved as global variables for easy referencing. The Canvas width, height and grid
 # are used for optimising the positioning of objects on creation or 'paste'
 # Also calls the run_layout.initialise function to set the tkinter canvas object
 #------------------------------------------------------------------------------------
 
+root = None
 canvas = None
 canvas_width = 0
 canvas_height = 0
 canvas_grid = 0
 
-def initialise (canvas_object, width:int, height:int, grid:int):
-    global canvas
+def initialise (root_object,canvas_object, width:int, height:int, grid:int):
+    global canvas, root
+    root = root_object
     canvas = canvas_object
     update_canvas(canvas_width, canvas_height, grid)
     run_layout.initialise(canvas)
     return()
 
 #------------------------------------------------------------------------------------
 # Function to update the Canvas Attributes (following layout load or canvas resize)
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/editor/objects/objects_instruments.py` & `model-railway-signals-3.4.0/model_railway_signals/editor/objects/objects_instruments.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,16 +45,15 @@
 
 #------------------------------------------------------------------------------------
 # Default Block Instrument Objects (i.e. state at creation)
 #------------------------------------------------------------------------------------
 
 default_instrument_object = copy.deepcopy(objects_common.default_object)
 default_instrument_object["item"] = objects_common.object_type.instrument
-default_instrument_object["itemid"] = 0
-default_instrument_object["itemtype"] = None
+default_instrument_object["itemtype"] = block_instruments.instrument_type.single_line.value
 default_instrument_object["bellsound"] = "bell-ring-01.wav"
 default_instrument_object["keysound"] = "telegraph-key-01.wav"
 default_instrument_object["linkedto"] = ""
 
 #------------------------------------------------------------------------------------
 # Internal function Update references from instruments linked to this one
 #------------------------------------------------------------------------------------
@@ -84,16 +83,15 @@
             objects_common.schematic_objects[instrument_object]["linkedto"] = ""
             # We have to delete and re-create the 'linked' instrument for changes to take effect
             delete_instrument_object(instrument_object)
             redraw_instrument_object(instrument_object)
     return()
     
 #------------------------------------------------------------------------------------
-# Function to to update (delete and re-draw) an Instrument object on the schematic. Called
-# when the object is first created or after the object attributes have been updated
+# Function to to update an instrument object after a configuration change
 #------------------------------------------------------------------------------------
 
 def update_instrument(object_id, new_object_configuration):
     # We need to track whether the Item ID has changed
     old_item_id = objects_common.schematic_objects[object_id]["itemid"]
     new_item_id = new_object_configuration["itemid"]
     # Delete the existing instrument object, copy across the new config and redraw
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/editor/objects/objects_points.py` & `model-railway-signals-3.4.0/model_railway_signals/editor/objects/objects_points.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,16 +57,15 @@
 
 #------------------------------------------------------------------------------------
 # Default Point Objects (i.e. state at creation)
 #------------------------------------------------------------------------------------
 
 default_point_object = copy.deepcopy(objects_common.default_object)
 default_point_object["item"] = objects_common.object_type.point
-default_point_object["itemid"] = 0
-default_point_object["itemtype"] = None
+default_point_object["itemtype"] = points.point_type.LH.value
 default_point_object["orientation"] = 0
 default_point_object["colour"] = "black"
 default_point_object["alsoswitch"] = 0
 default_point_object["reverse"] = False
 default_point_object["automatic"] = False
 default_point_object["hasfpl"] = False
 default_point_object["dccaddress"] = 0
@@ -173,16 +172,15 @@
             points.toggle_point_state(also_switch_id,True)
             # Recursively call back into the function with the object ID for the other point
             update_downstream_points(objects_common.point(str(also_switch_id)))
     return()
 
 
 #------------------------------------------------------------------------------------
-# Function to update (delete and re-draw) a Point object on the schematic. Called
-# when the object is first created or after the object attributes have been updated.
+# Function to to update a point object after a configuration change
 #------------------------------------------------------------------------------------
 
 def update_point(object_id, new_object_configuration):
     # We need to track whether the Item ID has changed
     old_item_id = objects_common.schematic_objects[object_id]["itemid"]
     new_item_id = new_object_configuration["itemid"]
     # Delete the existing point object, copy across the new configuration and redraw
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/editor/objects/objects_sections.py` & `model-railway-signals-3.4.0/model_railway_signals/editor/objects/objects_sections.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 
 #------------------------------------------------------------------------------------
 # Default Track Section Objects (i.e. state at creation)
 #------------------------------------------------------------------------------------
 
 default_section_object = copy.deepcopy(objects_common.default_object)
 default_section_object["item"] = objects_common.object_type.section
-default_section_object["itemid"] = 0
 default_section_object["defaultlabel"] = "XXXXX"
 default_section_object["label"] = default_section_object["defaultlabel"]
 default_section_object["state"] = False
 default_section_object["editable"] = True
 default_section_object["mirror"] = ""
 
 #------------------------------------------------------------------------------------
@@ -145,16 +144,15 @@
         section_object = objects_common.section(section_id)
         # We use string comparison as the IDs support local or remote sections
         if objects_common.schematic_objects[section_object]["mirror"] == str(deleted_sec_id):
             objects_common.schematic_objects[section_object]["mirror"] = ""
     return()
 
 #------------------------------------------------------------------------------------
-# Function to update (delete and re-draw) a Track Section object on the schematic. Called
-# when the object is first created or after the object attributes have been updated.
+# Function to to update asection object after a configuration change
 #------------------------------------------------------------------------------------
 
 def update_section(object_id, new_object_configuration):
     # We need to track whether the Item ID has changed
     old_item_id = objects_common.schematic_objects[object_id]["itemid"]
     new_item_id = new_object_configuration["itemid"]
     # Delete the existing section object, copy across the new config and redraw
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/editor/objects/objects_signals.py` & `model-railway-signals-3.4.0/model_railway_signals/editor/objects/objects_signals.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,22 +37,22 @@
 #    signals_common.sig_type - for setting the enum value when creating the object
 #    signals_colour_lights.signal_sub_type - for setting the enum value when creating the object
 #    signals_semaphores.semaphore_sub_type - for setting the enum value when creating the object
 #    signals_ground_position.ground_pos_sub_type - for setting the enum value when creating the object
 #    signals_ground_disc.ground_disc_sub_type - for setting the enum value when creating the object
 #
 # Makes the following external API calls to library modules:
-#    signals.delete_signal(id) - delete library drawing object (part of soft delete)
-#    signals.get_tags(id) - get the canvas 'tags' for the signal drawing objects
 #    signals.update_signal(id) - To set the initial colour light signal aspect following creation
 #    signals.set_route(id,route) - To set the initial route for a signal following creation
 #    signals_colour_lights.create_colour_light_signal - To create the library object (create or redraw)
 #    signals_semaphores.create_semaphore_signal - To create the library object (create or redraw)
 #    signals_ground_position.create_ground_position_signal - To create the library object (create or redraw)
 #    signals_ground_disc.create_ground_disc_signal - To create the library object (create or redraw)
+#    signals_common.get_tags(id) - get the canvas 'tags' for the signal drawing objects
+#    signals_common.delete_signal(id) - delete library drawing object (part of soft delete)
 #    dcc_control.delete_signal_mapping - delete the existing DCC mapping for the signal
 #    dcc_control.map_dcc_signal - to create a new DCC mapping for the signal
 #    dcc_control.map_semaphore_signal - to create a new DCC mapping for the signal
 #    track_sensors.delete_sensor_mapping - delete the existing signal sensor mapping
 #    track_sensors.create_track_sensor - To create a new signal sensor mapping
 #
 #------------------------------------------------------------------------------------
@@ -76,17 +76,16 @@
 #------------------------------------------------------------------------------------
 # Default Signal Objects (i.e. state at creation)
 #------------------------------------------------------------------------------------
 
 # This is the default signal object definition
 default_signal_object = copy.deepcopy(objects_common.default_object)
 default_signal_object["item"] = objects_common.object_type.signal
-default_signal_object["itemid"] = 0
-default_signal_object["itemtype"] = None
-default_signal_object["itemsubtype"] = None
+default_signal_object["itemtype"] = signals_common.sig_type.colour_light.value
+default_signal_object["itemsubtype"] = signals_colour_lights.signal_sub_type.four_aspect.value
 default_signal_object["orientation"] = 0 
 default_signal_object["subsidary"] = [False,0]  # [has_subsidary, dcc_address]
 default_signal_object["theatreroute"] = False
 default_signal_object["feathers"] = [False,False,False,False,False]  # [MAIN,LH1,LH2,RH1,RH2]
 default_signal_object["dccautoinhibit"] = False
 # Interlock a distant signal with all home signals ahead
 default_signal_object["interlockahead"] = False
@@ -411,16 +410,15 @@
         interlocking_table = objects_common.schematic_objects[sig_object]["pointinterlock"]
         for index, interlocked_route in enumerate (interlocking_table):
             if interlocked_route[2] == old_inst_id:
                 objects_common.schematic_objects[sig_object]["pointinterlock"][index][2] = new_inst_id
     return()
 
 #------------------------------------------------------------------------------------
-# Function to update (delete and re-draw) a Signal object on the schematic. Called
-# when the object is first created or after the object attributes have been updated.
+# Function to to update a signal object after a configuration change
 #------------------------------------------------------------------------------------
 
 def update_signal(object_id, new_object_configuration):
     # We need to track whether the Item ID has changed
     old_item_id = objects_common.schematic_objects[object_id]["itemid"]
     new_item_id = new_object_configuration["itemid"]    
     # Delete the existing signal object, copy across the new configuration and redraw
@@ -596,15 +594,15 @@
                     x = objects_common.schematic_objects[object_id]["posx"],
                     y = objects_common.schematic_objects[object_id]["posy"],
                     signal_subtype = sub_type,
                     sig_callback = run_layout.schematic_callback,
                     orientation = objects_common.schematic_objects[object_id]["orientation"],
                     sig_passed_button = objects_common.schematic_objects[object_id]["passedsensor"][0]) 
     # Create/update the canvas "tags" and selection rectangle for the signal
-    objects_common.schematic_objects[object_id]["tags"] = signals.get_tags(objects_common.schematic_objects[object_id]["itemid"])
+    objects_common.schematic_objects[object_id]["tags"] = signals_common.get_tags(objects_common.schematic_objects[object_id]["itemid"])
     objects_common.set_bbox (object_id, objects_common.canvas.bbox(objects_common.schematic_objects[object_id]["tags"]))         
     return()
 
 #------------------------------------------------------------------------------------
 # Function to Create a new default signal (and draw it on the canvas)
 #------------------------------------------------------------------------------------
 
@@ -686,34 +684,33 @@
 # associated dcc mappings and track sensor mappings. Primarily used to delete the
 # signal in its current configuration prior to re-creating in its new configuration
 # following a configuration change - also used as part of a hard delete (below)
 #------------------------------------------------------------------------------------
 
 def delete_signal_object(object_id):
     # Delete the signal drawing objects and associated DCC mapping
-    signals.delete_signal(objects_common.schematic_objects[object_id]["itemid"])
+    signals_common.delete_signal(objects_common.schematic_objects[object_id]["itemid"])
     dcc_control.delete_signal_mapping(objects_common.schematic_objects[object_id]["itemid"])
     # Delete the track sensor mappings for the signal (if any)
     track_sensors.delete_sensor_mapping(objects_common.schematic_objects[object_id]["itemid"]*10)
     track_sensors.delete_sensor_mapping(objects_common.schematic_objects[object_id]["itemid"]*10+1)
     # Delete the associated distant signal (if there is one)
-    signals.delete_signal(objects_common.schematic_objects[object_id]["itemid"]+100)
+    signals_common.delete_signal(objects_common.schematic_objects[object_id]["itemid"]+100)
     dcc_control.delete_signal_mapping(objects_common.schematic_objects[object_id]["itemid"]+100)
     return()
 
 #------------------------------------------------------------------------------------
 # Function to 'hard delete' a signal (drawing objects, DCC mappings, sensor mappings,
 # and the main dict entry). Function called when signal is deleted from the schematic.
 #------------------------------------------------------------------------------------
 
 def delete_signal(object_id):
     # Soft delete the associated library objects from the canvas
     delete_signal_object(object_id)
     # Remove any references to the signal from other signals
-    # Interlocking tables, signal ahead, timed signal sequences
     remove_references_to_signal(objects_common.schematic_objects[object_id]["itemid"])
     # "Hard Delete" the selected object - deleting the boundary box rectangle and deleting
     # the object from the dictionary of schematic objects (and associated dictionary keys)
     objects_common.canvas.delete(objects_common.schematic_objects[object_id]["bbox"])
     del objects_common.signal_index[str(objects_common.schematic_objects[object_id]["itemid"])]
     del objects_common.schematic_objects[object_id]
     # Recalculate point interlocking tables to remove references to the signal
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/editor/resources/block_instrument.png` & `model-railway-signals-3.4.0/model_railway_signals/editor/resources/instrument.png`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.3.0/model_railway_signals/editor/resources/track_section.png` & `model-railway-signals-3.4.0/model_railway_signals/editor/resources/section.png`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.3.0/model_railway_signals/editor/run_layout.py` & `model-railway-signals-3.4.0/model_railway_signals/editor/run_layout.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 #    signals_common.sig_callback_type - for accessing the enum value
 #    points.point_callback_type - for accessing the enum value
 #    track_sections.section_callback_type - for accessing the enum value
 #    block_instruments.block_callback_type - for accessing the enum value
 #    block_instruments.block_section_ahead_clear - for interlocking
 #    signals_colour_lights.signal_sub_type - for accessing the enum value
 #    signals_semaphores.semaphore_sub_type - for accessing the enum value
+#    signals_ground_position.ground_pos_sub_type - for accessing the enum value
+#    signals_ground_disc.ground_disc_sub_type - for accessing the enum value
 #    <MORE COMING>
 #
 # Makes the following external API calls to library modules:
 #    signals.signal_state(sig_id) - For testing the current displayed aspect
 #    signals.update_signal(sig_id, sig_ahead_id) - To update the signal aspect
 #    signals.signal_clear(sig_id, sig_route) - To test if a signal is clear
 #    signals.subsidary_clear(sig_id) - to test if a subsidary is clear
@@ -64,14 +66,16 @@
 
 from ..library import signals
 from ..library import points
 from ..library import block_instruments
 from ..library import signals_common
 from ..library import signals_semaphores
 from ..library import signals_colour_lights
+from ..library import signals_ground_position
+from ..library import signals_ground_disc
 from ..library import track_sections
 
 from . import objects
 
 #------------------------------------------------------------------------------------
 # The Tkinter Canvas Object is saved as a global variable for easy referencing
 # The set_canvas function is called at application startup (on canvas creation)
@@ -189,15 +193,14 @@
 # see if the signal is local or remote (sigID is integer or string). If the signal
 # is a remote signal then we should stop processing (as we have no idea of the
 # signal type) and return home_signal_at_danger=False
 #####################################################################################
 #------------------------------------------------------------------------------------
 
 def home_signal_ahead_at_danger(signal_object, recursion_level:int=0):
-    global logging
     home_signal_at_danger = False
     if recursion_level < 20:
         signal_ahead_object = find_signal_ahead(signal_object)
         if signal_ahead_object is not None:
             signal_id = signal_ahead_object["itemid"]
             is_home = ( ( signal_ahead_object["itemtype"] == signals_common.sig_type.colour_light.value and
                           signal_ahead_object["itemsubtype"] == signals_colour_lights.signal_sub_type.home.value ) or
@@ -359,57 +362,76 @@
     # Find the section ahead and section behind the signal (0 = No section)
     signal_route = find_signal_route(signal_object)
     if signal_route is not None:
         section_ahead = signal_object["tracksections"][1][signal_route.value-1]
     else:
         section_ahead = 0
     section_behind = signal_object["tracksections"][0]
-    # Distant signals can be Passed even when ON and we have to cater for distants on a
-    # bi-directional running line so we need to assume the direction of travel depending
-    # on which section each side of the signal is CLEAR and which is OCCUPIED
-    if ( ( signal_object["itemtype"] == signals_common.sig_type.colour_light.value and
-           signal_object["itemsubtype"] == signals_colour_lights.signal_sub_type.distant.value ) or
-         ( signal_object["itemtype"] == signals_common.sig_type.semaphore.value and
-           signal_object["itemsubtype"] == signals_semaphores.semaphore_sub_type.distant.value ) ):
+    # Distant signals and shunt-ahead signals can be passed when ON so we need
+    # to assume the direction of travel depending on which section on each side
+    # of the signal is CLEAR and which is OCCUPIED. If both sections are CLEAR
+    # or both sections are OCCUPIED when the signal passed event is generated
+    # then we cannot infer or assume anything - and therefore take no action
+    item_type = signal_object["itemtype"]
+    item_sub_type = signal_object["itemsubtype"]
+    if ( ( item_type == signals_common.sig_type.colour_light.value and
+           item_sub_type == signals_colour_lights.signal_sub_type.distant.value ) or
+         ( item_type == signals_common.sig_type.semaphore.value and
+           item_sub_type == signals_semaphores.semaphore_sub_type.distant.value ) or
+         ( item_type == signals_common.sig_type.ground_position.value and
+           item_sub_type == signals_ground_position.ground_pos_sub_type.shunt_ahead.value ) or
+         ( item_type == signals_common.sig_type.ground_position.value and
+           item_sub_type == signals_ground_position.ground_pos_sub_type.early_shunt_ahead.value ) or
+         ( item_type == signals_common.sig_type.ground_disc.value and
+           item_sub_type == signals_ground_disc.ground_disc_sub_type.shunt_ahead.value ) ):
         if ( section_ahead > 0 and track_sections.section_occupied(section_ahead) and
              section_behind > 0 and not track_sections.section_occupied(section_behind) ):
-            # Assume Direction of travel 'against' the signal
+            # Section ahead of signal is OCCUPIED and section behind is CLEAR
+            # Assume Direction of travel 'against' the signal (and 'pass' the train)
             track_sections.set_section_occupied (section_behind,
                    track_sections.clear_section_occupied(section_ahead))
         elif ( section_ahead > 0 and not track_sections.section_occupied(section_ahead) and
              section_behind > 0 and track_sections.section_occupied(section_behind) ):
-            # Assume Direction of travel 'with' the signal
+            # Section behind signal is OCCUPIED and section ahead is CLEAR
+            # Assume Direction of travel 'with' the signal (and 'pass' the train)
             track_sections.set_section_occupied (section_ahead,
                    track_sections.clear_section_occupied(section_behind))
         elif section_ahead > 0 and not track_sections.section_occupied(section_ahead):
+            # Section ahead of signal is CLEAR - section behind doesn't exist
+            # Assume Direction of travel 'with' the signal - set section ahead to OCCUPIED
             track_sections.set_section_occupied(section_ahead)
         elif section_behind > 0 and not track_sections.section_occupied(section_behind):
-            track_sections.set_section_occupied(section_behind)
+            # Section behind signal is CLEAR - section ahead doesn't exist
+            # Assume Direction of travel 'against' the signal - set section behind to OCCUPIED
+           track_sections.set_section_occupied(section_behind)
         elif section_ahead > 0 and track_sections.section_occupied(section_ahead):
+            # Section ahead of signal is OCCUPIED - section behind doesn't exist
+            # Assume Direction of travel 'against' the signal - set section ahead to CLEAR
             track_sections.clear_section_occupied(section_ahead)
         elif section_behind > 0 and track_sections.section_occupied(section_behind):
+            # Section behind signal is OCCUPIED - section ahead doesn't exist
+            # Assume Direction of travel 'with' the signal - set section behind to CLEAR
             track_sections.clear_section_occupied(section_behind)
     # Non-distant signals can only be passed when CLEAR (as long as the driver is
-    # doing their job so we assume direction of travel from signal CLEAR
+    # doing their job properly) so we assume direction of travel is 'with' the signal
+    # This is also important to cater for the case of opposing signals protecting
+    # points (with no track sections in between) - in this case, both signals will
+    # generate 'passed' events but we only act on the route that has been cleared
     elif ( signals.signal_clear(signal_id) or ( has_subsidary(signal_id)
                     and signals.subsidary_clear(signal_id) ) ):
-        # Update the track occupancy sections behind and ahead of the signal
-        # Also set/clear any overrides for this signal and the signal behind
-        signal_route = find_signal_route(signal_object)
-        section_behind = signal_object["tracksections"][0]
-        if signal_route is not None:
-            section_ahead = signal_object["tracksections"][1][signal_route.value-1]
-        else:
-            section_ahead = 0
         if section_ahead > 0 and section_behind > 0:
+            # Sections ahead of and behind the signal both exist ('pass' the train)
             track_sections.set_section_occupied (section_ahead,
                    track_sections.clear_section_occupied(section_behind))
         elif section_ahead > 0:
+            # Only the section ahead of the signal exists - set to OCCUPIED
+            # Assume Direction of travel 'against' the signal (and 'pass' train)
             track_sections.set_section_occupied(section_ahead)
         elif section_behind > 0:
+            # Only the section behind the signal exists - set to CLEAR
             track_sections.clear_section_occupied(section_behind)
     # Propagate changes to any mirrored track sections
     if section_ahead > 0:
         update_mirrored_section(objects.schematic_objects[objects.section(section_ahead)])
     if section_behind > 0:
         update_mirrored_section(objects.schematic_objects[objects.section(section_behind)])
     return()
@@ -723,15 +745,14 @@
 # Main callback function for when anything on the layout changes
 #####################################################################################
 # TODO - Update callback in light of the move to using IDs rather than objects
 #####################################################################################
 #------------------------------------------------------------------------------------
 
 def schematic_callback(item_id,callback_type):
-    global logging
     global editing_enabled
     logging.info("RUN LAYOUT - Callback - Item: "+str(item_id)+" - Callback Type: "+str(callback_type))
 
     # Timed signal sequences can be triggered by 'signal_passed' events
     if callback_type == signals_common.sig_callback_type.sig_passed:
         logging.info("RUN LAYOUT - Triggering any Timed Signal sequences (signal passed event):")
         trigger_timed_sequence(objects.schematic_objects[objects.signal(item_id)])
@@ -820,15 +841,14 @@
 #------------------------------------------------------------------------------------
 # Function to "initialise" the layout following a reset / re-load or item deletion
 # Also called after the configuration change of any layout object
 #------------------------------------------------------------------------------------
 
 def initialise_layout():
     global editing_enabled
-    global logging
     logging.info("RUN LAYOUT - Initialising Schematic **************************************************")
     logging.info("RUN LAYOUT - Updating Signal Routes based on Point settings:")
     set_all_signal_routes()
     # Track sections (the library objects) only "exist" in run mode"
     if editing_enabled:
         logging.info("RUN LAYOUT - Clearing down any Signal Overrides (for edit mode):")
         clear_all_signal_overrides()
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/editor/schematic.py` & `model-railway-signals-3.4.0/model_railway_signals/editor/schematic.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 # This Module provides all the internal functions for editing the layout schematic
 # in terms of adding/removing objects, drag/drop objects, copy/paste objects etc
 #------------------------------------------------------------------------------------
 #
 # External API functions intended for use by other editor modules:
 #    initialise(root, callback, width, height, grid) - Call once on startup
 #    update_canvas() - Call following a size update (or layout load/canvas resize)
-#    select_all_objects() - For selecting all objects prior to a "safe" delete
-#    delete_selected_objects() - To delete all objects (once all are selected)
+#    delete_all_objects() - To delete all objects for layout 'new' and layout 'load'
 #    enable_editing() - Call when 'Edit' Mode is selected (via toolbar or on load)
 #    disable_editing() - Call when 'Run' Mode is selected (via toolbar or on load)
 #
 # Makes the following external API calls to other editor modules:
 #    objects.initialise (canvas,width,height,grid) - Initialise the objects package and set defaults
 #    objects.update_canvas(width,height,grid) - update the attributes (on layout load or canvas re-size)
 #    objects.create_object(obj, type, subtype) - Create a default object on the schematic
@@ -22,14 +21,15 @@
 #    objects.undo() / objects.redo() - Undo and re-do functions as you would expect
 #    objects.enable_editing() - Call when 'Edit' Mode is selected 
 #    objects.disable_editing() - Call when 'Run' Mode is selected
 #    configure_signal.edit_signal(root,object_id) - Open signal edit window (on double click)
 #    configure_point.edit_point(root,object_id) - Open point edit window (on double click)
 #    configure_section.edit_section(root,object_id) - Open section edit window (on double click)
 #    configure_instrument.edit_instrument(root,object_id) - Open inst edit window (on double click)
+#    configure_line.edit_line(root,object_id) - Open line edit window (on double click)
 #    ########################## More to be added ########################################
 #
 # Accesses the following external editor objects directly:
 #    objects.schematic_objects - the dict holding descriptions for all objects
 #    objects.object_type - used to establish the type of the schematic objects
 #
 # Accesses the following external library objects directly:
@@ -55,17 +55,17 @@
 from ..library import points
 
 from . import objects
 from . import configure_signal
 from . import configure_point
 from . import configure_section
 from . import configure_instrument
+from . import configure_line
 
 import importlib.resources
-import logging
 import math
 import copy
 
 #------------------------------------------------------------------------------------
 # Global variables used to track the current selections/state of the Schematic Editor
 #------------------------------------------------------------------------------------
 
@@ -99,14 +99,25 @@
 popup2 = None
 # The Frame holding the "add object" buttons (for pack/forget on enable/disable editing)
 # and the Tkinter PhotoImage labels for the buttons
 button_frame = None
 button_images = {}
 
 #------------------------------------------------------------------------------------
+# Internal Function to return the absolute canvas coordinates for an event
+# (which take into account any canvas scroll bar offsets)
+#------------------------------------------------------------------------------------
+
+def canvas_coordinates(event):
+    canvas = event.widget
+    x = canvas.canvasx(event.x)
+    y = canvas.canvasy(event.y)
+    return(x, y)
+
+#------------------------------------------------------------------------------------
 # Internal Function to draw (or redraw) the grid on the screen (after re-sizing)
 # Uses the global canvas_width, canvas_height, canvas_grid variables
 #------------------------------------------------------------------------------------
 
 def draw_grid():
     # Note we leave the 'state' of the grid  unchanged when re-drawing
     # As the 'state' is set (normal or hidden) when enabling/disabling editing
@@ -171,22 +182,38 @@
 def deselect_all_objects(event=None):
     selections = copy.deepcopy(schematic_state["selectedobjects"])
     for object_id in selections:
         deselect_object(object_id)
     return()
 
 #------------------------------------------------------------------------------------
+# Internal function to delete all objects (for layout 'load' and layout 'new'
+#------------------------------------------------------------------------------------
+
+def delete_all_objects():
+    global schematic_state
+    # Select and delete all objects (also clear the selected objects list)
+    select_all_objects()
+    delete_selected_objects()
+    # Belt and braces delete of all canvas objects as I've seen issues when
+    # running the system tests (probably because I'm not using the mainloop)
+    canvas.delete("all")
+    # Set the select area box to 'None' so it gets created on first use
+    schematic_state["selectareabox"] = None
+    return()
+
+#------------------------------------------------------------------------------------
 # Internal function to edit an object configuration (double-click and popup menu)
 # Only a single Object will be selected when this function is called
 #------------------------------------------------------------------------------------
 
 def edit_selected_object():
     object_id = schematic_state["selectedobjects"][0]
     if objects.schematic_objects[object_id]["item"] == objects.object_type.line:
-        pass; #################### TODO #############################
+        configure_line.edit_line(root, object_id)
     elif objects.schematic_objects[object_id]["item"] == objects.object_type.signal:
         configure_signal.edit_signal(root, object_id)
     elif objects.schematic_objects[object_id]["item"] == objects.object_type.point:
         configure_point.edit_point(root, object_id)
     elif objects.schematic_objects[object_id]["item"] == objects.object_type.section:
         configure_section.edit_section(root,object_id)
     elif objects.schematic_objects[object_id]["item"] == objects.object_type.instrument:
@@ -210,14 +237,20 @@
         canvas.move(objects.schematic_objects[object_id]["end1"],xdiff,ydiff)
         x1,y1,x2,y2 = canvas.coords(objects.schematic_objects[object_id]["end1"])
         canvas.coords(objects.schematic_objects[object_id]["line"],(x1+x2)/2,(y1+y2)/2,endx,endy)
     elif schematic_state["editlineend2"]:
         canvas.move(objects.schematic_objects[object_id]["end2"],xdiff,ydiff)
         x1,y1,x2,y2 = canvas.coords(objects.schematic_objects[object_id]["end2"])
         canvas.coords(objects.schematic_objects[object_id]["line"],startx,starty,(x1+x2)/2,(y1+y2)/2)
+    # Update the coordinates for the line end stops using the 
+    # common function provided by the objects sub-package
+    x1,y1,x2,y2 = canvas.coords(objects.schematic_objects[object_id]["line"])
+    dx,dy = objects.get_endstop_offsets(x1,y1,x2,y2)
+    canvas.coords(objects.schematic_objects[object_id]["stop1"],x1+dx,y1+dy,x1-dx,y1-dy)
+    canvas.coords(objects.schematic_objects[object_id]["stop2"],x2+dx,y2+dy,x2-dx,y2-dy)
     return()
 
 #------------------------------------------------------------------------------------
 # Internal function to move all selected objects on the canvas
 #------------------------------------------------------------------------------------
         
 def move_selected_objects(xdiff:int,ydiff:int):
@@ -340,15 +373,19 @@
 # Right Button Click - Bring Up Context specific Popup menu
 # The event will only be bound to the canvas in "Edit" Mode
 #------------------------------------------------------------------------------------
 
 def right_button_click(event):
     global schematic_state
     # Find the object at the current cursor position (if there is one)
-    highlighted_object = find_highlighted_object(event.x,event.y)
+    # Note that we use the the canvas coordinates to see if the cursor
+    # is over the object (as these take into account the current scroll
+    # bar positions) and the event root coordinates for the popup 
+    canvas_x, canvas_y = canvas_coordinates(event)
+    highlighted_object = find_highlighted_object(canvas_x, canvas_y)
     if highlighted_object:
         # Clear any current selections and select the highlighted item
         deselect_all_objects()
         select_object(highlighted_object)
         # Enable the Object popup menu (which will be for the selected object)
         popup1.tk_popup(event.x_root,event.y_root)
     else:
@@ -362,59 +399,63 @@
 # The event will only be bound to the canvas in "Edit" Mode
 #------------------------------------------------------------------------------------
 
 def left_button_click(event):
     global schematic_state
     # set keyboard focus for the canvas (so that any key bindings will work)
     canvas.focus_set()
-    # For canvas events we can use the canvas coordinates
-    schematic_state["startx"] = event.x 
-    schematic_state["starty"] = event.y
-    schematic_state["lastx"] = event.x 
-    schematic_state["lasty"] = event.y
+    # Get the canvas coordinates (to take into account any scroll bar offsets) 
+    canvas_x, canvas_y = canvas_coordinates(event)
+    schematic_state["startx"] = canvas_x 
+    schematic_state["starty"] = canvas_y
+    schematic_state["lastx"] = canvas_x 
+    schematic_state["lasty"] = canvas_y
     # See if the cursor is over the "end" of an already selected line 
-    highlighted_object = find_highlighted_line_end(event.x,event.y)
+    highlighted_object = find_highlighted_line_end(canvas_x,canvas_y)
     if highlighted_object:
         # Clear selections and select the highlighted line. Note that the edit line
         # mode ("editline1" or "editline2") get set by "find_highlighted_line_end"
         deselect_all_objects()
         select_object(highlighted_object)
     else:
         # See if the cursor is over any other canvas object
-        highlighted_object = find_highlighted_object(event.x,event.y)
+        highlighted_object = find_highlighted_object(canvas_x,canvas_y)
         if highlighted_object:
             schematic_state["moveobjects"] = True
             if highlighted_object not in schematic_state["selectedobjects"]:
                 # Clear any current selections and select the highlighted object
                 deselect_all_objects()
                 select_object(highlighted_object)
         else:
             # Cursor is not over any object - Could be the start of a new area selection or
             # just clearing the current selection - In either case we deselect all objects
             deselect_all_objects()
             schematic_state["selectarea"] = True
-            #  Make the "select area" box visible (create it if necessary)
-            if not schematic_state["selectareabox"]:
+            # Make the 'selectareabox' visible. This will create the box on first use
+            # or after a 'delete_all_objects (when the box is set to 'None')
+            if schematic_state["selectareabox"] is None:
                 schematic_state["selectareabox"] = canvas.create_rectangle(0,0,0,0,outline="orange")
-            canvas.coords(schematic_state["selectareabox"],event.x,event.y,event.x,event.y)
+            canvas.coords(schematic_state["selectareabox"],canvas_x,canvas_y,canvas_x,canvas_y)
             canvas.itemconfigure(schematic_state["selectareabox"],state="normal")
     # Unbind the canvas keypresses until left button release to prevent mode changes,
     # rotate/delete of objects (i.e. prevent undesirable editor behavior)
     disable_all_keypress_events()
     return()
 
 #------------------------------------------------------------------------------------
 # Left-Shift-Click - Select/deselect Object
 # The event will only be bound to the canvas in "Edit" Mode
 #------------------------------------------------------------------------------------
 
 def left_shift_click(event):
     global schematic_state
+    # Get the canvas coordinates (to take into account any scroll bar offsets) 
+    canvas_x, canvas_y = canvas_coordinates(event)
     # Find the object at the current cursor position (if there is one)
-    highlighted_object = find_highlighted_object(event.x,event.y)
+    highlighted_object = find_highlighted_object(canvas_x,canvas_y)
     if highlighted_object and highlighted_object in schematic_state["selectedobjects"]:
         # Deselect just the highlighted object (leave everything else selected)
         deselect_object(highlighted_object)
     else:
         # Select the highlighted object to the list of selected objects
         select_object(highlighted_object)
     return()
@@ -422,16 +463,18 @@
 #------------------------------------------------------------------------------------
 # Left-Double-Click - Bring up edit object dialog for object
 # The event will only be bound to the canvas in "Edit" Mode
 #------------------------------------------------------------------------------------
 
 def left_double_click(event):
     global schematic_state
+    # Get the canvas coordinates (to take into account any scroll bar offsets) 
+    canvas_x, canvas_y = canvas_coordinates(event)
     # Find the object at the current cursor position (if there is one)
-    highlighted_object = find_highlighted_object(event.x,event.y)
+    highlighted_object = find_highlighted_object(canvas_x,canvas_y)
     if highlighted_object:
         # Clear any current selections and select the highlighted item
         deselect_all_objects()
         select_object(highlighted_object)
         # Call the function to open the edit dialog for the object
         edit_selected_object()
     return()
@@ -439,36 +482,38 @@
 #------------------------------------------------------------------------------------
 # Track Cursor - Move Selected Objects / Edit Selected Line / Change Area Selection
 # The event will only be bound to the canvas in "Edit" Mode
 #------------------------------------------------------------------------------------
 
 def track_cursor(event):
     global schematic_state
+    # Get the canvas coordinates (to take into account any scroll bar offsets) 
+    canvas_x, canvas_y = canvas_coordinates(event)
     if schematic_state["moveobjects"]:
         # Work out the delta movement since the last re-draw
-        deltax = event.x - schematic_state["lastx"]
-        deltay = event.y - schematic_state["lasty"]
+        deltax = canvas_x - schematic_state["lastx"]
+        deltay = canvas_y - schematic_state["lasty"]
         # Move all the objects that are selected
         move_selected_objects(deltax,deltay)
         # Set the 'last' position for the next move event
         schematic_state["lastx"] += deltax
         schematic_state["lasty"] += deltay
     elif schematic_state["editlineend1"] or schematic_state["editlineend2"]:
-        deltax = event.x - schematic_state["lastx"]
-        deltay = event.y - schematic_state["lasty"]
+        deltax = canvas_x - schematic_state["lastx"]
+        deltay = canvas_y - schematic_state["lasty"]
         # Move all the objects that are selected
         move_line_end(deltax,deltay)
         # Reset the "start" position for the next move
         schematic_state["lastx"] += deltax
         schematic_state["lasty"] += deltay
     elif schematic_state["selectarea"]:
         # Dynamically resize the selection area
         x1 = schematic_state["startx"]
         y1 = schematic_state["starty"]
-        canvas.coords(schematic_state["selectareabox"],x1,y1,event.x,event.y)
+        canvas.coords(schematic_state["selectareabox"],x1,y1,canvas_x,canvas_y)
     return()
 
 #------------------------------------------------------------------------------------
 # Left Button Release - Finish Object or line end Moves (by snapping to grid)
 # or select all objects within the canvas area selection box
 # The event will only be bound to the canvas in "Edit" Mode
 #------------------------------------------------------------------------------------
@@ -509,15 +554,16 @@
         # Calculate the total deltas for the move (from the startposition)
         finalx = schematic_state["lastx"] - schematic_state["startx"] + xdiff
         finaly = schematic_state["lasty"] - schematic_state["starty"] + ydiff
         # Finalise the move by updating the current object position
         objects.move_objects(schematic_state["selectedobjects"], xdiff2=finalx, ydiff2=finaly)
         # Clear the "Edit line mode" - but leave the line selected
         schematic_state["editlineend2"] = False
-    elif schematic_state["selectarea"]:
+        # Note the defensive programming - to ensure the bbox exists
+    elif schematic_state["selectarea"] and schematic_state["selectareabox"] is not None:
         # Select all Objects that are fully within the Area Selection Box
         abox = canvas.coords(schematic_state["selectareabox"])
         for object_id in objects.schematic_objects:
             bbox = canvas.coords(objects.schematic_objects[object_id]["bbox"])
             if bbox[0]>abox[0] and bbox[2]<abox[2] and bbox[1]>abox[1] and bbox[3]<abox[3]:
                 select_object(object_id)
         # Clear the Select Area Mode and Hide the area selection rectangle
@@ -532,15 +578,16 @@
 # of new schematic or re-size of canvas via menubar). Updates the global variables
 #------------------------------------------------------------------------------------
 
 def update_canvas(width:int, height:int, grid:int):
     global canvas_width, canvas_height, canvas_grid
     # Update the tkinter canvas object
     canvas.config (width=width, height=height, scrollregion=(0,0,width, height))
-    canvas.pack()
+    # reset the root window size (this will fit to contents)
+    root.geometry("")
     # Set the global variables (used in the 'draw_grid' function)
     canvas_width = width
     canvas_height = height
     canvas_grid = grid
     draw_grid()
     # Also update the objects module with the new settings
     objects.update_canvas(width, height, grid)
@@ -606,20 +653,24 @@
 # Externally called Functions to enable/disable schematic editing
 # Either from the Menubar Mode selection or the 'm' key
 #------------------------------------------------------------------------------------
 
 def enable_editing():
     global schematic_state
     global canvas_event_callback
-    global button_frame
+    global button_frame, canvas_frame
     canvas.itemconfig("grid",state="normal")
     # Enable editing of the schematic objects
     objects.enable_editing()
-    # Re-pack the subframe containing the "add object" buttons to display it        
-    button_frame.pack(side=Tk.RIGHT, expand=False, fill=Tk.BOTH)
+    # Re-pack the subframe containing the "add object" buttons to display it. Note that we
+    # first 'forget' the canvas_frame and then re-pack the button_frame first, followed by
+    # the canvas_frame - this ensures that the buttons don't dissapear on window re-size
+    canvas_frame.forget()
+    button_frame.pack(side=Tk.LEFT, expand=False, fill=Tk.BOTH)
+    canvas_frame.pack(side=Tk.LEFT, expand=True, fill=Tk.BOTH)
     # Bind the Canvas mouse and button events to the various callback functions
     canvas.bind("<Motion>", track_cursor)
     canvas.bind('<Button-1>', left_button_click)
     canvas.bind('<Button-2>', right_button_click)
     canvas.bind('<Button-3>', right_button_click)
     canvas.bind('<Shift-Button-1>', left_shift_click)
     canvas.bind('<ButtonRelease-1>', left_button_release)
@@ -657,29 +708,29 @@
 #------------------------------------------------------------------------------------
 # Externally Called Initialisation function for the Canvas object
 #------------------------------------------------------------------------------------
 
 def initialise (root_window, event_callback, width:int, height:int, grid:int):
     global root, canvas, popup1, popup2
     global canvas_width, canvas_height, canvas_grid
-    global button_frame
-    global button_images
+    global button_frame, canvas_frame, buttons, images
     global canvas_event_callback
-    global logging
     root = root_window
     canvas_event_callback = event_callback
     # Create a frame to hold the two subframes ("add" buttons and drawing canvas)
     frame = Tk.Frame(root_window)
-    frame.pack (expand=True, fill=Tk.BOTH)    
-    # Create a subframe to hold the canvas and scrollbars
-    canvas_frame = Tk.Frame(frame, borderwidth=1)
-    canvas_frame.pack(side=Tk.RIGHT, expand=True, fill=Tk.BOTH)
+    frame.pack (expand=True, fill=Tk.BOTH)
+    # Note that we pack the button_frame first, followed by the canvas_frame
+    # This ensures that the buttons don't dissapear on window re-size (shrink)
     # Create a subframe to hold the "add" buttons
     button_frame = Tk.Frame(frame, borderwidth=1)
-    button_frame.pack(side=Tk.RIGHT, expand=True, fill=Tk.BOTH)
+    button_frame.pack(side=Tk.LEFT, expand=True, fill=Tk.BOTH)
+    # Create a subframe to hold the canvas and scrollbars
+    canvas_frame = Tk.Frame(frame, borderwidth=1)
+    canvas_frame.pack(side=Tk.LEFT, expand=True, fill=Tk.BOTH)
     # Save the Default values for the canvas as global variables
     canvas_width, canvas_height, canvas_grid = width, height, grid
     # Create the canvas and scrollbars inside the parent frame
     # We also set focus on the canvas so the keypress events will take effect
     canvas = Tk.Canvas(canvas_frame ,bg="grey85", scrollregion=(0, 0, canvas_width, canvas_height))
     canvas.focus_set()
     hbar = Tk.Scrollbar(canvas_frame, orient=Tk.HORIZONTAL)
@@ -699,63 +750,51 @@
     popup1.add_command(label="Delete", command=delete_selected_objects)
     # Define the Canvas Popup menu for Right Click (nothing selected)
     popup2 = Tk.Menu(tearoff=0)
     popup2.add_command(label="Paste", command=paste_clipboard_objects)
     popup2.add_command(label="Select all", command=select_all_objects)
     # Now draw the initial grid
     draw_grid()
-    # Load the images for the for the "add object" buttons
+    # Define the object buttons [filename, function_to_call]
+    selections = [ ["line", lambda:objects.create_object(objects.object_type.line) ],
+                   ["colourlight", lambda:objects.create_object(objects.object_type.signal,
+                                            signals_common.sig_type.colour_light.value,
+                                            signals_colour_lights.signal_sub_type.four_aspect.value) ],
+                   ["semaphore", lambda:objects.create_object(objects.object_type.signal,
+                                            signals_common.sig_type.semaphore.value,
+                                            signals_semaphores.semaphore_sub_type.home.value) ],
+                   ["groundpos", lambda:objects.create_object(objects.object_type.signal,
+                                            signals_common.sig_type.ground_position.value,
+                                            signals_ground_position.ground_pos_sub_type.standard.value) ],
+                   ["grounddisc", lambda:objects.create_object(objects.object_type.signal,
+                                            signals_common.sig_type.ground_disc.value,
+                                            signals_ground_disc.ground_disc_sub_type.standard.value) ],
+                   ["lhpoint", lambda:objects.create_object(objects.object_type.point,
+                                            points.point_type.LH.value) ],
+                   ["rhpoint", lambda:objects.create_object(objects.object_type.point,
+                                            points.point_type.RH.value) ],
+                   ["section", lambda:objects.create_object(objects.object_type.section) ],
+                   ["instrument", lambda:objects.create_object(objects.object_type.instrument,
+                                            block_instruments.instrument_type.single_line.value) ] ]
+    # Create the buttons we need (adding the references to the buttons and images
+    # to a global list so they don't go out of scope and dont get garbage collected)
+    buttons = []
+    images = []
     resource_folder = 'model_railway_signals.editor.resources'
-    file_names = ['line','colour_light','semaphore','ground_position','ground_disc',
-                'left_hand_point','right_hand_point','track_section','block_instrument']
-    for file_name in file_names:
+    for index, button in enumerate (selections):
+        file_name = selections[index][0]
         try:
+            # Load the image file for the button if there is one
             with importlib.resources.path (resource_folder,(file_name+'.png')) as file_path:
-                button_images[file_name] = Tk.PhotoImage(file=file_path)
+                images.append(Tk.PhotoImage(file=file_path))
+                buttons.append(Tk.Button (button_frame, image=images[-1],
+                       command=selections[index][1]))
         except:
-            logging.error ("SCHEMATIC EDITOR - Error loading image file '"+file_name+".png'")
-            button_images[file_name]=None
-    # Add The Buttons for creating new objects and adding to the schematic
-    # Note that for enumeration types we pass the "value"
-    button1 = Tk.Button (button_frame, image=button_images['line'],
-                      command=lambda:objects.create_object(objects.object_type.line))
-    button1.pack (padx=2 ,pady=2)
-    button2 = Tk.Button (button_frame, image=button_images['colour_light'],
-                      command=lambda:objects.create_object(objects.object_type.signal,
-                           signals_common.sig_type.colour_light.value,
-                           signals_colour_lights.signal_sub_type.four_aspect.value) )
-    button2.pack (padx=2, pady=2)
-    button3 = Tk.Button (button_frame, image=button_images['semaphore'],
-                      command=lambda:objects.create_object(objects.object_type.signal,
-                           signals_common.sig_type.semaphore.value,
-                           signals_semaphores.semaphore_sub_type.home.value))
-    button3.pack (padx=2, pady=2)
-    button4 = Tk.Button (button_frame, image=button_images['ground_position'],
-                      command=lambda:objects.create_object(objects.object_type.signal,
-                           signals_common.sig_type.ground_position.value,
-                           signals_ground_position.ground_pos_sub_type.standard.value))
-    button4.pack (padx=2, pady=2)
-    button5 = Tk.Button (button_frame, image=button_images['ground_disc'],
-                      command=lambda:objects.create_object(objects.object_type.signal,
-                           signals_common.sig_type.ground_disc.value,
-                           signals_ground_disc.ground_disc_sub_type.standard.value))
-    button5.pack (padx=2, pady=2)
-    button6 = Tk.Button (button_frame, image=button_images['left_hand_point'],
-                      command=lambda:objects.create_object(objects.object_type.point,
-                           points.point_type.LH.value))
-    button6.pack (padx=2, pady=2)
-    button7 = Tk.Button (button_frame, image=button_images['right_hand_point'],
-                      command=lambda:objects.create_object(objects.object_type.point,
-                            points.point_type.RH.value))
-    button7.pack (padx=2, pady=2)
-    button8 = Tk.Button (button_frame, image=button_images['track_section'],
-                      command=lambda:objects.create_object(objects.object_type.section))
-    button8.pack (padx=2, pady=2)
-    button9 = Tk.Button (button_frame, image=button_images['block_instrument'],
-                      command=lambda:objects.create_object(objects.object_type.instrument,
-                            block_instruments.instrument_type.single_line.value))
-    button9.pack (padx=2, pady=2)
+            # Else fall back to using a text label (filename) for the button
+            buttons.append(Tk.Button (button_frame, text=selections[index][0],
+                       command=selections[index][1]))
+        buttons[-1].pack(padx=2, pady=2)
     # Initialise the Objects package with the required parameters
-    objects.initialise(canvas, canvas_width, canvas_height, canvas_grid)
+    objects.initialise(root, canvas, canvas_width, canvas_height, canvas_grid)
     return()
 
 ####################################################################################
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/editor/settings.py` & `model-railway-signals-3.4.0/model_railway_signals/editor/settings.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 # This module maintains the settings for the schematic editor
 #
 # External API functions intended for use by other editor modules:
 #    restore_defaults() - Restores all defaults
 #    get_all() - returns dictionary of settings
 #    set_all(new_settings) - pass in dictionary of new settings
 #    get_general() - returns: (filename, editmode)
-#    set_general(filename, editmode)
+#    get_version() - returns: (application version)
+#    get_layout_info() - returns: (Layout info)
+#    set_layout_info(info) - pass in layout info
+#    set_general(filename, editmode)- pass in one or both
 #    get_canvas() - returns width, height, grid
 #    set_canvas(width, height, grid)
 #    get_logging() - returns level (1=Error, 2=Warning, 3=Info, 4=Debug)
 #    set_logging(level) (1=Error, 2=Warning, 3=Info, 4=Debug)
 #------------------------------------------------------------------------------------
 
 import copy
@@ -20,15 +23,16 @@
 # These are the default settings
 #------------------------------------------------------------------------------------
 
 default_settings = {}
 default_settings["general"] = {}
 default_settings["general"]["filename"] = "new_layout.sig"
 default_settings["general"]["editmode"] = True
-default_settings["general"]["version"] = "Version 3.3.0"
+default_settings["general"]["version"] = "Version 3.4.0"
+default_settings["general"]["info"] = "Document your layout here"
 default_settings["canvas"] = {}
 default_settings["canvas"]["width"] = 1000
 default_settings["canvas"]["height"] = 500
 default_settings["canvas"]["grid"] = 25
 default_settings["logging"] = {}
 default_settings["logging"]["level"] = 2   # Warning
 default_settings["sprog"] = {}
@@ -61,57 +65,84 @@
 # Functions to set/get all settings (for load and save)
 #------------------------------------------------------------------------------------
 
 def get_all():
     return(settings)
 
 def set_all(new_settings):
-    global settings, logging
+    global settings
+    # List of warning messages to report
+    warning_messages = []
     # Defensive programming to populate the settings gracefully
     restore_defaults()
     # Populate an element at a time - and report any elements we don't recognise
     for group in new_settings:
         if group not in settings.keys():
-            logging.error("LOAD LAYOUT - Unexpected settings group '"+group+"'")
+            warning_message = "Unexpected settings group '"+group+"' - DISCARDED"
+            logging.warning("LOAD LAYOUT - "+warning_message)
+            warning_messages.append(warning_message)
         else:
             for element in new_settings[group]:
                 if element not in settings[group].keys():
-                    logging.error("LOAD LAYOUT - Unexpected settings element '"+group+":"+element+"'")
+                    warning_message = "Unexpected settings element '"+group+":"+element+"' - DISCARDED"
+                    logging.warning("LOAD LAYOUT - "+warning_message)
+                    warning_messages.append(warning_message)
                 else:
                     settings[group][element] = new_settings[group][element]
     # Now report any elements missing from the new configuration - intended to provide a
     # level of backward capability (able to load old config files into an extended config
     for group in settings:
         if group not in new_settings.keys():
-            logging.warning("LOAD LAYOUT - Missing settings group '"+group+"'")
+            warning_message = ("Missing settings group: '"+group+"' - Asigning default values:")
+            logging.warning("LOAD LAYOUT - "+warning_message)
+            warning_messages.append(warning_message)
+            for element in default_settings[group]:
+                warning_message = ("Missing settings element '"+group+":"+element+
+                    "' - Asigning default value '"+ str(default_settings[group][element])+"'")
+                logging.warning("LOAD LAYOUT - "+warning_message)
+                warning_messages.append(warning_message)
         else:
             for element in settings[group]:
                 if element not in new_settings[group].keys():
-                    logging.warning("LOAD LAYOUT - Missing settings element '"+group+":"+element+"'")
+                    warning_message= ("Missing settings element '"+group+":"+element+
+                        "' - Assigning Default Value '"+ str(default_settings[group][element])+"'")
+                    logging.warning("LOAD LAYOUT - "+warning_message)
+                    warning_messages.append(warning_message)
+    # Report the version of the file the application was generated by if different from the
+    # current version - this gets added to the start of the warning messages
+    if settings["general"]["version"] != default_settings["general"]["version"]:
+        warning_message= ("Layout file generated under Version "+str(settings["general"]["version"]))
+        logging.warning("LOAD LAYOUT - "+warning_message)
+        warning_messages.insert(0, warning_message)
+        warning_message = ("Current application version is "+str(default_settings["general"]["version"]))
+        logging.warning("LOAD LAYOUT - "+warning_message)
+        warning_messages.insert(1, warning_message)
     # We always maintain the current version of the application
     settings["general"]["version"] = default_settings["general"]["version"]
-    return()
+    # Return the list of warning messages (for display to the user)
+    return(warning_messages)
     
 #------------------------------------------------------------------------------------
 # Functions to set/get the general settings
 #------------------------------------------------------------------------------------
 
 def get_general(param=None):
     filename = settings["general"]["filename"]
     editmode = settings["general"]["editmode"]
-    return(filename, editmode)
+    version = settings["general"]["version"]
+    info = settings["general"]["info"]
+    return(filename, editmode, version, info)
 
-def set_general(filename:str=None, editmode:bool=None):
+def set_general(filename:str=None, editmode:bool=None, version:str=None, info:str=None):
     if filename is not None: settings["general"]["filename"] = filename
     if editmode is not None: settings["general"]["editmode"] = editmode
+    if version is not None: settings["general"]["version"] = version
+    if info is not None: settings["general"]["info"] = info
     return()
 
-def get_version():
-    return(default_settings["general"]["version"])
-
 #------------------------------------------------------------------------------------
 # Functions to set/get the canvas settings
 #------------------------------------------------------------------------------------
 
 def get_canvas():
     width = settings["canvas"]["width"]
     height = settings["canvas"]["height"]
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/library/block_instruments.py` & `model-railway-signals-3.4.0/model_railway_signals/library/block_instruments.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,32 +27,44 @@
 #       telegraph_sound_file:str - The filename of the soundfile (in the local package resources)
 #                           to use for the Telegraph key sound (default "telegraph-key-01.wav")
 #       linked_to:int/str - the identifier for the "paired" block instrument - can be specified
 #                           either as an integer (representing the ID of a Block Instrument on the
 #                           the local schematic), or a string representing a Block Instrument 
 #                           running on a remote node - see MQTT networking (default = None)
 # 
-# Note that the Block Instruments feature is primarily intended to provide a prototypical means of
-# communication between signallers working their respective signal boxes. As such, MQTT networking
-# is "built in" - If a remote instrument identifier is specified for the "linked_to" instrument
-# and the MQTT network has been configured then this function will automatically configured the
-# block instrument to publish its state and telegraph key clicks to the remote instrument and
-# will also subscribe to state updates and telegraph clicks from the remote instrument.
+# Note that automatic MQTT networking publish/subscribe on instrument creation is now DEPRECATED.
+# The 'set_instruments_to_publish_state' and 'subscribe_to_instrument_updates' functions should
+# be called to configure networking prior to creating Block Instruments on the local schematic.
+# This is to provide a level of consistency between other MQTT publish/subscribe functions.
 # 
 # block_section_ahead_clear(block_id:int) - Returns the state of the ASSOCIATED block instrument
 #           (i.e. the linked instrument controlling the state of the block section ahead of ours)
 #           This can be used to implement full interlocking of the Starter signal in our section
 #           (i.e. signal locked at danger until the box ahead sets their instrument to LINE-CLEAR)
 #           Returned state is: True = LINE-CLEAR, False = LINE-BLOCKED or TRAIN-ON-LINE
 #
 # If you want to use Block Instruments with full sound enabled (bell rings and telegraph key sounds)
 # then you will also need to install the 'simpleaudio' package. Note that for Windows it has a dependency 
 # on Microsoft Visual C++ 14.0 or greater (so you will need to ensure Visual Studio 2015 is installed first)
 # If 'simpleaudio' is not installed then the software will still function correctly (just without sound)
 #
+# ------------------------------------------------------------------------------------------
+#
+# The following functions are associated with the MQTT networking Feature:
+#
+# subscribe_to_instrument_updates - Subscribe to instrument updates from another node on the network
+#   Mandatory Parameters:
+#       node:str - The name of the node publishing the block instrument update feed
+#       *inst_ids:int - The instruments to subscribe to (multiple Instrument_IDs can be specified)
+#
+# set_instruments_to_publish_state - Enable the publication of state updates for block instruments.
+#                All subsequent changes will be automatically published to remote subscribers
+#   Mandatory Parameters:
+#       *inst_ids:int - The block instruments to publish (multiple Instrument_IDs can be specified)
+#
 # -----------------------------------------------------------------------------------------------
 
 from . import common
 from . import mqtt_interface
 from . import file_interface
 from typing import Union
 import tkinter as Tk
@@ -73,20 +85,20 @@
         import simpleaudio
         return (True)
     except Exception: pass
     return (False)
 audio_enabled = is_simpleaudio_installed()
 
 # -------------------------------------------------------------------------
-# Classes used by external functions when calling the create_point function
+# Classes used by external functions when calling create_instrument
 # -------------------------------------------------------------------------
     
 class instrument_type(enum.Enum):
-    single_line = 1   # Right Hand point
-    double_line = 2   # Left Hand point
+    single_line = 1
+    double_line = 2
 
 class block_callback_type(enum.Enum):
     block_section_ahead_updated = 51   # The instrument has been updated
 
 # --------------------------------------------------------------------------------
 # Block Instruments are to be added to a global dictionary when created
 # --------------------------------------------------------------------------------
@@ -95,14 +107,20 @@
 
 # --------------------------------------------------------------------------------
 # Global variable to indicate whether a Bell Code window is already open or not
 # --------------------------------------------------------------------------------
 
 bell_code_hints_open = False
 
+# --------------------------------------------------------------------------------
+# Global list of block instruments to publish to the MQTT Broker
+# --------------------------------------------------------------------------------
+
+list_of_instruments_to_publish = []
+
 # -------------------------------------------------------------------------
 # The default "External" callback for Block Instruments if one isn't specified
 # -------------------------------------------------------------------------
 
 def null_callback(block_id:int, callback_type):
     return(block_id, callback_type)
 
@@ -157,43 +175,40 @@
             text_entry_box2.config({'disabledbackground':'white'}) 
             text_entry_box2.config({'disabledforeground':'black'}) 
     return()
 
 # --------------------------------------------------------------------------------
 # Internal Function to check if a Block Instrument exists in the list of Instruments
 # Used in most externally-called functions to validate the Block instrument ID
+# Note the function will take in either local or (subscribed to) remote IDs
 # --------------------------------------------------------------------------------
 
-def instrument_exists(block_id:int):
+def instrument_exists(block_id:Union[int,str]):
     return (str(block_id) in instruments.keys() )
 
 # --------------------------------------------------------------------------------
 # Callbacks for handling button push events
 # --------------------------------------------------------------------------------
 
 def occup_button_event (block_id:int):
-    global logging
     logging.info ("Block Instrument "+str(block_id)+": Occup button event ***********************************************")
     set_section_occupied(block_id)
     return()
 
 def clear_button_event (block_id:int):
-    global logging
     logging.info ("Block Instrument "+str(block_id)+": Clear button event ***********************************************")
     set_section_clear(block_id)
     return()
 
 def blocked_button_event (block_id:int):
-    global logging
     logging.info ("Block Instrument "+str(block_id)+": Blocked button event *********************************************")
     set_section_blocked(block_id)
     return()
 
 def telegraph_key_button (block_id:int):
-    global logging
     logging.debug ("Block Instrument "+str(block_id)+": Telegraph key operated ************************************")
     # Provide a visual indication of the key being pressed
     instruments[str(block_id)]["bellbutton"].config(relief="sunken")
     common.root_window.after(10,lambda:instruments[str(block_id)]["bellbutton"].config(relief="raised"))
     # Sound the "clack" of the telegraph key - We put exception handling around this as the function can raise
     # exceptions if you try to play too many sounds simultaneously (if the button is clicked too quickly/frequently)
     if instruments[str(block_id)]["telegraphsound"] is not None:
@@ -209,15 +224,14 @@
 
 # --------------------------------------------------------------------------------
 # Internal Function to receive bell rings from another instrument and
 # sound a bell "ting" on the local instrument (with a visual indication)
 # --------------------------------------------------------------------------------
 
 def ring_section_bell (block_id:int):
-    global logging
     logging.debug ("Block Instrument "+str(block_id)+": Ringing Bell")
     # Provide a visual indication of an incoming bell
     instruments[str(block_id)]["bellbutton"].config(bg="yellow")
     common.root_window.after(100,lambda:instruments[str(block_id)]["bellbutton"].config(bg="black"))
     # Sound the Bell - We put exception handling around this as I've seen this function raise exceptions
     # if you try to play too many sounds simultaneously (if the button is clicked too quickly/frequently)
     if instruments[str(block_id)]["bellsound"] is not None:
@@ -228,15 +242,14 @@
 # --------------------------------------------------------------------------------
 # Function to set the repeater indicator (linked to another block section)
 # to BLOCKED - if its a single line instrument then we set the main indication
 # --------------------------------------------------------------------------------
 
 def set_repeater_blocked (block_id:int,make_callback:bool=True):
     global instruments
-    global logging
     # do some basic validation on the block ID we've been given
     if not instrument_exists(block_id):
         logging.error ("Block Instrument "+str(block_id)+": Can't set repeater to LINE BLOCKED - Block instrument doesn't exist")
     elif instruments[str(block_id)]["singleline"]:
         # If this is a single line instrument then we need to change the main instrument state
         # We need to inhibit the update of the linked instrument in this call to prevent recursion
         set_section_blocked(block_id,update_remote_instrument=False)
@@ -260,15 +273,14 @@
 # --------------------------------------------------------------------------------
 # Function to set the repeater indicator (linked to another block section)
 # to LINE CLEAR - if its a single line instrument then we set the main indication
 # --------------------------------------------------------------------------------
 
 def set_repeater_clear (block_id:int,make_callback:bool=True):
     global instruments
-    global logging
     # do some basic validation on the block ID we've been given
     if not instrument_exists (block_id):
         logging.error ("Block Instrument "+str(block_id)+": Can't set repeater to LINE CLEAR - Block instrument doesn't exist")
     elif instruments[str(block_id)]["singleline"]:
         # If this is a single line instrument then we need to change the main instrument state
         # We need to inhibit the update of the linked instrument in this call to prevent recursion
         set_section_clear(block_id,update_remote_instrument=False)
@@ -292,15 +304,14 @@
 # --------------------------------------------------------------------------------
 # Function to set the repeater indicator (linked to another block section)
 # to OCCUPIED - if its a single line instrument then we set the main indication
 # --------------------------------------------------------------------------------
 
 def set_repeater_occupied (block_id:int,make_callback:bool=True):
     global instruments
-    global logging
     # do some basic validation on the block ID we've been given
     if not instrument_exists (block_id):
         logging.error ("Block Instrument "+str(block_id)+": Can't set repeater to TRAIN ON LINE - Block instrument doesn't exist")
     elif instruments[str(block_id)]["singleline"]:
         # If this is a single line instrument then we need to change the main instrument state
         # We need to inhibit the update of the linked instrument in this call to prevent recursion
         set_section_occupied(block_id,update_remote_instrument=False)
@@ -326,15 +337,14 @@
 # called when the "BLOCKED" button is clicked on the local block instrument
 # Also called for single-line block instruments (without a repeater display)
 # following a state change of the linked remote block instrument
 # --------------------------------------------------------------------------------
 
 def set_section_blocked (block_id:int,update_remote_instrument:bool=True):
     global instruments
-    global logging
     # do some basic validation on the block ID we've been given
     if not instrument_exists (block_id):
         logging.error ("Block Instrument "+str(block_id)+": Can't set section to LINE BLOCKED - Block instrument doesn't exist")
     else:
         # Set the state of the buttons accordingly. We always do this (even if the state hasn't changed)
         # to deal with single line instruments being updated by a state change of the linked instrument
         instruments[str(block_id)]["blockbutton"].config(relief="sunken")
@@ -372,15 +382,14 @@
 # called when the "CLEAR" button is clicked on the local block instrument
 # Also called for single-line block instruments (without a repeater display)
 # following a state change of the linked remote block instrument
 # --------------------------------------------------------------------------------
 
 def set_section_clear (block_id:int,update_remote_instrument:bool=True):
     global instruments
-    global logging
     # do some basic validation on the block ID we've been given
     if not instrument_exists (block_id):
         logging.error ("Block Instrument "+str(block_id)+": Can't set section to LINE CLEAR - Block instrument doesn't exist")
     else:
         # Set the state of the buttons accordingly. We always do this (even if the state hasn't changed)
         # to deal with single line instruments being updated by a state change of the linked instrument
         instruments[str(block_id)]["blockbutton"].config(relief="raised")
@@ -418,15 +427,14 @@
 # called when the "OCCUP" button is clicked on the local block instrument
 # Also called for single-line block instruments (without a repeater display)
 # following a state change of the linked remote block instrument
 # --------------------------------------------------------------------------------
 
 def set_section_occupied (block_id:int,update_remote_instrument:bool=True):
     global instruments
-    global logging
     # do some basic validation on the block ID we've been given
     if not instrument_exists (block_id):
         logging.error ("Block Instrument "+str(block_id)+": Can't set section to TRAIN ON LINE - Block instrument doesn't exist")
     else:
         # Set the state of the buttons accordingly. We always do this (even if the state hasn't changed)
         # to deal with single line instruments being updated by a state change of the linked instrument
         instruments[str(block_id)]["blockbutton"].config(relief="raised")
@@ -483,25 +491,27 @@
 
 def load_audio_file(audio_filename):
     audio_object = None
     if os.path.split(audio_filename)[1] == audio_filename:
         try:
             with importlib.resources.path ('model_railway_signals.library.resources',audio_filename) as audio_file:
                 audio_object = simpleaudio.WaveObject.from_wave_file(str(audio_file))
-        except:
+        except Exception as exception:
             Tk.messagebox.showerror(parent=common.root_window, title="Load Error",
                             message="Error loading audio resource file '"+str(audio_filename)+"'")
-            logging.error ("Block Instruments - Error loading audio resource file '"+str(audio_filename)+"'")       
+            logging.error ("Block Instruments - Error loading audio resource file '"+str(audio_filename)+"'"+
+                           " \nReported Exception: "+str(exception))       
     else:        
         try:
             audio_object = simpleaudio.WaveObject.from_wave_file(str(audio_filename))
-        except:
+        except Exception as exception:
             Tk.messagebox.showerror(parent=common.root_window, title="Load Error",
                             message="Error loading audio file '"+str(audio_filename)+"'")
-            logging.error ("Block Instruments - Error loading audio file '"+str(audio_filename)+"'")       
+            logging.error ("Block Instruments - Error loading audio file '"+str(audio_filename)+"'"+
+                           " \nReported Exception: "+str(exception))       
     return(audio_object)
 
 # --------------------------------------------------------------------------------
 # Public API function to create a Block  Instrument (drawing objects and internal state)
 # --------------------------------------------------------------------------------
 
 def create_block_instrument (canvas,
@@ -510,16 +520,15 @@
                              inst_type:instrument_type = instrument_type.double_line,
                              block_callback = null_callback,
                              single_line:bool = False, ############################################################
                              bell_sound_file:str = "bell-ring-01.wav",
                              telegraph_sound_file:str = "telegraph-key-01.wav",
                              linked_to:Union[int,str] = None):
     global instruments
-    global audio_enabled
-    global logging
+    global list_of_instruments_to_publish
     logging.info ("Block Instrument "+str(block_id)+": Creating Block Instrument")
     # Find and store the root window (when the first block instrument is created)
     if common.root_window is None: common.find_root_window(canvas)
     # Establish whether the ID is a local or remote ID and set the type accordingly
     # We need to do this for the editor as the editor will give us an int as a string
     if linked_to is None or linked_to == "":
         linked_to_id = None
@@ -528,19 +537,20 @@
         except: linked_to_id = str(linked_to)
     # Do some basic validation on the parameters we have been given
     if instrument_exists(block_id):
         logging.error ("Block Instrument "+str(block_id)+": Instrument already exists")
     elif block_id < 1:
         logging.error ("Block Instrument "+str(block_id)+": Block ID must be greater than zero")
     elif linked_to_id == block_id:
-        logging.error ("Block Instrument "+str(block_id)+": ID for linked instrument is the same as the instrument to create")   
+        logging.error ("Block Instrument "+str(block_id)+": ID for linked instrument is the same as the instrument to create")
     elif isinstance(linked_to_id,str) and mqtt_interface.split_remote_item_identifier(linked_to_id) is None:
-        logging.error ("Block Instrument "+str(block_id)+": Compound ID for remote-node instrument is invalid")   
+        logging.error ("Block Instrument "+str(block_id)+": Compound ID for remote-node instrument is invalid")
     else:
         ####################################################################################################################
+        # DEPRECATED code to remove at a future release ####################################################################
         if single_line:
             logging.warning ("###########################################################################################")
             logging.warning ("Block Instrument "+str(block_id)+": single_line flag is DEPRECATED - use inst_type")
             logging.warning ("###########################################################################################")
         else:
             single_line = (inst_type == instrument_type.single_line)
         ####################################################################################################################
@@ -615,118 +625,194 @@
         elif loaded_state["sectionstate"] == False: set_section_occupied(block_id,update_remote_instrument=False)
         else: set_section_blocked(block_id,update_remote_instrument=False)
         # Only set the initial repeater state if this instrument has a repeater (i.e. not single line)
         if not instruments[str(block_id)]["singleline"]:
             if loaded_state["repeaterstate"] == True: set_repeater_clear(block_id,make_callback=False)
             elif loaded_state["repeaterstate"] == False: set_repeater_occupied(block_id,make_callback=False)
             else: set_repeater_blocked(block_id,make_callback=False)
+
+        ####################################################################################################################
+        # DEPRECATED code to remove at a future release ####################################################################
         # If the associated block instrument is associated with an external node (i.e. has a string-type
         # compound identifier rather than an integer) then subscribe to updates from the remote node and
         # publish the initial state of the local instrument (to be picked up by the remote node). State
         # will only be published if the MQTT interface has been configured and we are connected to the broker
-        if isinstance(linked_to_id,str):
-            subscribe_to_remote_instrument(linked_to_id)
-            send_mqtt_instrument_updated_event(block_id)
+        # Note that this function is DEPRECATED - you should always 'subscribe' to remote instruments beforehand
+        if isinstance(linked_to_id,str) and not instrument_exists(linked_to_id):
+            remote_node,remote_id = mqtt_interface.split_remote_item_identifier(linked_to_id)
+            mqtt_interface.subscribe_to_mqtt_messages("instrument_updated_event",remote_node,
+                                            remote_id,handle_mqtt_instrument_updated_event)
+            mqtt_interface.subscribe_to_mqtt_messages("instrument_telegraph_event",remote_node,
+                                            remote_id,handle_mqtt_ring_section_bell_event)
+            list_of_instruments_to_publish.append(block_id)
+            logging.warning ("###########################################################################################")
+            logging.warning ("Block Instrument "+str(block_id)+": Auto publish and subscribe is DEPRECATED - call the")
+            logging.warning ("'subscribe_to_instrument_updates'and 'set_instruments_to_publish_state' functions to")
+            logging.warning ("configure networking before creating the block instruments on the local schematic")
+            logging.warning ("###########################################################################################")
+        ####################################################################################################################
+
+        # Publish the initial state to the broker (for other nodes to consume). Note that changes will
+        # only be published if the MQTT interface has been configured for publishing updates for this
+        # instrument. This allows publish/subscribe to be configured prior to instrument creation
+        send_mqtt_instrument_updated_event(block_id)
     return ()
 
+#-----------------------------------------------------------------------------------------------
+# Public API Function to configure instruments to publish state changes to remote MQTT nodes
+# (i.e. effectively publish state changes to the local SECTION indicator)
+# Note that this function should be called BEFORE creating block instruments
+#-----------------------------------------------------------------------------------------------
+
+def set_instruments_to_publish_state(*inst_ids:int):
+    global list_of_instruments_to_publish
+    for inst_id in inst_ids:
+        logging.info("MQTT-Client: Configuring instrument "+str(inst_id)+" to publish state changes via MQTT broker")
+        if inst_id in list_of_instruments_to_publish:
+            logging.warning("MQTT-Client: Instrument "+str(inst_id)+" - is already configured to publish state changes")
+        else:
+            list_of_instruments_to_publish.append(inst_id)
+            # Publish the initial state now this has been added to the list of instruments to publish
+            # This allows the publish/subscribe functions to be configured after instrument creation
+            if str(inst_id) in instruments.keys(): send_mqtt_instrument_updated_event(inst_id)
+    return()
+
+#-----------------------------------------------------------------------------------------------
+# Public API Function to "subscribe" to instrument updates published by remote MQTT "Node"
+# Note that no callback is specified in the function call - the default internal one is used
+# to set the repeater display on the local instrument (to mirror the remote instrument)
+#-----------------------------------------------------------------------------------------------
+
+def subscribe_to_instrument_updates (node:str,*inst_ids:int):
+    global instruments
+    for inst_id in inst_ids:
+        instrument_identifier = mqtt_interface.create_remote_item_identifier(inst_id,node)
+        if not instrument_exists(instrument_identifier):
+            # Create a dummy instrument object to enable 'instrument_exists' validation checks
+            # Note that this does not hold state - as state is reflected on the local repeater indicator
+            # The Identifier for a remote instrument is a string combining the the Node-ID and Section-ID
+            instruments[instrument_identifier] = {}
+            # Subscribe to updates from the remote block instrument
+            mqtt_interface.subscribe_to_mqtt_messages("instrument_updated_event",node,
+                                    inst_id,handle_mqtt_instrument_updated_event)
+            mqtt_interface.subscribe_to_mqtt_messages("instrument_telegraph_event",node,
+                                    inst_id,handle_mqtt_ring_section_bell_event)
+    return()
+
 # --------------------------------------------------------------------------------
 # Public API function to find out if the block section ahead is clear.
 # This is represented by the current status of the REPEATER Indicator
 # --------------------------------------------------------------------------------
 
 def block_section_ahead_clear(block_id:int):
-    global logging
     # do some basic validation on the block ID we've been given
     if not instrument_exists (block_id):
         logging.error ("Block Instrument "+str(block_id)+": block_section_ahead_clear - Block instrument doesn't exist")
         section_ahead_clear = False
     elif instruments[str(block_id)]["repeaterstate"] == True:
         section_ahead_clear = True
     else:
         section_ahead_clear = False
     return(section_ahead_clear)
 
 # --------------------------------------------------------------------------------
-# Internal function to subscribe to the required MQTT messages from a remote instrument
-# --------------------------------------------------------------------------------
-
-def subscribe_to_remote_instrument(block_identifier:str):
-    remote_node,remote_id = mqtt_interface.split_remote_item_identifier(block_identifier) 
-    mqtt_interface.subscribe_to_mqtt_messages("instrument_updated_event",remote_node,
-                                            remote_id,handle_mqtt_instrument_updated_event)   
-    mqtt_interface.subscribe_to_mqtt_messages("instrument_telegraph_event",remote_node,
-                                            remote_id,handle_mqtt_ring_section_bell_event)  
-    return()
-
-# --------------------------------------------------------------------------------
 # Callbacks for handling received MQTT messages (from a remote Instrument)
 # --------------------------------------------------------------------------------
 
 def handle_mqtt_instrument_updated_event(message):
-    global logging
     if "instrumentid" in message.keys() and "sectionstate" in message.keys():
         block_identifier = message["instrumentid"]
         section_state = message["sectionstate"]
         node_id, block_id = mqtt_interface.split_remote_item_identifier(block_identifier)
         logging.info("Block Instrument "+str(block_id)+": State update from remote instrument ********************")
         if section_state == True: set_repeater_clear(block_id)
         elif section_state == False: set_repeater_occupied(block_id)
         else: set_repeater_blocked(block_id)
     return()
 
 def handle_mqtt_ring_section_bell_event(message):
-    global logging
     if "instrumentid" in message.keys():
         block_identifier = message["instrumentid"]
         node_id, block_id = mqtt_interface.split_remote_item_identifier(block_identifier)
         logging.debug("Block Instrument "+str(block_id)+": Telegraph key event from remote instrument ************")
         ring_section_bell(block_id)
     return()
 
 # --------------------------------------------------------------------------------
 # Internal functions for building and publishing MQTT messages (to a remote instrument)
 # --------------------------------------------------------------------------------
 
 def send_mqtt_instrument_updated_event(block_id:int):
-    data = {}
-    data["instrumentid"] = instruments[str(block_id)]["linkedto"]
-    data["sectionstate"] = instruments[str(block_id)]["sectionstate"]
-    log_message = "Block Instrument "+str(block_id)+": Publishing instrument state to MQTT Broker"
-    # Publish as "retained" messages so remote items that subscribe later will always pick up the latest state
-    mqtt_interface.send_mqtt_message("instrument_updated_event",block_id,data=data,log_message=log_message,retain=True)
+    if block_id in list_of_instruments_to_publish:
+        data = {}
+        data["instrumentid"] = instruments[str(block_id)]["linkedto"]
+        data["sectionstate"] = instruments[str(block_id)]["sectionstate"]
+        log_message = "Block Instrument "+str(block_id)+": Publishing instrument state to MQTT Broker"
+        # Publish as "retained" messages so remote items that subscribe later will always pick up the latest state
+        mqtt_interface.send_mqtt_message("instrument_updated_event",block_id,data=data,log_message=log_message,retain=True)
     return()
 
 def send_mqtt_ring_section_bell_event(block_id:int):
-    data = {}
-    data["instrumentid"] = instruments[str(block_id)]["linkedto"]
-    log_message = "Block Instrument "+str(block_id)+": Publishing telegraph key event to MQTT Broker"
-    # These are transitory events so we do not publish as "retained" messages (if they get missed, they get missed)
-    mqtt_interface.send_mqtt_message("instrument_telegraph_event",block_id,data=data,log_message=log_message,retain=False)
+    if block_id in list_of_instruments_to_publish:
+        data = {}
+        data["instrumentid"] = instruments[str(block_id)]["linkedto"]
+        log_message = "Block Instrument "+str(block_id)+": Publishing telegraph key event to MQTT Broker"
+        # These are transitory events so we do not publish as "retained" messages (if they get missed, they get missed)
+        mqtt_interface.send_mqtt_message("instrument_telegraph_event",block_id,data=data,log_message=log_message,retain=False)
     return()
 
 # ------------------------------------------------------------------------------------------
 # Non public API function for deleting an instrument object (including all the drawing objects)
 # This is used by the schematic editor for changing instrument types where we delete the existing
 # instrument with all its data and then recreate it (with the same ID) in its new configuration
 # ------------------------------------------------------------------------------------------
 
 def delete_instrument(block_id:int):
+    global instruments
+    global list_of_instruments_to_publish
     if instrument_exists(block_id):
         # Delete all the tkinter canvas drawing objects associated with the signal
         instruments[str(block_id)]["canvas"].delete("instrument"+str(block_id))
         # Delete all the tkinter button objects created for the signal
         instruments[str(block_id)]["blockbutton"].destroy()
         instruments[str(block_id)]["clearbutton"].destroy()
         instruments[str(block_id)]["occupbutton"].destroy()
         instruments[str(block_id)]["bellbutton"].destroy()
+        # Delete the instrument from the list_of_instruments_to_publish (if required)
+        if block_id in list_of_instruments_to_publish:
+            list_of_instruments_to_publish.remove(block_id)
         # Finally, delete the entry from the dictionary of instruments
         del instruments[str(block_id)]
     return()
 
 # ------------------------------------------------------------------------------------------
 # Non public API function to return the tkinter canvas 'tags' for the block instrument
 # ------------------------------------------------------------------------------------------
 
 def get_tags(block_id:int):
     return("instrument"+str(block_id))
 
+# ------------------------------------------------------------------------------------------
+# Non public API function to reset the list of published/subscribed instruments. Used
+# by the schematic editor for re-setting the MQTT configuration prior to re-configuring
+# via the subscribe_to_instrument_updates and subscribe_to_instrument_updates functions
+# ------------------------------------------------------------------------------------------
+
+def reset_mqtt_configuration():
+    global instruments
+    global list_of_instruments_to_publish
+    # We only need to clear the list to stop any further instrument events being published
+    list_of_instruments_to_publish.clear()
+    # For subscriptions we unsubscribe from all topics associated with the message_type
+    mqtt_interface.unsubscribe_from_message_type("instrument_updated_event")
+    mqtt_interface.unsubscribe_from_message_type("instrument_telegraph_event")
+    # Finally remove all "remote" instruments from the dictionary of instruments - these
+    # will be re-created if they are subsequently re-subscribed to. Note we don't iterate
+    # through the dictionary of instruments to remove items as it will change under us
+    new_instruments = {}
+    for key in instruments:
+        if mqtt_interface.split_remote_item_identifier(key) is not None:
+            new_instruments[key] = instruments[key]
+    instruments = new_instruments
+    return()
+
 ###############################################################################
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/library/common.py` & `model-railway-signals-3.4.0/model_railway_signals/library/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,17 +36,15 @@
 # Function to catch the root window close event so we can perform an
 # orderly shutdown of the other threads running in the application
 # The shutdown_initiated flag is used to tell the flash aspects and timed
 # signals functions to stop scheduling further "after" commands and exit 
 #-------------------------------------------------------------------------
 
 def on_closing(ask_to_save_state=True):
-    global logging
     global shutdown_initiated
-    global root_window
     if ask_to_save_state: confirm_quit = file_interface.save_state_and_quit()
     else: confirm_quit = True 
     if confirm_quit:       
         logging.info ("Initiating Application Shutdown")
         shutdown_initiated = True
         # Clear out any retained messages and disconnect from broker
         mqtt_interface.mqtt_shutdown()
@@ -108,15 +106,14 @@
        callback = event_queue.get(False)
     except event_queue.Empty:
         return()
     callback()
     return()
     
 def execute_function_in_tkinter_thread(callback_function):
-    global logging
     event_queue.put(callback_function)
     if root_window is not None:
         root_window.event_generate("<<ExtCallback>>", when="tail")
     else:
         logging.error ("execute_function_in_tkinter_thread - cannot execute callback function as root window is undefined")
     return()
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/library/dcc_control.py` & `model-railway-signals-3.4.0/model_railway_signals/library/dcc_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,17 +223,14 @@
                     LH2 = [[0,False],],
                     RH1 = [[0,False],],
                     RH2 = [[0,False],],
                     MAIN = [[0,False],],
                     NONE = [[0,False],],
                     THEATRE = [["#", [[0,False],]],],
                     subsidary:int=0):
-    
-    global logging
-    
     # Do some basic validation on the parameters we have been given
     logging.info ("Signal "+str(sig_id)+": Creating DCC Address mapping for a colour light signal")
     if sig_mapped(sig_id):
         logging.error ("Signal "+str(sig_id)+": Signal already has a DCC Address mapping")
     elif sig_id < 1:
         logging.error ("Signal "+str(sig_id)+": Signal ID for DCC Mapping must be greater than zero")
     else:
@@ -268,28 +265,26 @@
                 str(signals_common.route_type.LH1) : LH1,                                          # Specific to Colour_Light Mappings
                 str(signals_common.route_type.LH2) : LH2,                                          # Specific to Colour_Light Mappings
                 str(signals_common.route_type.RH1) : RH1,                                          # Specific to Colour_Light Mappings
                 str(signals_common.route_type.RH2) : RH2,                                          # Specific to Colour_Light Mappings
                 str(signals_common.route_type.MAIN) : MAIN,                                        # Specific to Colour_Light Mappings
                 str(signals_common.route_type.NONE) : NONE }                                       # Specific to Colour_Light Mappings
             dcc_signal_mappings[str(sig_id)] = new_dcc_mapping
-        
     return ()
 
 #-----------------------------------------------------------------------------------------
 # Function to "map" a TrainTech" Event-driven signal to the appropriate DCC addresses/commands
 # This function provided to simplify the calling code - i.e. this does all the hard work for you
 #-----------------------------------------------------------------------------------------
 
 def map_traintech_signal (sig_id:int,
                           base_address:int,
                           route_address:int = 0,
                           theatre_route = "NONE",
                           feather_route = signals_common.route_type.NONE):
-
     # Do some basic validation on the parameters we have been given
     logging.info ("Signal "+str(sig_id)+": Creating DCC Address mapping for a Train Tech Signal")
     if sig_mapped(sig_id):
         logging.error ("Signal "+str(sig_id)+": Signal already has a DCC Address mapping")
     elif sig_id < 1:
         logging.error ("Signal "+str(sig_id)+": Signal ID for DCC Mapping must be greater than zero")
     elif base_address < 0 or base_address > 2047:
@@ -320,21 +315,18 @@
                 str(signals_common.signal_state_type.FLASH_PRELIM_CAUTION) : [[base_address+3,False]], # Specific to Colour_Light Mappings
                 str(signals_common.route_type.LH1) : [[route_address,False]],                          # Specific to Colour_Light Mappings
                 str(signals_common.route_type.LH2) : [[route_address,False]],                          # Specific to Colour_Light Mappingss
                 str(signals_common.route_type.RH1) : [[route_address,False]],                          # Specific to Colour_Light Mappings
                 str(signals_common.route_type.RH2) : [[route_address,False]],                          # Specific to Colour_Light Mappingss
                 str(signals_common.route_type.MAIN) : [[route_address,False]],                         # Specific to Colour_Light Mappings 
                 str(signals_common.route_type.NONE) : [[route_address,False]] }                        # Specific to Colour_Light Mappings
-        
         # Configure the DCC Command  for the feather route indicator that we want to configured
         new_dcc_mapping[str(feather_route)] = [[route_address,True]]
-        
         # Finally save the DCC mapping into the dictionary of mappings 
         dcc_signal_mappings[str(sig_id)] = new_dcc_mapping
-        
     return ()
 
 #-----------------------------------------------------------------------------------------
 # Function to "map" a semaphore signal to the appropriate DCC addresses/commands using
 # a simple one-to-one mapping of each signal arm with a DCC accessory address apart from
 # the theatre route display where we send can send either a signle DCC command or a
 # series of DCC commands to put the theatre route indicator into the correct state
@@ -356,15 +348,14 @@
                           rh2_signal:int = 0,
                           main_subsidary:int = 0,
                           lh1_subsidary:int = 0,
                           lh2_subsidary:int = 0,
                           rh1_subsidary:int = 0,
                           rh2_subsidary:int = 0,
                           THEATRE = [["#", [[0,False],]],]):
-
     # Do some basic validation on the parameters we have been given
     logging.info ("Signal "+str(sig_id)+": Creating DCC Address mapping for a Semaphore Signal")
     if sig_mapped(sig_id):
         logging.error ("Signal "+str(sig_id)+": Signal already has a DCC Address mapping")
     elif sig_id < 1:
         logging.error ("Signal "+str(sig_id)+": Signal ID for DCC Mapping must be greater than zero")
     else: 
@@ -374,15 +365,14 @@
             for dcc_address in theatre_state[1]:
                 addresses = addresses + [dcc_address[0]]
         addresses_valid = True
         for entry in addresses:
             if entry < 0 or entry > 2047:
                 logging.error ("Signal "+str(sig_id)+": Invalid DCC Address "+str(entry)+" - must be between 1 and 2047")
                 addresses_valid = False
-        
         if addresses_valid:
             # Create the DCC Mapping entry for the signal.
             new_dcc_mapping = {
                 "mapping_type" : mapping_type.SEMAPHORE,     # Common to Colour_Light & Semaphore Mappings
                 "auto_route_inhibit" : False,                # Common to Colour_Light & Semaphore Mappings
                 "main_subsidary" :  main_subsidary,          # Common to Colour_Light & Semaphore Mappings 
                 "THEATRE"       : THEATRE,                   # Common to Colour_Light & Semaphore Mappings                                      str(signals_common.signal_state_type.DANGER)         :       [[0,False],],     # Specific to Colour Light Signal Mappings
@@ -392,52 +382,44 @@
                 "lh2_signal"    : lh2_signal,                # Specific to Semaphore Signal Mappings
                 "lh2_subsidary" : lh2_subsidary,             # Specific to Semaphore Signal Mappings
                 "rh1_signal"    : rh1_signal,                # Specific to Semaphore Signal Mappings
                 "rh1_subsidary" : rh1_subsidary,             # Common to both Semaphore and Colour Lights
                 "rh2_signal"    : rh2_signal,                # Specific to Semaphore Signal Mappings
                 "rh2_subsidary" : rh2_subsidary }            # Finally save the DCC mapping into the dictionary of mappings 
             dcc_signal_mappings[str(sig_id)] = new_dcc_mapping
-
     return ()
 
 #-----------------------------------------------------------------------------------------
 # Externally called unction to "map" a particular point object to a DCC address/command
 # This is much simpler than the signals as we only need to map a signle DCC address for
 # each point to be controlled - with an appropriate state (either switched or not_switched)
 #-----------------------------------------------------------------------------------------
 
 def map_dcc_point (point_id:int, address:int, state_reversed:bool = False):
-    
-    global logging
-    
     logging.info ("Point "+str(point_id)+": Creating DCC Address mapping")
     # Do some basic validation on the parameters we have been given
     if point_mapped(point_id):
         logging.error ("Point "+str(point_id)+": Point already has a DCC Address mapping")
     elif point_id < 1:
         logging.error ("Point "+str(point_id)+": Point ID for DCC Mapping must be greater than zero")
     elif (address < 1 or address > 2047):
         logging.error ("Point "+str(point_id)+": Invalid DCC Address "+str(address)+" - must be between 1 and 2047")
     else:
         # Create the DCC Mapping entry for the point
         new_dcc_mapping = {
             "address"  : address,
             "reversed" : state_reversed }
         dcc_point_mappings[str(point_id)] = new_dcc_mapping
-        
     return ()
 
 #-----------------------------------------------------------------------------------------
 # Function to send the appropriate DCC command to set the state of a DCC Point
 #------------------------------------------------------------------------------------------
 
-def update_dcc_point(point_id:int, state:bool):
-    
-    global logging
-    
+def update_dcc_point(point_id:int, state:bool):    
     if point_mapped(point_id):
         logging.debug ("Point "+str(point_id)+": Generating DCC Bus commands to switch point")
         # Retrieve the DCC mappings for our point
         dcc_mapping = dcc_point_mappings[str(point_id)]
         if dcc_mapping["reversed"]: state = not state
         if dcc_mapping["address"] > 0:
             # Send the DCC commands to change the state
@@ -445,17 +427,14 @@
     return ()
 
 #-----------------------------------------------------------------------------------------
 # Function to send the appropriate DCC commands to set the state of a DCC Signal
 #------------------------------------------------------------------------------------------
 
 def update_dcc_signal_aspects(sig_id: int):
-    
-    global logging
-    
     if sig_mapped(sig_id):
         # Retrieve the DCC mappings for our signal and validate its the correct mapping
         # This function should only be called for Colour Light Signal Types
         dcc_mapping = dcc_signal_mappings[str(sig_id)]
         if dcc_mapping["mapping_type"] != mapping_type.COLOUR_LIGHT:
             logging.error ("Signal "+str(sig_id)+": Incorrect DCC Mapping Type for signal - Expecting a Colour Light signal")
         else:
@@ -475,18 +454,15 @@
 #-----------------------------------------------------------------------------------------
 # Function to send the appropriate DCC commands to change a single element of a signal
 # This function primarily used for semaphore signals where each signal "arm" is normally
 # mapped to a single DCC address. Also used for the subsidary aspect of main colour light
 # signals where this subsidary aspect is normally mapped to a single DCC Address
 #------------------------------------------------------------------------------------------
             
-def update_dcc_signal_element (sig_id:int,state:bool, element:str="main_subsidary"):
-        
-    global logging
-    
+def update_dcc_signal_element (sig_id:int,state:bool, element:str="main_subsidary"):    
     if sig_mapped(sig_id):
         # Retrieve the DCC mappings for our signal and validate its the correct mapping
         # This function should only be called for anything other than the "main_subsidary" for Semaphore Signal Types
         dcc_mapping = dcc_signal_mappings[str(sig_id)]
         if element != "main_subsidary" and dcc_mapping["mapping_type"] != mapping_type.SEMAPHORE:
             logging.error ("Signal "+str(sig_id)+": Incorrect DCC Mapping Type for signal - Expecting a Semaphore signal")
         else:
@@ -511,16 +487,14 @@
 # For signals that don't do this, we need to send out commands every time we need to change
 # the route display - i.e. on all Signal Changes (to/from DANGER) to enable/disable the
 # display, and for all ROUTE changes when the signal is not at DANGER
 #------------------------------------------------------------------------------------------
             
 def update_dcc_signal_route (sig_id:int,route:signals_common.route_type,
                               signal_change:bool=False,sig_at_danger:bool=False):
-    global logging
-    
     if sig_mapped(sig_id):
         # Retrieve the DCC mappings for our signal and validate its the correct mapping
         # This function should only be called for Colour Light Signal Types
         dcc_mapping = dcc_signal_mappings[str(sig_id)]
         if dcc_mapping["mapping_type"] != mapping_type.COLOUR_LIGHT:
             logging.error ("Signal "+str(sig_id)+": Incorrect DCC Mapping Type for signal - Expecting a Colour Light signal")
         else:
@@ -552,17 +526,15 @@
 # to/from DANGER - In this case we only need to command it when the ROUTE has been changed.
 # For signals that don't do this, we need to send out commands every time we need to change
 # the route display - i.e. on all Signal Changes (to/from DANGER) to enable/disable the
 # display, and for all ROUTE changes when the signal is not at DANGER
 #------------------------------------------------------------------------------------------
             
 def update_dcc_signal_theatre (sig_id:int, character_to_display, 
-                               signal_change:bool=False,sig_at_danger:bool=False):
-    global logging
-    
+                               signal_change:bool=False,sig_at_danger:bool=False):    
     if sig_mapped(sig_id):
         # Retrieve the DCC mappings for our signal. We don't need to validate the mapping type
         # as Theatre route displays are supported by both Colour Light and Semaphore signal types 
         dcc_mapping = dcc_signal_mappings[str(sig_id)]       
         # Only send commands to enable/disable route if we need to:
         # All signals - Any route change when the signal is not at DANGER
         # Auto inhibit signals - additionally route changes when signal is at DANGER
@@ -582,15 +554,15 @@
                             # Publish the DCC commands to a remote pi-sprog "node" via an external MQTT broker.
                             # Note that the commands will only be published if networking is configured and
                             # the node this software is running on is not configured as a "pi-sprog" node
                             publish_accessory_short_event(command[0],command[1])       
     return()
 
 #-----------------------------------------------------------------------------------------------
-# Public API Function to "subscribe" to the published DCC commands from another "Node"
+# Public API Function to set this node to publish all DCC commands to the broker
 #-----------------------------------------------------------------------------------------------
 
 def set_node_to_publish_dcc_commands (publish_dcc_commands:bool=False):
     global publish_dcc_commands_to_mqtt_broker
     if publish_dcc_commands: logging.info("MQTT-Client - Configuring Application to publish DCC Commands to MQTT broker")
     else: logging.info("DCC Control - Configuring Application NOT to publish DCC Commands to MQTT broker")
     publish_dcc_commands_to_mqtt_broker = publish_dcc_commands
@@ -609,15 +581,14 @@
     return() 
 
 #-----------------------------------------------------------------------------------------------
 # Callback for handling received MQTT messages from a remote DCC-command-producer Node
 #-----------------------------------------------------------------------------------------------
 
 def handle_mqtt_dcc_accessory_short_event (message):    
-    global logging
     if "sourceidentifier" in message.keys() and "dccaddress" in message.keys() and "dccstate" in message.keys():
         source_node = message["sourceidentifier"]
         dcc_address = message["dccaddress"]
         dcc_state = message["dccstate"]
         if dcc_state: 
             logging.debug ("DCC Control: Received ASON command from \'"+source_node+"\' for DCC address: "+str(dcc_address))
         else:
@@ -639,30 +610,39 @@
         if active: log_message = "DCC Control: Publishing DCC command ASON with DCC address: "+str(address)+" to MQTT broker"
         else: log_message = "DCC Control: Publishing DCC command ASOF with DCC address: "+str(address)+" to MQTT broker"
         # Publish as "retained" messages so remote nodes that subscribe later will always pick up the latest state
         mqtt_interface.send_mqtt_message("dcc_accessory_short_events",0,data=data,
                             log_message=log_message,subtopic = str(address),retain=True)
     return()
 
+# ------------------------------------------------------------------------------------------
+# Non public API function to reset the list of subscribed Topics. Used by the schematic editor
+# for re-setting the MQTT configuration prior to re-configuring
+# ------------------------------------------------------------------------------------------
+
+def reset_mqtt_configuration():
+    global publish_dcc_commands_to_mqtt_broker
+    publish_dcc_commands_to_mqtt_broker = False
+    mqtt_interface.unsubscribe_from_message_type("dcc_accessory_short_events")
+    return()
+
 # --------------------------------------------------------------------------------
 # Non public API function for deleting a point mapping - This is used by the
 # schematic editor for deleting existing DCC mappings (before creating new ones)
 # --------------------------------------------------------------------------------
 
 def delete_point_mapping(point_id:int):
-    global points
     if point_mapped(point_id):
         del dcc_point_mappings[str(point_id)]
     return()
 
 # --------------------------------------------------------------------------------
 # Non public API function for deleting a signal mapping - This is used by the
 # schematic editor for deleting existing DCC mappings (before creating new ones)
 # --------------------------------------------------------------------------------
 
 def delete_signal_mapping(sig_id:int):
-    global points
     if sig_mapped(sig_id):
         del dcc_signal_mappings[str(sig_id)]
     return()
 
 #######################################################################################
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/library/file_interface.py` & `model-railway-signals-3.4.0/model_railway_signals/library/file_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import logging
 import tkinter.messagebox
 import tkinter.filedialog
 from . import signals_common
 from . import track_sections
 from . import block_instruments
 from . import points
+from . import common
 
 #-------------------------------------------------------------------------------------------------
 # Global variables to define what options are presented to the user on application quit
 #-------------------------------------------------------------------------------------------------
 
 filename_used_for_save = None
 filename_used_for_load = None
@@ -78,27 +79,27 @@
 # Returns the filename_used_for_load if the file was successfully loaded
 #-------------------------------------------------------------------------------------------------
 
 def load_layout_state(file_name:str=None,
                       load_file_dialog:bool=False,
                       save_file_dialog:bool=False,
                       ask_to_load_state:bool=True):
-    global logging
     global filename_used_for_load
     global save_as_option_enabled
     global layout_state
     # Get the name of the main python script as a string
     script_name = (__main__.__file__)
     default_file_name = script_name.rsplit('.',1)[0]+'.sig'
     # If the 'save_file_dialog' option has been specified then we save this to a global variable
     # to trigger the save file dialogue on quit of the application
     save_as_option_enabled = save_file_dialog
     # We always prompt for load state on startup unless this is inhibited
     if ask_to_load_state:
-        load_state = tkinter.messagebox.askokcancel("Load State","Do you want to load the last layout state?")
+        load_state = tkinter.messagebox.askokcancel(parent=common.root_window,
+                title="Load State", message="Do you want to load the last layout state?")
     else:
         load_state = True
     if not load_state:
         # if the user clicks on 'Cancel' then we still want to provide an option to save the layout
         # state on application quit - either using the filename passed to us or the default filename
         # derived from the name of the main python script (with a '.sig' extension)
         if file_name is not None: filename_used_for_load = file_name
@@ -127,38 +128,40 @@
         elif file_name is not None: filename = file_name
         # Fall back to a filename derived from the name of the main python script (with a '.sig' extension)
         else: filename = default_file_name
         # if the user clicks on 'Cancel' in the load file dialog then we still want to provide an option
         # to save the layout state on application quit - either using the filename passed to us or the
         # default filename derived from the name of the main python script (with a '.sig' extension)
         if filename is None:
-            logging.info("Load File - No file selected - Layout will be created in its default state")
+            logging.info("Load File - No file selected - Layout will remain in its default state")
             if file_name: filename_used_for_load = file_name
             else: filename_used_for_load = default_file_name
         else:
             # We have a valid filename so can proceed to try and open the file
-            logging.info("Load File - Loading layout state information from '"+filename+"'")
+            logging.info("Load File - Loading layout configuration from '"+filename+"'")
             try:
                 with open (filename,'r') as file:
                     file_contents=file.read()
                 file.close
             except Exception as exception:
-                logging.error("Load File - Error opening file - Layout will be created in its default state")
+                logging.error("Load File - Error opening file - Layout will remain in its default state")
                 logging.error("Load File - Reported Exception: "+str(exception))
-                tkinter.messagebox.showerror(title="File Load Error",message=str(exception))
+                tkinter.messagebox.showerror(parent=common.root_window,
+                                title="File Load Error", message=str(exception))
                 filename = None
             else:
                 # The file has been successfuly opened and loaded - Now convert it from the json format back
                 # into the dictionary of signals, points and sections - with exception handling in case it fails
                 try:
                     layout_state = json.loads(file_contents)
                 except Exception as exception:
                     logging.error("Load File - Couldn't read file - Layout will be created in its default state")
                     logging.error("Load File - Reported exception: "+str(exception))
-                    tkinter.messagebox.showerror(title="File Parse Error",message=str(exception))
+                    tkinter.messagebox.showerror(parent=common.root_window,
+                                title="File Parse Error", message=str(exception))
                     filename = None
             # Store the filename that was loaded - to use on application quit
             filename_used_for_load = filename
     return(filename)
 
 #-------------------------------------------------------------------------------------------------
 # Function called on application quit to save the current layout state to file. The actual options 
@@ -171,34 +174,35 @@
 # If 'save_as_option_enabled' is True, then we open a file dialogue to select a file.
 #
 # We return a 'quit_application' confirmation to the calling programme - This will be True if
 # the user selects to 'save & quit' or to 'quit without saving' - False if a dialog is cancelled
 #-------------------------------------------------------------------------------------------------
 
 def save_state_and_quit(quit_application:bool=True):
-    global logging
     global filename_used_for_load
     global save_as_option_enabled
     global filename_used_for_save
     global dictionary_to_save
     # filename_used_for_save will be None if the user subsequently cancels the save
     filename_used_for_save = None
     # get the filename that was used/attempted to load state on application startup
     filename = filename_used_for_load
     # Only pester the user with additional dialogs on application shutdown
     if quit_application:
         # if the global variable 'filename' is "None" then file loading/saving hasn't been configured by
         # the signalling application - we therefore just give the option to quit the application or cancel
         if filename is None:
-            quit_application = tkinter.messagebox.askokcancel("Quit","Do you want to quit the application?")
+            quit_application = tkinter.messagebox.askokcancel(parent=common.root_window,
+                            title="Quit", message="Do you want to quit the application?")
             # the value of quit_application will be True for YES and False for NO
             save_application = save_as_option_enabled
         else:
             # A filename has been configured - we need to give the option to save the current state
-            save_application = tkinter.messagebox.askyesnocancel("Quit","Do you want to save the current layout state")
+            save_application = tkinter.messagebox.askyesnocancel(parent=common.root_window,
+                            title="Quit", message="Do you want to save the current layout state")
             # the value of save_application will be True for YES, False for NO and None for CANCEL
             if save_application == True or save_application == False:
                 quit_application = True
             else:
                 quit_application = False
                 save_application = False
     else:
@@ -219,15 +223,15 @@
             # Force the ".sig" extension
             if not filename.endswith(".sig"): filename = filename+".sig"
             # Note that the asksaveasfilename dialog returns the fully qualified filename
             # (including the path) - we only need the name so strip out the path element
             # This also makes it clearer to see the default filename in the file save dialog
             path,name = os.path.split(filename)
             filename_used_for_save = filename            
-            logging.info("Saving Layout State Information as '"+name+"'")
+            logging.info("Saving Layout Configuration as '"+name+"'")
             dictionary_to_save["information"] = "Model Railway Signalling Configuration File"
             # Retrieve the DEFINITION of all the data items we need to save to maintain state
             # These are defined in a single function at the top of this source file. We also
             # retrieve the source DATA we need to save from the various source dictionaries
             layout_elements = get_sig_file_config(get_sig_file_data=True)
             # Iterate through the main LAYOUT-ELEMENTS (e.g. signals, points, sections etc)
             for layout_element in layout_elements:
@@ -262,26 +266,26 @@
             file_contents = json.dumps(dictionary_to_save,indent=4,sort_keys=True)
             try:
                 with open (filename_used_for_save,'w') as file:
                     file.write(file_contents)
                 file.close
             except Exception as exception:
                 logging.error("Save File - Error saving file - Reported exception: "+str(exception))
-                tkinter.messagebox.showerror(title="File Save Error",message=str(exception))
+                tkinter.messagebox.showerror(parent=common.root_window,
+                            title="File Save Error",message=str(exception))
                 quit_application = False
     return (quit_application)
 
 #-------------------------------------------------------------------------------------------------
 # Function called on creation of a signal/point/section/instrument Object to return the initial state
 # from the loaded data. If no layout state has been loaded or the loaded data doesn't include an
 # entry for the Object then we return 'None' and the Object will retain its "as created" default state
 #-------------------------------------------------------------------------------------------------
 
 def get_initial_item_state(layout_element:str,item_id:int):
-    global logging
     # Retrieve the DEFINITION of all the data items that are available
     sig_file_config = get_sig_file_config()
     # Check if the requested LAYOUT ELEMENT is a supported
     if layout_element not in sig_file_config.keys():
         logging.error("File Interface - Item type not supported : "+layout_element)
         state_to_return = None
     else:
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/library/mqtt_interface.py` & `model-railway-signals-3.4.0/model_railway_signals/library/mqtt_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,45 +83,42 @@
     return (return_value) 
 
 #-----------------------------------------------------------------------------------------------
 # Internal call-back to process mqtt log messages (only called if enhanced_debugging is set)
 #-----------------------------------------------------------------------------------------------
 
 def on_log(mqtt_client, obj, level, mqtt_log_message):
-    global logging
     logging.debug("MQTT-Client: "+mqtt_log_message)
     return()
 
 #-----------------------------------------------------------------------------------------------
 # Internal call-back to process broker disconnection events
 #-----------------------------------------------------------------------------------------------
 
 def on_disconnect(mqtt_client, userdata, rc):
-    global logging
     global node_config
     if rc==0: logging.info("MQTT-Client: Broker connection terminated")
     else: logging.warning("MQTT-Client: Unexpected disconnection from broker")
     node_config["connected_to_broker"] = False
     return()
 
 #-----------------------------------------------------------------------------------------------
 # Internal call-back to process broker connection / re-connection events
 #-----------------------------------------------------------------------------------------------
 
 def on_connect(mqtt_client, userdata, flags, rc):
-    global logging
     global node_config
     if rc == 0:
         logging.info("MQTT-Client: Successfully connected to MQTT Broker")
         # As we set up our broker connection with 'cleansession=true' a disconnection will have removed
         # all client connection information from the broker (including knowledge of the topics we have
         # subscribed to) - we therefore need to re-subscribe to all topics with this new connection
         # Note that this means we will immediately receive all retained messages for those topics
         if len(node_config["list_of_subscribed_topics"]) > 0:
-            logging.debug("MQTT-Client: Re-subscribing to all MQTT broker topics")
+            logging.debug("MQTT-Client: Re-subscribing to all MQTT broker topics:")
             for topic in node_config["list_of_subscribed_topics"]:
                 mqtt_client.subscribe(topic)
         # Pause just to ensure that MQTT is all fully up and running before we continue (and allow the client
         # to set up any subscriptions or publish any messages to the broker). We shouldn't need to do this but
         # I've experienced problems running on a Windows 10 platform if we don't include a short sleep
         time.sleep(0.1)
         node_config["connected_to_broker"] = True
@@ -136,42 +133,40 @@
 # Internal function to process messages received from the MQTT Broker - unpacking the message and then
 # making the registered callback to pass the message back to the main application. Note that this function
 # is executed in the main tkinter thread (as long as we know the main root window) to make it threadsafe
 # If we don't know the main root window then the function is executed in the current mqtt event thread.
 #--------------------------------------------------------------------------------------------------------
 
 def process_message(msg):
-    global logging
     # Unpack the json message so we can extract the contents (with exception handling)
     try:
         unpacked_json = json.loads(msg.payload)
     except Exception as exception:
         logging.error("MQTT-Client: Exception unpacking json - "+str(exception))
     else:
-        if node_config["enhanced_debugging"]:
-            logging.debug("MQTT-Client: Successfully parsed message:"+str(unpacked_json))
         # Make the callback (that was registered when the calling programme subscribed to the feed)
         # Note that we also need to test to see if the the topic is a partial match to cover the
         # case of subscribing to all subtopics for an specified item (with the '+' wildcard)
         if msg.topic in node_config["callbacks"]:
+            logging.debug("MQTT-Client: Received: "+str(msg.topic)+"-"+str(unpacked_json))
             node_config["callbacks"][msg.topic] (unpacked_json)
         elif msg.topic.rpartition('/')[0]+"/+" in node_config["callbacks"]:
+            logging.debug("MQTT-Client: Received: "+str(msg.topic)+"-"+str(unpacked_json))
             node_config["callbacks"][msg.topic.rpartition('/')[0]+"/+"] (unpacked_json)
         else:
-             logging.warning("MQTT-Client: unhandled message topic:"+str(msg.topic))
+            logging.warning("MQTT-Client: unhandled message topic: "+str(msg.topic))
     return()
 
 #--------------------------------------------------------------------------------------------------------
 # Internal function to handle messages received from the MQTT Broker. Note that we "pass" the
 # execution for processing the function back into the main Tkinter thread (assuming we know the
 # root window (if not, then as a fallback we raise a callback in the current mqtt event thread)
 #--------------------------------------------------------------------------------------------------------
 
 def on_message(mqtt_client,obj,msg):
-    global logging
     global node_config
     # Only process the message if there is a payload - If there is no payload then the message is
     # a "null message" - sent to purge retained messages from the broker on application exit
     if msg.payload:
         if common.root_window is not None:
             common.execute_function_in_tkinter_thread (lambda:process_message(msg)) 
         else:
@@ -185,15 +180,14 @@
 def configure_networking (broker_host:str,
                           network_identifier:str,
                           node_identifier:str,
                           broker_port:int = 1883,
                           broker_username:str = None,
                           broker_password:str = None,
                           mqtt_enhanced_debugging:bool = False):
-    global logging
     global node_config
     global mqtt_client
     logging.info("MQTT-Client: Connecting to Broker \'"+broker_host+"\'")
     mqtt_client = paho.mqtt.client.Client(clean_session=True)
     mqtt_client.on_message = on_message    
     mqtt_client.on_connect = on_connect    
     mqtt_client.on_disconnect = on_disconnect    
@@ -223,15 +217,14 @@
 
 #-----------------------------------------------------------------------------------------------
 # Externally called function to perform a gracefull shutdown of the MQTT networking
 # in terms of clearing out the publish topic queues (by sending null messages)
 #-----------------------------------------------------------------------------------------------
 
 def mqtt_shutdown():
-    global logging
     # Only shut down the mqtt networking if we configured it in the first place
     if node_config["network_configured"]:
         logging.info("MQTT-Client: Clearing message queues and shutting down")
         # Clean out the message queues on the broker by publishing null messages (empty strings)
         # to each of the topics that we have sent messages to during the lifetime of the session
         for topic in node_config["list_of_published_topics"]:
             publish_message(topic,payload=None,retain=True)
@@ -254,26 +247,25 @@
 # a fully qualified MQTT topic (using the Node and item ID). The registered callback will return
 # the content of the received messages. The optional subtopic flag enables you to subscribe
 # to all sub-topics from a particular item. This is used in the Model Railway Signalling Package
 # for subscribing to all DCC address messages (where each DCC address is a seperate subtopic)
 #-----------------------------------------------------------------------------------------------
 
 def subscribe_to_mqtt_messages (message_type:str,item_node:str,item_id:int,callback,subtopics:bool=False):
-    global logging
     global node_config
     global mqtt_client
     if not node_config["network_configured"]:
         logging.error("MQTT-Client: Networking Disabled - Cannot subscribe to MQTT messages")
     else:
         # The Identifier for a remote object is a string combining the the Node-ID and Object-ID
         item_identifier = create_remote_item_identifier(item_id,item_node)
-        logging.info("MQTT-Client: Subscribing to '"+message_type+"' from '"+item_identifier+"'")
         # Topic format: "<Message-Type>/<Network-ID>/<Item_Identifier>/<optional-subtopic>"
         topic = message_type+"/"+node_config["network_identifier"]+"/"+item_identifier
         if subtopics: topic = topic+"/+"
+        logging.info("MQTT-Client: Subscribing to topic' "+topic+"'")
         mqtt_client.subscribe(topic)
         # Add to the list of subscribed topics (so we can re-subscribe on reconnection)
         node_config["list_of_subscribed_topics"].append(topic)
         # Save the callback details for when we receive a message on the topic
         node_config["callbacks"][topic] = callback
         return()
 
@@ -296,23 +288,45 @@
     return()
 
 #-----------------------------------------------------------------------------------------------
 # Internal Function to Publish a json message to a fully qualified topic
 #-----------------------------------------------------------------------------------------------
 
 def publish_message (topic:str,payload:str,log_message:str=None,retain:bool=False):
-    global logging
     global mqtt_client
     global node_config
     if log_message is not None: logging.info(log_message)
-    if node_config["enhanced_debugging"]:
-        if payload is None: logging.debug("MQTT-Client: Publishing NULL message to MQTT broker")
-        else: logging.debug("MQTT-Client: Publishing JSON message to MQTT broker: "+payload)
+    if payload is None: logging.debug("MQTT-Client: Publishing: "+str(topic)+"-NULL")
+    else: logging.debug("MQTT-Client: Publishing: "+str(topic)+"-"+str(payload))
     # Publish the message to the broker
     mqtt_client.publish(topic,payload,retain=retain,qos=1)
     # Add to the list of published topics if this is a retained message so we
     # can 'Clean up' the MQTT broker by publishing empty messages on shutdown
     if topic not in node_config["list_of_published_topics"]:
         node_config["list_of_published_topics"].append(topic)
     return()
 
-##################################################################################################################
+#-----------------------------------------------------------------------------------------------
+# Non public  Function to unsubscribe to a particular message type from the broker. Called by
+# the higher-level 'reset_mqtt_configuration' functions for instruments, signals and sections to
+# clear out the relevant subscrptions in support of the editor - where a configuration change
+# to MQTT networking will trigger a reset of all subscriptions followed by a re-configuration
+#-----------------------------------------------------------------------------------------------
+
+def unsubscribe_from_message_type(message_type:str):
+    global node_config
+    # Only unsubscribe if networking has been configured
+    if node_config["network_configured"]:
+        # Topic format: "<Message-Type>/<Network-ID>/<Item_Identifier>/<optional-subtopic>"
+        # Finally, remove all instances of the message type from the internal subscriptions list
+        # Note we don't iterate through the list to remove items as it will change under us
+        new_list_of_subscribed_topics = []
+        for subscribed_topic in node_config["list_of_subscribed_topics"]:
+            if subscribed_topic.startswith(message_type):
+                logging.info("MQTT-Client: Unsubscribing from topic '"+subscribed_topic+"'")
+                mqtt_client.unsubscribe(subscribed_topic)
+            else:
+                new_list_of_subscribed_topics.append(subscribed_topic)
+        node_config["list_of_subscribed_topics"] = new_list_of_subscribed_topics
+    return()
+
+##################################################################################################################
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/library/pi_sprog_interface.py` & `model-railway-signals-3.4.0/model_railway_signals/library/pi_sprog_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,14 @@
 # short delay inbetween each message. We do this because some decoders don't
 # seem to process messages sent to them in quick succession - and if the
 # decoder "misses" an event the signal/point may end up in an erronous state
 #------------------------------------------------------------------------------
 
 def thread_to_send_buffered_data ():
     global transmit_delay
-    global logging
     global debug
     while True:
         command_string = output_buffer.get()
         #Print the Transmitted message (if the appropriate debug level is set)
         if debug:logging.debug ("Pi-SPROG - Transmit CBUS Message: " + command_string)
         # Write the CBUS Message to the serial port (with exception handling
         # We just handle any exceptions (we'll get exceptions during port re-configuration)
@@ -115,15 +114,14 @@
 # We're not receiving anything else on this port so its OK to set up the port 
 # without a timeout - as we are only interested in "complete" messages
 #------------------------------------------------------------------------------
 
 def thread_to_read_received_data ():
     global track_power_on
     global service_mode_status
-    global logging
     global rstat_response
     global qnn_response
     global debug
     while True:
         # Enbsure the thread doesn't hog all the CPU
         time.sleep(0.0001)
         # Read from the port until we get the GridConnect Protocol message termination character
@@ -225,15 +223,14 @@
 # References for Header Encoding - CBUS Developers Guide - Section 6.1, 6.4, 12.2
 #
 # Example - can_id=99 , mj_pri=2, min_pri=2, op_code=9 (RTON - request track on)
 # encodes into a CBUS Command 'SAC60N09;'
 #------------------------------------------------------------------------------
 
 def send_cbus_command (mj_pri:int, min_pri:int, op_code:int, *data_bytes:int):
-    global logging
     global can_bus_id
     if (mj_pri < 0 or mj_pri > 2):
         logging.error("CBUS Command - Invalid Major Priority "+str(mj_pri))
     elif (min_pri < 0 or min_pri > 3):
         logging.error("CBUS Command - Invalid Minor Priority "+str(min_pri))
     elif (op_code < 0 or op_code > 255):
         logging.error("CBUS Command - Op Code out of range "+str(op_code))
@@ -259,15 +256,14 @@
 # namely logging of all the CBUS commands sent to the Pi SPROG
 #------------------------------------------------------------------------------
 
 
 def initialise_pi_sprog (port_name:str="/dev/serial0",
                          baud_rate:int = 115200,
                          dcc_debug_mode:bool = False):
-    global logging
     global debug
     global threads_started
     # Assign the global "enhanced debugging" flag
     debug = dcc_debug_mode
     # Rx and Tx threads are Daemon so they will terminate with the main programme
     if not threads_started:
         logging.info ("Pi-SPROG: Starting Tx and Rx Threads")
@@ -349,15 +345,14 @@
     return(qnn_response)
 
 #------------------------------------------------------------------------------
 # Function called on shutdown to turn off DCC bus power and close the comms port
 #------------------------------------------------------------------------------
 
 def sprog_shutdown():
-    global logging
     # First switch off the DCC bus supply
     if track_power_on: request_dcc_power_off()
     # Now close the comms port
     if serial_port.is_open:
         logging.info ("Pi-SPROG: Closing Serial Port")
         try:
             serial_port.close()
@@ -368,15 +363,14 @@
 
 #------------------------------------------------------------------------------
 # Externally Called Function to turn on the track power
 #------------------------------------------------------------------------------
 
 def request_dcc_power_on():
     global track_power_on
-    global logging
     track_power_on = None    
     # Only bother sending commands to the Pi Sprog if the serial port has been opened
     if serial_port.is_open:
         # Send the command to switch on the Track Supply (to the DCC Bus)
         logging.info ("Pi-SPROG: Sending RTON command (Request Track Power On)")
         send_cbus_command (mj_pri=2, min_pri=2, op_code=9)
         # Now wait until we get confirmation thet the Track power is on
@@ -393,15 +387,14 @@
 
 #------------------------------------------------------------------------------
 # Externally Called Function to turn off the track power
 #------------------------------------------------------------------------------
 
 def request_dcc_power_off():
     global track_power_on
-    global logging
     track_power_on = None
     # Only bother sending commands to the Pi Sprog if the serial port has been opened
     if serial_port.is_open:
         # Send the command to switch on the Track Supply (to the DCC Bus)
         logging.info ("Pi-SPROG: Sending RTOF command (Request Track Power Off)")
         send_cbus_command (mj_pri=2, min_pri=2, op_code=8)
         # Now wait until we get confirmation thet the Track power is on
@@ -418,15 +411,14 @@
 #------------------------------------------------------------------------------
 # Externally Called Function to send an Accessory Short CBUS On/Off Event
 #------------------------------------------------------------------------------
 
 def send_accessory_short_event (address:int, active:bool):
     global pi_cbus_node
     global track_power_on
-    global logging
     if (address < 1 or address > 2047):
         logging.error ("Pi-SPROG: Invalid DCC short event accessory address: "+ str(address))
     # Only try to send the command if the PI-SPROG-3 has initialised correctly
     elif track_power_on:
         byte1 = (pi_cbus_node & 0xff00) >> 8
         byte2 = (pi_cbus_node & 0x00ff)
         byte3 = (address & 0xff00) >> 8
@@ -444,15 +436,14 @@
 # Externally Called Function to programme a single CV (used for testing)
 # Returns True if successful and False if no response is received (timeout)
 #------------------------------------------------------------------------------
 
 def service_mode_write_cv (cv:int, value:int):
     global track_power_on
     global service_mode_status
-    global logging
     if (cv < 0 or cv > 1023):
         logging.error("Pi-SPROG: WCVS (Write CV in Service Mode) - Invalid CV "+str(cv))
     elif (value < 0 or value > 255):
         logging.error("Pi-SPROG: WCVS (Write CV in Service Mode) - Invalid value for CV"+str(value))
     # Only try to send the command if the PI-SPROG-3 has initialised correctly
     elif track_power_on:
         byte1 = 255                    # Session ID
@@ -509,15 +500,14 @@
 #
 # NOTE - This function is currently untested as I have been unable to confirm
 # (either via research or Test) whether the Pi-SPROG-3 supports the RDDC3 Command 
 #------------------------------------------------------------------------------
 
 def send_DCC_accessory_decoder_packet (address:int, active:bool, output_channel:int = 0, repeat:int = 3):
     global track_power_on
-    global logging
     if (address < 1 or address > 511):
         logging.info("Error: send_accessory_decoder_packet - Invalid address "+str(address))
     elif (output_channel < 0 or output_channel > 7):
         logging.info("Error: send_accessory_decoder_packet - Invalid output channel " +
                       str(output_channel)+" for address "+str(address))    
     elif (repeat < 0 or repeat > 255):
         logging.info("Error: send_accessory_decoder_packet - Invalid Repeat Value " +
@@ -553,15 +543,14 @@
 #
 # NOTE - This function is currently untested as I have been unable to confirm
 # (either via research or Test) whether the Pi-SPROG-3 supports the RDDC4 Command 
 #------------------------------------------------------------------------------
 
 def send_extended_DCC_accessory_decoder_packet (address:int, aspect:int, repeat:int = 3, alt_address = False):
     global track_power_on
-    global logging
     if (address < 1 or address > 2044):
         logging.info("Error: send_extended_DCC_accessory_decoder_packet - Invalid address "+str(address))
     elif (aspect < 0 or aspect > 31):
         logging.info("Error: send_extended_DCC_accessory_decoder_packet - Invalid aspect "+str(aspect))
     elif track_power_on:
         # DCC Address interpretation 1 and 2
         address -= 1
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/library/points.py` & `model-railway-signals-3.4.0/model_railway_signals/library/points.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,36 +93,32 @@
     return(point_id,callback_type)
 
 # -------------------------------------------------------------------------
 # Callbacks for processing button pushes
 # -------------------------------------------------------------------------
 
 def fpl_button_event (point_id:int):
-    global logging
     logging.info("Point "+str(point_id)+": FPL Button Event ************************************************************")
     toggle_fpl(point_id)
     points[str(point_id)]["extcallback"] (point_id,point_callback_type.fpl_switched)
     return ()
 
 def change_button_event (point_id:int):
-    global logging
     logging.info("Point "+str(point_id)+": Change Button Event *********************************************************")
     toggle_point(point_id)
     points[str(point_id)]["extcallback"] (point_id,point_callback_type.point_switched)
     return ()
 
 # -------------------------------------------------------------------------
 # Public API Function to flip the state of the Point's Facing Point Lock (to
 # enable route setting functions. Also called whenthe FPL button is pressed 
 # -------------------------------------------------------------------------
 
 def toggle_fpl (point_id:int):
-
     global points 
-    global logging
     # Validate the point ID as this can be called by external code
     if not point_exists(point_id):
         logging.error ("Point "+str(point_id)+": Toggle FPL - Point does not exist")
     elif not points[str(point_id)]["hasfpl"]:
         logging.error ("Point "+str(point_id)+": Toggle FPL - Point does not have a facing point lock")
     else:
         if points[str(point_id)]["locked"]:
@@ -142,18 +138,15 @@
 # -------------------------------------------------------------------------
 # Internal Function to toggle the point blade drawing objects and update
 # the internal state of the point - called by the toggle_point function
 # Can also be called on point creation to set the initial (loaded) state
 # -------------------------------------------------------------------------
 
 def toggle_point_state (point_id:int, switched_by_another_point = False):
-
     global points
-    global logging
-
     if not points[str(point_id)]["switched"]:
         if switched_by_another_point:
             logging.info ("Point "+str(point_id)+": Changing point to SWITCHED (switched with another point)")
         else:
             logging.info ("Point "+str(point_id)+": Changing point to SWITCHED")
         points[str(point_id)]["changebutton"].config(relief="sunken",bg="white")
         points[str(point_id)]["switched"] = True
@@ -175,17 +168,15 @@
 # -------------------------------------------------------------------------
 # Public API Function to flip the route setting for the Point (to enable
 # route setting functions. Also called whenthe POINT button is pressed 
 # Will also recursivelly call itself to change any "also_switch" points
 # -------------------------------------------------------------------------
 
 def toggle_point (point_id:int, switched_by_another_point = False):
-    
     global points
-    global logging
     # Validate the point ID as this can be called by external code
     if not point_exists(point_id):
         logging.error ("Point "+str(point_id)+": Toggle Point - Point does not exist")
     elif points[str(point_id)]["automatic"] and not switched_by_another_point:
         logging.error ("Point "+str(point_id)+": Toggle Point - Point is automatic (should  be \'also switched\' by another point)")
     else:
         if points[str(point_id)]["locked"]:
@@ -215,17 +206,15 @@
 # external programme can change the colours if required)
 # -------------------------------------------------------------------------
 
 def create_point (canvas, point_id:int, pointtype:point_type,
                   x:int, y:int, colour:str="black", orientation:int = 0,
                   point_callback = null_callback, also_switch:int = 0,
                   reverse:bool=False,auto:bool=False,fpl:bool=False):
-    
     global points
-    global logging
     logging.info ("Point "+str(point_id)+": Creating Point")
     # Find and store the root window (when the first signal is created)
     if common.root_window is None: common.find_root_window(canvas)
     # Do some basic validation on the parameters we have been given
     if point_exists(point_id):
         logging.error ("Point "+str(point_id)+": Point already exists")
         point_objects = [0,0,0,0]
@@ -362,15 +351,14 @@
 # Public API function to Lock one or more points. The external signal/point
 # interlocking should be written to ensure it is only possible to lock a
 # point when the Facing point Lock is activated
 # -------------------------------------------------------------------------
 
 def lock_point (*point_ids:int):
     global points 
-    global logging
     for point_id in point_ids:
         # Validate the point exists 
         if not point_exists(point_id):
             logging.error ("Point "+str(point_id)+": lock_point - Point does not exist")
         elif not points[str(point_id)]["locked"]:
             logging.info ("Point "+str(point_id)+": Locking point")
             if not points[str(point_id)]["hasfpl"]:
@@ -387,15 +375,14 @@
 
 # -------------------------------------------------------------------------
 # Public API function to Unlock one or more points
 # -------------------------------------------------------------------------
 
 def unlock_point (*point_ids:int):
     global points 
-    global logging
     for point_id in point_ids:
         # Validate the point exists
         if not point_exists(point_id):
             logging.error ("Point "+str(point_id)+": unlock_point - Point does not exist")
         elif points[str(point_id)]["locked"]:
             logging.info ("Point "+str(point_id)+": Unlocking point")
             if not points[str(point_id)]["hasfpl"]:
@@ -408,30 +395,28 @@
     return ()
 
 # -------------------------------------------------------------------------
 # Public API function to Return the current state of the point
 # -------------------------------------------------------------------------
 
 def point_switched (point_id:int):
-    global logging
     # Validate the point exists
     if not point_exists(point_id):
         logging.error ("Point "+str(point_id)+": point_switched - Point does not exist")
         switched = False
     else:   
         switched = points[str(point_id)]["switched"]
     return(switched)
 
 # -------------------------------------------------------------------------
 # Public API function to query the current state of the FPL
 # if the point does not have a FPL the return will always be TRUE
 # -------------------------------------------------------------------------
 
 def fpl_active(point_id:int):
-    global logging
     # Validate the point exists
     if not point_exists(point_id):
         logging.error ("Point "+str(point_id)+": fpl_active - Point does not exist")
         locked = False
     elif not points[str(point_id)]["hasfpl"]:
         # Point does not have a FPL - always return True in this case
         locked = True
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/library/resources/bell-ring-01.wav` & `model-railway-signals-3.4.0/model_railway_signals/library/resources/bell-ring-01.wav`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.3.0/model_railway_signals/library/resources/bell-ring-02.wav` & `model-railway-signals-3.4.0/model_railway_signals/library/resources/bell-ring-02.wav`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.3.0/model_railway_signals/library/resources/bell-ring-03.wav` & `model-railway-signals-3.4.0/model_railway_signals/library/resources/bell-ring-03.wav`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.3.0/model_railway_signals/library/resources/bell-ring-04.wav` & `model-railway-signals-3.4.0/model_railway_signals/library/resources/bell-ring-04.wav`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.3.0/model_railway_signals/library/resources/telegraph-key-01.wav` & `model-railway-signals-3.4.0/model_railway_signals/library/resources/telegraph-key-01.wav`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.3.0/model_railway_signals/library/signals.py` & `model-railway-signals-3.4.0/model_railway_signals/library/signals.py`

 * *Files 2% similar despite different names*

```diff
@@ -334,15 +334,14 @@
 # Note that the DISPLAYED state of the signal may not be CLEAR if the signal is
 # overridden or subject to release on RED - See "signal_displaying_clear"
 # Function applicable to ALL signal types created on the local schematic
 # Function does not support REMOTE Signals (with a compound Sig-ID)
 # -------------------------------------------------------------------------
 
 def signal_clear (sig_id:int,route:signals_common.route_type = None):
-    global logging
     # Validate the signal exists
     if not signals_common.sig_exists(sig_id):
         logging.error ("Signal "+str(sig_id)+": signal_clear - Signal does not exist")
         sig_clear = False
     else:
         if route is None:
             sig_clear = signals_common.signals[str(sig_id)]["sigclear"]
@@ -356,15 +355,14 @@
 # (i.e. whether the signal is actually displaying a CLEAR aspect). Note that
 # this can be different to the state the signal has been manually set to (via
 # the signal button) - as it could be overridden or subject to Release on Red
 # Function applicable to ALL signal types - Including REMOTE SIGNALS
 # -------------------------------------------------------------------------
 
 def signal_state (sig_id:Union[int,str]):
-    global logging
     # Validate the signal exists
     if not signals_common.sig_exists(sig_id):
         logging.error ("Signal "+str(sig_id)+": signal_state - Signal does not exist")
         sig_state = signals_common.signal_state_type.DANGER
     else:
         sig_state = signals_common.signals[str(sig_id)]["sigstate"]
     return (sig_state)
@@ -373,15 +371,14 @@
 # Externally called function to Return the current state of the subsidary
 # signal - if the signal does not have one then the return will be FALSE
 # Function applicable to ALL signal types created on the local schematic
 # Function does not support REMOTE Signals (with a compound Sig-ID)
 # -------------------------------------------------------------------------
 
 def subsidary_clear (sig_id:int,route:signals_common.route_type = None):
-    global logging
     # Validate the signal exists
     if not signals_common.sig_exists(sig_id):
         logging.error ("Signal "+str(sig_id)+": subsidary_clear - Signal does not exist")
         sig_clear = False
     elif not signals_common.signals[str(sig_id)]["hassubsidary"]:
         logging.error ("Signal "+str(sig_id)+": subsidary_clear - Signal does not have a subsidary")
         sig_clear = False
@@ -397,15 +394,14 @@
 # Externally called function to Lock the signal (preventing it being cleared)
 # Multiple signal IDs can be specified in the call
 # Function applicable to ALL signal types created on the local schematic
 # Function does not support REMOTE Signals (with a compound Sig-ID)
 # -------------------------------------------------------------------------
 
 def lock_signal (*sig_ids:int):
-    global logging
     for sig_id in sig_ids:
         # Validate the signal exists
         if not signals_common.sig_exists(sig_id):
             logging.error ("Signal "+str(sig_id)+": lock_signal - Signal does not exist")
         else:
             signals_common.lock_signal(sig_id)
     return()
@@ -414,15 +410,14 @@
 # Externally called function to Unlock the main signal
 # Multiple signal IDs can be specified in the call
 # Function applicable to ALL signal types created on the local schematic
 # Function does not support REMOTE Signals (with a compound Sig-ID)
 # -------------------------------------------------------------------------
 
 def unlock_signal (*sig_ids:int):
-    global logging
     for sig_id in sig_ids:
         # Validate the signal exists
         if not signals_common.sig_exists(sig_id):
             logging.error ("Signal "+str(sig_id)+": unlock_signal - Signal does not exist")
         else:
             signals_common.unlock_signal(sig_id)
     return() 
@@ -433,15 +428,14 @@
 # Multiple signal IDs can be specified in the call
 # Function applicable to ALL signal types created on the local schematic
 # (will report an error if the specified signal does not have a subsidary)
 # Function does not support REMOTE Signals (with a compound Sig-ID)
 # -------------------------------------------------------------------------
 
 def lock_subsidary (*sig_ids:int):
-    global logging
     for sig_id in sig_ids:
         # Validate the signal exists
         if not signals_common.sig_exists(sig_id):
             logging.error ("Signal "+str(sig_id)+": lock_subsidary - Signal does not exist")
         elif not signals_common.signals[str(sig_id)]["hassubsidary"]:
             logging.error ("Signal "+str(sig_id)+": lock_subsidary - Signal does not have a subsidary")
         else:
@@ -454,15 +448,14 @@
 # Multiple signal IDs can be specified in the call
 # Function applicable to ALL signal types created on the local schematic
 # (will report an error if the specified signal does not have a subsidary)
 # Function does not support REMOTE Signals (with a compound Sig-ID)
 # -------------------------------------------------------------------------
 
 def unlock_subsidary (*sig_ids:int):
-    global logging
     for sig_id in sig_ids:
         # Validate the signal exists
         if not signals_common.sig_exists(sig_id):
             logging.error ("Signal "+str(sig_id)+": unlock_subsidary - Signal does not exist")
         elif not signals_common.signals[str(sig_id)]["hassubsidary"]:
             logging.error ("Signal "+str(sig_id)+": unlock_subsidary - Signal does not have a subsidary")
         else:
@@ -476,15 +469,14 @@
 # Used to support automation - e.g. set a signal to Danger once a train has passed
 # Multiple signal IDs can be specified in the call
 # Function applicable to ALL signal types created on the local schematic
 # Function does not support REMOTE Signals (with a compound Sig-ID)
 # -------------------------------------------------------------------------
 
 def set_signal_override (*sig_ids:int):
-    global logging
     for sig_id in sig_ids:
         # Validate the signal exists
         if not signals_common.sig_exists(sig_id):
             logging.error ("Signal "+str(sig_id)+": set_signal_override - Signal does not exist")
         else:
             # Set the override and refresh the signal following the change in state
             signals_common.set_signal_override(sig_id)
@@ -496,15 +488,14 @@
 # Signal will revert to its current manual setting (on/off) and aspect
 # Multiple signal IDs can be specified in the call
 # Function applicable to ALL signal types created on the local schematic
 # Function does not support REMOTE Signals (with a compound Sig-ID)
 # -------------------------------------------------------------------------
 
 def clear_signal_override (*sig_ids:int):
-    global logging
     for sig_id in sig_ids:
         # Validate the signal exists
         if not signals_common.sig_exists(sig_id):
             logging.error ("Signal "+str(sig_id)+": clear_signal_override - Signal does not exist")
         else:
             # Clear the override and refresh the signal following the change in state
             signals_common.clear_signal_override(sig_id)
@@ -517,15 +508,14 @@
 # e.g. set a signal to CAUTION if any Home signals ahead are at DANGER.
 # Multiple signal IDs can be specified in the call
 # Function applicable to all signal types apart from HOME signals
 # Function does not support REMOTE Signals (with a compound Sig-ID)
 # -------------------------------------------------------------------------
 
 def set_signal_override_caution (*sig_ids:int):
-    global logging
     for sig_id in sig_ids:
         # Validate the signal exists
         if not signals_common.sig_exists(sig_id):
             logging.error ("Signal "+str(sig_id)+": set_signal_override_caution - Signal does not exist")
         elif ( ( signals_common.signals[str(sig_id)]["sigtype"] == signals_common.sig_type.colour_light and
                  signals_common.signals[str(sig_id)]["subtype"] != signals_colour_lights.signal_sub_type.home ) or
                ( signals_common.signals[str(sig_id)]["sigtype"] == signals_common.sig_type.semaphore and
@@ -542,15 +532,14 @@
 # Signal will revert to its current manual setting (on/off) and aspect
 # Multiple signal IDs can be specified in the call
 # Function applicable to ALL signal types created on the local schematic
 # Function does not support REMOTE Signals (with a compound Sig-ID)
 # -------------------------------------------------------------------------
 
 def clear_signal_override_caution (*sig_ids:int):
-    global logging
     for sig_id in sig_ids:
         # Validate the signal exists
         if not signals_common.sig_exists(sig_id):
             logging.error ("Signal "+str(sig_id)+": clear_signal_override_caution - Signal does not exist")
         elif ( ( signals_common.signals[str(sig_id)]["sigtype"] == signals_common.sig_type.colour_light and
                  signals_common.signals[str(sig_id)]["subtype"] != signals_colour_lights.signal_sub_type.home ) or
                ( signals_common.signals[str(sig_id)]["sigtype"] == signals_common.sig_type.semaphore and
@@ -568,15 +557,14 @@
 # to enable automated route setting from the external programme.
 # Use in conjunction with 'signal_clear' to find the state first
 # Function applicable to ALL signal types created on the local schematic
 # Function does not support REMOTE Signals (with a compound Sig-ID)
 # -------------------------------------------------------------------------
 
 def toggle_signal (sig_id:int):
-    global logging
     # Validate the signal exists
     if not signals_common.sig_exists(sig_id):
         logging.error ("Signal "+str(sig_id)+": toggle_signal - Signal does not exist")
     else:
         if signals_common.signals[str(sig_id)]["siglocked"]:
             logging.warning ("Signal "+str(sig_id)+": toggle_signal - Signal is locked - Toggling anyway")
         # Toggle the signal and refresh the signal following the change in state
@@ -590,15 +578,14 @@
 # in conjunction with 'subsidary_signal_clear' to find the state first
 # Function applicable to ALL signal types created on the local schematic
 # (will report an error if the specified signal does not have a subsidary)
 # Function does not support REMOTE Signals (with a compound Sig-ID)
 # -------------------------------------------------------------------------
 
 def toggle_subsidary (sig_id:int):
-    global logging
     # Validate the signal exists
     if not signals_common.sig_exists(sig_id):
         logging.error ("Signal "+str(sig_id)+": toggle_subsidary - Signal does not exist")
     elif not signals_common.signals[str(sig_id)]["hassubsidary"]:
         logging.error ("Signal "+str(sig_id)+": toggle_subsidary - Signal does not have a subsidary")
     else:
         if signals_common.signals[str(sig_id)]["sublocked"]:
@@ -618,15 +605,14 @@
 # Calls the signal type-specific functions depending on the signal type
 # Function applicable to Colour Light and Semaphore signal types created on
 # the local schematic (will report an error if the particular signal type not
 # supported) Function does not support REMOTE Signals (with a compound Sig-ID)
 # -------------------------------------------------------------------------
 
 def set_approach_control (sig_id:int, release_on_yellow:bool = False, force_set:bool = True):
-    global logging
     # Validate the signal exists
     if not signals_common.sig_exists(sig_id):
         logging.error ("Signal "+str(sig_id)+": set_approach_control - Signal does not exist")
     else:
         # call the signal type-specific functions to update the signal (note that we only update
         # Semaphore and colour light signals if they are configured to update immediately)
         if signals_common.signals[str(sig_id)]["sigtype"] == signals_common.sig_type.colour_light:
@@ -660,15 +646,14 @@
 # Calls the signal type-specific functions depending on the signal type
 # Function applicable to Colour Light and Semaphore signal types created on
 # the local schematic (will have no effect on other signal types
 # Function does not support REMOTE Signals (with a compound Sig-ID)
 # -------------------------------------------------------------------------
 
 def clear_approach_control (sig_id:int):
-    global logging
     # Validate the signal exists
     if not signals_common.sig_exists(sig_id):
         logging.error ("Signal "+str(sig_id)+": clear_approach_control - Signal does not exist")  
     else:
         # call the signal type-specific functions to update the signal (note that we only update
         # Semaphore and colour light signals if they are configured to update immediately)
         if ( signals_common.signals[str(sig_id)]["sigtype"] == signals_common.sig_type.colour_light or
@@ -687,15 +672,14 @@
 # Calls the signal type-specific functions depending on the signal type
 # Function applicable only to Main colour Light and semaphore signal types
 # created on the local schematic - but either locally-created or REMOTE
 # Signals can be specified as the signal ahead
 # -------------------------------------------------------------------------
 
 def update_signal (sig_id:int, sig_ahead_id:Union[int,str]=None):
-    global logging
     # Validate the signal exists (and the one ahead if specified)
     if not signals_common.sig_exists(sig_id):
         logging.error ("Signal "+str(sig_id)+": update_signal - Signal does not exist")
     elif sig_ahead_id != None and not signals_common.sig_exists(sig_ahead_id): 
         logging.error ("Signal "+str(sig_id)+": update_signal - Signal ahead "+str(sig_ahead_id)+" does not exist")
     elif sig_id == sig_ahead_id: 
         logging.error ("Signal "+str(sig_id)+": update_signal - Signal ahead "+str(sig_ahead_id)+" is the same ID")
@@ -714,15 +698,14 @@
 # Calls the signal type-specific functions depending on the signal type
 # Function only applicable to Main Colour Light and Semaphore signal types
 # created on the local schematic (will raise an error if signal type not
 # supported. Function does not support REMOTE Signals (with a compound Sig-ID)
 # -------------------------------------------------------------------------
 
 def set_route (sig_id:int, route:signals_common.route_type = None, theatre_text:str = None):
-    global logging
     # Validate the signal exists
     if not signals_common.sig_exists(sig_id):
         logging.error ("Signal "+str(sig_id)+": set_route - Signal does not exist")
     else:
         if route is not None:
             # call the signal type-specific functions to update the signal
             if signals_common.signals[str(sig_id)]["sigtype"] == signals_common.sig_type.colour_light:
@@ -753,15 +736,14 @@
 # a'sig_updated' callback event will be generated
 # Function only applicable to Main Colour Light and Semaphore signal types
 # created on the local schematic (will raise an error if signal type not
 # supported. Function does not support REMOTE Signals (with a compound Sig-ID)
 # -------------------------------------------------------------------------
 
 def trigger_timed_signal (sig_id:int,start_delay:int=0,time_delay:int=5):
-    global logging
     # Validate the signal exists
     if not signals_common.sig_exists(sig_id):
         logging.error ("Signal "+str(sig_id)+": trigger_timed_signal - Signal does not exist")
     else:
         # call the signal type-specific functions to update the signal
         if signals_common.signals[str(sig_id)]["sigtype"] == signals_common.sig_type.colour_light:
             logging.info ("Signal "+str(sig_id)+": Triggering Timed Signal")
@@ -775,102 +757,74 @@
 
 #-----------------------------------------------------------------------------------------------
 # Public API Function to "subscribe" to signal updates published by another MQTT"Node"
 #-----------------------------------------------------------------------------------------------
 
 def subscribe_to_signal_updates (node:str,sig_callback,*sig_ids:int):    
     for sig_id in sig_ids:
-        mqtt_interface.subscribe_to_mqtt_messages("signal_updated_event",node,sig_id,
-                                                signals_common.handle_mqtt_signal_updated_event)
         # Create a dummy signal object to hold the state of the remote signal
         # The Identifier is a string combining the the Node-ID and Section-ID
         sig_identifier = mqtt_interface.create_remote_item_identifier(sig_id,node)
         if not signals_common.sig_exists(sig_identifier):
             signals_common.signals[sig_identifier] = {}
             signals_common.signals[sig_identifier]["sigtype"] = signals_common.sig_type.remote_signal
             signals_common.signals[sig_identifier]["sigstate"] = signals_common.signal_state_type.DANGER
             signals_common.signals[sig_identifier]["routeset"] = signals_common.route_type.NONE
             signals_common.signals[sig_identifier]["extcallback"] = sig_callback
+        # Subscribe to updates from the remote signal (even if we have already subscribed)
+        mqtt_interface.subscribe_to_mqtt_messages("signal_updated_event",node,sig_id,
+                                    signals_common.handle_mqtt_signal_updated_event)
     return()
 
 #-----------------------------------------------------------------------------------------------
 # Public API Function to "subscribe" to signal passed events published by another "Node"
 #-----------------------------------------------------------------------------------------------
 
 def subscribe_to_signal_passed_events (node:str, sig_callback, *sig_ids:int):    
     for sig_id in sig_ids:
-        mqtt_interface.subscribe_to_mqtt_messages("signal_passed_event",node,sig_id,
-                                                signals_common.handle_mqtt_signal_passed_event)
         # Create a dummy signal object to hold the state of the remote signal
         # The Identifier is a string combining the the Node-ID and Section-ID
         sig_identifier = mqtt_interface.create_remote_item_identifier(sig_id,node)
         if not signals_common.sig_exists(sig_identifier):
             signals_common.signals[sig_identifier] = {}
             signals_common.signals[sig_identifier]["sigtype"] = signals_common.sig_type.remote_signal
             signals_common.signals[sig_identifier]["sigstate"] = signals_common.signal_state_type.DANGER
             signals_common.signals[sig_identifier]["routeset"] = signals_common.route_type.NONE
             signals_common.signals[sig_identifier]["extcallback"] = sig_callback
+        # Subscribe to updates from the remote signal (even if we have already subscribed)
+        mqtt_interface.subscribe_to_mqtt_messages("signal_passed_event",node,sig_id,
+                                    signals_common.handle_mqtt_signal_passed_event)
     return()
 
 #-----------------------------------------------------------------------------------------------
 # Public API Function to set all aspect changes to be "published" for a signal
 #-----------------------------------------------------------------------------------------------
 
 def set_signals_to_publish_state(*sig_ids:int):    
-    global logging
     for sig_id in sig_ids:
         logging.info("MQTT-Client: Configuring signal "+str(sig_id)+" to publish state changes via MQTT broker")
         # Add the signal ID to the list of signals to publish
         if sig_id in signals_common.list_of_signals_to_publish_state_changes:
             logging.warning("MQTT-Client: Signal "+str(sig_id)+" - is already configured to publish state changes")
         else:
             signals_common.list_of_signals_to_publish_state_changes.append(sig_id)
+            # Publish the initial state now this has been added to the list of signals to publish
+            # This allows the publish/subscribe functions to be configured after signal creation
+            if str(sig_id) in signals_common.signals.keys(): signals_common.publish_signal_state(sig_id) 
     return()
 
 #-----------------------------------------------------------------------------------------------
 # Public API Function to set all "signal passed" events to be "published" for a signal
 #-----------------------------------------------------------------------------------------------
 
 def set_signals_to_publish_passed_events(*sig_ids:int):    
-    global logging
     for sig_id in sig_ids:
         logging.info("MQTT-Client: Configuring signal "+str(sig_id)+" to publish passed events via MQTT broker")
         # Add the signal ID to the list of signals to publish
         if sig_id in signals_common.list_of_signals_to_publish_passed_events:
             logging.warning("MQTT-Client: Signal "+str(sig_id)+" - is already configured to publish passed events")
         else:
             signals_common.list_of_signals_to_publish_passed_events.append(sig_id)
     return()
 
-# ------------------------------------------------------------------------------------------
-# Non public API function for deleting a signal object (including all the drawing objects)
-# This is used by the schematic editor for changing signal types where we delete the existing
-# signal with all its data and then recreate it (with the same ID) in its new configuration
-# ------------------------------------------------------------------------------------------
-
-def delete_signal(sig_id:int):
-    if signals_common.sig_exists(sig_id):
-        # Delete all the tkinter canvas drawing objects associated with the signal
-        signals_common.signals[str(sig_id)]["canvas"].delete("signal"+str(sig_id))
-        # Delete all the tkinter button objects created for the signal
-        signals_common.signals[str(sig_id)]["sigbutton"].destroy()
-        signals_common.signals[str(sig_id)]["subbutton"].destroy()
-        signals_common.signals[str(sig_id)]["passedbutton"].destroy()
-        if signals_common.signals[str(sig_id)]["sigtype"] in (signals_common.sig_type.colour_light,
-                                                              signals_common.sig_type.semaphore):
-            # This buttons is only common to colour light and semaphore types
-            signals_common.signals[str(sig_id)]["releasebutton"].destroy()
-            # Abort any timed signal sequences already in progess
-            route = signals_common.signals[str(sig_id)]["routeset"]
-            signals_common.signals[str(sig_id)]["timedsequence"][route.value].abort()
-        # Finally, delete the signal entry from the dictionary of signals
-        del signals_common.signals[str(sig_id)]
-    return()
-
-# ------------------------------------------------------------------------------------------
-# Non public API function to return the tkinter canvas 'tags' for the signal
-# ------------------------------------------------------------------------------------------
-
-def get_tags(sig_id:int):
-    return("signal"+str(sig_id))
 
 ##########################################################################################
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/library/signals_colour_lights.py` & `model-railway-signals-3.4.0/model_railway_signals/library/signals_colour_lights.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,14 @@
                                 lhfeather45:bool=False,
                                 lhfeather90:bool=False,
                                 rhfeather45:bool=False,
                                 rhfeather90:bool=False,
                                 theatre_route_indicator:bool=False,
                                 refresh_immediately = True,
                                 fully_automatic:bool=False):
-    global logging
-
     logging.info ("Signal "+str(sig_id)+": Creating Colour Light Signal")
     # Do some basic validation on the parameters we have been given
     signal_has_feathers = mainfeather or lhfeather45 or lhfeather90 or rhfeather45 or rhfeather90
     if signals_common.sig_exists(sig_id):
         logging.error ("Signal "+str(sig_id)+": Signal already exists")
     elif sig_id < 1:
         logging.error ("Signal "+str(sig_id)+": Signal ID must be greater than zero")
@@ -213,25 +211,28 @@
             # Set the initial state of the subsidary from the "loaded" state
             if loaded_state["subclear"]: signals_common.toggle_subsidary(sig_id)
             # Update the signal to show the initial aspect (and send out DCC commands)
             update_colour_light_subsidary(sig_id)
             # finally Lock the subsidary if required 
             if loaded_state["sublocked"]: signals_common.lock_subsidary(sig_id)
 
+        # Publish the initial state to the broker (for other nodes to consume). Note that changes will
+        # only be published if the MQTT interface has been configured for publishing updates for this 
+        # signal. This allows publish/subscribe to be configured prior to signal creation
+        signals_common.publish_signal_state(sig_id)
+        
     return ()
 
 #-------------------------------------------------------------------
 # Internal Function to update the current state of the Subsidary signal
 # (on/off). If a Subsidary was not specified at creation time then the
 # objects are hidden' and the function will have no effect.
 #------------------------------------------------------------------
     
 def update_colour_light_subsidary (sig_id:int):
-    
-    global logging
     if signals_common.signals[str(sig_id)]["subclear"]:
         logging.info ("Signal "+str(sig_id)+": Changing subsidary aspect to PROCEED")
         signals_common.signals[str(sig_id)]["canvas"].itemconfig (signals_common.signals[str(sig_id)]["pos1"],fill="white")
         signals_common.signals[str(sig_id)]["canvas"].itemconfig (signals_common.signals[str(sig_id)]["pos2"],fill="white")
         dcc_control.update_dcc_signal_element(sig_id,True,element="main_subsidary")  
     else:
         signals_common.signals[str(sig_id)]["canvas"].itemconfig (signals_common.signals[str(sig_id)]["pos1"],fill="grey")
@@ -245,17 +246,15 @@
 # Also takes into account the state of the signal ahead if one is specified
 # to ensure the correct aspect is displayed (for 3/4 aspect types and 2 aspect 
 # distant signals). E.g. for a 3/4 aspect signal - if the signal ahead is ON
 # and this signal is OFF then we want to change it to YELLOW rather than GREEN
 # -------------------------------------------------------------------------
 
 def update_colour_light_signal (sig_id:int, sig_ahead_id:Union[str,int]=None):
-
-    global logging
-
+    
     route = signals_common.signals[str(sig_id)]["routeset"]
     
     # ---------------------------------------------------------------------------------
     #  First deal with the Signal ON, Overridden or "Release on Red" cases
     #  as they will apply to all colour light signal types (2, 3 or 4 aspect)
     # ---------------------------------------------------------------------------------
 
@@ -468,15 +467,14 @@
     return ()
 
 # -------------------------------------------------------------------------
 # Function to change the feather route indication (on route change)
 # -------------------------------------------------------------------------
 
 def update_feather_route_indication (sig_id:int,route_to_set):
-    global logging
     # Only Change the route indication if the signal has feathers
     if signals_common.signals[str(sig_id)]["hasfeathers"]:
         # Deal with route changes - but only if the Route has actually been changed
         if route_to_set != signals_common.signals[str(sig_id)]["routeset"]:
             signals_common.signals[str(sig_id)]["routeset"] = route_to_set
             if signals_common.signals[str(sig_id)]["featherenabled"] == True:
                 logging.info ("Signal "+str(sig_id)+": Changing feather route display to "+ str(route_to_set).rpartition('.')[-1])
@@ -497,15 +495,14 @@
 
 # -------------------------------------------------------------------------
 # Internal Function that gets called on a signal aspect change - will
 # Enable/disable the feather route indication on a change to/from DANGER
 # -------------------------------------------------------------------------
 
 def enable_disable_feather_route_indication (sig_id:int):
-    global logging
     # Only Enable/Disable the route indication if the signal has feathers
     if signals_common.signals[str(sig_id)]["hasfeathers"]:
         # We test for !True and !False to support the initial state when the signal is created (state = None)
         if (signals_common.signals[str(sig_id)]["sigstate"] == signals_common.signal_state_type.DANGER
                      and signals_common.signals[str(sig_id)]["featherenabled"] != False):
             logging.info ("Signal "+str(sig_id)+": Disabling feather route display (signal is at RED)")
             signals_common.signals[str(sig_id)]["featherenabled"] = False
@@ -564,15 +561,14 @@
         self.sequence_abort_flag = False
         self.sequence_in_progress = False
 
     def abort(self):
         self.sequence_abort_flag = True
             
     def start(self):
-        global logging
         if self.sequence_abort_flag:
             self.sequence_in_progress = False
         else:
             self.sequence_in_progress = True
             # For a start delay of zero we assume the intention is not to make a callback (on the basis
             # that the user has triggered the timed signal in the first place). For start delays > 0 the 
             # sequence is initiated after the specified delay and this will trigger a callback
@@ -591,15 +587,14 @@
             # We only need to schedule the next YELLOW aspect for 3 and 4 aspect signals - otherwise schedule sequence completion
             if signals_common.signals[str(self.sig_id)]["subtype"] in (signal_sub_type.three_aspect, signal_sub_type.four_aspect):
                 common.root_window.after(self.time_delay*1000,lambda:self.timed_signal_sequence_yellow())
             else:
                 common.root_window.after(self.time_delay*1000,lambda:self.timed_signal_sequence_end())
 
     def timed_signal_sequence_yellow(self):
-        global logging
         if self.sequence_abort_flag:
             self.sequence_in_progress = False
         else:
             # This sequence step only applicable to 3 and 4 aspect signals
             self.aspect = signals_common.signal_state_type.CAUTION
             # Only change the aspect and generate the callback if the same route is set
             if signals_common.signals[str(self.sig_id)]["routeset"] == self.sig_route:
@@ -609,30 +604,28 @@
             # We only need to schedule the next DOUBLE YELLOW aspect for 4 aspect signals - otherwise schedule sequence completion
             if signals_common.signals[str(self.sig_id)]["subtype"] == signal_sub_type.four_aspect:
                 common.root_window.after(self.time_delay*1000,lambda:self.timed_signal_sequence_double_yellow())
             else:
                 common.root_window.after(self.time_delay*1000,lambda:self.timed_signal_sequence_end())
     
     def timed_signal_sequence_double_yellow(self):
-        global logging
         if self.sequence_abort_flag:
             self.sequence_in_progress = False
         else:
             # This sequence step only applicable to 4 aspect signals
             self.aspect = signals_common.signal_state_type.PRELIM_CAUTION
             # Only change the aspect and generate the callback if the same route is set
             if signals_common.signals[str(self.sig_id)]["routeset"] == self.sig_route:
                 logging.info("Signal "+str(self.sig_id)+": Timed Signal - Signal Updated Event *************************")
                 update_colour_light_signal(self.sig_id)
                 signals_common.signals[str(self.sig_id)]["extcallback"] (self.sig_id, signals_common.sig_callback_type.sig_updated)
             # Schedule the next aspect change (which will be the sequence completion)
             common.root_window.after(self.time_delay*1000,lambda:self.timed_signal_sequence_end())
     
     def timed_signal_sequence_end(self): 
-        global logging
         # We've finished - Set the signal back to its "normal" condition
         self.sequence_in_progress = False
         if not self.sequence_abort_flag:
             # Only change the aspect and generate the callback if the same route is set
             if signals_common.signals[str(self.sig_id)]["routeset"] == self.sig_route:
                 logging.info("Signal "+str(self.sig_id)+": Timed Signal - Signal Updated Event *************************")
                 update_colour_light_signal(self.sig_id)
@@ -646,15 +639,14 @@
 # signal is changed to RED and the time_delay is the delay (in seconds) between each 
 # aspect change. A 'sig_passed' callback event will be generated when the signal is 
 # overriden if a start delay (> 0) is specified. For each subsequent aspect change
 # a 'sig_updated' callback event will be generated.
 # -------------------------------------------------------------------------
 
 def trigger_timed_colour_light_signal (sig_id:int,start_delay:int=0,time_delay:int=5):
-    global logging
     # Don't initiate a timed signal sequence if a shutdown has already been initiated
     if common.shutdown_initiated:
         logging.warning("Signal "+str(sig_id)+": Timed Signal - Shutdown initiated - not triggering timed signal")
     else:
         # Abort any timed signal sequences already in progess
         route = signals_common.signals[str(sig_id)]["routeset"]
         signals_common.signals[str(sig_id)]["timedsequence"][route.value].abort()
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/library/signals_common.py` & `model-railway-signals-3.4.0/model_railway_signals/library/signals_common.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,38 +96,35 @@
     return (sig_id,callback_type)
 
 # -------------------------------------------------------------------------
 # Callbacks for processing button pushes
 # -------------------------------------------------------------------------
 
 def signal_button_event (sig_id:int):
-    global logging
     logging.info("Signal "+str(sig_id)+": Signal Change Button Event *************************************************")
     # toggle the signal state and refresh the signal
     toggle_signal(sig_id)
     auto_refresh_signal(sig_id)
     # Make the external callback (if one was specified at signal creation time)
     signals[str(sig_id)]['extcallback'] (sig_id,sig_callback_type.sig_switched)
     return ()
 
 def subsidary_button_event (sig_id:int):
-    global logging
     logging.info("Signal "+str(sig_id)+": Subsidary Change Button Event **********************************************")
     toggle_subsidary(sig_id)
     #  call the signal type-specific functions to update the signal
     if signals[str(sig_id)]["sigtype"] == sig_type.colour_light:
         signals_colour_lights.update_colour_light_subsidary(sig_id)
     elif signals[str(sig_id)]["sigtype"] == sig_type.semaphore:
         signals_semaphores.update_semaphore_subsidary_arms(sig_id)
     # Make the external callback (if one was specified at signal creation time)
     signals[str(sig_id)]['extcallback'] (sig_id,sig_callback_type.sub_switched)
     return ()
 
 def sig_passed_button_event (sig_id:int):
-    global logging
     logging.info("Signal "+str(sig_id)+": Signal Passed Event **********************************************")
     # Pulse the signal passed button to provide a visual indication (but not if a shutdown has been initiated)
     if not common.shutdown_initiated:
         signals[str(sig_id)]["passedbutton"].config(bg="red")
         common.root_window.after(1000,lambda:signals[str(sig_id)]["passedbutton"].config(bg=common.bgraised))
     # Reset the approach control 'released' state (if the signal supports approach control)
     if ( signals[str(sig_id)]["sigtype"] == sig_type.colour_light or
@@ -137,15 +134,14 @@
     # mqtt interface has been successfully configured and the signal has been set to publish passed events
     publish_signal_passed_event(sig_id)
     # Make the external callback (if one was specified at signal creation time)
     signals[str(sig_id)]['extcallback'] (sig_id,sig_callback_type.sig_passed)
     return ()
 
 def approach_release_button_event (sig_id:int):
-    global logging
     logging.info("Signal "+str(sig_id)+": Approach Release Event *******************************************")
     # Pulse the approach release button to provide a visual indication
     if not common.shutdown_initiated:
         signals[str(sig_id)]["releasebutton"].config(bg="red")
         common.root_window.after(1000,lambda:signals[str(sig_id)]["releasebutton"].config(bg=common.bgraised))
     # Set the approach control 'released' state (if the signal supports approach control)
     if ( signals[str(sig_id)]["sigtype"] == sig_type.colour_light or
@@ -176,15 +172,14 @@
     return()
 
 # -------------------------------------------------------------------------
 # Common function to flip the internal state of a signal
 # -------------------------------------------------------------------------
 
 def toggle_signal (sig_id:int):
-    global logging
     global signals
     # Update the state of the signal button - Common to ALL signal types
     # The Signal Clear boolean value will always be either True or False
     if signals[str(sig_id)]["sigclear"]:
         logging.info ("Signal "+str(sig_id)+": Toggling signal to ON")
         signals[str(sig_id)]["sigclear"] = False
         if not signals[str(sig_id)]["automatic"]:
@@ -199,15 +194,14 @@
     return ()
 
 # -------------------------------------------------------------------------
 # Common function to flip the internal state of a subsidary signal
 # -------------------------------------------------------------------------
 
 def toggle_subsidary (sig_id:int):
-    global logging
     global signals
     # Update the state of the subsidary button - Common to ALL signal types.
     # The subsidary clear boolean value will always be either True or False
     if signals[str(sig_id)]["subclear"]:
         logging.info ("Signal "+str(sig_id)+": Toggling subsidary to ON")
         signals[str(sig_id)]["subclear"] = False
         signals[str(sig_id)]["subbutton"].config(relief="raised",bg=common.bgraised)
@@ -219,15 +213,14 @@
 
 # -------------------------------------------------------------------------
 # Common function to Set the approach control mode for a signal
 # (shared by Colour Light and semaphore signal types)
 # -------------------------------------------------------------------------
 
 def set_approach_control (sig_id:int, release_on_yellow:bool = False, force_set:bool = True):
-    global logging
     global signals
     # Only set approach control if the signal is not in the period between 
     # 'released' and 'passed' events (unless the force_reset flag is set)
     if force_set or not signals[str(sig_id)]["released"]:
         # Give an indication that the approach control has been set for the signal
         signals[str(sig_id)]["sigbutton"].config(font=('Courier',common.fontsize,"underline"))
         # Only set approach control if it is not already set for the signal
@@ -245,86 +238,80 @@
 
 #-------------------------------------------------------------------------
 # Common function to Clear the approach control mode for a signal
 # (shared by Colour Light and semaphore signal types)
 # -------------------------------------------------------------------------
 
 def clear_approach_control (sig_id:int):
-    global logging
     global signals
     # Only Clear approach control if it is currently set for the signal
     if signals[str(sig_id)]["releaseonred"] or signals[str(sig_id)]["releaseonyel"]:
         logging.info ("Signal "+str(sig_id)+": Clearing approach control")
         signals[str(sig_id)]["releaseonyel"] = False
         signals[str(sig_id)]["releaseonred"] = False
         signals[str(sig_id)]["sigbutton"].config(font=('Courier',common.fontsize,"normal"))
     return()
 
 # -------------------------------------------------------------------------
 # Common Function to set a signal override
 # -------------------------------------------------------------------------
 
 def set_signal_override (sig_id:int):
-    global logging
     global signals
     # Only set the override if the signal is not already overridden
     if not signals[str(sig_id)]["override"]:
         logging.info ("Signal "+str(sig_id)+": Setting override")
         # Set the override state and change the button text to indicate override
         signals[str(sig_id)]["override"] = True
         signals[str(sig_id)]["sigbutton"].config(fg="red", disabledforeground="red")
     return()
 
 # -------------------------------------------------------------------------
 # Common Function to clear a signal override
 # -------------------------------------------------------------------------
 
 def clear_signal_override (sig_id:int):
-    global logging
     global signals
     # Only clear the override if the signal is already overridden
     if signals[str(sig_id)]["override"]:
         logging.info ("Signal "+str(sig_id)+": Clearing override")
         # Clear the override and change the button colour
         signals[str(sig_id)]["override"] = False
         signals[str(sig_id)]["sigbutton"].config(fg="black",disabledforeground="grey50")
     return()
 
 # -------------------------------------------------------------------------
 # Common Function to set a signal override
 # -------------------------------------------------------------------------
 
 def set_signal_override_caution (sig_id:int):
-    global logging
     global signals
     # Only set the override if the signal is not already overridden
     if not signals[str(sig_id)]["overcaution"]:
         logging.info ("Signal "+str(sig_id)+": Setting override CAUTION")
         signals[str(sig_id)]["overcaution"] = True
     return()
 
 # -------------------------------------------------------------------------
 # Common Function to clear a signal override
 # -------------------------------------------------------------------------
 
 def clear_signal_override_caution (sig_id:int):
-    global logging
     global signals
     # Only clear the override if the signal is already overridden
     if signals[str(sig_id)]["overcaution"]:
         logging.info ("Signal "+str(sig_id)+": Clearing override CAUTION")
         signals[str(sig_id)]["overcaution"] = False
     return()
 
 # -------------------------------------------------------------------------
 # Common Function to lock a signal (i.e. for point/signal interlocking)
 # -------------------------------------------------------------------------
 
 def lock_signal (sig_id:int):
-    global logging
     global signals
     # Only lock if it is currently unlocked
     if not signals[str(sig_id)]["siglocked"]:
         logging.info ("Signal "+str(sig_id)+": Locking signal")
         # If signal/point locking has been correctly implemented it should
         # only be possible to lock a signal that is "ON" (i.e. at DANGER)
         if signals[str(sig_id)]["sigclear"]:
@@ -335,15 +322,14 @@
     return()
 
 # -------------------------------------------------------------------------
 # Common Function to unlock a signal (i.e. for point/signal interlocking)
 # -------------------------------------------------------------------------
 
 def unlock_signal (sig_id:int):
-    global logging
     global signals
     # Only unlock if it is currently locked
     if signals[str(sig_id)]["siglocked"]:
         logging.info ("Signal "+str(sig_id)+": Unlocking signal")
         # Enable the Signal button to unlock it (if its not a fully automatic signal)
         if not signals[str(sig_id)]["automatic"]:
             signals[str(sig_id)]["sigbutton"].config(state="normal")
@@ -351,15 +337,14 @@
     return() 
 
 # -------------------------------------------------------------------------
 # Common Function to lock a subsidary (i.e. for point/signal interlocking)
 # -------------------------------------------------------------------------
 
 def lock_subsidary (sig_id:int):
-    global logging
     global signals
     # Only lock if it is currently unlocked
     if not signals[str(sig_id)]["sublocked"]:
         logging.info ("Signal "+str(sig_id)+": Locking subsidary")
         # If signal/point locking has been correctly implemented it should
         # only be possible to lock a signal that is "ON" (i.e. at DANGER)
         if signals[str(sig_id)]["subclear"]:
@@ -370,15 +355,14 @@
     return()
 
 # -------------------------------------------------------------------------
 # Common Function to unlock a subsidary (i.e. for point/signal interlocking)
 # -------------------------------------------------------------------------
 
 def unlock_subsidary (sig_id:int):
-    global logging
     global signals
     # Only unlock if it is currently locked
     if signals[str(sig_id)]["sublocked"]:
         logging.info ("Signal "+str(sig_id)+": Unlocking subsidary")
         # Re-enable the Button to unlock the subsidary signal
         signals[str(sig_id)]["subbutton"].config(state="normal")
         signals[str(sig_id)]["sublocked"] = False
@@ -528,15 +512,14 @@
 
 # -------------------------------------------------------------------------
 # Common function to change the theatre route indication
 # (shared by Colour Light and semaphore signal types)
 # -------------------------------------------------------------------------
 
 def update_theatre_route_indication (sig_id,theatre_text:str):
-    global logging
     global signals
     # Only update the Theatre route indication if one exists for the signal
     if signals[str(sig_id)]["hastheatre"]:
         # Deal with route changes (if a new route has been passed in) - but only if the theatre text has changed
         if theatre_text != signals[str(sig_id)]["theatretext"]:
             signals[str(sig_id)]["canvas"].itemconfig(signals[str(sig_id)]["theatreobject"],text=theatre_text)
             signals[str(sig_id)]["theatretext"] = theatre_text
@@ -553,15 +536,14 @@
 # -------------------------------------------------------------------------
 # Common Function that gets called on a signal aspect change - will
 # Enable/disable the theatre route indicator on a change to/from DANGER 
 # (shared by Colour Light and semaphore signal types)
 # -------------------------------------------------------------------------
 
 def enable_disable_theatre_route_indication (sig_id):
-    global logging
     global signals
     # Only update the Theatre route indication if one exists for the signal
     if signals[str(sig_id)]["hastheatre"]:
         # Deal with the theatre route inhibit/enable cases (i.e. signal at DANGER or not at DANGER)
         # We test for Not True and Not False to support the initial state when the signal is created (state = None)
         if signals[str(sig_id)]["sigstate"] == signal_state_type.DANGER and signals[str(sig_id)]["theatreenabled"] != False:
             logging.info ("Signal "+str(sig_id)+": Disabling theatre route display (signal is at DANGER)")
@@ -578,43 +560,44 @@
     return()
 
 # --------------------------------------------------------------------------------
 # Callbacks for handling MQTT messages received from a remote Signal
 # --------------------------------------------------------------------------------
 
 def handle_mqtt_signal_updated_event(message):
-    global logging
     global signals
     if "sourceidentifier" in message.keys() and "sigstate" in message.keys():
         signal_identifier = message["sourceidentifier"]
         # The sig state is an enumeration type - so its the VALUE that gets passed in the message
         signals[signal_identifier]["sigstate"] = signal_state_type(message["sigstate"])
         logging.info("Signal "+signal_identifier+": State update from remote signal *****************************")
         logging.info ("Signal "+signal_identifier+": Aspect has changed to : "+
                             str(signals[signal_identifier]["sigstate"]).rpartition('.')[-1])
         # Make the external callback (if one has been defined)
         signals[signal_identifier]["extcallback"] (signal_identifier,sig_callback_type.sig_updated)
     return()
 
 def handle_mqtt_signal_passed_event(message):
-    global logging
     if "sourceidentifier" in message.keys():
         signal_identifier = message["sourceidentifier"]
         logging.info("Signal "+signal_identifier+": Remote Signal Passed Event ***********************************")
         # Make the external callback (if one has been defined)
         signals[signal_identifier]["extcallback"] (signal_identifier,sig_callback_type.sig_passed)
     return()
 
 # --------------------------------------------------------------------------------
-# Common functions for building and sending MQTT messages - but only if the
-# Signal has been configured to publish the specified updates via the mqtt broker
+# Common functions for building and sending MQTT messages - but only if the Signal
+# has been configured to publish the specified updates via the mqtt broker. As this
+# function is called on signal creation, we also need to handle the case of a signal
+# configured to NOT to refresh on creation (i.e. it gets set when 'update_signal' is
+# called for the first time - in this case (sigstate = None) we don't publish
 # --------------------------------------------------------------------------------
 
 def publish_signal_state(sig_id:int):
-    if sig_id in list_of_signals_to_publish_state_changes:
+    if sig_id in list_of_signals_to_publish_state_changes and signals[str(sig_id)]["sigstate"] is not None:
         data = {}
         # The sig state is an enumeration type - so its the VALUE that gets passed in the message
         data["sigstate"] = signals[str(sig_id)]["sigstate"].value
         log_message = "Signal "+str(sig_id)+": Publishing signal state to MQTT Broker"
         # Publish as "retained" messages so remote items that subscribe later will always pick up the latest state
         mqtt_interface.send_mqtt_message("signal_updated_event",sig_id,data=data,log_message=log_message,retain=True)
         return()
@@ -631,22 +614,62 @@
 # Common internal functions for deleting a signal object (including all the drawing objects)
 # This is used by the schematic editor for moving signals and changing signal types where we
 # delete the existing signal with all its data and then recreate it in its new configuration
 # ------------------------------------------------------------------------------------------
 
 def delete_signal(sig_id:int):
     global signals
+    global list_of_signals_to_publish_state_changes
+    global list_of_signals_to_publish_passed_events
     if sig_exists(sig_id):
         # Delete all the tkinter canvas drawing objects created for the signal
         signals[str(sig_id)]["canvas"].delete("signal"+str(sig_id))
         # Delete all the tkinter button objects created for the signal
         signals[str(sig_id)]["sigbutton"].destroy()
         signals[str(sig_id)]["subbutton"].destroy()
         signals[str(sig_id)]["passedbutton"].destroy()
         # This buttons is only common to colour light and semaphore types
         if signals[str(sig_id)]["sigtype"] in (sig_type.colour_light,sig_type.semaphore):
             signals[str(sig_id)]["releasebutton"].destroy()
+        # Delete the signal from the list_of_signals_to_publish (if required)
+        if sig_id in list_of_signals_to_publish_passed_events:
+            list_of_signals_to_publish_passed_events.remove(sig_id)
+        if sig_id in list_of_signals_to_publish_state_changes:
+            list_of_signals_to_publish_state_changes.remove(sig_id)
         # Finally, delete the signal entry from the dictionary of signals
         del signals[str(sig_id)]
     return()
 
+# ------------------------------------------------------------------------------------------
+# Non public API function to reset the list of published/subscribed signals. Used
+# by the schematic editor for re-setting the MQTT configuration prior to re-configuring
+# via the signal-specific publish and subscribe configuration functions
+# ------------------------------------------------------------------------------------------
+
+def reset_mqtt_configuration():
+    global signals
+    global list_of_signals_to_publish_state_changes
+    global list_of_signals_to_publish_passed_events
+    # We only need to clear the list to stop any further signal events being published
+    list_of_signals_to_publish_state_changes.clear()
+    list_of_signals_to_publish_passed_events.clear()
+    # For subscriptions we unsubscribe from all topics associated with the message_type
+    mqtt_interface.unsubscribe_from_message_type("signal_updated_event")
+    mqtt_interface.unsubscribe_from_message_type("signal_passed_event")
+    # Finally remove all "remote" signals from the dictionary of signals - these will
+    # be re-created if they are subsequently re-subscribed to. Note we don't iterate 
+    # through the dictionary of signals to remove items as it will change under us
+    new_signals = {}
+    for key in signals:
+        if mqtt_interface.split_remote_item_identifier(key) is not None:
+            new_signals[key] = signals[key]
+    signals = new_signals
+    return()
+
+# ------------------------------------------------------------------------------------------
+# Non public API function to return the tkinter canvas 'tags' for the signal
+# ------------------------------------------------------------------------------------------
+
+def get_tags(sig_id:int):
+    return("signal"+str(sig_id))
+
 #################################################################################################
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/library/signals_ground_disc.py` & `model-railway-signals-3.4.0/model_railway_signals/library/signals_ground_disc.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,16 +25,14 @@
 # -------------------------------------------------------------------------
 
 def create_ground_disc_signal (canvas, sig_id:int, x:int, y:int,
                                signal_subtype=ground_disc_sub_type.standard,
                                sig_callback = None,
                                orientation:int = 0,
                                sig_passed_button: bool = False):
-    global logging
-
     logging.info ("Signal "+str(sig_id)+": Creating Ground Disc Signal")
     # Do some basic validation on the parameters we have been given
     if signals_common.sig_exists(sig_id):
         logging.error ("Signal "+str(sig_id)+": Signal already exists")        
     elif sig_id < 1:
         logging.error ("Signal "+str(sig_id)+": Signal ID must be greater than zero")        
     elif orientation != 0 and orientation != 180:
@@ -77,25 +75,27 @@
         # 'sigclear' for ground signals - everything else gets set when the signal is updated
         if loaded_state["override"]: signals_common.set_signal_override(sig_id)
         if loaded_state["sigclear"]: signals_common.toggle_signal(sig_id)
         # Update the signal to show the initial aspect (and send out DCC commands)
         update_ground_disc_signal(sig_id)
         # finally Lock the signal if required
         if loaded_state["siglocked"]: signals_common.lock_signal(sig_id)
-        
+        # Publish the initial state to the broker (for other nodes to consume). Note that changes will
+        # only be published if the MQTT interface has been configured for publishing updates for this 
+        # signal. This allows publish/subscribe to be configured prior to signal creation
+        signals_common.publish_signal_state(sig_id)
     return ()
 
 # -------------------------------------------------------------------------
 # Internal function to Refresh the aspects of a ground disc signal
 # Note that we expect this function to only ever get called on a state 
 # change therefore we don't track the displayed aspect of the signal
 # -------------------------------------------------------------------------
 
 def update_ground_disc_signal (sig_id:int):
-    global logging
     
     # Establish what the signal should be displaying based on the state
     if not signals_common.signals[str(sig_id)]["sigclear"]:   
         aspect_to_set = signals_common.signal_state_type.DANGER
         log_message = " (signal is ON)"
     elif signals_common.signals[str(sig_id)]["override"]:
         aspect_to_set = signals_common.signal_state_type.DANGER
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/library/signals_ground_position.py` & `model-railway-signals-3.4.0/model_railway_signals/library/signals_ground_position.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,16 +27,14 @@
 # -------------------------------------------------------------------------
 
 def create_ground_position_signal (canvas, sig_id:int, x:int, y:int,
                                     signal_subtype=ground_pos_sub_type.early_standard,
                                     sig_callback = None,
                                     orientation:int = 0,
                                     sig_passed_button: bool = False):
-    global logging
-    
     logging.info ("Signal "+str(sig_id)+": Creating Ground Position Signal")
     # Do some basic validation on the parameters we have been given
     if signals_common.sig_exists(sig_id):
         logging.error ("Signal "+str(sig_id)+": Signal already exists")        
     elif sig_id < 1:
         logging.error ("Signal "+str(sig_id)+": Signal ID must be greater than zero")        
     elif orientation != 0 and orientation != 180:
@@ -100,27 +98,28 @@
         # 'sigclear' for ground signals - everything else gets set when the signal is updated
         if loaded_state["override"]: signals_common.set_signal_override(sig_id)
         if loaded_state["sigclear"]: signals_common.toggle_signal(sig_id)
         # Update the signal to show the initial aspect (and send out DCC commands)
         update_ground_position_signal(sig_id)
         # finally Lock the signal if required
         if loaded_state["siglocked"]: signals_common.lock_signal(sig_id)
-
+        # Publish the initial state to the broker (for other nodes to consume). Note that changes will
+        # only be published if the MQTT interface has been configured for publishing updates for this 
+        # signal. This allows publish/subscribe to be configured prior to signal creation
+        signals_common.publish_signal_state(sig_id)
     return ()
 
 # -------------------------------------------------------------------------
 # Internal function to Refresh the aspects of a ground position signal
 # Note that we expect this function to only ever get called on a state 
 # change therefore we don't track the displayed aspect of the signal
 # -------------------------------------------------------------------------
 
 def update_ground_position_signal (sig_id:int):
 
-    global logging
-    
     # Establish what the signal should be displaying based on the state
     if not signals_common.signals[str(sig_id)]["sigclear"]:   
         aspect_to_set = signals_common.signal_state_type.DANGER
         log_message = " (signal is ON)"
     elif signals_common.signals[str(sig_id)]["override"]:
         aspect_to_set = signals_common.signal_state_type.DANGER
         log_message = " (signal is OVERRIDDEN)"
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/library/signals_semaphores.py` & `model-railway-signals-3.4.0/model_railway_signals/library/signals_semaphores.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,14 @@
                                 lh1_subsidary:bool=False,
                                 lh2_subsidary:bool=False,
                                 rh1_subsidary:bool=False,
                                 rh2_subsidary:bool=False,
                                 theatre_route_indicator:bool=False,
                                 refresh_immediately:bool = True,
                                 fully_automatic:bool=False):
-    global logging
     
     # Do some basic validation on the parameters we have been given
     logging.info ("Signal "+str(sig_id)+": Creating Semaphore Signal")
 
     has_subsidary = main_subsidary or lh1_subsidary or lh2_subsidary or rh1_subsidary or rh2_subsidary
     has_junction_arms = (lh1_subsidary or lh2_subsidary or rh1_subsidary or rh2_subsidary or
                          lh1_signal or lh2_signal or rh1_signal or rh2_signal )
@@ -376,27 +375,31 @@
                        and signals_common.signals[str(sig_id)]["rh2_subsidary"]==True ):
                     signals_common.signals[str(sig_id)]["rh2_subsidary"] = False
             # Update the signal to show the initial aspect (and send out DCC commands)
             update_semaphore_subsidary_arms(sig_id)
             # finally Lock the subsidary if required 
             if loaded_state["sublocked"]: signals_common.lock_subsidary(sig_id)
             
+        # Publish the initial state to the broker (for other nodes to consume). Note that changes will
+        # only be published if the MQTT interface has been configured for publishing updates for this 
+        # signal. This allows publish/subscribe to be configured prior to signal creation
+        signals_common.publish_signal_state(sig_id)
+
     return ()
 
 #-------------------------------------------------------------------
 # Internal Function to update the drawing objects for a specified signal Arm
 # to represent the state of the signal arm (either ON or OFF). If the signal
 # was not created with the specificed signal arm then the state of the signal
 # arm will be "None" and the function will have no effect. All changes in the
 # signal arm state are logged (together with the additional log message passed
 # into the function as to WHY the signal Arm is being changed to its new state
 #------------------------------------------------------------------
 
 def update_signal_arm (sig_id, signal_arm, off_element, on_element, set_to_clear, log_message = ""):
-    global logging
     # We explicitly test for True or False as "None" signifies the signal arm does not exist
     if set_to_clear and signals_common.signals[str(sig_id)][signal_arm]==False:
         logging.info ("Signal "+str(sig_id)+": Changing \'"+signal_arm+"\' arm to OFF"+log_message)
         signals_common.signals[str(sig_id)]["canvas"].itemconfigure(signals_common.signals[str(sig_id)][off_element],state='normal')
         signals_common.signals[str(sig_id)]["canvas"].itemconfigure(signals_common.signals[str(sig_id)][on_element],state='hidden')
         dcc_control.update_dcc_signal_element(sig_id,True,element=signal_arm)
         signals_common.signals[str(sig_id)][signal_arm]=True
@@ -413,15 +416,14 @@
 # a signal to reflect the current state of the subsidary (either ON or OFF)
 # and the route set for the signal (i.e the actual subsidary arm that is changed
 # will depend on the route that the particular subsidary arm is controlling
 # Calls the Update_Signal_Arm function to update the state of each arm
 #------------------------------------------------------------------
 
 def update_semaphore_subsidary_arms (sig_id:int, log_message:str=""):
-    global logging
     # We explicitly test for True and False as a state of 'None' signifies the signal was created without a subsidary
     if signals_common.signals[str(sig_id)]["subclear"] == True:
         # If the route has been set to signals_common.route_type.NONE then we assume the MAIN Route
         if signals_common.signals[str(sig_id)]["routeset"] in (signals_common.route_type.MAIN,signals_common.route_type.NONE):
             update_signal_arm (sig_id, "main_subsidary", "mainsuboff", "mainsubon", True, log_message)
             update_signal_arm (sig_id, "lh1_subsidary", "lh1suboff", "lh1subon", False, log_message)
             update_signal_arm (sig_id, "lh2_subsidary", "lh2suboff", "lh2subon", False, log_message)
@@ -473,15 +475,14 @@
 # a signal to reflect the current state of the main signal (either ON or OFF)
 # and the route set for the signal (i.e the actual  signal arm that is changed
 # will depend on the route that the particular signal arm is controlling
 # Calls the Update_Signal_Arm function to update the state of each arm
 # -------------------------------------------------------------------------
 
 def update_main_signal_arms(sig_id:int, log_message:str=""):
-    global logging
     # When Home/Distant signal is set to PROCEED - the main signal arms will reflect the route
     # Also the case of a home signal associated with a distant signal (i.e on the same post). In
     # this case if the home signal is at DANGER and the distant signal is at CAUTION then the state
     # of the Home signal will be set to caution - in this case we need to set the home arms to OFF
     if (signals_common.signals[str(sig_id)]["sigstate"] == signals_common.signal_state_type.PROCEED or
          (signals_common.signals[str(sig_id)]["sigstate"] == signals_common.signal_state_type.CAUTION and
            signals_common.signals[str(sig_id)]["subtype"] == semaphore_sub_type.home) ):
@@ -540,16 +541,14 @@
 # distant signals - e.g. for a 3/4 aspect signal - if the signal ahead is ON
 # and this signal is OFF then we want to change it to YELLOW rather than GREEN
 # This function assumes the Sig_ID has been validated by the calling programme
 # -------------------------------------------------------------------------
 
 def update_semaphore_signal (sig_id:int, sig_ahead_id:Union[int,str]=None, updating_associated_signal:bool=False):
     
-    global logging
-
     route = signals_common.signals[str(sig_id)]["routeset"]
     
     # Get the ID of the associated signal (to make the following code more readable)
     associated_signal = signals_common.signals[str(sig_id)]["associatedsignal"]
     # Establish what the signal should be displaying based on the state
     if signals_common.signals[str(sig_id)]["subtype"] == semaphore_sub_type.distant:
         if not signals_common.signals[str(sig_id)]["sigclear"]:
@@ -623,17 +622,14 @@
 # Function to set (and update) the route indication for the signal
 # Calls the internal functions to update the route feathers and the
 # theatre route indication. This Function assumes the Sig_ID has
 # already been validated by the calling programme
 # -------------------------------------------------------------------------
 
 def update_semaphore_route_indication (sig_id,route_to_set = None):
-
-    global logging
-    
     # Only update the respective route indication if the route has been changed and has actively
     # been set (a route of 'NONE' signifies that the particular route indication isn't used) 
     if route_to_set is not None and signals_common.signals[str(sig_id)]["routeset"] != route_to_set:
         logging.info ("Signal "+str(sig_id)+": Setting semaphore route to "+str(route_to_set).rpartition('.')[-1])
         signals_common.signals[str(sig_id)]["routeset"] = route_to_set
         # Refresh the signal drawing objects (which will also send the DCC commands to change the arms accordingly)
         # Log messages will also be generated for each change - so we don't need lo log anything extra here
@@ -667,15 +663,14 @@
         self.sequence_abort_flag = False
         self.sequence_in_progress = False
 
     def abort(self):
         self.sequence_abort_flag = True
             
     def start(self):
-        global logging
         if self.sequence_abort_flag:
             self.sequence_in_progress = False
         else:
             self.sequence_in_progress = True
             # For a start delay of zero we assume the intention is not to make a callback (on the basis
             # that the user has triggered the timed signal in the first place). For start delays > 0 the 
             # sequence is initiated after the specified delay and this will trigger a callback
@@ -690,15 +685,14 @@
                     signals_common.signals[str(self.sig_id)]["extcallback"] (self.sig_id,signals_common.sig_callback_type.sig_passed)
                 else:
                     update_semaphore_signal(self.sig_id)
             # We need to schedule the sequence completion (i.e. back to clear
             common.root_window.after(self.time_delay*1000,lambda:self.timed_signal_sequence_end())
 
     def timed_signal_sequence_end(self):
-        global logging
         # We've finished - Set the signal back to its "normal" condition
         self.sequence_in_progress = False
         if not self.sequence_abort_flag:
             logging.info("Signal "+str(self.sig_id)+": Timed Signal - Signal Updated Event *************************")
             update_semaphore_signal(self.sig_id)
             signals_common.signals[str(self.sig_id)]["extcallback"] (self.sig_id, signals_common.sig_callback_type.sig_updated)
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/library/track_sections.py` & `model-railway-signals-3.4.0/model_railway_signals/library/track_sections.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,15 +111,14 @@
     return (str(section_id) in sections.keys() )
 
 # -------------------------------------------------------------------------
 # Callback for processing Button presses (manual toggling of Track Sections)
 # -------------------------------------------------------------------------
 
 def section_button_event (section_id:int):
-    global logging
     logging.info ("Section "+str(section_id)+": Track Section Toggled *****************************************************")
     toggle_section(section_id)
     # Publish the state changes to the broker (for other nodes to consume). Note that changes will only
     # be published if the MQTT interface has been configured for publishing updates for this track section
     send_mqtt_section_updated_event(section_id)
     # Make the external callback (if one has been defined)
     sections[str(section_id)]["extcallback"] (section_id,section_callback_type.section_updated)
@@ -127,15 +126,14 @@
 
 # -------------------------------------------------------------------------
 # Internal function to flip the state of the section
 # -------------------------------------------------------------------------
 
 def toggle_section (section_id:int):
     global sections
-    global logging
     if sections[str(section_id)]["occupied"]:
         # section is on
         logging.info ("Section "+str(section_id)+": Changing to CLEAR - Label \'"
                                          +sections[str(section_id)]["labeltext"]+"\'")
         sections[str(section_id)]["occupied"] = False
         sections[str(section_id)]["button1"].config(relief="raised", bg="grey", fg="grey40",
                                             activebackground="grey", activeforeground="grey40")
@@ -226,15 +224,14 @@
 # -------------------------------------------------------------------------
 
 def create_section (canvas, section_id:int, x:int, y:int,
                     section_callback = null_callback,
                     label:str = "OCCUPIED",
                     editable:bool = True):
     global sections
-    global logging
     logging.info ("Section "+str(section_id)+": Creating Track Occupancy Section")
     # Find and store the root window (when the first signal is created)
     if common.root_window is None: common.find_root_window(canvas)
     # Verify that a section with the same ID does not already exist
     if section_exists(section_id):
         logging.error ("Section "+str(section_id)+": Section already exists")
     elif section_id < 1:
@@ -270,25 +267,24 @@
         # Set the label to the loaded_label (loaded_label will be 'None' if no data was loaded)
         if loaded_state["labeltext"]:
             sections[str(section_id)]["labeltext"] = loaded_state["labeltext"]
             sections[str(section_id)]["button1"]["text"] = loaded_state["labeltext"]
         # Toggle the section if OCCUPIED (loaded_state_occupied will be 'None' if no data was loaded)
         if loaded_state["occupied"]: toggle_section(section_id)
         # Publish the initial state to the broker (for other nodes to consume). Note that changes will only
-        # be published if the MQTT interface has been configured for publishing updates for this track section
+        # only be published if the MQTT interface has been configured for publishing updates for this track
+        # section. This allows publish/subscribe to be configured prior to track section creation
         send_mqtt_section_updated_event(section_id) 
-
     return()
 
 # -------------------------------------------------------------------------
 # Public API function to Return the current state of the section
 # -------------------------------------------------------------------------
 
 def section_occupied (section_id:Union[int,str]):
-    global logging
     # Validate the section exists
     if not section_exists(section_id):
         logging.error ("Section "+str(section_id)+": section_occupied - Section does not exist")
         occupied = False
     elif not sections[str(section_id)]["occupied"]:   
         occupied = False
     else:
@@ -296,29 +292,27 @@
     return(occupied)
 
 # -------------------------------------------------------------------------
 # Public API function to Return the current label of the section (train identifier)
 # -------------------------------------------------------------------------
 
 def section_label (section_id:Union[int,str]):
-    global logging
     # Validate the section exists
     if not section_exists(section_id):
         logging.error ("Section "+str(section_id)+": section_label - Section does not exist")
         section_label=None
     else:
         section_label = sections[str(section_id)]["labeltext"]
     return(section_label)
 
 # -------------------------------------------------------------------------
 # Public API function to Set a section to OCCUPIED (and optionally update the label)
 # -------------------------------------------------------------------------
 
 def set_section_occupied (section_id:int,label:str=None, publish:bool=True):
-    global logging
     # Validate the section exists
     if not section_exists(section_id):
         logging.error ("Section "+str(section_id)+": set_section_occupied - Section does not exist")
     else:
         if not section_occupied(section_id):
             # Need to toggle the section - ALSO update the label if that has been changed
             if label is not None and sections[str(section_id)]["labeltext"] != label:
@@ -338,15 +332,14 @@
     return()
 
 # -------------------------------------------------------------------------
 # Public API function to Set a section to CLEAR (returns the label)
 # -------------------------------------------------------------------------
 
 def clear_section_occupied (section_id:int, label:str=None, publish:bool=True):
-    global logging
     # Validate the section exists
     if not section_exists(section_id):
         logging.error ("Section "+str(section_id)+": clear_section_occupied - Section does not exist")
         section_label = ""
     elif section_occupied(section_id):
         # Need to toggle the section - ALSO update the label if that has been changed
         if label is not None and sections[str(section_id)]["labeltext"] != label:
@@ -368,47 +361,49 @@
 #-----------------------------------------------------------------------------------------------
 # Public API Function to "subscribe" to section updates published by remote MQTT "Node"
 #-----------------------------------------------------------------------------------------------
 
 def subscribe_to_section_updates (node:str,sec_callback,*sec_ids:int):    
     global sections
     for sec_id in sec_ids:
-        mqtt_interface.subscribe_to_mqtt_messages("section_updated_event",node,sec_id,
-                                                  handle_mqtt_section_updated_event)
         # Create a dummy section object to hold the state of the remote track occupancy section
         # The Identifier for a remote Section is a string combining the the Node-ID and Section-ID
         section_identifier = mqtt_interface.create_remote_item_identifier(sec_id,node)
         if not section_exists(section_identifier):
             sections[section_identifier] = {}
             sections[section_identifier]["occupied"] = False
             sections[section_identifier]["labeltext"] = "OCCUPIED"
             sections[section_identifier]["extcallback"] = sec_callback
+            # Subscribe to updates from the remote section
+            mqtt_interface.subscribe_to_mqtt_messages("section_updated_event",node,sec_id,
+                                                  handle_mqtt_section_updated_event)
     return()
 
 #-----------------------------------------------------------------------------------------------
 # Public API Function to set configure a section to publish state changes to remote MQTT nodes
 #-----------------------------------------------------------------------------------------------
 
 def set_sections_to_publish_state(*sec_ids:int):    
-    global logging
     global list_of_sections_to_publish
     for sec_id in sec_ids:
         logging.info("MQTT-Client: Configuring section "+str(sec_id)+" to publish state changes via MQTT broker")
         if sec_id in list_of_sections_to_publish:
             logging.warning("MQTT-Client: Section "+str(sec_id)+" - is already configured to publish state changes")
         else:
             list_of_sections_to_publish.append(sec_id)
+            # Publish the initial state now this has been added to the list of sections to publish
+            # This allows the publish/subscribe functions to be configured after section creation
+            if str(sec_id) in sections.keys(): send_mqtt_section_updated_event(sec_id) 
     return()
 
 # --------------------------------------------------------------------------------
 # Callback for handling received MQTT messages from a remote track section
 # --------------------------------------------------------------------------------
 
 def handle_mqtt_section_updated_event(message):
-    global logging
     global sections
     if "sourceidentifier" in message.keys() and "occupied" in message.keys() and "labeltext" in message.keys():
         section_identifier = message["sourceidentifier"]
         sections[section_identifier]["occupied"] = message["occupied"]
         sections[section_identifier]["labeltext"] = message["labeltext"]
         logging.info("Section "+section_identifier+": State update from remote section ***************************")
         # Make the external callback (if one has been defined)
@@ -435,29 +430,56 @@
 # This is used by the schematic editor for changing section types where we delete the existing
 # section with all its data and then recreate it (with the same ID) in its new configuration
 # ------------------------------------------------------------------------------------------
 
 def delete_section(section_id:int):
     global sections
     global entry_box_window
+    global list_of_sections_to_publish
     if section_exists(section_id):
         # If a text entry box is open then we need to destroy it
         if entry_box_window is not None:
             text_entry_box.destroy()
             sections[str(section_id)]["canvas"].delete(entry_box_window)
         # Delete all the tkinter canvas drawing objects associated with the section
         sections[str(section_id)]["canvas"].delete("section"+str(section_id))
         # Delete all the tkinter button objects created for the section
         sections[str(section_id)]["button1"].destroy()
+        # Delete the section from the list_of_sections_to_publish (if required)
+        if section_id in list_of_sections_to_publish:
+            list_of_sections_to_publish.remove(section_id)
         # Finally, delete the entry from the dictionary of sections
         del sections[str(section_id)]
     return()
 
 # ------------------------------------------------------------------------------------------
 # Non public API function to return the tkinter canvas 'tags' for the section
 # ------------------------------------------------------------------------------------------
 
 def get_tags(section_id:int):
     return("section"+str(section_id))
 
+# ------------------------------------------------------------------------------------------
+# Non public API function to reset the list of published/subscribed sections. Used by
+# the schematic editor for re-setting the MQTT configuration prior to re-configuring
+# via the set_sections_to_publish_state and subscribe_to_section_updates functions
+# ------------------------------------------------------------------------------------------
+
+def reset_mqtt_configuration():
+    global sections
+    global list_of_sections_to_publish
+    # We only need to clear the list to stop any further section events being published
+    list_of_sections_to_publish.clear()
+    # For subscriptions we unsubscribe from all topics associated with the message_type
+    mqtt_interface.unsubscribe_from_message_type("section_updated_event")
+    # Finally remove all "remote" sections from the dictionary of sections - these
+    # will be re-created if they are subsequently re-subscribed to. Note we don't iterate 
+    # through the dictionary of sections to remove items as it will change under us
+    new_sections = {}
+    for key in sections:
+        if mqtt_interface.split_remote_item_identifier(key) is not None:
+            new_sections[key] = sections[key]
+    sections = new_sections
+    return()
+
 ###############################################################################
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals/library/track_sensors.py` & `model-railway-signals-3.4.0/model_railway_signals/library/track_sensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,27 +86,25 @@
 # Internal function called each time the external sensor input is triggered
 # If the sensor is still within the timeout period (from the last time it
 # was triggered) then the timeout period will effectively be extended
 # If  not in the timouut period then the external callback will be made
 # -------------------------------------------------------------------------
 
 def track_sensor_triggered (gpio_channel:int):
-    
     global channels
-    global logging
     
     # Thread to "lock" the sensor for the specified timeout period
     def thread_to_timeout_sensor (channel):
         channels[str(channel)]["timeout_start"] = time.time()
         channels[str(channel)]["timeout_active"] = True
         while time.time() < channels[str(channel)]["timeout_start"] + channels[str(channel)]["timeout_value"]:
             time.sleep(0.001)
         channels[str(channel)]["timeout_active"] = False
         return()
-
+    
     # This is where the main code begins
     if not channel_mapped (gpio_channel):
         logging.error ("Sensor "+str(gpio_channel)+": Triggered sensor not mapped")
     else:
         if channels[str(gpio_channel)]["timeout_active"]:
             # If we are still in the timeout period then we want to extend it
             channels[str(gpio_channel)]["timeout_start"] = time.time()
@@ -162,19 +160,16 @@
 
 def create_track_sensor (sensor_id:int, gpio_channel:int,
                          sensor_callback = null_callback,
                          signal_passed:int = 0,
                          signal_approach:int = 0,
                          sensor_timeout:float = 3.0,
                          trigger_period:float = 0.001):
-    
     global channels 
-    global logging
     global raspberry_pi
-
     # Validate the parameters we have been given
     logging.info ("Sensor "+str(sensor_id)+": Creating track sensor mapping")
     if sensor_id < 1:
         logging.error ("Sensor "+str(sensor_id)+": Sensor ID must be greater than zero")
     elif channel_mapped(gpio_channel):
         logging.error ("Sensor "+str(sensor_id)+": Channel "+str(gpio_channel)+" is already mapped to another Sensor")
     elif gpio_channel < 4 or gpio_channel > 26 or gpio_channel == 14 or gpio_channel == 15:
@@ -208,18 +203,15 @@
     return() 
 
 # -------------------------------------------------------------------------
 # Externally called function to return the state of a sensor object 
 # -------------------------------------------------------------------------
 
 def track_sensor_active (sensor_id:int):
-
-    global logging
     global raspberry_pi
-    
     # A quick and dirty way of getting the code to run on Windows for development
     # As the Windows version of python doesn't include the RPi specific GPIO package
     if raspberry_pi:
         for channel in channels.keys():
             if channels[str(channel)]["sensor_id"] == sensor_id:
                 return not bool(GPIO.input(int(channel)))
         logging.error ("Sensor "+str(sensor_id)+": does not exist")
@@ -228,15 +220,14 @@
         return (False)
 
 # -------------------------------------------------------------------------
 # Function called on shutdown to set the gpio ports back to their defaults
 # -------------------------------------------------------------------------
 
 def gpio_shutdown():
-    global logging
     if raspberry_pi:
         logging.info ("GPIO: Restoring default settings")
         GPIO.setwarnings(False)
         GPIO.cleanup()
     return()
 
 # --------------------------------------------------------------------------------
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals.egg-info/PKG-INFO` & `model-railway-signals-3.4.0/model_railway_signals.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,50 @@
 Metadata-Version: 2.1
 Name: model-railway-signals
-Version: 3.3.0
+Version: 3.4.0
 Summary: Create your own DCC model railway signalling scheme
 Home-page: https://github.com/johnrm174/model-railway-signalling
 Author: johnrm174
 Author-email: johnrm17418@gmail.com
 License: GNU GENERAL PUBLIC LICENSE Version 2, June 1991
 Description: # model-railway-signalling
         
         A DCC model railway signalling system written in Python. Primarily intended for the Raspberry Pi, but 
         will also run on other platforms (albeit without some of the Raspberry-Pi specific interfacing functions). 
-        Most types of colour light signals, semaphore signals, and ground signals are supported.
+        * Enables schematics to be created with signals, points, track occupancy sections and block instruments
+        * Most types of colour light signals, semaphore signals, and ground signals are supported.
         * Interfaces with the Pi-SPROG DCC command station to drive the signals and points out on the layout
         * Uses the Raspberry Pi GPIO inputs to provide train detection in support of signalling automation
+        * Incorporates MQTT networking to allow multiple signalling applications to be linked for larger layouts
         
         ## Layout editor
         
-        From Release 3.0.0, the schematic editor application enables automated and interlocked layout signalling 
-        schemes to be designed and configured without the need to write any code. Note that the editor is in
+        The schematic editor application enables automated and interlocked layout signalling schemes to be
+        designed and configured via the UI without the need to write any code. Note that the editor is in
         active development so any comments and suggestions for future features are welcome.
         
-        What's supported in Release 3.3.0:
-        * Draw your layout schematic with lines, points, signals and track occupancy sections
-        * Define the DCC command sequences to drive the signals and points out on the layout
-        * Configure the signals and points to implement protototypical interlocking schemes
+        What's currently supported by the Editor:
+        * Draw your schematic with lines, points, signals, track occupancy sections and block instruments
+        * Define the DCC command sequences needed to drive the signals and points out on the layout
+        * Configure the signals, points and block instruments for protototypical interlocking
         * Configure GPIO sensors and track sections to provide a 'mimic' display of the layout
-        * Automation of signals as trains traverse the routes that have been configured
-        * Save and load your layout schematic and state between running sessions
-        * Block instruments - with interlocking of starting signals
-        * Popup error messages when things go wrong (reduced reliance on logs)
+        * Configure a level of automation for the signals as trains traverse the layout
+        
+        What's New in Release 3.4.0:
+        * Point and line colour selections - to enable colour coding of routes
+        * Line end-style selections - end-stops and arrow styles can now be specified
+        * Enhanced error/warning reporting via popups - reduced reliance on logs
+        * Layout 'info' function (under Help) allows you to add notes for your layout
+        * Fixed issue when selecting objects if Canvas is scrolled within the main window
+        * Various window geometry improvements to keep key UI elements visible on resizing
+        * Track section occupancy logic corrected for passing shunt-ahead ground signals
         
         What's coming soon:
         * MQTT networking (for linking layouts)
-        * Application documentation
+        * Better pplication documentation
         
         Any bug reports and feedback you may have would be gratefully appreciated - specifically:
         * What aspects are intuitive? What aspects aren't?
         * What aspects do you particularly like?
         * What aspects particularly irritate you?
         
         There are some example layout files in the 'configuration_examples' folder.
```

### Comparing `model-railway-signals-3.3.0/model_railway_signals.egg-info/SOURCES.txt` & `model-railway-signals-3.4.0/model_railway_signals.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 model_railway_signals.egg-info/SOURCES.txt
 model_railway_signals.egg-info/dependency_links.txt
 model_railway_signals.egg-info/requires.txt
 model_railway_signals.egg-info/top_level.txt
 model_railway_signals/editor/__init__.py
 model_railway_signals/editor/common.py
 model_railway_signals/editor/configure_instrument.py
+model_railway_signals/editor/configure_line.py
 model_railway_signals/editor/configure_point.py
 model_railway_signals/editor/configure_section.py
 model_railway_signals/editor/configure_signal.py
 model_railway_signals/editor/configure_signal_tab1.py
 model_railway_signals/editor/configure_signal_tab2.py
 model_railway_signals/editor/configure_signal_tab3.py
 model_railway_signals/editor/editor.py
@@ -27,23 +28,28 @@
 model_railway_signals/editor/objects/objects_common.py
 model_railway_signals/editor/objects/objects_instruments.py
 model_railway_signals/editor/objects/objects_lines.py
 model_railway_signals/editor/objects/objects_points.py
 model_railway_signals/editor/objects/objects_sections.py
 model_railway_signals/editor/objects/objects_signals.py
 model_railway_signals/editor/resources/__init__.py
-model_railway_signals/editor/resources/block_instrument.png
-model_railway_signals/editor/resources/colour_light.png
-model_railway_signals/editor/resources/ground_disc.png
-model_railway_signals/editor/resources/ground_position.png
-model_railway_signals/editor/resources/left_hand_point.png
+model_railway_signals/editor/resources/arrow1.png
+model_railway_signals/editor/resources/arrow2.png
+model_railway_signals/editor/resources/arrow3.png
+model_railway_signals/editor/resources/arrow4.png
+model_railway_signals/editor/resources/colourlight.png
+model_railway_signals/editor/resources/endstop.png
+model_railway_signals/editor/resources/grounddisc.png
+model_railway_signals/editor/resources/groundpos.png
+model_railway_signals/editor/resources/instrument.png
+model_railway_signals/editor/resources/lhpoint.png
 model_railway_signals/editor/resources/line.png
-model_railway_signals/editor/resources/right_hand_point.png
+model_railway_signals/editor/resources/rhpoint.png
+model_railway_signals/editor/resources/section.png
 model_railway_signals/editor/resources/semaphore.png
-model_railway_signals/editor/resources/track_section.png
 model_railway_signals/library/__init__.py
 model_railway_signals/library/block_instruments.py
 model_railway_signals/library/common.py
 model_railway_signals/library/dcc_control.py
 model_railway_signals/library/file_interface.py
 model_railway_signals/library/mqtt_interface.py
 model_railway_signals/library/pi_sprog_interface.py
```

### Comparing `model-railway-signals-3.3.0/setup.py` & `model-railway-signals-3.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="model-railway-signals",
-    version="3.3.0",
+    version="3.4.0",
     packages=find_packages(),
     include_package_data=True,
     description="Create your own DCC model railway signalling scheme",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/johnrm174/model-railway-signalling",
     author="johnrm174",
```

