# Comparing `tmp/xenosite-fragment-0a5.tar.gz` & `tmp/xenosite-fragment-0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xenosite-fragment-0a5.tar", last modified: Wed Jun 14 16:07:03 2023, max compression
+gzip compressed data, was "xenosite-fragment-0a7.tar", last modified: Sat Jun 17 22:07:51 2023, max compression
```

## Comparing `xenosite-fragment-0a5.tar` & `xenosite-fragment-0a7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 swamidass   (501) staff       (20)        0 2023-06-14 16:07:03.392874 xenosite-fragment-0a5/
--rw-r--r--   0 swamidass   (501) staff       (20)     4396 2023-06-14 16:07:03.392266 xenosite-fragment-0a5/PKG-INFO
--rw-r--r--   0 swamidass   (501) staff       (20)     3735 2023-06-09 19:04:17.000000 xenosite-fragment-0a5/README.md
--rw-r--r--   0 swamidass   (501) staff       (20)       76 2022-11-29 00:33:42.000000 xenosite-fragment-0a5/pyproject.toml
--rw-r--r--   0 swamidass   (501) staff       (20)       38 2023-06-14 16:07:03.393129 xenosite-fragment-0a5/setup.cfg
--rw-r--r--   0 swamidass   (501) staff       (20)     1790 2023-06-09 18:47:43.000000 xenosite-fragment-0a5/setup.py
-drwxr-xr-x   0 swamidass   (501) staff       (20)        0 2023-06-14 16:07:03.380389 xenosite-fragment-0a5/test/
--rw-r--r--   0 swamidass   (501) staff       (20)     1460 2023-06-08 21:38:52.000000 xenosite-fragment-0a5/test/test_fragment.py
--rw-r--r--   0 swamidass   (501) staff       (20)      950 2023-05-28 17:37:00.000000 xenosite-fragment-0a5/test/test_morgan.py
--rw-r--r--   0 swamidass   (501) staff       (20)     7779 2023-05-25 21:09:30.000000 xenosite-fragment-0a5/test/test_netx.py
--rw-r--r--   0 swamidass   (501) staff       (20)     1197 2022-12-08 17:59:30.000000 xenosite-fragment-0a5/test/test_remap.py
--rw-r--r--   0 swamidass   (501) staff       (20)     1106 2023-06-14 15:20:24.000000 xenosite-fragment-0a5/test/test_tanimoto.py
-drwxr-xr-x   0 swamidass   (501) staff       (20)        0 2023-06-14 16:07:03.376796 xenosite-fragment-0a5/xenosite/
-drwxr-xr-x   0 swamidass   (501) staff       (20)        0 2023-06-14 16:07:03.393497 xenosite-fragment-0a5/xenosite/fragment/
--rw-r--r--   0 swamidass   (501) staff       (20)     3976 2023-06-14 15:09:35.000000 xenosite-fragment-0a5/xenosite/fragment/__init__.py
--rw-r--r--   0 swamidass   (501) staff       (20)     9026 2022-11-28 23:05:55.000000 xenosite-fragment-0a5/xenosite/fragment/__main__.py
--rw-r--r--   0 swamidass   (501) staff       (20)       59 2023-06-14 16:07:03.393642 xenosite-fragment-0a5/xenosite/fragment/_static_version.py
--rw-r--r--   0 swamidass   (501) staff       (20)     5773 2022-11-09 23:54:52.000000 xenosite-fragment-0a5/xenosite/fragment/_version.py
--rw-r--r--   0 swamidass   (501) staff       (20)    12807 2023-06-14 15:22:00.000000 xenosite-fragment-0a5/xenosite/fragment/chem.py
--rw-r--r--   0 swamidass   (501) staff       (20)     6224 2023-06-07 17:13:05.000000 xenosite-fragment-0a5/xenosite/fragment/feature.py
--rw-r--r--   0 swamidass   (501) staff       (20)     4848 2023-06-08 21:33:14.000000 xenosite-fragment-0a5/xenosite/fragment/graph.py
--rw-r--r--   0 swamidass   (501) staff       (20)     1236 2023-06-14 16:06:47.000000 xenosite-fragment-0a5/xenosite/fragment/keras_backend.py
--rw-r--r--   0 swamidass   (501) staff       (20)     3063 2023-06-03 20:49:36.000000 xenosite-fragment-0a5/xenosite/fragment/morgan.py
--rw-r--r--   0 swamidass   (501) staff       (20)       78 2023-05-25 21:12:23.000000 xenosite-fragment-0a5/xenosite/fragment/netx.py
--rw-r--r--   0 swamidass   (501) staff       (20)     3180 2022-12-08 17:59:30.000000 xenosite-fragment-0a5/xenosite/fragment/remap.py
--rw-r--r--   0 swamidass   (501) staff       (20)     5640 2023-06-07 18:01:31.000000 xenosite-fragment-0a5/xenosite/fragment/serialize.py
--rw-r--r--   0 swamidass   (501) staff       (20)     3650 2023-05-27 20:39:10.000000 xenosite-fragment-0a5/xenosite/fragment/stats.py
-drwxr-xr-x   0 swamidass   (501) staff       (20)        0 2023-06-14 16:07:03.391438 xenosite-fragment-0a5/xenosite_fragment.egg-info/
--rw-r--r--   0 swamidass   (501) staff       (20)     4396 2023-06-14 16:07:03.000000 xenosite-fragment-0a5/xenosite_fragment.egg-info/PKG-INFO
--rw-r--r--   0 swamidass   (501) staff       (20)      765 2023-06-14 16:07:03.000000 xenosite-fragment-0a5/xenosite_fragment.egg-info/SOURCES.txt
--rw-r--r--   0 swamidass   (501) staff       (20)        1 2023-06-14 16:07:03.000000 xenosite-fragment-0a5/xenosite_fragment.egg-info/dependency_links.txt
--rw-r--r--   0 swamidass   (501) staff       (20)      131 2023-06-14 16:07:03.000000 xenosite-fragment-0a5/xenosite_fragment.egg-info/entry_points.txt
--rw-r--r--   0 swamidass   (501) staff       (20)       45 2023-06-14 16:07:03.000000 xenosite-fragment-0a5/xenosite_fragment.egg-info/requires.txt
--rw-r--r--   0 swamidass   (501) staff       (20)       18 2023-06-14 16:07:03.000000 xenosite-fragment-0a5/xenosite_fragment.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 22:07:51.207681 xenosite-fragment-0a7/
+-rw-r--r--   0 root         (0) root         (0)     4451 2023-06-17 22:07:51.207681 xenosite-fragment-0a7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3735 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/README.md
+-rw-r--r--   0 root         (0) root         (0)       76 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-17 22:07:51.207681 xenosite-fragment-0a7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1808 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 22:07:51.207681 xenosite-fragment-0a7/test/
+-rw-r--r--   0 root         (0) root         (0)     2294 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/test/test_fragment.py
+-rw-r--r--   0 root         (0) root         (0)      950 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/test/test_morgan.py
+-rw-r--r--   0 root         (0) root         (0)     7779 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/test/test_netx.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/test/test_remap.py
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/test/test_tanimoto.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 22:07:51.207681 xenosite-fragment-0a7/xenosite/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 22:07:51.207681 xenosite-fragment-0a7/xenosite/fragment/
+-rw-r--r--   0 root         (0) root         (0)     3976 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/xenosite/fragment/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9026 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/xenosite/fragment/__main__.py
+-rw-r--r--   0 root         (0) root         (0)       59 2023-06-17 22:07:51.207681 xenosite-fragment-0a7/xenosite/fragment/_static_version.py
+-rw-r--r--   0 root         (0) root         (0)     5773 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/xenosite/fragment/_version.py
+-rw-r--r--   0 root         (0) root         (0)    12807 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/xenosite/fragment/chem.py
+-rw-r--r--   0 root         (0) root         (0)     6224 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/xenosite/fragment/feature.py
+-rw-r--r--   0 root         (0) root         (0)     5887 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/xenosite/fragment/graph.py
+-rw-r--r--   0 root         (0) root         (0)     1236 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/xenosite/fragment/keras_backend.py
+-rw-r--r--   0 root         (0) root         (0)     3063 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/xenosite/fragment/morgan.py
+-rw-r--r--   0 root         (0) root         (0)       78 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/xenosite/fragment/netx.py
+-rw-r--r--   0 root         (0) root         (0)     3180 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/xenosite/fragment/remap.py
+-rw-r--r--   0 root         (0) root         (0)     5640 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/xenosite/fragment/serialize.py
+-rw-r--r--   0 root         (0) root         (0)     3650 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/xenosite/fragment/stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 22:07:51.207681 xenosite-fragment-0a7/xenosite_fragment.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4451 2023-06-17 22:07:51.000000 xenosite-fragment-0a7/xenosite_fragment.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      765 2023-06-17 22:07:51.000000 xenosite-fragment-0a7/xenosite_fragment.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 22:07:51.000000 xenosite-fragment-0a7/xenosite_fragment.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      132 2023-06-17 22:07:51.000000 xenosite-fragment-0a7/xenosite_fragment.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-17 22:07:51.000000 xenosite-fragment-0a7/xenosite_fragment.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-17 22:07:51.000000 xenosite-fragment-0a7/xenosite_fragment.egg-info/top_level.txt
```

### Comparing `xenosite-fragment-0a5/PKG-INFO` & `xenosite-fragment-0a7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: xenosite-fragment
-Version: 0a5
+Version: 0a7
 Summary: Library for molecule fragment operations.
