# Comparing `tmp/py_utilz-0.3.4.tar.gz` & `tmp/py_utilz-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_utilz-0.3.4.tar", max compression
+gzip compressed data, was "py_utilz-0.4.0.tar", max compression
```

## Comparing `py_utilz-0.3.4.tar` & `py_utilz-0.4.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     1067 2023-06-18 00:29:07.997893 py_utilz-0.3.4/LICENSE
--rw-r--r--   0        0        0     2211 2023-06-18 00:29:07.997893 py_utilz-0.3.4/README.md
--rw-r--r--   0        0        0      818 2023-06-18 00:29:08.001893 py_utilz-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      196 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/__init__.py
--rw-r--r--   0        0        0      754 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/_utils.py
--rw-r--r--   0        0        0     2419 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/boilerplate.py
--rw-r--r--   0        0        0     5387 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/decorators.py
--rw-r--r--   0        0        0     9423 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/dftools.py
--rw-r--r--   0        0        0       62 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/dfverbs/__init__.py
--rw-r--r--   0        0        0     4922 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/dfverbs/plot.py
--rw-r--r--   0        0        0     6230 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/dfverbs/stats.py
--rw-r--r--   0        0        0    18857 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/dfverbs/verbs.py
--rw-r--r--   0        0        0     5945 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/io.py
--rw-r--r--   0        0        0    16218 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/maps.py
--rw-r--r--   0        0        0    14804 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/ops.py
--rw-r--r--   0        0        0        0 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/pipeline.py
--rw-r--r--   0        0        0     9664 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/plot.py
--rw-r--r--   0        0        0     1003 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/shorts.py
--rw-r--r--   0        0        0      921 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/stats.py
--rw-r--r--   0        0        0      195 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/tests/conftest.py
--rw-r--r--   0        0        0     1783 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/tests/mtcars.csv
--rw-r--r--   0        0        0      741 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/tests/test_boilerplate.py
--rw-r--r--   0        0        0     5604 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/tests/test_decorators.py
--rw-r--r--   0        0        0     5195 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/tests/test_dftools.py
--rw-r--r--   0        0        0    13773 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/tests/test_dfverbs.py
--rw-r--r--   0        0        0     3994 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/tests/test_io.py
--rw-r--r--   0        0        0    17078 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/tests/test_ops.py
--rw-r--r--   0        0        0     1436 2023-06-18 00:29:08.001893 py_utilz-0.3.4/utilz/tests/test_plot.py
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 py_utilz-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-18 03:59:47.981301 py_utilz-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2211 2023-06-18 03:59:47.981301 py_utilz-0.4.0/README.md
+-rw-r--r--   0        0        0      818 2023-06-18 03:59:47.989301 py_utilz-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      217 2023-06-18 03:59:47.989301 py_utilz-0.4.0/utilz/__init__.py
+-rw-r--r--   0        0        0      754 2023-06-18 03:59:47.989301 py_utilz-0.4.0/utilz/_utils.py
+-rw-r--r--   0        0        0     2420 2023-06-18 03:59:47.989301 py_utilz-0.4.0/utilz/boilerplate.py
+-rw-r--r--   0        0        0     5468 2023-06-18 03:59:47.989301 py_utilz-0.4.0/utilz/decorators.py
+-rw-r--r--   0        0        0     9423 2023-06-18 03:59:47.989301 py_utilz-0.4.0/utilz/dftools.py
+-rw-r--r--   0        0        0       62 2023-06-18 03:59:47.989301 py_utilz-0.4.0/utilz/dfverbs/__init__.py
+-rw-r--r--   0        0        0     4922 2023-06-18 03:59:47.989301 py_utilz-0.4.0/utilz/dfverbs/plot.py
+-rw-r--r--   0        0        0     6232 2023-06-18 03:59:47.989301 py_utilz-0.4.0/utilz/dfverbs/stats.py
+-rw-r--r--   0        0        0    18857 2023-06-18 03:59:47.989301 py_utilz-0.4.0/utilz/dfverbs/verbs.py
+-rw-r--r--   0        0        0     5948 2023-06-18 03:59:47.989301 py_utilz-0.4.0/utilz/io.py
+-rw-r--r--   0        0        0    18649 2023-06-18 03:59:47.989301 py_utilz-0.4.0/utilz/maps.py
+-rw-r--r--   0        0        0     3406 2023-06-18 03:59:47.989301 py_utilz-0.4.0/utilz/ops.py
+-rw-r--r--   0        0        0     9340 2023-06-18 03:59:47.989301 py_utilz-0.4.0/utilz/pipes.py
+-rw-r--r--   0        0        0     9664 2023-06-18 03:59:47.993301 py_utilz-0.4.0/utilz/plot.py
+-rw-r--r--   0        0        0     3148 2023-06-18 03:59:47.993301 py_utilz-0.4.0/utilz/shorts.py
+-rw-r--r--   0        0        0      921 2023-06-18 03:59:47.993301 py_utilz-0.4.0/utilz/stats.py
+-rw-r--r--   0        0        0      195 2023-06-18 03:59:47.993301 py_utilz-0.4.0/utilz/tests/conftest.py
+-rw-r--r--   0        0        0     1783 2023-06-18 03:59:47.993301 py_utilz-0.4.0/utilz/tests/mtcars.csv
+-rw-r--r--   0        0        0      741 2023-06-18 03:59:47.993301 py_utilz-0.4.0/utilz/tests/test_boilerplate.py
+-rw-r--r--   0        0        0     5604 2023-06-18 03:59:47.993301 py_utilz-0.4.0/utilz/tests/test_decorators.py
+-rw-r--r--   0        0        0     5195 2023-06-18 03:59:47.993301 py_utilz-0.4.0/utilz/tests/test_dftools.py
+-rw-r--r--   0        0        0    13773 2023-06-18 03:59:47.993301 py_utilz-0.4.0/utilz/tests/test_dfverbs.py
+-rw-r--r--   0        0        0     3994 2023-06-18 03:59:47.993301 py_utilz-0.4.0/utilz/tests/test_io.py
+-rw-r--r--   0        0        0    17567 2023-06-18 03:59:47.993301 py_utilz-0.4.0/utilz/tests/test_ops.py
+-rw-r--r--   0        0        0     1436 2023-06-18 03:59:47.993301 py_utilz-0.4.0/utilz/tests/test_plot.py
+-rw-r--r--   0        0        0     1697 2023-06-18 03:59:47.993301 py_utilz-0.4.0/utilz/tests/test_shorts.py
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 py_utilz-0.4.0/PKG-INFO
```

### Comparing `py_utilz-0.3.4/LICENSE` & `py_utilz-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_utilz-0.3.4/README.md` & `py_utilz-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `py_utilz-0.3.4/pyproject.toml` & `py_utilz-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-utilz"
-version = "0.3.4"
+version = "0.4.0"
 description = "Faster, easier, more robust python data analysis"
 authors = ["ejolly <eshin.jolly@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "utilz" }]
 
 [tool.poetry.dependencies]
```

