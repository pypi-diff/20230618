# Comparing `tmp/classy_classification-0.6.2.tar.gz` & `tmp/classy_classification-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classy_classification-0.6.2.tar", max compression
+gzip compressed data, was "classy_classification-0.6.3.tar", max compression
```

## Comparing `classy_classification-0.6.2.tar` & `classy_classification-0.6.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1073 2023-02-15 16:10:38.671376 classy_classification-0.6.2/LICENSE
--rw-r--r--   0        0        0    10834 2023-02-15 16:10:38.671376 classy_classification-0.6.2/README.md
--rw-r--r--   0        0        0     2583 2023-02-15 16:10:38.671376 classy_classification-0.6.2/classy_classification/__init__.py
--rw-r--r--   0        0        0        0 2023-02-15 16:10:38.671376 classy_classification-0.6.2/classy_classification/classifiers/__init__.py
--rw-r--r--   0        0        0    10313 2023-02-15 16:10:38.671376 classy_classification-0.6.2/classy_classification/classifiers/classy_skeleton.py
--rw-r--r--   0        0        0     9555 2023-02-15 16:10:38.671376 classy_classification-0.6.2/classy_classification/classifiers/classy_spacy.py
--rw-r--r--   0        0        0     2070 2023-02-15 16:10:38.671376 classy_classification-0.6.2/classy_classification/classifiers/classy_standalone.py
--rw-r--r--   0        0        0        0 2023-02-15 16:10:38.671376 classy_classification-0.6.2/classy_classification/examples/__init__.py
--rw-r--r--   0        0        0     2324 2023-02-15 16:10:38.671376 classy_classification-0.6.2/classy_classification/examples/data.py
--rw-r--r--   0        0        0      230 2023-02-15 16:10:38.675376 classy_classification-0.6.2/classy_classification/examples/individual_transformer.py
--rw-r--r--   0        0        0      339 2023-02-15 16:10:38.675376 classy_classification-0.6.2/classy_classification/examples/spacy_few_shot_external.py
--rw-r--r--   0        0        0      368 2023-02-15 16:10:38.675376 classy_classification-0.6.2/classy_classification/examples/spacy_internal_embeddings.py
--rw-r--r--   0        0        0      372 2023-02-15 16:10:38.675376 classy_classification-0.6.2/classy_classification/examples/spacy_zero_shot_external.py
--rw-r--r--   0        0        0     2089 2023-02-15 16:10:38.675376 classy_classification-0.6.2/pyproject.toml
--rw-r--r--   0        0        0    12627 1970-01-01 00:00:00.000000 classy_classification-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-18 12:54:34.636812 classy_classification-0.6.3/LICENSE
+-rw-r--r--   0        0        0    10731 2023-06-18 12:54:34.636812 classy_classification-0.6.3/README.md
+-rw-r--r--   0        0        0     2583 2023-06-18 12:54:34.636812 classy_classification-0.6.3/classy_classification/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-18 12:54:34.636812 classy_classification-0.6.3/classy_classification/classifiers/__init__.py
+-rw-r--r--   0        0        0    10545 2023-06-18 12:54:34.636812 classy_classification-0.6.3/classy_classification/classifiers/classy_skeleton.py
+-rw-r--r--   0        0        0     9555 2023-06-18 12:54:34.636812 classy_classification-0.6.3/classy_classification/classifiers/classy_spacy.py
+-rw-r--r--   0        0        0     2274 2023-06-18 12:54:34.636812 classy_classification-0.6.3/classy_classification/classifiers/classy_standalone.py
+-rw-r--r--   0        0        0        0 2023-06-18 12:54:34.636812 classy_classification-0.6.3/classy_classification/examples/__init__.py
+-rw-r--r--   0        0        0     2324 2023-06-18 12:54:34.636812 classy_classification-0.6.3/classy_classification/examples/data.py
+-rw-r--r--   0        0        0      230 2023-06-18 12:54:34.636812 classy_classification-0.6.3/classy_classification/examples/individual_transformer.py
+-rw-r--r--   0        0        0      339 2023-06-18 12:54:34.636812 classy_classification-0.6.3/classy_classification/examples/spacy_few_shot_external.py
+-rw-r--r--   0        0        0      368 2023-06-18 12:54:34.636812 classy_classification-0.6.3/classy_classification/examples/spacy_internal_embeddings.py
+-rw-r--r--   0        0        0      372 2023-06-18 12:54:34.636812 classy_classification-0.6.3/classy_classification/examples/spacy_zero_shot_external.py
+-rw-r--r--   0        0        0     2051 2023-06-18 12:54:34.640812 classy_classification-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0    12322 1970-01-01 00:00:00.000000 classy_classification-0.6.3/PKG-INFO
```

### Comparing `classy_classification-0.6.2/LICENSE` & `classy_classification-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `classy_classification-0.6.2/README.md` & `classy_classification-0.6.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 # Classy Classification
-Have you every struggled with needing a [Spacy TextCategorizer](https://spacy.io/api/textcategorizer) but didn't have the time to train one from scratch? Classy Classification is the way to go! For few-shot classification using [sentence-transformers](https://github.com/UKPLab/sentence-transformers) or [spaCy models](https://spacy.io/usage/models), provide a dictionary with labels and examples, or just provide a list of labels for zero shot-classification with [Hugginface zero-shot classifiers](https://huggingface.co/models?pipeline_tag=zero-shot-classification).
+Have you ever struggled with needing a [Spacy TextCategorizer](https://spacy.io/api/textcategorizer) but didn't have the time to train one from scratch? Classy Classification is the way to go! For few-shot classification using [sentence-transformers](https://github.com/UKPLab/sentence-transformers) or [spaCy models](https://spacy.io/usage/models), provide a dictionary with labels and examples, or just provide a list of labels for zero shot-classification with [Hugginface zero-shot classifiers](https://huggingface.co/models?pipeline_tag=zero-shot-classification).
 
 [![Current Release Version](https://img.shields.io/github/release/pandora-intelligence/classy-classification.svg?style=flat-square&logo=github)](https://github.com/pandora-intelligence/classy-classification/releases)
 [![pypi Version](https://img.shields.io/pypi/v/classy-classification.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/classy-classification/)
 [![PyPi downloads](https://static.pepy.tech/personalized-badge/classy-classification?period=total&units=international_system&left_color=grey&right_color=orange&left_text=pip%20downloads)](https://pypi.org/project/classy-classification/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
 
 # Install
 ``` pip install classy-classification```
 
-or install with faster inference using onnx.
+Or, install with faster inference using ONNX.
 
 ``` pip install classy-classification[onnx]```
 
 ## ONNX issues
 
 ### pickling
 
 ONNX does show some issues when pickling the data.
 ### M1
+
 Some [installation issues](https://github.com/onnx/onnx/issues/3129) might occur, which can be fixed by these commands.
 
 ```
 brew install cmake
 brew install protobuf
 pip3 install onnx --no-use-pep517
 ```
 
 # Quickstart
 ## SpaCy embeddings
 ```python
 import spacy
 import classy_classification
