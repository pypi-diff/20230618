# Comparing `tmp/fairbench-0.2.5-py3-none-any.whl.zip` & `tmp/fairbench-0.2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,35 +1,41 @@
-Zip file size: 21873 bytes, number of entries: 33
--rw-rw-rw-  2.0 fat      382 b- defN 23-May-31 10:14 fairbench/__init__.py
+Zip file size: 29907 bytes, number of entries: 39
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-17 09:11 fairbench/__init__.py
 -rw-rw-rw-  2.0 fat     1952 b- defN 23-Jun-01 09:25 fairbench/export.py
--rw-rw-rw-  2.0 fat       38 b- defN 23-May-14 10:33 fairbench/bench/__init__.py
--rw-rw-rw-  2.0 fat      583 b- defN 23-May-14 15:09 fairbench/bench/loader.py
+-rw-rw-rw-  2.0 fat       38 b- defN 23-Jun-14 13:57 fairbench/bench/__init__.py
+-rw-rw-rw-  2.0 fat     2341 b- defN 23-Jun-15 21:51 fairbench/bench/demos.py
+-rw-rw-rw-  2.0 fat     1660 b- defN 23-Jun-15 09:42 fairbench/bench/loader.py
+-rw-rw-rw-  2.0 fat       93 b- defN 23-Jun-17 19:28 fairbench/export/__init__.py
+-rw-rw-rw-  2.0 fat    11887 b- defN 23-Jun-18 13:34 fairbench/export/interactive.py
+-rw-rw-rw-  2.0 fat     2912 b- defN 23-Jun-16 09:23 fairbench/export/native.py
 -rw-rw-rw-  2.0 fat      122 b- defN 23-May-13 22:58 fairbench/forks/__init__.py
 -rw-rw-rw-  2.0 fat     2130 b- defN 23-May-25 07:44 fairbench/forks/categorical.py
--rw-rw-rw-  2.0 fat     1161 b- defN 23-Jun-07 09:00 fairbench/forks/explanation.py
--rw-rw-rw-  2.0 fat    23920 b- defN 23-Jun-07 08:52 fairbench/forks/fork.py
+-rw-rw-rw-  2.0 fat     2586 b- defN 23-Jun-16 09:22 fairbench/forks/explanation.py
+-rw-rw-rw-  2.0 fat    25873 b- defN 23-Jun-15 09:40 fairbench/forks/fork.py
 -rw-rw-rw-  2.0 fat      154 b- defN 23-Jan-14 23:08 fairbench/metrics/__init__.py
--rw-rw-rw-  2.0 fat     2846 b- defN 23-May-31 08:40 fairbench/metrics/classification.py
+-rw-rw-rw-  2.0 fat     4164 b- defN 23-Jun-16 09:23 fairbench/metrics/classification.py
 -rw-rw-rw-  2.0 fat     2066 b- defN 23-May-31 07:41 fairbench/metrics/disparate_impact.py
 -rw-rw-rw-  2.0 fat     1494 b- defN 23-May-31 07:41 fairbench/metrics/disparate_mistreatment.py
 -rw-rw-rw-  2.0 fat      100 b- defN 23-May-31 10:15 fairbench/mitigation/__init__.py
 -rw-rw-rw-  2.0 fat     1790 b- defN 23-May-31 10:16 fairbench/mitigation/postprocessing.py
 -rw-rw-rw-  2.0 fat      207 b- defN 23-Jan-15 14:06 fairbench/reports/__init__.py
 -rw-rw-rw-  2.0 fat     1491 b- defN 23-Jun-07 08:52 fairbench/reports/accumulate.py
--rw-rw-rw-  2.0 fat     1648 b- defN 23-Jun-07 08:50 fairbench/reports/adhoc.py
--rw-rw-rw-  2.0 fat     2259 b- defN 23-May-28 14:54 fairbench/reports/base.py
+-rw-rw-rw-  2.0 fat     1937 b- defN 23-Jun-16 06:38 fairbench/reports/adhoc.py
+-rw-rw-rw-  2.0 fat     2567 b- defN 23-Jun-15 21:29 fairbench/reports/base.py
 -rw-rw-rw-  2.0 fat      883 b- defN 23-May-14 15:09 fairbench/reports/surrogate.py
 -rw-rw-rw-  2.0 fat      155 b- defN 23-Feb-20 08:42 fairbench/reports/reduction/__init__.py
--rw-rw-rw-  2.0 fat      794 b- defN 23-May-28 14:54 fairbench/reports/reduction/expanders.py
--rw-rw-rw-  2.0 fat     1853 b- defN 23-Jun-02 08:25 fairbench/reports/reduction/reduce.py
--rw-rw-rw-  2.0 fat     2364 b- defN 23-May-28 14:54 fairbench/reports/reduction/reducers.py
+-rw-rw-rw-  2.0 fat     2260 b- defN 23-Jun-16 09:23 fairbench/reports/reduction/expanders.py
+-rw-rw-rw-  2.0 fat     2611 b- defN 23-Jun-15 20:51 fairbench/reports/reduction/reduce.py
+-rw-rw-rw-  2.0 fat     2834 b- defN 23-Jun-16 06:45 fairbench/reports/reduction/reducers.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-26 21:15 tests/__init__.py
--rw-rw-rw-  2.0 fat     1394 b- defN 23-May-28 18:45 tests/test_batching.py
+-rw-rw-rw-  2.0 fat     1394 b- defN 23-Jun-12 10:06 tests/test_batching.py
 -rw-rw-rw-  2.0 fat     1278 b- defN 23-Jun-01 09:09 tests/test_benchmarks.py
