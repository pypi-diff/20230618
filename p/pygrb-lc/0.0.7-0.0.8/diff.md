# Comparing `tmp/pygrb_lc-0.0.7.tar.gz` & `tmp/pygrb_lc-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrb_lc-0.0.7.tar", last modified: Sat Jun 17 18:22:21 2023, max compression
+gzip compressed data, was "pygrb_lc-0.0.8.tar", last modified: Sun Jun 18 21:45:47 2023, max compression
```

## Comparing `pygrb_lc-0.0.7.tar` & `pygrb_lc-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:22:21.739962 pygrb_lc-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-17 18:22:09.000000 pygrb_lc-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-17 18:22:21.739962 pygrb_lc-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-17 18:22:09.000000 pygrb_lc-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-17 18:22:09.000000 pygrb_lc-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-17 18:22:21.739962 pygrb_lc-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:22:21.735962 pygrb_lc-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:22:21.739962 pygrb_lc-0.0.7/src/pygrb_lc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 18:22:09.000000 pygrb_lc-0.0.7/src/pygrb_lc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-06-17 18:22:09.000000 pygrb_lc-0.0.7/src/pygrb_lc/blind_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-17 18:22:09.000000 pygrb_lc-0.0.7/src/pygrb_lc/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-17 18:22:09.000000 pygrb_lc-0.0.7/src/pygrb_lc/crossmatching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-06-17 18:22:09.000000 pygrb_lc-0.0.7/src/pygrb_lc/furie.py
--rw-r--r--   0 runner    (1001) docker     (123)    32959 2023-06-17 18:22:09.000000 pygrb_lc-0.0.7/src/pygrb_lc/light_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-17 18:22:09.000000 pygrb_lc-0.0.7/src/pygrb_lc/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-17 18:22:09.000000 pygrb_lc-0.0.7/src/pygrb_lc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:22:21.739962 pygrb_lc-0.0.7/src/pygrb_lc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-17 18:22:21.000000 pygrb_lc-0.0.7/src/pygrb_lc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-17 18:22:21.000000 pygrb_lc-0.0.7/src/pygrb_lc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 18:22:21.000000 pygrb_lc-0.0.7/src/pygrb_lc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-17 18:22:21.000000 pygrb_lc-0.0.7/src/pygrb_lc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:22:21.739962 pygrb_lc-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 18:22:09.000000 pygrb_lc-0.0.7/tests/test_light_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 18:22:09.000000 pygrb_lc-0.0.7/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-17 18:22:09.000000 pygrb_lc-0.0.7/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:45:47.946636 pygrb_lc-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-18 21:45:47.950636 pygrb_lc-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-18 21:45:47.950636 pygrb_lc-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:45:47.946636 pygrb_lc-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:45:47.946636 pygrb_lc-0.0.8/src/pygrb_lc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/src/pygrb_lc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/src/pygrb_lc/blind_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/src/pygrb_lc/catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/src/pygrb_lc/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/src/pygrb_lc/crossmatching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/src/pygrb_lc/furie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32959 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/src/pygrb_lc/light_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/src/pygrb_lc/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/src/pygrb_lc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:45:47.946636 pygrb_lc-0.0.8/src/pygrb_lc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-18 21:45:47.000000 pygrb_lc-0.0.8/src/pygrb_lc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-18 21:45:47.000000 pygrb_lc-0.0.8/src/pygrb_lc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 21:45:47.000000 pygrb_lc-0.0.8/src/pygrb_lc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-18 21:45:47.000000 pygrb_lc-0.0.8/src/pygrb_lc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:45:47.946636 pygrb_lc-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/tests/test_light_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/tests/test_utils.py
```

### Comparing `pygrb_lc-0.0.7/LICENSE` & `pygrb_lc-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.0.7/PKG-INFO` & `pygrb_lc-0.0.8/src/pygrb_lc.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pygrb_lc
-Version: 0.0.7
+Name: pygrb-lc
+Version: 0.0.8
 Summary: Python package for GRB analysis
 Home-page: https://github.com/Jorezzz/pygrb_lc
 Author: Mozgunov Georgiy
 Author-email: georgiy99@bk.ru
 Project-URL: Bug Tracker, https://github.com/Jorezzz/pygrb_lc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,14 +22,16 @@
 pip install --upgrade pygrb_lc
 ```
 or
 ```bash
 pip3 install --upgrade pygrb_lc
 ```
 
+## Light curves
+
 Main object in this package is LightCurve object and its children. Start by creating one
 ```python
 from pygrb_lc.light_curves import LightCurve # base class for ligth curve
 
 lc = LightCurve()
 print(lc)
 ```
@@ -38,14 +40,34 @@
 import numpy as np
 
 data = np.loadtxt('test.txt')
 lc = LightCurve(data = data)
 print(lc)
 ```
 
