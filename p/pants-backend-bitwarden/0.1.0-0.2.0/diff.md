# Comparing `tmp/pants-backend-bitwarden-0.1.0.tar.gz` & `tmp/pants-backend-bitwarden-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pants-backend-bitwarden-0.1.0.tar", last modified: Fri Feb 10 15:51:28 2023, max compression
+gzip compressed data, was "pants-backend-bitwarden-0.2.0.tar", last modified: Sun Jun 18 19:14:14 2023, max compression
```

## Comparing `pants-backend-bitwarden-0.1.0.tar` & `pants-backend-bitwarden-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2023-02-10 15:51:28.459373 pants-backend-bitwarden-0.1.0/LICENSE-MIT.txt
--rw-r--r--   0        0        0     3621 2023-02-10 15:51:28.459373 pants-backend-bitwarden-0.1.0/README.md
--rw-r--r--   0        0        0     1575 2023-02-10 15:51:28.459373 pants-backend-bitwarden-0.1.0/pants_backend_bitwarden/goals/decrypt.py
--rw-r--r--   0        0        0      322 2023-02-10 15:51:28.459373 pants-backend-bitwarden-0.1.0/pants_backend_bitwarden/register.py
--rw-r--r--   0        0        0      937 2023-02-10 15:51:28.459373 pants-backend-bitwarden-0.1.0/pants_backend_bitwarden/subsystem.py
--rw-r--r--   0        0        0     1490 2023-02-10 15:51:28.459373 pants-backend-bitwarden-0.1.0/pants_backend_bitwarden/targets.py
--rw-r--r--   0        0        0     6593 2023-02-10 15:51:28.459373 pants-backend-bitwarden-0.1.0/pants_backend_bitwarden/util_rules/secret.py
--rw-r--r--   0        0        0     1117 2023-02-10 15:51:28.459373 pants-backend-bitwarden-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4290 1970-01-01 00:00:00.000000 pants-backend-bitwarden-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-18 19:14:14.607641 pants-backend-bitwarden-0.2.0/LICENSE-MIT.txt
+-rw-r--r--   0        0        0     3621 2023-06-18 19:14:14.607641 pants-backend-bitwarden-0.2.0/README.md
+-rw-r--r--   0        0        0     1575 2023-06-18 19:14:14.607641 pants-backend-bitwarden-0.2.0/pants_backend_bitwarden/goals/decrypt.py
+-rw-r--r--   0        0        0      322 2023-06-18 19:14:14.607641 pants-backend-bitwarden-0.2.0/pants_backend_bitwarden/register.py
+-rw-r--r--   0        0        0     1003 2023-06-18 19:14:14.607641 pants-backend-bitwarden-0.2.0/pants_backend_bitwarden/subsystem.py
+-rw-r--r--   0        0        0     1490 2023-06-18 19:14:14.607641 pants-backend-bitwarden-0.2.0/pants_backend_bitwarden/targets.py
+-rw-r--r--   0        0        0     6618 2023-06-18 19:14:14.607641 pants-backend-bitwarden-0.2.0/pants_backend_bitwarden/util_rules/secret.py
+-rw-r--r--   0        0        0     1117 2023-06-18 19:14:14.607641 pants-backend-bitwarden-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4290 1970-01-01 00:00:00.000000 pants-backend-bitwarden-0.2.0/PKG-INFO
```

### Comparing `pants-backend-bitwarden-0.1.0/LICENSE-MIT.txt` & `pants-backend-bitwarden-0.2.0/LICENSE-MIT.txt`

 * *Files identical despite different names*

### Comparing `pants-backend-bitwarden-0.1.0/README.md` & `pants-backend-bitwarden-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pants-backend-bitwarden-0.1.0/pants_backend_bitwarden/goals/decrypt.py` & `pants-backend-bitwarden-0.2.0/pants_backend_bitwarden/goals/decrypt.py`

 * *Files identical despite different names*

### Comparing `pants-backend-bitwarden-0.1.0/pants_backend_bitwarden/subsystem.py` & `pants-backend-bitwarden-0.2.0/pants_backend_bitwarden/subsystem.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,7 +25,13 @@
         }
         platform = platform_mapping[plat.value]
         base = "https://github.com/bitwarden/clients/releases/download"
         return f"{base}/cli-v{self.version}/bw-{platform}-{self.version}.zip"
 
     def generate_exe(self, _: Platform) -> str:
         return "./bw"
