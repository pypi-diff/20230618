# Comparing `tmp/spacy_partial_tagger-0.9.3.tar.gz` & `tmp/spacy_partial_tagger-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy_partial_tagger-0.9.3.tar", max compression
+gzip compressed data, was "spacy_partial_tagger-0.9.4.tar", max compression
```

## Comparing `spacy_partial_tagger-0.9.3.tar` & `spacy_partial_tagger-0.9.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1065 2022-10-25 07:41:17.147394 spacy_partial_tagger-0.9.3/LICENSE
--rw-r--r--   0        0        0     3785 2022-10-25 07:41:17.147394 spacy_partial_tagger-0.9.3/README.md
--rw-r--r--   0        0        0     2513 2022-10-25 07:41:17.151394 spacy_partial_tagger-0.9.3/pyproject.toml
--rw-r--r--   0        0        0        0 2022-10-25 07:41:17.151394 spacy_partial_tagger-0.9.3/spacy_partial_tagger/__init__.py
--rw-r--r--   0        0        0     2797 2022-10-25 07:41:17.151394 spacy_partial_tagger-0.9.3/spacy_partial_tagger/aligners.py
--rw-r--r--   0        0        0     1733 2022-10-25 07:41:17.151394 spacy_partial_tagger-0.9.3/spacy_partial_tagger/label_indexers.py
--rw-r--r--   0        0        0        0 2022-10-25 07:41:17.151394 spacy_partial_tagger-0.9.3/spacy_partial_tagger/layers/__init__.py
--rw-r--r--   0        0        0     4397 2022-10-25 07:41:17.151394 spacy_partial_tagger-0.9.3/spacy_partial_tagger/layers/decoder.py
--rw-r--r--   0        0        0     3016 2022-10-25 07:41:17.151394 spacy_partial_tagger-0.9.3/spacy_partial_tagger/layers/encoder.py
--rw-r--r--   0        0        0     4363 2022-10-25 07:41:17.151394 spacy_partial_tagger-0.9.3/spacy_partial_tagger/layers/tok2vec_transformer.py
--rw-r--r--   0        0        0     1076 2022-10-25 07:41:17.151394 spacy_partial_tagger-0.9.3/spacy_partial_tagger/layers/tok2vec_wrapper.py
--rw-r--r--   0        0        0      300 2022-10-25 07:41:17.151394 spacy_partial_tagger-0.9.3/spacy_partial_tagger/layers/util.py
--rw-r--r--   0        0        0     3061 2022-10-25 07:41:17.151394 spacy_partial_tagger-0.9.3/spacy_partial_tagger/loss.py
--rw-r--r--   0        0        0     8787 2022-10-25 07:41:17.151394 spacy_partial_tagger-0.9.3/spacy_partial_tagger/pipeline.py
--rw-r--r--   0        0        0     1587 2022-10-25 07:41:17.151394 spacy_partial_tagger-0.9.3/spacy_partial_tagger/tagger.py
--rw-r--r--   0        0        0     1066 2022-10-25 07:41:17.151394 spacy_partial_tagger-0.9.3/spacy_partial_tagger/tokenizer.py
--rw-r--r--   0        0        0      796 2022-10-25 07:41:17.151394 spacy_partial_tagger-0.9.3/spacy_partial_tagger/util.py
--rw-r--r--   0        0        0     6325 1970-01-01 00:00:00.000000 spacy_partial_tagger-0.9.3/setup.py
--rw-r--r--   0        0        0     4914 1970-01-01 00:00:00.000000 spacy_partial_tagger-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-10-31 01:08:35.278848 spacy_partial_tagger-0.9.4/LICENSE
+-rw-r--r--   0        0        0     3853 2022-10-31 01:08:35.278848 spacy_partial_tagger-0.9.4/README.md
+-rw-r--r--   0        0        0     2513 2022-10-31 01:08:35.282848 spacy_partial_tagger-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-10-31 01:08:35.282848 spacy_partial_tagger-0.9.4/spacy_partial_tagger/__init__.py
+-rw-r--r--   0        0        0     2797 2022-10-31 01:08:35.282848 spacy_partial_tagger-0.9.4/spacy_partial_tagger/aligners.py
+-rw-r--r--   0        0        0     1733 2022-10-31 01:08:35.282848 spacy_partial_tagger-0.9.4/spacy_partial_tagger/label_indexers.py
+-rw-r--r--   0        0        0        0 2022-10-31 01:08:35.282848 spacy_partial_tagger-0.9.4/spacy_partial_tagger/layers/__init__.py
+-rw-r--r--   0        0        0     4397 2022-10-31 01:08:35.282848 spacy_partial_tagger-0.9.4/spacy_partial_tagger/layers/decoder.py
+-rw-r--r--   0        0        0     3016 2022-10-31 01:08:35.282848 spacy_partial_tagger-0.9.4/spacy_partial_tagger/layers/encoder.py
+-rw-r--r--   0        0        0     4363 2022-10-31 01:08:35.282848 spacy_partial_tagger-0.9.4/spacy_partial_tagger/layers/tok2vec_transformer.py
+-rw-r--r--   0        0        0     1076 2022-10-31 01:08:35.282848 spacy_partial_tagger-0.9.4/spacy_partial_tagger/layers/tok2vec_wrapper.py
+-rw-r--r--   0        0        0      300 2022-10-31 01:08:35.282848 spacy_partial_tagger-0.9.4/spacy_partial_tagger/layers/util.py
+-rw-r--r--   0        0        0     3061 2022-10-31 01:08:35.282848 spacy_partial_tagger-0.9.4/spacy_partial_tagger/loss.py
+-rw-r--r--   0        0        0     8787 2022-10-31 01:08:35.286848 spacy_partial_tagger-0.9.4/spacy_partial_tagger/pipeline.py
+-rw-r--r--   0        0        0     1587 2022-10-31 01:08:35.286848 spacy_partial_tagger-0.9.4/spacy_partial_tagger/tagger.py
+-rw-r--r--   0        0        0     1066 2022-10-31 01:08:35.286848 spacy_partial_tagger-0.9.4/spacy_partial_tagger/tokenizer.py
+-rw-r--r--   0        0        0      796 2022-10-31 01:08:35.286848 spacy_partial_tagger-0.9.4/spacy_partial_tagger/util.py
+-rw-r--r--   0        0        0     6393 1970-01-01 00:00:00.000000 spacy_partial_tagger-0.9.4/setup.py
+-rw-r--r--   0        0        0     4982 1970-01-01 00:00:00.000000 spacy_partial_tagger-0.9.4/PKG-INFO
```

### Comparing `spacy_partial_tagger-0.9.3/LICENSE` & `spacy_partial_tagger-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy_partial_tagger-0.9.3/README.md` & `spacy_partial_tagger-0.9.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # spacy-partial-tagger
 
 This is a library to build a CRF tagger for a partially annotated dataset in spaCy. You can build your own NER tagger only from dictionary. The algorithm of this tagger is based on Effland and Collins. (2021).
 
 ## Overview
 
