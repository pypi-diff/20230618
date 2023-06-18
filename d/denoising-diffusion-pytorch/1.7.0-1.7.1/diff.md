# Comparing `tmp/denoising-diffusion-pytorch-1.7.0.tar.gz` & `tmp/denoising-diffusion-pytorch-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising-diffusion-pytorch-1.7.0.tar", last modified: Sun Jun 18 18:39:04 2023, max compression
+gzip compressed data, was "denoising-diffusion-pytorch-1.7.1.tar", last modified: Sun Jun 18 18:45:21 2023, max compression
```

## Comparing `denoising-diffusion-pytorch-1.7.0.tar` & `denoising-diffusion-pytorch-1.7.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:39:04.313675 denoising-diffusion-pytorch-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-18 18:39:04.313675 denoising-diffusion-pytorch-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:39:04.313675 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28415 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    36235 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    30279 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    36221 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21193 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:39:04.313675 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-18 18:39:04.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-18 18:39:04.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 18:39:04.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-18 18:39:04.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-18 18:39:04.000000 denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 18:39:04.313675 denoising-diffusion-pytorch-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-18 18:38:54.000000 denoising-diffusion-pytorch-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:45:21.591915 denoising-diffusion-pytorch-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-18 18:45:12.000000 denoising-diffusion-pytorch-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-18 18:45:21.591915 denoising-diffusion-pytorch-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-06-18 18:45:12.000000 denoising-diffusion-pytorch-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:45:21.591915 denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-18 18:45:12.000000 denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28424 2023-06-18 18:45:12.000000 denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-06-18 18:45:12.000000 denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36244 2023-06-18 18:45:12.000000 denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30288 2023-06-18 18:45:12.000000 denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-18 18:45:12.000000 denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36230 2023-06-18 18:45:12.000000 denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-18 18:45:12.000000 denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21193 2023-06-18 18:45:12.000000 denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-06-18 18:45:12.000000 denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-18 18:45:12.000000 denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-18 18:45:12.000000 denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:45:21.591915 denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-18 18:45:21.000000 denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-18 18:45:21.000000 denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 18:45:21.000000 denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-18 18:45:21.000000 denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-18 18:45:21.000000 denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 18:45:21.591915 denoising-diffusion-pytorch-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-18 18:45:12.000000 denoising-diffusion-pytorch-1.7.1/setup.py
```

### Comparing `denoising-diffusion-pytorch-1.7.0/LICENSE` & `denoising-diffusion-pytorch-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.0/PKG-INFO` & `denoising-diffusion-pytorch-1.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.7.0
+Version: 1.7.1
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.7.0/README.md` & `denoising-diffusion-pytorch-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/__init__.py` & `denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     """
     def forward(self, x):
         eps = 1e-5 if x.dtype == torch.float32 else 1e-3
 
         weight = self.weight
         mean = reduce(weight, 'o ... -> o 1 1 1', 'mean')
         var = reduce(weight, 'o ... -> o 1 1 1', partial(torch.var, unbiased = False))
-        normalized_weight = (weight - mean) * (var + eps).rsqrt()
+        normalized_weight = (weight - mean) * var.clamp(min = eps).rsqrt()
 
         return F.conv2d(x, normalized_weight, self.bias, self.stride, self.padding, self.dilation, self.groups)
 
 class RMSNorm(nn.Module):
     def __init__(self, dim):
         super().__init__()
         self.g = nn.Parameter(torch.ones(1, dim, 1, 1))
```

### Comparing `denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     """
     def forward(self, x):
         eps = 1e-5 if x.dtype == torch.float32 else 1e-3
 
         weight = self.weight
         mean = reduce(weight, 'o ... -> o 1 1 1', 'mean')
         var = reduce(weight, 'o ... -> o 1 1 1', partial(torch.var, unbiased = False))
-        normalized_weight = (weight - mean) * (var + eps).rsqrt()
+        normalized_weight = (weight - mean) * var.clamp(min = eps).rsqrt()
 
         return F.conv2d(x, normalized_weight, self.bias, self.stride, self.padding, self.dilation, self.groups)
 
 class RMSNorm(nn.Module):
     def __init__(self, dim):
         super().__init__()
         self.g = nn.Parameter(torch.ones(1, dim, 1, 1))
```

### Comparing `denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     """
     def forward(self, x):
         eps = 1e-5 if x.dtype == torch.float32 else 1e-3
 
         weight = self.weight
         mean = reduce(weight, 'o ... -> o 1 1', 'mean')
         var = reduce(weight, 'o ... -> o 1 1', partial(torch.var, unbiased = False))
-        normalized_weight = (weight - mean) * (var + eps).rsqrt()
+        normalized_weight = (weight - mean) * var.clamp(min = eps).rsqrt()
 
         return F.conv1d(x, normalized_weight, self.bias, self.stride, self.padding, self.dilation, self.groups)
 
 class RMSNorm(nn.Module):
     def __init__(self, dim):
         super().__init__()
         self.g = nn.Parameter(torch.ones(1, dim, 1))
```

### Comparing `denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     """
     def forward(self, x):
         eps = 1e-5 if x.dtype == torch.float32 else 1e-3
 
         weight = self.weight
         mean = reduce(weight, 'o ... -> o 1 1 1', 'mean')
         var = reduce(weight, 'o ... -> o 1 1 1', partial(torch.var, unbiased = False))
-        normalized_weight = (weight - mean) * (var + eps).rsqrt()
+        normalized_weight = (weight - mean) * var.clamp(min = eps).rsqrt()
 
         return F.conv2d(x, normalized_weight, self.bias, self.stride, self.padding, self.dilation, self.groups)
 
 class RMSNorm(nn.Module):
     def __init__(self, dim):
         super().__init__()
         self.g = nn.Parameter(torch.ones(1, dim, 1, 1))
```

### Comparing `denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.7.0
+Version: 1.7.1
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.7.0/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising-diffusion-pytorch-1.7.1/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.7.0/setup.py` & `denoising-diffusion-pytorch-1.7.1/setup.py`

 * *Files identical despite different names*

