# Comparing `tmp/foxops-1.6.5.tar.gz` & `tmp/foxops-2.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxops-1.6.5.tar", max compression
+gzip compressed data, was "foxops-2.0.0a4.tar", max compression
```

## Comparing `foxops-1.6.5.tar` & `foxops-2.0.0a4.tar`

### file list

```diff
@@ -1,25 +1,55 @@
--rw-r--r--   0        0        0    11358 2022-08-19 09:34:21.666129 foxops-1.6.5/LICENSE
--rw-r--r--   0        0        0      517 2022-08-19 09:34:21.666129 foxops-1.6.5/README.md
--rw-r--r--   0        0        0     1871 2022-08-19 09:34:35.114030 foxops-1.6.5/pyproject.toml
--rw-r--r--   0        0        0       72 2022-08-19 09:34:21.666129 foxops-1.6.5/src/foxops/__init__.py
--rw-r--r--   0        0        0     4507 2022-08-19 09:34:21.666129 foxops-1.6.5/src/foxops/__main__.py
--rw-r--r--   0        0        0      814 2022-08-19 09:34:21.666129 foxops-1.6.5/src/foxops/engine/__init__.py
--rw-r--r--   0        0        0     9691 2022-08-19 09:34:21.666129 foxops-1.6.5/src/foxops/engine/__main__.py
--rw-r--r--   0        0        0     1234 2022-08-19 09:34:21.666129 foxops-1.6.5/src/foxops/engine/fvars.py
--rw-r--r--   0        0        0     4002 2022-08-19 09:34:21.666129 foxops-1.6.5/src/foxops/engine/initialization.py
--rw-r--r--   0        0        0     5057 2022-08-19 09:34:21.666129 foxops-1.6.5/src/foxops/engine/models.py
--rw-r--r--   0        0        0        0 2022-08-19 09:34:21.666129 foxops-1.6.5/src/foxops/engine/patching/__init__.py
--rw-r--r--   0        0        0     7067 2022-08-19 09:34:21.666129 foxops-1.6.5/src/foxops/engine/patching/git_diff_patch.py
--rw-r--r--   0        0        0     9151 2022-08-19 09:34:21.666129 foxops-1.6.5/src/foxops/engine/rendering.py
--rw-r--r--   0        0        0     5929 2022-08-19 09:34:21.666129 foxops-1.6.5/src/foxops/engine/update.py
--rw-r--r--   0        0        0      205 2022-08-19 09:34:21.666129 foxops-1.6.5/src/foxops/errors.py
--rw-r--r--   0        0        0        0 2022-08-19 09:34:21.666129 foxops-1.6.5/src/foxops/external/__init__.py
--rw-r--r--   0        0        0     7372 2022-08-19 09:34:21.666129 foxops-1.6.5/src/foxops/external/git.py
--rw-r--r--   0        0        0     6520 2022-08-19 09:34:21.666129 foxops-1.6.5/src/foxops/external/gitlab.py
--rw-r--r--   0        0        0     2422 2022-08-19 09:34:21.666129 foxops-1.6.5/src/foxops/loggingcfg.py
--rw-r--r--   0        0        0     1546 2022-08-19 09:34:21.666129 foxops-1.6.5/src/foxops/models.py
--rw-r--r--   0        0        0    19334 2022-08-19 09:34:21.666129 foxops-1.6.5/src/foxops/reconciliation.py
--rw-r--r--   0        0        0      325 2022-08-19 09:34:21.666129 foxops-1.6.5/src/foxops/settings.py
--rw-r--r--   0        0        0     2244 2022-08-19 09:34:21.666129 foxops-1.6.5/src/foxops/utils.py
--rw-r--r--   0        0        0     1602 2022-08-19 09:34:35.153903 foxops-1.6.5/setup.py
--rw-r--r--   0        0        0     1207 2022-08-19 09:34:35.154269 foxops-1.6.5/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-18 13:07:08.074449 foxops-2.0.0a4/LICENSE
+-rw-r--r--   0        0        0      517 2023-06-18 13:07:08.074449 foxops-2.0.0a4/README.md
+-rw-r--r--   0        0        0     2138 2023-06-18 13:07:28.934662 foxops-2.0.0a4/pyproject.toml
+-rw-r--r--   0        0        0       72 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/__init__.py
+-rw-r--r--   0        0        0     3451 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/database/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/database/repositories/__init__.py
+-rw-r--r--   0        0        0    11781 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/database/repositories/change.py
+-rw-r--r--   0        0        0        0 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/database/repositories/incarnation/__init__.py
+-rw-r--r--   0        0        0      111 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/database/repositories/incarnation/errors.py
+-rw-r--r--   0        0        0      209 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/database/repositories/incarnation/model.py
+-rw-r--r--   0        0        0     2541 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/database/repositories/incarnation/repository.py
+-rw-r--r--   0        0        0     1411 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/database/schema.py
+-rw-r--r--   0        0        0     3805 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/dependencies.py
+-rw-r--r--   0        0        0      814 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/engine/__init__.py
+-rw-r--r--   0        0        0     9434 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/engine/__main__.py
+-rw-r--r--   0        0        0      275 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/engine/custom_filters.py
+-rw-r--r--   0        0        0     1233 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/engine/fvars.py
+-rw-r--r--   0        0        0     4399 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/engine/initialization.py
+-rw-r--r--   0        0        0     5137 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/engine/models.py
+-rw-r--r--   0        0        0        0 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/engine/patching/__init__.py
+-rw-r--r--   0        0        0     8976 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/engine/patching/git_diff_patch.py
+-rw-r--r--   0        0        0     9071 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/engine/rendering.py
+-rw-r--r--   0        0        0     6114 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/engine/update.py
+-rw-r--r--   0        0        0     1009 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/error_handlers.py
+-rw-r--r--   0        0        0     1697 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/errors.py
+-rw-r--r--   0        0        0        0 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/external/__init__.py
+-rw-r--r--   0        0        0     8563 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/external/git.py
+-rw-r--r--   0        0        0      141 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/hosters/__init__.py
+-rw-r--r--   0        0        0      113 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/hosters/gitlab/__init__.py
+-rw-r--r--   0        0        0    19920 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/hosters/gitlab/gitlab.py
+-rw-r--r--   0        0        0      431 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/hosters/gitlab/settings.py
+-rw-r--r--   0        0        0     8110 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/hosters/local.py
+-rw-r--r--   0        0        0     2377 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/hosters/types.py
+-rw-r--r--   0        0        0     2557 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/logger.py
+-rw-r--r--   0        0        0      988 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/middlewares.py
+-rw-r--r--   0        0        0      359 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/models/__init__.py
+-rw-r--r--   0        0        0      580 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/models/change.py
+-rw-r--r--   0        0        0     1224 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/models/desired_incarnation_state.py
+-rw-r--r--   0        0        0       77 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/models/errors.py
+-rw-r--r--   0        0        0      267 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/models/helpers.py
+-rw-r--r--   0        0        0     1243 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/models/incarnation.py
+-rw-r--r--   0        0        0      655 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/openapi.py
+-rw-r--r--   0        0        0        0 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/routers/__init__.py
+-rw-r--r--   0        0        0      407 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/routers/auth.py
+-rw-r--r--   0        0        0      935 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/routers/changes.py
+-rw-r--r--   0        0        0    11911 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/routers/incarnations.py
+-rw-r--r--   0        0        0      331 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/routers/not_found.py
+-rw-r--r--   0        0        0      351 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/routers/version.py
+-rw-r--r--   0        0        0        0 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/services/__init__.py
+-rw-r--r--   0        0        0    29073 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/services/change.py
+-rw-r--r--   0        0        0     1566 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/services/incarnation.py
+-rw-r--r--   0        0        0      638 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/settings.py
+-rw-r--r--   0        0        0     2201 2023-06-18 13:07:08.078449 foxops-2.0.0a4/src/foxops/utils.py
+-rw-r--r--   0        0        0     1607 1970-01-01 00:00:00.000000 foxops-2.0.0a4/PKG-INFO
```

### Comparing `foxops-1.6.5/LICENSE` & `foxops-2.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `foxops-1.6.5/README.md` & `foxops-2.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `foxops-1.6.5/src/foxops/engine/__init__.py` & `foxops-2.0.0a4/src/foxops/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `foxops-1.6.5/src/foxops/engine/__main__.py` & `foxops-2.0.0a4/src/foxops/engine/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import asyncio
+import copy
 import logging
 from dataclasses import asdict
 from pathlib import Path
 from subprocess import PIPE, check_output
 from typing import Optional
 
 import typer
-from structlog.stdlib import BoundLogger
 
 from foxops.engine.initialization import initialize_incarnation
 from foxops.engine.models import (
     IncarnationState,
     TemplateConfig,
     TemplateData,
     VariableDefinition,
     load_incarnation_state,
 )
 from foxops.engine.patching.git_diff_patch import diff_and_patch
 from foxops.engine.update import update_incarnation_from_git_template_repository
-from foxops.loggingcfg import get_logger, setup_logging
+from foxops.logger import bind, get_logger, setup_logging
 
 app = typer.Typer()
 
-logger: BoundLogger
+#: Holds the module logger
+logger = get_logger(__name__)
 
 
 @app.command(name="new", help="Creates a new template scaffold in the given directory")
 def cmd_new(
     target_directory: Path = typer.Argument(  # noqa: B008
         ...,
         exists=False,
@@ -53,17 +54,15 @@
             )
         }
     )
     template_config.to_yaml(target_directory / "fengine.yaml")
 
     # Create sample README in template directory
     (target_directory / "template").mkdir(0o755)
-    (target_directory / "template" / "README.md").write_text(
-        "Created by {{ author }}\n"
-    )
+    (target_directory / "template" / "README.md").write_text("Created by {{ author }}\n")
 
 
 @app.command(name="initialize")
 def cmd_initialize(
     template_repository: Path = typer.Argument(  # noqa: B008
         ...,
         exists=True,
@@ -87,65 +86,54 @@
     template_repository_version: Optional[str] = typer.Option(  # noqa: B008
         None,
         "--template-version",
         help="Template repository version to use",
     ),
 ):
     """Initialize an incarnation repository with a version of a template and some data."""
-    template_data: TemplateData = dict(
-        tuple(x.split("=", maxsplit=1)) for x in raw_template_data  # type: ignore
-    )
+    template_data: TemplateData = dict(tuple(x.split("=", maxsplit=1)) for x in raw_template_data)  # type: ignore
 
-    log = logger.bind(
-        template_repository=template_repository,
-        incarnation_dir=incarnation_dir,
-        template_data=template_data,
-    )
+    bind(template_repository=template_repository)
+    bind(incarnation_dir=incarnation_dir)
+    bind(template_data=template_data)
 
-    log.debug("creating empty incarnation directory")
+    logger.debug("creating empty incarnation directory")
     incarnation_dir.mkdir(parents=True, exist_ok=False)
 
     if template_repository_version:
-        log.debug(
-            f"checking out template repository version {template_repository_version}"
-        )
+        logger.debug(f"checking out template repository version {template_repository_version}")
         check_output(
             ["git", "checkout", template_repository_version],
             cwd=template_repository,
             stderr=PIPE,
         )
 
-    repository_version = (
-        check_output(["git", "rev-parse", "HEAD"], cwd=template_repository)
-        .decode()
-        .strip()
-    )
+    repository_version = check_output(["git", "rev-parse", "HEAD"], cwd=template_repository).decode().strip()
 
-    log.info(
+    logger.info(
         "starting initialization incarnation ...",
         template_repository=str(template_repository),
         template_repository_version=repository_version,
         template_data=template_data,
     )
 
     try:
         asyncio.run(
             initialize_incarnation(
                 template_root_dir=template_repository,
                 template_repository=str(template_repository),
                 template_repository_version=repository_version,
                 template_data=template_data,
                 incarnation_root_dir=incarnation_dir,
-                logger=log,
             )
         )
     except Exception as exc:
-        log.exception(f"initialization failed: {exc}")
+        logger.exception(f"initialization failed: {exc}")
     else:
-        log.info("successfully initialized incarnation")
+        logger.info("successfully initialized incarnation")
     finally:
         if template_repository_version:
             check_output(
                 ["git", "checkout", "-"],
                 cwd=template_repository,
                 stderr=PIPE,
             )
@@ -182,33 +170,27 @@
         None,
         "--template-repository",
         "-r",
         help="Override the template repository with a local path recorded in the incarnation state",
     ),
 ):
     """Initialize an incarnation repository with a version of a template and some data."""
-    template_data: dict[str, str] = dict(
-        tuple(x.split("=", maxsplit=1)) for x in raw_template_data  # type: ignore
-    )
+    template_data: dict[str, str] = dict(tuple(x.split("=", maxsplit=1)) for x in raw_template_data)  # type: ignore
 
     incarnation_state_path = incarnation_dir / ".fengine.yaml"
-    logger.debug(
-        f"getting template repository path from incarnation state at {incarnation_state_path}"
-    )
+    logger.debug(f"getting template repository path from incarnation state at {incarnation_state_path}")
     incarnation_state = load_incarnation_state(incarnation_state_path)
 
     logger.debug(
         f"loaded incarnation state from incarnation repository {incarnation_state_path}",
         incarnation_state=incarnation_state,
     )
 
     if overridden_template_repository is not None:
-        logger.debug(
-            f"overriding template repository with {overridden_template_repository}"
-        )
+        logger.debug(f"overriding template repository with {overridden_template_repository}")
         incarnation_state = IncarnationState(
             **{
                 **asdict(incarnation_state),  # type: ignore
                 "template_repository": str(overridden_template_repository),
             }
         )
 
@@ -221,81 +203,70 @@
         raise typer.Exit(1)
 
     logger.debug(
         "updating template data from incarnation state with given data from user",
         incarnation_state_data=incarnation_state.template_data,
         user_template_data=template_data,
     )
-    merged_template_data = incarnation_state.template_data.copy()
+    merged_template_data = dict(copy.deepcopy(incarnation_state.template_data))
     merged_template_data.update(template_data)
-    merged_template_data = {
-        k: v for k, v in merged_template_data.items() if k not in remove_template_data
-    }
-
-    log = logger.bind(
-        template_repository=incarnation_state.template_repository,
-        incarnation_dir=incarnation_dir,
-        template_data=merged_template_data,
-    )
+    merged_template_data = {k: v for k, v in merged_template_data.items() if k not in remove_template_data}
+
+    bind(template_repository=incarnation_state.template_repository)
+    bind(incarnation_dir=incarnation_dir)
+    bind(template_data=merged_template_data)
 
     if update_repository_version is None:
         update_repository_version = (
-            check_output(
-                ["git", "rev-parse", "HEAD"], cwd=incarnation_state.template_repository
-            )
+            check_output(["git", "rev-parse", "HEAD"], cwd=incarnation_state.template_repository)
             .decode("utf-8")
             .strip()
         )
 
-    log.info(
+    logger.info(
         f"starting update of incarnation to version {update_repository_version}...",
         template_repository=str(incarnation_state.template_repository),
         template_repository_version=update_repository_version,
         template_data=merged_template_data,
     )
 
     try:
-        files_with_conflicts = asyncio.run(
+        _, _, patch_result = asyncio.run(
             update_incarnation_from_git_template_repository(
-                template_git_root_dir=Path(incarnation_state.template_repository),
-                update_template_repository=str(incarnation_state.template_repository),
+                template_git_repository=Path(incarnation_state.template_repository),
                 update_template_repository_version=update_repository_version,
                 update_template_data=merged_template_data,
                 incarnation_root_dir=incarnation_dir,
                 diff_patch_func=diff_and_patch,
-                logger=log,
             )
         )
 
-        if files_with_conflicts:
-            log.error(
-                f"update failed, there were conflicts while updating the following files: {', '.join([str(f) for f in files_with_conflicts])}"
+        if patch_result and patch_result.has_errors():
+            logger.error(
+                f"update failed, there were conflicts while updating the "
+                f"following files: {', '.join([str(f) for f in patch_result.conflicts])}"
+            )
+            logger.error(
+                f"update failed, the following files had changes, but didn't exist anymore "
+                f"in the incarnation: {', '.join([str(f) for f in patch_result.deleted])}"
             )
         else:
-            log.info("successfully updated incarnation")
+            logger.info("successfully updated incarnation")
     except Exception as exc:
-        log.exception(f"update failed: {exc}")
+        logger.exception(f"update failed: {exc}")
 
 
 @app.callback()
 def main(
-    verbose: bool = typer.Option(  # noqa: B008
-        False, "--verbose", "-v", help="turn on verbose logging"
-    ),
-    logs_as_json: bool = typer.Option(  # noqa: B008
-        False, "--json-logs", "-j", help="render logs as JSON"
-    ),
+    verbose: bool = typer.Option(False, "--verbose", "-v", help="turn on verbose logging"),  # noqa: B008
 ):
     """
     Foxops engine ... use it to initialize or update template incarnations.
     """
     if verbose:
-        setup_logging(logging.DEBUG, logs_as_json)
+        setup_logging(level=logging.DEBUG)
     else:
-        setup_logging(logging.INFO, logs_as_json)
-
-    global logger
-    logger = get_logger("app")
+        setup_logging(level=logging.INFO)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `foxops-1.6.5/src/foxops/engine/fvars.py` & `foxops-2.0.0a4/src/foxops/engine/fvars.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 from pathlib import Path
 
