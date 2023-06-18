# Comparing `tmp/denoising-diffusion-pytorch-1.6.4.tar.gz` & `tmp/denoising-diffusion-pytorch-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising-diffusion-pytorch-1.6.4.tar", last modified: Sun May 21 15:56:55 2023, max compression
+gzip compressed data, was "denoising-diffusion-pytorch-1.7.0.tar", last modified: Sun Jun 18 18:39:04 2023, max compression
```

## Comparing `denoising-diffusion-pytorch-1.6.4.tar` & `denoising-diffusion-pytorch-1.7.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:56:55.148841 denoising-diffusion-pytorch-1.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-21 15:56:55.148841 denoising-diffusion-pytorch-1.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:56:55.148841 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28589 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    36409 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    30453 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    36394 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:56:55.148841 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-21 15:56:55.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-21 15:56:55.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 15:56:55.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-21 15:56:55.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-21 15:56:55.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 15:56:55.148841 denoising-diffusion-pytorch-1.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:39:04.313675 denoising-diffusion-pytorch-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-18 18:39:04.313675 denoising-diffusion-pytorch-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:39:04.313675 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28415 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36235 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30279 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36221 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21193 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:39:04.313675 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-18 18:39:04.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-18 18:39:04.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 18:39:04.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-18 18:39:04.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-18 18:39:04.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 18:39:04.313675 denoising-diffusion-pytorch-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/setup.py
```

### Comparing `denoising-diffusion-pytorch-1.6.4/LICENSE` & `denoising-diffusion-pytorch-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.4/PKG-INFO` & `denoising-diffusion-pytorch-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.6.4
+Version: 1.7.0
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.6.4/README.md` & `denoising-diffusion-pytorch-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/__init__.py` & `denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,30 +104,27 @@
         weight = self.weight
         mean = reduce(weight, 'o ... -> o 1 1 1', 'mean')
         var = reduce(weight, 'o ... -> o 1 1 1', partial(torch.var, unbiased = False))
         normalized_weight = (weight - mean) * (var + eps).rsqrt()
 
         return F.conv2d(x, normalized_weight, self.bias, self.stride, self.padding, self.dilation, self.groups)
 
-class LayerNorm(nn.Module):
+class RMSNorm(nn.Module):
     def __init__(self, dim):
         super().__init__()
         self.g = nn.Parameter(torch.ones(1, dim, 1, 1))
 
     def forward(self, x):
-        eps = 1e-5 if x.dtype == torch.float32 else 1e-3
-        var = torch.var(x, dim = 1, unbiased = False, keepdim = True)
-        mean = torch.mean(x, dim = 1, keepdim = True)
-        return (x - mean) * (var + eps).rsqrt() * self.g
+        return F.normalize(x, dim = 1) * self.g * (x.shape[1] ** 0.5)
 
 class PreNorm(nn.Module):
     def __init__(self, dim, fn):
         super().__init__()
         self.fn = fn
-        self.norm = LayerNorm(dim)
+        self.norm = RMSNorm(dim)
 
     def forward(self, x):
         x = self.norm(x)
         return self.fn(x)
 
 # sinusoidal positional embeds
 
@@ -216,15 +213,15 @@
         self.scale = dim_head ** -0.5
         self.heads = heads
         hidden_dim = dim_head * heads
         self.to_qkv = nn.Conv2d(dim, hidden_dim * 3, 1, bias = False)
 
         self.to_out = nn.Sequential(
             nn.Conv2d(hidden_dim, dim, 1),
-            LayerNorm(dim)
+            RMSNorm(dim)
         )
 
     def forward(self, x):
         b, c, h, w = x.shape
         qkv = self.to_qkv(x).chunk(3, dim = 1)
         q, k, v = map(lambda t: rearrange(t, 'b (h c) x y -> b h c (x y)', h = self.heads), qkv)
```

### Comparing `denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,30 +109,27 @@
         weight = self.weight
         mean = reduce(weight, 'o ... -> o 1 1 1', 'mean')
         var = reduce(weight, 'o ... -> o 1 1 1', partial(torch.var, unbiased = False))
         normalized_weight = (weight - mean) * (var + eps).rsqrt()
 
         return F.conv2d(x, normalized_weight, self.bias, self.stride, self.padding, self.dilation, self.groups)
 
-class LayerNorm(nn.Module):
+class RMSNorm(nn.Module):
     def __init__(self, dim):
         super().__init__()
         self.g = nn.Parameter(torch.ones(1, dim, 1, 1))
 
     def forward(self, x):
-        eps = 1e-5 if x.dtype == torch.float32 else 1e-3
-        var = torch.var(x, dim = 1, unbiased = False, keepdim = True)
-        mean = torch.mean(x, dim = 1, keepdim = True)
-        return (x - mean) * (var + eps).rsqrt() * self.g
+        return F.normalize(x, dim = 1) * self.g * (x.shape[1] ** 0.5)
 
 class PreNorm(nn.Module):
     def __init__(self, dim, fn):
         super().__init__()
         self.fn = fn
