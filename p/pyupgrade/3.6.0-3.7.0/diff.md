# Comparing `tmp/pyupgrade-3.6.0.tar.gz` & `tmp/pyupgrade-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyupgrade-3.6.0.tar", last modified: Sat Jun 10 21:49:32 2023, max compression
+gzip compressed data, was "pyupgrade-3.7.0.tar", last modified: Sun Jun 18 20:41:39 2023, max compression
```

## Comparing `pyupgrade-3.6.0.tar` & `pyupgrade-3.7.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 21:49:32.239703 pyupgrade-3.6.0/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)    13524 2023-06-10 21:49:32.239703 pyupgrade-3.6.0/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)    12902 2023-06-10 21:49:31.000000 pyupgrade-3.6.0/README.md
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 21:49:32.235703 pyupgrade-3.6.0/pyupgrade/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      126 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/__main__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1445 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_ast_helpers.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3237 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_data.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    11830 2023-06-10 20:48:20.000000 pyupgrade-3.6.0/pyupgrade/_main.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 21:49:32.239703 pyupgrade-3.6.0/pyupgrade/_plugins/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      985 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/collections_abc.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      970 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/datetime_utc_alias.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1465 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/default_encoding.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2185 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/dict_literals.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1769 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/format_locals.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4398 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/fstrings.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1543 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/identity_equality.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    20494 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/imports.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      919 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/io_open.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     7781 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/legacy.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2447 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/lru_cache.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      967 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/metaclass_type.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      870 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/mock.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2438 2023-06-10 20:48:20.000000 pyupgrade-3.6.0/pyupgrade/_plugins/native_literals.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      631 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/new_style_classes.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4031 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/open_mode.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4213 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/oserror_aliases.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     9476 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/percent_format.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2303 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/set_literals.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      692 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/six_base_classes.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6522 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/six_calls.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3340 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/six_metaclasses.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      808 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/six_remove_decorators.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3634 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/six_simple.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3617 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/subprocess_run.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1413 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/type_of_primitive.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     8320 2023-06-10 20:48:20.000000 pyupgrade-3.6.0/pyupgrade/_plugins/typing_classes.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5714 2023-06-10 21:49:31.000000 pyupgrade-3.6.0/pyupgrade/_plugins/typing_pep563.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1695 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/typing_pep585.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5787 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/typing_pep604.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1208 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/typing_pep646_unpack.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1083 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/typing_text.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2182 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/unittest_aliases.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1073 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/unpack_list_comprehension.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6490 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_plugins/versioned_branches.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1949 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_string_helpers.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    14591 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/pyupgrade/_token_helpers.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 21:49:32.235703 pyupgrade-3.6.0/pyupgrade.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)    13524 2023-06-10 21:49:32.000000 pyupgrade-3.6.0/pyupgrade.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1711 2023-06-10 21:49:32.000000 pyupgrade-3.6.0/pyupgrade.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-10 21:49:32.000000 pyupgrade-3.6.0/pyupgrade.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       51 2023-06-10 21:49:32.000000 pyupgrade-3.6.0/pyupgrade.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       19 2023-06-10 21:49:32.000000 pyupgrade-3.6.0/pyupgrade.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       10 2023-06-10 21:49:32.000000 pyupgrade-3.6.0/pyupgrade.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1200 2023-06-10 21:49:32.239703 pyupgrade-3.6.0/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-06-10 20:34:09.000000 pyupgrade-3.6.0/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-18 20:41:39.758722 pyupgrade-3.7.0/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2022-04-30 16:59:39.000000 pyupgrade-3.7.0/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    13524 2023-06-18 20:41:39.758722 pyupgrade-3.7.0/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    12902 2023-06-18 20:41:39.000000 pyupgrade-3.7.0/README.md
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-18 20:41:39.754721 pyupgrade-3.7.0/pyupgrade/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-04-30 16:59:39.000000 pyupgrade-3.7.0/pyupgrade/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      126 2022-04-30 16:59:39.000000 pyupgrade-3.7.0/pyupgrade/__main__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1445 2022-04-30 16:59:39.000000 pyupgrade-3.7.0/pyupgrade/_ast_helpers.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3237 2022-11-10 15:38:09.000000 pyupgrade-3.7.0/pyupgrade/_data.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    11830 2023-06-18 20:35:59.000000 pyupgrade-3.7.0/pyupgrade/_main.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-18 20:41:39.758722 pyupgrade-3.7.0/pyupgrade/_plugins/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-04-30 16:59:39.000000 pyupgrade-3.7.0/pyupgrade/_plugins/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      985 2022-10-29 19:34:22.000000 pyupgrade-3.7.0/pyupgrade/_plugins/collections_abc.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      970 2022-12-02 18:20:28.000000 pyupgrade-3.7.0/pyupgrade/_plugins/datetime_utc_alias.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1465 2023-06-02 22:05:16.000000 pyupgrade-3.7.0/pyupgrade/_plugins/default_encoding.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2185 2022-04-30 16:59:39.000000 pyupgrade-3.7.0/pyupgrade/_plugins/dict_literals.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1769 2023-06-02 22:05:16.000000 pyupgrade-3.7.0/pyupgrade/_plugins/format_locals.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4398 2023-06-02 22:05:16.000000 pyupgrade-3.7.0/pyupgrade/_plugins/fstrings.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1543 2023-06-02 22:05:16.000000 pyupgrade-3.7.0/pyupgrade/_plugins/identity_equality.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    20218 2023-06-18 20:41:39.000000 pyupgrade-3.7.0/pyupgrade/_plugins/imports.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      919 2022-10-29 19:34:22.000000 pyupgrade-3.7.0/pyupgrade/_plugins/io_open.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     7781 2022-10-29 19:34:22.000000 pyupgrade-3.7.0/pyupgrade/_plugins/legacy.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2447 2023-06-02 22:05:16.000000 pyupgrade-3.7.0/pyupgrade/_plugins/lru_cache.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      967 2022-10-29 19:34:22.000000 pyupgrade-3.7.0/pyupgrade/_plugins/metaclass_type.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      870 2022-10-29 19:34:22.000000 pyupgrade-3.7.0/pyupgrade/_plugins/mock.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2438 2023-06-18 20:35:59.000000 pyupgrade-3.7.0/pyupgrade/_plugins/native_literals.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      631 2022-10-29 19:34:22.000000 pyupgrade-3.7.0/pyupgrade/_plugins/new_style_classes.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4031 2023-06-02 22:05:16.000000 pyupgrade-3.7.0/pyupgrade/_plugins/open_mode.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4213 2022-10-29 19:34:22.000000 pyupgrade-3.7.0/pyupgrade/_plugins/oserror_aliases.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     9476 2023-06-02 22:05:16.000000 pyupgrade-3.7.0/pyupgrade/_plugins/percent_format.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2303 2022-10-29 19:34:22.000000 pyupgrade-3.7.0/pyupgrade/_plugins/set_literals.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      692 2022-10-29 19:34:22.000000 pyupgrade-3.7.0/pyupgrade/_plugins/six_base_classes.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     6522 2023-06-02 22:05:16.000000 pyupgrade-3.7.0/pyupgrade/_plugins/six_calls.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3340 2022-10-29 19:34:22.000000 pyupgrade-3.7.0/pyupgrade/_plugins/six_metaclasses.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      808 2022-10-29 19:34:22.000000 pyupgrade-3.7.0/pyupgrade/_plugins/six_remove_decorators.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3634 2022-10-29 19:34:22.000000 pyupgrade-3.7.0/pyupgrade/_plugins/six_simple.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3617 2022-04-30 16:59:39.000000 pyupgrade-3.7.0/pyupgrade/_plugins/subprocess_run.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1413 2023-06-02 22:05:16.000000 pyupgrade-3.7.0/pyupgrade/_plugins/type_of_primitive.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     8320 2023-06-18 20:35:59.000000 pyupgrade-3.7.0/pyupgrade/_plugins/typing_classes.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5714 2023-06-18 20:35:59.000000 pyupgrade-3.7.0/pyupgrade/_plugins/typing_pep563.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1695 2022-04-30 16:59:39.000000 pyupgrade-3.7.0/pyupgrade/_plugins/typing_pep585.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5787 2023-06-02 22:05:16.000000 pyupgrade-3.7.0/pyupgrade/_plugins/typing_pep604.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1208 2022-11-10 15:10:00.000000 pyupgrade-3.7.0/pyupgrade/_plugins/typing_pep646_unpack.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1083 2022-10-29 19:34:22.000000 pyupgrade-3.7.0/pyupgrade/_plugins/typing_text.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2182 2022-10-29 19:34:22.000000 pyupgrade-3.7.0/pyupgrade/_plugins/unittest_aliases.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1073 2023-06-02 22:05:16.000000 pyupgrade-3.7.0/pyupgrade/_plugins/unpack_list_comprehension.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     6490 2023-06-02 22:05:16.000000 pyupgrade-3.7.0/pyupgrade/_plugins/versioned_branches.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1949 2022-04-30 16:59:39.000000 pyupgrade-3.7.0/pyupgrade/_string_helpers.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    14591 2023-06-02 22:05:16.000000 pyupgrade-3.7.0/pyupgrade/_token_helpers.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-18 20:41:39.754721 pyupgrade-3.7.0/pyupgrade.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    13524 2023-06-18 20:41:39.000000 pyupgrade-3.7.0/pyupgrade.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1711 2023-06-18 20:41:39.000000 pyupgrade-3.7.0/pyupgrade.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-18 20:41:39.000000 pyupgrade-3.7.0/pyupgrade.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       51 2023-06-18 20:41:39.000000 pyupgrade-3.7.0/pyupgrade.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       19 2023-06-18 20:41:39.000000 pyupgrade-3.7.0/pyupgrade.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       10 2023-06-18 20:41:39.000000 pyupgrade-3.7.0/pyupgrade.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1200 2023-06-18 20:41:39.758722 pyupgrade-3.7.0/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-04-30 16:59:39.000000 pyupgrade-3.7.0/setup.py
```

### Comparing `pyupgrade-3.6.0/LICENSE` & `pyupgrade-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/PKG-INFO` & `pyupgrade-3.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyupgrade
-Version: 3.6.0
+Version: 3.7.0
 Summary: A tool to automatically upgrade syntax for newer versions.
 Home-page: https://github.com/asottile/pyupgrade
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -34,15 +34,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.6.0
+    rev: v3.7.0
     hooks:
     -   id: pyupgrade
 ```
 
 ## Implemented features
 
 ### Set literals
```

