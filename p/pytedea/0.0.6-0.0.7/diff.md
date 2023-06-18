# Comparing `tmp/pytedea-0.0.6.tar.gz` & `tmp/pytedea-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytedea-0.0.6.tar", last modified: Thu May 11 14:40:13 2023, max compression
+gzip compressed data, was "pytedea-0.0.7.tar", last modified: Sun Jun 18 12:06:52 2023, max compression
```

## Comparing `pytedea-0.0.6.tar` & `pytedea-0.0.7.tar`

### file list

```diff
@@ -1,94 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:40:13.451293 pytedea-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-11 14:39:57.000000 pytedea-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-11 14:39:57.000000 pytedea-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-11 14:40:13.451293 pytedea-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-11 14:39:57.000000 pytedea-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:40:13.443293 pytedea-0.0.6/pytedea/
--rw-r--r--   0 runner    (1001) docker     (123)    13582 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/CNLS.py
--rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/CNLSDDF.py
--rw-r--r--   0 runner    (1001) docker     (123)    13797 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/DDF.py
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/DDFt.py
--rw-r--r--   0 runner    (1001) docker     (123)    23722 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/DEA.py
--rw-r--r--   0 runner    (1001) docker     (123)   138957 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/DEAt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/HYPER.py
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/HYPERt.py
--rw-r--r--   0 runner    (1001) docker     (123)    59916 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/MB.py
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/MQDDF.py
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/MQDDFt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/MQDEA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/MQDEAt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/MQNDDF.py
--rw-r--r--   0 runner    (1001) docker     (123)    17367 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/NDDF.py
--rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/StoNED.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/pytedea.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:40:13.451293 pytedea-0.0.6/pytedea/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/CNLSDDFG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/CNLSDDFG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/CNLSDDFZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/CNLSDDFZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/CNLSG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/CNLSG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/CNLSZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/CNLSZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/CQERDDFG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/CQERDDFG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    16178 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/CQERDDFZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/CQERDDFZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/CQERG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/CQERG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13749 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/CQERZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/CQERZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    53114 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/MB_.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/sweet.py
--rw-r--r--   0 runner    (1001) docker     (123)    36941 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCNLSDDFG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCNLSDDFG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18293 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCNLSDDFZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCNLSDDFZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCNLSG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCNLSG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15035 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCNLSZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCNLSZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCNLSbG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCNLSbG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCNLSbZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCNLSbZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCNLSxG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCNLSxG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCNLSxZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCNLSxZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCQERDDFG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCQERDDFG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15268 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCQERDDFZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCQERDDFZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCQERG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCQERG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCQERZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9714 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCQERZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCQERbG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCQERbG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14301 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCQERbZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCQERbZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCQERxG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCQERxG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14227 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCQERxZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/utils/weakCQERxZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/weakCNLSDDF.py
--rw-r--r--   0 runner    (1001) docker     (123)    19540 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/weakCNLSNDDF.py
--rw-r--r--   0 runner    (1001) docker     (123)    20648 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/weakCNLSb.py
--rw-r--r--   0 runner    (1001) docker     (123)    19573 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/weakCNLSx.py
--rw-r--r--   0 runner    (1001) docker     (123)    19443 2023-05-11 14:39:57.000000 pytedea-0.0.6/pytedea/weakCNLSy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:40:13.443293 pytedea-0.0.6/pytedea.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-11 14:40:13.000000 pytedea-0.0.6/pytedea.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-11 14:40:13.000000 pytedea-0.0.6/pytedea.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 14:40:13.000000 pytedea-0.0.6/pytedea.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:40:13.000000 pytedea-0.0.6/pytedea.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-11 14:40:13.000000 pytedea-0.0.6/pytedea.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 14:40:13.000000 pytedea-0.0.6/pytedea.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-11 14:39:57.000000 pytedea-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-11 14:40:13.451293 pytedea-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-11 14:39:57.000000 pytedea-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:06:52.199868 pytedea-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-18 12:06:43.000000 pytedea-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-18 12:06:43.000000 pytedea-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-18 12:06:52.199868 pytedea-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-18 12:06:43.000000 pytedea-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:06:52.191868 pytedea-0.0.7/pytedea/
+-rw-r--r--   0 runner    (1001) docker     (123)    13582 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/CNLS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12068 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/CNLSDDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13797 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/DDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/DDFDUAL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/DDFt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23722 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/DEA.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138957 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/DEAt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/HYPER.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/HYPERt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59916 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/MB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/MQDDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/MQDDFt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/MQDEA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/MQDEAt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/MQNDDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17367 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/NDDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/NDDFDUAL.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13425 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/StoNED.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/pytedea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:06:52.199868 pytedea-0.0.7/pytedea/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/CNLSDDFG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/CNLSDDFG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/CNLSDDFZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/CNLSDDFZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/CNLSG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/CNLSG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/CNLSZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/CNLSZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/CQERDDFG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/CQERDDFG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16178 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/CQERDDFZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/CQERDDFZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/CQERG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/CQERG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13749 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/CQERZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/CQERZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53114 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/MB_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/sweet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36941 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCNLSDDFG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCNLSDDFG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18293 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCNLSDDFZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCNLSDDFZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCNLSG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCNLSG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15035 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCNLSZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCNLSZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCNLSbG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCNLSbG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCNLSbZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCNLSbZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCNLSxG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCNLSxG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCNLSxZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCNLSxZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCQERDDFG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCQERDDFG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15268 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCQERDDFZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCQERDDFZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCQERG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCQERG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCQERZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9714 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCQERZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCQERbG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCQERbG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14301 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCQERbZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCQERbZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCQERxG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCQERxG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14227 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCQERxZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/utils/weakCQERxZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18454 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/weakCNLSDDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/weakCNLSNDDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19551 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/weakCNLSNDDF_notransfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20722 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/weakCNLSb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19573 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/weakCNLSx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19443 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/weakCNLSy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18691 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/weakMetaCNLSDDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22174 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/weakMetaCNLSNDDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21054 2023-06-18 12:06:43.000000 pytedea-0.0.7/pytedea/weakMetaCNLSb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:06:52.191868 pytedea-0.0.7/pytedea.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-18 12:06:52.000000 pytedea-0.0.7/pytedea.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-18 12:06:52.000000 pytedea-0.0.7/pytedea.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-18 12:06:52.000000 pytedea-0.0.7/pytedea.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 12:06:52.000000 pytedea-0.0.7/pytedea.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-18 12:06:52.000000 pytedea-0.0.7/pytedea.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 12:06:52.000000 pytedea-0.0.7/pytedea.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-18 12:06:43.000000 pytedea-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-18 12:06:52.199868 pytedea-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-18 12:06:43.000000 pytedea-0.0.7/setup.py
```

### Comparing `pytedea-0.0.6/LICENSE` & `pytedea-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/PKG-INFO` & `pytedea-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytedea
-Version: 0.0.6
+Version: 0.0.7
 Summary: Data envelopment analysis using Python.
 Home-page: https://github.com/advancehs/pytedea
 Author: advancehs
 Author-email: 1019753743@qq.com
 License: GNU General Public License v3
 Keywords: pytedea
 Classifier: Intended Audience :: Developers
