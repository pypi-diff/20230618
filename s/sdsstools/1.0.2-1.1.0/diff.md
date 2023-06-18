# Comparing `tmp/sdsstools-1.0.2.tar.gz` & `tmp/sdsstools-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdsstools-1.0.2.tar", max compression
+gzip compressed data, was "sdsstools-1.1.0.tar", max compression
```

## Comparing `sdsstools-1.0.2.tar` & `sdsstools-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1504 2022-12-27 20:04:20.189550 sdsstools-1.0.2/LICENSE.md
--rw-r--r--   0        0        0    11344 2022-12-27 20:04:20.189550 sdsstools-1.0.2/README.md
--rw-r--r--   0        0        0     2143 2022-12-27 20:04:20.189550 sdsstools-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      447 2022-12-27 20:04:20.189550 sdsstools-1.0.2/src/sdsstools/__init__.py
--rw-r--r--   0        0        0     4263 2022-12-27 20:04:20.189550 sdsstools-1.0.2/src/sdsstools/_tasks.py
--rw-r--r--   0        0        0        0 2022-12-27 20:04:20.189550 sdsstools-1.0.2/src/sdsstools/_vendor/__init__.py
--rw-r--r--   0        0        0     6457 2022-12-27 20:04:20.189550 sdsstools-1.0.2/src/sdsstools/_vendor/color_print.py
--rwxr-xr-x   0        0        0      717 2022-12-27 20:04:20.189550 sdsstools-1.0.2/src/sdsstools/_vendor/toml/__init__.py
--rwxr-xr-x   0        0        0    38049 2022-12-27 20:04:20.189550 sdsstools-1.0.2/src/sdsstools/_vendor/toml/decoder.py
--rwxr-xr-x   0        0        0     9988 2022-12-27 20:04:20.189550 sdsstools-1.0.2/src/sdsstools/_vendor/toml/encoder.py
--rwxr-xr-x   0        0        0      346 2022-12-27 20:04:20.189550 sdsstools-1.0.2/src/sdsstools/_vendor/toml/ordered.py
--rwxr-xr-x   0        0        0      618 2022-12-27 20:04:20.193550 sdsstools-1.0.2/src/sdsstools/_vendor/toml/tz.py
--rwxr-xr-x   0        0        0     1348 2022-12-27 20:04:20.193550 sdsstools-1.0.2/src/sdsstools/cli.py
--rw-r--r--   0        0        0     9250 2022-12-27 20:04:20.193550 sdsstools-1.0.2/src/sdsstools/configuration.py
--rw-r--r--   0        0        0     7796 2022-12-27 20:04:20.193550 sdsstools-1.0.2/src/sdsstools/daemonizer.py
--rw-r--r--   0        0        0    10270 2022-12-27 20:04:20.193550 sdsstools-1.0.2/src/sdsstools/logger.py
--rw-r--r--   0        0        0     3268 2022-12-27 20:04:20.193550 sdsstools-1.0.2/src/sdsstools/metadata.py
--rw-r--r--   0        0        0     4588 2022-12-27 20:04:20.193550 sdsstools-1.0.2/src/sdsstools/time.py
--rw-r--r--   0        0        0      692 2022-12-27 20:04:20.193550 sdsstools-1.0.2/src/sdsstools/utils.py
--rw-r--r--   0        0        0    12668 1970-01-01 00:00:00.000000 sdsstools-1.0.2/setup.py
--rw-r--r--   0        0        0    12508 1970-01-01 00:00:00.000000 sdsstools-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-06-18 18:51:07.295337 sdsstools-1.1.0/LICENSE.md
+-rw-r--r--   0        0        0    11344 2023-06-18 18:51:07.295337 sdsstools-1.1.0/README.md
+-rw-r--r--   0        0        0     2246 2023-06-18 18:51:07.299337 sdsstools-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-06-18 18:51:07.299337 sdsstools-1.1.0/src/sdsstools/__init__.py
+-rw-r--r--   0        0        0     4263 2023-06-18 18:51:07.299337 sdsstools-1.1.0/src/sdsstools/_tasks.py
+-rw-r--r--   0        0        0        0 2023-06-18 18:51:07.299337 sdsstools-1.1.0/src/sdsstools/_vendor/__init__.py
+-rw-r--r--   0        0        0     6457 2023-06-18 18:51:07.299337 sdsstools-1.1.0/src/sdsstools/_vendor/color_print.py
+-rwxr-xr-x   0        0        0      717 2023-06-18 18:51:07.299337 sdsstools-1.1.0/src/sdsstools/_vendor/toml/__init__.py
+-rwxr-xr-x   0        0        0    38049 2023-06-18 18:51:07.299337 sdsstools-1.1.0/src/sdsstools/_vendor/toml/decoder.py
+-rwxr-xr-x   0        0        0     9988 2023-06-18 18:51:07.299337 sdsstools-1.1.0/src/sdsstools/_vendor/toml/encoder.py
+-rwxr-xr-x   0        0        0      346 2023-06-18 18:51:07.299337 sdsstools-1.1.0/src/sdsstools/_vendor/toml/ordered.py
+-rwxr-xr-x   0        0        0      618 2023-06-18 18:51:07.299337 sdsstools-1.1.0/src/sdsstools/_vendor/toml/tz.py
+-rwxr-xr-x   0        0        0     1348 2023-06-18 18:51:07.299337 sdsstools-1.1.0/src/sdsstools/cli.py
+-rw-r--r--   0        0        0    10043 2023-06-18 18:51:07.299337 sdsstools-1.1.0/src/sdsstools/configuration.py
+-rw-r--r--   0        0        0     7796 2023-06-18 18:51:07.299337 sdsstools-1.1.0/src/sdsstools/daemonizer.py
+-rw-r--r--   0        0        0    10466 2023-06-18 18:51:07.299337 sdsstools-1.1.0/src/sdsstools/logger.py
+-rw-r--r--   0        0        0     3268 2023-06-18 18:51:07.299337 sdsstools-1.1.0/src/sdsstools/metadata.py
+-rw-r--r--   0        0        0     4588 2023-06-18 18:51:07.299337 sdsstools-1.1.0/src/sdsstools/time.py
+-rw-r--r--   0        0        0      692 2023-06-18 18:51:07.299337 sdsstools-1.1.0/src/sdsstools/utils.py
+-rw-r--r--   0        0        0    12558 1970-01-01 00:00:00.000000 sdsstools-1.1.0/PKG-INFO
```

### Comparing `sdsstools-1.0.2/LICENSE.md` & `sdsstools-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdsstools-1.0.2/README.md` & `sdsstools-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sdsstools-1.0.2/pyproject.toml` & `sdsstools-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdsstools"
-version = "1.0.2"
+version = "1.1.0"
 description = "Small tools for SDSS products"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/sdsstools"
 repository = "https://github.com/sdss/sdsstools"
 keywords = ["astronomy", "software"]
