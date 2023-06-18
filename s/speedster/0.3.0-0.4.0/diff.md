# Comparing `tmp/speedster-0.3.0.tar.gz` & `tmp/speedster-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedster-0.3.0.tar", last modified: Tue Mar 21 12:56:33 2023, max compression
+gzip compressed data, was "speedster-0.4.0.tar", last modified: Sun Jun 18 11:01:52 2023, max compression
```

## Comparing `speedster-0.3.0.tar` & `speedster-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:56:33.454771 speedster-0.3.0/
--rw-r--r--   0 diegofiori   (501) staff       (20)    17422 2023-03-21 12:56:33.454604 speedster-0.3.0/PKG-INFO
--rw-r--r--   0 diegofiori   (501) staff       (20)    17328 2023-03-21 12:50:34.000000 speedster-0.3.0/README.md
--rw-r--r--   0 diegofiori   (501) staff       (20)       38 2023-03-21 12:56:33.454811 speedster-0.3.0/setup.cfg
--rw-r--r--   0 diegofiori   (501) staff       (20)      492 2023-03-21 12:53:24.000000 speedster-0.3.0/setup.py
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:56:33.452165 speedster-0.3.0/speedster/
--rw-r--r--   0 diegofiori   (501) staff       (20)      172 2023-01-23 23:00:29.000000 speedster-0.3.0/speedster/__init__.py
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:56:33.453089 speedster-0.3.0/speedster/api/
--rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-12-16 18:45:48.000000 speedster-0.3.0/speedster/api/__init__.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     7448 2023-01-22 15:05:27.000000 speedster-0.3.0/speedster/api/functions.py
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:56:33.454343 speedster-0.3.0/speedster/api/tests/
--rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-12-16 18:45:48.000000 speedster-0.3.0/speedster/api/tests/__init__.py
--rw-r--r--   0 diegofiori   (501) staff       (20)    13231 2023-02-15 12:55:17.000000 speedster-0.3.0/speedster/api/tests/test_huggingface.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     8073 2023-03-21 12:50:34.000000 speedster-0.3.0/speedster/api/tests/test_onnx.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     7717 2023-02-15 12:55:17.000000 speedster-0.3.0/speedster/api/tests/test_pytorch.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     6950 2023-01-23 23:00:29.000000 speedster-0.3.0/speedster/api/tests/test_tensorflow.py
--rw-r--r--   0 diegofiori   (501) staff       (20)      640 2023-03-21 12:50:34.000000 speedster-0.3.0/speedster/api/tests/utils.py
--rw-r--r--   0 diegofiori   (501) staff       (20)    22525 2023-03-21 12:53:24.000000 speedster-0.3.0/speedster/root_op.py
--rw-r--r--   0 diegofiori   (501) staff       (20)      295 2023-01-05 10:07:54.000000 speedster-0.3.0/speedster/speedster.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     1703 2023-02-15 12:55:17.000000 speedster-0.3.0/speedster/utils.py
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:56:33.452885 speedster-0.3.0/speedster.egg-info/
--rw-r--r--   0 diegofiori   (501) staff       (20)    17422 2023-03-21 12:56:33.000000 speedster-0.3.0/speedster.egg-info/PKG-INFO
--rw-r--r--   0 diegofiori   (501) staff       (20)      529 2023-03-21 12:56:33.000000 speedster-0.3.0/speedster.egg-info/SOURCES.txt
--rw-r--r--   0 diegofiori   (501) staff       (20)        1 2023-03-21 12:56:33.000000 speedster-0.3.0/speedster.egg-info/dependency_links.txt
--rw-r--r--   0 diegofiori   (501) staff       (20)       32 2023-03-21 12:56:33.000000 speedster-0.3.0/speedster.egg-info/requires.txt
--rw-r--r--   0 diegofiori   (501) staff       (20)       10 2023-03-21 12:56:33.000000 speedster-0.3.0/speedster.egg-info/top_level.txt
+drwxr-xr-x   0 valeriosofi   (501) staff       (20)        0 2023-06-18 11:01:52.658854 speedster-0.4.0/
+-rw-r--r--   0 valeriosofi   (501) staff       (20)    17370 2023-06-18 11:01:52.658661 speedster-0.4.0/PKG-INFO
+-rw-r--r--   0 valeriosofi   (501) staff       (20)    17276 2023-06-18 10:44:23.000000 speedster-0.4.0/README.md
+-rw-r--r--   0 valeriosofi   (501) staff       (20)       38 2023-06-18 11:01:52.658892 speedster-0.4.0/setup.cfg
+-rw-r--r--   0 valeriosofi   (501) staff       (20)      492 2023-06-18 10:44:23.000000 speedster-0.4.0/setup.py
+drwxr-xr-x   0 valeriosofi   (501) staff       (20)        0 2023-06-18 11:01:52.656279 speedster-0.4.0/speedster/
+-rw-r--r--   0 valeriosofi   (501) staff       (20)      172 2023-06-18 10:44:23.000000 speedster-0.4.0/speedster/__init__.py
+drwxr-xr-x   0 valeriosofi   (501) staff       (20)        0 2023-06-18 11:01:52.657020 speedster-0.4.0/speedster/api/
+-rw-r--r--   0 valeriosofi   (501) staff       (20)        0 2023-06-18 10:44:23.000000 speedster-0.4.0/speedster/api/__init__.py
+-rw-r--r--   0 valeriosofi   (501) staff       (20)     7422 2023-06-18 10:44:23.000000 speedster-0.4.0/speedster/api/functions.py
+drwxr-xr-x   0 valeriosofi   (501) staff       (20)        0 2023-06-18 11:01:52.658011 speedster-0.4.0/speedster/api/tests/
+-rw-r--r--   0 valeriosofi   (501) staff       (20)        0 2023-06-18 10:44:23.000000 speedster-0.4.0/speedster/api/tests/__init__.py
+-rw-r--r--   0 valeriosofi   (501) staff       (20)    13237 2023-06-18 10:44:23.000000 speedster-0.4.0/speedster/api/tests/test_huggingface.py
+-rw-r--r--   0 valeriosofi   (501) staff       (20)     8095 2023-06-18 10:44:23.000000 speedster-0.4.0/speedster/api/tests/test_onnx.py
+-rw-r--r--   0 valeriosofi   (501) staff       (20)     9067 2023-06-18 10:44:23.000000 speedster-0.4.0/speedster/api/tests/test_pytorch.py
+-rw-r--r--   0 valeriosofi   (501) staff       (20)     6950 2023-06-18 10:44:23.000000 speedster-0.4.0/speedster/api/tests/test_tensorflow.py
+-rw-r--r--   0 valeriosofi   (501) staff       (20)      641 2023-06-18 10:44:23.000000 speedster-0.4.0/speedster/api/tests/utils.py
+-rw-r--r--   0 valeriosofi   (501) staff       (20)     8039 2023-06-18 10:44:23.000000 speedster-0.4.0/speedster/root_op.py
+-rw-r--r--   0 valeriosofi   (501) staff       (20)      295 2023-06-18 10:44:23.000000 speedster-0.4.0/speedster/speedster.py
+drwxr-xr-x   0 valeriosofi   (501) staff       (20)        0 2023-06-18 11:01:52.658460 speedster-0.4.0/speedster/tests/
+-rw-r--r--   0 valeriosofi   (501) staff       (20)        0 2023-06-18 10:44:23.000000 speedster-0.4.0/speedster/tests/__init__.py
+-rw-r--r--   0 valeriosofi   (501) staff       (20)     1766 2023-06-18 10:44:23.000000 speedster-0.4.0/speedster/tests/test_root_op.py
+-rw-r--r--   0 valeriosofi   (501) staff       (20)        0 2023-06-18 10:44:23.000000 speedster-0.4.0/speedster/utils.py
+drwxr-xr-x   0 valeriosofi   (501) staff       (20)        0 2023-06-18 11:01:52.656829 speedster-0.4.0/speedster.egg-info/
+-rw-r--r--   0 valeriosofi   (501) staff       (20)    17370 2023-06-18 11:01:52.000000 speedster-0.4.0/speedster.egg-info/PKG-INFO
+-rw-r--r--   0 valeriosofi   (501) staff       (20)      589 2023-06-18 11:01:52.000000 speedster-0.4.0/speedster.egg-info/SOURCES.txt
+-rw-r--r--   0 valeriosofi   (501) staff       (20)        1 2023-06-18 11:01:52.000000 speedster-0.4.0/speedster.egg-info/dependency_links.txt
+-rw-r--r--   0 valeriosofi   (501) staff       (20)       32 2023-06-18 11:01:52.000000 speedster-0.4.0/speedster.egg-info/requires.txt
+-rw-r--r--   0 valeriosofi   (501) staff       (20)       10 2023-06-18 11:01:52.000000 speedster-0.4.0/speedster.egg-info/top_level.txt
```

### Comparing `speedster-0.3.0/PKG-INFO` & `speedster-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: speedster
-Version: 0.3.0
+Version: 0.4.0
 Description-Content-Type: text/markdown
 
 # 💥 Speedster
 
