# Comparing `tmp/finch-clust-0.1.8.tar.gz` & `tmp/finch-clust-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finch-clust-0.1.8.tar", last modified: Wed Feb 22 08:01:24 2023, max compression
+gzip compressed data, was "finch-clust-0.1.9.tar", last modified: Sun Jun 18 13:19:41 2023, max compression
```

## Comparing `finch-clust-0.1.8.tar` & `finch-clust-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ssarfraz (12118) i14staff (10001)        0 2023-02-22 08:01:24.654965 finch-clust-0.1.8/
--rw-r--r--   0 ssarfraz (12118) i14staff (10001)    20717 2020-06-18 07:58:27.000000 finch-clust-0.1.8/LICENSE.txt
--rw-r--r--   0 ssarfraz (12118) i14staff (10001)     3675 2023-02-22 08:01:24.654965 finch-clust-0.1.8/PKG-INFO
--rw-r--r--   0 ssarfraz (12118) i14staff (10001)     2721 2022-09-14 11:44:22.000000 finch-clust-0.1.8/README.md
-drwxr-xr-x   0 ssarfraz (12118) i14staff (10001)        0 2023-02-22 08:01:24.622964 finch-clust-0.1.8/finch/
--rw-r--r--   0 ssarfraz (12118) i14staff (10001)       24 2022-08-23 09:49:33.000000 finch-clust-0.1.8/finch/__init__.py
--rw-r--r--   0 ssarfraz (12118) i14staff (10001)     7562 2022-08-26 08:16:50.000000 finch-clust-0.1.8/finch/finch.py
-drwxr-xr-x   0 ssarfraz (12118) i14staff (10001)        0 2023-02-22 08:01:24.646965 finch-clust-0.1.8/finch_clust.egg-info/
--rw-r--r--   0 ssarfraz (12118) i14staff (10001)     3675 2023-02-22 08:01:23.000000 finch-clust-0.1.8/finch_clust.egg-info/PKG-INFO
--rw-r--r--   0 ssarfraz (12118) i14staff (10001)      237 2023-02-22 08:01:23.000000 finch-clust-0.1.8/finch_clust.egg-info/SOURCES.txt
--rw-r--r--   0 ssarfraz (12118) i14staff (10001)        1 2023-02-22 08:01:23.000000 finch-clust-0.1.8/finch_clust.egg-info/dependency_links.txt
--rw-r--r--   0 ssarfraz (12118) i14staff (10001)       58 2023-02-22 08:01:23.000000 finch-clust-0.1.8/finch_clust.egg-info/requires.txt
--rw-r--r--   0 ssarfraz (12118) i14staff (10001)        6 2023-02-22 08:01:23.000000 finch-clust-0.1.8/finch_clust.egg-info/top_level.txt
--rw-r--r--   0 ssarfraz (12118) i14staff (10001)       38 2023-02-22 08:01:24.654965 finch-clust-0.1.8/setup.cfg
--rw-r--r--   0 ssarfraz (12118) i14staff (10001)     1360 2023-02-22 07:59:34.000000 finch-clust-0.1.8/setup.py
+drwxr-xr-x   0 ssarfraz (12118) i14staff (10001)        0 2023-06-18 13:19:41.108627 finch-clust-0.1.9/
+-rw-r--r--   0 ssarfraz (12118) i14staff (10001)    20717 2020-06-18 07:58:27.000000 finch-clust-0.1.9/LICENSE.txt
+-rw-r--r--   0 ssarfraz (12118) i14staff (10001)     3675 2023-06-18 13:19:41.104627 finch-clust-0.1.9/PKG-INFO
+-rw-r--r--   0 ssarfraz (12118) i14staff (10001)     2721 2022-09-14 11:44:22.000000 finch-clust-0.1.9/README.md
+drwxr-xr-x   0 ssarfraz (12118) i14staff (10001)        0 2023-06-18 13:19:41.064626 finch-clust-0.1.9/finch/
+-rw-r--r--   0 ssarfraz (12118) i14staff (10001)       24 2022-08-23 09:49:33.000000 finch-clust-0.1.9/finch/__init__.py
+-rw-r--r--   0 ssarfraz (12118) i14staff (10001)     7562 2022-08-26 08:16:50.000000 finch-clust-0.1.9/finch/finch.py
+drwxr-xr-x   0 ssarfraz (12118) i14staff (10001)        0 2023-06-18 13:19:41.100627 finch-clust-0.1.9/finch_clust.egg-info/
+-rw-r--r--   0 ssarfraz (12118) i14staff (10001)     3675 2023-06-18 13:19:40.000000 finch-clust-0.1.9/finch_clust.egg-info/PKG-INFO
+-rw-r--r--   0 ssarfraz (12118) i14staff (10001)      237 2023-06-18 13:19:40.000000 finch-clust-0.1.9/finch_clust.egg-info/SOURCES.txt
+-rw-r--r--   0 ssarfraz (12118) i14staff (10001)        1 2023-06-18 13:19:40.000000 finch-clust-0.1.9/finch_clust.egg-info/dependency_links.txt
+-rw-r--r--   0 ssarfraz (12118) i14staff (10001)       56 2023-06-18 13:19:40.000000 finch-clust-0.1.9/finch_clust.egg-info/requires.txt
+-rw-r--r--   0 ssarfraz (12118) i14staff (10001)        6 2023-06-18 13:19:40.000000 finch-clust-0.1.9/finch_clust.egg-info/top_level.txt
+-rw-r--r--   0 ssarfraz (12118) i14staff (10001)       38 2023-06-18 13:19:41.108627 finch-clust-0.1.9/setup.cfg
+-rw-r--r--   0 ssarfraz (12118) i14staff (10001)     1358 2023-06-18 13:17:49.000000 finch-clust-0.1.9/setup.py
```

### Comparing `finch-clust-0.1.8/LICENSE.txt` & `finch-clust-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `finch-clust-0.1.8/PKG-INFO` & `finch-clust-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finch-clust
-Version: 0.1.8
+Version: 0.1.9
 Summary: FINCH - First Integer Neighbor Clustering Hierarchy: A parameter-free fast clustering algorithm.
 Author: Saquib Sarfraz
 Author-email: saquibsarfraz@gmail.com
 Project-URL: Repository, https://github.com/ssarfraz/FINCH-Clustering
 Project-URL: Publication, https://openaccess.thecvf.com/content_CVPR_2019/html/Sarfraz_Efficient_Parameter-Free_Clustering_Using_First_Neighbor_Relations_CVPR_2019_paper.html
 Keywords: finch,finch clustering,clustering,hierarchical clustering
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `finch-clust-0.1.8/README.md` & `finch-clust-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `finch-clust-0.1.8/finch/finch.py` & `finch-clust-0.1.9/finch/finch.py`

 * *Files identical despite different names*

