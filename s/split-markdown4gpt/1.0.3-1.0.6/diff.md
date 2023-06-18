# Comparing `tmp/split_markdown4gpt-1.0.3.tar.gz` & `tmp/split_markdown4gpt-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "split_markdown4gpt-1.0.3.tar", last modified: Sun Jun 18 01:23:03 2023, max compression
+gzip compressed data, was "split_markdown4gpt-1.0.6.tar", last modified: Sun Jun 18 02:07:46 2023, max compression
```

## Comparing `split_markdown4gpt-1.0.3.tar` & `split_markdown4gpt-1.0.6.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:23:03.183791 split_markdown4gpt-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:23:03.179791 split_markdown4gpt-1.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:23:03.183791 split_markdown4gpt-1.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6793 2023-06-18 01:23:03.183791 split_markdown4gpt-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-18 01:23:03.187791 split_markdown4gpt-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:23:03.183791 split_markdown4gpt-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:23:03.183791 split_markdown4gpt-1.0.3/src/split_markdown4gpt/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/src/split_markdown4gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/src/split_markdown4gpt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/src/split_markdown4gpt/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:23:03.183791 split_markdown4gpt-1.0.3/src/split_markdown4gpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6793 2023-06-18 01:23:03.000000 split_markdown4gpt-1.0.3/src/split_markdown4gpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-18 01:23:03.000000 split_markdown4gpt-1.0.3/src/split_markdown4gpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 01:23:03.000000 split_markdown4gpt-1.0.3/src/split_markdown4gpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-18 01:23:03.000000 split_markdown4gpt-1.0.3/src/split_markdown4gpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 01:23:02.000000 split_markdown4gpt-1.0.3/src/split_markdown4gpt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-18 01:23:03.000000 split_markdown4gpt-1.0.3/src/split_markdown4gpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 01:23:03.000000 split_markdown4gpt-1.0.3/src/split_markdown4gpt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:23:03.183791 split_markdown4gpt-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/tests/test.md
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/tests/test_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-18 01:22:49.000000 split_markdown4gpt-1.0.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:07:46.134235 split_markdown4gpt-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:07:46.130234 split_markdown4gpt-1.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:07:46.130234 split_markdown4gpt-1.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/API.md
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-06-18 02:07:46.134235 split_markdown4gpt-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/pydoc-markdown.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-18 02:07:46.134235 split_markdown4gpt-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:07:46.130234 split_markdown4gpt-1.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:07:46.130234 split_markdown4gpt-1.0.6/src/split_markdown4gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/src/split_markdown4gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/src/split_markdown4gpt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/src/split_markdown4gpt/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:07:46.134235 split_markdown4gpt-1.0.6/src/split_markdown4gpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-06-18 02:07:46.000000 split_markdown4gpt-1.0.6/src/split_markdown4gpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-18 02:07:46.000000 split_markdown4gpt-1.0.6/src/split_markdown4gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:07:46.000000 split_markdown4gpt-1.0.6/src/split_markdown4gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-18 02:07:46.000000 split_markdown4gpt-1.0.6/src/split_markdown4gpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:07:45.000000 split_markdown4gpt-1.0.6/src/split_markdown4gpt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-18 02:07:46.000000 split_markdown4gpt-1.0.6/src/split_markdown4gpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 02:07:46.000000 split_markdown4gpt-1.0.6/src/split_markdown4gpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:07:46.134235 split_markdown4gpt-1.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/tests/test.md
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/tests/test_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-18 02:07:32.000000 split_markdown4gpt-1.0.6/tox.ini
```

### Comparing `split_markdown4gpt-1.0.3/.DS_Store` & `split_markdown4gpt-1.0.6/.DS_Store`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.3/.coveragerc` & `split_markdown4gpt-1.0.6/.coveragerc`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.3/.github/workflows/ci.yml` & `split_markdown4gpt-1.0.6/.github/workflows/ci.yml`

 * *Files 16% similar despite different names*

```diff
@@ -6,20 +6,21 @@
     tags: ['v[0-9]*', '[0-9]+.[0-9]+*']
   pull_request:
   workflow_dispatch:
   schedule:
     - cron: '0 0 1,16 * *'
 
 permissions:
-  contents: read
+  contents: write
 
 concurrency:
   group: >-
     ${{ github.workflow }}-${{ github.ref_type }}- ${{ github.event.pull_request.number || github.sha }}
 
+
   cancel-in-progress: true
 
 jobs:
   test:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
@@ -31,14 +32,33 @@
         run: |
           python -m pip install --upgrade pip
           pip install pytest
           pip install -e .
       - name: Run tests
         run: pytest
 
+  update-docs:
+    needs: test
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v2
+      - name: Set up Python
+        uses: actions/setup-python@v2
+        with:
+          python-version: '3.10'
+      - name: Install pydoc-markdown
+        run: pip install pydoc-markdown
+      - name: Generate API documentation
+        run: pydoc-markdown > API.md
+      - name: Commit and push if it's changed
+        uses: EndBug/add-and-commit@v9
+        with:
+          message: 'Update API documentation'
+          add: 'API.md'
+      
   build-and-publish:
     needs: test
     runs-on: ubuntu-latest
     if: startsWith(github.ref, 'refs/tags/')
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python
@@ -52,7 +72,9 @@
       - name: Build distribution
         run: python -m build
       - name: Publish to PyPi
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
           password: ${{ secrets.PYPI_TOKEN }}
+
+
```

### Comparing `split_markdown4gpt-1.0.3/.gitignore` & `split_markdown4gpt-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.3/.pre-commit-config.yaml` & `split_markdown4gpt-1.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.3/LICENSE.txt` & `split_markdown4gpt-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.3/PKG-INFO` & `split_markdown4gpt-1.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: split_markdown4gpt
-Version: 1.0.3
+Version: 1.0.6
 Summary: A Python tool for splitting large Markdown files into smaller sections based on a specified token limit. This is particularly useful for processing large Markdown files with GPT models, as it allows the models to handle the data in manageable chunks.
 Home-page: https://github.com/twardoch/split-markdown4gpt
 Author: Adam Twardoch
 Author-email: adam+github@twardoch.com
 License: Apache-2.0
-Project-URL: Documentation, https://github.com/twardoch/split-markdown4gpt
+Project-URL: Documentation, https://twardoch.github.io/split-markdown4gpt/
 Project-URL: Source, https://github.com/twardoch/split-markdown4gpt
 Keywords: python,nlp,markdown,natural-language-processing,text-analysis,openai,text-summarization,summarization,text-processing,gpt,data-preprocessing,mistletoe,split-text,text-tokenization,openai-gpt,gpt-3,gpt-4,gpt-35-turbo,gpt-35-turbo-16k,markdown-processing
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -25,15 +25,15 @@
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 # split_markdown4gpt
 
 `split_markdown4gpt` is a Python tool designed to split large Markdown files into smaller sections based on a specified token limit. This is particularly useful for processing large Markdown files with GPT models, as it allows the models to handle the data in manageable chunks.
 
-_Version 1.0.3_ (2023-06-18)
+_**Version 1.0.6** (2023-06-18)_
 
 ## Installation
 
 You can install `split_markdown4gpt` via pip:
 
 ```bash
 pip install split_markdown4gpt
@@ -93,14 +93,16 @@
 sections = split("path_to_your_file.md", model="gpt-3.5-turbo", limit=4096)
 for section in sections:
     print(section)
 ```
 
 This code does the same thing as the CLI command above, but in Python.
 
