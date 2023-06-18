# Comparing `tmp/pystructurizr-0.1.0.tar.gz` & `tmp/pystructurizr-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystructurizr-0.1.0.tar", last modified: Fri Jun 16 18:52:03 2023, max compression
+gzip compressed data, was "pystructurizr-0.1.1.tar", last modified: Sun Jun 18 09:58:37 2023, max compression
```

## Comparing `pystructurizr-0.1.0.tar` & `pystructurizr-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-06-16 18:52:03.107522 pystructurizr-0.1.0/
--rw-r--r--   0 niels      (501) staff       (20)     1091 2023-06-15 21:03:41.000000 pystructurizr-0.1.0/LICENSE.txt
--rw-r--r--   0 niels      (501) staff       (20)      670 2023-06-16 18:52:03.107030 pystructurizr-0.1.0/PKG-INFO
--rw-r--r--   0 niels      (501) staff       (20)     3417 2023-06-15 21:10:05.000000 pystructurizr-0.1.0/README.md
-drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-06-16 18:52:03.092385 pystructurizr-0.1.0/example/
--rw-r--r--   0 niels      (501) staff       (20)        0 2023-05-29 09:48:57.000000 pystructurizr-0.1.0/example/__init__.py
--rw-r--r--   0 niels      (501) staff       (20)       13 2023-06-11 13:23:09.000000 pystructurizr-0.1.0/example/bad.py
--rw-r--r--   0 niels      (501) staff       (20)      860 2023-06-10 15:04:26.000000 pystructurizr-0.1.0/example/chatsystem.py
--rw-r--r--   0 niels      (501) staff       (20)      198 2023-06-11 13:15:44.000000 pystructurizr-0.1.0/example/componentview.py
--rw-r--r--   0 niels      (501) staff       (20)      195 2023-06-10 16:13:37.000000 pystructurizr-0.1.0/example/containerview.py
--rw-r--r--   0 niels      (501) staff       (20)      163 2023-06-11 13:15:48.000000 pystructurizr-0.1.0/example/systemlandscapeview.py
--rw-r--r--   0 niels      (501) staff       (20)      197 2023-06-15 18:40:02.000000 pystructurizr-0.1.0/example/users.py
--rw-r--r--   0 niels      (501) staff       (20)      670 2023-06-15 20:39:26.000000 pystructurizr-0.1.0/example/workspace.py
-drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-06-16 18:52:03.098944 pystructurizr-0.1.0/pystructurizr/
--rw-r--r--   0 niels      (501) staff       (20)        0 2023-05-29 09:49:07.000000 pystructurizr-0.1.0/pystructurizr/__init__.py
--rw-r--r--   0 niels      (501) staff       (20)     3103 2023-06-15 19:23:40.000000 pystructurizr-0.1.0/pystructurizr/cli.py
--rw-r--r--   0 niels      (501) staff       (20)     1687 2023-06-15 19:29:11.000000 pystructurizr-0.1.0/pystructurizr/cli_helper.py
--rw-r--r--   0 niels      (501) staff       (20)     2197 2023-06-11 15:48:17.000000 pystructurizr-0.1.0/pystructurizr/cli_watcher.py
--rw-r--r--   0 niels      (501) staff       (20)     2469 2023-06-15 19:22:38.000000 pystructurizr-0.1.0/pystructurizr/cloudstorage.py
--rw-r--r--   0 niels      (501) staff       (20)    11140 2023-06-15 19:58:02.000000 pystructurizr-0.1.0/pystructurizr/dsl.py
--rw-r--r--   0 niels      (501) staff       (20)      390 2023-06-10 16:11:28.000000 pystructurizr-0.1.0/pystructurizr/index.html
-drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-06-16 18:52:03.106315 pystructurizr-0.1.0/pystructurizr.egg-info/
--rw-r--r--   0 niels      (501) staff       (20)      670 2023-06-16 18:52:03.000000 pystructurizr-0.1.0/pystructurizr.egg-info/PKG-INFO
--rw-r--r--   0 niels      (501) staff       (20)      610 2023-06-16 18:52:03.000000 pystructurizr-0.1.0/pystructurizr.egg-info/SOURCES.txt
--rw-r--r--   0 niels      (501) staff       (20)        1 2023-06-16 18:52:03.000000 pystructurizr-0.1.0/pystructurizr.egg-info/dependency_links.txt
--rw-r--r--   0 niels      (501) staff       (20)       57 2023-06-16 18:52:03.000000 pystructurizr-0.1.0/pystructurizr.egg-info/entry_points.txt
--rw-r--r--   0 niels      (501) staff       (20)       80 2023-06-16 18:52:03.000000 pystructurizr-0.1.0/pystructurizr.egg-info/requires.txt
--rw-r--r--   0 niels      (501) staff       (20)       22 2023-06-16 18:52:03.000000 pystructurizr-0.1.0/pystructurizr.egg-info/top_level.txt
--rw-r--r--   0 niels      (501) staff       (20)       38 2023-06-16 18:52:03.107716 pystructurizr-0.1.0/setup.cfg
--rw-r--r--   0 niels      (501) staff       (20)     1072 2023-06-16 18:51:37.000000 pystructurizr-0.1.0/setup.py
+drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-06-18 09:58:37.675823 pystructurizr-0.1.1/
+-rw-r--r--   0 niels      (501) staff       (20)     1091 2023-06-15 21:03:41.000000 pystructurizr-0.1.1/LICENSE.txt
+-rw-r--r--   0 niels      (501) staff       (20)     4120 2023-06-18 09:58:37.675407 pystructurizr-0.1.1/PKG-INFO
+-rw-r--r--   0 niels      (501) staff       (20)     3417 2023-06-15 21:10:05.000000 pystructurizr-0.1.1/README.md
+drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-06-18 09:58:37.664757 pystructurizr-0.1.1/example/
+-rw-r--r--   0 niels      (501) staff       (20)        0 2023-05-29 09:48:57.000000 pystructurizr-0.1.1/example/__init__.py
+-rw-r--r--   0 niels      (501) staff       (20)     2492 2023-06-18 09:38:04.000000 pystructurizr-0.1.1/example/analysissystem.py
+-rw-r--r--   0 niels      (501) staff       (20)      286 2023-06-18 09:39:00.000000 pystructurizr-0.1.1/example/analysisystem_containerview.py
+-rw-r--r--   0 niels      (501) staff       (20)      197 2023-06-18 09:39:15.000000 pystructurizr-0.1.1/example/chatserver_componentview.py
+-rw-r--r--   0 niels      (501) staff       (20)     1060 2023-06-17 18:06:20.000000 pystructurizr-0.1.1/example/chatsystem.py
+-rw-r--r--   0 niels      (501) staff       (20)      194 2023-06-18 09:39:26.000000 pystructurizr-0.1.1/example/chatsystem_containerview.py
+-rw-r--r--   0 niels      (501) staff       (20)      163 2023-06-11 13:15:48.000000 pystructurizr-0.1.1/example/systemlandscapeview.py
+-rw-r--r--   0 niels      (501) staff       (20)      315 2023-06-17 10:47:22.000000 pystructurizr-0.1.1/example/users.py
+-rw-r--r--   0 niels      (501) staff       (20)      606 2023-06-17 18:12:09.000000 pystructurizr-0.1.1/example/workspace.py
+drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-06-18 09:58:37.670364 pystructurizr-0.1.1/pystructurizr/
+-rw-r--r--   0 niels      (501) staff       (20)        0 2023-05-29 09:49:07.000000 pystructurizr-0.1.1/pystructurizr/__init__.py
+-rw-r--r--   0 niels      (501) staff       (20)     3469 2023-06-18 09:28:43.000000 pystructurizr-0.1.1/pystructurizr/cli.py
+-rw-r--r--   0 niels      (501) staff       (20)     1937 2023-06-18 09:29:38.000000 pystructurizr-0.1.1/pystructurizr/cli_helper.py
+-rw-r--r--   0 niels      (501) staff       (20)     2251 2023-06-17 20:24:22.000000 pystructurizr-0.1.1/pystructurizr/cli_watcher.py
+-rw-r--r--   0 niels      (501) staff       (20)     2516 2023-06-17 20:29:47.000000 pystructurizr-0.1.1/pystructurizr/cloudstorage.py
+-rw-r--r--   0 niels      (501) staff       (20)    12123 2023-06-17 20:41:33.000000 pystructurizr-0.1.1/pystructurizr/dsl.py
+-rw-r--r--   0 niels      (501) staff       (20)      249 2023-06-17 11:06:39.000000 pystructurizr-0.1.1/pystructurizr/index.html
+drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-06-18 09:58:37.673808 pystructurizr-0.1.1/pystructurizr.egg-info/
+-rw-r--r--   0 niels      (501) staff       (20)     4120 2023-06-18 09:58:37.000000 pystructurizr-0.1.1/pystructurizr.egg-info/PKG-INFO
+-rw-r--r--   0 niels      (501) staff       (20)      699 2023-06-18 09:58:37.000000 pystructurizr-0.1.1/pystructurizr.egg-info/SOURCES.txt
+-rw-r--r--   0 niels      (501) staff       (20)        1 2023-06-18 09:58:37.000000 pystructurizr-0.1.1/pystructurizr.egg-info/dependency_links.txt
+-rw-r--r--   0 niels      (501) staff       (20)       57 2023-06-18 09:58:37.000000 pystructurizr-0.1.1/pystructurizr.egg-info/entry_points.txt
+-rw-r--r--   0 niels      (501) staff       (20)       80 2023-06-18 09:58:37.000000 pystructurizr-0.1.1/pystructurizr.egg-info/requires.txt
+-rw-r--r--   0 niels      (501) staff       (20)       22 2023-06-18 09:58:37.000000 pystructurizr-0.1.1/pystructurizr.egg-info/top_level.txt
+-rw-r--r--   0 niels      (501) staff       (20)       38 2023-06-18 09:58:37.675961 pystructurizr-0.1.1/setup.cfg
+-rw-r--r--   0 niels      (501) staff       (20)     1271 2023-06-18 09:55:27.000000 pystructurizr-0.1.1/setup.py
+drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-06-18 09:58:37.674396 pystructurizr-0.1.1/test/
+-rw-r--r--   0 niels      (501) staff       (20)      675 2023-06-17 20:47:58.000000 pystructurizr-0.1.1/test/test_cli.py
```

### Comparing `pystructurizr-0.1.0/LICENSE.txt` & `pystructurizr-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pystructurizr-0.1.0/README.md` & `pystructurizr-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pystructurizr-0.1.0/pystructurizr/cli_helper.py` & `pystructurizr-0.1.1/pystructurizr/cli_helper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,58 @@
-import click
 import importlib
