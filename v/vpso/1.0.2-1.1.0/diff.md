# Comparing `tmp/vpso-1.0.2.tar.gz` & `tmp/vpso-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vpso-1.0.2.tar", last modified: Wed Jun 14 09:06:32 2023, max compression
+gzip compressed data, was "vpso-1.1.0.tar", last modified: Sun Jun 18 08:23:23 2023, max compression
```

## Comparing `vpso-1.0.2.tar` & `vpso-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 09:06:32.213582 vpso-1.0.2/
--rw-rw-rw-   0        0        0     1093 2023-06-06 07:34:41.000000 vpso-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     3575 2023-06-14 09:06:32.212581 vpso-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2872 2023-06-11 14:02:36.000000 vpso-1.0.2/README.md
--rw-rw-rw-   0        0        0      977 2023-06-14 09:02:19.000000 vpso-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 09:06:32.213582 vpso-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-14 09:06:32.152070 vpso-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-14 09:06:32.178837 vpso-1.0.2/src/vpso/
--rw-rw-rw-   0        0        0       50 2023-06-06 08:52:06.000000 vpso-1.0.2/src/vpso/__init__.py
--rw-rw-rw-   0        0        0     5945 2023-06-13 22:13:58.000000 vpso-1.0.2/src/vpso/adaptation.py
--rw-rw-rw-   0        0        0     5423 2023-06-13 20:32:15.000000 vpso-1.0.2/src/vpso/ask_and_tell.py
--rw-rw-rw-   0        0        0     5149 2023-06-13 15:20:00.000000 vpso-1.0.2/src/vpso/initialization.py
--rw-rw-rw-   0        0        0     4367 2023-06-13 22:06:07.000000 vpso-1.0.2/src/vpso/jit.py
--rw-rw-rw-   0        0        0     6709 2023-06-13 22:05:05.000000 vpso-1.0.2/src/vpso/math.py
--rw-rw-rw-   0        0        0     3752 2023-06-13 20:32:15.000000 vpso-1.0.2/src/vpso/mutation.py
--rw-rw-rw-   0        0        0     3270 2023-06-13 20:32:15.000000 vpso-1.0.2/src/vpso/reparation.py
--rw-rw-rw-   0        0        0     5513 2023-06-13 20:32:15.000000 vpso-1.0.2/src/vpso/termination.py
--rw-rw-rw-   0        0        0      295 2023-06-12 15:05:01.000000 vpso-1.0.2/src/vpso/typing.py
--rw-rw-rw-   0        0        0     7929 2023-06-13 15:19:02.000000 vpso-1.0.2/src/vpso/vpso.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:06:32.190663 vpso-1.0.2/src/vpso.egg-info/
--rw-rw-rw-   0        0        0     3575 2023-06-14 09:06:32.000000 vpso-1.0.2/src/vpso.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      569 2023-06-14 09:06:32.000000 vpso-1.0.2/src/vpso.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 09:06:32.000000 vpso-1.0.2/src/vpso.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-06-14 09:06:32.000000 vpso-1.0.2/src/vpso.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-14 09:06:32.000000 vpso-1.0.2/src/vpso.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-14 09:06:32.210594 vpso-1.0.2/tests/
--rw-rw-rw-   0        0        0     4314 2023-06-12 15:49:15.000000 vpso-1.0.2/tests/test_adaptation.py
--rw-rw-rw-   0        0        0     1201 2023-06-10 15:53:49.000000 vpso-1.0.2/tests/test_initialization.py
--rw-rw-rw-   0        0        0     3467 2023-06-13 22:08:14.000000 vpso-1.0.2/tests/test_math.py
--rw-rw-rw-   0        0        0     3669 2023-06-10 15:56:14.000000 vpso-1.0.2/tests/test_mutation.py
--rw-rw-rw-   0        0        0     2119 2023-06-13 20:45:53.000000 vpso-1.0.2/tests/test_numerical.py
--rw-rw-rw-   0        0        0     3211 2023-06-10 15:56:23.000000 vpso-1.0.2/tests/test_reparation.py
+drwxrwxrwx   0        0        0        0 2023-06-18 08:23:23.932776 vpso-1.1.0/
+-rw-rw-rw-   0        0        0     1093 2023-06-06 07:34:41.000000 vpso-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3575 2023-06-18 08:23:23.931776 vpso-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2872 2023-06-11 14:02:36.000000 vpso-1.1.0/README.md
+-rw-rw-rw-   0        0        0      977 2023-06-18 07:38:18.000000 vpso-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-18 08:23:23.932776 vpso-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-18 08:23:23.893828 vpso-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-18 08:23:23.910774 vpso-1.1.0/src/vpso/
+-rw-rw-rw-   0        0        0       50 2023-06-06 08:52:06.000000 vpso-1.1.0/src/vpso/__init__.py
+-rw-rw-rw-   0        0        0     4396 2023-06-18 08:10:29.000000 vpso-1.1.0/src/vpso/adaptation.py
+-rw-rw-rw-   0        0        0     6066 2023-06-18 08:08:37.000000 vpso-1.1.0/src/vpso/ask_and_tell.py
+-rw-rw-rw-   0        0        0     5178 2023-06-18 08:09:33.000000 vpso-1.1.0/src/vpso/initialization.py
+-rw-rw-rw-   0        0        0     7815 2023-06-18 07:14:19.000000 vpso-1.1.0/src/vpso/math.py
+-rw-rw-rw-   0        0        0     4496 2023-06-18 08:12:30.000000 vpso-1.1.0/src/vpso/mutation.py
+-rw-rw-rw-   0        0        0     3898 2023-06-18 08:08:51.000000 vpso-1.1.0/src/vpso/reparation.py
+-rw-rw-rw-   0        0        0     6822 2023-06-18 08:22:24.000000 vpso-1.1.0/src/vpso/termination.py
+-rw-rw-rw-   0        0        0      302 2023-06-18 08:09:11.000000 vpso-1.1.0/src/vpso/typing.py
+-rw-rw-rw-   0        0        0     7396 2023-06-18 08:20:41.000000 vpso-1.1.0/src/vpso/vpso.py
+drwxrwxrwx   0        0        0        0 2023-06-18 08:23:23.917777 vpso-1.1.0/src/vpso.egg-info/
+-rw-rw-rw-   0        0        0     3575 2023-06-18 08:23:23.000000 vpso-1.1.0/src/vpso.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2023-06-18 08:23:23.000000 vpso-1.1.0/src/vpso.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 08:23:23.000000 vpso-1.1.0/src/vpso.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-18 08:23:23.000000 vpso-1.1.0/src/vpso.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-18 08:23:23.000000 vpso-1.1.0/src/vpso.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 08:23:23.930782 vpso-1.1.0/tests/
+-rw-rw-rw-   0        0        0     4264 2023-06-18 07:52:24.000000 vpso-1.1.0/tests/test_adaptation.py
+-rw-rw-rw-   0        0        0     1201 2023-06-10 15:53:49.000000 vpso-1.1.0/tests/test_initialization.py
+-rw-rw-rw-   0        0        0     3467 2023-06-13 22:08:14.000000 vpso-1.1.0/tests/test_math.py
+-rw-rw-rw-   0        0        0     3669 2023-06-10 15:56:14.000000 vpso-1.1.0/tests/test_mutation.py
+-rw-rw-rw-   0        0        0     2119 2023-06-13 20:45:53.000000 vpso-1.1.0/tests/test_numerical.py
+-rw-rw-rw-   0        0        0     3211 2023-06-10 15:56:23.000000 vpso-1.1.0/tests/test_reparation.py
```

### Comparing `vpso-1.0.2/LICENSE` & `vpso-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vpso-1.0.2/PKG-INFO` & `vpso-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vpso
-Version: 1.0.2
+Version: 1.1.0
 Summary: Vectorized Particle Swarm Optimization
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/vectorized-particle-swarm
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/vectorized-particle-swarm/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vpso-1.0.2/README.md` & `vpso-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `vpso-1.0.2/pyproject.toml` & `vpso-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vpso"
-version = "1.0.2"
+version = "1.1.0"
 authors = [
   { name="Filippo Airaldi", email="filippoairaldi@gmail.com" },
 ]
 description = "Vectorized Particle Swarm Optimization"
 readme = "README.md"
 requires-python = ">=3.9"
 license = { text = "MIT" }
```

