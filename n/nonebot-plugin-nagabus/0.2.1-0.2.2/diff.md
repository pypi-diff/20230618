# Comparing `tmp/nonebot_plugin_nagabus-0.2.1.tar.gz` & `tmp/nonebot_plugin_nagabus-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nagabus-0.2.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_nagabus-0.2.2.tar", max compression
```

## Comparing `nonebot_plugin_nagabus-0.2.1.tar` & `nonebot_plugin_nagabus-0.2.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448000 nonebot_plugin_nagabus-0.2.1/LICENSE
--rw-r--r--   0        0        0     1237 2023-06-01 03:26:14.711563 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/__init__.py
--rw-r--r--   0        0        0      129 2023-05-27 04:29:09.849196 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/ac.py
--rw-r--r--   0        0        0     1197 2023-05-28 14:51:33.775850 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/config.py
--rw-r--r--   0        0        0        4 2023-05-26 13:11:24.775555 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/data/__init__.py
--rw-r--r--   0        0        0      116 2023-05-26 11:41:42.946553 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/data/base.py
--rw-r--r--   0        0        0      317 2023-05-26 11:41:42.956553 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/data/mjs.py
--rw-r--r--   0        0        0     1697 2023-06-09 05:28:00.065113 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/data/naga.py
--rw-r--r--   0        0        0      775 2023-05-26 11:41:42.960551 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/data/session.py
--rw-r--r--   0        0        0      713 2023-05-26 15:21:27.421204 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/data/utils/__init__.py
--rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843000 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/data/utils/utc_datetime.py
--rw-r--r--   0        0        0       43 2023-05-28 14:51:33.785849 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/errors.py
--rw-r--r--   0        0        0       95 2023-05-28 01:19:53.575323 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/matchers/__init__.py
--rw-r--r--   0        0        0      189 2023-05-30 02:32:55.940589 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/matchers/errors.py
--rw-r--r--   0        0        0        0 2023-05-30 02:22:08.333037 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/matchers/interceptors/__init__.py
--rw-r--r--   0        0        0     2872 2023-06-09 05:28:24.454277 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py
--rw-r--r--   0        0        0     4650 2023-06-09 06:01:06.071925 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/matchers/naga_analyze.py
--rw-r--r--   0        0        0     2420 2023-06-01 06:58:40.633672 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/matchers/naga_statistic.py
--rw-r--r--   0        0        0     2278 2023-05-27 02:48:33.707764 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/migrations/24aec3c56623_.py
--rw-r--r--   0        0        0     1617 2023-06-09 05:51:28.775960 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/migrations/70ff5fb4923e_.py
--rw-r--r--   0        0        0     1350 2023-05-27 07:17:07.623159 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py
--rw-r--r--   0        0        0     1009 2023-05-26 15:21:27.440185 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/mjs/__init__.py
--rw-r--r--   0        0        0      176 2023-05-25 15:39:25.419279 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/naga/__init__.py
--rw-r--r--   0        0        0     3709 2023-06-09 06:12:20.123461 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/naga/api.py
--rw-r--r--   0        0        0      436 2023-06-09 05:28:00.075631 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/naga/errors.py
--rw-r--r--   0        0        0     3415 2023-06-09 15:01:04.190237 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/naga/fake_api.py
--rw-r--r--   0        0        0     1248 2023-06-09 15:00:22.460735 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/naga/model.py
--rw-r--r--   0        0        0    21192 2023-06-09 14:41:10.459561 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/naga/service.py
--rw-r--r--   0        0        0      347 2023-06-09 05:53:37.650409 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/naga/utils.py
--rw-r--r--   0        0        0        0 2023-05-25 16:04:02.955709 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/utils/__init__.py
--rw-r--r--   0        0        0     1092 2023-05-25 16:06:56.701500 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/utils/integer.py
--rw-r--r--   0        0        0        0 2023-05-26 12:48:40.974521 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/utils/mapping.py
--rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247000 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/utils/nonebot.py
--rw-r--r--   0        0        0       68 2023-05-26 15:50:47.559077 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/utils/tz.py
--rw-r--r--   0        0        0      997 2023-06-09 06:08:29.587244 nonebot_plugin_nagabus-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1789 2023-05-28 03:26:24.309853 nonebot_plugin_nagabus-0.2.1/README.md
--rw-r--r--   0        0        0     2706 1970-01-01 00:00:00.000000 nonebot_plugin_nagabus-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448000 nonebot_plugin_nagabus-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1505 2023-06-18 15:16:39.550248 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/__init__.py
+-rw-r--r--   0        0        0      129 2023-05-27 04:29:09.849196 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/ac.py
+-rw-r--r--   0        0        0     1197 2023-05-28 14:51:33.775850 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/config.py
+-rw-r--r--   0        0        0        4 2023-05-26 13:11:24.775555 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/data/__init__.py
+-rw-r--r--   0        0        0      116 2023-05-26 11:41:42.946553 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/data/base.py
+-rw-r--r--   0        0        0      317 2023-05-26 11:41:42.956553 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/data/mjs.py
+-rw-r--r--   0        0        0     1697 2023-06-09 05:28:00.065113 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/data/naga.py
+-rw-r--r--   0        0        0      775 2023-05-26 11:41:42.960551 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/data/session.py
+-rw-r--r--   0        0        0      713 2023-05-26 15:21:27.421204 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/data/utils/__init__.py
+-rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843000 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/data/utils/utc_datetime.py
+-rw-r--r--   0        0        0       43 2023-05-28 14:51:33.785849 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/errors.py
+-rw-r--r--   0        0        0       95 2023-05-28 01:19:53.575323 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/matchers/__init__.py
+-rw-r--r--   0        0        0      189 2023-05-30 02:32:55.940589 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/matchers/errors.py
+-rw-r--r--   0        0        0        0 2023-05-30 02:22:08.333037 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/matchers/interceptors/__init__.py
+-rw-r--r--   0        0        0     2872 2023-06-09 05:28:24.454277 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py
+-rw-r--r--   0        0        0     4650 2023-06-09 06:01:06.071925 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/matchers/naga_analyze.py
+-rw-r--r--   0        0        0     2420 2023-06-01 06:58:40.633672 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/matchers/naga_statistic.py
+-rw-r--r--   0        0        0     2278 2023-05-27 02:48:33.707764 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/migrations/24aec3c56623_.py
+-rw-r--r--   0        0        0     1617 2023-06-09 05:51:28.775960 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/migrations/70ff5fb4923e_.py
+-rw-r--r--   0        0        0     1350 2023-05-27 07:17:07.623159 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py
+-rw-r--r--   0        0        0     1009 2023-05-26 15:21:27.440185 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/mjs/__init__.py
+-rw-r--r--   0        0        0      176 2023-05-25 15:39:25.419279 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/naga/__init__.py
+-rw-r--r--   0        0        0     3709 2023-06-09 06:12:20.123461 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/naga/api.py
+-rw-r--r--   0        0        0      436 2023-06-09 05:28:00.075631 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/naga/errors.py
+-rw-r--r--   0        0        0     3415 2023-06-09 15:01:04.190237 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/naga/fake_api.py
+-rw-r--r--   0        0        0     1248 2023-06-09 15:00:22.460735 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/naga/model.py
+-rw-r--r--   0        0        0    21192 2023-06-09 14:41:10.459561 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/naga/service.py
+-rw-r--r--   0        0        0      347 2023-06-09 05:53:37.650409 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/naga/utils.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:04:02.955709 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/utils/__init__.py
+-rw-r--r--   0        0        0     1092 2023-05-25 16:06:56.701500 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/utils/integer.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:48:40.974521 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/utils/mapping.py
+-rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247000 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/utils/nonebot.py
+-rw-r--r--   0        0        0       68 2023-05-26 15:50:47.559077 nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/utils/tz.py
+-rw-r--r--   0        0        0      997 2023-06-18 15:16:39.541668 nonebot_plugin_nagabus-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1789 2023-05-28 03:26:24.309853 nonebot_plugin_nagabus-0.2.2/README.md
+-rw-r--r--   0        0        0     2706 1970-01-01 00:00:00.000000 nonebot_plugin_nagabus-0.2.2/PKG-INFO
```

### Comparing `nonebot_plugin_nagabus-0.2.1/LICENSE` & `nonebot_plugin_nagabus-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/config.py` & `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/data/naga.py` & `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/data/naga.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/data/session.py` & `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/data/session.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/data/utils/__init__.py` & `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/data/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/data/utils/utc_datetime.py` & `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/data/utils/utc_datetime.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py` & `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/matchers/naga_analyze.py` & `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/matchers/naga_analyze.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/matchers/naga_statistic.py` & `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/matchers/naga_statistic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/migrations/24aec3c56623_.py` & `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/migrations/24aec3c56623_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/migrations/70ff5fb4923e_.py` & `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/migrations/70ff5fb4923e_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py` & `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/mjs/__init__.py` & `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/mjs/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/naga/api.py` & `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/naga/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/naga/fake_api.py` & `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/naga/fake_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/naga/model.py` & `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/naga/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/naga/service.py` & `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/naga/service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/utils/integer.py` & `nonebot_plugin_nagabus-0.2.2/nonebot_plugin_nagabus/utils/integer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.1/pyproject.toml` & `nonebot_plugin_nagabus-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-nagabus"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_nagabus" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `nonebot_plugin_nagabus-0.2.1/README.md` & `nonebot_plugin_nagabus-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.1/PKG-INFO` & `nonebot_plugin_nagabus-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nagabus
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

