# Comparing `tmp/nebullvm-0.9.0.tar.gz` & `tmp/nebullvm-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nebullvm-0.9.0.tar", last modified: Tue Mar 21 12:54:53 2023, max compression
+gzip compressed data, was "nebullvm-0.9.1.tar", last modified: Tue Mar 21 15:48:21 2023, max compression
```

## Comparing `nebullvm-0.9.0.tar` & `nebullvm-0.9.1.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:54:53.757123 nebullvm-0.9.0/
--rw-r--r--   0 diegofiori   (501) staff       (20)    11357 2022-02-12 17:19:29.000000 nebullvm-0.9.0/LICENSE
--rw-r--r--   0 diegofiori   (501) staff       (20)      103 2022-10-19 13:49:59.000000 nebullvm-0.9.0/MANIFEST.in
--rw-r--r--   0 diegofiori   (501) staff       (20)     4338 2023-03-21 12:54:53.756973 nebullvm-0.9.0/PKG-INFO
--rw-r--r--   0 diegofiori   (501) staff       (20)     4223 2023-03-08 18:43:55.000000 nebullvm-0.9.0/README.md
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:54:53.729265 nebullvm-0.9.0/nebullvm/
--rw-r--r--   0 diegofiori   (501) staff       (20)      129 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/__init__.py
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:54:53.730053 nebullvm-0.9.0/nebullvm/api/
--rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-02-17 10:31:51.000000 nebullvm-0.9.0/nebullvm/api/__init__.py
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:54:53.730222 nebullvm-0.9.0/nebullvm/apps/
--rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-12-16 18:45:48.000000 nebullvm-0.9.0/nebullvm/apps/__init__.py
--rw-r--r--   0 diegofiori   (501) staff       (20)      178 2022-12-16 18:45:48.000000 nebullvm-0.9.0/nebullvm/apps/base.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     2021 2023-03-21 12:53:44.000000 nebullvm-0.9.0/nebullvm/config.py
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:54:53.731779 nebullvm-0.9.0/nebullvm/installers/
--rw-r--r--   0 diegofiori   (501) staff       (20)      329 2022-10-19 13:49:59.000000 nebullvm-0.9.0/nebullvm/installers/__init__.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     6556 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/installers/auto_installer.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     1196 2022-10-19 13:49:59.000000 nebullvm-0.9.0/nebullvm/installers/install_bladedisc.sh
--rw-r--r--   0 diegofiori   (501) staff       (20)     2114 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/installers/install_tensor_rt.sh
--rw-r--r--   0 diegofiori   (501) staff       (20)      600 2022-10-19 13:49:59.000000 nebullvm-0.9.0/nebullvm/installers/install_tvm.sh
--rw-r--r--   0 diegofiori   (501) staff       (20)     1174 2022-04-26 21:58:32.000000 nebullvm-0.9.0/nebullvm/installers/install_tvm_prerequisites.sh
--rw-r--r--   0 diegofiori   (501) staff       (20)    15233 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/installers/installers.py
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:54:53.732067 nebullvm-0.9.0/nebullvm/installers/tests/
--rw-r--r--   0 diegofiori   (501) staff       (20)        0 2023-01-06 15:52:28.000000 nebullvm-0.9.0/nebullvm/installers/tests/__init__.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     5767 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/installers/tests/test_install_frameworks.py
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:54:53.722861 nebullvm-0.9.0/nebullvm/installers/tvm_installers/
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:54:53.732256 nebullvm-0.9.0/nebullvm/installers/tvm_installers/arm/
--rw-r--r--   0 diegofiori   (501) staff       (20)    11553 2021-12-22 14:06:00.000000 nebullvm-0.9.0/nebullvm/installers/tvm_installers/arm/config.cmake
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:54:53.732487 nebullvm-0.9.0/nebullvm/installers/tvm_installers/arm_cuda/
--rw-r--r--   0 diegofiori   (501) staff       (20)    11552 2021-12-22 14:06:00.000000 nebullvm-0.9.0/nebullvm/installers/tvm_installers/arm_cuda/config.cmake
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:54:53.732741 nebullvm-0.9.0/nebullvm/installers/tvm_installers/x86/
--rw-r--r--   0 diegofiori   (501) staff       (20)    11553 2021-12-22 14:06:00.000000 nebullvm-0.9.0/nebullvm/installers/tvm_installers/x86/config.cmake
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:54:53.732931 nebullvm-0.9.0/nebullvm/installers/tvm_installers/x86_cuda/
--rw-r--r--   0 diegofiori   (501) staff       (20)    11552 2021-12-22 14:06:00.000000 nebullvm-0.9.0/nebullvm/installers/tvm_installers/x86_cuda/config.cmake
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:54:53.733256 nebullvm-0.9.0/nebullvm/operations/
--rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-12-16 18:45:48.000000 nebullvm-0.9.0/nebullvm/operations/__init__.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     1209 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/base.py
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:54:53.734008 nebullvm-0.9.0/nebullvm/operations/conversions/
--rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-12-16 18:45:48.000000 nebullvm-0.9.0/nebullvm/operations/conversions/__init__.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     4307 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/operations/conversions/converters.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     5256 2023-01-05 10:07:54.000000 nebullvm-0.9.0/nebullvm/operations/conversions/huggingface.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     5687 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/operations/conversions/pytorch.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     3916 2023-03-11 13:48:08.000000 nebullvm-0.9.0/nebullvm/operations/conversions/tensorflow.py
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:54:53.734321 nebullvm-0.9.0/nebullvm/operations/fetch_operations/
--rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-12-16 18:45:48.000000 nebullvm-0.9.0/nebullvm/operations/fetch_operations/__init__.py
--rw-r--r--   0 diegofiori   (501) staff       (20)      574 2022-12-16 18:45:48.000000 nebullvm-0.9.0/nebullvm/operations/fetch_operations/local.py
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:54:53.737346 nebullvm-0.9.0/nebullvm/operations/inference_learners/
--rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-12-16 18:45:48.000000 nebullvm-0.9.0/nebullvm/operations/inference_learners/__init__.py
--rw-r--r--   0 diegofiori   (501) staff       (20)    20475 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/inference_learners/base.py
--rw-r--r--   0 diegofiori   (501) staff       (20)      909 2023-01-05 10:07:54.000000 nebullvm-0.9.0/nebullvm/operations/inference_learners/blade_disc.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     9014 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/inference_learners/builders.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     6167 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/inference_learners/deepsparse.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     4286 2022-12-16 18:45:48.000000 nebullvm-0.9.0/nebullvm/operations/inference_learners/huggingface.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     6189 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/inference_learners/neural_compressor.py
--rw-r--r--   0 diegofiori   (501) staff       (20)    14863 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/inference_learners/onnx.py
--rw-r--r--   0 diegofiori   (501) staff       (20)    15049 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/inference_learners/openvino.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     4174 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/inference_learners/pytorch.py
--rw-r--r--   0 diegofiori   (501) staff       (20)    23322 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/operations/inference_learners/tensor_rt.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     4740 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/inference_learners/tensorflow.py
--rw-r--r--   0 diegofiori   (501) staff       (20)    16684 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/inference_learners/tvm.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     1482 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/operations/inference_learners/utils.py
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:54:53.737958 nebullvm-0.9.0/nebullvm/operations/measures/
--rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-12-16 18:45:48.000000 nebullvm-0.9.0/nebullvm/operations/measures/__init__.py
--rw-r--r--   0 diegofiori   (501) staff       (20)      417 2022-12-16 18:45:48.000000 nebullvm-0.9.0/nebullvm/operations/measures/base.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     3695 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/operations/measures/measures.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     7992 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/measures/utils.py
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:54:53.745028 nebullvm-0.9.0/nebullvm/operations/optimizations/
--rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-12-16 18:45:48.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/__init__.py
--rw-r--r--   0 diegofiori   (501) staff       (20)    15276 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/base.py
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:54:53.747118 nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/
--rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-12-16 18:45:48.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/__init__.py
--rw-r--r--   0 diegofiori   (501) staff       (20)      721 2022-12-16 18:45:48.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/base.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     2548 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/deepsparse.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     3134 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/intel_neural_compressor.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     3104 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/onnxruntime.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     4829 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/openvino.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     4676 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/pytorch.py
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:54:53.748776 nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/quantizations/
--rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-12-16 18:45:48.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/quantizations/__init__.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     3780 2022-12-16 18:45:48.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/quantizations/intel_neural_compressor.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     4940 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/quantizations/onnx.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     1960 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/quantizations/openvino.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     5089 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/quantizations/pytorch.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     2263 2023-01-30 07:58:21.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/quantizations/tensor_rt.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     1761 2022-12-16 18:45:48.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/quantizations/tensorflow.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     2236 2022-12-16 18:45:48.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/quantizations/tvm.py
--rw-r--r--   0 diegofiori   (501) staff       (20)      405 2023-01-13 13:47:01.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/quantizations/utils.py
--rw-r--r--   0 diegofiori   (501) staff       (20)    16819 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/tensor_rt.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     5205 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/tensorflow.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     8750 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/tvm.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     3153 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/utils.py
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:54:53.749411 nebullvm-0.9.0/nebullvm/operations/optimizations/compressors/
--rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-12-16 18:45:48.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/compressors/__init__.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     1379 2022-12-16 18:45:48.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/compressors/base.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     5966 2022-12-16 18:45:48.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/compressors/intel.py
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:54:53.749877 nebullvm-0.9.0/nebullvm/operations/optimizations/compressors/scripts/
--rw-r--r--   0 diegofiori   (501) staff       (20)    11416 2022-12-16 18:45:48.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/compressors/scripts/__init__.py
--rw-r--r--   0 diegofiori   (501) staff       (20)    11416 2022-12-16 18:45:48.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/compressors/scripts/neural_magic_training.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     4598 2023-01-13 13:47:01.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/compressors/sparseml.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     2746 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/optimizers.py
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:54:53.751289 nebullvm-0.9.0/nebullvm/operations/optimizations/tests/
--rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-12-16 18:45:48.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/tests/__init__.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     4139 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/tests/test_deepsparse.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     4311 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/tests/test_intel_neural_compressor.py
--rw-r--r--   0 diegofiori   (501) staff       (20)    14813 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/tests/test_onnxruntime.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     5212 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/tests/test_openvino.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     9098 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/tests/test_tensor_rt.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     6897 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/tests/test_tensorflow.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     6223 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/tests/test_torchscript.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     8831 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/tests/test_tvm.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     9667 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/tests/utils.py
--rw-r--r--   0 diegofiori   (501) staff       (20)      269 2023-01-23 23:00:29.000000 nebullvm-0.9.0/nebullvm/operations/optimizations/utils.py
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:54:53.753611 nebullvm-0.9.0/nebullvm/optional_modules/
--rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-11-10 18:55:07.000000 nebullvm-0.9.0/nebullvm/optional_modules/__init__.py
--rw-r--r--   0 diegofiori   (501) staff       (20)      133 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/optional_modules/blade_disc.py
--rw-r--r--   0 diegofiori   (501) staff       (20)      164 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/optional_modules/deepsparse.py
--rw-r--r--   0 diegofiori   (501) staff       (20)      701 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/optional_modules/diffusers.py
--rw-r--r--   0 diegofiori   (501) staff       (20)       27 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/optional_modules/dummy.py
--rw-r--r--   0 diegofiori   (501) staff       (20)      403 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/optional_modules/huggingface.py
--rw-r--r--   0 diegofiori   (501) staff       (20)      620 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/optional_modules/neural_compressor.py
--rw-r--r--   0 diegofiori   (501) staff       (20)      366 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/optional_modules/onnx.py
--rw-r--r--   0 diegofiori   (501) staff       (20)      813 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/optional_modules/onnxruntime.py
--rw-r--r--   0 diegofiori   (501) staff       (20)      125 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/optional_modules/onnxsim.py
--rw-r--r--   0 diegofiori   (501) staff       (20)      819 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/optional_modules/openvino.py
--rw-r--r--   0 diegofiori   (501) staff       (20)      484 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/optional_modules/tensor_rt.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     1187 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/optional_modules/tensorflow.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     1246 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/optional_modules/torch.py
--rw-r--r--   0 diegofiori   (501) staff       (20)      240 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/optional_modules/torch_tensorrt.py
--rw-r--r--   0 diegofiori   (501) staff       (20)      687 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/optional_modules/tvm.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     6001 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/optional_modules/utils.py
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:54:53.756397 nebullvm-0.9.0/nebullvm/tools/
--rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-12-16 18:45:48.000000 nebullvm-0.9.0/nebullvm/tools/__init__.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     8168 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/tools/base.py
--rw-r--r--   0 diegofiori   (501) staff       (20)    10851 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/tools/benchmark.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     7226 2023-01-23 21:57:41.000000 nebullvm-0.9.0/nebullvm/tools/data.py
--rw-r--r--   0 diegofiori   (501) staff       (20)    26833 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/tools/diffusers.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     2109 2023-01-01 22:23:50.000000 nebullvm-0.9.0/nebullvm/tools/feedback_collector.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     6333 2023-02-15 12:55:17.000000 nebullvm-0.9.0/nebullvm/tools/huggingface.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     1561 2023-01-13 13:47:01.000000 nebullvm-0.9.0/nebullvm/tools/logger.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     5196 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/tools/onnx.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     5952 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/tools/pytorch.py
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:54:53.756710 nebullvm-0.9.0/nebullvm/tools/tests/
--rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-12-16 18:45:48.000000 nebullvm-0.9.0/nebullvm/tools/tests/__init__.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     5008 2022-12-16 18:45:48.000000 nebullvm-0.9.0/nebullvm/tools/tests/test_data.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     4185 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/tools/tf.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     3494 2022-12-16 18:45:48.000000 nebullvm-0.9.0/nebullvm/tools/transformations.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     7625 2023-03-21 12:50:34.000000 nebullvm-0.9.0/nebullvm/tools/utils.py
--rw-r--r--   0 diegofiori   (501) staff       (20)     2346 2023-01-13 13:47:01.000000 nebullvm-0.9.0/nebullvm/tools/venv.py
-drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 12:54:53.729937 nebullvm-0.9.0/nebullvm.egg-info/
--rw-r--r--   0 diegofiori   (501) staff       (20)     4338 2023-03-21 12:54:53.000000 nebullvm-0.9.0/nebullvm.egg-info/PKG-INFO
--rw-r--r--   0 diegofiori   (501) staff       (20)     5626 2023-03-21 12:54:53.000000 nebullvm-0.9.0/nebullvm.egg-info/SOURCES.txt
--rw-r--r--   0 diegofiori   (501) staff       (20)        1 2023-03-21 12:54:53.000000 nebullvm-0.9.0/nebullvm.egg-info/dependency_links.txt
--rw-r--r--   0 diegofiori   (501) staff       (20)      126 2023-03-21 12:54:53.000000 nebullvm-0.9.0/nebullvm.egg-info/requires.txt
--rw-r--r--   0 diegofiori   (501) staff       (20)        9 2023-03-21 12:54:53.000000 nebullvm-0.9.0/nebullvm.egg-info/top_level.txt
--rw-r--r--   0 diegofiori   (501) staff       (20)       38 2023-03-21 12:54:53.757171 nebullvm-0.9.0/setup.cfg
--rw-r--r--   0 diegofiori   (501) staff       (20)      628 2023-03-21 12:53:44.000000 nebullvm-0.9.0/setup.py
+drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 15:48:21.673322 nebullvm-0.9.1/
+-rw-r--r--   0 diegofiori   (501) staff       (20)    11357 2022-02-12 17:19:29.000000 nebullvm-0.9.1/LICENSE
+-rw-r--r--   0 diegofiori   (501) staff       (20)      103 2022-10-19 13:49:59.000000 nebullvm-0.9.1/MANIFEST.in
+-rw-r--r--   0 diegofiori   (501) staff       (20)     4338 2023-03-21 15:48:21.673181 nebullvm-0.9.1/PKG-INFO
+-rw-r--r--   0 diegofiori   (501) staff       (20)     4223 2023-03-08 18:43:55.000000 nebullvm-0.9.1/README.md
+drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 15:48:21.646066 nebullvm-0.9.1/nebullvm/
+-rw-r--r--   0 diegofiori   (501) staff       (20)      129 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/__init__.py
+drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 15:48:21.646835 nebullvm-0.9.1/nebullvm/api/
+-rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-02-17 10:31:51.000000 nebullvm-0.9.1/nebullvm/api/__init__.py
+drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 15:48:21.647012 nebullvm-0.9.1/nebullvm/apps/
+-rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-12-16 18:45:48.000000 nebullvm-0.9.1/nebullvm/apps/__init__.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)      178 2022-12-16 18:45:48.000000 nebullvm-0.9.1/nebullvm/apps/base.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     2021 2023-03-21 15:47:04.000000 nebullvm-0.9.1/nebullvm/config.py
+drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 15:48:21.648655 nebullvm-0.9.1/nebullvm/installers/
+-rw-r--r--   0 diegofiori   (501) staff       (20)      329 2022-10-19 13:49:59.000000 nebullvm-0.9.1/nebullvm/installers/__init__.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     6556 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/installers/auto_installer.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     1196 2022-10-19 13:49:59.000000 nebullvm-0.9.1/nebullvm/installers/install_bladedisc.sh
+-rw-r--r--   0 diegofiori   (501) staff       (20)     2114 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/installers/install_tensor_rt.sh
+-rw-r--r--   0 diegofiori   (501) staff       (20)      600 2022-10-19 13:49:59.000000 nebullvm-0.9.1/nebullvm/installers/install_tvm.sh
+-rw-r--r--   0 diegofiori   (501) staff       (20)     1174 2022-04-26 21:58:32.000000 nebullvm-0.9.1/nebullvm/installers/install_tvm_prerequisites.sh
+-rw-r--r--   0 diegofiori   (501) staff       (20)    15567 2023-03-21 15:46:35.000000 nebullvm-0.9.1/nebullvm/installers/installers.py
+drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 15:48:21.648985 nebullvm-0.9.1/nebullvm/installers/tests/
+-rw-r--r--   0 diegofiori   (501) staff       (20)        0 2023-01-06 15:52:28.000000 nebullvm-0.9.1/nebullvm/installers/tests/__init__.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     5767 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/installers/tests/test_install_frameworks.py
+drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 15:48:21.640438 nebullvm-0.9.1/nebullvm/installers/tvm_installers/
+drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 15:48:21.649199 nebullvm-0.9.1/nebullvm/installers/tvm_installers/arm/
+-rw-r--r--   0 diegofiori   (501) staff       (20)    11553 2021-12-22 14:06:00.000000 nebullvm-0.9.1/nebullvm/installers/tvm_installers/arm/config.cmake
+drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 15:48:21.649427 nebullvm-0.9.1/nebullvm/installers/tvm_installers/arm_cuda/
+-rw-r--r--   0 diegofiori   (501) staff       (20)    11552 2021-12-22 14:06:00.000000 nebullvm-0.9.1/nebullvm/installers/tvm_installers/arm_cuda/config.cmake
+drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 15:48:21.649663 nebullvm-0.9.1/nebullvm/installers/tvm_installers/x86/
+-rw-r--r--   0 diegofiori   (501) staff       (20)    11553 2021-12-22 14:06:00.000000 nebullvm-0.9.1/nebullvm/installers/tvm_installers/x86/config.cmake
+drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 15:48:21.649842 nebullvm-0.9.1/nebullvm/installers/tvm_installers/x86_cuda/
+-rw-r--r--   0 diegofiori   (501) staff       (20)    11552 2021-12-22 14:06:00.000000 nebullvm-0.9.1/nebullvm/installers/tvm_installers/x86_cuda/config.cmake
+drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 15:48:21.650175 nebullvm-0.9.1/nebullvm/operations/
+-rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-12-16 18:45:48.000000 nebullvm-0.9.1/nebullvm/operations/__init__.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     1209 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/base.py
+drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 15:48:21.651107 nebullvm-0.9.1/nebullvm/operations/conversions/
+-rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-12-16 18:45:48.000000 nebullvm-0.9.1/nebullvm/operations/conversions/__init__.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     4307 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/operations/conversions/converters.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     5256 2023-01-05 10:07:54.000000 nebullvm-0.9.1/nebullvm/operations/conversions/huggingface.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     5687 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/operations/conversions/pytorch.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     3916 2023-03-11 13:48:08.000000 nebullvm-0.9.1/nebullvm/operations/conversions/tensorflow.py
+drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 15:48:21.651433 nebullvm-0.9.1/nebullvm/operations/fetch_operations/
+-rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-12-16 18:45:48.000000 nebullvm-0.9.1/nebullvm/operations/fetch_operations/__init__.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)      574 2022-12-16 18:45:48.000000 nebullvm-0.9.1/nebullvm/operations/fetch_operations/local.py
+drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 15:48:21.655017 nebullvm-0.9.1/nebullvm/operations/inference_learners/
+-rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-12-16 18:45:48.000000 nebullvm-0.9.1/nebullvm/operations/inference_learners/__init__.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)    20475 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/inference_learners/base.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)      909 2023-01-05 10:07:54.000000 nebullvm-0.9.1/nebullvm/operations/inference_learners/blade_disc.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     9014 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/inference_learners/builders.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     6167 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/inference_learners/deepsparse.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     4286 2022-12-16 18:45:48.000000 nebullvm-0.9.1/nebullvm/operations/inference_learners/huggingface.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     6189 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/inference_learners/neural_compressor.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)    14863 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/inference_learners/onnx.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)    15049 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/inference_learners/openvino.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     4174 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/inference_learners/pytorch.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)    23322 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/operations/inference_learners/tensor_rt.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     4740 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/inference_learners/tensorflow.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)    16684 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/inference_learners/tvm.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     1482 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/operations/inference_learners/utils.py
+drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 15:48:21.655723 nebullvm-0.9.1/nebullvm/operations/measures/
+-rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-12-16 18:45:48.000000 nebullvm-0.9.1/nebullvm/operations/measures/__init__.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)      417 2022-12-16 18:45:48.000000 nebullvm-0.9.1/nebullvm/operations/measures/base.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     3695 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/operations/measures/measures.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     7992 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/measures/utils.py
+drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 15:48:21.661856 nebullvm-0.9.1/nebullvm/operations/optimizations/
+-rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-12-16 18:45:48.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/__init__.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)    15276 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/base.py
+drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 15:48:21.663657 nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/
+-rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-12-16 18:45:48.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/__init__.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)      721 2022-12-16 18:45:48.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/base.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     2548 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/deepsparse.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     3134 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/intel_neural_compressor.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     3104 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/onnxruntime.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     4829 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/openvino.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     4676 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/pytorch.py
+drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 15:48:21.665198 nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/quantizations/
+-rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-12-16 18:45:48.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/quantizations/__init__.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     3780 2022-12-16 18:45:48.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/quantizations/intel_neural_compressor.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     4940 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/quantizations/onnx.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     1960 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/quantizations/openvino.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     5089 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/quantizations/pytorch.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     2263 2023-01-30 07:58:21.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/quantizations/tensor_rt.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     1761 2022-12-16 18:45:48.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/quantizations/tensorflow.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     2236 2022-12-16 18:45:48.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/quantizations/tvm.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)      405 2023-01-13 13:47:01.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/quantizations/utils.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)    16819 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/tensor_rt.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     5205 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/tensorflow.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     8750 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/tvm.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     3153 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/utils.py
+drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 15:48:21.665815 nebullvm-0.9.1/nebullvm/operations/optimizations/compressors/
+-rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-12-16 18:45:48.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/compressors/__init__.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     1379 2022-12-16 18:45:48.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/compressors/base.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     5966 2022-12-16 18:45:48.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/compressors/intel.py
+drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 15:48:21.666286 nebullvm-0.9.1/nebullvm/operations/optimizations/compressors/scripts/
+-rw-r--r--   0 diegofiori   (501) staff       (20)    11416 2022-12-16 18:45:48.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/compressors/scripts/__init__.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)    11416 2022-12-16 18:45:48.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/compressors/scripts/neural_magic_training.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     4598 2023-01-13 13:47:01.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/compressors/sparseml.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     2746 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/optimizers.py
+drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 15:48:21.667674 nebullvm-0.9.1/nebullvm/operations/optimizations/tests/
+-rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-12-16 18:45:48.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/tests/__init__.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     4139 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/tests/test_deepsparse.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     4311 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/tests/test_intel_neural_compressor.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)    14813 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/tests/test_onnxruntime.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     5212 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/tests/test_openvino.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     9098 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/tests/test_tensor_rt.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     6897 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/tests/test_tensorflow.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     6223 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/tests/test_torchscript.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     8831 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/tests/test_tvm.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     9667 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/tests/utils.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)      269 2023-01-23 23:00:29.000000 nebullvm-0.9.1/nebullvm/operations/optimizations/utils.py
+drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 15:48:21.670040 nebullvm-0.9.1/nebullvm/optional_modules/
+-rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-11-10 18:55:07.000000 nebullvm-0.9.1/nebullvm/optional_modules/__init__.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)      133 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/optional_modules/blade_disc.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)      164 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/optional_modules/deepsparse.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)      701 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/optional_modules/diffusers.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)       27 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/optional_modules/dummy.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)      403 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/optional_modules/huggingface.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)      620 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/optional_modules/neural_compressor.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)      366 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/optional_modules/onnx.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)      813 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/optional_modules/onnxruntime.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)      125 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/optional_modules/onnxsim.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)      819 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/optional_modules/openvino.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)      484 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/optional_modules/tensor_rt.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     1187 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/optional_modules/tensorflow.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     1246 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/optional_modules/torch.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)      240 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/optional_modules/torch_tensorrt.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)      687 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/optional_modules/tvm.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     6001 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/optional_modules/utils.py
+drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 15:48:21.672654 nebullvm-0.9.1/nebullvm/tools/
+-rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-12-16 18:45:48.000000 nebullvm-0.9.1/nebullvm/tools/__init__.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     8168 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/tools/base.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)    10851 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/tools/benchmark.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     7226 2023-01-23 21:57:41.000000 nebullvm-0.9.1/nebullvm/tools/data.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)    26833 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/tools/diffusers.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     2109 2023-01-01 22:23:50.000000 nebullvm-0.9.1/nebullvm/tools/feedback_collector.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     6333 2023-02-15 12:55:17.000000 nebullvm-0.9.1/nebullvm/tools/huggingface.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     1561 2023-01-13 13:47:01.000000 nebullvm-0.9.1/nebullvm/tools/logger.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     5196 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/tools/onnx.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     5952 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/tools/pytorch.py
+drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 15:48:21.672946 nebullvm-0.9.1/nebullvm/tools/tests/
+-rw-r--r--   0 diegofiori   (501) staff       (20)        0 2022-12-16 18:45:48.000000 nebullvm-0.9.1/nebullvm/tools/tests/__init__.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     5008 2022-12-16 18:45:48.000000 nebullvm-0.9.1/nebullvm/tools/tests/test_data.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     4185 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/tools/tf.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     3494 2022-12-16 18:45:48.000000 nebullvm-0.9.1/nebullvm/tools/transformations.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     7625 2023-03-21 12:50:34.000000 nebullvm-0.9.1/nebullvm/tools/utils.py
+-rw-r--r--   0 diegofiori   (501) staff       (20)     2346 2023-01-13 13:47:01.000000 nebullvm-0.9.1/nebullvm/tools/venv.py
+drwxr-xr-x   0 diegofiori   (501) staff       (20)        0 2023-03-21 15:48:21.646726 nebullvm-0.9.1/nebullvm.egg-info/
+-rw-r--r--   0 diegofiori   (501) staff       (20)     4338 2023-03-21 15:48:21.000000 nebullvm-0.9.1/nebullvm.egg-info/PKG-INFO
+-rw-r--r--   0 diegofiori   (501) staff       (20)     5626 2023-03-21 15:48:21.000000 nebullvm-0.9.1/nebullvm.egg-info/SOURCES.txt
+-rw-r--r--   0 diegofiori   (501) staff       (20)        1 2023-03-21 15:48:21.000000 nebullvm-0.9.1/nebullvm.egg-info/dependency_links.txt
+-rw-r--r--   0 diegofiori   (501) staff       (20)      126 2023-03-21 15:48:21.000000 nebullvm-0.9.1/nebullvm.egg-info/requires.txt
+-rw-r--r--   0 diegofiori   (501) staff       (20)        9 2023-03-21 15:48:21.000000 nebullvm-0.9.1/nebullvm.egg-info/top_level.txt
+-rw-r--r--   0 diegofiori   (501) staff       (20)       38 2023-03-21 15:48:21.673372 nebullvm-0.9.1/setup.cfg
+-rw-r--r--   0 diegofiori   (501) staff       (20)      628 2023-03-21 15:47:04.000000 nebullvm-0.9.1/setup.py
```

### Comparing `nebullvm-0.9.0/LICENSE` & `nebullvm-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/PKG-INFO` & `nebullvm-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nebullvm
-Version: 0.9.0
+Version: 0.9.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
 <br><br><br>
 <a https://docs.nebuly.com/welcome/quick-start"><img src="https://user-images.githubusercontent.com/83510798/208247207-861541f0-b968-484c-8a0c-0fb110399c16.png" width="400px"></a>
 <br><br><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nebullvm Version: 0.9.0 Description-Content-Type:
