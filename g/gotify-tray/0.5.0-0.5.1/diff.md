# Comparing `tmp/gotify-tray-0.5.0.tar.gz` & `tmp/gotify-tray-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gotify-tray-0.5.0.tar", last modified: Sat May 27 22:42:56 2023, max compression
+gzip compressed data, was "gotify-tray-0.5.1.tar", last modified: Sun Jun 18 15:35:37 2023, max compression
```

## Comparing `gotify-tray-0.5.0.tar` & `gotify-tray-0.5.1.tar`

### file list

```diff
@@ -1,93 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:56.939483 gotify-tray-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-27 22:42:56.939483 gotify-tray-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:56.923482 gotify-tray-0.5.0/gotify_tray/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:56.923482 gotify-tray-0.5.0/gotify_tray/database/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/database/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/database/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/database/default_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/database/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/database/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:56.927482 gotify-tray-0.5.0/gotify_tray/gotify/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gotify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gotify/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gotify/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gotify/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:56.927482 gotify-tray-0.5.0/gotify_tray/gui/
--rw-r--r--   0 runner    (1001) docker     (123)    15871 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/MainApplication.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:56.927482 gotify-tray-0.5.0/gotify_tray/gui/designs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/designs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/designs/widget_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/designs/widget_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/designs/widget_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/designs/widget_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:56.931482 gotify-tray-0.5.0/gotify_tray/gui/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   346772 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/images/gotify-small-macos.png
--rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/images/gotify-small.png
--rw-r--r--   0 runner    (1001) docker     (123)    73216 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/images/logo-macos.ico
--rw-r--r--   0 runner    (1001) docker     (123)   135098 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/images/logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)   339880 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/images/tray-error-macos.png
--rw-r--r--   0 runner    (1001) docker     (123)    17860 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/images/tray-error.png
--rw-r--r--   0 runner    (1001) docker     (123)   341637 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/images/tray-macos.png
--rw-r--r--   0 runner    (1001) docker     (123)   341277 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/images/tray-unread-macos.png
--rw-r--r--   0 runner    (1001) docker     (123)    17854 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/images/tray-unread.png
--rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/images/tray.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:56.931482 gotify-tray-0.5.0/gotify_tray/gui/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/models/ApplicationModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/models/MessagesModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:56.935483 gotify-tray-0.5.0/gotify_tray/gui/themes/
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:56.935483 gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/palette.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/refresh.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/status_active.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/status_connecting.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/status_error.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/status_inactive.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/style.qss
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/trashcan.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:56.935483 gotify-tray-0.5.0/gotify_tray/gui/themes/default/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/default/palette.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/default/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:56.939483 gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/palette.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/refresh.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/status_active.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/status_connecting.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/status_error.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/status_inactive.svg
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/style.qss
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/trashcan.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:56.939483 gotify-tray-0.5.0/gotify_tray/gui/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/widgets/ImagePopup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/widgets/MainWindow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/widgets/MessageWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/widgets/ServerInfoDialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/widgets/SettingsDialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/widgets/StatusWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/widgets/Tray.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/gui/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/gotify_tray/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 22:42:56.923482 gotify-tray-0.5.0/gotify_tray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-27 22:42:56.000000 gotify-tray-0.5.0/gotify_tray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-27 22:42:56.000000 gotify-tray-0.5.0/gotify_tray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 22:42:56.000000 gotify-tray-0.5.0/gotify_tray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-27 22:42:56.000000 gotify-tray-0.5.0/gotify_tray.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 22:42:56.000000 gotify-tray-0.5.0/gotify_tray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-27 22:42:56.000000 gotify-tray-0.5.0/gotify_tray.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 22:42:56.939483 gotify-tray-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-27 22:42:24.000000 gotify-tray-0.5.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:35:37.718039 gotify-tray-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-18 15:35:37.718039 gotify-tray-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:35:37.702040 gotify-tray-0.5.1/gotify_tray/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:35:37.706040 gotify-tray-0.5.1/gotify_tray/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/database/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/database/default_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/database/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/database/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:35:37.706040 gotify-tray-0.5.1/gotify_tray/gotify/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gotify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gotify/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gotify/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gotify/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:35:37.706040 gotify-tray-0.5.1/gotify_tray/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)    16073 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/MainApplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:35:37.710039 gotify-tray-0.5.1/gotify_tray/gui/designs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/designs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/designs/widget_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/designs/widget_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/designs/widget_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/designs/widget_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:35:37.714039 gotify-tray-0.5.1/gotify_tray/gui/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   346772 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/images/gotify-small-macos.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/images/gotify-small.png
+-rw-r--r--   0 runner    (1001) docker     (123)    73216 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/images/logo-macos.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   135098 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/images/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   339880 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/images/tray-error-macos.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17860 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/images/tray-error.png
+-rw-r--r--   0 runner    (1001) docker     (123)   341637 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/images/tray-macos.png
+-rw-r--r--   0 runner    (1001) docker     (123)   341277 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/images/tray-unread-macos.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17854 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/images/tray-unread.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/images/tray.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:35:37.714039 gotify-tray-0.5.1/gotify_tray/gui/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/models/ApplicationModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/models/MessagesModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:35:37.714039 gotify-tray-0.5.1/gotify_tray/gui/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/themes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/themes/base.qss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:35:37.714039 gotify-tray-0.5.1/gotify_tray/gui/themes/dark/
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/themes/dark/refresh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/themes/dark/status_active.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/themes/dark/status_connecting.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/themes/dark/status_error.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/themes/dark/status_inactive.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/themes/dark/style.qss
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/themes/dark/trashcan.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:35:37.714039 gotify-tray-0.5.1/gotify_tray/gui/themes/light/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/themes/light/refresh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/themes/light/status_active.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/themes/light/status_connecting.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/themes/light/status_error.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/themes/light/status_inactive.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/themes/light/style.qss
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/themes/light/trashcan.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:35:37.718039 gotify-tray-0.5.1/gotify_tray/gui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/widgets/ImagePopup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7712 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/widgets/MainWindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/widgets/MessageWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/widgets/ServerInfoDialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/widgets/SettingsDialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/widgets/StatusWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/widgets/Tray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/gui/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/gotify_tray/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:35:37.702040 gotify-tray-0.5.1/gotify_tray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-18 15:35:37.000000 gotify-tray-0.5.1/gotify_tray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-18 15:35:37.000000 gotify-tray-0.5.1/gotify_tray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 15:35:37.000000 gotify-tray-0.5.1/gotify_tray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 15:35:37.000000 gotify-tray-0.5.1/gotify_tray.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-18 15:35:37.000000 gotify-tray-0.5.1/gotify_tray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 15:35:37.000000 gotify-tray-0.5.1/gotify_tray.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 15:35:37.718039 gotify-tray-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-18 15:35:10.000000 gotify-tray-0.5.1/version.txt
```

### Comparing `gotify-tray-0.5.0/LICENSE` & `gotify-tray-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/PKG-INFO` & `gotify-tray-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotify-tray
-Version: 0.5.0
+Version: 0.5.1
 Summary: A tray notification application for receiving messages from a Gotify server.
 Home-page: https://github.com/seird/gotify-tray
 Author: k.dries@protonmail.com
 Author-email: k.dries@protonmail.com
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `gotify-tray-0.5.0/README.md` & `gotify-tray-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/database/cache.py` & `gotify-tray-0.5.1/gotify_tray/database/cache.py`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/database/database.py` & `gotify-tray-0.5.1/gotify_tray/database/database.py`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/database/default_settings.py` & `gotify-tray-0.5.1/gotify_tray/database/default_settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 from pathlib import Path
 
 from ..__version__ import __title__
 
 
 DEFAULT_SETTINGS = {
-    "theme": "automatic",
     "message/check_missed/notify": True,
     "locale": False,
     "logging/level": "Disabled",
     "export/path": os.path.join(
         Path.home(), f"{__title__.replace(' ', '-').lower()}-settings.bytes"
     ),
     "shortcuts/quit": "Ctrl+Q",
```

### Comparing `gotify-tray-0.5.0/gotify_tray/database/downloader.py` & `gotify-tray-0.5.1/gotify_tray/database/downloader.py`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/database/settings.py` & `gotify-tray-0.5.1/gotify_tray/database/settings.py`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/gotify/api.py` & `gotify-tray-0.5.1/gotify_tray/gotify/api.py`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/gotify/listener.py` & `gotify-tray-0.5.1/gotify_tray/gotify/listener.py`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/gotify/models.py` & `gotify-tray-0.5.1/gotify_tray/gotify/models.py`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/MainApplication.py` & `gotify-tray-0.5.1/gotify_tray/gui/MainApplication.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,27 +56,25 @@
         filename=os.path.join(logdir, f"{title}.log"),
         format="%(levelname)s > %(name)s > %(asctime)s > %(filename)20s:%(lineno)3s - %(funcName)20s() > %(message)s",
     )
 
 
 class MainApplication(QtWidgets.QApplication):
     def init_ui(self):
-        set_theme(self, settings.value("theme", type=str))
-
         self.gotify_client = gotify.GotifyClient(
             settings.value("Server/url", type=str),
             settings.value("Server/client_token", type=str),
         )
 
         self.downloader = Downloader()
 
         self.messages_model = MessagesModel()
         self.application_model = ApplicationModel()
 
-        self.main_window = MainWindow(self, self.application_model, self.messages_model)
+        self.main_window = MainWindow(self.application_model, self.messages_model)
         self.main_window.show()  # The initial .show() is necessary to get the correct sizes when adding MessageWigets
         QtCore.QTimer.singleShot(0, self.main_window.hide)
 
         self.refresh_applications()
 
         self.tray = Tray()
         self.tray.show()
