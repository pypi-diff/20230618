# Comparing `tmp/nobuco-0.4.9.tar.gz` & `tmp/nobuco-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobuco-0.4.9.tar", last modified: Fri Jun  9 15:15:49 2023, max compression
+gzip compressed data, was "nobuco-0.5.0.tar", last modified: Sun Jun 18 11:29:57 2023, max compression
```

## Comparing `nobuco-0.4.9.tar` & `nobuco-0.5.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-09 15:15:49.353446 nobuco-0.4.9/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.4.9/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)    22071 2023-06-09 15:15:49.353446 nobuco-0.4.9/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    20237 2023-05-17 10:50:20.000000 nobuco-0.4.9/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-09 15:15:49.349446 nobuco-0.4.9/nobuco/
--rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/commons.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    13696 2023-06-09 15:12:04.000000 nobuco-0.4.9/nobuco/convert.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-09 15:15:49.349446 nobuco-0.4.9/nobuco/converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/converters/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-06-02 13:56:50.000000 nobuco-0.4.9/nobuco/converters/channel_ordering.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/converters/node_converter.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2256 2023-06-02 12:03:42.000000 nobuco-0.4.9/nobuco/converters/tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/converters/type_cast.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     4064 2023-06-06 20:42:12.000000 nobuco-0.4.9/nobuco/converters/validation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-09 15:15:49.349446 nobuco-0.4.9/nobuco/entity/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/entity/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/entity/keras.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-05-17 10:49:40.000000 nobuco-0.4.9/nobuco/entity/pytorch.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/funcs.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-09 15:15:49.349446 nobuco-0.4.9/nobuco/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/layers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/layers/channel_order.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/layers/container.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/layers/stub.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1069 2023-06-06 15:58:09.000000 nobuco-0.4.9/nobuco/layers/weight.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-09 15:15:49.349446 nobuco-0.4.9/nobuco/locate/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/locate/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/locate/link.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/locate/locate.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-09 15:15:49.353446 nobuco-0.4.9/nobuco/node_converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/node_converters/__init__.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     6206 2023-05-04 09:06:58.000000 nobuco-0.4.9/nobuco/node_converters/activation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      901 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/node_converters/boolean.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1211 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/node_converters/boolean_mask.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3504 2023-06-01 14:17:46.000000 nobuco-0.4.9/nobuco/node_converters/comparison.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-05-03 16:03:42.000000 nobuco-0.4.9/nobuco/node_converters/convolution.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/node_converters/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1533 2023-06-06 20:30:38.000000 nobuco-0.4.9/nobuco/node_converters/interpolation.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     5086 2023-05-01 12:01:37.000000 nobuco-0.4.9/nobuco/node_converters/linear.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13838 2023-06-06 20:13:59.000000 nobuco-0.4.9/nobuco/node_converters/math.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-05-16 10:06:23.000000 nobuco-0.4.9/nobuco/node_converters/misc.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1638 2023-05-17 15:16:26.000000 nobuco-0.4.9/nobuco/node_converters/normalization.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1261 2023-06-07 02:32:02.000000 nobuco-0.4.9/nobuco/node_converters/padding.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2879 2023-05-17 15:16:26.000000 nobuco-0.4.9/nobuco/node_converters/pooling.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/node_converters/recurrent.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7966 2023-06-09 15:13:56.000000 nobuco-0.4.9/nobuco/node_converters/slice.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3895 2023-05-17 10:46:04.000000 nobuco-0.4.9/nobuco/node_converters/tensor_cast.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5969 2023-06-07 02:44:23.000000 nobuco-0.4.9/nobuco/node_converters/tensor_creation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11126 2023-06-06 20:13:14.000000 nobuco-0.4.9/nobuco/node_converters/tensor_manipulation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      369 2023-06-06 21:33:32.000000 nobuco-0.4.9/nobuco/node_converters/tensor_shape.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-09 15:15:49.353446 nobuco-0.4.9/nobuco/trace/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/trace/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1378 2023-06-06 19:21:15.000000 nobuco-0.4.9/nobuco/trace/tensor_storage.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10039 2023-06-09 15:11:00.000000 nobuco-0.4.9/nobuco/trace/trace.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/util.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-09 15:15:49.353446 nobuco-0.4.9/nobuco/vis/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/vis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/vis/console_stylizer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/vis/html_stylizer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-09 15:15:49.349446 nobuco-0.4.9/nobuco.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)    22071 2023-06-09 15:15:49.000000 nobuco-0.4.9/nobuco.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     1628 2023-06-09 15:15:49.000000 nobuco-0.4.9/nobuco.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-09 15:15:49.000000 nobuco-0.4.9/nobuco.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-06-09 15:15:49.000000 nobuco-0.4.9/nobuco.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-06-09 15:15:49.000000 nobuco-0.4.9/nobuco.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-06-09 15:14:07.000000 nobuco-0.4.9/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-09 15:15:49.353446 nobuco-0.4.9/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-18 11:29:57.491739 nobuco-0.5.0/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.5.0/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22522 2023-06-18 11:29:57.491739 nobuco-0.5.0/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20688 2023-06-18 11:15:01.000000 nobuco-0.5.0/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-18 11:29:57.487739 nobuco-0.5.0/nobuco/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/commons.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    13696 2023-06-09 15:12:04.000000 nobuco-0.5.0/nobuco/convert.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-18 11:29:57.487739 nobuco-0.5.0/nobuco/converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/converters/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-06-02 13:56:50.000000 nobuco-0.5.0/nobuco/converters/channel_ordering.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/converters/node_converter.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2256 2023-06-02 12:03:42.000000 nobuco-0.5.0/nobuco/converters/tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/converters/type_cast.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     4064 2023-06-06 20:42:12.000000 nobuco-0.5.0/nobuco/converters/validation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-18 11:29:57.487739 nobuco-0.5.0/nobuco/entity/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/entity/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/entity/keras.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-05-17 10:49:40.000000 nobuco-0.5.0/nobuco/entity/pytorch.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/funcs.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-18 11:29:57.487739 nobuco-0.5.0/nobuco/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/layers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4419 2023-06-17 09:52:53.000000 nobuco-0.5.0/nobuco/layers/channel_order.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/layers/container.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/layers/stub.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1069 2023-06-06 15:58:09.000000 nobuco-0.5.0/nobuco/layers/weight.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-18 11:29:57.487739 nobuco-0.5.0/nobuco/locate/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/locate/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/locate/link.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/locate/locate.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-18 11:29:57.491739 nobuco-0.5.0/nobuco/node_converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/node_converters/__init__.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     6967 2023-06-15 13:23:44.000000 nobuco-0.5.0/nobuco/node_converters/activation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      901 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/node_converters/boolean.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1165 2023-06-16 16:26:28.000000 nobuco-0.5.0/nobuco/node_converters/boolean_mask.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3504 2023-06-01 14:17:46.000000 nobuco-0.5.0/nobuco/node_converters/comparison.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-05-03 16:03:42.000000 nobuco-0.5.0/nobuco/node_converters/convolution.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/node_converters/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1533 2023-06-06 20:30:38.000000 nobuco-0.5.0/nobuco/node_converters/interpolation.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     5086 2023-05-01 12:01:37.000000 nobuco-0.5.0/nobuco/node_converters/linear.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13838 2023-06-06 20:13:59.000000 nobuco-0.5.0/nobuco/node_converters/math.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-05-16 10:06:23.000000 nobuco-0.5.0/nobuco/node_converters/misc.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1638 2023-05-17 15:16:26.000000 nobuco-0.5.0/nobuco/node_converters/normalization.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1261 2023-06-07 02:32:02.000000 nobuco-0.5.0/nobuco/node_converters/padding.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2879 2023-05-17 15:16:26.000000 nobuco-0.5.0/nobuco/node_converters/pooling.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/node_converters/recurrent.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9372 2023-06-17 10:31:40.000000 nobuco-0.5.0/nobuco/node_converters/slice.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3895 2023-05-17 10:46:04.000000 nobuco-0.5.0/nobuco/node_converters/tensor_cast.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5969 2023-06-07 02:44:23.000000 nobuco-0.5.0/nobuco/node_converters/tensor_creation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11126 2023-06-06 20:13:14.000000 nobuco-0.5.0/nobuco/node_converters/tensor_manipulation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      369 2023-06-06 21:33:32.000000 nobuco-0.5.0/nobuco/node_converters/tensor_shape.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-18 11:29:57.491739 nobuco-0.5.0/nobuco/trace/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/trace/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1378 2023-06-06 19:21:15.000000 nobuco-0.5.0/nobuco/trace/tensor_storage.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10039 2023-06-09 15:11:00.000000 nobuco-0.5.0/nobuco/trace/trace.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-18 11:29:57.491739 nobuco-0.5.0/nobuco/vis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/vis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/vis/console_stylizer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.5.0/nobuco/vis/html_stylizer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-18 11:29:57.487739 nobuco-0.5.0/nobuco.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22522 2023-06-18 11:29:57.000000 nobuco-0.5.0/nobuco.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1628 2023-06-18 11:29:57.000000 nobuco-0.5.0/nobuco.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-18 11:29:57.000000 nobuco-0.5.0/nobuco.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-06-18 11:29:57.000000 nobuco-0.5.0/nobuco.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-06-18 11:29:57.000000 nobuco-0.5.0/nobuco.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-06-18 11:27:44.000000 nobuco-0.5.0/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-18 11:29:57.491739 nobuco-0.5.0/setup.cfg
```

### Comparing `nobuco-0.4.9/LICENSE` & `nobuco-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/PKG-INFO` & `nobuco-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.4.9
+Version: 0.5.0
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,14 +43,15 @@
 
 - Supports a wide range of architectures
   - [x] Control flow ops (If, While)
   - [x] Recurrent layers (LSTM, GRU)
   - [x] Arbitrary torch functions
 - Simple
 - Flexible