### Comparing `finch-clust-0.1.8/finch_clust.egg-info/PKG-INFO` & `finch-clust-0.1.9/finch_clust.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finch-clust
-Version: 0.1.8
+Version: 0.1.9
 Summary: FINCH - First Integer Neighbor Clustering Hierarchy: A parameter-free fast clustering algorithm.
 Author: Saquib Sarfraz
 Author-email: saquibsarfraz@gmail.com
 Project-URL: Repository, https://github.com/ssarfraz/FINCH-Clustering
 Project-URL: Publication, https://openaccess.thecvf.com/content_CVPR_2019/html/Sarfraz_Efficient_Parameter-Free_Clustering_Using_First_Neighbor_Relations_CVPR_2019_paper.html
 Keywords: finch,finch clustering,clustering,hierarchical clustering
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `finch-clust-0.1.8/setup.py` & `finch-clust-0.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setuptools.setup(
     name="finch-clust",
-    version="0.1.8",
+    version="0.1.9",
     author="Saquib Sarfraz",
     author_email="saquibsarfraz@gmail.com",
     description="FINCH - First Integer Neighbor Clustering Hierarchy: A parameter-free fast clustering algorithm.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['finch'],
     classifiers=[
@@ -21,17 +21,17 @@
         "Operating System :: MacOS",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
     keywords="finch, finch clustering, clustering, hierarchical clustering",
     install_requires=[
+        "scipy",
         "scikit-learn",
-        "numpy",
-        "sklearn"
+        "numpy"
     ],
     extras_require={'ann': ["numpy==1.21", "pynndescent"]},
     project_urls={
         "Repository": "https://github.com/ssarfraz/FINCH-Clustering",
         "Publication": "https://openaccess.thecvf.com/content_CVPR_2019/html/Sarfraz_Efficient_Parameter-Free_Clustering_Using_First_Neighbor_Relations_CVPR_2019_paper.html"
     }
 )
```