```

### Comparing `pytedea-0.0.6/pytedea/CNLS.py` & `pytedea-0.0.7/pytedea/CNLS.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,37 +105,37 @@
             if self.rts == RTS_VRS:
                 if type(self.z) != type(None):
                     def regression_rule(model, i):
                         return np.array((self.y.loc[i,])) \
                             == model.alpha[i] \
                                 + sum(model.beta[i, k] * self.x.loc[i,self.xcol[k]] for k in model.K) \
                                 - sum(model.lamda[m] * self.z.loc[i,self.zcol[m]] for m in model.M) \
-                                - model.epsilon[i]
+                                + model.epsilon[i]
                     return regression_rule
 
 
                 def regression_rule(model, i):
                     return np.array((self.y.loc[i,]))   == model.alpha[i] \
                         + sum(model.beta[i, k] * self.x.loc[i,self.xcol[k]] for k in model.K) \
-                        - model.epsilon[i]
+                        + model.epsilon[i]
                 return regression_rule
 
             elif self.rts == RTS_CRS:
                 if type(self.z) != type(None):
                     def regression_rule(model, i):
                         return np.array((self.y.loc[i,]))   == \
                                 sum(model.beta[i, k] * self.x.loc[i,self.xcol[k]] for k in model.K) \
                                 - sum(model.lamda[m] * self.z.loc[i,self.zcol[m]] for m in model.M) \
-                                - model.epsilon[i]
+                                + model.epsilon[i]
                     return regression_rule
 
                 def regression_rule(model, i):
                     return np.array((self.y.loc[i,])) == \
                         sum(model.beta[i, k] * self.x.loc[i,self.xcol[k]] for k in model.K) \
-                        - model.epsilon[i]
+                        + model.epsilon[i]
                 return regression_rule
 
         elif self.cet == CET_MULT:
             if type(self.z) != type(None):
                 def regression_rule(model, i):
                     return log(np.array(self.y.loc[i,:]) ) == log(model.frontier[i] + 1) \
                             - sum(model.lamda[m] * self.z.loc[i,self.zcol[m]] for m in model.M) \
```

### Comparing `pytedea-0.0.6/pytedea/CNLSDDF.py` & `pytedea-0.0.7/pytedea/CNLSDDF.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,37 +9,64 @@
 from .utils import tools
 
 
 class CNLSDDF(CNLS.CNLS):
     """Convex Nonparametric Least Square with directional distance function
     """
 
-    def __init__(self, data,sent = "inputvar=outputvar:unoutputvar",z=None, gy=[1], gx=[1], gb=None, \
+    def __init__(self, data,sent = "inputvar=outputvar:unoutputvar",z=None, gy=[1], gx=[1],deduce="Y",  \
                  fun=FUN_PROD, rts=RTS_VRS, baseindex=None,refindex=None):
         """CNLS DDF model
 
         Args:
             data (pandas.DataFrame): input pandas.
-            sent (str): inputvars=outputvars: unoutputvars. e.g.: "K L CO2= Y"
+            sent (string): inputvars=outputvars: unoutputvars. e.g.: "K L CO2= Y"
             z (float, optional): Contextual variable(s). Defaults to None.
             gy (list, optional): output directional vector. Defaults to [1].
             gx (list, optional): input directional vector. Defaults to [1].
-            gb (list, optional): undesirable output directional vector. Defaults to None.
+            deduce(string,optional): deduce the value of the variable / directional vector of the variable \
+                                         form the value of all the varibles.Defaults to minus Y/gy .
             fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
             rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
         """
 
         self.outputvars, self.inputvars,  self.zvars, self.gy, self.gx,  \
             = tools.assert_valid_CNLSDDF(sent, gy, gx, z)
         self.y, self.x,  self.z, self.yref, self.xref,  self.zref,self.referenceflag\
             = tools.assert_valid_CNLS2(baseindex, refindex, data, \
                                        self.outputvars, self.inputvars,  self.zvars)
         self.xcol = self.x.columns
         self.ycol = self.y.columns
         self.zcol = self.z.columns if type(z) != type(None) else None
+
+        self.decuce = deduce
+        if deduce in self.xcol:
+            tomunus_col=self.x[[deduce]]
+            tomunus_index = list(self.xcol).index(deduce)
+            tomunus_g = self.gx[tomunus_index]
+            self.actrual_value = tomunus_col / tomunus_g
+            if tomunus_g==0:
+                raise ValueError("The directional vector of the variable you want to minus must not be 0.")
+        elif deduce in self.ycol:
+            tomunus_col=self.y[[deduce]]
+            tomunus_index = list(self.ycol).index(deduce)
+            tomunus_g = self.gy[tomunus_index]
+            self.actrual_value = tomunus_col / tomunus_g
+            if tomunus_g==0:
+                raise ValueError("The directional vector of the variable you want to minus must not be 0.")
+        else:
+            raise ValueError("deduce must be selected in your variables")
+        self.y = pd.DataFrame(self.y.to_numpy() -\
+                      self.actrual_value.to_numpy() * np.array(self.gy),columns=self.y.columns,index=self.y.index)
+        self.x = pd.DataFrame(self.x.to_numpy() -\
+                      self.actrual_value.to_numpy() * np.array(self.gx),columns=self.x.columns,index=self.x.index)
+
+
+        print("actrual_value is:",self.actrual_value)
+
         print("xcol,ycol are:",self.x.columns,self.y.columns)
 
         print("gx,gy are:",self.gx,self.gy)
         print("aaa",self.y,self.x)
         self.fun = fun
         self.rts = rts
 
@@ -98,45 +125,48 @@
             self.__model__, email, CET_ADDI, solver)
 
     def __regression_rule(self):
         """Return the proper regression constraint"""
         if self.rts == RTS_VRS:
             if type(self.z) != type(None):
                 def regression_rule(model, i):
