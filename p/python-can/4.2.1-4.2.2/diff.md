# Comparing `tmp/python-can-4.2.1.tar.gz` & `tmp/python-can-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-can-4.2.1.tar", last modified: Mon May 15 10:17:10 2023, max compression
+gzip compressed data, was "python-can-4.2.2.tar", last modified: Sun Jun 18 15:01:11 2023, max compression
```

## Comparing `python-can-4.2.1.tar` & `python-can-4.2.2.tar`

### file list

```diff
@@ -1,241 +1,242 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:17:10.375517 python-can-4.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-15 10:17:00.000000 python-can-4.2.1/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-15 10:17:00.000000 python-can-4.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-15 10:17:00.000000 python-can-4.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-05-15 10:17:10.375517 python-can-4.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-05-15 10:17:00.000000 python-can-4.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:17:10.351517 python-can-4.2.1/can/
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-15 10:17:00.000000 python-can-4.2.1/can/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38043 2023-05-15 10:17:00.000000 python-can-4.2.1/can/bit_timing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-15 10:17:00.000000 python-can-4.2.1/can/broadcastmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-05-15 10:17:00.000000 python-can-4.2.1/can/bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-05-15 10:17:00.000000 python-can-4.2.1/can/ctypesutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-15 10:17:00.000000 python-can-4.2.1/can/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:17:10.355517 python-can-4.2.1/can/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/canalystii.py
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/cantact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:17:10.355517 python-can-4.2.1/can/interfaces/etas/
--rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/etas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20644 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/etas/boa.py
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/gs_usb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:17:10.355517 python-can-4.2.1/can/interfaces/ics_neovi/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/ics_neovi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17330 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/ics_neovi/neovi_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/iscan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:17:10.355517 python-can-4.2.1/can/interfaces/ixxat/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/ixxat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/ixxat/canlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    34976 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/ixxat/canlib_vcinpl.py
--rw-r--r--   0 runner    (1001) docker     (123)    38458 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/ixxat/canlib_vcinpl2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/ixxat/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/ixxat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/ixxat/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:17:10.355517 python-can-4.2.1/can/interfaces/kvaser/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/kvaser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24303 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/kvaser/canlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/kvaser/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/kvaser/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:17:10.355517 python-can-4.2.1/can/interfaces/neousys/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/neousys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/neousys/neousys.py
--rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/nican.py
--rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/nixnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:17:10.355517 python-can-4.2.1/can/interfaces/pcan/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/pcan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41809 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/pcan/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    26817 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/pcan/pcan.py
--rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/robotell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:17:10.355517 python-can-4.2.1/can/interfaces/seeedstudio/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/seeedstudio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/seeedstudio/seeedstudio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:17:10.355517 python-can-4.2.1/can/interfaces/serial/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/serial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/serial/serial_can.py
--rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/slcan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:17:10.355517 python-can-4.2.1/can/interfaces/socketcan/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/socketcan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/socketcan/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    32057 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/socketcan/socketcan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/socketcan/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:17:10.355517 python-can-4.2.1/can/interfaces/socketcand/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/socketcand/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/socketcand/socketcand.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:17:10.359517 python-can-4.2.1/can/interfaces/systec/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/systec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22700 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/systec/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/systec/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/systec/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)    46740 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/systec/ucan.py
--rw-r--r--   0 runner    (1001) docker     (123)    11213 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/systec/ucanbus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:17:10.359517 python-can-4.2.1/can/interfaces/udp_multicast/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/udp_multicast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16610 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/udp_multicast/bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/udp_multicast/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:17:10.359517 python-can-4.2.1/can/interfaces/usb2can/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/usb2can/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/usb2can/serial_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/usb2can/usb2canInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/usb2can/usb2canabstractionlayer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:17:10.359517 python-can-4.2.1/can/interfaces/vector/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43917 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/vector/canlib.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/vector/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/vector/xlclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/vector/xldefine.py
--rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/vector/xldriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-05-15 10:17:00.000000 python-can-4.2.1/can/interfaces/virtual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:17:10.359517 python-can-4.2.1/can/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-15 10:17:00.000000 python-can-4.2.1/can/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-05-15 10:17:00.000000 python-can-4.2.1/can/io/asc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21908 2023-05-15 10:17:00.000000 python-can-4.2.1/can/io/blf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-05-15 10:17:00.000000 python-can-4.2.1/can/io/canutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-15 10:17:00.000000 python-can-4.2.1/can/io/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-15 10:17:00.000000 python-can-4.2.1/can/io/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-05-15 10:17:00.000000 python-can-4.2.1/can/io/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    18222 2023-05-15 10:17:00.000000 python-can-4.2.1/can/io/mf4.py
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-05-15 10:17:00.000000 python-can-4.2.1/can/io/player.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-15 10:17:00.000000 python-can-4.2.1/can/io/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-05-15 10:17:00.000000 python-can-4.2.1/can/io/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-05-15 10:17:00.000000 python-can-4.2.1/can/io/trc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-05-15 10:17:00.000000 python-can-4.2.1/can/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-15 10:17:00.000000 python-can-4.2.1/can/logconvert.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-05-15 10:17:00.000000 python-can-4.2.1/can/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-05-15 10:17:00.000000 python-can-4.2.1/can/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-05-15 10:17:00.000000 python-can-4.2.1/can/notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-15 10:17:00.000000 python-can-4.2.1/can/player.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:17:00.000000 python-can-4.2.1/can/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-15 10:17:00.000000 python-can-4.2.1/can/thread_safe_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-15 10:17:00.000000 python-can-4.2.1/can/typechecking.py
--rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-05-15 10:17:00.000000 python-can-4.2.1/can/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    22278 2023-05-15 10:17:00.000000 python-can-4.2.1/can/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:17:10.363517 python-can-4.2.1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/asyncio.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/bcm.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/bit_timing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/bus.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/errors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:17:10.367517 python-can-4.2.1/doc/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/interfaces/canalystii.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/interfaces/cantact.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/interfaces/etas.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     2566 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/interfaces/gs_usb.rst
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/interfaces/iscan.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/interfaces/ixxat.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/interfaces/kvaser.rst
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/interfaces/neousys.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/interfaces/neovi.rst
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/interfaces/nican.rst
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/interfaces/nixnet.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/interfaces/pcan.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/interfaces/robotell.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/interfaces/seeedstudio.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/interfaces/serial.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1055 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/interfaces/slcan.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/interfaces/socketcan.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/interfaces/socketcand.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/interfaces/systec.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/interfaces/udp_multicast.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/interfaces/usb2can.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/interfaces/vector.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/interfaces/virtual.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/interfaces.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/internal-api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/listeners.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/message.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/other-tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/plugin-interface.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/scripts.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8462 2023-05-15 10:17:00.000000 python-can-4.2.1/doc/virtual-interfaces.rst
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-15 10:17:00.000000 python-can-4.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:17:10.367517 python-can-4.2.1/python_can.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-05-15 10:17:10.000000 python-can-4.2.1/python_can.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-05-15 10:17:10.000000 python-can-4.2.1/python_can.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 10:17:10.000000 python-can-4.2.1/python_can.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-15 10:17:10.000000 python-can-4.2.1/python_can.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-15 10:17:10.000000 python-can-4.2.1/python_can.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-15 10:17:00.000000 python-can-4.2.1/requirements-lint.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:17:10.367517 python-can-4.2.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-15 10:17:00.000000 python-can-4.2.1/scripts/can_logconvert.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-15 10:17:00.000000 python-can-4.2.1/scripts/can_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-15 10:17:00.000000 python-can-4.2.1/scripts/can_player.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-15 10:17:00.000000 python-can-4.2.1/scripts/can_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-15 10:17:10.375517 python-can-4.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-15 10:17:00.000000 python-can-4.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:17:10.371517 python-can-4.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 10:17:00.000000 python-can-4.2.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15773 2023-05-15 10:17:00.000000 python-can-4.2.1/test/back2back_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-15 10:17:00.000000 python-can-4.2.1/test/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-15 10:17:00.000000 python-can-4.2.1/test/contextmanager_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:17:10.375517 python-can-4.2.1/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 10:17:00.000000 python-can-4.2.1/test/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-05-15 10:17:00.000000 python-can-4.2.1/test/data/example_data.py
--rw-r--r--   0 runner    (1001) docker     (123)   128078 2023-05-15 10:17:00.000000 python-can-4.2.1/test/data/issue_1256.asc
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-15 10:17:00.000000 python-can-4.2.1/test/data/issue_1299.asc
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-05-15 10:17:00.000000 python-can-4.2.1/test/data/logfile.asc
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-15 10:17:00.000000 python-can-4.2.1/test/data/logfile_errorframes.asc
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-15 10:17:00.000000 python-can-4.2.1/test/data/test_CanErrorFrameExt.blf
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-15 10:17:00.000000 python-can-4.2.1/test/data/test_CanErrorFrames.asc
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-15 10:17:00.000000 python-can-4.2.1/test/data/test_CanFdMessage.asc
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-15 10:17:00.000000 python-can-4.2.1/test/data/test_CanFdMessage.blf
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-15 10:17:00.000000 python-can-4.2.1/test/data/test_CanFdMessage64.asc
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-15 10:17:00.000000 python-can-4.2.1/test/data/test_CanFdMessage64.blf
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-15 10:17:00.000000 python-can-4.2.1/test/data/test_CanFdRemoteMessage.asc
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-15 10:17:00.000000 python-can-4.2.1/test/data/test_CanMessage.asc
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-15 10:17:00.000000 python-can-4.2.1/test/data/test_CanMessage.asc.gz
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-15 10:17:00.000000 python-can-4.2.1/test/data/test_CanMessage.blf
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-15 10:17:00.000000 python-can-4.2.1/test/data/test_CanMessage.trc
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-15 10:17:00.000000 python-can-4.2.1/test/data/test_CanMessage2.blf
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-15 10:17:00.000000 python-can-4.2.1/test/data/test_CanMessage_V1_0_BUS1.trc
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-15 10:17:00.000000 python-can-4.2.1/test/data/test_CanMessage_V1_1.trc
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-15 10:17:00.000000 python-can-4.2.1/test/data/test_CanMessage_V2_0_BUS1.trc
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-15 10:17:00.000000 python-can-4.2.1/test/data/test_CanMessage_V2_1.trc
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-15 10:17:00.000000 python-can-4.2.1/test/data/test_CanRemoteMessage.asc
--rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-05-15 10:17:00.000000 python-can-4.2.1/test/listener_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-05-15 10:17:00.000000 python-can-4.2.1/test/logformats_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-15 10:17:00.000000 python-can-4.2.1/test/message_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-15 10:17:00.000000 python-can-4.2.1/test/network_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-15 10:17:00.000000 python-can-4.2.1/test/notifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-05-15 10:17:00.000000 python-can-4.2.1/test/serial_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-05-15 10:17:00.000000 python-can-4.2.1/test/simplecyclic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13580 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_bit_timing.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_cantact.py
--rw-r--r--   0 runner    (1001) docker     (123)    22230 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_cyclic_socketcan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_detect_available_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_interface.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3367 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_interface_canalystii.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_interface_ixxat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_interface_ixxat_fd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_interface_virtual.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_kvaser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_load_file_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_message_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_message_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_message_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_neousys.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_neovi.py
--rw-r--r--   0 runner    (1001) docker     (123)    19093 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_pcan.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3930 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_player.py
--rw-r--r--   0 runner    (1001) docker     (123)    24830 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_robotell.py
--rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_rotating_loggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_slcan.py
--rw-r--r--   0 runner    (1001) docker     (123)    13308 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_socketcan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_socketcan_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_socketcan_loopback.py
--rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_systec.py
--rw-r--r--   0 runner    (1001) docker     (123)    11232 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    47118 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)    20951 2023-05-15 10:17:00.000000 python-can-4.2.1/test/test_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-15 10:17:00.000000 python-can-4.2.1/test/zero_dlc_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:01:11.348160 python-can-4.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-18 15:01:02.000000 python-can-4.2.2/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-18 15:01:02.000000 python-can-4.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-18 15:01:02.000000 python-can-4.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-06-18 15:01:11.348160 python-can-4.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-18 15:01:02.000000 python-can-4.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:01:11.320160 python-can-4.2.2/can/
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-18 15:01:02.000000 python-can-4.2.2/can/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38043 2023-06-18 15:01:02.000000 python-can-4.2.2/can/bit_timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-06-18 15:01:02.000000 python-can-4.2.2/can/broadcastmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-06-18 15:01:02.000000 python-can-4.2.2/can/bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-18 15:01:02.000000 python-can-4.2.2/can/ctypesutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-06-18 15:01:02.000000 python-can-4.2.2/can/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-06-18 15:01:02.000000 python-can-4.2.2/can/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:01:11.320160 python-can-4.2.2/can/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-18 15:01:02.000000 python-can-4.2.2/can/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-06-18 15:01:02.000000 python-can-4.2.2/can/interfaces/canalystii.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-06-18 15:01:02.000000 python-can-4.2.2/can/interfaces/cantact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:01:11.320160 python-can-4.2.2/can/interfaces/etas/
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-06-18 15:01:02.000000 python-can-4.2.2/can/interfaces/etas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20644 2023-06-18 15:01:02.000000 python-can-4.2.2/can/interfaces/etas/boa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-06-18 15:01:02.000000 python-can-4.2.2/can/interfaces/gs_usb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:01:11.320160 python-can-4.2.2/can/interfaces/ics_neovi/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-18 15:01:02.000000 python-can-4.2.2/can/interfaces/ics_neovi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17330 2023-06-18 15:01:02.000000 python-can-4.2.2/can/interfaces/ics_neovi/neovi_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-06-18 15:01:02.000000 python-can-4.2.2/can/interfaces/iscan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:01:11.324160 python-can-4.2.2/can/interfaces/ixxat/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-18 15:01:02.000000 python-can-4.2.2/can/interfaces/ixxat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-06-18 15:01:02.000000 python-can-4.2.2/can/interfaces/ixxat/canlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35003 2023-06-18 15:01:02.000000 python-can-4.2.2/can/interfaces/ixxat/canlib_vcinpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38485 2023-06-18 15:01:02.000000 python-can-4.2.2/can/interfaces/ixxat/canlib_vcinpl2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-06-18 15:01:02.000000 python-can-4.2.2/can/interfaces/ixxat/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-18 15:01:02.000000 python-can-4.2.2/can/interfaces/ixxat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-06-18 15:01:02.000000 python-can-4.2.2/can/interfaces/ixxat/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:01:11.324160 python-can-4.2.2/can/interfaces/kvaser/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-18 15:01:02.000000 python-can-4.2.2/can/interfaces/kvaser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24353 2023-06-18 15:01:02.000000 python-can-4.2.2/can/interfaces/kvaser/canlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-06-18 15:01:02.000000 python-can-4.2.2/can/interfaces/kvaser/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-18 15:01:02.000000 python-can-4.2.2/can/interfaces/kvaser/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:01:11.324160 python-can-4.2.2/can/interfaces/neousys/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-18 15:01:02.000000 python-can-4.2.2/can/interfaces/neousys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/neousys/neousys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/nican.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/nixnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:01:11.324160 python-can-4.2.2/can/interfaces/pcan/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/pcan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41809 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/pcan/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26817 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/pcan/pcan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/robotell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:01:11.324160 python-can-4.2.2/can/interfaces/seeedstudio/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/seeedstudio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/seeedstudio/seeedstudio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:01:11.324160 python-can-4.2.2/can/interfaces/serial/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/serial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/serial/serial_can.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/slcan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:01:11.324160 python-can-4.2.2/can/interfaces/socketcan/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/socketcan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/socketcan/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32057 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/socketcan/socketcan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/socketcan/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:01:11.324160 python-can-4.2.2/can/interfaces/socketcand/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/socketcand/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/socketcand/socketcand.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:01:11.324160 python-can-4.2.2/can/interfaces/systec/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/systec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22700 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/systec/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/systec/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/systec/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46740 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/systec/ucan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11213 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/systec/ucanbus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:01:11.328160 python-can-4.2.2/can/interfaces/udp_multicast/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/udp_multicast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16610 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/udp_multicast/bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/udp_multicast/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:01:11.328160 python-can-4.2.2/can/interfaces/usb2can/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/usb2can/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/usb2can/serial_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/usb2can/usb2canInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/usb2can/usb2canabstractionlayer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:01:11.328160 python-can-4.2.2/can/interfaces/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43917 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/vector/canlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/vector/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/vector/xlclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/vector/xldefine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/vector/xldriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-06-18 15:01:03.000000 python-can-4.2.2/can/interfaces/virtual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:01:11.328160 python-can-4.2.2/can/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-18 15:01:03.000000 python-can-4.2.2/can/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-06-18 15:01:03.000000 python-can-4.2.2/can/io/asc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21908 2023-06-18 15:01:03.000000 python-can-4.2.2/can/io/blf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-06-18 15:01:03.000000 python-can-4.2.2/can/io/canutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-18 15:01:03.000000 python-can-4.2.2/can/io/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-06-18 15:01:03.000000 python-can-4.2.2/can/io/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-06-18 15:01:03.000000 python-can-4.2.2/can/io/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18268 2023-06-18 15:01:03.000000 python-can-4.2.2/can/io/mf4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-06-18 15:01:03.000000 python-can-4.2.2/can/io/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-18 15:01:03.000000 python-can-4.2.2/can/io/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-06-18 15:01:03.000000 python-can-4.2.2/can/io/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-06-18 15:01:03.000000 python-can-4.2.2/can/io/trc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-06-18 15:01:03.000000 python-can-4.2.2/can/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-18 15:01:03.000000 python-can-4.2.2/can/logconvert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-06-18 15:01:03.000000 python-can-4.2.2/can/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-06-18 15:01:03.000000 python-can-4.2.2/can/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-06-18 15:01:03.000000 python-can-4.2.2/can/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-06-18 15:01:03.000000 python-can-4.2.2/can/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 15:01:03.000000 python-can-4.2.2/can/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-18 15:01:03.000000 python-can-4.2.2/can/thread_safe_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-18 15:01:03.000000 python-can-4.2.2/can/typechecking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-06-18 15:01:03.000000 python-can-4.2.2/can/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22278 2023-06-18 15:01:03.000000 python-can-4.2.2/can/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:01:11.332160 python-can-4.2.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/asyncio.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/bcm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/bit_timing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/bus.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:01:11.336160 python-can-4.2.2/doc/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/interfaces/canalystii.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/interfaces/cantact.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/interfaces/etas.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2566 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/interfaces/gs_usb.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/interfaces/iscan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/interfaces/ixxat.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/interfaces/kvaser.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/interfaces/neousys.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/interfaces/neovi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/interfaces/nican.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/interfaces/nixnet.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/interfaces/pcan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/interfaces/robotell.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/interfaces/seeedstudio.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/interfaces/serial.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1055 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/interfaces/slcan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/interfaces/socketcan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/interfaces/socketcand.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/interfaces/systec.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/interfaces/udp_multicast.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/interfaces/usb2can.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/interfaces/vector.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/interfaces/virtual.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/interfaces.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/internal-api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/listeners.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/message.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/other-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/plugin-interface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/scripts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8462 2023-06-18 15:01:03.000000 python-can-4.2.2/doc/virtual-interfaces.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-18 15:01:03.000000 python-can-4.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:01:11.336160 python-can-4.2.2/python_can.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-06-18 15:01:11.000000 python-can-4.2.2/python_can.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-06-18 15:01:11.000000 python-can-4.2.2/python_can.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 15:01:11.000000 python-can-4.2.2/python_can.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-18 15:01:11.000000 python-can-4.2.2/python_can.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-18 15:01:11.000000 python-can-4.2.2/python_can.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-18 15:01:03.000000 python-can-4.2.2/requirements-lint.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:01:11.336160 python-can-4.2.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-18 15:01:03.000000 python-can-4.2.2/scripts/can_logconvert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-18 15:01:03.000000 python-can-4.2.2/scripts/can_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-18 15:01:03.000000 python-can-4.2.2/scripts/can_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-18 15:01:03.000000 python-can-4.2.2/scripts/can_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-18 15:01:11.348160 python-can-4.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-06-18 15:01:03.000000 python-can-4.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:01:11.344160 python-can-4.2.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-18 15:01:03.000000 python-can-4.2.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15773 2023-06-18 15:01:03.000000 python-can-4.2.2/test/back2back_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-18 15:01:03.000000 python-can-4.2.2/test/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-18 15:01:03.000000 python-can-4.2.2/test/contextmanager_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:01:11.348160 python-can-4.2.2/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-18 15:01:03.000000 python-can-4.2.2/test/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-06-18 15:01:03.000000 python-can-4.2.2/test/data/example_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-18 15:01:03.000000 python-can-4.2.2/test/data/ip_link_list.json
+-rw-r--r--   0 runner    (1001) docker     (123)   128078 2023-06-18 15:01:03.000000 python-can-4.2.2/test/data/issue_1256.asc
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-18 15:01:03.000000 python-can-4.2.2/test/data/issue_1299.asc
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-06-18 15:01:03.000000 python-can-4.2.2/test/data/logfile.asc
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-18 15:01:03.000000 python-can-4.2.2/test/data/logfile_errorframes.asc
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-18 15:01:03.000000 python-can-4.2.2/test/data/test_CanErrorFrameExt.blf
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-18 15:01:03.000000 python-can-4.2.2/test/data/test_CanErrorFrames.asc
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-18 15:01:03.000000 python-can-4.2.2/test/data/test_CanFdMessage.asc
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-18 15:01:03.000000 python-can-4.2.2/test/data/test_CanFdMessage.blf
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-18 15:01:03.000000 python-can-4.2.2/test/data/test_CanFdMessage64.asc
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-18 15:01:03.000000 python-can-4.2.2/test/data/test_CanFdMessage64.blf
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-18 15:01:03.000000 python-can-4.2.2/test/data/test_CanFdRemoteMessage.asc
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-18 15:01:03.000000 python-can-4.2.2/test/data/test_CanMessage.asc
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-18 15:01:03.000000 python-can-4.2.2/test/data/test_CanMessage.asc.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-18 15:01:03.000000 python-can-4.2.2/test/data/test_CanMessage.blf
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-18 15:01:03.000000 python-can-4.2.2/test/data/test_CanMessage.trc
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-18 15:01:03.000000 python-can-4.2.2/test/data/test_CanMessage2.blf
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-18 15:01:03.000000 python-can-4.2.2/test/data/test_CanMessage_V1_0_BUS1.trc
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-18 15:01:03.000000 python-can-4.2.2/test/data/test_CanMessage_V1_1.trc
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-18 15:01:03.000000 python-can-4.2.2/test/data/test_CanMessage_V2_0_BUS1.trc
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-18 15:01:03.000000 python-can-4.2.2/test/data/test_CanMessage_V2_1.trc
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-18 15:01:03.000000 python-can-4.2.2/test/data/test_CanRemoteMessage.asc
+-rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-06-18 15:01:03.000000 python-can-4.2.2/test/listener_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-06-18 15:01:03.000000 python-can-4.2.2/test/logformats_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-18 15:01:03.000000 python-can-4.2.2/test/message_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-18 15:01:03.000000 python-can-4.2.2/test/network_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-18 15:01:03.000000 python-can-4.2.2/test/notifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-06-18 15:01:03.000000 python-can-4.2.2/test/serial_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-06-18 15:01:03.000000 python-can-4.2.2/test/simplecyclic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13580 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_bit_timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_cantact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22230 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_cyclic_socketcan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_detect_available_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_interface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3367 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_interface_canalystii.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_interface_ixxat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_interface_ixxat_fd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_interface_virtual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_kvaser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_load_file_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_message_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_message_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_message_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_neousys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_neovi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19093 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_pcan.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3930 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24830 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_robotell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_rotating_loggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_slcan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13308 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_socketcan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_socketcan_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_socketcan_loopback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_systec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11232 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47118 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20951 2023-06-18 15:01:03.000000 python-can-4.2.2/test/test_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-18 15:01:03.000000 python-can-4.2.2/test/zero_dlc_test.py
```

### Comparing `python-can-4.2.1/CONTRIBUTORS.txt` & `python-can-4.2.2/CONTRIBUTORS.txt`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/LICENSE.txt` & `python-can-4.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/PKG-INFO` & `python-can-4.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-can
-Version: 4.2.1
+Version: 4.2.2
 Summary: Controller Area Network interface module for Python
 Home-page: https://github.com/hardbyte/python-can
 Author: python-can contributors
 License: LGPL v3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `python-can-4.2.1/README.rst` & `python-can-4.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/__init__.py` & `python-can-4.2.2/can/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 different hardware devices, and a suite of utilities for sending and receiving
 messages on a can bus.
 """
 
 import logging
 from typing import Any, Dict
 
-__version__ = "4.2.1"
+__version__ = "4.2.2"
 __all__ = [
     "ASCReader",
     "ASCWriter",
     "AsyncBufferedReader",
     "BitTiming",
     "BitTimingFd",
     "BLFReader",
```

### Comparing `python-can-4.2.1/can/bit_timing.py` & `python-can-4.2.2/can/bit_timing.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/broadcastmanager.py` & `python-can-4.2.2/can/broadcastmanager.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/bus.py` & `python-can-4.2.2/can/bus.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/ctypesutil.py` & `python-can-4.2.2/can/ctypesutil.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/exceptions.py` & `python-can-4.2.2/can/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interface.py` & `python-can-4.2.2/can/interface.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/__init__.py` & `python-can-4.2.2/can/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/canalystii.py` & `python-can-4.2.2/can/interfaces/canalystii.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/cantact.py` & `python-can-4.2.2/can/interfaces/cantact.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/etas/__init__.py` & `python-can-4.2.2/can/interfaces/etas/__init__.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/etas/boa.py` & `python-can-4.2.2/can/interfaces/etas/boa.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/gs_usb.py` & `python-can-4.2.2/can/interfaces/gs_usb.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/ics_neovi/neovi_bus.py` & `python-can-4.2.2/can/interfaces/ics_neovi/neovi_bus.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/iscan.py` & `python-can-4.2.2/can/interfaces/iscan.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/ixxat/canlib.py` & `python-can-4.2.2/can/interfaces/ixxat/canlib.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/ixxat/canlib_vcinpl.py` & `python-can-4.2.2/can/interfaces/ixxat/canlib_vcinpl.py`

 * *Files 0% similar despite different names*

```diff
@@ -794,14 +794,15 @@
             self._scheduler_resolution = caps.dwClockFreq / caps.dwCmsDivisor
             _canlib.canSchedulerActivate(self._scheduler, constants.TRUE)
         return CyclicSendTask(
             self._scheduler, msgs, period, duration, self._scheduler_resolution
         )
 
     def shutdown(self):
+        super().shutdown()
         if self._scheduler is not None:
             _canlib.canSchedulerClose(self._scheduler)
         _canlib.canChannelClose(self._channel_handle)
         _canlib.canControlStart(self._control_handle, constants.FALSE)
         _canlib.canControlReset(self._control_handle)
         _canlib.canControlClose(self._control_handle)
         _canlib.vciDeviceClose(self._device_handle)
```

### Comparing `python-can-4.2.1/can/interfaces/ixxat/canlib_vcinpl2.py` & `python-can-4.2.2/can/interfaces/ixxat/canlib_vcinpl2.py`

 * *Files 0% similar despite different names*

```diff
@@ -943,14 +943,15 @@
             )  # TODO: confirm
             _canlib.canSchedulerActivate(self._scheduler, constants.TRUE)
         return CyclicSendTask(
             self._scheduler, msgs, period, duration, self._scheduler_resolution
         )
 
     def shutdown(self):
+        super().shutdown()
         if self._scheduler is not None:
             _canlib.canSchedulerClose(self._scheduler)
         _canlib.canChannelClose(self._channel_handle)
         _canlib.canControlStart(self._control_handle, constants.FALSE)
         _canlib.canControlClose(self._control_handle)
         _canlib.vciDeviceClose(self._device_handle)
```

### Comparing `python-can-4.2.1/can/interfaces/ixxat/constants.py` & `python-can-4.2.2/can/interfaces/ixxat/constants.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/ixxat/exceptions.py` & `python-can-4.2.2/can/interfaces/ixxat/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/ixxat/structures.py` & `python-can-4.2.2/can/interfaces/ixxat/structures.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/kvaser/canlib.py` & `python-can-4.2.2/can/interfaces/kvaser/canlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -718,11 +718,12 @@
     canGetChannelData(
         channel,
         canstat.canCHANNELDATA_CHAN_NO_ON_CARD,
         ctypes.byref(number),
         ctypes.sizeof(number),
     )
 
-    return f"{name.value.decode('ascii')}, S/N {serial.value} (#{number.value + 1})"
+    name_decoded = name.value.decode("ascii", errors="replace")
+    return f"{name_decoded}, S/N {serial.value} (#{number.value + 1})"
 
 
 init_kvaser_library()
```

### Comparing `python-can-4.2.1/can/interfaces/kvaser/constants.py` & `python-can-4.2.2/can/interfaces/kvaser/constants.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/kvaser/structures.py` & `python-can-4.2.2/can/interfaces/kvaser/structures.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/neousys/neousys.py` & `python-can-4.2.2/can/interfaces/neousys/neousys.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/nican.py` & `python-can-4.2.2/can/interfaces/nican.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/nixnet.py` & `python-can-4.2.2/can/interfaces/nixnet.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/pcan/basic.py` & `python-can-4.2.2/can/interfaces/pcan/basic.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/pcan/pcan.py` & `python-can-4.2.2/can/interfaces/pcan/pcan.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/robotell.py` & `python-can-4.2.2/can/interfaces/robotell.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/seeedstudio/seeedstudio.py` & `python-can-4.2.2/can/interfaces/seeedstudio/seeedstudio.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/serial/serial_can.py` & `python-can-4.2.2/can/interfaces/serial/serial_can.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/slcan.py` & `python-can-4.2.2/can/interfaces/slcan.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/socketcan/constants.py` & `python-can-4.2.2/can/interfaces/socketcan/constants.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/socketcan/socketcan.py` & `python-can-4.2.2/can/interfaces/socketcan/socketcan.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/socketcan/utils.py` & `python-can-4.2.2/can/interfaces/socketcan/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         return []
 
     log.debug(
         "find_available_interfaces(): detected these interfaces (before filtering): %s",
         output_json,
     )
 
-    interfaces = [i["ifname"] for i in output_json if i["link_type"] == "can"]
+    interfaces = [i["ifname"] for i in output_json if i.get("link_type") == "can"]
     return interfaces
 
 
 def error_code_to_str(code: Optional[int]) -> str:
     """
     Converts a given error code (errno) to a useful and human readable string.
