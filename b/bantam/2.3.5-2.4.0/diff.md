# Comparing `tmp/bantam-2.3.5.tar.gz` & `tmp/bantam-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bantam-2.3.5.tar", last modified: Sun Jun 11 03:59:44 2023, max compression
+gzip compressed data, was "bantam-2.4.0.tar", last modified: Sat Jun 17 16:42:43 2023, max compression
```

## Comparing `bantam-2.3.5.tar` & `bantam-2.4.0.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-11 03:59:44.679059 bantam-2.3.5/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-11 03:59:44.679059 bantam-2.3.5/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.3.5/README
--rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-06-11 03:58:58.000000 bantam-2.3.5/requirements.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-06-11 03:59:44.679059 bantam-2.3.5/setup.cfg
--rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-06-11 03:59:41.000000 bantam-2.3.5/setup.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-11 03:59:44.679059 bantam-2.3.5/src/
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-11 03:59:44.679059 bantam-2.3.5/src/bantam/
--rw-rw-r--   0 pi        (1000) pi        (1000)     4613 2023-06-11 03:31:41.000000 bantam-2.3.5/src/bantam/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    10548 2023-06-10 22:52:38.000000 bantam-2.3.5/src/bantam/api.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-11 03:59:44.679059 bantam-2.3.5/src/bantam/autogen/
--rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.3.5/src/bantam/autogen/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.3.5/src/bantam/autogen/main.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    20981 2023-06-10 22:33:04.000000 bantam-2.3.5/src/bantam/client.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     5520 2023-06-04 02:57:43.000000 bantam-2.3.5/src/bantam/conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4684 2023-06-04 23:41:07.000000 bantam-2.3.5/src/bantam/decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    49446 2023-06-11 03:23:34.000000 bantam-2.3.5/src/bantam/http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    22133 2023-06-04 14:44:14.000000 bantam-2.3.5/src/bantam/js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    20369 2023-06-04 03:38:29.000000 bantam-2.3.5/src/bantam/js_async.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    13103 2023-06-03 15:15:17.000000 bantam-2.3.5/src/bantam/pythonclient.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-11 03:59:44.679059 bantam-2.3.5/src/bantam.egg-info/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-11 03:59:44.000000 bantam-2.3.5/src/bantam.egg-info/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      699 2023-06-11 03:59:44.000000 bantam-2.3.5/src/bantam.egg-info/SOURCES.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-11 03:59:44.000000 bantam-2.3.5/src/bantam.egg-info/dependency_links.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-06-11 03:59:44.000000 bantam-2.3.5/src/bantam.egg-info/entry_points.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-06-11 03:59:44.000000 bantam-2.3.5/src/bantam.egg-info/requires.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-06-11 03:59:44.000000 bantam-2.3.5/src/bantam.egg-info/top_level.txt
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-11 03:59:44.679059 bantam-2.3.5/test/
--rw-rw-r--   0 pi        (1000) pi        (1000)     4785 2023-06-10 04:24:24.000000 bantam-2.3.5/test/test_client_get.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4634 2023-06-10 04:24:36.000000 bantam-2.3.5/test/test_client_post.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     6038 2023-06-11 01:57:09.000000 bantam-2.3.5/test/test_client_post_inherited_apis.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.3.5/test/test_conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.3.5/test/test_decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.3.5/test/test_http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3001 2023-06-11 03:15:10.000000 bantam-2.3.5/test/test_js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     2856 2023-06-10 16:58:56.000000 bantam-2.3.5/test/test_js_async.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-17 16:42:43.850515 bantam-2.4.0/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-17 16:42:43.850515 bantam-2.4.0/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.4.0/README
+-rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-06-11 03:58:58.000000 bantam-2.4.0/requirements.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-06-17 16:42:43.850515 bantam-2.4.0/setup.cfg
+-rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-06-17 16:41:46.000000 bantam-2.4.0/setup.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-17 16:42:43.846516 bantam-2.4.0/src/
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-17 16:42:43.846516 bantam-2.4.0/src/bantam/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4616 2023-06-11 16:48:25.000000 bantam-2.4.0/src/bantam/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    11963 2023-06-17 16:30:44.000000 bantam-2.4.0/src/bantam/api.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-17 16:42:43.846516 bantam-2.4.0/src/bantam/autogen/
+-rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.4.0/src/bantam/autogen/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.4.0/src/bantam/autogen/main.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    21101 2023-06-17 16:17:43.000000 bantam-2.4.0/src/bantam/client.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5705 2023-06-17 16:33:30.000000 bantam-2.4.0/src/bantam/conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4684 2023-06-04 23:41:07.000000 bantam-2.4.0/src/bantam/decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    49748 2023-06-17 16:36:40.000000 bantam-2.4.0/src/bantam/http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    22114 2023-06-17 16:10:55.000000 bantam-2.4.0/src/bantam/js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    20369 2023-06-04 03:38:29.000000 bantam-2.4.0/src/bantam/js_async.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-17 16:42:43.846516 bantam-2.4.0/src/bantam.egg-info/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-17 16:42:43.000000 bantam-2.4.0/src/bantam.egg-info/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      672 2023-06-17 16:42:43.000000 bantam-2.4.0/src/bantam.egg-info/SOURCES.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-17 16:42:43.000000 bantam-2.4.0/src/bantam.egg-info/dependency_links.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-06-17 16:42:43.000000 bantam-2.4.0/src/bantam.egg-info/entry_points.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-06-17 16:42:43.000000 bantam-2.4.0/src/bantam.egg-info/requires.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-06-17 16:42:43.000000 bantam-2.4.0/src/bantam.egg-info/top_level.txt
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-17 16:42:43.850515 bantam-2.4.0/test/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4821 2023-06-17 16:39:40.000000 bantam-2.4.0/test/test_client_get.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4670 2023-06-17 15:47:27.000000 bantam-2.4.0/test/test_client_post.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     6038 2023-06-11 01:57:09.000000 bantam-2.4.0/test/test_client_post_inherited_apis.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.4.0/test/test_conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.4.0/test/test_decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.4.0/test/test_http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3001 2023-06-11 03:15:10.000000 bantam-2.4.0/test/test_js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     2856 2023-06-10 16:58:56.000000 bantam-2.4.0/test/test_js_async.py
```

### Comparing `bantam-2.3.5/PKG-INFO` & `bantam-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.3.5
+Version: 2.4.0
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.3.5
+Download-URL: https://github.com/bantam/dist/2.4.0
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.3.5/setup.py` & `bantam-2.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import setuptools
 
