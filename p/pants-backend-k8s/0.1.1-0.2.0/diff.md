# Comparing `tmp/pants-backend-k8s-0.1.1.tar.gz` & `tmp/pants-backend-k8s-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pants-backend-k8s-0.1.1.tar", last modified: Thu Nov 17 21:41:30 2022, max compression
+gzip compressed data, was "pants-backend-k8s-0.2.0.tar", last modified: Sun Jun 18 19:14:14 2023, max compression
```

## Comparing `pants-backend-k8s-0.1.1.tar` & `pants-backend-k8s-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0 ts        (1000) ts        (1000)     1068 2022-11-17 21:41:30.299539 pants-backend-k8s-0.1.1/LICENSE-MIT.txt
--rw-r--r--   0 ts        (1000) ts        (1000)     2698 2022-11-17 21:41:30.299539 pants-backend-k8s-0.1.1/README.md
--rw-r--r--   0 ts        (1000) ts        (1000)        0 2022-11-17 21:41:30.299539 pants-backend-k8s-0.1.1/pants_backend_k8s/__init__.py
--rw-r--r--   0 ts        (1000) ts        (1000)        0 2022-11-17 21:41:30.299539 pants-backend-k8s-0.1.1/pants_backend_k8s/goals/__init__.py
--rw-r--r--   0 ts        (1000) ts        (1000)     5501 2022-11-17 21:41:30.299539 pants-backend-k8s-0.1.1/pants_backend_k8s/goals/run.py
--rw-r--r--   0 ts        (1000) ts        (1000)      295 2022-11-17 21:41:30.299539 pants-backend-k8s-0.1.1/pants_backend_k8s/register.py
--rw-r--r--   0 ts        (1000) ts        (1000)     1010 2022-11-17 21:41:30.299539 pants-backend-k8s-0.1.1/pants_backend_k8s/subsystem.py
--rw-r--r--   0 ts        (1000) ts        (1000)     4287 2022-11-17 21:41:30.299539 pants-backend-k8s-0.1.1/pants_backend_k8s/target_generators.py
--rw-r--r--   0 ts        (1000) ts        (1000)     2420 2022-11-17 21:41:30.299539 pants-backend-k8s-0.1.1/pants_backend_k8s/target_types.py
--rw-r--r--   0 ts        (1000) ts        (1000)     1052 2022-11-17 21:41:30.299539 pants-backend-k8s-0.1.1/pyproject.toml
--rw-------   0 ts        (1000) ts        (1000)     3351 2022-11-17 21:41:30.409539 pants-backend-k8s-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-18 19:14:14.607641 pants-backend-k8s-0.2.0/LICENSE-MIT.txt
+-rw-r--r--   0        0        0     3619 2023-06-18 19:14:14.607641 pants-backend-k8s-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-18 19:14:14.607641 pants-backend-k8s-0.2.0/pants_backend_k8s/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-18 19:14:14.607641 pants-backend-k8s-0.2.0/pants_backend_k8s/goals/__init__.py
+-rw-r--r--   0        0        0     6531 2023-06-18 19:14:14.607641 pants-backend-k8s-0.2.0/pants_backend_k8s/goals/run.py
+-rw-r--r--   0        0        0      295 2023-06-18 19:14:14.607641 pants-backend-k8s-0.2.0/pants_backend_k8s/register.py
+-rw-r--r--   0        0        0     1034 2023-06-18 19:14:14.607641 pants-backend-k8s-0.2.0/pants_backend_k8s/subsystem.py
+-rw-r--r--   0        0        0     4246 2023-06-18 19:14:14.607641 pants-backend-k8s-0.2.0/pants_backend_k8s/target_generators.py
+-rw-r--r--   0        0        0     2392 2023-06-18 19:14:14.607641 pants-backend-k8s-0.2.0/pants_backend_k8s/target_types.py
+-rw-r--r--   0        0        0     1052 2023-06-18 19:14:14.607641 pants-backend-k8s-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4272 1970-01-01 00:00:00.000000 pants-backend-k8s-0.2.0/PKG-INFO
```

### Comparing `pants-backend-k8s-0.1.1/LICENSE-MIT.txt` & `pants-backend-k8s-0.2.0/LICENSE-MIT.txt`

 * *Files identical despite different names*

### Comparing `pants-backend-k8s-0.1.1/README.md` & `pants-backend-k8s-0.2.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-:warning: This plugin is in development. No stability is guaranteed! Contributions welcome.
-
 # Kubernetes backend for Pants
 