-        self.norm = LayerNorm(dim)
+        self.norm = RMSNorm(dim)
 
     def forward(self, x):
         x = self.norm(x)
         return self.fn(x)
 
 # sinusoidal positional embeds
 
@@ -219,15 +216,15 @@
         self.scale = dim_head ** -0.5
         self.heads = heads
         hidden_dim = dim_head * heads
         self.to_qkv = nn.Conv2d(dim, hidden_dim * 3, 1, bias = False)
 
         self.to_out = nn.Sequential(
             nn.Conv2d(hidden_dim, dim, 1),
-            LayerNorm(dim)
+            RMSNorm(dim)
         )
 
     def forward(self, x):
         b, c, h, w = x.shape
         qkv = self.to_qkv(x).chunk(3, dim = 1)
         q, k, v = map(lambda t: rearrange(t, 'b (h c) x y -> b h c (x y)', h = self.heads), qkv)
```

### Comparing `denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,30 +96,27 @@
         weight = self.weight
         mean = reduce(weight, 'o ... -> o 1 1', 'mean')
         var = reduce(weight, 'o ... -> o 1 1', partial(torch.var, unbiased = False))
         normalized_weight = (weight - mean) * (var + eps).rsqrt()
 
         return F.conv1d(x, normalized_weight, self.bias, self.stride, self.padding, self.dilation, self.groups)
 
-class LayerNorm(nn.Module):
+class RMSNorm(nn.Module):
     def __init__(self, dim):
         super().__init__()
         self.g = nn.Parameter(torch.ones(1, dim, 1))
 
     def forward(self, x):
-        eps = 1e-5 if x.dtype == torch.float32 else 1e-3
-        var = torch.var(x, dim = 1, unbiased = False, keepdim = True)
-        mean = torch.mean(x, dim = 1, keepdim = True)
-        return (x - mean) * (var + eps).rsqrt() * self.g
+        return F.normalize(x, dim = 1) * self.g * (x.shape[1] ** 0.5)
 
 class PreNorm(nn.Module):
     def __init__(self, dim, fn):
         super().__init__()
         self.fn = fn
-        self.norm = LayerNorm(dim)
+        self.norm = RMSNorm(dim)
 
     def forward(self, x):
         x = self.norm(x)
         return self.fn(x)
 
 # sinusoidal positional embeds
 
@@ -206,15 +203,15 @@
         self.scale = dim_head ** -0.5
         self.heads = heads
         hidden_dim = dim_head * heads
         self.to_qkv = nn.Conv1d(dim, hidden_dim * 3, 1, bias = False)
 
         self.to_out = nn.Sequential(
             nn.Conv1d(hidden_dim, dim, 1),
-            LayerNorm(dim)
+            RMSNorm(dim)
         )
 
     def forward(self, x):
         b, c, n = x.shape
         qkv = self.to_qkv(x).chunk(3, dim = 1)
         q, k, v = map(lambda t: rearrange(t, 'b (h c) n -> b h c n', h = self.heads), qkv)
```

### Comparing `denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,30 +104,27 @@
         weight = self.weight
         mean = reduce(weight, 'o ... -> o 1 1 1', 'mean')
         var = reduce(weight, 'o ... -> o 1 1 1', partial(torch.var, unbiased = False))
         normalized_weight = (weight - mean) * (var + eps).rsqrt()
 
         return F.conv2d(x, normalized_weight, self.bias, self.stride, self.padding, self.dilation, self.groups)
 
-class LayerNorm(nn.Module):
+class RMSNorm(nn.Module):
     def __init__(self, dim):
         super().__init__()
         self.g = nn.Parameter(torch.ones(1, dim, 1, 1))
 
     def forward(self, x):
-        eps = 1e-5 if x.dtype == torch.float32 else 1e-3
-        var = torch.var(x, dim = 1, unbiased = False, keepdim = True)
-        mean = torch.mean(x, dim = 1, keepdim = True)
-        return (x - mean) * (var + eps).rsqrt() * self.g
+        return F.normalize(x, dim = 1) * self.g * (x.shape[-1] ** 0.5)
 
 class PreNorm(nn.Module):
     def __init__(self, dim, fn):
         super().__init__()
         self.fn = fn
-        self.norm = LayerNorm(dim)
+        self.norm = RMSNorm(dim)
 
     def forward(self, x):
         x = self.norm(x)
         return self.fn(x)
 
 # sinusoidal positional embeds
 
@@ -214,15 +211,15 @@
         self.scale = dim_head ** -0.5
         self.heads = heads
         hidden_dim = dim_head * heads
         self.to_qkv = nn.Conv2d(dim, hidden_dim * 3, 1, bias = False)
 
         self.to_out = nn.Sequential(
             nn.Conv2d(hidden_dim, dim, 1),
-            LayerNorm(dim)
+            RMSNorm(dim)
         )
 
     def forward(self, x):
         b, c, h, w = x.shape
         qkv = self.to_qkv(x).chunk(3, dim = 1)
         q, k, v = map(lambda t: rearrange(t, 'b (h c) x y -> b h c (x y)', h = self.heads), qkv)