### Comparing `py_utilz-0.3.4/utilz/_utils.py` & `py_utilz-0.4.0/utilz/_utils.py`

 * *Files identical despite different names*

### Comparing `py_utilz-0.3.4/utilz/boilerplate.py` & `py_utilz-0.4.0/utilz/boilerplate.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 __all__ = ["randdf"]
 
 import pandas as pd
 from typing import Union
 import string
 from itertools import cycle
-from .ops import check_random_state
+from .maps import check_random_state
 
 
 def randdf(
     size: tuple = (10, 3),
     columns: Union[list, None] = None,
     groups: Union[dict, None] = None,
     func=None,
```

### Comparing `py_utilz-0.3.4/utilz/decorators.py` & `py_utilz-0.4.0/utilz/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,25 +128,25 @@
 
 def maybe(function):
     """
     A decorator that wraps a function which should take a kwarg called `out_file`. If
     `out_file` exists then it's loaded from disk, otherwise the wrapped function is
     called. If the wrapped function takes a kwarg `overwrite = True` then it always runs. You can also pass `loader_func = callable` to use a custom loading function
 
-    Example:
+        @maybe
+        def expensive_func(data, **kwargs'):
+            b = something_expensive(data)
+            np.save(b, kwargs.get('out_file')
+            return b
 
-    >>> @maybe
-    >>> def mean_brain(subpath, **kwargs):
-    >>> b = Brain_Data(subpath)
-    >>> m = b.mean()
-    >>> out_file = kwargs.get('out_file')
-    >>> m.write(out_file)
-    >>> return m
+        # First run will execute the function
+        expensive_func(data, out_file='result.npy')
 
-    >>> mean_brain(subpath, out_file='mean_brain.h5', loader_func=Brain_Data)
+        # Second run will load from 'result.npy'
+        expensive_func(data, out_file='result.npy')
 
     """
 
     @wraps(function)
     def wrapper(*args, **kwargs):
         # get out_file from the wrapped function
         out_file = kwargs.get("out_file", None)
```

### Comparing `py_utilz-0.3.4/utilz/dftools.py` & `py_utilz-0.4.0/utilz/dftools.py`

 * *Files identical despite different names*

### Comparing `py_utilz-0.3.4/utilz/dfverbs/plot.py` & `py_utilz-0.4.0/utilz/dfverbs/plot.py`

 * *Files identical despite different names*

### Comparing `py_utilz-0.3.4/utilz/dfverbs/stats.py` & `py_utilz-0.4.0/utilz/dfverbs/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 ]
 
 import numpy as np
 import pandas as pd
 from toolz import curry
 from .verbs import _reset_index_helper, apply, split, summarize, merge, mutate
 import seaborn as sns
