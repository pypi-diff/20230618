# Comparing `tmp/pyisyox-1.0.0a6.tar.gz` & `tmp/pyisyox-1.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyisyox-1.0.0a6.tar", last modified: Mon Mar 20 13:23:03 2023, max compression
+gzip compressed data, was "pyisyox-1.0.0a7.tar", last modified: Sun Jun 18 15:31:50 2023, max compression
```

## Comparing `pyisyox-1.0.0a6.tar` & `pyisyox-1.0.0a7.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:23:03.958238 pyisyox-1.0.0a6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:23:03.954239 pyisyox-1.0.0a6/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/.devcontainer/devcontainer.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      324 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/.devcontainer/postCreate.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:23:03.954239 pyisyox-1.0.0a6/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:23:03.954239 pyisyox-1.0.0a6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/.github/workflows/pythonpublish.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      948 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:23:03.954239 pyisyox-1.0.0a6/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-03-20 13:23:03.958238 pyisyox-1.0.0a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:23:03.954239 pyisyox-1.0.0a6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:23:03.954239 pyisyox-1.0.0a6/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/docs/api/helpers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/docs/constants.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/docs/events.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/docs/library.rst
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:23:03.954239 pyisyox-1.0.0a6/docs/test_cases/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/docs/test_cases/node_battery_only.xml
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/docs/test_cases/parsed_node_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:23:03.954239 pyisyox-1.0.0a6/pyisyox/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1539 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/clock.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4282 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    30753 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:23:03.954239 pyisyox-1.0.0a6/pyisyox/events/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/events/eventreader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/events/router.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/events/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/events/tcpsocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/events/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:23:03.958238 pyisyox-1.0.0a6/pyisyox/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/helpers/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/helpers/entity_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/helpers/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/helpers/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/helpers/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/helpers/timeit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/helpers/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/isy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/logging.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3664 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)    14434 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/node_servers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:23:03.958238 pyisyox-1.0.0a6/pyisyox/nodes/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11880 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/nodes/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2872 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/nodes/folder.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4513 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/nodes/group.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21142 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/nodes/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/nodes/node_events.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7849 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/nodes/nodebase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:23:03.958238 pyisyox-1.0.0a6/pyisyox/programs/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4388 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/programs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/programs/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/programs/program.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:23:03.958238 pyisyox-1.0.0a6/pyisyox/util/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/util/backports.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/util/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:23:03.958238 pyisyox-1.0.0a6/pyisyox/variables/
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyisyox/variables/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:23:03.954239 pyisyox-1.0.0a6/pyisyox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-03-20 13:23:03.000000 pyisyox-1.0.0a6/pyisyox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-03-20 13:23:03.000000 pyisyox-1.0.0a6/pyisyox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 13:23:03.000000 pyisyox-1.0.0a6/pyisyox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 13:23:03.000000 pyisyox-1.0.0a6/pyisyox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-20 13:23:03.000000 pyisyox-1.0.0a6/pyisyox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-20 13:23:03.000000 pyisyox-1.0.0a6/pyisyox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-20 13:23:03.958238 pyisyox-1.0.0a6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1400 2023-03-20 13:22:53.000000 pyisyox-1.0.0a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.624329 pyisyox-1.0.0a7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.616330 pyisyox-1.0.0a7/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/.devcontainer/devcontainer.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      324 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/.devcontainer/postCreate.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.616330 pyisyox-1.0.0a7/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.616330 pyisyox-1.0.0a7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/.github/workflows/pythonpublish.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      948 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.616330 pyisyox-1.0.0a7/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-18 15:31:50.624329 pyisyox-1.0.0a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.616330 pyisyox-1.0.0a7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.620329 pyisyox-1.0.0a7/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/docs/api/helpers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/docs/constants.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/docs/events.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/docs/library.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.620329 pyisyox-1.0.0a7/docs/test_cases/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/docs/test_cases/node_battery_only.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/docs/test_cases/parsed_node_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.620329 pyisyox-1.0.0a7/pyisyox/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1539 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/clock.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4282 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30753 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.620329 pyisyox-1.0.0a7/pyisyox/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/events/eventreader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/events/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/events/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/events/tcpsocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/events/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.620329 pyisyox-1.0.0a7/pyisyox/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/helpers/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/helpers/entity_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/helpers/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/helpers/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/helpers/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/helpers/timeit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/helpers/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/isy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3973 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15768 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/node_servers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.620329 pyisyox-1.0.0a7/pyisyox/nodes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11942 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/nodes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2872 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/nodes/folder.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4513 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/nodes/group.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21160 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/nodes/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/nodes/node_events.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7857 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/nodes/nodebase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.624329 pyisyox-1.0.0a7/pyisyox/programs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4404 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/programs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/programs/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/programs/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.624329 pyisyox-1.0.0a7/pyisyox/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/util/backports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/util/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.624329 pyisyox-1.0.0a7/pyisyox/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/variables/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.620329 pyisyox-1.0.0a7/pyisyox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-18 15:31:49.000000 pyisyox-1.0.0a7/pyisyox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-18 15:31:50.000000 pyisyox-1.0.0a7/pyisyox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 15:31:50.000000 pyisyox-1.0.0a7/pyisyox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 15:31:49.000000 pyisyox-1.0.0a7/pyisyox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-18 15:31:50.000000 pyisyox-1.0.0a7/pyisyox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 15:31:50.000000 pyisyox-1.0.0a7/pyisyox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-18 15:31:50.624329 pyisyox-1.0.0a7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1400 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/setup.py
```

### Comparing `pyisyox-1.0.0a6/.devcontainer/Dockerfile` & `pyisyox-1.0.0a7/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/.devcontainer/devcontainer.json` & `pyisyox-1.0.0a7/.devcontainer/devcontainer.json`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,16 @@
         "esbenp.prettier-vscode",
         "github.vscode-pull-request-github",
         "streetsidesoftware.code-spell-checker",
         "njpwerner.autodocstring",
         "ms-python.black-formatter",
         "ms-python.python",
         "ms-python.flake8",
-        "matangover.mypy"
+        "matangover.mypy",
+        "charliermarsh.ruff"
       ],
       "settings": {
         "python.pythonPath": "/usr/local/bin/python",
         "python.linting.enabled": true,
         "python.linting.pylintEnabled": true,
         "python.formatting.blackPath": "/usr/local/bin/black",
         "python.linting.flake8Path": "/usr/local/bin/flake8",
```