+- Efficient
 - Sanity-preserving, with clear mistake messaging
 
 <!-- toc -->
 
 ## Installation <img src="https://img.shields.io/pypi/v/nobuco?color=blue&style=flat-square">
 <img src="https://img.shields.io/badge/PyTorch-2.0.0-EE4C2C.svg?style=flat&logo=pytorch"> <img src="https://img.shields.io/badge/TensorFlow-2.10-FF6F00.svg?style=flat&logo=tensorflow">
 
@@ -151,17 +152,17 @@
 Best we can do without the converter constantly lacking essential functionality, being riddled with bugs, doing weird stuff and breaking apart with every other PT/TF release 
 is to keep the tool simple and customizable, make it clear where a problem comes from and let the _user_ sort things out.
 Usually it's easy for a human to translate an isolated operation from one framework to another.
 Reproducing the graph structure is a different matter entirely. For that, Nobuco has you covered!
 
 https://user-images.githubusercontent.com/2457934/233740603-cc11acc5-cd6b-48c8-b089-ff3ead772dd0.mp4
 
-<p align="center">
+<p align="center"><em>
 To ease debugging, Nobuco lets you jump right where the node was [I]nvoked, [D]efined and [C]onverted
-</p>
+</em></p>
 
 ## Channel order wizardry
 
 Some operations assume its input tensors have a channel dimension. 
 And as you probably know, pytorch and tensorflow do not agree on the layout of such tensors.
 Pytorch adopts channel-first layout (_B**C**H_, _B**C**HW_, etc.) 
 while tensorflow works efficiently with channel-last tensors (_BH**C**_, _BHW**C**_, ...).
