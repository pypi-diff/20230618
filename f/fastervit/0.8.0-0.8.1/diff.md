# Comparing `tmp/fastervit-0.8.0.tar.gz` & `tmp/fastervit-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ali/Desktop/Gitlab_repos/FasterViT_pip_test/dist/.tmp-ipahv624/fastervit-0.8.0.tar", last modified: Sun Jun 18 17:33:37 2023, max compression
+gzip compressed data, was "/home/ali/Desktop/Gitlab_repos/FasterViT_pip_test/dist/.tmp-5w8l1052/fastervit-0.8.1.tar", last modified: Sun Jun 18 18:55:22 2023, max compression
```

## Comparing `fastervit-0.8.0.tar` & `fastervit-0.8.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-18 17:33:37.000000 fastervit-0.8.0/
--rw-rw-r--   0 ali       (1000) ali       (1000)     4146 2023-06-17 23:20:57.000000 fastervit-0.8.0/LICENSE
--rw-rw-r--   0 ali       (1000) ali       (1000)       20 2023-06-18 16:31:37.000000 fastervit-0.8.0/MANIFEST.in
--rw-rw-r--   0 ali       (1000) ali       (1000)     8182 2023-06-18 17:33:37.000000 fastervit-0.8.0/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)     7232 2023-06-17 23:28:51.000000 fastervit-0.8.0/README.md
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-18 17:33:37.000000 fastervit-0.8.0/fastervit/
--rw-rw-r--   0 ali       (1000) ali       (1000)        0 2023-06-18 16:26:32.000000 fastervit-0.8.0/fastervit/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1878 2023-06-17 23:20:57.000000 fastervit-0.8.0/fastervit/onnx_convert.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      331 2023-06-17 23:20:57.000000 fastervit-0.8.0/fastervit/onnx_test.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-18 17:33:37.000000 fastervit-0.8.0/fastervit/scheduler/
--rw-rw-r--   0 ali       (1000) ali       (1000)      291 2023-06-17 23:20:57.000000 fastervit-0.8.0/fastervit/scheduler/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     4161 2023-06-17 23:20:57.000000 fastervit-0.8.0/fastervit/scheduler/cosine_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     2098 2023-06-17 23:20:57.000000 fastervit-0.8.0/fastervit/scheduler/multistep_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3457 2023-06-17 23:20:57.000000 fastervit-0.8.0/fastervit/scheduler/plateau_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     4003 2023-06-17 23:20:57.000000 fastervit-0.8.0/fastervit/scheduler/poly_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     5095 2023-06-17 23:20:57.000000 fastervit-0.8.0/fastervit/scheduler/scheduler.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3907 2023-06-17 23:20:57.000000 fastervit-0.8.0/fastervit/scheduler/scheduler_factory.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1902 2023-06-17 23:20:57.000000 fastervit-0.8.0/fastervit/scheduler/step_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3936 2023-06-17 23:20:57.000000 fastervit-0.8.0/fastervit/scheduler/tanh_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      734 2023-06-17 23:20:57.000000 fastervit-0.8.0/fastervit/tensorboard.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    49797 2023-06-17 23:23:20.000000 fastervit-0.8.0/fastervit/train.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    16145 2023-06-17 23:20:57.000000 fastervit-0.8.0/fastervit/validate.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-18 17:33:37.000000 fastervit-0.8.0/fastervit.egg-info/
--rw-rw-r--   0 ali       (1000) ali       (1000)     8182 2023-06-18 17:33:37.000000 fastervit-0.8.0/fastervit.egg-info/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)      651 2023-06-18 17:33:37.000000 fastervit-0.8.0/fastervit.egg-info/SOURCES.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)        1 2023-06-18 17:33:37.000000 fastervit-0.8.0/fastervit.egg-info/dependency_links.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       32 2023-06-18 17:33:37.000000 fastervit-0.8.0/fastervit.egg-info/requires.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       10 2023-06-18 17:33:37.000000 fastervit-0.8.0/fastervit.egg-info/top_level.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)      126 2023-06-18 17:33:37.000000 fastervit-0.8.0/setup.cfg
--rw-rw-r--   0 ali       (1000) ali       (1000)     1549 2023-06-18 17:31:30.000000 fastervit-0.8.0/setup.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-18 18:55:22.000000 fastervit-0.8.1/
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4146 2023-06-17 23:20:57.000000 fastervit-0.8.1/LICENSE
+-rw-rw-r--   0 ali       (1000) ali       (1000)       30 2023-06-18 18:51:30.000000 fastervit-0.8.1/MANIFEST.in
+-rw-rw-r--   0 ali       (1000) ali       (1000)     8192 2023-06-18 18:55:22.000000 fastervit-0.8.1/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)     7242 2023-06-18 18:51:46.000000 fastervit-0.8.1/README.md
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-18 18:55:22.000000 fastervit-0.8.1/fastervit/
+-rw-rw-r--   0 ali       (1000) ali       (1000)        0 2023-06-18 16:26:32.000000 fastervit-0.8.1/fastervit/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1878 2023-06-17 23:20:57.000000 fastervit-0.8.1/fastervit/onnx_convert.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      331 2023-06-17 23:20:57.000000 fastervit-0.8.1/fastervit/onnx_test.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-18 18:55:22.000000 fastervit-0.8.1/fastervit/scheduler/
+-rw-rw-r--   0 ali       (1000) ali       (1000)      291 2023-06-17 23:20:57.000000 fastervit-0.8.1/fastervit/scheduler/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4161 2023-06-17 23:20:57.000000 fastervit-0.8.1/fastervit/scheduler/cosine_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     2098 2023-06-17 23:20:57.000000 fastervit-0.8.1/fastervit/scheduler/multistep_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3457 2023-06-17 23:20:57.000000 fastervit-0.8.1/fastervit/scheduler/plateau_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4003 2023-06-17 23:20:57.000000 fastervit-0.8.1/fastervit/scheduler/poly_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     5095 2023-06-17 23:20:57.000000 fastervit-0.8.1/fastervit/scheduler/scheduler.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3907 2023-06-17 23:20:57.000000 fastervit-0.8.1/fastervit/scheduler/scheduler_factory.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1902 2023-06-17 23:20:57.000000 fastervit-0.8.1/fastervit/scheduler/step_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3936 2023-06-17 23:20:57.000000 fastervit-0.8.1/fastervit/scheduler/tanh_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      734 2023-06-17 23:20:57.000000 fastervit-0.8.1/fastervit/tensorboard.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    49797 2023-06-17 23:23:20.000000 fastervit-0.8.1/fastervit/train.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    16145 2023-06-17 23:20:57.000000 fastervit-0.8.1/fastervit/validate.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-18 18:55:22.000000 fastervit-0.8.1/fastervit.egg-info/
+-rw-rw-r--   0 ali       (1000) ali       (1000)     8192 2023-06-18 18:55:22.000000 fastervit-0.8.1/fastervit.egg-info/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)      651 2023-06-18 18:55:22.000000 fastervit-0.8.1/fastervit.egg-info/SOURCES.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)        1 2023-06-18 18:55:22.000000 fastervit-0.8.1/fastervit.egg-info/dependency_links.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       32 2023-06-18 18:55:22.000000 fastervit-0.8.1/fastervit.egg-info/requires.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       10 2023-06-18 18:55:22.000000 fastervit-0.8.1/fastervit.egg-info/top_level.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)      126 2023-06-18 18:55:22.000000 fastervit-0.8.1/setup.cfg
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1549 2023-06-18 18:55:04.000000 fastervit-0.8.1/setup.py
```

### Comparing `fastervit-0.8.0/LICENSE` & `fastervit-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.0/PKG-INFO` & `fastervit-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastervit
-Version: 0.8.0
+Version: 0.8.1
 Summary: FasterViT: Fast Vision Transformers with Hierarchical Attention
 Home-page: https://github.com/NVlabs/FasterViT
 Author: Ali Hatamizadeh
 Author-email: ahatamiz123@gmail.com
 License: NVIDIA Source Code License-NC
 Keywords: pytorch pretrained models efficientnet mobilenetv3 mnasnet resnet vision transformer vit
 Classifier: Programming Language :: Python :: 3.7
