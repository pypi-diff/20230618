# Comparing `tmp/miniwdl-omics-run-0.1.0.tar.gz` & `tmp/miniwdl-omics-run-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniwdl-omics-run-0.1.0.tar", last modified: Tue Apr  4 03:54:13 2023, max compression
+gzip compressed data, was "miniwdl-omics-run-0.2.0.tar", last modified: Sun Jun 18 00:32:03 2023, max compression
```

## Comparing `miniwdl-omics-run-0.1.0.tar` & `miniwdl-omics-run-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-04-04 03:54:13.551741 miniwdl-omics-run-0.1.0/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     1830 2023-04-03 05:58:09.000000 miniwdl-omics-run-0.1.0/.gitignore
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      203 2023-04-03 05:53:41.000000 miniwdl-omics-run-0.1.0/.pre-commit-config.yaml
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     1056 2023-04-03 05:55:43.000000 miniwdl-omics-run-0.1.0/LICENSE
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     5316 2023-04-04 03:54:13.551741 miniwdl-omics-run-0.1.0/PKG-INFO
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     4981 2023-04-04 03:47:14.000000 miniwdl-omics-run-0.1.0/README.md
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-04-04 03:54:13.551741 miniwdl-omics-run-0.1.0/miniwdl_omics_run/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)       47 2023-04-03 05:53:41.000000 miniwdl-omics-run-0.1.0/miniwdl_omics_run/__init__.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     9258 2023-04-03 08:49:28.000000 miniwdl-omics-run-0.1.0/miniwdl_omics_run/__main__.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      160 2023-04-04 03:54:13.000000 miniwdl-omics-run-0.1.0/miniwdl_omics_run/_version.py
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-04-04 03:54:13.551741 miniwdl-omics-run-0.1.0/miniwdl_omics_run.egg-info/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     5316 2023-04-04 03:54:13.000000 miniwdl-omics-run-0.1.0/miniwdl_omics_run.egg-info/PKG-INFO
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      446 2023-04-04 03:54:13.000000 miniwdl-omics-run-0.1.0/miniwdl_omics_run.egg-info/SOURCES.txt
--rw-rw-r--   0 mlin      (1000) mlin      (1000)        1 2023-04-04 03:54:13.000000 miniwdl-omics-run-0.1.0/miniwdl_omics_run.egg-info/dependency_links.txt
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      104 2023-04-04 03:54:13.000000 miniwdl-omics-run-0.1.0/miniwdl_omics_run.egg-info/entry_points.txt
--rw-rw-r--   0 mlin      (1000) mlin      (1000)       85 2023-04-04 03:54:13.000000 miniwdl-omics-run-0.1.0/miniwdl_omics_run.egg-info/requires.txt
--rw-rw-r--   0 mlin      (1000) mlin      (1000)       18 2023-04-04 03:54:13.000000 miniwdl-omics-run-0.1.0/miniwdl_omics_run.egg-info/top_level.txt
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      927 2023-04-04 03:16:29.000000 miniwdl-omics-run-0.1.0/pyproject.toml
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      118 2023-04-03 18:39:13.000000 miniwdl-omics-run-0.1.0/release.sh
--rw-rw-r--   0 mlin      (1000) mlin      (1000)       38 2023-04-04 03:54:13.551741 miniwdl-omics-run-0.1.0/setup.cfg
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-04-04 03:54:13.551741 miniwdl-omics-run-0.1.0/test/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      764 2023-04-03 05:59:03.000000 miniwdl-omics-run-0.1.0/test/TestFlow.wdl
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-06-18 00:32:03.931066 miniwdl-omics-run-0.2.0/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     1830 2023-04-03 05:58:09.000000 miniwdl-omics-run-0.2.0/.gitignore
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      203 2023-04-03 05:53:41.000000 miniwdl-omics-run-0.2.0/.pre-commit-config.yaml
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     1056 2023-04-03 05:55:43.000000 miniwdl-omics-run-0.2.0/LICENSE
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     5316 2023-06-18 00:32:03.927066 miniwdl-omics-run-0.2.0/PKG-INFO
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     4981 2023-04-04 03:47:14.000000 miniwdl-omics-run-0.2.0/README.md
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-06-18 00:32:03.927066 miniwdl-omics-run-0.2.0/miniwdl_omics_run/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)       47 2023-04-03 05:53:41.000000 miniwdl-omics-run-0.2.0/miniwdl_omics_run/__init__.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    10070 2023-06-18 00:04:27.000000 miniwdl-omics-run-0.2.0/miniwdl_omics_run/__main__.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      160 2023-06-18 00:32:03.000000 miniwdl-omics-run-0.2.0/miniwdl_omics_run/_version.py
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-06-18 00:32:03.927066 miniwdl-omics-run-0.2.0/miniwdl_omics_run.egg-info/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     5316 2023-06-18 00:32:03.000000 miniwdl-omics-run-0.2.0/miniwdl_omics_run.egg-info/PKG-INFO
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      446 2023-06-18 00:32:03.000000 miniwdl-omics-run-0.2.0/miniwdl_omics_run.egg-info/SOURCES.txt
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)        1 2023-06-18 00:32:03.000000 miniwdl-omics-run-0.2.0/miniwdl_omics_run.egg-info/dependency_links.txt
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      104 2023-06-18 00:32:03.000000 miniwdl-omics-run-0.2.0/miniwdl_omics_run.egg-info/entry_points.txt
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)       85 2023-06-18 00:32:03.000000 miniwdl-omics-run-0.2.0/miniwdl_omics_run.egg-info/requires.txt
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)       18 2023-06-18 00:32:03.000000 miniwdl-omics-run-0.2.0/miniwdl_omics_run.egg-info/top_level.txt
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      927 2023-04-04 03:16:29.000000 miniwdl-omics-run-0.2.0/pyproject.toml
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      118 2023-04-03 18:39:13.000000 miniwdl-omics-run-0.2.0/release.sh
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)       38 2023-06-18 00:32:03.931066 miniwdl-omics-run-0.2.0/setup.cfg
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-06-18 00:32:03.927066 miniwdl-omics-run-0.2.0/test/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      764 2023-04-03 05:59:03.000000 miniwdl-omics-run-0.2.0/test/TestFlow.wdl
```

### Comparing `miniwdl-omics-run-0.1.0/.gitignore` & `miniwdl-omics-run-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `miniwdl-omics-run-0.1.0/LICENSE` & `miniwdl-omics-run-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `miniwdl-omics-run-0.1.0/PKG-INFO` & `miniwdl-omics-run-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniwdl-omics-run
-Version: 0.1.0
+Version: 0.2.0
 Summary: WDL launcher for Amazon Omics
 Project-URL: repository, https://github.com/miniwdl-ext/miniwdl-omics-run.git
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `miniwdl-omics-run-0.1.0/README.md` & `miniwdl-omics-run-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `miniwdl-omics-run-0.1.0/miniwdl_omics_run/__main__.py` & `miniwdl-omics-run-0.2.0/miniwdl_omics_run/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 import logging
 import os
 import subprocess
 import sys
 import tempfile
 import time
