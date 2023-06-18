# Comparing `tmp/tailwiz-0.0.8.tar.gz` & `tmp/tailwiz-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tailwiz-0.0.8.tar", last modified: Tue Feb 21 00:04:48 2023, max compression
+gzip compressed data, was "dist/tailwiz-0.0.9.tar", last modified: Thu Feb 23 06:55:11 2023, max compression
```

## Comparing `tailwiz-0.0.8.tar` & `tailwiz-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-sr-x   0 timdai   (20656) future   (20099)        0 2023-02-21 00:04:48.000000 tailwiz-0.0.8/
--rw-r--r--   0 timdai   (20656) future   (20099)     1068 2023-02-20 05:20:56.000000 tailwiz-0.0.8/LICENSE
--rw-r--r--   0 timdai   (20656) future   (20099)     6291 2023-02-21 00:04:48.000000 tailwiz-0.0.8/PKG-INFO
--rw-r--r--   0 timdai   (20656) future   (20099)     5830 2023-02-20 23:06:50.000000 tailwiz-0.0.8/README.md
--rw-r--r--   0 timdai   (20656) future   (20099)       38 2023-02-21 00:04:48.000000 tailwiz-0.0.8/setup.cfg
--rw-r--r--   0 timdai   (20656) future   (20099)      884 2023-02-20 18:08:53.000000 tailwiz-0.0.8/setup.py
-drwxr-sr-x   0 timdai   (20656) future   (20099)        0 2023-02-21 00:04:48.000000 tailwiz-0.0.8/tailwiz/
--rw-r--r--   0 timdai   (20656) future   (20099)       80 2023-02-10 21:35:09.000000 tailwiz-0.0.8/tailwiz/__init__.py
--rw-r--r--   0 timdai   (20656) future   (20099)      201 2023-02-10 21:30:41.000000 tailwiz-0.0.8/tailwiz/list_tasks.py
-drwxr-sr-x   0 timdai   (20656) future   (20099)        0 2023-02-21 00:04:48.000000 tailwiz-0.0.8/tailwiz/tasks/
--rw-r--r--   0 timdai   (20656) future   (20099)       86 2023-02-10 06:15:39.000000 tailwiz-0.0.8/tailwiz/tasks/__init__.py
--rw-r--r--   0 timdai   (20656) future   (20099)     9969 2023-02-20 23:59:26.000000 tailwiz-0.0.8/tailwiz/tasks/classify.py
--rw-r--r--   0 timdai   (20656) future   (20099)     5204 2023-02-20 23:59:42.000000 tailwiz-0.0.8/tailwiz/tasks/generate.py
--rw-r--r--   0 timdai   (20656) future   (20099)     7842 2023-02-21 00:04:10.000000 tailwiz-0.0.8/tailwiz/tasks/parse.py
--rw-r--r--   0 timdai   (20656) future   (20099)      268 2023-02-10 22:08:51.000000 tailwiz-0.0.8/tailwiz/tasks/task.py
--rw-r--r--   0 timdai   (20656) future   (20099)      668 2023-02-08 08:13:52.000000 tailwiz-0.0.8/tailwiz/tasks/utils.py
-drwxr-sr-x   0 timdai   (20656) future   (20099)        0 2023-02-21 00:04:48.000000 tailwiz-0.0.8/tailwiz.egg-info/
--rw-r--r--   0 timdai   (20656) future   (20099)     6291 2023-02-21 00:04:47.000000 tailwiz-0.0.8/tailwiz.egg-info/PKG-INFO
--rw-r--r--   0 timdai   (20656) future   (20099)      384 2023-02-21 00:04:47.000000 tailwiz-0.0.8/tailwiz.egg-info/SOURCES.txt
--rw-r--r--   0 timdai   (20656) future   (20099)        1 2023-02-21 00:04:47.000000 tailwiz-0.0.8/tailwiz.egg-info/dependency_links.txt
--rw-r--r--   0 timdai   (20656) future   (20099)       68 2023-02-21 00:04:47.000000 tailwiz-0.0.8/tailwiz.egg-info/requires.txt
--rw-r--r--   0 timdai   (20656) future   (20099)        8 2023-02-21 00:04:47.000000 tailwiz-0.0.8/tailwiz.egg-info/top_level.txt
+drwxr-sr-x   0 timdai   (20656) future   (20099)        0 2023-02-23 06:55:11.000000 tailwiz-0.0.9/
+-rw-r--r--   0 timdai   (20656) future   (20099)     1068 2023-02-20 05:20:56.000000 tailwiz-0.0.9/LICENSE
+-rw-r--r--   0 timdai   (20656) future   (20099)     7085 2023-02-23 06:55:11.000000 tailwiz-0.0.9/PKG-INFO
+-rw-r--r--   0 timdai   (20656) future   (20099)     6624 2023-02-23 05:50:55.000000 tailwiz-0.0.9/README.md
+-rw-r--r--   0 timdai   (20656) future   (20099)       38 2023-02-23 06:55:11.000000 tailwiz-0.0.9/setup.cfg
+-rw-r--r--   0 timdai   (20656) future   (20099)      884 2023-02-23 06:55:04.000000 tailwiz-0.0.9/setup.py
+drwxr-sr-x   0 timdai   (20656) future   (20099)        0 2023-02-23 06:55:11.000000 tailwiz-0.0.9/tailwiz/
+-rw-r--r--   0 timdai   (20656) future   (20099)       80 2023-02-10 21:35:09.000000 tailwiz-0.0.9/tailwiz/__init__.py
+-rw-r--r--   0 timdai   (20656) future   (20099)      201 2023-02-10 21:30:41.000000 tailwiz-0.0.9/tailwiz/list_tasks.py
+drwxr-sr-x   0 timdai   (20656) future   (20099)        0 2023-02-23 06:55:11.000000 tailwiz-0.0.9/tailwiz/tasks/
+-rw-r--r--   0 timdai   (20656) future   (20099)       86 2023-02-10 06:15:39.000000 tailwiz-0.0.9/tailwiz/tasks/__init__.py
+-rw-r--r--   0 timdai   (20656) future   (20099)     7918 2023-02-23 05:26:07.000000 tailwiz-0.0.9/tailwiz/tasks/classify.py
+-rw-r--r--   0 timdai   (20656) future   (20099)     5204 2023-02-23 06:49:36.000000 tailwiz-0.0.9/tailwiz/tasks/generate.py
+-rw-r--r--   0 timdai   (20656) future   (20099)     8019 2023-02-23 06:54:09.000000 tailwiz-0.0.9/tailwiz/tasks/parse.py
+-rw-r--r--   0 timdai   (20656) future   (20099)      268 2023-02-10 22:08:51.000000 tailwiz-0.0.9/tailwiz/tasks/task.py
+-rw-r--r--   0 timdai   (20656) future   (20099)      668 2023-02-08 08:13:52.000000 tailwiz-0.0.9/tailwiz/tasks/utils.py
+drwxr-sr-x   0 timdai   (20656) future   (20099)        0 2023-02-23 06:55:11.000000 tailwiz-0.0.9/tailwiz.egg-info/
+-rw-r--r--   0 timdai   (20656) future   (20099)     7085 2023-02-23 06:55:10.000000 tailwiz-0.0.9/tailwiz.egg-info/PKG-INFO
+-rw-r--r--   0 timdai   (20656) future   (20099)      384 2023-02-23 06:55:10.000000 tailwiz-0.0.9/tailwiz.egg-info/SOURCES.txt
+-rw-r--r--   0 timdai   (20656) future   (20099)        1 2023-02-23 06:55:10.000000 tailwiz-0.0.9/tailwiz.egg-info/dependency_links.txt
+-rw-r--r--   0 timdai   (20656) future   (20099)       68 2023-02-23 06:55:10.000000 tailwiz-0.0.9/tailwiz.egg-info/requires.txt
+-rw-r--r--   0 timdai   (20656) future   (20099)        8 2023-02-23 06:55:10.000000 tailwiz-0.0.9/tailwiz.egg-info/top_level.txt
```

### Comparing `tailwiz-0.0.8/LICENSE` & `tailwiz-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tailwiz-0.0.8/PKG-INFO` & `tailwiz-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tailwiz
-Version: 0.0.8
+Version: 0.0.9
 Home-page: https://github.com/timothydai/tailwiz
 Author: Timothy Dai
 Author-email: timdai@stanford.edu
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,46 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Text Labeling AI Wizard (tailwiz)
 
 `tailwiz` is an AI-powered tool for labeling text. It has three main capabilties: classifying text (`tailwiz.classify`), parsing text given context and prompts (`tailwiz.parse`), and generating text given prompts (`tailwiz.generate`).
 
