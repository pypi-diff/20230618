# Comparing `tmp/cq23-1.9.3.tar.gz` & `tmp/cq23-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cq23-1.9.3.tar", last modified: Sat Jun 17 07:26:41 2023, max compression
+gzip compressed data, was "cq23-1.9.4.tar", last modified: Sat Jun 17 07:45:55 2023, max compression
```

## Comparing `cq23-1.9.3.tar` & `cq23-1.9.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:26:41.987405 cq23-1.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-17 07:26:41.987405 cq23-1.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-17 07:26:34.000000 cq23-1.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-17 07:26:34.000000 cq23-1.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-17 07:26:41.987405 cq23-1.9.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:26:41.983405 cq23-1.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:26:41.983405 cq23-1.9.3/src/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:26:34.000000 cq23-1.9.3/src/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-17 07:26:34.000000 cq23-1.9.3/src/admin/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-17 07:26:34.000000 cq23-1.9.3/src/admin/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-17 07:26:34.000000 cq23-1.9.3/src/admin/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:26:41.983405 cq23-1.9.3/src/check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:26:34.000000 cq23-1.9.3/src/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-17 07:26:34.000000 cq23-1.9.3/src/check/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:26:41.983405 cq23-1.9.3/src/cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:26:34.000000 cq23-1.9.3/src/cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-17 07:26:34.000000 cq23-1.9.3/src/cleanup/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:26:41.983405 cq23-1.9.3/src/cq23.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-17 07:26:41.000000 cq23-1.9.3/src/cq23.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-17 07:26:41.000000 cq23-1.9.3/src/cq23.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 07:26:41.000000 cq23-1.9.3/src/cq23.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-17 07:26:41.000000 cq23-1.9.3/src/cq23.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-17 07:26:41.000000 cq23-1.9.3/src/cq23.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-17 07:26:41.000000 cq23-1.9.3/src/cq23.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:26:41.983405 cq23-1.9.3/src/main/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:26:34.000000 cq23-1.9.3/src/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-17 07:26:34.000000 cq23-1.9.3/src/main/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-17 07:26:34.000000 cq23-1.9.3/src/main/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:26:41.983405 cq23-1.9.3/src/new_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:26:34.000000 cq23-1.9.3/src/new_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-17 07:26:34.000000 cq23-1.9.3/src/new_client/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:26:41.983405 cq23-1.9.3/src/replay/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:26:34.000000 cq23-1.9.3/src/replay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-17 07:26:34.000000 cq23-1.9.3/src/replay/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:26:41.987405 cq23-1.9.3/src/run_game/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:26:34.000000 cq23-1.9.3/src/run_game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-17 07:26:34.000000 cq23-1.9.3/src/run_game/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-17 07:26:34.000000 cq23-1.9.3/src/run_game/docker_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-17 07:26:34.000000 cq23-1.9.3/src/run_game/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:26:41.987405 cq23-1.9.3/src/web_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:26:34.000000 cq23-1.9.3/src/web_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-17 07:26:34.000000 cq23-1.9.3/src/web_server/flask_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:26:41.987405 cq23-1.9.3/src/zip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:26:34.000000 cq23-1.9.3/src/zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-17 07:26:34.000000 cq23-1.9.3/src/zip/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:55.296350 cq23-1.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-17 07:45:55.296350 cq23-1.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-17 07:45:47.000000 cq23-1.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-17 07:45:47.000000 cq23-1.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-17 07:45:55.296350 cq23-1.9.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:55.292350 cq23-1.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:55.296350 cq23-1.9.4/src/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:47.000000 cq23-1.9.4/src/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-17 07:45:47.000000 cq23-1.9.4/src/admin/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-17 07:45:47.000000 cq23-1.9.4/src/admin/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-17 07:45:47.000000 cq23-1.9.4/src/admin/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:55.296350 cq23-1.9.4/src/check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:47.000000 cq23-1.9.4/src/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-17 07:45:47.000000 cq23-1.9.4/src/check/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:55.296350 cq23-1.9.4/src/cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:47.000000 cq23-1.9.4/src/cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-17 07:45:47.000000 cq23-1.9.4/src/cleanup/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:55.296350 cq23-1.9.4/src/cq23.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-17 07:45:55.000000 cq23-1.9.4/src/cq23.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-17 07:45:55.000000 cq23-1.9.4/src/cq23.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 07:45:55.000000 cq23-1.9.4/src/cq23.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-17 07:45:55.000000 cq23-1.9.4/src/cq23.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-17 07:45:55.000000 cq23-1.9.4/src/cq23.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-17 07:45:55.000000 cq23-1.9.4/src/cq23.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:55.296350 cq23-1.9.4/src/main/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:47.000000 cq23-1.9.4/src/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-17 07:45:47.000000 cq23-1.9.4/src/main/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-17 07:45:47.000000 cq23-1.9.4/src/main/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:55.296350 cq23-1.9.4/src/new_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:47.000000 cq23-1.9.4/src/new_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-17 07:45:47.000000 cq23-1.9.4/src/new_client/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:55.296350 cq23-1.9.4/src/replay/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:47.000000 cq23-1.9.4/src/replay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-17 07:45:47.000000 cq23-1.9.4/src/replay/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:55.296350 cq23-1.9.4/src/run_game/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:47.000000 cq23-1.9.4/src/run_game/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-17 07:45:47.000000 cq23-1.9.4/src/run_game/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-17 07:45:47.000000 cq23-1.9.4/src/run_game/docker_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-17 07:45:47.000000 cq23-1.9.4/src/run_game/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:55.296350 cq23-1.9.4/src/web_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:47.000000 cq23-1.9.4/src/web_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-06-17 07:45:47.000000 cq23-1.9.4/src/web_server/flask_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:55.296350 cq23-1.9.4/src/zip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:45:47.000000 cq23-1.9.4/src/zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-17 07:45:47.000000 cq23-1.9.4/src/zip/command.py
```

### Comparing `cq23-1.9.3/PKG-INFO` & `cq23-1.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 1.9.3
+Version: 1.9.4
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-1.9.3/setup.cfg` & `cq23-1.9.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cq23
-version = 1.9.3
+version = 1.9.4
 author = CodeQuest
 author_email = info@codequest.club
 description = CLI Tools for CodeQuest 23
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CALED-Team/cq23-cli-utilities
 project_urls =
