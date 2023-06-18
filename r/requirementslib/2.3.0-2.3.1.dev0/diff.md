# Comparing `tmp/requirementslib-2.3.0.tar.gz` & `tmp/requirementslib-2.3.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requirementslib-2.3.0.tar", last modified: Sat Apr 29 03:45:44 2023, max compression
+gzip compressed data, was "requirementslib-2.3.1.dev0.tar", last modified: Sun Jun 18 11:26:36 2023, max compression
```

## Comparing `requirementslib-2.3.0.tar` & `requirementslib-2.3.1.dev0.tar`

### file list

```diff
@@ -1,65 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:45:44.483582 requirementslib-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35765 2023-04-29 03:45:07.000000 requirementslib-2.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-29 03:45:07.000000 requirementslib-2.3.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-29 03:45:07.000000 requirementslib-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-29 03:45:07.000000 requirementslib-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-04-29 03:45:44.483582 requirementslib-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11036 2023-04-29 03:45:07.000000 requirementslib-2.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:45:44.479582 requirementslib-2.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-29 03:45:07.000000 requirementslib-2.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-04-29 03:45:07.000000 requirementslib-2.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-29 03:45:07.000000 requirementslib-2.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-29 03:45:07.000000 requirementslib-2.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-29 03:45:07.000000 requirementslib-2.3.0/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-29 03:45:07.000000 requirementslib-2.3.0/docs/requirementslib.environment.rst
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-29 03:45:07.000000 requirementslib-2.3.0/docs/requirementslib.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-29 03:45:07.000000 requirementslib-2.3.0/docs/requirementslib.models.cache.rst
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-29 03:45:07.000000 requirementslib-2.3.0/docs/requirementslib.models.dependencies.rst
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-29 03:45:07.000000 requirementslib-2.3.0/docs/requirementslib.models.lockfile.rst
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-29 03:45:07.000000 requirementslib-2.3.0/docs/requirementslib.models.markers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-29 03:45:07.000000 requirementslib-2.3.0/docs/requirementslib.models.metadata.rst
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-29 03:45:07.000000 requirementslib-2.3.0/docs/requirementslib.models.pipfile.rst
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-29 03:45:07.000000 requirementslib-2.3.0/docs/requirementslib.models.project.rst
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-29 03:45:07.000000 requirementslib-2.3.0/docs/requirementslib.models.requirements.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-29 03:45:07.000000 requirementslib-2.3.0/docs/requirementslib.models.resolvers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-29 03:45:07.000000 requirementslib-2.3.0/docs/requirementslib.models.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-29 03:45:07.000000 requirementslib-2.3.0/docs/requirementslib.models.setup_info.rst
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-29 03:45:07.000000 requirementslib-2.3.0/docs/requirementslib.models.url.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-29 03:45:07.000000 requirementslib-2.3.0/docs/requirementslib.models.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-29 03:45:07.000000 requirementslib-2.3.0/docs/requirementslib.models.vcs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 03:45:07.000000 requirementslib-2.3.0/docs/requirementslib.rst
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-29 03:45:07.000000 requirementslib-2.3.0/docs/requirementslib.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-29 03:45:07.000000 requirementslib-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-29 03:45:44.483582 requirementslib-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-29 03:45:07.000000 requirementslib-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:45:44.471582 requirementslib-2.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:45:44.479582 requirementslib-2.3.0/src/requirementslib/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-29 03:45:07.000000 requirementslib-2.3.0/src/requirementslib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-29 03:45:07.000000 requirementslib-2.3.0/src/requirementslib/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-29 03:45:07.000000 requirementslib-2.3.0/src/requirementslib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-04-29 03:45:07.000000 requirementslib-2.3.0/src/requirementslib/fileutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-29 03:45:07.000000 requirementslib-2.3.0/src/requirementslib/funktools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:45:44.483582 requirementslib-2.3.0/src/requirementslib/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 03:45:07.000000 requirementslib-2.3.0/src/requirementslib/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-29 03:45:07.000000 requirementslib-2.3.0/src/requirementslib/models/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    26616 2023-04-29 03:45:07.000000 requirementslib-2.3.0/src/requirementslib/models/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-04-29 03:45:07.000000 requirementslib-2.3.0/src/requirementslib/models/lockfile.py
--rw-r--r--   0 runner    (1001) docker     (123)    26367 2023-04-29 03:45:07.000000 requirementslib-2.3.0/src/requirementslib/models/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)    44134 2023-04-29 03:45:07.000000 requirementslib-2.3.0/src/requirementslib/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-29 03:45:07.000000 requirementslib-2.3.0/src/requirementslib/models/old_pip_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-04-29 03:45:07.000000 requirementslib-2.3.0/src/requirementslib/models/pipfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-29 03:45:07.000000 requirementslib-2.3.0/src/requirementslib/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)   119684 2023-04-29 03:45:07.000000 requirementslib-2.3.0/src/requirementslib/models/requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-04-29 03:45:07.000000 requirementslib-2.3.0/src/requirementslib/models/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    66148 2023-04-29 03:45:07.000000 requirementslib-2.3.0/src/requirementslib/models/setup_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    18385 2023-04-29 03:45:07.000000 requirementslib-2.3.0/src/requirementslib/models/url.py
--rw-r--r--   0 runner    (1001) docker     (123)    34664 2023-04-29 03:45:07.000000 requirementslib-2.3.0/src/requirementslib/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-04-29 03:45:07.000000 requirementslib-2.3.0/src/requirementslib/models/vcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27937 2023-04-29 03:45:07.000000 requirementslib-2.3.0/src/requirementslib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:45:44.479582 requirementslib-2.3.0/src/requirementslib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-04-29 03:45:44.000000 requirementslib-2.3.0/src/requirementslib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-29 03:45:44.000000 requirementslib-2.3.0/src/requirementslib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 03:45:44.000000 requirementslib-2.3.0/src/requirementslib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-29 03:45:44.000000 requirementslib-2.3.0/src/requirementslib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-29 03:45:44.000000 requirementslib-2.3.0/src/requirementslib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 03:45:12.000000 requirementslib-2.3.0/src/requirementslib.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:26:36.551856 requirementslib-2.3.1.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35908 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-06-18 11:26:36.551856 requirementslib-2.3.1.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11036 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:26:36.547856 requirementslib-2.3.1.dev0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.environment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.models.cache.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.models.dependencies.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.models.lockfile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.models.markers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.models.metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.models.pipfile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.models.project.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.models.requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.models.resolvers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.models.setup_info.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.models.url.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.models.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.models.vcs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/docs/requirementslib.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-18 11:26:36.551856 requirementslib-2.3.1.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:26:36.543856 requirementslib-2.3.1.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:26:36.547856 requirementslib-2.3.1.dev0/src/requirementslib/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10862 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/fileutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/funktools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:26:36.551856 requirementslib-2.3.1.dev0/src/requirementslib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/models/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/models/lockfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/models/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36642 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/models/old_pip_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/models/pipfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109147 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/models/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61722 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/models/setup_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17937 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/models/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26802 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/models/vcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27937 2023-06-18 11:26:01.000000 requirementslib-2.3.1.dev0/src/requirementslib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:26:36.547856 requirementslib-2.3.1.dev0/src/requirementslib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-06-18 11:26:36.000000 requirementslib-2.3.1.dev0/src/requirementslib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-18 11:26:36.000000 requirementslib-2.3.1.dev0/src/requirementslib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 11:26:36.000000 requirementslib-2.3.1.dev0/src/requirementslib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-18 11:26:36.000000 requirementslib-2.3.1.dev0/src/requirementslib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-18 11:26:36.000000 requirementslib-2.3.1.dev0/src/requirementslib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 11:26:05.000000 requirementslib-2.3.1.dev0/src/requirementslib.egg-info/zip-safe
```

### Comparing `requirementslib-2.3.0/CHANGELOG.rst` & `requirementslib-2.3.1.dev0/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Requirementslib 3.0.0 (2023-06-18)
+==================================
+
+ * Drop attrs lib and replace with pydantic.
+ * Remove unused modules.
+
 Requirementslib 2.3.0 (2023-04-28)
 ==================================
 
 
 No significant changes.
```

### Comparing `requirementslib-2.3.0/CONTRIBUTING.rst` & `requirementslib-2.3.1.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.0/LICENSE` & `requirementslib-2.3.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.0/MANIFEST.in` & `requirementslib-2.3.1.dev0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.0/PKG-INFO` & `requirementslib-2.3.1.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requirementslib
-Version: 2.3.0
+Version: 2.3.1.dev0
 Summary: A tool for converting between pip-style and pipfile requirements.
 Home-page: https://github.com/sarugaku/requirementslib
 Author: Dan Ryan
 Author-email: dan@danryan.co
 Maintainer: Frost Ming
 Maintainer-email: mianghong@gmail.com
 License: MIT
```

### Comparing `requirementslib-2.3.0/README.rst` & `requirementslib-2.3.1.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.0/docs/Makefile` & `requirementslib-2.3.1.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.0/docs/conf.py` & `requirementslib-2.3.1.dev0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.0/docs/make.bat` & `requirementslib-2.3.1.dev0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.0/docs/requirementslib.models.rst` & `requirementslib-2.3.1.dev0/docs/requirementslib.models.rst`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.0/pyproject.toml` & `requirementslib-2.3.1.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.0/setup.cfg` & `requirementslib-2.3.1.dev0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -37,20 +37,20 @@
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: Utilities
 
 [options]
 zip_safe = true
 python_requires = >=3.7
 install_requires = 
-	attrs>=19.2
 	distlib>=0.2.8
 	pep517>=0.5.0
 	pip>=23.1
 	platformdirs
 	plette[validation]
+	pydantic
 	requests
 	setuptools>=40.8
 	tomlkit>=0.5.3
 
 [options.extras_require]
 tests = 
 	pytest
```

### Comparing `requirementslib-2.3.0/setup.py` & `requirementslib-2.3.1.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.0/src/requirementslib/exceptions.py` & `requirementslib-2.3.1.dev0/src/requirementslib/exceptions.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.0/src/requirementslib/fileutils.py` & `requirementslib-2.3.1.dev0/src/requirementslib/fileutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,41 +87,30 @@
         BUFFER_SIZE = 500
         buffer = create_unicode_buffer(BUFFER_SIZE)
         get_long_path_name = windll.kernel32.GetLongPathNameW
         get_long_path_name(short_path, buffer, BUFFER_SIZE)
         return buffer.value
 
 
-def normalize_path(path):
-    """Return a case-normalized absolute variable-expanded path.
-
-    :param str path: The non-normalized path
-    :return: A normalized, expanded, case-normalized path
-    :rtype: str
-    """
-
-    path = os.path.abspath(os.path.expandvars(os.path.expanduser(str(path))))
-    if os.name == "nt" and os.path.exists(path):
-
-        path = get_long_path(path)
-
-    return os.path.normpath(os.path.normcase(path))
+def normalize_path(path: str) -> str:
+    """Return a case-normalized absolute variable-expanded path."""
+    return os.path.expandvars(
+        os.path.expanduser(os.path.normcase(os.path.normpath(os.path.abspath(str(path)))))
+    )
 
 
 def normalize_drive(path):
     """Normalize drive in path so they stay consistent.
 
     This currently only affects local drives on Windows, which can be
     identified with either upper or lower cased drive names. The case is
     always converted to uppercase because it seems to be preferred.
     """
-    if os.name != "nt" or not (
-        isinstance(path, str) or getattr(path, "__fspath__", None)
-    ):
-        return path  # type: ignore
+    if os.name != "nt" or not isinstance(path, str):
+        return path
 
     drive, tail = os.path.splitdrive(path)
     # Only match (lower cased) local drives (e.g. 'c:'), not UNC mounts.
     if drive.islower() and len(drive) == 2 and drive[1] == ":":
         return f"{drive.upper()}{tail}"
 
     return path
```

### Comparing `requirementslib-2.3.0/src/requirementslib/funktools.py` & `requirementslib-2.3.1.dev0/src/requirementslib/funktools.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.0/src/requirementslib/models/dependencies.py` & `requirementslib-2.3.1.dev0/src/requirementslib/models/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,692 +1,788 @@
-import atexit
-import contextlib
-import copy
-import functools
 import os
-from json import JSONDecodeError
+import re
+import string
+from functools import lru_cache
+from pathlib import Path
+from typing import (
+    Any,
+    AnyStr,
+    Dict,
+    List,
+    Match,
+    Optional,
+    Set,
+    Text,
+    Tuple,
+    TypeVar,
+    Union,
+)
 
-import attr
-import requests
-from pip._internal.cache import WheelCache
-from pip._internal.operations.build.build_tracker import get_build_tracker
+import tomlkit as tomlkit
+from pip._internal.models.link import Link
 from pip._internal.req.constructors import install_req_from_line
-from pip._internal.req.req_install import InstallRequirement
-from pip._internal.req.req_set import RequirementSet
-from pip._internal.utils.temp_dir import TempDirectory, global_tempdir_manager
-from pip._vendor.packaging.markers import Marker
+from pip._internal.utils._jaraco_text import drop_comment, join_continuation, yield_lines
+from pip._vendor.packaging.markers import InvalidMarker, Marker, Op, Value, Variable
+from pip._vendor.packaging.requirements import Requirement as PackagingRequirement
+from pip._vendor.packaging.specifiers import InvalidSpecifier, Specifier, SpecifierSet
 from pip._vendor.packaging.utils import canonicalize_name
-from pip._vendor.packaging.version import parse
+from pip._vendor.packaging.version import parse as parse_version
+from pip._vendor.pkg_resources import Requirement, get_distribution, safe_name
+from pip._vendor.urllib3 import util as urllib3_util
+from pip._vendor.urllib3.util import parse_url as urllib3_parse
+from plette.models import Package, PackageCollection
+from tomlkit.container import Container
+from tomlkit.items import AoT, Array, Bool, InlineTable, Item, String, Table
 
 from ..environment import MYPY_RUNNING
-from ..fileutils import create_tracked_tempdir
-from ..utils import (
-    get_package_finder,
-    get_pip_command,
-    prepare_pip_source_args,
-    temp_environ,
-)
-from .cache import CACHE_DIR, DependencyCache
-from .setup_info import SetupInfo
-from .utils import (
-    clean_requires_python,
-    format_requirement,
-    full_groupby,
-    is_pinned_requirement,
-    key_from_ireq,
-    make_install_requirement,
-    name_from_req,
-    version_from_ireq,
-)
+from ..fileutils import is_valid_url
+from ..utils import VCS_LIST, is_star
 
 if MYPY_RUNNING:
-    from typing import Any, Dict, List, Optional, Set, Text, TypeVar, Union
-
-    from pip._internal.commands import Command
-    from pip._internal.index.package_finder import PackageFinder
-    from pip._internal.models.candidate import InstallationCandidate
-    from pip._vendor.packaging.requirements import Requirement as PackagingRequirement
-
-    TRequirement = TypeVar("TRequirement")
-    RequirementType = TypeVar(
-        "RequirementType", covariant=True, bound=PackagingRequirement
-    )
-    MarkerType = TypeVar("MarkerType", covariant=True, bound=Marker)
-    STRING_TYPE = Union[str, bytes, Text]
+    from pip._vendor.packaging.markers import Marker as PkgResourcesMarker
+    from pip._vendor.packaging.markers import Op as PkgResourcesOp
+    from pip._vendor.packaging.markers import Value as PkgResourcesValue
+    from pip._vendor.packaging.markers import Variable as PkgResourcesVariable
+    from pip._vendor.urllib3.util.url import Url
+
+    _T = TypeVar("_T")
+    TMarker = Union[Marker, PkgResourcesMarker]
+    TVariable = TypeVar("TVariable", PkgResourcesVariable, Variable)
+    TValue = TypeVar("TValue", PkgResourcesValue, Value)
+    TOp = TypeVar("TOp", PkgResourcesOp, Op)
+    MarkerTuple = Tuple[TVariable, TOp, TValue]
+    TRequirement = Union[PackagingRequirement, Requirement]
+    STRING_TYPE = Union[bytes, str, Text]
+    TOML_DICT_TYPES = Union[Container, Package, PackageCollection, Table, InlineTable]
     S = TypeVar("S", bytes, str, Text)
 
 
-PKGS_DOWNLOAD_DIR = os.path.join(CACHE_DIR, "pkgs")
-WHEEL_DOWNLOAD_DIR = os.path.join(CACHE_DIR, "wheels")
+TOML_DICT_OBJECTS = (Container, Package, Table, InlineTable, PackageCollection)
+TOML_DICT_NAMES = [o.__class__.__name__ for o in TOML_DICT_OBJECTS]
+
+HASH_STRING = " --hash={0}"
+
+ALPHA_NUMERIC = r"[{0}{1}]".format(string.ascii_letters, string.digits)
+PUNCTUATION = r"[\-_\.]"
+ALPHANUM_PUNCTUATION = r"[{0}{1}\-_\.]".format(string.ascii_letters, string.digits)
+NAME = r"{0}+{1}*{2}".format(ALPHANUM_PUNCTUATION, PUNCTUATION, ALPHA_NUMERIC)
+REF = r"[{0}{1}\-\_\./]".format(string.ascii_letters, string.digits)
+EXTRAS = r"(?P<extras>\[{0}(?:,{0})*\])".format(NAME)
+NAME_WITH_EXTRAS = r"(?P<name>{0}){1}?".format(NAME, EXTRAS)
+NAME_RE = re.compile(NAME_WITH_EXTRAS)
+SUBDIR_RE = r"(?:[&#]subdirectory=(?P<subdirectory>.*))"
+URL_NAME = r"(?:#egg={0})".format(NAME_WITH_EXTRAS)
+REF_RE = r"(?:@(?P<ref>{0}+)?)".format(REF)
+PATH_RE = r"(?P<pathsep>[:/])(?P<path>[^ @]+){0}?".format(REF_RE)
+PASS_RE = r"(?:(?<=:)(?P<password>[^ ]+))"
+AUTH_RE = r"(?:(?P<username>[^ ]+)[:@]{0}?@)".format(PASS_RE)
+HOST_RE = r"(?:{0}?(?P<host>[^ ]+?\.?{1}+(?P<port>:\d+)?))?".format(
+    AUTH_RE, ALPHA_NUMERIC
+)
+URL = r"(?P<scheme>[^ ]+://){0}{1}".format(HOST_RE, PATH_RE)
+URL_RE = re.compile(r"{0}(?:{1}?{2}?)?".format(URL, URL_NAME, SUBDIR_RE))
+DIRECT_URL_RE = re.compile(r"{0}\s?@\s?{1}".format(NAME_WITH_EXTRAS, URL))
+
+
+def filter_none(k, v) -> bool:
+    if v:
+        return True
+    return False
+
+
+def filter_dict(dict_) -> Dict[AnyStr, Any]:
+    return {k: v for k, v in dict_.items() if filter_none(k, v)}
+
+
+def create_link(link):
+    # type: (AnyStr) -> Link
+
+    if not isinstance(link, str):
+        raise TypeError("must provide a string to instantiate a new link")
+
+    return Link(link)
+
+
+def tomlkit_value_to_python(toml_value):
+    # type: (Union[Array, AoT, TOML_DICT_TYPES, Item]) -> Union[List, Dict]
+    value_type = type(toml_value).__name__
+    if (
+        isinstance(toml_value, TOML_DICT_OBJECTS + (dict,))
+        or value_type in TOML_DICT_NAMES
+    ):
+        return tomlkit_dict_to_python(toml_value)
+    elif isinstance(toml_value, AoT) or value_type == "AoT":
+        return [tomlkit_value_to_python(val) for val in toml_value._body]
+    elif isinstance(toml_value, Array) or value_type == "Array":
+        return [tomlkit_value_to_python(val) for val in list(toml_value)]
+    elif isinstance(toml_value, String) or value_type == "String":
+        return "{0!s}".format(toml_value)
+    elif isinstance(toml_value, Bool) or value_type == "Bool":
+        return toml_value.value
+    elif isinstance(toml_value, Item):
+        return toml_value.value
+    return toml_value
+
+
+def tomlkit_dict_to_python(toml_dict):
+    # type: (TOML_DICT_TYPES) -> Dict
+    value_type = type(toml_dict).__name__
+    if toml_dict is None:
+        raise TypeError("Invalid type NoneType when converting toml dict to python")
+    converted = None  # type: Optional[Dict]
+    if isinstance(toml_dict, (InlineTable, Table)) or value_type in (
+        "InlineTable",
+        "Table",
+    ):
+        converted = toml_dict.value
+    elif isinstance(toml_dict, (Package, PackageCollection)) or value_type in (
+        "Package, PackageCollection"
+    ):
+        converted = toml_dict._data
+        if isinstance(converted, Container) or type(converted).__name__ == "Container":
+            converted = converted.value
+    elif isinstance(toml_dict, Container) or value_type == "Container":
+        converted = toml_dict.value
+    elif isinstance(toml_dict, dict):
+        converted = toml_dict.copy()
+    else:
+        raise TypeError(
+            "Invalid type for conversion: expected Container, Dict, or Table, "
+            "got {0!r}".format(toml_dict)
+        )
+    if isinstance(converted, dict):
+        return {k: tomlkit_value_to_python(v) for k, v in converted.items()}
+    elif isinstance(converted, (TOML_DICT_OBJECTS)) or value_type in TOML_DICT_NAMES:
+        return tomlkit_dict_to_python(converted)
+    return converted
 
-DEPENDENCY_CACHE = DependencyCache()
 
+def get_url_name(url):
+    # type: (AnyStr) -> AnyStr
+    """Given a url, derive an appropriate name to use in a pipfile.
+
+    :param str url: A url to derive a string from
+    :returns: The name of the corresponding pipfile entry
+    :rtype: Text
+    """
+    if not isinstance(url, str):
+        raise TypeError("Expected a string, got {0!r}".format(url))
+    return urllib3_util.parse_url(url).host
 
