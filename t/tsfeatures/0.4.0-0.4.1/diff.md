# Comparing `tmp/tsfeatures-0.4.0.tar.gz` & `tmp/tsfeatures-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsfeatures-0.4.0.tar", last modified: Thu Dec  8 03:42:36 2022, max compression
+gzip compressed data, was "tsfeatures-0.4.1.tar", last modified: Sun Jun 18 02:44:53 2023, max compression
```

## Comparing `tsfeatures-0.4.0.tar` & `tsfeatures-0.4.1.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-08 03:42:36.008808 tsfeatures-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1089 2022-12-08 03:42:28.000000 tsfeatures-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     7150 2022-12-08 03:42:36.008808 tsfeatures-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6756 2022-12-08 03:42:28.000000 tsfeatures-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-08 03:42:36.008808 tsfeatures-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      792 2022-12-08 03:42:28.000000 tsfeatures-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-08 03:42:36.008808 tsfeatures-0.4.0/tsfeatures/
--rw-r--r--   0 runner    (1001) docker     (122)       65 2022-12-08 03:42:28.000000 tsfeatures-0.4.0/tsfeatures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2323 2022-12-08 03:42:28.000000 tsfeatures-0.4.0/tsfeatures/compare_with_r.py
--rw-r--r--   0 runner    (1001) docker     (122)     6518 2022-12-08 03:42:28.000000 tsfeatures-0.4.0/tsfeatures/m4_data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-08 03:42:36.008808 tsfeatures-0.4.0/tsfeatures/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)       62 2022-12-08 03:42:28.000000 tsfeatures-0.4.0/tsfeatures/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10356 2022-12-08 03:42:28.000000 tsfeatures-0.4.0/tsfeatures/metrics/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-08 03:42:36.008808 tsfeatures-0.4.0/tsfeatures/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-08 03:42:28.000000 tsfeatures-0.4.0/tsfeatures/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1076 2022-12-08 03:42:28.000000 tsfeatures-0.4.0/tsfeatures/tests/test_acf_features.py
--rw-r--r--   0 runner    (1001) docker     (122)      449 2022-12-08 03:42:28.000000 tsfeatures-0.4.0/tsfeatures/tests/test_arch_stat.py
--rw-r--r--   0 runner    (1001) docker     (122)      573 2022-12-08 03:42:28.000000 tsfeatures-0.4.0/tsfeatures/tests/test_holt_parameters.py
--rw-r--r--   0 runner    (1001) docker     (122)      755 2022-12-08 03:42:28.000000 tsfeatures-0.4.0/tsfeatures/tests/test_pacf_features.py
--rw-r--r--   0 runner    (1001) docker     (122)      668 2022-12-08 03:42:28.000000 tsfeatures-0.4.0/tsfeatures/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (122)    28031 2022-12-08 03:42:28.000000 tsfeatures-0.4.0/tsfeatures/tsfeatures.py
--rw-r--r--   0 runner    (1001) docker     (122)     5790 2022-12-08 03:42:28.000000 tsfeatures-0.4.0/tsfeatures/tsfeatures_r.py
--rw-r--r--   0 runner    (1001) docker     (122)     7680 2022-12-08 03:42:28.000000 tsfeatures-0.4.0/tsfeatures/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-08 03:42:36.008808 tsfeatures-0.4.0/tsfeatures.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7150 2022-12-08 03:42:35.000000 tsfeatures-0.4.0/tsfeatures.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      618 2022-12-08 03:42:35.000000 tsfeatures-0.4.0/tsfeatures.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-08 03:42:35.000000 tsfeatures-0.4.0/tsfeatures.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      100 2022-12-08 03:42:35.000000 tsfeatures-0.4.0/tsfeatures.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2022-12-08 03:42:35.000000 tsfeatures-0.4.0/tsfeatures.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:44:53.100658 tsfeatures-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-06-18 02:44:53.100658 tsfeatures-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 02:44:53.100658 tsfeatures-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:44:53.096658 tsfeatures-0.4.1/tsfeatures/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/compare_with_r.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/m4_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:44:53.100658 tsfeatures-0.4.1/tsfeatures/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/metrics/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:44:53.100658 tsfeatures-0.4.1/tsfeatures/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/tests/test_acf_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/tests/test_arch_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/tests/test_holt_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/tests/test_pacf_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/tests/test_sparsity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28105 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/tsfeatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/tsfeatures_r.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-06-18 02:44:37.000000 tsfeatures-0.4.1/tsfeatures/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:44:53.100658 tsfeatures-0.4.1/tsfeatures.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-06-18 02:44:53.000000 tsfeatures-0.4.1/tsfeatures.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-18 02:44:53.000000 tsfeatures-0.4.1/tsfeatures.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:44:53.000000 tsfeatures-0.4.1/tsfeatures.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-18 02:44:53.000000 tsfeatures-0.4.1/tsfeatures.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-18 02:44:53.000000 tsfeatures-0.4.1/tsfeatures.egg-info/top_level.txt
```

### Comparing `tsfeatures-0.4.0/LICENSE` & `tsfeatures-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.0/PKG-INFO` & `tsfeatures-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsfeatures
-Version: 0.4.0
+Version: 0.4.1
 Summary: Calculates various features from time series data.
 Home-page: https://github.com/Nixtla/tsfeatures
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `tsfeatures-0.4.0/README.md` & `tsfeatures-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.0/setup.py` & `tsfeatures-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tsfeatures",
-    version="0.4.0",
+    version="0.4.1",
     description="Calculates various features from time series data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Nixtla/tsfeatures",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `tsfeatures-0.4.0/tsfeatures/compare_with_r.py` & `tsfeatures-0.4.1/tsfeatures/compare_with_r.py`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.0/tsfeatures/m4_data.py` & `tsfeatures-0.4.1/tsfeatures/m4_data.py`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.0/tsfeatures/metrics/metrics.py` & `tsfeatures-0.4.1/tsfeatures/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.0/tsfeatures/tests/test_acf_features.py` & `tsfeatures-0.4.1/tsfeatures/tests/test_acf_features.py`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.0/tsfeatures/tests/test_holt_parameters.py` & `tsfeatures-0.4.1/tsfeatures/tests/test_holt_parameters.py`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.0/tsfeatures/tests/test_pipeline.py` & `tsfeatures-0.4.1/tsfeatures/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.0/tsfeatures/tsfeatures.py` & `tsfeatures-0.4.1/tsfeatures/tsfeatures.py`

 * *Files 1% similar despite different names*

```diff
@@ -561,15 +561,18 @@
     output = {
         'x_pacf5': pacf_5,
         'diff1x_pacf5': diff1_pacf_5,
         'diff2x_pacf5': diff2_pacf_5
     }
 
     if m > 1:
-        output['seas_pacf'] = pacfx[m] if len(pacfx) > m else np.nan
+        try:
+            output['seas_pacf'] = pacfx[m] if len(pacfx) > m else np.nan
+        except:
+            output['seas_pacf'] = np.nan
 
     return output
 
 def series_length(x: np.array, freq: int = 1) -> Dict[str, float]:
     """Series length.
 
     Parameters
```

### Comparing `tsfeatures-0.4.0/tsfeatures/tsfeatures_r.py` & `tsfeatures-0.4.1/tsfeatures/tsfeatures_r.py`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.0/tsfeatures/utils.py` & `tsfeatures-0.4.1/tsfeatures/utils.py`

 * *Files identical despite different names*

### Comparing `tsfeatures-0.4.0/tsfeatures.egg-info/PKG-INFO` & `tsfeatures-0.4.1/tsfeatures.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsfeatures
-Version: 0.4.0
+Version: 0.4.1
 Summary: Calculates various features from time series data.
 Home-page: https://github.com/Nixtla/tsfeatures
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `tsfeatures-0.4.0/tsfeatures.egg-info/SOURCES.txt` & `tsfeatures-0.4.1/tsfeatures.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -15,8 +15,9 @@
 tsfeatures/metrics/__init__.py
 tsfeatures/metrics/metrics.py
 tsfeatures/tests/__init__.py
 tsfeatures/tests/test_acf_features.py
 tsfeatures/tests/test_arch_stat.py
 tsfeatures/tests/test_holt_parameters.py
 tsfeatures/tests/test_pacf_features.py
-tsfeatures/tests/test_pipeline.py
+tsfeatures/tests/test_pipeline.py
+tsfeatures/tests/test_sparsity.py
```

