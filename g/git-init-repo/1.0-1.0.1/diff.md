# Comparing `tmp/git_init_repo-1.0.tar.gz` & `tmp/git_init_repo-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_init_repo-1.0.tar", last modified: Sun Jun 18 17:56:05 2023, max compression
+gzip compressed data, was "git_init_repo-1.0.1.tar", last modified: Sun Jun 18 18:55:10 2023, max compression
```

## Comparing `git_init_repo-1.0.tar` & `git_init_repo-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:56:05.958586 git_init_repo-1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-18 17:55:56.000000 git_init_repo-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-18 17:56:05.958586 git_init_repo-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-18 17:55:56.000000 git_init_repo-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:56:05.954586 git_init_repo-1.0/api_queries/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-18 17:55:56.000000 git_init_repo-1.0/api_queries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:56:05.958586 git_init_repo-1.0/git_init_repo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-18 17:56:05.000000 git_init_repo-1.0/git_init_repo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-18 17:56:05.000000 git_init_repo-1.0/git_init_repo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 17:56:05.000000 git_init_repo-1.0/git_init_repo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 17:56:05.000000 git_init_repo-1.0/git_init_repo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-18 17:56:05.000000 git_init_repo-1.0/git_init_repo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 17:56:05.958586 git_init_repo-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-18 17:55:56.000000 git_init_repo-1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:56:05.958586 git_init_repo-1.0/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-18 17:55:56.000000 git_init_repo-1.0/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-18 17:55:56.000000 git_init_repo-1.0/utils/vscode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:55:10.873213 git_init_repo-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-18 18:55:01.000000 git_init_repo-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-18 18:55:10.873213 git_init_repo-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-18 18:55:01.000000 git_init_repo-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:55:10.873213 git_init_repo-1.0.1/api_queries/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-18 18:55:01.000000 git_init_repo-1.0.1/api_queries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:55:10.873213 git_init_repo-1.0.1/git_init_repo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-18 18:55:10.000000 git_init_repo-1.0.1/git_init_repo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-18 18:55:10.000000 git_init_repo-1.0.1/git_init_repo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 18:55:10.000000 git_init_repo-1.0.1/git_init_repo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 18:55:10.000000 git_init_repo-1.0.1/git_init_repo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-18 18:55:10.000000 git_init_repo-1.0.1/git_init_repo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 18:55:10.873213 git_init_repo-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-18 18:55:01.000000 git_init_repo-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:55:10.873213 git_init_repo-1.0.1/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-18 18:55:01.000000 git_init_repo-1.0.1/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-18 18:55:01.000000 git_init_repo-1.0.1/utils/vscode.py
```

### Comparing `git_init_repo-1.0/LICENSE` & `git_init_repo-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `git_init_repo-1.0/api_queries/__init__.py` & `git_init_repo-1.0.1/api_queries/__init__.py`

 * *Files identical despite different names*

### Comparing `git_init_repo-1.0/utils/__init__.py` & `git_init_repo-1.0.1/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `git_init_repo-1.0/utils/vscode.py` & `git_init_repo-1.0.1/utils/vscode.py`

 * *Files identical despite different names*

