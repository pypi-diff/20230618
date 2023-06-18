# Comparing `tmp/pytorch_partial_tagger-0.1.8.tar.gz` & `tmp/pytorch_partial_tagger-0.1.9.tar.gz`

## Comparing `pytorch_partial_tagger-0.1.8.tar` & `pytorch_partial_tagger-0.1.9.tar`

### file list

```diff
@@ -1,68 +1,60 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/.DS_Store
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/cli.py
--rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/cli_head.py
--rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/cli_lora.py
--rw-r--r--   0        0        0     5245 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/cli_lora_base.py
--rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/cli_lora_base_accelerate.py
--rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/cli_lora_large.py
--rw-r--r--   0        0        0  1193604 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/entity.dev.jsonl
--rw-r--r--   0        0        0  1141566 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/entity.test.jsonl
--rw-r--r--   0        0        0  4012618 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/entity.train_r0.5_p0.9.jsonl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/log.jsonl
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/log_head.jsonl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/log_lora_base.jsonl
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/scores.json
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/.github/workflows/ci.yml
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0    84871 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/notebooks/basic.ipynb
--rw-r--r--   0        0        0  4032390 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/scirex/dev.jsonl
--rw-r--r--   0        0        0  4869030 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/scirex/test.jsonl
--rw-r--r--   0        0        0 20510651 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/scirex/train.jsonl
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/.DS_Store
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/__about__.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/matchers.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/metric.py
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/recognizer.py
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/tagger.py
--rw-r--r--   0        0        0     9713 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/training.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/utils.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/crf/.DS_Store
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/crf/__init__.py
--rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/crf/functional.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/crf/nn.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/data/.DS_Store
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/data/__init__.py
--rw-r--r--   0        0        0    15475 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/data/core.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/data/batch/__init__.py
--rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/data/batch/tag.py
--rw-r--r--   0        0        0     7951 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/data/batch/text.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/decoders/.DS_Store
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/decoders/__init__.py
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/decoders/viterbi.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/encoders/.DS_Store
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/encoders/__init__.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/encoders/base.py
--rw-r--r--   0        0        0     5144 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/encoders/transformer.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/conftest.py
--rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/helpers.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/test_matchers.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/test_metric.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/test_recognizer.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/crf/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/crf/__init__.py
--rw-r--r--   0        0        0    10350 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/crf/test_functional.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/crf/test_nn.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/data/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/data/__init__.py
--rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/data/test_core.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/data/batch/conftest.py
--rw-r--r--   0        0        0    21181 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/data/batch/test_tag.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/data/batch/test_text.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/LICENSE
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/README.md
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/docs/.readthedocs.yaml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/docs/make.bat
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/docs/source/conf.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/docs/source/index.rst
+-rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/docs/source/quick_start.md
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/docs/source/reference.rst
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/docs/source/reference/partial_tagger.crf.functional.rst
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/docs/source/reference/partial_tagger.crf.nn.rst
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/docs/source/reference/partial_tagger.crf.rst
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/docs/source/reference/partial_tagger.data.batch.tag.rst
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/docs/source/reference/partial_tagger.data.batch.text.rst
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/docs/source/reference/partial_tagger.data.rst
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/docs/source/reference/partial_tagger.decoders.rst
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/docs/source/reference/partial_tagger.encoders.rst
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/docs/source/reference/partial_tagger.recognizer.rst
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/docs/source/reference/partial_tagger.tagger.rst
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/docs/source/reference/partial_tagger.training.rst
+-rw-r--r--   0        0        0    84871 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/notebooks/basic.ipynb
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/src/partial_tagger/__about__.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/src/partial_tagger/matchers.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/src/partial_tagger/metric.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/src/partial_tagger/recognizer.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/src/partial_tagger/tagger.py
+-rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/src/partial_tagger/training.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/src/partial_tagger/utils.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/src/partial_tagger/crf/__init__.py
+-rw-r--r--   0        0        0    10065 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/src/partial_tagger/crf/functional.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/src/partial_tagger/crf/nn.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/src/partial_tagger/data/__init__.py
+-rw-r--r--   0        0        0    15491 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/src/partial_tagger/data/core.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/src/partial_tagger/data/batch/__init__.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/src/partial_tagger/data/batch/tag.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/src/partial_tagger/data/batch/text.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/src/partial_tagger/decoders/__init__.py
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/src/partial_tagger/decoders/viterbi.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/src/partial_tagger/encoders/__init__.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/src/partial_tagger/encoders/base.py
+-rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/src/partial_tagger/encoders/transformer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/tests/conftest.py
+-rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/tests/helpers.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/tests/test_matchers.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/tests/test_metric.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/tests/test_recognizer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/tests/crf/__init__.py
+-rw-r--r--   0        0        0    10350 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/tests/crf/test_functional.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/tests/crf/test_nn.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/tests/data/__init__.py
+-rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/tests/data/test_core.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/tests/data/batch/conftest.py
+-rw-r--r--   0        0        0    21181 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/tests/data/batch/test_tag.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/tests/data/batch/test_text.py
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/README.md
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4522 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.9/PKG-INFO
```