+## Quickstart
+
+Install `tailwiz` by copying and pasting the following into command line:
+
+```
+python -m pip install tailwiz
+```
+Then run the following in a Python environment for a quick example of text classification:
+
+```python
+import tailwiz
+import pandas as pd
+
+prelabeled_text = pd.DataFrame(
+    [
+        ['Love you to the moon', 'nice'],
+        ['I hate you', 'mean'],
+        ['Have a great day', 'nice'],
+    ],
+    columns=['text', 'label'],
+)
+text_to_label = pd.DataFrame(
+    ['You are the best!', 'You make me sick'],
+    columns=['text'],
+)
+results = tailwiz.classify(
+    text_to_label=text_to_label,
+    prelabeled_text=prelabeled_text,
+)
+print(results)
+```
+
 ## Installation
 
 Install `tailwiz` through `pip`:
 
 ```
 python -m pip install tailwiz
 ```
@@ -39,26 +71,35 @@
 
 #### Returns:
 - `results` : _pandas.DataFrame_. A copy of `text_to_label` with a new column, `label_from_tailwiz`, containing classification results.
 - `performance_estimate` : _Dict[str, float]_. Dictionary of metric name to metric value mappings. Included together with results in a tuple if `output_metrics` is True. Uses prelabeled_text to give an estimate of the accuracy of the classification. One vs. all metrics are given for multiclass classification.
 
 #### Example:
 
