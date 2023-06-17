# Comparing `tmp/meow-sim-0.6.0.tar.gz` & `tmp/meow-sim-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.6.0.tar", last modified: Thu Jun 15 17:58:52 2023, max compression
+gzip compressed data, was "meow-sim-0.6.1.tar", last modified: Sat Jun 17 23:33:33 2023, max compression
```

## Comparing `meow-sim-0.6.0.tar` & `meow-sim-0.6.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 17:58:52.397406 meow-sim-0.6.0/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-06-15 17:58:48.000000 meow-sim-0.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-15 17:58:52.397406 meow-sim-0.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2223 2023-06-15 17:58:48.000000 meow-sim-0.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 17:58:52.393406 meow-sim-0.6.0/meow/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 17:58:52.393406 meow-sim-0.6.0/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8378 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     4628 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     2495 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 17:58:52.393406 meow-sim-0.6.0/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6175 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     3923 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 17:58:52.393406 meow-sim-0.6.0/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4621 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     2969 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2318 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)    10642 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    10062 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)    12777 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     1751 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     7947 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 17:58:52.393406 meow-sim-0.6.0/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-15 17:58:52.000000 meow-sim-0.6.0/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-06-15 17:58:52.000000 meow-sim-0.6.0/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 17:58:52.000000 meow-sim-0.6.0/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-15 17:58:52.000000 meow-sim-0.6.0/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-15 17:58:52.000000 meow-sim-0.6.0/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1819 2023-06-15 17:58:48.000000 meow-sim-0.6.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 17:58:52.397406 meow-sim-0.6.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 17:58:52.397406 meow-sim-0.6.0/tests/
--rw-r--r--   0 root         (0) root         (0)     3931 2023-06-15 17:58:48.000000 meow-sim-0.6.0/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)     3767 2023-06-15 17:58:48.000000 meow-sim-0.6.0/tests/test_mode_operators.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-06-15 17:58:48.000000 meow-sim-0.6.0/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 23:33:33.974767 meow-sim-0.6.1/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-06-17 23:33:29.000000 meow-sim-0.6.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-17 23:33:33.974767 meow-sim-0.6.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-06-17 23:33:29.000000 meow-sim-0.6.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 23:33:33.974767 meow-sim-0.6.1/meow/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 23:33:33.974767 meow-sim-0.6.1/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8378 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     3855 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     5473 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 23:33:33.974767 meow-sim-0.6.1/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6175 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     3923 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 23:33:33.974767 meow-sim-0.6.1/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4911 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     3275 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)    10421 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    10062 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     4280 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    13595 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     8100 2023-06-17 23:33:29.000000 meow-sim-0.6.1/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 23:33:33.974767 meow-sim-0.6.1/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-17 23:33:33.000000 meow-sim-0.6.1/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-17 23:33:33.000000 meow-sim-0.6.1/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 23:33:33.000000 meow-sim-0.6.1/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      444 2023-06-17 23:33:33.000000 meow-sim-0.6.1/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-17 23:33:33.000000 meow-sim-0.6.1/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-06-17 23:33:29.000000 meow-sim-0.6.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-17 23:33:33.974767 meow-sim-0.6.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 23:33:33.974767 meow-sim-0.6.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     3931 2023-06-17 23:33:29.000000 meow-sim-0.6.1/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2023-06-17 23:33:29.000000 meow-sim-0.6.1/tests/test_mode_operators.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-06-17 23:33:29.000000 meow-sim-0.6.1/tests/test_nbs.py
```

### Comparing `meow-sim-0.6.0/LICENSE` & `meow-sim-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.0/PKG-INFO` & `meow-sim-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.6.0
+Version: 0.6.1
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.6.0/README.md` & `meow-sim-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.0/meow/__init__.py` & `meow-sim-0.6.1/meow/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 
 import warnings
 
 # Silence Excessive Logging...
 
 try:
     from loguru import logger