-VERSION = "2.3.5"
+VERSION = "2.4.0"
 
 setuptools.setup(
     name='bantam',
     author='John Rusnak',
     author_email='john.j.rusnak@att.net',
     version=VERSION,
     data_files=[('.', ['requirements.txt'])],
```

### Comparing `bantam-2.3.5/src/bantam/__init__.py` & `bantam-2.4.0/src/bantam/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,8 +98,8 @@
 
     def __init__(self, code: int, msg: str):
         super().__init__(msg)
         self._code = code
 
     @property
     def status_code(self):
-        return self._code
+        return self._codesud
```

### Comparing `bantam-2.3.5/src/bantam/api.py` & `bantam-2.4.0/src/bantam/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import inspect
+import typing
 from enum import Enum
-from typing import Callable, Awaitable, AsyncGenerator, Dict, List, Optional, Type
+from typing import Callable, Awaitable, AsyncGenerator, Dict, List, Optional, Type, TypeVar
 
 from aiohttp import ClientTimeout
 
 AsyncChunkIterator = Callable[[int], Awaitable[AsyncGenerator[None, bytes]]]
 AsyncLineIterator = AsyncGenerator[None, str]
 
 
@@ -30,26 +32,33 @@
         self._func = func
         self._real_func = func
         self._method = method
         self._timeout = timeout or ClientTimeout()
         if 'return' not in annotations:
             raise TypeError(f"No annotation for return type in {func}")
         self._arg_annotations = {name: typ for name, typ in annotations.items() if name != 'return'}
+        if not func.__name__.startswith('_'):
+            sig = inspect.signature(func)
+            for name in self._arg_annotations:
+                if sig.parameters[name].kind == inspect.Parameter.VAR_POSITIONAL:
+                    self._arg_annotations[name] = typing.Tuple[int, None]
+                elif sig.parameters[name].kind == inspect.Parameter.VAR_KEYWORD:
+                    self._arg_annotations[name] = typing.Dict[str, self._arg_annotations[name]]
         self._async_arg_annotations = {
             name: typ for name, typ in self._arg_annotations.items()
             if typ in (bytes, AsyncChunkIterator, AsyncLineIterator)
         }
         if len(self._async_arg_annotations) > 1:
             raise TypeError("At most one parameter can be and async iterator in a web_api request")
         self._return_type = annotations['return']
         self._has_streamed_response = False
-        if str(self._return_type).startswith('typing.AsyncIterator'):
+        if str(self._return_type).startswith('typing.AsyncIterator') or self._return_type == typing.AsyncIterator:
             self._return_type = self._return_type.__args__[0]
             self._has_streamed_response = True
-        elif str(self._return_type).startswith('typing.AsyncGenerator'):
+        elif str(self._return_type).startswith('typing.AsyncGenerator') or self._return_type == typing.AsyncGenerator:
             self._return_type = self._return_type.__args__[1]
             self._has_streamed_response = True
         self._content_type = content_type if not self.has_streamed_response else 'text/streamed; charset=x-user-defined'
         self._is_constructor = is_constructor
         if is_constructor:
             self._return_type = str
         self._uuid_param = uuid_param
@@ -137,14 +146,30 @@
     @property
     def has_streamed_response(self) -> bool:
         return self._has_streamed_response
 
     def __call__(self, *args, **kwargs):
         return self._func(*args, **kwargs)
 
+    def update_varargs(self, kwargs: Dict[str, typing.Any]) -> [Dict[str, typing.Any], typing.Tuple[typing.Any]]:
+        """
+        takes list of kwargs for the call and transforms as needed for any varargs  or varkwargs in call
+        """
+        sig = inspect.signature(self._func)
+        updated = kwargs
+        varargs = tuple()
+        for name, param in sig.parameters.items():
+            if param.kind == inspect.Parameter.VAR_KEYWORD:
+                del updated[name]
+                updated.update(**kwargs[name])
+            elif param.kind == inspect.Parameter.VAR_POSITIONAL:
+                varargs = kwargs[name]
+                del updated[name]
+        return updated, varargs
+
 
 class APIDoc:
     """
     Class for converting python docs to target language/protocol (javascript, ReST API, ...)
     """
 
     class Flavor(Enum):
@@ -257,7 +282,14 @@
             return f"dict of {root_type}"
         elif str(typ).startswith('typing.Dict') or str(typ).startswith('typing.Mapping'):
             key_type, value_type = str(typ).split('[')[1].replace(']', '').split(',')
             return f"Dictionary of key type {key_type} and value type {value_type}"
         else:
             # noinspection PyProtectedMember
             return typ.__name__ if hasattr(typ, '__name__') else typ._name if hasattr(typ, '_name') else str(typ)
+
+
+V = TypeVar('V')
+
+
+def raise_is_abstract(v: V = None) -> V:
+    raise NotImplemented(f"Call to abstract function")
```

### Comparing `bantam-2.3.5/src/bantam/autogen/main.py` & `bantam-2.4.0/src/bantam/autogen/main.py`

 * *Files identical despite different names*

### Comparing `bantam-2.3.5/src/bantam/client.py` & `bantam-2.4.0/src/bantam/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,17 +140,20 @@
         async def class_method(cls_, *args, **kwargs_):
             nonlocal api, end_point
             # noinspection PyBroadException
             try:
                 arg_spec = inspect.getfullargspec(api._func)
             except Exception:
                 arg_spec = inspect.getfullargspec(api._func.__func__)
-            kwargs_.update({
-                arg_spec.args[n + 1]: arg for n, arg in enumerate(args)
-            })
+            if arg_spec.varargs is None:
+                kwargs_.update({
+                    arg_spec.args[n + 1]: arg for n, arg in enumerate(args)
+                })
+            else:
+                kwargs_[arg_spec.varargs] = args
             # noinspection PyBroadException
             rest_method = api._func._bantam_web_api.method
             if rest_method.value == RestMethod.GET.value:
                 url_args = cls._generate_url_args(kwargs=kwargs_)
                 url = f"{base_url}{url_args}"
                 async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
                     async with session.get(url) as resp:
```

### Comparing `bantam-2.3.5/src/bantam/conversions.py` & `bantam-2.4.0/src/bantam/conversions.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,19 @@
             for k, v in json_data.items()
         }
     elif getattr(typ, '_name', None) in ('List', ):
         return [normalize_from_json(value, typ.__args__[0]) for index, value in enumerate(json_data)]
     elif getattr(typ, '_name', None) in ('Set', ):
         return {normalize_from_json(value, typ.__args__[0]) for index, value in enumerate(json_data)}
     elif getattr(typ, '_name', None) in ('Tuple', ):
