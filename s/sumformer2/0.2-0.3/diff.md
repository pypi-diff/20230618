# Comparing `tmp/sumformer2-0.2.tar.gz` & `tmp/sumformer2-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sumformer2-0.2.tar", last modified: Sun Jun 18 10:08:41 2023, max compression
+gzip compressed data, was "sumformer2-0.3.tar", last modified: Sun Jun 18 11:22:05 2023, max compression
```

## Comparing `sumformer2-0.2.tar` & `sumformer2-0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-18 10:08:41.748424 sumformer2-0.2/
--rw-r--r--   0 ryan       (501) staff       (20)     1065 2023-06-07 16:24:08.000000 sumformer2-0.2/LICENSE
--rw-r--r--   0 ryan       (501) staff       (20)      210 2023-06-18 10:08:41.748030 sumformer2-0.2/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)       61 2023-06-07 16:24:08.000000 sumformer2-0.2/README.md
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-06-18 10:08:41.748566 sumformer2-0.2/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)      489 2023-06-18 10:07:41.000000 sumformer2-0.2/setup.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-18 10:08:41.743599 sumformer2-0.2/sumformer2/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-06-18 10:03:46.000000 sumformer2-0.2/sumformer2/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)    14712 2023-06-18 09:24:29.000000 sumformer2-0.2/sumformer2/main.py
--rw-r--r--   0 ryan       (501) staff       (20)     8269 2023-06-15 18:12:32.000000 sumformer2-0.2/sumformer2/modules.py
--rw-r--r--   0 ryan       (501) staff       (20)     5888 2023-06-17 19:25:15.000000 sumformer2-0.2/sumformer2/transformer.py
--rw-r--r--   0 ryan       (501) staff       (20)     5819 2023-06-18 09:24:12.000000 sumformer2-0.2/sumformer2/utils.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-18 10:08:41.747182 sumformer2-0.2/sumformer2.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)      210 2023-06-18 10:08:41.000000 sumformer2-0.2/sumformer2.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      342 2023-06-18 10:08:41.000000 sumformer2-0.2/sumformer2.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-06-18 10:08:41.000000 sumformer2-0.2/sumformer2.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)       52 2023-06-18 10:08:41.000000 sumformer2-0.2/sumformer2.egg-info/entry_points.txt
--rw-r--r--   0 ryan       (501) staff       (20)     1140 2023-06-18 10:08:41.000000 sumformer2-0.2/sumformer2.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)       11 2023-06-18 10:08:41.000000 sumformer2-0.2/sumformer2.egg-info/top_level.txt
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-18 11:22:05.578117 sumformer2-0.3/
+-rw-r--r--   0 ryan       (501) staff       (20)     1065 2023-06-07 16:24:08.000000 sumformer2-0.3/LICENSE
+-rw-r--r--   0 ryan       (501) staff       (20)      210 2023-06-18 11:22:05.577660 sumformer2-0.3/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)       61 2023-06-07 16:24:08.000000 sumformer2-0.3/README.md
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-06-18 11:22:05.578316 sumformer2-0.3/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)      490 2023-06-18 11:22:01.000000 sumformer2-0.3/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-18 11:22:05.573523 sumformer2-0.3/sumformer2/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-06-18 10:03:46.000000 sumformer2-0.3/sumformer2/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)    14829 2023-06-18 11:21:28.000000 sumformer2-0.3/sumformer2/main.py
+-rw-r--r--   0 ryan       (501) staff       (20)     8269 2023-06-15 18:12:32.000000 sumformer2-0.3/sumformer2/modules.py
+-rw-r--r--   0 ryan       (501) staff       (20)     5889 2023-06-18 10:37:23.000000 sumformer2-0.3/sumformer2/transformer.py
+-rw-r--r--   0 ryan       (501) staff       (20)     5819 2023-06-18 10:37:43.000000 sumformer2-0.3/sumformer2/utils.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-18 11:22:05.577056 sumformer2-0.3/sumformer2.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)      210 2023-06-18 11:22:05.000000 sumformer2-0.3/sumformer2.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      342 2023-06-18 11:22:05.000000 sumformer2-0.3/sumformer2.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-06-18 11:22:05.000000 sumformer2-0.3/sumformer2.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       53 2023-06-18 11:22:05.000000 sumformer2-0.3/sumformer2.egg-info/entry_points.txt
+-rw-r--r--   0 ryan       (501) staff       (20)     1140 2023-06-18 11:22:05.000000 sumformer2-0.3/sumformer2.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       11 2023-06-18 11:22:05.000000 sumformer2-0.3/sumformer2.egg-info/top_level.txt
```

### Comparing `sumformer2-0.2/LICENSE` & `sumformer2-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sumformer2-0.2/sumformer2/main.py` & `sumformer2-0.3/sumformer2/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 import wandb
 
 from torch.cuda.amp import autocast, GradScaler
 from torch.nn.functional import pad
 from torch.optim import AdamW
 from transformers import T5Tokenizer
 
-from transformer import Sumformer
-from utils import *
+from .transformer import Sumformer
+from .utils import *
 
 
 INTERVAL = 100  # Init logging interval
 MIN_INPUT_LEN = 50
 MAX_INPUT_LEN = 256
 
 
