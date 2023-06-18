# Comparing `tmp/homelab_node_red_backup-1.3.0.tar.gz` & `tmp/homelab_node_red_backup-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homelab_node_red_backup-1.3.0.tar", max compression
+gzip compressed data, was "homelab_node_red_backup-1.4.0.tar", max compression
```

## Comparing `homelab_node_red_backup-1.3.0.tar` & `homelab_node_red_backup-1.4.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1133 2023-06-18 13:05:44.937843 homelab_node_red_backup-1.3.0/LICENSE.md
--rw-r--r--   0        0        0     3042 2023-06-18 13:05:44.937843 homelab_node_red_backup-1.3.0/README.md
--rw-r--r--   0        0        0       46 2023-06-18 13:05:44.937843 homelab_node_red_backup-1.3.0/homelab_node_red_backup/__init__.py
--rw-r--r--   0        0        0     2186 2023-06-18 13:05:44.937843 homelab_node_red_backup-1.3.0/homelab_node_red_backup/__main__.py
--rw-r--r--   0        0        0       35 2023-06-18 13:05:44.937843 homelab_node_red_backup-1.3.0/homelab_node_red_backup/handler/__init__.py
--rw-r--r--   0        0        0     1658 2023-06-18 13:05:44.937843 homelab_node_red_backup-1.3.0/homelab_node_red_backup/handler/backup.py
--rw-r--r--   0        0        0      444 2023-06-18 13:05:44.937843 homelab_node_red_backup-1.3.0/homelab_node_red_backup/handler/check.py
--rw-r--r--   0        0        0      705 2023-06-18 13:05:44.937843 homelab_node_red_backup-1.3.0/homelab_node_red_backup/handler/flows.py
--rw-r--r--   0        0        0      565 2023-06-18 13:05:44.937843 homelab_node_red_backup-1.3.0/homelab_node_red_backup/handler/restore.py
--rw-r--r--   0        0        0     2152 2023-06-18 13:05:44.937843 homelab_node_red_backup-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     3881 1970-01-01 00:00:00.000000 homelab_node_red_backup-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1133 2023-06-18 13:49:32.050068 homelab_node_red_backup-1.4.0/LICENSE.md
+-rw-r--r--   0        0        0     3213 2023-06-18 13:49:32.050068 homelab_node_red_backup-1.4.0/README.md
+-rw-r--r--   0        0        0       46 2023-06-18 13:49:32.050068 homelab_node_red_backup-1.4.0/homelab_node_red_backup/__init__.py
+-rw-r--r--   0        0        0     3385 2023-06-18 13:49:32.050068 homelab_node_red_backup-1.4.0/homelab_node_red_backup/__main__.py
+-rw-r--r--   0        0        0       35 2023-06-18 13:49:32.050068 homelab_node_red_backup-1.4.0/homelab_node_red_backup/handler/__init__.py
+-rw-r--r--   0        0        0     1758 2023-06-18 13:49:32.050068 homelab_node_red_backup-1.4.0/homelab_node_red_backup/handler/backup.py
+-rw-r--r--   0        0        0      528 2023-06-18 13:49:32.050068 homelab_node_red_backup-1.4.0/homelab_node_red_backup/handler/check.py
+-rw-r--r--   0        0        0      705 2023-06-18 13:49:32.050068 homelab_node_red_backup-1.4.0/homelab_node_red_backup/handler/flows.py
+-rw-r--r--   0        0        0      565 2023-06-18 13:49:32.050068 homelab_node_red_backup-1.4.0/homelab_node_red_backup/handler/restore.py
+-rw-r--r--   0        0        0     2152 2023-06-18 13:49:32.050068 homelab_node_red_backup-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4052 1970-01-01 00:00:00.000000 homelab_node_red_backup-1.4.0/PKG-INFO
```

### Comparing `homelab_node_red_backup-1.3.0/LICENSE.md` & `homelab_node_red_backup-1.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `homelab_node_red_backup-1.3.0/README.md` & `homelab_node_red_backup-1.4.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -39,19 +39,21 @@
 - `servers`: e.g. a Home Assistant server with an access token
 - `telegram bot`: Telegram bot with a token
 
 ## Usage
 
 The following commands are available, and all commands require the arguments `--endpoint`, and, optionally, `--jwt-token` set.
 
-- `check`: checks if data exists for a backup
+- `check`: checks if data exists for a backup (return code `0` if data exists, else `1`)
 - `backup`: creates a backup
   - requires: `--file`
 - `restore`: restores from a backup
   - requires: `--file`
+- `auto`: performs a `check` and either creates a backup to or restores a backup from the given `--file`
+  - requires: `--file`
 
 ### Examples
 
 ```bash
 # checking if data exists
 homelab-node-red-backup check -e http://localhost:1880 -jwt <TOKEN>
