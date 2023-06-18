# Comparing `tmp/eva4-controller-py-0.0.9.tar.gz` & `tmp/eva4-controller-py-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eva4-controller-py-0.0.9.tar", last modified: Wed Apr 27 02:37:48 2022, max compression
+gzip compressed data, was "eva4-controller-py-0.1.0.tar", last modified: Sun Jun 18 20:04:36 2023, max compression
```

## Comparing `eva4-controller-py-0.0.9.tar` & `eva4-controller-py-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2022-04-27 02:37:48.204387 eva4-controller-py-0.0.9/
--rw-r--r--   0 divisor   (1000) root         (0)    10639 2022-03-19 18:20:58.000000 eva4-controller-py-0.0.9/LICENSE
--rw-r--r--   0 divisor   (1000) root         (0)      520 2022-04-27 02:37:48.204387 eva4-controller-py-0.0.9/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)       46 2022-04-01 21:38:20.000000 eva4-controller-py-0.0.9/README.md
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2022-04-27 02:37:48.204387 eva4-controller-py-0.0.9/bin/
--rwxr-xr-x   0 divisor   (1000) root         (0)       75 2022-04-01 21:42:50.000000 eva4-controller-py-0.0.9/bin/eva4-svc-controller-py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2022-04-27 02:37:48.204387 eva4-controller-py-0.0.9/eva4_controller_py/
--rw-r--r--   0 divisor   (1000) root         (0)     5544 2022-04-27 02:18:07.000000 eva4-controller-py-0.0.9/eva4_controller_py/__init__.py
--rw-r--r--   0 divisor   (1000) root         (0)    18005 2022-04-27 02:18:07.000000 eva4-controller-py-0.0.9/eva4_controller_py/macro_api.py
--rw-r--r--   0 divisor   (1000) root         (0)     1049 2022-04-27 02:18:07.000000 eva4-controller-py-0.0.9/eva4_controller_py/macro_builtins.py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2022-04-27 02:37:48.204387 eva4-controller-py-0.0.9/eva4_controller_py.egg-info/
--rw-r--r--   0 divisor   (1000) root         (0)      520 2022-04-27 02:37:48.000000 eva4-controller-py-0.0.9/eva4_controller_py.egg-info/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)      362 2022-04-27 02:37:48.000000 eva4-controller-py-0.0.9/eva4_controller_py.egg-info/SOURCES.txt
--rw-r--r--   0 divisor   (1000) root         (0)        1 2022-04-27 02:37:48.000000 eva4-controller-py-0.0.9/eva4_controller_py.egg-info/dependency_links.txt
--rw-r--r--   0 divisor   (1000) root         (0)       62 2022-04-27 02:37:48.000000 eva4-controller-py-0.0.9/eva4_controller_py.egg-info/requires.txt
--rw-r--r--   0 divisor   (1000) root         (0)       19 2022-04-27 02:37:48.000000 eva4-controller-py-0.0.9/eva4_controller_py.egg-info/top_level.txt
--rw-r--r--   0 divisor   (1000) root         (0)       38 2022-04-27 02:37:48.204387 eva4-controller-py-0.0.9/setup.cfg
--rw-r--r--   0 divisor   (1000) root         (0)     1077 2022-04-27 02:18:07.000000 eva4-controller-py-0.0.9/setup.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-06-18 20:04:36.444981 eva4-controller-py-0.1.0/
+-rw-r--r--   0 divisor   (1000) root         (0)    10639 2022-06-30 23:31:17.000000 eva4-controller-py-0.1.0/LICENSE
+-rw-r--r--   0 divisor   (1000) root         (0)      521 2023-06-18 20:04:36.444981 eva4-controller-py-0.1.0/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)       46 2022-04-01 21:38:20.000000 eva4-controller-py-0.1.0/README.md
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-06-18 20:04:36.440981 eva4-controller-py-0.1.0/bin/
+-rwxr-xr-x   0 divisor   (1000) root         (0)       75 2022-04-01 21:42:50.000000 eva4-controller-py-0.1.0/bin/eva4-svc-controller-py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-06-18 20:04:36.440981 eva4-controller-py-0.1.0/eva4_controller_py/
+-rw-r--r--   0 divisor   (1000) root         (0)     5666 2023-06-18 20:04:26.000000 eva4-controller-py-0.1.0/eva4_controller_py/__init__.py
+-rw-r--r--   0 divisor   (1000) root         (0)    18971 2023-06-18 20:04:26.000000 eva4-controller-py-0.1.0/eva4_controller_py/macro_api.py
+-rw-r--r--   0 divisor   (1000) root         (0)     1049 2023-06-18 20:04:26.000000 eva4-controller-py-0.1.0/eva4_controller_py/macro_builtins.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-06-18 20:04:36.444981 eva4-controller-py-0.1.0/eva4_controller_py.egg-info/
+-rw-r--r--   0 divisor   (1000) root         (0)      521 2023-06-18 20:04:36.000000 eva4-controller-py-0.1.0/eva4_controller_py.egg-info/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)      362 2023-06-18 20:04:36.000000 eva4-controller-py-0.1.0/eva4_controller_py.egg-info/SOURCES.txt
+-rw-r--r--   0 divisor   (1000) root         (0)        1 2023-06-18 20:04:36.000000 eva4-controller-py-0.1.0/eva4_controller_py.egg-info/dependency_links.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       45 2023-06-18 20:04:36.000000 eva4-controller-py-0.1.0/eva4_controller_py.egg-info/requires.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       19 2023-06-18 20:04:36.000000 eva4-controller-py-0.1.0/eva4_controller_py.egg-info/top_level.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       38 2023-06-18 20:04:36.444981 eva4-controller-py-0.1.0/setup.cfg
+-rw-r--r--   0 divisor   (1000) root         (0)      820 2023-06-18 20:04:26.000000 eva4-controller-py-0.1.0/setup.py
```

### Comparing `eva4-controller-py-0.0.9/LICENSE` & `eva4-controller-py-0.1.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-EVA ICS v3 is licensed under Apache License 2.0 with additional Common Clauses
+EVA ICS v4 is licensed under Apache License 2.0 with additional Common Clauses
 (1).
 
 Minor modules may contain the code, developed or included under different
 non-compatible Open Source licenses. In this case, specific module license may
 vary. Refer to the Module Info for more details.
 
 Copyright Altertech Group and other contributors, https://www.altertech.com/