```

### Comparing `cq23-1.9.3/src/admin/aws.py` & `cq23-1.9.4/src/admin/aws.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.3/src/admin/builder.py` & `cq23-1.9.4/src/admin/builder.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.3/src/admin/worker.py` & `cq23-1.9.4/src/admin/worker.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.3/src/check/command.py` & `cq23-1.9.4/src/check/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.3/src/cleanup/command.py` & `cq23-1.9.4/src/cleanup/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.3/src/cq23.egg-info/PKG-INFO` & `cq23-1.9.4/src/cq23.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 1.9.3
+Version: 1.9.4
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-1.9.3/src/cq23.egg-info/SOURCES.txt` & `cq23-1.9.4/src/cq23.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cq23-1.9.3/src/main/command.py` & `cq23-1.9.4/src/main/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.3/src/main/utils.py` & `cq23-1.9.4/src/main/utils.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.3/src/new_client/command.py` & `cq23-1.9.4/src/new_client/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.3/src/replay/command.py` & `cq23-1.9.4/src/replay/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.3/src/run_game/command.py` & `cq23-1.9.4/src/run_game/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.3/src/run_game/docker_tools.py` & `cq23-1.9.4/src/run_game/docker_tools.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.3/src/run_game/gcs.py` & `cq23-1.9.4/src/run_game/gcs.py`

 * *Files identical despite different names*

### Comparing `cq23-1.9.3/src/web_server/flask_api.py` & `cq23-1.9.4/src/web_server/flask_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -96,14 +96,17 @@
     with open(response) as f:
         file_content = f.read()
 
     return jsonify({"message": "ok", "content": file_content})
 
 
 def start(replay_files_directory, port=2023, debug=False):
+    # This wait time here is implemented for the game server to have enough time to write a couple of the replay files
+    time.sleep(5)
+
     global ROOT_DIRECTORY, PORT
     ROOT_DIRECTORY = replay_files_directory
     PORT = port
 
     global SERVER
     SERVER = make_server("127.0.0.1", port, app)
     SERVER.serve_forever()
```

### Comparing `cq23-1.9.3/src/zip/command.py` & `cq23-1.9.4/src/zip/command.py`

 * *Files identical despite different names*

