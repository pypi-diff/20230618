# Comparing `tmp/pants-backend-secrets-0.1.0.tar.gz` & `tmp/pants-backend-secrets-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pants-backend-secrets-0.1.0.tar", last modified: Fri Feb 10 15:51:28 2023, max compression
+gzip compressed data, was "pants-backend-secrets-0.2.0.tar", last modified: Sun Jun 18 19:28:28 2023, max compression
```

## Comparing `pants-backend-secrets-0.1.0.tar` & `pants-backend-secrets-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1068 2023-02-10 15:51:28.459373 pants-backend-secrets-0.1.0/LICENSE-MIT.txt
--rw-r--r--   0        0        0     1477 2023-02-10 15:51:28.459373 pants-backend-secrets-0.1.0/README.md
--rw-r--r--   0        0        0        9 2023-02-10 15:51:28.459373 pants-backend-secrets-0.1.0/pants_backend_secrets/__init__.py
--rw-r--r--   0        0        0     2568 2023-02-10 15:51:28.459373 pants-backend-secrets-0.1.0/pants_backend_secrets/env_secret_provider.py
--rw-r--r--   0        0        0      194 2023-02-10 15:51:28.459373 pants-backend-secrets-0.1.0/pants_backend_secrets/exception.py
--rw-r--r--   0        0        0     4836 2023-02-10 15:51:28.459373 pants-backend-secrets-0.1.0/pants_backend_secrets/goals/decrypt.py
--rw-r--r--   0        0        0     7586 2023-02-10 15:51:28.459373 pants-backend-secrets-0.1.0/pants_backend_secrets/publish_secret_python.py
--rw-r--r--   0        0        0      494 2023-02-10 15:51:28.459373 pants-backend-secrets-0.1.0/pants_backend_secrets/register.py
--rw-r--r--   0        0        0      421 2023-02-10 15:51:28.459373 pants-backend-secrets-0.1.0/pants_backend_secrets/secret.py
--rw-r--r--   0        0        0     3662 2023-02-10 15:51:28.459373 pants-backend-secrets-0.1.0/pants_backend_secrets/secret_request.py
--rw-r--r--   0        0        0      500 2023-02-10 15:51:28.459373 pants-backend-secrets-0.1.0/pants_backend_secrets/targets.py
--rw-r--r--   0        0        0     1075 2023-02-10 15:51:28.459373 pants-backend-secrets-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2145 1970-01-01 00:00:00.000000 pants-backend-secrets-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-18 19:28:28.837520 pants-backend-secrets-0.2.0/LICENSE-MIT.txt
+-rw-r--r--   0        0        0     1477 2023-06-18 19:28:28.837520 pants-backend-secrets-0.2.0/README.md
+-rw-r--r--   0        0        0        9 2023-06-18 19:28:28.837520 pants-backend-secrets-0.2.0/pants_backend_secrets/__init__.py
+-rw-r--r--   0        0        0     2675 2023-06-18 19:28:28.837520 pants-backend-secrets-0.2.0/pants_backend_secrets/env_secret_provider.py
+-rw-r--r--   0        0        0      194 2023-06-18 19:28:28.837520 pants-backend-secrets-0.2.0/pants_backend_secrets/exception.py
+-rw-r--r--   0        0        0     4728 2023-06-18 19:28:28.837520 pants-backend-secrets-0.2.0/pants_backend_secrets/goals/decrypt.py
+-rw-r--r--   0        0        0     7795 2023-06-18 19:28:28.837520 pants-backend-secrets-0.2.0/pants_backend_secrets/publish_secret_python.py
+-rw-r--r--   0        0        0      494 2023-06-18 19:28:28.837520 pants-backend-secrets-0.2.0/pants_backend_secrets/register.py
+-rw-r--r--   0        0        0      421 2023-06-18 19:28:28.837520 pants-backend-secrets-0.2.0/pants_backend_secrets/secret.py
+-rw-r--r--   0        0        0     3398 2023-06-18 19:28:28.837520 pants-backend-secrets-0.2.0/pants_backend_secrets/secret_request.py
+-rw-r--r--   0        0        0      500 2023-06-18 19:28:28.837520 pants-backend-secrets-0.2.0/pants_backend_secrets/targets.py
+-rw-r--r--   0        0        0     1075 2023-06-18 19:28:28.837520 pants-backend-secrets-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2145 1970-01-01 00:00:00.000000 pants-backend-secrets-0.2.0/PKG-INFO
```

### Comparing `pants-backend-secrets-0.1.0/LICENSE-MIT.txt` & `pants-backend-secrets-0.2.0/LICENSE-MIT.txt`

 * *Files identical despite different names*

### Comparing `pants-backend-secrets-0.1.0/README.md` & `pants-backend-secrets-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pants-backend-secrets-0.1.0/pants_backend_secrets/env_secret_provider.py` & `pants-backend-secrets-0.2.0/pants_backend_secrets/env_secret_provider.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from dataclasses import dataclass
 