### Comparing `vpso-1.0.2/src/vpso/ask_and_tell.py` & `vpso-1.1.0/src/vpso/ask_and_tell.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,39 @@
-import logging
-
+import numba as nb
 import numpy as np
 
-from vpso.jit import jit
 from vpso.math import pso_equation
 from vpso.mutation import mutate
 from vpso.reparation import repair_out_of_bounds
 from vpso.typing import Array1d, Array2d, Array3d
 
 
-@jit()
+@nb.njit(
+    nb.types.UniTuple(nb.float64[:, :, :], 2)(
+        nb.float64[:, :, :],  # x
+        nb.float64[:, :, :],  # px
+        nb.float64[:, :],  # pf
+        nb.float64[:, :, :],  # sx
+        nb.float64[:, :, :],  # v
+        nb.float64[:, :, :],  # v_max
+        nb.float64[:, :, :],  # lb
+        nb.float64[:, :, :],  # ub
+        nb.int32,  # nvec
+        nb.int32,  # dim
+        nb.float64[:, :, :],  # w
+        nb.float64[:, :, :],  # c1
+        nb.float64[:, :, :],  # c2
+        nb.int32,  # iters
+        nb.bool_,  # perturb_best
+        nb.float64,  # mutation_prob
+        nb.types.NumPyRandomGeneratorType("NumPyRandomGeneratorType"),
+    ),
+    cache=True,
+    nogil=True,
+)
 def generate_offsprings(
     x: Array3d,
     px: Array3d,
     pf: Array2d,
     sx: Array3d,
     v: Array3d,
     v_max: Array3d,
@@ -83,15 +103,24 @@
         x, x_new, v_new, px, sx, v, v_max, lb, ub, w, c1, c2, repair_iters, np_random
     )
     if perturb_best:
         mutate(x_new, px, pf, lb, ub, nvec, dim, mutation_prob, np_random)
     return x_new, v_new
 
 