-```
->>> import tailwiz
->>> results = tailwiz.classify(
-...     text_to_label=pd.DataFrame(['You are the best!', 'You make me sick'], columns=['text']),
-...     prelabeled_text=pd.DataFrame([
-...         ['Love you to the moon', 'nice'],
-...         ['I hate you', 'mean'],
-...         ['Have a great day', 'nice']
-...     ], column=['text', 'label'])
-... )
->>> results.label_from_tailwiz.tolist()
-['nice', 'mean']
+```python
+import tailwiz
+import pandas as pd
+
+prelabeled_text = pd.DataFrame(
+    [
+        ['Love you to the moon', 'nice'],
+        ['I hate you', 'mean'],
+        ['Have a great day', 'nice'],
+    ],
+    columns=['text', 'label'],
+)
+text_to_label = pd.DataFrame(
+    ['You are the best!', 'You make me sick'],
+    columns=['text'],
+)
+results = tailwiz.classify(
+    text_to_label=text_to_label,
+    prelabeled_text=prelabeled_text,
+)
+print(results)
 ```
 
 ### <code>tailwiz.parse<i>(text_to_label, prelabeled_text=None, output_metrics=False)</i></code>
 
 Given a prompt and a context, parse the answer from the context.
 #### Parameters:
 - `text_to_label` : _pandas.DataFrame_. Data containing prompts and contexts from which answers will be parsed. Must contain a string column for the context named `context` and a string column for the prompt named `prompt`.
@@ -66,26 +107,35 @@
 - `output_metrics` : _bool, default False_. Whether to output `performance_estimate` together with results in a tuple.
 
 #### Returns:
 - `results` : _pandas.DataFrame_. A copy of `text_to_label` with a new column, `label_from_tailwiz`, containing parsed results.
 - `performance_estimate` : _Dict[str, float]_. Dictionary of metric name to metric value mappings. Included together with results in a tuple if `output_metrics` is True. Uses prelabeled_text to give an estimate of the accuracy of the parsing job.
 
 #### Example:
-```
->>> import tailwiz
->>> results = tailwiz.parse(
-...     text_to_label=pd.DataFrame([['Extract the number.', 'Figure 8']], columns=['prompt', 'context']),
-...     prelabeled_text=pd.DataFrame([
-...         ['Extract the number.', 'Noon is twelve oclock', 'twelve'],
-...         ['Extract the number.', '10 jumping jacks', '10'],
-...         ['Extract the number.', 'I have 3 eggs', '3'],
-...     ], columns=['prompt', 'context', 'label'])
-... )
->>> results.label_from_tailwiz.tolist()
-['8']
+```python
+import tailwiz
+import pandas as pd
+
+prelabeled_text = pd.DataFrame(
+    [
+        ['Extract the number.', 'Noon is twelve oclock', 'twelve'],
+        ['Extract the number.', '10 jumping jacks', '10'],
+        ['Extract the number.', 'I have 3 eggs', '3'],
+    ],
+    columns=['prompt', 'context', 'label'],
+)
+text_to_label = pd.DataFrame(
+    [['Extract the number.', 'Figure 8']],
+    columns=['prompt', 'context'],
+)
+results = tailwiz.parse(
+    text_to_label=text_to_label,
+    prelabeled_text=prelabeled_text,
+)
+print(results)
 ```
 
 
 ### <code>tailwiz.generate<i>(text_to_label, prelabeled_text=None, output_metrics=False)</i></code>
 
 Given a prompt, generate an answer.
 #### Parameters:
@@ -94,25 +144,33 @@
 - `output_metrics` : _bool, default False_. Whether to output `performance_estimate` together with results in a tuple.
 
 #### Returns:
 - `results` : _pandas.DataFrame_. A copy of `text_to_label` with a new column, `label_from_tailwiz`, containing generated results.
 - `performance_estimate` : _Dict[str, float]_. Dictionary of metric name to metric value mappings. Included together with results in a tuple if `output_metrics` is True. Uses prelabeled_text to give an estimate of the accuracy of the text generation job.
 
 #### Example:
-```
->>> import tailwiz
->>> results = tailwiz.generate(
-...     text_to_label=pd.DataFrame(['Is this sentence Happy or Sad? I am crying my eyes out.'], columns=['prompt']),
-...     prelabeled_text=pd.DataFrame([
-...         ['Is this sentence Happy or Sad? I love puppies!', 'Happy'],
-...         ['Is this sentence Happy or Sad? I do not like you at all.', 'Sad'],
-...     ], columns=['prompt', 'label'])
-... )
->>> results.label_from_tailwiz.tolist()
-['Sad']
+```python
+import tailwiz
+import pandas as pd
+
+prelabeled_text = pd.DataFrame(
+    [
+        ['Is this sentence Happy or Sad? I love puppies!', 'Happy'],
+        ['Is this sentence Happy or Sad? I do not like you at all.', 'Sad'],
+    ],
+    columns=['prompt', 'label']
+)
+text_to_label = pd.DataFrame(
+    ['Is this sentence Happy or Sad? I am crying my eyes out.'],
+    columns=['prompt']
+)
+results = tailwiz.generate(
+    text_to_label=text_to_label,
+    prelabeled_text=prelabeled_text,
+)
 ```
 
 ## Templates (Notebooks)
 
 Use these Jupyter Notebook examples as templates to help load your data and run any of the three `tailwiz` functions:
 - For an example of `tailwiz.classify`, see [`examples/classify.ipynb`](https://github.com/timothydai/tailwiz/blob/main/examples/classify.ipynb)
 - For an example of `tailwiz.parse`, see [`examples/parse.ipynb`](https://github.com/timothydai/tailwiz/blob/main/examples/parse.ipynb)
```

### Comparing `tailwiz-0.0.8/README.md` & `tailwiz-0.0.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,43 @@
 # Text Labeling AI Wizard (tailwiz)
 
 `tailwiz` is an AI-powered tool for labeling text. It has three main capabilties: classifying text (`tailwiz.classify`), parsing text given context and prompts (`tailwiz.parse`), and generating text given prompts (`tailwiz.generate`).
 
+## Quickstart
+
+Install `tailwiz` by copying and pasting the following into command line:
+
+```
+python -m pip install tailwiz
+```
+Then run the following in a Python environment for a quick example of text classification:
+
+```python
+import tailwiz
+import pandas as pd
+
+prelabeled_text = pd.DataFrame(
+    [
+        ['Love you to the moon', 'nice'],
+        ['I hate you', 'mean'],
+        ['Have a great day', 'nice'],
+    ],
+    columns=['text', 'label'],
+)
+text_to_label = pd.DataFrame(
+    ['You are the best!', 'You make me sick'],
+    columns=['text'],
+)
+results = tailwiz.classify(
+    text_to_label=text_to_label,
+    prelabeled_text=prelabeled_text,
+)
+print(results)
+```
+
 ## Installation
 
 Install `tailwiz` through `pip`:
 
 ```
 python -m pip install tailwiz
 ```
@@ -25,26 +57,35 @@
 
 #### Returns:
 - `results` : _pandas.DataFrame_. A copy of `text_to_label` with a new column, `label_from_tailwiz`, containing classification results.
 - `performance_estimate` : _Dict[str, float]_. Dictionary of metric name to metric value mappings. Included together with results in a tuple if `output_metrics` is True. Uses prelabeled_text to give an estimate of the accuracy of the classification. One vs. all metrics are given for multiclass classification.
 
 #### Example:
 
