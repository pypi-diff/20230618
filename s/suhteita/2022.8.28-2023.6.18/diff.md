# Comparing `tmp/suhteita-2022.8.28.tar.gz` & `tmp/suhteita-2023.6.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suhteita-2022.8.28.tar", last modified: Sun Aug 28 20:40:42 2022, max compression
+gzip compressed data, was "suhteita-2023.6.18.tar", last modified: Sun Jun 18 20:32:11 2023, max compression
```

## Comparing `suhteita-2022.8.28.tar` & `suhteita-2023.6.18.tar`

### file list

```diff
@@ -1,82 +1,33 @@
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-28 20:40:42.875452 suhteita-2022.8.28/
--rw-r--r--   0 ruth       (501) staff       (20)     1161 2022-04-30 21:02:24.000000 suhteita-2022.8.28/.editorconfig
--rw-r--r--   0 ruth       (501) staff       (20)       19 2022-06-18 09:14:29.000000 suhteita-2022.8.28/.gitattributes
--rw-r--r--   0 ruth       (501) staff       (20)     1929 2022-08-27 20:57:25.000000 suhteita-2022.8.28/.gitignore
--rw-r--r--   0 ruth       (501) staff       (20)     1069 2022-08-11 18:51:10.000000 suhteita-2022.8.28/LICENSE
--rw-r--r--   0 ruth       (501) staff       (20)       34 2021-05-12 16:52:51.000000 suhteita-2022.8.28/MANIFEST.in
--rw-r--r--   0 ruth       (501) staff       (20)     2087 2022-08-27 16:42:49.000000 suhteita-2022.8.28/Makefile
--rw-r--r--   0 ruth       (501) staff       (20)     3899 2022-08-28 20:40:42.875576 suhteita-2022.8.28/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     1632 2022-08-15 11:14:58.000000 suhteita-2022.8.28/README.md
--rw-r--r--   0 ruth       (501) staff       (20)     4459 2022-08-28 20:36:57.000000 suhteita-2022.8.28/baseline-bandit.json
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-28 20:40:42.854928 suhteita-2022.8.28/docs/
--rw-r--r--   0 ruth       (501) staff       (20)      141 2022-08-22 20:39:32.000000 suhteita-2022.8.28/docs/api.md
--rw-r--r--   0 ruth       (501) staff       (20)     4862 2022-08-28 20:36:48.000000 suhteita-2022.8.28/docs/changes.md
--rw-r--r--   0 ruth       (501) staff       (20)     1451 2022-08-15 11:14:58.000000 suhteita-2022.8.28/docs/index.md
--rw-r--r--   0 ruth       (501) staff       (20)      239 2022-08-11 19:06:50.000000 suhteita-2022.8.28/docs/install.md
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-28 20:40:42.859090 suhteita-2022.8.28/docs/third-party/
--rw-r--r--   0 ruth       (501) staff       (20)     4636 2022-08-28 20:37:15.000000 suhteita-2022.8.28/docs/third-party/README.md
--rw-r--r--   0 ruth       (501) staff       (20)    29494 2022-08-28 20:37:09.000000 suhteita-2022.8.28/docs/third-party/all-dependency-licenses.json
--rw-r--r--   0 ruth       (501) staff       (20)    27537 2022-08-28 20:37:08.000000 suhteita-2022.8.28/docs/third-party/direct-dependency-licenses.json
--rw-r--r--   0 ruth       (501) staff       (20)      940 2022-08-28 20:37:15.000000 suhteita-2022.8.28/docs/third-party/package-dependency-tree.console.txt
--rw-r--r--   0 ruth       (501) staff       (20)     1112 2022-08-28 20:37:10.000000 suhteita-2022.8.28/docs/third-party/package-dependency-tree.dot.txt
--rw-r--r--   0 ruth       (501) staff       (20)     5309 2022-08-28 20:37:13.000000 suhteita-2022.8.28/docs/third-party/package-dependency-tree.json
--rw-r--r--   0 ruth       (501) staff       (20)    11319 2022-08-28 20:37:12.000000 suhteita-2022.8.28/docs/third-party/package-dependency-tree.svg
--rw-r--r--   0 ruth       (501) staff       (20)     1238 2022-08-22 20:39:53.000000 suhteita-2022.8.28/docs/usage.md
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-28 20:40:42.865267 suhteita-2022.8.28/examples/
--rwxr-xr-x   0 ruth       (501) staff       (20)     6332 2022-08-16 20:44:01.000000 suhteita-2022.8.28/examples/analyze.py
--rwxr-xr-x   0 ruth       (501) staff       (20)     5696 2022-08-28 16:32:44.000000 suhteita-2022.8.28/examples/creator.py
--rwxr-xr-x   0 ruth       (501) staff       (20)    10575 2022-08-27 16:48:53.000000 suhteita-2022.8.28/examples/cstrep.py
--rwxr-xr-x   0 ruth       (501) staff       (20)     6098 2022-08-25 21:31:08.000000 suhteita-2022.8.28/examples/extract.py
--rwxr-xr-x   0 ruth       (501) staff       (20)     4302 2022-08-16 05:20:07.000000 suhteita-2022.8.28/examples/parse.py
--rwxr-xr-x   0 ruth       (501) staff       (20)     4188 2022-08-28 16:32:44.000000 suhteita-2022.8.28/examples/ping.py
--rwxr-xr-x   0 ruth       (501) staff       (20)    10527 2022-08-27 16:44:46.000000 suhteita-2022.8.28/examples/pstrep.py
--rwxr-xr-x   0 ruth       (501) staff       (20)     5614 2022-08-16 05:20:15.000000 suhteita-2022.8.28/examples/report.py
--rw-r--r--   0 ruth       (501) staff       (20)     1377 2022-08-28 20:34:07.000000 suhteita-2022.8.28/examples/source_server.robot
--rw-r--r--   0 ruth       (501) staff       (20)    11257 2022-08-27 16:45:40.000000 suhteita-2022.8.28/examples/strep.py
--rwxr-xr-x   0 ruth       (501) staff       (20)     7745 2022-08-27 16:48:10.000000 suhteita-2022.8.28/examples/summarize.py
--rw-r--r--   0 ruth       (501) staff       (20)     1242 2022-08-28 10:39:45.000000 suhteita-2022.8.28/examples/ticket_system.robot
--rwxr-xr-x   0 ruth       (501) staff       (20)      240 2022-02-27 12:03:21.000000 suhteita-2022.8.28/gen-sbom
--rw-r--r--   0 ruth       (501) staff       (20)     5810 2022-07-28 15:18:24.000000 suhteita-2022.8.28/gen_licenses.py
--rw-r--r--   0 ruth       (501) staff       (20)      599 2022-07-28 15:11:55.000000 suhteita-2022.8.28/gen_sbom.py
--rw-r--r--   0 ruth       (501) staff       (20)     1109 2022-08-21 21:41:20.000000 suhteita-2022.8.28/gen_version.py
--rw-r--r--   0 ruth       (501) staff       (20)     1349 2022-08-11 19:43:17.000000 suhteita-2022.8.28/mkdocs.yml
--rw-r--r--   0 ruth       (501) staff       (20)     2233 2022-08-28 20:38:45.000000 suhteita-2022.8.28/pyproject.toml
--rw-r--r--   0 ruth       (501) staff       (20)       81 2022-08-28 08:48:59.000000 suhteita-2022.8.28/requirements.txt
--rw-r--r--   0 ruth       (501) staff       (20)     2806 2022-08-28 20:37:07.000000 suhteita-2022.8.28/sbom.json
--rw-r--r--   0 ruth       (501) staff       (20)       65 2022-08-28 20:37:07.000000 suhteita-2022.8.28/sbom.json.sha256
--rw-r--r--   0 ruth       (501) staff       (20)      157 2022-08-28 20:40:42.876103 suhteita-2022.8.28/setup.cfg
--rw-r--r--   0 ruth       (501) staff       (20)       38 2021-08-15 06:39:14.000000 suhteita-2022.8.28/setup.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-28 20:40:42.867956 suhteita-2022.8.28/suhteita/
--rw-r--r--   0 ruth       (501) staff       (20)     2750 2022-08-28 20:39:35.000000 suhteita-2022.8.28/suhteita/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)      183 2022-08-11 19:10:03.000000 suhteita-2022.8.28/suhteita/__main__.py
--rw-r--r--   0 ruth       (501) staff       (20)     2486 2022-08-27 13:47:38.000000 suhteita-2022.8.28/suhteita/cli.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-28 20:40:42.870402 suhteita-2022.8.28/suhteita/robot/
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-28 20:40:42.871026 suhteita-2022.8.28/suhteita/robot/SourceServerLibrary/
--rw-r--r--   0 ruth       (501) staff       (20)      251 2022-08-28 16:28:01.000000 suhteita-2022.8.28/suhteita/robot/SourceServerLibrary/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)     3499 2022-08-28 20:24:29.000000 suhteita-2022.8.28/suhteita/robot/SourceServerLibrary/source_server_bridge.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-28 20:40:42.871779 suhteita-2022.8.28/suhteita/robot/TicketSystemLibrary/
--rw-r--r--   0 ruth       (501) staff       (20)      251 2022-08-28 16:28:13.000000 suhteita-2022.8.28/suhteita/robot/TicketSystemLibrary/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)     3477 2022-08-28 16:30:56.000000 suhteita-2022.8.28/suhteita/robot/TicketSystemLibrary/ticket_system_bridge.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-08-27 19:38:53.000000 suhteita-2022.8.28/suhteita/robot/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)     1711 2022-08-28 16:35:21.000000 suhteita-2022.8.28/suhteita/source_server_actions.py
--rw-r--r--   0 ruth       (501) staff       (20)     2881 2022-08-27 13:47:46.000000 suhteita-2022.8.28/suhteita/store.py
--rw-r--r--   0 ruth       (501) staff       (20)    14762 2022-08-28 16:32:11.000000 suhteita-2022.8.28/suhteita/suhteita.py
--rw-r--r--   0 ruth       (501) staff       (20)     9679 2022-08-28 16:29:57.000000 suhteita-2022.8.28/suhteita/ticket_system_actions.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-28 20:40:42.870026 suhteita-2022.8.28/suhteita.egg-info/
--rw-r--r--   0 ruth       (501) staff       (20)     3899 2022-08-28 20:40:42.000000 suhteita-2022.8.28/suhteita.egg-info/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     1699 2022-08-28 20:40:42.000000 suhteita-2022.8.28/suhteita.egg-info/SOURCES.txt
--rw-r--r--   0 ruth       (501) staff       (20)        1 2022-08-28 20:40:42.000000 suhteita-2022.8.28/suhteita.egg-info/dependency_links.txt
--rw-r--r--   0 ruth       (501) staff       (20)       47 2022-08-28 20:40:42.000000 suhteita-2022.8.28/suhteita.egg-info/entry_points.txt
--rw-r--r--   0 ruth       (501) staff       (20)      207 2022-08-28 20:40:42.000000 suhteita-2022.8.28/suhteita.egg-info/requires.txt
--rw-r--r--   0 ruth       (501) staff       (20)        9 2022-08-28 20:40:42.000000 suhteita-2022.8.28/suhteita.egg-info/top_level.txt
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-28 20:40:42.875336 suhteita-2022.8.28/test/
--rw-r--r--   0 ruth       (501) staff       (20)      130 2021-08-15 06:39:14.000000 suhteita-2022.8.28/test/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-08-11 19:09:51.000000 suhteita-2022.8.28/test/conftest.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2021-08-15 08:36:18.000000 suhteita-2022.8.28/test/context.py
--rw-r--r--   0 ruth       (501) staff       (20)      767 2022-08-26 20:07:20.000000 suhteita-2022.8.28/test/requirements-dev.txt
--rw-r--r--   0 ruth       (501) staff       (20)      722 2022-08-27 13:12:39.000000 suhteita-2022.8.28/test/requirements.txt
--rw-r--r--   0 ruth       (501) staff       (20)     1161 2022-08-26 22:03:44.000000 suhteita-2022.8.28/test/test_cli.py
--rw-r--r--   0 ruth       (501) staff       (20)     3020 2022-08-28 13:53:08.000000 suhteita-2022.8.28/test/test_robot_ticket_system.py
--rw-r--r--   0 ruth       (501) staff       (20)      582 2022-08-27 14:28:13.000000 suhteita-2022.8.28/test/test_store.py
--rw-r--r--   0 ruth       (501) staff       (20)      731 2022-08-27 14:27:36.000000 suhteita-2022.8.28/test/test_suhteita.py
--rw-r--r--   0 ruth       (501) staff       (20)     8151 2022-08-28 16:31:42.000000 suhteita-2022.8.28/test/test_ticket_system_actions.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 20:32:11.754433 suhteita-2023.6.18/
+-rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 suhteita-2023.6.18/LICENSE
+-rw-r--r--   0 ruth       (501) staff       (20)       34 2021-05-12 16:52:51.000000 suhteita-2023.6.18/MANIFEST.in
+-rw-r--r--   0 ruth       (501) staff       (20)     3221 2023-06-18 20:32:11.754516 suhteita-2023.6.18/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     2149 2023-03-14 22:44:51.000000 suhteita-2023.6.18/README.md
+-rw-r--r--   0 ruth       (501) staff       (20)     2851 2023-06-18 20:16:57.000000 suhteita-2023.6.18/pyproject.toml
+-rw-r--r--   0 ruth       (501) staff       (20)      151 2023-06-18 20:32:11.756672 suhteita-2023.6.18/setup.cfg
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 20:32:11.747381 suhteita-2023.6.18/suhteita/
+-rw-r--r--   0 ruth       (501) staff       (20)     2750 2023-06-18 20:30:37.000000 suhteita-2023.6.18/suhteita/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)      183 2022-08-11 19:10:03.000000 suhteita-2023.6.18/suhteita/__main__.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2486 2022-08-27 13:47:38.000000 suhteita-2023.6.18/suhteita/cli.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 20:32:11.750887 suhteita-2023.6.18/suhteita/robot/
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 20:32:11.751449 suhteita-2023.6.18/suhteita/robot/TicketSystemLibrary/
+-rw-r--r--   0 ruth       (501) staff       (20)      251 2022-08-28 16:28:13.000000 suhteita-2023.6.18/suhteita/robot/TicketSystemLibrary/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3477 2022-08-28 16:30:56.000000 suhteita-2023.6.18/suhteita/robot/TicketSystemLibrary/ticket_system_bridge.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-08-27 19:38:53.000000 suhteita-2023.6.18/suhteita/robot/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1711 2022-08-28 16:35:21.000000 suhteita-2023.6.18/suhteita/source_server_actions.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2881 2022-08-27 13:47:46.000000 suhteita-2023.6.18/suhteita/store.py
+-rw-r--r--   0 ruth       (501) staff       (20)    14762 2022-08-28 16:32:11.000000 suhteita-2023.6.18/suhteita/suhteita.py
+-rw-r--r--   0 ruth       (501) staff       (20)     9679 2022-08-28 16:29:57.000000 suhteita-2023.6.18/suhteita/ticket_system_actions.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 20:32:11.750528 suhteita-2023.6.18/suhteita.egg-info/
+-rw-r--r--   0 ruth       (501) staff       (20)     3221 2023-06-18 20:32:11.000000 suhteita-2023.6.18/suhteita.egg-info/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)      672 2023-06-18 20:32:11.000000 suhteita-2023.6.18/suhteita.egg-info/SOURCES.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        1 2023-06-18 20:32:11.000000 suhteita-2023.6.18/suhteita.egg-info/dependency_links.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       47 2023-06-18 20:32:11.000000 suhteita-2023.6.18/suhteita.egg-info/entry_points.txt
+-rw-r--r--   0 ruth       (501) staff       (20)      203 2023-06-18 20:32:11.000000 suhteita-2023.6.18/suhteita.egg-info/requires.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        9 2023-06-18 20:32:11.000000 suhteita-2023.6.18/suhteita.egg-info/top_level.txt
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 20:32:11.754324 suhteita-2023.6.18/test/
+-rw-r--r--   0 ruth       (501) staff       (20)     1161 2022-08-26 22:03:44.000000 suhteita-2023.6.18/test/test_cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3020 2022-08-28 13:53:08.000000 suhteita-2023.6.18/test/test_robot_ticket_system.py
+-rw-r--r--   0 ruth       (501) staff       (20)      582 2022-08-27 14:28:13.000000 suhteita-2023.6.18/test/test_store.py
+-rw-r--r--   0 ruth       (501) staff       (20)      731 2022-08-27 14:27:36.000000 suhteita-2023.6.18/test/test_suhteita.py
+-rw-r--r--   0 ruth       (501) staff       (20)     8151 2022-08-28 16:31:42.000000 suhteita-2023.6.18/test/test_ticket_system_actions.py
```

### Comparing `suhteita-2022.8.28/LICENSE` & `suhteita-2023.6.18/LICENSE`

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

### Comparing `suhteita-2022.8.28/PKG-INFO` & `suhteita-2023.6.18/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,69 @@
 Metadata-Version: 2.1
 Name: suhteita