-from ..ops import pipe
+from ..pipes import pipe
 from ..maps import filter
 
 
 @curry
 def mean(*args, **kwargs):
     """Call df.mean"""
```

### Comparing `py_utilz-0.3.4/utilz/dfverbs/verbs.py` & `py_utilz-0.4.0/utilz/dfverbs/verbs.py`

 * *Files identical despite different names*

### Comparing `py_utilz-0.3.4/utilz/io.py` & `py_utilz-0.4.0/utilz/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 from typing import Union, Any, List, Callable
 import pandas as pd
 import numpy as np
 import pickle
 import json
 from warnings import warn
-from .ops import sort
+from .shorts import sort
 from .maps import mapcat, filter
 from toolz import pipe
 from fnmatch import fnmatchcase
 
 
 def load(
     f: Union[Path, str],
```

### Comparing `py_utilz-0.3.4/utilz/maps.py` & `py_utilz-0.4.0/utilz/maps.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """
-The maps module is a generalization of many of the functions in `utilz.ops` that operate
-on **iterables**. Here are the parallels:
+The maps module is designed to be used with sequences and has several generalizations of functions in `utilz.ops` that work with sequences. Here are the parallels:
 
 | map function (s)   | op function(s)  | description |
 |---|---|---|
 | `map`  | `do`  | apply **one function** |
 | `mapcompose`  | `pipe`/`do(compose())`  | apply **multiple functions in sequence** |
 | `mapmany`  | `many`  | apply **multiple functions in parallel** |
-| `mapacross`  | `None`  | apply **multiple functions** to **multiple inputs** in pairs
 | `mapif`  | `iffy`  | apply **one function** if a *predicate function* otherwise noop |
-| `mapcat`  | `None`/`concat`  | apply **one multi-output function** and flatten the results |
+| `mapacross`  | `None`  | apply **multiple functions** to **multiple inputs** in pairs
+| `mapcat`  | `None`  | apply **one multi-output function** and flatten the results |
 | `mapwith`  | `None`  | map a two argument function to an iterable and a fixed arg or two iterables |
 
 
 All members of the `map` family, expect an iterable as their **last** argument, each
 element of which is passed to functions as their **first** argument. Except for
 `mapcat`, all `map*` functions return a sequence the same length as the input they received.
 """
@@ -23,44 +22,48 @@
     "map",
     "mapcat",
     "mapcompose",
     "mapmany",
     "mapacross",
     "mapif",
     "mapwith",
+    "check_random_state",
 ]
 
+import numpy as np
+import pandas as pd
 from joblib import delayed, Parallel
 from collections.abc import Callable, Iterable
 from typing import Union, Any
-from .ops import curry, concat, check_random_state, iffy, compose, many
+from .ops import iffy, compose, do
+from toolz import curry
 from ._utils import ProgressParallel
 from tqdm import tqdm
 from inspect import signature
 import numpy as np
-from itertools import filterfalse
+from itertools import filterfalse, chain
 from copy import deepcopy
 
 
 MAX_INT = np.iinfo(np.int32).max
 _filter = filter  # we're overwriting the base func
 
 
-# Helper used by map
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
+    """Helper used by map"""
     # Setup progress bars and parallelization
     if n_jobs < 1 or n_jobs > 1:
         # Initialize joblib parallelizer
         if progressbar:
             parfor = ProgressParallel(
                 prefer=backend, n_jobs=n_jobs, verbose=verbose, total=len(iterme)
             )
