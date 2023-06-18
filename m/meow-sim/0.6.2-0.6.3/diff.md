# Comparing `tmp/meow-sim-0.6.2.tar.gz` & `tmp/meow-sim-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.6.2.tar", last modified: Sun Jun 18 16:52:23 2023, max compression
+gzip compressed data, was "meow-sim-0.6.3.tar", last modified: Sun Jun 18 18:53:35 2023, max compression
```

## Comparing `meow-sim-0.6.2.tar` & `meow-sim-0.6.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:52:23.816506 meow-sim-0.6.2/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-06-18 16:52:18.000000 meow-sim-0.6.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-18 16:52:23.816506 meow-sim-0.6.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2223 2023-06-18 16:52:18.000000 meow-sim-0.6.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:52:23.812506 meow-sim-0.6.2/meow/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:52:23.812506 meow-sim-0.6.2/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8378 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     3855 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     5473 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:52:23.816506 meow-sim-0.6.2/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6175 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     3923 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:52:23.816506 meow-sim-0.6.2/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4911 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     3275 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2318 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)    10421 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    10062 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     4758 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)    13596 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     1751 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     8100 2023-06-18 16:52:18.000000 meow-sim-0.6.2/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:52:23.816506 meow-sim-0.6.2/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-18 16:52:23.000000 meow-sim-0.6.2/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-06-18 16:52:23.000000 meow-sim-0.6.2/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-18 16:52:23.000000 meow-sim-0.6.2/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      444 2023-06-18 16:52:23.000000 meow-sim-0.6.2/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-18 16:52:23.000000 meow-sim-0.6.2/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1864 2023-06-18 16:52:18.000000 meow-sim-0.6.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-18 16:52:23.816506 meow-sim-0.6.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:52:23.816506 meow-sim-0.6.2/tests/
--rw-r--r--   0 root         (0) root         (0)     3931 2023-06-18 16:52:18.000000 meow-sim-0.6.2/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)     3767 2023-06-18 16:52:18.000000 meow-sim-0.6.2/tests/test_mode_operators.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-06-18 16:52:18.000000 meow-sim-0.6.2/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 18:53:35.774995 meow-sim-0.6.3/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-06-18 18:53:31.000000 meow-sim-0.6.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-18 18:53:35.774995 meow-sim-0.6.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-06-18 18:53:31.000000 meow-sim-0.6.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 18:53:35.774995 meow-sim-0.6.3/meow/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-06-18 18:53:31.000000 meow-sim-0.6.3/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 18:53:35.774995 meow-sim-0.6.3/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-06-18 18:53:31.000000 meow-sim-0.6.3/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-06-18 18:53:31.000000 meow-sim-0.6.3/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8378 2023-06-18 18:53:31.000000 meow-sim-0.6.3/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-18 18:53:31.000000 meow-sim-0.6.3/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     3855 2023-06-18 18:53:31.000000 meow-sim-0.6.3/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     5473 2023-06-18 18:53:31.000000 meow-sim-0.6.3/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 18:53:35.774995 meow-sim-0.6.3/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-06-18 18:53:31.000000 meow-sim-0.6.3/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6175 2023-06-18 18:53:31.000000 meow-sim-0.6.3/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     3923 2023-06-18 18:53:31.000000 meow-sim-0.6.3/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-18 18:53:31.000000 meow-sim-0.6.3/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 18:53:35.774995 meow-sim-0.6.3/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-18 18:53:31.000000 meow-sim-0.6.3/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4911 2023-06-18 18:53:31.000000 meow-sim-0.6.3/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     3275 2023-06-18 18:53:31.000000 meow-sim-0.6.3/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-06-18 18:53:31.000000 meow-sim-0.6.3/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)    10421 2023-06-18 18:53:31.000000 meow-sim-0.6.3/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-06-18 18:53:31.000000 meow-sim-0.6.3/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    10062 2023-06-18 18:53:31.000000 meow-sim-0.6.3/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     4758 2023-06-18 18:53:31.000000 meow-sim-0.6.3/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    17342 2023-06-18 18:53:31.000000 meow-sim-0.6.3/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2023-06-18 18:53:31.000000 meow-sim-0.6.3/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     8100 2023-06-18 18:53:31.000000 meow-sim-0.6.3/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 18:53:35.774995 meow-sim-0.6.3/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-18 18:53:35.000000 meow-sim-0.6.3/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-18 18:53:35.000000 meow-sim-0.6.3/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-18 18:53:35.000000 meow-sim-0.6.3/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      444 2023-06-18 18:53:35.000000 meow-sim-0.6.3/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-18 18:53:35.000000 meow-sim-0.6.3/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-06-18 18:53:31.000000 meow-sim-0.6.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-18 18:53:35.774995 meow-sim-0.6.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 18:53:35.774995 meow-sim-0.6.3/tests/
+-rw-r--r--   0 root         (0) root         (0)     3931 2023-06-18 18:53:31.000000 meow-sim-0.6.3/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2023-06-18 18:53:31.000000 meow-sim-0.6.3/tests/test_mode_operators.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-06-18 18:53:31.000000 meow-sim-0.6.3/tests/test_nbs.py
```

### Comparing `meow-sim-0.6.2/LICENSE` & `meow-sim-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.2/PKG-INFO` & `meow-sim-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.6.2
+Version: 0.6.3
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.6.2/README.md` & `meow-sim-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.2/meow/__init__.py` & `meow-sim-0.6.3/meow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.6.2"
+__version__ = "0.6.3"
 
 import warnings
 
 # Silence Excessive Logging...
 
 try:
     from loguru import logger