### Comparing `pyupgrade-3.6.0/README.md` & `pyupgrade-3.7.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.6.0
+    rev: v3.7.0
     hooks:
     -   id: pyupgrade
 ```
 
 ## Implemented features
 
 ### Set literals
```

### Comparing `pyupgrade-3.6.0/pyupgrade/_ast_helpers.py` & `pyupgrade-3.7.0/pyupgrade/_ast_helpers.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_data.py` & `pyupgrade-3.7.0/pyupgrade/_data.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_main.py` & `pyupgrade-3.7.0/pyupgrade/_main.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/collections_abc.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/collections_abc.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/datetime_utc_alias.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/datetime_utc_alias.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/default_encoding.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/default_encoding.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/dict_literals.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/dict_literals.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/format_locals.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/format_locals.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/fstrings.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/fstrings.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/identity_equality.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/identity_equality.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/imports.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/imports.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pyupgrade._data import TokenFunc
 from pyupgrade._token_helpers import find_end
 from pyupgrade._token_helpers import find_token
 from pyupgrade._token_helpers import has_space_before
 from pyupgrade._token_helpers import indented_amount
 
 # GENERATED VIA generate-imports
-# Using reorder-python-imports==3.9.0
+# Using reorder-python-imports==3.10.0
 REMOVALS = {
     (3,): {
         '__future__': {
             'absolute_import', 'division', 'generators', 'nested_scopes',
             'print_function', 'unicode_literals', 'with_statement',
         },
         'builtins': {
@@ -92,15 +92,14 @@
         ('typing_extensions', 'AsyncIterable'): 'typing',
         ('typing_extensions', 'AsyncIterator'): 'typing',
         ('typing_extensions', 'Awaitable'): 'typing',
         ('typing_extensions', 'ClassVar'): 'typing',
         ('typing_extensions', 'ContextManager'): 'typing',
         ('typing_extensions', 'Coroutine'): 'typing',
         ('typing_extensions', 'DefaultDict'): 'typing',
-        ('typing_extensions', 'NewType'): 'typing',
         ('typing_extensions', 'TYPE_CHECKING'): 'typing',
         ('typing_extensions', 'Text'): 'typing',
         ('typing_extensions', 'Type'): 'typing',
     },
     (3, 7): {
         ('mypy_extensions', 'NoReturn'): 'typing',
         ('typing_extensions', 'AsyncContextManager'): 'typing',
@@ -109,17 +108,15 @@
         ('typing_extensions', 'Counter'): 'typing',
         ('typing_extensions', 'Deque'): 'typing',
         ('typing_extensions', 'NoReturn'): 'typing',
     },
     (3, 8): {
         ('mypy_extensions', 'TypedDict'): 'typing',
         ('typing_extensions', 'Final'): 'typing',
-        ('typing_extensions', 'Literal'): 'typing',
         ('typing_extensions', 'OrderedDict'): 'typing',
-        ('typing_extensions', 'Protocol'): 'typing',
         ('typing_extensions', 'SupportsIndex'): 'typing',
         ('typing_extensions', 'runtime_checkable'): 'typing',
     },
     (3, 9): {
         ('typing', 'AsyncGenerator'): 'collections.abc',
         ('typing', 'AsyncIterable'): 'collections.abc',
         ('typing', 'AsyncIterator'): 'collections.abc',
@@ -152,36 +149,34 @@
         ('typing.re', 'Pattern'): 're',
         ('typing_extensions', 'Annotated'): 'typing',
         ('typing_extensions', 'get_type_hints'): 'typing',
     },
     (3, 10): {
         ('typing', 'Callable'): 'collections.abc',
         ('typing_extensions', 'Concatenate'): 'typing',
+        ('typing_extensions', 'Literal'): 'typing',
+        ('typing_extensions', 'NewType'): 'typing',
         ('typing_extensions', 'ParamSpecArgs'): 'typing',
         ('typing_extensions', 'ParamSpecKwargs'): 'typing',
         ('typing_extensions', 'TypeAlias'): 'typing',
         ('typing_extensions', 'TypeGuard'): 'typing',
         ('typing_extensions', 'get_args'): 'typing',
         ('typing_extensions', 'get_origin'): 'typing',
         ('typing_extensions', 'is_typeddict'): 'typing',
     },
     (3, 11): {
         ('typing_extensions', 'Any'): 'typing',
         ('typing_extensions', 'LiteralString'): 'typing',
-        ('typing_extensions', 'NamedTuple'): 'typing',
         ('typing_extensions', 'Never'): 'typing',
         ('typing_extensions', 'NotRequired'): 'typing',
         ('typing_extensions', 'Required'): 'typing',
         ('typing_extensions', 'Self'): 'typing',
-        ('typing_extensions', 'TypedDict'): 'typing',
-        ('typing_extensions', 'Unpack'): 'typing',
         ('typing_extensions', 'assert_never'): 'typing',
         ('typing_extensions', 'assert_type'): 'typing',
         ('typing_extensions', 'clear_overloads'): 'typing',
-        ('typing_extensions', 'dataclass_transform'): 'typing',
         ('typing_extensions', 'final'): 'typing',
         ('typing_extensions', 'get_overloads'): 'typing',
         ('typing_extensions', 'overload'): 'typing',
         ('typing_extensions', 'reveal_type'): 'typing',
     },
 }
 REPLACE_MODS = {
```

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/io_open.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/io_open.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/legacy.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/legacy.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/lru_cache.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/lru_cache.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/metaclass_type.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/metaclass_type.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/mock.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/mock.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/native_literals.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/native_literals.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/new_style_classes.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/new_style_classes.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/open_mode.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/open_mode.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/oserror_aliases.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/oserror_aliases.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/percent_format.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/percent_format.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/set_literals.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/set_literals.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/six_base_classes.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/six_base_classes.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/six_calls.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/six_calls.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/six_metaclasses.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/six_metaclasses.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/six_remove_decorators.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/six_remove_decorators.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/six_simple.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/six_simple.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/subprocess_run.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/subprocess_run.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/type_of_primitive.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/type_of_primitive.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/typing_classes.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/typing_classes.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/typing_pep563.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/typing_pep563.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/typing_pep585.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/typing_pep585.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/typing_pep604.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/typing_pep604.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/typing_pep646_unpack.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/typing_pep646_unpack.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/typing_text.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/typing_text.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/unittest_aliases.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/unittest_aliases.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/unpack_list_comprehension.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/unpack_list_comprehension.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_plugins/versioned_branches.py` & `pyupgrade-3.7.0/pyupgrade/_plugins/versioned_branches.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_string_helpers.py` & `pyupgrade-3.7.0/pyupgrade/_string_helpers.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade/_token_helpers.py` & `pyupgrade-3.7.0/pyupgrade/_token_helpers.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/pyupgrade.egg-info/PKG-INFO` & `pyupgrade-3.7.0/pyupgrade.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyupgrade
-Version: 3.6.0
+Version: 3.7.0
 Summary: A tool to automatically upgrade syntax for newer versions.
 Home-page: https://github.com/asottile/pyupgrade
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -34,15 +34,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.6.0
+    rev: v3.7.0
     hooks:
     -   id: pyupgrade
 ```
 
 ## Implemented features
 
 ### Set literals
```

### Comparing `pyupgrade-3.6.0/pyupgrade.egg-info/SOURCES.txt` & `pyupgrade-3.7.0/pyupgrade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.6.0/setup.cfg` & `pyupgrade-3.7.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyupgrade
-version = 3.6.0
+version = 3.7.0
 description = A tool to automatically upgrade syntax for newer versions.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/pyupgrade
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
```

