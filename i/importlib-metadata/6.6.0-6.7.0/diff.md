# Comparing `tmp/importlib_metadata-6.6.0.tar.gz` & `tmp/importlib_metadata-6.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "importlib_metadata-6.6.0.tar", last modified: Sat Apr 22 12:56:52 2023, max compression
+gzip compressed data, was "importlib_metadata-6.7.0.tar", last modified: Sun Jun 18 21:44:24 2023, max compression
```

## Comparing `importlib_metadata-6.6.0.tar` & `importlib_metadata-6.7.0.tar`

### file list

```diff
@@ -1,73 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:52.094148 importlib_metadata-6.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:52.086147 importlib_metadata-6.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:52.086147 importlib_metadata-6.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21158 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-22 12:56:52.094148 importlib_metadata-6.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:52.086147 importlib_metadata-6.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/docs/migration.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13744 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/docs/using.rst
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/exercises.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:52.090148 importlib_metadata-6.6.0/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    29949 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/importlib_metadata/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/importlib_metadata/_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/importlib_metadata/_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/importlib_metadata/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/importlib_metadata/_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/importlib_metadata/_py39compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/importlib_metadata/_text.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/importlib_metadata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:52.090148 importlib_metadata-6.6.0/importlib_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-22 12:56:52.000000 importlib_metadata-6.6.0/importlib_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-22 12:56:52.000000 importlib_metadata-6.6.0/importlib_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 12:56:52.000000 importlib_metadata-6.6.0/importlib_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-22 12:56:52.000000 importlib_metadata-6.6.0/importlib_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-22 12:56:52.000000 importlib_metadata-6.6.0/importlib_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:52.082147 importlib_metadata-6.6.0/prepare/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:52.090148 importlib_metadata-6.6.0/prepare/example/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:52.090148 importlib_metadata-6.6.0/prepare/example/example/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/prepare/example/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/prepare/example/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:52.090148 importlib_metadata-6.6.0/prepare/example2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:52.090148 importlib_metadata-6.6.0/prepare/example2/example2/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/prepare/example2/example2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/prepare/example2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-22 12:56:52.094148 importlib_metadata-6.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:52.094148 importlib_metadata-6.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tests/_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tests/_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:52.094148 importlib_metadata-6.6.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tests/data/example-21.12-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tests/data/example-21.12-py3.6.egg
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tests/data/example2-1.0.0-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tests/py39compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    14024 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tests/test_py39compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tests/test_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:24.622949 importlib_metadata-6.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:24.618949 importlib_metadata-6.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:24.618949 importlib_metadata-6.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21332 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-18 21:44:24.622949 importlib_metadata-6.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:24.618949 importlib_metadata-6.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/docs/migration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13744 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/docs/using.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/exercises.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:24.618949 importlib_metadata-6.7.0/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    30724 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/importlib_metadata/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/importlib_metadata/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/importlib_metadata/_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/importlib_metadata/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/importlib_metadata/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/importlib_metadata/_py39compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/importlib_metadata/_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/importlib_metadata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:24.622949 importlib_metadata-6.7.0/importlib_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-18 21:44:24.000000 importlib_metadata-6.7.0/importlib_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-18 21:44:24.000000 importlib_metadata-6.7.0/importlib_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 21:44:24.000000 importlib_metadata-6.7.0/importlib_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-18 21:44:24.000000 importlib_metadata-6.7.0/importlib_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 21:44:24.000000 importlib_metadata-6.7.0/importlib_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:24.614949 importlib_metadata-6.7.0/prepare/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:24.622949 importlib_metadata-6.7.0/prepare/example/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:24.622949 importlib_metadata-6.7.0/prepare/example/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/prepare/example/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/prepare/example/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:24.622949 importlib_metadata-6.7.0/prepare/example2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:24.622949 importlib_metadata-6.7.0/prepare/example2/example2/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/prepare/example2/example2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/prepare/example2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-18 21:44:24.622949 importlib_metadata-6.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:24.622949 importlib_metadata-6.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tests/_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tests/_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:24.622949 importlib_metadata-6.7.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tests/data/example-21.12-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tests/data/example-21.12-py3.6.egg
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tests/data/example2-1.0.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)    10575 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tests/py39compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15082 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tests/test_py39compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tests/test_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tox.ini
```

### Comparing `importlib_metadata-6.6.0/.github/workflows/main.yml` & `importlib_metadata-6.7.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.6.0/CHANGES.rst` & `importlib_metadata-6.7.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+v6.7.0
+======
+
+* #453: When inferring top-level names that are importable for
+  distributions in ``package_distributions``, now symlinks to
+  other directories are honored.
+
 v6.6.0
 ======
 
 * #449: Expanded type annotations.
 
 v6.5.1
 ======
