# Comparing `tmp/nonebot-plugin-mcversion-0.1.2.tar.gz` & `tmp/nonebot-plugin-mcversion-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-mcversion-0.1.2.tar", last modified: Mon Jun 12 14:44:59 2023, max compression
+gzip compressed data, was "nonebot-plugin-mcversion-0.2.0.tar", last modified: Sun Jun 18 11:13:34 2023, max compression
```

## Comparing `nonebot-plugin-mcversion-0.1.2.tar` & `nonebot-plugin-mcversion-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1065 2023-06-12 14:44:48.571203 nonebot-plugin-mcversion-0.1.2/LICENSE
--rw-r--r--   0        0        0     1931 2023-06-12 14:44:48.571203 nonebot-plugin-mcversion-0.1.2/README.md
--rw-r--r--   0        0        0     4199 2023-06-12 14:44:48.571203 nonebot-plugin-mcversion-0.1.2/nonebot_plugin_mcversion/__init__.py
--rw-r--r--   0        0        0      621 2023-06-12 14:44:48.571203 nonebot-plugin-mcversion-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2314 1970-01-01 00:00:00.000000 nonebot-plugin-mcversion-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-18 11:13:20.557077 nonebot-plugin-mcversion-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1931 2023-06-18 11:13:20.557077 nonebot-plugin-mcversion-0.2.0/README.md
+-rw-r--r--   0        0        0     2547 2023-06-18 11:13:20.557077 nonebot-plugin-mcversion-0.2.0/nonebot_plugin_mcversion/__init__.py
+-rw-r--r--   0        0        0      621 2023-06-18 11:13:20.557077 nonebot-plugin-mcversion-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2314 1970-01-01 00:00:00.000000 nonebot-plugin-mcversion-0.2.0/PKG-INFO
```

### Comparing `nonebot-plugin-mcversion-0.1.2/LICENSE` & `nonebot-plugin-mcversion-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcversion-0.1.2/README.md` & `nonebot-plugin-mcversion-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcversion-0.1.2/pyproject.toml` & `nonebot-plugin-mcversion-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-mcversion"
-version = "0.1.2"
+version = "0.2.0"
 description = "NoneBot2 plugin for CheckMCupdate"
 authors = [
     { name = "CN171-1", email = "3428166361@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc2",
     "nonebot-adapter-onebot>=2.1.5",
```

### Comparing `nonebot-plugin-mcversion-0.1.2/PKG-INFO` & `nonebot-plugin-mcversion-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcversion
-Version: 0.1.2
+Version: 0.2.0
 Summary: NoneBot2 plugin for CheckMCupdate
 License: MIT
 Author-email: CN171-1 <3428166361@qq.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/CN171-1/nonebot-plugin-mcversion
 Project-URL: Repository, https://github.com/CN171-1/nonebot-plugin-mcversion
 Description-Content-Type: text/markdown
```

