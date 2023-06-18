# Comparing `tmp/callbackin-0.5.0.tar.gz` & `tmp/callbackin-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "callbackin-0.5.0.tar", max compression
+gzip compressed data, was "callbackin-0.6.0.tar", max compression
```

## Comparing `callbackin-0.5.0.tar` & `callbackin-0.6.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1535 2023-06-17 11:36:46.832824 callbackin-0.5.0/README.md
--rw-r--r--   0        0        0       21 2023-06-17 12:25:28.545417 callbackin-0.5.0/callbackin/__init__.py
--rw-r--r--   0        0        0       49 2023-06-17 11:29:59.539358 callbackin-0.5.0/callbackin/__main__.py
--rw-r--r--   0        0        0        0 2023-06-17 10:51:29.295912 callbackin-0.5.0/callbackin/handler/__init__.py
--rw-r--r--   0        0        0     2261 2023-06-17 12:25:13.371198 callbackin-0.5.0/callbackin/handler/callback.py
--rw-r--r--   0        0        0     1944 2023-06-17 11:55:24.500003 callbackin-0.5.0/callbackin/handler/login.py
--rw-r--r--   0        0        0     4813 2023-06-17 12:18:07.035407 callbackin-0.5.0/callbackin/main.py
--rw-r--r--   0        0        0        0 2023-06-17 10:51:29.286706 callbackin-0.5.0/callbackin/schemas/__init__.py
--rw-r--r--   0        0        0      210 2023-06-17 10:51:29.288644 callbackin-0.5.0/callbackin/schemas/callback.py
--rw-r--r--   0        0        0        0 2023-06-17 10:51:29.261151 callbackin-0.5.0/callbackin/utils/__init__.py
--rw-r--r--   0        0        0     1322 2023-06-17 11:08:57.376439 callbackin-0.5.0/callbackin/utils/config.py
--rw-r--r--   0        0        0     1493 2023-06-17 11:32:01.695647 callbackin-0.5.0/callbackin/utils/request.py
--rw-r--r--   0        0        0      440 2023-06-17 12:25:23.187309 callbackin-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2049 1970-01-01 00:00:00.000000 callbackin-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1535 2023-06-17 11:36:46.832824 callbackin-0.6.0/README.md
+-rw-r--r--   0        0        0       21 2023-06-18 07:09:47.051683 callbackin-0.6.0/callbackin/__init__.py
+-rw-r--r--   0        0        0       49 2023-06-17 11:29:59.539358 callbackin-0.6.0/callbackin/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-17 10:51:29.295912 callbackin-0.6.0/callbackin/handler/__init__.py
+-rw-r--r--   0        0        0     2261 2023-06-17 12:25:13.371198 callbackin-0.6.0/callbackin/handler/callback.py
+-rw-r--r--   0        0        0     1954 2023-06-18 07:09:18.773367 callbackin-0.6.0/callbackin/handler/login.py
+-rw-r--r--   0        0        0     4823 2023-06-18 07:09:22.999549 callbackin-0.6.0/callbackin/main.py
+-rw-r--r--   0        0        0        0 2023-06-17 10:51:29.286706 callbackin-0.6.0/callbackin/schemas/__init__.py
+-rw-r--r--   0        0        0      210 2023-06-17 10:51:29.288644 callbackin-0.6.0/callbackin/schemas/callback.py
+-rw-r--r--   0        0        0        0 2023-06-17 10:51:29.261151 callbackin-0.6.0/callbackin/utils/__init__.py
+-rw-r--r--   0        0        0     1409 2023-06-18 07:06:48.557196 callbackin-0.6.0/callbackin/utils/config.py
+-rw-r--r--   0        0        0     1677 2023-06-18 07:07:50.774615 callbackin-0.6.0/callbackin/utils/request.py
+-rw-r--r--   0        0        0      440 2023-06-18 07:09:38.885541 callbackin-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2049 1970-01-01 00:00:00.000000 callbackin-0.6.0/PKG-INFO
```

### Comparing `callbackin-0.5.0/README.md` & `callbackin-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `callbackin-0.5.0/callbackin/handler/callback.py` & `callbackin-0.6.0/callbackin/handler/callback.py`

 * *Files identical despite different names*

### Comparing `callbackin-0.5.0/callbackin/handler/login.py` & `callbackin-0.6.0/callbackin/handler/login.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from http.server import BaseHTTPRequestHandler, HTTPServer
 import threading
 import webbrowser
 import typer
 from callbackin.utils.config import is_authenticated, get_config, CONFIG_FILE
-from callbackin.utils.request import BASE_URL
+from callbackin.utils.request import get_base_url
 
 class CallbackHandler(BaseHTTPRequestHandler):
     token = None
 
     def log_request(self, code: int | str = "-", size: int | str = "-") -> None:
         pass
 
@@ -38,15 +38,15 @@
         self.server_thread.daemon = True
 
     def run(self):
         config = get_config()
         if not is_authenticated():
             self.server_thread.start()
             typer.echo("Login to GitHub")
-            webbrowser.open(f'{BASE_URL}/auth/github/login/cli')
+            webbrowser.open(f'{get_base_url()}/auth/github/login/cli')
             while CallbackHandler.get_token() is None:
                 pass
             typer.echo("Login successful")
             self.server.shutdown()
             self.server.server_close()
             config["DEFAULT"]["user_token"] = CallbackHandler.get_token()
             config["DEFAULT"]["is_authenticated"] = "True"
```

### Comparing `callbackin-0.5.0/callbackin/main.py` & `callbackin-0.6.0/callbackin/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typer
 from callbackin.handler.callback import CallbackHanler
 from callbackin.handler.login import LoginHandler
 from pathlib import Path
 from callbackin.schemas.callback import Callback
 from callbackin.utils.config import create_config, CONFIG_FILE, get_config, is_authenticated
-from callbackin.utils.request import post, get, delete, put, BASE_URL
+from callbackin.utils.request import post, get, delete, put, get_base_url
 from rich.table import Table
 from rich.console import Console
 
 
 
 APP_NAME = "callbackin"
 
@@ -61,15 +61,15 @@
     if response.status_code == 200:
         callbacks = response.json()
         table = Table("ID", "Name", "Local Endpoint", "Server Endpoint")
         for callback in callbacks:
             table.add_row(str(callback["id"]), 
                           callback["name"], 
                           callback["local_endpoint"],
-                          f"{BASE_URL}/handle/{callback['path']}"
+                          f"{get_base_url()}/handle/{callback['path']}"
                           )
         console = Console()
         console.print(table)
 
 
 
 @app.command("delete")
```

### Comparing `callbackin-0.5.0/callbackin/utils/config.py` & `callbackin-0.6.0/callbackin/utils/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import typer
 
 CONFIG_DIR = Path(typer.get_app_dir("callbackin"))
 CONFIG_FILE = CONFIG_DIR / "config.ini"
 
 
 def get_config() -> configparser.ConfigParser:
+    if not CONFIG_FILE.exists():
+        raise Exception("Config file does not exist")
     config = configparser.ConfigParser()
     config.read(CONFIG_FILE)
     return config
 
 
 def create_config(
     base_url: str,
```

### Comparing `callbackin-0.5.0/PKG-INFO` & `callbackin-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: callbackin
-Version: 0.5.0
+Version: 0.6.0
 Summary: 
 Author: ibrahim4529
 Author-email: ibrahim.hanif4529@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