-@contextlib.contextmanager
-def _get_wheel_cache():
-    with global_tempdir_manager():
-        yield WheelCache(CACHE_DIR)
-
-
-def _get_filtered_versions(ireq, versions, prereleases):
-    return set(ireq.specifier.filter(versions, prereleases=prereleases))
-
-
-def find_all_matches(finder, ireq, pre=False):
-    # type: (PackageFinder, InstallRequirement, bool) -> List[InstallationCandidate]
-    """Find all matching dependencies using the supplied finder and the given
-    ireq.
-
-    :param finder: A package finder for discovering matching candidates.
-    :type finder: :class:`~pip._internal.index.PackageFinder`
-    :param ireq: An install requirement.
-    :type ireq: :class:`~pip._internal.req.req_install.InstallRequirement`
-    :return: A list of matching candidates.
-    :rtype: list[:class:`~pip._internal.index.InstallationCandidate`]
-    """
-
-    candidates = clean_requires_python(finder.find_all_candidates(ireq.name))
-    versions = {candidate.version for candidate in candidates}
-    allowed_versions = _get_filtered_versions(ireq, versions, pre)
-    if not pre and not allowed_versions:
-        allowed_versions = _get_filtered_versions(ireq, versions, True)
-    candidates = {c for c in candidates if c.version in allowed_versions}
-    return candidates
-
-
-@attr.s
-class AbstractDependency(object):
-    name = attr.ib()  # type: STRING_TYPE
-    specifiers = attr.ib()
-    markers = attr.ib()
-    candidates = attr.ib()
-    requirement = attr.ib()
-    parent = attr.ib()
-    finder = attr.ib()
-    dep_dict = attr.ib(default=attr.Factory(dict))
-
-    @property
-    def version_set(self):
-        """Return the set of versions for the candidates in this abstract
-        dependency.
-
-        :return: A set of matching versions
-        :rtype: set(str)
-        """
-
-        if len(self.candidates) == 1:
-            return set()
-        return set(parse(version_from_ireq(c)) for c in self.candidates)
-
-    def compatible_versions(self, other):
-        """Find compatible version numbers between this abstract dependency and
-        another one.
-
-        :param other: An abstract dependency to compare with.
-        :type other: :class:`~requirementslib.models.dependency.AbstractDependency`
-        :return: A set of compatible version strings
-        :rtype: set(str)
-        """
-
-        if len(self.candidates) == 1 and next(iter(self.candidates)).editable:
-            return self
-        elif len(other.candidates) == 1 and next(iter(other.candidates)).editable:
-            return other
-        return self.version_set & other.version_set
-
-    def compatible_abstract_dep(self, other):
-        """Merge this abstract dependency with another one.
-
-        Return the result of the merge as a new abstract dependency.
-
-        :param other: An abstract dependency to merge with
-        :type other: :class:`~requirementslib.models.dependency.AbstractDependency`
-        :return: A new, combined abstract dependency
-        :rtype: :class:`~requirementslib.models.dependency.AbstractDependency`
-        """
-
-        from .requirements import Requirement
-
-        if len(self.candidates) == 1 and next(iter(self.candidates)).editable:
-            return self
-        elif len(other.candidates) == 1 and next(iter(other.candidates)).editable:
-            return other
-        new_specifiers = self.specifiers & other.specifiers
-        markers = set(self.markers) if self.markers else set()
-        if other.markers:
-            markers.add(other.markers)
-        new_markers = None
-        if markers:
-            new_markers = Marker(" or ".join(str(m) for m in sorted(markers)))
-        new_ireq = copy.deepcopy(self.requirement.ireq)
-        new_ireq.req.specifier = new_specifiers
-        new_ireq.req.marker = new_markers
-        new_requirement = Requirement.from_line(format_requirement(new_ireq))
-        compatible_versions = self.compatible_versions(other)
-        if isinstance(compatible_versions, AbstractDependency):
-            return compatible_versions
-        candidates = [
-            c
-            for c in self.candidates
-            if parse(version_from_ireq(c)) in compatible_versions
-        ]
-        dep_dict = {}
-        candidate_strings = [format_requirement(c) for c in candidates]
-        for c in candidate_strings:
-            if c in self.dep_dict:
-                dep_dict[c] = self.dep_dict.get(c)
-        return AbstractDependency(
-            name=self.name,
-            specifiers=new_specifiers,
-            markers=new_markers,
-            candidates=candidates,
-            requirement=new_requirement,
-            parent=self.parent,
-            dep_dict=dep_dict,
-            finder=self.finder,
+
+class HashableRequirement(Requirement):
+    def __hash__(self):
+        specifier_hash = hash(tuple((str(s),) for s in self.specifier))
+        return hash(
+            (
+                self.url,
+                specifier_hash,
+                frozenset(self.extras),
+                str(self.marker) if self.marker else None,
+            )
         )
 
-    def get_deps(self, candidate):
-        """Get the dependencies of the supplied candidate.
+    @staticmethod
+    def parse(s):
+        (req,) = map(
+            HashableRequirement, join_continuation(map(drop_comment, yield_lines(s)))
+        )
+        return req
 
-        :param candidate: An installrequirement
-        :type candidate: :class:`~pip._internal.req.req_install.InstallRequirement`
-        :return: A list of abstract dependencies
-        :rtype: list[:class:`~requirementslib.models.dependency.AbstractDependency`]
-        """
-
-        key = format_requirement(candidate)
-        if key not in self.dep_dict:
-            from .requirements import Requirement
-
-            req = Requirement.from_line(key)
-            req = req.merge_markers(self.markers)
-            self.dep_dict[key] = req.abstract_dependencies()
-        return self.dep_dict[key]
-
-    @classmethod
-    def from_requirement(cls, requirement, parent=None):
-        """Creates a new
-        :class:`~requirementslib.models.dependency.AbstractDependency` from a
-        :class:`~requirementslib.models.requirements.Requirement` object.
-
-        This class is used to find all candidates matching a given set of specifiers
-        and a given requirement.
-
-        :param requirement: A requirement for resolution
-        :type requirement: :class:`~requirementslib.models.requirements.Requirement` object.
-        """
-        name = requirement.normalized_name
-        specifiers = requirement.ireq.specifier if not requirement.editable else ""
-        markers = requirement.ireq.markers
-        extras = requirement.ireq.extras
-        is_pinned = is_pinned_requirement(requirement.ireq)
-        is_constraint = bool(parent)
-        _, finder = get_finder(sources=None)
-        candidates = []
-        if not is_pinned and not requirement.editable:
-            for r in requirement.find_all_matches(finder=finder):
-                req = make_install_requirement(
-                    name,
-                    r.version,
-                    extras=extras,
-                    markers=markers,
-                    constraint=is_constraint,
-                )
-                req.req.link = getattr(r, "location", getattr(r, "link", None))
-                req.parent = parent
-                candidates.append(req)
-                candidates = sorted(
-                    set(candidates),
-                    key=lambda k: parse(version_from_ireq(k)),
-                )
+
+def init_requirement(name):
+    if not isinstance(name, str):
+        raise TypeError("must supply a name to generate a requirement")
+
+    req = HashableRequirement.parse(name)
+    req.vcs = None
+    req.local_file = None
+    req.revision = None
+    req.path = None
+    return req
+
+
+def convert_to_hashable_requirement(req: Requirement) -> Optional[HashableRequirement]:
+    if req is None:
+        return None
+
+    hashable_req = HashableRequirement(str(req))
+    hashable_req.extras = req.extras
+    hashable_req.marker = req.marker
+    hashable_req.url = req.url
+    return hashable_req
+
+
+def extras_to_string(extras) -> str:
+    """Turn a list of extras into a string."""
+    if isinstance(extras, str):
+        if extras.startswith("["):
+            return extras
         else:
-            candidates = [requirement.ireq]
-        return cls(
-            name=name,
-            specifiers=specifiers,
-            markers=markers,
-            candidates=candidates,
-            requirement=requirement,
-            parent=parent,
-            finder=finder,
+            extras = [extras]
+    if not extras:
+        return ""
+    return "[{0}]".format(",".join(sorted(set(extras))))
+
+
+def parse_extras_str(extras_str):
+    """Turn a string of extras into a parsed extras list.
+
+    :param str extras_str: An extras string
+    :return: A sorted list of extras
+    :rtype: List[str]
+    """
+    extras = Requirement.parse("fakepkg{0}".format(extras_to_string(extras_str))).extras
+    return sorted(dict.fromkeys([extra.lower() for extra in extras]))
+
+
+def parse_extras_from_line(installable_line):
+    extras = []
+
+    # Extract the part within square brackets, if any
+    start = installable_line.find("[")
+    end = installable_line.find("]")
+
+    if start != -1 and end != -1 and start < end:
+        extras_str = installable_line[start + 1 : end]
+        extras = extras_str.split(",")
+
+    return extras
+
+
+def specs_to_string(specs):
+    # type: (List[Union[STRING_TYPE, Specifier]]) -> AnyStr
+    """Turn a list of specifier tuples into a string.
+
+    :param List[Union[Specifier, str]] specs: a list of specifiers to format
+    :return: A string of specifiers
+    :rtype: str
+    """
+
+    if specs:
+        if isinstance(specs, str):
+            return specs
+        try:
+            extras = ",".join(["".join(spec) for spec in specs])
+        except TypeError:
+            extras = ",".join(["".join(spec._spec) for spec in specs])  # type: ignore
+        return extras
+    return ""
+
+
+def build_vcs_uri(
+    vcs,
+    uri,
+    name=None,
+    ref=None,
+    subdirectory=None,
+    extras=None,
+):
+    # type: (...) -> STRING_TYPE
+    if extras is None:
+        extras = []
+    vcs_start = ""
+    if vcs is not None:
+        vcs_start = "{0}+".format(vcs)
+        if not uri.startswith(vcs_start):
+            uri = "{0}{1}".format(vcs_start, uri)
+    if ref:
+        uri = "{0}@{1}".format(uri, ref)
+    if name:
+        uri = "{0}#egg={1}".format(uri, name)
+        if extras:
+            extras_string = extras_to_string(extras)
+            uri = "{0}{1}".format(uri, extras_string)
+    if subdirectory:
+        uri = "{0}&subdirectory={1}".format(uri, subdirectory)
+    return uri
+
+
+def _get_parsed_url(url):
+    # type: (S) -> Url
+    """This is a stand-in function for `urllib3.util.parse_url`
+
+    The original function doesn't handle special characters very well, this simply splits
+    out the authentication section, creates the parsed url, then puts the authentication
+    section back in, bypassing validation.
+
+    :return: The new, parsed URL object
+    :rtype: :class:`~urllib3.util.url.Url`
+    """
+
+    try:
+        parsed = urllib3_parse(url)
+    except ValueError:
+        scheme, _, url = url.partition("://")
+        auth, _, url = url.rpartition("@")
+        url = "{scheme}://{url}".format(scheme=scheme, url=url)
+        parsed = urllib3_parse(url)._replace(auth=auth)
+    return parsed
+
+
+def convert_direct_url_to_url(direct_url):
+    # type: (AnyStr) -> AnyStr
+    """Converts direct URLs to standard, link-style URLs.
+
+    Given a direct url as defined by *PEP 508*, convert to a :class:`Link`
+    compatible URL by moving the name and extras into an **egg_fragment**.
+
+    :param str direct_url: A pep-508 compliant direct url.
+    :return: A reformatted URL for use with Link objects and :class:`InstallRequirement` objects.
+    :rtype: AnyStr
+    """
+    direct_match = DIRECT_URL_RE.match(direct_url)  # type: Optional[Match]
+    if direct_match is None:
+        url_match = URL_RE.match(direct_url)
+        if url_match or is_valid_url(direct_url):
+            return direct_url
+    match_dict = (
+        {}
+    )  # type: Dict[STRING_TYPE, Union[Tuple[STRING_TYPE, ...], STRING_TYPE]]
+    if direct_match is not None:
+        match_dict = direct_match.groupdict()  # type: ignore
+    if not match_dict:
+        raise ValueError(
+            "Failed converting value to normal URL, is it a direct URL? {0!r}".format(
+                direct_url
+            )
         )
+    url_segments = [match_dict.get(s) for s in ("scheme", "host", "path", "pathsep")]
+    url = ""  # type: STRING_TYPE
+    url = "".join([s for s in url_segments if s is not None])  # type: ignore
+    new_url = build_vcs_uri(
+        None,
+        url,
+        ref=match_dict.get("ref"),
+        name=match_dict.get("name"),
+        extras=match_dict.get("extras"),
+        subdirectory=match_dict.get("subdirectory"),
+    )
+    return new_url
+
+
+def get_version(pipfile_entry):
+    if str(pipfile_entry) == "{}" or is_star(pipfile_entry):
+        return ""
 
-    @classmethod
-    def from_string(cls, line, parent=None):
-        from .requirements import Requirement
-
-        req = Requirement.from_line(line)
-        abstract_dep = cls.from_requirement(req, parent=parent)
-        return abstract_dep
-
-
-def get_abstract_dependencies(reqs, parent=None):
-    """Get all abstract dependencies for a given list of requirements.
-
-    Given a set of requirements, convert each requirement to an Abstract Dependency.
-
-    :param reqs: A list of Requirements
-    :type reqs: list[:class:`~requirementslib.models.requirements.Requirement`]
-    :param parent: The parent of this list of dependencies, defaults to None
-    :param parent: :class:`~requirementslib.models.requirements.Requirement`, optional
-    :return: A list of Abstract Dependencies
-    :rtype: list[:class:`~requirementslib.models.dependency.AbstractDependency`]
-    """
-    deps = []
-    from .requirements import Requirement
-
-    for req in reqs:
-        if isinstance(req, InstallRequirement):
-            requirement = Requirement.from_line("{0}{1}".format(req.name, req.specifier))
-            if req.link:
-                requirement.req.link = req.link
-                requirement.markers = req.markers
-                requirement.req.markers = req.markers
-                requirement.extras = req.extras
-                requirement.req.extras = req.extras
-        elif isinstance(req, Requirement):
-            requirement = copy.deepcopy(req)
+    if hasattr(pipfile_entry, "keys") and "version" in pipfile_entry:
+        if is_star(pipfile_entry.get("version")):
+            return ""
+        version = pipfile_entry.get("version")
+        if version is None:
+            version = ""
+        return version.strip().lstrip("(").rstrip(")")
+
+    if isinstance(pipfile_entry, str):
+        return pipfile_entry.strip().lstrip("(").rstrip(")")
+    return ""
+
+
+def strip_extras_markers_from_requirement(req):
+    # type: (TRequirement) -> TRequirement
+    """Strips extras markers from requirement instances.
+
+    Given a :class:`~packaging.requirements.Requirement` instance with markers defining
+    *extra == 'name'*, strip out the extras from the markers and return the cleaned
+    requirement
+
+    :param PackagingRequirement req: A packaging requirement to clean
+    :return: A cleaned requirement
+    :rtype: PackagingRequirement
+    """
+    if req is None:
+        raise TypeError("Must pass in a valid requirement, received {0!r}".format(req))
+    if getattr(req, "marker", None) is not None:
+        marker = req.marker  # type: TMarker
+        marker._markers = _strip_extras_markers(marker._markers)
+        if not marker._markers:
+            req.marker = None
         else:
-            requirement = Requirement.from_line(req)
-        dep = AbstractDependency.from_requirement(requirement, parent=parent)
-        deps.append(dep)
-    return deps
-
-
-def get_dependencies(ireq, sources=None, parent=None):
-    # type: (Union[InstallRequirement, InstallationCandidate], Optional[List[Dict[S, Union[S, bool]]]], Optional[AbstractDependency]) -> Set[S, ...]
-    """Get all dependencies for a given install requirement.
-
-    :param ireq: A single InstallRequirement
-    :type ireq: :class:`~pip._internal.req.req_install.InstallRequirement`
-    :param sources: Pipfile-formatted sources, defaults to None
-    :type sources: list[dict], optional
-    :param parent: The parent of this list of dependencies, defaults to None
-    :type parent: :class:`~pip._internal.req.req_install.InstallRequirement`
-    :return: A set of dependency lines for generating new InstallRequirements.
-    :rtype: set(str)
-    """
-    if not isinstance(ireq, InstallRequirement):
-        name = getattr(ireq, "project_name", getattr(ireq, "project", ireq.name))
-        version = getattr(ireq, "version", None)
-        if not version:
-            ireq = install_req_from_line("{0}".format(name))
+            req.marker = marker
+    return req
+
+
+def _strip_extras_markers(marker):
+    # type: (Union[MarkerTuple, List[Union[MarkerTuple, str]]]) -> List[Union[MarkerTuple, str]]
+    if marker is None or not isinstance(marker, (list, tuple)):
+        raise TypeError("Expecting a marker type, received {0!r}".format(marker))
+    markers_to_remove = []
+    # iterate forwards and generate a list of indexes to remove first, then reverse the
+    # list so we can remove the text that normally occurs after (but we will already
+    # be past it in the loop)
+    for i, marker_list in enumerate(marker):
+        if isinstance(marker_list, list):
+            cleaned = _strip_extras_markers(marker_list)
+            if not cleaned:
+                markers_to_remove.append(i)
+        elif isinstance(marker_list, tuple) and marker_list[0].value == "extra":
+            markers_to_remove.append(i)
+    for i in reversed(markers_to_remove):
+        del marker[i]
+        if i > 0 and marker[i - 1] == "and":
+            del marker[i - 1]
+    return marker
+
+
+@lru_cache()
+def get_setuptools_version():
+    # type: () -> Optional[STRING_TYPE]
+
+    setuptools_dist = get_distribution(Requirement("setuptools"))
+    return getattr(setuptools_dist, "version", None)
+
+
+def get_default_pyproject_backend():
+    # type: () -> STRING_TYPE
+    st_version = get_setuptools_version()
+    if st_version is not None:
+        parsed_st_version = parse_version(st_version)
+        if parsed_st_version >= parse_version("40.8.0"):
+            return "setuptools.build_meta:__legacy__"
+    return "setuptools.build_meta"
+
+
+def get_pyproject(path):
+    # type: (Union[STRING_TYPE, Path]) -> Optional[Tuple[List[STRING_TYPE], STRING_TYPE]]
+    """Given a base path, look for the corresponding ``pyproject.toml`` file
+    and return its build_requires and build_backend.
+
+    :param AnyStr path: The root path of the project, should be a directory (will be truncated)
+    :return: A 2 tuple of build requirements and the build backend
+    :rtype: Optional[Tuple[List[AnyStr], AnyStr]]
+    """
+    if not path:
+        return
+
+    if not isinstance(path, Path):
+        path = Path(path)
+    if not path.is_dir():
+        path = path.parent
+    pp_toml = path.joinpath("pyproject.toml")
+    setup_py = path.joinpath("setup.py")
+    if not pp_toml.exists():
+        if not setup_py.exists():
+            return None
+        requires = ["setuptools>=40.8", "wheel"]
+        backend = get_default_pyproject_backend()
+    else:
+        pyproject_data = {}
+        with open(pp_toml.as_posix(), encoding="utf-8") as fh:
+            pyproject_data = tomlkit.loads(fh.read())
+        build_system = pyproject_data.get("build-system", None)
+        if build_system is None:
+            if setup_py.exists():
+                requires = ["setuptools>=40.8", "wheel"]
+                backend = get_default_pyproject_backend()
+            else:
+                requires = ["setuptools>=40.8", "wheel"]
+                backend = get_default_pyproject_backend()
+            build_system = {"requires": requires, "build-backend": backend}
+            pyproject_data["build_system"] = build_system
         else:
-            ireq = install_req_from_line("{0}=={1}".format(name, version))
-    getters = [
-        get_dependencies_from_cache,
-        get_dependencies_from_wheel_cache,
-        get_dependencies_from_json,
-        functools.partial(get_dependencies_from_index, sources=sources),
-    ]
-    for getter in getters:
-        deps = getter(ireq)
-        if deps is not None:
-            return deps
-    raise RuntimeError("failed to get dependencies for {}".format(ireq))
-
-
-def get_dependencies_from_wheel_cache(ireq):
-    # type: (InstallRequirement) -> Optional[Set[InstallRequirement]]
-    """Retrieves dependencies for the given install requirement from the wheel
-    cache.
-
-    :param ireq: A single InstallRequirement
-    :type ireq: :class:`~pip._internal.req.req_install.InstallRequirement`
-    :return: A set of dependency lines for generating new InstallRequirements.
-    :rtype: set(str) or None
+            requires = build_system.get("requires", ["setuptools>=40.8", "wheel"])
+            backend = build_system.get("build-backend", get_default_pyproject_backend())
+    return requires, backend
+
+
+def split_markers_from_line(line):
+    # type: (AnyStr) -> Tuple[AnyStr, Optional[AnyStr]]
+    """Split markers from a dependency."""
+    quote_chars = ["'", '"']
+    line_quote = next(
+        iter(quote for quote in quote_chars if line.startswith(quote)), None
+    )
+    if line_quote and line.endswith(line_quote):
+        line = line.strip(line_quote)
+    marker_sep = " ; "
+    markers = None
+    if marker_sep in line:
+        line, markers = line.split(marker_sep, 1)
+        markers = markers.strip() if markers else None
+    return line, markers
+
+
+def split_vcs_method_from_uri(uri):
+    # type: (AnyStr) -> Tuple[Optional[STRING_TYPE], STRING_TYPE]
+    """Split a vcs+uri formatted uri into (vcs, uri)"""
+    vcs_start = "{0}+"
+    vcs = next(
+        iter([vcs for vcs in VCS_LIST if uri.startswith(vcs_start.format(vcs))]), None
+    )
+    if vcs:
+        vcs, uri = uri.split("+", 1)
+    return vcs, uri
+
+
+def split_ref_from_uri(uri):
+    # type: (AnyStr) -> Tuple[AnyStr, Optional[AnyStr]]
+    """Given a path or URI, check for a ref and split it from the path if it is
+    present, returning a tuple of the original input and the ref or None.
+
+    :param AnyStr uri: The path or URI to split
+    :returns: A 2-tuple of the path or URI and the ref
+    :rtype: Tuple[AnyStr, Optional[AnyStr]]
     """
+    if not isinstance(uri, str):
+        raise TypeError("Expected a string, received {0!r}".format(uri))
+    parsed = _get_parsed_url(uri)
+    path = parsed.path if parsed.path else ""
+    scheme = parsed.scheme if parsed.scheme else ""
+    ref = None
+    schema_is_filelike = scheme in ("", "file")
+    if (not schema_is_filelike and "@" in path) or (
+        schema_is_filelike and (re.match("^.*@[^/@]*$", path) or path.count("@") >= 2)
+    ):
+        path, _, ref = path.rpartition("@")
+    parsed = parsed._replace(path=path)
+    return (parsed.url, ref)
+
+
+def validate_vcs(instance, attr_, value):
+    if value not in VCS_LIST:
+        raise ValueError("Invalid vcs {0!r}".format(value))
+
+
+def validate_path(instance, attr_, value):
+    if not os.path.exists(value):
+        raise ValueError("Invalid path {0!r}".format(value))
+
+
+def validate_specifiers(instance, attr_, value):
+    if value == "":
+        return True
+    try:
+        SpecifierSet(value)
+    except (InvalidMarker, InvalidSpecifier):
+        raise ValueError("Invalid Specifiers {0}".format(value))
 
-    if ireq.editable or not is_pinned_requirement(ireq):
-        return
-    with _get_wheel_cache() as wheel_cache:
-        matches = wheel_cache.get(ireq.link, name_from_req(ireq.req), ireq.markers)
-        if matches:
-            matches = set(matches)
-            if not DEPENDENCY_CACHE.get(ireq):
-                DEPENDENCY_CACHE[ireq] = [format_requirement(m) for m in matches]
-            return matches
-        return None
 
+def key_from_req(req):
+    """Get an all-lowercase version of the requirement's name."""
+    if hasattr(req, "key"):
+        # from pkg_resources, such as installed dists for pip-sync
+        key = req.key
+    else:
+        # from packaging, such as install requirements from requirements.txt
+        key = req.name
+
+    key = key.replace("_", "-").lower()
+    return key
 
-def _marker_contains_extra(ireq):
-    # TODO: Implement better parsing logic avoid false-positives.
-    return "extra" in repr(ireq.markers)
 
+def _requirement_to_str_lowercase_name(requirement):
+    """Formats a packaging.requirements.Requirement with a lowercase name.
 
-def get_dependencies_from_json(ireq):
-    """Retrieves dependencies for the given install requirement from the json
-    api.
+    This is simply a copy of
+    https://github.com/pypa/packaging/blob/16.8/packaging/requirements.py#L109-L124
+    modified to lowercase the dependency name.
 
-    :param ireq: A single InstallRequirement
-    :type ireq: :class:`~pip._internal.req.req_install.InstallRequirement`
-    :return: A set of dependency lines for generating new InstallRequirements.
-    :rtype: set(str) or None
+    Previously, we were invoking the original Requirement.__str__ method and
+    lower-casing the entire result, which would lowercase the name, *and* other,
+    important stuff that should not be lower-cased (such as the marker). See
+    this issue for more information: https://github.com/pypa/pipenv/issues/2113.
     """
+    parts = [requirement.name.lower()]
 
-    if ireq.editable or not is_pinned_requirement(ireq):
-        return
+    if requirement.extras:
+        parts.append("[{0}]".format(",".join(sorted(requirement.extras))))
 
-    # It is technically possible to parse extras out of the JSON API's
-    # requirement format, but it is such a chore let's just use the simple API.
-    if ireq.extras:
-        return
+    if requirement.specifier:
+        parts.append(str(requirement.specifier))
 
-    session = requests.session()
-    atexit.register(session.close)
-    version = str(ireq.req.specifier).lstrip("=")
+    if requirement.url:
+        parts.append("@ {0}".format(requirement.url))
 
-    def gen(ireq):
-        info = None
-        try:
-            info = session.get(
-                "https://pypi.org/pypi/{0}/{1}/json".format(ireq.req.name, version)
-            ).json()["info"]
-        finally:
-            session.close()
-        requires_dist = info.get("requires_dist", info.get("requires"))
-        if not requires_dist:  # The API can return None for this.
-            return
-        for requires in requires_dist:
-            i = install_req_from_line(requires)
-            # See above, we don't handle requirements with extras.
-            if not _marker_contains_extra(i):
-                yield format_requirement(i)
+    if requirement.marker:
+        parts.append(" ; {0}".format(requirement.marker))
 
-    if ireq not in DEPENDENCY_CACHE:
-        try:
-            reqs = DEPENDENCY_CACHE[ireq] = list(gen(ireq))
-        except JSONDecodeError:
-            return
-        req_iter = iter(reqs)
+    return "".join(parts)
+
+
+def format_requirement(ireq):
+    """Formats an `InstallRequirement` instance as a string.
+
+    Generic formatter for pretty printing InstallRequirements to the terminal
+    in a less verbose way than using its `__str__` method.
+
+    :param :class:`InstallRequirement` ireq: A pip **InstallRequirement** instance.
+    :return: A formatted string for prettyprinting
+    :rtype: str
+    """
+    if ireq.editable:
+        line = "-e {}".format(ireq.link)
     else:
-        req_iter = gen(ireq)
-    return set(req_iter)
+        line = _requirement_to_str_lowercase_name(ireq.req)
 
+    if str(ireq.req.marker) != str(ireq.markers):
+        if not ireq.req.marker:
+            line = "{} ; {}".format(line, ireq.markers)
+        else:
+            name, markers = line.split(";", 1)
+            markers = markers.strip()
+            line = "{} ; ({}) and ({})".format(name, markers, ireq.markers)
+
+    return line
+
+
+def get_pinned_version(ireq):
+    """Get the pinned version of an InstallRequirement.
 
-def get_dependencies_from_cache(ireq):
-    """Retrieves dependencies for the given install requirement from the
-    dependency cache.
+    An InstallRequirement is considered pinned if:
 
-    :param ireq: A single InstallRequirement
-    :type ireq: :class:`~pip._internal.req.req_install.InstallRequirement`
-    :return: A set of dependency lines for generating new InstallRequirements.
-    :rtype: set(str) or None
+    - Is not editable
+    - It has exactly one specifier
+    - That specifier is "=="
+    - The version does not contain a wildcard
+
+    Examples:
+        django==1.8   # pinned
+        django>1.8    # NOT pinned
+        django~=1.8   # NOT pinned
+        django==1.*   # NOT pinned
+
+    Raises `TypeError` if the input is not a valid InstallRequirement, or
+    `ValueError` if the InstallRequirement is not pinned.
+    """
+    try:
+        specifier = ireq.specifier
+    except AttributeError:
+        raise TypeError("Expected InstallRequirement, not {}".format(type(ireq).__name__))
+
+    if getattr(ireq, "editable", False):
+        raise ValueError("InstallRequirement is editable")
+    if not specifier:
+        raise ValueError("InstallRequirement has no version specification")
+    if len(specifier._specs) != 1:
+        raise ValueError("InstallRequirement has multiple specifications")
+
+    op, version = next(iter(specifier._specs))._spec
+    if op not in ("==", "===") or version.endswith(".*"):
+        raise ValueError("InstallRequirement not pinned (is {0!r})".format(op + version))
+
+    return version
+
+
+def is_pinned_requirement(ireq):
+    """Returns whether an InstallRequirement is a "pinned" requirement.
+
+    An InstallRequirement is considered pinned if:
+
+    - Is not editable
+    - It has exactly one specifier
+    - That specifier is "=="
+    - The version does not contain a wildcard
+
+    Examples:
+        django==1.8   # pinned
+        django>1.8    # NOT pinned
+        django~=1.8   # NOT pinned
+        django==1.*   # NOT pinned
     """
-    if ireq.editable or not is_pinned_requirement(ireq):
-        return
-    if ireq not in DEPENDENCY_CACHE:
-        return
-    cached = set(DEPENDENCY_CACHE[ireq])
 
-    # Preserving sanity: Run through the cache and make sure every entry if
-    # valid. If this fails, something is wrong with the cache. Drop it.
     try:
-        broken = False
-        for line in cached:
-            dep_ireq = install_req_from_line(line)
-            name = canonicalize_name(dep_ireq.name)
-            if _marker_contains_extra(dep_ireq):
-                broken = True  # The "extra =" marker breaks everything.
-            elif name == canonicalize_name(ireq.name):
-                broken = True  # A package cannot depend on itself.
-            if broken:
-                break
-    except Exception:
-        broken = True
+        get_pinned_version(ireq)
+    except (TypeError, ValueError):
+        return False
+    return True
 
-    if broken:
-        del DEPENDENCY_CACHE[ireq]
-        return
 
-    return cached
+def as_tuple(ireq):
+    """Pulls out the (name: str, version:str, extras:(str)) tuple from the
+    pinned InstallRequirement."""
 
+    if not is_pinned_requirement(ireq):
+        raise TypeError("Expected a pinned InstallRequirement, got {}".format(ireq))
 
-def is_python(section):
-    return section.startswith("[") and ":" in section
+    name = key_from_req(ireq.req)
+    version = next(iter(ireq.specifier._specs))._spec[1]
+    extras = tuple(sorted(ireq.extras))
+    return name, version, extras
 
 
-def get_resolver(
-    finder, build_tracker, pip_options, session, directory, install_command=None
+def make_install_requirement(
+    name, version=None, extras=None, markers=None, constraint=False
 ):
-    wheel_cache = WheelCache(pip_options.cache_dir)
-    if install_command is None:
-        install_command = get_pip_command()
-    preparer = install_command.make_requirement_preparer(
-        temp_build_dir=directory,
-        options=pip_options,
-        build_tracker=build_tracker,
-        session=session,
-        finder=finder,
-        use_user_site=False,
-    )
-    resolver = install_command.make_resolver(
-        preparer=preparer,
-        finder=finder,
-        options=pip_options,
-        wheel_cache=wheel_cache,
-        use_user_site=False,
-        ignore_installed=True,
-        ignore_requires_python=pip_options.ignore_requires_python,
-        force_reinstall=pip_options.force_reinstall,
-        upgrade_strategy="to-satisfy-only",
-        use_pep517=pip_options.use_pep517,
-    )
-    return resolver
+    """Generates an :class:`~pip._internal.req.req_install.InstallRequirement`.
 
+    Create an InstallRequirement from the supplied metadata.
 
-def resolve(ireq, sources, install_command, pip_options):
-    with global_tempdir_manager(), get_build_tracker() as build_tracker, TempDirectory() as directory:
-        session, finder = get_finder(
-            sources=sources, pip_command=install_command, pip_options=pip_options
-        )
-        resolver = get_resolver(
-            finder=finder,
-            build_tracker=build_tracker,
-            pip_options=pip_options,
-            session=session,
-            directory=directory,
-            install_command=install_command,
-        )
-        reqset = RequirementSet(install_command)
-        reqset.add_named_requirement(ireq)
-        resolver_args = []
-        resolver_args.append([ireq])
-        resolver_args.append(True)  # check_supported_wheels
-        if getattr(reqset, "prepare_files", None):
-            reqset.prepare_files(finder)
-            result = reqset.requirements
-            reqset.cleanup_files()
-            return result
-        result_reqset = resolver.resolve(*resolver_args)
-        if result_reqset is None:
-            result_reqset = reqset
-        results = result_reqset.requirements
-        cleanup_fn = getattr(reqset, "cleanup_files", None)
-        if cleanup_fn is not None:
-            cleanup_fn()
-        return results
-
-
-def get_dependencies_from_index(dep, sources=None, pip_options=None, wheel_cache=None):
-    """Retrieves dependencies for the given install requirement from the pip
-    resolver.
-
-    :param dep: A single InstallRequirement
-    :type dep: :class:`~pip._internal.req.req_install.InstallRequirement`
-    :param sources: Pipfile-formatted sources, defaults to None
-    :type sources: list[dict], optional
-    :return: A set of dependency lines for generating new InstallRequirements.
-    :rtype: set(str) or None
-    """
-    install_command = get_pip_command()
-    if pip_options is None:
-        pip_options = get_pip_options(sources=sources, pip_command=install_command)
-    dep.is_direct = True
-    setup_requires = {}
-    with temp_environ():
-        os.environ["PIP_EXISTS_ACTION"] = "i"
-        if dep.editable and not dep.prepared and not dep.req:
-            setup_info = SetupInfo.from_ireq(dep)
-            results = setup_info.get_info()
-            setup_requires.update(results["setup_requires"])
-            requirements = set(results["requires"].values())
-        else:
-            results = resolve(
-                dep,
-                sources=sources,
-                install_command=install_command,
-                pip_options=pip_options,
-            )
-            requirements = [v for v in results.values() if v.name != dep.name]
-        requirements = set([format_requirement(r) for r in requirements])
-    if not dep.editable and is_pinned_requirement(dep) and requirements is not None:
-        DEPENDENCY_CACHE[dep] = list(requirements)
-    return requirements
-
-
-def get_pip_options(args=None, sources=None, pip_command=None):
-    """Build a pip command from a list of sources.
-
-    :param args: positional arguments passed through to the pip parser
-    :param sources: A list of pipfile-formatted sources, defaults to None
-    :param sources: list[dict], optional
-    :param pip_command: A pre-built pip command instance
-    :type pip_command: :class:`~pip._internal.cli.base_command.Command`
-    :return: An instance of pip_options using the supplied arguments plus sane defaults
-    :rtype: :class:`~pip._internal.cli.cmdoptions`
-    """
-
-    if not pip_command:
-        pip_command = get_pip_command()
-    if not sources:
-        sources = [{"url": "https://pypi.org/simple", "name": "pypi", "verify_ssl": True}]
-    os.makedirs(CACHE_DIR, mode=0o777, exist_ok=True)
-    pip_args = args or []
-    pip_args = prepare_pip_source_args(sources, pip_args)
-    pip_options, _ = pip_command.parser.parse_args(pip_args)
-    pip_options.cache_dir = CACHE_DIR
-    return pip_options
-
-
-def get_finder(sources=None, pip_command=None, pip_options=None):
-    # type: (List[Dict[S, Union[S, bool]]], Optional[Command], Any) -> PackageFinder
-    """Get a package finder for looking up candidates to install.
-
-    :param sources: A list of pipfile-formatted sources, defaults to None
-    :param sources: list[dict], optional
-    :param pip_command: A pip command instance, defaults to None
-    :type pip_command: :class:`~pip._internal.cli.base_command.Command`
-    :param pip_options: A pip options, defaults to None
-    :type pip_options: :class:`~pip._internal.cli.cmdoptions`
-    :return: A package finder
-    :rtype: :class:`~pip._internal.index.PackageFinder`
-    """
-
-    if not pip_command:
-        pip_command = get_pip_command()
-    if not sources:
-        sources = [{"url": "https://pypi.org/simple", "name": "pypi", "verify_ssl": True}]
-    if not pip_options:
-        pip_options = get_pip_options(sources=sources, pip_command=pip_command)
-    session = pip_command._build_session(pip_options)
-    atexit.register(session.close)
-    finder = get_package_finder(get_pip_command(), options=pip_options, session=session)
-    return session, finder
-
-
-@contextlib.contextmanager
-def start_resolver(finder=None, session=None, wheel_cache=None):
-    """Context manager to produce a resolver.
-
-    :param finder: A package finder to use for searching the index
-    :type finder: :class:`~pip._internal.index.PackageFinder`
-    :param :class:`~requests.Session` session: A session instance
-    :param :class:`~pip._internal.cache.WheelCache` wheel_cache: A pip WheelCache instance
-    :return: A 3-tuple of finder, preparer, resolver
-    :rtype: (:class:`~pip._internal.operations.prepare.RequirementPreparer`,
-             :class:`~pip._internal.resolve.Resolver`)
-    """
-
-    pip_command = get_pip_command()
-    pip_options = get_pip_options(pip_command=pip_command)
-    session = None
-    if not finder:
-        session, finder = get_finder(pip_command=pip_command, pip_options=pip_options)
-    if not session:
-        session = pip_command._build_session(pip_options)
-
-    download_dir = PKGS_DOWNLOAD_DIR
-    os.makedir(download_dir, mode=0o777)
-
-    _build_dir = create_tracked_tempdir("build")
-    _source_dir = create_tracked_tempdir("source")
-    pip_options.src_dir = _source_dir
-    try:
-        with global_tempdir_manager(), get_build_tracker() as build_tracker:
-            if not wheel_cache:
-                wheel_cache = _get_wheel_cache()
-            os.makdirs(os.path.join(wheel_cache.cache_dir, "wheels"))
-            preparer = pip_command.make_requirement_preparer(
-                temp_build_dir=_build_dir,
-                options=pip_options,
-                build_tracker=build_tracker,
-                session=session,
-                finder=finder,
-                use_user_site=False,
-            )
-            resolver = pip_command.make_resolver(
-                preparer=preparer,
-                finder=finder,
-                options=pip_options,
-                wheel_cache=wheel_cache,
-                use_user_site=False,
-                ignore_installed=True,
-                ignore_requires_python=pip_options.ignore_requires_python,
-                force_reinstall=pip_options.force_reinstall,
-                upgrade_strategy="to-satisfy-only",
-                use_pep517=pip_options.use_pep517,
-            )
-            yield resolver
-    finally:
-        session.close()
-
-
-def get_grouped_dependencies(constraints):
-    # We need to track what contributed a specifierset
-    # as well as which specifiers were required by the root node
-    # in order to resolve any conflicts when we are deciding which thing to backtrack on
-    # then we take the loose match (which _is_ flexible) and start moving backwards in
-    # versions by popping them off of a stack and checking for the conflicting package
-    for _, ireqs in full_groupby(constraints, key=key_from_ireq):
-        ireqs = sorted(ireqs, key=lambda ireq: ireq.editable)
-        editable_ireq = next(iter(ireq for ireq in ireqs if ireq.editable), None)
-        if editable_ireq:
-            yield editable_ireq  # only the editable match mattters, ignore all others
-            continue
-        ireqs = iter(ireqs)
-        # deepcopy the accumulator so as to not modify the self.our_constraints invariant
-        combined_ireq = copy.deepcopy(next(ireqs))
-        for ireq in ireqs:
-            # NOTE we may be losing some info on dropped reqs here
-            try:
-                combined_ireq.req.specifier &= ireq.req.specifier
-            except TypeError:
-                if ireq.req.specifier._specs and not combined_ireq.req.specifier._specs:
-                    combined_ireq.req.specifier._specs = ireq.req.specifier._specs
-            combined_ireq.constraint &= ireq.constraint
-            if not combined_ireq.markers:
-                combined_ireq.markers = ireq.markers
+    :param name: The requirement's name.
+    :type name: str
+    :param version: The requirement version (must be pinned).
+    :type version: str.
+    :param extras: The desired extras.
+    :type extras: list[str]
+    :param markers: The desired markers, without a preceding semicolon.
+    :type markers: str
+    :param constraint: Whether to flag the requirement as a constraint, defaults to False.
+    :param constraint: bool, optional
+    :return: A generated InstallRequirement
+    :rtype: :class:`~pip._internal.req.req_install.InstallRequirement`
+    """
+    requirement_string = "{0}".format(name)
+    if extras:
+        # Sort extras for stability
+        extras_string = "[{}]".format(",".join(sorted(extras)))
+        requirement_string = "{0}{1}".format(requirement_string, extras_string)
+    if version:
+        requirement_string = "{0}=={1}".format(requirement_string, str(version))
+    if markers:
+        requirement_string = "{0} ; {1}".format(requirement_string, str(markers))
+    return install_req_from_line(requirement_string, constraint=constraint)
+
+
+def normalize_name(pkg) -> str:
+    """Given a package name, return its normalized, non-canonicalized form."""
+    return pkg.replace("_", "-").lower()
+
+
+def get_name_variants(pkg):
+    # type: (STRING_TYPE) -> Set[STRING_TYPE]
+    """Given a packager name, get the variants of its name for both the
+    canonicalized and "safe" forms.
+
+    :param AnyStr pkg: The package to lookup
+    :returns: A list of names.
+    :rtype: Set
+    """
+
+    if not isinstance(pkg, str):
+        raise TypeError("must provide a string to derive package names")
+
+    pkg = pkg.lower()
+    names = {safe_name(pkg), canonicalize_name(pkg), pkg.replace("-", "_")}
+    return names
+
+
+def expand_env_variables(line):
+    # type: (AnyStr) -> AnyStr
+    """Expand the env vars in a line following pip's standard.
+    https://pip.pypa.io/en/stable/reference/pip_install/#id10.
+
+    Matches environment variable-style values in '${MY_VARIABLE_1}' with
+    the variable name consisting of only uppercase letters, digits or
+    the '_'
+    """
+
+    def replace_with_env(match):
+        value = os.getenv(match.group(1))
+        return value if value else match.group()
+
+    return re.sub(r"\$\{([A-Z0-9_]+)\}", replace_with_env, line)
+
+
+def tuple_to_dict(input_tuple):
+    result_dict = {}
+    i = 0
+    while i < len(input_tuple):
+        key = input_tuple[i]
+        i += 1
+        if i < len(input_tuple):
+            if isinstance(input_tuple[i], tuple):
+                value = tuple_to_dict(input_tuple[i])
+                i += 1
             else:
-                _markers = combined_ireq.markers._markers
-                if not isinstance(_markers[0], (tuple, list)):
-                    combined_ireq.markers._markers = [
-                        _markers,
-                        "and",
-                        ireq.markers._markers,
-                    ]
-            # Return a sorted, de-duped tuple of extras
-            combined_ireq.extras = tuple(
-                sorted(set(tuple(combined_ireq.extras) + tuple(ireq.extras)))
-            )
-        yield combined_ireq
+                value = input_tuple[i]
+                i += 1
+            result_dict[key] = value
+    return result_dict
```

### Comparing `requirementslib-2.3.0/src/requirementslib/models/lockfile.py` & `requirementslib-2.3.1.dev0/src/requirementslib/models/lockfile.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,59 +1,48 @@
 import copy
 import itertools
 import os
 from json import JSONDecodeError
 from pathlib import Path
+from typing import Dict, Iterator, List, Optional
 
-import attr
 from plette import lockfiles
+from pydantic import Field
 
 from ..exceptions import LockfileCorruptException, MissingParameter, PipfileNotFound
 from ..utils import is_editable, is_vcs, merge_items
+from .common import ReqLibBaseModel
 from .project import ProjectFile
 from .requirements import Requirement
-from .utils import optional_instance_of
 
 DEFAULT_NEWLINES = "\n"
 
 
 def preferred_newlines(f):
     if isinstance(f.newlines, str):
         return f.newlines
     return DEFAULT_NEWLINES
 
 
-is_lockfile = optional_instance_of(lockfiles.Lockfile)
-is_projectfile = optional_instance_of(ProjectFile)
-
-
-@attr.s(slots=True)
-class Lockfile(object):
-    path = attr.ib(validator=optional_instance_of(Path), type=Path)
-    _requirements = attr.ib(default=attr.Factory(list), type=list)
-    _dev_requirements = attr.ib(default=attr.Factory(list), type=list)
-    projectfile = attr.ib(validator=is_projectfile, type=ProjectFile)
-    _lockfile = attr.ib(validator=is_lockfile, type=lockfiles.Lockfile)
-    newlines = attr.ib(default=DEFAULT_NEWLINES, type=str)
-
-    @path.default
-    def _get_path(self):
-        return Path(os.curdir).joinpath("Pipfile.lock").absolute()
-
-    @projectfile.default
-    def _get_projectfile(self):
-        return self.load_projectfile(self.path)
-
-    @_lockfile.default
-    def _get_lockfile(self):
-        return self.projectfile.model
-
-    @property
-    def lockfile(self):
-        return self._lockfile
+class Lockfile(ReqLibBaseModel):
+    path: Path = Field(
+        default_factory=lambda: Path(os.curdir).joinpath("Pipfile.lock").absolute()
+    )
+    _requirements: Optional[list] = Field(default_factory=list)
+    _dev_requirements: Optional[list] = Field(default_factory=list)
+    projectfile: ProjectFile = None
+    lockfile: lockfiles.Lockfile
+    newlines: str = DEFAULT_NEWLINES
+
+    class Config:
+        validate_assignment = True
+        arbitrary_types_allowed = True
+        allow_mutation = True
+        include_private_attributes = True
+        # keep_untouched = (cached_property,)
 
     @property
     def section_keys(self):
         return set(self.lockfile.keys()) - {"_meta"}
 
     @property
     def extended_keys(self):
@@ -65,20 +54,20 @@
     def __contains__(self, k):
         check_lockfile = k in self.extended_keys or self.lockfile.__contains__(k)
         if check_lockfile:
             return True
         return super(Lockfile, self).__contains__(k)
 
     def __setitem__(self, k, v):
-        lockfile = self._lockfile
+        lockfile = self.lockfile
         lockfile.__setitem__(k, v)
 
     def __getitem__(self, k, *args, **kwargs):
         retval = None
-        lockfile = self._lockfile
+        lockfile = self.lockfile
         try:
             retval = lockfile[k]
         except KeyError:
             if "-" in k:
                 section, _, pkg_type = k.rpartition("-")
                 vals = getattr(lockfile.get(section, {}), "_data", {})
                 if pkg_type == "vcs":
@@ -88,15 +77,15 @@
             if retval is None:
                 raise
         else:
             retval = getattr(retval, "_data", retval)
         return retval
 
     def __getattr__(self, k, *args, **kwargs):
-        lockfile = super(Lockfile, self).__getattribute__("_lockfile")
+        lockfile = self.lockfile
         try:
             return super(Lockfile, self).__getattribute__(k)
         except AttributeError:
             retval = getattr(lockfile, k, None)
         if retval is not None:
             return retval
         return super(Lockfile, self).__getattribute__(k, *args, **kwargs)
@@ -108,82 +97,62 @@
             if only:
                 return deps
         deps = merge_items([deps, self.default._data])
         return deps
 
     @classmethod
     def read_projectfile(cls, path):
-        """Read the specified project file and provide an interface for
-        writing/updating.
-
-        :param str path: Path to the target file.
-        :return: A project file with the model and location for interaction
-        :rtype: :class:`~requirementslib.models.project.ProjectFile`
-        """
         pf = ProjectFile.read(path, lockfiles.Lockfile, invalid_ok=True)
         return pf
 
     @classmethod
     def lockfile_from_pipfile(cls, pipfile_path):
         from .pipfile import Pipfile
 
         if os.path.isfile(pipfile_path):
             if not os.path.isabs(pipfile_path):
                 pipfile_path = os.path.abspath(pipfile_path)
             pipfile = Pipfile.load(os.path.dirname(pipfile_path))
-            return lockfiles.Lockfile.with_meta_from(pipfile._pipfile)
+            return lockfiles.Lockfile.with_meta_from(pipfile.pipfile)
         raise PipfileNotFound(pipfile_path)
 
     @classmethod
-    def load_projectfile(cls, path, create=True, data=None):
-        """Given a path, load or create the necessary lockfile.
-
-        :param str path: Path to the project root or lockfile
-        :param bool create: Whether to create the lockfile if not found, defaults to True
-        :raises OSError: Thrown if the project root directory doesn't exist
-        :raises FileNotFoundError: Thrown if the lockfile doesn't exist and ``create=False``
-        :return: A project file instance for the supplied project
-        :rtype: :class:`~requirementslib.models.project.ProjectFile`
-        """
-
+    def load_projectfile(
+        cls, path: Optional[str] = None, create: bool = True, data: Optional[Dict] = None
+    ) -> "ProjectFile":
         if not path:
             path = os.curdir
         path = Path(path).absolute()
         project_path = path if path.is_dir() else path.parent
         lockfile_path = path if path.is_file() else project_path / "Pipfile.lock"
         if not project_path.exists():
-            raise OSError("Project does not exist: %s" % project_path.as_posix())
+            raise OSError(f"Project does not exist: {project_path.as_posix()}")
         elif not lockfile_path.exists() and not create:
             raise FileNotFoundError(
-                "Lockfile does not exist: %s" % lockfile_path.as_posix()
+                f"Lockfile does not exist: {lockfile_path.as_posix()}"
             )
         projectfile = cls.read_projectfile(lockfile_path.as_posix())
         if not lockfile_path.exists():
             if not data:
-                path_str = lockfile_path.as_posix()
-                if path_str[-5:] == ".lock":
-                    pipfile = Path(path_str[:-5])
-                else:
-                    pipfile = project_path.joinpath("Pipfile")
+                pipfile = project_path.joinpath("Pipfile")
                 lf = cls.lockfile_from_pipfile(pipfile)
             else:
                 lf = lockfiles.Lockfile(data)
             projectfile.model = lf
+        else:
+            if data:
+                raise ValueError("Cannot pass data when loading existing lockfile")
+            with open(lockfile_path.as_posix(), "r") as f:
+                projectfile.model = lockfiles.Lockfile.load(f)
         return projectfile
 
     @classmethod
-    def from_data(cls, path, data, meta_from_project=True):
-        """Create a new lockfile instance from a dictionary.
-
-        :param str path: Path to the project root.
-        :param dict data: Data to load into the lockfile.
-        :param bool meta_from_project: Attempt to populate the meta section from the
-            project root, default True.
-        """
-
+    def from_data(
+        cls, path: Optional[str], data: Optional[Dict], meta_from_project: bool = True
+    ) -> "Lockfile":
         if path is None:
             raise MissingParameter("path")
         if data is None:
             raise MissingParameter("data")
         if not isinstance(data, dict):
             raise TypeError("Expecting a dictionary for parameter 'data'")
         path = os.path.abspath(str(path))
@@ -205,103 +174,86 @@
             projectfile=projectfile,
             lockfile=lockfile,
             newlines=projectfile.line_ending,
             path=Path(projectfile.location),
         )
 
     @classmethod
-    def load(cls, path, create=True):
-        """Create a new lockfile instance.
-
-        :param project_path: Path to  project root or lockfile
-        :type project_path: str or :class:`pathlib.Path`
-        :param str lockfile_name: Name of the lockfile in the project root directory
-        :param pipfile_path: Path to the project pipfile
-        :type pipfile_path: :class:`pathlib.Path`
-        :returns: A new lockfile representing the supplied project paths
-        :rtype: :class:`~requirementslib.models.lockfile.Lockfile`
-        """
-
+    def load(cls, path: Optional[str], create: bool = True) -> "Lockfile":
         try:
             projectfile = cls.load_projectfile(path, create=create)
         except JSONDecodeError:
             path = os.path.abspath(path)
             path = Path(
                 os.path.join(path, "Pipfile.lock") if os.path.isdir(path) else path
             )
             formatted_path = path.as_posix()
-            backup_path = "%s.bak" % formatted_path
+            backup_path = f"{formatted_path}.bak"
             LockfileCorruptException.show(formatted_path, backup_path=backup_path)
             path.rename(backup_path)
             cls.load(formatted_path, create=True)
         lockfile_path = Path(projectfile.location)
         creation_args = {
             "projectfile": projectfile,
             "lockfile": projectfile.model,
             "newlines": projectfile.line_ending,
             "path": lockfile_path,
         }
         return cls(**creation_args)
 
     @classmethod
-    def create(cls, path, create=True):
+    def create(cls, path: Optional[str], create: bool = True) -> "Lockfile":
         return cls.load(path, create=create)
 
-    def get_section(self, name):
-        return self._lockfile.get(name)
+    def get_section(self, name: str) -> Optional[Dict]:
+        return self.lockfile.get(name)
 
     @property
-    def develop(self):
-        return self._lockfile.develop
+    def develop(self) -> Dict:
+        return self.lockfile.develop
 
     @property
-    def default(self):
-        return self._lockfile.default
+    def default(self) -> Dict:
+        return self.lockfile.default
 
-    def get_requirements(self, dev=True, only=False, categories=None):
-        """Produces a generator which generates requirements from the desired
-        section.
-
-        :param bool dev: Indicates whether to use dev requirements, defaults to False
-        :return: Requirements from the relevant pipfile
-        :rtype: :class:`Iterator[~requirementslib.models.requirements.Requirement]`
-        """
+    def get_requirements(
+        self, dev: bool = True, only: bool = False, categories: Optional[List[str]] = None
+    ) -> Iterator[Requirement]:
         if categories:
             deps = {}
             for category in categories:
                 if category == "packages":
                     category = "default"
                 elif category == "dev-packages":
                     category = "develop"
                 try:
                     category_deps = self[category]
                 except KeyError:
                     category_deps = {}
-                    self._lockfile[category] = category_deps
+                    self.lockfile[category] = category_deps
                 deps = merge_items([deps, category_deps])
         else:
             deps = self.get_deps(dev=dev, only=only)
         for k, v in deps.items():
             yield Requirement.from_pipfile(k, v)
 
-    def requirements_list(self, category):
-        if self._lockfile.get(category):
+    def requirements_list(self, category: str) -> List[Dict]:
+        if self.lockfile.get(category):
             return [
-                {name: entry._data} for name, entry in self._lockfile[category].items()
+                {name: entry._data} for name, entry in self.lockfile[category].items()
             ]
         return []
 
-    def as_requirements(self, category, include_hashes=False):
-        """Returns a list of requirements in pip-style format."""
+    def as_requirements(self, category: str, include_hashes: bool = False) -> List[str]:
         lines = []
         section = list(self.get_requirements(categories=[category]))
         for req in section:
             kwargs = {"include_hashes": include_hashes}
             if req.editable:
                 kwargs["include_markers"] = False
             r = req.as_line(**kwargs)
             lines.append(r.strip())
         return lines
 
-    def write(self):
-        self.projectfile.model = copy.deepcopy(self._lockfile)
+    def write(self) -> None:
+        self.projectfile.model = copy.deepcopy(self.lockfile)
         self.projectfile.write()
```

### Comparing `requirementslib-2.3.0/src/requirementslib/models/markers.py` & `requirementslib-2.3.1.dev0/src/requirementslib/models/markers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,82 +1,49 @@
 import itertools
 import operator
 import re
 from collections.abc import Mapping, Set
 from functools import reduce
+from typing import Any, AnyStr, Iterator, List, Optional, Tuple, Type, Union
 
-import attr
-from distlib import markers
+from pip._vendor.distlib import markers
 from pip._vendor.packaging.markers import InvalidMarker, Marker
 from pip._vendor.packaging.specifiers import LegacySpecifier, Specifier, SpecifierSet
-from pip._vendor.packaging.version import parse
+from pydantic import BaseModel
 
-from ..environment import MYPY_RUNNING
 from ..exceptions import RequirementError
-from .utils import filter_none, validate_markers
-
-if MYPY_RUNNING:
-    from typing import Any, AnyStr, Iterator, List, Optional, Text, Tuple, Type, Union
-
-    STRING_TYPE = Union[str, bytes, Text]
 
 MAX_VERSIONS = {1: 7, 2: 7, 3: 11, 4: 0}
 DEPRECATED_VERSIONS = ["3.0", "3.1", "3.2", "3.3"]
 
 
 def is_instance(item, cls):
     # type: (Any, Type) -> bool
     if isinstance(item, cls) or item.__class__.__name__ == cls.__name__:
         return True
     return False
 
 
-@attr.s
-class PipenvMarkers(object):
-    """System-level requirements - see PEP508 for more detail"""
-
-    os_name = attr.ib(default=None, validator=attr.validators.optional(validate_markers))
-    sys_platform = attr.ib(
-        default=None, validator=attr.validators.optional(validate_markers)
-    )
-    platform_machine = attr.ib(
-        default=None, validator=attr.validators.optional(validate_markers)
-    )
-    platform_python_implementation = attr.ib(
-        default=None, validator=attr.validators.optional(validate_markers)
-    )
-    platform_release = attr.ib(
-        default=None, validator=attr.validators.optional(validate_markers)
-    )
-    platform_system = attr.ib(
-        default=None, validator=attr.validators.optional(validate_markers)
-    )
-    platform_version = attr.ib(
-        default=None, validator=attr.validators.optional(validate_markers)
-    )
-    python_version = attr.ib(
-        default=None, validator=attr.validators.optional(validate_markers)
-    )
-    python_full_version = attr.ib(
-        default=None, validator=attr.validators.optional(validate_markers)
-    )
-    implementation_name = attr.ib(
-        default=None, validator=attr.validators.optional(validate_markers)
-    )
-    implementation_version = attr.ib(
-        default=None, validator=attr.validators.optional(validate_markers)
-    )
+class PipenvMarkers(BaseModel):
+    os_name: Optional[str] = None
+    sys_platform: Optional[str] = None
+    platform_machine: Optional[str] = None
+    platform_python_implementation: Optional[str] = None
+    platform_release: Optional[str] = None
+    platform_system: Optional[str] = None
+    platform_version: Optional[str] = None
+    python_version: Optional[str] = None
+    python_full_version: Optional[str] = None
+    implementation_name: Optional[str] = None
+    implementation_version: Optional[str] = None
 
     @property
     def line_part(self):
         return " and ".join(
-            [
-                "{0} {1}".format(k, v)
-                for k, v in attr.asdict(self, filter=filter_none).items()
-            ]
+            ["{0} {1}".format(k, v) for k, v in self.dict().items() if v is not None]
         )
 
     @property
     def pipfile_part(self):
         return {"markers": self.as_line}
 
     @classmethod
@@ -94,15 +61,15 @@
         if ";" in line:
             line = line.rsplit(";", 1)[1].strip()
         marker = cls.make_marker(line)
         return marker
 
     @classmethod
     def from_pipfile(cls, name, pipfile):
-        attr_fields = [field.name for field in attr.fields(cls)]
+        attr_fields = [field_name for field_name in cls.__fields__]
         found_keys = [k for k in pipfile.keys() if k in attr_fields]
         marker_strings = ["{0} {1}".format(k, pipfile[k]) for k in found_keys]
         if pipfile.get("markers"):
             marker_strings.append(pipfile.get("markers"))
         markers = set()
         for marker in marker_strings:
             markers.add(marker)
@@ -112,40 +79,39 @@
         except RequirementError:
             pass
         else:
             return combined_marker
 
 
 def _tuplize_version(version):
-    # type: (STRING_TYPE) -> Union[Tuple[()], Tuple[int, ...], Tuple[int, int, str]]
+    # type: (str) -> Union[Tuple[()], Tuple[int, ...], Tuple[int, int, str]]
     output = []
     for idx, part in enumerate(version.split(".")):
         if part == "*":
             break
         if idx in (0, 1):
             # Only convert the major and minor identifiers into integers (if present),
             # the patch identifier can include strings like 'b' marking a beta: ex 3.11.0b1
             part = int(part)
         output.append(part)
     return tuple(output)
 
 
-def _format_version(version):
-    # type: (Tuple[int, ...]) -> STRING_TYPE
+def _format_version(version) -> str:
     if not isinstance(version, str):
         return ".".join(str(i) for i in version)
     return version
 
 
 # Prefer [x,y) ranges.
 REPLACE_RANGES = {">": ">=", "<=": "<"}
 
 
 def _format_pyspec(specifier):
-    # type: (Union[STRING_TYPE, Specifier]) -> Specifier
+    # type: (Union[str, Specifier]) -> Specifier
     if isinstance(specifier, str):
         if not specifier.startswith(tuple(Specifier._operators.keys())):
             specifier = "=={0}".format(specifier)
         specifier = Specifier(specifier)
     version = getattr(specifier, "version", specifier).rstrip()
     if version:
         if version.startswith("*"):
@@ -312,48 +278,23 @@
     max_allowed = MAX_VERSIONS[version[0]]
     if op == "<" and version[1] > max_allowed and version[1] - 1 <= max_allowed:
         op = "<="
         version = (version[0], version[1] - 1)
     return (op, version)
 
 
-# TODO: Rename this to something meaningful, deprecate it (See prior function)
-def get_versions(specset, group_by_operator=True):
-    # type: (Union[Set[Specifier], SpecifierSet], bool) -> List[Tuple[STRING_TYPE, STRING_TYPE]]
-    specs = [_get_specs(x) for x in list(tuple(specset))]
-    initial_sort_key = lambda k: (k[0], k[1])
-    initial_grouping_key = operator.itemgetter(0)
-    if not group_by_operator:
-        initial_grouping_key = operator.itemgetter(1)
-        initial_sort_key = operator.itemgetter(1)
-    version_tuples = sorted(
-        set((op, version) for spec in specs for op, version in spec), key=initial_sort_key
-    )
-    version_tuples = [fix_version_tuple(t) for t in version_tuples]
-    op_groups = [
-        (grp, list(map(operator.itemgetter(1), keys)))
-        for grp, keys in itertools.groupby(version_tuples, key=initial_grouping_key)
-    ]
-    versions = [
-        (op, parse(".".join(str(v) for v in val)))
-        for op, vals in op_groups
-        for val in vals
-    ]
-    return sorted(versions, key=operator.itemgetter(1))
-
-
 def _ensure_marker(marker):
-    # type: (Union[STRING_TYPE, Marker]) -> Marker
+    # type: (Union[str, Marker]) -> Marker
     if not is_instance(marker, Marker):
         return Marker(str(marker))
     return marker
 
 
 def gen_marker(mkr):
-    # type: (List[STRING_TYPE]) -> Marker
+    # type: (List[str]) -> Marker
     m = Marker("python_version == '1'")
     m._markers.pop()
     m._markers.append(mkr)
     return m
 
 
 def _strip_extra(elements):
@@ -609,19 +550,19 @@
     # And if we hit the end of the parse tree we use this format string to make a marker
     format_string = "{lhs} {op} {rhs}"
     specset = SpecifierSet()
     specs = set()
     # Essentially we will iterate over each side of the parsed marker if either one is
     # A mapping instance (i.e. a dictionary) and recursively parse and reduce the specset
     # Union the "and" specs, intersect the "or"s to find the most appropriate range
-    if any(issubclass(type(side), Mapping) for side in (lhs, rhs)):
+    if any(isinstance(side, Mapping) for side in (lhs, rhs)):
         for side in (lhs, rhs):
             side_specs = set()
             side_markers = set()
-            if issubclass(type(side), Mapping):
+            if isinstance(side, Mapping):
                 merged_side_specs, merged_side_markers = parse_marker_dict(side)
                 side_specs.update(merged_side_specs)
                 side_markers.update(merged_side_markers)
             else:
                 marker = _ensure_marker(side)
                 marker_parts = getattr(marker, "_markers", [])
                 if marker_parts[0][0].value == "python_version":
@@ -674,16 +615,15 @@
     op, val = parts
     version_marker = (
         "python_full_version" if _contains_micro_version(val) else "python_version"
     )
     return "{0} {1} '{2}'".format(version_marker, op, val)
 
 
-def normalize_marker_str(marker):
-    # type: (Union[Marker, STRING_TYPE]) -> str
+def normalize_marker_str(marker) -> str:
     marker_str = ""
     if not marker:
         return None
     if not is_instance(marker, Marker):
         marker = _ensure_marker(marker)
     pyversion = get_contained_pyversions(marker)
     marker = get_without_pyversion(marker)
@@ -694,16 +634,15 @@
         if marker_str:
             marker_str = "{0!s} and {1!s}".format(marker_str, marker)
         else:
             marker_str = "{0!s}".format(marker)
     return marker_str.replace('"', "'")
 
 
-def marker_from_specifier(spec):
-    # type: (STRING_TYPE) -> Marker
+def marker_from_specifier(spec) -> Marker:
     if not any(spec.startswith(k) for k in Specifier._operators.keys()):
         if spec.strip().lower() in ["any", "<any>", "*"]:
             return None
         spec = "=={0}".format(spec)
     elif spec.startswith("==") and spec.count("=") > 3:
         spec = "=={0}".format(spec.lstrip("="))
     if not spec:
```

### Comparing `requirementslib-2.3.0/src/requirementslib/models/old_pip_utils.py` & `requirementslib-2.3.1.dev0/src/requirementslib/models/old_pip_utils.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.0/src/requirementslib/models/pipfile.py` & `requirementslib-2.3.1.dev0/src/requirementslib/models/pipfile.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,32 @@
-import copy
 import itertools
 import os
 from pathlib import Path
+from typing import Any, Dict, Iterable, List, Optional, Text, Union
 
-import attr
-import tomlkit
+import tomlkit as tomlkit
 from plette import pipfiles
+from pydantic import BaseModel, validator
 
 from ..environment import MYPY_RUNNING
 from ..exceptions import RequirementError
 from ..utils import is_editable, is_vcs, merge_items
+from .common import ReqLibBaseModel
 from .project import ProjectFile
 from .requirements import Requirement
-from .utils import get_url_name, optional_instance_of, tomlkit_value_to_python
+from .utils import get_url_name, tomlkit_value_to_python
 
 if MYPY_RUNNING:
-    from typing import Any, Dict, Iterable, List, Text, Union
-
     package_type = Dict[Text, Dict[Text, Union[List[Text], Text]]]
     source_type = Dict[Text, Union[Text, bool]]
     sources_type = Iterable[source_type]
     meta_type = Dict[Text, Union[int, Dict[Text, Text], sources_type]]
     lockfile_type = Dict[Text, Union[package_type, meta_type]]
 
 
-is_pipfile = optional_instance_of(pipfiles.Pipfile)
-is_path = optional_instance_of(Path)
-is_projectfile = optional_instance_of(ProjectFile)
-
-
 def reorder_source_keys(data):
     # type: (tomlkit.toml_document.TOMLDocument) -> tomlkit.toml_document.TOMLDocument
     sources = []  # type: sources_type
     for source_key in ["source", "sources"]:
         sources.extend(data.get(source_key, tomlkit.aot()).value)
     new_source_aot = tomlkit.aot()
     for entry in sources:
@@ -127,85 +121,77 @@
     def __getattribute__(self, key):
         # type: (Text) -> Any
         if key == "source":
             return self._data[key]
         return super(PipfileLoader, self).__getattribute__(key)
 
 
-@attr.s(slots=True)
-class Pipfile(object):
-    path = attr.ib(validator=is_path, type=Path)
-    projectfile = attr.ib(validator=is_projectfile, type=ProjectFile)
-    _pipfile = attr.ib(type=PipfileLoader)
-    _pyproject = attr.ib(
-        default=attr.Factory(tomlkit.document), type=tomlkit.toml_document.TOMLDocument
-    )
-    build_system = attr.ib(default=attr.Factory(dict), type=dict)
-    _requirements = attr.ib(default=attr.Factory(list), type=list)
-    _dev_requirements = attr.ib(default=attr.Factory(list), type=list)
-
-    @path.default
-    def _get_path(self):
-        # type: () -> Path
-        return Path(os.curdir).absolute()
-
-    @projectfile.default
-    def _get_projectfile(self):
-        # type: () -> ProjectFile
-        return self.load_projectfile(os.curdir, create=False)
-
-    @_pipfile.default
-    def _get_pipfile(self):
-        # type: () -> Union[pipfiles.Pipfile, PipfileLoader]
-        return self.projectfile.model
+class Pipfile(ReqLibBaseModel):
+    path: Path
+    projectfile: ProjectFile
+    pipfile: Optional[PipfileLoader]
+    _pyproject: Optional[tomlkit.TOMLDocument] = tomlkit.document()
+    build_system: Optional[Dict] = dict()
+    _requirements: Optional[List] = list()
+    _dev_requirements: Optional[List] = list()
+
+    class Config:
+        validate_assignment = True
+        arbitrary_types_allowed = True
+        allow_mutation = True
+        include_private_attributes = True
+        # keep_untouched = (cached_property,)
+
+    @validator("path", pre=True, always=True)
+    def _get_path(cls, v):
+        return v or Path(os.curdir).absolute()
+
+    @validator("projectfile", pre=True, always=True)
+    def _get_projectfile(cls, v, values):
+        return v or cls.load_projectfile(os.curdir, create=False)
+
+    @validator("pipfile", pre=True, always=True)
+    def _get_pipfile(cls, v, values):
+        return v or values["projectfile"].model
 
     @property
     def root(self):
         return self.path.parent
 
     @property
     def extended_keys(self):
         return [
             k
             for k in itertools.product(
                 ("packages", "dev-packages"), ("", "vcs", "editable")
             )
         ]
 
-    @property
-    def pipfile(self):
-        # type: () -> Union[PipfileLoader, pipfiles.Pipfile]
-        return self._pipfile
-
     def get_deps(self, dev=False, only=True):
-        # type: (bool, bool) -> Dict[Text, Dict[Text, Union[List[Text], Text]]]
         deps = {}  # type: Dict[Text, Dict[Text, Union[List[Text], Text]]]
         if dev:
             deps.update(dict(self.pipfile._data.get("dev-packages", {})))
             if only:
                 return deps
         return tomlkit_value_to_python(
             merge_items([deps, dict(self.pipfile._data.get("packages", {}))])
         )
 
     def get(self, k):
-        # type: (Text) -> Any
         return self.__getitem__(k)
 
     def __contains__(self, k):
-        # type: (Text) -> bool
         check_pipfile = k in self.extended_keys or self.pipfile.__contains__(k)
         if check_pipfile:
             return True
         return False
 
     def __getitem__(self, k, *args, **kwargs):
-        # type: ignore
         retval = None
-        pipfile = self._pipfile
+        pipfile = self.pipfile
         section = None
         pkg_type = None
         try:
             retval = pipfile[k]
         except KeyError:
             if "-" in k:
                 section, _, pkg_type = k.rpartition("-")
@@ -218,38 +204,34 @@
             if retval is None:
                 raise
         else:
             retval = getattr(retval, "_data", retval)
         return retval
 
     def __getattr__(self, k, *args, **kwargs):
-        # type: ignore
-        retval = None
-        pipfile = super(Pipfile, self).__getattribute__("_pipfile")
+        pipfile = self.pipfile
         try:
-            retval = super(Pipfile, self).__getattribute__(k)
+            retval = super(Pipfile).__getattribute__(k)
         except AttributeError:
             retval = getattr(pipfile, k, None)
-        if retval is not None:
-            return retval
-        return super(Pipfile, self).__getattribute__(k, *args, **kwargs)
+        return retval
 
     @property
     def requires_python(self):
         # type: () -> bool
         return getattr(
-            self._pipfile.requires,
+            self.pipfile.requires,
             "python_version",
-            getattr(self._pipfile.requires, "python_full_version", None),
+            getattr(self.pipfile.requires, "python_full_version", None),
         )
 
     @property
     def allow_prereleases(self):
         # type: () -> bool
-        return self._pipfile.get("pipenv", {}).get("allow_prereleases", False)
+        return self.pipfile.get("pipenv", {}).get("allow_prereleases", False)
 
     @classmethod
     def read_projectfile(cls, path):
         # type: (Text) -> ProjectFile
         """Read the specified project file and provide an interface for
         writing/updating.
 
@@ -303,19 +285,14 @@
         creation_args = {
             "projectfile": projectfile,
             "pipfile": pipfile,
             "path": Path(projectfile.location),
         }
         return cls(**creation_args)
 
-    def write(self):
-        # type: () -> None
-        self.projectfile.model = copy.deepcopy(self._pipfile)
-        self.projectfile.write()
-
     @property
     def dev_packages(self):
         # type: () -> List[Requirement]
         return self.dev_requirements
 
     @property
     def packages(self):
@@ -341,36 +318,7 @@
             packages = tomlkit_value_to_python(self.pipfile.get("packages", {}))
             self._requirements = [
                 Requirement.from_pipfile(k, v)
                 for k, v in packages.items()
                 if v is not None
             ]
         return self._requirements
-
-    def _read_pyproject(self):
-        # type: () -> None
-        pyproject = self.path.parent.joinpath("pyproject.toml")
-        if pyproject.exists():
-            self._pyproject = tomlkit.loads(pyproject.read_text())
-            build_system = self._pyproject.get("build-system", None)
-            if build_system and not build_system.get("build_backend"):
-                build_system["build-backend"] = "setuptools.build_meta:__legacy__"
-            elif not build_system or not build_system.get("requires"):
-                build_system = {
-                    "requires": ["setuptools>=40.8", "wheel"],
-                    "build-backend": "setuptools.build_meta:__legacy__",
-                }
-            self.build_system = build_system
-
-    @property
-    def build_requires(self):
-        # type: () -> List[Text]
-        if not self.build_system:
-            self._read_pyproject()
-        return self.build_system.get("requires", [])
-
-    @property
-    def build_backend(self):
-        # type: () -> Text
-        if not self.build_system:
-            self._read_pyproject()
-        return self.build_system.get("build-backend", None)
```

### Comparing `requirementslib-2.3.0/src/requirementslib/models/project.py` & `requirementslib-2.3.1.dev0/src/requirementslib/models/project.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import collections
 import io
 import os
+from typing import Any, Optional
 
-import attr
 from pip._vendor.packaging.markers import Marker
+from pydantic import BaseModel, Field
 
 SectionDifference = collections.namedtuple("SectionDifference", ["inthis", "inthat"])
 FileDifference = collections.namedtuple("FileDifference", ["default", "develop"])
 
 
 def _are_pipfile_entries_equal(a, b):
     a = {k: v for k, v in a.items() if k not in ("markers", "hashes", "hash")}
@@ -30,39 +31,39 @@
 
 def preferred_newlines(f):
     if isinstance(f.newlines, str):
         return f.newlines
     return DEFAULT_NEWLINES
 
 
-@attr.s
-class ProjectFile(object):
-    """A file in the Pipfile project."""
-
-    location = attr.ib()
-    line_ending = attr.ib()
-    model = attr.ib()
+class ProjectFile(BaseModel):
+    location: str
+    line_ending: str
+    model: Optional[Any] = Field(default_factory=lambda: dict())
 
     @classmethod
-    def read(cls, location, model_cls, invalid_ok=False):
+    def read(cls, location: str, model_cls, invalid_ok: bool = False) -> "ProjectFile":
         if not os.path.exists(location) and not invalid_ok:
             raise FileNotFoundError(location)
         try:
             with io.open(location, encoding="utf-8") as f:
                 model = model_cls.load(f)
                 line_ending = preferred_newlines(f)
         except Exception:
             if not invalid_ok:
                 raise
-            model = None
+            model = {}
             line_ending = DEFAULT_NEWLINES
         return cls(location=location, line_ending=line_ending, model=model)
 
-    def write(self):
+    def write(self) -> None:
         kwargs = {"encoding": "utf-8", "newline": self.line_ending}
         with io.open(self.location, "w", **kwargs) as f:
-            self.model.dump(f)
+            if self.model:
+                self.model.dump(f)
 
-    def dumps(self):
-        strio = io.StringIO()
-        self.model.dump(strio)
-        return strio.getvalue()
+    def dumps(self) -> str:
+        if self.model:
+            strio = io.StringIO()
+            self.model.dump(strio)
+            return strio.getvalue()
+        return ""
```

### Comparing `requirementslib-2.3.0/src/requirementslib/models/requirements.py` & `requirementslib-2.3.1.dev0/src/requirementslib/models/requirements.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,33 @@
 import collections
 import copy
 import os
 import sys
 from contextlib import contextmanager
-from functools import lru_cache
 from pathlib import Path
 from sysconfig import get_path
+from typing import (
+    Any,
+    AnyStr,
+    Dict,
+    Generator,
+    List,
+    Optional,
+    Sequence,
+    Set,
+    Text,
+    Tuple,
+    TypeVar,
+    Union,
+)
 from urllib import parse as urllib_parse
-from urllib.parse import unquote
+from urllib.parse import SplitResult, unquote, urlparse
+from urllib.request import url2pathname
 
-import attr
+from pip._internal.index.package_finder import PackageFinder
 from pip._internal.models.link import Link
 from pip._internal.models.wheel import Wheel
 from pip._internal.req.constructors import (
     _strip_extras,
     install_req_from_editable,
     install_req_from_line,
 )
@@ -27,14 +41,15 @@
     InvalidSpecifier,
     LegacySpecifier,
     Specifier,
     SpecifierSet,
 )
 from pip._vendor.packaging.utils import canonicalize_name
 from pip._vendor.packaging.version import parse
+from pydantic import Field
 
 from ..environment import MYPY_RUNNING
 from ..exceptions import RequirementError
 from ..fileutils import (
     create_tracked_tempdir,
     get_converted_relative_path,
     is_file_url,
@@ -48,15 +63,15 @@
     add_ssh_scheme_to_git_uri,
     get_setup_paths,
     is_installable_dir,
     is_installable_file,
     is_vcs,
     strip_ssh_from_git_uri,
 )
-from .dependencies import AbstractDependency, get_abstract_dependencies, get_dependencies
+from .common import ReqLibBaseModel
 from .markers import normalize_marker_str
 from .setup_info import (
     SetupInfo,
     _prepare_wheel_building_kwargs,
     ast_parse_setup_py,
     get_metadata,
 )
@@ -65,129 +80,120 @@
     DIRECT_URL_RE,
     HASH_STRING,
     build_vcs_uri,
     convert_direct_url_to_url,
     create_link,
     expand_env_variables,
     extras_to_string,
-    filter_none,
     format_requirement,
     get_default_pyproject_backend,
     get_pyproject,
     get_version,
     init_requirement,
-    is_pinned_requirement,
     make_install_requirement,
     normalize_name,
-    parse_extras,
+    parse_extras_str,
     specs_to_string,
     split_markers_from_line,
     split_ref_from_uri,
     split_vcs_method_from_uri,
     validate_path,
-    validate_specifiers,
     validate_vcs,
 )
+from .vcs import VCSRepository
 
 if MYPY_RUNNING:
-    from typing import (
-        Any,
-        AnyStr,
-        Dict,
-        FrozenSet,
-        Generator,
-        Iterator,
-        List,
-        Optional,
-        Sequence,
-        Set,
-        Text,
-        Tuple,
-        TypeVar,
-        Union,
-    )
-
-    from pip._internal.index.package_finder import PackageFinder
-    from pip._internal.models.candidate import InstallationCandidate
-
-    RequirementType = TypeVar(
-        "RequirementType", covariant=True, bound=PackagingRequirement
-    )
-    F = TypeVar("F", "FileRequirement", "VCSRequirement", covariant=True)
-    from urllib.parse import SplitResult
-
-    from .vcs import VCSRepository
-
-    NON_STRING_ITERABLE = Union[List, Set, Tuple]
-    STRING_TYPE = Union[str, bytes, Text]
     S = TypeVar("S", bytes, str, Text)
-    BASE_TYPES = Union[bool, STRING_TYPE, Tuple[STRING_TYPE, ...]]
-    CUSTOM_TYPES = Union[VCSRepository, RequirementType, SetupInfo, "Line"]
-    CREATION_ARG_TYPES = Union[BASE_TYPES, Link, CUSTOM_TYPES]
-    PIPFILE_ENTRY_TYPE = Union[STRING_TYPE, bool, Tuple[STRING_TYPE], List[STRING_TYPE]]
-    PIPFILE_TYPE = Union[STRING_TYPE, Dict[STRING_TYPE, PIPFILE_ENTRY_TYPE]]
-    TPIPFILE = Dict[STRING_TYPE, PIPFILE_ENTRY_TYPE]
 
 
 SPECIFIERS_BY_LENGTH = sorted(list(Specifier._operators.keys()), key=len, reverse=True)
 
 
-class Line(object):
-    def __init__(self, line, extras=None):
-        # type: (AnyStr, Optional[Union[List[S], Set[S], Tuple[S, ...]]]) -> None
-        self.editable = False  # type: bool
+class Line(ReqLibBaseModel):
+    line: str
+    extras: Optional[Union[List[str], Set[str], Tuple[str, ...]]] = None
+    editable: bool = False
+    hashes: List[str] = []
+    markers: Optional[str] = None
+    vcs: Optional[str] = None
+    path: Optional[str] = None
+    relpath: Optional[str] = None
+    uri: Optional[str] = None
+    _link: Optional[Any] = None
+    is_local: bool = False
+    _name: Optional[str] = None
+    _specifier: Optional[str] = None
+    parsed_marker: Optional[Any] = None
+    preferred_scheme: Optional[str] = None
+    _requirement: Optional[Any] = None
+    _parsed_url: Optional[Any] = None
+    _setup_cfg: Optional[str] = None
+    _setup_py: Optional[str] = None
+    _pyproject_toml: Optional[str] = None
+    _pyproject_requires: Optional[Tuple[str, ...]] = None
+    _pyproject_backend: Optional[str] = None
+    _wheel_kwargs: Optional[Dict[str, str]] = None
+    _vcsrepo: Optional[Any] = None
+    _stack: Optional[Any] = None
+    setup_info: Optional[Any] = None
+    _ref: Optional[str] = None
+    _ireq: Optional[Any] = None
+    _src_root: Optional[str] = None
+    dist: Optional[Any] = None
+
+    class Config:
+        validate_assignment = True
+        arbitrary_types_allowed = True
+        allow_mutation = True
+        include_private_attributes = True
+        keep_untouched = (cached_property,)
+
+    def __init__(
+        self,
+        line: str,
+        extras: Optional[Union[List[str], Set[str], Tuple[str, ...]]] = None,
+        name: Optional[str] = None,
+        editable: Optional[bool] = False,
+    ) -> None:
+        super().__init__(line=line, extras=extras)
         if line.startswith("-e "):
             line = line[len("-e ") :]
             self.editable = True
-        self.extras = ()  # type: Tuple[STRING_TYPE, ...]
         if extras is not None:
             self.extras = tuple(sorted(set(extras)))
-        self.line = line  # type: STRING_TYPE
-        self.hashes = []  # type: List[STRING_TYPE]
-        self.markers = None  # type: Optional[STRING_TYPE]
-        self.vcs = None  # type: Optional[STRING_TYPE]
-        self.path = None  # type: Optional[STRING_TYPE]
-        self.relpath = None  # type: Optional[STRING_TYPE]
-        self.uri = None  # type: Optional[STRING_TYPE]
-        self._link = None  # type: Optional[Link]
-        self.is_local = False  # type: bool
-        self._name = None  # type: Optional[STRING_TYPE]
-        self._specifier = None  # type: Optional[STRING_TYPE]
-        self.parsed_marker = None  # type: Optional[Marker]
-        self.preferred_scheme = None  # type: Optional[STRING_TYPE]
-        self._requirement = None  # type: Optional[PackagingRequirement]
-        self._parsed_url = None  # type: Optional[URI]
-        self._setup_cfg = None  # type: Optional[STRING_TYPE]
-        self._setup_py = None  # type: Optional[STRING_TYPE]
-        self._pyproject_toml = None  # type: Optional[STRING_TYPE]
-        self._pyproject_requires = None  # type: Optional[Tuple[STRING_TYPE, ...]]
-        self._pyproject_backend = None  # type: Optional[STRING_TYPE]
-        self._wheel_kwargs = None  # type: Optional[Dict[STRING_TYPE, STRING_TYPE]]
-        self._vcsrepo = None  # type: Optional[VCSRepository]
-        self._setup_info = None  # type: Optional[SetupInfo]
-        self._ref = None  # type: Optional[STRING_TYPE]
-        self._ireq = None  # type: Optional[InstallRequirement]
-        self._src_root = None  # type: Optional[STRING_TYPE]
-        self.dist = None  # type: Any
-        super(Line, self).__init__()
+        self.line = line
         self.parse()
 
     def __hash__(self):
+        # Convert the _requirement attribute to a hashable type if it's a dict
+        requirement_hash = (
+            hash(tuple(self._requirement.items()))
+            if isinstance(self._requirement, dict)
+            else self._requirement
+        )
+
+        # Convert the extras attribute to a hashable type if it's a dict
+        extras_hash = (
+            hash(tuple(self.extras.items()))
+            if isinstance(self.extras, dict)
+            else tuple(self.extras)
+        )
+
         return hash(
             (
                 self.editable,
                 self.line,
                 self.markers,
-                tuple(self.extras),
+                extras_hash,
                 tuple(self.hashes),
                 self.vcs,
                 self.uri,
                 self.path,
                 self.name,
-                self._requirement,
+                requirement_hash,
             )
         )
 
     def __repr__(self):
         try:
             return (
                 "<Line (editable={self.editable}, name={self._name}, path={self.path}, "
@@ -197,24 +203,26 @@
                 "pyproject_backend={self._pyproject_backend}, ireq={self._ireq})>".format(
                     self=self
                 )
             )
         except Exception:
             return "<Line {0}>".format(self.__dict__.values())
 
-    def __str__(self):
-        # type: () -> str
+    def __str__(self) -> str:
         if self.markers:
             return "{0} ; {1}".format(self.get_line(), self.markers)
         return self.get_line()
 
     def get_line(
-        self, with_prefix=False, with_markers=False, with_hashes=True, as_list=False
-    ):
-        # type: (bool, bool, bool, bool) -> Union[STRING_TYPE, List[STRING_TYPE]]
+        self,
+        with_prefix: bool = False,
+        with_markers: bool = False,
+        with_hashes: bool = True,
+        as_list: bool = False,
+    ) -> Union[str, List[str]]:
         line = self.line
         extras_str = extras_to_string(self.extras)
         with_hashes = False if self.editable or self.is_vcs else with_hashes
         hash_list = ["--hash={0}".format(h) for h in sorted(self.hashes)]
         if self.is_named:
             line = self.name_and_specifier
         elif self.is_direct_url:
@@ -249,52 +257,48 @@
             return result_list
         if with_prefix and self.editable:
             line = "-e {0}".format(line)
         if with_hashes and hash_list:
             line = "{0} {1}".format(line, " ".join(hash_list))
         return line
 
-    @property
-    def name_and_specifier(self):
+    @cached_property
+    def name_and_specifier(self) -> str:
         name_str, spec_str = "", ""
         if self.name:
             name_str = "{0}".format(self.name.lower())
             extras_str = extras_to_string(self.extras)
             if extras_str:
                 name_str = "{0}{1}".format(name_str, extras_str)
         if self.specifier:
             spec_str = "{0}".format(self.specifier)
         return "{0}{1}".format(name_str, spec_str)
 
     @classmethod
-    def split_hashes(cls, line):
-        # type: (S) -> Tuple[S, List[S]]
+    def split_hashes(cls, line: str) -> Tuple[str, List[str]]:
         if "--hash" not in line:
             return line, []
         split_line = line.split()
-        line_parts = []  # type: List[S]
-        hashes = []  # type: List[S]
+        line_parts = []  # type: List[str]
+        hashes = []  # type: List[str]
         for part in split_line:
             if part.startswith("--hash"):
                 param, _, value = part.partition("=")
                 hashes.append(value)
             else:
                 line_parts.append(part)
         line = " ".join(line_parts)
         return line, hashes
 
     @property
-    def line_with_prefix(self):
-        # type: () -> STRING_TYPE
+    def line_with_prefix(self) -> str:
         return self.get_line(with_prefix=True, with_hashes=False)
 
-    @property
-    def line_for_ireq(self):
-        # type: () -> STRING_TYPE
-        line = ""  # type: STRING_TYPE
+    def line_for_ireq(self) -> str:
+        line = ""
         if self.is_file or self.is_remote_url and not self.is_vcs:
             scheme = self.preferred_scheme if self.preferred_scheme is not None else "uri"
             local_line = next(
                 iter(
                     [
                         os.path.dirname(os.path.abspath(f))
                         for f in [self.setup_py, self.setup_cfg, self.pyproject_toml]
@@ -340,85 +344,81 @@
                     line = self.link.url
         elif self.is_vcs and not self.editable:
             line = add_ssh_scheme_to_git_uri(self.line)
         if not line:
             line = self.line
         return line
 
-    @property
+    @cached_property
     def base_path(self):
         # type: () -> Optional[S]
-        if not self.link and not self.path:
-            self.parse_link()
+        self.parse_link()
         if not self.path:
-            pass
+            return None
         path = normalize_path(self.path)
         if os.path.exists(path) and os.path.isdir(path):
             path = path
         elif os.path.exists(path) and os.path.isfile(path):
             path = os.path.dirname(path)
         else:
             path = None
         return path
 
     @property
     def setup_py(self):
-        # type: () -> Optional[STRING_TYPE]
+        # type: () -> Optional[str]
         if self._setup_py is None:
             self.populate_setup_paths()
         return self._setup_py
 
     @property
     def setup_cfg(self):
-        # type: () -> Optional[STRING_TYPE]
+        # type: () -> Optional[str]
         if self._setup_cfg is None:
             self.populate_setup_paths()
         return self._setup_cfg
 
     @property
     def pyproject_toml(self):
-        # type: () -> Optional[STRING_TYPE]
+        # type: () -> Optional[str]
         if self._pyproject_toml is None:
             self.populate_setup_paths()
         return self._pyproject_toml
 
-    @property
-    def specifier(self):
-        # type: () -> Optional[STRING_TYPE]
+    @cached_property
+    def specifier(self) -> Optional[str]:
         options = [self._specifier]
         for req in (self.ireq, self.requirement):
             if req is not None and getattr(req, "specifier", None):
                 options.append(req.specifier)
         specifier = next(
             iter(spec for spec in options if spec is not None), None
         )  # type: Optional[Union[Specifier, SpecifierSet]]
-        spec_string = None  # type: Optional[STRING_TYPE]
+        spec_string = None  # type: Optional[str]
         if specifier is not None:
             spec_string = specs_to_string(specifier)
+            self.set_specifiers(specifier)
         elif (
             specifier is None
             and not self.is_named
-            and (self._setup_info is not None and self._setup_info.version)
+            and (self.setup_info is not None and self.setup_info.version)
         ):
-            spec_string = "=={0}".format(self._setup_info.version)
+            spec_string = "=={0}".format(self.setup_info.version)
         if spec_string:
             self._specifier = spec_string
         return self._specifier
 
-    @specifier.setter
-    def specifier(self, spec):
-        # type: (str) -> None
+    def set_specifier(self, spec: str) -> None:
         if not spec.startswith("=="):
             spec = "=={0}".format(spec)
         self._specifier = spec
-        self.specifiers = SpecifierSet(spec)
+        self.set_specifiers(SpecifierSet(spec))
 
     @property
-    def specifiers(self):
-        # type: () -> Optional[SpecifierSet]
+    def specifiers(self) -> Optional[SpecifierSet]:
         ireq_needs_specifier = False
         req_needs_specifier = False
         if self.ireq is None or self.ireq.req is None or not self.ireq.req.specifier:
             ireq_needs_specifier = True
         if self.requirement is None or not self.requirement.specifier:
             req_needs_specifier = True
         if any([ireq_needs_specifier, req_needs_specifier]):
@@ -431,32 +431,29 @@
                 or self.is_path
                 or (self.is_vcs and not self.editable)
             ):
                 if self.specifier is not None:
                     specifier = self.specifier
                     if not isinstance(specifier, SpecifierSet):
                         specifier = SpecifierSet(specifier)
-                    self.specifiers = specifier
                     return specifier
-        if self.ireq is not None and self.ireq.req is not None:
-            return self.ireq.req.specifier
+        if self._ireq is not None and self._ireq.req is not None:
+            return self._ireq.req.specifier
         elif self.requirement is not None:
             return self.requirement.specifier
         return None
 
-    @specifiers.setter
-    def specifiers(self, specifiers):
-        # type: (Union[Text, str, SpecifierSet]) -> None
+    def set_specifiers(self, specifiers):
         if not isinstance(specifiers, SpecifierSet):
             if isinstance(specifiers, str):
                 specifiers = SpecifierSet(specifiers)
             else:
                 raise TypeError("Must pass a string or a SpecifierSet")
         specs = self.get_requirement_specs(specifiers)
-        if self.ireq is not None and self._ireq and self._ireq.req is not None:
+        if self._ireq and self._ireq.req is not None:
             self._ireq.req.specifier = specifiers
             self._ireq.req.specs = specs
         if self.requirement is not None:
             self.requirement.specifier = specifiers
             self.requirement.specs = specs
 
     @classmethod
@@ -466,15 +463,14 @@
         spec = next(iter(specifierset._specs), None)
         if spec:
             specs.append(spec._spec)
         return specs
 
     @property
     def requirement(self):
-        # type: () -> Optional[RequirementType]
         if self._requirement is None:
             self.parse_requirement()
             if self._requirement is None and self._name is not None:
                 self._requirement = init_requirement(canonicalize_name(self.name))
                 if self.is_file or self.is_remote_url and self._requirement is not None:
                     self._requirement.url = self.url
         if (
@@ -482,50 +478,58 @@
             and self._requirement.specifier
             and not self._requirement.specs
         ):
             specs = self.get_requirement_specs(self._requirement.specifier)
             self._requirement.specs = specs
         return self._requirement
 
-    def populate_setup_paths(self):
-        # type: () -> None
+    def populate_setup_paths(self) -> None:
         if not self.link and not self.path:
             self.parse_link()
         if not self.path:
             return
         base_path = self.base_path
         if base_path is None:
             return
-        setup_paths = get_setup_paths(
-            base_path, subdirectory=self.subdirectory
-        )  # type: Dict[STRING_TYPE, Optional[STRING_TYPE]]
+        setup_paths = get_setup_paths(base_path, subdirectory=self.subdirectory)
+        self._setup_py = setup_paths.get("setup_py")
+        self._setup_cfg = setup_paths.get("setup_cfg")
+        self._pyproject_toml = setup_paths.get("pyproject_toml")
+
+    def get_setup_paths(self) -> None:
+        if not self.link and not self.path:
+            self.parse_link()
+        base_path = self.base_path
+        if base_path is None:
+            return
+        setup_paths = get_setup_paths(base_path, subdirectory=self.subdirectory)
         self._setup_py = setup_paths.get("setup_py")
         self._setup_cfg = setup_paths.get("setup_cfg")
         self._pyproject_toml = setup_paths.get("pyproject_toml")
 
     @property
     def pyproject_requires(self):
-        # type: () -> Optional[Tuple[STRING_TYPE, ...]]
+        # type: () -> Optional[Tuple[str, ...]]
         if self._pyproject_requires is None and self.pyproject_toml is not None:
             if self.path is not None:
                 pyproject_requires, pyproject_backend = None, None
                 pyproject_results = get_pyproject(self.path)  # type: ignore
                 if pyproject_results:
                     pyproject_requires, pyproject_backend = pyproject_results
                 if pyproject_requires:
                     self._pyproject_requires = tuple(pyproject_requires)
                 self._pyproject_backend = pyproject_backend
         return self._pyproject_requires
 
     @property
     def pyproject_backend(self):
-        # type: () -> Optional[STRING_TYPE]
+        # type: () -> Optional[str]
         if self._pyproject_requires is None and self.pyproject_toml is not None:
-            pyproject_requires = None  # type: Optional[Sequence[STRING_TYPE]]
-            pyproject_backend = None  # type: Optional[STRING_TYPE]
+            pyproject_requires = None  # type: Optional[Sequence[str]]
+            pyproject_backend = None  # type: Optional[str]
             pyproject_results = get_pyproject(self.path)  # type: ignore
             if pyproject_results:
                 pyproject_requires, pyproject_backend = pyproject_results
             if not pyproject_backend and self.setup_cfg is not None:
                 setup_dict = SetupInfo.get_setup_cfg(self.setup_cfg)
                 pyproject_backend = get_default_pyproject_backend()
                 pyproject_requires = setup_dict.get(
@@ -572,61 +576,60 @@
                         direct=False,
                         strip_ssh=self.parsed_url.is_implicit_ssh,
                     )
             except ValueError:
                 self.line, extras = _strip_extras(self.line)
         else:
             self.line, extras = _strip_extras(self.line)
-        extras_set = set()  # type: Set[STRING_TYPE]
+        extras_set = set()  # type: Set[str]
         if extras is not None:
-            extras_set = set(parse_extras(extras))
+            extras_set = set(parse_extras_str(extras))
         if self._name:
             self._name, name_extras = _strip_extras(self._name)
             if name_extras:
-                name_extras = set(parse_extras(name_extras))
+                name_extras = set(parse_extras_str(name_extras))
                 extras_set |= name_extras
         if extras_set is not None:
             self.extras = tuple(sorted(extras_set))
         return self
 
     def get_url(self):
-        # type: () -> STRING_TYPE
+        # type: () -> str
         """Sets ``self.name`` if given a **PEP-508** style URL."""
         return self.parsed_url.to_string(
             escape_password=False, direct=False, strip_ref=True
         )
 
     @property
-    def name(self):
-        # type: () -> Optional[STRING_TYPE]
+    def name(self) -> Optional[str]:
         if self._name is None:
             self.parse_name()
             if self._name is None and not self.is_named and not self.is_wheel:
                 if self.setup_info:
                     self._name = self.setup_info.name
             elif self.is_wheel:
                 self._name = self._parse_wheel()
             if not self._name:
                 self._name = self.ireq.name
         return self._name
 
     @name.setter
     def name(self, name):
-        # type: (STRING_TYPE) -> None
+        # type: (str) -> None
         self._name = name
-        if self._setup_info:
-            self._setup_info.name = name
+        if self.setup_info:
+            self.setup_info.name = name
         if self.requirement and self._requirement:
             self._requirement.name = name
         if self.ireq and self._ireq and self._ireq.req:
             self._ireq.req.name = name
 
     @property
     def url(self):
-        # type: () -> Optional[STRING_TYPE]
+        # type: () -> Optional[str]
         try:
             return self.parsed_url.to_string(
                 escape_password=False,
                 strip_ref=True,
                 strip_name=True,
                 strip_subdir=True,
                 strip_ssh=False,
@@ -639,15 +642,15 @@
         # type: () -> Link
         if self._link is None:
             self.parse_link()
         return self._link
 
     @property
     def subdirectory(self):
-        # type: () -> Optional[STRING_TYPE]
+        # type: () -> Optional[str]
         if self.link is not None:
             return self.link.subdirectory_fragment
         return ""
 
     @property
     def is_wheel(self):
         # type: () -> bool
@@ -757,15 +760,15 @@
             or self.is_file
             or self.is_vcs
             or self.is_direct_url
         )
 
     @property
     def ref(self):
-        # type: () -> Optional[STRING_TYPE]
+        # type: () -> Optional[str]
         if self._ref is None and self.relpath is not None:
             self.relpath, self._ref = split_ref_from_uri(self.relpath)
         return self._ref
 
     @property
     def ireq(self):
         # type: () -> Optional[InstallRequirement]
@@ -785,43 +788,27 @@
 
     @property
     def wheel_kwargs(self):
         if not self._wheel_kwargs:
             self._wheel_kwargs = _prepare_wheel_building_kwargs(self.ireq)
         return self._wheel_kwargs
 
-    def get_setup_info(self):
-        # type: () -> SetupInfo
-        setup_info = None
-        with global_tempdir_manager():
-            setup_info = SetupInfo.from_ireq(self.ireq, subdir=self.subdirectory)
-            if not setup_info.name:
-                setup_info.get_info()
+    def get_setup_info(self) -> SetupInfo:
+        setup_info = self.setup_info
+        if setup_info is None:
+            with global_tempdir_manager():
+                setup_info = SetupInfo.from_ireq(self.ireq, subdir=self.subdirectory)
+                if not setup_info.name:
+                    setup_info.get_info()
         return setup_info
 
-    @property
-    def setup_info(self):
-        # type: () -> Optional[SetupInfo]
-        if not self._setup_info and not self.is_named and not self.is_wheel:
-            # make two attempts at this before failing to allow for stale data
-            try:
-                self.setup_info = self.get_setup_info()
-            except FileNotFoundError:
-                try:
-                    self.setup_info = self.get_setup_info()
-                except FileNotFoundError:
-                    raise
-        return self._setup_info
-
-    @setup_info.setter
-    def setup_info(self, setup_info):
-        # type: (SetupInfo) -> None
-        self._setup_info = setup_info
+    def set_setup_info(self, setup_info) -> None:
+        self.setup_info = setup_info
         if setup_info.version:
-            self.specifier = setup_info.version
+            self.set_specifiers(f"=={setup_info.version}")
         if setup_info.name and not self.name:
             self.name = setup_info.name
 
     def _get_vcsrepo(self):
         # type: () -> Optional[VCSRepository]
         from .vcs import VCSRepository
 
@@ -846,25 +833,24 @@
     def vcsrepo(self):
         # type: () -> Optional[VCSRepository]
         if self._vcsrepo is None and self.is_vcs:
             self._vcsrepo = self._get_vcsrepo()
         return self._vcsrepo
 
     @property
-    def parsed_url(self):
-        # type: () -> URI
+    def parsed_url(self) -> URI:
         if self._parsed_url is None:
             self._parsed_url = URI.parse(self.line)
         return self._parsed_url
 
     @property
     def is_direct_url(self):
         # type: () -> bool
         try:
-            return self.is_url and self.parsed_url.is_direct_url
+            return self.is_url and self._parsed_url.is_direct_url
         except ValueError:
             return self.is_url and bool(DIRECT_URL_RE.match(self.line))
 
     @cached_property
     def metadata(self):
         # type: () -> Dict[Any, Any]
         if self.is_local and self.path and is_installable_dir(self.path):
@@ -887,82 +873,78 @@
     def parsed_setup_py(self):
         # type: () -> Dict[Any, Any]
         if self.is_local and self.path and is_installable_dir(self.path):
             if self.setup_py:
                 return ast_parse_setup_py(self.setup_py, raising=False)
         return {}
 
-    @vcsrepo.setter
-    def vcsrepo(self, repo):
+    def set_vcsrepo(self, repo):
         # type (VCSRepository) -> None
         self._vcsrepo = repo
         ireq = self.ireq
         wheel_kwargs = self.wheel_kwargs.copy()
         wheel_kwargs["src_dir"] = repo.checkout_directory
         with global_tempdir_manager(), temp_path():
             ireq.ensure_has_source_dir(wheel_kwargs["src_dir"])
             sys.path = [repo.checkout_directory, "", ".", get_path("purelib")]
             setupinfo = SetupInfo.create(
                 repo.checkout_directory,
                 ireq=ireq,
                 subdirectory=self.subdirectory,
                 kwargs=wheel_kwargs,
             )
-            self._setup_info = setupinfo
-            self._setup_info.reload()
+            self.setup_info = setupinfo
 
-    def get_ireq(self):
-        # type: () -> InstallRequirement
-        line = self.line_for_ireq
+    def get_ireq(self) -> InstallRequirement:
+        line = self.line_for_ireq()
         if self.editable:
             ireq = install_req_from_editable(line)
         else:
             ireq = install_req_from_line(line)
         if self.is_named:
             ireq = install_req_from_line(self.line)
         if self.is_file or self.is_remote_url:
             ireq.link = Link(expand_env_variables(self.link.url))
         if self.extras and not ireq.extras:
             ireq.extras = set(self.extras)
         if self.parsed_marker is not None and not ireq.markers:
             ireq.markers = self.parsed_marker
         if not ireq.req and self._requirement is not None:
-            ireq.req = copy.deepcopy(self._requirement)
+            ireq.req = self._requirement
         return ireq
 
     def parse_ireq(self):
         # type: () -> None
         if self._ireq is None:
             self._ireq = self.get_ireq()
         if self._ireq is not None:
             if self.requirement is not None and self._ireq.req is None:
                 self._ireq.req = self.requirement
 
     def _parse_wheel(self):
-        # type: () -> Optional[STRING_TYPE]
+        # type: () -> Optional[str]
         if not self.is_wheel:
             return
         _wheel = Wheel(self.link.filename)
         name = _wheel.name
         version = _wheel.version
         self._specifier = "=={0}".format(version)
         return name
 
     def _parse_name_from_link(self):
-        # type: () -> Optional[STRING_TYPE]
+        # type: () -> Optional[str]
         if self.link is None:
             return None
         if getattr(self.link, "egg_fragment", None):
             return self.link.egg_fragment
         elif self.is_wheel:
             return self._parse_wheel()
         return None
 
-    def _parse_name_from_line(self):
-        # type: () -> Optional[STRING_TYPE]
+    def _parse_name_from_line(self) -> Optional[str]:
         if not self.is_named:
             pass
         try:
             self._requirement = init_requirement(self.line)
         except Exception:
             raise RequirementError(
                 "Failed parsing requirement from {0!r}".format(self.line)
@@ -973,27 +955,30 @@
         if self._requirement.extras and not self.extras:
             self.extras = self._requirement.extras
         if not name:
             name = self.line
             specifier_match = next(
                 iter(spec for spec in SPECIFIERS_BY_LENGTH if spec in self.line), None
             )
-            specifier = None  # type: Optional[STRING_TYPE]
+            specifier = None  # type: Optional[str]
             if specifier_match:
                 specifier = "{0!s}".format(specifier_match)
             if specifier is not None and specifier in name:
-                version = None  # type: Optional[STRING_TYPE]
                 name, specifier, version = name.partition(specifier)
                 self._specifier = "{0}{1}".format(specifier, version)
         return name
 
     def _parse_name_from_path(self):
         # type: () -> Optional[S]
-        if self.path and self.is_local and is_installable_dir(self.path):
-            metadata = get_metadata(self.path)
+        path = self.path
+        if path and path.startswith("file:"):
+            parsed_url = urlparse(path)
+            path = url2pathname(parsed_url.path)
+        if path and self.is_local and is_installable_dir(path):
+            metadata = get_metadata(path)
             if metadata:
                 name = metadata.get("name", "")
                 if name and name != "wheel":
                     return name
             parsed_setup_cfg = self.parsed_setup_cfg
             if parsed_setup_cfg:
                 name = parsed_setup_cfg.get("name", "")
@@ -1003,40 +988,36 @@
             parsed_setup_py = self.parsed_setup_py
             if parsed_setup_py:
                 name = parsed_setup_py.get("name", "")
                 if name and isinstance(name, str):
                     return name
         return None
 
-    def parse_name(self):
-        # type: () -> "Line"
-        if self._name is None:
-            name = None
-            if self.link is not None and self.line_is_installable:
-                name = self._parse_name_from_link()
-            if name is None and (
-                (self.is_remote_url or self.is_artifact or self.is_vcs)
-                and self._parsed_url
-            ):
-                if self._parsed_url.fragment:
-                    _, _, name = self._parsed_url.fragment.partition("egg=")
-                    if "&" in name:
-                        # subdirectory fragments might also be in here
-                        name, _, _ = name.partition("&")
-            if name is None and self.is_named:
-                name = self._parse_name_from_line()
-            elif name is None and (self.is_file or self.is_remote_url or self.is_path):
-                if self.is_local:
-                    name = self._parse_name_from_path()
-            if name is not None:
-                name, extras = _strip_extras(name)
-                if extras is not None and not self.extras:
-                    self.extras = tuple(sorted(set(parse_extras(extras))))
-                self._name = name
-        return self
+    def parse_name(self) -> None:
+        name = None
+        if self.link is not None and self.line_is_installable:
+            name = self._parse_name_from_link()
+        if name is None and (
+            (self.is_remote_url or self.is_artifact or self.is_vcs) and self.parsed_url
+        ):
+            if self._parsed_url.fragment:
+                _, _, name = self._parsed_url.fragment.partition("egg=")
+                if "&" in name:
+                    # subdirectory fragments might also be in here
+                    name, _, _ = name.partition("&")
+        if name is None and self.is_named:
+            name = self._parse_name_from_line()
+        elif name is None and (self.is_file or self.is_remote_url or self.is_path):
+            if self.is_local:
+                name = self._parse_name_from_path()
+        if name is not None:
+            name, extras = _strip_extras(name)
+            if extras is not None and not self.extras:
+                self.extras = tuple(sorted(set(parse_extras_str(extras))))
+        self._name = name
 
     def _parse_requirement_from_vcs(self):
         # type: () -> Optional[PackagingRequirement]
         url = self.url if self.url else self.link.url
         if url:
             url = unquote(url)
         if (
@@ -1062,19 +1043,18 @@
                 self._requirement.link = self.link
         # else:
         #     req.link = self.link
         if self.ref and self._requirement is not None:
             self._requirement.revision = self.ref
             if self._vcsrepo is not None:
                 with global_tempdir_manager():
-                    self._requirement.revision = self._vcsrepo.get_commit_hash()
+                    self._requirement.revision = self._vcsrepo.commit_hash
         return self._requirement
 
-    def parse_requirement(self):
-        # type: () -> "Line"
+    def parse_requirement(self) -> "Line":
         if self._name is None:
             self.parse_name()
             if not any([self._name, self.is_vcs, self.is_named]):
                 if self.setup_info and self.setup_info.name:
                     self._name = self.setup_info.name
         name, extras, url = self.requirement_info
         if name:
@@ -1158,24 +1138,26 @@
         )
         ref = None
         if link is not None and "@" in unquote(link.path) and uri is not None:
             uri, _, ref = unquote(uri).rpartition("@")
         if relpath is not None and "@" in relpath:
             relpath, _, ref = relpath.rpartition("@")
         if path is not None and "@" in path:
-            path, _ = split_ref_from_uri(path)
+            path, prefix = split_ref_from_uri(path)
         link_url = link.url_without_fragment
         if "@" in link_url:
             link_url, _ = split_ref_from_uri(link_url)
         self.preferred_scheme = prefer
         self.relpath = relpath
         self.path = path
-        # self.uri = uri
+        self.uri = uri
         if prefer in ("path", "relpath") or uri.startswith("file"):
             self.is_local = True
+            if uri.startswith("file"):
+                self.path = uri
         if parsed_url.is_vcs or parsed_url.is_direct_url and parsed_link:
             self._link = parsed_link
         else:
             self._link = link
         return self
 
     def parse_markers(self):
@@ -1186,24 +1168,23 @@
 
     @property
     def requirement_info(self):
         # type: () -> Tuple[Optional[S], Tuple[Optional[S], ...], Optional[S]]
         """
         Generates a 3-tuple of the requisite *name*, *extras* and *url* to generate a
         :class:`~packaging.requirements.Requirement` out of.
-
         :return: A Tuple of an optional name, a Tuple of extras, and an optional URL.
         :rtype: Tuple[Optional[S], Tuple[Optional[S], ...], Optional[S]]
         """
 
         # Direct URLs can be converted to packaging requirements directly, but
         # only if they are `file://` (with only two slashes)
         name = None  # type: Optional[S]
         extras = ()  # type: Tuple[Optional[S], ...]
-        url = None  # type: Optional[STRING_TYPE]
+        url = None  # type: Optional[str]
         # if self.is_direct_url:
         if self._name:
             name = canonicalize_name(self._name)
         if self.is_file or self.is_url or self.is_path or self.is_file_url or self.is_vcs:
             url = ""
             if self.is_vcs:
                 url = self.url if self.url else self.uri
@@ -1296,47 +1277,44 @@
             else:
                 raise RequirementError(
                     "Supplied requirement is not installable: {0!r}".format(self.line)
                 )
         elif self.is_named and self._name is None:
             self.parse_name()
         self.parse_link()
-        # self.parse_requirement()
-        # self.parse_ireq()
 
 
-@attr.s(slots=True, hash=True)
-class NamedRequirement(object):
-    name = attr.ib()  # type: STRING_TYPE
-    version = attr.ib()  # type: Optional[STRING_TYPE]
-    req = attr.ib()  # type: PackagingRequirement
-    extras = attr.ib(default=attr.Factory(list))  # type: Tuple[STRING_TYPE, ...]
-    editable = attr.ib(default=False)  # type: bool
-    _parsed_line = attr.ib(default=None)  # type: Optional[Line]
+class NamedRequirement(ReqLibBaseModel):
+    name: str
+    version: Optional[str]
+    req: PackagingRequirement
+    extras: Optional[Tuple[str, ...]] = Field(default_factory=list)
+    editable: bool = False
+    parsed_line: Optional[Line] = None
+
+    class Config:
+        validate_assignment = True
+        arbitrary_types_allowed = True
+        allow_mutation = True
+        include_private_attributes = True
+        keep_untouched = (cached_property,)
 
-    @req.default
-    def get_requirement(self):
-        # type: () -> RequirementType
-        req = init_requirement(
-            "{0}{1}".format(canonicalize_name(self.name), self.version)
-        )
-        return req
+    def __init__(self, **data):
+        super().__init__(**data)
 
-    @property
-    def parsed_line(self):
-        # type: () -> Optional[Line]
-        if self._parsed_line is None:
-            self._parsed_line = Line(self.line_part)
-        return self._parsed_line
+        self.parsed_line = Line(line=self.line_part)
+
+        # Set default values using the methods
+        if not self.req:
+            self.req = self.get_requirement()
 
     @classmethod
-    def from_line(cls, line, parsed_line=None):
-        # type: (AnyStr, Optional[Line]) -> NamedRequirement
+    def from_line(cls, line, parsed_line=None) -> "NamedRequirement":
         req = init_requirement(line)
-        specifiers = None  # type: Optional[STRING_TYPE]
+        specifiers = None  # type: Optional[str]
         if req.specifier:
             specifiers = specs_to_string(req.specifier)
         req.line = line
         name = getattr(req, "name", None)
         if not name:
             name = getattr(req, "project_name", None)
             req.name = name
@@ -1346,178 +1324,191 @@
         creation_kwargs = {
             "name": name,
             "version": specifiers,
             "req": req,
             "parsed_line": parsed_line,
             "extras": None,
         }
-        extras = None  # type: Optional[Tuple[STRING_TYPE, ...]]
+        extras = None  # type: Optional[Tuple[str, ...]]
         if req.extras:
             extras = tuple(req.extras)
         creation_kwargs["extras"] = extras
         return cls(**creation_kwargs)
 
     @classmethod
-    def from_pipfile(cls, name, pipfile):
-        # type: (S, TPIPFILE) -> NamedRequirement
-        creation_args = {}  # type: TPIPFILE
+    def from_pipfile(cls, name: str, pipfile: Dict[str, Any]) -> "NamedRequirement":
+        creation_args = {}
         if hasattr(pipfile, "keys"):
-            attr_fields = [field.name for field in attr.fields(cls)]
-            creation_args = {
-                k: v for k, v in pipfile.items() if k in attr_fields
-            }  # type: ignore
+            # Get field names from the Pydantic model
+            pydantic_fields = cls.__fields__.keys()
+            creation_args = {k: v for k, v in pipfile.items() if k in pydantic_fields}
         creation_args["name"] = name
-        version = get_version(pipfile)  # type: Optional[STRING_TYPE]
+        version = get_version(pipfile)
         extras = creation_args.get("extras", None)
-        creation_args["version"] = version  # type: ignore
+        creation_args["version"] = version
         req = init_requirement("{0}{1}".format(name, version))
         if req and extras and req.extras and isinstance(req.extras, tuple):
             if isinstance(extras, str):
-                req.extras = (extras) + tuple(["{0}".format(xtra) for xtra in req.extras])
+                req.extras = (extras,) + tuple(
+                    ["{0}".format(xtra) for xtra in req.extras]
+                )
             elif isinstance(extras, (tuple, list)):
                 req.extras += tuple(extras)
         creation_args["req"] = req
-        return cls(**creation_args)  # type: ignore
+        return cls(**creation_args)
 
-    @property
-    def line_part(self):
-        # type: () -> STRING_TYPE
-        # FIXME: This should actually be canonicalized but for now we have to
-        # simply lowercase it and replace underscores, since full canonicalization
-        # also replaces dots and that doesn't actually work when querying the index
+    @cached_property
+    def line_part(self) -> str:
         return normalize_name(self.name)
 
-    @property
-    def pipfile_part(self):
-        # type: () -> Dict[STRING_TYPE, Any]
-        pipfile_dict = attr.asdict(self, filter=filter_none).copy()  # type: ignore
-        if "version" not in pipfile_dict:
+    @cached_property
+    def pipfile_part(self) -> Dict[str, Any]:
+        pipfile_dict = self.dict()
+        if "version" not in pipfile_dict or pipfile_dict["version"] is None:
             pipfile_dict["version"] = "*"
-        if "_parsed_line" in pipfile_dict:
-            pipfile_dict.pop("_parsed_line")
+        if "parsed_line" in pipfile_dict:
+            pipfile_dict.pop("parsed_line")
+        if pipfile_dict.get("editable") is False:
+            pipfile_dict.pop("editable")
+        if pipfile_dict.get("line_part"):
+            pipfile_dict.pop("line_part")
+        if not pipfile_dict.get("extras", True):
+            pipfile_dict.pop("extras")
         name = pipfile_dict.pop("name")
         return {name: pipfile_dict}
 
 
 LinkInfo = collections.namedtuple(
     "LinkInfo", ["vcs_type", "prefer", "relpath", "path", "uri", "link"]
 )
 
 
-@attr.s(slots=True, eq=True, order=True, hash=True)
-class FileRequirement(object):
+class FileRequirement(ReqLibBaseModel):
     """File requirements for tar.gz installable files or wheels or setup.py
     containing directories."""
 
-    #: Path to the relevant `setup.py` location
-    setup_path = attr.ib(default=None, eq=True, order=True)  # type: Optional[STRING_TYPE]
-    #: path to hit - without any of the VCS prefixes (like git+ / http+ / etc)
-    path = attr.ib(default=None, eq=True, order=True)  # type: Optional[STRING_TYPE]
-    #: Whether the package is editable
-    editable = attr.ib(default=False, eq=True, order=True)  # type: bool
-    #: Extras if applicable
-    extras = attr.ib(
-        default=attr.Factory(tuple), eq=True, order=True
-    )  # type: Tuple[STRING_TYPE, ...]
-    _uri_scheme = attr.ib(
-        default=None, eq=True, order=True
-    )  # type: Optional[STRING_TYPE]
-    #: URI of the package
-    uri = attr.ib(eq=True, order=True)  # type: Optional[STRING_TYPE]
-    #: Link object representing the package to clone
-    link = attr.ib(eq=True, order=True)  # type: Optional[Link]
-    #: PyProject Requirements
-    pyproject_requires = attr.ib(
-        factory=tuple, eq=True, order=True
-    )  # type: Optional[Tuple[STRING_TYPE, ...]]
-    #: PyProject Build System
-    pyproject_backend = attr.ib(
-        default=None, eq=True, order=True
-    )  # type: Optional[STRING_TYPE]
-    #: PyProject Path
-    pyproject_path = attr.ib(
-        default=None, eq=True, order=True
-    )  # type: Optional[STRING_TYPE]
-    subdirectory = attr.ib(default=None)  # type: Optional[STRING_TYPE]
-    #: Setup metadata e.g. dependencies
-    _setup_info = attr.ib(default=None, eq=True, order=True)  # type: Optional[SetupInfo]
-    _has_hashed_name = attr.ib(default=False, eq=True, order=True)  # type: bool
-    _parsed_line = attr.ib(
-        default=None, eq=False, order=False, hash=True
-    )  # type: Optional[Line]
-    #: Package name
-    name = attr.ib(eq=True, order=True)  # type: Optional[STRING_TYPE]
-    #: A :class:`~pkg_resources.Requirement` instance
-    req = attr.ib(eq=True, order=True)  # type: Optional[PackagingRequirement]
+    setup_path: Optional[str] = None
+    path: Optional[str] = None
+    editable: bool = False
+    extras: Optional[Tuple[str, ...]] = ()
+    uri_scheme: Optional[str] = None
+    uri: Optional[str] = Field(default_factory=lambda: "")
+    name: Optional[str] = Field(default_factory=lambda: "")
+    link: Optional[Link] = Field(default_factory=lambda: None)
+    pyproject_requires: Optional[Tuple[str, ...]] = ()
+    pyproject_backend: Optional[str] = None
+    pyproject_path: Optional[Any] = None
+    subdirectory: Optional[str] = None
+    setup_info: Optional[SetupInfo] = None
+    _has_hashed_name: bool = False
+    parsed_line: Optional[Line] = None
+    req: Optional[PackagingRequirement] = Field(default_factory=lambda: None)
+
+    class Config:
+        validate_assignment = True
+        arbitrary_types_allowed = True
+        allow_mutation = True
+        include_private_attributes = True
+        keep_untouched = (cached_property,)
+
+    def __init__(self, **data):
+        super().__init__(**data)
+        # Set default values using the methods
+        if not self.name:
+            self.name = self.get_name()
+        if not self.link:
+            self.link = self.get_link()
+        if not self.req:
+            self.req = self.get_requirement()
+        if not self.uri:
+            self.uri = self.get_uri()
+        if not self.path and self.uri:
+            self.path = self.uri
+            self.uri_scheme = "file"
+        elif self.path and self.path.startswith("file:"):
+            self.uri_scheme = "file"
+        elif self.path:
+            self.uri_scheme = "path"
+        # self.parse_setup_info()
+        if self.parsed_line is None:
+            self.parsed_line = Line(line=self.line_part)
+        if self.name is None and self.parsed_line:
+            if self.parsed_line.setup_info:
+                self.setup_info = self.parsed_line.setup_info
+                if self.parsed_line.setup_info.name:
+                    self.name = self.parsed_line.setup_info.name
+        if self.req is None and (
+            self.parsed_line is not None and self.parsed_line.requirement is not None
+        ):
+            self.req = self.parsed_line.requirement
+        if self.parsed_line and self.parsed_line.ireq and not self.parsed_line.ireq.req:
+            if self.req is not None and self.parsed_line._ireq is not None:
+                self.parsed_line._ireq.req = self.req
 
     @classmethod
     def get_link_from_line(cls, line):
-        # type: (STRING_TYPE) -> LinkInfo
-        """Parse link information from given requirement line.
-
-        Return a 6-tuple:
+        # type: (str) -> LinkInfo
+        """Parse link information from given requirement line. Return a
+        6-tuple:
 
         - `vcs_type` indicates the VCS to use (e.g. "git"), or None.
         - `prefer` is either "file", "path" or "uri", indicating how the
             information should be used in later stages.
         - `relpath` is the relative path to use when recording the dependency,
             instead of the absolute path/URI used to perform installation.
             This can be None (to prefer the absolute path or URI).
         - `path` is the absolute file path to the package. This will always use
             forward slashes. Can be None if the line is a remote URI.
         - `uri` is the absolute URI to the package. Can be None if the line is
             not a URI.
-        - `link` is an instance of :class:`pip._internal.index.Link`,
+        - `link` is an instance of :class:`pipenv.patched.pip._internal.index.Link`,
             representing a URI parse result based on the value of `uri`.
-
         This function is provided to deal with edge cases concerning URIs
         without a valid netloc. Those URIs are problematic to a straight
         ``urlsplit` call because they cannot be reliably reconstructed with
         ``urlunsplit`` due to a bug in the standard library:
-
         >>> from urllib.parse import urlsplit, urlunsplit
         >>> urlunsplit(urlsplit('git+file:///this/breaks'))
         'git+file:/this/breaks'
         >>> urlunsplit(urlsplit('file:///this/works'))
         'file:///this/works'
-
         See `https://bugs.python.org/issue23505#msg277350`.
         """
 
         # Git allows `git@github.com...` lines that are not really URIs.
-        # Add "ssh://" so we can parse correctly, and restore afterwards.
-        fixed_line = add_ssh_scheme_to_git_uri(line)  # type: STRING_TYPE
+        # Add "ssh://" so we can parse correctly, and restore afterward.
+        fixed_line = add_ssh_scheme_to_git_uri(line)  # type: str
         added_ssh_scheme = fixed_line != line  # type: bool
 
         # We can assume a lot of things if this is a local filesystem path.
         if "://" not in fixed_line:
             p = Path(fixed_line).absolute()  # type: Path
-            path = p.as_posix()  # type: Optional[STRING_TYPE]
-            uri = p.as_uri()  # type: STRING_TYPE
+            path = p.as_posix()  # type: Optional[str]
+            uri = p.as_uri()  # type: str
             link = create_link(uri)  # type: Link
-            relpath = None  # type: Optional[STRING_TYPE]
+            relpath = None  # type: Optional[str]
             try:
                 relpath = get_converted_relative_path(path)
             except ValueError:
                 relpath = None
             return LinkInfo(None, "path", relpath, path, uri, link)
 
         # This is an URI. We'll need to perform some elaborated parsing.
 
         parsed_url = urllib_parse.urlsplit(fixed_line)  # type: SplitResult
         original_url = parsed_url._replace()  # type: SplitResult
 
         # Split the VCS part out if needed.
-        original_scheme = parsed_url.scheme  # type: STRING_TYPE
-        vcs_type = None  # type: Optional[STRING_TYPE]
+        original_scheme = parsed_url.scheme  # type: str
+        vcs_type = None  # type: Optional[str]
         if "+" in original_scheme:
-            scheme = None  # type: Optional[STRING_TYPE]
+            scheme = None  # type: Optional[str]
             vcs_type, _, scheme = original_scheme.partition("+")
             parsed_url = parsed_url._replace(scheme=scheme)  # type: ignore
-            prefer = "uri"  # type: STRING_TYPE
+            prefer = "uri"  # type: str
         else:
             vcs_type = None
             prefer = "file"
 
         if parsed_url.scheme == "file" and parsed_url.path:
             # This is a "file://" URI. Use url_to_path and path_to_url to
             # ensure the path is absolute. Also we need to build relpath.
@@ -1548,160 +1539,122 @@
                 parsed_url._replace(scheme=original_scheme)
             )  # type: ignore
         )
 
         return LinkInfo(vcs_type, prefer, relpath, path, uri, link)
 
     @property