@@ -207,15 +208,15 @@
         return x1, x2
 
 pytorch_module = MyModule().eval()
 
 inputs = [
     torch.normal(0, 1, size=(1, 12, 32)),
 ]
-
+You can
 keras_model = nobuco.pytorch_to_keras(
     pytorch_module, inputs,
     inputs_channel_order=ChannelOrder.PYTORCH,
 )
 ```
 
 The laziness shoots us in the foot here, and we get not one transpose but two:
@@ -465,78 +466,90 @@
         shape = tf.unstack(tf.shape(x))
         if get_channel_order(x) == ChannelOrder.TENSORFLOW:
             shape = permute_keras2pytorch(shape)
         return tuple(shape)
     return func
 ```
 
+It's also possible to automatically substitute every `.shape` call with `nobuco.shape` during the tracing phase by setting `trace_shape` flag:
+
+```python
+keras_model = nobuco.pytorch_to_keras(
+  # ...
+  trace_shape=True
+)
+```
+
 ## So we put a converter inside your converter
 
-One of the operations currently not supported is mask assign.
-There's no particular reason why, I just haven't done it yet (and your contribution is highly welcome!) 
-For now, let's use it as an excuse to explain the concept of nested converters.
-Like I said, for this module, conversion will fail:
+As we've learned, Nobuco gets confused when in-place operation is applied to a slice.
+There's a way to fix that, but let's not do it now.
+Instead, we'll use it as an excuse to explain the concept of nested converters.
+So, for this module, conversion will give us incorrect result:
 
 ```python
 class MyModule(nn.Module):
     def __init__(self):
         super().__init__()
         self.conv = nn.Conv2d(3, 3, kernel_size=(3, 3), padding=(1, 1))
 
     def forward(self, x):
         x = self.conv(x)
-        x[x > 0] += 1
+        # Gives incorrect result after conversion
+        torch.relu_(x[:, 1:2, 16:25, 8::2])
+        # That's the recommended approach, but we're not going for it now
+        # x[:, 1:2, 16:25, 8::2] = torch.relu_(x[:, 1:2, 16:25, 8::2])
         return x
 ```
 
 <img src="docs/converter_inside_converter1.svg" width="100%">
 
 In the previous section, we've seen it's possible to invoke a Nobuco converter inside another Nobuco converter.
 Can we embed some third-party converter? You bet! Why? Because it might just do what we need.
 Let's consider the standard route: pytorch -> onnx -> tensorflow, with the latter step done with [onnx-tf](https://github.com/onnx/onnx-tensorflow).
 This library likes transposing stuff so much, converting the whole graph with it may introduce intolerable inference overhead. Nonetheless, it does the job.
 A sensible tradeoff would be to wrap the problematic operation into its own `nn.Module` and give it a special treat, while handling everything else with Nobuco.
 
 ```python
-class AddByMask(nn.Module):
-    def forward(self, x, mask):
-        x[mask] += 1
+class SliceReLU(nn.Module):
+    def forward(self, x):
+        torch.relu_(x[:, 1:2, 16:25, 8::2])
         return x
 
 
 class MyModule(nn.Module):
     def __init__(self):
         super().__init__()
         self.conv = nn.Conv2d(3, 3, kernel_size=(3, 3), padding=(1, 1))
 
     def forward(self, x):
         x = self.conv(x)
-        mask = x > 0
-        AddByMask()(x, mask)
+        SliceReLU()(x)
         return x
 ```
 
 ```python
 import onnx
 from onnx_tf.backend import prepare
 
 
-@nobuco.converter(AddByMask, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER, reusable=False)
-def converter_AddByMask(self, x, mask):
-    model_path = 'add_by_mask'
+@nobuco.converter(SliceReLU, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER, reusable=False)
+def converter_SliceReLU(self, x):
+    model_path = 'slice_relu'
     onnx_path = model_path + '.onnx'
 
-    # NB: onnx.export is implemented via tracing i.e. it may modify the inputs!
-    torch.onnx.export(self, (x, mask), onnx_path, opset_version=12, input_names=['input', 'mask'], dynamic_axes={'input': [0, 1, 2, 3]})
-
+    # NB: onnx.export in implemented via tracing i.e. it may modify the inputs!
+    torch.onnx.export(self, (x,), onnx_path, opset_version=12, input_names=['input'],
+                      dynamic_axes={'input': [0, 1, 2, 3]}
+                      )
     onnx_model = onnx.load(onnx_path)
     tf_rep = prepare(onnx_model)
     tf_rep.export_graph(model_path)
     model = tf.keras.models.load_model(model_path)
-    return keras.layers.Lambda(lambda x, mask: model(input=x, mask=mask))
+    return keras.layers.Lambda(lambda x: model(input=x))
 ```
 
 <img src="docs/converter_inside_converter2.svg" width="100%">
 
 ## More nice things
 
 ### Nobuco knowledge base
