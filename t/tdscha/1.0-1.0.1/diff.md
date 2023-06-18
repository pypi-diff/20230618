# Comparing `tmp/tdscha-1.0.tar.gz` & `tmp/tdscha-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdscha-1.0.tar", last modified: Tue Jun  6 10:50:26 2023, max compression
+gzip compressed data, was "tdscha-1.0.1.tar", last modified: Sun Jun 18 18:16:45 2023, max compression
```

## Comparing `tdscha-1.0.tar` & `tdscha-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 10:50:26.703264 tdscha-1.0/
-drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 10:50:26.703264 tdscha-1.0/CModules/
--rw-rw-r--   0 monacell  (1001) monacell  (1001)   101220 2023-05-22 15:37:19.000000 tdscha-1.0/CModules/LanczosFunctions.c
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    13176 2023-05-22 15:37:19.000000 tdscha-1.0/CModules/LanczosFunctions.h
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    46966 2023-05-22 15:37:19.000000 tdscha-1.0/CModules/odd_corr_module.c
-drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 10:50:26.703264 tdscha-1.0/Modules/
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    10306 2023-05-22 15:37:19.000000 tdscha-1.0/Modules/Dynamical.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)   192063 2023-05-23 10:18:45.000000 tdscha-1.0/Modules/DynamicalLanczos.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1264 2023-05-22 15:37:19.000000 tdscha-1.0/Modules/Parallel.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     3485 2023-05-22 15:37:19.000000 tdscha-1.0/Modules/Perturbations.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    27095 2023-05-22 15:37:19.000000 tdscha-1.0/Modules/StaticHessian.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    31830 2023-05-22 15:37:19.000000 tdscha-1.0/Modules/Tools.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)       80 2023-05-22 15:37:19.000000 tdscha-1.0/Modules/__init__.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     9935 2023-05-26 14:55:58.000000 tdscha-1.0/Modules/tdscha_core.jl
--rw-rw-r--   0 monacell  (1001) monacell  (1001)      199 2023-06-06 10:50:26.703264 tdscha-1.0/PKG-INFO
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     7401 2023-05-22 15:37:19.000000 tdscha-1.0/README.md
-drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 10:50:26.703264 tdscha-1.0/scripts/
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     3525 2023-05-22 15:37:19.000000 tdscha-1.0/scripts/plot_hessian_convergence.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     3943 2023-05-22 15:37:19.000000 tdscha-1.0/scripts/plot_lanczos_convergence.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1549 2023-05-22 15:37:19.000000 tdscha-1.0/scripts/tdscha-output2abc.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1554 2023-05-22 15:37:19.000000 tdscha-1.0/scripts/tdscha-plot.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)       38 2023-06-06 10:50:26.703264 tdscha-1.0/setup.cfg
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     6794 2023-06-06 10:50:12.000000 tdscha-1.0/setup.py
-drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 10:50:26.703264 tdscha-1.0/tdscha.egg-info/
--rw-rw-r--   0 monacell  (1001) monacell  (1001)      199 2023-06-06 10:50:26.000000 tdscha-1.0/tdscha.egg-info/PKG-INFO
--rw-rw-r--   0 monacell  (1001) monacell  (1001)      553 2023-06-06 10:50:26.000000 tdscha-1.0/tdscha.egg-info/SOURCES.txt
--rw-rw-r--   0 monacell  (1001) monacell  (1001)        1 2023-06-06 10:50:26.000000 tdscha-1.0/tdscha.egg-info/dependency_links.txt
--rw-rw-r--   0 monacell  (1001) monacell  (1001)       45 2023-06-06 10:50:26.000000 tdscha-1.0/tdscha.egg-info/requires.txt
--rw-rw-r--   0 monacell  (1001) monacell  (1001)       20 2023-06-06 10:50:26.000000 tdscha-1.0/tdscha.egg-info/top_level.txt
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-18 18:16:45.471073 tdscha-1.0.1/
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-18 18:16:45.467073 tdscha-1.0.1/CModules/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)   101262 2023-06-18 18:14:47.000000 tdscha-1.0.1/CModules/LanczosFunctions.c
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    13176 2023-05-22 15:37:19.000000 tdscha-1.0.1/CModules/LanczosFunctions.h
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    46966 2023-05-22 15:37:19.000000 tdscha-1.0.1/CModules/odd_corr_module.c
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-18 18:16:45.471073 tdscha-1.0.1/Modules/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    10306 2023-05-22 15:37:19.000000 tdscha-1.0.1/Modules/Dynamical.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)   192371 2023-06-18 18:14:47.000000 tdscha-1.0.1/Modules/DynamicalLanczos.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1264 2023-05-22 15:37:19.000000 tdscha-1.0.1/Modules/Parallel.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     3485 2023-05-22 15:37:19.000000 tdscha-1.0.1/Modules/Perturbations.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    27095 2023-05-22 15:37:19.000000 tdscha-1.0.1/Modules/StaticHessian.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    31830 2023-05-22 15:37:19.000000 tdscha-1.0.1/Modules/Tools.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)       80 2023-05-22 15:37:19.000000 tdscha-1.0.1/Modules/__init__.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     9935 2023-05-26 14:55:58.000000 tdscha-1.0.1/Modules/tdscha_core.jl
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      201 2023-06-18 18:16:45.471073 tdscha-1.0.1/PKG-INFO
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     7401 2023-05-22 15:37:19.000000 tdscha-1.0.1/README.md
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-18 18:16:45.471073 tdscha-1.0.1/scripts/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     3525 2023-05-22 15:37:19.000000 tdscha-1.0.1/scripts/plot_hessian_convergence.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4796 2023-06-18 18:14:47.000000 tdscha-1.0.1/scripts/tdscha-convergence-analysis.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1549 2023-05-22 15:37:19.000000 tdscha-1.0.1/scripts/tdscha-output2abc.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1554 2023-05-22 15:37:19.000000 tdscha-1.0.1/scripts/tdscha-plot.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)       38 2023-06-18 18:16:45.471073 tdscha-1.0.1/setup.cfg
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     6796 2023-06-18 18:15:11.000000 tdscha-1.0.1/setup.py
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-18 18:16:45.471073 tdscha-1.0.1/tdscha.egg-info/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      201 2023-06-18 18:16:45.000000 tdscha-1.0.1/tdscha.egg-info/PKG-INFO
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      556 2023-06-18 18:16:45.000000 tdscha-1.0.1/tdscha.egg-info/SOURCES.txt
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)        1 2023-06-18 18:16:45.000000 tdscha-1.0.1/tdscha.egg-info/dependency_links.txt
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)       45 2023-06-18 18:16:45.000000 tdscha-1.0.1/tdscha.egg-info/requires.txt
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)       20 2023-06-18 18:16:45.000000 tdscha-1.0.1/tdscha.egg-info/top_level.txt
```

### Comparing `tdscha-1.0/CModules/LanczosFunctions.c` & `tdscha-1.0.1/CModules/LanczosFunctions.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #include "LanczosFunctions.h"
 
 
 #define DEB 0
 #define DEB_L 0
