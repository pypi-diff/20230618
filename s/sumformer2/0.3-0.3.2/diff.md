# Comparing `tmp/sumformer2-0.3.tar.gz` & `tmp/sumformer2-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sumformer2-0.3.tar", last modified: Sun Jun 18 11:22:05 2023, max compression
+gzip compressed data, was "sumformer2-0.3.2.tar", last modified: Sun Jun 18 17:35:52 2023, max compression
```

## Comparing `sumformer2-0.3.tar` & `sumformer2-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-18 11:22:05.578117 sumformer2-0.3/
--rw-r--r--   0 ryan       (501) staff       (20)     1065 2023-06-07 16:24:08.000000 sumformer2-0.3/LICENSE
--rw-r--r--   0 ryan       (501) staff       (20)      210 2023-06-18 11:22:05.577660 sumformer2-0.3/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)       61 2023-06-07 16:24:08.000000 sumformer2-0.3/README.md
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-06-18 11:22:05.578316 sumformer2-0.3/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)      490 2023-06-18 11:22:01.000000 sumformer2-0.3/setup.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-18 11:22:05.573523 sumformer2-0.3/sumformer2/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-06-18 10:03:46.000000 sumformer2-0.3/sumformer2/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)    14829 2023-06-18 11:21:28.000000 sumformer2-0.3/sumformer2/main.py
--rw-r--r--   0 ryan       (501) staff       (20)     8269 2023-06-15 18:12:32.000000 sumformer2-0.3/sumformer2/modules.py
--rw-r--r--   0 ryan       (501) staff       (20)     5889 2023-06-18 10:37:23.000000 sumformer2-0.3/sumformer2/transformer.py
--rw-r--r--   0 ryan       (501) staff       (20)     5819 2023-06-18 10:37:43.000000 sumformer2-0.3/sumformer2/utils.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-18 11:22:05.577056 sumformer2-0.3/sumformer2.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)      210 2023-06-18 11:22:05.000000 sumformer2-0.3/sumformer2.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      342 2023-06-18 11:22:05.000000 sumformer2-0.3/sumformer2.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-06-18 11:22:05.000000 sumformer2-0.3/sumformer2.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)       53 2023-06-18 11:22:05.000000 sumformer2-0.3/sumformer2.egg-info/entry_points.txt
--rw-r--r--   0 ryan       (501) staff       (20)     1140 2023-06-18 11:22:05.000000 sumformer2-0.3/sumformer2.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)       11 2023-06-18 11:22:05.000000 sumformer2-0.3/sumformer2.egg-info/top_level.txt
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-18 17:35:52.988746 sumformer2-0.3.2/
+-rw-r--r--   0 ryan       (501) staff       (20)     1065 2023-06-07 16:24:08.000000 sumformer2-0.3.2/LICENSE
+-rw-r--r--   0 ryan       (501) staff       (20)      212 2023-06-18 17:35:52.988103 sumformer2-0.3.2/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)       61 2023-06-07 16:24:08.000000 sumformer2-0.3.2/README.md
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-06-18 17:35:52.988980 sumformer2-0.3.2/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)      492 2023-06-18 17:35:39.000000 sumformer2-0.3.2/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-18 17:35:52.983643 sumformer2-0.3.2/sumformer2/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-06-18 10:03:46.000000 sumformer2-0.3.2/sumformer2/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)    14680 2023-06-18 17:19:05.000000 sumformer2-0.3.2/sumformer2/main.py
+-rw-r--r--   0 ryan       (501) staff       (20)     8921 2023-06-18 14:27:38.000000 sumformer2-0.3.2/sumformer2/modules.py
+-rw-r--r--   0 ryan       (501) staff       (20)     5889 2023-06-18 14:29:22.000000 sumformer2-0.3.2/sumformer2/transformer.py
+-rw-r--r--   0 ryan       (501) staff       (20)     5820 2023-06-18 17:10:08.000000 sumformer2-0.3.2/sumformer2/utils.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-18 17:35:52.987219 sumformer2-0.3.2/sumformer2.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)      212 2023-06-18 17:35:52.000000 sumformer2-0.3.2/sumformer2.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      342 2023-06-18 17:35:52.000000 sumformer2-0.3.2/sumformer2.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-06-18 17:35:52.000000 sumformer2-0.3.2/sumformer2.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       53 2023-06-18 17:35:52.000000 sumformer2-0.3.2/sumformer2.egg-info/entry_points.txt
+-rw-r--r--   0 ryan       (501) staff       (20)     1459 2023-06-18 17:35:52.000000 sumformer2-0.3.2/sumformer2.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       11 2023-06-18 17:35:52.000000 sumformer2-0.3.2/sumformer2.egg-info/top_level.txt
```

### Comparing `sumformer2-0.3/LICENSE` & `sumformer2-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sumformer2-0.3/sumformer2/main.py` & `sumformer2-0.3.2/sumformer2/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 import random
 import time
 import fire
 import numpy as np
 import torch
 import wandb
 