-```
->>> import tailwiz
->>> results = tailwiz.classify(
-...     text_to_label=pd.DataFrame(['You are the best!', 'You make me sick'], columns=['text']),
-...     prelabeled_text=pd.DataFrame([
-...         ['Love you to the moon', 'nice'],
-...         ['I hate you', 'mean'],
-...         ['Have a great day', 'nice']
-...     ], column=['text', 'label'])
-... )
->>> results.label_from_tailwiz.tolist()
-['nice', 'mean']
+```python
+import tailwiz
+import pandas as pd
+
+prelabeled_text = pd.DataFrame(
+    [
+        ['Love you to the moon', 'nice'],
+        ['I hate you', 'mean'],
+        ['Have a great day', 'nice'],
+    ],
+    columns=['text', 'label'],
+)
+text_to_label = pd.DataFrame(
+    ['You are the best!', 'You make me sick'],
+    columns=['text'],
+)
+results = tailwiz.classify(
+    text_to_label=text_to_label,
+    prelabeled_text=prelabeled_text,
+)
+print(results)
 ```
 
 ### <code>tailwiz.parse<i>(text_to_label, prelabeled_text=None, output_metrics=False)</i></code>
 
 Given a prompt and a context, parse the answer from the context.
 #### Parameters:
 - `text_to_label` : _pandas.DataFrame_. Data containing prompts and contexts from which answers will be parsed. Must contain a string column for the context named `context` and a string column for the prompt named `prompt`.
@@ -52,26 +93,35 @@
 - `output_metrics` : _bool, default False_. Whether to output `performance_estimate` together with results in a tuple.
 
 #### Returns:
 - `results` : _pandas.DataFrame_. A copy of `text_to_label` with a new column, `label_from_tailwiz`, containing parsed results.
 - `performance_estimate` : _Dict[str, float]_. Dictionary of metric name to metric value mappings. Included together with results in a tuple if `output_metrics` is True. Uses prelabeled_text to give an estimate of the accuracy of the parsing job.
 
 #### Example:
-```
->>> import tailwiz
->>> results = tailwiz.parse(
-...     text_to_label=pd.DataFrame([['Extract the number.', 'Figure 8']], columns=['prompt', 'context']),
-...     prelabeled_text=pd.DataFrame([
-...         ['Extract the number.', 'Noon is twelve oclock', 'twelve'],
-...         ['Extract the number.', '10 jumping jacks', '10'],
-...         ['Extract the number.', 'I have 3 eggs', '3'],
-...     ], columns=['prompt', 'context', 'label'])
-... )
->>> results.label_from_tailwiz.tolist()
-['8']
+```python
+import tailwiz
+import pandas as pd
+
+prelabeled_text = pd.DataFrame(
+    [
+        ['Extract the number.', 'Noon is twelve oclock', 'twelve'],
+        ['Extract the number.', '10 jumping jacks', '10'],
+        ['Extract the number.', 'I have 3 eggs', '3'],
+    ],
+    columns=['prompt', 'context', 'label'],
+)
+text_to_label = pd.DataFrame(
+    [['Extract the number.', 'Figure 8']],
+    columns=['prompt', 'context'],
+)
+results = tailwiz.parse(
+    text_to_label=text_to_label,
+    prelabeled_text=prelabeled_text,
+)
+print(results)
 ```
 
 
 ### <code>tailwiz.generate<i>(text_to_label, prelabeled_text=None, output_metrics=False)</i></code>
 
 Given a prompt, generate an answer.
 #### Parameters:
@@ -80,25 +130,33 @@
 - `output_metrics` : _bool, default False_. Whether to output `performance_estimate` together with results in a tuple.
 
 #### Returns:
 - `results` : _pandas.DataFrame_. A copy of `text_to_label` with a new column, `label_from_tailwiz`, containing generated results.
 - `performance_estimate` : _Dict[str, float]_. Dictionary of metric name to metric value mappings. Included together with results in a tuple if `output_metrics` is True. Uses prelabeled_text to give an estimate of the accuracy of the text generation job.
 
 #### Example:
-```
->>> import tailwiz
->>> results = tailwiz.generate(
-...     text_to_label=pd.DataFrame(['Is this sentence Happy or Sad? I am crying my eyes out.'], columns=['prompt']),
-...     prelabeled_text=pd.DataFrame([
-...         ['Is this sentence Happy or Sad? I love puppies!', 'Happy'],
-...         ['Is this sentence Happy or Sad? I do not like you at all.', 'Sad'],
-...     ], columns=['prompt', 'label'])
-... )
->>> results.label_from_tailwiz.tolist()
-['Sad']
+```python
+import tailwiz
+import pandas as pd
+
+prelabeled_text = pd.DataFrame(
+    [
+        ['Is this sentence Happy or Sad? I love puppies!', 'Happy'],
+        ['Is this sentence Happy or Sad? I do not like you at all.', 'Sad'],
+    ],
+    columns=['prompt', 'label']
+)
+text_to_label = pd.DataFrame(
+    ['Is this sentence Happy or Sad? I am crying my eyes out.'],
+    columns=['prompt']
+)
+results = tailwiz.generate(
+    text_to_label=text_to_label,
+    prelabeled_text=prelabeled_text,
+)
 ```
 
 ## Templates (Notebooks)
 
 Use these Jupyter Notebook examples as templates to help load your data and run any of the three `tailwiz` functions:
 - For an example of `tailwiz.classify`, see [`examples/classify.ipynb`](https://github.com/timothydai/tailwiz/blob/main/examples/classify.ipynb)
 - For an example of `tailwiz.parse`, see [`examples/parse.ipynb`](https://github.com/timothydai/tailwiz/blob/main/examples/parse.ipynb)
```

### Comparing `tailwiz-0.0.8/setup.py` & `tailwiz-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='tailwiz',
-    version='0.0.8',
+    version='0.0.9',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'scikit-learn',
         'transformers',
         'evaluate',
```

### Comparing `tailwiz-0.0.8/tailwiz/tasks/classify.py` & `tailwiz-0.0.9/tailwiz/tasks/classify.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,121 +8,70 @@
 import torch
 import transformers
 
 from . import utils
 from .task import Task
 
 