### Comparing `pyisyox-1.0.0a6/.github/workflows/pythonpublish.yml` & `pyisyox-1.0.0a7/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/.gitignore` & `pyisyox-1.0.0a7/.gitignore`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/.pre-commit-config.yaml` & `pyisyox-1.0.0a7/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,27 @@
 repos:
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.257
+    rev: v0.0.272
     hooks:
       - id: ruff
         args:
           - --fix
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
-    hooks:
-      - id: pyupgrade
-        args: [--py37-plus]
-  - repo: https://github.com/PyCQA/autoflake
-    rev: v2.0.2
-    hooks:
-      - id: autoflake
-        args:
-          - --in-place
-          - --remove-all-unused-imports
   - hooks:
       - args: [--safe, --quiet]
         files: ^((pyisyox|examples)/.+)?[^/]+\.py$
         id: black
     repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
   - hooks:
       - id: codespell
         additional_dependencies:
           - tomli
         args: [--toml, pyproject.toml]
     repo: https://github.com/codespell-project/codespell
-    rev: v2.2.4
-  - hooks:
-      - additional_dependencies:
-          - pycodestyle==2.10.0
-          - pyflakes==3.0.1
-          - flake8-docstrings==1.6.0
-          - pydocstyle==6.1.1
-          - flake8-comprehensions==3.10.1
-          - flake8-noqa==1.3.0
-          - mccabe==0.7.0
-        files: ^(pyisyox)/.+\.py$
-        id: flake8
-    repo: https://github.com/pycqa/flake8
-    rev: 6.0.0
+    rev: v2.2.5
 
   - hooks:
       - id: isort
     repo: https://github.com/PyCQA/isort
     rev: 5.12.0
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
@@ -57,19 +32,19 @@
       - id: check-json
         exclude: (.vscode|.devcontainer)
       - id: no-commit-to-branch
         args:
           - --branch=dev
           - --branch=main
   - repo: https://github.com/adrienverge/yamllint.git
-    rev: v1.29.0
+    rev: v1.32.0
     hooks:
       - id: yamllint
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.0-alpha.6
+    rev: v3.0.0-alpha.9-for-vscode
     hooks:
       - id: prettier
 
   - repo: local
     hooks:
       - id: pylint
         name: pylint
```

### Comparing `pyisyox-1.0.0a6/.vscode/settings.json` & `pyisyox-1.0.0a7/.vscode/settings.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'python.linting.flake8Enabled'": 'False'}*

```diff
@@ -28,13 +28,13 @@
     "files.trimTrailingWhitespace": true,
     "python.analysis.autoImportCompletions": true,
     "python.autoComplete.extraPaths": [
         "/workspaces"
     ],
     "python.formatting.provider": "black",
     "python.linting.enabled": true,
-    "python.linting.flake8Enabled": true,
+    "python.linting.flake8Enabled": false,
     "python.linting.mypyEnabled": true,
     "python.linting.pycodestyleEnabled": false,
     "python.linting.pydocstyleEnabled": true,
     "python.linting.pylintEnabled": true
 }
```

