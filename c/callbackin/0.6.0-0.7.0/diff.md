# Comparing `tmp/callbackin-0.6.0.tar.gz` & `tmp/callbackin-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "callbackin-0.6.0.tar", max compression
+gzip compressed data, was "callbackin-0.7.0.tar", max compression
```

## Comparing `callbackin-0.6.0.tar` & `callbackin-0.7.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1535 2023-06-17 11:36:46.832824 callbackin-0.6.0/README.md
--rw-r--r--   0        0        0       21 2023-06-18 07:09:47.051683 callbackin-0.6.0/callbackin/__init__.py
--rw-r--r--   0        0        0       49 2023-06-17 11:29:59.539358 callbackin-0.6.0/callbackin/__main__.py
--rw-r--r--   0        0        0        0 2023-06-17 10:51:29.295912 callbackin-0.6.0/callbackin/handler/__init__.py
--rw-r--r--   0        0        0     2261 2023-06-17 12:25:13.371198 callbackin-0.6.0/callbackin/handler/callback.py
--rw-r--r--   0        0        0     1954 2023-06-18 07:09:18.773367 callbackin-0.6.0/callbackin/handler/login.py
--rw-r--r--   0        0        0     4823 2023-06-18 07:09:22.999549 callbackin-0.6.0/callbackin/main.py
--rw-r--r--   0        0        0        0 2023-06-17 10:51:29.286706 callbackin-0.6.0/callbackin/schemas/__init__.py
--rw-r--r--   0        0        0      210 2023-06-17 10:51:29.288644 callbackin-0.6.0/callbackin/schemas/callback.py
--rw-r--r--   0        0        0        0 2023-06-17 10:51:29.261151 callbackin-0.6.0/callbackin/utils/__init__.py
--rw-r--r--   0        0        0     1409 2023-06-18 07:06:48.557196 callbackin-0.6.0/callbackin/utils/config.py
--rw-r--r--   0        0        0     1677 2023-06-18 07:07:50.774615 callbackin-0.6.0/callbackin/utils/request.py
--rw-r--r--   0        0        0      440 2023-06-18 07:09:38.885541 callbackin-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2049 1970-01-01 00:00:00.000000 callbackin-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1535 2023-06-17 11:36:46.832824 callbackin-0.7.0/README.md
+-rw-r--r--   0        0        0       21 2023-06-18 07:13:27.350991 callbackin-0.7.0/callbackin/__init__.py
+-rw-r--r--   0        0        0       49 2023-06-17 11:29:59.539358 callbackin-0.7.0/callbackin/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-17 10:51:29.295912 callbackin-0.7.0/callbackin/handler/__init__.py
+-rw-r--r--   0        0        0     2261 2023-06-17 12:25:13.371198 callbackin-0.7.0/callbackin/handler/callback.py
+-rw-r--r--   0        0        0     1954 2023-06-18 07:09:18.773367 callbackin-0.7.0/callbackin/handler/login.py
+-rw-r--r--   0        0        0     4823 2023-06-18 07:09:22.999549 callbackin-0.7.0/callbackin/main.py
+-rw-r--r--   0        0        0        0 2023-06-17 10:51:29.286706 callbackin-0.7.0/callbackin/schemas/__init__.py
+-rw-r--r--   0        0        0      210 2023-06-17 10:51:29.288644 callbackin-0.7.0/callbackin/schemas/callback.py
+-rw-r--r--   0        0        0        0 2023-06-17 10:51:29.261151 callbackin-0.7.0/callbackin/utils/__init__.py
+-rw-r--r--   0        0        0     1607 2023-06-18 07:12:34.471642 callbackin-0.7.0/callbackin/utils/config.py
+-rw-r--r--   0        0        0     1708 2023-06-18 07:11:10.976813 callbackin-0.7.0/callbackin/utils/request.py
+-rw-r--r--   0        0        0      440 2023-06-18 07:13:20.696615 callbackin-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2049 1970-01-01 00:00:00.000000 callbackin-0.7.0/PKG-INFO
```

### Comparing `callbackin-0.6.0/README.md` & `callbackin-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `callbackin-0.6.0/callbackin/handler/callback.py` & `callbackin-0.7.0/callbackin/handler/callback.py`

 * *Files identical despite different names*

### Comparing `callbackin-0.6.0/callbackin/handler/login.py` & `callbackin-0.7.0/callbackin/handler/login.py`

 * *Files identical despite different names*

### Comparing `callbackin-0.6.0/callbackin/main.py` & `callbackin-0.7.0/callbackin/main.py`

 * *Files identical despite different names*

### Comparing `callbackin-0.6.0/callbackin/utils/config.py` & `callbackin-0.7.0/callbackin/utils/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,21 @@
 
 CONFIG_DIR = Path(typer.get_app_dir("callbackin"))
 CONFIG_FILE = CONFIG_DIR / "config.ini"
 
 
 def get_config() -> configparser.ConfigParser:
     if not CONFIG_FILE.exists():
-        raise Exception("Config file does not exist")
+        create_config(
+            typer.prompt("Base URL"),
+            typer.prompt("MQTT Host"),
+            typer.prompt("MQTT Port"),
+            typer.prompt("MQTT Username"),
+            typer.prompt("MQTT Password", hide_input=True),
+        )
     config = configparser.ConfigParser()
     config.read(CONFIG_FILE)
     return config
 
 
 def create_config(
     base_url: str,
```

### Comparing `callbackin-0.6.0/callbackin/utils/request.py` & `callbackin-0.7.0/callbackin/utils/request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import requests
 from callbackin.utils.config import get_config
 
-config = get_config()
+
 
 def get_base_url() -> str:
+    config = get_config()
     if config["DEFAULT"]["base_url"] == "":
         raise Exception(
             "Base URL is not set, please run callbackin init")
     return config["DEFAULT"]["base_url"]
 
 
 def get_token() -> str:
+    config = get_config()
     if config["DEFAULT"]["user_token"] == "":
         raise Exception(
             "You are not authenticated, please login first, using callbackin login")
     return config["DEFAULT"]["user_token"]
 
 
 def get(path: str, params={}):
```

### Comparing `callbackin-0.6.0/PKG-INFO` & `callbackin-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: callbackin
-Version: 0.6.0
+Version: 0.7.0
 Summary: 
 Author: ibrahim4529
 Author-email: ibrahim.hanif4529@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