+#define USEBLAS 
+
 
 // These are used for debugging
 #define X_VAL 1534
 #define Y_VAL 36
 
 // The eigenvalues of the inverse Covariance matrix
 double f_ups(double w, double T) {
@@ -2187,14 +2189,15 @@
 				printf("\n");
 				//fflush(stdout);
 			}
 			
 
 			// Compute the standard weight Y1
 			weight = 0;
+			// TODO, explot BLAS
 			for (mu = 0; mu < n_modes; ++mu) {
 				for (nu = 0; nu < n_modes; ++nu) {
 					weight -= displacement[mu] * displacement[nu] * Y1[mu * n_modes +  nu] / 2;
 				}
 			}
```

### Comparing `tdscha-1.0/CModules/LanczosFunctions.h` & `tdscha-1.0.1/CModules/LanczosFunctions.h`

 * *Files identical despite different names*

### Comparing `tdscha-1.0/CModules/odd_corr_module.c` & `tdscha-1.0.1/CModules/odd_corr_module.c`

 * *Files identical despite different names*

### Comparing `tdscha-1.0/Modules/Dynamical.py` & `tdscha-1.0.1/Modules/Dynamical.py`

 * *Files identical despite different names*

### Comparing `tdscha-1.0/Modules/DynamicalLanczos.py` & `tdscha-1.0.1/Modules/DynamicalLanczos.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
 
 def is_julia_enabled():
     return __JULIA_EXT__
 
 
 class Lanczos(object):