--rw-rw-rw-  2.0 fat     4884 b- defN 23-Jun-07 08:14 tests/test_forks.py
--rw-rw-rw-  2.0 fat     1572 b- defN 23-Jun-02 08:24 tests/test_reduction.py
+-rw-rw-rw-  2.0 fat     1103 b- defN 23-Jun-16 09:20 tests/test_demos.py
+-rw-rw-rw-  2.0 fat     5807 b- defN 23-Jun-15 09:42 tests/test_forks.py
+-rw-rw-rw-  2.0 fat     1287 b- defN 23-Jun-08 09:09 tests/test_metrics.py
+-rw-rw-rw-  2.0 fat     1624 b- defN 23-Jun-14 06:40 tests/test_reduction.py
 -rw-rw-rw-  2.0 fat     6556 b- defN 23-May-31 14:04 tests/test_reports.py
--rw-rw-rw-  2.0 fat      809 b- defN 23-Jun-07 09:48 fairbench-0.2.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-07 09:48 fairbench-0.2.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-Jun-07 09:48 fairbench-0.2.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2783 b- defN 23-Jun-07 09:48 fairbench-0.2.5.dist-info/RECORD
-33 files, 69776 bytes uncompressed, 17395 bytes compressed:  75.1%
+-rw-rw-rw-  2.0 fat      830 b- defN 23-Jun-18 14:03 fairbench-0.2.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-18 14:03 fairbench-0.2.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Jun-18 14:03 fairbench-0.2.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     3273 b- defN 23-Jun-18 14:03 fairbench-0.2.6.dist-info/RECORD
+39 files, 99571 bytes uncompressed, 24675 bytes compressed:  75.2%
```

## zipnote {}

```diff
@@ -3,17 +3,29 @@
 
 Filename: fairbench/export.py
 Comment: 
 
 Filename: fairbench/bench/__init__.py
 Comment: 
 
+Filename: fairbench/bench/demos.py
+Comment: 
+
 Filename: fairbench/bench/loader.py
 Comment: 
 
+Filename: fairbench/export/__init__.py
+Comment: 
+
+Filename: fairbench/export/interactive.py
+Comment: 
+
+Filename: fairbench/export/native.py
+Comment: 
+
 Filename: fairbench/forks/__init__.py
 Comment: 
 
 Filename: fairbench/forks/categorical.py
 Comment: 
 
 Filename: fairbench/forks/explanation.py
@@ -72,29 +84,35 @@
 
 Filename: tests/test_batching.py
 Comment: 
 
 Filename: tests/test_benchmarks.py
 Comment: 
 
+Filename: tests/test_demos.py
+Comment: 
+
 Filename: tests/test_forks.py
 Comment: 
 
+Filename: tests/test_metrics.py
+Comment: 
+
 Filename: tests/test_reduction.py
 Comment: 
 
 Filename: tests/test_reports.py
 Comment: 
 
-Filename: fairbench-0.2.5.dist-info/METADATA
+Filename: fairbench-0.2.6.dist-info/METADATA
 Comment: 
 
-Filename: fairbench-0.2.5.dist-info/WHEEL
+Filename: fairbench-0.2.6.dist-info/WHEEL
 Comment: 
 
-Filename: fairbench-0.2.5.dist-info/top_level.txt
+Filename: fairbench-0.2.6.dist-info/top_level.txt
 Comment: 
 
-Filename: fairbench-0.2.5.dist-info/RECORD
+Filename: fairbench-0.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fairbench/__init__.py

```diff
@@ -1,13 +1,2 @@
-from fairbench.forks import *
-from fairbench.metrics import *
-from fairbench.reports import *
-from fairbench.export import *
-from fairbench.mitigation import *
-from fairbench.bench import *
 
-from fairbench import forks
-from fairbench import metrics
-from fairbench import reports
-from fairbench import export
-from fairbench import mitigation
-from fairbench import bench
+
```

## fairbench/bench/loader.py

```diff
@@ -1,17 +1,49 @@
-import os, wget
+import os
+import wget
 import pandas as pd
+import zipfile
+import re
 
 
-def read_csv(uci, *args, **kwargs):
-    path = "data/" + uci.replace("\\", "/")
-    if not os.path.exists(path):
-        url = "https://archive.ics.uci.edu/ml/machine-learning-databases/" + uci
-        os.makedirs("/".join(path.split("/")[:-1]), exist_ok=True)
-        wget.download(url, path)
+def _extract_nested_zip(file, folder):
+    print(file, folder)
+    os.makedirs(folder, exist_ok=True)
+    with zipfile.ZipFile(file, "r") as zfile:
+        zfile.extractall(path=folder)
+    os.remove(file)
+    for root, dirs, files in os.walk(folder):
+        for filename in files:
+            if filename.endswith(".zip"):
+                _extract_nested_zip(
+                    os.path.join(root, filename), os.path.join(root, filename[:-4])
+                )
+
+
+def read_csv(url, *args, **kwargs):
+    url = url.replace("\\", "/")
+    if ".zip/" in url:
+        url, path = url.split(".zip/", 1)
+        extract_to = "data/"
+        if "/" not in path:
+            extract_to += url.split("/")[-1]
+            path = os.path.join(url.split("/")[-1], path)
+        path = os.path.join("data", path)
+        url += ".zip"
+        temp = "data/" + url.split("/")[-1]
+        if not os.path.exists(path):
+            os.makedirs(os.path.join(*path.split("/")[:-1]), exist_ok=True)
+            wget.download(url, temp)
+            _extract_nested_zip(temp, extract_to)
+    else:
+        shortened = "/".join(url.split("/")[-2:])
+        path = "data/" + shortened
+        if not os.path.exists(path):
+            os.makedirs("/".join(path.split("/")[:-1]), exist_ok=True)
+            wget.download(url, path)
     return pd.read_csv(path, *args, **kwargs)
 
 
 def features(df, numeric, categorical):
     dfs = [df[col] for col in numeric] + [
         pd.get_dummies(df[col]) for col in categorical
     ]
```