-        return tuple(normalize_from_json(value, typ.__args__[index]) for index, value in enumerate(json_data))
+        if typ.__args__[-1] == type(None):  # var args
+            return tuple(normalize_from_json(value, typ.__args__[0]) for index, value in enumerate(json_data))
+        else:
+            return tuple(normalize_from_json(value, typ.__args__[index]) for index, value in enumerate(json_data))
+
     elif hasattr(typ, '__dataclass_fields__'):
         return typ(**{
             name: normalize_from_json(json_data[name], field.type)
             for name, field in typ.__dataclass_fields__.items()
         })
     else:
         raise TypeError(f"Unsupported typ for web api: '{typ}'")
```

### Comparing `bantam-2.3.5/src/bantam/decorators.py` & `bantam-2.4.0/src/bantam/decorators.py`

 * *Files identical despite different names*

### Comparing `bantam-2.3.5/src/bantam/http.py` & `bantam-2.4.0/src/bantam/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -381,19 +381,19 @@
         for module in modules:
             self.preprocess_module(module)
             if module not in sys.modules:
                 mod = importlib.import_module(module)
             else:
                 mod = sys.modules.get(module)
             for api in list(self.module_mapping_get.get(module, {}).values()):
-                if api.name in ['_expire']:
+                if api.name in ['_expire', '_create']:
                     continue
                 self._process_module_classes(mod, api)
             for api in self.module_mapping_post.get(module, {}).values():