@@ -46,15 +46,15 @@
 </p>
 
 
 We introduce a new self-attention mechanism, denoted as Hierarchical
 Attention (HAT), that captures both short and long-range information by learning
 cross-window carrier tokens.
 
-![teaser](./assets/hierarchial_attn.png)
+![teaser](./fastervit/assets/hierarchial_attn.png)
 
 ## 💥 News 💥
 
 - **[06.17.2023]** 🔥 Any-resolution FasterViT model is now available ! the model can be used for variety of applications such as detection and segmentation or high-resolution fine-tuning with arbitrary input image resolutions. 
 - **[06.09.2023]** 🔥🔥 We have released source code and ImageNet-1K FasterViT-models !
 
 ## Catalog
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastervit Version: 0.8.0 Summary: FasterViT: Fast
+Metadata-Version: 2.1 Name: fastervit Version: 0.8.1 Summary: FasterViT: Fast
 Vision Transformers with Hierarchical Attention Home-page: https://github.com/
 NVlabs/FasterViT Author: Ali Hatamizadeh Author-email: ahatamiz123@gmail.com
 License: NVIDIA Source Code License-NC Keywords: pytorch pretrained models
 efficientnet mobilenetv3 mnasnet resnet vision transformer vit Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -23,18 +23,18 @@
 www.nvidia.com/en-us/research/inquiries/) --- FasterViT achieves a new SOTA
 Pareto-front in terms of accuracy vs. image throughput (no extra training data
 !)
  [https://github.com/NVlabs/FasterViT/assets/26806394/253d1a2e-b5f5-4a9b-a362-
                                  6cdd16bfccc1]
 We introduce a new self-attention mechanism, denoted as Hierarchical Attention
 (HAT), that captures both short and long-range information by learning cross-
