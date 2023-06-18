# Comparing `tmp/eva4-repl-legacy-0.0.9.tar.gz` & `tmp/eva4-repl-legacy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eva4-repl-legacy-0.0.9.tar", last modified: Fri Apr  1 21:33:41 2022, max compression
+gzip compressed data, was "eva4-repl-legacy-0.1.0.tar", last modified: Sun Jun 18 17:21:41 2023, max compression
```

## Comparing `eva4-repl-legacy-0.0.9.tar` & `eva4-repl-legacy-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2022-04-01 21:33:41.306388 eva4-repl-legacy-0.0.9/
--rw-r--r--   0 divisor   (1000) root         (0)      509 2022-04-01 21:33:41.306388 eva4-repl-legacy-0.0.9/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)       46 2022-03-19 18:21:20.000000 eva4-repl-legacy-0.0.9/README.md
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2022-04-01 21:33:41.302387 eva4-repl-legacy-0.0.9/bin/
--rwxr-xr-x   0 divisor   (1000) root         (0)       71 2022-03-22 22:13:22.000000 eva4-repl-legacy-0.0.9/bin/eva4-repl-legacy
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2022-04-01 21:33:41.306388 eva4-repl-legacy-0.0.9/eva4_repl_legacy/
--rw-r--r--   0 divisor   (1000) root         (0)    19703 2022-04-01 21:33:39.000000 eva4-repl-legacy-0.0.9/eva4_repl_legacy/__init__.py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2022-04-01 21:33:41.306388 eva4-repl-legacy-0.0.9/eva4_repl_legacy.egg-info/
--rw-r--r--   0 divisor   (1000) root         (0)      509 2022-04-01 21:33:41.000000 eva4-repl-legacy-0.0.9/eva4_repl_legacy.egg-info/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)      267 2022-04-01 21:33:41.000000 eva4-repl-legacy-0.0.9/eva4_repl_legacy.egg-info/SOURCES.txt
--rw-r--r--   0 divisor   (1000) root         (0)        1 2022-04-01 21:33:41.000000 eva4-repl-legacy-0.0.9/eva4_repl_legacy.egg-info/dependency_links.txt
--rw-r--r--   0 divisor   (1000) root         (0)      112 2022-04-01 21:33:41.000000 eva4-repl-legacy-0.0.9/eva4_repl_legacy.egg-info/requires.txt
--rw-r--r--   0 divisor   (1000) root         (0)       17 2022-04-01 21:33:41.000000 eva4-repl-legacy-0.0.9/eva4_repl_legacy.egg-info/top_level.txt
--rw-r--r--   0 divisor   (1000) root         (0)       38 2022-04-01 21:33:41.306388 eva4-repl-legacy-0.0.9/setup.cfg
--rw-r--r--   0 divisor   (1000) root         (0)     1143 2022-04-01 21:33:39.000000 eva4-repl-legacy-0.0.9/setup.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-06-18 17:21:41.259422 eva4-repl-legacy-0.1.0/
+-rw-r--r--   0 divisor   (1000) root         (0)    10639 2022-06-30 23:31:26.000000 eva4-repl-legacy-0.1.0/LICENSE
+-rw-r--r--   0 divisor   (1000) root         (0)      513 2023-06-18 17:21:41.259422 eva4-repl-legacy-0.1.0/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)       46 2022-03-19 18:21:20.000000 eva4-repl-legacy-0.1.0/README.md
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-06-18 17:21:41.259422 eva4-repl-legacy-0.1.0/bin/
+-rwxr-xr-x   0 divisor   (1000) root         (0)       71 2022-03-22 22:13:22.000000 eva4-repl-legacy-0.1.0/bin/eva4-svc-repl-legacy
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-06-18 17:21:41.259422 eva4-repl-legacy-0.1.0/eva4_repl_legacy/
+-rw-r--r--   0 divisor   (1000) root         (0)    21530 2023-06-18 17:21:32.000000 eva4-repl-legacy-0.1.0/eva4_repl_legacy/__init__.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-06-18 17:21:41.259422 eva4-repl-legacy-0.1.0/eva4_repl_legacy.egg-info/
+-rw-r--r--   0 divisor   (1000) root         (0)      513 2023-06-18 17:21:41.000000 eva4-repl-legacy-0.1.0/eva4_repl_legacy.egg-info/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)      279 2023-06-18 17:21:41.000000 eva4-repl-legacy-0.1.0/eva4_repl_legacy.egg-info/SOURCES.txt
+-rw-r--r--   0 divisor   (1000) root         (0)        1 2023-06-18 17:21:41.000000 eva4-repl-legacy-0.1.0/eva4_repl_legacy.egg-info/dependency_links.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       96 2023-06-18 17:21:41.000000 eva4-repl-legacy-0.1.0/eva4_repl_legacy.egg-info/requires.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       17 2023-06-18 17:21:41.000000 eva4-repl-legacy-0.1.0/eva4_repl_legacy.egg-info/top_level.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       38 2023-06-18 17:21:41.259422 eva4-repl-legacy-0.1.0/setup.cfg
+-rw-r--r--   0 divisor   (1000) root         (0)     1108 2023-06-18 17:21:32.000000 eva4-repl-legacy-0.1.0/setup.py
```

### Comparing `eva4-repl-legacy-0.0.9/eva4_repl_legacy/__init__.py` & `eva4-repl-legacy-0.1.0/eva4_repl_legacy/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,61 @@
-__version__ = '0.0.9'
+__version__ = '0.1.0'
 
 import evaics.sdk as sdk
 from types import SimpleNamespace
 import psrt
 import threading
