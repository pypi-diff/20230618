# Comparing `tmp/minecraft-launcher-lib-6.0.tar.gz` & `tmp/minecraft-launcher-lib-6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minecraft-launcher-lib-6.0.tar", last modified: Fri Jun  9 11:27:23 2023, max compression
+gzip compressed data, was "minecraft-launcher-lib-6.1.tar", last modified: Sun Jun 18 08:11:44 2023, max compression
```

## Comparing `minecraft-launcher-lib-6.0.tar` & `minecraft-launcher-lib-6.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 11:27:23.751604 minecraft-launcher-lib-6.0/
--rw-r--r--   0 root         (0) root         (0)     1318 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      117 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4987 2023-06-09 11:27:23.751604 minecraft-launcher-lib-6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3259 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 11:27:23.747604 minecraft-launcher-lib-6.0/minecraft_launcher_lib/
--rw-r--r--   0 root         (0) root         (0)      350 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10512 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 11:27:23.747604 minecraft-launcher-lib-6.0/minecraft_launcher_lib/_internal_types/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/_internal_types/__init__.py
--rw-r--r--   0 root         (0) root         (0)      903 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/_internal_types/forge_types.py
--rw-r--r--   0 root         (0) root         (0)      271 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/_internal_types/helper_types.py
--rw-r--r--   0 root         (0) root         (0)      174 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/_internal_types/install_types.py
--rw-r--r--   0 root         (0) root         (0)      776 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/_internal_types/mrpack_types.py
--rw-r--r--   0 root         (0) root         (0)      815 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/_internal_types/runtime_types.py
--rw-r--r--   0 root         (0) root         (0)     2587 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/_internal_types/shared_types.py
--rw-r--r--   0 root         (0) root         (0)      443 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/_internal_types/vanilla_launcher_types.py
--rw-r--r--   0 root         (0) root         (0)    10945 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/command.py
--rw-r--r--   0 root         (0) root         (0)     3479 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     5507 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/fabric.py
--rw-r--r--   0 root         (0) root         (0)    10464 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/forge.py
--rw-r--r--   0 root         (0) root         (0)     9281 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/install.py
--rw-r--r--   0 root         (0) root         (0)     4522 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/java_utils.py
--rw-r--r--   0 root         (0) root         (0)    14509 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/microsoft_account.py
--rw-r--r--   0 root         (0) root         (0)     1554 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/microsoft_types.py
--rw-r--r--   0 root         (0) root         (0)     7692 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/mrpack.py
--rw-r--r--   0 root         (0) root         (0)     3584 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/natives.py
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/py.typed
--rw-r--r--   0 root         (0) root         (0)     5719 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/quilt.py
--rw-r--r--   0 root         (0) root         (0)     7695 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/runtime.py
--rw-r--r--   0 root         (0) root         (0)     3602 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/types.py
--rw-r--r--   0 root         (0) root         (0)     6639 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/utils.py
--rw-r--r--   0 root         (0) root         (0)     8876 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/vanilla_launcher.py
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/version.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 11:27:23.747604 minecraft-launcher-lib-6.0/minecraft_launcher_lib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4987 2023-06-09 11:27:23.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1692 2023-06-09 11:27:23.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 11:27:23.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-09 11:27:23.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-09 11:27:23.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1845 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 11:27:23.751604 minecraft-launcher-lib-6.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 11:27:23.751604 minecraft-launcher-lib-6.0/tests/
--rw-r--r--   0 root         (0) root         (0)     5523 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/tests/test_command.py
--rw-r--r--   0 root         (0) root         (0)     1889 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/tests/test_exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1966 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/tests/test_fabric.py
--rw-r--r--   0 root         (0) root         (0)     1461 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/tests/test_forge.py
--rw-r--r--   0 root         (0) root         (0)      363 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/tests/test_install.py
--rw-r--r--   0 root         (0) root         (0)      256 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/tests/test_java_utils.py
--rw-r--r--   0 root         (0) root         (0)     1100 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/tests/test_microsoft_account.py
--rw-r--r--   0 root         (0) root         (0)     6588 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/tests/test_mrpack.py
--rw-r--r--   0 root         (0) root         (0)      347 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/tests/test_natives.py
--rw-r--r--   0 root         (0) root         (0)     1891 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/tests/test_quilt.py
--rw-r--r--   0 root         (0) root         (0)     1238 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/tests/test_runtime.py
--rw-r--r--   0 root         (0) root         (0)     3971 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     3897 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/tests/test_vanilla_launcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 08:11:44.605982 minecraft-launcher-lib-6.1/
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      117 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4987 2023-06-18 08:11:44.605982 minecraft-launcher-lib-6.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3259 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 08:11:44.601982 minecraft-launcher-lib-6.1/minecraft_launcher_lib/
+-rw-r--r--   0 root         (0) root         (0)      350 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10512 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib/_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 08:11:44.601982 minecraft-launcher-lib-6.1/minecraft_launcher_lib/_internal_types/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib/_internal_types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      903 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib/_internal_types/forge_types.py
+-rw-r--r--   0 root         (0) root         (0)      271 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib/_internal_types/helper_types.py
+-rw-r--r--   0 root         (0) root         (0)      174 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib/_internal_types/install_types.py
+-rw-r--r--   0 root         (0) root         (0)      776 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib/_internal_types/mrpack_types.py
+-rw-r--r--   0 root         (0) root         (0)      815 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib/_internal_types/runtime_types.py
+-rw-r--r--   0 root         (0) root         (0)     2587 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib/_internal_types/shared_types.py
+-rw-r--r--   0 root         (0) root         (0)      443 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib/_internal_types/vanilla_launcher_types.py
+-rw-r--r--   0 root         (0) root         (0)    10968 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib/command.py
+-rw-r--r--   0 root         (0) root         (0)     3982 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     5507 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib/fabric.py
+-rw-r--r--   0 root         (0) root         (0)    10464 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib/forge.py
+-rw-r--r--   0 root         (0) root         (0)     9304 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib/install.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib/java_utils.py
+-rw-r--r--   0 root         (0) root         (0)    14781 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib/microsoft_account.py
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib/microsoft_types.py
+-rw-r--r--   0 root         (0) root         (0)     8050 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib/mrpack.py
+-rw-r--r--   0 root         (0) root         (0)     3607 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib/natives.py
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib/py.typed
+-rw-r--r--   0 root         (0) root         (0)     5719 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib/quilt.py
+-rw-r--r--   0 root         (0) root         (0)     7695 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib/runtime.py
+-rw-r--r--   0 root         (0) root         (0)     3602 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib/types.py
+-rw-r--r--   0 root         (0) root         (0)     7273 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib/utils.py
+-rw-r--r--   0 root         (0) root         (0)     9062 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib/vanilla_launcher.py
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 08:11:44.601982 minecraft-launcher-lib-6.1/minecraft_launcher_lib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4987 2023-06-18 08:11:44.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-06-18 08:11:44.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-18 08:11:44.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-18 08:11:44.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-18 08:11:44.000000 minecraft-launcher-lib-6.1/minecraft_launcher_lib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1845 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-18 08:11:44.605982 minecraft-launcher-lib-6.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 08:11:44.605982 minecraft-launcher-lib-6.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     4993 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/tests/test_command.py
+-rw-r--r--   0 root         (0) root         (0)     1889 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/tests/test_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1966 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/tests/test_fabric.py
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/tests/test_forge.py
+-rw-r--r--   0 root         (0) root         (0)     2928 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/tests/test_install.py
+-rw-r--r--   0 root         (0) root         (0)     3301 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/tests/test_java_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7813 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/tests/test_microsoft_account.py
+-rw-r--r--   0 root         (0) root         (0)     6708 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/tests/test_mrpack.py
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/tests/test_natives.py
+-rw-r--r--   0 root         (0) root         (0)     1891 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/tests/test_quilt.py
+-rw-r--r--   0 root         (0) root         (0)     1238 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/tests/test_runtime.py
+-rw-r--r--   0 root         (0) root         (0)    10207 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8138 2023-06-18 08:11:06.000000 minecraft-launcher-lib-6.1/tests/test_vanilla_launcher.py
```

### Comparing `minecraft-launcher-lib-6.0/LICENSE` & `minecraft-launcher-lib-6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.0/PKG-INFO` & `minecraft-launcher-lib-6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minecraft-launcher-lib
-Version: 6.0
+Version: 6.1
 Summary: A library for creating a custom Minecraft launcher
 Author-email: JakobDev <jakobdev@gmx.de>
 License: BSD-2-Clause
 Project-URL: Documentation, https://minecraft-launcher-lib.readthedocs.io/en/stable/index.html
 Project-URL: Issues, https://codeberg.org/JakobDev/minecraft-launcher-lib/issues
 Project-URL: Source, https://codeberg.org/JakobDev/minecraft-launcher-lib
 Project-URL: Changelog, https://minecraft-launcher-lib.readthedocs.io/en/stable/changelog.html