+![PyPI](https://img.shields.io/pypi/v/pants-backend-k8s?label=Latest%20release)
+
+> **Warning**
+> This plugin is in development. No stability is guaranteed! Contributions welcome.
+
 This backends implements targets for working with Kubernetes clusters using raw YAML.
 
 * [kubectl](https://github.com/kubernetes/kubectl) for cluster operations
 
 ## Targets
 
 There's currently three targets for `pants-backend-k8s`:
@@ -24,18 +27,18 @@
     source="namespace.yaml",
 )
 ```
 
 
 | Argument | Meaning | Default value |
 | --- | --- | --- |
-| name | The target name | Same as any other target, which is the directory name |
-| source | The raw file | Required |
-| decsription | A description of the target | "" |
-| tags | List of tags | [] |
+| `name` | The target name | Same as any other target, which is the directory name |
+| `source` | The raw file | **Required** |
+| `decsription` | A description of the target |  |
+| `tags` | List of tags | `[]` |
 
 
 This'll eventually be automated like other rules once a suitable heuristic for generation with tailor is found. PRs welcome!
 
 
 ### `k8s_object`
 
@@ -48,22 +51,22 @@
     template=[":kustomize"],
     namespace="chat-app",
     cluster="prod",
 )
 ```
 
 
-| Argument | Meaning | Default value |
-| --- | --- | --- |
-| name | The target name | Same as any other target, which is the directory name |
-| template | The target to act on | Required |
-| namespace | Namespace to target | Optional, will use default kubectl namespace |
-| cluster | cluster to target | Optional, will use default kubectl cluster |
-| decsription | A description of the target | "" |
-| tags | List of tags | [] |
+| Argument      | Meaning                     | Default value                                         |
+|---------------|-----------------------------|-------------------------------------------------------|
+| `name`        | The target name             | Same as any other target, which is the directory name |
+| `template`    | The target to act on        | **Required**                                          |
+| `namespace`   | Namespace to target         | Optional, will use default kubectl namespace          |
+| `cluster`     | cluster to target           | Optional, will use default kubectl cluster            |
+| `decsription` | A description of the target |                                                       |
+| `tags`        | List of tags                | `[]`                                                  |
 
 `k8s_object` is a generator for `kubernetes` target parametrized by the potential commands that are available: `apply`,
 `create`, `get`, `describe`, `replace`, and `delete`.
 
 ### `k8s_objects`
 
 A collection of kubernetes objects that should be managed together.
@@ -73,16 +76,16 @@
     name="my-service",
     description="all components of service-x"
     objects=[":namespace", ":deployment"],
 )
 ```
 
 
-| Argument | Meaning | Default value |
-| --- | --- | --- |
-| name | The target name | Same as any other target, which is the directory name |
-| objects | k8s_object targets that should be managed | Required |
-| decsription | A description of the target | "" |
-| tags | List of tags | [] |
+| Argument      | Meaning                                   | Default value                                         |
+|---------------|-------------------------------------------|-------------------------------------------------------|
+| `name`        | The target name                           | Same as any other target, which is the directory name |
+| `objects`     | k8s_object targets that should be managed | **Required**                                          |
+| `decsription` | A description of the target               |                                                       |
+| `tags`        | List of tags                              | `[]`                                                  |
 
 Like `k8s_object`, `k8s_objects` is a generator for parametrized targets for the commands that are available: `apply`,
 `create`, `get`, `describe`, `replace`, and `delete`.
```