-@jit()
+@nb.njit(
+    nb.types.Tuple((nb.float64[:, :, :], nb.float64[:, :]))(
+        nb.float64[:, :, :],  # x
+        nb.float64[:, :],  # f
+        nb.float64[:, :, :],  # px
+        nb.float64[:, :],  # pf
+    ),
+    cache=True,
+    nogil=True,
+)
 def advance_population(
     x: Array3d, f: Array2d, px: Array3d, pf: Array2d
 ) -> tuple[Array3d, Array2d]:
     """Advances the population by replacing the particles with better positions.
 
     Parameters
     ----------
@@ -113,41 +142,32 @@
     """
     improvement_mask = f < pf
     px = np.where(improvement_mask[:, :, np.newaxis], x, px)
     pf = np.where(improvement_mask, f, pf)
     return px, pf
 
 
-def get_best(
-    px: Array3d, pf: Array2d, nvec: int, logger: logging.Logger, iter: int
-) -> tuple[Array3d, Array1d]:
+def get_best(px: Array3d, pf: Array2d, nvec: int) -> tuple[Array3d, Array1d]:
     """Returns the best particle and its value for each problem.
 
     Parameters
     ----------
     px : 3d array
         Best positions of the particles so far. An array of shape `(N, M, d)`, where `N`
         is the number of vectorized problems to solve simultaneously, `M` is the number
         of particles in the swarm, and `d` is the dimension of the search space.
     pf : 2d array
         Best values of the particles so far. An array of shape `(N, M)`.
     nvec : int
         Number of vectorized problems.
-    logger : logging.Logger
-        Logger object.
-    iter : int
-        Current iteration. Only used for logging.
 
     Returns
     -------
     tuple of 3d and 1d arrays
         The best particle and its value for each problem with shape `(N, 1, d)` and
         `(N,)`, respectively.
     """
     idx = np.arange(nvec)
     k = pf.argmin(1)
     sx = px[idx, np.newaxis, k]  # (social/global) best particle
     sf = pf[idx, k]  # (social/global) best value
-
-    if logger.level <= logging.INFO:
-        logger.info("best values at iteration %i ∈ [%e, %e]", iter, sf.min(), sf.max())
     return sx, sf
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `vpso-1.0.2/src/vpso/initialization.py` & `vpso-1.1.0/src/vpso/initialization.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,29 +73,29 @@
 
     Returns
     -------
     tuple of 3d and 1d arrays
         Returns the `lb`, `ub`, `nvec`, `dim`, `max_velocity_rate`, `w`, `c1`, `c2`,
         `ftol`, `xtol`, and `patience`.
     """
-    lb = np.expand_dims(lb, 1).astype(float, copy=True)  # add swarm dimension
-    ub = np.expand_dims(ub, 1).astype(float, copy=True)  # add swarm dimension
+    lb = lb[:, np.newaxis].astype(float, copy=False)  # add swarm dimension
+    ub = ub[:, np.newaxis].astype(float, copy=False)  # add swarm dimension
     nvec, _, dim = lb.shape
     return (
         lb,
         ub,
         nvec,
         dim,
-        _asarray(max_velocity_rate, nvec, float, 3),
-        _asarray(w, nvec, float, 3),
-        _asarray(c1, nvec, float, 3),
-        _asarray(c2, nvec, float, 3),
-        _asarray(ftol, nvec, float, 1),
-        _asarray(xtol, nvec, float, 1),
-        _asarray(patience, nvec, int, 1),
+        _asarray(max_velocity_rate, nvec, np.float64, 3),
+        _asarray(w, nvec, np.float64, 3),
+        _asarray(c1, nvec, np.float64, 3),
+        _asarray(c2, nvec, np.float64, 3),
+        _asarray(ftol, nvec, np.float64, 1),
+        _asarray(xtol, nvec, np.float64, 1),
+        _asarray(patience, nvec, np.int32, 1),
     )
 
 
 def initialize_particles(
     nvec: int,
     swarmsize: int,
     dim: int,
```

### Comparing `vpso-1.0.2/src/vpso/math.py` & `vpso-1.1.0/src/vpso/math.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from typing import Literal
 
+import numba as nb
 import numpy as np
-from numba import prange
 