@@ -20,17 +20,19 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 pyyaml = ">=4.0"
 pygments = "^2.5.2"
 invoke = "^1.3.0"
 packaging = ">=20.4"
 daemonocle = "^1.0.2"
+typing-extensions = "^4.6.3"
 
-[tool.poetry.dev-dependencies]
-ipython = ">=8.0.0"
+[tool.poetry.group.dev.dependencies]
+ipython = [{version = ">=8.14.0", python = ">=3.9"},
+           {version = ">=8.0.0", python = ">=3.8,<3.9"}]
 flake8 = ">=3.7.9"
 doc8 = ">=0.8.0"
 isort = ">=5.0.0"
 ipdb = ">=0.13.3"
 toml = ">=0.10.0"
 pytest = ">=6.0.0"
 pytest-sugar = ">=0.9.4"
@@ -40,16 +42,14 @@
 wheel = ">=0.33.6"
 click = ">=8.0.0"
 pytest-click = ">=0.3"
 pytest-mock = ">=3.2.0"
 pytest-asyncio = ">=0.14.0"
 black = {version = ">=20.8b1", allow-prereleases = true}
 
-[tool.poetry.extras]
-
 [tool.poetry.scripts]
 sdss = 'sdsstools.cli:main'
 daemonize = 'sdsstools.daemonizer:daemonize'
 
 [tool.black]
 line-length = 88
 target-version = ['py38']
```

### Comparing `sdsstools-1.0.2/src/sdsstools/_tasks.py` & `sdsstools-1.1.0/src/sdsstools/_tasks.py`

 * *Files identical despite different names*

### Comparing `sdsstools-1.0.2/src/sdsstools/_vendor/color_print.py` & `sdsstools-1.1.0/src/sdsstools/_vendor/color_print.py`

 * *Files identical despite different names*

### Comparing `sdsstools-1.0.2/src/sdsstools/_vendor/toml/__init__.py` & `sdsstools-1.1.0/src/sdsstools/_vendor/toml/__init__.py`

 * *Files identical despite different names*

### Comparing `sdsstools-1.0.2/src/sdsstools/_vendor/toml/decoder.py` & `sdsstools-1.1.0/src/sdsstools/_vendor/toml/decoder.py`

 * *Files identical despite different names*

### Comparing `sdsstools-1.0.2/src/sdsstools/_vendor/toml/encoder.py` & `sdsstools-1.1.0/src/sdsstools/_vendor/toml/encoder.py`

 * *Files identical despite different names*

### Comparing `sdsstools-1.0.2/src/sdsstools/_vendor/toml/tz.py` & `sdsstools-1.1.0/src/sdsstools/_vendor/toml/tz.py`

 * *Files identical despite different names*

### Comparing `sdsstools-1.0.2/src/sdsstools/cli.py` & `sdsstools-1.1.0/src/sdsstools/cli.py`

 * *Files identical despite different names*

### Comparing `sdsstools-1.0.2/src/sdsstools/configuration.py` & `sdsstools-1.1.0/src/sdsstools/configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import os
 import pathlib
 import re
 
 from typing import Any, Dict, Optional, Union
 
 import yaml