## fairbench/forks/explanation.py

```diff
@@ -1,40 +1,93 @@
 from typing import Any
 import eagerpy as ep
-from objwrap import Wrapper
+from objwrap import ClosedWrapper
+import numpy as np
+from scipy import interpolate
 
 
 def tofloat(value):
     if isinstance(value, ep.Tensor):
         return float(value.raw)
     return float(value)
 
 
-class Explainable(Wrapper):
+class ExplainableError(Exception):
+    def __init__(self, message):
+        super().__init__(message)
+        self.explain = message
+        self.value = float("NaN")
+        self.distribution = None
+        self.desc = None
+
+    def __float__(self):
+        return self.value
+
+    def __int__(self):
+        return self.value
+
+    def __str__(self):
+        return "---"
+
+
+class ExplanationCurve:
+    def __init__(self, x, y, name="Curve"):
+        assert isinstance(x, np.ndarray)
+        assert isinstance(y, np.ndarray)
+        self.x = x
+        self.y = y
+        self.name = name
+        assert x.shape == y.shape
+
+    def togrid(self, grid):
+        new_x = np.linspace(self.x.min(), self.x.max(), num=grid)
+        approx = interpolate.interp1d(x=self.x, y=self.y)
+        return ExplanationCurve(new_x, approx(new_x))
+
+    @property
+    def points(self):
+        return self.x.shape[0]
+
+    def __str__(self):
+        return f"{self.name} ({self.points} points)"
+
+
+class Explainable(ClosedWrapper):
     def __init__(self, value, explain: Any = None, desc: str = None, **kwargs):
         from fairbench.forks import Fork
 
         if value.__class__.__name__ == "Future":
             value = value.result()
-
+        if isinstance(value, int) or isinstance(value, float):
+            value = np.float64(value)
         assert (
             isinstance(value, float)
             or isinstance(value, int)
+            or isinstance(value, np.floating)
             or "tensor" in value.__class__.__name__.lower()
             or "array" in value.__class__.__name__
-        ), "Can not set non-numeric as explainable"
+        ), f"Can not set data type as explainable: {type(value)}"
         assert (
             explain is None or not kwargs
         ), "Cannot create explainable with both todict and a Fork"
         super().__init__(value)
         self.explain = Fork(kwargs) if explain is None else explain
         self.desc = desc
 
     def __float__(self):
         return tofloat(self.__value__())
 
+    def __int__(self):
+        return int(self.__float__())
+
+    def __str__(self):
+        return f"{self.__float__():.3f}"
+
     @property
     def value(self):
         return self.__value__()
 
     def numpy(self):
         return self.value.numpy()
+
+    def __after__(self, obj):
+        return obj
```

## fairbench/forks/fork.py

