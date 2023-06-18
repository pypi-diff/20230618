# Comparing `tmp/ceffyl-1.25.tar.gz` & `tmp/ceffyl-1.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ceffyl-1.25.tar", last modified: Sun Jun 18 16:09:29 2023, max compression
+gzip compressed data, was "ceffyl-1.26.tar", last modified: Sun Jun 18 18:13:20 2023, max compression
```

## Comparing `ceffyl-1.25.tar` & `ceffyl-1.26.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dave      (1000) dave      (1000)        0 2023-06-18 16:09:29.239869 ceffyl-1.25/
--rw-r--r--   0 dave      (1000) dave      (1000)     1071 2023-06-18 04:43:51.000000 ceffyl-1.25/LICENSE
--rw-r--r--   0 dave      (1000) dave      (1000)     1751 2023-06-18 16:09:29.239869 ceffyl-1.25/PKG-INFO
--rw-r--r--   0 dave      (1000) dave      (1000)     1442 2023-06-18 04:43:51.000000 ceffyl-1.25/README.md
-drwxr-xr-x   0 dave      (1000) dave      (1000)        0 2023-06-18 16:09:29.233203 ceffyl-1.25/ceffyl/
--rw-r--r--   0 dave      (1000) dave      (1000)    17367 2023-06-18 04:43:51.000000 ceffyl-1.25/ceffyl/Ceffyl.py
--rw-r--r--   0 dave      (1000) dave      (1000)    19674 2023-06-18 04:43:51.000000 ceffyl-1.25/ceffyl/Sampler.py
-drwxr-xr-x   0 dave      (1000) dave      (1000)        0 2023-06-18 16:09:29.236536 ceffyl-1.25/ceffyl/bw/
--rw-r--r--   0 dave      (1000) dave      (1000)     5220 2023-06-18 04:43:51.000000 ceffyl-1.25/ceffyl/bw/bandwidths.py
--rw-r--r--   0 dave      (1000) dave      (1000)   949936 2023-06-18 16:09:28.000000 ceffyl-1.25/ceffyl/bw/cbandwidths.c
--rw-r--r--   0 dave      (1000) dave      (1000)     2097 2023-06-18 04:43:51.000000 ceffyl-1.25/ceffyl/bw/cbandwidths.pyx
--rw-r--r--   0 dave      (1000) dave      (1000)    27924 2023-06-18 04:43:51.000000 ceffyl-1.25/ceffyl/ceffyl_gp.py
--rw-r--r--   0 dave      (1000) dave      (1000)     1967 2023-06-18 04:43:51.000000 ceffyl-1.25/ceffyl/chain_utils.py
--rw-r--r--   0 dave      (1000) dave      (1000)    17028 2023-06-18 04:43:51.000000 ceffyl-1.25/ceffyl/densities.py
--rw-r--r--   0 dave      (1000) dave      (1000)     3604 2023-06-18 04:43:51.000000 ceffyl-1.25/ceffyl/metrics.py
--rw-r--r--   0 dave      (1000) dave      (1000)     4526 2023-06-18 04:43:51.000000 ceffyl-1.25/ceffyl/models.py
-drwxr-xr-x   0 dave      (1000) dave      (1000)        0 2023-06-18 16:09:29.233203 ceffyl-1.25/ceffyl.egg-info/
--rw-r--r--   0 dave      (1000) dave      (1000)     1751 2023-06-18 16:09:29.000000 ceffyl-1.25/ceffyl.egg-info/PKG-INFO
--rw-r--r--   0 dave      (1000) dave      (1000)      425 2023-06-18 16:09:29.000000 ceffyl-1.25/ceffyl.egg-info/SOURCES.txt
--rw-r--r--   0 dave      (1000) dave      (1000)        1 2023-06-18 16:09:29.000000 ceffyl-1.25/ceffyl.egg-info/dependency_links.txt
--rw-r--r--   0 dave      (1000) dave      (1000)        1 2023-06-18 04:57:33.000000 ceffyl-1.25/ceffyl.egg-info/not-zip-safe
--rw-r--r--   0 dave      (1000) dave      (1000)      300 2023-06-18 16:09:29.000000 ceffyl-1.25/ceffyl.egg-info/requires.txt
--rw-r--r--   0 dave      (1000) dave      (1000)       19 2023-06-18 16:09:29.000000 ceffyl-1.25/ceffyl.egg-info/top_level.txt
--rw-r--r--   0 dave      (1000) dave      (1000)      140 2023-06-18 04:54:44.000000 ceffyl-1.25/pyproject.toml
--rw-r--r--   0 dave      (1000) dave      (1000)       38 2023-06-18 16:09:29.239869 ceffyl-1.25/setup.cfg
--rw-r--r--   0 dave      (1000) dave      (1000)     1322 2023-06-18 16:08:28.000000 ceffyl-1.25/setup.py
+drwxr-xr-x   0 dave      (1000) dave      (1000)        0 2023-06-18 18:13:20.635400 ceffyl-1.26/
+-rw-r--r--   0 dave      (1000) dave      (1000)     1071 2023-06-18 04:43:51.000000 ceffyl-1.26/LICENSE
+-rw-r--r--   0 dave      (1000) dave      (1000)     1751 2023-06-18 18:13:20.635400 ceffyl-1.26/PKG-INFO
+-rw-r--r--   0 dave      (1000) dave      (1000)     1442 2023-06-18 04:43:51.000000 ceffyl-1.26/README.md
+drwxr-xr-x   0 dave      (1000) dave      (1000)        0 2023-06-18 18:13:20.635400 ceffyl-1.26/ceffyl/
+-rw-r--r--   0 dave      (1000) dave      (1000)    17434 2023-06-18 17:38:42.000000 ceffyl-1.26/ceffyl/Ceffyl.py
+-rw-r--r--   0 dave      (1000) dave      (1000)    19674 2023-06-18 04:43:51.000000 ceffyl-1.26/ceffyl/Sampler.py
+drwxr-xr-x   0 dave      (1000) dave      (1000)        0 2023-06-18 18:13:20.635400 ceffyl-1.26/ceffyl/bw/
+-rw-r--r--   0 dave      (1000) dave      (1000)     5220 2023-06-18 04:43:51.000000 ceffyl-1.26/ceffyl/bw/bandwidths.py
+-rw-r--r--   0 dave      (1000) dave      (1000)   949936 2023-06-18 18:13:20.000000 ceffyl-1.26/ceffyl/bw/cbandwidths.c
+-rw-r--r--   0 dave      (1000) dave      (1000)     2097 2023-06-18 04:43:51.000000 ceffyl-1.26/ceffyl/bw/cbandwidths.pyx
+-rw-r--r--   0 dave      (1000) dave      (1000)    27924 2023-06-18 04:43:51.000000 ceffyl-1.26/ceffyl/ceffyl_gp.py
+-rw-r--r--   0 dave      (1000) dave      (1000)     1967 2023-06-18 04:43:51.000000 ceffyl-1.26/ceffyl/chain_utils.py
+-rw-r--r--   0 dave      (1000) dave      (1000)    17028 2023-06-18 04:43:51.000000 ceffyl-1.26/ceffyl/densities.py
+-rw-r--r--   0 dave      (1000) dave      (1000)     3604 2023-06-18 04:43:51.000000 ceffyl-1.26/ceffyl/metrics.py
+-rw-r--r--   0 dave      (1000) dave      (1000)     4526 2023-06-18 04:43:51.000000 ceffyl-1.26/ceffyl/models.py
+drwxr-xr-x   0 dave      (1000) dave      (1000)        0 2023-06-18 18:13:20.635400 ceffyl-1.26/ceffyl.egg-info/
+-rw-r--r--   0 dave      (1000) dave      (1000)     1751 2023-06-18 18:13:20.000000 ceffyl-1.26/ceffyl.egg-info/PKG-INFO
+-rw-r--r--   0 dave      (1000) dave      (1000)      425 2023-06-18 18:13:20.000000 ceffyl-1.26/ceffyl.egg-info/SOURCES.txt
+-rw-r--r--   0 dave      (1000) dave      (1000)        1 2023-06-18 18:13:20.000000 ceffyl-1.26/ceffyl.egg-info/dependency_links.txt
+-rw-r--r--   0 dave      (1000) dave      (1000)        1 2023-06-18 04:57:33.000000 ceffyl-1.26/ceffyl.egg-info/not-zip-safe
+-rw-r--r--   0 dave      (1000) dave      (1000)      300 2023-06-18 18:13:20.000000 ceffyl-1.26/ceffyl.egg-info/requires.txt
+-rw-r--r--   0 dave      (1000) dave      (1000)       19 2023-06-18 18:13:20.000000 ceffyl-1.26/ceffyl.egg-info/top_level.txt
+-rw-r--r--   0 dave      (1000) dave      (1000)      140 2023-06-18 04:54:44.000000 ceffyl-1.26/pyproject.toml
+-rw-r--r--   0 dave      (1000) dave      (1000)       38 2023-06-18 18:13:20.635400 ceffyl-1.26/setup.cfg
+-rw-r--r--   0 dave      (1000) dave      (1000)     1322 2023-06-18 18:08:05.000000 ceffyl-1.26/setup.py
```

### Comparing `ceffyl-1.25/LICENSE` & `ceffyl-1.26/LICENSE`

 * *Files identical despite different names*

### Comparing `ceffyl-1.25/PKG-INFO` & `ceffyl-1.26/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ceffyl
-Version: 1.25
+Version: 1.26
 Summary: Software to rapidly and flexibly analyse Pulsar Timing Array data via the Generalised Factorised Likelihood (GFL)method
 Author: William G. Lamb
 Author-email: william.g.lamb@vanderbilt.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ceffyl