-from structlog.stdlib import BoundLogger
-
 from foxops.engine.models import TemplateData
+from foxops.logger import get_logger
+
+#: Holds the module logger
+logger = get_logger(__name__)
 
 #: Holds the filename for the fvars file.
 FVARS_FILENAME = "default.fvars"
 
 
 def merge_template_data_with_fvars(
     template_data: TemplateData,
     fvars_directory: Path,
-    logger: BoundLogger,
 ) -> TemplateData:
     """Merge the given Template data with fvars.
 
     The fvars filename is hardcoded as `default.fvars`.
 
     The `template_data` takes precedence over fvars.
     If no fvars file in `fvars_directory` exists, the `template_data` is returned.
     """
     fvars_path = fvars_directory / FVARS_FILENAME
-    fvars = read_variables_from_fvars_file(fvars_path, logger)
+    fvars = read_variables_from_fvars_file(fvars_path)
     return {**fvars, **template_data}
 
 
-def read_variables_from_fvars_file(path: Path, logger: BoundLogger) -> TemplateData:
+def read_variables_from_fvars_file(path: Path) -> TemplateData:
     """Read variables from a fvars file.
 
     If the file does not exist an empty `TemplateData` is returned.
     """
     if not path.exists():
         return {}
```

### Comparing `foxops-1.6.5/src/foxops/engine/initialization.py` & `foxops-2.0.0a4/src/foxops/engine/initialization.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,106 +1,106 @@
+import copy
 from pathlib import Path
 
