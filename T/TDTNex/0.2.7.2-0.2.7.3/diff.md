# Comparing `tmp/TDTNex-0.2.7.2.tar.gz` & `tmp/TDTNex-0.2.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TDTNex-0.2.7.2.tar", last modified: Mon Mar 13 18:55:50 2023, max compression
+gzip compressed data, was "TDTNex-0.2.7.3.tar", last modified: Sun Jun 18 10:36:27 2023, max compression
```

## Comparing `TDTNex-0.2.7.2.tar` & `TDTNex-0.2.7.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2023-03-13 18:55:50.404251 TDTNex-0.2.7.2/
--rw-r--r--   0 matthew   (1000) matthew   (1000)     2163 2020-03-31 12:57:27.000000 TDTNex-0.2.7.2/.gitignore
--rw-r--r--   0 matthew   (1000) matthew   (1000)     1023 2020-03-29 19:51:03.000000 TDTNex-0.2.7.2/LICENSE
--rw-r--r--   0 matthew   (1000) matthew   (1000)      483 2023-03-13 18:55:50.404251 TDTNex-0.2.7.2/PKG-INFO
--rw-r--r--   0 matthew   (1000) matthew   (1000)       86 2020-03-29 19:43:28.000000 TDTNex-0.2.7.2/README.md
-drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2023-03-13 18:55:50.403251 TDTNex-0.2.7.2/TDTNex/
--rw-r--r--   0 matthew   (1000) matthew   (1000)    47836 2023-03-13 18:47:34.000000 TDTNex-0.2.7.2/TDTNex/TDTNexReader.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)       55 2020-03-31 10:39:18.000000 TDTNex-0.2.7.2/TDTNex/__init__.py
-drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2023-03-13 18:55:50.404251 TDTNex-0.2.7.2/TDTNex.egg-info/
--rw-r--r--   0 matthew   (1000) matthew   (1000)      483 2023-03-13 18:55:50.000000 TDTNex-0.2.7.2/TDTNex.egg-info/PKG-INFO
--rw-r--r--   0 matthew   (1000) matthew   (1000)      234 2023-03-13 18:55:50.000000 TDTNex-0.2.7.2/TDTNex.egg-info/SOURCES.txt
--rw-r--r--   0 matthew   (1000) matthew   (1000)        1 2023-03-13 18:55:50.000000 TDTNex-0.2.7.2/TDTNex.egg-info/dependency_links.txt
--rw-r--r--   0 matthew   (1000) matthew   (1000)       32 2023-03-13 18:55:50.000000 TDTNex-0.2.7.2/TDTNex.egg-info/requires.txt
--rw-r--r--   0 matthew   (1000) matthew   (1000)        7 2023-03-13 18:55:50.000000 TDTNex-0.2.7.2/TDTNex.egg-info/top_level.txt
--rw-r--r--   0 matthew   (1000) matthew   (1000)      608 2023-03-13 18:55:22.000000 TDTNex-0.2.7.2/pyproject.toml
--rw-r--r--   0 matthew   (1000) matthew   (1000)       38 2023-03-13 18:55:50.404251 TDTNex-0.2.7.2/setup.cfg
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2023-06-18 10:36:27.563299 TDTNex-0.2.7.3/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     2163 2020-03-31 12:57:27.000000 TDTNex-0.2.7.3/.gitignore
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     1023 2020-03-29 19:51:03.000000 TDTNex-0.2.7.3/LICENSE
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      483 2023-06-18 10:36:27.563299 TDTNex-0.2.7.3/PKG-INFO
+-rw-r--r--   0 matthew   (1000) matthew   (1000)       86 2020-03-29 19:43:28.000000 TDTNex-0.2.7.3/README.md
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2023-06-18 10:36:27.563299 TDTNex-0.2.7.3/TDTNex/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)    47883 2023-06-17 14:34:11.000000 TDTNex-0.2.7.3/TDTNex/TDTNexReader.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)       55 2020-03-31 10:39:18.000000 TDTNex-0.2.7.3/TDTNex/__init__.py
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2023-06-18 10:36:27.563299 TDTNex-0.2.7.3/TDTNex.egg-info/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      483 2023-06-18 10:36:27.000000 TDTNex-0.2.7.3/TDTNex.egg-info/PKG-INFO
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      234 2023-06-18 10:36:27.000000 TDTNex-0.2.7.3/TDTNex.egg-info/SOURCES.txt
+-rw-r--r--   0 matthew   (1000) matthew   (1000)        1 2023-06-18 10:36:27.000000 TDTNex-0.2.7.3/TDTNex.egg-info/dependency_links.txt
+-rw-r--r--   0 matthew   (1000) matthew   (1000)       32 2023-06-18 10:36:27.000000 TDTNex-0.2.7.3/TDTNex.egg-info/requires.txt
+-rw-r--r--   0 matthew   (1000) matthew   (1000)        7 2023-06-18 10:36:27.000000 TDTNex-0.2.7.3/TDTNex.egg-info/top_level.txt
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      608 2023-06-17 14:36:50.000000 TDTNex-0.2.7.3/pyproject.toml
+-rw-r--r--   0 matthew   (1000) matthew   (1000)       38 2023-06-18 10:36:27.563299 TDTNex-0.2.7.3/setup.cfg
```

### Comparing `TDTNex-0.2.7.2/.gitignore` & `TDTNex-0.2.7.3/.gitignore`

 * *Files identical despite different names*

### Comparing `TDTNex-0.2.7.2/LICENSE` & `TDTNex-0.2.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `TDTNex-0.2.7.2/TDTNex/TDTNexReader.py` & `TDTNex-0.2.7.3/TDTNex/TDTNexReader.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,14 +313,15 @@
         try:
             iter(times)
         except TypeError:
             times=[times]
         nsnips = int(np.array([g.TDTts.between(t-lpad,t+rpad).sum() for t in times]).sum())
         if nsnips<1:
             print("fewer than 1 snips")
+            return (None,None,None,(None,None))
         raster_segs = np.zeros((nsnips,30,2))
         # do the xs on the raster_segs collection just 0-30
         raster_segs[:,:,0]=np.r_[0:30]
         evntsArray = np.zeros((nsnips,))
         evnts = []
         rates = np.zeros((len(times),len(bins)-1))
         _seg_idx=0
@@ -713,14 +714,15 @@
             times = g.loc[_mask,'TDTts'].values
             times = times[(times>lpad)&(times<self._tdt_dur-rpad)]
             f,ax = plt.subplots(1,1)
 
         # if there are a ton of spikes, randomly select times upto MaxN
         if len(times)>MaxN:
             from numpy.random import default_rng 
+
             rng = default_rng()
             times = rng.choice(times,MaxN,replace=False)
 
         # # Create a vector from 0 up to nsamples
         sample_idx = np.arange(nsamples)
 
         # # Calculate the index of the first sample for each chunk
@@ -971,15 +973,15 @@
             SC_cnt = 0
             for ii,(sc,g) in enumerate(wg.groupby('NEXSC')):
                 if sc==0:
                     continue
                 g_mask = g.TDTts.between(*times)
                 if g_mask.sum()>0:
                     axar[i].eventplot(g[g_mask]['TDTts'].values, 
-                                      lineoffsets=(0.3*(SC_count/nm_units_here))+0.65,
+                                      lineoffsets=(0.3*(SC_cnt/nm_units_here))+0.65,
                                       linelengths=0.3/nm_units_here,
                                       transform = axar[i].get_xaxis_transform(),
                                       color = cmap(SC_cnt/nm_units_here))
                     segs = np.zeros(self.waveforms[(wn,sc)][g_mask,:].shape+(2,))
                     segs[:,:,0] = np.r_[0:30]
                     segs[:,:,1] = self.waveforms[(wn,sc)][g_mask,:]
                     axins = axar[i].inset_axes([0.82,(SC_cnt)/nm_units_here,0.18,1/nm_units_here])
```

### Comparing `TDTNex-0.2.7.2/pyproject.toml` & `TDTNex-0.2.7.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "TDTNex"
-version = "0.2.7.2"
+version = "0.2.7.3"
 authors = [
   { name="Matthew Perkins", email="matthew.perkins@mssm.edu" },
   ]
   description = "To add OfflineSorter codes to TDT blocks"
   readme = "README.md"
   requires-python = ">=3.7"
   classifiers = [
```