```

### Comparing `nobuco-0.4.9/README.md` & `nobuco-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 - Supports a wide range of architectures
   - [x] Control flow ops (If, While)
   - [x] Recurrent layers (LSTM, GRU)
   - [x] Arbitrary torch functions
 - Simple
 - Flexible
+- Efficient
 - Sanity-preserving, with clear mistake messaging
 
 <!-- toc -->
 
 ## Installation <img src="https://img.shields.io/pypi/v/nobuco?color=blue&style=flat-square">
 <img src="https://img.shields.io/badge/PyTorch-2.0.0-EE4C2C.svg?style=flat&logo=pytorch"> <img src="https://img.shields.io/badge/TensorFlow-2.10-FF6F00.svg?style=flat&logo=tensorflow">
 
@@ -115,17 +116,17 @@
 Best we can do without the converter constantly lacking essential functionality, being riddled with bugs, doing weird stuff and breaking apart with every other PT/TF release 
 is to keep the tool simple and customizable, make it clear where a problem comes from and let the _user_ sort things out.
 Usually it's easy for a human to translate an isolated operation from one framework to another.
 Reproducing the graph structure is a different matter entirely. For that, Nobuco has you covered!
 
 https://user-images.githubusercontent.com/2457934/233740603-cc11acc5-cd6b-48c8-b089-ff3ead772dd0.mp4
 
-<p align="center">
+<p align="center"><em>
 To ease debugging, Nobuco lets you jump right where the node was [I]nvoked, [D]efined and [C]onverted
-</p>
+</em></p>
 
 ## Channel order wizardry
 
 Some operations assume its input tensors have a channel dimension. 
 And as you probably know, pytorch and tensorflow do not agree on the layout of such tensors.
 Pytorch adopts channel-first layout (_B**C**H_, _B**C**HW_, etc.) 
 while tensorflow works efficiently with channel-last tensors (_BH**C**_, _BHW**C**_, ...).
@@ -171,15 +172,15 @@
         return x1, x2
 
 pytorch_module = MyModule().eval()
 
 inputs = [
     torch.normal(0, 1, size=(1, 12, 32)),
 ]
-
+You can
 keras_model = nobuco.pytorch_to_keras(
     pytorch_module, inputs,
     inputs_channel_order=ChannelOrder.PYTORCH,
 )
 ```
 
 The laziness shoots us in the foot here, and we get not one transpose but two:
@@ -429,78 +430,90 @@
         shape = tf.unstack(tf.shape(x))
         if get_channel_order(x) == ChannelOrder.TENSORFLOW:
             shape = permute_keras2pytorch(shape)
         return tuple(shape)
     return func
 ```
 
+It's also possible to automatically substitute every `.shape` call with `nobuco.shape` during the tracing phase by setting `trace_shape` flag:
+
+```python
+keras_model = nobuco.pytorch_to_keras(
+  # ...
+  trace_shape=True
+)
+```
+
 ## So we put a converter inside your converter
 
-One of the operations currently not supported is mask assign.
-There's no particular reason why, I just haven't done it yet (and your contribution is highly welcome!) 
-For now, let's use it as an excuse to explain the concept of nested converters.
-Like I said, for this module, conversion will fail:
+As we've learned, Nobuco gets confused when in-place operation is applied to a slice.
+There's a way to fix that, but let's not do it now.
+Instead, we'll use it as an excuse to explain the concept of nested converters.
+So, for this module, conversion will give us incorrect result:
 
 ```python
 class MyModule(nn.Module):
     def __init__(self):
         super().__init__()
         self.conv = nn.Conv2d(3, 3, kernel_size=(3, 3), padding=(1, 1))
 
     def forward(self, x):
         x = self.conv(x)
-        x[x > 0] += 1
+        # Gives incorrect result after conversion
+        torch.relu_(x[:, 1:2, 16:25, 8::2])
+        # That's the recommended approach, but we're not going for it now
+        # x[:, 1:2, 16:25, 8::2] = torch.relu_(x[:, 1:2, 16:25, 8::2])
         return x
 ```
 
 <img src="docs/converter_inside_converter1.svg" width="100%">
 
 In the previous section, we've seen it's possible to invoke a Nobuco converter inside another Nobuco converter.
 Can we embed some third-party converter? You bet! Why? Because it might just do what we need.
 Let's consider the standard route: pytorch -> onnx -> tensorflow, with the latter step done with [onnx-tf](https://github.com/onnx/onnx-tensorflow).
 This library likes transposing stuff so much, converting the whole graph with it may introduce intolerable inference overhead. Nonetheless, it does the job.
 A sensible tradeoff would be to wrap the problematic operation into its own `nn.Module` and give it a special treat, while handling everything else with Nobuco.
 
 ```python
-class AddByMask(nn.Module):
-    def forward(self, x, mask):
-        x[mask] += 1
+class SliceReLU(nn.Module):
+    def forward(self, x):
+        torch.relu_(x[:, 1:2, 16:25, 8::2])
         return x
 
 
 class MyModule(nn.Module):
     def __init__(self):
         super().__init__()
         self.conv = nn.Conv2d(3, 3, kernel_size=(3, 3), padding=(1, 1))
 
     def forward(self, x):
         x = self.conv(x)
-        mask = x > 0
-        AddByMask()(x, mask)
+        SliceReLU()(x)
         return x
 ```
 
 ```python
 import onnx
 from onnx_tf.backend import prepare
 
 
-@nobuco.converter(AddByMask, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER, reusable=False)
-def converter_AddByMask(self, x, mask):
-    model_path = 'add_by_mask'
+@nobuco.converter(SliceReLU, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER, reusable=False)
+def converter_SliceReLU(self, x):
+    model_path = 'slice_relu'
     onnx_path = model_path + '.onnx'
 
-    # NB: onnx.export is implemented via tracing i.e. it may modify the inputs!
-    torch.onnx.export(self, (x, mask), onnx_path, opset_version=12, input_names=['input', 'mask'], dynamic_axes={'input': [0, 1, 2, 3]})
-
+    # NB: onnx.export in implemented via tracing i.e. it may modify the inputs!
+    torch.onnx.export(self, (x,), onnx_path, opset_version=12, input_names=['input'],
+                      dynamic_axes={'input': [0, 1, 2, 3]}
+                      )
     onnx_model = onnx.load(onnx_path)
     tf_rep = prepare(onnx_model)
     tf_rep.export_graph(model_path)
     model = tf.keras.models.load_model(model_path)
-    return keras.layers.Lambda(lambda x, mask: model(input=x, mask=mask))
+    return keras.layers.Lambda(lambda x: model(input=x))
 ```
 
 <img src="docs/converter_inside_converter2.svg" width="100%">
 
 ## More nice things
 
 ### Nobuco knowledge base