```

### Comparing `minecraft-launcher-lib-6.0/README.md` & `minecraft-launcher-lib-6.1/README.md`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.0/minecraft_launcher_lib/_helper.py` & `minecraft-launcher-lib-6.1/minecraft_launcher_lib/_helper.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.0/minecraft_launcher_lib/_internal_types/forge_types.py` & `minecraft-launcher-lib-6.1/minecraft_launcher_lib/_internal_types/forge_types.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.0/minecraft_launcher_lib/_internal_types/mrpack_types.py` & `minecraft-launcher-lib-6.1/minecraft_launcher_lib/_internal_types/mrpack_types.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.0/minecraft_launcher_lib/_internal_types/runtime_types.py` & `minecraft-launcher-lib-6.1/minecraft_launcher_lib/_internal_types/runtime_types.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.0/minecraft_launcher_lib/_internal_types/shared_types.py` & `minecraft-launcher-lib-6.1/minecraft_launcher_lib/_internal_types/shared_types.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.0/minecraft_launcher_lib/command.py` & `minecraft-launcher-lib-6.1/minecraft_launcher_lib/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
     path = str(minecraft_directory)
 
     if not os.path.isdir(os.path.join(path, "versions", version)):
         raise VersionNotFound(version)
 
     options = copy.deepcopy(options)
 
-    with open(os.path.join(path, "versions", version, version + ".json")) as f:
+    with open(os.path.join(path, "versions", version, version + ".json"), "r", encoding="utf-8") as f:
         data: ClientJson = json.load(f)
 
     if "inheritsFrom" in data:
         data = inherit_json(data, path)
 
     options["nativesDirectory"] = options.get("nativesDirectory", os.path.join(path, "versions", data["id"], "natives"))
     classpath = get_libraries(data, path)
```