+Base class can rebin data, subtract polynomial function, filter peaks, set intervals and load and save data to ```LIGHT_CURVE_SAVE``` folder in pickle format.
+
 There are specific classes for INTERAL/SPI-ACS and Fermi/GBM instruments. They are able to load actual data from web, you need to specify it in loading_method parameter
 ```python
 from pygrb_lc.light_curves import SPI_ACS_LightCurve, GBM_LightCurve
 
 lc1 = SPI_ACS_LightCurve('2020-01-01 00:00:00', 500, loading_method = 'web')
 lc2 = GBM_LightCurve('2020-01-01 00:00:00', ['na'], duration = 500, loading_method = 'web')
 ```
+## Furie transformations
+
+Furie transformation is performed by FurieTransformation class. It requires LightCurve object as an argument
+```python
+from pygrb_lc.furie import FurieLightCurve
+
+lc = LightCurve(data = np.loadtxt('test.txt'))
+flc = FurieLightCurve(lc, interval_t90 = (0, 10))
+
+flc.plot()
+```
+
+All classes have plot method, you can provide matplotlib.pyplot.Axes object as an argument to plot on existing plot
+```python
+fig,(ax1,ax2) = plt.subplots(2,1)
+lc.plot(ax = ax1)
+flc.plot(ax = ax2)
+```
```

### Comparing `pygrb_lc-0.0.7/README.md` & `pygrb_lc-0.0.8/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 pip install --upgrade pygrb_lc
 ```
 or
 ```bash
 pip3 install --upgrade pygrb_lc
 ```
 
+## Light curves
+
 Main object in this package is LightCurve object and its children. Start by creating one
 ```python
 from pygrb_lc.light_curves import LightCurve # base class for ligth curve
 
 lc = LightCurve()
 print(lc)
 ```
@@ -23,14 +25,34 @@
 import numpy as np
 
 data = np.loadtxt('test.txt')
 lc = LightCurve(data = data)
 print(lc)
 ```
 
+Base class can rebin data, subtract polynomial function, filter peaks, set intervals and load and save data to ```LIGHT_CURVE_SAVE``` folder in pickle format.
+
 There are specific classes for INTERAL/SPI-ACS and Fermi/GBM instruments. They are able to load actual data from web, you need to specify it in loading_method parameter
 ```python
 from pygrb_lc.light_curves import SPI_ACS_LightCurve, GBM_LightCurve
 
 lc1 = SPI_ACS_LightCurve('2020-01-01 00:00:00', 500, loading_method = 'web')
 lc2 = GBM_LightCurve('2020-01-01 00:00:00', ['na'], duration = 500, loading_method = 'web')
 ```
+## Furie transformations
+
+Furie transformation is performed by FurieTransformation class. It requires LightCurve object as an argument
+```python
+from pygrb_lc.furie import FurieLightCurve
+
+lc = LightCurve(data = np.loadtxt('test.txt'))
+flc = FurieLightCurve(lc, interval_t90 = (0, 10))
+
+flc.plot()
+```
+
+All classes have plot method, you can provide matplotlib.pyplot.Axes object as an argument to plot on existing plot
+```python
+fig,(ax1,ax2) = plt.subplots(2,1)
+lc.plot(ax = ax1)
+flc.plot(ax = ax2)
+```
```

### Comparing `pygrb_lc-0.0.7/setup.cfg` & `pygrb_lc-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pygrb_lc
-version = 0.0.7
+version = 0.0.8
 author = Mozgunov Georgiy
 author_email = georgiy99@bk.ru
 description = Python package for GRB analysis
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Jorezzz/pygrb_lc
 project_urls =
```

### Comparing `pygrb_lc-0.0.7/src/pygrb_lc/blind_search.py` & `pygrb_lc-0.0.8/src/pygrb_lc/blind_search.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.0.7/src/pygrb_lc/config.py` & `pygrb_lc-0.0.8/src/pygrb_lc/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,10 +27,11 @@
     'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:77.0) Gecko/20100101 Firefox/77.0',
     'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_5) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.97 Safari/537.36',
     'Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:77.0) Gecko/20100101 Firefox/77.0',
     'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.97 Safari/537.36',
 ]
 
 GBM_DETECTOR_CODES = {0:'n0',1:'n1',2:'n2',3:'n3',4:'n4',5:'n5',6:'n6',7:'n7',8:'n8',9:'n9',10:'na',11:'nb',12:'b0',13:'b1'}