+from bert_score import BERTScorer
+from rouge import Rouge
 from torch.cuda.amp import autocast, GradScaler
 from torch.nn.functional import pad
 from torch.optim import AdamW
 from transformers import T5Tokenizer
 
 from .transformer import Sumformer
 from .utils import *
 
 
 INTERVAL = 100  # Init logging interval
 MIN_INPUT_LEN = 50
-MAX_INPUT_LEN = 256
+MAX_INPUT_LEN = 512
 
 
-def main(train=True, test=False, epochs=1, batch_size=16, lr=3.4e-4, sched="onecycle", emb_dim=512, max_out_len=30, clip=0.0, sample=None, load=None, pos_enc=False, GLU=False, gen="greedy", ignore_pad=False,
+def main(train=True, test=False, epochs=6, batch_size=24, lr=3.4e-4, sched="onecycle", emb_dim=512, max_out_len=30, clip=0.0, sample=None, load=None, pos_enc=False, GLU=False, norm="post", gen="greedy", ignore_pad=False,
          enc_heads=8, enc_hidden=6, enc_depth=8, enc_dropout=0.3,
          dec_heads=8, dec_hidden=6, dec_depth=8, dec_dropout=0.3):
     # Ensure deterministic behavior
     set_seed(69420)
 
     best_val_loss = float("inf")  # Init best loss
+    best_val_model_path = None
+    best_model = None
     running_time = 0.0  # Init throughput measurements
     running_tokens = 0
     
     device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
     print(f'Using device "{device}"')
 
     # Initialize wandb
@@ -48,14 +52,15 @@
         "dec_hidden": dec_hidden,
         "dec_depth": dec_depth,
         "dec_dropout": dec_dropout,
         "schedule": sched,
         "clip": clip,
         "pos_enc": pos_enc,
         "GLU": GLU,
+        "norm": norm,
         "inference_type": gen,
         "ignore_padding": ignore_pad
     })
 
     # Load dataset and prepare DataLoader
     # train_dataset, val_dataset, test_dataset = load_reddit(0.8, 0.1, min_len=MIN_INPUT_LEN)
     train_dataset, val_dataset, test_dataset = load_xsum()
@@ -84,31 +89,19 @@
         decoder_inputs["padding_mask"] = decoder_inputs["input_ids"].ne(tokenizer.pad_token_id)
 
         return encoder_inputs.to(device), decoder_inputs.to(device)
 
     train_loader = create_data_loader(train_dataset, batch_size, collate_fn)
     val_loader = create_data_loader(val_dataset, batch_size, collate_fn)
     test_loader = create_data_loader(test_dataset, batch_size, collate_fn)
-    
-    # Printing some sample data and padding mask
-    # data_iter = iter(train_loader)
-    # for i in range(3):
-    #     encoder_inputs, decoder_inputs = next(data_iter)
-    #     print(f"Encoder inputs shape: {encoder_inputs['input_ids'].shape}")
-    #     first_doc = encoder_inputs["input_ids"][0]
-    #     print(f"First doc: {first_doc}")
-    #     first_doc_mask = encoder_inputs["padding_mask"][0]
-    #     print(f"First doc mask: {first_doc_mask}")
-    #     first_doc_decoded = tokenizer.decode(first_doc)
-    #     print(f"First doc decoded: {first_doc_decoded}")
 
     scaler = GradScaler()  # Init gradient scaler for mixed precision training
 
     if train:
-        model = Sumformer(device, emb_dim, len(tokenizer.get_vocab()), max(MAX_INPUT_LEN, max_out_len), pos_enc, GLU, enc_heads, enc_hidden, enc_depth, enc_dropout, dec_heads, dec_hidden, dec_depth, dec_dropout).to(device)
+        model = Sumformer(device, emb_dim, len(tokenizer.get_vocab()), max(MAX_INPUT_LEN, max_out_len), pos_enc, GLU, norm, enc_heads, enc_hidden, enc_depth, enc_dropout, dec_heads, dec_hidden, dec_depth, dec_dropout).to(device)
         optimizer = AdamW(model.parameters(), lr)
         criterion = torch.nn.CrossEntropyLoss(ignore_index=tokenizer.pad_token_id if ignore_pad else -100, reduction='mean')  # * see without padding mask in decoder
         scheduler = init_schedule(optimizer, sched, train_loader, lr, epochs, emb_dim)
 
         for epoch in range(epochs):
             # torch.autograd.set_detect_anomaly(True)  # ! REMOVE WHEN NOT NEEDED
             # -----TRAINING-----
@@ -219,62 +212,73 @@
                 model_params = {
                     'device': device,
                     'emb_dim': emb_dim,
                     'vocab_size': tokenizer.vocab_size,
                     'max_len': max(MAX_INPUT_LEN, max_out_len),
                     'pos_encoding': pos_enc,
                     'GLU': GLU,
+                    'norm': norm,
                     'enc_heads': enc_heads,
                     'enc_hidden': enc_hidden,
                     'enc_depth': enc_depth,
                     'enc_dropout': enc_dropout,
                     'dec_heads': dec_heads,
                     'dec_hidden': dec_hidden,
                     'dec_depth': dec_depth,
                     'dec_dropout': dec_dropout
                 }
                 save_best_model(model, epoch, model_params)
-            
-            # Clear CUDA cache
-            torch.cuda.empty_cache()
-    
+                best_model = model
+
     # -----TESTING-----
     if test:
         print("Testing...")
-        if load is not None:  # TODO automatically load the correct params
-            test_model = Sumformer(device, emb_dim, len(tokenizer.get_vocab()), max(MAX_INPUT_LEN, max_out_len), pos_enc, GLU, enc_heads, enc_hidden, enc_depth, enc_dropout, dec_heads, dec_hidden, dec_depth, dec_dropout).to(device)
-            test_model.load_state_dict(torch.load(f"{load}"))
-        else:
-            try:
-                test_model = model
-            except NameError:
-                print("No model to test. Either train a model or load a model with --load <path>")
-                return
 
-        test_model.eval()
-        total_test_loss = 0.0
+        rouge = Rouge()
+        bert_score = BERTScorer(lang="en")
+
+        # Generate summaries for the test set and compare them to the reference summaries
         with torch.no_grad():
+            best_model.eval()
+            all_generated_summaries = []
+            all_reference_summaries = []
             for b_idx, (encoder_inputs, decoder_inputs) in enumerate(test_loader):
