# Comparing `tmp/flash-attention-jax-0.2.0.tar.gz` & `tmp/flash-attention-jax-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flash-attention-jax-0.2.0.tar", last modified: Tue Nov  1 18:09:50 2022, max compression
+gzip compressed data, was "flash-attention-jax-0.3.0.tar", last modified: Sun Jun 18 17:53:40 2023, max compression
```

## Comparing `flash-attention-jax-0.2.0.tar` & `flash-attention-jax-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 18:09:50.936452 flash-attention-jax-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-11-01 18:09:34.000000 flash-attention-jax-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      630 2022-11-01 18:09:50.936452 flash-attention-jax-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2646 2022-11-01 18:09:34.000000 flash-attention-jax-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 18:09:50.936452 flash-attention-jax-0.2.0/flash_attention_jax/
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-11-01 18:09:34.000000 flash-attention-jax-0.2.0/flash_attention_jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1424 2022-11-01 18:09:34.000000 flash-attention-jax-0.2.0/flash_attention_jax/attention.py
--rw-r--r--   0 runner    (1001) docker     (121)     6505 2022-11-01 18:09:34.000000 flash-attention-jax-0.2.0/flash_attention_jax/causal_flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (121)     5822 2022-11-01 18:09:34.000000 flash-attention-jax-0.2.0/flash_attention_jax/cosine_sim_flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (121)     6715 2022-11-01 18:09:34.000000 flash-attention-jax-0.2.0/flash_attention_jax/flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (121)     2174 2022-11-01 18:09:34.000000 flash-attention-jax-0.2.0/flash_attention_jax/rabe_attention.py
--rw-r--r--   0 runner    (1001) docker     (121)     1348 2022-11-01 18:09:34.000000 flash-attention-jax-0.2.0/flash_attention_jax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 18:09:50.936452 flash-attention-jax-0.2.0/flash_attention_jax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      630 2022-11-01 18:09:50.000000 flash-attention-jax-0.2.0/flash_attention_jax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-11-01 18:09:50.000000 flash-attention-jax-0.2.0/flash_attention_jax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 18:09:50.000000 flash-attention-jax-0.2.0/flash_attention_jax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-11-01 18:09:50.000000 flash-attention-jax-0.2.0/flash_attention_jax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-11-01 18:09:50.000000 flash-attention-jax-0.2.0/flash_attention_jax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 18:09:50.936452 flash-attention-jax-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      827 2022-11-01 18:09:34.000000 flash-attention-jax-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:53:40.365268 flash-attention-jax-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-18 17:53:27.000000 flash-attention-jax-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-18 17:53:40.365268 flash-attention-jax-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-18 17:53:27.000000 flash-attention-jax-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:53:40.365268 flash-attention-jax-0.3.0/flash_attention_jax/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-18 17:53:27.000000 flash-attention-jax-0.3.0/flash_attention_jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-18 17:53:27.000000 flash-attention-jax-0.3.0/flash_attention_jax/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-06-18 17:53:27.000000 flash-attention-jax-0.3.0/flash_attention_jax/causal_flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-06-18 17:53:27.000000 flash-attention-jax-0.3.0/flash_attention_jax/cosine_sim_flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-06-18 17:53:27.000000 flash-attention-jax-0.3.0/flash_attention_jax/flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-18 17:53:27.000000 flash-attention-jax-0.3.0/flash_attention_jax/rabe_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-18 17:53:27.000000 flash-attention-jax-0.3.0/flash_attention_jax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:53:40.365268 flash-attention-jax-0.3.0/flash_attention_jax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-18 17:53:40.000000 flash-attention-jax-0.3.0/flash_attention_jax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-18 17:53:40.000000 flash-attention-jax-0.3.0/flash_attention_jax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 17:53:40.000000 flash-attention-jax-0.3.0/flash_attention_jax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 17:53:40.000000 flash-attention-jax-0.3.0/flash_attention_jax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-18 17:53:40.000000 flash-attention-jax-0.3.0/flash_attention_jax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 17:53:40.365268 flash-attention-jax-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-18 17:53:27.000000 flash-attention-jax-0.3.0/setup.py
```

### Comparing `flash-attention-jax-0.2.0/LICENSE` & `flash-attention-jax-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flash-attention-jax-0.2.0/PKG-INFO` & `flash-attention-jax-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flash-attention-jax
-Version: 0.2.0
+Version: 0.3.0
 Summary: Flash Attention - in Jax
 Home-page: https://github.com/lucidrains/flash-attention-jax
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,jax
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flash-attention-jax-0.2.0/README.md` & `flash-attention-jax-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -62,18 +62,19 @@
 out, _ = causal_flash_attention(q, k, v)
 
 out.shape  # (131072, 512)
 ```
 
 ## Todo
 
+- [x] leading dimensions for causal flash attention variant
+
 - [ ] figure out issue with jit and static argnums
 - [ ] comment with references to paper algorithms and explanations
 - [ ] make sure it can work one-headed key / values, as in PaLM
-- [ ] leading dimensions for causal flash attention variant
 
 ## Citations
 
 ```bibtex
 @article{Dao2022FlashAttentionFA,
     title   = {FlashAttention: Fast and Memory-Efficient Exact Attention with IO-Awareness},
     author  = {Tri Dao and Daniel Y. Fu and Stefano Ermon and Atri Rudra and Christopher R'e},
```

#### html2text {}

```diff
@@ -15,18 +15,18 @@
 ('shows differences between normal and flash attention for output, dq, dk, dv')
 print(f'o: {diff}') # < 1e-4 print(f'dq: {dq_diff}') # < 1e-6 print(f'dk:
 {dk_diff}') # < 1e-6 print(f'dv: {dv_diff}') # < 1e-6 ``` Autoregressive Flash
 Attention - GPT-like decoder attention ```python from jax import random from
 flash_attention_jax import causal_flash_attention rng_key = random.PRNGKey(42)
 q = random.normal(rng_key, (131072, 512)) k = random.normal(rng_key, (131072,
 512)) v = random.normal(rng_key, (131072, 512)) out, _ = causal_flash_attention
-(q, k, v) out.shape # (131072, 512) ``` ## Todo - [ ] figure out issue with jit
-and static argnums - [ ] comment with references to paper algorithms and
-explanations - [ ] make sure it can work one-headed key / values, as in PaLM -
-[ ] leading dimensions for causal flash attention variant ## Citations
+(q, k, v) out.shape # (131072, 512) ``` ## Todo - [x] leading dimensions for
+causal flash attention variant - [ ] figure out issue with jit and static
+argnums - [ ] comment with references to paper algorithms and explanations -
+[ ] make sure it can work one-headed key / values, as in PaLM ## Citations
 ```bibtex @article{Dao2022FlashAttentionFA, title = {FlashAttention: Fast and
 Memory-Efficient Exact Attention with IO-Awareness}, author = {Tri Dao and
 Daniel Y. Fu and Stefano Ermon and Atri Rudra and Christopher R'e}, journal =
 {ArXiv}, year = {2022}, volume = {abs/2205.14135} } ``` ```bibtex @article
 {Rabe2021SelfattentionDN, title = {Self-attention Does Not Need O(n2) Memory},
 author = {Markus N. Rabe and Charles Staats}, journal = {ArXiv}, year = {2021},
 volume = {abs/2112.05682} } ```
```

### Comparing `flash-attention-jax-0.2.0/flash_attention_jax/attention.py` & `flash-attention-jax-0.3.0/flash_attention_jax/attention.py`

 * *Files identical despite different names*

### Comparing `flash-attention-jax-0.2.0/flash_attention_jax/causal_flash_attention.py` & `flash-attention-jax-0.3.0/flash_attention_jax/causal_flash_attention.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,189 +1,206 @@
 import math
 import jax
 from functools import partial
 from jax import nn
 from jax import custom_vjp
 from jax import numpy as jnp, lax, jit
+from jax.numpy import einsum
+
+from einops import rearrange
 
 # constants
 
 EPSILON = 1e-10
 MASK_VALUE = -1e10
 
 Q_CHUNK_SIZE = 1024
 K_CHUNK_SIZE = 1024
 
 # flash attention
 
 def _query_chunk_flash_attention(q_range_chunk, k_range, q, k, v):
-    q_len, k_len, dim, v_dim = q.shape[-2], *k.shape, v.shape[-1]
+    q_len, k_len, bh, dim, v_dim = q.shape[0], *k.shape, v.shape[-1]
     scale = 1 / jnp.sqrt(dim)
     q_scaled  = q * scale
 
     def chunk_scanner(carries, _):
         key_chunk_idx, out, row_sum, row_max = carries
         k_chunk_sizes = min(K_CHUNK_SIZE, k_len)
 
-        k_chunk = lax.dynamic_slice(k, (key_chunk_idx, 0), slice_sizes=(k_chunk_sizes, dim))
-        v_chunk = lax.dynamic_slice(v, (key_chunk_idx, 0), slice_sizes=(k_chunk_sizes, v_dim))
+        k_chunk = lax.dynamic_slice(k, (key_chunk_idx, 0, 0), slice_sizes=(k_chunk_sizes, bh, dim))
+        v_chunk = lax.dynamic_slice(v, (key_chunk_idx, 0, 0), slice_sizes=(k_chunk_sizes, bh, v_dim))
 
         k_range_chunk = lax.dynamic_slice(k_range, (0, key_chunk_idx), slice_sizes=(1, k_chunk_sizes))
 
         causal_mask = q_range_chunk < k_range_chunk
 
-        attn_weights = q_scaled @ k_chunk.transpose()
+        attn_weights = einsum('i ... d, j ... d -> i ... j', q_scaled, k_chunk)
 
+        causal_mask = rearrange(causal_mask, 'i j -> i 1 j')
         attn_weights = jnp.where(causal_mask, MASK_VALUE, attn_weights)
 
         block_row_max = jnp.max(attn_weights, axis = -1, keepdims = True)
 
         exp_weights = jnp.exp(attn_weights - block_row_max)
 
         exp_weights = jnp.where(causal_mask, 0., exp_weights)
 
         block_row_sum = jnp.sum(exp_weights, axis = -1, keepdims = True) + EPSILON
 
-        exp_values = exp_weights @ v_chunk
+        exp_values = einsum('i ... j, j ... d -> i ... d', exp_weights, v_chunk)
 
         new_row_max = jnp.maximum(block_row_max, row_max)
 
         exp_row_max_diff = jnp.exp(row_max - new_row_max)
         exp_block_row_max_diff = jnp.exp(block_row_max - new_row_max)
 
         new_row_sum = exp_row_max_diff * row_sum + exp_block_row_max_diff * block_row_sum
 
         out = (row_sum / new_row_sum) * exp_row_max_diff * out + \
               (exp_block_row_max_diff / new_row_sum) * exp_values
 
         return (key_chunk_idx + k_chunk_sizes, out, new_row_sum, new_row_max), None
 
-    out = jnp.zeros((q_len, dim))
-    row_sum = jnp.zeros((q_len, 1))
-    row_max = jnp.ones((q_len, 1)) * -1e6
+    out = jnp.zeros((q_len, bh, dim))
+    row_sum = jnp.zeros((q_len, bh, 1))
+    row_max = jnp.ones((q_len, bh, 1)) * -1e6
 
     (_, out, row_sum, row_max), _ = lax.scan(chunk_scanner, init = (0, out, row_sum, row_max), xs = None, length = math.ceil(k_len / K_CHUNK_SIZE))
 
-    out = out.reshape(q_len, v_dim)
-    row_sum = row_sum.reshape(q_len)
-    row_max = row_max.reshape(q_len)
+    out = out.reshape(q_len, bh, v_dim)
+    row_sum = row_sum.reshape(q_len, bh)
+    row_max = row_max.reshape(q_len, bh)
 
     return out, row_sum, row_max
 
 def _causal_flash_attention(q, k, v):
-    q_len, dim, k_len, v_dim = *q.shape, *v.shape
+    batch, heads, q_len, dim, k_len, v_dim = *q.shape, *v.shape[-2:]
+
+    bh = batch * heads
+
+    q, k, v = map(lambda t: rearrange(t, 'b h n d -> n (b h) d'), (q, k, v))
 
     q_range = jnp.arange(q_len).reshape(q_len, 1) + (k_len - q_len)
     k_range = jnp.arange(k_len).reshape(1, k_len)
 
     def chunk_scanner(chunk_idx, _):
         chunk_sizes = min(Q_CHUNK_SIZE, q_len)
 
-        q_chunk = lax.dynamic_slice(q, (chunk_idx, 0), slice_sizes = (chunk_sizes, dim))
+        q_chunk = lax.dynamic_slice(q, (chunk_idx, 0, 0), slice_sizes = (chunk_sizes, bh, dim))
         q_range_chunk = lax.dynamic_slice(q_range, (chunk_idx, 0), slice_sizes = (chunk_sizes, 1))
 
         return (chunk_idx + chunk_sizes, _query_chunk_flash_attention(q_range_chunk, k_range, q_chunk, k, v))
 
     _, (out, row_sum, row_max) = lax.scan(chunk_scanner, init = 0, xs = None, length = math.ceil(q_len / Q_CHUNK_SIZE))
 
-    out = out.reshape(q_len, v_dim)
-    row_sum = row_sum.reshape(q_len)
-    row_max = row_max.reshape(q_len)
+    out = out.reshape(q_len, bh, v_dim)
+    row_sum = row_sum.reshape(q_len, bh)
+    row_max = row_max.reshape(q_len, bh)
 
+    out = rearrange(out, 'n (b h) d -> b h n d', b = batch)
     return out, (row_sum, row_max)
 
 @custom_vjp
+@jit
 def causal_flash_attention(q, k, v):
   out, _ = _causal_flash_attention(q, k, v)
   return out
 
 @jit
 def flash_attention_forward(q, k, v):
     out, (row_sum, row_max) = _causal_flash_attention(q, k, v)
     return out, (q, k, v, out, row_sum, row_max)
 
 def _query_chunk_flash_attention_backward(query_range_chunk, key_range, q, k, v, o, do, l, m):
-    q_len, dim, k_len, v_dim = *q.shape, *v.shape
+    q_len, bh, dim, k_len, _, v_dim = *q.shape, *v.shape
 
     scale = 1 / jnp.sqrt(dim)
     q_scaled = q * scale
 
     def chunk_scanner(carries, _):
         key_chunk_idx, dq = carries
         k_chunk_sizes = min(K_CHUNK_SIZE, k_len)
 
-        k_chunk = lax.dynamic_slice(k, (key_chunk_idx, 0), slice_sizes=(k_chunk_sizes, dim))
-        v_chunk = lax.dynamic_slice(v, (key_chunk_idx, 0), slice_sizes=(k_chunk_sizes, v_dim))
+        k_chunk = lax.dynamic_slice(k, (key_chunk_idx, 0, 0), slice_sizes=(k_chunk_sizes, bh, dim))
+        v_chunk = lax.dynamic_slice(v, (key_chunk_idx, 0, 0), slice_sizes=(k_chunk_sizes, bh, v_dim))
 
         key_range_chunk = lax.dynamic_slice(key_range, (0, key_chunk_idx), slice_sizes=(1, k_chunk_sizes))
 
         causal_mask = query_range_chunk < key_range_chunk
 
-        attn_weights = q_scaled @ k_chunk.transpose()
+        attn_weights = einsum('i ... d, j ... d -> i ... j', q_scaled, k_chunk)
 
+        causal_mask = rearrange(causal_mask, 'i j -> i 1 j')
         attn_weights = jnp.where(causal_mask, MASK_VALUE, attn_weights)
 
         exp_attn_weights = jnp.exp(attn_weights - m)
 
         exp_attn_weights = jnp.where(causal_mask, 0., exp_attn_weights)
 
         p = exp_attn_weights / l
 
-        dv_chunk = p.transpose() @ do
-        dp = do @ v_chunk.transpose()
+        dv_chunk = einsum('i ... j, i ... d -> j ... d', p, do)
+        dp = einsum('i ... d, j ... d -> i ... j', do, v_chunk)
 
         D = jnp.sum(do * o, axis = -1, keepdims = True)
         ds = p * scale * (dp - D)
 
-        dq_chunk = ds @ k_chunk
-        dk_chunk = ds.transpose() @ q
+        dq_chunk = einsum('i ... j, j ... d -> i ... d', ds, k_chunk)
+        dk_chunk = einsum('i ... j, i ... d -> j ... d', ds, q)
 
         return (key_chunk_idx + k_chunk_sizes, dq + dq_chunk), (dk_chunk, dv_chunk)
 
     dq = jnp.zeros_like(q)
 
     (_, dq), (dk, dv) = lax.scan(chunk_scanner, init = (0, dq), xs = None, length = math.ceil(k_len / K_CHUNK_SIZE))
 
-    dq = dq.reshape(q_len, dim)
-    dk = dk.reshape(k_len, v_dim)
-    dv = dv.reshape(k_len, v_dim)
+    dq = dq.reshape(q_len, bh, dim)
+    dk = dk.reshape(k_len, bh, v_dim)
+    dv = dv.reshape(k_len, bh, v_dim)
 
     return dq, dk, dv
 
 @jit
 def flash_attention_backward(res, do):
     q, k, v, o, l, m = res
 
-    q_len, dim, k_len, v_dim = *q.shape, *v.shape
+    batch, heads, q_len, dim, k_len, v_dim = *q.shape, *v.shape[-2:]
+
+    bh = batch * heads
+
+    m = m.reshape(q_len, bh, 1)
+    l = l.reshape(q_len, bh, 1)
+
+    q, k, v, o, do = map(lambda t: rearrange(t, 'b h n d -> n (b h) d'), (q, k, v, o, do))
 
     dk = jnp.zeros_like(k)
     dv = jnp.zeros_like(v)
 
-    m = m.reshape(q_len, 1)
-    l = l.reshape(q_len, 1)
-
     q_range = jnp.arange(q_len).reshape(q_len, 1) + (k_len - q_len)
     k_range = jnp.arange(k_len).reshape(1, k_len)
 
     def chunk_scanner(carries, _):
         chunk_idx, dk, dv = carries
 
         chunk_sizes = min(Q_CHUNK_SIZE, q_len)
 
-        q_chunk = lax.dynamic_slice(q, (chunk_idx, 0), slice_sizes = (chunk_sizes, q.shape[-1]))
+        q_chunk = lax.dynamic_slice(q, (chunk_idx, 0, 0), slice_sizes = (chunk_sizes, bh, q.shape[-1]))
         q_range_chunk = lax.dynamic_slice(q_range, (chunk_idx, 0), slice_sizes = (chunk_sizes, 1))
 
-        m_chunk = lax.dynamic_slice(m, (chunk_idx, 0), slice_sizes = (chunk_sizes, 1))
-        l_chunk = lax.dynamic_slice(l, (chunk_idx, 0), slice_sizes = (chunk_sizes, 1))
-        o_chunk = lax.dynamic_slice(o, (chunk_idx, 0), slice_sizes = (chunk_sizes, o.shape[-1]))
-        do_chunk = lax.dynamic_slice(do, (chunk_idx, 0), slice_sizes = (chunk_sizes, do.shape[-1]))
+        m_chunk = lax.dynamic_slice(m, (chunk_idx, 0, 0), slice_sizes = (chunk_sizes, bh, 1))
+        l_chunk = lax.dynamic_slice(l, (chunk_idx, 0, 0), slice_sizes = (chunk_sizes, bh, 1))
+        o_chunk = lax.dynamic_slice(o, (chunk_idx, 0, 0), slice_sizes = (chunk_sizes, bh, o.shape[-1]))
+        do_chunk = lax.dynamic_slice(do, (chunk_idx, 0, 0), slice_sizes = (chunk_sizes, bh, do.shape[-1]))
 
         dq_chunk, dk_chunk, dv_chunk = _query_chunk_flash_attention_backward(q_range_chunk, k_range, q_chunk, k, v, o_chunk, do_chunk, l_chunk, m_chunk)
         return (chunk_idx + chunk_sizes, dk + dk_chunk, dv + dv_chunk), dq_chunk
 
     (_, dk, dv), dq = lax.scan(chunk_scanner, init = (0, dk, dv), xs = None, length = math.ceil(q_len / Q_CHUNK_SIZE))
 
-    dq = dq.reshape(q_len, dim)
+    dq = dq.reshape(q_len, bh, dim)
+
+    dq, dk, dv = map(lambda t: rearrange(t, 'n (b h) d -> b h n d', b = batch), (dq, dk, dv))
 
     return dq, dk, dv
 
 causal_flash_attention.defvjp(flash_attention_forward, flash_attention_backward)
```

### Comparing `flash-attention-jax-0.2.0/flash_attention_jax/cosine_sim_flash_attention.py` & `flash-attention-jax-0.3.0/flash_attention_jax/cosine_sim_flash_attention.py`

 * *Files identical despite different names*

### Comparing `flash-attention-jax-0.2.0/flash_attention_jax/flash_attention.py` & `flash-attention-jax-0.3.0/flash_attention_jax/flash_attention.py`

 * *Files identical despite different names*

### Comparing `flash-attention-jax-0.2.0/flash_attention_jax/rabe_attention.py` & `flash-attention-jax-0.3.0/flash_attention_jax/rabe_attention.py`

 * *Files identical despite different names*

### Comparing `flash-attention-jax-0.2.0/flash_attention_jax/utils.py` & `flash-attention-jax-0.3.0/flash_attention_jax/utils.py`

 * *Files identical despite different names*

### Comparing `flash-attention-jax-0.2.0/flash_attention_jax.egg-info/PKG-INFO` & `flash-attention-jax-0.3.0/flash_attention_jax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flash-attention-jax
-Version: 0.2.0
+Version: 0.3.0
 Summary: Flash Attention - in Jax
 Home-page: https://github.com/lucidrains/flash-attention-jax
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,jax
 Classifier: Development Status :: 4 - Beta
```

