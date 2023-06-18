# Comparing `tmp/mdis-0.3.tar.gz` & `tmp/mdis-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ghostmansd/mdis/dist/.tmp-8cr_ulv3/mdis-0.3.tar", last modified: Sun Jun 18 11:21:15 2023, max compression
+gzip compressed data, was "/home/ghostmansd/mdis/dist/.tmp-r8vxm8o1/mdis-0.4.tar", last modified: Sun Jun 18 19:00:10 2023, max compression
```

## Comparing `mdis-0.3.tar` & `mdis-0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-18 11:21:15.000000 mdis-0.3/
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     1272 2023-06-13 22:23:19.000000 mdis-0.3/LICENSE
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     4473 2023-06-18 11:21:15.000000 mdis-0.3/PKG-INFO
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     3649 2023-06-16 20:42:33.000000 mdis-0.3/README.md
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      938 2023-06-18 11:20:46.000000 mdis-0.3/pyproject.toml
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)       38 2023-06-18 11:21:15.000000 mdis-0.3/setup.cfg
-drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-18 11:21:15.000000 mdis-0.3/src/
-drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-18 11:21:15.000000 mdis-0.3/src/mdis/
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      328 2023-06-18 11:20:50.000000 mdis-0.3/src/mdis/__init__.py
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     2430 2023-06-14 10:35:12.000000 mdis-0.3/src/mdis/dispatcher.py
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      477 2023-06-16 20:42:11.000000 mdis-0.3/src/mdis/visitor.py
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      624 2023-06-14 10:29:43.000000 mdis-0.3/src/mdis/walker.py
-drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-18 11:21:15.000000 mdis-0.3/src/mdis.egg-info/
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     4473 2023-06-18 11:21:15.000000 mdis-0.3/src/mdis.egg-info/PKG-INFO
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      243 2023-06-18 11:21:15.000000 mdis-0.3/src/mdis.egg-info/SOURCES.txt
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)        1 2023-06-18 11:21:15.000000 mdis-0.3/src/mdis.egg-info/dependency_links.txt
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)        5 2023-06-18 11:21:15.000000 mdis-0.3/src/mdis.egg-info/top_level.txt
+drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-18 19:00:10.000000 mdis-0.4/
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     1272 2023-06-13 22:23:19.000000 mdis-0.4/LICENSE
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     4473 2023-06-18 19:00:10.000000 mdis-0.4/PKG-INFO
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     3649 2023-06-16 20:42:33.000000 mdis-0.4/README.md
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      938 2023-06-18 18:53:24.000000 mdis-0.4/pyproject.toml
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)       38 2023-06-18 19:00:10.000000 mdis-0.4/setup.cfg
+drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-18 19:00:10.000000 mdis-0.4/src/
+drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-18 19:00:10.000000 mdis-0.4/src/mdis/
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      316 2023-06-18 18:53:19.000000 mdis-0.4/src/mdis/__init__.py
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     2725 2023-06-18 18:51:54.000000 mdis-0.4/src/mdis/dispatcher.py
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      513 2023-06-18 18:42:08.000000 mdis-0.4/src/mdis/visitor.py
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      959 2023-06-18 18:46:15.000000 mdis-0.4/src/mdis/walker.py
+drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-18 19:00:10.000000 mdis-0.4/src/mdis.egg-info/
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     4473 2023-06-18 19:00:10.000000 mdis-0.4/src/mdis.egg-info/PKG-INFO
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      243 2023-06-18 19:00:10.000000 mdis-0.4/src/mdis.egg-info/SOURCES.txt
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)        1 2023-06-18 19:00:10.000000 mdis-0.4/src/mdis.egg-info/dependency_links.txt
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)        5 2023-06-18 19:00:10.000000 mdis-0.4/src/mdis.egg-info/top_level.txt
```

### Comparing `mdis-0.3/LICENSE` & `mdis-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mdis-0.3/PKG-INFO` & `mdis-0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdis
-Version: 0.3
+Version: 0.4
 Summary: Python dispatching library
 Author-email: Dmitry Selyutin <ghostmansd@gmail.com>
 Project-URL: Homepage, https://git.libre-soc.org/?p=mdis.git
 Project-URL: Bug Tracker, https://bugs.libre-soc.org/
 Keywords: dispatch,dispather,map,iterator,iterable,visitor,walker
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `mdis-0.3/README.md` & `mdis-0.4/README.md`

 * *Files identical despite different names*