+from typing_extensions import Self
 
 
 __all__ = ["read_yaml_file", "merge_config", "get_config", "Configuration"]
 
 
 __ENVVARS__ = {}
 
@@ -192,19 +193,23 @@
     elif user_path and os.path.exists(user_path):
         custom_config_fn = user_path
     else:
         custom_config_fn = None
 
     if merge_mode == "update":
         return Configuration(
-            custom_config_fn, base_config=config_file, default_envvars=default_envvars
+            custom_config_fn,
+            base_config=config_file,
+            default_envvars=default_envvars,
         )
     else:
         return Configuration(
-            custom_config_fn, base_config=None, default_envvars=default_envvars
+            custom_config_fn,
+            base_config=None,
+            default_envvars=default_envvars,
         )
 
 
 class Configuration(dict):
     """A configuration class.
 
     Parameters
@@ -223,25 +228,34 @@
         self,
         config: Optional[Union[AnyPath, ConfigType]] = None,
         base_config: Optional[Union[AnyPath, ConfigType]] = None,
         default_envvars: Dict[str, Any] = {},
     ):
         global __ENVVARS__
 
+        self._BASE: dict | None = None
+        self._CONFIG: dict | None = None
+
+        self._BASE_CONFIG_FILE: AnyPath | None = None
+        self._CONFIG_FILE: AnyPath | None = None
+
         if base_config:
             self._BASE = self._parse_config(base_config, use_base=False)
             if isinstance(base_config, dict):
-                self.CONFIG_FILE = None
+                self._BASE_CONFIG_FILE = None
             else:
-                self.CONFIG_FILE = os.path.realpath(str(base_config))
+                self._BASE_CONFIG_FILE = os.path.realpath(str(base_config))
         else:
             self._BASE = {}
-            self.CONFIG_FILE = None
+            self._BASE_CONFIG_FILE = None
 
-        self._BASE_CONFIG_FILE = self.CONFIG_FILE
+        if isinstance(config, dict):
+            self._CONFIG = config
+        else:
+            self._CONFIG_FILE = config
 
         __ENVVARS__ = default_envvars
 
         self.load(config)
 
     def _parse_config(self, config, use_base=True):
         """Parses the configuration and merges it with the base one."""
@@ -264,23 +278,39 @@
         config
             The configuration file or dictionary to load. If a base
             configuration was defined when the object was instantiated, it
             will be merged. If ``config=None``, the object will revert to the
             base configuration.
         use_base
             Merge the new configuration with the base config.
+
         """
 
         self.clear()
 
         if config is None:
             dict.__init__(self, self._BASE)
-            self.CONFIG_FILE = self._BASE_CONFIG_FILE
+            self._CONFIG_FILE = self._BASE_CONFIG_FILE
             return
 
         dict.__init__(self, self._parse_config(config, use_base=use_base))
 
         # Save name of the configuration file (if the input is a file).
         if isinstance(config, (str, pathlib.Path)):
-            self.CONFIG_FILE = str(config)
+            self._CONFIG_FILE = str(config)
         else:
-            self.CONFIG_FILE = None
+            self._CONFIG_FILE = None
+
+    def reload(self) -> Self:
+        """Reloads the configuration.
+
+        This will only have an effect if the configuration has been loaded from
+        files, in which case the files will be read again.
+
+        """
+
+        if self._BASE_CONFIG_FILE is not None:
+            self._BASE = self._parse_config(self._BASE_CONFIG_FILE, use_base=False)
+
+        self.load(self._CONFIG_FILE or dict(self))
+
+        return self
```

### Comparing `sdsstools-1.0.2/src/sdsstools/daemonizer.py` & `sdsstools-1.1.0/src/sdsstools/daemonizer.py`

 * *Files identical despite different names*

### Comparing `sdsstools-1.0.2/src/sdsstools/logger.py` & `sdsstools-1.1.0/src/sdsstools/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,16 @@
     """Custom `Formatter <logging.Formatter>` for the stream handler."""
 
     base_fmt = "%(message)s"
 
     def __init__(self, fmt=base_fmt):
         logging.Formatter.__init__(self, fmt)
 
