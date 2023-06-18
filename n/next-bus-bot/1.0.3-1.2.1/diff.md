# Comparing `tmp/next-bus-bot-1.0.3.tar.gz` & `tmp/next-bus-bot-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "next-bus-bot-1.0.3.tar", last modified: Tue Dec 13 08:52:18 2022, max compression
+gzip compressed data, was "next-bus-bot-1.2.1.tar", last modified: Sun Jun 18 10:19:07 2023, max compression
```

## Comparing `next-bus-bot-1.0.3.tar` & `next-bus-bot-1.2.1.tar`

### file list

```diff
@@ -1,18 +1,28 @@
-drwxr-xr-x   0 pac       (1000) pac       (1000)        0 2022-12-13 08:52:18.809865 next-bus-bot-1.0.3/
--rw-r--r--   0 pac       (1000) pac       (1000)     2748 2022-12-13 08:52:18.809865 next-bus-bot-1.0.3/PKG-INFO
--rw-r--r--   0 pac       (1000) pac       (1000)     1990 2022-12-12 22:00:13.000000 next-bus-bot-1.0.3/README.rst
--rw-r--r--   0 pac       (1000) pac       (1000)     1673 2022-12-13 08:51:44.000000 next-bus-bot-1.0.3/pyproject.toml
--rw-r--r--   0 pac       (1000) pac       (1000)       38 2022-12-13 08:52:18.809865 next-bus-bot-1.0.3/setup.cfg
-drwxr-xr-x   0 pac       (1000) pac       (1000)        0 2022-12-13 08:52:18.806532 next-bus-bot-1.0.3/src/
-drwxr-xr-x   0 pac       (1000) pac       (1000)        0 2022-12-13 08:52:18.806532 next-bus-bot-1.0.3/src/nbb/
--rw-r--r--   0 pac       (1000) pac       (1000)        0 2022-12-03 11:17:27.000000 next-bus-bot-1.0.3/src/nbb/__init__.py
--rw-r--r--   0 pac       (1000) pac       (1000)     5364 2022-12-12 21:49:32.000000 next-bus-bot-1.0.3/src/nbb/backend.py
--rwxr-xr-x   0 pac       (1000) pac       (1000)     1864 2022-12-12 21:39:45.000000 next-bus-bot-1.0.3/src/nbb/cli.py
--rw-r--r--   0 pac       (1000) pac       (1000)     1503 2022-12-12 21:13:50.000000 next-bus-bot-1.0.3/src/nbb/nbb_conf.toml
-drwxr-xr-x   0 pac       (1000) pac       (1000)        0 2022-12-13 08:52:18.806532 next-bus-bot-1.0.3/src/next_bus_bot.egg-info/
--rw-r--r--   0 pac       (1000) pac       (1000)     2748 2022-12-13 08:52:18.000000 next-bus-bot-1.0.3/src/next_bus_bot.egg-info/PKG-INFO
--rw-r--r--   0 pac       (1000) pac       (1000)      343 2022-12-13 08:52:18.000000 next-bus-bot-1.0.3/src/next_bus_bot.egg-info/SOURCES.txt
--rw-r--r--   0 pac       (1000) pac       (1000)        1 2022-12-13 08:52:18.000000 next-bus-bot-1.0.3/src/next_bus_bot.egg-info/dependency_links.txt
--rw-r--r--   0 pac       (1000) pac       (1000)       37 2022-12-13 08:52:18.000000 next-bus-bot-1.0.3/src/next_bus_bot.egg-info/entry_points.txt
--rw-r--r--   0 pac       (1000) pac       (1000)      115 2022-12-13 08:52:18.000000 next-bus-bot-1.0.3/src/next_bus_bot.egg-info/requires.txt
--rw-r--r--   0 pac       (1000) pac       (1000)        4 2022-12-13 08:52:18.000000 next-bus-bot-1.0.3/src/next_bus_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:19:07.561010 next-bus-bot-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:19:07.557009 next-bus-bot-1.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:19:07.557009 next-bus-bot-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-18 10:18:44.000000 next-bus-bot-1.2.1/.github/workflows/linters.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-18 10:18:44.000000 next-bus-bot-1.2.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-18 10:18:44.000000 next-bus-bot-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-18 10:18:44.000000 next-bus-bot-1.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-18 10:19:07.557009 next-bus-bot-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-18 10:18:44.000000 next-bus-bot-1.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-18 10:18:44.000000 next-bus-bot-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 10:19:07.561010 next-bus-bot-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:19:07.557009 next-bus-bot-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:19:07.557009 next-bus-bot-1.2.1/src/nbb/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-18 10:18:44.000000 next-bus-bot-1.2.1/src/nbb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 10:19:07.000000 next-bus-bot-1.2.1/src/nbb/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-18 10:18:44.000000 next-bus-bot-1.2.1/src/nbb/api_call.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1739 2023-06-18 10:18:44.000000 next-bus-bot-1.2.1/src/nbb/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-18 10:18:44.000000 next-bus-bot-1.2.1/src/nbb/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-18 10:18:44.000000 next-bus-bot-1.2.1/src/nbb/idfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-18 10:18:44.000000 next-bus-bot-1.2.1/src/nbb/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-18 10:18:44.000000 next-bus-bot-1.2.1/src/nbb/nbb_conf.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:19:07.557009 next-bus-bot-1.2.1/src/next_bus_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-18 10:19:07.000000 next-bus-bot-1.2.1/src/next_bus_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-18 10:19:07.000000 next-bus-bot-1.2.1/src/next_bus_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 10:19:07.000000 next-bus-bot-1.2.1/src/next_bus_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-18 10:19:07.000000 next-bus-bot-1.2.1/src/next_bus_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-18 10:19:07.000000 next-bus-bot-1.2.1/src/next_bus_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-18 10:19:07.000000 next-bus-bot-1.2.1/src/next_bus_bot.egg-info/top_level.txt
```

### Comparing `next-bus-bot-1.0.3/PKG-INFO` & `next-bus-bot-1.2.1/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,18 @@
-Metadata-Version: 2.1
-Name: next-bus-bot
-Version: 1.0.3
-Summary: Get the next in coming buses at a Paris area Station.
-Author-email: Pierre-Antoine Comby <pierre-antoine.comby@crans.org>
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Utilities
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: test
-Provides-Extra: dev
-
 ===============
 Next Bus Bot
 ===============
 
 A bot/ cli tool that simply gives you the waiting times for next buses at your favorite bus stop.
 
 It works only for the IDFM/RATP Network, relying on the api ``lines/v4``. For now only a handfull of bus stops on the Plateau de Saclay are registered, but you can add your own
 
 
 .. warning::
 