-                if api.name in ['_expire']:
+                if api.name in ['_expire', '_create']:
                     continue
                 self._process_module_classes(mod, api)
         allowed_get_routes = {}
         for module in [m for m in modules if m in self.module_mapping_get]:
             allowed_get_routes.update(self.module_mapping_get[module])
         for route, api_get in allowed_get_routes.items():
             log.debug(f">>>>>>>>>> GET ROUTE {route}")
@@ -611,24 +611,23 @@
         if '__isabstractmethod__' in func.__dict__:
             return func
 
         async def invoke(app: WebApplication, request: Request):
 
             async def invoke_proper():
                 nonlocal preprocess, postprocess
-                print(f">>>>>>>>>>>>>> INVOKING {api.name}")
                 try:
                     preprocess = preprocess or app.preprocessor
                     try:
                         addl_args = (preprocess(request) or {}) if preprocess else {}
                     except Exception as e:
                         text = traceback.format_exc()
-                        resp = Response(status=400, text=f"Error in preprocessing request: {e}\n{text}")
-                        await resp.prepare(request)
-                        return resp
+                        resp_ = Response(status=400, text=f"Error in preprocessing request: {e}\n{text}")
+                        await resp_.prepare(request)
+                        return resp_
                     if method == RestMethod.GET:
                         # noinspection PyProtectedMember
                         response = await cls._invoke_get_api_wrapper(
                             api, content_type=content_type, request=request, **addl_args
                         )
                     elif method == RestMethod.POST:
                         # noinspection PyProtectedMember
@@ -638,30 +637,29 @@
                     else:
                         raise ValueError(f"Unknown method {method} in @web-api")
                     try:
                         postprocess = postprocess or app.postprocessor
                         postprocess(response) if postprocess else response
                     except Exception as e:
                         text = traceback.format_exc()
-                        resp = Response(status=400, text=f"Error in post-processing of response: {e}\n{text}")
-                        await resp.prepare(request)
-                        return resp
+                        resp_ = Response(status=400, text=f"Error in post-processing of response: {e}\n{text}")
+                        await resp_.prepare(request)
+                        return resp_
                     return response
                 except (CancelledError, ConnectionResetError, ClientConnectionError):
                     raise
                 except BaseException as e:
                     text = traceback.format_exc()
