# Comparing `tmp/pants-backend-kustomize-0.1.2.tar.gz` & `tmp/pants-backend-kustomize-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pants-backend-kustomize-0.1.2.tar", last modified: Fri Feb 10 15:51:28 2023, max compression
+gzip compressed data, was "pants-backend-kustomize-0.2.0.tar", last modified: Sun Jun 18 19:14:14 2023, max compression
```

## Comparing `pants-backend-kustomize-0.1.2.tar` & `pants-backend-kustomize-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-02-10 15:51:28.489373 pants-backend-kustomize-0.1.2/LICENSE-MIT.txt
--rw-r--r--   0        0        0     1408 2023-02-10 15:51:28.489373 pants-backend-kustomize-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-02-10 15:51:28.489373 pants-backend-kustomize-0.1.2/pants_backend_kustomize/__init__.py
--rw-r--r--   0        0        0     2778 2023-02-10 15:51:28.489373 pants-backend-kustomize-0.1.2/pants_backend_kustomize/codegen.py
--rw-r--r--   0        0        0      465 2023-02-10 15:51:28.489373 pants-backend-kustomize-0.1.2/pants_backend_kustomize/register.py
--rw-r--r--   0        0        0     2587 2023-02-10 15:51:28.489373 pants-backend-kustomize-0.1.2/pants_backend_kustomize/requests.py
--rw-r--r--   0        0        0     1384 2023-02-10 15:51:28.489373 pants-backend-kustomize-0.1.2/pants_backend_kustomize/subsystem.py
--rw-r--r--   0        0        0     1945 2023-02-10 15:51:28.489373 pants-backend-kustomize-0.1.2/pants_backend_kustomize/target_types.py
--rw-r--r--   0        0        0     3938 2023-02-10 15:51:28.489373 pants-backend-kustomize-0.1.2/pants_backend_kustomize/util_rules/prepare_context.py
--rw-r--r--   0        0        0     1131 2023-02-10 15:51:28.489373 pants-backend-kustomize-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2088 1970-01-01 00:00:00.000000 pants-backend-kustomize-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-18 19:14:14.607641 pants-backend-kustomize-0.2.0/LICENSE-MIT.txt
+-rw-r--r--   0        0        0     1408 2023-06-18 19:14:14.607641 pants-backend-kustomize-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-18 19:14:14.607641 pants-backend-kustomize-0.2.0/pants_backend_kustomize/__init__.py
+-rw-r--r--   0        0        0     2799 2023-06-18 19:14:14.607641 pants-backend-kustomize-0.2.0/pants_backend_kustomize/codegen.py
+-rw-r--r--   0        0        0      465 2023-06-18 19:14:14.607641 pants-backend-kustomize-0.2.0/pants_backend_kustomize/register.py
+-rw-r--r--   0        0        0     2233 2023-06-18 19:14:14.607641 pants-backend-kustomize-0.2.0/pants_backend_kustomize/requests.py
+-rw-r--r--   0        0        0     1299 2023-06-18 19:14:14.607641 pants-backend-kustomize-0.2.0/pants_backend_kustomize/subsystem.py
+-rw-r--r--   0        0        0     1903 2023-06-18 19:14:14.607641 pants-backend-kustomize-0.2.0/pants_backend_kustomize/target_types.py
+-rw-r--r--   0        0        0     3938 2023-06-18 19:14:14.607641 pants-backend-kustomize-0.2.0/pants_backend_kustomize/util_rules/prepare_context.py
+-rw-r--r--   0        0        0     1129 2023-06-18 19:14:14.607641 pants-backend-kustomize-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2088 1970-01-01 00:00:00.000000 pants-backend-kustomize-0.2.0/PKG-INFO
```

### Comparing `pants-backend-kustomize-0.1.2/LICENSE-MIT.txt` & `pants-backend-kustomize-0.2.0/LICENSE-MIT.txt`

 * *Files identical despite different names*

### Comparing `pants-backend-kustomize-0.1.2/README.md` & `pants-backend-kustomize-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pants-backend-kustomize-0.1.2/pants_backend_kustomize/codegen.py` & `pants-backend-kustomize-0.2.0/pants_backend_kustomize/codegen.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,22 +21,24 @@
 class GenerateKubernetesFromKustomizeRequest(GenerateSourcesRequest):
     input = KustomizeSourcesField
     output = KubernetesSourceField
 
 
 @rule
 async def generate_kubernetes_from_kustomize(
-    request: GenerateKubernetesFromKustomizeRequest, kustomize: KustomizeTool
+    request: GenerateKubernetesFromKustomizeRequest,
+    kustomize: KustomizeTool,
+    platform: Platform,
 ) -> GeneratedSources:
     (context, kustomize) = await MultiGet(
         Get(KustomizationContext, KustomizationContextRequest(request.protocol_target)),
         Get(
             DownloadedExternalTool,
             ExternalToolRequest,
-            kustomize.get_request(Platform.current),
+            kustomize.get_request(platform),
         ),
     )
 
     merged_digest = await Get(
         Digest,
         MergeDigests(
             [context.digest, kustomize.digest],
```

### Comparing `pants-backend-kustomize-0.1.2/pants_backend_kustomize/requests.py` & `pants-backend-kustomize-0.2.0/pants_backend_kustomize/requests.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,48 +4,35 @@
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import ClassVar
 
 from pants.engine.addresses import Address
+from pants.engine.environment import EnvironmentName
 from pants.engine.rules import collect_rules, rule
 from pants.engine.target import FieldSet, Target
 from pants.engine.unions import UnionMembership, union
 from pants.util.strutil import bullet_list
-from pants.version import PANTS_SEMVER, Version
 
 
 @dataclass(frozen=True)
 class KustomizeInjectRequestQuery:
     """Query for whether the provided target can be the source of Kustomize injection data."""
 
     target: Target
 
 
-if PANTS_SEMVER >= Version("2.15.0.dev0"):
-    from pants.engine.environment import EnvironmentName
-
-    @union(in_scope_types=[EnvironmentName])
-    @dataclass(frozen=True)
-    class KustomizeInjectRequest:
-        """Base class for requests to generate data for Kustomize injection."""
-
-        target: Target
-        field_set_type: ClassVar[type[FieldSet]]
-
-else:
-
-    @union
-    @dataclass(frozen=True)
-    class KustomizeInjectRequest:
-        """Base class for requests to generate data for Kustomize injection."""
+@union(in_scope_types=[EnvironmentName])
+@dataclass(frozen=True)
+class KustomizeInjectRequest:
+    """Base class for requests to generate data for Kustomize injection."""
 
-        target: Target
-        field_set_type: ClassVar[type[FieldSet]]
+    target: Target
+    field_set_type: ClassVar[type[FieldSet]]
 
 
 @dataclass(frozen=True)
 class KustomizeInjectData:
     """Base class for requests to generate data for Kustomize injection."""
 
     address: Address
```

### Comparing `pants-backend-kustomize-0.1.2/pants_backend_kustomize/subsystem.py` & `pants-backend-kustomize-0.2.0/pants_backend_kustomize/subsystem.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 
     def generate_url(self, plat: Platform) -> str:
         platform_mapping = {
             "macos_arm64": "darwin_arm64",
             "macos_x86_64": "darwin_amd64",
             "linux_arm64": "linux_arm64",
             "linux_x86_64": "linux_amd64",
-            "linux_arm64": "linux_arm64",
-            "linux_x86_64": "linux_amd64",
         }
         plat_str = platform_mapping[plat.value]
         base = "https://github.com/kubernetes-sigs/kustomize/releases/download/kustomize"
         return f"{base}/{self.version}/kustomize_{self.version}_{plat_str}.tar.gz"
 
     def generate_exe(self, _: Platform) -> str:
         return "./kustomize"
```

### Comparing `pants-backend-kustomize-0.1.2/pants_backend_kustomize/target_types.py` & `pants-backend-kustomize-0.2.0/pants_backend_kustomize/target_types.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,56 +23,50 @@
 class KustomizeSourceField(SingleSourceField):
     """A file included in a kustomize run. Likely a .yml or .yaml, but could also be other artifacts
     consumed by secret/cm generators."""
 
     expected_file_extensions = (".yaml", ".yml")
     uses_source_roots = False
 
-    help = softwrap(
-        """
+    help = softwrap("""
         A source file included in a kustomize run. Most likely this'll be other .yaml or .yml files,
         but any other resource that can be put into Kubernetes is valid.
-        """
-    )
+        """)
 
 
 class KustomizeSourcesField(MultipleSourcesField):
     """A set of files feeding into kustomize."""
 
     alias = "sources"
     uses_source_roots = False
 
-    help = softwrap(
-        """
+    help = softwrap("""
         A group of files used in a kustomize target.
-        """
-    )
+        """)
 
 
 class KustomizeTarget(Target):
     alias = "kustomize"
     core_fields = (
         *COMMON_TARGET_FIELDS,
         KustomizeDependenciesField,
         KustomizeSourcesField,
     )
-    help = softwrap(
-        """A target for converting a kustomization.yaml and dependencies into a YAML document for
+    help = softwrap("""A target for converting a kustomization.yaml and dependencies into a YAML document for
         use with kubectl.
 
         Example BUILD file:
 
             kustomize(
                 name="kustomize",
                 root_src="kustomization.yaml",
                 dependencies=[],
                 sources=["namespace.yaml", "deployment.yaml", "service.yaml"],
             )
-        """
-    )
+        """)
 
 
 def targets():
     return [
         KustomizeTarget,
     ]
```

### Comparing `pants-backend-kustomize-0.1.2/pants_backend_kustomize/util_rules/prepare_context.py` & `pants-backend-kustomize-0.2.0/pants_backend_kustomize/util_rules/prepare_context.py`

 * *Files identical despite different names*

### Comparing `pants-backend-kustomize-0.1.2/pyproject.toml` & `pants-backend-kustomize-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "pants_backend_kustomize"
 description = "A Kustomize plugin for the Pants build system"
-version = "0.1.2"
+version = "0.2.0"
 authors = [
     { name = "Tom Solberg", email = "me@sbg.dev" },
 ]
 dependencies = [
-    "pants_backend_k8s~=0.1.1",
+    "pants_backend_k8s>=0.2",
 ]
 readme = "README.md"
 keywords = [
     "pantsbuild",
     "pants",
     "backend",
     "kustomize",
```

### Comparing `pants-backend-kustomize-0.1.2/PKG-INFO` & `pants-backend-kustomize-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pants_backend_kustomize
-Version: 0.1.2
+Version: 0.2.0
 Summary: A Kustomize plugin for the Pants build system
 Keywords: pantsbuild,pants,backend,kustomize,kubernetes
 Author-email: Tom Solberg <me@sbg.dev>
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Build Tools
 Project-URL: Changelog, https://github.com/tgolsson/pants-backends/tree/main/pants-plugins/kustomize/CHANGELOG.md
```