+- **[See the API documentation](https://twardoch.github.io/split-markdown4gpt/API.html)** for more advanced usage
+
 ## How it Works
 
 `split_markdown4gpt` works by tokenizing the input Markdown file using the specified GPT model's tokenizer (default is `gpt-3.5-turbo`). It then splits the file into sections, each containing no more than the specified token limit.
 
 The splitting process respects the structure of the Markdown file. It will not split a section (as defined by Markdown headings) across multiple output sections unless the section is longer than the token limit. In that case, it
 
 will split the section at the sentence level.
@@ -120,37 +122,17 @@
 
 - **Text Generation**: If you're using a GPT model to generate text based on a large Markdown file, you can use `split_markdown4gpt` to split the file into manageable sections. This allows the GPT model to process the file in chunks, preventing memory overflow errors.
 
 - **Data Preprocessing**: In machine learning projects, you often need to preprocess your data before feeding it into your model. If your data is in the form of large Markdown files, `split_markdown4gpt` can help you split these files into smaller sections based on the token limit of your model.
 
 - **Document Analysis**: If you're analyzing large Markdown documents (e.g., extracting keywords, summarizing content), you can use `split_markdown4gpt` to break down the documents into smaller sections. This makes the analysis more manageable and efficient.
 
-### Usage Examples
-
-Here's an example of how you can use `split_markdown4gpt` in your Python code:
-
-```python
-from split_markdown4gpt import split
-
-# Path to your large Markdown file
-md_file_path = "path_to_your_file.md"
-
-# Split the file into sections
-sections = split(md_file_path, model="gpt-3.5-turbo", limit=4096)
-
-# Process each section with your GPT model
-for section in sections:
-    # Replace this with your GPT model's processing function
-    process_with_gpt_model(section)
-```
-
-In this example, `process_with_gpt_model` is a placeholder for your GPT model's processing function. You would replace this with the actual function you're using to process the text with your GPT model.
-
 ## Contributing
 
 Contributions to `split_markdown4gpt` are welcome! Please open an issue or submit a pull request on the [GitHub repository](https://github.com/twardoch/split-markdown4gpt).
 
 ## License
 
-- Copyright (c) 2023 Adam Twardoch
+- Copyright (c) 2023 [Adam Twardoch](./AUTHORS.md)
 - Written with assistance from ChatGPT
-- Licensed under the [Apache License 2.0](./LICENSE.txt)
+- Licensed under the [Apache License 2.0](./LICENSE.txt)<a id="split_markdown4gpt"></a>
+
```

### Comparing `split_markdown4gpt-1.0.3/README.md` & `split_markdown4gpt-1.0.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # split_markdown4gpt
 
 `split_markdown4gpt` is a Python tool designed to split large Markdown files into smaller sections based on a specified token limit. This is particularly useful for processing large Markdown files with GPT models, as it allows the models to handle the data in manageable chunks.
 
-_Version 1.0.3_ (2023-06-18)
+_**Version 1.0.6** (2023-06-18)_
 
 ## Installation
 
 You can install `split_markdown4gpt` via pip:
 
 ```bash
 pip install split_markdown4gpt
@@ -66,14 +66,16 @@
 sections = split("path_to_your_file.md", model="gpt-3.5-turbo", limit=4096)
 for section in sections:
     print(section)
 ```
 
 This code does the same thing as the CLI command above, but in Python.
 
+- **[See the API documentation](https://twardoch.github.io/split-markdown4gpt/API.html)** for more advanced usage
+
 ## How it Works
 
 `split_markdown4gpt` works by tokenizing the input Markdown file using the specified GPT model's tokenizer (default is `gpt-3.5-turbo`). It then splits the file into sections, each containing no more than the specified token limit.
 
 The splitting process respects the structure of the Markdown file. It will not split a section (as defined by Markdown headings) across multiple output sections unless the section is longer than the token limit. In that case, it
 
 will split the section at the sentence level.
@@ -93,37 +95,17 @@
 
 - **Text Generation**: If you're using a GPT model to generate text based on a large Markdown file, you can use `split_markdown4gpt` to split the file into manageable sections. This allows the GPT model to process the file in chunks, preventing memory overflow errors.
 
 - **Data Preprocessing**: In machine learning projects, you often need to preprocess your data before feeding it into your model. If your data is in the form of large Markdown files, `split_markdown4gpt` can help you split these files into smaller sections based on the token limit of your model.
 
 - **Document Analysis**: If you're analyzing large Markdown documents (e.g., extracting keywords, summarizing content), you can use `split_markdown4gpt` to break down the documents into smaller sections. This makes the analysis more manageable and efficient.
 
-### Usage Examples
-
-Here's an example of how you can use `split_markdown4gpt` in your Python code:
-
-```python
-from split_markdown4gpt import split
-
-# Path to your large Markdown file
-md_file_path = "path_to_your_file.md"
-
-# Split the file into sections
-sections = split(md_file_path, model="gpt-3.5-turbo", limit=4096)
-
-# Process each section with your GPT model
-for section in sections:
-    # Replace this with your GPT model's processing function
-    process_with_gpt_model(section)
-```
-
-In this example, `process_with_gpt_model` is a placeholder for your GPT model's processing function. You would replace this with the actual function you're using to process the text with your GPT model.
-
 ## Contributing
 
 Contributions to `split_markdown4gpt` are welcome! Please open an issue or submit a pull request on the [GitHub repository](https://github.com/twardoch/split-markdown4gpt).
 
 ## License
 
-- Copyright (c) 2023 Adam Twardoch
+- Copyright (c) 2023 [Adam Twardoch](./AUTHORS.md)
 - Written with assistance from ChatGPT
-- Licensed under the [Apache License 2.0](./LICENSE.txt)
+- Licensed under the [Apache License 2.0](./LICENSE.txt)<a id="split_markdown4gpt"></a>
+
```

### Comparing `split_markdown4gpt-1.0.3/setup.cfg` & `split_markdown4gpt-1.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 author_email = adam+github@twardoch.com
 license = Apache-2.0
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://github.com/twardoch/split-markdown4gpt
 project_urls = 
-	Documentation = https://github.com/twardoch/split-markdown4gpt
+	Documentation = https://twardoch.github.io/split-markdown4gpt/
 	Source = https://github.com/twardoch/split-markdown4gpt
 platforms = any
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.10
```

### Comparing `split_markdown4gpt-1.0.3/setup.py` & `split_markdown4gpt-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.3/src/split_markdown4gpt/__init__.py` & `split_markdown4gpt-1.0.6/src/split_markdown4gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.3/src/split_markdown4gpt/__main__.py` & `split_markdown4gpt-1.0.6/src/split_markdown4gpt/__main__.py`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.3/src/split_markdown4gpt/splitter.py` & `split_markdown4gpt-1.0.6/src/split_markdown4gpt/splitter.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 RE_NEWLINES = re.compile("\n{3,}")
 
 Section = namedtuple("Section", ("md", "size"))
 
 
 class MarkdownLLMSplitter:
     """
-    A class to split Markdown files into sections according to GPT token size limits.
+    A class to split Markdown files into sections according to GPT token size limits. Currently supports OpenAI models only, since it uses the `tiktoken` library for tokenization.
     
     Attributes:
         gptoker: GPT tokenizer instance used to calculate token sizes.
         gptok_limit: The maximum number of GPT tokens allowed per section.
         md_meta: Metadata found in the source Markdown file.
         md_str: The source Markdown string.
         md_doc: The parsed source Markdown document as a mistletoe Document instance.
```

### Comparing `split_markdown4gpt-1.0.3/src/split_markdown4gpt.egg-info/PKG-INFO` & `split_markdown4gpt-1.0.6/src/split_markdown4gpt.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: split-markdown4gpt
-Version: 1.0.3
+Version: 1.0.6
 Summary: A Python tool for splitting large Markdown files into smaller sections based on a specified token limit. This is particularly useful for processing large Markdown files with GPT models, as it allows the models to handle the data in manageable chunks.
 Home-page: https://github.com/twardoch/split-markdown4gpt
 Author: Adam Twardoch
 Author-email: adam+github@twardoch.com
 License: Apache-2.0
-Project-URL: Documentation, https://github.com/twardoch/split-markdown4gpt
+Project-URL: Documentation, https://twardoch.github.io/split-markdown4gpt/
 Project-URL: Source, https://github.com/twardoch/split-markdown4gpt
 Keywords: python,nlp,markdown,natural-language-processing,text-analysis,openai,text-summarization,summarization,text-processing,gpt,data-preprocessing,mistletoe,split-text,text-tokenization,openai-gpt,gpt-3,gpt-4,gpt-35-turbo,gpt-35-turbo-16k,markdown-processing
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -25,15 +25,15 @@
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 # split_markdown4gpt
 
 `split_markdown4gpt` is a Python tool designed to split large Markdown files into smaller sections based on a specified token limit. This is particularly useful for processing large Markdown files with GPT models, as it allows the models to handle the data in manageable chunks.
 
-_Version 1.0.3_ (2023-06-18)
+_**Version 1.0.6** (2023-06-18)_
 
 ## Installation
 
 You can install `split_markdown4gpt` via pip:
 
 ```bash
 pip install split_markdown4gpt
@@ -93,14 +93,16 @@
 sections = split("path_to_your_file.md", model="gpt-3.5-turbo", limit=4096)
 for section in sections:
     print(section)
 ```
 
 This code does the same thing as the CLI command above, but in Python.
 
+- **[See the API documentation](https://twardoch.github.io/split-markdown4gpt/API.html)** for more advanced usage
+
 ## How it Works
 
 `split_markdown4gpt` works by tokenizing the input Markdown file using the specified GPT model's tokenizer (default is `gpt-3.5-turbo`). It then splits the file into sections, each containing no more than the specified token limit.
 
 The splitting process respects the structure of the Markdown file. It will not split a section (as defined by Markdown headings) across multiple output sections unless the section is longer than the token limit. In that case, it
 
 will split the section at the sentence level.
@@ -120,37 +122,17 @@
 
 - **Text Generation**: If you're using a GPT model to generate text based on a large Markdown file, you can use `split_markdown4gpt` to split the file into manageable sections. This allows the GPT model to process the file in chunks, preventing memory overflow errors.
 
 - **Data Preprocessing**: In machine learning projects, you often need to preprocess your data before feeding it into your model. If your data is in the form of large Markdown files, `split_markdown4gpt` can help you split these files into smaller sections based on the token limit of your model.
 
 - **Document Analysis**: If you're analyzing large Markdown documents (e.g., extracting keywords, summarizing content), you can use `split_markdown4gpt` to break down the documents into smaller sections. This makes the analysis more manageable and efficient.
 
-### Usage Examples
-
-Here's an example of how you can use `split_markdown4gpt` in your Python code:
-
-```python
-from split_markdown4gpt import split
-
-# Path to your large Markdown file
-md_file_path = "path_to_your_file.md"
-
-# Split the file into sections
-sections = split(md_file_path, model="gpt-3.5-turbo", limit=4096)
-
-# Process each section with your GPT model
-for section in sections:
-    # Replace this with your GPT model's processing function
-    process_with_gpt_model(section)
-```
-
-In this example, `process_with_gpt_model` is a placeholder for your GPT model's processing function. You would replace this with the actual function you're using to process the text with your GPT model.
-
 ## Contributing
 
 Contributions to `split_markdown4gpt` are welcome! Please open an issue or submit a pull request on the [GitHub repository](https://github.com/twardoch/split-markdown4gpt).
 
 ## License
 
-- Copyright (c) 2023 Adam Twardoch
+- Copyright (c) 2023 [Adam Twardoch](./AUTHORS.md)
 - Written with assistance from ChatGPT
-- Licensed under the [Apache License 2.0](./LICENSE.txt)
+- Licensed under the [Apache License 2.0](./LICENSE.txt)<a id="split_markdown4gpt"></a>
+
```

### Comparing `split_markdown4gpt-1.0.3/src/split_markdown4gpt.egg-info/SOURCES.txt` & `split_markdown4gpt-1.0.6/src/split_markdown4gpt.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 .DS_Store
 .coveragerc
 .gitignore
 .isort.cfg
 .pre-commit-config.yaml
+API.md
 AUTHORS.md
 LICENSE.txt
 README.md
+pydoc-markdown.yml
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 .github/workflows/ci.yml
 src/split_markdown4gpt/__init__.py
 src/split_markdown4gpt/__main__.py
```

### Comparing `split_markdown4gpt-1.0.3/tests/test.md` & `split_markdown4gpt-1.0.6/tests/test.md`

 * *Files identical despite different names*

### Comparing `split_markdown4gpt-1.0.3/tox.ini` & `split_markdown4gpt-1.0.6/tox.ini`

 * *Files identical despite different names*

