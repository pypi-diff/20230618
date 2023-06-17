# Comparing `tmp/PyXAB-0.2.4.tar.gz` & `tmp/PyXAB-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyXAB-0.2.4.tar", last modified: Mon Jun 12 00:06:57 2023, max compression
+gzip compressed data, was "dist/PyXAB-0.3.0.tar", last modified: Sat Jun 17 23:09:01 2023, max compression
```

## Comparing `PyXAB-0.2.4.tar` & `PyXAB-0.3.0.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-12 00:06:57.869989 PyXAB-0.2.4/
--rw-r--r--   0 william    (501) staff       (20)     1066 2022-03-24 15:30:00.000000 PyXAB-0.2.4/LICENSE
--rw-r--r--   0 william    (501) staff       (20)    16675 2023-06-12 00:06:57.870227 PyXAB-0.2.4/PKG-INFO
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-12 00:06:57.851595 PyXAB-0.2.4/PyXAB/
--rw-r--r--   0 william    (501) staff       (20)        0 2022-03-22 23:40:33.000000 PyXAB-0.2.4/PyXAB/__init__.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-12 00:06:57.860496 PyXAB-0.2.4/PyXAB/algos/
--rw-r--r--   0 william    (501) staff       (20)     1415 2023-05-24 05:55:11.000000 PyXAB-0.2.4/PyXAB/algos/Algo.py
--rw-r--r--   0 william    (501) staff       (20)     6201 2023-05-24 05:55:19.000000 PyXAB-0.2.4/PyXAB/algos/DOO.py
--rw-r--r--   0 william    (501) staff       (20)     5406 2023-05-24 05:55:19.000000 PyXAB-0.2.4/PyXAB/algos/GPO.py
--rw-r--r--   0 william    (501) staff       (20)    10197 2023-05-24 05:55:19.000000 PyXAB-0.2.4/PyXAB/algos/HCT.py
--rw-r--r--   0 william    (501) staff       (20)     8980 2023-05-24 05:55:19.000000 PyXAB-0.2.4/PyXAB/algos/HOO.py
--rw-r--r--   0 william    (501) staff       (20)     2428 2023-05-24 05:55:19.000000 PyXAB-0.2.4/PyXAB/algos/PCT.py
--rw-r--r--   0 william    (501) staff       (20)     5740 2023-05-24 05:55:19.000000 PyXAB-0.2.4/PyXAB/algos/POO.py
--rw-r--r--   0 william    (501) staff       (20)     5461 2023-05-24 05:55:19.000000 PyXAB-0.2.4/PyXAB/algos/SOO.py
--rw-r--r--   0 william    (501) staff       (20)     7241 2023-05-24 05:55:19.000000 PyXAB-0.2.4/PyXAB/algos/SequOOL.py
--rw-r--r--   0 william    (501) staff       (20)     7408 2023-05-24 05:55:19.000000 PyXAB-0.2.4/PyXAB/algos/StoSOO.py
--rw-r--r--   0 william    (501) staff       (20)    11065 2023-05-24 05:55:19.000000 PyXAB-0.2.4/PyXAB/algos/StroquOOL.py
--rw-r--r--   0 william    (501) staff       (20)    12008 2023-05-24 05:55:19.000000 PyXAB-0.2.4/PyXAB/algos/VHCT.py
--rw-r--r--   0 william    (501) staff       (20)     2430 2023-05-24 05:55:19.000000 PyXAB-0.2.4/PyXAB/algos/VPCT.py
--rw-r--r--   0 william    (501) staff       (20)     5288 2023-05-24 05:55:19.000000 PyXAB-0.2.4/PyXAB/algos/Zooming.py
--rw-r--r--   0 william    (501) staff       (20)      331 2023-05-24 05:55:11.000000 PyXAB-0.2.4/PyXAB/algos/__init__.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-12 00:06:57.864468 PyXAB-0.2.4/PyXAB/partition/
--rw-r--r--   0 william    (501) staff       (20)     2806 2023-03-13 03:58:11.000000 PyXAB-0.2.4/PyXAB/partition/BinaryPartition.py
--rw-r--r--   0 william    (501) staff       (20)     3131 2023-03-13 03:58:11.000000 PyXAB-0.2.4/PyXAB/partition/DimensionBinaryPartition.py
--rw-r--r--   0 william    (501) staff       (20)     2807 2023-03-13 03:58:11.000000 PyXAB-0.2.4/PyXAB/partition/KaryPartition.py
--rw-r--r--   0 william    (501) staff       (20)     2298 2023-02-16 03:14:10.000000 PyXAB-0.2.4/PyXAB/partition/Node.py
--rw-r--r--   0 william    (501) staff       (20)     3019 2023-03-13 03:58:11.000000 PyXAB-0.2.4/PyXAB/partition/Partition.py
--rw-r--r--   0 william    (501) staff       (20)     2861 2023-03-13 03:58:11.000000 PyXAB-0.2.4/PyXAB/partition/RandomBinaryPartition.py
--rw-r--r--   0 william    (501) staff       (20)     3068 2023-03-13 03:58:11.000000 PyXAB-0.2.4/PyXAB/partition/RandomKaryPartition.py
--rw-r--r--   0 william    (501) staff       (20)       83 2023-03-13 03:58:11.000000 PyXAB-0.2.4/PyXAB/partition/__init__.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-12 00:06:57.867975 PyXAB-0.2.4/PyXAB/synthetic_obj/
--rw-r--r--   0 william    (501) staff       (20)     2534 2023-03-13 03:58:11.000000 PyXAB-0.2.4/PyXAB/synthetic_obj/Ackley.py
--rw-r--r--   0 william    (501) staff       (20)     1027 2023-03-13 03:58:11.000000 PyXAB-0.2.4/PyXAB/synthetic_obj/Cexample.py
--rw-r--r--   0 william    (501) staff       (20)     1224 2023-03-13 03:58:11.000000 PyXAB-0.2.4/PyXAB/synthetic_obj/DifficultFunc.py
--rw-r--r--   0 william    (501) staff       (20)     4145 2023-03-13 03:58:11.000000 PyXAB-0.2.4/PyXAB/synthetic_obj/DoubleSine.py
--rw-r--r--   0 william    (501) staff       (20)     2118 2023-03-13 03:58:11.000000 PyXAB-0.2.4/PyXAB/synthetic_obj/Garland.py
--rw-r--r--   0 william    (501) staff       (20)     2095 2023-03-13 03:58:11.000000 PyXAB-0.2.4/PyXAB/synthetic_obj/Himmelblau.py
--rw-r--r--   0 william    (501) staff       (20)      484 2023-02-16 02:41:47.000000 PyXAB-0.2.4/PyXAB/synthetic_obj/Objective.py
--rw-r--r--   0 william    (501) staff       (20)     2116 2023-03-13 03:58:11.000000 PyXAB-0.2.4/PyXAB/synthetic_obj/Rastrigin.py
--rw-r--r--   0 william    (501) staff       (20)      380 2023-02-16 02:41:47.000000 PyXAB-0.2.4/PyXAB/synthetic_obj/__init__.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-12 00:06:57.869550 PyXAB-0.2.4/PyXAB/utils/
--rw-r--r--   0 william    (501) staff       (20)        0 2022-03-22 23:40:33.000000 PyXAB-0.2.4/PyXAB/utils/__init__.py
--rw-r--r--   0 william    (501) staff       (20)     1467 2023-02-16 03:14:10.000000 PyXAB-0.2.4/PyXAB/utils/plot.py
--rw-r--r--   0 william    (501) staff       (20)     2477 2023-05-24 05:55:11.000000 PyXAB-0.2.4/PyXAB/utils/run_synthetic.py
--rw-r--r--   0 william    (501) staff       (20)     4350 2023-03-13 03:58:11.000000 PyXAB-0.2.4/PyXAB/utils/visualize_gif.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-12 00:06:57.853044 PyXAB-0.2.4/PyXAB.egg-info/
--rw-r--r--   0 william    (501) staff       (20)    16675 2023-06-12 00:06:57.000000 PyXAB-0.2.4/PyXAB.egg-info/PKG-INFO
--rw-r--r--   0 william    (501) staff       (20)     1179 2023-06-12 00:06:57.000000 PyXAB-0.2.4/PyXAB.egg-info/SOURCES.txt
--rw-r--r--   0 william    (501) staff       (20)        1 2023-06-12 00:06:57.000000 PyXAB-0.2.4/PyXAB.egg-info/dependency_links.txt
--rw-r--r--   0 william    (501) staff       (20)       25 2023-06-12 00:06:57.000000 PyXAB-0.2.4/PyXAB.egg-info/requires.txt
--rw-r--r--   0 william    (501) staff       (20)        6 2023-06-12 00:06:57.000000 PyXAB-0.2.4/PyXAB.egg-info/top_level.txt
--rw-r--r--   0 william    (501) staff       (20)    14238 2023-06-11 23:42:09.000000 PyXAB-0.2.4/README.md
--rw-r--r--   0 william    (501) staff       (20)      103 2023-06-12 00:06:57.870678 PyXAB-0.2.4/setup.cfg
--rw-r--r--   0 william    (501) staff       (20)     3907 2023-06-11 23:42:09.000000 PyXAB-0.2.4/setup.py
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-17 23:09:01.009141 PyXAB-0.3.0/
+-rw-r--r--   0 william    (501) staff       (20)     1066 2022-03-24 15:30:00.000000 PyXAB-0.3.0/LICENSE
+-rw-r--r--   0 william    (501) staff       (20)    16965 2023-06-17 23:09:01.009353 PyXAB-0.3.0/PKG-INFO
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-17 23:09:00.990526 PyXAB-0.3.0/PyXAB/
+-rw-r--r--   0 william    (501) staff       (20)        0 2022-03-22 23:40:33.000000 PyXAB-0.3.0/PyXAB/__init__.py
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-17 23:09:00.999474 PyXAB-0.3.0/PyXAB/algos/
+-rw-r--r--   0 william    (501) staff       (20)     1415 2023-05-24 05:55:11.000000 PyXAB-0.3.0/PyXAB/algos/Algo.py
+-rw-r--r--   0 william    (501) staff       (20)     6201 2023-05-24 05:55:19.000000 PyXAB-0.3.0/PyXAB/algos/DOO.py
+-rw-r--r--   0 william    (501) staff       (20)     5406 2023-05-24 05:55:19.000000 PyXAB-0.3.0/PyXAB/algos/GPO.py
+-rw-r--r--   0 william    (501) staff       (20)    10197 2023-05-24 05:55:19.000000 PyXAB-0.3.0/PyXAB/algos/HCT.py
+-rw-r--r--   0 william    (501) staff       (20)     8980 2023-05-24 05:55:19.000000 PyXAB-0.3.0/PyXAB/algos/HOO.py
+-rw-r--r--   0 william    (501) staff       (20)     2428 2023-05-24 05:55:19.000000 PyXAB-0.3.0/PyXAB/algos/PCT.py
+-rw-r--r--   0 william    (501) staff       (20)     5740 2023-05-24 05:55:19.000000 PyXAB-0.3.0/PyXAB/algos/POO.py
+-rw-r--r--   0 william    (501) staff       (20)     5057 2023-06-17 04:52:40.000000 PyXAB-0.3.0/PyXAB/algos/SOO.py
+-rw-r--r--   0 william    (501) staff       (20)     7327 2023-06-17 04:52:40.000000 PyXAB-0.3.0/PyXAB/algos/SequOOL.py
+-rw-r--r--   0 william    (501) staff       (20)     7408 2023-05-24 05:55:19.000000 PyXAB-0.3.0/PyXAB/algos/StoSOO.py
+-rw-r--r--   0 william    (501) staff       (20)    11151 2023-06-17 04:52:40.000000 PyXAB-0.3.0/PyXAB/algos/StroquOOL.py
+-rw-r--r--   0 william    (501) staff       (20)    12008 2023-05-24 05:55:19.000000 PyXAB-0.3.0/PyXAB/algos/VHCT.py
+-rw-r--r--   0 william    (501) staff       (20)     2430 2023-05-24 05:55:19.000000 PyXAB-0.3.0/PyXAB/algos/VPCT.py
+-rw-r--r--   0 william    (501) staff       (20)     9343 2023-06-17 05:10:22.000000 PyXAB-0.3.0/PyXAB/algos/VROOM.py
+-rw-r--r--   0 william    (501) staff       (20)     5288 2023-05-24 05:55:19.000000 PyXAB-0.3.0/PyXAB/algos/Zooming.py
+-rw-r--r--   0 william    (501) staff       (20)      331 2023-05-24 05:55:11.000000 PyXAB-0.3.0/PyXAB/algos/__init__.py
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-17 23:09:01.002880 PyXAB-0.3.0/PyXAB/partition/
+-rw-r--r--   0 william    (501) staff       (20)     2806 2023-03-13 03:58:11.000000 PyXAB-0.3.0/PyXAB/partition/BinaryPartition.py
+-rw-r--r--   0 william    (501) staff       (20)     3131 2023-03-13 03:58:11.000000 PyXAB-0.3.0/PyXAB/partition/DimensionBinaryPartition.py
+-rw-r--r--   0 william    (501) staff       (20)     2807 2023-03-13 03:58:11.000000 PyXAB-0.3.0/PyXAB/partition/KaryPartition.py
+-rw-r--r--   0 william    (501) staff       (20)     2298 2023-02-16 03:14:10.000000 PyXAB-0.3.0/PyXAB/partition/Node.py
+-rw-r--r--   0 william    (501) staff       (20)     3019 2023-03-13 03:58:11.000000 PyXAB-0.3.0/PyXAB/partition/Partition.py
+-rw-r--r--   0 william    (501) staff       (20)     2861 2023-03-13 03:58:11.000000 PyXAB-0.3.0/PyXAB/partition/RandomBinaryPartition.py
+-rw-r--r--   0 william    (501) staff       (20)     3068 2023-03-13 03:58:11.000000 PyXAB-0.3.0/PyXAB/partition/RandomKaryPartition.py
+-rw-r--r--   0 william    (501) staff       (20)       83 2023-03-13 03:58:11.000000 PyXAB-0.3.0/PyXAB/partition/__init__.py
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-17 23:09:01.006829 PyXAB-0.3.0/PyXAB/synthetic_obj/
+-rw-r--r--   0 william    (501) staff       (20)     2534 2023-03-13 03:58:11.000000 PyXAB-0.3.0/PyXAB/synthetic_obj/Ackley.py
+-rw-r--r--   0 william    (501) staff       (20)     1027 2023-03-13 03:58:11.000000 PyXAB-0.3.0/PyXAB/synthetic_obj/Cexample.py
+-rw-r--r--   0 william    (501) staff       (20)     1224 2023-03-13 03:58:11.000000 PyXAB-0.3.0/PyXAB/synthetic_obj/DifficultFunc.py
+-rw-r--r--   0 william    (501) staff       (20)     4145 2023-03-13 03:58:11.000000 PyXAB-0.3.0/PyXAB/synthetic_obj/DoubleSine.py
+-rw-r--r--   0 william    (501) staff       (20)     2118 2023-03-13 03:58:11.000000 PyXAB-0.3.0/PyXAB/synthetic_obj/Garland.py
+-rw-r--r--   0 william    (501) staff       (20)     2095 2023-03-13 03:58:11.000000 PyXAB-0.3.0/PyXAB/synthetic_obj/Himmelblau.py
+-rw-r--r--   0 william    (501) staff       (20)      484 2023-02-16 02:41:47.000000 PyXAB-0.3.0/PyXAB/synthetic_obj/Objective.py
+-rw-r--r--   0 william    (501) staff       (20)     2116 2023-03-13 03:58:11.000000 PyXAB-0.3.0/PyXAB/synthetic_obj/Rastrigin.py
+-rw-r--r--   0 william    (501) staff       (20)      380 2023-02-16 02:41:47.000000 PyXAB-0.3.0/PyXAB/synthetic_obj/__init__.py
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-17 23:09:01.008691 PyXAB-0.3.0/PyXAB/utils/
+-rw-r--r--   0 william    (501) staff       (20)        0 2022-03-22 23:40:33.000000 PyXAB-0.3.0/PyXAB/utils/__init__.py
+-rw-r--r--   0 william    (501) staff       (20)     1467 2023-02-16 03:14:10.000000 PyXAB-0.3.0/PyXAB/utils/plot.py
+-rw-r--r--   0 william    (501) staff       (20)     2477 2023-05-24 05:55:11.000000 PyXAB-0.3.0/PyXAB/utils/run_synthetic.py
+-rw-r--r--   0 william    (501) staff       (20)     4350 2023-03-13 03:58:11.000000 PyXAB-0.3.0/PyXAB/utils/visualize_gif.py
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-17 23:09:00.991896 PyXAB-0.3.0/PyXAB.egg-info/
+-rw-r--r--   0 william    (501) staff       (20)    16965 2023-06-17 23:09:00.000000 PyXAB-0.3.0/PyXAB.egg-info/PKG-INFO
+-rw-r--r--   0 william    (501) staff       (20)     1200 2023-06-17 23:09:00.000000 PyXAB-0.3.0/PyXAB.egg-info/SOURCES.txt
+-rw-r--r--   0 william    (501) staff       (20)        1 2023-06-17 23:09:00.000000 PyXAB-0.3.0/PyXAB.egg-info/dependency_links.txt
+-rw-r--r--   0 william    (501) staff       (20)       25 2023-06-17 23:09:00.000000 PyXAB-0.3.0/PyXAB.egg-info/requires.txt
+-rw-r--r--   0 william    (501) staff       (20)        6 2023-06-17 23:09:00.000000 PyXAB-0.3.0/PyXAB.egg-info/top_level.txt
+-rw-r--r--   0 william    (501) staff       (20)    14520 2023-06-17 05:14:45.000000 PyXAB-0.3.0/README.md
+-rw-r--r--   0 william    (501) staff       (20)      103 2023-06-17 23:09:01.009797 PyXAB-0.3.0/setup.cfg
+-rw-r--r--   0 william    (501) staff       (20)     3907 2023-06-17 04:25:10.000000 PyXAB-0.3.0/setup.py
```

### Comparing `PyXAB-0.2.4/LICENSE` & `PyXAB-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PKG-INFO` & `PyXAB-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyXAB
-Version: 0.2.4
+Version: 0.3.0
 Summary: PyXAB - A Python Library for X-Armed Bandit and Online Blackbox Optimization Algorithms.
 Home-page: https://github.com/WilliamLwj/PyXAB
 Author: Wenjie Li, Haoze Li, Qifan Song, Jean Honorio
 Author-email: lil3549@purdue.edu
 License: MIT
 Description: 
         
