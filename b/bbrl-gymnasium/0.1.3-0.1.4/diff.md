# Comparing `tmp/bbrl_gymnasium-0.1.3.tar.gz` & `tmp/bbrl_gymnasium-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbrl_gymnasium-0.1.3.tar", last modified: Fri Jun  2 08:03:52 2023, max compression
+gzip compressed data, was "bbrl_gymnasium-0.1.4.tar", last modified: Sun Jun 18 16:39:41 2023, max compression
```

## Comparing `bbrl_gymnasium-0.1.3.tar` & `bbrl_gymnasium-0.1.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:03:52.551940 bbrl_gymnasium-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:03:52.535940 bbrl_gymnasium-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:03:52.543940 bbrl_gymnasium-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-02 08:03:39.000000 bbrl_gymnasium-0.1.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 08:03:39.000000 bbrl_gymnasium-0.1.3/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-06-02 08:03:39.000000 bbrl_gymnasium-0.1.3/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)       24 2023-06-02 08:03:39.000000 bbrl_gymnasium-0.1.3/MANIFEST.in
--rwxr-xr-x   0 runner    (1001) docker     (123)     1388 2023-06-02 08:03:39.000000 bbrl_gymnasium-0.1.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-02 08:03:52.555940 bbrl_gymnasium-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-02 08:03:39.000000 bbrl_gymnasium-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:03:52.543940 bbrl_gymnasium-0.1.3/bbrl_gymnasium/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-02 08:03:39.000000 bbrl_gymnasium-0.1.3/bbrl_gymnasium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 08:03:52.000000 bbrl_gymnasium-0.1.3/bbrl_gymnasium/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:03:52.551940 bbrl_gymnasium-0.1.3/bbrl_gymnasium/envs/
--rwxr-xr-x   0 runner    (1001) docker     (123)      434 2023-06-02 08:03:39.000000 bbrl_gymnasium-0.1.3/bbrl_gymnasium/envs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2693 2023-06-02 08:03:39.000000 bbrl_gymnasium-0.1.3/bbrl_gymnasium/envs/continuous_2D_mdp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5895 2023-06-02 08:03:39.000000 bbrl_gymnasium-0.1.3/bbrl_gymnasium/envs/continuous_cartpole.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2557 2023-06-02 08:03:39.000000 bbrl_gymnasium-0.1.3/bbrl_gymnasium/envs/continuous_line_mdp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1786 2023-06-02 08:03:39.000000 bbrl_gymnasium-0.1.3/bbrl_gymnasium/envs/debug_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2391 2023-06-02 08:03:39.000000 bbrl_gymnasium-0.1.3/bbrl_gymnasium/envs/line_mdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-06-02 08:03:39.000000 bbrl_gymnasium-0.1.3/bbrl_gymnasium/envs/maze_mdp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21845 2023-06-02 08:03:39.000000 bbrl_gymnasium-0.1.3/bbrl_gymnasium/envs/rocket_lander.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:03:52.551940 bbrl_gymnasium-0.1.3/bbrl_gymnasium/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-02 08:03:39.000000 bbrl_gymnasium-0.1.3/bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-06-02 08:03:39.000000 bbrl_gymnasium-0.1.3/bbrl_gymnasium/wrappers/rocket_lander_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:03:52.547940 bbrl_gymnasium-0.1.3/bbrl_gymnasium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-02 08:03:52.000000 bbrl_gymnasium-0.1.3/bbrl_gymnasium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-02 08:03:52.000000 bbrl_gymnasium-0.1.3/bbrl_gymnasium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:03:52.000000 bbrl_gymnasium-0.1.3/bbrl_gymnasium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-02 08:03:52.000000 bbrl_gymnasium-0.1.3/bbrl_gymnasium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-02 08:03:52.000000 bbrl_gymnasium-0.1.3/bbrl_gymnasium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-02 08:03:39.000000 bbrl_gymnasium-0.1.3/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)       58 2023-06-02 08:03:39.000000 bbrl_gymnasium-0.1.3/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      466 2023-06-02 08:03:52.555940 bbrl_gymnasium-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-02 08:03:39.000000 bbrl_gymnasium-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:03:52.551940 bbrl_gymnasium-0.1.3/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:03:39.000000 bbrl_gymnasium-0.1.3/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      811 2023-06-02 08:03:39.000000 bbrl_gymnasium-0.1.3/tests/test_bbrl_gym.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2735 2023-06-02 08:03:39.000000 bbrl_gymnasium-0.1.3/tests/test_maze.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      144 2023-06-02 08:03:39.000000 bbrl_gymnasium-0.1.3/tests/test_rocket_lander.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:39:41.273652 bbrl_gymnasium-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:39:41.269651 bbrl_gymnasium-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:39:41.269651 bbrl_gymnasium-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)       24 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/MANIFEST.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1388 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-18 16:39:41.273652 bbrl_gymnasium-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:39:41.269651 bbrl_gymnasium-0.1.4/bbrl_gymnasium/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 16:39:41.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:39:41.273652 bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      434 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2693 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/continuous_2D_mdp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3027 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/continuous_cartpole.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2557 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/continuous_line_mdp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1786 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/debug_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2391 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/line_mdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/maze_mdp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21845 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/rocket_lander.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:39:41.273652 bbrl_gymnasium-0.1.4/bbrl_gymnasium/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium/wrappers/rocket_lander_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:39:41.269651 bbrl_gymnasium-0.1.4/bbrl_gymnasium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-18 16:39:41.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-18 16:39:41.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 16:39:41.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-18 16:39:41.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-18 16:39:41.000000 bbrl_gymnasium-0.1.4/bbrl_gymnasium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       56 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      408 2023-06-18 16:39:41.273652 bbrl_gymnasium-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:39:41.273652 bbrl_gymnasium-0.1.4/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      811 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/tests/test_bbrl_gym.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2735 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/tests/test_maze.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      144 2023-06-18 16:39:30.000000 bbrl_gymnasium-0.1.4/tests/test_rocket_lander.py
```

### Comparing `bbrl_gymnasium-0.1.3/.github/workflows/python-publish.yml` & `bbrl_gymnasium-0.1.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.3/LICENSE` & `bbrl_gymnasium-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.3/Makefile` & `bbrl_gymnasium-0.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.3/PKG-INFO` & `bbrl_gymnasium-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbrl_gymnasium
-Version: 0.1.3
+Version: 0.1.4
 Summary: A set of additional gym environments
 Home-page: https://github.com/osigaud/bbrl_gym
 Author: Olivier Sigaud
 Author-email: Olivier.Sigaud@isir.upmc.fr
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bbrl_gymnasium-0.1.3/README.md` & `bbrl_gymnasium-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.3/bbrl_gymnasium/__init__.py` & `bbrl_gymnasium-0.1.4/bbrl_gymnasium/__init__.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.3/bbrl_gymnasium/envs/continuous_2D_mdp.py` & `bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/continuous_2D_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.3/bbrl_gymnasium/envs/continuous_line_mdp.py` & `bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/continuous_line_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.3/bbrl_gymnasium/envs/debug_env.py` & `bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/debug_env.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.3/bbrl_gymnasium/envs/line_mdp.py` & `bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/line_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.3/bbrl_gymnasium/envs/maze_mdp.py` & `bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/maze_mdp.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.3/bbrl_gymnasium/envs/rocket_lander.py` & `bbrl_gymnasium-0.1.4/bbrl_gymnasium/envs/rocket_lander.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.3/bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py` & `bbrl_gymnasium-0.1.4/bbrl_gymnasium/wrappers/mazemdp_continuous_wrapper.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.3/bbrl_gymnasium/wrappers/rocket_lander_wrapper.py` & `bbrl_gymnasium-0.1.4/bbrl_gymnasium/wrappers/rocket_lander_wrapper.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.3/bbrl_gymnasium.egg-info/PKG-INFO` & `bbrl_gymnasium-0.1.4/bbrl_gymnasium.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbrl-gymnasium
-Version: 0.1.3
+Version: 0.1.4
 Summary: A set of additional gym environments
 Home-page: https://github.com/osigaud/bbrl_gym
 Author: Olivier Sigaud
 Author-email: Olivier.Sigaud@isir.upmc.fr
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bbrl_gymnasium-0.1.3/bbrl_gymnasium.egg-info/SOURCES.txt` & `bbrl_gymnasium-0.1.4/bbrl_gymnasium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.3/setup.py` & `bbrl_gymnasium-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.3/tests/test_bbrl_gym.py` & `bbrl_gymnasium-0.1.4/tests/test_bbrl_gym.py`

 * *Files identical despite different names*

### Comparing `bbrl_gymnasium-0.1.3/tests/test_maze.py` & `bbrl_gymnasium-0.1.4/tests/test_maze.py`

 * *Files identical despite different names*

