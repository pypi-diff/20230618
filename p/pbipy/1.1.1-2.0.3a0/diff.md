# Comparing `tmp/pbipy-1.1.1.tar.gz` & `tmp/pbipy-2.0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbipy-1.1.1.tar", last modified: Wed May 31 03:48:56 2023, max compression
+gzip compressed data, was "pbipy-2.0.3a0.tar", last modified: Sun Jun 18 05:31:15 2023, max compression
```

## Comparing `pbipy-1.1.1.tar` & `pbipy-2.0.3a0.tar`

### file list

```diff
@@ -1,24 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 03:48:56.360582 pbipy-1.1.1/
--rw-rw-rw-   0        0        0    11523 2022-10-28 08:16:15.000000 pbipy-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     6480 2023-05-31 03:48:56.359580 pbipy-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5717 2022-12-05 03:27:44.000000 pbipy-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 03:48:56.340579 pbipy-1.1.1/pbipy/
--rw-rw-rw-   0        0        0       29 2022-10-28 07:52:32.000000 pbipy-1.1.1/pbipy/__init__.py
--rw-rw-rw-   0        0        0      314 2023-05-31 02:18:20.000000 pbipy-1.1.1/pbipy/__version__.py
--rw-rw-rw-   0        0        0     7769 2023-05-30 19:56:55.000000 pbipy-1.1.1/pbipy/models.py
-drwxrwxrwx   0        0        0        0 2023-05-31 03:48:56.358580 pbipy-1.1.1/pbipy/operationgroups/
--rw-rw-rw-   0        0        0      110 2023-05-29 23:59:34.000000 pbipy-1.1.1/pbipy/operationgroups/__init__.py
--rw-rw-rw-   0        0        0     3468 2022-12-05 03:27:44.000000 pbipy-1.1.1/pbipy/operationgroups/admin.py
--rw-rw-rw-   0        0        0     5126 2023-05-31 01:18:53.000000 pbipy-1.1.1/pbipy/operationgroups/apps.py
--rw-rw-rw-   0        0        0     8788 2023-05-29 23:59:34.000000 pbipy-1.1.1/pbipy/operationgroups/datasets.py
--rw-rw-rw-   0        0        0     1249 2023-05-29 23:59:34.000000 pbipy-1.1.1/pbipy/operationgroups/groups.py
--rw-rw-rw-   0        0        0     4996 2023-05-29 23:59:34.000000 pbipy-1.1.1/pbipy/powerbi.py
--rw-rw-rw-   0        0        0     1059 2022-10-31 06:57:03.000000 pbipy-1.1.1/pbipy/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-31 03:48:56.347582 pbipy-1.1.1/pbipy.egg-info/
--rw-rw-rw-   0        0        0     6480 2023-05-31 03:48:56.000000 pbipy-1.1.1/pbipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      418 2023-05-31 03:48:56.000000 pbipy-1.1.1/pbipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 03:48:56.000000 pbipy-1.1.1/pbipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-31 03:48:56.000000 pbipy-1.1.1/pbipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-31 03:48:56.000000 pbipy-1.1.1/pbipy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 03:48:56.360582 pbipy-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     3594 2022-12-05 03:27:44.000000 pbipy-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 05:31:15.364409 pbipy-2.0.3a0/
+-rw-rw-rw-   0        0        0    11523 2022-10-28 08:16:15.000000 pbipy-2.0.3a0/LICENSE
+-rw-rw-rw-   0        0        0     8991 2023-06-18 05:31:15.363410 pbipy-2.0.3a0/PKG-INFO
+-rw-rw-rw-   0        0        0     8205 2023-06-18 05:21:13.000000 pbipy-2.0.3a0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 05:31:15.355410 pbipy-2.0.3a0/pbipy/
+-rw-rw-rw-   0        0        0       29 2022-10-28 07:52:32.000000 pbipy-2.0.3a0/pbipy/__init__.py
+-rw-rw-rw-   0        0        0      341 2023-06-18 05:25:30.000000 pbipy-2.0.3a0/pbipy/__version__.py
+-rw-rw-rw-   0        0        0     4240 2023-06-18 05:21:13.000000 pbipy-2.0.3a0/pbipy/powerbi.py
+-rw-rw-rw-   0        0        0    20774 2023-06-18 05:21:13.000000 pbipy-2.0.3a0/pbipy/resources.py
+-rw-rw-rw-   0        0        0      110 2023-06-18 05:21:13.000000 pbipy-2.0.3a0/pbipy/settings.py
+-rw-rw-rw-   0        0        0    10220 2023-06-18 05:21:13.000000 pbipy-2.0.3a0/pbipy/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-18 05:31:15.362409 pbipy-2.0.3a0/pbipy.egg-info/
+-rw-rw-rw-   0        0        0     8991 2023-06-18 05:31:15.000000 pbipy-2.0.3a0/pbipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-06-18 05:31:15.000000 pbipy-2.0.3a0/pbipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 05:31:15.000000 pbipy-2.0.3a0/pbipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-18 05:31:15.000000 pbipy-2.0.3a0/pbipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-18 05:31:15.000000 pbipy-2.0.3a0/pbipy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 05:31:15.364409 pbipy-2.0.3a0/setup.cfg
+-rw-rw-rw-   0        0        0     3594 2022-12-05 03:27:44.000000 pbipy-2.0.3a0/setup.py
```

### Comparing `pbipy-1.1.1/LICENSE` & `pbipy-2.0.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pbipy-1.1.1/setup.py` & `pbipy-2.0.3a0/setup.py`

 * *Files identical despite different names*