### Comparing `mdis-0.3/pyproject.toml` & `mdis-0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=46.4.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mdis"
-version = "0.3"
+version = "0.4"
 authors = [
   { name="Dmitry Selyutin", email="ghostmansd@gmail.com" },
 ]
 keywords = [
     "dispatch",
     "dispather",
     "map",
```

### Comparing `mdis-0.3/src/mdis/dispatcher.py` & `mdis-0.4/src/mdis/dispatcher.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,23 @@
-import collections as _collections
-import inspect as _inspect
-import types as _types
+__all__ = [
+    "Dispatcher",
+    "DispatcherMeta",
+    "Hook",
+]
+
+import collections
+import functools
+import inspect
+import types
 
 
 class Hook(object):
     def __init__(self, *typeids):
         for typeid in typeids:
-            if not isinstance(typeid, type):
+            if not callable(typeid):
                 raise ValueError(typeid)
         self.__typeids = typeids
         return super().__init__()
 
     def __iter__(self):
         yield from self.__typeids
 
@@ -36,38 +43,45 @@
     __hooks__ = {}
 
     def __new__(metacls, name, bases, ns):
         hooks = {}
         ishook = lambda member: isinstance(member, Hook)
 
         for basecls in reversed(bases):
-            members = _inspect.getmembers(basecls, predicate=ishook)
+            members = inspect.getmembers(basecls, predicate=ishook)
             for (_, hook) in members:
                 hooks.update(dict.fromkeys(hook, hook))
 
-        conflicts = _collections.defaultdict(list)
+        conflicts = collections.defaultdict(list)
         for (key, value) in tuple(ns.items()):
             if not ishook(value):
                 continue
             hook = value
             for typeid in hook:
                 hooks[typeid] = hook
                 conflicts[typeid].append(key)
             ns[key] = hook
 
         for (typeid, keys) in conflicts.items():
             if len(keys) > 1:
                 raise ValueError(f"dispatch conflict: {keys!r}")
 
-        ns["__hooks__"] = _types.MappingProxyType(hooks)
+        ns["__hooks__"] = types.MappingProxyType(hooks)
 
         return super().__new__(metacls, name, bases, ns)
 
+    @functools.lru_cache(maxsize=None)
     def dispatch(cls, typeid=object):
-        return cls.__hooks__.get(typeid)
+        hook = cls.__hooks__.get(typeid)
+        if hook is not None:
+            return hook
+        for (checker, hook) in cls.__hooks__.items():
+            if not isinstance(checker, type) and checker(typeid):
+                return hook
+        return None
 
 
 class Dispatcher(metaclass=DispatcherMeta):
     def __call__(self, instance):
         for typeid in instance.__class__.__mro__:
             hook = self.__class__.dispatch(typeid=typeid)
             if hook is not None:
```

### Comparing `mdis-0.3/src/mdis/walker.py` & `mdis-0.4/src/mdis/walker.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,38 @@
-from . import dispatcher as _dispatcher
+__all__ = [
+    "Walker",
+    "WalkerMeta",
+]
 
+import dataclasses
 
-class WalkerMeta(_dispatcher.DispatcherMeta):
+from . import dispatcher
+
+
+class WalkerMeta(dispatcher.DispatcherMeta):
     pass
 
 
-class Walker(_dispatcher.Dispatcher, metaclass=WalkerMeta):
-    @_dispatcher.Hook(tuple, list, set, frozenset)
+class Walker(dispatcher.Dispatcher, metaclass=WalkerMeta):
+    @dispatcher.Hook(tuple, list, set, frozenset)
     def dispatch_sequence(self, instance):
         for item in instance:
             yield item
             yield from self(item)
 
-    @_dispatcher.Hook(dict)
+    @dispatcher.Hook(dict)
     def dispatch_mapping(self, instance):
         for (key, value) in instance.items():
             yield (key, value)
             yield from self((key, value))
 
-    @_dispatcher.Hook(object)
+    @dispatcher.Hook(dataclasses.is_dataclass)
+    def dispatch_dataclass(self, instance):
+        for field in dataclasses.fields(instance):
+            key = field.name
+            value = getattr(instance, key)
+            yield (key, value)
+            yield from self((key, value))
+
+    @dispatcher.Hook(object)
     def dispatch_object(self, instance):
         yield from ()
```

### Comparing `mdis-0.3/src/mdis.egg-info/PKG-INFO` & `mdis-0.4/src/mdis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdis
-Version: 0.3
+Version: 0.4
 Summary: Python dispatching library
 Author-email: Dmitry Selyutin <ghostmansd@gmail.com>
 Project-URL: Homepage, https://git.libre-soc.org/?p=mdis.git
 Project-URL: Bug Tracker, https://bugs.libre-soc.org/
 Keywords: dispatch,dispather,map,iterator,iterable,visitor,walker
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

