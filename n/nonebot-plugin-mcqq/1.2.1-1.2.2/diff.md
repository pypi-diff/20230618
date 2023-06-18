# Comparing `tmp/nonebot-plugin-mcqq-1.2.1.tar.gz` & `tmp/nonebot-plugin-mcqq-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-mcqq-1.2.1.tar", last modified: Tue May  9 03:14:47 2023, max compression
+gzip compressed data, was "nonebot-plugin-mcqq-1.2.2.tar", last modified: Sun Jun 18 16:26:21 2023, max compression
```

## Comparing `nonebot-plugin-mcqq-1.2.1.tar` & `nonebot-plugin-mcqq-1.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:14:47.557895 nonebot-plugin-mcqq-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-09 03:14:40.000000 nonebot-plugin-mcqq-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-09 03:14:47.557895 nonebot-plugin-mcqq-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-09 03:14:40.000000 nonebot-plugin-mcqq-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:14:47.557895 nonebot-plugin-mcqq-1.2.1/nonebot_plugin_mcqq/
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-09 03:14:40.000000 nonebot-plugin-mcqq-1.2.1/nonebot_plugin_mcqq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-09 03:14:40.000000 nonebot-plugin-mcqq-1.2.1/nonebot_plugin_mcqq/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-09 03:14:40.000000 nonebot-plugin-mcqq-1.2.1/nonebot_plugin_mcqq/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:14:47.557895 nonebot-plugin-mcqq-1.2.1/nonebot_plugin_mcqq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-09 03:14:47.000000 nonebot-plugin-mcqq-1.2.1/nonebot_plugin_mcqq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-09 03:14:47.000000 nonebot-plugin-mcqq-1.2.1/nonebot_plugin_mcqq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 03:14:47.000000 nonebot-plugin-mcqq-1.2.1/nonebot_plugin_mcqq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-09 03:14:47.000000 nonebot-plugin-mcqq-1.2.1/nonebot_plugin_mcqq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-09 03:14:47.000000 nonebot-plugin-mcqq-1.2.1/nonebot_plugin_mcqq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 03:14:47.557895 nonebot-plugin-mcqq-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-09 03:14:40.000000 nonebot-plugin-mcqq-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:26:21.468087 nonebot-plugin-mcqq-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-18 16:26:15.000000 nonebot-plugin-mcqq-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-18 16:26:21.468087 nonebot-plugin-mcqq-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-18 16:26:15.000000 nonebot-plugin-mcqq-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:26:21.464087 nonebot-plugin-mcqq-1.2.2/nonebot_plugin_mcqq/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-18 16:26:15.000000 nonebot-plugin-mcqq-1.2.2/nonebot_plugin_mcqq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-18 16:26:15.000000 nonebot-plugin-mcqq-1.2.2/nonebot_plugin_mcqq/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-18 16:26:15.000000 nonebot-plugin-mcqq-1.2.2/nonebot_plugin_mcqq/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:26:21.468087 nonebot-plugin-mcqq-1.2.2/nonebot_plugin_mcqq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-18 16:26:21.000000 nonebot-plugin-mcqq-1.2.2/nonebot_plugin_mcqq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-18 16:26:21.000000 nonebot-plugin-mcqq-1.2.2/nonebot_plugin_mcqq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 16:26:21.000000 nonebot-plugin-mcqq-1.2.2/nonebot_plugin_mcqq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-18 16:26:21.000000 nonebot-plugin-mcqq-1.2.2/nonebot_plugin_mcqq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-18 16:26:21.000000 nonebot-plugin-mcqq-1.2.2/nonebot_plugin_mcqq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 16:26:21.468087 nonebot-plugin-mcqq-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-18 16:26:15.000000 nonebot-plugin-mcqq-1.2.2/setup.py
```

### Comparing `nonebot-plugin-mcqq-1.2.1/LICENSE` & `nonebot-plugin-mcqq-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.2.1/PKG-INFO` & `nonebot-plugin-mcqq-1.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: nonebot-plugin-mcqq
-Version: 1.2.1
-Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通插件
-Home-page: https://github.com/17TheWord/nonebot-plugin-mcqq
-Author: 17TheWord
-Author-email: 17theword@gmail.com
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![nonebot-plugin-mcqq](https://socialify.git.ci/17TheWord/nonebot-plugin-mcqq/image?description=1&font=Inter&forks=1&issues=1&language=1&logo=https%3A%2F%2Favatars.githubusercontent.com%2F17TheWord&owner=1&pattern=Plus&stargazers=1&theme=Dark)](https://17theword.github.io/mc_qq/)
 
 # NoneBot-Plugin-MCQQ
 
 基于 `NoneBot` 的与 `Minecraft Server` 互通消息插件
 
 - 支持QQ群、QQ频道
```

### Comparing `nonebot-plugin-mcqq-1.2.1/README.md` & `nonebot-plugin-mcqq-1.2.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: nonebot-plugin-mcqq
+Version: 1.2.2
+Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通插件
+Home-page: https://github.com/17TheWord/nonebot-plugin-mcqq
+Author: 17TheWord
+Author-email: 17theword@gmail.com
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![nonebot-plugin-mcqq](https://socialify.git.ci/17TheWord/nonebot-plugin-mcqq/image?description=1&font=Inter&forks=1&issues=1&language=1&logo=https%3A%2F%2Favatars.githubusercontent.com%2F17TheWord&owner=1&pattern=Plus&stargazers=1&theme=Dark)](https://17theword.github.io/mc_qq/)
 
 # NoneBot-Plugin-MCQQ
 
 基于 `NoneBot` 的与 `Minecraft Server` 互通消息插件
 
 - 支持QQ群、QQ频道
```

### Comparing `nonebot-plugin-mcqq-1.2.1/nonebot_plugin_mcqq/__init__.py` & `nonebot-plugin-mcqq-1.2.2/nonebot_plugin_mcqq/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 from typing import Union
 
+from mcqq_tool.config import Config
 from mcqq_tool.common import GUILD_ADMIN
 from mcqq_tool.utils import send_msg_to_mc, send_cmd_to_mc
 from nonebot import on_message, on_command, get_driver
 from nonebot.adapters import Message
 from nonebot.params import CommandArg
 from nonebot.permission import SUPERUSER
 from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent, GROUP_ADMIN, GROUP_OWNER
 from nonebot_plugin_guild_patch import GuildMessageEvent
+from nonebot.plugin import PluginMetadata
 
 from .data_source import start_ws_server, stop_ws_server
 from .utils import msg_rule
 
+__plugin_meta__ = PluginMetadata(
+    name="MC_QQ",
+    description="适配 OneBot V11（QQ）与 Minecraft 服务器通信的插件",
+    usage="在群聊发送消息即可同步至 Minecraft 服务器",
+    config=Config,
+    extra={},
+)
+
 mc_qq = on_message(priority=2, rule=msg_rule)
 
 mc_qq_cmd = on_command("minecraft_command", aliases={"mcc"}, priority=1, rule=msg_rule, block=True)
 
 driver = get_driver()
```

### Comparing `nonebot-plugin-mcqq-1.2.1/nonebot_plugin_mcqq/data_source.py` & `nonebot-plugin-mcqq-1.2.2/nonebot_plugin_mcqq/data_source.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,56 +13,74 @@
         server_name = websocket.request_headers["x-self-name"].encode('utf-8').decode('unicode_escape')
     except KeyError as e:
         # 服务器名为空
         logger.error(f"[MC_QQ]丨未获取到该服务器的名称，连接断开：{e}")
         await websocket.close(1008, "[MC_QQ]丨未获取到该服务器的名称，连接断开")
         return
     else:
-        try:
-            CLIENTS.get(server_name)
-        except KeyError as e:
-            # 服务器名不在配置文件中
-            logger.error(f"[MC_QQ]丨[Server:{server_name}] 未在配置文件中配置，连接断开：{e}")
-            await websocket.close(1008, f"[MC_QQ]丨[Server:{server_name}] 未在配置文件中配置，连接断开")
+
+        if CLIENTS.get(server_name) is None:
+            # 服务器名已存在
+            logger.error(f"[MC_QQ]丨已有相同服务器名的连接，连接断开")
+            await websocket.close(1008, "[MC_QQ]丨已有相同服务器名的连接")
             return
+
         rcon_client = None
+        bot_id = ""
         for server in plugin_config.mc_qq_server_list:
-            if server_name == server.server_name and server.rcon_enable:
-                rcon_client = aiomcrcon.Client(
-                    websocket.remote_address[0],
-                    plugin_config.mc_qq_rcon_dict[server_name],
-                    plugin_config.mc_qq_rcon_password
-                )
-                await rcon_connect(rcon_client=rcon_client, server_name=server_name)
-                break
+            if server_name == server.server_name:
+                bot_id = str(server.self_id)
+                if server.rcon_enable:
+                    rcon_client = aiomcrcon.Client(
+                        websocket.remote_address[0],
+                        plugin_config.mc_qq_rcon_dict[server_name],
+                        plugin_config.mc_qq_rcon_password
+                    )
+                    await rcon_connect(rcon_client=rcon_client, server_name=server_name)
+                    break
         CLIENTS[server_name] = Client(
             server_name=server_name,
             websocket=websocket,
             rcon=rcon_client
         )
         logger.success(f"[MC_QQ]丨[Server:{server_name}] 已连接至 WebSocket 服务器")
 
         try:
             async for message in websocket:
-                await send_msg_to_qq(bot=get_bot(), message=message)
+                try:
+                    # 获取指定ID Bot
+                    bot = get_bot(bot_id)
+                except KeyError as e:
+                    logger.error(f"[MC_QQ]丨[Server:{server_name}] 的 Bot 未获取，将尝试使用其他Bot发送消息：{e}")
+                    try:
+                        # 获取可用 Bot
+                        bot = get_bot()
+                    except ValueError as e:
+                        logger.error(f"[MC_QQ]丨[Server:{server_name}] 没有可用的 Bot，无法发送消息：{e}")
+                    else:
+                        # 以可用 Bot 发送消息
+                        # 如果 Bot 未在指定群聊，则会报错
+                        await send_msg_to_qq(bot=bot, message=message)
+                else:
+                    # 以指定ID Bot 发送消息
+                    await send_msg_to_qq(bot=bot, message=message)
+
         except websockets.WebSocketException as e:
-            # 移除当前客户端
-            await remove_client(server_name=server_name)
-            logger.error(f"[MC_QQ]丨[Server:{server_name}] 的 WebSocket 连接已断开：{e}")
-        else:
+            logger.error(f"[MC_QQ]丨[Server:{server_name}] 的 WebSocket 出现异常：{e}")
+        finally:
             if websocket.closed:
-                await remove_client(server_name=server_name)
                 logger.error(f"[MC_QQ]丨[Server:{server_name}] 的 WebSocket 连接已断开")
+            await remove_client(server_name=server_name)
 
 
 async def start_ws_server():
     """启动 WebSocket 服务器"""
     global ws
     ws = await websockets.serve(ws_client, plugin_config.mc_qq_ws_ip, plugin_config.mc_qq_ws_port)
-    logger.success("[MC_QQ]丨WebSocket 服务器已开启")
+    logger.success(f"[MC_QQ]丨WebSocket 服务器已在 {plugin_config.mc_qq_ws_ip}:{plugin_config.mc_qq_ws_port} 已开启")
 
 
 async def stop_ws_server():
     """关闭 WebSocket 服务器"""
     global ws
     ws.close()
     logger.success("[MC_QQ]丨WebSocket 服务器已关闭")
```

### Comparing `nonebot-plugin-mcqq-1.2.1/nonebot_plugin_mcqq/utils.py` & `nonebot-plugin-mcqq-1.2.2/nonebot_plugin_mcqq/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.2.1/nonebot_plugin_mcqq.egg-info/PKG-INFO` & `nonebot-plugin-mcqq-1.2.2/nonebot_plugin_mcqq.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcqq
-Version: 1.2.1
+Version: 1.2.2
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通插件
 Home-page: https://github.com/17TheWord/nonebot-plugin-mcqq
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot-plugin-mcqq-1.2.1/setup.py` & `nonebot-plugin-mcqq-1.2.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot-plugin-mcqq",
-    version="1.2.1",
+    version="1.2.2",
     author="17TheWord",
     author_email="17theword@gmail.com",
     description="基于NoneBot的QQ群聊与Minecraft Server消息互通插件",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/17TheWord/nonebot-plugin-mcqq",
     packages=["nonebot_plugin_mcqq"],
     classifiers=[
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: OS Independent"
     ],
     install_requires=[
         'mcqq-tool>=0.0.5',
-        'nonebot2>=2.0.0rc4',
+        'nonebot2>=2.0.0',
         'nonebot-adapter-onebot>=2.1.1',
         'nonebot-plugin-guild-patch>=0.2.0',
         'websockets>=10.3',
         'aio-mc-rcon>=3.2.0'
     ]
 )
```