+import json
+import os
 import subprocess
 import sys
+
 import aiofiles
 import click
 import httpx
-import sys
-import os
 
 
 def generate_diagram_code(view: str) -> str:
     try:
+        initial_modules = set(sys.modules.keys())
         module = importlib.import_module(view)
+        imported_modules = set(sys.modules.keys()) - initial_modules
         code = module.workspace.dump()
-        return code
+        return code, imported_modules
     except ModuleNotFoundError:
+        # pylint: disable=raise-missing-from
         raise click.BadParameter("Invalid view name. Make sure you don't include the .py file extension.")
     except AttributeError:
+        # pylint: disable=raise-missing-from
         raise click.BadParameter("Non-compliant view file: make sure it exports the PyStructurizr workspace.")
 
 
 def generate_diagram_code_in_child_process(view: str) -> str:
     def run_child_process():
         # Run a separate Python script as a child process
-        output = subprocess.check_output([sys.executable, "-m", "pystructurizr.cli", "dump", "--view", view])
+        output = subprocess.check_output([sys.executable, "-m", "pystructurizr.cli", "dump", "--as-json", "--view", view])
         return output.decode().strip()
 
     # Run the child process and capture its output
     child_output = run_child_process()
-    return child_output
+    return json.loads(child_output)
 
 
 async def generate_svg(diagram_code: str, tmp_folder: str) -> str:
-    url = f"https://kroki.io/structurizr/svg"
+    url = "https://kroki.io/structurizr/svg"
     async with httpx.AsyncClient() as client:
         resp = await client.post(url, data=diagram_code)
 
     if resp.status_code != 200:
         print(resp)
         if resp.content:
             print(resp.content.decode())
         raise click.ClickException("Failed to create diagram")
-    
+
     svg_file_path = f"{tmp_folder}/diagram.svg"
-    async with aiofiles.open(svg_file_path, "w") as f:
-        await f.write(resp.text)
+    async with aiofiles.open(svg_file_path, "w") as svg_file:
+        await svg_file.write(resp.text)
 
     return svg_file_path
 
 
 def ensure_tmp_folder_exists() -> str:
     tmp_folder = "/tmp/pystructurizr"
     os.makedirs(tmp_folder, exist_ok=True)
```

### Comparing `pystructurizr-0.1.0/pystructurizr/cli_watcher.py` & `pystructurizr-0.1.1/pystructurizr/cli_watcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import datetime
 import os
 import time
-from watchdog.observers import Observer
+
 from watchdog.events import FileSystemEventHandler
-import datetime
+from watchdog.observers import Observer
 
 
 def formatted_timestamp():
     return datetime.datetime.now().strftime('%H:%M:%S')
 
 class CodeChangeEventHandler(FileSystemEventHandler):
     def __init__(self, modules_to_monitor, on_modified_callback):