+Metadata-Version: 2.1 Name: nebullvm Version: 0.9.1 Description-Content-Type:
 text/markdown License-File: LICENSE
 
 
 
               docs.nebuly.com/welcome/quick-start">[https://user-
    images.githubusercontent.com/83510798/208247207-861541f0-b968-484c-8a0c-
                                0fb110399c16.png]
```

### Comparing `nebullvm-0.9.0/README.md` & `nebullvm-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/config.py` & `nebullvm-0.9.1/nebullvm/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from nebullvm.optional_modules.torch import torch
 
 
-VERSION = "0.9.0"
+VERSION = "0.9.1"
 LEARNER_METADATA_FILENAME = "metadata.json"
 ONNX_OPSET_VERSION = 13
 NEBULLVM_DEBUG_FILE = "nebullvm_debug.json"
 
 AUTO_TVM_TUNING_OPTION = {
     "tuner": "xgb",
     "trials": 10,
```

### Comparing `nebullvm-0.9.0/nebullvm/installers/auto_installer.py` & `nebullvm-0.9.1/nebullvm/installers/auto_installer.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/installers/install_bladedisc.sh` & `nebullvm-0.9.1/nebullvm/installers/install_bladedisc.sh`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/installers/install_tensor_rt.sh` & `nebullvm-0.9.1/nebullvm/installers/install_tensor_rt.sh`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/installers/install_tvm.sh` & `nebullvm-0.9.1/nebullvm/installers/install_tvm.sh`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/installers/install_tvm_prerequisites.sh` & `nebullvm-0.9.1/nebullvm/installers/install_tvm_prerequisites.sh`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/installers/installers.py` & `nebullvm-0.9.1/nebullvm/installers/installers.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,23 @@
         "pip3",
         "install",
         "torch-tensorrt",
         "--find-links",
         "https://github.com/pytorch/TensorRT/releases/expanded_assets/v1.3.0",
     ]
     subprocess.run(cmd)