-    def __init__(self, ensemble = None, mode = 1, unwrap_symmetries = False, select_modes = None):
+    def __init__(self, ensemble = None, mode = 1, unwrap_symmetries = False, select_modes = None, lo_to_split = "random"):
         """
         INITIALIZE THE LANCZOS
         ======================
 
         This function extracts the weights, the X and Y arrays for the d3 and d4
         computation as well as the polarization vectors and frequencies.
 
@@ -117,14 +117,17 @@
                    3) Fast Julia multithreading (only if julia is available)
             unwrap_symmetries : bool
                 If true (default), the ensemble is unwrapped to respect the symmetries.
                 This requires SPGLIB installed.
             select_modes : ndarray(size = n_modes, dtype = bool)
                 A mask for each mode, if False, the mode is neglected. Use this to exclude some modes that you know are not
                 involved in the calculation. If not specified, all modes are considered by default.
+            lo_to_split : string or ndarray
+                Mode of lo_to_splitting. If empty or none, it is LO-TO splitting correction is neglected.
+                If a ndarray is provided, it is the direction of q on which the LO-TO splitting is computed.
 
         """
 
         self.mode = mode
 
         # Define the order
         order = "C"
@@ -199,15 +202,15 @@
         self.dyn = ensemble.current_dyn.Copy() 
         #superdyn = self.dyn.GenerateSupercellDyn(ensemble.supercell)
         self.uci_structure = ensemble.current_dyn.structure.copy()
         self.super_structure = self.dyn.structure.generate_supercell(self.dyn.GetSupercell())#superdyn.structure
 
         self.T = ensemble.current_T
 
-        ws, pols = self.dyn.DiagonalizeSupercell()
+        ws, pols = self.dyn.DiagonalizeSupercell(lo_to_split = lo_to_split)
 
 
         self.nat = self.super_structure.N_atoms
         n_cell = np.prod(self.dyn.GetSupercell())
 
         self.qe_sym = CC.symmetries.QE_Symmetry(self.dyn.structure)
         self.qe_sym.SetupQPoint()
```

### Comparing `tdscha-1.0/Modules/Parallel.py` & `tdscha-1.0.1/Modules/Parallel.py`

 * *Files identical despite different names*

### Comparing `tdscha-1.0/Modules/Perturbations.py` & `tdscha-1.0.1/Modules/Perturbations.py`

 * *Files identical despite different names*

### Comparing `tdscha-1.0/Modules/StaticHessian.py` & `tdscha-1.0.1/Modules/StaticHessian.py`

 * *Files identical despite different names*

### Comparing `tdscha-1.0/Modules/Tools.py` & `tdscha-1.0.1/Modules/Tools.py`

 * *Files identical despite different names*

### Comparing `tdscha-1.0/Modules/tdscha_core.jl` & `tdscha-1.0.1/Modules/tdscha_core.jl`

 * *Files identical despite different names*

### Comparing `tdscha-1.0/README.md` & `tdscha-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tdscha-1.0/scripts/plot_hessian_convergence.py` & `tdscha-1.0.1/scripts/plot_hessian_convergence.py`

 * *Files identical despite different names*

### Comparing `tdscha-1.0/scripts/plot_lanczos_convergence.py` & `tdscha-1.0.1/scripts/tdscha-convergence-analysis.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,132 +10,156 @@
 
 import cellconstructor as CC
 import cellconstructor.Phonons
 
 import sscha
 import tdscha, tdscha.DynamicalLanczos as DL
 import sscha.Ensemble
