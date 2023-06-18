# Comparing `tmp/tsfeatures-0.4.1.tar.gz` & `tmp/tsfeatures-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsfeatures-0.4.1.tar", last modified: Sun Jun 18 02:44:53 2023, max compression
+gzip compressed data, was "tsfeatures-0.4.2.tar", last modified: Sun Jun 18 03:47:36 2023, max compression
```

## Comparing `tsfeatures-0.4.1.tar` & `tsfeatures-0.4.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:44:53.100658 tsfeatures-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-06-18 02:44:53.100658 tsfeatures-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 02:44:53.100658 tsfeatures-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:44:53.096658 tsfeatures-0.4.1/tsfeatures/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/compare_with_r.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/m4_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:44:53.100658 tsfeatures-0.4.1/tsfeatures/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/metrics/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:44:53.100658 tsfeatures-0.4.1/tsfeatures/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/tests/test_acf_features.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/tests/test_arch_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/tests/test_holt_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/tests/test_pacf_features.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/tests/test_sparsity.py
--rw-r--r--   0 runner    (1001) docker     (123)    28105 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/tsfeatures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/tsfeatures_r.py
--rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:44:53.100658 tsfeatures-0.4.1/tsfeatures.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-06-18 02:44:53.000000 tsfeatures-0.4.1/tsfeatures.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-18 02:44:53.000000 tsfeatures-0.4.1/tsfeatures.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:44:53.000000 tsfeatures-0.4.1/tsfeatures.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-18 02:44:53.000000 tsfeatures-0.4.1/tsfeatures.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-18 02:44:53.000000 tsfeatures-0.4.1/tsfeatures.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:47:36.979164 tsfeatures-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-06-18 03:47:27.000000 tsfeatures-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-06-18 03:47:36.979164 tsfeatures-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-06-18 03:47:27.000000 tsfeatures-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 03:47:36.979164 tsfeatures-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-18 03:47:27.000000 tsfeatures-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:47:36.975164 tsfeatures-0.4.2/tsfeatures/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-18 03:47:27.000000 tsfeatures-0.4.2/tsfeatures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-18 03:47:27.000000 tsfeatures-0.4.2/tsfeatures/compare_with_r.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-06-18 03:47:27.000000 tsfeatures-0.4.2/tsfeatures/m4_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:47:36.975164 tsfeatures-0.4.2/tsfeatures/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-18 03:47:27.000000 tsfeatures-0.4.2/tsfeatures/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-06-18 03:47:27.000000 tsfeatures-0.4.2/tsfeatures/metrics/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:47:36.979164 tsfeatures-0.4.2/tsfeatures/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 03:47:27.000000 tsfeatures-0.4.2/tsfeatures/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-18 03:47:27.000000 tsfeatures-0.4.2/tsfeatures/tests/test_acf_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-18 03:47:27.000000 tsfeatures-0.4.2/tsfeatures/tests/test_arch_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-18 03:47:27.000000 tsfeatures-0.4.2/tsfeatures/tests/test_holt_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-18 03:47:27.000000 tsfeatures-0.4.2/tsfeatures/tests/test_mutability.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-18 03:47:27.000000 tsfeatures-0.4.2/tsfeatures/tests/test_pacf_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-18 03:47:27.000000 tsfeatures-0.4.2/tsfeatures/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-18 03:47:27.000000 tsfeatures-0.4.2/tsfeatures/tests/test_sparsity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28108 2023-06-18 03:47:27.000000 tsfeatures-0.4.2/tsfeatures/tsfeatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-06-18 03:47:27.000000 tsfeatures-0.4.2/tsfeatures/tsfeatures_r.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-06-18 03:47:27.000000 tsfeatures-0.4.2/tsfeatures/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:47:36.975164 tsfeatures-0.4.2/tsfeatures.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-06-18 03:47:36.000000 tsfeatures-0.4.2/tsfeatures.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-18 03:47:36.000000 tsfeatures-0.4.2/tsfeatures.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 03:47:36.000000 tsfeatures-0.4.2/tsfeatures.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-18 03:47:36.000000 tsfeatures-0.4.2/tsfeatures.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-18 03:47:36.000000 tsfeatures-0.4.2/tsfeatures.egg-info/top_level.txt
```

### Comparing `tsfeatures-0.4.1/PKG-INFO` & `tsfeatures-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsfeatures
-Version: 0.4.1
+Version: 0.4.2
 Summary: Calculates various features from time series data.
 Home-page: https://github.com/Nixtla/tsfeatures
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `tsfeatures-0.4.1/README.md` & `tsfeatures-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.1/setup.py` & `tsfeatures-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tsfeatures",
-    version="0.4.1",
+    version="0.4.2",
     description="Calculates various features from time series data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Nixtla/tsfeatures",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `tsfeatures-0.4.1/tsfeatures/compare_with_r.py` & `tsfeatures-0.4.2/tsfeatures/compare_with_r.py`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.1/tsfeatures/m4_data.py` & `tsfeatures-0.4.2/tsfeatures/m4_data.py`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.1/tsfeatures/metrics/metrics.py` & `tsfeatures-0.4.2/tsfeatures/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.1/tsfeatures/tests/test_acf_features.py` & `tsfeatures-0.4.2/tsfeatures/tests/test_acf_features.py`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.1/tsfeatures/tests/test_holt_parameters.py` & `tsfeatures-0.4.2/tsfeatures/tests/test_holt_parameters.py`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.1/tsfeatures/tests/test_pipeline.py` & `tsfeatures-0.4.2/tsfeatures/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.1/tsfeatures/tests/test_sparsity.py` & `tsfeatures-0.4.2/tsfeatures/tests/test_sparsity.py`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.1/tsfeatures/tsfeatures.py` & `tsfeatures-0.4.2/tsfeatures/tsfeatures.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     -------
     dict
         'arch_lm': R^2 value of an autoregressive model of order lags applied to x**2.
     """
     if len(x) <= lags + 1:
         return {'arch_lm': np.nan}
     if demean:
-        x -= np.mean(x)
+        x = x - np.mean(x)
 
     size_x = len(x)
     mat = embed(x ** 2, lags + 1)
     X = mat[:, 1:]
     y = np.vstack(mat[:, 0])
 
     try:
```

### Comparing `tsfeatures-0.4.1/tsfeatures/tsfeatures_r.py` & `tsfeatures-0.4.2/tsfeatures/tsfeatures_r.py`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.1/tsfeatures/utils.py` & `tsfeatures-0.4.2/tsfeatures/utils.py`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.1/tsfeatures.egg-info/PKG-INFO` & `tsfeatures-0.4.2/tsfeatures.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsfeatures
-Version: 0.4.1
+Version: 0.4.2
 Summary: Calculates various features from time series data.
 Home-page: https://github.com/Nixtla/tsfeatures
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `tsfeatures-0.4.1/tsfeatures.egg-info/SOURCES.txt` & `tsfeatures-0.4.2/tsfeatures.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,10 +14,11 @@
 tsfeatures.egg-info/top_level.txt
 tsfeatures/metrics/__init__.py
 tsfeatures/metrics/metrics.py
 tsfeatures/tests/__init__.py
 tsfeatures/tests/test_acf_features.py
 tsfeatures/tests/test_arch_stat.py
 tsfeatures/tests/test_holt_parameters.py
+tsfeatures/tests/test_mutability.py
 tsfeatures/tests/test_pacf_features.py
 tsfeatures/tests/test_pipeline.py
 tsfeatures/tests/test_sparsity.py
```