### Comparing `pants-backend-k8s-0.1.1/pants_backend_k8s/subsystem.py` & `pants-backend-k8s-0.2.0/pants_backend_k8s/subsystem.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 
 class KubernetesTool(ExternalTool):
     options_scope = "kubectl-tool"
     help = "Wrapper for kubectl."
 
     default_version = "v1.25.2"
     default_known_versions = [
-        "v1.25.2|macos_arm64 |3c1e8b95cef4ff6e52d5f4b8c65b8d9d06b75f42d1cb40986c1d67729d82411a|10169842",  # noqa
+        (  # noqa
+            "v1.25.2|macos_arm64 |3c1e8b95cef4ff6e52d5f4b8c65b8d9d06b75f42d1cb40986c1d67729d82411a|10169842"
+        ),
         "v1.25.2|macos_x86_64|6fd57e78ed0c06b5bdd82750c5dc6d0f992a7b926d114fe94be46d7a7e32b63a|10496583",  # noqa
         "v1.25.2|linux_x86_64|8639f2b9c33d38910d706171ce3d25be9b19fc139d0e3d4627f38ce84f9040eb|45015040",  # noqa
     ]
 
     def generate_url(self, plat: Platform) -> str:
         platform_mapping = {
             "macos_arm64": "darwin/arm64",
```

### Comparing `pants-backend-k8s-0.1.1/pants_backend_k8s/target_generators.py` & `pants-backend-k8s-0.2.0/pants_backend_k8s/target_generators.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,33 +9,32 @@
     GeneratedTargets,
     GenerateTargetsRequest,
     Target,
     TargetGenerator,
 )
 from pants.engine.unions import UnionMembership, UnionRule
 from pants.util.strutil import softwrap
+
 from pants_backend_k8s.target_types import (
     KubernetesClusterField,
     KubernetesCommandField,
     KubernetesKindField,
     KubernetesNamespaceField,
     KubernetesTarget,
     KubernetesTargetBundle,
     KubernetesTargetBundleDependencies,
     KubernetesTemplateDependency,
 )
 
 
 class KubernetesTargetGenerator(TargetGenerator):
     alias = "k8s_object"
-    help = softwrap(
-        """
+    help = softwrap("""
         Generate `kubernetes` targets with all specific commands.
-        """
-    )
+        """)
     generated_target_cls = KubernetesTarget
     core_fields = (
         *COMMON_TARGET_FIELDS,
         KubernetesTemplateDependency,
         KubernetesKindField,
         KubernetesClusterField,
         KubernetesCommandField,
@@ -79,19 +78,17 @@
 @dataclass(frozen=True)
 class KubernetesTargetBundleCommandProcessRequest:
     target: Target
 
 
 class KubernetesTargetBundleGenerator(TargetGenerator):
     alias = "k8s_objects"
-    help = softwrap(
-        """
+    help = softwrap("""
         Generate `kubernetes` targets with all specific commands.
-        """
-    )
+        """)
     generated_target_cls = ShellCommandRunTarget
     core_fields = (
         *COMMON_TARGET_FIELDS,
         KubernetesTargetBundleDependencies,
     )
     copied_fields = COMMON_TARGET_FIELDS
     moved_fields = (KubernetesTargetBundleDependencies,)
@@ -123,17 +120,15 @@
             {
                 ShellCommandCommandField.alias: cli,
             },
             request.template_address.create_generated(command),
             union_membership,
         )
 
-    result = [
-        await create_tgt(c) for c in ("apply", "describe", "delete", "get", "replace", "create")
-    ]
+    result = [await create_tgt(c) for c in ("apply", "describe", "delete", "get", "replace", "create")]
 
     return GeneratedTargets(generator, result)
 
 
 def targets():
     return [
         KubernetesTargetGenerator,
```

### Comparing `pants-backend-k8s-0.1.1/pants_backend_k8s/target_types.py` & `pants-backend-k8s-0.2.0/pants_backend_k8s/target_types.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,28 +42,24 @@
 class KubernetesTemplateDependency(Dependencies):
     help = "the name of the dependency to use as the template"
     alias = "template"
 
 
 class KubernetesClusterField(StringField):
     alias = "cluster"
-    help = softwrap(
-        """
+    help = softwrap("""
         The target cluster/context to run on. If not provided; the command cannot be ran.
-        """
-    )
+        """)
 
 
 class KubernetesKindField(StringField):
     alias = "kind"
-    help = softwrap(
-        """
+    help = softwrap("""
         A descriptor of the kinds included.
-        """
-    )
+        """)
 
 
 class KubernetesTarget(Target):
     alias = "kubernetes"
     core_fields = (
         *COMMON_TARGET_FIELDS,
         KubernetesTemplateDependency,
```

### Comparing `pants-backend-k8s-0.1.1/pyproject.toml` & `pants-backend-k8s-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "pants_backend_k8s"
 description = "A Kubernetes plugin for the Pants build system"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
     { name = "Tom Solberg", email = "me@sbg.dev" },
 ]
 dependencies = []
 readme = "README.md"
 keywords = [
     "pantsbuild",
```

