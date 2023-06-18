# Comparing `tmp/streamlit-base-extras-0.2.8.tar.gz` & `tmp/streamlit-base-extras-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-base-extras-0.2.8.tar", last modified: Thu Oct 27 02:14:46 2022, max compression
+gzip compressed data, was "streamlit-base-extras-0.2.9.tar", last modified: Thu Oct 27 12:44:03 2022, max compression
```

## Comparing `streamlit-base-extras-0.2.8.tar` & `streamlit-base-extras-0.2.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 kronosol  (1000) kronosol  (1000)        0 2022-10-27 02:14:46.720075 streamlit-base-extras-0.2.8/
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)     1326 2022-10-23 02:14:36.000000 streamlit-base-extras-0.2.8/LICENCE
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)       69 2022-10-23 03:26:34.000000 streamlit-base-extras-0.2.8/MANIFEST.in
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)     9945 2022-10-27 02:14:46.720075 streamlit-base-extras-0.2.8/PKG-INFO
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)     8511 2022-10-27 02:14:35.000000 streamlit-base-extras-0.2.8/README.md
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)     9193 2022-10-27 02:14:35.000000 streamlit-base-extras-0.2.8/README.rst
-drwxr-xr-x   0 kronosol  (1000) kronosol  (1000)        0 2022-10-27 02:14:46.710075 streamlit-base-extras-0.2.8/build_tools/
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)     4042 2022-10-23 09:35:20.000000 streamlit-base-extras-0.2.8/build_tools/README.template.md
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)     2093 2022-10-25 05:46:19.000000 streamlit-base-extras-0.2.8/build_tools/make_readme.py
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)       38 2022-10-27 02:14:46.720075 streamlit-base-extras-0.2.8/setup.cfg
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)     2775 2022-10-23 06:14:30.000000 streamlit-base-extras-0.2.8/setup.py
-drwxr-xr-x   0 kronosol  (1000) kronosol  (1000)        0 2022-10-27 02:14:46.710075 streamlit-base-extras-0.2.8/streamlit_base_extras.egg-info/
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)     9945 2022-10-27 02:14:46.000000 streamlit-base-extras-0.2.8/streamlit_base_extras.egg-info/PKG-INFO
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)     1713 2022-10-27 02:14:46.000000 streamlit-base-extras-0.2.8/streamlit_base_extras.egg-info/SOURCES.txt
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)        1 2022-10-27 02:14:46.000000 streamlit-base-extras-0.2.8/streamlit_base_extras.egg-info/dependency_links.txt
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)      350 2022-10-27 02:14:46.000000 streamlit-base-extras-0.2.8/streamlit_base_extras.egg-info/requires.txt
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)       16 2022-10-27 02:14:46.000000 streamlit-base-extras-0.2.8/streamlit_base_extras.egg-info/top_level.txt
-drwxr-xr-x   0 kronosol  (1000) kronosol  (1000)        0 2022-10-27 02:14:46.713408 streamlit-base-extras-0.2.8/streamlitextras/
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)      273 2022-10-27 02:11:23.000000 streamlit-base-extras-0.2.8/streamlitextras/__init__.py
-drwxr-xr-x   0 kronosol  (1000) kronosol  (1000)        0 2022-10-27 02:14:46.713408 streamlit-base-extras-0.2.8/streamlitextras/authenticator/
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)    32787 2022-10-27 02:14:21.000000 streamlit-base-extras-0.2.8/streamlitextras/authenticator/__init__.py
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)     1199 2022-10-21 23:08:14.000000 streamlit-base-extras-0.2.8/streamlitextras/authenticator/exceptions.py
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)     3399 2022-10-23 05:09:20.000000 streamlit-base-extras-0.2.8/streamlitextras/authenticator/user.py
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)     2221 2022-10-23 05:09:48.000000 streamlit-base-extras-0.2.8/streamlitextras/authenticator/utils.py
-drwxr-xr-x   0 kronosol  (1000) kronosol  (1000)        0 2022-10-27 02:14:46.713408 streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)     4885 2022-10-23 04:52:22.000000 streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/__init__.py
-drwxr-xr-x   0 kronosol  (1000) kronosol  (1000)        0 2022-10-27 02:14:46.706741 streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/frontend/
-drwxr-xr-x   0 kronosol  (1000) kronosol  (1000)        0 2022-10-27 02:14:46.713408 streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/frontend/build/
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)      859 2022-10-21 16:17:03.000000 streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/frontend/build/asset-manifest.json
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)     2076 2022-10-21 16:17:03.000000 streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/frontend/build/index.html
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)      564 2022-10-21 16:17:03.000000 streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/frontend/build/precache-manifest.d091de9fa4668477ba52acdbecc2c864.js
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)     1183 2022-10-21 16:17:03.000000 streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/frontend/build/service-worker.js
-drwxr-xr-x   0 kronosol  (1000) kronosol  (1000)        0 2022-10-27 02:14:46.706741 streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/frontend/build/static/
-drwxr-xr-x   0 kronosol  (1000) kronosol  (1000)        0 2022-10-27 02:14:46.720075 streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/frontend/build/static/js/
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)   461164 2022-10-21 16:17:03.000000 streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/frontend/build/static/js/2.2bc12ddb.chunk.js
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)     1432 2022-10-21 16:17:03.000000 streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/frontend/build/static/js/2.2bc12ddb.chunk.js.LICENSE.txt
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)  1266888 2022-10-21 16:17:03.000000 streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/frontend/build/static/js/2.2bc12ddb.chunk.js.map
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)      972 2022-10-21 16:17:03.000000 streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/frontend/build/static/js/main.a8b332f3.chunk.js
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)     3309 2022-10-21 16:17:03.000000 streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/frontend/build/static/js/main.a8b332f3.chunk.js.map
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)     1604 2022-10-21 16:17:03.000000 streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/frontend/build/static/js/runtime-main.41b280b5.js
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)     8323 2022-10-21 16:17:03.000000 streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/frontend/build/static/js/runtime-main.41b280b5.js.map
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)     9415 2022-10-22 00:27:14.000000 streamlit-base-extras-0.2.8/streamlitextras/helpers.py
-drwxr-xr-x   0 kronosol  (1000) kronosol  (1000)        0 2022-10-27 02:14:46.720075 streamlit-base-extras-0.2.8/streamlitextras/logger/
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)     4452 2022-10-23 04:54:20.000000 streamlit-base-extras-0.2.8/streamlitextras/logger/__init__.py
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)      207 2022-10-23 04:55:00.000000 streamlit-base-extras-0.2.8/streamlitextras/logger/firebasesink.py
-drwxr-xr-x   0 kronosol  (1000) kronosol  (1000)        0 2022-10-27 02:14:46.720075 streamlit-base-extras-0.2.8/streamlitextras/router/
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)     7239 2022-10-26 04:10:22.000000 streamlit-base-extras-0.2.8/streamlitextras/router/__init__.py
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)     4546 2022-10-23 08:55:42.000000 streamlit-base-extras-0.2.8/streamlitextras/storageservice.py
-drwxr-xr-x   0 kronosol  (1000) kronosol  (1000)        0 2022-10-27 02:14:46.720075 streamlit-base-extras-0.2.8/streamlitextras/threader/
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)     4430 2022-10-25 05:10:15.000000 streamlit-base-extras-0.2.8/streamlitextras/threader/__init__.py
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)        0 2022-10-22 02:03:44.000000 streamlit-base-extras-0.2.8/streamlitextras/threader/reruntrigger.py
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)     1857 2022-10-25 05:45:51.000000 streamlit-base-extras-0.2.8/streamlitextras/utils.py
--rw-r--r--   0 kronosol  (1000) kronosol  (1000)     4839 2022-10-26 04:09:37.000000 streamlit-base-extras-0.2.8/streamlitextras/webutils.py
+drwxr-xr-x   0 kronosol  (1000) kronosol  (1000)        0 2022-10-27 12:44:03.479750 streamlit-base-extras-0.2.9/
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)     1326 2022-10-23 02:14:36.000000 streamlit-base-extras-0.2.9/LICENCE
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)       69 2022-10-23 03:26:34.000000 streamlit-base-extras-0.2.9/MANIFEST.in
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)     9945 2022-10-27 12:44:03.479750 streamlit-base-extras-0.2.9/PKG-INFO
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)     8511 2022-10-27 12:43:45.000000 streamlit-base-extras-0.2.9/README.md
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)     9193 2022-10-27 12:43:46.000000 streamlit-base-extras-0.2.9/README.rst
+drwxr-xr-x   0 kronosol  (1000) kronosol  (1000)        0 2022-10-27 12:44:03.459750 streamlit-base-extras-0.2.9/build_tools/
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)     4042 2022-10-23 09:35:20.000000 streamlit-base-extras-0.2.9/build_tools/README.template.md
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)     2093 2022-10-25 05:46:19.000000 streamlit-base-extras-0.2.9/build_tools/make_readme.py
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)       38 2022-10-27 12:44:03.479750 streamlit-base-extras-0.2.9/setup.cfg
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)     2775 2022-10-23 06:14:30.000000 streamlit-base-extras-0.2.9/setup.py
+drwxr-xr-x   0 kronosol  (1000) kronosol  (1000)        0 2022-10-27 12:44:03.459750 streamlit-base-extras-0.2.9/streamlit_base_extras.egg-info/
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)     9945 2022-10-27 12:44:03.000000 streamlit-base-extras-0.2.9/streamlit_base_extras.egg-info/PKG-INFO
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)     1713 2022-10-27 12:44:03.000000 streamlit-base-extras-0.2.9/streamlit_base_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)        1 2022-10-27 12:44:03.000000 streamlit-base-extras-0.2.9/streamlit_base_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)      350 2022-10-27 12:44:03.000000 streamlit-base-extras-0.2.9/streamlit_base_extras.egg-info/requires.txt
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)       16 2022-10-27 12:44:03.000000 streamlit-base-extras-0.2.9/streamlit_base_extras.egg-info/top_level.txt
+drwxr-xr-x   0 kronosol  (1000) kronosol  (1000)        0 2022-10-27 12:44:03.463083 streamlit-base-extras-0.2.9/streamlitextras/
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)      273 2022-10-27 12:42:45.000000 streamlit-base-extras-0.2.9/streamlitextras/__init__.py
+drwxr-xr-x   0 kronosol  (1000) kronosol  (1000)        0 2022-10-27 12:44:03.463083 streamlit-base-extras-0.2.9/streamlitextras/authenticator/
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)    35514 2022-10-27 12:43:35.000000 streamlit-base-extras-0.2.9/streamlitextras/authenticator/__init__.py
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)     1199 2022-10-21 23:08:14.000000 streamlit-base-extras-0.2.9/streamlitextras/authenticator/exceptions.py
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)     4206 2022-10-27 11:35:53.000000 streamlit-base-extras-0.2.9/streamlitextras/authenticator/user.py
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)     2221 2022-10-23 05:09:48.000000 streamlit-base-extras-0.2.9/streamlitextras/authenticator/utils.py
+drwxr-xr-x   0 kronosol  (1000) kronosol  (1000)        0 2022-10-27 12:44:03.463083 streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)     4885 2022-10-23 04:52:22.000000 streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/__init__.py
+drwxr-xr-x   0 kronosol  (1000) kronosol  (1000)        0 2022-10-27 12:44:03.456417 streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/frontend/
+drwxr-xr-x   0 kronosol  (1000) kronosol  (1000)        0 2022-10-27 12:44:03.463083 streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/frontend/build/
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)      859 2022-10-21 16:17:03.000000 streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/frontend/build/asset-manifest.json
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)     2076 2022-10-21 16:17:03.000000 streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/frontend/build/index.html
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)      564 2022-10-21 16:17:03.000000 streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/frontend/build/precache-manifest.d091de9fa4668477ba52acdbecc2c864.js
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)     1183 2022-10-21 16:17:03.000000 streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/frontend/build/service-worker.js
+drwxr-xr-x   0 kronosol  (1000) kronosol  (1000)        0 2022-10-27 12:44:03.456417 streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/frontend/build/static/
+drwxr-xr-x   0 kronosol  (1000) kronosol  (1000)        0 2022-10-27 12:44:03.476416 streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/frontend/build/static/js/
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)   461164 2022-10-21 16:17:03.000000 streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/frontend/build/static/js/2.2bc12ddb.chunk.js
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)     1432 2022-10-21 16:17:03.000000 streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/frontend/build/static/js/2.2bc12ddb.chunk.js.LICENSE.txt
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)  1266888 2022-10-21 16:17:03.000000 streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/frontend/build/static/js/2.2bc12ddb.chunk.js.map
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)      972 2022-10-21 16:17:03.000000 streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/frontend/build/static/js/main.a8b332f3.chunk.js
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)     3309 2022-10-21 16:17:03.000000 streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/frontend/build/static/js/main.a8b332f3.chunk.js.map
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)     1604 2022-10-21 16:17:03.000000 streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/frontend/build/static/js/runtime-main.41b280b5.js
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)     8323 2022-10-21 16:17:03.000000 streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/frontend/build/static/js/runtime-main.41b280b5.js.map
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)     9415 2022-10-22 00:27:14.000000 streamlit-base-extras-0.2.9/streamlitextras/helpers.py
+drwxr-xr-x   0 kronosol  (1000) kronosol  (1000)        0 2022-10-27 12:44:03.476416 streamlit-base-extras-0.2.9/streamlitextras/logger/
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)     4452 2022-10-23 04:54:20.000000 streamlit-base-extras-0.2.9/streamlitextras/logger/__init__.py
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)      207 2022-10-23 04:55:00.000000 streamlit-base-extras-0.2.9/streamlitextras/logger/firebasesink.py
+drwxr-xr-x   0 kronosol  (1000) kronosol  (1000)        0 2022-10-27 12:44:03.476416 streamlit-base-extras-0.2.9/streamlitextras/router/
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)     7239 2022-10-26 04:10:22.000000 streamlit-base-extras-0.2.9/streamlitextras/router/__init__.py
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)     4546 2022-10-23 08:55:42.000000 streamlit-base-extras-0.2.9/streamlitextras/storageservice.py
+drwxr-xr-x   0 kronosol  (1000) kronosol  (1000)        0 2022-10-27 12:44:03.476416 streamlit-base-extras-0.2.9/streamlitextras/threader/
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)     4552 2022-10-27 03:15:31.000000 streamlit-base-extras-0.2.9/streamlitextras/threader/__init__.py
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)        0 2022-10-22 02:03:44.000000 streamlit-base-extras-0.2.9/streamlitextras/threader/reruntrigger.py
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)     1857 2022-10-25 05:45:51.000000 streamlit-base-extras-0.2.9/streamlitextras/utils.py
+-rw-r--r--   0 kronosol  (1000) kronosol  (1000)     4839 2022-10-26 04:09:37.000000 streamlit-base-extras-0.2.9/streamlitextras/webutils.py
```

### Comparing `streamlit-base-extras-0.2.8/LICENCE` & `streamlit-base-extras-0.2.9/LICENCE`

 * *Files identical despite different names*

### Comparing `streamlit-base-extras-0.2.8/PKG-INFO` & `streamlit-base-extras-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: streamlit-base-extras
-Version: 0.2.8
+Version: 0.2.9
 Summary: Make building with streamlit easier.
 Home-page: https://github.com/blipk/streamlitextras