### Comparing `minecraft-launcher-lib-6.0/minecraft_launcher_lib/exceptions.py` & `minecraft-launcher-lib-6.1/minecraft_launcher_lib/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,7 +106,16 @@
         self.expected_checksum: str = expected_checksum
         "The expected Checksum"
 
         self.actual_checksum: str = actual_checksum
         "The actual Checksum"
 
         super().__init__("InvalidChecksum", f"{path} has the wrong Checksum")
+
+
+class AzureAppNotPermitted(Exception):
+    """
+    Raised when you try to use a Azure App, that don't have the Permission to use the Minecraft API.
+    Take a look at the For more information about the options take a look at the :doc:`/tutorial/microsoft_login` tutorial to learn how to fix this.
+    """
+    def __init__(self) -> None:
+        super().__init__("It looks like your Azure App don't have the Permission to use the Minecraft API. Take a look at the Documentation for more Information.")
```

### Comparing `minecraft-launcher-lib-6.0/minecraft_launcher_lib/fabric.py` & `minecraft-launcher-lib-6.1/minecraft_launcher_lib/fabric.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.0/minecraft_launcher_lib/forge.py` & `minecraft-launcher-lib-6.1/minecraft_launcher_lib/forge.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.0/minecraft_launcher_lib/install.py` & `minecraft-launcher-lib-6.1/minecraft_launcher_lib/install.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
     """
     Installs the given version
     """
     # Download and read versions.json
     if url:
         download_file(url, os.path.join(path, "versions", versionid, versionid + ".json"), callback, sha1=sha1, minecraft_directory=path)
 
