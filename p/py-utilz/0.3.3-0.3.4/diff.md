# Comparing `tmp/py_utilz-0.3.3.tar.gz` & `tmp/py_utilz-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_utilz-0.3.3.tar", max compression
+gzip compressed data, was "py_utilz-0.3.4.tar", max compression
```

## Comparing `py_utilz-0.3.3.tar` & `py_utilz-0.3.4.tar`

### file list

```diff
@@ -1,33 +1,29 @@
--rw-r--r--   0        0        0     1067 2022-12-09 22:53:50.675909 py_utilz-0.3.3/LICENSE
--rw-r--r--   0        0        0     2204 2022-12-09 22:53:50.675909 py_utilz-0.3.3/README.md
--rw-r--r--   0        0        0      867 2022-12-09 22:53:50.679909 py_utilz-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      196 2022-12-09 22:53:50.679909 py_utilz-0.3.3/utilz/__init__.py
--rw-r--r--   0        0        0      754 2022-12-09 22:53:50.679909 py_utilz-0.3.3/utilz/_utils.py
--rw-r--r--   0        0        0     2419 2022-12-09 22:53:50.679909 py_utilz-0.3.3/utilz/boilerplate.py
--rw-r--r--   0        0        0     5645 2022-12-09 22:53:50.679909 py_utilz-0.3.3/utilz/decorators.py
--rw-r--r--   0        0        0     9423 2022-12-09 22:53:50.679909 py_utilz-0.3.3/utilz/dftools.py
--rw-r--r--   0        0        0       62 2022-12-09 22:53:50.679909 py_utilz-0.3.3/utilz/dfverbs/__init__.py
--rw-r--r--   0        0        0     4888 2022-12-09 22:53:50.679909 py_utilz-0.3.3/utilz/dfverbs/plot.py
--rw-r--r--   0        0        0     6230 2022-12-09 22:53:50.679909 py_utilz-0.3.3/utilz/dfverbs/stats.py
--rw-r--r--   0        0        0    18839 2022-12-09 22:53:50.679909 py_utilz-0.3.3/utilz/dfverbs/verbs.py
--rw-r--r--   0        0        0     4856 2022-12-09 22:53:50.679909 py_utilz-0.3.3/utilz/io.py
--rw-r--r--   0        0        0    89664 2022-12-09 22:53:50.679909 py_utilz-0.3.3/utilz/jquery-3.6.1.min.js
--rw-r--r--   0        0        0    18369 2022-12-09 22:53:50.683909 py_utilz-0.3.3/utilz/jquery.dataTables.min.css
--rw-r--r--   0        0        0    90265 2022-12-09 22:53:50.683909 py_utilz-0.3.3/utilz/jquery.dataTables.min.js
--rw-r--r--   0        0        0    16159 2022-12-09 22:53:50.683909 py_utilz-0.3.3/utilz/maps.py
--rw-r--r--   0        0        0    17319 2022-12-09 22:53:50.683909 py_utilz-0.3.3/utilz/ops.py
--rw-r--r--   0        0        0        0 2022-12-09 22:53:50.683909 py_utilz-0.3.3/utilz/pipeline.py
--rw-r--r--   0        0        0     9662 2022-12-09 22:53:50.683909 py_utilz-0.3.3/utilz/plot.py
--rw-r--r--   0        0        0      767 2022-12-09 22:53:50.683909 py_utilz-0.3.3/utilz/shorts.py
--rw-r--r--   0        0        0      921 2022-12-09 22:53:50.683909 py_utilz-0.3.3/utilz/stats.py
--rw-r--r--   0        0        0      195 2022-12-09 22:53:50.683909 py_utilz-0.3.3/utilz/tests/conftest.py
--rw-r--r--   0        0        0     1783 2022-12-09 22:53:50.683909 py_utilz-0.3.3/utilz/tests/mtcars.csv
--rw-r--r--   0        0        0      741 2022-12-09 22:53:50.683909 py_utilz-0.3.3/utilz/tests/test_boilerplate.py
--rw-r--r--   0        0        0     5513 2022-12-09 22:53:50.683909 py_utilz-0.3.3/utilz/tests/test_decorators.py
--rw-r--r--   0        0        0     5199 2022-12-09 22:53:50.683909 py_utilz-0.3.3/utilz/tests/test_dftools.py
--rw-r--r--   0        0        0    13776 2022-12-09 22:53:50.683909 py_utilz-0.3.3/utilz/tests/test_dfverbs.py
--rw-r--r--   0        0        0     3487 2022-12-09 22:53:50.683909 py_utilz-0.3.3/utilz/tests/test_io.py
--rw-r--r--   0        0        0    17167 2022-12-09 22:53:50.683909 py_utilz-0.3.3/utilz/tests/test_ops.py
--rw-r--r--   0        0        0     1437 2022-12-09 22:53:50.683909 py_utilz-0.3.3/utilz/tests/test_plot.py
--rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 py_utilz-0.3.3/setup.py
--rw-r--r--   0        0        0     3056 1970-01-01 00:00:00.000000 py_utilz-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-18 00:29:07.997893 py_utilz-0.3.4/LICENSE
+-rw-r--r--   0        0        0     2211 2023-06-18 00:29:07.997893 py_utilz-0.3.4/README.md
+-rw-r--r--   0        0        0      818 2023-06-18 00:29:08.001893 py_utilz-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      196 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/__init__.py
+-rw-r--r--   0        0        0      754 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/_utils.py
+-rw-r--r--   0        0        0     2419 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/boilerplate.py
+-rw-r--r--   0        0        0     5387 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/decorators.py
+-rw-r--r--   0        0        0     9423 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/dftools.py
+-rw-r--r--   0        0        0       62 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/dfverbs/__init__.py
+-rw-r--r--   0        0        0     4922 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/dfverbs/plot.py
+-rw-r--r--   0        0        0     6230 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/dfverbs/stats.py
+-rw-r--r--   0        0        0    18857 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/dfverbs/verbs.py
+-rw-r--r--   0        0        0     5945 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/io.py
+-rw-r--r--   0        0        0    16218 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/maps.py
+-rw-r--r--   0        0        0    14804 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/ops.py
+-rw-r--r--   0        0        0        0 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/pipeline.py
+-rw-r--r--   0        0        0     9664 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/plot.py
+-rw-r--r--   0        0        0     1003 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/shorts.py
+-rw-r--r--   0        0        0      921 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/stats.py
+-rw-r--r--   0        0        0      195 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/tests/conftest.py
+-rw-r--r--   0        0        0     1783 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/tests/mtcars.csv
+-rw-r--r--   0        0        0      741 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/tests/test_boilerplate.py
+-rw-r--r--   0        0        0     5604 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/tests/test_decorators.py
+-rw-r--r--   0        0        0     5195 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/tests/test_dftools.py
+-rw-r--r--   0        0        0    13773 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/tests/test_dfverbs.py
+-rw-r--r--   0        0        0     3994 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/tests/test_io.py
+-rw-r--r--   0        0        0    17078 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/tests/test_ops.py
+-rw-r--r--   0        0        0     1436 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/tests/test_plot.py
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 py_utilz-0.3.4/PKG-INFO
```

### Comparing `py_utilz-0.3.3/LICENSE` & `py_utilz-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py_utilz-0.3.3/README.md` & `py_utilz-0.3.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Utilz
-![Build Status](https://github.com/ejolly/utilz/workflows/Utilz/badge.svg)
+# py-utilz
+
+![Build Status](https://github.com/ejolly/py-utilz/workflows/Utilz/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/ejolly/utilz/badge.svg?branch=master)](https://coveralls.io/github/ejolly/utilz?branch=master)
 ![Python Versions](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
 ![Platforms](https://img.shields.io/badge/platform-linux%20%7C%20osx%20%7C%20win-blue)
 
 Convenient helper functions, decorators, and data analysis tools to make life easier with minimal dependencies:
 
 `pip install py-utilz`
 
 [dplyr](https://dplyr.tidyverse.org/) like data grammar:
 
-
 ```python
 from utilz import pipe
 import utilz.dfverbs as _
 
 out = pipe(
     df,
     _.rename({"weight (male, lbs)": "male", "weight (female, lbs)": "female"}),
@@ -26,21 +26,21 @@
     _.mutate(weight="weight.mean()"),
     _.pivot_wider(column="sex", using="weight"),
     _.mutate(dimorphism="male / female")
 )
 ```
 
 ```python
-from utilz import mapcat
+from utilz import map
 
 # Combine function results into a list, array, or dataframe
-mapcat(myfunc, myiterable) 
+map(myfunc, myiterable)
 
 # Syntactic sugar for joblib.Parallel
-mapcat(myfunc, myiterable, n_jobs=4)
+map(myfunc, myiterable, n_jobs=4)
 ```
 
 ```python
 from utilz import log, maybe
 
 # Print the shape of args and outputs before and after execute
 @log
@@ -49,21 +49,21 @@
 
 # Only run myfunc if results.csv doesn't eist
 @maybe('results.csv')
 def myfunc(args):
     return out
 ```
 
-
 ## Development
 
 1. Install [poetry](https://python-poetry.org/): `curl -sSL https://install.python-poetry.org | python`
-2. Setup virtual environment `poetry install`
+2. Setup virtual environment `poetry install --with dev`
 3. Run all tests: `poetry run pytest`
 4. Live render docs: `poetry run mkdocs serve`
 
 ### Additional poetry/virtual environment commands
+
 - Activate environment in current shell: `source activate .venv/bin/activate`
 - Activate environment in sub-process shell: `poetry shell`
 - Add/remove additional packages: `poetry add/remove package_name`
 - Build local package: `poetry build`
 - Deploy to pypi: `poetry publish` (requires auth)
```

### Comparing `py_utilz-0.3.3/utilz/_utils.py` & `py_utilz-0.3.4/utilz/_utils.py`

 * *Files identical despite different names*

### Comparing `py_utilz-0.3.3/utilz/boilerplate.py` & `py_utilz-0.3.4/utilz/boilerplate.py`

 * *Files identical despite different names*

### Comparing `py_utilz-0.3.3/utilz/decorators.py` & `py_utilz-0.3.4/utilz/decorators.py`

 * *Files 14% similar despite different names*

```diff
@@ -122,59 +122,59 @@
         time_taken = str(dt.datetime.now() - tic)
         print(f"{func.__name__}, took {time_taken}s")
         return result
 
     return wrapper
 
 
-def maybe(
-    fpath: Union[str, Path],
-    loadfunc: Union[Callable, None] = None,
-    force: bool = False,
-    as_arr: bool = False,
-    as_str: bool = False,
-    verbose: bool = False,
-    **kwargs,
-) -> Any:
+def maybe(function):
     """
-    Run the decorated `func` only if `fpath` doesn't exist or if it isn't an empty
-    directory. If `fpath` exists will load the file from disk or if `fpath` is a directory,
-    will return the results of globbing the directory for all files
-
-    Args:
-        fpath (Path/str): filename or dirname to check existence for
-        force (bool, optional): always run the function even if filepath exists,
-        possibly overwriting filepath (based on whatever func does internally). Defaults
-        to False.
-        as_arr (bool, optional): treat a .txt file as a numpy array;
-        Default False
-        as_str (bool, optional): open txt/json as a single string instead of
-        splitting on newlines; Default False
-        verbose (bool, optional): whether to print messages during load. Default False
+    A decorator that wraps a function which should take a kwarg called `out_file`. If
+    `out_file` exists then it's loaded from disk, otherwise the wrapped function is
+    called. If the wrapped function takes a kwarg `overwrite = True` then it always runs. You can also pass `loader_func = callable` to use a custom loading function
+
+    Example:
+
+    >>> @maybe
+    >>> def mean_brain(subpath, **kwargs):
+    >>> b = Brain_Data(subpath)
+    >>> m = b.mean()
+    >>> out_file = kwargs.get('out_file')
+    >>> m.write(out_file)
+    >>> return m
+
+    >>> mean_brain(subpath, out_file='mean_brain.h5', loader_func=Brain_Data)
+
     """
 
-    def decorator(func):
-        @wraps(func)
-        def wrapper(*args, **kwargs):
-            if not force and fpath.exists():
-                if fpath.is_file() or (fpath.is_dir() and any(fpath.iterdir())):
-                    print(f"Exists: loading previously saved file: {fpath}")
-                    if loadfunc is not None:
-                        return loadfunc(fpath, **kwargs)
-                    return load(
-                        fpath,
-                        as_str=as_str,
-                        as_arr=as_arr,
-                        verbose=verbose,
-                    )
-            return func(*args, **kwargs)
+    @wraps(function)
+    def wrapper(*args, **kwargs):
+        # get out_file from the wrapped function
+        out_file = kwargs.get("out_file", None)
+
+        # get out_file from the wrapped function
+        overwrite = kwargs.get("overwrite", False)
+
+        if out_file is None:
+            raise ValueError(
+                "out_file must be provided as a kwarg to the decorated function!"
+            )
+
+        out_file = Path(out_file)
+
+        if out_file.exists() and not overwrite:
+            print(f"Loading precomputed result from: {out_file}")
+            load_kwargs = {
+                k: v for k, v in kwargs.items() if k not in ["out_file", "overwrite"]
+            }
+            return load(out_file, **load_kwargs)
 
-        return wrapper
+        return function(*args, **kwargs)
 
-    return decorator
+    return wrapper
 
 
 def expensive(
     force: bool = False,
 ) -> Any:
     """
     A decorator that wraps `joblib.Memory` for caching the results of a function to disk.
```

### Comparing `py_utilz-0.3.3/utilz/dftools.py` & `py_utilz-0.3.4/utilz/dftools.py`

 * *Files identical despite different names*

### Comparing `py_utilz-0.3.3/utilz/dfverbs/plot.py` & `py_utilz-0.3.4/utilz/dfverbs/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,15 +277,16 @@
 
 
 @curry
 def stripbarplot(**kwargs):
     """Call to combined stripplot and barplot. See utilz.plot.stripbarplot"""
 
     def plot(data):
-        return _stripbarplot(data=data, ax="newax", **kwargs)
+        ax = kwargs.pop("ax", "newax")
+        return _stripbarplot(data=data, ax=ax, **kwargs)
 
     return plot
 
 
 @curry
 def plot(*args, **kwargs):
     """Call a dataframe's .plot method"""
```

### Comparing `py_utilz-0.3.3/utilz/dfverbs/stats.py` & `py_utilz-0.3.4/utilz/dfverbs/stats.py`

 * *Files identical despite different names*

### Comparing `py_utilz-0.3.3/utilz/dfverbs/verbs.py` & `py_utilz-0.3.4/utilz/dfverbs/verbs.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     "squeeze",
     "to_numpy",
     "to_list",
     "ngroups",
     "get_group",
     "reset_index",
     "split_groups",
+    "assign",
 ]
 
 import pandas as pd
 from toolz import curry
 from ..ops import do
 from ..maps import filter
 
@@ -421,15 +422,16 @@
     return call
 
 
 @curry
 def select(*args):
     """
     Select one or more columns by name. Drop one or more columns by prepending '-' to
-    the name. **Always returns a dataframe** even if there is just 1 column. Does not support renaming"""
+    the name. **Always returns a dataframe** even if there is just 1 column. Does not support renaming
+    """
 
     def call(df):
         return do("select", df, *args)
 
     return call
 
 
@@ -487,15 +489,14 @@
         sep (str, list): separator to split on. Use [] for list
 
     """
 
     col, into = args
 
     def call(df):
-
         if isinstance(sep, str):
             out = df[col].str.split(sep, expand=True)
         elif isinstance(sep, list):
             out = pd.DataFrame(df[col].to_list())
         if len(into) != out.shape[1]:
             raise ValueError(
                 f"into has {len(into)} elements, but splitting creates a dataframe with {out.shape[1]} columns"
```

### Comparing `py_utilz-0.3.3/utilz/io.py` & `py_utilz-0.3.4/utilz/io.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 I/O Module
 """
 __all__ = ["load", "crawl"]
 from pathlib import Path
-from typing import Union, Any, List
+from typing import Union, Any, List, Callable
 import pandas as pd
 import numpy as np
 import pickle
 import json
 from warnings import warn
 from .ops import sort
 from .maps import mapcat, filter
@@ -17,54 +17,81 @@
 
 def load(
     f: Union[Path, str],
     as_arr: bool = False,
     as_str: bool = False,
     verbose: bool = False,
     glob: str = "*",
+    glob_sort: bool = True,
     assert_notempty: bool = True,
+    loader_func: Union[Callable, None] = None,
     **kwargs,
 ) -> Any:
     """
-    A handy dandy all-in-one loading function. Simply pass a Path object to a file (or a
-    string) and you'll back a python object based on the file-extension:
+    A handy dandy all-in-one loading function. Simply pass a Path object to a file or directory and you'll back a python object or list of objects based on the file-extension:
 
     - `.csv`: `pd.Dataframe`
     - `.p/.pickle`: output of `pickle.load`
     - `.json`: `str` or `dict`
+    - `.npy`: `np.ndarray`
     - `.txt`: `np.ndarray`, `list[str]` (lines a file), or `str` (all file contents)
     - other file-extensions are attempted to be loaded like `.txt` files
+    - if give a directory all files matching `glob` in that directory will be loaded
 
     Args:
         f (Path/str): name or path object to load
         as_arr (bool, optional): treat a .txt file as a numpy array;
         Default False
         as_str (bool, optional): open txt/json as a single string instead of
         splitting on newlines; Default False
         assert_notempty(bool, optional): make sure the output is not Falsey (e.g. empty
         array, dataframe, string, list); Default True
         verbose (bool, optional): whether to print messages during load. Default False
         **kwargs: keyword arguments to `pd.read_csv` or `np.loadtxt`
         glob (string, optional): globbing pattern if f is a directory. Defaults to all files
+        glob_sort (bool, optional): sort the globa before loadin. Defaults to True
         assert_notempty (bool, optional): raise an error if the returned output is
         empty; Default True
+        loader_func (callable, optional): a custom function to use for loading; Default None, uses file extension
 
     Returns:
-        the loaded object
+        the loaded object or list of objects
     """
 
     if isinstance(f, str):
         f = Path(f)
     if not isinstance(f, Path):
         raise TypeError("Input must be a string or Path object")
 
     if f.is_dir():
         out = list(f.glob(glob))
+        out = sorted(out) if glob_sort else out
+        # Recursively call load on each file in dir and forward args
+        out = [
+            load(
+                o,
+                as_arr=as_arr,
+                as_str=as_str,
+                verbose=verbose,
+                loader_func=loader_func,
+                assert_notempty=assert_notempty,
+                **kwargs,
+            )
+            for o in out
+        ]
 
-    # TODO: add support for np.save .npz files
+    elif loader_func is not None:
+        if verbose:
+            print("Using provided custom load function")
+        out = loader_func(str(f))
+
+    elif f.suffix == ".npy":
+        if verbose:
+            print("npy file - using numpy")
+        out = np.load(str(f), **kwargs)
 
     elif f.suffix == ".csv":
         if verbose:
             print("csv file - using pandas")
         out = pd.read_csv(str(f), **kwargs)
 
     elif f.suffix == ".p" or f.suffix == ".pickle":
```

### Comparing `py_utilz-0.3.3/utilz/maps.py` & `py_utilz-0.3.4/utilz/maps.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,27 +40,27 @@
 from itertools import filterfalse
 from copy import deepcopy
 
 
 MAX_INT = np.iinfo(np.int32).max
 _filter = filter  # we're overwriting the base func
 
+
 # Helper used by map
 def _pmap(
     func: Callable,
     iterme: Iterable,
     enum: bool = False,
     seeds: Union[None, list] = None,
     n_jobs: int = 1,
     backend: Union[None, str] = None,
     progressbar: bool = True,
     verbose: int = 0,
     func_kwargs: Union[None, dict] = None,
 ) -> Any:
-
     # Setup progress bars and parallelization
     if n_jobs < 1 or n_jobs > 1:
         # Initialize joblib parallelizer
         if progressbar:
             parfor = ProgressParallel(
                 prefer=backend, n_jobs=n_jobs, verbose=verbose, total=len(iterme)
             )
@@ -74,15 +74,14 @@
         if progressbar:
             iterme = tqdm(iterme)
 
         wrapped = func
 
     # Without enumeration
     if not enum:
-
         # Without random seeds
         if seeds is None:
             iterator = iterme
             if func_kwargs is None:
                 call_list = [wrapped(elem) for elem in iterator]
             else:
                 call_list = [wrapped(elem, **func_kwargs) for elem in iterator]
@@ -240,15 +239,16 @@
         op = _pmap(func, iterme, enum, seeds, n_jobs, backend, pbar, verbose, kwargs)
 
     return op
 
 
 @curry
 def mapcat(func: Union[Callable, None], iterme: Iterable, **kwargs):
-    """Call map and concatenate results after"""
+    """Call map and concatenate results after.
+    Particularly useful to ensure results are numpy arrays"""
 
     concat_axis = kwargs.pop("concat_axis", None)
     ignore_index = kwargs.pop("ignore_index", True)
     out = map(func, iterme, **kwargs)
 
     return concat(out, iterme, concat_axis, ignore_index)
```

### Comparing `py_utilz-0.3.3/utilz/ops.py` & `py_utilz-0.3.4/utilz/ops.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,107 +33,30 @@
     "do",
     "iffy",
     "compose",
     "curry",
     "pop",
     "nth",
     "check_random_state",
-    "datatable",
     "pairs",
 ]
 
-from ._utils import get_resource_path
 import numpy as np
 import pandas as pd
 from typing import Union, Any
 from collections.abc import Callable, Iterable
 from itertools import chain as it_chain
 import itertools as it
 from inspect import signature
 from toolz import curry, juxt
 from toolz.curried import compose_left as compose, nth
-from matplotlib.figure import Figure, Axes
-from matplotlib.axes._subplots import Subplot
 from inspect import signature
-from seaborn import FacetGrid, PairGrid
-from seaborn.matrix import ClusterGrid
-import uuid
-from warnings import warn
 from pathlib import Path
 
 
-@curry
-def datatable(df):
-    """Prints a pandas.DataFrame using the jQuery DataTable plugin"""
-    if not isinstance(df, pd.DataFrame):
-        warn("Not a pandas dataframe returning input...")
-        return df
-
-    try:
-        shell = get_ipython().__class__.__name__
-        if shell == "ZMQInteractiveShell":
-            from IPython.display import HTML
-
-            table_id = uuid.uuid1()
-            loc = get_resource_path()
-            if df.shape[0] > 500:
-                warn("df has more than 500 rows endering...")
-
-            output = f"""
-
-                <link rel="stylesheet" type="text/css" href="{loc}/jquery.dataTables.min.css">
-                
-                <script type="text/javascript">
-                    console.log('setting up requirejs imports...')
-
-                    require.config({{
-                        paths: {{
-                            jquery: '{loc}/jquery-3.6.1.min.js',
-                            datatables: '{loc}/jquery.datatables.min'
-                        }}
-                    }});
-
-                </script>
-
-                <div id='datatable-{table_id}'>
-
-                    {df.to_html(classes=f"datatable display compact")}
-
-                    <script type="text/javascript">
-                        $(document).ready( function () {{
-                            console.log('rendering interactive datatable...')
-
-                            require(['datatables'], function () {{
-
-                                    $('#datatable-{table_id}').find('table.datatable').dataTable();
-                            }});
-                        }});
-                    </script>
-
-                    <style>
-                        .dataTables_info, 
-                        .dataTables_wrapper label, 
-                        .dataTables_wrapper select,
-                        .dataTables_wrapper .dataTables_filter input,
-                        .dataTables_wrapper .dataTables_paginate .paginate_button {{
-                            color: #CCCAC2 !important;
-                        }}
-                    
-                    </style>
-
-                </div>
-
-            """
-            return HTML(output)
-        else:
-            return df
-    except NameError:
-        return df
-
-
 def check_random_state(seed=None):
     """Turn seed into a np.random.RandomState instance. Note: credit for this code goes entirely to `sklearn.utils.check_random_state`. Using the source here simply avoids an unecessary dependency.
 
     Args:
         seed (None, int, np.RandomState): if seed is None, return the RandomState singleton used by np.random. If seed is an int, return a new RandomState instance seeded with seed. If seed is already a RandomState instance, return it. Otherwise raise ValueError.
     """
 
@@ -332,15 +255,16 @@
 
     return call
 
 
 @curry
 def many(*args):
     """Apply many functions separately to a single input. Operates like the inverse of
-    map(). Whereas map takes applies 1 func to multiple elements, many applies multiple funcs to 1 element. Returns a tuple the same length as args containing the output of each function"""
+    map(). Whereas map takes applies 1 func to multiple elements, many applies multiple funcs to 1 element. Returns a tuple the same length as args containing the output of each function
+    """
 
     def call(data):
         if isinstance(data, (list, tuple)):
             raise TypeError(
                 f"Expected a single input but receive {len(data)}. Use mapmany() to operate on an iterable"
             )
         if len(args) <= 1:
@@ -443,15 +367,14 @@
         return tuple([f(a) for f, a in zip(args, data)])
 
     return call
 
 
 @curry
 def gather(func, data):
-
     if not (isinstance(data, (list, tuple)) and len(data) > 1):
         raise TypeError(
             f"gather expects the previous step's output to be a list/tuple of length > 1 but received a {type(data)}"
         )
 
     return func(*data)
```

### Comparing `py_utilz-0.3.3/utilz/plot.py` & `py_utilz-0.3.4/utilz/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
         title_params["loc"] = title_loc
     if title_fontsize is not None:
         title_params["fontsize"] = title_fontsize
 
     # Legend settings
     legend_params = dict()
     legend_params["loc"] = kwargs.pop("loc", "best")
-    legend_params["ncols"] = kwargs.pop("loc", 1)
+    legend_params["ncols"] = kwargs.pop("ncols", 1)
     legend_params["fontsize"] = kwargs.pop("fontsize", None)
     legend_params["title"] = kwargs.pop("legend_title", None)
     legend_params["title_fontsize"] = kwargs.pop("legend_title_fontsize", None)
     legend_params["fontsize"] = kwargs.pop("legend_labels_fontsize", None)
     legend_params["frameon"] = kwargs.pop("legend_frame", True)
     legend_labels = kwargs.pop("legend_labels", None)
     labels = labels if legend_labels is None else legend_labels
```

### Comparing `py_utilz-0.3.3/utilz/shorts.py` & `py_utilz-0.3.4/utilz/shorts.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,7 +25,17 @@
     """Enumerated `list`"""
     return list(range(n))
 
 
 def equal(*seqs):
     """Lazily checks if two sequences of potentionally different lengths are equal"""
     return not any(diff(*seqs, default=object()))
+
+
+def aslist(e):
+    """Idempotently convert something to a list."""
+    return [e] if not isinstance(e, list) else e
+
+
+def asstr(e):
+    """Idempotently convert something to a str."""
+    return str(e) if not isinstance(e, str) else e
```

### Comparing `py_utilz-0.3.3/utilz/stats.py` & `py_utilz-0.3.4/utilz/stats.py`

 * *Files identical despite different names*

### Comparing `py_utilz-0.3.3/utilz/tests/mtcars.csv` & `py_utilz-0.3.4/utilz/tests/mtcars.csv`

 * *Files identical despite different names*

### Comparing `py_utilz-0.3.3/utilz/tests/test_boilerplate.py` & `py_utilz-0.3.4/utilz/tests/test_boilerplate.py`

 * *Files identical despite different names*

### Comparing `py_utilz-0.3.3/utilz/tests/test_decorators.py` & `py_utilz-0.3.4/utilz/tests/test_decorators.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import pandas as pd
 import numpy as np
 from utilz.decorators import timeit, maybe, log, expensive, show
 from time import sleep, time
 from pathlib import Path
 from shutil import rmtree
 from joblib import Memory
-import pickle
+import pytest
+from utilz.io import load
+from utilz.shorts import equal
 
 
 def test_show(capsys, df):
     @show
     def f(x):
         return x
 
@@ -70,119 +72,107 @@
     _ = myfunc(df)
     captured = capsys.readouterr()
     assert "myfunc, took" in captured.out
     assert "3" in captured.out
 
 
 def test_maybe(tmp_path, capsys):
-    p = Path(f"{tmp_path}/test.csv")
-    if p.exists():
-        p.unlink()
+    temp_file = Path(f"{tmp_path}/test.csv")
+    if temp_file.exists():
+        temp_file.unlink()
 
     # Decorate a function that simulates running a computation that saves and returns a
     # dataframe
-    @maybe(p)
-    def f(save_to):
+    @maybe
+    def f(shape, **kwargs):
         print("I'm running")
-        df = pd.DataFrame(np.random.randn(5, 3))
-        df.to_csv(tmp_path.joinpath(save_to), index=False)
+        df = pd.DataFrame(np.random.randn(*shape))
+        save_path = kwargs.get("out_file")
+        df.to_csv(save_path, index=False)
         return df
 
     # First run: func executes and saves file
-    out = f("test.csv")
+    out = f((5, 3), out_file=temp_file)
     captured = capsys.readouterr()
     assert "I'm running" in captured.out
     assert isinstance(out, pd.DataFrame)
-    assert p.exists()
+    assert temp_file.exists()
 
     # Second run: just loads file
-    out_loaded = f("test.csv")
+    out_loaded = f((5, 3), out_file=temp_file)
     captured = capsys.readouterr()
     assert "I'm running" not in captured.out
-    assert "Exists: loading previously saved file" in captured.out
+    assert f"Loading precomputed result from: {temp_file}" in captured.out
     assert isinstance(out_loaded, pd.DataFrame)
-    assert p.exists()
+    assert temp_file.exists()
     assert np.allclose(out.to_numpy(), out_loaded.to_numpy())
 
-    # Force reruns by adding kwargs to the decorator
-    @maybe(p, force=True)
-    def f(save_to):
-        print("I'm running")
-        df = pd.DataFrame(np.random.randn(5, 3))
-        df.to_csv(tmp_path.joinpath(save_to), index=False)
-        return df
-
-    # Third run: func reruns and overwrites files
-    out_rerun = f("test.csv")
+    # Force a rerun with overwrite=True
+    out_rerun = f((5, 3), out_file=temp_file, overwrite=True)
     captured = capsys.readouterr()
     assert "I'm running" in captured.out
     assert isinstance(out_rerun, pd.DataFrame)
-    assert p.exists()
-    assert not np.allclose(out.to_numpy(), out_rerun.to_numpy())
+    assert temp_file.exists()
+    assert not np.allclose(out_loaded.to_numpy(), out_rerun.to_numpy())
+
+    # Missing out_file as a kwarg to decorated function raises error
+    with pytest.raises(ValueError):
+        f((5, 3))
 
     # Clean up
-    p.unlink()
+    temp_file.unlink()
 
     # Test with list of files
-    p = Path(f"{tmp_path}/myfiles")
-    p.mkdir()
+    temp_dir = Path(f"{tmp_path}/myfiles")
 
-    @maybe(p)
-    def f(p):
+    @maybe
+    def f(shape, **kwargs):
+        save_folder = kwargs.get("out_file")
+        save_folder.mkdir()
         print("I'm running")
-        out_files = []
+        out = []
         for i in range(3):
-            df = pd.DataFrame(np.random.randn(5, 3))
-            df.to_csv(p / f"{i}.csv", index=False)
-            out_files.append(df)
-        return out_files
+            df = pd.DataFrame(np.random.randn(*shape))
+            df.to_csv(save_folder / f"{i}.csv", index=False)
+            out.append(df)
+        return out
 
-    out_files = f(p)
+    # First run: func executes and saves multiple files to dir
+    out = f((5, 3), out_file=temp_dir)
     captured = capsys.readouterr()
     assert "I'm running" in captured.out
-    assert isinstance(out_files, list)
-    assert isinstance(out_files[0], pd.DataFrame)
+    assert isinstance(out, list)
+    assert isinstance(out[0], pd.DataFrame)
+    assert any(temp_dir.iterdir())
 
-    out_files = f(p)
+    # Second run: just loads files
+    out_loaded = f((5, 3), out_file=temp_dir)
     captured = capsys.readouterr()
     assert "I'm running" not in captured.out
-    assert "Exists: loading previously saved file" in captured.out
-    assert isinstance(out_files, list)
-    assert isinstance(out_files[0], Path)
-
-    # Test custom load
-    p = Path(f"{tmp_path}/test.p")
-
-    def myload(f):
-        print("custom load running!")
-        return pickle.load(open(f, "rb"))
+    assert f"Loading precomputed result from: {temp_dir}" in captured.out
+    assert isinstance(out_loaded, list)
+    assert len(list(temp_dir.iterdir()))
+    assert all(
+        np.allclose(one.to_numpy(), two.to_numpy()) for one, two in zip(out, out_loaded)
+    )
 
-    @maybe(p, loadfunc=myload)
-    def f(p):
-        print("I'm running")
-        pickle.dump(["hi"], open(p, "wb"))
+    # Passing custom loader works, in this case no-op to just get file names
+    custom_loader = lambda x: x
 
-    # First run: func executes and saves file
-    out = f(p)
-    captured = capsys.readouterr()
-    assert "I'm running" in captured.out
-    assert p.exists()
+    maybe_out_files = f((5, 3), out_file=temp_dir, loader_func=custom_loader)
 
-    # Second run: just loads file
-    out_loaded = f(p)
-    captured = capsys.readouterr()
-    # assert "I'm running" not in captured.out
-    assert "Exists: loading previously saved file" in captured.out
-    assert "custom load running!" in captured.out
+    # Equivalent to loading file names directly
+    out_files = load(temp_dir, loader_func=custom_loader)
 
-    p.unlink()
+    assert equal(maybe_out_files, out_files)
 
+    rmtree(temp_dir)
 
-def test_expensive(df, capsys):
 
+def test_expensive(df, capsys):
     memory = Memory("./cachedir")
     memory.clear()
 
     @expensive()
     def myfunc(df):
         print("Computing...")
         sleep(3)
```

### Comparing `py_utilz-0.3.3/utilz/tests/test_dftools.py` & `py_utilz-0.3.4/utilz/tests/test_dftools.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,25 +28,23 @@
 
     out = df.norm_by_group("species", "sepal_length", addcol=False)
     assert isinstance(out, pd.Series)
     assert len(out) == df.shape[0]
 
 
 def test_assert_balanced_groups(df):
-
     assert df.assert_balanced_groups("species")
 
     assert df.assert_balanced_groups("species", 50)
 
     with pytest.raises(AssertionError):
         df.iloc[:-1, :].assert_balanced_groups("species")
 
 
 def test_assert_same_nunique(df):
-
     with pytest.raises(AssertionError):
         assert df.assert_same_nunique("species", "sepal_length")
 
     _df = df.assign(val=list(range(10)) * 15)
     assert _df.assert_same_nunique("species", "val")
 
 
@@ -103,15 +101,14 @@
 
     # Dataframe has no unique method; only Series do
     with pytest.raises(AttributeError):
         dfg.unique()
 
 
 def test_pivot_longer(df):
-
     # No need to specify id_vars as the rest of the cols will be used by default
     long = df.pivot_longer(
         columns=["sepal_width", "sepal_length"], into=("sepal_dim", "inches")
     )
     assert long.shape[0] == df.shape[0] * 2
     assert long.sepal_dim.nunique() == 2
 
@@ -126,15 +123,14 @@
     long = df.pivot_longer(
         ["sepal_length", "sepal_width", "petal_length", "petal_width"],
         into=("dimension", "inches"),
     )
 
 
 def test_to_wide(df):
-
     # Generate long form data with no unique id column
     long = df.pivot_longer(
         ["sepal_length", "sepal_width", "petal_length", "petal_width"],
         into=("dimension", "inches"),
     )
     # Because we can't infer uniques there are duplicate possibilities so this fails
     with pytest.raises(ValueError):
```

### Comparing `py_utilz-0.3.3/utilz/tests/test_dfverbs.py` & `py_utilz-0.3.4/utilz/tests/test_dfverbs.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
     assert out.shape[0] < df.shape[0]
 
     out = pipe(df, _.query(lambda A1: A1 > x))
     assert out.shape[0] < df.shape[0]
 
 
 def test_mutate():
-
     df = randdf((20, 3))
     # Assign values directly
     out = pipe(df, _.mutate(group=["A"] * 10 + ["B"] * 10))
     assert "group" in out.columns
 
     # Or use str eval ops
     out = pipe(out, _.mutate(A1_doubled="A1 * 2"))
@@ -179,15 +178,14 @@
 
     df = randdf((20, 3), groups={"group": 4})
     out = pipe(df, _.groupby("group"), _.select("A1"), _.call("mean"))
     assert out.equals(df.groupby("group")["A1"].mean())
 
 
 def test_summarize():
-
     df = pd.read_csv("./utilz/tests/mtcars.csv")
 
     # str
     out = pipe(df, _.summarize(avg="mpg.mean()"))
     assert isinstance(out, pd.DataFrame)
     assert out.shape == (1, 1)
 
@@ -332,15 +330,14 @@
         out.groupby(["group", "school"])["B1"]
         .transform(lambda x: x - x.mean())
         .to_numpy(),
     )
 
 
 def test_sort():
-
     data = randdf((20, 3), groups={"condition": 2, "group": 4})
 
     out = pipe(data, _.sort("group", "condition", ascending=False))
     assert out.equals(
         data.sort_values(by=["group", "condition"], ascending=False, ignore_index=True)
     )
```

### Comparing `py_utilz-0.3.3/utilz/tests/test_io.py` & `py_utilz-0.3.4/utilz/tests/test_io.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     Creates several test data files:
     arr.txt, arr.gz, mydicts.json, mdictlist.json, h5.h5, pickle.p, df.csv, df.h5, df.hd5f
     """
 
     arr = np.random.randn(10)
     np.savetxt(tmp_path.joinpath("arr.txt"), arr)
     np.savetxt(tmp_path.joinpath("arr.gz"), arr)
+    np.save(tmp_path.joinpath("arr.npy"), arr)
+    np.save(tmp_path.joinpath("arr.npz"), arr)
 
     tmp_path.joinpath("txt.txt").write_text("hello world\nhello world")
 
     mydict = {"name": "Bob", "age": 1}
     with tmp_path.joinpath("mydict.json").open("w") as file_handle:
         json.dump(mydict, file_handle)
     tmp_path.joinpath("mydicts.json").write_text(json.dumps(mydict))
@@ -35,24 +37,20 @@
 
     df = pd.DataFrame(np.random.randn(10, 3), columns=["a", "b", "c"])
     df.to_csv(tmp_path.joinpath("df.csv"), index=False)
 
 
 @pytest.mark.usefixtures("setup_data")
 def test_load(tmp_path: Path):
-
     # Load csv
     out = load(tmp_path.joinpath("df.csv"))
     assert isinstance(out, pd.DataFrame)
     assert out.shape == (10, 3)
 
     # load txt
-    out = load(tmp_path.joinpath("arr.txt"), as_arr=True)
-    assert isinstance(out, np.ndarray)
-    assert len(out) == 10
     out = load(tmp_path.joinpath("txt.txt"))
     assert isinstance(out, list)
     assert len(out) == 2
     out = load(tmp_path.joinpath("txt.txt"), as_str=True)
     assert isinstance(out, str)
     assert out == "hello world\nhello world"
 
@@ -75,15 +73,32 @@
     assert len(out) == 2
     assert "name" in out[0].keys()
     out = load(tmp_path.joinpath("mydictlists.json"), as_str=True)
     assert isinstance(out, list)
     assert len(out) == 2
     assert "name" in out[0].keys()
 
-    # Everything else as text
+    # load numpy
+    out = load(tmp_path.joinpath("arr.txt"), as_arr=True)
+    assert isinstance(out, np.ndarray)
+    assert len(out) == 10
+
+    out = load(tmp_path.joinpath("arr.npy"))
+    assert isinstance(out, np.ndarray)
+    assert len(out) == 10
+
+    # Custom loader function
+    def custom_loader(file):
+        with Path(file).open() as file_handle:
+            out = file_handle.readlines()
+        return out
+
+    out = load(".gitignore", verbose=True, loader_func=custom_loader)
+
+    # Attemp everything else as text, but with no custom loader issue warning
     with pytest.warns(UserWarning, match="not supported"):
         out = load(".gitignore", verbose=True)
 
     # incorrect type
     with pytest.raises(TypeError):
         out = load(10)
 
@@ -99,15 +114,14 @@
 
     # No error
     out = load("empty", assert_notempty=False)
     empty.unlink()
 
 
 def test_crawl():
-
     # TODO: test ignore arg more thoroughly
     project_root = Path(__file__).parent.parent.parent
     out = crawl(project_root)
     assert len(out)
     assert all(map(lambda f: ".git" not in str(f), out))
     outf = crawl(project_root, ignore=".vscode")
     assert all(map(lambda f: ".vscode" not in str(f), outf))
```

### Comparing `py_utilz-0.3.3/utilz/tests/test_ops.py` & `py_utilz-0.3.4/utilz/tests/test_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,59 +39,56 @@
     two = check_random_state()
     assert one.rand(1) != two.rand(1)
     three = check_random_state(999)
     four = check_random_state(999)
     assert three.rand(1) == four.rand(1)
 
 
-def test_mapcat():
-
-    # Just like map
+def test_map():
+    # Just like list comprehension
     out = map(lambda x: x * 2, [1, 2, 3, 4])
     correct = [x * 2 for x in [1, 2, 3, 4]]
     assert out == correct
 
     # Currying
     out = pipe([1, 2, 3, 4], map(lambda x: x * 2))
     assert out == correct
 
-    # Concatenating nested lists
+
+def test_mapcat():
+    # Nested lists are flattened
     data = [[1, 2], [3, 4]]
     out = mapcat(None, data)
     assert len(out) == 4
 
-    # Contrived examples as you'd most often just use np funcs directly:
-
-    # Type inference returns same type
+    # Numpy
     data = np.array(data)
-    out = mapcat(np.mean, data)
-    assert isinstance(out, np.ndarray)
-    assert len(out) == 2
-    assert out.ndim == 1
 
-    # If func returns a 1d iterable then concat will be 2d, just like np.array(list of
-    # lists)
+    # If input and return are both numpy arrays then the default concat_axis = None
+    # casts using np.array(mapresult)
+    # Here 1d func operates on each row of the 2d matrix
     out = mapcat(lambda x: np.power(x, 2), data)
     assert isinstance(out, np.ndarray)
     assert out.ndim == 2
 
-    # This is the same as setting axis to 1
-    out = mapcat(lambda x: np.power(x, 2), data, concat_axis=1)
-    assert out.ndim == 2
-
-    # Axis = 0 will flatten the array to 1d
-    out = mapcat(lambda x: np.power(x, 2), data, concat_axis=0)
-    assert out.ndim == 1
-
     # But when using regular map just return a list of numpy arrays
     out = map(lambda x: np.power(x, 2), data)
     assert isinstance(out, list)
     assert len(out) == 2
     assert isinstance(out[0], np.ndarray)
 
+    # This is the same as setting axis to 1 manually
+    out = mapcat(lambda x: np.power(x, 2), data, concat_axis=1)
+    assert out.ndim == 2
+
+    # Setting it to 0, flattens/hstacks the array into a 1d
+    out = mapcat(lambda x: np.power(x, 2), data, concat_axis=0)
+    assert out.ndim == 1
+    assert len(out) == 4
+
     # Passing kwargs to function works
     out = mapcat(np.std, data, ddof=1)
     assert isinstance(out, np.ndarray)
     assert np.allclose(out, np.std(data, ddof=1, axis=1))
     assert len(out) == 2
 
     # Loading files into a single dataframe
@@ -105,51 +102,51 @@
     assert out.shape == (30, 3)
 
     out = mapcat(load_data, ["file1.txt", "file2.txt", "file3.txt"], concat_axis=1)
     assert isinstance(out, pd.DataFrame)
     assert out.shape == (10, 9)
 
 
-def test_parallel_mapcat():
+def test_parallel_map():
     def f(x):
         sleep(0.5)
         return x**2
 
     def f_random(x, random_state=None):
         random_state = check_random_state(random_state)
         sleep(0.5)
         return x + random_state.rand()
 
     # Running sequentially takes 5s
     start = time()
-    out = mapcat(f, range(20), n_jobs=1)
+    out = map(f, range(20), n_jobs=1)
     duration = time() - start
     assert len(out) == 20
 
     # Running 2 jobs takes less time
     start = time()
-    out = mapcat(f, range(20), n_jobs=2)
+    out = map(f, range(20), n_jobs=2)
     par_duration = time() - start
     assert par_duration < duration
     assert len(out) == 20
 
     # By default if a function to be parallelized handles it's own randomization
     # interally, there should be no issue with repeated values when run in parallel
-    out = mapcat(f_random, [1, 1, 1, 1, 1], n_jobs=2)
+    out = map(f_random, [1, 1, 1, 1, 1], n_jobs=2)
     assert len(out) == len(set(out))
 
     # But for reproducibility we can set random_state to a number which will be passed
     # to the func's random_state argument
-    out = mapcat(f_random, [1, 1, 1, 1, 1], n_jobs=2, random_state=1)
-    out2 = mapcat(f_random, [1, 1, 1, 1, 1], n_jobs=2, random_state=1)
+    out = map(f_random, [1, 1, 1, 1, 1], n_jobs=2, random_state=1)
+    out2 = map(f_random, [1, 1, 1, 1, 1], n_jobs=2, random_state=1)
     assert np.allclose(out, out2)
 
     # But not if it doesn't accept that kwarg
     with pytest.raises(TypeError):
-        out = mapcat(f, [1, 1, 1, 1, 1], n_jobs=2, random_state=1)
+        out = map(f, [1, 1, 1, 1, 1], n_jobs=2, random_state=1)
 
 
 def test_mapalts():
     """Just easier shorthands for things we can do with default mapcat"""
 
     # Map a sequence of functions on after another
     out = pipe(seq(10), mapcompose(lambda x: x**2, np.sqrt))
@@ -213,15 +210,14 @@
 
     out = pipe(["A", "C"], mapwith(lambda label, df: df.query("Group == @label"), df))
     assert len(out) == 2
     assert out[0].shape[0] == int(df.shape[0] / 4)
 
 
 def test_filter():
-
     # Length 9
     arr = ["aa", "ab", "ac", "ba", "bb", "bc", "ca", "cb", "cc"]
     # Keep anything containing "a"
     assert len(filter("a", arr)) == 5
     # Alias
     assert len(keep("a", arr)) == 5
     # Drop anything containing "a"
@@ -245,15 +241,14 @@
     assert len(pipe(arr, filter("a"))) == 5
 
     # Normal filtering
     assert all(filter(lambda x: isinstance(x, str), arr))
 
 
 def test_pipes_basic():
-
     df = randdf((20, 3)).assign(Group=["A"] * 5 + ["B"] * 5 + ["C"] * 5 + ["D"] * 5)
 
     # input -> output
     out = pipe(df, lambda df: df.head())
     assert out.shape == (5, 4)
     out = pipe(df, lambda df: df.head(10), lambda df: df.tail(5))
     assert out.shape == (5, 4)
@@ -392,27 +387,26 @@
 
     # like this
     out = pipe(df, do("head", n=10))
     assert out.equals(df.head(10))
 
 
 def test_iffy():
-
     bigger_5 = lambda x: x > 5
 
     # Pass in predicate func and return value
     out = pipe(10, iffy(bigger_5, 2))
     assert out == 2
 
     # Without if_false returns input by default
     out = pipe(1, iffy(bigger_5, 2))
     assert out == 1
 
     # Useful to conditionally apply func over iterable when combined with map
-    out = pipe(seq(10), mapcat(iffy(bigger_5, lambda x: x * 2)))
+    out = pipe(seq(10), map(iffy(bigger_5, lambda x: x * 2)))
     assert equal(out, [0, 1, 2, 3, 4, 5, 12, 14, 16, 18])
 
 
 def test_pop():
     # Pop is for shrinking outputs to other funcs
     # Keep is pruning the final outputs of a complicated pipe
```

### Comparing `py_utilz-0.3.3/utilz/tests/test_plot.py` & `py_utilz-0.3.4/utilz/tests/test_plot.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     f, axs = mpinit()
     out = stripbarplot(x="group", y="A1", data=df, ax=axs, estimator=np.median)
     assert out == axs
     plt.close(f)
 
 
 def test_savefig(tmp_path: Path):
-
     # Save to cwd
     f, _ = mpinit(subplots=(2, 2))
     save_raster = Path.cwd() / "raster" / "test.jpg"
     save_vector = Path.cwd() / "vector" / "test.pdf"
     savefig(f, "test")
     plt.close(f)
     assert save_raster.exists()
```

### Comparing `py_utilz-0.3.3/setup.py` & `py_utilz-0.3.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,93 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: py-utilz
+Version: 0.3.4
+Summary: Faster, easier, more robust python data analysis
+License: MIT
+Author: ejolly
+Author-email: eshin.jolly@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: joblib (>=1.1.0,<2.0.0)
+Requires-Dist: matplotlib (>=3.1.0,<4.0.0)
+Requires-Dist: numpy (>=1.16,<2.0)
+Requires-Dist: pandas (>=1.2.0,<2.0.0)
+Requires-Dist: seaborn (>=0.12.0)
+Requires-Dist: toolz (>=0.12.0,<0.13.0)
+Requires-Dist: tqdm (>=4.64.1,<5.0.0)
+Description-Content-Type: text/markdown
+
+# py-utilz
+
+![Build Status](https://github.com/ejolly/py-utilz/workflows/Utilz/badge.svg)
+[![Coverage Status](https://coveralls.io/repos/github/ejolly/utilz/badge.svg?branch=master)](https://coveralls.io/github/ejolly/utilz?branch=master)
+![Python Versions](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
+![Platforms](https://img.shields.io/badge/platform-linux%20%7C%20osx%20%7C%20win-blue)
+
+Convenient helper functions, decorators, and data analysis tools to make life easier with minimal dependencies:
+
+`pip install py-utilz`
+
+[dplyr](https://dplyr.tidyverse.org/) like data grammar:
+
+```python
+from utilz import pipe
+import utilz.dfverbs as _
+
+out = pipe(
+    df,
+    _.rename({"weight (male, lbs)": "male", "weight (female, lbs)": "female"}),
+    _.pivot_longer(columns=["male", "female"], into=("sex", "weight")),
+    _.split("weight", ("min", "max"), sep="-"),
+    _.pivot_longer(columns=["min", "max"], into=("stat", "weight")),
+    _.astype({"weight": float}),
+    _.groupby("genus", "sex"),
+    _.mutate(weight="weight.mean()"),
+    _.pivot_wider(column="sex", using="weight"),
+    _.mutate(dimorphism="male / female")
+)
+```
+
+```python
+from utilz import map
+
+# Combine function results into a list, array, or dataframe
+map(myfunc, myiterable)
+
+# Syntactic sugar for joblib.Parallel
+map(myfunc, myiterable, n_jobs=4)
+```
+
+```python
+from utilz import log, maybe
+
+# Print the shape of args and outputs before and after execute
+@log
+def myfunc(args):
+    return out
+
+# Only run myfunc if results.csv doesn't eist
+@maybe('results.csv')
+def myfunc(args):
+    return out
+```
+
+## Development
+
+1. Install [poetry](https://python-poetry.org/): `curl -sSL https://install.python-poetry.org | python`
+2. Setup virtual environment `poetry install --with dev`
+3. Run all tests: `poetry run pytest`
+4. Live render docs: `poetry run mkdocs serve`
+
+### Additional poetry/virtual environment commands
+
+- Activate environment in current shell: `source activate .venv/bin/activate`
+- Activate environment in sub-process shell: `poetry shell`
+- Add/remove additional packages: `poetry add/remove package_name`
+- Build local package: `poetry build`
+- Deploy to pypi: `poetry publish` (requires auth)
 
-packages = \
-['utilz', 'utilz.dfverbs', 'utilz.tests']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['ipdb>=0.13.9,<0.14.0',
- 'joblib>=1.1.0,<2.0.0',
- 'matplotlib>=3.1.0,<4.0.0',
- 'numpy>=1.16,<2.0',
- 'pandas>=1.2.0,<2.0.0',
- 'seaborn>=0.12.0',
- 'toolz>=0.12.0,<0.13.0',
- 'tqdm>=4.64.1,<5.0.0']
-
-setup_kwargs = {
-    'name': 'py-utilz',
-    'version': '0.3.3',
-    'description': 'Faster, easier, more robust python data analysis',
-    'long_description': '# Utilz\n![Build Status](https://github.com/ejolly/utilz/workflows/Utilz/badge.svg)\n[![Coverage Status](https://coveralls.io/repos/github/ejolly/utilz/badge.svg?branch=master)](https://coveralls.io/github/ejolly/utilz?branch=master)\n![Python Versions](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)\n![Platforms](https://img.shields.io/badge/platform-linux%20%7C%20osx%20%7C%20win-blue)\n\nConvenient helper functions, decorators, and data analysis tools to make life easier with minimal dependencies:\n\n`pip install py-utilz`\n\n[dplyr](https://dplyr.tidyverse.org/) like data grammar:\n\n\n```python\nfrom utilz import pipe\nimport utilz.dfverbs as _\n\nout = pipe(\n    df,\n    _.rename({"weight (male, lbs)": "male", "weight (female, lbs)": "female"}),\n    _.pivot_longer(columns=["male", "female"], into=("sex", "weight")),\n    _.split("weight", ("min", "max"), sep="-"),\n    _.pivot_longer(columns=["min", "max"], into=("stat", "weight")),\n    _.astype({"weight": float}),\n    _.groupby("genus", "sex"),\n    _.mutate(weight="weight.mean()"),\n    _.pivot_wider(column="sex", using="weight"),\n    _.mutate(dimorphism="male / female")\n)\n```\n\n```python\nfrom utilz import mapcat\n\n# Combine function results into a list, array, or dataframe\nmapcat(myfunc, myiterable) \n\n# Syntactic sugar for joblib.Parallel\nmapcat(myfunc, myiterable, n_jobs=4)\n```\n\n```python\nfrom utilz import log, maybe\n\n# Print the shape of args and outputs before and after execute\n@log\ndef myfunc(args):\n    return out\n\n# Only run myfunc if results.csv doesn\'t eist\n@maybe(\'results.csv\')\ndef myfunc(args):\n    return out\n```\n\n\n## Development\n\n1. Install [poetry](https://python-poetry.org/): `curl -sSL https://install.python-poetry.org | python`\n2. Setup virtual environment `poetry install`\n3. Run all tests: `poetry run pytest`\n4. Live render docs: `poetry run mkdocs serve`\n\n### Additional poetry/virtual environment commands\n- Activate environment in current shell: `source activate .venv/bin/activate`\n- Activate environment in sub-process shell: `poetry shell`\n- Add/remove additional packages: `poetry add/remove package_name`\n- Build local package: `poetry build`\n- Deploy to pypi: `poetry publish` (requires auth)\n',
-    'author': 'ejolly',
-    'author_email': 'eshin.jolly@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

