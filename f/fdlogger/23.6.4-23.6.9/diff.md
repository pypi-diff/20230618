# Comparing `tmp/fdlogger-23.6.4.tar.gz` & `tmp/fdlogger-23.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdlogger-23.6.4.tar", last modified: Mon Jun  5 04:30:52 2023, max compression
+gzip compressed data, was "fdlogger-23.6.9.tar", last modified: Fri Jun  9 20:25:40 2023, max compression
```

## Comparing `fdlogger-23.6.4.tar` & `fdlogger-23.6.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-05 04:30:52.085427 fdlogger-23.6.4/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-07-24 04:24:05.000000 fdlogger-23.6.4/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20909 2023-06-05 04:30:52.084427 fdlogger-23.6.4/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20121 2023-06-01 02:56:25.000000 fdlogger-23.6.4/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-05 04:30:51.973425 fdlogger-23.6.4/fdlogger/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-01 14:55:26.000000 fdlogger-23.6.4/fdlogger/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   105318 2023-05-30 15:44:18.000000 fdlogger-23.6.4/fdlogger/__main__.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-05 04:30:52.021426 fdlogger-23.6.4/fdlogger/data/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-02-01 14:55:26.000000 fdlogger-23.6.4/fdlogger/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   331983 2023-02-01 14:55:26.000000 fdlogger-23.6.4/fdlogger/data/MASTER.SCP
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2972 2023-02-01 14:55:26.000000 fdlogger-23.6.4/fdlogger/data/arrl_sect.dat
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      482 2023-06-01 02:37:05.000000 fdlogger-23.6.4/fdlogger/data/cwmacros_fd.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10325 2023-02-01 18:15:34.000000 fdlogger-23.6.4/fdlogger/data/dialog.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      592 2023-06-01 02:37:17.000000 fdlogger-23.6.4/fdlogger/data/fd_preferences.json
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      213 2023-02-01 14:59:00.000000 fdlogger-23.6.4/fdlogger/data/k6gte-fieldday.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   104172 2023-02-02 21:16:39.000000 fdlogger-23.6.4/fdlogger/data/main.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30785 2023-02-02 20:14:22.000000 fdlogger-23.6.4/fdlogger/data/settings.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3812 2023-02-01 18:15:34.000000 fdlogger-23.6.4/fdlogger/data/startup.ui
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-05 04:30:52.048426 fdlogger-23.6.4/fdlogger/icon/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      626 2023-02-01 14:55:26.000000 fdlogger-23.6.4/fdlogger/icon/cloud_green.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      641 2023-02-01 14:55:26.000000 fdlogger-23.6.4/fdlogger/icon/cloud_grey.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      482 2023-02-01 14:55:26.000000 fdlogger-23.6.4/fdlogger/icon/cloud_red.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      605 2023-02-01 14:55:26.000000 fdlogger-23.6.4/fdlogger/icon/gear16x16.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2876 2023-02-01 14:55:26.000000 fdlogger-23.6.4/fdlogger/icon/k6gte-fdlogger.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    96313 2023-02-19 21:29:22.000000 fdlogger-23.6.4/fdlogger/icon/logo.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5972 2023-02-01 14:55:26.000000 fdlogger-23.6.4/fdlogger/icon/radio.svg
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1234 2023-02-01 14:55:26.000000 fdlogger-23.6.4/fdlogger/icon/radio_green.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1258 2023-02-01 14:55:26.000000 fdlogger-23.6.4/fdlogger/icon/radio_grey.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      957 2023-02-01 14:55:26.000000 fdlogger-23.6.4/fdlogger/icon/radio_red.png
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-05 04:30:52.082427 fdlogger-23.6.4/fdlogger/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-01 14:55:26.000000 fdlogger-23.6.4/fdlogger/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10234 2023-02-02 20:57:22.000000 fdlogger-23.6.4/fdlogger/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1661 2023-02-02 20:57:35.000000 fdlogger-23.6.4/fdlogger/lib/cwinterface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13592 2023-02-02 20:58:22.000000 fdlogger-23.6.4/fdlogger/lib/database.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14064 2023-02-03 16:08:03.000000 fdlogger-23.6.4/fdlogger/lib/lookup.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4626 2023-02-02 20:59:29.000000 fdlogger-23.6.4/fdlogger/lib/n1mm.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6707 2023-04-08 23:33:07.000000 fdlogger-23.6.4/fdlogger/lib/settings.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-06-05 04:29:17.000000 fdlogger-23.6.4/fdlogger/lib/version.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1289 2023-02-02 20:14:22.000000 fdlogger-23.6.4/fdlogger/lib/versiontest.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-05 04:30:51.988426 fdlogger-23.6.4/fdlogger.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20909 2023-06-05 04:30:51.000000 fdlogger-23.6.4/fdlogger.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1170 2023-06-05 04:30:51.000000 fdlogger-23.6.4/fdlogger.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-06-05 04:30:51.000000 fdlogger-23.6.4/fdlogger.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2023-06-05 04:30:51.000000 fdlogger-23.6.4/fdlogger.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       35 2023-06-05 04:30:51.000000 fdlogger-23.6.4/fdlogger.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-06-05 04:30:51.000000 fdlogger-23.6.4/fdlogger.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1179 2023-06-05 04:29:01.000000 fdlogger-23.6.4/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-06-05 04:30:52.085427 fdlogger-23.6.4/setup.cfg
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-05 04:30:52.084427 fdlogger-23.6.4/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2714 2022-09-14 17:33:52.000000 fdlogger-23.6.4/testing/inject_multicast.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      862 2022-07-24 04:24:05.000000 fdlogger-23.6.4/testing/inject_udp.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)     1051 2023-03-01 19:35:50.000000 fdlogger-23.6.4/testing/multicast_listener.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    10948 2023-03-01 19:35:42.000000 fdlogger-23.6.4/testing/simulant.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-09 20:25:40.295438 fdlogger-23.6.9/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-07-24 04:24:05.000000 fdlogger-23.6.9/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    21363 2023-06-09 20:25:40.295438 fdlogger-23.6.9/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20575 2023-06-09 20:18:37.000000 fdlogger-23.6.9/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-09 20:25:40.289438 fdlogger-23.6.9/fdlogger/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-01 14:55:26.000000 fdlogger-23.6.9/fdlogger/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   106766 2023-06-09 20:15:48.000000 fdlogger-23.6.9/fdlogger/__main__.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-09 20:25:40.291438 fdlogger-23.6.9/fdlogger/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-02-01 14:55:26.000000 fdlogger-23.6.9/fdlogger/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   331983 2023-02-01 14:55:26.000000 fdlogger-23.6.9/fdlogger/data/MASTER.SCP
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2972 2023-02-01 14:55:26.000000 fdlogger-23.6.9/fdlogger/data/arrl_sect.dat
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      482 2023-06-01 02:37:05.000000 fdlogger-23.6.9/fdlogger/data/cwmacros_fd.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10325 2023-02-01 18:15:34.000000 fdlogger-23.6.9/fdlogger/data/dialog.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      592 2023-06-01 02:37:17.000000 fdlogger-23.6.9/fdlogger/data/fd_preferences.json
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      213 2023-02-01 14:59:00.000000 fdlogger-23.6.9/fdlogger/data/k6gte-fieldday.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   104172 2023-02-02 21:16:39.000000 fdlogger-23.6.9/fdlogger/data/main.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30785 2023-02-02 20:14:22.000000 fdlogger-23.6.9/fdlogger/data/settings.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3812 2023-02-01 18:15:34.000000 fdlogger-23.6.9/fdlogger/data/startup.ui
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-09 20:25:40.293438 fdlogger-23.6.9/fdlogger/icon/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      626 2023-02-01 14:55:26.000000 fdlogger-23.6.9/fdlogger/icon/cloud_green.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      641 2023-02-01 14:55:26.000000 fdlogger-23.6.9/fdlogger/icon/cloud_grey.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      482 2023-02-01 14:55:26.000000 fdlogger-23.6.9/fdlogger/icon/cloud_red.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      605 2023-02-01 14:55:26.000000 fdlogger-23.6.9/fdlogger/icon/gear16x16.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2876 2023-02-01 14:55:26.000000 fdlogger-23.6.9/fdlogger/icon/k6gte-fdlogger.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    96313 2023-02-19 21:29:22.000000 fdlogger-23.6.9/fdlogger/icon/logo.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5972 2023-02-01 14:55:26.000000 fdlogger-23.6.9/fdlogger/icon/radio.svg
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1234 2023-02-01 14:55:26.000000 fdlogger-23.6.9/fdlogger/icon/radio_green.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1258 2023-02-01 14:55:26.000000 fdlogger-23.6.9/fdlogger/icon/radio_grey.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      957 2023-02-01 14:55:26.000000 fdlogger-23.6.9/fdlogger/icon/radio_red.png
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-09 20:25:40.294438 fdlogger-23.6.9/fdlogger/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-01 14:55:26.000000 fdlogger-23.6.9/fdlogger/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10234 2023-02-02 20:57:22.000000 fdlogger-23.6.9/fdlogger/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1661 2023-02-02 20:57:35.000000 fdlogger-23.6.9/fdlogger/lib/cwinterface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13600 2023-06-09 20:05:46.000000 fdlogger-23.6.9/fdlogger/lib/database.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14064 2023-02-03 16:08:03.000000 fdlogger-23.6.9/fdlogger/lib/lookup.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4626 2023-02-02 20:59:29.000000 fdlogger-23.6.9/fdlogger/lib/n1mm.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6707 2023-04-08 23:33:07.000000 fdlogger-23.6.9/fdlogger/lib/settings.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-06-09 19:46:54.000000 fdlogger-23.6.9/fdlogger/lib/version.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1289 2023-02-02 20:14:22.000000 fdlogger-23.6.9/fdlogger/lib/versiontest.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-09 20:25:40.290438 fdlogger-23.6.9/fdlogger.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    21363 2023-06-09 20:25:40.000000 fdlogger-23.6.9/fdlogger.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1170 2023-06-09 20:25:40.000000 fdlogger-23.6.9/fdlogger.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-06-09 20:25:40.000000 fdlogger-23.6.9/fdlogger.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2023-06-09 20:25:40.000000 fdlogger-23.6.9/fdlogger.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       35 2023-06-09 20:25:40.000000 fdlogger-23.6.9/fdlogger.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-06-09 20:25:40.000000 fdlogger-23.6.9/fdlogger.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1179 2023-06-09 19:47:19.000000 fdlogger-23.6.9/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-06-09 20:25:40.296438 fdlogger-23.6.9/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-09 20:25:40.295438 fdlogger-23.6.9/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2714 2022-09-14 17:33:52.000000 fdlogger-23.6.9/testing/inject_multicast.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      862 2022-07-24 04:24:05.000000 fdlogger-23.6.9/testing/inject_udp.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)     1051 2023-03-01 19:35:50.000000 fdlogger-23.6.9/testing/multicast_listener.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    10948 2023-06-09 19:22:31.000000 fdlogger-23.6.9/testing/simulant.py
```

### Comparing `fdlogger-23.6.4/LICENSE` & `fdlogger-23.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fdlogger-23.6.4/PKG-INFO` & `fdlogger-23.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdlogger
-Version: 23.6.4
+Version: 23.6.9
 Summary: ARRL Field Day logger GUI
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/FieldDayLogger
 Project-URL: Bug Tracker, https://github.com/mbridak/FieldDayLogger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -92,14 +92,15 @@
 Just search for the two places in the code 'FT8' is used and Bob's your dads
 brother.
 
 **WB8ERJ's blog writeup** [Mike's Tech Blog WB8ERJ](https://mikestechblog.com/field-day-logging-software-for-the-raspberry-pi/)
 
 ## Recent Changes
 
+- [23.6.9] Added server dupe check. Thanks @kybrjo, Be sure to pip update the fdserver for this. Bugfix: was unable to edit frequency. Thanks @km4ack.
 - [23.5.31] Replaced some deleted stuff. Thanks @ATCUSA for finding it!
 - [23.5.30] Changed default multicast address from 224.1.1.1 to 239.1.1.1
 - [23.4.8] Fixed crash on setting setup.
 - [23.2.3] Fixed crash when qrz or hamqth was used. Fixed crash when not debugging. Contact lookup now shows in infoline. Reduced font size in the group chat window. Improved debug logging.
 - [23.2.2] Added N1MM status packets. fdserver program moved into it's own repo/PyPi package.
 - [23.2.1] Made interface resizable.
 - [23.1.30] Repackaged for PyPi pip installation
@@ -137,14 +138,16 @@
 # remove
 pip uninstall fdlogger
 
 # run it
 fdlogger
 ```
 
+If you get a message about `./local/bin` not being in your PATH, try logging out and right back in. Most of the time your linux distro will detect you now have files in there and add it to your PATH.
+
 ## What to do first
 
 When run for the first time, you will be greeted by a dialog asking for your
 Callsign, Class and Section. Afterward, there is a gear icon on the main
 screen, where you can change your CAT, CW interface, callsign lookup service
 etc. You can also change your call class and section by clicking on the
 respective fields.
@@ -240,14 +243,16 @@
 be highlighted, the screen will flash, a bell will sound to alert you that this
 is a DUP. At this point you and the other OP can argue back and forth about
 who's wrong. In the end you'll put your big boy pants on and make a decision if
 you'll enter the call or not.
 
 ![Picture showing dup checking](https://github.com/mbridak/FieldDayLogger/raw/main/pics/dupe.png)
 
+If you are using the group server, the client will poll the server as well asking if this is a dupe.
+
 ## Autofill
 
 If you have worked this person before on another band/mode the program will
 load the class and section used previously for this call so you will not have
 to enter this info again.
 
 ## CW Macros
```

### Comparing `fdlogger-23.6.4/README.md` & `fdlogger-23.6.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 Just search for the two places in the code 'FT8' is used and Bob's your dads
 brother.
 
 **WB8ERJ's blog writeup** [Mike's Tech Blog WB8ERJ](https://mikestechblog.com/field-day-logging-software-for-the-raspberry-pi/)
 
 ## Recent Changes
 
+- [23.6.9] Added server dupe check. Thanks @kybrjo, Be sure to pip update the fdserver for this. Bugfix: was unable to edit frequency. Thanks @km4ack.
 - [23.5.31] Replaced some deleted stuff. Thanks @ATCUSA for finding it!
 - [23.5.30] Changed default multicast address from 224.1.1.1 to 239.1.1.1
 - [23.4.8] Fixed crash on setting setup.
 - [23.2.3] Fixed crash when qrz or hamqth was used. Fixed crash when not debugging. Contact lookup now shows in infoline. Reduced font size in the group chat window. Improved debug logging.
 - [23.2.2] Added N1MM status packets. fdserver program moved into it's own repo/PyPi package.
 - [23.2.1] Made interface resizable.
 - [23.1.30] Repackaged for PyPi pip installation
@@ -118,14 +119,16 @@
 # remove
 pip uninstall fdlogger
 
 # run it
 fdlogger
 ```
 
+If you get a message about `./local/bin` not being in your PATH, try logging out and right back in. Most of the time your linux distro will detect you now have files in there and add it to your PATH.
+
 ## What to do first
 
 When run for the first time, you will be greeted by a dialog asking for your
 Callsign, Class and Section. Afterward, there is a gear icon on the main
 screen, where you can change your CAT, CW interface, callsign lookup service
 etc. You can also change your call class and section by clicking on the
 respective fields.
@@ -221,14 +224,16 @@
 be highlighted, the screen will flash, a bell will sound to alert you that this
 is a DUP. At this point you and the other OP can argue back and forth about
 who's wrong. In the end you'll put your big boy pants on and make a decision if
 you'll enter the call or not.
 
 ![Picture showing dup checking](https://github.com/mbridak/FieldDayLogger/raw/main/pics/dupe.png)
 
+If you are using the group server, the client will poll the server as well asking if this is a dupe.
+
 ## Autofill
 
 If you have worked this person before on another band/mode the program will
 load the class and section used previously for this call so you will not have
 to enter this info again.
 
 ## CW Macros
```

### Comparing `fdlogger-23.6.4/fdlogger/__main__.py` & `fdlogger-23.6.9/fdlogger/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -441,14 +441,24 @@
                         self.server_seen = datetime.now() + timedelta(seconds=30)
                         self.group_call_indicator.setStyleSheet(
                             "border: 1px solid green;"
                         )
                         return
                     if json_data.get("subject") == "LOG":
                         self.infoline.setText("Server Generated Log.")
+
+                    if json_data.get("subject") == "DUPE":
+                        if json_data.get("isdupe") is not 0:
+                            if json_data.get("contact") == self.callsign_entry.text():
+                                self.flash()
+                                self.infobox.setTextColor(QtGui.QColor(245, 121, 0))
+                                self.infobox.insertPlainText(
+                                    f"{json_data.get('contact')}: " "Server DUPE\n"
+                                )
+
                     self.remove_confirmed_commands(json_data)
                     continue
 
             if json_data.get("cmd") == "CHAT":
                 self.display_chat(json_data.get("sender"), json_data.get("message"))
                 continue
 
@@ -466,14 +476,38 @@
         try:
             self.server_udp.sendto(
                 bytesToSend, (self.multicast_group, int(self.multicast_port))
             )
         except OSError as err:
             logger.warning("%s", err)
 
+    def check_dupe_status_udp(self):
+        """Ask server if our contact is a dupe"""
+        if self.connect_to_server:
+            if self.groupcall is None and self.preference["mycall"] != "":
+                self.query_group()
+                return
+
+            ask_if_dupe = {
+                "cmd": "DUPE",
+                "mode": self.mode,
+                "band": self.band,
+                "station": self.preference["mycall"],
+                "contact": self.callsign_entry.text(),
+            }
+            bytesToSend = bytes(dumps(ask_if_dupe), encoding="ascii")
+            try:
+                self.server_udp.sendto(
+                    bytesToSend, (self.multicast_group, int(self.multicast_port))
+                )
+            except OSError as err:
+                logger.warning("%s", err)
+
+            self.check_for_stale_commands()
+
     def send_status_udp(self):
         """Send status update to server informing of our band and mode"""
         if self.connect_to_server:
             if self.groupcall is None and self.preference["mycall"] != "":
                 self.query_group()
                 return
 
@@ -1762,14 +1796,15 @@
         if len(acall) > 2:
             matches = list(filter(lambda x: x.startswith(acall), self.scp))
             for match in matches:
                 self.infobox.insertPlainText(match + " ")
 
     def dup_check(self):
         """check for duplicates"""
+        self.check_dupe_status_udp()
         acall = self.callsign_entry.text()
         self.infobox.clear()
         log = self.db.dup_check(acall)
         for contact in log:
             hiscall, hisclass, hissection, hisband, hismode = contact
             if len(self.class_entry.text()) == 0:
                 self.class_entry.setText(hisclass)
@@ -2426,14 +2461,15 @@
             self.editCallsign.text().upper(),
             self.editClass.text().upper(),
             self.editSection.text().upper(),
             self.editDateTime.text(),
             self.editBand.currentText(),
             self.editMode.currentText().upper(),
             self.editPower.value(),
+            self.editFreq.text(),
             self.theitem,
         ]
         self.database.change_contact(qso)
         if window.connect_to_server:
             stale = datetime.now() + timedelta(seconds=30)
             command = {"cmd": "UPDATE"}
             command["hiscall"] = self.editCallsign.text().upper()
