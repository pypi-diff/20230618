# Comparing `tmp/web_ext_helper-1.0.3.tar.gz` & `tmp/web_ext_helper-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_ext_helper-1.0.3.tar", max compression
+gzip compressed data, was "web_ext_helper-1.0.4.tar", max compression
```

## Comparing `web_ext_helper-1.0.3.tar` & `web_ext_helper-1.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.0.3/LICENSE
--rw-r--r--   0        0        0      572 2023-06-17 20:50:14.892163 web_ext_helper-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1754 2023-06-17 20:34:00.666577 web_ext_helper-1.0.3/README.md
--rw-r--r--   0        0        0     9875 2023-06-17 18:50:16.248365 web_ext_helper-1.0.3/web_ext_helper/web_ext_helper.py
--rw-r--r--   0        0        0     2162 1970-01-01 00:00:00.000000 web_ext_helper-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.0.4/LICENSE
+-rw-r--r--   0        0        0      572 2023-06-17 20:58:39.887166 web_ext_helper-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1754 2023-06-17 20:34:00.666577 web_ext_helper-1.0.4/README.md
+-rw-r--r--   0        0        0     8760 2023-06-17 20:57:38.453775 web_ext_helper-1.0.4/web_ext_helper/web_ext_helper.py
+-rw-r--r--   0        0        0     2162 1970-01-01 00:00:00.000000 web_ext_helper-1.0.4/PKG-INFO
```

### Comparing `web_ext_helper-1.0.3/LICENSE` & `web_ext_helper-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.0.3/pyproject.toml` & `web_ext_helper-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "web-ext-helper"
-version = "1.0.3"
+version = "1.0.4"
 description = "A simple cli tool that helps you building your web extensions."
 authors = ["AppSolves <appsolves@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "web_ext_helper"}]
 
 [tool.poetry.dependencies]
```

### Comparing `web_ext_helper-1.0.3/README.md` & `web_ext_helper-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.0.3/web_ext_helper/web_ext_helper.py` & `web_ext_helper-1.0.4/web_ext_helper/web_ext_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,17 @@
 except FileNotFoundError:
     name = None
     version = None
 
 
 @app.command(help="Build the extension", name="build")
 def __build__(
-    name: str = typer.Option(None, "--name", "-n", help="Name of the build"),
+    name: str = typer.Option(
+        f"{name}-{version}.zip", "--name", "-n", help="Name of the build"
+    ),
     version: str = typer.Option(
         version,
         "--version",
         "-v",
         help="Specify the version of the extension",
     ),
     new_version: bool = typer.Option(
@@ -58,50 +60,16 @@
         error("manifest.json not found")
         raise typer.Exit(1)
 
     if version is not None and new_version:
         error("Cannot specify both version and new-version")
         raise typer.Exit(1)
 
-    if name is None:
-
-        def __get_zip_name__(version: str, new_version: bool = False) -> str:
-            def update_manifest(version: str):
-                with open("manifest.json", "r") as manifest:
-                    manifest_data = json.load(manifest)
-
-                with open("manifest.json", "w") as manifest:
-                    manifest_data["version"] = version
-                    json.dump(manifest_data, manifest, indent=2)
-
-            def get_new_version(version: str) -> str:
-                major, minor, patch = version.split(".")
-                patch = int(patch)
-                minor = int(minor)
-                major = int(major)
-
-                if patch == 9:
-                    patch = 0
-                    minor += 1
-                else:
-                    patch += 1
-
-                if minor == 9:
-                    minor = 0
-                    major += 1
-
-                return f"{major}.{minor}.{patch}"
-
-            if new_version:
-                version = get_new_version(version)
-                update_manifest(version)
-
-            return f"{name}-{version}.zip"
-
-        name = __get_zip_name__(version, new_version)
+    if not name.endswith(".zip"):
+        name += ".zip"
 
     if clean:
         shutil.rmtree("builds")
         shutil.rmtree("__pycache__")
         os.mkdir("builds")
 
     def write_dir(build, dirname):
```

### Comparing `web_ext_helper-1.0.3/PKG-INFO` & `web_ext_helper-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ext-helper
-Version: 1.0.3
+Version: 1.0.4
 Summary: A simple cli tool that helps you building your web extensions.
 License: GPL-3.0-or-later
 Author: AppSolves
 Author-email: appsolves@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

