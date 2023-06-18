# Comparing `tmp/classy_classification-0.6.3.tar.gz` & `tmp/classy-classification-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classy_classification-0.6.3.tar", max compression
+gzip compressed data, was "classy-classification-0.6.4.tar", max compression
```

## Comparing `classy_classification-0.6.3.tar` & `classy-classification-0.6.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1073 2023-06-18 12:54:34.636812 classy_classification-0.6.3/LICENSE
--rw-r--r--   0        0        0    10731 2023-06-18 12:54:34.636812 classy_classification-0.6.3/README.md
--rw-r--r--   0        0        0     2583 2023-06-18 12:54:34.636812 classy_classification-0.6.3/classy_classification/__init__.py
--rw-r--r--   0        0        0        0 2023-06-18 12:54:34.636812 classy_classification-0.6.3/classy_classification/classifiers/__init__.py
--rw-r--r--   0        0        0    10545 2023-06-18 12:54:34.636812 classy_classification-0.6.3/classy_classification/classifiers/classy_skeleton.py
--rw-r--r--   0        0        0     9555 2023-06-18 12:54:34.636812 classy_classification-0.6.3/classy_classification/classifiers/classy_spacy.py
--rw-r--r--   0        0        0     2274 2023-06-18 12:54:34.636812 classy_classification-0.6.3/classy_classification/classifiers/classy_standalone.py
--rw-r--r--   0        0        0        0 2023-06-18 12:54:34.636812 classy_classification-0.6.3/classy_classification/examples/__init__.py
--rw-r--r--   0        0        0     2324 2023-06-18 12:54:34.636812 classy_classification-0.6.3/classy_classification/examples/data.py
--rw-r--r--   0        0        0      230 2023-06-18 12:54:34.636812 classy_classification-0.6.3/classy_classification/examples/individual_transformer.py
--rw-r--r--   0        0        0      339 2023-06-18 12:54:34.636812 classy_classification-0.6.3/classy_classification/examples/spacy_few_shot_external.py
--rw-r--r--   0        0        0      368 2023-06-18 12:54:34.636812 classy_classification-0.6.3/classy_classification/examples/spacy_internal_embeddings.py
--rw-r--r--   0        0        0      372 2023-06-18 12:54:34.636812 classy_classification-0.6.3/classy_classification/examples/spacy_zero_shot_external.py
--rw-r--r--   0        0        0     2051 2023-06-18 12:54:34.640812 classy_classification-0.6.3/pyproject.toml
--rw-r--r--   0        0        0    12322 1970-01-01 00:00:00.000000 classy_classification-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-11-01 08:20:25.558101 classy-classification-0.6.4/LICENSE
+-rw-r--r--   0        0        0    10731 2023-06-18 12:45:02.602513 classy-classification-0.6.4/README.md
+-rw-r--r--   0        0        0     2583 2022-12-30 07:44:33.081954 classy-classification-0.6.4/classy_classification/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-01 08:20:25.558372 classy-classification-0.6.4/classy_classification/classifiers/__init__.py
+-rw-r--r--   0        0        0    10545 2023-06-18 12:48:16.591005 classy-classification-0.6.4/classy_classification/classifiers/classy_skeleton.py
+-rw-r--r--   0        0        0     9186 2023-06-18 14:01:58.082842 classy-classification-0.6.4/classy_classification/classifiers/classy_spacy.py
+-rw-r--r--   0        0        0     2274 2023-06-18 12:48:19.711859 classy-classification-0.6.4/classy_classification/classifiers/classy_standalone.py
+-rw-r--r--   0        0        0        0 2022-11-01 08:20:25.558915 classy-classification-0.6.4/classy_classification/examples/__init__.py
+-rw-r--r--   0        0        0     2324 2023-01-14 09:24:42.022043 classy-classification-0.6.4/classy_classification/examples/data.py
+-rw-r--r--   0        0        0      230 2022-12-30 07:21:01.276435 classy-classification-0.6.4/classy_classification/examples/individual_transformer.py
+-rw-r--r--   0        0        0      339 2023-03-03 12:03:23.566908 classy-classification-0.6.4/classy_classification/examples/spacy_few_shot_external.py
+-rw-r--r--   0        0        0      368 2023-03-03 12:03:22.068037 classy-classification-0.6.4/classy_classification/examples/spacy_internal_embeddings.py
+-rw-r--r--   0        0        0      372 2023-03-03 12:03:19.152952 classy-classification-0.6.4/classy_classification/examples/spacy_zero_shot_external.py
+-rw-r--r--   0        0        0     2191 2023-06-18 13:56:56.117112 classy-classification-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0    12256 1970-01-01 00:00:00.000000 classy-classification-0.6.4/setup.py
+-rw-r--r--   0        0        0    12581 1970-01-01 00:00:00.000000 classy-classification-0.6.4/PKG-INFO
```

### Comparing `classy_classification-0.6.3/LICENSE` & `classy-classification-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `classy_classification-0.6.3/README.md` & `classy-classification-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `classy_classification-0.6.3/classy_classification/__init__.py` & `classy-classification-0.6.4/classy_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `classy_classification-0.6.3/classy_classification/classifiers/classy_skeleton.py` & `classy-classification-0.6.4/classy_classification/classifiers/classy_skeleton.py`

 * *Files identical despite different names*

