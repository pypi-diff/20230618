# Comparing `tmp/autoconf-language-server-0.0.1.tar.gz` & `tmp/autoconf-language-server-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoconf-language-server-0.0.1.tar", last modified: Sat Jun 17 17:35:54 2023, max compression
+gzip compressed data, was "autoconf-language-server-0.0.2.tar", last modified: Sun Jun 18 04:45:41 2023, max compression
```

## Comparing `autoconf-language-server-0.0.1.tar` & `autoconf-language-server-0.0.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:35:54.659230 autoconf-language-server-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:35:54.655230 autoconf-language-server-0.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:35:54.655230 autoconf-language-server-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-06-17 17:35:54.659230 autoconf-language-server-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:35:54.655230 autoconf-language-server-0.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:35:54.655230 autoconf-language-server-0.0.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/docs/api/autoconf-language-server.md
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/docs/index.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:35:54.659230 autoconf-language-server-0.0.1/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/flake.nix
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:35:54.659230 autoconf-language-server-0.0.1/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:35:54.659230 autoconf-language-server-0.0.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/scripts/generate-api.md.pl
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 17:35:54.659230 autoconf-language-server-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:35:54.655230 autoconf-language-server-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:35:54.659230 autoconf-language-server-0.0.1/src/autoconf_language_server/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/src/autoconf_language_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/src/autoconf_language_server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-17 17:35:54.000000 autoconf-language-server-0.0.1/src/autoconf_language_server/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/src/autoconf_language_server/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:35:54.655230 autoconf-language-server-0.0.1/src/autoconf_language_server/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:35:54.659230 autoconf-language-server-0.0.1/src/autoconf_language_server/assets/json/
--rw-r--r--   0 runner    (1001) docker     (123)   402908 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/src/autoconf_language_server/assets/json/autoconf.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/src/autoconf_language_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/src/autoconf_language_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:35:54.659230 autoconf-language-server-0.0.1/src/autoconf_language_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-06-17 17:35:54.000000 autoconf-language-server-0.0.1/src/autoconf_language_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-17 17:35:54.000000 autoconf-language-server-0.0.1/src/autoconf_language_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 17:35:54.000000 autoconf-language-server-0.0.1/src/autoconf_language_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-17 17:35:54.000000 autoconf-language-server-0.0.1/src/autoconf_language_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-17 17:35:54.000000 autoconf-language-server-0.0.1/src/autoconf_language_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-17 17:35:54.000000 autoconf-language-server-0.0.1/src/autoconf_language_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:35:54.659230 autoconf-language-server-0.0.1/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/templates/noarg.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:35:54.659230 autoconf-language-server-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-17 17:35:26.000000 autoconf-language-server-0.0.1/tests/api_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.268030 autoconf-language-server-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.264030 autoconf-language-server-0.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.264030 autoconf-language-server-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-06-18 04:45:41.268030 autoconf-language-server-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.264030 autoconf-language-server-0.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.264030 autoconf-language-server-0.0.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/docs/api/autoconf-language-server.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/docs/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.264030 autoconf-language-server-0.0.2/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/docs/resources/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/flake.nix
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.264030 autoconf-language-server-0.0.2/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.264030 autoconf-language-server-0.0.2/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/scripts/generate-api.md.pl
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 04:45:41.268030 autoconf-language-server-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.264030 autoconf-language-server-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.264030 autoconf-language-server-0.0.2/src/autoconf_language_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/src/autoconf_language_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/src/autoconf_language_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 04:45:41.000000 autoconf-language-server-0.0.2/src/autoconf_language_server/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/src/autoconf_language_server/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.264030 autoconf-language-server-0.0.2/src/autoconf_language_server/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.268030 autoconf-language-server-0.0.2/src/autoconf_language_server/assets/json/
+-rw-r--r--   0 runner    (1001) docker     (123)   402908 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/src/autoconf_language_server/assets/json/autoconf.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/src/autoconf_language_server/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/src/autoconf_language_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.268030 autoconf-language-server-0.0.2/src/autoconf_language_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-06-18 04:45:41.000000 autoconf-language-server-0.0.2/src/autoconf_language_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-18 04:45:41.000000 autoconf-language-server-0.0.2/src/autoconf_language_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 04:45:41.000000 autoconf-language-server-0.0.2/src/autoconf_language_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-18 04:45:41.000000 autoconf-language-server-0.0.2/src/autoconf_language_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-18 04:45:41.000000 autoconf-language-server-0.0.2/src/autoconf_language_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-18 04:45:41.000000 autoconf-language-server-0.0.2/src/autoconf_language_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.268030 autoconf-language-server-0.0.2/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/templates/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/templates/def.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/templates/noarg.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.268030 autoconf-language-server-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/tests/server_test.py
```

### Comparing `autoconf-language-server-0.0.1/.github/workflows/main.yml` & `autoconf-language-server-0.0.2/.github/workflows/main.yml`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         if: runner.os == 'Linux' && ! startsWith(github.ref, 'refs/tags/')
         with:
           path: |
             dist/*
       - uses: softprops/action-gh-release@v1
         if: runner.os == 'Linux' && startsWith(github.ref, 'refs/tags/')
         with:
-          body_path: build/CHANGELOG.md
+          # body_path: build/CHANGELOG.md
           files: |
             dist/*
   deploy:
     needs: build
     runs-on: ubuntu-latest
     steps:
       - uses: Freed-Wu/update-aur-package@v1.0.10
```

