# Comparing `tmp/pants-backend-oci-0.3.1.tar.gz` & `tmp/pants_backend_oci-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pants-backend-oci-0.3.1.tar", last modified: Thu Mar 16 22:13:43 2023, max compression
+gzip compressed data, was "pants_backend_oci-0.4.0.tar", last modified: Sun Jun 18 19:14:15 2023, max compression
```

## Comparing `pants-backend-oci-0.3.1.tar` & `pants_backend_oci-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,33 @@
--rw-r--r--   0        0        0     1068 2023-03-16 22:13:43.433439 pants-backend-oci-0.3.1/LICENSE-MIT.txt
--rw-r--r--   0        0        0     7282 2023-03-16 22:13:43.433439 pants-backend-oci-0.3.1/README.md
--rw-r--r--   0        0        0      166 2023-03-16 22:13:43.433439 pants-backend-oci-0.3.1/pants_backend_oci/goals/__init__.py
--rw-r--r--   0        0        0     4349 2023-03-16 22:13:43.433439 pants-backend-oci-0.3.1/pants_backend_oci/goals/package.py
--rw-r--r--   0        0        0     4242 2023-03-16 22:13:43.433439 pants-backend-oci-0.3.1/pants_backend_oci/goals/publish.py
--rw-r--r--   0        0        0     5521 2023-03-16 22:13:43.433439 pants-backend-oci-0.3.1/pants_backend_oci/goals/run.py
--rw-r--r--   0        0        0      191 2023-03-16 22:13:43.433439 pants-backend-oci-0.3.1/pants_backend_oci/language_target/__init__.py
--rw-r--r--   0        0        0     5591 2023-03-16 22:13:43.433439 pants-backend-oci-0.3.1/pants_backend_oci/language_target/python.py
--rw-r--r--   0        0        0      595 2023-03-16 22:13:43.433439 pants-backend-oci-0.3.1/pants_backend_oci/register.py
--rw-r--r--   0        0        0     2524 2023-03-16 22:13:43.433439 pants-backend-oci-0.3.1/pants_backend_oci/rules/kustomize_inject.py
--rw-r--r--   0        0        0     3221 2023-03-16 22:13:43.433439 pants-backend-oci-0.3.1/pants_backend_oci/subsystem.py
--rw-r--r--   0        0        0     1485 2023-03-16 22:13:43.433439 pants-backend-oci-0.3.1/pants_backend_oci/target_types.py
--rw-r--r--   0        0        0     2716 2023-03-16 22:13:43.433439 pants-backend-oci-0.3.1/pants_backend_oci/targets.py
--rw-r--r--   0        0        0     1424 2023-03-16 22:13:43.433439 pants-backend-oci-0.3.1/pants_backend_oci/tools/process.py
--rw-r--r--   0        0        0      398 2023-03-16 22:13:43.433439 pants-backend-oci-0.3.1/pants_backend_oci/util_rules/__init__.py
--rw-r--r--   0        0        0     3166 2023-03-16 22:13:43.433439 pants-backend-oci-0.3.1/pants_backend_oci/util_rules/archive.py
--rw-r--r--   0        0        0     4285 2023-03-16 22:13:43.433439 pants-backend-oci-0.3.1/pants_backend_oci/util_rules/build_image_bundle.py
--rw-r--r--   0        0        0     3130 2023-03-16 22:13:43.433439 pants-backend-oci-0.3.1/pants_backend_oci/util_rules/image_bundle.py
--rw-r--r--   0        0        0     3924 2023-03-16 22:13:43.433439 pants-backend-oci-0.3.1/pants_backend_oci/util_rules/layer.py
--rw-r--r--   0        0        0      941 2023-03-16 22:13:43.433439 pants-backend-oci-0.3.1/pants_backend_oci/util_rules/oci_sha.py
--rw-r--r--   0        0        0     2701 2023-03-16 22:13:43.433439 pants-backend-oci-0.3.1/pants_backend_oci/util_rules/pull_image_bundle.py
--rw-r--r--   0        0        0     1277 2023-03-16 22:13:43.433439 pants-backend-oci-0.3.1/pants_backend_oci/util_rules/unpack.py
--rw-r--r--   0        0        0     1092 2023-03-16 22:13:43.433439 pants-backend-oci-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     7931 1970-01-01 00:00:00.000000 pants-backend-oci-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/LICENSE-MIT.txt
+-rw-r--r--   0        0        0    10372 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/README.md
+-rw-r--r--   0        0        0      223 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/goals/__init__.py
+-rw-r--r--   0        0        0     5081 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/goals/package.py
+-rw-r--r--   0        0        0     2004 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/goals/package_build_step.py
+-rw-r--r--   0        0        0     3814 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/goals/publish.py
+-rw-r--r--   0        0        0     8237 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/goals/run.py
+-rw-r--r--   0        0        0      191 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/language_target/__init__.py
+-rw-r--r--   0        0        0     6414 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/language_target/python.py
+-rw-r--r--   0        0        0      679 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/register.py
+-rw-r--r--   0        0        0     2524 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/rules/kustomize_inject.py
+-rw-r--r--   0        0        0     4438 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/subsystem.py
+-rw-r--r--   0        0        0     1900 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/synthetic_targets.py
+-rw-r--r--   0        0        0     2777 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/target_types.py
+-rw-r--r--   0        0        0     3562 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/targets.py
+-rw-r--r--   0        0        0     1791 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/tools/process.py
+-rw-r--r--   0        0        0      701 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/util_rules/__init__.py
+-rw-r--r--   0        0        0     4932 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/util_rules/archive.py
+-rw-r--r--   0        0        0     1017 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/util_rules/binaries.py
+-rw-r--r--   0        0        0     6046 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/util_rules/build_image_artifact.py
+-rw-r--r--   0        0        0     7725 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/util_rules/build_image_bundle.py
+-rw-r--r--   0        0        0     1232 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/util_rules/configure.py
+-rw-r--r--   0        0        0     2537 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/util_rules/copy.py
+-rw-r--r--   0        0        0     2927 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/util_rules/empty_image_bundle.py
+-rw-r--r--   0        0        0     2856 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/util_rules/image_bundle.py
+-rw-r--r--   0        0        0      920 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/util_rules/jq.py
+-rw-r--r--   0        0        0     5523 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/util_rules/layer.py
+-rw-r--r--   0        0        0      941 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/util_rules/oci_sha.py
+-rw-r--r--   0        0        0     2634 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/util_rules/pull_image_bundle.py
+-rw-r--r--   0        0        0     8311 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/util_rules/run.py
+-rw-r--r--   0        0        0     2562 2023-06-18 19:14:15.497641 pants_backend_oci-0.4.0/pants_backend_oci/util_rules/unpack.py
+-rw-r--r--   0        0        0     1136 2023-06-18 19:14:15.647641 pants_backend_oci-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    12301 1970-01-01 00:00:00.000000 pants_backend_oci-0.4.0/PKG-INFO
```

### Comparing `pants-backend-oci-0.3.1/LICENSE-MIT.txt` & `pants_backend_oci-0.4.0/LICENSE-MIT.txt`

 * *Files identical despite different names*

### Comparing `pants-backend-oci-0.3.1/README.md` & `pants_backend_oci-0.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -12,26 +12,29 @@
 * [skopeo](https://github.com/containers/skopeo) for pulling and pushing images
 
 # Planned and missing features
 
 * Currently there's no support for pulling tags, as that would break determinism
 * Multi-platform SHA/.sig is untested/unsupported
 * skopeo doesn't support MacOS, preventing pulling and pushing images.
-* No empty image base
 * No "in-container" build steps
 
 ## Targets
 
-There's three targets currently implemented:
+There's six targets currently implemented, of which five are generic:
 
 * `oci_pull_image`
 * `oci_pull_images`
-* `oci_build_image`
+* `oci_image_build`
+* `oci_image_empty`
+* `oci_build_layer`
 
-There are also plans to support targets optimized for various languages.
+And one with some special language semantics:
+
+* `oci_python_image` - this is the same as `oci_image_build`, but will prefer to set the entrypoint to `.pex` files.
 
 ### `oci_pull_image`
 
 Pull an image from a repository with a specific digest.
 
 ``` python
 oci_pull_image(
@@ -119,7 +122,48 @@
 | `base`        | The base image to use. Matches the `FROM` directive in a Dockerfile            | **Required**                                          |
 | `packages`    | Packaged targets to include. The first element will be used as the entrypoint. | `[]`                                                  |
 | `python_main` | The main file to run                                                           | The last `.pex` in the dependency list                |
 | `repository`  | Fully qualified repository name                                                | Required when publishing                              |
 | `tag`         | Remote tag to use                                                              | Required when publishing                              |
 | `decsription` | A description of the target                                                    |                                                       |
 | `tags`        | List of tags                                                                   | `[]`                                                  |
+
+### `oci_image_empty`
+
+An empty base image with no contents at all. This is declared as `//:empty` automatically, but you can use this to create new targets.
+
+``` python
+oci_image_empty(
+    name="empty",
+)
+```
+
+| Argument      | Meaning                                                                        | Default value                                         |
+|---------------|--------------------------------------------------------------------------------|-------------------------------------------------------|
+| `name`        | The target name                                                                | Same as any other target, which is the directory name |
+| `decsription` | A description of the target                                                    |                                                       |
+| `tags`        | List of tags                                                                   | `[]`                                                  |
+
+### `oci_build_layer`
+
+Run an image command, and capture the configured output into a layer artifact, that can be injected into other images. This matches the `COPY --from` workflows.
+
+oci_build_layer(
+    name="layer"
+	base=[":rust-1-70"],
+    packages=[":files"],
+    env=['RUSTC_OPTS=...'],
+	command=['cd /my-package && cargo build --release'],
+	outputs=['/my-package/target/release/my-package'],
+)
+```
+
+| Argument      | Meaning                                                                        | Default value                                          |
+|---------------|--------------------------------------------------------------------------------|--------------------------------------------------------|
+| `name`        | The target name                                                                | Same as any other target, which is the directory name  |
+| `packages`    | Packaged targets to include. The first element will be used as the entrypoint. | `[]`                                                   |
+| `env`         | Environment variables to set. Does not support interpolation.                  | `[]`                                                   |
+| `outputs`     | Paths to capture into the built layer.                                         | `[]`                                                   |
+| `exclude`     | Globs to not include in the output.                                            | `[]`                                                   |
+| `decsription` | A description of the target                                                    |                                                        |
+| `output_path` | The output path during `pants package`                                         | A variant generated from the target name and directory |
+| `tags`        | List of tags                                                                   | `[]`                                                   |
```

### Comparing `pants-backend-oci-0.3.1/pants_backend_oci/goals/package.py` & `pants_backend_oci-0.4.0/pants_backend_oci/goals/package.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,86 +1,114 @@
-# Copyright 2022 Tom Solberg.
-# Licensed under the Apache License, Version 2.0 (see LICENSE).
+from __future__ import annotations
 
 from dataclasses import dataclass
 
-from pants.core.goals.package import BuiltPackage, BuiltPackageArtifact, PackageFieldSet
+from pants.core.goals.package import (
+    BuiltPackage,
+    BuiltPackageArtifact,
+    OutputPathField,
+    PackageFieldSet,
+)
 from pants.core.util_rules.external_tool import DownloadedExternalTool, ExternalToolRequest
 from pants.engine.fs import Digest, MergeDigests
 from pants.engine.internals.selectors import Get
 from pants.engine.platform import Platform
 from pants.engine.process import Process, ProcessResult
 from pants.engine.rules import collect_rules, rule
 from pants.engine.target import InvalidTargetException, WrappedTarget, WrappedTargetRequest
 from pants.engine.unions import UnionRule
 from pants.util.logging import LogLevel
 
 from pants_backend_oci.subsystem import SkopeoTool
-from pants_backend_oci.target_types import ImageDigest, ImageRepository, ImageTag
+from pants_backend_oci.target_types import ImageBuildOutputs, ImageDigest, ImageRepository, ImageTag
 from pants_backend_oci.util_rules.image_bundle import (
     FallibleImageBundle,
     FallibleImageBundleRequest,
     FallibleImageBundleRequestWrap,
     ImageBundleRequest,
 )
 
 
 @dataclass(frozen=True)
 class ImageFieldSet(PackageFieldSet):
     required_fields = (ImageRepository,)
 
     repository: ImageRepository
     tag: ImageTag
+
+    output_path: OutputPathField
+
     digest: ImageDigest
 
 
 @dataclass(frozen=True)
+class ArtifactFieldSet(PackageFieldSet):
+    required_fields = (ImageBuildOutputs,)
+
+    outputs: ImageBuildOutputs
+    output_path: OutputPathField
+
+
+@dataclass(frozen=True)
 class OciArchiveRequest:
     input_digest: Digest
     output_filename: str
     description: str
 
 
 @dataclass(frozen=True)
-class OciArchive:
+class BuiltOciArchive(BuiltPackage):
     """An OCI image in `oci-archive` format."""
 
-    digest: Digest
+    directory: str = ""
+    tag: str = ""
+    sha: str = ""
 
 
 @rule(desc="Convert OCI Image to Archive", level=LogLevel.DEBUG)
-async def package_oci_archive(
-    request: OciArchiveRequest, skopeo: SkopeoTool, platform: Platform
-) -> OciArchive:
+async def package_oci_archive(request: OciArchiveRequest, skopeo: SkopeoTool, platform: Platform) -> Process:
     skopeo = await Get(
         DownloadedExternalTool,
         ExternalToolRequest,
         skopeo.get_request(platform),
     )
 
     sandbox_input = await Get(Digest, MergeDigests([skopeo.digest, request.input_digest]))
-    result = await Get(
-        ProcessResult,
-        Process(
-            input_digest=sandbox_input,
-            argv=(
-                skopeo.exe,
-                # TODO[TSOL]: Should likely provide a way to inject a
-                # policy into this... Maybe dependency injector?
-                "--insecure-policy",
-                "copy",
-                "oci:build:build",
-                f"oci-archive:{request.output_filename}",
-            ),
-            description=f"Generate OCI Archive: {request.output_filename}",
-            output_files=(request.output_filename,),
+    return Process(
+        input_digest=sandbox_input,
+        argv=(
+            skopeo.exe,
+            # TODO[TSOL]: Should likely provide a way to inject a
+            # policy into this... Maybe dependency injector?
+            "--insecure-policy",
+            "copy",
+            "oci:build:build",
+            f"oci:{request.output_filename}",
         ),
+        description=f"Generate OCI Archive: {request.output_filename}",
+        output_directories=(request.output_filename,),
     )
 
-    return OciArchive(result.output_digest)
+
+@dataclass(frozen=True)
+class BuiltOciImage(BuiltPackageArtifact):
+    # We don't really want a default for this field, but the superclass has a field with
+    # a default, so all subsequent fields must have one too. The `create()` method below
+    # will ensure that this field is properly populated in practice.
+    sha: str = ""
+    tag: str = ""
+
+    @classmethod
+    def create(cls, sha: str, tag: str, directory: str) -> BuiltOciImage:
+        return cls(
+            sha=sha,
+            tag=tag,
+            relpath=directory,
+            extra_log_lines=(f"  {cls.__name__}: {directory}@{sha}",),
+        )
 
 
 @rule(desc="Package OCI Image", level=LogLevel.DEBUG)
 async def package_oci_image(field_set: ImageFieldSet) -> BuiltPackage:
     wrapped_target = await Get(
         WrappedTarget,
         WrappedTargetRequest(field_set.address, description_of_origin="package_oci_image"),
@@ -97,32 +125,38 @@
     if image.exit_code != 0 or image.dependency_failed:
         raise Exception(
             f"Failed packaging image:\n{image.stderr}",
         )
 
     image_digest = image.output.digest
 
-    name = (
-        field_set.repository.value.replace("/", "_").replace(":", "_")
-        if field_set.repository.value
-        else str(target.address.spec).replace("/", "_").replace(":", "_")
-    )
     suffix = field_set.tag.value if field_set.tag.value else field_set.digest.value
-    archive = await Get(
-        OciArchive,
+    archive_process = await Get(
+        Process,
         OciArchiveRequest(
             input_digest=image_digest,
-            output_filename=f"./{name}.{suffix}",
+            output_filename=field_set.output_path.value_or_default(file_ending="d"),
             description=f"Package OCI Image {field_set.address} -> {field_set.repository.value}:{suffix}",
         ),
     )
 
-    artifact = BuiltPackageArtifact(
-        relpath=f"{name}.{suffix}",
-        extra_log_lines=(f"Packaged image: {image.output.image_sha}",),
+    result = await Get(
+        ProcessResult,
+        Process,
+        archive_process,
     )
 
-    return BuiltPackage(archive.digest, (artifact,))
+    return BuiltPackage(
+        digest=result.output_digest,
+        artifacts=(
+            BuiltOciImage.create(
+                image.output.image_sha, "build", field_set.output_path.value_or_default(file_ending="d")
+            ),
+        ),
+    )
 
 
 def rules():
-    return [*collect_rules(), UnionRule(PackageFieldSet, ImageFieldSet)]
+    return [
+        *collect_rules(),
+        UnionRule(PackageFieldSet, ImageFieldSet),
+    ]
```

### Comparing `pants-backend-oci-0.3.1/pants_backend_oci/goals/publish.py` & `pants_backend_oci-0.4.0/pants_backend_oci/goals/publish.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,34 +7,29 @@
     PublishFieldSet,
     PublishOutputData,
     PublishPackages,
     PublishProcesses,
     PublishRequest,
 )
 from pants.core.util_rules.external_tool import DownloadedExternalTool, ExternalToolRequest
-from pants.engine.environment import Environment, EnvironmentRequest
+from pants.engine.env_vars import EnvironmentVars as Environment
+from pants.engine.env_vars import EnvironmentVarsRequest as EnvironmentRequest
 from pants.engine.fs import Digest, MergeDigests
 from pants.engine.internals.selectors import Get
 from pants.engine.platform import Platform
 from pants.engine.process import InteractiveProcess, Process
 from pants.engine.rules import collect_rules, rule
-from pants.engine.target import WrappedTarget, WrappedTargetRequest
 from pants.engine.unions import UnionRule
 from pants.util.logging import LogLevel
 
 from pants_backend_oci.subsystem import SkopeoTool
 from pants_backend_oci.target_types import ImageRepository, ImageTag
-from pants_backend_oci.util_rules.image_bundle import (
-    FallibleImageBundle,
-    FallibleImageBundleRequest,
-    FallibleImageBundleRequestWrap,
-    ImageBundleRequest,
-)
 
 
+@dataclass(frozen=True)
 class PublishImageRequest(PublishRequest):
     pass
 
 
 @dataclass(frozen=True)
 class PublishImageFieldSet(PublishFieldSet):
     publish_request_type = PublishImageRequest
@@ -58,73 +53,68 @@
 @dataclass(frozen=True)
 class OciPublishProcessRequest:
     input_digest: Digest
     repository: str
     tag: str
     description: str
 
+    directory: str
+
 
 @rule(desc="Convert OCI Image to Archive", level=LogLevel.DEBUG)
 async def publish_oci_process(
     request: OciPublishProcessRequest, skopeo: SkopeoTool, platform: Platform
 ) -> Process:
     skopeo = await Get(
         DownloadedExternalTool,
         ExternalToolRequest,
         skopeo.get_request(platform),
     )
     sandbox_input = await Get(Digest, MergeDigests([skopeo.digest, request.input_digest]))
-
     relevant_env = await Get(Environment, EnvironmentRequest(["HOME", "PATH", "XDG_RUNTIME_DIR"]))
     return Process(
         input_digest=sandbox_input,
         argv=(
             skopeo.exe,
             # TODO[TSOL]: Should likely provide a way to inject a
             # policy into this... Maybe dependency injector?
             "--insecure-policy",
             "copy",
-            "oci:build",
+            f"oci:{request.directory}",
             f"docker://{request.repository}:{request.tag}",
         ),
         description=f"{request.repository}:{request.tag}",
         output_files=tuple(),
         env=relevant_env,
     )
 
 
 @rule(desc="Publish OCI Image")
 async def publish_oci_image(request: PublishImageRequest) -> PublishProcesses:
-    wrapped_target = await Get(
-        WrappedTarget,
-        WrappedTargetRequest(request.field_set.address, description_of_origin="package_oci_image"),
-    )
-    target = wrapped_target.target
-    image_request = await Get(FallibleImageBundleRequestWrap, ImageBundleRequest(target))
-    image = await Get(FallibleImageBundle, FallibleImageBundleRequest, image_request.request)
-    image_digest = image.output.digest
-
     field_set = request.field_set
+    package = request.packages[0]
+    metadata = package.artifacts[0]
 
     process = await Get(
         Process,
         OciPublishProcessRequest(
-            input_digest=image_digest,
+            input_digest=package.digest,
             repository=field_set.repository.value,
             tag=field_set.tag.value,
             description=(
                 f"Publish OCI Image {field_set.address} -> {field_set.repository.value}:{field_set.tag.value}"
             ),
+            directory=metadata.relpath,
         ),
     )
 
     return PublishProcesses(
         (
             PublishPackages(
-                names=(f"{image.output.image_sha}",),
+                names=(f"{metadata.sha}",),
                 process=InteractiveProcess.from_process(process),
                 description=process.description,
                 data=PublishOutputData({"repository": process.description}),
             ),
         )
     )
```

### Comparing `pants-backend-oci-0.3.1/pants_backend_oci/language_target/python.py` & `pants_backend_oci-0.4.0/pants_backend_oci/language_target/python.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 
 """
 
+import datetime
+import os
 from dataclasses import dataclass
 
 from pants.core.util_rules.external_tool import DownloadedExternalTool, ExternalToolRequest
 from pants.engine.addresses import Addresses, UnparsedAddressInputs
 from pants.engine.fs import Digest, MergeDigests
 from pants.engine.platform import Platform
 from pants.engine.process import Process, ProcessResult
@@ -19,34 +21,39 @@
     Target,
     Targets,
     WrappedTarget,
     WrappedTargetRequest,
 )
 from pants.engine.unions import UnionRule
 from pants.util.strutil import softwrap
+from pants.version import PANTS_SEMVER, Version
 
 from pants_backend_oci.subsystem import UmociTool
 from pants_backend_oci.target_types import ImageBase, ImageRepository, ImageTag
+from pants_backend_oci.tools.process import FusedProcess
 from pants_backend_oci.util_rules.image_bundle import (
     FallibleImageBundle,
     FallibleImageBundleRequest,
     FallibleImageBundleRequestWrap,
     ImageBundle,
     ImageBundleRequest,
 )
 from pants_backend_oci.util_rules.layer import ImageLayer, ImageLayerRequest
 from pants_backend_oci.util_rules.oci_sha import OciSha, OciShaRequest
 
+if PANTS_SEMVER >= Version("2.17.0.dev0"):
+    from pants.core.util_rules.adhoc_binaries import GunzipBinary
+else:
+    from pants.core.util_rules.system_binaries import GunzipBinary
+
 
 class PythonMain(StringField):
     alias = "main"
-    help = softwrap(
-        """ The python main to use. If not provided, the rule will
-        attempt to derive it from the dependencies.  """
-    )
+    help = softwrap(""" The python main to use. If not provided, the rule will
+        attempt to derive it from the dependencies.  """)
 
 
 class PythonImageLayers(Dependencies):
     alias = "packages"
     help = softwrap("""The dependencies to add to the image""")
 
 
@@ -80,14 +87,15 @@
 
 
 @rule(desc="Build Python OCI image")
 async def build_python_image(
     request: BuildPythonImageRequest,
     umoci: UmociTool,
     platform: Platform,
+    gunzip: GunzipBinary,
 ) -> FallibleImageBundle:
     umoci_request = Get(DownloadedExternalTool, ExternalToolRequest, umoci.get_request(platform))
     base = await Get(
         Addresses,
         UnparsedAddressInputs,
         request.target.base.to_unparsed_address_inputs(),
     )
@@ -122,57 +130,70 @@
             if "--config.entrypoint" in layer.config_command:
                 idx = layer.config_command.index("--config.entrypoint")
                 ep = layer.config_command[idx + 1]
                 if ep.endswith(".pex"):
                     pex = ep
 
         input_digest = await Get(Digest, MergeDigests([umoci.digest, digest, layer.digest]))
-
-        image_with_layer = await Get(
-            ProcessResult,
+        layer_processes = (
             Process(
-                (umoci.exe, *layer.layer_command),
+                (umoci.exe, *layer.layer_command[:-1], layer.layer_command[-1].rstrip(".gz")),
                 input_digest=input_digest,
                 description=f"Package OCI Image Bundle: {layer.address}",
-                output_directories=("build/",),
             ),
-        )
-
-        digest = image_with_layer.output_digest
-        input_digest = await Get(Digest, MergeDigests([umoci.digest, digest]))
-        image_with_config = await Get(
-            ProcessResult,
             Process(
                 (umoci.exe, *layer.config_command),
-                input_digest=input_digest,
                 description=f"Configure OCI Image Bundle: {layer.address}",
                 output_directories=("build/",),
             ),
         )
-        digest = image_with_config.output_digest
+        if layer.compressed:
+            layer_processes = (
+                Process(
+                    argv=gunzip.extract_archive_argv(
+                        layer.layer_command[-1], os.path.dirname(layer.layer_command[-1])
+                    ),
+                    description=f"Uncompress OCI Image Bundle: {layer.address}",
+                ),
+                *layer_processes,
+            )
+        image = await Get(
+            ProcessResult,
+            FusedProcess(
+                layer_processes,
+            ),
+        )
+
+        digest = image.output_digest
 
     input_digest = await Get(Digest, MergeDigests([umoci.digest, digest]))
-    image_with_layer = await Get(
-        ProcessResult,
-        Process(
-            (
-                umoci.exe,
-                "config",
-                "--image",
-                "build:build",
-                "--config.entrypoint",
-                "python",
-                "--config.entrypoint",
-                pex,
+    timestamp = datetime.datetime(1970, 1, 1).isoformat() + "Z"
+
+    if pex is not None:
+        image_with_layer = await Get(
+            ProcessResult,
+            Process(
+                (
+                    umoci.exe,
+                    "config",
+                    "--image",
+                    "build:build",
+                    "--config.entrypoint",
+                    "python",
+                    "--config.entrypoint",
+                    pex,
+                    f"--history.created={timestamp}",
+                ),
+                input_digest=input_digest,
+                description=f"Package OCI Image Bundle: {layer.address}",
+                output_directories=("build/",),
             ),
-            input_digest=input_digest,
-            description=f"Package OCI Image Bundle: {layer.address}",
-            output_directories=("build/",),
-        ),
-    )
+        )
+    else:
+        image_with_layer = image
 
     image_digest = await Get(OciSha, OciShaRequest(image_with_layer.output_digest))
     output = ImageBundle(
         digest=image_with_layer.output_digest,
         image_sha=image_digest.image_digest,
         is_local=True,
     )
```

### Comparing `pants-backend-oci-0.3.1/pants_backend_oci/register.py` & `pants_backend_oci-0.4.0/pants_backend_oci/register.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 from pants.engine.rules import collect_rules
 
-from pants_backend_oci import goals, language_target, subsystem, targets, util_rules
+from pants_backend_oci import (
+    goals,
+    language_target,
+    subsystem,
+    synthetic_targets,
+    targets,
+    util_rules,
+)
 from pants_backend_oci.rules import kustomize_inject
 from pants_backend_oci.tools import process
 
 
 def target_types():
     return [
         *language_target.targets(),
@@ -18,8 +25,9 @@
         *goals.rules(),
         *kustomize_inject.rules(),
         *language_target.rules(),
         *process.rules(),
         *subsystem.rules(),
         *targets.rules(),
         *util_rules.rules(),
+        *synthetic_targets.rules(),
     ]
```

### Comparing `pants-backend-oci-0.3.1/pants_backend_oci/rules/kustomize_inject.py` & `pants_backend_oci-0.4.0/pants_backend_oci/rules/kustomize_inject.py`

 * *Files identical despite different names*

### Comparing `pants-backend-oci-0.3.1/pants_backend_oci/subsystem.py` & `pants_backend_oci-0.4.0/pants_backend_oci/subsystem.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,68 @@
 from __future__ import annotations
 
 from pants.core.util_rules.external_tool import ExternalTool
 from pants.engine.platform import Platform
-from pants.engine.rules import SubsystemRule
+from pants.option.option_types import BoolOption, StrListOption, StrOption
+from pants.option.subsystem import Subsystem
+
+
+class OciSubsystem(Subsystem):
+    options_scope = "oci"
+    help = "Generic options for the OCI subsystem."
+
+    command_shell = StrListOption(
+        default=["/bin/sh", "-c"],
+        advanced=True,
+        help="The default shell to use for container build commands.",
+    )
+
+    rootless = BoolOption(
+        default=True,
+        advanced=True,
+        help=(
+            "Whether to run in rootless mode, which changes behavior for some commands. Recommended on but"
+            " may require more setup.."
+        ),
+    )
+
+    uid_map = StrListOption(
+        default=["0:1000:1", "1:100000:65536"],
+        advanced=True,
+        help="The UID map to use.",
+    )
+
+    gid_map = StrListOption(
+        default=["0:1000:1", "1:100000:65536"],
+        advanced=True,
+        help="The GID map to use.",
+    )
+
+    empty_image_target = StrOption(
+        default="empty",
+        advanced=False,
+        help="The name of the synthetic target for an empty base image.",
+    )
 
 
 class UmociTool(ExternalTool):
     options_scope = "umoci"
-    help = "Wrapper for kustomize."
+    help = "Umoci is used for manipulating OCI images."
 
     default_version = "v0.4.7"
     default_known_versions = [
         "v0.4.7|linux_x86_64|6abecdbe7ac96a8e48fdb73fb53f08d21d4dc5e040f7590d2ca5547b7f2b2e85|7499776",
     ]
 
+    log = StrOption(
+        default="warn",
+        advanced=False,
+        help="The log level for umoci.",
+    )
+
     def generate_url(self, plat: Platform) -> str:
         platform_mapping = {
             "linux_x86_64": "amd64",
         }
         plat_str = platform_mapping[plat.value]
         return f"https://github.com/opencontainers/umoci/releases/download/{self.version}/umoci.{plat_str}"
 
@@ -27,15 +72,15 @@
         }
         plat_str = platform_mapping[plat.value]
         return f"./umoci.{plat_str}"
 
 
 class SkopeoTool(ExternalTool):
     options_scope = "skopeo"
-    help = "Wrapper for kustomize."
+    help = "Tool for moving containers."
 
     default_version = "v1.9.3"
     default_known_versions = [
         "v1.9.2|linux_arm64 |1b7b4411c9723dbbdda4ae9dde23a33d8ab093b54c97d3323784b117d3e9413f|32542312",
         "v1.9.2|linux_x86_64|5c82f8fc2bcb2502cf7cdf9239f54468d52f5a2a8072893c75408b78173c4ba6|30920360",
         "v1.9.3|linux_arm64 |27c88183de036ebd4ffa5bc5211329666e3c40ac69c5d938bcdab9b9ec248fd4|30189956",
         "v1.9.3|linux_x86_64|6e00cf4661c081fb1d010ce60904dccb880788a52bf10de16a40f32082415a87|29390800",
@@ -83,11 +128,12 @@
         }
         plat_str = platform_mapping[plat.value]
         return f"./runc.{plat_str}"
 
 
 def rules():
     return [
-        SubsystemRule(SkopeoTool),
-        SubsystemRule(RuncTool),
-        SubsystemRule(UmociTool),
+        *SkopeoTool.rules(),
+        *RuncTool.rules(),
+        *UmociTool.rules(),
+        *OciSubsystem.rules(),
     ]
```

### Comparing `pants-backend-oci-0.3.1/pants_backend_oci/targets.py` & `pants_backend_oci-0.4.0/pants_backend_oci/targets.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,44 @@
+from pants.core.goals.package import OutputPathField
 from pants.engine.rules import collect_rules, rule
 from pants.engine.target import (
     COMMON_TARGET_FIELDS,
     DictStringToStringField,
     GeneratedTargets,
     GenerateTargetsRequest,
     Target,
     TargetGenerator,
 )
 from pants.engine.unions import UnionMembership, UnionRule
 from pants.util.strutil import softwrap
 
 from pants_backend_oci.target_types import (
+    ImageArgs,
+    ImageArtifactExclusions,
     ImageBase,
+    ImageBuildCommand,
+    ImageBuildOutputs,
     ImageDependencies,
     ImageDigest,
+    ImageEmptyMarker,
+    ImageEntrypoint,
+    ImageEnvironment,
     ImageRepository,
     ImageRepositoryAnonymous,
     ImageRunTty,
     ImageTag,
 )
 
 
 # Only used here
 class _ImageVariants(DictStringToStringField):
     alias = "variants"
-    help = softwrap(
-        """
+    help = softwrap("""
         The digests to use and names to export as.
-        """
-    )
+        """)
 
 
 class PullImage(Target):
     alias = "oci_pull_image"
     core_fields = (
         *COMMON_TARGET_FIELDS,
         ImageRepository,
@@ -40,19 +46,17 @@
         ImageDigest,
     )
     help = "An imported OCI image."
 
 
 class PullImagesGenerator(TargetGenerator):
     alias = "oci_pull_images"
-    help = softwrap(
-        """
+    help = softwrap("""
         The list of base images to import.
-        """
-    )
+        """)
     generated_target_cls = PullImage
     core_fields = (
         *COMMON_TARGET_FIELDS,
         ImageRepository,
         ImageRepositoryAnonymous,
         _ImageVariants,
     )
@@ -93,20 +97,49 @@
     core_fields = (
         *COMMON_TARGET_FIELDS,
         ImageRepository,
         ImageTag,
         ImageBase,
         ImageDependencies,
         ImageRunTty,
+        ImageEnvironment,
+        ImageEntrypoint,
+        ImageArgs,
+        OutputPathField,
+        ImageBuildCommand,
+    )
+    help = "An imported OCI image."
+
+
+class ImageEmpty(Target):
+    alias = "oci_image_empty"
+    core_fields = (
+        *COMMON_TARGET_FIELDS,
+        ImageEmptyMarker,
+    )
+    help = "An imported OCI image."
+
+
+class ImageBuildStep(Target):
+    alias = "oci_build_layer"
+    core_fields = (
+        *COMMON_TARGET_FIELDS,
+        ImageBase,
+        ImageDependencies,
+        ImageBuildOutputs,
+        ImageBuildCommand,
+        ImageEnvironment,
+        ImageArtifactExclusions,
+        OutputPathField,
     )
     help = "An imported OCI image."
 
 
 def targets():
-    return [PullImage, PullImagesGenerator, ImageBuild]
+    return [PullImage, PullImagesGenerator, ImageBuild, ImageBuildStep, ImageEmpty]
 
 
 def rules():
     return [
         *collect_rules(),
         UnionRule(GenerateTargetsRequest, GenerateFromPullImagesRequest),
     ]
```

### Comparing `pants-backend-oci-0.3.1/pants_backend_oci/tools/process.py` & `pants_backend_oci-0.4.0/pants_backend_oci/tools/process.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Various tools for creating processes.
 """
 
 from __future__ import annotations
 
+import shlex
 from dataclasses import dataclass
 
 from pants.core.util_rules.system_binaries import BashBinary
 from pants.engine.fs import Digest, MergeDigests
 from pants.engine.process import Process
 from pants.engine.rules import Get, collect_rules, rule
 
@@ -16,35 +17,43 @@
 class FusedProcess:
     processes: tuple(Process)
 
 
 @rule
 async def fuse_process(request: FusedProcess, bash: BashBinary) -> Process:
     common_output_directories = list(set(sum([list(p.output_directories) for p in request.processes], [])))
+    immutable_input_digests = {}
+    for p in request.processes:
+        immutable_input_digests.update(p.immutable_input_digests)
 
     common_output_files = list(set(sum([list(p.output_files) for p in request.processes], [])))
-
     common_digest_input = list(set([p.input_digest for p in request.processes if p.input_digest]))
-
     common_description = " | ".join(p.description for p in request.processes)
 
     common_digest = await Get(Digest, MergeDigests(common_digest_input))
 
+    env = {}
+    for p in request.processes:
+        env.update(p.env)
+
     script = """
+    set -euxo pipefail
     export ROOT_DIR="$(pwd)"
     export SANDBOX_DIR="{chroot}"
     cd $SANDBOX_DIR
     """ + "\n".join(
-        " ".join(p.argv) for p in request.processes
+        " ".join(v if "# nosplit" in v else shlex.quote(v) for v in p.argv) for p in request.processes
     )
 
     return Process(
-        (bash.path, "-c", script, "$@"),
+        argv=(bash.path, "-c", script, "$@"),
         description=f"Fused run of: {common_description}",
         input_digest=common_digest,
         output_files=common_output_files,
         output_directories=common_output_directories,
+        immutable_input_digests=immutable_input_digests,
+        env=env,
     )
 
 
 def rules():
     return collect_rules()
```

### Comparing `pants-backend-oci-0.3.1/pants_backend_oci/util_rules/build_image_bundle.py` & `pants_backend_oci-0.4.0/pants_backend_oci/util_rules/build_image_artifact.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,89 @@
+"""
+
+"""
 from __future__ import annotations
 
 import dataclasses
 from dataclasses import dataclass
+from typing import ClassVar
 
+from pants.core.goals.package import OutputPathField, PackageFieldSet
 from pants.core.util_rules.external_tool import DownloadedExternalTool, ExternalToolRequest
+from pants.core.util_rules.system_binaries import BashBinary, CatBinary, CpBinary, MkdirBinary
 from pants.engine.addresses import Addresses, UnparsedAddressInputs
 from pants.engine.fs import Digest, MergeDigests
 from pants.engine.platform import Platform
 from pants.engine.process import Process, ProcessResult
 from pants.engine.rules import Get, MultiGet, collect_rules, rule
 from pants.engine.target import (
-    Dependencies,
     DependenciesRequest,
     FieldSet,
     Target,
     Targets,
     WrappedTarget,
     WrappedTargetRequest,
 )
-from pants.engine.unions import UnionRule
 from pants.util.logging import LogLevel
 
-from pants_backend_oci.subsystem import UmociTool
-from pants_backend_oci.target_types import ImageBase, ImageDependencies
-from pants_backend_oci.tools.process import FusedProcess
+from pants_backend_oci.subsystem import RuncTool, UmociTool
+from pants_backend_oci.target_types import (
+    ImageArtifactExclusions,
+    ImageBase,
+    ImageBuildCommand,
+    ImageBuildOutputs,
+    ImageDependencies,
+    ImageEnvironment,
+)
+from pants_backend_oci.util_rules.copy import CopyFromRequest
 from pants_backend_oci.util_rules.image_bundle import (
     FallibleImageBundle,
     FallibleImageBundleRequest,
     FallibleImageBundleRequestWrap,
     ImageBundle,
     ImageBundleRequest,
 )
 from pants_backend_oci.util_rules.layer import ImageLayer, ImageLayerRequest
-from pants_backend_oci.util_rules.oci_sha import OciSha, OciShaRequest
+from pants_backend_oci.util_rules.run import RunContainerRequest
 
 
 @dataclass(frozen=True)
-class BuildImageBundleFieldSet(FieldSet):
-    required_fields = (ImageBase, ImageDependencies)
+class ImageArtifactBuildFieldSet(PackageFieldSet):
+    required_fields = (ImageBase, ImageBuildCommand, ImageBuildOutputs)
 
     base: ImageBase
-    dependencies: Dependencies
 
+    commands: ImageBuildCommand
+    outputs: ImageBuildOutputs
 
-@dataclass(frozen=True)
-class BuildImageBundleRequest(FallibleImageBundleRequest):
+    dependencies: ImageDependencies
+    environment: ImageEnvironment
+
+    output_path: OutputPathField
+
+    exclude: ImageArtifactExclusions
+
+
+class ImageArtifactBuildRequest(FallibleImageBundleRequest):
     target: Target
 
-    field_set_type = BuildImageBundleFieldSet
+    field_set_type: ClassVar[type[FieldSet]] = ImageArtifactBuildFieldSet
 
 
-@rule(desc="Build OCI image", level=LogLevel.DEBUG)
-async def build_oci_bundle_package(
-    request: BuildImageBundleRequest,
+@rule(desc="Build artifact in container", level=LogLevel.DEBUG)
+async def build_image_artifact(
+    request: ImageArtifactBuildRequest,
     umoci: UmociTool,
+    runc: RuncTool,
     platform: Platform,
-) -> FallibleImageBundle:
+    bash: BashBinary,
+    cat: CatBinary,
+    cp: CpBinary,
+    mkdir: MkdirBinary,
+) -> ProcessResult:
     base = await Get(
         Addresses,
         UnparsedAddressInputs,
         request.target.base.to_unparsed_address_inputs(),
     )
 
     wrapped_target = await Get(
@@ -69,61 +93,106 @@
 
     build_request = await Get(FallibleImageBundleRequestWrap, ImageBundleRequest(wrapped_target.target))
     maybe_built_base = await Get(FallibleImageBundle, FallibleImageBundleRequest, build_request.request)
 
     if maybe_built_base.output is None:
         return dataclasses.replace(maybe_built_base, dependency_failed=True)
 
-    umoci = await Get(DownloadedExternalTool, ExternalToolRequest, umoci.get_request(platform))
+    umoci_request = Get(DownloadedExternalTool, ExternalToolRequest, umoci.get_request(platform))
     base = maybe_built_base.output
     base_digest = base.digest
 
     if request.target.dependencies:
-        root_dependencies = await Get(Targets, DependenciesRequest(request.target.dependencies))
+        dependencies = await MultiGet(
+            Get(Targets, DependenciesRequest(request.target.dependencies)),
+        )
 
         layers = []
-        for dependency in root_dependencies:
-            layers.append(Get(ImageLayer, ImageLayerRequest(dependency)))
+        for dependency in dependencies:
+            layers.append(Get(ImageLayer, ImageLayerRequest(dependency[0])))
 
-        layers = await MultiGet(*layers)
+        umoci, *layers = await MultiGet(
+            umoci_request,
+            *layers,
+        )
 
         for layer in layers:
             input_digest = await Get(Digest, MergeDigests([umoci.digest, base_digest, layer.digest]))
 
             image_with_layer = await Get(
                 ProcessResult,
-                FusedProcess(
-                    (
-                        Process(
-                            (umoci.exe, *layer.layer_command),
-                            input_digest=input_digest,
-                            description=f"Package OCI Image Bundle: {layer.address}",
-                            output_directories=("build/",),
-                        ),
-                        Process(
-                            (umoci.exe, *layer.config_command),
-                            input_digest=input_digest,
-                            description=f"Configure OCI Image Bundle: {layer.address}",
-                            output_directories=("build/",),
-                        ),
-                    )
+                Process(
+                    (umoci.exe, *layer.layer_command),
+                    input_digest=input_digest,
+                    description=f"Package OCI Layer Artifact: {layer.address}",
+                    output_directories=("build/",),
                 ),
             )
-            base_digest = image_with_layer.output_digest
+
+            digest = image_with_layer.output_digest
+            input_digest = await Get(Digest, MergeDigests([umoci.digest, digest]))
+            image_with_config = await Get(
+                ProcessResult,
+                Process(
+                    (umoci.exe, *layer.config_command),
+                    input_digest=input_digest,
+                    description=f"Configure OCI Layer Artifact: {layer.address}",
+                    output_directories=("build/",),
+                ),
+            )
+            base_digest = image_with_config.output_digest
+
+        config = []
+        for value in request.target.environment.value:
+            config.extend(
+                [
+                    "--config.env",
+                    value,
+                ]
+            )
 
         output_digest = base_digest
+        image_with_config = await Get(
+            ProcessResult,
+            Process(
+                (
+                    umoci.exe,
+                    "config",
+                    *config,
+                    "--image",
+                    "build:build",
+                ),
+                input_digest=input_digest,
+                description=f"Configure OCI Image Bundle: {layer.address}",
+                output_directories=("build/",),
+            ),
+        )
 
+        output_digest = image_with_config.output_digest
     else:
         output_digest = base_digest
 
-    image_digest = await Get(OciSha, OciShaRequest(output_digest))
+    bundle = ImageBundle(output_digest, "", True)
+
+    modified_image = await Get(
+        ProcessResult, RunContainerRequest(bundle, request.target.commands.value, True)
+    )
+    bundle = ImageBundle(modified_image.output_digest, "", True)
 
-    output = ImageBundle(digest=output_digest, image_sha=image_digest.image_digest, is_local=True)
+    artifacts = await Get(
+        ProcessResult,
+        CopyFromRequest(
+            request.target.output_path.value_or_default(file_ending="tar.gz"),
+            bundle,
+            tuple(),
+            request.target.outputs.value,
+            exclude_patterns=tuple(request.target.exclude.value or ()),
+        ),
+    )
 
-    return FallibleImageBundle(output)
+    return artifacts
 
 
 def rules():
     return [
         *collect_rules(),
-        UnionRule(FallibleImageBundleRequest, BuildImageBundleRequest),
     ]
```

### Comparing `pants-backend-oci-0.3.1/pants_backend_oci/util_rules/image_bundle.py` & `pants_backend_oci-0.4.0/pants_backend_oci/util_rules/image_bundle.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,33 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import ClassVar
 
 from pants.engine.engine_aware import EngineAwareReturnType
+from pants.engine.environment import EnvironmentName
 from pants.engine.fs import Digest
 from pants.engine.rules import collect_rules, rule
 from pants.engine.target import FieldSet, Target
 from pants.engine.unions import UnionMembership, union
 from pants.util.logging import LogLevel
 from pants.util.strutil import bullet_list
-from pants.version import PANTS_SEMVER, Version
 
 
 @dataclass(frozen=True)
 class ImageBundleRequest:
     target: Target
 
 
-if PANTS_SEMVER >= Version("2.15.0.dev0"):
-    from pants.engine.environment import EnvironmentName
-
-    @union(in_scope_types=[EnvironmentName])
-    @dataclass(frozen=True)
-    class FallibleImageBundleRequest:
-        target: Target
-
-        field_set_type: ClassVar[type[FieldSet]]
-
-else:
-
-    @union
-    @dataclass(frozen=True)
-    class FallibleImageBundleRequest:
-        target: Target
+@union(in_scope_types=[EnvironmentName])
+@dataclass(frozen=True)
+class FallibleImageBundleRequest:
+    target: Target
 
-        field_set_type: ClassVar[type[FieldSet]]
+    field_set_type: ClassVar[type[FieldSet]]
 
 
 @dataclass(frozen=True)
 class FallibleImageBundleRequestWrap:
     """A built OCI image layer."""
 
     request: FallibleImageBundleRequest
```

### Comparing `pants-backend-oci-0.3.1/pants_backend_oci/util_rules/layer.py` & `pants_backend_oci-0.4.0/pants_backend_oci/util_rules/layer.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,24 +4,29 @@
 
 from __future__ import annotations
 
 import datetime
 import logging
 from dataclasses import dataclass
 
-from pants.core.goals.package import BuiltPackage, PackageFieldSet
+from pants.core.goals.package import BuiltPackage, BuiltPackageArtifact, PackageFieldSet
 from pants.core.target_types import FileSourceField
 from pants.core.util_rules.source_files import SourceFiles, SourceFilesRequest
 from pants.engine.addresses import Address
 from pants.engine.fs import Digest, MergeDigests, Snapshot
 from pants.engine.rules import Get, MultiGet, collect_rules, rule
 from pants.engine.target import FieldSetsPerTarget, FieldSetsPerTargetRequest, SourcesField, Target
 
 from pants_backend_oci.util_rules.archive import CreateDeterministicTar
 
+
+class BuiltLayerArtifact(BuiltPackageArtifact):
+    pass
+
+
 logger = logging
 
 
 @dataclass(frozen=True)
 class ImageLayerRequest:
     target: Target
 
@@ -30,14 +35,16 @@
 class ImageLayer:
     address: Address
     digest: Digest
 
     layer_command: tuple[str]
     config_command: tuple[str]
 
+    compressed: bool = True
+
 
 @rule
 async def build_image_layer(request: ImageLayerRequest) -> ImageLayer:
     # Get all dependencies for the root target.
     root_dependencies = [request.target]
 
     # Get all file sources from the root dependencies. That includes any non-file sources that can
@@ -73,25 +80,73 @@
     )
 
     packages_str = ", ".join(a.relpath for p in embedded_pkgs for a in p.artifacts if a.relpath)
     if packages_str:
         logger.info(f"Built {len(embedded_pkgs)} packages for OCI image: {packages_str}")
     else:
         logger.info("Did not build any packages for OCI image")
+    other_artifacts = []
+    layer_artifacts = []
 
-    embedded_pkgs_digest = [built_package.digest for built_package in embedded_pkgs]
-    all_digests = (sources.snapshot.digest, *embedded_pkgs_digest)
+    is_compressed = False
+    for target in embedded_pkgs:
+        if len(target.artifacts) > 1 or not isinstance(target.artifacts[0], BuiltLayerArtifact):
+            other_artifacts.append(target)
+
+        else:
+            layer_artifacts.append(target)
+            if target.artifacts[0].relpath.endswith(".tar.gz"):
+                is_compressed = True
 
-    snapshot = await Get(
-        Snapshot,
-        MergeDigests(all_digests),
-    )
+    embedded_pkgs_digest = [built_package.digest for built_package in other_artifacts]
+
+    if sources.snapshot.files or sources.snapshot.dirs:
+        all_digests = (sources.snapshot.digest, *embedded_pkgs_digest)
+    else:
+        all_digests = embedded_pkgs_digest
+
+    real_layers = []
+
+    if all_digests:
+        snapshot = await Get(
+            Snapshot,
+            MergeDigests(all_digests),
+        )
+
+        raw_layer_digest = await Get(Digest, CreateDeterministicTar(snapshot, "layers/image_bundle.tar"))
+        layer_name = "layers/image_bundle.tar"
+        real_layers.append(
+            (
+                raw_layer_digest,
+                layer_name,
+            )
+        )
+
+    for layer in layer_artifacts:
+        snapshot = await Get(
+            Snapshot,
+            MergeDigests([layer.digest]),
+        )
+
+        real_layers.append(
+            (
+                snapshot.digest,
+                snapshot.files[0],
+            )
+        )
 
-    raw_layer_digest = await Get(Digest, CreateDeterministicTar(snapshot, "layers/image_bundle.tar"))
+    if len(real_layers) > 1:
+        # TODO[TSolberg]: Support multiple layers. We need to merge the layers together to create a single
+        # layer that can be added to the image.
+        #
+        # Things to note:
+        # Layer order matters. Determinism. `tar --concatenate` is ridiculusly slow.
+        raise Exception(f"Multiple layers not yet supported: {real_layers}")
 
+    raw_layer_digest, layer_name = real_layers[0]
     timestamp = datetime.datetime(1970, 1, 1).isoformat() + "Z"
     config = [
         "--config.env",
         "BUILT_BY=pants.oci",
         "--author=pants_backend_oci",
         f"--created={timestamp}",
         "--no-history",
@@ -114,20 +169,21 @@
             "add-layer",
             "--history.author=pants_backend_oci",
             f"--history.created_by='Layer target: {request.target.address}'",
             f"--history.comment='Layer target: {request.target.address}'",
             f"--history.created={timestamp}",
             "--image",
             "build:build",
-            "layers/image_bundle.tar",
+            layer_name,
         ),
         (
             "config",
             *config,
             "--image",
             "build:build",
         ),
+        compressed=is_compressed,
     )
 
 
 def rules():
     return collect_rules()
```

### Comparing `pants-backend-oci-0.3.1/pants_backend_oci/util_rules/oci_sha.py` & `pants_backend_oci-0.4.0/pants_backend_oci/util_rules/oci_sha.py`

 * *Files identical despite different names*

### Comparing `pants-backend-oci-0.3.1/pants_backend_oci/util_rules/pull_image_bundle.py` & `pants_backend_oci-0.4.0/pants_backend_oci/util_rules/pull_image_bundle.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import ClassVar
 
-from pants.core.goals.package import PackageFieldSet
 from pants.core.util_rules.external_tool import DownloadedExternalTool, ExternalToolRequest
 from pants.engine.platform import Platform
-from pants.engine.process import Process, ProcessResult
+from pants.engine.process import FallibleProcessResult, Process
 from pants.engine.rules import Get, collect_rules, rule
 from pants.engine.target import FieldSet, Target
 from pants.engine.unions import UnionRule
-from pants.util.logging import LogLevel
 
 from pants_backend_oci.subsystem import SkopeoTool
 from pants_backend_oci.target_types import ImageDigest, ImageRepository, ImageRepositoryAnonymous
 from pants_backend_oci.util_rules.image_bundle import (
     FallibleImageBundle,
     FallibleImageBundleRequest,
     ImageBundle,
@@ -26,29 +24,22 @@
     required_fields = (ImageDigest, ImageRepository)
 
     repository: ImageRepository
     digest: ImageDigest
     anonymous: ImageRepositoryAnonymous
 
 
+@dataclass(frozen=True)
 class ImageBundlePullRequest(FallibleImageBundleRequest):
     target: Target
 
     field_set_type: ClassVar[type[FieldSet]] = ImageBundlePullFieldSet
 
 
-@dataclass(frozen=True)
-class PullImageFieldset(PackageFieldSet):
-    required_fields = (ImageRepository, ImageDigest)
-
-    repository: ImageRepository
-    digest: ImageDigest
-
-
-@rule(level=LogLevel.DEBUG)
+@rule
 async def pull_oci_image(
     request: ImageBundlePullRequest, skopeo_tool: SkopeoTool, platform: Platform
 ) -> FallibleImageBundle:
     skopeo = await Get(
         DownloadedExternalTool,
         ExternalToolRequest,
         skopeo_tool.get_request(platform),
@@ -70,24 +61,32 @@
             f"docker://{request.target.repository.value}@sha256:{request.target.digest.value}",
             "oci:build:build",
         ]
     )
 
     desc = f"Download OCI image {request.target.repository.value}@sha256:{request.target.digest.value}"
 
+    p = Process(
+        argv=tuple(args),
+        input_digest=skopeo.digest,
+        description=desc,
+        output_directories=("build",),
+    )
+
     result = await Get(
-        ProcessResult,
-        Process(
-            argv=tuple(args),
-            input_digest=skopeo.digest,
-            description=desc,
-            output_directories=("build",),
-        ),
+        FallibleProcessResult,
+        Process,
+        p,
     )
 
+    if result.exit_code != 0:
+        return FallibleImageBundle(
+            exit_code=result.exit_code, stderr=result.stderr.decode(), stdout=result.stdout.decode()
+        )
+
     return FallibleImageBundle(
         ImageBundle(result.output_digest, f"sha256:{request.target.digest.value}", is_local=False)
     )
 
 
 def rules():
     return [
```

### Comparing `pants-backend-oci-0.3.1/pyproject.toml` & `pants_backend_oci-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "pants_backend_oci"
 description = "An OCI plugin for the Pants build system"
-version = "0.3.1"
+version = "0.4.0"
 authors = [
     { name = "Tom Solberg", email = "me@sbg.dev" },
 ]
 dependencies = [
-    "pants-backend-kustomize>=0.1",
+    "pants-backend-kustomize>=0.2",
 ]
 readme = "README.md"
 keywords = [
     "pantsbuild",
     "pants",
     "docker",
     "oci",
@@ -30,24 +30,28 @@
 Code = "https://github.com/tgolsson/pants-backends/tree/main/pants-plugins/oci"
 Changelog = "https://github.com/tgolsson/pants-backends/tree/main/pants-plugins/oci/CHANGELOG.md"
 
 [tool.pdm.build]
 includes = [
     "pants_backend_oci",
 ]
+excludes = [
+    "**/BUILD",
+]
 
 [tool.isort]
 profile = "black"
 known_first_party = [
     "pants_backend_oci",
 ]
 line_length = 100
 include_trailing_comma = true
 
 [tool.black]
-line-length = 100
+line-length = 110
+preview = true
 
 [build-system]
 requires = [
-    "pdm-pep517>=1.0.0",
+    "pdm-backend>=1.0.0",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
```

