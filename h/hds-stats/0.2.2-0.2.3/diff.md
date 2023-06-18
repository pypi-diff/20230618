# Comparing `tmp/hds-stats-0.2.2.tar.gz` & `tmp/hds-stats-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hds-stats-0.2.2.tar", last modified: Sun Jun 18 16:31:19 2023, max compression
+gzip compressed data, was "hds-stats-0.2.3.tar", last modified: Sun Jun 18 16:49:46 2023, max compression
```

## Comparing `hds-stats-0.2.2.tar` & `hds-stats-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-06-18 16:31:19.657003 hds-stats-0.2.2/
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.2.2/LICENSE
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-06-18 16:31:19.656685 hds-stats-0.2.2/PKG-INFO
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.2.2/README.md
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-06-18 16:31:19.654334 hds-stats-0.2.2/hds_stats/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       82 2023-04-09 20:34:59.000000 hds-stats-0.2.2/hds_stats/__init__.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    11955 2023-06-18 16:25:20.000000 hds-stats-0.2.2/hds_stats/plot.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    27171 2023-06-18 16:25:56.000000 hds-stats-0.2.2/hds_stats/stat.py
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-06-18 16:31:19.656236 hds-stats-0.2.2/hds_stats.egg-info/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-06-18 16:31:19.000000 hds-stats-0.2.2/hds_stats.egg-info/PKG-INFO
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      263 2023-06-18 16:31:19.000000 hds-stats-0.2.2/hds_stats.egg-info/SOURCES.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-06-18 16:31:19.000000 hds-stats-0.2.2/hds_stats.egg-info/dependency_links.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       63 2023-06-18 16:31:19.000000 hds-stats-0.2.2/hds_stats.egg-info/requires.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       20 2023-06-18 16:31:19.000000 hds-stats-0.2.2/hds_stats.egg-info/top_level.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.2.2/pyproject.toml
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-06-18 16:31:19.657096 hds-stats-0.2.2/setup.cfg
--rw-r--r--   0 hdsceokevin   (501) staff       (20)     1178 2023-06-18 16:28:22.000000 hds-stats-0.2.2/setup.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-06-18 16:49:46.260728 hds-stats-0.2.3/
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.2.3/LICENSE
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-06-18 16:49:46.260484 hds-stats-0.2.3/PKG-INFO
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.2.3/README.md
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-06-18 16:49:46.258219 hds-stats-0.2.3/hds_stats/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       82 2023-04-09 20:34:59.000000 hds-stats-0.2.3/hds_stats/__init__.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)    11955 2023-06-18 16:25:20.000000 hds-stats-0.2.3/hds_stats/plot.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)    27195 2023-06-18 16:48:47.000000 hds-stats-0.2.3/hds_stats/stat.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-06-18 16:49:46.260111 hds-stats-0.2.3/hds_stats.egg-info/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-06-18 16:49:46.000000 hds-stats-0.2.3/hds_stats.egg-info/PKG-INFO
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      263 2023-06-18 16:49:46.000000 hds-stats-0.2.3/hds_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-06-18 16:49:46.000000 hds-stats-0.2.3/hds_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       63 2023-06-18 16:49:46.000000 hds-stats-0.2.3/hds_stats.egg-info/requires.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       20 2023-06-18 16:49:46.000000 hds-stats-0.2.3/hds_stats.egg-info/top_level.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.2.3/pyproject.toml
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-06-18 16:49:46.260815 hds-stats-0.2.3/setup.cfg
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)     1178 2023-06-18 16:48:09.000000 hds-stats-0.2.3/setup.py
```

### Comparing `hds-stats-0.2.2/LICENSE` & `hds-stats-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hds-stats-0.2.2/PKG-INFO` & `hds-stats-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.2.2
+Version: 0.2.3
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds-stats-0.2.2/hds_stats/plot.py` & `hds-stats-0.2.3/hds_stats/plot.py`

 * *Files identical despite different names*

### Comparing `hds-stats-0.2.2/hds_stats/stat.py` & `hds-stats-0.2.3/hds_stats/stat.py`

 * *Files 0% similar despite different names*

```diff
@@ -785,14 +785,15 @@
     매개변수:
         y_true: 목표변수의 실제값을 pd.Series 또는 1차원 np.ndarray로 지정합니다.
         y_pred: 목표변수의 추정값을 pd.Series 또는 1차원 np.ndarray로 지정합니다.
     
     반환:
         분류모형의 다양한 성능 지표를 출력합니다.
     '''
+    import pandas as pd
     from sklearn.metrics import classification_report
     
     print('▶ Confusion Matrix')
     cfm = pd.crosstab(
         index = y_pred, 
         columns = y_true, 
         margins = True
```

### Comparing `hds-stats-0.2.2/hds_stats.egg-info/PKG-INFO` & `hds-stats-0.2.3/hds_stats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.2.2
+Version: 0.2.3
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds-stats-0.2.2/setup.py` & `hds-stats-0.2.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 
 with open(file = 'README.md', mode = 'r', encoding = 'UTF-8') as file:
     long_description = file.read()
 
 setup(
     name = 'hds-stats',
-    version = '0.2.2',
+    version = '0.2.3',
     author = 'HelloDataScience',
     author_email = 'hellodatasciencekorea@gmail.com',
     
     description = 'Useful functions for Statistics and Machine Learning',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
```