-`Speedster` is an open-source module designed to speed up AI inference in just a few lines of code. The library automatically applies the best set of SOTA optimization techniques to achieve the maximum inference speed-up (latency, throughput, model size) physically possible on your hardware (single machine).
+`Speedster` reduces inference costs by leveraging SOTA optimization techniques that best couple your AI models with the underlying hardware (GPUs and CPUs). The idea is to make AI inference way cheaper in just a few lines of code.
 
-`Speedster` makes it easy to combine optimization techniques across the whole software-to-hardware stack, delivering best-in-class speed-ups. If you like the idea, give us a star to support the project ⭐
+`Speedster` makes it easy to combine optimization techniques across the whole software-to-hardware stack, delivering best-in-class cost savings. If you like the idea, give us a star to support the project ⭐
 
 ![speedster](https://user-images.githubusercontent.com/53374883/225599469-f1a626f0-c001-42bd-bc8b-ec0e966ddad6.png)
 
 The core `Speedster` workflow consists of 3 steps:
 
-
 - [x]  **Select**: input your model in your preferred DL framework and express your preferences regarding:
-    - Accuracy loss: do you want to trade off a little accuracy for much higher performance?
-    - Optimization time: stellar accelerations can be time-consuming. Can you wait, or do you need an instant answer?
+    - Accuracy loss: do you want to trade off a little accuracy for significant cost savings?
+    - Optimization time: achieving great savings can be time-consuming. Can you wait, or do you need an instant answer?
 - [x]  **Search**: the library automatically tests every combination of optimization techniques across the software-to-hardware stack (sparsity, quantization, compilers, etc.) that is compatible with your needs and local hardware.
-- [x]  **Serve**: finally, `Speedster` chooses the best configuration of optimization techniques and returns an accelerated version of your model in the DL framework of your choice (just on steroids 🚀).
-
+- [x]  **Serve**: finally, `Speedster` chooses the best configuration of optimization techniques and returns an accelerated version of your model in the DL framework of your choice (just cheaper 🚀).
 
 # Installation
 
 Install `Speedster` and its base requirements:
 ```
 pip install speedster
 ```
@@ -185,15 +183,15 @@
     </details>
     
 </details>
 
 <details>
 <summary>🧨 Hugging Face Diffusers </summary>
 
-> :warning: In order to work properly, the diffusers optimization requires `CUDA>=12.0` and `tensorrt>=8.6.0`. For additional details, please look the docs [here](https://docs.nebuly.com/Speedster/getting_started/diffusers_getting_started/).
+> :warning: In order to work properly, the diffusers optimization requires `CUDA>=12.0`, `tensorrt>=8.6.0` and `torch<=1.13.1`. For additional details, please look the docs [here](https://docs.nebuly.com/Speedster/getting_started/diffusers_getting_started/).
 
 In this section, we will learn about the 4 main steps needed to optimize Stable Diffusion models from the Diffusers library:
 
 1) Input your model and data
 2) Run the optimization
 3) Save your optimized model 
 4) Load and run your optimized model in production