+# or import standalon
+from classy_classification import ClassyClassifier
 
 data = {
     "furniture": ["This text is about chairs.",
                "Couches, benches and televisions.",
                "I really need to get a new sofa."],
     "kitchen": ["There also exist things like fridges.",
                 "I hope to be getting a new stove today.",
@@ -51,15 +54,15 @@
     }
 )
 
 print(nlp("I am looking for kitchen appliances.")._.cats)
 
 # Output:
 #
-# [{"label": "furniture", "score": 0.21}, {"label": "kitchen", "score": 0.79}]
+# [{"furniture" : 0.21}, {"kitchen": 0.79}]
 ```
 ### Sentence level classification
 ```python
 import spacy
 import classy_classification
 
 data = {
@@ -80,15 +83,15 @@
     }
 )
 
 print(nlp("I am looking for kitchen appliances. And I love doing so.").sents[0]._.cats)
 
 # Output:
 #
-# [{"label": "furniture", "score": 0.21}, {"label": "kitchen", "score": 0.79}]
+# [[{"furniture" : 0.21}, {"kitchen": 0.79}]
 ```
 ### Define random seed and verbosity
 ```python
 
 nlp.add_pipe(
     "text_categorizer",
     config={
@@ -134,15 +137,15 @@
     }
 )
 
 print(nlp("I am looking for furniture and kitchen equipment.")._.cats)
 
 # Output:
 #
-# [{"label": "furniture", "score": 0.92}, {"label": "kitchen", "score": 0.91}]
+# [{"furniture": 0.92}, {"kitchen": 0.91}]
 ```
 ### Outlier detection
 Sometimes it is worth to be able to do outlier detection or binary classification. This can either be approached using
 a binary training dataset, however, I have also implemented support for a `OneClassSVM` for [outlier detection using a single label](https://scikit-learn.org/stable/modules/generated/sklearn.svm.OneClassSVM.html). Not that this method does not return probabilities, but that the data is formatted like label-score value pair to ensure uniformity.
 
 Approach 1:
 ```python