### Comparing `pyisyox-1.0.0a6/.yamllint` & `pyisyox-1.0.0a7/.yamllint`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/CHANGELOG.md` & `pyisyox-1.0.0a7/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/LICENSE.txt` & `pyisyox-1.0.0a7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/PKG-INFO` & `pyisyox-1.0.0a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyisyox
-Version: 1.0.0a6
+Version: 1.0.0a7
 Summary: Python module for asynchronous communication with Universal Devices, Inc.'s ISY & IoX controllers.
 Home-page: https://github.com/shbatm/pyisyox
 Author: shbatm
 Author-email: Ryan Kraus <automicus@gmail.com>, shbatm <support@shbatm.com>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/shbatm/pyisyox
 Project-URL: Homepage, https://github.com/shbatm/pyisyox
```

### Comparing `pyisyox-1.0.0a6/README.md` & `pyisyox-1.0.0a7/README.md`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/docs/Makefile` & `pyisyox-1.0.0a7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/docs/conf.py` & `pyisyox-1.0.0a7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/docs/events.rst` & `pyisyox-1.0.0a7/docs/events.rst`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/docs/index.rst` & `pyisyox-1.0.0a7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/docs/library.rst` & `pyisyox-1.0.0a7/docs/library.rst`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/docs/make.bat` & `pyisyox-1.0.0a7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/docs/quickstart.rst` & `pyisyox-1.0.0a7/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/docs/test_cases/node_battery_only.xml` & `pyisyox-1.0.0a7/docs/test_cases/node_battery_only.xml`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/docs/test_cases/parsed_node_info.json` & `pyisyox-1.0.0a7/docs/test_cases/parsed_node_info.json`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/mypy.ini` & `pyisyox-1.0.0a7/mypy.ini`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/pyisyox/__init__.py` & `pyisyox-1.0.0a7/pyisyox/__init__.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/pyisyox/__main__.py` & `pyisyox-1.0.0a7/pyisyox/__main__.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/pyisyox/clock.py` & `pyisyox-1.0.0a7/pyisyox/clock.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/pyisyox/configuration.py` & `pyisyox-1.0.0a7/pyisyox/configuration.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/pyisyox/connection.py` & `pyisyox-1.0.0a7/pyisyox/connection.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/pyisyox/constants.py` & `pyisyox-1.0.0a7/pyisyox/constants.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/pyisyox/events/eventreader.py` & `pyisyox-1.0.0a7/pyisyox/events/eventreader.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/pyisyox/events/router.py` & `pyisyox-1.0.0a7/pyisyox/events/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         # A wild stream id appears!
         if (sid := xml_dict.get("sid")) and self._stream_id == "":
             self._stream_id = sid
             self.stream.update_stream_id(sid)
             return
         if event := xml_dict.get("event", {}):
             try:
-                self.route_message(EventData(**event))
+                self.route_message(EventData.from_dict(event))
             except (KeyError, ValueError, NameError):
                 _LOGGER.error("Could not validate event", exc_info=True)
 
     def route_message(self, event: EventData) -> None:
         """Route a received message from the event stream.
 
         https://www.universal-devices.com/docs/production/The+ISY994+Developer+Cookbook.pdf
```

### Comparing `pyisyox-1.0.0a6/pyisyox/events/strings.py` & `pyisyox-1.0.0a7/pyisyox/events/strings.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/pyisyox/events/tcpsocket.py` & `pyisyox-1.0.0a7/pyisyox/events/tcpsocket.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,18 +194,18 @@
                 msg = self._create_message(strings.RESUB_MSG)
                 self.write(msg)
             self._subscribed = True
 
     def unsubscribe(self) -> None:
         """Unsubscribe from the Event Stream."""
         if self._subscribed and self._connected:
-            msg = self._create_message(strings.UNSUB_MSG)
             try:
+                msg = self._create_message(strings.UNSUB_MSG)
                 self.write(msg)
-            except OSError as ex:
+            except (OSError, KeyError) as ex:
                 _LOGGER.error(
                     "PyISYoX encountered a socket error while writing unsubscribe message to the socket: %s.",
                     ex,
                 )
             self._subscribed = False
             self.disconnect()
```

### Comparing `pyisyox-1.0.0a6/pyisyox/events/websocket.py` & `pyisyox-1.0.0a7/pyisyox/events/websocket.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/pyisyox/exceptions.py` & `pyisyox-1.0.0a7/pyisyox/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/pyisyox/helpers/__init__.py` & `pyisyox-1.0.0a7/pyisyox/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/pyisyox/helpers/entity.py` & `pyisyox-1.0.0a7/pyisyox/helpers/entity.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/pyisyox/helpers/entity_platform.py` & `pyisyox-1.0.0a7/pyisyox/helpers/entity_platform.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/pyisyox/helpers/events.py` & `pyisyox-1.0.0a7/pyisyox/helpers/events.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/pyisyox/helpers/session.py` & `pyisyox-1.0.0a7/pyisyox/helpers/session.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/pyisyox/helpers/timeit.py` & `pyisyox-1.0.0a7/pyisyox/helpers/timeit.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/pyisyox/helpers/xml.py` & `pyisyox-1.0.0a7/pyisyox/helpers/xml.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,14 +58,17 @@
     elif key == "_value":  # Make CData text an integer
         key = TAG_VALUE
         with suppress(ValueError):
             value = int(cast(str, value))
     elif key == ATTR_FLAG:
         with suppress(ValueError):
             value = int(cast(str, value))
+    elif key == "step":
+        with suppress(ValueError):
+            value = int(cast(str, value))
     # Convert known dates
     if (key.endswith("_time") or key == "ts") and value is not None:
         with suppress(ValueError):
             value = parser.parse(cast(str, value))
 
     return key, value
```

### Comparing `pyisyox-1.0.0a6/pyisyox/isy.py` & `pyisyox-1.0.0a7/pyisyox/isy.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/pyisyox/logging.py` & `pyisyox-1.0.0a7/pyisyox/logging.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/pyisyox/networking.py` & `pyisyox-1.0.0a7/pyisyox/networking.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ISY Network Resources Module."""
 from __future__ import annotations
 
 from dataclasses import dataclass, field