```

### Comparing `importlib_metadata-6.6.0/LICENSE` & `importlib_metadata-6.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.6.0/PKG-INFO` & `importlib_metadata-6.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: importlib_metadata
-Version: 6.6.0
+Version: 6.7.0
 Summary: Read metadata from Python packages
 Home-page: https://github.com/python/importlib_metadata
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `importlib_metadata-6.6.0/README.rst` & `importlib_metadata-6.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.6.0/conftest.py` & `importlib_metadata-6.7.0/conftest.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.6.0/docs/conf.py` & `importlib_metadata-6.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.6.0/docs/index.rst` & `importlib_metadata-6.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.6.0/docs/migration.rst` & `importlib_metadata-6.7.0/docs/migration.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.6.0/docs/using.rst` & `importlib_metadata-6.7.0/docs/using.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.6.0/exercises.py` & `importlib_metadata-6.7.0/exercises.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.6.0/importlib_metadata/__init__.py` & `importlib_metadata-6.7.0/importlib_metadata/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import pathlib
 import operator
 import textwrap
 import warnings
 import functools
 import itertools
 import posixpath
-import contextlib
 import collections
 
 from . import _adapters, _meta, _py39compat
 from ._collections import FreezableDefaultDict, Pair
 from ._compat import (
     NullFinder,
     StrPath,
@@ -970,18 +969,47 @@
     return dict(pkg_to_dist)
 
 
 def _top_level_declared(dist):
     return (dist.read_text('top_level.txt') or '').split()
 
 
+def _topmost(name: PackagePath) -> Optional[str]:
+    """
+    Return the top-most parent as long as there is a parent.
+    """
+    top, *rest = name.parts
+    return top if rest else None
+
+
+def _get_toplevel_name(name: PackagePath) -> str:
+    """
+    Infer a possibly importable module name from a name presumed on
+    sys.path.
+
+    >>> _get_toplevel_name(PackagePath('foo.py'))
+    'foo'
+    >>> _get_toplevel_name(PackagePath('foo'))
+    'foo'
+    >>> _get_toplevel_name(PackagePath('foo.pyc'))
+    'foo'
+    >>> _get_toplevel_name(PackagePath('foo/__init__.py'))
+    'foo'
+    >>> _get_toplevel_name(PackagePath('foo.pth'))
+    'foo.pth'
+    >>> _get_toplevel_name(PackagePath('foo.dist-info'))
+    'foo.dist-info'
+    """
+    return _topmost(name) or (
+        # python/typeshed#10328
+        inspect.getmodulename(name)  # type: ignore
+        or str(name)
+    )
+
+
 def _top_level_inferred(dist):
-    opt_names = {
-        f.parts[0] if len(f.parts) > 1 else inspect.getmodulename(f)
-        for f in always_iterable(dist.files)
-    }
+    opt_names = set(map(_get_toplevel_name, always_iterable(dist.files)))
 
-    @pass_none
     def importable_name(name):
         return '.' not in name
 
     return filter(importable_name, opt_names)
```