-![The overview of spacy-partial-tagger](images/overview.png)
+![The overview of spacy-partial-tagger](https://raw.githubusercontent.com/doccano/spacy-partial-tagger/main/images/overview.png)
 
 ## Dataset Preparation
 
 Prepare spaCy binary format file. This library expects tokenization is character-based.
 For more detail about spaCy binary format, see [this page](https://spacy.io/api/data-formats#training).
 
 You can prepare your own dataset with [spaCy's entity ruler](https://spacy.io/usage/rule-based-matching#entityruler) as follows:
```

### Comparing `spacy_partial_tagger-0.9.3/pyproject.toml` & `spacy_partial_tagger-0.9.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spacy-partial-tagger"
-version = "0.9.3"
+version = "0.9.4"
 description = "Sequence Tagger for Partially Annotated Dataset in spaCy"
 authors = ["yasufumi <yasufumi.taniguchi@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/tech-sketch/spacy-partial-tagger"
 classifiers = [
     "Programming Language :: Python",
```

### Comparing `spacy_partial_tagger-0.9.3/spacy_partial_tagger/aligners.py` & `spacy_partial_tagger-0.9.4/spacy_partial_tagger/aligners.py`

 * *Files identical despite different names*

### Comparing `spacy_partial_tagger-0.9.3/spacy_partial_tagger/label_indexers.py` & `spacy_partial_tagger-0.9.4/spacy_partial_tagger/label_indexers.py`

 * *Files identical despite different names*

### Comparing `spacy_partial_tagger-0.9.3/spacy_partial_tagger/layers/decoder.py` & `spacy_partial_tagger-0.9.4/spacy_partial_tagger/layers/decoder.py`

 * *Files identical despite different names*

### Comparing `spacy_partial_tagger-0.9.3/spacy_partial_tagger/layers/encoder.py` & `spacy_partial_tagger-0.9.4/spacy_partial_tagger/layers/encoder.py`

 * *Files identical despite different names*

### Comparing `spacy_partial_tagger-0.9.3/spacy_partial_tagger/layers/tok2vec_transformer.py` & `spacy_partial_tagger-0.9.4/spacy_partial_tagger/layers/tok2vec_transformer.py`

 * *Files identical despite different names*

### Comparing `spacy_partial_tagger-0.9.3/spacy_partial_tagger/layers/tok2vec_wrapper.py` & `spacy_partial_tagger-0.9.4/spacy_partial_tagger/layers/tok2vec_wrapper.py`

 * *Files identical despite different names*

### Comparing `spacy_partial_tagger-0.9.3/spacy_partial_tagger/loss.py` & `spacy_partial_tagger-0.9.4/spacy_partial_tagger/loss.py`

 * *Files identical despite different names*

### Comparing `spacy_partial_tagger-0.9.3/spacy_partial_tagger/pipeline.py` & `spacy_partial_tagger-0.9.4/spacy_partial_tagger/pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy_partial_tagger-0.9.3/spacy_partial_tagger/tagger.py` & `spacy_partial_tagger-0.9.4/spacy_partial_tagger/tagger.py`

 * *Files identical despite different names*

### Comparing `spacy_partial_tagger-0.9.3/spacy_partial_tagger/tokenizer.py` & `spacy_partial_tagger-0.9.4/spacy_partial_tagger/tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy_partial_tagger-0.9.3/spacy_partial_tagger/util.py` & `spacy_partial_tagger-0.9.4/spacy_partial_tagger/util.py`

 * *Files identical despite different names*

### Comparing `spacy_partial_tagger-0.9.3/setup.py` & `spacy_partial_tagger-0.9.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,17 @@
  'spacy_tokenizers': ['character_tokenizer.v1 = '
                       'spacy_partial_tagger.tokenizer:create_character_tokenizer'],
  'thinc_losses': ['spacy-partial-tagger.ExpectedEntityRatioLoss.v1 = '
                   'spacy_partial_tagger.loss:configure_ExpectedEntityRatioLoss']}
 
 setup_kwargs = {
     'name': 'spacy-partial-tagger',
-    'version': '0.9.3',
+    'version': '0.9.4',
     'description': 'Sequence Tagger for Partially Annotated Dataset in spaCy',
-    'long_description': '# spacy-partial-tagger\n\nThis is a library to build a CRF tagger for a partially annotated dataset in spaCy. You can build your own NER tagger only from dictionary. The algorithm of this tagger is based on Effland and Collins. (2021).\n\n## Overview\n\n![The overview of spacy-partial-tagger](images/overview.png)\n\n## Dataset Preparation\n\nPrepare spaCy binary format file. This library expects tokenization is character-based.\nFor more detail about spaCy binary format, see [this page](https://spacy.io/api/data-formats#training).\n\nYou can prepare your own dataset with [spaCy\'s entity ruler](https://spacy.io/usage/rule-based-matching#entityruler) as follows:\n\n```py\nimport spacy\nfrom spacy.tokens import DocBin\nfrom spacy_partial_tagger.tokenizer import CharacterTokenizer\n\n\nnlp = spacy.blank("en")\nnlp.tokenizer = CharacterTokenizer(nlp.vocab)  # Use a character-based tokenizer\n\npatterns = [{"label": "LOC", "pattern": "Tokyo"}, {"label": "LOC", "pattern": "Japan"}]\nruler = nlp.add_pipe("entity_ruler")\nruler.add_patterns(patterns)\n\ndoc = nlp("Tokyo is the capital of Japan.")\n\ndoc_bin = DocBin()\ndoc_bin.add(doc)\n\n# Replace /path/to/data.spacy with your own path\ndoc_bin.to_disk("/path/to/data.spacy")\n```\n\nIn the example above, entities are extracted by character-based matching. However, in some cases, character-based matching may not be suitable (e.g., the element symbol `na` for sodium matches name). In such cases, token-based matching can be used as follows:\n\n```py\nimport spacy\nfrom spacy.tokens import DocBin\nfrom spacy_partial_tagger.tokenizer import CharacterTokenizer\n\ntext = "Selegiline - induced postural hypotension in Parkinson\'s disease: a longitudinal study on the effects of drug withdrawal."\npatterns = [\n    {"label": "Chemical", "pattern": [{"LOWER": "selegiline"}]},\n    {"label": "Disease", "pattern": [{"LOWER": "hypotension"}]},\n    {\n        "label": "Disease",\n        "pattern": [{"LOWER": "parkinson"}, {"LOWER": "\'s"}, {"LOWER": "disease"}],\n    },\n]\n\n# Add an entity ruler to the pipeline.\nnlp = spacy.blank("en")\nruler = nlp.add_pipe("entity_ruler")\nruler.add_patterns(patterns)\n\n# Extract entities from the text.\ndoc = nlp(text)\nentities = [(ent.start_char, ent.end_char, ent.label_) for ent in doc.ents]\n\n# Create a DocBin object.\nnlp = spacy.blank("en")\nnlp.tokenizer = CharacterTokenizer(nlp.vocab)\ndoc_bin = DocBin()\ndoc = nlp.make_doc(text)\ndoc.ents = [\n    doc.char_span(start, end, label=label) for start, end, label in entities\n]\ndoc_bin.add(doc)\ndoc_bin.to_disk("/path/to/data.spacy")\n```\n\n## Training\n\nTrain your model as follows:\n\n```sh\npython -m spacy train config.cfg --output outputs --paths.train /path/to/train.spacy --paths.dev /path/to/dev.spacy --gpu-id 0\n```\n\nYou could download `config.cfg` [here](https://github.com/tech-sketch/spacy-partial-tagger/blob/main/config.cfg).\nOr you could setup your own. This library would train models through spaCy. If you are not familiar with spaCy\'s config file format, please check the [documentation](https://spacy.io/usage/training#config).\n\nDon\'t forget to replace `/path/to/train.spacy` and `/path/to/dev.spacy` with your own.\n\n## Evaluation\n\nEvaluate your model as follows:\n\n```sh\npython -m spacy evaluate outputs/model-best /path/to/test.spacy --gpu-id 0\n```\n\nDon\'t forget to replace `/path/to/test.spacy` with your own.\n\n## Installation\n\n```sh\npip install spacy-partial-tagger\n```\n\nIf you use M1 Mac, you might have problems installing `fugashi`. In that case, please try `brew install mecab` before the installation.\n\n## References\n\n- Thomas Effland and Michael Collins. 2021. [Partially Supervised Named Entity Recognition via the Expected Entity Ratio Loss](https://aclanthology.org/2021.tacl-1.78/). _Transactions of the Association for Computational Linguistics_, 9:1320–1335.\n',
+    'long_description': '# spacy-partial-tagger\n\nThis is a library to build a CRF tagger for a partially annotated dataset in spaCy. You can build your own NER tagger only from dictionary. The algorithm of this tagger is based on Effland and Collins. (2021).\n\n## Overview\n\n![The overview of spacy-partial-tagger](https://raw.githubusercontent.com/doccano/spacy-partial-tagger/main/images/overview.png)\n\n## Dataset Preparation\n\nPrepare spaCy binary format file. This library expects tokenization is character-based.\nFor more detail about spaCy binary format, see [this page](https://spacy.io/api/data-formats#training).\n\nYou can prepare your own dataset with [spaCy\'s entity ruler](https://spacy.io/usage/rule-based-matching#entityruler) as follows:\n\n```py\nimport spacy\nfrom spacy.tokens import DocBin\nfrom spacy_partial_tagger.tokenizer import CharacterTokenizer\n\n\nnlp = spacy.blank("en")\nnlp.tokenizer = CharacterTokenizer(nlp.vocab)  # Use a character-based tokenizer\n\npatterns = [{"label": "LOC", "pattern": "Tokyo"}, {"label": "LOC", "pattern": "Japan"}]\nruler = nlp.add_pipe("entity_ruler")\nruler.add_patterns(patterns)\n\ndoc = nlp("Tokyo is the capital of Japan.")\n\ndoc_bin = DocBin()\ndoc_bin.add(doc)\n\n# Replace /path/to/data.spacy with your own path\ndoc_bin.to_disk("/path/to/data.spacy")\n```\n\nIn the example above, entities are extracted by character-based matching. However, in some cases, character-based matching may not be suitable (e.g., the element symbol `na` for sodium matches name). In such cases, token-based matching can be used as follows:\n\n```py\nimport spacy\nfrom spacy.tokens import DocBin\nfrom spacy_partial_tagger.tokenizer import CharacterTokenizer\n\ntext = "Selegiline - induced postural hypotension in Parkinson\'s disease: a longitudinal study on the effects of drug withdrawal."\npatterns = [\n    {"label": "Chemical", "pattern": [{"LOWER": "selegiline"}]},\n    {"label": "Disease", "pattern": [{"LOWER": "hypotension"}]},\n    {\n        "label": "Disease",\n        "pattern": [{"LOWER": "parkinson"}, {"LOWER": "\'s"}, {"LOWER": "disease"}],\n    },\n]\n\n# Add an entity ruler to the pipeline.\nnlp = spacy.blank("en")\nruler = nlp.add_pipe("entity_ruler")\nruler.add_patterns(patterns)\n\n# Extract entities from the text.\ndoc = nlp(text)\nentities = [(ent.start_char, ent.end_char, ent.label_) for ent in doc.ents]\n\n# Create a DocBin object.\nnlp = spacy.blank("en")\nnlp.tokenizer = CharacterTokenizer(nlp.vocab)\ndoc_bin = DocBin()\ndoc = nlp.make_doc(text)\ndoc.ents = [\n    doc.char_span(start, end, label=label) for start, end, label in entities\n]\ndoc_bin.add(doc)\ndoc_bin.to_disk("/path/to/data.spacy")\n```\n\n## Training\n\nTrain your model as follows:\n\n```sh\npython -m spacy train config.cfg --output outputs --paths.train /path/to/train.spacy --paths.dev /path/to/dev.spacy --gpu-id 0\n```\n\nYou could download `config.cfg` [here](https://github.com/tech-sketch/spacy-partial-tagger/blob/main/config.cfg).\nOr you could setup your own. This library would train models through spaCy. If you are not familiar with spaCy\'s config file format, please check the [documentation](https://spacy.io/usage/training#config).\n\nDon\'t forget to replace `/path/to/train.spacy` and `/path/to/dev.spacy` with your own.\n\n## Evaluation\n\nEvaluate your model as follows:\n\n```sh\npython -m spacy evaluate outputs/model-best /path/to/test.spacy --gpu-id 0\n```\n\nDon\'t forget to replace `/path/to/test.spacy` with your own.\n\n## Installation\n\n```sh\npip install spacy-partial-tagger\n```\n\nIf you use M1 Mac, you might have problems installing `fugashi`. In that case, please try `brew install mecab` before the installation.\n\n## References\n\n- Thomas Effland and Michael Collins. 2021. [Partially Supervised Named Entity Recognition via the Expected Entity Ratio Loss](https://aclanthology.org/2021.tacl-1.78/). _Transactions of the Association for Computational Linguistics_, 9:1320–1335.\n',
     'author': 'yasufumi',
     'author_email': 'yasufumi.taniguchi@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tech-sketch/spacy-partial-tagger',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `spacy_partial_tagger-0.9.3/PKG-INFO` & `spacy_partial_tagger-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-partial-tagger
-Version: 0.9.3
+Version: 0.9.4
 Summary: Sequence Tagger for Partially Annotated Dataset in spaCy
 Home-page: https://github.com/tech-sketch/spacy-partial-tagger
 License: MIT
 Author: yasufumi
 Author-email: yasufumi.taniguchi@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -27,15 +27,15 @@
 
 # spacy-partial-tagger
 
 This is a library to build a CRF tagger for a partially annotated dataset in spaCy. You can build your own NER tagger only from dictionary. The algorithm of this tagger is based on Effland and Collins. (2021).
 
 ## Overview
 
-![The overview of spacy-partial-tagger](images/overview.png)
+![The overview of spacy-partial-tagger](https://raw.githubusercontent.com/doccano/spacy-partial-tagger/main/images/overview.png)
 
 ## Dataset Preparation
 
 Prepare spaCy binary format file. This library expects tokenization is character-based.
 For more detail about spaCy binary format, see [this page](https://spacy.io/api/data-formats#training).
 
 You can prepare your own dataset with [spaCy's entity ruler](https://spacy.io/usage/rule-based-matching#entityruler) as follows:
```