+Home-page: UNKNOWN
 Author: S. Joshua Swamidass
 Author-email: swamidass@wustl.edu
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
@@ -152,24 +155,25 @@
 Enumerate and compute statistics on all the subgraphs in a molecule:
 
 ```
 >>> from xenosite.fragment.net import SubGraphFragmentNetwork
 >>> N = SubGraphFragmentNetwork("CC1COC1")
 >>> fragments = N.to_pandas()
 >>> list(fragments.index)
-['C-C', 'C', 'C-O-C', 'C-O', 'O', 'C-C1-C-O-C-1', 'C1-C-O-C-1', 'C-C-C-O', 'C-C(-C)-C', 'C-C-O', 'C-C-C']
+['C-C', 'C', 'C-O-C', 'C-O', 'O', 'C-C1-C-O-C-1', 'C1-C-C-O-1', 'C-C-C-O', 'C-C(-C)-C', 'C-C-O', 'C-C-C']
 >>> fragments["size"].to_numpy()
 array([2, 1, 3, 2, 1, 5, 4, 4, 4, 3, 3])
 ```
 
 Better fragments can be enumerated by collapsing all atoms in a ring into a single node
 during subgraph enumeration. 
 
 ```
 >>> from xenosite.fragment.net import RingFragmentNetwork
 >>> N = RingFragmentNetwork("CC1COC1")
 >>> fragments = N.to_pandas()
 >>> list(fragments.index)
-['C-C1-C-O-C-1', 'C', 'C1-C-O-C-1']
+['C-C1-C-O-C-1', 'C', 'C1-C-C-O-1']
 >>> fragments["size"].to_numpy()
 array([5, 1, 4])
 ```