-    def setup_py_dir(self):
-        # type: () -> Optional[STRING_TYPE]
+    def setup_py_dir(self) -> Optional[str]:
         if self.setup_path:
             return os.path.dirname(os.path.abspath(self.setup_path))
         return None
 
     @property
     def dependencies(self):
         # type: () -> Tuple[Dict[S, PackagingRequirement], List[Union[S, PackagingRequirement]], List[S]]
         build_deps = []  # type: List[Union[S, PackagingRequirement]]
         setup_deps = []  # type: List[S]
         deps = {}  # type: Dict[S, PackagingRequirement]
-        if self.setup_info:
-            setup_info = self.setup_info.as_dict()
-            deps.update(setup_info.get("requires", {}))
-            setup_deps.extend(setup_info.get("setup_requires", []))
-            build_deps.extend(setup_info.get("build_requires", []))
-            if self.extras and self.setup_info.extras:
-                for dep in self.extras:
-                    if dep not in self.setup_info.extras:
-                        continue
-                    extras_list = self.setup_info.extras.get(dep, [])  # type: ignore
-                    for req_instance in extras_list:  # type: ignore
-                        deps[req_instance.key] = req_instance
         if self.pyproject_requires:
             build_deps.extend(list(self.pyproject_requires))
+        else:
+            if not self.setup_info:
+                self.parse_setup_info()
+            if self.setup_info:
+                setup_info = self.setup_info.as_dict()
+                deps.update(setup_info.get("requires", {}))
+                setup_deps.extend(setup_info.get("setup_requires", []))
+                build_deps.extend(setup_info.get("build_requires", []))
+                if self.extras and self.setup_info.extras:
+                    for dep in self.extras:
+                        if dep not in self.setup_info.extras:
+                            continue
+                        extras_list = self.setup_info.extras.get(dep, [])  # type: ignore
+                        for req_instance in extras_list:  # type: ignore
+                            deps[req_instance.key] = req_instance
         setup_deps = list(set(setup_deps))
         build_deps = list(set(build_deps))
         return deps, setup_deps, build_deps
 
