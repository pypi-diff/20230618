# Comparing `tmp/bank_scrapers-1.0.2.tar.gz` & `tmp/bank_scrapers-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bank_scrapers-1.0.2.tar", last modified: Sun Jun 18 09:11:13 2023, max compression
+gzip compressed data, was "bank_scrapers-1.0.3.tar", last modified: Sun Jun 18 14:12:22 2023, max compression
```

## Comparing `bank_scrapers-1.0.2.tar` & `bank_scrapers-1.0.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 09:11:13.911367 bank_scrapers-1.0.2/
--rw-rw-r--   0 eric      (1000) eric      (1000)     1066 2023-06-18 06:33:32.000000 bank_scrapers-1.0.2/LICENSE
--rw-rw-r--   0 eric      (1000) eric      (1000)    19810 2023-06-18 09:11:13.911367 bank_scrapers-1.0.2/PKG-INFO
--rw-rw-r--   0 eric      (1000) eric      (1000)    18278 2023-06-18 08:57:03.000000 bank_scrapers-1.0.2/README.md
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 09:11:13.911367 bank_scrapers-1.0.2/bank_scrapers/
--rw-rw-r--   0 eric      (1000) eric      (1000)      476 2023-06-18 08:57:28.000000 bank_scrapers-1.0.2/bank_scrapers/__init__.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 09:11:13.911367 bank_scrapers-1.0.2/bank_scrapers/api_wrappers/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-12 11:03:00.000000 bank_scrapers-1.0.2/bank_scrapers/api_wrappers/__init__.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 09:11:13.911367 bank_scrapers-1.0.2/bank_scrapers/api_wrappers/kraken/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-12 11:03:11.000000 bank_scrapers-1.0.2/bank_scrapers/api_wrappers/kraken/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     2863 2023-06-17 11:54:24.000000 bank_scrapers-1.0.2/bank_scrapers/api_wrappers/kraken/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 09:11:13.911367 bank_scrapers-1.0.2/bank_scrapers/cli/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-18 04:02:26.000000 bank_scrapers-1.0.2/bank_scrapers/cli/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     9027 2023-06-18 08:52:15.000000 bank_scrapers-1.0.2/bank_scrapers/cli/cli.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 09:11:13.911367 bank_scrapers-1.0.2/bank_scrapers/common/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-18 04:04:49.000000 bank_scrapers-1.0.2/bank_scrapers/common/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)      272 2023-06-18 04:49:40.000000 bank_scrapers-1.0.2/bank_scrapers/common/log.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 09:11:13.911367 bank_scrapers-1.0.2/bank_scrapers/scrapers/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:17:21.000000 bank_scrapers-1.0.2/bank_scrapers/scrapers/__init__.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 09:11:13.911367 bank_scrapers-1.0.2/bank_scrapers/scrapers/becu/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.2/bank_scrapers/scrapers/becu/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     4284 2023-06-18 08:44:27.000000 bank_scrapers-1.0.2/bank_scrapers/scrapers/becu/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 09:11:13.911367 bank_scrapers-1.0.2/bank_scrapers/scrapers/chase/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.2/bank_scrapers/scrapers/chase/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     9219 2023-06-18 08:44:27.000000 bank_scrapers-1.0.2/bank_scrapers/scrapers/chase/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 09:11:13.911367 bank_scrapers-1.0.2/bank_scrapers/scrapers/common/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:48:23.000000 bank_scrapers-1.0.2/bank_scrapers/scrapers/common/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     4039 2023-06-18 08:44:27.000000 bank_scrapers-1.0.2/bank_scrapers/scrapers/common/functions.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 09:11:13.911367 bank_scrapers-1.0.2/bank_scrapers/scrapers/fidelity_netbenefits/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.2/bank_scrapers/scrapers/fidelity_netbenefits/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     8402 2023-06-18 09:04:24.000000 bank_scrapers-1.0.2/bank_scrapers/scrapers/fidelity_netbenefits/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 09:11:13.911367 bank_scrapers-1.0.2/bank_scrapers/scrapers/roundpoint/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.2/bank_scrapers/scrapers/roundpoint/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     8692 2023-06-18 08:44:27.000000 bank_scrapers-1.0.2/bank_scrapers/scrapers/roundpoint/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 09:11:13.911367 bank_scrapers-1.0.2/bank_scrapers/scrapers/smbc_prestia/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.2/bank_scrapers/scrapers/smbc_prestia/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     4627 2023-06-18 08:44:27.000000 bank_scrapers-1.0.2/bank_scrapers/scrapers/smbc_prestia/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 09:11:13.911367 bank_scrapers-1.0.2/bank_scrapers/scrapers/uhfcu/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.2/bank_scrapers/scrapers/uhfcu/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     8700 2023-06-18 08:44:27.000000 bank_scrapers-1.0.2/bank_scrapers/scrapers/uhfcu/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 09:11:13.911367 bank_scrapers-1.0.2/bank_scrapers/scrapers/vanguard/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.2/bank_scrapers/scrapers/vanguard/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     7781 2023-06-18 08:44:27.000000 bank_scrapers-1.0.2/bank_scrapers/scrapers/vanguard/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 09:11:13.911367 bank_scrapers-1.0.2/bank_scrapers/scrapers/zillow/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.2/bank_scrapers/scrapers/zillow/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     3457 2023-06-18 08:44:27.000000 bank_scrapers-1.0.2/bank_scrapers/scrapers/zillow/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 09:11:13.911367 bank_scrapers-1.0.2/bank_scrapers.egg-info/
--rw-rw-r--   0 eric      (1000) eric      (1000)    19810 2023-06-18 09:11:13.000000 bank_scrapers-1.0.2/bank_scrapers.egg-info/PKG-INFO
--rw-rw-r--   0 eric      (1000) eric      (1000)     1347 2023-06-18 09:11:13.000000 bank_scrapers-1.0.2/bank_scrapers.egg-info/SOURCES.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)        1 2023-06-18 09:11:13.000000 bank_scrapers-1.0.2/bank_scrapers.egg-info/dependency_links.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)       59 2023-06-18 09:11:13.000000 bank_scrapers-1.0.2/bank_scrapers.egg-info/entry_points.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)      118 2023-06-18 09:11:13.000000 bank_scrapers-1.0.2/bank_scrapers.egg-info/requires.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)       14 2023-06-18 09:11:13.000000 bank_scrapers-1.0.2/bank_scrapers.egg-info/top_level.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)      945 2023-06-18 08:57:28.000000 bank_scrapers-1.0.2/pyproject.toml
--rw-rw-r--   0 eric      (1000) eric      (1000)       38 2023-06-18 09:11:13.911367 bank_scrapers-1.0.2/setup.cfg
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1066 2023-06-18 06:33:32.000000 bank_scrapers-1.0.3/LICENSE
+-rw-rw-r--   0 eric      (1000) eric      (1000)    19810 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)    18278 2023-06-18 08:57:03.000000 bank_scrapers-1.0.3/README.md
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.631040 bank_scrapers-1.0.3/bank_scrapers/
+-rw-rw-r--   0 eric      (1000) eric      (1000)      476 2023-06-18 14:11:13.000000 bank_scrapers-1.0.3/bank_scrapers/__init__.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.631040 bank_scrapers-1.0.3/bank_scrapers/api_wrappers/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-12 11:03:00.000000 bank_scrapers-1.0.3/bank_scrapers/api_wrappers/__init__.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.631040 bank_scrapers-1.0.3/bank_scrapers/api_wrappers/kraken/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-12 11:03:11.000000 bank_scrapers-1.0.3/bank_scrapers/api_wrappers/kraken/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2863 2023-06-17 11:54:24.000000 bank_scrapers-1.0.3/bank_scrapers/api_wrappers/kraken/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/bank_scrapers/cli/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-18 04:02:26.000000 bank_scrapers-1.0.3/bank_scrapers/cli/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     9027 2023-06-18 08:52:15.000000 bank_scrapers-1.0.3/bank_scrapers/cli/cli.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/bank_scrapers/common/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-18 04:04:49.000000 bank_scrapers-1.0.3/bank_scrapers/common/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)      272 2023-06-18 04:49:40.000000 bank_scrapers-1.0.3/bank_scrapers/common/log.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/bank_scrapers/scrapers/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:17:21.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/__init__.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/bank_scrapers/scrapers/becu/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/becu/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     4284 2023-06-18 08:44:27.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/becu/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/bank_scrapers/scrapers/chase/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/chase/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     9153 2023-06-18 14:10:29.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/chase/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/bank_scrapers/scrapers/common/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:48:23.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/common/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     4541 2023-06-18 14:09:43.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/common/functions.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/bank_scrapers/scrapers/fidelity_netbenefits/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/fidelity_netbenefits/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     8335 2023-06-18 14:10:29.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/fidelity_netbenefits/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/bank_scrapers/scrapers/roundpoint/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/roundpoint/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     8626 2023-06-18 14:10:29.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/roundpoint/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/bank_scrapers/scrapers/smbc_prestia/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/smbc_prestia/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     4627 2023-06-18 08:44:27.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/smbc_prestia/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/bank_scrapers/scrapers/uhfcu/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/uhfcu/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     8643 2023-06-18 14:10:29.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/uhfcu/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/bank_scrapers/scrapers/vanguard/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/vanguard/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     7716 2023-06-18 14:10:29.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/vanguard/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/bank_scrapers/scrapers/zillow/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/zillow/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     3457 2023-06-18 08:44:27.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/zillow/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.631040 bank_scrapers-1.0.3/bank_scrapers.egg-info/
+-rw-rw-r--   0 eric      (1000) eric      (1000)    19810 2023-06-18 14:12:22.000000 bank_scrapers-1.0.3/bank_scrapers.egg-info/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1347 2023-06-18 14:12:22.000000 bank_scrapers-1.0.3/bank_scrapers.egg-info/SOURCES.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)        1 2023-06-18 14:12:22.000000 bank_scrapers-1.0.3/bank_scrapers.egg-info/dependency_links.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)       59 2023-06-18 14:12:22.000000 bank_scrapers-1.0.3/bank_scrapers.egg-info/entry_points.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)      118 2023-06-18 14:12:22.000000 bank_scrapers-1.0.3/bank_scrapers.egg-info/requires.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)       14 2023-06-18 14:12:22.000000 bank_scrapers-1.0.3/bank_scrapers.egg-info/top_level.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)      945 2023-06-18 14:11:13.000000 bank_scrapers-1.0.3/pyproject.toml
+-rw-rw-r--   0 eric      (1000) eric      (1000)       38 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/setup.cfg
```

### Comparing `bank_scrapers-1.0.2/LICENSE` & `bank_scrapers-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.2/PKG-INFO` & `bank_scrapers-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bank_scrapers
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library for working with bank_scrapers drivers.
 Author: Eric Bette
 License: MIT License
         
         Copyright (c) 2023 Eric Bette
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bank_scrapers-1.0.2/README.md` & `bank_scrapers-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.2/bank_scrapers/api_wrappers/kraken/driver.py` & `bank_scrapers-1.0.3/bank_scrapers/api_wrappers/kraken/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.2/bank_scrapers/cli/cli.py` & `bank_scrapers-1.0.3/bank_scrapers/cli/cli.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.2/bank_scrapers/scrapers/becu/driver.py` & `bank_scrapers-1.0.3/bank_scrapers/scrapers/becu/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.2/bank_scrapers/scrapers/chase/driver.py` & `bank_scrapers-1.0.3/bank_scrapers/scrapers/chase/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 tables = get_accounts_info(username="{username}", password="{password}")
 for t in tables:
     print(t.to_string())
 ```
 """
 
 # Standard Library Imports
-import sys
 from typing import Dict
 
 # Non-Standard Imports
 import pandas as pd
 from selenium.common.exceptions import TimeoutException
 from selenium.webdriver.common.by import By
 
@@ -252,17 +251,15 @@
         wait.until(
             lambda driver: "chase.com/web/auth/dashboard#/dashboard/overviewAccounts/overview/singleCard"
             in driver.current_url
             or is_2fa_redirect()
             or password_needs_reset()
         )
     except TimeoutException as e:
-        print(driver.current_url)
-        print(driver.page_source)
-        sys.exit(1)
+        leave_on_timeout(driver)
 
     # Handle 2FA if prompted, or quit if Chase catches us
     if is_2fa_redirect():
         handle_multi_factor_authentication(driver, wait, password)
     elif password_needs_reset():
         print("Password needs reset!")
         sys.exit(1)
```