+import inspect
 from typing import TYPE_CHECKING, Any
 
 from pyisyox.constants import TAG_ID, TAG_NAME, URL_NETWORK, URL_RESOURCES, Protocol
 from pyisyox.helpers.entity import Entity
 from pyisyox.helpers.entity_platform import EntityPlatform
 from pyisyox.helpers.events import EventEmitter
 from pyisyox.helpers.models import EntityDetail
@@ -17,14 +18,21 @@
 PLATFORM = "networking"
 
 
 @dataclass
 class NetworkCommandDetail(EntityDetail):
     """Dataclass to hold entity detail info."""
 
+    @classmethod
+    def from_dict(cls: type[NetworkCommandDetail], props: dict) -> NetworkCommandDetail:
+        """Create a dataclass from a dictionary."""
+        return cls(
+            **{k: v for k, v in props.items() if k in inspect.signature(cls).parameters}
+        )
+
     control_info: dict[str, str | bool] = field(default_factory=dict)
     id: str = ""
     is_modified: bool = False
     name: str = ""
 
 
 class NetworkResources(EntityPlatform):
@@ -36,30 +44,30 @@
         Iterate over self.values()
         """
         super().__init__(isy=isy, platform_name=PLATFORM)
         self.url = self.isy.conn.compile_url([URL_NETWORK, URL_RESOURCES])
 
     def parse(self, xml_dict: dict[str, Any]) -> None:
         """Parse the results from the ISY."""
-        if not (net_config := xml_dict["net_config"]) or not (
-            features := net_config["net_rule"]
+        if not (net_config := xml_dict.get("net_config")) or not (
+            features := net_config.get("net_rule")
         ):
             return
         for feature in features:
             self.parse_entity(feature)
 
         _LOGGER.info("Loaded network resources commands")
 
     def parse_entity(self, feature: dict[str, Any]) -> None:
         """Parse a single value and add it to the platform."""
         try:
             address = feature[TAG_ID]
             name = feature[TAG_NAME]
             _LOGGER.debug("Parsing %s: %s (%s)", PLATFORM, name, address)
-            detail = NetworkCommandDetail(**feature)
+            detail = NetworkCommandDetail.from_dict(feature)
             entity = NetworkCommand(self, address, name, detail)
             self.add_or_update_entity(address, name, entity)
         except (TypeError, KeyError, ValueError) as exc:
             _LOGGER.exception("Error loading %s: %s", PLATFORM, exc)
 
     async def update_threaded(self, interval: float) -> None:
         """Continually update the class until it is told to stop.