```

### Comparing `fdlogger-23.6.4/fdlogger/data/JetBrainsMono-Regular.ttf` & `fdlogger-23.6.9/fdlogger/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `fdlogger-23.6.4/fdlogger/data/MASTER.SCP` & `fdlogger-23.6.9/fdlogger/data/MASTER.SCP`

 * *Files identical despite different names*

### Comparing `fdlogger-23.6.4/fdlogger/data/arrl_sect.dat` & `fdlogger-23.6.9/fdlogger/data/arrl_sect.dat`

 * *Files identical despite different names*

### Comparing `fdlogger-23.6.4/fdlogger/data/dialog.ui` & `fdlogger-23.6.9/fdlogger/data/dialog.ui`

 * *Files identical despite different names*

### Comparing `fdlogger-23.6.4/fdlogger/data/fd_preferences.json` & `fdlogger-23.6.9/fdlogger/data/fd_preferences.json`

 * *Files identical despite different names*

### Comparing `fdlogger-23.6.4/fdlogger/data/main.ui` & `fdlogger-23.6.9/fdlogger/data/main.ui`

 * *Files identical despite different names*

### Comparing `fdlogger-23.6.4/fdlogger/data/settings.ui` & `fdlogger-23.6.9/fdlogger/data/settings.ui`

 * *Files identical despite different names*

