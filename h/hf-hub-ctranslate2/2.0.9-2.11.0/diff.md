# Comparing `tmp/hf_hub_ctranslate2-2.0.9.tar.gz` & `tmp/hf_hub_ctranslate2-2.11.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hf_hub_ctranslate2-2.0.9.tar", last modified: Fri Jun  2 15:54:11 2023, max compression
+gzip compressed data, was "hf_hub_ctranslate2-2.11.0.tar", last modified: Sun Jun 18 21:47:30 2023, max compression
```

## Comparing `hf_hub_ctranslate2-2.0.9.tar` & `hf_hub_ctranslate2-2.11.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:54:11.639657 hf_hub_ctranslate2-2.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-02 15:54:00.000000 hf_hub_ctranslate2-2.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-02 15:54:11.639657 hf_hub_ctranslate2-2.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-06-02 15:54:00.000000 hf_hub_ctranslate2-2.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:54:11.635657 hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-02 15:54:00.000000 hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-06-02 15:54:00.000000 hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:54:11.639657 hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 15:54:00.000000 hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-02 15:54:00.000000 hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2/util/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:54:11.639657 hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-02 15:54:11.000000 hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-02 15:54:11.000000 hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 15:54:11.000000 hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-02 15:54:11.000000 hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-02 15:54:11.000000 hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-02 15:54:00.000000 hf_hub_ctranslate2-2.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 15:54:11.639657 hf_hub_ctranslate2-2.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-02 15:54:00.000000 hf_hub_ctranslate2-2.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:54:11.639657 hf_hub_ctranslate2-2.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-02 15:54:00.000000 hf_hub_ctranslate2-2.0.9/tests/test_translate.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-02 15:54:00.000000 hf_hub_ctranslate2-2.0.9/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:47:30.984673 hf_hub_ctranslate2-2.11.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-18 21:47:22.000000 hf_hub_ctranslate2-2.11.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-06-18 21:47:30.984673 hf_hub_ctranslate2-2.11.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-06-18 21:47:22.000000 hf_hub_ctranslate2-2.11.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:47:30.984673 hf_hub_ctranslate2-2.11.0/hf_hub_ctranslate2/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-18 21:47:22.000000 hf_hub_ctranslate2-2.11.0/hf_hub_ctranslate2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-06-18 21:47:22.000000 hf_hub_ctranslate2-2.11.0/hf_hub_ctranslate2/ct2_sentence_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19419 2023-06-18 21:47:22.000000 hf_hub_ctranslate2-2.11.0/hf_hub_ctranslate2/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:47:30.984673 hf_hub_ctranslate2-2.11.0/hf_hub_ctranslate2/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 21:47:22.000000 hf_hub_ctranslate2-2.11.0/hf_hub_ctranslate2/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-18 21:47:22.000000 hf_hub_ctranslate2-2.11.0/hf_hub_ctranslate2/util/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:47:30.984673 hf_hub_ctranslate2-2.11.0/hf_hub_ctranslate2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-06-18 21:47:30.000000 hf_hub_ctranslate2-2.11.0/hf_hub_ctranslate2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-18 21:47:30.000000 hf_hub_ctranslate2-2.11.0/hf_hub_ctranslate2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 21:47:30.000000 hf_hub_ctranslate2-2.11.0/hf_hub_ctranslate2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-18 21:47:30.000000 hf_hub_ctranslate2-2.11.0/hf_hub_ctranslate2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 21:47:30.000000 hf_hub_ctranslate2-2.11.0/hf_hub_ctranslate2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-18 21:47:22.000000 hf_hub_ctranslate2-2.11.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 21:47:30.984673 hf_hub_ctranslate2-2.11.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-18 21:47:22.000000 hf_hub_ctranslate2-2.11.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:47:30.984673 hf_hub_ctranslate2-2.11.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-06-18 21:47:22.000000 hf_hub_ctranslate2-2.11.0/tests/test_ct2_sentence_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-18 21:47:22.000000 hf_hub_ctranslate2-2.11.0/tests/test_translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-18 21:47:22.000000 hf_hub_ctranslate2-2.11.0/tests/test_version.py
```

### Comparing `hf_hub_ctranslate2-2.0.9/LICENSE` & `hf_hub_ctranslate2-2.11.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hf_hub_ctranslate2-2.0.9/PKG-INFO` & `hf_hub_ctranslate2-2.11.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,11 @@
-Metadata-Version: 2.1
-Name: hf_hub_ctranslate2
-Version: 2.0.9
-Summary: Connecting Transfromers on HuggingfaceHub with Ctranslate2 
-Home-page: https://github.com/michaelfeil/hf-hub-ctranslate2
-Author: Michael Feil
-License: MIT
-Project-URL: Bug Tracker, https://github.com/michaelfeil/hf-hub-ctranslate2/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 hf_hub_ctranslate2
 ==============================
 