-Download-URL: https://github.com/blipk/streamlitextras/archive/0.2.8.tar.gz
+Download-URL: https://github.com/blipk/streamlitextras/archive/0.2.9.tar.gz
 Author: blipk
 Author-email: blipk+@github.com
 License: MIT license
 Project-URL: Changelog, https://github.com/blipk/streamlitextras/commits/
 Project-URL: Documentation, https://streamlitextras.readthedocs.io/en/stable/index.html
 Keywords: streamlitextras,streamlit,router,authenticator,javascript,cookie,thread
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `streamlit-base-extras-0.2.8/README.md` & `streamlit-base-extras-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-base-extras-0.2.8/README.rst` & `streamlit-base-extras-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `streamlit-base-extras-0.2.8/build_tools/README.template.md` & `streamlit-base-extras-0.2.9/build_tools/README.template.md`

 * *Files identical despite different names*

### Comparing `streamlit-base-extras-0.2.8/build_tools/make_readme.py` & `streamlit-base-extras-0.2.9/build_tools/make_readme.py`

 * *Files identical despite different names*

### Comparing `streamlit-base-extras-0.2.8/setup.py` & `streamlit-base-extras-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `streamlit-base-extras-0.2.8/streamlit_base_extras.egg-info/PKG-INFO` & `streamlit-base-extras-0.2.9/streamlit_base_extras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: streamlit-base-extras
-Version: 0.2.8
+Version: 0.2.9
 Summary: Make building with streamlit easier.
 Home-page: https://github.com/blipk/streamlitextras
-Download-URL: https://github.com/blipk/streamlitextras/archive/0.2.8.tar.gz
+Download-URL: https://github.com/blipk/streamlitextras/archive/0.2.9.tar.gz
 Author: blipk
 Author-email: blipk+@github.com
 License: MIT license
 Project-URL: Changelog, https://github.com/blipk/streamlitextras/commits/
 Project-URL: Documentation, https://streamlitextras.readthedocs.io/en/stable/index.html
 Keywords: streamlitextras,streamlit,router,authenticator,javascript,cookie,thread
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `streamlit-base-extras-0.2.8/streamlit_base_extras.egg-info/SOURCES.txt` & `streamlit-base-extras-0.2.9/streamlit_base_extras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `streamlit-base-extras-0.2.8/streamlitextras/authenticator/__init__.py` & `streamlit-base-extras-0.2.9/streamlitextras/authenticator/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import jwt
 import pytz
 import dateutil.parser
 from types import ModuleType
-from typing import Union, Optional, Tuple, TypeVar, Type
+from typing import Union, Optional, Tuple, TypeVar, Type, Callable
 from datetime import datetime, timedelta
 
 import streamlit as st
 from streamlit.delta_generator import DeltaGenerator
 from streamlitextras.logger import log
 from streamlitextras.utils import repr_
 from streamlitextras.authenticator.user import User
@@ -19,18 +19,18 @@
 import requests
 import pyrebase
 import firebase_admin
 from firebase_admin import auth as service_auth
 from streamlitextras.helpers import custom_html
 
 config = st.secrets["firebase"]
-firebase = pyrebase.initialize_app(config)
-auth = firebase.auth()
-db = firebase.database()
-storage = firebase.storage()
+pyrebase = pyrebase.initialize_app(config)
+auth = pyrebase.auth()
+db = pyrebase.database()
+storage = pyrebase.storage()
 
 # PyPI doesn't contain the latest git commits for pyrebase4
 def update_profile(id_token, display_name = None, photo_url=None, delete_attribute = None, *args):
     """
     Pyrebase on PyPI seems to be missing latest commits - adding this in here.
     https://firebase.google.com/docs/reference/rest/auth#section-update-profile
     """
@@ -223,14 +223,16 @@
         if type(expiry_date) is not datetime:
             expiry_date = datetime.fromtimestamp(expiry_date, tz=pytz.UTC)
 
         user = self.user_class(self, **firebase_data)
         self.last_user = user
         token_expiry_time = expiry_date.astimezone(tz=pytz.UTC)
         cookie_expiry_time = expiry_date.astimezone(tz=pytz.timezone(self.user_tz))
+        # token_expiry_time_delta = cookie_expiry_time.timestamp() - datetime.now(pytz.UTC).timestamp()
+        # session_cookie = service_auth.create_session_cookie(user.idToken, expires_in=token_expiry_time_delta)
         token = self._token_encode(user, token_expiry_time)
         st.session_state["authentication_token"] = token
         st.session_state[self.session_name] = user
         self.cookie_manager.set(self.cookie_name, token, expires_at=cookie_expiry_time)
         log.success(f"Created session {user}")
 
         return user
@@ -350,14 +352,44 @@
         if "account_info" not in firebase_token:
             error = AuthException("No account_info in decoded cookie token")
             return (self._revoke_auth(error), error, token_decoded)
         if firebase_token["registered"] is False:
             error = AuthException("Account with unverified email shouldn't have cookie")
             return (self._revoke_auth(error), error, token_decoded)
 
+        # try:
+        #     decoded_claims = service_auth.verify_session_cookie(session_cookie, check_revoked=True)
+        # except service_auth.InvalidSessionCookieError as e:
+        #      error = e
+        #      return (self._revoke_auth(error), error, token_decoded)
+
+        # try:
+        #     decoded_claims = service_auth.verify_id_token(firebase_token["idToken"], check_revoke=True)
+        # except ValueError:
+        #     error = e # Invalid token format
+        #     return (self._revoke_auth(error), error, token_decoded)
+        # except service_auth.InvalidIdTokenError as e:
+        #     error = e
+        #     # Refresh here
+        # except service_auth.ExpiredIdTokenError as e:
+        #     error = e
+        #     return (self._revoke_auth(error), error, token_decoded)
+        # except service_auth.RevokedIdTokenError as e:
+        #     error = e
+        #     return (self._revoke_auth(error), error, token_decoded)
+        # except service_auth.CertificateFetchError as e:
+        #     error = e
+        #     return (self._revoke_auth(error), error, token_decoded)
+        # except service_auth.UserDisabledError as e:
+        #     error = e
+        #     return (self._revoke_auth(error), error, token_decoded)
+        # if datetime.now(pytz.UTC) - decoded_claims['auth_time'] < self.session_expiry_seconds:
+        #     error = AuthException(f"old session id token {decoded_claims}")
+        #     return (self._revoke_auth(error), error, token_decoded)
+
         cookie_account_info = firebase_token["account_info"]
         utcnow = datetime.now(pytz.UTC)
         valid_since_datetime = datetime.fromtimestamp(int(cookie_account_info["users"][0]["validSince"]), tz=pytz.UTC)
         valid_since_seconds = utcnow.timestamp() - valid_since_datetime.timestamp()
         last_login_datetime = datetime.fromtimestamp(float(cookie_account_info["users"][0]["lastLoginAt"][:10] + '.' + cookie_account_info["users"][0]["lastLoginAt"][-3]), tz=pytz.UTC)
         last_login_age_seconds = utcnow.timestamp() - last_login_datetime.timestamp()
         last_refresh_datetime = dateutil.parser.isoparse(cookie_account_info["users"][0]["lastRefreshAt"])
@@ -457,15 +489,20 @@
                 st.button("Resend verification email", on_click=self._resend_verification, args=(res["idToken"],))
 
         if res and not error:
             if account_info:
                 account_info["users"][0]["passwordHash"] = ""
                 res["account_info"] = account_info
                 user = self._create_session(res)
-                log.success(f"""{account_info["users"][0]["email"]} logged in with password""")
+                log.success(f"""{user.email} logged in with password""")
+                if user.is_admin:
+                    service_auth.set_custom_user_claims(user.localId, {'admin': True})
+                    log.success(f"""Welcome {user.displayName}""")
+                if user.is_developer:
+                    service_auth.set_custom_user_claims(user.localId, {'devops': True})
             else:
                 error = LoginError("Error retrieving account info")
 
         return (user, res, error)
 
     def _resend_verification(self, user_id_token: str) -> Tuple[Optional[dict], Optional[AuthException]]:
         """
@@ -514,20 +551,29 @@
             raise ValueError("Location must be a streamlit DeltaGenerator (st container object such as st.sidebar) or the global st module.")
 
         if button_location.button(button_name, disabled=disabled, on_click=self._revoke_auth, args=(AuthException("Logout requested"), disabled,)):
             return True
 
         return False
 
-    def login(self, form_name: str, form_location: Union[DeltaGenerator, ModuleType] = st) -> Tuple[Optional[UserInherited], dict, Optional[LoginError]]:
+    def login(self, form_name: str,
+              form_location: Union[DeltaGenerator, ModuleType] = st,
+              success_callback: Optional[Callable] = None,
+              cb_args: Optional[tuple] = None,
+              cb_kwargs: Optional[dict] = None) -> Tuple[Optional[UserInherited], dict, Optional[LoginError]]:
         """
         Creates a login widget.
 
         :param str form_name: The rendered name of the login form.
         :param Union[DeltaGenerator, ModuleType] form_location: The streamlit container to place the form. Either global `st` or a st container object such as st.sidebar.
+        :param Callable success_callback:
+            Optional function to call if a user is created without error.
+            Will be passed a kwargs login_return which will be the same tuple returned from this login function.
+        :param cb_args: Extra args for success_callback
+        :param cb_kwargs: Extra keyword args for success_callback
 
         :returns: 3 element tuple containing the a User class if one was created, response from the firebase calls, and/or any errors
         """
         if not isinstance(form_location, DeltaGenerator) and form_location != st:
             raise ValueError("Location must be a streamlit DeltaGenerator (st container object such as st.sidebar) or the global st module.")
 
         res = None
@@ -552,14 +598,16 @@
             if login_form.form_submit_button("Login"):
                 if len(email) == 0:
                     error = LoginError("Please enter an email")
                 elif len(password) == 0:
                     error = LoginError("Please enter a password")
                 else:
                     user, res, error = self._check_credentials(email, password)
+                    if user and not error and success_callback and callable(success_callback):
+                        success_callback(*cb_args, login_return=(user, res, error,), **cb_kwargs)
 
             login_form.form_submit_button("Register", on_click=self.set_form, args=("register",))
             login_form.form_submit_button("Forgot password?", on_click=self.set_form, args=("reset_password",))
 
         return (user, res, error)
 
     def register_user(self, form_name: str, form_location: Union[DeltaGenerator, ModuleType] = st) -> Tuple[Optional[dict], Optional[RegisterError]]:
```