### Comparing `importlib_metadata-6.6.0/importlib_metadata/_adapters.py` & `importlib_metadata-6.7.0/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.6.0/importlib_metadata/_collections.py` & `importlib_metadata-6.7.0/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.6.0/importlib_metadata/_compat.py` & `importlib_metadata-6.7.0/importlib_metadata/_compat.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,22 +52,14 @@
     but may find distributions.
     """
 
     @staticmethod
     def find_spec(*args, **kwargs):
         return None
 
-    # In Python 2, the import system requires finders
-    # to have a find_module() method, but this usage
-    # is deprecated in Python 3 in favor of find_spec().
-    # For the purposes of this finder (i.e. being present
-    # on sys.meta_path but having no other import
-    # system functionality), the two methods are identical.
-    find_module = find_spec
-
 
 def pypy_partial(val):
     """
     Adjust for variable stacklevel on partial under PyPy.
 
     Workaround for #327.
     """
```

### Comparing `importlib_metadata-6.6.0/importlib_metadata/_functools.py` & `importlib_metadata-6.7.0/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.6.0/importlib_metadata/_itertools.py` & `importlib_metadata-6.7.0/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.6.0/importlib_metadata/_meta.py` & `importlib_metadata-6.7.0/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.6.0/importlib_metadata/_py39compat.py` & `importlib_metadata-6.7.0/importlib_metadata/_py39compat.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.6.0/importlib_metadata/_text.py` & `importlib_metadata-6.7.0/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.6.0/importlib_metadata.egg-info/PKG-INFO` & `importlib_metadata-6.7.0/importlib_metadata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: importlib-metadata
-Version: 6.6.0
+Version: 6.7.0
 Summary: Read metadata from Python packages
 Home-page: https://github.com/python/importlib_metadata
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `importlib_metadata-6.6.0/importlib_metadata.egg-info/SOURCES.txt` & `importlib_metadata-6.7.0/importlib_metadata.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 .coveragerc
 .editorconfig
-.flake8
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yaml
 CHANGES.rst
 LICENSE
 README.rst
 conftest.py
```

### Comparing `importlib_metadata-6.6.0/pytest.ini` & `importlib_metadata-6.7.0/pytest.ini`

 * *Files 26% similar despite different names*

```diff
@@ -3,30 +3,25 @@
 addopts=--doctest-modules
 filterwarnings=
 	## upstream
 
 	# Ensure ResourceWarnings are emitted
 	default::ResourceWarning
 
-	# Suppress deprecation warning in flake8
-	ignore:SelectableGroups dict interface is deprecated::flake8
-
 	# shopkeep/pytest-black#55
 	ignore:<class 'pytest_black.BlackItem'> is not using a cooperative constructor:pytest.PytestDeprecationWarning
 	ignore:The \(fspath. py.path.local\) argument to BlackItem is deprecated.:pytest.PytestDeprecationWarning
 	ignore:BlackItem is an Item subclass and should not be a collector:pytest.PytestWarning
 
-	# tholo/pytest-flake8#83
-	ignore:<class 'pytest_flake8.Flake8Item'> is not using a cooperative constructor:pytest.PytestDeprecationWarning
-	ignore:The \(fspath. py.path.local\) argument to Flake8Item is deprecated.:pytest.PytestDeprecationWarning
-	ignore:Flake8Item is an Item subclass and should not be a collector:pytest.PytestWarning
-
 	# shopkeep/pytest-black#67
 	ignore:'encoding' argument not specified::pytest_black
 
 	# realpython/pytest-mypy#152
 	ignore:'encoding' argument not specified::pytest_mypy
 
 	# python/cpython#100750
 	ignore:'encoding' argument not specified::platform
 
+	# pypa/build#615
+	ignore:'encoding' argument not specified::build.env
+
 	## end upstream
```

### Comparing `importlib_metadata-6.6.0/setup.cfg` & `importlib_metadata-6.7.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -28,23 +28,21 @@
 	tests*
 	prepare*
 
 [options.extras_require]
 testing = 
 	pytest >= 6
 	pytest-checkdocs >= 2.4
-	pytest-flake8; \
-	python_version < "3.12"
-	flake8 < 5
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
 	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
 	pytest-enabler >= 1.3
+	pytest-ruff
 	
 	importlib_resources>=1.3; python_version < "3.9"
 	packaging
 	pyfakefs
 	flufl.flake8
 	pytest-perf >= 0.9.2
 docs =
```

### Comparing `importlib_metadata-6.6.0/tests/_path.py` & `importlib_metadata-6.7.0/tests/_path.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,27 @@
-# from jaraco.path 3.5
+# from jaraco.path 3.6
 
 import functools
 import pathlib
 from typing import Dict, Union
 
 try:
     from typing import Protocol, runtime_checkable
 except ImportError:  # pragma: no cover
     # Python 3.7
     from typing_extensions import Protocol, runtime_checkable  # type: ignore
 
 
-FilesSpec = Dict[str, Union[str, bytes, 'FilesSpec']]  # type: ignore
+class Symlink(str):
+    """
+    A string indicating the target of a symlink.
+    """
+
+
+FilesSpec = Dict[str, Union[str, bytes, Symlink, 'FilesSpec']]  # type: ignore
 
 
 @runtime_checkable
 class TreeMaker(Protocol):
     def __truediv__(self, *args, **kwargs):
         ...  # pragma: no cover
 
@@ -24,14 +30,17 @@
 
     def write_text(self, content, **kwargs):
         ...  # pragma: no cover
 
     def write_bytes(self, content):
         ...  # pragma: no cover
 
+    def symlink_to(self, target):
+        ...  # pragma: no cover
+
 
 def _ensure_tree_maker(obj: Union[str, TreeMaker]) -> TreeMaker:
     return obj if isinstance(obj, TreeMaker) else pathlib.Path(obj)  # type: ignore
 
 
 def build(
     spec: FilesSpec,
@@ -47,20 +56,24 @@
     ...     'README.txt': "A README file",
     ...     "foo": {
     ...         "__init__.py": "",
     ...         "bar": {
     ...             "__init__.py": "",
     ...         },
     ...         "baz.py": "# Some code",
-    ...     }
+    ...         "bar.py": Symlink("baz.py"),
+    ...     },
+    ...     "bing": Symlink("foo"),
     ... }
     >>> target = getfixture('tmp_path')
     >>> build(spec, target)
     >>> target.joinpath('foo/baz.py').read_text(encoding='utf-8')
     '# Some code'
+    >>> target.joinpath('bing/bar.py').read_text(encoding='utf-8')
+    '# Some code'
     """
     for name, contents in spec.items():
         create(contents, _ensure_tree_maker(prefix) / name)
 
 
 @functools.singledispatch
 def create(content: Union[str, bytes, FilesSpec], path):