+GBM_DETECTORS = [item for item in GBM_DETECTOR_CODES.values()]
 
 logging.basicConfig(format='%(asctime)s.%(msecs)03d %(levelname)s %(module)s - %(funcName)s: %(message)s', filename=f'{LOGS_PATH}log.log',
                     level=logging.INFO, datefmt='%Y-%m-%d %H:%M:%S')
```

### Comparing `pygrb_lc-0.0.7/src/pygrb_lc/crossmatching.py` & `pygrb_lc-0.0.8/src/pygrb_lc/crossmatching.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.0.7/src/pygrb_lc/furie.py` & `pygrb_lc-0.0.8/src/pygrb_lc/furie.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,28 +2,32 @@
 import matplotlib.pyplot as plt
 import matplotlib as mpl
 from .light_curves import LightCurve
 from scipy.stats import chi2
 from typing import Callable, Iterable
 
 
-def make_pds(signal, time_step, pad_size = None):
+def make_pds(signal, time_step, total_counts = None, pad_size = None):
     '''
     Get Power Density Spectrum from signal
     Args:
         signal (np.array): input signal
         time_step (float): time step
+        total_counts (int): total counts in signal, if None uses np.sum(signal)
         pad_size (int): number of bins to pad, if None then doesn't pad
     '''
     mean = np.mean(signal)
     if pad_size is not None:
         signal = np.pad(signal, (pad_size - signal.shape[0], 0), 'constant')
         
+    if total_counts is None:
+        total_counts = np.sum(signal)
+
     freqs = np.fft.fftfreq(signal.shape[0], time_step)
-    ps = 2*np.abs(np.fft.fft(signal - mean))**(2)/np.sum(signal)
+    ps = 2*np.abs(np.fft.fft(signal - mean))**(2)/total_counts
     mask = (freqs>0)
     
     return freqs[mask], ps[mask]
 
 def group_log_bins(freqs: np.array, ps: np.array, N_bins: int = 30, step: float = None, log_scale: np.array = None):
     '''
     Group bins in log scale
@@ -80,26 +84,26 @@
         
         self.bkg_intervals = bkg_intervals
         self.interval_t90 = interval_t90
 
         rebined_param = np.polyfit(self.light_curve.rebin(bkg_substraction_resolution).set_intervals(*bkg_intervals).times,self.light_curve.rebin(bkg_substraction_resolution).set_intervals(*bkg_intervals).signal,bkg_polynom_degree)
         rebined_param = rebined_param * (self.light_curve.original_resolution/self.light_curve.resolution)
         self.rebined_param = rebined_param
-        self.bkg_mean = np.mean(self.light_curve.rebin().set_intervals(*bkg_intervals).signal)
+        self.N = np.sum(self.light_curve.rebin().set_intervals(*bkg_intervals).signal)
 
         signal = self.light_curve.rebin().substract_polynom(rebined_param).set_intervals(interval_t90).signal
         
 
         if window is not None:
             signal = signal * window(signal.shape[0])
 
-        self.freqs, self.ps =  make_pds(signal + self.bkg_mean, self.light_curve.original_resolution, pad_size)
+        self.freqs, self.ps =  make_pds(signal, self.light_curve.original_resolution, self.N, pad_size)
         self.freqs_err, self.ps_err = np.full(self.freqs.shape[0], 0), np.sqrt(self.ps)
 
-    def plot(self, kind: str = 'scatter', logx: bool = True, logy: bool = True, N_bins: int = 30, ax: mpl.axes.Axes = None, **kwargs):
+    def plot(self, kind: str = 'scatter', subtract_poisson = False, logx: bool = True, logy: bool = True, N_bins: int = 30, ax: mpl.axes.Axes = None, **kwargs):
         '''
         Plot PDS
         Args:
             kind (str, optional): plotting method
             logx (bool, optional): log x axis, defaults to True
             logy (bool, optional): log y axis, defaults to True
             N_bins (int, optional): number of bins, if None - plots without grouping