### Comparing `streamlit-base-extras-0.2.8/streamlitextras/authenticator/exceptions.py` & `streamlit-base-extras-0.2.9/streamlitextras/authenticator/exceptions.py`

 * *Files identical despite different names*

### Comparing `streamlit-base-extras-0.2.8/streamlitextras/authenticator/utils.py` & `streamlit-base-extras-0.2.9/streamlitextras/authenticator/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/__init__.py` & `streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/frontend/build/asset-manifest.json` & `streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/frontend/build/index.html` & `streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/frontend/build/precache-manifest.d091de9fa4668477ba52acdbecc2c864.js` & `streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/frontend/build/precache-manifest.d091de9fa4668477ba52acdbecc2c864.js`

 * *Files identical despite different names*

### Comparing `streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/frontend/build/service-worker.js` & `streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/frontend/build/static/js/2.2bc12ddb.chunk.js` & `streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/frontend/build/static/js/2.2bc12ddb.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/frontend/build/static/js/2.2bc12ddb.chunk.js.LICENSE.txt` & `streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/frontend/build/static/js/2.2bc12ddb.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/frontend/build/static/js/2.2bc12ddb.chunk.js.map` & `streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/frontend/build/static/js/2.2bc12ddb.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/frontend/build/static/js/main.a8b332f3.chunk.js` & `streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/frontend/build/static/js/main.a8b332f3.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/frontend/build/static/js/main.a8b332f3.chunk.js.map` & `streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/frontend/build/static/js/main.a8b332f3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/frontend/build/static/js/runtime-main.41b280b5.js` & `streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/frontend/build/static/js/runtime-main.41b280b5.js`

 * *Files identical despite different names*