@@ -128,14 +131,80 @@
     if n_jobs < 1 or n_jobs > 1:
         return parfor(call_list)
     else:
         return call_list
 
 
 @curry
+def _many(*args):
+    """Helper used by mapmany"""
+
+    def call(data):
+        if isinstance(data, (list, tuple)):
+            raise TypeError(
+                f"Expected a single input but receive {len(data)}. Use mapmany() to operate on an iterable"
+            )
+        if len(args) <= 1:
+            raise ValueError(
+                f"many applies *multiple* function calls separately but only received {len(args)} function. Use map() to apply a single function."
+            )
+
+        return tuple([do(f, data) for f in args])
+
+    return call
+
+
+def _concat(op, iterme, axis, ignore_index):
+    """Intelligently try to concatenate an iterable. Supports dataframe, arrays, and lists"""
+
+    try:
+        if isinstance(op[0], (pd.DataFrame, pd.Series)):
+            return pd.concat(
+                op, axis=0 if axis is None else axis, ignore_index=ignore_index
+            )
+
+        if isinstance(op[0], np.ndarray) or isinstance(iterme, np.ndarray):
+            try:
+                if axis is None:
+                    return np.array(op)
+                return np.concatenate(op, axis=axis)
+            except np.AxisError as _:
+                return np.stack(op, axis=axis - 1)
+            except ValueError as _:
+                return np.array(op)
+        if isinstance(op[0], list):
+            return list(chain.from_iterable(op))
+        return op
+
+    except Exception as e:
+        print(e)
+        return op
+
+
+def check_random_state(seed=None):
+    """Turn seed into a np.random.RandomState instance. Note: credit for this code goes entirely to `sklearn.utils.check_random_state`. Using the source here simply avoids an unecessary dependency.
+
+    Args:
+        seed (None, int, np.RandomState): if seed is None, return the RandomState singleton used by np.random. If seed is an int, return a new RandomState instance seeded with seed. If seed is already a RandomState instance, return it. Otherwise raise ValueError.
+    """
+
+    import numbers
+
+    if seed is None or seed is np.random:
+        return np.random.mtrand._rand
+    if isinstance(seed, (numbers.Integral, np.integer)):
+        return np.random.RandomState(seed)
+    if isinstance(seed, np.random.RandomState):
+        return seed
+    raise ValueError(
+        "%r cannot be used to seed a numpy.random.RandomState" " instance" % seed
+    )
+
+
+@curry
 def map(
     func: Union[Callable, None],
     iterme: Iterable,
     **kwargs,
 ):
     """
     Super-power your `for` loops with a progress-bar and optional *reproducible*
@@ -246,15 +315,15 @@
     """Call map and concatenate results after.
     Particularly useful to ensure results are numpy arrays"""
 
     concat_axis = kwargs.pop("concat_axis", None)
     ignore_index = kwargs.pop("ignore_index", True)
     out = map(func, iterme, **kwargs)
 
-    return concat(out, iterme, concat_axis, ignore_index)
+    return _concat(out, iterme, concat_axis, ignore_index)
 
 
 @curry
 def mapacross(*args):
     """Map multiple functions to an iterable in a matched-pair fasion. The
     number of funcions needs to equal the length of the iterable."""
 
@@ -284,15 +353,15 @@
                 f"All map* funcs expect a list/tuple of input, but received a single {type(data)}."
             )
         if len(args) <= 1:
             raise ValueError(
                 f"mapmany applies *multiple* function calls separately but only received {len(args)} function. Use mapcat() to apply a single function."
             )
 
-        together = many(*args)
+        together = _many(*args)
         return map(together, data, **kwargs)
 
     return call
 
 
 @curry
 def mapcompose(*args, **kwargs):
```

### Comparing `py_utilz-0.3.4/utilz/ops.py` & `py_utilz-0.4.0/utilz/pipes.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,118 +2,43 @@
 Functional tools intended to be used with `pipe()`. Everything in this module except for
 `pipe` itself, is *curried* so can be called without a full set of args.
 
 ## Overview
 
 | function (s)   | description  | 
 |---|---|
-| `do`  | apply a function or method to an object |
 | `pipe`  | run an input through a sequence of functions  |
 | `append`/`alongwith`  | apply a function and return `(input, result)` as a `tuple` |
 | `fork`  | call `input.copy` if possible otheriwse create `n` duplicate `deepcopy`'s of `input` |
-| `many`  | applies **multiple functions in parallel** to a **single** input and returns an iterable; like an "inverse `map`" |
 | `spread`  | acts like `fork` if given an `int` otherwise acts like `many` |
-| `across`  | apply **multiple functions** to **multiple inputs** in pairs; alias for `mapacross` |
-| `compose`  | combine **multiple functions** into **one function** sequence (mini-pipe) |
 | `gather`/`unpack`  | make an iterable's items separately accessible to a **single function** |
-| `iffy`  | apply a function if a predicate function is true otherwise noop |
+| `pop`  | pop off an element from an iterable, useful for pruning down calls to `alongwith`/`spread` |
 
 ---
 """
 __all__ = [
     "pipe",
     "append",
     "alongwith",
-    "across",
-    "sort",
     "fork",
-    "many",
     "spread",
     "gather",
     "unpack",
-    "do",
-    "iffy",
-    "compose",
-    "curry",
     "pop",
-    "nth",
-    "check_random_state",
-    "pairs",
 ]
 
 import numpy as np
 import pandas as pd
 from typing import Union, Any
