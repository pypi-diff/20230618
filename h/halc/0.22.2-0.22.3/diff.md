# Comparing `tmp/halc-0.22.2.tar.gz` & `tmp/halc-0.22.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halc-0.22.2.tar", last modified: Fri Jun 16 14:02:09 2023, max compression
+gzip compressed data, was "halc-0.22.3.tar", last modified: Sun Jun 18 05:38:33 2023, max compression
```

## Comparing `halc-0.22.2.tar` & `halc-0.22.3.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-16 14:02:09.283882 halc-0.22.2/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1061 2023-06-14 16:42:42.000000 halc-0.22.2/LICENSE
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      858 2023-06-16 14:02:09.283882 halc-0.22.2/PKG-INFO
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      328 2023-06-14 16:36:58.000000 halc-0.22.2/README.md
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-16 14:02:09.283882 halc-0.22.2/halc/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      227 2023-06-16 14:02:07.000000 halc-0.22.2/halc/__about__.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       95 2023-06-16 02:01:38.000000 halc-0.22.2/halc/__init__.py
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-16 14:02:09.283882 halc-0.22.2/halc/images/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       27 2023-06-16 03:45:31.000000 halc-0.22.2/halc/images/__init__.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      487 2023-06-16 03:44:51.000000 halc-0.22.2/halc/images/get.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     5167 2023-06-16 13:59:13.000000 halc-0.22.2/halc/initialize.py
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-16 14:02:09.283882 halc-0.22.2/halc/projects/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       28 2023-06-16 01:55:40.000000 halc-0.22.2/halc/projects/__init__.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      507 2023-06-16 04:57:49.000000 halc-0.22.2/halc/projects/get.py
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-16 14:02:09.283882 halc-0.22.2/halc/upload/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      101 2023-06-16 03:33:09.000000 halc-0.22.2/halc/upload/__init__.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     4633 2023-06-16 04:59:32.000000 halc-0.22.2/halc/upload/images.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     6447 2023-06-16 04:54:54.000000 halc-0.22.2/halc/upload/labels.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      987 2023-06-16 04:34:06.000000 halc-0.22.2/halc/utils.py
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-16 14:02:09.283882 halc-0.22.2/halc/versions/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       42 2023-06-16 01:53:27.000000 halc-0.22.2/halc/versions/__init__.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      934 2023-06-16 02:12:02.000000 halc-0.22.2/halc/versions/get.py
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-16 14:02:09.283882 halc-0.22.2/halc.egg-info/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      858 2023-06-16 14:02:09.000000 halc-0.22.2/halc.egg-info/PKG-INFO
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      448 2023-06-16 14:02:09.000000 halc-0.22.2/halc.egg-info/SOURCES.txt
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)        1 2023-06-16 14:02:09.000000 halc-0.22.2/halc.egg-info/dependency_links.txt
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       88 2023-06-16 14:02:09.000000 halc-0.22.2/halc.egg-info/requires.txt
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)        5 2023-06-16 14:02:09.000000 halc-0.22.2/halc.egg-info/top_level.txt
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       79 2023-06-16 14:02:09.283882 halc-0.22.2/setup.cfg
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1383 2023-06-16 03:56:22.000000 halc-0.22.2/setup.py
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-18 05:38:33.635181 halc-0.22.3/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1061 2023-06-14 16:42:42.000000 halc-0.22.3/LICENSE
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      858 2023-06-18 05:38:33.635181 halc-0.22.3/PKG-INFO
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      328 2023-06-14 16:36:58.000000 halc-0.22.3/README.md
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-18 05:38:33.631181 halc-0.22.3/halc/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      227 2023-06-18 05:38:27.000000 halc-0.22.3/halc/__about__.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       95 2023-06-16 02:01:38.000000 halc-0.22.3/halc/__init__.py
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-18 05:38:33.631181 halc-0.22.3/halc/images/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       27 2023-06-16 03:45:31.000000 halc-0.22.3/halc/images/__init__.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      527 2023-06-18 05:34:51.000000 halc-0.22.3/halc/images/get.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     5773 2023-06-18 03:52:20.000000 halc-0.22.3/halc/initialize.py
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-18 05:38:33.635181 halc-0.22.3/halc/projects/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      127 2023-06-18 04:01:46.000000 halc-0.22.3/halc/projects/__init__.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1388 2023-06-18 05:35:04.000000 halc-0.22.3/halc/projects/create.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      538 2023-06-18 05:11:14.000000 halc-0.22.3/halc/projects/delete.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1015 2023-06-18 04:06:48.000000 halc-0.22.3/halc/projects/get.py
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-18 05:38:33.635181 halc-0.22.3/halc/upload/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      101 2023-06-16 03:33:09.000000 halc-0.22.3/halc/upload/__init__.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     4762 2023-06-18 05:36:30.000000 halc-0.22.3/halc/upload/images.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     6532 2023-06-18 05:32:04.000000 halc-0.22.3/halc/upload/labels.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      987 2023-06-16 04:34:06.000000 halc-0.22.3/halc/utils.py
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-18 05:38:33.635181 halc-0.22.3/halc/versions/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      157 2023-06-18 05:17:09.000000 halc-0.22.3/halc/versions/__init__.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1186 2023-06-18 05:37:02.000000 halc-0.22.3/halc/versions/create.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      707 2023-06-18 05:26:55.000000 halc-0.22.3/halc/versions/delete.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1596 2023-06-18 05:37:38.000000 halc-0.22.3/halc/versions/get.py
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-18 05:38:33.631181 halc-0.22.3/halc.egg-info/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      858 2023-06-18 05:38:33.000000 halc-0.22.3/halc.egg-info/PKG-INFO
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      544 2023-06-18 05:38:33.000000 halc-0.22.3/halc.egg-info/SOURCES.txt
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)        1 2023-06-18 05:38:33.000000 halc-0.22.3/halc.egg-info/dependency_links.txt
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       88 2023-06-18 05:38:33.000000 halc-0.22.3/halc.egg-info/requires.txt
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)        5 2023-06-18 05:38:33.000000 halc-0.22.3/halc.egg-info/top_level.txt
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       79 2023-06-18 05:38:33.635181 halc-0.22.3/setup.cfg
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1383 2023-06-16 03:56:22.000000 halc-0.22.3/setup.py
```

### Comparing `halc-0.22.2/LICENSE` & `halc-0.22.3/LICENSE`

 * *Files identical despite different names*

### Comparing `halc-0.22.2/PKG-INFO` & `halc-0.22.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halc
-Version: 0.22.2
+Version: 0.22.3
 Summary: Python SDK for Happyrobot's HALC
 Home-page: https://happyrobot.ai
 Author: Happyrobot
 Author-email: luis.paarup@happyrobot.ai
 License: MIT
 Keywords: happyrobot computer vision artificial intelligence foundation models large vision
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `halc-0.22.2/halc/initialize.py` & `halc-0.22.3/halc/initialize.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,17 +12,19 @@
 class ConfigNotFound(Exception):
     pass
 
 
 class InvalidConfig(Exception):
     pass
 
+
 class NotInitialized(Exception):
     pass
 
+
 @dataclass
 class HRConfig:
     hr_dir: Path = Path.home() / ".happyrobot"
     hr_file: Path = hr_dir / "config.yaml"
 
     endpoint: str = "https://app.happyrobot.ai"
     hrid: str = None
@@ -53,15 +55,20 @@
                     current[key] = value
             return cls.from_json(**current)
         except FileNotFoundError:
             return cls(**kwargs)
 
     @property
     def json(self) -> dict:
-        return {"endpoint": self.endpoint, "hrid": self.hrid, "hrinfo": self.hrinfo, "token": self.token}
+        return {
+            "endpoint": self.endpoint,
+            "hrid": self.hrid,
+            "hrinfo": self.hrinfo,
+            "token": self.token,
+        }
 
     @property
     def yaml(self) -> str:
         return yaml.dump(self.json)
 
     def commit(self) -> dict:
         self.hr_dir.mkdir(parents=False, exist_ok=True)
@@ -109,16 +116,18 @@
                 raise ConfigNotFound(
                     "Happyrobot Config not found. Run 'halc login' or place a config.yaml file here."
                 )
         except IsADirectoryError:
             raise ConfigNotFound(f"Config file provided [{config_file}] is a directory")
 
         if not self.config.is_valid():
-            raise InvalidConfig("Happyrobot Config is invalid. Run 'halc login' or check the provided hrid, hrinfo, token or endpoint")
-        
+            raise InvalidConfig(
+                "Happyrobot Config is invalid. Run 'halc login' or check the provided hrid, hrinfo, token or endpoint"
+            )
+
     @property
     def base_url(self):
         return f"{self.config.endpoint}/api/v1"
 
     def get(self, endpoint: str, params: dict = None):
         cookies = {
             "HRID": urllib.parse.quote(self.config.hrid),
@@ -131,15 +140,15 @@
             params=params,
             headers=headers,
             cookies=cookies,
         )
         res.raise_for_status()
 
         return res
-    
+
     def post(
         self,
         endpoint: str,
         data: Any,
         params: dict = None,
     ):
         cookies = {
@@ -155,25 +164,44 @@
             self.base_url + endpoint,
             data,
             params=params,
             headers=headers,
             cookies=cookies,
         )
         res.raise_for_status()
+        return res
+
+    def delete(self, endpoint: str, params: dict = None):
+        cookies = {
+            "HRID": urllib.parse.quote(self.config.hrid),
+            "HRINFO": urllib.parse.quote(self.config.hrinfo),
+        }
+        headers = {"authorization": f"Bearer {self.config.token}"}
+
+        res = requests.delete(
+            self.base_url + endpoint,
+            params=params,
+            headers=headers,
+            cookies=cookies,
+        )
+        res.raise_for_status()
+
+        return res
 
 
 def initialize(**kwargs) -> Client:
-    """ Initialize the session
-    """
+    """Initialize the session"""
     global _client
     _client = Client(**kwargs)
     return _client
 
 
 def get_client() -> Client:
     if _client is None:
-        raise NotInitialized("Please initialize the session with halc.initialize() before using any halc functionality.")
+        raise NotInitialized(
+            "Please initialize the session with halc.initialize() before using any halc functionality."
+        )
     return _client
 
 
 def config() -> HRConfig:
     return _client.config if _client else None
```

