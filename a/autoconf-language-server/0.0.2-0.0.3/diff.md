# Comparing `tmp/autoconf-language-server-0.0.2.tar.gz` & `tmp/autoconf-language-server-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoconf-language-server-0.0.2.tar", last modified: Sun Jun 18 04:45:41 2023, max compression
+gzip compressed data, was "autoconf-language-server-0.0.3.tar", last modified: Sun Jun 18 04:54:06 2023, max compression
```

## Comparing `autoconf-language-server-0.0.2.tar` & `autoconf-language-server-0.0.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.268030 autoconf-language-server-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.264030 autoconf-language-server-0.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.264030 autoconf-language-server-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-06-18 04:45:41.268030 autoconf-language-server-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.264030 autoconf-language-server-0.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.264030 autoconf-language-server-0.0.2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/docs/api/autoconf-language-server.md
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/docs/index.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.264030 autoconf-language-server-0.0.2/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/flake.nix
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.264030 autoconf-language-server-0.0.2/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.264030 autoconf-language-server-0.0.2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/scripts/generate-api.md.pl
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 04:45:41.268030 autoconf-language-server-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.264030 autoconf-language-server-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.264030 autoconf-language-server-0.0.2/src/autoconf_language_server/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/src/autoconf_language_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/src/autoconf_language_server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 04:45:41.000000 autoconf-language-server-0.0.2/src/autoconf_language_server/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/src/autoconf_language_server/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.264030 autoconf-language-server-0.0.2/src/autoconf_language_server/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.268030 autoconf-language-server-0.0.2/src/autoconf_language_server/assets/json/
--rw-r--r--   0 runner    (1001) docker     (123)   402908 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/src/autoconf_language_server/assets/json/autoconf.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/src/autoconf_language_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/src/autoconf_language_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.268030 autoconf-language-server-0.0.2/src/autoconf_language_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-06-18 04:45:41.000000 autoconf-language-server-0.0.2/src/autoconf_language_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-18 04:45:41.000000 autoconf-language-server-0.0.2/src/autoconf_language_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 04:45:41.000000 autoconf-language-server-0.0.2/src/autoconf_language_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-18 04:45:41.000000 autoconf-language-server-0.0.2/src/autoconf_language_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-18 04:45:41.000000 autoconf-language-server-0.0.2/src/autoconf_language_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-18 04:45:41.000000 autoconf-language-server-0.0.2/src/autoconf_language_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.268030 autoconf-language-server-0.0.2/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/templates/noarg.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:45:41.268030 autoconf-language-server-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-18 04:45:28.000000 autoconf-language-server-0.0.2/tests/server_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:54:06.435254 autoconf-language-server-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:54:06.423254 autoconf-language-server-0.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:54:06.423254 autoconf-language-server-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-06-18 04:54:06.435254 autoconf-language-server-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:54:06.427254 autoconf-language-server-0.0.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:54:06.427254 autoconf-language-server-0.0.3/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/docs/api/autoconf-language-server.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/docs/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:54:06.427254 autoconf-language-server-0.0.3/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/docs/resources/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/flake.nix
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:54:06.427254 autoconf-language-server-0.0.3/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:54:06.427254 autoconf-language-server-0.0.3/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/scripts/generate-api.md.pl
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 04:54:06.435254 autoconf-language-server-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:54:06.419254 autoconf-language-server-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:54:06.431254 autoconf-language-server-0.0.3/src/autoconf_language_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/src/autoconf_language_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/src/autoconf_language_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 04:54:06.000000 autoconf-language-server-0.0.3/src/autoconf_language_server/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/src/autoconf_language_server/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:54:06.419254 autoconf-language-server-0.0.3/src/autoconf_language_server/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:54:06.435254 autoconf-language-server-0.0.3/src/autoconf_language_server/assets/json/
+-rw-r--r--   0 runner    (1001) docker     (123)   402908 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/src/autoconf_language_server/assets/json/autoconf.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/src/autoconf_language_server/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/src/autoconf_language_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:54:06.431254 autoconf-language-server-0.0.3/src/autoconf_language_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-06-18 04:54:06.000000 autoconf-language-server-0.0.3/src/autoconf_language_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-18 04:54:06.000000 autoconf-language-server-0.0.3/src/autoconf_language_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 04:54:06.000000 autoconf-language-server-0.0.3/src/autoconf_language_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-18 04:54:06.000000 autoconf-language-server-0.0.3/src/autoconf_language_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-18 04:54:06.000000 autoconf-language-server-0.0.3/src/autoconf_language_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-18 04:54:06.000000 autoconf-language-server-0.0.3/src/autoconf_language_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:54:06.435254 autoconf-language-server-0.0.3/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/templates/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/templates/def.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/templates/noarg.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:54:06.435254 autoconf-language-server-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-18 04:53:50.000000 autoconf-language-server-0.0.3/tests/server_test.py
```

### Comparing `autoconf-language-server-0.0.2/.github/workflows/main.yml` & `autoconf-language-server-0.0.3/.github/workflows/main.yml`

 * *Files 8% similar despite different names*

```diff
@@ -88,9 +88,9 @@
   deploy:
     needs: build
     runs-on: ubuntu-latest
     steps:
       - uses: Freed-Wu/update-aur-package@v1.0.10
         if: startsWith(github.ref, 'refs/tags/')
         with:
-          package_name: python-${{github.repository}}
+          package_name: python-autoconf-language-server
           ssh_private_key: ${{secrets.AUR_SSH_PRIVATE_KEY}}
```

### Comparing `autoconf-language-server-0.0.2/.gitignore` & `autoconf-language-server-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.2/.pre-commit-config.yaml` & `autoconf-language-server-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.2/LICENSE` & `autoconf-language-server-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.2/PKG-INFO` & `autoconf-language-server-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoconf-language-server
-Version: 0.0.2
+Version: 0.0.3
 Summary: autoconf language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://autoconf-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/autoconf-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/autoconf-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/autoconf-language-server
```

### Comparing `autoconf-language-server-0.0.2/README.md` & `autoconf-language-server-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.2/docs/conf.py` & `autoconf-language-server-0.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.2/docs/resources/install.md` & `autoconf-language-server-0.0.3/docs/resources/install.md`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.2/flake.nix` & `autoconf-language-server-0.0.3/flake.nix`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.2/pyproject.toml` & `autoconf-language-server-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.2/src/autoconf_language_server/__main__.py` & `autoconf-language-server-0.0.3/src/autoconf_language_server/__main__.py`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.2/src/autoconf_language_server/api.py` & `autoconf-language-server-0.0.3/src/autoconf_language_server/api.py`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.2/src/autoconf_language_server/assets/json/autoconf.json` & `autoconf-language-server-0.0.3/src/autoconf_language_server/assets/json/autoconf.json`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.2/src/autoconf_language_server/server.py` & `autoconf-language-server-0.0.3/src/autoconf_language_server/server.py`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.2/src/autoconf_language_server.egg-info/PKG-INFO` & `autoconf-language-server-0.0.3/src/autoconf_language_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoconf-language-server
-Version: 0.0.2
+Version: 0.0.3
 Summary: autoconf language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://autoconf-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/autoconf-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/autoconf-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/autoconf-language-server
```

### Comparing `autoconf-language-server-0.0.2/src/autoconf_language_server.egg-info/SOURCES.txt` & `autoconf-language-server-0.0.3/src/autoconf_language_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

