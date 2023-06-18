# Comparing `tmp/requirements-language-server-0.0.1.tar.gz` & `tmp/requirements-language-server-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requirements-language-server-0.0.1.tar", last modified: Sun Jun 18 17:18:00 2023, max compression
+gzip compressed data, was "requirements-language-server-0.0.2.tar", last modified: Sun Jun 18 17:24:24 2023, max compression
```

## Comparing `requirements-language-server-0.0.1.tar` & `requirements-language-server-0.0.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:18:00.702471 requirements-language-server-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:18:00.698471 requirements-language-server-0.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:18:00.698471 requirements-language-server-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-06-18 17:18:00.698471 requirements-language-server-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:18:00.698471 requirements-language-server-0.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:18:00.698471 requirements-language-server-0.0.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/docs/api/requirements-language-server.md
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/docs/index.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:18:00.698471 requirements-language-server-0.0.1/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/flake.nix
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:18:00.698471 requirements-language-server-0.0.1/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:18:00.698471 requirements-language-server-0.0.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/scripts/generate-api.md.pl
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 17:18:00.702471 requirements-language-server-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:18:00.694471 requirements-language-server-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:18:00.698471 requirements-language-server-0.0.1/src/requirements_language_server/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/src/requirements_language_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/src/requirements_language_server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 17:18:00.000000 requirements-language-server-0.0.1/src/requirements_language_server/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/src/requirements_language_server/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:18:00.694471 requirements-language-server-0.0.1/src/requirements_language_server/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:18:00.698471 requirements-language-server-0.0.1/src/requirements_language_server/assets/jinja2/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/src/requirements_language_server/assets/jinja2/template.md.j2
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/src/requirements_language_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9468 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/src/requirements_language_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:18:00.698471 requirements-language-server-0.0.1/src/requirements_language_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-06-18 17:18:00.000000 requirements-language-server-0.0.1/src/requirements_language_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-18 17:18:00.000000 requirements-language-server-0.0.1/src/requirements_language_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 17:18:00.000000 requirements-language-server-0.0.1/src/requirements_language_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-18 17:18:00.000000 requirements-language-server-0.0.1/src/requirements_language_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-18 17:18:00.000000 requirements-language-server-0.0.1/src/requirements_language_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-18 17:18:00.000000 requirements-language-server-0.0.1/src/requirements_language_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:18:00.698471 requirements-language-server-0.0.1/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/templates/noarg.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:18:00.698471 requirements-language-server-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/tests/api_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/tests/requirements.txt.in
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-18 17:17:48.000000 requirements-language-server-0.0.1/tests/server_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.682070 requirements-language-server-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.678070 requirements-language-server-0.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.678070 requirements-language-server-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-06-18 17:24:24.682070 requirements-language-server-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.678070 requirements-language-server-0.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.678070 requirements-language-server-0.0.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/docs/api/requirements-language-server.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/docs/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.678070 requirements-language-server-0.0.2/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/docs/resources/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/flake.nix
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.678070 requirements-language-server-0.0.2/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.678070 requirements-language-server-0.0.2/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/scripts/generate-api.md.pl
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 17:24:24.682070 requirements-language-server-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.678070 requirements-language-server-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.678070 requirements-language-server-0.0.2/src/requirements_language_server/
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/src/requirements_language_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/src/requirements_language_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 17:24:24.000000 requirements-language-server-0.0.2/src/requirements_language_server/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/src/requirements_language_server/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.678070 requirements-language-server-0.0.2/src/requirements_language_server/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.682070 requirements-language-server-0.0.2/src/requirements_language_server/assets/jinja2/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/src/requirements_language_server/assets/jinja2/template.md.j2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/src/requirements_language_server/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9468 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/src/requirements_language_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.682070 requirements-language-server-0.0.2/src/requirements_language_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-06-18 17:24:24.000000 requirements-language-server-0.0.2/src/requirements_language_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-18 17:24:24.000000 requirements-language-server-0.0.2/src/requirements_language_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 17:24:24.000000 requirements-language-server-0.0.2/src/requirements_language_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-18 17:24:24.000000 requirements-language-server-0.0.2/src/requirements_language_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-18 17:24:24.000000 requirements-language-server-0.0.2/src/requirements_language_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-18 17:24:24.000000 requirements-language-server-0.0.2/src/requirements_language_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.682070 requirements-language-server-0.0.2/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/templates/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/templates/def.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/templates/noarg.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.682070 requirements-language-server-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/tests/api_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/tests/requirements.txt.in
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/tests/server_test.py
```

### Comparing `requirements-language-server-0.0.1/.github/workflows/main.yml` & `requirements-language-server-0.0.2/.github/workflows/main.yml`

 * *Files 2% similar despite different names*

```diff
@@ -89,9 +89,9 @@
   deploy:
     needs: build
     runs-on: ubuntu-latest
     steps:
       - uses: Freed-Wu/update-aur-package@v1.0.11
         if: startsWith(github.ref, 'refs/tags/')
         with:
-          package_name: python-autoconf-language-server
+          package_name: python-requirements-language-server
           ssh_private_key: ${{secrets.AUR_SSH_PRIVATE_KEY}}
```

### Comparing `requirements-language-server-0.0.1/.gitignore` & `requirements-language-server-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.1/.pre-commit-config.yaml` & `requirements-language-server-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.1/LICENSE` & `requirements-language-server-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.1/PKG-INFO` & `requirements-language-server-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requirements-language-server
-Version: 0.0.1
+Version: 0.0.2
 Summary: requirements language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://requirements-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/requirements-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/requirements-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/requirements-language-server
```

### Comparing `requirements-language-server-0.0.1/README.md` & `requirements-language-server-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.1/docs/conf.py` & `requirements-language-server-0.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.1/docs/resources/install.md` & `requirements-language-server-0.0.2/docs/resources/install.md`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.1/flake.nix` & `requirements-language-server-0.0.2/flake.nix`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.1/pyproject.toml` & `requirements-language-server-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.1/src/requirements_language_server/__init__.py` & `requirements-language-server-0.0.2/src/requirements_language_server/__init__.py`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.1/src/requirements_language_server/__main__.py` & `requirements-language-server-0.0.2/src/requirements_language_server/__main__.py`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.1/src/requirements_language_server/api.py` & `requirements-language-server-0.0.2/src/requirements_language_server/api.py`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.1/src/requirements_language_server/server.py` & `requirements-language-server-0.0.2/src/requirements_language_server/server.py`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.1/src/requirements_language_server.egg-info/PKG-INFO` & `requirements-language-server-0.0.2/src/requirements_language_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requirements-language-server
-Version: 0.0.1
+Version: 0.0.2
 Summary: requirements language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://requirements-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/requirements-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/requirements-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/requirements-language-server
```

### Comparing `requirements-language-server-0.0.1/src/requirements_language_server.egg-info/SOURCES.txt` & `requirements-language-server-0.0.2/src/requirements_language_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

