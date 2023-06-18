# Comparing `tmp/bio-pypage-0.1.4.tar.gz` & `tmp/bio-pypage-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bio-pypage-0.1.4.tar", last modified: Sat Jun 17 06:42:59 2023, max compression
+gzip compressed data, was "bio-pypage-0.1.5.tar", last modified: Sun Jun 18 19:24:01 2023, max compression
```

## Comparing `bio-pypage-0.1.4.tar` & `bio-pypage-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 workspace   (502) staff       (20)        0 2023-06-17 06:42:59.236970 bio-pypage-0.1.4/
--rw-r--r--   0 workspace   (502) staff       (20)     1070 2022-06-09 10:36:48.000000 bio-pypage-0.1.4/LICENSE
--rw-r--r--   0 workspace   (502) staff       (20)     5122 2023-06-17 06:42:59.236567 bio-pypage-0.1.4/PKG-INFO
--rw-r--r--   0 workspace   (502) staff       (20)     4640 2023-06-17 06:35:29.000000 bio-pypage-0.1.4/README.md
-drwxr-xr-x   0 workspace   (502) staff       (20)        0 2023-06-17 06:42:59.227183 bio-pypage-0.1.4/bio_pypage.egg-info/
--rw-r--r--   0 workspace   (502) staff       (20)     5122 2023-06-17 06:42:58.000000 bio-pypage-0.1.4/bio_pypage.egg-info/PKG-INFO
--rw-r--r--   0 workspace   (502) staff       (20)      397 2023-06-17 06:42:59.000000 bio-pypage-0.1.4/bio_pypage.egg-info/SOURCES.txt
--rw-r--r--   0 workspace   (502) staff       (20)        1 2023-06-17 06:42:58.000000 bio-pypage-0.1.4/bio_pypage.egg-info/dependency_links.txt
--rw-r--r--   0 workspace   (502) staff       (20)       58 2023-06-17 06:42:58.000000 bio-pypage-0.1.4/bio_pypage.egg-info/requires.txt
--rw-r--r--   0 workspace   (502) staff       (20)        7 2023-06-17 06:42:59.000000 bio-pypage-0.1.4/bio_pypage.egg-info/top_level.txt
-drwxr-xr-x   0 workspace   (502) staff       (20)        0 2023-06-17 06:42:59.232192 bio-pypage-0.1.4/pypage/
--rw-r--r--   0 workspace   (502) staff       (20)      132 2023-06-15 22:20:27.000000 bio-pypage-0.1.4/pypage/__init__.py
--rw-r--r--   0 workspace   (502) staff       (20)     9455 2023-06-15 14:51:03.000000 bio-pypage-0.1.4/pypage/heatmap.py
--rw-r--r--   0 workspace   (502) staff       (20)     3657 2022-06-09 10:36:48.000000 bio-pypage-0.1.4/pypage/hist.py
--rw-r--r--   0 workspace   (502) staff       (20)    12550 2022-06-29 13:50:11.000000 bio-pypage-0.1.4/pypage/information.py
-drwxr-xr-x   0 workspace   (502) staff       (20)        0 2023-06-17 06:42:59.235338 bio-pypage-0.1.4/pypage/io/
--rw-r--r--   0 workspace   (502) staff       (20)       73 2023-06-15 14:40:59.000000 bio-pypage-0.1.4/pypage/io/__init__.py
--rw-r--r--   0 workspace   (502) staff       (20)     2472 2022-06-04 21:11:51.000000 bio-pypage-0.1.4/pypage/io/accession_types.py
--rw-r--r--   0 workspace   (502) staff       (20)     6388 2023-06-15 19:19:22.000000 bio-pypage-0.1.4/pypage/io/expression.py
--rw-r--r--   0 workspace   (502) staff       (20)    11432 2023-06-16 23:07:24.000000 bio-pypage-0.1.4/pypage/io/ontology.py
--rw-r--r--   0 workspace   (502) staff       (20)    15280 2023-06-16 09:02:29.000000 bio-pypage-0.1.4/pypage/page.py
--rw-r--r--   0 workspace   (502) staff       (20)     3909 2022-06-09 13:50:18.000000 bio-pypage-0.1.4/pypage/utils.py
--rw-r--r--   0 workspace   (502) staff       (20)       38 2023-06-17 06:42:59.237148 bio-pypage-0.1.4/setup.cfg
--rw-r--r--   0 workspace   (502) staff       (20)      800 2023-06-17 06:34:43.000000 bio-pypage-0.1.4/setup.py
+drwxr-xr-x   0 workspace   (502) staff       (20)        0 2023-06-18 19:24:01.390540 bio-pypage-0.1.5/
+-rw-r--r--   0 workspace   (502) staff       (20)     1070 2022-06-09 10:36:48.000000 bio-pypage-0.1.5/LICENSE
+-rw-r--r--   0 workspace   (502) staff       (20)     5132 2023-06-18 19:24:01.390135 bio-pypage-0.1.5/PKG-INFO
+-rw-r--r--   0 workspace   (502) staff       (20)     4650 2023-06-18 19:23:08.000000 bio-pypage-0.1.5/README.md
+drwxr-xr-x   0 workspace   (502) staff       (20)        0 2023-06-18 19:24:01.382065 bio-pypage-0.1.5/bio_pypage.egg-info/
+-rw-r--r--   0 workspace   (502) staff       (20)     5132 2023-06-18 19:24:00.000000 bio-pypage-0.1.5/bio_pypage.egg-info/PKG-INFO
+-rw-r--r--   0 workspace   (502) staff       (20)      397 2023-06-18 19:24:01.000000 bio-pypage-0.1.5/bio_pypage.egg-info/SOURCES.txt
+-rw-r--r--   0 workspace   (502) staff       (20)        1 2023-06-18 19:24:00.000000 bio-pypage-0.1.5/bio_pypage.egg-info/dependency_links.txt
+-rw-r--r--   0 workspace   (502) staff       (20)       58 2023-06-18 19:24:01.000000 bio-pypage-0.1.5/bio_pypage.egg-info/requires.txt
+-rw-r--r--   0 workspace   (502) staff       (20)        7 2023-06-18 19:24:01.000000 bio-pypage-0.1.5/bio_pypage.egg-info/top_level.txt
+drwxr-xr-x   0 workspace   (502) staff       (20)        0 2023-06-18 19:24:01.386624 bio-pypage-0.1.5/pypage/
+-rw-r--r--   0 workspace   (502) staff       (20)      132 2023-06-15 22:20:27.000000 bio-pypage-0.1.5/pypage/__init__.py
+-rw-r--r--   0 workspace   (502) staff       (20)     9455 2023-06-15 14:51:03.000000 bio-pypage-0.1.5/pypage/heatmap.py
+-rw-r--r--   0 workspace   (502) staff       (20)     3657 2022-06-09 10:36:48.000000 bio-pypage-0.1.5/pypage/hist.py
+-rw-r--r--   0 workspace   (502) staff       (20)    12550 2022-06-29 13:50:11.000000 bio-pypage-0.1.5/pypage/information.py
+drwxr-xr-x   0 workspace   (502) staff       (20)        0 2023-06-18 19:24:01.389200 bio-pypage-0.1.5/pypage/io/
+-rw-r--r--   0 workspace   (502) staff       (20)       73 2023-06-15 14:40:59.000000 bio-pypage-0.1.5/pypage/io/__init__.py
+-rw-r--r--   0 workspace   (502) staff       (20)     2472 2022-06-04 21:11:51.000000 bio-pypage-0.1.5/pypage/io/accession_types.py
+-rw-r--r--   0 workspace   (502) staff       (20)     6388 2023-06-15 19:19:22.000000 bio-pypage-0.1.5/pypage/io/expression.py
+-rw-r--r--   0 workspace   (502) staff       (20)    11432 2023-06-16 23:07:24.000000 bio-pypage-0.1.5/pypage/io/ontology.py
+-rw-r--r--   0 workspace   (502) staff       (20)    15280 2023-06-16 09:02:29.000000 bio-pypage-0.1.5/pypage/page.py
+-rw-r--r--   0 workspace   (502) staff       (20)     3909 2022-06-09 13:50:18.000000 bio-pypage-0.1.5/pypage/utils.py
+-rw-r--r--   0 workspace   (502) staff       (20)       38 2023-06-18 19:24:01.390663 bio-pypage-0.1.5/setup.cfg
+-rw-r--r--   0 workspace   (502) staff       (20)      800 2023-06-18 19:23:23.000000 bio-pypage-0.1.5/setup.py
```

### Comparing `bio-pypage-0.1.4/LICENSE` & `bio-pypage-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bio-pypage-0.1.4/PKG-INFO` & `bio-pypage-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bio-pypage
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python implementation of the PAGE algorithm
 Home-page: https://github.com/goodarzilab/pypage
 Author: Artemy Bakulin, Noam Teyssier
 Author-email: logic2000.bakulin@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -141,15 +141,15 @@
     hm.show(show_reg=True)
     
     return results
 ```
 
 ## Manual
 
-For an exhaustive description of pyPAGE functions refer to the [manual](https://github.com/goodarzilab/pyPAGE/MANUAL.md).
+For an exhaustive description of pyPAGE functions refer to the [manual](https://github.com/goodarzilab/pypage/blob/main/MANUAL.md).
 
 ## License
 MIT license
 
 ## Citing
 See the paper
```