```

#### html2text {}

```diff
@@ -21,16 +21,18 @@
 Configuration The following arguments are available: - `--endpoint` / `-e`: the
 Node-RED endpoint - `--file` / `-f`: the JSON file - `--jwt-token` / `-jwt`:
 the JWT token to authenticate with ## Credentials Credentials are detected,
 retrieved, and merged to the output JSON file. The following credential types
 are recognized: - `servers`: e.g. a Home Assistant server with an access token
 - `telegram bot`: Telegram bot with a token ## Usage The following commands are
 available, and all commands require the arguments `--endpoint`, and,
-optionally, `--jwt-token` set. - `check`: checks if data exists for a backup -
-`backup`: creates a backup - requires: `--file` - `restore`: restores from a
-backup - requires: `--file` ### Examples ```bash # checking if data exists
-homelab-node-red-backup check -e http://localhost:1880 -jwt  # creating a
-backup homelab-node-red-backup backup -e http://localhost:1880 -jwt  -
-f backup.json # restoring from the backup homelab-node-red-backup restore -
+optionally, `--jwt-token` set. - `check`: checks if data exists for a backup
+(return code `0` if data exists, else `1`) - `backup`: creates a backup -
+requires: `--file` - `restore`: restores from a backup - requires: `--file` -
+`auto`: performs a `check` and either creates a backup to or restores a backup
+from the given `--file` - requires: `--file` ### Examples ```bash # checking if
+data exists homelab-node-red-backup check -e http://localhost:1880 -jwt  #
+creating a backup homelab-node-red-backup backup -e http://localhost:1880 -jwt
+-f backup.json # restoring from the backup homelab-node-red-backup restore -
 e http://localhost:1880 -jwt  -f backup.json ``` --- ## Supporting If you enjoy
 the application and want to support my efforts, please feel free to buy me a
 coffe. :) [Buy_Me_A_Coffee]
```

### Comparing `homelab_node_red_backup-1.3.0/homelab_node_red_backup/__main__.py` & `homelab_node_red_backup-1.4.0/homelab_node_red_backup/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,93 @@
 """Backup and Restore CLI."""
 import click
 import json
 from typing import Optional
 from homelab_node_red_backup.handler.backup import create_backup
 from homelab_node_red_backup.handler.check import data_exists
 from homelab_node_red_backup.handler.restore import restore_backup
+from homelab_node_red_backup.handler.flows import get_flows
 
 
 @click.group(chain=True)
 def main():
     """CLI Entrypoint"""
     pass
 
 
-@main.command()
+@main.command(help="Checks if data exists. Return code is not 0 if no data exists!")
 @click.option("--endpoint", "-e", type=str, required=True, help="Node-RED endpoint")
 @click.option(
     "--jwt-token", "-jwt", type=str, required=False, help="JWT Token for authentication"
 )
 def check(endpoint: str, jwt_token: Optional[str]):
     click.echo(
         f"Using {endpoint} to check for Node-RED configuration "
         + f"(JWT enabled: {jwt_token != None})."
     )
+
     checkpoint = data_exists(endpoint, jwt_token)
     click.echo(f"Data exists: {checkpoint}")
+    exit(not checkpoint)
 
 
-@main.command()
+@main.command(help="Backups the flows to the given file.")
 @click.option("--endpoint", "-e", type=str, required=True, help="Node-RED endpoint")
 @click.option("--file", "-f", type=str, required=True, help="Output JSON file")
 @click.option(
     "--jwt-token", "-jwt", type=str, required=False, help="JWT Token for authentication"
 )
 def backup(endpoint: str, file: str, jwt_token: Optional[str]):
     click.echo(
         f"Using {endpoint} to backup Node-RED configuration to {file} "
         + f"(JWT enabled: {jwt_token != None})."
     )