-                    return sum(model.gamma[i, l] * self.y.loc[i, self.ycol[l]] for l in model.L) \
+                    return self.actrual_value.loc[i,self.decuce]\
                         == model.alpha[i] \
                         + sum(model.beta[i, k] * self.x.loc[i, self.xcol[k]] for k in model.K) \
+                        - sum(model.gamma[i, l] * self.y.loc[i, self.ycol[l]] for l in model.L)\
                         - sum(model.lamda[m] * self.z.loc[i, self.zcol[m]] for m in model.M) \
                         - model.epsilon[i]
 
                 return regression_rule
 
             def regression_rule(model, i):
-                return sum(model.gamma[i, l] * self.y.loc[i, self.ycol[l]] for l in model.L) \
+                return self.actrual_value.loc[i,self.decuce] \
                     == model.alpha[i] \
                     + sum(model.beta[i, k] * self.x.loc[i, self.xcol[k]] for k in model.K) \
+                    - sum(model.gamma[i, l] * self.y.loc[i, self.ycol[l]] for l in model.L) \
                     - model.epsilon[i]
 
             return regression_rule
 
         elif self.rts == RTS_CRS:
             if type(self.z) != type(None):
                 def regression_rule(model, i):
-                    return sum(model.gamma[i, l] * self.y.loc[i, self.ycol[l]] for l in model.L) \
+                    return self.actrual_value.loc[i,self.decuce] \
                         == sum(model.beta[i, k] * self.x.loc[i, self.xcol[k]] for k in model.K) \
+                        - sum(model.gamma[i, l] * self.y.loc[i, self.ycol[l]] for l in model.L) \
                         - sum(model.lamda[m] * self.z.loc[i, self.zcol[m]] for m in model.M) \
                         - model.epsilon[i]
 
                 return regression_rule
 
             def regression_rule(model, i):
-                return sum(model.gamma[i, l] * self.y.loc[i, self.ycol[l]] for l in model.L) \
+                return self.actrual_value.loc[i,self.decuce] \
                     == sum(model.beta[i, k] * self.x.loc[i, self.xcol[k]] for k in model.K) \
+                    - sum(model.gamma[i, l] * self.y.loc[i, self.ycol[l]] for l in model.L) \
                     - model.epsilon[i]
-
             return regression_rule
 
         raise ValueError("Undefined model parameters.")
 
     def __translation_property(self):
         """Return the proper translation property"""
```

### Comparing `pytedea-0.0.6/pytedea/DDF.py` & `pytedea-0.0.7/pytedea/DDF.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/DDFt.py` & `pytedea-0.0.7/pytedea/DDFt.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/DEA.py` & `pytedea-0.0.7/pytedea/DEA.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/DEAt.py` & `pytedea-0.0.7/pytedea/DEAt.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/HYPER.py` & `pytedea-0.0.7/pytedea/HYPER.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/HYPERt.py` & `pytedea-0.0.7/pytedea/HYPERt.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/MB.py` & `pytedea-0.0.7/pytedea/MB.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/MQDDF.py` & `pytedea-0.0.7/pytedea/MQDDF.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/MQDDFt.py` & `pytedea-0.0.7/pytedea/MQDDFt.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/MQDEA.py` & `pytedea-0.0.7/pytedea/MQDEA.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/MQDEAt.py` & `pytedea-0.0.7/pytedea/MQDEAt.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/MQNDDF.py` & `pytedea-0.0.7/pytedea/MQNDDF.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/NDDF.py` & `pytedea-0.0.7/pytedea/NDDF.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/StoNED.py` & `pytedea-0.0.7/pytedea/StoNED.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,28 +14,31 @@
 
     def __init__(self, model):
         """StoNED
         model: The input model for residual decomposition
         """
         self.model = model
         self.x = model.x
-        if self.model.__class__.__name__ == "weakCNLSb":
-            print("kind1 weakCNLSb")
-            self.y = self.model.b.iloc[:,0].values
-        elif self.model.__class__.__name__ == "weakCNLSx":
-            print("kind2 weakCNLSx")
-            self.y = self.model.x.iloc[:,0].values
+
         # If the model is a directional distance based, set cet to CET_ADDI
-        elif hasattr(self.model, 'get_gamma2'):
-            print("kind3 has get_gamma2")
+        if hasattr(self.model, 'gx'):
+            print("kind1 cnlsddf model")
             self.model.cet = CET_ADDI
-            self.y = np.diag(np.tensordot(
-                self.model.y, self.model.get_gamma2(), axes=([1], [1])))
+            if model.__class__.__name__ == "weakCNLSNDDF_notransfer":
+                self.y = np.diag(np.tensordot(
+                    self.model.y, self.model.get_gamma2(), axes=([1], [1])))
+            else:
+                self.y = model.actrual_value.iloc[:, 0].values
+
+        elif model.__class__.__name__ == "weakCNLSb":
+            self.y = 1/self.model.b.iloc[:,0].values
+        elif model.__class__.__name__ == "weakMetaCNLSb":
+            self.y = 1/self.model.GCE_C.iloc[:,0].values
         else:
-            print("kind4 has not get_gamma2")
+            print("kind2 cnls model")
             self.y = self.model.y.iloc[:,0].values
 
     def get_unconditional_expected_inefficiency(self, method=RED_MOM):
         """
         Args:
             method (String, optional): RED_MOM (Method of moments) or RED_QLE (Quassi-likelihood estimation) or RED_KDE (Kernel deconvolution estimation). Defaults to RED_MOM.
         """