-from pants.engine.environment import Environment, EnvironmentRequest
+from pants.engine.env_vars import EnvironmentVars as EnvironmentVars
+from pants.engine.env_vars import EnvironmentVarsRequest as EnvironmentVarsRequest
 from pants.engine.rules import Get, collect_rules, rule
 from pants.engine.target import FieldSet
 from pants.engine.unions import UnionRule
 
 from pants_backend_secrets.exception import MissingSecret
 from pants_backend_secrets.goals.decrypt import DecryptFieldSet, DecryptRequest, DecryptResponse
 from pants_backend_secrets.secret_request import (
@@ -33,49 +34,49 @@
     field_set_type = EnvironmentSecretFieldSet
 
 
 @rule
 async def get_environment_key(
     request: FallibleEnvironmentSecretsRequest,
 ) -> FallibleSecretsResponse:
-    relevant_env = await Get(Environment, EnvironmentRequest([request.target.key.value]))
+    relevant_env = await Get(EnvironmentVars, EnvironmentVarsRequest([request.target.key.value]))
 
     if request.target.key.value not in relevant_env:
         return FallibleSecretsResponse(
             exit_code=1,
             stdout=f"secret is not in host environment: `{request.target.key.value}`",
         )
 
     # no stdout or stderr on exit 0, to avoid leaks
     return FallibleSecretsResponse(
         exit_code=0,
         response=SecretsResponse(
-            SecretValue(relevant_env[request.target.key.value], request.target.address, "Environment"),
+            SecretValue(relevant_env[request.target.key.value], request.target.address, "EnvironmentVars"),
         ),
     )
 
 
-class DecryptEnvironmentRequest(DecryptRequest):
+class DecryptEnvironmentVarsRequest(DecryptRequest):
     pass
 
 
 @dataclass(frozen=True)
 class DecryptEnvironmentFieldSet(DecryptFieldSet):
-    decrypt_request_type = DecryptEnvironmentRequest
+    decrypt_request_type = DecryptEnvironmentVarsRequest
     required_fields = (EnvironmentSecretKey,)
 
     key: EnvironmentSecretKey
 
 
 @rule
-async def decrypt_environment(request: DecryptEnvironmentRequest) -> DecryptResponse:
+async def decrypt_environment(request: DecryptEnvironmentVarsRequest) -> DecryptResponse:
     response = await Get(FallibleSecretsResponse, FallibleEnvironmentSecretsRequest(request.field_set))
 
     if response.exit_code != 0:
-        raise MissingSecret(f"failed retreiving environment secret: {response.stdout}")
+        raise MissingSecret(f"failed retrieving environment secret: {response.stdout}")
 
     return DecryptResponse(response.response.value)
 
 
 def rules():
     return [
         *collect_rules(),
```

### Comparing `pants-backend-secrets-0.1.0/pants_backend_secrets/goals/decrypt.py` & `pants-backend-secrets-0.2.0/pants_backend_secrets/goals/decrypt.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from __future__ import annotations
 
 from abc import ABCMeta
 from dataclasses import dataclass
 from typing import ClassVar, Generic, Type, TypeVar
 
 from pants.engine.console import Console
+from pants.engine.environment import EnvironmentName
 from pants.engine.goal import Goal, GoalSubsystem, Outputting
 from pants.engine.rules import Get, MultiGet, collect_rules, goal_rule
 from pants.engine.target import (
     FieldSet,
     ImmutableValue,
     NoApplicableTargetsBehavior,
     TargetRootsToFieldSets,
@@ -30,32 +31,24 @@
     name = "decrypt"
     help = "A decrypt goal for secrets."
 
 
 class Decrypt(Goal):
     subsystem_cls = DecryptSubsystem
 
+    environment_behavior = Goal.EnvironmentBehavior.LOCAL_ONLY
 
-_F = TypeVar("_F", bound=FieldSet)
 
+_F = TypeVar("_F", bound=FieldSet)
 
-if PANTS_SEMVER >= Version("2.15.0.dev0"):
-    from pants.engine.environment import EnvironmentName
 
-    @union(in_scope_types=[EnvironmentName])
-    @dataclass(frozen=True)
-    class DecryptRequest(Generic[_F]):
-        field_set: _F
-
-else:
-
-    @union
-    @dataclass(frozen=True)
-    class DecryptRequest(Generic[_F]):
-        field_set: _F
+@union(in_scope_types=[EnvironmentName])
+@dataclass(frozen=True)
+class DecryptRequest(Generic[_F]):
+    field_set: _F
 
 
 @dataclass(frozen=True)
 class DecryptResponse:
     secret: SecretValue
```

### Comparing `pants-backend-secrets-0.1.0/pants_backend_secrets/publish_secret_python.py` & `pants-backend-secrets-0.2.0/pants_backend_secrets/publish_secret_python.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from dataclasses import dataclass
 
 from pants.backend.python.goals.publish import (
     PublishPythonPackageFieldSet,
     PublishPythonPackageRequest,
     PythonRepositoriesField,
+    SkipTwineUploadField,
     twine_upload_args,
 )
 from pants.backend.python.subsystems.twine import TwineSubsystem
 from pants.backend.python.target_types import (
     BuildBackendEnvVarsField,
     GenerateSetupField,
     InterpreterConstraintsField,
@@ -17,15 +18,20 @@
     PythonProvidesField,
     SDistConfigSettingsField,
     SDistField,
     WheelConfigSettingsField,
     WheelField,
 )
 from pants.backend.python.util_rules.pex import PexRequest, VenvPex, VenvPexProcess
-from pants.core.goals.publish import PublishOutputData, PublishPackages, PublishProcesses
+from pants.core.goals.publish import (
+    PublishFieldSet,
+    PublishOutputData,
+    PublishPackages,
+    PublishProcesses,
+)
 from pants.core.util_rules.config_files import ConfigFiles, ConfigFilesRequest
 from pants.engine.addresses import Addresses, UnparsedAddressInputs
 from pants.engine.fs import CreateDigest, Digest, MergeDigests, Snapshot
 from pants.engine.process import InteractiveProcess, Process
 from pants.engine.rules import Get, MultiGet, collect_rules, rule
 from pants.engine.target import COMMON_TARGET_FIELDS, Target, WrappedTarget, WrappedTargetRequest
 from pants.option.global_options import GlobalOptions
@@ -41,27 +47,30 @@
     SecretsRequestWrap,
 )
 
 
 class PublishSecretsField(SecretsField):
     alias = "repo_secrets"
 
-    help = softwrap("Dictionary with all secrets to request. Each key should match a repository name.")
+    help = softwrap(
+        "Dictionary with all secrets to request. Each key should match a repository name."
+    )
 
 
 class PublishPythonWithSecretPackageRequest(PublishPythonPackageRequest):
     pass
 
 
 @dataclass(frozen=True)
-class PublishPythonWithSecretPackageFieldSet(PublishPythonPackageFieldSet):
+class PublishPythonWithSecretPackageFieldSet(PublishFieldSet):
     publish_request_type = PublishPythonWithSecretPackageRequest
-    required_fields = PublishPythonPackageFieldSet.required_fields + (PublishSecretsField,)
+    required_fields = (PublishSecretsField,)
 
-    secrets: PublishSecretsField
+    repositories: PublishSecretsField
+    skip_twine: SkipTwineUploadField
 
     def get_output_data(self) -> PublishOutputData:
         return PublishOutputData(
             {
                 "publisher": "twine",
                 **super().get_output_data(),
             }
@@ -97,15 +106,18 @@
 @rule
 async def twine_upload_with_secret(
     request: PublishPythonWithSecretPackageRequest,
     twine_subsystem: TwineSubsystem,
     global_options: GlobalOptions,
 ) -> PublishProcesses:
     dists = tuple(
-        artifact.relpath for pkg in request.packages for artifact in pkg.artifacts if artifact.relpath
+        artifact.relpath
+        for pkg in request.packages
+        for artifact in pkg.artifacts
+        if artifact.relpath
     )
 
     if twine_subsystem.skip or not dists:
         return PublishProcesses()
 
     # Too verbose to provide feedback as to why some packages were skipped?
     skip = None
@@ -138,65 +150,73 @@
 
     input_digest = await Get(
         Digest, MergeDigests((packages_digest, config_files.snapshot.digest, *ca_cert_digest))
     )
     pex_proc_requests = []
     secret_requests = []
 
-    for repo in request.field_set.repositories.value:
-        secret = request.field_set.secrets.value[repo]
+    repositories = []
+    for repo, secret in request.field_set.repositories.value.items():
+        repositories.append(repo)
         secret_address = await Get(
             Addresses,
             UnparsedAddressInputs(
                 [secret],
                 owning_address=request.field_set.address,
-                description_of_origin=f"the `{secret}` from the target {request.field_set.secrets}",
+                description_of_origin=f"the `{secret}` from the target {request.field_set.repositories}",
             ),
         )
         wrapped_target = await Get(
             WrappedTarget,
-            WrappedTargetRequest(secret_address[0], description_of_origin="twine_upload_with_secret"),
+            WrappedTargetRequest(
+                secret_address[0], description_of_origin="twine_upload_with_secret"
+            ),
         )
 
         secret_request = await Get(SecretsRequestWrap, SecretsRequestRequest(wrapped_target.target))
         if secret_request.request is None:
             raise NoDecrypterException(
                 f"No valid decrypter found for secret: `{secret_address[0]}` of "
                 f"type `{wrapped_target.target.alias}`"
             )
 
-        secret_requests.append(Get(FallibleSecretsResponse, FallibleSecretsRequest, secret_request.request))
+        secret_requests.append(
+            Get(FallibleSecretsResponse, FallibleSecretsRequest, secret_request.request)
+        )
 
     fallible_secrets = await MultiGet(*secret_requests)
     secrets = []
-    for repo, maybe_secret in zip(request.field_set.repositories.value, fallible_secrets):
+    for repo, maybe_secret in zip(repositories, fallible_secrets):
         if maybe_secret.exit_code != 0:
             raise FailedDecryptException(
                 f"Failed decrypting secret for repo: {repo}",
                 maybe_secret.stdout,
                 maybe_secret.stderr,
             )
 
+        assert maybe_secret.response is not None, "cannot be None if exit_code is 0"
         secrets.append(maybe_secret.response.value)
 
-    for repo, secret in zip(request.field_set.repositories.value, secrets):
+    for repo, secret in zip(repositories, secrets):
         pex_proc_requests.append(
             VenvPexProcess(
                 twine_pex,
                 argv=twine_upload_args(twine_subsystem, config_files, repo, dists, ca_cert),
                 input_digest=input_digest,
                 extra_env={
                     "TWINE_USERNAME": "__token__",
                     "TWINE_PASSWORD": secret.value,
                 },
                 description=repo,
             )
         )
 
-    processes = await MultiGet(Get(Process, VenvPexProcess, request) for request in pex_proc_requests)
+    processes = await MultiGet(
+        Get(Process, VenvPexProcess, request) for request in pex_proc_requests
+    )
 
     return PublishProcesses(
         PublishPackages(
             names=dists,
             process=InteractiveProcess.from_process(process),
             description=process.description,
             data=PublishOutputData({"repository": process.description}),
```

### Comparing `pants-backend-secrets-0.1.0/pants_backend_secrets/secret_request.py` & `pants-backend-secrets-0.2.0/pants_backend_secrets/secret_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import ClassVar
 
 from pants.engine.engine_aware import EngineAwareReturnType
+from pants.engine.environment import EnvironmentName
 from pants.engine.rules import collect_rules, rule
 from pants.engine.target import FieldSet, Target
 from pants.engine.unions import UnionMembership, union
 from pants.util.strutil import bullet_list
-from pants.version import PANTS_SEMVER, Version
 
 from pants_backend_secrets.exception import FailedDecryptException
 
 
 @dataclass(frozen=True)
 class SecretValue:
     """Wrapped for a secret which redacts its value when printed"""
@@ -36,32 +36,20 @@
 
         if self.source:
             msg += f" from `{self.source}`"
 
         return f"<{msg}>"
 
 
-if PANTS_SEMVER >= Version("2.15.0.dev0"):
-    from pants.engine.environment import EnvironmentName
-
-    @union(in_scope_types=[EnvironmentName])
-    @dataclass(frozen=True)
-    class FallibleSecretsRequest:
-        target: Target
-
-        field_set_type: ClassVar[FieldSet]
-
-else:
-
-    @union
-    @dataclass(frozen=True)
-    class FallibleSecretsRequest:
-        target: Target
+@union(in_scope_types=[EnvironmentName])
+@dataclass(frozen=True)
+class FallibleSecretsRequest:
+    target: Target
 
-        field_set_type: ClassVar[FieldSet]
+    field_set_type: ClassVar[FieldSet]
 
 
 @dataclass(frozen=True)
 class SecretsRequestRequest:
     target: Target
```

### Comparing `pants-backend-secrets-0.1.0/pyproject.toml` & `pants-backend-secrets-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "pants_backend_secrets"
 description = "A secrets plumbing plugin for the Pants build system"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
     { name = "Tom Solberg", email = "me@sbg.dev" },
 ]
 dependencies = []
 readme = "README.md"
 keywords = [
     "pantsbuild",
```

### Comparing `pants-backend-secrets-0.1.0/PKG-INFO` & `pants-backend-secrets-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pants_backend_secrets
-Version: 0.1.0
+Version: 0.2.0
 Summary: A secrets plumbing plugin for the Pants build system
 Keywords: pantsbuild,pants,backend,secrets
 Author-email: Tom Solberg <me@sbg.dev>
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Build Tools
 Project-URL: Changelog, https://github.com/tgolsson/pants-backends/tree/main/pants-plugins/secrets/CHANGELOG.md
```