```

### Comparing `eva4-controller-py-0.0.9/PKG-INFO` & `eva4-controller-py-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: eva4-controller-py
-Version: 0.0.9
+Version: 0.1.0
 Summary: EVA ICS v4 Python macros controller service
-Home-page: https://github.com/alttch/eva4
+Home-page: https://github.com/eva-ics/eva4
 Author: Bohemia Automation / Altertech
 Author-email: div@altertech.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Communications
```

### Comparing `eva4-controller-py-0.0.9/eva4_controller_py/__init__.py` & `eva4-controller-py-0.1.0/eva4_controller_py/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-__version__ = '0.0.9'
+__version__ = '0.1.0'
 
 from evaics.sdk import Service, Controller, Action, no_rpc_method, ServiceInfo
 from evaics.sdk import OID
 
 from timeouter import Timer
 
-import msgpack
-
 from types import SimpleNamespace
 from pathlib import Path
 from concurrent.futures import ThreadPoolExecutor
 
 from . import macro_api
 
+import sys
 import os
 import threading
 import traceback
 
 dir_me = Path(__file__).absolute().parents[0].as_posix()
 
 _d = SimpleNamespace(dir_xcpy=None,
@@ -155,17 +154,23 @@
     service = Service()
     _d.timeout = service.timeout['default']
     config = service.get_config()
     poll_delay = config.get('poll_delay', 0.1)
     pool_size = config.get('pool_size', 50)
     _d.pool = ThreadPoolExecutor(max_workers=pool_size)
     eva_dir = service.initial['core']['path']
+    sys.path.insert(0, f'{eva_dir}/venv/bin')
     macro_api.eva_dir = eva_dir
-    dir_xcpy = f'{eva_dir}/runtime/xc/py'
-    Path(dir_xcpy).mkdir(parents=True, exist_ok=True)
+    macro_api.svc_data_dir = service.data_path
+    macro_dir = config.get('macro_dir', 'xc/py')
+    dir_xcpy = f'{eva_dir}/runtime/{macro_dir}'
+    try:
+        Path(dir_xcpy).mkdir(parents=True, exist_ok=True)
+    except:
+        pass
     _d.dir_xcpy = dir_xcpy
     _d.common_py = f'{dir_xcpy}/common.py'
     service.init_bus()
     service.drop_privileges()
     _d.service = service
     _d.controller = Controller(service.bus)
     _d.logger = service.init_logs()
@@ -176,16 +181,15 @@
     _d.env.update(config.get('cvars', {}))
     _d.env.update(macro_api.api_globals)
     macro_api.service = service
     macro_api.locker_svc = config.get('locker_svc')
     macro_api.mailer_svc = config.get('mailer_svc')
     service.on_rpc_call = handle_rpc
     service.init_rpc(info)
-    _d.logger.info(f'Python macros controller started ({service.id}), '
-                   f'dir: {_d.dir_xcpy}, pool_size: {pool_size}')
+    _d.logger.info(f'dir: {_d.dir_xcpy}, pool_size: {pool_size}')
     service.register_signals()
     service.mark_ready()
     service.wait_core()
     _d.pool.submit(safe_run_system_macro, 'autoexec')
-    service.block()
+    service.block(prepare=False)
     _d.pool.submit(safe_run_system_macro, 'shutdown')
     service.mark_terminating()
```

### Comparing `eva4-controller-py-0.0.9/eva4_controller_py/macro_api.py` & `eva4-controller-py-0.1.0/eva4_controller_py/macro_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-import elbus
+import busrt
 import logging
 import sys
 import os
 import glob
 import time
-import msgpack
 try:
     import rapidjson as json
 except:
     import json
 import threading
 import datetime
 
@@ -18,57 +17,95 @@
 from evaics.exceptions import ResourceAlreadyExists
 from evaics.exceptions import ResourceNotFound
 from evaics.exceptions import ResourceBusy
 from evaics.exceptions import AccessDenied
 from evaics.exceptions import InvalidParameter
 from evaics.exceptions import MethodNotImplemented
 
-from evaics.sdk import LocalProxy, rpc_e2e
+from evaics.sdk import LocalProxy, rpc_e2e, pack, unpack
 
 from evaics.tools import dict_from_str
 
 _shared = {}
 _shared_lock = threading.RLock()
 
 eva_dir = None
+svc_data_dir = None
 service = None
 
 locker_svc = None
 mailer_svc = None
 
 g = LocalProxy()
 
 
 def parse_action_payload(payload):
     payload['uuid'] = str(UUID(bytes=payload['uuid']))
     return payload
 
 
+def get_service():
+    """
+    Get the service object for the direct access
+
+    e.g. service.bus: direct access to BUS/RT
+    service.rpc: direct access to BUS/RT RPC
+
+    Returns:
+        the service object
+    """
+    return service
+
+
+def get_system_name():
+    """
+    Get the system name
+
+    Returns:
+        system name
+    """
+    return service.system_name
+
+
 def rpc_call(method=None, _target='eva.core', _timeout=None, **kwargs):
+    """
+    Performs a bus RPC call
+
+    The method parameters are specified in kwargs
+
+    Args:
+        method: method
+
+    Optional:
+        _target: target service (default: eva.core)
+        _timeout: call timeout
+
+    Returns:
+        the bus call result
+    """
     try:
         result = service.rpc.call(
-            _target,
-            elbus.rpc.Request(
+            _target, busrt.rpc.Request(
                 method,
-                msgpack.dumps(kwargs) if kwargs else None)).wait_completed(
+                pack(kwargs) if kwargs else None)).wait_completed(
                     _timeout if _timeout is not None else g.get('t').get(
                         check=True)).get_payload()
-    except elbus.rpc.RpcException as e:
+    except busrt.rpc.RpcException as e:
         raise rpc_e2e(e)
     if result:
-        return msgpack.loads(result, raw=False)
+        return unpack(result)
     else:
         return True
 
 
 def shared(name, default=None):
     """
-    get value of the shared variable
+    Gets value of the shared variable
 
-    Get value of the variable, shared between controller macros
+    Gets value of the variable, shared between controller macros
 
     Args:
         name: variable name
 
     Optional:
         default: value if variable doesn't exist
 
@@ -77,40 +114,40 @@
     """
     with _shared_lock:
         return _shared.get(name, default)
 
 
 def set_shared(name, value=None):
     """
-    set value of the shared variable
+    Sets value of the shared variable
 
-    Set value of the variable, shared between controller macros
+    Sets value of the variable, shared between controller macros
 
     Args:
         name: variable name
 
     Optional:
-        value: value to set. If empty, varible is deleted
+        value: value to set. If empty, the variable is deleted
     """
     with _shared_lock:
         if value is None:
             try:
                 del _shared[name]
             except KeyError:
                 pass
         else:
             _shared[name] = value
         return True
 
 
 def increment_shared(name):
     """
-    increment value of the shared variable
+    Increments value of the shared variable
 
-    Increment value of the variable, shared between controller macros. Initial
+    Increments value of the variable, shared between controller macros. Initial
     value must be number
 
     Args:
         name: variable name
     """
     with _shared_lock:
         v = shared(name)
@@ -120,18 +157,18 @@
             v = int(v) + 1
         set_shared(name, v)
         return v
 
 
 def decrement_shared(name):
     """
-    decrement value of the shared variable
+    Decrements value of the shared variable
 
-    Decrement value of the variable, shared between controller macros. Initial
-    value must be number
+    Decrements value of the variable, shared between controller macros.
+    Initial value must be number
 
     Args:
         name: variable name
     """
     with _shared_lock:
         v = shared(name)
         if v is None:
@@ -140,15 +177,15 @@
             v = int(v) - 1
         set_shared(name, v)
         return v
 
 
 def ping(host, timeout=1000, count=1):
     """
-    ping remote host
+    Pings a remote host
 
     Requires fping tool
 
     Args:
         host: host name or IP to ping
         timeout: ping timeout in milliseconds (default: 1000)
         count: number of packets to send (default: 1)
@@ -158,25 +195,25 @@
     """
     return os.system(
         f'fping -t {timeout} -c {count} {host} > /dev/null 2>&1') == 0
 
 
 def _exit(code=0):
     """
-    finish macro execution
+    Finishes macro execution
 
     Args:
         code: macro exit code (default: 0, no errors)
     """
     sys.exit(code)
 
 
 def lock(lock_id, expires, timeout=None):
     """
-    acquire a lock
+    Acquires a lock
 
     Requires locker svc to be set in the controller config
 
     Args:
         lock_id: lock id
         expires: time after which the lock is automatically unlocked (sec)
 
@@ -196,15 +233,15 @@
                  expires=expires,
                  timeout=timeout,
                  _timeout=timeout)
 
 
 def unlock(lock_id):
     """
-    release lock
+    Releases a lock
 
     Releases the previously acquired lock
 
     Args:
         lock_id: lock id
 
     Raises:
@@ -214,15 +251,15 @@
         raise MethodNotImplemented('no locker svc defined')
     else:
         rpc_call('unlock', _target=locker_svc, i=lock_id)
 
 
 def mail(subject=None, text=None, rcp=None):
     """
-    send email message
+    Sends email message
 
     Requires mailer svc to be set in the controller config
 
     Optional:
         subject: email subject
         text: email text
         rcp: recipient or array of the recipients
@@ -238,15 +275,15 @@
                  subject=subject,
                  text=text,
                  rcp=rcp)
 
 
 def state(oid):
     """
-    get item state
+    Gets item state
 
     Args:
         oid: item OID or mask
 
     Returns:
         item status/value dict or list for mask
 
@@ -266,15 +303,15 @@
         raise ResourceNotFound
     else:
         return result[0]
 
 
 def status(oid):
     """
-    get item status
+    Gets item status
 
     Args:
         oid: item OID
 
     Returns:
         item status (integer)
 
@@ -282,15 +319,15 @@
         ResourceNotFound: item not found
     """
     return state(oid)['status']
 
 
 def value(oid, default=None):
     """
-    get item value
+    Gets item value
 
     Args:
         i: item OID
 
     Optional:
         default: value if null (default is empty string)
 
@@ -305,47 +342,47 @@
         return default
     else:
         return value
 
 
 def is_expired(oid):
     """
-    is lvar (timer) or item state expired/error
+    Checks is lvar (timer) or item state expired/error
 
     Args:
         oid: item OID
 
     Returns:
-        True, if the timer has been expired
+        True if the timer has been expired
 
     Raises:
-        ResourceNotFound
+        ResourceNotFound: item not found
     """
     return state(oid)['status'] == -1
 
 
 def is_busy(oid):
     """
-    is the unit busy
+    Checks is the unit busy
 
     Args:
         oid: unit OID
 
     Returns:
-        True, if unit is busy (action is executed)
+        True if unit is busy (action is executed)
 
     Raises:
         ResourceNotFound: unit not found
     """
     return state(oid)['act'] > 0
 
 
 def _set(oid, status=None, value=None):
     """
-    set lvar value
+    Sets lvar value
 
     Args:
         oid: lvar OID
 
     Optional:
         value: lvar value (if not specified, lvar is set to null)
 
@@ -359,15 +396,15 @@
     if value is not None:
         params['value'] = None if value == 'null' else value
     return rpc_call('lvar.set', **params)
 
 
 def reset(oid):
     """
-    reset lvar status
+    Resets lvar status
 
     Set lvar status to 1 or start lvar timer
 
     Args:
         oid: lvar OID
 
     Raises:
@@ -375,15 +412,15 @@
         ResourceNotFound: lvar not found
     """
     return rpc_call('lvar.reset', i=str(oid))
 
 
 def clear(oid):
     """
-    clear lvar status
+    Clears lvar status
 
     Set lvar status to 0 or stop timer lvar (set timer status to 0)
 
     Args:
         oid: lvar OID
 
     Raises:
@@ -391,15 +428,15 @@
         ResourceNotFound: lvar not found
     """
     return rpc_call('lvar.clear', i=str(oid))
 
 
 def toggle(oid):
     """
-    toggle lvar status
+    Toggles lvar status
 
     Change lvar status to opposite boolean (0->1, 1->0)
 
     Args:
         oid: lvar OID
 
     Raises:
@@ -407,79 +444,78 @@
         ResourceNotFound: lvar not found
     """
     return rpc_call('lvar.toggle', i=str(oid))
 
 
 def increment(oid):
     """
-    Increment lvar value
+    Increments lvar value
 
     Args:
         lvar_id: lvar OID
 
     Raises:
         FunctionFailed: lvar value increment error
         ResourceNotFound: lvar not found
     """
     return rpc_call('lvar.incr', i=str(oid))
 
 
 def decrement(oid):
     """
-    Decrement lvar value
+    Decrements lvar value
 
     Args:
         oid: lvar OID
 
     Raises:
         FunctionFailed: lvar value decrement error
         ResourceNotFound: lvar not found
     """
     return rpc_call('lvar.decr', i=str(oid))
 
 
-def action(oid, status, value=None, wait=None, priority=None):
+def action(oid, value, status=None, wait=None, priority=None):
     """
-    unit control action
+    Executes unit control action
     
     Args:
         oid: unit OID
-        status: desired unit status
+        value: desired unit value
 
     Optional:
-        value: desired unit value
         wait: wait for the completion for the specified number of seconds
         priority: queue priority (default is 100, lower is better)
 
     Returns:
         Serialized action object (dict)
 
     Raises:
         FunctionFailed: action failed to be executed
         ResourceNotFound: unit not found
 
     @var_out exitcode Exit code
     @var_out status Action status
     """
-    params = {
-        'i': str(oid),
-        'status': status,
-    }
-    if value is not None:
-        params['value'] = None if value == 'null' else value
+    params = {'value': value}
+    if status is not None:
+        logging.warning(
+            'status field in actions is ignored and deprecated. remove the field from API call payloads'
+        )
+    payload = {'i': str(oid), 'params': params}
     if wait is not None:
-        params['wait'] = wait
+        payload['wait'] = wait
     if priority is not None:
-        params['priority'] = priority
-    return parse_action_payload(rpc_call('action', **params))
+        payload['priority'] = priority
+    return parse_action_payload(rpc_call('action', **payload))
 
 
 def action_toggle(oid, wait=None, priority=None):
     """
-    toggle unit status
+    Executes an action to toggle unit status
     
     Creates a unit control action to toggle its status (1->0, 0->1)
 
     Args:
         oid: unit OID
 
     Optional:
@@ -499,15 +535,15 @@
     """
     return parse_action_payload(
         rpc_call('action.toggle', i=str(oid), wait=wait, priority=priority))
 
 
 def result(oid=None, uuid=None, sq=None, limit=None):
     """
-    get action status
+    Gets action status
 
     Checks the result of the action by its UUID or returns the actions for
     the specified unit
 
     Args:
         oid: unit OID or
         uuid: action uuid
@@ -534,99 +570,99 @@
     elif uuid is not None:
         return parse_action_payload(
             rpc_call('action.result', u=UUID(str(uuid)).bytes))
     else:
         raise InvalidParameter('either oid or uuid must be specified')
 
 
-def action_start(oid, value=None, wait=None, priority=None):
+def action_start(oid, wait=None, priority=None):
     """
-    start a unit
+    Executes an action to a unit
     
-    Create unit control action to set its status to 1
+    Creates unit control action to set its value to 1
 
     Args:
         oid: unit OID
 
     Optional:
-        value: desired unit value
         wait: wait for the completion for the specified number of seconds
         priority: queue priority (default is 100, lower is better)
 
     Returns:
         Serialized action object (dict)
 
     Raises:
         ResourceNotFound: unit not found
 
     @var_out exitcode Exit code
     @var_out status Action status
     """
-    return action(oid, status=1, value=value, wait=wait, priority=priority)
+    return action(oid, value=1, wait=wait, priority=priority)
 
 
-def action_stop(oid, value=None, wait=None, priority=None):
+def action_stop(oid, wait=None, priority=None):
     """
-    stop a unit
+    Executes an action to stop a unit
     
-    Create unit control action to set its status to 0
+    Creates unit control action to set its value to 0
 
     Args:
         oid: unit OID
 
     Optional:
-        value: desired unit value
         wait: wait for the completion for the specified number of seconds
         priority: queue priority (default is 100, lower is better)
 
     Returns:
         Serialized action object (dict)
 
     Raises:
         ResourceNotFound: unit not found
 
     @var_out exitcode Exit code
     @var_out status Action status
     """
-    return action(oid, status=0, value=value, wait=wait, priority=priority)
+    return action(oid, value=0, wait=wait, priority=priority)
 
 
 def terminate(uuid):
     """
-    terminate action execution
+    Terminates action execution
     
     Terminates or cancel the action if it is still queued
     
     Args:
         uuid: action uuid
         
     Raises:
         ResourceNotFound: if action is not found or action is already finished
     """
     return rpc_call('action.terminate', u=UUID(str(uuid)).bytes)
 
 
 def kill(oid):
     """
-    kill unit actions
+    Kills unit actions
 
     Terminates the current action (if possible) and cancels all pending
 
     Args:
         oid: unit OID
 
     Raises:
         ResourceNotFound: unit not found
     """
     return rpc_call('action.kill', i=str(oid))
 
 
 def run(_oid, *args, _wait=None, _priority=None, **kwargs):
     """
-    execute another lmacro
+    Executes another lmacro
+
+    Args and kwargs are passed to the target lmacro as-is, except listed below.
 
     Args:
         _oid: lmacro OID
 
     Optional:
         _wait: wait for the completion for the specified number of seconds
         _priority: queue priority (default is 100, lower is better)
@@ -637,29 +673,29 @@
     Raises:
         ResourceNotFound: macro not found
 
     @var_out exitcode Exit code
     @var_out status Action status
     @var_out out Macro "out" variable
     """
-    params = {'i': str(_oid)}
+    payload = {'i': str(_oid)}
     if _wait is not None:
-        params['wait'] = _wait
+        payload['wait'] = _wait
     if _priority is not None:
-        params['priority'] = _priority
+        payload['priority'] = _priority
     if args:
-        params['args'] = args
+        payload.setdefault('params', {})['args'] = args
     if kwargs:
-        params['kwargs'] = kwargs
-    return parse_action_payload(rpc_call('run', **params))
+        payload.setdefault('params', {})['kwargs'] = kwargs
+    return parse_action_payload(rpc_call('run', **payload))
 
 
 def date():
     """
-    get current date/time
+    Gets current date/time
 
     Returns:
         Serialized date/time object (dict)
 
     @var_out year
     @var_out month
     @var_out day
@@ -680,15 +716,15 @@
         'second': t.second,
         'timestamp': t.timestamp()
     }
 
 
 def ls(mask, recursive=False):
     """
-    list files in directory
+    Lists files in directory
 
     If recursive is true, the pattern "**" will match any files and zero or
     more directories and subdirectories.
 
     Args:
         mask: path and mask (e.g. /opt/data/\*.jpg)
         recursive: if True, perform a recursive search
@@ -710,15 +746,15 @@
             }
         })
     return l
 
 
 def sha256sum(value, hexdigest=True):
     """
