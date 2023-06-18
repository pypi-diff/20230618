# Comparing `tmp/simple-interpolator-0.1.1.tar.gz` & `tmp/simple-interpolator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-interpolator-0.1.1.tar", last modified: Sat Jun 17 10:31:38 2023, max compression
+gzip compressed data, was "simple-interpolator-0.1.2.tar", last modified: Sun Jun 18 07:22:39 2023, max compression
```

## Comparing `simple-interpolator-0.1.1.tar` & `simple-interpolator-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-17 10:31:38.031640 simple-interpolator-0.1.1/
--rw-r--r--   0 stef      (1000) stef      (1000)      494 2023-06-17 10:31:38.028307 simple-interpolator-0.1.1/PKG-INFO
--rw-r--r--   0 stef      (1000) stef      (1000)     2855 2023-06-17 09:43:55.000000 simple-interpolator-0.1.1/README.md
--rw-r--r--   0 stef      (1000) stef      (1000)       38 2023-06-17 10:31:38.031640 simple-interpolator-0.1.1/setup.cfg
--rw-r--r--   0 stef      (1000) stef      (1000)      794 2023-06-17 10:31:36.000000 simple-interpolator-0.1.1/setup.py
-drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-17 10:31:38.028307 simple-interpolator-0.1.1/simple_interpolator/
--rw-r--r--   0 stef      (1000) stef      (1000)       57 2023-06-17 10:31:04.000000 simple-interpolator-0.1.1/simple_interpolator/__init__.py
--rw-r--r--   0 stef      (1000) stef      (1000)     2269 2023-06-17 10:30:44.000000 simple-interpolator-0.1.1/simple_interpolator/interpolator.py
--rw-r--r--   0 stef      (1000) stef      (1000)      664 2023-06-16 14:59:49.000000 simple-interpolator-0.1.1/simple_interpolator/stylizer.py
-drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-17 10:31:38.028307 simple-interpolator-0.1.1/simple_interpolator.egg-info/
--rw-r--r--   0 stef      (1000) stef      (1000)      494 2023-06-17 10:31:37.000000 simple-interpolator-0.1.1/simple_interpolator.egg-info/PKG-INFO
--rw-r--r--   0 stef      (1000) stef      (1000)      332 2023-06-17 10:31:37.000000 simple-interpolator-0.1.1/simple_interpolator.egg-info/SOURCES.txt
--rw-r--r--   0 stef      (1000) stef      (1000)        1 2023-06-17 10:31:37.000000 simple-interpolator-0.1.1/simple_interpolator.egg-info/dependency_links.txt
--rw-r--r--   0 stef      (1000) stef      (1000)       17 2023-06-17 10:31:37.000000 simple-interpolator-0.1.1/simple_interpolator.egg-info/requires.txt
--rw-r--r--   0 stef      (1000) stef      (1000)       20 2023-06-17 10:31:37.000000 simple-interpolator-0.1.1/simple_interpolator.egg-info/top_level.txt
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-18 07:22:39.197807 simple-interpolator-0.1.2/
+-rw-r--r--   0 stef      (1000) stef      (1000)      494 2023-06-18 07:22:39.197807 simple-interpolator-0.1.2/PKG-INFO
+-rw-r--r--   0 stef      (1000) stef      (1000)     3427 2023-06-18 07:17:25.000000 simple-interpolator-0.1.2/README.md
+-rw-r--r--   0 stef      (1000) stef      (1000)       38 2023-06-18 07:22:39.197807 simple-interpolator-0.1.2/setup.cfg
+-rw-r--r--   0 stef      (1000) stef      (1000)      794 2023-06-18 07:22:20.000000 simple-interpolator-0.1.2/setup.py
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-18 07:22:39.197807 simple-interpolator-0.1.2/simple_interpolator/
+-rw-r--r--   0 stef      (1000) stef      (1000)       57 2023-06-18 07:19:33.000000 simple-interpolator-0.1.2/simple_interpolator/__init__.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     2781 2023-06-18 07:19:46.000000 simple-interpolator-0.1.2/simple_interpolator/interpolator.py
+-rw-r--r--   0 stef      (1000) stef      (1000)      664 2023-06-16 14:59:49.000000 simple-interpolator-0.1.2/simple_interpolator/stylizer.py
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-18 07:22:39.197807 simple-interpolator-0.1.2/simple_interpolator.egg-info/
+-rw-r--r--   0 stef      (1000) stef      (1000)      494 2023-06-18 07:22:39.000000 simple-interpolator-0.1.2/simple_interpolator.egg-info/PKG-INFO
+-rw-r--r--   0 stef      (1000) stef      (1000)      332 2023-06-18 07:22:39.000000 simple-interpolator-0.1.2/simple_interpolator.egg-info/SOURCES.txt
+-rw-r--r--   0 stef      (1000) stef      (1000)        1 2023-06-18 07:22:39.000000 simple-interpolator-0.1.2/simple_interpolator.egg-info/dependency_links.txt
+-rw-r--r--   0 stef      (1000) stef      (1000)       17 2023-06-18 07:22:39.000000 simple-interpolator-0.1.2/simple_interpolator.egg-info/requires.txt
+-rw-r--r--   0 stef      (1000) stef      (1000)       20 2023-06-18 07:22:39.000000 simple-interpolator-0.1.2/simple_interpolator.egg-info/top_level.txt
```

### Comparing `simple-interpolator-0.1.1/README.md` & `simple-interpolator-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -33,22 +33,26 @@
 from simple_interpolator.interpolator import Interpolator
 ```
 
 <br>
 
 # `Interpolator` class
 
-|                     members                     | desription                                     |
-| :---------------------------------------------: | :--------------------------------------------- |
-|    [`graph()`](./docs/Interpolator/graph.md)    | three-dimentional graph of the interpolant     |
-| [`colormap()`](./docs/Interpolator/colormap.md) | two-dimentional colormap of the interpolant    |
-|                    `show()`                     | renders all of the visualisations              |
-|                     `data`                      | a list of the provided coordinates             |
-|                       `f`                       | an interpolant function                        |
-| [`print_f()` ](./docs/Interpolator/print_f.md)  | mathematical representation of the interpolant |
+|                            members                            | desription                                     |
+| :-----------------------------------------------------------: | :--------------------------------------------- |
+|           [`graph()`](./docs/Interpolator/graph.md)           | three-dimentional graph of the interpolant     |
+|        [`colormap()`](./docs/Interpolator/colormap.md)        | two-dimentional colormap of the interpolant    |
+|            [`show()`](./docs/Interpolator/show.md)            | renders all of the visualisations              |
+|  [`add_coordinate()`](./docs/Interpolator/add_coordiante.md)  | provide an additional coordiante               |
+| [`add_coordinates()`](./docs/Interpolator/add_coordinates.md) | provide a list of additional coordinates       |
+|        [`set_rank()`](./docs/Interpolator/set_rank.md)        | set a max power of a variable                  |
+|       [`auto_rank()`](./docs/Interpolator/auto_rank.md)       | fit the data perfectly automatically           |
+|                            `data`                             | a list of the provided coordinates             |
+|                              `f`                              | an interpolant function                        |
+|        [`print_f()` ](./docs/Interpolator/print_f.md)         | mathematical representation of the interpolant |
 
 <br>
 
 # Example
 
 ```python
 from simple_interpolator.interpolator import Interpolator