### Comparing `classy_classification-0.6.3/classy_classification/classifiers/classy_spacy.py` & `classy-classification-0.6.4/classy_classification/classifiers/classy_spacy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import importlib.util
-import pathlib
 import warnings
 from typing import List, Union
 
 import numpy as np
 from spacy import util
 from spacy.tokens import Doc
 
@@ -96,15 +95,17 @@
         embeddings = []
         for doc in docs:
             if doc.has_vector:
                 embeddings.append(doc.vector)
             elif doc.has_extension("trf_data"):
                 embeddings.append(doc._.trf_data.model_output.pooler_output[0])
             else:
-                warnings.warn(f"None of the words in the text `{str(doc)}` have vectors. Returning zeros.")
+                warnings.warn(
+                    f"None of the words in the text `{str(doc)}` have vectors. Returning zeros.", stacklevel=1
+                )
                 embeddings.append(np.zeros(self.nlp.vocab.vectors_length))
         return np.array(embeddings)
 
 
 class ClassySpacyInternalFewShot(ClassySpacyInternal, ClassySkeletonFewShot):
     def __init__(self, *args, **kwargs):
         ClassySkeletonFewShot.__init__(self, *args, **kwargs)
@@ -149,38 +150,34 @@
             model (str, optional): the model name. Defaults to self.model, if no model is provided.
         """
         if model:  # update if overwritten
             self.model = model
         if device:
             self.device = device
 
-        if importlib.util.find_spec("fast-sentence-transformers") is None:
-            from transformers import pipeline
+        try:
+            from optimum.pipelines import pipeline
 
             if self.device in ["gpu", "cuda", 0]:
                 self.device = 0
             else:
                 self.device = -1
-            self.pipeline = pipeline("zero-shot-classification", model=self.model, device=self.device, top_k=None)
-        else:
-            from fast_sentence_transformers.txtai import HFOnnx
-            from fast_sentence_transformers.txtai.text import Labels
 
-            # Export model to ONNX
-            p = pathlib.Path(self.model)
-            if p.parent:
-                p.parent.mkdir(parents=True, exist_ok=True)
-            onnx = HFOnnx()
-            onnx_model = onnx(self.model, "text-classification", f"{self.model}.onnx", quantize=False)
+            self.pipeline = pipeline(
+                "zero-shot-classification", model=model, device=self.device, top_k=None, accelerator="ort"
+            )
+        except ImportError:
+            from transformers import pipeline
 
-            # Run inference and validate
             if self.device in ["gpu", "cuda", 0]:
-                self.pipeline = Labels((onnx_model, self.model), dynamic=True, gpu=True)
+                self.device = 0
             else:
-                self.pipeline = Labels((onnx_model, self.model), dynamic=True)
+                self.device = -1
+
+            self.pipeline = pipeline("zero-shot-classification", model=self.model, device=self.device, top_k=None)
 
     def set_config(self, _: dict = None):
         """Zero-shot models don't require a config"""
         pass
 
     def set_training_data(self, _: dict = None):
         """Zero-shot models don't require training data"""