-class BinaryClassificationTask(Task):
+class ClassificationTask(Task):
     def __init__(self, train, val, test):
+        train = train if train is not None else pd.DataFrame([], columns=['text', 'label'])
+        val = val if val is not None else pd.DataFrame([], columns=['text', 'label'])
         (
             self.train_embeds,
             self.train_labels,
             self.val_embeds,
             self.val_labels,
             self.test_embeds
         ) = self._load_data(train, val, test)
-        self.model = self._load_model()
 
+        self.classes = list(set(self.train_labels + self.val_labels))
+        self.train_labels = sklearn.preprocessing.label_binarize(self.train_labels, classes=self.classes).tolist()
+        if len(self.train_labels[0]) == 1:  # Quirk of label_binarize: binary cases must be expanded from a single column vector.
+            self.train_labels = [[1, 0] if x == [0] else [0, 1] for x in self.train_labels]
+        if len(self.val_labels) > 0:
+            self.val_labels = sklearn.preprocessing.label_binarize(self.val_labels, classes=self.classes).tolist()
+            if len(self.val_labels[0]) == 1:  # Quirk of label_binarize: binary cases must be expanded from a single column vector.
+                self.val_labels = [[1, 0] if x == [0] else [0, 1] for x in self.val_labels]
+
+        self.model = self._load_model()
+    
     def _load_data(self, train, val, test):
-        text = [x[0] for x in train] + [x[0] for x in val] + test  # Must embed togeter to match sequence length.
+        text = train.text.tolist() + val.text.tolist() + test.text.tolist()  # Must embed togeter to match sequence length.
 
         # Tokenize.
         tokenizer = transformers.BertTokenizer.from_pretrained('bert-base-uncased')
         token_ids = tokenizer(text, return_tensors='pt', padding=True)
         
         # Embed.
         embed_model = transformers.BertModel.from_pretrained('bert-base-uncased')
         embed_model.eval()
         with torch.no_grad():
             embeds = embed_model(**token_ids)[0]
         embeds = embeds.mean(axis=1)
 
-        return embeds[:len(train)], [x[1] for x in train], embeds[len(train):len(train) + len(val)], [x[1] for x in val], embeds[len(train) + len(val):]
-
-    def _load_model(self):
-        return linear_model.LogisticRegression(random_state=0, max_iter=1000)
-
-    def train(self):
-        self.model.fit(self.train_embeds, self.train_labels)
-
-    def evaluate(self):
-        if len(self.val_embeds) == 0:
-            return None
-
-        val_preds = self.model.predict(self.val_embeds)
-        val_probs = self.model.predict_proba(self.val_embeds)
-
-        acc = metrics.accuracy_score(self.val_labels, val_preds).item()
-        prec = metrics.precision_score(self.val_labels, val_preds, zero_division=0).item()
-        rec = metrics.recall_score(self.val_labels, val_preds, zero_division=0).item()
-        f1 = metrics.f1_score(self.val_labels, val_preds, zero_division=0).item()
-
-        fpr, tpr, _ = metrics.roc_curve(self.val_labels, val_probs[:,1])
-        auroc = metrics.auc(fpr, tpr).item()
-
-        precision, recall, _ = metrics.precision_recall_curve(self.val_labels, val_probs[:,1])
-        aupr = metrics.auc(recall, precision).item()
-
-        return {
-            'acc': acc,
-            'prec': prec,
-            'rec': rec,
-            'f1': f1,
-            'metrics@90rec': utils.metrics_at_recall(0.9, val_probs[:,1].tolist(), self.val_labels),
-            'metrics@95rec': utils.metrics_at_recall(0.95, val_probs[:,1].tolist(), self.val_labels),
-            'metrics@99rec': utils.metrics_at_recall(0.99, val_probs[:,1].tolist(), self.val_labels),
-            'auroc': auroc,
-            'aupr': aupr,
-        }
-
-    def predict(self):
-        return self.model.predict(self.test_embeds).tolist()
-
-
-class MulticlassClassificationTask(BinaryClassificationTask):
-    def __init__(self, train, val, test):
-        (
-            self.train_embeds,
-            self.train_labels,
-            self.val_embeds,
-            self.val_labels,
-            self.test_embeds
-        ) = self._load_data(train, val, test)
-
-        self.classes = list(set(self.train_labels + self.val_labels))
-        self.train_labels = sklearn.preprocessing.label_binarize(self.train_labels, classes=self.classes).tolist()
-        if len(self.val_labels) > 0:
-            self.val_labels = sklearn.preprocessing.label_binarize(self.val_labels, classes=self.classes).tolist()
-
-        self.model = self._load_model()
-    
-    def _load_data(self, train, val, test):
-        return super()._load_data(train, val, test)
+        return embeds[:len(train)], train.label.tolist(), embeds[len(train):len(train) + len(val)], val.label.tolist(), embeds[len(train) + len(val):]
 
     def _load_model(self):
         return multiclass.OneVsRestClassifier(linear_model.LogisticRegression(random_state=0, max_iter=1000))
     
     def train(self):
-        return super().train()
+        self.model.fit(self.train_embeds, self.train_labels)
 
     def evaluate(self):
         if len(self.val_embeds) == 0:
             return None
 
         val_preds = self.model.predict(self.val_embeds)
         val_probs = self.model.predict_proba(self.val_embeds)
 
         accs = {}
         precs = {}
         recs = {}
         f1s = {}
-        metrics_at_90rec = {}
-        metrics_at_95rec = {}
-        metrics_at_99rec = {}
         aurocs = {}
         auprs = {}
 
         # Get one-vs-all classification metrics for each class.
         for i, class_name in enumerate(self.classes):
             class_bin = [0 for _ in range(len(self.classes))]
             class_bin[i] = 1