-Version: 2022.8.28
+Version: 2023.6.18
 Summary: Relationships (Finnish: suhteita) maintained across distances as load test core.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
-License: MIT License
-        
-        Copyright (c) 2022 Stefan Hagen
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
 Project-URL: Homepage, https://git.sr.ht/~sthagen/suhteita
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/suhteita
 Project-URL: Documentation, https://codes.dilettant.life/docs/suhteita
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/suhteita
 Project-URL: Test-Coverage, https://codes.dilettant.life/coverage/suhteita
 Keywords: developer-tools,validation,verification
 Classifier: Development Status :: 3 - Alpha
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
 
-# suhteita
+# Suhteita
 
 Relationships (Finnish: suhteita) maintained across distances as load test core.
 
 [License: MIT](https://git.sr.ht/~sthagen/suhteita/tree/default/item/LICENSE)
 
+Third party dependencies are documented in the folder [third-party](docs/third-party/README.md).
+
 [![version](https://img.shields.io/pypi/v/suhteita.svg?style=flat)](https://pypi.python.org/pypi/suhteita/)
 [![downloads](https://pepy.tech/badge/suhteita/month)](https://pepy.tech/project/suhteita)
 [![wheel](https://img.shields.io/pypi/wheel/suhteita.svg?style=flat)](https://pypi.python.org/pypi/suhteita/)
 [![supported-versions](https://img.shields.io/pypi/pyversions/suhteita.svg?style=flat)](https://pypi.python.org/pypi/suhteita/)
 [![supported-implementations](https://img.shields.io/pypi/implementation/suhteita.svg?style=flat)](https://pypi.python.org/pypi/suhteita/)
 
 ## Documentation
 
 User and developer [documentation of suhteita](https://codes.dilettant.life/docs/suhteita).
 
 ## Bug Tracker
 
-Feature requests and bug reports are best entered in the [todos of suhteita](https://todo.sr.ht/~sthagen/suhteita).
+Any feature requests or bug reports shall go to the [todos of suhteita](https://todo.sr.ht/~sthagen/suhteita).
 
 ## Primary Source repository
 
-The primary source of `suhteita` lives somewhere on a mountain in Central Switzerland.
-But, we use decentralized version control (git), so any clone can become the source to everyone's benefit, no central only code.
-Anyway, the preferred public clones of `suhteita` are:
+The main source of `suhteita` is on a mountain in central Switzerland.
+We use distributed version control (git).
+There is no central hub.
+Every clone can become a new source for the benefit of all.
+The preferred public clones of `suhteita` are:
 
 * [on codeberg](https://codeberg.org/sthagen/suhteita) - a democratic community-driven, non-profit software development platform operated by Codeberg e.V.
 * [at sourcehut](https://git.sr.ht/~sthagen/suhteita) - a collection of tools useful for software development.
 
+## Contributions
+
+Please do not submit "pull requests" (I found no way to disable that "feature" on GitHub).
+If you like to share small changes under the repositories license please kindly do so by sending a patchset.
+You can either send such a patchset per email using [git send-email](https://git-send-email.io) or 
+if you are a sourcehut user by selecting "Prepare a patchset" on the summary page of your fork at [sourcehut](https://git.sr.ht/).
+
 ## Status
 
 Experimental.
 
 **Note**: The default branch is `default`.
```

### Comparing `suhteita-2022.8.28/pyproject.toml` & `suhteita-2023.6.18/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "suhteita"
-version = "2022.8.28"
+version = "2023.6.18"
 description = "Relationships (Finnish: suhteita) maintained across distances as load test core."
 readme = "README.md"
 authors = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 maintainers = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
-license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.9",
 ]
 keywords = ["developer-tools", "validation", "verification"]
 dependencies = [
-    "atlassian-python-api >= 3.27.0",
+    "atlassian-python-api >= 3.39.0",
     "jmespath >= 1.0.1",
-    "robotframework >= 5.0.1",
-    "wrapt >= 1.14.1",
+    "robotframework >= 6.1",
+    "wrapt >= 1.15.0",
     'tomli; python_version < "3.11"',
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 
 [project.optional-dependencies]
-dev = ["black", "coverage", "flake8", "hypothesis", "mypy", "pytest", "pytest-cov", "pytest-flake8", "types-jmespath"]
+dev = ["black", "coverage", "hypothesis", "mypy", "pytest", "pytest-cov", "pytest-flake8", "ruff", "types-jmespath"]
 
 [project.urls]
 Homepage = "https://git.sr.ht/~sthagen/suhteita"
 Bug-Tracker = "https://todo.sr.ht/~sthagen/suhteita"
 Documentation = "https://codes.dilettant.life/docs/suhteita"
 Source-Code = "https://git.sr.ht/~sthagen/suhteita"
 Test-Coverage = "https://codes.dilettant.life/coverage/suhteita"
@@ -41,21 +41,18 @@
 [project.scripts]
 suhteita = "suhteita.cli:main"
 
 [tool.setuptools.packages.find]
 include = ["suhteita", "suhteita.robot", "suhteita.robot.TicketSystemLibrary"]
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
@@ -64,21 +61,59 @@
     "if TYPE_CHECKING:",
     "@overload",
 ]
 omit = [
     "*/__main__.py",
 ]
 
-[tool.isort]
-line_length = 120
-known_first_party = "suhteita"
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
```

### Comparing `suhteita-2022.8.28/suhteita/__init__.py` & `suhteita-2023.6.18/suhteita/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import pathlib
 import platform
 import secrets
 import uuid
 from typing import Tuple, no_type_check
 
 # [[[fill git_describe()]]]
-__version__ = '2022.8.28+parent.09889aef'
-# [[[end]]] (checksum: da5ccbf710f2439a095cf4a0ac6a98ec)
+__version__ = '2023.6.18+parent.b59b2bfe'
+# [[[end]]] (checksum: 2ff08a325317e78f9992a600ae7274f6)
 __version_info__ = tuple(
     e if '-' not in e else e.split('-')[0] for part in __version__.split('+') for e in part.split('.') if e != 'parent'
 )
 
 APP_ALIAS = 'suhteita'
 APP_ENV = APP_ALIAS.upper()
 DEBUG = os.getenv(f'{APP_ENV}_DEBUG', '')
```

### Comparing `suhteita-2022.8.28/suhteita/cli.py` & `suhteita-2023.6.18/suhteita/cli.py`

 * *Files identical despite different names*

### Comparing `suhteita-2022.8.28/suhteita/robot/SourceServerLibrary/source_server_bridge.py` & `suhteita-2023.6.18/suhteita/robot/TicketSystemLibrary/ticket_system_bridge.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-"""Source server abstraction relaying keywords to API methods of the underlying source server system (Bitbucket)."""
+"""Ticket system abstraction relaying keywords to API methods of the underlying ticket system (JIRA)."""
 import ast
 from typing import List, no_type_check
 
 import jmespath
 import wrapt  # type: ignore
 from robot.api import ContinuableFailure, logger  # type: ignore
 
-from suhteita.source_server_actions import Bitbucket as Source
+from suhteita.ticket_system_actions import Jira as Ticket
 
 
 @no_type_check
 def _string_to_data(string):
     """Parse the string into the underlying data type if successful else return the string."""
     try:
         return ast.literal_eval(str(string).strip())
@@ -24,34 +24,34 @@
     """Transform the string variables to data, relay to function, and return the call result."""
     args = [_string_to_data(arg) for arg in args]
     kwargs = dict((arg_name, _string_to_data(arg)) for arg_name, arg in kwargs.items())
     return function(*args, **kwargs)
 
 
 @no_type_check
-class SourceServerBridge(object):
+class TicketSystemBridge(object):
     """Use the robot framework hybrid API to proxy the calls and support discovery of keywords."""
 
     ROBOT_LIBRARY_SCOPE = 'Global'
-    _source_server = Source
+    _ticket_system = Ticket
     _session = None
 
     def get_keyword_names(self) -> List[str]:
         """Generate the list of keywords from the underlying provider - required hybrid API method."""
-        get_members = self._source_server.__dict__.items
+        get_members = self._ticket_system.__dict__.items
         kws = [name for name, function in get_members() if hasattr(function, '__call__')]
-        kws += ['extract_fields', 'extract_paths', 'extract_project_keys', 'source_session']
+        kws += ['extract_fields', 'extract_paths', 'extract_project_keys', 'ticket_session']
 
-        return list(set([kw for kw in kws if not kw.startswith('delete_') and kw not in ('__init__', 'get_pullrequest')]))
+        return [kw for kw in kws if not kw.startswith('delete_') and kw not in ('__init__', 'get_issue_remotelinks')]
 
     @no_type_check
-    def source_session(self, url=None, username=None, password=None, **kwargs):
+    def ticket_session(self, url=None, username=None, password=None, **kwargs):
         """Login and fetch the session object."""
-        self._session = self._source_server(url=url, username=username, password=password, **kwargs)
-        logger.debug('Connected to source server')
+        self._session = self._ticket_system(url=url, username=username, password=password, **kwargs)
+        logger.debug('Connected to ticket system')
         return self._session
 
     @no_type_check
     @staticmethod
     def extract_fields(data, fields):
         """Extract dictionary fields from data per key value (field name) to reduce the clutter in logs."""
         try:
@@ -74,14 +74,14 @@
         except KeyError as err:
             raise ContinuableFailure(f'Extraction of key field failed for projects (field=={err})')
 
     @no_type_check
     def __getattr__(self, name):
         """Relay the function matching the keyword or the lookup error."""
         func = None
-        if name in self._source_server.__dict__.keys():
-            func = getattr(self._source_server, name)
+        if name in self._ticket_system.__dict__.keys():
+            func = getattr(self._ticket_system, name)
 
         if func:
             return _string_variables_to_data(func)
 
         raise AttributeError(f'Keyword {name} does not exist or has been overridden by this library.')
```

### Comparing `suhteita-2022.8.28/suhteita/source_server_actions.py` & `suhteita-2023.6.18/suhteita/source_server_actions.py`

 * *Files identical despite different names*

### Comparing `suhteita-2022.8.28/suhteita/store.py` & `suhteita-2023.6.18/suhteita/store.py`

 * *Files identical despite different names*

### Comparing `suhteita-2022.8.28/suhteita/suhteita.py` & `suhteita-2023.6.18/suhteita/suhteita.py`

 * *Files identical despite different names*

### Comparing `suhteita-2022.8.28/suhteita/ticket_system_actions.py` & `suhteita-2023.6.18/suhteita/ticket_system_actions.py`

 * *Files identical despite different names*

### Comparing `suhteita-2022.8.28/suhteita.egg-info/PKG-INFO` & `suhteita-2023.6.18/suhteita.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,69 @@
 Metadata-Version: 2.1
 Name: suhteita
-Version: 2022.8.28
+Version: 2023.6.18
 Summary: Relationships (Finnish: suhteita) maintained across distances as load test core.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
-License: MIT License
-        
-        Copyright (c) 2022 Stefan Hagen
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
 Project-URL: Homepage, https://git.sr.ht/~sthagen/suhteita
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/suhteita
 Project-URL: Documentation, https://codes.dilettant.life/docs/suhteita
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/suhteita
 Project-URL: Test-Coverage, https://codes.dilettant.life/coverage/suhteita
 Keywords: developer-tools,validation,verification
 Classifier: Development Status :: 3 - Alpha
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
 
-# suhteita
+# Suhteita
 
 Relationships (Finnish: suhteita) maintained across distances as load test core.
 
 [License: MIT](https://git.sr.ht/~sthagen/suhteita/tree/default/item/LICENSE)
 
+Third party dependencies are documented in the folder [third-party](docs/third-party/README.md).
+
 [![version](https://img.shields.io/pypi/v/suhteita.svg?style=flat)](https://pypi.python.org/pypi/suhteita/)
 [![downloads](https://pepy.tech/badge/suhteita/month)](https://pepy.tech/project/suhteita)
 [![wheel](https://img.shields.io/pypi/wheel/suhteita.svg?style=flat)](https://pypi.python.org/pypi/suhteita/)
 [![supported-versions](https://img.shields.io/pypi/pyversions/suhteita.svg?style=flat)](https://pypi.python.org/pypi/suhteita/)
 [![supported-implementations](https://img.shields.io/pypi/implementation/suhteita.svg?style=flat)](https://pypi.python.org/pypi/suhteita/)
 
 ## Documentation
 
 User and developer [documentation of suhteita](https://codes.dilettant.life/docs/suhteita).
 
 ## Bug Tracker
 
-Feature requests and bug reports are best entered in the [todos of suhteita](https://todo.sr.ht/~sthagen/suhteita).
+Any feature requests or bug reports shall go to the [todos of suhteita](https://todo.sr.ht/~sthagen/suhteita).
 
 ## Primary Source repository
 
-The primary source of `suhteita` lives somewhere on a mountain in Central Switzerland.
-But, we use decentralized version control (git), so any clone can become the source to everyone's benefit, no central only code.
-Anyway, the preferred public clones of `suhteita` are:
+The main source of `suhteita` is on a mountain in central Switzerland.
+We use distributed version control (git).
+There is no central hub.
+Every clone can become a new source for the benefit of all.
+The preferred public clones of `suhteita` are:
 
 * [on codeberg](https://codeberg.org/sthagen/suhteita) - a democratic community-driven, non-profit software development platform operated by Codeberg e.V.
 * [at sourcehut](https://git.sr.ht/~sthagen/suhteita) - a collection of tools useful for software development.
 
+## Contributions
+
+Please do not submit "pull requests" (I found no way to disable that "feature" on GitHub).
+If you like to share small changes under the repositories license please kindly do so by sending a patchset.
+You can either send such a patchset per email using [git send-email](https://git-send-email.io) or 
+if you are a sourcehut user by selecting "Prepare a patchset" on the summary page of your fork at [sourcehut](https://git.sr.ht/).
+
 ## Status
 
 Experimental.
 
 **Note**: The default branch is `default`.
```

### Comparing `suhteita-2022.8.28/test/test_cli.py` & `suhteita-2023.6.18/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `suhteita-2022.8.28/test/test_robot_ticket_system.py` & `suhteita-2023.6.18/test/test_robot_ticket_system.py`

 * *Files identical despite different names*

### Comparing `suhteita-2022.8.28/test/test_store.py` & `suhteita-2023.6.18/test/test_store.py`

 * *Files identical despite different names*

### Comparing `suhteita-2022.8.28/test/test_suhteita.py` & `suhteita-2023.6.18/test/test_suhteita.py`

 * *Files identical despite different names*

### Comparing `suhteita-2022.8.28/test/test_ticket_system_actions.py` & `suhteita-2023.6.18/test/test_ticket_system_actions.py`

 * *Files identical despite different names*

