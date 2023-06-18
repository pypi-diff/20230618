# Comparing `tmp/atksh-utils-0.1.2.tar.gz` & `tmp/atksh-utils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atksh-utils-0.1.2.tar", last modified: Sun Jun 18 02:19:52 2023, max compression
+gzip compressed data, was "atksh-utils-0.1.3.tar", last modified: Sun Jun 18 02:20:34 2023, max compression
```

## Comparing `atksh-utils-0.1.2.tar` & `atksh-utils-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:19:52.601730 atksh-utils-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:19:52.601730 atksh-utils-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:19:52.601730 atksh-utils-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-18 02:19:42.000000 atksh-utils-0.1.2/.github/workflows/publish_to_pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-18 02:19:42.000000 atksh-utils-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-18 02:19:42.000000 atksh-utils-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-18 02:19:42.000000 atksh-utils-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-18 02:19:52.601730 atksh-utils-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-18 02:19:42.000000 atksh-utils-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-18 02:19:42.000000 atksh-utils-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-18 02:19:52.601730 atksh-utils-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:19:52.601730 atksh-utils-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:19:52.601730 atksh-utils-0.1.2/src/atksh_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 02:19:42.000000 atksh-utils-0.1.2/src/atksh_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:19:52.601730 atksh-utils-0.1.2/src/atksh_utils/openai/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-18 02:19:42.000000 atksh-utils-0.1.2/src/atksh_utils/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-06-18 02:19:42.000000 atksh-utils-0.1.2/src/atksh_utils/openai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-18 02:19:42.000000 atksh-utils-0.1.2/src/atksh_utils/openai/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-18 02:19:42.000000 atksh-utils-0.1.2/src/atksh_utils/openai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 02:19:52.000000 atksh-utils-0.1.2/src/atksh_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:19:52.601730 atksh-utils-0.1.2/src/atksh_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-18 02:19:52.000000 atksh-utils-0.1.2/src/atksh_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-18 02:19:52.000000 atksh-utils-0.1.2/src/atksh_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:19:52.000000 atksh-utils-0.1.2/src/atksh_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-18 02:19:52.000000 atksh-utils-0.1.2/src/atksh_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 02:19:52.000000 atksh-utils-0.1.2/src/atksh_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:19:52.601730 atksh-utils-0.1.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:19:52.601730 atksh-utils-0.1.2/tests/openai/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-18 02:19:42.000000 atksh-utils-0.1.2/tests/openai/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-18 02:19:42.000000 atksh-utils-0.1.2/tests/openai/test_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:20:34.290058 atksh-utils-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:20:34.290058 atksh-utils-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:20:34.290058 atksh-utils-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-18 02:20:21.000000 atksh-utils-0.1.3/.github/workflows/publish_to_pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-18 02:20:21.000000 atksh-utils-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-18 02:20:21.000000 atksh-utils-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-18 02:20:21.000000 atksh-utils-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-18 02:20:34.290058 atksh-utils-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-18 02:20:21.000000 atksh-utils-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-18 02:20:21.000000 atksh-utils-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-18 02:20:34.290058 atksh-utils-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:20:34.290058 atksh-utils-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:20:34.290058 atksh-utils-0.1.3/src/atksh_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 02:20:21.000000 atksh-utils-0.1.3/src/atksh_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:20:34.290058 atksh-utils-0.1.3/src/atksh_utils/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-18 02:20:21.000000 atksh-utils-0.1.3/src/atksh_utils/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-06-18 02:20:21.000000 atksh-utils-0.1.3/src/atksh_utils/openai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-18 02:20:21.000000 atksh-utils-0.1.3/src/atksh_utils/openai/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-18 02:20:21.000000 atksh-utils-0.1.3/src/atksh_utils/openai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 02:20:34.000000 atksh-utils-0.1.3/src/atksh_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:20:34.290058 atksh-utils-0.1.3/src/atksh_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-18 02:20:34.000000 atksh-utils-0.1.3/src/atksh_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-18 02:20:34.000000 atksh-utils-0.1.3/src/atksh_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:20:34.000000 atksh-utils-0.1.3/src/atksh_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-18 02:20:34.000000 atksh-utils-0.1.3/src/atksh_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 02:20:34.000000 atksh-utils-0.1.3/src/atksh_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:20:34.290058 atksh-utils-0.1.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:20:34.290058 atksh-utils-0.1.3/tests/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-18 02:20:21.000000 atksh-utils-0.1.3/tests/openai/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-18 02:20:21.000000 atksh-utils-0.1.3/tests/openai/test_functional.py
```

### Comparing `atksh-utils-0.1.2/.github/workflows/publish_to_pypi.yaml` & `atksh-utils-0.1.3/.github/workflows/publish_to_pypi.yaml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.2/.gitignore` & `atksh-utils-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.2/LICENSE` & `atksh-utils-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.2/PKG-INFO` & `atksh-utils-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.1.2/README.md` & `atksh-utils-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.2/pyproject.toml` & `atksh-utils-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.2/src/atksh_utils/openai/api.py` & `atksh-utils-0.1.3/src/atksh_utils/openai/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,15 +201,15 @@
             :type description: str
             :return: The goal state, the current state, and summary of the current situation and the context. This includes the available functions and their arguments.
             :rtype: str
             """
             return analyzer(f"{description}")[1]
 
         def plan(goal_state, current_state):
-            """Plan the sequence of actions to achieve the goal state from the current state.
+            """Plan the sequence of actions to achieve the goal state from the current state. This can also be called multiple times to replan the sequence of actions.
 
             :param goal_state: The goal state.
             :type goal_state: str
             :param current_state: The current state.
             :type current_state: str
             :return: The sequence of actions to achieve the goal state from the current state.
             :rtype: list[str]
```

### Comparing `atksh-utils-0.1.2/src/atksh_utils/openai/functional.py` & `atksh-utils-0.1.3/src/atksh_utils/openai/functional.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.2/src/atksh_utils/openai/prompt.py` & `atksh-utils-0.1.3/src/atksh_utils/openai/prompt.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.2/src/atksh_utils.egg-info/PKG-INFO` & `atksh-utils-0.1.3/src/atksh_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.1.2/src/atksh_utils.egg-info/SOURCES.txt` & `atksh-utils-0.1.3/src/atksh_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.2/tests/openai/test_api.py` & `atksh-utils-0.1.3/tests/openai/test_api.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.2/tests/openai/test_functional.py` & `atksh-utils-0.1.3/tests/openai/test_functional.py`

 * *Files identical despite different names*

