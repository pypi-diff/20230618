# Comparing `tmp/pydantic_resolve-1.1.1.tar.gz` & `tmp/pydantic_resolve-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_resolve-1.1.1.tar", max compression
+gzip compressed data, was "pydantic_resolve-1.2.0.tar", max compression
```

## Comparing `pydantic_resolve-1.1.1.tar` & `pydantic_resolve-1.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.1.1/LICENSE
--rw-r--r--   0        0        0      550 2023-06-16 10:18:24.373879 pydantic_resolve-1.1.1/pydantic_resolve/__init__.py
--rw-r--r--   0        0        0       19 2023-04-05 08:27:57.212146 pydantic_resolve-1.1.1/pydantic_resolve/constant.py
--rw-r--r--   0        0        0     1990 2023-06-16 21:31:45.713490 pydantic_resolve-1.1.1/pydantic_resolve/core.py
--rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.1.1/pydantic_resolve/exceptions.py
--rw-r--r--   0        0        0     4620 2023-06-16 21:32:01.947620 pydantic_resolve-1.1.1/pydantic_resolve/resolver.py
--rw-r--r--   0        0        0     2833 2023-06-16 23:09:49.647683 pydantic_resolve-1.1.1/pydantic_resolve/util.py
--rw-r--r--   0        0        0      814 2023-06-16 23:13:04.858829 pydantic_resolve-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     5622 2023-06-16 21:48:45.117807 pydantic_resolve-1.1.1/README.md
--rw-r--r--   0        0        0     6283 1970-01-01 00:00:00.000000 pydantic_resolve-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.2.0/LICENSE
+-rw-r--r--   0        0        0      550 2023-06-16 10:18:24.373879 pydantic_resolve-1.2.0/pydantic_resolve/__init__.py
+-rw-r--r--   0        0        0       42 2023-06-18 14:32:47.738157 pydantic_resolve-1.2.0/pydantic_resolve/constant.py
+-rw-r--r--   0        0        0     2217 2023-06-18 14:39:54.866965 pydantic_resolve-1.2.0/pydantic_resolve/core.py
+-rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.2.0/pydantic_resolve/exceptions.py
+-rw-r--r--   0        0        0     5140 2023-06-18 15:07:09.605671 pydantic_resolve-1.2.0/pydantic_resolve/resolver.py
+-rw-r--r--   0        0        0     3898 2023-06-18 01:11:55.489541 pydantic_resolve-1.2.0/pydantic_resolve/util.py
+-rw-r--r--   0        0        0      814 2023-06-18 15:00:21.348884 pydantic_resolve-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5694 2023-06-18 15:05:30.997444 pydantic_resolve-1.2.0/README.md
+-rw-r--r--   0        0        0     6353 1970-01-01 00:00:00.000000 pydantic_resolve-1.2.0/PKG-INFO
```

### Comparing `pydantic_resolve-1.1.1/LICENSE` & `pydantic_resolve-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.1.1/pydantic_resolve/__init__.py` & `pydantic_resolve-1.2.0/pydantic_resolve/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.1.1/pydantic_resolve/core.py` & `pydantic_resolve-1.2.0/pydantic_resolve/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 from inspect import ismethod, iscoroutine
 from pydantic import BaseModel
 from dataclasses import is_dataclass
 from typing import TypeVar
 from .exceptions import ResolverTargetAttrNotFound, DataloaderDependCantBeResolved