### Comparing `pytorch_partial_tagger-0.1.8/.github/workflows/ci.yml` & `pytorch_partial_tagger-0.1.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.8/.github/workflows/pypi-publish.yml` & `pytorch_partial_tagger-0.1.9/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.8/notebooks/basic.ipynb` & `pytorch_partial_tagger-0.1.9/notebooks/basic.ipynb`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.8/src/partial_tagger/metric.py` & `pytorch_partial_tagger-0.1.9/src/partial_tagger/metric.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from .data.core import CharBasedTags
+from partial_tagger.data.core import CharBasedTags
 
 
 class Metric:
     def __init__(self) -> None:
         self.__tp = 0
         self.__fp = 0
         self.__fn = 0
```

### Comparing `pytorch_partial_tagger-0.1.8/src/partial_tagger/recognizer.py` & `pytorch_partial_tagger-0.1.9/src/partial_tagger/recognizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 from collections.abc import Sequence
 
 import torch
 from torch.utils.data import DataLoader
 
-from .data import CharBasedTags, LabelSet
-from .data.batch.text import BaseTokenizer, TextBatch
-from .tagger import SequenceTagger
+from partial_tagger.data import CharBasedTags, LabelSet
+from partial_tagger.data.batch.text import BaseTokenizer, TextBatch
+from partial_tagger.tagger import SequenceTagger
 
 
 class Recognizer:
     """A recognizer which predicts character-based tags from a given text with
     a trained sequence tagger.
 
     Args:
```

### Comparing `pytorch_partial_tagger-0.1.8/src/partial_tagger/tagger.py` & `pytorch_partial_tagger-0.1.9/src/partial_tagger/tagger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import torch
 from torch.nn import Module
 
-from .crf.nn import CRF
-from .decoders import ViterbiDecoder
-from .encoders import BaseEncoder
+from partial_tagger.crf.nn import CRF
+from partial_tagger.decoders import ViterbiDecoder
+from partial_tagger.encoders import BaseEncoder
 
 
 class SequenceTagger(Module):
     """A sequence tagging model with a CRF layer.
 
     Args:
         encoder: An encoder module.
```

### Comparing `pytorch_partial_tagger-0.1.8/src/partial_tagger/training.py` & `pytorch_partial_tagger-0.1.9/src/partial_tagger/training.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 import logging
 from collections.abc import Sequence
 from logging import Logger
 
 import torch
 from torch.utils.data import DataLoader
 
-from .crf import functional as F
-from .data import CharBasedTags, LabelSet
-from .data.batch import Collator
-from .data.batch.tag import TagsBatch
-from .data.batch.text import BaseTokenizer, TextBatch
-from .decoders.viterbi import Constrainer, ViterbiDecoder
-from .encoders import BaseEncoderFactory
-from .metric import Metric
-from .recognizer import Recognizer
-from .tagger import SequenceTagger
+from partial_tagger.crf import functional as F
+from partial_tagger.data import CharBasedTags, LabelSet
+from partial_tagger.data.batch import Collator
+from partial_tagger.data.batch.tag import TagsBatch
+from partial_tagger.data.batch.text import BaseTokenizer, TextBatch
+from partial_tagger.decoders.viterbi import Constrainer, ViterbiDecoder
+from partial_tagger.encoders import BaseEncoderFactory
+from partial_tagger.metric import Metric
+from partial_tagger.recognizer import Recognizer
+from partial_tagger.tagger import SequenceTagger
 
 
 class SlantedTriangular:
     def __init__(self, max_steps: int, cut_frac: float = 0.1, ratio: int = 16):
         self.__cut_frac = cut_frac
         self.__cut = int(max_steps * cut_frac)
         self.__ratio = ratio
