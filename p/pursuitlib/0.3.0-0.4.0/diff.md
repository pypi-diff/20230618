# Comparing `tmp/pursuitlib-0.3.0.tar.gz` & `tmp/pursuitlib-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pursuitlib-0.3.0.tar", last modified: Sun Apr 23 21:39:55 2023, max compression
+gzip compressed data, was "pursuitlib-0.4.0.tar", last modified: Sun Jun 18 20:15:29 2023, max compression
```

## Comparing `pursuitlib-0.3.0.tar` & `pursuitlib-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 21:39:55.748036 pursuitlib-0.3.0/
--rw-rw-rw-   0        0        0      510 2023-04-23 21:39:55.747036 pursuitlib-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      110 2022-12-04 22:52:50.000000 pursuitlib-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 21:39:55.725034 pursuitlib-0.3.0/pursuitlib/
--rw-rw-rw-   0        0        0        0 2022-12-04 22:52:50.000000 pursuitlib-0.3.0/pursuitlib/__init__.py
--rw-rw-rw-   0        0        0      651 2022-12-04 22:52:50.000000 pursuitlib-0.3.0/pursuitlib/color.py
--rw-rw-rw-   0        0        0     1043 2023-04-23 18:50:32.000000 pursuitlib-0.3.0/pursuitlib/decorators.py
--rw-rw-rw-   0        0        0      314 2023-04-15 22:57:18.000000 pursuitlib-0.3.0/pursuitlib/indexedenum.py
--rw-rw-rw-   0        0        0     1411 2023-04-14 17:01:53.000000 pursuitlib-0.3.0/pursuitlib/iterators.py
--rw-rw-rw-   0        0        0      962 2023-04-10 18:15:09.000000 pursuitlib-0.3.0/pursuitlib/parsing.py
--rw-rw-rw-   0        0        0      781 2023-04-10 18:11:46.000000 pursuitlib-0.3.0/pursuitlib/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-23 21:39:55.744036 pursuitlib-0.3.0/pursuitlib.egg-info/
--rw-rw-rw-   0        0        0      510 2023-04-23 21:39:55.000000 pursuitlib-0.3.0/pursuitlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-04-23 21:39:55.000000 pursuitlib-0.3.0/pursuitlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 21:39:55.000000 pursuitlib-0.3.0/pursuitlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-23 21:39:55.000000 pursuitlib-0.3.0/pursuitlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      177 2022-12-04 22:52:50.000000 pursuitlib-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-23 21:39:55.749035 pursuitlib-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      691 2023-04-23 21:16:54.000000 pursuitlib-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:15:29.153437 pursuitlib-0.4.0/
+-rw-rw-rw-   0        0        0      510 2023-06-18 20:15:29.153437 pursuitlib-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      110 2023-06-18 20:00:12.000000 pursuitlib-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 20:15:29.145808 pursuitlib-0.4.0/pursuitlib/
+-rw-rw-rw-   0        0        0       23 2023-06-18 20:03:59.000000 pursuitlib-0.4.0/pursuitlib/__init__.py
+-rw-rw-rw-   0        0        0      651 2023-06-18 20:00:12.000000 pursuitlib-0.4.0/pursuitlib/color.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:15:29.152931 pursuitlib-0.4.0/pursuitlib/console/
+-rw-rw-rw-   0        0        0        0 2023-05-28 13:49:51.000000 pursuitlib-0.4.0/pursuitlib/console/__init__.py
+-rw-rw-rw-   0        0        0     1721 2023-06-18 20:08:23.000000 pursuitlib-0.4.0/pursuitlib/console/console.py
+-rw-rw-rw-   0        0        0     1724 2023-06-18 20:08:23.000000 pursuitlib-0.4.0/pursuitlib/console/table.py
+-rw-rw-rw-   0        0        0      393 2023-06-18 20:08:23.000000 pursuitlib-0.4.0/pursuitlib/console/textcolor.py
+-rw-rw-rw-   0        0        0      724 2023-06-18 20:08:23.000000 pursuitlib-0.4.0/pursuitlib/console/textcolors.py
+-rw-rw-rw-   0        0        0     2212 2023-06-18 20:08:23.000000 pursuitlib-0.4.0/pursuitlib/console/textcomponent.py
+-rw-rw-rw-   0        0        0      572 2023-05-28 16:25:50.000000 pursuitlib-0.4.0/pursuitlib/console/textformatting.py
+-rw-rw-rw-   0        0        0     3367 2023-06-18 20:08:23.000000 pursuitlib-0.4.0/pursuitlib/console/textstyle.py
+-rw-rw-rw-   0        0        0     1103 2023-06-18 20:09:11.000000 pursuitlib-0.4.0/pursuitlib/decorators.py
+-rw-rw-rw-   0        0        0      218 2023-06-18 20:09:30.000000 pursuitlib-0.4.0/pursuitlib/errors.py
+-rw-rw-rw-   0        0        0      314 2023-06-18 20:00:12.000000 pursuitlib-0.4.0/pursuitlib/indexedenum.py
+-rw-rw-rw-   0        0        0     1411 2023-06-18 20:08:52.000000 pursuitlib-0.4.0/pursuitlib/iterators.py
+-rw-rw-rw-   0        0        0      962 2023-06-18 20:00:12.000000 pursuitlib-0.4.0/pursuitlib/parsing.py
+-rw-rw-rw-   0        0        0      781 2023-06-18 20:00:12.000000 pursuitlib-0.4.0/pursuitlib/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:15:29.148863 pursuitlib-0.4.0/pursuitlib.egg-info/
+-rw-rw-rw-   0        0        0      510 2023-06-18 20:15:29.000000 pursuitlib-0.4.0/pursuitlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2023-06-18 20:15:29.000000 pursuitlib-0.4.0/pursuitlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 20:15:29.000000 pursuitlib-0.4.0/pursuitlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-18 20:15:29.000000 pursuitlib-0.4.0/pursuitlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      177 2023-06-18 20:00:12.000000 pursuitlib-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-18 20:15:29.153944 pursuitlib-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      707 2023-06-18 20:15:17.000000 pursuitlib-0.4.0/setup.py
```

### Comparing `pursuitlib-0.3.0/pursuitlib/color.py` & `pursuitlib-0.4.0/pursuitlib/color.py`

 * *Files identical despite different names*

### Comparing `pursuitlib-0.3.0/pursuitlib/decorators.py` & `pursuitlib-0.4.0/pursuitlib/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,27 @@
+from typing import TypeVar
+
+T = TypeVar("T")
+
+
 # This decorator can be used to easily create decorators that
 # can optionally take arguments
 def decorator(function):
     def wrapper(*args, **kwargs):
         # If the decorator is used without parenthesis, the first argument
         # is the function that needs to be passed to "decorator"
         if len(args) == 1 and callable(args[0]) and len(kwargs) == 0:
             fn = args[0]
             return function(fn)
         else: return lambda f: function(f, *args, **kwargs)
     return wrapper
 
 
 # This decorator can be used to cache the result of a method
-def cached(function):
+def cached(function: T) -> T:
     def wrapper(self, *args, force_update: bool = False, **kwargs):
         cached_field = f"__cached_{function.__name__}"
 
         # Use the cached value when available
         if not force_update and hasattr(self, cached_field):
             return getattr(self, cached_field)
```

### Comparing `pursuitlib-0.3.0/pursuitlib/iterators.py` & `pursuitlib-0.4.0/pursuitlib/iterators.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import TypeVar, Iterable, Iterator, Callable, Optional
 
 ###############################################################
 # Iterator that allow the use of transformers using methods   #
 # rather than functions                                       #
 ###############################################################
 
-
 T = TypeVar("T")
 R = TypeVar("R")
 
+
 class ChainableIterator(Iterator[T]):
     def __init__(self, base: Iterator[T]):
         self.base = base
 
     def first(self) -> T:
         return next(self.base)
```

### Comparing `pursuitlib-0.3.0/pursuitlib/parsing.py` & `pursuitlib-0.4.0/pursuitlib/parsing.py`

 * *Files identical despite different names*

### Comparing `pursuitlib-0.3.0/pursuitlib/utils.py` & `pursuitlib-0.4.0/pursuitlib/utils.py`

 * *Files identical despite different names*