-import msgpack
 import time
 import os
 import uuid
 import zlib
 import hashlib
 import pyaltt2.crypto
-import elbus
+import busrt
 try:
     import rapidjson as json
 except:
     import json
 
 from functools import partial
 from cachetools import TTLCache
 
+from evaics.sdk import pack, unpack
+
 encrypt = partial(pyaltt2.crypto.encrypt, hmac_key=True, b64=False)
 decrypt = partial(pyaltt2.crypto.decrypt, hmac_key=True, b64=False)
 
 key_cache = TTLCache(ttl=5, maxsize=4096)
 
 api_callback = {}
 
 _d = SimpleNamespace(test_passed=threading.Event(), lc={})
 
 
 def get_key_val(key_id):
     try:
         return key_cache[key_id]
     except KeyError:
-        key = msgpack.loads(_d.service.rpc.call(
-            _d.key_svc,
-            elbus.rpc.Request('key.get',
-                              msgpack.dumps({'i': key_id
-                                            }))).wait_completed().get_payload(),
-                            raw=False)['key']
+        key = unpack(
+            _d.service.rpc.call(
+                _d.key_svc, busrt.rpc.Request('key.get', pack(
+                    {'i': key_id}))).wait_completed().get_payload())['key']
         key_cache[key_id] = key
         return key
 
 
-def mark_node(node, status):
+def mark_node(node, status, info=None, timeout=None):
+    payload = {'status': status}
+    if info is not None:
+        payload['info'] = info
+    if timeout is not None:
+        payload['timeout'] = timeout
     _d.service.bus.send(
         f'RPL/NODE/{node}',
-        elbus.client.Frame(msgpack.dumps({'status': status}),
-                           tp=elbus.client.OP_PUBLISH))
+        busrt.client.Frame(pack(payload), tp=busrt.client.OP_PUBLISH))
 
 
 def jreq(id, method, params=None):
     d = {'jsonrpc': '2.0', 'method': method, 'id': id}
     if params is not None:
         d['params'] = params
     return d
@@ -102,57 +105,62 @@
         _d.pubsub.unsubscribe(t)
     except:
         sdk.log_traceback()
 
 
 class LegacyNode:
 
-    def __init__(self, id, key, key_ln, reload_interval, timeout, controllers):
+    def __init__(self, id, key_id, key_lid, reload_interval, ping_interval,
+                 timeout, controllers):
         self.id = id
         for c in controllers:
             if c not in ['uc', 'lm']:
                 raise ValueError(f'invalid controller type: {c}')
         self.controllers = controllers
         self.online = False
         self.reload_interval = reload_interval