+
```

### Comparing `xenosite-fragment-0a5/README.md` & `xenosite-fragment-0a7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -134,24 +134,24 @@
 Enumerate and compute statistics on all the subgraphs in a molecule:
 
 ```
 >>> from xenosite.fragment.net import SubGraphFragmentNetwork
 >>> N = SubGraphFragmentNetwork("CC1COC1")
 >>> fragments = N.to_pandas()
 >>> list(fragments.index)
-['C-C', 'C', 'C-O-C', 'C-O', 'O', 'C-C1-C-O-C-1', 'C1-C-O-C-1', 'C-C-C-O', 'C-C(-C)-C', 'C-C-O', 'C-C-C']
+['C-C', 'C', 'C-O-C', 'C-O', 'O', 'C-C1-C-O-C-1', 'C1-C-C-O-1', 'C-C-C-O', 'C-C(-C)-C', 'C-C-O', 'C-C-C']
 >>> fragments["size"].to_numpy()
 array([2, 1, 3, 2, 1, 5, 4, 4, 4, 3, 3])
 ```
 
 Better fragments can be enumerated by collapsing all atoms in a ring into a single node
 during subgraph enumeration. 
 
 ```
 >>> from xenosite.fragment.net import RingFragmentNetwork
 >>> N = RingFragmentNetwork("CC1COC1")
 >>> fragments = N.to_pandas()
 >>> list(fragments.index)
-['C-C1-C-O-C-1', 'C', 'C1-C-O-C-1']
+['C-C1-C-O-C-1', 'C', 'C1-C-C-O-1']
 >>> fragments["size"].to_numpy()
 array([5, 1, 4])
 ```
```

### Comparing `xenosite-fragment-0a5/setup.py` & `xenosite-fragment-0a7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     packages=["xenosite/fragment"],
     entry_points={
         "console_scripts": [
             "xenosite-fragment=xenosite.fragment.__main__:app",
         ],
         "xenosite_command": ["fragment=xenosite.fragment.__main__:app"],
     },