### Comparing `fdlogger-23.6.4/fdlogger/data/startup.ui` & `fdlogger-23.6.9/fdlogger/data/startup.ui`

 * *Files identical despite different names*

### Comparing `fdlogger-23.6.4/fdlogger/icon/cloud_green.png` & `fdlogger-23.6.9/fdlogger/icon/cloud_green.png`

 * *Files identical despite different names*

### Comparing `fdlogger-23.6.4/fdlogger/icon/cloud_grey.png` & `fdlogger-23.6.9/fdlogger/icon/cloud_grey.png`

 * *Files identical despite different names*

### Comparing `fdlogger-23.6.4/fdlogger/icon/gear16x16.png` & `fdlogger-23.6.9/fdlogger/icon/gear16x16.png`

 * *Files identical despite different names*

### Comparing `fdlogger-23.6.4/fdlogger/icon/k6gte-fdlogger.png` & `fdlogger-23.6.9/fdlogger/icon/k6gte-fdlogger.png`

 * *Files identical despite different names*

### Comparing `fdlogger-23.6.4/fdlogger/icon/logo.png` & `fdlogger-23.6.9/fdlogger/icon/logo.png`

 * *Files identical despite different names*

### Comparing `fdlogger-23.6.4/fdlogger/icon/radio.svg` & `fdlogger-23.6.9/fdlogger/icon/radio.svg`

 * *Files identical despite different names*