@@ -39,15 +40,16 @@
     observer.schedule(event_handler, path='.', recursive=True)
 
     # Start the observer
     observer.start()
 
     try:
         # Keep the observer running until interrupted
-        print(f"{formatted_timestamp()}: Monitoring for file changes...")
+        print(f"{formatted_timestamp()}: Monitoring for file changes in following modules:")
+        print(modules_to_monitor)
         while True:
             time.sleep(1)
             if bool(event_handler.modified_modules):
                 event_handler.modified_modules.clear()
                 print(f"{datetime.datetime.now().strftime('%H:%M:%S')}: Regenerating diagram...")
                 await event_handler.on_modified_callback()
                 print(f"{formatted_timestamp()}: Monitoring for file changes...")
```

### Comparing `pystructurizr-0.1.0/pystructurizr/cloudstorage.py` & `pystructurizr-0.1.1/pystructurizr/cloudstorage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,68 @@
+import json
 from abc import ABC, abstractmethod
 from enum import Enum
-import json
 from typing import Dict
 
+import boto3
+from google.cloud import storage
+from google.cloud.exceptions import GoogleCloudError
+
 
+# pylint: disable=too-few-public-methods
 class CloudStorage(ABC):
     class Provider(Enum):
         GCS = "GCS"
         S3 = "S3"
 
     @abstractmethod
     def upload_file(self, file_path: str, bucket_name: str, object_name: str) -> str:
         pass
- 
+
 
 class GCS(CloudStorage):
     def __init__(self, gcs_credentials):
         self.gcs_credentials = gcs_credentials
 
     def upload_file(self, file_path: str, bucket_name: str, object_name: str) -> str:
-        from google.cloud import storage
-        from google.cloud.exceptions import GoogleCloudError
         try:
             gcs_client = storage.Client.from_service_account_json(self.gcs_credentials)
             gcs_bucket = gcs_client.get_bucket(bucket_name)
             gcs_blob = gcs_bucket.blob(object_name)
             gcs_blob.upload_from_filename(file_path)
             return f"https://storage.googleapis.com/{bucket_name}/{object_name}"
