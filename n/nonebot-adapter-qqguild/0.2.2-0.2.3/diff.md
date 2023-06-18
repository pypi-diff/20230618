# Comparing `tmp/nonebot_adapter_qqguild-0.2.2.tar.gz` & `tmp/nonebot_adapter_qqguild-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_qqguild-0.2.2.tar", max compression
+gzip compressed data, was "nonebot_adapter_qqguild-0.2.3.tar", max compression
```

## Comparing `nonebot_adapter_qqguild-0.2.2.tar` & `nonebot_adapter_qqguild-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1064 2023-03-12 07:10:37.992717 nonebot_adapter_qqguild-0.2.2/LICENSE
--rw-r--r--   0        0        0      906 2023-03-12 07:10:37.992717 nonebot_adapter_qqguild-0.2.2/README.md
--rw-r--r--   0        0        0      213 2023-03-12 07:10:37.992717 nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/__init__.py
--rw-r--r--   0        0        0    12609 2023-03-12 07:10:37.992717 nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/adapter.py
--rw-r--r--   0        0        0      113 2023-03-12 07:10:37.996717 nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/api/__init__.py
--rw-r--r--   0        0        0     9306 2023-03-12 07:10:37.996717 nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/api/client.py
--rw-r--r--   0        0        0    21451 2023-03-12 07:10:37.996717 nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/api/handle.py
--rw-r--r--   0        0        0    10734 2023-03-12 07:10:37.996717 nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/api/model.py
--rw-r--r--   0        0        0     1668 2023-03-12 07:10:37.996717 nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/api/request.py
--rw-r--r--   0        0        0     1023 2023-03-12 07:10:37.996717 nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/api/utils.py
--rw-r--r--   0        0        0     6537 2023-03-12 07:10:37.996717 nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/bot.py
--rw-r--r--   0        0        0     1353 2023-03-12 07:10:37.996717 nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/config.py
--rw-r--r--   0        0        0     8004 2023-03-12 07:10:37.996717 nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/event.py
--rw-r--r--   0        0        0     2292 2023-03-12 07:10:37.996717 nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/exception.py
--rw-r--r--   0        0        0     6703 2023-03-12 07:10:37.996717 nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/message.py
--rw-r--r--   0        0        0     2087 2023-03-12 07:10:37.996717 nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/payload.py
--rw-r--r--   0        0        0      874 2023-03-12 07:10:37.996717 nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/store.py
--rw-r--r--   0        0        0     3416 2023-03-12 07:10:37.996717 nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/transformer.py
--rw-r--r--   0        0        0      289 2023-03-12 07:10:37.996717 nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/utils.py
--rw-r--r--   0        0        0     1661 2023-03-12 07:10:37.996717 nonebot_adapter_qqguild-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2008 1970-01-01 00:00:00.000000 nonebot_adapter_qqguild-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-18 15:43:56.922875 nonebot_adapter_qqguild-0.2.3/LICENSE
+-rw-r--r--   0        0        0      895 2023-06-18 15:43:56.922875 nonebot_adapter_qqguild-0.2.3/README.md
+-rw-r--r--   0        0        0      239 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/__init__.py
+-rw-r--r--   0        0        0    12671 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/adapter.py
+-rw-r--r--   0        0        0      113 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/api/__init__.py
+-rw-r--r--   0        0        0     9270 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/api/client.py
+-rw-r--r--   0        0        0    21428 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/api/handle.py
+-rw-r--r--   0        0        0    10734 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/api/model.py
+-rw-r--r--   0        0        0     1668 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/api/request.py
+-rw-r--r--   0        0        0     1023 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/api/utils.py
+-rw-r--r--   0        0        0     6410 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/bot.py
+-rw-r--r--   0        0        0     1353 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/config.py
+-rw-r--r--   0        0        0     9534 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/event.py
+-rw-r--r--   0        0        0     2292 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/exception.py
+-rw-r--r--   0        0        0     6703 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/message.py
+-rw-r--r--   0        0        0     2087 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/payload.py
+-rw-r--r--   0        0        0      982 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/permission.py
+-rw-r--r--   0        0        0      874 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/store.py
+-rw-r--r--   0        0        0     3416 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/transformer.py
+-rw-r--r--   0        0        0      289 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/utils.py
+-rw-r--r--   0        0        0     1697 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1949 1970-01-01 00:00:00.000000 nonebot_adapter_qqguild-0.2.3/PKG-INFO
```

### Comparing `nonebot_adapter_qqguild-0.2.2/LICENSE` & `nonebot_adapter_qqguild-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qqguild-0.2.2/README.md` & `nonebot_adapter_qqguild-0.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-  <a href="https://v2.nonebot.dev/"><img src="https://raw.githubusercontent.com/nonebot/adapter-qqguild/master/assets/logo.png" width="200" height="200" alt="nonebot-adapter-qqguild"></a>
+  <a href="https://nonebot.dev/"><img src="https://raw.githubusercontent.com/nonebot/adapter-qqguild/master/assets/logo.png" width="200" height="200" alt="nonebot-adapter-qqguild"></a>
 </p>
 
 <div align="center">
 
 # NoneBot-Adapter-QQGuild
 
 _✨ QQ 频道协议适配 ✨_