-from collections.abc import Callable, Iterable
-from itertools import chain as it_chain
-import itertools as it
+from collections.abc import Iterable
 from inspect import signature
 from toolz import curry, juxt
-from toolz.curried import compose_left as compose, nth
-from inspect import signature
 from pathlib import Path
 
 
-def check_random_state(seed=None):
-    """Turn seed into a np.random.RandomState instance. Note: credit for this code goes entirely to `sklearn.utils.check_random_state`. Using the source here simply avoids an unecessary dependency.
-
-    Args:
-        seed (None, int, np.RandomState): if seed is None, return the RandomState singleton used by np.random. If seed is an int, return a new RandomState instance seeded with seed. If seed is already a RandomState instance, return it. Otherwise raise ValueError.
-    """
-
-    import numbers
-
-    if seed is None or seed is np.random:
-        return np.random.mtrand._rand
-    if isinstance(seed, (numbers.Integral, np.integer)):
-        return np.random.RandomState(seed)
-    if isinstance(seed, np.random.RandomState):
-        return seed
-    raise ValueError(
-        "%r cannot be used to seed a numpy.random.RandomState" " instance" % seed
-    )
-
-
-def concat(op, iterme, axis, ignore_index):
-    """Intelligently try to concatenate an iterable. Supports dataframe, arrays, and lists"""
-
-    try:
-        if isinstance(op[0], (pd.DataFrame, pd.Series)):
-            return pd.concat(
-                op, axis=0 if axis is None else axis, ignore_index=ignore_index
-            )
-
-        if isinstance(op[0], np.ndarray) or isinstance(iterme, np.ndarray):
-            try:
-                if axis is None:
-                    return np.array(op)
-                return np.concatenate(op, axis=axis)
-            except np.AxisError as _:
-                return np.stack(op, axis=axis - 1)
-            except ValueError as _:
-                return np.array(op)
-        if isinstance(op[0], list):
-            return list(it_chain.from_iterable(op))
-        return op
-
-    except Exception as e:
-        print(e)
-        return op
-
-
-@curry
-def sort(iterme: Iterable, **kwargs):
-    return sorted(iterme, **kwargs)
-
-
-@curry
-def pairs(iterme: Iterable):
-    return list(it.combinations(iterme, 2))
-
-
 def pipe(
     data: Any,
     *funcs: Iterable,
     output: bool = True,
     show: bool = False,
     debug: bool = False,
     keep: Union[int, None] = None,
@@ -242,63 +167,76 @@
                 else:
                     _out.append(o)
             out = tuple(_out)
         return out
 
 
 @curry
-def chain(*args, **kwargs):
-    """Chain a sequence of functions on an input, i.e. a mini-pipe"""
-
-    def call(data):
-        for f in args:
-            data = f(data, **kwargs)
-
-    return call
-
-
-@curry
-def many(*args):
-    """Apply many functions separately to a single input. Operates like the inverse of
-    map(). Whereas map takes applies 1 func to multiple elements, many applies multiple funcs to 1 element. Returns a tuple the same length as args containing the output of each function
-    """
+def pop(idx):
+    """Given a tuple, removes an element located at an `idx`. Useful for pruning down a
+    call to append or spread."""
 
-    def call(data):
-        if isinstance(data, (list, tuple)):
-            raise TypeError(
-                f"Expected a single input but receive {len(data)}. Use mapmany() to operate on an iterable"
-            )
-        if len(args) <= 1:
-            raise ValueError(
-                f"many applies *multiple* function calls separately but only received {len(args)} function. Use map() to apply a single function."
-            )
+    if isinstance(idx, int):
 
-        return tuple([f(data) for f in args])
+        def remove(data):
+            if isinstance(data, (tuple, list)):
+                data = list(data) if isinstance(data, tuple) else data
+                _ = data.pop(idx)
+                out = tuple(data)
+                out = out[0] if len(out) == 1 else out
+                return out
+            else:
+                raise TypeError(
+                    f"expected a tuple of input data by received a single {type(data)}"
+                )
 
-    return call
+        return remove
+    else:
+        raise TypeError("pop requires an integer index to of the ouput to drop")
 
 
 @curry
-def fork(*args):
-    """Duplicate an input N number of times"""
+def fork(n):
+    """Duplicate an input `n` number of times"""
     from copy import deepcopy
 
     def duplicate(data):
         copy = getattr(data, "copy", None)
         if callable(copy):
-            return tuple([data.copy()] * args[0])
-        return tuple([deepcopy(data)] * args[0])
+            return tuple([data.copy()] * n)
+        return tuple([deepcopy(data)] * n)
 
     return duplicate
 
 
-# Deprecate?
+@curry
+def gather(func, data):
+    """Wraps a function that takes multiple inputs to make the output of a previous
+    function with multiple outputs easier to work with. Useful after a call to `append`,
+    `spread`, `across` or `mapmany` e.g.
+
+        gather(lambda first_name, last_name: first_name + last_name)
+    """
+    if not (isinstance(data, (list, tuple)) and len(data) > 1):
+        raise TypeError(
+            f"gather expects the previous step's output to be a list/tuple of length > 1 but received a {type(data)}"
+        )
+
+    return func(*data)
+
+
+@curry
+def unpack(func, data):
+    """Alias for `gather`"""
+    return gather(func, data)
+
+
 @curry
 def spread(*args):
-    """Generalization of fork OR many"""
+    """Like `fork` but expects multiple functions"""
 
     from copy import deepcopy
 
     if len(args) == 1:
         if isinstance(args[0], int):
 
             def duplicate(data):
@@ -317,19 +255,19 @@
         together = juxt(*args)
         return together
     else:
         raise TypeError(f"spread expected an integer or 1+ functions")
 
 
 @curry
-def append(func):
+def alongwith(func):
     """Takes a function or obj and returns a new function that prepends the args to the
     function as part of the input, i.e. (input, funcval)"""
 
-    def alongwith(data):
+    def _alongwith(data):
         # If data is a tuple and func only takes 1 arg, then assume the user wants the
         # original data in the chain
         if callable(func):
             if isinstance(data, tuple):
                 sig = signature(func)
                 if len(sig.parameters) == 1:
                     out = func(data[0])
@@ -338,117 +276,14 @@
                 # Otherwise give them the entire chain
                 return (*data, out)
             else:
                 out = func(data)
                 return (data, out)
         return (data, func)
 
-    return alongwith
+    return _alongwith
 
 
-# Alias
 @curry
-def alongwith(thing):
-    return append(thing)
-
-
-# Alias for mapacross but returns tuple
-def across(*args):
-    """Like mapacross but returns a tuple"""
-
-    def call(data):
-        if not isinstance(data, (list, tuple)):
-            raise TypeError(
-                f"Expected a list/tuple of input, but received a single {type(data)}. If you want to apply a function to a single input either use a lambda or do()"
-            )
-        if len(data) != len(args):
-            raise ValueError(
-                f"Te number of functions passed must equal the length of the previous output, but {len(data)} data and {len(args)} functions don't match. To run the same set of functions over the previous inputs see separate()"
-            )
-        return tuple([f(a) for f, a in zip(args, data)])
-
-    return call
-
-
-@curry
-def gather(func, data):
-    if not (isinstance(data, (list, tuple)) and len(data) > 1):
-        raise TypeError(
-            f"gather expects the previous step's output to be a list/tuple of length > 1 but received a {type(data)}"
-        )
-
-    return func(*data)
-
-
-# Alias for gather
-@curry
-def unpack(func, data):
-    """Wraps a function that takes multiple inputs to make the output of a previous
-    function with multiple outputs easier to work with. Useful after a call to `append`,
-    `spread`, `across` or `mapmany` e.g.
-
-    `unpack(lambda first_name, last_name: first_name + last_name)`
-    """
-
-    return gather(func, data)
-
-
-@curry
-def do(func, data, *args, **kwargs):
-    """Apply a single function to data or call a method on data, while passing optional
-    kwargs to that functinon or method"""
-    from operator import methodcaller as mc
-
-    if isinstance(func, str):
-        func = mc(func, *args, **kwargs)
-    return func(data)
-
-
-@curry
-def iffy(predicate_func: Callable, if_true: Union[Any, Callable], data: Any):
-    """
-    Conditionally apply a function based on a predicate function. Useful to
-    conditionally map a function to an interable when combined with mapcat
-
-    Args:
-        conditional (callable): callable function on which data will be evaluated.
-        Should return a boolean value
-        if_true (any, callable, optional): Value or function to call if predicate_func
-        is True
-        data (any): previous pipe output
-
-    """
-
-    if not callable(predicate_func):
-        raise TypeError("ifelse requires a function that returns a boolean value")
-
-    if predicate_func(data):
-        if callable(if_true):
-            return if_true(data)
-        else:
-            return if_true
-    else:
-        return data
-
-
-@curry
-def pop(idx):
-    """Given a tuple, removes an element located at an index. Useful for pruning down a
-    call to append or spread."""
-
-    if isinstance(idx, int):
-
-        def remove(data):
-            if isinstance(data, (tuple, list)):
-                data = list(data) if isinstance(data, tuple) else data
-                _ = data.pop(idx)
-                out = tuple(data)
-                out = out[0] if len(out) == 1 else out
-                return out
-            else:
-                raise TypeError(
-                    f"expected a tuple of input data by received a single {type(data)}"
-                )
-
-        return remove
-    else:
-        raise TypeError("pop requires an integer index to of the ouput to drop")
+def append(thing):
+    """Alias for `alongwith`"""
+    return alongwith(thing)
```

### Comparing `py_utilz-0.3.4/utilz/plot.py` & `py_utilz-0.4.0/utilz/plot.py`

 * *Files identical despite different names*

### Comparing `py_utilz-0.3.4/utilz/stats.py` & `py_utilz-0.4.0/utilz/stats.py`

 * *Files identical despite different names*

### Comparing `py_utilz-0.3.4/utilz/tests/mtcars.csv` & `py_utilz-0.4.0/utilz/tests/mtcars.csv`

 * *Files identical despite different names*

### Comparing `py_utilz-0.3.4/utilz/tests/test_boilerplate.py` & `py_utilz-0.4.0/utilz/tests/test_boilerplate.py`

 * *Files identical despite different names*

### Comparing `py_utilz-0.3.4/utilz/tests/test_decorators.py` & `py_utilz-0.4.0/utilz/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `py_utilz-0.3.4/utilz/tests/test_dftools.py` & `py_utilz-0.4.0/utilz/tests/test_dftools.py`

 * *Files identical despite different names*

### Comparing `py_utilz-0.3.4/utilz/tests/test_dfverbs.py` & `py_utilz-0.4.0/utilz/tests/test_dfverbs.py`

 * *Files identical despite different names*

### Comparing `py_utilz-0.3.4/utilz/tests/test_io.py` & `py_utilz-0.4.0/utilz/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `py_utilz-0.3.4/utilz/tests/test_ops.py` & `py_utilz-0.4.0/utilz/tests/test_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     mapif,
     mapwith,
     filter,
     pipe,
     spread,
     gather,
     unpack,
-    across,
     do,
+    many,
     iffy,
     append,
     compose,
     curry,
     pop,
     keep,
     discard,
@@ -300,32 +300,32 @@
     # (input1, input2) -> (output1, output2)
 
     # Use map instead for 1 func
     with pytest.raises(ValueError):
         out = pipe([df, df], mapmany(lambda df: df.head(5)))
 
     # 2 func-input pairs
-    out = pipe([df, df], across(lambda df: df.head(5), lambda df: df.tail(10)))
+    out = pipe([df, df], mapacross(lambda df: df.head(5), lambda df: df.tail(10)))
     assert len(out) == 2
     assert out[0].equals(df.head(5))
     assert out[1].equals(df.tail(10))
 
     # 2 funcs, i.e. mini-pipe
     out = pipe([df, df], mapcompose(lambda df: df.head(10), lambda df: df.tail(5)))
     assert isinstance(out, list) and len(out) == 2
     assert out[0].equals(out[1])
     assert out[0].equals(df.iloc[5:10, :])
 
     # not enough funcs
     with pytest.raises(ValueError):
-        out = pipe([df, df], across(lambda df: df.head(5)))
+        out = pipe([df, df], mapacross(lambda df: df.head(5)))
 
     # not enough data
     with pytest.raises(ValueError):
-        out = pipe([df], across(lambda df: df.head(5), lambda df: df.tail(2)))
+        out = pipe([df], mapacross(lambda df: df.head(5), lambda df: df.tail(2)))
 
     # SPREAD (one2many)
     # input -> (input, input, input)
     out = pipe(df, spread(3))
     assert isinstance(out, tuple)
     assert len(out) == 3
     assert all(df.equals(ddf) for ddf in out)
@@ -386,14 +386,32 @@
         out = pipe(df, do("head", 10))
 
     # like this
     out = pipe(df, do("head", n=10))
     assert out.equals(df.head(10))
 
 
+def test_many():
+    df = randdf()
+    out = many(("head", "tail"), df)
+    assert len(out) == 2
+
+    out = many((lambda df: df.mean(), lambda df: df.std(), lambda df: df.var()), df)
+    assert out[0].equals(df.mean())
+    assert out[1].equals(df.std())
+    assert out[2].equals(df.var())
+
+    # Should pass iterable of funcs
+    with pytest.raises(ValueError):
+        out = many("head", df)
+
+    out = many(("head", "head"), df)
+    assert do("head", df).equals(out[0])
+
+
 def test_iffy():
     bigger_5 = lambda x: x > 5
 
     # Pass in predicate func and return value
     out = pipe(10, iffy(bigger_5, 2))
     assert out == 2
 
@@ -508,36 +526,36 @@
         df,
         lambda df: df.groupby("group"),
         spread(
             lambda dfg: dfg.select("A1").mean(),
             lambda dfg: dfg.select("B1").mean(),
         ),
         ...,
-        across(
+        mapacross(
             lambda means: sns.histplot(means),
             lambda means: sns.boxplot(means),
         ),
         debug=True,
     )
     assert len(out) == 3  # 3 steps in pipe
-    assert isinstance(out[-1], tuple)  # plots
+    assert isinstance(out[-1], list)  # plots
     assert isinstance(out[-2], tuple)  # series
     assert isinstance(out[-3], pd.core.groupby.generic.DataFrameGroupBy)
 
     # Same as above but with a compose thrown in for extra complexity.
     # Without debug=True we can unpack the tuple
     out1, out2 = pipe(
         df,
         lambda df: df.groupby("group"),
         spread(
             lambda dfg: dfg.select("A1").mean(),
             lambda dfg: dfg.select("B1").mean(),
         ),
         ...,
-        across(
+        mapacross(
             compose(lambda means: sns.histplot(means), tweak(title="histplot")),
             compose(lambda means: sns.boxplot(means), tweak(title="boxplot")),
         ),
     )
     assert isinstance(out1, pd.Series)
     assert isinstance(out2, pd.Series)
 
@@ -546,15 +564,15 @@
         df,
         lambda df: df.groupby("group"),
         spread(
             lambda dfg: dfg.select("A1").mean(),
             lambda dfg: dfg.select("B1").mean(),
         ),
         ...,
-        across(
+        mapacross(
             compose(lambda means: sns.histplot(means), tweak(title="histplot")),
             compose(lambda means: sns.boxplot(means), tweak(title="boxplot")),
         ),
         keep=0,
     )
     assert isinstance(a1_mean, pd.Series)
```

### Comparing `py_utilz-0.3.4/utilz/tests/test_plot.py` & `py_utilz-0.4.0/utilz/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `py_utilz-0.3.4/PKG-INFO` & `py_utilz-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-utilz
-Version: 0.3.4
+Version: 0.4.0
 Summary: Faster, easier, more robust python data analysis
 License: MIT
 Author: ejolly
 Author-email: eshin.jolly@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