-    with open(os.path.join(path, "versions", versionid, versionid + ".json")) as f:
+    with open(os.path.join(path, "versions", versionid, versionid + ".json"), "r", encoding="utf-8") as f:
         versiondata: ClientJson = json.load(f)
 
     # For Forge
     if "inheritsFrom" in versiondata:
         try:
             install_minecraft_version(versiondata["inheritsFrom"], path, callback=callback)
         except VersionNotFound:
```

### Comparing `minecraft-launcher-lib-6.0/minecraft_launcher_lib/java_utils.py` & `minecraft-launcher-lib-6.1/minecraft_launcher_lib/java_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,21 +35,21 @@
     information["is_64bit"] = "64-Bit" in lines[2]
     information["openjdk"] = lines[0].startswith("openjdk")
 
     if platform.system() == "Windows":
         information["java_path"] = os.path.join(os.path.abspath(path), "bin", "java.exe")
         information["javaw_path"] = os.path.join(os.path.abspath(path), "bin", "javaw.exe")
     else:
-        information["java_path"] = os.path.join(os.path.abspath(path), "bin", "java.exe")
+        information["java_path"] = os.path.join(os.path.abspath(path), "bin", "java")
         information["javaw_path"] = None
 
     return information
 
 
-def _search_java_directory(path: str) -> List[str]:
+def _search_java_directory(path: Union[str, os.PathLike]) -> List[str]:
     "Used by find_system_java_versions() to parse a Directory"
     if not os.path.isdir(path):
         return []
 
     java_list: List[str] = []
     for i in os.listdir(path):
         current_entry = os.path.join(path, i)
@@ -59,15 +59,15 @@
 
         if os.path.isfile(os.path.join(current_entry, "bin", "java")) or os.path.isfile(os.path.join(current_entry, "bin", "java.exe")):
             java_list.append(current_entry)
 
     return java_list
 
 
-def find_system_java_versions(additional_directories: Optional[List[str]] = None) -> List[str]:
+def find_system_java_versions(additional_directories: Optional[List[Union[str, os.PathLike]]] = None) -> List[str]:
     """
     Try to find all Java Versions installed on the System. You can use this to e.g. let the User choose between different Java Versions in a Dropdown.
 
     :param additional_directories: A List of additional Directories to search for Java in custom locations
     :return: A List with all Directories of Java Installations
 
     macOS is not supported yet
@@ -84,15 +84,15 @@
     if additional_directories is not None:
         for i in additional_directories:
             java_list += _search_java_directory(i)
 
     return java_list
 
 
-def find_system_java_versions_information(additional_directories: Optional[List[str]] = None) -> List[JavaInformation]:
+def find_system_java_versions_information(additional_directories: Optional[List[Union[str, os.PathLike]]] = None) -> List[JavaInformation]:
     """
     Same as :func:`find_system_java_version`, but uses :func:`get_java_information` to get some Information about the Installation instead of just proving a Path.
 
     :param additional_directories: A List of additional Directories to search for Java in custom locations
     :return: A List with Information of Java Installations
 
     macOS is not supported yet