```

### Comparing `nobuco-0.4.9/nobuco/__init__.py` & `nobuco-0.5.0/nobuco/__init__.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/commons.py` & `nobuco-0.5.0/nobuco/commons.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/convert.py` & `nobuco-0.5.0/nobuco/convert.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/converters/channel_ordering.py` & `nobuco-0.5.0/nobuco/converters/channel_ordering.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/converters/node_converter.py` & `nobuco-0.5.0/nobuco/converters/node_converter.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/converters/tensor.py` & `nobuco-0.5.0/nobuco/converters/tensor.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/converters/type_cast.py` & `nobuco-0.5.0/nobuco/converters/type_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/converters/validation.py` & `nobuco-0.5.0/nobuco/converters/validation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/entity/keras.py` & `nobuco-0.5.0/nobuco/entity/keras.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/entity/pytorch.py` & `nobuco-0.5.0/nobuco/entity/pytorch.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/funcs.py` & `nobuco-0.5.0/nobuco/funcs.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/layers/channel_order.py` & `nobuco-0.5.0/nobuco/layers/channel_order.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,16 @@
 from nobuco.commons import ChannelOrderingStrategy, ChannelOrder, TF_TENSOR_CLASSES
 from nobuco.converters.channel_ordering import set_channel_order, get_channel_order
 from nobuco.converters.tensor import _permute, perm_keras2pytorch, perm_pytorch2keras
 from nobuco.converters.type_cast import tf_cast_recursively
 from nobuco.util import collect_recursively, replace_recursively_func
 
 
-class SetOrderLayer:
-    def __init__(self, func, channel_order):
-        self.func = func
-        self.channel_order = channel_order
-
-    def __call__(self, *args, **kwargs):
-        args = tf_annotate_recursively(args, channel_order=self.channel_order)
-        kwargs = tf_annotate_recursively(kwargs, channel_order=self.channel_order)
-        outputs = self.func(*args, **kwargs)
-        outputs = tf_annotate_recursively(outputs, channel_order=self.channel_order)
-        return outputs
-
-    def __str__(self):
-        return f"{self.__class__.__name__}(func={self.func})"
-
-
 class ChangeOrderingLayer:
-    def __init__(self, func, channel_ordering_strategy, autocast):
+    def __init__(self, func, channel_ordering_strategy, autocast=False):
         self.func = func
         self.channel_ordering_strategy = channel_ordering_strategy
         self.autocast = autocast
 
     def __call__(self, *args, **kwargs):
         tf_assert_has_attr_recursively((args, kwargs), 'channel_order')
