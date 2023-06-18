# Comparing `tmp/webhooklib-0.6.0.tar.gz` & `tmp/webhooklib-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webhooklib-0.6.0.tar", last modified: Sun Jun 18 03:51:32 2023, max compression
+gzip compressed data, was "webhooklib-0.7.0.tar", last modified: Sun Jun 18 07:16:02 2023, max compression
```

## Comparing `webhooklib-0.6.0.tar` & `webhooklib-0.7.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:51:32.192966 webhooklib-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-18 03:51:32.192966 webhooklib-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-18 03:51:17.000000 webhooklib-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-18 03:51:17.000000 webhooklib-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 03:51:32.192966 webhooklib-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:51:32.192966 webhooklib-0.6.0/webhooklib/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-18 03:51:17.000000 webhooklib-0.6.0/webhooklib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-06-18 03:51:17.000000 webhooklib-0.6.0/webhooklib/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-18 03:51:17.000000 webhooklib-0.6.0/webhooklib/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-18 03:51:17.000000 webhooklib-0.6.0/webhooklib/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-18 03:51:17.000000 webhooklib-0.6.0/webhooklib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-18 03:51:17.000000 webhooklib-0.6.0/webhooklib/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-18 03:51:17.000000 webhooklib-0.6.0/webhooklib/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-18 03:51:17.000000 webhooklib-0.6.0/webhooklib/process_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-18 03:51:17.000000 webhooklib-0.6.0/webhooklib/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:51:32.192966 webhooklib-0.6.0/webhooklib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-18 03:51:32.000000 webhooklib-0.6.0/webhooklib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-18 03:51:32.000000 webhooklib-0.6.0/webhooklib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 03:51:32.000000 webhooklib-0.6.0/webhooklib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-18 03:51:32.000000 webhooklib-0.6.0/webhooklib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-18 03:51:32.000000 webhooklib-0.6.0/webhooklib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:16:02.027503 webhooklib-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-18 07:16:02.027503 webhooklib-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-18 07:15:47.000000 webhooklib-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-18 07:15:47.000000 webhooklib-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 07:16:02.027503 webhooklib-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:16:02.027503 webhooklib-0.7.0/webhooklib/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-18 07:15:47.000000 webhooklib-0.7.0/webhooklib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-06-18 07:15:47.000000 webhooklib-0.7.0/webhooklib/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-18 07:15:47.000000 webhooklib-0.7.0/webhooklib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-18 07:15:47.000000 webhooklib-0.7.0/webhooklib/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-18 07:15:47.000000 webhooklib-0.7.0/webhooklib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-18 07:15:47.000000 webhooklib-0.7.0/webhooklib/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-18 07:15:47.000000 webhooklib-0.7.0/webhooklib/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-18 07:15:47.000000 webhooklib-0.7.0/webhooklib/process_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-18 07:15:47.000000 webhooklib-0.7.0/webhooklib/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:16:02.027503 webhooklib-0.7.0/webhooklib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-18 07:16:02.000000 webhooklib-0.7.0/webhooklib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-18 07:16:02.000000 webhooklib-0.7.0/webhooklib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 07:16:02.000000 webhooklib-0.7.0/webhooklib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-18 07:16:02.000000 webhooklib-0.7.0/webhooklib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-18 07:16:02.000000 webhooklib-0.7.0/webhooklib.egg-info/top_level.txt
```

### Comparing `webhooklib-0.6.0/pyproject.toml` & `webhooklib-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [project]
 name = "webhooklib"
-version = "0.6.0"
+version = "0.7.0"
 authors = [
     {name = "Alexander Rodionov", email = "tandav@tandav.me"},
 ]
 description = " tool for remote process call"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
     "fastapi",
     "uvicorn",
     "redis",
     "requests",