-from .constant import PREFIX
+from .constant import PREFIX, POST_PREFIX
 
 T = TypeVar("T")
 
 def is_acceptable_type(target):
     """
     Check whether target is Pydantic object or Dataclass object
 
@@ -21,14 +21,20 @@
 
 def iter_over_object_resolvers(target):
     """get method starts with resolve_"""
     for k in dir(target):
         if k.startswith(PREFIX) and ismethod(target.__getattribute__(k)):
             yield k
 
+def iter_over_object_post_methods(target):
+    """get method starts with post_"""
+    for k in dir(target):
+        if k.startswith(POST_PREFIX) and ismethod(target.__getattribute__(k)):
+            yield k
+
 async def resolve_obj(target, field):
     item = target.__getattribute__(field)
     try:
         val = item()
     except AttributeError as e:
         if str(e) == "'Depends' object has no attribute 'load'":  
             # TODO: str(e) may changes in future, not stable
```

### Comparing `pydantic_resolve-1.1.1/pydantic_resolve/resolver.py` & `pydantic_resolve-1.2.0/pydantic_resolve/resolver.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import inspect
 import contextvars
 from inspect import iscoroutine
 from typing import TypeVar, Dict
 from .exceptions import ResolverTargetAttrNotFound, LoaderFieldNotProvidedError, MissingAnnotationError
 from typing import Any, Callable, Optional
 from pydantic_resolve import core
-from .constant import PREFIX
+from .constant import PREFIX, POST_PREFIX
 from .util import get_class_field_annotations
 from inspect import isclass
 from aiodataloader import DataLoader
 
 
 def LoaderDepend(  # noqa: N802
     dependency: Optional[Callable[..., Any]] = None,
@@ -96,18 +96,28 @@
         if self.ensure_type:
             if not item.__annotations__:
                 raise MissingAnnotationError(f'{field}: return annotation is required')
 
         while iscoroutine(val) or asyncio.isfuture(val):
             val = await val
 
+        # start to resolve
         val = await self.resolve(val)  
-
+        # all children is resolved
         target.__setattr__(target_attr_name, val)
 
+        # execute post methods, accept no params
+        for post_key in core.iter_over_object_post_methods(target):
+            post_attr_name = post_key.replace(POST_PREFIX, '')
+            if not hasattr(target, post_attr_name):
+                raise ResolverTargetAttrNotFound(f"fail to run {post_key}(), attribute {post_attr_name} not found")
+
+            post_method = target.__getattribute__(post_key)
+            post_method()
+
     async def resolve(self, target: T) -> T:
         """ entry: resolve dataclass object or pydantic object / or list in place """
 
         if isinstance(target, (list, tuple)):
             await asyncio.gather(*[self.resolve(t) for t in target])
 
         if core.is_acceptable_type(target):
```

### Comparing `pydantic_resolve-1.1.1/pydantic_resolve/util.py` & `pydantic_resolve-1.2.0/pydantic_resolve/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 from collections import defaultdict
 from dataclasses import is_dataclass
 import functools
 from pydantic import BaseModel
 from inspect import iscoroutine
-from typing import DefaultDict, Sequence, Type, TypeVar, List, Callable, Optional, Mapping, Union
+from typing import Any, DefaultDict, Sequence, Type, TypeVar, List, Callable, Optional, Mapping, Union
 import types
 
 def get_class_field_annotations(cls: Type):
     anno = cls.__dict__.get('__annotations__') or {}
     return anno.keys()
 
 
@@ -51,45 +51,66 @@
         is func: run func
         is class: call auto_mapping to have a try
     """
     def inner(inner_fn):
         @functools.wraps(inner_fn)
         async def wrap(*args, **kwargs):
 
-            val = inner_fn(*args, **kwargs)
-            while iscoroutine(val) or asyncio.isfuture(val):
-                val = await val
+            retVal = inner_fn(*args, **kwargs)
+            while iscoroutine(retVal) or asyncio.isfuture(retVal):
+                retVal = await retVal  # get final result
             
-            if val is None:
+            if retVal is None:
                 return None
 
             if isinstance(func_or_class, types.FunctionType):
-                return func_or_class(val)
+                # manual mapping
+                return func_or_class(retVal)
             else:
-                if isinstance(val, list):
-                    return [auto_mapping(func_or_class, v) for v in val]
-                return auto_mapping(func_or_class, val)
+                # auto mapping
+                if isinstance(retVal, list):
+                    if retVal:
+                        rule = get_mapping_rule(func_or_class, retVal[0])
+                        return apply_rule(rule, func_or_class, retVal, True)
+                    else:
+                        return retVal  # return []
+                else:
+                    rule = get_mapping_rule(func_or_class, retVal)
+                    return apply_rule(rule, func_or_class, retVal, False)
         return wrap
     return inner
 
 