```

### Comparing `pyisyox-1.0.0a6/pyisyox/node_servers.py` & `pyisyox-1.0.0a7/pyisyox/node_servers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ISY Node Server Information."""
 from __future__ import annotations
 
 import asyncio
 from dataclasses import InitVar, asdict, dataclass, field
+import inspect
 import json
 import re
 from typing import TYPE_CHECKING, Any
 
 from pyisyox.constants import ATTR_ID, DEFAULT_DIR, TAG_NAME, UOM_INDEX, URL_PROFILE_NS
 from pyisyox.helpers.xml import parse_xml
 from pyisyox.logging import _LOGGER
@@ -41,38 +42,60 @@
 URL_NS_ALL = "0"
 
 
 @dataclass
 class EditorRange:
     """Node Server Editor Range definition."""
 
+    @classmethod
+    def from_dict(cls, props: dict) -> EditorRange:
+        """Create a dataclass from a dictionary."""
+        return cls(
+            **{k: v for k, v in props.items() if k in inspect.signature(cls).parameters}
+        )
+
     uom: str = ""
     min: str = ""
     max: str = ""
+    step: int = 0
     precision: int = 0
     subset: str = ""
     nls: str = ""
 
 
 @dataclass
 class NodeEditor:
     """Node Server Editor definition."""
 
+    @classmethod
+    def from_dict(cls, props: dict) -> NodeEditor:
+        """Create a dataclass from a dictionary."""
+        return cls(
+            **{k: v for k, v in props.items() if k in inspect.signature(cls).parameters}
+        )
+
     editor_id: str = ""
     # Ranges are a dict with UoM as the key
     ranges: dict[str, EditorRange] = field(default_factory=dict)
     nls: str = ""
     slot: str = ""
     values: dict[int, str] = field(default_factory=dict)
 
 
 @dataclass
 class NodeServerConnection:
     """Node Server Connection details."""
 
+    @classmethod
+    def from_dict(cls, props: dict) -> NodeServerConnection:
+        """Create a dataclass from a dictionary."""
+        return cls(
+            **{k: v for k, v in props.items() if k in inspect.signature(cls).parameters}
+        )
+
     profile: str = ""
     type_: str = ""
     enabled: bool = False
     name: str = ""
     ssl: bool = False
     sni: bool = False
     port: str = ""
@@ -88,45 +111,56 @@
         return f"{protocol}{self.ip}:{self.port}"
 
 
 @dataclass
 class NodeDef:
     """Node Server Node Definition parsed from the ISY/IoX."""
 
+    @classmethod
+    def from_dict(cls, props: dict) -> NodeDef:
+        """Create a dataclass from a dictionary."""
+        return cls(
+            **{k: v for k, v in props.items() if k in inspect.signature(cls).parameters}
+        )
+
     sts: InitVar[dict[str, list | dict]]
-    cmds: InitVar[dict[str, Any]]
+    cmds: InitVar[dict[str, Any]] | None
     id: str = ""
     node_type: str = ""
     name: str = ""
     nls: str = ""
     slot: str = ""
     editors: Any = ""
     statuses: dict[str, str] = field(init=False, default_factory=dict)
     status_names: dict[str, str] = field(default_factory=dict)
     status_editors: dict[str, NodeEditor] = field(default_factory=dict)
     sends: dict[str, Any] = field(init=False, default_factory=dict)
     accepts: dict[str, Any] = field(init=False, default_factory=dict)
 
-    def __post_init__(self, sts: dict[str, list | dict], cmds: dict[str, Any]) -> None:
+    def __post_init__(
+        self, sts: dict[str, list | dict], cmds: dict[str, Any] | None
+    ) -> None:
         """Post-process node server definition."""
         statuses = {}
         if sts:
             if isinstance(st_list := sts[ATTR_ST], dict):
                 st_list = [st_list]
             for st in st_list:
                 statuses.update({st[ATTR_ID]: st[ATTR_EDITOR]})
         self.statuses = statuses
 
-        if cmds_sends := cmds[ATTR_SENDS]:
-            if isinstance((cmd_list := cmds_sends[ATTR_CMD]), dict):
+        if cmds is None:
+            return
+        if cmds_sends := cmds.get(ATTR_SENDS):
+            if isinstance((cmd_list := cmds_sends.get(ATTR_CMD)), dict):
                 cmd_list = [cmd_list]
             self.sends = {i[ATTR_ID]: i for i in cmd_list}
 
-        if cmds_accepts := cmds[ATTR_ACCEPTS]:
-            if isinstance((cmd_list := cmds_accepts[ATTR_CMD]), dict):
+        if cmds_accepts := cmds.get(ATTR_ACCEPTS):
+            if isinstance((cmd_list := cmds_accepts.get(ATTR_CMD)), dict):
                 cmd_list = [cmd_list]
             self.accepts = {i[ATTR_ID]: i for i in cmd_list}
 
 
 class NodeServers:
     """ISY NodeServers class object.
 
@@ -200,15 +234,15 @@
             self.parse_connection(connection)
 
         _LOGGER.debug("Updated node server connection info")
 
     def parse_connection(self, conn: dict) -> None:
         """Parse the node server connection files from the ISY."""
         try:
-            self._connections.append(NodeServerConnection(**conn))
+            self._connections.append(NodeServerConnection.from_dict(conn))
         except (ValueError, KeyError, NameError) as exc:
             _LOGGER.error("Could not parse node server connection: %s", exc)
             return
 
     async def get_node_server_profiles(self) -> None:
         """Retrieve the node server definition files from the ISY."""
         result = await self.isy.conn.request(
@@ -312,16 +346,21 @@
             nls_lookup: dict = {}
             nls_list = [
                 line
                 for line in file_content.split("\n")
                 if not line.startswith("#") and line != ""
             ]
             if nls_list:
-                nls_lookup = dict(re.split(r"\s?=\s?", line) for line in nls_list)
-                self._node_server_nls[slot] = nls_lookup
+                try:
+                    nls_lookup = dict(re.split(r"\s+=\s+", line) for line in nls_list)
+                    self._node_server_nls[slot] = nls_lookup
+                except ValueError:
+                    _LOGGER.error(
+                        "Error parsing language file for node server slot %s, invalid format"
+                    )
 
             if self.isy.args and self.isy.args.file:
                 filename = "-".join(path.split("/")[-2:]).replace(".txt", ".yaml")
                 await self.isy.loop.run_in_executor(
                     None,
                     write_to_file,
                     nls_lookup,
@@ -332,30 +371,30 @@
         _LOGGER.warning(
             "Unknown file for slot %s: %s", slot, "/".join(path.split("/")[-2:])
         )
 
     def parse_node_server_defs(self, slot: str, node_def: dict) -> None:
         """Retrieve and parse the node server definitions."""
         try:
-            self._node_server_node_definitions[slot][node_def[ATTR_ID]] = NodeDef(
-                **node_def
-            )
+            self._node_server_node_definitions[slot][
+                node_def[ATTR_ID]
+            ] = NodeDef.from_dict(node_def)
 
         except (ValueError, KeyError, NameError) as exc:
-            _LOGGER.error("Could not parse node server connection: %s", exc)
+            _LOGGER.error("Could not parse node server definition: %s", exc)
             return
 
     def parse_node_server_editor(self, slot: str, editor: dict) -> None:
         """Retrieve and parse the node server definitions."""
         editor_id = editor[ATTR_ID]
         if isinstance((ranges := editor[ATTR_RANGE]), dict):
             ranges = [ranges]
         editor_ranges = {}
         for rng in ranges:
-            editor_ranges[rng["uom"]] = EditorRange(**rng)
+            editor_ranges[rng["uom"]] = EditorRange.from_dict(rng)
 
         self._node_server_node_editors[slot][editor_id] = NodeEditor(
             editor_id=editor_id,
             ranges=editor_ranges,
             slot=slot,
         )
 
@@ -371,15 +410,15 @@
                 return
 
             for editor in editors.values():
                 if (index_range := editor.ranges.get(UOM_INDEX)) and index_range.nls:
                     editor.values = {
                         int(k.replace(f"{index_range.nls}-", "")): v
                         for k, v in nls.items()
-                        if k.startswith(index_range.nls)
+                        if k.startswith(f"{index_range.nls}-")
                     }
 
             if not (node_defs := self._node_server_node_definitions.get(slot)):
                 return
             for node_def in node_defs.values():
                 if (name_key := f"ND-{node_def.id}-NAME") in nls:
                     node_def.name = nls[name_key]
```

### Comparing `pyisyox-1.0.0a6/pyisyox/nodes/__init__.py` & `pyisyox-1.0.0a7/pyisyox/nodes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,17 @@
 
     def parse_folder_entity(self, feature: dict[str, Any]) -> None:
         """Parse a single folder and add to the platform."""
         try:
             address = feature[TAG_ADDRESS]
             name = feature[TAG_NAME]
             _LOGGER.log(LOG_VERBOSE, "Parsing %s: %s (%s)", PLATFORM, name, address)
-            entity = NodeFolder(self, address, name, NodeFolderDetail(**feature))
+            entity = NodeFolder(
+                self, address, name, NodeFolderDetail.from_dict(feature)
+            )
             self.add_or_update_entity(address, name, entity)
         except (TypeError, KeyError, ValueError) as exc:
             _LOGGER.exception("Error loading %s: %s", PLATFORM, exc)
 
     def parse_node_entity(self, feature: dict[str, Any]) -> None:
         """Parse a single node and add to the platform."""
         try:
@@ -129,29 +131,29 @@
                 if (
                     isinstance(family, dict)
                     and family[TAG_ADDRESS] == NodeFamily.NODESERVER
                 ):
                     feature["node_server"] = family.get("instance", "")
                 feature["protocol"] = self.get_protocol_from_family(family)
 
-            entity = Node(self, address, name, NodeDetail(**feature))
+            entity = Node(self, address, name, NodeDetail.from_dict(feature))
             self.add_or_update_entity(address, name, entity)
         except (TypeError, KeyError, ValueError) as exc:
             _LOGGER.exception("Error loading %s: %s", PLATFORM, exc)
 
     def parse_group_entity(self, feature: dict[str, Any]) -> None:
         """Parse a single group and add to the platform."""
         try:
             address = feature[TAG_ADDRESS]
             name = feature[TAG_NAME]
             _LOGGER.log(LOG_VERBOSE, "Parsing %s: %s (%s)", PLATFORM, name, address)
             if (flag := feature["flag"]) & NodeFlag.ROOT:
                 _LOGGER.debug("Skipping root group flag=%s %s", flag, address)
                 return
-            entity = Group(self, address, name, GroupDetail(**feature))
+            entity = Group(self, address, name, GroupDetail.from_dict(feature))
             self.add_or_update_entity(address, name, entity)
         except (TypeError, KeyError, ValueError) as exc:
             _LOGGER.exception("Error loading %s: %s", PLATFORM, exc)
 
     def get_protocol_from_family(self, family: str | dict[str, str] | None) -> str:
         """Identify protocol from family type."""
         if family is None:
@@ -222,15 +224,15 @@
                 self.parse_node_properties(prop, entity)
 
         except (TypeError, KeyError, ValueError) as exc:
             _LOGGER.exception("Error loading node status (%s): %s", address, exc)
 
     def parse_node_properties(self, prop: dict[str, Any], entity: Node) -> None:
         """Parse the node node property from the ISY."""
-        result = NodeProperty(**prop)
+        result = NodeProperty.from_dict(prop)
         if result.control == PROP_STATUS:
             entity.update_state(result)
         if result.control == PROP_BATTERY_LEVEL and not entity.state_set:
             # Use BATLVL as state if no ST given.
             entity.is_battery_node = True
             entity.update_state(result)
         elif result.control == PROP_RAMP_RATE and result.value:
```

### Comparing `pyisyox-1.0.0a6/pyisyox/nodes/folder.py` & `pyisyox-1.0.0a7/pyisyox/nodes/folder.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/pyisyox/nodes/group.py` & `pyisyox-1.0.0a7/pyisyox/nodes/group.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/pyisyox/nodes/node.py` & `pyisyox-1.0.0a7/pyisyox/nodes/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     rsp: dict | None = None
     tx: str = ""
     rx: str = ""
 
     def __post_init__(self) -> None:
         """Post-initialization of Node detail dataclass."""
         if self.devtype:
-            self.zwave_props = ZWaveProperties(**self.devtype)
+            self.zwave_props = ZWaveProperties.from_dict(self.devtype)
 
 
 class Node(NodeBase, Entity[NodeDetail, StatusT]):
     """This class handles ISY nodes."""
 
     _parent_node: str | None
     control_events: EventEmitter
@@ -116,15 +116,15 @@
         self._parent_node = detail.pnode if detail.pnode != address else None
         self._protocol = detail.protocol
         self._enabled = detail.enabled
         self.control_events = EventEmitter()
         if detail.property and PROP_STATUS in detail.property:
             self.state_set = True
             self._is_battery_node = False
-            self.update_state(NodeProperty(**detail.property))
+            self.update_state(NodeProperty.from_dict(detail.property))
 
     @property
     def formatted(self) -> str:
         """Return the formatted value with units, if provided."""
         return self._formatted
 
     @property
@@ -156,42 +156,42 @@
         Check ISYv4 UOM, then Insteon and Z-Wave Types for dimmable types.
         """
         dimmable = (
             "%" in str(self._uom)
             or (
                 self._protocol == Protocol.INSTEON
                 and self.type_
-                and any({self.type_.startswith(t) for t in INSTEON_TYPE_DIMMABLE})
+                and any(self.type_.startswith(t) for t in INSTEON_TYPE_DIMMABLE)
                 and self.address.endswith(INSTEON_SUBNODE_DIMMABLE)
             )
             or (
                 self._protocol == Protocol.ZWAVE
                 and self.zwave_props is not None
                 and self.zwave_props.category in ZWAVE_CAT_DIMMABLE
             )
         )
         return dimmable
 
     @property
     def is_lock(self) -> bool:
         """Determine if this device is a door lock type."""
         return (
-            self.type_ and any({self.type_.startswith(t) for t in INSTEON_TYPE_LOCK})
+            self.type_ and any(self.type_.startswith(t) for t in INSTEON_TYPE_LOCK)
         ) or (
             self.protocol == Protocol.ZWAVE
             and self.zwave_props is not None
             and self.zwave_props.category in ZWAVE_CAT_LOCK
         )
 
     @property
     def is_thermostat(self) -> bool:
         """Determine if this device is a thermostat/climate control device."""
         return (
             self.type_
-            and any({self.type_.startswith(t) for t in INSTEON_TYPE_THERMOSTAT})
+            and any(self.type_.startswith(t) for t in INSTEON_TYPE_THERMOSTAT)
         ) or (
             self._protocol == Protocol.ZWAVE
             and self.zwave_props is not None
             and self.zwave_props.category in ZWAVE_CAT_THERMOSTAT
         )
 
     @property
@@ -328,15 +328,15 @@
             return None
 
         parameter_dict: dict[str, Any] = parse_xml(parameter_xml)
         if not (config := parameter_dict[TAG_CONFIG]):
             _LOGGER.warning("Error fetching parameter from ISY")
             return None
 
-        result = ZWaveParameter(**config)
+        result = ZWaveParameter.from_dict(config)
 
         # Add/update the aux_properties to include the parameter.
         node_prop = NodeProperty(
             control=f"{PROP_ZWAVE_PREFIX}{parameter}",
             value=cast(int, result.value),
             uom=f"{PROP_ZWAVE_PREFIX}{result.size}",
             address=self.address,
```

### Comparing `pyisyox-1.0.0a6/pyisyox/nodes/node_events.py` & `pyisyox-1.0.0a7/pyisyox/nodes/node_events.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/pyisyox/nodes/nodebase.py` & `pyisyox-1.0.0a7/pyisyox/nodes/nodebase.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
             return
 
         notes_dict: dict[str, Any] = parse_xml(notes_xml)
 
         if not (notes := notes_dict.get("node_properties")):
             return
 
-        self.notes = NodeNotes(**cast(dict, notes))
+        self.notes = NodeNotes.from_dict(cast(dict, notes))
 
     async def send_cmd(
         self,
         cmd: str,
         val: str | int | float | None = None,
         uom: str | None = None,
         query: dict[str, str] | None = None,
```

### Comparing `pyisyox-1.0.0a6/pyisyox/programs/__init__.py` & `pyisyox-1.0.0a7/pyisyox/programs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,17 +72,17 @@
         """Parse a single value and add it to the platform."""
         try:
             address = feature["id"]
             name = feature["name"]
             _LOGGER.log(LOG_VERBOSE, "Parsing %s: %s (%s)", PLATFORM, name, address)
 
             if feature[TAG_FOLDER]:
-                entity = Folder(self, address, name, FolderDetail(**feature))
+                entity = Folder(self, address, name, FolderDetail.from_dict(feature))
             else:
-                entity = Program(self, address, name, ProgramDetail(**feature))
+                entity = Program(self, address, name, ProgramDetail.from_dict(feature))
 
             self.add_or_update_entity(address, name, entity)
         except (TypeError, KeyError, ValueError) as exc:
             _LOGGER.exception("Error loading %s: %s", PLATFORM, exc)
 
     def update_received(self, event: EventData) -> None:
         """Update programs from EventStream message.
```

### Comparing `pyisyox-1.0.0a6/pyisyox/programs/folder.py` & `pyisyox-1.0.0a7/pyisyox/programs/folder.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/pyisyox/programs/program.py` & `pyisyox-1.0.0a7/pyisyox/programs/program.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/pyisyox/util/backports.py` & `pyisyox-1.0.0a7/pyisyox/util/backports.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/pyisyox/util/output.py` & `pyisyox-1.0.0a7/pyisyox/util/output.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/pyisyox/variables/__init__.py` & `pyisyox-1.0.0a7/pyisyox/variables/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 
     def parse_entity(self, feature: dict[str, Any]) -> None:
         """Parse a single value and add it to the platform."""
         try:
             address = f"{feature[ATTR_TYPE]}.{feature[ATTR_ID]}"
             name = feature["name"]
             _LOGGER.log(LOG_VERBOSE, "Parsing %s: %s (%s)", PLATFORM, name, address)
-            detail = VariableDetail(**feature)
+            detail = VariableDetail.from_dict(feature)
             entity = Variable(self, address, name, detail)
             self.add_or_update_entity(address, name, entity)
         except (TypeError, KeyError, ValueError) as exc:
             _LOGGER.exception("Error loading %s: %s", PLATFORM, exc)
 
     def update_received(self, event: EventData, init: bool = False) -> None:
         """Process an update received from the event stream."""
```

### Comparing `pyisyox-1.0.0a6/pyisyox/variables/variable.py` & `pyisyox-1.0.0a7/pyisyox/variables/variable.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/pyisyox.egg-info/PKG-INFO` & `pyisyox-1.0.0a7/pyisyox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyisyox
-Version: 1.0.0a6
+Version: 1.0.0a7
 Summary: Python module for asynchronous communication with Universal Devices, Inc.'s ISY & IoX controllers.
 Home-page: https://github.com/shbatm/pyisyox
 Author: shbatm
 Author-email: Ryan Kraus <automicus@gmail.com>, shbatm <support@shbatm.com>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/shbatm/pyisyox
 Project-URL: Homepage, https://github.com/shbatm/pyisyox
```

### Comparing `pyisyox-1.0.0a6/pyisyox.egg-info/SOURCES.txt` & `pyisyox-1.0.0a7/pyisyox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a6/pyproject.toml` & `pyisyox-1.0.0a7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -214,17 +214,14 @@
     "E501",  # line too long
     "E731",  # do not assign a lambda expression, use a def
 ]
 
 [tool.ruff.flake8-pytest-style]
 fixture-parentheses = false
 
-[tool.ruff.pyupgrade]
-keep-runtime-typing = true
-
 [tool.ruff.per-file-ignores]
 # Match Case syntax not yet supported by ruff
 "pyisyox/events/router.py" = ["E999"]
 
 # Allow for main entry & scripts to write to stdout
 "pyisyox/__main__.py" = ["T201"]
```

### Comparing `pyisyox-1.0.0a6/setup.py` & `pyisyox-1.0.0a7/setup.py`

 * *Files identical despite different names*

