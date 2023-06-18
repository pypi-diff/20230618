# Comparing `tmp/nonebot-plugin-mcqq-1.2.2.tar.gz` & `tmp/nonebot-plugin-mcqq-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-mcqq-1.2.2.tar", last modified: Sun Jun 18 16:26:21 2023, max compression
+gzip compressed data, was "nonebot-plugin-mcqq-1.2.3.tar", last modified: Sun Jun 18 16:42:22 2023, max compression
```

## Comparing `nonebot-plugin-mcqq-1.2.2.tar` & `nonebot-plugin-mcqq-1.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:26:21.468087 nonebot-plugin-mcqq-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-18 16:26:15.000000 nonebot-plugin-mcqq-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-18 16:26:21.468087 nonebot-plugin-mcqq-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-18 16:26:15.000000 nonebot-plugin-mcqq-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:26:21.464087 nonebot-plugin-mcqq-1.2.2/nonebot_plugin_mcqq/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-18 16:26:15.000000 nonebot-plugin-mcqq-1.2.2/nonebot_plugin_mcqq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-18 16:26:15.000000 nonebot-plugin-mcqq-1.2.2/nonebot_plugin_mcqq/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-18 16:26:15.000000 nonebot-plugin-mcqq-1.2.2/nonebot_plugin_mcqq/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:26:21.468087 nonebot-plugin-mcqq-1.2.2/nonebot_plugin_mcqq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-18 16:26:21.000000 nonebot-plugin-mcqq-1.2.2/nonebot_plugin_mcqq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-18 16:26:21.000000 nonebot-plugin-mcqq-1.2.2/nonebot_plugin_mcqq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 16:26:21.000000 nonebot-plugin-mcqq-1.2.2/nonebot_plugin_mcqq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-18 16:26:21.000000 nonebot-plugin-mcqq-1.2.2/nonebot_plugin_mcqq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-18 16:26:21.000000 nonebot-plugin-mcqq-1.2.2/nonebot_plugin_mcqq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 16:26:21.468087 nonebot-plugin-mcqq-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-18 16:26:15.000000 nonebot-plugin-mcqq-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:22.048681 nonebot-plugin-mcqq-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-18 16:42:14.000000 nonebot-plugin-mcqq-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-18 16:42:22.048681 nonebot-plugin-mcqq-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-18 16:42:14.000000 nonebot-plugin-mcqq-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:22.048681 nonebot-plugin-mcqq-1.2.3/nonebot_plugin_mcqq/
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-18 16:42:14.000000 nonebot-plugin-mcqq-1.2.3/nonebot_plugin_mcqq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-18 16:42:14.000000 nonebot-plugin-mcqq-1.2.3/nonebot_plugin_mcqq/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-18 16:42:14.000000 nonebot-plugin-mcqq-1.2.3/nonebot_plugin_mcqq/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:22.048681 nonebot-plugin-mcqq-1.2.3/nonebot_plugin_mcqq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-18 16:42:22.000000 nonebot-plugin-mcqq-1.2.3/nonebot_plugin_mcqq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-18 16:42:22.000000 nonebot-plugin-mcqq-1.2.3/nonebot_plugin_mcqq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 16:42:22.000000 nonebot-plugin-mcqq-1.2.3/nonebot_plugin_mcqq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-18 16:42:22.000000 nonebot-plugin-mcqq-1.2.3/nonebot_plugin_mcqq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-18 16:42:22.000000 nonebot-plugin-mcqq-1.2.3/nonebot_plugin_mcqq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 16:42:22.048681 nonebot-plugin-mcqq-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-18 16:42:14.000000 nonebot-plugin-mcqq-1.2.3/setup.py
```

### Comparing `nonebot-plugin-mcqq-1.2.2/LICENSE` & `nonebot-plugin-mcqq-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.2.2/PKG-INFO` & `nonebot-plugin-mcqq-1.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcqq
-Version: 1.2.2
+Version: 1.2.3
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通插件
 Home-page: https://github.com/17TheWord/nonebot-plugin-mcqq
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot-plugin-mcqq-1.2.2/README.md` & `nonebot-plugin-mcqq-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.2.2/nonebot_plugin_mcqq/__init__.py` & `nonebot-plugin-mcqq-1.2.3/nonebot_plugin_mcqq/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,22 @@
 from nonebot.plugin import PluginMetadata
 
 from .data_source import start_ws_server, stop_ws_server
 from .utils import msg_rule
 
 __plugin_meta__ = PluginMetadata(
     name="MC_QQ",
-    description="适配 OneBot V11（QQ）与 Minecraft 服务器通信的插件",
+    description="基于NoneBot的与Minecraft Server互通消息的插件",
+    homepage="https://github.com/17TheWord/nonebot-plugin-mcqq",
     usage="在群聊发送消息即可同步至 Minecraft 服务器",
     config=Config,
-    extra={},
+    type="application",
+    supported_adapters=[
+        "nonebot.adapters.onebot.v11"
+    ]
 )
 
 mc_qq = on_message(priority=2, rule=msg_rule)
 
 mc_qq_cmd = on_command("minecraft_command", aliases={"mcc"}, priority=1, rule=msg_rule, block=True)
 
 driver = get_driver()
```

### Comparing `nonebot-plugin-mcqq-1.2.2/nonebot_plugin_mcqq/data_source.py` & `nonebot-plugin-mcqq-1.2.3/nonebot_plugin_mcqq/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.2.2/nonebot_plugin_mcqq/utils.py` & `nonebot-plugin-mcqq-1.2.3/nonebot_plugin_mcqq/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.2.2/nonebot_plugin_mcqq.egg-info/PKG-INFO` & `nonebot-plugin-mcqq-1.2.3/nonebot_plugin_mcqq.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcqq
-Version: 1.2.2
+Version: 1.2.3
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通插件
 Home-page: https://github.com/17TheWord/nonebot-plugin-mcqq
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot-plugin-mcqq-1.2.2/setup.py` & `nonebot-plugin-mcqq-1.2.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot-plugin-mcqq",
-    version="1.2.2",
+    version="1.2.3",
     author="17TheWord",
     author_email="17theword@gmail.com",
     description="基于NoneBot的QQ群聊与Minecraft Server消息互通插件",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/17TheWord/nonebot-plugin-mcqq",
     packages=["nonebot_plugin_mcqq"],
```

