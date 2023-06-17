# Comparing `tmp/history_matching-0.0.8.tar.gz` & `tmp/history_matching-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "history_matching-0.0.8.tar", last modified: Mon Feb 27 21:13:21 2023, max compression
+gzip compressed data, was "history_matching-0.0.9.tar", last modified: Tue Feb 28 22:40:41 2023, max compression
```

## Comparing `history_matching-0.0.8.tar` & `history_matching-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 21:13:21.416789 history_matching-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35128 2023-02-27 21:12:53.000000 history_matching-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-02-27 21:13:21.416789 history_matching-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-02-27 21:12:53.000000 history_matching-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-02-27 21:12:53.000000 history_matching-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 21:13:21.416789 history_matching-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-27 21:12:53.000000 history_matching-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 21:13:21.416789 history_matching-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 21:13:21.416789 history_matching-0.0.8/src/history_matching/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 21:12:53.000000 history_matching-0.0.8/src/history_matching/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 21:13:21.416789 history_matching-0.0.8/src/history_matching/emulator/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-27 21:12:53.000000 history_matching-0.0.8/src/history_matching/emulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-02-27 21:12:53.000000 history_matching-0.0.8/src/history_matching/emulator/emulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 21:13:21.416789 history_matching-0.0.8/src/history_matching/samples/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-27 21:12:53.000000 history_matching-0.0.8/src/history_matching/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-02-27 21:12:53.000000 history_matching-0.0.8/src/history_matching/samples/sample_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-02-27 21:12:53.000000 history_matching-0.0.8/src/history_matching/samples/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 21:13:21.416789 history_matching-0.0.8/src/history_matching.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-02-27 21:13:21.000000 history_matching-0.0.8/src/history_matching.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-02-27 21:13:21.000000 history_matching-0.0.8/src/history_matching.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 21:13:21.000000 history_matching-0.0.8/src/history_matching.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-27 21:13:21.000000 history_matching-0.0.8/src/history_matching.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:40:41.372324 history_matching-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35128 2023-02-28 22:40:12.000000 history_matching-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-02-28 22:40:41.372324 history_matching-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-02-28 22:40:12.000000 history_matching-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-02-28 22:40:12.000000 history_matching-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 22:40:41.372324 history_matching-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-28 22:40:12.000000 history_matching-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:40:41.368324 history_matching-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:40:41.368324 history_matching-0.0.9/src/history_matching/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 22:40:12.000000 history_matching-0.0.9/src/history_matching/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:40:41.368324 history_matching-0.0.9/src/history_matching/emulator/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-28 22:40:12.000000 history_matching-0.0.9/src/history_matching/emulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-02-28 22:40:12.000000 history_matching-0.0.9/src/history_matching/emulator/emulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:40:41.372324 history_matching-0.0.9/src/history_matching/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-28 22:40:12.000000 history_matching-0.0.9/src/history_matching/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-02-28 22:40:12.000000 history_matching-0.0.9/src/history_matching/samples/sample_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-02-28 22:40:12.000000 history_matching-0.0.9/src/history_matching/samples/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:40:41.368324 history_matching-0.0.9/src/history_matching.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-02-28 22:40:41.000000 history_matching-0.0.9/src/history_matching.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-02-28 22:40:41.000000 history_matching-0.0.9/src/history_matching.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 22:40:41.000000 history_matching-0.0.9/src/history_matching.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-02-28 22:40:41.000000 history_matching-0.0.9/src/history_matching.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-28 22:40:41.000000 history_matching-0.0.9/src/history_matching.egg-info/top_level.txt
```

### Comparing `history_matching-0.0.8/LICENSE` & `history_matching-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `history_matching-0.0.8/PKG-INFO` & `history_matching-0.0.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: history_matching
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package contains helper modules for using history matching for parameter optimzation.
 Author-email: Robert King <robcking@stanford.edu>
 Project-URL: Homepage, https://github.com/OneOneFour/History-Matching-Core
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `history_matching-0.0.8/pyproject.toml` & `history_matching-0.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0","netcdf4>=1.6.2","xarray>=2023.2.0","joblib>=1.2.0","numpy>=1.24.2","pyDOE>=0.3.8","scikit-learn>=1.2.1","scipy>=1.10.0","threadpoolctl>=3.1.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "history_matching"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Robert King", email="robcking@stanford.edu" },
 ]
 description = "Package contains helper modules for using history matching for parameter optimzation."
+dependencies = ["netcdf4>=1.6.2","xarray>=2023.2.0","joblib>=1.2.0","numpy>=1.24.2","pyDOE>=0.3.8","scikit-learn>=1.2.1","scipy>=1.10.0"]
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
```

### Comparing `history_matching-0.0.8/src/history_matching/emulator/emulator.py` & `history_matching-0.0.9/src/history_matching/emulator/emulator.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from sklearn.gaussian_process import GaussianProcessRegressor
 from sklearn.preprocessing import StandardScaler
 
 from ..samples import SampleSpace
 
 
 def implausibility(
-    predict_mean: np.ndarray,
-    predict_err: np.ndarray,
+    predict_mean: xr.DataArray,
+    predict_err: xr.DataArray,
     obs_mean: np.ndarray,
     obs_err: np.ndarray,
 ):
     """
     Calculate implausibility score for set of predictions
 
     Input:
@@ -22,22 +22,22 @@
     predict_err - Standard Error in predictions
     obs_err- Standard error in mean of observations
     """
     n_features = obs_mean.shape[0]
     if n_features != predict_mean.shape[0]:
         raise ValueError("Incompatible shapes between observations and predictions")
     return np.sqrt(
-        np.sum(
+        xr.concat(
             [
                 (predict_mean[i] - obs_mean[i]) ** 2
                 / (predict_err[i] ** 2 + obs_err[i] ** 2)
                 for i in range(n_features)
             ],
-            axis=0,
-        )
+            dim="n_features",
+        ).sum(dim="n_features")
     )
 
 
 class GPEmulator(BaseEstimator):
     def __init__(self, n_features=2, random_state=None, kernel=None):
         self.random_state = random_state
         self.kernel = kernel
```

### Comparing `history_matching-0.0.8/src/history_matching/samples/sample_space.py` & `history_matching-0.0.9/src/history_matching/samples/sample_space.py`

 * *Files identical despite different names*

### Comparing `history_matching-0.0.8/src/history_matching/samples/stats.py` & `history_matching-0.0.9/src/history_matching/samples/stats.py`

 * *Files identical despite different names*

### Comparing `history_matching-0.0.8/src/history_matching.egg-info/PKG-INFO` & `history_matching-0.0.9/src/history_matching.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: history-matching
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package contains helper modules for using history matching for parameter optimzation.
 Author-email: Robert King <robcking@stanford.edu>
 Project-URL: Homepage, https://github.com/OneOneFour/History-Matching-Core
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

