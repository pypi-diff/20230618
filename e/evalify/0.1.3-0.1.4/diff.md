# Comparing `tmp/evalify-0.1.3.tar.gz` & `tmp/evalify-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evalify-0.1.3.tar", max compression
+gzip compressed data, was "evalify-0.1.4.tar", max compression
```

## Comparing `evalify-0.1.3.tar` & `evalify-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1516 2022-02-23 20:05:13.003132 evalify-0.1.3/LICENSE
--rw-r--r--   0        0        0     3779 2022-02-23 20:05:13.003132 evalify-0.1.3/README.md
--rw-r--r--   0        0        0      165 2022-02-23 20:05:13.003132 evalify-0.1.3/evalify/__init__.py
--rw-r--r--   0        0        0    16716 2022-02-23 20:05:13.003132 evalify-0.1.3/evalify/evalify.py
--rw-r--r--   0        0        0     2742 2022-02-23 20:05:13.003132 evalify-0.1.3/evalify/metrics.py
--rw-r--r--   0        0        0     1093 2022-02-23 20:05:13.003132 evalify-0.1.3/evalify/utils.py
--rw-r--r--   0        0        0     2619 2022-02-23 20:05:13.023132 evalify-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       37 2022-02-23 20:05:13.023132 evalify-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     9539 2022-02-23 20:05:13.023132 evalify-0.1.3/tests/test_evalify.py
--rw-r--r--   0        0        0     4512 2022-02-23 20:05:13.023132 evalify-0.1.3/tests/test_metrics.py
--rw-r--r--   0        0        0     1655 2022-02-23 20:05:13.023132 evalify-0.1.3/tests/test_utils.py
--rw-r--r--   0        0        0     5374 2022-02-23 20:09:17.392515 evalify-0.1.3/setup.py
--rw-r--r--   0        0        0     5867 2022-02-23 20:09:17.393102 evalify-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1516 2023-06-17 23:27:01.818756 evalify-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4225 2023-06-17 23:27:01.818756 evalify-0.1.4/README.md
+-rw-r--r--   0        0        0      165 2023-06-17 23:27:01.818756 evalify-0.1.4/evalify/__init__.py
+-rw-r--r--   0        0        0    19474 2023-06-17 23:27:01.818756 evalify-0.1.4/evalify/evalify.py
+-rw-r--r--   0        0        0     2742 2023-06-17 23:27:01.818756 evalify-0.1.4/evalify/metrics.py
+-rw-r--r--   0        0        0     1093 2023-06-17 23:27:01.818756 evalify-0.1.4/evalify/utils.py
+-rw-r--r--   0        0        0     2619 2023-06-17 23:27:01.838756 evalify-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-06-17 23:27:01.838756 evalify-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     9963 2023-06-17 23:27:01.838756 evalify-0.1.4/tests/test_evalify.py
+-rw-r--r--   0        0        0     4512 2023-06-17 23:27:01.838756 evalify-0.1.4/tests/test_metrics.py
+-rw-r--r--   0        0        0     1655 2023-06-17 23:27:01.838756 evalify-0.1.4/tests/test_utils.py
+-rw-r--r--   0        0        0     6330 1970-01-01 00:00:00.000000 evalify-0.1.4/PKG-INFO
```

### Comparing `evalify-0.1.3/LICENSE` & `evalify-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `evalify-0.1.3/evalify/evalify.py` & `evalify-0.1.4/evalify/evalify.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   experiment = Experiment()
   experiment.run(X, y)
   ```
   """
 import itertools
 import sys
 from collections import OrderedDict
-from typing import Any, Sequence, Union
+from typing import Any, List, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from sklearn.metrics import auc, confusion_matrix, roc_curve
 
 from evalify.metrics import (
     DISTANCE_TO_SIMILARITY,
@@ -49,15 +49,15 @@
         X: np.ndarray,
         y: np.ndarray,
         metrics: Union[str, Sequence[str]] = "cosine_similarity",
         same_class_samples: T_str_int = "full",
         different_class_samples: Union[str, int, Sequence[T_str_int]] = "minimal",
         batch_size: Union[T_str_int, None] = "best",
         shuffle: bool = False,
-        seed: int = None,
+        seed: Union[int, None] = None,
         return_embeddings: bool = False,
         p: int = 3,
     ) -> pd.DataFrame:
         """Runs an experiment for face verification
 
         Args:
             X: Embeddings array