+        self.ping_interval = ping_interval
         self._last_reload = 0
-        self.key = key
-        self.key_ln = key_ln
+        self.key_id = key_id
+        self.key_lid = key_lid
         self.timeout = timeout
         self.need_reload = threading.Event()
+        self.need_ping = threading.Event()
+        self.lock = threading.RLock()
         self.build = None
         self.version = None
 
     def call(self, ctype, method, params=None):
-        key_val = get_key_val(self.key)
+        key_val = get_key_val(self.key_id)
         if params is None:
             params = {'k': key_val}
         else:
             params['k'] = key_val
         rid = uuid.uuid4().bytes
         request_id = rid.hex()
         payload = jreq(request_id, method, params)
         controller_id = f'{ctype}/{self.id}'
         private_key = hashlib.sha512(str(key_val).encode()).digest()
         rid = uuid.uuid4().bytes
         request_id = rid.hex()
         header = b'\x00\x03'
-        data = rid + zlib.compress(msgpack.dumps(payload))
+        data = rid + zlib.compress(pack(payload))
         cb = Callback()
         send_api_request(
-            request_id, controller_id, header + self.key_ln.encode() + b'\x00' +
-            encrypt(data, private_key, key_is_hash=True), cb.data_handler)
+            request_id, controller_id, header + self.key_lid.encode() +
+            b'\x00' + encrypt(data, private_key, key_is_hash=True),
+            cb.data_handler)
         if not cb.completed.wait(self.timeout):
             finish_api_request(request_id)
             raise TimeoutError
         if cb.code:
             if cb.code != 200:
                 raise RuntimeError(
                     f'{controller_id} response error code: {cb.code}')
-            content = msgpack.loads(
+            content = unpack(
                 zlib.decompress(decrypt(cb.body, private_key,
                                         key_is_hash=True)))
             try:
                 error = content['error']
                 code = error.get('code', None)
                 msg = error.get('message', '')
                 raise RuntimeError(
@@ -164,55 +172,100 @@
             raise RuntimeError(f'{controller_id} no response')
 
     def serialize(self):
         d = {}
         d['id'] = self.id
         d['controllers'] = self.controllers
         d['online'] = self.online
-        d['key'] = self.key
-        d['key_legacy'] = self.key_ln
+        d['key_id'] = self.key_id
+        d['key_legacy_id'] = self.key_lid
         d['reload_interval'] = self.reload_interval
         d['timeout'] = self.timeout
         d['build'] = self.build
         d['version'] = self.version
         return d
 
     def force_reload(self):
         self._last_reload = 0
         self.need_reload.set()
 
     def start(self):
         logger.info(f'legacy v3 replication for the node {self.id} active')
         threading.Thread(target=self._t_reloader, daemon=True).start()
         threading.Thread(target=self._t_reload_scheduler, daemon=True).start()
+        if self.ping_interval:
+            threading.Thread(target=self._t_pinger, daemon=True).start()
+            threading.Thread(target=self._t_ping_scheduler, daemon=True).start()
 
     def _t_reloader(self):
         while True:
             self.need_reload.wait()
             self.need_reload.clear()
             if (time.perf_counter() -
                     self._last_reload) > self.reload_interval / 2:
                 self._last_reload = time.perf_counter()
                 try:
-                    self.reload()
+                    with self.lock:
+                        self.reload()
                 except:
                     sdk.log_traceback()
             else:
                 logger.warning(
                     f'{self.id} reload triggered too often, skipping')
 
+    def _t_pinger(self):
+        while True:
+            self.need_ping.wait()
+            self.need_ping.clear()
+            try:
+                with self.lock:
+                    self.ping()
+            except:
+                sdk.log_traceback()
+
     def _t_reload_scheduler(self):
         next_reload = time.perf_counter() + self.reload_interval
         while True:
             self.need_reload.set()
             to_sleep = next_reload - time.perf_counter()
             next_reload += self.reload_interval
             if to_sleep > 0:
                 time.sleep(to_sleep)
 
+    def _t_ping_scheduler(self):
+        next_ping = time.perf_counter() + self.ping_interval
+        while True:
+            self.need_ping.set()
+            to_sleep = next_ping - time.perf_counter()
+            next_ping += self.ping_interval
+            if to_sleep > 0:
+                time.sleep(to_sleep)
+
+    def ping(self):
+        try:
+            if not self.controllers:
+                return
+            for i, controller in enumerate(self.controllers):
+                result = self.call(controller, 'test')
+                if i == 0:
+                    self.build = result['product_build']
+                    self.version = result['version']
+            logger.debug(f'{self.id} ping passed')
+            mark_node(self.id,
+                      'online',
+                      info={
+                          'build': self.build,
+                          'version': self.version
+                      },
+                      timeout=self.timeout)
+        except:
+            sdk.log_traceback()
+            self.online = False
+            mark_node(self.id, 'offline')
+
     def reload(self):
         try:
             if not self.controllers:
                 return
             result = self.call(self.controllers[0], 'test')
             self.build = result['product_build']
             self.version = result['version']
@@ -286,33 +339,37 @@
                         'meta': {
                             'description': lmacro.get('description')
                         }
                     }
                     inventory.append(v4lmacro)
             _d.service.bus.send(
                 f'RPL/INVENTORY/{self.id}',
-                elbus.client.Frame(msgpack.dumps(inventory),
-                                   tp=elbus.client.OP_PUBLISH))
+                busrt.client.Frame(pack(inventory), tp=busrt.client.OP_PUBLISH))
             self.online = True