@@ -221,15 +224,15 @@
     }
 )
 
 print(nlp("I am looking for kitchen appliances.")._.cats)
 
 # Output:
 #
-# [{"label": "furniture", "score": 0.21}, {"label": "kitchen", "score": 0.79}]
+# [{"furniture": 0.21}, {"kitchen": 0.79}]
 ```
 ## Hugginface zero-shot classifiers
 ```python
 import spacy
 import classy_classification
 
 data = ["furniture", "kitchen"]
@@ -245,15 +248,15 @@
     }
 )
 
 print(nlp("I am looking for kitchen appliances.")._.cats)
 
 # Output:
 #
-# [{"label": "furniture", "score": 0.21}, {"label": "kitchen", "score": 0.79}]
+# [{"furniture": 0.21}, {"kitchen": 0.79}]
 ```
 # Credits
 ## Inspiration Drawn From
 [Huggingface](https://huggingface.co/) does offer some nice models for few/zero-shot classification, but these are not tailored to multi-lingual approaches. Rasa NLU has [a nice approach](https://rasa.com/blog/rasa-nlu-in-depth-part-1-intent-classification/) for this, but its too embedded in their codebase for easy usage outside of Rasa/chatbots. Additionally, it made sense to integrate [sentence-transformers](https://github.com/UKPLab/sentence-transformers) and [Hugginface zero-shot](https://huggingface.co/models?pipeline_tag=zero-shot-classification), instead of default [word embeddings](https://arxiv.org/abs/1301.3781). Finally, I decided to integrate with Spacy, since training a custom [Spacy TextCategorizer](https://spacy.io/api/textcategorizer) seems like a lot of hassle if you want something quick and dirty.
 
 - [Scikit-learn](https://github.com/scikit-learn/scikit-learn)
 - [Rasa NLU](https://github.com/RasaHQ/rasa)
```

### Comparing `classy_classification-0.6.2/classy_classification/__init__.py` & `classy_classification-0.6.3/classy_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `classy_classification-0.6.2/classy_classification/classifiers/classy_skeleton.py` & `classy_classification-0.6.3/classy_classification/classifiers/classy_skeleton.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import collections
 import importlib.util
 from typing import List, Union
 
 import numpy as np
 import pandas as pd
 from sklearn import preprocessing
 from sklearn.model_selection import GridSearchCV