@@ -173,15 +173,16 @@
 
     def _get_pairs(
         self,
         y,
         same_class_samples,
         different_class_samples,
         target,
-    ):
+    ) -> List[Tuple]:
+        """Generates experiment pairs."""
         same_ixs_full = np.argwhere(y == target).ravel()
         if isinstance(same_class_samples, int):
             same_class_samples = min(len(same_ixs_full), same_class_samples)
             same_ixs = self.rng.choice(same_ixs_full, same_class_samples)
         elif same_class_samples == "full":
             same_ixs = same_ixs_full
         same_pairs = itertools.combinations(same_ixs, 2)
@@ -210,15 +211,16 @@
         )
         different_pairs = [(a, b, target, y[b], 0) for a, b in different_pairs if a < b]
 
         return same_pairs + different_pairs
 
     def _validate_args(
         self, metrics, same_class_samples, different_class_samples, batch_size, p
-    ):
+    ) -> None:
+        """Validates passed arguments to Experiment.run() method."""
         if same_class_samples != "full" and not isinstance(same_class_samples, int):
             raise ValueError(
                 "`same_class_samples` argument must be one of 'full' or an integer "
                 f"Received: same_class_samples={same_class_samples}"
             )
 
         if different_class_samples not in ("full", "minimal"):
@@ -258,20 +260,20 @@
         if any(metric not in metrics_caller for metric in metrics):
             raise ValueError(
                 f"`metric` argument must be one of {tuple(metrics_caller.keys())} "
                 f"Received: metric={metrics}"
             )
 
         if p < 1:
-            raise ValueError(f"`p` must be at least 1. Received: p={p}")
+            raise ValueError(f"`p` must be an int and at least 1. Received: p={p}")
 
     def find_optimal_cutoff(self):
         """Find the optimal cutoff point
         Returns:
-            float: optimal cutoff value
+            float: Optimal cutoff value
 
         """
         self.check_experiment_run()
         self.optimal_cutoff = {}
         for metric in self.metrics:
             fpr, tpr, threshold = roc_curve(self.df["target"], self.df[metric])
             i = np.arange(len(tpr))
@@ -282,15 +284,15 @@
                 }
             )
             roc_t = roc.iloc[(roc.tf - 0).abs().argsort()[:1]]
             self.optimal_cutoff[metric] = roc_t["threshold"].item()
         return self.optimal_cutoff
 
     def find_threshold_at_fpr(self, fpr: float):
-        """Runs an experiment for face verification
+        """Finds optimal threshold at a given FPR.
 
         Args:
             fpr: False positive rate to find best threshold for.
         Returns:
             dict: A dictionary with keys as metrics and values as thresholds.
         Raises:
             ValueError: If `fpr` is not between 0 and 1.
@@ -310,15 +312,15 @@
             ix_left = np.searchsorted(df_fpr_tpr["FPR"], fpr, side="left")
             ix_right = np.searchsorted(df_fpr_tpr["FPR"], fpr, side="right")
 
             if fpr == 0:
                 best = df_fpr_tpr.iloc[ix_right]
             elif fpr == 1 or ix_left == ix_right:
                 best = df_fpr_tpr.iloc[ix_left]
-            else: 
+            else:
                 best = (
                     df_fpr_tpr.iloc[ix_left]
                     if abs(df_fpr_tpr.iloc[ix_left].FPR - fpr)
                     < abs(df_fpr_tpr.iloc[ix_right].FPR - fpr)
                     else df_fpr_tpr.iloc[ix_right]
                 )
             best = best.to_dict()
@@ -326,28 +328,35 @@
                 best["Threshold"] = REVERSE_DISTANCE_TO_SIMILARITY.get(metric)(
                     best["Threshold"]
                 )
             threshold_at_fpr[metric] = best
         return threshold_at_fpr
 
     def get_binary_prediction(self, metric, threshold):