### Comparing `streamlit-base-extras-0.2.8/streamlitextras/cookiemanager/frontend/build/static/js/runtime-main.41b280b5.js.map` & `streamlit-base-extras-0.2.9/streamlitextras/cookiemanager/frontend/build/static/js/runtime-main.41b280b5.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-base-extras-0.2.8/streamlitextras/helpers.py` & `streamlit-base-extras-0.2.9/streamlitextras/helpers.py`

 * *Files identical despite different names*

### Comparing `streamlit-base-extras-0.2.8/streamlitextras/logger/__init__.py` & `streamlit-base-extras-0.2.9/streamlitextras/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-base-extras-0.2.8/streamlitextras/router/__init__.py` & `streamlit-base-extras-0.2.9/streamlitextras/router/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-base-extras-0.2.8/streamlitextras/storageservice.py` & `streamlit-base-extras-0.2.9/streamlitextras/storageservice.py`

 * *Files identical despite different names*

### Comparing `streamlit-base-extras-0.2.8/streamlitextras/threader/__init__.py` & `streamlit-base-extras-0.2.9/streamlitextras/threader/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import time
 import threading
 from . import reruntrigger
 from streamlit.runtime.scriptrunner import add_script_run_ctx, get_script_run_ctx, RerunException
-from typing import Callable
+from typing import Callable, Optional
 
 # script_dir = os.path.dirname(os.path.realpath(__file__))
 script_dir = os.getcwd()
 trigger_file_path = os.path.join(script_dir, "reruntrigger.py")
 if not os.path.exists(trigger_file_path):
     with open(trigger_file_path, "w") as f:
         f.write(f"timestamp = {time.time()}")
