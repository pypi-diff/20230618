# Comparing `tmp/recnetpy-0.1.49.tar.gz` & `tmp/recnetpy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recnetpy-0.1.49.tar", last modified: Fri Jun 16 07:53:53 2023, max compression
+gzip compressed data, was "recnetpy-0.1.5.tar", last modified: Sun Jun 18 11:23:42 2023, max compression
```

## Comparing `recnetpy-0.1.49.tar` & `recnetpy-0.1.5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 07:53:53.409621 recnetpy-0.1.49/
--rw-rw-rw-   0        0        0     1140 2023-05-26 12:49:51.000000 recnetpy-0.1.49/LICENSE
--rw-rw-rw-   0        0        0     3242 2023-06-16 07:53:53.409112 recnetpy-0.1.49/PKG-INFO
--rw-rw-rw-   0        0        0     2672 2023-05-26 12:49:51.000000 recnetpy-0.1.49/README.md
--rw-rw-rw-   0        0        0      715 2023-06-16 07:52:44.000000 recnetpy-0.1.49/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-16 07:53:53.409621 recnetpy-0.1.49/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-16 07:53:53.135156 recnetpy-0.1.49/src/
-drwxrwxrwx   0        0        0        0 2023-06-16 07:53:53.151886 recnetpy-0.1.49/src/recnetpy/
--rw-rw-rw-   0        0        0       26 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/__init__.py
--rw-rw-rw-   0        0        0     1550 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/client.py
-drwxrwxrwx   0        0        0        0 2023-06-16 07:53:53.262512 recnetpy-0.1.49/src/recnetpy/dataclasses/
--rw-rw-rw-   0        0        0      534 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/dataclasses/__init__.py
--rw-rw-rw-   0        0        0    10007 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/dataclasses/account.py
--rw-rw-rw-   0        0        0     1368 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/dataclasses/base.py
--rw-rw-rw-   0        0        0     1011 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/dataclasses/comment.py
--rw-rw-rw-   0        0        0     7806 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/dataclasses/event.py
--rw-rw-rw-   0        0        0     1300 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/dataclasses/event_response.py
--rw-rw-rw-   0        0        0     9314 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/dataclasses/image.py
--rw-rw-rw-   0        0        0     7413 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/dataclasses/invention.py
--rw-rw-rw-   0        0        0     1371 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/dataclasses/invention_version.py
--rw-rw-rw-   0        0        0      740 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/dataclasses/loading_screen.py
--rw-rw-rw-   0        0        0      694 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/dataclasses/progression.py
--rw-rw-rw-   0        0        0      821 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/dataclasses/promo_external_content.py
--rw-rw-rw-   0        0        0     1679 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/dataclasses/role.py
--rw-rw-rw-   0        0        0    11138 2023-05-26 13:30:17.000000 recnetpy-0.1.49/src/recnetpy/dataclasses/room.py
--rw-rw-rw-   0        0        0      852 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/dataclasses/score.py
--rw-rw-rw-   0        0        0     2177 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/dataclasses/subroom.py
--rw-rw-rw-   0        0        0      701 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/dataclasses/tag.py
-drwxrwxrwx   0        0        0        0 2023-06-16 07:53:53.314199 recnetpy-0.1.49/src/recnetpy/managers/
--rw-rw-rw-   0        0        0      252 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/managers/__init__.py
--rw-rw-rw-   0        0        0     4175 2023-06-16 07:50:54.000000 recnetpy-0.1.49/src/recnetpy/managers/account_manager.py
--rw-rw-rw-   0        0        0     2035 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/managers/base_manager.py
--rw-rw-rw-   0        0        0     5380 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/managers/event_manager.py
--rw-rw-rw-   0        0        0     7463 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/managers/image_manager.py
--rw-rw-rw-   0        0        0     3578 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/managers/invention_manager.py
--rw-rw-rw-   0        0        0     7202 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/managers/room_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-16 07:53:53.349224 recnetpy-0.1.49/src/recnetpy/misc/
--rw-rw-rw-   0        0        0      169 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/misc/__init__.py
--rw-rw-rw-   0        0        0    10958 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/misc/api_responses.py
--rw-rw-rw-   0        0        0      589 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/misc/bitmask_decode.py
--rw-rw-rw-   0        0        0      124 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/misc/constants.py
--rw-rw-rw-   0        0        0      458 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/misc/date_to_unix.py
--rw-rw-rw-   0        0        0      245 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/misc/stringify_bulk.py
--rw-rw-rw-   0        0        0      959 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/misc/variable_class.py
-drwxrwxrwx   0        0        0        0 2023-06-16 07:53:53.367533 recnetpy-0.1.49/src/recnetpy/rest/
--rw-rw-rw-   0        0        0       71 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/rest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 07:53:53.384280 recnetpy-0.1.49/src/recnetpy/rest/async_threads/
--rw-rw-rw-   0        0        0       83 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/rest/async_threads/__init__.py
--rw-rw-rw-   0        0        0     1244 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/rest/async_threads/async_thread.py
--rw-rw-rw-   0        0        0     1875 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/rest/async_threads/async_thread_pool.py
--rw-rw-rw-   0        0        0     1588 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/rest/async_threads/thread_task.py
-drwxrwxrwx   0        0        0        0 2023-06-16 07:53:53.408096 recnetpy-0.1.49/src/recnetpy/rest/exceptions/
--rw-rw-rw-   0        0        0      159 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/rest/exceptions/__init__.py
--rw-rw-rw-   0        0        0      213 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/rest/exceptions/bad_request.py
--rw-rw-rw-   0        0        0      474 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/rest/exceptions/http_error.py
--rw-rw-rw-   0        0        0      257 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/rest/exceptions/internal_server_error.py
--rw-rw-rw-   0        0        0      252 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/rest/exceptions/not_found.py
--rw-rw-rw-   0        0        0     2092 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/rest/http_client.py
--rw-rw-rw-   0        0        0     2632 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/rest/request.py
--rw-rw-rw-   0        0        0      397 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/rest/response.py
--rw-rw-rw-   0        0        0     1809 2023-05-26 12:49:51.000000 recnetpy-0.1.49/src/recnetpy/rest/route_builder.py
--rw-rw-rw-   0        0        0     2998 2023-06-16 07:50:44.000000 recnetpy-0.1.49/src/recnetpy/rest/route_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-16 07:53:53.171231 recnetpy-0.1.49/src/recnetpy.egg-info/
--rw-rw-rw-   0        0        0     3242 2023-06-16 07:53:53.000000 recnetpy-0.1.49/src/recnetpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2016 2023-06-16 07:53:53.000000 recnetpy-0.1.49/src/recnetpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 07:53:53.000000 recnetpy-0.1.49/src/recnetpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-16 07:53:53.000000 recnetpy-0.1.49/src/recnetpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-16 07:53:53.000000 recnetpy-0.1.49/src/recnetpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 11:23:42.783598 recnetpy-0.1.5/
+-rw-rw-rw-   0        0        0     1140 2023-05-26 12:49:51.000000 recnetpy-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     3241 2023-06-18 11:23:42.782599 recnetpy-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2672 2023-05-26 12:49:51.000000 recnetpy-0.1.5/README.md
+-rw-rw-rw-   0        0        0      714 2023-06-18 11:23:03.000000 recnetpy-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-18 11:23:42.783598 recnetpy-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-18 11:23:42.412109 recnetpy-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-18 11:23:42.438470 recnetpy-0.1.5/src/recnetpy/
+-rw-rw-rw-   0        0        0       26 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/__init__.py
+-rw-rw-rw-   0        0        0     1550 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/client.py
+drwxrwxrwx   0        0        0        0 2023-06-18 11:23:42.559610 recnetpy-0.1.5/src/recnetpy/dataclasses/
+-rw-rw-rw-   0        0        0      534 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/dataclasses/__init__.py
+-rw-rw-rw-   0        0        0    10007 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/dataclasses/account.py
+-rw-rw-rw-   0        0        0     1368 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/dataclasses/base.py
+-rw-rw-rw-   0        0        0     1011 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/dataclasses/comment.py
+-rw-rw-rw-   0        0        0     7806 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/dataclasses/event.py
+-rw-rw-rw-   0        0        0     1300 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/dataclasses/event_response.py
+-rw-rw-rw-   0        0        0     9314 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/dataclasses/image.py
+-rw-rw-rw-   0        0        0     7413 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/dataclasses/invention.py
+-rw-rw-rw-   0        0        0     1371 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/dataclasses/invention_version.py
+-rw-rw-rw-   0        0        0      740 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/dataclasses/loading_screen.py
+-rw-rw-rw-   0        0        0      694 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/dataclasses/progression.py
+-rw-rw-rw-   0        0        0      821 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/dataclasses/promo_external_content.py
+-rw-rw-rw-   0        0        0     1679 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/dataclasses/role.py
+-rw-rw-rw-   0        0        0    11138 2023-05-26 13:30:17.000000 recnetpy-0.1.5/src/recnetpy/dataclasses/room.py
+-rw-rw-rw-   0        0        0      852 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/dataclasses/score.py
+-rw-rw-rw-   0        0        0     2679 2023-06-18 11:11:30.000000 recnetpy-0.1.5/src/recnetpy/dataclasses/subroom.py
+-rw-rw-rw-   0        0        0      701 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/dataclasses/tag.py
+drwxrwxrwx   0        0        0        0 2023-06-18 11:23:42.645581 recnetpy-0.1.5/src/recnetpy/managers/
+-rw-rw-rw-   0        0        0      252 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/managers/__init__.py
+-rw-rw-rw-   0        0        0     4175 2023-06-16 07:50:54.000000 recnetpy-0.1.5/src/recnetpy/managers/account_manager.py
+-rw-rw-rw-   0        0        0     2035 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/managers/base_manager.py
+-rw-rw-rw-   0        0        0     5380 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/managers/event_manager.py
+-rw-rw-rw-   0        0        0     7463 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/managers/image_manager.py
+-rw-rw-rw-   0        0        0     3578 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/managers/invention_manager.py
+-rw-rw-rw-   0        0        0     7202 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/managers/room_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-18 11:23:42.690596 recnetpy-0.1.5/src/recnetpy/misc/
+-rw-rw-rw-   0        0        0      169 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/misc/__init__.py
+-rw-rw-rw-   0        0        0    10958 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/misc/api_responses.py
+-rw-rw-rw-   0        0        0      589 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/misc/bitmask_decode.py
+-rw-rw-rw-   0        0        0      124 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/misc/constants.py
+-rw-rw-rw-   0        0        0      458 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/misc/date_to_unix.py
+-rw-rw-rw-   0        0        0      245 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/misc/stringify_bulk.py
+-rw-rw-rw-   0        0        0      959 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/misc/variable_class.py
+drwxrwxrwx   0        0        0        0 2023-06-18 11:23:42.727591 recnetpy-0.1.5/src/recnetpy/rest/
+-rw-rw-rw-   0        0        0       71 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/rest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 11:23:42.753091 recnetpy-0.1.5/src/recnetpy/rest/async_threads/
+-rw-rw-rw-   0        0        0       83 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/rest/async_threads/__init__.py
+-rw-rw-rw-   0        0        0     1244 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/rest/async_threads/async_thread.py
+-rw-rw-rw-   0        0        0     1875 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/rest/async_threads/async_thread_pool.py
+-rw-rw-rw-   0        0        0     1588 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/rest/async_threads/thread_task.py
+drwxrwxrwx   0        0        0        0 2023-06-18 11:23:42.781602 recnetpy-0.1.5/src/recnetpy/rest/exceptions/
+-rw-rw-rw-   0        0        0      159 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/rest/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      213 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/rest/exceptions/bad_request.py
+-rw-rw-rw-   0        0        0      474 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/rest/exceptions/http_error.py
+-rw-rw-rw-   0        0        0      257 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/rest/exceptions/internal_server_error.py
+-rw-rw-rw-   0        0        0      252 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/rest/exceptions/not_found.py
+-rw-rw-rw-   0        0        0     2092 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/rest/http_client.py
+-rw-rw-rw-   0        0        0     2632 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/rest/request.py
+-rw-rw-rw-   0        0        0      397 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/rest/response.py
+-rw-rw-rw-   0        0        0     1809 2023-05-26 12:49:51.000000 recnetpy-0.1.5/src/recnetpy/rest/route_builder.py
+-rw-rw-rw-   0        0        0     2998 2023-06-16 07:50:44.000000 recnetpy-0.1.5/src/recnetpy/rest/route_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-18 11:23:42.460093 recnetpy-0.1.5/src/recnetpy.egg-info/
+-rw-rw-rw-   0        0        0     3241 2023-06-18 11:23:42.000000 recnetpy-0.1.5/src/recnetpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2016 2023-06-18 11:23:42.000000 recnetpy-0.1.5/src/recnetpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 11:23:42.000000 recnetpy-0.1.5/src/recnetpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-18 11:23:42.000000 recnetpy-0.1.5/src/recnetpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-18 11:23:42.000000 recnetpy-0.1.5/src/recnetpy.egg-info/top_level.txt
```

### Comparing `recnetpy-0.1.49/LICENSE` & `recnetpy-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/PKG-INFO` & `recnetpy-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recnetpy
-Version: 0.1.49
+Version: 0.1.5
 Summary: RecNetPy is an API wrapper built in Python for pulling data from RecNet.
 Author: RecNetBot Development
 Project-URL: Homepage, https://github.com/RecNetBot-Development/RecNetPy
 Project-URL: Bug Tracker, https://github.com/RecNetBot-Development/RecNetPy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `recnetpy-0.1.49/README.md` & `recnetpy-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/pyproject.toml` & `recnetpy-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "recnetpy"