-   This is a personal toy project for learning new stuff in python (Python packaging, TDD, CLI tools, etc ...).
-   It *might* feel overengineered, if so, it's on purpose.
-
    I am not responsible if you arrive late at your work.
    For serious travel planning, use your favorite app.
 
 Example
 -------
 ::
 
@@ -66,33 +43,60 @@
    $ git clone git@github.com:paquiteau/nbb/
 
 2. create your venv with your favorite tool
 3. Install locally the package with bells and whistles ::
 
    $ (venv) pip install -e .[dev,test]
 
-4. Run tests ::
-
-   $ pytest
-
-
 
 TODO
 ----
- - automatic aliasing of stops (based on initials )
+ - automatic aliasing of stops (based on initials)
  - support for direction filtering
- - publish on PyPi
  - Add support for a bot front-end (slack, discord, IRC, etc).
  - Extend the useful bus stops.
 
 Configuration
 =============
 
 nbb can be configured via its command line argument, or via a config file `nbb_conf.toml`, it uses `TOML https://toml.io/en/` syntax formatting. Suitable location for the config file are, loaded in this order:
 
  1. `nbb/nbb_conf.toml`
  2. `~/.config/nbb_conf.toml`
  3. `nbb_conf.toml` in current directory.
  4. `nbb --config <file>`
 
 
