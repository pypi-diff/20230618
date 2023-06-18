# Comparing `tmp/pydis_core-9.8.0.tar.gz` & `tmp/pydis_core-9.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydis_core-9.8.0.tar", max compression
+gzip compressed data, was "pydis_core-9.9.0.tar", max compression
```

## Comparing `pydis_core-9.8.0.tar` & `pydis_core-9.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1071 2022-03-31 15:49:16.729733 pydis_core-9.8.0/LICENSE
--rw-r--r--   0        0        0      320 2023-06-10 18:44:50.836639 pydis_core-9.8.0/pydis_core/__init__.py
--rw-r--r--   0        0        0    11394 2023-06-10 18:44:50.836639 pydis_core-9.8.0/pydis_core/_bot.py
--rw-r--r--   0        0        0     1886 2023-06-10 18:44:50.837639 pydis_core-9.8.0/pydis_core/async_stats.py
--rw-r--r--   0        0        0       93 2023-06-10 18:44:50.837639 pydis_core-9.8.0/pydis_core/exts/__init__.py
--rw-r--r--   0        0        0     6309 2023-06-10 18:44:50.837639 pydis_core-9.8.0/pydis_core/site_api.py
--rw-r--r--   0        0        0     1336 2023-06-10 18:49:04.940072 pydis_core-9.8.0/pydis_core/utils/__init__.py
--rw-r--r--   0        0        0     1680 2022-11-05 14:18:24.788185 pydis_core-9.8.0/pydis_core/utils/_extensions.py
--rw-r--r--   0        0        0     2749 2023-06-10 18:44:50.838639 pydis_core-9.8.0/pydis_core/utils/_monkey_patches.py
--rw-r--r--   0        0        0     1810 2022-11-05 14:18:24.789186 pydis_core-9.8.0/pydis_core/utils/caching.py
--rw-r--r--   0        0        0     1705 2023-06-04 20:04:18.921646 pydis_core-9.8.0/pydis_core/utils/channel.py
--rw-r--r--   0        0        0     1490 2023-06-10 18:44:50.839639 pydis_core-9.8.0/pydis_core/utils/commands.py
--rw-r--r--   0        0        0     7740 2023-06-10 18:44:50.839639 pydis_core-9.8.0/pydis_core/utils/cooldown.py
--rw-r--r--   0        0        0     1253 2023-06-10 18:49:04.941072 pydis_core-9.8.0/pydis_core/utils/error_handling.py
--rw-r--r--   0        0        0     4253 2023-06-10 18:44:50.839639 pydis_core-9.8.0/pydis_core/utils/function.py
--rw-r--r--   0        0        0     4462 2023-06-14 11:22:24.729367 pydis_core-9.8.0/pydis_core/utils/interactions.py
--rw-r--r--   0        0        0     1422 2023-06-10 18:44:50.840639 pydis_core-9.8.0/pydis_core/utils/logging.py
--rw-r--r--   0        0        0     1985 2023-06-10 18:44:50.840639 pydis_core-9.8.0/pydis_core/utils/members.py
--rw-r--r--   0        0        0     3958 2023-06-10 18:44:50.841639 pydis_core-9.8.0/pydis_core/utils/paste_service.py
--rw-r--r--   0        0        0     2397 2022-11-05 14:18:24.793186 pydis_core-9.8.0/pydis_core/utils/regex.py
--rw-r--r--   0        0        0    10730 2023-06-10 18:49:04.941072 pydis_core-9.8.0/pydis_core/utils/scheduling.py
--rw-r--r--   0        0        0     2872 2023-06-14 11:22:24.730366 pydis_core-9.8.0/pyproject.toml
--rw-r--r--   0        0        0      120 2022-05-31 19:45:29.494670 pydis_core-9.8.0/README.md
--rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 pydis_core-9.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-03-31 15:49:16.729733 pydis_core-9.9.0/LICENSE
+-rw-r--r--   0        0        0      320 2023-06-10 18:44:50.836639 pydis_core-9.9.0/pydis_core/__init__.py
+-rw-r--r--   0        0        0    11394 2023-06-10 18:44:50.836639 pydis_core-9.9.0/pydis_core/_bot.py
+-rw-r--r--   0        0        0     1886 2023-06-10 18:44:50.837639 pydis_core-9.9.0/pydis_core/async_stats.py
+-rw-r--r--   0        0        0       93 2023-06-10 18:44:50.837639 pydis_core-9.9.0/pydis_core/exts/__init__.py
+-rw-r--r--   0        0        0     6309 2023-06-10 18:44:50.837639 pydis_core-9.9.0/pydis_core/site_api.py
+-rw-r--r--   0        0        0     1336 2023-06-10 18:49:04.940072 pydis_core-9.9.0/pydis_core/utils/__init__.py
+-rw-r--r--   0        0        0     1680 2022-11-05 14:18:24.788185 pydis_core-9.9.0/pydis_core/utils/_extensions.py
+-rw-r--r--   0        0        0     2749 2023-06-10 18:44:50.838639 pydis_core-9.9.0/pydis_core/utils/_monkey_patches.py
+-rw-r--r--   0        0        0     1810 2022-11-05 14:18:24.789186 pydis_core-9.9.0/pydis_core/utils/caching.py
+-rw-r--r--   0        0        0     1705 2023-06-04 20:04:18.921646 pydis_core-9.9.0/pydis_core/utils/channel.py
+-rw-r--r--   0        0        0     1490 2023-06-10 18:44:50.839639 pydis_core-9.9.0/pydis_core/utils/commands.py
+-rw-r--r--   0        0        0     7740 2023-06-10 18:44:50.839639 pydis_core-9.9.0/pydis_core/utils/cooldown.py
+-rw-r--r--   0        0        0     1253 2023-06-10 18:49:04.941072 pydis_core-9.9.0/pydis_core/utils/error_handling.py
+-rw-r--r--   0        0        0     4253 2023-06-10 18:44:50.839639 pydis_core-9.9.0/pydis_core/utils/function.py
+-rw-r--r--   0        0        0     4462 2023-06-14 11:22:24.729367 pydis_core-9.9.0/pydis_core/utils/interactions.py
+-rw-r--r--   0        0        0     1422 2023-06-10 18:44:50.840639 pydis_core-9.9.0/pydis_core/utils/logging.py
+-rw-r--r--   0        0        0     1985 2023-06-10 18:44:50.840639 pydis_core-9.9.0/pydis_core/utils/members.py
+-rw-r--r--   0        0        0    12906 2023-06-18 19:13:54.974997 pydis_core-9.9.0/pydis_core/utils/paste_service.py
+-rw-r--r--   0        0        0     2397 2022-11-05 14:18:24.793186 pydis_core-9.9.0/pydis_core/utils/regex.py
+-rw-r--r--   0        0        0    10730 2023-06-10 18:49:04.941072 pydis_core-9.9.0/pydis_core/utils/scheduling.py
+-rw-r--r--   0        0        0     2872 2023-06-18 19:14:01.306298 pydis_core-9.9.0/pyproject.toml
+-rw-r--r--   0        0        0      120 2022-05-31 19:45:29.494670 pydis_core-9.9.0/README.md
+-rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 pydis_core-9.9.0/PKG-INFO
```

### Comparing `pydis_core-9.8.0/LICENSE` & `pydis_core-9.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydis_core-9.8.0/pydis_core/_bot.py` & `pydis_core-9.9.0/pydis_core/_bot.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.8.0/pydis_core/async_stats.py` & `pydis_core-9.9.0/pydis_core/async_stats.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.8.0/pydis_core/site_api.py` & `pydis_core-9.9.0/pydis_core/site_api.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.8.0/pydis_core/utils/__init__.py` & `pydis_core-9.9.0/pydis_core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.8.0/pydis_core/utils/_extensions.py` & `pydis_core-9.9.0/pydis_core/utils/_extensions.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.8.0/pydis_core/utils/_monkey_patches.py` & `pydis_core-9.9.0/pydis_core/utils/_monkey_patches.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.8.0/pydis_core/utils/caching.py` & `pydis_core-9.9.0/pydis_core/utils/caching.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.8.0/pydis_core/utils/channel.py` & `pydis_core-9.9.0/pydis_core/utils/channel.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.8.0/pydis_core/utils/commands.py` & `pydis_core-9.9.0/pydis_core/utils/commands.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.8.0/pydis_core/utils/cooldown.py` & `pydis_core-9.9.0/pydis_core/utils/cooldown.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.8.0/pydis_core/utils/error_handling.py` & `pydis_core-9.9.0/pydis_core/utils/error_handling.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.8.0/pydis_core/utils/function.py` & `pydis_core-9.9.0/pydis_core/utils/function.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.8.0/pydis_core/utils/interactions.py` & `pydis_core-9.9.0/pydis_core/utils/interactions.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.8.0/pydis_core/utils/logging.py` & `pydis_core-9.9.0/pydis_core/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.8.0/pydis_core/utils/members.py` & `pydis_core-9.9.0/pydis_core/utils/members.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.8.0/pydis_core/utils/regex.py` & `pydis_core-9.9.0/pydis_core/utils/regex.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.8.0/pydis_core/utils/scheduling.py` & `pydis_core-9.9.0/pydis_core/utils/scheduling.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.8.0/pyproject.toml` & `pydis_core-9.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydis_core"
-version = "9.8.0"
+version = "9.9.0"
 description = "PyDis core provides core functionality and utility to the bots of the Python Discord community."
 authors = ["Python Discord <info@pythondiscord.com>"]
 license = "MIT"
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `pydis_core-9.8.0/PKG-INFO` & `pydis_core-9.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydis-core
-Version: 9.8.0
+Version: 9.9.0
 Summary: PyDis core provides core functionality and utility to the bots of the Python Discord community.
 Home-page: https://pythondiscord.com/
 License: MIT
 Keywords: bot,discord,discord.py
 Author: Python Discord
 Author-email: info@pythondiscord.com
 Requires-Python: >=3.10.dev0,<3.12.dev0
```

