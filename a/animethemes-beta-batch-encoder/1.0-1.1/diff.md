# Comparing `tmp/animethemes-beta-batch-encoder-1.0.tar.gz` & `tmp/animethemes-beta-batch-encoder-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animethemes-beta-batch-encoder-1.0.tar", last modified: Sun Jun 18 16:33:42 2023, max compression
+gzip compressed data, was "animethemes-beta-batch-encoder-1.1.tar", last modified: Sun Jun 18 16:57:16 2023, max compression
```

## Comparing `animethemes-beta-batch-encoder-1.0.tar` & `animethemes-beta-batch-encoder-1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 16:33:42.382031 animethemes-beta-batch-encoder-1.0/
--rw-rw-rw-   0        0        0     1082 2023-06-16 19:11:39.000000 animethemes-beta-batch-encoder-1.0/LICENSE
--rw-rw-rw-   0        0        0     4718 2023-06-18 16:33:42.381031 animethemes-beta-batch-encoder-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3810 2023-06-18 16:30:02.000000 animethemes-beta-batch-encoder-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 16:33:42.358065 animethemes-beta-batch-encoder-1.0/animethemes_beta_batch_encoder.egg-info/
--rw-rw-rw-   0        0        0     4718 2023-06-18 16:33:42.000000 animethemes-beta-batch-encoder-1.0/animethemes_beta_batch_encoder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      643 2023-06-18 16:33:42.000000 animethemes-beta-batch-encoder-1.0/animethemes_beta_batch_encoder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 16:33:42.000000 animethemes-beta-batch-encoder-1.0/animethemes_beta_batch_encoder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-18 16:33:42.000000 animethemes-beta-batch-encoder-1.0/animethemes_beta_batch_encoder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-18 16:33:42.000000 animethemes-beta-batch-encoder-1.0/animethemes_beta_batch_encoder.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-18 16:33:42.380030 animethemes-beta-batch-encoder-1.0/batch_encoder/
--rw-rw-rw-   0        0        0        0 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.0/batch_encoder/__init__.py
--rw-rw-rw-   0        0        0     7406 2023-06-18 16:30:18.000000 animethemes-beta-batch-encoder-1.0/batch_encoder/__main__.py
--rw-rw-rw-   0        0        0     1280 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.0/batch_encoder/_bitrate_mode.py
--rw-rw-rw-   0        0        0     2615 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.0/batch_encoder/_colorspace.py
--rw-rw-rw-   0        0        0    13495 2023-06-16 19:01:34.000000 animethemes-beta-batch-encoder-1.0/batch_encoder/_encode_webm.py
--rw-rw-rw-   0        0        0     3814 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.0/batch_encoder/_encoding_config.py
--rw-rw-rw-   0        0        0     5145 2023-06-18 16:06:11.000000 animethemes-beta-batch-encoder-1.0/batch_encoder/_interface.py
--rw-rw-rw-   0        0        0     2527 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.0/batch_encoder/_loudnorm_filter.py
--rw-rw-rw-   0        0        0      779 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.0/batch_encoder/_seek.py
--rw-rw-rw-   0        0        0     6874 2023-06-18 15:20:40.000000 animethemes-beta-batch-encoder-1.0/batch_encoder/_seek_collector.py
--rw-rw-rw-   0        0        0     6594 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.0/batch_encoder/_source_file.py
--rw-rw-rw-   0        0        0     1375 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.0/batch_encoder/_utils.py
--rw-rw-rw-   0        0        0       42 2023-06-18 16:33:42.382031 animethemes-beta-batch-encoder-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1199 2023-06-18 16:13:09.000000 animethemes-beta-batch-encoder-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:57:16.940486 animethemes-beta-batch-encoder-1.1/
+-rw-rw-rw-   0        0        0     1082 2023-06-16 19:11:39.000000 animethemes-beta-batch-encoder-1.1/LICENSE
+-rw-rw-rw-   0        0        0     4718 2023-06-18 16:57:16.939487 animethemes-beta-batch-encoder-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3810 2023-06-18 16:30:02.000000 animethemes-beta-batch-encoder-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 16:57:16.926487 animethemes-beta-batch-encoder-1.1/animethemes_beta_batch_encoder.egg-info/
+-rw-rw-rw-   0        0        0     4718 2023-06-18 16:57:16.000000 animethemes-beta-batch-encoder-1.1/animethemes_beta_batch_encoder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      703 2023-06-18 16:57:16.000000 animethemes-beta-batch-encoder-1.1/animethemes_beta_batch_encoder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 16:57:16.000000 animethemes-beta-batch-encoder-1.1/animethemes_beta_batch_encoder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-18 16:57:16.000000 animethemes-beta-batch-encoder-1.1/animethemes_beta_batch_encoder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-18 16:57:16.000000 animethemes-beta-batch-encoder-1.1/animethemes_beta_batch_encoder.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 16:57:16.938488 animethemes-beta-batch-encoder-1.1/beta_batch_encoder/
+-rw-rw-rw-   0        0        0        0 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.1/beta_batch_encoder/__init__.py
+-rw-rw-rw-   0        0        0     7406 2023-06-18 16:30:18.000000 animethemes-beta-batch-encoder-1.1/beta_batch_encoder/__main__.py
+-rw-rw-rw-   0        0        0     1280 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.1/beta_batch_encoder/_bitrate_mode.py
+-rw-rw-rw-   0        0        0     2615 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.1/beta_batch_encoder/_colorspace.py
+-rw-rw-rw-   0        0        0    13495 2023-06-16 19:01:34.000000 animethemes-beta-batch-encoder-1.1/beta_batch_encoder/_encode_webm.py
+-rw-rw-rw-   0        0        0     3814 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.1/beta_batch_encoder/_encoding_config.py
+-rw-rw-rw-   0        0        0     5145 2023-06-18 16:06:11.000000 animethemes-beta-batch-encoder-1.1/beta_batch_encoder/_interface.py
+-rw-rw-rw-   0        0        0     2527 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.1/beta_batch_encoder/_loudnorm_filter.py
+-rw-rw-rw-   0        0        0      779 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.1/beta_batch_encoder/_seek.py
+-rw-rw-rw-   0        0        0     6874 2023-06-18 15:20:40.000000 animethemes-beta-batch-encoder-1.1/beta_batch_encoder/_seek_collector.py
+-rw-rw-rw-   0        0        0     6594 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.1/beta_batch_encoder/_source_file.py
+-rw-rw-rw-   0        0        0     1375 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.1/beta_batch_encoder/_utils.py
+-rw-rw-rw-   0        0        0       42 2023-06-18 16:57:16.940486 animethemes-beta-batch-encoder-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1199 2023-06-18 16:52:39.000000 animethemes-beta-batch-encoder-1.1/setup.py
```

### Comparing `animethemes-beta-batch-encoder-1.0/LICENSE` & `animethemes-beta-batch-encoder-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.0/PKG-INFO` & `animethemes-beta-batch-encoder-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animethemes-beta-batch-encoder
-Version: 1.0
+Version: 1.1
 Summary: Generate/Execute FFmpeg commands for files in acting directory
 Home-page: https://github.com/AnimeThemes/animethemes-batch-encoder
 Author: AnimeThemes
 Author-email: admin@animethemes.moe
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `animethemes-beta-batch-encoder-1.0/README.md` & `animethemes-beta-batch-encoder-1.1/README.md`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.0/animethemes_beta_batch_encoder.egg-info/PKG-INFO` & `animethemes-beta-batch-encoder-1.1/animethemes_beta_batch_encoder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animethemes-beta-batch-encoder
-Version: 1.0
+Version: 1.1
 Summary: Generate/Execute FFmpeg commands for files in acting directory
 Home-page: https://github.com/AnimeThemes/animethemes-batch-encoder
 Author: AnimeThemes
 Author-email: admin@animethemes.moe
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `animethemes-beta-batch-encoder-1.0/animethemes_beta_batch_encoder.egg-info/SOURCES.txt` & `animethemes-beta-batch-encoder-1.1/animethemes_beta_batch_encoder.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 README.md
 setup.py
 animethemes_beta_batch_encoder.egg-info/PKG-INFO
 animethemes_beta_batch_encoder.egg-info/SOURCES.txt
 animethemes_beta_batch_encoder.egg-info/dependency_links.txt
 animethemes_beta_batch_encoder.egg-info/requires.txt
 animethemes_beta_batch_encoder.egg-info/top_level.txt
-batch_encoder/__init__.py
-batch_encoder/__main__.py
-batch_encoder/_bitrate_mode.py
-batch_encoder/_colorspace.py
-batch_encoder/_encode_webm.py
-batch_encoder/_encoding_config.py
-batch_encoder/_interface.py
-batch_encoder/_loudnorm_filter.py
-batch_encoder/_seek.py
-batch_encoder/_seek_collector.py
-batch_encoder/_source_file.py
-batch_encoder/_utils.py
+beta_batch_encoder/__init__.py
+beta_batch_encoder/__main__.py
+beta_batch_encoder/_bitrate_mode.py
+beta_batch_encoder/_colorspace.py
+beta_batch_encoder/_encode_webm.py
+beta_batch_encoder/_encoding_config.py
+beta_batch_encoder/_interface.py
+beta_batch_encoder/_loudnorm_filter.py
+beta_batch_encoder/_seek.py
+beta_batch_encoder/_seek_collector.py
+beta_batch_encoder/_source_file.py
+beta_batch_encoder/_utils.py
```

