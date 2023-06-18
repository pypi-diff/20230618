# Comparing `tmp/web_ext_helper-1.0.6.tar.gz` & `tmp/web_ext_helper-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_ext_helper-1.0.6.tar", max compression
+gzip compressed data, was "web_ext_helper-1.0.7.tar", max compression
```

## Comparing `web_ext_helper-1.0.6.tar` & `web_ext_helper-1.0.7.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.0.6/LICENSE
--rw-r--r--   0        0        0      654 2023-06-18 15:12:47.246288 web_ext_helper-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     1754 2023-06-17 20:34:00.666577 web_ext_helper-1.0.6/README.md
--rw-r--r--   0        0        0    18615 2023-06-18 15:05:47.937969 web_ext_helper-1.0.6/web_ext_helper/web_ext_helper.py
--rw-r--r--   0        0        0     2325 1970-01-01 00:00:00.000000 web_ext_helper-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.0.7/LICENSE
+-rw-r--r--   0        0        0      654 2023-06-18 17:37:12.434008 web_ext_helper-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1754 2023-06-17 20:34:00.666577 web_ext_helper-1.0.7/README.md
+-rw-r--r--   0        0        0      237 2023-06-18 17:20:13.515316 web_ext_helper-1.0.7/web_ext_helper/classes.py
+-rw-r--r--   0        0        0      547 2023-06-18 17:36:56.873136 web_ext_helper-1.0.7/web_ext_helper/functions.py
+-rw-r--r--   0        0        0    17958 2023-06-18 17:37:01.118273 web_ext_helper-1.0.7/web_ext_helper/web_ext_helper.py
+-rw-r--r--   0        0        0     2325 1970-01-01 00:00:00.000000 web_ext_helper-1.0.7/PKG-INFO
```

### Comparing `web_ext_helper-1.0.6/LICENSE` & `web_ext_helper-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.0.6/pyproject.toml` & `web_ext_helper-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "web-ext-helper"
-version = "1.0.6"
+version = "1.0.7"
 description = "A simple cli tool that helps you building your web extensions."
 authors = ["AppSolves <appsolves@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "web_ext_helper"}]
 
 [tool.poetry.dependencies]
```

### Comparing `web_ext_helper-1.0.6/README.md` & `web_ext_helper-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.0.6/web_ext_helper/web_ext_helper.py` & `web_ext_helper-1.0.7/web_ext_helper/web_ext_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,60 +1,31 @@
 import os
-import jwt
 import json
 import time
 import shutil
 import typer
 import zipfile
 import rich.progress
 import requests as req
 import subprocess as sp
 from PIL import Image
 from dotenv import load_dotenv
 from appdirs import user_cache_dir
+from .functions import error, generate_jwt
+from .classes import bcolors
 
 cached_app_build_dir = f"{user_cache_dir('web-ext-helper', False)}/build"
 cached_app_data_env_dir = f"{user_cache_dir('web-ext-helper', False)}/data/.env"
 cached_app_dir = os.path.dirname(os.path.dirname(cached_app_build_dir))
 os.makedirs(cached_app_build_dir, exist_ok=True)
 os.makedirs(os.path.dirname(cached_app_data_env_dir), exist_ok=True)
 
 load_dotenv(cached_app_data_env_dir)
 
 
-class bcolors:
-    HEADER = "\033[95m"
-    OKBLUE = "\033[94m"
-    OKCYAN = "\033[96m"
-    OKGREEN = "\033[92m"
-    WARNING = "\033[93m"
-    FAIL = "\033[91m"
-    ENDC = "\033[0m"
-    BOLD = "\033[1m"
-    UNDERLINE = "\033[4m"
-
-
-def error(message: str):
-    typer.echo(f"{bcolors.FAIL}Error: {message}{bcolors.ENDC}", err=True)
-    raise typer.Exit(1)
-
-
-def generate_jwt(api_key, api_secret):
-    issued_at = int(time.time())
-    expiration = issued_at + 300
-    jwt_payload = {
-        "iss": api_key,
-        "jti": str(time.time()),
-        "iat": issued_at,
-        "exp": expiration,
-    }
-    jwt_token = jwt.encode(jwt_payload, api_secret, algorithm="HS256")
-    return jwt_token
-
-
 app = typer.Typer()
 typer.clear()
 
 try:
     with open("src/manifest.json", "r") as manifest_file:
         manifest_data = json.load(manifest_file)
```

### Comparing `web_ext_helper-1.0.6/PKG-INFO` & `web_ext_helper-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ext-helper
-Version: 1.0.6
+Version: 1.0.7
 Summary: A simple cli tool that helps you building your web extensions.
 License: GPL-3.0-or-later
 Author: AppSolves
 Author-email: appsolves@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