```diff
@@ -1,23 +1,53 @@
 from makefun import wraps
 import eagerpy as ep
 import numpy as np
 import inspect
 import sys
 from collections.abc import Mapping
+from objwrap import ClosedWrapper
 
 _backend = "numpy"
 
 
+def _str_foreign(v, tabs=0):
+    if isinstance(v, Fork):
+        v = v.branches()
+    if isinstance(v, dict):
+        complicated = False
+        for val in v.values():
+            if isinstance(val, Fork) or isinstance(val, dict):
+                complicated = True
+        return "\n".join(
+            "   " * tabs
+            + k
+            + ": "
+            + ("\n" if complicated else "")
+            + _str_foreign(fromtensor(v), tabs + 1)
+            for k, v in v.items()
+        )
+    if isinstance(v, float) or isinstance(v, np.float64):
+        return f"{v:.3f}"
+    return str(v)
+
+
 class Forklike(dict):
     def __getattribute__(self, name):
-        if name in dir(Fork):
+        if name in dir(Forklike):
             return object.__getattribute__(self, name)
         return self[name]
 
+    def __getitem__(self, item):
+        if item in self:
+            return super().__getitem__(item)
+        return Forklike({k: getattr(v, item) for k, v in self.items()})
+
+    def __str__(self):
+        return _str_foreign(self)
+
 
 def _result(ret):
     if ret.__class__.__name__ == "Future":
         ret = ret.result()
     if isinstance(ret, dict):
         return Forklike(ret)
     return ret
@@ -26,14 +56,18 @@
 def setbackend(backend_name: str):
     assert backend_name in ["torch", "tensorflow", "jax", "numpy"]
     global _backend
     _backend = backend_name
 
 
 def tobackend(value):
+    if isinstance(value, ep.Tensor) and isinstance(
+        value.raw, np.float64
+    ):  # TODO: investigate why this is needed for distributed mode
+        return value
     global _backend
     name = type(value.raw if isinstance(value, ep.Tensor) else value).__module__.split(
         "."
     )[0]
     m = sys.modules
     if isinstance(value, list):
         value = np.array(value)
@@ -67,31 +101,51 @@
         "tensor" not in value.__class__.__name__.lower()
         and "array" not in value.__class__.__name__.lower()
     ):
         return False
     return True
 
 
-def astensor(value, _allow_explanation=False) -> ep.Tensor:
+def astensor(value, _allow_explanation=True) -> ep.Tensor:
     if value.__class__.__name__ == "Explainable" and not _allow_explanation:
         value = value.value
+    elif value.__class__.__name__ == "Explainable":
+        from fairbench import Explainable
+
+        return Explainable(
+            astensor(value.value), explain=value.explain, desc=value.desc
+        )
+    if isinstance(value, int) or isinstance(value, float):
+        value = np.float64(value)
     if (
         "tensor" not in value.__class__.__name__.lower()
         and "array" not in value.__class__.__name__.lower()
+        and not isinstance(value, np.float64)
     ):
         return value
     if isinstance(value, list):
         value = np.array(value, dtype=np.float)
-    value = tobackend(value)
+    if isinstance(value, np.float64):
+        value = ep.NumPyTensor(value)
+    else:
+        value = tobackend(value)
     if value.ndim != 0:
         value = value.flatten()
     return value.float64()
 
 
-def fromtensor(value):
+def fromtensor(value, _allow_explanation=True):
+    if value.__class__.__name__ == "Explainable" and not _allow_explanation:
+        value = value.value
+    elif value.__class__.__name__ == "Explainable":
+        from fairbench import Explainable
+
+        return Explainable(
+            fromtensor(value.value), explain=value.explain, desc=value.desc
+        )
     # TODO: maybe applying this as a wrapper to methods instead of submitting to dask can be faster
     if isinstance(value, ep.Tensor):
         return value.raw
 
     return value
 
 
@@ -311,17 +365,15 @@
                 if not isinstance(value, Explainable)
                 else value
                 for branch, value in self._branches.items()
             }
         )
 
     def __str__(self):
-        return "\n".join(
-            k + ": " + str(fromtensor(v)) for k, v in self.branches().items()
-        )
+        return _str_foreign(self)
 
     def __repr__(self):
         # from IPython.display import display_html, HTML
         # display_html(HTML(self.__repr_html__()))
         return super().__repr__()
 
     def _repr_html_(self):
@@ -379,19 +431,25 @@
 _client = _NoClient()
 
 
 def distributed(*args, **kwargs):
     global _client
     from dask.distributed import Client
 
+    if isinstance(_client, Client):
+        _client.close()
     _client = Client(*args, **kwargs)
 
 
 def serial():
     global _client
+    from dask.distributed import Client
+
+    if isinstance(_client, Client):
+        _client.close()
     _client = _NoClient()
 
 
 def parallel(_wrapped_method):
     if len(inspect.getfullargspec(_wrapped_method)[0]) <= 1:
         raise Exception(
             "To avoid ambiguity, the @parallel decorator can be applied only to methods with at least"
```

## fairbench/metrics/classification.py