```

### Comparing `meow-sim-0.6.0/meow/assets/silicon.csv` & `meow-sim-0.6.1/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.0/meow/assets/silicon_oxide.csv` & `meow-sim-0.6.1/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.0/meow/base_model.py` & `meow-sim-0.6.1/meow/base_model.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.0/meow/cache.py` & `meow-sim-0.6.1/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.0/meow/eme/__init__.py` & `meow-sim-0.6.1/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.0/meow/eme/common.py` & `meow-sim-0.6.1/meow/eme/common.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.0/meow/eme/sax.py` & `meow-sim-0.6.1/meow/eme/sax.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.0/meow/environment.py` & `meow-sim-0.6.1/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.0/meow/fde/lumerical.py` & `meow-sim-0.6.1/meow/fde/lumerical.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,56 +78,69 @@
             }
         )
         num_pml_z = 22  # TODO: allow adjusting these values
     sim.addfde(
         background_index=1.0,
         solver_type="2D X normal",
         x=float(cs.cell.z * unit),
-        y_min=float(cs.mesh.x.min() * unit),
-        y_max=float(cs.mesh.x.max() * unit),
-        z_min=float(cs.mesh.y.min() * unit),
-        z_max=float(cs.mesh.y.max() * unit),
+        y_min=float(cs.cell.mesh.x.min() * unit),
+        y_max=float(cs.cell.mesh.x.max() * unit),
+        z_min=float(cs.cell.mesh.y.min() * unit),
+        z_max=float(cs.cell.mesh.y.max() * unit),
         define_y_mesh_by="number of mesh cells",
         define_z_mesh_by="number of mesh cells",
-        mesh_cells_y=cs.mesh.x_.shape[0],
-        mesh_cells_z=cs.mesh.y_.shape[0],
+        mesh_cells_y=cs.cell.mesh.x_.shape[0],
+        mesh_cells_z=cs.cell.mesh.y_.shape[0],
         **pml_settings,
     )
     # set mesh size again, because PML messes with it:
     if cs.cell.mesh.num_pml[0] > 0:
-        sim.setnamed("FDE", "mesh cells y", cs.mesh.x_.shape[0] - num_pml_y)
+        sim.setnamed("FDE", "mesh cells y", cs.cell.mesh.x_.shape[0] - num_pml_y)
     if cs.cell.mesh.num_pml[1] > 0:
-        sim.setnamed("FDE", "mesh cells z", cs.mesh.y_.shape[0] - num_pml_z)
+        sim.setnamed("FDE", "mesh cells z", cs.cell.mesh.y_.shape[0] - num_pml_z)
     sim.setanalysis("number of trial modes", int(num_modes))
     sim.setanalysis("search", "near n")
     sim.setanalysis("use max index", True)
     sim.setanalysis("wavelength", float(cs.env.wl * unit))
     sim.findmodes()
     modes = []
     for j in range(1, num_modes + 1):
         try:
-            mode = Mode(
-                neff=sim.getdata(f"mode{j}", "neff").ravel().item(),
+            mode = _lumerical_fields_to_mode(
                 cs=cs,
-                Ez=sim.getdata(f"mode{j}", "Ex").squeeze()[:-1, :-1],
-                Ex=sim.getdata(f"mode{j}", "Ey").squeeze()[:-1, :-1],
-                Ey=sim.getdata(f"mode{j}", "Ez").squeeze()[:-1, :-1],
-                Hz=sim.getdata(f"mode{j}", "Hx").squeeze()[:-1, :-1],
-                Hx=sim.getdata(f"mode{j}", "Hy").squeeze()[:-1, :-1],
-                Hy=sim.getdata(f"mode{j}", "Hz").squeeze()[:-1, :-1],
+                lneff=sim.getdata(f"mode{j}", "neff"),
+                lEx=sim.getdata(f"mode{j}", "Ex"),
+                lEy=sim.getdata(f"mode{j}", "Ey"),
+                lEz=sim.getdata(f"mode{j}", "Ez"),
+                lHx=sim.getdata(f"mode{j}", "Hx"),
+                lHy=sim.getdata(f"mode{j}", "Hy"),
+                lHz=sim.getdata(f"mode{j}", "Hz"),
             )
         except LumApiError:
             break
         mode = normalize_energy(mode)
         mode = zero_phase(mode)
         modes.append(mode)
 
     return sorted(modes, key=lambda m: np.real(m.neff), reverse=True)
 
 
+def _lumerical_fields_to_mode(cs, lneff, lEx, lEy, lEz, lHx, lHy, lHz):
+    return Mode(
+        cs=cs,
+        neff=lneff.ravel().item(),
+        Ex=lEy.squeeze()[1:, :-1],
+        Ey=lEz.squeeze()[:-1, 1:],
+        Ez=lEx.squeeze()[:-1, :-1],
+        Hx=lHy.squeeze()[:-1, 1:],
+        Hy=lHz.squeeze()[1:, :-1],
+        Hz=lHx.squeeze()[1:, 1:],
+    )
+
+
 def _assert_default_mesh_setting(condition, param_name):
     if not condition:
         raise NotImplementedError(
             f"Setting mesh.{param_name} is currently not supported in the Lumerical Backend. "
             "Please open an issue of submit a PR on GitHub to fix this: ",
             "https://github.com/flaport/meow",
         )
```

### Comparing `meow-sim-0.6.0/meow/fde/tidy3d.py` & `meow-sim-0.6.1/meow/fde/tidy3d.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,30 +8,34 @@
 from packaging import version
 from pydantic import validate_arguments
 from pydantic.types import PositiveFloat, PositiveInt
 from scipy.constants import c
 from tidy3d.plugins.mode.solver import compute_modes as _compute_modes
 
 from ..cross_section import CrossSection
-from ..mode import Mode, Modes, normalize_energy, zero_phase
+from ..mode import Mode, Modes, is_pml_mode, normalize_energy, zero_phase
 
 
 @validate_arguments
 def compute_modes_tidy3d(
     cs: CrossSection,
     num_modes: PositiveInt = 10,
     target_neff: PositiveFloat | None = None,
     precision: Literal["single", "double"] = "double",
+    pml_mode_threshold: float = 1.0,
 ) -> Modes:
-    """compute ``Modes`` for a given ``FdeSpec`` (Tidy3D backend)
+    """compute ``Modes`` for a given ``CrossSection``
 
     Args:
         cs: The ``CrossSection`` to calculate the modes for
         num_modes: Number of modes returned by mode solver.
         target_neff: Guess for initial effective index of the mode.
+        pml_mode_threshold: If the mode has more than `pml_mode_threshold` part of its
+            energy in the PML, it will be removed.
+            default: 1.0 = 100% = no fitering.
     """
 
     if num_modes < 1:
         raise ValueError("You need to request at least 1 mode.")
 
     od = np.zeros_like(cs.nx)  # off diagonal entry
     new_tidy3d = version.parse(tidy3d.__version__) >= version.parse("2.2.0")
@@ -54,15 +58,15 @@
         group_index_step=False,
     )
 
     ((Ex, Ey, Ez), (Hx, Hy, Hz)), neffs = (
         x.squeeze()
         for x in _compute_modes(
             eps_cross=eps_cross,
-            coords=[cs.mesh.x, cs.mesh.y],
+            coords=[cs.cell.mesh.x, cs.cell.mesh.y],
             freq=c / (cs.env.wl * 1e-6),
             mode_spec=mode_spec,
         )
     )
 
     if num_modes == 1:
         modes = [
@@ -91,9 +95,10 @@
                 neff=neffs[i],
             )
             for i in range(num_modes)
         ]
 
     modes = [zero_phase(normalize_energy(mode)) for mode in modes]
     modes = sorted(modes, key=lambda m: float(np.real(m.neff)), reverse=True)
+    modes = [m for m in modes if not is_pml_mode(m, pml_mode_threshold)]
 
     return modes
```

### Comparing `meow-sim-0.6.0/meow/gds_structures.py` & `meow-sim-0.6.1/meow/gds_structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.0/meow/geometries.py` & `meow-sim-0.6.1/meow/geometries.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from typing import Dict, List, Literal, Tuple, Union, cast
 
 import numpy as np
 import shapely.geometry as sg
 from pydantic import Field, validator
 
 from .base_model import BaseModel
-from .mesh import Mesh2d
 
 GEOMETRIES: Dict[str, type] = {}
 
 
 class Geometry(BaseModel):
     type: str = ""
 
@@ -39,23 +38,17 @@
         from trimesh.transformations import rotation_matrix  # fmt: skip
 
         scene = Scene()
         scene.add_geometry(self._trimesh(scale=scale))
         scene.apply_transform(rotation_matrix(-np.pi / 6, (0, 1, 0)))
         return scene.show()
 
-    def _mask2d_single(self, X, Y, z):
+    def _mask2d(self, X, Y, z):
         raise NotImplementedError(f"{self.__class__.__name__!r} cannot be masked.")
 
-    def _mask2d(self, mesh: Mesh2d, z: float):
-        mx = self._mask2d_single(mesh.Xx, mesh.Yx, z)
-        my = self._mask2d_single(mesh.Xy, mesh.Yy, z)
-        mz = self._mask2d_single(mesh.Xz, mesh.Yz, z)
-        return mx, my, mz
-
     def _lumadd(self, sim, material_name, mesh_order, unit=1e-6, xyz="yzx"):
         raise NotImplementedError(
             f"{self.__class__.__name__!r} cannot be added to Lumerical."
         )
 
     def _trimesh(self, **kwargs):
         raise NotImplementedError(f"{self.__class__.__name__!r} cannot be visualized.")
@@ -70,15 +63,15 @@
     x_min: float = Field(description="the minimum x-value of the box")
     x_max: float = Field(description="the maximum x-value of the box")
     y_min: float = Field(description="the minimum y-value of the box")
     y_max: float = Field(description="the maximum y-value of the box")
     z_min: float = Field(description="the minimum z-value of the box")
     z_max: float = Field(description="the maximum z-value of the box")
 
-    def _mask2d_single(self, X, Y, z):
+    def _mask2d(self, X, Y, z):
         if (z < self.z_min) or (self.z_max < z):
             return np.zeros_like(X, dtype=bool)
         return (
             (self.x_min <= X)
             & (X <= self.x_max)
             & (self.y_min <= Y)
             & (Y <= self.y_max)
@@ -140,78 +133,84 @@
     h_min: float = Field(description="the start height of the extrusion")
     h_max: float = Field(description="the end height of the extrusion")
     axis: AxisDirection = Field(
         default="y",
         description="the axis along which the polygon will be extruded ('x', 'y', or 'z').",
     )
 
-    def _mask2d_single(self, X, Y, z):
+    def _mask2d_axis_x(self, X, Y, z):
+        # x, y, z -> y, z, x
         poly = sg.Polygon(self.poly)
-        if self.axis == "x":
-            # x, y, z -> y, z, x
-            y_min, _ = self.poly.min(0)
-            y_max, _ = self.poly.max(0)
-            line = sg.LineString([(y_min, z), (y_max, z)])
-            with warnings.catch_warnings():
-                warnings.filterwarnings(
-                    "ignore", category=RuntimeWarning, module="shapely"
-                )
-                intersections = poly.intersection(line)
-
-            if not isinstance(intersections, sg.MultiLineString):
-                intersection_array = np.asarray(intersections.coords)
-                if not intersection_array.shape[0]:
-                    return np.zeros_like(Y, dtype=bool)
-                intersections = sg.MultiLineString([intersections])
-
-            mask = np.zeros_like(Y, dtype=bool)
-            for intersection in intersections.geoms:
-                intersection = np.asarray(intersection.coords)
-                if not intersection.shape[0]:
-                    return np.zeros_like(X, dtype=bool)
-                (y_min, _), (y_max, _) = intersection
-                y_min, y_max = min(y_min, y_max), max(y_min, y_max)
-                x_min, x_max = min(self.h_min, self.h_max), max(self.h_min, self.h_max)
-                return (x_min <= X) & (X <= x_max) & (y_min <= Y) & (Y <= y_max)
+        y_min, _ = self.poly.min(0)
+        y_max, _ = self.poly.max(0)
+        line = sg.LineString([(y_min, z), (y_max, z)])
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", category=RuntimeWarning, module="shapely")
+            intersections = poly.intersection(line)
+
+        if not isinstance(intersections, sg.MultiLineString):
+            intersection_array = np.asarray(intersections.coords)
+            if not intersection_array.shape[0]:
+                return np.zeros_like(Y, dtype=bool)
+            intersections = sg.MultiLineString([intersections])
+
+        mask = np.zeros_like(Y, dtype=bool)
+        for intersection in intersections.geoms:
+            intersection = np.asarray(intersection.coords)
+            if not intersection.shape[0]:
+                return np.zeros_like(X, dtype=bool)
+            (y_min, _), (y_max, _) = intersection
+            y_min, y_max = min(y_min, y_max), max(y_min, y_max)
+            x_min, x_max = min(self.h_min, self.h_max), max(self.h_min, self.h_max)
+            return (x_min <= X) & (X <= x_max) & (y_min <= Y) & (Y <= y_max)
+
+    def _mask2d_axis_y(self, X, Y, z):
+        # x, y, z -> z, x, y
+        poly = sg.Polygon(self.poly)
+        _, x_min = self.poly.min(0)
+        _, x_max = self.poly.max(0)
+        line = sg.LineString([(z, x_min), (z, x_max)])
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", category=RuntimeWarning, module="shapely")
+            intersections = poly.intersection(line)
+
+        if not isinstance(intersections, sg.MultiLineString):
+            intersection_array = np.asarray(intersections.coords)
+            if not intersection_array.shape[0]:
+                return np.zeros_like(Y, dtype=bool)
+            intersections = sg.MultiLineString([intersections])
+
+        mask = np.zeros_like(Y, dtype=bool)
+        for intersection in intersections.geoms:
+            intersection = np.asarray(intersection.coords)
+            if not intersection.shape[0]:
+                continue
+            (_, x_min), (_, x_max) = intersection
+            x_min, x_max = min(x_min, x_max), max(x_min, x_max)
+            y_min, y_max = min(self.h_min, self.h_max), max(self.h_min, self.h_max)
+            mask |= (x_min <= X) & (X <= x_max) & (y_min <= Y) & (Y <= y_max)
+        return mask
 
+    def _mask2d_axis_z(self, X, Y, z):
+        # x, y, z -> x, y, z
+        poly = sg.Polygon(self.poly)
+        if (z < self.h_min) or (self.h_max < z):
+            return np.zeros_like(X, dtype=bool)
+        return np.asarray(
+            [poly.contains(sg.Point(x, y)) for x, y in zip(X.ravel(), Y.ravel())],
+            dtype=bool,
+        ).reshape(X.shape)
+
+    def _mask2d(self, X, Y, z):
+        if self.axis == "x":
+            return self._mask2d_axis_x(X, Y, z)
         elif self.axis == "y":
-            # x, y, z -> z, x, y
-            _, x_min = self.poly.min(0)
-            _, x_max = self.poly.max(0)
-            line = sg.LineString([(z, x_min), (z, x_max)])
-            with warnings.catch_warnings():
-                warnings.filterwarnings(
-                    "ignore", category=RuntimeWarning, module="shapely"
-                )
-                intersections = poly.intersection(line)
-
-            if not isinstance(intersections, sg.MultiLineString):
-                intersection_array = np.asarray(intersections.coords)
-                if not intersection_array.shape[0]:
-                    return np.zeros_like(Y, dtype=bool)
-                intersections = sg.MultiLineString([intersections])
-
-            mask = np.zeros_like(Y, dtype=bool)
-            for intersection in intersections.geoms:
-                intersection = np.asarray(intersection.coords)
-                if not intersection.shape[0]:
-                    continue
-                (_, x_min), (_, x_max) = intersection
-                x_min, x_max = min(x_min, x_max), max(x_min, x_max)
-                y_min, y_max = min(self.h_min, self.h_max), max(self.h_min, self.h_max)
-                mask |= (x_min <= X) & (X <= x_max) & (y_min <= Y) & (Y <= y_max)
-            return mask
+            return self._mask2d_axis_y(X, Y, z)
         else:
-            # x, y, z -> x, y, z
-            if (z < self.h_min) or (self.h_max < z):
-                return np.zeros_like(X, dtype=bool)
-            return np.asarray(
-                [poly.contains(sg.Point(x, y)) for x, y in zip(X.ravel(), Y.ravel())],
-                dtype=bool,
-            ).reshape(X.shape)
+            return self._mask2d_axis_z(X, Y, z)
 
     def _lumadd(self, sim, material_name, mesh_order, unit=1e-6, xyz="yzx"):
         name = token_hex(4)
 
         if xyz not in ("xyz", "yzx", "zxy"):
             raise ValueError(
                 f"Prism axes should be positively oriented when adding to Lumerical. Got: {xyz!r}"
```

### Comparing `meow-sim-0.6.0/meow/integrate.py` & `meow-sim-0.6.1/meow/integrate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.0/meow/materials.py` & `meow-sim-0.6.1/meow/materials.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.0/meow/mesh.py` & `meow-sim-0.6.1/meow/mesh.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import Literal, Tuple
 
 import numpy as np
 from pydantic import Field
 from pydantic.types import NonNegativeInt
 
-from .base_model import BaseModel
+from .base_model import BaseModel, _array, cached_property
 
 
 class Mesh(BaseModel):
     """[BaseClass] a ``Mesh`` describes how a ``Structure`` is discretized"""
 
 
 class Mesh2d(Mesh):
@@ -48,66 +48,88 @@
         ),
     )
     num_pml: Tuple[NonNegativeInt, NonNegativeInt] = Field(
         default=(0, 0),
         description="Number of standard pml layers to add in the two tangential axes.",
     )
 
-    @property
+    @cached_property
     def dx(self):
         """x-coordinate mesh step (Hz locations, i.e. center of the 2D cell)"""
-        return self.x[1:] - self.x[:-1]
+        return (self.x[1:] - self.x[:-1]).view(_array)
 
-    @property
+    @cached_property
     def dy(self):
         """y-coordinate mesh step (Hz locations, i.e. center of the 2D cell)"""
-        return self.y[1:] - self.y[:-1]
+        return (self.y[1:] - self.y[:-1]).view(_array)
 
-    @property
+    @cached_property
     def x_(self):
-        """x-coordinates of the mesh (Hz locations, i.e. center of the 2D cell)"""
-        return 0.5 * (self.x[1:] + self.x[:-1])
+        """x-coordinate mesh step (Hz locations, i.e. center of the 2D cell)"""
+        return 0.5 * (self.x[1:] + self.x[:-1]).view(_array)
 
-    @property
+    @cached_property
     def y_(self):
-        """y-coordinates of the mesh (Hz locations, i.e. center of the 2D cell)"""
-        return 0.5 * (self.y[1:] + self.y[:-1])
+        """y-coordinate mesh step (Hz locations, i.e. center of the 2D cell)"""
+        return 0.5 * (self.y[1:] + self.y[:-1]).view(_array)
+
+    @cached_property
+    def x_full(self):
+        return (
+            np.stack([self.x[:-1] + self.dx / 4, self.x[:-1] + 3 * self.dx / 4], 1)
+            .ravel()
+            .view(_array)
+        )
+
+    @cached_property
+    def y_full(self):
+        return (
+            np.stack([self.y[:-1] + self.dy / 4, self.y[:-1] + 3 * self.dy / 4], 1)
+            .ravel()
+            .view(_array)
+        )
+
+    @cached_property
+    def XY_full(self):
+        Y_full, X_full = np.meshgrid(self.y_full, self.x_full)
+        return X_full.view(_array), Y_full.view(_array)
 
     @property
-    def X(self):
-        return np.meshgrid(self.y_, self.x_)[1]
+    def X_full(self):
+        return self.XY_full[0].view(_array)
 
     @property
-    def Y(self):
-        return np.meshgrid(self.y_, self.x_)[0]
+    def Y_full(self):
+        return self.XY_full[1].view(_array)
 
     @property
     def Xx(self):
-        return np.meshgrid(self.y[:-1], self.x_)[1]
+        return self.X_full[1::2, ::2].view(_array)
 
     @property
     def Yx(self):
-        return np.meshgrid(self.y[:-1], self.x_)[0]
+        return self.Y_full[1::2, ::2].view(_array)
 
     @property
     def Xy(self):
-        return np.meshgrid(self.y_, self.x[:-1])[1]
+        return self.X_full[::2, 1::2].view(_array)
 
     @property
     def Yy(self):
-        return np.meshgrid(self.y_, self.x[:-1])[0]
+        return self.Y_full[::2, 1::2].view(_array)
 
     @property
     def Xz(self):
-        return np.meshgrid(self.y[:-1], self.x[:-1])[1]
+        return self.X_full[::2, ::2].view(_array)
 
     @property
     def Yz(self):
-        return np.meshgrid(self.y[:-1], self.x[:-1])[0]
+        return self.Y_full[::2, ::2].view(_array)
 
     def __eq__(self, other):
-        try:
-            x_eq = ((self.x - other.x) < 1e-6).all()
-            y_eq = ((self.y - other.y) < 1e-6).all()
-        except Exception:
-            return False
-        return x_eq and y_eq
+        eq = True
+        for k, v in self.dict().items():
+            if isinstance(v, np.ndarray):
+                eq &= ((v - getattr(other, k)) < 1e-6).all()
+            else:
+                eq &= v == getattr(other, k)
+        return eq
```

### Comparing `meow-sim-0.6.0/meow/mode.py` & `meow-sim-0.6.1/meow/mode.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,25 +75,25 @@
 
     @cached_property
     def A(self):
         """mode area"""
         vecE = np.stack([self.Ex, self.Ey, self.Ez], axis=-1)
         E_sq = norm(vecE, axis=-1, ord=2)
         E_qu = E_sq**2
-        x = self.cs.mesh.x_
-        y = self.cs.mesh.y_
+        x = self.cs.cell.mesh.x_
+        y = self.cs.cell.mesh.y_
         return np.float_(integrate_2d(x, y, E_sq) ** 2 / integrate_2d(x, y, E_qu))
 
     @property
     def env(self):
         return self.cs.env
 
     @property
     def mesh(self):
-        return self.cs.mesh
+        return self.cs.cell.mesh
 
     @property
     def cell(self):
         return self.cs.cell
 
     def _visualize(
         self,
@@ -150,36 +150,38 @@
                 f"Invalid field {field!r}. Valid fields: {', '.join(valid_fields)}."
             )
 
         if ax is None:
             ax = plt.gca()
         plt.sca(ax)
 
-        x, y = "x", "y"  # currently only propagation in z supported, see Mesh2d
-        c = field[-1]
         if n_cmap is None:
+            # little bit lighter colored than the one in cs._visualize:
             n_cmap = colors.LinearSegmentedColormap.from_list(
                 name="c_cmap", colors=["#ffffff", "#c1d9ed"]
             )
+        self.cs._visualize(ax=ax, n_cmap=n_cmap, cbar=False, show=False)
+
+        x, y = "x", "y"  # currently only propagation in z supported, see Mesh2d
+        c = {"Ex": "x", "Ey": "y", "Ez": "z", "Hx": "y", "Hy": "x", "Hz": "z"}[field]
         if mode_cmap is None:
             mode_cmap = "inferno"
         X = getattr(self.mesh, f"X{c}")
         Y = getattr(self.mesh, f"Y{c}")
         mode = operation(getattr(self, field))
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=UserWarning)
             levels = np.linspace(mode.min(), mode.max(), num_levels + 1)[1:]
             plt.contour(X, Y, mode, cmap=mode_cmap, levels=levels)  # fmt: skip
+            # plt.pcolormesh(X, Y, mode, cmap=mode_cmap, alpha=0.5) #, levels=levels)  # fmt: skip
         divider = make_axes_locatable(ax)
         cax = divider.append_axes("right", size="5%", pad=0.05)
         plt.colorbar(cax=cax)
         plt.sca(ax)
 
-        n = np.real(getattr(self.cs, f"n{c}"))
-        plt.pcolormesh(X, Y, n, cmap=n_cmap)
         plt.xlabel(x)
         plt.ylabel(y)
         plt.grid(True, alpha=0.4)
         if title is None:
             plt.title(f"{title_prefix}{field} [neff={float(np.real(self.neff)):.6f}]")
         else:
             plt.title(f"{title_prefix}{title}")
@@ -212,15 +214,15 @@
             Hx=self.Hx + other.Hx,
             Hy=self.Hy + other.Hy,
             Hz=self.Hz + other.Hz,
         )
         return new_mode
 
     def __mul__(self, other):
-        if not isinstance(other, (float, complex)):
+        if not isinstance(other, (float, np.floating, complex, int, np.integer)):
             raise TypeError(
                 f"unsupported operand type(s) for *: 'Mode' and '{type(other).__name__}'"
             )
         new_mode = Mode(
             neff=self.neff,
             cs=self.cs,
             Ex=self.Ex * other,
@@ -231,26 +233,26 @@
             Hz=self.Hz * other,
         )
         return new_mode
 
     __rmul__ = __mul__
 
     def __truediv__(self, other):
-        if not isinstance(other, (float, complex)):
+        if not isinstance(other, (float, np.floating, complex, int, np.integer)):
             raise TypeError(
                 f"unsupported operand type(s) for /: 'Mode' and '{type(other).__name__}'"
             )
         return self * (1 / other)
 
     def __sub__(self, other):
         if not isinstance(other, Mode):
             raise TypeError(
                 f"unsupported operand type(s) for -: 'Mode' and '{type(other).__name__}'"
             )
-        return self + other * (-1)
+        return self + other * (-1.0)
 
 
 Modes = List[Mode]
 
 
 def zero_phase(mode: Mode) -> Mode:
     """normalize (zero out) the phase of a `Mode`"""
@@ -391,26 +393,41 @@
         Ez=mode.Ez / e,
         Hx=mode.Hx / h,
         Hy=mode.Hy / h,
         Hz=mode.Hz / h,
     )
 
 
-def is_pml_mode(mode, threshold_factor=0.2):
+def is_pml_mode(mode, threshold):
+    """check whether a mode can be considered a PML mode.
+
+    Args:
+        mode: the mode to classify as PML mode or not.
+        pml_mode_threshold: If the mode has more than `pml_mode_threshold` part of its
+            energy in the PML, it will be removed.
+
+    Returns:
+        bool: whether the mode is a PML mode or not
+    """
+    threshold = min(max(threshold, 0.0), 1.0)
+    if threshold > 0.999:
+        return False
     numx, numy = mode.cell.mesh.num_pml
     ed = energy_density(mode)
     m, n = ed.shape
     lft = ed[:numx, :]
     rgt = ed[m - numx :, :]
     top = ed[numx : m - numx, n:numy]
     btm = ed[numx : m - numx, n - numy :]
     rest = ed[numx : m - numx, numy : n - numy]
     pml_sum = lft.sum() + rgt.sum() + top.sum() + btm.sum()
     rest_sum = rest.sum()
-    is_pml = pml_sum > threshold_factor * rest_sum
+    # probably propper integration considering
+    # the size of the mesh cells would be better here
+    is_pml = pml_sum > threshold * (rest_sum + pml_sum)
     return is_pml
 
 
 def te_fraction(mode: Mode) -> float:
     """the TE polarization fraction of the `Mode`"""
     epsx = mode.cs.nx**2
     e = np.sum(0.5 * eps0 * epsx * np.abs(mode.Ex) ** 2)
```

### Comparing `meow-sim-0.6.0/meow/structures.py` & `meow-sim-0.6.1/meow/structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.0/meow/visualize.py` & `meow-sim-0.6.1/meow/visualize.py`

 * *Files 3% similar despite different names*

```diff
@@ -184,60 +184,65 @@
         x, y = obj  # type: ignore
         return True
     except Exception:
         return False
 
 
 def _figsize_visualize_mode(cs, W0):
-    x_min, x_max = cs.mesh.x.min(), cs.mesh.x.max()
-    y_min, y_max = cs.mesh.y.min(), cs.mesh.y.max()
+    x_min, x_max = cs.cell.mesh.x.min(), cs.cell.mesh.x.max()
+    y_min, y_max = cs.cell.mesh.y.min(), cs.cell.mesh.y.max()
     delta_x = x_max - x_min
     delta_y = y_max - y_min
     aspect = delta_y / delta_x
-    W0 = 6.4
     W, H = W0 + 1, W0 * aspect + 1
     return W, H
 
 
 def _visualize_modes(
     modes,
     n_cmap=None,
     mode_cmap=None,
     num_levels=8,
     operation=lambda x: np.abs(x) ** 2,
     show=True,
     plot_width=6.4,
+    fields=("Ex", "Hx"),
+    ax=None,
 ):
     import matplotlib.pyplot as plt  # fmt: skip
 
     num_modes = len(modes)
     cs = modes[0].cs
     W, H = _figsize_visualize_mode(cs, plot_width)
 
-    fig, ax = plt.subplots(
-        num_modes,
-        2,
-        figsize=(2 * W, num_modes * H),
-        sharex=True,
-        sharey=True,
-        squeeze=False,
-    )
+    if ax is None:
+        fig, ax = plt.subplots(
+            num_modes,
+            2,
+            figsize=(2 * W, num_modes * H),
+            sharex=True,
+            sharey=True,
+            squeeze=False,
+        )
+    else:
+        fig = None
     for i, m in enumerate(modes):
         m._visualize(
             title=None,
             title_prefix=f"m{i}: ",
-            fields=["Ex", "Hx"],
+            fields=list(fields),
             ax=ax[i],
             n_cmap=n_cmap,
             mode_cmap=mode_cmap,
             num_levels=num_levels,
             operation=operation,
             show=False,
         )
-    fig.subplots_adjust(hspace=0, wspace=2 / (2 * W))
+    if fig is not None:
+        fig.subplots_adjust(hspace=0, wspace=2 / (2 * W))
     if show:
         plt.show()
 
 
 def _visualize_base_model(obj, **kwargs):
     return obj._visualize(**kwargs)
```

### Comparing `meow-sim-0.6.0/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.6.1/meow_sim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.6.0
+Version: 0.6.1
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.6.0/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.6.1/meow_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.0/pyproject.toml` & `meow-sim-0.6.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.6.0"
+version = "0.6.1"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 [project.optional-dependencies]
 min = ["meow-sim"]
 vis = ["matplotlib", "trimesh[easy]"]
 jax = ["jax", "jaxlib"]
 klu = ["klujax>0.1.2"]
 ipy = ["ipykernel", "ipywidgets", "ipympl", "nbstripout", "tqdm"]
 gds = ["gdsfactory>6.27.0", "klayout>0.28.2"]
-dev = ["bump2version", "nbstripout", "pre-commit", "black", "sphinx", "autodoc-pydantic", "myst-nb>0.17.1", "jupyter-book"]
+dev = ["bump2version", "nbstripout", "pre-commit", "black[jupyter]", "autoimport", "isort", "sphinx", "autodoc-pydantic", "myst-nb>0.17.1", "jupyter-book", "papermill"]
 full = ["meow-sim[vis,klu,jax,ipy,gds]"]
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["meow*"]
 exclude = []
 namespaces = true
```

### Comparing `meow-sim-0.6.0/tests/test_deserialization.py` & `meow-sim-0.6.1/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.0/tests/test_mode_operators.py` & `meow-sim-0.6.1/tests/test_mode_operators.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.0/tests/test_nbs.py` & `meow-sim-0.6.1/tests/test_nbs.py`

 * *Files identical despite different names*