+
     backup = create_backup(endpoint, jwt_token)
     with open(file, "w") as outfile:
         json.dump(backup, outfile, indent=2)
     click.echo("Backup created successfully.")
 
 
-@main.command()
+@main.command(help="Restores flows from the given file.")
 @click.option("--endpoint", "-e", type=str, required=True, help="Node-RED endpoint")
 @click.option("--file", "-f", type=str, required=True, help="Output JSON file")
 @click.option(
     "--jwt-token", "-jwt", type=str, required=False, help="JWT Token for authentication"
 )
 def restore(endpoint: str, file: str, jwt_token: Optional[str]):
     click.echo(
         f"Using {endpoint} to restore {file} to Node-RED "
         + f"(JWT enabled: {jwt_token != None})."
     )
+
     with open(file, "r") as backup:
         restore_backup(endpoint, jwt_token, json.load(backup))
     click.echo("Restored backup successfully.")
 
 
+@main.command(
+    help="Backups to or restores from the given file depending on whether data exists."
+)
+@click.option("--endpoint", "-e", type=str, required=True, help="Node-RED endpoint")
+@click.option("--file", "-f", type=str, required=True, help="Output JSON file")
+@click.option(
+    "--jwt-token", "-jwt", type=str, required=False, help="JWT Token for authentication"
+)
+def auto(endpoint: str, file: str, jwt_token: Optional[str]):
+    click.echo(
+        f"Using {endpoint} to auto backup/restore from/to {file} from/to Node-RED "
+        + f"(JWT enabled: {jwt_token != None})."
+    )
+
+    flows = get_flows(endpoint, jwt_token)
+    if data_exists(endpoint, jwt_token, flows):
+        create_backup(endpoint, jwt_token, flows)
+        click.echo("Created backup successfully.")
+    else:
+        with open(file, "r") as backup:
+            restore_backup(endpoint, jwt_token, json.load(backup))
+        click.echo("Restored backup successfully.")
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `homelab_node_red_backup-1.3.0/homelab_node_red_backup/handler/backup.py` & `homelab_node_red_backup-1.4.0/homelab_node_red_backup/handler/backup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 from homelab_node_red_backup.handler.flows import get_flows
 from typing import Optional
 import click
 
 CREDENTIAL_NODES = ["server", "telegram bot"]
 
 
-def create_backup(endpoint: str, jwt_token: Optional[str]) -> dict:
+def create_backup(
+    endpoint: str, jwt_token: Optional[str], flows: Optional[dict] = None
+) -> dict:
     """Creates a backup JSON."""
     try:
-        flows = get_flows(endpoint, jwt_token)
-        credentials = _get_credentials(endpoint, jwt_token, flows)
+        fetched_flows = flows if flows is not None else get_flows(endpoint, jwt_token)
+        credentials = _get_credentials(endpoint, jwt_token, fetched_flows)
         return {
-            "rev": flows["rev"],
-            "flows": flows["flows"],
+            "rev": fetched_flows["rev"],
+            "flows": fetched_flows["flows"],
             "credentials": credentials,
         }
     except Exception as error:
         click.echo(f"Could not make request to Node-RED: {error}")
         raise click.Abort()
```

### Comparing `homelab_node_red_backup-1.3.0/homelab_node_red_backup/handler/flows.py` & `homelab_node_red_backup-1.4.0/homelab_node_red_backup/handler/flows.py`

 * *Files identical despite different names*

### Comparing `homelab_node_red_backup-1.3.0/homelab_node_red_backup/handler/restore.py` & `homelab_node_red_backup-1.4.0/homelab_node_red_backup/handler/restore.py`

 * *Files identical despite different names*