-window carrier tokens. ![teaser](./assets/hierarchial_attn.png) ## ð¥ News
-ð¥ - **[06.17.2023]** ð¥ Any-resolution FasterViT model is now available !
-the model can be used for variety of applications such as detection and
-segmentation or high-resolution fine-tuning with arbitrary input image
+window carrier tokens. ![teaser](./fastervit/assets/hierarchial_attn.png) ##
+ð¥ News ð¥ - **[06.17.2023]** ð¥ Any-resolution FasterViT model is now
+available ! the model can be used for variety of applications such as detection
+and segmentation or high-resolution fine-tuning with arbitrary input image
 resolutions. - **[06.09.2023]** ð¥ð¥ We have released source code and
 ImageNet-1K FasterViT-models ! ## Catalog - [x] ImageNet-1K training code - [x]
 ImageNet-1K pre-trained models - [x] Any-resolution FasterViT - [ ] ImageNet-
 21K pre-trained models - [ ] ImageNet-21K fine-tune scripts - [ ] Detection
 code (DINO) + models - [ ] Segmentation code + models ## Results + Pretrained
 Models ### ImageNet-1K **FasterViT ImageNet-1K Pretrained Models**
 Name       Acc@1(%) Acc@5(%) Throughput Resolution #Params(M) FLOPs(G) Download
```

### Comparing `fastervit-0.8.0/README.md` & `fastervit-0.8.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 </p>
 
 
 We introduce a new self-attention mechanism, denoted as Hierarchical
 Attention (HAT), that captures both short and long-range information by learning
 cross-window carrier tokens.
 