@@ -353,15 +351,15 @@
 - [Notebooks](https://github.com/nebuly-ai/nebullvm/tree/main/notebooks/speedster)
 - [Advanced options](https://docs.nebuly.com/Speedster/advanced_options/)
 - [Benchmarks](https://docs.nebuly.com/Speedster/benchmarks/)
 
 
 # **Key concepts**
 
-`Speedster`'s design reflects our mission to automatically master each and every existing AI acceleration technique to deliver the **fastest AI ever**. As a result, `Speedster` leverages available enterprise-grade open-source optimization tools. If these tools and  communities already exist, and are distributed under a permissive license (Apache, MIT, etc), we integrate them and happily contribute to their communities. However, many tools do not exist yet, in which case we implement them and open-source the code so that our community can benefit from it.
+Speedster's design reflects our mission to automatically master each and every existing AI acceleration technique to deliver the most cost-efficient AI ever. As a result, `Speedster` leverages available enterprise-grade open-source optimization tools. If these tools and  communities already exist, and are distributed under a permissive license (Apache, MIT, etc), we integrate them and happily contribute to their communities. However, many tools do not exist yet, in which case we implement them and open-source the code so that our community can benefit from it.
 
 `Speedster` is shaped around **4 building blocks** and leverages a modular design to foster scalability and integration of new acceleration components across the software to hardware stack.
 
 - [x]  **Converter:** converts the input model from its original framework to the framework backends supported by `Speedster`, namely PyTorch, ONNX and TensorFlow. This allows the Compressor and Compiler modules to apply any optimization technique to the model.
 - [x]  **Compressor:** applies various compression techniques to the model, such as pruning, knowledge distillation, or quantization-aware training.
 - [x]  **Compiler:** converts the compressed models to the intermediate representation (IR) of the supported deep learning compilers. The compilers apply both post-training quantization techniques and graph optimizations, to produce compiled binary files.
 - [x]  **Inference Learner:** takes the best performing compiled model and converts it back into the same interface as the original input model.
```

### Comparing `speedster-0.3.0/README.md` & `speedster-0.4.0/speedster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,27 @@
+Metadata-Version: 2.1
+Name: speedster
+Version: 0.4.0
+Description-Content-Type: text/markdown
+
 # 💥 Speedster
 
-`Speedster` is an open-source module designed to speed up AI inference in just a few lines of code. The library automatically applies the best set of SOTA optimization techniques to achieve the maximum inference speed-up (latency, throughput, model size) physically possible on your hardware (single machine).
+`Speedster` reduces inference costs by leveraging SOTA optimization techniques that best couple your AI models with the underlying hardware (GPUs and CPUs). The idea is to make AI inference way cheaper in just a few lines of code.
 
-`Speedster` makes it easy to combine optimization techniques across the whole software-to-hardware stack, delivering best-in-class speed-ups. If you like the idea, give us a star to support the project ⭐
+`Speedster` makes it easy to combine optimization techniques across the whole software-to-hardware stack, delivering best-in-class cost savings. If you like the idea, give us a star to support the project ⭐
 
 ![speedster](https://user-images.githubusercontent.com/53374883/225599469-f1a626f0-c001-42bd-bc8b-ec0e966ddad6.png)
 
 The core `Speedster` workflow consists of 3 steps:
 
-
 - [x]  **Select**: input your model in your preferred DL framework and express your preferences regarding:
-    - Accuracy loss: do you want to trade off a little accuracy for much higher performance?
-    - Optimization time: stellar accelerations can be time-consuming. Can you wait, or do you need an instant answer?
+    - Accuracy loss: do you want to trade off a little accuracy for significant cost savings?
+    - Optimization time: achieving great savings can be time-consuming. Can you wait, or do you need an instant answer?
 - [x]  **Search**: the library automatically tests every combination of optimization techniques across the software-to-hardware stack (sparsity, quantization, compilers, etc.) that is compatible with your needs and local hardware.
-- [x]  **Serve**: finally, `Speedster` chooses the best configuration of optimization techniques and returns an accelerated version of your model in the DL framework of your choice (just on steroids 🚀).
-
+- [x]  **Serve**: finally, `Speedster` chooses the best configuration of optimization techniques and returns an accelerated version of your model in the DL framework of your choice (just cheaper 🚀).
 
 # Installation
 
 Install `Speedster` and its base requirements:
 ```
 pip install speedster
 ```
@@ -180,15 +183,15 @@
     </details>
     
 </details>
 
 <details>
 <summary>🧨 Hugging Face Diffusers </summary>
 
-> :warning: In order to work properly, the diffusers optimization requires `CUDA>=12.0` and `tensorrt>=8.6.0`. For additional details, please look the docs [here](https://docs.nebuly.com/Speedster/getting_started/diffusers_getting_started/).
+> :warning: In order to work properly, the diffusers optimization requires `CUDA>=12.0`, `tensorrt>=8.6.0` and `torch<=1.13.1`. For additional details, please look the docs [here](https://docs.nebuly.com/Speedster/getting_started/diffusers_getting_started/).
 
 In this section, we will learn about the 4 main steps needed to optimize Stable Diffusion models from the Diffusers library:
 
 1) Input your model and data
 2) Run the optimization
 3) Save your optimized model 
 4) Load and run your optimized model in production
@@ -348,15 +351,15 @@
 - [Notebooks](https://github.com/nebuly-ai/nebullvm/tree/main/notebooks/speedster)
 - [Advanced options](https://docs.nebuly.com/Speedster/advanced_options/)
 - [Benchmarks](https://docs.nebuly.com/Speedster/benchmarks/)
 
 
 # **Key concepts**
 
-`Speedster`'s design reflects our mission to automatically master each and every existing AI acceleration technique to deliver the **fastest AI ever**. As a result, `Speedster` leverages available enterprise-grade open-source optimization tools. If these tools and  communities already exist, and are distributed under a permissive license (Apache, MIT, etc), we integrate them and happily contribute to their communities. However, many tools do not exist yet, in which case we implement them and open-source the code so that our community can benefit from it.
+Speedster's design reflects our mission to automatically master each and every existing AI acceleration technique to deliver the most cost-efficient AI ever. As a result, `Speedster` leverages available enterprise-grade open-source optimization tools. If these tools and  communities already exist, and are distributed under a permissive license (Apache, MIT, etc), we integrate them and happily contribute to their communities. However, many tools do not exist yet, in which case we implement them and open-source the code so that our community can benefit from it.
 
 `Speedster` is shaped around **4 building blocks** and leverages a modular design to foster scalability and integration of new acceleration components across the software to hardware stack.
 
 - [x]  **Converter:** converts the input model from its original framework to the framework backends supported by `Speedster`, namely PyTorch, ONNX and TensorFlow. This allows the Compressor and Compiler modules to apply any optimization technique to the model.
 - [x]  **Compressor:** applies various compression techniques to the model, such as pruning, knowledge distillation, or quantization-aware training.
 - [x]  **Compiler:** converts the compressed models to the intermediate representation (IR) of the supported deep learning compilers. The compilers apply both post-training quantization techniques and graph optimizations, to produce compiled binary files.
 - [x]  **Inference Learner:** takes the best performing compiled model and converts it back into the same interface as the original input model.
```

### Comparing `speedster-0.3.0/speedster/api/functions.py` & `speedster-0.4.0/speedster/api/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,22 +120,20 @@
     """
     root_op = SpeedsterRootOp()
     device = check_device(device)
 
     disable_log = True if not debug_mode_enabled() else False
 
     with LoggingContext(logging.getLogger(), disabled=disable_log):
-        root_op.to(device).execute(
+        return root_op.to(device).execute(
             model=model,
             input_data=input_data,
             metric_drop_ths=metric_drop_ths,
             metric=metric,
             optimization_time=optimization_time,
             dynamic_info=dynamic_info,
             config_file=config_file,
             ignore_compilers=ignore_compilers,
             ignore_compressors=ignore_compressors,
             store_latencies=store_latencies,
             **kwargs,
         )
-
-    return root_op.get_result()
```

### Comparing `speedster-0.3.0/speedster/api/tests/test_huggingface.py` & `speedster-0.4.0/speedster/api/tests/test_huggingface.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,26 +58,26 @@
     model.to(device)
     res_original = model(**inputs)
     res_optimized = optimized_model(**inputs)
 
     assert isinstance(optimized_model, HuggingFaceInferenceLearner)
 
     assert (
-        torch.max(
+        torch.mean(
             abs(
                 (
                     res_original["last_hidden_state"]
                     - res_optimized["last_hidden_state"]
                 )
             )
         )
         < 1e-2
     )
     assert (
-        torch.max(
+        torch.mean(
             abs(
                 (
                     res_original["pooler_output"]
                     - res_optimized["pooler_output"]
                 )
             )
         )
@@ -122,26 +122,26 @@
     model.to(device)
     res_original = model(**inputs)
     res_optimized = optimized_model(**inputs)
 
     assert isinstance(optimized_model, HuggingFaceInferenceLearner)
 
     assert (
-        torch.max(
+        torch.mean(
             abs(
                 (
                     res_original["last_hidden_state"]
                     - res_optimized["last_hidden_state"]
                 )
             )
         )
         < 1e-2
     )
     assert (
-        torch.max(
+        torch.mean(
             abs(
                 (
                     res_original["pooler_output"]
                     - res_optimized["pooler_output"]
                 )
             )
         )
@@ -185,16 +185,16 @@
     inputs = tokenizer(x, return_tensors="pt").to(device)
     model.to(device)
     res_original = model(**inputs)
     res_optimized = optimized_model(**inputs)
 
     assert isinstance(optimized_model, HuggingFaceInferenceLearner)
 
-    assert torch.max(abs((res_original[0] - res_optimized[0]))) < 1e-2
-    assert torch.max(abs((res_original[1] - res_optimized[1]))) < 1e-2
+    assert torch.mean(abs((res_original[0] - res_optimized[0]))) < 1e-2
+    assert torch.mean(abs((res_original[1] - res_optimized[1]))) < 1e-2
 
 
 def test_tensorflow_huggingface_ort_input_text_np():
     tokenizer = AlbertTokenizer.from_pretrained("albert-base-v1")
     model = TFAlbertModel.from_pretrained("albert-base-v1")
 
     input_data = [
```

### Comparing `speedster-0.3.0/speedster/api/tests/test_onnx.py` & `speedster-0.4.0/speedster/api/tests/test_onnx.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,30 +41,29 @@
             input_data=input_data,
             ignore_compilers=[
                 compiler
                 for compiler in COMPILER_LIST
                 if compiler != "onnxruntime"
             ],
             ignore_compressors=[compressor for compressor in COMPRESSOR_LIST],
-            # metric_drop_ths=2,
         )
 
         with TemporaryDirectory() as tmp_dir:
             optimized_model.save(tmp_dir)
             loaded_model = load_model(tmp_dir)
             assert isinstance(loaded_model, NumpyONNXInferenceLearner)
 
             assert isinstance(loaded_model.get_size(), int)
 
             # Try the optimized model
             device = torch.device(
                 "cuda" if torch.cuda.is_available() else "cpu"
             )
             x = torch.randn(1, 3, 256, 256, requires_grad=False)
-            model.eval()
+            model.to(device).eval()
             with torch.inference_mode():
                 res_original = model(x.to(device))
             res_optimized = optimized_model(x.numpy())[0]
 
             assert (
                 abs(
                     (res_original.detach().cpu().numpy() - res_optimized)
@@ -95,15 +94,15 @@
             ],
             ignore_compressors=[compressor for compressor in COMPRESSOR_LIST],
             metric_drop_ths=2,
         )
 
         # Try the optimized model
         device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-        model.eval()
+        model.to(device).eval()
         x = torch.randn(1, 3, 256, 256, requires_grad=False)
         with torch.inference_mode():
             res_original = model(x.to(device))
         res_optimized = optimized_model(x.numpy())[0]
 
         assert isinstance(optimized_model, NumpyONNXInferenceLearner)
         assert (
@@ -138,15 +137,15 @@
             ],
             ignore_compressors=[compressor for compressor in COMPRESSOR_LIST],
         )
 
         # Try the optimized model
         device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
         x = torch.randn(1, 3, 256, 256, requires_grad=False)
-        model.eval()
+        model.to(device).eval()
         with torch.inference_mode():
             res_original = model(x.to(device))
         res_optimized = optimized_model(x.numpy())[0]
 
         assert isinstance(optimized_model, NumpyONNXTensorRTInferenceLearner)
         assert (
             abs((res_original.detach().cpu().numpy() - res_optimized)).max()
@@ -181,15 +180,15 @@
             ignore_compressors=[compressor for compressor in COMPRESSOR_LIST],
             device="cpu",
         )
 
         # Try the optimized model
         device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
         x = torch.randn(1, 3, 256, 256, requires_grad=False)
-        model.eval()
+        model.to(device).eval()
         with torch.inference_mode():
             res_original = model(x.to(device))
         res_optimized = optimized_model(x.numpy())[0]
 
         assert isinstance(optimized_model, NumpyOpenVinoInferenceLearner)
         assert (
             abs((res_original.detach().cpu().numpy() - res_optimized)).max()
@@ -220,15 +219,15 @@
             ],
             ignore_compressors=[compressor for compressor in COMPRESSOR_LIST],
         )
 
         # Try the optimized model
         device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
         x = torch.randn(1, 3, 256, 256, requires_grad=False)
-        model.eval()
+        model.to(device).eval()
         with torch.inference_mode():
             res_original = model(x.to(device))
         res_optimized = optimized_model(x.numpy())[0]
 
         assert isinstance(optimized_model, NumpyApacheTVMInferenceLearner)
         assert (
             abs((res_original.detach().cpu().numpy() - res_optimized)).max()
```

### Comparing `speedster-0.3.0/speedster/api/tests/test_pytorch.py` & `speedster-0.4.0/speedster/api/tests/test_pytorch.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,31 +10,36 @@
 )
 from nebullvm.operations.inference_learners.onnx import (
     PytorchONNXInferenceLearner,
 )
 from nebullvm.operations.inference_learners.openvino import (
     PytorchOpenVinoInferenceLearner,
 )
-from nebullvm.operations.inference_learners.pytorch import (
-    PytorchBackendInferenceLearner,
-)
 from nebullvm.operations.inference_learners.tensor_rt import (
     PytorchTensorRTInferenceLearner,
     PytorchONNXTensorRTInferenceLearner,
 )
+from nebullvm.operations.inference_learners.torch_dynamo import (
+    TorchDynamoInferenceLearner,
+)
+from nebullvm.operations.inference_learners.torchscript import (
+    TorchScriptInferenceLearner,
+)
 from nebullvm.operations.inference_learners.tvm import (
     PytorchApacheTVMInferenceLearner,
 )
 from nebullvm.operations.optimizations.compilers.utils import (
     tvm_is_available,
     bladedisc_is_available,
 )
 
 from speedster import optimize_model, load_model
 
+from nebullvm.tools.utils import check_module_version
+
 
 def test_torch_ort():
     model = models.resnet18()
     input_data = [((torch.randn(1, 3, 256, 256),), 0) for i in range(100)]
 
     # Run nebullvm optimization in one line of code
     optimized_model = optimize_model(
@@ -107,22 +112,57 @@
     # Try the optimized model
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
     x = torch.randn(1, 3, 256, 256, requires_grad=False).to(device)
     model.to(device).eval()
     res_original = model(x)
     res_optimized = optimized_model(x)[0]
 
-    assert isinstance(optimized_model, PytorchBackendInferenceLearner)
+    assert isinstance(optimized_model, TorchScriptInferenceLearner)
+    assert torch.max(abs((res_original - res_optimized))) < 1e-2
+
+
+@pytest.mark.skipif(
+    not check_module_version(torch, min_version="2.0.0") or True,
+    reason="Torch version is not supported",
+)
+def test_torch_torch_dynamo():
+    model = models.resnet18()
+    input_data = [((torch.randn(1, 3, 256, 256),), 0) for i in range(100)]
+
+    # Run nebullvm optimization in one line of code
+    optimized_model = optimize_model(
+        model,
+        input_data=input_data,
+        ignore_compilers=[
+            compiler
+            for compiler in COMPILER_LIST
+            if compiler != "torch_dynamo"
+        ],
+        ignore_compressors=[compressor for compressor in COMPRESSOR_LIST],
+    )
+
+    # Try the optimized model
+    device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+    x = torch.randn(1, 3, 256, 256, requires_grad=False).to(device)
+    model.to(device).eval()
+    res_original = model(x)
+    res_optimized = optimized_model(x)[0]
+
+    assert isinstance(optimized_model, TorchDynamoInferenceLearner)
     assert torch.max(abs((res_original - res_optimized))) < 1e-2
 
 
 @pytest.mark.skipif(
     not torch.cuda.is_available(),
     reason="Skip because cuda is not available.",
 )
+@pytest.mark.skipif(
+    not check_module_version(torch, max_version="1.13.1+cu117"),
+    reason="Skip because torch version is not supported.",
+)
 def test_torch_tensorrt():
     model = models.resnet18()
     input_data = [((torch.randn(1, 3, 256, 256),), 0) for i in range(100)]
 
     # Run nebullvm optimization in one line of code
     optimized_model = optimize_model(
         model,
@@ -219,13 +259,13 @@
         ],
         ignore_compressors=[compressor for compressor in COMPRESSOR_LIST],
     )
 
     # Try the optimized model
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
     x = torch.randn(1, 3, 256, 256, requires_grad=False).to(device)
-    model.eval()
+    model.to(device).eval()
     res_original = model(x)
     res_optimized = optimized_model(x)[0]
 
     assert isinstance(optimized_model, BladeDISCInferenceLearner)
     assert torch.max(abs((res_original - res_optimized))) < 1e-2
```

### Comparing `speedster-0.3.0/speedster/api/tests/test_tensorflow.py` & `speedster-0.4.0/speedster/api/tests/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `speedster-0.3.0/speedster/api/tests/utils.py` & `speedster-0.4.0/speedster/api/tests/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from pathlib import Path
 
+from nebullvm.core.models import ModelParams, Device, DeviceType
 from nebullvm.operations.conversions.pytorch import convert_torch_to_onnx
-from nebullvm.tools.base import ModelParams, Device, DeviceType
 from nebullvm.tools.data import DataManager
 from nebullvm.tools.utils import gpu_is_available
 
 
 def torch_to_onnx(model, input_data, output_path):
     model_params = ModelParams(1, [], [], [])
     output_path = os.path.join(output_path, "model.onnx")
```

### Comparing `speedster-0.3.0/speedster.egg-info/PKG-INFO` & `speedster-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,22 @@
-Metadata-Version: 2.1
-Name: speedster
-Version: 0.3.0
-Description-Content-Type: text/markdown
-
 # 💥 Speedster
 
-`Speedster` is an open-source module designed to speed up AI inference in just a few lines of code. The library automatically applies the best set of SOTA optimization techniques to achieve the maximum inference speed-up (latency, throughput, model size) physically possible on your hardware (single machine).
+`Speedster` reduces inference costs by leveraging SOTA optimization techniques that best couple your AI models with the underlying hardware (GPUs and CPUs). The idea is to make AI inference way cheaper in just a few lines of code.
 
-`Speedster` makes it easy to combine optimization techniques across the whole software-to-hardware stack, delivering best-in-class speed-ups. If you like the idea, give us a star to support the project ⭐
+`Speedster` makes it easy to combine optimization techniques across the whole software-to-hardware stack, delivering best-in-class cost savings. If you like the idea, give us a star to support the project ⭐
 
 ![speedster](https://user-images.githubusercontent.com/53374883/225599469-f1a626f0-c001-42bd-bc8b-ec0e966ddad6.png)
 
 The core `Speedster` workflow consists of 3 steps:
 
-
 - [x]  **Select**: input your model in your preferred DL framework and express your preferences regarding:
-    - Accuracy loss: do you want to trade off a little accuracy for much higher performance?
-    - Optimization time: stellar accelerations can be time-consuming. Can you wait, or do you need an instant answer?
+    - Accuracy loss: do you want to trade off a little accuracy for significant cost savings?
+    - Optimization time: achieving great savings can be time-consuming. Can you wait, or do you need an instant answer?
 - [x]  **Search**: the library automatically tests every combination of optimization techniques across the software-to-hardware stack (sparsity, quantization, compilers, etc.) that is compatible with your needs and local hardware.
-- [x]  **Serve**: finally, `Speedster` chooses the best configuration of optimization techniques and returns an accelerated version of your model in the DL framework of your choice (just on steroids 🚀).
-
+- [x]  **Serve**: finally, `Speedster` chooses the best configuration of optimization techniques and returns an accelerated version of your model in the DL framework of your choice (just cheaper 🚀).
 
 # Installation
 
 Install `Speedster` and its base requirements:
 ```
 pip install speedster
 ```
@@ -185,15 +178,15 @@
     </details>
     
 </details>
 
 <details>
 <summary>🧨 Hugging Face Diffusers </summary>
 
-> :warning: In order to work properly, the diffusers optimization requires `CUDA>=12.0` and `tensorrt>=8.6.0`. For additional details, please look the docs [here](https://docs.nebuly.com/Speedster/getting_started/diffusers_getting_started/).
+> :warning: In order to work properly, the diffusers optimization requires `CUDA>=12.0`, `tensorrt>=8.6.0` and `torch<=1.13.1`. For additional details, please look the docs [here](https://docs.nebuly.com/Speedster/getting_started/diffusers_getting_started/).
 
 In this section, we will learn about the 4 main steps needed to optimize Stable Diffusion models from the Diffusers library:
 
 1) Input your model and data
 2) Run the optimization
 3) Save your optimized model 
 4) Load and run your optimized model in production
@@ -353,15 +346,15 @@
 - [Notebooks](https://github.com/nebuly-ai/nebullvm/tree/main/notebooks/speedster)
 - [Advanced options](https://docs.nebuly.com/Speedster/advanced_options/)
 - [Benchmarks](https://docs.nebuly.com/Speedster/benchmarks/)
 
 
 # **Key concepts**
 
-`Speedster`'s design reflects our mission to automatically master each and every existing AI acceleration technique to deliver the **fastest AI ever**. As a result, `Speedster` leverages available enterprise-grade open-source optimization tools. If these tools and  communities already exist, and are distributed under a permissive license (Apache, MIT, etc), we integrate them and happily contribute to their communities. However, many tools do not exist yet, in which case we implement them and open-source the code so that our community can benefit from it.
+Speedster's design reflects our mission to automatically master each and every existing AI acceleration technique to deliver the most cost-efficient AI ever. As a result, `Speedster` leverages available enterprise-grade open-source optimization tools. If these tools and  communities already exist, and are distributed under a permissive license (Apache, MIT, etc), we integrate them and happily contribute to their communities. However, many tools do not exist yet, in which case we implement them and open-source the code so that our community can benefit from it.
 
 `Speedster` is shaped around **4 building blocks** and leverages a modular design to foster scalability and integration of new acceleration components across the software to hardware stack.
 
 - [x]  **Converter:** converts the input model from its original framework to the framework backends supported by `Speedster`, namely PyTorch, ONNX and TensorFlow. This allows the Compressor and Compiler modules to apply any optimization technique to the model.
 - [x]  **Compressor:** applies various compression techniques to the model, such as pruning, knowledge distillation, or quantization-aware training.
 - [x]  **Compiler:** converts the compressed models to the intermediate representation (IR) of the supported deep learning compilers. The compilers apply both post-training quantization techniques and graph optimizations, to produce compiled binary files.
 - [x]  **Inference Learner:** takes the best performing compiled model and converts it back into the same interface as the original input model.
```

### Comparing `speedster-0.3.0/speedster.egg-info/SOURCES.txt` & `speedster-0.4.0/speedster.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -12,8 +12,10 @@
 speedster/api/__init__.py
 speedster/api/functions.py
 speedster/api/tests/__init__.py
 speedster/api/tests/test_huggingface.py
 speedster/api/tests/test_onnx.py
 speedster/api/tests/test_pytorch.py
 speedster/api/tests/test_tensorflow.py
-speedster/api/tests/utils.py
+speedster/api/tests/utils.py
+speedster/tests/__init__.py
+speedster/tests/test_root_op.py
```