```

### Comparing `denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,30 +79,26 @@
     factor = 2
 ):
     return nn.Sequential(
         Rearrange('b c (h p1) (w p2) -> b (c p1 p2) h w', p1 = factor, p2 = factor),
         nn.Conv2d(dim * (factor ** 2), default(dim_out, dim), 1)
     )
 
-class LayerNorm(nn.Module):
+class RMSNorm(nn.Module):
     def __init__(self, dim, scale = True, normalize_dim = 2):
         super().__init__()
         self.g = nn.Parameter(torch.ones(dim)) if scale else 1
 
         self.scale = scale
         self.normalize_dim = normalize_dim
 
     def forward(self, x):
         normalize_dim = self.normalize_dim
         scale = append_dims(self.g, x.ndim - self.normalize_dim - 1) if self.scale else 1
-
-        eps = 1e-5 if x.dtype == torch.float32 else 1e-3
-        var = torch.var(x, dim = normalize_dim, unbiased = False, keepdim = True)
-        mean = torch.mean(x, dim = normalize_dim, keepdim = True)
-        return (x - mean) * var.clamp(min = eps).rsqrt() * scale
+        return F.normalize(x, dim = normalize_dim) * scale * (x.shape[normalize_dim] ** 0.5)
 
 # sinusoidal positional embeds
 
 class LearnedSinusoidalPosEmb(nn.Module):
     def __init__(self, dim):
         super().__init__()
         assert (dim % 2) == 0
@@ -165,20 +161,20 @@
 class LinearAttention(nn.Module):
     def __init__(self, dim, heads = 4, dim_head = 32):
         super().__init__()
         self.scale = dim_head ** -0.5
         self.heads = heads
         hidden_dim = dim_head * heads
 
-        self.norm = LayerNorm(dim, normalize_dim = 1)
+        self.norm = RMSNorm(dim, normalize_dim = 1)
         self.to_qkv = nn.Conv2d(dim, hidden_dim * 3, 1, bias = False)
 
         self.to_out = nn.Sequential(
             nn.Conv2d(hidden_dim, dim, 1),
-            LayerNorm(dim, normalize_dim = 1)
+            RMSNorm(dim, normalize_dim = 1)
         )
 
     def forward(self, x):
         residual = x
 
         b, c, h, w = x.shape
 
@@ -203,15 +199,15 @@
 class Attention(nn.Module):
     def __init__(self, dim, heads = 4, dim_head = 32, scale = 8, dropout = 0.):
         super().__init__()
         self.scale = scale
         self.heads = heads
         hidden_dim = dim_head * heads
 
-        self.norm = LayerNorm(dim)
+        self.norm = RMSNorm(dim)
 
         self.attn_dropout = nn.Dropout(dropout)
         self.to_qkv = nn.Linear(dim, hidden_dim * 3, bias = False)
 
         self.q_scale = nn.Parameter(torch.ones(dim_head))
         self.k_scale = nn.Parameter(torch.ones(dim_head))
 
@@ -243,15 +239,15 @@
         self,
         dim,
         cond_dim,
         mult = 4,
         dropout = 0.
     ):
         super().__init__()
-        self.norm = LayerNorm(dim, scale = False)
+        self.norm = RMSNorm(dim, scale = False)
         dim_hidden = dim * mult
 
         self.to_scale_shift = nn.Sequential(
             nn.SiLU(),
             nn.Linear(cond_dim, dim_hidden * 2),
             Rearrange('b d -> b 1 d')
         )
@@ -355,18 +351,19 @@
         needs_patch = patch_size > 1
 
         if needs_patch:
             if not dual_patchnorm:
                 self.init_conv = nn.Conv2d(channels, init_dim, patch_size, stride = patch_size)
             else:
                 self.init_conv = nn.Sequential(
-                    Rearrange('b c (h p1) (w p2) -> b (c p1 p2) h w', p1 = patch_size, p2 = patch_size),
-                    LayerNorm(input_channels, normalize_dim = 1),
-                    nn.Conv2d(input_channels, init_dim, 1),
-                    LayerNorm(init_dim, normalize_dim = 1)
+                    Rearrange('b c (h p1) (w p2) -> b h w (c p1 p2)', p1 = patch_size, p2 = patch_size),
+                    nn.LayerNorm(input_channels),
+                    nn.Linear(input_channels, init_dim),
+                    nn.LayerNorm(init_dim),
+                    Rearrange('b h w c -> b c h w')
                 )
 
             self.unpatchify = nn.ConvTranspose2d(input_channels, channels, patch_size, stride = patch_size)
 
         # determine dimensions
 
         dims = [init_dim, *map(lambda m: dim * m, dim_mults)]
```

### Comparing `denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.6.4
+Version: 1.7.0
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.4/setup.py` & `denoising-diffusion-pytorch-1.7.0/setup.py`

 * *Files identical despite different names*