-from vpso.jit import jit
 from vpso.typing import Array2d, Array3d
 
 
-@jit()
+@nb.njit(
+    nb.float64[:, :](nb.float64[:, :], nb.float64[:, :], nb.types.unicode_type),
+    cache=True,
+    nogil=True,
+)
 def cdist_func(
     x: Array2d, y: Array2d, type: Literal["euclidean", "sqeuclidean"]
 ) -> Array2d:
     """Computes the distance matrix for 2D arrays `x` and `y`.
 
     Parameters
     ----------
@@ -34,15 +37,19 @@
     if type == "euclidean":
         return np.sqrt(D)
     if type == "sqeuclidean":
         return D
     raise ValueError(f"unknown cdist type: {type}")
 
 
-@jit()
+@nb.njit(
+    nb.float64[:, :](nb.float64[:, :], nb.types.unicode_type),
+    cache=True,
+    nogil=True,
+)
 def pdist_func(x: Array2d, type: Literal["euclidean", "sqeuclidean"]) -> Array2d:
     """Computes the pairwise distance matrix of the elements in the 2D array `x`.
 
     Parameters
     ----------
     x : 2d array
         A 2D array of shape `(N, d)`.
@@ -61,15 +68,22 @@
     if type == "euclidean":
         return np.sqrt(D)
     if type == "sqeuclidean":
         return D
     raise ValueError(f"unknown pdist type: {type}")
 
 
-@jit(parallel=True)
+@nb.njit(
+    nb.float64[:, :, :](
+        nb.float64[:, :, :], nb.float64[:, :, :], nb.types.unicode_type
+    ),
+    cache=True,
+    nogil=True,
+    parallel=True,
+)
 def batch_cdist(
     X: Array3d, Y: Array3d, type: Literal["euclidean", "sqeuclidean"]
 ) -> Array3d:
     """Computes the distance matrices for 3D arrays.
 
     Parameters
     ----------
@@ -86,20 +100,25 @@
     3d array
         Distance matrices between each of the `(M, d)` and `(K, d)` matrices, where `d`
         is assumed to be the axis over which the distance is computed. The output has
         thus shape (N, M, K).
     """
     B, N, _ = X.shape
     out = np.empty((B, N, Y.shape[1]), dtype=X.dtype)
-    for i in prange(B):
+    for i in nb.prange(B):
         out[i] = cdist_func(X[i], Y[i], type)
     return out
 
 
-@jit(parallel=True)
+@nb.njit(
+    nb.float64[:, :, :](nb.float64[:, :, :], nb.types.unicode_type),
+    cache=True,
+    nogil=True,
+    parallel=True,
+)
 def batch_pdist(X: Array3d, type: Literal["euclidean", "sqeuclidean"]) -> Array3d:
     """Computes the pairwise distance matrices for the entries of a 3D array.
 
     Parameters
     ----------
     X : 3d array
         An array of shape `(N, M, d)`.
@@ -112,20 +131,27 @@
     3d array
         Distance matrix of shape `(N, M, M)` between each pair of entries of
         the `(M, d)` matrices, where `d` is assumed to be the axis over which the
         distance is computed.
     """
     B, N, _ = X.shape
     out = np.empty((B, N, N), dtype=X.dtype)
-    for i in prange(B):
+    for i in nb.prange(B):
         out[i] = pdist_func(X[i], type)
     return out
 
 
-@jit(parallel=True)
+@nb.njit(
+    nb.types.UniTuple(nb.float64[:, :, :], 2)(
+        nb.float64[:, :, :], nb.float64[:, :, :], nb.types.unicode_type
+    ),
+    cache=True,
+    nogil=True,
+    parallel=True,
+)
 def batch_cdist_and_pdist(
     X: Array3d, Y: Array3d, type: Literal["euclidean", "sqeuclidean"]
 ) -> tuple[Array3d, Array3d]:
     """Computes the distance matrices between the 3D arrays `X` and `Y`, as well as the
     pairwise distance matrices for the entries of `X`.
 
     Parameters
@@ -143,21 +169,35 @@
     tuple of 3d arrays
         Returns both distance matrices between `X` and `Y` and `X` itself. See
         `batch_cdist` and `batch_pdist` for more details.
     """
     B, N, _ = X.shape
     out_c = np.empty((B, N, Y.shape[1]), dtype=X.dtype)
     out_p = np.empty((B, N, N), dtype=X.dtype)
-    for i in prange(B):
+    for i in nb.prange(B):
         out_c[i] = cdist_func(X[i], Y[i], type)
         out_p[i] = pdist_func(X[i], type)
     return out_c, out_p
 
 