```

### Comparing `ceffyl-1.25/README.md` & `ceffyl-1.26/README.md`

 * *Files identical despite different names*

### Comparing `ceffyl-1.25/ceffyl/Ceffyl.py` & `ceffyl-1.26/ceffyl/Ceffyl.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,14 +300,15 @@
             s.ixgrid = np.ix_(s.psr_idx, s.freq_idxs)
 
         # save array of signals
         self.signals = signals
 
         # save complete array of parameters
         self.param_names = list(np.hstack([s.param_names for s in signals]))
+        self.params = list(np.hstack([s.params for s in signals]))
         self.ndim = len(self.param_names)
 
         # setup empty 2d grid to vectorize product of pdfs
         self._I, self._J = np.ogrid[:self.N_psrs, :self.N_freqs]
 
         # information for nested sampling
         posterior_samples, hist_cumulative, binmid = [], [], []
```

### Comparing `ceffyl-1.25/ceffyl/Sampler.py` & `ceffyl-1.26/ceffyl/Sampler.py`

 * *Files identical despite different names*

### Comparing `ceffyl-1.25/ceffyl/bw/bandwidths.py` & `ceffyl-1.26/ceffyl/bw/bandwidths.py`

 * *Files identical despite different names*

### Comparing `ceffyl-1.25/ceffyl/bw/cbandwidths.c` & `ceffyl-1.26/ceffyl/bw/cbandwidths.c`

 * *Files 2% similar despite different names*

```diff
@@ -1108,177 +1108,177 @@
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":688
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":689
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":690
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":691
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":695
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":696
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":697
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":698
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":702
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":703
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":712
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":713
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":715
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":716
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":718
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":719
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":721
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":722
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":723
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1309,42 +1309,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":725
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":726
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":727
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":729
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -4549,15 +4549,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_arr, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_cnt, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":731
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4566,29 +4566,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":732
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":731
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4599,15 +4599,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":734
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4616,29 +4616,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4649,15 +4649,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":737
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4666,29 +4666,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4699,15 +4699,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":740
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4716,29 +4716,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4749,15 +4749,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":743
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4766,29 +4766,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4799,89 +4799,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":746
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":748
+    /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":747
+    /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":925
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -4889,33 +4889,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":926
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":926
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":927
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":927
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 927, __pyx_L1_error)
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":925
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -4923,96 +4923,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":929
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":931
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":932
+    /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":932
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":931
+    /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":933
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":937
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5028,15 +5028,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":938
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -5044,53 +5044,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":939
+      /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":939
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 939, __pyx_L3_error)
 
