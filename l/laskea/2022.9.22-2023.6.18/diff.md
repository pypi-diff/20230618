# Comparing `tmp/laskea-2022.9.22.tar.gz` & `tmp/laskea-2023.6.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laskea-2022.9.22.tar", last modified: Wed Sep 21 18:38:47 2022, max compression
+gzip compressed data, was "laskea-2023.6.18.tar", last modified: Sun Jun 18 13:22:48 2023, max compression
```

## Comparing `laskea-2022.9.22.tar` & `laskea-2023.6.18.tar`

### file list

```diff
@@ -1,82 +1,29 @@
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-09-21 18:38:47.861630 laskea-2022.9.22/
--rw-r--r--   0 ruth       (501) staff       (20)     1161 2022-04-30 21:02:24.000000 laskea-2022.9.22/.editorconfig
--rw-r--r--   0 ruth       (501) staff       (20)       19 2022-06-18 09:14:29.000000 laskea-2022.9.22/.gitattributes
--rw-r--r--   0 ruth       (501) staff       (20)     1908 2022-07-02 11:55:06.000000 laskea-2022.9.22/.gitignore
--rw-r--r--   0 ruth       (501) staff       (20)     1069 2022-02-26 15:38:11.000000 laskea-2022.9.22/LICENSE
--rw-r--r--   0 ruth       (501) staff       (20)       34 2021-05-12 16:52:51.000000 laskea-2022.9.22/MANIFEST.in
--rw-r--r--   0 ruth       (501) staff       (20)     2277 2022-09-21 17:29:35.000000 laskea-2022.9.22/Makefile
--rw-r--r--   0 ruth       (501) staff       (20)     2662 2022-09-21 18:38:47.861870 laskea-2022.9.22/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     1659 2022-08-15 11:12:22.000000 laskea-2022.9.22/README.md
--rw-r--r--   0 ruth       (501) staff       (20)      379 2022-06-02 14:50:04.000000 laskea-2022.9.22/SECURITY.md
--rw-r--r--   0 ruth       (501) staff       (20)       96 2022-03-12 00:33:38.000000 laskea-2022.9.22/SUPPORT.md
--rw-r--r--   0 ruth       (501) staff       (20)     3960 2022-09-21 18:24:08.000000 laskea-2022.9.22/baseline-bandit.json
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-09-21 18:38:47.833807 laskea-2022.9.22/docs/
--rw-r--r--   0 ruth       (501) staff       (20)     2216 2022-09-21 18:22:48.000000 laskea-2022.9.22/docs/api.md
--rw-r--r--   0 ruth       (501) staff       (20)     5012 2022-09-21 18:34:38.000000 laskea-2022.9.22/docs/changes.md
--rw-r--r--   0 ruth       (501) staff       (20)     1467 2022-08-15 11:12:22.000000 laskea-2022.9.22/docs/index.md
--rw-r--r--   0 ruth       (501) staff       (20)      206 2022-03-07 19:26:08.000000 laskea-2022.9.22/docs/install.md
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-09-21 18:38:47.838081 laskea-2022.9.22/docs/third-party/
--rw-r--r--   0 ruth       (501) staff       (20)    12485 2022-09-21 18:24:25.000000 laskea-2022.9.22/docs/third-party/README.md
--rw-r--r--   0 ruth       (501) staff       (20)    74066 2022-09-21 18:24:19.000000 laskea-2022.9.22/docs/third-party/all-dependency-licenses.json
--rw-r--r--   0 ruth       (501) staff       (20)    26475 2022-09-21 18:24:18.000000 laskea-2022.9.22/docs/third-party/direct-dependency-licenses.json
--rw-r--r--   0 ruth       (501) staff       (20)     1879 2022-09-21 18:24:25.000000 laskea-2022.9.22/docs/third-party/package-dependency-tree.console.txt
--rw-r--r--   0 ruth       (501) staff       (20)     2165 2022-09-21 18:24:20.000000 laskea-2022.9.22/docs/third-party/package-dependency-tree.dot.txt
--rw-r--r--   0 ruth       (501) staff       (20)    10643 2022-09-21 18:24:23.000000 laskea-2022.9.22/docs/third-party/package-dependency-tree.json
--rw-r--r--   0 ruth       (501) staff       (20)    22383 2022-09-21 18:24:22.000000 laskea-2022.9.22/docs/third-party/package-dependency-tree.svg
--rw-r--r--   0 ruth       (501) staff       (20)     7236 2022-09-21 18:30:39.000000 laskea-2022.9.22/docs/usage.md
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-09-21 18:38:47.820125 laskea-2022.9.22/examples/
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-09-21 18:38:47.841465 laskea-2022.9.22/examples/basic/
--rw-r--r--   0 ruth       (501) staff       (20)      759 2022-03-02 19:03:04.000000 laskea-2022.9.22/examples/basic/.laskea.json
--rw-r--r--   0 ruth       (501) staff       (20)     2172 2022-03-02 19:03:04.000000 laskea-2022.9.22/examples/basic/README.md
--rw-r--r--   0 ruth       (501) staff       (20)      200 2022-02-28 19:35:24.000000 laskea-2022.9.22/examples/basic/files.md
--rw-r--r--   0 ruth       (501) staff       (20)      517 2022-06-08 20:57:31.000000 laskea-2022.9.22/examples/basic/grid_table.md
--rw-r--r--   0 ruth       (501) staff       (20)     8032 2022-07-09 13:59:42.000000 laskea-2022.9.22/examples/basic/test-plans-from-local-data.md
--rwxr-xr-x   0 ruth       (501) staff       (20)      240 2022-02-27 12:03:21.000000 laskea-2022.9.22/gen-sbom
--rw-r--r--   0 ruth       (501) staff       (20)     6125 2022-07-10 11:37:15.000000 laskea-2022.9.22/gen_licenses.py
--rw-r--r--   0 ruth       (501) staff       (20)      601 2022-02-27 14:20:26.000000 laskea-2022.9.22/gen_sbom.py
--rw-r--r--   0 ruth       (501) staff       (20)     1109 2022-09-21 16:42:21.000000 laskea-2022.9.22/gen_version.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-09-21 18:38:47.847544 laskea-2022.9.22/laskea/
--rw-r--r--   0 ruth       (501) staff       (20)     3476 2022-09-21 18:37:07.000000 laskea-2022.9.22/laskea/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)      149 2022-07-09 20:48:21.000000 laskea-2022.9.22/laskea/__main__.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-09-21 18:38:47.852806 laskea-2022.9.22/laskea/api/
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-02-26 20:23:00.000000 laskea-2022.9.22/laskea/api/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)     3260 2022-09-21 18:11:48.000000 laskea-2022.9.22/laskea/api/excel.py
--rw-r--r--   0 ruth       (501) staff       (20)    15265 2022-07-10 12:01:48.000000 laskea-2022.9.22/laskea/api/jira.py
--rw-r--r--   0 ruth       (501) staff       (20)     6004 2022-07-09 20:42:31.000000 laskea-2022.9.22/laskea/api/tabulator.py
--rw-r--r--   0 ruth       (501) staff       (20)     4711 2022-07-10 11:40:50.000000 laskea-2022.9.22/laskea/cli.py
--rw-r--r--   0 ruth       (501) staff       (20)    14130 2022-09-21 16:21:07.000000 laskea-2022.9.22/laskea/config.py
--rw-r--r--   0 ruth       (501) staff       (20)     4518 2022-09-21 17:32:13.000000 laskea-2022.9.22/laskea/embed.py
--rw-r--r--   0 ruth       (501) staff       (20)     1950 2022-03-07 18:40:17.000000 laskea-2022.9.22/laskea/env.py
--rw-r--r--   0 ruth       (501) staff       (20)     1325 2022-03-09 16:17:00.000000 laskea-2022.9.22/laskea/laskea.py
--rw-r--r--   0 ruth       (501) staff       (20)      409 2022-03-09 17:40:55.000000 laskea-2022.9.22/laskea.ABOUT
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-09-21 18:38:47.850576 laskea-2022.9.22/laskea.egg-info/
--rw-r--r--   0 ruth       (501) staff       (20)     2662 2022-09-21 18:38:47.000000 laskea-2022.9.22/laskea.egg-info/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     1517 2022-09-21 18:38:47.000000 laskea-2022.9.22/laskea.egg-info/SOURCES.txt
--rw-r--r--   0 ruth       (501) staff       (20)        1 2022-09-21 18:38:47.000000 laskea-2022.9.22/laskea.egg-info/dependency_links.txt
--rw-r--r--   0 ruth       (501) staff       (20)       42 2022-09-21 18:38:47.000000 laskea-2022.9.22/laskea.egg-info/entry_points.txt
--rw-r--r--   0 ruth       (501) staff       (20)      252 2022-09-21 18:38:47.000000 laskea-2022.9.22/laskea.egg-info/requires.txt
--rw-r--r--   0 ruth       (501) staff       (20)        7 2022-09-21 18:38:47.000000 laskea-2022.9.22/laskea.egg-info/top_level.txt
--rw-r--r--   0 ruth       (501) staff       (20)     1300 2022-07-30 16:56:14.000000 laskea-2022.9.22/mkdocs.yml
--rw-r--r--   0 ruth       (501) staff       (20)     2212 2022-09-21 18:35:27.000000 laskea-2022.9.22/pyproject.toml
--rw-r--r--   0 ruth       (501) staff       (20)      160 2022-09-21 16:32:10.000000 laskea-2022.9.22/requirements.txt
--rw-r--r--   0 ruth       (501) staff       (20)     4179 2022-09-21 18:24:17.000000 laskea-2022.9.22/sbom.json
--rw-r--r--   0 ruth       (501) staff       (20)       65 2022-09-21 18:24:17.000000 laskea-2022.9.22/sbom.json.sha256
--rw-r--r--   0 ruth       (501) staff       (20)      157 2022-09-21 18:38:47.862805 laskea-2022.9.22/setup.cfg
--rw-r--r--   0 ruth       (501) staff       (20)       38 2022-02-26 15:38:11.000000 laskea-2022.9.22/setup.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-09-21 18:38:47.858851 laskea-2022.9.22/test/
--rw-r--r--   0 ruth       (501) staff       (20)      130 2022-02-26 15:38:11.000000 laskea-2022.9.22/test/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-02-26 20:22:08.000000 laskea-2022.9.22/test/conftest.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-09-21 18:38:47.820515 laskea-2022.9.22/test/fixtures/
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-09-21 18:38:47.861503 laskea-2022.9.22/test/fixtures/basic/
--rw-r--r--   0 ruth       (501) staff       (20)      751 2022-03-06 04:48:16.000000 laskea-2022.9.22/test/fixtures/basic/dot.laskea.json
--rw-r--r--   0 ruth       (501) staff       (20)        1 2022-02-26 15:38:11.000000 laskea-2022.9.22/test/fixtures/basic/empty.md
--rw-r--r--   0 ruth       (501) staff       (20)      107 2022-02-26 15:38:11.000000 laskea-2022.9.22/test/fixtures/basic/no-code.md
--rw-r--r--   0 ruth       (501) staff       (20)     6481 2022-06-07 19:30:38.000000 laskea-2022.9.22/test/fixtures/basic/p_c_jira.json
--rw-r--r--   0 ruth       (501) staff       (20)      786 2022-09-19 14:55:10.000000 laskea-2022.9.22/test/requirements-dev.txt
--rw-r--r--   0 ruth       (501) staff       (20)      724 2022-09-18 10:26:03.000000 laskea-2022.9.22/test/requirements.txt
--rw-r--r--   0 ruth       (501) staff       (20)     4216 2022-07-09 13:58:22.000000 laskea-2022.9.22/test/test_api.py
--rw-r--r--   0 ruth       (501) staff       (20)     5465 2022-07-09 13:58:34.000000 laskea-2022.9.22/test/test_cfg.py
--rw-r--r--   0 ruth       (501) staff       (20)      646 2022-03-09 16:38:51.000000 laskea-2022.9.22/test/test_cli.py
--rw-r--r--   0 ruth       (501) staff       (20)     7154 2022-03-09 16:42:11.000000 laskea-2022.9.22/test/test_embed.py
--rw-r--r--   0 ruth       (501) staff       (20)      162 2022-03-05 17:53:30.000000 laskea-2022.9.22/test/test_env.py
--rw-r--r--   0 ruth       (501) staff       (20)      679 2022-03-05 17:51:41.000000 laskea-2022.9.22/test/test_laskea.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 13:22:48.607404 laskea-2023.6.18/
+-rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 laskea-2023.6.18/LICENSE
+-rw-r--r--   0 ruth       (501) staff       (20)       34 2021-05-12 16:52:51.000000 laskea-2023.6.18/MANIFEST.in
+-rw-r--r--   0 ruth       (501) staff       (20)     3138 2023-06-18 13:22:48.607265 laskea-2023.6.18/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     2083 2023-03-14 22:26:03.000000 laskea-2023.6.18/README.md
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 13:22:48.602380 laskea-2023.6.18/laskea/
+-rw-r--r--   0 ruth       (501) staff       (20)     3844 2023-06-18 13:20:46.000000 laskea-2023.6.18/laskea/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)      149 2022-07-09 20:48:21.000000 laskea-2023.6.18/laskea/__main__.py
+-rw-r--r--   0 ruth       (501) staff       (20)     8660 2022-11-08 15:35:37.000000 laskea-2023.6.18/laskea/cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)    14211 2022-11-07 22:13:00.000000 laskea-2023.6.18/laskea/config.py
+-rw-r--r--   0 ruth       (501) staff       (20)     5241 2022-11-06 18:21:02.000000 laskea-2023.6.18/laskea/embed.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1950 2022-03-07 18:40:17.000000 laskea-2023.6.18/laskea/env.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1325 2022-03-09 16:17:00.000000 laskea-2023.6.18/laskea/laskea.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 13:22:48.604638 laskea-2023.6.18/laskea.egg-info/
+-rw-r--r--   0 ruth       (501) staff       (20)     3138 2023-06-18 13:22:48.000000 laskea-2023.6.18/laskea.egg-info/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)      449 2023-06-18 13:22:48.000000 laskea-2023.6.18/laskea.egg-info/SOURCES.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        1 2023-06-18 13:22:48.000000 laskea-2023.6.18/laskea.egg-info/dependency_links.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       42 2023-06-18 13:22:48.000000 laskea-2023.6.18/laskea.egg-info/entry_points.txt
+-rw-r--r--   0 ruth       (501) staff       (20)      249 2023-06-18 13:22:48.000000 laskea-2023.6.18/laskea.egg-info/requires.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        7 2023-06-18 13:22:48.000000 laskea-2023.6.18/laskea.egg-info/top_level.txt
+-rw-r--r--   0 ruth       (501) staff       (20)     2865 2023-06-18 13:01:25.000000 laskea-2023.6.18/pyproject.toml
+-rw-r--r--   0 ruth       (501) staff       (20)       38 2023-06-18 13:22:48.607440 laskea-2023.6.18/setup.cfg
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 13:22:48.607091 laskea-2023.6.18/test/
+-rw-r--r--   0 ruth       (501) staff       (20)     5717 2022-11-08 15:35:47.000000 laskea-2023.6.18/test/test_api.py
+-rw-r--r--   0 ruth       (501) staff       (20)     5484 2022-11-03 16:33:55.000000 laskea-2023.6.18/test/test_cfg.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1092 2022-11-08 14:54:36.000000 laskea-2023.6.18/test/test_cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)     8473 2022-11-08 16:29:50.000000 laskea-2023.6.18/test/test_embed.py
+-rw-r--r--   0 ruth       (501) staff       (20)      162 2022-03-05 17:53:30.000000 laskea-2023.6.18/test/test_env.py
+-rw-r--r--   0 ruth       (501) staff       (20)      679 2022-03-05 17:51:41.000000 laskea-2023.6.18/test/test_laskea.py
```

### Comparing `laskea-2022.9.22/LICENSE` & `laskea-2023.6.18/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Stefan Hagen
+Copyright (c) 2023 Stefan Hagen
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `laskea-2022.9.22/PKG-INFO` & `laskea-2023.6.18/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,69 @@
 Metadata-Version: 2.1
 Name: laskea
-Version: 2022.9.22
+Version: 2023.6.18
 Summary: Calculate (Finnish: laskea) some parts.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/laskea
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/laskea
 Project-URL: Documentation, https://codes.dilettant.life/docs/laskea
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/laskea
 Project-URL: Test-Coverage, https://codes.dilettant.life/coverage/laskea
 Keywords: code-generation,developer-tools,markdown,validation,erification
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Laskea
 
 Calculate (Finnish: laskea) some parts.
 
 [License: MIT](https://git.sr.ht/~sthagen/laskea/tree/default/item/LICENSE)
 
-Third party dependencies are documented in the folder [docs/third-party](docs/third-party/README.md).
+Third party dependencies are documented in the folder [docs/third-party](docs/docs/third-party/README.md).
 
 [![version](https://img.shields.io/pypi/v/laskea.svg?style=flat)](https://pypi.python.org/pypi/laskea/)
 [![downloads](https://pepy.tech/badge/laskea/month)](https://pepy.tech/project/laskea)
 [![wheel](https://img.shields.io/pypi/wheel/laskea.svg?style=flat)](https://pypi.python.org/pypi/laskea/)
 [![supported-versions](https://img.shields.io/pypi/pyversions/laskea.svg?style=flat)](https://pypi.python.org/pypi/laskea/)
 [![supported-implementations](https://img.shields.io/pypi/implementation/laskea.svg?style=flat)](https://pypi.python.org/pypi/laskea/)
 
 ## Documentation
 
 User and developer [documentation of laskea](https://codes.dilettant.life/docs/laskea).
 
 ## Bug Tracker
 
-Feature requests and bug reports are best entered in the [todos of laskea](https://todo.sr.ht/~sthagen/laskea).
+Any feature requests or bug reports shall go to the [todos of laskea](https://todo.sr.ht/~sthagen/laskea).
 
 ## Primary Source repository
 
-The primary source of `laskea` lives somewhere on a mountain in Central Switzerland.
-But, we use decentralized version control (git), so any clone can become the source to everyone's benefit, no central only code.
-Anyway, the preferred public clones of `laskea` are:
+The main source of `laskea` is on a mountain in central Switzerland.
+We use distributed version control (git).
+There is no central hub.
+Every clone can become a new source for the benefit of all.
+The preferred public clones of `laskea` are:
 
 * [on codeberg](https://codeberg.org/sthagen/laskea) - a democratic community-driven, non-profit software development platform operated by Codeberg e.V.
 * [at sourcehut](https://git.sr.ht/~sthagen/laskea) - a collection of tools useful for software development.
 
+## Contributions
+
+Please do not submit "pull requests" (I found no way to disable that "feature" on GitHub).
+If you like to share small changes under the repositories license please kindly do so by sending a patchset.
+You can either send such a patchset per email using [git send-email](https://git-send-email.io) or 
+if you are a sourcehut user by selecting "Prepare a patchset" on the summary page of your fork at [sourcehut](https://git.sr.ht/).
+
 ## Status
 
 Production/Stable.
 
 **Note**: The default branch is `default`.
```