-    install_requires=["rdkit", "numpy", "numba", "rich", "typer", "networkx", "pandas"],
+    install_requires=["rdkit", "numpy", "numba", "rich", "typer", "networkx", "pandas", "pynauty==2.8.6"],
     classifiers=[
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "Operating System :: MacOS",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python",
```

### Comparing `xenosite-fragment-0a5/test/test_morgan.py` & `xenosite-fragment-0a7/test/test_morgan.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a5/test/test_netx.py` & `xenosite-fragment-0a7/test/test_netx.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a5/test/test_remap.py` & `xenosite-fragment-0a7/test/test_remap.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a5/test/test_tanimoto.py` & `xenosite-fragment-0a7/test/test_tanimoto.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a5/xenosite/fragment/__init__.py` & `xenosite-fragment-0a7/xenosite/fragment/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,26 +104,26 @@
 
 Enumerate and compute statistics on all the subgraphs in a molecule:
 
 >>> from xenosite.fragment.net import SubGraphFragmentNetwork
 >>> N = SubGraphFragmentNetwork("CC1COC1")
 >>> fragments = N.to_pandas()
 >>> list(fragments.index)
-['C-C', 'C', 'C-O-C', 'C-O', 'O', 'C-C1-C-O-C-1', 'C1-C-O-C-1', 'C-C-C-O', 'C-C(-C)-C', 'C-C-O', 'C-C-C']
+['C-C', 'C', 'C-O-C', 'C-O', 'O', 'C-C1-C-O-C-1', 'C1-C-C-O-1', 'C-C-C-O', 'C-C(-C)-C', 'C-C-O', 'C-C-C']
 >>> fragments["size"].to_numpy()
 array([2, 1, 3, 2, 1, 5, 4, 4, 4, 3, 3])
 
 Better fragments can be enumerated by collapsing all atoms in a ring into a single node
 during subgraph enumeration. 
 
 >>> from xenosite.fragment.net import RingFragmentNetwork
 >>> N = RingFragmentNetwork("CC1COC1")
 >>> fragments = N.to_pandas()
 >>> list(fragments.index)
-['C-C1-C-O-C-1', 'C', 'C1-C-O-C-1']
+['C-C1-C-O-C-1', 'C', 'C1-C-C-O-1']
 >>> fragments["size"].to_numpy()
 array([5, 1, 4])
 
 """
 
 
 from .graph import Graph
```

### Comparing `xenosite-fragment-0a5/xenosite/fragment/__main__.py` & `xenosite-fragment-0a7/xenosite/fragment/__main__.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a5/xenosite/fragment/_version.py` & `xenosite-fragment-0a7/xenosite/fragment/_version.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a5/xenosite/fragment/chem.py` & `xenosite-fragment-0a7/xenosite/fragment/chem.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a5/xenosite/fragment/feature.py` & `xenosite-fragment-0a7/xenosite/fragment/feature.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a5/xenosite/fragment/graph.py` & `xenosite-fragment-0a7/xenosite/fragment/graph.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from enum import Enum
 from typing import NamedTuple, Optional, Sequence, Union, Any
-
+from numba import jit, njit
 import numpy as np
 
 from . import serialize
 from .morgan import morgan
 
 
 class BaseGraph:
@@ -98,26 +98,67 @@
               e1 = self.edge[0]
               e2 = self.edge[1]
 
               self._morgan = morgan(self.nlabel, e1, e2)  # type: ignore
     
         return self._morgan
 
+    def _to_nauty(self, colors=True):
+        import pynauty
+        g = pynauty.Graph(self.n)
+        for i,j in zip(*self.edge): g.connect_vertex(i,j)
+
+        if colors and self.nlabel:
+            c = self.nlabel
+            c = _to_nauty_colors(c)
+            g.set_vertex_coloring(c)         
+        return g
+    
+    def _nauty_order(self):
+        import pynauty
+        if self.elabel:
+            return self.edge_to_node()._nauty_order()[:self.n]
+        
+        g = self._to_nauty()
+
+        c = pynauty.canon_label(g)
+        c = np.asarray(c) #type:  ignore
+        c = _invert_mapping(c)
+        return c
+
     def serialize(self, canonize=True) -> serialize.Serialized:
         return serialize.serialize(self, canonize)
 
     @classmethod
     def from_molecule(cls, molecule, smiles=False) -> "Graph":
         from . import chem  # lazy import to prevent load of rdkit unless needed
 
         if smiles:
             return chem.MolToSmilesGraph(molecule)
         return chem.MolToSmartsGraph(molecule)
 
 
+def _to_nauty_colors(x):
+  unq = sorted(np.unique(x))
+  unq_lookup = {u: n for n,u in enumerate(unq)}
+
+  colors = [set() for _ in range(len(unq))]
+  for n, l in enumerate(x):
+    colors[unq_lookup[l]].add(n)
+
+  return colors
+
+
+@njit
+def _invert_mapping(x):
+    y = np.zeros_like(x)
+    for i in range(len(x)): y[x[i]] = i
+    return y
+
+
 class DFS_TYPE(int, Enum):
     TREE = 0
     RING = 1
 
 
 class DFS_EDGE(NamedTuple):
     i: int
@@ -128,16 +169,16 @@
 def _dfs(
     start: int,
     neighbors: dict[int, list[int]],
     visited: Optional[set[Union[int, tuple[int, int]]]] = None,
     out: Optional[list[DFS_EDGE]] = None,
 ) -> list[DFS_EDGE]:
 
-    visited = visited or set()
-    out = out or []
+    visited = visited if visited is not None else set()
+    out = out if out is not None else []
     visited.add(start)
 
     for n in neighbors[start]:
         e = tuple((n, start) if n < start else (start, n))
         if e in visited:
             continue
 
@@ -156,15 +197,15 @@
     N = neighbors(G)
     start = 0
 
     if G.n <= 1:
         return []
 
     if canonize:
-        M = G.morgan()
+        M = G._nauty_order()
         start = int(np.argmin(M))
         for n in N:
             N[n] = sorted(N[n], key=lambda x: M[x])
     else:
         for n in N:
             N[n] = sorted(N[n])
```

### Comparing `xenosite-fragment-0a5/xenosite/fragment/keras_backend.py` & `xenosite-fragment-0a7/xenosite/fragment/keras_backend.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a5/xenosite/fragment/morgan.py` & `xenosite-fragment-0a7/xenosite/fragment/morgan.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a5/xenosite/fragment/remap.py` & `xenosite-fragment-0a7/xenosite/fragment/remap.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a5/xenosite/fragment/serialize.py` & `xenosite-fragment-0a7/xenosite/fragment/serialize.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a5/xenosite/fragment/stats.py` & `xenosite-fragment-0a7/xenosite/fragment/stats.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a5/xenosite_fragment.egg-info/PKG-INFO` & `xenosite-fragment-0a7/xenosite_fragment.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: xenosite-fragment
-Version: 0a5
+Version: 0a7
 Summary: Library for molecule fragment operations.
+Home-page: UNKNOWN
 Author: S. Joshua Swamidass
 Author-email: swamidass@wustl.edu
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
@@ -152,24 +155,25 @@
 Enumerate and compute statistics on all the subgraphs in a molecule:
 
 ```
 >>> from xenosite.fragment.net import SubGraphFragmentNetwork
 >>> N = SubGraphFragmentNetwork("CC1COC1")
 >>> fragments = N.to_pandas()
 >>> list(fragments.index)
-['C-C', 'C', 'C-O-C', 'C-O', 'O', 'C-C1-C-O-C-1', 'C1-C-O-C-1', 'C-C-C-O', 'C-C(-C)-C', 'C-C-O', 'C-C-C']
+['C-C', 'C', 'C-O-C', 'C-O', 'O', 'C-C1-C-O-C-1', 'C1-C-C-O-1', 'C-C-C-O', 'C-C(-C)-C', 'C-C-O', 'C-C-C']
 >>> fragments["size"].to_numpy()
 array([2, 1, 3, 2, 1, 5, 4, 4, 4, 3, 3])
 ```
 
 Better fragments can be enumerated by collapsing all atoms in a ring into a single node
 during subgraph enumeration. 
 
 ```
 >>> from xenosite.fragment.net import RingFragmentNetwork
 >>> N = RingFragmentNetwork("CC1COC1")
 >>> fragments = N.to_pandas()
 >>> list(fragments.index)
-['C-C1-C-O-C-1', 'C', 'C1-C-O-C-1']
+['C-C1-C-O-C-1', 'C', 'C1-C-C-O-1']
 >>> fragments["size"].to_numpy()
 array([5, 1, 4])
 ```
+
```

### Comparing `xenosite-fragment-0a5/xenosite_fragment.egg-info/SOURCES.txt` & `xenosite-fragment-0a7/xenosite_fragment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

