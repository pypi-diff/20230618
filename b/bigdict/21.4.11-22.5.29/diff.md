# Comparing `tmp/bigdict-21.4.11.tar.gz` & `tmp/bigdict-22.5.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigdict-21.4.11.tar", last modified: Sun Apr 11 07:20:50 2021, max compression
+gzip compressed data, was "bigdict-22.5.29.tar", last modified: Mon May 30 01:02:24 2022, max compression
```

## Comparing `bigdict-21.4.11.tar` & `bigdict-22.5.29.tar`

### file list

```diff
@@ -1,18 +1,7 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-11 07:20:50.093240 bigdict-21.4.11/
--rw-rw-r--   0 root         (0) root         (0)     1067 2021-03-28 05:22:35.000000 bigdict-21.4.11/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       81 2021-04-10 07:13:28.000000 bigdict-21.4.11/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1585 2021-04-11 07:20:50.089240 bigdict-21.4.11/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1004 2021-04-11 07:18:04.000000 bigdict-21.4.11/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2021-04-11 07:20:50.093240 bigdict-21.4.11/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      634 2021-04-11 07:13:06.000000 bigdict-21.4.11/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-11 07:20:50.085240 bigdict-21.4.11/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-11 07:20:50.089240 bigdict-21.4.11/src/bigdict/
--rw-rw-r--   0 root         (0) root         (0)      112 2021-04-11 07:13:13.000000 bigdict-21.4.11/src/bigdict/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6224 2021-04-11 07:09:11.000000 bigdict-21.4.11/src/bigdict/_bigdict.py
--rw-rw-r--   0 root         (0) root         (0)        0 2021-04-10 07:12:54.000000 bigdict-21.4.11/src/bigdict/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-11 07:20:50.089240 bigdict-21.4.11/src/bigdict.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1585 2021-04-11 07:20:50.000000 bigdict-21.4.11/src/bigdict.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      281 2021-04-11 07:20:50.000000 bigdict-21.4.11/src/bigdict.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-11 07:20:50.000000 bigdict-21.4.11/src/bigdict.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2021-04-11 07:20:50.000000 bigdict-21.4.11/src/bigdict.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2021-04-11 07:20:50.000000 bigdict-21.4.11/src/bigdict.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1067 2021-03-28 05:22:35.008888 bigdict-22.5.29/LICENSE
+-rw-r--r--   0        0        0     1004 2021-05-06 05:52:05.660601 bigdict-22.5.29/README.md
+-rw-r--r--   0        0        0     1241 2022-05-30 00:56:47.146578 bigdict-22.5.29/pyproject.toml
+-rw-r--r--   0        0        0       86 2022-05-30 00:56:01.231560 bigdict-22.5.29/src/bigdict/__init__.py
+-rw-r--r--   0        0        0     6449 2022-05-30 00:54:59.304883 bigdict-22.5.29/src/bigdict/_bigdict.py
+-rw-r--r--   0        0        0        0 2021-04-10 07:12:54.773652 bigdict-22.5.29/src/bigdict/py.typed
+-rw-r--r--   0        0        0     1764 1970-01-01 00:00:00.000000 bigdict-22.5.29/PKG-INFO
```

### Comparing `bigdict-21.4.11/LICENSE` & `bigdict-22.5.29/LICENSE`

 * *Files identical despite different names*

### Comparing `bigdict-21.4.11/README.md` & `bigdict-22.5.29/README.md`

 * *Files identical despite different names*

### Comparing `bigdict-21.4.11/src/bigdict/_bigdict.py` & `bigdict-22.5.29/src/bigdict/_bigdict.py`

 * *Files 3% similar despite different names*

```diff
@@ -199,14 +199,19 @@
     def view(self) -> 'DictView':
         return DictView(
             self.__class__(self.path, read_only=True)
         )
 
 
 class DictView(Mapping):
+    # `types.MappingProxyType` could achieve similar effects,
+    # but it might be problematic when we send the object
+    # to another process. Plus, this separate class will have
+    # any flexibility that may be needed.
+
     def __init__(self, dict_: Mapping):
         self._dict = dict_
 
     def __repr__(self):
         return f'{self.__class__.__name__}({repr(self._dict)})'
 
     def __str__(self):
```