### Comparing `fdlogger-23.6.4/fdlogger/icon/radio_green.png` & `fdlogger-23.6.9/fdlogger/icon/radio_green.png`

 * *Files identical despite different names*

### Comparing `fdlogger-23.6.4/fdlogger/icon/radio_grey.png` & `fdlogger-23.6.9/fdlogger/icon/radio_grey.png`

 * *Files identical despite different names*

### Comparing `fdlogger-23.6.4/fdlogger/icon/radio_red.png` & `fdlogger-23.6.9/fdlogger/icon/radio_red.png`

 * *Files identical despite different names*

### Comparing `fdlogger-23.6.4/fdlogger/lib/cat_interface.py` & `fdlogger-23.6.9/fdlogger/lib/cat_interface.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.6.4/fdlogger/lib/cwinterface.py` & `fdlogger-23.6.9/fdlogger/lib/cwinterface.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.6.4/fdlogger/lib/database.py` & `fdlogger-23.6.9/fdlogger/lib/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,32 +106,31 @@
             try:
                 with sqlite3.connect(self.database) as conn:
                     sql = f"delete from contacts where id={int(contact)}"
                     cur = conn.cursor()
                     cur.execute(sql)
                     conn.commit()
             except sqlite3.Error as exception:
-                self.logger.debug("DataBase delete_contact: %s", exception)
+                self.logger.critical("DataBase delete_contact: %s", exception)
 
     def change_contact(self, qso):
         """Update an existing contact."""