@@ -75,16 +88,16 @@
 
 @create.register
 def _(content: str, path):
     path.write_text(content, encoding='utf-8')
 
 
 @create.register
-def _(content: str, path):
-    path.write_text(content, encoding='utf-8')
+def _(content: Symlink, path):
+    path.symlink_to(content)
 
 
 class Recording:
     """
     A TreeMaker object that records everything that would be written.
 
     >>> r = Recording()
@@ -103,7 +116,10 @@
     def write_text(self, content, **kwargs):
         self.record.append(str(self.loc))
 
     write_bytes = write_text
 
     def mkdir(self, **kwargs):
         return
+
+    def symlink_to(self, target):
+        pass
```

### Comparing `importlib_metadata-6.6.0/tests/data/example-21.12-py3-none-any.whl` & `importlib_metadata-6.7.0/tests/data/example-21.12-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.6.0/tests/data/example-21.12-py3.6.egg` & `importlib_metadata-6.7.0/tests/data/example-21.12-py3.6.egg`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.6.0/tests/data/example2-1.0.0-py3-none-any.whl` & `importlib_metadata-6.7.0/tests/data/example2-1.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.6.0/tests/fixtures.py` & `importlib_metadata-6.7.0/tests/fixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,19 +345,14 @@
 
 
 def DALS(str):
     "Dedent and left-strip"
     return textwrap.dedent(str).lstrip()
 
 
-class NullFinder:
-    def find_module(self, name):
-        pass
-
-
 class ZipFixtures:
     root = 'tests.data'
 
     def _fixture_on_path(self, filename):
         pkg_file = resources.files(self.root).joinpath(filename)
         file = self.resources.enter_context(resources.as_file(pkg_file))
         assert file.name.startswith('example'), file.name
```

### Comparing `importlib_metadata-6.6.0/tests/test_api.py` & `importlib_metadata-6.7.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.6.0/tests/test_integration.py` & `importlib_metadata-6.7.0/tests/test_integration.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,23 @@
+"""
+Test behaviors specific to importlib_metadata.
+
+These tests are excluded downstream in CPython as they
+test functionality only in importlib_metadata or require
+behaviors ('packaging') that aren't available in the
+stdlib.
+"""
+
 import unittest
 import packaging.requirements
 import packaging.version
 
 from . import fixtures
 from importlib_metadata import (
-    MetadataPathFinder,
     _compat,
-    distributions,
     version,
 )
 
 
 class IntegrationTests(fixtures.DistInfoPkg, unittest.TestCase):
     def test_package_spec_installed(self):
         """
@@ -25,43 +32,22 @@
         assert is_installed('distinfo-pkg==1.0')
         assert is_installed('distinfo-pkg>=1.0,<2.0')
         assert not is_installed('distinfo-pkg<1.0')
 
 
 class FinderTests(fixtures.Fixtures, unittest.TestCase):
     def test_finder_without_module(self):
-        class ModuleFreeFinder(fixtures.NullFinder):
+        class ModuleFreeFinder:
             """
             A finder without an __module__ attribute
             """
 