-    calculate SHA256 sum
+    Calculates SHA256 sum
 
     Args:
         value: value to calculate
         hexdigest: return binary digest or hex (True, default)
 
     Returns:
         sha256 digest
@@ -729,24 +765,26 @@
     s = sha256()
     s.update(value)
     return s.hexdigest() if hexdigest else s.digest()
 
 
 def get_directory(tp):
     """
-    Get path to EVA ICS directory
+    Gets path to EVA ICS directory
 
     Args:
-        tp: directory type: eva, runtime, or xc
+        tp: directory type: eva, runtime, svc_data, venv or xc
     Raises:
         LookupError: if the directory type is invalid
     """
     if tp == 'eva':
         return eva_dir
-    elif tp not in ['runtime', 'xc']:
+    elif tp == 'svc_data':
+        return svc_data_dir
+    elif tp not in ['runtime', 'xc', 'venv']:
         raise LookupError
     else:
         return f'{eva_dir}/{tp}'
 
 
 def _system(*args, **kwargs):
     code = os.system(*args, **kwargs)
@@ -764,15 +802,15 @@
     'ResourceNotFound': ResourceNotFound,
     'ResourceAlreadyExists': ResourceBusy,
     'AccessDenied': AccessDenied,
     'InvalidParameter': InvalidParameter,
     'json': json,
     'os': os,
     'sys': sys,