-                if gen == "greedy":
-                    test_outputs = test_model.greedy(
-                        encoder_inputs["input_ids"], start_token=tokenizer.bos_token_id, end_token=tokenizer.eos_token_id, max_len=max_out_len)
-                elif gen == "beam":  # ! DOESN'T WORK YET
-                    test_outputs = test_model.beam(encoder_inputs["input_ids"], start_token=tokenizer.bos_token_id, end_token=tokenizer.eos_token_id, max_len=max_out_len, source_mask=None)
-                else:
-                     raise ValueError(f"{gen} is not a valid generation method")
-                generated_text = tokenizer.decode(test_outputs, skip_special_tokens=False)
-                
-                print(f"\nBatch {b_idx+1}")
-                print(f"Generated ids shape: {test_outputs.shape}")
-                print(f"Generated ids: {test_outputs}")
-                print(f"Generated ids decoded: {generated_text}")
-
-        # log the test loss to wandb
-        avg_test_loss = total_test_loss / len(test_loader)
-        wandb.log({"Test Loss": avg_test_loss})
+                generated_outputs = best_model.greedy(encoder_inputs["input_ids"], start_token=tokenizer.bos_token_id, end_token=tokenizer.eos_token_id, max_len=max_out_len)
+                generated_summaries = [tokenizer.decode(g, skip_special_tokens=True) for g in generated_outputs]
+                reference_summaries = [tokenizer.decode(d, skip_special_tokens=True) for d in decoder_inputs["input_ids"]]
+                all_generated_summaries.extend(generated_summaries)
+                all_reference_summaries.extend(reference_summaries)
+
+        # Print an example generated summary and its reference summary
+        print(f"Example generated summary: {all_generated_summaries[5]}")
+        print(f"Example reference summary: {all_reference_summaries[5]}")
+
+        # Calculate and print the Rouge scores
+        rouge_scores = rouge.get_scores(all_generated_summaries, all_reference_summaries, avg=True)
+        for metric, score_dict in rouge_scores.items():
+            f1_score = score_dict['f']
+            wandb.log({f"{metric} F1 Score": f1_score})
+
+        # Print F1 rouge_scores nicely
+        for metric, score_dict in rouge_scores.items():
+            f1_score = score_dict['f']
+            print(f"{metric} F1 Score: {f1_score:.4f}")
+
+        # Calculate and print the BERTScore
+        P, R, F1 = bert_score.score(all_generated_summaries, all_reference_summaries)
+        P_mean = P.mean().item()
+        R_mean = R.mean().item()
+        F1_mean = F1.mean().item()
+        print(f"BERTScore Precision: {P_mean}")
+        print(f"BERTScore Recall: {R_mean}")
+        print(f"BERTScore F1: {F1_mean}")
+
+        # Log to wandb
+        wandb.log({"Rouge-1 F1": rouge_scores["rouge-1"]["f"], "BERTScore F1": F1_mean})
+
     
     wandb.finish()
 
 
 def pad_sequences(seq1, seq2, pad_token):
     seq1_len, seq2_len = seq1.size(1), seq2.size(1)
 
@@ -287,15 +291,15 @@
         padding_size = max_seq_len - seq2_len
         seq2 = pad(seq2, pad=(0, padding_size), value=pad_token)
 
     return seq1, seq2
 
 
 def setup_tokenizer():
-    tokenizer = T5Tokenizer.from_pretrained('t5-base', use_fast=True, model_max_length=MAX_INPUT_LEN)
+    tokenizer = T5Tokenizer.from_pretrained('t5-base', use_fast=True, model_max_length=MAX_INPUT_LEN, )
     tokenizer.bos_token = "<s>"
     tokenizer.bos_token_id = tokenizer.convert_tokens_to_ids("<s>")
     tokenizer.add_special_tokens({"bos_token": "<s>"})
 
     return tokenizer
```

### Comparing `sumformer2-0.3/sumformer2/modules.py` & `sumformer2-0.3.2/sumformer2/modules.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         super().__init__()
 
         assert k % heads == 0  # embedding dimension must be divisible by number of heads
         self.k, self.heads, self.mask = k, heads, mask  # mask is a flag to use a look-ahead mask
 
         # computing queries, keys and values in parallel for all heads
         # bias=False so that we can use this as a simple projection
-        self.toQueries = nn.Linear(k, k, bias=False)
+        self.toQueries = nn.Linear(k, k, bias=False)  # * mention that bias is turned off to increase throughput in paper
         self.toKeys = nn.Linear(k, k, bias=False)
         self.toValues = nn.Linear(k, k, bias=False)
 
         self.unifyHeads = nn.Linear(k, k)  # W0 matrix
 
     def forward(self, x, padding_mask=None):
         b, t, e = x.size()
@@ -132,43 +132,48 @@
 
         out = out.transpose(1, 2).contiguous().view(b, t, h * s)
 
         return self.unifyHeads(out)
 
 
 class EncoderBlock(nn.Module):
-    def __init__(self, emb, heads, hidden=4, dropout=0.1, GLU=False):
+    def __init__(self, emb, heads, hidden=4, dropout=0.1, GLU=False, norm="post"):
         super().__init__()
 
         self.attention = MHSelfAttention(emb, heads, mask=False)
 
         self.norm1 = nn.LayerNorm(emb)
         self.norm2 = nn.LayerNorm(emb)
 
         if GLU:  # * test GLU vs FF
             self.ff = GLUlayer(emb, hidden)
         else:
             self.ff = FFLayer(emb, hidden)
