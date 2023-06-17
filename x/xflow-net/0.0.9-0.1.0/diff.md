# Comparing `tmp/xflow-net-0.0.9.tar.gz` & `tmp/xflow-net-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xflow-net-0.0.9.tar", last modified: Fri Jun 16 03:29:19 2023, max compression
+gzip compressed data, was "xflow-net-0.1.0.tar", last modified: Sat Jun 17 22:42:14 2023, max compression
```

## Comparing `xflow-net-0.0.9.tar` & `xflow-net-0.1.0.tar`

### file list

```diff
@@ -1,34 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:29:19.772961 xflow-net-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-16 03:29:05.000000 xflow-net-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-16 03:29:19.772961 xflow-net-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-06-16 03:29:05.000000 xflow-net-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:29:19.768961 xflow-net-0.0.9/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 03:29:05.000000 xflow-net-0.0.9/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-16 03:29:05.000000 xflow-net-0.0.9/examples/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-16 03:29:05.000000 xflow-net-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-16 03:29:19.772961 xflow-net-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-16 03:29:05.000000 xflow-net-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:29:19.768961 xflow-net-0.0.9/xflow/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-16 03:29:05.000000 xflow-net-0.0.9/xflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:29:19.768961 xflow-net-0.0.9/xflow/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-16 03:29:05.000000 xflow-net-0.0.9/xflow/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-16 03:29:05.000000 xflow-net-0.0.9/xflow/dataset/nx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-16 03:29:05.000000 xflow-net-0.0.9/xflow/dataset/pyg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:29:19.768961 xflow-net-0.0.9/xflow/diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-16 03:29:05.000000 xflow-net-0.0.9/xflow/diffusion/IC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-16 03:29:05.000000 xflow-net-0.0.9/xflow/diffusion/LT.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-16 03:29:05.000000 xflow-net-0.0.9/xflow/diffusion/SI.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 03:29:05.000000 xflow-net-0.0.9/xflow/diffusion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:29:19.768961 xflow-net-0.0.9/xflow/method/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 03:29:05.000000 xflow-net-0.0.9/xflow/method/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-16 03:29:05.000000 xflow-net-0.0.9/xflow/method/ibm.py
--rw-r--r--   0 runner    (1001) docker     (123)    14127 2023-06-16 03:29:05.000000 xflow-net-0.0.9/xflow/method/im.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-16 03:29:05.000000 xflow-net-0.0.9/xflow/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-16 03:29:05.000000 xflow-net-0.0.9/xflow/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-16 03:29:05.000000 xflow-net-0.0.9/xflow/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:29:19.772961 xflow-net-0.0.9/xflow_net.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-16 03:29:19.000000 xflow-net-0.0.9/xflow_net.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-16 03:29:19.000000 xflow-net-0.0.9/xflow_net.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 03:29:19.000000 xflow-net-0.0.9/xflow_net.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 03:29:19.000000 xflow-net-0.0.9/xflow_net.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-16 03:29:19.000000 xflow-net-0.0.9/xflow_net.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:42:14.198340 xflow-net-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-17 22:42:03.000000 xflow-net-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-17 22:42:14.198340 xflow-net-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-06-17 22:42:03.000000 xflow-net-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:42:14.194340 xflow-net-0.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 22:42:03.000000 xflow-net-0.1.0/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-17 22:42:03.000000 xflow-net-0.1.0/examples/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-17 22:42:03.000000 xflow-net-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-17 22:42:14.198340 xflow-net-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-17 22:42:03.000000 xflow-net-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:42:14.194340 xflow-net-0.1.0/xflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:42:14.194340 xflow-net-0.1.0/xflow/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/dataset/nx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/dataset/pyg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:42:14.194340 xflow-net-0.1.0/xflow/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/diffusion/IC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/diffusion/LT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/diffusion/SI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/diffusion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:42:14.194340 xflow-net-0.1.0/xflow/method/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/method/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:42:14.194340 xflow-net-0.1.0/xflow/method/cosasi/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/method/cosasi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:42:14.194340 xflow-net-0.1.0/xflow/method/cosasi/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/method/cosasi/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/method/cosasi/benchmark/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:42:14.198340 xflow-net-0.1.0/xflow/method/cosasi/contagion/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/method/cosasi/contagion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/method/cosasi/contagion/static_network_contagion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:42:14.198340 xflow-net-0.1.0/xflow/method/cosasi/source_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/method/cosasi/source_inference/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:42:14.198340 xflow-net-0.1.0/xflow/method/cosasi/source_inference/multiple_source/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/method/cosasi/source_inference/multiple_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/method/cosasi/source_inference/multiple_source/jordan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/method/cosasi/source_inference/multiple_source/lisn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/method/cosasi/source_inference/multiple_source/netsleuth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:42:14.198340 xflow-net-0.1.0/xflow/method/cosasi/source_inference/single_source/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/method/cosasi/source_inference/single_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/method/cosasi/source_inference/single_source/earliest_infection_first.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/method/cosasi/source_inference/single_source/jordan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/method/cosasi/source_inference/single_source/lisn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/method/cosasi/source_inference/single_source/netsleuth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/method/cosasi/source_inference/single_source/rumor_centrality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/method/cosasi/source_inference/single_source/short_fat_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10919 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/method/cosasi/source_inference/source_results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:42:14.198340 xflow-net-0.1.0/xflow/method/cosasi/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/method/cosasi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15690 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/method/cosasi/utils/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/method/cosasi/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/method/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14190 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/method/im.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/method/sl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-17 22:42:03.000000 xflow-net-0.1.0/xflow/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:42:14.198340 xflow-net-0.1.0/xflow_net.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-17 22:42:14.000000 xflow-net-0.1.0/xflow_net.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-17 22:42:14.000000 xflow-net-0.1.0/xflow_net.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 22:42:14.000000 xflow-net-0.1.0/xflow_net.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-17 22:42:14.000000 xflow-net-0.1.0/xflow_net.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-17 22:42:14.000000 xflow-net-0.1.0/xflow_net.egg-info/top_level.txt
```

### Comparing `xflow-net-0.0.9/LICENSE` & `xflow-net-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.9/PKG-INFO` & `xflow-net-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xflow-net
-Version: 0.0.9
+Version: 0.1.0
 Summary: a python library for graph flow
 Home-page: https://xflow.network/
 Author: XGraphing
 Author-email: zchen@cse.msstate.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `xflow-net-0.0.9/README.md` & `xflow-net-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.9/setup.py` & `xflow-net-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Package meta-data.
 NAME = 'xflow-net'
 DESCRIPTION = 'a python library for graph flow'
 URL = 'https://xflow.network/'
 EMAIL = 'zchen@cse.msstate.edu'
 AUTHOR = 'XGraphing'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.0.9'
+VERSION = '0.1.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
    'networkx', 'ndlib', 'torch_geometric'
 ]
 
 # What packages are optional?
```