-        except GoogleCloudError as e:
+        except GoogleCloudError as exc:
             print("An error occurred while uploading the file to Google Cloud Storage:")
-            print(e)
+            print(exc)
+            return ""
 
 
 class S3(CloudStorage):
     def __init__(self, credentials_file: str):
-        import boto3
         self.credentials = self._load_credentials(credentials_file)
         self.client = boto3.client(
             "s3",
             aws_access_key_id=self.credentials["access_key"],
             aws_secret_access_key=self.credentials["secret_key"],
             region_name=self.credentials["region"]
         )
-    
+
     def _load_credentials(self, credentials_file: str) -> Dict[str, str]:
-        with open(credentials_file, "r") as f:
-            credentials = json.load(f)
+        with open(credentials_file, "r", encoding='utf-8') as cred:
+            credentials = json.load(cred)
         required_keys = ["access_key", "secret_key", "region"]
         if not all(key in credentials for key in required_keys):
             raise ValueError("Invalid credentials format")
         return credentials
 
     def upload_file(self, file_path: str, bucket_name: str, object_name: str) -> str:
         self.client.upload_file(file_path, bucket_name, object_name)
         url = f"https://{bucket_name}.s3.amazonaws.com/{object_name}"
         return url
 
 
 def create_cloud_storage(provider: CloudStorage.Provider, credentials_file: str) -> CloudStorage:
     if provider == CloudStorage.Provider.GCS:
         return GCS(credentials_file)
-    elif provider == CloudStorage.Provider.S3:
+    if provider == CloudStorage.Provider.S3:
         return S3(credentials_file)
-    else:
-        raise ValueError("Invalid cloud storage provider")
+    raise ValueError("Invalid cloud storage provider")
```

### Comparing `pystructurizr-0.1.0/pystructurizr/dsl.py` & `pystructurizr-0.1.1/pystructurizr/dsl.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import re
 import keyword
+import re
 from enum import Enum
 from typing import List, Optional
 
 
+# pylint: disable=too-few-public-methods
 class Identifier:
     counter = {}
 
     @staticmethod
     def make_identifier(name: str) -> str:
         # Replace invalid characters
         identifier = re.sub('[^0-9a-zA-Z_]', '_', name.lower())
@@ -25,102 +26,95 @@
 
         # Append counter if identifier already exists
         if identifier in Identifier.counter:
             Identifier.counter[identifier] += 1
             identifier = f"{identifier}_{Identifier.counter[identifier]}"
         else:
             Identifier.counter[identifier] = 1
-        
+
         return identifier
-    
+
 
 class Dumper:
     def __init__(self):
         self.level = 0
         self.lines = []
 
-    def add(self, s: str) -> None:
-        self.lines.append(f'{"  " * self.level}{s}')
+    def add(self, txt: str) -> None:
+        self.lines.append(f'{"  " * self.level}{txt}')
 
     def indent(self) -> None:
         self.level += 1
 
     def outdent(self):
-        self.level -= 1
-        if self.level < 0:
-            self.level = 0
+        self.level = max(self.level - 1, 0)
 
     def result(self) -> str:
         return "\n".join(self.lines)
 
 
 class Element:
     def __init__(self, name: str, description: Optional[str]=None, technology: Optional[str]=None, tags: Optional[List[str]]=None):
         self.name = name
-        self.description = description
-        self.technology = technology
+        self.description = description if description else ""
+        self.technology = technology if technology else ""
         self.tags = tags if tags else []
         self.relationships = []
         self.instname = Identifier.make_identifier(name)
 
     def uses(self, destination: str, description: Optional[str]=None, technology: Optional[str]=None) -> 'Relationship':
         relationship = Relationship(self, destination, description, technology)
         self.relationships.append(relationship)
         return relationship
-    
+
     def dump(self, dumper: Dumper) -> None:
         raise NotImplementedError("This method must be implemented in a subclass.")
 
     def dump_relationships(self, dumper: Dumper) -> None:
         raise NotImplementedError("This method must be implemented in a subclass.")
 
 
 class Person(Element):