@@ -93,14 +91,17 @@
         self.watchdog = ServerConnectionWatchdogTask(self.gotify_client)
 
         self.link_callbacks()
         self.init_shortcuts()
 
         self.watchdog.start()
 
+    def set_theme(self):
+        set_theme(self)
+
     def refresh_applications(self):
         self.messages_model.clear()
         self.application_model.clear()
 
         self.application_model.setItem(0, 0, ApplicationAllMessagesItem())
 
         self.get_applications_task = GetApplicationsTask(self.gotify_client)
@@ -171,30 +172,37 @@
         Abort any tasks that will result in new messages getting appended to messages_model
         """
         aborted_tasks = []
         for s in ["get_application_messages_task", "get_messages_task"]:
             if task := getattr(self, s, None):
                 task.abort()
                 aborted_tasks.append(task)
+                try:
+                    task.message.disconnect()
+                except TypeError:
+                    pass
         
         for task in aborted_tasks:
             task.wait()
 
     def application_selection_changed_callback(self, item: ApplicationModelItem | ApplicationAllMessagesItem):
+        self.main_window.disable_buttons()
         self.abort_get_messages_task()
         self.messages_model.clear()
 
         if isinstance(item, ApplicationModelItem):
             self.get_application_messages_task = GetApplicationMessagesTask(item.data(ApplicationItemDataRole.ApplicationRole).id, self.gotify_client)
             self.get_application_messages_task.message.connect(self.messages_model.append_message)
+            self.get_application_messages_task.finished.connect(self.main_window.enable_buttons)
             self.get_application_messages_task.start()
 
         elif isinstance(item, ApplicationAllMessagesItem):
             self.get_messages_task = GetMessagesTask(self.gotify_client)
             self.get_messages_task.message.connect(self.messages_model.append_message)
+            self.get_messages_task.finished.connect(self.main_window.enable_buttons)
             self.get_messages_task.start()
 
     def add_message_to_model(self, message: gotify.GotifyMessageModel, process: bool = True):
         if self.application_model.itemFromId(message.appid):
             application_index = self.main_window.currentApplicationIndex()
             if selected_application_item := self.application_model.itemFromIndex(application_index):
 
@@ -220,28 +228,28 @@
         else:
             logger.error(f"App id {message.appid} could not be found. Refreshing applications.")
             self.refresh_applications()
 
     def new_message_callback(self, message: gotify.GotifyMessageModel, process: bool = True):
         self.add_message_to_model(message, process=process)
 
-        # Change the tray icon to show there are unread notifications
-        if (
-            settings.value("tray/icon/unread", type=bool)
-            and not self.main_window.isActiveWindow()
-        ):
-            self.tray.set_icon_unread()
-
         # Don't show a notification if it's low priority or the window is active
         if (
             message.priority < settings.value("tray/notifications/priority", type=int)
             or self.main_window.isActiveWindow()
         ):
             return
 
+        # Change the tray icon to show there are unread notifications
+        if (
+            settings.value("tray/icon/unread", type=bool)
+            and not self.main_window.isActiveWindow()
+        ):
+            self.tray.set_icon_unread()
+
         # Get the application icon
         if (
             settings.value("tray/notifications/icon/show", type=bool)
             and (application_item := self.application_model.itemFromId(message.appid))
         ):
             icon = application_item.icon()
         else:
@@ -288,30 +296,29 @@
         else:
             logger.warning(f"Image {link} is not in the cache")
 
     def main_window_hidden_callback(self):
         if image_popup := getattr(self, "image_popup", None):
             image_popup.close()
 
-    def theme_change_requested_callback(self, theme: str):
+    def theme_change_requested_callback(self, *args):
         # Set the theme
-        set_theme(self, theme)
+        self.set_theme()
 
         # Update the main window icons
         self.main_window.set_icons()
 
         # Update the message widget icons
         for r in range(self.messages_model.rowCount()):
             message_widget: MessageWidget = self.main_window.listView_messages.indexWidget(self.messages_model.index(r, 0))
             message_widget.set_icons()
 
     def settings_callback(self):
-        settings_dialog = SettingsDialog(self)
+        settings_dialog = SettingsDialog()
         settings_dialog.quit_requested.connect(self.quit)
-        settings_dialog.theme_change_requested.connect(self.theme_change_requested_callback)
         accepted = settings_dialog.exec()
 
         if accepted and settings_dialog.settings_changed:
             settings_dialog.apply_settings()
 
         if settings_dialog.server_changed:
             # Restart the listener
@@ -352,15 +359,15 @@
         self.main_window.delete_all.connect(self.delete_all_messages_callback)
         self.main_window.application_selection_changed.connect(self.application_selection_changed_callback)
         self.main_window.delete_message.connect(self.delete_message_callback)
         self.main_window.image_popup.connect(self.image_popup_callback)
         self.main_window.hidden.connect(self.main_window_hidden_callback)
         self.main_window.activated.connect(self.tray.revert_icon)
         
-        self.styleHints().colorSchemeChanged.connect(lambda _: self.theme_change_requested_callback(settings.value("theme", type=str)))
+        self.styleHints().colorSchemeChanged.connect(self.theme_change_requested_callback)
 
         self.messages_model.rowsInserted.connect(self.main_window.display_message_widgets)
 
         self.watchdog.closed.connect(lambda: self.listener_closed_callback(0, 0))
 
     def init_shortcuts(self):
         self.shortcut_quit = QtGui.QShortcut(
@@ -390,14 +397,15 @@
 
 def start_gui():
     app = MainApplication(sys.argv)
     app.setApplicationName(title)
     app.setQuitOnLastWindowClosed(False)
     app.setWindowIcon(QtGui.QIcon(get_icon("gotify-small")))
     app.setStyle("fusion")
+    app.set_theme()
 
     init_logger(logger)
 
     # prevent multiple instances
     if (app.acquire_lock() or "--no-lock" in sys.argv) and verify_server():
         app.init_ui()
         sys.exit(app.exec())
```

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/designs/widget_main.py` & `gotify-tray-0.5.1/gotify_tray/gui/designs/widget_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 # Form implementation generated from reading ui file 'gotify_tray/gui/designs\widget_main.ui'
 #
-# Created by: PyQt6 UI code generator 6.1.0
+# Created by: PyQt6 UI code generator 6.5.0
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic6 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt6 import QtCore, QtGui, QtWidgets
 
 
 class Ui_MainWindow(object):
     def setupUi(self, MainWindow):
         MainWindow.setObjectName("MainWindow")
         MainWindow.resize(809, 647)
-        self.centralwidget = QtWidgets.QWidget(MainWindow)
+        self.centralwidget = QtWidgets.QWidget(parent=MainWindow)
         self.centralwidget.setObjectName("centralwidget")
         self.gridLayout = QtWidgets.QGridLayout(self.centralwidget)
         self.gridLayout.setContentsMargins(4, 4, 4, 4)
         self.gridLayout.setObjectName("gridLayout")
-        self.splitter = QtWidgets.QSplitter(self.centralwidget)
+        self.splitter = QtWidgets.QSplitter(parent=self.centralwidget)
         self.splitter.setOrientation(QtCore.Qt.Orientation.Horizontal)
         self.splitter.setObjectName("splitter")
-        self.listView_applications = QtWidgets.QListView(self.splitter)
+        self.listView_applications = QtWidgets.QListView(parent=self.splitter)
         self.listView_applications.setEditTriggers(QtWidgets.QAbstractItemView.EditTrigger.NoEditTriggers)
         self.listView_applications.setObjectName("listView_applications")
-        self.verticalLayoutWidget = QtWidgets.QWidget(self.splitter)
+        self.verticalLayoutWidget = QtWidgets.QWidget(parent=self.splitter)
         self.verticalLayoutWidget.setObjectName("verticalLayoutWidget")
         self.verticalLayout_2 = QtWidgets.QVBoxLayout(self.verticalLayoutWidget)
         self.verticalLayout_2.setContentsMargins(0, 0, 0, 0)
         self.verticalLayout_2.setObjectName("verticalLayout_2")
         self.horizontalLayout = QtWidgets.QHBoxLayout()
         self.horizontalLayout.setObjectName("horizontalLayout")
         spacerItem = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
         self.horizontalLayout.addItem(spacerItem)
-        self.label_application = QtWidgets.QLabel(self.verticalLayoutWidget)
+        self.label_application = QtWidgets.QLabel(parent=self.verticalLayoutWidget)
         self.label_application.setObjectName("label_application")
         self.horizontalLayout.addWidget(self.label_application)
         spacerItem1 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
         self.horizontalLayout.addItem(spacerItem1)
-        self.pb_refresh = QtWidgets.QPushButton(self.verticalLayoutWidget)
+        self.pb_refresh = QtWidgets.QPushButton(parent=self.verticalLayoutWidget)
         self.pb_refresh.setText("")
         self.pb_refresh.setObjectName("pb_refresh")
         self.horizontalLayout.addWidget(self.pb_refresh)
-        self.pb_delete_all = QtWidgets.QPushButton(self.verticalLayoutWidget)
+        self.pb_delete_all = QtWidgets.QPushButton(parent=self.verticalLayoutWidget)
         self.pb_delete_all.setText("")
         self.pb_delete_all.setObjectName("pb_delete_all")
         self.horizontalLayout.addWidget(self.pb_delete_all)
         self.verticalLayout_2.addLayout(self.horizontalLayout)
-        self.listView_messages = QtWidgets.QListView(self.verticalLayoutWidget)
+        self.listView_messages = QtWidgets.QListView(parent=self.verticalLayoutWidget)
         self.listView_messages.setAutoScroll(True)
         self.listView_messages.setEditTriggers(QtWidgets.QAbstractItemView.EditTrigger.NoEditTriggers)
         self.listView_messages.setVerticalScrollMode(QtWidgets.QAbstractItemView.ScrollMode.ScrollPerPixel)
         self.listView_messages.setObjectName("listView_messages")
         self.verticalLayout_2.addWidget(self.listView_messages)
         self.gridLayout.addWidget(self.splitter, 0, 0, 1, 1)
         MainWindow.setCentralWidget(self.centralwidget)
```

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/designs/widget_message.py` & `gotify-tray-0.5.1/gotify_tray/gui/designs/widget_message.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Form implementation generated from reading ui file 'gotify_tray/gui/designs\widget_message.ui'
 #
-# Created by: PyQt6 UI code generator 6.4.0
+# Created by: PyQt6 UI code generator 6.5.0
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic6 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt6 import QtCore, QtGui, QtWidgets
 
@@ -14,73 +14,73 @@
         Form.setObjectName("Form")
         Form.resize(454, 90)
         self.gridLayout = QtWidgets.QGridLayout(Form)
         self.gridLayout.setSizeConstraint(QtWidgets.QLayout.SizeConstraint.SetMinimumSize)
         self.gridLayout.setContentsMargins(0, 0, 0, 0)
         self.gridLayout.setHorizontalSpacing(0)
         self.gridLayout.setObjectName("gridLayout")
-        self.frame = QtWidgets.QFrame(Form)
+        self.frame = QtWidgets.QFrame(parent=Form)
         self.frame.setFrameShape(QtWidgets.QFrame.Shape.StyledPanel)
         self.frame.setFrameShadow(QtWidgets.QFrame.Shadow.Raised)
         self.frame.setObjectName("frame")
         self.gridLayout_frame = QtWidgets.QGridLayout(self.frame)
         self.gridLayout_frame.setSizeConstraint(QtWidgets.QLayout.SizeConstraint.SetMinimumSize)
         self.gridLayout_frame.setContentsMargins(0, 0, -1, 0)
         self.gridLayout_frame.setVerticalSpacing(3)
         self.gridLayout_frame.setObjectName("gridLayout_frame")
-        self.label_message = QtWidgets.QLabel(self.frame)
+        self.label_message = QtWidgets.QLabel(parent=self.frame)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Preferred, QtWidgets.QSizePolicy.Policy.MinimumExpanding)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.label_message.sizePolicy().hasHeightForWidth())
         self.label_message.setSizePolicy(sizePolicy)
         font = QtGui.QFont()
         font.setPointSize(11)
         self.label_message.setFont(font)
         self.label_message.setWordWrap(True)
         self.label_message.setOpenExternalLinks(True)
         self.label_message.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.LinksAccessibleByMouse|QtCore.Qt.TextInteractionFlag.TextSelectableByMouse)
         self.label_message.setObjectName("label_message")
         self.gridLayout_frame.addWidget(self.label_message, 4, 3, 1, 4)
-        self.pb_delete = QtWidgets.QPushButton(self.frame)
+        self.pb_delete = QtWidgets.QPushButton(parent=self.frame)
         self.pb_delete.setText("")
         self.pb_delete.setFlat(True)
         self.pb_delete.setObjectName("pb_delete")
         self.gridLayout_frame.addWidget(self.pb_delete, 1, 6, 1, 1)
         spacerItem = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Maximum, QtWidgets.QSizePolicy.Policy.Minimum)
         self.gridLayout_frame.addItem(spacerItem, 1, 4, 1, 1)
         spacerItem1 = QtWidgets.QSpacerItem(0, 2, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Fixed)
         self.gridLayout_frame.addItem(spacerItem1, 0, 3, 1, 4)
-        self.label_date = QtWidgets.QLabel(self.frame)
+        self.label_date = QtWidgets.QLabel(parent=self.frame)
         font = QtGui.QFont()
         font.setPointSize(11)
         self.label_date.setFont(font)
         self.label_date.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.LinksAccessibleByMouse|QtCore.Qt.TextInteractionFlag.TextSelectableByMouse)
         self.label_date.setObjectName("label_date")
         self.gridLayout_frame.addWidget(self.label_date, 1, 5, 1, 1)
-        self.label_title = QtWidgets.QLabel(self.frame)
+        self.label_title = QtWidgets.QLabel(parent=self.frame)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.label_title.sizePolicy().hasHeightForWidth())
         self.label_title.setSizePolicy(sizePolicy)
         font = QtGui.QFont()
         font.setPointSize(17)
         font.setBold(False)
         font.setWeight(50)
         self.label_title.setFont(font)
         self.label_title.setWordWrap(True)
         self.label_title.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.LinksAccessibleByMouse|QtCore.Qt.TextInteractionFlag.TextSelectableByMouse)
         self.label_title.setObjectName("label_title")
         self.gridLayout_frame.addWidget(self.label_title, 1, 3, 1, 1)
-        self.label_image = QtWidgets.QLabel(self.frame)
+        self.label_image = QtWidgets.QLabel(parent=self.frame)
         self.label_image.setText("")
         self.label_image.setObjectName("label_image")
         self.gridLayout_frame.addWidget(self.label_image, 1, 2, 1, 1)
-        self.label_priority = QtWidgets.QLabel(self.frame)
+        self.label_priority = QtWidgets.QLabel(parent=self.frame)
         self.label_priority.setMaximumSize(QtCore.QSize(6, 16777215))
         self.label_priority.setText("")
         self.label_priority.setObjectName("label_priority")
         self.gridLayout_frame.addWidget(self.label_priority, 0, 1, 5, 1)
         self.gridLayout.addWidget(self.frame, 0, 0, 1, 1)
 
         self.retranslateUi(Form)
```

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/designs/widget_server.py` & `gotify-tray-0.5.1/gotify_tray/gui/designs/widget_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 # Form implementation generated from reading ui file 'gotify_tray/gui/designs\widget_server.ui'
 #
-# Created by: PyQt6 UI code generator 6.1.0
+# Created by: PyQt6 UI code generator 6.5.0
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic6 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt6 import QtCore, QtGui, QtWidgets
 
 
 class Ui_Dialog(object):
     def setupUi(self, Dialog):
         Dialog.setObjectName("Dialog")
         Dialog.resize(300, 130)
         self.gridLayout = QtWidgets.QGridLayout(Dialog)
         self.gridLayout.setObjectName("gridLayout")
-        self.label_server_info = QtWidgets.QLabel(Dialog)
+        self.label_server_info = QtWidgets.QLabel(parent=Dialog)
         self.label_server_info.setText("")
         self.label_server_info.setObjectName("label_server_info")
         self.gridLayout.addWidget(self.label_server_info, 1, 1, 1, 2)
         self.formLayout = QtWidgets.QFormLayout()
         self.formLayout.setObjectName("formLayout")
-        self.label = QtWidgets.QLabel(Dialog)
+        self.label = QtWidgets.QLabel(parent=Dialog)
         self.label.setObjectName("label")
         self.formLayout.setWidget(0, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label)
-        self.line_url = QtWidgets.QLineEdit(Dialog)
+        self.line_url = QtWidgets.QLineEdit(parent=Dialog)
         self.line_url.setObjectName("line_url")
         self.formLayout.setWidget(0, QtWidgets.QFormLayout.ItemRole.FieldRole, self.line_url)
-        self.label_2 = QtWidgets.QLabel(Dialog)
+        self.label_2 = QtWidgets.QLabel(parent=Dialog)
         self.label_2.setObjectName("label_2")
         self.formLayout.setWidget(1, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_2)
-        self.line_token = QtWidgets.QLineEdit(Dialog)
+        self.line_token = QtWidgets.QLineEdit(parent=Dialog)
         self.line_token.setObjectName("line_token")
         self.formLayout.setWidget(1, QtWidgets.QFormLayout.ItemRole.FieldRole, self.line_token)
         self.gridLayout.addLayout(self.formLayout, 0, 1, 1, 5)
-        self.pb_test = QtWidgets.QPushButton(Dialog)
+        self.pb_test = QtWidgets.QPushButton(parent=Dialog)
         self.pb_test.setObjectName("pb_test")
         self.gridLayout.addWidget(self.pb_test, 1, 5, 1, 1)
-        self.buttonBox = QtWidgets.QDialogButtonBox(Dialog)
+        self.buttonBox = QtWidgets.QDialogButtonBox(parent=Dialog)
         self.buttonBox.setOrientation(QtCore.Qt.Orientation.Horizontal)
         self.buttonBox.setStandardButtons(QtWidgets.QDialogButtonBox.StandardButton.Cancel|QtWidgets.QDialogButtonBox.StandardButton.Ok)
         self.buttonBox.setObjectName("buttonBox")
         self.gridLayout.addWidget(self.buttonBox, 2, 5, 1, 1)
         spacerItem = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
         self.gridLayout.addItem(spacerItem, 1, 3, 1, 1)
-        self.pb_import = QtWidgets.QPushButton(Dialog)
+        self.pb_import = QtWidgets.QPushButton(parent=Dialog)
         self.pb_import.setMaximumSize(QtCore.QSize(30, 16777215))
         self.pb_import.setObjectName("pb_import")
         self.gridLayout.addWidget(self.pb_import, 1, 4, 1, 1)
 
         self.retranslateUi(Dialog)
         self.buttonBox.accepted.connect(Dialog.accept) # type: ignore
         self.buttonBox.rejected.connect(Dialog.reject) # type: ignore
```

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/designs/widget_settings.py` & `gotify-tray-0.5.1/gotify_tray/gui/designs/widget_settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,221 +1,210 @@
 # Form implementation generated from reading ui file 'gotify_tray/gui/designs\widget_settings.ui'
 #
-# Created by: PyQt6 UI code generator 6.4.0
+# Created by: PyQt6 UI code generator 6.5.0
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic6 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt6 import QtCore, QtGui, QtWidgets
 
 
 class Ui_Dialog(object):
     def setupUi(self, Dialog):
         Dialog.setObjectName("Dialog")
-        Dialog.resize(415, 450)
+        Dialog.resize(415, 420)
         self.gridLayout = QtWidgets.QGridLayout(Dialog)
         self.gridLayout.setObjectName("gridLayout")
-        self.buttonBox = QtWidgets.QDialogButtonBox(Dialog)
+        self.buttonBox = QtWidgets.QDialogButtonBox(parent=Dialog)
         self.buttonBox.setOrientation(QtCore.Qt.Orientation.Horizontal)
         self.buttonBox.setStandardButtons(QtWidgets.QDialogButtonBox.StandardButton.Apply|QtWidgets.QDialogButtonBox.StandardButton.Cancel|QtWidgets.QDialogButtonBox.StandardButton.Ok)
         self.buttonBox.setObjectName("buttonBox")
         self.gridLayout.addWidget(self.buttonBox, 1, 0, 1, 1)
-        self.tabWidget = QtWidgets.QTabWidget(Dialog)
+        self.tabWidget = QtWidgets.QTabWidget(parent=Dialog)
         self.tabWidget.setObjectName("tabWidget")
         self.tab_general = QtWidgets.QWidget()
         self.tab_general.setObjectName("tab_general")
         self.verticalLayout_4 = QtWidgets.QVBoxLayout(self.tab_general)
         self.verticalLayout_4.setObjectName("verticalLayout_4")
-        self.groupBox_notifications = QtWidgets.QGroupBox(self.tab_general)
+        self.groupBox_notifications = QtWidgets.QGroupBox(parent=self.tab_general)
         self.groupBox_notifications.setObjectName("groupBox_notifications")
         self.gridLayout_4 = QtWidgets.QGridLayout(self.groupBox_notifications)
         self.gridLayout_4.setObjectName("gridLayout_4")
-        self.label_notification_duration = QtWidgets.QLabel(self.groupBox_notifications)
+        self.label_notification_duration = QtWidgets.QLabel(parent=self.groupBox_notifications)
         self.label_notification_duration.setObjectName("label_notification_duration")
         self.gridLayout_4.addWidget(self.label_notification_duration, 1, 0, 1, 1)
-        self.spin_duration = QtWidgets.QSpinBox(self.groupBox_notifications)
+        self.spin_duration = QtWidgets.QSpinBox(parent=self.groupBox_notifications)
         self.spin_duration.setMinimum(500)
         self.spin_duration.setMaximum(30000)
         self.spin_duration.setSingleStep(100)
         self.spin_duration.setObjectName("spin_duration")
         self.gridLayout_4.addWidget(self.spin_duration, 1, 1, 1, 1)
-        self.cb_notification_click = QtWidgets.QCheckBox(self.groupBox_notifications)
+        self.cb_notification_click = QtWidgets.QCheckBox(parent=self.groupBox_notifications)
         self.cb_notification_click.setObjectName("cb_notification_click")
         self.gridLayout_4.addWidget(self.cb_notification_click, 3, 0, 1, 3)
-        self.label_notification_duration_ms = QtWidgets.QLabel(self.groupBox_notifications)
+        self.label_notification_duration_ms = QtWidgets.QLabel(parent=self.groupBox_notifications)
         self.label_notification_duration_ms.setObjectName("label_notification_duration_ms")
         self.gridLayout_4.addWidget(self.label_notification_duration_ms, 1, 2, 1, 1)
         spacerItem = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
         self.gridLayout_4.addItem(spacerItem, 0, 2, 1, 1)
-        self.cb_notify = QtWidgets.QCheckBox(self.groupBox_notifications)
+        self.cb_notify = QtWidgets.QCheckBox(parent=self.groupBox_notifications)
         self.cb_notify.setObjectName("cb_notify")
         self.gridLayout_4.addWidget(self.cb_notify, 2, 0, 1, 3)
-        self.spin_priority = QtWidgets.QSpinBox(self.groupBox_notifications)
+        self.spin_priority = QtWidgets.QSpinBox(parent=self.groupBox_notifications)
         self.spin_priority.setMinimum(1)
         self.spin_priority.setMaximum(10)
         self.spin_priority.setProperty("value", 5)
         self.spin_priority.setObjectName("spin_priority")
         self.gridLayout_4.addWidget(self.spin_priority, 0, 1, 1, 1)
-        self.label_notification_priority = QtWidgets.QLabel(self.groupBox_notifications)
+        self.label_notification_priority = QtWidgets.QLabel(parent=self.groupBox_notifications)
         self.label_notification_priority.setObjectName("label_notification_priority")
         self.gridLayout_4.addWidget(self.label_notification_priority, 0, 0, 1, 1)
-        self.cb_tray_icon_unread = QtWidgets.QCheckBox(self.groupBox_notifications)
+        self.cb_tray_icon_unread = QtWidgets.QCheckBox(parent=self.groupBox_notifications)
         self.cb_tray_icon_unread.setObjectName("cb_tray_icon_unread")
         self.gridLayout_4.addWidget(self.cb_tray_icon_unread, 4, 0, 1, 3)
         self.verticalLayout_4.addWidget(self.groupBox_notifications)
-        self.groupBox_2 = QtWidgets.QGroupBox(self.tab_general)
+        self.groupBox_2 = QtWidgets.QGroupBox(parent=self.tab_general)
         self.groupBox_2.setObjectName("groupBox_2")
         self.verticalLayout_2 = QtWidgets.QVBoxLayout(self.groupBox_2)
         self.verticalLayout_2.setObjectName("verticalLayout_2")
-        self.horizontalLayout_3 = QtWidgets.QHBoxLayout()
-        self.horizontalLayout_3.setObjectName("horizontalLayout_3")
-        self.label_theme = QtWidgets.QLabel(self.groupBox_2)
-        self.label_theme.setObjectName("label_theme")
-        self.horizontalLayout_3.addWidget(self.label_theme)
-        self.combo_theme = QtWidgets.QComboBox(self.groupBox_2)
-        self.combo_theme.setObjectName("combo_theme")
-        self.horizontalLayout_3.addWidget(self.combo_theme)
-        spacerItem1 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
-        self.horizontalLayout_3.addItem(spacerItem1)
-        self.verticalLayout_2.addLayout(self.horizontalLayout_3)
-        self.cb_priority_colors = QtWidgets.QCheckBox(self.groupBox_2)
+        self.cb_priority_colors = QtWidgets.QCheckBox(parent=self.groupBox_2)
         self.cb_priority_colors.setObjectName("cb_priority_colors")
         self.verticalLayout_2.addWidget(self.cb_priority_colors)
-        self.cb_locale = QtWidgets.QCheckBox(self.groupBox_2)
+        self.cb_locale = QtWidgets.QCheckBox(parent=self.groupBox_2)
         self.cb_locale.setObjectName("cb_locale")
         self.verticalLayout_2.addWidget(self.cb_locale)
         self.verticalLayout_4.addWidget(self.groupBox_2)
-        self.groupBox_server_info = QtWidgets.QGroupBox(self.tab_general)
+        self.groupBox_server_info = QtWidgets.QGroupBox(parent=self.tab_general)
         self.groupBox_server_info.setObjectName("groupBox_server_info")
         self.gridLayout_3 = QtWidgets.QGridLayout(self.groupBox_server_info)
         self.gridLayout_3.setObjectName("gridLayout_3")
-        self.pb_change_server_info = QtWidgets.QPushButton(self.groupBox_server_info)
+        self.pb_change_server_info = QtWidgets.QPushButton(parent=self.groupBox_server_info)
         self.pb_change_server_info.setObjectName("pb_change_server_info")
         self.gridLayout_3.addWidget(self.pb_change_server_info, 0, 0, 1, 1)
-        spacerItem2 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
-        self.gridLayout_3.addItem(spacerItem2, 0, 1, 1, 1)
+        spacerItem1 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
+        self.gridLayout_3.addItem(spacerItem1, 0, 1, 1, 1)
         self.verticalLayout_4.addWidget(self.groupBox_server_info)
-        spacerItem3 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
-        self.verticalLayout_4.addItem(spacerItem3)
+        spacerItem2 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
+        self.verticalLayout_4.addItem(spacerItem2)
         self.tabWidget.addTab(self.tab_general, "")
         self.tab_fonts = QtWidgets.QWidget()
         self.tab_fonts.setObjectName("tab_fonts")
         self.verticalLayout_5 = QtWidgets.QVBoxLayout(self.tab_fonts)
         self.verticalLayout_5.setObjectName("verticalLayout_5")
         self.horizontalLayout_5 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_5.setObjectName("horizontalLayout_5")
-        self.pb_reset_fonts = QtWidgets.QPushButton(self.tab_fonts)
+        self.pb_reset_fonts = QtWidgets.QPushButton(parent=self.tab_fonts)
         self.pb_reset_fonts.setObjectName("pb_reset_fonts")
         self.horizontalLayout_5.addWidget(self.pb_reset_fonts)
         self.verticalLayout_5.addLayout(self.horizontalLayout_5)
-        self.groupBox_fonts_message = QtWidgets.QGroupBox(self.tab_fonts)
+        self.groupBox_fonts_message = QtWidgets.QGroupBox(parent=self.tab_fonts)
         self.groupBox_fonts_message.setObjectName("groupBox_fonts_message")
         self.layout_fonts_message = QtWidgets.QVBoxLayout(self.groupBox_fonts_message)
         self.layout_fonts_message.setContentsMargins(4, 4, 4, 4)
         self.layout_fonts_message.setSpacing(6)
         self.layout_fonts_message.setObjectName("layout_fonts_message")
         self.horizontalLayout = QtWidgets.QHBoxLayout()
         self.horizontalLayout.setObjectName("horizontalLayout")
-        self.pb_font_message_title = QtWidgets.QPushButton(self.groupBox_fonts_message)
+        self.pb_font_message_title = QtWidgets.QPushButton(parent=self.groupBox_fonts_message)
         self.pb_font_message_title.setObjectName("pb_font_message_title")
         self.horizontalLayout.addWidget(self.pb_font_message_title)
-        self.pb_font_message_date = QtWidgets.QPushButton(self.groupBox_fonts_message)
+        self.pb_font_message_date = QtWidgets.QPushButton(parent=self.groupBox_fonts_message)
         self.pb_font_message_date.setObjectName("pb_font_message_date")
         self.horizontalLayout.addWidget(self.pb_font_message_date)
-        self.pb_font_message_content = QtWidgets.QPushButton(self.groupBox_fonts_message)
+        self.pb_font_message_content = QtWidgets.QPushButton(parent=self.groupBox_fonts_message)
         self.pb_font_message_content.setObjectName("pb_font_message_content")
         self.horizontalLayout.addWidget(self.pb_font_message_content)
         self.layout_fonts_message.addLayout(self.horizontalLayout)
         self.verticalLayout_5.addWidget(self.groupBox_fonts_message)
-        spacerItem4 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
-        self.verticalLayout_5.addItem(spacerItem4)
+        spacerItem3 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
+        self.verticalLayout_5.addItem(spacerItem3)
         self.tabWidget.addTab(self.tab_fonts, "")
         self.tab_advanced = QtWidgets.QWidget()
         self.tab_advanced.setObjectName("tab_advanced")
         self.verticalLayout = QtWidgets.QVBoxLayout(self.tab_advanced)
         self.verticalLayout.setObjectName("verticalLayout")
-        self.groupBox = QtWidgets.QGroupBox(self.tab_advanced)
+        self.groupBox = QtWidgets.QGroupBox(parent=self.tab_advanced)
         self.groupBox.setObjectName("groupBox")
         self.horizontalLayout_2 = QtWidgets.QHBoxLayout(self.groupBox)
         self.horizontalLayout_2.setObjectName("horizontalLayout_2")
-        self.pb_reset = QtWidgets.QPushButton(self.groupBox)
+        self.pb_reset = QtWidgets.QPushButton(parent=self.groupBox)
         self.pb_reset.setObjectName("pb_reset")
         self.horizontalLayout_2.addWidget(self.pb_reset)
-        self.pb_import = QtWidgets.QPushButton(self.groupBox)
+        self.pb_import = QtWidgets.QPushButton(parent=self.groupBox)
         self.pb_import.setObjectName("pb_import")
         self.horizontalLayout_2.addWidget(self.pb_import)
-        self.pb_export = QtWidgets.QPushButton(self.groupBox)
+        self.pb_export = QtWidgets.QPushButton(parent=self.groupBox)
         self.pb_export.setObjectName("pb_export")
         self.horizontalLayout_2.addWidget(self.pb_export)
         self.verticalLayout.addWidget(self.groupBox)
-        self.groupbox_image_popup = QtWidgets.QGroupBox(self.tab_advanced)
+        self.groupbox_image_popup = QtWidgets.QGroupBox(parent=self.tab_advanced)
         self.groupbox_image_popup.setCheckable(True)
         self.groupbox_image_popup.setObjectName("groupbox_image_popup")
         self.gridLayout_2 = QtWidgets.QGridLayout(self.groupbox_image_popup)
         self.gridLayout_2.setObjectName("gridLayout_2")
         self.horizontalLayout_4 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_4.setObjectName("horizontalLayout_4")
-        self.label = QtWidgets.QLabel(self.groupbox_image_popup)
+        self.label = QtWidgets.QLabel(parent=self.groupbox_image_popup)
         self.label.setObjectName("label")
         self.horizontalLayout_4.addWidget(self.label)
-        self.spin_popup_w = QtWidgets.QSpinBox(self.groupbox_image_popup)
+        self.spin_popup_w = QtWidgets.QSpinBox(parent=self.groupbox_image_popup)
         self.spin_popup_w.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.spin_popup_w.setMinimum(100)
         self.spin_popup_w.setMaximum(10000)
         self.spin_popup_w.setObjectName("spin_popup_w")
         self.horizontalLayout_4.addWidget(self.spin_popup_w)
-        self.label_2 = QtWidgets.QLabel(self.groupbox_image_popup)
+        self.label_2 = QtWidgets.QLabel(parent=self.groupbox_image_popup)
         self.label_2.setObjectName("label_2")
         self.horizontalLayout_4.addWidget(self.label_2)
-        self.spin_popup_h = QtWidgets.QSpinBox(self.groupbox_image_popup)
+        self.spin_popup_h = QtWidgets.QSpinBox(parent=self.groupbox_image_popup)
         self.spin_popup_h.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.spin_popup_h.setMinimum(100)
         self.spin_popup_h.setMaximum(10000)
         self.spin_popup_h.setObjectName("spin_popup_h")
         self.horizontalLayout_4.addWidget(self.spin_popup_h)
-        spacerItem5 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
-        self.horizontalLayout_4.addItem(spacerItem5)
+        spacerItem4 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
+        self.horizontalLayout_4.addItem(spacerItem4)
         self.gridLayout_2.addLayout(self.horizontalLayout_4, 0, 0, 1, 1)
         self.verticalLayout.addWidget(self.groupbox_image_popup)
-        self.groupBox_cache = QtWidgets.QGroupBox(self.tab_advanced)
+        self.groupBox_cache = QtWidgets.QGroupBox(parent=self.tab_advanced)
         self.groupBox_cache.setObjectName("groupBox_cache")
         self.horizontalLayout_6 = QtWidgets.QHBoxLayout(self.groupBox_cache)
         self.horizontalLayout_6.setObjectName("horizontalLayout_6")
-        self.pb_clear_cache = QtWidgets.QPushButton(self.groupBox_cache)
+        self.pb_clear_cache = QtWidgets.QPushButton(parent=self.groupBox_cache)
         self.pb_clear_cache.setObjectName("pb_clear_cache")
         self.horizontalLayout_6.addWidget(self.pb_clear_cache)
-        self.pb_open_cache_dir = QtWidgets.QPushButton(self.groupBox_cache)
+        self.pb_open_cache_dir = QtWidgets.QPushButton(parent=self.groupBox_cache)
         self.pb_open_cache_dir.setObjectName("pb_open_cache_dir")
         self.horizontalLayout_6.addWidget(self.pb_open_cache_dir)
-        self.label_cache = QtWidgets.QLabel(self.groupBox_cache)
+        self.label_cache = QtWidgets.QLabel(parent=self.groupBox_cache)
         self.label_cache.setObjectName("label_cache")
         self.horizontalLayout_6.addWidget(self.label_cache)
-        spacerItem6 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
-        self.horizontalLayout_6.addItem(spacerItem6)
+        spacerItem5 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
+        self.horizontalLayout_6.addItem(spacerItem5)
         self.verticalLayout.addWidget(self.groupBox_cache)
-        self.groupBox_logging = QtWidgets.QGroupBox(self.tab_advanced)
+        self.groupBox_logging = QtWidgets.QGroupBox(parent=self.tab_advanced)
         self.groupBox_logging.setObjectName("groupBox_logging")
         self.gridLayout_6 = QtWidgets.QGridLayout(self.groupBox_logging)
         self.gridLayout_6.setObjectName("gridLayout_6")
-        self.combo_logging = QtWidgets.QComboBox(self.groupBox_logging)
+        self.combo_logging = QtWidgets.QComboBox(parent=self.groupBox_logging)
         self.combo_logging.setObjectName("combo_logging")
         self.gridLayout_6.addWidget(self.combo_logging, 0, 1, 1, 1)
-        spacerItem7 = QtWidgets.QSpacerItem(190, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
-        self.gridLayout_6.addItem(spacerItem7, 0, 3, 1, 1)
-        self.pb_open_log = QtWidgets.QPushButton(self.groupBox_logging)
+        spacerItem6 = QtWidgets.QSpacerItem(190, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
+        self.gridLayout_6.addItem(spacerItem6, 0, 3, 1, 1)
+        self.pb_open_log = QtWidgets.QPushButton(parent=self.groupBox_logging)
         self.pb_open_log.setMaximumSize(QtCore.QSize(30, 16777215))
         self.pb_open_log.setObjectName("pb_open_log")
         self.gridLayout_6.addWidget(self.pb_open_log, 0, 2, 1, 1)
-        self.label_logging = QtWidgets.QLabel(self.groupBox_logging)
+        self.label_logging = QtWidgets.QLabel(parent=self.groupBox_logging)
         self.label_logging.setObjectName("label_logging")
         self.gridLayout_6.addWidget(self.label_logging, 0, 0, 1, 1)
         self.verticalLayout.addWidget(self.groupBox_logging)
-        spacerItem8 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
-        self.verticalLayout.addItem(spacerItem8)
+        spacerItem7 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
+        self.verticalLayout.addItem(spacerItem7)
         self.tabWidget.addTab(self.tab_advanced, "")
         self.gridLayout.addWidget(self.tabWidget, 0, 0, 1, 1)
 
         self.retranslateUi(Dialog)
         self.tabWidget.setCurrentIndex(0)
         self.buttonBox.accepted.connect(Dialog.accept) # type: ignore
         self.buttonBox.rejected.connect(Dialog.reject) # type: ignore
@@ -235,15 +224,14 @@
         self.label_notification_duration.setText(_translate("Dialog", "Notification duration:"))
         self.cb_notification_click.setText(_translate("Dialog", "Clicking the notification pop-up opens the main window"))
         self.label_notification_duration_ms.setText(_translate("Dialog", "ms"))
         self.cb_notify.setText(_translate("Dialog", "Show a notification for missed messages after reconnecting"))
         self.label_notification_priority.setText(_translate("Dialog", "Minimum priority to show notifications:"))
         self.cb_tray_icon_unread.setText(_translate("Dialog", "Change the tray icon color when there are unread notifications"))
         self.groupBox_2.setTitle(_translate("Dialog", "Interface"))
-        self.label_theme.setText(_translate("Dialog", "Theme:"))
         self.cb_priority_colors.setToolTip(_translate("Dialog", "4..7   -> medium\n"
 "8..10 -> high"))
         self.cb_priority_colors.setText(_translate("Dialog", "Show message priority colors"))
         self.cb_locale.setText(_translate("Dialog", "Display date in the system locale format"))
         self.groupBox_server_info.setTitle(_translate("Dialog", "Server info"))
         self.pb_change_server_info.setText(_translate("Dialog", "Change server info"))
         self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_general), _translate("Dialog", "General"))
```

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/images/gotify-small-macos.png` & `gotify-tray-0.5.1/gotify_tray/gui/images/gotify-small-macos.png`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/images/gotify-small.png` & `gotify-tray-0.5.1/gotify_tray/gui/images/gotify-small.png`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/images/logo-macos.ico` & `gotify-tray-0.5.1/gotify_tray/gui/images/logo-macos.ico`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/images/logo.ico` & `gotify-tray-0.5.1/gotify_tray/gui/images/logo.ico`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/images/tray-error-macos.png` & `gotify-tray-0.5.1/gotify_tray/gui/images/tray-error-macos.png`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/images/tray-error.png` & `gotify-tray-0.5.1/gotify_tray/gui/images/tray-error.png`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/images/tray-macos.png` & `gotify-tray-0.5.1/gotify_tray/gui/images/tray-macos.png`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/images/tray-unread-macos.png` & `gotify-tray-0.5.1/gotify_tray/gui/images/tray-unread-macos.png`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/images/tray-unread.png` & `gotify-tray-0.5.1/gotify_tray/gui/images/tray-unread.png`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/images/tray.png` & `gotify-tray-0.5.1/gotify_tray/gui/images/tray.png`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/models/ApplicationModel.py` & `gotify-tray-0.5.1/gotify_tray/gui/models/ApplicationModel.py`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/models/MessagesModel.py` & `gotify-tray-0.5.1/gotify_tray/gui/models/MessagesModel.py`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/refresh.svg` & `gotify-tray-0.5.1/gotify_tray/gui/themes/dark/refresh.svg`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/status_active.svg` & `gotify-tray-0.5.1/gotify_tray/gui/themes/dark/status_active.svg`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/status_connecting.svg` & `gotify-tray-0.5.1/gotify_tray/gui/themes/dark/status_connecting.svg`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/status_error.svg` & `gotify-tray-0.5.1/gotify_tray/gui/themes/dark/status_error.svg`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/themes/dark_purple/status_inactive.svg` & `gotify-tray-0.5.1/gotify_tray/gui/themes/dark/status_inactive.svg`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/refresh.svg` & `gotify-tray-0.5.1/gotify_tray/gui/themes/light/refresh.svg`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/status_active.svg` & `gotify-tray-0.5.1/gotify_tray/gui/themes/light/status_active.svg`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/status_connecting.svg` & `gotify-tray-0.5.1/gotify_tray/gui/themes/light/status_connecting.svg`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/status_error.svg` & `gotify-tray-0.5.1/gotify_tray/gui/themes/light/status_error.svg`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/themes/light_purple/status_inactive.svg` & `gotify-tray-0.5.1/gotify_tray/gui/themes/light/status_inactive.svg`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/widgets/ImagePopup.py` & `gotify-tray-0.5.1/gotify_tray/gui/widgets/ImagePopup.py`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/widgets/MainWindow.py` & `gotify-tray-0.5.1/gotify_tray/gui/widgets/MainWindow.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,40 +23,35 @@
     delete_all = QtCore.pyqtSignal(QtGui.QStandardItem)
     delete_message = QtCore.pyqtSignal(MessagesModelItem)
     application_selection_changed = QtCore.pyqtSignal(QtGui.QStandardItem)
     image_popup = QtCore.pyqtSignal(str, QtCore.QPoint)
     hidden = QtCore.pyqtSignal()
     activated = QtCore.pyqtSignal()
 
-    def __init__(
-        self, app: QtWidgets.QApplication,
-        application_model: ApplicationModel, messages_model: MessagesModel
-    ):
+    def __init__(self, application_model: ApplicationModel, messages_model: MessagesModel):
         super(MainWindow, self).__init__()
         self.setupUi(self)
 
         self.installEventFilter(self)
 
         self.setWindowTitle(__title__)
 
-        self.app = app
-
         self.application_model = application_model
         self.messages_model = messages_model
 
         self.listView_applications.setModel(application_model)
         self.listView_messages.setModel(messages_model)
 
         # Do not expand the applications listview when resizing
         self.splitter.setStretchFactor(0, 0)
         self.splitter.setStretchFactor(1, 1)
 
         # Do not collapse the message list
         self.splitter.setCollapsible(1, False)
-        self.status_widget = StatusWidget(app)
+        self.status_widget = StatusWidget()
         self.horizontalLayout.insertWidget(0, self.status_widget)
 
         self.set_icons()
 
         font_title = QtGui.QFont()
         if s := settings.value("MainWindow/font/application", type=str):
             font_title.fromString(s)
@@ -71,16 +66,16 @@
 
         self.restore_state()
 
         self.link_callbacks()
 
     def set_icons(self):
         # Set button icons
-        self.pb_refresh.setIcon(QtGui.QIcon(get_theme_file(self.app, "refresh.svg")))
-        self.pb_delete_all.setIcon(QtGui.QIcon(get_theme_file(self.app, "trashcan.svg")))
+        self.pb_refresh.setIcon(QtGui.QIcon(get_theme_file("refresh.svg")))
+        self.pb_delete_all.setIcon(QtGui.QIcon(get_theme_file("trashcan.svg")))
 
         # Resize the labels and icons
         size = settings.value("MainWindow/label/size", type=int)
         self.status_widget.setFixedSize(QtCore.QSize(size, size))
 
         size = settings.value("MainWindow/button/size", type=int)
         self.pb_refresh.setFixedSize(QtCore.QSize(size, size))
@@ -111,19 +106,19 @@
             if index := self.messages_model.index(i, 0, parent):
                 message_item = self.messages_model.itemFromIndex(index)
 
                 message: gotify.GotifyMessageModel = self.messages_model.data(index, MessageItemDataRole.MessageRole)
 
                 application_item = self.application_model.itemFromId(message.appid)
                 
-                message_widget = MessageWidget(self.app, self.listView_messages, message_item, icon=application_item.icon())
+                message_widget = MessageWidget(self.listView_messages, message_item, icon=application_item.icon())
                 message_widget.deletion_requested.connect(self.delete_message.emit)
                 message_widget.image_popup.connect(self.image_popup.emit)
                 
-                self.listView_messages.setIndexWidget(self.messages_model.indexFromItem(message_item), message_widget)
+                self.listView_messages.setIndexWidget(index, message_widget)
 
     def currentApplicationIndex(self) -> QtCore.QModelIndex:
         return self.listView_applications.selectionModel().currentIndex()
 
     def application_selection_changed_callback(
         self, current: QtCore.QModelIndex, previous: QtCore.QModelIndex
     ):
@@ -154,14 +149,22 @@
         self.listView_applications.clearSelection()
         self.listView_applications.setDisabled(True)
 
     def enable_applications(self):
         self.listView_applications.setEnabled(True)
         self.listView_applications.setCurrentIndex(self.application_model.index(0, 0))
 
+    def disable_buttons(self):
+        self.pb_delete_all.setDisabled(True)
+        self.pb_refresh.setDisabled(True)
+
+    def enable_buttons(self):
+        self.pb_delete_all.setEnabled(True)
+        self.pb_refresh.setEnabled(True)
+
     def bring_to_front(self):
         self.ensurePolished()
         self.setWindowState(
             self.windowState() & ~QtCore.Qt.WindowState.WindowMinimized
             | QtCore.Qt.WindowState.WindowActive
         )
         self.show()
```

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/widgets/MessageWidget.py` & `gotify-tray-0.5.1/gotify_tray/gui/widgets/MessageWidget.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,36 +2,33 @@
 
 from PyQt6 import QtCore, QtGui, QtWidgets
 
 from ..models.MessagesModel import MessageItemDataRole, MessagesModelItem
 from ..designs.widget_message import Ui_Form
 from gotify_tray.database import Downloader
 from gotify_tray.database import Settings
-from gotify_tray.utils import convert_links, get_image
+from gotify_tray.utils import convert_links, get_image, update_widget_property
 from gotify_tray.gui.themes import get_theme_file
 from gotify_tray.gotify.models import GotifyMessageModel
 
 
 settings = Settings("gotify-tray")
 
 
 class MessageWidget(QtWidgets.QWidget, Ui_Form):
     deletion_requested = QtCore.pyqtSignal(MessagesModelItem)
     image_popup = QtCore.pyqtSignal(str, QtCore.QPoint)
 
     def __init__(
         self,
-        app: QtWidgets.QApplication,
         parent: QtWidgets.QWidget,
         message_item: MessagesModelItem,
         icon: QtGui.QIcon | None = None,
     ):
         super(MessageWidget, self).__init__(parent)
-        self.app = app
-        self._parent = parent
         self.setupUi(self)
         self.setAutoFillBackground(True)
         self.message_item = message_item
         message: GotifyMessageModel = message_item.data(MessageItemDataRole.MessageRole)
 
         # Fonts
         self.set_fonts()
@@ -98,25 +95,24 @@
             font_content.fromString(s)
 
         self.label_title.setFont(font_title)
         self.label_date.setFont(font_date)
         self.label_message.setFont(font_content)
 
     def set_icons(self):
-        self.pb_delete.setIcon(QtGui.QIcon(get_theme_file(self.app, "trashcan.svg")))
-        self.pb_delete.setIconSize(QtCore.QSize(24, 24))
+        self.pb_delete.setIcon(QtGui.QIcon(get_theme_file("trashcan.svg")))
 
     def set_message_image(self, filename: str):
         pixmap = QtGui.QPixmap(filename)
 
         # Make sure the image fits within the listView
         W = settings.value("MessageWidget/content_image/W_percentage", type=float)
         H = settings.value("MessageWidget/content_image/H_percentage", type=float)
-        W *= self._parent.width() - self.label_image.width()
-        H *= self._parent.height()
+        W *= self.parent().width() - self.label_image.width()
+        H *= self.parent().height()
 
         if pixmap.width() > W or pixmap.height() > H:
             pixmap = pixmap.scaled(
                 QtCore.QSize(int(W), int(H)),
                 aspectRatioMode=QtCore.Qt.AspectRatioMode.KeepAspectRatio,
                 transformMode=QtCore.Qt.TransformationMode.SmoothTransformation,
             )
@@ -125,17 +121,17 @@
 
     def set_priority_color(self, priority: int):
         if not settings.value("MessageWidget/priority_color", type=bool):
             self.label_priority.setFixedWidth(0) # set width to 0 instead of hiding, so we still get the content margins
             return
 
         if priority >= 4 and priority <= 7:
-                self.label_priority.setStyleSheet("background-color: rgba(230, 126, 34, 0.7);")
+            update_widget_property(self.label_priority, "priority", "medium")
         elif priority > 7:
-            self.label_priority.setStyleSheet("background-color: #e74c3c;")
+            update_widget_property(self.label_priority, "priority", "high")
 
     def link_hovered_callback(self, link: str):
         if not settings.value("ImagePopup/enabled", type=bool):
             return
 
         qurl = QtCore.QUrl(link)
         _, ext = os.path.splitext(qurl.fileName())
```

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/widgets/ServerInfoDialog.py` & `gotify-tray-0.5.1/gotify_tray/gui/widgets/ServerInfoDialog.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 
 from gotify_tray.database import Settings
 from gotify_tray.gotify.models import GotifyVersionModel
 from gotify_tray.tasks import ImportSettingsTask, VerifyServerInfoTask
+from gotify_tray.utils import update_widget_property
 from PyQt6 import QtWidgets
 
 from ..designs.widget_server import Ui_Dialog
 
 
 settings = Settings("gotify-tray")
 
@@ -20,17 +21,17 @@
         self.line_url.setText(url)
         self.line_token.setText(token)
         self.buttonBox.button(QtWidgets.QDialogButtonBox.StandardButton.Ok).setDisabled(True)
         self.pb_import.setVisible(enable_import)
         self.link_callbacks()
 
     def test_server_info(self):
-        self.pb_test.setStyleSheet("")
-        self.line_url.setStyleSheet("")
-        self.line_token.setStyleSheet("")
+        update_widget_property(self.pb_test, "state", "")
+        update_widget_property(self.line_url, "state", "")
+        update_widget_property(self.line_token, "state", "")
         self.label_server_info.clear()
 
         url = self.line_url.text()
         client_token = self.line_token.text()
         if not url or not client_token:
             return
 
@@ -39,48 +40,42 @@
 
         self.task = VerifyServerInfoTask(url, client_token)
         self.task.success.connect(self.server_info_success)
         self.task.incorrect_token.connect(self.incorrect_token_callback)
         self.task.incorrect_url.connect(self.incorrect_url_callback)
         self.task.start()
 
-    def update_widget_state(self, widget: QtWidgets.QWidget, state: str):
-        widget.setProperty("state", state)
-        widget.style().unpolish(widget)
-        widget.style().polish(widget)
-        widget.update()
-
     def server_info_success(self, version: GotifyVersionModel):
         self.pb_test.setEnabled(True)
         self.label_server_info.setText(f"Version: {version.version}")
-        self.update_widget_state(self.pb_test, "success")
-        self.update_widget_state(self.line_token, "success")
-        self.update_widget_state(self.line_url, "success")
+        update_widget_property(self.pb_test, "state", "success")
+        update_widget_property(self.line_token, "state", "success")
+        update_widget_property(self.line_url, "state", "success")
         self.buttonBox.button(QtWidgets.QDialogButtonBox.StandardButton.Ok).setEnabled(True)
         self.buttonBox.button(QtWidgets.QDialogButtonBox.StandardButton.Ok).setFocus()
 
     def incorrect_token_callback(self, version: GotifyVersionModel):
         self.pb_test.setEnabled(True)
         self.label_server_info.setText(f"Version: {version.version}")
-        self.update_widget_state(self.pb_test, "failed")
-        self.update_widget_state(self.line_token, "failed")
-        self.update_widget_state(self.line_url, "success")
+        update_widget_property(self.pb_test, "state", "failed")
+        update_widget_property(self.line_token, "state", "failed")
+        update_widget_property(self.line_url, "state", "success")
         self.line_token.setFocus()
 
     def incorrect_url_callback(self):
         self.pb_test.setEnabled(True)
         self.label_server_info.clear()
-        self.update_widget_state(self.pb_test, "failed")
-        self.update_widget_state(self.line_token, "success")
-        self.update_widget_state(self.line_url, "failed")
+        update_widget_property(self.pb_test, "state", "failed")
+        update_widget_property(self.line_token, "state", "success")
+        update_widget_property(self.line_url, "state", "failed")
         self.line_url.setFocus()
 
     def input_changed_callback(self):
         self.buttonBox.button(QtWidgets.QDialogButtonBox.StandardButton.Ok).setDisabled(True)
-        self.update_widget_state(self.pb_test, "")
+        update_widget_property(self.pb_test, "state", "")
 
     def import_success_callback(self):
         self.line_url.setText(settings.value("Server/url", type=str))
         self.line_token.setText(settings.value("Server/client_token"))
 
     def import_callback(self):
         fname = QtWidgets.QFileDialog.getOpenFileName(
```

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/widgets/SettingsDialog.py` & `gotify-tray-0.5.1/gotify_tray/gui/widgets/SettingsDialog.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,35 +9,31 @@
 from gotify_tray.utils import get_icon, verify_server, open_file
 from gotify_tray.tasks import (
     ExportSettingsTask,
     ImportSettingsTask,
     CacheSizeTask,
     ClearCacheTask,
 )
-from gotify_tray.gui.themes import get_themes
 from PyQt6 import QtCore, QtGui, QtWidgets
 
 from ..designs.widget_settings import Ui_Dialog
 
 
 logger = logging.getLogger("gotify-tray")
 settings = Settings("gotify-tray")
 
 
 class SettingsDialog(QtWidgets.QDialog, Ui_Dialog):
     quit_requested = QtCore.pyqtSignal()
-    theme_change_requested = QtCore.pyqtSignal(str)
 
-    def __init__(self, app: QtWidgets.QApplication):
+    def __init__(self):
         super(SettingsDialog, self).__init__()
         self.setupUi(self)
         self.setWindowTitle("Settings")
         
-        self.app = app
-
         self.settings_changed = False
         self.changes_applied = False
         self.server_changed = False
 
         self.initUI()
 
         self.link_callbacks()
@@ -58,16 +54,14 @@
         self.cb_notify.setChecked(settings.value("message/check_missed/notify", type=bool))
 
         self.cb_notification_click.setChecked(settings.value("tray/notifications/click", type=bool))
 
         self.cb_tray_icon_unread.setChecked(settings.value("tray/icon/unread", type=bool))
 
         # Interface
-        self.combo_theme.addItems(get_themes())
-        self.combo_theme.setCurrentText(settings.value("theme", type=str))
         self.cb_priority_colors.setChecked(settings.value("MessageWidget/priority_color", type=bool))
         self.cb_locale.setChecked(settings.value("locale", type=bool))
 
         # Logging
         self.combo_logging.addItems(
             [
                 logging.getLevelName(logging.ERROR),
@@ -87,15 +81,14 @@
         self.spin_popup_w.setValue(settings.value("ImagePopup/w", type=int))
         self.spin_popup_h.setValue(settings.value("ImagePopup/h", type=int))
         self.label_cache.setText("0 MB")
         self.compute_cache_size()
 
     def add_message_widget(self):
         self.message_widget = MessageWidget(
-            self.app,
             self,
             MessagesModelItem(
                 GotifyMessageModel(
                     {
                         "date": "2021-01-01T11:11:00.928224+01:00",
                         "message": "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin luctus.",
                         "title": "Title",
@@ -192,15 +185,14 @@
         self.spin_priority.valueChanged.connect(self.settings_changed_callback)
         self.spin_duration.valueChanged.connect(self.settings_changed_callback)
         self.cb_notify.stateChanged.connect(self.settings_changed_callback)
         self.cb_notification_click.stateChanged.connect(self.settings_changed_callback)
         self.cb_tray_icon_unread.stateChanged.connect(self.settings_changed_callback)
 
         # Interface
-        self.combo_theme.currentTextChanged.connect(self.settings_changed_callback)
         self.cb_priority_colors.stateChanged.connect(self.settings_changed_callback)
         self.cb_locale.stateChanged.connect(self.settings_changed_callback)
 
         # Server info
         self.pb_change_server_info.clicked.connect(self.change_server_info_callback)
 
         # Logging
@@ -229,20 +221,14 @@
         settings.setValue("tray/notifications/priority", self.spin_priority.value())
         settings.setValue("tray/notifications/duration_ms", self.spin_duration.value())
         settings.setValue("message/check_missed/notify", self.cb_notify.isChecked())
         settings.setValue("tray/notifications/click", self.cb_notification_click.isChecked())
         settings.setValue("tray/icon/unread", self.cb_tray_icon_unread.isChecked())
 
         # Interface
-        current_theme = settings.value("theme", type=str)
-        selected_theme = self.combo_theme.currentText()
-        if current_theme != selected_theme:
-            settings.setValue("theme", selected_theme)
-            self.theme_change_requested.emit(selected_theme)
-
         settings.setValue("MessageWidget/priority_color", self.cb_priority_colors.isChecked())
         settings.setValue("locale", self.cb_locale.isChecked())
 
         # Logging
         selected_level = self.combo_logging.currentText()
         settings.setValue("logging/level", selected_level)
         if selected_level == "Disabled":
```

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/widgets/StatusWidget.py` & `gotify-tray-0.5.1/gotify_tray/gui/widgets/StatusWidget.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,24 @@
 from gotify_tray.gui.themes import get_theme_file
 
 
 settings = Settings("gotify-tray")
 
 
 class StatusWidget(QtWidgets.QLabel):
-    def __init__(self, app: QtWidgets.QApplication):
+    def __init__(self):
         super(StatusWidget, self).__init__()
-        self.app = app
         self.setFixedSize(QtCore.QSize(20, 20))
         self.setScaledContents(True)
         self.set_connecting()
         self.image = None
 
     def set_status(self, image: str):
         self.image = image
-        self.setPixmap(QtGui.QPixmap(get_theme_file(self.app, image)))
+        self.setPixmap(QtGui.QPixmap(get_theme_file(image)))
 
     def set_active(self):
         self.setToolTip("Listening for new messages")
         self.set_status("status_active.svg")
 
     def set_connecting(self):
         self.setToolTip("Connecting...")
```

### Comparing `gotify-tray-0.5.0/gotify_tray/gui/widgets/Tray.py` & `gotify-tray-0.5.1/gotify_tray/gui/widgets/Tray.py`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/tasks.py` & `gotify-tray-0.5.1/gotify_tray/tasks.py`

 * *Files identical despite different names*

### Comparing `gotify-tray-0.5.0/gotify_tray/utils.py` & `gotify-tray-0.5.1/gotify_tray/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import platform
 import re
 import subprocess
 
 from pathlib import Path
 from typing import Iterator
+from PyQt6 import QtWidgets
 
 from gotify_tray import gotify
 from gotify_tray.database import Downloader
 
 
 def verify_server(force_new: bool = False, enable_import: bool = True) -> bool:
     from gotify_tray.gui import ServerInfoDialog
@@ -91,7 +92,13 @@
 
 
 def get_icon(name: str) -> str:
     if platform.system() == "Darwin":
         name += "-macos"
 
     return get_abs_path(f"gotify_tray/gui/images/{name}.png")
+
+def update_widget_property(widget: QtWidgets.QWidget, property: str, value: str):
+    widget.setProperty(property, value)
+    widget.style().unpolish(widget)
+    widget.style().polish(widget)
+    widget.update()
```

### Comparing `gotify-tray-0.5.0/gotify_tray.egg-info/PKG-INFO` & `gotify-tray-0.5.1/gotify_tray.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotify-tray
-Version: 0.5.0
+Version: 0.5.1
 Summary: A tray notification application for receiving messages from a Gotify server.
 Home-page: https://github.com/seird/gotify-tray
 Author: k.dries@protonmail.com
 Author-email: k.dries@protonmail.com
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `gotify-tray-0.5.0/gotify_tray.egg-info/SOURCES.txt` & `gotify-tray-0.5.1/gotify_tray.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -42,35 +42,29 @@
 gotify_tray/gui/images/tray-unread-macos.png
 gotify_tray/gui/images/tray-unread.png
 gotify_tray/gui/images/tray.png
 gotify_tray/gui/models/ApplicationModel.py
 gotify_tray/gui/models/MessagesModel.py
 gotify_tray/gui/models/__init__.py
 gotify_tray/gui/themes/__init__.py
-gotify_tray/gui/themes/dark_purple/__init__.py
-gotify_tray/gui/themes/dark_purple/palette.py
-gotify_tray/gui/themes/dark_purple/refresh.svg
-gotify_tray/gui/themes/dark_purple/status_active.svg
-gotify_tray/gui/themes/dark_purple/status_connecting.svg
-gotify_tray/gui/themes/dark_purple/status_error.svg
-gotify_tray/gui/themes/dark_purple/status_inactive.svg
-gotify_tray/gui/themes/dark_purple/style.qss
-gotify_tray/gui/themes/dark_purple/trashcan.svg
-gotify_tray/gui/themes/default/__init__.py
-gotify_tray/gui/themes/default/palette.py
-gotify_tray/gui/themes/default/style.qss
-gotify_tray/gui/themes/light_purple/__init__.py
-gotify_tray/gui/themes/light_purple/palette.py
-gotify_tray/gui/themes/light_purple/refresh.svg
-gotify_tray/gui/themes/light_purple/status_active.svg
-gotify_tray/gui/themes/light_purple/status_connecting.svg
-gotify_tray/gui/themes/light_purple/status_error.svg
-gotify_tray/gui/themes/light_purple/status_inactive.svg
-gotify_tray/gui/themes/light_purple/style.qss
-gotify_tray/gui/themes/light_purple/trashcan.svg
+gotify_tray/gui/themes/base.qss
+gotify_tray/gui/themes/dark/refresh.svg
+gotify_tray/gui/themes/dark/status_active.svg
+gotify_tray/gui/themes/dark/status_connecting.svg
+gotify_tray/gui/themes/dark/status_error.svg
+gotify_tray/gui/themes/dark/status_inactive.svg
+gotify_tray/gui/themes/dark/style.qss
+gotify_tray/gui/themes/dark/trashcan.svg
+gotify_tray/gui/themes/light/refresh.svg
+gotify_tray/gui/themes/light/status_active.svg
+gotify_tray/gui/themes/light/status_connecting.svg
+gotify_tray/gui/themes/light/status_error.svg
+gotify_tray/gui/themes/light/status_inactive.svg
+gotify_tray/gui/themes/light/style.qss
+gotify_tray/gui/themes/light/trashcan.svg
 gotify_tray/gui/widgets/ImagePopup.py
 gotify_tray/gui/widgets/MainWindow.py
 gotify_tray/gui/widgets/MessageWidget.py
 gotify_tray/gui/widgets/ServerInfoDialog.py
 gotify_tray/gui/widgets/SettingsDialog.py
 gotify_tray/gui/widgets/StatusWidget.py
 gotify_tray/gui/widgets/Tray.py
```

### Comparing `gotify-tray-0.5.0/setup.py` & `gotify-tray-0.5.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 EMAIL = "k.dries@protonmail.com"
 REQUIRES_PYTHON = '>=3.10.0'
 with open("version.txt", "r") as f:
     VERSION = f.read()
 
 # What packages are required for this module to be executed?
 REQUIRED = [
-    'requests', 'PyQt6', 'websocket-client', 'python-dateutil'
+    'requests==2.31.0', 'pyqt6==6.5.1', 'websocket-client==1.5.2', 'python-dateutil==2.8.2'
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'socks5 proxy': ['pysocks'],
 }
 
@@ -60,17 +60,17 @@
     python_requires=REQUIRES_PYTHON,
     url=URL,
     # packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
     # If your package is a single module, use this instead of 'packages':
     packages=find_packages(),
     package_data={
         'gotify_tray.gui.images': ['*.ico', '*.png'],
-        'gotify_tray.gui.themes.default': ['*.qss', '*.svg', '*.png'],
-        'gotify_tray.gui.themes.dark_purple': ['*.qss', '*.svg', '*.png'],
-        'gotify_tray.gui.themes.light_purple': ['*.qss', '*.svg', '*.png'],
+        'gotify_tray.gui.themes': ['*.qss'],
+        'gotify_tray.gui.themes.dark': ['*.qss', '*.svg', '*.png'],
+        'gotify_tray.gui.themes.light': ['*.qss', '*.svg', '*.png'],
     },
     data_files = [
     ],
 
     entry_points={
         'console_scripts': ['gotify-tray=gotify_tray.__main__:main'],
     },
```