### Comparing `bio-pypage-0.1.4/README.md` & `bio-pypage-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     hm.show(show_reg=True)
     
     return results
 ```
 
 ## Manual
 
-For an exhaustive description of pyPAGE functions refer to the [manual](https://github.com/goodarzilab/pyPAGE/MANUAL.md).
+For an exhaustive description of pyPAGE functions refer to the [manual](https://github.com/goodarzilab/pypage/blob/main/MANUAL.md).
 
 ## License
 MIT license
 
 ## Citing
 See the paper
```

### Comparing `bio-pypage-0.1.4/bio_pypage.egg-info/PKG-INFO` & `bio-pypage-0.1.5/bio_pypage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bio-pypage
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python implementation of the PAGE algorithm
 Home-page: https://github.com/goodarzilab/pypage
 Author: Artemy Bakulin, Noam Teyssier
 Author-email: logic2000.bakulin@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -141,15 +141,15 @@
     hm.show(show_reg=True)
     
     return results
 ```
 
 ## Manual
 
-For an exhaustive description of pyPAGE functions refer to the [manual](https://github.com/goodarzilab/pyPAGE/MANUAL.md).
+For an exhaustive description of pyPAGE functions refer to the [manual](https://github.com/goodarzilab/pypage/blob/main/MANUAL.md).
 
 ## License
 MIT license
 
 ## Citing
 See the paper
```