@@ -57,52 +60,98 @@
             method (String, optional): RED_MOM (Method of moments) or RED_QLE (Quassi-likelihood estimation). Defaults to RED_MOM.
 
         calculate sigma_u, sigma_v, mu, and epsilon value
         """
         tools.assert_optimized(self.model.optimization_status)
         self.get_unconditional_expected_inefficiency(method)
         sigmas = self.sigma_u * self.sigma_v / math.sqrt(self.sigma_u ** 2 + self.sigma_v ** 2)
-        mus = (self.mu * (self.sigma_v**2)-self.residual * (self.sigma_u**2)) / (self.sigma_u ** 2 + self.sigma_v ** 2)
+        mus = (self.mu * (self.sigma_v**2)-self.epsilon2 * (self.sigma_u**2)) / (self.sigma_u ** 2 + self.sigma_v ** 2)
         if self.model.fun == FUN_PROD:
             jlms = sigmas * (stats.norm.pdf(mus / sigmas)) / (stats.norm.cdf(mus / sigmas)) + mus
             if self.model.cet == CET_ADDI:
-                print("haha",jlms,self.y)
-                return pd.Series(jlms / self.y,index=self.model.get_residual().index)
+                print("jlms",jlms,self.y)
+                return pd.Series(jlms / (self.y + jlms)  ,index=self.model.get_residual().index)
             elif self.model.cet == CET_MULT:
+                print("jlms",jlms,self.y)
+
+                # bc = np.exp(-mus + 0.5 * (sigmas) ** 2) * (stats.norm.cdf((mus / sigmas) - sigmas) / stats.norm.cdf(mus / sigmas))
+                # print("bc",bc)
+                # return pd.Series(1-bc,index=self.model.get_residual().index)
                 return pd.Series(1-np.exp(-jlms),index=self.model.get_residual().index)
 
         elif self.model.fun == FUN_COST:
             jlms = sigmas * (stats.norm.pdf(-mus / sigmas)) / (stats.norm.cdf(-mus / sigmas)) - mus
             if self.model.cet == CET_ADDI:
                 return pd.Series(-jlms / self.y,index=self.model.get_residual().index)
             elif self.model.cet == CET_MULT:
                 return pd.Series(1-np.exp(jlms),index=self.model.get_residual().index)
 
         raise ValueError("Undefined model parameters.")
 
-    def get_technical_efficiency(self, method=RED_MOM):
+    def get_inefficiency(self, method=RED_MOM): ## E(u_i|epsilon_i)
         """
         Args:
             method (String, optional): RED_MOM (Method of moments) or RED_QLE (Quassi-likelihood estimation). Defaults to RED_MOM.
 
         calculate sigma_u, sigma_v, mu, and epsilon value
         """
         tools.assert_optimized(self.model.optimization_status)
         self.get_unconditional_expected_inefficiency(method)
         sigmas = self.sigma_u * self.sigma_v / math.sqrt(self.sigma_u ** 2 + self.sigma_v ** 2)
-        mus = (self.mu* (self.sigma_v ** 2) -self.residual * (self.sigma_u ** 2) )/ (self.sigma_u ** 2 + self.sigma_v ** 2)
+        mus = (self.mu * (self.sigma_v**2)-self.epsilon2 * (self.sigma_u**2)) / (self.sigma_u ** 2 + self.sigma_v ** 2)
+        if self.model.fun == FUN_PROD:
+            jlms = sigmas * (stats.norm.pdf(mus / sigmas)) / (stats.norm.cdf(mus / sigmas)) + mus
+            return pd.Series(jlms, index=self.model.get_residual().index)
+        elif self.model.fun == FUN_COST:
+            jlms = sigmas * (stats.norm.pdf(-mus / sigmas)) / (stats.norm.cdf(-mus / sigmas)) - mus
+            return pd.Series(jlms, index=self.model.get_residual().index)
+        raise ValueError("Undefined model parameters.")
+
 
 
-        bc = np.exp(-mus + 0.5 * (sigmas) ** 2) * (stats.norm.cdf((mus / sigmas) - sigmas) / stats.norm.cdf(mus / sigmas))
+    def get_technical_efficiency(self, method=RED_MOM):
+        """
+        Args:
+            method (String, optional): RED_MOM (Method of moments) or RED_QLE (Quassi-likelihood estimation). Defaults to RED_MOM.
+
+        calculate sigma_u, sigma_v, mu, and epsilon value
+        """
+        tools.assert_optimized(self.model.optimization_status)
+        self.get_unconditional_expected_inefficiency(method)
+        sigmas = self.sigma_u * self.sigma_v / math.sqrt(self.sigma_u ** 2 + self.sigma_v ** 2)
+        mus = (self.mu * (self.sigma_v**2)-self.residual * (self.sigma_u**2)) / (self.sigma_u ** 2 + self.sigma_v ** 2)
         if self.model.fun == FUN_PROD:
-            # return bc
-            return pd.Series(bc,index=self.model.get_residual().index)
+            if self.model.cet == CET_ADDI:
+                jlms = sigmas * (stats.norm.pdf(mus / sigmas)) / (stats.norm.cdf(mus / sigmas)) + mus
+
+                print("haha",jlms,self.y)
+                return pd.Series(self.y / (self.y+jlms),index=self.model.get_residual().index)
+            elif self.model.cet == CET_MULT:
+                # bc = np.exp(-mus + 0.5 * (sigmas) ** 2) * (stats.norm.cdf((mus / sigmas) - sigmas) / stats.norm.cdf(mus / sigmas))
+                jlms = sigmas * (stats.norm.pdf(mus / sigmas)) / (stats.norm.cdf(mus / sigmas)) + mus
+
+                print("haha",jlms,self.y)
+                # print("haha",bc,self.y)
+
+                # bc = np.exp(-mus + 0.5 * (sigmas) ** 2) * (stats.norm.cdf((mus / sigmas) - sigmas) / stats.norm.cdf(mus / sigmas))
+                # return pd.Series(self.y / (self.y * np.exp(jlms)-1),index=self.model.get_residual().index) # 负的
+                return pd.Series(np.exp(-jlms),index=self.model.get_residual().index)
+                # return pd.Series(bc,index=self.model.get_residual().index)
+
+        elif self.model.fun == FUN_COST:
+            jlms = sigmas * (stats.norm.pdf(-mus / sigmas)) / (stats.norm.cdf(-mus / sigmas)) - mus
+            if self.model.cet == CET_ADDI:
+                return pd.Series( self.y/ (self.y-jlms),index=self.model.get_residual().index)
+            elif self.model.cet == CET_MULT:
+                return pd.Series(np.exp(jlms),index=self.model.get_residual().index)
 
         raise ValueError("Undefined model parameters.")
 
+        # bc = np.exp(-mus + 0.5 * (sigmas) ** 2) * (stats.norm.cdf((mus / sigmas) - sigmas) / stats.norm.cdf(mus / sigmas))
+
     def __method_of_moment(self, residual):
         """Method of moment"""
         M2 = (residual - np.mean(residual)) ** 2
         M3 = (residual - np.mean(residual)) ** 3
 
         M2_mean = np.mean(M2, axis=0)
         M3_mean = np.mean(M3, axis=0)
@@ -121,17 +170,17 @@
 
         else:
             raise ValueError("Undefined model parameters.")
 
         self.sigma_v = (M2_mean - ((math.pi - 2) / math.pi) * self.sigma_u ** 2) ** (1 / 2)
         self.mu = (self.sigma_u ** 2 * 2 / math.pi) ** (1 / 2)
         if self.model.fun == FUN_PROD:
-            self.epsilon = residual - self.mu
+            self.epsilon2 = residual - self.mu
         else:
-            self.epsilon = residual + self.mu
+            self.epsilon2 = residual + self.mu
 
     def __quassi_likelihood(self, residual):
         def __quassi_likelihood_estimation(lamda, eps):
             """ This function computes the negative of the log likelihood function
             given parameter (lambda) and residual (eps).
 
             Args:
@@ -179,17 +228,17 @@
         self.mu = math.sqrt(2) * sigma * lamda / math.sqrt(math.pi *(1 + lamda ** 2))
 
         # calculate sigma.u and sigma.v
         self.sigma_v = (sigma ** 2 / (1 + lamda ** 2)) ** (1 / 2)
         self.sigma_u = self.sigma_v * lamda
 
         if self.model.fun == FUN_PROD:
-            self.epsilon = residual - self.mu
+            self.epsilon2 = residual - self.mu
         elif self.model.fun == FUN_COST:
-            self.epsilon = residual + self.mu
+            self.epsilon2 = residual + self.mu
         self.residual = residual
     def __gaussian_kernel_estimation(self, residual):
         def __gaussian_kernel_estimator(g):
             """Gaussian kernel estimator"""
             return (1 / math.sqrt(2 * math.pi)) * np.exp(-0.5 * g ** 2)
 
         x = np.array(residual)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytedea-0.0.6/pytedea/__init__.py` & `pytedea-0.0.7/pytedea/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __author__ = """advancehs"""
 __email__ = '1019753743@qq.com'
-__version__ = '0.0.6'
+__version__ = '0.0.7'
 
 from . import DEAt
 from . import DDFt
 from . import DEA
 from . import DDF
 from . import HYPER
 # from . import CQER
```

### Comparing `pytedea-0.0.6/pytedea/constant.py` & `pytedea-0.0.7/pytedea/constant.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/CNLSDDFG1.py` & `pytedea-0.0.7/pytedea/utils/CNLSDDFG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/CNLSDDFG2.py` & `pytedea-0.0.7/pytedea/utils/CNLSDDFG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/CNLSDDFZG1.py` & `pytedea-0.0.7/pytedea/utils/CNLSDDFZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/CNLSDDFZG2.py` & `pytedea-0.0.7/pytedea/utils/CNLSDDFZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/CNLSG1.py` & `pytedea-0.0.7/pytedea/utils/CNLSG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/CNLSG2.py` & `pytedea-0.0.7/pytedea/utils/CNLSG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/CNLSZG1.py` & `pytedea-0.0.7/pytedea/utils/CNLSZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/CNLSZG2.py` & `pytedea-0.0.7/pytedea/utils/CNLSZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/CQERDDFG1.py` & `pytedea-0.0.7/pytedea/utils/CQERDDFG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/CQERDDFG2.py` & `pytedea-0.0.7/pytedea/utils/CQERDDFG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/CQERDDFZG1.py` & `pytedea-0.0.7/pytedea/utils/CQERDDFZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/CQERDDFZG2.py` & `pytedea-0.0.7/pytedea/utils/CQERDDFZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/CQERG1.py` & `pytedea-0.0.7/pytedea/utils/CQERG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/CQERG2.py` & `pytedea-0.0.7/pytedea/utils/CQERG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/CQERZG1.py` & `pytedea-0.0.7/pytedea/utils/CQERZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/CQERZG2.py` & `pytedea-0.0.7/pytedea/utils/CQERZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/MB_.py` & `pytedea-0.0.7/pytedea/utils/MB_.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/interpolation.py` & `pytedea-0.0.7/pytedea/utils/interpolation.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/sweet.py` & `pytedea-0.0.7/pytedea/utils/sweet.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/tools.py` & `pytedea-0.0.7/pytedea/utils/tools.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCNLSDDFG1.py` & `pytedea-0.0.7/pytedea/utils/weakCNLSDDFG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCNLSDDFG2.py` & `pytedea-0.0.7/pytedea/utils/weakCNLSDDFG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCNLSDDFZG1.py` & `pytedea-0.0.7/pytedea/utils/weakCNLSDDFZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCNLSDDFZG2.py` & `pytedea-0.0.7/pytedea/utils/weakCNLSDDFZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCNLSG1.py` & `pytedea-0.0.7/pytedea/utils/weakCNLSG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCNLSG2.py` & `pytedea-0.0.7/pytedea/utils/weakCNLSG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCNLSZG1.py` & `pytedea-0.0.7/pytedea/utils/weakCNLSZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCNLSZG2.py` & `pytedea-0.0.7/pytedea/utils/weakCNLSZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCNLSbG1.py` & `pytedea-0.0.7/pytedea/utils/weakCNLSbG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCNLSbG2.py` & `pytedea-0.0.7/pytedea/utils/weakCNLSbG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCNLSbZG1.py` & `pytedea-0.0.7/pytedea/utils/weakCNLSbZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCNLSbZG2.py` & `pytedea-0.0.7/pytedea/utils/weakCNLSbZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCNLSxG1.py` & `pytedea-0.0.7/pytedea/utils/weakCNLSxG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCNLSxG2.py` & `pytedea-0.0.7/pytedea/utils/weakCNLSxG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCNLSxZG1.py` & `pytedea-0.0.7/pytedea/utils/weakCNLSxZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCNLSxZG2.py` & `pytedea-0.0.7/pytedea/utils/weakCNLSxZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCQERDDFG1.py` & `pytedea-0.0.7/pytedea/utils/weakCQERDDFG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCQERDDFG2.py` & `pytedea-0.0.7/pytedea/utils/weakCQERDDFG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCQERDDFZG1.py` & `pytedea-0.0.7/pytedea/utils/weakCQERDDFZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCQERDDFZG2.py` & `pytedea-0.0.7/pytedea/utils/weakCQERDDFZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCQERG1.py` & `pytedea-0.0.7/pytedea/utils/weakCQERG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCQERG2.py` & `pytedea-0.0.7/pytedea/utils/weakCQERG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCQERZG1.py` & `pytedea-0.0.7/pytedea/utils/weakCQERZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCQERZG2.py` & `pytedea-0.0.7/pytedea/utils/weakCQERZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCQERbG1.py` & `pytedea-0.0.7/pytedea/utils/weakCQERbG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCQERbG2.py` & `pytedea-0.0.7/pytedea/utils/weakCQERbG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCQERbZG1.py` & `pytedea-0.0.7/pytedea/utils/weakCQERbZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCQERbZG2.py` & `pytedea-0.0.7/pytedea/utils/weakCQERbZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCQERxG1.py` & `pytedea-0.0.7/pytedea/utils/weakCQERxG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCQERxG2.py` & `pytedea-0.0.7/pytedea/utils/weakCQERxG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCQERxZG1.py` & `pytedea-0.0.7/pytedea/utils/weakCQERxZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/utils/weakCQERxZG2.py` & `pytedea-0.0.7/pytedea/utils/weakCQERxZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/weakCNLSDDF.py` & `pytedea-0.0.7/pytedea/weakMetaCNLSDDF.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,29 +5,31 @@
 import numpy as np
 
 from . import  weakCNLSy
 from .constant import CET_ADDI, FUN_COST, FUN_PROD, RTS_VRS, RTS_CRS,OPT_DEFAULT, OPT_LOCAL
 from .utils import tools
 
 