### Comparing `halc-0.22.2/halc/upload/images.py` & `halc-0.22.3/halc/upload/images.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,22 +58,24 @@
     return image
 
 
 def upload_images(
     paths: List[str],
     project_id: str,
     tags: List[str] = [],
-) -> None:
+) -> dict:
     """Upload a list of local images to the app
     :param paths: list of paths to images
     :param project_id: Id of the project
     :param tags: list of tags to apply to the uploaded images
+    :return: status of the operation
     """
 
     # Get project from backend
+    client = get_client()
     project = get_project(project_id)
 
     # If tags provided, merge them with existing tags and update the project
     tag_ids = []
     project_tags = project["attributes"][0]
     if len(tags) > 0:
         # Map tags to project tags
@@ -91,15 +93,14 @@
                     "name": tag,
                     "color": get_random_color(),
                 }
                 project_options.append(opt)
                 tag_ids.append(opt["id"])
 
         # Save options to backend
-        client = get_client()
         client.post(
             f"/attributes/options/{project['id']}/{project_tags['id']}",
             project_options,
         )
     attributes = {project_tags["id"]: tag_ids}
 
     # Upload images params
@@ -141,32 +142,35 @@
 
     # Wait for queue to empty
     read.join()
 
     # Finish the progress bar
     pbar.update(total - pbar.n)
 