```diff
@@ -1,37 +1,61 @@
 from fairbench.forks import parallel, unit_bounded
+from fairbench.forks.explanation import Explainable, ExplanationCurve
 from eagerpy import Tensor
 
 
 @parallel
 @unit_bounded
 def accuracy(predictions: Tensor, labels: Tensor, sensitive: Tensor = None):
     if sensitive is None:
         sensitive = predictions.ones_like()
     num_sensitive = sensitive.sum()
-    if num_sensitive == 0:
-        return 0
-    return 1 - ((predictions - labels) * sensitive).abs().sum() / num_sensitive
+    true = ((predictions - labels) * sensitive).abs().sum()
+    return Explainable(
+        0 if num_sensitive == 0 else 1 - true / num_sensitive,
+        samples=num_sensitive,
+        true=true,
+    )
+
+
+@parallel
+@unit_bounded
+def auc(scores: Tensor, labels: Tensor, sensitive: Tensor = None):
+    import sklearn
+
+    if sensitive is None:
+        sensitive = scores.ones_like()
+    scores = scores[sensitive == 1]
+    labels = labels[sensitive == 1]
+    fpr, tpr, _ = sklearn.metrics.roc_curve(labels.numpy(), scores.numpy())
+    return Explainable(
+        sklearn.metrics.auc(fpr, tpr),
+        curve=ExplanationCurve(fpr, tpr, "ROC"),
+        samples=sensitive.sum(),
+    )
 
 
 @parallel
 @unit_bounded
 def pr(predictions: Tensor, sensitive: Tensor = None):
     if sensitive is None:
         sensitive = predictions.ones_like()
     sum_sensitive = sensitive.sum()
-    if sum_sensitive == 0:
-        return sum_sensitive
-    return (predictions * sensitive).sum() / sum_sensitive
+    sum_positives = (predictions * sensitive).sum()
+    return Explainable(
+        0 if sum_sensitive == 0 else (sum_positives / sum_sensitive),
+        samples=sum_sensitive,
+        positives=sum_positives,
+    )
 
 
 @parallel
 @unit_bounded
 def positives(predictions: Tensor, sensitive: Tensor):
-    return (predictions * sensitive).mean()
+    return (predictions * sensitive).sum()
 
 
 @parallel
 @unit_bounded
 def tpr(
     predictions: Tensor,
     labels: Tensor,
@@ -39,17 +63,20 @@
     max_prediction: float = 1,
 ):
     if sensitive is None:
         sensitive = predictions.ones_like()
     error = (max_prediction - (predictions - labels).abs()) * predictions
     error_sensitive = error * sensitive
     num_sensitive = (sensitive * predictions).sum()
-    if num_sensitive == 0:
-        return 0
-    return error_sensitive.sum() / num_sensitive
+    return Explainable(
+        0 if num_sensitive == 0 else (error_sensitive.sum() / num_sensitive),
+        positives=num_sensitive,
+        true_positives=error_sensitive.sum(),
+        samples=sensitive.sum(),
+    )
 
 
 @parallel
 @unit_bounded
 def fpr(
     predictions: Tensor,
     labels: Tensor,
@@ -58,15 +85,20 @@
     if sensitive is None:
         sensitive = predictions.ones_like()
     error = (predictions - labels).abs() * predictions
     error_sensitive = error * sensitive
     num_sensitive = (sensitive * predictions).sum()
     if num_sensitive == 0:
         return 0
-    return error_sensitive.sum() / num_sensitive
+    return Explainable(
+        0 if num_sensitive == 0 else (error_sensitive.sum() / num_sensitive),
+        positives=num_sensitive,
+        false_positives=error_sensitive.sum(),
+        samples=sensitive.sum(),
+    )
 
 
 @parallel
 @unit_bounded
 def tnr(
     predictions: Tensor,
     labels: Tensor,
@@ -75,17 +107,20 @@
 ):
     if sensitive is None:
         sensitive = predictions.ones_like()
     negatives = max_prediction - predictions
     error = (max_prediction - (predictions - labels).abs()) * negatives
     error_sensitive = error * sensitive
     num_sensitive = (sensitive * negatives).sum()
-    if num_sensitive == 0:
-        return 0
-    return error_sensitive.sum() / num_sensitive
+    return Explainable(
+        0 if num_sensitive == 0 else (error_sensitive.sum() / num_sensitive),
+        negatives=num_sensitive,
+        true_negatives=error_sensitive.sum(),
+        samples=sensitive.sum(),
+    )
 
 
 @parallel
 @unit_bounded
 def fnr(
     predictions: Tensor,
     labels: Tensor,
@@ -94,10 +129,13 @@
 ):
     if sensitive is None:
         sensitive = predictions.ones_like()
     negatives = max_prediction - predictions
     error = (predictions - labels).abs() * negatives
     error_sensitive = error * sensitive
     num_sensitive = (sensitive * negatives).sum()
-    if num_sensitive == 0:
-        return 0
-    return error_sensitive.sum() / num_sensitive
+    return Explainable(
+        0 if num_sensitive == 0 else (error_sensitive.sum() / num_sensitive),
+        negatives=num_sensitive,
+        false_negatives=error_sensitive.sum(),
+        samples=sensitive.sum(),
+    )
```

## fairbench/reports/adhoc.py

```diff
@@ -1,34 +1,40 @@
 from fairbench.reports.base import report, reportargsparse
 from fairbench.reports import reduction as fb
 from fairbench.reports.accumulate import todict as tokwargs
 from fairbench.forks.fork import combine, merge
 from fairbench.reports.surrogate import surrogate_positives
 from fairbench import metrics
+from fairbench.reports import reduction
 
 
 common_metrics = (metrics.accuracy, metrics.prule, metrics.dfpr, metrics.dfnr)
-acc_metrics = (metrics.accuracy, metrics.pr, metrics.tpr, metrics.tnr)
+acc_metrics = (metrics.accuracy, metrics.pr, metrics.tpr, metrics.tnr, metrics.auc)
+common_reduction = (
+    {"reducer": reduction.min},
+    {"reducer": reduction.wmean},
+    {"reducer": reduction.min, "expand": reduction.ratio},
+    {"reducer": reduction.max, "expand": reduction.diff},
+    {"reducer": reduction.max, "expand": reduction.barea},
+)
 
 
 def accreport(*args, metrics=acc_metrics, **kwargs):
     return report(*args, metrics=metrics, **kwargs)
 
 
 def binreport(*args, metrics=common_metrics, **kwargs):
     return report(*args, metrics=metrics, **kwargs)
 
 
-def multireport(*args, metrics=acc_metrics, **kwargs):
+def multireport(
+    *args, metrics=acc_metrics, reduction_schemes=common_reduction, **kwargs
+):
     base = report(*args, metrics=metrics, **kwargs)
-    return combine(
-        fb.reduce(base, fb.min),
-        fb.reduce(base, fb.min, expand=fb.ratio),
-        fb.reduce(base, fb.max, expand=fb.diff),
-    )
+    return combine(*[fb.reduce(base, **scheme) for scheme in reduction_schemes])
 
 
 def isecreport(*args, **kwargs):
     if len(args) == 0:
         params = tokwargs(**kwargs)
     else:
         params = dict()
```

## fairbench/reports/base.py

```diff
@@ -27,21 +27,26 @@
     if not isinstance(metrics, Iterable):
         metrics = [metrics]
     if not isinstance(metrics, dict):
         metrics = {metric.__name__: metric for metric in metrics}
     ret = dict()
     for name, metric in metrics.items():
         arg_names = set(inspect.getfullargspec(metric)[0])
-        ret[name] = metric(
-            **{
-                arg: Explainable(value, desc=arg)
-                for arg, value in kwargs.items()
-                if arg in arg_names
-            }
-        )
+        parsed_kwargs = {
+            arg: value  # TODO: find a way to add this Explainable(value, desc=arg) - this makes measures compute on explainable objects, which throws an error
+            for arg, value in kwargs.items()
+            if arg in arg_names
+            and (
+                not isinstance(value, str) or arg != value
+            )  # last statement for yamlres support
+        }
+        try:
+            ret[name] = metric(**parsed_kwargs)
+        except TypeError:
+            pass
     return ret
 
 
 def areport(*args, metrics: Union[Callable, Iterable, dict] = None, **kwargs):
     assert (
         metrics is not None
     ), "Cannot use fairbench.report() without explicitly declared metrics.\nUse accreport, binreport, multireport, or isecreport as ad-hoc report generation mechanisms."
```

