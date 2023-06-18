# Comparing `tmp/gecs-0.14.0.tar.gz` & `tmp/gecs-0.14.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gecs-0.14.0.tar", max compression
+gzip compressed data, was "gecs-0.14.1.tar", max compression
```

## Comparing `gecs-0.14.0.tar` & `gecs-0.14.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1060 2023-04-06 09:38:20.465352 gecs-0.14.0/LICENSE
--rw-r--r--   0        0        0        0 2023-04-06 08:53:47.610205 gecs-0.14.0/README.md
--rw-r--r--   0        0        0      697 2023-06-18 17:02:21.635905 gecs-0.14.0/pyproject.toml
--rw-r--r--   0        0        0    43059 2023-06-18 17:09:05.807811 gecs-0.14.0/src/gecs/gec.py
--rw-r--r--   0        0        0     2112 2023-06-18 16:26:28.103885 gecs-0.14.0/src/gecs/utils/gaussian_process_visualisation.py
--rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 gecs-0.14.0/setup.py
--rw-r--r--   0        0        0      964 1970-01-01 00:00:00.000000 gecs-0.14.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-06 09:38:20.465352 gecs-0.14.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-06 08:53:47.610205 gecs-0.14.1/README.md
+-rw-r--r--   0        0        0      697 2023-06-18 17:27:33.582283 gecs-0.14.1/pyproject.toml
+-rw-r--r--   0        0        0    43030 2023-06-18 17:26:22.404258 gecs-0.14.1/src/gecs/gec.py
+-rw-r--r--   0        0        0     2112 2023-06-18 16:26:28.103885 gecs-0.14.1/src/gecs/utils/gaussian_process_visualisation.py
+-rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 gecs-0.14.1/setup.py
+-rw-r--r--   0        0        0      964 1970-01-01 00:00:00.000000 gecs-0.14.1/PKG-INFO
```

### Comparing `gecs-0.14.0/LICENSE` & `gecs-0.14.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gecs-0.14.0/pyproject.toml` & `gecs-0.14.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gecs"
-version = "0.14.0"
+version = "0.14.1"
 authors = ["Leon Luithlen <leontimnaluithlen@gmail.com>"]
 description = "LightGBM Classifier with integrated bayesian hyperparameter optimization"
 keywords = ["lightgbm", "classification", "machine learning", "hyperparameter optimization", "classifier"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/0xideas/sequifier"
 repository = "https://github.com/0xideas/sequifier"
```

### Comparing `gecs-0.14.0/src/gecs/gec.py` & `gecs-0.14.1/src/gecs/gec.py`

 * *Files 0% similar despite different names*

```diff
@@ -711,15 +711,14 @@
                         arguments["bagging_fraction"],
                     ) = best_predicted_combination_bagging
 
             del arguments["bagging"]
             arguments["verbosity"] = -1
 
             arguments = self._set_n_estimators_and_num_leaves(arguments, i, n_iter)
-            print(arguments)
 
             try:
                 score = self._calculate_cv_score(X, Y, arguments)
                 if np.isnan(score):
                     score = 0
 
                 if best_score is None or score > best_score:
```

### Comparing `gecs-0.14.0/src/gecs/utils/gaussian_process_visualisation.py` & `gecs-0.14.1/src/gecs/utils/gaussian_process_visualisation.py`

 * *Files identical despite different names*

### Comparing `gecs-0.14.0/setup.py` & `gecs-0.14.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'scikit-learn==1.2.2',
  'scipy==1.10.1',
  'tqdm==4.65.0',
  'typer==0.9.0']
 
 setup_kwargs = {
     'name': 'gecs',
-    'version': '0.14.0',
+    'version': '0.14.1',
     'description': 'LightGBM Classifier with integrated bayesian hyperparameter optimization',
     'long_description': '',
     'author': 'Leon Luithlen',
     'author_email': 'leontimnaluithlen@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/0xideas/sequifier',
```

### Comparing `gecs-0.14.0/PKG-INFO` & `gecs-0.14.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gecs
-Version: 0.14.0
+Version: 0.14.1
 Summary: LightGBM Classifier with integrated bayesian hyperparameter optimization
 Home-page: https://github.com/0xideas/sequifier
 License: MIT
 Keywords: lightgbm,classification,machine learning,hyperparameter optimization,classifier
 Author: Leon Luithlen
 Author-email: leontimnaluithlen@gmail.com
 Requires-Python: >=3.10.0,<3.11.0
```