-      /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":938
+      /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":940
+    /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":940
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 940, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 941, __pyx_L5_except_error)
@@ -5098,30 +5098,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 941, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":938
+    /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":937
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5136,15 +5136,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":943
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5160,15 +5160,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5176,53 +5176,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":945
+      /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":945
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 945, __pyx_L3_error)
 
-      /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":946
+    /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":946
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 946, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 947, __pyx_L5_except_error)
@@ -5230,30 +5230,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 947, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":944
+    /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":943
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5268,15 +5268,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":949
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5292,15 +5292,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5308,53 +5308,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":951
+      /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":951
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 951, __pyx_L3_error)
 
-      /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":952
+    /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":952
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 952, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":953
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 953, __pyx_L5_except_error)
@@ -5362,30 +5362,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 953, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":950
+    /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":949
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5400,176 +5400,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":963
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":975
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":975
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":963
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":978
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":990
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":990
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":993
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":1000
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":1000
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":1003
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":1007
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":1007
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":1010
+/* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":1014
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -19545,26 +19545,26 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 941, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../../../../../tmp/build-env-d3zg7gvq/lib/python3.9/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../../../../../tmp/build-env-d24xs9h_/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 947, __pyx_L1_error)
```

### Comparing `ceffyl-1.25/ceffyl/bw/cbandwidths.pyx` & `ceffyl-1.26/ceffyl/bw/cbandwidths.pyx`

 * *Files identical despite different names*

### Comparing `ceffyl-1.25/ceffyl/ceffyl_gp.py` & `ceffyl-1.26/ceffyl/ceffyl_gp.py`

 * *Files identical despite different names*

### Comparing `ceffyl-1.25/ceffyl/chain_utils.py` & `ceffyl-1.26/ceffyl/chain_utils.py`

 * *Files identical despite different names*

### Comparing `ceffyl-1.25/ceffyl/densities.py` & `ceffyl-1.26/ceffyl/densities.py`

 * *Files identical despite different names*

### Comparing `ceffyl-1.25/ceffyl/metrics.py` & `ceffyl-1.26/ceffyl/metrics.py`

 * *Files identical despite different names*

### Comparing `ceffyl-1.25/ceffyl/models.py` & `ceffyl-1.26/ceffyl/models.py`

 * *Files identical despite different names*

### Comparing `ceffyl-1.25/ceffyl.egg-info/PKG-INFO` & `ceffyl-1.26/ceffyl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ceffyl
-Version: 1.25
+Version: 1.26
 Summary: Software to rapidly and flexibly analyse Pulsar Timing Array data via the Generalised Factorised Likelihood (GFL)method
 Author: William G. Lamb
 Author-email: william.g.lamb@vanderbilt.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ceffyl
```

### Comparing `ceffyl-1.25/setup.py` & `ceffyl-1.26/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='ceffyl',
-    version='1.25',
+    version='1.26',
     description=('Software to rapidly and flexibly analyse Pulsar Timing ' +
                  'Array data via the Generalised Factorised Likelihood (GFL)' +
                  'method'),
     author='William G. Lamb',
     author_email='william.g.lamb@vanderbilt.edu',
     packages=['ceffyl', 'ceffyl.bw'],
     ext_modules=cythonize("ceffyl/bw/cbandwidths.pyx", include_path=["ceffyl/bw/"]),
```