+        """Find binary prediction from distance or similarity.
+        Args:
+            metric: Metric name for the desired prediction.
+            threshold: Cut off threshold.
+        Returns:
+            pd.Series: Binary predictions.
+        """
         return (
             self.df[metric].apply(lambda x: 1 if x < threshold else 0)
             if metric in DISTANCE_TO_SIMILARITY
             else self.df[metric].apply(lambda x: 1 if x > threshold else 0)
         )
 
     def evaluate_at_threshold(self, threshold: float, metric: str):
         """Evaluate performance at specific threshold
         Args:
-            threshold: cut-off threshold.
-            metric: metric to use.
+            threshold: Cut-off threshold.
+            metric: Metric to use.
 
         Returns:
-            dict: containing all evaluation metrics.
+            dict: A dict ontaining all evaluation metrics.
         """
         self.metrics_evaluation = {}
         self.check_experiment_run(metric)
         for metric in self.metrics:
             predicted = self.get_binary_prediction(metric, threshold)
             cm = confusion_matrix(self.df["target"], predicted)
             tn, fp, fn, tp = cm.ravel()
@@ -391,30 +400,80 @@
         if metric is not None and metric not in self.metrics:
             raise ValueError(
                 f"`{caller}` function was can only be called with `metric` from "
                 f"{self.metrics} which were used while running the experiment"
             )
         return True
 
-    def get_roc_auc(self):
+    def get_roc_auc(self) -> OrderedDict:
+        """Find ROC AUC for all the metrics used.
+        Returns:
+            collections.OrderedDict: An OrderedDict with AUC for all metrics.
+        """
         self.check_experiment_run()
         self.roc_auc = {}
         for metric in self.metrics:
             predicted = self.predicted_as_similarity(metric)
             fpr, tpr, thresholds = roc_curve(
                 self.df["target"], predicted, drop_intermediate=False
             )
             self.roc_auc[metric] = auc(fpr, tpr)
         self.roc_auc = OrderedDict(
             sorted(self.roc_auc.items(), key=lambda x: x[1], reverse=True)
         )
         return self.roc_auc
 
-    def predicted_as_similarity(self, metric):
+    def predicted_as_similarity(self, metric: str) -> pd.Series:
+        """Convert distance metrics to a similarity measure.
+        Args:
+            metric: distance metric to convert to similarity. If a similarity metric is
+                passed, It gets returned unchanged.
+        Returns:
+            pd.Series: Converted distance to similarity.
+
+        """
         predicted = self.df[metric]
         if metric in DISTANCE_TO_SIMILARITY:
             predicted = (
                 self.cached_predicted_as_similarity[metric]
                 if metric in self.cached_predicted_as_similarity
                 else DISTANCE_TO_SIMILARITY.get(metric)(predicted)
             )
+            self.cached_predicted_as_similarity[metric] = predicted
         return predicted
+    
+    def calculate_eer(self) -> OrderedDict:
+        """
+        Calculates the Equal Error Rate (EER) for each metric.
+
+        Returns an ordered dictionary containing the EER value and threshold for each metric.
+        The metrics are sorted in ascending order based on the EER values.
+
+        Returns:
+            OrderedDict: A dictionary containing the EER value and threshold for each metric.
+                The metrics are sorted in ascending order based on the EER values.
+                Example: {'metric1': {'EER': 0.123, 'Threshold': 0.456},
+                        ...}
+        """
+        self.check_experiment_run()
+        self.eer = {}
+        for metric in self.metrics:
+            predicted = self.predicted_as_similarity(metric)
+            actual = self.df["target"]
+
+            # Calculate False Positive Rate (FPR) and True Positive Rate (TPR)
+            fpr, tpr, thresholds = roc_curve(actual, predicted, pos_label=1, drop_intermediate=False)
+            fnr = 1 - tpr
+            eer_threshold = thresholds[np.nanargmin(np.absolute(fnr - fpr))]
+            # theoretically eer from fpr and eer from fnr should be identical but they can be slightly differ in reality
+            eer_1 = fpr[np.nanargmin(np.absolute((fnr - fpr)))]
+            eer_2 = fnr[np.nanargmin(np.absolute((fnr - fpr)))]
+            if metric in REVERSE_DISTANCE_TO_SIMILARITY:
+                eer_threshold = REVERSE_DISTANCE_TO_SIMILARITY.get(metric)(eer_threshold)
+
+            # return the mean of eer from fpr and from fnr
+            self.eer[metric] = {'EER': (eer_1 + eer_2) / 2, 'Threshold': eer_threshold}
+        self.eer = OrderedDict(
+            sorted(self.eer.items(), key=lambda x: x[1]['EER'], reverse=False)
+        )
+
+        return self.eer
```

### Comparing `evalify-0.1.3/evalify/metrics.py` & `evalify-0.1.4/evalify/metrics.py`

 * *Files identical despite different names*

### Comparing `evalify-0.1.3/evalify/utils.py` & `evalify-0.1.4/evalify/utils.py`

 * *Files identical despite different names*

### Comparing `evalify-0.1.3/pyproject.toml` & `evalify-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 [tool]
 [tool.poetry]
 name = "evalify"
