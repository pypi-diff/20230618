# Comparing `tmp/split_markdown4gpt-1.0.2.tar.gz` & `tmp/split_markdown4gpt-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "split_markdown4gpt-1.0.2.tar", last modified: Sun Jun 18 01:08:39 2023, max compression
+gzip compressed data, was "split_markdown4gpt-1.0.3.tar", last modified: Sun Jun 18 01:23:03 2023, max compression
```

## Comparing `split_markdown4gpt-1.0.2.tar` & `split_markdown4gpt-1.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:08:39.230404 split_markdown4gpt-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-18 01:08:23.000000 split_markdown4gpt-1.0.2/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-18 01:08:23.000000 split_markdown4gpt-1.0.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:08:39.226404 split_markdown4gpt-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:08:39.226404 split_markdown4gpt-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-18 01:08:23.000000 split_markdown4gpt-1.0.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-18 01:08:23.000000 split_markdown4gpt-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-18 01:08:23.000000 split_markdown4gpt-1.0.2/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-18 01:08:23.000000 split_markdown4gpt-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 01:08:23.000000 split_markdown4gpt-1.0.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-18 01:08:23.000000 split_markdown4gpt-1.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-06-18 01:08:39.230404 split_markdown4gpt-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-06-18 01:08:23.000000 split_markdown4gpt-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-18 01:08:23.000000 split_markdown4gpt-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-18 01:08:39.230404 split_markdown4gpt-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-18 01:08:23.000000 split_markdown4gpt-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:08:39.226404 split_markdown4gpt-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:08:39.226404 split_markdown4gpt-1.0.2/src/split_markdown4gpt/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-18 01:08:23.000000 split_markdown4gpt-1.0.2/src/split_markdown4gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-18 01:08:23.000000 split_markdown4gpt-1.0.2/src/split_markdown4gpt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-06-18 01:08:23.000000 split_markdown4gpt-1.0.2/src/split_markdown4gpt/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:08:39.230404 split_markdown4gpt-1.0.2/src/split_markdown4gpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-06-18 01:08:39.000000 split_markdown4gpt-1.0.2/src/split_markdown4gpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-18 01:08:39.000000 split_markdown4gpt-1.0.2/src/split_markdown4gpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 01:08:39.000000 split_markdown4gpt-1.0.2/src/split_markdown4gpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-18 01:08:39.000000 split_markdown4gpt-1.0.2/src/split_markdown4gpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 01:08:38.000000 split_markdown4gpt-1.0.2/src/split_markdown4gpt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-18 01:08:39.000000 split_markdown4gpt-1.0.2/src/split_markdown4gpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 01:08:39.000000 split_markdown4gpt-1.0.2/src/split_markdown4gpt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:08:39.230404 split_markdown4gpt-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-18 01:08:23.000000 split_markdown4gpt-1.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-18 01:08:23.000000 split_markdown4gpt-1.0.2/tests/test.md
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-18 01:08:23.000000 split_markdown4gpt-1.0.2/tests/test_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-18 01:08:23.000000 split_markdown4gpt-1.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:23:03.183791 split_markdown4gpt-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:23:03.179791 split_markdown4gpt-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:23:03.183791 split_markdown4gpt-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6793 2023-06-18 01:23:03.183791 split_markdown4gpt-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-18 01:23:03.187791 split_markdown4gpt-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:23:03.183791 split_markdown4gpt-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:23:03.183791 split_markdown4gpt-1.0.3/src/split_markdown4gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/src/split_markdown4gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/src/split_markdown4gpt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/src/split_markdown4gpt/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:23:03.183791 split_markdown4gpt-1.0.3/src/split_markdown4gpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6793 2023-06-18 01:23:03.000000 split_markdown4gpt-1.0.3/src/split_markdown4gpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-18 01:23:03.000000 split_markdown4gpt-1.0.3/src/split_markdown4gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 01:23:03.000000 split_markdown4gpt-1.0.3/src/split_markdown4gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-18 01:23:03.000000 split_markdown4gpt-1.0.3/src/split_markdown4gpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 01:23:02.000000 split_markdown4gpt-1.0.3/src/split_markdown4gpt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-18 01:23:03.000000 split_markdown4gpt-1.0.3/src/split_markdown4gpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 01:23:03.000000 split_markdown4gpt-1.0.3/src/split_markdown4gpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:23:03.183791 split_markdown4gpt-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/tests/test.md
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/tests/test_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/tox.ini
```

### Comparing `split_markdown4gpt-1.0.2/.DS_Store` & `split_markdown4gpt-1.0.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.2/.coveragerc` & `split_markdown4gpt-1.0.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.2/.github/workflows/ci.yml` & `split_markdown4gpt-1.0.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.2/.gitignore` & `split_markdown4gpt-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.2/.pre-commit-config.yaml` & `split_markdown4gpt-1.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.2/LICENSE.txt` & `split_markdown4gpt-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.2/PKG-INFO` & `split_markdown4gpt-1.0.3/src/split_markdown4gpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
-Name: split_markdown4gpt
-Version: 1.0.2
+Name: split-markdown4gpt
+Version: 1.0.3
 Summary: A Python tool for splitting large Markdown files into smaller sections based on a specified token limit. This is particularly useful for processing large Markdown files with GPT models, as it allows the models to handle the data in manageable chunks.
 Home-page: https://github.com/twardoch/split-markdown4gpt
 Author: Adam Twardoch
 Author-email: adam+github@twardoch.com
 License: Apache-2.0
 Project-URL: Documentation, https://github.com/twardoch/split-markdown4gpt
 Project-URL: Source, https://github.com/twardoch/split-markdown4gpt
