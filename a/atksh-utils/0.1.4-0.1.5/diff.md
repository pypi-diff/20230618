# Comparing `tmp/atksh-utils-0.1.4.tar.gz` & `tmp/atksh-utils-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atksh-utils-0.1.4.tar", last modified: Sun Jun 18 02:54:33 2023, max compression
+gzip compressed data, was "atksh-utils-0.1.5.tar", last modified: Sun Jun 18 03:01:26 2023, max compression
```

## Comparing `atksh-utils-0.1.4.tar` & `atksh-utils-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:54:33.903774 atksh-utils-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:54:33.903774 atksh-utils-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:54:33.903774 atksh-utils-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-18 02:54:23.000000 atksh-utils-0.1.4/.github/workflows/publish_to_pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-18 02:54:23.000000 atksh-utils-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-18 02:54:23.000000 atksh-utils-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-18 02:54:23.000000 atksh-utils-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-18 02:54:33.903774 atksh-utils-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-18 02:54:23.000000 atksh-utils-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-18 02:54:23.000000 atksh-utils-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-18 02:54:33.907774 atksh-utils-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:54:33.903774 atksh-utils-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:54:33.903774 atksh-utils-0.1.4/src/atksh_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 02:54:23.000000 atksh-utils-0.1.4/src/atksh_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:54:33.903774 atksh-utils-0.1.4/src/atksh_utils/openai/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-18 02:54:23.000000 atksh-utils-0.1.4/src/atksh_utils/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9489 2023-06-18 02:54:23.000000 atksh-utils-0.1.4/src/atksh_utils/openai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-18 02:54:23.000000 atksh-utils-0.1.4/src/atksh_utils/openai/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-18 02:54:23.000000 atksh-utils-0.1.4/src/atksh_utils/openai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 02:54:33.000000 atksh-utils-0.1.4/src/atksh_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:54:33.903774 atksh-utils-0.1.4/src/atksh_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-18 02:54:33.000000 atksh-utils-0.1.4/src/atksh_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-18 02:54:33.000000 atksh-utils-0.1.4/src/atksh_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:54:33.000000 atksh-utils-0.1.4/src/atksh_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-18 02:54:33.000000 atksh-utils-0.1.4/src/atksh_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 02:54:33.000000 atksh-utils-0.1.4/src/atksh_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:54:33.903774 atksh-utils-0.1.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:54:33.903774 atksh-utils-0.1.4/tests/openai/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-18 02:54:23.000000 atksh-utils-0.1.4/tests/openai/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-18 02:54:23.000000 atksh-utils-0.1.4/tests/openai/test_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:01:26.255397 atksh-utils-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:01:26.251397 atksh-utils-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:01:26.255397 atksh-utils-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-18 03:01:16.000000 atksh-utils-0.1.5/.github/workflows/publish_to_pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-18 03:01:16.000000 atksh-utils-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-18 03:01:16.000000 atksh-utils-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-18 03:01:16.000000 atksh-utils-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-18 03:01:26.255397 atksh-utils-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-18 03:01:16.000000 atksh-utils-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-18 03:01:16.000000 atksh-utils-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-18 03:01:26.255397 atksh-utils-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:01:26.251397 atksh-utils-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:01:26.255397 atksh-utils-0.1.5/src/atksh_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 03:01:16.000000 atksh-utils-0.1.5/src/atksh_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:01:26.255397 atksh-utils-0.1.5/src/atksh_utils/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-18 03:01:16.000000 atksh-utils-0.1.5/src/atksh_utils/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9654 2023-06-18 03:01:16.000000 atksh-utils-0.1.5/src/atksh_utils/openai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-18 03:01:16.000000 atksh-utils-0.1.5/src/atksh_utils/openai/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-18 03:01:16.000000 atksh-utils-0.1.5/src/atksh_utils/openai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 03:01:26.000000 atksh-utils-0.1.5/src/atksh_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:01:26.255397 atksh-utils-0.1.5/src/atksh_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-18 03:01:26.000000 atksh-utils-0.1.5/src/atksh_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-18 03:01:26.000000 atksh-utils-0.1.5/src/atksh_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 03:01:26.000000 atksh-utils-0.1.5/src/atksh_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-18 03:01:26.000000 atksh-utils-0.1.5/src/atksh_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 03:01:26.000000 atksh-utils-0.1.5/src/atksh_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:01:26.255397 atksh-utils-0.1.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:01:26.255397 atksh-utils-0.1.5/tests/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-18 03:01:16.000000 atksh-utils-0.1.5/tests/openai/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-18 03:01:16.000000 atksh-utils-0.1.5/tests/openai/test_functional.py
```

### Comparing `atksh-utils-0.1.4/.github/workflows/publish_to_pypi.yaml` & `atksh-utils-0.1.5/.github/workflows/publish_to_pypi.yaml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.4/.gitignore` & `atksh-utils-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.4/LICENSE` & `atksh-utils-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.4/PKG-INFO` & `atksh-utils-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.1.4
+Version: 0.1.5
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.1.4/README.md` & `atksh-utils-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.4/pyproject.toml` & `atksh-utils-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.4/src/atksh_utils/openai/api.py` & `atksh-utils-0.1.5/src/atksh_utils/openai/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,16 +42,18 @@
         self.model_name = model_name
         self.temperature = temperature
         self.top_p = top_p
         self.functions: List[FunctionWrapper] = []
 
         self.system_prompt = generate_prompt()
 