```

### Comparing `python-can-4.2.1/can/interfaces/socketcand/socketcand.py` & `python-can-4.2.2/can/interfaces/socketcand/socketcand.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/systec/constants.py` & `python-can-4.2.2/can/interfaces/systec/constants.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/systec/exceptions.py` & `python-can-4.2.2/can/interfaces/systec/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/systec/structures.py` & `python-can-4.2.2/can/interfaces/systec/structures.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/systec/ucan.py` & `python-can-4.2.2/can/interfaces/systec/ucan.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/systec/ucanbus.py` & `python-can-4.2.2/can/interfaces/systec/ucanbus.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/udp_multicast/bus.py` & `python-can-4.2.2/can/interfaces/udp_multicast/bus.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/udp_multicast/utils.py` & `python-can-4.2.2/can/interfaces/udp_multicast/utils.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/usb2can/serial_selector.py` & `python-can-4.2.2/can/interfaces/usb2can/serial_selector.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/usb2can/usb2canInterface.py` & `python-can-4.2.2/can/interfaces/usb2can/usb2canInterface.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/usb2can/usb2canabstractionlayer.py` & `python-can-4.2.2/can/interfaces/usb2can/usb2canabstractionlayer.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/vector/__init__.py` & `python-can-4.2.2/can/interfaces/vector/__init__.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/vector/canlib.py` & `python-can-4.2.2/can/interfaces/vector/canlib.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/vector/exceptions.py` & `python-can-4.2.2/can/interfaces/vector/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/vector/xlclass.py` & `python-can-4.2.2/can/interfaces/vector/xlclass.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/vector/xldefine.py` & `python-can-4.2.2/can/interfaces/vector/xldefine.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/vector/xldriver.py` & `python-can-4.2.2/can/interfaces/vector/xldriver.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/interfaces/virtual.py` & `python-can-4.2.2/can/interfaces/virtual.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/io/__init__.py` & `python-can-4.2.2/can/io/__init__.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/io/asc.py` & `python-can-4.2.2/can/io/asc.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/io/blf.py` & `python-can-4.2.2/can/io/blf.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/io/canutils.py` & `python-can-4.2.2/can/io/canutils.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/io/csv.py` & `python-can-4.2.2/can/io/csv.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/io/generic.py` & `python-can-4.2.2/can/io/generic.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/io/logger.py` & `python-can-4.2.2/can/io/logger.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/io/mf4.py` & `python-can-4.2.2/can/io/mf4.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,15 +268,19 @@
 class MF4Reader(MessageReader):
     """
     Iterator of CAN messages from a MF4 logging file.
 
     The MF4Reader only supports MF4 files that were recorded with python-can.
     """
 