@@ -43,25 +43,25 @@
     entity_ratio_margin: float = 0.05,
     balancing_coefficient: int = 10,
 ) -> torch.Tensor:
     """Computes the loss proposed in Effland and Collins. '21.
 
     Args:
         log_potentials: A [batch_size, sequence_length, num_tag, num_tag] float tensor
-        representing log potentials.
+            representing log potentials.
         tag_bitmap: A [batch_size, sequence_length, num_tag] boolean tensor indicating
-        all active tags at each index.
+            all active tags at each index.
         mask: A [batch_size, sequence_length] boolean tensor.
         outside_index: An integer representing a non-entity index.
         target_entity_ratio: A float representing a target entity ratio
-        for training. Defaults to 0.15.
+            for training. Defaults to 0.15.
         entity_ratio_margin: A float representing a margin for the entity ratio.
-        Defaults to 0.05.
+            Defaults to 0.05.
         balancing_coefficient: An integer representing a balancing coefficient
-        for the loss function. Defaults to 10.
+            for the loss function. Defaults to 10.
 
     Returns:
         A float representing loss.
     """
     with torch.enable_grad():
         # log partition
         log_Z = F.forward_algorithm(log_potentials)
@@ -91,25 +91,25 @@
     """A trainer for fitting the parameters of a tagger based on a given dataset.
 
     Args:
         tokenizer: An instance of BaseTokenizer.
         encoder_factory: An encoder factory for creating encoders.
         batch_size: An integer representing a batch size for training. Defaults to 15.
         num_epochs: An integer representing the number of epochs for training.
-        Defaults to 20.
+            Defaults to 20.
         learning_rate: A float representing a learning rate for optimization.
-        Defaults to 2e-5.
+            Defaults to 2e-5.
         gradient_clip_value: A float representing a maximum gradient value
-        for clipping. Defaults to 5.0.
+            for clipping. Defaults to 5.0.
         target_entity_ratio: A float representing a target entity ratio
-        for training. Defaults to 0.15.
+            for training. Defaults to 0.15.
         entity_ratio_margin: A float representing a margin for the entity ratio.
-        Defaults to 0.05.
+            Defaults to 0.05.
         balancing_coefficient: An integer representing a balancing coefficient
-        for the loss function. Defaults to 10.
+            for the loss function. Defaults to 10.
         padding_index: An integer representing an index for padding. Defaults to -1.
     """
 
     def __init__(
         self,
         tokenizer: BaseTokenizer,
         encoder_factory: BaseEncoderFactory,
@@ -141,15 +141,15 @@
         logger: Logger | None = None,
     ) -> Recognizer:
         """Trains an instance of SequenceTagger.
 
         Args:
             train_dataset: A list of training data tuples containing text and tags.
             validation_dataset: A list of validation data tuples
-            containing text and tags.
+                containing text and tags.
             device: A device to be used for training.
             logger: A logger for logging training progress. Defaults to None.
 
         Returns:
             An instance of Recognizer which predicts character-based tags
             from a given text.
         """
```

### Comparing `pytorch_partial_tagger-0.1.8/src/partial_tagger/utils.py` & `pytorch_partial_tagger-0.1.9/src/partial_tagger/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 from transformers import AutoTokenizer
 