```

### Comparing `minecraft-launcher-lib-6.0/minecraft_launcher_lib/microsoft_account.py` & `minecraft-launcher-lib-6.1/minecraft_launcher_lib/microsoft_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 microsoft_account contains functions for login with a Microsoft Account. Before using this module you need to `create a Azure application <https://docs.microsoft.com/en-us/azure/active-directory/develop/quickstart-register-app>`_.
 Many thanks to wiki.vg for it's `documentation of the login process <https://wiki.vg/Microsoft_Authentication_Scheme>`_.
 You may want to read the :doc:`/tutorial/microsoft_login` tutorial before using this module.
 For a list of all types see :doc:`microsoft_types`.
 """
 from .microsoft_types import AuthorizationTokenResponse, XBLResponse, XSTSResponse, MinecraftAuthenticateResponse, MinecraftStoreResponse, MinecraftProfileResponse, CompleteLoginResponse
-from typing import Literal, Optional, Tuple, cast
+from .exceptions import InvalidRefreshToken, AzureAppNotPermitted
 from ._helper import get_user_agent, assert_func
-from .exceptions import InvalidRefreshToken
+from typing import Literal, Optional, Tuple, cast
 from base64 import urlsafe_b64encode
 from hashlib import sha256
 import urllib.parse
 import requests
 import secrets
 
 __AUTH_URL__ = "https://login.microsoftonline.com/consumers/oauth2/v2.0/authorize"
@@ -296,14 +296,15 @@
     Do the complete login process.
 
     :param client_id: The Client ID of your Azure App
     :param client_secret: The Client Secret of your Azure App. This is deprecated and should not been used anymore.
     :param redirect_uri: The Redirect URI of your Azure App
     :param auth_code: The Code you get from :func:`parse_auth_code_url`
     :param code_verifier: The 3rd entry in the Tuple you get from :func:`get_secure_login_data`
+    :raises AzureAppNotPermitted: Your Azure App don't have the Permission to use the Minecraft API
 
     It returns the following:
 
     .. code:: json
 
         {
             "id" : "The uuid",
@@ -327,14 +328,18 @@
     xbl_token = xbl_request["Token"]
     userhash = xbl_request["DisplayClaims"]["xui"][0]["uhs"]
 
     xsts_request = authenticate_with_xsts(xbl_token)
     xsts_token = xsts_request["Token"]
 
     account_request = authenticate_with_minecraft(userhash, xsts_token)
+
+    if "access_token" not in account_request:
+        raise AzureAppNotPermitted()
+
     access_token = account_request["access_token"]
 
     profile = cast(CompleteLoginResponse, get_profile(access_token))
 
     profile["access_token"] = account_request["access_token"]
     profile["refresh_token"] = token_request["refresh_token"]
 
@@ -345,14 +350,15 @@
     """
     Do the complete login process with a refresh token. It returns the same as :func:`complete_login`.
 
     :param client_id: The Client ID of your Azure App
     :param client_secret: The Client Secret of your Azure App. This is deprecated and should not been used anymore.
     :param redirect_uri: The Redirect URI of Azure App. This Parameter only exists for backwards compatibility and is not used anymore.
     :param refresh_token: Your refresh token
