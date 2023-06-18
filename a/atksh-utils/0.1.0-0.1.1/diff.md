# Comparing `tmp/atksh-utils-0.1.0.tar.gz` & `tmp/atksh-utils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atksh-utils-0.1.0.tar", last modified: Sun Jun 18 01:41:51 2023, max compression
+gzip compressed data, was "atksh-utils-0.1.1.tar", last modified: Sun Jun 18 01:57:44 2023, max compression
```

## Comparing `atksh-utils-0.1.0.tar` & `atksh-utils-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:41:51.443400 atksh-utils-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:41:51.439399 atksh-utils-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:41:51.443400 atksh-utils-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-18 01:41:38.000000 atksh-utils-0.1.0/.github/workflows/publish_to_pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-18 01:41:38.000000 atksh-utils-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-18 01:41:38.000000 atksh-utils-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-18 01:41:38.000000 atksh-utils-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-18 01:41:51.443400 atksh-utils-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-18 01:41:38.000000 atksh-utils-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-18 01:41:38.000000 atksh-utils-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-18 01:41:51.443400 atksh-utils-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:41:51.439399 atksh-utils-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:41:51.443400 atksh-utils-0.1.0/src/atksh_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 01:41:38.000000 atksh-utils-0.1.0/src/atksh_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:41:51.443400 atksh-utils-0.1.0/src/atksh_utils/openai/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-18 01:41:38.000000 atksh-utils-0.1.0/src/atksh_utils/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-06-18 01:41:38.000000 atksh-utils-0.1.0/src/atksh_utils/openai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-18 01:41:38.000000 atksh-utils-0.1.0/src/atksh_utils/openai/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-18 01:41:38.000000 atksh-utils-0.1.0/src/atksh_utils/openai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 01:41:51.000000 atksh-utils-0.1.0/src/atksh_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:41:51.443400 atksh-utils-0.1.0/src/atksh_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-18 01:41:51.000000 atksh-utils-0.1.0/src/atksh_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-18 01:41:51.000000 atksh-utils-0.1.0/src/atksh_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 01:41:51.000000 atksh-utils-0.1.0/src/atksh_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-18 01:41:51.000000 atksh-utils-0.1.0/src/atksh_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 01:41:51.000000 atksh-utils-0.1.0/src/atksh_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:41:51.439399 atksh-utils-0.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:41:51.443400 atksh-utils-0.1.0/tests/openai/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-18 01:41:38.000000 atksh-utils-0.1.0/tests/openai/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-18 01:41:38.000000 atksh-utils-0.1.0/tests/openai/test_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:57:44.600569 atksh-utils-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:57:44.596569 atksh-utils-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:57:44.596569 atksh-utils-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-18 01:57:34.000000 atksh-utils-0.1.1/.github/workflows/publish_to_pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-18 01:57:34.000000 atksh-utils-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-18 01:57:34.000000 atksh-utils-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-18 01:57:34.000000 atksh-utils-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-18 01:57:44.600569 atksh-utils-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-18 01:57:34.000000 atksh-utils-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-18 01:57:34.000000 atksh-utils-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-18 01:57:44.600569 atksh-utils-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:57:44.596569 atksh-utils-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:57:44.600569 atksh-utils-0.1.1/src/atksh_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 01:57:34.000000 atksh-utils-0.1.1/src/atksh_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:57:44.600569 atksh-utils-0.1.1/src/atksh_utils/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-18 01:57:34.000000 atksh-utils-0.1.1/src/atksh_utils/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-06-18 01:57:34.000000 atksh-utils-0.1.1/src/atksh_utils/openai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-18 01:57:34.000000 atksh-utils-0.1.1/src/atksh_utils/openai/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-18 01:57:34.000000 atksh-utils-0.1.1/src/atksh_utils/openai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 01:57:44.000000 atksh-utils-0.1.1/src/atksh_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:57:44.600569 atksh-utils-0.1.1/src/atksh_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-18 01:57:44.000000 atksh-utils-0.1.1/src/atksh_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-18 01:57:44.000000 atksh-utils-0.1.1/src/atksh_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 01:57:44.000000 atksh-utils-0.1.1/src/atksh_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-18 01:57:44.000000 atksh-utils-0.1.1/src/atksh_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 01:57:44.000000 atksh-utils-0.1.1/src/atksh_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:57:44.596569 atksh-utils-0.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:57:44.600569 atksh-utils-0.1.1/tests/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-18 01:57:34.000000 atksh-utils-0.1.1/tests/openai/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-18 01:57:34.000000 atksh-utils-0.1.1/tests/openai/test_functional.py
```

### Comparing `atksh-utils-0.1.0/.github/workflows/publish_to_pypi.yaml` & `atksh-utils-0.1.1/.github/workflows/publish_to_pypi.yaml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.0/.gitignore` & `atksh-utils-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.0/LICENSE` & `atksh-utils-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.0/PKG-INFO` & `atksh-utils-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.1.0
+Version: 0.1.1
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.1.0/README.md` & `atksh-utils-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.0/pyproject.toml` & `atksh-utils-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.0/src/atksh_utils/openai/api.py` & `atksh-utils-0.1.1/src/atksh_utils/openai/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
         actor.set_system_prompt(generate_react_prompt(turn="act"))
 
         def analyze(description):
             """Analyze the description. The output format is like `goal state: xxx, current state: xxx, summary: xxx`.
 
             :param description: The well described text of the current situation and the context.
             :type description: str
-            :return: The goal state, the current state, and summary of the current situation and the context.
+            :return: The goal state, the current state, and summary of the current situation and the context. This includes the available functions and their arguments.
             :rtype: str
             """
             return analyzer(f"{description}")[1]
 
         def plan(goal_state, current_state):
             """Plan the sequence of actions to achieve the goal state from the current state.
```

### Comparing `atksh-utils-0.1.0/src/atksh_utils/openai/functional.py` & `atksh-utils-0.1.1/src/atksh_utils/openai/functional.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.0/src/atksh_utils/openai/prompt.py` & `atksh-utils-0.1.1/src/atksh_utils/openai/prompt.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.0/src/atksh_utils.egg-info/PKG-INFO` & `atksh-utils-0.1.1/src/atksh_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.1.0
+Version: 0.1.1
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.1.0/src/atksh_utils.egg-info/SOURCES.txt` & `atksh-utils-0.1.1/src/atksh_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.0/tests/openai/test_api.py` & `atksh-utils-0.1.1/tests/openai/test_api.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.0/tests/openai/test_functional.py` & `atksh-utils-0.1.1/tests/openai/test_functional.py`

 * *Files identical despite different names*