-from .data.batch.text import TransformerTokenizer
-from .data.core import Span, Tag
-from .encoders.transformer import (
+from partial_tagger.data.batch.text import TransformerTokenizer
+from partial_tagger.data.core import Span, Tag
+from partial_tagger.encoders.transformer import (
     TransformerModelEncoderFactory,
     TransformerModelWithHeadEncoderFactory,
 )
-from .training import Trainer
+from partial_tagger.training import Trainer
 
 
 def create_tag(start: int, length: int, label: str) -> Tag:
     """Creates a tag.
 
     Args:
         start: An integer representing a start index of a tag.
```

### Comparing `pytorch_partial_tagger-0.1.8/src/partial_tagger/crf/functional.py` & `pytorch_partial_tagger-0.1.9/src/partial_tagger/crf/functional.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from typing import Callable, Optional, Tuple
 
 import torch
 
-from . import NINF
+from partial_tagger.crf import NINF
 
 # collections.abc.Callable is preferred.
 Matmul = Callable[[torch.Tensor, torch.Tensor], torch.Tensor]
 
 
 def log_likelihood(
     log_potentials: torch.Tensor,
     tag_indices: torch.Tensor,
     mask: Optional[torch.Tensor] = None,
 ) -> torch.Tensor:
     """Computes log likelihood.
 
     Args:
         log_potentials: A [batch_size, sequence_length, num_tags, num_tags]
-        float tensor.
+            float tensor.
         tag_indices: A [batch_size, sequence_length] integer tensor
-        indicating an active index.
+            indicating an active index.
         mask: A [batch_size, sequence_length] boolean tensor.
 
     Returns:
         A [batch_size] float tensor representing log likelihood.
     """
 
     score = sequence_score(log_potentials, tag_indices, mask)
@@ -37,17 +37,17 @@
     tag_bitmap: torch.Tensor,
     mask: Optional[torch.Tensor] = None,
 ) -> torch.Tensor:
     """Computes marginal log likelihood.
 
     Args:
         log_potentials: A [batch_size, sequence_length, num_tags, num_tags]
-        float tensor.
+            float tensor.
         tag_bitmap: A [batch_size, sequence_length, num_tags] boolean tensor
-        indicating all active tags at each index.
+            indicating all active tags at each index.
         mask: A [batch_size, sequence_length] boolean tensor.
 
     Returns:
         A [batch_size] float tensor representing marginal log likelihood.
     """
 
     score = multitag_sequence_score(log_potentials, tag_bitmap, mask)
@@ -59,15 +59,15 @@
 def normalize(
     log_potentials: torch.Tensor, matmul: Matmul, normalizer: Callable
 ) -> torch.Tensor:
     """Normalizes log potentials based on normalizer.
 
     Args:
         log_potentials: A [batch_size, sequence_length, num_tags, num_tags]
-        float tensor.
+            float tensor.
         matmul: A general matrix multiplication.
         normalizer: A reduce operation.
 
     Returns:
         A [batch_size] float tensor representing the normalized value.
     """
     batch_size, sequence_length, num_tags, _ = log_potentials.size()
@@ -122,28 +122,28 @@
 
 
 def forward_algorithm(log_potentials: torch.Tensor) -> torch.Tensor:
     """Computes the normalizer for a CRF.
 
     Args:
         log_potentials: A [batch_size, sequence_length, num_tags, num_tags]
-        float tensor.
+            float tensor.
 
     Returns:
         A [batch_size] float tensor representing the normalizer.
     """
     return normalize(log_potentials, log_matmul, torch.logsumexp)
 
 
 def amax(log_potentials: torch.Tensor) -> torch.Tensor:
     """Computes the maximum score for a CRF.
 
     Args:
         log_potentials: A [batch_size, sequence_length, num_tags, num_tags]
-        float tensor.
+            float tensor.
 
     Returns:
         A [batch_size] float tensor representing the maximum score.
     """
 
     def _amax(inputs: torch.Tensor, dim: int) -> torch.Tensor:
         return torch.max(inputs, dim=dim).values
@@ -152,15 +152,15 @@
 
 
 def decode(log_potentials: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
     """Computes the tag sequence gives the maximum probability for log potentials.
 
     Args:
         log_potentials: A [batch_size, sequence_length, num_tags, num_tags]
-        float tensor.
+            float tensor.
 
     Returns:
         A tuple of tensors. The first tensor is a [batch_size] float tensor
         representing the maximum score. The second tensor is
         a [batch_size, sequence_length] integer tensor representing the tag sequence.
     """
     max_score = amax(log_potentials)
@@ -182,15 +182,15 @@
     end_constraints: torch.Tensor,
     transition_constraints: torch.Tensor,
 ) -> torch.Tensor:
     """Constrains start/end/transition to the given log potentials.
 
     Args:
         log_potentials: A [batch_size, sequence_length, num_tags, num_tags]
-        float tensor.
+            float tensor.
         mask: A [batch_size, sequence_length] boolean tensor.
         start_constraints: A [num_tags] boolean tensor.
         end_constraints: A [num_tags] boolean tensor.
         transition_constraints: A [num_tags, num_tags] boolean tensor.
 
     Returns:
         A [batch_size, sequence_length, num_tags, num_tags] float tensor.
@@ -226,17 +226,17 @@
     tag_indices: torch.Tensor,
     mask: Optional[torch.Tensor] = None,
 ) -> torch.Tensor:
     """Computes the sequence score based on the given tag_bitmap.
 
     Args:
         log_potentials: A [batch_size, sequence_length, num_tags, num_tags]
-        float tensor.
+            float tensor.
         tag_indices: A [batch_size, sequence_length] integer tensor
-        indicating an active index.
+            indicating an active index.
         mask: A [batch_size, sequence_length] boolean tensor.
 
     Returns:
         A [batch_size] float tensor representing the sequence score.
     """
     if mask is None:
         mask = torch.ones_like(tag_indices, dtype=torch.bool)