@@ -130,49 +79,46 @@
             labels_bin = [1 if j == class_bin else 0 for j in self.val_labels]
             preds_bin = [1 if j == class_bin else 0 for j in val_preds.tolist()]
 
             accs[class_name] = metrics.accuracy_score(labels_bin, preds_bin).item()
             precs[class_name] = metrics.precision_score(labels_bin, preds_bin, zero_division=0).item()
             recs[class_name] = metrics.recall_score(labels_bin, preds_bin, zero_division=0).item()
             f1s[class_name] = metrics.f1_score(labels_bin, preds_bin, zero_division=0).item()
-            metrics_at_90rec[class_name] = utils.metrics_at_recall(0.9, val_probs[:, i].tolist(), labels_bin)
-            metrics_at_95rec[class_name] = utils.metrics_at_recall(0.95, val_probs[:, i].tolist(), labels_bin)
-            metrics_at_99rec[class_name] = utils.metrics_at_recall(0.99, val_probs[:, i].tolist(), labels_bin)
-
 
             fpr, tpr, _ = metrics.roc_curve(labels_bin, val_probs[:,i])
             aurocs[class_name] = metrics.auc(fpr, tpr).item()
 
             precision, recall, _ = metrics.precision_recall_curve(labels_bin, val_probs[:,i])
             auprs[class_name] = metrics.auc(recall, precision).item()
 
         return {
             'acc': accs,
             'prec': precs,
             'rec': recs,
             'f1': f1s,
-            'metrics@90rec': metrics_at_90rec,
-            'metrics@95rec': metrics_at_95rec,
-            'metrics@99rec': metrics_at_99rec,
             'auroc': aurocs,
             'aupr': auprs,
         }
     
     def predict(self):
         predictions = self.model.predict(self.test_embeds)
         out_predictions = []
         for i in range(len(predictions)):
             class_i = np.argmax(predictions[i])
             out_predictions.append(self.classes[class_i])
         return out_predictions
 
 
-class KMeansClassificationTask(BinaryClassificationTask):
+class KMeansClassificationTask(ClassificationTask):
     def __init__(self, test):
-        (_, _, _, _, self.test_embeds) = self._load_data([], [], test)
+        (_, _, _, _, self.test_embeds) = self._load_data(
+            pd.DataFrame([], columns=['text', 'label']),
+            pd.DataFrame([], columns=['text', 'label']),
+            test
+        )
         self.model = self._load_model()
     
     def _load_data(self, train, val, test):
         return super()._load_data(train, val, test)
 
     def _load_model(self):
         return cluster.KMeans(n_clusters=2, random_state=0, max_iter=1000)
@@ -193,50 +139,45 @@
     assert isinstance(text_to_label, pd.DataFrame), 'Make sure you are passing in pandas DataFrames.'
     assert 'text' in text_to_label.columns, 'Make sure the text column in your pandas DataFrame is named "text".'
 
     if prelabeled_text is not None:
         assert isinstance(prelabeled_text, pd.DataFrame), 'Make sure you are passing in pandas DataFrames.'
         assert 'text' in prelabeled_text.columns and 'label' in prelabeled_text.columns, \
             'Make sure the text column in your pandas DataFrame is named "text" and the label column is named "label"'
-        prelabeled_text = list(zip(prelabeled_text.text.tolist(), prelabeled_text.label.tolist()))
 
     if output_metrics:
         assert prelabeled_text is not None, 'In order to output an estimate of performance with output_metrics, prelabeled_text must be provided.'
 
     # Perform KMeans if no training data is given.
     if prelabeled_text is None:
-        task = KMeansClassificationTask(text_to_label.text.tolist())
+        task = KMeansClassificationTask(text_to_label)
         task.train()
         pred_results = task.predict()
         results = text_to_label.copy()
         results['label_from_tailwiz'] = pred_results
         return results
 
     if len(prelabeled_text) < 3:
         raise ValueError('prelabeled_text has too few examples. At least 3 are required.')
 
-    num_unique_classes = len(set([x[1] for x in prelabeled_text]))
+    num_unique_classes = len(prelabeled_text.label.unique())
     if num_unique_classes <= 1:
         raise ValueError('prelabeled_text contains examples from just one class. Examples from at least 2 classes are required.')
-    elif num_unique_classes == 2:
-        task = BinaryClassificationTask
-    else:
-        task = MulticlassClassificationTask
 
     # Try 10 times to get a proper split. Sometimes, a split will cause all training examples to be
     # in the same class, which will error.
     classify_task_out = None
     split_attempt = 0
     while split_attempt < 10 and classify_task_out is None:
         train, val = sklearn.model_selection.train_test_split(prelabeled_text, test_size=0.2)
-        num_unique_classes_in_train = len(set([x[1] for x in train]))
+        num_unique_classes_in_train = len(train.label.unique())
         if num_unique_classes_in_train < 2:
             split_attempt += 1
             continue
-        classify_task_out = task(train, val, text_to_label.text.tolist())
+        classify_task_out = ClassificationTask(train, val, text_to_label)
         classify_task_out.train()
     
     if classify_task_out is None:
         raise ValueError('''The provided prelabeled_text examples were not diverse enough to estimate performance.
         Try balancing your prelabeled_text examples by adding more examples of each class.''')
     
     pred_results = classify_task_out.predict()
```

### Comparing `tailwiz-0.0.8/tailwiz/tasks/generate.py` & `tailwiz-0.0.9/tailwiz/tasks/generate.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                 return len(self.data['input_ids'])
             
             def __getitem__(self, index):
                 return {k: self.data[k][index] for k in self.data.keys()}
 
         args = transformers.Seq2SeqTrainingArguments(
             'cache/flan-t5',
-            num_train_epochs=15,
+            num_train_epochs=10,
             evaluation_strategy='epoch',
             save_strategy='epoch',
             load_best_model_at_end=True,
             predict_with_generate=True,
             metric_for_best_model='eval_loss',
             logging_steps=1,
         )
