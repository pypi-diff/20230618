# Comparing `tmp/classattr-1.0.0.tar.gz` & `tmp/classattr-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classattr-1.0.0.tar", last modified: Sun Jun 18 14:56:27 2023, max compression
+gzip compressed data, was "classattr-1.0.1.tar", last modified: Sun Jun 18 15:17:06 2023, max compression
```

## Comparing `classattr-1.0.0.tar` & `classattr-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-06-18 14:56:27.363165 classattr-1.0.0/
--rw-rw-r--   0 thierry   (1000) thierry   (1000)     1075 2023-05-20 07:22:28.000000 classattr-1.0.0/LICENSE
--rw-rw-r--   0 thierry   (1000) thierry   (1000)      318 2023-06-18 14:56:27.363165 classattr-1.0.0/PKG-INFO
--rw-rw-r--   0 thierry   (1000) thierry   (1000)     1010 2023-06-18 07:21:25.000000 classattr-1.0.0/README.md
-drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-06-18 14:56:27.363165 classattr-1.0.0/classattr.egg-info/
--rw-rw-r--   0 thierry   (1000) thierry   (1000)      318 2023-06-18 14:56:27.000000 classattr-1.0.0/classattr.egg-info/PKG-INFO
--rw-rw-r--   0 thierry   (1000) thierry   (1000)      158 2023-06-18 14:56:27.000000 classattr-1.0.0/classattr.egg-info/SOURCES.txt
--rw-rw-r--   0 thierry   (1000) thierry   (1000)        1 2023-06-18 14:56:27.000000 classattr-1.0.0/classattr.egg-info/dependency_links.txt
--rw-rw-r--   0 thierry   (1000) thierry   (1000)        1 2023-06-18 14:56:27.000000 classattr-1.0.0/classattr.egg-info/top_level.txt
--rw-rw-r--   0 thierry   (1000) thierry   (1000)       38 2023-06-18 14:56:27.363165 classattr-1.0.0/setup.cfg
--rw-rw-r--   0 thierry   (1000) thierry   (1000)      328 2023-06-18 14:55:57.000000 classattr-1.0.0/setup.py
+drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-06-18 15:17:06.807811 classattr-1.0.1/
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)     1075 2023-05-20 07:22:28.000000 classattr-1.0.1/LICENSE
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)     1221 2023-06-18 15:17:06.807811 classattr-1.0.1/PKG-INFO
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)     1010 2023-06-18 07:21:25.000000 classattr-1.0.1/README.md
+drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-06-18 15:17:06.807811 classattr-1.0.1/classattr.egg-info/
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)     1221 2023-06-18 15:17:06.000000 classattr-1.0.1/classattr.egg-info/PKG-INFO
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)      158 2023-06-18 15:17:06.000000 classattr-1.0.1/classattr.egg-info/SOURCES.txt
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)        1 2023-06-18 15:17:06.000000 classattr-1.0.1/classattr.egg-info/dependency_links.txt
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)        1 2023-06-18 15:17:06.000000 classattr-1.0.1/classattr.egg-info/top_level.txt
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)       38 2023-06-18 15:17:06.807811 classattr-1.0.1/setup.cfg
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)      490 2023-06-18 15:16:55.000000 classattr-1.0.1/setup.py
```

### Comparing `classattr-1.0.0/LICENSE` & `classattr-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `classattr-1.0.0/README.md` & `classattr-1.0.1/README.md`

 * *Files identical despite different names*