### Comparing `xflow-net-0.0.9/xflow/dataset/nx.py` & `xflow-net-0.1.0/xflow/dataset/nx.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.9/xflow/dataset/pyg.py` & `xflow-net-0.1.0/xflow/dataset/pyg.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.9/xflow/diffusion/IC.py` & `xflow-net-0.1.0/xflow/diffusion/IC.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.9/xflow/diffusion/LT.py` & `xflow-net-0.1.0/xflow/diffusion/LT.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.9/xflow/diffusion/SI.py` & `xflow-net-0.1.0/xflow/diffusion/SI.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.9/xflow/method/ibm.py` & `xflow-net-0.1.0/xflow/method/ibm.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 import statistics as s
 import random
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import time
 import random
-from xflow.diffusion import SI, IC, LT
-
+from xflow.diffusion.SI import SI
+from xflow.diffusion.IC import IC
+from xflow.diffusion.LT import LT
 # random
 
 # baselines: simulation based
 
 # greedy
 def greedy(g, config, budget, seeds, rounds=100, model='SI', beta=0.1):
```

### Comparing `xflow-net-0.0.9/xflow/method/im.py` & `xflow-net-0.1.0/xflow/method/im.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 import pandas as pd
 import time
 from random import uniform, seed
 
 from collections import Counter
 import operator
 import copy
-from xflow.diffusion import SI, IC, LT
+from xflow.diffusion.SI import SI
+from xflow.diffusion.IC import IC
+from xflow.diffusion.LT import LT
 
 # random
 
 # baselines: simulation based
 
 # greedy
 def greedy(g, config, budget, rounds=100, model='SI', beta=0.1):
```

### Comparing `xflow-net-0.0.9/xflow/visualization.py` & `xflow-net-0.1.0/xflow/visualization.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.9/xflow_net.egg-info/PKG-INFO` & `xflow-net-0.1.0/xflow_net.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xflow-net
-Version: 0.0.9
+Version: 0.1.0
 Summary: a python library for graph flow
 Home-page: https://xflow.network/
 Author: XGraphing
 Author-email: zchen@cse.msstate.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