-                    resp = Response(status=500, reason=f"Server error: {e}",
-                                    body=f"Server error: {e}\n{text}", content_type="test/plain")
-                    await resp.prepare(request)
-                    return resp
+                    resp_ = Response(status=500, reason=f"Server error: {e}",
+                                     body=f"Server error: {e}\n{text}", content_type="test/plain")
+                    await resp_.prepare(request)
+                    return resp_
             resp_q = asynciomultiplexer.AsyncAdaptorQueue(1)
             await cls.MainThread.start(invoke_proper(), resp_q)
             resp = await resp_q.get()
-            print(f">>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>> {api.name} RESP WRITE DONE {resp}")
             if isinstance(resp, Exception):
                 raise
             return resp
 
         invoke.clazz = WebApplication._instance_methods_class_map.get(api) if is_instance_method else None
         if method == RestMethod.GET:
             # noinspection PyProtectedMember
@@ -715,26 +713,29 @@
                 if self_id is None:
                     raise ValueError(
                         "A self request parameter is needed. No instance provided for call to instance method")
                 instance = cls.ObjectRepo.instances.get(self_id)
                 if instance is None:
                     raise ValueError(f"No instance found for request with 'self' id of {self_id}")
                 del kwargs['self']
-                result = api(instance, **kwargs)
+                kwargs, varargs = api.update_varargs(kwargs)
+                result = api(instance, *varargs, **kwargs)
             elif api.is_class_method:
                 if isinstance(api.clazz, tuple):
                     module_name, class_name = api.clazz
                     api._clazz = getattr(sys.modules.get(module_name), class_name)
+                kwargs, varargs = api.update_varargs(kwargs)
                 if 'cls' not in kwargs:
-                    result = api(**kwargs, cls=api.clazz)
+                    result = api(api.clazz, *varargs, **kwargs)
                 else:
-                    result = api(**kwargs)
+                    result = api(*varargs, **kwargs)
             else:
+                kwargs, varargs = api.update_varargs(kwargs)
                 # call the underlying function:
-                result = api(**kwargs)
+                result = api(*varargs, **kwargs)
             if inspect.isasyncgen(result):
                 #################
                 #  streamed response through async generator:
                 #################
                 # underlying function has yielded a result rather than turning
                 # process the yielded value and allow execution to resume from yielding task
                 content_type = "text-streamed; charset=x-user-defined"
@@ -791,15 +792,15 @@
                                 content_type=content_type)
                 await resp.prepare(request)
                 return resp
         except TypeError as e:
             resp = Response(status=400, text=f"Improperly formatted query: {str(e)}\n{traceback.format_exc()}")
             await resp.prepare(request)
             return resp
-        except HTTPException as e:
+        except HTTPException:
             raise
         except Exception as e:
             resp = Response(status=500, text=f"Exception: {e}: \n{traceback.format_exc()}")
             await resp.prepare(request)
             return resp
         finally:
             # noinspection PyUnresolvedReferences,PyProtectedMember
@@ -893,25 +894,28 @@
                         self_id = json.loads(self_id)['uuid']
                         instance = cls.ObjectRepo.instances.get(self_id)
                         if instance is None:
                             raise ValueError(f"No instance id found for request {self_id}")
                     except Exception:
                         raise ValueError(f"Error in json representation of an instance: {self_id}")
                 del kwargs['self']
-                awaitable = api(instance, **kwargs)
+                kwargs, varargs = api.update_varargs(kwargs)
+                awaitable = api(instance, *varargs, **kwargs)
                 if api.expire_object:
                     del cls.ObjectRepo.instances[self_id]
             elif api.is_class_method:
 
                 if isinstance(api.clazz, tuple):
                     module_name, class_name = api.clazz
                     api._clazz = getattr(sys.modules.get(module_name), class_name)
-                awaitable = api(**kwargs, cls=api.clazz)
+                kwargs, varargs = api.update_varargs(kwargs)
+                awaitable = api(api.clazz, *varargs, **kwargs)
             else:
-                awaitable = api(**kwargs)
+                kwargs, varargs = api.update_varargs(kwargs)
+                awaitable = api(*varags, **kwargs)
             if inspect.isasyncgen(awaitable):
                 #################
                 #  streamed response through async generator:
                 #################
                 # underlying function has yielded a result rather than turning
                 # process the yielded value and allow execution to resume from yielding task
                 async_q = asyncio.Queue()