-@jit()
+@nb.njit(
+    nb.types.UniTuple(nb.float64[:, :, :], 2)(
+        nb.float64[:, :, :],  # x
+        nb.float64[:, :, :],  # px
+        nb.float64[:, :, :],  # sx
+        nb.float64[:, :, :],  # v
+        nb.float64[:, :, :],  # v_max
+        nb.float64[:, :, :],  # w
+        nb.float64[:, :, :],  # c1
+        nb.float64[:, :, :],  # c2
+        nb.types.NumPyRandomGeneratorType("NumPyRandomGeneratorType"),
+    ),
+    cache=True,
+    nogil=True,
+)
 def pso_equation(
     x: Array3d,
     px: Array3d,
     sx: Array3d,
     v: Array3d,
     v_max: Array3d,
     w: Array3d,
```

### Comparing `vpso-1.0.2/src/vpso/mutation.py` & `vpso-1.1.0/src/vpso/mutation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,26 @@
+import numba as nb
 import numpy as np
 
-from vpso.jit import _int, jit
 from vpso.typing import Array2d, Array3d
 
 
-@jit()
+@nb.njit(
+    nb.float64[:, :](
+        nb.float64[:, :],  # x_best
+        nb.bool_[:, :],  # mutation_mask
+        nb.float64[:, :],  # lb
+        nb.float64[:, :],  # ub
+        nb.int32,  # nvec
+        nb.int32,  # dim
+        nb.types.NumPyRandomGeneratorType("NumPyRandomGeneratorType"),
+    ),
+    cache=True,
+    nogil=True,
+)
 def polynomial_mutation(
     x_best: Array2d,
     mutation_mask: Array2d,
     lb: Array2d,
     ub: Array2d,
     nvec: int,
     dim: int,
@@ -36,27 +48,41 @@
 
     Returns
     -------
     2d array
         Modified best particles. An array of shape `(nvec, dim)`.
     """
     domain = ub - lb
-    eta = np_random.uniform(6.0, 31.0, (nvec, _int(1)))
+    eta = np_random.uniform(6.0, 31.0, (nvec, np.int32(1)))
     mut_pow = 1.0 / eta
     xy1 = np.power((ub - x_best) / domain, eta)
     xy2 = np.power((x_best - lb) / domain, eta)
     R = np_random.random((nvec, dim))
     val1 = np.power(2.0 * R + (1.0 - 2.0 * R) * xy1, mut_pow)
     val2 = np.power(2.0 * (1.0 - R) + 2.0 * (R - 0.5) * xy2, mut_pow)
     deltaq = np.where(R <= 0.5, val1 - 1.0, 1.0 - val2)
 
     return np.where(mutation_mask, x_best + deltaq * domain, x_best).clip(lb, ub)
 
 
-@jit()
+@nb.njit(
+    nb.types.void(
+        nb.float64[:, :, :],  # x
+        nb.float64[:, :, :],  # px
+        nb.float64[:, :],  # pf
+        nb.float64[:, :, :],  # lb
+        nb.float64[:, :, :],  # ub
+        nb.int32,  # nvec
+        nb.int32,  # dim
+        nb.float64,  # mutation_prob
+        nb.types.NumPyRandomGeneratorType("NumPyRandomGeneratorType"),
+    ),
+    cache=True,
+    nogil=True,
+)
 def mutate(
     x: Array3d,
     px: Array3d,
     pf: Array2d,
     lb: Array3d,
     ub: Array3d,
     nvec: int,
@@ -88,15 +114,15 @@
     mutation_prob : float
         Probability of applying the mutation.
     np_random : np.random.Generator
         Random number generator.
     """
     # get the mutation mask for each vectorized problem, and for each dimension
     mutation_mask = np.logical_and(
-        np_random.random((nvec, _int(1))) <= mutation_prob,
+        np_random.random((nvec, np.int32(1))) <= mutation_prob,
         np_random.random((nvec, dim)) <= min(0.5, 1 / dim),
     )
     if not mutation_mask.any():
         return
 
     # pick the best particle from each problem as target for mutation
     k = pf.argmin(1)
```

### Comparing `vpso-1.0.2/src/vpso/reparation.py` & `vpso-1.1.0/src/vpso/reparation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,34 @@
+import numba as nb
 import numpy as np
 
-from vpso.jit import jit
 from vpso.math import pso_equation
 from vpso.typing import Array3d
 
 
-@jit()
+@nb.njit(
+    nb.types.UniTuple(nb.float64[:, :, :], 2)(
+        nb.float64[:, :, :],  # x
+        nb.float64[:, :, :],  # x_new
+        nb.float64[:, :, :],  # v_new
+        nb.float64[:, :, :],  # px
+        nb.float64[:, :, :],  # sx
+        nb.float64[:, :, :],  # v
+        nb.float64[:, :, :],  # v_max
+        nb.float64[:, :, :],  # lb
+        nb.float64[:, :, :],  # ub
+        nb.float64[:, :, :],  # w
+        nb.float64[:, :, :],  # c1
+        nb.float64[:, :, :],  # c2
+        nb.int32,  # iters
+        nb.types.NumPyRandomGeneratorType("NumPyRandomGeneratorType"),
+    ),
+    cache=True,
+    nogil=True,
+)
 def repair_out_of_bounds(
     x: Array3d,
     x_new: Array3d,
     v_new: Array3d,
     px: Array3d,
     sx: Array3d,
     v: Array3d,
```

### Comparing `vpso-1.0.2/src/vpso/termination.py` & `vpso-1.1.0/src/vpso/termination.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,28 @@
-import logging
-
+import numba as nb
 import numpy as np
 
-from vpso.jit import jit
 from vpso.typing import Array1d, Array1i, Array2i, Array3d
 
 
-@jit()
+@nb.njit(
+    nb.types.UniTuple(nb.float64[:], 2)(
+        nb.float64[:, :, :],  # sx
+        nb.float64[:],  # sf
+        nb.float64[:, :, :],  # sx_new
+        nb.float64[:],  # sf_new
+        nb.float64[:, :, :],  # lb
+        nb.float64[:, :, :],  # ub
+        nb.float64[:],  # xtol
+        nb.float64[:],  # ftol
+        nb.int32[:, :],  # current_patience_level
+    ),
+    cache=True,
+    nogil=True,
+)
 def update_patience(
     sx: Array3d,
     sf: Array1d,
     sx_new: Array3d,
     sf_new: Array1d,
     lb: Array3d,
     ub: Array3d,
@@ -41,57 +53,75 @@
         Upper bound of the search space. An array of shape `(N, 1, d)`.
     xtol : 1d array
         Tolerance for average changes in the objective minimizer before terminating the
         solver. An array of shape `(N,)`.
     ftol : 1d array
         Number of iterations to wait before terminating the solver if no improvement is
         witnessed. An array of shape `(N,)`.
-    current_patience_level : Array2i
+    current_patience_level : 2d array of ints
         Current patience level, i.e., for how many iterations the tolerances have been
         met. An array of shape `(N, 2)`, where the first column corresponds to the
         tolerance in `x`, and the second column in `f`. This array is modified in-place.
 
     Returns
     -------
     tuple of 1d arrays
-        Returns the current termination criteria for `x` and `f`, respectively.
+        Returns the current termination criteria for `x` and `f`, respectively, for each
+        vectorized problem.
     """
     # NOTE: current patience level is to be modified in-place
     # normalize sx and sx_new and compute normalized euclidean distance (could call
     # batch_cdist here, but it's only one vector per bathc, so this should be faster)
     domain = ub - lb
-    sx_norm = sx / domain
-    sx_new_norm = sx_new / domain
-    D = np.sqrt(np.square(sx_norm - sx_new_norm).sum(2))[:, 0]
+    D = np.sqrt(np.square((sx - sx_new) / domain).sum(2))[:, 0]
     current_patience_level[:, 0] = np.where(
         D <= xtol, current_patience_level[:, 0] + 1, 0
     )
 
     # compute tolerance for f
     F = np.maximum(0.0, sf - sf_new)
     current_patience_level[:, 1] = np.where(
         F <= ftol, current_patience_level[:, 1] + 1, 0
     )
     return D, F
 
 
+@nb.njit(
+    nb.types.Tuple((nb.bool_, nb.types.unicode_type, nb.float64, nb.float64))(
+        nb.float64[:, :, :],  # sx
+        nb.float64[:],  # sf
+        nb.float64[:, :, :],  # sx_new
+        nb.float64[:],  # sf_new
+        nb.float64[:, :, :],  # lb
+        nb.float64[:, :, :],  # ub
+        nb.float64[:],  # xtol
+        nb.float64[:],  # ftol
+        nb.int32[:],  # patience
+        nb.int32[:, :],  # current_patience_level
+    ),
+    cache=True,
+    nogil=True,
+)
 def termination(
     sx: Array3d,
     sf: Array1d,
     sx_new: Array3d,
     sf_new: Array1d,
     lb: Array3d,
     ub: Array3d,
     xtol: Array1d,
     ftol: Array1d,
     patience: Array1i,
     current_patience_level: Array2i,
-    logger: logging.Logger,
-) -> tuple[bool, str]:
-    """_summary_
+) -> tuple[bool, str, float, float]:
+    """Checks whether the solver should terminate, and the reason why. Updates the
+    patience level for each problem as a function of the previous and next best
+    particle. The level is increased if tolerances are met, and reset to zero if the new
+    best particle is better than the previous one by a margin larger than the
+    tolerances. `current_patience_level` is modified in-place.
 
     Parameters
     ----------
     sx : 3d array
         Social best, i.e., the best particle so far. An array of shape `(N, 1, d)`,
         where `N` is the number of vectorized problems to solve simultaneously, and `d`
         is the dimension of the search space.
@@ -107,38 +137,32 @@
         Upper bound of the search space. An array of shape `(N, 1, d)`.
     xtol : 1d array
         Tolerance for average changes in the objective minimizer before terminating the
         solver. An array of shape `(N,)`.
     ftol : 1d array
         Number of iterations to wait before terminating the solver if no improvement is
         witnessed. An array of shape `(N,)`.
-    patience : int or 1d array_like of ints, optional
+    patience : 1d array of ints, optional
         Number of iterations to wait before terminating the solver if no improvement is
         witnessed. An array of shape `(N,)`.
-    current_patience_level : Array2i
+    current_patience_level : 2d array of ints
         Current patience level, i.e., for how many iterations the tolerances have been
         met. An array of shape `(N, 2)`, where the first column corresponds to the
         tolerance in `x`, and the second column in `f`. This array is modified in-place.
 
     Returns
     -------
-    tuple of bool and str
+    tuple of bool, str, range_min, range_max
         Returns whether the solver should terminate, and the reason why. The reason can
         be either `xtol` or `ftol`, depending on which tolerance was met first.
+        Moreover, the min/max range for the tolerances that induced termination across
+        the vectorized problems is returned.
     """
     D, F = update_patience(
         sx, sf, sx_new, sf_new, lb, ub, xtol, ftol, current_patience_level
     )
-    if logger.level <= logging.DEBUG:
-        logger.debug(
-            "changes: x ∈ [%e, %e], f ∈ [%e, %e]",
-            D.min(),
-            D.max(),
-            F.min(),
-            F.max(),
-        )
-
+    # NOTE: can't f-string here because of numba, so we just return the ingredients
     if (current_patience_level[:, 0] >= patience).all():
-        return True, "xtol"
+        return True, "xtol", D.min(), D.max()
     if (current_patience_level[:, 1] >= patience).all():
-        return True, "ftol"
-    return False, ""
+        return True, "ftol", F.min(), F.max()
+    return False, "", np.nan, np.nan
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `vpso-1.0.2/src/vpso/vpso.py` & `vpso-1.1.0/src/vpso/vpso.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-import logging
 from typing import Callable, Optional, Union
 
 import numpy as np
 from numpy.typing import ArrayLike
 from scipy.stats.qmc import LatinHypercube
 
 from vpso.adaptation import adapt
 from vpso.ask_and_tell import advance_population, generate_offsprings, get_best
 from vpso.initialization import adjust_dimensions as adj_dim
 from vpso.initialization import initialize_particles
 from vpso.termination import termination
 from vpso.typing import Array1d, Array1i, Array2d, Array3d
 
-logger = logging.getLogger(__name__)
-
 
 def vpso(
     func: Callable[[Array3d], ArrayLike],
     lb: Array2d,
     ub: Array2d,
     #
     swarmsize: int = 25,
@@ -33,15 +30,14 @@
     #
     maxiter: int = 300,  # could be an array, but only the max would be then used
     ftol: Union[float, Array1d] = 1e-8,
     xtol: Union[float, Array1d] = 1e-8,
     patience: Union[int, Array1i] = 30,
     #
     seed: Optional[int] = None,
-    verbosity: int = logging.WARNING,
 ) -> tuple[Array2d, Array1d, str]:
     """Vectorized Particle Swarm Optimization (VPSO). This implementation of PSO is able
     to solve multiple optimization problems simultaneously in a vectorized fashion.
 
     Parameters
     ----------
     func : callable
@@ -95,49 +91,44 @@
         negative value to disable this check.
     patience : int or 1d array_like of ints, optional
         Number of iterations to wait before terminating the solver if no improvement is
         witnessed. Can also be an 1d array_like of shape `(N,)` to specify a different
         value for each of the `N` vectorized problems. By default, `1`.
     seed : int, optional
         Seed for the random number generator. By default, `None`.
-    verbosity : int, optional
-        Verbosity level of the solver. Levels higher than `INFO` log nothig. By default,
-        `logging.WARNING` is used.
 
     Returns
     -------
     tuple of (2d array, 1d array, str)
         Returns a tuple containing
          - the best minimizer of each problem
          - the best minimum of each problem
          - the termination reason as a string
     """
-    logger.setLevel(verbosity)
-
     # first, adjust some dimensions
     lb, ub, nvec, dim, max_velocity_rate, w, c1, c2, ftol, xtol, patience = adj_dim(
         lb, ub, max_velocity_rate, w, c1, c2, ftol, xtol, patience
     )
 
     # initialize particle positions and velocities
-    lhs_sampler = LatinHypercube(d=nvec * dim, seed=seed)
     np_random = np.random.Generator(np.random.PCG64(seed))
+    lhs_sampler = LatinHypercube(d=nvec * dim, seed=np_random)
     x, v, v_max = initialize_particles(
         nvec, swarmsize, dim, lb, ub, max_velocity_rate, lhs_sampler, np_random
     )
 
     # initialize particle's best pos/value and global best
     px = x  # particle's best position
     pf = np.reshape(func(x), (nvec, swarmsize))  # particle's best value
-    sx, sf = get_best(px, pf, nvec, logger, 0)  # social/global best position/value
+    sx, sf = get_best(px, pf, nvec)  # social/global best position/value
 
     # main optimization loop
     patience_level = np.zeros((nvec, 2), dtype=np.int32)  # 2 level for x and for f
     termination_reason = "maxiter"
-    for i in range(1, maxiter + 1):
+    for _ in range(maxiter):
         x, v = generate_offsprings(
             x,
             px,
             pf,
             sx,
             v,
             v_max,
@@ -151,44 +142,30 @@
             repair_iters,
             perturb_best,
             mutation_prob,
             np_random,
         )
         f = np.reshape(func(x), (nvec, swarmsize))  # evaluate particles (non-jittable)
         px, pf = advance_population(x, f, px, pf)
-        sx_new, sf_new = get_best(px, pf, nvec, logger, i)
+        sx_new, sf_new = get_best(px, pf, nvec)
 
         # DEBUG
         # px.flags.writeable = (
         #     pf.flags.writeable
         # ) = sx.flags.writeable = sf.flags.writeable = False
         # assert (sf_new <= sf).all()
 
         if adaptive:
-            w, c1, c2 = adapt(
-                px,
-                sx_new,
-                nvec,
-                swarmsize,
-                lb,
-                ub,
-                w,
-                c1,
-                c2,
-                np_random,
-                logger,
-            )
+            w, c1, c2 = adapt(px, sx_new, nvec, swarmsize, lb, ub, w, c1, c2, np_random)
 
         # check termination conditions
-        should_terminate, reason = termination(
-            sx, sf, sx_new, sf_new, lb, ub, xtol, ftol, patience, patience_level, logger
+        should_terminate, reason, range_min, range_max = termination(
+            sx, sf, sx_new, sf_new, lb, ub, xtol, ftol, patience, patience_level
         )
         if should_terminate:
-            termination_reason = reason
+            termination_reason = f"{reason} ∈ [{range_min:e}, {range_max:e}]"
             break
 
         # save new best
         sx = sx_new
         sf = sf_new
-
-    logger.info('termination due to "%s"', termination_reason)
     return sx[:, 0], sf, termination_reason
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `vpso-1.0.2/src/vpso.egg-info/PKG-INFO` & `vpso-1.1.0/src/vpso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vpso
-Version: 1.0.2
+Version: 1.1.0
 Summary: Vectorized Particle Swarm Optimization
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/vectorized-particle-swarm
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/vectorized-particle-swarm/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vpso-1.0.2/src/vpso.egg-info/SOURCES.txt` & `vpso-1.1.0/src/vpso.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 src/vpso/__init__.py
 src/vpso/adaptation.py
 src/vpso/ask_and_tell.py
 src/vpso/initialization.py
-src/vpso/jit.py
 src/vpso/math.py
 src/vpso/mutation.py
 src/vpso/reparation.py
 src/vpso/termination.py
 src/vpso/typing.py
 src/vpso/vpso.py
 src/vpso.egg-info/PKG-INFO
```

### Comparing `vpso-1.0.2/tests/test_adaptation.py` & `vpso-1.1.0/tests/test_adaptation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 import unittest
 
 import numpy as np
 from pymoo.problems.functional import FunctionalProblem
 from pymoo.util.misc import norm_eucl_dist
 
 from vpso.adaptation import adapt, adaptation_strategy
@@ -122,15 +121,14 @@
             swarmsize,
             lb[:, np.newaxis],
             ub[:, np.newaxis],
             w[:, np.newaxis, np.newaxis],
             c1[:, np.newaxis, np.newaxis],
             c2[:, np.newaxis, np.newaxis],
             np_random,
-            logging.getLogger(),
         )
         np.testing.assert_allclose(w_new_.squeeze(), w_new, err_msg="w")
         np.testing.assert_allclose(c1_new_.squeeze(), c1_new, err_msg="c1")
         np.testing.assert_allclose(c2_new_.squeeze(), c2_new, err_msg="c2")
 
 
 if __name__ == "__main__":
```

### Comparing `vpso-1.0.2/tests/test_initialization.py` & `vpso-1.1.0/tests/test_initialization.py`

 * *Files identical despite different names*

### Comparing `vpso-1.0.2/tests/test_math.py` & `vpso-1.1.0/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `vpso-1.0.2/tests/test_mutation.py` & `vpso-1.1.0/tests/test_mutation.py`

 * *Files identical despite different names*

### Comparing `vpso-1.0.2/tests/test_numerical.py` & `vpso-1.1.0/tests/test_numerical.py`

 * *Files identical despite different names*

### Comparing `vpso-1.0.2/tests/test_reparation.py` & `vpso-1.1.0/tests/test_reparation.py`

 * *Files identical despite different names*