-![teaser](./assets/hierarchial_attn.png)
+![teaser](./fastervit/assets/hierarchial_attn.png)
 
 ## 💥 News 💥
 
 - **[06.17.2023]** 🔥 Any-resolution FasterViT model is now available ! the model can be used for variety of applications such as detection and segmentation or high-resolution fine-tuning with arbitrary input image resolutions. 
 - **[06.09.2023]** 🔥🔥 We have released source code and ImageNet-1K FasterViT-models !
 
 ## Catalog
```

#### html2text {}

```diff
@@ -10,18 +10,18 @@
 Research Licensing](https://www.nvidia.com/en-us/research/inquiries/) --
 - FasterViT achieves a new SOTA Pareto-front in terms of accuracy vs. image
 throughput (no extra training data !)
  [https://github.com/NVlabs/FasterViT/assets/26806394/253d1a2e-b5f5-4a9b-a362-
                                  6cdd16bfccc1]
 We introduce a new self-attention mechanism, denoted as Hierarchical Attention
 (HAT), that captures both short and long-range information by learning cross-
-window carrier tokens. ![teaser](./assets/hierarchial_attn.png) ## ð¥ News
-ð¥ - **[06.17.2023]** ð¥ Any-resolution FasterViT model is now available !
-the model can be used for variety of applications such as detection and
-segmentation or high-resolution fine-tuning with arbitrary input image
+window carrier tokens. ![teaser](./fastervit/assets/hierarchial_attn.png) ##
+ð¥ News ð¥ - **[06.17.2023]** ð¥ Any-resolution FasterViT model is now
+available ! the model can be used for variety of applications such as detection
+and segmentation or high-resolution fine-tuning with arbitrary input image
 resolutions. - **[06.09.2023]** ð¥ð¥ We have released source code and
 ImageNet-1K FasterViT-models ! ## Catalog - [x] ImageNet-1K training code - [x]
 ImageNet-1K pre-trained models - [x] Any-resolution FasterViT - [ ] ImageNet-
 21K pre-trained models - [ ] ImageNet-21K fine-tune scripts - [ ] Detection
 code (DINO) + models - [ ] Segmentation code + models ## Results + Pretrained
 Models ### ImageNet-1K **FasterViT ImageNet-1K Pretrained Models**
 Name       Acc@1(%) Acc@5(%) Throughput Resolution #Params(M) FLOPs(G) Download
```

### Comparing `fastervit-0.8.0/fastervit/onnx_convert.py` & `fastervit-0.8.1/fastervit/onnx_convert.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.0/fastervit/scheduler/cosine_lr.py` & `fastervit-0.8.1/fastervit/scheduler/cosine_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.0/fastervit/scheduler/multistep_lr.py` & `fastervit-0.8.1/fastervit/scheduler/multistep_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.0/fastervit/scheduler/plateau_lr.py` & `fastervit-0.8.1/fastervit/scheduler/plateau_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.0/fastervit/scheduler/poly_lr.py` & `fastervit-0.8.1/fastervit/scheduler/poly_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.0/fastervit/scheduler/scheduler.py` & `fastervit-0.8.1/fastervit/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.0/fastervit/scheduler/scheduler_factory.py` & `fastervit-0.8.1/fastervit/scheduler/scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.0/fastervit/scheduler/step_lr.py` & `fastervit-0.8.1/fastervit/scheduler/step_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.0/fastervit/scheduler/tanh_lr.py` & `fastervit-0.8.1/fastervit/scheduler/tanh_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.0/fastervit/tensorboard.py` & `fastervit-0.8.1/fastervit/tensorboard.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.0/fastervit/train.py` & `fastervit-0.8.1/fastervit/train.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.0/fastervit/validate.py` & `fastervit-0.8.1/fastervit/validate.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.0/fastervit.egg-info/PKG-INFO` & `fastervit-0.8.1/fastervit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastervit
-Version: 0.8.0
+Version: 0.8.1
 Summary: FasterViT: Fast Vision Transformers with Hierarchical Attention
 Home-page: https://github.com/NVlabs/FasterViT
 Author: Ali Hatamizadeh
 Author-email: ahatamiz123@gmail.com
 License: NVIDIA Source Code License-NC
 Keywords: pytorch pretrained models efficientnet mobilenetv3 mnasnet resnet vision transformer vit
 Classifier: Programming Language :: Python :: 3.7
@@ -46,15 +46,15 @@
 </p>
 
 
 We introduce a new self-attention mechanism, denoted as Hierarchical
 Attention (HAT), that captures both short and long-range information by learning
 cross-window carrier tokens.
 
-![teaser](./assets/hierarchial_attn.png)
+![teaser](./fastervit/assets/hierarchial_attn.png)
 
 ## 💥 News 💥
 
 - **[06.17.2023]** 🔥 Any-resolution FasterViT model is now available ! the model can be used for variety of applications such as detection and segmentation or high-resolution fine-tuning with arbitrary input image resolutions. 
 - **[06.09.2023]** 🔥🔥 We have released source code and ImageNet-1K FasterViT-models !
 
 ## Catalog
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastervit Version: 0.8.0 Summary: FasterViT: Fast
+Metadata-Version: 2.1 Name: fastervit Version: 0.8.1 Summary: FasterViT: Fast
 Vision Transformers with Hierarchical Attention Home-page: https://github.com/
 NVlabs/FasterViT Author: Ali Hatamizadeh Author-email: ahatamiz123@gmail.com
 License: NVIDIA Source Code License-NC Keywords: pytorch pretrained models
 efficientnet mobilenetv3 mnasnet resnet vision transformer vit Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -23,18 +23,18 @@
 www.nvidia.com/en-us/research/inquiries/) --- FasterViT achieves a new SOTA
 Pareto-front in terms of accuracy vs. image throughput (no extra training data
 !)
  [https://github.com/NVlabs/FasterViT/assets/26806394/253d1a2e-b5f5-4a9b-a362-
                                  6cdd16bfccc1]
 We introduce a new self-attention mechanism, denoted as Hierarchical Attention
 (HAT), that captures both short and long-range information by learning cross-
