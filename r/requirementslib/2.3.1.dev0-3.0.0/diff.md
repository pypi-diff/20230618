# Comparing `tmp/requirementslib-2.3.1.dev0.tar.gz` & `tmp/requirementslib-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requirementslib-2.3.1.dev0.tar", last modified: Sun Jun 18 11:26:36 2023, max compression
+gzip compressed data, was "requirementslib-3.0.0.tar", last modified: Sun Jun 18 11:42:28 2023, max compression
```

## Comparing `requirementslib-2.3.1.dev0.tar` & `requirementslib-3.0.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:26:36.551856 requirementslib-2.3.1.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)    35908 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-06-18 11:26:36.551856 requirementslib-2.3.1.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11036 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:26:36.547856 requirementslib-2.3.1.dev0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.environment.rst
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.models.cache.rst
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.models.dependencies.rst
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.models.lockfile.rst
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.models.markers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.models.metadata.rst
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.models.pipfile.rst
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.models.project.rst
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.models.requirements.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.models.resolvers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.models.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.models.setup_info.rst
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.models.url.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.models.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.models.vcs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.rst
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-18 11:26:36.551856 requirementslib-2.3.1.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:26:36.543856 requirementslib-2.3.1.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:26:36.547856 requirementslib-2.3.1.dev0/src/requirementslib/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10862 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/fileutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/funktools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:26:36.551856 requirementslib-2.3.1.dev0/src/requirementslib/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/models/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/models/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/models/lockfile.py
--rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/models/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)    36642 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/models/old_pip_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/models/pipfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)   109147 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/models/requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)    61722 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/models/setup_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    17937 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/models/url.py
--rw-r--r--   0 runner    (1001) docker     (123)    26802 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/models/vcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27937 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:26:36.547856 requirementslib-2.3.1.dev0/src/requirementslib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-06-18 11:26:36.000000 requirementslib-2.3.1.dev0/src/requirementslib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-18 11:26:36.000000 requirementslib-2.3.1.dev0/src/requirementslib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 11:26:36.000000 requirementslib-2.3.1.dev0/src/requirementslib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-18 11:26:36.000000 requirementslib-2.3.1.dev0/src/requirementslib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-18 11:26:36.000000 requirementslib-2.3.1.dev0/src/requirementslib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 11:26:05.000000 requirementslib-2.3.1.dev0/src/requirementslib.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:42:28.173332 requirementslib-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35908 2023-06-18 11:41:45.000000 requirementslib-3.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-18 11:41:45.000000 requirementslib-3.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-18 11:41:45.000000 requirementslib-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-18 11:41:45.000000 requirementslib-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-06-18 11:42:28.173332 requirementslib-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11036 2023-06-18 11:41:45.000000 requirementslib-3.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:42:28.169332 requirementslib-3.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-18 11:41:45.000000 requirementslib-3.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-06-18 11:41:45.000000 requirementslib-3.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-18 11:41:45.000000 requirementslib-3.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-18 11:41:45.000000 requirementslib-3.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-18 11:41:45.000000 requirementslib-3.0.0/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-18 11:41:45.000000 requirementslib-3.0.0/docs/requirementslib.environment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-18 11:41:45.000000 requirementslib-3.0.0/docs/requirementslib.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-18 11:41:45.000000 requirementslib-3.0.0/docs/requirementslib.models.cache.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-18 11:41:45.000000 requirementslib-3.0.0/docs/requirementslib.models.dependencies.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-18 11:41:45.000000 requirementslib-3.0.0/docs/requirementslib.models.lockfile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-18 11:41:45.000000 requirementslib-3.0.0/docs/requirementslib.models.markers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-18 11:41:45.000000 requirementslib-3.0.0/docs/requirementslib.models.metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-18 11:41:45.000000 requirementslib-3.0.0/docs/requirementslib.models.pipfile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-18 11:41:45.000000 requirementslib-3.0.0/docs/requirementslib.models.project.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-18 11:41:45.000000 requirementslib-3.0.0/docs/requirementslib.models.requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-18 11:41:45.000000 requirementslib-3.0.0/docs/requirementslib.models.resolvers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-18 11:41:45.000000 requirementslib-3.0.0/docs/requirementslib.models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-18 11:41:45.000000 requirementslib-3.0.0/docs/requirementslib.models.setup_info.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-18 11:41:45.000000 requirementslib-3.0.0/docs/requirementslib.models.url.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-18 11:41:45.000000 requirementslib-3.0.0/docs/requirementslib.models.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-18 11:41:45.000000 requirementslib-3.0.0/docs/requirementslib.models.vcs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-18 11:41:45.000000 requirementslib-3.0.0/docs/requirementslib.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-18 11:41:45.000000 requirementslib-3.0.0/docs/requirementslib.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-18 11:41:45.000000 requirementslib-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-18 11:42:28.177332 requirementslib-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-18 11:41:45.000000 requirementslib-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:42:28.165331 requirementslib-3.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:42:28.169332 requirementslib-3.0.0/src/requirementslib/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-18 11:41:45.000000 requirementslib-3.0.0/src/requirementslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-18 11:41:45.000000 requirementslib-3.0.0/src/requirementslib/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-18 11:41:45.000000 requirementslib-3.0.0/src/requirementslib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10862 2023-06-18 11:41:45.000000 requirementslib-3.0.0/src/requirementslib/fileutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-18 11:41:45.000000 requirementslib-3.0.0/src/requirementslib/funktools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:42:28.173332 requirementslib-3.0.0/src/requirementslib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 11:41:45.000000 requirementslib-3.0.0/src/requirementslib/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-18 11:41:45.000000 requirementslib-3.0.0/src/requirementslib/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-18 11:41:45.000000 requirementslib-3.0.0/src/requirementslib/models/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-06-18 11:41:45.000000 requirementslib-3.0.0/src/requirementslib/models/lockfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-06-18 11:41:45.000000 requirementslib-3.0.0/src/requirementslib/models/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36642 2023-06-18 11:41:45.000000 requirementslib-3.0.0/src/requirementslib/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-06-18 11:41:45.000000 requirementslib-3.0.0/src/requirementslib/models/old_pip_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-06-18 11:41:45.000000 requirementslib-3.0.0/src/requirementslib/models/pipfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-18 11:41:45.000000 requirementslib-3.0.0/src/requirementslib/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109147 2023-06-18 11:41:45.000000 requirementslib-3.0.0/src/requirementslib/models/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61722 2023-06-18 11:41:45.000000 requirementslib-3.0.0/src/requirementslib/models/setup_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17937 2023-06-18 11:41:45.000000 requirementslib-3.0.0/src/requirementslib/models/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26802 2023-06-18 11:41:45.000000 requirementslib-3.0.0/src/requirementslib/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-18 11:41:45.000000 requirementslib-3.0.0/src/requirementslib/models/vcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27937 2023-06-18 11:41:45.000000 requirementslib-3.0.0/src/requirementslib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:42:28.173332 requirementslib-3.0.0/src/requirementslib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-06-18 11:42:28.000000 requirementslib-3.0.0/src/requirementslib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-18 11:42:28.000000 requirementslib-3.0.0/src/requirementslib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 11:42:28.000000 requirementslib-3.0.0/src/requirementslib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-18 11:42:28.000000 requirementslib-3.0.0/src/requirementslib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-18 11:42:28.000000 requirementslib-3.0.0/src/requirementslib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 11:41:49.000000 requirementslib-3.0.0/src/requirementslib.egg-info/zip-safe
```

### Comparing `requirementslib-2.3.1.dev0/CHANGELOG.rst` & `requirementslib-3.0.0/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/CONTRIBUTING.rst` & `requirementslib-3.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/LICENSE` & `requirementslib-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/MANIFEST.in` & `requirementslib-3.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/PKG-INFO` & `requirementslib-3.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requirementslib
-Version: 2.3.1.dev0
+Version: 3.0.0
 Summary: A tool for converting between pip-style and pipfile requirements.
 Home-page: https://github.com/sarugaku/requirementslib
 Author: Dan Ryan
 Author-email: dan@danryan.co
 Maintainer: Frost Ming
 Maintainer-email: mianghong@gmail.com
 License: MIT