@@ -107,14 +111,17 @@
             kwargs (dict, optional): keyword arguments for plotting used by matplotlib.pyplot.plot
         '''
         if N_bins is None:
             x,x_err,y,y_err = self.freqs, self.freqs_err, self.ps, self.ps_err
         else:
             x,x_err,y,y_err = group_log_bins(self.freqs, self.ps, N_bins)
 
+        if subtract_poisson:
+            y = y - 2
+            
         if ax is None:
             if kind == 'plot':
                 plt.plot(x, y, **kwargs)
             elif kind == 'errorbar':
                 plt.errorbar(x, y, xerr=x_err, yerr=y_err, fmt = 'o', **kwargs)
             elif kind == 'scatter':
                 plt.scatter(x, y, **kwargs)
@@ -138,16 +145,8 @@
                 ax.step(x, y, **kwargs)
             else:
                 raise NotImplementedError(f"Plotting method '{kind}' not supported")
             
             if logx:
                 ax.set_xscale('log')
             if logy:
-                ax.set_yscale('log')
-                
-        
-
-
-        
-
-
-    
+                ax.set_yscale('log')
```

### Comparing `pygrb_lc-0.0.7/src/pygrb_lc/light_curves.py` & `pygrb_lc-0.0.8/src/pygrb_lc/light_curves.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import pandas as pd
 import datetime
 import numpy as np
-from .config import LIGHT_CURVE_SAVE, GBM_DETECTOR_CODES, logging
+from .config import LIGHT_CURVE_SAVE, GBM_DETECTOR_CODES, logging, GBM_DETECTORS
 from astropy.io import fits
 import matplotlib.pyplot as plt
 import matplotlib as mpl
 from .time import change_fermi_seconds, change_utc
 from .utils import get_first_intersection, is_iterable, retry
 import pickle
 from .config import ACS_DATA_PATH
@@ -706,15 +706,15 @@
         plt.axvline(t_5_high)
         plt.axvline(t_95_low)
         plt.axvline(t_95_high)
 
     return t_90, (-negative_err, positive_err)
 
 def plot_gbm_all_detectors(center_time: str, duration: float, binning: float = 0.5):
-    detector_list = [x for _,x in GBM_DETECTOR_CODES.items() if x[0] == 'n']
+    detector_list = [x for x in GBM_DETECTORS if x[0] == 'n']
     data = {}
 
     fig, ax = plt.subplots(4,3,figsize=(30,30))
     ax = ax.reshape(-1,)
     for i, detector in enumerate(detector_list[:-2]):
         lc = GBM_LightCurve(center_time, [detector], duration = duration)
         lc.rebin(0.5).plot(ax=ax[i], label = detector)
```

### Comparing `pygrb_lc-0.0.7/src/pygrb_lc/time.py` & `pygrb_lc-0.0.8/src/pygrb_lc/time.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.0.7/src/pygrb_lc/utils.py` & `pygrb_lc-0.0.8/src/pygrb_lc/utils.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.0.7/src/pygrb_lc.egg-info/PKG-INFO` & `pygrb_lc-0.0.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pygrb-lc
-Version: 0.0.7
+Name: pygrb_lc
+Version: 0.0.8
 Summary: Python package for GRB analysis
 Home-page: https://github.com/Jorezzz/pygrb_lc
 Author: Mozgunov Georgiy
 Author-email: georgiy99@bk.ru
 Project-URL: Bug Tracker, https://github.com/Jorezzz/pygrb_lc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,14 +22,16 @@
 pip install --upgrade pygrb_lc
 ```
 or
 ```bash
 pip3 install --upgrade pygrb_lc
 ```
 
+## Light curves
+
 Main object in this package is LightCurve object and its children. Start by creating one
 ```python
 from pygrb_lc.light_curves import LightCurve # base class for ligth curve
 
 lc = LightCurve()
 print(lc)
 ```
@@ -38,14 +40,34 @@
 import numpy as np
 
 data = np.loadtxt('test.txt')
 lc = LightCurve(data = data)
 print(lc)
 ```
 
+Base class can rebin data, subtract polynomial function, filter peaks, set intervals and load and save data to ```LIGHT_CURVE_SAVE``` folder in pickle format.
+
 There are specific classes for INTERAL/SPI-ACS and Fermi/GBM instruments. They are able to load actual data from web, you need to specify it in loading_method parameter
 ```python
 from pygrb_lc.light_curves import SPI_ACS_LightCurve, GBM_LightCurve
 
 lc1 = SPI_ACS_LightCurve('2020-01-01 00:00:00', 500, loading_method = 'web')
 lc2 = GBM_LightCurve('2020-01-01 00:00:00', ['na'], duration = 500, loading_method = 'web')
 ```
+## Furie transformations
+
+Furie transformation is performed by FurieTransformation class. It requires LightCurve object as an argument
+```python
+from pygrb_lc.furie import FurieLightCurve
+
+lc = LightCurve(data = np.loadtxt('test.txt'))
+flc = FurieLightCurve(lc, interval_t90 = (0, 10))
+
+flc.plot()
+```
+
+All classes have plot method, you can provide matplotlib.pyplot.Axes object as an argument to plot on existing plot
+```python
+fig,(ax1,ax2) = plt.subplots(2,1)
+lc.plot(ax = ax1)
+flc.plot(ax = ax2)
+```
```

### Comparing `pygrb_lc-0.0.7/tests/test_utils.py` & `pygrb_lc-0.0.8/tests/test_utils.py`

 * *Files identical despite different names*

