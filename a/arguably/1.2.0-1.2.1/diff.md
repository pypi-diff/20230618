# Comparing `tmp/arguably-1.2.0.tar.gz` & `tmp/arguably-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arguably-1.2.0.tar", max compression
+gzip compressed data, was "arguably-1.2.1.tar", max compression
```

## Comparing `arguably-1.2.0.tar` & `arguably-1.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1538 2023-06-16 21:30:05.237718 arguably-1.2.0/LICENSE.txt
--rw-r--r--   0        0        0     2455 2023-06-16 21:30:05.237718 arguably-1.2.0/arguably/__init__.py
--rw-r--r--   0        0        0     2074 2023-06-16 21:30:05.237718 arguably-1.2.0/arguably/__main__.py
--rw-r--r--   0        0        0    14402 2023-06-16 21:30:05.237718 arguably-1.2.0/arguably/_argparse_extensions.py
--rw-r--r--   0        0        0     9794 2023-06-16 21:30:05.237718 arguably-1.2.0/arguably/_commands.py
--rw-r--r--   0        0        0    38301 2023-06-16 21:30:05.237718 arguably-1.2.0/arguably/_context.py
--rw-r--r--   0        0        0     9268 2023-06-16 21:30:05.237718 arguably-1.2.0/arguably/_modifiers.py
--rw-r--r--   0        0        0    14144 2023-06-16 21:30:05.237718 arguably-1.2.0/arguably/_util.py
--rw-r--r--   0        0        0        0 2023-06-16 21:30:05.237718 arguably-1.2.0/arguably/py.typed
--rw-r--r--   0        0        0     7121 2023-06-16 21:30:05.241718 arguably-1.2.0/etc/pypi/PYPI_README.md
--rw-r--r--   0        0        0     1135 2023-06-16 21:30:05.241718 arguably-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     7884 1970-01-01 00:00:00.000000 arguably-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1538 2023-06-18 21:45:39.713756 arguably-1.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     2455 2023-06-18 21:45:39.713756 arguably-1.2.1/arguably/__init__.py
+-rw-r--r--   0        0        0     2074 2023-06-18 21:45:39.713756 arguably-1.2.1/arguably/__main__.py
+-rw-r--r--   0        0        0    14402 2023-06-18 21:45:39.713756 arguably-1.2.1/arguably/_argparse_extensions.py
+-rw-r--r--   0        0        0     9972 2023-06-18 21:45:39.713756 arguably-1.2.1/arguably/_commands.py
+-rw-r--r--   0        0        0    38301 2023-06-18 21:45:39.713756 arguably-1.2.1/arguably/_context.py
+-rw-r--r--   0        0        0     9310 2023-06-18 21:45:39.713756 arguably-1.2.1/arguably/_modifiers.py
+-rw-r--r--   0        0        0    14487 2023-06-18 21:45:39.713756 arguably-1.2.1/arguably/_util.py
+-rw-r--r--   0        0        0        0 2023-06-18 21:45:39.713756 arguably-1.2.1/arguably/py.typed
+-rw-r--r--   0        0        0     6847 2023-06-18 21:45:39.721756 arguably-1.2.1/etc/pypi/PYPI_README.md
+-rw-r--r--   0        0        0     1129 2023-06-18 21:45:39.721756 arguably-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7604 1970-01-01 00:00:00.000000 arguably-1.2.1/PKG-INFO
```

### Comparing `arguably-1.2.0/LICENSE.txt` & `arguably-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arguably-1.2.0/arguably/__init__.py` & `arguably-1.2.1/arguably/__init__.py`

 * *Files identical despite different names*

### Comparing `arguably-1.2.0/arguably/__main__.py` & `arguably-1.2.1/arguably/__main__.py`

 * *Files identical despite different names*

### Comparing `arguably-1.2.0/arguably/_argparse_extensions.py` & `arguably-1.2.1/arguably/_argparse_extensions.py`

 * *Files identical despite different names*

### Comparing `arguably-1.2.0/arguably/_commands.py` & `arguably-1.2.1/arguably/_commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import asyncio
 import enum
 import inspect
 from dataclasses import dataclass, field
 from typing import Callable, Any, Union, Optional, List, Dict, Tuple
 
 import arguably._modifiers as mods
 import arguably._util as util
@@ -231,15 +232,18 @@
                 args.append(filtered_args[arg.cli_arg_name])
             elif arg.input_method.is_positional and arg.is_variadic:
                 args.extend(filtered_args[arg.cli_arg_name])
             else:
                 kwargs[arg.func_arg_name] = filtered_args[arg.func_arg_name]
 
         # Call the function
-        return self.function(*args, **kwargs)
+        if util.is_async_callable(self.function):
+            return asyncio.get_event_loop().run_until_complete(self.function(*args, **kwargs))
+        else:
+            return self.function(*args, **kwargs)
 
     def get_subcommand_metavar(self, command_metavar: str) -> str:
         """If this command has a subparser (for subcommands of its own), this can be called to generate a unique name
         for the subparser's command metavar"""
         if self.name == "__root__":
             return command_metavar
         return f"{self.name.replace(' ', '_')}{'_' if len(self.name) > 0 else ''}{command_metavar}"