-from structlog.stdlib import BoundLogger
-
 from foxops.engine.fvars import merge_template_data_with_fvars
 from foxops.engine.models import (
     IncarnationState,
     TemplateData,
     fill_missing_optionals_with_defaults,
     load_template_config,
     save_incarnation_state,
 )
 from foxops.engine.rendering import render_template
+from foxops.errors import ReconciliationUserError
 from foxops.external.git import GitRepository
+from foxops.logger import get_logger
+
+#: Holds the module logger
+logger = get_logger(__name__)
 
 
 async def initialize_incarnation(
     template_root_dir: Path,
     template_repository: str,
     template_repository_version: str,
     template_data: TemplateData,
     incarnation_root_dir: Path,
-    logger: BoundLogger,
 ) -> IncarnationState:
     """Initialize an incarnation repository with a version of a template.
 
     The initialization process consists of the following steps:
         * ensure incarnation directory exists
         * render template directory file system contents into incarnation directory
     """
     template_data = merge_template_data_with_fvars(
         template_data=template_data,
         fvars_directory=incarnation_root_dir,
-        logger=logger,
     )
     return await _initialize_incarnation(
         template_root_dir=template_root_dir,
         template_repository=template_repository,
         template_repository_version=template_repository_version,
         template_data=template_data,
         incarnation_root_dir=incarnation_root_dir,
-        logger=logger,
     )
 
 
 async def _initialize_incarnation(
     template_root_dir: Path,
     template_repository: str,
     template_repository_version: str,
     template_data: TemplateData,
     incarnation_root_dir: Path,
-    logger: BoundLogger,
 ) -> IncarnationState:
     # verify that the template data in the desired incarnation state match the required template variables
     template_config = load_template_config(template_root_dir / "fengine.yaml")
