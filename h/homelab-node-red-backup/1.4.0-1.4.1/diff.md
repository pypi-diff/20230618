# Comparing `tmp/homelab_node_red_backup-1.4.0.tar.gz` & `tmp/homelab_node_red_backup-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homelab_node_red_backup-1.4.0.tar", max compression
+gzip compressed data, was "homelab_node_red_backup-1.4.1.tar", max compression
```

## Comparing `homelab_node_red_backup-1.4.0.tar` & `homelab_node_red_backup-1.4.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1133 2023-06-18 13:49:32.050068 homelab_node_red_backup-1.4.0/LICENSE.md
--rw-r--r--   0        0        0     3213 2023-06-18 13:49:32.050068 homelab_node_red_backup-1.4.0/README.md
--rw-r--r--   0        0        0       46 2023-06-18 13:49:32.050068 homelab_node_red_backup-1.4.0/homelab_node_red_backup/__init__.py
--rw-r--r--   0        0        0     3385 2023-06-18 13:49:32.050068 homelab_node_red_backup-1.4.0/homelab_node_red_backup/__main__.py
--rw-r--r--   0        0        0       35 2023-06-18 13:49:32.050068 homelab_node_red_backup-1.4.0/homelab_node_red_backup/handler/__init__.py
--rw-r--r--   0        0        0     1758 2023-06-18 13:49:32.050068 homelab_node_red_backup-1.4.0/homelab_node_red_backup/handler/backup.py
--rw-r--r--   0        0        0      528 2023-06-18 13:49:32.050068 homelab_node_red_backup-1.4.0/homelab_node_red_backup/handler/check.py
--rw-r--r--   0        0        0      705 2023-06-18 13:49:32.050068 homelab_node_red_backup-1.4.0/homelab_node_red_backup/handler/flows.py
--rw-r--r--   0        0        0      565 2023-06-18 13:49:32.050068 homelab_node_red_backup-1.4.0/homelab_node_red_backup/handler/restore.py
--rw-r--r--   0        0        0     2152 2023-06-18 13:49:32.050068 homelab_node_red_backup-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     4052 1970-01-01 00:00:00.000000 homelab_node_red_backup-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1133 2023-06-18 15:46:41.072341 homelab_node_red_backup-1.4.1/LICENSE.md
+-rw-r--r--   0        0        0     3213 2023-06-18 15:46:41.072341 homelab_node_red_backup-1.4.1/README.md
+-rw-r--r--   0        0        0       46 2023-06-18 15:46:41.072341 homelab_node_red_backup-1.4.1/homelab_node_red_backup/__init__.py
+-rw-r--r--   0        0        0     3385 2023-06-18 15:46:41.072341 homelab_node_red_backup-1.4.1/homelab_node_red_backup/__main__.py
+-rw-r--r--   0        0        0       35 2023-06-18 15:46:41.072341 homelab_node_red_backup-1.4.1/homelab_node_red_backup/handler/__init__.py
+-rw-r--r--   0        0        0     1758 2023-06-18 15:46:41.072341 homelab_node_red_backup-1.4.1/homelab_node_red_backup/handler/backup.py
+-rw-r--r--   0        0        0      528 2023-06-18 15:46:41.072341 homelab_node_red_backup-1.4.1/homelab_node_red_backup/handler/check.py
+-rw-r--r--   0        0        0      786 2023-06-18 15:46:41.072341 homelab_node_red_backup-1.4.1/homelab_node_red_backup/handler/flows.py
+-rw-r--r--   0        0        0      785 2023-06-18 15:46:41.072341 homelab_node_red_backup-1.4.1/homelab_node_red_backup/handler/restore.py
+-rw-r--r--   0        0        0     2152 2023-06-18 15:46:41.072341 homelab_node_red_backup-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4052 1970-01-01 00:00:00.000000 homelab_node_red_backup-1.4.1/PKG-INFO
```

### Comparing `homelab_node_red_backup-1.4.0/LICENSE.md` & `homelab_node_red_backup-1.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `homelab_node_red_backup-1.4.0/README.md` & `homelab_node_red_backup-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `homelab_node_red_backup-1.4.0/homelab_node_red_backup/__main__.py` & `homelab_node_red_backup-1.4.1/homelab_node_red_backup/__main__.py`

 * *Files identical despite different names*

### Comparing `homelab_node_red_backup-1.4.0/homelab_node_red_backup/handler/backup.py` & `homelab_node_red_backup-1.4.1/homelab_node_red_backup/handler/backup.py`

 * *Files identical despite different names*

### Comparing `homelab_node_red_backup-1.4.0/homelab_node_red_backup/handler/check.py` & `homelab_node_red_backup-1.4.1/homelab_node_red_backup/handler/check.py`

 * *Files identical despite different names*

### Comparing `homelab_node_red_backup-1.4.0/homelab_node_red_backup/handler/flows.py` & `homelab_node_red_backup-1.4.1/homelab_node_red_backup/handler/flows.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,13 +8,16 @@
     """Gets the existing flows."""
     headers = {"Node-RED-API-Version": "v2"}
     if jwt_token is not None:
         headers["Authorization"] = f"Bearer {jwt_token}"
     try:
         flows_request = requests.get(f"{endpoint}/flows/", headers=headers)
         if not flows_request.ok:
-            click.echo(f"Could not get flows from Node-RED: {flows_request.text}")
+            click.echo(
+                f"Could not get flows from Node-RED: {flows_request.status_code}, "
+                + f"{flows_request.text}"
+            )
             raise click.Abort()
         return flows_request.json()
     except Exception as err:
         click.echo(f"Error performing request to Node-RED: {err}")
         raise click.Abort()
```

### Comparing `homelab_node_red_backup-1.4.0/homelab_node_red_backup/handler/restore.py` & `homelab_node_red_backup-1.4.1/homelab_node_red_backup/handler/restore.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,11 +6,17 @@
 
 def restore_backup(endpoint: str, jwt_token: Optional[str], flows: str):
     """Restores from a backup."""
     headers = {"Node-RED-API-Version": "v2", "Node-RED-Deployment-Type": "full"}
     if jwt_token is not None:
         headers["Authorization"] = f"Bearer {jwt_token}"
     try:
-        requests.post(f"{endpoint}/flows/", json=flows, headers=headers)
+        request = requests.post(f"{endpoint}/flows/", json=flows, headers=headers)
+        if not request.ok:
+            click.echo(
+                f"Could not push flows to Node-RED: {request.status_code}, "
+                + f"{request.text}"
+            )
+            raise click.Abort()
     except Exception as error:
         click.echo(f"Could not make request to Node-RED: {error}")
         raise click.Abort()
```

### Comparing `homelab_node_red_backup-1.4.0/pyproject.toml` & `homelab_node_red_backup-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "poetry-core"
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "homelab-node-red-backup"
-version = "1.4.0"
+version = "1.4.1"
 description = "Backup and Restore for Node-RED."
 license = "MIT"
 authors = [
     "Daniel Muehlbachler-Pietrzykowski <daniel.muehlbachler@niftyside.io>"
 ]
 readme = "README.md"
 repository = "https://github.com/muhlba91/onyx-client"
```

### Comparing `homelab_node_red_backup-1.4.0/PKG-INFO` & `homelab_node_red_backup-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homelab-node-red-backup
-Version: 1.4.0
+Version: 1.4.1
 Summary: Backup and Restore for Node-RED.
 Home-page: https://github.com/muhlba91/onyx-client
 License: MIT
 Keywords: node-red,homelab
 Author: Daniel Muehlbachler-Pietrzykowski
 Author-email: daniel.muehlbachler@niftyside.io
 Requires-Python: >=3.11,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: homelab-node-red-backup Version: 1.4.0 Summary:
+Metadata-Version: 2.1 Name: homelab-node-red-backup Version: 1.4.1 Summary:
 Backup and Restore for Node-RED. Home-page: https://github.com/muhlba91/onyx-
 client License: MIT Keywords: node-red,homelab Author: Daniel Muehlbachler-
 Pietrzykowski Author-email: daniel.muehlbachler@niftyside.io Requires-Python:
 >=3.11,<4.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
```