```

### Comparing `arguably-1.2.0/arguably/_context.py` & `arguably-1.2.1/arguably/_context.py`

 * *Files identical despite different names*

### Comparing `arguably-1.2.0/arguably/_modifiers.py` & `arguably-1.2.1/arguably/_modifiers.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,19 +196,19 @@
         Examples:
             ```python
             def main(*, opt: Annotated[str, arguably.arg.missing("omit-val")] = "no-flag"):
                 print(opt)
             ```
 
             ```shell
-            $ ./test.py
+            user@machine:~$ ./test.py
             no-flag
-            $ ./test.py --opt input
+            user@machine:~$ ./test.py --opt input
             input
-            $ ./test.py --opt
+            user@machine:~$ ./test.py --opt
             omit-val
             ```
 
         Args:
             omit_value: The value that will be used if the flag is present, but the value is omitted.
 
         Returns:
```

### Comparing `arguably-1.2.0/arguably/_util.py` & `arguably-1.2.1/arguably/_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
 import ast
+import asyncio
 import enum
+import functools
 import importlib.util
 import inspect
 import logging
 import math
 import multiprocessing
 import re
 import sys
@@ -32,14 +34,21 @@
     class UnionType:
         """Stub this out, we only use it for issubclass() checks"""
 
 
 logger = logging.getLogger("arguably")
 
 
+def is_async_callable(obj: Any) -> bool:
+    """Checks if an object is an async callable - https://stackoverflow.com/a/72682939"""
+    while isinstance(obj, functools.partial):
+        obj = obj.func
+    return asyncio.iscoroutinefunction(obj) or (callable(obj) and asyncio.iscoroutinefunction(obj.__call__))
+
+
 def split_unquoted(unsplit: str, delimeter: str, limit: Union[int, float] = math.inf) -> List[str]:
     """Splits text at a delimiter, as long as that delimiter is not quoted (either single ' or double quotes ")."""
     assert len(delimeter) == 1
     assert limit > 0
     result = list()
     quote_char = None
     accumulator: List[str] = list()
```

### Comparing `arguably-1.2.0/etc/pypi/PYPI_README.md` & `arguably-1.2.1/etc/pypi/PYPI_README.md`

 * *Files 4% similar despite different names*

```diff
@@ -74,21 +74,16 @@
 | positional args, with default `not_required=2` | positional CLI args, optional `[not-required]` |
 | positional args, variadic `*others`            | any extra positional CLI args `[others ...]`   |
 | keyword-only arguments `option`                | command-line options `[-x OPTION]`             |
 
 `arguably` uses your docstrings to automatically generate help messages. It supports all major formats for docstrings:
 reStructuredText, Google, Numpydoc, and Epydoc.
 
-Type annotations are optional, but `arguably` can use them to automatically convert arguments to their type. It has
-smart handling for a few built-in types:
-
-* `tuple` is comma-separated: `tuple[str,float]` &rightarrow; `foo,2.0`
-* `list` is like `tuple`, but `--option`s can be repeated: `nums: list[int]` &rightarrow; `--nums 1 --nums 2`
-* `enum.Enum` takes lowercase enum item names, like `read` or `write`
-* `enum.Flag` is like `enum.Enum`, but values can be specified multiple times: `-r -w -x`
+Type annotations are optional, but `arguably` can use them to automatically convert arguments. It has smart handling for
+mapping built-in types to the command line, including `tuple`, `list`, `enum.Enum`, and `enum.Flag`.
 
 There are also a few special behaviors you can attach to a parameter via `Annotated[]` and the `arguably.arg.*`
 functions. Using `arguably.arg.builder()`, you can even build an object to pass in from the command line (using syntax
 inspired by QEMU):
 
 <div align="right"><sub>
     <a href="https://github.com/treykeown/arguably/blob/main/etc/scripts/readme-2.py">[source]</a>