-version = "0.1.49"
+version = "0.1.5"
 authors = [
     { name="RecNetBot Development"}
 ]
 description = "RecNetPy is an API wrapper built in Python for pulling data from RecNet."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `recnetpy-0.1.49/src/recnetpy/client.py` & `recnetpy-0.1.5/src/recnetpy/client.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/dataclasses/__init__.py` & `recnetpy-0.1.5/src/recnetpy/dataclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/dataclasses/account.py` & `recnetpy-0.1.5/src/recnetpy/dataclasses/account.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/dataclasses/base.py` & `recnetpy-0.1.5/src/recnetpy/dataclasses/base.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/dataclasses/comment.py` & `recnetpy-0.1.5/src/recnetpy/dataclasses/comment.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/dataclasses/event.py` & `recnetpy-0.1.5/src/recnetpy/dataclasses/event.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/dataclasses/event_response.py` & `recnetpy-0.1.5/src/recnetpy/dataclasses/event_response.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/dataclasses/image.py` & `recnetpy-0.1.5/src/recnetpy/dataclasses/image.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/dataclasses/invention.py` & `recnetpy-0.1.5/src/recnetpy/dataclasses/invention.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/dataclasses/invention_version.py` & `recnetpy-0.1.5/src/recnetpy/dataclasses/invention_version.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/dataclasses/loading_screen.py` & `recnetpy-0.1.5/src/recnetpy/dataclasses/loading_screen.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/dataclasses/progression.py` & `recnetpy-0.1.5/src/recnetpy/dataclasses/progression.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/dataclasses/promo_external_content.py` & `recnetpy-0.1.5/src/recnetpy/dataclasses/promo_external_content.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/dataclasses/role.py` & `recnetpy-0.1.5/src/recnetpy/dataclasses/role.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/dataclasses/room.py` & `recnetpy-0.1.5/src/recnetpy/dataclasses/room.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/dataclasses/score.py` & `recnetpy-0.1.5/src/recnetpy/dataclasses/score.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/dataclasses/subroom.py` & `recnetpy-0.1.5/src/recnetpy/dataclasses/subroom.py`

 * *Files 26% similar despite different names*

