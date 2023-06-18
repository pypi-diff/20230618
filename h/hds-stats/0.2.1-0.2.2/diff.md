# Comparing `tmp/hds-stats-0.2.1.tar.gz` & `tmp/hds-stats-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hds-stats-0.2.1.tar", last modified: Sun Jun 18 15:52:49 2023, max compression
+gzip compressed data, was "hds-stats-0.2.2.tar", last modified: Sun Jun 18 16:31:19 2023, max compression
```

## Comparing `hds-stats-0.2.1.tar` & `hds-stats-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-06-18 15:52:49.941866 hds-stats-0.2.1/
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.2.1/LICENSE
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-06-18 15:52:49.941619 hds-stats-0.2.1/PKG-INFO
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.2.1/README.md
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-06-18 15:52:49.939485 hds-stats-0.2.1/hds_stats/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       82 2023-04-09 20:34:59.000000 hds-stats-0.2.1/hds_stats/__init__.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    11955 2023-04-25 11:45:11.000000 hds-stats-0.2.1/hds_stats/plot.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    27158 2023-06-18 15:48:20.000000 hds-stats-0.2.1/hds_stats/stat.py
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-06-18 15:52:49.941243 hds-stats-0.2.1/hds_stats.egg-info/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-06-18 15:52:49.000000 hds-stats-0.2.1/hds_stats.egg-info/PKG-INFO
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      263 2023-06-18 15:52:49.000000 hds-stats-0.2.1/hds_stats.egg-info/SOURCES.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-06-18 15:52:49.000000 hds-stats-0.2.1/hds_stats.egg-info/dependency_links.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       63 2023-06-18 15:52:49.000000 hds-stats-0.2.1/hds_stats.egg-info/requires.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       20 2023-06-18 15:52:49.000000 hds-stats-0.2.1/hds_stats.egg-info/top_level.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.2.1/pyproject.toml
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-06-18 15:52:49.941953 hds-stats-0.2.1/setup.cfg
--rw-r--r--   0 hdsceokevin   (501) staff       (20)     1178 2023-04-25 11:50:37.000000 hds-stats-0.2.1/setup.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-06-18 16:31:19.657003 hds-stats-0.2.2/
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.2.2/LICENSE
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-06-18 16:31:19.656685 hds-stats-0.2.2/PKG-INFO
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.2.2/README.md
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-06-18 16:31:19.654334 hds-stats-0.2.2/hds_stats/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       82 2023-04-09 20:34:59.000000 hds-stats-0.2.2/hds_stats/__init__.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)    11955 2023-06-18 16:25:20.000000 hds-stats-0.2.2/hds_stats/plot.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)    27171 2023-06-18 16:25:56.000000 hds-stats-0.2.2/hds_stats/stat.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-06-18 16:31:19.656236 hds-stats-0.2.2/hds_stats.egg-info/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-06-18 16:31:19.000000 hds-stats-0.2.2/hds_stats.egg-info/PKG-INFO
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      263 2023-06-18 16:31:19.000000 hds-stats-0.2.2/hds_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-06-18 16:31:19.000000 hds-stats-0.2.2/hds_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       63 2023-06-18 16:31:19.000000 hds-stats-0.2.2/hds_stats.egg-info/requires.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       20 2023-06-18 16:31:19.000000 hds-stats-0.2.2/hds_stats.egg-info/top_level.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.2.2/pyproject.toml
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-06-18 16:31:19.657096 hds-stats-0.2.2/setup.cfg
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)     1178 2023-06-18 16:28:22.000000 hds-stats-0.2.2/setup.py
```

### Comparing `hds-stats-0.2.1/LICENSE` & `hds-stats-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hds-stats-0.2.1/PKG-INFO` & `hds-stats-0.2.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.2.1
+Version: 0.2.2
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds-stats-0.2.1/hds_stats/plot.py` & `hds-stats-0.2.2/hds_stats/plot.py`

 * *Files identical despite different names*

### Comparing `hds-stats-0.2.1/hds_stats/stat.py` & `hds-stats-0.2.2/hds_stats/stat.py`

 * *Files 0% similar despite different names*

```diff
@@ -501,24 +501,24 @@
         data = test, 
         index = ['Statistic', 'P-Value', 'F-Value', 'F P-Value']
     ).T
     
     return result
 
 
-# 분산 팽창 지수
+# 분산팽창지수
 def vif(model):
     '''
-    이 함수는 입력변수 행렬의 분산 팽창 지수를 계산합니다.
+    이 함수는 입력변수 행렬의 분산팽창지수를 계산합니다.
     
     매개변수:
          model: statsmodels.formula.api.ols 함수로 적합한 선형 회귀모형을 지정합니다.
     
     반환:
-        입력변수 행렬의 열별 분산 팽창 지수를 반환합니다.
+        입력변수 행렬의 열별 분산팽창지수를 반환합니다.
     '''
     import numpy as np
     import pandas as pd
     import statsmodels.stats.outliers_influence as oi
     
     func = oi.variance_inflation_factor
     ncol = len(model.model.exog_names)
@@ -785,24 +785,25 @@
     매개변수:
         y_true: 목표변수의 실제값을 pd.Series 또는 1차원 np.ndarray로 지정합니다.
         y_pred: 목표변수의 추정값을 pd.Series 또는 1차원 np.ndarray로 지정합니다.
     
     반환:
         분류모형의 다양한 성능 지표를 출력합니다.
     '''
-    from sklearn.metrics import confusion_matrix
     from sklearn.metrics import classification_report
     
     print('▶ Confusion Matrix')
-    print(
-        confusion_matrix(
-            y_true = y_true, 
-            y_pred = y_pred
-        )
+    cfm = pd.crosstab(
+        index = y_pred, 
+        columns = y_true, 
+        margins = True
     )
+    cfm.index.name = 'Pred'
+    cfm.columns.name = 'Real'
+    display(cfm)
     
     print()
     
     print('▶ Classification Report')
     print(
         classification_report(
             y_true = y_true,
```

### Comparing `hds-stats-0.2.1/hds_stats.egg-info/PKG-INFO` & `hds-stats-0.2.2/hds_stats.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.2.1
+Version: 0.2.2
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds-stats-0.2.1/setup.py` & `hds-stats-0.2.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 
 with open(file = 'README.md', mode = 'r', encoding = 'UTF-8') as file:
     long_description = file.read()
 
 setup(
     name = 'hds-stats',
-    version = '0.2.1',
+    version = '0.2.2',
     author = 'HelloDataScience',
     author_email = 'hellodatasciencekorea@gmail.com',
     
     description = 'Useful functions for Statistics and Machine Learning',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
```