-        print(qso)
         try:
             with sqlite3.connect(self.database) as conn:
                 sql = (
                     f"update contacts set callsign = '{qso[0]}', class = '{qso[1]}', "
                     f"section = '{qso[2]}', date_time = '{qso[3]}', band = '{qso[4]}', "
-                    f"mode = '{qso[5]}', power = '{qso[6]}'  where id='{qso[7]}'"
+                    f"mode = '{qso[5]}', power = '{qso[6]}', frequency = '{qso[7]}' "
+                    f"where id='{qso[8]}';"
                 )
-                print(sql)
                 cur = conn.cursor()
                 cur.execute(sql)
                 conn.commit()
         except sqlite3.Error as exception:
-            self.logger.debug("DataBase change_contact: %s", exception)
+            self.logger.critical("DataBase change_contact: %s", exception)
 
     def stats(self) -> tuple:
         """
         returns a tuple with some stats:
         cwcontacts, phonecontacts, digitalcontacts, bandmodemult, last15, lasthour, hignpower, qrp
         """
         with sqlite3.connect(self.database) as conn:
```

### Comparing `fdlogger-23.6.4/fdlogger/lib/lookup.py` & `fdlogger-23.6.9/fdlogger/lib/lookup.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.6.4/fdlogger/lib/n1mm.py` & `fdlogger-23.6.9/fdlogger/lib/n1mm.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.6.4/fdlogger/lib/settings.py` & `fdlogger-23.6.9/fdlogger/lib/settings.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.6.4/fdlogger/lib/versiontest.py` & `fdlogger-23.6.9/fdlogger/lib/versiontest.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.6.4/fdlogger.egg-info/PKG-INFO` & `fdlogger-23.6.9/fdlogger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdlogger
-Version: 23.6.4
+Version: 23.6.9
 Summary: ARRL Field Day logger GUI
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/FieldDayLogger
 Project-URL: Bug Tracker, https://github.com/mbridak/FieldDayLogger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -92,14 +92,15 @@
 Just search for the two places in the code 'FT8' is used and Bob's your dads
 brother.
 
 **WB8ERJ's blog writeup** [Mike's Tech Blog WB8ERJ](https://mikestechblog.com/field-day-logging-software-for-the-raspberry-pi/)
 
 ## Recent Changes
 
+- [23.6.9] Added server dupe check. Thanks @kybrjo, Be sure to pip update the fdserver for this. Bugfix: was unable to edit frequency. Thanks @km4ack.
 - [23.5.31] Replaced some deleted stuff. Thanks @ATCUSA for finding it!
 - [23.5.30] Changed default multicast address from 224.1.1.1 to 239.1.1.1
 - [23.4.8] Fixed crash on setting setup.
 - [23.2.3] Fixed crash when qrz or hamqth was used. Fixed crash when not debugging. Contact lookup now shows in infoline. Reduced font size in the group chat window. Improved debug logging.
 - [23.2.2] Added N1MM status packets. fdserver program moved into it's own repo/PyPi package.
 - [23.2.1] Made interface resizable.
 - [23.1.30] Repackaged for PyPi pip installation
@@ -137,14 +138,16 @@
 # remove
 pip uninstall fdlogger
 
 # run it
 fdlogger
 ```
 
+If you get a message about `./local/bin` not being in your PATH, try logging out and right back in. Most of the time your linux distro will detect you now have files in there and add it to your PATH.
+
 ## What to do first
 
 When run for the first time, you will be greeted by a dialog asking for your
 Callsign, Class and Section. Afterward, there is a gear icon on the main
 screen, where you can change your CAT, CW interface, callsign lookup service
 etc. You can also change your call class and section by clicking on the
 respective fields.
@@ -240,14 +243,16 @@
 be highlighted, the screen will flash, a bell will sound to alert you that this
 is a DUP. At this point you and the other OP can argue back and forth about
 who's wrong. In the end you'll put your big boy pants on and make a decision if
 you'll enter the call or not.
 
 ![Picture showing dup checking](https://github.com/mbridak/FieldDayLogger/raw/main/pics/dupe.png)
 
+If you are using the group server, the client will poll the server as well asking if this is a dupe.
+
 ## Autofill
 
 If you have worked this person before on another band/mode the program will
 load the class and section used previously for this call so you will not have
 to enter this info again.
 
 ## CW Macros
```

### Comparing `fdlogger-23.6.4/fdlogger.egg-info/SOURCES.txt` & `fdlogger-23.6.9/fdlogger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fdlogger-23.6.4/pyproject.toml` & `fdlogger-23.6.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fdlogger" 
-version = "23.6.4"
+version = "23.6.9"
 description = "ARRL Field Day logger GUI"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```

### Comparing `fdlogger-23.6.4/testing/inject_multicast.py` & `fdlogger-23.6.9/testing/inject_multicast.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.6.4/testing/inject_udp.py` & `fdlogger-23.6.9/testing/inject_udp.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.6.4/testing/multicast_listener.py` & `fdlogger-23.6.9/testing/multicast_listener.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.6.4/testing/simulant.py` & `fdlogger-23.6.9/testing/simulant.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 parser.add_argument("-b", "--band", type=str, help="Your Band")
 parser.add_argument("-m", "--mode", type=str, help="Your Mode")
 parser.add_argument("-p", "--power", type=str, help="Your Power")
 
 args = parser.parse_args()
 
 MULTICAST_PORT = 2239
-MULTICAST_GROUP = "224.1.1.1"
+MULTICAST_GROUP = "239.1.1.1"
 INTERFACE_IP = "0.0.0.0"
 GROUP_CALL = None
 
 eightymeterstalk = (
     "What are the @stats?",
     "That K6GTE guy is a jerk!",
     "I worked your mama on 80 meters.",
```