+Keywords: python,nlp,markdown,natural-language-processing,text-analysis,openai,text-summarization,summarization,text-processing,gpt,data-preprocessing,mistletoe,split-text,text-tokenization,openai-gpt,gpt-3,gpt-4,gpt-35-turbo,gpt-35-turbo-16k,markdown-processing
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -24,15 +25,15 @@
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 # split_markdown4gpt
 
 `split_markdown4gpt` is a Python tool designed to split large Markdown files into smaller sections based on a specified token limit. This is particularly useful for processing large Markdown files with GPT models, as it allows the models to handle the data in manageable chunks.
 
-_Version 1.0.2_ (2023-06-18)
+_Version 1.0.3_ (2023-06-18)
 
 ## Installation
 
 You can install `split_markdown4gpt` via pip:
 
 ```bash
 pip install split_markdown4gpt
```

### Comparing `split_markdown4gpt-1.0.2/README.md` & `split_markdown4gpt-1.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # split_markdown4gpt
 
 `split_markdown4gpt` is a Python tool designed to split large Markdown files into smaller sections based on a specified token limit. This is particularly useful for processing large Markdown files with GPT models, as it allows the models to handle the data in manageable chunks.
 
-_Version 1.0.2_ (2023-06-18)
+_Version 1.0.3_ (2023-06-18)
 
 ## Installation
 
 You can install `split_markdown4gpt` via pip:
 
 ```bash
 pip install split_markdown4gpt
```

### Comparing `split_markdown4gpt-1.0.2/setup.cfg` & `split_markdown4gpt-1.0.3/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 	Programming Language :: Python :: 3.10
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Topic :: Text Processing
 	Topic :: Text Processing :: Markup :: Markdown
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
+keywords = python, nlp, markdown, natural-language-processing, text-analysis, openai, text-summarization, summarization, text-processing, gpt, data-preprocessing, mistletoe, split-text, text-tokenization, openai-gpt, gpt-3, gpt-4, gpt-35-turbo, gpt-35-turbo-16k, markdown-processing
 
 [options]
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
```

### Comparing `split_markdown4gpt-1.0.2/setup.py` & `split_markdown4gpt-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.2/src/split_markdown4gpt/__init__.py` & `split_markdown4gpt-1.0.3/src/split_markdown4gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.2/src/split_markdown4gpt/__main__.py` & `split_markdown4gpt-1.0.3/src/split_markdown4gpt/__main__.py`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.2/src/split_markdown4gpt/splitter.py` & `split_markdown4gpt-1.0.3/src/split_markdown4gpt/splitter.py`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.2/src/split_markdown4gpt.egg-info/PKG-INFO` & `split_markdown4gpt-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
-Name: split-markdown4gpt
-Version: 1.0.2
+Name: split_markdown4gpt
+Version: 1.0.3
 Summary: A Python tool for splitting large Markdown files into smaller sections based on a specified token limit. This is particularly useful for processing large Markdown files with GPT models, as it allows the models to handle the data in manageable chunks.
 Home-page: https://github.com/twardoch/split-markdown4gpt
 Author: Adam Twardoch
 Author-email: adam+github@twardoch.com
 License: Apache-2.0
 Project-URL: Documentation, https://github.com/twardoch/split-markdown4gpt
 Project-URL: Source, https://github.com/twardoch/split-markdown4gpt
+Keywords: python,nlp,markdown,natural-language-processing,text-analysis,openai,text-summarization,summarization,text-processing,gpt,data-preprocessing,mistletoe,split-text,text-tokenization,openai-gpt,gpt-3,gpt-4,gpt-35-turbo,gpt-35-turbo-16k,markdown-processing
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -24,15 +25,15 @@
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 # split_markdown4gpt
 
 `split_markdown4gpt` is a Python tool designed to split large Markdown files into smaller sections based on a specified token limit. This is particularly useful for processing large Markdown files with GPT models, as it allows the models to handle the data in manageable chunks.
 
-_Version 1.0.2_ (2023-06-18)
+_Version 1.0.3_ (2023-06-18)
 
 ## Installation
 
 You can install `split_markdown4gpt` via pip:
 
 ```bash
 pip install split_markdown4gpt
```

### Comparing `split_markdown4gpt-1.0.2/src/split_markdown4gpt.egg-info/SOURCES.txt` & `split_markdown4gpt-1.0.3/src/split_markdown4gpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.2/tests/test.md` & `split_markdown4gpt-1.0.3/tests/test.md`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.2/tox.ini` & `split_markdown4gpt-1.0.3/tox.ini`

 * *Files identical despite different names*