+        self.print_time = False
+
     def format(self, record):
         colours = {
             "info": "blue",
             "debug": "magenta",
             "warning": "yellow",
             "critical": "red",
             "error": "red",
@@ -62,14 +64,17 @@
 
         levelname = record_cp.levelname.lower()
         message = record_cp.msg
 
         if levelname.lower() in colours:
             level_colour = colours[levelname]
             header = color_text("[{}]: ".format(levelname.upper()), level_colour)
+            if self.print_time:
+                now = datetime.datetime.now()
+                header = color_text(now.strftime("%H:%M:%S "), "lightgrey") + header
         else:
             return logging.Formatter.format(self, record)
 
         record_cp.msg = "{}{}".format(header, message)
 
         if levelname == "warning" and record_cp.args and len(record_cp.args) > 0:
             args = cast(List[str], record_cp.args)
```

### Comparing `sdsstools-1.0.2/src/sdsstools/metadata.py` & `sdsstools-1.1.0/src/sdsstools/metadata.py`

 * *Files identical despite different names*

### Comparing `sdsstools-1.0.2/src/sdsstools/time.py` & `sdsstools-1.1.0/src/sdsstools/time.py`

 * *Files identical despite different names*

### Comparing `sdsstools-1.0.2/src/sdsstools/utils.py` & `sdsstools-1.1.0/src/sdsstools/utils.py`

 * *Files identical despite different names*

### Comparing `sdsstools-1.0.2/setup.py` & `sdsstools-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,266 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: sdsstools
+Version: 1.1.0
+Summary: Small tools for SDSS products
+Home-page: https://github.com/sdss/sdsstools
+License: BSD-3-Clause
+Keywords: astronomy,software
+Author: José Sánchez-Gallego
+Author-email: gallegoj@uw.edu
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Documentation :: Sphinx
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: daemonocle (>=1.0.2,<2.0.0)
+Requires-Dist: invoke (>=1.3.0,<2.0.0)
+Requires-Dist: packaging (>=20.4)
+Requires-Dist: pygments (>=2.5.2,<3.0.0)
+Requires-Dist: pyyaml (>=4.0)
+Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
+Project-URL: Repository, https://github.com/sdss/sdsstools
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# sdsstools
 
-packages = \
-['sdsstools', 'sdsstools._vendor', 'sdsstools._vendor.toml']
+[![Versions](https://img.shields.io/badge/python->3.7-blue)](https://docs.python.org/3/)
+[![PyPI version](https://badge.fury.io/py/sdsstools.svg)](https://badge.fury.io/py/sdsstools)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Tests Status](https://github.com/sdss/sdsstools/workflows/Test/badge.svg)](https://github.com/sdss/sdsstools/actions)
+[![codecov](https://codecov.io/gh/sdss/sdsstools/branch/main/graph/badge.svg)](https://codecov.io/gh/sdss/sdsstools)
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['daemonocle>=1.0.2,<2.0.0',
- 'invoke>=1.3.0,<2.0.0',
- 'packaging>=20.4',
- 'pygments>=2.5.2,<3.0.0',
- 'pyyaml>=4.0']
-
-entry_points = \
-{'console_scripts': ['daemonize = sdsstools.daemonizer:daemonize',
-                     'sdss = sdsstools.cli:main']}
-
-setup_kwargs = {
-    'name': 'sdsstools',
-    'version': '1.0.2',
-    'description': 'Small tools for SDSS products',
-    'long_description': '# sdsstools\n\n[![Versions](https://img.shields.io/badge/python->3.7-blue)](https://docs.python.org/3/)\n[![PyPI version](https://badge.fury.io/py/sdsstools.svg)](https://badge.fury.io/py/sdsstools)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Tests Status](https://github.com/sdss/sdsstools/workflows/Test/badge.svg)](https://github.com/sdss/sdsstools/actions)\n[![codecov](https://codecov.io/gh/sdss/sdsstools/branch/main/graph/badge.svg)](https://codecov.io/gh/sdss/sdsstools)\n\n`sdsstools` provides several common tools for logging, configuration handling, version parsing, packaging, etc. Its main purpose is to consolidate some of the utilities originally found in the [python_template](https://github.com/sdss/python_template), allowing them to become dependencies that can be updated.\n\n**This is not intended to be a catch-all repository for astronomical tools.** `sdsstools` itself aims to have minimal dependencies (i.e., mainly the Python standard library and setuptools).\n\n## Using sdsstools\n\nTo use sdsstools simply install it with\n\n```console\npip install sdsstools\n```\n\nMost likely, you\'ll want to include sdsstools as a dependency for your library. To do so, either add to your `setup.cfg`\n\n```ini\n[options]\ninstall_requires =\n    sdsstools>=0.1.0\n```\n\n(this is equivalent of passing `install_requires=[\'sdsstools>=0.1.0\']` to `setuptools.setup`), or if you are using [poetry](https://poetry.eustace.io/) run `poetry add sdsstools`, which should add this line to your `pyproject.toml`\n\n```toml\n[tool.poetry.dependencies]\nsdsstools = { version="^0.1.0" }\n```\n\n## Logging\n\nsdsstools includes the [sdsstools.logger.SDSSLogger](https://github.com/sdss/sdsstools/blob/f30e00f527660fe8627e33a7f931b44410b0ff06/src/sdsstools/logger.py#L107) class, which provides a wrapper around the standard Python [logging](https://docs.python.org/3/library/logging.html) module. `SDSSLoger` provides the following features:\n\n- A console handler (accessible via the `.sh` attribute) with nice colouring.\n- Automatic capture of warnings and exceptions, which are formatted and redirected to the logger. For the console handler, this means that once the logger has been created, all warnings and exceptions are output normally but are clearer and more aesthetic.\n- A [TimedRotatingFileHandler](https://docs.python.org/3.8/library/logging.handlers.html#logging.handlers.TimedRotatingFileHandler) (accessible via the `.fh` attribute) that rotates at midnight UT, with good formatting.\n\nTo get a new logger for your application, simply do\n\n```python\nfrom sdsstools.logger import get_logger\n\nNAME = \'myrepo\'\nlog = get_logger(NAME)\n```\n\nThe file logger is disabled by default and can be started by calling `log.start_file_logger(path)`. By default a `TimedRotatingFileHandler` is created. If you want a normal `FileHandler` use `rotate=False`. The file mode defaults to `mode=\'a\'` (append).\n\nThe `SDSSLoger` instance also include an `asyncio_exception_handler` method that can be added to the asyncio event loop to handle exceptions; for example `loop.set_exception_handler(log.asyncio_exception_handler)`.\n\n## Configuration\n\nThe `sdsstools.configuration` module contains several utilities to deal with configuration files. The most useful one is [get_config](https://github.com/sdss/sdsstools/blob/d3d337953a37aaff9c38fead76b08b414164775a/src/sdsstools/configuration.py#L40), which allows to read a YAML configuration file. For example\n\n```python\nfrom sdsstools.configuration import get_config\n\nNAME = \'myrepo\'\nconfig = get_config(NAME, allow_user=True)\n```\n\n`get_config` assumes that the file is located in `etc/<NAME>.yml` relative from the file that calls `get_config`, but that can be changed by passing `config_file=<config-file-path>`. Additionally, if `allow_user=True` and a file exists in `~/.config/sdss/<NAME>.yaml`, this file is read and merged with the default configuration, overriding any parameter that is present in the user file. This allows to create a default configuration that lives with the library but that can be overridden by a user.\n\nIn addition to the (recommended) location `~/.config/sdss/<NAME>.yaml`, `get_config` also looks for user configuration files in `~/.config/sdss/<NAME>.yml`, `~/.config/sdss/<NAME>/<NAME>.y(a)ml`, and `~/.<NAME>/<NAME>.y(a)ml`.\n\n`get_config` returns an instance of [Configuration](https://github.com/sdss/sdsstools/blob/5af8339d2696d92e122b4195272130101b54daa7/src/sdsstools/configuration.py#L162), which behaves as a dictionary but allows to dynamically reload the configuration from a new user file by calling `load()`.\n\n`sdsstools.configuration` includes two other tools, `merge_config`, that allows to merge dictionaries recursively, and `read_yaml_file` to read a YAML file.\n\n### Extending a YAML file\n\n`read_yaml_file` provides a non-standard feature that allows you to extend one YAML file with another. To achieve this you need to add the tag `!extends <base-file>` at the top of the file that you want to extend. For example, if you have a file `base.yaml`\n\n```yaml\ncat1:\n    key1: value2\n\ncat2:\n    key2: 1\n```\n\nthat you want to use as a template for `extendable.yaml`\n\n```yaml\n#!extends base.yaml\n\ncat1:\n    key1: value1\n```\n\nyou can use `read_yaml_file` to parse the result\n\n```python\n>>> read_yaml_file(\'extendable.yaml\')\n{\'cat1\': {\'key1\': \'value2\'}, \'cat2\': {\'key2\': 1}}\n```\n\nThe path to the base file must be absolute or relative to the location of the file to be extended.\n\n## Metadata\n\nsdsscore provides tools to locate and parse metadata files (`pyproject.toml`, `setup.cfg`, `setup.py`). `get_metadata_files` locates the path of the metadata file relative to a given `path`. `get_package_version` tries to find the version of the package by looking for a version string in the metadata file or in the egg/wheel metadata file, if the package has been installed. To use it\n\n```python\nfrom sdsstools.metadata import get_package_version\n\n__version__ = get_package_version(path=__file__, package_name=\'sdss-camera\') or \'dev\'\n```\n\nThis will try to find and parse the version from the metadata file (we pass `__file__` to indicate where to start looking); if that fails, it will try to get the version from the installed package `sdss-camera`. If all fails, it will set the fallback version `\'dev\'`.\n\n## Command Line Interface\n\n`sdsstools` provides the command line tool `sdss`, which is just a thin wrapper around some commonly used [Invoke](https://www.pyinvoke.org/) tasks. `sdsstools` does not automatically install all the dependencies for the tasks, which need to be added manually.\n\n`sdss` provides the following tasks\n\n| Task | Options | Description |\n| --- | --- | --- |\n| clean | | Removes files produces during build and packaging. |\n| deploy | --test | Builds and deploys to PyPI (or the test server). Requires `twine` and `wheel`. |\n| install-deps | --extras | Installs dependencies from a `setup.cfg` file |\n| docs.build | --target | Builds the Sphinx documentation. Requires `Sphinx`. |\n| docs.show | --target | Shows the documentation in the browser. Requires `Sphinx`. |\n| docs.clean | --target | Cleans the documentation build. Requires `Sphinx`. |\n\n`sdss` assumes that the documentation lives in `docs/sphinx` relative to the root of the repository. This can be changed by setting the `sphinx.target` configuration in an `invoke.yaml` file, for example\n\n```yaml\nsphinx:\n    target: docs\n```\n\n## Click daemon command\n\nThe [daemonizer](src/sdsstools/daemonizer.py) module implements a [Click](https://palletsprojects.com/p/click/) command group that allows to spawn a daemon, and to stop and restart it. Internally the module uses [daemonocle](https://github.com/jnrbsn/daemonocle) (the package is not installed with `sdsstools` and needs to be pip-installed manually).\n\nA simple example of how to use `daemonizer` is\n\n```python\nimport time\nimport click\nfrom sdsstools.daemonizer import DaemonGroup\n\n@click.group(cls=DaemonGroup, prog=\'hello\', pidfile=\'/var/tmp/hello.pid\')\n@click.argument(\'NAME\', type=str)\n@click.option(\'--file\', type=str, default=\'hello.dat\')\ndef daemon(name):\n\n    with open(file, \'w\') as unit:\n        while True:\n            unit.write(f\'Hi {name}!\\n\')\n            unit.flush()\n            time.sleep(1)\n\nif __name__ == \'__main__\':\n    daemon()\n```\n\nThis will create a new group `hello` with four subcommands\n\n```console\nUsage: daemon [OPTIONS] NAME COMMAND [ARGS]...\n\nOptions:\n  --file\n  --help  Show this message and exit.\n\nCommands:\n  restart  Restart the daemon.\n  start    Start the daemon.\n  status   Report if the daemon is running.\n  stop     Stop the daemon.\n```\n\nNow we can run `daemon --file ~/hello.dat John start` and a new background process will start, writing to the file every second. We can stop it with `daemon stop`. In general the behaviour is identical to the [daemonocle Click implementation](https://github.com/jnrbsn/daemonocle#integration-with-mitsuhiko-s-click) but the internal are slightly different to allow the group callback to accept arguments. If the callback is a coroutine, it can be wrapped with the `cli_coro` decorator\n\n```python\nimport asyncio\nimport signal\nimport click\nfrom sdsstools.daemonizer import DaemonGroup, cli_coro\n\ndef shutdown(signal):\n    if signal == signal.SIGTERM:\n        cancel_something()\n\n@click.group(cls=DaemonGroup, prog=\'hello\', pidfile=\'/var/tmp/hello.pid\')\n@click.argument(\'NAME\', type=str)\n@click.option(\'--file\', type=str, default=\'hello.dat\')\n@cli_coro(shutdown_func=shutdown, signals=(signal.SIGTERM, signal.SIGINT))\nasync def daemon(name):\n\n    with open(file, \'w\') as unit:\n        while True:\n            unit.write(f\'Hi {name}!\\n\')\n            unit.flush()\n            await asyncio.sleep(1)\n```\n\n`cli_coro` can accept a `shutdown_func` function that is called when the coroutine receives a signal. The default signals handled are `(SIGHUP, SIGTERM, SIGINT)`.\n\n### Daemonizing a command\n\nTo execute any command as a daemon you can use the `daemonize` script that is installed with `sdsstools`. To start the process as a daemon do `daemonize start NAME COMMAND` when `NAME` is the name associated to the daemon (so that it can be stopped later) and `COMMAND` is the command to run, for example:\n\n```console\ndaemonize start apoActor python ./apoActor_main.py\n```\n\nTo stop the daemon do `daemonize stop NAME`. See `daemonize --help` for more options.\n\n## Date functions\n\nThe function `sdsstools.time.get_sjd()` returns the integer with the SDSS-style Modified Julian Day. The function accepts an observatory (`\'APO\'` or `\'LCO\'`) but otherwise will try to determine the current location from environment variables or the fully qualified domain name.\n\n## Bundled packages\n\nFor convenience, `sdsstools` bundles the following products:\n\n- A copy of [releases](https://github.com/bitprophet/releases) that fixes some issues with recent versions of `semantic-version`. This copy is not available in `sdsstools>=1.0.0`. `releases` is not maintained anymore, so use at your own risk.\n- A copy of [toml](https://github.com/uiri/toml) to read TOML files (used by the metadata submodule).\n\nYou can access them directly from the top-level namespace, `sdsstools.toml`, `sdsstools.releases`. To use `releases` with sphinx, simply add the following to your `config.py`\n\n```python\nextensions += [\'sdsstools.releases\']\n```\n',
-    'author': 'José Sánchez-Gallego',
-    'author_email': 'gallegoj@uw.edu',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/sdss/sdsstools',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+`sdsstools` provides several common tools for logging, configuration handling, version parsing, packaging, etc. Its main purpose is to consolidate some of the utilities originally found in the [python_template](https://github.com/sdss/python_template), allowing them to become dependencies that can be updated.
 
+**This is not intended to be a catch-all repository for astronomical tools.** `sdsstools` itself aims to have minimal dependencies (i.e., mainly the Python standard library and setuptools).
+
+## Using sdsstools
+
+To use sdsstools simply install it with
+
+```console
+pip install sdsstools
+```
+
+Most likely, you'll want to include sdsstools as a dependency for your library. To do so, either add to your `setup.cfg`
+
+```ini
+[options]
+install_requires =
+    sdsstools>=0.1.0
+```
+
+(this is equivalent of passing `install_requires=['sdsstools>=0.1.0']` to `setuptools.setup`), or if you are using [poetry](https://poetry.eustace.io/) run `poetry add sdsstools`, which should add this line to your `pyproject.toml`
+
+```toml
+[tool.poetry.dependencies]
+sdsstools = { version="^0.1.0" }
+```
+
+## Logging
+
+sdsstools includes the [sdsstools.logger.SDSSLogger](https://github.com/sdss/sdsstools/blob/f30e00f527660fe8627e33a7f931b44410b0ff06/src/sdsstools/logger.py#L107) class, which provides a wrapper around the standard Python [logging](https://docs.python.org/3/library/logging.html) module. `SDSSLoger` provides the following features:
+
+- A console handler (accessible via the `.sh` attribute) with nice colouring.
+- Automatic capture of warnings and exceptions, which are formatted and redirected to the logger. For the console handler, this means that once the logger has been created, all warnings and exceptions are output normally but are clearer and more aesthetic.
+- A [TimedRotatingFileHandler](https://docs.python.org/3.8/library/logging.handlers.html#logging.handlers.TimedRotatingFileHandler) (accessible via the `.fh` attribute) that rotates at midnight UT, with good formatting.
+
+To get a new logger for your application, simply do
+
+```python
+from sdsstools.logger import get_logger
+
+NAME = 'myrepo'
+log = get_logger(NAME)
+```
+
+The file logger is disabled by default and can be started by calling `log.start_file_logger(path)`. By default a `TimedRotatingFileHandler` is created. If you want a normal `FileHandler` use `rotate=False`. The file mode defaults to `mode='a'` (append).
+
+The `SDSSLoger` instance also include an `asyncio_exception_handler` method that can be added to the asyncio event loop to handle exceptions; for example `loop.set_exception_handler(log.asyncio_exception_handler)`.
+
+## Configuration
+
+The `sdsstools.configuration` module contains several utilities to deal with configuration files. The most useful one is [get_config](https://github.com/sdss/sdsstools/blob/d3d337953a37aaff9c38fead76b08b414164775a/src/sdsstools/configuration.py#L40), which allows to read a YAML configuration file. For example
+
+```python
+from sdsstools.configuration import get_config
+
+NAME = 'myrepo'
+config = get_config(NAME, allow_user=True)
+```
+
+`get_config` assumes that the file is located in `etc/<NAME>.yml` relative from the file that calls `get_config`, but that can be changed by passing `config_file=<config-file-path>`. Additionally, if `allow_user=True` and a file exists in `~/.config/sdss/<NAME>.yaml`, this file is read and merged with the default configuration, overriding any parameter that is present in the user file. This allows to create a default configuration that lives with the library but that can be overridden by a user.
+
+In addition to the (recommended) location `~/.config/sdss/<NAME>.yaml`, `get_config` also looks for user configuration files in `~/.config/sdss/<NAME>.yml`, `~/.config/sdss/<NAME>/<NAME>.y(a)ml`, and `~/.<NAME>/<NAME>.y(a)ml`.
+
+`get_config` returns an instance of [Configuration](https://github.com/sdss/sdsstools/blob/5af8339d2696d92e122b4195272130101b54daa7/src/sdsstools/configuration.py#L162), which behaves as a dictionary but allows to dynamically reload the configuration from a new user file by calling `load()`.
+
+`sdsstools.configuration` includes two other tools, `merge_config`, that allows to merge dictionaries recursively, and `read_yaml_file` to read a YAML file.
+
+### Extending a YAML file
+
+`read_yaml_file` provides a non-standard feature that allows you to extend one YAML file with another. To achieve this you need to add the tag `!extends <base-file>` at the top of the file that you want to extend. For example, if you have a file `base.yaml`
+
+```yaml
+cat1:
+    key1: value2
+
+cat2:
+    key2: 1
+```
+
+that you want to use as a template for `extendable.yaml`
+
+```yaml
+#!extends base.yaml
+
+cat1:
+    key1: value1
+```
+
+you can use `read_yaml_file` to parse the result
+
+```python
+>>> read_yaml_file('extendable.yaml')
+{'cat1': {'key1': 'value2'}, 'cat2': {'key2': 1}}
+```
+
+The path to the base file must be absolute or relative to the location of the file to be extended.
+
+## Metadata
+
+sdsscore provides tools to locate and parse metadata files (`pyproject.toml`, `setup.cfg`, `setup.py`). `get_metadata_files` locates the path of the metadata file relative to a given `path`. `get_package_version` tries to find the version of the package by looking for a version string in the metadata file or in the egg/wheel metadata file, if the package has been installed. To use it
+
+```python
+from sdsstools.metadata import get_package_version
+
+__version__ = get_package_version(path=__file__, package_name='sdss-camera') or 'dev'
+```
+
+This will try to find and parse the version from the metadata file (we pass `__file__` to indicate where to start looking); if that fails, it will try to get the version from the installed package `sdss-camera`. If all fails, it will set the fallback version `'dev'`.
+
+## Command Line Interface
+
+`sdsstools` provides the command line tool `sdss`, which is just a thin wrapper around some commonly used [Invoke](https://www.pyinvoke.org/) tasks. `sdsstools` does not automatically install all the dependencies for the tasks, which need to be added manually.
+
+`sdss` provides the following tasks
+
+| Task | Options | Description |
+| --- | --- | --- |
+| clean | | Removes files produces during build and packaging. |
+| deploy | --test | Builds and deploys to PyPI (or the test server). Requires `twine` and `wheel`. |
+| install-deps | --extras | Installs dependencies from a `setup.cfg` file |
+| docs.build | --target | Builds the Sphinx documentation. Requires `Sphinx`. |
+| docs.show | --target | Shows the documentation in the browser. Requires `Sphinx`. |
+| docs.clean | --target | Cleans the documentation build. Requires `Sphinx`. |
+
+`sdss` assumes that the documentation lives in `docs/sphinx` relative to the root of the repository. This can be changed by setting the `sphinx.target` configuration in an `invoke.yaml` file, for example
+
+```yaml
+sphinx:
+    target: docs
+```
+
+## Click daemon command
+
+The [daemonizer](src/sdsstools/daemonizer.py) module implements a [Click](https://palletsprojects.com/p/click/) command group that allows to spawn a daemon, and to stop and restart it. Internally the module uses [daemonocle](https://github.com/jnrbsn/daemonocle) (the package is not installed with `sdsstools` and needs to be pip-installed manually).
+
+A simple example of how to use `daemonizer` is
+
+```python
+import time
+import click
+from sdsstools.daemonizer import DaemonGroup
+
+@click.group(cls=DaemonGroup, prog='hello', pidfile='/var/tmp/hello.pid')
+@click.argument('NAME', type=str)
+@click.option('--file', type=str, default='hello.dat')
+def daemon(name):
+
+    with open(file, 'w') as unit:
+        while True:
+            unit.write(f'Hi {name}!\n')
+            unit.flush()
+            time.sleep(1)
+
+if __name__ == '__main__':
+    daemon()
+```
+
+This will create a new group `hello` with four subcommands
+
+```console
+Usage: daemon [OPTIONS] NAME COMMAND [ARGS]...
+
+Options:
+  --file
+  --help  Show this message and exit.
+
+Commands:
+  restart  Restart the daemon.
+  start    Start the daemon.
+  status   Report if the daemon is running.
+  stop     Stop the daemon.
+```
+
+Now we can run `daemon --file ~/hello.dat John start` and a new background process will start, writing to the file every second. We can stop it with `daemon stop`. In general the behaviour is identical to the [daemonocle Click implementation](https://github.com/jnrbsn/daemonocle#integration-with-mitsuhiko-s-click) but the internal are slightly different to allow the group callback to accept arguments. If the callback is a coroutine, it can be wrapped with the `cli_coro` decorator
+
+```python
+import asyncio
+import signal
+import click
+from sdsstools.daemonizer import DaemonGroup, cli_coro
+
+def shutdown(signal):
+    if signal == signal.SIGTERM:
+        cancel_something()
+
+@click.group(cls=DaemonGroup, prog='hello', pidfile='/var/tmp/hello.pid')
+@click.argument('NAME', type=str)
+@click.option('--file', type=str, default='hello.dat')
+@cli_coro(shutdown_func=shutdown, signals=(signal.SIGTERM, signal.SIGINT))
+async def daemon(name):
+
+    with open(file, 'w') as unit:
+        while True:
+            unit.write(f'Hi {name}!\n')
+            unit.flush()
+            await asyncio.sleep(1)
+```
+
+`cli_coro` can accept a `shutdown_func` function that is called when the coroutine receives a signal. The default signals handled are `(SIGHUP, SIGTERM, SIGINT)`.
+
+### Daemonizing a command
+
+To execute any command as a daemon you can use the `daemonize` script that is installed with `sdsstools`. To start the process as a daemon do `daemonize start NAME COMMAND` when `NAME` is the name associated to the daemon (so that it can be stopped later) and `COMMAND` is the command to run, for example:
+
+```console
+daemonize start apoActor python ./apoActor_main.py
+```
+
+To stop the daemon do `daemonize stop NAME`. See `daemonize --help` for more options.
+
+## Date functions
+
+The function `sdsstools.time.get_sjd()` returns the integer with the SDSS-style Modified Julian Day. The function accepts an observatory (`'APO'` or `'LCO'`) but otherwise will try to determine the current location from environment variables or the fully qualified domain name.
+
+## Bundled packages
+
+For convenience, `sdsstools` bundles the following products:
+
+- A copy of [releases](https://github.com/bitprophet/releases) that fixes some issues with recent versions of `semantic-version`. This copy is not available in `sdsstools>=1.0.0`. `releases` is not maintained anymore, so use at your own risk.
+- A copy of [toml](https://github.com/uiri/toml) to read TOML files (used by the metadata submodule).
+
+You can access them directly from the top-level namespace, `sdsstools.toml`, `sdsstools.releases`. To use `releases` with sphinx, simply add the following to your `config.py`
+
+```python
+extensions += ['sdsstools.releases']
+```
 
-setup(**setup_kwargs)
```