+    :raises InvalidRefreshToken: Your refresh token is not valid
 
     Raises a :class:`~minecraft_launcher_lib.exceptions.InvalidRefreshToken` exception when the refresh token is invalid.
     """
     token_request = refresh_authorization_token(client_id, client_secret, redirect_uri, refresh_token)
 
     if "error" in token_request:
         raise InvalidRefreshToken()
```

### Comparing `minecraft-launcher-lib-6.0/minecraft_launcher_lib/microsoft_types.py` & `minecraft-launcher-lib-6.1/minecraft_launcher_lib/microsoft_types.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.0/minecraft_launcher_lib/mrpack.py` & `minecraft-launcher-lib-6.1/minecraft_launcher_lib/mrpack.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,22 +95,28 @@
         mrpack_install_options = {}
 
     with zipfile.ZipFile(path, "r") as zf:
         with zf.open("modrinth.index.json", "r") as f:
             index: MrpackIndex = json.load(f)
 
         # Download the files
-        for file in _filter_mrpack_files(index["files"], mrpack_install_options):
+        callback.get("setStatus", empty)("Download mrpack files")
+        file_list = _filter_mrpack_files(index["files"], mrpack_install_options)
+        callback.get("setMax", empty)(len(file_list))
+        for count, file in enumerate(file_list):
             full_path = os.path.abspath(os.path.join(modpack_directory, file["path"]))
 
             check_path_inside_minecraft_directory(modpack_directory, full_path)
 
             download_file(file["downloads"][0], full_path, sha1=file["hashes"]["sha1"], callback=callback)
 
+            callback.get("setProgress", empty)(count + 1)
+
         # Extract the overrides
+        callback.get("setStatus", empty)("Extract overrides")
         for zip_name in zf.namelist():
             # Check if the entry is in the overrides and if it is a file
             if (not zip_name.startswith("overrides/") and not zip_name.startswith("client-overrides/")) or zf.getinfo(zip_name).file_size == 0:
                 continue
 
             # Remove the overrides at the start of the Name
             # We don't have removeprefix() in Python 3.8
@@ -120,14 +126,15 @@
                 file_name = zip_name[len("overrides/"):]
 
             # Constructs the full Path
             full_path = os.path.abspath(os.path.join(modpack_directory, file_name))
 
             check_path_inside_minecraft_directory(modpack_directory, full_path)
 
+            callback.get("setStatus", empty)(f"Extract {zip_name}]")
             zf.extract(zip_name, full_path)
 
         if mrpack_install_options.get("skipDependenciesInstall"):
             return
 
         # Install dependencies
         callback.get("setStatus", empty)("Installing Minecraft " + index["dependencies"]["minecraft"])
```

### Comparing `minecraft-launcher-lib-6.0/minecraft_launcher_lib/natives.py` & `minecraft-launcher-lib-6.1/minecraft_launcher_lib/natives.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     :raises FileOutsideMinecraftDirectory: A File should be placed outside the given Minecraft directory
 
     The natives are all extracted while installing. So you don't need to use this function in most cases.
     """
     if not os.path.isfile(os.path.join(path, "versions", versionid, versionid + ".json")):
         raise VersionNotFound(versionid)
 
-    with open(os.path.join(path, "versions", versionid, versionid + ".json")) as f:
+    with open(os.path.join(path, "versions", versionid, versionid + ".json"), "r", encoding="utf-8") as f:
         data: ClientJson = json.load(f)
 
     for i in data["libraries"]:
         # Check, if the rules allow this lib for the current system
         if "rules" in i and not parse_rule_list(i["rules"], {}):
             continue
```

### Comparing `minecraft-launcher-lib-6.0/minecraft_launcher_lib/quilt.py` & `minecraft-launcher-lib-6.1/minecraft_launcher_lib/quilt.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.0/minecraft_launcher_lib/runtime.py` & `minecraft-launcher-lib-6.1/minecraft_launcher_lib/runtime.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.0/minecraft_launcher_lib/types.py` & `minecraft-launcher-lib-6.1/minecraft_launcher_lib/types.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.0/minecraft_launcher_lib/utils.py` & `minecraft-launcher-lib-6.1/minecraft_launcher_lib/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 "utils contains a few functions for helping you that doesn't fit in any other category"
 from .types import Articles, MinecraftOptions, LatestMinecraftVersions, MinecraftVersionInfo
 from ._internal_types.shared_types import ClientJson, VersionListManifestJson
-from ._helper import get_requests_response_cache
+from ._helper import get_requests_response_cache, assert_func
 from typing import List, Union
 from datetime import datetime
 import platform
 import requests
 import random
 import pathlib
 import shutil
@@ -189,7 +189,23 @@
 def is_platform_supported() -> bool:
     """
     Checks if the current platform is supported
     """
     if platform.system() not in ["Windows", "Darwin", "Linux"]:
         return False
     return True
+
+
+def is_minecraft_installed(minecraft_directory: Union[str, os.PathLike]) -> bool:
+    """
+    Checks, if there is already a existing Minecraft Installation in the given Directory
+
+    :param minecraft_directory: The path to your Minecraft directory
+    :return: Is a Installation is found
+    """
+    try:
+        assert_func(os.path.isdir(os.path.join(minecraft_directory, "versions")))
+        assert_func(os.path.isdir(os.path.join(minecraft_directory, "libraries")))
+        assert_func(os.path.isdir(os.path.join(minecraft_directory, "assets")))
+        return True
+    except AssertionError:
+        return False
```

### Comparing `minecraft-launcher-lib-6.0/minecraft_launcher_lib/vanilla_launcher.py` & `minecraft-launcher-lib-6.1/minecraft_launcher_lib/vanilla_launcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -175,15 +175,16 @@
     new_profile["name"] = vanilla_profile["name"]
 
     if vanilla_profile["versionType"] == "latest-release":
         new_profile["lastVersionId"] = "latest-release"
     elif vanilla_profile["versionType"] == "latest-snapshot":
         new_profile["lastVersionId"] = "latest-snapshot"
     elif vanilla_profile["versionType"] == "custom":