@@ -44,17 +45,22 @@
                 example
                 {
                     "C": [1, 2, 5, 10, 20, 100],
                     "kernel": ["linear"],
                     "max_cross_validation_folds": 5
                 }.
         """
+
         self.multi_label = multi_label
 
-        self.data = data
+        if isinstance(data, dict):
+            self.data = collections.OrderedDict(sorted(data.items()))
+        elif isinstance(data, list):  # in case of zero-shot classification
+            self.data = data
+
         self.name = name
         self.nlp = nlp
         self.verbose = verbose
         self.include_doc = include_doc
         self.include_sent = include_sent
         if include_sent:
             Span.set_extension("cats", default=None, force=True)
@@ -121,15 +127,15 @@
         :type config: Union[dict, None]
         """
 
         if config is None:
             if len(self.label_list) > 1:
                 config = {
                     "C": [1, 2, 5, 10, 20, 50, 100],
-                    "kernel": ["linear"],
+                    "kernel": ["linear", "rbf", "poly", "sigmoid"],
                     "max_cross_validation_folds": 5,
                     "seed": None,
                 }
             else:
                 config = {
                     "nu": 0.1,
                     "kernel": "rbf",
```

### Comparing `classy_classification-0.6.2/classy_classification/classifiers/classy_spacy.py` & `classy_classification-0.6.3/classy_classification/classifiers/classy_spacy.py`

 * *Files identical despite different names*

### Comparing `classy_classification-0.6.2/classy_classification/classifiers/classy_standalone.py` & `classy_classification-0.6.3/classy_classification/classifiers/classy_standalone.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import collections
 from typing import List, Union
 
 from .classy_spacy import ClassyExternal, ClassySkeletonFewShot
 
 
 class ClassyStandalone(ClassyExternal):
     def __call__(self, text: str) -> dict:
@@ -55,15 +56,18 @@
                 {
                     "C": [1, 2, 5, 10, 20, 100],
                     "kernel": ["linear"],
                     "max_cross_validation_folds": 5
                 }.
         """
         self.multi_label = multi_label
-        self.data = data
+        if isinstance(data, dict):
+            self.data = collections.OrderedDict(sorted(data.items()))
+        elif isinstance(data, list):  # in case of zero-shot classification
+            self.data = data
         self.model = model
         self.device = device
         self.verbose = verbose
         self.set_embedding_model()
         self.set_training_data()
         self.set_config(config)
         self.set_classification_model()
```

### Comparing `classy_classification-0.6.2/classy_classification/examples/data.py` & `classy_classification-0.6.3/classy_classification/examples/data.py`

 * *Files identical despite different names*

### Comparing `classy_classification-0.6.2/pyproject.toml` & `classy_classification-0.6.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "classy-classification"
-version = "0.6.2"
+version = "0.6.3"
 description = "Have you every struggled with needing a Spacy TextCategorizer but didn't have the time to train one from scratch? Classy Classification is the way to go!"
 authors = ["David Berenstein <david.m.berenstein@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/davidberenstein1957/classy-classification"
 repository = "https://github.com/davidberenstein1957/classy-classification"
 documentation = "https://github.com/davidberenstein1957/classy-classification"
@@ -40,16 +40,14 @@
 flake8 = "^4.0.1"
 black = "^22.3.0"
 flake8-bugbear = "^22.3.23"
 flake8-docstrings = "^1.6.0"
 isort = "^5.10.1"
 pep8-naming = "^0.12.1"
 pre-commit = "^2.17.0"
-
-[tool.poetry.group.dev.dependencies]
 jupyterlab = "^3.5.2"
 ipython = "^8.8.0"
 jupyter = "^1.0.0"
 ipykernel = "^6.20.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `classy_classification-0.6.2/PKG-INFO` & `classy_classification-0.6.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classy-classification
-Version: 0.6.2
+Version: 0.6.3
 Summary: Have you every struggled with needing a Spacy TextCategorizer but didn't have the time to train one from scratch? Classy Classification is the way to go!
 Home-page: https://github.com/davidberenstein1957/classy-classification
 License: MIT
 Keywords: spacy,rasa,few-shot classification,nlu,sentence-transformers
 Author: David Berenstein
 Author-email: david.m.berenstein@gmail.com
 Requires-Python: >=3.8,<3.12
@@ -14,65 +14,64 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Provides-Extra: onnx
 Requires-Dist: fast-sentence-transformers (>=0.4.1,<0.5.0) ; extra == "onnx"
 Requires-Dist: pandas (>=1.4,<2.0)
 Requires-Dist: scikit-learn (>=1.0,<2.0)
 Requires-Dist: sentence-transformers (>=2.0,<3.0)
 Requires-Dist: spacy[transformers] (>=3.0,<4.0)
 Project-URL: Documentation, https://github.com/davidberenstein1957/classy-classification
 Project-URL: Repository, https://github.com/davidberenstein1957/classy-classification
 Description-Content-Type: text/markdown
 
 # Classy Classification
-Have you every struggled with needing a [Spacy TextCategorizer](https://spacy.io/api/textcategorizer) but didn't have the time to train one from scratch? Classy Classification is the way to go! For few-shot classification using [sentence-transformers](https://github.com/UKPLab/sentence-transformers) or [spaCy models](https://spacy.io/usage/models), provide a dictionary with labels and examples, or just provide a list of labels for zero shot-classification with [Hugginface zero-shot classifiers](https://huggingface.co/models?pipeline_tag=zero-shot-classification).
+Have you ever struggled with needing a [Spacy TextCategorizer](https://spacy.io/api/textcategorizer) but didn't have the time to train one from scratch? Classy Classification is the way to go! For few-shot classification using [sentence-transformers](https://github.com/UKPLab/sentence-transformers) or [spaCy models](https://spacy.io/usage/models), provide a dictionary with labels and examples, or just provide a list of labels for zero shot-classification with [Hugginface zero-shot classifiers](https://huggingface.co/models?pipeline_tag=zero-shot-classification).
 
 [![Current Release Version](https://img.shields.io/github/release/pandora-intelligence/classy-classification.svg?style=flat-square&logo=github)](https://github.com/pandora-intelligence/classy-classification/releases)
 [![pypi Version](https://img.shields.io/pypi/v/classy-classification.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/classy-classification/)
 [![PyPi downloads](https://static.pepy.tech/personalized-badge/classy-classification?period=total&units=international_system&left_color=grey&right_color=orange&left_text=pip%20downloads)](https://pypi.org/project/classy-classification/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
 
 # Install
 ``` pip install classy-classification```
 
-or install with faster inference using onnx.
+Or, install with faster inference using ONNX.
 
 ``` pip install classy-classification[onnx]```
 
 ## ONNX issues
 
 ### pickling
 
 ONNX does show some issues when pickling the data.
 ### M1
+
 Some [installation issues](https://github.com/onnx/onnx/issues/3129) might occur, which can be fixed by these commands.
 
 ```
 brew install cmake
 brew install protobuf
 pip3 install onnx --no-use-pep517
 ```
 
 # Quickstart
 ## SpaCy embeddings
 ```python
 import spacy
 import classy_classification
+# or import standalon
+from classy_classification import ClassyClassifier
 
 data = {
     "furniture": ["This text is about chairs.",
                "Couches, benches and televisions.",
                "I really need to get a new sofa."],
     "kitchen": ["There also exist things like fridges.",
                 "I hope to be getting a new stove today.",
@@ -88,15 +87,15 @@
     }
 )
 
 print(nlp("I am looking for kitchen appliances.")._.cats)
 
 # Output:
 #
-# [{"label": "furniture", "score": 0.21}, {"label": "kitchen", "score": 0.79}]
+# [{"furniture" : 0.21}, {"kitchen": 0.79}]
 ```
 ### Sentence level classification
 ```python
 import spacy
 import classy_classification
 
 data = {
@@ -117,15 +116,15 @@
     }
 )
 
 print(nlp("I am looking for kitchen appliances. And I love doing so.").sents[0]._.cats)
 
 # Output:
 #
-# [{"label": "furniture", "score": 0.21}, {"label": "kitchen", "score": 0.79}]
+# [[{"furniture" : 0.21}, {"kitchen": 0.79}]
 ```
 ### Define random seed and verbosity
 ```python
 
 nlp.add_pipe(
     "text_categorizer",
     config={
@@ -171,15 +170,15 @@
     }
 )
 
 print(nlp("I am looking for furniture and kitchen equipment.")._.cats)
 
 # Output:
 #
-# [{"label": "furniture", "score": 0.92}, {"label": "kitchen", "score": 0.91}]
+# [{"furniture": 0.92}, {"kitchen": 0.91}]
 ```
 ### Outlier detection
 Sometimes it is worth to be able to do outlier detection or binary classification. This can either be approached using
 a binary training dataset, however, I have also implemented support for a `OneClassSVM` for [outlier detection using a single label](https://scikit-learn.org/stable/modules/generated/sklearn.svm.OneClassSVM.html). Not that this method does not return probabilities, but that the data is formatted like label-score value pair to ensure uniformity.
 
 Approach 1:
 ```python
@@ -258,15 +257,15 @@
     }
 )
 
 print(nlp("I am looking for kitchen appliances.")._.cats)
 
 # Output:
 #
-# [{"label": "furniture", "score": 0.21}, {"label": "kitchen", "score": 0.79}]
+# [{"furniture": 0.21}, {"kitchen": 0.79}]
 ```
 ## Hugginface zero-shot classifiers
 ```python
 import spacy
 import classy_classification
 
 data = ["furniture", "kitchen"]
@@ -282,15 +281,15 @@
     }
 )
 
 print(nlp("I am looking for kitchen appliances.")._.cats)
 
 # Output:
 #
-# [{"label": "furniture", "score": 0.21}, {"label": "kitchen", "score": 0.79}]
+# [{"furniture": 0.21}, {"kitchen": 0.79}]
 ```
 # Credits
 ## Inspiration Drawn From
 [Huggingface](https://huggingface.co/) does offer some nice models for few/zero-shot classification, but these are not tailored to multi-lingual approaches. Rasa NLU has [a nice approach](https://rasa.com/blog/rasa-nlu-in-depth-part-1-intent-classification/) for this, but its too embedded in their codebase for easy usage outside of Rasa/chatbots. Additionally, it made sense to integrate [sentence-transformers](https://github.com/UKPLab/sentence-transformers) and [Hugginface zero-shot](https://huggingface.co/models?pipeline_tag=zero-shot-classification), instead of default [word embeddings](https://arxiv.org/abs/1301.3781). Finally, I decided to integrate with Spacy, since training a custom [Spacy TextCategorizer](https://spacy.io/api/textcategorizer) seems like a lot of hassle if you want something quick and dirty.
 
 - [Scikit-learn](https://github.com/scikit-learn/scikit-learn)
 - [Rasa NLU](https://github.com/RasaHQ/rasa)
```