@@ -262,17 +262,17 @@
     tag_bitmap: torch.Tensor,
     mask: Optional[torch.Tensor] = None,
 ) -> torch.Tensor:
     """Computes the sequence score of all tag sequences matching.
 
     Args:
         log_potentials: A [batch_size, sequence_length, num_tags, num_tags]
-        float tensor.
+            float tensor.
         tag_bitmap: A [batch_size, sequence_length, num_tags] boolean tensor
-        indicating all active tags at each index.
+            indicating all active tags at each index.
         mask: A [batch_size, sequence_length] boolean tensor.
 
     Returns:
         A [batch_size] float tensor representing the sequence score.
     """
     if mask is None:
         mask = tag_bitmap.new_ones(tag_bitmap.shape[:-1], dtype=torch.bool)
```

### Comparing `pytorch_partial_tagger-0.1.8/src/partial_tagger/crf/nn.py` & `pytorch_partial_tagger-0.1.9/src/partial_tagger/crf/nn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import torch
 from torch import nn
 
-from . import NINF
+from partial_tagger.crf import NINF
 
 
 class CRF(nn.Module):
     """A Conditional Random Field (CRF) layer.
 
     Args:
         num_tags: An integer representing the number of tags.
```

### Comparing `pytorch_partial_tagger-0.1.8/src/partial_tagger/data/core.py` & `pytorch_partial_tagger-0.1.9/src/partial_tagger/data/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 class TokenizedText:
     """A TokenizedText represents a text that has been tokenized and provides
     convenient methods to access its tokens and spans.
 
     Args:
         text: An original text.
         char_spans: A tuple of character spans for each token, or None if
-        there is no corresponding span.
+            there is no corresponding span.
         token_indices: A tuple of token indices for each character, or -1 if there is
-        no corresponding token.
+            no corresponding token.
         addtional_token: A string used to represent token without no corresponding
-        character span. Defaults to "[Token]".
+            character span. Defaults to "[Token]".
     """
 
     def __init__(
         self,
         text: str,
         char_spans: tuple[Span | None, ...],
         token_indices: tuple[int, ...],
@@ -219,15 +219,15 @@
         self, label_set: LabelSet, unknown_index: int = -100
     ) -> list[int]:
         """Returns a list of active tag indices.
 
         Args:
             label_set: An instance of LabelSet.
             unknown_index: An integer representing an index for an unknown tag.
-            Defaults to -100.
+                Defaults to -100.
 
         Returns:
             A list of integers, where each integer represents an active tag.
 
         """
         tag_indices = [unknown_index] * self.tokenized_text.num_tokens
```

### Comparing `pytorch_partial_tagger-0.1.8/src/partial_tagger/data/batch/__init__.py` & `pytorch_partial_tagger-0.1.9/src/partial_tagger/data/batch/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
-from ..core import CharBasedTags, LabelSet
-from .tag import TagsBatch
-from .text import BaseTokenizer, TextBatch
+from partial_tagger.data.batch.tag import TagsBatch
+from partial_tagger.data.batch.text import BaseTokenizer, TextBatch
+from partial_tagger.data.core import CharBasedTags, LabelSet
 
 
 class Collator:
     def __init__(self, tokenizer: BaseTokenizer, label_set: LabelSet):
         self.__tokenizer = tokenizer
         self.__label_set = label_set
```

### Comparing `pytorch_partial_tagger-0.1.8/src/partial_tagger/data/batch/tag.py` & `pytorch_partial_tagger-0.1.9/src/partial_tagger/data/batch/tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import torch
 
-from ..core import CharBasedTags, LabelSet, TokenBasedTags
+from partial_tagger.data.core import CharBasedTags, LabelSet, TokenBasedTags
 
 
 class TagsBatch:
     """A batch of token-based tags.
 
     Args:
         tags_batch: A tuple of instances of TokenBasedTags.