@@ -12,15 +12,15 @@
 
 ## 配置
 
 修改 NoneBot 配置文件 `.env` 或者 `.env.*`。
 
 ### Driver
 
-参考 [driver](https://v2.nonebot.dev/docs/tutorial/configuration#driver) 配置项，添加 `ForwardDriver` 支持。
+参考 [driver](https://nonebot.dev/docs/appendices/config#driver) 配置项，添加 `ForwardDriver` 支持。
 
 如：
 
 ```dotenv
 DRIVER=~httpx+~websockets
 DRIVER=~aiohttp
 ```
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
                            [nonebot-adapter-qqguild]
            # NoneBot-Adapter-QQGuild _â¨ QQ é¢éåè®®éé â¨_
 ## éç½® ä¿®æ¹ NoneBot éç½®æä»¶ `.env` æè `.env.*`ã ### Driver
-åè [driver](https://v2.nonebot.dev/docs/tutorial/configuration#driver)
+åè [driver](https://nonebot.dev/docs/appendices/config#driver)
 éç½®é¡¹ï¼æ·»å  `ForwardDriver` æ¯æã å¦ï¼ ```dotenv
 DRIVER=~httpx+~websockets DRIVER=~aiohttp ``` ### QQGUILD_IS_SANDBOX
 æ¯å¦ä¸ºæ²çæ¨¡å¼ï¼é»è®¤ä¸º `False`ã ```dotenv QQGUILD_IS_SANDBOX=true
 ``` ### QQGUILD_BOTS éç½®æºå¨äººå¸å·ï¼å¦ï¼ ```dotenv QQGUILD_BOTS=' [
 { "id": "xxx", "token": "xxx", "secret": "xxx", "intent": { "guild_messages":
 true, "at_messages": false } } ] ' ```
```

### Comparing `nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/adapter.py` & `nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/adapter.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from pydantic import parse_raw_as
 from nonebot.typing import overrides
 from nonebot.utils import escape_tag
 from nonebot.exception import WebSocketClosed
 from nonebot.drivers import URL, Driver, Request, WebSocket, ForwardDriver
 
 from nonebot.adapters import Adapter as BaseAdapter
-from nonebot.adapters.qqguild.exception import ApiNotAvailable
 
 from .bot import Bot
 from .utils import log
 from .api import API_HANDLERS
 from .store import audit_result
 from .config import Config, BotInfo
-from .event import Event, MessageAuditEvent, event_classes
+from .exception import ApiNotAvailable
+from .event import Event, ReadyEvent, MessageAuditEvent, event_classes
 from .payload import (
     Hello,
     Resume,
     Payload,
     Dispatch,
     Identify,
     Heartbeat,
@@ -137,119 +137,33 @@
                 async with self.websocket(request) as ws:
                     log(
                         "DEBUG",
                         f"WebSocket Connection to {escape_tag(str(ws_url))} established",
                     )
 
                     try:
-                        try:
-                            payload = await self.receive_payload(ws)
-                            assert isinstance(
-                                payload, Hello
-                            ), f"Received unexpected payload: {payload!r}"
-                            heartbeat_interval = payload.data.heartbeat_interval
-                        except Exception as e:
-                            log(
-                                "ERROR",
-                                "<r><bg #f8bbd0>Error while receiving server hello event</bg #f8bbd0></r>",
-                                e,
-                            )
+                        # hello
+                        heartbeat_interval = await self._hello(ws)
+                        if not heartbeat_interval:
                             await asyncio.sleep(RECONNECT_INTERVAL)
                             continue
 
-                        if not bot.ready:
-                            payload = Identify.parse_obj(
-                                {
-                                    "data": {
-                                        "token": self.get_authorization(bot.bot_info),
-                                        "intents": bot.bot_info.intent.to_int(),
-                                        "shard": list(shard),
-                                        "properties": {
-                                            "$os": sys.platform,
-                                            "$sdk": "NoneBot2",
-                                        },
-                                    },
-                                }
-                            )
-                        else:
-                            payload = Resume.parse_obj(
-                                {
-                                    "data": {
-                                        "token": self.get_authorization(bot.bot_info),
-                                        "session_id": bot.session_id,
-                                        "seq": bot.sequence,
-                                    }
-                                }
-                            )
-
-                        try:
-                            await ws.send(json.dumps(payload.dict()))
-                        except Exception as e:
-                            log(
-                                "ERROR",
-                                "<r><bg #f8bbd0>Error while sending " + "Identify"
-                                if isinstance(payload, Identify)
-                                else "Resume" + " event</bg #f8bbd0></r>",
-                                e,
-                            )
+                        # identify/resume
+                        result = await self._authenticate(bot, ws, shard)
+                        if not result:
                             await asyncio.sleep(RECONNECT_INTERVAL)
                             continue
 
-                        # only connect for single shard
-                        if bot.self_id not in self.bots:
-                            self.bot_connect(bot)
-                            log(
-                                "INFO",
-                                f"<y>Bot {escape_tag(bot.self_id)}</y> connected",
-                            )
                         # start heartbeat
                         heartbeat_task = asyncio.create_task(
                             self._heartbeat(ws, bot, heartbeat_interval)
                         )
-                        while True:
-                            payload = await self.receive_payload(ws)
-                            log(
-                                "TRACE",
-                                f"Received payload: {escape_tag(repr(payload))}",
-                            )
-                            if isinstance(payload, Dispatch):
-                                bot.sequence = payload.sequence
-                                try:
-                                    event = self.payload_to_event(payload)
-                                except Exception as e:
-                                    log(
-                                        "WARNING",
-                                        f"Failed to parse event {escape_tag(repr(payload))}",
-                                        e,
-                                    )
-                                else:
-                                    if isinstance(event, MessageAuditEvent):
-                                        audit_result.add_result(event)
-                                    asyncio.create_task(bot.handle_event(event))
-                            elif isinstance(payload, HeartbeatAck):
-                                log("TRACE", "Heartbeat ACK")
-                                continue
-                            elif isinstance(payload, Reconnect):
-                                log(
-                                    "WARNING",
-                                    "Received reconnect event from server. Try to reconnect...",
-                                )
-                                break
-                            elif isinstance(payload, InvalidSession):
-                                bot.clear()
-                                log(
-                                    "ERROR",
-                                    "Received invalid session event from server. Try to reconnect...",
-                                )
-                                break
-                            else:
-                                log(
-                                    "WARNING",
-                                    f"Unknown payload from server: {escape_tag(repr(payload))}",
-                                )
+
+                        # process events
+                        await self._loop(bot, ws)
                     except WebSocketClosed as e:
                         log(
                             "ERROR",
                             f"<r><bg #f8bbd0>WebSocket Closed</bg #f8bbd0></r>",
                             e,
                         )
                     except Exception as e:
@@ -271,25 +185,153 @@
                     "<r><bg #f8bbd0>Error while setup websocket to "
                     f"{escape_tag(str(ws_url))}. Trying to reconnect...</bg #f8bbd0></r>",
                     e,
                 )
 
             await asyncio.sleep(RECONNECT_INTERVAL)
 
+    async def _hello(self, ws: WebSocket):
+        """接收并处理服务器的 Hello 事件"""
+        try:
+            payload = await self.receive_payload(ws)
+            assert isinstance(
+                payload, Hello
+            ), f"Received unexpected payload: {payload!r}"
+            return payload.data.heartbeat_interval
+        except Exception as e:
+            log(
+                "ERROR",
+                "<r><bg #f8bbd0>Error while receiving server hello event</bg #f8bbd0></r>",
+                e,
+            )
+
+    async def _authenticate(self, bot: Bot, ws: WebSocket, shard: Tuple[int, int]):
+        """鉴权连接"""
+        if not bot.ready:
+            payload = Identify.parse_obj(
+                {
+                    "data": {
+                        "token": self.get_authorization(bot.bot_info),
+                        "intents": bot.bot_info.intent.to_int(),
+                        "shard": list(shard),
+                        "properties": {
+                            "$os": sys.platform,
+                            "$sdk": "NoneBot2",
+                        },
+                    },
+                }
+            )
+        else:
+            payload = Resume.parse_obj(
+                {
+                    "data": {
+                        "token": self.get_authorization(bot.bot_info),
+                        "session_id": bot.session_id,
+                        "seq": bot.sequence,
+                    }
+                }
+            )
+
+        try:
+            await ws.send(json.dumps(payload.dict()))
+        except Exception as e:
+            log(
+                "ERROR",
+                "<r><bg #f8bbd0>Error while sending " + "Identify"
+                if isinstance(payload, Identify)
+                else "Resume" + " event</bg #f8bbd0></r>",
+                e,
+            )
+            return
+
+        ready_event = None
+        if not bot.ready:
+            # https://bot.q.qq.com/wiki/develop/api/gateway/reference.html#_2-%E9%89%B4%E6%9D%83%E8%BF%9E%E6%8E%A5
+            # 鉴权成功之后，后台会下发一个 Ready Event
+            payload = await self.receive_payload(ws)
+            assert isinstance(
+                payload, Dispatch
+            ), f"Received unexpected payload: {payload!r}"
+            bot.sequence = payload.sequence
+            ready_event = self.payload_to_event(payload)
+            assert isinstance(
+                ready_event, ReadyEvent
+            ), f"Received unexpected event: {ready_event!r}"
+            bot.session_id = ready_event.session_id
+            bot.self_info = ready_event.user
+
+        # only connect for single shard
+        if bot.self_id not in self.bots:
+            self.bot_connect(bot)
+            log(
+                "INFO",
+                f"<y>Bot {escape_tag(bot.self_id)}</y> connected",
+            )
+
+        if ready_event:
+            asyncio.create_task(bot.handle_event(ready_event))
+
+        return True
+
     async def _heartbeat(self, ws: WebSocket, bot: Bot, heartbeat_interval: int):
+        """心跳"""
         while True:
             if bot.has_sequence:
                 log("TRACE", f"Heartbeat {bot.sequence}")
                 payload = Heartbeat.parse_obj({"data": bot.sequence})
                 try:
                     await ws.send(json.dumps(payload.dict()))
                 except Exception:
                     pass
             await asyncio.sleep(heartbeat_interval / 1000)
 
+    async def _loop(self, bot: Bot, ws: WebSocket):
+        """接收并处理事件"""
+        while True:
+            payload = await self.receive_payload(ws)
+            log(
+                "TRACE",
+                f"Received payload: {escape_tag(repr(payload))}",
+            )
+            if isinstance(payload, Dispatch):
+                bot.sequence = payload.sequence
+                try:
+                    event = self.payload_to_event(payload)
+                except Exception as e:
+                    log(
+                        "WARNING",
+                        f"Failed to parse event {escape_tag(repr(payload))}",
+                        e,
+                    )
+                else:
+                    if isinstance(event, MessageAuditEvent):
+                        audit_result.add_result(event)
+                    asyncio.create_task(bot.handle_event(event))
+            elif isinstance(payload, HeartbeatAck):
+                log("TRACE", "Heartbeat ACK")
+                continue
+            elif isinstance(payload, Reconnect):
+                log(
+                    "WARNING",
+                    "Received reconnect event from server. Try to reconnect...",
+                )
+                break
+            elif isinstance(payload, InvalidSession):
+                bot.clear()
+                log(
+                    "ERROR",
+                    "Received invalid session event from server. Try to reconnect...",
+                )
+                break
+            else:
+                log(
+                    "WARNING",
+                    f"Unknown payload from server: {escape_tag(repr(payload))}",
+                )
+
     def get_api_base(self) -> URL:
         if self.qqguild_config.qqguild_is_sandbox:
             return URL(self.qqguild_config.qqguild_sandbox_api_base)
         else:
             return URL(self.qqguild_config.qqguild_api_base)
 
     def get_authorization(self, bot: BotInfo) -> str:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/api/client.py` & `nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/api/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from datetime import date, datetime
 from typing import TYPE_CHECKING, List, Optional
 
 from pydantic import Extra, BaseModel
 
 from .model import *
 
 if TYPE_CHECKING:
```

### Comparing `nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/api/handle.py` & `nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/api/handle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-import json
-from typing import TYPE_CHECKING, Any, Dict, List, Optional
+from typing import TYPE_CHECKING, List, Optional
 
 from pydantic import parse_obj_as
 from nonebot.drivers import Request
 
 from .model import *
 from .utils import parse_send_message
 from .request import _request, _exclude_none
```

### Comparing `nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/api/model.py` & `nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/api/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/api/request.py` & `nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/api/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/api/utils.py` & `nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/api/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/bot.py` & `nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from nonebot.adapters import Bot as BaseBot
 
 from .utils import log
 from .config import BotInfo
 from .api import User, ApiClient
 from .message import Message, MessageSegment
-from .event import Event, ReadyEvent, MessageEvent, DirectMessageCreateEvent
+from .event import Event, MessageEvent, DirectMessageCreateEvent
 
 if TYPE_CHECKING:
     from .adapter import Adapter
 
 
 async def _check_reply(bot: "Bot", event: MessageEvent) -> None:
     """检查消息中存在的回复，赋值 `event.reply`, `event.to_me`。
@@ -128,18 +128,15 @@
         self._sequence = sequence
 
     def clear(self) -> None:
         self._session_id = None
         self._sequence = None
 
     async def handle_event(self, event: Event) -> None:
-        if isinstance(event, ReadyEvent):
-            self.session_id = event.session_id
-            self.self_info = event.user
-        elif isinstance(event, MessageEvent):
+        if isinstance(event, MessageEvent):
             await _check_reply(self, event)
             _check_at_me(self, event)
         await handle_event(self, event)
 
     @overrides(BaseBot)
     async def send(
         self,
@@ -166,15 +163,15 @@
         if reference := (message["reference"] or None):
             reference = reference[-1].data["reference"]
 
         # 私信需要使用 post_dms_messages
         # https://bot.q.qq.com/wiki/develop/api/openapi/dms/post_dms_messages.html#%E5%8F%91%E9%80%81%E7%A7%81%E4%BF%A1
         if isinstance(event, DirectMessageCreateEvent):
             return await self.post_dms_messages(
-                guild_id=event.guild_id,
+                guild_id=event.guild_id,  # type: ignore
                 msg_id=event.id,
                 content=content,
                 embed=embed,  # type: ignore
                 ark=ark,  # type: ignore
                 image=image,  # type: ignore
                 file_image=file_image,  # type: ignore
                 markdown=markdown,  # type: ignore
```

### Comparing `nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/config.py` & `nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/event.py` & `nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/event.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from nonebot.utils import escape_tag
 
 from nonebot.adapters import Event as BaseEvent
 
 from .message import Message
 from .api import Message as GuildMessage
 from .api import User, Guild, Member, Channel
-from .api import MessageGet, MessageAudited, MessageReaction
+from .api import MessageGet, MessageDelete, MessageAudited, MessageReaction
 
 
 class EventType(str, Enum):
     # Init Event
     READY = "READY"
     RESUMED = "RESUMED"
 
@@ -28,21 +28,23 @@
     # GUILD_MEMBERS
     GUILD_MEMBER_ADD = "GUILD_MEMBER_ADD"
     GUILD_MEMBER_UPDATE = "GUILD_MEMBER_UPDATE"
     GUILD_MEMBER_REMOVE = "GUILD_MEMBER_REMOVE"
 
     # GUILD_MESSAGES
     MESSAGE_CREATE = "MESSAGE_CREATE"
+    MESSAGE_DELETE = "MESSAGE_DELETE"
 
     # GUILD_MESSAGE_REACTIONS
     MESSAGE_REACTION_ADD = "MESSAGE_REACTION_ADD"
     MESSAGE_REACTION_REMOVE = "MESSAGE_REACTION_REMOVE"
 
     # DIRECT_MESSAGE
     DIRECT_MESSAGE_CREATE = "DIRECT_MESSAGE_CREATE"
+    DIRECT_MESSAGE_DELETE = "DIRECT_MESSAGE_DELETE"
 
     # MESSAGE_AUDIT
     MESSAGE_AUDIT_PASS = "MESSAGE_AUDIT_PASS"
     MESSAGE_AUDIT_REJECT = "MESSAGE_AUDIT_REJECT"
 
     # FORUM_EVENT
     THREAD_CREATE = "THREAD_CREATE"
@@ -57,14 +59,15 @@
     AUDIO_START = "AUDIO_START"
     AUDIO_FINISH = "AUDIO_FINISH"
     AUDIO_ON_MIC = "AUDIO_ON_MIC"
     AUDIO_OFF_MIC = "AUDIO_OFF_MIC"
 
     # AT_MESSAGES
     AT_MESSAGE_CREATE = "AT_MESSAGE_CREATE"
+    PUBLIC_MESSAGE_DELETE = "PUBLIC_MESSAGE_DELETE"
 
 
 class Event(BaseEvent):
     __type__: EventType
 
     @overrides(BaseEvent)
     def get_event_name(self) -> str:
@@ -162,14 +165,20 @@
         return "notice"
 
     @overrides(Event)
     def get_user_id(self) -> str:
         return str(self.user.id)  # type: ignore
 
     @overrides(Event)
+    def get_event_description(self) -> str:
+        return escape_tag(
+            f"Notice {getattr(self.user, 'username', None)}@[Guild:{self.guild_id}] Roles:{self.roles}"
+        )
+
+    @overrides(Event)
     def get_session_id(self) -> str:
         return str(self.user.id)  # type: ignore
 
 
 class GuildMemberAddEvent(GuildMemberEvent):
     __type__ = EventType.GUILD_MEMBER_ADD
 
@@ -201,14 +210,20 @@
     def get_user_id(self) -> str:
         return str(self.author.id)  # type: ignore
 
     @overrides(Event)
     def get_session_id(self) -> str:
         return str(self.author.id)  # type: ignore
 
+    @overrides(BaseEvent)
+    def get_event_description(self) -> str:
+        return escape_tag(
+            f"Message {self.id} from {getattr(self.author, 'username', None)}@[Guild:{self.guild_id}/{self.channel_id}] Roles:{getattr(self.member, 'roles', None)}: {self.get_message()}"
+        )
+
     @overrides(Event)
     def get_message(self) -> Message:
         if not hasattr(self, "_message"):
             setattr(self, "_message", Message.from_guild_message(self))
         return getattr(self, "_message")
 
     @overrides(Event)
@@ -216,23 +231,45 @@
         return self.to_me
 
 
 class MessageCreateEvent(MessageEvent):
     __type__ = EventType.MESSAGE_CREATE
 
 
+class MessageDeleteEvent(Event, MessageDelete):
+    __type__ = EventType.MESSAGE_DELETE
+
+    @overrides(BaseEvent)
+    def get_type(self) -> str:
+        return "notice"
+
+
 class AtMessageCreateEvent(MessageEvent):
     __type__ = EventType.AT_MESSAGE_CREATE
     to_me: bool = True
 
 
+class PublicMessageDeleteEvent(MessageDeleteEvent):
+    __type__ = EventType.PUBLIC_MESSAGE_DELETE
+
+
 class DirectMessageCreateEvent(MessageEvent):
     __type__ = EventType.DIRECT_MESSAGE_CREATE
     to_me: bool = True
 
+    @overrides(MessageEvent)
+    def get_event_description(self) -> str:
+        return escape_tag(
+            f"Message {self.id} from {getattr(self.author, 'username', None)}: {self.get_message()}"
+        )
+
+
+class DirectMessageDeleteEvent(MessageDeleteEvent):
+    __type__ = EventType.DIRECT_MESSAGE_DELETE
+
 
 # Message Audit Event
 class MessageAuditEvent(Event, MessageAudited):
     @overrides(BaseEvent)
     def get_type(self) -> str:
         return "notice"
 
@@ -279,16 +316,19 @@
     EventType.CHANNEL_CREATE.value: ChannelCreateEvent,
     EventType.CHANNEL_DELETE.value: ChannelDeleteEvent,
     EventType.CHANNEL_UPDATE.value: ChannelUpdateEvent,
     EventType.GUILD_MEMBER_ADD.value: GuildMemberAddEvent,
     EventType.GUILD_MEMBER_UPDATE.value: GuildMemberUpdateEvent,
     EventType.GUILD_MEMBER_REMOVE.value: GuildMemberRemoveEvent,
     EventType.MESSAGE_CREATE.value: MessageCreateEvent,
+    EventType.MESSAGE_DELETE.value: MessageDeleteEvent,
     EventType.AT_MESSAGE_CREATE.value: AtMessageCreateEvent,
+    EventType.PUBLIC_MESSAGE_DELETE.value: PublicMessageDeleteEvent,
     EventType.DIRECT_MESSAGE_CREATE.value: DirectMessageCreateEvent,
+    EventType.DIRECT_MESSAGE_DELETE.value: DirectMessageDeleteEvent,
     EventType.MESSAGE_AUDIT_PASS.value: MessageAuditPassEvent,
     EventType.MESSAGE_AUDIT_REJECT.value: MessageAuditRejectEvent,
     EventType.MESSAGE_REACTION_ADD.value: MessageReactionAddEvent,
     EventType.MESSAGE_REACTION_REMOVE.value: MessageReactionRemoveEvent,
 }
 
 __all__ = [
@@ -304,16 +344,19 @@
     "ChannelDeleteEvent",
     "GuildMemberEvent",
     "GuildMemberAddEvent",
     "GuildMemberUpdateEvent",
     "GuildMemberRemoveEvent",
     "MessageEvent",
     "MessageCreateEvent",
+    "MessageDeleteEvent",
     "AtMessageCreateEvent",
+    "PublicMessageDeleteEvent",
     "DirectMessageCreateEvent",
+    "DirectMessageDeleteEvent",
     "MessageAuditEvent",
     "MessageAuditPassEvent",
     "MessageAuditRejectEvent",
     "MessageReactionEvent",
     "MessageReactionAddEvent",
     "MessageReactionRemoveEvent",
 ]
```

### Comparing `nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/exception.py` & `nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/message.py` & `nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/payload.py` & `nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/payload.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/store.py` & `nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qqguild-0.2.2/nonebot/adapters/qqguild/transformer.py` & `nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/transformer.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qqguild-0.2.2/pyproject.toml` & `nonebot_adapter_qqguild-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-qqguild"
-version = "0.2.2"
+version = "0.2.3"
 description = "QQ Guild adapter for nonebot2"
 authors = ["yanyongyu <yyy@nonebot.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/nonebot/adapter-qqguild"
 repository = "https://github.com/nonebot/adapter-qqguild"
 documentation = "https://github.com/nonebot/adapter-qqguild#readme"
@@ -23,18 +23,18 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.9.0"
 nonebot2 = "^2.0.0-beta.1"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.10.1"
-black = "^22.1.0"
+black = "^23.1.0"
 Jinja2 = "^3.0.3"
 nonemoji = "^0.1.3"
-pre-commit = "^2.17.0"
+pre-commit = "^3.3.0"
 httpx = ">=0.22.0, <1.0.0"
 nonebot2 = { git = "https://github.com/nonebot/nonebot2.git" }
 
 [tool.black]
 line-length = 88
 include = '\.pyi?$'
 extend-exclude = '''
@@ -44,14 +44,18 @@
 profile = "black"
 line_length = 88
 length_sort = true
 skip_gitignore = true
 force_sort_within_sections = true
 extra_standard_library = ["typing_extensions"]
 
+[tool.pycln]
+path = "."
+all = false
+
 [tool.pyright]
 pythonVersion = "3.8"
 pythonPlatform = "All"
 
 [tool.codegen]
 url = "https://cdn.jsdelivr.net/gh/tencent-connect/bot-oas/v1/openapi.yaml"
 model-output = "nonebot/adapters/qqguild/api/model.py"
```

### Comparing `nonebot_adapter_qqguild-0.2.2/PKG-INFO` & `nonebot_adapter_qqguild-0.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-qqguild
-Version: 0.2.2
+Version: 0.2.3
 Summary: QQ Guild adapter for nonebot2
 Home-page: https://github.com/nonebot/adapter-qqguild
 License: MIT
 Keywords: bot,qq,qqbot,qqguild
 Author: yanyongyu
 Author-email: yyy@nonebot.dev
 Requires-Python: >=3.8,<4.0
@@ -14,23 +14,22 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Requires-Dist: nonebot2 (>=2.0.0-beta.1,<3.0.0)
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
 Project-URL: Documentation, https://github.com/nonebot/adapter-qqguild#readme
 Project-URL: Repository, https://github.com/nonebot/adapter-qqguild
 Description-Content-Type: text/markdown
 
 <p align="center">
-  <a href="https://v2.nonebot.dev/"><img src="https://raw.githubusercontent.com/nonebot/adapter-qqguild/master/assets/logo.png" width="200" height="200" alt="nonebot-adapter-qqguild"></a>
+  <a href="https://nonebot.dev/"><img src="https://raw.githubusercontent.com/nonebot/adapter-qqguild/master/assets/logo.png" width="200" height="200" alt="nonebot-adapter-qqguild"></a>
 </p>
 
 <div align="center">
 
 # NoneBot-Adapter-QQGuild
 
 _✨ QQ 频道协议适配 ✨_
@@ -39,15 +38,15 @@
 
 ## 配置
 
 修改 NoneBot 配置文件 `.env` 或者 `.env.*`。
 
 ### Driver
 
-参考 [driver](https://v2.nonebot.dev/docs/tutorial/configuration#driver) 配置项，添加 `ForwardDriver` 支持。
+参考 [driver](https://nonebot.dev/docs/appendices/config#driver) 配置项，添加 `ForwardDriver` 支持。
 
 如：
 
 ```dotenv
 DRIVER=~httpx+~websockets
 DRIVER=~aiohttp
 ```
```

#### html2text {}

```diff
@@ -1,25 +1,24 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-qqguild Version: 0.2.2 Summary: QQ
+Metadata-Version: 2.1 Name: nonebot-adapter-qqguild Version: 0.2.3 Summary: QQ
 Guild adapter for nonebot2 Home-page: https://github.com/nonebot/adapter-
 qqguild License: MIT Keywords: bot,qq,qqbot,qqguild Author: yanyongyu Author-
 email: yyy@nonebot.dev Requires-Python: >=3.8,<4.0 Classifier: Development
 Status :: 5 - Production/Stable Classifier: Framework :: Robot Framework
 Classifier: Framework :: Robot Framework :: Library Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3
-Requires-Dist: nonebot2 (>=2.0.0-beta.1,<3.0.0) Requires-Dist: pydantic
-(>=1.9.0,<2.0.0) Project-URL: Documentation, https://github.com/nonebot/
-adapter-qqguild#readme Project-URL: Repository, https://github.com/nonebot/
-adapter-qqguild Description-Content-Type: text/markdown
+Language :: Python :: 3.11 Requires-Dist: nonebot2 (>=2.0.0-beta.1,<3.0.0)
+Requires-Dist: pydantic (>=1.9.0,<2.0.0) Project-URL: Documentation, https://
+github.com/nonebot/adapter-qqguild#readme Project-URL: Repository, https://
+github.com/nonebot/adapter-qqguild Description-Content-Type: text/markdown
                            [nonebot-adapter-qqguild]
            # NoneBot-Adapter-QQGuild _â¨ QQ é¢éåè®®éé â¨_
 ## éç½® ä¿®æ¹ NoneBot éç½®æä»¶ `.env` æè `.env.*`ã ### Driver
-åè [driver](https://v2.nonebot.dev/docs/tutorial/configuration#driver)
+åè [driver](https://nonebot.dev/docs/appendices/config#driver)
 éç½®é¡¹ï¼æ·»å  `ForwardDriver` æ¯æã å¦ï¼ ```dotenv
 DRIVER=~httpx+~websockets DRIVER=~aiohttp ``` ### QQGUILD_IS_SANDBOX
 æ¯å¦ä¸ºæ²çæ¨¡å¼ï¼é»è®¤ä¸º `False`ã ```dotenv QQGUILD_IS_SANDBOX=true
 ``` ### QQGUILD_BOTS éç½®æºå¨äººå¸å·ï¼å¦ï¼ ```dotenv QQGUILD_BOTS=' [
 { "id": "xxx", "token": "xxx", "secret": "xxx", "intent": { "guild_messages":
 true, "at_messages": false } } ] ' ```
```