@@ -18,15 +18,15 @@
     """
     Returns the seconds since last writing the trigger file
     """
     modified_time = os.path.getmtime(trigger_file_path)
     modified_time_seconds = time.time() - modified_time
     return modified_time_seconds
 
-def trigger_rerun(last_write_margin: int = 1, delay: int = 0):
+def trigger_rerun(last_write_margin: int = 1, delay: int = 0) -> None:
     """
     Triggers treamlit to rerun the current page state.
     runOnSave must be set to true in config.toml
 
     :param int last_write_margin:
         If the file was modified less than this many seconds ago, the rerun will not be performed
     :param int delay: sleep for this many seconds before writing the rerun trigger
@@ -44,30 +44,30 @@
     # https://discuss.streamlit.io/t/how-to-run-a-subprocess-programs-using-thread-inside-streamlit/2440/2
     # https://discuss.streamlit.io/t/how-to-monitor-the-filesystem-and-have-streamlit-updated-when-some-files-are-modified/822/3
 
 def thread_wrapper(thread_func,
                 rerun_st = True,
                 last_write_margin: int = 1,
                 delay: int = 0,
-                *args, **kwargs):
+                *args, **kwargs) -> None:
     """
     Wrapper for running thread functions
     For parameters see streamlit_thread() and trigger_rerun()
     """
     # print("Hashseed in thread:", os.environ.get("PYTHONHASHSEED", False))
     thread_func(*args, **kwargs)
     if rerun_st == True:
         trigger_rerun(last_write_margin, delay)
 
 def streamlit_thread(thread_func: Callable,
                     args: tuple = (),
                     kwargs: dict = {},
                     rerun_st: bool = True,
                     last_write_margin: int = 1,
-                    delay: int = 0):
+                    delay: int = 0) -> str:
     """
     Spawns and starts a threading.Thread that runs thread_func with the passed args and kwargs
 
     :param Callable thread_func: The function to run in the thread
     :param tuple args: The args to pass to the function in the thread
     :param dict kwargs: The kwargs to pass to the function in the thread
     :param bool rerun_st: Whether to rerun streamlit after the thread function finishes
@@ -78,20 +78,21 @@
     args = (thread_func, rerun_st, last_write_margin, delay, *args)
     thread = PropagatingThread(target=thread_wrapper, args=args, kwargs=kwargs)
     add_script_run_ctx(thread, get_script_run_ctx())
     time.sleep(0.1)
     thread.start()
     return thread.name
 
-def get_thread(thread_name):
+def get_thread(thread_name) -> Optional[threading.Thread]:
     """
     Gets the threading.Thread instance thats name attribute matches thread_name
 
-    :param thread_name:
-        The name attribute of the thread to look for, or None if it's not found.
+    :param thread_name: The name attribute of the thread to look for.
+
+    :returns: The threading.Thread or None if theres no thread with the supplied thread_name
     """
     threads = threading.enumerate()
     target_thread = None
     for thread in threads:
         if thread.name == thread_name:
             target_thread = thread
             break
```

### Comparing `streamlit-base-extras-0.2.8/streamlitextras/utils.py` & `streamlit-base-extras-0.2.9/streamlitextras/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit-base-extras-0.2.8/streamlitextras/webutils.py` & `streamlit-base-extras-0.2.9/streamlitextras/webutils.py`

 * *Files identical despite different names*