-Connecting Transfromers on HuggingfaceHub with Ctranslate2 - a small utility for keeping tokenizer and model around Huggingface Hub.
+Connecting Transformers on HuggingfaceHub with Ctranslate2 - a small utility for keeping tokenizer and model around Huggingface Hub.
 
 [![codecov](https://codecov.io/gh/michaelfeil/hf-hub-ctranslate2/branch/main/graph/badge.svg?token=U9VIEFEELS)](https://codecov.io/gh/michaelfeil/hf-hub-ctranslate2)![CI pytest](https://github.com/michaelfeil/hf-hub-ctranslate2/actions/workflows/test_release.yml/badge.svg)
 
 [Read the docs](https://michaelfeil.github.io/hf-hub-ctranslate2/)
 
 <!-- PROJECT SHIELDS -->
 [![Contributors][contributors-shield]][contributors-url]
@@ -27,31 +13,32 @@
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
 [![LinkedIn][linkedin-shield]][linkedin-url]
 
 --------
 ## Usage:
-#### Decoder-only Transformer:
+## Decoder-only Transformer:
 ```python
 # download ctranslate.Generator repos from Huggingface Hub (GPT-J, ..)
 from hf_hub_ctranslate2 import TranslatorCT2fromHfHub, GeneratorCT2fromHfHub
 
 model_name_1="michaelfeil/ct2fast-pythia-160m"
 model = GeneratorCT2fromHfHub(
     # load in int8 on CPU
     model_name_or_path=model_name_1, device="cpu", compute_type="int8"
 )
 outputs = model.generate(
     text=["How do you call a fast Flan-ingo?", "User: How are you doing?"]
     # add arguments specifically to ctranslate2.Generator here
 )
 ```
-#### Encoder-Decoder:
+## Encoder-Decoder:
 ```python
+from hf_hub_ctranslate2 import TranslatorCT2fromHfHub
 # download ctranslate.Translator repos from Huggingface Hub (T5, ..)
 model_name_2 = "michaelfeil/ct2fast-flan-alpaca-base"
 model = TranslatorCT2fromHfHub(
         # load in int8 on CUDA
         model_name_or_path=model_name_2, device="cuda", compute_type="int8_float16"
 )
 outputs = model.generate(
@@ -60,27 +47,60 @@
     min_decoding_length=8,
     max_decoding_length=16,
     max_input_length=512,
     beam_size=3
 )
 print(outputs)
 ```
-#### Encoder-Decoder for multilingual translations (m2m-100):
+## Encoder-Decoder for multilingual translations (m2m-100):
 ```python
+from hf_hub_ctranslate2 import MultiLingualTranslatorCT2fromHfHub
 model = MultiLingualTranslatorCT2fromHfHub(
     model_name_or_path="michaelfeil/ct2fast-m2m100_418M", device="cpu", compute_type="int8",
     tokenizer=AutoTokenizer.from_pretrained(f"facebook/m2m100_418M")
 )
 
 outputs = model.generate(
     ["How do you call a fast Flamingo?", "Wie geht es dir?"],
     src_lang=["en", "de"],
     tgt_lang=["de", "fr"]
 )
 ```
+## Encoder-only Sentence Transformers
+```python
+from hf_hub_ctranslate2 import CT2SentenceTransformer
+model_name_pytorch = "intfloat/e5-small"
+model = CT2SentenceTransformer(
+    model_name_pytorch, compute_type="int8", device="cuda", 
+)
+embeddings = model.encode(
+    ["I like soccer", "I like tennis", "The eiffel tower is in Paris"],
+    batch_size=32,
+    convert_to_numpy=True,
+    normalize_embeddings=True,
+)
+print(embeddings.shape, embeddings)
+scores = (embeddings @ embeddings.T) * 100
+```
+
+## Encoder-only
+```python
+from hf_hub_ctranslate2 import EncoderCT2fromHfHub
+model_name = "michaelfeil/ct2fast-e5-small"
+model = EncoderCT2fromHfHub(
+        # load in int8 on CUDA
+        model_name_or_path=model_name,
+        device="cuda",
+        compute_type="int8_float16",
+)
+outputs = model.generate(
+    text=["I like soccer", "I like tennis", "The eiffel tower is in Paris"],
+    max_length=64,
+)
+```
 
 --------
 ## PYPI Install
 ```bash
 pip install hf-hub-ctranslate2
 ```
 --------
```

### Comparing `hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2/translate.py` & `hf_hub_ctranslate2-2.11.0/hf_hub_ctranslate2/translate.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import ctranslate2
+import functools
+
 try:
     from transformers import AutoTokenizer
     autotokenizer_ok = True
 except ImportError:
     AutoTokenizer = object
     autotokenizer_ok = False
 
@@ -24,56 +26,71 @@
         self,
         model_name_or_path: str,
         device: Literal["cpu", "cuda"] = "cuda",
         device_index=0,
         compute_type: Literal["int8_float16", "int8"] = "int8_float16",
         tokenizer: Union[AutoTokenizer, None] = None,
         hub_kwargs: dict = {},
-        **kwargs: Any
+        **kwargs: Any,
     ):
         # adaptions from https://github.com/guillaumekln/faster-whisper
         if os.path.isdir(model_name_or_path):
             model_path = model_name_or_path
         else:
             try:
-                model_path = _utils._download_model(model_name_or_path, hub_kwargs=hub_kwargs)
-            except:
+                model_path = _utils._download_model(
+                    model_name_or_path, hub_kwargs=hub_kwargs
+                )
+            except Exception:
                 hub_kwargs["local_files_only"] = True
-                model_path = _utils._download_model(model_name_or_path, hub_kwargs=hub_kwargs)
+                model_path = _utils._download_model(
+                    model_name_or_path, hub_kwargs=hub_kwargs
+                )
         self.model = self.ctranslate_class(
             model_path,
             device=device,
             device_index=device_index,
             compute_type=compute_type,
-            **kwargs
+            **kwargs,
         )
 
         if tokenizer is not None:
             self.tokenizer = tokenizer
         else:
             if "tokenizer.json" in os.listdir(model_path):
                 if not autotokenizer_ok:
-                    raise ValueError("`pip install transformers` missing to load AutoTokenizer.")
+                    raise ValueError(
+                        "`pip install transformers` missing to load AutoTokenizer."
+                    )
                 self.tokenizer = AutoTokenizer.from_pretrained(model_path, fast=True)
             else:
-                raise ValueError("no suitable Tokenizer found. "
-                                 "Please set one via tokenizer=AutoTokenizer.from_pretrained(..) arg.")
-                
+                raise ValueError(
+                    "no suitable Tokenizer found. "
+                    "Please set one via tokenizer=AutoTokenizer.from_pretrained(..) arg."
+                )
 
     def _forward(self, *args: Any, **kwds: Any) -> Any:
         raise NotImplementedError
-    
+
     def tokenize_encode(self, text, *args, **kwargs):
         return [
             self.tokenizer.convert_ids_to_tokens(self.tokenizer.encode(p)) for p in text
         ]
+
     def tokenize_decode(self, tokens_out, *args, **kwargs):
         raise NotImplementedError
 
-    def generate(self, text: Union[str, List[str]], encode_kwargs={}, decode_kwargs={}, *forward_args, **forward_kwds: Any):
+    def generate(
+        self,
+        text: Union[str, List[str]],
+        encode_kwargs={},
+        decode_kwargs={},
+        *forward_args,
+        **forward_kwds: Any,
+    ):
         orig_type = list
         if isinstance(text, str):
             orig_type = str
             text = [text]
         token_list = self.tokenize_encode(text, **encode_kwargs)
         tokens_out = self._forward(token_list, *forward_args, **forward_kwds)
         texts_out = self.tokenize_decode(tokens_out, **decode_kwargs)
@@ -88,51 +105,59 @@
         self,
         model_name_or_path: str,
         device: Literal["cpu", "cuda"] = "cuda",
         device_index=0,
         compute_type: Literal["int8_float16", "int8"] = "int8_float16",
         tokenizer: Union[AutoTokenizer, None] = None,
         hub_kwargs={},
-        **kwargs: Any
+        **kwargs: Any,
     ):
         """for ctranslate2.Translator models, in particular m2m-100
 
         Args:
             model_name_or_path (str): _description_
-            device (Literal[&quot;cpu&quot;, &quot;cuda&quot;], optional): _description_. Defaults to "cuda".
+            device (Literal[cpu, cuda], optional): _description_. Defaults to "cuda".
             device_index (int, optional): _description_. Defaults to 0.
-            compute_type (Literal[&quot;int8_float16&quot;, &quot;int8&quot;], optional): _description_. Defaults to "int8_float16".
+            compute_type (Literal[int8_float16, int8], optional): _description_. Defaults to "int8_float16".
             tokenizer (Union[AutoTokenizer, None], optional): _description_. Defaults to None.
             hub_kwargs (dict, optional): _description_. Defaults to {}.
             **kwargs (Any, optional): Any additional arguments
         """
         self.ctranslate_class = ctranslate2.Translator
         super().__init__(
             model_name_or_path,
             device,
             device_index,
             compute_type,
             tokenizer,
             hub_kwargs,
-            **kwargs
+            **kwargs,
         )
 
     def _forward(self, *args, **kwds):
         return self.model.translate_batch(*args, **kwds)
-    
+
     def tokenize_decode(self, tokens_out, *args, **kwargs):
         return [
             self.tokenizer.decode(
                 self.tokenizer.convert_tokens_to_ids(tokens_out[i].hypotheses[0]),
-                *args, **kwargs
+                *args,
+                **kwargs,
             )
             for i in range(len(tokens_out))
         ]
 
-    def generate(self, text: Union[str, List[str]], encode_tok_kwargs={}, decode_tok_kwargs={}, *forward_args, **forward_kwds: Any):
+    def generate(
+        self,
+        text: Union[str, List[str]],
+        encode_tok_kwargs={},
+        decode_tok_kwargs={},
+        *forward_args,
+        **forward_kwds: Any,
+    ):
         """_summary_
 
         Args:
             text (Union[str, List[str]]): Input texts
             encode_tok_kwargs (dict, optional): additional kwargs for tokenizer
             decode_tok_kwargs (dict, optional): additional kwargs for tokenizer
             max_batch_size (int, optional): Batch size. Defaults to 0.
@@ -164,72 +189,91 @@
             sampling_temperature (float, optional): _. Defaults to 1.
             replace_unknowns (bool, optional): _. Defaults to False.
             callback (_type_, optional): _. Defaults to None.
 
         Returns:
             Union[str, List[str]]: text as output, if list, same len as input
         """
-        return super().generate(text, encode_kwargs=encode_tok_kwargs, decode_kwargs=decode_tok_kwargs, *forward_args, **forward_kwds)
+        return super().generate(
+            text,
+            encode_kwargs=encode_tok_kwargs,
+            decode_kwargs=decode_tok_kwargs,
+            *forward_args,
+            **forward_kwds,
+        )
+
 
 class MultiLingualTranslatorCT2fromHfHub(CTranslate2ModelfromHuggingfaceHub):
     def __init__(
         self,
         model_name_or_path: str,
         device: Literal["cpu", "cuda"] = "cuda",
         device_index=0,
         compute_type: Literal["int8_float16", "int8"] = "int8_float16",
         tokenizer: Union[AutoTokenizer, None] = None,
         hub_kwargs={},
-        **kwargs: Any
+        **kwargs: Any,
     ):
         """for ctranslate2.Translator models
 
         Args:
             model_name_or_path (str): _description_
-            device (Literal[&quot;cpu&quot;, &quot;cuda&quot;], optional): _description_. Defaults to "cuda".
+            device (Literal[cpu, cuda], optional): _description_. Defaults to "cuda".
             device_index (int, optional): _description_. Defaults to 0.
-            compute_type (Literal[&quot;int8_float16&quot;, &quot;int8&quot;], optional): _description_. Defaults to "int8_float16".
+            compute_type (Literal[int8_float16, int8], optional): _description_. Defaults to "int8_float16".
             tokenizer (Union[AutoTokenizer, None], optional): _description_. Defaults to None.
             hub_kwargs (dict, optional): _description_. Defaults to {}.
             **kwargs (Any, optional): Any additional arguments
         """
         self.ctranslate_class = ctranslate2.Translator
         super().__init__(
             model_name_or_path,
             device,
             device_index,
             compute_type,
             tokenizer,
             hub_kwargs,
-            **kwargs
+            **kwargs,
         )
-        
+
     def _forward(self, *args, **kwds):
-        target_prefix = [[self.tokenizer.lang_code_to_token[l]] for l in kwds.pop("tgt_lang")]
+        target_prefix = [
+            [self.tokenizer.lang_code_to_token[lng]] for lng in kwds.pop("tgt_lang")
+        ]
         # target_prefix=[['__de__'], ['__fr__']]
         return self.model.translate_batch(*args, **kwds, target_prefix=target_prefix)
-    
+
     def tokenize_encode(self, text, *args, **kwargs):
         tokens = []
         src_lang = kwargs.pop("src_lang")
         for t, src_language in zip(text, src_lang):
             self.tokenizer.src_lang = src_language
-            tokens.append(self.tokenizer.convert_ids_to_tokens(self.tokenizer.encode(t)))
+            tokens.append(
+                self.tokenizer.convert_ids_to_tokens(self.tokenizer.encode(t))
+            )
         return tokens
-    
+
     def tokenize_decode(self, tokens_out, *args, **kwargs):
         return [
             self.tokenizer.decode(
                 self.tokenizer.convert_tokens_to_ids(tokens_out[i].hypotheses[0][1:]),
-                *args, **kwargs
+                *args,
+                **kwargs,
             )
             for i in range(len(tokens_out))
         ]
 
-    def generate(self, text: Union[str, List[str]], src_lang: Union[str, List[str]], tgt_lang: Union[str, List[str]], *forward_args, **forward_kwds: Any):
+    def generate(
+        self,
+        text: Union[str, List[str]],
+        src_lang: Union[str, List[str]],
+        tgt_lang: Union[str, List[str]],
+        *forward_args,
+        **forward_kwds: Any,
+    ):
         """_summary_
 
         Args:
             text (Union[str, List[str]]): Input texts
             src_lang (Union[str, List[str]]): soruce language of the Input texts
             tgt_lang (Union[str, List[str]]): target language for outputs
             max_batch_size (int, optional): Batch size. Defaults to 0.
@@ -262,62 +306,159 @@
             replace_unknowns (bool, optional): _. Defaults to False.
             callback (_type_, optional): _. Defaults to None.
 
         Returns:
             Union[str, List[str]]: text as output, if list, same len as input
         """
         if not len(text) == len(src_lang) == len(tgt_lang):
-            raise ValueError(f"unequal len: text={len(text)} src_lang={len(src_lang)} tgt_lang={len(tgt_lang)}")
+            raise ValueError(
+                f"unequal len: text={len(text)} src_lang={len(src_lang)} tgt_lang={len(tgt_lang)}"
+            )
         forward_kwds["tgt_lang"] = tgt_lang
-        return super().generate(text, *forward_args, **forward_kwds, encode_kwargs={"src_lang": src_lang})
+        return super().generate(
+            text, *forward_args, **forward_kwds, encode_kwargs={"src_lang": src_lang}
+        )
+
+
+class EncoderCT2fromHfHub(CTranslate2ModelfromHuggingfaceHub):
+    def __init__(
+        self,
+        model_name_or_path: str,
+        device: Literal["cpu", "cuda"] = "cuda",
+        device_index=0,
+        compute_type: Literal["int8_float16", "int8"] = "int8_float16",
+        tokenizer: Union[AutoTokenizer, None] = None,
+        hub_kwargs={},
+        **kwargs: Any,
+    ):
+        """for ctranslate2.Translator models, in particular m2m-100
+
+        Args:
+            model_name_or_path (str): _description_
+            device (Literal[cpu, cuda], optional): _description_. Defaults to "cuda".
+            device_index (int, optional): _description_. Defaults to 0.
+            compute_type (Literal[int8_float16, int8], optional): _description_. Defaults to "int8_float16".
+            tokenizer (Union[AutoTokenizer, None], optional): _description_. Defaults to None.
+            hub_kwargs (dict, optional): _description_. Defaults to {}.
+            **kwargs (Any, optional): Any additional arguments
+        """
+        self.ctranslate_class = ctranslate2.Encoder
+        super().__init__(
+            model_name_or_path,
+            device,
+            device_index,
+            compute_type,
+            tokenizer,
+            hub_kwargs,
+            **kwargs,
+        )
+        self.device = device
+        if device == "cuda":
+            try:
+                import torch
+            except ImportError:
+                raise ValueError(
+                    "decoding storageview on CUDA of encoder requires torch"
+                )
+            self.tensor_decode_method = functools.partial(
+                torch.as_tensor, device=device
+            )
+            self.input_dtype=torch.int32
+        else:
+            try:
+                import numpy as np
+            except ImportError:
+                raise ValueError(
+                    "decoding storageview on CPU of encoder requires numpy"
+                )
+            self.tensor_decode_method = np.asarray
+
+    def _forward(self, features, *args, **kwds):
+        input_ids = features["input_ids"]
+        tokens_out = self.model.forward_batch(input_ids, *args,  **kwds)
+        outputs = dict(
+            pooler_output = self.tensor_decode_method(tokens_out.pooler_output),
+            last_hidden_state = self.tensor_decode_method(tokens_out.last_hidden_state),
+            attention_mask=features["attention_mask"]
+        )
+        return outputs
+
+    def tokenize_encode(self, text, *args, **kwargs):
+        return self.tokenizer(text)
+
+    def tokenize_decode(self, tokens_out, *args, **kwargs):
+        return tokens_out
+
+    def generate(
+        self,
+        text: Union[str, List[str]],
+        encode_tok_kwargs={},
+        decode_tok_kwargs={},
+        *forward_args,
+        **forward_kwds: Any,
+    ):
+        return super().generate(
+            text,
+            encode_kwargs=encode_tok_kwargs,
+            decode_kwargs=decode_tok_kwargs,
+            *forward_args,
+            **forward_kwds,
+        )
+
 
 class GeneratorCT2fromHfHub(CTranslate2ModelfromHuggingfaceHub):
     def __init__(
         self,
         model_name_or_path: str,
         device: Literal["cpu", "cuda"] = "cuda",
         device_index=0,
         compute_type: Literal["int8_float16", "int8"] = "int8_float16",
         tokenizer: Union[AutoTokenizer, None] = None,
         hub_kwargs={},
-        **kwargs: Any
+        **kwargs: Any,
     ):
         """for ctranslate2.Generator models
 
         Args:
             model_name_or_path (str): _description_
-            device (Literal[&quot;cpu&quot;, &quot;cuda&quot;], optional): _description_. Defaults to "cuda".
+            device (Literal[cpu, cuda], optional): _description_. Defaults to "cuda".
             device_index (int, optional): _description_. Defaults to 0.
-            compute_type (Literal[&quot;int8_float16&quot;, &quot;int8&quot;], optional): _description_. Defaults to "int8_float16".
+            compute_type (Literal[int8_float16, int8], optional): _description_. Defaults to "int8_float16".
             tokenizer (Union[AutoTokenizer, None], optional): _description_. Defaults to None.
             hub_kwargs (dict, optional): _description_. Defaults to {}.
             **kwargs (Any, optional): Any additional arguments
         """
         self.ctranslate_class = ctranslate2.Generator
         super().__init__(
             model_name_or_path,
             device,
             device_index,
             compute_type,
             tokenizer,
             hub_kwargs,
-            **kwargs
+            **kwargs,
         )
 
     def _forward(self, *args, **kwds):
         return self.model.generate_batch(*args, **kwds)
-        
+
     def tokenize_decode(self, tokens_out, *args, **kwargs):
         return [
             self.tokenizer.decode(tokens_out[i].sequences_ids[0], *args, **kwargs)
             for i in range(len(tokens_out))
         ]
 
-        
-    def generate(self, text: Union[str, List[str]], encode_tok_kwargs={}, decode_tok_kwargs={},  *forward_args, **forward_kwds: Any):
+    def generate(
+        self,
+        text: Union[str, List[str]],
+        encode_tok_kwargs={},
+        decode_tok_kwargs={},
+        *forward_args,
+        **forward_kwds: Any,
+    ):
         """_summary_
 
         Args:
             text (str | List[str]): Input texts
             encode_tok_kwargs (dict, optional): additional kwargs for tokenizer
             decode_tok_kwargs (dict, optional): additional kwargs for tokenizer
             max_batch_size (int, optional): _. Defaults to 0.
@@ -343,9 +484,14 @@
             min_alternative_expansion_prob (float, optional): _. Defaults to 0.
             sampling_topk (int, optional): _. Defaults to 1.
             sampling_temperature (float, optional): _. Defaults to 1.
 
         Returns:
             str | List[str]: text as output, if list, same len as input
         """
-        return super().generate(text, encode_kwargs=encode_tok_kwargs, decode_kwargs=decode_tok_kwargs,  *forward_args, **forward_kwds)
-    
+        return super().generate(
+            text,
+            encode_kwargs=encode_tok_kwargs,
+            decode_kwargs=decode_tok_kwargs,
+            *forward_args,
+            **forward_kwds,
+        )
```

### Comparing `hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2/util/utils.py` & `hf_hub_ctranslate2-2.11.0/hf_hub_ctranslate2/util/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     allow_patterns = [
         "config.json",
         "model.bin",
         "tokenizer.json",
         "vocabulary.txt",
         "tokenizer_config.json",
         "*ocabulary.txt",
+        "vocab.txt",
     ]
 
     return huggingface_hub.snapshot_download(
         model_name,
         allow_patterns=allow_patterns,
         tqdm_class=_disabled_tqdm,
         **kwargs,
```

### Comparing `hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2.egg-info/PKG-INFO` & `hf_hub_ctranslate2-2.11.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
-Name: hf-hub-ctranslate2
-Version: 2.0.9
+Name: hf_hub_ctranslate2
+Version: 2.11.0
 Summary: Connecting Transfromers on HuggingfaceHub with Ctranslate2 
 Home-page: https://github.com/michaelfeil/hf-hub-ctranslate2
 Author: Michael Feil
 License: MIT
 Project-URL: Bug Tracker, https://github.com/michaelfeil/hf-hub-ctranslate2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
+Provides-Extra: sentence_transformers
 License-File: LICENSE
 
 hf_hub_ctranslate2
 ==============================
 
-Connecting Transfromers on HuggingfaceHub with Ctranslate2 - a small utility for keeping tokenizer and model around Huggingface Hub.
+Connecting Transformers on HuggingfaceHub with Ctranslate2 - a small utility for keeping tokenizer and model around Huggingface Hub.
 
 [![codecov](https://codecov.io/gh/michaelfeil/hf-hub-ctranslate2/branch/main/graph/badge.svg?token=U9VIEFEELS)](https://codecov.io/gh/michaelfeil/hf-hub-ctranslate2)![CI pytest](https://github.com/michaelfeil/hf-hub-ctranslate2/actions/workflows/test_release.yml/badge.svg)
 
 [Read the docs](https://michaelfeil.github.io/hf-hub-ctranslate2/)
 
 <!-- PROJECT SHIELDS -->
 [![Contributors][contributors-shield]][contributors-url]
@@ -27,31 +28,32 @@
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
 [![LinkedIn][linkedin-shield]][linkedin-url]
 
 --------
 ## Usage:
-#### Decoder-only Transformer:
+## Decoder-only Transformer:
 ```python
 # download ctranslate.Generator repos from Huggingface Hub (GPT-J, ..)
 from hf_hub_ctranslate2 import TranslatorCT2fromHfHub, GeneratorCT2fromHfHub
 
 model_name_1="michaelfeil/ct2fast-pythia-160m"
 model = GeneratorCT2fromHfHub(
     # load in int8 on CPU
     model_name_or_path=model_name_1, device="cpu", compute_type="int8"
 )
 outputs = model.generate(
     text=["How do you call a fast Flan-ingo?", "User: How are you doing?"]
     # add arguments specifically to ctranslate2.Generator here
 )
 ```
-#### Encoder-Decoder:
+## Encoder-Decoder:
 ```python
+from hf_hub_ctranslate2 import TranslatorCT2fromHfHub
 # download ctranslate.Translator repos from Huggingface Hub (T5, ..)
 model_name_2 = "michaelfeil/ct2fast-flan-alpaca-base"
 model = TranslatorCT2fromHfHub(
         # load in int8 on CUDA
         model_name_or_path=model_name_2, device="cuda", compute_type="int8_float16"
 )
 outputs = model.generate(
@@ -60,27 +62,60 @@
     min_decoding_length=8,
     max_decoding_length=16,
     max_input_length=512,
     beam_size=3
 )
 print(outputs)
 ```
-#### Encoder-Decoder for multilingual translations (m2m-100):
+## Encoder-Decoder for multilingual translations (m2m-100):
 ```python
+from hf_hub_ctranslate2 import MultiLingualTranslatorCT2fromHfHub
 model = MultiLingualTranslatorCT2fromHfHub(
     model_name_or_path="michaelfeil/ct2fast-m2m100_418M", device="cpu", compute_type="int8",
     tokenizer=AutoTokenizer.from_pretrained(f"facebook/m2m100_418M")
 )
 
 outputs = model.generate(
     ["How do you call a fast Flamingo?", "Wie geht es dir?"],
     src_lang=["en", "de"],
     tgt_lang=["de", "fr"]
 )
 ```
+## Encoder-only Sentence Transformers
+```python
+from hf_hub_ctranslate2 import CT2SentenceTransformer
+model_name_pytorch = "intfloat/e5-small"
+model = CT2SentenceTransformer(
+    model_name_pytorch, compute_type="int8", device="cuda", 
+)
+embeddings = model.encode(
+    ["I like soccer", "I like tennis", "The eiffel tower is in Paris"],
+    batch_size=32,
+    convert_to_numpy=True,
+    normalize_embeddings=True,
+)
+print(embeddings.shape, embeddings)
+scores = (embeddings @ embeddings.T) * 100
+```
+
+## Encoder-only
+```python
+from hf_hub_ctranslate2 import EncoderCT2fromHfHub
+model_name = "michaelfeil/ct2fast-e5-small"
+model = EncoderCT2fromHfHub(
+        # load in int8 on CUDA
+        model_name_or_path=model_name,
+        device="cuda",
+        compute_type="int8_float16",
+)
+outputs = model.generate(
+    text=["I like soccer", "I like tennis", "The eiffel tower is in Paris"],
+    max_length=64,
+)
+```
 
 --------
 ## PYPI Install
 ```bash
 pip install hf-hub-ctranslate2
 ```
 --------
```

### Comparing `hf_hub_ctranslate2-2.0.9/setup.py` & `hf_hub_ctranslate2-2.11.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,13 +31,19 @@
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
     ],
     install_requires=[
-        "ctranslate2>=3.13.0",
+        "ctranslate2>=3.16.0",
         "transformers>=4.28.0",
         "huggingface-hub",
         "typing_extensions",
     ],
+    extras_require={
+        'sentence_transformers': [
+            'sentence_transformers>=2.2.2',
+            'torch'
+        ],
+    },
 )
```

### Comparing `hf_hub_ctranslate2-2.0.9/tests/test_translate.py` & `hf_hub_ctranslate2-2.11.0/tests/test_translate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,80 @@
-from hf_hub_ctranslate2 import TranslatorCT2fromHfHub, GeneratorCT2fromHfHub, MultiLingualTranslatorCT2fromHfHub
+from hf_hub_ctranslate2 import (
+    TranslatorCT2fromHfHub,
+    GeneratorCT2fromHfHub,
+    MultiLingualTranslatorCT2fromHfHub,
+    EncoderCT2fromHfHub,
+)
+
 from hf_hub_ctranslate2.util import utils as _utils
 from transformers import AutoTokenizer
 
 
+def test_encoder(model_name="michaelfeil/ct2fast-e5-small-v2"):
+    model = EncoderCT2fromHfHub(
+        model_name_or_path=model_name, device="cpu", compute_type="int8"
+    )
+
+    embeddings = model.generate(
+        text=["I like soccer", "I like tennis", "The eiffel tower is in Paris"],
+    )['pooler_output']
+    assert len(embeddings) == 3
+    assert len(embeddings[0]) == len(embeddings[1])
+    import numpy as np
+
+    assert isinstance(embeddings, np.ndarray)
+    embeddings_norm = embeddings / (embeddings**2).sum(axis=1, keepdims=True) ** 0.5
+    scores = (embeddings_norm @ embeddings_norm.T) * 100
+    assert 100.05 > scores[0][0] >= 99.95
+    assert scores[0][0] > scores[0][1]
+    assert scores[0][1] > scores[0][2]
+
+    embeddings2 = model.generate(
+        ["I like soccer", "I like tennis", "The eiffel tower is in Paris"],
+    )['pooler_output']
+    assert (embeddings2 == embeddings).all()
+
 def test_translator(model_name="michaelfeil/ct2fast-flan-alpaca-base"):
     model = TranslatorCT2fromHfHub(
         model_name_or_path=model_name, device="cpu", compute_type="int8"
     )
 
     outputs = model.generate(
         ["How do you call a fast Flan-ingo?", "Translate to german: How are you doing?"]
     )
     assert len(outputs) == 2
     assert len(outputs[0]) != len(outputs[1])
     assert "flan" in outputs[0].lower()
     for o in outputs:
         assert isinstance(o, str)
 
+
 def test_multilingualtranslator(model_name="michaelfeil/ct2fast-m2m100_418M"):
     model = MultiLingualTranslatorCT2fromHfHub(
-        model_name_or_path=model_name, device="cpu", compute_type="int8",
-        tokenizer=AutoTokenizer.from_pretrained(f"facebook/{model_name.split('-')[-1]}")
+        model_name_or_path=model_name,
+        device="cpu",
+        compute_type="int8",
+        tokenizer=AutoTokenizer.from_pretrained(
+            f"facebook/{model_name.split('-')[-1]}"
+        ),
     )
 
     outputs = model.generate(
         ["How do you call a fast Flamingo?", "Wie geht es dir?"],
         src_lang=["en", "de"],
-        tgt_lang=["de", "fr"]
+        tgt_lang=["de", "fr"],
     )
     assert len(outputs) == 2
     assert len(outputs[0]) != len(outputs[1])
     assert "nennt" in outputs[0].lower()
     assert "comment" in outputs[1].lower()
     for o in outputs:
         assert isinstance(o, str)
 
+
 def test_generator(model_name="michaelfeil/ct2fast-pythia-160m"):
     model = GeneratorCT2fromHfHub(
         model_name_or_path=model_name, device="cpu", compute_type="int8"
     )
 
     outputs = model.generate(
         ["How do you call a fast Flan-ingo?", "Translate to german: How are you doing?"]
@@ -63,9 +99,8 @@
 
     outputs = model.generate("How do you call a fast Flan-ingo?")
     assert isinstance(outputs, str)
     assert "flan" in outputs.lower()
 
 
 if __name__ == "__main__":
-    test_generator()
-    test_translator()
+    test_encoder()
```