-    'elbus': elbus,
+    'bus': busrt,
     'on': 1,
     'off': 0,
     'yes': True,
     'no': False,
     'get_directory': get_directory,
     'shared': shared,
     'set_shared': set_shared,
@@ -803,14 +841,16 @@
     'increment': increment,
     'decrement': decrement,
     'action': action,
     'action_toggle': action_toggle,
     'result': result,
     'start': action_start,
     'stop': action_stop,
+    'service': get_service,
+    'system_name': get_system_name,
     'terminate': terminate,
     'kill': kill,
     'run': run,
     'system': _system,
     'ping': ping,
     'time': time.time,
     'mail': mail,
```

### Comparing `eva4-controller-py-0.0.9/eva4_controller_py/macro_builtins.py` & `eva4-controller-py-0.1.0/eva4_controller_py/macro_builtins.py`

 * *Files identical despite different names*

### Comparing `eva4-controller-py-0.0.9/eva4_controller_py.egg-info/PKG-INFO` & `eva4-controller-py-0.1.0/eva4_controller_py.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: eva4-controller-py
-Version: 0.0.9
+Version: 0.1.0
 Summary: EVA ICS v4 Python macros controller service
-Home-page: https://github.com/alttch/eva4
+Home-page: https://github.com/eva-ics/eva4
 Author: Bohemia Automation / Altertech
 Author-email: div@altertech.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Communications
