# Comparing `tmp/ipcs-0.1.4.tar.gz` & `tmp/ipcs-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipcs-0.1.4.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `ipcs-0.1.4.tar` & `ipcs-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,26 @@
--rw-r--r--   0        0        0     1070 2022-12-31 05:37:18.641438 ipcs-0.1.4/LICENSE
--rw-r--r--   0        0        0     1553 2023-01-07 11:01:29.687242 ipcs-0.1.4/README.md
--rw-r--r--   0        0        0      403 2023-04-03 06:20:25.116332 ipcs-0.1.4/ipcs/__init__.py
--rw-r--r--   0        0        0     1416 2023-04-03 06:20:51.294255 ipcs-0.1.4/ipcs/__main__.py
--rw-r--r--   0        0        0    19189 2023-04-03 06:22:14.134797 ipcs-0.1.4/ipcs/client.py
--rw-r--r--   0        0        0     3405 2023-04-03 06:22:59.710887 ipcs-0.1.4/ipcs/connection.py
--rw-r--r--   0        0        0     1198 2023-04-03 06:23:15.878915 ipcs-0.1.4/ipcs/errors.py
--rw-r--r--   0        0        0     5328 2023-04-03 06:23:26.103865 ipcs-0.1.4/ipcs/server.py
--rw-r--r--   0        0        0     1874 2023-04-03 06:23:40.322738 ipcs-0.1.4/ipcs/types_.py
--rw-r--r--   0        0        0     2104 2023-04-03 06:24:04.107326 ipcs-0.1.4/ipcs/utils.py
--rw-r--r--   0        0        0      763 2023-04-03 06:24:36.470931 ipcs-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2338 1970-01-01 00:00:00.000000 ipcs-0.1.4/setup.py
--rw-r--r--   0        0        0     2423 1970-01-01 00:00:00.000000 ipcs-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 ipcs-0.1.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 ipcs-0.1.5/README.md
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 ipcs-0.1.5/mypy.ini
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 ipcs-0.1.5/test.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ipcs-0.1.5/.github/dependabot.yml
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 ipcs-0.1.5/.venv/.gitignore
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 ipcs-0.1.5/docs/conf.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 ipcs-0.1.5/docs/event_reference.rst
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 ipcs-0.1.5/docs/index.rst
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 ipcs-0.1.5/docs/ipcs.rst
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 ipcs-0.1.5/docs/modules.rst
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ipcs-0.1.5/docs/requirements.txt
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 ipcs-0.1.5/examples/chat.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 ipcs-0.1.5/examples/readme.md
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 ipcs-0.1.5/src/ipcs/__init__.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 ipcs-0.1.5/src/ipcs/__main__.py
+-rw-r--r--   0        0        0    19183 2020-02-02 00:00:00.000000 ipcs-0.1.5/src/ipcs/client.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 ipcs-0.1.5/src/ipcs/connection.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 ipcs-0.1.5/src/ipcs/errors.py
+-rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 ipcs-0.1.5/src/ipcs/server.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 ipcs-0.1.5/src/ipcs/types_.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 ipcs-0.1.5/src/ipcs/utils.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ipcs-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ipcs-0.1.5/LICENSE
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 ipcs-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 ipcs-0.1.5/PKG-INFO
```

### Comparing `ipcs-0.1.4/LICENSE` & `ipcs-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ipcs-0.1.4/README.md` & `ipcs-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ipcs-0.1.4/ipcs/__main__.py` & `ipcs-0.1.5/src/ipcs/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-"ipcs - Main"
-
 from argparse import ArgumentParser
 import logging
 
 try:
     from ipcs import __version__, Server, Request
     from ipcs.client import logger
 except ImportError:
```

### Comparing `ipcs-0.1.4/ipcs/client.py` & `ipcs-0.1.5/src/ipcs/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-"ipcs - Client"
-
 from __future__ import annotations
 
 __all__ = ("Request", "AbcClient", "Client", "logger")
 
 from typing import TypeAlias, Generic, TypeVar, ParamSpec, Any, cast
 from collections.abc import Callable, Coroutine
 
@@ -231,36 +229,41 @@
         ))
         data = ResponsePayload(
             source=self.id_, target=payload["source"], secret=payload["secret"],
             session=payload["session"], route=payload["route"], type="response",
             status="error", result=None
         )
         function = None
+
         try:
             if payload["route"] not in self.routes and (
                 payload["secret"] and payload["route"] not in self._secret_routes
             ):
                 raise IdIsNotFound("The route is not found: %s" % payload_to_str(payload))
+
             function = self._secret_routes[payload["route"]] \
                 if payload["secret"] else \
                 self.routes[payload["route"]]
             result = function(
                 Request.from_payload(self.connections[payload["source"]], payload),
                 *payload["args"], **payload["kwargs"]
             )
