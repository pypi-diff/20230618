# Comparing `tmp/sumformer2-0.1.tar.gz` & `tmp/sumformer2-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sumformer2-0.1.tar", last modified: Sun Jun 18 09:45:57 2023, max compression
+gzip compressed data, was "sumformer2-0.2.tar", last modified: Sun Jun 18 10:08:41 2023, max compression
```

## Comparing `sumformer2-0.1.tar` & `sumformer2-0.2.tar`

### file list

```diff
@@ -1,13 +1,19 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-18 09:45:57.491985 sumformer2-0.1/
--rw-r--r--   0 ryan       (501) staff       (20)     1065 2023-06-07 16:24:08.000000 sumformer2-0.1/LICENSE
--rw-r--r--   0 ryan       (501) staff       (20)      210 2023-06-18 09:45:57.491609 sumformer2-0.1/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)       61 2023-06-07 16:24:08.000000 sumformer2-0.1/README.md
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-06-18 09:45:57.492102 sumformer2-0.1/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)      493 2023-06-18 09:45:22.000000 sumformer2-0.1/setup.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-18 09:45:57.490713 sumformer2-0.1/sumformer2.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)      210 2023-06-18 09:45:57.000000 sumformer2-0.1/sumformer2.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      232 2023-06-18 09:45:57.000000 sumformer2-0.1/sumformer2.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-06-18 09:45:57.000000 sumformer2-0.1/sumformer2.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)       56 2023-06-18 09:45:57.000000 sumformer2-0.1/sumformer2.egg-info/entry_points.txt
--rw-r--r--   0 ryan       (501) staff       (20)     1140 2023-06-18 09:45:57.000000 sumformer2-0.1/sumformer2.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-06-18 09:45:57.000000 sumformer2-0.1/sumformer2.egg-info/top_level.txt
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-18 10:08:41.748424 sumformer2-0.2/
+-rw-r--r--   0 ryan       (501) staff       (20)     1065 2023-06-07 16:24:08.000000 sumformer2-0.2/LICENSE
+-rw-r--r--   0 ryan       (501) staff       (20)      210 2023-06-18 10:08:41.748030 sumformer2-0.2/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)       61 2023-06-07 16:24:08.000000 sumformer2-0.2/README.md
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-06-18 10:08:41.748566 sumformer2-0.2/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)      489 2023-06-18 10:07:41.000000 sumformer2-0.2/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-18 10:08:41.743599 sumformer2-0.2/sumformer2/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-06-18 10:03:46.000000 sumformer2-0.2/sumformer2/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)    14712 2023-06-18 09:24:29.000000 sumformer2-0.2/sumformer2/main.py
+-rw-r--r--   0 ryan       (501) staff       (20)     8269 2023-06-15 18:12:32.000000 sumformer2-0.2/sumformer2/modules.py
+-rw-r--r--   0 ryan       (501) staff       (20)     5888 2023-06-17 19:25:15.000000 sumformer2-0.2/sumformer2/transformer.py
+-rw-r--r--   0 ryan       (501) staff       (20)     5819 2023-06-18 09:24:12.000000 sumformer2-0.2/sumformer2/utils.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-06-18 10:08:41.747182 sumformer2-0.2/sumformer2.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)      210 2023-06-18 10:08:41.000000 sumformer2-0.2/sumformer2.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      342 2023-06-18 10:08:41.000000 sumformer2-0.2/sumformer2.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-06-18 10:08:41.000000 sumformer2-0.2/sumformer2.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       52 2023-06-18 10:08:41.000000 sumformer2-0.2/sumformer2.egg-info/entry_points.txt
+-rw-r--r--   0 ryan       (501) staff       (20)     1140 2023-06-18 10:08:41.000000 sumformer2-0.2/sumformer2.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       11 2023-06-18 10:08:41.000000 sumformer2-0.2/sumformer2.egg-info/top_level.txt
```

### Comparing `sumformer2-0.1/LICENSE` & `sumformer2-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sumformer2-0.1/sumformer2.egg-info/requires.txt` & `sumformer2-0.2/sumformer2.egg-info/requires.txt`

 * *Files identical despite different names*