```diff
@@ -28,24 +28,37 @@
     name: str
     #: If true the room is a sandbox..
     is_sandbox: bool
     #: This is the max number of players allowed to join the rooom.
     max_players: int
     #: This is the visibilty of the image which has the possible value of ``['Private', 'Public', 'Unlisted']``.
     accessibility: str
+    #: The blob that contains the data
     data_blob: Optional[str]
+    #: The user who saved the last
     data_saved_at: Optional[int]
+    #: The latest save description for the subroom
+    description: Optional[str]
 
     def __init__(self, data: 'SubRoomResponse'):
+        if data.get("CurrentSave"):
+            description = data["CurrentSave"].get("Description")
+            saved_at = date_to_unix(data["CurrentSave"]["CreatedAt"])
+            saved_by = data["CurrentSave"].get("SavedByAccountId", 1)
+        else:
+            saved_at, saved_by, description = None, 1, None
+
         self.supports_join_in_progress = data['SupportsJoinInProgress']
         self.use_level_based_matchmaking = data['UseLevelBasedMatchmaking']
         self.use_age_based_matchmaking = data['UseAgeBasedMatchmaking']
         self.use_rec_royale_matchmaking = data['UseRecRoyaleMatchmaking']
         self.subroom_id = data['SubRoomId']
         self.room_id = data['RoomId']
         self.unity_scene_id = data['UnitySceneId']
         self.name = data['Name']
         self.data_blob = data.get("DataBlob", None)
-        self.data_saved_at = date_to_unix(data['DataSavedAt']) if 'DataSavedAt' in data else None
+        self.data_saved_at = saved_at
+        self.data_saved_by = saved_by
+        self.description = description
         self.is_sandbox = data['IsSandbox']
         self.max_players = data['MaxPlayers']
         self.accessibility = ACCESSIBILITY_DICT.get(data['Accessibility'])
```