-    def __init__(self, name: str, description: Optional[str]=None, technology: Optional[str]=None, tags: Optional[List[str]]=None):
-        super().__init__(name, description, technology, tags)
-
     def dump(self, dumper: Dumper) -> None:
         dumper.add(f'{self.instname} = Person "{self.name}" "{self.description}" {{')
         dumper.indent()
         if self.technology:
             dumper.add(f'technology "{self.technology}"')
         if self.tags:
             dumper.add(f'tags "{", ".join(self.tags)}"')
         dumper.outdent()
-        dumper.add(f'}}')
+        dumper.add('}')
 
     def dump_relationships(self, dumper: Dumper) -> None:
         for rel in self.relationships:
             rel.dump(dumper)
 
 
 class Component(Element):
-    def __init__(self, name: str, description: Optional[str]=None, technology: Optional[str]=None, tags: Optional[List[str]]=None):
-        super().__init__(name, description, technology, tags)
-
     def dump(self, dumper: Dumper) -> None:
         dumper.add(f'{self.instname} = Component "{self.name}" "{self.description}" {{')
         dumper.indent()
         if self.technology:
             dumper.add(f'technology "{self.technology}"')
         if self.tags:
             dumper.add(f'tags "{", ".join(self.tags)}"')
         dumper.outdent()
-        dumper.add(f'}}')
+        dumper.add('}')
 
     def dump_relationships(self, dumper: Dumper) -> None:
         for rel in self.relationships:
             rel.dump(dumper)
 
 
 class Container(Element):
     def __init__(self, name: str, description: Optional[str]=None, technology: Optional[str]=None, tags: Optional[List[str]]=None):
         super().__init__(name, description, technology, tags)
         self.components = []
 
+    # pylint: disable=invalid-name
     def Component(self, *args, **kwargs) -> Component:
         if args and isinstance(args[0], Component):
             component = args[0]
         else:
             component = Component(*args, **kwargs)
         self.components.append(component)
         return component
@@ -131,28 +125,29 @@
         if self.technology:
             dumper.add(f'technology "{self.technology}"')
         if self.tags:
             dumper.add(f'tags "{", ".join(self.tags)}"')
         for component in self.components:
             component.dump(dumper)
         dumper.outdent()
-        dumper.add(f'}}')
+        dumper.add('}')
 
     def dump_relationships(self, dumper: Dumper) -> None:
         for rel in self.relationships:
             rel.dump(dumper)
         for component in self.components:
             component.dump_relationships(dumper)
 
 
 class SoftwareSystem(Element):
     def __init__(self, name: str, description: Optional[str]=None, technology: Optional[str]=None, tags: Optional[List[str]]=None):
         super().__init__(name, description, technology, tags)
         self.containers = []
 
+    # pylint: disable=invalid-name
     def Container(self, *args, **kwargs) -> Container:
         if args and isinstance(args[0], Container):
             container = args[0]
         else:
             container = Container(*args, **kwargs)
         self.containers.append(container)
         return container
@@ -163,36 +158,38 @@
         if self.technology:
             dumper.add(f'technology "{self.technology}"')
         if self.tags:
             dumper.add(f'tags "{", ".join(self.tags)}"')
         for container in self.containers:
             container.dump(dumper)
         dumper.outdent()
-        dumper.add(f'}}')
+        dumper.add('}')
 
     def dump_relationships(self, dumper: Dumper) -> None:
         for rel in self.relationships:
             rel.dump(dumper)
         for container in self.containers:
             container.dump_relationships(dumper)
 
 
 class Model(Element):
     def __init__(self, name: str):
         super().__init__(name)
         self.elements = []
 
+    # pylint: disable=invalid-name
     def Person(self, *args, **kwargs) -> Person:
         if args and isinstance(args[0], Person):
             person = args[0]
         else:
             person = Person(*args, **kwargs)
         self.elements.append(person)
         return person
 