## fairbench/reports/reduction/expanders.py

```diff
@@ -1,20 +1,55 @@
 import eagerpy as ep
 from typing import Iterable
+from fairbench.forks.explanation import Explainable, ExplainableError, ExplanationCurve
+import numpy as np
 
 
 def ratio(values: Iterable[ep.Tensor]) -> Iterable[ep.Tensor]:
-    assert isinstance(values, list), "Can only reduce lists with fairbench.ratio."
+    assert isinstance(values, list), "fairbench.ratio can only reduce lists ."
     return [value1 / value2 for value1 in values for value2 in values if value2 != 0]
 
 
 def diff(values: Iterable[ep.Tensor]) -> Iterable[ep.Tensor]:
-    assert isinstance(values, list), "Can only reduce lists with fairbench.diff."
+    assert isinstance(values, list), "fairbench.diff can only reduce lists."
     return [abs(value1 - value2) for value1 in values for value2 in values]
 
 
+def barea(values: Iterable[ep.Tensor]) -> Iterable[ep.Tensor]:
+    assert isinstance(values, list), "fairbench.diff can only reduce lists."
+    x_min = None
+    x_max = None
+    n_max = float("inf")
+    for value in values:
+        if (
+            not isinstance(value, Explainable)
+            or "curve" not in value.explain.branches()
+            or not isinstance(value.explain.curve, ExplanationCurve)
+        ):
+            raise ExplainableError("Explanation absent or does not store `curve`")
+        if x_min is None:
+            x_min = value.explain.curve.x.min()
+        elif value.explain.curve.x.min() != x_min:
+            raise ExplainableError(
+                f"Incompatible curves min: {x_min} vs {value.explain.curve.x.min()}"
+            )
+        if x_max is None:
+            x_max = value.explain.curve.x.max()
+        elif value.explain.curve.x.max() != x_max:
+            raise ExplainableError(
+                f"Incompatible curve max: {x_max} vs {value.explain.curve.x.max()}"
+            )
+        n_max = min(
+            n_max, value.explain.curve.points
+        )  # get the same discretization as the densest curve
+    values = [value.explain.curve.togrid(n_max).y for value in values]
+    return [
+        np.absolute(value1 - value2).mean() * (x_max - x_min)
+        for value1 in values
+        for value2 in values
+    ]
+
+
 def todata(values: Iterable[ep.Tensor]) -> ep.Tensor:
-    assert isinstance(
-        values, list
-    ), "Can only reduce lists of tensors with fairbench.todata."
+    assert isinstance(values, list), "fairbench.todata can only reduce lists ."
     values = [ep.reshape(value, (-1, 1)) for value in values]
     return ep.concatenate(values, axis=1)
```

## fairbench/reports/reduction/reduce.py

```diff
@@ -1,18 +1,31 @@
-from fairbench.forks.fork import Fork, astensor, comparator
-from fairbench.forks.explanation import Explainable
+from fairbench.forks.fork import Fork, astensor, comparator, fromtensor
+from fairbench.forks.explanation import Explainable, ExplainableError
 from typing import Optional
 
 # from fairbench.reports.accumulate import todict as tokwargs
 
 
 def areduce(fork: Fork, reducer, expand=None, transform=None, branches=None):
     return reduce(fork, reducer, expand, transform, branches, name=None)
 
 
+def _tryorexplainable(method, *args, **kwargs):
+    for arg in args:
+        if isinstance(arg, ExplainableError):
+            return arg
+    for arg in kwargs.values():
+        if isinstance(arg, ExplainableError):
+            return arg
+    try:
+        return method(*args, **kwargs)
+    except ExplainableError as e:
+        return e
+
+
 @comparator
 def reduce(
     fork: Fork,
     reducer,
     expand=None,
     transform=None,
     branches=None,
@@ -39,17 +52,30 @@
                 )
         else:
             fields.append(
                 astensor(v) if transform is None else transform(astensor(v[v]))
             )
     if expand is not None:
         fields = (
-            {k: expand(v) for k, v in fields.items()}
+            {k: _tryorexplainable(expand, v) for k, v in fields.items()}
             if isinstance(fields, dict)
-            else expand(fields)
+            else _tryorexplainable(expand, fields)
         )
     result = (
-        {k: Explainable(reducer(v), fork[k], desc=name) for k, v in fields.items()}
+        {
+            k: _tryorexplainable(
+                Explainable,
+                _tryorexplainable(fromtensor, _tryorexplainable(reducer, v), False),
+                fork[k],
+                desc=name,
+            )
+            for k, v in fields.items()
+        }
         if isinstance(fields, dict)
-        else Explainable(reducer(fields), fork, desc=name)
+        else _tryorexplainable(
+            Explainable,
+            _tryorexplainable(fromtensor, _tryorexplainable(reducer, fields), False),
+            fork,
+            desc=name,
+        )
     )
     return result if name is None else Fork({name: result})
```

## fairbench/reports/reduction/reducers.py