```

### Comparing `requirementslib-2.3.1.dev0/README.rst` & `requirementslib-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/docs/Makefile` & `requirementslib-3.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/docs/conf.py` & `requirementslib-3.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/docs/make.bat` & `requirementslib-3.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/docs/requirementslib.models.rst` & `requirementslib-3.0.0/docs/requirementslib.models.rst`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/pyproject.toml` & `requirementslib-3.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/setup.cfg` & `requirementslib-3.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/setup.py` & `requirementslib-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/src/requirementslib/exceptions.py` & `requirementslib-3.0.0/src/requirementslib/exceptions.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/src/requirementslib/fileutils.py` & `requirementslib-3.0.0/src/requirementslib/fileutils.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/src/requirementslib/funktools.py` & `requirementslib-3.0.0/src/requirementslib/funktools.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/src/requirementslib/models/common.py` & `requirementslib-3.0.0/src/requirementslib/models/common.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/src/requirementslib/models/dependencies.py` & `requirementslib-3.0.0/src/requirementslib/models/dependencies.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/src/requirementslib/models/lockfile.py` & `requirementslib-3.0.0/src/requirementslib/models/lockfile.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/src/requirementslib/models/markers.py` & `requirementslib-3.0.0/src/requirementslib/models/markers.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/src/requirementslib/models/metadata.py` & `requirementslib-3.0.0/src/requirementslib/models/metadata.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/src/requirementslib/models/old_pip_utils.py` & `requirementslib-3.0.0/src/requirementslib/models/old_pip_utils.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/src/requirementslib/models/pipfile.py` & `requirementslib-3.0.0/src/requirementslib/models/pipfile.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/src/requirementslib/models/project.py` & `requirementslib-3.0.0/src/requirementslib/models/project.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/src/requirementslib/models/requirements.py` & `requirementslib-3.0.0/src/requirementslib/models/requirements.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/src/requirementslib/models/setup_info.py` & `requirementslib-3.0.0/src/requirementslib/models/setup_info.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/src/requirementslib/models/url.py` & `requirementslib-3.0.0/src/requirementslib/models/url.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/src/requirementslib/models/utils.py` & `requirementslib-3.0.0/src/requirementslib/models/utils.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/src/requirementslib/models/vcs.py` & `requirementslib-3.0.0/src/requirementslib/models/vcs.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/src/requirementslib/utils.py` & `requirementslib-3.0.0/src/requirementslib/utils.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.1.dev0/src/requirementslib.egg-info/PKG-INFO` & `requirementslib-3.0.0/src/requirementslib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requirementslib
-Version: 2.3.1.dev0
+Version: 3.0.0
 Summary: A tool for converting between pip-style and pipfile requirements.
 Home-page: https://github.com/sarugaku/requirementslib
 Author: Dan Ryan
 Author-email: dan@danryan.co
 Maintainer: Frost Ming
 Maintainer-email: mianghong@gmail.com
 License: MIT
```

### Comparing `requirementslib-2.3.1.dev0/src/requirementslib.egg-info/SOURCES.txt` & `requirementslib-3.0.0/src/requirementslib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