```

### Comparing `tailwiz-0.0.8/tailwiz/tasks/parse.py` & `tailwiz-0.0.9/tailwiz/tasks/parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,46 +25,53 @@
         
         val_tokens = None if val is None else self.tokenizer(val.prompt.tolist(), val.context.tolist(), val.label.tolist(), padding=True, return_tensors='pt')
 
         test_tokens = self.tokenizer(test.prompt.tolist(), test.context.tolist(), padding=True, return_tensors='pt')
 
         # Helper function that finds the start and end positions of the label within the context.
         # By default sets the start and end positions to the first occurrence of the label.
-        def get_target_start_end_pos(tokens):
+        def get_target_start_end_pos(tokens, contexts, labels):
             target_start_pos = []
             target_end_pos = []
-            for i, (text_tokenized, label_tokenized) in enumerate(zip(tokens['input_ids'], tokens['labels'])):
+            for i, (text_tokenized, label_tokenized, context, label) in enumerate(zip(tokens['input_ids'], tokens['labels'], contexts, labels)):
                 if label_tokenized[0] == 101 and label_tokenized[1] == 102:
                     target_start_pos.append(0)
                     target_end_pos.append(0)
                 else:
                     label_tokenized_nopad = label_tokenized[label_tokenized.nonzero()].squeeze()
                     label_tokenized_nospectoks = label_tokenized_nopad[1:-1]
 
                     for j in range(len(text_tokenized) - len(label_tokenized_nospectoks)):  # Search from start for label
                         if (text_tokenized[j:j+len(label_tokenized_nospectoks)] == label_tokenized_nospectoks).all():
                             target_start_pos.append(j)
                             target_end_pos.append(j+len(label_tokenized_nospectoks))
                             break
                 if len(target_start_pos) != i + 1:
-                    raise ValueError('''We could not find the label in the context for one of your provided prelabeled_text examples.
-                        Either: (A) only include labels where the label is extracted exactly from the context, or (B) use the generate()
-                        function, which does not require the labels do be found in the context.''')
+                    raise ValueError(f'''We could not find the label:
+                        
+                        {label}
+
+in the context:
+                        
+                        {context}
+
+Either: (A) only include labels where the label is extracted exactly from the context as whole words, or (B) use the generate()
+function, which does not require the labels do be found in the context.''')
             target_start_pos = torch.tensor(target_start_pos)
             target_end_pos = torch.tensor(target_end_pos)
             return target_start_pos, target_end_pos
 
         if train_tokens is not None:
-            train_target_start_pos, train_target_end_pos = get_target_start_end_pos(train_tokens)
+            train_target_start_pos, train_target_end_pos = get_target_start_end_pos(train_tokens, train.context.tolist(), train.label.tolist())
             train_tokens['start_positions'] = train_target_start_pos
             train_tokens['end_positions'] =  train_target_end_pos
             train_tokens = {k:v for k, v in train_tokens.items() if k != 'labels'}
 
         if val_tokens is not None:
-            val_target_start_pos, val_target_end_pos = get_target_start_end_pos(val_tokens)
+            val_target_start_pos, val_target_end_pos = get_target_start_end_pos(val_tokens, val.context.tolist(), val.label.tolist())
             val_tokens['start_positions'] = val_target_start_pos
             val_tokens['end_positions'] =  val_target_end_pos
             val_tokens = {k:v for k, v in val_tokens.items() if k != 'labels'}
 
         return train_tokens, val_tokens, test_tokens
 
     def _load_model(self):