+
             if getattr(function, "__ipcs_is_coroutine_function__"):
                 result = await result
         except Exception as error:
             logger.exception(self._IGNORE_EXC % f"in route '{payload['route']}'")
             data["result"] = error_to_str(error)
         else:
             data["result"] = result
             data["status"] = "ok"
+
         logger.info("Response: %s" % payload_to_str(payload))
         self.dispatch("on_response", data)
+
         try:
             await self._send(data)
         except TypeError:
             logger.error(
                 "The return value was something that could not be made into data: %s"
                     % (None if function is None else getfile(function))
             )
@@ -307,19 +310,22 @@
             c.request(route, *args, **kwargs),
             name="ipcs: request_all: %s" % c.id_
         )) for c in filter(
             lambda c: key_(c) and c.id_ != self.id_,
             self.connections.values()
         )}:
             result, error = None, None
+
             try:
                 result = await task
             except RequestError as e:
                 error = e
+
             data[id_] = (result, error)
+
         return data
 
     @abstractmethod
     async def start(self, *args: Any, **kwargs: Any) -> None:
         "This method is not fully implemented. Implemented are :class:`ipcs.client.Client` and :class:`ipcs.server.Server`."
         self._closing = False
         self.dispatch("on_ready")
@@ -331,16 +337,18 @@
             id_or_connection = self.connections[id_or_connection]
         await id_or_connection.close()
 
     @abstractmethod
     async def close(self, code: int = 1000, reason: str = "...") -> None:
         "This method is not fully implemented. Implemented are :class:`ipcs.client.Client` and :class:`ipcs.server.Server`."
         logger.info("Closing...")
+
         self._closing = True
         self.dispatch("on_close", code, reason)
+
         await asyncio.gather(*(
             self._close_connection(connection)
             for connection in list(self.connections.values())
         ))
 
     async def _wrapped_start(self, args, kwargs) -> None:
         try:
@@ -356,15 +364,15 @@
 
         Args:
             *args: The arguments to be passed to :meth:`ipcs.AbcClient.start`.
             **kwrags: The keyword arguments to be passed to :meth:`ipcs.AbcClient.start`."""
         try:
             asyncio.run(self._wrapped_start(args, kwargs))
         except KeyboardInterrupt:
-            ...
+            pass
 
 
 class Client(AbcClient[Connection]):
     "This is the class of the client for ipc communication with the server."
 
     ready: asyncio.Event
     """This is an ``Event`` in the standard library asyncio to put if it has already started (connected to the server).
```

### Comparing `ipcs-0.1.4/ipcs/connection.py` & `ipcs-0.1.5/src/ipcs/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-"ipcs - Connection"
-
 from __future__ import annotations
 
 __all__ = ("Connection",)
 
 from typing import TYPE_CHECKING, Any
 
 import asyncio
```

### Comparing `ipcs-0.1.4/ipcs/errors.py` & `ipcs-0.1.5/src/ipcs/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-"ipcs - Errors"
-
 __all__ = (
     "IpcsError", "IdIsNotFound", "RequestError", "FailedToRequestError",
     "FailedToProcessError", "ClosedConnectionError"
 )
 
 from typing import Any
```

### Comparing `ipcs-0.1.4/ipcs/server.py` & `ipcs-0.1.5/src/ipcs/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-"ipcs - Server"
-
 __all__ = ("ConnectionForServer", "Server")
 
 from typing import Any
 
 from asyncio import Future
 
 from websockets.exceptions import ConnectionClosed
```

### Comparing `ipcs-0.1.4/ipcs/types_.py` & `ipcs-0.1.5/src/ipcs/types_.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-"icps - Types"
-
 __all__ = (
     "BasePayload", "RequestPayload",
     "ResponsePayload", "WebSocketProtocol"
 )
 
 from typing import Protocol, TypedDict, Literal, Any
 from collections.abc import Sequence
@@ -48,16 +46,15 @@
 
 
 class WebSocketProtocol(Protocol):
     "Protocol class to indicate functions that must be implemented in the class for WebSocket communication used within ipcs."
 
     @property
     def closed(self) -> bool:
-        "Returns whether the websocket is closed or not."
-        ...
+        "Returns whether the websocket is closed or not."; ...
 
     async def send(self, data: Any, *args: Any, **kwargs: Any) -> None:
         "Sends data via websockets."
 
     async def recv(self) -> Any:
         "Receives data via websockets."
```

### Comparing `ipcs-0.1.4/ipcs/utils.py` & `ipcs-0.1.5/src/ipcs/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-"ipcs - Utils"
-
 __all__ = ("SimpleAttrDict", "DataEvent", "payload_to_str")
 
 from typing import TypeVar, Generic
 
 from asyncio import Event as AsyncioEvent
 
 from .types_ import RequestPayload, ResponsePayload
```