-            mark_node(self.id, 'online')
+            mark_node(self.id,
+                      'online',
+                      info={
+                          'build': self.build,
+                          'version': self.version
+                      },
+                      timeout=self.timeout)
         except:
             sdk.log_traceback()
             self.online = False
             mark_node(self.id, 'offline')
 
 
 def process_message(client, userdata, message):
     topic = message.topic
     if topic == _d.test_topic and message.payload == b'passed':
         logger.debug('PING test passed')
         _d.test_passed.set()
     elif topic in _d.bulks:
         if message.payload.startswith(b'\x00'):
-            payload = msgpack.loads(zlib.decompress(message.payload[2:]),
-                                    raw=False)
+            payload = unpack(zlib.decompress(message.payload[2:]))
         else:
             payload = json.loads(message.payload.decode())
         node_id = payload['c'].split('/')[1]
         for state in payload['d']:
             v4state = {
                 'status': state['status'],
                 'value': state['value'],
@@ -321,16 +378,15 @@
                 'node': node_id
             }
             if 'nstatus' in state:
                 v4state['act'] = 0 if state['status'] == state[
                     'nstatus'] and state['value'] == state['nvalue'] else 1
             _d.service.bus.send(
                 f'RPL/ST/{state["oid"].replace(":", "/",1)}',
-                elbus.client.Frame(msgpack.dumps(v4state),
-                                   tp=elbus.client.OP_PUBLISH))
+                busrt.client.Frame(pack(v4state), tp=busrt.client.OP_PUBLISH))
     elif topic == 'controller/discovery':
         node_id = message.payload.decode().split('/')[1]
         try:
             node = _d.lc[node_id]
             if not node.online:
                 logger.info(f'{node_id} is back online, triggering reload')
                 node.need_reload.set()
@@ -358,34 +414,34 @@
 }
 
 
 def handle_rpc(event):
     method = event.method.decode()
     if method == 'node.list':
         if event.get_payload():
