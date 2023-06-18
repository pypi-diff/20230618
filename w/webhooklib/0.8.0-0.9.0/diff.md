# Comparing `tmp/webhooklib-0.8.0.tar.gz` & `tmp/webhooklib-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webhooklib-0.8.0.tar", last modified: Sun Jun 18 07:36:35 2023, max compression
+gzip compressed data, was "webhooklib-0.9.0.tar", last modified: Sun Jun 18 08:08:24 2023, max compression
```

## Comparing `webhooklib-0.8.0.tar` & `webhooklib-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:36:35.241902 webhooklib-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-18 07:36:35.241902 webhooklib-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-18 07:36:18.000000 webhooklib-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-18 07:36:18.000000 webhooklib-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 07:36:35.241902 webhooklib-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:36:35.241902 webhooklib-0.8.0/webhooklib/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-18 07:36:18.000000 webhooklib-0.8.0/webhooklib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-06-18 07:36:18.000000 webhooklib-0.8.0/webhooklib/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-18 07:36:18.000000 webhooklib-0.8.0/webhooklib/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-18 07:36:18.000000 webhooklib-0.8.0/webhooklib/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-18 07:36:18.000000 webhooklib-0.8.0/webhooklib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-18 07:36:18.000000 webhooklib-0.8.0/webhooklib/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-18 07:36:18.000000 webhooklib-0.8.0/webhooklib/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-18 07:36:18.000000 webhooklib-0.8.0/webhooklib/process_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-18 07:36:18.000000 webhooklib-0.8.0/webhooklib/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:36:35.241902 webhooklib-0.8.0/webhooklib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-18 07:36:35.000000 webhooklib-0.8.0/webhooklib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-18 07:36:35.000000 webhooklib-0.8.0/webhooklib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 07:36:35.000000 webhooklib-0.8.0/webhooklib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-18 07:36:35.000000 webhooklib-0.8.0/webhooklib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-18 07:36:35.000000 webhooklib-0.8.0/webhooklib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:08:24.520145 webhooklib-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-18 08:08:24.520145 webhooklib-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-18 08:08:05.000000 webhooklib-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-18 08:08:05.000000 webhooklib-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 08:08:24.520145 webhooklib-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:08:24.520145 webhooklib-0.9.0/webhooklib/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-18 08:08:05.000000 webhooklib-0.9.0/webhooklib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-06-18 08:08:05.000000 webhooklib-0.9.0/webhooklib/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-18 08:08:05.000000 webhooklib-0.9.0/webhooklib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-18 08:08:05.000000 webhooklib-0.9.0/webhooklib/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-18 08:08:05.000000 webhooklib-0.9.0/webhooklib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-18 08:08:05.000000 webhooklib-0.9.0/webhooklib/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-18 08:08:05.000000 webhooklib-0.9.0/webhooklib/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-18 08:08:05.000000 webhooklib-0.9.0/webhooklib/process_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-18 08:08:05.000000 webhooklib-0.9.0/webhooklib/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:08:24.520145 webhooklib-0.9.0/webhooklib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-18 08:08:24.000000 webhooklib-0.9.0/webhooklib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-18 08:08:24.000000 webhooklib-0.9.0/webhooklib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 08:08:24.000000 webhooklib-0.9.0/webhooklib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-18 08:08:24.000000 webhooklib-0.9.0/webhooklib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-18 08:08:24.000000 webhooklib-0.9.0/webhooklib.egg-info/top_level.txt
```

### Comparing `webhooklib-0.8.0/pyproject.toml` & `webhooklib-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "webhooklib"
-version = "0.8.0"
+version = "0.9.0"
 authors = [
     {name = "Alexander Rodionov", email = "tandav@tandav.me"},
 ]
 description = " tool for remote process call"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
@@ -33,15 +33,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 # ==============================================================================
 
 [tool.bumpver]
-current_version = "v0.8.0"
+current_version = "v0.9.0"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
```

### Comparing `webhooklib-0.8.0/webhooklib/client.py` & `webhooklib-0.9.0/webhooklib/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,25 +52,38 @@
     p = redis.pubsub()
     p.subscribe(channel)
     while not (message := p.get_message(ignore_subscribe_messages=True)):
         pass
     print(message)
 
 
+def wait_resource_semaphore(
+    resource: Resource,
+    job_stop_channel: str,
+    redis: Redis,
+) -> None:
+    if resource.usage_current < resource.usage_limit:
+        return
+    print('resource busy, waiting... :', resource)
+    wait_message(job_stop_channel, redis)
+    wait_resources_semaphore(resource, job_stop_channel, redis)
+
+
 def wait_resources_semaphore(
     resources: list[Resource],
     job_stop_channel: str,
     redis: Redis,
 ) -> None:
     for resource in resources:
-        if resource.usage_current >= resource.usage_limit:
-            print('resource busy, waiting... :', resource)
-            wait_message(job_stop_channel, redis)
-            wait_resources_semaphore(resources, job_stop_channel, redis)
-            return
+        wait_resource_semaphore(resource, job_stop_channel, redis)
+        # if resource.usage_current >= resource.usage_limit:
+        #     print('resource busy, waiting... :', resource)
+        #     wait_message(job_stop_channel, redis)
+        #     wait_resources_semaphore(resources, job_stop_channel, redis)
+        #     return
 
 
 # def wait_max_jobs_quota(redis):
 #     n_jobs_key = os.environ['WEBHOOK_N_JOBS_KEY']
 #     n_jobs = redis.get(n_jobs_key)
 #     max_jobs = int(os.environ.get('WEBHOOK_MAX_JOBS', 10))
 #     if n_jobs is None:
```

### Comparing `webhooklib-0.8.0/webhooklib/models.py` & `webhooklib-0.9.0/webhooklib/models.py`

 * *Files identical despite different names*

### Comparing `webhooklib-0.8.0/webhooklib/pipeline.py` & `webhooklib-0.9.0/webhooklib/pipeline.py`

 * *Files identical despite different names*

### Comparing `webhooklib-0.8.0/webhooklib/process_wrapper.py` & `webhooklib-0.9.0/webhooklib/process_wrapper.py`

 * *Files identical despite different names*

### Comparing `webhooklib-0.8.0/webhooklib/server.py` & `webhooklib-0.9.0/webhooklib/server.py`

 * *Files identical despite different names*