-    def __init__(self, file: Union[StringPathLike, BinaryIO]) -> None:
+    def __init__(
+        self,
+        file: Union[StringPathLike, BinaryIO],
+        **kwargs: Any,
+    ) -> None:
         """
         :param file: a path-like object or as file-like object to read from
                         If this is a file-like object, is has to be opened in
                         binary read mode, not text read mode.
         """
         if asammdf is None:
             raise NotImplementedError(
```

### Comparing `python-can-4.2.1/can/io/player.py` & `python-can-4.2.2/can/io/player.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/io/printer.py` & `python-can-4.2.2/can/io/printer.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/io/sqlite.py` & `python-can-4.2.2/can/io/sqlite.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/io/trc.py` & `python-can-4.2.2/can/io/trc.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Version 1.1 will be implemented as it is most commonly used
 """
 
 import logging
 import os
 from datetime import datetime, timedelta, timezone
 from enum import Enum
-from typing import Callable, Dict, Generator, List, Optional, TextIO, Union
+from typing import Any, Callable, Dict, Generator, List, Optional, TextIO, Union
 
 from ..message import Message
 from ..typechecking import StringPathLike
 from ..util import channel2int, dlc2len, len2dlc
 from .generic import FileIOMessageWriter, MessageReader
 
 logger = logging.getLogger("can.io.trc")
@@ -42,14 +42,15 @@
     """
 
     file: TextIO
 
     def __init__(
         self,
         file: Union[StringPathLike, TextIO],
+        **kwargs: Any,
     ) -> None:
         """
         :param file: a path-like object or as file-like object to read from
                      If this is a file-like object, is has to opened in text
                      read mode, not binary read mode.
         """
         super().__init__(file, mode="r")
@@ -258,14 +259,15 @@
     )
     FORMAT_MESSAGE_V1_0 = "{msgnr:>6}) {time:7.0f} {id:>8} {dlc:<1} {data}"
 
     def __init__(
         self,
         file: Union[StringPathLike, TextIO],
         channel: int = 1,
+        **kwargs: Any,
     ) -> None:
         """
         :param file: a path-like object or as file-like object to write to
                      If this is a file-like object, is has to opened in text
                      write mode, not binary write mode.
         :param channel: a default channel to use when the message does not
                         have a channel set
```

### Comparing `python-can-4.2.1/can/listener.py` & `python-can-4.2.2/can/listener.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/logconvert.py` & `python-can-4.2.2/can/logconvert.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/logger.py` & `python-can-4.2.2/can/logger.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/message.py` & `python-can-4.2.2/can/message.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/notifier.py` & `python-can-4.2.2/can/notifier.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/player.py` & `python-can-4.2.2/can/player.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/thread_safe_bus.py` & `python-can-4.2.2/can/thread_safe_bus.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/typechecking.py` & `python-can-4.2.2/can/typechecking.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/util.py` & `python-can-4.2.2/can/util.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/can/viewer.py` & `python-can-4.2.2/can/viewer.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/asyncio.rst` & `python-can-4.2.2/doc/asyncio.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/bcm.rst` & `python-can-4.2.2/doc/bcm.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/bit_timing.rst` & `python-can-4.2.2/doc/bit_timing.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/bus.rst` & `python-can-4.2.2/doc/bus.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/configuration.rst` & `python-can-4.2.2/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/development.rst` & `python-can-4.2.2/doc/development.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/history.rst` & `python-can-4.2.2/doc/history.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/index.rst` & `python-can-4.2.2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/installation.rst` & `python-can-4.2.2/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/interfaces/canalystii.rst` & `python-can-4.2.2/doc/interfaces/canalystii.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/interfaces/etas.rst` & `python-can-4.2.2/doc/interfaces/etas.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/interfaces/gs_usb.rst` & `python-can-4.2.2/doc/interfaces/gs_usb.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/interfaces/ixxat.rst` & `python-can-4.2.2/doc/interfaces/ixxat.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/interfaces/kvaser.rst` & `python-can-4.2.2/doc/interfaces/kvaser.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/interfaces/neousys.rst` & `python-can-4.2.2/doc/interfaces/neousys.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/interfaces/neovi.rst` & `python-can-4.2.2/doc/interfaces/neovi.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/interfaces/nican.rst` & `python-can-4.2.2/doc/interfaces/nican.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/interfaces/pcan.rst` & `python-can-4.2.2/doc/interfaces/pcan.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/interfaces/robotell.rst` & `python-can-4.2.2/doc/interfaces/robotell.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/interfaces/seeedstudio.rst` & `python-can-4.2.2/doc/interfaces/seeedstudio.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/interfaces/serial.rst` & `python-can-4.2.2/doc/interfaces/serial.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/interfaces/slcan.rst` & `python-can-4.2.2/doc/interfaces/slcan.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/interfaces/socketcan.rst` & `python-can-4.2.2/doc/interfaces/socketcan.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/interfaces/socketcand.rst` & `python-can-4.2.2/doc/interfaces/socketcand.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/interfaces/systec.rst` & `python-can-4.2.2/doc/interfaces/systec.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/interfaces/udp_multicast.rst` & `python-can-4.2.2/doc/interfaces/udp_multicast.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/interfaces/usb2can.rst` & `python-can-4.2.2/doc/interfaces/usb2can.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/interfaces/vector.rst` & `python-can-4.2.2/doc/interfaces/vector.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/interfaces/virtual.rst` & `python-can-4.2.2/doc/interfaces/virtual.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/interfaces.rst` & `python-can-4.2.2/doc/interfaces.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/internal-api.rst` & `python-can-4.2.2/doc/internal-api.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/listeners.rst` & `python-can-4.2.2/doc/listeners.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/message.rst` & `python-can-4.2.2/doc/message.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/other-tools.rst` & `python-can-4.2.2/doc/other-tools.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/plugin-interface.rst` & `python-can-4.2.2/doc/plugin-interface.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/scripts.rst` & `python-can-4.2.2/doc/scripts.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/doc/virtual-interfaces.rst` & `python-can-4.2.2/doc/virtual-interfaces.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/python_can.egg-info/PKG-INFO` & `python-can-4.2.2/python_can.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-can
-Version: 4.2.1
+Version: 4.2.2
 Summary: Controller Area Network interface module for Python
 Home-page: https://github.com/hardbyte/python-can
 Author: python-can contributors
 License: LGPL v3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `python-can-4.2.1/python_can.egg-info/SOURCES.txt` & `python-can-4.2.2/python_can.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -189,14 +189,15 @@
 test/test_systec.py
 test/test_util.py
 test/test_vector.py
 test/test_viewer.py
 test/zero_dlc_test.py
 test/data/__init__.py
 test/data/example_data.py
+test/data/ip_link_list.json
 test/data/issue_1256.asc
 test/data/issue_1299.asc
 test/data/logfile.asc
 test/data/logfile_errorframes.asc
 test/data/test_CanErrorFrameExt.blf
 test/data/test_CanErrorFrames.asc
 test/data/test_CanFdMessage.asc
```

### Comparing `python-can-4.2.1/python_can.egg-info/requires.txt` & `python-can-4.2.2/python_can.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/setup.cfg` & `python-can-4.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/setup.py` & `python-can-4.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/back2back_test.py` & `python-can-4.2.2/test/back2back_test.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/config.py` & `python-can-4.2.2/test/config.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/contextmanager_test.py` & `python-can-4.2.2/test/contextmanager_test.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/data/example_data.py` & `python-can-4.2.2/test/data/example_data.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/data/issue_1256.asc` & `python-can-4.2.2/test/data/issue_1256.asc`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/data/issue_1299.asc` & `python-can-4.2.2/test/data/issue_1299.asc`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/data/logfile.asc` & `python-can-4.2.2/test/data/logfile.asc`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/data/logfile_errorframes.asc` & `python-can-4.2.2/test/data/logfile_errorframes.asc`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/data/test_CanErrorFrames.asc` & `python-can-4.2.2/test/data/test_CanErrorFrames.asc`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/data/test_CanFdMessage.asc` & `python-can-4.2.2/test/data/test_CanFdMessage.asc`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/data/test_CanFdMessage.blf` & `python-can-4.2.2/test/data/test_CanFdMessage.blf`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/data/test_CanFdMessage64.asc` & `python-can-4.2.2/test/data/test_CanFdMessage64.asc`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/data/test_CanFdMessage64.blf` & `python-can-4.2.2/test/data/test_CanFdMessage64.blf`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/data/test_CanMessage.trc` & `python-can-4.2.2/test/data/test_CanMessage.trc`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/data/test_CanMessage_V1_0_BUS1.trc` & `python-can-4.2.2/test/data/test_CanMessage_V1_0_BUS1.trc`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/data/test_CanMessage_V1_1.trc` & `python-can-4.2.2/test/data/test_CanMessage_V1_1.trc`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/data/test_CanMessage_V2_0_BUS1.trc` & `python-can-4.2.2/test/data/test_CanMessage_V2_0_BUS1.trc`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/data/test_CanMessage_V2_1.trc` & `python-can-4.2.2/test/data/test_CanMessage_V2_1.trc`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/listener_test.py` & `python-can-4.2.2/test/listener_test.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/logformats_test.py` & `python-can-4.2.2/test/logformats_test.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/message_helper.py` & `python-can-4.2.2/test/message_helper.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/network_test.py` & `python-can-4.2.2/test/network_test.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/notifier_test.py` & `python-can-4.2.2/test/notifier_test.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/serial_test.py` & `python-can-4.2.2/test/serial_test.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/simplecyclic_test.py` & `python-can-4.2.2/test/simplecyclic_test.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_bit_timing.py` & `python-can-4.2.2/test/test_bit_timing.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_bus.py` & `python-can-4.2.2/test/test_bus.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_cantact.py` & `python-can-4.2.2/test/test_cantact.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_cyclic_socketcan.py` & `python-can-4.2.2/test/test_cyclic_socketcan.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_detect_available_configs.py` & `python-can-4.2.2/test/test_detect_available_configs.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_interface.py` & `python-can-4.2.2/test/test_interface.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_interface_canalystii.py` & `python-can-4.2.2/test/test_interface_canalystii.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_interface_ixxat.py` & `python-can-4.2.2/test/test_interface_ixxat.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_interface_ixxat_fd.py` & `python-can-4.2.2/test/test_interface_ixxat_fd.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_interface_virtual.py` & `python-can-4.2.2/test/test_interface_virtual.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_kvaser.py` & `python-can-4.2.2/test/test_kvaser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 
 """
 """
 
+import ctypes
 import time
 import unittest
 from unittest.mock import Mock
 
 import pytest
 
 import can
@@ -44,14 +45,34 @@
             self.bus = None
 
     def test_bus_creation(self):
         self.assertIsInstance(self.bus, canlib.KvaserBus)
         self.assertTrue(canlib.canOpenChannel.called)
         self.assertTrue(canlib.canBusOn.called)
 
+    def test_bus_creation_illegal_channel_name(self):
+        # Test if the bus constructor is able to deal with non-ASCII characters
+        def canGetChannelDataMock(
+            channel: ctypes.c_int,
+            param: ctypes.c_int,
+            buf: ctypes.c_void_p,
+            bufsize: ctypes.c_size_t,
+        ):
+            if param == constants.canCHANNELDATA_DEVDESCR_ASCII:
+                buf_char_ptr = ctypes.cast(buf, ctypes.POINTER(ctypes.c_char))
+                for i, char in enumerate(b"hello\x7a\xcb"):
+                    buf_char_ptr[i] = char
+
+        canlib.canGetChannelData = canGetChannelDataMock
+        bus = can.Bus(channel=0, interface="kvaser")
+
+        self.assertTrue(bus.channel_info.startswith("hello"))
+
+        bus.shutdown()
+
     def test_bus_shutdown(self):
         self.bus.shutdown()
         self.assertTrue(canlib.canBusOff.called)
         self.assertTrue(canlib.canClose.called)
 
     def test_filter_setup(self):
         # No filter in constructor
```

### Comparing `python-can-4.2.1/test/test_load_config.py` & `python-can-4.2.2/test/test_load_config.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_load_file_config.py` & `python-can-4.2.2/test/test_load_file_config.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_logger.py` & `python-can-4.2.2/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_message_class.py` & `python-can-4.2.2/test/test_message_class.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_message_filtering.py` & `python-can-4.2.2/test/test_message_filtering.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_message_sync.py` & `python-can-4.2.2/test/test_message_sync.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_neousys.py` & `python-can-4.2.2/test/test_neousys.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_neovi.py` & `python-can-4.2.2/test/test_neovi.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_pcan.py` & `python-can-4.2.2/test/test_pcan.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_player.py` & `python-can-4.2.2/test/test_player.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_robotell.py` & `python-can-4.2.2/test/test_robotell.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_rotating_loggers.py` & `python-can-4.2.2/test/test_rotating_loggers.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_scripts.py` & `python-can-4.2.2/test/test_scripts.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_slcan.py` & `python-can-4.2.2/test/test_slcan.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_socketcan.py` & `python-can-4.2.2/test/test_socketcan.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_socketcan_helpers.py` & `python-can-4.2.2/test/test_socketcan_helpers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 #!/usr/bin/env python
 
 """
 Tests helpers in `can.interfaces.socketcan.socketcan_common`.
 """
 
-import gzip
 import unittest
-from base64 import b64decode
+from pathlib import Path
 from unittest import mock
 
 from can.interfaces.socketcan.utils import error_code_to_str, find_available_interfaces
 
 from .config import IS_LINUX, TEST_INTERFACE_SOCKETCAN
 
 
@@ -38,25 +37,15 @@
         self.assertGreaterEqual(len(result), 3)
         self.assertIn("vcan0", result)
         self.assertIn("vxcan0", result)
         self.assertIn("slcan0", result)
 
     def test_find_available_interfaces_w_patch(self):
         # Contains lo, eth0, wlan0, vcan0, mycustomCan123
-        ip_output_gz_b64 = (
-            "H4sIAAAAAAAAA+2UzW+CMBjG7/wVhrNL+BC29IboEqNSwzQejDEViiMC5aNsmmX/+wpZTGUwDAcP"
-            "y5qmh+d5++bN80u7EXpsfZRnsUTf8yMXn0TQk/u8GqEQM1EMiMjpXoAOGZM3F6mUZxAuhoY55UpL"
-            "fbWoKjO4Hts7pl/kLdc+pDlrrmuaqnNq4vqZU8wSkSTHOeYHIjFOM4poOevKmlpwbfF+4EfHkLil"
-            "PRo/G6vZkrcPKcnjwnOxh/KA8h49JQGOimAkSaq03NFz/B0PiffIOfIXkeumOCtiEiUJXG++bp8S"
-            "5Dooo/WVZeFnvxmYUgsM01fpBmQWfDAN256M7SqioQ2NkWm8LKvGnIU3qTN+xylrV/FdaHrJzmFk"
-            "gkacozuzZMnhtAGkLANFAaoKBgOgaUDXG0F6Hrje7SDVWpDvAYpuIdmJV4dn2cSx9VUuGiFCe25Y"
-            "fwTi4KmW4ptzG0ULGvYPLN1APSqdMN3/82TRtOeqSbW5hmcnzygJTRTJivofcEvAgrAVvgD8aLkv"
-            "/AcAAA=="
-        )
-        ip_output = gzip.decompress(b64decode(ip_output_gz_b64)).decode("ascii")
+        ip_output = (Path(__file__).parent / "data" / "ip_link_list.json").read_text()
 
         with mock.patch("subprocess.check_output") as check_output:
             check_output.return_value = ip_output
             ifs = find_available_interfaces()
 
             self.assertEqual(["vcan0", "mycustomCan123"], ifs)
```

### Comparing `python-can-4.2.1/test/test_socketcan_loopback.py` & `python-can-4.2.2/test/test_socketcan_loopback.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_systec.py` & `python-can-4.2.2/test/test_systec.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_util.py` & `python-can-4.2.2/test/test_util.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_vector.py` & `python-can-4.2.2/test/test_vector.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/test_viewer.py` & `python-can-4.2.2/test/test_viewer.py`

 * *Files identical despite different names*

### Comparing `python-can-4.2.1/test/zero_dlc_test.py` & `python-can-4.2.2/test/zero_dlc_test.py`

 * *Files identical despite different names*