-        
+
         self.dropout = nn.Dropout(dropout)
+        self.norm = norm
 
     def forward(self, x, padding_mask=None):
+        if self.norm == "pre":
+            x = self.norm1(x)
         attended = self.attention(x, padding_mask)
         attended = self.dropout(attended)
-        x = self.norm1(x + attended)
+        x = x + attended if self.norm == "pre" else self.norm1(x + attended)
         
+        if self.norm == "pre":
+            x = self.norm2(x)
         fedforward = self.ff(x)
         fedforward = self.dropout(fedforward)
-        x = self.norm2(x + fedforward)
+        x = x + fedforward if self.norm == "pre" else self.norm2(x + fedforward)
         
         return x
 
 
 class DecoderBlock(nn.Module):
-    def __init__(self, emb, heads, hidden=4, dropout=0.1, GLU=False):
+    def __init__(self, emb, heads, hidden=4, dropout=0.1, GLU=False, norm="post"):
         super().__init__()
 
         self.maskedAttention = MHSelfAttention(emb, heads, mask=True)
         self.crossAttention = MHCrossAttention(emb, heads)
 
         self.norm1 = nn.LayerNorm(emb)
         self.norm2 = nn.LayerNorm(emb)
@@ -176,30 +181,38 @@
 
         self.dropout = nn.Dropout(dropout)
 
         if GLU:
             self.ff = GLUlayer(emb, hidden)
         else:
             self.ff = FFLayer(emb, hidden)
-        
+
+        self.norm = norm
     
     def forward(self, x, context, padding_mask=None):
+        if self.norm == "pre":
+            x = self.norm1(x)
         masked_attended = self.maskedAttention(x, padding_mask)
         masked_attended = self.dropout(masked_attended)
-        x = self.norm1(x + masked_attended)
+        x = x + masked_attended if self.norm == "pre" else self.norm1(x + masked_attended)
 
+        if self.norm == "pre":
+            x = self.norm2(x)
         cross_attended = self.crossAttention(x, context, padding_mask)
         cross_attended = self.dropout(cross_attended)
-        x = self.norm2(x + cross_attended)
+        x = x + cross_attended if self.norm == "pre" else self.norm2(x + cross_attended)
 
+        if self.norm == "pre":
+            x = self.norm3(x)
         fedforward = self.ff(x)
         fedforward = self.dropout(fedforward)
-        x = self.norm3(x + fedforward)
+        x = x + fedforward if self.norm == "pre" else self.norm3(x + fedforward)
         
         return x
+
     
 
 class GLUlayer(nn.Module):
     """Gated Linear Unit"""
     def __init__(self, emb_dim, hidden):
         super().__init__()
         self.linear1 = nn.Linear(emb_dim, emb_dim * hidden * 2)
```

### Comparing `sumformer2-0.3/sumformer2/transformer.py` & `sumformer2-0.3.2/sumformer2/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 
 from torch.utils.checkpoint import checkpoint
 
 from .modules import *
 
 class Sumformer(nn.Module):
     """Text summarization transformer."""
-    def __init__(self, device, emb_dim, vocab_size, max_len, pos_encoding, GLU, enc_heads, enc_hidden, enc_depth, enc_dropout, dec_heads, dec_hidden, dec_depth, dec_dropout):
+    def __init__(self, device, emb_dim, vocab_size, max_len, pos_encoding, GLU, norm, enc_heads, enc_hidden, enc_depth, enc_dropout, dec_heads, dec_hidden, dec_depth, dec_dropout):
         super().__init__()
 
         self.device = device
         self.emb_dim = emb_dim
         self.vocab_size = vocab_size
         self.max_len = max_len
-        # self.pos_encoding = pos_encoding
+        self.norm = norm
 
         self.token_embedding = nn.Embedding(num_embeddings=vocab_size, embedding_dim=emb_dim).to(device)
         if pos_encoding:
             self.pos_embedding = self.compute_encodings(max_len, emb_dim).to(device)
         else:
             self.pos_embedding = nn.Embedding(num_embeddings=max_len, embedding_dim=emb_dim).to(device)
 