-    logger.debug(
-        f"load template config from {template_config} to initialize incarnation at {incarnation_root_dir}"
-    )
+    logger.debug(f"load template config from {template_config} to initialize incarnation at {incarnation_root_dir}")
     required_variable_names = set(template_config.required_variables.keys())
     provided_variable_names = set(template_data.keys())
     if not required_variable_names.issubset(provided_variable_names):
-        raise ValueError(
+        raise ReconciliationUserError(
             f"the template required the variables {sorted(required_variable_names)} "
             "but the provided template data for the incarnation "
             f"where {sorted(provided_variable_names)}. "
             "Please make sure that the provided ones are a superset of the required ones."
         )
 
     # log additional template data passed for the incarnation
     config_variable_names = set(template_config.variables.keys())
     if additional_values := provided_variable_names - config_variable_names:
-        logger.warn(
-            f"got additional template data for the incarnation: {sorted(additional_values)}"
-        )
+        logger.warn(f"got additional template data for the incarnation: {sorted(additional_values)}")
 
     # fill defaults in passed data
     template_data_with_defaults = fill_missing_optionals_with_defaults(
         provided_template_data=template_data,
         template_config=template_config,
-        logger=logger,
+    )
+
+    # add meta-information to the template data.
+    # ... we don't want to include that in the "template_data" section of the `.fengine.yaml` file
+    template_data_with_defaults_and_metadata = dict(copy.deepcopy(template_data_with_defaults))
+    template_data_with_defaults_and_metadata.update(
+        {
+            "_fengine_template_repository": template_repository,
+            "_fengine_template_repository_version": template_repository_version,
+        }
     )
 
     await render_template(
         template_root_dir / "template",
         incarnation_root_dir,
-        template_data_with_defaults,
+        template_data_with_defaults_and_metadata,
         rendering_filename_exclude_patterns=template_config.rendering.excluded_files,
-        logger=logger,
     )
 
-    template_repository_version_hash = await GitRepository(
-        template_root_dir, logger
-    ).head()
+    template_repository_version_hash = await GitRepository(template_root_dir).head()
     incarnation_state = IncarnationState(
         template_repository=template_repository,
         template_repository_version=template_repository_version,
         template_repository_version_hash=template_repository_version_hash,
         template_data=template_data_with_defaults,
     )
 
     incarnation_config_path = Path(incarnation_root_dir, ".fengine.yaml")
     save_incarnation_state(incarnation_config_path, incarnation_state)
-    logger.debug(
-        f"save incarnation state to {incarnation_config_path} after template initialization"
-    )
+    logger.debug(f"save incarnation state to {incarnation_config_path} after template initialization")
     return incarnation_state
```

### Comparing `foxops-1.6.5/src/foxops/engine/models.py` & `foxops-2.0.0a4/src/foxops/engine/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,28 @@
+import copy
 from dataclasses import asdict, dataclass
 from pathlib import Path
+from typing import Annotated, Mapping
 
 from pydantic import BaseModel, Field
 from ruamel.yaml import YAML
-from structlog.stdlib import BoundLogger
+
+from foxops.logger import get_logger
+
+#: Holds the module logger
+logger = get_logger(__name__)
 
 yaml = YAML(typ="safe")
 yaml.default_flow_style = False
 
 
 #: Holds the type for all `template_data` dictionary values
 TemplateDataValue = str | int | float
 #: Holds the type for all `template_data` dictionaries
-TemplateData = dict[str, TemplateDataValue]
+TemplateData = Mapping[str, TemplateDataValue]
 
 
 @dataclass(frozen=True)
 class IncarnationState:
     """Represents an Incarnation State record.
 
     The incarnation state is recorded for every incarnation in `.fengine.yaml`
@@ -34,17 +40,15 @@
     #: Holds a git sha of the template repository the `template_repository_version` points to
     template_repository_version_hash: str
     #: Holds a dict of string key value pairs which have been used to
     #: as template render data.
     template_data: TemplateData
 
 
-def save_incarnation_state(
-    incarnation_state_path: Path, incarnation_state: IncarnationState
-) -> None:
+def save_incarnation_state(incarnation_state_path: Path, incarnation_state: IncarnationState) -> None:
     with incarnation_state_path.open("w") as f:
         f.write("# This file is auto-generated and owned by foxops.\n")
         f.write("# DO NOT EDIT MANUALLY.\n")
         yaml.dump(asdict(incarnation_state), f)
 
 
 def load_incarnation_state(incarnation_state_path: Path) -> IncarnationState:
@@ -57,18 +61,18 @@
     raw_state = yaml.load(incarnation_state)
     return IncarnationState(**raw_state)
 
 
 class VariableDefinition(BaseModel):
     type: str = Field(..., description="The type of the variable")
     description: str = Field(..., help="The description for this variable")
-    default: TemplateDataValue | None = Field(
-        None,
-        help="The default value for this variable (setting this makes the variable optional)",
-    )
+    default: Annotated[
+        TemplateDataValue | None,
+        Field(help="The default value for this variable (setting this makes the variable optional)"),
+    ] = None
 
     def is_required(self) -> bool:
         return self.default is None
 
     class Config:
         allow_mutation = False
 
@@ -110,17 +114,15 @@
 
     @property
     def required_variables(self) -> dict[str, VariableDefinition]:
         return {k: v for k, v in self.variables.items() if v.is_required()}
 
     @property
     def optional_variables_defaults(self) -> TemplateData:
-        return {
-            k: v.default for k, v in self.variables.items() if v.default is not None
-        }
+        return {k: v.default for k, v in self.variables.items() if v.default is not None}
 
     def to_yaml(self, target: Path) -> None:
         with target.open("w") as f:
             yaml.dump(self.dict(), f)
 
     class Config:
         allow_mutation = False
@@ -134,19 +136,18 @@
     except FileNotFoundError:
         return TemplateConfig()
 
 
 def fill_missing_optionals_with_defaults(
     provided_template_data: TemplateData,
     template_config: TemplateConfig,
-    logger: BoundLogger,
 ) -> TemplateData:
     provided_variable_names = set(provided_template_data.keys())
     config_variable_names = set(template_config.variables.keys())
-    template_data_with_defaults = provided_template_data.copy()
+    template_data_with_defaults = dict(copy.deepcopy(provided_template_data))
     optional_vars = template_config.optional_variables_defaults
     if need_default := config_variable_names.difference(provided_variable_names):
         logger.debug(
             f"Given template data is missing the values for the optional variables {need_default}, using defaults for those"
         )
         for key in (k for k in need_default if k in optional_vars):
             template_data_with_defaults[key] = optional_vars[key]
```

### Comparing `foxops-1.6.5/src/foxops/engine/patching/git_diff_patch.py` & `foxops-2.0.0a4/src/foxops/engine/patching/git_diff_patch.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,72 @@
 import filecmp
+import os
 import re
 import shutil
 import typing
 from contextlib import asynccontextmanager
+from dataclasses import dataclass
 from pathlib import Path
 from tempfile import TemporaryDirectory, mkstemp
 
-from structlog.stdlib import BoundLogger
-
 from foxops.external.git import GitRepository
-from foxops.settings import Settings
+from foxops.logger import get_logger
 from foxops.utils import CalledProcessError, check_call
 
+#: Holds the module logger
+logger = get_logger(__name__)
+
+
+@dataclass
+class PatchResult:
+    # file paths that should have been patched, but could not because of a conflict
+    conflicts: list[Path]
+    # file paths that should have been patched, but could not because of a missing file
+    deleted: list[Path]
+
+    def has_errors(self) -> bool:
+        return len(self.conflicts) >= 1 or len(self.deleted) >= 1
+
 
 async def diff_and_patch(
     diff_a_directory: Path,
     diff_b_directory: Path,
     patch_directory: Path,
-    logger: BoundLogger,
-) -> list[Path]:
-    patch_path = await diff(diff_a_directory, diff_b_directory, logger=logger)
-    try:
-        return await patch(
-            patch_path,
-            patch_directory,
-            diff_a_directory,
-            diff_b_directory,
-            logger=logger,
-        )
-    finally:
-        patch_path.unlink()
+) -> PatchResult | None:
+    if (patch_path := await diff(diff_a_directory, diff_b_directory)) is not None:
+        try:
+            return await patch(
+                patch_path,
+                patch_directory,
+                diff_b_directory,
+            )
+        finally:
+            patch_path.unlink()
+    return None
 
 
 @asynccontextmanager
-async def setup_diff_git_repository(
-    old_directory: Path, new_directory: Path
-) -> typing.AsyncGenerator[Path, None]:
+async def setup_diff_git_repository(old_directory: Path, new_directory: Path) -> typing.AsyncGenerator[Path, None]:
     # FIXME(TF): in case the *git way* provides as the viable long-term solution we could directly
     #            bootstrap that intermediate git repository instead of this copy-paste roundtrip.
-    settings = Settings()
     git_tmpdir: str
     with TemporaryDirectory() as git_tmpdir:
         await check_call("git", "init", ".", "--initial-branch", "main", cwd=git_tmpdir)
         await check_call(
             "git",
             "config",
             "user.name",
-            settings.git_commit_author_name,
+            "fengine",
             cwd=git_tmpdir,
         )
         await check_call(
             "git",
             "config",
             "user.email",
-            settings.git_commit_author_email,
+            "noreply@fengine.io",
             cwd=git_tmpdir,
         )
         await check_call(
             "git",
             "commit",
             "--allow-empty",
             "-m",
@@ -72,131 +81,157 @@
         shutil.copytree(new_directory, git_tmpdir, dirs_exist_ok=True)
         await check_call("git", "add", ".", cwd=git_tmpdir)
         await check_call("git", "commit", "-m", "new template status", cwd=git_tmpdir)
 
         yield Path(git_tmpdir)
 
 
-async def diff(old_directory: Path, new_directory: Path, logger: BoundLogger) -> Path:
+async def diff(old_directory: Path, new_directory: Path) -> Path | None:
     async with setup_diff_git_repository(old_directory, new_directory) as git_tmpdir:
         logger.debug(f"create git diff between branch old and new in {git_tmpdir}")
 
-        repo = GitRepository(git_tmpdir, logger)
+        repo = GitRepository(git_tmpdir)
         diff_output = await repo.diff("old", "new")
 
-        patch_path: str
-        _, patch_path = mkstemp(prefix="fengine-update-", suffix=".patch")
+        if diff_output == "":
+            logger.info("The update didn't change anything, no patch to create")
+            return None
+
+        logger.debug("create patch from git diff", diff_output=diff_output)
+        fd, patch_path = mkstemp(prefix="fengine-update-", suffix=".patch")
+        os.close(fd)
 
         (p := Path(patch_path)).write_text(diff_output)
         return p
 
 
 async def patch(
     patch_path: Path,
     incarnation_root_dir: Path,
-    diff_a_directory: Path,
-    diff_b_directory: Path,
-    logger: BoundLogger,
-) -> list[Path]:
+    rendered_updated_template_directory: Path,
+) -> PatchResult:
     # NOTE(TF): it's crucial that the paths are fully resolved here,
     #           because we are going to fiddle around how they
     #           are relative to each other.
     resolved_incarnation_root_dir = incarnation_root_dir.resolve()
-    proc = await check_call(
-        "git", "rev-parse", "--show-toplevel", cwd=str(resolved_incarnation_root_dir)
-    )
-    incarnation_git_root_dir = Path((await proc.stdout.read()).decode("utf-8").strip()).resolve()  # type: ignore
-    incarnation_git_dir = (
-        resolved_incarnation_root_dir.relative_to(incarnation_git_root_dir)
-        if resolved_incarnation_root_dir != incarnation_git_root_dir
-        else ""
+    proc = await check_call("git", "rev-parse", "--show-toplevel", cwd=str(resolved_incarnation_root_dir))
+    incarnation_repository_dir = Path((await proc.stdout.read()).decode("utf-8").strip()).resolve()  # type: ignore
+    incarnation_subdir = (
+        resolved_incarnation_root_dir.relative_to(incarnation_repository_dir)
+        if resolved_incarnation_root_dir != incarnation_repository_dir
+        else None
     )
 
     # FIXME(TF): may check git status to check if something has been modified or not ...
-    logger.debug(
-        f"applying patch {patch_path} to {incarnation_git_dir} inside {incarnation_root_dir}"
-    )
+    logger.debug(f"applying patch {patch_path} to {incarnation_subdir} inside {incarnation_root_dir}")
     try:
+        # The `--reject` option makes it apply the parts of the patch that are applicable,
+        # and leave the rejected hunks in corresponding *.rej files.
+        git_apply_options = [
+            "--reject",
+            "--verbose",
+        ]
+        if incarnation_subdir is not None:
+            git_apply_options.extend(["--directory", str(incarnation_subdir)])
+
         await check_call(
             "git",
             "apply",
-            "--reject",  # This option makes it apply the parts of the patch that are applicable, and leave the rejected hunks in corresponding *.rej files.
-            "--verbose",
-            "--directory",
-            str(incarnation_git_dir),
+            *git_apply_options,
             str(patch_path),
-            cwd=str(incarnation_git_root_dir),
+            cwd=str(incarnation_repository_dir),
         )
     except CalledProcessError as exc:
         logger.debug(
             "detected conflicts with patch, analyzing rejections ...",
             patch_path=patch_path,
+            exc=exc,
         )
         apply_rejection_output = exc.stderr
-        files_with_conflicts = await analyze_patch_rejections(
+        return await analyze_patch_rejections(
             apply_rejection_output,
-            resolved_incarnation_root_dir,
-            diff_a_directory,
-            diff_b_directory,
-            logger=logger,
+            incarnation_repository_dir,
+            incarnation_subdir,
+            rendered_updated_template_directory,
         )
-        return files_with_conflicts
     else:
-        return []
+        return PatchResult(conflicts=[], deleted=[])
 
 
 async def analyze_patch_rejections(
     apply_rejection_output: bytes,
-    patch_directory: Path,
-    diff_a_directory: Path,
-    diff_b_directory: Path,
-    logger: BoundLogger,
-) -> list[Path]:
-    reject_file_regex = re.compile(rb"Applying patch (.*?) with (\d+) reject...")
+    incarnation_repository_dir: Path,
+    incarnation_subdir: Path | None,
+    rendered_updated_template_directory: Path,
+) -> PatchResult:
+    if incarnation_subdir is None:
+        incarnation_dir = incarnation_repository_dir
+    else:
+        incarnation_dir = incarnation_repository_dir / incarnation_subdir
 
-    files_with_rejections = []
-    for line in apply_rejection_output.splitlines():
-        if match := reject_file_regex.match(line):
-            files_with_rejections.append(Path(match.group(1).decode()))
+    patch_outcome = parse_git_apply_rejection_output(apply_rejection_output)
 
-    logger.debug(
-        f"detected {len(files_with_rejections)} files with rejections",
-        files_with_rejections=files_with_rejections,
-    )
     files_with_conflicts: list[Path] = []
-    for file_with_rejection in files_with_rejections:
+    for file_with_rejection in patch_outcome.conflicts:
         conflict_fixed = await attempt_fixing_rejection(
-            file_with_rejection,
-            patch_directory,
-            diff_a_directory,
-            diff_b_directory,
-            logger=logger,
+            (incarnation_repository_dir / file_with_rejection).relative_to(incarnation_dir),
+            incarnation_dir,
+            rendered_updated_template_directory,
         )
         if not conflict_fixed:
             logger.debug(f"file {file_with_rejection} still has conflicts")
             files_with_conflicts.append(file_with_rejection)
-    return files_with_conflicts
+    return PatchResult(conflicts=files_with_conflicts, deleted=patch_outcome.deleted)
 
 
 async def attempt_fixing_rejection(
     file_with_rejection: Path,
     patch_directory: Path,
-    diff_a_directory: Path,
     diff_b_directory: Path,
-    logger: BoundLogger,
 ) -> bool:
-    # diff_a_file = diff_a_directory / file_with_rejection
     diff_b_file = diff_b_directory / file_with_rejection
     patch_file = patch_directory / file_with_rejection
+    if not diff_b_file.exists() or not patch_file.exists():
+        logger.info("could not fix rejection - file doesn't exist anymore", file=file_with_rejection)
+        return False
 
     logger.debug(f"attempting to fix rejection for file {file_with_rejection} ...")
 
     if filecmp.cmp(diff_b_file, patch_file, shallow=True):
         # the rejected hunk tried to apply a change which was already applied,
         # we can safely remove the rejection file.
         (patch_file.with_suffix(patch_file.suffix + ".rej")).unlink()
         logger.debug(
             f"the rejection was caused because the two files are identical, mark {file_with_rejection} as fixed"
         )
         return True
 
     return False
+
+
+def parse_git_apply_rejection_output(output: bytes) -> PatchResult:
+    """
+    Parse the output of `git apply --reject` to extract the list of files.
+
+    Returns:
+        list[Path]: the list of filenames with rejections. The returned paths are relative to the repository root.
+        list[Path]: the list of filenames that have changes but have been deleted in the incarnation.
+                    The returned paths are relative to the repository root.
+    """
+    reject_file_regex = re.compile(rb"Applying patch (.*?) with (\d+) reject...")
+    deleted_target_regex = re.compile(rb"error: (.*): No such file or directory")
+
+    files_with_rejections = []
+    deleted_target_files = []
+    for line in output.splitlines():
+        if match := reject_file_regex.match(line):
+            files_with_rejections.append(Path(match.group(1).decode()))
+        if match := deleted_target_regex.match(line):
+            deleted_target_files.append(Path(match.group(1).decode()))
+
+    logger.debug(
+        f"detected {len(files_with_rejections)} files with rejections and {len(deleted_target_files)} deleted target files",
+        files_with_rejections=files_with_rejections,
+        deleted_target_files=deleted_target_files,
+    )
+
+    return PatchResult(conflicts=files_with_rejections, deleted=deleted_target_files)
```

### Comparing `foxops-1.6.5/src/foxops/engine/rendering.py` & `foxops-2.0.0a4/src/foxops/engine/rendering.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,21 @@
 import os
 import typing
 from pathlib import Path
 
 from aiopath import AsyncPath
 from jinja2 import FileSystemLoader, StrictUndefined
 from jinja2.sandbox import SandboxedEnvironment
-from structlog.stdlib import BoundLogger
 
+from foxops.engine.custom_filters import ip_add_integer
 from foxops.engine.models import TemplateData
+from foxops.logger import get_logger
+
+#: Holds the module logger
+logger = get_logger(__name__)
 
 
 def create_template_environment(template_root_dir: Path) -> SandboxedEnvironment:
     """Create a virtual environment to render a template into an incarnation.
 
     As of now the environment is an untouched jinja2 sandboxed environment
     which only has access to the template root directory.
@@ -22,35 +26,34 @@
     # NOTE(TF): add extensions to the loader if necessary.
     env = SandboxedEnvironment(
         loader=loader,
         enable_async=True,
         keep_trailing_newline=True,
         undefined=StrictUndefined,
     )
+    env.filters["ip_add_integer"] = ip_add_integer
     return env
 
 
 async def render_template(
     template_root_dir: Path,
     incarnation_root_dir: Path,
     template_data: TemplateData,
     rendering_filename_exclude_patterns: list[str],
-    logger: BoundLogger,
 ) -> None:
     """Render a template into an incarnation.
 
     As of now a very simplistic approach is used to find and render the files
     and folders in a template.
 
-    :param rendering_filename_exclude_patterns: A list of glob patterns matching files which contents should not be rendered. Can be empty.
+    :param rendering_filename_exclude_patterns: A list of glob patterns matching files which contents should not be
+    rendered. Can be empty.
     """
     if not template_root_dir.is_absolute():
-        raise ValueError(
-            f"template_root_dir must be an absolute path, got {template_root_dir}"
-        )
+        raise ValueError(f"template_root_dir must be an absolute path, got {template_root_dir}")
 
     files_to_render = set(template_root_dir.glob("**/*"))
     for pattern in rendering_filename_exclude_patterns:
         files_to_render -= set(template_root_dir.glob(pattern))
 
     environment = create_template_environment(template_root_dir)
 
@@ -64,34 +67,31 @@
 
     async def _render_template_symlink(template_symlink_path):
         return await render_template_symlink(
             environment,
             template_symlink_path,
             incarnation_root_dir,
             template_data,
-            logger=logger,
         )
 
     async def _render_template_dir(template_dir_path):
         return await render_template_dir(
             environment,
             template_dir_path,
             incarnation_root_dir,
             template_data,
-            logger=logger,
         )
 
     async def _render_template_file(template_file_path, render_content: bool):
         return await render_template_file(
             environment,
             template_file_path,
             incarnation_root_dir,
             template_data,
             render_content=render_content,
-            logger=logger,
         )
 
     for root_dir, dirs, files in os.walk(template_root_dir):
         for d in dirs:
             template_dir_path = Path(root_dir) / d
             if template_dir_path.is_symlink():
                 await _render_template_symlink(template_dir_path)
@@ -111,15 +111,14 @@
 
 async def render_template_file(
     environment: SandboxedEnvironment,
     template_file_path: Path,
     incarnation_root_dir: Path,
     template_data: TemplateData,
     render_content: bool,
-    logger: BoundLogger,
 ) -> Path:
     """Render a template file into an incarnation file.
 
     The template file content and file name are rendered if rendering_enabled is True. Otherwise, rendering of the file
     content is skipped.
     """
     loader: FileSystemLoader = typing.cast(FileSystemLoader, environment.loader)
@@ -154,15 +153,14 @@
 
 
 async def render_template_dir(
     environment: SandboxedEnvironment,
     template_dir_path: Path,
     incarnation_root_dir: Path,
     template_data: TemplateData,
-    logger: BoundLogger,
 ) -> Path:
     """Render a template directory path into an incarnation directory path."""
     loader: FileSystemLoader = typing.cast(FileSystemLoader, environment.loader)
     relative_template_dir_path = template_dir_path.relative_to(loader.searchpath[0])
 
     # get and render template file path
     path_template = environment.from_string(str(relative_template_dir_path))
@@ -178,32 +176,25 @@
 
 
 async def render_template_symlink(
     environment: SandboxedEnvironment,
     template_symlink_path: Path,
     incarnation_root_dir: Path,
     template_data: TemplateData,
-    logger: BoundLogger,
 ) -> Path:
     """Render a template symlink path into an incarnation symlink path."""
     loader: FileSystemLoader = typing.cast(FileSystemLoader, environment.loader)
-    relative_template_symlink_path = template_symlink_path.relative_to(
-        loader.searchpath[0]
-    )
+    relative_template_symlink_path = template_symlink_path.relative_to(loader.searchpath[0])
 
     # get and render template file path
     path_template = environment.from_string(str(relative_template_symlink_path))
     rendered_path = Path(await path_template.render_async(**template_data))
     # get and render template symlink target
-    symlink_target_template = environment.from_string(
-        str(template_symlink_path.readlink())
-    )
-    rendered_symlink_target_path = Path(
-        await symlink_target_template.render_async(**template_data)
-    )
+    symlink_target_template = environment.from_string(str(template_symlink_path.readlink()))
+    rendered_symlink_target_path = Path(await symlink_target_template.render_async(**template_data))
 
     logger.debug(
         "rendering symlink in incarnation",
         source_path=rendered_path,
         target_path=rendered_symlink_target_path,
     )
```

### Comparing `foxops-1.6.5/src/foxops/engine/update.py` & `foxops-2.0.0a4/src/foxops/engine/update.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,153 +1,136 @@
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
-from dictdiffer import diff
-from structlog.stdlib import BoundLogger
-
 from foxops import utils
 from foxops.engine.fvars import merge_template_data_with_fvars
 from foxops.engine.initialization import _initialize_incarnation
-from foxops.engine.models import (
-    IncarnationState,
-    TemplateData,
-    fill_missing_optionals_with_defaults,
-    load_incarnation_state,
-    load_template_config,
-)
-
-
-def get_data_mismatch(
-    desired_template_data: TemplateData,
-    actual_template_data: TemplateData,
-    template_root_dir: Path,
-    logger: BoundLogger,
-) -> list:
-    template_config = load_template_config(template_root_dir / "fengine.yaml")
-
-    # fill defaults in passed data
-    template_data_with_defaults = fill_missing_optionals_with_defaults(
-        provided_template_data=desired_template_data,
-        template_config=template_config,
-        logger=logger,
-    )
-
-    return list(
-        diff(
-            actual_template_data,
-            template_data_with_defaults,
-        )
-    )
+from foxops.engine.models import IncarnationState, TemplateData, load_incarnation_state
+from foxops.engine.patching.git_diff_patch import PatchResult
+from foxops.logger import get_logger
+
+#: Holds the module logger
+logger = get_logger(__name__)
 
 
 async def update_incarnation_from_git_template_repository(
-    template_git_root_dir: Path,
-    update_template_repository: str,
+    template_git_repository: Path,
     update_template_repository_version: str,
     update_template_data: TemplateData,
     incarnation_root_dir: Path,
     diff_patch_func,
-    logger: BoundLogger,
-) -> tuple[IncarnationState, list[Path]]:
+) -> tuple[bool, IncarnationState, PatchResult | None]:
+    if update_template_repository_version.startswith("-"):
+        raise ValueError(
+            f"update_template_repository_version must ba a valid git refspec and "
+            f"not start with a dash (-): {update_template_repository_version}"
+        )
+
     # initialize pristine incarnation from current incarnation state
     current_incarnation_state_path = incarnation_root_dir / ".fengine.yaml"
     current_incarnation_state = load_incarnation_state(current_incarnation_state_path)
 