-def auto_mapping(target, source):
+def get_mapping_rule(target, source) -> Optional[Callable]:
     # do noting
     if isinstance(source, target):
-        return source
+        return None
 
-    try:
-        # pydantic
-        if issubclass(target, BaseModel):
-            if target.Config.orm_mode:
-                return target.from_orm(source)
-            return target.parse_obj(source)
-        
-        # dataclass
-        if is_dataclass(target):
+    # pydantic
+    if issubclass(target, BaseModel):
+        if target.Config.orm_mode:
             if isinstance(source, dict):
-                return target(**source)
+                raise AttributeError(f"{type(source)} -> {target.__name__}: pydantic from_orm can't handle dict object")
+            else:
+                return lambda t, s: t.from_orm(s)
 
-    except Exception as e:
-        raise e
+        if isinstance(source, dict):
+            return lambda t, s: t.parse_obj(s)
+        else:
+            raise AttributeError(f"{type(source)} -> {target.__name__}: pydantic can't handle non-dict data")
     
-    raise RuntimeError('auto mapping fails')
+    # dataclass
+    if is_dataclass(target):
+        if isinstance(source, dict):
+            return lambda t, s: t(**s)
+    
+    raise NotImplementedError(f"{type(source)} -> {target.__name__}: faild to get auto mapping rule and execut mapping, use your own rule instead.")
+
+
+def apply_rule(rule: Optional[Callable], target, source: Any, is_list: bool):
+    if not rule:  # no change
+        return source
+
+    if is_list:
+        return [rule(target, s) for s in source]
+    else:
+        return rule(target, source)
```

### Comparing `pydantic_resolve-1.1.1/pyproject.toml` & `pydantic_resolve-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-resolve"
-version = "1.1.1"
+version = "1.2.0"
 description = "Make pydantic have a GraphQL-like assembly experience."
 authors = ["tangkikodo <allmonday@126.com>"]
 readme = "README.md"
 repository = "https://github.com/allmonday/pydantic_resolve"
 keywords = ["pydantic", "fastapi"]
 license = "MIT"
 packages = [{include = "pydantic_resolve"}]
