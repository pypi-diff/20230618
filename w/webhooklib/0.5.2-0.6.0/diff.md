# Comparing `tmp/webhooklib-0.5.2.tar.gz` & `tmp/webhooklib-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webhooklib-0.5.2.tar", last modified: Sat Jun 17 19:12:27 2023, max compression
+gzip compressed data, was "webhooklib-0.6.0.tar", last modified: Sun Jun 18 03:51:32 2023, max compression
```

## Comparing `webhooklib-0.5.2.tar` & `webhooklib-0.6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:12:27.241637 webhooklib-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-17 19:12:27.241637 webhooklib-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-17 19:12:12.000000 webhooklib-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-06-17 19:12:12.000000 webhooklib-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 19:12:27.241637 webhooklib-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:12:27.241637 webhooklib-0.5.2/webhooklib/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-17 19:12:12.000000 webhooklib-0.5.2/webhooklib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-06-17 19:12:12.000000 webhooklib-0.5.2/webhooklib/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-17 19:12:12.000000 webhooklib-0.5.2/webhooklib/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-17 19:12:12.000000 webhooklib-0.5.2/webhooklib/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-17 19:12:12.000000 webhooklib-0.5.2/webhooklib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-17 19:12:12.000000 webhooklib-0.5.2/webhooklib/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-17 19:12:12.000000 webhooklib-0.5.2/webhooklib/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-17 19:12:12.000000 webhooklib-0.5.2/webhooklib/process_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-17 19:12:12.000000 webhooklib-0.5.2/webhooklib/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:12:27.241637 webhooklib-0.5.2/webhooklib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-17 19:12:27.000000 webhooklib-0.5.2/webhooklib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-17 19:12:27.000000 webhooklib-0.5.2/webhooklib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 19:12:27.000000 webhooklib-0.5.2/webhooklib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-17 19:12:27.000000 webhooklib-0.5.2/webhooklib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-17 19:12:27.000000 webhooklib-0.5.2/webhooklib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:51:32.192966 webhooklib-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-18 03:51:32.192966 webhooklib-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-18 03:51:17.000000 webhooklib-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-18 03:51:17.000000 webhooklib-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 03:51:32.192966 webhooklib-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:51:32.192966 webhooklib-0.6.0/webhooklib/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-18 03:51:17.000000 webhooklib-0.6.0/webhooklib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-06-18 03:51:17.000000 webhooklib-0.6.0/webhooklib/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-18 03:51:17.000000 webhooklib-0.6.0/webhooklib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-18 03:51:17.000000 webhooklib-0.6.0/webhooklib/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-18 03:51:17.000000 webhooklib-0.6.0/webhooklib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-18 03:51:17.000000 webhooklib-0.6.0/webhooklib/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-18 03:51:17.000000 webhooklib-0.6.0/webhooklib/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-18 03:51:17.000000 webhooklib-0.6.0/webhooklib/process_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-18 03:51:17.000000 webhooklib-0.6.0/webhooklib/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:51:32.192966 webhooklib-0.6.0/webhooklib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-18 03:51:32.000000 webhooklib-0.6.0/webhooklib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-18 03:51:32.000000 webhooklib-0.6.0/webhooklib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 03:51:32.000000 webhooklib-0.6.0/webhooklib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-18 03:51:32.000000 webhooklib-0.6.0/webhooklib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-18 03:51:32.000000 webhooklib-0.6.0/webhooklib.egg-info/top_level.txt
```

### Comparing `webhooklib-0.5.2/pyproject.toml` & `webhooklib-0.6.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "webhooklib"
-version = "0.5.2"
+version = "0.6.0"
 authors = [
     {name = "Alexander Rodionov", email = "tandav@tandav.me"},
 ]
 description = " tool for remote process call"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
@@ -32,15 +32,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 # ==============================================================================
 
 [tool.bumpver]
-current_version = "v0.5.2"
+current_version = "v0.6.0"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
@@ -71,14 +71,16 @@
     "ARG005", # Unused lambda argument
     "PTH123", # `open()` should be replaced by `Path.open()`
     "N812", # lowercase imported as non lowercase
     "T201",
     "S113",
     "A003",
     "G004",
+    "ERA001", # commented-out-code
+    "C901", # function is too complex
 ]
 
 [tool.ruff.per-file-ignores]
 "examples/*" = ["INP001"]
 "tests/*" = ["S101", "PLR2004"]
 
 [tool.ruff.isort]
@@ -101,14 +103,16 @@
     "multiple-statements",
     "line-too-long",
     "unspecified-encoding",
     "wildcard-import",
     "unused-wildcard-import",
     "keyword-arg-before-vararg",
     "too-few-public-methods",