### Comparing `laskea-2022.9.22/laskea/__init__.py` & `laskea-2023.6.18/laskea/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,39 @@
 """Calculate (Finnish: laskea) some parts."""
 import os
 
 # [[[fill git_describe()]]]
-__version__ = '2022.9.22+parent.222fc8ca'
-# [[[end]]] (checksum: 06eeb450e70dd9504d5a7b974122631e)
+__version__ = '2023.6.18+parent.e984ef8f'
+# [[[end]]] (checksum: acaf14066cd24e0140e2bfe3687a469c)
 __version_info__ = tuple(
     e if '-' not in e else e.split('-')[0] for part in __version__.split('+') for e in part.split('.') if e != 'parent'
 )
 
 APP_NAME = 'Calculate (Finnish: laskea) some parts.'
 APP_ALIAS = 'laskea'
 APP_ENV = 'LASKEA'
 CACHE_EXPIRY_SECONDS = int(os.getenv(f'{APP_ENV}_CACHE_EXPIRY_SECONDS', '180'))
+REQUESTS_TIMEOUT_SECS = 30
+
+FIELD_SEPARATORS = (
+    CARET := '^',
+    COLON := ':',
+    COMMA := ',',
+    DASH := '-',
+    DOT := '.',
+    PIPE := '|',
+    PLUS := '+',
+    RS := '\x1e',
+    SEMI := ';',
+    SPACE := ' ',
+    TAB := '\t',
+    USCORE := '_',
+)
+FS_SLUG = '$FIELD_SEPARATOR$'
+
 DEBUG = bool(os.getenv(f'{APP_ENV}_DEBUG', ''))
 DRY_RUN = False
 VERBOSE = bool(os.getenv(f'{APP_ENV}_VERBOSE', ''))
 QUIET = False
 STRICT = bool(os.getenv(f'{APP_ENV}_STRICT', ''))
 ENCODING = 'utf-8'
 ENCODING_ERRORS_POLICY = 'ignore'