-            raise elbus.rpc.RpcException(code=sdk.ERR_CODE_INVALID_PARAMS)
-        return msgpack.dumps(
+            raise busrt.rpc.RpcException(code=sdk.ERR_CODE_INVALID_PARAMS)
+        return pack(
             sorted([c.serialize() for _, c in _d.lc.items()],
                    key=lambda k: k['id']))
     elif method == 'node.reload':
         try:
-            params = msgpack.loads(event.get_payload(), raw=False)
+            params = unpack(event.get_payload())
             node_id = params['i']
         except Exception as e:
-            raise elbus.rpc.RpcException(str(e), sdk.ERR_CODE_INVALID_PARAMS)
+            raise busrt.rpc.RpcException(str(e), sdk.ERR_CODE_INVALID_PARAMS)
         try:
             node = _d.lc[node_id]
             node.force_reload()
         except KeyError:
-            raise elbus.rpc.RpcException(f'node {node_id} not found',
+            raise busrt.rpc.RpcException(f'node {node_id} not found',
                                          sdk.ERR_CODE_NOT_FOUND)
     # end of user method, the next methods are proxied to v3 nodes
     elif method.startswith('lvar.'):
         try:
-            params = msgpack.loads(event.get_payload(), raw=False)
+            params = unpack(event.get_payload())
             oid = params['i']
             node_id = params['node']
             p = {'i': oid}
             if 'status' in params:
                 p['s'] = params['status']
             if 'value' in params:
                 p['v'] = params['value']
@@ -393,69 +449,69 @@
                     p['v'] = ''
             rm = method[5:]
             if rm == 'incr':
                 rm = 'increment'
             elif rm == 'decr':
                 rm = 'decrement'
         except Exception as e:
-            raise elbus.rpc.RpcException(str(e), sdk.ERR_CODE_INVALID_PARAMS)
+            raise busrt.rpc.RpcException(str(e), sdk.ERR_CODE_INVALID_PARAMS)
         node = _d.lc[node_id]
         node.call('lm', rm, p)
-        return msgpack.dumps(None)
+        return pack(None)
     elif method == 'action':
         try:
-            params = msgpack.loads(event.get_payload(), raw=False)
+            params = unpack(event.get_payload())
             node_id = params['node']
             i = params['i']
             priority = params['priority']
             ap = params['params']
-            status = ap['status']
+            status = ap.get('status', 1)
             p = {'i': i, 'p': priority, 's': status}
             if 'value' in ap:
                 p['v'] = ap['value']
                 if p['v'] is None:
                     p['v'] = ''
             if 'wait' in params:
                 p['w'] = params['wait']
         except Exception as e:
-            raise elbus.rpc.RpcException(str(e), sdk.ERR_CODE_INVALID_PARAMS)
+            raise busrt.rpc.RpcException(str(e), sdk.ERR_CODE_INVALID_PARAMS)
         node = _d.lc[node_id]
         act_info = node.call('uc', 'action', p)
-        return msgpack.dumps(to_v4action(act_info, node_id))
+        return pack(to_v4action(act_info, node_id))
     elif method == 'action.result':
         try:
-            params = msgpack.loads(event.get_payload(), raw=False)
+            params = unpack(event.get_payload())
             node_id = params['node']
             i = params['i']
             u = uuid.UUID(bytes=params['u'])
             ctp = 'lm' if i.startswith('lmacro:') else 'uc'
         except Exception as e:
-            raise elbus.rpc.RpcException(str(e), sdk.ERR_CODE_INVALID_PARAMS)
+            raise busrt.rpc.RpcException(str(e), sdk.ERR_CODE_INVALID_PARAMS)
         node = _d.lc[node_id]
         act_info = node.call(ctp, 'result', {'u': str(u)})
-        return msgpack.dumps(to_v4action(act_info, node_id))
+        return pack(to_v4action(act_info, node_id))
     elif method == 'run':
         try:
-            params = msgpack.loads(event.get_payload(), raw=False)
+            params = unpack(event.get_payload())
             node_id = params['node']
             i = params['i']
             priority = params['priority']
             ap = params['params']
             p = {'i': i, 'p': priority}
             if 'args' in ap:
                 p['a'] = ap['args']
             if 'kwargs' in ap:
                 p['kw'] = ap['kwargs']
             if 'wait' in params:
                 p['w'] = params['wait']
         except Exception as e:
-            raise elbus.rpc.RpcException(str(e), sdk.ERR_CODE_INVALID_PARAMS)
+            raise busrt.rpc.RpcException(str(e), sdk.ERR_CODE_INVALID_PARAMS)
         node = _d.lc[node_id]
         act_info = node.call('lm', 'run', p)
-        return msgpack.dumps(to_v4action(act_info, node_id))
+        return pack(to_v4action(act_info, node_id))
     else:
         sdk.no_rpc_method()
 
 
 def to_v4action(res, node_id):
     ap = {}
     st = res.get('nstatus')
@@ -517,29 +573,32 @@
     info.add_method('node.list')
     info.add_method('node.reload', required=['i'])
     service = sdk.Service()
     _d.service = service
     config = service.get_config()
     pubsub_cfg = config['pubsub']
     service.init_bus()
+    service.drop_privileges()
     logger = service.init_logs()
     if pubsub_cfg['proto'] != 'psrt':
         raise RuntimeError('only PSRT proto is supported')
     del pubsub_cfg['proto']
     if 'user' in pubsub_cfg and pubsub_cfg['user'] is None:
         del pubsub_cfg['user']
     if 'password' in pubsub_cfg and pubsub_cfg['password'] is None:
         del pubsub_cfg['password']
     for id, c in config.get('nodes', {}).items():
-        key = c['key']
-        key_ln = c['key_legacy_name']
+        key_id = c['key_id']
+        key_lid = c['key_legacy_id']
         reload_interval = c['reload_interval']
+        ping_interval = c.get('ping_interval')
         timeout = c.get('timeout', service.timeout['default'])
         controllers = c.get('controllers', [])
-        c = LegacyNode(id, key, key_ln, reload_interval, timeout, controllers)
+        c = LegacyNode(id, key_id, key_lid, reload_interval, ping_interval,
+                       timeout, controllers)
         _d.lc[id] = c
         mark_node(c.id, 'offline')
     pubsub = psrt.Client(**pubsub_cfg)
     pubsub.on_message = process_message
     pubsub.connect()
     test_topic = f'v4/tests/{service.system_name}/{service.id}/test'
     pubsub.subscribe(test_topic)
@@ -549,19 +608,18 @@
     service.on_rpc_call = handle_rpc
     service.init_rpc(info)
     pubsub.subscribe('controller/discovery')
     _d.bulks = [f'state/{t}' for t in pubsub_cfg.get('bulk_subscribe', [])]
     pubsub.subscribe_bulk(_d.bulks)
     service.register_signals()
     service.mark_ready()
-    logger.info('legacy replication service started')
     service.wait_core()
     for _, c in _d.lc.items():
         c.start()
     threading.Thread(target=watch_pubsub, daemon=True).start()
     threading.Thread(target=ping_pubsub, args=(test_topic,),
                      daemon=True).start()
-    service.block()
+    service.block(prepare=False)
     service.mark_terminating()
     for _, c in _d.lc.items():
         mark_node(c.id, 'removed')
     pubsub.bye()
```

### Comparing `eva4-repl-legacy-0.0.9/setup.py` & `eva4-repl-legacy-0.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-__version__ = '0.0.9'
+__version__ = '0.1.0'
 
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(name='eva4-repl-legacy',
                  version=__version__,
                  author='Bohemia Automation / Altertech',
                  author_email='div@altertech.com',
                  description='EVA ICS v4 legacy replication service',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
-                 url='https://github.com/alttch/eva4',
+                 url='https://github.com/eva-ics/eva4',
                  packages=setuptools.find_packages(),
                  license='Apache License 2.0',
                  install_requires=[
-                     'cachetools>=4.11', 'elbus>=0.0.14', 'evaics>=0.0.9',
-                     'msgpack>=1.0.3', 'psrt>=0.0.18', 'pyaltt2>=0.0.116',
-                     'pycryptodomex>=3.12.0'
+                     'cachetools>=4.11', 'busrt>=0.1.0', 'evaics>=0.2.9',
+                     'psrt>=0.0.18', 'pyaltt2>=0.0.116', 'pycryptodomex>=3.12.0'
                  ],
                  classifiers=('Programming Language :: Python :: 3',
                               'License :: OSI Approved :: MIT License',
                               'Topic :: Communications'),
-                 scripts=['bin/eva4-repl-legacy'])
+                 scripts=['bin/eva4-svc-repl-legacy'])
```