### Comparing `homelab_node_red_backup-1.3.0/pyproject.toml` & `homelab_node_red_backup-1.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "poetry-core"
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "homelab-node-red-backup"
-version = "1.3.0"
+version = "1.4.0"
 description = "Backup and Restore for Node-RED."
 license = "MIT"
 authors = [
     "Daniel Muehlbachler-Pietrzykowski <daniel.muehlbachler@niftyside.io>"
 ]
 readme = "README.md"
 repository = "https://github.com/muhlba91/onyx-client"
```

### Comparing `homelab_node_red_backup-1.3.0/PKG-INFO` & `homelab_node_red_backup-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homelab-node-red-backup
-Version: 1.3.0
+Version: 1.4.0
 Summary: Backup and Restore for Node-RED.
 Home-page: https://github.com/muhlba91/onyx-client
 License: MIT
 Keywords: node-red,homelab
 Author: Daniel Muehlbachler-Pietrzykowski
 Author-email: daniel.muehlbachler@niftyside.io
 Requires-Python: >=3.11,<4.0
@@ -61,19 +61,21 @@
 - `servers`: e.g. a Home Assistant server with an access token
 - `telegram bot`: Telegram bot with a token
 
 ## Usage
 
 The following commands are available, and all commands require the arguments `--endpoint`, and, optionally, `--jwt-token` set.
 
-- `check`: checks if data exists for a backup
+- `check`: checks if data exists for a backup (return code `0` if data exists, else `1`)
 - `backup`: creates a backup
   - requires: `--file`
 - `restore`: restores from a backup
   - requires: `--file`
+- `auto`: performs a `check` and either creates a backup to or restores a backup from the given `--file`
+  - requires: `--file`
 
 ### Examples
 
 ```bash
 # checking if data exists
 homelab-node-red-backup check -e http://localhost:1880 -jwt <TOKEN>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: homelab-node-red-backup Version: 1.3.0 Summary:
+Metadata-Version: 2.1 Name: homelab-node-red-backup Version: 1.4.0 Summary:
 Backup and Restore for Node-RED. Home-page: https://github.com/muhlba91/onyx-
 client License: MIT Keywords: node-red,homelab Author: Daniel Muehlbachler-
 Pietrzykowski Author-email: daniel.muehlbachler@niftyside.io Requires-Python:
 >=3.11,<4.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
@@ -32,15 +32,17 @@
 available: - `--endpoint` / `-e`: the Node-RED endpoint - `--file` / `-f`: the
 JSON file - `--jwt-token` / `-jwt`: the JWT token to authenticate with ##
 Credentials Credentials are detected, retrieved, and merged to the output JSON
 file. The following credential types are recognized: - `servers`: e.g. a Home
 Assistant server with an access token - `telegram bot`: Telegram bot with a
 token ## Usage The following commands are available, and all commands require
 the arguments `--endpoint`, and, optionally, `--jwt-token` set. - `check`:
-checks if data exists for a backup - `backup`: creates a backup - requires: `--
-file` - `restore`: restores from a backup - requires: `--file` ### Examples
-```bash # checking if data exists homelab-node-red-backup check -e http://
-localhost:1880 -jwt  # creating a backup homelab-node-red-backup backup -
-e http://localhost:1880 -jwt  -f backup.json # restoring from the backup
-homelab-node-red-backup restore -e http://localhost:1880 -jwt  -f backup.json
-``` --- ## Supporting If you enjoy the application and want to support my
-efforts, please feel free to buy me a coffe. :) [Buy_Me_A_Coffee]
+checks if data exists for a backup (return code `0` if data exists, else `1`) -
+`backup`: creates a backup - requires: `--file` - `restore`: restores from a
+backup - requires: `--file` - `auto`: performs a `check` and either creates a
+backup to or restores a backup from the given `--file` - requires: `--file` ###
+Examples ```bash # checking if data exists homelab-node-red-backup check -
+e http://localhost:1880 -jwt  # creating a backup homelab-node-red-backup
+backup -e http://localhost:1880 -jwt  -f backup.json # restoring from the
+backup homelab-node-red-backup restore -e http://localhost:1880 -jwt  -
+f backup.json ``` --- ## Supporting If you enjoy the application and want to
+support my efforts, please feel free to buy me a coffe. :) [Buy_Me_A_Coffee]
```