-    def make_child(self) -> "OpenAI":
-        return OpenAI(self.api_key, self.model_name, self.temperature, self.top_p, self.openai)
+    def make_child(self, model_name=None) -> "OpenAI":
+        if model_name is None:
+            model_name = self.model_name
+        return OpenAI(self.api_key, model_name, self.temperature, self.top_p, self.openai)
 
     def set_function(self, func):
         """
         Adds a function to the list of functions that can be called by the OpenAI API.
 
         Args:
             func: The function to add.
@@ -181,19 +183,19 @@
         """
         messages = self.call(user_prompt, stream_callback=stream_callback)
         return messages, messages[-1]["content"]
 
     def __repr__(self) -> str:
         return f"OpenAI(model_name={self.model_name}, temperature={self.temperature}, top_p={self.top_p})"
 
-    def _create_react_functions(self, stream_callback=None):
+    def _create_react_functions(self, stream_callback=None, model_name=None):
         """Creates three OpenAI agents"""
-        analyzer = self.make_child()
-        planner = self.make_child()
-        actor = self.make_child()
+        analyzer = self.make_child(model_name)
+        planner = self.make_child(model_name)
+        actor = self.make_child(model_name)
         analyzer.set_system_prompt(generate_react_prompt(turn="analyze"))
         planner.set_system_prompt(generate_react_prompt(turn="plan"))
         actor.set_system_prompt(generate_react_prompt(turn="act"))
 
         def analyze(description):
             """Analyze the description. The output format is like `goal state: xxx, current state: xxx, summary: xxx`.
 
@@ -234,13 +236,13 @@
             return actor(
                 f"Current state: {current_state}, Action: {action}, Summary: {summary}",
                 stream_callback=stream_callback,
             )[1]
 
         return analyze, plan, act
 
-    def set_react_functions(self, stream_callback=None):
+    def set_react_functions(self, stream_callback=None, model_name=None):
         """Adds three OpenAI agents"""
-        analyzer, planner, actor = self._create_react_functions(stream_callback)
+        analyzer, planner, actor = self._create_react_functions(stream_callback, model_name=None)
         self.set_function(analyzer)
         self.set_function(planner)
         self.set_function(actor)
```

### Comparing `atksh-utils-0.1.4/src/atksh_utils/openai/functional.py` & `atksh-utils-0.1.5/src/atksh_utils/openai/functional.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.4/src/atksh_utils/openai/prompt.py` & `atksh-utils-0.1.5/src/atksh_utils/openai/prompt.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.4/src/atksh_utils.egg-info/PKG-INFO` & `atksh-utils-0.1.5/src/atksh_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.1.4
+Version: 0.1.5
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.1.4/src/atksh_utils.egg-info/SOURCES.txt` & `atksh-utils-0.1.5/src/atksh_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.4/tests/openai/test_api.py` & `atksh-utils-0.1.5/tests/openai/test_api.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.4/tests/openai/test_functional.py` & `atksh-utils-0.1.5/tests/openai/test_functional.py`

 * *Files identical despite different names*