```

### Comparing `nobuco-0.4.9/nobuco/layers/container.py` & `nobuco-0.5.0/nobuco/layers/container.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/layers/weight.py` & `nobuco-0.5.0/nobuco/layers/weight.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/locate/link.py` & `nobuco-0.5.0/nobuco/locate/link.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/locate/locate.py` & `nobuco-0.5.0/nobuco/locate/locate.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/node_converters/activation.py` & `nobuco-0.5.0/nobuco/node_converters/activation.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,7 +151,26 @@
 
 
 @converter(torch.clip, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def converter_clip(input: Tensor, min: Optional[Tensor]=None, max: Optional[Tensor]=None, *, out: Optional[Tensor]=None):
     def func(input, min=None, max=None, *, out=None):
         return tf.clip_by_value(input, min, max)
     return func
+
+
+@converter(F.silu, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+def converter_silu(input: Tensor, inplace=False):
+    def func(input: Tensor, inplace=False):
+        return tf.nn.silu(input, beta=1.0)
+    return func
+
+      
+@converter(F.gelu, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+def converter_gelu(input: Tensor, approximate='none'):
+    def func(input: Tensor, approximate='none'):
+        if approximate.lower() == 'none':
+            # Gaussian Error Linear Units (GELUs)
+            # https://arxiv.org/abs/1606.08415
+            return input * 0.5 * (1 + tf.math.erf(input / tf.math.sqrt(2.)))
+        else:
+            return tf.nn.gelu(input, approximate=approximate)
+    return func
```

### Comparing `nobuco-0.4.9/nobuco/node_converters/boolean.py` & `nobuco-0.5.0/nobuco/node_converters/boolean.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/node_converters/boolean_mask.py` & `nobuco-0.5.0/nobuco/node_converters/boolean_mask.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from nobuco.commons import ChannelOrder, ChannelOrderingStrategy
 from nobuco.converters.node_converter import converter
 
 
 @converter(torch.masked_select, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
 def converter_masked_select(input: Tensor, mask: Tensor, *, out: Optional[Tensor]=None):
     def func(input, mask, *, out=None):
-        # return tf.boolean_mask(input, mask)
         return input[mask]
     return func
 
 
 @converter(torch.masked_fill, torch.Tensor.masked_fill, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
 def converter_masked_fill(input: Tensor, mask: Tensor, value: Number):
     def func(input, mask, value):
```

### Comparing `nobuco-0.4.9/nobuco/node_converters/comparison.py` & `nobuco-0.5.0/nobuco/node_converters/comparison.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/node_converters/convolution.py` & `nobuco-0.5.0/nobuco/node_converters/convolution.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/node_converters/dropout.py` & `nobuco-0.5.0/nobuco/node_converters/dropout.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/node_converters/interpolation.py` & `nobuco-0.5.0/nobuco/node_converters/interpolation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/node_converters/linear.py` & `nobuco-0.5.0/nobuco/node_converters/linear.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/node_converters/math.py` & `nobuco-0.5.0/nobuco/node_converters/math.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/node_converters/misc.py` & `nobuco-0.5.0/nobuco/node_converters/misc.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/node_converters/normalization.py` & `nobuco-0.5.0/nobuco/node_converters/normalization.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/node_converters/padding.py` & `nobuco-0.5.0/nobuco/node_converters/padding.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/node_converters/pooling.py` & `nobuco-0.5.0/nobuco/node_converters/pooling.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/node_converters/recurrent.py` & `nobuco-0.5.0/nobuco/node_converters/recurrent.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/node_converters/slice.py` & `nobuco-0.5.0/nobuco/node_converters/slice.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import tensorflow as tf
 import torch
 
 import numpy as np
+from nobuco.layers.channel_order import ChangeOrderingLayer
 
 from nobuco.commons import ChannelOrder, ChannelOrderingStrategy, TF_TENSOR_CLASSES
 from nobuco.converters.channel_ordering import set_channel_order, get_channel_order
 from nobuco.converters.node_converter import converter
 from nobuco.converters.tensor import perm_keras2pytorch, _permute, _flatten, permute_pytorch2keras, _ensure_iterable, _ensure_tuple
 from nobuco.layers.weight import WeightLayer
 from nobuco.node_converters.boolean_mask import converter_masked_select
@@ -30,15 +31,15 @@
     shape = tensors[0].shape
     for tens in tensors:
         shape = tf.broadcast_dynamic_shape(shape, tens.shape)
     tensors = [tf.broadcast_to(t, shape) for t in tensors]
     return tensors
 
 
-def slice_assign(sliced_tensor, assigned_tensor, slice_args, is_scatter=False):
+def slice_assign(sliced_tensor, slice_args, assigned_tensor, is_scatter=False):
     slice_args = _ensure_iterable(slice_args)
     """Assign a tensor to the slice of another tensor.
     No broadcast is performed.
     Args:
         - sliced_tensor (tf.Tensor): the tensor whose slice you want changed.
         - assigned_tensor (tf.Tensor): the tensor which you want assigned.
         - *slice_args (str or slice): the slices arguments. Can be ':', '...'
@@ -132,14 +133,53 @@
         indices=update_indices,
         updates=assigned_tensor_reshaped,
     )
     sliced_tensor_updated = tf.transpose(sliced_tensor_reshaped, perm=inverse_scatter_nd_perm)
     return sliced_tensor_updated
 
 
+def slice_assign_boolean_mask_scatter(sliced_tensor, slice_args, assigned_tensor):
+    update_indices = tf.where(slice_args)
+    sliced_tensor = tf.tensor_scatter_nd_update(
+        tensor=sliced_tensor,
+        indices=update_indices,
+        updates=assigned_tensor,
+    )
+    return sliced_tensor
+
+
+def slice_assign_boolean_mask_select(sliced_tensor, slice_args, assigned_tensor):
+    if isinstance(assigned_tensor, TF_TENSOR_CLASSES):
+        assigned_tensor = tf.cast(assigned_tensor, dtype=sliced_tensor.dtype)
+    else:
+        assigned_tensor = tf.convert_to_tensor(assigned_tensor, dtype=sliced_tensor.dtype)
+    return tf.where(slice_args, assigned_tensor, sliced_tensor)
+
+
+@converter(torch.Tensor.__setitem__, channel_ordering_strategy=ChannelOrderingStrategy.MANUAL)
+def converter_setitem(sliced_tensor, slice_args, assigned_tensor):
+    if isinstance(slice_args, torch.Tensor) and slice_args.dtype == torch.bool:
+        if isinstance(assigned_tensor, torch.Tensor) and assigned_tensor.numel() != 1:
+            func = slice_assign_boolean_mask_scatter
+            func = ChangeOrderingLayer(func, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
+        else:
+            func = slice_assign_boolean_mask_select
+            func = ChangeOrderingLayer(func, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+    else:
+        n_dims = sliced_tensor.dim()
+
+        def func(sliced_tensor, slice_args, assigned_tensor):
+            if get_channel_order(sliced_tensor) == ChannelOrder.TENSORFLOW:
+                slice_args = slices_make_full(slice_args, n_dims)
+                slice_args = permute_pytorch2keras(slice_args)
+            return slice_assign(sliced_tensor, slice_args, assigned_tensor)
+        func = ChangeOrderingLayer(func, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+    return func
+
+
 @converter(channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
 def getitem_indexed(self, *slices):
     def func(self, *slices):
         slices = _ensure_iterable(slices)
         slices = broadcast(slices)
         slices = tf.stack(slices, axis=-1)
         return tf.gather_nd(self, slices)
@@ -150,15 +190,15 @@
 def converter_getitem(self, *slices):
     n_dims = self.dim()
 
     slices = _flatten(slices)
 
     if isinstance(slices[0], torch.Tensor):
         if slices[0].dtype == torch.bool:
-            return converter_masked_select(self, slices[0])
+            return converter_masked_select.convert(self, slices[0])
         elif slices[0].dtype == torch.int64:
             return getitem_indexed.convert(self, slices)
 
     def is_light(slices):
         return all(isinstance(slc, slice) for slc in slices)
 
     if is_light(slices):
@@ -185,26 +225,14 @@
                 x = _permute(perm)(x)
             x = x.__getitem__(slices)
             x = set_channel_order(x, ChannelOrder.PYTORCH)
             return x
     return func
 
 
-@converter(torch.Tensor.__setitem__, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
-def converter_setitem(sliced_tensor, slice_args, assigned_tensor):
-    n_dims = sliced_tensor.dim()
-
-    def func(sliced_tensor, slice_args, assigned_tensor):
-        if get_channel_order(sliced_tensor) == ChannelOrder.TENSORFLOW:
-            slice_args = slices_make_full(slice_args, n_dims)
-            slice_args = permute_pytorch2keras(slice_args)
-        return slice_assign(sliced_tensor, assigned_tensor, slice_args)
-    return func
-
-
 # @converter(torch.Tensor.scatter, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 # def converter_scatter(self, dim, index, src):
 #     assert dim == 0
 #     def func(self, dim, index, src):
 #         slice_args = (tf.reshape(index, -1),)
 #         return slice_assign(self, src, slice_args, is_scatter=True)
 #     return func
```

### Comparing `nobuco-0.4.9/nobuco/node_converters/tensor_cast.py` & `nobuco-0.5.0/nobuco/node_converters/tensor_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/node_converters/tensor_creation.py` & `nobuco-0.5.0/nobuco/node_converters/tensor_creation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/node_converters/tensor_manipulation.py` & `nobuco-0.5.0/nobuco/node_converters/tensor_manipulation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/trace/tensor_storage.py` & `nobuco-0.5.0/nobuco/trace/tensor_storage.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/trace/trace.py` & `nobuco-0.5.0/nobuco/trace/trace.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/util.py` & `nobuco-0.5.0/nobuco/util.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/vis/console_stylizer.py` & `nobuco-0.5.0/nobuco/vis/console_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco/vis/html_stylizer.py` & `nobuco-0.5.0/nobuco/vis/html_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/nobuco.egg-info/PKG-INFO` & `nobuco-0.5.0/nobuco.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.4.9
+Version: 0.5.0
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,14 +43,15 @@
 
 - Supports a wide range of architectures
   - [x] Control flow ops (If, While)
   - [x] Recurrent layers (LSTM, GRU)
   - [x] Arbitrary torch functions
 - Simple
 - Flexible
+- Efficient
 - Sanity-preserving, with clear mistake messaging
 
 <!-- toc -->
 
 ## Installation <img src="https://img.shields.io/pypi/v/nobuco?color=blue&style=flat-square">
 <img src="https://img.shields.io/badge/PyTorch-2.0.0-EE4C2C.svg?style=flat&logo=pytorch"> <img src="https://img.shields.io/badge/TensorFlow-2.10-FF6F00.svg?style=flat&logo=tensorflow">
 
@@ -151,17 +152,17 @@
 Best we can do without the converter constantly lacking essential functionality, being riddled with bugs, doing weird stuff and breaking apart with every other PT/TF release 
 is to keep the tool simple and customizable, make it clear where a problem comes from and let the _user_ sort things out.
 Usually it's easy for a human to translate an isolated operation from one framework to another.
 Reproducing the graph structure is a different matter entirely. For that, Nobuco has you covered!
 
 https://user-images.githubusercontent.com/2457934/233740603-cc11acc5-cd6b-48c8-b089-ff3ead772dd0.mp4
 
-<p align="center">
+<p align="center"><em>
 To ease debugging, Nobuco lets you jump right where the node was [I]nvoked, [D]efined and [C]onverted
-</p>
+</em></p>
 
 ## Channel order wizardry
 
 Some operations assume its input tensors have a channel dimension. 
 And as you probably know, pytorch and tensorflow do not agree on the layout of such tensors.
 Pytorch adopts channel-first layout (_B**C**H_, _B**C**HW_, etc.) 
 while tensorflow works efficiently with channel-last tensors (_BH**C**_, _BHW**C**_, ...).
@@ -207,15 +208,15 @@
         return x1, x2
 
 pytorch_module = MyModule().eval()
 
 inputs = [
     torch.normal(0, 1, size=(1, 12, 32)),
 ]
-
+You can
 keras_model = nobuco.pytorch_to_keras(
     pytorch_module, inputs,
     inputs_channel_order=ChannelOrder.PYTORCH,
 )
 ```
 
 The laziness shoots us in the foot here, and we get not one transpose but two:
@@ -465,78 +466,90 @@
         shape = tf.unstack(tf.shape(x))
         if get_channel_order(x) == ChannelOrder.TENSORFLOW:
             shape = permute_keras2pytorch(shape)
         return tuple(shape)
     return func
 ```
 
+It's also possible to automatically substitute every `.shape` call with `nobuco.shape` during the tracing phase by setting `trace_shape` flag:
+
+```python
+keras_model = nobuco.pytorch_to_keras(
+  # ...
+  trace_shape=True
+)
+```
+
 ## So we put a converter inside your converter
 
-One of the operations currently not supported is mask assign.
-There's no particular reason why, I just haven't done it yet (and your contribution is highly welcome!) 
-For now, let's use it as an excuse to explain the concept of nested converters.
-Like I said, for this module, conversion will fail:
+As we've learned, Nobuco gets confused when in-place operation is applied to a slice.
+There's a way to fix that, but let's not do it now.
+Instead, we'll use it as an excuse to explain the concept of nested converters.
+So, for this module, conversion will give us incorrect result:
 
 ```python
 class MyModule(nn.Module):
     def __init__(self):
         super().__init__()
         self.conv = nn.Conv2d(3, 3, kernel_size=(3, 3), padding=(1, 1))
 
     def forward(self, x):
         x = self.conv(x)
-        x[x > 0] += 1
+        # Gives incorrect result after conversion
+        torch.relu_(x[:, 1:2, 16:25, 8::2])
+        # That's the recommended approach, but we're not going for it now
+        # x[:, 1:2, 16:25, 8::2] = torch.relu_(x[:, 1:2, 16:25, 8::2])
         return x
 ```
 
 <img src="docs/converter_inside_converter1.svg" width="100%">
 
 In the previous section, we've seen it's possible to invoke a Nobuco converter inside another Nobuco converter.
 Can we embed some third-party converter? You bet! Why? Because it might just do what we need.
 Let's consider the standard route: pytorch -> onnx -> tensorflow, with the latter step done with [onnx-tf](https://github.com/onnx/onnx-tensorflow).
 This library likes transposing stuff so much, converting the whole graph with it may introduce intolerable inference overhead. Nonetheless, it does the job.
 A sensible tradeoff would be to wrap the problematic operation into its own `nn.Module` and give it a special treat, while handling everything else with Nobuco.
 
 ```python
-class AddByMask(nn.Module):
-    def forward(self, x, mask):
-        x[mask] += 1
+class SliceReLU(nn.Module):
+    def forward(self, x):
+        torch.relu_(x[:, 1:2, 16:25, 8::2])
         return x
 
 
 class MyModule(nn.Module):
     def __init__(self):
         super().__init__()
         self.conv = nn.Conv2d(3, 3, kernel_size=(3, 3), padding=(1, 1))
 
     def forward(self, x):
         x = self.conv(x)
-        mask = x > 0
-        AddByMask()(x, mask)
+        SliceReLU()(x)
         return x
 ```
 
 ```python
 import onnx
 from onnx_tf.backend import prepare
 
 
-@nobuco.converter(AddByMask, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER, reusable=False)
-def converter_AddByMask(self, x, mask):
-    model_path = 'add_by_mask'
+@nobuco.converter(SliceReLU, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER, reusable=False)
+def converter_SliceReLU(self, x):
+    model_path = 'slice_relu'
     onnx_path = model_path + '.onnx'
 
-    # NB: onnx.export is implemented via tracing i.e. it may modify the inputs!
-    torch.onnx.export(self, (x, mask), onnx_path, opset_version=12, input_names=['input', 'mask'], dynamic_axes={'input': [0, 1, 2, 3]})
-
+    # NB: onnx.export in implemented via tracing i.e. it may modify the inputs!
+    torch.onnx.export(self, (x,), onnx_path, opset_version=12, input_names=['input'],
+                      dynamic_axes={'input': [0, 1, 2, 3]}
+                      )
     onnx_model = onnx.load(onnx_path)
     tf_rep = prepare(onnx_model)
     tf_rep.export_graph(model_path)
     model = tf.keras.models.load_model(model_path)
-    return keras.layers.Lambda(lambda x, mask: model(input=x, mask=mask))
+    return keras.layers.Lambda(lambda x: model(input=x))
 ```
 
 <img src="docs/converter_inside_converter2.svg" width="100%">
 
 ## More nice things
 
 ### Nobuco knowledge base
```

### Comparing `nobuco-0.4.9/nobuco.egg-info/SOURCES.txt` & `nobuco-0.5.0/nobuco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.9/pyproject.toml` & `nobuco-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nobuco"
-version = "0.4.9"
+version = "0.5.0"
 description = "Pytorch to Tensorflow conversion made somewhat easy"
 readme = "README.md"
 authors = [
   { name="Alexander Lutsenko", email="lex.lutsenko@gmail.com" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