### Comparing `bio-pypage-0.1.4/pypage/heatmap.py` & `bio-pypage-0.1.5/pypage/heatmap.py`

 * *Files identical despite different names*

### Comparing `bio-pypage-0.1.4/pypage/hist.py` & `bio-pypage-0.1.5/pypage/hist.py`

 * *Files identical despite different names*

### Comparing `bio-pypage-0.1.4/pypage/information.py` & `bio-pypage-0.1.5/pypage/information.py`

 * *Files identical despite different names*

### Comparing `bio-pypage-0.1.4/pypage/io/accession_types.py` & `bio-pypage-0.1.5/pypage/io/accession_types.py`

 * *Files identical despite different names*

### Comparing `bio-pypage-0.1.4/pypage/io/expression.py` & `bio-pypage-0.1.5/pypage/io/expression.py`

 * *Files identical despite different names*

### Comparing `bio-pypage-0.1.4/pypage/io/ontology.py` & `bio-pypage-0.1.5/pypage/io/ontology.py`

 * *Files identical despite different names*

### Comparing `bio-pypage-0.1.4/pypage/page.py` & `bio-pypage-0.1.5/pypage/page.py`

 * *Files identical despite different names*

### Comparing `bio-pypage-0.1.4/pypage/utils.py` & `bio-pypage-0.1.5/pypage/utils.py`

 * *Files identical despite different names*

### Comparing `bio-pypage-0.1.4/setup.py` & `bio-pypage-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
    name='bio-pypage',
-   version='0.1.4',
+   version='0.1.5',
    description='Python implementation of the PAGE algorithm',
    author='Artemy Bakulin, Noam Teyssier',
    long_description=long_description,
    long_description_content_type="text/markdown",
    url='https://github.com/goodarzilab/pypage',
    author_email="logic2000.bakulin@gmail.com",
    packages=['pypage', 'pypage.io'],
```