### Comparing `bank_scrapers-1.0.2/bank_scrapers/scrapers/common/functions.py` & `bank_scrapers-1.0.3/bank_scrapers/scrapers/common/functions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Handy functions to be used by any driver
 """
 from __future__ import annotations
 
+import sys
 import os
 import shutil
+from datetime import datetime
 from pathlib import Path
 
 # Standard Imports
 from typing import Tuple, List
 
 # Non-standard Imports
 from selenium.common import NoSuchElementException
@@ -26,24 +28,29 @@
     Inspired by https://github.com/ultrafunkamsterdam/undetected-chromedriver/issues/727#issuecomment-1216199477
     A workaround for getting this to run on arm64. Use the locally installed chromedriver as a base if it's there
     :param options: An Options object to use for the driver
     :return: An undetectable chrome instance
     """
     # Check if there's an existing chromedriver
     if os.path.exists("/usr/bin/chromedriver"):
+
+        filepath = os.path.join(f"{Path.home()}/.local/share/undetected_chromedriver", "chromedriver_copy")
+        if not os.path.exists(f"{Path.home()}/.local/share/undetected_chromedriver"):
+            os.makedirs(f"{Path.home()}/.local/share/undetected_chromedriver")
+
         # If there is, copy it to the undetected chrome installation path
         shutil.copy(
             "/usr/bin/chromedriver",
-            f"{Path.home()}/.local/share/undetected_chromedriver/chromedriver_copy",
+            filepath,
         )
 
         # Instantiating the Driver with the chromedriver copy
         driver: Chrome = Chrome(
             options=options,
-            driver_executable_path=f"{Path.home()}/.local/share/undetected_chromedriver/chromedriver_copy",
+            driver_executable_path=filepath,
         )
     else:
         # Otherwise start as normal
         driver: Chrome = Chrome(options=options)
 
     return driver
 