-    def __attrs_post_init__(self):
-        # type: () -> None
-        if self.name is None and self.parsed_line:
-            if self.parsed_line.setup_info:
-                self._setup_info = self.parsed_line.setup_info
-                if self.parsed_line.setup_info.name:
-                    self.name = self.parsed_line.setup_info.name
-        if self.req is None and (
-            self._parsed_line is not None and self._parsed_line.requirement is not None
-        ):
-            self.req = self._parsed_line.requirement
-        if (
-            self._parsed_line
-            and self._parsed_line.ireq
-            and not self._parsed_line.ireq.req
-        ):
-            if self.req is not None and self._parsed_line._ireq is not None:
-                self._parsed_line._ireq.req = self.req
-
-    @property
-    def setup_info(self):
-        # type: () -> Optional[SetupInfo]
-        if self._setup_info is None and self.parsed_line:
-            if self.parsed_line and self._parsed_line and self.parsed_line.setup_info:
-                if (
-                    self._parsed_line._setup_info
-                    and not self._parsed_line._setup_info.name
-                ):
+    def parse_setup_info(self) -> Optional[SetupInfo]:
+        if self.setup_info is None and self.parsed_line:
+            if self.parsed_line and self.parsed_line and self.parsed_line.setup_info:
+                if self.parsed_line.setup_info and not self.parsed_line.setup_info.name:
                     with global_tempdir_manager():