+
+
+def rules():
+    return [
+        *BitwardenTool.rules(),
+    ]
```

### Comparing `pants-backend-bitwarden-0.1.0/pants_backend_bitwarden/targets.py` & `pants-backend-bitwarden-0.2.0/pants_backend_bitwarden/targets.py`

 * *Files identical despite different names*

### Comparing `pants-backend-bitwarden-0.1.0/pants_backend_bitwarden/util_rules/secret.py` & `pants-backend-bitwarden-0.2.0/pants_backend_bitwarden/util_rules/secret.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 import json
 import os
 from dataclasses import dataclass
 
 from pants.core.util_rules.external_tool import DownloadedExternalTool, ExternalToolRequest
 from pants.engine.addresses import Addresses, UnparsedAddressInputs
-from pants.engine.environment import Environment, EnvironmentRequest
+from pants.engine.env_vars import EnvironmentVars, EnvironmentVarsRequest
 from pants.engine.platform import Platform
 from pants.engine.process import FallibleProcessResult, Process, ProcessCacheScope
 from pants.engine.rules import Get, collect_rules, rule
 from pants.engine.target import FieldSet, WrappedTarget, WrappedTargetRequest
 from pants.engine.unions import UnionRule
 
 from pants_backend_bitwarden.subsystem import BitwardenTool
@@ -106,23 +106,23 @@
         WrappedTargetRequest(
             item[0],
             description_of_origin="Resolve BitWarden ID",
         ),
     )
 
     env_request = ["HOME"]
-    extra_env = Environment()
+    extra_env = EnvironmentVars()
     if wrapped_target.target[BitWardenSessionSecret].value is not None:
         bw_session_secret = await Get(SecretsResponse, BitWardenSessionKeyRequest(wrapped_target.target))
-        extra_env = Environment(**{"BW_SESSION": bw_session_secret.value.value})
+        extra_env = EnvironmentVars(**{"BW_SESSION": bw_session_secret.value.value})
     else:
         env_request.append("BW_SESSION")
 
-    relevant_env = await Get(Environment, EnvironmentRequest(env_request))
-    command_env = Environment(**relevant_env, **extra_env)
+    relevant_env = await Get(EnvironmentVars, EnvironmentVarsRequest(env_request))
+    command_env = EnvironmentVars(**relevant_env, **extra_env)
 
     if request.target.field.value:
         command = [
             f"{bw_tool.exe}",
             "--nointeraction",
             "get",
             "item",
```

### Comparing `pants-backend-bitwarden-0.1.0/pyproject.toml` & `pants-backend-bitwarden-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "pants_backend_bitwarden"
 description = "A Bitwarden plugin for the Pants build system"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
     { name = "Tom Solberg", email = "me@sbg.dev" },
 ]
 dependencies = [
-    "pants_backend_secrets>=0.1.0",
+    "pants_backend_secrets>=0.2.0",
 ]
 readme = "README.md"
 keywords = [
     "pantsbuild",
     "pants",
     "backend",
     "bitwarden",
```

### Comparing `pants-backend-bitwarden-0.1.0/PKG-INFO` & `pants-backend-bitwarden-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pants_backend_bitwarden
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Bitwarden plugin for the Pants build system
 Keywords: pantsbuild,pants,backend,bitwarden
 Author-email: Tom Solberg <me@sbg.dev>
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Build Tools
 Project-URL: Changelog, https://github.com/tgolsson/pants-backends/tree/main/pants-plugins/bitwarden/CHANGELOG.md
```