-An example (and default) config file is available in `nbb/nbb_conf.toml`.
+An example (and default) config file is available in `nbb/nbb_conf`, and a example config is:
+
+.. code-block:: toml
+
+    [cli]
+    # Default parameters for the CLI
+    pretty = true     # Emoji in the terminal
+    compact = false    # More condensed output
+    verbose = false    # More verbose output, only for debugging.
+
+    [stop.places]
+    # List of bus stops, with their name and their ID
+    # You can find the ID of a stop by looking at the URL of the stop on the IDFM website
+    # https://data.iledefrance-mobilites.fr/explore/dataset/zones-de-correspondance/custom/?disjunctive.zdctype
+
+    # The name of the step as a key does not matter,
+    # it should only be consistent between the stops, stops.aliases and stop.directions sections.
+    #
+    # The first stop defined is the default one.
+
+    [stop.aliases]
+    # Aliases for the stops defined in stop.places
+    "Mare du Vivier" = ["CEA Porte Sud", "Neurospin", "nsp", "mdv"]
+    "Moulon" = ["ens"]
+    "Raoul Dautry" = ["CEA Porte Est"]
+    "Place Marguerite Perey" = ["Inria"]
+
+
+    [stop.direction_filter]
+    # Direction filter for the stops defined in stop.places.
+
+    # For each stop you can filter the direction
+    "Mare du Vivier" = ["Gare du Guichet", "Centre Commercial Ulis 2"]      # Only keep the buses that have either 'gare du guichet'  or  'Centre commercial ulis2' as destination.
+    "Moulon" = ["Gare du Guichet", "Centre Commercial Ulis 2"]      # Only keep the gare du guichet  and Centre commercial ulis2
```

### Comparing `next-bus-bot-1.0.3/pyproject.toml` & `next-bus-bot-1.2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [project]
 name = "next-bus-bot"
 description = "Get the next in coming buses at a Paris area Station."
 
-version = "1.0.3"
+dynamic = ["version"]
 authors =[
 {name="Pierre-Antoine Comby", email="pierre-antoine.comby@crans.org"}
 ]
 
 dependencies = [
   "requests",
   "tomli; python_version <= '3.10'",
 ]
 
 readme = "README.rst"