-                        self._parsed_line._setup_info.get_info()
-                self._setup_info = self.parsed_line._setup_info
+                        self.parsed_line.setup_info.get_info()
+                self.setup_info = self.parsed_line.setup_info
             elif self.parsed_line and (
                 self.parsed_line.ireq and not self.parsed_line.is_wheel
             ):
                 with global_tempdir_manager():
-                    self._setup_info = SetupInfo.from_ireq(
+                    self.setup_info = SetupInfo.from_ireq(
                         self.parsed_line.ireq, subdir=self.subdirectory
                     )
             else:
                 if self.link and not self.link.is_wheel:
-                    self._setup_info = Line(self.line_part).setup_info
+                    self.setup_info = Line(self.line_part).setup_info
                     with global_tempdir_manager():
-                        self._setup_info.get_info()
-        return self._setup_info
+                        self.setup_info.get_info()
+        return self.setup_info
+
+    def set_setup_info(self, setup_info) -> None:
+        self.setup_info = setup_info
+        if self.parsed_line:
+            self.parsed_line.setup_info = setup_info
 
-    @setup_info.setter
-    def setup_info(self, setup_info):
-        # type: (SetupInfo) -> None
-        self._setup_info = setup_info
-        if self._parsed_line:
-            self._parsed_line._setup_info = setup_info
-
-    @uri.default
-    def get_uri(self):
-        # type: () -> STRING_TYPE
+    def get_uri(self) -> str:
         if self.path and not self.uri:
-            self._uri_scheme = "path"
+            self.uri_scheme = "path"
             return path_to_url(os.path.abspath(self.path))
         elif (
             getattr(self, "req", None)
             and self.req is not None
             and getattr(self.req, "url", None)
         ):
             return self.req.url
         elif self.link is not None:
             return self.link.url_without_fragment
         return ""
 
-    @name.default
-    def get_name(self):
-        # type: () -> STRING_TYPE
+    def get_name(self) -> str:
         if self.parsed_line and self.parsed_line.name:
             return self.parsed_line.name
         elif self.link and self.link.egg_fragment:
             return self.link.egg_fragment
         elif self.setup_info and self.setup_info.name:
             return self.setup_info.name
 
-    @link.default
     def get_link(self) -> Link:
         target = "{0}".format(self.uri)
         if hasattr(self, "name") and not self._has_hashed_name:
             target = "{0}#egg={1}".format(target, self.name)
         link = create_link(target)
         return link
 
-    @req.default
-    def get_requirement(self):
-        # type () -> RequirementType
+    def get_requirement(self) -> PackagingRequirement:
         if self.name is None:
-            if self._parsed_line is not None and self._parsed_line.name is not None:
-                self.name = self._parsed_line.name
+            if self.parsed_line is not None and self.parsed_line.name is not None:
+                self.name = self.parsed_line.name
             else:
                 raise ValueError(
                     "Failed to generate a requirement: missing name for {0!r}".format(
                         self
                     )
                 )
-        if self._parsed_line:
+        if self.parsed_line:
             try:
                 # initialize specifiers to make sure we capture them
-                self._parsed_line.specifiers
+                self.parsed_line.specifiers
             except Exception:
                 pass
-            req = copy.deepcopy(self._parsed_line.requirement)
+            req = copy.deepcopy(self.parsed_line.requirement)
             if req:
                 return req
 
     @property
-    def parsed_line(self):
-        # type: () -> Optional[Line]
-        if self._parsed_line is None:
-            self._parsed_line = Line(self.line_part)
-        return self._parsed_line
-
-    @property
     def is_local(self):
         # type: () -> bool
         uri = getattr(self, "uri", None)
         if uri is None:
             if getattr(self, "path", None) and self.path is not None:
                 uri = path_to_url(os.path.abspath(self.path))
             elif (
@@ -1710,80 +1663,74 @@
                 and (getattr(self.req, "url", None) and self.req.url is not None)
             ):
                 uri = self.req.url
             if uri and is_file_url(uri):
                 return True
         return False
 
-    @property
+    @cached_property
     def is_remote_artifact(self):
         # type: () -> bool
         if self.link is None:
             return False
         return (
-            self._parsed_line
-            and not self._parsed_line.is_local
-            and (self._parsed_line.is_artifact or self._parsed_line.is_wheel)
+            self.parsed_line
+            and not self.parsed_line.is_local
+            and (self.parsed_line.is_artifact or self.parsed_line.is_wheel)
             and not self.editable
         )
 
     @property
     def is_direct_url(self):
         # type: () -> bool
-        if self._parsed_line is not None and self._parsed_line.is_direct_url:
+        if self.parsed_line is not None and self.parsed_line.is_direct_url:
             return True
         return self.is_remote_artifact
 
     @property
     def formatted_path(self):
-        # type: () -> Optional[STRING_TYPE]
+        # type: () -> Optional[str]
         if self.path:
             path = self.path
             if not isinstance(path, Path):
                 path = Path(path)
             return path.as_posix()
         return None
 
     @classmethod
-    def from_line(cls, line, editable=None, extras=None, parsed_line=None):
-        # type: (AnyStr, Optional[bool], Optional[Tuple[AnyStr, ...]], Optional[Line]) -> F
-        parsed_line = Line(line)
+    def from_line(
+        cls, line, editable=None, extras=None, parsed_line=None
+    ) -> Union["FileRequirement", "VCSRequirement"]:
+        parsed_line = Line(line=line)
         file_req_from_parsed_line(parsed_line)
 
     @classmethod
-    def from_pipfile(cls, name, pipfile):
-        # type: (STRING_TYPE, Dict[STRING_TYPE, Union[Tuple[STRING_TYPE, ...], STRING_TYPE, bool]]) -> F
+    def from_pipfile(cls, name, pipfile) -> Union["FileRequirement", "VCSRequirement"]:
         # Parse the values out. After this dance we should have two variables:
         # path - Local filesystem path.
         # uri - Absolute URI that is parsable with urlsplit.
         # One of these will be a string; the other would be None.
         uri = pipfile.get("uri")
         fil = pipfile.get("file")
         path = pipfile.get("path")
         if path and isinstance(path, str):
-            if isinstance(path, Path) and not path.is_absolute():
-                path = get_converted_relative_path(path.as_posix())
-            elif not os.path.isabs(path):
+            if not urllib_parse.urlparse(path).scheme and not os.path.isabs(path):
                 path = get_converted_relative_path(path)
         if path and uri:
             raise ValueError("do not specify both 'path' and 'uri'")
-        if path and fil:
-            raise ValueError("do not specify both 'path' and 'file'")
-        uri = uri or fil
+        uri = uri or fil or path
 
         # Decide that scheme to use.
-        # 'path' - local filesystem path.
         # 'file' - A file:// URI (possibly with VCS prefix).
+        # 'path' - local filesystem path.
         # 'uri' - Any other URI.
-        if path:
-            uri_scheme = "path"
-        else:
-            # URI is not currently a valid key in pipfile entries
-            # see https://github.com/pypa/pipfile/issues/110
+        if fil or (path and path.startswith("file:/")):
             uri_scheme = "file"
+        else:
+            uri_scheme = "path"
 
         if not uri:
             uri = path_to_url(path)
         link_info = None  # type: Optional[LinkInfo]
         if uri and isinstance(uri, str):
             link_info = cls.get_link_from_line(uri)
         else:
@@ -1791,29 +1738,28 @@
                 "Failed parsing requirement from pipfile: {0!r}".format(pipfile)
             )
         link = None  # type: Optional[Link]
         if link_info:
             link = link_info.link
             if link.url_without_fragment:
                 uri = link.url_without_fragment
-        extras = ()  # type: Optional[Tuple[STRING_TYPE, ...]]
+        extras = ()  # type: Optional[Tuple[str, ...]]
         if "extras" in pipfile:
             extras = tuple(pipfile["extras"])  # type: ignore
         editable = pipfile["editable"] if "editable" in pipfile else False
         arg_dict = {
             "name": name,
             "path": path,
             "uri": uri,
             "editable": editable,
             "link": link,
             "uri_scheme": uri_scheme,
             "extras": extras if extras else None,
         }
 
-        line = ""  # type: STRING_TYPE
         extras_string = "" if not extras else extras_to_string(extras)
         if editable and uri_scheme == "path":
             line = "{0}{1}".format(path, extras_string)
         else:
             if name:
                 line_name = "{0}{1}".format(name, extras_string)
                 line = "{0}#egg={1}".format(link.url_without_fragment, line_name)
@@ -1828,30 +1774,30 @@
                     )
                 line = "{0}{1}".format(line, extras_string)
             if "subdirectory" in pipfile:
                 arg_dict["subdirectory"] = pipfile["subdirectory"]
                 line = "{0}&subdirectory={1}".format(line, pipfile["subdirectory"])
         if editable:
             line = "-e {0}".format(line)
-        arg_dict["parsed_line"] = Line(line, extras=extras)
+        arg_dict["parsed_line"] = Line(line=line, extras=extras)
         arg_dict["setup_info"] = arg_dict["parsed_line"].setup_info
         return cls(**arg_dict)  # type: ignore
 
-    @property
+    @cached_property
     def line_part(self):
-        # type: () -> STRING_TYPE
-        link_url = None  # type: Optional[STRING_TYPE]
-        seed = None  # type: Optional[STRING_TYPE]
+        # type: () -> str
+        link_url = None  # type: Optional[str]
+        seed = None  # type: Optional[str]
         if self.link is not None:
             link_url = self.link.url_without_fragment
         is_vcs = getattr(self.link, "is_vcs", False)
-        if self._uri_scheme and self._uri_scheme == "path":
+        if self.uri_scheme and self.uri_scheme == "path":
             # We may need any one of these for passing to pip
             seed = self.path or link_url or self.uri
-        elif (self._uri_scheme and self._uri_scheme == "file") or (
+        elif (self.uri_scheme and self.uri_scheme == "file") or (
             (self.link.is_wheel or not is_vcs) and self.link.url
         ):
             seed = link_url or self.uri
         # add egg fragments to remote artifacts (valid urls only)
         if not self._has_hashed_name and self.is_remote_artifact and seed is not None:
             seed += "#egg={0}".format(self.name)
         editable = "-e " if self.editable else ""
@@ -1863,181 +1809,146 @@
     def pipfile_part(self):
         # type: () -> Dict[AnyStr, Dict[AnyStr, Any]]
         excludes = [
             "_base_line",
             "_has_hashed_name",
             "setup_path",
             "pyproject_path",
-            "_uri_scheme",
+            "uri_scheme",
             "pyproject_requires",
             "pyproject_backend",
-            "_setup_info",
-            "_parsed_line",
+            "setup_info",
+            "parsed_line",
         ]
-        filter_func = lambda k, v: bool(v) is True and k.name not in excludes  # noqa
-        pipfile_dict = attr.asdict(self, filter=filter_func).copy()  # type: Dict
+        pipfile_dict = self.dict()
+        for k in list(pipfile_dict.keys()):
+            if k in excludes:
+                pipfile_dict.pop(k)
+            elif not pipfile_dict.get(k):
+                pipfile_dict.pop(k)
+        if pipfile_dict.get("editable") is False:
+            pipfile_dict.pop("editable")
+        if pipfile_dict.get("line_part"):
+            pipfile_dict.pop("line_part")
         name = pipfile_dict.pop("name", None)
         if name is None:
             if self.name:
                 name = self.name
             elif self.parsed_line and self.parsed_line.name:
                 name = self.name = self.parsed_line.name
             elif self.setup_info and self.setup_info.name:
                 name = self.name = self.setup_info.name
-        if "_uri_scheme" in pipfile_dict:
-            pipfile_dict.pop("_uri_scheme")
+        if "uri_scheme" in pipfile_dict:
+            pipfile_dict.pop("uri_scheme")
         # For local paths and remote installable artifacts (zipfiles, etc)
         collision_keys = {"file", "uri", "path"}
-        collision_order = ["file", "uri", "path"]  # type: List[STRING_TYPE]
-        collisions = []  # type: List[STRING_TYPE]
+        collision_order = ["file", "uri", "path"]  # type: List[str]
         key_match = next(iter(k for k in collision_order if k in pipfile_dict.keys()))
         is_vcs = None
         if self.link is not None:
             is_vcs = getattr(self.link, "is_vcs", False)
-        if self._uri_scheme:
-            dict_key = self._uri_scheme
+        if self.uri_scheme:
+            dict_key = self.uri_scheme
             target_key = dict_key if dict_key in pipfile_dict else key_match
             if target_key is not None:
                 winning_value = pipfile_dict.pop(target_key)
                 collisions = [k for k in collision_keys if k in pipfile_dict]
                 for key in collisions:
                     pipfile_dict.pop(key)
                 pipfile_dict[dict_key] = winning_value
         elif (
             self.is_remote_artifact
             or (is_vcs is not None and not is_vcs)
-            and (self._uri_scheme and self._uri_scheme == "file")
+            and (self.uri_scheme and self.uri_scheme == "file")
         ):
             dict_key = "file"
             # Look for uri first because file is a uri format and this is designed
             # to make sure we add file keys to the pipfile as a replacement of uri
             if key_match is not None:
                 winning_value = pipfile_dict.pop(key_match)
+                pipfile_dict[dict_key] = winning_value
             key_to_remove = (k for k in collision_keys if k in pipfile_dict)
             for key in key_to_remove:
                 pipfile_dict.pop(key)
-            pipfile_dict[dict_key] = winning_value
         else:
             collisions = [key for key in collision_order if key in pipfile_dict.keys()]
             if len(collisions) > 1:
                 for k in collisions[1:]:
                     pipfile_dict.pop(k)
         return {name: pipfile_dict}
 
 
-@attr.s(slots=True, hash=True)
 class VCSRequirement(FileRequirement):
-    #: Whether the repository is editable
-    editable = attr.ib(default=None)  # type: Optional[bool]
-    #: URI for the repository
-    uri = attr.ib(default=None)  # type: Optional[STRING_TYPE]
-    #: path to the repository, if it's local
-    path = attr.ib(
-        default=None, validator=attr.validators.optional(validate_path)
-    )  # type: Optional[STRING_TYPE]
-    #: vcs type, i.e. git/hg/svn
-    vcs = attr.ib(
-        validator=attr.validators.optional(validate_vcs), default=None
-    )  # type: Optional[STRING_TYPE]
-    #: vcs reference name (branch / commit / tag)
-    ref = attr.ib(default=None)  # type: Optional[STRING_TYPE]
-    #: Subdirectory to use for installation if applicable
-    _repo = attr.ib(default=None)  # type: Optional[VCSRepository]
-    _base_line = attr.ib(default=None)  # type: Optional[STRING_TYPE]
-    name = attr.ib()  # type: STRING_TYPE
-    link = attr.ib()  # type: Optional[Link]
-    req = attr.ib()  # type: Optional[RequirementType]
-
-    def __attrs_post_init__(self):
-        # type: () -> None
-        if not self.uri:
-            if self.path:
-                self.uri = path_to_url(self.path)
+    editable: Optional[bool] = None
+    uri: Optional[str] = None
+    path: Optional[str] = Field(default=None, validator=validate_path)
+    vcs: Optional[str] = Field(default=None, validator=validate_vcs)
+    ref: Optional[str] = None
+    _repo: Optional[VCSRepository] = None
+    _base_line: Optional[str] = None
+    parsed_line: Optional[Line] = None
+    uri_scheme: Optional[str] = None
+    name: str
+    link: Optional[Link]
+    req: Optional[PackagingRequirement]
+
+    def __init__(self, **data):
+        super().__init__(**data)
+        if not self.uri and self.path:
+            self.uri = path_to_url(self.path)
         if self.uri is not None:
             split = urllib_parse.urlsplit(self.uri)
             scheme, rest = split[0], split[1:]
             vcs_type = ""
             if "+" in scheme:
                 vcs_type, scheme = scheme.split("+", 1)
                 vcs_type = "{0}+".format(vcs_type)
             new_uri = urllib_parse.urlunsplit((scheme,) + rest[:-1] + ("",))
             new_uri = "{0}{1}".format(vcs_type, new_uri)
             self.uri = new_uri
 
-    @property
-    def url(self):
-        # type: () -> STRING_TYPE
+    @cached_property
+    def url(self) -> str:
         if self.link and self.link.url:
             return self.link.url
         elif self.uri:
             return self.uri
         raise ValueError("No valid url found for requirement {0!r}".format(self))
 
-    @link.default
     def get_link(self) -> Link:
         uri = self.uri if self.uri else path_to_url(self.path)
         vcs_uri = build_vcs_uri(
             self.vcs,
             add_ssh_scheme_to_git_uri(uri),
             name=self.name,
             ref=self.ref,
             subdirectory=self.subdirectory,
             extras=self.extras,
         )
         return self.get_link_from_line(vcs_uri).link
 
-    @name.default
-    def get_name(self):
-        # type: () -> STRING_TYPE
+    def get_name(self) -> str:
         if self.link and self.link.egg_fragment:
             return self.link.egg_fragment
         if self.req and self.req.name:
             return self.req.name
         return super(VCSRequirement, self).get_name()
 
-    @property
+    @cached_property
     def vcs_uri(self):
-        # type: () -> Optional[STRING_TYPE]
+        # type: () -> Optional[str]
         uri = self.uri
         if uri and not any(uri.startswith("{0}+".format(vcs)) for vcs in VCS_LIST):
             if self.vcs:
                 uri = "{0}+{1}".format(self.vcs, uri)
         return uri
 
-    @property
-    def setup_info(self):
-        if self._parsed_line and self._parsed_line.setup_info:
-            if not self._parsed_line.setup_info.name:
-                with global_tempdir_manager():
-                    self._parsed_line._setup_info.get_info()
-            return self._parsed_line.setup_info
-        subdir = self.subdirectory or self.parsed_line.subdirectory
-        if self._repo:
-            with global_tempdir_manager():
-                self._setup_info = SetupInfo.from_ireq(
-                    Line(self._repo.checkout_directory).ireq, subdir=subdir
-                )
-                self._setup_info.get_info()
-            return self._setup_info
-        ireq = self.parsed_line.ireq
-
-        with global_tempdir_manager():
-            self._setup_info = SetupInfo.from_ireq(ireq, subdir=subdir)
-        return self._setup_info
-
-    @setup_info.setter
-    def setup_info(self, setup_info):
-        self._setup_info = setup_info
-        if self._parsed_line:
-            self._parsed_line.setup_info = setup_info
-
-    @req.default
     def get_requirement(self):
         # type: () -> PackagingRequirement
-        name = None  # type: Optional[STRING_TYPE]
+        name = None  # type: Optional[str]
         if self.name:
             name = self.name
         elif self.link and self.link.egg_fragment:
             name = self.link.egg_fragment
         url = None
         if self.uri:
             url = self.uri
@@ -2094,28 +2005,26 @@
                 and url.startswith("git+file:/")
                 and not url.startswith("git+file:///")
             ):
                 url = url.replace("git+file:/", "git+file:///")
             req.url = url
         return req
 
-    @property
-    def repo(self):
-        # type: () -> VCSRepository
+    @cached_property
+    def repo(self) -> VCSRepository:
         if self._repo is None:
-            if self._parsed_line and self._parsed_line.vcsrepo:
-                self._repo = self._parsed_line.vcsrepo
+            if self.parsed_line and self.parsed_line.vcsrepo:
+                self._repo = self.parsed_line.vcsrepo
             else:
                 self._repo = self.get_vcs_repo()
-                if self._parsed_line:
-                    self._parsed_line.vcsrepo = self._repo
+                if self.parsed_line:
+                    self.parsed_line.set_vcsrepo(self._repo)
         return self._repo
 
-    def get_checkout_dir(self, src_dir=None):
-        # type: (Optional[S]) -> STRING_TYPE
+    def get_checkout_dir(self, src_dir=None) -> str:
         src_dir = os.environ.get("PIP_SRC", None) if not src_dir else src_dir
         checkout_dir = None
         if self.is_local:
             path = self.path
             if not path:
                 path = url_to_path(self.uri)
             if path and os.path.exists(path):
@@ -2124,15 +2033,15 @@
         if src_dir is not None:
             checkout_dir = os.path.join(os.path.abspath(src_dir), self.name)
             os.makedirs(src_dir, exist_ok=True)
             return checkout_dir
         return os.path.join(create_tracked_tempdir(prefix="requirementslib"), self.name)
 
     def get_vcs_repo(self, src_dir=None, checkout_dir=None):