-        new_profile["lastVersionId"] = "version"
+        # _is_vanilla_launcher_profile_valid() ensures that version is not None, when versionType is set to custom, so we can ignore the mypy error here
+        new_profile["lastVersionId"] = vanilla_profile["version"]  # type: ignore
 
     if (game_directory := vanilla_profile.get("gameDirectory")) is not None:
         new_profile["gameDir"] = game_directory
 
     if (java_executable := vanilla_profile.get("javaExecutable")) is not None:
         new_profile["javaDir"] = java_executable
```

### Comparing `minecraft-launcher-lib-6.0/minecraft_launcher_lib.egg-info/PKG-INFO` & `minecraft-launcher-lib-6.1/minecraft_launcher_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minecraft-launcher-lib
-Version: 6.0
+Version: 6.1
 Summary: A library for creating a custom Minecraft launcher
 Author-email: JakobDev <jakobdev@gmx.de>
 License: BSD-2-Clause
 Project-URL: Documentation, https://minecraft-launcher-lib.readthedocs.io/en/stable/index.html
 Project-URL: Issues, https://codeberg.org/JakobDev/minecraft-launcher-lib/issues
 Project-URL: Source, https://codeberg.org/JakobDev/minecraft-launcher-lib
 Project-URL: Changelog, https://minecraft-launcher-lib.readthedocs.io/en/stable/changelog.html
```

### Comparing `minecraft-launcher-lib-6.0/minecraft_launcher_lib.egg-info/SOURCES.txt` & `minecraft-launcher-lib-6.1/minecraft_launcher_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.0/pyproject.toml` & `minecraft-launcher-lib-6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.0/tests/test_exceptions.py` & `minecraft-launcher-lib-6.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.0/tests/test_fabric.py` & `minecraft-launcher-lib-6.1/tests/test_fabric.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.0/tests/test_forge.py` & `minecraft-launcher-lib-6.1/tests/test_forge.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.0/tests/test_mrpack.py` & `minecraft-launcher-lib-6.1/tests/test_mrpack.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,14 +163,16 @@
     with pytest.raises(minecraft_launcher_lib.exceptions.FileOutsideMinecraftDirectory):
         minecraft_launcher_lib.mrpack.install_mrpack(_create_test_index_pack(index, tmp_path, overrides=["../overrides.txt"]), fifth_dir, mrpack_install_options={"skipDependenciesInstall": True})
 
 
 def test_mrpack_launch_version(tmp_path) -> None:
     index = _get_test_index()
 
+    assert minecraft_launcher_lib.mrpack.get_mrpack_launch_version(_create_test_index_pack(index, tmp_path)) == "1.19"
+
     index["dependencies"]["forge"] = "41.1.0"
     assert minecraft_launcher_lib.mrpack.get_mrpack_launch_version(_create_test_index_pack(index, tmp_path)) == "1.19-forge-41.1.0"
     del index["dependencies"]["forge"]
 
     index["dependencies"]["fabric-loader"] = "0.14.15"
     assert minecraft_launcher_lib.mrpack.get_mrpack_launch_version(_create_test_index_pack(index, tmp_path)) == "fabric-loader-0.14.15-1.19"
     del index["dependencies"]["fabric-loader"]
```

### Comparing `minecraft-launcher-lib-6.0/tests/test_quilt.py` & `minecraft-launcher-lib-6.1/tests/test_quilt.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.0/tests/test_runtime.py` & `minecraft-launcher-lib-6.1/tests/test_runtime.py`

 * *Files identical despite different names*

