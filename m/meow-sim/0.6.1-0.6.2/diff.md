# Comparing `tmp/meow-sim-0.6.1.tar.gz` & `tmp/meow-sim-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.6.1.tar", last modified: Sat Jun 17 23:33:33 2023, max compression
+gzip compressed data, was "meow-sim-0.6.2.tar", last modified: Sun Jun 18 16:52:23 2023, max compression
```

## Comparing `meow-sim-0.6.1.tar` & `meow-sim-0.6.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 23:33:33.974767 meow-sim-0.6.1/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-06-17 23:33:29.000000 meow-sim-0.6.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-17 23:33:33.974767 meow-sim-0.6.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2223 2023-06-17 23:33:29.000000 meow-sim-0.6.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 23:33:33.974767 meow-sim-0.6.1/meow/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 23:33:33.974767 meow-sim-0.6.1/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8378 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     3855 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     5473 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 23:33:33.974767 meow-sim-0.6.1/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6175 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     3923 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 23:33:33.974767 meow-sim-0.6.1/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4911 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     3275 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2318 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)    10421 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    10062 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     4280 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)    13595 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     1751 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     8100 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 23:33:33.974767 meow-sim-0.6.1/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-17 23:33:33.000000 meow-sim-0.6.1/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-06-17 23:33:33.000000 meow-sim-0.6.1/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 23:33:33.000000 meow-sim-0.6.1/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      444 2023-06-17 23:33:33.000000 meow-sim-0.6.1/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-17 23:33:33.000000 meow-sim-0.6.1/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1864 2023-06-17 23:33:29.000000 meow-sim-0.6.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-17 23:33:33.974767 meow-sim-0.6.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 23:33:33.974767 meow-sim-0.6.1/tests/
--rw-r--r--   0 root         (0) root         (0)     3931 2023-06-17 23:33:29.000000 meow-sim-0.6.1/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)     3767 2023-06-17 23:33:29.000000 meow-sim-0.6.1/tests/test_mode_operators.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-06-17 23:33:29.000000 meow-sim-0.6.1/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:52:23.816506 meow-sim-0.6.2/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-06-18 16:52:18.000000 meow-sim-0.6.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-18 16:52:23.816506 meow-sim-0.6.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-06-18 16:52:18.000000 meow-sim-0.6.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:52:23.812506 meow-sim-0.6.2/meow/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:52:23.812506 meow-sim-0.6.2/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8378 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     3855 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     5473 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:52:23.816506 meow-sim-0.6.2/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6175 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     3923 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:52:23.816506 meow-sim-0.6.2/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4911 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     3275 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)    10421 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    10062 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     4758 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    13596 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     8100 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:52:23.816506 meow-sim-0.6.2/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-18 16:52:23.000000 meow-sim-0.6.2/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-18 16:52:23.000000 meow-sim-0.6.2/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-18 16:52:23.000000 meow-sim-0.6.2/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      444 2023-06-18 16:52:23.000000 meow-sim-0.6.2/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-18 16:52:23.000000 meow-sim-0.6.2/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-06-18 16:52:18.000000 meow-sim-0.6.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-18 16:52:23.816506 meow-sim-0.6.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:52:23.816506 meow-sim-0.6.2/tests/
+-rw-r--r--   0 root         (0) root         (0)     3931 2023-06-18 16:52:18.000000 meow-sim-0.6.2/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2023-06-18 16:52:18.000000 meow-sim-0.6.2/tests/test_mode_operators.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-06-18 16:52:18.000000 meow-sim-0.6.2/tests/test_nbs.py
```

### Comparing `meow-sim-0.6.1/LICENSE` & `meow-sim-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.1/PKG-INFO` & `meow-sim-0.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.6.1
+Version: 0.6.2
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.6.1/README.md` & `meow-sim-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.1/meow/__init__.py` & `meow-sim-0.6.2/meow/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 
 import warnings
 
 # Silence Excessive Logging...
 
 try:
     from loguru import logger
```

### Comparing `meow-sim-0.6.1/meow/assets/silicon.csv` & `meow-sim-0.6.2/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.1/meow/assets/silicon_oxide.csv` & `meow-sim-0.6.2/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.1/meow/base_model.py` & `meow-sim-0.6.2/meow/base_model.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.1/meow/cache.py` & `meow-sim-0.6.2/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.1/meow/cell.py` & `meow-sim-0.6.2/meow/cell.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.1/meow/cross_section.py` & `meow-sim-0.6.2/meow/cross_section.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.1/meow/eme/__init__.py` & `meow-sim-0.6.2/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.1/meow/eme/common.py` & `meow-sim-0.6.2/meow/eme/common.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.1/meow/eme/sax.py` & `meow-sim-0.6.2/meow/eme/sax.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.1/meow/environment.py` & `meow-sim-0.6.2/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.1/meow/fde/lumerical.py` & `meow-sim-0.6.2/meow/fde/lumerical.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.1/meow/fde/tidy3d.py` & `meow-sim-0.6.2/meow/fde/tidy3d.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.1/meow/gds_structures.py` & `meow-sim-0.6.2/meow/gds_structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.1/meow/geometries.py` & `meow-sim-0.6.2/meow/geometries.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.1/meow/integrate.py` & `meow-sim-0.6.2/meow/integrate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.1/meow/materials.py` & `meow-sim-0.6.2/meow/materials.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.1/meow/mesh.py` & `meow-sim-0.6.2/meow/mesh.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,85 +50,102 @@
     num_pml: Tuple[NonNegativeInt, NonNegativeInt] = Field(
         default=(0, 0),
         description="Number of standard pml layers to add in the two tangential axes.",
     )
 
     @cached_property
     def dx(self):