+import uuid
 from contextlib import ExitStack
 
 import boto3
 import botocore.config
 import WDL
 import WDL.CLI
 from WDL._util import configure_logger
@@ -69,15 +70,17 @@
         # start run
         res = omics.start_run(
             outputUri=args.output_uri,
             parameters=input_dict,
             roleArn=args.role_arn,
             workflowId=workflow_id,
             workflowType="PRIVATE",
-            # TODO: name, priority, runGroupId, storageCapacity (from args)
+            logLevel="ALL",
+            requestId=str(uuid.uuid4()),
+            **start_run_options(args),
         )
 
     run_id = res["id"]
     aws_region = omics.meta.region_name
     run_info = {
         "workflowId": workflow_id,
         "runId": run_id,
@@ -150,21 +153,43 @@
         help="ARN of IAM role",
         required=True,
     )
     group.add_argument(
         "--output-uri",
         metavar="OUTPUT_S3_URI",
         type=check_s3_uri_arg,
-        help="Base S3 URI for workflow outputs",
+        help="S3 URI prefix for workflow outputs",
         required=True,
     )
+    group.add_argument("--name", type=str, help="Name", default=None)
+    group.add_argument("--priority", type=int, help="Priority (integer)", default=None)
+    group.add_argument("--run-group-id", type=str, help="Run group ID", default=None)
+    group.add_argument(
+        "--storage-capacity",
+        type=int,
+        help="Storage capacity in gigabytes",
+        default=None,
+    )
 
     return parser
 
 
+def start_run_options(args):
+    ans = {}
+    if args.name is not None:
+        ans["name"] = args.name
+    if args.priority is not None:
+        ans["priority"] = args.priority
+    if args.run_group_id is not None:
+        ans["runGroupId"] = args.run_group_id
+    if args.storage_capacity is not None:
+        ans["storageCapacity"] = args.storage_capacity
+    return ans
+
+
 class VersionAction(argparse.Action):
     def __init__(self, option_strings, dest, nargs=None, **kwargs):
         super().__init__(option_strings, dest, nargs=0, **kwargs)
 
     def __call__(self, parser, namespace, values, option_string=None):
         print(f"miniwdl-omics-run v{__version__}")
         subprocess.call(["miniwdl", "--version"])
```

### Comparing `miniwdl-omics-run-0.1.0/miniwdl_omics_run.egg-info/PKG-INFO` & `miniwdl-omics-run-0.2.0/miniwdl_omics_run.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniwdl-omics-run
-Version: 0.1.0
+Version: 0.2.0
 Summary: WDL launcher for Amazon Omics
 Project-URL: repository, https://github.com/miniwdl-ext/miniwdl-omics-run.git
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `miniwdl-omics-run-0.1.0/pyproject.toml` & `miniwdl-omics-run-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `miniwdl-omics-run-0.1.0/test/TestFlow.wdl` & `miniwdl-omics-run-0.2.0/test/TestFlow.wdl`

 * *Files identical despite different names*

