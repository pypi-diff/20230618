# Comparing `tmp/nlp-models-2.2.0.tar.gz` & `tmp/nlp-models-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp-models-2.2.0.tar", last modified: Mon May 29 08:56:40 2023, max compression
+gzip compressed data, was "nlp-models-2.2.1.tar", last modified: Sun Jun 18 19:57:50 2023, max compression
```

## Comparing `nlp-models-2.2.0.tar` & `nlp-models-2.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:56:40.389879 nlp-models-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-29 08:56:28.000000 nlp-models-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-29 08:56:40.389879 nlp-models-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-29 08:56:28.000000 nlp-models-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-29 08:56:28.000000 nlp-models-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-29 08:56:40.389879 nlp-models-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-29 08:56:28.000000 nlp-models-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:56:40.385878 nlp-models-2.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:56:40.389879 nlp-models-2.2.0/src/bert_classifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 08:56:28.000000 nlp-models-2.2.0/src/bert_classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-29 08:56:28.000000 nlp-models-2.2.0/src/bert_classifier/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-29 08:56:28.000000 nlp-models-2.2.0/src/bert_classifier/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-29 08:56:28.000000 nlp-models-2.2.0/src/bert_classifier/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-29 08:56:28.000000 nlp-models-2.2.0/src/bert_classifier/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-29 08:56:28.000000 nlp-models-2.2.0/src/bert_classifier/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-29 08:56:28.000000 nlp-models-2.2.0/src/bert_classifier/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:56:40.389879 nlp-models-2.2.0/src/multi_task_model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 08:56:28.000000 nlp-models-2.2.0/src/multi_task_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-29 08:56:28.000000 nlp-models-2.2.0/src/multi_task_model/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-29 08:56:28.000000 nlp-models-2.2.0/src/multi_task_model/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-29 08:56:28.000000 nlp-models-2.2.0/src/multi_task_model/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-29 08:56:28.000000 nlp-models-2.2.0/src/multi_task_model/mtl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-05-29 08:56:28.000000 nlp-models-2.2.0/src/multi_task_model/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-29 08:56:28.000000 nlp-models-2.2.0/src/multi_task_model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:56:40.389879 nlp-models-2.2.0/src/nlp_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-29 08:56:40.000000 nlp-models-2.2.0/src/nlp_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-29 08:56:40.000000 nlp-models-2.2.0/src/nlp_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 08:56:40.000000 nlp-models-2.2.0/src/nlp_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-29 08:56:40.000000 nlp-models-2.2.0/src/nlp_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-29 08:56:40.000000 nlp-models-2.2.0/src/nlp_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:57:50.020737 nlp-models-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-18 19:57:40.000000 nlp-models-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-18 19:57:50.020737 nlp-models-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-18 19:57:40.000000 nlp-models-2.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-18 19:57:40.000000 nlp-models-2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-18 19:57:50.024737 nlp-models-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-18 19:57:40.000000 nlp-models-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:57:50.020737 nlp-models-2.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:57:50.020737 nlp-models-2.2.1/src/bert_classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 19:57:40.000000 nlp-models-2.2.1/src/bert_classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-18 19:57:40.000000 nlp-models-2.2.1/src/bert_classifier/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-18 19:57:40.000000 nlp-models-2.2.1/src/bert_classifier/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-18 19:57:40.000000 nlp-models-2.2.1/src/bert_classifier/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-18 19:57:40.000000 nlp-models-2.2.1/src/bert_classifier/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-18 19:57:40.000000 nlp-models-2.2.1/src/bert_classifier/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-06-18 19:57:40.000000 nlp-models-2.2.1/src/bert_classifier/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:57:50.020737 nlp-models-2.2.1/src/multi_task_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 19:57:40.000000 nlp-models-2.2.1/src/multi_task_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-18 19:57:40.000000 nlp-models-2.2.1/src/multi_task_model/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-18 19:57:40.000000 nlp-models-2.2.1/src/multi_task_model/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-18 19:57:40.000000 nlp-models-2.2.1/src/multi_task_model/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-18 19:57:40.000000 nlp-models-2.2.1/src/multi_task_model/mtl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-06-18 19:57:40.000000 nlp-models-2.2.1/src/multi_task_model/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-18 19:57:40.000000 nlp-models-2.2.1/src/multi_task_model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:57:50.020737 nlp-models-2.2.1/src/nlp_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-18 19:57:50.000000 nlp-models-2.2.1/src/nlp_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-18 19:57:50.000000 nlp-models-2.2.1/src/nlp_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 19:57:50.000000 nlp-models-2.2.1/src/nlp_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-18 19:57:50.000000 nlp-models-2.2.1/src/nlp_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-18 19:57:50.000000 nlp-models-2.2.1/src/nlp_models.egg-info/top_level.txt
```

### Comparing `nlp-models-2.2.0/LICENSE` & `nlp-models-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nlp-models-2.2.0/PKG-INFO` & `nlp-models-2.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-models
-Version: 2.2.0
+Version: 2.2.1
 Summary: Transformers based NLP models
 Home-page: https://github.com/minggnim/nlp-models
 Author: Ming Gao
 Author-email: ming_gao@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `nlp-models-2.2.0/README.md` & `nlp-models-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nlp-models-2.2.0/setup.cfg` & `nlp-models-2.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nlp-models
-version = 2.2.0
+version = 2.2.1
 author = Ming Gao
 author_email = ming_gao@outlook.com
 url = https://github.com/minggnim/nlp-models
 description = Transformers based NLP models
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers =
```

