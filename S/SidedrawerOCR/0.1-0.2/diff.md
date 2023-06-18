# Comparing `tmp/SidedrawerOCR-0.1.tar.gz` & `tmp/SidedrawerOCR-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SidedrawerOCR-0.1.tar", last modified: Sun Jun 18 15:59:43 2023, max compression
+gzip compressed data, was "SidedrawerOCR-0.2.tar", last modified: Sun Jun 18 16:32:07 2023, max compression
```

## Comparing `SidedrawerOCR-0.1.tar` & `SidedrawerOCR-0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 woojaejo   (501) staff       (20)        0 2023-06-18 15:59:43.383789 SidedrawerOCR-0.1/
--rw-r--r--   0 woojaejo   (501) staff       (20)     1071 2023-06-18 15:19:16.000000 SidedrawerOCR-0.1/LICENSE
-drwxr-xr-x   0 woojaejo   (501) staff       (20)        0 2023-06-18 15:59:43.382406 SidedrawerOCR-0.1/Library/
--rw-r--r--   0 woojaejo   (501) staff       (20)       22 2023-06-18 15:32:03.000000 SidedrawerOCR-0.1/Library/__init__.py
--rw-r--r--   0 woojaejo   (501) staff       (20)     1850 2023-06-18 15:56:05.000000 SidedrawerOCR-0.1/Library/main.py
--rw-r--r--   0 woojaejo   (501) staff       (20)     7416 2023-06-18 15:58:52.000000 SidedrawerOCR-0.1/Library/utils.py
--rw-r--r--   0 woojaejo   (501) staff       (20)      190 2023-06-18 15:59:43.383640 SidedrawerOCR-0.1/PKG-INFO
--rw-r--r--   0 woojaejo   (501) staff       (20)       12 2023-06-18 15:00:09.000000 SidedrawerOCR-0.1/README.md
-drwxr-xr-x   0 woojaejo   (501) staff       (20)        0 2023-06-18 15:59:43.383129 SidedrawerOCR-0.1/SidedrawerOCR.egg-info/
--rw-r--r--   0 woojaejo   (501) staff       (20)      190 2023-06-18 15:59:43.000000 SidedrawerOCR-0.1/SidedrawerOCR.egg-info/PKG-INFO
--rw-r--r--   0 woojaejo   (501) staff       (20)      300 2023-06-18 15:59:43.000000 SidedrawerOCR-0.1/SidedrawerOCR.egg-info/SOURCES.txt
--rw-r--r--   0 woojaejo   (501) staff       (20)        1 2023-06-18 15:59:43.000000 SidedrawerOCR-0.1/SidedrawerOCR.egg-info/dependency_links.txt
--rw-r--r--   0 woojaejo   (501) staff       (20)       39 2023-06-18 15:59:43.000000 SidedrawerOCR-0.1/SidedrawerOCR.egg-info/requires.txt
--rw-r--r--   0 woojaejo   (501) staff       (20)       14 2023-06-18 15:59:43.000000 SidedrawerOCR-0.1/SidedrawerOCR.egg-info/top_level.txt
--rw-r--r--   0 woojaejo   (501) staff       (20)       38 2023-06-18 15:59:43.383834 SidedrawerOCR-0.1/setup.cfg
--rw-r--r--   0 woojaejo   (501) staff       (20)      409 2023-06-18 15:17:56.000000 SidedrawerOCR-0.1/setup.py
-drwxr-xr-x   0 woojaejo   (501) staff       (20)        0 2023-06-18 15:59:43.383392 SidedrawerOCR-0.1/tests/
--rw-r--r--   0 woojaejo   (501) staff       (20)        0 2023-06-18 15:33:04.000000 SidedrawerOCR-0.1/tests/__init__.py
--rw-r--r--   0 woojaejo   (501) staff       (20)     2299 2023-06-18 15:37:18.000000 SidedrawerOCR-0.1/tests/test_main.py
+drwxr-xr-x   0 woojaejo   (501) staff       (20)        0 2023-06-18 16:32:07.745532 SidedrawerOCR-0.2/
+-rw-r--r--   0 woojaejo   (501) staff       (20)     1071 2023-06-18 15:19:16.000000 SidedrawerOCR-0.2/LICENSE
+drwxr-xr-x   0 woojaejo   (501) staff       (20)        0 2023-06-18 16:32:07.744138 SidedrawerOCR-0.2/Library/
+-rw-r--r--   0 woojaejo   (501) staff       (20)       22 2023-06-18 15:32:03.000000 SidedrawerOCR-0.2/Library/__init__.py
+-rw-r--r--   0 woojaejo   (501) staff       (20)     1850 2023-06-18 15:56:05.000000 SidedrawerOCR-0.2/Library/main.py
+-rw-r--r--   0 woojaejo   (501) staff       (20)     7416 2023-06-18 16:02:31.000000 SidedrawerOCR-0.2/Library/utils.py
+-rw-r--r--   0 woojaejo   (501) staff       (20)      190 2023-06-18 16:32:07.745379 SidedrawerOCR-0.2/PKG-INFO
+-rw-r--r--   0 woojaejo   (501) staff       (20)       12 2023-06-18 15:00:09.000000 SidedrawerOCR-0.2/README.md
+drwxr-xr-x   0 woojaejo   (501) staff       (20)        0 2023-06-18 16:32:07.744909 SidedrawerOCR-0.2/SidedrawerOCR.egg-info/
+-rw-r--r--   0 woojaejo   (501) staff       (20)      190 2023-06-18 16:32:07.000000 SidedrawerOCR-0.2/SidedrawerOCR.egg-info/PKG-INFO
+-rw-r--r--   0 woojaejo   (501) staff       (20)      300 2023-06-18 16:32:07.000000 SidedrawerOCR-0.2/SidedrawerOCR.egg-info/SOURCES.txt
+-rw-r--r--   0 woojaejo   (501) staff       (20)        1 2023-06-18 16:32:07.000000 SidedrawerOCR-0.2/SidedrawerOCR.egg-info/dependency_links.txt
+-rw-r--r--   0 woojaejo   (501) staff       (20)       49 2023-06-18 16:32:07.000000 SidedrawerOCR-0.2/SidedrawerOCR.egg-info/requires.txt
+-rw-r--r--   0 woojaejo   (501) staff       (20)       14 2023-06-18 16:32:07.000000 SidedrawerOCR-0.2/SidedrawerOCR.egg-info/top_level.txt
+-rw-r--r--   0 woojaejo   (501) staff       (20)       38 2023-06-18 16:32:07.745577 SidedrawerOCR-0.2/setup.cfg
+-rw-r--r--   0 woojaejo   (501) staff       (20)      419 2023-06-18 16:31:59.000000 SidedrawerOCR-0.2/setup.py
+drwxr-xr-x   0 woojaejo   (501) staff       (20)        0 2023-06-18 16:32:07.745155 SidedrawerOCR-0.2/tests/
+-rw-r--r--   0 woojaejo   (501) staff       (20)        0 2023-06-18 15:33:04.000000 SidedrawerOCR-0.2/tests/__init__.py
+-rw-r--r--   0 woojaejo   (501) staff       (20)     2299 2023-06-18 15:37:18.000000 SidedrawerOCR-0.2/tests/test_main.py
```

### Comparing `SidedrawerOCR-0.1/LICENSE` & `SidedrawerOCR-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SidedrawerOCR-0.1/Library/main.py` & `SidedrawerOCR-0.2/Library/main.py`

 * *Files identical despite different names*

### Comparing `SidedrawerOCR-0.1/Library/utils.py` & `SidedrawerOCR-0.2/Library/utils.py`

 * *Files identical despite different names*

### Comparing `SidedrawerOCR-0.1/tests/test_main.py` & `SidedrawerOCR-0.2/tests/test_main.py`

 * *Files identical despite different names*

