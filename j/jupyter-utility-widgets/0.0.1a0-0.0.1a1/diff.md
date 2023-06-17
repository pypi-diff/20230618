# Comparing `tmp/jupyter-utility-widgets-0.0.1a0.tar.gz` & `tmp/jupyter-utility-widgets-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-utility-widgets-0.0.1a0.tar", last modified: Fri Jun 16 08:47:30 2023, max compression
+gzip compressed data, was "jupyter-utility-widgets-0.0.1a1.tar", last modified: Sat Jun 17 22:34:41 2023, max compression
```

## Comparing `jupyter-utility-widgets-0.0.1a0.tar` & `jupyter-utility-widgets-0.0.1a1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:47:30.247846 jupyter-utility-widgets-0.0.1a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-16 08:47:18.000000 jupyter-utility-widgets-0.0.1a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-16 08:47:30.247846 jupyter-utility-widgets-0.0.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-16 08:47:18.000000 jupyter-utility-widgets-0.0.1a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:47:30.247846 jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:47:18.000000 jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-16 08:47:18.000000 jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets/file_explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-16 08:47:18.000000 jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets/filter_design.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:47:30.247846 jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets/plot/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-16 08:47:18.000000 jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets/plot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:47:30.247846 jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets/plot/figures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:47:18.000000 jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets/plot/figures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-16 08:47:18.000000 jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets/plot/figures/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-16 08:47:18.000000 jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets/plot/figures/lines.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-16 08:47:18.000000 jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets/plot/figures/specgram.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-16 08:47:18.000000 jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets/plot/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-16 08:47:18.000000 jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets/plot/specgram_examiner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:47:30.247846 jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets/selector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:47:18.000000 jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets/selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-16 08:47:18.000000 jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets/selector/index_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:47:30.247846 jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets/utility/
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-16 08:47:18.000000 jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets/utility/numpy_parameter_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:47:30.247846 jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-16 08:47:30.000000 jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-16 08:47:30.000000 jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 08:47:30.000000 jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-16 08:47:30.000000 jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 08:47:30.000000 jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-16 08:47:18.000000 jupyter-utility-widgets-0.0.1a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 08:47:30.247846 jupyter-utility-widgets-0.0.1a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:34:41.644863 jupyter-utility-widgets-0.0.1a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-17 22:34:41.640863 jupyter-utility-widgets-0.0.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:34:41.640863 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/file_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/filter_design.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:34:41.640863 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/plot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:34:41.640863 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/plot/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/plot/figures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/plot/figures/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/plot/figures/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/plot/figures/specgram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/plot/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/plot/specgram_examiner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:34:41.640863 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/selector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/selector/index_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:34:41.640863 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/utility/numpy_parameter_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:34:41.640863 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-17 22:34:41.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-17 22:34:41.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 22:34:41.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-17 22:34:41.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-17 22:34:41.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 22:34:41.644863 jupyter-utility-widgets-0.0.1a1/setup.cfg
```

### Comparing `jupyter-utility-widgets-0.0.1a0/LICENSE` & `jupyter-utility-widgets-0.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.1a0/PKG-INFO` & `jupyter-utility-widgets-0.0.1a1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-utility-widgets
-Version: 0.0.1a0
+Version: 0.0.1a1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-utility
 
 Seeing I have been using a few widgets "patterns" over and over, I have decided to share and pack them in a convenient manner.
```

### Comparing `jupyter-utility-widgets-0.0.1a0/README.md` & `jupyter-utility-widgets-0.0.1a1/README.md`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets/file_explorer.py` & `jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/file_explorer.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets/filter_design.py` & `jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/filter_design.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,14 @@
         ]
         super().__init__(children, **kwargs)
 
         for child in children:
             child.observe(lambda evt: self.calc_filt(),names=["value"])
     
     def calc_filt(self, ):
-        print(self.window_selector.value)
         self.value = firwin(
             self.window_length.value,
             self.cutoff_input.value,
             window=self.window_selector.value
         )
 
 class FilterDesign(HBox):
```

### Comparing `jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets/plot/figures/base.py` & `jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/plot/figures/base.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets/plot/figures/lines.py` & `jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/plot/figures/lines.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets/plot/figures/specgram.py` & `jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/plot/figures/specgram.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets/plot/filter.py` & `jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/plot/filter.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets/plot/specgram_examiner.py` & `jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/plot/specgram_examiner.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets/selector/index_selector.py` & `jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/selector/index_selector.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets/utility/numpy_parameter_converter.py` & `jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/utility/numpy_parameter_converter.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets.egg-info/PKG-INFO` & `jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-utility-widgets
-Version: 0.0.1a0
+Version: 0.0.1a1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-utility
 
 Seeing I have been using a few widgets "patterns" over and over, I have decided to share and pack them in a convenient manner.
```

### Comparing `jupyter-utility-widgets-0.0.1a0/jupyter_utility_widgets.egg-info/SOURCES.txt` & `jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