@@ -74,46 +92,50 @@
 from laskea.api.jira import (  # noqa
     login,
     markdown_heading,
     markdown_list,
     markdown_table,
     parent_children_sections,
     query,
+    separated_values_list,
 )
 from laskea.embed import (  # noqa
     dl,
     h1,
     h2,
     h3,
     h4,
     h5,
     h6,
     kpi_table,
     mbom_table,
     metrics_table,
     ol,
+    svl,
     table,
     test_plans,
     ul,
 )
 
 __all__ = [
+    'REQUESTS_TIMEOUT_SECS',
     'h1',
     'h2',
     'h3',
     'h4',
     'h5',
     'h6',
     'dl',
     'login',
     'markdown_heading',
     'markdown_table',
     'markdown_list',
     'query',
     'ol',
+    'svl',
     'table',
     'ul',
     'kpi_table',
     'mbom_table',
     'metrics_table',
     'parent_children_sections',
     'test_plans',
```

### Comparing `laskea-2022.9.22/laskea/cli.py` & `laskea-2023.6.18/laskea/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         '--strict',
         help='Ouput noisy warnings on console and in the processed document (default is False)',
     ),
     expires: int = typer.Option(
         180,
         '-x',
         '--cache-expiry-seconds',
-        help='Request cache expiry in seconds (default is 180)',
+        help='Request cache expiry in seconds',
     ),
 ) -> int:
     """
     Fill in some parts of the input document.
 
     You can set some options per evironment variables:
 
@@ -162,13 +162,143 @@
     }
     cfg.process(conf, options)
 
     paths = (inp,) if inp else tuple(source)
     return sys.exit(fill.process(command, transaction_mode, paths, options))
 
 
+@app.command('csv')
+def svl_cmd(  # noqa
+    query: str = typer.Argument(''),
+    jql_query: str = typer.Option(
+        '',
+        '-j',
+        '--jql-query',
+        help=(
+            'The query in JQL format.'
+            '\nFor example given a project YES and two issues 123 and 124:'
+            "\n'project = YES and key in (YES-123, YES-124) order by created DESC'"
+        ),
+        metavar='<jql-query>',
+    ),
+    conf: str = typer.Option(
+        '',
+        '-c',
+        '--config',
+        help=f'Path to config file (default is $HOME/{laskea.DEFAULT_CONFIG_NAME})',
+        metavar='<configpath>',
+    ),
+    key_magic: bool = typer.Option(
+        False,
+        '-k',
+        '--key-magic',
+        help='Apply magic to key by replacing with markdown like link (default is False)',
+    ),
+    field_sep: str = typer.Option(
+        laskea.PIPE,
+        '-d',
+        '--delimiter',
+        help=(
+            'Delimiter / field separator'
+            '\nOn output, header and data cell values will have any occurences'
+            '\nof the field separator replaced with the replacement string'
+        ),
+        metavar='<field-separator>',
+    ),
+    replacement: str = typer.Option(
+        laskea.FS_SLUG,
+        '-r',
+        '--replacement',
+        help=(
+            'Replacement string for occurences of FS in text\n'
+            '\nOn output, header and data cell values will have any occurences'
+            '\nof the field separator replaced with the replacement string'
+        ),
+        metavar='<replacement-text>',
+    ),
+    verify: bool = typer.Option(
+        False,
+        '-n',
+        '--dry-run',
+        help='Dry run (default is False)',
+    ),
+    verbose: bool = typer.Option(
+        False,
+        '-v',
+        '--verbose',
+        help='Verbose output (default is False)',
+    ),
+    strict: bool = typer.Option(
+        False,
+        '-s',
+        '--strict',
+        help='Ouput noisy warnings on console and in the processed document (default is False)',
+    ),
+    expires: int = typer.Option(
+        180,
+        '-x',
+        '--cache-expiry-seconds',
+        help='Request cache expiry in seconds',
+    ),
+) -> int:
+    """
+    Export query result as separated values list.
+
+    You can set some options per evironment variables:
+
+    \b
+    * LASKEA_USER='remote-user'
+    * LASKEA_TOKEN='remote-secret'
+    * LASKEA_BASE_URL='https://remote-jira-instance.example.com/'
+    * LASKEA_CACHE_EXPIRY_SECONDS=180
+    * LASKEA_COL_FIELDS: '["Key", "Summary", "Custom Field Name"]'
+    * LASKEA_COL_MAPS='{"key": ["key", "key"], "summary": ["summary", "fields.summary"],
+    "custom field name": ["customfield_123", "fields.customfield_123"]}'
+    * LASKEA_JOIN_STRING=' <br>'
+    * LASKEA_LF_ONLY='AnythingTruthy'
+    * LASKEA_IS_CLOUD='WhenNotConnectingToJiraServerButJiraCloud'
+    * LASKEA_MARKERS='[[[fill ]]] [[[end]]]'
+    * LASKEA_DEBUG='AnythingTruthy'
+    * LASKEA_VERBOSE='AnythingTruthy'
+    * LASKEA_STRICT='AnythingTruthy'
+
+    The quiet option (if given) disables any conflicting verbosity setting.
+    """
+    transaction_mode = 'commit' if not verify else 'dry-run'
+    jql = jql_query.strip()
+    if not jql and query:
+        jql = query
+    if not jql:
+        print('JQL query required.', file=sys.stderr)
+        return sys.exit(2)
+    quiet = True
+    laskea.QUIET = True
+    laskea.DEBUG = False
+    laskea.VERBOSE = False
+    if verbose:
+        laskea.VERBOSE = True
+
+    if strict:
+        laskea.STRICT = True
+
+    if transaction_mode == 'dry-run':
+        laskea.DRY_RUN = True
+
+    requests_cache.install_cache(cache_name='.laskea_cache', backend='sqlite', expire_after=expires)
+    laskea.CACHE_EXPIRY_SECONDS = expires
+    options = {
+        'quiet': quiet,
+        'strict': strict,
+        'verbose': verbose,
+    }
+    if conf:
+        cfg.process(conf, options)
+
+    return sys.exit(laskea.svl(jql, key_magic=key_magic, field_sep=field_sep, replacement=replacement))
+
+
 @app.command('version')
 def app_version() -> None:
     """
     Display the laskea version and exit.
     """
     callback(True)
```

### Comparing `laskea-2022.9.22/laskea/config.py` & `laskea-2023.6.18/laskea/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,15 +370,15 @@
         },
     }
     safe_report_configuration(effective, header)
 
 
 def process(conf: str, options: Mapping[str, bool]) -> None:
     """SPOC."""
-    configuration, cp = discover_configuration(conf)
+    configuration, cp = discover_configuration(conf if isinstance(conf, str) else '')
 
     verbose = bool(options.get('verbose', ''))
     if configuration is not None:
         if laskea.DEBUG or verbose:
             safe_report_configuration(configuration, f'Loaded configuration from {cp}:')
 
         source_of = load_configuration(configuration)
@@ -389,11 +389,12 @@
         if not laskea.QUIET:
             print('Configuration interface combined file, environment, and commandline values!', file=sys.stderr)
 
         create_and_report_effective_configuration(
             f'Effective configuration combining {cp}, environment variables, and defaults:'
         )
 
-    print(
-        f'INFO: Upstream JIRA instance is addressed per {"cloud" if api.BASE_IS_CLOUD else "server"} rules',
-        file=sys.stderr,
-    )
+    if laskea.DEBUG or verbose:
+        print(
+            f'INFO: Upstream JIRA instance is addressed per {"cloud" if api.BASE_IS_CLOUD else "server"} rules',
+            file=sys.stderr,
+        )
```

### Comparing `laskea-2022.9.22/laskea/embed.py` & `laskea-2023.6.18/laskea/embed.py`

 * *Files 12% similar despite different names*

```diff
@@ -53,14 +53,40 @@
 
         print(api.parent_children_sections(DB['handle'], parent_jql, children_jql, parent_type, children_type))
     else:
         print(api.parent_children_sections(DB['handle'], parent_jql, children_jql, parent_type, children_type, data))
 
 
 @no_type_check
+def svl(
+    query_text: str = '',
+    key_magic: bool = False,
+    field_sep: str = laskea.PIPE,
+    replacement: str = laskea.FS_SLUG,
+    data=None,
+) -> None:
+    """Public separated values list interface."""
+    if data is None:
+        if not DB.get('handle', None):
+            DB['handle'] = api.login()
+
+        print(
+            api.separated_values_list(
+                DB['handle'], query_text, key_magic=key_magic, field_sep=field_sep, replacement=replacement
+            )
+        )
+    else:
+        print(
+            api.separated_values_list(
+                DB['handle'], query_text, key_magic=key_magic, field_sep=field_sep, replacement=replacement, data=data
+            )
+        )
+
+
+@no_type_check
 def table(query_text: str = '', data=None) -> None:
     """Public document interface."""
     if data is None:
         if not DB.get('handle', None):
             DB['handle'] = api.login()
 
         print(api.markdown_table(DB['handle'], query_text))
```

### Comparing `laskea-2022.9.22/laskea/env.py` & `laskea-2023.6.18/laskea/env.py`

 * *Files identical despite different names*

### Comparing `laskea-2022.9.22/laskea/laskea.py` & `laskea-2023.6.18/laskea/laskea.py`

 * *Files identical despite different names*

### Comparing `laskea-2022.9.22/laskea.egg-info/PKG-INFO` & `laskea-2023.6.18/laskea.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,69 @@
 Metadata-Version: 2.1
 Name: laskea
-Version: 2022.9.22
+Version: 2023.6.18
 Summary: Calculate (Finnish: laskea) some parts.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/laskea
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/laskea
 Project-URL: Documentation, https://codes.dilettant.life/docs/laskea
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/laskea
 Project-URL: Test-Coverage, https://codes.dilettant.life/coverage/laskea
 Keywords: code-generation,developer-tools,markdown,validation,erification
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Laskea
 
 Calculate (Finnish: laskea) some parts.
 
 [License: MIT](https://git.sr.ht/~sthagen/laskea/tree/default/item/LICENSE)
 
-Third party dependencies are documented in the folder [docs/third-party](docs/third-party/README.md).
+Third party dependencies are documented in the folder [docs/third-party](docs/docs/third-party/README.md).
 
 [![version](https://img.shields.io/pypi/v/laskea.svg?style=flat)](https://pypi.python.org/pypi/laskea/)
 [![downloads](https://pepy.tech/badge/laskea/month)](https://pepy.tech/project/laskea)
 [![wheel](https://img.shields.io/pypi/wheel/laskea.svg?style=flat)](https://pypi.python.org/pypi/laskea/)
 [![supported-versions](https://img.shields.io/pypi/pyversions/laskea.svg?style=flat)](https://pypi.python.org/pypi/laskea/)
 [![supported-implementations](https://img.shields.io/pypi/implementation/laskea.svg?style=flat)](https://pypi.python.org/pypi/laskea/)
 
 ## Documentation
 
 User and developer [documentation of laskea](https://codes.dilettant.life/docs/laskea).
 
 ## Bug Tracker
 
-Feature requests and bug reports are best entered in the [todos of laskea](https://todo.sr.ht/~sthagen/laskea).
+Any feature requests or bug reports shall go to the [todos of laskea](https://todo.sr.ht/~sthagen/laskea).
 
 ## Primary Source repository
 
-The primary source of `laskea` lives somewhere on a mountain in Central Switzerland.
-But, we use decentralized version control (git), so any clone can become the source to everyone's benefit, no central only code.
-Anyway, the preferred public clones of `laskea` are:
+The main source of `laskea` is on a mountain in central Switzerland.
+We use distributed version control (git).
+There is no central hub.
+Every clone can become a new source for the benefit of all.
+The preferred public clones of `laskea` are:
 
 * [on codeberg](https://codeberg.org/sthagen/laskea) - a democratic community-driven, non-profit software development platform operated by Codeberg e.V.
 * [at sourcehut](https://git.sr.ht/~sthagen/laskea) - a collection of tools useful for software development.
 
+## Contributions
+
+Please do not submit "pull requests" (I found no way to disable that "feature" on GitHub).
+If you like to share small changes under the repositories license please kindly do so by sending a patchset.
+You can either send such a patchset per email using [git send-email](https://git-send-email.io) or 
+if you are a sourcehut user by selecting "Prepare a patchset" on the summary page of your fork at [sourcehut](https://git.sr.ht/).
+
 ## Status
 
 Production/Stable.
 
 **Note**: The default branch is `default`.
```

### Comparing `laskea-2022.9.22/pyproject.toml` & `laskea-2023.6.18/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "laskea"
-version = "2022.9.22"
+version = "2023.6.18"
 description = "Calculate (Finnish: laskea) some parts."
 readme = "README.md"
 authors = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 maintainers = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.9",
 ]
 keywords = ["code-generation", "developer-tools", "markdown", "validation", "erification"]
 dependencies = [
-    "atlassian-python-api >= 3.28.1",
+    "atlassian-python-api >= 3.39.0",
     "cogapp >= 3.3.0",
     "defusedxml >= 0.7.1",
     "jmespath >= 1.0.1",
-    "openpyxl >= 3.0.10",
-    "pydantic >= 1.10.2",
-    "requests-cache >= 0.9.6",
-    "scooby >= 0.6.0",
-    "typer >= 0.6.1",
+    "openpyxl >= 3.1.2",
+    "pydantic >= 1.10.9",
+    "requests-cache >= 1.0.1",
+    "scooby >= 0.7.2",
+    "typer >= 0.9.0",
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 
 [project.optional-dependencies]
-dev = ["black", "coverage", "flake8", "hypothesis", "mypy", "pytest", "pytest-cov", "pytest-flake8", "types-jmespath"]
+dev = ["black", "coverage", "hypothesis", "mypy", "pytest", "pytest-cov", "pytest-flake8", "ruff", "types-jmespath"]
 
 [project.urls]
 Homepage = "https://git.sr.ht/~sthagen/laskea"
 Bug-Tracker = "https://todo.sr.ht/~sthagen/laskea"
 Documentation = "https://codes.dilettant.life/docs/laskea"
 Source-Code = "https://git.sr.ht/~sthagen/laskea"
 Test-Coverage = "https://codes.dilettant.life/coverage/laskea"
@@ -44,21 +45,18 @@
 [project.scripts]
 laskea = "laskea.cli:app"
 
 [tool.setuptools.packages.find]
 include = ["laskea"]
 exclude = ["test*"]
 
-[bdist_wheel]
-universal = true
-
 [tool.black]
 line-length = 120
 skip-string-normalization = true
-target-version = ["py38", "py39", "py310"]
+target-version = ["py39", "py310", "py311", "py312"]
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.report]
 precision = 2
 exclude_lines = [
@@ -67,22 +65,61 @@
     "if TYPE_CHECKING:",
     "@overload",
 ]
 omit = [
     "*/__main__.py",
 ]
 
-[tool.isort]
-line_length = 120
-known_first_party = "laskea"
-multi_line_output = 3
-include_trailing_comma = true
-force_grid_wrap = 0
-combine_as_imports = true
+[tool.ruff]
+line-length = 120
+select = ["E", "F", "Q"]
+ignore = []
+exclude = [
+    ".bzr",
+    ".direnv",
+    ".eggs",
+    ".git",
+    ".hg",
+    ".mypy_cache",
+    ".nox",
+    ".pants.d",
+    ".ruff_cache",
+    ".svn",
+    ".tox",
+    ".venv",
+    "__pypackages__",
+    "_build",
+    "buck-out",
+    "build",
+    "dist",
+    "node_modules",
+    "venv",
+]
+dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
+target-version = "py310"
+unfixable = ["F401"]
+
+[tool.ruff.flake8-quotes]
+docstring-quotes = "double"
+inline-quotes = "single"
+
+[tool.ruff.per-file-ignores]
+"__init__.py" = ["E402"]
+
+[tool.ruff.flake8-import-conventions.aliases]
+altair = "alt"
+"matplotlib.pyplot" = "plt"
+numpy = "np"
+pandas = "pd"
+seaborn = "sns"
+
+[tool.ruff.mccabe]
+max-complexity = 42  # default is 10
 
 [tool.mypy]
 strict = true
 implicit_reexport = true
 
 [tool.pytest]
 testpaths = "test"
 filterwarnings = "error"
+
```

### Comparing `laskea-2022.9.22/test/test_api.py` & `laskea-2023.6.18/test/test_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import pathlib
 
 import pytest
 
+import laskea.api.excel as xls
 import laskea.api.jira as impl
 
 URL_FIXTURE = ''
 HEADING_FIXTURE = {
     'rows': [
         {
             'key': 'ABC-42',
@@ -48,14 +49,29 @@
     ]
 }
 D_LIST_PAYLOADS = tuple(
     f'[{row["key"]}]({URL_FIXTURE}/browse/{row["key"]})\n:{row["summary"]}\n' for row in D_LIST_FIXTURE['rows']
 )
 
 P_C_L_FIXTURE_PATH = pathlib.Path('test', 'fixtures', 'basic', 'p_c_jira.json')
+EMPTY_FIXTURE_PATH = pathlib.Path('test', 'fixtures', 'basic', 'empty.md')
+EMPTY_SHA512_HEX = (
+    'cf83e1357eefb8bdf1542850d66d8007d620e4050b5715dc83f4a921d36ce9ce'
+    '47d0d13c5d85f2b0ff8318d2877eec2f63b931bd47417a81a538327af927da3e'
+)
+MBOM_FIXTURE_PATH = pathlib.Path('test', 'fixtures', 'basic', 'mbom.xlsx')
+MBOM_TABLE = f"""\
+<!-- anchor: ('0', '1233333', 'asdasd', '')-->
+| Level | P/N | Item Name | SW Version |
+|:------|:----|:----------|:-----------|
+| 1     | 124 | a a       | 1          |
+| 2     | 123 | b b       | 2          |
+<!-- source: {MBOM_FIXTURE_PATH}-->
+<!-- s-hash: sha512:98f49a212325387c2a800c000f6892879a38cae9fde357cca3de57bfcc18bb28\
+5d34ad81f19fae1df735ec85e8ada40e7f4ae06ffb5bfb4f89bc7592c8d63111-->"""
 
 
 @pytest.mark.parametrize('level', [lv for lv in range(1, 6 + 1)])
 def test_impl_headings(level):
     impl.BASE_URL = URL_FIXTURE
     hd = impl.markdown_heading(impl.Jira(''), jql_text='', column_fields=tuple(), level=level, data=HEADING_FIXTURE)
     token = '#' * level
@@ -67,29 +83,44 @@
     impl.BASE_URL = URL_FIXTURE
     text = impl.markdown_list(impl.Jira(''), jql_text='', column_fields=tuple(), list_type=kind, data=UO_LIST_FIXTURE)
     items = text.strip().split('\n')
     for slot in (0, 1):
         assert items[slot] == f'{marker}{UO_LIST_PAYLOAD_POSTFIXES[slot]}'
 
 
+def test_impl_svl():
+    text = impl.separated_values_list(
+        impl.Jira(''), jql_text='', column_fields=tuple(), field_sep='x', data=D_LIST_FIXTURE
+    )
+    assert text == (
+        'keyxsummary\nABC-42xFirst issue to show off the definition lists\n'
+        'ABC-1001xSecond issue to show off the definition lists\n'
+    )
+
+
+def test_impl_svl_empty():
+    kwargs = dict(jql_text='', column_fields=tuple(), field_sep='x', data={'rows': []})
+    assert impl.separated_values_list(impl.Jira(''), **kwargs) == ''  # type: ignore
+
+
 def test_impl_d_list():
     impl.BASE_URL = URL_FIXTURE
     text = impl.markdown_list(impl.Jira(''), jql_text='', column_fields=tuple(), list_type='dl', data=D_LIST_FIXTURE)
     assert text == '\n'.join(D_LIST_PAYLOADS) + '\n'
 
 
 def test_impl_login_no_user():
     impl.BASE_USER = ''
     message = 'User, Token, and URL are all required for login.'
     with pytest.raises(ValueError, match=message):
         _ = impl.login(url='does-not-help-as-user-is-missing')
 
 
 def test_impl_login_no_token():
-    impl.BASE_TOKEN = ''
+    impl.BASE_PASS = ''
     message = 'User, Token, and URL are all required for login.'
     with pytest.raises(ValueError, match=message):
         _ = impl.login(user='not-relevant-as-token-is-missing')
 
 
 def test_impl_login_no_url():
     impl.BASE_URL = ''
@@ -123,7 +154,15 @@
 
 def test_parent_children_sections():
     with open(P_C_L_FIXTURE_PATH, 'rt', encoding='utf-8') as handle:
         data = json.load(handle)
 
     doc = impl.parent_children_sections(impl.Jira(''), 'parent_jql', 'children_jql', 'Test Plan', 'Test Case', data)
     assert '## First summary' in doc
+
+
+def test_xls_hash_file_empty():
+    assert xls.hash_file(EMPTY_FIXTURE_PATH) == EMPTY_SHA512_HEX
+
+
+def test_xls_mbom_table_basic():
+    assert xls.mbom_table(str(MBOM_FIXTURE_PATH)) == MBOM_TABLE
```

### Comparing `laskea-2022.9.22/test/test_cfg.py` & `laskea-2023.6.18/test/test_cfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,14 @@
 
 
 def test_load_configuration_remote_token(capsys):
     quiet_flag_restore = laskea.DEBUG
     base_markers_restore = laskea.BASE_MARKERS
     laskea.DEBUG = False
     thing = {'remote': {'token': 'leak'}}
-    gnith = {'remote_base_url': 'env', 'remote_token': 'env', 'remote_user': 'env'}
+    gnith = {'is_cloud': 'env', 'remote_base_url': 'env', 'remote_token': 'env', 'remote_user': 'env'}
     assert cfg.load_configuration(configuration=thing) == gnith
     out, err = capsys.readouterr()
     assert not out
     assert not err
     laskea.DEBUG = quiet_flag_restore
     laskea.BASE_MARKERS = base_markers_restore
```

### Comparing `laskea-2022.9.22/test/test_embed.py` & `laskea-2023.6.18/test/test_embed.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import pathlib
+
 import pytest
 
 import laskea
 import laskea.api.jira as impl
 import laskea.embed as emb
 
 URL_FIXTURE = 'https://remote-jira-instance.example.com'
@@ -82,14 +84,25 @@
     '|:---------------------------------------------------------------------|:------------------------------------|',
     '| [ABC-42](https://remote-jira-instance.example.com/browse/ABC-42)     | First issue to show off the tables  |',
     '| [ABC-1001](https://remote-jira-instance.example.com/browse/ABC-1001) | Second issue to show off the tables |',
     '',
     '2 issues',
 )
 
+MBOM_FIXTURE_PATH = pathlib.Path('test', 'fixtures', 'basic', 'mbom.xlsx')
+MBOM_TABLE = f"""\
+<!-- anchor: ('0', '1233333', 'asdasd', '')-->
+| Level | P/N | Item Name | SW Version |
+|:------|:----|:----------|:-----------|
+| 1     | 124 | a a       | 1          |
+| 2     | 123 | b b       | 2          |
+<!-- source: {MBOM_FIXTURE_PATH}-->
+<!-- s-hash: sha512:98f49a212325387c2a800c000f6892879a38cae9fde357cca3de57bfcc18bb28\
+5d34ad81f19fae1df735ec85e8ada40e7f4ae06ffb5bfb4f89bc7592c8d63111-->"""
+
 
 @pytest.mark.parametrize('level', [lv for lv in range(1, 6 + 1)])
 def test_embed_headings(level, capsys):
     impl.BASE_URL = URL_FIXTURE
     hx = [None, emb.h1, emb.h2, emb.h3, emb.h4, emb.h5, emb.h6]
     token = '#' * level
     assert hx[level](query_text='', data=HEADING_FIXTURE) is None
@@ -123,52 +136,68 @@
     impl.BASE_URL = URL_FIXTURE
     strictness = laskea.STRICT
     laskea.STRICT = True
     hx = [None, emb.h1, emb.h2, emb.h3, emb.h4, emb.h5, emb.h6]
     query_text = ''
     assert hx[level](query_text=query_text, data=HEADING_WARN_TOO_FEW_FIXTURE) is None
     out, err = capsys.readouterr()
-    assert not err  # f'WARNING: received 0 results instead of 1 for JQL ({query_text}) and h{level}' in err
-    assert out == f'WARNING: received 0 results instead of 1 for JQL () and h{level}\n'
+    assert f'WARNING: received 0 results instead of 1 for JQL ({query_text}) and h{level}' in err
+    assert f'WARNING: received 0 results instead of 1 for JQL () and h{level}\n' in out
     laskea.STRICT = strictness
 
 
 @pytest.mark.parametrize('level', [lv for lv in range(1, 6 + 1)])
 def test_embed_headings_too_many_strict(level, capsys):
     impl.BASE_URL = URL_FIXTURE
     strictness = laskea.STRICT
     laskea.STRICT = True
     hx = [None, emb.h1, emb.h2, emb.h3, emb.h4, emb.h5, emb.h6]
     query_text = ''
-    # mis_count = HEADING_WARN_TOO_MANY_FIXTURE_COUNT
+    mis_count = HEADING_WARN_TOO_MANY_FIXTURE_COUNT
     assert hx[level](query_text=query_text, data=HEADING_WARN_TOO_MANY_FIXTURE) is None
     out, err = capsys.readouterr()
-    assert not err  # f'WARNING: received {mis_count} results instead of 1 for JQL ({query_text}) and h{level}' in err
+    assert f'WARNING: received {mis_count} results instead of 1 for JQL ({query_text}) and h{level}' in err
     assert out
     laskea.STRICT = strictness
 
 
 def test_embed_table(capsys):
     impl.BASE_URL = URL_FIXTURE
     expected = '\n'.join(TABLE_FIXTURE_PAYLOADS)
     assert emb.table(query_text='', data=TABLE_FIXTURE) is None
     out, err = capsys.readouterr()
     assert not err
     assert out.strip() == expected
 
 
+def test_embed_svl(capsys):
+    expected = 'key|summary\nABC-42|First issue to show off the tables\nABC-1001|Second issue to show off the tables'
+    assert emb.svl(query_text='', data=TABLE_FIXTURE) is None
+    out, err = capsys.readouterr()
+    assert not err
+    assert out.strip() == expected
+
+
+def test_embed_svl_field_sep_substitute(capsys):
+    expected = 'keyusummary\nABC-42uFirst issue to show off the tables\nABC-1001uSecond issue to show off the tables'
+    assert emb.svl(query_text='', field_sep='u', replacement='u', data=TABLE_FIXTURE) is None
+    out, err = capsys.readouterr()
+    assert not err
+    assert out.strip() == expected
+
+
 def test_embed_table_no_result_strict(capsys):
     impl.BASE_URL = URL_FIXTURE
     strictness = laskea.STRICT
     laskea.STRICT = True
     query_text = ''
     expected = f'WARNING: received 0 results for JQL ({query_text}) and table'
     assert emb.table(query_text=query_text, data=HEADING_WARN_TOO_FEW_FIXTURE) is None
     out, err = capsys.readouterr()
-    assert not err  # == 'WARNING: received 0 results for JQL () and table\n'
+    assert 'WARNING: received 0 results for JQL () and table\n' in err
     assert out.strip() == expected
     laskea.STRICT = strictness
 
 
 def test_embed_table_no_result_non_strict(capsys):
     impl.BASE_URL = URL_FIXTURE
     strictness = laskea.STRICT
@@ -204,7 +233,14 @@
     hx = [None, emb.h1, emb.h2, emb.h3, emb.h4, emb.h5, emb.h6]
     query_text = ''
     assert hx[level](query_text=query_text, data=HEADING_WARN_TOO_MANY_FIXTURE) is None
     out, err = capsys.readouterr()
     assert not err
     assert not out.strip()
     laskea.STRICT = strictness
+
+
+def test_embed_mbom_table_basic(capsys):
+    assert emb.mbom_table(str(MBOM_FIXTURE_PATH)) is None
+    out, err = capsys.readouterr()
+    assert not err
+    assert MBOM_TABLE in out
```

### Comparing `laskea-2022.9.22/test/test_laskea.py` & `laskea-2023.6.18/test/test_laskea.py`

 * *Files identical despite different names*