-window carrier tokens. ![teaser](./assets/hierarchial_attn.png) ## ð¥ News
-ð¥ - **[06.17.2023]** ð¥ Any-resolution FasterViT model is now available !
-the model can be used for variety of applications such as detection and
-segmentation or high-resolution fine-tuning with arbitrary input image
+window carrier tokens. ![teaser](./fastervit/assets/hierarchial_attn.png) ##
+ð¥ News ð¥ - **[06.17.2023]** ð¥ Any-resolution FasterViT model is now
+available ! the model can be used for variety of applications such as detection
+and segmentation or high-resolution fine-tuning with arbitrary input image
 resolutions. - **[06.09.2023]** ð¥ð¥ We have released source code and
 ImageNet-1K FasterViT-models ! ## Catalog - [x] ImageNet-1K training code - [x]
 ImageNet-1K pre-trained models - [x] Any-resolution FasterViT - [ ] ImageNet-
 21K pre-trained models - [ ] ImageNet-21K fine-tune scripts - [ ] Detection
 code (DINO) + models - [ ] Segmentation code + models ## Results + Pretrained
 Models ### ImageNet-1K **FasterViT ImageNet-1K Pretrained Models**
 Name       Acc@1(%) Acc@5(%) Throughput Resolution #Params(M) FLOPs(G) Download
```

### Comparing `fastervit-0.8.0/fastervit.egg-info/SOURCES.txt` & `fastervit-0.8.1/fastervit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.0/setup.py` & `fastervit-0.8.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='fastervit',
-    version='0.8.0',
+    version='0.8.1',
     description='FasterViT: Fast Vision Transformers with Hierarchical Attention',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/NVlabs/FasterViT',
     author='Ali Hatamizadeh',
     author_email='ahatamiz123@gmail.com',
     classifiers=[
```

