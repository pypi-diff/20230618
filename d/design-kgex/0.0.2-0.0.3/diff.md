# Comparing `tmp/design_kgex-0.0.2.tar.gz` & `tmp/design_kgex-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "design_kgex-0.0.2.tar", last modified: Sun Jun 18 03:26:20 2023, max compression
+gzip compressed data, was "design_kgex-0.0.3.tar", last modified: Sun Jun 18 03:33:32 2023, max compression
```

## Comparing `design_kgex-0.0.2.tar` & `design_kgex-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 03:26:20.940007 design_kgex-0.0.2/
--rw-rw-rw-   0        0        0     1134 2023-06-18 02:58:12.000000 design_kgex-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      757 2023-06-18 03:26:20.940007 design_kgex-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-18 03:26:20.940007 design_kgex-0.0.2/design_kgex/
--rw-rw-rw-   0        0        0        0 2023-06-18 03:24:08.000000 design_kgex-0.0.2/design_kgex/__init__.py
--rw-rw-rw-   0        0        0     2819 2023-06-18 02:53:49.000000 design_kgex-0.0.2/design_kgex/design_knowledge.py
--rw-rw-rw-   0        0        0     4894 2023-06-18 02:53:06.000000 design_kgex-0.0.2/design_kgex/patent_text.py
--rw-rw-rw-   0        0        0    16255 2023-06-16 23:48:26.000000 design_kgex-0.0.2/design_kgex/supplementary.py
-drwxrwxrwx   0        0        0        0 2023-06-18 03:26:20.940007 design_kgex-0.0.2/design_kgex.egg-info/
--rw-rw-rw-   0        0        0      757 2023-06-18 03:26:20.000000 design_kgex-0.0.2/design_kgex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-06-18 03:26:20.000000 design_kgex-0.0.2/design_kgex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 03:26:20.000000 design_kgex-0.0.2/design_kgex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-06-18 03:26:20.000000 design_kgex-0.0.2/design_kgex.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-18 03:26:20.000000 design_kgex-0.0.2/design_kgex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 03:26:20.940007 design_kgex-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1286 2023-06-18 03:25:25.000000 design_kgex-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:33:32.716196 design_kgex-0.0.3/
+-rw-rw-rw-   0        0        0     1134 2023-06-18 02:58:12.000000 design_kgex-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      757 2023-06-18 03:33:32.713761 design_kgex-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-18 03:33:32.693900 design_kgex-0.0.3/design_kgex/
+-rw-rw-rw-   0        0        0      114 2023-06-18 03:30:48.000000 design_kgex-0.0.3/design_kgex/__init__.py
+-rw-rw-rw-   0        0        0     2819 2023-06-18 02:53:49.000000 design_kgex-0.0.3/design_kgex/design_knowledge.py
+-rw-rw-rw-   0        0        0     4894 2023-06-18 02:53:06.000000 design_kgex-0.0.3/design_kgex/patent_text.py
+-rw-rw-rw-   0        0        0    16255 2023-06-16 23:48:26.000000 design_kgex-0.0.3/design_kgex/supplementary.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:33:32.710744 design_kgex-0.0.3/design_kgex.egg-info/
+-rw-rw-rw-   0        0        0      757 2023-06-18 03:33:32.000000 design_kgex-0.0.3/design_kgex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-06-18 03:33:32.000000 design_kgex-0.0.3/design_kgex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 03:33:32.000000 design_kgex-0.0.3/design_kgex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-06-18 03:33:32.000000 design_kgex-0.0.3/design_kgex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-18 03:33:32.000000 design_kgex-0.0.3/design_kgex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 03:33:32.716196 design_kgex-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1286 2023-06-18 03:33:06.000000 design_kgex-0.0.3/setup.py
```

### Comparing `design_kgex-0.0.2/LICENSE` & `design_kgex-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `design_kgex-0.0.2/PKG-INFO` & `design_kgex-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design_kgex
-Version: 0.0.2
+Version: 0.0.3
 Summary: Extracting Design Knowledge from Patent-Text
 Author: L. Siddharth
 Author-email: siddharthl.iitrpr.sutd@gmail.com
 Keywords: Design Knowledge,Knowledge Extraction,Knowledge Graph,Engineering Design,Patent Text,Token Classification,Transformers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: GPU
 Classifier: Intended Audience :: Science/Research
```

### Comparing `design_kgex-0.0.2/design_kgex/design_knowledge.py` & `design_kgex-0.0.3/design_kgex/design_knowledge.py`

 * *Files identical despite different names*

### Comparing `design_kgex-0.0.2/design_kgex/patent_text.py` & `design_kgex-0.0.3/design_kgex/patent_text.py`

 * *Files identical despite different names*

### Comparing `design_kgex-0.0.2/design_kgex/supplementary.py` & `design_kgex-0.0.3/design_kgex/supplementary.py`

 * *Files identical despite different names*

### Comparing `design_kgex-0.0.2/design_kgex.egg-info/PKG-INFO` & `design_kgex-0.0.3/design_kgex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design-kgex
-Version: 0.0.2
+Version: 0.0.3
 Summary: Extracting Design Knowledge from Patent-Text
 Author: L. Siddharth
 Author-email: siddharthl.iitrpr.sutd@gmail.com
 Keywords: Design Knowledge,Knowledge Extraction,Knowledge Graph,Engineering Design,Patent Text,Token Classification,Transformers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: GPU
 Classifier: Intended Audience :: Science/Research
```

### Comparing `design_kgex-0.0.2/setup.py` & `design_kgex-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Extracting Design Knowledge from Patent-Text'
 
 setup(
     name="design_kgex",
     version=VERSION,
     author="L. Siddharth",
     author_email="siddharthl.iitrpr.sutd@gmail.com",
```