@@ -42,17 +42,17 @@
     def get_tag_indices(
         self, padding_index: int = -1, unknown_index: int = -100
     ) -> torch.Tensor:
         """Returns a tensor of tag indices for a batch.
 
         Args:
             padding_index: An integer representing an index to pad a tensor.
-            Defaults to -1.
+                Defaults to -1.
             unknown_index: An integer representing an index for an unknown tag.
-            Defaults to -100.
+                Defaults to -100.
 
         Returns:
             A [batch_size, sequence_length] integer tensor representing tag indices.
         """
         label_set = self.__label_set
 
         max_length = max(tags.num_tokens for tags in self.__tags_batch)
```

### Comparing `pytorch_partial_tagger-0.1.8/src/partial_tagger/data/batch/text.py` & `pytorch_partial_tagger-0.1.9/src/partial_tagger/data/batch/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from abc import ABCMeta, abstractmethod
 from typing import Any
 
 import torch
 from transformers.tokenization_utils import PreTrainedTokenizer
 
-from ..core import (
+from partial_tagger.data.core import (
     CharBasedTags,
     LabelSet,
     Span,
     Status,
     Tag,
     TokenBasedTags,
     TokenizedText,
@@ -67,15 +67,15 @@
 class TextBatch:
     """A batch of text data for tagging.
 
     Args:
         tokenized_texts: A tuple of instances of TokenizedText.
         tagger_inputs: A dictionary that maps string keys to a tensor values.
         mask: A [batch_size, sequence_length] float tensor representing
-        a mask for a batch.
+            a mask for a batch.
         device: A device on which to place tensors. Defaults to None.
 
     Attributes:
         tokenized_texts: A tuple of instances of TokenizedText.
     """
 
     def __init__(
```

### Comparing `pytorch_partial_tagger-0.1.8/src/partial_tagger/decoders/viterbi.py` & `pytorch_partial_tagger-0.1.9/src/partial_tagger/decoders/viterbi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from __future__ import annotations
 
 import torch
 from torch.nn import Module, Parameter
 
-from ..crf import functional as F
+from partial_tagger.crf import functional as F
 
 
 class Constrainer(Module):
     """A constrainer to constrain the given log potentials of a CRF.
 
     Args:
         start_states: A list of boolean values representing the start states.
-        True indicates an allowed state, while False indicates an otherwise state.
+            True indicates an allowed state, while False indicates an otherwise state.
         end_states: A list of boolean values representing the end states.
-        True indicates an allowed state, while False indicates an otherwise state.
+            True indicates an allowed state, while False indicates an otherwise state.
         transitions: A list of lists of boolean values representing the transitions.
-        True indicates an allowed transition,
-        while False indicates an otherwise transition.
+            True indicates an allowed transition,
+            while False indicates an otherwise transition.
 
     Attributes:
         start_states: Start states parameters.
         end_states: End states parameters.
         transitions: transitions parameters.
 
     """
@@ -38,15 +38,15 @@
         self.transitions = Parameter(torch.tensor(transitions), requires_grad=False)
 
     def forward(self, log_potentials: torch.Tensor, mask: torch.Tensor) -> torch.Tensor:
         """Applies constraints to a given log potentials.
 
         Args:
             log_potentials: A [batch_size, sequence_length, num_tags, num_tags]
-            float tensor.
+                float tensor.
             mask: A [batch_size, sequence_length] boolean tensor.
 
         Returns:
             A [batch_size, sequence_length, num_tags, num_tags] float tensor
             representing constrained log potentials.
         """
         return F.constrain_log_potentials(
@@ -77,15 +77,15 @@
         self.constrainer = constrainer
 
     def forward(self, log_potentials: torch.Tensor, mask: torch.Tensor) -> torch.Tensor:
         """Computes the best tag sequence from the given log potentials.
 
         Args:
             log_potentials: A [batch_size, sequence_length, num_tags, num_tags]
-            float tensor.
+                float tensor.
             mask: A [batch_size, sequence_length] boolean tensor.
 
         Returns:
             A [batch_size, sequence_length] integer tensor representing
             the best tag sequence.
         """
```

### Comparing `pytorch_partial_tagger-0.1.8/src/partial_tagger/encoders/base.py` & `pytorch_partial_tagger-0.1.9/src/partial_tagger/encoders/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
 
 import torch
 from torch.nn import Module
 
-from ..data.core import LabelSet
+from partial_tagger.data.core import LabelSet
 
 
 class BaseEncoder(Module, metaclass=ABCMeta):
     """Base class for all encoders."""
 
     @abstractmethod
     def forward(self, inputs: dict[str, torch.Tensor]) -> torch.Tensor:
```

### Comparing `pytorch_partial_tagger-0.1.8/src/partial_tagger/encoders/transformer.py` & `pytorch_partial_tagger-0.1.9/src/partial_tagger/encoders/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from __future__ import annotations
 
 import torch
 from torch import nn
 from transformers import AutoModel, AutoModelForTokenClassification, PreTrainedModel
 
-from ..data.core import LabelSet
-from .base import BaseEncoder, BaseEncoderFactory
+from partial_tagger.data.core import LabelSet
+from partial_tagger.encoders.base import BaseEncoder, BaseEncoderFactory
 
 
 class TransformerModelEncoder(BaseEncoder):
     """A Transformer-based encoder for transforming inputs into
     a fixed-size tensor representation.
 
     Args:
         model: A pre-trained transformer model to use for encoding.
         embedding_size: An integer representing the size of the input embeddings.
         hidden_size: An integer representing the dimension size of
-        the output tensor representation.
+            the output tensor representation.
         dropout_prob: A float representing dropout probability to apply.
-        Defaults to 0.2.
+            Defaults to 0.2.
 
     Attributes:
         model: A pre-trained transformer model.
         linear: A linear layer for projecting embeddings to the hidden size.
         dropout: A dropout layer for regularization.
     """
```

### Comparing `pytorch_partial_tagger-0.1.8/tests/conftest.py` & `pytorch_partial_tagger-0.1.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.8/tests/helpers.py` & `pytorch_partial_tagger-0.1.9/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.8/tests/test_matchers.py` & `pytorch_partial_tagger-0.1.9/tests/test_matchers.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.8/tests/test_metric.py` & `pytorch_partial_tagger-0.1.9/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.8/tests/test_recognizer.py` & `pytorch_partial_tagger-0.1.9/tests/test_recognizer.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.8/tests/crf/test_functional.py` & `pytorch_partial_tagger-0.1.9/tests/crf/test_functional.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.8/tests/crf/test_nn.py` & `pytorch_partial_tagger-0.1.9/tests/crf/test_nn.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.8/tests/data/test_core.py` & `pytorch_partial_tagger-0.1.9/tests/data/test_core.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.8/tests/data/batch/test_tag.py` & `pytorch_partial_tagger-0.1.9/tests/data/batch/test_tag.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.8/tests/data/batch/test_text.py` & `pytorch_partial_tagger-0.1.9/tests/data/batch/test_text.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.8/.gitignore` & `pytorch_partial_tagger-0.1.9/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -158,7 +158,9 @@
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 .pdm-python
 pdm.lock
 
 .tool-versions
+
+_autosummary
```

### Comparing `pytorch_partial_tagger-0.1.8/LICENSE` & `pytorch_partial_tagger-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.8/README.md` & `pytorch_partial_tagger-0.1.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # pytorch-partial-tagger
 
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/17GcpKmYn49bMM-mCZhiuRu8dkPZ0WXuD?usp=sharing)
+
  This is a library to build a CRF tagger for a partially annotated dataset in PyTorch. You can build your own NER tagger only from dictionary. The algorithm of this tagger is based on Effland and Collins. (2021).
 
 
 ## Usage
 
 Import all dependencies first:
 
@@ -67,12 +69,16 @@
 
 ## Installation
 
 ```bash
 pip install pytorch-partial-tagger
 ```
 
+## Documentation
+
+For details about the pytorch-partial-tagger API,  see the [documentation](https://pytorch-partial-tagger.readthedocs.io/en/latest/).
+
 ## References
 
  - Yuta Tsuboi, Hisashi Kashima, Shinsuke Mori, Hiroki Oda, and Yuji Matsumoto. 2008. [Training Conditional Random Fields Using Incomplete Annotations](https://aclanthology.org/C08-1113/). In _Proceedings of the 22nd International Conference on Computational Linguistics (Coling 2008)_, pages 897–904, Manchester, UK. Coling 2008 Organizing Committee.
 - Alexander Rush. 2020. [Torch-Struct: Deep Structured Prediction Library](https://aclanthology.org/2020.acl-demos.38/). In _Proceedings of the 58th Annual Meeting of the Association for Computational Linguistics: System Demonstrations_, pages 335–342, Online. Association for Computational Linguistics.
 - Thomas Effland and Michael Collins. 2021. [Partially Supervised Named Entity Recognition via the Expected Entity Ratio Loss](https://aclanthology.org/2021.tacl-1.78/). _Transactions of the Association for Computational Linguistics_, 9:1320–1335.
```

### Comparing `pytorch_partial_tagger-0.1.8/pyproject.toml` & `pytorch_partial_tagger-0.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,20 @@
 dev = [
     "pytest>=7.3.1",
     "pytest-cov>=4.1.0",
     "ruff>=0.0.270",
     "black>=23.3.0",
     "mypy>=1.3.0",
 ]
+docs = [
+    "sphinx>=6.2.1",
+    "sphinx-book-theme>=1.0.1",
+    "myst-parser>=2.0.0",
+    "sphinx-copybutton>=0.5.2",
+]
 
 [project.urls]
 Homepage = "https://github.com/yasufumy/pytorch-partial-tagger"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
```

### Comparing `pytorch_partial_tagger-0.1.8/PKG-INFO` & `pytorch_partial_tagger-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-partial-tagger
-Version: 0.1.8
+Version: 0.1.9
 Summary: Sequence Tagger for Partially Annotated Dataset in PyTorch
 Project-URL: Homepage, https://github.com/yasufumy/pytorch-partial-tagger
 Author-email: Yasufumi Taniguchi <yasufumi.taniguchi@gmail.com>
 License: MIT
 License-File: LICENSE
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
@@ -17,18 +17,25 @@
 Requires-Dist: transformers>=4.29.2
 Provides-Extra: dev
 Requires-Dist: black>=23.3.0; extra == 'dev'
 Requires-Dist: mypy>=1.3.0; extra == 'dev'
 Requires-Dist: pytest-cov>=4.1.0; extra == 'dev'
 Requires-Dist: pytest>=7.3.1; extra == 'dev'
 Requires-Dist: ruff>=0.0.270; extra == 'dev'
+Provides-Extra: docs
+Requires-Dist: myst-parser>=2.0.0; extra == 'docs'
+Requires-Dist: sphinx-book-theme>=1.0.1; extra == 'docs'
+Requires-Dist: sphinx-copybutton>=0.5.2; extra == 'docs'
+Requires-Dist: sphinx>=6.2.1; extra == 'docs'
 Description-Content-Type: text/markdown
 
 # pytorch-partial-tagger
 
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/17GcpKmYn49bMM-mCZhiuRu8dkPZ0WXuD?usp=sharing)
+
  This is a library to build a CRF tagger for a partially annotated dataset in PyTorch. You can build your own NER tagger only from dictionary. The algorithm of this tagger is based on Effland and Collins. (2021).
 
 
 ## Usage
 
 Import all dependencies first:
 
@@ -92,12 +99,16 @@
 
 ## Installation
 
 ```bash
 pip install pytorch-partial-tagger
 ```
 
+## Documentation
+
+For details about the pytorch-partial-tagger API,  see the [documentation](https://pytorch-partial-tagger.readthedocs.io/en/latest/).
+
 ## References
 
  - Yuta Tsuboi, Hisashi Kashima, Shinsuke Mori, Hiroki Oda, and Yuji Matsumoto. 2008. [Training Conditional Random Fields Using Incomplete Annotations](https://aclanthology.org/C08-1113/). In _Proceedings of the 22nd International Conference on Computational Linguistics (Coling 2008)_, pages 897–904, Manchester, UK. Coling 2008 Organizing Committee.
 - Alexander Rush. 2020. [Torch-Struct: Deep Structured Prediction Library](https://aclanthology.org/2020.acl-demos.38/). In _Proceedings of the 58th Annual Meeting of the Association for Computational Linguistics: System Demonstrations_, pages 335–342, Online. Association for Computational Linguistics.
 - Thomas Effland and Michael Collins. 2021. [Partially Supervised Named Entity Recognition via the Expected Entity Ratio Loss](https://aclanthology.org/2021.tacl-1.78/). _Transactions of the Association for Computational Linguistics_, 9:1320–1335.
```

