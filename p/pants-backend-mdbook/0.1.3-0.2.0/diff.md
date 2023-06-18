# Comparing `tmp/pants-backend-mdbook-0.1.3.tar.gz` & `tmp/pants-backend-mdbook-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pants-backend-mdbook-0.1.3.tar", last modified: Fri Nov 18 23:05:43 2022, max compression
+gzip compressed data, was "pants-backend-mdbook-0.2.0.tar", last modified: Sun Jun 18 19:14:14 2023, max compression
```

## Comparing `pants-backend-mdbook-0.1.3.tar` & `pants-backend-mdbook-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0 ts        (1000) ts        (1000)     1068 2022-11-18 23:05:43.184026 pants-backend-mdbook-0.1.3/LICENSE-MIT.txt
--rw-r--r--   0 ts        (1000) ts        (1000)      586 2022-11-18 23:05:43.184026 pants-backend-mdbook-0.1.3/README.md
--rw-r--r--   0 ts        (1000) ts        (1000)       99 2022-11-18 23:05:43.184026 pants-backend-mdbook-0.1.3/pants_backend_mdbook/goals/__init__.py
--rw-r--r--   0 ts        (1000) ts        (1000)      881 2022-11-18 23:05:43.184026 pants-backend-mdbook-0.1.3/pants_backend_mdbook/goals/package.py
--rw-r--r--   0 ts        (1000) ts        (1000)      312 2022-11-18 23:05:43.184026 pants-backend-mdbook-0.1.3/pants_backend_mdbook/register.py
--rw-r--r--   0 ts        (1000) ts        (1000)     1102 2022-11-18 23:05:43.184026 pants-backend-mdbook-0.1.3/pants_backend_mdbook/subsystem.py
--rw-r--r--   0 ts        (1000) ts        (1000)      229 2022-11-18 23:05:43.184026 pants-backend-mdbook-0.1.3/pants_backend_mdbook/target_types_rules.py
--rw-r--r--   0 ts        (1000) ts        (1000)      727 2022-11-18 23:05:43.184026 pants-backend-mdbook-0.1.3/pants_backend_mdbook/targets.py
--rw-r--r--   0 ts        (1000) ts        (1000)      152 2022-11-18 23:05:43.184026 pants-backend-mdbook-0.1.3/pants_backend_mdbook/util_rules/__init__.py
--rw-r--r--   0 ts        (1000) ts        (1000)     1593 2022-11-18 23:05:43.184026 pants-backend-mdbook-0.1.3/pants_backend_mdbook/util_rules/build.py
--rw-r--r--   0 ts        (1000) ts        (1000)     2085 2022-11-18 23:05:43.184026 pants-backend-mdbook-0.1.3/pants_backend_mdbook/util_rules/prepare.py
--rw-r--r--   0 ts        (1000) ts        (1000)     1098 2022-11-18 23:05:43.184026 pants-backend-mdbook-0.1.3/pyproject.toml
--rw-------   0 ts        (1000) ts        (1000)     1272 2022-11-18 23:05:43.314026 pants-backend-mdbook-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-18 19:14:14.607641 pants-backend-mdbook-0.2.0/LICENSE-MIT.txt
+-rw-r--r--   0        0        0      726 2023-06-18 19:14:14.607641 pants-backend-mdbook-0.2.0/README.md
+-rw-r--r--   0        0        0       99 2023-06-18 19:14:14.607641 pants-backend-mdbook-0.2.0/pants_backend_mdbook/goals/__init__.py
+-rw-r--r--   0        0        0     1023 2023-06-18 19:14:14.607641 pants-backend-mdbook-0.2.0/pants_backend_mdbook/goals/package.py
+-rw-r--r--   0        0        0      255 2023-06-18 19:14:14.607641 pants-backend-mdbook-0.2.0/pants_backend_mdbook/register.py
+-rw-r--r--   0        0        0     1075 2023-06-18 19:14:14.607641 pants-backend-mdbook-0.2.0/pants_backend_mdbook/subsystem.py
+-rw-r--r--   0        0        0      727 2023-06-18 19:14:14.607641 pants-backend-mdbook-0.2.0/pants_backend_mdbook/targets.py
+-rw-r--r--   0        0        0      152 2023-06-18 19:14:14.607641 pants-backend-mdbook-0.2.0/pants_backend_mdbook/util_rules/__init__.py
+-rw-r--r--   0        0        0     1398 2023-06-18 19:14:14.607641 pants-backend-mdbook-0.2.0/pants_backend_mdbook/util_rules/build.py
+-rw-r--r--   0        0        0     2088 2023-06-18 19:14:14.607641 pants-backend-mdbook-0.2.0/pants_backend_mdbook/util_rules/prepare.py
+-rw-r--r--   0        0        0     1098 2023-06-18 19:14:14.607641 pants-backend-mdbook-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1412 1970-01-01 00:00:00.000000 pants-backend-mdbook-0.2.0/PKG-INFO
```

### Comparing `pants-backend-mdbook-0.1.3/LICENSE-MIT.txt` & `pants-backend-mdbook-0.2.0/LICENSE-MIT.txt`

 * *Files identical despite different names*

### Comparing `pants-backend-mdbook-0.1.3/README.md` & `pants-backend-mdbook-0.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # MDBook backend for Pants
 