@@ -106,7 +113,18 @@
     :return: The web element object
     """
     try:
         driver.find_element(*identifier)
     except NoSuchElementException:
         return False
     return True
+
+
+def leave_on_timeout(driver):
+    print(driver.current_url)
+    driver.save_screenshot(
+        f"{Path.home()}/{datetime.today().strftime('%Y%M%d%H%m%s')}.png"
+    )
+    print(
+        f"Screenshot saved to {Path.home()}/bank_scrapers_err_{datetime.today().strftime('%Y%M%d%H%m%s')}.png"
+    )
+    sys.exit(1)
```

### Comparing `bank_scrapers-1.0.2/bank_scrapers/scrapers/fidelity_netbenefits/driver.py` & `bank_scrapers-1.0.3/bank_scrapers/scrapers/fidelity_netbenefits/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 import shutil
 shutil.rmtree(tmp_dir)
 ```
 """
 
 # Standard Library Imports
-import sys
 from time import sleep
 
 # Non-Standard Imports
 import pandas as pd
 from selenium.common.exceptions import TimeoutException
 from selenium.webdriver import Chrome
 from selenium.webdriver.common.by import By
@@ -180,15 +179,15 @@
         )
     )
 
     # Click the button
     download_btn.click()
 
     # Sleep time to make sure the download completes