+    cuda_version = subprocess.check_output(["nvidia-smi"])
+    cuda_version = int(cuda_version.decode("utf-8").split("\n")[2].split("|")[-2].split(":")[-1].strip().split(".")[0])
+    if cuda_version >= 12:
+        cmd = [
+            "pip3",
+            "install",
+            "tensorrt==8.6.0",
+        ]
+        subprocess.run(cmd)
 
     try:
         import torch_tensorrt  # noqa F401
     except ImportError:
         return False
 
     return True
```

### Comparing `nebullvm-0.9.0/nebullvm/installers/tests/test_install_frameworks.py` & `nebullvm-0.9.1/nebullvm/installers/tests/test_install_frameworks.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/installers/tvm_installers/arm/config.cmake` & `nebullvm-0.9.1/nebullvm/installers/tvm_installers/arm/config.cmake`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/installers/tvm_installers/arm_cuda/config.cmake` & `nebullvm-0.9.1/nebullvm/installers/tvm_installers/arm_cuda/config.cmake`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/installers/tvm_installers/x86/config.cmake` & `nebullvm-0.9.1/nebullvm/installers/tvm_installers/x86/config.cmake`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/installers/tvm_installers/x86_cuda/config.cmake` & `nebullvm-0.9.1/nebullvm/installers/tvm_installers/x86_cuda/config.cmake`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/base.py` & `nebullvm-0.9.1/nebullvm/operations/base.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/conversions/converters.py` & `nebullvm-0.9.1/nebullvm/operations/conversions/converters.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/conversions/huggingface.py` & `nebullvm-0.9.1/nebullvm/operations/conversions/huggingface.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/conversions/pytorch.py` & `nebullvm-0.9.1/nebullvm/operations/conversions/pytorch.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/conversions/tensorflow.py` & `nebullvm-0.9.1/nebullvm/operations/conversions/tensorflow.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/fetch_operations/local.py` & `nebullvm-0.9.1/nebullvm/operations/fetch_operations/local.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/inference_learners/base.py` & `nebullvm-0.9.1/nebullvm/operations/inference_learners/base.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/inference_learners/blade_disc.py` & `nebullvm-0.9.1/nebullvm/operations/inference_learners/blade_disc.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/inference_learners/builders.py` & `nebullvm-0.9.1/nebullvm/operations/inference_learners/builders.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/inference_learners/deepsparse.py` & `nebullvm-0.9.1/nebullvm/operations/inference_learners/deepsparse.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/inference_learners/huggingface.py` & `nebullvm-0.9.1/nebullvm/operations/inference_learners/huggingface.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/inference_learners/neural_compressor.py` & `nebullvm-0.9.1/nebullvm/operations/inference_learners/neural_compressor.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/inference_learners/onnx.py` & `nebullvm-0.9.1/nebullvm/operations/inference_learners/onnx.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/inference_learners/openvino.py` & `nebullvm-0.9.1/nebullvm/operations/inference_learners/openvino.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/inference_learners/pytorch.py` & `nebullvm-0.9.1/nebullvm/operations/inference_learners/pytorch.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/inference_learners/tensor_rt.py` & `nebullvm-0.9.1/nebullvm/operations/inference_learners/tensor_rt.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/inference_learners/tensorflow.py` & `nebullvm-0.9.1/nebullvm/operations/inference_learners/tensorflow.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/inference_learners/tvm.py` & `nebullvm-0.9.1/nebullvm/operations/inference_learners/tvm.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/inference_learners/utils.py` & `nebullvm-0.9.1/nebullvm/operations/inference_learners/utils.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/measures/measures.py` & `nebullvm-0.9.1/nebullvm/operations/measures/measures.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/measures/utils.py` & `nebullvm-0.9.1/nebullvm/operations/measures/utils.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/base.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/base.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/base.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/base.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/deepsparse.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/deepsparse.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/intel_neural_compressor.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/intel_neural_compressor.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/onnxruntime.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/onnxruntime.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/openvino.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/openvino.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/pytorch.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/pytorch.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/quantizations/intel_neural_compressor.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/quantizations/intel_neural_compressor.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/quantizations/onnx.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/quantizations/onnx.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/quantizations/openvino.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/quantizations/openvino.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/quantizations/pytorch.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/quantizations/pytorch.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/quantizations/tensor_rt.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/quantizations/tensor_rt.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/quantizations/tensorflow.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/quantizations/tensorflow.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/quantizations/tvm.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/quantizations/tvm.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/tensor_rt.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/tensor_rt.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/tensorflow.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/tensorflow.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/tvm.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/tvm.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/compilers/utils.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/compilers/utils.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/compressors/base.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/compressors/base.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/compressors/intel.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/compressors/intel.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/compressors/scripts/__init__.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/compressors/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/compressors/scripts/neural_magic_training.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/compressors/scripts/neural_magic_training.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/compressors/sparseml.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/compressors/sparseml.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/optimizers.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/optimizers.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/tests/test_deepsparse.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/tests/test_deepsparse.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/tests/test_intel_neural_compressor.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/tests/test_intel_neural_compressor.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/tests/test_onnxruntime.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/tests/test_onnxruntime.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/tests/test_openvino.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/tests/test_openvino.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/tests/test_tensor_rt.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/tests/test_tensor_rt.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/tests/test_tensorflow.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/tests/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/tests/test_torchscript.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/tests/test_torchscript.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/tests/test_tvm.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/tests/test_tvm.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/operations/optimizations/tests/utils.py` & `nebullvm-0.9.1/nebullvm/operations/optimizations/tests/utils.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/optional_modules/diffusers.py` & `nebullvm-0.9.1/nebullvm/optional_modules/diffusers.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/optional_modules/neural_compressor.py` & `nebullvm-0.9.1/nebullvm/optional_modules/neural_compressor.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/optional_modules/onnxruntime.py` & `nebullvm-0.9.1/nebullvm/optional_modules/onnxruntime.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/optional_modules/openvino.py` & `nebullvm-0.9.1/nebullvm/optional_modules/openvino.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/optional_modules/tensorflow.py` & `nebullvm-0.9.1/nebullvm/optional_modules/tensorflow.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/optional_modules/torch.py` & `nebullvm-0.9.1/nebullvm/optional_modules/torch.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/optional_modules/tvm.py` & `nebullvm-0.9.1/nebullvm/optional_modules/tvm.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/optional_modules/utils.py` & `nebullvm-0.9.1/nebullvm/optional_modules/utils.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/tools/base.py` & `nebullvm-0.9.1/nebullvm/tools/base.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/tools/benchmark.py` & `nebullvm-0.9.1/nebullvm/tools/benchmark.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/tools/data.py` & `nebullvm-0.9.1/nebullvm/tools/data.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/tools/diffusers.py` & `nebullvm-0.9.1/nebullvm/tools/diffusers.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/tools/feedback_collector.py` & `nebullvm-0.9.1/nebullvm/tools/feedback_collector.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/tools/huggingface.py` & `nebullvm-0.9.1/nebullvm/tools/huggingface.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/tools/logger.py` & `nebullvm-0.9.1/nebullvm/tools/logger.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/tools/onnx.py` & `nebullvm-0.9.1/nebullvm/tools/onnx.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/tools/pytorch.py` & `nebullvm-0.9.1/nebullvm/tools/pytorch.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/tools/tests/test_data.py` & `nebullvm-0.9.1/nebullvm/tools/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/tools/tf.py` & `nebullvm-0.9.1/nebullvm/tools/tf.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/tools/transformations.py` & `nebullvm-0.9.1/nebullvm/tools/transformations.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/tools/utils.py` & `nebullvm-0.9.1/nebullvm/tools/utils.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm/tools/venv.py` & `nebullvm-0.9.1/nebullvm/tools/venv.py`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/nebullvm.egg-info/PKG-INFO` & `nebullvm-0.9.1/nebullvm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nebullvm
-Version: 0.9.0
+Version: 0.9.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
 <br><br><br>
 <a https://docs.nebuly.com/welcome/quick-start"><img src="https://user-images.githubusercontent.com/83510798/208247207-861541f0-b968-484c-8a0c-0fb110399c16.png" width="400px"></a>
 <br><br><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nebullvm Version: 0.9.0 Description-Content-Type:
+Metadata-Version: 2.1 Name: nebullvm Version: 0.9.1 Description-Content-Type:
 text/markdown License-File: LICENSE
 
 
 
               docs.nebuly.com/welcome/quick-start">[https://user-
    images.githubusercontent.com/83510798/208247207-861541f0-b968-484c-8a0c-
                                0fb110399c16.png]
```

### Comparing `nebullvm-0.9.0/nebullvm.egg-info/SOURCES.txt` & `nebullvm-0.9.1/nebullvm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nebullvm-0.9.0/setup.py` & `nebullvm-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 ]
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf8")
 
 setup(
     name="nebullvm",
-    version="0.9.0",
+    version="0.9.1",
     packages=find_packages(),
     install_requires=REQUIREMENTS,
     long_description=long_description,
     include_package_data=True,
     long_description_content_type="text/markdown",
 )
```