### Comparing `nlp-models-2.2.0/src/bert_classifier/bert.py` & `nlp-models-2.2.1/src/bert_classifier/bert.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.2.0/src/bert_classifier/data.py` & `nlp-models-2.2.1/src/bert_classifier/data.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.2.0/src/bert_classifier/io.py` & `nlp-models-2.2.1/src/bert_classifier/io.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.2.0/src/bert_classifier/metrics.py` & `nlp-models-2.2.1/src/bert_classifier/metrics.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.2.0/src/bert_classifier/predict.py` & `nlp-models-2.2.1/src/bert_classifier/predict.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.2.0/src/bert_classifier/train.py` & `nlp-models-2.2.1/src/bert_classifier/train.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.2.0/src/multi_task_model/layers.py` & `nlp-models-2.2.1/src/multi_task_model/layers.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.2.0/src/multi_task_model/mtl.py` & `nlp-models-2.2.1/src/multi_task_model/mtl.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,26 +28,29 @@
 
     def mean_pooling(self, model_output, attention_mask):
         token_embeddings = model_output[0]
         input_mask_expanded = attention_mask.unsqueeze(-1).expand(token_embeddings.size()).float()
         return torch.sum(token_embeddings * input_mask_expanded, 1) / torch.clamp(input_mask_expanded.sum(1), min=1e-9)
 
     def cls_pooling(self, model_output):
-        return model_output[0][:,0]
+        return model_output[0][:, 0]
     
     @staticmethod
     def save_model(model, dir):
         torch.save(model, dir)
 
     @staticmethod
     def load_model(dir, device=torch.device('cpu')):
         return torch.load(dir, device)
 
 
 class MTLInference:
+    '''
+    class for MTL model infering
+    '''
     def __init__(self, tokenizer_card, model_card, num_labels=None, pretrained_model=True, device=torch.device('cpu')) -> None:
         self.tokenizer = transformers.AutoTokenizer.from_pretrained(tokenizer_card)
         if pretrained_model:
             self.mtl_model = AutoModelForMTL(model_card, num_labels)
         else:
             self.mtl_model = AutoModelForMTL.load_model(model_card, device)
         self.mtl_model.eval()
@@ -62,18 +65,17 @@
         pred_label = outputs[0]
         query_embedding = outputs[1]
         return pred_label, query_embedding
 
     def optimal_answer(self, query, cat_lookup, corpus, top_k=1):
         pred_label, query_embedding = self.predict(query)
         corpus_embeddings, question_corpus, answer_corpus = get_embedding_group(pred_label, cat_lookup, corpus)
-        sim_scores = torch.mm(query_embedding, corpus_embeddings.transpose(0,1).cpu().tolist())
+        sim_scores = torch.mm(query_embedding, corpus_embeddings.transpose(0, 1).cpu().tolist())
         top_idx = np.argpartition(sim_scores, range(-top_k, 0))[-top_k:][::-1]
         score = list(sim_scores[top_idx])
         question_matched = [question_corpus[i] for i in top_idx]
         answer_matched = [answer_corpus[i] for i in top_idx]
         return dict(
             question_matched=question_matched,
             answer_matched=answer_matched,
             score=score
         )
-
```

### Comparing `nlp-models-2.2.0/src/multi_task_model/trainer.py` & `nlp-models-2.2.1/src/multi_task_model/trainer.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.2.0/src/multi_task_model/utils.py` & `nlp-models-2.2.1/src/multi_task_model/utils.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.2.0/src/nlp_models.egg-info/PKG-INFO` & `nlp-models-2.2.1/src/nlp_models.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-models
-Version: 2.2.0
+Version: 2.2.1
 Summary: Transformers based NLP models
 Home-page: https://github.com/minggnim/nlp-models
 Author: Ming Gao
 Author-email: ming_gao@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `nlp-models-2.2.0/src/nlp_models.egg-info/SOURCES.txt` & `nlp-models-2.2.1/src/nlp_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