-version = "0.1.3"
+version = "0.1.4"
 homepage = "https://github.com/ma7555/evalify"
 description = "Evaluate your face  or voice verification models literally in seconds."
 authors = ["Mahmoud Bahaa <mah.alaa@nu.edu.eg>"]
 readme = "README.md"
 license =  "BSD-3-Clause"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: BSD License',
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+
 ]
 packages = [
     { include = "evalify" },
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7.1,<4.0"
+python = ">=3.8,<4.0"
 pandas = "^1.3.5"
 numpy = "^1.16.0"
 psutil = "^5.0.0"
-scikit-learn = "^1.0.0"
+scikit-learn = "^1.1.0"
 
 black  = { version = "22.1.0", optional = true}
 isort  = { version = "5.10.1", optional = true}
 flake8  = { version = "4.0.1", optional = true}
 flake8-docstrings = { version = "^1.6.0", optional = true }
 pytest  = { version = "^7.0.1", optional = true}
 pytest-cov  = { version = "^3.0.0", optional = true}
```

### Comparing `evalify-0.1.3/tests/test_evalify.py` & `evalify-0.1.4/tests/test_evalify.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,14 +175,29 @@
         fpr_d1 = experiment.find_threshold_at_fpr(1)
         fpr_d0 = experiment.find_threshold_at_fpr(0)
         self.assertEqual(len(fpr_d01[metric]), 3)
         self.assertAlmostEqual(fpr_d01[metric]["Threshold"], 0.8939142, 3)
         self.assertAlmostEqual(fpr_d0[metric]["Threshold"], 0.9953355, 3)
         self.assertAlmostEqual(fpr_d1[metric]["Threshold"], 0.2060538, 3)
 
+
+    def test_run_calculate_eer(self):
+        """Test run with calculate_eer"""
+        experiment = Experiment()
+        metric = "cosine_similarity"
+        df = experiment.run(
+            self.embs,
+            self.targets,
+            metrics=metric,
+            different_class_samples=("full", "full"),
+        ) 
+        eer  = experiment.calculate_eer()
+        self.assertTrue('EER' in eer[metric])
+
+
     def test__call__(self):
         """Test run with __call__"""
         experiment = Experiment()
         result = experiment.run(self.embs, self.targets, seed=555)
         result_2 = experiment(self.embs, self.targets, seed=555)
         self.assertTrue(np.array_equal(result.to_numpy(), result_2.to_numpy()))
 
@@ -217,15 +232,15 @@
             experiment = Experiment()
             _ = experiment.run(self.embs, self.targets, batch_size="all")
 
         with self.assertRaisesRegex(ValueError, "`metric` argument must be one of "):
             experiment = Experiment()
             _ = experiment.run(self.embs, self.targets, metrics="dot_prod")
 
-        with self.assertRaisesRegex(ValueError, "`p` must be at least 1. Received: p="):
+        with self.assertRaisesRegex(ValueError, "`p` must be an int and at least 1. Received: p="):
             experiment = Experiment()
             _ = experiment.run(self.embs, self.targets, p=0.1)
 
         with self.assertRaisesRegex(
             NotImplementedError,
             "`evaluate_at_threshold` function can only be run after running "
             "`run_experiment`.",
```

### Comparing `evalify-0.1.3/tests/test_metrics.py` & `evalify-0.1.4/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `evalify-0.1.3/tests/test_utils.py` & `evalify-0.1.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `evalify-0.1.3/PKG-INFO` & `evalify-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 Metadata-Version: 2.1
 Name: evalify
-Version: 0.1.3
+Version: 0.1.4
 Summary: Evaluate your face  or voice verification models literally in seconds.
 Home-page: https://github.com/ma7555/evalify
 License: BSD-3-Clause
 Author: Mahmoud Bahaa
 Author-email: mah.alaa@nu.edu.eg
-Requires-Python: >=3.7.1,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
-Requires-Dist: black (==22.1.0); extra == "test"
-Requires-Dist: flake8 (==4.0.1); extra == "test"
-Requires-Dist: flake8-docstrings (>=1.6.0,<2.0.0); extra == "test"
-Requires-Dist: isort (==5.10.1); extra == "test"
-Requires-Dist: livereload (>=2.6.3,<3.0.0); extra == "doc"
-Requires-Dist: mkdocs (>=1.2.3,<2.0.0); extra == "doc"
-Requires-Dist: mkdocs-autorefs (>=0.3.1,<0.4.0); extra == "doc"
-Requires-Dist: mkdocs-include-markdown-plugin (>=3.2.3,<4.0.0); extra == "doc"
-Requires-Dist: mkdocs-material (>=8.1.11,<9.0.0); extra == "doc"
+Requires-Dist: black (==22.1.0) ; extra == "test"
+Requires-Dist: flake8 (==4.0.1) ; extra == "test"
+Requires-Dist: flake8-docstrings (>=1.6.0,<2.0.0) ; extra == "test"
+Requires-Dist: isort (==5.10.1) ; extra == "test"
+Requires-Dist: livereload (>=2.6.3,<3.0.0) ; extra == "doc"
+Requires-Dist: mkdocs (>=1.2.3,<2.0.0) ; extra == "doc"
+Requires-Dist: mkdocs-autorefs (>=0.3.1,<0.4.0) ; extra == "doc"
+Requires-Dist: mkdocs-include-markdown-plugin (>=3.2.3,<4.0.0) ; extra == "doc"
+Requires-Dist: mkdocs-material (>=8.1.11,<9.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-material-extensions (>=1.0.3,<2.0.0)
-Requires-Dist: mkdocstrings (>=0.18.0,<0.19.0); extra == "doc"
+Requires-Dist: mkdocstrings (>=0.18.0,<0.19.0) ; extra == "doc"
 Requires-Dist: numpy (>=1.16.0,<2.0.0)
 Requires-Dist: pandas (>=1.3.5,<2.0.0)
-Requires-Dist: pip (>=22.0.3,<23.0.0); extra == "dev"
+Requires-Dist: pip (>=22.0.3,<23.0.0) ; extra == "dev"
 Requires-Dist: psutil (>=5.0.0,<6.0.0)
-Requires-Dist: pyreadline (>=2.1,<3.0); extra == "test"
-Requires-Dist: pytest (>=7.0.1,<8.0.0); extra == "test"
-Requires-Dist: pytest-cov (>=3.0.0,<4.0.0); extra == "test"
-Requires-Dist: scikit-learn (>=1.0.0,<2.0.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0); extra == "dev"
-Requires-Dist: tox (>=3.24.5,<4.0.0); extra == "dev"
-Requires-Dist: twine (>=3.8.0,<4.0.0); extra == "dev"
-Requires-Dist: virtualenv (>=20.13.1,<21.0.0); extra == "dev"
+Requires-Dist: pyreadline (>=2.1,<3.0) ; extra == "test"
+Requires-Dist: pytest (>=7.0.1,<8.0.0) ; extra == "test"
+Requires-Dist: pytest-cov (>=3.0.0,<4.0.0) ; extra == "test"
+Requires-Dist: scikit-learn (>=1.1.0,<2.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "dev"
+Requires-Dist: tox (>=3.24.5,<4.0.0) ; extra == "dev"
+Requires-Dist: twine (>=3.8.0,<4.0.0) ; extra == "dev"
+Requires-Dist: virtualenv (>=20.13.1,<21.0.0) ; extra == "dev"
 Description-Content-Type: text/markdown
 
 # evalify
 
 <p align="center">
 
 <img src="https://user-images.githubusercontent.com/7144929/154332210-fa1fee34-faae-4567-858a-49fa53e99a2b.svg" width="292" height="120" alt="Logo"/>
@@ -75,36 +75,32 @@
 </a>
 <a href="https://github.com/psf/black">
     <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black">
 </a>
 <a href="https://codecov.io/gh/ma7555/evalify">
   <img src="https://codecov.io/gh/ma7555/evalify/branch/main/graph/badge.svg" />
 </a>
-<a href="https://github.com/ma7555/evalify/releases"><img alt="GitHub all releases" src="https://img.shields.io/github/downloads/ma7555/evalify/total">
+<a href="https://pypi.org/project/evalify/"><img alt="PyPI Downloads/Month" src="https://img.shields.io/pypi/dm/evalify">
 </a>
 
 </p>
 
-
-Evaluate your face or voice verification models literally in seconds.
+**Evaluate Biometric Authentication Models Literally in Seconds.**
 
 ## Installation
-#### Stable release
+#### Stable release:
 ```bash
 pip install evalify
 ```
-#### Bleeding edge
-* From source
-    ```bash
-    pip install git+https://github.com/ma7555/evalify.git
-    ```
-* From TestPyPI
-    ```bash
-    pip install --index-url https://test.pypi.org/simple/ evalify
-    ```
+#### Bleeding edge:
+```bash
+pip install git+https://github.com/ma7555/evalify.git
+```
+## Used for
+Evaluating all biometric authentication models, where the model output is a high-level embeddings known as feature vectors for visual or behaviour biometrics or d-vectors for auditory biometrics.
 
 ## Usage
 
 ```python
 import numpy as np
 from evalify import Experiment
 
@@ -114,26 +110,30 @@
 nclasses = 10
 X = rng.random((self.nphotos, self.emb_size))
 y = rng.integers(self.nclasses, size=self.nphotos)
 
 experiment = Experiment()
 experiment.run(X, y)
 experiment.get_roc_auc()
-print(experiment.df.roc_auc)
+print(experiment.roc_auc)
 print(experiment.find_threshold_at_fpr(0.01))
 ```
+## How it works
+* When you run an experiment, evalify tries all the possible combinations between individuals for authentication based on the `X` and `y` parameters and returns the results including FPR, TPR, FNR, TNR and ROC AUC. `X` is an array of embeddings and `y` is an array of corresponding targets.
+* Evalify can find the optimal threshold based on your agreed FPR and desired similarity or distance metric.
+
 ## Documentation: 
 * <https://ma7555.github.io/evalify/>
 
 
 ## Features
 
 * Blazing fast implementation for metrics calculation through optimized einstein sum and vectorized calculations.
 * Many operations are dispatched to canonical BLAS, cuBLAS, or other specialized routines.
-* Smart sampling options using direct indexing from pre-calculated arrays with an option to have fine control over sampling strategy and sampling numbers.
+* Smart sampling options using direct indexing from pre-calculated arrays with total control over sampling strategy and sampling numbers.
 * Supports most evaluation metrics:
     - `cosine_similarity`
     - `pearson_similarity`
     - `cosine_distance`
     - `euclidean_distance`
     - `euclidean_distance_l2`
     - `minkowski_distance`
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,56 +1,64 @@
-Metadata-Version: 2.1 Name: evalify Version: 0.1.3 Summary: Evaluate your face
+Metadata-Version: 2.1 Name: evalify Version: 0.1.4 Summary: Evaluate your face
 or voice verification models literally in seconds. Home-page: https://
 github.com/ma7555/evalify License: BSD-3-Clause Author: Mahmoud Bahaa Author-
-email: mah.alaa@nu.edu.eg Requires-Python: >=3.7.1,<4.0 Classifier: Development
+email: mah.alaa@nu.edu.eg Requires-Python: >=3.8,<4.0 Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: BSD License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Provides-Extra: dev Provides-Extra: doc Provides-
-Extra: test Requires-Dist: black (==22.1.0); extra == "test" Requires-Dist:
-flake8 (==4.0.1); extra == "test" Requires-Dist: flake8-docstrings
-(>=1.6.0,<2.0.0); extra == "test" Requires-Dist: isort (==5.10.1); extra ==
-"test" Requires-Dist: livereload (>=2.6.3,<3.0.0); extra == "doc" Requires-
-Dist: mkdocs (>=1.2.3,<2.0.0); extra == "doc" Requires-Dist: mkdocs-autorefs
-(>=0.3.1,<0.4.0); extra == "doc" Requires-Dist: mkdocs-include-markdown-plugin
-(>=3.2.3,<4.0.0); extra == "doc" Requires-Dist: mkdocs-material
-(>=8.1.11,<9.0.0); extra == "doc" Requires-Dist: mkdocs-material-extensions
-(>=1.0.3,<2.0.0) Requires-Dist: mkdocstrings (>=0.18.0,<0.19.0); extra == "doc"
-Requires-Dist: numpy (>=1.16.0,<2.0.0) Requires-Dist: pandas (>=1.3.5,<2.0.0)
-Requires-Dist: pip (>=22.0.3,<23.0.0); extra == "dev" Requires-Dist: psutil
-(>=5.0.0,<6.0.0) Requires-Dist: pyreadline (>=2.1,<3.0); extra == "test"
-Requires-Dist: pytest (>=7.0.1,<8.0.0); extra == "test" Requires-Dist: pytest-
-cov (>=3.0.0,<4.0.0); extra == "test" Requires-Dist: scikit-learn
-(>=1.0.0,<2.0.0) Requires-Dist: toml (>=0.10.2,<0.11.0); extra == "dev"
-Requires-Dist: tox (>=3.24.5,<4.0.0); extra == "dev" Requires-Dist: twine
-(>=3.8.0,<4.0.0); extra == "dev" Requires-Dist: virtualenv (>=20.13.1,<21.0.0);
-extra == "dev" Description-Content-Type: text/markdown # evalify
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Provides-Extra: dev Provides-Extra: doc Provides-
+Extra: test Requires-Dist: black (==22.1.0) ; extra == "test" Requires-Dist:
+flake8 (==4.0.1) ; extra == "test" Requires-Dist: flake8-docstrings
+(>=1.6.0,<2.0.0) ; extra == "test" Requires-Dist: isort (==5.10.1) ; extra ==
+"test" Requires-Dist: livereload (>=2.6.3,<3.0.0) ; extra == "doc" Requires-
+Dist: mkdocs (>=1.2.3,<2.0.0) ; extra == "doc" Requires-Dist: mkdocs-autorefs
+(>=0.3.1,<0.4.0) ; extra == "doc" Requires-Dist: mkdocs-include-markdown-plugin
+(>=3.2.3,<4.0.0) ; extra == "doc" Requires-Dist: mkdocs-material
+(>=8.1.11,<9.0.0) ; extra == "doc" Requires-Dist: mkdocs-material-extensions
+(>=1.0.3,<2.0.0) Requires-Dist: mkdocstrings (>=0.18.0,<0.19.0) ; extra ==
+"doc" Requires-Dist: numpy (>=1.16.0,<2.0.0) Requires-Dist: pandas
+(>=1.3.5,<2.0.0) Requires-Dist: pip (>=22.0.3,<23.0.0) ; extra == "dev"
+Requires-Dist: psutil (>=5.0.0,<6.0.0) Requires-Dist: pyreadline (>=2.1,<3.0) ;
+extra == "test" Requires-Dist: pytest (>=7.0.1,<8.0.0) ; extra == "test"
+Requires-Dist: pytest-cov (>=3.0.0,<4.0.0) ; extra == "test" Requires-Dist:
+scikit-learn (>=1.1.0,<2.0.0) Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra ==
+"dev" Requires-Dist: tox (>=3.24.5,<4.0.0) ; extra == "dev" Requires-Dist:
+twine (>=3.8.0,<4.0.0) ; extra == "dev" Requires-Dist: virtualenv
+(>=20.13.1,<21.0.0) ; extra == "dev" Description-Content-Type: text/markdown #
+evalify
                                     [Logo]
   [License] [DOI] [Python_3.7_|_3.8_|_3.9_|_3] [Release_Status] [CI_Status]
    [Documentation_Status] [Code_style:_black] [https://codecov.io/gh/ma7555/
-          evalify/branch/main/graph/badge.svg] [GitHub_all_releases]
-Evaluate your face or voice verification models literally in seconds. ##
-Installation #### Stable release ```bash pip install evalify ``` #### Bleeding
-edge * From source ```bash pip install git+https://github.com/ma7555/
-evalify.git ``` * From TestPyPI ```bash pip install --index-url https://
-test.pypi.org/simple/ evalify ``` ## Usage ```python import numpy as np from
-evalify import Experiment rng = np.random.default_rng() nphotos = 500 emb_size
-= 32 nclasses = 10 X = rng.random((self.nphotos, self.emb_size)) y =
-rng.integers(self.nclasses, size=self.nphotos) experiment = Experiment()
-experiment.run(X, y) experiment.get_roc_auc() print(experiment.df.roc_auc)
-print(experiment.find_threshold_at_fpr(0.01)) ``` ## Documentation: *
+          evalify/branch/main/graph/badge.svg] [PyPI_Downloads/Month]
+**Evaluate Biometric Authentication Models Literally inÂ Seconds.** ##
+Installation #### Stable release: ```bash pip install evalify ``` #### Bleeding
+edge: ```bash pip install git+https://github.com/ma7555/evalify.git ``` ## Used
+for Evaluating all biometric authentication models, where the model output is a
+high-level embeddings known as feature vectors for visual or behaviour
+biometrics or d-vectors for auditory biometrics. ## Usage ```python import
+numpy as np from evalify import Experiment rng = np.random.default_rng()
+nphotos = 500 emb_size = 32 nclasses = 10 X = rng.random((self.nphotos,
+self.emb_size)) y = rng.integers(self.nclasses, size=self.nphotos) experiment =
+Experiment() experiment.run(X, y) experiment.get_roc_auc() print
+(experiment.roc_auc) print(experiment.find_threshold_at_fpr(0.01)) ``` ## How
+it works * When you run an experiment, evalify tries all the possible
+combinations between individuals for authentication based on the `X` and `y`
+parameters and returns the results including FPR, TPR, FNR, TNR and ROC AUC.
+`X` is an array of embeddings and `y` is an array of corresponding targets. *
+Evalify can find the optimal threshold based on your agreed FPR and desired
+similarity or distance metric. ## Documentation: *
 ma7555.github.io/evalify/> ## Features * Blazing fast implementation for
 metrics calculation through optimized einstein sum and vectorized calculations.
 * Many operations are dispatched to canonical BLAS, cuBLAS, or other
 specialized routines. * Smart sampling options using direct indexing from pre-
-calculated arrays with an option to have fine control over sampling strategy
-and sampling numbers. * Supports most evaluation metrics: - `cosine_similarity`
-- `pearson_similarity` - `cosine_distance` - `euclidean_distance` -
+calculated arrays with total control over sampling strategy and sampling
+numbers. * Supports most evaluation metrics: - `cosine_similarity` -
+`pearson_similarity` - `cosine_distance` - `euclidean_distance` -
 `euclidean_distance_l2` - `minkowski_distance` - `manhattan_distance` -
 `chebyshev_distance` * Computation time for 4 metrics 4.2 million samples
 experiment is **24 seconds vs 51 minutes** if looping using
 `scipy.spatial.distance` implemntations. ## TODO * Safer memory allocation. I
 did not have issues but if you ran out of memory please manually set the
 `batch_size` argument. ## Contribution * Contributions are welcomed, and they
 are greatly appreciated! Every little bit helps, and credit will always be
```