```

### Comparing `classy_classification-0.6.3/classy_classification/classifiers/classy_standalone.py` & `classy-classification-0.6.4/classy_classification/classifiers/classy_standalone.py`

 * *Files identical despite different names*

### Comparing `classy_classification-0.6.3/classy_classification/examples/data.py` & `classy-classification-0.6.4/classy_classification/examples/data.py`

 * *Files identical despite different names*

### Comparing `classy_classification-0.6.3/pyproject.toml` & `classy-classification-0.6.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "classy-classification"
-version = "0.6.3"
+version = "0.6.4"
 description = "Have you every struggled with needing a Spacy TextCategorizer but didn't have the time to train one from scratch? Classy Classification is the way to go!"
 authors = ["David Berenstein <david.m.berenstein@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/davidberenstein1957/classy-classification"
 repository = "https://github.com/davidberenstein1957/classy-classification"
 documentation = "https://github.com/davidberenstein1957/classy-classification"
@@ -27,17 +27,19 @@
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 spacy = {extras = ["transformers"], version = "^3.0"}
 sentence-transformers = "^2.0"
 scikit-learn = "^1.0"
 pandas = "^1.4"
 fast-sentence-transformers = { version = "^0.4.1", optional = true }
+optimum = { version = "^1.8", optional = true,  extras = ["onnxruntime"]}
+transformers = {extras = ["torch"], version = "<4.30"}
 
 [tool.poetry.extras]
-onnx = ["fast-sentence-transformers"]
+onnx = ["fast-sentence-transformers", "optimum"]
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0.1"
 flake8 = "^4.0.1"
 black = "^22.3.0"
 flake8-bugbear = "^22.3.23"
 flake8-docstrings = "^1.6.0"
```

### Comparing `classy_classification-0.6.3/PKG-INFO` & `classy-classification-0.6.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classy-classification
-Version: 0.6.3
+Version: 0.6.4
 Summary: Have you every struggled with needing a Spacy TextCategorizer but didn't have the time to train one from scratch? Classy Classification is the way to go!
 Home-page: https://github.com/davidberenstein1957/classy-classification
 License: MIT
 Keywords: spacy,rasa,few-shot classification,nlu,sentence-transformers
 Author: David Berenstein
 Author-email: david.m.berenstein@gmail.com
 Requires-Python: >=3.8,<3.12
@@ -13,24 +13,29 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Provides-Extra: onnx
-Requires-Dist: fast-sentence-transformers (>=0.4.1,<0.5.0) ; extra == "onnx"
+Requires-Dist: fast-sentence-transformers (>=0.4.1,<0.5.0); extra == "onnx"
+Requires-Dist: optimum[onnxruntime] (>=1.8,<2.0); extra == "onnx"
 Requires-Dist: pandas (>=1.4,<2.0)
 Requires-Dist: scikit-learn (>=1.0,<2.0)
 Requires-Dist: sentence-transformers (>=2.0,<3.0)
 Requires-Dist: spacy[transformers] (>=3.0,<4.0)
+Requires-Dist: transformers[torch] (<4.30)
 Project-URL: Documentation, https://github.com/davidberenstein1957/classy-classification
 Project-URL: Repository, https://github.com/davidberenstein1957/classy-classification
 Description-Content-Type: text/markdown
 
 # Classy Classification
 Have you ever struggled with needing a [Spacy TextCategorizer](https://spacy.io/api/textcategorizer) but didn't have the time to train one from scratch? Classy Classification is the way to go! For few-shot classification using [sentence-transformers](https://github.com/UKPLab/sentence-transformers) or [spaCy models](https://spacy.io/usage/models), provide a dictionary with labels and examples, or just provide a list of labels for zero shot-classification with [Hugginface zero-shot classifiers](https://huggingface.co/models?pipeline_tag=zero-shot-classification).
```