-    with TemporaryDirectory() as template_root_dir, TemporaryDirectory() as updated_template_root_dir:
+    with TemporaryDirectory() as original_template_root_dir, TemporaryDirectory() as updated_template_root_dir:
         logger.debug(
-            f"creating git worktree from current template repository (version: {current_incarnation_state.template_repository_version_hash}) at {template_root_dir}"
+            f"creating git worktree from current template repository "
+            f"(version: {current_incarnation_state.template_repository_version_hash}) at {original_template_root_dir}"
         )
         await utils.check_call(
             "git",
             "worktree",
             "add",
-            template_root_dir,
+            original_template_root_dir,
             current_incarnation_state.template_repository_version_hash,
-            cwd=template_git_root_dir,
+            cwd=template_git_repository,
         )
         logger.debug(
-            f"creating git worktree from updated template repository (version: {update_template_repository_version}) at {updated_template_root_dir}"
+            f"creating git worktree from updated template repository "
+            f"(version: {update_template_repository_version}) at {updated_template_root_dir}"
         )
         await utils.check_call(
             "git",
             "worktree",
             "add",
             updated_template_root_dir,
             update_template_repository_version,
-            cwd=template_git_root_dir,
+            cwd=template_git_repository,
         )
 
         return await update_incarnation(
-            template_root_dir=Path(template_root_dir),
-            update_template_root_dir=Path(updated_template_root_dir),
-            update_template_repository=update_template_repository,
-            update_template_repository_version=update_template_repository_version,
-            update_template_data=update_template_data,
+            original_template_root_dir=Path(original_template_root_dir),
+            updated_template_root_dir=Path(updated_template_root_dir),
+            updated_template_repository_version=update_template_repository_version,
+            updated_template_data=update_template_data,
             incarnation_root_dir=incarnation_root_dir,
             diff_patch_func=diff_patch_func,
-            logger=logger,
         )
 
 
 async def update_incarnation(
-    template_root_dir: Path,
-    update_template_root_dir: Path,
-    update_template_repository: str,
-    update_template_repository_version: str,
-    update_template_data: TemplateData,
+    original_template_root_dir: Path,
+    updated_template_root_dir: Path,
+    updated_template_repository_version: str,
+    updated_template_data: TemplateData,
     incarnation_root_dir: Path,
     diff_patch_func,
-    logger: BoundLogger,
-) -> tuple[IncarnationState, list[Path]]:
+) -> tuple[bool, IncarnationState, PatchResult | None]:
     """Update an incarnation with a new version of a template."""
     # initialize pristine incarnation from current incarnation state
     current_incarnation_state_path = incarnation_root_dir / ".fengine.yaml"
     current_incarnation_state = load_incarnation_state(current_incarnation_state_path)
 
     with TemporaryDirectory() as tmp_pristine_incarnation_dir, TemporaryDirectory() as tmp_updated_incarnation_dir:
         logger.debug(
             "initialize pristine incarnation from current incarnation state",
-            template_dir=template_root_dir,
+            template_dir=original_template_root_dir,
             incarnation_dir=tmp_pristine_incarnation_dir,
         )
         await _initialize_incarnation(
-            template_root_dir=template_root_dir,
+            template_root_dir=original_template_root_dir,
             template_repository=current_incarnation_state.template_repository,
             template_repository_version=current_incarnation_state.template_repository_version,
             template_data=current_incarnation_state.template_data,
             incarnation_root_dir=Path(tmp_pristine_incarnation_dir),
-            logger=logger,
         )
 