```

### Comparing `bantam-2.3.5/src/bantam/js.py` & `bantam-2.4.0/src/bantam/js.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,19 +258,18 @@
         lines = [line for line in docs.splitlines() if not line.strip().startswith(':return')]
         docs = '\n'.join(lines) + '\n'
         out.write(docs.encode(cls.ENCODING))
 
     @classmethod
     def _generate_request(cls, out: IO, route: str, api: API, tab: str):
         func = api._func
-        arg_count = func.__code__.co_argcount
-        if 'self' in func.__code__.co_varnames or 'cls' in func.__code__.co_varnames\
-                or 'this' in func.__code__.co_varnames:
+        sig = inspect.signature(func)
+        arg_count = len(sig.parameters)
+        if 'self' in sig.parameters or 'cls' in sig.parameters or 'this' in sig.parameters:
             arg_count -= 1
-
         if not api.name.startswith('_') and arg_count != len(api.arg_annotations):
             raise Exception(f"Not all arguments of '{api.qualname}' have type hints.  This is required for web_api")
         if api.has_streamed_response is True:
             callback = 'onreceive'
             state = 3
             api._content_type = 'text/streamed; charset=x-user-defined'
         else:
```

### Comparing `bantam-2.3.5/src/bantam/js_async.py` & `bantam-2.4.0/src/bantam/js_async.py`

 * *Files identical despite different names*

### Comparing `bantam-2.3.5/src/bantam.egg-info/PKG-INFO` & `bantam-2.4.0/src/bantam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.3.5
+Version: 2.4.0
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.3.5
+Download-URL: https://github.com/bantam/dist/2.4.0
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.3.5/src/bantam.egg-info/SOURCES.txt` & `bantam-2.4.0/src/bantam.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 src/bantam/api.py
 src/bantam/client.py
 src/bantam/conversions.py
 src/bantam/decorators.py
 src/bantam/http.py
 src/bantam/js.py
 src/bantam/js_async.py
-src/bantam/pythonclient.py
 src/bantam.egg-info/PKG-INFO
 src/bantam.egg-info/SOURCES.txt
 src/bantam.egg-info/dependency_links.txt
 src/bantam.egg-info/entry_points.txt
 src/bantam.egg-info/requires.txt
 src/bantam.egg-info/top_level.txt
 src/bantam/autogen/__init__.py
```

### Comparing `bantam-2.3.5/test/test_client_get.py` & `bantam-2.4.0/test/test_client_get.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
     task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_get']))
     try:
         await asyncio.sleep(1)
         end_point = f'http://localhost:{PORT}/'
         client_mapping = RestAPIExampleAsyncInterface.ClientEndpointMapping()
         Client = client_mapping[end_point]
-        response = await Client.api_get_basic(42, True, 992.123)
+        response = await Client.api_get_basic(1, 2, 3, 4, 5, param1=42, param2=True, param3=992.123)
         assert response == f"Response to test_api_basic 1.0 2"
     finally:
         task.cancel()
         with suppress(CancelledError):
             await task
```

### Comparing `bantam-2.3.5/test/test_client_post.py` & `bantam-2.4.0/test/test_client_post.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 async def test_client_class_method(tmpdir):
     app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
     task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_post']))
     try:
         await asyncio.sleep(1)
         client = RestAPIExampleAsyncPostInterface.ClientEndpointMapping()
         client = client[f'http://localhost:{PORT}/']
-        response = await client.api_post_basic(42, True, 992.123)
+        response = await client.api_post_basic(1, 2, 4, 5, 6, param1=42, param2=True, param3=992.123)
         assert response == f"Response to test_api_basic 1.0 2"
     finally:
         task.cancel()
         with suppress(CancelledError):
             await task
```

### Comparing `bantam-2.3.5/test/test_client_post_inherited_apis.py` & `bantam-2.4.0/test/test_client_post_inherited_apis.py`

 * *Files identical despite different names*

### Comparing `bantam-2.3.5/test/test_conversions.py` & `bantam-2.4.0/test/test_conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.3.5/test/test_decorators.py` & `bantam-2.4.0/test/test_decorators.py`

 * *Files identical despite different names*

### Comparing `bantam-2.3.5/test/test_js.py` & `bantam-2.4.0/test/test_js.py`

 * *Files identical despite different names*

### Comparing `bantam-2.3.5/test/test_js_async.py` & `bantam-2.4.0/test/test_js_async.py`

 * *Files identical despite different names*