-def main(train=True, test=False, epochs=1, batch_size=8, lr=3.4e-4, sched="warmup", emb_dim=512, max_out_len=30, clip=0.0, sample=None, load=None, pos_enc=False, GLU=False, gen="greedy", ignore_pad=False,
-         enc_heads=8, enc_hidden=6, enc_depth=8, enc_dropout=0.4,
-         dec_heads=8, dec_hidden=6, dec_depth=8, dec_dropout=0.4):
+def main(train=True, test=False, epochs=1, batch_size=16, lr=3.4e-4, sched="onecycle", emb_dim=512, max_out_len=30, clip=0.0, sample=None, load=None, pos_enc=False, GLU=False, gen="greedy", ignore_pad=False,
+         enc_heads=8, enc_hidden=6, enc_depth=8, enc_dropout=0.3,
+         dec_heads=8, dec_hidden=6, dec_depth=8, dec_dropout=0.3):
     # Ensure deterministic behavior
     set_seed(69420)
 
     best_val_loss = float("inf")  # Init best loss
     running_time = 0.0  # Init throughput measurements
     running_tokens = 0
     
@@ -55,15 +55,20 @@
         "inference_type": gen,
         "ignore_padding": ignore_pad
     })
 
     # Load dataset and prepare DataLoader
     # train_dataset, val_dataset, test_dataset = load_reddit(0.8, 0.1, min_len=MIN_INPUT_LEN)
     train_dataset, val_dataset, test_dataset = load_xsum()
-    print(len(train_dataset))
+    if sample is not None:
+        print(f"Sampling {sample} rows from dataset")
+        train_dataset = train_dataset.select(range(sample))
+        val_dataset = val_dataset.select(range(sample))
+        test_dataset = test_dataset.select(range(sample))
+    print("Number of rows: ", len(train_dataset))
 
     # Init the T5 tokenizer
     tokenizer = setup_tokenizer()
 
     def collate_fn(batch):
         docs = [item['document'] for item in batch]
         summaries = [item['summary'] for item in batch]
@@ -76,19 +81,14 @@
 
         # create attention masks to ignore padding tokens
         encoder_inputs["padding_mask"] = encoder_inputs["input_ids"].ne(tokenizer.pad_token_id)
         decoder_inputs["padding_mask"] = decoder_inputs["input_ids"].ne(tokenizer.pad_token_id)
 
         return encoder_inputs.to(device), decoder_inputs.to(device)
 
-    if sample is not None:
-        train_dataset = train_dataset.select(range(sample))
-        val_dataset = val_dataset.select(range(sample))
-        test_dataset = test_dataset.select(range(sample))
-
     train_loader = create_data_loader(train_dataset, batch_size, collate_fn)
     val_loader = create_data_loader(val_dataset, batch_size, collate_fn)
     test_loader = create_data_loader(test_dataset, batch_size, collate_fn)
     
     # Printing some sample data and padding mask
     # data_iter = iter(train_loader)
     # for i in range(3):
@@ -322,11 +322,15 @@
     with torch.no_grad():
         summary_ids = model.greedy(input_ids, start_token=tokenizer.bos_token_id, end_token=tokenizer.eos_token_id, max_len=max_out_len)
     
     # Return the decoded summary
     return tokenizer.decode(summary_ids[0], skip_special_tokens=True)
 
 
-if __name__ == '__main__':
-    fire.Fire(main)
+# if __name__ == '__main__':
+#     fire.Fire(main)
     # main(train=False, test=True, load="models/fearless-oath-237/model_fearless-oath-237_e0.pt")
-    # main(batch_size=8, sample=48, max_out_len=32, enc_heads=2, dec_heads=4, test=True)
+    # main(batch_size=8, sample=48, max_out_len=32, enc_heads=2, dec_heads=4, test=True)
+
+
+def start():
+    fire.Fire(main)
```

### Comparing `sumformer2-0.2/sumformer2/modules.py` & `sumformer2-0.3/sumformer2/modules.py`

 * *Files identical despite different names*

### Comparing `sumformer2-0.2/sumformer2/transformer.py` & `sumformer2-0.3/sumformer2/transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import torch
 import torch.nn as nn
 
 from torch.utils.checkpoint import checkpoint
 
-from modules import *
+from .modules import *
 
 class Sumformer(nn.Module):
     """Text summarization transformer."""
     def __init__(self, device, emb_dim, vocab_size, max_len, pos_encoding, GLU, enc_heads, enc_hidden, enc_depth, enc_dropout, dec_heads, dec_hidden, dec_depth, dec_dropout):
         super().__init__()
 
         self.device = device
```

### Comparing `sumformer2-0.2/sumformer2/utils.py` & `sumformer2-0.3/sumformer2/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import math
 import os
+import torch
+import wandb
 
 from datasets import load_dataset, concatenate_datasets
-import torch
 from torch.optim import lr_scheduler
 from torch.utils.data import DataLoader, SequentialSampler, BatchSampler
-import wandb
 
 
 def create_data_loader(dataset, batch_size, collate_fn):
     sampler = SequentialSampler(dataset)
     batch_sampler = BatchSampler(sampler, batch_size, drop_last=False)
     return DataLoader(dataset, batch_sampler=batch_sampler, collate_fn=collate_fn)
```

### Comparing `sumformer2-0.2/sumformer2.egg-info/requires.txt` & `sumformer2-0.3/sumformer2.egg-info/requires.txt`

 * *Files identical despite different names*