-class weakCNLSDDF(weakCNLSy.weakCNLSy):
+class weakMetaCNLSDDF(weakCNLSy.weakCNLSy):
     """Convex Nonparametric Least Square with directional distance function
     """
 
-    def __init__(self, data,sent = "inputvar=outputvar:unoutputvar",z=None,  gy=[1], gx=[1], gb=[1], \
-                 rts=RTS_VRS,fun=FUN_PROD, baseindex=None,refindex=None):
+    def __init__(self, data,Eineff,sent = "inputvar=outputvar:unoutputvar",z=None,  gy=[1], gx=[1], gb=[1],\
+                 deduce="Y", fun=FUN_PROD,rts=RTS_VRS, baseindex=None,refindex=None):
         """DDFDUAL: Dual of Directional distance function
 
         Args:
             data (pandas.DataFrame): input pandas.
             sent (str): inputvars=outputvars: unoutputvars. e.g.: "K L = Y : CO2"
             z(str): contextual variable. e.g.: "Z1 Z2"
             gy (list, optional): output directional vector. Defaults to [1].
             gx (list, optional): input directional vector. Defaults to [1].
             gb (list, optional): undesirable output directional vector. Defaults to [1].
+            deduce(string,optional): deduce the value of the variable / directional vector of the variable \
+                                         form the value of all the varibles.Defaults to minus Y/gy .
             rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale)
             # year_name(str, optional): 年份列的名称. Defaults to None. e.g.: "Year"
             baseindex (String, optional): estimate index. Defaults to None. e.g.: "Year=[2010]"
             refindex (String, optional): reference index. Defaults to None. e.g.: "Year=[2010]"
         """
 
         self.outputvars, self.inputvars, self.unoutputvars, self.zvars, self.gy, self.gx, self.gb \
@@ -38,21 +40,60 @@
 
 
         self.xcol = self.x.columns
         self.ycol = self.y.columns
         self.bcol = self.b.columns
         self.zcol = self.z.columns if type(z) != type(None) else None
 
+        self.decuce = deduce
+        if deduce in self.xcol:
+            tomunus_col=self.x[[deduce]]
+            tomunus_index = list(self.xcol).index(deduce)
+            tomunus_g = self.gx[tomunus_index]
+            self.actrual_value = tomunus_col / tomunus_g
+            if tomunus_g==0:
+                raise ValueError("The directional vector of the variable you want to minus must not be 0.")
+        elif deduce in self.ycol:
+            tomunus_col=self.y[[deduce]]
+            tomunus_index = list(self.ycol).index(deduce)
+            tomunus_g = self.gy[tomunus_index]
+            self.actrual_value = tomunus_col / tomunus_g
+            if tomunus_g==0:
+                raise ValueError("The directional vector of the variable you want to minus must not be 0.")
+        elif deduce in self.bcol:
+            tomunus_col = self.b[[deduce]]
+            tomunus_index = list(self.bcol).index(deduce)
+            tomunus_g = self.gb[tomunus_index]
+            self.actrual_value = tomunus_col / tomunus_g
+            if tomunus_g == 0:
+                raise ValueError("The directional vector of the variable you want to minus must not be 0.")
+        else:
+            raise ValueError("deduce must be selected in your variables")
+        self.y = pd.DataFrame(self.y.to_numpy() -\
+                      self.actrual_value.to_numpy() * np.array(self.gy),columns=self.y.columns,index=self.y.index)
+        self.x = pd.DataFrame(self.x.to_numpy() +\
+                      self.actrual_value.to_numpy() * np.array(self.gx),columns=self.x.columns,index=self.x.index)
+        self.b = pd.DataFrame(self.b.to_numpy() +\
+                      self.actrual_value.to_numpy() * np.array(self.gb),columns=self.b.columns,index=self.b.index)
+
+        print("actrual_value222 is:",self.actrual_value)
+
         self.fun = fun
         self.rts = rts
 
         print("xcol,ycol,bcol are:",self.x.columns,self.y.columns,self.b.columns)
 
         print("gx,gy,gb are:",self.gx,self.gy,self.gb)
         # print("aaa",self.y,self.x,self.b)
+        self.Eineff = Eineff
+        Eineff.columns = ['Eineff1']
+        print("Eineff is:",self.Eineff)
+
+
+
 
         self.__model__ = ConcreteModel()
 
         # Initialize the sets
         self.__model__.I = Set(initialize=self.x.index)  ## I 是 被评价决策单元的数量
         if self.referenceflag:
             self.__model__.I2 = Set(initialize=self.xref.index)  ## I2 是 参考决策单元的数量
@@ -133,45 +174,49 @@
             self.__model__, email, CET_ADDI, solver)
 
     def __regression_rule(self):
         """Return the proper regression constraint"""
         if self.rts == RTS_VRS:
             if type(self.z) != type(None):
                 def regression_rule(model, i):
