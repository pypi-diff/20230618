# Comparing `tmp/xicorpy-0.3.tar.gz` & `tmp/xicorpy-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xicorpy-0.3.tar", max compression
+gzip compressed data, was "xicorpy-0.4.tar", max compression
```

## Comparing `xicorpy-0.3.tar` & `xicorpy-0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1076 2023-05-14 02:50:32.949022 xicorpy-0.3/LICENSE
--rw-r--r--   0        0        0     1479 2023-05-14 02:50:32.949022 xicorpy-0.3/README.md
--rw-r--r--   0        0        0     1534 2023-05-14 02:50:32.949022 xicorpy-0.3/pyproject.toml
--rw-r--r--   0        0        0      256 2023-05-14 02:50:32.949022 xicorpy-0.3/xicorpy/__init__.py
--rw-r--r--   0        0        0     1175 2023-05-14 02:50:32.949022 xicorpy-0.3/xicorpy/_utils.py
--rw-r--r--   0        0        0     8832 2023-05-14 02:50:32.949022 xicorpy-0.3/xicorpy/conditional_dependence.py
--rw-r--r--   0        0        0    12440 2023-05-14 02:50:32.949022 xicorpy-0.3/xicorpy/correlation.py
--rw-r--r--   0        0        0     4324 2023-05-14 02:50:32.949022 xicorpy-0.3/xicorpy/foci.py
--rw-r--r--   0        0        0     2967 1970-01-01 00:00:00.000000 xicorpy-0.3/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-18 00:32:26.747014 xicorpy-0.4/LICENSE
+-rw-r--r--   0        0        0     1479 2023-06-18 00:32:26.747014 xicorpy-0.4/README.md
+-rw-r--r--   0        0        0     1553 2023-06-18 00:32:26.747014 xicorpy-0.4/pyproject.toml
+-rw-r--r--   0        0        0      256 2023-06-18 00:32:26.747014 xicorpy-0.4/xicorpy/__init__.py
+-rw-r--r--   0        0        0     1175 2023-06-18 00:32:26.747014 xicorpy-0.4/xicorpy/_utils.py
+-rw-r--r--   0        0        0     8832 2023-06-18 00:32:26.747014 xicorpy-0.4/xicorpy/conditional_dependence.py
+-rw-r--r--   0        0        0    12440 2023-06-18 00:32:26.747014 xicorpy-0.4/xicorpy/correlation.py
+-rw-r--r--   0        0        0     5579 2023-06-18 00:32:26.747014 xicorpy-0.4/xicorpy/foci.py
+-rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 xicorpy-0.4/PKG-INFO
```

### Comparing `xicorpy-0.3/LICENSE` & `xicorpy-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xicorpy-0.3/README.md` & `xicorpy-0.4/README.md`

 * *Files identical despite different names*

### Comparing `xicorpy-0.3/pyproject.toml` & `xicorpy-0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xicorpy"
-version = "0.3"
+version = "0.4"
 description = "Python implementation of Chatterjee's Rank Correlation, its modifications, and other offshoots"
 authors = ["Swarna Vallabhaneni <swarnakumar@gmail.com>"]
 maintainers = ["Swarna Vallabhaneni <swarnakumar@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/swarnakumar/xicorpy"
 homepage = "https://swarnakumar.github.io/xicorpy"
@@ -21,15 +21,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 pandas = "^2"
 numpy = "^1.24"
 scikit-learn = "^1.2"
 mypy = "1.2"
-mkdocstrings = {version = "~0.20", optional = true}
+mkdocstrings = {version = "~0.20", optional = true, extras=["python"]}
 mkdocs-material = {version = "~9.1", optional = true}
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2"
 pytest-cov = "^4.0.0"
 pre-commit = "^2.16.0"
 coverage = {extras = ["toml"], version = "^7.2"}
```

### Comparing `xicorpy-0.3/xicorpy/_utils.py` & `xicorpy-0.4/xicorpy/_utils.py`

 * *Files identical despite different names*

### Comparing `xicorpy-0.3/xicorpy/conditional_dependence.py` & `xicorpy-0.4/xicorpy/conditional_dependence.py`

 * *Files identical despite different names*

### Comparing `xicorpy-0.3/xicorpy/correlation.py` & `xicorpy-0.4/xicorpy/correlation.py`

 * *Files identical despite different names*

### Comparing `xicorpy-0.3/xicorpy/foci.py` & `xicorpy-0.4/xicorpy/foci.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import warnings
-from typing import List, Union
+from typing import List, Union, Tuple
 
 import numpy.typing as npt
 
 from ._utils import validate_and_prepare_for_conditional_dependence
-from .conditional_dependence import compute_conditional_dependence_1d
+from .conditional_dependence import (
+    compute_conditional_dependence_1d,
+    compute_conditional_dependence,
+)
 
 
 class FOCI:
     """Class for computing FOCI."""
 
     def __init__(self, y: npt.ArrayLike, x: npt.ArrayLike):
         """
@@ -40,75 +43,99 @@
         next_p = max(codec, key=lambda k: codec[k])
         return next_p, codec[next_p]
 
     def select_features(
         self,
         num_features: int = None,
         init_selection: List[Union[int, str]] = None,
-    ) -> List[Union[int, str]]:
+        get_conditional_dependency: bool = False,
+    ) -> Union[List[Union[int, str]], Tuple[List[Union[int, str]], List[float]]]:
         """
         Selects features based on the Feature Ordering based on Conditional Independence (FOCI) algorithm in:
             [Azadkia and Chatterjee (2021). "A simple measure of conditional dependence", Annals of Statistics](https://arxiv.org/abs/1910.12327)
 
         Args:
             num_features: Maximum number of features to select. Defaults to the number of features in x.
             init_selection (list): Initial selection of features.
+            get_conditional_dependency (bool): If True, returns conditional dependency. Defaults to False
 
         Returns:
             list: List of selected features.
                 If x was `pd.DataFrame`, this will be column names.
                 Otherwise, this will be indices.
+            list: Conditional Dependency measure as each feature got selected
+                Only when get_conditional_dependency is True
 
         """
         if num_features is None:  # pragma: no cover
             num_features = self.x_df.shape[1]
 
         current_selection = [i for i in (init_selection or [])]
         if len(current_selection) >= num_features:
             warnings.warn("Initial selection is already complete")
+            if get_conditional_dependency:  # pragma: no cover
+                return current_selection, []
             return current_selection
 
+        codec = []
         stop = False
         while not stop and len(current_selection) < num_features:
             next_p, next_t = self._get_next_p(current_selection)
 
             if next_t <= 0:  # pragma: no cover
                 stop = True
             else:
                 current_selection.append(next_p)
+                if get_conditional_dependency:
+                    codec.append(
+                        compute_conditional_dependence(
+                            self.y_, self.x_df[current_selection]
+                        )
+                    )
+
+        if get_conditional_dependency:
+            return current_selection, codec
 
         return current_selection
 
 
 def select_features_using_foci(
     y: npt.ArrayLike,
     x: npt.ArrayLike,
     num_features: int = None,
     init_selection: List[Union[int, str]] = None,
-) -> List[Union[int, str]]:
+    get_conditional_dependency: bool = False,
+) -> Union[List[Union[int, str]], Tuple[List[Union[int, str]], List[float]]]:
     """
     Implements the FOCI algorithm for feature selection.
 
     Azadkia and Chatterjee (2021). "A simple measure of conditional dependence", Annals of Statistics.
     https://arxiv.org/abs/1910.12327.
 
     Args:
         y (npt.ArrayLike): The dependent variable. A single list or 1D array or a pandas Series.
         x (npt.ArrayLike): The independent variables. A single list or list of lists or 1D/2D numpy array or pd.Series or pd.DataFrame.
         num_features: Max number of features to select. Defaults to ALL features.
         init_selection (list): Initial selection of features.
             If `x` is a `pd.DataFrame`, this is expected to be a list of column names.
             Otherwise, this is expected to be a list of indices.
+        get_conditional_dependency (bool): If True, returns conditional dependency
 
     Returns:
         list: List of selected features.
             If x was `pd.DataFrame`, this will be column names.
             Otherwise, this will be indices.
+        list: Conditional Dependency measure as each feature got selected
+            Only when get_conditional_dependency is True
 
     Raises:
         ValueError: If y is not 1d.
         ValueError: If x is not 1d or 2d.
         ValueError: If y and x have different lengths.
         ValueError: If there are <= 2 valid y values.
 
     """
-    return FOCI(y, x).select_features(num_features, init_selection)
+    return FOCI(y, x).select_features(
+        num_features,
+        init_selection,
+        get_conditional_dependency=get_conditional_dependency,
+    )
```

### Comparing `xicorpy-0.3/PKG-INFO` & `xicorpy-0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xicorpy
-Version: 0.3
+Version: 0.4
 Summary: Python implementation of Chatterjee's Rank Correlation, its modifications, and other offshoots
 Home-page: https://swarnakumar.github.io/xicorpy
 License: MIT
 Author: Swarna Vallabhaneni
 Author-email: swarnakumar@gmail.com
 Maintainer: Swarna Vallabhaneni
 Maintainer-email: swarnakumar@gmail.com
@@ -21,15 +21,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: docs
 Provides-Extra: typings
 Requires-Dist: mkdocs-material (>=9.1,<9.2) ; extra == "docs"
-Requires-Dist: mkdocstrings (>=0.20,<0.21) ; extra == "docs"
+Requires-Dist: mkdocstrings[python] (>=0.20,<0.21) ; extra == "docs"
 Requires-Dist: mypy (==1.2) ; extra == "typings"
 Requires-Dist: numpy (>=1.24,<2.0)
 Requires-Dist: pandas (>=2,<3)
 Requires-Dist: scikit-learn (>=1.2,<2.0)
 Project-URL: Repository, https://github.com/swarnakumar/xicorpy
 Description-Content-Type: text/markdown
```