@@ -139,14 +139,15 @@
         | [StoSOO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py)       | [Stochastic Simultaneous Optimistic Optimization](http://proceedings.mlr.press/v28/valko13.pdf)                                                                                          | 2013 |
         | [HCT](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/HCT.py)             | [Online Stochastic Optimization Under Correlated Bandit Feedback](https://proceedings.mlr.press/v32/azar14.html)                                                                         | 2014 |
         | [POO*](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/POO.py)            | [Black-box optimization of noisy functions with unknown smoothness](https://papers.nips.cc/paper/2015/hash/ab817c9349cf9c4f6877e1894a1faa00-Abstract.html)                               | 2015 |
         | [GPO*](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/GPO.py)            | [General Parallel Optimization Without A Metric](https://proceedings.mlr.press/v98/xuedong19a.html)                                                                                      | 2019 |
         | [PCT](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/PCT.py)             | [General Parallel Optimization Without A Metric](https://proceedings.mlr.press/v98/xuedong19a.html)                                                                                      | 2019 |
         | [SequOOL](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/SequOOL.py)     | [A Simple Parameter-free And Adaptive Approach to Optimization Under A Minimal Local Smoothness Assumption](https://arxiv.org/pdf/1810.00997.pdf)                                        | 2019 |
         | [StroquOOL](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StroquOOL.py) | [A Simple Parameter-free And Adaptive Approach to Optimization Under A Minimal Local Smoothness Assumption](https://arxiv.org/pdf/1810.00997.pdf)                                        | 2019 |
+        | [VROOM](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/VROOM.py)         | [Derivative-Free & Order-Robust Optimisation](https://arxiv.org/pdf/1910.04034.pdf)                                                                                                      | 2020 |
         | [VHCT](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/VHCT.py)           | [Optimum-statistical Collaboration Towards General and Efficient Black-box Optimization](https://openreview.net/forum?id=ClIcmwdlxn)                                                     | 2023 |
         | [VPCT](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/VPCT.py)           | N.A. ([GPO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/GPO.py) + [VHCT](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/VHCT.py))                               | N.A. |
         
         
         ### Hierarchical partition 
         
         | Partition                                                                                                             | Description                                                                                                        |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyXAB Version: 0.2.4 Summary: PyXAB - A Python
+Metadata-Version: 2.1 Name: PyXAB Version: 0.3.0 Summary: PyXAB - A Python
 Library for X-Armed Bandit and Online Blackbox Optimization Algorithms. Home-
 page: https://github.com/WilliamLwj/PyXAB Author: Wenjie Li, Haoze Li, Qifan
 Song, Jean Honorio Author-email: lil3549@purdue.edu License: MIT Description: #
 PyXAB - Python *X*-Armed Bandit
 [PyPI_version] [https://codecov.io/gh/WilliamLwj/PyXAB/branch/main/graph/
 badge.svg?token=VACRX9AQBM] [Documentation_Status] [Code_style:_black]
 [testing] [github-PyXAB_forks] [github-PyXAB_stars] [downloads] [github-PyXAB
@@ -81,50 +81,52 @@
 Without A Metric](https://proceedings.mlr.press/v98/xuedong19a.html) | 2019 | |
 [SequOOL](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/SequOOL.py)
 | [A Simple Parameter-free And Adaptive Approach to Optimization Under A
 Minimal Local Smoothness Assumption](https://arxiv.org/pdf/1810.00997.pdf) |
 2019 | | [StroquOOL](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/
 StroquOOL.py) | [A Simple Parameter-free And Adaptive Approach to Optimization
 Under A Minimal Local Smoothness Assumption](https://arxiv.org/pdf/
-1810.00997.pdf) | 2019 | | [VHCT](https://github.com/WilliamLwj/PyXAB/blob/
-main/PyXAB/algos/VHCT.py) | [Optimum-statistical Collaboration Towards General
-and Efficient Black-box Optimization](https://openreview.net/
-forum?id=ClIcmwdlxn) | 2023 | | [VPCT](https://github.com/WilliamLwj/PyXAB/
-blob/main/PyXAB/algos/VPCT.py) | N.A. ([GPO](https://github.com/WilliamLwj/
-PyXAB/blob/main/PyXAB/algos/GPO.py) + [VHCT](https://github.com/WilliamLwj/
-PyXAB/blob/main/PyXAB/algos/VHCT.py)) | N.A. | ### Hierarchical partition |
-Partition | Description | |----------------------------------------------------
--------------------------------------------------------------------|-----------
+1810.00997.pdf) | 2019 | | [VROOM](https://github.com/WilliamLwj/PyXAB/blob/
+main/PyXAB/algos/VROOM.py) | [Derivative-Free & Order-Robust Optimisation]
+(https://arxiv.org/pdf/1910.04034.pdf) | 2020 | | [VHCT](https://github.com/
+WilliamLwj/PyXAB/blob/main/PyXAB/algos/VHCT.py) | [Optimum-statistical
+Collaboration Towards General and Efficient Black-box Optimization](https://
+openreview.net/forum?id=ClIcmwdlxn) | 2023 | | [VPCT](https://github.com/
+WilliamLwj/PyXAB/blob/main/PyXAB/algos/VPCT.py) | N.A. ([GPO](https://
+github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/GPO.py) + [VHCT](https://
+github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/VHCT.py)) | N.A. | ###
+Hierarchical partition | Partition | Description | |---------------------------
 -------------------------------------------------------------------------------
---------------------------| | [BinaryPartition](https://github.com/WilliamLwj/
-PyXAB/blob/main/PyXAB/partition/BinaryPartition.py) | Equal-size binary
-partition of the parameter space, the split dimension is chosen uniform
-randomly | | [RandomBinaryPartition](https://github.com/WilliamLwj/PyXAB/blob/
-main/PyXAB/partition/RandomBinaryPartition.py) | Random-size binary partition
+-------------|-----------------------------------------------------------------
+---------------------------------------------------| | [BinaryPartition](https:
+//github.com/WilliamLwj/PyXAB/blob/main/PyXAB/partition/BinaryPartition.py) |
+Equal-size binary partition of the parameter space, the split dimension is
+chosen uniform randomly | | [RandomBinaryPartition](https://github.com/
+WilliamLwj/PyXAB/blob/main/PyXAB/partition/RandomBinaryPartition.py) | Random-
+size binary partition of the parameter space, the split dimension is chosen
+uniform randomly | | [DimensionBinaryPartition](https://github.com/WilliamLwj/
+PyXAB/blob/main/PyXAB/partition/DimensionBinaryPartition.py) | Equal-size
+partition of the space with a binary split on each dimension, the number of
+children of one node is 2^d | | [KaryPartition](https://github.com/WilliamLwj/
+PyXAB/blob/main/PyXAB/partition/KaryPartition.py) | Equal-size K-ary partition
 of the parameter space, the split dimension is chosen uniform randomly | |
-[DimensionBinaryPartition](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/
-partition/DimensionBinaryPartition.py) | Equal-size partition of the space with
-a binary split on each dimension, the number of children of one node is 2^d | |
-[KaryPartition](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/partition/
-KaryPartition.py) | Equal-size K-ary partition of the parameter space, the
-split dimension is chosen uniform randomly | | [RandomKaryPartition](https://
-github.com/WilliamLwj/PyXAB/blob/main/PyXAB/partition/RandomKaryPartition.py) |
-Random-size K-ary partition of the parameter space, the split dimension is
-chosen uniform randomly | ### Synthetic objectives * Some of these objectives
-can be found [on Wikipedia](https://en.wikipedia.org/wiki/
-Test_functions_for_optimization) | Objectives [Image]| Image | | --- |--- | |
-[Garland](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/synthetic_obj/
-Garland.py) | [Garland] | | [DoubleSine](https://github.com/WilliamLwj/PyXAB/
-blob/main/PyXAB/synthetic_obj/DoubleSine.py) | [DoubleSine] | | [DifficultFunc]
-(https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/synthetic_obj/
-DifficultFunc.py) | [DifficultFunc] | | [Ackley](https://github.com/WilliamLwj/
-PyXAB/blob/main/PyXAB/synthetic_obj/Ackley.py) | [Ackley] | | [Himmelblau]
-(https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/synthetic_obj/
-Himmelblau.py) | [Himmelblau] | | [Rastrigin](https://github.com/WilliamLwj/
-PyXAB/blob/main/PyXAB/synthetic_obj/Rastrigin.py) | [Rastrigin] | ##
+[RandomKaryPartition](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/
+partition/RandomKaryPartition.py) | Random-size K-ary partition of the
+parameter space, the split dimension is chosen uniform randomly | ### Synthetic
+objectives * Some of these objectives can be found [on Wikipedia](https://
+en.wikipedia.org/wiki/Test_functions_for_optimization) | Objectives [Image]|
+Image | | --- |--- | | [Garland](https://github.com/WilliamLwj/PyXAB/blob/main/
+PyXAB/synthetic_obj/Garland.py) | [Garland] | | [DoubleSine](https://
+github.com/WilliamLwj/PyXAB/blob/main/PyXAB/synthetic_obj/DoubleSine.py) |
+[DoubleSine] | | [DifficultFunc](https://github.com/WilliamLwj/PyXAB/blob/main/
+PyXAB/synthetic_obj/DifficultFunc.py) | [DifficultFunc] | | [Ackley](https://
+github.com/WilliamLwj/PyXAB/blob/main/PyXAB/synthetic_obj/Ackley.py) | [Ackley]
+| | [Himmelblau](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/
+synthetic_obj/Himmelblau.py) | [Himmelblau] | | [Rastrigin](https://github.com/
+WilliamLwj/PyXAB/blob/main/PyXAB/synthetic_obj/Rastrigin.py) | [Rastrigin] | ##
 Contributing We appreciate all forms of help and contributions, including but
 not limited to * Star and watch our project * Open an issue for any bugs you
 find or features you want to add to our library * Fork our project and submit a
 pull request with your valuable codes Please read the [contributing
 instructions](https://pyxab.readthedocs.io/en/latest/info/contributing.html)
 before submitting a pull request. ## Citations If you use our package in your
 research or projects, we kindly ask you to cite our work ```text @misc
```

### Comparing `PyXAB-0.2.4/PyXAB/algos/Algo.py` & `PyXAB-0.3.0/PyXAB/algos/Algo.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PyXAB/algos/DOO.py` & `PyXAB-0.3.0/PyXAB/algos/DOO.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PyXAB/algos/GPO.py` & `PyXAB-0.3.0/PyXAB/algos/GPO.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PyXAB/algos/HCT.py` & `PyXAB-0.3.0/PyXAB/algos/HCT.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PyXAB/algos/HOO.py` & `PyXAB-0.3.0/PyXAB/algos/HOO.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PyXAB/algos/PCT.py` & `PyXAB-0.3.0/PyXAB/algos/PCT.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PyXAB/algos/POO.py` & `PyXAB-0.3.0/PyXAB/algos/POO.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PyXAB/algos/SOO.py` & `PyXAB-0.3.0/PyXAB/algos/SOO.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,15 +121,14 @@
         -------
         point: list
             the point to be evaluated
         """
 
         self.iteration = time
         node_list = self.partition.get_node_list()
-        flag = False  # indicate if we should terminate the iteration
 
         while True:
             h = 0
             v_max = -np.inf
             while h <= min(self.partition.get_depth(), self.h_max):
                 max_value = -np.inf
                 max_node = None
@@ -144,23 +143,17 @@
                         if (
                             node.get_reward() >= max_value
                         ):  # find the leaf node with maximal reward
                             max_value = node.get_reward()
                             max_node = node
                 if max_value >= v_max:
                     if max_node is not None:  # Found a leaf node
-                        self.partition.make_children(max_node, newlayer=True)
+                        self.partition.make_children(max_node, newlayer=(h>=self.partition.get_depth()))
                         v_max = max_value
                 h += 1
-            if max_node is None:
-                if (
-                    flag
-                ):  # We terminate the outer loop if we cannot find a leaf node that satisfies those conditions
-                    return self.partition.get_root().get_cpoint()
-                flag = True  # We set flag = True iff the loop cannot find the node starting from root.
 
     def receive_reward(self, time, reward):
         """
         The receive_reward function of SOO to obtain the reward and update Statistics (for current node)
 
         Parameters
         ----------
```

### Comparing `PyXAB-0.2.4/PyXAB/algos/SequOOL.py` & `PyXAB-0.3.0/PyXAB/algos/SequOOL.py`

 * *Files 6% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         node_list = self.partition.get_node_list()
         self.iteration = t
 
         if self.curr_depth <= self.h_max:
             if self.curr_depth == 0:
                 node = node_list[0][0]
                 if node.get_children() is None:
-                    self.partition.make_children(node, newlayer=True)
+                    self.partition.make_children(node, newlayer=(self.curr_depth >= self.partition.get_depth()))
                 if self.loc < len(node.get_children()):
                     if self.loc == len(node.get_children()) - 1:
                         self.loc = 0
                         self.curr_depth += 1
                         self.budget = math.floor(self.h_max / self.curr_depth)
                         self.chosen.append(node.get_children()[-1])
                         self.curr_node = node.get_children()[-1]
@@ -180,15 +180,15 @@
                     if node.not_opened():
                         num += 1
                         if node.get_reward() >= max_value:
                             max_value = node.get_reward()
                             max_node = node
 
                 if max_node.get_children() is None:
-                    self.partition.make_children(max_node, newlayer=True)
+                    self.partition.make_children(max_node, newlayer=(self.curr_depth >= self.partition.get_depth()))
                 if self.loc < len(max_node.get_children()):
                     if self.loc == len(max_node.get_children()) - 1:
                         max_node.open()
                         self.loc = 0
                         self.budget -= 1
                         if self.budget == 0 or num == 1:
                             self.curr_depth += 1
```

### Comparing `PyXAB-0.2.4/PyXAB/algos/StoSOO.py` & `PyXAB-0.3.0/PyXAB/algos/StoSOO.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PyXAB/algos/StroquOOL.py` & `PyXAB-0.3.0/PyXAB/algos/StroquOOL.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,15 +210,15 @@
         self.iteration = time
         node_list = self.partition.get_node_list()
 
         if self.curr_depth <= self.h_max:
             # init
             if self.curr_depth == 0:
                 if node_list[0][0].get_children() is None:
-                    self.partition.make_children(node_list[0][0], newlayer=True)
+                    self.partition.make_children(node_list[0][0], newlayer=(self.curr_depth >= self.partition.get_depth()))
                     self.chosen.append(node_list[0][0].get_children()[0])
                     self.chosen.append(node_list[0][0].get_children()[1])
                 if self.iteration <= self.h_max:
                     self.curr_node = node_list[0][0].get_children()[0]
                     return node_list[0][0].get_children()[0].get_cpoint()
                 if self.h_max < self.iteration <= 2 * self.h_max:
                     if self.iteration == 2 * self.h_max:
@@ -241,15 +241,15 @@
                             node.compute_mean_reward()
                             if node.get_mean_reward() >= max_reward:
                                 max_reward = node.get_mean_reward()
                                 self.max_node = node
                     self.eval = False
                     # partition
                     if self.max_node.get_children() is None:
-                        self.partition.make_children(self.max_node, newlayer=True)
+                        self.partition.make_children(self.max_node, newlayer=(self.curr_depth >= self.partition.get_depth()))
                         self.chosen.append(self.max_node.get_children()[0])
                         self.chosen.append(self.max_node.get_children()[1])
                 # evaluate children
                 if self.iteration <= self.time_stamp + 2 ** self.curr_p:
                     self.curr_node = self.max_node.get_children()[0]
                     return self.max_node.get_children()[0].get_cpoint()
                 if (
```

### Comparing `PyXAB-0.2.4/PyXAB/algos/VHCT.py` & `PyXAB-0.3.0/PyXAB/algos/VHCT.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PyXAB/algos/VPCT.py` & `PyXAB-0.3.0/PyXAB/algos/VPCT.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PyXAB/algos/Zooming.py` & `PyXAB-0.3.0/PyXAB/algos/Zooming.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PyXAB/partition/BinaryPartition.py` & `PyXAB-0.3.0/PyXAB/partition/BinaryPartition.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PyXAB/partition/DimensionBinaryPartition.py` & `PyXAB-0.3.0/PyXAB/partition/DimensionBinaryPartition.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PyXAB/partition/KaryPartition.py` & `PyXAB-0.3.0/PyXAB/partition/KaryPartition.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PyXAB/partition/Node.py` & `PyXAB-0.3.0/PyXAB/partition/Node.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PyXAB/partition/Partition.py` & `PyXAB-0.3.0/PyXAB/partition/Partition.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PyXAB/partition/RandomBinaryPartition.py` & `PyXAB-0.3.0/PyXAB/partition/RandomBinaryPartition.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PyXAB/partition/RandomKaryPartition.py` & `PyXAB-0.3.0/PyXAB/partition/RandomKaryPartition.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PyXAB/synthetic_obj/Ackley.py` & `PyXAB-0.3.0/PyXAB/synthetic_obj/Ackley.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PyXAB/synthetic_obj/Cexample.py` & `PyXAB-0.3.0/PyXAB/synthetic_obj/Cexample.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PyXAB/synthetic_obj/DifficultFunc.py` & `PyXAB-0.3.0/PyXAB/synthetic_obj/DifficultFunc.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PyXAB/synthetic_obj/DoubleSine.py` & `PyXAB-0.3.0/PyXAB/synthetic_obj/DoubleSine.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PyXAB/synthetic_obj/Garland.py` & `PyXAB-0.3.0/PyXAB/synthetic_obj/Garland.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PyXAB/synthetic_obj/Himmelblau.py` & `PyXAB-0.3.0/PyXAB/synthetic_obj/Himmelblau.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PyXAB/synthetic_obj/Rastrigin.py` & `PyXAB-0.3.0/PyXAB/synthetic_obj/Rastrigin.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PyXAB/utils/plot.py` & `PyXAB-0.3.0/PyXAB/utils/plot.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PyXAB/utils/run_synthetic.py` & `PyXAB-0.3.0/PyXAB/utils/run_synthetic.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PyXAB/utils/visualize_gif.py` & `PyXAB-0.3.0/PyXAB/utils/visualize_gif.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.4/PyXAB.egg-info/PKG-INFO` & `PyXAB-0.3.0/PyXAB.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyXAB
-Version: 0.2.4
+Version: 0.3.0
 Summary: PyXAB - A Python Library for X-Armed Bandit and Online Blackbox Optimization Algorithms.
 Home-page: https://github.com/WilliamLwj/PyXAB
 Author: Wenjie Li, Haoze Li, Qifan Song, Jean Honorio
 Author-email: lil3549@purdue.edu
 License: MIT
 Description: 
         
@@ -139,14 +139,15 @@
         | [StoSOO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py)       | [Stochastic Simultaneous Optimistic Optimization](http://proceedings.mlr.press/v28/valko13.pdf)                                                                                          | 2013 |
         | [HCT](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/HCT.py)             | [Online Stochastic Optimization Under Correlated Bandit Feedback](https://proceedings.mlr.press/v32/azar14.html)                                                                         | 2014 |
         | [POO*](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/POO.py)            | [Black-box optimization of noisy functions with unknown smoothness](https://papers.nips.cc/paper/2015/hash/ab817c9349cf9c4f6877e1894a1faa00-Abstract.html)                               | 2015 |
         | [GPO*](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/GPO.py)            | [General Parallel Optimization Without A Metric](https://proceedings.mlr.press/v98/xuedong19a.html)                                                                                      | 2019 |
         | [PCT](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/PCT.py)             | [General Parallel Optimization Without A Metric](https://proceedings.mlr.press/v98/xuedong19a.html)                                                                                      | 2019 |
         | [SequOOL](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/SequOOL.py)     | [A Simple Parameter-free And Adaptive Approach to Optimization Under A Minimal Local Smoothness Assumption](https://arxiv.org/pdf/1810.00997.pdf)                                        | 2019 |
         | [StroquOOL](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StroquOOL.py) | [A Simple Parameter-free And Adaptive Approach to Optimization Under A Minimal Local Smoothness Assumption](https://arxiv.org/pdf/1810.00997.pdf)                                        | 2019 |
+        | [VROOM](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/VROOM.py)         | [Derivative-Free & Order-Robust Optimisation](https://arxiv.org/pdf/1910.04034.pdf)                                                                                                      | 2020 |
         | [VHCT](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/VHCT.py)           | [Optimum-statistical Collaboration Towards General and Efficient Black-box Optimization](https://openreview.net/forum?id=ClIcmwdlxn)                                                     | 2023 |
         | [VPCT](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/VPCT.py)           | N.A. ([GPO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/GPO.py) + [VHCT](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/VHCT.py))                               | N.A. |
         
         
         ### Hierarchical partition 
         
         | Partition                                                                                                             | Description                                                                                                        |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyXAB Version: 0.2.4 Summary: PyXAB - A Python
+Metadata-Version: 2.1 Name: PyXAB Version: 0.3.0 Summary: PyXAB - A Python
 Library for X-Armed Bandit and Online Blackbox Optimization Algorithms. Home-
 page: https://github.com/WilliamLwj/PyXAB Author: Wenjie Li, Haoze Li, Qifan
 Song, Jean Honorio Author-email: lil3549@purdue.edu License: MIT Description: #
 PyXAB - Python *X*-Armed Bandit
 [PyPI_version] [https://codecov.io/gh/WilliamLwj/PyXAB/branch/main/graph/
 badge.svg?token=VACRX9AQBM] [Documentation_Status] [Code_style:_black]
 [testing] [github-PyXAB_forks] [github-PyXAB_stars] [downloads] [github-PyXAB
@@ -81,50 +81,52 @@
 Without A Metric](https://proceedings.mlr.press/v98/xuedong19a.html) | 2019 | |
 [SequOOL](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/SequOOL.py)
 | [A Simple Parameter-free And Adaptive Approach to Optimization Under A
 Minimal Local Smoothness Assumption](https://arxiv.org/pdf/1810.00997.pdf) |
 2019 | | [StroquOOL](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/
 StroquOOL.py) | [A Simple Parameter-free And Adaptive Approach to Optimization
 Under A Minimal Local Smoothness Assumption](https://arxiv.org/pdf/
-1810.00997.pdf) | 2019 | | [VHCT](https://github.com/WilliamLwj/PyXAB/blob/
-main/PyXAB/algos/VHCT.py) | [Optimum-statistical Collaboration Towards General
-and Efficient Black-box Optimization](https://openreview.net/
-forum?id=ClIcmwdlxn) | 2023 | | [VPCT](https://github.com/WilliamLwj/PyXAB/
-blob/main/PyXAB/algos/VPCT.py) | N.A. ([GPO](https://github.com/WilliamLwj/
-PyXAB/blob/main/PyXAB/algos/GPO.py) + [VHCT](https://github.com/WilliamLwj/
-PyXAB/blob/main/PyXAB/algos/VHCT.py)) | N.A. | ### Hierarchical partition |
-Partition | Description | |----------------------------------------------------
--------------------------------------------------------------------|-----------
+1810.00997.pdf) | 2019 | | [VROOM](https://github.com/WilliamLwj/PyXAB/blob/
+main/PyXAB/algos/VROOM.py) | [Derivative-Free & Order-Robust Optimisation]
+(https://arxiv.org/pdf/1910.04034.pdf) | 2020 | | [VHCT](https://github.com/
+WilliamLwj/PyXAB/blob/main/PyXAB/algos/VHCT.py) | [Optimum-statistical
+Collaboration Towards General and Efficient Black-box Optimization](https://
+openreview.net/forum?id=ClIcmwdlxn) | 2023 | | [VPCT](https://github.com/
+WilliamLwj/PyXAB/blob/main/PyXAB/algos/VPCT.py) | N.A. ([GPO](https://
+github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/GPO.py) + [VHCT](https://
+github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/VHCT.py)) | N.A. | ###
+Hierarchical partition | Partition | Description | |---------------------------
 -------------------------------------------------------------------------------
---------------------------| | [BinaryPartition](https://github.com/WilliamLwj/
-PyXAB/blob/main/PyXAB/partition/BinaryPartition.py) | Equal-size binary
-partition of the parameter space, the split dimension is chosen uniform
-randomly | | [RandomBinaryPartition](https://github.com/WilliamLwj/PyXAB/blob/
-main/PyXAB/partition/RandomBinaryPartition.py) | Random-size binary partition
+-------------|-----------------------------------------------------------------
+---------------------------------------------------| | [BinaryPartition](https:
+//github.com/WilliamLwj/PyXAB/blob/main/PyXAB/partition/BinaryPartition.py) |
+Equal-size binary partition of the parameter space, the split dimension is
+chosen uniform randomly | | [RandomBinaryPartition](https://github.com/
+WilliamLwj/PyXAB/blob/main/PyXAB/partition/RandomBinaryPartition.py) | Random-
+size binary partition of the parameter space, the split dimension is chosen
+uniform randomly | | [DimensionBinaryPartition](https://github.com/WilliamLwj/
+PyXAB/blob/main/PyXAB/partition/DimensionBinaryPartition.py) | Equal-size
+partition of the space with a binary split on each dimension, the number of
+children of one node is 2^d | | [KaryPartition](https://github.com/WilliamLwj/
+PyXAB/blob/main/PyXAB/partition/KaryPartition.py) | Equal-size K-ary partition
 of the parameter space, the split dimension is chosen uniform randomly | |
-[DimensionBinaryPartition](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/
-partition/DimensionBinaryPartition.py) | Equal-size partition of the space with
-a binary split on each dimension, the number of children of one node is 2^d | |
-[KaryPartition](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/partition/
-KaryPartition.py) | Equal-size K-ary partition of the parameter space, the
-split dimension is chosen uniform randomly | | [RandomKaryPartition](https://
-github.com/WilliamLwj/PyXAB/blob/main/PyXAB/partition/RandomKaryPartition.py) |
-Random-size K-ary partition of the parameter space, the split dimension is
-chosen uniform randomly | ### Synthetic objectives * Some of these objectives
-can be found [on Wikipedia](https://en.wikipedia.org/wiki/
-Test_functions_for_optimization) | Objectives [Image]| Image | | --- |--- | |
-[Garland](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/synthetic_obj/
-Garland.py) | [Garland] | | [DoubleSine](https://github.com/WilliamLwj/PyXAB/
-blob/main/PyXAB/synthetic_obj/DoubleSine.py) | [DoubleSine] | | [DifficultFunc]
-(https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/synthetic_obj/
-DifficultFunc.py) | [DifficultFunc] | | [Ackley](https://github.com/WilliamLwj/
-PyXAB/blob/main/PyXAB/synthetic_obj/Ackley.py) | [Ackley] | | [Himmelblau]
-(https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/synthetic_obj/
-Himmelblau.py) | [Himmelblau] | | [Rastrigin](https://github.com/WilliamLwj/
-PyXAB/blob/main/PyXAB/synthetic_obj/Rastrigin.py) | [Rastrigin] | ##
+[RandomKaryPartition](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/
+partition/RandomKaryPartition.py) | Random-size K-ary partition of the
+parameter space, the split dimension is chosen uniform randomly | ### Synthetic
+objectives * Some of these objectives can be found [on Wikipedia](https://
+en.wikipedia.org/wiki/Test_functions_for_optimization) | Objectives [Image]|
+Image | | --- |--- | | [Garland](https://github.com/WilliamLwj/PyXAB/blob/main/
+PyXAB/synthetic_obj/Garland.py) | [Garland] | | [DoubleSine](https://
+github.com/WilliamLwj/PyXAB/blob/main/PyXAB/synthetic_obj/DoubleSine.py) |
+[DoubleSine] | | [DifficultFunc](https://github.com/WilliamLwj/PyXAB/blob/main/
+PyXAB/synthetic_obj/DifficultFunc.py) | [DifficultFunc] | | [Ackley](https://
+github.com/WilliamLwj/PyXAB/blob/main/PyXAB/synthetic_obj/Ackley.py) | [Ackley]
+| | [Himmelblau](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/
+synthetic_obj/Himmelblau.py) | [Himmelblau] | | [Rastrigin](https://github.com/
+WilliamLwj/PyXAB/blob/main/PyXAB/synthetic_obj/Rastrigin.py) | [Rastrigin] | ##
 Contributing We appreciate all forms of help and contributions, including but
 not limited to * Star and watch our project * Open an issue for any bugs you
 find or features you want to add to our library * Fork our project and submit a
 pull request with your valuable codes Please read the [contributing
 instructions](https://pyxab.readthedocs.io/en/latest/info/contributing.html)
 before submitting a pull request. ## Citations If you use our package in your
 research or projects, we kindly ask you to cite our work ```text @misc
```

### Comparing `PyXAB-0.2.4/PyXAB.egg-info/SOURCES.txt` & `PyXAB-0.3.0/PyXAB.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 PyXAB/algos/POO.py
 PyXAB/algos/SOO.py
 PyXAB/algos/SequOOL.py
 PyXAB/algos/StoSOO.py
 PyXAB/algos/StroquOOL.py
 PyXAB/algos/VHCT.py
 PyXAB/algos/VPCT.py
+PyXAB/algos/VROOM.py
 PyXAB/algos/Zooming.py
 PyXAB/algos/__init__.py
 PyXAB/partition/BinaryPartition.py
 PyXAB/partition/DimensionBinaryPartition.py
 PyXAB/partition/KaryPartition.py
 PyXAB/partition/Node.py
 PyXAB/partition/Partition.py
```

### Comparing `PyXAB-0.2.4/README.md` & `PyXAB-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,15 @@
 | [StoSOO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py)       | [Stochastic Simultaneous Optimistic Optimization](http://proceedings.mlr.press/v28/valko13.pdf)                                                                                          | 2013 |
 | [HCT](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/HCT.py)             | [Online Stochastic Optimization Under Correlated Bandit Feedback](https://proceedings.mlr.press/v32/azar14.html)                                                                         | 2014 |
 | [POO*](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/POO.py)            | [Black-box optimization of noisy functions with unknown smoothness](https://papers.nips.cc/paper/2015/hash/ab817c9349cf9c4f6877e1894a1faa00-Abstract.html)                               | 2015 |
 | [GPO*](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/GPO.py)            | [General Parallel Optimization Without A Metric](https://proceedings.mlr.press/v98/xuedong19a.html)                                                                                      | 2019 |
 | [PCT](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/PCT.py)             | [General Parallel Optimization Without A Metric](https://proceedings.mlr.press/v98/xuedong19a.html)                                                                                      | 2019 |
 | [SequOOL](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/SequOOL.py)     | [A Simple Parameter-free And Adaptive Approach to Optimization Under A Minimal Local Smoothness Assumption](https://arxiv.org/pdf/1810.00997.pdf)                                        | 2019 |
 | [StroquOOL](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StroquOOL.py) | [A Simple Parameter-free And Adaptive Approach to Optimization Under A Minimal Local Smoothness Assumption](https://arxiv.org/pdf/1810.00997.pdf)                                        | 2019 |
+| [VROOM](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/VROOM.py)         | [Derivative-Free & Order-Robust Optimisation](https://arxiv.org/pdf/1910.04034.pdf)                                                                                                      | 2020 |
 | [VHCT](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/VHCT.py)           | [Optimum-statistical Collaboration Towards General and Efficient Black-box Optimization](https://openreview.net/forum?id=ClIcmwdlxn)                                                     | 2023 |
 | [VPCT](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/VPCT.py)           | N.A. ([GPO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/GPO.py) + [VHCT](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/VHCT.py))                               | N.A. |
 
 
 ### Hierarchical partition 
 
 | Partition                                                                                                             | Description                                                                                                        |
```

#### html2text {}

```diff
@@ -77,50 +77,52 @@
 Without A Metric](https://proceedings.mlr.press/v98/xuedong19a.html) | 2019 | |
 [SequOOL](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/SequOOL.py)
 | [A Simple Parameter-free And Adaptive Approach to Optimization Under A
 Minimal Local Smoothness Assumption](https://arxiv.org/pdf/1810.00997.pdf) |
 2019 | | [StroquOOL](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/
 StroquOOL.py) | [A Simple Parameter-free And Adaptive Approach to Optimization
 Under A Minimal Local Smoothness Assumption](https://arxiv.org/pdf/
-1810.00997.pdf) | 2019 | | [VHCT](https://github.com/WilliamLwj/PyXAB/blob/
-main/PyXAB/algos/VHCT.py) | [Optimum-statistical Collaboration Towards General
-and Efficient Black-box Optimization](https://openreview.net/
-forum?id=ClIcmwdlxn) | 2023 | | [VPCT](https://github.com/WilliamLwj/PyXAB/
-blob/main/PyXAB/algos/VPCT.py) | N.A. ([GPO](https://github.com/WilliamLwj/
-PyXAB/blob/main/PyXAB/algos/GPO.py) + [VHCT](https://github.com/WilliamLwj/
-PyXAB/blob/main/PyXAB/algos/VHCT.py)) | N.A. | ### Hierarchical partition |
-Partition | Description | |----------------------------------------------------
--------------------------------------------------------------------|-----------
+1810.00997.pdf) | 2019 | | [VROOM](https://github.com/WilliamLwj/PyXAB/blob/
+main/PyXAB/algos/VROOM.py) | [Derivative-Free & Order-Robust Optimisation]
+(https://arxiv.org/pdf/1910.04034.pdf) | 2020 | | [VHCT](https://github.com/
+WilliamLwj/PyXAB/blob/main/PyXAB/algos/VHCT.py) | [Optimum-statistical
+Collaboration Towards General and Efficient Black-box Optimization](https://
+openreview.net/forum?id=ClIcmwdlxn) | 2023 | | [VPCT](https://github.com/
+WilliamLwj/PyXAB/blob/main/PyXAB/algos/VPCT.py) | N.A. ([GPO](https://
+github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/GPO.py) + [VHCT](https://
+github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/VHCT.py)) | N.A. | ###
+Hierarchical partition | Partition | Description | |---------------------------
 -------------------------------------------------------------------------------
---------------------------| | [BinaryPartition](https://github.com/WilliamLwj/
-PyXAB/blob/main/PyXAB/partition/BinaryPartition.py) | Equal-size binary
-partition of the parameter space, the split dimension is chosen uniform
-randomly | | [RandomBinaryPartition](https://github.com/WilliamLwj/PyXAB/blob/
-main/PyXAB/partition/RandomBinaryPartition.py) | Random-size binary partition
+-------------|-----------------------------------------------------------------
+---------------------------------------------------| | [BinaryPartition](https:
+//github.com/WilliamLwj/PyXAB/blob/main/PyXAB/partition/BinaryPartition.py) |
+Equal-size binary partition of the parameter space, the split dimension is
+chosen uniform randomly | | [RandomBinaryPartition](https://github.com/
+WilliamLwj/PyXAB/blob/main/PyXAB/partition/RandomBinaryPartition.py) | Random-
+size binary partition of the parameter space, the split dimension is chosen
+uniform randomly | | [DimensionBinaryPartition](https://github.com/WilliamLwj/
+PyXAB/blob/main/PyXAB/partition/DimensionBinaryPartition.py) | Equal-size
+partition of the space with a binary split on each dimension, the number of
+children of one node is 2^d | | [KaryPartition](https://github.com/WilliamLwj/
+PyXAB/blob/main/PyXAB/partition/KaryPartition.py) | Equal-size K-ary partition
 of the parameter space, the split dimension is chosen uniform randomly | |
-[DimensionBinaryPartition](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/
-partition/DimensionBinaryPartition.py) | Equal-size partition of the space with
-a binary split on each dimension, the number of children of one node is 2^d | |
-[KaryPartition](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/partition/
-KaryPartition.py) | Equal-size K-ary partition of the parameter space, the
-split dimension is chosen uniform randomly | | [RandomKaryPartition](https://
-github.com/WilliamLwj/PyXAB/blob/main/PyXAB/partition/RandomKaryPartition.py) |
-Random-size K-ary partition of the parameter space, the split dimension is
-chosen uniform randomly | ### Synthetic objectives * Some of these objectives
-can be found [on Wikipedia](https://en.wikipedia.org/wiki/
-Test_functions_for_optimization) | Objectives [Image]| Image | | --- |--- | |
-[Garland](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/synthetic_obj/
-Garland.py) | [Garland] | | [DoubleSine](https://github.com/WilliamLwj/PyXAB/
-blob/main/PyXAB/synthetic_obj/DoubleSine.py) | [DoubleSine] | | [DifficultFunc]
-(https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/synthetic_obj/
-DifficultFunc.py) | [DifficultFunc] | | [Ackley](https://github.com/WilliamLwj/
-PyXAB/blob/main/PyXAB/synthetic_obj/Ackley.py) | [Ackley] | | [Himmelblau]
-(https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/synthetic_obj/
-Himmelblau.py) | [Himmelblau] | | [Rastrigin](https://github.com/WilliamLwj/
-PyXAB/blob/main/PyXAB/synthetic_obj/Rastrigin.py) | [Rastrigin] | ##
+[RandomKaryPartition](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/
+partition/RandomKaryPartition.py) | Random-size K-ary partition of the
+parameter space, the split dimension is chosen uniform randomly | ### Synthetic
+objectives * Some of these objectives can be found [on Wikipedia](https://
+en.wikipedia.org/wiki/Test_functions_for_optimization) | Objectives [Image]|
+Image | | --- |--- | | [Garland](https://github.com/WilliamLwj/PyXAB/blob/main/
+PyXAB/synthetic_obj/Garland.py) | [Garland] | | [DoubleSine](https://
+github.com/WilliamLwj/PyXAB/blob/main/PyXAB/synthetic_obj/DoubleSine.py) |
+[DoubleSine] | | [DifficultFunc](https://github.com/WilliamLwj/PyXAB/blob/main/
+PyXAB/synthetic_obj/DifficultFunc.py) | [DifficultFunc] | | [Ackley](https://
+github.com/WilliamLwj/PyXAB/blob/main/PyXAB/synthetic_obj/Ackley.py) | [Ackley]
+| | [Himmelblau](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/
+synthetic_obj/Himmelblau.py) | [Himmelblau] | | [Rastrigin](https://github.com/
+WilliamLwj/PyXAB/blob/main/PyXAB/synthetic_obj/Rastrigin.py) | [Rastrigin] | ##
 Contributing We appreciate all forms of help and contributions, including but
 not limited to * Star and watch our project * Open an issue for any bugs you
 find or features you want to add to our library * Fork our project and submit a
 pull request with your valuable codes Please read the [contributing
 instructions](https://pyxab.readthedocs.io/en/latest/info/contributing.html)
 before submitting a pull request. ## Citations If you use our package in your
 research or projects, we kindly ask you to cite our work ```text @misc
```

### Comparing `PyXAB-0.2.4/setup.py` & `PyXAB-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'PyXAB'
 DESCRIPTION = 'PyXAB - A Python Library for X-Armed Bandit and Online Blackbox Optimization Algorithms.'
 URL = 'https://github.com/WilliamLwj/PyXAB'
 EMAIL = 'lil3549@purdue.edu'
 AUTHOR = 'Wenjie Li, Haoze Li, Qifan Song, Jean Honorio'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.2.4'
+VERSION = '0.3.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'numpy>=1.20.3',
     'matplotlib',
     # 'requests', 'maya', 'records',
 ]
```