-                    return sum(model.gamma[i, l] * self.y.loc[i,self.ycol[l]] for l in model.L) \
+                    return self.actrual_value.loc[i,self.decuce]+self.Eineff.loc[i,'Eineff1']\
                         == model.alpha[i] \
                         + sum(model.beta[i, k] * self.x.loc[i,self.xcol[k]] for k in model.K) \
                         + sum(model.delta[i, j] * self.b.loc[i,self.bcol[j]] for j in model.J) \
+                        - sum(model.gamma[i, l] * self.y.loc[i, self.ycol[l]] for l in model.L) \
                         - sum(model.lamda[m] * self.z.loc[i,self.zcol[m]] for m in model.M) \
-                    - model.epsilon[i]
+                        - model.epsilon[i]
                 return regression_rule
 
             def regression_rule(model,i):
-                return sum(model.gamma[i,l] * self.y.loc[i,self.ycol[l]] for l in model.L) \
-                        == model.alpha[i] \
-                + sum(model.beta[i,k] * self.x.loc[i,self.xcol[k]] for k in model.K) \
-                + sum(model.delta[i,j] * self.b.loc[i,self.bcol[j]] for j in model.J) \
-                - model.epsilon[i]
+                return self.actrual_value.loc[i, self.decuce]+self.Eineff.loc[i,'Eineff1']\
+                    == model.alpha[i] \
+                    + sum(model.beta[i, k] * self.x.loc[i, self.xcol[k]] for k in model.K) \
+                    + sum(model.delta[i, j] * self.b.loc[i, self.bcol[j]] for j in model.J) \
+                    - sum(model.gamma[i, l] * self.y.loc[i, self.ycol[l]] for l in model.L) \
+                    - model.epsilon[i]
             return regression_rule
 
         elif self.rts == RTS_CRS:
             if type(self.z) != type(None):
                 def regression_rule(model, i):
-                    return sum(model.gamma[i, l] * self.y.loc[i,self.ycol[l]] for l in model.L) \
+                    return self.actrual_value.loc[i,self.decuce]+self.Eineff.loc[i,'Eineff1']\
                         == sum(model.beta[i, k] * self.x.loc[i,self.xcol[k]] for k in model.K) \
                         + sum(model.delta[i, j] * self.b.loc[i,self.bcol[j]] for j in model.J) \
+                        - sum(model.gamma[i, l] * self.y.loc[i, self.ycol[l]] for l in model.L) \
                         - sum(model.lamda[m] * self.z.loc[i,self.zcol[m]] for m in model.M) \
-                    - model.epsilon[i]
+                        - model.epsilon[i]
                 return regression_rule
 
             def regression_rule(model,i):
-                return sum(model.gamma[i,l] * self.y.loc[i,self.ycol[l]] for l in model.L) \
-                        == sum(model.beta[i,k] * self.x.loc[i,self.xcol[k]] for k in model.K) \
-                + sum(model.delta[i,j] * self.b.loc[i,self.bcol[j]] for j in model.J) \
-                - model.epsilon[i]
+                return self.actrual_value.loc[i, self.decuce]+self.Eineff.loc[i,'Eineff1']\
+                    == sum(model.beta[i, k] * self.x.loc[i, self.xcol[k]] for k in model.K) \
+                    + sum(model.delta[i, j] * self.b.loc[i, self.bcol[j]] for j in model.J) \
+                    - sum(model.gamma[i, l] * self.y.loc[i, self.ycol[l]] for l in model.L) \
+                    - model.epsilon[i]
             return regression_rule
 
         raise ValueError("Undefined model parameters.")
 
     def __translation_property(self):
         """Return the proper translation property"""
```

### Comparing `pytedea-0.0.6/pytedea/weakCNLSNDDF.py` & `pytedea-0.0.7/pytedea/weakCNLSNDDF_notransfer.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .constant import CET_ADDI, FUN_COST, FUN_PROD, RTS_VRS, RTS_CRS,OPT_DEFAULT, OPT_LOCAL
 from .utils import tools
 from . import  weakCNLSy
 import pandas as pd
 import numpy as np
 
 
-class weakCNLSNDDF(weakCNLSy.weakCNLSy):
+class weakCNLSNDDF_notransfer(weakCNLSy.weakCNLSy):
     """Convex Nonparametric Least Square with non-radial directional distance function
     """
 
     def __init__(self,data,sent, z=None, gy=[1], gx=[1], gb=[1],weight =None, \
                  fun=FUN_PROD, rts=RTS_VRS, baseindex=None,refindex=None):
         """weakCNLS NDDF model
```

### Comparing `pytedea-0.0.6/pytedea/weakCNLSb.py` & `pytedea-0.0.7/pytedea/weakCNLSb.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
             refindex (String, optional): reference index. Defaults to None. e.g.: "Year=[2010]"
         """
         self.outputvars,self.inputvars,self.unoutputvars,self.zvars = tools.assert_valid_weakCNLS(sent, z)
 
         self.y, self.x, self.b, self.z, self.yref, self.xref, self.bref, self.zref, self.referenceflag\
             = tools.assert_valid_weakCNLSDDF2(baseindex,refindex,data,\
                                        self.outputvars,self.inputvars,self.unoutputvars,self.zvars)
+        self.x["one"] = 1
         self.xcol = self.x.columns
         self.ycol = self.y.columns
         self.bcol = self.b.columns
         self.zcol = self.z.columns if type(z) != type(None) else None
 
         print("xcol,ycol,bcol are:",self.x.columns,self.y.columns,self.b.columns)
 
@@ -126,58 +127,60 @@
 
     def __regression_rule(self):
         """Return the proper regression constraint"""
         if self.cet == CET_ADDI:
             if self.rts == RTS_VRS:
                 if type(self.z) != type(None):
                     def regression_rule(model, i):
-                        return np.array((self.b.loc[i,]))  == -model.alpha[i] \
-                                - sum(model.beta[i, k] * self.x.loc[i,self.xcol[k]] for k in model.K) \
-                                + sum(model.gamma[i, l] * self.y.loc[i,self.ycol[l]] for l in model.L) \
-                                + sum(model.lamda[m] * self.z.loc[i,self.zcol[m]] for m in model.M) \
-                                + model.epsilon[i]
+                        return np.array(1/self.b.loc[i,])  == model.alpha[i] \
+                                + sum(model.beta[i, k] * self.x.loc[i,self.xcol[k]] for k in model.K) \
+                                - sum(model.gamma[i, l] * self.y.loc[i,self.ycol[l]] for l in model.L) \
+                                - sum(model.lamda[m] * self.z.loc[i,self.zcol[m]] for m in model.M) \
+                                - model.epsilon[i]
 
                     return regression_rule
 
                 def regression_rule(model, i):