```

#### html2text {}

```diff
@@ -12,21 +12,27 @@
 - Mathematical representation of the interpolant polynomial.
 # How to install it? ```shell pip install simple-interpolator ``` > Find out
 more [here](https://pypi.org/project/simple-interpolator/).
 # How to use it? The library `simple_interpolator` provides a file
 `interpolator` encapsulating a class `Interpolator`. ```python from
 simple_interpolator.interpolator import Interpolator ```
 # `Interpolator` class | members | desription | | :----------------------------
------------------: | :--------------------------------------------- | | [`graph
-()`](./docs/Interpolator/graph.md) | three-dimentional graph of the interpolant
-| | [`colormap()`](./docs/Interpolator/colormap.md) | two-dimentional colormap
-of the interpolant | | `show()` | renders all of the visualisations | | `data`
-| a list of the provided coordinates | | `f` | an interpolant function | |
-[`print_f()` ](./docs/Interpolator/print_f.md) | mathematical representation of
-the interpolant |
+-------------------------------: | :-------------------------------------------
+-- | | [`graph()`](./docs/Interpolator/graph.md) | three-dimentional graph of
+the interpolant | | [`colormap()`](./docs/Interpolator/colormap.md) | two-
+dimentional colormap of the interpolant | | [`show()`](./docs/Interpolator/
+show.md) | renders all of the visualisations | | [`add_coordinate()`](./docs/
+Interpolator/add_coordiante.md) | provide an additional coordiante | |
+[`add_coordinates()`](./docs/Interpolator/add_coordinates.md) | provide a list
+of additional coordinates | | [`set_rank()`](./docs/Interpolator/set_rank.md) |
+set a max power of a variable | | [`auto_rank()`](./docs/Interpolator/
+auto_rank.md) | fit the data perfectly automatically | | `data` | a list of the
+provided coordinates | | `f` | an interpolant function | | [`print_f()` ](./
+docs/Interpolator/print_f.md) | mathematical representation of the interpolant
+|
 # Example ```python from simple_interpolator.interpolator import Interpolator i
 = Interpolator([(2,-5,2),(6,-3,4),(3,-6,4),(-4,3,5),(5,-4,8),(3,7,-5)]) print
 ("Provided coordinates:\n\n\t", i.data, "\n") print("An interpolant:
 \n\n",end='\t') i.print_f(1) i.graph() i.colormap() i.show() ``` Output:
 ```shell Provided coordinates: [(2, 5, -4), (6, 3, -4), (3, -6, 4), (4, -3, 5),
 (5, -4, 8)] Generated interpolant: 9.7+1.5x+0.4xÂ²-0.1y-0.1xy-0.1xÂ²y+0.2yÂ²
 ``` [./assets/graph.png] [./assets/colormap.png] > The spacial visualisation is
```

### Comparing `simple-interpolator-0.1.1/setup.py` & `simple-interpolator-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 DESCRIPTION = 'A simple interpolator.'
 
 # Setting up
 setup(
     name="simple-interpolator",
     version=VERSION,
     author="var-pi (Stefan Ehin)",
```

### Comparing `simple-interpolator-0.1.1/simple_interpolator/interpolator.py` & `simple-interpolator-0.1.2/simple_interpolator/interpolator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,64 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import functools
 import math
 from simple_interpolator.stylizer import f_as_text
 
 class Interpolator:
-    def __init__(self, data):
+    data = []
+    __power_touples = []
+    __b = []
+    f = None
+    rank = -1
+
+    def __init__(self, data, rank=-1):
         self.data = data
-        self.__power_touples = self.__generate_power_touples()
-        self.__b = self.__generate_b()
-        self.f = self.__generate_f()
+        self.rank = rank
+        self.__generate_f()
 
     def __generate_power_touples(self):
-        rank = math.ceil(len(self.data)**0.5)-1
+        rank = math.ceil(len(self.data)**0.5)-1 if self.rank == -1 else self.rank
         return [[i, j] for j in range(rank+1) for i in range(rank+1)]
 
     def __generate_b(self):
         def power_values(x, y):
             return [x**p_t[0]*y**p_t[1] for p_t in self.__power_touples]
 
         A = [power_values(touple[0], touple[1]) for touple in self.data]
         At = np.transpose(A)
         f = list(map(lambda touple : touple[2], self.data))
 
         return np.linalg.solve(np.matmul(At, A), np.matmul(At, f))
 
     def __generate_f(self):
-        def f(x, y):
-            return sum([self.__b[i]*x**powers[0]*y**powers[1] for i, powers in enumerate(self.__power_touples)])
-        return f
+        print("ehere")
+        self.__power_touples = self.__generate_power_touples()
+        self.__b = self.__generate_b()
+        self.f = lambda x, y : sum([self.__b[i]*x**powers[0]*y**powers[1] for i, powers in enumerate(self.__power_touples)])
 
     def print_f(self, accuracy=-1):
         print(f_as_text(self.__b, self.__power_touples,accuracy))
 
+    def add_coordinates(self, coordinates):
+        self.data += coordinates
+        self.__generate_f()
+
+    def add_coordinate(self, coordinate):
+        self.data += [coordinate]
+        self.__generate_f()
+
+    def set_rank(self, rank):
+        self.rank = rank
+        self.__generate_f()
+    
+    def auto_rank(self):
+        self.rank = -1
+        self.__generate_f()
+
     def __getXYZ(self, knots_per_unit):
         bound = lambda f, axis_id : functools.reduce(lambda acc, touple : f(touple[axis_id], acc), self.data, self.data[0][axis_id])
 
         X, Y = np.meshgrid(
                 np.linspace(bound(min, 0), bound(max, 0), knots_per_unit), 
                 np.linspace(bound(min, 1), bound(max, 1), knots_per_unit))
```

### Comparing `simple-interpolator-0.1.1/simple_interpolator/stylizer.py` & `simple-interpolator-0.1.2/simple_interpolator/stylizer.py`

 * *Files identical despite different names*

