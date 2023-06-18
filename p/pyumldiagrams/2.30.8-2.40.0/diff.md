# Comparing `tmp/pyumldiagrams-2.30.8.tar.gz` & `tmp/pyumldiagrams-2.40.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyumldiagrams-2.30.8.tar", last modified: Fri Aug  5 18:11:27 2022, max compression
+gzip compressed data, was "pyumldiagrams-2.40.0.tar", last modified: Sun Jun 18 20:51:26 2023, max compression
```

## Comparing `pyumldiagrams-2.30.8.tar` & `pyumldiagrams-2.40.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-05 18:11:27.565134 pyumldiagrams-2.30.8/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7652 2020-08-24 19:39:24.000000 pyumldiagrams-2.30.8/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1665 2022-08-05 18:11:27.565019 pyumldiagrams-2.30.8/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1351 2022-08-05 17:30:51.000000 pyumldiagrams-2.30.8/README.md
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-05 18:11:27.560470 pyumldiagrams-2.30.8/pyumldiagrams/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8957 2022-08-05 00:37:03.000000 pyumldiagrams-2.30.8/pyumldiagrams/BaseDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4584 2022-08-05 02:15:52.000000 pyumldiagrams-2.30.8/pyumldiagrams/Common.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1129 2022-08-05 00:43:50.000000 pyumldiagrams-2.30.8/pyumldiagrams/Defaults.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7203 2022-02-22 21:38:04.000000 pyumldiagrams-2.30.8/pyumldiagrams/Definitions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1090 2022-08-04 20:45:52.000000 pyumldiagrams-2.30.8/pyumldiagrams/IDiagramLine.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1054 2022-02-22 18:13:04.000000 pyumldiagrams-2.30.8/pyumldiagrams/Internal.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2020-08-01 19:41:03.000000 pyumldiagrams-2.30.8/pyumldiagrams/UnsupportedException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      100 2020-08-03 15:47:41.000000 pyumldiagrams-2.30.8/pyumldiagrams/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-05 18:11:27.561581 pyumldiagrams-2.30.8/pyumldiagrams/image/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      959 2022-08-05 01:58:55.000000 pyumldiagrams-2.30.8/pyumldiagrams/image/ImageCommon.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12055 2022-08-05 01:52:26.000000 pyumldiagrams-2.30.8/pyumldiagrams/image/ImageDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      191 2020-08-03 16:50:51.000000 pyumldiagrams-2.30.8/pyumldiagrams/image/ImageFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6681 2022-08-05 01:56:05.000000 pyumldiagrams-2.30.8/pyumldiagrams/image/ImageLine.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       70 2020-08-03 15:48:19.000000 pyumldiagrams-2.30.8/pyumldiagrams/image/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 pyumldiagrams-2.30.8/pyumldiagrams/image/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-05 18:11:27.561936 pyumldiagrams-2.30.8/pyumldiagrams/image/resources/
--rwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)    58088 2012-07-20 15:07:58.000000 pyumldiagrams-2.30.8/pyumldiagrams/image/resources/MonoFonto.ttf
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       67 2020-08-03 15:48:48.000000 pyumldiagrams-2.30.8/pyumldiagrams/image/resources/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 pyumldiagrams-2.30.8/pyumldiagrams/image/resources/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-05 18:11:27.562590 pyumldiagrams-2.30.8/pyumldiagrams/pdf/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1016 2022-08-04 20:30:37.000000 pyumldiagrams-2.30.8/pyumldiagrams/pdf/FPDFExtended.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3274 2022-08-05 01:23:52.000000 pyumldiagrams-2.30.8/pyumldiagrams/pdf/PdfCommon.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11583 2022-08-04 20:29:14.000000 pyumldiagrams-2.30.8/pyumldiagrams/pdf/PdfDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13819 2022-08-04 20:48:55.000000 pyumldiagrams-2.30.8/pyumldiagrams/pdf/PdfLine.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       62 2020-08-01 19:41:03.000000 pyumldiagrams-2.30.8/pyumldiagrams/pdf/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 pyumldiagrams-2.30.8/pyumldiagrams/pdf/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-05 18:11:27.562770 pyumldiagrams-2.30.8/pyumldiagrams/pdf/resources/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       71 2020-08-01 19:41:03.000000 pyumldiagrams-2.30.8/pyumldiagrams/pdf/resources/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 pyumldiagrams-2.30.8/pyumldiagrams/pdf/resources/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 pyumldiagrams-2.30.8/pyumldiagrams/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-05 18:11:27.563148 pyumldiagrams-2.30.8/pyumldiagrams/xmlsupport/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9461 2022-08-05 00:38:47.000000 pyumldiagrams-2.30.8/pyumldiagrams/xmlsupport/ToClassDefinition.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      920 2020-10-14 16:32:41.000000 pyumldiagrams-2.30.8/pyumldiagrams/xmlsupport/XmlConstants.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       68 2020-09-30 15:02:32.000000 pyumldiagrams-2.30.8/pyumldiagrams/xmlsupport/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 pyumldiagrams-2.30.8/pyumldiagrams/xmlsupport/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-05 18:11:27.560950 pyumldiagrams-2.30.8/pyumldiagrams.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1665 2022-08-05 18:11:27.000000 pyumldiagrams-2.30.8/pyumldiagrams.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1699 2022-08-05 18:11:27.000000 pyumldiagrams-2.30.8/pyumldiagrams.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2022-08-05 18:11:27.000000 pyumldiagrams-2.30.8/pyumldiagrams.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       27 2022-08-05 18:11:27.000000 pyumldiagrams-2.30.8/pyumldiagrams.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       20 2022-08-05 18:11:27.000000 pyumldiagrams-2.30.8/pyumldiagrams.egg-info/top_level.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2022-08-05 18:11:27.565173 pyumldiagrams-2.30.8/setup.cfg
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1099 2022-08-05 18:11:20.000000 pyumldiagrams-2.30.8/setup.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-05 18:11:27.563949 pyumldiagrams-2.30.8/tests/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4735 2022-02-22 18:13:04.000000 pyumldiagrams-2.30.8/tests/TestAll.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1251 2020-10-14 00:27:38.000000 pyumldiagrams-2.30.8/tests/TestBase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      115 2020-08-01 14:04:46.000000 pyumldiagrams-2.30.8/tests/TestConstants.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4870 2020-08-02 00:55:00.000000 pyumldiagrams-2.30.8/tests/TestDiagramCommon.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11588 2021-03-20 16:27:02.000000 pyumldiagrams-2.30.8/tests/TestDiagramParent.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1168 2020-08-08 18:58:48.000000 pyumldiagrams-2.30.8/tests/TestTemplate.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5726 2020-12-06 16:37:59.000000 pyumldiagrams-2.30.8/tests/TestToClassDefinition.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2020-08-01 14:04:46.000000 pyumldiagrams-2.30.8/tests/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-05 18:11:27.564254 pyumldiagrams-2.30.8/tests/image/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    16797 2020-12-06 16:37:59.000000 pyumldiagrams-2.30.8/tests/image/TestImageDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    14545 2022-02-22 21:56:03.000000 pyumldiagrams-2.30.8/tests/image/TestImageLine.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2020-08-02 01:01:05.000000 pyumldiagrams-2.30.8/tests/image/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-05 18:11:27.564566 pyumldiagrams-2.30.8/tests/pdf/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    18996 2022-02-22 21:44:29.000000 pyumldiagrams-2.30.8/tests/pdf/TestPdfDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    14717 2022-02-22 18:44:57.000000 pyumldiagrams-2.30.8/tests/pdf/TestPdfLine.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2020-08-01 23:13:31.000000 pyumldiagrams-2.30.8/tests/pdf/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-05 18:11:27.564642 pyumldiagrams-2.30.8/tests/resources/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2020-08-01 14:04:46.000000 pyumldiagrams-2.30.8/tests/resources/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-05 18:11:27.564733 pyumldiagrams-2.30.8/tests/resources/basefiles/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2020-11-11 20:48:00.000000 pyumldiagrams-2.30.8/tests/resources/basefiles/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-05 18:11:27.564810 pyumldiagrams-2.30.8/tests/resources/basefiles/image/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2020-11-11 20:48:29.000000 pyumldiagrams-2.30.8/tests/resources/basefiles/image/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-05 18:11:27.564890 pyumldiagrams-2.30.8/tests/resources/basefiles/pdf/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2020-11-11 20:48:13.000000 pyumldiagrams-2.30.8/tests/resources/basefiles/pdf/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-18 20:51:26.062138 pyumldiagrams-2.40.0/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-07-23 23:19:08.000000 pyumldiagrams-2.40.0/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    41470 2023-06-18 20:51:26.062002 pyumldiagrams-2.40.0/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1351 2022-08-05 17:30:51.000000 pyumldiagrams-2.40.0/README.md
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-18 20:51:26.053315 pyumldiagrams-2.40.0/pyumldiagrams/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8962 2023-06-13 16:54:07.000000 pyumldiagrams-2.40.0/pyumldiagrams/BaseDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4584 2022-08-05 02:15:52.000000 pyumldiagrams-2.40.0/pyumldiagrams/Common.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1129 2022-08-05 00:43:50.000000 pyumldiagrams-2.40.0/pyumldiagrams/Defaults.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7694 2023-06-16 15:46:42.000000 pyumldiagrams-2.40.0/pyumldiagrams/Definitions.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1090 2022-08-04 20:45:52.000000 pyumldiagrams-2.40.0/pyumldiagrams/IDiagramLine.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1234 2023-06-16 03:15:59.000000 pyumldiagrams-2.40.0/pyumldiagrams/Internal.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2020-08-01 19:41:03.000000 pyumldiagrams-2.40.0/pyumldiagrams/UnsupportedException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      100 2020-08-03 15:47:41.000000 pyumldiagrams-2.40.0/pyumldiagrams/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-18 20:51:26.055051 pyumldiagrams-2.40.0/pyumldiagrams/image/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      959 2022-08-05 01:58:55.000000 pyumldiagrams-2.40.0/pyumldiagrams/image/ImageCommon.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12197 2023-06-11 22:14:44.000000 pyumldiagrams-2.40.0/pyumldiagrams/image/ImageDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      191 2020-08-03 16:50:51.000000 pyumldiagrams-2.40.0/pyumldiagrams/image/ImageFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6681 2022-08-05 01:56:05.000000 pyumldiagrams-2.40.0/pyumldiagrams/image/ImageLine.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       70 2020-08-03 15:48:19.000000 pyumldiagrams-2.40.0/pyumldiagrams/image/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 pyumldiagrams-2.40.0/pyumldiagrams/image/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-18 20:51:26.055821 pyumldiagrams-2.40.0/pyumldiagrams/image/resources/
+-rwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)    58088 2012-07-20 15:07:58.000000 pyumldiagrams-2.40.0/pyumldiagrams/image/resources/MonoFonto.ttf
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       67 2020-08-03 15:48:48.000000 pyumldiagrams-2.40.0/pyumldiagrams/image/resources/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 pyumldiagrams-2.40.0/pyumldiagrams/image/resources/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-18 20:51:26.057231 pyumldiagrams-2.40.0/pyumldiagrams/pdf/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1216 2023-06-11 01:37:25.000000 pyumldiagrams-2.40.0/pyumldiagrams/pdf/FPDFExtended.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3517 2023-06-16 03:22:56.000000 pyumldiagrams-2.40.0/pyumldiagrams/pdf/PdfCommon.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11583 2022-08-04 20:29:14.000000 pyumldiagrams-2.40.0/pyumldiagrams/pdf/PdfDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13819 2022-08-04 20:48:55.000000 pyumldiagrams-2.40.0/pyumldiagrams/pdf/PdfLine.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       62 2020-08-01 19:41:03.000000 pyumldiagrams-2.40.0/pyumldiagrams/pdf/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 pyumldiagrams-2.40.0/pyumldiagrams/pdf/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-18 20:51:26.057490 pyumldiagrams-2.40.0/pyumldiagrams/pdf/resources/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       71 2020-08-01 19:41:03.000000 pyumldiagrams-2.40.0/pyumldiagrams/pdf/resources/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 pyumldiagrams-2.40.0/pyumldiagrams/pdf/resources/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 pyumldiagrams-2.40.0/pyumldiagrams/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-18 20:51:26.058181 pyumldiagrams-2.40.0/pyumldiagrams/xmlsupport/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9410 2023-06-16 03:40:53.000000 pyumldiagrams-2.40.0/pyumldiagrams/xmlsupport/ToClassDefinition.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      920 2020-10-14 16:32:41.000000 pyumldiagrams-2.40.0/pyumldiagrams/xmlsupport/XmlConstants.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       68 2020-09-30 15:02:32.000000 pyumldiagrams-2.40.0/pyumldiagrams/xmlsupport/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 pyumldiagrams-2.40.0/pyumldiagrams/xmlsupport/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-18 20:51:26.053919 pyumldiagrams-2.40.0/pyumldiagrams.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    41470 2023-06-18 20:51:26.000000 pyumldiagrams-2.40.0/pyumldiagrams.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1699 2023-06-18 20:51:26.000000 pyumldiagrams-2.40.0/pyumldiagrams.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-06-18 20:51:26.000000 pyumldiagrams-2.40.0/pyumldiagrams.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       27 2023-06-18 20:51:26.000000 pyumldiagrams-2.40.0/pyumldiagrams.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       20 2023-06-18 20:51:26.000000 pyumldiagrams-2.40.0/pyumldiagrams.egg-info/top_level.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-06-18 20:51:26.062173 pyumldiagrams-2.40.0/setup.cfg
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1140 2023-06-18 20:33:44.000000 pyumldiagrams-2.40.0/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-18 20:51:26.059947 pyumldiagrams-2.40.0/tests/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4738 2023-06-17 17:33:32.000000 pyumldiagrams-2.40.0/tests/TestAll.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1251 2020-10-14 00:27:38.000000 pyumldiagrams-2.40.0/tests/TestBase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      115 2020-08-01 14:04:46.000000 pyumldiagrams-2.40.0/tests/TestConstants.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4791 2023-06-17 17:55:41.000000 pyumldiagrams-2.40.0/tests/TestDiagramCommon.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12126 2023-06-18 19:57:48.000000 pyumldiagrams-2.40.0/tests/TestDiagramParent.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1168 2020-08-08 18:58:48.000000 pyumldiagrams-2.40.0/tests/TestTemplate.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5726 2020-12-06 16:37:59.000000 pyumldiagrams-2.40.0/tests/TestToClassDefinition.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2020-08-01 14:04:46.000000 pyumldiagrams-2.40.0/tests/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-18 20:51:26.060679 pyumldiagrams-2.40.0/tests/image/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    16840 2023-06-17 17:22:27.000000 pyumldiagrams-2.40.0/tests/image/TestImageDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    14548 2023-06-17 17:23:21.000000 pyumldiagrams-2.40.0/tests/image/TestImageLine.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2020-08-02 01:01:05.000000 pyumldiagrams-2.40.0/tests/image/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-18 20:51:26.061366 pyumldiagrams-2.40.0/tests/pdf/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    18998 2023-06-17 17:27:21.000000 pyumldiagrams-2.40.0/tests/pdf/TestPdfDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    15689 2023-06-17 17:22:55.000000 pyumldiagrams-2.40.0/tests/pdf/TestPdfLine.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2020-08-01 23:13:31.000000 pyumldiagrams-2.40.0/tests/pdf/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-18 20:51:26.061468 pyumldiagrams-2.40.0/tests/resources/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2020-08-01 14:04:46.000000 pyumldiagrams-2.40.0/tests/resources/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-18 20:51:26.061553 pyumldiagrams-2.40.0/tests/resources/basefiles/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2020-11-11 20:48:00.000000 pyumldiagrams-2.40.0/tests/resources/basefiles/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-18 20:51:26.061657 pyumldiagrams-2.40.0/tests/resources/basefiles/image/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2020-11-11 20:48:29.000000 pyumldiagrams-2.40.0/tests/resources/basefiles/image/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-18 20:51:26.061764 pyumldiagrams-2.40.0/tests/resources/basefiles/pdf/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2020-11-11 20:48:13.000000 pyumldiagrams-2.40.0/tests/resources/basefiles/pdf/__init__.py
```

### Comparing `pyumldiagrams-2.30.8/PKG-INFO` & `pyumldiagrams-2.40.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: pyumldiagrams
-Version: 2.30.8
-Summary: Draw UML diagrams in various formats
-Home-page: https://github.com/hasii2011/pyumldiagrams
-Author: Humberto A. Sanchez II
-Author-email: humberto.a.sanchez.ii@gmail.com
-License: GPL V3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Build Status](https://travis-ci.com/hasii2011/pyumldiagrams.svg?branch=master)](https://travis-ci.com/hasii2011/pyumldiagrams)
 [![PyPI version](https://badge.fury.io/py/pyumldiagrams.svg)](https://badge.fury.io/py/pyumldiagrams)
 [![Documentation Status](https://readthedocs.org/projects/pyumldiagrams/badge/?version=latest)](https://pyumldiagrams.readthedocs.io/en/latest/?badge=latest)
       
 The documentation is on [read the docs](https://pyumldiagrams.readthedocs.io/en/latest/).
```

### Comparing `pyumldiagrams-2.30.8/pyumldiagrams/BaseDiagram.py` & `pyumldiagrams-2.40.0/pyumldiagrams/BaseDiagram.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         Must be overridden by implementors
 
         Args:
             bareFileName:
 
         Returns: a fully qualified name
         """
-        pass
+        return ''
 
     def drawClass(self, classDefinition: ClassDefinition):
         """
         Draw the class diagram defined by the input
         Must be overridden by implementors
 
         Args:
```

### Comparing `pyumldiagrams-2.30.8/pyumldiagrams/Common.py` & `pyumldiagrams-2.40.0/pyumldiagrams/Common.py`

 * *Files identical despite different names*

### Comparing `pyumldiagrams-2.30.8/pyumldiagrams/Defaults.py` & `pyumldiagrams-2.40.0/pyumldiagrams/Defaults.py`

 * *Files identical despite different names*

### Comparing `pyumldiagrams-2.30.8/pyumldiagrams/Definitions.py` & `pyumldiagrams-2.40.0/pyumldiagrams/Definitions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 
 from typing import List
+from typing import NewType
 
 from enum import Enum
 
 from dataclasses import dataclass
 from dataclasses import field
 
 from pyumldiagrams.Defaults import TOP_MARGIN
 from pyumldiagrams.Defaults import LEFT_MARGIN
 from pyumldiagrams.Defaults import DEFAULT_HORIZONTAL_GAP
 from pyumldiagrams.Defaults import DEFAULT_VERTICAL_GAP
 from pyumldiagrams.UnsupportedException import UnsupportedException
 
-ClassName = str
+
+ClassName = NewType('ClassName', str)
 
 
 @dataclass
 class Position:
     """
     The x and y coordinates are in screen/display resolution.  Diagramming modules may
     convert these to appropriate positions based on the rendering technology.
@@ -27,14 +29,18 @@
     """
     y: int = 0
     """
     The y-axis (vertical) ordinate
     """
 
 
+def createPositionFactory() -> Position:
+    return Position()
+
+
 @dataclass
 class DiagramPadding:
     """
     todo::  These should move to the Internal package
     """
 
     topMargin:  int = TOP_MARGIN
@@ -69,14 +75,18 @@
     """
     height: int = 100
     """
     The height of the shape
     """
 
 
+def createSizeFactory() -> Size:
+    return Size()
+
+
 class DefinitionType(Enum):
     """
     Defines the visibility of either methods or fields
     """
     Public    = '+'
     Private   = '-'
     Protected = '#'
@@ -135,53 +145,61 @@
     """
     parameters: Parameters = field(default_factory=list)
     """
     Define the parameters for a particular method
     """
 
 
-Methods = List[MethodDefinition]
+Methods = NewType('Methods', List[MethodDefinition])
 """
 Syntactic sugar to define a list of methods.
 """
 
 
+def createMethodsFactory() -> Methods:
+    return Methods([])
+
+
 @dataclass
 class FieldDefinition(ParameterDefinition):
     """
     Defines a single instance variable;  Seems funny to inherit from a
     parameter definition.
     """
     visibility: DefinitionType = DefinitionType.Public
     """
     Defines the field visibility.  See `DefinitionType`
     """
 
 
-Fields = List[FieldDefinition]
+Fields = NewType('Fields', List[FieldDefinition])
+
+
+def createFieldsFactory() -> Fields:
+    return Fields([])
 
 
 @dataclass
 class ClassDefinition(BaseDefinition):
     """
     The class definition.  Currently, does not support instance properties.
     """
-    size:     Size     = Size()
+    size:     Size     = field(default_factory=createSizeFactory)
     """
     The size of UML class symbol.  See `Size`
     """
-    position: Position = Position(0, 0)
+    position: Position = field(default_factory=createPositionFactory)
     """
     The position of the UML class symbol.  See `Position`
     """
-    methods: Methods   = field(default_factory=list)
+    methods: Methods   = field(default_factory=createMethodsFactory)
     """
     The list of methods this class implements.  
     """
-    fields: Fields = field(default_factory=list)
+    fields:  Fields    = field(default_factory=createFieldsFactory)
     """
     The list of instance variables this class defines.
     """
     displayStereotype:  bool = True
     """
     If true display the class stereotype when drawing the class diagram
     """
@@ -289,19 +307,19 @@
     Defines a rectangle
     """
 
     renderStyle: RenderStyle = RenderStyle.Draw
     """
     How to draw the rectangle.  See `RenderStyle`
     """
-    position:    Position    = Position(0, 0)
+    position:    Position    = field(default_factory=createPositionFactory)
     """
     Where to put the rectangle.  See `Position`
     """
-    size:        Size        = Size(0, 0)
+    size:        Size        = field(default_factory=createSizeFactory)
     """
     The rectangle size.  See `Size`
     """
 
 
 @dataclass
 class EllipseDefinition(RectangleDefinition):
```

### Comparing `pyumldiagrams-2.30.8/pyumldiagrams/IDiagramLine.py` & `pyumldiagrams-2.40.0/pyumldiagrams/IDiagramLine.py`

 * *Files identical despite different names*

### Comparing `pyumldiagrams-2.30.8/pyumldiagrams/Internal.py` & `pyumldiagrams-2.40.0/pyumldiagrams/Internal.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 
-from dataclasses import dataclass
 from typing import List
 from typing import Union
 
+from dataclasses import dataclass
+from dataclasses import field
+
 
 @dataclass(eq=True)
 class InternalPosition:
     """
     The x and y coordinates are relative to the diagramming method.  For pdf
     documents they are in points.  For images, they are in pixels.  In all cases, the position is
     adjusted for left and right margins plus vertical and horizontal gaps.
     """
     x: int = 0
     y: int = 0
 
 
+def createInternalPositionFactory() -> InternalPosition:
+    return InternalPosition()
+
+
 @dataclass
 class SeparatorPosition(InternalPosition):
     pass
 
 
 ArrowPoints   = List[InternalPosition]
 DiamondPoints = List[InternalPosition]
@@ -28,9 +34,9 @@
 @dataclass
 class ScanPoints:
     """
     Used by diagramming methods that cannot fill in a polygon.  In that case, the diagrammer
     scans these points to determine if they are in the polygon.  If they are then presumably the
     diagramming method will draw a dot at the specified point to simulate a fill.
     """
-    startScan: InternalPosition = InternalPosition(0, 0)
-    endScan:   InternalPosition = InternalPosition(0, 0)
+    startScan: InternalPosition = field(default_factory=createInternalPositionFactory)
+    endScan:   InternalPosition = field(default_factory=createInternalPositionFactory)
```

### Comparing `pyumldiagrams-2.30.8/pyumldiagrams/image/ImageCommon.py` & `pyumldiagrams-2.40.0/pyumldiagrams/image/ImageCommon.py`

 * *Files identical despite different names*

### Comparing `pyumldiagrams-2.30.8/pyumldiagrams/image/ImageDiagram.py` & `pyumldiagrams-2.40.0/pyumldiagrams/image/ImageDiagram.py`

 * *Files 4% similar despite different names*

```diff
@@ -214,16 +214,18 @@
         self.logger.debug(f'Class Symbol {xy=}')
         imgDraw.rectangle(xy=xy, fill=None, outline=ImageDiagram.DEFAULT_LINE_COLOR, width=1)
 
     def _drawClassName(self, classDefinition: ClassDefinition, rectX: float, rectY: float, symbolWidth: float):
 
         imgDraw: ImageDraw = self._imgDraw
 
-        nameWidth, nameHeight = imgDraw.textsize(text=classDefinition.name, font=self._font)
+        # nameWidth, nameHeight = imgDraw.textsize(text=classDefinition.name, font=self._font)
 
+        left, top, right, bottom = imgDraw.textbbox(xy=(0, 0), text=classDefinition.name, font=self._font)
+        nameWidth = right - left
         textX: float = rectX + ((symbolWidth / 2) - (nameWidth / 2))
         textY: float = rectY + (self._fontSize / 2)
 
         xy = (textX, textY)
         self.logger.debug(f'ClassName {xy=}')
         imgDraw.text(xy=xy, fill=ImageDiagram.DEFAULT_TEXT_COLOR, font=self._font, text=classDefinition.name)
```

### Comparing `pyumldiagrams-2.30.8/pyumldiagrams/image/ImageLine.py` & `pyumldiagrams-2.40.0/pyumldiagrams/image/ImageLine.py`

 * *Files identical despite different names*

### Comparing `pyumldiagrams-2.30.8/pyumldiagrams/image/resources/MonoFonto.ttf` & `pyumldiagrams-2.40.0/pyumldiagrams/image/resources/MonoFonto.ttf`

 * *Files identical despite different names*

### Comparing `pyumldiagrams-2.30.8/pyumldiagrams/pdf/FPDFExtended.py` & `pyumldiagrams-2.40.0/pyumldiagrams/pdf/FPDFExtended.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,18 +23,21 @@
     def header(self):
 
         self.set_font('Arial', 'B', 15)
         # Move to the right
         self.cell(80)
 
         textWidth: int = self.get_string_width(self._headerText)
-        self.cell(w=textWidth, h=10, txt=f'{self._headerText}', border=0, ln=0, align='L')
+        # self.cell(w=textWidth, h=10, txt=f'{self._headerText}', border=0, ln=0, align='L')
+        self.cell(w=textWidth, h=10, txt=f'{self._headerText}', border=0, align='L')
         # Line break
         self.ln(20)
 
     def footer(self):
 
         self.set_y(-15)
 
         self.set_font('Arial', 'I', 15)
         # Print Left Aligned page number
-        self.cell(0, 10, 'Page %s' % self.page_no(), 0, 0, 'L')
+        # self.cell(0, 10, 'Page %s' % self.page_no(), 0, 0, 'L')
+        pageNum: str = f'Page {self.page_no()}'
+        self.cell(w=0, h=10, txt=pageNum, border=0, align='L')
```

### Comparing `pyumldiagrams-2.30.8/pyumldiagrams/pdf/PdfCommon.py` & `pyumldiagrams-2.40.0/pyumldiagrams/pdf/PdfCommon.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 
 from dataclasses import dataclass
+from dataclasses import field
 
 from pyumldiagrams.Common import Common
 from pyumldiagrams.Definitions import Position
 
 from pyumldiagrams.Defaults import LEFT_MARGIN
 from pyumldiagrams.Defaults import TOP_MARGIN
 
@@ -14,24 +15,32 @@
 
 @dataclass
 class Coordinates:
     x: int = 0
     y: int = 0
 
 
+def createCoordinatesFactory() -> Coordinates:
+    return Coordinates()
+
+
 @dataclass
 class Dimensions:
     width:  int = 0
     height: int = 0
 
 
+def createDimensionsFactory() -> Dimensions:
+    return Dimensions()
+
+
 @dataclass
 class PdfShapeDefinition:
-    coordinates: Coordinates = Coordinates()
-    dimensions:  Dimensions  = Dimensions()
+    coordinates: Coordinates = field(default_factory=createCoordinatesFactory)
+    dimensions:  Dimensions  = field(default_factory=createDimensionsFactory)
 
 
 class PdfCommon(Common):
 
     @classmethod
     def toPdfPoints(cls, pixelNumber: float, dpi: int) -> int:
         """
```

### Comparing `pyumldiagrams-2.30.8/pyumldiagrams/pdf/PdfDiagram.py` & `pyumldiagrams-2.40.0/pyumldiagrams/pdf/PdfDiagram.py`

 * *Files identical despite different names*

### Comparing `pyumldiagrams-2.30.8/pyumldiagrams/pdf/PdfLine.py` & `pyumldiagrams-2.40.0/pyumldiagrams/pdf/PdfLine.py`

 * *Files identical despite different names*

### Comparing `pyumldiagrams-2.30.8/pyumldiagrams/xmlsupport/ToClassDefinition.py` & `pyumldiagrams-2.40.0/pyumldiagrams/xmlsupport/ToClassDefinition.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from pyumldiagrams.Definitions import Methods
 from pyumldiagrams.Definitions import ParameterDefinition
 from pyumldiagrams.Definitions import Parameters
 from pyumldiagrams.Definitions import Position
 from pyumldiagrams.Definitions import Size
 from pyumldiagrams.Definitions import UmlLineDefinition
 from pyumldiagrams.Definitions import UmlLineDefinitions
+from pyumldiagrams.Definitions import createMethodsFactory
 
 from pyumldiagrams.UnsupportedException import UnsupportedException
 
 from pyumldiagrams.xmlsupport.XmlConstants import ATTR_DEFAULT_VALUE
 from pyumldiagrams.xmlsupport.XmlConstants import ATTR_DISPLAY_PARAMETERS
 from pyumldiagrams.xmlsupport.XmlConstants import ATTR_HEIGHT
 from pyumldiagrams.xmlsupport.XmlConstants import ATTR_LINK_DESTINATION_ANCHOR_X
@@ -69,37 +70,36 @@
 
     def generateClassDefinitions(self):
 
         graphicClassNodes: NodeList = self._documentNode.getElementsByTagName(ELEMENT_GRAPHIC_CLASS)
 
         self.logger.debug(f'{graphicClassNodes=}')
 
-        for xmlGraphicClass in graphicClassNodes:
+        for xmlGraphicClassNode in graphicClassNodes:
 
-            xmlGraphicClass: Element = cast(Element, xmlGraphicClass)
+            xmlGraphicClass: Element = cast(Element, xmlGraphicClassNode)
 
-            height: float = float(xmlGraphicClass.getAttribute(ATTR_HEIGHT))
-            width:  float = float(xmlGraphicClass.getAttribute(ATTR_WIDTH))
-            x:      float = float(xmlGraphicClass.getAttribute(ATTR_X))
-            y:      float = float(xmlGraphicClass.getAttribute(ATTR_Y))
+            height: int = int(xmlGraphicClass.getAttribute(ATTR_HEIGHT))
+            width:  int = int(xmlGraphicClass.getAttribute(ATTR_WIDTH))
+            x:      int = int(xmlGraphicClass.getAttribute(ATTR_X))
+            y:      int = int(xmlGraphicClass.getAttribute(ATTR_Y))
 
             xmlClass:  Element = xmlGraphicClass.getElementsByTagName(ELEMENT_MODEL_CLASS)[0]
             className: str     = xmlClass.getAttribute(ATTR_NAME)
 
             displayMethods:    bool = self._stringToBoolean(xmlClass.getAttribute(ATTR_SHOW_METHODS))
             displayFields:     bool = self._stringToBoolean(xmlClass.getAttribute(ATTR_SHOW_FIELDS))
             displayStereotype: bool = self._stringToBoolean(xmlClass.getAttribute(ATTR_SHOW_STEREOTYPE))
 
             displayParametersStr: str = xmlClass.getAttribute(ATTR_DISPLAY_PARAMETERS)
-            displayMethodParameters: DisplayMethodParameters
 
             if displayParametersStr is None or displayParametersStr == '':
                 displayMethodParameters: DisplayMethodParameters = DisplayMethodParameters.UNSPECIFIED
             else:
-                displayMethodParameters: DisplayMethodParameters = DisplayMethodParameters(displayParametersStr)
+                displayMethodParameters = DisplayMethodParameters(displayParametersStr)
 
             classDef: ClassDefinition = ClassDefinition(name=className)
 
             classDef.displayMethods    = displayMethods
             classDef.displayFields     = displayFields
             classDef.displayStereotype = displayStereotype
             classDef.displayMethodParameters = displayMethodParameters
@@ -113,15 +113,15 @@
             classDef.methods = self.generateMethods(xmlClass=xmlClass)
 
             self.logger.debug(f'{classDef=}')
             self._classDefinitions.append(classDef)
 
     def generateMethods(self, xmlClass: Element) -> Methods:
 
-        methods: Methods = []
+        methods: Methods = createMethodsFactory()
 
         for xmlMethod in xmlClass.getElementsByTagName(ELEMENT_MODEL_METHOD):
             methodName: str = xmlMethod.getAttribute(ATTR_NAME)
             self.logger.debug(f'{methodName=}')
 
             method: MethodDefinition = MethodDefinition(name=methodName)
 
@@ -131,43 +131,43 @@
 
         return methods
 
     def generateUmlLineDefinitions(self):
 
         graphicLinkNodes: NodeList = self._documentNode.getElementsByTagName(ELEMENT_GRAPHIC_LINK)
 
-        for xmlGraphicLink in graphicLinkNodes:
+        for graphicLinkNode in graphicLinkNodes:
 
-            xmlGraphicLink: Element = cast(Element, xmlGraphicLink)
+            xmlGraphicLink: Element = cast(Element, graphicLinkNode)
 
             xmlLink:       Element  = xmlGraphicLink.getElementsByTagName(ELEMENT_MODEL_LINK)[0]
             controlPoints: NodeList = xmlGraphicLink.getElementsByTagName(ELEMENT_CONTROL_POINT)
 
-            srcX: float = float(xmlGraphicLink.getAttribute(ATTR_LINK_SOURCE_ANCHOR_X))
-            srcY: float = float(xmlGraphicLink.getAttribute(ATTR_LINK_SOURCE_ANCHOR_Y))
+            srcX: int = int(xmlGraphicLink.getAttribute(ATTR_LINK_SOURCE_ANCHOR_X))
+            srcY: int = int(xmlGraphicLink.getAttribute(ATTR_LINK_SOURCE_ANCHOR_Y))
 
             strType:  str      = xmlLink.getAttribute(ATTR_TYPE)
             lineType: LineType = LineType.toEnum(strType)
 
             srcPosition: Position = Position(x=srcX, y=srcY)
             linePositions: LinePositions = [srcPosition]
             umlLineDefinition: UmlLineDefinition = UmlLineDefinition(linePositions=linePositions, lineType=lineType)
 
-            for controlPoint in controlPoints:
+            for point in controlPoints:
 
-                controlPoint: Element = cast(Element, controlPoint)
+                controlPoint: Element = cast(Element, point)
 
                 self.logger.debug(f'{controlPoint=}')
-                x: float = float(controlPoint.getAttribute(ATTR_X))
-                y: float = float(controlPoint.getAttribute(ATTR_Y))
+                x: int = int(controlPoint.getAttribute(ATTR_X))
+                y: int = int(controlPoint.getAttribute(ATTR_Y))
                 bendPosition: Position = Position(x=x, y=y)
                 linePositions.append(bendPosition)
 
-            destX: float = float(xmlGraphicLink.getAttribute(ATTR_LINK_DESTINATION_ANCHOR_X))
-            destY: float = float(xmlGraphicLink.getAttribute(ATTR_LINK_DESTINATION_ANCHOR_Y))
+            destX: int = int(xmlGraphicLink.getAttribute(ATTR_LINK_DESTINATION_ANCHOR_X))
+            destY: int = int(xmlGraphicLink.getAttribute(ATTR_LINK_DESTINATION_ANCHOR_Y))
 
             destPosition: Position = Position(x=destX, y=destY)
 
             linePositions.append(destPosition)
             self.logger.debug(f'{umlLineDefinition=}')
             self._umlLineDefinitions.append(umlLineDefinition)
```

### Comparing `pyumldiagrams-2.30.8/pyumldiagrams/xmlsupport/XmlConstants.py` & `pyumldiagrams-2.40.0/pyumldiagrams/xmlsupport/XmlConstants.py`

 * *Files identical despite different names*

### Comparing `pyumldiagrams-2.30.8/pyumldiagrams.egg-info/SOURCES.txt` & `pyumldiagrams-2.40.0/pyumldiagrams.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyumldiagrams-2.30.8/setup.py` & `pyumldiagrams-2.40.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,31 +2,32 @@
 from setuptools import setup
 from setuptools import find_packages
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
-README = (HERE / "README.md").read_text()
+README  = (HERE / "README.md").read_text()
+LICENSE = (HERE / 'LICENSE').read_text()
 
 setup(
     name='pyumldiagrams',
-    version='2.30.8',
+    version='2.40.0',
     description='Draw UML diagrams in various formats',
     author='Humberto A. Sanchez II',
     author_email='humberto.a.sanchez.ii@gmail.com',
     long_description=README,
     long_description_content_type='text/markdown',
-    license='GPL V3',
+    license=LICENSE,
     url='https://github.com/hasii2011/pyumldiagrams',
     packages=find_packages(),
     include_package_data=False,
     package_data={
         'pyumldiagrams.image.resources': ['*.ttf', 'pyumldiagrams/image/resources/*.ttf', 'py.typed'],
         'pyumldiagrams':               ['py.typed'],
         'pyumldiagrams.image':         ['py.typed'],
         'pyumldiagrams.pdf':           ['py.typed'],
         'pyumldiagrams.pdf.resources': ['py.typed'],
         'pyumldiagrams.xmlsupport':    ['py.typed'],
     },
-    install_requires=['fpdf2>=2.5.4', 'Pillow>=9.1.1']
+    install_requires=['fpdf2>=2.7.4', 'Pillow>=9.5.0']
 )
```

### Comparing `pyumldiagrams-2.30.8/tests/TestAll.py` & `pyumldiagrams-2.40.0/tests/TestAll.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     """
     The class that can run our unit tests in various formats
     """
     REPORT_NAME: str = 'PDFDiagramming'
     NOT_TESTS:   List[str] = ['TestAll', 'TestTemplate', 'TestBase', 'TestConstants', 'TestDiagramParent']
 
     VERBOSITY_QUIET:   int = 0  # Print the total numbers of tests executed and the global result
-    VERBOSITY_DEFAULT: int = 1  # VERBOSITY_QUIET plus a dot for every successful test or a F for every failure
+    VERBOSITY_DEFAULT: int = 1  # VERBOSITY_QUIET plus a dot for every successful test or an 'F' for every failure
     VERBOSITY_VERBOSE: int = 2  # Print help string of every test and the result
     VERBOSITY_LOUD:    int = 3  # ??
 
     def __init__(self):
 
         self._setupSystemLogging()
```

### Comparing `pyumldiagrams-2.30.8/tests/TestBase.py` & `pyumldiagrams-2.40.0/tests/TestBase.py`

 * *Files identical despite different names*

### Comparing `pyumldiagrams-2.30.8/tests/TestDiagramCommon.py` & `pyumldiagrams-2.40.0/tests/TestDiagramCommon.py`

 * *Files 18% similar despite different names*

```diff
@@ -50,97 +50,97 @@
     def setUpClass(cls):
         TestBase.setUpLogging()
         TestDiagramCommon.clsLogger = getLogger(__name__)
 
     def setUp(self):
         self.logger: Logger = TestDiagramCommon.clsLogger
         self.diamond: PolygonPoints = [
-            InternalPosition(1118.0, 460.0),
-            InternalPosition(1122.0, 469.0717),
-            InternalPosition(1114.0, 469.0717),
-            InternalPosition(1118.0, 476.0)
+            InternalPosition(1118, 460),
+            InternalPosition(1122, 469),
+            InternalPosition(1114, 469),
+            InternalPosition(1118, 476)
         ]
         self.arrow: PolygonPoints = [
-            InternalPosition(1122.0, 469.0717),
-            InternalPosition(1118.0, 476.0),
-            InternalPosition(1114.0, 469.0717)
+            InternalPosition(1122, 469),
+            InternalPosition(1118, 476),
+            InternalPosition(1114, 469)
         ]
 
     def tearDown(self):
         pass
 
     def testPointLeftOfDiamond(self):
 
-        notInPolygon: InternalPosition = InternalPosition(0.0, 0.0)
+        notInPolygon: InternalPosition = InternalPosition(0, 0)
         actualAns:    bool = PdfCommon.pointInsidePolygon(pos=notInPolygon, polygon=self.diamond)
 
         self.assertFalse(actualAns, 'Diamond check is bad')
 
     def testInCenterOfDiamond(self):
 
-        inPolygon: InternalPosition = InternalPosition(1118.0, 470.0)
+        inPolygon: InternalPosition = InternalPosition(1118, 470)
         actualAns: bool = PdfCommon.pointInsidePolygon(pos=inPolygon, polygon=self.diamond)
 
         self.assertTrue(actualAns, 'Diamond check in center of diamond is bad')
 
     def testPointRightOfDiamond(self):
 
-        notInPolygon: InternalPosition = InternalPosition(1122.0, 490.0)
+        notInPolygon: InternalPosition = InternalPosition(1122, 490)
         actualAns:    bool = PdfCommon.pointInsidePolygon(pos=notInPolygon, polygon=self.diamond)
 
         self.assertFalse(actualAns, 'Diamond check is bad')
 
     def testPointLeftOfArrow(self):
 
-        notInPolygon: InternalPosition = InternalPosition(0.0, 0.0)
+        notInPolygon: InternalPosition = InternalPosition(0, 0)
         actualAns:    bool = PdfCommon.pointInsidePolygon(pos=notInPolygon, polygon=self.arrow)
 
         self.assertFalse(actualAns, 'Arrow check is bad')
 
     def testInCenterOfArrow(self):
 
-        inPolygon: InternalPosition = InternalPosition(1118.0, 472.0)
+        inPolygon: InternalPosition = InternalPosition(1118, 472)
         actualAns: bool = PdfCommon.pointInsidePolygon(pos=inPolygon, polygon=self.arrow)
 
         self.assertTrue(actualAns, 'Diamond check is bad')
 
     def testPointRightOfArrow(self):
 
-        notInPolygon: InternalPosition = InternalPosition(1122.0, 490.0)
+        notInPolygon: InternalPosition = InternalPosition(1122, 490)
         actualAns:    bool = PdfCommon.pointInsidePolygon(pos=notInPolygon, polygon=self.arrow)
 
         self.assertFalse(actualAns, 'Diamond check is bad')
 
     def testBuildScanPointsForArrow(self):
 
         scanPoints: ScanPoints = PdfCommon.buildScanPoints(points=self.arrow)
 
-        self.assertEqual(1114.0, scanPoints.startScan.x, 'Minimum X not correct for arrow')
-        self.assertEqual(469.0717,  scanPoints.startScan.y, 'Minimum Y not correct for arrow')
+        self.assertEqual(1114, scanPoints.startScan.x, 'Minimum X not correct for arrow')
+        self.assertEqual(469.,  scanPoints.startScan.y, 'Minimum Y not correct for arrow')
 
-        self.assertEqual(1122.0, scanPoints.endScan.x, 'Max x is not correct for arrow')
-        self.assertEqual(476.0, scanPoints.endScan.y, 'Max y is not correct for arrow')
+        self.assertEqual(1122, scanPoints.endScan.x, 'Max x is not correct for arrow')
+        self.assertEqual(476, scanPoints.endScan.y, 'Max y is not correct for arrow')
 
     def testBuildScanPointsForDiamond(self):
 
         scanPoints: ScanPoints = PdfCommon.buildScanPoints(points=self.diamond)
 
-        self.assertEqual(1114.0, scanPoints.startScan.x, 'Minimum X not correct for diamond')
-        self.assertEqual(460.0, scanPoints.startScan.y, 'Minimum Y not correct for diamond')
+        self.assertEqual(1114, scanPoints.startScan.x, 'Minimum X not correct for diamond')
+        self.assertEqual(460, scanPoints.startScan.y, 'Minimum Y not correct for diamond')
 
-        self.assertEqual(1122.0, scanPoints.endScan.x, 'Max x is not correct for diamond')
-        self.assertEqual(476.0, scanPoints.endScan.y, 'Max y is not correct for diamond')
+        self.assertEqual(1122, scanPoints.endScan.x, 'Max x is not correct for diamond')
+        self.assertEqual(476, scanPoints.endScan.y, 'Max y is not correct for diamond')
 
 
 def suite() -> TestSuite:
     """You need to change the name of the test class here also."""
     import unittest
 
     testSuite: TestSuite = TestSuite()
-    # noinspection PyUnresolvedReferences
-    testSuite.addTest(unittest.makeSuite(TestDiagramCommon))
+
+    testSuite.addTest(unittest.defaultTestLoader.loadTestsFromTestCase(testCaseClass=TestDiagramCommon))
 
     return testSuite
 
 
 if __name__ == '__main__':
     unitTestMain()
```

### Comparing `pyumldiagrams-2.30.8/tests/TestDiagramParent.py` & `pyumldiagrams-2.40.0/tests/TestDiagramParent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,16 @@
-from datetime import datetime
+
 from typing import final
 
-from os import system as osSystem
+from subprocess import run as subProcessRun
+from subprocess import CompletedProcess
+
+from datetime import datetime
+from datetime import timezone
+from datetime import timedelta
 
 from pkg_resources import resource_filename
 
 from pyumldiagrams.BaseDiagram import BaseDiagram
 
 from pyumldiagrams.Definitions import ClassDefinition
 from pyumldiagrams.Definitions import DefinitionType
@@ -30,44 +35,51 @@
 class TestDiagramParent(TestBase):
 
     UNIT_TEST_HEADER:               final = 'Unit Test Header'
     UNIT_TEST_SOPHISTICATED_HEADER: final = 'Pyut Export Version 6.0'
 
     BASE_TEST_CLASS_NAME: str = 'TestClassName'
 
+    # noinspection SpellCheckingInspection
     BASE_FILES_PACKAGE_NAME:          str = f'{TestBase.RESOURCES_PACKAGE_NAME}.basefiles'
     BASE_IMAGE_RESOURCE_PACKAGE_NAME: str = f'{BASE_FILES_PACKAGE_NAME}.image'
     BASE_PDF_RESOURCE_PACKAGE_NAME:   str = f'{BASE_FILES_PACKAGE_NAME}.pdf'
 
     EXTERNAL_DIFF_PROGRAM:    str = 'diff'
+    # noinspection SpellCheckingInspection
     EXTERNAL_PDF_DIFF_SCRIPT: str = './scripts/diffpdf.sh'
 
     STANDARD_SUFFIX: str = '-Standard'
 
-    KNOWABLE_DATE: datetime = datetime(2020, 3, 1, 8, 30)
+    KNOWABLE_DATE: datetime = datetime(2020, 3, 1, 8, 30, tzinfo=timezone(offset=timedelta(), name='America/Chicago'))
 
     def _getFullyQualifiedImagePath(self, imageFileName: str) -> str:
 
         fqFileName: str = resource_filename(TestDiagramParent.BASE_IMAGE_RESOURCE_PACKAGE_NAME, imageFileName)
         return fqFileName
 
     def _getFullyQualifiedPdfPath(self, pdfFileName: str) -> str:
 
         fqFileName: str = resource_filename(TestDiagramParent.BASE_PDF_RESOURCE_PACKAGE_NAME, pdfFileName)
         return fqFileName
 
-    def _runDiff(self, baseFileName: str, standardFileName) -> int:
+    def _runDiff(self, baseFileName: str, standardFileName: str, diffProgram: str = EXTERNAL_DIFF_PROGRAM) -> int:
 
-        status: int = osSystem(f'{TestDiagramParent.EXTERNAL_DIFF_PROGRAM} {baseFileName} {standardFileName}')
+        command: str = f'{diffProgram} {baseFileName} {standardFileName}'
+        completedProcess: CompletedProcess = subProcessRun([command], shell=True, capture_output=True, text=True, check=False)
 
-        return status
+        return completedProcess.returncode
 
     def _runPdfDiff(self, baseFileName: str, standardFileName) -> int:
-
-        status: int = osSystem(f'{TestDiagramParent.EXTERNAL_PDF_DIFF_SCRIPT} {baseFileName} {standardFileName}')
+        """
+        """
+        status: int = self._runDiff(baseFileName=baseFileName,
+                                    standardFileName=standardFileName,
+                                    diffProgram=TestDiagramParent.EXTERNAL_PDF_DIFF_SCRIPT
+                                    )
 
         return status
 
     def _buildCar(self) -> ClassDefinition:
 
         car: ClassDefinition = ClassDefinition(name='Car', position=Position(107, 30), size=Size(width=266, height=100))
 
@@ -170,40 +182,40 @@
         lineDefinitions: UmlLineDefinitions = [
             opieToCat, eCarToCar
         ]
 
         return lineDefinitions
 
     def _buildTopClass(self) -> ClassDefinition:
-        top: ClassDefinition = ClassDefinition(name='TopClass', position=Position(409.0, 159.0), size=Size(height=100, width=113))
+        top: ClassDefinition = ClassDefinition(name='TopClass', position=Position(409, 159), size=Size(height=100, width=113))
         return top
 
     def _buildLeftClass(self) -> ClassDefinition:
-        left: ClassDefinition = ClassDefinition(name='LeftClass', position=Position(266.0, 359.0), size=Size(height=99.0, width=127.0))
+        left: ClassDefinition = ClassDefinition(name='LeftClass', position=Position(266, 359), size=Size(height=99, width=127))
         return left
 
     def _buildRightClass(self) -> ClassDefinition:
-        right: ClassDefinition = ClassDefinition(name='RightClass', position=Position(522.0, 354.0), size=Size(height=107.0, width=167.0))
+        right: ClassDefinition = ClassDefinition(name='RightClass', position=Position(522, 354), size=Size(height=107, width=167))
         return right
 
     def _buildBendTest(self):
 
-        startPos: Position = Position(x=330.0, y=359.0)
-        cp1Pos:   Position = Position(x=330.0, y=286.0)
-        cp2Pos:   Position = Position(x=178.0, y=286.0)
-        cp3Pos:   Position = Position(x=178.0, y=207.0)
-        endPos:   Position = Position(x=409.0, y=207.0)
+        startPos: Position = Position(x=330, y=359)
+        cp1Pos:   Position = Position(x=330, y=286)
+        cp2Pos:   Position = Position(x=178, y=286)
+        cp3Pos:   Position = Position(x=178, y=207)
+        endPos:   Position = Position(x=409, y=207)
 
         bigBends: LinePositions = [startPos, cp1Pos, cp2Pos, cp3Pos, endPos]
 
         leftToTop: UmlLineDefinition = UmlLineDefinition(lineType=LineType.Inheritance, linePositions=bigBends)
 
-        startPosition2: Position = Position(x=604.0, y=354.0)
-        midPosition:    Position = Position(x=604.0, y=209.0)
-        endPosition2:   Position = Position(x=523.0, y=209.0)
+        startPosition2: Position = Position(x=604, y=354)
+        midPosition:    Position = Position(x=604, y=209)
+        endPosition2:   Position = Position(x=523, y=209)
 
         basicBends: LinePositions = [startPosition2, midPosition, endPosition2]
         rightToTop: UmlLineDefinition = UmlLineDefinition(lineType=LineType.Inheritance, linePositions=basicBends)
 
         bentLineDefinitions: UmlLineDefinitions = [leftToTop, rightToTop]
 
         return bentLineDefinitions
```

### Comparing `pyumldiagrams-2.30.8/tests/TestTemplate.py` & `pyumldiagrams-2.40.0/tests/TestTemplate.py`

 * *Files identical despite different names*

### Comparing `pyumldiagrams-2.30.8/tests/TestToClassDefinition.py` & `pyumldiagrams-2.40.0/tests/TestToClassDefinition.py`

 * *Files identical despite different names*

### Comparing `pyumldiagrams-2.30.8/tests/image/TestImageDiagram.py` & `pyumldiagrams-2.40.0/tests/image/TestImageDiagram.py`

 * *Files 0% similar despite different names*

```diff
@@ -371,44 +371,45 @@
 
         adjustedName: str = diagram._addSuffix(fileName=TestImageDiagram.DOTTED_EXPECTED_NAME, suffix=TestImageDiagram.EXPECTED_SUFFIX)
 
         self.assertEqual(TestImageDiagram.DOTTED_EXPECTED_NAME, adjustedName, 'Suffix incorrectly added for embedded periods')
 
     def testGetFullyQualifiedImagePath(self):
 
-        self.logger.warning(f'{TestDiagramParent.BASE_IMAGE_RESOURCE_PACKAGE_NAME}')
+        self.logger.debug(f'{TestDiagramParent.BASE_IMAGE_RESOURCE_PACKAGE_NAME}')
         actualName:   str = self._getFullyQualifiedImagePath('Test-Basic-Standard.png')
 
+        # noinspection SpellCheckingInspection
         partialPath: str = '/tests/resources/basefiles/image/'    # needs to match resource package name
         self.assertTrue(partialPath in actualName, 'Name does not match')
 
     def _assertIdenticalFiles(self, baseName: str, generatedFileName: str, failMessage: str, removeTestFile: bool = True) -> None:
         """
-        The side-affect here is that if the assertion passes then this method removes the generated file
+        The side effect here is that if the assertion passes then this method removes the generated file
 
         Args:
             baseName:           The base image file name
             generatedFileName:  The generated image file name
             failMessage:        The message to display if the image files fail comparison
         """
         standardFileName: str = self._getFullyQualifiedImagePath(f'{baseName}{TestDiagramParent.STANDARD_SUFFIX}.{ImageFormat.PNG.value}')
         status:           int = self._runDiff(baseFileName=generatedFileName, standardFileName=standardFileName)
-        self.assertTrue(status == 0, f'{failMessage}')
+        self.assertTrue(status == 0, failMessage)
 
         if removeTestFile is True:
             self.logger.info(f'Removing: {generatedFileName}')
             osRemove(generatedFileName)
 
 
 def suite() -> TestSuite:
     """You need to change the name of the test class here also."""
     import unittest
 
     testSuite: TestSuite = TestSuite()
-    # noinspection PyUnresolvedReferences
-    testSuite.addTest(unittest.makeSuite(TestImageDiagram))
+
+    testSuite.addTest(unittest.defaultTestLoader.loadTestsFromTestCase(testCaseClass=TestImageDiagram))
 
     return testSuite
 
 
 if __name__ == '__main__':
     unitTestMain()
```

### Comparing `pyumldiagrams-2.30.8/tests/image/TestImageLine.py` & `pyumldiagrams-2.40.0/tests/image/TestImageLine.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,15 +344,15 @@
 
 
 def suite() -> TestSuite:
     """You need to change the name of the test class here also."""
     import unittest
 
     testSuite: TestSuite = TestSuite()
-    # noinspection PyUnresolvedReferences
-    testSuite.addTest(unittest.makeSuite(TestImageLine))
+
+    testSuite.addTest(unittest.defaultTestLoader.loadTestsFromTestCase(testCaseClass=TestImageLine))
 
     return testSuite
 
 
 if __name__ == '__main__':
     unitTestMain()
```

### Comparing `pyumldiagrams-2.30.8/tests/pdf/TestPdfDiagram.py` & `pyumldiagrams-2.40.0/tests/pdf/TestPdfDiagram.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,16 +91,16 @@
         baseName: str = f'{TestConstants.TEST_FILE_NAME}-Basic'
         fileName: str = f'{baseName}{TestConstants.TEST_SUFFIX}'
 
         diagram:  PdfDiagram      = PdfDiagram(fileName=fileName, dpi=TestConstants.TEST_DPI)
         classDef: ClassDefinition = ClassDefinition(name=TestDiagramParent.BASE_TEST_CLASS_NAME,
                                                     size=Size(width=TestPdfDiagram.CELL_WIDTH, height=TestPdfDiagram.CELL_HEIGHT))
 
-        diagram.docTimeStamp = self.unitTestTimeStamp
         diagram.drawClass(classDef)
+        diagram.docTimeStamp = self.unitTestTimeStamp
         diagram.write()
 
         self._assertIdenticalFiles(baseName=baseName, generatedFileName=fileName, failMessage='Basic should be identical')
 
     def testBasicFields(self):
 
         baseName: str = f'{TestConstants.TEST_FILE_NAME}-BasicFields'
@@ -402,15 +402,15 @@
         diagram.docTimeStamp = self.unitTestTimeStamp
         diagram.write()
 
         self._assertIdenticalFiles(baseName=baseName, generatedFileName=fileName, failMessage='CaptureShowMethodsFalse should be identical')
 
     def testGetFullyQualifiedPdfPath(self):
 
-        self.logger.warning(f'{TestDiagramParent.BASE_PDF_RESOURCE_PACKAGE_NAME}')
+        self.logger.debug(f'{TestDiagramParent.BASE_PDF_RESOURCE_PACKAGE_NAME}')
 
         actualName:   str = self._getFullyQualifiedPdfPath('Test-Basic-Standard.pdf')
 
         # noinspection SpellCheckingInspection
         partialPath: str = '/tests/resources/basefiles/pdf/'    # needs to match resource package name
         self.assertTrue(partialPath in actualName, 'Name does not match')
 
@@ -446,24 +446,24 @@
 
         standardFileName: str = self._getFullyQualifiedPdfPath(f'{baseName}{TestDiagramParent.STANDARD_SUFFIX}{TestConstants.TEST_SUFFIX}')
         status:           int = self._runPdfDiff(baseFileName=generatedFileName, standardFileName=standardFileName)
 
         self.assertTrue(status == 0, failMessage)
 
         if removeTestFile is True:
-            self.logger.info(f'Removing: {generatedFileName}')
+            self.logger.debug(f'Removing: {generatedFileName}')
             osRemove(generatedFileName)
 
 
 def suite() -> TestSuite:
     """You need to change the name of the test class here also."""
     import unittest
 
     testSuite: TestSuite = TestSuite()
-    # noinspection PyUnresolvedReferences
-    testSuite.addTest(unittest.makeSuite(TestPdfDiagram))
+
+    testSuite.addTest(unittest.defaultTestLoader.loadTestsFromTestCase(testCaseClass=TestPdfDiagram))
 
     return testSuite
 
 
 if __name__ == '__main__':
     unitTestMain()
```

### Comparing `pyumldiagrams-2.30.8/tests/pdf/TestPdfLine.py` & `pyumldiagrams-2.40.0/tests/pdf/TestPdfLine.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from unittest import TestSuite
 from unittest import main as unitTestMain
 
 from pyumldiagrams.Defaults import LEFT_MARGIN
 from pyumldiagrams.Defaults import TOP_MARGIN
 from pyumldiagrams.Definitions import LinePositions
+from pyumldiagrams.pdf.FPDFExtended import FPDFExtended
 
 from pyumldiagrams.pdf.PdfCommon import PdfCommon
 
 from pyumldiagrams.Definitions import EllipseDefinition
 from pyumldiagrams.Definitions import UmlLineDefinition
 from pyumldiagrams.Definitions import UmlLineDefinitions
 from pyumldiagrams.Definitions import LineType
@@ -44,14 +45,18 @@
     H_LEFT_TOP_Y:     int = V_TOP_Y
     H_LEFT_BOTTOM_Y:  int = V_BOTTOM_Y
     H_RIGHT_BOTTOM_Y: int = H_LEFT_BOTTOM_Y
 
     Y_INC: int = 50
     DASH_LINE_SPACE_LENGTH: int = 4
 
+    DASH_LENGTH:   int = 1
+    BACK_TO_SOLID: int = 0
+    DASH_GAP:      int = 4
+
     ELLIPSE_X: int = V_LEFT_X
     ELLIPSE_Y: int = V_TOP_Y
 
     ELLIPSE_WIDTH:  int = 200
     ELLIPSE_HEIGHT: int = 200
 
     ELLIPSE_FILL_STYLE: str = 'D'
@@ -248,33 +253,56 @@
 
     def __drawHorizontalBoundaries(self, diagram: PdfDiagram):
 
         x1: int = PdfCommon.toPdfPoints(TestPdfLine.TOP_LINE_LEFT_X, diagram._dpi) + LEFT_MARGIN + diagram.verticalGap
         x2: int = PdfCommon.toPdfPoints(TestPdfLine.TOP_LINE_RIGHT_X, diagram._dpi) + LEFT_MARGIN + diagram.verticalGap
         y2: int = PdfCommon.toPdfPoints(TestPdfLine.V_BOTTOM_Y, diagram._dpi) + TOP_MARGIN + diagram.horizontalGap
 
-        diagram._pdf.dashed_line(x1=x1, y1=y2, x2=x2, y2=y2, space_length=TestPdfLine.DASH_LINE_SPACE_LENGTH)
+        pdf: FPDFExtended = diagram._pdf
+        # diagram._pdf.dashed_line(x1=x1, y1=y2, x2=x2, y2=y2, space_length=TestPdfLine.DASH_LINE_SPACE_LENGTH)
+
+        pdf.set_dash_pattern(dash=TestPdfLine.DASH_LENGTH, gap=TestPdfLine.DASH_LINE_SPACE_LENGTH, phase=0)
+        with pdf.new_path() as path:
+            path.move_to(x1, y2)
+            path.line_to(x2, y2)
 
         y2 = PdfCommon.toPdfPoints(TestPdfLine.V_TOP_Y, diagram._dpi) + TOP_MARGIN + diagram.horizontalGap
 
-        diagram._pdf.dashed_line(x1=x1, y1=y2, x2=x2, y2=y2, space_length=TestPdfLine.DASH_LINE_SPACE_LENGTH)
+        # diagram._pdf.dashed_line(x1=x1, y1=y2, x2=x2, y2=y2, space_length=TestPdfLine.DASH_GAP)
+        with pdf.new_path() as path:
+            path.move_to(x1, y2)
+            path.line_to(x2, y2)
+
+        pdf.set_dash_pattern(dash=TestPdfLine.BACK_TO_SOLID)
 
     def __drawVerticalBoundaries(self, diagram: PdfDiagram):
 
         x1: int = PdfCommon.toPdfPoints(TestPdfLine.H_LEFT_X, diagram._dpi) + LEFT_MARGIN + diagram.verticalGap
         x2: int = x1
         y1: int = PdfCommon.toPdfPoints(TestPdfLine.H_LEFT_TOP_Y, diagram._dpi) + TOP_MARGIN + diagram.horizontalGap
         y2: int = PdfCommon.toPdfPoints(TestPdfLine.H_LEFT_BOTTOM_Y, diagram._dpi) + TOP_MARGIN + diagram.horizontalGap
 
-        diagram._pdf.dashed_line(x1=x1, y1=y1, x2=x2, y2=y2, space_length=TestPdfLine.DASH_LINE_SPACE_LENGTH)
+        # diagram._pdf.dashed_line(x1=x1, y1=y1, x2=x2, y2=y2, space_length=TestPdfLine.DASH_LINE_SPACE_LENGTH)
+        pdf: FPDFExtended = diagram._pdf
+        pdf.set_dash_pattern(dash=TestPdfLine.DASH_LENGTH, gap=TestPdfLine.DASH_LINE_SPACE_LENGTH, phase=0)
+
+        with pdf.new_path() as path:
+            path.move_to(x1, y1)
+            path.line_to(x2, y2)
 
         x1 = PdfCommon.toPdfPoints(TestPdfLine.H_RIGHT_X, diagram._dpi) + LEFT_MARGIN + diagram.verticalGap
         x2 = x1
 
-        diagram._pdf.dashed_line(x1=x1, y1=y1, x2=x2, y2=y2, space_length=TestPdfLine.DASH_LINE_SPACE_LENGTH)
+        # diagram._pdf.dashed_line(x1=x1, y1=y1, x2=x2, y2=y2, space_length=TestPdfLine.DASH_LINE_SPACE_LENGTH)
+
+        with pdf.new_path() as path:
+            path.move_to(x1, y1)
+            path.line_to(x2, y2)
+
+        pdf.set_dash_pattern(dash=TestPdfLine.BACK_TO_SOLID)
 
     def __drawEllipseForDiagonalLines(self, diagram: PdfDiagram):
 
         eDef: EllipseDefinition = EllipseDefinition()
         pos:  Position          = Position(TestPdfLine.ELLIPSE_X, TestPdfLine.ELLIPSE_Y)
         size: Size              = Size(width=TestPdfLine.ELLIPSE_WIDTH, height=TestPdfLine.ELLIPSE_HEIGHT)
 
@@ -333,15 +361,15 @@
 
 
 def suite() -> TestSuite:
     """You need to change the name of the test class here also."""
     import unittest
 
     testSuite: TestSuite = TestSuite()
-    # noinspection PyUnresolvedReferences
-    testSuite.addTest(unittest.makeSuite(TestPdfLine))
+
+    testSuite.addTest(unittest.defaultTestLoader.loadTestsFromTestCase(testCaseClass=TestPdfLine))
 
     return testSuite
 
 
 if __name__ == '__main__':
     unitTestMain()
```