@@ -126,16 +121,16 @@
 ## Installation
 
 Install using `pip install arguably`. If you want to install using `conda`, please comment on
 [this issue](https://github.com/treykeown/arguably/issues/12).
 
 ## Documentation
 
-* All-in-one Example: [https://treykeown.github.io/arguably/example/](https://treykeown.github.io/arguably/example/)
-* Tutorial: [https://treykeown.github.io/arguably/tutorial/](https://treykeown.github.io/arguably/tutorial/)
+* Examples: [https://treykeown.github.io/arguably/examples/](https://treykeown.github.io/arguably/examples/)
+* Tutorial: [https://treykeown.github.io/arguably/tutorial/intro/](https://treykeown.github.io/arguably/tutorial/intro/)
 * API Reference: [https://treykeown.github.io/arguably/api-reference/](https://treykeown.github.io/arguably/api-reference/)
 
 ## Dependencies
 
 All of `arguably` is built on top of `argparse`. It has two dependencies:
 
 * `docstring-parser` for parsing function docstrings
@@ -144,15 +139,15 @@
 ## Contributing
 
 Ideas and help are very much appreciated! There's a guide for getting started with contributing to `arguably` that shows
 you how to run tests and pre-commit hooks.
 
 * Contributing: [https://treykeown.github.io/arguably/contributing/](https://treykeown.github.io/arguably/contributing/)
 
-## Future Roadmap
+## Future roadmap
 
 If you have any interest in these (either as a user or implementer), please leave a comment!
 
 * [#8 - Display all enum options in a command group](https://github.com/treykeown/arguably/issues/8)
 * [#9 - Both positive and negative boolean flags](https://github.com/treykeown/arguably/issues/9)
 * [#10 - Take inputs from environment variables](https://github.com/treykeown/arguably/issues/10)
 * [#13 - Load configuration for a script via a `.yml`](https://github.com/treykeown/arguably/issues/13)
```

### Comparing `arguably-1.2.0/pyproject.toml` & `arguably-1.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "arguably"
-version = "1.2.0"
-description = "turns functions into command line interfaces"
+version = "1.2.1"
+description = "The best Python CLI library, arguably."
 authors = ["treykeown <2755914+treykeown@users.noreply.github.com>"]
 readme = "etc/pypi/PYPI_README.md"
 homepage = "https://treykeown.github.io/arguably/"
 repository = "https://github.com/treykeown/arguably"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `arguably-1.2.0/PKG-INFO` & `arguably-1.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: arguably
-Version: 1.2.0
-Summary: turns functions into command line interfaces
+Version: 1.2.1
+Summary: The best Python CLI library, arguably.
 Home-page: https://treykeown.github.io/arguably/
 Author: treykeown
 Author-email: 2755914+treykeown@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -92,21 +92,16 @@
 | positional args, with default `not_required=2` | positional CLI args, optional `[not-required]` |
 | positional args, variadic `*others`            | any extra positional CLI args `[others ...]`   |
 | keyword-only arguments `option`                | command-line options `[-x OPTION]`             |
 
 `arguably` uses your docstrings to automatically generate help messages. It supports all major formats for docstrings:
 reStructuredText, Google, Numpydoc, and Epydoc.
 
-Type annotations are optional, but `arguably` can use them to automatically convert arguments to their type. It has
-smart handling for a few built-in types:
-
-* `tuple` is comma-separated: `tuple[str,float]` &rightarrow; `foo,2.0`
-* `list` is like `tuple`, but `--option`s can be repeated: `nums: list[int]` &rightarrow; `--nums 1 --nums 2`
-* `enum.Enum` takes lowercase enum item names, like `read` or `write`
-* `enum.Flag` is like `enum.Enum`, but values can be specified multiple times: `-r -w -x`
+Type annotations are optional, but `arguably` can use them to automatically convert arguments. It has smart handling for
+mapping built-in types to the command line, including `tuple`, `list`, `enum.Enum`, and `enum.Flag`.
 
 There are also a few special behaviors you can attach to a parameter via `Annotated[]` and the `arguably.arg.*`
 functions. Using `arguably.arg.builder()`, you can even build an object to pass in from the command line (using syntax
 inspired by QEMU):
 
 <div align="right"><sub>
     <a href="https://github.com/treykeown/arguably/blob/main/etc/scripts/readme-2.py">[source]</a>
@@ -144,16 +139,16 @@
 ## Installation
 
 Install using `pip install arguably`. If you want to install using `conda`, please comment on
 [this issue](https://github.com/treykeown/arguably/issues/12).
 
 ## Documentation
 
-* All-in-one Example: [https://treykeown.github.io/arguably/example/](https://treykeown.github.io/arguably/example/)
-* Tutorial: [https://treykeown.github.io/arguably/tutorial/](https://treykeown.github.io/arguably/tutorial/)
+* Examples: [https://treykeown.github.io/arguably/examples/](https://treykeown.github.io/arguably/examples/)
+* Tutorial: [https://treykeown.github.io/arguably/tutorial/intro/](https://treykeown.github.io/arguably/tutorial/intro/)
 * API Reference: [https://treykeown.github.io/arguably/api-reference/](https://treykeown.github.io/arguably/api-reference/)
 
 ## Dependencies
 
 All of `arguably` is built on top of `argparse`. It has two dependencies:
 
 * `docstring-parser` for parsing function docstrings
@@ -162,15 +157,15 @@
 ## Contributing
 
 Ideas and help are very much appreciated! There's a guide for getting started with contributing to `arguably` that shows
 you how to run tests and pre-commit hooks.
 
 * Contributing: [https://treykeown.github.io/arguably/contributing/](https://treykeown.github.io/arguably/contributing/)
 
-## Future Roadmap
+## Future roadmap
 
 If you have any interest in these (either as a user or implementer), please leave a comment!
 
 * [#8 - Display all enum options in a command group](https://github.com/treykeown/arguably/issues/8)
 * [#9 - Both positive and negative boolean flags](https://github.com/treykeown/arguably/issues/9)
 * [#10 - Take inputs from environment variables](https://github.com/treykeown/arguably/issues/10)
 * [#13 - Load configuration for a script via a `.yml`](https://github.com/treykeown/arguably/issues/13)
```