```diff
@@ -1,79 +1,89 @@
 import eagerpy as ep
 from typing import Iterable
+from fairbench.forks import Explainable, ExplainableError
 
 
 def abs(value):
     if value < 0:
         return -value
     return value
 
 
 def sum(values: Iterable[ep.Tensor]) -> ep.Tensor:
     assert isinstance(
         values, list
-    ), "Can only reduce lists with fairbench.sum. Maybe you meant to use eagerpy.sum?"
+    ), "fairbench.sum can only reduce lists. Maybe you meant to use eagerpy.sum?"
     ret = 0
     for value in values:
         ret = ret + value
     return ret
 
 
 def mean(values: Iterable[ep.Tensor]) -> ep.Tensor:
-    if not isinstance(values, list):
-        raise TypeError(
-            "Can only reduce lists with fairbench.mean. Maybe you meant to use eagerpy.mean?"
-        )
+    assert isinstance(
+        values, list
+    ), "fairbench.mean can only reduce lists. Maybe you meant to use eagerpy.mean?"
     return sum(values) / len(values)
 
 
+def wmean(values: Iterable[ep.Tensor]) -> ep.Tensor:
+    assert isinstance(values, list), "fairbench.wmean can only reduce lists."
+    for value in values:
+        if (
+            not isinstance(value, Explainable)
+            or "samples" not in value.explain.branches()
+        ):
+            raise ExplainableError("Explanation absent or does not store `samples`")
+    nom = sum([value * value.explain.samples for value in values])
+    denom = sum([value.explain.samples for value in values])
+    return nom if denom == 0 else nom / denom
+
+
 def identical(values: Iterable[ep.Tensor]) -> ep.Tensor:
     assert isinstance(
         values, list
-    ), "Can only reduce lists with fairbench.mean. Maybe you meant to use eagerpy.identical?"
+    ), "Can only reduce lists with fairbench.identical. Maybe you meant to use an eagerpy method?"
     for value in values:
-        assert (
-            value - values[0]
-        ).abs().sum() == 0, "eagerpy.identical requires that the exact same tensor is placed on all branches"
+        if (value - values[0]).abs().sum() != 0:
+            raise ExplainableError(
+                "The same value should reside in all branches for identical reduction."
+            )
     return values[0]
 
 
 def gm(values: Iterable[ep.Tensor]) -> ep.Tensor:
-    assert isinstance(
-        values, list
-    ), "Can only reduce lists with fairbench.mean. Maybe you meant to use eagerpy.mean?"
+    assert isinstance(values, list), "fairbench.gm can only reduce lists."
     ret = 1
     for value in values:
         ret = ret * value
     return ret ** (1.0 / len(values))
 
 
 def max(values: Iterable[ep.Tensor]) -> ep.Tensor:
     assert isinstance(
         values, list
-    ), "Can only reduce lists with fairbench.max. Maybe you meant to use eagerpy.maximum?"
+    ), "fairbench.max can only reduce lists. Maybe you meant to use eagerpy.maximum?"
     ret = float("-inf")
     for value in values:
         if value > ret:
             ret = value
     return ret
 
 
 def budget(values: Iterable[ep.Tensor]) -> ep.Tensor:
-    assert isinstance(
-        values, list
-    ), "Can only reduce lists with fairbench.budget. Maybe you meant to use an eagerpy method?"
+    assert isinstance(values, list), "fairbench.budget can only reduce lists."
     from math import log  # TODO: make this compatible with backpropagation
 
     # "An Intersectional Definition of Fairness"
-    return log(float(max(values)))
+    return max(values).log()
 
 
 def min(values: Iterable[ep.Tensor]) -> ep.Tensor:
     assert isinstance(
         values, list
-    ), "Can only reduce lists with fairbench.min. Maybe you meant to use eagerpy.minimum?"
+    ), "fairbench.min can only reduce lists. Maybe you meant to use eagerpy.minimum?"
     ret = float("inf")
     for value in values:
         if value < ret:
             ret = value
     return ret
```

## tests/test_forks.py

```diff
@@ -1,16 +1,31 @@
 import fairbench as fb
 import numpy as np
 
 
 def environment():
-    fb.distributed()
-    yield "distributed"
-    fb.serial()
-    yield "serial"
+    for _ in ["torch", "numpy"]:
+        fb.distributed()
+        yield "distributed"
+        fb.serial()
+        yield "serial"
+
+
+def test_conversion_number():
+    for _ in environment():
+        x = np.float64(2)
+        y = fb.astensor(x).log()
+        x2 = fb.fromtensor(y)
+        assert isinstance(x2, np.float64)
+
+
+def test_explainble():
+    x = fb.Explainable(fb.astensor(1))
+    y = fb.Explainable(fb.astensor(np.float32(2)))
+    assert x/y == 0.5
 
 
 def test_fork_generation():
     for _ in environment():
         fork = fb.Fork(a=1)
         assert fork.a == 1
         fork = fb.Fork(a=1, b=2, c=3)
@@ -130,19 +145,31 @@
         assert isinstance(fork.b, fb.Fork)
         assert isinstance(fork.x, fb.Fork)
         assert isinstance(fork.y, fb.Fork)
         assert fork.x.a == fork.a.x
         assert fork.x.b == fork.b.x
         assert fork.y.a == fork.a.y
         assert fork.y.b == fork.b.y
+        assert isinstance(fork.y.b, int)
 
 
 def test_fork_to_array():
     import fairbench as fb
     import numpy as np
 
     sensitive = fb.Fork(gender=fb.categories@np.array([1, 0, 0, 1]),
                         race=fb.categories@np.array([0, 1, 2, 3]),
                         age=fb.categories@np.array([3, 1, 2, 0]))
 
     report = fb.multireport(predictions=np.array([0, 0, 1, 1]), labels=np.array([0, 1, 1, 0]), sensitive=sensitive)
     print(report)
+
+
+def test_fork_direct_explain():
+    import fairbench as fb
+    import numpy as np
+    sensitive = fb.Fork(gender=fb.categories@np.array([1, 0, 0, 1]),
+                        race=fb.categories@np.array([0, 1, 2, 3]),
+                        age=fb.categories@np.array([3, 1, 2, 0]))
+    report = fb.multireport(predictions=np.array([0, 0, 1, 1]), labels=np.array([0, 1, 1, 0]), sensitive=sensitive)
+    explanation = report.explain
+    assert "min" in explanation.branches()
```