+license = {file = "LICENSE.txt"}
 
 requires-python = ">=3.7"
 # For a list of valid classifiers, see https://pypi.org/classifiers/
 classifiers = [ 
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "Topic :: Utilities",
@@ -36,20 +37,29 @@
 [project.scripts]
 nbb = "nbb.cli:main"
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov", "pytest-xdist", "pytest-sugar"]
 dev = ["black", "isort"]
 
+
 [build-system]
-requires = ["setuptools", "wheel"]
+# These are the assumed default build requirements from pip:
+# https://pip.pypa.io/en/stable/reference/pip/#pep-517-and-518-support
+requires = ["setuptools>=43.0.0", "setuptools_scm[toml]>=6.2", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools.packages.find]
+where=["src"]
 
-[tool.setuptools]
 
-package-data = {"nbb" = ["*.toml"]}
+[tool.setuptools_scm]
+write_to = "src/nbb/_version.py"
+version_scheme = "python-simplified-semver"
+local_scheme="no-local-version"
 
 [tool.coverage.run]
 omit = ["*tests*"]
 
 [tool.coverage.report]
 precision = 2
 exclude_lines = ["pragma: no cover", "raise NotImplementedError"]
```

### Comparing `next-bus-bot-1.0.3/src/nbb/cli.py` & `next-bus-bot-1.2.1/src/nbb/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,59 @@
 # /usr/bin/env python3
 """
 CLI frontend.
 """
 import argparse
-import os
+import datetime
 
-try:
-    import tomllib as toml
-except ImportError:
-    import tomli as toml
-
-from nbb.backend import get_formatted_response, get_stop_infos
+from nbb.api_call import get_next_passes
+from nbb.config import get_config, get_stop_infos
 
 
 def parser():
     """Initialize parser."""
     parser = argparse.ArgumentParser()
     parser.add_argument("--config", default=None)
+    parser.add_argument("--raw", action="store_true")
     parser.add_argument("--simple", action="store_true")
     parser.add_argument("--compact", action="store_true")
     parser.add_argument("--verbose", action="store_true")
-    parser.add_argument("stop_name", nargs="*", default=None)
+    parser.add_argument("stop_name", nargs="?", default=None)
     ns = parser.parse_args()
-    if len(ns.stop_name) > 0:
-        ns.stop_name = " ".join(ns.stop_name)
-    else:
-        ns.stop_name = None
     if ns.verbose:
         print("This is nbb cli\nVerbose = ON")
     return ns
 
 
-def _load_toml(filename):
-    with open(filename, "rb") as f:
-        try:
-            conf = toml.load(f)
-        except FileNotFoundError:
-            print(f"{filename} specified but not found.")
-            exit(1)
-        except toml.TOMLDecodeError as e:
-            print(e)
-            exit(1)
-    return conf
-
-
-def get_config(config_file=None):
-    """Load config file."""
-    if config_file is None:
-        config_file = os.path.join(os.path.dirname(__file__), "nbb_conf.toml")
-
-    conf = _load_toml(config_file)
-    return conf
-
-
 def main():
     """Execute main CLI function."""
     ns = parser()
     if ns.verbose:
         print("loading config")
 
     conf = get_config(ns.config)
     # Get the default stop as the first one registered:
-    stop_name, line_code, stop_code, filters = get_stop_infos(conf, ns.stop_name)
+    stop_name, stop_code, filters = get_stop_infos(conf, ns.stop_name)
+
+    next_passes = get_next_passes(stop_code)
+    # Remove past buses
+    for i, n in enumerate(next_passes):
+        if n.time < datetime.datetime.now().astimezone():
+            n.is_valid = False
+    # Filter by direction
+    if direction_filter := conf["stop"]["direction_filter"].get(stop_name, None):
+        for i, n in enumerate(next_passes):
+            if n.destination not in direction_filter:
+                n.is_valid = False
 
-    print(f"Next buses at {stop_name}")
     print(
-        get_formatted_response(
-            line_code, stop_code, filters, pretty=not ns.simple, compact=ns.compact
-        )
+        f"Next buses at {stop_name} planned at "
+        f"{datetime.datetime.now().astimezone().strftime('%H:%M')}"
+    )
+    ret_string = "\n".join(
+        n.as_str(ns.compact, pretty=not ns.simple) for n in next_passes if n.is_valid
     )
+    print(ret_string)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `next-bus-bot-1.0.3/src/nbb/nbb_conf.toml` & `next-bus-bot-1.2.1/src/nbb/nbb_conf.toml`

 * *Files 26% similar despite different names*

```diff
@@ -4,40 +4,36 @@
 # output formatting option, default are False.
 
 pretty = true
 compact = true
 verbose = false
 
 [stop.places]
-# each stop shoud contains a line code and a "Zone de correspondance" code
-#
-# Line references:
-# https://data.iledefrance-mobilites.fr/explore/dataset/referentiel-des-lignes/table/
-# Zone de correspondance reference:
+
+# List of bus stops, with their name and their ID
+# You can find the ID of a stop by looking at the URL of the stop on the IDFM website
 # https://data.iledefrance-mobilites.fr/explore/dataset/zones-de-correspondance/custom/?disjunctive.zdctype
-#
-# C01561 is the bus line "9" on the Plateau de Saclay.
-# C01567 is the bus line "Express 91-06" on the plateau de Saclay.
-#
+
 # The name of the step as a key does not matter,
 # it should only be consistent between the stops, stops.aliases and stop.directions sections.
 #
 # The first stop defined is the default one.
-#
-"Mare du Vivier" = ["C01561", 420704]
-"Moulon" = ["C01561", 63086]
-"Raoul Dautry" = ["C01561", 63236]
-"Place Marguerite Perey" = ["C01567", 63144]
+
+"Mare du Vivier" = 420704
+"Moulon" =  63086
+"Raoul Dautry" = 63236
+"Place Marguerite Perey" = 63144
 
 [stop.aliases]
-#
-"Mare du Vivier" = ["CEA Porte Sud", "Neurospin", "nsp"]
-"Moulon" = ["ENS Paris-Saclay"]
+# Aliases for the stops defined in stop.places
+"Mare du Vivier" = ["CEA Porte Sud", "Neurospin", "nsp", "mdv"]
+"Moulon" = ["ens"]
 "Raoul Dautry" = ["CEA Porte Est"]
 "Place Marguerite Perey" = ["Inria"]
 
 [stop.direction_filter]
 
 # For each stop you can filter direction, either by specifying a IDFM stop_area code, or the commercial name.
 
-"Mare du Vivier" = ["Gare du Guichet", 60998]      # Only keep the gare du guichet  and Centre commercial ulis2
+"Mare du Vivier" = ["Gare du Guichet", "Centre Commercial Ulis 2"]      # Only keep the gare du guichet  and Centre commercial ulis2
+"Moulon" = ["Gare du Guichet", "Centre Commercial Ulis 2"]      # Only keep the gare du guichet  and Centre commercial ulis2
 #"Mare du Vivier" = ["Gare du Guichet", "60998", "!Christ de Saclay"]  # Filter Christ de Saclay direction out
```