### Comparing `animethemes-beta-batch-encoder-1.0/batch_encoder/__main__.py` & `animethemes-beta-batch-encoder-1.1/beta_batch_encoder/__main__.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.0/batch_encoder/_bitrate_mode.py` & `animethemes-beta-batch-encoder-1.1/beta_batch_encoder/_bitrate_mode.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.0/batch_encoder/_colorspace.py` & `animethemes-beta-batch-encoder-1.1/beta_batch_encoder/_colorspace.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.0/batch_encoder/_encode_webm.py` & `animethemes-beta-batch-encoder-1.1/beta_batch_encoder/_encode_webm.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.0/batch_encoder/_encoding_config.py` & `animethemes-beta-batch-encoder-1.1/beta_batch_encoder/_encoding_config.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.0/batch_encoder/_interface.py` & `animethemes-beta-batch-encoder-1.1/beta_batch_encoder/_interface.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.0/batch_encoder/_loudnorm_filter.py` & `animethemes-beta-batch-encoder-1.1/beta_batch_encoder/_loudnorm_filter.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.0/batch_encoder/_seek.py` & `animethemes-beta-batch-encoder-1.1/beta_batch_encoder/_seek.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.0/batch_encoder/_seek_collector.py` & `animethemes-beta-batch-encoder-1.1/beta_batch_encoder/_seek_collector.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.0/batch_encoder/_source_file.py` & `animethemes-beta-batch-encoder-1.1/beta_batch_encoder/_source_file.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.0/batch_encoder/_utils.py` & `animethemes-beta-batch-encoder-1.1/beta_batch_encoder/_utils.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.0/setup.py` & `animethemes-beta-batch-encoder-1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='animethemes-beta-batch-encoder',
-    version='1.0',
+    version='1.1',
     author='AnimeThemes',
     author_email='admin@animethemes.moe',
     url='https://github.com/AnimeThemes/animethemes-batch-encoder',
     description='Generate/Execute FFmpeg commands for files in acting directory',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