+![PyPI](https://img.shields.io/pypi/v/pants-backend-mdbook?label=Latest%20release)
+
 > **Warning**
-> 🚧 Very WIP plugin 🚧
+> This plugin is in development. No stability is guaranteed! Contributions welcome.
 
 This provides a tool for building mdbook targets with pants. There is currently a single very simple rule:
 
 ``` python
 md_book(
     name="my-docs",
     sources=["book.toml", "src/*"],
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pants-backend-mdbook-0.1.3/pants_backend_mdbook/subsystem.py` & `pants-backend-mdbook-0.2.0/pants_backend_mdbook/subsystem.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 
 """
 from __future__ import annotations
 
 from pants.core.util_rules.external_tool import ExternalTool
 from pants.engine.platform import Platform
-from pants.engine.rules import SubsystemRule
 
 _mdbook_platform_mapping = {
     "linux_x86_64": "x86_64-unknown-linux-gnu",
     "macos_x86_64": "x86_64-apple-darwin",
 }
 
 
@@ -21,17 +20,18 @@
     default_known_versions = [
         "v0.4.21|macos_x86_64|c1f3e8235f8b3128f6020397061c97444007e090ac42358402d3f25eee8499bd|4292102",
         "v0.4.21|linux_x86_64|ec3c978a255b444987fd6e0805147f4ea75d221f68c6e27dbf3e8a28aba166b7|4861607",
     ]
 
     def generate_url(self, plat: Platform) -> str:
         plat_str = _mdbook_platform_mapping[plat.value]
-        return f"https://github.com/rust-lang/mdBook/releases/download/{self.version}/mdbook-{self.version}-{plat_str}.tar.gz"
+        base = "https://github.com/rust-lang/mdBook/releases/download"
+        return f"{base}/{self.version}/mdbook-{self.version}-{plat_str}.tar.gz"
 
     def generate_exe(self, plat: Platform) -> str:
         return "./mdbook"
 
 
 def rules():
     return [
-        SubsystemRule(MdBookTool),
+        *MdBookTool.rules(),
     ]
```

### Comparing `pants-backend-mdbook-0.1.3/pants_backend_mdbook/targets.py` & `pants-backend-mdbook-0.2.0/pants_backend_mdbook/targets.py`

 * *Files identical despite different names*

### Comparing `pants-backend-mdbook-0.1.3/pants_backend_mdbook/util_rules/build.py` & `pants-backend-mdbook-0.2.0/pants_backend_mdbook/util_rules/build.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 
 """
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 
-from pants.core.util_rules.external_tool import DownloadedExternalTool, ExternalToolRequest
-from pants.core.util_rules.source_files import SourceFiles, SourceFilesRequest
-from pants.engine.addresses import Address, Addresses
-from pants.engine.fs import Digest, MergeDigests
+from pants.engine.addresses import Address
+from pants.engine.fs import Digest
 from pants.engine.process import Process, ProcessResult
 from pants.engine.rules import Get, collect_rules, rule
+
 from pants_backend_mdbook.subsystem import MdBookTool
 from pants_backend_mdbook.util_rules.prepare import MdBookAnalysis, MdBookAnalysisRequest
 
 
 @dataclass(frozen=True)
 class MdBookBuildOutput:
     digest: Digest | None
```

### Comparing `pants-backend-mdbook-0.1.3/pants_backend_mdbook/util_rules/prepare.py` & `pants-backend-mdbook-0.2.0/pants_backend_mdbook/util_rules/prepare.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from pants.engine.target import (
     InvalidTargetException,
     SourcesField,
     Targets,
     TransitiveTargets,
     TransitiveTargetsRequest,
 )
+
 from pants_backend_mdbook.subsystem import MdBookTool
 from pants_backend_mdbook.targets import MdBookSources
 
 
 @dataclass(frozen=True)
 class MdBookAnalysis:
     digest: Digest
@@ -27,34 +28,35 @@
 
 @dataclass(frozen=True)
 class MdBookAnalysisRequest:
     address: Address
 
 
 @rule(desc="Prepare MD Book Build Context")
-async def prepare_md_book_ctx(request: MdBookAnalysisRequest, mdbook: MdBookTool) -> MdBookAnalysis:
+async def prepare_md_book_ctx(
+    request: MdBookAnalysisRequest, mdbook: MdBookTool, platform: Platform
+) -> MdBookAnalysis:
     (targets, transitive_targets) = await MultiGet(
         Get(Targets, Addresses([request.address])),
         Get(TransitiveTargets, TransitiveTargetsRequest([request.address])),
     )
 
     target = targets[0]
 
     (sources, tool) = await MultiGet(
         Get(
             SourceFiles,
             SourceFilesRequest(
-                [target.get(MdBookSources)]
-                + [t.get(SourcesField) for t in transitive_targets.dependencies],
+                [target.get(MdBookSources)] + [t.get(SourcesField) for t in transitive_targets.dependencies],
             ),
         ),
         Get(
             DownloadedExternalTool,
             ExternalToolRequest,
-            mdbook.get_request(Platform.current),
+            mdbook.get_request(platform),
         ),
     )
 
     build_root = None
     for s in sources.files:
         if s.endswith("book.toml"):
             build_root = os.path.dirname(s)
```

### Comparing `pants-backend-mdbook-0.1.3/pyproject.toml` & `pants-backend-mdbook-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "pants_backend_mdbook"
 description = "A  MdBook documentation builder plugin for the Pants buildsystem."
-version = "0.1.3"
+version = "0.2.0"
 authors = [
     { name = "Tom Solberg", email = "me@sbg.dev" },
 ]
 dependencies = []
 readme = "README.md"
 keywords = [
     "pantsbuild",
```

### Comparing `pants-backend-mdbook-0.1.3/PKG-INFO` & `pants-backend-mdbook-0.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: pants_backend_mdbook
-Version: 0.1.3
+Version: 0.2.0
 Summary: A  MdBook documentation builder plugin for the Pants buildsystem.
 Keywords: pantsbuild,pants,backend,mdbook,markdown
 Author-email: Tom Solberg <me@sbg.dev>
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Build Tools
 Project-URL: Changelog, https://github.com/tgolsson/pants-backends/tree/main/pants-plugins/mdbook/CHANGELOG.md
 Project-URL: Code, https://github.com/tgolsson/pants-backends/tree/main/pants-plugins/mdbook
 Project-URL: Repository, https://github.com/tgolsson/pants-backends
 Description-Content-Type: text/markdown
 
 # MDBook backend for Pants
 
+![PyPI](https://img.shields.io/pypi/v/pants-backend-mdbook?label=Latest%20release)
+
 > **Warning**
-> 🚧 Very WIP plugin 🚧
+> This plugin is in development. No stability is guaranteed! Contributions welcome.
 
 This provides a tool for building mdbook targets with pants. There is currently a single very simple rule:
 
 ``` python
 md_book(
     name="my-docs",
     sources=["book.toml", "src/*"],
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