### Comparing `recnetpy-0.1.49/src/recnetpy/dataclasses/tag.py` & `recnetpy-0.1.5/src/recnetpy/dataclasses/tag.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/managers/account_manager.py` & `recnetpy-0.1.5/src/recnetpy/managers/account_manager.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/managers/base_manager.py` & `recnetpy-0.1.5/src/recnetpy/managers/base_manager.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/managers/event_manager.py` & `recnetpy-0.1.5/src/recnetpy/managers/event_manager.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/managers/image_manager.py` & `recnetpy-0.1.5/src/recnetpy/managers/image_manager.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/managers/invention_manager.py` & `recnetpy-0.1.5/src/recnetpy/managers/invention_manager.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/managers/room_manager.py` & `recnetpy-0.1.5/src/recnetpy/managers/room_manager.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/misc/api_responses.py` & `recnetpy-0.1.5/src/recnetpy/misc/api_responses.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/misc/bitmask_decode.py` & `recnetpy-0.1.5/src/recnetpy/misc/bitmask_decode.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/misc/variable_class.py` & `recnetpy-0.1.5/src/recnetpy/misc/variable_class.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/rest/async_threads/async_thread.py` & `recnetpy-0.1.5/src/recnetpy/rest/async_threads/async_thread.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/rest/async_threads/async_thread_pool.py` & `recnetpy-0.1.5/src/recnetpy/rest/async_threads/async_thread_pool.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/rest/async_threads/thread_task.py` & `recnetpy-0.1.5/src/recnetpy/rest/async_threads/thread_task.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/rest/http_client.py` & `recnetpy-0.1.5/src/recnetpy/rest/http_client.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/rest/request.py` & `recnetpy-0.1.5/src/recnetpy/rest/request.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/rest/route_builder.py` & `recnetpy-0.1.5/src/recnetpy/rest/route_builder.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy/rest/route_manager.py` & `recnetpy-0.1.5/src/recnetpy/rest/route_manager.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.49/src/recnetpy.egg-info/PKG-INFO` & `recnetpy-0.1.5/src/recnetpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recnetpy
-Version: 0.1.49
+Version: 0.1.5
 Summary: RecNetPy is an API wrapper built in Python for pulling data from RecNet.
 Author: RecNetBot Development
 Project-URL: Homepage, https://github.com/RecNetBot-Development/RecNetPy
 Project-URL: Bug Tracker, https://github.com/RecNetBot-Development/RecNetPy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `recnetpy-0.1.49/src/recnetpy.egg-info/SOURCES.txt` & `recnetpy-0.1.5/src/recnetpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