### Comparing `autoconf-language-server-0.0.1/.gitignore` & `autoconf-language-server-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.1/.pre-commit-config.yaml` & `autoconf-language-server-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.1/LICENSE` & `autoconf-language-server-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.1/PKG-INFO` & `autoconf-language-server-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoconf-language-server
-Version: 0.0.1
+Version: 0.0.2
 Summary: autoconf language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://autoconf-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/autoconf-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/autoconf-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/autoconf-language-server
@@ -120,12 +120,12 @@
   augroup END
 endif
 ```
 
 ## Customization
 
 See
-<https://autoconf-language-server.readthedocs.io/en/latest/api/autoconf-language-server.html#autoconf_language_server.api.get_document>.
+<https://autoconf-language-server.readthedocs.io/en/latest/api/autoconf-language-server.html#autoconf_language_server.server.get_document>.
 
 ## Similar Projects
 
 - [cmake-language-server](https://github.com/regen100/cmake-language-server)
```

### Comparing `autoconf-language-server-0.0.1/README.md` & `autoconf-language-server-0.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -87,12 +87,12 @@
   augroup END
 endif
 ```
 
 ## Customization
 
 See
-<https://autoconf-language-server.readthedocs.io/en/latest/api/autoconf-language-server.html#autoconf_language_server.api.get_document>.
+<https://autoconf-language-server.readthedocs.io/en/latest/api/autoconf-language-server.html#autoconf_language_server.server.get_document>.
 
 ## Similar Projects
 
 - [cmake-language-server](https://github.com/regen100/cmake-language-server)
```

### Comparing `autoconf-language-server-0.0.1/docs/conf.py` & `autoconf-language-server-0.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.1/docs/resources/install.md` & `autoconf-language-server-0.0.2/docs/resources/install.md`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.1/flake.nix` & `autoconf-language-server-0.0.2/flake.nix`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.1/pyproject.toml` & `autoconf-language-server-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.1/src/autoconf_language_server/__main__.py` & `autoconf-language-server-0.0.2/src/autoconf_language_server/__main__.py`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.1/src/autoconf_language_server/assets/json/autoconf.json` & `autoconf-language-server-0.0.2/src/autoconf_language_server/assets/json/autoconf.json`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.1/src/autoconf_language_server.egg-info/PKG-INFO` & `autoconf-language-server-0.0.2/src/autoconf_language_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoconf-language-server
-Version: 0.0.1
+Version: 0.0.2
 Summary: autoconf language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://autoconf-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/autoconf-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/autoconf-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/autoconf-language-server
@@ -120,12 +120,12 @@
   augroup END
 endif
 ```
 
 ## Customization
 
 See
-<https://autoconf-language-server.readthedocs.io/en/latest/api/autoconf-language-server.html#autoconf_language_server.api.get_document>.
+<https://autoconf-language-server.readthedocs.io/en/latest/api/autoconf-language-server.html#autoconf_language_server.server.get_document>.
 
 ## Similar Projects
 
 - [cmake-language-server](https://github.com/regen100/cmake-language-server)
```

### Comparing `autoconf-language-server-0.0.1/src/autoconf_language_server.egg-info/SOURCES.txt` & `autoconf-language-server-0.0.2/src/autoconf_language_server.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -29,8 +29,8 @@
 src/autoconf_language_server.egg-info/entry_points.txt
 src/autoconf_language_server.egg-info/requires.txt
 src/autoconf_language_server.egg-info/top_level.txt
 src/autoconf_language_server/assets/json/autoconf.json
 templates/class.txt
 templates/def.txt
 templates/noarg.txt
-tests/api_test.py
+tests/server_test.py
```