+        # copy over .fengine.yaml from the actual incarnation, just to make sure there are no formatting differences
+        # that would be messing up the patching.
+        #
+        # there were unclear cases where the YAML rending was slightly different (e.g. strings starting on a newline)
+        # during updates, compared to the original incarnation rendering (reason unclear)
+        (Path(tmp_pristine_incarnation_dir) / ".fengine.yaml").write_bytes(current_incarnation_state_path.read_bytes())
+
         logger.debug(
             "initialize new incarnation from update incarnation state",
-            template_dir=update_template_root_dir,
+            template_dir=updated_template_root_dir,
             incarnation_dir=tmp_updated_incarnation_dir,
         )
         updated_incarnation_state = await _initialize_incarnation(
-            template_root_dir=update_template_root_dir,
-            template_repository=update_template_repository,
-            template_repository_version=update_template_repository_version,
+            template_root_dir=updated_template_root_dir,
+            template_repository=current_incarnation_state.template_repository,
+            template_repository_version=updated_template_repository_version,
             template_data=merge_template_data_with_fvars(
-                update_template_data,
+                updated_template_data,
                 incarnation_root_dir,
-                logger,
             ),
             incarnation_root_dir=Path(tmp_updated_incarnation_dir),
-            logger=logger,
         )
 
         # diff pristine and new incarnations
         # apply patch on incarnation to update
         logger.debug(
             "applying patch on pristine and new incarnations",
             diff_a_directory=tmp_pristine_incarnation_dir,
             diff_b_directory=tmp_updated_incarnation_dir,
             patch_directory=incarnation_root_dir,
         )