+    "pydantic",
 ]
 
 [project.optional-dependencies]
 dev = [
     "bumpver",
     "pre-commit",
     "pytest",
@@ -32,15 +33,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 # ==============================================================================
 
 [tool.bumpver]
-current_version = "v0.6.0"
+current_version = "v0.7.0"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
```

### Comparing `webhooklib-0.6.0/webhooklib/client.py` & `webhooklib-0.7.0/webhooklib/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,44 +2,70 @@
 import sys
 
 import requests
 from redis import Redis
 
 from webhooklib import config
 from webhooklib import exceptions
+from webhooklib.models import Resource
 from webhooklib.models import ShellCommand
 from webhooklib.models import ShellResult
 
 ENV_PREFIX = 'WEBHOOK_ENV_'
 
 
 def red(obj):
     return f'\033[31m{obj}\033[0m'
 
 
+def job_resources(resources_key: str, redis: Redis) -> dict[str, Resource]:
+    pipeline = redis.pipeline()
+    keys = redis.keys(f'{resources_key}:*')
+    names = []
+    for key in keys:
+        pipeline.hgetall(key)
+        _, name = key.rsplit(':', maxsplit=1)
+        names.append(name)
+    resources = pipeline.execute()
+    resources = {name: Resource(**r, key=k, name=name) for r, k, name in zip(resources, keys, names, strict=True)}
+    return resources
+
+
 def wait_message(channel: str, redis: Redis) -> None:
     p = redis.pubsub()
     p.subscribe(channel)
     while not (message := p.get_message(ignore_subscribe_messages=True)):
         pass
     print(message)
 
 
-def wait_max_jobs_quota(redis):
-    n_jobs_key = os.environ['WEBHOOK_N_JOBS_KEY']
-    n_jobs = redis.get(n_jobs_key)
-    max_jobs = int(os.environ.get('WEBHOOK_MAX_JOBS', 10))
-    if n_jobs is None:
-        return
-    if int(n_jobs) <= max_jobs:
-        return
-
-    print(f'{n_jobs=}, {max_jobs=}, waiting...')
-    wait_message(os.environ['WEBHOOK_JOB_STOP_CHANNEL'], redis)
-    wait_max_jobs_quota(redis)
+def wait_resources_semaphore(
+    resources: list[Resource],
+    job_stop_channel: str,
+    redis: Redis,
+) -> None:
+    for resource in resources:
+        if resource.usage_current >= resource.usage_limit:
+            print('resource busy, waiting... :', resource)
+            wait_message(job_stop_channel, redis)
+            wait_resources_semaphore(resources, job_stop_channel, redis)
+            return
+
+
+# def wait_max_jobs_quota(redis):
+#     n_jobs_key = os.environ['WEBHOOK_N_JOBS_KEY']
+#     n_jobs = redis.get(n_jobs_key)
+#     max_jobs = int(os.environ.get('WEBHOOK_MAX_JOBS', 10))
+#     if n_jobs is None:
+#         return
+#     if int(n_jobs) <= max_jobs:
+#         return
+#     print(f'{n_jobs=}, {max_jobs=}, waiting...')
+#     wait_message(os.environ['WEBHOOK_JOB_STOP_CHANNEL'], redis)
+#     wait_max_jobs_quota(redis)
 
 
 def read_rest_logs(redis: Redis, stdout_key: str, stderr_key: str) -> None:
     pipeline = redis.pipeline()
     pipeline.lrange(stdout_key, 1, -1)
     pipeline.lrange(stderr_key, 1, -1)
     stdout, stderr = pipeline.execute()
@@ -47,16 +73,21 @@
         print(line, end='')
     for line in stderr:
         print(red(line), end='')
 
 
 def main(line_buffer_size: int = 100):
     redis = Redis.from_url(os.environ['REDIS_URL'], decode_responses=True)
-    wait_max_jobs_quota(redis)
-    redis.incr(os.environ['WEBHOOK_N_JOBS_KEY'])
+    resources = job_resources(os.environ['WEBHOOK_RESOURCES_KEY'], redis)
+    del resources['pipeline']
+    wait_resources_semaphore(list(resources.values()), os.environ['WEBHOOK_JOB_STOP_CHANNEL'], redis)
+
+    # wait_max_jobs_quota(redis)
+    # redis.incr(os.environ['WEBHOOK_N_JOBS_KEY'])
+    redis.hincrby(resources['job'].key, 'usage_current')
 
     url = os.environ['WEBHOOK_URL']
     payload = {
         'cmd': sys.argv[1:],
     }
     if 'WEBHOOK_CWD' in os.environ:
         payload['cwd'] = os.environ['WEBHOOK_CWD']
@@ -123,12 +154,13 @@
     # _, message = redis.brpop(key)
     # result = ShellResult.parse_raw(message)
     result = ShellResult.parse_raw(result)
     # result.pprint()
     if result.returncode != 0:
         raise exceptions.ProcessResultError
     redis.delete(key)
-    redis.decr(os.environ['WEBHOOK_N_JOBS_KEY'])
+    # redis.decr(os.environ['WEBHOOK_N_JOBS_KEY'])
+    redis.hincrby(resources['job'].key, 'usage_current', -1)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `webhooklib-0.6.0/webhooklib/pipeline.py` & `webhooklib-0.7.0/webhooklib/pipeline.py`

 * *Files identical despite different names*

### Comparing `webhooklib-0.6.0/webhooklib/process_wrapper.py` & `webhooklib-0.7.0/webhooklib/process_wrapper.py`

 * *Files identical despite different names*

### Comparing `webhooklib-0.6.0/webhooklib/server.py` & `webhooklib-0.7.0/webhooklib/server.py`

 * *Files identical despite different names*