-        """x-coordinate mesh step (Hz locations, i.e. center of the 2D cell)"""
+        """dx at Hz locations, i.e. center of the 2D cell"""
         return (self.x[1:] - self.x[:-1]).view(_array)
 
     @cached_property
     def dy(self):
-        """y-coordinate mesh step (Hz locations, i.e. center of the 2D cell)"""
+        """dy at Hz locations, i.e. center of the 2D cell"""
         return (self.y[1:] - self.y[:-1]).view(_array)
 
     @cached_property
     def x_(self):
-        """x-coordinate mesh step (Hz locations, i.e. center of the 2D cell)"""
+        """x at Hz locations, i.e. center of the 2D cell"""
         return 0.5 * (self.x[1:] + self.x[:-1]).view(_array)
 
     @cached_property
     def y_(self):
-        """y-coordinate mesh step (Hz locations, i.e. center of the 2D cell)"""
+        """y at Hz locations, i.e. center of the 2D cell"""
         return 0.5 * (self.y[1:] + self.y[:-1]).view(_array)
 
     @cached_property
     def x_full(self):
+        """x at half-integer locations"""
         return (
-            np.stack([self.x[:-1] + self.dx / 4, self.x[:-1] + 3 * self.dx / 4], 1)
-            .ravel()
-            .view(_array)
+            np.stack([self.x[:-1], self.x[:-1] + self.dx / 2], 1).ravel().view(_array)
         )
 
     @cached_property
     def y_full(self):
+        """y at half-integer locations"""
         return (
-            np.stack([self.y[:-1] + self.dy / 4, self.y[:-1] + 3 * self.dy / 4], 1)
-            .ravel()
-            .view(_array)
+            np.stack([self.y[:-1], self.y[:-1] + self.dy / 2], 1).ravel().view(_array)
         )
 
     @cached_property
     def XY_full(self):
+        """X and Y at half-integer locations"""
         Y_full, X_full = np.meshgrid(self.y_full, self.x_full)
         return X_full.view(_array), Y_full.view(_array)
 
     @property
     def X_full(self):
+        """X at half-integer locations"""
         return self.XY_full[0].view(_array)
 
     @property
     def Y_full(self):
+        """Y at half-integer locations"""
         return self.XY_full[1].view(_array)
 
     @property
     def Xx(self):
+        """X at Ex locations"""
         return self.X_full[1::2, ::2].view(_array)
 
     @property
     def Yx(self):
+        """Y at Ex locations"""
         return self.Y_full[1::2, ::2].view(_array)
 
     @property
     def Xy(self):
+        """X at Ey locations"""
         return self.X_full[::2, 1::2].view(_array)
 
     @property
     def Yy(self):
+        """Y at Ey locations"""
         return self.Y_full[::2, 1::2].view(_array)
 
     @property
     def Xz(self):
+        """X at Ez locations"""
         return self.X_full[::2, ::2].view(_array)
 
     @property
     def Yz(self):
+        """Y at Ez locations"""
         return self.Y_full[::2, ::2].view(_array)
 
+    @property
+    def Xz_(self):
+        """X at Hz locations"""
+        return self.X_full[1::2, 1::2].view(_array)
+
+    @property
+    def Yz_(self):
+        """Y at Hz locations"""
+        return self.Y_full[1::2, 1::2].view(_array)
+
     def __eq__(self, other):
         eq = True
         for k, v in self.dict().items():
             if isinstance(v, np.ndarray):
                 eq &= ((v - getattr(other, k)) < 1e-6).all()
             else:
                 eq &= v == getattr(other, k)
```

### Comparing `meow-sim-0.6.1/meow/mode.py` & `meow-sim-0.6.2/meow/mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
             # little bit lighter colored than the one in cs._visualize:
             n_cmap = colors.LinearSegmentedColormap.from_list(
                 name="c_cmap", colors=["#ffffff", "#c1d9ed"]
             )
         self.cs._visualize(ax=ax, n_cmap=n_cmap, cbar=False, show=False)
 
         x, y = "x", "y"  # currently only propagation in z supported, see Mesh2d
-        c = {"Ex": "x", "Ey": "y", "Ez": "z", "Hx": "y", "Hy": "x", "Hz": "z"}[field]
+        c = {"Ex": "x", "Ey": "y", "Ez": "z", "Hx": "y", "Hy": "x", "Hz": "z_"}[field]
         if mode_cmap is None:
             mode_cmap = "inferno"
         X = getattr(self.mesh, f"X{c}")
         Y = getattr(self.mesh, f"Y{c}")
         mode = operation(getattr(self, field))
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=UserWarning)
```

### Comparing `meow-sim-0.6.1/meow/structures.py` & `meow-sim-0.6.2/meow/structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.1/meow/visualize.py` & `meow-sim-0.6.2/meow/visualize.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.1/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.6.2/meow_sim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.6.1
+Version: 0.6.2
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.6.1/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.6.2/meow_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.1/pyproject.toml` & `meow-sim-0.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.6.1"
+version = "0.6.2"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `meow-sim-0.6.1/tests/test_deserialization.py` & `meow-sim-0.6.2/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.1/tests/test_mode_operators.py` & `meow-sim-0.6.2/tests/test_mode_operators.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.1/tests/test_nbs.py` & `meow-sim-0.6.2/tests/test_nbs.py`

 * *Files identical despite different names*