-        files_with_conflicts = await diff_patch_func(
-            diff_a_directory=tmp_pristine_incarnation_dir,
-            diff_b_directory=tmp_updated_incarnation_dir,
-            patch_directory=incarnation_root_dir,
-            logger=logger,
-        )
-        return updated_incarnation_state, files_with_conflicts
+        if (
+            patch_result := await diff_patch_func(
+                diff_a_directory=tmp_pristine_incarnation_dir,
+                diff_b_directory=tmp_updated_incarnation_dir,
+                patch_directory=incarnation_root_dir,
+            )
+        ) is not None:
+            return True, updated_incarnation_state, patch_result
+        else:
+            logger.debug("Update didn't change anything")
+            return False, updated_incarnation_state, None
```

### Comparing `foxops-1.6.5/src/foxops/utils.py` & `foxops-2.0.0a4/src/foxops/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import subprocess
 
 from .errors import FoxopsError
-from .loggingcfg import get_logger
+from .logger import get_logger
 
 logger = get_logger("utils")
 
 
 class CalledProcessError(subprocess.CalledProcessError, FoxopsError):
     """Error raised when copier fails."""
 
@@ -33,15 +33,14 @@
     -> Setting the timeout to None (default) will allow the child process to take forever.
     """
     proc = await asyncio.create_subprocess_exec(
         program,
         *args,
         stdout=asyncio.subprocess.PIPE,
         stderr=asyncio.subprocess.PIPE,
-        stdin=asyncio.subprocess.PIPE,
         **kwargs,
     )
 
     try:
         await asyncio.wait_for(proc.wait(), timeout=timeout)
     except asyncio.TimeoutError:
         proc.kill()
```

### Comparing `foxops-1.6.5/PKG-INFO` & `foxops-2.0.0a4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 Metadata-Version: 2.1
 Name: foxops
-Version: 1.6.5
+Version: 2.0.0a4
 Summary: Foxops 🦊
+License: Apache-2.0
 Author: Alexander Hungenberg
 Author-email: alexander.hungenberg@roche.com
 Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.0.3,<4.0.0)
-Requires-Dist: aiohttp (>=3.8.0,<4.0.0)
+Requires-Dist: SQLAlchemy[asyncio] (>=2.0.2,<3.0.0)
 Requires-Dist: aiopath (>=0.6.10,<0.7.0)
-Requires-Dist: dictdiffer (>=0.9.0,<0.10.0)
+Requires-Dist: aiosqlite (>=0.19.0,<0.20.0)
+Requires-Dist: alembic[tz] (>=1.8.1,<2.0.0)
+Requires-Dist: asyncpg (>=0.27.0,<0.28.0)
+Requires-Dist: fastapi (>=0.95.2,<0.96.0)
+Requires-Dist: greenlet (>=2.0.0,<3.0.0)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
 Requires-Dist: ruamel.yaml (>=0.17.20,<0.18.0)
-Requires-Dist: structlog (>=21.2.0,<22.0.0)
-Requires-Dist: tenacity (>=8.0.1,<9.0.0)
-Requires-Dist: typer (>=0.4.0,<0.5.0)
+Requires-Dist: structlog (>=23.1.0,<24.0.0)
+Requires-Dist: tenacity (>=8.2.1,<9.0.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Description-Content-Type: text/markdown
 
 # foxops 🦊
 
 A modest templating tool to keep your projects up-to-date.
 
 more coming soon, stay tuned! 🚧
```