-        # type: (Optional[STRING_TYPE], STRING_TYPE) -> VCSRepository
+        # type: (Optional[str], str) -> VCSRepository
         from .vcs import VCSRepository
 
         if checkout_dir is None:
             checkout_dir = self.get_checkout_dir(src_dir=src_dir)
         vcsrepo = VCSRepository(
             url=expand_env_variables(self.url),
             name=self.name,
@@ -2156,80 +2065,70 @@
             pyproject_info = get_pyproject(checkout_dir)
         if pyproject_info is not None:
             pyproject_requires, pyproject_backend = pyproject_info
             self.pyproject_requires = tuple(pyproject_requires)
             self.pyproject_backend = pyproject_backend
         return vcsrepo
 
-    def get_commit_hash(self):
-        # type: () -> STRING_TYPE
-        with global_tempdir_manager():
-            hash_ = self.repo.get_commit_hash()
-        return hash_
+    @cached_property
+    def commit_hash(self) -> str:
+        return self.repo.commit_hash
 
-    def update_repo(self, src_dir=None, ref=None):
-        # type: (Optional[STRING_TYPE], Optional[STRING_TYPE]) -> STRING_TYPE
+    def update_repo(self, src_dir=None, ref=None) -> str:
         if ref:
             self.ref = ref
-        repo_hash = None
         if not self.is_local and self.ref is not None:
             self.repo.checkout_ref(self.ref)
-        repo_hash = self.get_commit_hash()
+        repo_hash = self.commit_hash
         if self.req:
             self.req.revision = repo_hash
         return repo_hash
 
     @contextmanager
-    def locked_vcs_repo(self, src_dir=None):
-        # type: (Optional[AnyStr]) -> Generator[VCSRepository, None, None]
+    def locked_vcs_repo(
+        self, src_dir: Optional[str] = None
+    ) -> Generator[VCSRepository, None, None]:
         if not src_dir:
             src_dir = create_tracked_tempdir(prefix="requirementslib-", suffix="-src")
         vcsrepo = self.get_vcs_repo(src_dir=src_dir)
         if not self.req:
             if self.parsed_line is not None:
                 self.req = self.parsed_line.requirement
             else:
                 self.req = self.get_requirement()
         with global_tempdir_manager():
-            revision = self.req.revision = vcsrepo.get_commit_hash()
+            revision = self.req.revision = vcsrepo.commit_hash
 
         # Remove potential ref in the end of uri after ref is parsed
         if self.link and "@" in self.link.show_url and self.uri and "@" in self.uri:
             uri, ref = split_ref_from_uri(self.uri)
             checkout = revision
             if checkout and ref and ref in checkout:
                 self.uri = uri
         orig_repo = self._repo
         self._repo = vcsrepo
-        if self._parsed_line:
-            self._parsed_line.vcsrepo = vcsrepo
-        if self._setup_info:
-            self._setup_info = attr.evolve(
-                self._setup_info,
-                requirements=(),
-                _extras_requirements=(),
-                build_requires=(),
-                setup_requires=(),
-                version=None,
-                metadata=None,
-            )
-        if self.parsed_line and self._parsed_line:
-            self._parsed_line.vcsrepo = vcsrepo
+        if self.parsed_line:
+            self.parsed_line.set_vcsrepo(vcsrepo)
+        if self.parsed_line and self.parsed_line:
+            self.parsed_line.set_vcsrepo(vcsrepo)
         if self.req and not self.editable:
+            if self.setup_info is None and self.parsed_line.setup_info:
+                self.setup_info = self.parsed_line.setup_info
+            if self.setup_info and not self.setup_info.version:
+                self.setup_info.build()
             self.req.specifier = SpecifierSet("=={0}".format(self.setup_info.version))
         try:
             yield self._repo
         except Exception:
             self._repo = orig_repo
             raise
 
     @classmethod
-    def from_pipfile(cls, name, pipfile):
-        # type: (STRING_TYPE, Dict[S, Union[Tuple[S, ...], S, bool]]) -> F
-        creation_args = {}  # type: Dict[STRING_TYPE, CREATION_ARG_TYPES]
+    def from_pipfile(cls, name, pipfile) -> Union["FileRequirement", "VCSRequirement"]:
+        creation_args = {}
         pipfile_keys = [
             k
             for k in (
                 "ref",
                 "vcs",
                 "subdirectory",
                 "path",
@@ -2237,15 +2136,14 @@
                 "file",
                 "uri",
                 "extras",
             )
             + VCS_LIST
             if k in pipfile
         ]
-        # extras = None  # type: Optional[Tuple[STRING_TYPE, ...]]
         for key in pipfile_keys:
             if key == "extras" and key in pipfile:
                 extras = pipfile[key]
                 if isinstance(extras, (list, tuple)):
                     pipfile[key] = tuple(sorted({extra.lower() for extra in extras}))
                 else:
                     pipfile[key] = extras
@@ -2271,37 +2169,36 @@
             elif key in pipfile_keys:
                 creation_args[key] = pipfile[key]
         creation_args["name"] = name
         cls_inst = cls(**creation_args)  # type: ignore
         return cls_inst
 
     @classmethod
-    def from_line(cls, line, editable=None, extras=None, parsed_line=None):
-        # type: (AnyStr, Optional[bool], Optional[Tuple[AnyStr, ...]], Optional[Line]) -> F
-        parsed_line = Line(line)
+    def from_line(
+        cls, line, editable=None, extras=None, parsed_line=None
+    ) -> Union["FileRequirement", "VCSRequirement"]:
+        parsed_line = Line(line=line)
         return vcs_req_from_parsed_line(parsed_line)
 
     @property
-    def line_part(self):
-        # type: () -> STRING_TYPE
+    def line_part(self) -> str:
         """requirements.txt compatible line part sans-extras."""
-        base = ""  # type: STRING_TYPE
         if self.is_local:
             base_link = self.link
             if not self.link:
                 base_link = self.get_link()
             if base_link and base_link.egg_fragment:
                 final_format = "{{0}}#egg={0}".format(base_link.egg_fragment)
             else:
                 final_format = "{0}"
             base = final_format.format(self.vcs_uri)
-        elif self._parsed_line is not None and (
-            self._parsed_line.is_direct_url and self._parsed_line.line_with_prefix
+        elif self.parsed_line is not None and (
+            self.parsed_line.is_direct_url and self.parsed_line.line_with_prefix
         ):
-            return self._parsed_line.line_with_prefix
+            return self.parsed_line.line_with_prefix
         elif getattr(self, "_base_line", None) and (isinstance(self._base_line, str)):
             base = self._base_line
         else:
             base = getattr(self, "link", self.get_link()).url
         if base and self.extras and extras_to_string(self.extras) not in base:
             if self.subdirectory:
                 base = "{0}".format(self.get_link().url)
@@ -2312,377 +2209,291 @@
         if self.editable and not base.startswith("-e "):
             base = "-e {0}".format(base)
         return base
 
     @staticmethod
     def _choose_vcs_source(pipfile):
         # type: (Dict[S, Union[S, Any]]) -> Dict[S, Union[S, Any]]
-        src_keys = [k for k in pipfile.keys() if k in ["path", "uri", "file"]]
-        vcs_type = ""  # type: Optional[STRING_TYPE]
-        alt_type = ""  # type: Optional[STRING_TYPE]
-        vcs_value = ""  # type: STRING_TYPE
+        src_keys = []
+        for key in ["path", "uri", "file"]:
+            if pipfile.get(key):
+                src_keys.append(key)
+        vcs_type = ""  # type: Optional[str]
+        alt_type = ""  # type: Optional[str]
+        vcs_value = ""  # type: str
         if src_keys:
             chosen_key = next(iter(src_keys))
             vcs_type = pipfile.pop("vcs")
             if chosen_key in pipfile:
                 vcs_value = pipfile[chosen_key]
                 alt_type, pipfile_url = split_vcs_method_from_uri(vcs_value)
                 if vcs_type is None:
                     vcs_type = alt_type
             if vcs_type and pipfile_url:
                 pipfile[vcs_type] = pipfile_url
-            for removed in src_keys:
-                pipfile.pop(removed)
         return pipfile
 
     @property
     def pipfile_part(self):
-        # type: () -> Dict[S, Dict[S, Union[List[S], S, bool, RequirementType, Link]]]
+        # type: () -> Dict[S, Dict[S, Union[List[S], S, bool, PackagingRequirement, Link]]]
         excludes = [
             "_repo",
             "_base_line",
             "setup_path",
             "_has_hashed_name",
             "pyproject_path",
             "pyproject_requires",
             "pyproject_backend",
             "_setup_info",
-            "_parsed_line",
-            "_uri_scheme",
+            "parsed_line",
+            "uri_scheme",
         ]
         filter_func = lambda k, v: bool(v) is True and k.name not in excludes  # noqa
-        pipfile_dict = attr.asdict(self, filter=filter_func).copy()
-        name = pipfile_dict.pop("name", None)
+        pipfile_dict = self.dict()
+        for k in list(pipfile_dict.keys()):
+            if k in excludes:
+                pipfile_dict.pop(k)
+            elif not pipfile_dict.get(k):
+                pipfile_dict.pop(k)
+        if pipfile_dict.get("editable") is False:
+            pipfile_dict.pop("editable")
+        if pipfile_dict.get("line_part"):
+            pipfile_dict.pop("line_part")
+        name = pipfile_dict.get("name")
         if name is None:
             if self.name:
                 name = self.name
             elif self.parsed_line and self.parsed_line.name:
                 name = self.name = self.parsed_line.name
             elif self.setup_info and self.setup_info.name:
                 name = self.name = self.setup_info.name
         if "vcs" in pipfile_dict:
             pipfile_dict = self._choose_vcs_source(pipfile_dict)
         name, _ = _strip_extras(name)
         return {name: pipfile_dict}  # type: ignore
 
 
-@attr.s(eq=True, order=True, hash=True)
-class Requirement(object):
-    _name = attr.ib(eq=True, order=True)  # type: STRING_TYPE
-    vcs = attr.ib(
-        default=None,
-        validator=attr.validators.optional(validate_vcs),
-        eq=True,
-        order=True,
-    )  # type: Optional[STRING_TYPE]
-    req = attr.ib(
-        default=None, eq=True, order=True
-    )  # type: Optional[Union[VCSRequirement, FileRequirement, NamedRequirement]]
-    markers = attr.ib(default=None, eq=True, order=True)  # type: Optional[STRING_TYPE]
-    _specifiers = attr.ib(
-        validator=attr.validators.optional(validate_specifiers), eq=True, order=True
-    )  # type: Optional[STRING_TYPE]
-    index = attr.ib(default=None, eq=True, order=True)  # type: Optional[STRING_TYPE]
-    editable = attr.ib(default=None, eq=True, order=True)  # type: Optional[bool]
-    hashes = attr.ib(
-        factory=frozenset, converter=frozenset, eq=True, order=True
-    )  # type: FrozenSet[STRING_TYPE]
-    extras = attr.ib(factory=tuple, eq=True, order=True)  # type: Tuple[STRING_TYPE, ...]
-    abstract_dep = attr.ib(
-        default=None, eq=False, order=False
-    )  # type: Optional[AbstractDependency]
-    _line_instance = attr.ib(default=None, eq=False, order=False)  # type: Optional[Line]
-    _ireq = attr.ib(
-        default=None, eq=False, order=False
-    )  # type: Optional[InstallRequirement]
+class Requirement(ReqLibBaseModel):
+    vcs: Optional[str] = Field(None, eq=True, order=True)
+    req: Optional[Any] = Field(None, eq=True, order=True)
+    markers: Optional[str] = Field("", eq=True, order=True)
+    index: Optional[str] = Field(None, eq=True, order=True)
+    editable: Optional[bool] = Field(None, eq=True, order=True)
+    hashes: Set[str] = set()
+    extras: Tuple[str, ...] = Field(tuple(), eq=True, order=True)
+    _line_instance: Optional[Line] = None
+    # ireq: Optional[InstallRequirement] = Field(None, eq=False, order=False)
+    # _ireq: Optional[Any] = Field(None, eq=False, order=False)
+
+    class Config:
+        validate_assignment = True
+        arbitrary_types_allowed = True
+        allow_mutation = True
+        include_private_attributes = True
+        keep_untouched = (cached_property,)
 
     def __hash__(self):
         return hash(self.as_line())
 
-    @_name.default
-    def get_name(self):
-        # type: () -> Optional[STRING_TYPE]
-        if self.req is not None:
-            return self.req.name
-        return None
-
-    @property
-    def name(self):
-        # type: () -> Optional[STRING_TYPE]
-        if self._name is not None:
-            return self._name
+    @cached_property
+    def name(self) -> Optional[str]:
         name = None
         if self.req and self.req.name:
             name = self.req.name
         elif self.req and self.is_file_or_url and self.req.setup_info:
             name = self.req.setup_info.name
-        self._name = name
         return name
 
-    @property
-    def requirement(self):
-        # type: () -> Optional[PackagingRequirement]
+    @cached_property
+    def requirement(self) -> Optional[PackagingRequirement]:
         if self.req:
             return self.req.req
         return None
 
-    def add_hashes(self, hashes):
-        # type: (Union[S, List[S], Set[S], Tuple[S, ...]]) -> Requirement
-        new_hashes = set()  # type: Set[STRING_TYPE]
+    def add_hashes(self, hashes: set) -> "Requirement":
+        new_hashes = set()
         if self.hashes is not None:
             new_hashes |= set(self.hashes)
         if isinstance(hashes, str):
             new_hashes.add(hashes)
         else:
             new_hashes |= set(hashes)
-        return attr.evolve(self, hashes=tuple(new_hashes))
+        self.hashes = new_hashes
 
-    def get_hashes_as_pip(self, as_list=False):
-        # type: (bool) -> Union[STRING_TYPE, List[STRING_TYPE]]
-        hashes = ""  # type: Union[STRING_TYPE, List[STRING_TYPE]]
+    def get_hashes_as_pip(self, as_list: bool = False) -> Union[str, List[str]]:
         if as_list:
-            hashes = []
-            if self.hashes:
-                hashes = [HASH_STRING.format(h) for h in self.hashes]
+            return [HASH_STRING.format(h) for h in self.hashes] if self.hashes else []
         else:
-            hashes = ""
-            if self.hashes:
-                hashes = "".join([HASH_STRING.format(h) for h in self.hashes])
-        return hashes
-
-    @property
-    def hashes_as_pip(self):
-        # type: () -> STRING_TYPE
-        hashes = self.get_hashes_as_pip()
-        assert isinstance(hashes, str)
-        return hashes
-
-    @property
-    def markers_as_pip(self):
-        # type: () -> S
-        if self.markers:
-            return " ; {0}".format(self.markers).replace('"', "'")
-
-        return ""
-
-    @property
-    def extras_as_pip(self):
-        # type: () -> STRING_TYPE
-        if self.extras:
-            return "[{0}]".format(
-                ",".join(sorted([extra.lower() for extra in self.extras]))  # type: ignore
+            return (
+                "".join([HASH_STRING.format(h) for h in self.hashes])
+                if self.hashes
+                else ""
             )
 
-        return ""
+    @cached_property
+    def hashes_as_pip(self) -> str:
+        return self.get_hashes_as_pip()
 
     @cached_property
-    def commit_hash(self):
-        # type: () -> Optional[S]
+    def extras_as_pip(self) -> str:
+        return (
+            f"[{','.join(sorted([extra.lower() for extra in self.extras]))}]"
+            if self.extras
+            else ""
+        )
+
+    @cached_property
+    def commit_hash(self) -> Optional[str]:
         if self.req is None or not isinstance(self.req, VCSRequirement):
             return None
         commit_hash = None
         if self.req is not None:
             with self.req.locked_vcs_repo() as repo:
-                commit_hash = repo.get_commit_hash()
+                commit_hash = repo.commit_hash
         return commit_hash
 
-    @_specifiers.default
-    def get_specifiers(self):
-        # type: () -> S
+    @cached_property
+    def get_specifiers(self) -> str:
         if self.req and self.req.req and self.req.req.specifier:
             return specs_to_string(self.req.req.specifier)
         return ""
 
-    def update_name_from_path(self, path):
+    def update_name_from_path(self, path: str) -> None:
         metadata = get_metadata(path)
         name = self.name
         if metadata is not None:
             metadata_name = metadata.get("name")
             if metadata_name and metadata_name != "wheel":
                 name = metadata_name
         if name is not None:
             if self.req.name is None:
                 self.req.name = name
             if self.req.req and self.req.req.name is None:
                 self.req.req.name = name
-            if self._line_instance._name is None:
-                self._line_instance.name = name
-            if self.req._parsed_line._name is None:
-                self.req._parsed_line.name = name
-            if self.req._setup_info and self.req._setup_info.name is None:
-                self.req._setup_info.name = name
-
-    def get_line_instance(self):
-        # type: () -> Line
-        line_parts = []
-        local_editable = False
-        if self.req:
-            if self.req.line_part.startswith("-e "):
-                local_editable = True
-                line_parts.extend(self.req.line_part.split(" ", 1))
-            else:
-                line_parts.append(self.req.line_part)
-        if not self.is_vcs and not self.vcs and self.extras_as_pip:
+            if self.req.parsed_line._name is None:
+                self.req.parsed_line.name = name
+            if self.req.setup_info and self.req.setup_info.name is None:
+                self.req.setup_info.name = name
+
+    def get_line_instance(self) -> Line:
+        if self._line_instance is None:
+            line_parts = []
+            local_editable = False
+            if self.req:
+                if self.req.line_part.startswith("-e "):
+                    local_editable = True
+                    line_parts.extend(self.req.line_part.split(" ", 1))
+                else:
+                    line_parts.append(self.req.line_part)
+
+            version, fetched = self.get_version_from_setup_info()
+            if version is not None and not (self.is_file_or_url or self.is_vcs):
+                line_parts.append(f"=={version}")
             if (
                 self.is_file_or_url
                 and not local_editable
                 and not self.req.get_uri().startswith("file://")
                 # fix for file uri with egg names and extras
                 and not len(self.req.line_part.split("#")) > 1
             ):
-                line_parts.append(f"#egg={self._name}{self.extras_as_pip}")
-            else:
+                line_parts.append(f"#egg={self.name}{self.extras_as_pip}")
+            elif not any(part for part in line_parts if self.extras_as_pip in part):
                 line_parts.append(self.extras_as_pip)
-        if self._specifiers and not (self.is_file_or_url or self.is_vcs):
-            line_parts.append(self._specifiers)
-        if self.markers:
-            line_parts.append(" ; {0}".format(self.markers.replace('"', "'")))
-        if self.hashes_as_pip and not (self.editable or self.vcs or self.is_vcs):
-            line_parts.append(self.hashes_as_pip)
-        if self.editable:
-            if line_parts[0] == "-e":
-                line = "".join(line_parts[1:])
+            if self.specifiers and not (self.is_file_or_url or self.is_vcs):
+                line_parts.append(self.specifiers)
+            if self.markers and not self.is_file_or_url:
+                line_parts.append(" ; {0}".format(self.markers.replace('"', "'")))
+
+            if self.hashes_as_pip and not (self.editable or self.vcs or self.is_vcs):
+                line_parts.append(self.hashes_as_pip)
+
+            if self.editable:
+                if line_parts[0] == "-e":
+                    line = "".join(line_parts[1:])
+                else:
+                    line = "".join(line_parts)
+                if self.markers:
+                    line = '"{0}"'.format(line)
+                line = "-e {0}".format(line)
             else:
                 line = "".join(line_parts)
-            if self.markers:
-                line = '"{0}"'.format(line)
-            line = "-e {0}".format(line)
-        else:
-            line = "".join(line_parts)
-        return Line(line)
+            self._line_instance = Line(line=line)
+        return self._line_instance
 
     @property
     def line_instance(self):
-        # type: () -> Optional[Line]
-        if self._line_instance is None:
-            self.line_instance = self.get_line_instance()
-        return self._line_instance
-
-    @line_instance.setter
-    def line_instance(self, line_instance):
-        # type: (Line) -> None
-        if self.req:
-            self.req._parsed_line = line_instance
-        self._line_instance = line_instance
+        return self.get_line_instance()
 
-    @property
-    def specifiers(self):
-        # type: () -> Optional[STRING_TYPE]
-        if self._specifiers:
-            return self._specifiers
-        else:
-            specs = self.get_specifiers()
-            if specs:
-                self._specifiers = specs
-                return specs
-        if not self._specifiers and (
-            self.req is not None
-            and isinstance(self.req, NamedRequirement)
-            and self.req.version
-        ):
-            self._specifiers = self.req.version
+    @cached_property
+    def specifiers(self) -> Optional[str]:
+        specs = self.get_specifiers
+        if specs:
+            return specs
+        elif self.req and isinstance(self.req, NamedRequirement) and self.req.version:
+            return "=={0}".format(self.req.version)
         elif (
-            not self.editable
-            and self.req
-            and (not isinstance(self.req, NamedRequirement) and self.req.setup_info)
-        ):
-            if (
-                self.line_instance
-                and self.line_instance.setup_info
-                and self.line_instance.setup_info.version
-            ):
-                self._specifiers = "=={0}".format(self.req.setup_info.version)
-        elif not self._specifiers:
-            if self.req and self.req.parsed_line and self.req.parsed_line.specifiers:
-                self._specifiers = specs_to_string(self.req.parsed_line.specifiers)
-            elif self.line_instance and self.line_instance.specifiers:
-                self._specifiers = specs_to_string(self.line_instance.specifiers)
-            elif self.is_file_or_url or self.is_vcs:
+            self.req
+            and hasattr(self.req, "setup_info")
+            and self.req.setup_info
+            and self.req.setup_info.version
+        ):
+            return "=={0}".format(self.req.setup_info.version)
+        # TODO This creates circular call chain that eventuallys gets cached by cached_property
+        elif self.is_file_or_url or self.is_vcs:
+            version, fetched = self.get_version_from_setup_info()
+            if version is not None:
+                return "=={0}".format(version)
+            elif not fetched:
                 try:
                     setupinfo_dict = self.run_requires()
                 except Exception:
                     setupinfo_dict = None
                 if setupinfo_dict is not None:
-                    self._specifiers = "=={0}".format(setupinfo_dict.get("version"))
-        if self._specifiers:
-            specset = SpecifierSet(self._specifiers)
-            if self.line_instance and not self.line_instance.specifiers:
-                self.line_instance.specifiers = specset
-            if self.req:
-                if self.req._parsed_line and not self.req._parsed_line.specifiers:
-                    self.req._parsed_line.specifiers = specset
-                elif not self.req._parsed_line and self.line_instance:
-                    self.req._parsed_line = self.line_instance
-            if self.req and self.req.req and not self.req.req.specifier:
-                self.req.req.specifier = specset
-        return self._specifiers
+                    return "=={0}".format(setupinfo_dict.get("version"))
+        elif self.req and hasattr(self.req, "setup_info") and self.req.setup_info.version:
+            return "=={0}".format(self.req.setup_info.version)
 
-    @property
-    def is_vcs(self):
-        # type: () -> bool
+    @cached_property
+    def is_vcs(self) -> bool:
         return isinstance(self.req, VCSRequirement)
 
-    @property
-    def build_backend(self):
-        # type: () -> Optional[STRING_TYPE]
-        if self.req is not None and (
-            not isinstance(self.req, NamedRequirement) and self.req.is_local
-        ):
-            with global_tempdir_manager():
-                setup_info = self.run_requires()
-            build_backend = setup_info.get("build_backend")
-            return build_backend
-        return "setuptools.build_meta"
-
-    @property
-    def uses_pep517(self):
-        # type: () -> bool
-        if self.build_backend:
-            return True
-        return False
-
-    @property
-    def is_file_or_url(self):
-        # type: () -> bool
+    @cached_property
+    def is_file_or_url(self) -> bool:
         return isinstance(self.req, FileRequirement)
 
-    @property
-    def is_named(self):
-        # type: () -> bool
+    @cached_property
+    def is_named(self) -> bool:
         return isinstance(self.req, NamedRequirement)
 
-    @property
-    def is_wheel(self):
-        # type: () -> bool
+    @cached_property
+    def is_wheel(self) -> bool:
         if (
             self.req
             and not isinstance(self.req, NamedRequirement)
             and (self.req.link is not None and self.req.link.is_wheel)
         ):
             return True
         return False
 
-    @property
-    def normalized_name(self):
-        # type: () -> S
+    @cached_property
+    def normalized_name(self) -> str:
         return canonicalize_name(self.name)
 
-    def copy(self):
-        return attr.evolve(self)
+    def _copy(self):
+        return self.__class__(**self.__dict__)
 
     @classmethod
-    @lru_cache()
-    def from_line(cls, line):
-        # type: (AnyStr) -> Requirement
+    def from_line(cls, line, parse_setup_info=True) -> "Requirement":
+        if isinstance(line, Requirement):
+            return line
         if isinstance(line, InstallRequirement):
             line = format_requirement(line)
-        parsed_line = Line(line)
-        r = (
-            None
-        )  # type: Optional[Union[VCSRequirement, FileRequirement, NamedRequirement]]
+        parsed_line = Line(line=line)
+        if parse_setup_info and not parsed_line.is_named and not parsed_line.is_wheel:
+            parsed_line.set_setup_info(parsed_line.get_setup_info())
         if (
             (parsed_line.is_file and parsed_line.is_installable)
             or parsed_line.is_remote_url
         ) and not parsed_line.is_vcs:
             r = file_req_from_parsed_line(parsed_line)
         elif parsed_line.is_vcs:
             r = vcs_req_from_parsed_line(parsed_line)
@@ -2695,25 +2506,22 @@
         req_markers = None
         if parsed_line.markers:
             req_markers = PackagingRequirement(
                 "fakepkg ; {0}".format(parsed_line.markers)
             )
         if r is not None and r.req is not None:
             r.req.marker = getattr(req_markers, "marker", None) if req_markers else None
-        args = {}  # type: Dict[STRING_TYPE, CREATION_ARG_TYPES]
         args = {
             "name": r.name,
             "vcs": parsed_line.vcs,
             "req": r,
             "markers": parsed_line.markers,
             "editable": parsed_line.editable,
-            "line_instance": parsed_line,
         }
         if parsed_line.extras:
-            extras = ()  # type: Tuple[STRING_TYPE, ...]
             extras = tuple(sorted(dedup([extra.lower() for extra in parsed_line.extras])))
             args["extras"] = extras
             if r is not None:
                 r.extras = extras
             elif r is not None and r.extras is not None:
                 args["extras"] = tuple(
                     sorted(dedup([extra.lower() for extra in r.extras]))
@@ -2756,16 +2564,15 @@
         if markers:
             markers = str(markers)
             req_markers = PackagingRequirement("fakepkg ; {0}".format(markers))
             if r.req is not None:
                 r.req.marker = req_markers.marker
         extras = _pipfile.get("extras")
         if r.req:
-            if r.req.specifier:
-                r.req.specifier = SpecifierSet(_pipfile["version"])
+            r.req.specifier = SpecifierSet(_pipfile["version"])
             r.req.extras = (
                 tuple(sorted(dedup([extra.lower() for extra in extras])))
                 if extras
                 else ()
             )
         args = {
             "name": r.name,
@@ -2814,262 +2621,212 @@
             if as_list:
                 parts.extend(sources)
             else:
                 index_string = " ".join(source_list)
                 parts = "{0} {1}".format(parts, index_string)
         return parts
 
+    @cached_property
     def get_markers(self):
-        # type: () -> Marker
         markers = self.markers
         if markers:
             fake_pkg = PackagingRequirement("fakepkg ; {0}".format(markers))
             markers = fake_pkg.marker
         return markers
 
-    def get_specifier(self):
-        # type: () -> Union[SpecifierSet, LegacySpecifier]
+    @cached_property
+    def get_specifier(self) -> Union[Specifier, LegacySpecifier]:
         try:
             return Specifier(self.specifiers)
         except InvalidSpecifier:
             return LegacySpecifier(self.specifiers)
 
+    @cached_property
     def get_version(self):
-        return parse(self.get_specifier().version)
+        return parse(self.get_specifier.version)
 
-    def get_requirement(self):
+    def get_requirement(self) -> PackagingRequirement:
         req_line = self.req.req.line
         if req_line.startswith("-e "):
             _, req_line = req_line.split(" ", 1)
         req = init_requirement(self.name)
         req.line = req_line
         req.specifier = SpecifierSet(self.specifiers if self.specifiers else "")
         if self.is_vcs or self.is_file_or_url:
             req.url = getattr(self.req.req, "url", self.req.link.url_without_fragment)
-        req.marker = self.get_markers()
+        req.marker = self.get_markers
         req.extras = set(self.extras) if self.extras else set()
         return req
 
-    @property
-    def constraint_line(self):
+    @cached_property
+    def constraint_line(self) -> str:
         return self.as_line()
 
-    @property
-    def is_direct_url(self):
+    @cached_property
+    def is_direct_url(self) -> bool:
         return (
             self.is_file_or_url
             and self.req.is_direct_url
             or (self.line_instance.is_direct_url or self.req.parsed_line.is_direct_url)
         )
 
-    def as_pipfile(self):
+    def as_pipfile(self) -> Dict[str, Any]:
+
         good_keys = (
             "hashes",
             "extras",
             "markers",
             "editable",
             "version",
             "index",
         ) + VCS_LIST
-        req_dict = {
-            k: v
-            for k, v in attr.asdict(self, recurse=False, filter=filter_none).items()
-            if k in good_keys
-        }
+        req_dict = {}
+        for k, v in self.dict().items():
+            if k in good_keys and v:
+                req_dict[k] = v
+        if req_dict.get("editable") is False:
+            req_dict.pop("editable")
+
         name = self.name
         if "markers" in req_dict and req_dict["markers"]:
             req_dict["markers"] = req_dict["markers"].replace('"', "'")
         if not self.req.name:
             name_carriers = (self.req, self, self.line_instance, self.req.parsed_line)
             name_options = [
                 getattr(carrier, "name", None)
                 for carrier in name_carriers
                 if carrier is not None
             ]
             req_name = next(iter(n for n in name_options if n is not None), None)
             self.req.name = req_name
-        req_name, dict_from_subreq = self.req.pipfile_part.popitem()
+        req_name = next(reversed(list(self.req.pipfile_part.keys())))
+        dict_from_subreq = self.req.pipfile_part[req_name]
         base_dict = {
             k: v
             for k, v in dict_from_subreq.items()
             if k not in ["req", "link", "_setup_info"]
         }
         base_dict.update(req_dict)
-        conflicting_keys = ("file", "path", "uri")
-        if "file" in base_dict and any(k in base_dict for k in conflicting_keys[1:]):
-            conflicts = [k for k in (conflicting_keys[1:],) if k in base_dict]
+        file_conflicting_keys = ("path", "uri", "name")
+        if "file" in base_dict and any(k in base_dict for k in file_conflicting_keys):
+            conflicts = [k for k in file_conflicting_keys if k in base_dict]
+            for k in conflicts:
+                base_dict.pop(k)
+        vcs_conflicting_keys = ("path", "uri", "name")
+        if any(k in base_dict for k in VCS_LIST):
+            conflicts = [k for k in vcs_conflicting_keys if k in base_dict]
             for k in conflicts:
                 base_dict.pop(k)
         if "hashes" in base_dict:
             _hashes = base_dict.pop("hashes")
             hashes = []
             for _hash in _hashes:
                 try:
                     hashes.append(_hash.as_line())
                 except AttributeError:
                     hashes.append(_hash)
             base_dict["hashes"] = sorted(hashes)
         if "extras" in base_dict:
             base_dict["extras"] = list(base_dict["extras"])
+        if "setup_info" in base_dict:
+            del base_dict["setup_info"]
         if len(base_dict.keys()) == 1 and "version" in base_dict:
             base_dict = base_dict.get("version")
+
         return {name: base_dict}
 
-    def as_ireq(self):
+    def as_ireq(self) -> InstallRequirement:
         if self.line_instance and self.line_instance.ireq:
             return self.line_instance.ireq
-        elif getattr(self.req, "_parsed_line", None) and self.req._parsed_line.ireq:
-            return self.req._parsed_line.ireq
+        elif getattr(self.req, "parsed_line", None) and self.req.parsed_line.ireq:
+            return self.req.parsed_line.ireq
         kwargs = {"include_hashes": False}
         if (self.is_file_or_url and self.req.is_local) or self.is_vcs:
             kwargs["include_markers"] = False
         ireq_line = self.as_line(**kwargs)
-        ireq = Line(ireq_line).ireq
+        ireq = Line(line=ireq_line).ireq
         if not getattr(ireq, "req", None):
             ireq.req = self.req.req
             if (self.is_file_or_url and self.req.is_local) or self.is_vcs:
                 if getattr(ireq, "req", None) and getattr(ireq.req, "marker", None):
                     ireq.req.marker = None
         else:
             ireq.req.extras = self.req.req.extras
             if not ((self.is_file_or_url and self.req.is_local) or self.is_vcs):
                 ireq.req.marker = self.req.req.marker
         return ireq
 
-    @property
-    def pipfile_entry(self):
-        return self.as_pipfile().copy().popitem()
+    @cached_property
+    def pipfile_entry(self) -> Tuple[str, Any]:
+        pipfile = self.as_pipfile()
+        last_key = next(reversed(list(pipfile.keys())))
+        last_value = pipfile[last_key]
+        return last_key, last_value
 
-    @property
-    def ireq(self):
+    @cached_property
+    def ireq(self) -> InstallRequirement:
         return self.as_ireq()
 
-    def dependencies(self, sources=None):
-        """Retrieve the dependencies of the current requirement.
-
-        Retrieves dependencies of the current requirement.  This only works on pinned
-        requirements.
-
-        :param sources: Pipfile-formatted sources, defaults to None
-        :param sources: list[dict], optional
-        :return: A set of requirement strings of the dependencies of this requirement.
-        :rtype: set(str)
-        """
-        if not sources:
-            sources = [
-                {"name": "pypi", "url": "https://pypi.org/simple", "verify_ssl": True}
-            ]
-        return get_dependencies(self.as_ireq(), sources=sources)
-
-    def abstract_dependencies(self, sources=None):
-        """Retrieve the abstract dependencies of this requirement.
-
-        Returns the abstract dependencies of the current requirement in order to resolve.
-
-        :param sources: A list of sources (pipfile format), defaults to None
-        :param sources: list, optional
-        :return: A list of abstract (unpinned) dependencies
-        :rtype: list[ :class:`~requirementslib.models.dependency.AbstractDependency` ]
-        """
-
-        if not self.abstract_dep:
-            parent = getattr(self, "parent", None)
-            self.abstract_dep = AbstractDependency.from_requirement(self, parent=parent)
-        if not sources:
-            sources = [
-                {"url": "https://pypi.org/simple", "name": "pypi", "verify_ssl": True}
-            ]
-        if is_pinned_requirement(self.ireq):
-            deps = self.dependencies()
-        else:
-            ireq = sorted(self.find_all_matches(), key=lambda k: k.version)
-            deps = get_dependencies(ireq.pop())
-        return get_abstract_dependencies(deps, parent=self.abstract_dep)
-
-    def find_all_matches(self, sources=None, finder=None):
-        # type: (Optional[List[Dict[S, Union[S, bool]]]], Optional[PackageFinder]) -> List[InstallationCandidate]
-        """Find all matching candidates for the current requirement.
-
-        Consults a finder to find all matching candidates.
-
-        :param sources: Pipfile-formatted sources, defaults to None
-        :param sources: list[dict], optional
-        :param PackageFinder finder: A **PackageFinder** instance from pip's repository implementation
-        :return: A list of Installation Candidates
-        :rtype: list[ :class:`~pip._internal.index.InstallationCandidate` ]
-        """
-
-        from .dependencies import find_all_matches, get_finder
-
-        if not finder:
-            _, finder = get_finder(sources=sources)
-        return find_all_matches(finder, self.as_ireq())
-
-    def run_requires(self, sources=None, finder=None):
-        if self.req and self.req.setup_info is not None:
-            info_dict = self.req.setup_info.as_dict()
-        elif self.line_instance and self.line_instance.setup_info is not None:
+    def get_version_from_setup_info(self) -> Tuple[Optional[str], bool]:
+        if self.req and isinstance(self.req, FileRequirement):
+            self.req.parse_setup_info()
+        if self.req and hasattr(self.req, "setup_info") and self.req.setup_info:
+            return self.req.setup_info.version, True
+        elif self._line_instance and self._line_instance.setup_info:
+            return self._line_instance.setup_info.version, True
+
+        return None, False
+
+    def run_requires(
+        self, sources: Optional[List[str]] = None, finder: Optional[PackageFinder] = None
+    ) -> Dict[str, Any]:
+        if self.line_instance and self._line_instance.setup_info:
             info_dict = self.line_instance.setup_info.as_dict()
         else:
-
             if not finder:
                 from .dependencies import get_finder
 
                 finder = get_finder(sources=sources)
             with global_tempdir_manager():
-                info = SetupInfo.from_requirement(self, finder=finder)
-                if info is None:
+                setup_info = SetupInfo.from_requirement(self, finder=finder)
+                if setup_info is None:
                     return {}
-                info_dict = info.get_info()
-            if self.req and not self.req.setup_info:
-                self.req._setup_info = info
-        if self.req._has_hashed_name and info_dict.get("name"):
-            self.req.name = self.name = info_dict["name"]
-            if self.req.req.name != info_dict["name"]:
-                self.req.req.name = info_dict["name"]
+                info_dict = setup_info.as_dict()
+                if self.req:
+                    self.req.setup_info = setup_info
+                if self.req._has_hashed_name and info_dict.get("name"):
+                    self.req.name = self.name = info_dict["name"]
+                    if self.req.req.name != info_dict["name"]:
+                        self.req.req.name = info_dict["name"]
         return info_dict
 
-    def merge_markers(self, markers):
-        # type: (Union[AnyStr, Marker]) -> None
+    def merge_markers(self, markers: Union[str, Marker]) -> "Requirement":
         if not markers:
             return self
         if not isinstance(markers, Marker):
             markers = Marker(markers)
         _markers = []  # type: List[Marker]
-        ireq = self.as_ireq()
+        ireq = self.ireq
         if ireq and ireq.markers:
             ireq_marker = ireq.markers
             _markers.append(str(ireq_marker))
         _markers.append(str(markers))
         marker_str = " and ".join([normalize_marker_str(m) for m in _markers if m])
+        self.markers = marker_str
         new_marker = Marker(marker_str)
-        line = copy.deepcopy(self._line_instance)
-        line.markers = marker_str
-        line.parsed_marker = new_marker
-        if getattr(line, "_requirement", None) is not None:
-            line._requirement.marker = new_marker
-        if getattr(line, "_ireq", None) is not None and line._ireq.req:
-            line._ireq.req.marker = new_marker
         new_ireq = getattr(self, "ireq", None)
         if new_ireq and new_ireq.req:
             new_ireq.req.marker = new_marker
-        req = self.req
-        if req.req:
-            req_requirement = req.req
-            req_requirement.marker = new_marker
-            req = attr.evolve(req, req=req_requirement, parsed_line=line)
-        return attr.evolve(
-            self, markers=str(new_marker), ireq=new_ireq, req=req, line_instance=line
-        )
+        if self.req.req:
+            self.req.req = new_marker
 
 
-def file_req_from_parsed_line(parsed_line):
-    # type: (Line) -> FileRequirement
+def file_req_from_parsed_line(parsed_line) -> FileRequirement:
     path = parsed_line.relpath if parsed_line.relpath else parsed_line.path
-    pyproject_requires = None  # type: Optional[Tuple[STRING_TYPE, ...]]
+    pyproject_requires = None  # type: Optional[Tuple[str, ...]]
     if parsed_line.pyproject_requires is not None:
         pyproject_requires = tuple(parsed_line.pyproject_requires)
     pyproject_path = (
         Path(parsed_line.pyproject_toml) if parsed_line.pyproject_toml else None
     )
     req_dict = {
         "setup_path": parsed_line.setup_py,
@@ -3080,22 +2837,22 @@
         "link": parsed_line.link,
         "uri": parsed_line.uri,
         "pyproject_requires": pyproject_requires,
         "pyproject_backend": parsed_line.pyproject_backend,
         "pyproject_path": pyproject_path,
         "parsed_line": parsed_line,
         "req": parsed_line.requirement,
+        "_setup_info": parsed_line.setup_info,
     }
     if parsed_line.name is not None:
         req_dict["name"] = parsed_line.name
     return FileRequirement(**req_dict)  # type: ignore
 
 
-def vcs_req_from_parsed_line(parsed_line):
-    # type: (Line) -> VCSRequirement
+def vcs_req_from_parsed_line(parsed_line) -> VCSRequirement:
     line = "{0}".format(parsed_line.line)
     if parsed_line.editable:
         line = "-e {0}".format(line)
     if parsed_line.url is not None:
         link = create_link(
             build_vcs_uri(
                 vcs=parsed_line.vcs,
@@ -3104,15 +2861,15 @@
                 ref=parsed_line.ref,
                 subdirectory=parsed_line.subdirectory,
                 extras=list(parsed_line.extras),
             )
         )
     else:
         link = parsed_line.link
-    pyproject_requires = ()  # type: Optional[Tuple[STRING_TYPE, ...]]
+    pyproject_requires = ()
     if parsed_line.pyproject_requires is not None:
         pyproject_requires = tuple(parsed_line.pyproject_requires)
     vcs_dict = {
         "setup_path": parsed_line.setup_py,
         "path": parsed_line.path,
         "editable": parsed_line.editable,
         "vcs": parsed_line.vcs,
@@ -3144,12 +2901,7 @@
             version=parsed_line.specifier,
             req=parsed_line.requirement,
             extras=parsed_line.extras,
             editable=parsed_line.editable,
             parsed_line=parsed_line,
         )
     return NamedRequirement.from_line(parsed_line.line)
-
-
-if __name__ == "__main__":
-    line = Line("vistir@ git+https://github.com/sarugaku/vistir.git@master")
-    print(line)
```

### Comparing `requirementslib-2.3.0/src/requirementslib/models/setup_info.py` & `requirementslib-2.3.1.dev0/src/requirementslib/models/setup_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,92 +13,62 @@
 import warnings
 from collections.abc import Iterable, Mapping
 from contextlib import ExitStack
 from functools import lru_cache
 from itertools import count
 from os import scandir
 from pathlib import Path
-from typing import Callable, Optional
+from typing import Any, AnyStr, Callable, Dict, Generator, List, Optional, Tuple, Union
 from urllib.parse import parse_qs, urlparse, urlunparse
-from weakref import finalize
 
-import attr
 from distlib.wheel import Wheel
 from pep517 import envbuild, wrappers
 from pip._internal.network.download import Downloader
 from pip._internal.operations.prepare import unpack_url
+from pip._internal.req.req_install import InstallRequirement
 from pip._internal.utils.temp_dir import global_tempdir_manager
-from pip._internal.utils.urls import url_to_path
-from pip._vendor.packaging.markers import Marker
+from pip._vendor.packaging.requirements import Requirement as PackagingRequirement
 from pip._vendor.packaging.specifiers import SpecifierSet
 from pip._vendor.packaging.version import parse
 from pip._vendor.pkg_resources import (
+    DistInfoDistribution,
+    EggInfoDistribution,
     PathMetadata,
     Requirement,
     distributions_from_metadata,
     find_distributions,
 )
-from platformdirs import user_cache_dir
+from pip._vendor.platformdirs import user_cache_dir
+from pip._vendor.pyparsing.core import cached_property
+from pydantic import Field
 
-from ..environment import MYPY_RUNNING
-from ..exceptions import RequirementError
-from ..fileutils import cd, create_tracked_tempdir, temp_path
+from ..fileutils import cd, create_tracked_tempdir, temp_path, url_to_path
 from ..utils import get_pip_command
+from .common import ReqLibBaseModel
 from .old_pip_utils import _copy_source_tree
 from .utils import (
+    HashableRequirement,
+    convert_to_hashable_requirement,
     get_default_pyproject_backend,
     get_name_variants,
     get_pyproject,
     init_requirement,
     split_vcs_method_from_uri,
     strip_extras_markers_from_requirement,
 )
 
-if MYPY_RUNNING:
-    from typing import (
-        Any,
-        AnyStr,
-        Dict,
-        Generator,
-        List,
-        Sequence,
-        Set,
-        Text,
-        Tuple,
-        TypeVar,
-        Union,
-    )
-
-    from pip._internal.index.package_finder import PackageFinder
-    from pip._internal.req.req_install import InstallRequirement
-    from pip._vendor.packaging.requirements import Requirement as PackagingRequirement
-    from pip._vendor.pkg_resources import DistInfoDistribution, EggInfoDistribution
-    from pip._vendor.requests import Session
-    from setuptools.dist import Distribution
-
-    TRequirement = TypeVar("TRequirement")
-    RequirementType = TypeVar(
-        "RequirementType", covariant=True, bound=PackagingRequirement
-    )
-    MarkerType = TypeVar("MarkerType", covariant=True, bound=Marker)
-    STRING_TYPE = Union[str, bytes, Text]
-    S = TypeVar("S", bytes, str, Text)
-    AST_SEQ = TypeVar("AST_SEQ", ast.Tuple, ast.List)
-
-
 CACHE_DIR = os.environ.get("PIPENV_CACHE_DIR", user_cache_dir("pipenv"))
 
 # The following are necessary for people who like to use "if __name__" conditionals
 # in their setup.py scripts
 _setup_stop_after = None
 _setup_distribution = None
 
 
-def pep517_subprocess_runner(cmd, cwd=None, extra_environ=None):
-    # type: (List[AnyStr], Optional[AnyStr], Optional[Mapping[S, S]]) -> None
+def pep517_subprocess_runner(cmd, cwd=None, extra_environ=None) -> None:
     """The default method of calling the wrapper subprocess."""
     env = os.environ.copy()
     if extra_environ:
         env.update(extra_environ)
 
     sp.run(cmd, cwd=cwd, env=env, stdout=sp.PIPE, stderr=sp.STDOUT)
 
@@ -350,26 +320,25 @@
     for root, dirs, files in os.walk(fn, topdown=False):
         for dir_ in [os.path.join(root, d) for d in dirs]:
             set_write_bit(dir_)
         for file_ in [os.path.join(root, f) for f in files]:
             set_write_bit(file_)
 
 
-def make_base_requirements(reqs):
-    # type: (Sequence[STRING_TYPE]) -> Set[BaseRequirement]
-    requirements = set()
+def make_base_requirements(reqs) -> Tuple:
+    requirements = ()
     if not isinstance(reqs, (list, tuple, set)):
         reqs = [reqs]
     for req in reqs:
         if isinstance(req, BaseRequirement):
-            requirements.add(req)
+            requirements += (req,)
         elif isinstance(req, Requirement):
-            requirements.add(BaseRequirement.from_req(req))
+            requirements += (BaseRequirement.from_req(req),)
         elif req and isinstance(req, str) and not req.startswith("#"):
-            requirements.add(BaseRequirement.from_string(req))
+            requirements += (BaseRequirement.from_string(req),)
     return requirements
 
 
 def handle_remove_readonly(func, path, exc):
     """Error handler for shutil.rmtree.
 
     Windows source repo folders are read-only by default, so this error handler
@@ -875,15 +844,15 @@
 
     os.makedirs(src_dir, mode=0o775)
     return src_dir
 
 
 @lru_cache()
 def ensure_reqs(reqs):
-    # type: (List[Union[S, Requirement]]) -> List[Requirement]
+    # type: (List[Union[Requirement]]) -> List[Requirement]
 
     if not isinstance(reqs, Iterable):
         raise TypeError("Expecting an Iterable, got %r" % reqs)
     new_reqs = []
     for req in reqs:
         if not req:
             continue
@@ -904,29 +873,29 @@
 
     fields = [field for field in fields if field in data]
     return fields and all(is_valid(data[field]) for field in fields)
 
 
 def _prepare_wheel_building_kwargs(
     ireq=None,  # type: Optional[InstallRequirement]
-    src_root=None,  # type: Optional[STRING_TYPE]
-    src_dir=None,  # type: Optional[STRING_TYPE]
+    src_root=None,  # type: Optional[str]
+    src_dir=None,  # type: Optional[str]
     editable=False,  # type: bool
 ):
-    # type: (...) -> Dict[STRING_TYPE, STRING_TYPE]
-    download_dir = os.path.join(CACHE_DIR, "pkgs")  # type: STRING_TYPE
+    # type: (...) -> Dict[str, str]
+    download_dir = os.path.join(CACHE_DIR, "pkgs")  # type: str
     os.makedirs(download_dir, exist_ok=True)
 
-    wheel_download_dir = os.path.join(CACHE_DIR, "wheels")  # type: STRING_TYPE
+    wheel_download_dir = os.path.join(CACHE_DIR, "wheels")  # type: str
     os.makedirs(wheel_download_dir, exist_ok=True)
     if src_dir is None:
         if editable and src_root is not None:
             src_dir = src_root
         elif src_root is not None:
-            src_dir = _get_src_dir(root=src_root)  # type: STRING_TYPE
+            src_dir = _get_src_dir(root=src_root)  # type: str
         else:
             src_dir = create_tracked_tempdir(prefix="reqlib-src")
 
     # Let's always resolve in isolation
     if src_dir is None:
         src_dir = create_tracked_tempdir(prefix="reqlib-src")
     build_dir = create_tracked_tempdir(prefix="reqlib-build")
@@ -967,16 +936,15 @@
         )
     else:
         return os.path.isfile(os.path.join(path, "bin/python")) or os.path.isfile(
             os.path.join(path, "bin/activate")
         )
 
 
-def iter_metadata(path, pkg_name=None, metadata_type="egg-info"):
-    # type: (AnyStr, Optional[AnyStr], AnyStr) -> Generator
+def iter_metadata(path, pkg_name=None, metadata_type="egg-info") -> Generator:
     if pkg_name is not None:
         pkg_variants = get_name_variants(pkg_name)
     dirs_to_search = [path]
     while dirs_to_search:
         p = dirs_to_search.pop(0)
         # Skip when the directory is like a venv
         if _is_venv_dir(p):
@@ -1018,85 +986,75 @@
     if pkg_name:
         yield next(iter(dist for dist in dist_dirs if dist is not None), None)
     else:
         for dist_dir in dist_dirs:
             yield dist_dir
 
 
-def get_distinfo_dist(path, pkg_name=None):
-    # type: (S, Optional[S]) -> Optional[DistInfoDistribution]
-
+def get_distinfo_dist(path, pkg_name=None) -> Optional[DistInfoDistribution]:
     dist_dir = next(iter(find_distinfo(path, pkg_name=pkg_name)), None)
     if dist_dir is not None:
         metadata_dir = dist_dir.path
         base_dir = os.path.dirname(metadata_dir)
         dist = next(iter(find_distributions(base_dir)), None)
         if dist is not None:
             return dist
     return None
 
 
-def get_egginfo_dist(path, pkg_name=None):
-    # type: (S, Optional[S]) -> Optional[EggInfoDistribution]
-
+def get_egginfo_dist(path, pkg_name=None) -> Optional[EggInfoDistribution]:
     egg_dir = next(iter(find_egginfo(path, pkg_name=pkg_name)), None)
     if egg_dir is not None:
         metadata_dir = egg_dir.path
         base_dir = os.path.dirname(metadata_dir)
         path_metadata = PathMetadata(base_dir, metadata_dir)
         dist_iter = distributions_from_metadata(path_metadata.egg_info)
         dist = next(iter(dist_iter), None)
         if dist is not None:
             return dist
     return None
 
 
 def get_metadata(path, pkg_name=None, metadata_type=None):
-    # type: (S, Optional[S], Optional[S]) -> Dict[S, Union[S, List[RequirementType], Dict[S, RequirementType]]]
     wheel_allowed = metadata_type == "wheel" or metadata_type is None
     egg_allowed = metadata_type == "egg" or metadata_type is None
     dist = None  # type: Optional[Union[DistInfoDistribution, EggInfoDistribution]]
     if wheel_allowed:
         dist = get_distinfo_dist(path, pkg_name=pkg_name)
     if egg_allowed and dist is None:
         dist = get_egginfo_dist(path, pkg_name=pkg_name)
     if dist is not None:
         return get_metadata_from_dist(dist)
     return {}
 
 
-@lru_cache()
 def get_extra_name_from_marker(marker):
-    # type: (MarkerType) -> Optional[S]
     if not marker:
         raise ValueError("Invalid value for marker: {0!r}".format(marker))
     if not getattr(marker, "_markers", None):
         raise TypeError("Expecting a marker instance, received {0!r}".format(marker))
     for elem in marker._markers:
         if isinstance(elem, tuple) and elem[0].value == "extra":
             return elem[2].value
     return None
 
 
-def get_metadata_from_wheel(wheel_path):
-    # type: (S) -> Dict[Any, Any]
+def get_metadata_from_wheel(wheel_path) -> Dict[Any, Any]:
     if not isinstance(wheel_path, str):
         raise TypeError("Expected string instance, received {0!r}".format(wheel_path))
     try:
         dist = Wheel(wheel_path)
     except Exception:
         pass
     metadata = dist.metadata
     name = metadata.name
     version = metadata.version
     requires = []
-    extras_keys = getattr(metadata, "extras", [])  # type: List[STRING_TYPE]
-    extras = {
-        k: [] for k in extras_keys
-    }  # type: Dict[STRING_TYPE, List[RequirementType]]
+    extras_keys = getattr(metadata, "extras", [])  # type: List[str]
+    extras = {k: [] for k in extras_keys}  # type: Dict[str, List[PackagingRequirement]]
     for req in getattr(metadata, "run_requires", []):
         parsed_req = init_requirement(req)
         parsed_marker = parsed_req.marker
         if parsed_marker:
             extra = get_extra_name_from_marker(parsed_marker)
             if extra is None:
                 requires.append(parsed_req)
@@ -1107,15 +1065,14 @@
             extras[extra].append(parsed_req)
         else:
             requires.append(parsed_req)
     return {"name": name, "version": version, "requires": requires, "extras": extras}
 
 
 def get_metadata_from_dist(dist):
-    # type: (Union[PathMetadata, EggInfoDistribution, DistInfoDistribution]) -> Dict[S, Union[S, List[RequirementType], Dict[S, RequirementType]]]
     try:
         requires = dist.requires()
     except Exception:
         requires = []
     try:
         dep_map = dist._build_dep_map()
     except Exception:
@@ -1155,19 +1112,18 @@
 
 
 def ast_parse_setup_py(path: str, raising: bool = True) -> "Dict[str, Any]":
     return SetupReader.read_setup_py(Path(path), raising)
 
 
 def run_setup(script_path, egg_base=None):
-    # type: (str, Optional[str]) -> Distribution
     """Run a `setup.py` script with a target **egg_base** if provided.
 
-    :param S script_path: The path to the `setup.py` script to run
-    :param Optional[S] egg_base: The metadata directory to build in
+    :param script_path: The path to the `setup.py` script to run
+    :param Optional egg_base: The metadata directory to build in
     :raises FileNotFoundError: If the provided `script_path` does not exist
     :return: The metadata dictionary
     :rtype: Dict[Any, Any]
     """
 
     if not os.path.exists(script_path):
         raise FileNotFoundError(script_path)
@@ -1207,147 +1163,158 @@
             _setup_stop_after = None
             sys.argv = save_argv
             _setup_distribution = get_metadata(egg_base, metadata_type="egg")
         dist = _setup_distribution
     return dist
 
 
-@attr.s(slots=True, frozen=True)
-class BaseRequirement(object):
-    name = attr.ib(default="", eq=True, order=True)  # type: STRING_TYPE
-    requirement = attr.ib(
-        default=None, eq=True, order=True
-    )  # type: Optional[Requirement]
+class BaseRequirement(ReqLibBaseModel):
+    name: str = ""
+    requirement: Optional[HashableRequirement] = None
+
+    class Config:
+        validate_assignment = True
+        arbitrary_types_allowed = True
+        allow_mutation = True
+        include_private_attributes = True
+        keep_untouched = (cached_property,)
+
+    def __setattr__(self, name, value):
+        if name == "requirement" and isinstance(value, Requirement):
+            value = convert_to_hashable_requirement(value)
+        super().__setattr__(name, value)
 
-    def __str__(self):
-        # type: () -> S
+    def __str__(self) -> str:
         return "{0}".format(str(self.requirement))
 
-    def as_dict(self):
-        # type: () -> Dict[STRING_TYPE, Optional[Requirement]]
+    def __hash__(self):
+        return hash((self.name, str(self.requirement)))
+
+    def as_dict(self) -> Dict[str, Optional[Requirement]]:
         return {self.name: self.requirement}
 
-    def as_tuple(self):
-        # type: () -> Tuple[STRING_TYPE, Optional[Requirement]]
+    def as_tuple(self) -> Tuple[str, Optional[Requirement]]:
         return (self.name, self.requirement)
 
     @classmethod
     @lru_cache()
-    def from_string(cls, line):
-        # type: (S) -> BaseRequirement
+    def from_string(cls, line: str) -> "HashableRequirement":
         line = line.strip()
         req = init_requirement(line)
         return cls.from_req(req)
 
     @classmethod
     @lru_cache()
-    def from_req(cls, req):
-        # type: (Requirement) -> BaseRequirement
+    def from_req(cls, req: Requirement) -> "HashableRequirement":
         name = None
         key = getattr(req, "key", None)
         name = getattr(req, "name", None)
         project_name = getattr(req, "project_name", None)
         if key is not None:
             name = key
         if name is None:
             name = project_name
-        return cls(name=name, requirement=req)
+        hashable_req = convert_to_hashable_requirement(req)
+        return cls(name=name, requirement=hashable_req)
 
 
-@attr.s(slots=True, frozen=True)
-class Extra(object):
-    name = attr.ib(default=None, eq=True, order=True)  # type: STRING_TYPE
-    requirements = attr.ib(factory=frozenset, eq=True, order=True, type=frozenset)
-
-    def __str__(self):
-        # type: () -> S
-        return "{0}: {{{1}}}".format(
-            self.name, ", ".join([r.name for r in self.requirements])
-        )
+class SetupInfo(ReqLibBaseModel):
+    name: Optional[str] = None
+    base_dir: Optional[str] = None
+    _version: Optional[str] = None
+    _requirements: Optional[Tuple] = None
+    build_requires: Optional[Tuple] = None
+    build_backend: Optional[str] = None
+    setup_requires: Optional[Tuple] = None
+    python_requires: Optional[SpecifierSet] = None
+    _extras_requirements: Optional[Tuple] = None
+    setup_cfg: Optional[Path] = None
+    setup_py: Optional[Path] = None
+    pyproject: Optional[Path] = None
+    ireq: Optional[InstallRequirement] = None
+    extra_kwargs: Optional[Dict] = Field(default_factory=dict)
+    metadata: Optional[Tuple[str]] = None
+    _is_built: bool = False
+    _ran_setup: bool = False
+
+    class Config:
+        validate_assignment = True
+        arbitrary_types_allowed = True
+        allow_mutation = True
+        include_private_attributes = True
+        keep_untouched = (cached_property,)
+
+    def __init__(self, **data):
+        super().__init__(**data)
+        self._is_built = False
+        self._ran_setup = False
+        if not self.build_backend:
+            self.build_backend = "setuptools.build_meta:__legacy__"
+        if self._requirements is None:
+            self._requirements = ()
+        self.get_initial_info()
+        self.get_info()
 
-    def add(self, req):
-        # type: (BaseRequirement) -> "Extra"
-        if req not in self.requirements:
-            current_set = set(self.requirements)
-            current_set.add(req)
-            return attr.evolve(self, requirements=frozenset(current_set))
-        return self
+    def __hash__(self):
+        return hash(
+            (
+                self.name,
+                self._version,
+                self._requirements,
+                self.build_requires,
+                self.build_backend,
+                self.setup_requires,
+                self.python_requires,
+                self._extras_requirements,
+                self.setup_cfg,
+                self.setup_py,
+                self.pyproject,
+                self.ireq,
+            )
+        )
 
-    def as_dict(self):
-        # type: () -> Dict[STRING_TYPE, Tuple[RequirementType, ...]]
-        return {self.name: tuple([r.requirement for r in self.requirements])}
-
-
-@attr.s(slots=True, eq=True, hash=True)
-class SetupInfo(object):
-    name = attr.ib(default=None, eq=True)  # type: STRING_TYPE
-    base_dir = attr.ib(default=None, eq=True, hash=False)  # type: STRING_TYPE
-    _version = attr.ib(default=None, eq=True)  # type: STRING_TYPE
-    _requirements = attr.ib(
-        type=frozenset, factory=frozenset, eq=True, hash=True
-    )  # type: Optional[frozenset]
-    build_requires = attr.ib(default=None, eq=True)  # type: Optional[Tuple]
-    build_backend = attr.ib(eq=True)  # type: STRING_TYPE
-    setup_requires = attr.ib(default=None, eq=True)  # type: Optional[Tuple]
-    python_requires = attr.ib(default=None, eq=True)  # type: Optional[SpecifierSet]
-    _extras_requirements = attr.ib(default=None, eq=True)  # type: Optional[Tuple]
-    setup_cfg = attr.ib(type=Path, default=None, eq=True, hash=False)
-    setup_py = attr.ib(type=Path, default=None, eq=True, hash=False)
-    pyproject = attr.ib(type=Path, default=None, eq=True, hash=False)
-    ireq = attr.ib(
-        default=None, eq=True, hash=False
-    )  # type: Optional[InstallRequirement]
-    extra_kwargs = attr.ib(default=attr.Factory(dict), type=dict, eq=False, hash=False)
-    metadata = attr.ib(default=None)  # type: Optional[Tuple[STRING_TYPE]]
-    stack = attr.ib(default=None, eq=False)  # type: Optional[ExitStack]
-    _finalizer = attr.ib(default=None, eq=False)  # type: Any
-
-    def __attrs_post_init__(self):
-        self._finalizer = finalize(self, self.stack.close)
-
-    @build_backend.default
-    def get_build_backend(self):
-        # type: () -> STRING_TYPE
-        return get_default_pyproject_backend()
+    def __eq__(self, other):
+        if not isinstance(other, SetupInfo):
+            return NotImplemented
+        return (
+            self.name == other.name
+            and self._version == other._version
+            and self._requirements == other._requirements
+            and self.build_requires == other.build_requires
+        )
 
-    @property
-    def requires(self):
-        # type: () -> Dict[S, RequirementType]
+    @cached_property
+    def requires(self) -> Dict[str, HashableRequirement]:
         if self._requirements is None:
-            self._requirements = frozenset()
-            self.get_info()
+            self._requirements = ()
         return {req.name: req.requirement for req in self._requirements}
 
-    @property
-    def extras(self):
-        # type: () -> Dict[S, Optional[Any]]
+    @cached_property
+    def extras(self) -> Dict[str, Optional[Any]]:
         if self._extras_requirements is None:
             self._extras_requirements = ()
-            self.get_info()
         extras_dict = {}
         extras = set(self._extras_requirements)
         for section, deps in extras:
             if isinstance(deps, BaseRequirement):
                 extras_dict[section] = deps.requirement
             elif isinstance(deps, (list, tuple)):
                 extras_dict[section] = [d.requirement for d in deps]
         return extras_dict
 
     @property
-    def version(self):
-        # type: () -> Optional[str]
+    def version(self) -> Optional[str]:
         if not self._version:
-            info = self.get_info()
+            info = self.as_dict()
             self._version = info.get("version", None)
         return self._version
 
     @property
-    def egg_base(self):
-        # type: () -> S
-        base = None  # type: Optional[STRING_TYPE]
+    def egg_base(self) -> str:
+        base = None  # type: Optional[str]
         if self.setup_py.exists():
             base = self.setup_py.parent
         elif self.pyproject.exists():
             base = self.pyproject.parent
         elif self.setup_cfg.exists():
             base = self.setup_cfg.parent
         if base is None:
@@ -1356,15 +1323,15 @@
             base = Path(self.extra_kwargs["src_dir"])
         egg_base = base.joinpath("reqlib-metadata")
         if not egg_base.exists():
             atexit.register(rmtree, egg_base.as_posix())
         egg_base.mkdir(parents=True, exist_ok=True)
         return egg_base.as_posix()
 
-    def update_from_dict(self, metadata):
+    def update_from_dict(self, metadata: Dict[str, Any]) -> None:
         name = metadata.get("name", self.name)
         if isinstance(name, str):
             self.name = self.name if self.name else name
         version = metadata.get("version", None)
         if version:
             try:
                 parse(version)
@@ -1374,121 +1341,89 @@
                 version = version
         if version:
             self._version = version
         build_requires = metadata.get("build_requires", [])
         if self.build_requires is None:
             self.build_requires = ()
         self.build_requires = tuple(set(self.build_requires) | set(build_requires))
-        self._requirements = (
-            frozenset() if self._requirements is None else self._requirements
-        )
-        requirements = set(self._requirements)
+        self._requirements = () if self._requirements is None else self._requirements
+        requirements = self._requirements
         install_requires = make_base_requirements(metadata.get("install_requires", []))
-        requirements |= install_requires
+        requirements += install_requires
         setup_requires = make_base_requirements(metadata.get("setup_requires", []))
         if self.setup_requires is None:
             self.setup_requires = ()
-        self.setup_requires = tuple(set(self.setup_requires) | setup_requires)
-        if self.ireq.editable:
-            requirements |= setup_requires
-        # TODO: Should this be a specifierset?
+        self.setup_requires = tuple(self.setup_requires + setup_requires)
+        requirements += self.setup_requires
         self.python_requires = metadata.get("python_requires", self.python_requires)
         extras_require = metadata.get("extras_require", {})
         extras_tuples = []
         if self._extras_requirements is None:
             self._extras_requirements = ()
         for section in set(extras_require) - {v[0] for v in self._extras_requirements}:
             extras = extras_require[section]
             extras_set = make_base_requirements(extras)
             if self.ireq and self.ireq.extras and section in self.ireq.extras:
-                requirements |= extras_set
+                requirements += extras_set
             extras_tuples.append((section, tuple(extras_set)))
         self._extras_requirements += tuple(extras_tuples)
-        build_backend = metadata.get("build_backend", "setuptools.build_meta:__legacy__")
-        if not self.build_backend:
-            self.build_backend = build_backend
-        self._requirements = frozenset(requirements)
+        self.build_backend = metadata.get(
+            "build_backend", "setuptools.build_meta:__legacy__"
+        )
+        self._requirements = requirements
 
-    def get_extras_from_ireq(self):
-        # type: () -> None
+    def get_extras_from_ireq(self) -> None:
         if self.ireq and self.ireq.extras:
             for extra in self.ireq.extras:
                 if extra in self.extras:
                     extras = make_base_requirements(self.extras[extra])
-                    self._requirements = frozenset(set(self._requirements) | extras)
+                    self._requirements = self._requirements + extras
                 else:
                     extras = tuple(make_base_requirements(extra))
                     self._extras_requirements += (extra, extras)
 
-    def parse_setup_cfg(self):
-        # type: () -> Dict[STRING_TYPE, Any]
+    def parse_setup_cfg(self) -> Dict[str, Any]:
         if self.setup_cfg is not None and self.setup_cfg.exists():
             try:
                 parsed = setuptools_parse_setup_cfg(self.setup_cfg.as_posix())
             except Exception:
                 parsed = parse_setup_cfg(self.setup_cfg.as_posix())
             if not parsed:
                 return {}
             return parsed
         return {}
 
-    def parse_setup_py(self):
-        # type: () -> Dict[STRING_TYPE, Any]
+    def parse_setup_py(self) -> Dict[str, Any]:
         if self.setup_py is not None and self.setup_py.exists():
             parsed = ast_parse_setup_py(self.setup_py.as_posix())
             if not parsed:
                 return {}
             return parsed
         return {}
 
-    def run_setup(self):
-        # type: () -> "SetupInfo"
-        if self.setup_py is not None and self.setup_py.exists():
+    def run_setup(self) -> None:
+        if not self._ran_setup and self.setup_py is not None and self.setup_py.exists():
             dist = run_setup(self.setup_py.as_posix(), egg_base=self.egg_base)
             target_cwd = self.setup_py.parent.as_posix()
             with temp_path(), cd(target_cwd):
                 if not dist:
                     metadata = self.get_egg_metadata()
                     if metadata:
-                        return self.populate_metadata(metadata)
-
-                if isinstance(dist, Mapping):
+                        self.populate_metadata(metadata)
+                elif isinstance(dist, Mapping):
                     self.populate_metadata(dist)
-                    return
-                name = dist.get_name()
-                if name:
-                    self.name = name
-                update_dict = {}
-                if dist.python_requires:
-                    update_dict["python_requires"] = dist.python_requires
-                update_dict["extras_require"] = {}
-                if dist.extras_require:
-                    for extra, extra_requires in dist.extras_require:
-                        extras_tuple = make_base_requirements(extra_requires)
-                        update_dict["extras_require"][extra] = extras_tuple
-                update_dict["install_requires"] = make_base_requirements(
-                    dist.get_requires()
-                )
-                if dist.setup_requires:
-                    update_dict["setup_requires"] = make_base_requirements(
-                        dist.setup_requires
-                    )
-                version = dist.get_version()
-                if version:
-                    update_dict["version"] = version
-                return self.update_from_dict(update_dict)
+                self._ran_setup = True
 
     @property
-    def pep517_config(self):
+    def pep517_config(self) -> Dict[str, Any]:
         config = {}
         config.setdefault("--global-option", [])
         return config
 
-    def build_wheel(self):
-        # type: () -> S
+    def build_wheel(self) -> str:
         need_delete = False
         if not self.pyproject.exists():
             if not self.build_requires:
                 build_requires = '"setuptools", "wheel"'
             else:
                 build_requires = ", ".join(
                     ['"{0}"'.format(r) for r in self.build_requires]
@@ -1518,16 +1453,15 @@
             dist_type="wheel",
         )
         if need_delete:
             self.pyproject.unlink()
         return result
 
     # noinspection PyPackageRequirements
-    def build_sdist(self):
-        # type: () -> S
+    def build_sdist(self) -> str:
         need_delete = False
         if not self.pyproject.exists():
             if not self.build_requires:
                 build_requires = '"setuptools", "wheel"'
             else:
                 build_requires = ", ".join(
                     ['"{0}"'.format(r) for r in self.build_requires]
@@ -1550,17 +1484,17 @@
             config_settings=self.pep517_config,
             dist_type="sdist",
         )
         if need_delete:
             self.pyproject.unlink()
         return result
 
-    def build(self):
-        # type: () -> "SetupInfo"
-        dist_path = None
+    def build(self) -> None:
+        if self._is_built:
+            return
         metadata = None
         try:
             dist_path = self.build_wheel()
             metadata = self.get_metadata_from_wheel(
                 os.path.join(self.extra_kwargs["build_dir"], dist_path)
             )
         except Exception:
@@ -1574,55 +1508,38 @@
         if metadata:
             self.populate_metadata(metadata)
         if not self.metadata or not self.name:
             metadata = self.get_egg_metadata()
             if metadata:
                 self.populate_metadata(metadata)
         if not self.metadata or not self.name:
-            return self.run_setup()
-        return self
-
-    def reload(self):
-        # type: () -> Dict[S, Any]
-        """Wipe existing distribution info metadata for rebuilding.
+            self.run_setup()
+        self._is_built = True
 
-        Erases metadata from **self.egg_base** and unsets
-        **self.requirements** and **self.extras**.
-        """
-        for metadata_dir in os.listdir(self.egg_base):
-            shutil.rmtree(metadata_dir, ignore_errors=True)
-        self.metadata = None
-        self._requirements = frozenset()
-        self._extras_requirements = ()
-        self.get_info()
-
-    def get_metadata_from_wheel(self, wheel_path):
-        # type: (S) -> Dict[Any, Any]
+    def get_metadata_from_wheel(self, wheel_path) -> Dict[Any, Any]:
         """Given a path to a wheel, return the metadata from that wheel.
 
         :return: A dictionary of metadata from the provided wheel
         :rtype: Dict[Any, Any]
         """
 
         metadata_dict = get_metadata_from_wheel(wheel_path)
         return metadata_dict
 
-    def get_egg_metadata(self, metadata_dir=None, metadata_type=None):
-        # type: (Optional[AnyStr], Optional[AnyStr]) -> Dict[Any, Any]
+    def get_egg_metadata(self, metadata_dir=None, metadata_type=None) -> Dict[Any, Any]:
         """Given a metadata directory, return the corresponding metadata
         dictionary.
 
         :param Optional[str] metadata_dir: Root metadata path, default: `os.getcwd()`
         :param Optional[str] metadata_type: Type of metadata to search for, default None
         :return: A metadata dictionary built from the metadata in the given location
-        :rtype: Dict[Any, Any]
         """
 
         package_indicators = [self.pyproject, self.setup_py, self.setup_cfg]
-        metadata_dirs = []  # type: List[STRING_TYPE]
+        metadata_dirs = []  # type: List[str]
         if any([fn is not None and fn.exists() for fn in package_indicators]):
             metadata_dirs = [
                 self.extra_kwargs["build_dir"],
                 self.egg_base,
                 self.extra_kwargs["src_dir"],
             ]
         if metadata_dir is not None:
@@ -1631,54 +1548,49 @@
             get_metadata(d, pkg_name=self.name, metadata_type=metadata_type)
             for d in metadata_dirs
             if os.path.exists(d)
         ]
         metadata = next(iter(d for d in metadata if d), None)
         return metadata
 
-    def populate_metadata(self, metadata):
-        # type: (Dict[Any, Any]) -> "SetupInfo"
-        """Populates the metadata dictionary from the supplied metadata.
-
-        :return: The current instance.
-        :rtype: `SetupInfo`
-        """
+    def populate_metadata(self, metadata) -> "SetupInfo":
+        """Populates the metadata dictionary from the supplied metadata."""
 
         _metadata = ()
         for k, v in metadata.items():
             if k == "extras" and isinstance(v, dict):
                 extras = ()
                 for extra, reqs in v.items():
                     extras += ((extra, tuple(reqs)),)
                 _metadata += extras
             elif isinstance(v, (list, tuple)):
                 _metadata += (k, tuple(v))
             else:
                 _metadata += (k, v)
         self.metadata = _metadata
-        cleaned = metadata.copy()
-        cleaned.update(
-            {
-                "install_requires": metadata.get("requires", []),
-                "extras_require": metadata.get("extras", {}),
-            }
-        )
-        if cleaned:
-            self.update_from_dict(cleaned.copy())
-        else:
-            self.update_from_dict(metadata)
+        self.setup_requires = make_base_requirements(metadata.get("requires", ()))
+        self._requirements += tuple(self.setup_requires)
+        name = metadata.get("name")
+        if name:
+            self.name = name
+        version = metadata.get("version")
+        if version:
+            self._version = version
+        extras_require = metadata.get("extras", ())
+        extras_tuples = []
+        for section in set(extras_require):
+            extras = extras_require[section]
+            extras_set = make_base_requirements(extras)
+            if self.ireq and self.ireq.extras and section in self.ireq.extras:
+                self._requirements += extras_set
+            extras_tuples.append((section, tuple(extras_set)))
         return self
 
-    def run_pyproject(self):
-        # type: () -> "SetupInfo"
-        """Populates the **pyproject.toml** metadata if available.
-
-        :return: The current instance
-        :rtype: `SetupInfo`
-        """
+    def run_pyproject(self) -> "SetupInfo":
+        """Populates the **pyproject.toml** metadata if available."""
         if self.pyproject and self.pyproject.exists():
             result = get_pyproject(self.pyproject.parent)
             if result is not None:
                 requires, backend = result
                 if self.build_requires is None:
                     self.build_requires = ()
                 if backend:
@@ -1687,19 +1599,19 @@
                     self.build_backend = get_default_pyproject_backend()
                 if requires:
                     self.build_requires = tuple(set(requires) | set(self.build_requires))
                 else:
                     self.build_requires = ("setuptools", "wheel")
         return self
 
-    def get_initial_info(self):
-        # type: () -> Dict[S, Any]
+    def get_initial_info(self) -> Dict[str, Any]:
         parse_setupcfg = False
         parse_setuppy = False
         self.run_pyproject()
+        self.run_setup()
         if self.setup_cfg and self.setup_cfg.exists():
             parse_setupcfg = True
         if self.setup_py and self.setup_py.exists():
             parse_setuppy = True
         if (
             self.build_backend.startswith("setuptools")
             and parse_setuppy
@@ -1714,71 +1626,63 @@
                         parsed.update(self.parse_setup_cfg())
             except Unparsable:
                 pass
             else:
                 self.update_from_dict(parsed)
                 return self.as_dict()
 
-        return self.get_info()
+        return self.as_dict()
 
-    def get_info(self):
-        # type: () -> Dict[S, Any]
+    def get_info(self) -> None:
         if self.metadata is None:
-            with cd(self.base_dir):
-                self.build()
-
-        if self.setup_py and self.setup_py.exists() and self.metadata is None:
-            if not self.requires or not self.name:
-                try:
-                    with cd(self.base_dir):
-                        self.run_setup()
-                except Exception:
-                    with cd(self.base_dir):
-                        metadata = self.get_egg_metadata()
-                        if metadata:
-                            self.populate_metadata(metadata)
-                if self.metadata is None or not self.name:
-                    with cd(self.base_dir):
-                        metadata = self.get_egg_metadata()
-                        if metadata:
-                            self.populate_metadata(metadata)
+            self.build()
 
-        return self.as_dict()
+        if self.setup_py and self.setup_py.exists():
+            try:
+                self.run_setup()
+            except Exception:
+                metadata = self.get_egg_metadata()
+                if metadata:
+                    self.populate_metadata(metadata)
+            if self.metadata is None or not self.name:
+                metadata = self.get_egg_metadata()
+                if metadata:
+                    self.populate_metadata(metadata)
 
-    def as_dict(self):
-        # type: () -> Dict[STRING_TYPE, Any]
+    def as_dict(self) -> Dict[str, Any]:
         prop_dict = {
             "name": self.name,
             "version": self.version if self._version else None,
             "base_dir": self.base_dir,
             "ireq": self.ireq,
             "build_backend": self.build_backend,
             "build_requires": self.build_requires,
-            "requires": self.requires if self._requirements else None,
+            "requires": self.requires,
             "setup_requires": self.setup_requires,
             "python_requires": self.python_requires,
-            "extras": self.extras if self._extras_requirements else None,
+            "extras": self.extras,
             "extra_kwargs": self.extra_kwargs,
             "setup_cfg": self.setup_cfg,
             "setup_py": self.setup_py,
             "pyproject": self.pyproject,
         }
         return {k: v for k, v in prop_dict.items() if v}
 
     @classmethod
-    def from_requirement(cls, requirement, finder=None):
-        # type: (TRequirement, Optional[PackageFinder]) -> Optional[SetupInfo]
-        ireq = requirement.as_ireq()
+    def from_requirement(cls, requirement, finder=None) -> Optional["SetupInfo"]:
+        ireq = requirement.ireq
         subdir = getattr(requirement.req, "subdirectory", None)
         return cls.from_ireq(ireq, subdir=subdir, finder=finder)
 
     @classmethod
-    @lru_cache()
-    def from_ireq(cls, ireq, subdir=None, finder=None, session=None):
-        # type: (InstallRequirement, Optional[AnyStr], Optional[PackageFinder], Optional[Session]) -> Optional[SetupInfo]
+    def from_ireq(
+        cls, ireq, subdir=None, finder=None, session=None
+    ) -> Optional["SetupInfo"]:
+        if not ireq:
+            return None
         if not ireq.link:
             return None
         if ireq.link.is_wheel:
             return None
         stack = ExitStack()
         if not session:
             cmd = get_pip_command()
@@ -1789,36 +1693,28 @@
         parsed = urlparse(uri)
         if "file" in parsed.scheme:
             url_path = parsed.path
             if "@" in url_path:
                 url_path, _, _ = url_path.rpartition("@")
             parsed = parsed._replace(path=url_path)
             uri = urlunparse(parsed)
-        path = None
         is_file = False
         if ireq.link.scheme == "file" or uri.startswith("file://"):
             is_file = True
-            if "file:/" in uri and "file:///" not in uri:
-                uri = uri.replace("file:/", "file:///")
-            path = url_to_path(uri)
         kwargs = _prepare_wheel_building_kwargs(ireq)
         is_artifact_or_vcs = getattr(
             ireq.link, "is_vcs", getattr(ireq.link, "is_artifact", False)
         )
         is_vcs = True if vcs else is_artifact_or_vcs
         download_dir = None
         if not (ireq.editable and is_file and is_vcs):
             if ireq.is_wheel:
                 download_dir = kwargs["wheel_download_dir"]
             else:
                 download_dir = kwargs["download_dir"]
-        elif path is not None and os.path.isdir(path):
-            raise RequirementError(
-                "The file URL points to a directory not installable: {}".format(ireq.link)
-            )
         # this ensures the build dir is treated as the temporary build location
         # and the source dir is treated as permanent / not deleted by pip
         build_location_func = getattr(ireq, "build_location", None)
         if build_location_func is None:
             build_location_func = getattr(ireq, "ensure_build_location", None)
         if not ireq.source_dir:
             if subdir:
@@ -1846,28 +1742,29 @@
                     location=location,
                     download=Downloader(session, "off"),
                     verbosity=1,
                     download_dir=download_dir,
                     hashes=ireq.hashes(True),
                 )
         created = cls.create(
-            ireq.source_dir, subdirectory=subdir, ireq=ireq, kwargs=kwargs, stack=stack
+            ireq.source_dir,
+            subdirectory=subdir,
+            ireq=ireq,
+            kwargs=kwargs,
         )
         return created
 
     @classmethod
     def create(
         cls,
-        base_dir,  # type: str
-        subdirectory=None,  # type: Optional[str]
-        ireq=None,  # type: Optional[InstallRequirement]
-        kwargs=None,  # type: Optional[Dict[str, str]]
-        stack=None,  # type: Optional[ExitStack]
-    ):
-        # type: (...) -> Optional[SetupInfo]
+        base_dir: str,
+        subdirectory: Optional[str] = None,
+        ireq: Optional[InstallRequirement] = None,
+        kwargs: Optional[Dict[str, str]] = None,
+    ) -> Optional["SetupInfo"]:
         if not base_dir or base_dir is None:
             return None
 
         creation_kwargs = {"extra_kwargs": kwargs}
         if not isinstance(base_dir, Path):
             base_dir = Path(base_dir)
         creation_kwargs["base_dir"] = base_dir.as_posix()
@@ -1876,15 +1773,12 @@
         if subdirectory is not None:
             base_dir = base_dir.joinpath(subdirectory)
         setup_py = base_dir.joinpath("setup.py")
         setup_cfg = base_dir.joinpath("setup.cfg")
         creation_kwargs["pyproject"] = pyproject
         creation_kwargs["setup_py"] = setup_py
         creation_kwargs["setup_cfg"] = setup_cfg
-        if stack is None:
-            stack = ExitStack()
-        creation_kwargs["stack"] = stack
         if ireq:
             creation_kwargs["ireq"] = ireq
         created = cls(**creation_kwargs)
         created.get_initial_info()
         return created
```

### Comparing `requirementslib-2.3.0/src/requirementslib/models/url.py` & `requirementslib-2.3.1.dev0/src/requirementslib/models/url.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
+from typing import Dict, Optional, Text, Tuple, TypeVar, Union
 from urllib.parse import quote
 from urllib.parse import unquote as url_unquote
 from urllib.parse import unquote_plus
 
-import attr
 from pip._internal.models.link import Link
 from pip._internal.req.constructors import _strip_extras
-from urllib3.util import parse_url as urllib3_parse
-from urllib3.util.url import Url
+from pip._vendor.urllib3.util import parse_url as urllib3_parse
+from pip._vendor.urllib3.util.url import Url
+from pydantic import Field
 
 from ..environment import MYPY_RUNNING
 from ..utils import is_installable_file
-from .utils import extras_to_string, parse_extras
+from .common import ReqLibBaseModel
+from .utils import DIRECT_URL_RE, extras_to_string, parse_extras_str, split_ref_from_uri
 
 if MYPY_RUNNING:
-    from typing import Dict, Optional, Text, Tuple, TypeVar, Union
 
     _T = TypeVar("_T")
     STRING_TYPE = Union[bytes, str, Text]
     S = TypeVar("S", bytes, str, Text)
 
 
-def _get_parsed_url(url):
-    # type: (S) -> Url
+def _get_parsed_url(url) -> Url:
     """This is a stand-in function for `urllib3.util.parse_url`
 
     The original function doesn't handle special characters very well, this simply splits
     out the authentication section, creates the parsed url, then puts the authentication
     section back in, bypassing validation.
 
     :return: The new, parsed URL object
@@ -40,148 +40,133 @@
         url = "{scheme}://{url}".format(scheme=scheme, url=url)
         parsed = urllib3_parse(url)._replace(auth=auth)
     if parsed.auth:
         return parsed._replace(auth=url_unquote(parsed.auth))
     return parsed
 
 
-def remove_password_from_url(url):
-    # type: (S) -> S
-    """Given a url, remove the password and insert 4 dashes.
-
-    :param url: The url to replace the authentication in
-    :type url: S
-    :return: The new URL without authentication
-    :rtype: S
-    """
-
-    parsed = _get_parsed_url(url)
-    if parsed.auth:
-        auth, _, _ = parsed.auth.partition(":")
-        return parsed._replace(auth="{auth}:----".format(auth=auth)).url
-    return parsed.url
-
-
-@attr.s(hash=True)
-class URI(object):
-    #: The target hostname, e.g. `amazon.com`
-    host = attr.ib(type=str)
-    #: The URI Scheme, e.g. `salesforce`
-    scheme = attr.ib(default="https", type=str)
-    #: The numeric port of the url if specified
-    port = attr.ib(default=None, type=int)
-    #: The url path, e.g. `/path/to/endpoint`
-    path = attr.ib(default="", type=str)
-    #: Query parameters, e.g. `?variable=value...`
-    query = attr.ib(default="", type=str)
-    #: URL Fragments, e.g. `#fragment=value`
-    fragment = attr.ib(default="", type=str)
-    #: Subdirectory fragment, e.g. `&subdirectory=blah...`
-    subdirectory = attr.ib(default="", type=str)
-    #: VCS ref this URI points at, if available
-    ref = attr.ib(default="", type=str)
-    #: The username if provided, parsed from `user:password@hostname`
-    username = attr.ib(default="", type=str)
-    #: Password parsed from `user:password@hostname`
-    password = attr.ib(default="", type=str, repr=False)
-    #: A dictionary representing query fragments
-    query_dict = attr.ib(factory=dict, type=dict)
-    #: The name of the specified package in case it is a VCS URI with an egg fragment
-    name = attr.ib(default="", type=str)
-    #: Any extras requested from the requirement
-    extras = attr.ib(factory=tuple, type=tuple)
-    #: Whether the url was parsed as a direct pep508-style URL
-    is_direct_url = attr.ib(default=False, type=bool)
-    #: Whether the url was an implicit `git+ssh` url (passed as `git+git@`)
-    is_implicit_ssh = attr.ib(default=False, type=bool)
-    _auth = attr.ib(default=None, type=str, repr=False)
-    _fragment_dict = attr.ib(factory=dict, type=dict)
-    _username_is_quoted = attr.ib(type=bool, default=False)
-    _password_is_quoted = attr.ib(type=bool, default=False)
+class URI(ReqLibBaseModel):
+    host: Optional[str] = Field(...)
+    scheme: Optional[str] = Field(
+        "https", description="The URI Scheme, e.g. `salesforce`"
+    )
+    port: Optional[int] = Field(
+        None, description="The numeric port of the url if specified"
+    )
+    path: Optional[str] = Field("", description="The url path, e.g. `/path/to/endpoint`")
+    query: Optional[str] = Field(
+        "", description="Query parameters, e.g. `?variable=value...`"
+    )
+    fragment: Optional[str] = Field(
+        "", description="URL Fragments, e.g. `#fragment=value`"
+    )
+    subdirectory: Optional[str] = Field(
+        "", description="Subdirectory fragment, e.g. `&subdirectory=blah...`"
+    )
+    ref: Optional[str] = Field("", description="VCS ref this URI points at, if available")
+    username: Optional[str] = Field(
+        "", description="The username if provided, parsed from `user:password@hostname`"
+    )
+    password: Optional[str] = Field(
+        "", description="Password parsed from `user:password@hostname`", repr=False
+    )
+    query_dict: Optional[Dict] = Field(default_factory=dict)
+    name: Optional[str] = Field(
+        "",
+        description="The name of the specified package in case it is a VCS URI with an egg fragment",
+    )
+    extras: Optional[Tuple] = Field(default_factory=tuple)
+    is_direct_url: Optional[bool] = Field(False)
+    is_implicit_ssh: Optional[bool] = Field(False)
+    auth: Optional[str] = None
+    _fragment_dict: Optional[Dict] = Field(default_factory=dict)
+    _username_is_quoted: Optional[bool] = False
+    _password_is_quoted: Optional[bool] = False
+
+    class Config:
+        validate_assignment = True
+        arbitrary_types_allowed = True
+        allow_mutation = True
+        include_private_attributes = True
+        # keep_untouched = (cached_property,)
+
+    def __init__(self, **data):
+        super().__init__(**data)
+        self._parse_auth()
+        self._parse_query()
+        self._parse_fragment()
 
-    def _parse_query(self):
-        # type: () -> URI
+    def _parse_query(self) -> None:
         query = self.query if self.query is not None else ""
         query_dict = dict()
         queries = query.split("&")
         query_items = []
         subdirectory = self.subdirectory if self.subdirectory else None
         for q in queries:
             key, _, val = q.partition("=")
             val = unquote_plus(val)
             if key == "subdirectory" and not subdirectory:
                 subdirectory = val
             else:
                 query_items.append((key, val))
         query_dict.update(query_items)
-        return attr.evolve(
-            self, query_dict=query_dict, subdirectory=subdirectory, query=query
-        )
+        self.query_dict = query_dict
+        self.subdirectory = subdirectory
+        self.query = query
 
-    def _parse_fragment(self):
-        # type: () -> URI
+    def _parse_fragment(self) -> None:
         subdirectory = self.subdirectory if self.subdirectory else ""
         fragment = self.fragment if self.fragment else ""
         if self.fragment is None:
             return self
         fragments = self.fragment.split("&")
         fragment_items = {}
         name = self.name if self.name else ""
         extras = self.extras
         for q in fragments:
             key, _, val = q.partition("=")
             val = unquote_plus(val)
             fragment_items[key] = val
             if key == "egg":
-                from .utils import parse_extras
+                from .utils import parse_extras_str
 
                 name, stripped_extras = _strip_extras(val)
                 if stripped_extras:
-                    extras = tuple(parse_extras(stripped_extras))
+                    extras = tuple(parse_extras_str(stripped_extras))
             elif key == "subdirectory":
                 subdirectory = val
-        return attr.evolve(
-            self,
-            fragment_dict=fragment_items,
-            subdirectory=subdirectory,
-            fragment=fragment,
-            extras=extras,
-            name=name,
-        )
-
-    def _parse_auth(self):
-        # type: () -> URI
-        if self._auth:
-            username, _, password = self._auth.partition(":")
+        self.name = name
+        self.extras = extras
+        self.subdirectory = subdirectory
+        self.fragment = fragment
+        self._fragment_dict = fragment_items
+
+    def _parse_auth(self) -> None:
+        if self.auth:
+            username, _, password = self.auth.partition(":")
             username_is_quoted, password_is_quoted = False, False
             quoted_username, quoted_password = "", ""
             if password:
                 quoted_password = quote(password)
                 password_is_quoted = quoted_password != password
             if username:
                 quoted_username = quote(username)
                 username_is_quoted = quoted_username != username
-            return attr.evolve(
-                self,
-                username=quoted_username,
-                password=quoted_password,
-                username_is_quoted=username_is_quoted,
-                password_is_quoted=password_is_quoted,
-            )
-        return self
+            self.username = quoted_username
+            self.password = quoted_password
+            self._username_is_quoted = username_is_quoted
+            self._password_is_quoted = password_is_quoted
 
-    def get_password(self, unquote=False, include_token=True):
-        # type: (bool, bool) -> str
+    def get_password(self, unquote=False, include_token=True) -> str:
         password = self.password if self.password else ""
         if password and unquote and self._password_is_quoted:
             password = url_unquote(password)
         return password
 
-    def get_username(self, unquote=False):
-        # type: (bool) -> str
+    def get_username(self, unquote=False) -> str:
         username = self.username if self.username else ""
         if username and unquote and self._username_is_quoted:
             username = url_unquote(username)
         return username
 
     @staticmethod
     def parse_subdirectory(url_part):
@@ -194,32 +179,30 @@
             else:
                 subdir = "&{0}".format(subdir.strip())
         return url_part.strip(), subdir
 
     @classmethod
     def get_parsed_url(cls, url):
         # if there is a "#" in the auth section, this could break url parsing
+        maybe_auth = None
         parsed_url = _get_parsed_url(url)
         if "@" in url and "#" in url:
             scheme = "{0}://".format(parsed_url.scheme)
             if parsed_url.scheme == "file":
                 scheme = "{0}/".format(scheme)
             url_without_scheme = url.replace(scheme, "")
             maybe_auth, _, maybe_url = url_without_scheme.partition("@")
             if "#" in maybe_auth and (not parsed_url.host or "." not in parsed_url.host):
                 new_parsed_url = _get_parsed_url("{0}{1}".format(scheme, maybe_url))
                 new_parsed_url = new_parsed_url._replace(auth=maybe_auth)
                 return new_parsed_url
         return parsed_url
 
     @classmethod
-    def parse(cls, url):
-        # type: (S) -> URI
-        from .utils import DIRECT_URL_RE, split_ref_from_uri
-
+    def parse(cls, url) -> "URI":
         is_direct_url = False
         name_with_extras = None
         is_implicit_ssh = url.strip().startswith("git+git@")
         if is_implicit_ssh:
             from ..utils import add_ssh_scheme_to_git_uri
 
             url = add_ssh_scheme_to_git_uri(url)
@@ -243,15 +226,15 @@
                 raise ValueError("Failed parsing URL {0!r} - Not a valid url".format(url))
         parsed_dict = dict(parsed._asdict()).copy()
         parsed_dict["is_direct_url"] = is_direct_url
         parsed_dict["is_implicit_ssh"] = is_implicit_ssh
         parsed_dict.update(
             **update_url_name_and_fragment(name_with_extras, ref, parsed_dict)
         )  # type: ignore
-        return cls(**parsed_dict)._parse_auth()._parse_query()._parse_fragment()
+        return cls(**parsed_dict)
 
     def to_string(
         self,
         escape_password=True,  # type: bool
         unquote=True,  # type: bool
         direct=None,  # type: Optional[bool]
         strip_ssh=False,  # type: bool
@@ -471,23 +454,25 @@
 def update_url_name_and_fragment(name_with_extras, ref, parsed_dict):
     # type: (Optional[str], Optional[str], Dict[str, Optional[str]]) -> Dict[str, Optional[str]]
     if name_with_extras:
         fragment = ""  # type: Optional[str]
         parsed_extras = ()
         name, extras = _strip_extras(name_with_extras)
         if extras:
-            parsed_extras = parsed_extras + tuple(parse_extras(extras))
+            parsed_extras = parsed_extras + tuple(parse_extras_str(extras))
         if parsed_dict["fragment"] is not None:
             fragment = "{0}".format(parsed_dict["fragment"])
             if fragment.startswith("egg="):
                 _, _, fragment_part = fragment.partition("=")
                 fragment_name, fragment_extras = _strip_extras(fragment_part)
                 name = name if name else fragment_name
                 if fragment_extras:
-                    parsed_extras = parsed_extras + tuple(parse_extras(fragment_extras))
+                    parsed_extras = parsed_extras + tuple(
+                        parse_extras_str(fragment_extras)
+                    )
                 name_with_extras = "{0}{1}".format(name, extras_to_string(parsed_extras))
         elif (
             parsed_dict.get("path") is not None and "&subdirectory" in parsed_dict["path"]
         ):
             path, fragment = URI.parse_subdirectory(parsed_dict["path"])  # type: ignore
             parsed_dict["path"] = path
         elif ref is not None and "&subdirectory" in ref:
```

### Comparing `requirementslib-2.3.0/src/requirementslib/models/vcs.py` & `requirementslib-2.3.1.dev0/src/requirementslib/models/vcs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,63 @@
 import importlib
 import os
 import sys
+from typing import Any, Optional, Tuple
 
-import attr
 from pip._internal.utils.temp_dir import global_tempdir_manager
 from pip._internal.vcs.versioncontrol import VcsSupport
+from pip._vendor.pyparsing.core import cached_property
+from pydantic import BaseModel, Field
 
-from ..environment import MYPY_RUNNING
+from .common import ReqLibBaseModel
 from .url import URI
 
-if MYPY_RUNNING:
-    from typing import Any, Optional, Tuple
 
+class VCSRepository(ReqLibBaseModel):
+    url: str
+    name: str
+    checkout_directory: str
+    vcs_type: str
+    parsed_url: Optional[URI] = Field(default_factory=None)
+    subdirectory: Optional[str] = None
+    commit_sha: Optional[str] = None
+    ref: Optional[str] = None
+    repo_backend: Any = None
+    clone_log: Optional[str] = None
+    DEFAULT_RUN_ARGS: Optional[Any] = None
+
+    class Config:
+        validate_assignment = True
+        arbitrary_types_allowed = True
+        allow_mutation = True
+        include_private_attributes = True
+        keep_untouched = (cached_property,)
+
+    def __init__(self, **data):
+        super().__init__(**data)
+        self.parsed_url = self.get_parsed_url()
+        self.repo_backend = self.get_repo_backend()
 
-@attr.s(hash=True)
-class VCSRepository(object):
-    DEFAULT_RUN_ARGS = None
-
-    url = attr.ib()  # type: str
-    name = attr.ib()  # type: str
-    checkout_directory = attr.ib()  # type: str
-    vcs_type = attr.ib()  # type: str
-    parsed_url = attr.ib()  # type: URI
-    subdirectory = attr.ib(default=None)  # type: Optional[str]
-    commit_sha = attr.ib(default=None)  # type: Optional[str]
-    ref = attr.ib(default=None)  # type: Optional[str]
-    repo_backend = attr.ib()  # type: Any
-    clone_log = attr.ib(default=None)  # type: Optional[str]
-
-    @parsed_url.default
-    def get_parsed_url(self):
-        # type: () -> URI
+    def get_parsed_url(self) -> URI:
         return URI.parse(self.url)
 
-    @repo_backend.default
     def get_repo_backend(self):
         if self.DEFAULT_RUN_ARGS is None:
             default_run_args = self.monkeypatch_pip()
         else:
             default_run_args = self.DEFAULT_RUN_ARGS
 
         VCS_SUPPORT = VcsSupport()
         backend = VCS_SUPPORT.get_backend(self.vcs_type)
-        # repo = backend(url=self.url)
         if backend.run_command.__func__.__defaults__ != default_run_args:
             backend.run_command.__func__.__defaults__ = default_run_args
         return backend
 
     @property
-    def is_local(self):
-        # type: () -> bool
+    def is_local(self) -> bool:
         url = self.url
         if "+" in url:
             url = url.split("+")[1]
         return url.startswith("file")
 
     def obtain(self, verbosity=1) -> None:
         if os.path.exists(
@@ -62,45 +66,40 @@
             self.repo_backend.unpack(self.checkout_directory)
         elif not os.path.exists(self.checkout_directory):
             self.repo_backend.obtain(self.checkout_directory, self.parsed_url, verbosity)
         else:
             if self.ref:
                 self.checkout_ref(self.ref)
         if not self.commit_sha:
-            self.commit_sha = self.get_commit_hash()
+            self.commit_sha = self.commit_hash
 
-    def checkout_ref(self, ref):
-        # type: (str) -> None
+    def checkout_ref(self, ref: str) -> None:
         rev_opts = self.repo_backend.make_rev_options(ref)
         if not any(
             [
                 self.repo_backend.is_commit_id_equal(self.checkout_directory, ref),
                 self.repo_backend.is_commit_id_equal(self.checkout_directory, rev_opts),
                 self.is_local,
             ]
         ):
             self.update(ref)
 
-    def update(self, ref):
-        # type: (str) -> None
+    def update(self, ref: str) -> None:
         target_ref = self.repo_backend.make_rev_options(ref)
         self.repo_backend.update(self.checkout_directory, self.url, target_ref)
-        self.commit_sha = self.get_commit_hash()
+        self.commit_sha = self.commit_hash
 
-    def get_commit_hash(self, ref=None):
-        # type: (Optional[str]) -> str
-        with global_tempdir_manager():
-            return self.repo_backend.get_revision(self.checkout_directory)
+    @cached_property
+    def commit_hash(self) -> str:
+        return self.repo_backend.get_revision(self.checkout_directory)
 
     @classmethod
-    def monkeypatch_pip(cls):
-        # type: () -> Tuple[Any, ...]
+    def monkeypatch_pip(cls) -> Tuple[Any, ...]:
         target_module = VcsSupport.__module__
         pip_vcs = importlib.import_module(target_module)
         run_command_defaults = pip_vcs.VersionControl.run_command.__func__.__defaults__
-        # set the default to not write stdout, the first option sets this value
         new_defaults = [False] + list(run_command_defaults)[1:]
         new_defaults = tuple(new_defaults)
         pip_vcs.VersionControl.run_command.__func__.__defaults__ = new_defaults
         sys.modules[target_module] = pip_vcs
         cls.DEFAULT_RUN_ARGS = new_defaults
         return new_defaults
```

### Comparing `requirementslib-2.3.0/src/requirementslib/utils.py` & `requirementslib-2.3.1.dev0/src/requirementslib/utils.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.3.0/src/requirementslib.egg-info/PKG-INFO` & `requirementslib-2.3.1.dev0/src/requirementslib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requirementslib
-Version: 2.3.0
+Version: 2.3.1.dev0
 Summary: A tool for converting between pip-style and pipfile requirements.
 Home-page: https://github.com/sarugaku/requirementslib
 Author: Dan Ryan
 Author-email: dan@danryan.co
 Maintainer: Frost Ming
 Maintainer-email: mianghong@gmail.com
 License: MIT
```

### Comparing `requirementslib-2.3.0/src/requirementslib.egg-info/SOURCES.txt` & `requirementslib-2.3.1.dev0/src/requirementslib.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -38,21 +38,20 @@
 src/requirementslib.egg-info/PKG-INFO
 src/requirementslib.egg-info/SOURCES.txt
 src/requirementslib.egg-info/dependency_links.txt
 src/requirementslib.egg-info/requires.txt
 src/requirementslib.egg-info/top_level.txt
 src/requirementslib.egg-info/zip-safe
 src/requirementslib/models/__init__.py
-src/requirementslib/models/cache.py
+src/requirementslib/models/common.py
 src/requirementslib/models/dependencies.py
 src/requirementslib/models/lockfile.py
 src/requirementslib/models/markers.py
 src/requirementslib/models/metadata.py
 src/requirementslib/models/old_pip_utils.py
 src/requirementslib/models/pipfile.py
 src/requirementslib/models/project.py
 src/requirementslib/models/requirements.py
-src/requirementslib/models/resolvers.py
 src/requirementslib/models/setup_info.py
 src/requirementslib/models/url.py
 src/requirementslib/models/utils.py
 src/requirementslib/models/vcs.py
```