-
-# Get from command line the last lanczos step
-if not len(sys.argv) in [2, 3]:
-    print("Error, I require the Lanczos .npz file to be analyzed (the last), and (optionally) the smearing [cm-1]")
-    raise ValueError("Error, I require the Lanczos .npz file to be analyzed (the last)")
-
-fname = sys.argv[1]
-
-smearing = 1
-if len(sys.argv) == 3:
-    smearing = float(sys.argv[2])
-
-# Check if the file exists
-if not os.path.exists(fname):
-    raise IOError("Error, the specified file '{}' does not exist.".format(fname))
-
-# Check how many files are here
-#files = [x for x in  os.listdir(".") if "LANCZOS_STEP" in x and ".npz" in x]
-
-
-data = []
-nat = 0
-print ("Reading the lanczos file...")
-data = DL.Lanczos()
-
-if fname.endswith('.abc'):
-    data.load_abc(fname)
-else:
-    data.load_status(fname)
-nat = data.nat
-N_iters = len(data.a_coeffs) - 1
-
-# Now get the static converge
-W_START = 0
-W_END = 10000 / CC.Units.RY_TO_CM
-NW = 10000
-SMEARING = smearing / CC.Units.RY_TO_CM
-
-print ("Computing the static responce...")
-freqs = np.zeros((N_iters, 3*nat))
-dynamical = np.zeros((N_iters, NW))
-dynamical_noterm = np.zeros((N_iters, NW))
-w_array = np.linspace(W_START, W_END, NW)
-w_static = np.zeros((N_iters), dtype = np.double)
-
-a_coeffs = np.copy(data.a_coeffs)
-b_coeffs = np.copy(data.b_coeffs)
-c_coeffs = np.copy(data.c_coeffs)
-
-for i in range(N_iters):
-    data.a_coeffs = a_coeffs[:i+1]
-    data.b_coeffs = b_coeffs[:i]
-    data.c_coeffs = c_coeffs[:i]
-    
-    #fc_odd = data.get_static_odd_fc(False)
-    #fc_odd /= np.sqrt(np.outer(data.m, data.m))
-    #w, p = np.linalg.eigh(fc_odd)
-    #sign_mask = np.sign(w)
-    #w = sign_mask * np.sqrt(np.abs(w))
-    #w *= CC.Phonons.RY_TO_CM
-    #freqs[i, :] = w 
-
-    gf = data.get_green_function_continued_fraction(w_array, use_terminator = False, smearing = SMEARING)
-
-    dynamical_noterm[i, :] = -np.imag( gf)
-    w2 = 1 / np.real(gf[0])
-    w_static[i] = np.sign(w2) * np.sqrt(np.abs(w2)) * CC.Units.RY_TO_CM
-    dynamical[i, :] = -np.imag( data.get_green_function_continued_fraction(w_array, use_terminator = True, smearing = SMEARING))
-    
-
-
-
-    if i % 10 == 0:
-        sys.stderr.write("\rProgress %% %d" % (i * 100 / N_iters))
-        sys.stderr.flush()
-sys.stderr.write("\n")
-
-print ("Plotting the results...")
-
-plt.figure(dpi = 160)
-plt.title("Static Frequency")
-plt.plot(np.arange(N_iters), w_static, marker = "o")
-plt.xlabel("Lanczos step")
-plt.ylabel("Static frequency [cm-1]")
-plt.tight_layout()
-
-
-plt.figure(dpi = 160)
-plt.title("Green function without terminator")
-plt.imshow(dynamical_noterm, aspect = "auto", origin = "lower", extent = [W_START*CC.Phonons.RY_TO_CM, W_END*CC.Phonons.RY_TO_CM, 1, N_iters])
-plt.xlabel("Frequency [cm-1]")
-plt.ylabel("Steps")
-plt.colorbar()
-plt.tight_layout()
-
-
-plt.figure(dpi = 160)
-plt.title("Green function with terminator")
-plt.imshow(dynamical, aspect = "auto", origin = "lower", extent = [W_START*CC.Phonons.RY_TO_CM, W_END*CC.Phonons.RY_TO_CM, 1, N_iters])
-plt.xlabel("Frequency [cm-1]")
-plt.ylabel("Steps")
-plt.colorbar()
-plt.tight_layout()
-
-
-
-# get colormap
-cmap=plt.cm.viridis
-# build cycler with 5 equally spaced colors from that colormap
-c = cycler('color', cmap(np.linspace(0,1,N_iters)) )
-# supply cycler to the rcParam
-plt.rcParams["axes.prop_cycle"] = c
-
-plt.figure(dpi = 160)
-plt.title("Green function with terminator")
-for i in range(N_iters):
-    plt.plot(w_array * CC.Phonons.RY_TO_CM, dynamical[i, :])
-
-# The last one is plotted in red underlined
-plt.plot(w_array * CC.Phonons.RY_TO_CM, dynamical[-1, :], color = "r", linewidth = 3.5)
-plt.xlabel("Frequency [cm-1]")
-plt.ylabel("Steps")
-plt.tight_layout()
-
-plt.show()
+MSG = """
+TDSCHA  
+======
+
+Analyze the convergence with the number of steps of a Lanczos
+calculation
+Usage:
+
+tdscha-convergence-analysis.py  lanczos_status_file [smearing]
+
+lanczos_status_file is either a npz or a abc file generated by the script.
+text output file can be converted into the abc file with the tdscha-output2abc.py utility.
+
+The smearing is in cm-1
+"""
+
+def print_usage():
+    print(MSG)
+
+def main():
+    # Get from command line the last lanczos step
+    if not len(sys.argv) in [2, 3]:
+        print("Error, require the Lanczos .npz (or .abc) file to be analyzed, and (optionally) the smearing [cm-1]")
+        raise ValueError("Error, I require the Lanczos .npz (or .abc) file to be analyzed)")
+
+    fname = sys.argv[1]
+
+    smearing = 1
+    if len(sys.argv) == 3:
+        smearing = float(sys.argv[2])
+
+    # Check if the file exists
+    if not os.path.exists(fname):
+        raise IOError("Error, the specified file '{}' does not exist.".format(fname))
+
+    # Check how many files are here
+    #files = [x for x in  os.listdir(".") if "LANCZOS_STEP" in x and ".npz" in x]
+
+
+    data = []
+    nat = 0
+    print ("Reading the lanczos file...")
+    data = DL.Lanczos()
+
+    if fname.endswith('.abc'):
+        data.load_abc(fname)
+    else:
+        data.load_status(fname)
+    nat = data.nat
+    N_iters = len(data.a_coeffs) - 1
+
+    # Now get the static converge
+    W_START = 0
+    W_END = 10000 / CC.Units.RY_TO_CM
+    NW = 10000
+    SMEARING = smearing / CC.Units.RY_TO_CM
+
+    print ("Computing the static responce...")
+    freqs = np.zeros((N_iters, 3*nat))
+    dynamical = np.zeros((N_iters, NW))
+    dynamical_noterm = np.zeros((N_iters, NW))
+    w_array = np.linspace(W_START, W_END, NW)
+    w_static = np.zeros((N_iters), dtype = np.double)
+
+    a_coeffs = np.copy(data.a_coeffs)
+    b_coeffs = np.copy(data.b_coeffs)
+    c_coeffs = np.copy(data.c_coeffs)
+
+    for i in range(N_iters):
+        data.a_coeffs = a_coeffs[:i+1]
+        data.b_coeffs = b_coeffs[:i]
+        data.c_coeffs = c_coeffs[:i]
+        
+        #fc_odd = data.get_static_odd_fc(False)
+        #fc_odd /= np.sqrt(np.outer(data.m, data.m))
+        #w, p = np.linalg.eigh(fc_odd)
+        #sign_mask = np.sign(w)
+        #w = sign_mask * np.sqrt(np.abs(w))
+        #w *= CC.Phonons.RY_TO_CM
+        #freqs[i, :] = w 
+
+        gf = data.get_green_function_continued_fraction(w_array, use_terminator = False, smearing = SMEARING)
+
+        dynamical_noterm[i, :] = -np.imag( gf)
+        w2 = 1 / np.real(gf[0])
+        w_static[i] = np.sign(w2) * np.sqrt(np.abs(w2)) * CC.Units.RY_TO_CM
+        dynamical[i, :] = -np.imag( data.get_green_function_continued_fraction(w_array, use_terminator = True, smearing = SMEARING))
+        
+
+
+
+        if i % 10 == 0:
+            sys.stderr.write("\rProgress %% %d" % (i * 100 / N_iters))
+            sys.stderr.flush()
+    sys.stderr.write("\n")
+
+    print ("Plotting the results...")
+
+    plt.figure(dpi = 160)
+    plt.title("Static Frequency")
+    plt.plot(np.arange(N_iters), w_static, marker = "o")
+    plt.xlabel("Lanczos step")
+    plt.ylabel("Static frequency [cm-1]")
+    plt.tight_layout()
+
+
+    plt.figure(dpi = 160)
+    plt.title("Green function without terminator")
+    plt.imshow(dynamical_noterm, aspect = "auto", origin = "lower", extent = [W_START*CC.Phonons.RY_TO_CM, W_END*CC.Phonons.RY_TO_CM, 1, N_iters])
+    plt.xlabel("Frequency [cm-1]")
+    plt.ylabel("Steps")
+    plt.colorbar()
+    plt.tight_layout()
+
+
+    plt.figure(dpi = 160)
+    plt.title("Green function with terminator")
+    plt.imshow(dynamical, aspect = "auto", origin = "lower", extent = [W_START*CC.Phonons.RY_TO_CM, W_END*CC.Phonons.RY_TO_CM, 1, N_iters])
+    plt.xlabel("Frequency [cm-1]")
+    plt.ylabel("Steps")
+    plt.colorbar()
+    plt.tight_layout()
+
+
+
+    # get colormap
+    cmap=plt.cm.viridis
+    # build cycler with 5 equally spaced colors from that colormap
+    c = cycler('color', cmap(np.linspace(0,1,N_iters)) )
+    # supply cycler to the rcParam
+    plt.rcParams["axes.prop_cycle"] = c
+
+    plt.figure(dpi = 160)
+    plt.title("Green function with terminator")
+    for i in range(N_iters):
+        plt.plot(w_array * CC.Phonons.RY_TO_CM, dynamical[i, :])
+
+    # The last one is plotted in red underlined
+    plt.plot(w_array * CC.Phonons.RY_TO_CM, dynamical[-1, :], color = "r", linewidth = 3.5)
+    plt.xlabel("Frequency [cm-1]")
+    plt.ylabel("Steps")
+    plt.tight_layout()
+
+    plt.show()
+
+
+if __name__ == "__main__":
+    print_usage()
+    main()
```

### Comparing `tdscha-1.0/scripts/tdscha-output2abc.py` & `tdscha-1.0.1/scripts/tdscha-output2abc.py`

 * *Files identical despite different names*

### Comparing `tdscha-1.0/scripts/tdscha-plot.py` & `tdscha-1.0.1/scripts/tdscha-plot.py`

 * *Files identical despite different names*

### Comparing `tdscha-1.0/setup.py` & `tdscha-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
                    extra_link_args = mpi_link_args + extra_link_args_c
                    )
 
 
 
 # Prepare the compilation of the Python Conde
 setup( name = "tdscha",
-       version = "1.0",
+       version = "1.0.1",
        description = "Time Dependent Self Consistent Harmonic Approximation",
        author = "Lorenzo Monacelli",
        url = "https://github.com/SSCHAcode/tdscha",
        packages = ["tdscha"],
        include_package_data=True,
        package_dir = {"tdscha": "Modules"},
        package_data={"": ["*.jl"]},
```

### Comparing `tdscha-1.0/tdscha.egg-info/SOURCES.txt` & `tdscha-1.0.1/tdscha.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 Modules/Parallel.py
 Modules/Perturbations.py
 Modules/StaticHessian.py
 Modules/Tools.py
 Modules/__init__.py
 Modules/tdscha_core.jl
 scripts/plot_hessian_convergence.py
-scripts/plot_lanczos_convergence.py
+scripts/tdscha-convergence-analysis.py
 scripts/tdscha-output2abc.py
 scripts/tdscha-plot.py
 tdscha.egg-info/PKG-INFO
 tdscha.egg-info/SOURCES.txt
 tdscha.egg-info/dependency_links.txt
 tdscha.egg-info/requires.txt
 tdscha.egg-info/top_level.txt
```