-        self.encoder = [EncoderBlock(emb_dim, enc_heads, enc_hidden, enc_dropout, GLU) for _ in range(enc_depth)]
+        self.encoder = [EncoderBlock(emb_dim, enc_heads, enc_hidden, enc_dropout, GLU, norm) for _ in range(enc_depth)]
         for module in self.encoder: module.to(device)
-        self.decoder = [DecoderBlock(emb_dim, dec_heads, dec_hidden, dec_dropout, GLU) for _ in range(dec_depth)]
+        self.decoder = [DecoderBlock(emb_dim, dec_heads, dec_hidden, dec_dropout, GLU, norm) for _ in range(dec_depth)]
         for module in self.decoder: module.to(device)
 
         self.toProbs = nn.Linear(emb_dim, vocab_size).to(device)  # convert to probabilities over vocab
 
     def compute_encodings(self, max_len, emb_dim):
         """Initialise positional encodings."""
         pos_encodings = torch.zeros(max_len, emb_dim).float()
```

### Comparing `sumformer2-0.3/sumformer2/utils.py` & `sumformer2-0.3.2/sumformer2/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -114,8 +114,8 @@
     model_path = os.path.join(models_dir, f"model_{wandb.run.name}_e{epoch}.pt")
     model_info = {
         'params': model_params,
         'state_dict': model.state_dict()
     }
     
     torch.save(model_info, model_path)
-    wandb.save(model_path)
+    wandb.save(model_path)
```

### Comparing `sumformer2-0.3/sumformer2.egg-info/requires.txt` & `sumformer2-0.3.2/sumformer2.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,88 @@
 absl-py==1.4.0
 aiohttp==3.8.4
 aiosignal==1.3.1
 appdirs==1.4.4
 async-timeout==4.0.2
 attrs==23.1.0
 bert-score==0.3.13
+bleach==6.0.0
 certifi==2023.5.7
 charset-normalizer==3.1.0
 click==8.1.3
 contourpy==1.1.0
 cycler==0.11.0
 datasets==2.12.0
 dill==0.3.6
 docker-pycreds==0.4.0
 docopt==0.6.2
+docutils==0.20.1
 filelock==3.12.0
 fire==0.5.0
 fonttools==4.40.0
 frozenlist==1.3.3
 fsspec==2023.5.0
 gitdb==4.0.10
 GitPython==3.1.31
 huggingface-hub==0.15.1
 idna==3.4
+importlib-metadata==6.6.0
+jaraco.classes==3.2.3
 Jinja2==3.1.2
 joblib==1.2.0
+keyring==23.13.1
 kiwisolver==1.4.4
+markdown-it-py==3.0.0
 MarkupSafe==2.1.3
 matplotlib==3.7.1
+mdurl==0.1.2
+more-itertools==9.1.0
 mpmath==1.3.0
 multidict==6.0.4
 multiprocess==0.70.14
 networkx==3.1
 nltk==3.8.1
 numpy==1.24.3
 packaging==23.1
 pandas==2.0.2
 pathtools==0.1.2
 Pillow==9.5.0
 pipreqs==0.4.13
+pkginfo==1.9.6
 protobuf==4.23.2
 psutil==5.9.5
 pyarrow==12.0.0
+Pygments==2.15.1
 pyparsing==3.0.9
 python-dateutil==2.8.2
 pytz==2023.3
 PyYAML==6.0
+readme-renderer==37.3
 regex==2023.6.3
 requests==2.31.0
+requests-toolbelt==1.0.0
 responses==0.18.0
+rfc3986==2.0.0
+rich==13.4.2
+rouge==1.0.1
 rouge-score==0.1.2
 sentencepiece==0.1.99
 sentry-sdk==1.25.0
 setproctitle==1.3.2
 six==1.16.0
 smmap==5.0.0
 sympy==1.12
 termcolor==2.3.0
 tokenizers==0.13.3
 torch==2.0.1
 tqdm==4.65.0
 transformers==4.29.2
+twine==4.0.2
 typing_extensions==4.6.3
 tzdata==2023.3
 urllib3==2.0.3
 wandb==0.15.4
+webencodings==0.5.1
 xxhash==3.2.0
 yarg==0.1.9
 yarl==1.9.2
+zipp==3.15.0
```

