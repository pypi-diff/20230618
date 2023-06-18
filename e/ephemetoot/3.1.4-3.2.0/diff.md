# Comparing `tmp/ephemetoot-3.1.4.tar.gz` & `tmp/ephemetoot-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ephemetoot-3.1.4.tar", max compression
+gzip compressed data, was "ephemetoot-3.2.0.tar", last modified: Sun Jun 18 09:27:25 2023, max compression
```

## Comparing `ephemetoot-3.1.4.tar` & `ephemetoot-3.2.0.tar`

### file list

```diff
@@ -1,11 +1,22 @@
--rw-r--r--   0        0        0    32471 2020-04-20 00:45:02.123384 ephemetoot-3.1.4/LICENSE
--rw-r--r--   0        0        0        0 2020-09-26 03:20:29.307070 ephemetoot-3.1.4/ephemetoot/__init__.py
--rw-r--r--   0        0        0     5560 2023-01-15 04:52:46.428084 ephemetoot-3.1.4/ephemetoot/console.py
--rw-r--r--   0        0        0    23266 2021-08-23 05:28:50.882240 ephemetoot-3.1.4/ephemetoot/ephemetoot.py
--rw-r--r--   0        0        0      780 2020-09-26 03:20:29.309416 ephemetoot-3.1.4/ephemetoot/plist.py
--rw-r--r--   0        0        0     1144 2020-09-26 03:33:47.967157 ephemetoot-3.1.4/pypi-readme.md
--rw-r--r--   0        0        0      827 2023-01-15 05:02:21.066990 ephemetoot-3.1.4/pyproject.toml
--rw-r--r--   0        0        0    30126 2021-08-23 22:21:04.388429 ephemetoot-3.1.4/tests/accomplished.jpg
--rw-r--r--   0        0        0    24002 2021-08-23 22:21:04.390099 ephemetoot-3.1.4/tests/test_ephemetoot.py
--rw-r--r--   0        0        0     1995 1970-01-01 00:00:00.000000 ephemetoot-3.1.4/setup.py
--rw-r--r--   0        0        0     2117 1970-01-01 00:00:00.000000 ephemetoot-3.1.4/PKG-INFO
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2023-06-18 09:27:24.998985 ephemetoot-3.2.0/
+-rw-r--r--   0 hugh       (501) staff       (20)    32471 2020-04-20 00:45:02.000000 ephemetoot-3.2.0/LICENSE
+-rw-r--r--   0 hugh       (501) staff       (20)        8 2023-06-18 08:20:59.000000 ephemetoot-3.2.0/MANIFEST.in
+-rw-r--r--   0 hugh       (501) staff       (20)     1684 2023-06-18 09:27:24.997801 ephemetoot-3.2.0/PKG-INFO
+-rw-r--r--   0 hugh       (501) staff       (20)     1933 2023-06-18 08:57:42.000000 ephemetoot-3.2.0/README.md
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2023-06-18 09:27:24.989112 ephemetoot-3.2.0/ephemetoot/
+-rw-r--r--   0 hugh       (501) staff       (20)        0 2020-09-26 03:20:29.000000 ephemetoot-3.2.0/ephemetoot/__init__.py
+-rw-r--r--   0 hugh       (501) staff       (20)     5560 2023-06-18 05:01:12.000000 ephemetoot-3.2.0/ephemetoot/console.py
+-rw-r--r--   0 hugh       (501) staff       (20)    23495 2023-06-18 08:20:59.000000 ephemetoot-3.2.0/ephemetoot/ephemetoot.py
+-rw-r--r--   0 hugh       (501) staff       (20)      780 2020-09-26 03:20:29.000000 ephemetoot-3.2.0/ephemetoot/plist.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2023-06-18 09:27:24.994967 ephemetoot-3.2.0/ephemetoot.egg-info/
+-rw-r--r--   0 hugh       (501) staff       (20)     1684 2023-06-18 09:27:24.000000 ephemetoot-3.2.0/ephemetoot.egg-info/PKG-INFO
+-rw-r--r--   0 hugh       (501) staff       (20)      380 2023-06-18 09:27:24.000000 ephemetoot-3.2.0/ephemetoot.egg-info/SOURCES.txt
+-rw-r--r--   0 hugh       (501) staff       (20)        1 2023-06-18 09:27:24.000000 ephemetoot-3.2.0/ephemetoot.egg-info/dependency_links.txt
+-rw-r--r--   0 hugh       (501) staff       (20)       55 2023-06-18 09:27:24.000000 ephemetoot-3.2.0/ephemetoot.egg-info/entry_points.txt
+-rw-r--r--   0 hugh       (501) staff       (20)       65 2023-06-18 09:27:24.000000 ephemetoot-3.2.0/ephemetoot.egg-info/requires.txt
+-rw-r--r--   0 hugh       (501) staff       (20)       11 2023-06-18 09:27:24.000000 ephemetoot-3.2.0/ephemetoot.egg-info/top_level.txt
+-rw-r--r--   0 hugh       (501) staff       (20)     1127 2023-06-18 08:57:33.000000 ephemetoot-3.2.0/pypi-readme.md
+-rw-r--r--   0 hugh       (501) staff       (20)      885 2023-06-18 08:20:59.000000 ephemetoot-3.2.0/pyproject.toml
+-rw-r--r--   0 hugh       (501) staff       (20)       38 2023-06-18 09:27:24.999325 ephemetoot-3.2.0/setup.cfg
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2023-06-18 09:27:24.995703 ephemetoot-3.2.0/tests/
+-rw-r--r--   0 hugh       (501) staff       (20)    24002 2023-06-18 05:01:12.000000 ephemetoot-3.2.0/tests/test_ephemetoot.py
```

### Comparing `ephemetoot-3.1.4/LICENSE` & `ephemetoot-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ephemetoot-3.1.4/ephemetoot/console.py` & `ephemetoot-3.2.0/ephemetoot/console.py`

 * *Files identical despite different names*

### Comparing `ephemetoot-3.1.4/ephemetoot/ephemetoot.py` & `ephemetoot-3.2.0/ephemetoot/ephemetoot.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,14 +188,15 @@
         conf_token = compulsory_input(tags, "Access token: ", None)
         conf_user = compulsory_input(
             tags, "Username", "(without the '@' - e.g. alice):"
         )
         conf_url = compulsory_input(tags, "Base URL", "(e.g. example.social):")
         conf_days = digit_input(tags, "Days to keep", "(default 365):")
         conf_pinned = yes_no_input(tags, "Keep pinned toots?")