+    return {"status": "ok", "upload_count": total}
+
 
 def upload_images_from_dir(
     base_dir: str,
     project_id: str,
     tags: List[str] = [],
     valid_images: List[str] = [".jpg", ".jpeg", ".png", ".tif", ".tiff"],
-) -> None:
+) -> dict:
     """Upload images from a directory
     :param base_dir: directory where the images live
     :param project_id: Id of the project
     :param tags: list of tags to apply to the uploaded images
     :param valid_images: valid extensions for the image files
+    :return: status of the operation
     """
 
     # Find the images
     files = []
     for f in os.listdir(base_dir):
         ext = os.path.splitext(f)[1]
         if ext.lower() not in valid_images:
             continue
         files.append(os.path.join(base_dir, f))
     print(f"Found {len(files)} images in {base_dir}")
 
     # Upload them to the app
-    upload_images(files, project_id, tags)
+    return upload_images(files, project_id, tags)
```

### Comparing `halc-0.22.2/halc/upload/labels.py` & `halc-0.22.3/halc/upload/labels.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,19 +37,20 @@
     return string.lower().replace(r"[\s_]", "")
 
 
 def upload_labels(
     ds: dict,
     project_id: str,
     version_id: str,
-) -> None:
+) -> dict:
     """Upload labels from a COCO json
     :param ds: COCO datasource with categories, images and annotations
     :param project_id: Id of the project
     :param version_id: Id of the version
+    :return: status of the operation
     """
 
     # Get project
     project = get_project(project_id)
 
     # Get all the images in the project
     images = get_images(project_id)
@@ -192,32 +193,34 @@
 
     # Upload the annotations
     client = get_client()
     client.post(
         f"/label/annotations/{project_id}",
         {"annotations": annotations, "classes": classes},
     )
-    print(f"Uploaded {n_annotations} annotations to project '{project['name']}'")
+
+    return {"status": "ok", "upload_count": n_annotations, "version_id": version_id}
 
 
 def upload_labels_from_file(
     path: str,
     project_id: str,
     version_id: str,
-) -> None:
+) -> dict:
     """Upload labels from a COCO json file
     :param path: path to the COCO file
     :param project_id: Id of the project
     :param version_id: Id of the version
+    :return: status of the operation
     """
 
     # Assert path
     _path = Path(path)
     if not _path.is_file():
         raise PathNotFound(f"File '{path}' not found")
 
     # Open file
     with _path.open("r") as f:
         ds = json.load(f)
 
     # Upload labels
-    upload_labels(ds, project_id, version_id)
+    return upload_labels(ds, project_id, version_id)
```

### Comparing `halc-0.22.2/halc/utils.py` & `halc-0.22.3/halc/utils.py`

 * *Files identical despite different names*

### Comparing `halc-0.22.2/halc.egg-info/PKG-INFO` & `halc-0.22.3/halc.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halc
-Version: 0.22.2
+Version: 0.22.3
 Summary: Python SDK for Happyrobot's HALC
 Home-page: https://happyrobot.ai
 Author: Happyrobot
 Author-email: luis.paarup@happyrobot.ai
 License: MIT
 Keywords: happyrobot computer vision artificial intelligence foundation models large vision
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `halc-0.22.2/setup.py` & `halc-0.22.3/setup.py`

 * *Files identical despite different names*