-    sleep(20)
+    sleep(3)
 
 
 def parse_accounts_summary(full_path: str) -> pd.DataFrame:
     """
     Post-processing of the downloaded file removing disclaimers and other irrelevant mumbo jumbo
     :param full_path: The path to the file to parse
     :return: A pandas dataframe of the downloaded data
@@ -221,17 +220,15 @@
     try:
         wait.until(
             lambda driver: "https://workplaceservices.fidelity.com/"
             in driver.current_url
             or str("Extra security step required") in driver.page_source
         )
     except TimeoutException as e:
-        print(driver.current_url)
-        print(driver.page_source)
-        sys.exit(1)
+        leave_on_timeout(driver)
 
     # If 2FA...
     def is_2fa_redirect():
         if (
             "https://login.fidelity.com/" in driver.current_url
             and str("Extra security step required") in driver.page_source
         ):
```

### Comparing `bank_scrapers-1.0.2/bank_scrapers/scrapers/roundpoint/driver.py` & `bank_scrapers-1.0.3/bank_scrapers/scrapers/roundpoint/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 tables = get_accounts_info(username="{username}", password="{password}")
 for t in tables:
     print(t.to_string())
 ```
 """
 
 # Standard Library Imports
-import sys
 from time import sleep
 from typing import Dict
 
 # Non-Standard Imports
 import pandas as pd
 from selenium.common.exceptions import TimeoutException
 from selenium.webdriver.common.by import By
@@ -234,17 +233,15 @@
     try:
         wait.until(
             lambda driver: "https://loansphereservicingdigital.bkiconnect.com/servicinghome/#/dashboard"
             in driver.current_url
             or is_2fa_redirect()
         )
     except TimeoutException as e:
-        print(driver.current_url)
-        print(driver.page_source)
-        sys.exit(1)
+        leave_on_timeout(driver)
 
     # Handle 2FA if prompted, or quit if Chase catches us
     if is_2fa_redirect():
         handle_multi_factor_authentication(driver, wait)
 
     # Wait for landing page after handling 2FA
     wait.until(
```

### Comparing `bank_scrapers-1.0.2/bank_scrapers/scrapers/smbc_prestia/driver.py` & `bank_scrapers-1.0.3/bank_scrapers/scrapers/smbc_prestia/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.2/bank_scrapers/scrapers/uhfcu/driver.py` & `bank_scrapers-1.0.3/bank_scrapers/scrapers/uhfcu/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 tables = get_accounts_info(username="{username}", password="{password}")
 for t in tables:
     print(t.to_string())
 ```
 """
 
 # Standard Library Imports
-import sys
 from time import sleep
 from typing import Dict
 
 # Non-Standard Imports
 import pandas as pd
 from selenium.common.exceptions import TimeoutException
 from selenium.webdriver.common.by import By
@@ -22,15 +21,15 @@
 # Local Imports
 from bank_scrapers.scrapers.common.functions import *
 
 # Logon page
 HOMEPAGE: str = "https://online.uhfcu.com/sign-in?user=&SubmitNext=Sign%20On"
 
 # Timeout
-TIMEOUT: int = 60
+TIMEOUT: int = 5
 
 # Chrome config
 CHROME_OPTIONS: List[str] = [
     "--no-sandbox",
     "--window-size=1920,1080",
     "--headless",
     "--disable-gpu",
@@ -187,16 +186,16 @@
     # Get a list of the card text
     account_info: List[str] = table.text.split(sep="\n")
 
     # Remove the first element (Share Account title)
     account_info.pop(0)
 
     # Data
-    account_type = account_info.pop(0)
-    account_desc = account_info.pop(0)
+    account_type: str = account_info.pop(0)
+    account_desc: str = account_info.pop(0)
 
     # The remaining elements are alternating kv pairs as list elements, so split and zip
     balance_infos: zip = zip(
         list(e for i, e in enumerate(account_info) if i % 2 == 0),
         list(e for i, e in enumerate(account_info) if i % 2 != 0),
     )
 
@@ -238,17 +237,15 @@
     try:
         wait.until(
             lambda driver: "https://online.uhfcu.com/consumer/main/dashboard"
             in driver.current_url
             or is_2fa_redirect()
         )
     except TimeoutException as e:
-        print(driver.current_url)
-        print(driver.page_source)
-        sys.exit(1)
+        leave_on_timeout(driver)
 
     # Handle 2FA if prompted, or quit if Chase catches us
     if is_2fa_redirect():
         handle_multi_factor_authentication(driver, wait)
 
     # Wait for landing page after handling 2FA
     wait.until(
```

### Comparing `bank_scrapers-1.0.2/bank_scrapers/scrapers/vanguard/driver.py` & `bank_scrapers-1.0.3/bank_scrapers/scrapers/vanguard/driver.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 import shutil
 shutil.rmtree(tmp_dir)
 ```
 """
 
 # Standard Library Imports
-import sys
+
 # Non-Standard Imports
 from time import sleep
 
 import pandas as pd
 from selenium.common.exceptions import TimeoutException
 from selenium.webdriver.common.by import By
 
@@ -215,17 +215,15 @@
     try:
         wait.until(
             lambda driver: "https://dashboard.web.vanguard.com/" in driver.current_url
             or "https://challenges.web.vanguard.com/" in driver.current_url
             or is_2fa_redirect()
         )
     except TimeoutException as e:
-        print(driver.current_url)
-        print(driver.page_source)
-        sys.exit(1)
+        leave_on_timeout(driver)
 
     # Handle 2FA if prompted, or quit if Chase catches us
     if is_2fa_redirect():
         handle_multi_factor_authentication(driver, wait)
 
     # Wait for landing page after handling 2FA
     wait.until(
```

### Comparing `bank_scrapers-1.0.2/bank_scrapers/scrapers/zillow/driver.py` & `bank_scrapers-1.0.3/bank_scrapers/scrapers/zillow/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.2/bank_scrapers.egg-info/PKG-INFO` & `bank_scrapers-1.0.3/bank_scrapers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bank-scrapers
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library for working with bank_scrapers drivers.
 Author: Eric Bette
 License: MIT License
         
         Copyright (c) 2023 Eric Bette
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bank_scrapers-1.0.2/bank_scrapers.egg-info/SOURCES.txt` & `bank_scrapers-1.0.3/bank_scrapers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.2/pyproject.toml` & `bank_scrapers-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 dependencies = [
     "beautifulsoup4>=4.12.2",
     "pandas>=2.0.2",
     "requests>=2.31.0",
     "undetected-chromedriver>=3.5.0",
     "lxml>=4.9.2",
-    "bank_scrapers==1.0.2",
+    "bank_scrapers==1.0.3",
 ]
 
 [project.urls]
 homepage = "https://github.com/eebette/bank_scrapers/tree/master"
 
 [project.scripts]
 bank-scrape = "bank_scrapers.cli.cli:main"
```