```

### Comparing `meow-sim-0.6.2/meow/assets/silicon.csv` & `meow-sim-0.6.3/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.2/meow/assets/silicon_oxide.csv` & `meow-sim-0.6.3/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.2/meow/base_model.py` & `meow-sim-0.6.3/meow/base_model.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.2/meow/cache.py` & `meow-sim-0.6.3/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.2/meow/cell.py` & `meow-sim-0.6.3/meow/cell.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.2/meow/cross_section.py` & `meow-sim-0.6.3/meow/cross_section.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.2/meow/eme/__init__.py` & `meow-sim-0.6.3/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.2/meow/eme/common.py` & `meow-sim-0.6.3/meow/eme/common.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.2/meow/eme/sax.py` & `meow-sim-0.6.3/meow/eme/sax.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.2/meow/environment.py` & `meow-sim-0.6.3/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.2/meow/fde/lumerical.py` & `meow-sim-0.6.3/meow/fde/lumerical.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.2/meow/fde/tidy3d.py` & `meow-sim-0.6.3/meow/fde/tidy3d.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.2/meow/gds_structures.py` & `meow-sim-0.6.3/meow/gds_structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.2/meow/geometries.py` & `meow-sim-0.6.3/meow/geometries.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.2/meow/integrate.py` & `meow-sim-0.6.3/meow/integrate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.2/meow/materials.py` & `meow-sim-0.6.3/meow/materials.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.2/meow/mesh.py` & `meow-sim-0.6.3/meow/mesh.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.2/meow/mode.py` & `meow-sim-0.6.3/meow/mode.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ An EigenMode """
 
 import pickle
 import warnings
 from itertools import product
-from typing import List, Tuple
+from typing import List, Literal, Tuple
 
 import numpy as np
 from pydantic import Field
 from scipy.constants import epsilon_0 as eps0
 from scipy.constants import mu_0 as mu0
 from scipy.linalg import norm
 
@@ -38,14 +38,32 @@
     )
     Hy: np.ndarray[Tuple[int, int], np.dtype[np.complex_]] = Field(
         description="the Hy-fields of the mode"
     )
     Hz: np.ndarray[Tuple[int, int], np.dtype[np.complex_]] = Field(
         description="the Hz-fields of the mode"
     )
+    interpolation: Literal["Ex", "Ey", "Ez", "Hz"] | None = Field(
+        default=None,
+        description="To which 2D Yee-location the fields are interpolated to.",
+    )
+
+    def interpolate(self, location: Literal["Ex", "Ey", "Ez", "Hx", "Hy", "Hz"]):
+        if self.interpolation is not None:
+            raise RuntimeError("Cannot interpolate from already interpolated mode!")
+        interpolate_funcs = {
+            "EX": _interpolate_Ex,
+            "EY": _interpolate_Ey,
+            "EZ": _interpolate_Ez,
+            "HX": _interpolate_Ey,
+            "HY": _interpolate_Ex,
+            "HZ": _interpolate_Hz,
+        }
+        interpolate_func = interpolate_funcs[location.upper()]
+        return interpolate_func(self)
 
     @property
     def te_fraction(self):
         """the TE polarization fraction of the mode."""
         return te_fraction(self)
 
     @cached_property
@@ -429,7 +447,97 @@
 
 def te_fraction(mode: Mode) -> float:
     """the TE polarization fraction of the `Mode`"""
     epsx = mode.cs.nx**2
     e = np.sum(0.5 * eps0 * epsx * np.abs(mode.Ex) ** 2)
     h = np.sum(0.5 * mu0 * np.abs(mode.Hx) ** 2)
     return float(e / (e + h))
+
+
+def _average(field, direction="forward", axis=0):
+    direction = direction.lower()
+    if not direction in ["forward", "backward"]:
+        raise ValueError("direction should be 'forward' or backward")
+    if not axis in [0, 1]:
+        raise ValueError("axis should be zero or 1")
+    elif axis == 1:
+        return _average(field.T, direction=direction, axis=0).T
+    average = 0.5 * (field[1:] + field[:-1])
+    zero = np.zeros_like(average[:1])
+    if direction == "forward":
+        return np.concatenate([zero, average], axis=0)
+    else:
+        return np.concatenate([average, zero], axis=0)
+
+
+def _interpolate_Ex(mode: Mode) -> Mode:
+    # TODO: take grid spacing into account
+    Ey_at_Ez = _average(mode.Ey, direction="backward", axis=1)
+    Ey_at_Ex = _average(Ey_at_Ez, direction="forward", axis=0)
+    Ez_at_Ex = _average(mode.Ez, direction="forward", axis=0)
+    Hx_at_Hz = _average(mode.Hx, direction="forward", axis=0)
+    Hx_at_Ex = _average(Hx_at_Hz, direction="backward", axis=1)
+    Hz_at_Ex = _average(mode.Hz, direction="backward", axis=1)
+    return Mode(
+        neff=mode.neff,
+        cs=mode.cs,
+        Ex=mode.Ex,
+        Ey=Ey_at_Ex,
+        Ez=Ez_at_Ex,
+        Hx=Hx_at_Ex,
+        Hy=mode.Hy,
+        Hz=Hz_at_Ex,
+    )
+
+
+def _interpolate_Ey(mode: Mode) -> Mode:
+    # TODO: take grid spacing into account
+    Ex_at_Ez = _average(mode.Ex, direction="backward", axis=0)
+    Ex_at_Ey = _average(Ex_at_Ez, direction="forward", axis=1)
+    Ez_at_Ey = _average(mode.Ez, direction="forward", axis=1)
+    Hy_at_Hz = _average(mode.Hy, direction="forward", axis=1)
+    Hy_at_Ey = _average(Hy_at_Hz, direction="backward", axis=0)
+    Hz_at_Ey = _average(mode.Hz, direction="backward", axis=0)
+    return Mode(
+        neff=mode.neff,
+        cs=mode.cs,
+        Ex=Ex_at_Ey,
+        Ey=mode.Ey,
+        Ez=Ez_at_Ey,
+        Hx=mode.Hx,
+        Hy=Hy_at_Ey,
+        Hz=Hz_at_Ey,
+    )
+
+
+def _interpolate_Ez(mode: Mode) -> Mode:
+    # TODO: take grid spacing into account
+    return Mode(
+        neff=mode.neff,
+        cs=mode.cs,
+        Ex=_average(mode.Ex, direction="backward", axis=0),
+        Ey=_average(mode.Ey, direction="backward", axis=1),
+        Ez=mode.Ez,
+        Hx=_average(mode.Hx, direction="backward", axis=1),
+        Hy=_average(mode.Hy, direction="backward", axis=0),
+        Hz=_average(
+            _average(mode.Hz, direction="backward", axis=0),
+            direction="backward",
+            axis=1,
+        ),
+    )
+
+
+def _interpolate_Hz(mode: Mode) -> Mode:
+    # TODO: take grid spacing into account
+    return Mode(
+        neff=mode.neff,
+        cs=mode.cs,
+        Ex=_average(mode.Ex, direction="forward", axis=1),
+        Ey=_average(mode.Ey, direction="forward", axis=0),
+        Ez=_average(
+            _average(mode.Ez, direction="forward", axis=0), direction="forward", axis=1
+        ),
+        Hx=_average(mode.Hx, direction="forward", axis=0),
+        Hy=_average(mode.Hy, direction="forward", axis=1),
+        Hz=mode.Hz,
+    )
```

### Comparing `meow-sim-0.6.2/meow/structures.py` & `meow-sim-0.6.3/meow/structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.2/meow/visualize.py` & `meow-sim-0.6.3/meow/visualize.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.2/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.6.3/meow_sim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.6.2
+Version: 0.6.3
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.6.2/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.6.3/meow_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.2/pyproject.toml` & `meow-sim-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.6.2"
+version = "0.6.3"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `meow-sim-0.6.2/tests/test_deserialization.py` & `meow-sim-0.6.3/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.2/tests/test_mode_operators.py` & `meow-sim-0.6.3/tests/test_mode_operators.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.2/tests/test_nbs.py` & `meow-sim-0.6.3/tests/test_nbs.py`

 * *Files identical despite different names*