+    "too-many-locals",
+    "fixme",
     "consider-using-with",
     "import-error",
     "logging-fstring-interpolation",
 ]
 
 [tool.pylint-per-file-ignores]
 "server.py" = "import-error"
```

### Comparing `webhooklib-0.5.2/webhooklib/models.py` & `webhooklib-0.6.0/webhooklib/models.py`

 * *Files identical despite different names*

### Comparing `webhooklib-0.5.2/webhooklib/pipeline.py` & `webhooklib-0.6.0/webhooklib/pipeline.py`

 * *Files identical despite different names*

### Comparing `webhooklib-0.5.2/webhooklib/process_wrapper.py` & `webhooklib-0.6.0/webhooklib/process_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import logging
-import subprocess
 import selectors
-import time
-import sys
 import signal
+import subprocess
+import time
+
 from redis import Redis
 
 from webhooklib import config
 from webhooklib.models import ShellCommand
 from webhooklib.models import ShellResult
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
+
 def read_rest_of_lines(p, redis, stdout_key, stderr_key) -> None:
     for line in p.stdout:
-        redis.lpush(stdout_key, line)
+        redis.lpush(stdout_key, f'[STDOUT] {line}')
     for line in p.stderr:
-        redis.lpush(stderr_key, line)
+        redis.lpush(stderr_key, f'[STDERR] {line}')
 
 
 def non_blocking_process(command: ShellCommand, redis: Redis):
     print('non_blocking_process:', command)
-    
+
     stdout_key = f'{config.LOGS}:{command.id}:stdout'
     stderr_key = f'{config.LOGS}:{command.id}:stderr'
 
     # create empty line to set ttl before logs are written
     pipeline = redis.pipeline()
     pipeline.lpush(stdout_key, '')
-    pipeline.lpush(stderr_key, '') 
+    pipeline.lpush(stderr_key, '')
     pipeline.expire(stdout_key, config.LOGS_TTL)
     pipeline.expire(stderr_key, config.LOGS_TTL)
     pipeline.execute()
 
     t_start = time.time()
     p = subprocess.Popen(
         command.cmd,
@@ -44,44 +45,45 @@
         text=True,
     )
     logger.info('Popen done')
 
     # Create the default selector
     sel = selectors.DefaultSelector()
 
-    # Register the subprocess's stdout and stderr for monitoring 
+    # Register the subprocess's stdout and stderr for monitoring
     # route them to current process's stdout and stderr
     sel.register(p.stdout, selectors.EVENT_READ, data='stdout')
     sel.register(p.stderr, selectors.EVENT_READ, data='stderr')
 
     while p.poll() is None:  # While the process is still running...
         if command.timeout is not None and time.time() - t_start > command.timeout:
             print('timeout: killing the proccess')
             p.kill()
             read_rest_of_lines(p, redis, stdout_key)
             return ShellResult(
                 status='killed by timeout',
                 returncode=signal.SIGKILL,
-                stdout=redis.lrange(stdout_key, 0, -1),
-                stderr=redis.lrange(stderr_key, 0, -1),
+                stdout='\n'.join(redis.lrange(stdout_key, 0, -1)),
+                stderr='\n'.join(redis.lrange(stderr_key, 0, -1)),
             )
         for key, _ in sel.select():  # Wait until stdout or stderr has data
             line = key.fileobj.readline()  # Read a line from the pipe
             if line:  # If the line is not empty...
                 if key.data == 'stdout':
-                    redis.lpush(stdout_key, line)
+                    redis.lpush(stdout_key, f'[STDOUT] {line}')
                 elif key.data == 'stderr':
-                    redis.lpush(stderr_key, line)
+                    redis.lpush(stderr_key, f'[STDERR] {line}')
     return ShellResult(
         status='success',
         returncode=p.returncode,
-        stdout=redis.lrange(stdout_key, 0, -1),
-        stderr=redis.lrange(stderr_key, 0, -1),
+        stdout='\n'.join(redis.lrange(stdout_key, 0, -1)),
+        stderr='\n'.join(redis.lrange(stderr_key, 0, -1)),
     )
 
+
 def run_subprocess(
     command: ShellCommand,
     redis: Redis,
 ) -> None:
     logger.info('start')
     result = non_blocking_process(command, redis)
     # p = subprocess.Popen(
```

### Comparing `webhooklib-0.5.2/webhooklib/server.py` & `webhooklib-0.6.0/webhooklib/server.py`

 * *Files identical despite different names*