@@ -86,15 +93,15 @@
                 return len(self.data['input_ids'])
             
             def __getitem__(self, index):
                 return {k: self.data[k][index] for k in self.data.keys()}
 
         args = transformers.TrainingArguments(
             'cache/bert-qa',
-            num_train_epochs=15,
+            num_train_epochs=10,
             evaluation_strategy='epoch',
             save_strategy='epoch',
             load_best_model_at_end=True,
             metric_for_best_model='eval_loss',
             logging_steps=1,
         )
         trainer = transformers.Trainer(
```

### Comparing `tailwiz-0.0.8/tailwiz/tasks/utils.py` & `tailwiz-0.0.9/tailwiz/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `tailwiz-0.0.8/tailwiz.egg-info/PKG-INFO` & `tailwiz-0.0.9/tailwiz.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tailwiz
-Version: 0.0.8
+Version: 0.0.9
 Home-page: https://github.com/timothydai/tailwiz
 Author: Timothy Dai
 Author-email: timdai@stanford.edu
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,46 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Text Labeling AI Wizard (tailwiz)
 
 `tailwiz` is an AI-powered tool for labeling text. It has three main capabilties: classifying text (`tailwiz.classify`), parsing text given context and prompts (`tailwiz.parse`), and generating text given prompts (`tailwiz.generate`).
 
+## Quickstart
+
+Install `tailwiz` by copying and pasting the following into command line:
+
+```
+python -m pip install tailwiz
+```
+Then run the following in a Python environment for a quick example of text classification:
+
+```python
+import tailwiz
+import pandas as pd
+
+prelabeled_text = pd.DataFrame(
+    [
+        ['Love you to the moon', 'nice'],
+        ['I hate you', 'mean'],
+        ['Have a great day', 'nice'],
+    ],
+    columns=['text', 'label'],
+)
+text_to_label = pd.DataFrame(
+    ['You are the best!', 'You make me sick'],
+    columns=['text'],
+)
+results = tailwiz.classify(
+    text_to_label=text_to_label,
+    prelabeled_text=prelabeled_text,
+)
+print(results)
+```
+
 ## Installation
 
 Install `tailwiz` through `pip`:
 
 ```
 python -m pip install tailwiz
 ```
@@ -39,26 +71,35 @@
 
 #### Returns:
 - `results` : _pandas.DataFrame_. A copy of `text_to_label` with a new column, `label_from_tailwiz`, containing classification results.
 - `performance_estimate` : _Dict[str, float]_. Dictionary of metric name to metric value mappings. Included together with results in a tuple if `output_metrics` is True. Uses prelabeled_text to give an estimate of the accuracy of the classification. One vs. all metrics are given for multiclass classification.
 
 #### Example:
 
-```
->>> import tailwiz
->>> results = tailwiz.classify(
-...     text_to_label=pd.DataFrame(['You are the best!', 'You make me sick'], columns=['text']),
-...     prelabeled_text=pd.DataFrame([
-...         ['Love you to the moon', 'nice'],
-...         ['I hate you', 'mean'],
-...         ['Have a great day', 'nice']
-...     ], column=['text', 'label'])
-... )
->>> results.label_from_tailwiz.tolist()
-['nice', 'mean']
+```python
+import tailwiz
+import pandas as pd
+
+prelabeled_text = pd.DataFrame(
+    [
+        ['Love you to the moon', 'nice'],
+        ['I hate you', 'mean'],
+        ['Have a great day', 'nice'],
+    ],
+    columns=['text', 'label'],
+)
+text_to_label = pd.DataFrame(
+    ['You are the best!', 'You make me sick'],
+    columns=['text'],
+)
+results = tailwiz.classify(
+    text_to_label=text_to_label,
+    prelabeled_text=prelabeled_text,
+)
+print(results)
 ```
 
 ### <code>tailwiz.parse<i>(text_to_label, prelabeled_text=None, output_metrics=False)</i></code>
 
 Given a prompt and a context, parse the answer from the context.
 #### Parameters:
 - `text_to_label` : _pandas.DataFrame_. Data containing prompts and contexts from which answers will be parsed. Must contain a string column for the context named `context` and a string column for the prompt named `prompt`.
@@ -66,26 +107,35 @@
 - `output_metrics` : _bool, default False_. Whether to output `performance_estimate` together with results in a tuple.
 
 #### Returns:
 - `results` : _pandas.DataFrame_. A copy of `text_to_label` with a new column, `label_from_tailwiz`, containing parsed results.
 - `performance_estimate` : _Dict[str, float]_. Dictionary of metric name to metric value mappings. Included together with results in a tuple if `output_metrics` is True. Uses prelabeled_text to give an estimate of the accuracy of the parsing job.
 
 #### Example:
-```
->>> import tailwiz
->>> results = tailwiz.parse(
-...     text_to_label=pd.DataFrame([['Extract the number.', 'Figure 8']], columns=['prompt', 'context']),
-...     prelabeled_text=pd.DataFrame([
-...         ['Extract the number.', 'Noon is twelve oclock', 'twelve'],
-...         ['Extract the number.', '10 jumping jacks', '10'],
-...         ['Extract the number.', 'I have 3 eggs', '3'],
-...     ], columns=['prompt', 'context', 'label'])
-... )
->>> results.label_from_tailwiz.tolist()
-['8']
+```python
+import tailwiz
+import pandas as pd
+
+prelabeled_text = pd.DataFrame(
+    [
+        ['Extract the number.', 'Noon is twelve oclock', 'twelve'],
+        ['Extract the number.', '10 jumping jacks', '10'],
+        ['Extract the number.', 'I have 3 eggs', '3'],
+    ],
+    columns=['prompt', 'context', 'label'],
+)
+text_to_label = pd.DataFrame(
+    [['Extract the number.', 'Figure 8']],
+    columns=['prompt', 'context'],
+)
+results = tailwiz.parse(
+    text_to_label=text_to_label,
+    prelabeled_text=prelabeled_text,
+)
+print(results)
 ```
 
 
 ### <code>tailwiz.generate<i>(text_to_label, prelabeled_text=None, output_metrics=False)</i></code>
 
 Given a prompt, generate an answer.
 #### Parameters:
@@ -94,25 +144,33 @@
 - `output_metrics` : _bool, default False_. Whether to output `performance_estimate` together with results in a tuple.
 
 #### Returns:
 - `results` : _pandas.DataFrame_. A copy of `text_to_label` with a new column, `label_from_tailwiz`, containing generated results.
 - `performance_estimate` : _Dict[str, float]_. Dictionary of metric name to metric value mappings. Included together with results in a tuple if `output_metrics` is True. Uses prelabeled_text to give an estimate of the accuracy of the text generation job.
 
 #### Example:
-```
->>> import tailwiz
->>> results = tailwiz.generate(
-...     text_to_label=pd.DataFrame(['Is this sentence Happy or Sad? I am crying my eyes out.'], columns=['prompt']),
-...     prelabeled_text=pd.DataFrame([
-...         ['Is this sentence Happy or Sad? I love puppies!', 'Happy'],
-...         ['Is this sentence Happy or Sad? I do not like you at all.', 'Sad'],
-...     ], columns=['prompt', 'label'])
-... )
->>> results.label_from_tailwiz.tolist()
-['Sad']
+```python
+import tailwiz
+import pandas as pd
+
+prelabeled_text = pd.DataFrame(
+    [
+        ['Is this sentence Happy or Sad? I love puppies!', 'Happy'],
+        ['Is this sentence Happy or Sad? I do not like you at all.', 'Sad'],
+    ],
+    columns=['prompt', 'label']
+)
+text_to_label = pd.DataFrame(
+    ['Is this sentence Happy or Sad? I am crying my eyes out.'],
+    columns=['prompt']
+)
+results = tailwiz.generate(
+    text_to_label=text_to_label,
+    prelabeled_text=prelabeled_text,
+)
 ```
 
 ## Templates (Notebooks)
 
 Use these Jupyter Notebook examples as templates to help load your data and run any of the three `tailwiz` functions:
 - For an example of `tailwiz.classify`, see [`examples/classify.ipynb`](https://github.com/timothydai/tailwiz/blob/main/examples/classify.ipynb)
 - For an example of `tailwiz.parse`, see [`examples/parse.ipynb`](https://github.com/timothydai/tailwiz/blob/main/examples/parse.ipynb)
```

