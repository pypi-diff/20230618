# Comparing `tmp/skmetpy-0.0.9.tar.gz` & `tmp/skmetpy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skmetpy-0.0.9.tar", last modified: Sun Jun 18 17:58:29 2023, max compression
+gzip compressed data, was "skmetpy-0.1.0.tar", last modified: Sun Jun 18 21:26:26 2023, max compression
```

## Comparing `skmetpy-0.0.9.tar` & `skmetpy-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 17:58:29.333502 skmetpy-0.0.9/
--rw-rw-rw-   0        0        0      259 2023-06-18 17:58:29.333502 skmetpy-0.0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-18 17:58:29.327679 skmetpy-0.0.9/nunpy/
--rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.0.9/nunpy/__init__.py
--rw-rw-rw-   0        0        0    25181 2023-06-18 17:58:17.000000 skmetpy-0.0.9/nunpy/rechape.py
--rw-rw-rw-   0        0        0       42 2023-06-18 17:58:29.333502 skmetpy-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      324 2023-06-18 17:58:24.000000 skmetpy-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:58:29.332500 skmetpy-0.0.9/skmetpy.egg-info/
--rw-rw-rw-   0        0        0      259 2023-06-18 17:58:29.000000 skmetpy-0.0.9/skmetpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-06-18 17:58:29.000000 skmetpy-0.0.9/skmetpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 17:58:29.000000 skmetpy-0.0.9/skmetpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-18 17:58:29.000000 skmetpy-0.0.9/skmetpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 21:26:26.694148 skmetpy-0.1.0/
+-rw-rw-rw-   0        0        0      259 2023-06-18 21:26:26.693147 skmetpy-0.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-18 21:26:26.685140 skmetpy-0.1.0/nunpy/
+-rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.1.0/nunpy/__init__.py
+-rw-rw-rw-   0        0        0    25182 2023-06-18 21:25:23.000000 skmetpy-0.1.0/nunpy/rechape.py
+-rw-rw-rw-   0        0        0       42 2023-06-18 21:26:26.695149 skmetpy-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      324 2023-06-18 21:26:17.000000 skmetpy-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 21:26:26.691144 skmetpy-0.1.0/skmetpy.egg-info/
+-rw-rw-rw-   0        0        0      259 2023-06-18 21:26:26.000000 skmetpy-0.1.0/skmetpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-06-18 21:26:26.000000 skmetpy-0.1.0/skmetpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 21:26:26.000000 skmetpy-0.1.0/skmetpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-18 21:26:26.000000 skmetpy-0.1.0/skmetpy.egg-info/top_level.txt
```

### Comparing `skmetpy-0.0.9/nunpy/rechape.py` & `skmetpy-0.1.0/nunpy/rechape.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,15 +254,15 @@
                 return gradiente
       '''
     print(string)
 
 
 def fmin1():
     string = '''
-            maxiter = 15
+            maxiter = 200
             nn_params = opt.fmin_cg(maxiter=maxiter, f=nnCostFunction, x0=nn_params, fprime=nnGradFunction, args=(
             input_layer_size, hidden_layer_size1, hidden_layer_size2, num_labels, X_training, y_training.flatten()))
       '''
     print(string)
 
 
 def unroll1():
```