```

### Comparing `pydantic_resolve-1.1.1/README.md` & `pydantic_resolve-1.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 ![Python Versions](https://img.shields.io/pypi/pyversions/pydantic-resolve)
 ![Test Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/allmonday/6f1661c6310e1b31c9a10b0d09d52d11/raw/covbadge.json)
 [![pypi](https://img.shields.io/pypi/v/pydantic-resolve.svg)](https://pypi.python.org/pypi/pydantic-resolve)
 [![Downloads](https://static.pepy.tech/personalized-badge/pydantic-resolve?period=month&units=abbreviation&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/pydantic-resolve)
 
 > A small yet powerful package which can run resolvers to generate deep nested datasets.
 
+[Change log](./changelog.md)
+
 **example**:
 
 ```python
 # define loader functions
 async def friends_batch_load_fn(names):
     mock_db = {
         'tangkikodo': ['tom', 'jerry'],
@@ -32,47 +34,47 @@
 # define schemas
 class Contact(BaseModel):
     number: Optional[int]
 
 class Friend(BaseModel):
     name: str
 
-    contact: int = 0
+    contact: Optional[Contact] = None
     @mapper(lambda n: Contact(number=n))
     def resolve_contact(self, loader=LoaderDepend(contact_batch_load_fn)):
         return loader.load(self.name)
 
 class User(BaseModel):
     name: str
     age: int
 
     greeting: str = ''
     def resolve_greeting(self):
         return f"hello, i'm {self.name}, {self.age} years old."
 
-    contact: int = 0
+    contact: Optional[Contact] = None
     @mapper(lambda n: Contact(number=n))
     def resolve_contact(self, loader=LoaderDepend(contact_batch_load_fn)):
         return loader.load(self.name)
 
     friends: List[Friend] = []
     @mapper(lambda items: [Friend(name=item) for item in items])  # transform after data received
     def resolve_friends(self, loader=LoaderDepend(friends_batch_load_fn)):
         return loader.load(self.name)
 
 class Root(BaseModel):
     users: List[User] = []
+    @mapper(lambda items: [User(**item) for item in items])
     def resolve_users(self):
         return [
-          {"name": "tangkikodo", "age": 19},
-            User(name="tangkikodo", age=19),  # transform first
-            User(name='john', age=21),
-            # User(name='trump', age=59),
-            # User(name='sally', age=21),
-            # User(name='some one', age=0)
+            {"name": "tangkikodo", "age": 19},
+            {"name": "john", "age": 20},
+            # {"name": "trump", "age": 21},
+            # {"name": "sally", "age": 22},
+            # {"name": "no man", "age": 23},
         ]
 
 async def main():
     import json
     root = await Resolver().resolve(Root())
     dct = root.dict()
     print(json.dumps(dct, indent=4))
```

### Comparing `pydantic_resolve-1.1.1/PKG-INFO` & `pydantic_resolve-1.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-resolve
-Version: 1.1.1
+Version: 1.2.0
 Summary: Make pydantic have a GraphQL-like assembly experience.
 Home-page: https://github.com/allmonday/pydantic_resolve
 License: MIT
 Keywords: pydantic,fastapi
 Author: tangkikodo
 Author-email: allmonday@126.com
 Requires-Python: >=3.7,<4.0
@@ -26,14 +26,16 @@
 ![Python Versions](https://img.shields.io/pypi/pyversions/pydantic-resolve)
 ![Test Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/allmonday/6f1661c6310e1b31c9a10b0d09d52d11/raw/covbadge.json)
 [![pypi](https://img.shields.io/pypi/v/pydantic-resolve.svg)](https://pypi.python.org/pypi/pydantic-resolve)
 [![Downloads](https://static.pepy.tech/personalized-badge/pydantic-resolve?period=month&units=abbreviation&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/pydantic-resolve)
 
 > A small yet powerful package which can run resolvers to generate deep nested datasets.
 
+[Change log](./changelog.md)
+
 **example**:
 
 ```python
 # define loader functions
 async def friends_batch_load_fn(names):
     mock_db = {
         'tangkikodo': ['tom', 'jerry'],
@@ -54,47 +56,47 @@
 # define schemas
 class Contact(BaseModel):
     number: Optional[int]
 
 class Friend(BaseModel):
     name: str
 
-    contact: int = 0
+    contact: Optional[Contact] = None
     @mapper(lambda n: Contact(number=n))
     def resolve_contact(self, loader=LoaderDepend(contact_batch_load_fn)):
         return loader.load(self.name)
 
 class User(BaseModel):
     name: str
     age: int
 
     greeting: str = ''
     def resolve_greeting(self):
         return f"hello, i'm {self.name}, {self.age} years old."
 
-    contact: int = 0
+    contact: Optional[Contact] = None
     @mapper(lambda n: Contact(number=n))
     def resolve_contact(self, loader=LoaderDepend(contact_batch_load_fn)):
         return loader.load(self.name)
 
     friends: List[Friend] = []
     @mapper(lambda items: [Friend(name=item) for item in items])  # transform after data received
     def resolve_friends(self, loader=LoaderDepend(friends_batch_load_fn)):
         return loader.load(self.name)
 
 class Root(BaseModel):
     users: List[User] = []
+    @mapper(lambda items: [User(**item) for item in items])
     def resolve_users(self):
         return [
-          {"name": "tangkikodo", "age": 19},
-            User(name="tangkikodo", age=19),  # transform first
-            User(name='john', age=21),
-            # User(name='trump', age=59),
-            # User(name='sally', age=21),
-            # User(name='some one', age=0)
+            {"name": "tangkikodo", "age": 19},
+            {"name": "john", "age": 20},
+            # {"name": "trump", "age": 21},
+            # {"name": "sally", "age": 22},
+            # {"name": "no man", "age": 23},
         ]
 
 async def main():
     import json
     root = await Resolver().resolve(Root())
     dct = root.dict()
     print(json.dumps(dct, indent=4))
```

