# Comparing `tmp/skmetpy-0.0.8.tar.gz` & `tmp/skmetpy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skmetpy-0.0.8.tar", last modified: Sun Jun 18 15:29:05 2023, max compression
+gzip compressed data, was "skmetpy-0.0.9.tar", last modified: Sun Jun 18 17:58:29 2023, max compression
```

## Comparing `skmetpy-0.0.8.tar` & `skmetpy-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 15:29:05.791853 skmetpy-0.0.8/
--rw-rw-rw-   0        0        0      259 2023-06-18 15:29:05.790851 skmetpy-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-18 15:29:05.785334 skmetpy-0.0.8/nunpy/
--rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.0.8/nunpy/__init__.py
--rw-rw-rw-   0        0        0    25022 2023-06-18 15:28:54.000000 skmetpy-0.0.8/nunpy/rechape.py
--rw-rw-rw-   0        0        0       42 2023-06-18 15:29:05.791853 skmetpy-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      324 2023-06-18 15:29:01.000000 skmetpy-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 15:29:05.789851 skmetpy-0.0.8/skmetpy.egg-info/
--rw-rw-rw-   0        0        0      259 2023-06-18 15:29:05.000000 skmetpy-0.0.8/skmetpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-06-18 15:29:05.000000 skmetpy-0.0.8/skmetpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 15:29:05.000000 skmetpy-0.0.8/skmetpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-18 15:29:05.000000 skmetpy-0.0.8/skmetpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 17:58:29.333502 skmetpy-0.0.9/
+-rw-rw-rw-   0        0        0      259 2023-06-18 17:58:29.333502 skmetpy-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-18 17:58:29.327679 skmetpy-0.0.9/nunpy/
+-rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.0.9/nunpy/__init__.py
+-rw-rw-rw-   0        0        0    25181 2023-06-18 17:58:17.000000 skmetpy-0.0.9/nunpy/rechape.py
+-rw-rw-rw-   0        0        0       42 2023-06-18 17:58:29.333502 skmetpy-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      324 2023-06-18 17:58:24.000000 skmetpy-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:58:29.332500 skmetpy-0.0.9/skmetpy.egg-info/
+-rw-rw-rw-   0        0        0      259 2023-06-18 17:58:29.000000 skmetpy-0.0.9/skmetpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-06-18 17:58:29.000000 skmetpy-0.0.9/skmetpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 17:58:29.000000 skmetpy-0.0.9/skmetpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-18 17:58:29.000000 skmetpy-0.0.9/skmetpy.egg-info/top_level.txt
```

### Comparing `skmetpy-0.0.8/nunpy/rechape.py` & `skmetpy-0.0.9/nunpy/rechape.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,23 +113,27 @@
 
     print(string)
 
 
 def norm1():
     string = '''
             def normalize(X, X_training):
-                  mean = np.mean(X_training, axis=0)
-                  std = np.mean(X_training, axis=0)
-
-                  X_normalizado = list()
-
-                  for i in range(len(X_training)):
-                  X_normalizado.append((X_training[i] - mean) / std)
-
-                  return X_normalizado, mean, std
+                # Obtenemos la media por columnas
+                mean = np.mean(X, axis=0)
+                std = np.std(X, axis=0)
+            
+                normal = []
+            
+                # Calculamos por filas los nuevos valores de las X
+                for i in range(X_training.shape[0]):
+                    x = X_training[i] - mean
+                    x = x / std
+                    normal.append(x)
+            
+                return normal, mean, std
       '''
 
     print(string)
 
 
 def ini1():
     string = '''
```