+            def find_module(self, name):
+                pass
+
             def __getattribute__(self, name):
                 if name == '__module__':
                     raise AttributeError(name)
                 return super().__getattribute__(name)
 
         self.fixtures.enter_context(fixtures.install_finder(ModuleFreeFinder()))
         _compat.disable_stdlib_finder()
-
-
-class DistSearch(unittest.TestCase):
-    def test_search_dist_dirs(self):
-        """
-        Pip needs the _search_paths interface to locate
-        distribution metadata dirs. Protect it for PyPA
-        use-cases (only). Ref python/importlib_metadata#111.
-        """
-        res = MetadataPathFinder._search_paths('any-name', [])
-        assert list(res) == []
-
-    def test_interleaved_discovery(self):
-        """
-        When the search is cached, it is
-        possible for searches to be interleaved, so make sure
-        those use-cases are safe.
-
-        Ref #293
-        """
-        dists = distributions()
-        next(dists)
-        version('importlib_metadata')
-        next(dists)
```

### Comparing `importlib_metadata-6.6.0/tests/test_main.py` & `importlib_metadata-6.7.0/tests/test_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import re
 import pickle
 import unittest
 import warnings
 import importlib
 import importlib_metadata
 import contextlib
-import itertools
 import pyfakefs.fake_filesystem_unittest as ffs
 
 from . import fixtures
 from ._context import suppress
+from ._path import Symlink
 from importlib_metadata import (
     Distribution,
     EntryPoint,
     PackageNotFoundError,
     _unique,
     distributions,
     entry_points,
@@ -201,14 +201,28 @@
         assert any(dist.metadata['Name'] == 'sources_fallback-pkg' for dist in dists)
         assert any(dist.metadata['Name'] == 'distinfo-pkg' for dist in dists)
 
     def test_invalid_usage(self):
         with self.assertRaises(ValueError):
             list(distributions(context='something', name='else'))
 
+    def test_interleaved_discovery(self):
+        """
+        Ensure interleaved searches are safe.
+
+        When the search is cached, it is possible for searches to be
+        interleaved, so make sure those use-cases are safe.
+
+        Ref #293
+        """
+        dists = distributions()
+        next(dists)
+        version('egginfo-pkg')
+        next(dists)
+
 
 class DirectoryTest(fixtures.OnSysPath, fixtures.SiteDir, unittest.TestCase):
     def test_egg_info(self):
         # make an `EGG-INFO` directory that's unrelated
         self.site_dir.joinpath('EGG-INFO').mkdir()
         # used to crash with `IsADirectoryError`
         with self.assertRaises(PackageNotFoundError):
@@ -382,14 +396,35 @@
         for i in range(len(suffixes)):
             assert distributions[f'importable-name {i}'] == ['all_distributions']
             assert distributions[f'in_namespace_{i}'] == ['all_distributions']
             assert distributions[f'in_package_{i}'] == ['all_distributions']
 
         assert not any(name.endswith('.dist-info') for name in distributions)
 
+    def test_packages_distributions_symlinked_top_level(self):
+        """
+        Distribution is resolvable from a simple top-level symlink in RECORD.
+        See #452.
+        """
+
+        files: fixtures.FilesSpec = {
+            "symlinked_pkg-1.0.0.dist-info": {
+                "METADATA": """
+                    Name: symlinked-pkg
+                    Version: 1.0.0
+                    """,
+                "RECORD": "symlinked,,\n",
+            },
+            ".symlink.target": {},
+            "symlinked": Symlink(".symlink.target"),
+        }
+
+        fixtures.build_files(files, self.site_dir)
+        assert packages_distributions()['symlinked'] == ['symlinked-pkg']
+
 
 class PackagesDistributionsEggTest(
     fixtures.EggInfoPkg,
     fixtures.EggInfoPkgPipInstalledNoToplevel,
     fixtures.EggInfoPkgPipInstalledNoModules,
     fixtures.EggInfoPkgSourcesFallback,
     unittest.TestCase,
```

### Comparing `importlib_metadata-6.6.0/tests/test_py39compat.py` & `importlib_metadata-6.7.0/tests/test_py39compat.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.6.0/tests/test_zip.py` & `importlib_metadata-6.7.0/tests/test_zip.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.6.0/tox.ini` & `importlib_metadata-6.7.0/tox.ini`

 * *Files identical despite different names*