+    # pylint: disable=invalid-name
     def SoftwareSystem(self, *args, **kwargs) -> SoftwareSystem:
         if args and isinstance(args[0], SoftwareSystem):
             system = args[0]
         else:
             system = SoftwareSystem(*args, **kwargs)
         self.elements.append(system)
         return system
@@ -206,16 +203,16 @@
             element.dump_relationships(dumper)
 
 
 class Relationship:
     def __init__(self, source: Element, destination: Element, description: Optional[str]=None, technology: Optional[str]=None):
         self.source = source
         self.destination = destination
-        self.description = description
-        self.technology = technology
+        self.description = description if description else ""
+        self.technology = technology if technology else ""
 
     def dump(self, dumper: Dumper) -> None:
         dumper.add(f'{self.source.instname} -> {self.destination.instname} "{self.description}" "{self.technology}"')
 
 
 class View:
     class Kind(Enum):
@@ -228,109 +225,146 @@
         self.viewkind = viewkind
         self.element = element
         self.name = name
         self.description = description
         self.includes = []
         self.excludes = []
 
-    def include(self, element: Element) -> None:
+    def include(self, element: Element) -> 'View':
         self.includes.append(element)
-        
-    def exclude(self, element: Element) -> None:
+        return self
+
+    def exclude(self, element: Element) -> 'View':
         self.excludes.append(element)
+        return self
 
     def dump(self, dumper: Dumper) -> None:
         dumper.add(f'{self.viewkind.value} {self.element.instname if self.element else ""} {{')
         dumper.indent()
         if self.description:
             dumper.add(f'description "{self.description}"')
         dumper.add('include *')
         for include in self.includes:
-            dumper.add(f'include {include}')
+            dumper.add(f'include {include.instname}')
         for exclude in self.excludes:
-            dumper.add(f'exclude {exclude}')
+            dumper.add(f'exclude {exclude.instname}')
         dumper.add('autoLayout')
         dumper.outdent()
-        dumper.add(f'}}')
+        dumper.add('}')
 
 
 class Style:
-    def __init__(self, map: dict[str, str]):
-        self.map = map
+    def __init__(self, style_map: dict[str, str]):
+        self.map = style_map
 
     def dump(self, dumper: Dumper) -> None:
         dumper.add(f'element "{self.map["tag"]}" {{')
         dumper.indent()
-        for k, v in self.map.items():
-            if k == "tag":
+        for key, value in self.map.items():
+            if key == "tag":
                 continue
-            dumper.add(f'{k} "{v}"')
+            dumper.add(f'{key} "{value}"')
         dumper.outdent()
-        dumper.add(f'}}')
+        dumper.add('}')
 
 
 class Workspace:
     def __init__(self):
         self.models = []
         self.views = []
         self.styles = []
+        # Default styling
+        self.Styles(
+            {
+                "tag": "Element",
+                "shape": "RoundedBox"
+            }, {
+                "tag": "Software System",
+                "background": "#1168bd",
+                "color": "#ffffff"
+            }, {
+                "tag": "Container",
+                "background": "#438dd5",
+                "color": "#ffffff"
+            }, {
+                "tag": "Component",
+                "background": "#85bbf0",
+                "color": "#000000"
+            }, {
+                "tag": "Person",
+                "background": "#08427b",
+                "color": "#ffffff",
+                "shape": "Person"
+            }, {
+                "tag": "Infrastructure Node",
+                "background": "#ffffff"
+            }, {
+                "tag": "database",
+                "shape": "Cylinder"
+            }
+        )
 
     def dump(self, dumper: Dumper = Dumper()) -> None:
-        dumper.add(f'workspace {{')
+        dumper.add('workspace {')
         dumper.indent()
 
-        dumper.add(f'model {{')
+        dumper.add('model {')
         dumper.indent()
         for model in self.models:
             model.dump(dumper)
         for model in self.models:
             model.dump_relationships(dumper)
         dumper.outdent()
-        dumper.add(f'}}')
+        dumper.add('}')
 