```

### Comparing `eva4-controller-py-0.0.9/setup.py` & `eva4-controller-py-0.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-__version__ = '0.0.9'
+__version__ = '0.1.0'
 
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
-setuptools.setup(name='eva4-controller-py',
-                 version=__version__,
-                 author='Bohemia Automation / Altertech',
-                 author_email='div@altertech.com',
-                 description='EVA ICS v4 Python macros controller service',
-                 long_description=long_description,
-                 long_description_content_type='text/markdown',
-                 url='https://github.com/alttch/eva4',
-                 packages=setuptools.find_packages(),
-                 license='Apache License 2.0',
-                 install_requires=[
-                     'elbus>=0.0.14', 'evaics>=0.0.16', 'msgpack>=1.0.3',
-                     'timeouter>=0.0.15'
-                 ],
-                 classifiers=('Programming Language :: Python :: 3',
-                              'License :: OSI Approved :: MIT License',
-                              'Topic :: Communications'),
-                 scripts=['bin/eva4-svc-controller-py'])
+setuptools.setup(
+    name='eva4-controller-py',
+    version=__version__,
+    author='Bohemia Automation / Altertech',
+    author_email='div@altertech.com',
+    description='EVA ICS v4 Python macros controller service',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    url='https://github.com/eva-ics/eva4',
+    packages=setuptools.find_packages(),
+    license='Apache License 2.0',
+    install_requires=['busrt>=0.1.0', 'evaics>=0.2.9', 'timeouter>=0.0.15'],
+    classifiers=('Programming Language :: Python :: 3',
+                 'License :: OSI Approved :: MIT License',
+                 'Topic :: Communications'),
+    scripts=['bin/eva4-svc-controller-py'])
```