-                    return np.array((self.b.loc[i,])) == -model.alpha[i] \
-                            - sum(model.beta[i, k] * self.x.loc[i,self.xcol[k]] for k in model.K) \
-                            + sum(model.gamma[i, l] * self.y.loc[i,self.ycol[l]] for l in model.L) \
-                            + model.epsilon[i]
+                    return np.array(1/self.b.loc[i,]) == model.alpha[i] \
+                            + sum(model.beta[i, k] * self.x.loc[i,self.xcol[k]] for k in model.K) \
+                            - sum(model.gamma[i, l] * self.y.loc[i,self.ycol[l]] for l in model.L) \
+                            - model.epsilon[i]
 
                 return regression_rule
             elif self.rts == RTS_CRS:
                 if type(self.z) != type(None):
                     def regression_rule(model, i):
-                        return np.array((self.b.loc[i,])) == -sum(model.beta[i, k] * self.x.loc[i,self.xcol[k]] for k in model.K) \
-                                + sum(model.gamma[i, l] * self.y.loc[i,self.ycol[l]] for l in model.L) \
-                                + sum(model.lamda[m] * self.z.loc[i,self.ycol[m]] for m in model.M) \
-                                + model.epsilon[i]
+                        return np.array(1/self.b.loc[i,]) == \
+                            sum(model.beta[i, k] * self.x.loc[i,self.xcol[k]] for k in model.K) \
+                                - sum(model.gamma[i, l] * self.y.loc[i,self.ycol[l]] for l in model.L) \
+                                - sum(model.lamda[m] * self.z.loc[i,self.ycol[m]] for m in model.M) \
+                                - model.epsilon[i]
 
                     return regression_rule
 
                 def regression_rule(model, i):
-                    return np.array((self.b.loc[i,])) == -sum(model.beta[i, k] * self.x.loc[i,self.xcol[k]] for k in model.K) \
-                            + sum(model.gamma[i, l] * self.y.loc[i,self.ycol[l]]  for l in model.L) \
-                            + model.epsilon[i]
+                    return np.array(1/self.b.loc[i,]) == \
+                        sum(model.beta[i, k] * self.x.loc[i,self.xcol[k]] for k in model.K) \
+                            - sum(model.gamma[i, l] * self.y.loc[i,self.ycol[l]]  for l in model.L) \
+                            - model.epsilon[i]
 
                 return regression_rule
 
         elif self.cet == CET_MULT:
             if type(self.z) != type(None):
                 def regression_rule(model, i):
-                    return log(np.array((self.b.loc[i,]))) == - log(model.frontier[i] + 1) \
+                    return log(np.array(1/self.b.loc[i,])) == log(model.frontier[i] + 1) \
                             + sum(model.lamda[m] * self.z.loc[i,self.ycol[m]]  for m in model.M) \
-                            + model.epsilon[i]
+                            - model.epsilon[i]
 
                 return regression_rule
 
             def regression_rule(model, i):
-                return log(np.array((self.b.loc[i,]))) == - log(model.frontier[i] + 1) \
-                        + model.epsilon[i]
+                return log(np.array(1/self.b.loc[i,])) == log(model.frontier[i] + 1) \
+                        - model.epsilon[i]
 
             return regression_rule
 
         raise ValueError("Undefined model parameters.")
 
     def __log_rule(self):
         """Return the proper log constraint"""
```

### Comparing `pytedea-0.0.6/pytedea/weakCNLSx.py` & `pytedea-0.0.7/pytedea/weakCNLSx.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea/weakCNLSy.py` & `pytedea-0.0.7/pytedea/weakCNLSy.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.6/pytedea.egg-info/PKG-INFO` & `pytedea-0.0.7/pytedea.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytedea
-Version: 0.0.6
+Version: 0.0.7
 Summary: Data envelopment analysis using Python.
 Home-page: https://github.com/advancehs/pytedea
 Author: advancehs
 Author-email: 1019753743@qq.com
 License: GNU General Public License v3
 Keywords: pytedea
 Classifier: Intended Audience :: Developers
```

### Comparing `pytedea-0.0.6/pytedea.egg-info/SOURCES.txt` & `pytedea-0.0.7/pytedea.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,35 +3,41 @@
 README.md
 requirements.txt
 setup.cfg
 setup.py
 pytedea/CNLS.py
 pytedea/CNLSDDF.py
 pytedea/DDF.py
+pytedea/DDFDUAL.py
 pytedea/DDFt.py
 pytedea/DEA.py
 pytedea/DEAt.py
 pytedea/HYPER.py
 pytedea/HYPERt.py
 pytedea/MB.py
 pytedea/MQDDF.py
 pytedea/MQDDFt.py
 pytedea/MQDEA.py
 pytedea/MQDEAt.py
 pytedea/MQNDDF.py
 pytedea/NDDF.py
+pytedea/NDDFDUAL.py
 pytedea/StoNED.py
 pytedea/__init__.py
 pytedea/constant.py
 pytedea/pytedea.py
 pytedea/weakCNLSDDF.py
 pytedea/weakCNLSNDDF.py
+pytedea/weakCNLSNDDF_notransfer.py
 pytedea/weakCNLSb.py
 pytedea/weakCNLSx.py
 pytedea/weakCNLSy.py
+pytedea/weakMetaCNLSDDF.py
+pytedea/weakMetaCNLSNDDF.py
+pytedea/weakMetaCNLSb.py
 pytedea.egg-info/PKG-INFO
 pytedea.egg-info/SOURCES.txt
 pytedea.egg-info/dependency_links.txt
 pytedea.egg-info/not-zip-safe
 pytedea.egg-info/requires.txt
 pytedea.egg-info/top_level.txt
 pytedea/utils/CNLSDDFG1.py
```

### Comparing `pytedea-0.0.6/setup.py` & `pytedea-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='pytedea',
     name='pytedea',
     packages=find_packages(include=['pytedea', 'pytedea.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/advancehs/pytedea',
-    version='0.0.6',
+    version='0.0.7',
     zip_safe=False,
 )
```