-        dumper.add(f'views {{')
+        dumper.add('views {')
         dumper.indent()
         for view in self.views:
             view.dump(dumper)
-        dumper.add(f'styles {{')
+        dumper.add('styles {')
         dumper.indent()
         for style in self.styles:
             style.dump(dumper)
         dumper.outdent()
-        dumper.add(f'}}')
+        dumper.add('}')
         dumper.outdent()
-        dumper.add(f'}}')
+        dumper.add('}')
 
         dumper.outdent()
-        dumper.add(f'}}')
+        dumper.add('}')
         return dumper.result()
 
+    # pylint: disable=invalid-name
     def Model(self, model: Optional[Model]=None, name: Optional[str]=None):
         if model is None:
             model = Model(name)
         self.models.append(model)
         return model
 
+    # pylint: disable=invalid-name
     def SystemLandscapeView(self, name: str, description: str):
         view = View(View.Kind.SYSTEM_LANDSCAPE, None, name, description)
         self.views.append(view)
         return view
-    
+
+    # pylint: disable=invalid-name
     def SystemContextView(self, element: Element, name: str, description: str):
         view = View(View.Kind.SYSTEM_CONTEXT, element, name, description)
         self.views.append(view)
         return view
-    
+
+    # pylint: disable=invalid-name
     def ContainerView(self, element: Element, name: str, description: str):
         view = View(View.Kind.CONTAINER, element, name, description)
         self.views.append(view)
         return view
-    
+
+    # pylint: disable=invalid-name
     def ComponentView(self, element: Element, name: str, description: str):
         view = View(View.Kind.COMPONENT, element, name, description)
         self.views.append(view)
         return view
 
+    # pylint: disable=invalid-name
     def Styles(self, *styles: dict[str, str]) -> None:
         for style in styles:
             self.styles.append(Style(style))
-
```

### Comparing `pystructurizr-0.1.0/pystructurizr.egg-info/SOURCES.txt` & `pystructurizr-0.1.1/pystructurizr.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 LICENSE.txt
 README.md
 setup.py
 example/__init__.py
-example/bad.py
+example/analysissystem.py
+example/analysisystem_containerview.py
+example/chatserver_componentview.py
 example/chatsystem.py
-example/componentview.py
-example/containerview.py
+example/chatsystem_containerview.py
 example/systemlandscapeview.py
 example/users.py
 example/workspace.py
 pystructurizr/__init__.py
 pystructurizr/cli.py
 pystructurizr/cli_helper.py
 pystructurizr/cli_watcher.py
@@ -17,8 +18,9 @@
 pystructurizr/dsl.py
 pystructurizr/index.html
 pystructurizr.egg-info/PKG-INFO
 pystructurizr.egg-info/SOURCES.txt
 pystructurizr.egg-info/dependency_links.txt
 pystructurizr.egg-info/entry_points.txt
 pystructurizr.egg-info/requires.txt
-pystructurizr.egg-info/top_level.txt
+pystructurizr.egg-info/top_level.txt
+test/test_cli.py
```

### Comparing `pystructurizr-0.1.0/setup.py` & `pystructurizr-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 from setuptools import setup, find_packages
 
-with open('requirements.txt') as f:
+with open('requirements.txt', 'r', encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
+with open('README.md', 'r', encoding='utf-8') as f:
+    long_description = f.read()
+
 setup(
     name='pystructurizr',
-    version='0.1.0',
+    version='0.1.1',
     description='A Python DSL inspired by Structurizr, intended for generating C4 diagrams',
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     author='Niels Vanspauwen',
     author_email='niels.vanspauwen@gmail.com',
     license='MIT',
     url='https://github.com/nielsvanspauwen/pystructurizr',
     data_files=[('', ['LICENSE.txt'])],
     packages=find_packages(),
     package_data={
@@ -27,8 +32,8 @@
         'Programming Language :: Python :: 3.8',
     ],
     entry_points={
         'console_scripts': [
             'pystructurizr = pystructurizr.cli:cli'
         ]
     },
-)
+)
```