## tests/test_reduction.py

```diff
@@ -1,25 +1,33 @@
 import fairbench as fb
 import numpy as np
 from .test_forks import environment
 
 
+def produce_report():
+    predictions = np.array([1, 0, 1, 0, 1, 0, 0, 0])
+    labels = np.array([1, 0, 1, 0, 1, 1, 0, 0])
+    men = np.array([1, 1, 1, 0, 0, 0, 0, 0])
+    women = np.array([0, 0, 0, 1, 1, 1, 0, 0])
+    nonbin = np.array([0, 0, 0, 0, 0, 0, 1, 1])
+    sensitive = fb.Fork(men=men, women=women, nonbin=nonbin)
+    report = fb.binreport(sensitive=sensitive, predictions=predictions, labels=labels)
+    return report
+
+
 def test_reduce():
     for _ in environment():
-        predictions = np.array([1, 0, 1, 0, 1, 0, 0, 0])
-        labels = np.array([1, 0, 1, 0, 1, 1, 0, 0])
-        men = np.array([1, 1, 1, 0, 0, 0, 0, 0])
-        women = np.array([0, 0, 0, 1, 1, 1, 0, 0])
-        nonbin = np.array([0, 0, 0, 0, 0, 0, 1, 1])
-        sensitive = fb.Fork(men=men, women=women, nonbin=nonbin)
-        report = fb.binreport(sensitive=sensitive, predictions=predictions, labels=labels)
-        reduction = fb.reduce(report, reducer=fb.min, expand=fb.ratio)
+        reduction = fb.reduce(produce_report(), reducer=fb.min, expand=fb.ratio)
         assert reduction.minratio.accuracy.value == 0.6666666666666667
         assert reduction.minratio.dfnr.value == -2
-        assert fb.areduce(report.accuracy, reducer=fb.min, expand=fb.ratio) == 0.6666666666666667
-        assert fb.areduce(report.accuracy, reducer=fb.max, expand=fb.diff) == 0.33333333333333326
-        assert fb.areduce(report.accuracy, reducer=fb.mean, expand=fb.diff) == 0.1481481481481481
-        assert fb.areduce(report.accuracy, reducer=fb.budget, expand=fb.diff) == -1.09861228866811
-        assert fb.areduce(report.accuracy, reducer=fb.min, expand=fb.ratio).value == 0.6666666666666667
-        assert fb.areduce(report.accuracy, reducer=fb.max, expand=fb.diff).value == 0.33333333333333326
-        assert fb.areduce(report.accuracy, reducer=fb.mean, expand=fb.diff).value == 0.1481481481481481
-        assert fb.areduce(report.accuracy, reducer=fb.budget, expand=fb.diff).value == -1.09861228866811
+
+
+def test_areduce():
+    report = produce_report()
+    assert fb.areduce(report.accuracy, reducer=fb.min, expand=fb.ratio) == 0.6666666666666667
+    assert fb.areduce(report.accuracy, reducer=fb.max, expand=fb.diff) == 0.33333333333333326
+    assert fb.areduce(report.accuracy, reducer=fb.mean, expand=fb.diff) == 0.1481481481481481
+    assert fb.areduce(report.accuracy, reducer=fb.budget, expand=fb.diff) == -1.09861228866811
+    assert fb.areduce(report.accuracy, reducer=fb.min, expand=fb.ratio).value == 0.6666666666666667
+    assert fb.areduce(report.accuracy, reducer=fb.max, expand=fb.diff).value == 0.33333333333333326
+    assert fb.areduce(report.accuracy, reducer=fb.mean, expand=fb.diff).value == 0.1481481481481481
+    assert fb.areduce(report.accuracy, reducer=fb.budget, expand=fb.diff).value == -1.09861228866811
```

## Comparing `fairbench-0.2.5.dist-info/METADATA` & `fairbench-0.2.6.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairbench
-Version: 0.2.5
+Version: 0.2.6
 Summary: Fairness model assessment framework
 Home-page: https://github.com/mever-team/FairBench
 Author: Emmanouil (Manios) Krasanakis
 Author-email: maniospas@hotmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -16,10 +16,11 @@
 Requires-Dist: distributed
 Requires-Dist: makefun
 Requires-Dist: matplotlib
 Requires-Dist: wget
 Requires-Dist: scikit-learn
 Requires-Dist: pandas
 Requires-Dist: objwrap
+Requires-Dist: bokeh
 
 For tutorials, documentation, and contribution guidelines, please visit the project's homepage at https://github.com/mever-team/FairBench
```