+        conf_boosts_only = yes_no_input(tags, "Only remove boosted toots?")
         conf_keep_toots = optional_input(
             tags, "Toots to keep", "(optional list of IDs separated by commas):"
         )
         conf_keep_hashtags = optional_input(
             tags,
             "Hashtags to keep",
             "(optional list without '#' e.g. mastodon, gardening, cats):",
@@ -215,14 +216,15 @@
 
             configfile.write("-")
             configfile.write("\n  access_token: " + conf_token)
             configfile.write("\n  username: " + conf_user)
             configfile.write("\n  base_url: " + conf_url)
             configfile.write("\n  days_to_keep: " + conf_days)
             configfile.write("\n  keep_pinned: " + conf_pinned)
+            configfile.write("\n  boosts_only: " + conf_boosts_only)
 
             if len(conf_keep_toots) > 0:
                 keep_list = conf_keep_toots.split(",")
                 configfile.write("\n  toots_to_keep:")
                 for toot in keep_list:
                     configfile.write("\n    - " + toot.strip())
 
@@ -420,14 +422,15 @@
     else:
         raise TimeoutError("Gave up after 5 attempts")
 
 
 def process_toot(config, options, mastodon, toot, deleted_count=0):
 
     keep_pinned = "keep_pinned" in config and config["keep_pinned"]
+    boosts_only = "boosts_only" in config and config["boosts_only"]
     toots_to_keep = config["toots_to_keep"] if "toots_to_keep" in config else []
     visibility_to_keep = (
         config["visibility_to_keep"] if "visibility_to_keep" in config else []
     )
     hashtags_to_keep = (
         set(config["hashtags_to_keep"]) if "hashtags_to_keep" in config else set()
     )
@@ -487,15 +490,15 @@
                     # check for --archive-deleted
                     if options.archive_deleted and "id" in toot and "archive" in config:
                         # write toot to archive
                         archive_toot(config, toot)
 
                     mastodon.status_unreblog(toot.reblog)
 
-            else:
+            elif not boosts_only:
                 console_print(
                     "❌ deleting toot " + str(toot.id) + " tooted " + tooted_date(toot),
                     options,
                     False,
                 )
 
                 deleted_count += 1
```

### Comparing `ephemetoot-3.1.4/ephemetoot/plist.py` & `ephemetoot-3.2.0/ephemetoot/plist.py`

 * *Files identical despite different names*

### Comparing `ephemetoot-3.1.4/pypi-readme.md` & `ephemetoot-3.2.0/pypi-readme.md`

 * *Files 14% similar despite different names*

```diff
@@ -17,10 +17,10 @@
 
 Run from the command line with `ephemetoot`.
 
 Run `ephemetoot --help` or read the docs for all options.
 
 ## Contributing
 
-ephemetoot is packaged using `poetry` and tested using `pytest`.
+ephemetoot is now in maintenance mode, and new features will not be considered.
 
-For all bugs, suggestions, pull requests or other contributions, please check the [contributing guide](https://github.com/hughrun/ephemetoot/blob/master/docs/contributing.md).
+For bugs or other contributions, please check the [contributing guide](https://github.com/hughrun/ephemetoot/blob/master/docs/contributing.md).
```

### Comparing `ephemetoot-3.1.4/pyproject.toml` & `ephemetoot-3.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,38 @@
-[tool.poetry]
+[project]
 name = "ephemetoot"
-version = "3.1.4"
+version = "3.2.0"
 description = "A command line tool to delete your old toots"
-authors = ["Hugh Rundle <ephemetoot@hugh.run>"]
-license = "GPL-3.0-or-later"
+requires-python = ">=3.8"
+authors = [
+    {name = "Hugh Rundle", email = "ephemetoot@hugh.run"}
+    ]
+license = { text = "GPL-3.0-or-later"}
 readme = "pypi-readme.md"
-homepage = "https://ephemetoot.hugh.run"
-repository = "https://github.com/hughrun/ephemetoot"
 keywords = ["mastodon", "api", "microblogging"]
 classifiers = [
     "Environment :: Console",
     "Operating System :: OS Independent",
     "Topic :: Communications"
 ]
-include = [
-    "LICENSE",
-    "tests"
+dependencies = [
+    "requests>=2.31.0",
+    "mastodon.py>=1.4.3",
+    "pyyaml>=5.0"
 ]
 
-[tool.poetry.dependencies]
-python = "^3.8"
-requests = "^2.22.0"
-"mastodon.py" = "^1.4.3"
-pyyaml = "^5.0"
+[project.optional-dependencies]
+dev = ["pytest>=6"]
 
-[tool.poetry.dev-dependencies]
-pytest = "^6"
-
-[tool.poetry.scripts]
+[project.scripts]
 ephemetoot = 'ephemetoot.console:main'
 
+[project.urls]
+homepage = "https://ephemetoot.hugh.run"
+repository = "https://github.com/hughrun/ephemetoot"
+
 [build-system]
-requires = ["poetry-core>=1.0.0a5"]
-build-backend = "poetry.core.masonry.api"
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools]
+packages = ["ephemetoot"]
```

### Comparing `ephemetoot-3.1.4/tests/test_ephemetoot.py` & `ephemetoot-3.2.0/tests/test_ephemetoot.py`

 * *Files identical despite different names*

### Comparing `ephemetoot-3.1.4/setup.py` & `ephemetoot-3.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,43 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: ephemetoot
+Version: 3.2.0
+Summary: A command line tool to delete your old toots
+Author-email: Hugh Rundle <ephemetoot@hugh.run>
+License: GPL-3.0-or-later
+Project-URL: homepage, https://ephemetoot.hugh.run
+Project-URL: repository, https://github.com/hughrun/ephemetoot
+Keywords: mastodon,api,microblogging
+Classifier: Environment :: Console
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Communications
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
 
-packages = \
-['ephemetoot']
+# 🥳 ==> 🧼 ==> 😇
 
-package_data = \
-{'': ['*']}
+## Prior work
+The initial `ephemetoot` script was based on [this tweet-deleting script](https://gist.github.com/flesueur/bcb2d9185b64c5191915d860ad19f23f) by [@flesueur](https://github.com/flesueur)
 
-install_requires = \
-['mastodon.py>=1.4.3,<2.0.0', 'pyyaml>=5.0,<6.0', 'requests>=2.22.0,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['ephemetoot = ephemetoot.console:main']}
-
-setup_kwargs = {
-    'name': 'ephemetoot',
-    'version': '3.1.4',
-    'description': 'A command line tool to delete your old toots',
-    'long_description': '# 🥳 ==> 🧼 ==> 😇\n\n## Prior work\nThe initial `ephemetoot` script was based on [this tweet-deleting script](https://gist.github.com/flesueur/bcb2d9185b64c5191915d860ad19f23f) by [@flesueur](https://github.com/flesueur)\n\n`ephemetoot` relies heavily on the [Mastodon.py](https://pypi.org/project/Mastodon.py/) package by [@halcy](https://github.com/halcy)\n\n## Usage\n\nYou can use `ephemetoot` to delete [Mastodon](https://github.com/tootsuite/mastodon) toots that are older than a certain number of days (default is 365). Toots can optionally be saved from deletion if:\n* they are pinned; or\n* they include certain hashtags; or\n* they have certain visibility; or\n* they are individually listed to be kept\n\nThere are various options controlling timing, scheduling, and output.\n\nRun from the command line with `ephemetoot`.\n\nRun `ephemetoot --help` or read the docs for all options.\n\n## Contributing\n\nephemetoot is packaged using `poetry` and tested using `pytest`.\n\nFor all bugs, suggestions, pull requests or other contributions, please check the [contributing guide](https://github.com/hughrun/ephemetoot/blob/master/docs/contributing.md).\n',
-    'author': 'Hugh Rundle',
-    'author_email': 'ephemetoot@hugh.run',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://ephemetoot.hugh.run',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+`ephemetoot` relies heavily on the [Mastodon.py](https://pypi.org/project/Mastodon.py/) package by [@halcy](https://github.com/halcy)
 
+## Usage
 
-setup(**setup_kwargs)
+You can use `ephemetoot` to delete [Mastodon](https://github.com/tootsuite/mastodon) toots that are older than a certain number of days (default is 365). Toots can optionally be saved from deletion if:
+* they are pinned; or
+* they include certain hashtags; or
+* they have certain visibility; or
+* they are individually listed to be kept
+
+There are various options controlling timing, scheduling, and output.
+
+Run from the command line with `ephemetoot`.
+
+Run `ephemetoot --help` or read the docs for all options.
+
+## Contributing
+
+ephemetoot is now in maintenance mode, and new features will not be considered.
+
+For bugs or other contributions, please check the [contributing guide](https://github.com/hughrun/ephemetoot/blob/master/docs/contributing.md).
```

### Comparing `ephemetoot-3.1.4/PKG-INFO` & `ephemetoot-3.2.0/ephemetoot.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 Metadata-Version: 2.1
 Name: ephemetoot
-Version: 3.1.4
+Version: 3.2.0
 Summary: A command line tool to delete your old toots
-Home-page: https://ephemetoot.hugh.run
+Author-email: Hugh Rundle <ephemetoot@hugh.run>
 License: GPL-3.0-or-later
+Project-URL: homepage, https://ephemetoot.hugh.run
+Project-URL: repository, https://github.com/hughrun/ephemetoot
 Keywords: mastodon,api,microblogging
-Author: Hugh Rundle
-Author-email: ephemetoot@hugh.run
-Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications
-Requires-Dist: mastodon.py (>=1.4.3,<2.0.0)
-Requires-Dist: pyyaml (>=5.0,<6.0)
-Requires-Dist: requests (>=2.22.0,<3.0.0)
-Project-URL: Repository, https://github.com/hughrun/ephemetoot
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
 
 # 🥳 ==> 🧼 ==> 😇
 
 ## Prior work
 The initial `ephemetoot` script was based on [this tweet-deleting script](https://gist.github.com/flesueur/bcb2d9185b64c5191915d860ad19f23f) by [@flesueur](https://github.com/flesueur)
 
 `ephemetoot` relies heavily on the [Mastodon.py](https://pypi.org/project/Mastodon.py/) package by [@halcy](https://github.com/halcy)
@@ -42,11 +34,10 @@
 
 Run from the command line with `ephemetoot`.
 
 Run `ephemetoot --help` or read the docs for all options.
 
 ## Contributing
 
-ephemetoot is packaged using `poetry` and tested using `pytest`.
-
-For all bugs, suggestions, pull requests or other contributions, please check the [contributing guide](https://github.com/hughrun/ephemetoot/blob/master/docs/contributing.md).
+ephemetoot is now in maintenance mode, and new features will not be considered.
 
+For bugs or other contributions, please check the [contributing guide](https://github.com/hughrun/ephemetoot/blob/master/docs/contributing.md).
```

