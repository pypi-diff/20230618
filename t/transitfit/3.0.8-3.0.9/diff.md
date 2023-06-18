# Comparing `tmp/transitfit-3.0.8.tar.gz` & `tmp/transitfit-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transitfit-3.0.8.tar", last modified: Sat Jun 17 14:26:10 2023, max compression
+gzip compressed data, was "transitfit-3.0.9.tar", last modified: Sun Jun 18 12:29:59 2023, max compression
```

## Comparing `transitfit-3.0.8.tar` & `transitfit-3.0.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-17 14:26:10.259761 transitfit-3.0.8/
--rw-rw-r--   0 a         (1000) a         (1000)    35129 2023-05-18 21:20:57.000000 transitfit-3.0.8/LICENSE
--rw-rw-r--   0 a         (1000) a         (1000)     3944 2023-06-17 14:26:10.259761 transitfit-3.0.8/PKG-INFO
--rw-rw-r--   0 a         (1000) a         (1000)     3303 2023-05-18 21:20:57.000000 transitfit-3.0.8/README.md
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-17 14:26:10.259761 transitfit-3.0.8/filters/
--rw-rw-r--   0 a         (1000) a         (1000)      542 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/CousinsI.csv
--rw-rw-r--   0 a         (1000) a         (1000)      674 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/CousinsR.csv
--rw-rw-r--   0 a         (1000) a         (1000)      231 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/JohnsonB.csv
--rw-rw-r--   0 a         (1000) a         (1000)      341 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/JohnsonI.csv
--rw-rw-r--   0 a         (1000) a         (1000)      296 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/JohnsonR.csv
--rw-rw-r--   0 a         (1000) a         (1000)      176 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/JohnsonU.csv
--rw-rw-r--   0 a         (1000) a         (1000)      200 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/JohnsonV.csv
--rw-rw-r--   0 a         (1000) a         (1000)     8960 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/Kepler.csv
--rw-rw-r--   0 a         (1000) a         (1000)     1259 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/SLOAN_g.csv
--rw-rw-r--   0 a         (1000) a         (1000)    35084 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/SLOAN_gprime.csv
--rw-rw-r--   0 a         (1000) a         (1000)     1255 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/SLOAN_i.csv
--rw-rw-r--   0 a         (1000) a         (1000)    36720 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/SLOAN_iprime.csv
--rw-rw-r--   0 a         (1000) a         (1000)     1064 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/SLOAN_r.csv
--rw-rw-r--   0 a         (1000) a         (1000)    31574 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/SLOAN_rprime.csv
--rw-rw-r--   0 a         (1000) a         (1000)      672 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/SLOAN_u.csv
--rw-rw-r--   0 a         (1000) a         (1000)    15446 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/SLOAN_uprime.csv
--rw-rw-r--   0 a         (1000) a         (1000)     2030 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/SLOAN_z.csv
--rw-rw-r--   0 a         (1000) a         (1000)    92169 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/SLOAN_zprime.csv
--rw-rw-r--   0 a         (1000) a         (1000)     6743 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/TESS.csv
--rw-rw-r--   0 a         (1000) a         (1000)      104 2023-05-18 21:20:57.000000 transitfit-3.0.8/pyproject.toml
--rw-rw-r--   0 a         (1000) a         (1000)      897 2023-06-17 14:26:10.259761 transitfit-3.0.8/setup.cfg
--rw-rw-r--   0 a         (1000) a         (1000)     1559 2023-05-18 21:25:42.000000 transitfit-3.0.8/setup.py
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-17 14:26:10.247760 transitfit-3.0.8/transitfit/
--rw-rw-r--   0 a         (1000) a         (1000)      440 2023-06-17 14:19:14.000000 transitfit-3.0.8/transitfit/__init__.py
--rw-rw-r--   0 a         (1000) a         (1000)     7634 2023-05-18 21:20:57.000000 transitfit-3.0.8/transitfit/_ldtk_handler.py
--rw-rw-r--   0 a         (1000) a         (1000)     7687 2023-05-18 21:20:57.000000 transitfit-3.0.8/transitfit/_likelihood.py
--rw-rw-r--   0 a         (1000) a         (1000)    11790 2023-05-18 21:20:57.000000 transitfit-3.0.8/transitfit/_limb_darkening_handler.py
--rw-rw-r--   0 a         (1000) a         (1000)     8547 2023-05-18 21:25:01.000000 transitfit-3.0.8/transitfit/_paramarray.py
--rw-rw-r--   0 a         (1000) a         (1000)     2547 2023-05-18 21:25:01.000000 transitfit-3.0.8/transitfit/_params.py
--rw-rw-r--   0 a         (1000) a         (1000)    16682 2023-05-18 21:25:01.000000 transitfit-3.0.8/transitfit/_pipeline.py
--rw-rw-r--   0 a         (1000) a         (1000)     9903 2023-05-18 21:20:57.000000 transitfit-3.0.8/transitfit/_utils.py
--rw-rw-r--   0 a         (1000) a         (1000)     1644 2023-05-18 21:20:57.000000 transitfit-3.0.8/transitfit/detrender.py
--rw-rw-r--   0 a         (1000) a         (1000)     2354 2023-05-18 21:20:57.000000 transitfit-3.0.8/transitfit/detrending_funcs.py
--rw-rw-r--   0 a         (1000) a         (1000)    16505 2023-06-17 14:25:48.000000 transitfit-3.0.8/transitfit/error_analysis.py
--rw-rw-r--   0 a         (1000) a         (1000)    32649 2023-05-18 21:20:57.000000 transitfit-3.0.8/transitfit/io.py
--rw-rw-r--   0 a         (1000) a         (1000)    22728 2023-05-18 21:25:01.000000 transitfit-3.0.8/transitfit/lightcurve.py
--rw-rw-r--   0 a         (1000) a         (1000)    52943 2023-05-18 21:25:01.000000 transitfit-3.0.8/transitfit/output_handler.py
--rw-rw-r--   0 a         (1000) a         (1000)    14804 2023-05-18 21:25:01.000000 transitfit-3.0.8/transitfit/plotting.py
--rw-rw-r--   0 a         (1000) a         (1000)    25606 2023-06-13 12:31:25.000000 transitfit-3.0.8/transitfit/priorinfo.py
--rw-rw-r--   0 a         (1000) a         (1000)    72989 2023-05-18 21:25:01.000000 transitfit-3.0.8/transitfit/retriever.py
--rw-rw-r--   0 a         (1000) a         (1000)     1878 2023-05-18 21:20:57.000000 transitfit-3.0.8/transitfit/time_conversions.py
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-17 14:26:10.247760 transitfit-3.0.8/transitfit.egg-info/
--rw-rw-r--   0 a         (1000) a         (1000)     3944 2023-06-17 14:26:10.000000 transitfit-3.0.8/transitfit.egg-info/PKG-INFO
--rw-rw-r--   0 a         (1000) a         (1000)     1392 2023-06-17 14:26:10.000000 transitfit-3.0.8/transitfit.egg-info/SOURCES.txt
--rw-rw-r--   0 a         (1000) a         (1000)        1 2023-06-17 14:26:10.000000 transitfit-3.0.8/transitfit.egg-info/dependency_links.txt
--rw-rw-r--   0 a         (1000) a         (1000)        1 2023-05-18 21:21:16.000000 transitfit-3.0.8/transitfit.egg-info/not-zip-safe
--rw-rw-r--   0 a         (1000) a         (1000)      101 2023-06-17 14:26:10.000000 transitfit-3.0.8/transitfit.egg-info/requires.txt
--rw-rw-r--   0 a         (1000) a         (1000)       11 2023-06-17 14:26:10.000000 transitfit-3.0.8/transitfit.egg-info/top_level.txt
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-18 12:29:59.921537 transitfit-3.0.9/
+-rw-rw-r--   0 a         (1000) a         (1000)    35129 2023-06-18 12:28:24.000000 transitfit-3.0.9/LICENSE
+-rw-rw-r--   0 a         (1000) a         (1000)     3944 2023-06-18 12:29:59.921537 transitfit-3.0.9/PKG-INFO
+-rw-rw-r--   0 a         (1000) a         (1000)     3303 2023-06-18 12:28:24.000000 transitfit-3.0.9/README.md
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-18 12:29:59.921537 transitfit-3.0.9/filters/
+-rw-rw-r--   0 a         (1000) a         (1000)      542 2023-06-18 12:28:24.000000 transitfit-3.0.9/filters/CousinsI.csv
+-rw-rw-r--   0 a         (1000) a         (1000)      674 2023-06-18 12:28:24.000000 transitfit-3.0.9/filters/CousinsR.csv
+-rw-rw-r--   0 a         (1000) a         (1000)      231 2023-06-18 12:28:24.000000 transitfit-3.0.9/filters/JohnsonB.csv
+-rw-rw-r--   0 a         (1000) a         (1000)      341 2023-06-18 12:28:24.000000 transitfit-3.0.9/filters/JohnsonI.csv
+-rw-rw-r--   0 a         (1000) a         (1000)      296 2023-06-18 12:28:24.000000 transitfit-3.0.9/filters/JohnsonR.csv
+-rw-rw-r--   0 a         (1000) a         (1000)      176 2023-06-18 12:28:24.000000 transitfit-3.0.9/filters/JohnsonU.csv
+-rw-rw-r--   0 a         (1000) a         (1000)      200 2023-06-18 12:28:24.000000 transitfit-3.0.9/filters/JohnsonV.csv
+-rw-rw-r--   0 a         (1000) a         (1000)     8960 2023-06-18 12:28:24.000000 transitfit-3.0.9/filters/Kepler.csv
+-rw-rw-r--   0 a         (1000) a         (1000)     1259 2023-06-18 12:28:24.000000 transitfit-3.0.9/filters/SLOAN_g.csv
+-rw-rw-r--   0 a         (1000) a         (1000)    35084 2023-06-18 12:28:24.000000 transitfit-3.0.9/filters/SLOAN_gprime.csv
+-rw-rw-r--   0 a         (1000) a         (1000)     1255 2023-06-18 12:28:24.000000 transitfit-3.0.9/filters/SLOAN_i.csv
+-rw-rw-r--   0 a         (1000) a         (1000)    36720 2023-06-18 12:28:24.000000 transitfit-3.0.9/filters/SLOAN_iprime.csv
+-rw-rw-r--   0 a         (1000) a         (1000)     1064 2023-06-18 12:28:24.000000 transitfit-3.0.9/filters/SLOAN_r.csv
+-rw-rw-r--   0 a         (1000) a         (1000)    31574 2023-06-18 12:28:24.000000 transitfit-3.0.9/filters/SLOAN_rprime.csv
+-rw-rw-r--   0 a         (1000) a         (1000)      672 2023-06-18 12:28:24.000000 transitfit-3.0.9/filters/SLOAN_u.csv
+-rw-rw-r--   0 a         (1000) a         (1000)    15446 2023-06-18 12:28:24.000000 transitfit-3.0.9/filters/SLOAN_uprime.csv
+-rw-rw-r--   0 a         (1000) a         (1000)     2030 2023-06-18 12:28:24.000000 transitfit-3.0.9/filters/SLOAN_z.csv
+-rw-rw-r--   0 a         (1000) a         (1000)    92169 2023-06-18 12:28:24.000000 transitfit-3.0.9/filters/SLOAN_zprime.csv
+-rw-rw-r--   0 a         (1000) a         (1000)     6743 2023-06-18 12:28:24.000000 transitfit-3.0.9/filters/TESS.csv
+-rw-rw-r--   0 a         (1000) a         (1000)      104 2023-06-18 12:28:24.000000 transitfit-3.0.9/pyproject.toml
+-rw-rw-r--   0 a         (1000) a         (1000)      897 2023-06-18 12:29:59.921537 transitfit-3.0.9/setup.cfg
+-rw-rw-r--   0 a         (1000) a         (1000)     1559 2023-06-18 12:28:24.000000 transitfit-3.0.9/setup.py
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-18 12:29:59.917537 transitfit-3.0.9/transitfit/
+-rw-rw-r--   0 a         (1000) a         (1000)      440 2023-06-18 12:29:07.000000 transitfit-3.0.9/transitfit/__init__.py
+-rw-rw-r--   0 a         (1000) a         (1000)     7634 2023-06-18 12:28:24.000000 transitfit-3.0.9/transitfit/_ldtk_handler.py
+-rw-rw-r--   0 a         (1000) a         (1000)     7687 2023-06-18 12:28:24.000000 transitfit-3.0.9/transitfit/_likelihood.py
+-rw-rw-r--   0 a         (1000) a         (1000)    11790 2023-06-18 12:28:24.000000 transitfit-3.0.9/transitfit/_limb_darkening_handler.py
+-rw-rw-r--   0 a         (1000) a         (1000)     8547 2023-06-18 12:28:24.000000 transitfit-3.0.9/transitfit/_paramarray.py
+-rw-rw-r--   0 a         (1000) a         (1000)     2547 2023-06-18 12:28:24.000000 transitfit-3.0.9/transitfit/_params.py
+-rw-rw-r--   0 a         (1000) a         (1000)    16682 2023-06-18 12:28:24.000000 transitfit-3.0.9/transitfit/_pipeline.py
+-rw-rw-r--   0 a         (1000) a         (1000)     9903 2023-06-18 12:28:24.000000 transitfit-3.0.9/transitfit/_utils.py
+-rw-rw-r--   0 a         (1000) a         (1000)     1644 2023-06-18 12:28:24.000000 transitfit-3.0.9/transitfit/detrender.py
+-rw-rw-r--   0 a         (1000) a         (1000)     2354 2023-06-18 12:28:24.000000 transitfit-3.0.9/transitfit/detrending_funcs.py
+-rw-rw-r--   0 a         (1000) a         (1000)    18558 2023-06-18 12:28:48.000000 transitfit-3.0.9/transitfit/error_analysis.py
+-rw-rw-r--   0 a         (1000) a         (1000)    32649 2023-06-18 12:28:24.000000 transitfit-3.0.9/transitfit/io.py
+-rw-rw-r--   0 a         (1000) a         (1000)    22730 2023-06-18 12:28:24.000000 transitfit-3.0.9/transitfit/lightcurve.py
+-rw-rw-r--   0 a         (1000) a         (1000)    52944 2023-06-18 12:28:24.000000 transitfit-3.0.9/transitfit/output_handler.py
+-rw-rw-r--   0 a         (1000) a         (1000)    14804 2023-06-18 12:28:24.000000 transitfit-3.0.9/transitfit/plotting.py
+-rw-rw-r--   0 a         (1000) a         (1000)    25606 2023-06-18 12:28:24.000000 transitfit-3.0.9/transitfit/priorinfo.py
+-rw-rw-r--   0 a         (1000) a         (1000)    73404 2023-06-18 12:28:24.000000 transitfit-3.0.9/transitfit/retriever.py
+-rw-rw-r--   0 a         (1000) a         (1000)     1878 2023-06-18 12:28:24.000000 transitfit-3.0.9/transitfit/time_conversions.py
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-18 12:29:59.917537 transitfit-3.0.9/transitfit.egg-info/
+-rw-rw-r--   0 a         (1000) a         (1000)     3944 2023-06-18 12:29:59.000000 transitfit-3.0.9/transitfit.egg-info/PKG-INFO
+-rw-rw-r--   0 a         (1000) a         (1000)     1392 2023-06-18 12:29:59.000000 transitfit-3.0.9/transitfit.egg-info/SOURCES.txt
+-rw-rw-r--   0 a         (1000) a         (1000)        1 2023-06-18 12:29:59.000000 transitfit-3.0.9/transitfit.egg-info/dependency_links.txt
+-rw-rw-r--   0 a         (1000) a         (1000)        1 2023-06-18 12:29:51.000000 transitfit-3.0.9/transitfit.egg-info/not-zip-safe
+-rw-rw-r--   0 a         (1000) a         (1000)      101 2023-06-18 12:29:59.000000 transitfit-3.0.9/transitfit.egg-info/requires.txt
+-rw-rw-r--   0 a         (1000) a         (1000)       11 2023-06-18 12:29:59.000000 transitfit-3.0.9/transitfit.egg-info/top_level.txt
```

### Comparing `transitfit-3.0.8/LICENSE` & `transitfit-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/PKG-INFO` & `transitfit-3.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transitfit
-Version: 3.0.8
+Version: 3.0.9
 Summary: A package to fit exoplanet transit light curves
 Home-page: https://github.com/SPEARNET/TransitFit
 Author: Joshua Hayes and collaborators
 Author-email: Eamonn.Kerins@manchester.ac.uk
 Project-URL: Documentation, https://transitfit.readthedocs.io/en/latest/index.html
 Keywords: exoplanets,transits,fitting
 Classifier: Programming Language :: Python :: 3
```

### Comparing `transitfit-3.0.8/README.md` & `transitfit-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/filters/CousinsI.csv` & `transitfit-3.0.9/filters/CousinsI.csv`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/filters/CousinsR.csv` & `transitfit-3.0.9/filters/CousinsR.csv`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/filters/Kepler.csv` & `transitfit-3.0.9/filters/Kepler.csv`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/filters/SLOAN_g.csv` & `transitfit-3.0.9/filters/SLOAN_g.csv`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/filters/SLOAN_gprime.csv` & `transitfit-3.0.9/filters/SLOAN_gprime.csv`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/filters/SLOAN_i.csv` & `transitfit-3.0.9/filters/SLOAN_i.csv`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/filters/SLOAN_iprime.csv` & `transitfit-3.0.9/filters/SLOAN_iprime.csv`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/filters/SLOAN_r.csv` & `transitfit-3.0.9/filters/SLOAN_r.csv`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/filters/SLOAN_rprime.csv` & `transitfit-3.0.9/filters/SLOAN_rprime.csv`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/filters/SLOAN_u.csv` & `transitfit-3.0.9/filters/SLOAN_u.csv`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/filters/SLOAN_uprime.csv` & `transitfit-3.0.9/filters/SLOAN_uprime.csv`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/filters/SLOAN_z.csv` & `transitfit-3.0.9/filters/SLOAN_z.csv`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/filters/SLOAN_zprime.csv` & `transitfit-3.0.9/filters/SLOAN_zprime.csv`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/filters/TESS.csv` & `transitfit-3.0.9/filters/TESS.csv`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/setup.cfg` & `transitfit-3.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = TransitFit
-version = 3.0.6
+version = 3.0.9
 author = Joshua Hayes and collaborators
 author_email = Eamonn.Kerins@manchester.ac.uk
 description = Package for fitting of transit light curves with host-characteristic-informed limb darkening
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/SPEARNET/TransitFit
 project_urls =
```

### Comparing `transitfit-3.0.8/setup.py` & `transitfit-3.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/transitfit/_ldtk_handler.py` & `transitfit-3.0.9/transitfit/_ldtk_handler.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/transitfit/_likelihood.py` & `transitfit-3.0.9/transitfit/_likelihood.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/transitfit/_limb_darkening_handler.py` & `transitfit-3.0.9/transitfit/_limb_darkening_handler.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/transitfit/_paramarray.py` & `transitfit-3.0.9/transitfit/_paramarray.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/transitfit/_params.py` & `transitfit-3.0.9/transitfit/_params.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/transitfit/_pipeline.py` & `transitfit-3.0.9/transitfit/_pipeline.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/transitfit/_utils.py` & `transitfit-3.0.9/transitfit/_utils.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/transitfit/detrender.py` & `transitfit-3.0.9/transitfit/detrender.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/transitfit/detrending_funcs.py` & `transitfit-3.0.9/transitfit/detrending_funcs.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/transitfit/error_analysis.py` & `transitfit-3.0.9/transitfit/error_analysis.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     total_sum = 0
     for i in range(best_val_idx, 0, -1):
         total_sum += sorted_weights[i]
         if total_sum >= .6827*np.sum(sorted_weights[:best_val_idx]):
             lower_error = sorted_samples[i]-best_val
             break"""
 
-    return lower_error, upper_error
+    return -np.abs(lower_error), np.abs(upper_error)
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~#
 
 
 def make_dict(val_dict, key, vals):
     """makes dictionary using the given values. if the key already 
     exists, then the values get appended. 
@@ -85,16 +85,16 @@
 
     Returns:
         list: errors on u0, u1
     """
 
     u_err = []
     u_err.append(np.sqrt(((q[1] * q_err[0])**2)/q[0] + 4 * q[0] * q_err[1]**2))
-    u_err.append(np.sqrt(
-        (((1 - 2 * q[1]) * q_err[0])**2)/(0.25 * q[0]) + 4 * q[0] * q_err[1] ** 2))
+    u_err.append(np.abs(np.sqrt(
+        (((1 - 2 * q[1]) * q_err[0])**2)/(0.25 * q[0]) + 4 * q[0] * q_err[1] ** 2)))
 
     return u_err
 
 
 def q_to_u(q, q_err_l, q_err_u):
     """Converts q (Kipping parameters) to limb darkening parameters u.
     Handles only quadratic limb darkening currently.
@@ -104,20 +104,24 @@
         q_err_l (list): lower bound of errors on q0, q1
         q_err_u (list): upper bound of errors on q0, q1
 
     Returns:
         tuple: the values of u, lower bound on values, upper bound on values.
     """
 
+    q_err_l = np.abs(np.array(q_err_l,dtype=float))
+    q_err_u = np.abs(np.array(q_err_u,dtype=float))
+
+
     u = [2 * np.sqrt(q[0]) * q[1], np.sqrt(q[0]) * (1 - 2 * q[1])]
 
     u_err_l = q_to_u_err(q, q_err_l)
     u_err_u = q_to_u_err(q, q_err_u)
 
-    return u, u_err_l, u_err_u
+    return np.array(u,dtype=float), -np.abs(np.array(u_err_l,dtype=float)), np.abs(np.array(u_err_u,dtype=float))
 
 
 class ErrorLimits:
     """
     Initializes the error limit analysis.
 
     Args:
@@ -177,17 +181,24 @@
             if self.allow_ttv:
                 print('TTV mode detected.')
 
         else:
             self.allow_ttv = False
             self.FOLDED_MODE = False
             self.folded_params = []
+            self.priors_pkl = glob.glob(
+                self.OUTPUT_PARAMETERS_FOLDER+'/quicksaves/*priors.pkl')
+            self.priors_pkl.sort()
+            with open(self.priors_pkl[0], 'rb') as handle:
+                priors = pickle.load(handle)
 
         # The list of required parameters to analyze
         self.required_params = ['P', 't0', 'a/r*', 'inc', 'rp/r*']
+        self.limb_dark_coeffs = priors.limb_dark_coeffs#['q0','q1']#
+        self.ld_method = priors.limb_dark #'quadratic' #
         self.values = {}
 
     def handle_ttv(self):
         """ Handles the case of TTV analysis.
         """
         all_epochs = np.empty(0)
         for i, fmpk in enumerate(self.folded_mode_priors_pkl):
@@ -253,22 +264,26 @@
                 errs = get_quantiles_on_best_val(
                     samples=self.values[param_], weights=self.values[param_+'_weights'], best_val=self.values[param_+'_best'])
                 # (model.mean)
 
                 mso.write(
                     f"{p},-,-,{self.values[param_+'_best']},{errs[0]},{errs[1]}\n")
 
-                if p in {'q0', 'q1'}:
+                if p in self.limb_dark_coeffs:
                     q.append(self.values[param_+'_best']),
                     q_low.append(errs[0])
                     q_up.append(errs[1])
+            
+            if self.ld_method=='quadratic':
+                u, u_low, u_up = q_to_u(q, q_low, q_up)
 
-            u, u_low, u_up = q_to_u(q, q_low, q_up)
-            mso.write(f"u0,-,-,{u[0]},{u_low[0]},{u_up[0]}\n")
-            mso.write(f"u1,-,-,{u[1]},{u_low[1]},{u_up[1]}\n")
+                for i, p in enumerate(self.limb_dark_coeffs):
+                    mso.write(f"u{str(i)},-,-,{u[i]},{u_low[i]},{u_up[i]}\n")
+                    #mso.write(f"u0,-,-,{u[0]},{u_low[0]},{u_up[0]}\n")
+                    #mso.write(f"u1,-,-,{u[1]},{u_low[1]},{u_up[1]}\n")
 
         print(
             f"Saved results in {self.OUTPUT_PARAMETERS_FOLDER+'/'+self.MODIFIED_SUMMARY_OUTPUT}")
 
         return
 
     def get_errors(self):
@@ -318,44 +333,61 @@
                     batch_filters = selected_df['Filter'].to_list()
                     filters += batch_filters
                     for i, f in enumerate(batch_filters):
                         make_dict(self.values, param+'_'+f,
                                   result.samples[:, index[i]])
                         make_dict(self.values, param+'_'+f +
                                   '_weights', result.weights)
-                        i = 2*i  # q0 and q1 are saved as pairs in the .pkl files
-                        make_dict(self.values, 'q0'+'_'+f,
-                                  result.samples[:, index[-1]+1+i])
-                        make_dict(self.values, 'q1'+'_'+f,
-                                  result.samples[:, index[-1]+1+i+1])
-
-                        make_dict(self.values, 'q0'+'_'+f +
-                                  '_weights', result.weights)
-                        make_dict(self.values, 'q1'+'_'+f +
-                                  '_weights', result.weights)
+                        
+                        for j,u in enumerate(self.limb_dark_coeffs):
+                            i = len(self.limb_dark_coeffs)*i  
+                            # limb darkenening coeffs are saved together in the .pkl files
+                            
+                            make_dict(self.values, 'q'+str(j)+'_'+f,
+                                    result.samples[:, index[-1]+1+i])
+                            make_dict(self.values, 'q'+str(j)+'_'+f +
+                                    '_weights', result.weights)
+                            
+                            #if self.ld_method=='quadratic':
+                            """make_dict(self.values, 'q0'+'_'+f,
+                                    result.samples[:, index[-1]+1+i])
+                            make_dict(self.values, 'q1'+'_'+f,
+                                    result.samples[:, index[-1]+1+i+1])
+
+                            make_dict(self.values, 'q0'+'_'+f +
+                                    '_weights', result.weights)
+                            make_dict(self.values, 'q1'+'_'+f +
+                                    '_weights', result.weights)"""
                 
                 elif selected_df['Error'].iloc[0]=='-':
                     self.required_params.remove(param)
                 
                 else:
 
                     make_dict(self.values, param, result.samples[:, index])
                     make_dict(self.values, param+'_weights', result.weights)
 
                     if param == 'rp/r*':  # Folded mode
-                        make_dict(self.values, 'q0',
-                                  result.samples[:, index+1])
-                        make_dict(self.values, 'q1',
-                                  result.samples[:, index+2])
+                        for j,u in enumerate(self.limb_dark_coeffs):
+
+                            make_dict(self.values, 'q'+str(j),
+                                    result.samples[:, index+1])
+                            make_dict(self.values, 'q'+str(j)+'_weights', result.weights)
 
-                        make_dict(self.values, 'q0'+'_weights', result.weights)
-                        make_dict(self.values, 'q1'+'_weights', result.weights)
+                            """make_dict(self.values, 'q1',
+                                    result.samples[:, index+2])
 
+                            make_dict(self.values, 'q'+str(j)+'_weights', result.weights)
+                            make_dict(self.values, 'q1'+'_weights', result.weights)"""
+        
+        #if self.ld_method=='quadratic':
         self.required_params = self.folded_params + \
-            self.required_params+['q0', 'q1']
+            self.required_params+self.limb_dark_coeffs#['q0', 'q1']
+            
+
         filters = list(set(filters))
         filters = np.sort(np.array(filters, dtype=int))
 
         df_so = pd.read_csv(self.summary_output[0])
 
         # Getting the best_values from the summary_output.csv file
         for p in self.required_params:
@@ -372,52 +404,58 @@
         # Generating the output
         with open(self.OUTPUT_PARAMETERS_FOLDER+'/'+self.MODIFIED_SUMMARY_OUTPUT, 'w') as mso:
             mso.write('Parameter,Filter,Best,Lower_error,Upper_error\n')
             q, q_low, q_up = [], [], []
             q_dict = {}
 
             for param in self.required_params:
-                if param in {'rp/r*', 'q0', 'q1'} and len(filters) > 0:
+                if param in ['rp/r*']+self.limb_dark_coeffs and len(filters) > 0:
                     for fil in filters:
                         param_ = param+'_'+str(int(fil))
                         errs = get_quantiles_on_best_val(
                             samples=self.values[param_], weights=self.values[param_+'_weights'], best_val=self.values[param_+'_best'])
                         # (model.mean)
                         mso.write(
                             f"{param},{fil},{self.values[param_+'_best']},{errs[0]},{errs[1]}\n")
 
                 else:
                     errs = get_quantiles_on_best_val(
                         samples=self.values[param], weights=self.values[param+'_weights'], best_val=self.values[param+'_best'])
                     mso.write(
                         f"{param},-,{self.values[param+'_best']},{errs[0]},{errs[1]}\n")
 
-                    if param in {'q0', 'q1'}:
+                    if param in self.limb_dark_coeffs:
                         q.append(self.values[param+'_best']),
                         q_low.append(errs[0])
                         q_up.append(errs[1])
-            if len(q) > 0:
-                u, u_low, u_up = q_to_u(q, q_low, q_up)
-                mso.write(f"u0,-,{u[0]},{u_low[0]},{u_up[0]}\n")
-                mso.write(f"u1,-,{u[1]},{u_low[1]},{u_up[1]}\n")
-
-            elif len(filters) > 0:
-                for fil in filters:
-                    for param in ['q0', 'q1']:
-                        param_ = param+'_'+str(int(fil))
-                        errs = get_quantiles_on_best_val(
-                            samples=self.values[param_], weights=self.values[param_+'_weights'], best_val=self.values[param_+'_best'])
-
-                        q.append(self.values[param_+'_best']),
-                        q_low.append(errs[0])
-                        q_up.append(errs[1])
 
+            if self.ld_method=='quadratic':
+                if len(q) > 0:
                     u, u_low, u_up = q_to_u(q, q_low, q_up)
-                    mso.write(
-                        f"u0,{str(int(fil))},{u[0]},{u_low[0]},{u_up[0]}\n")
-                    mso.write(
-                        f"u1,{str(int(fil))},{u[1]},{u_low[1]},{u_up[1]}\n")
+                    
+                    for j,p in enumerate(self.limb_dark_coeffs):
+                        mso.write(f"u{str(j)},-,{u[j]},{u_low[j]},{u_up[j]}\n")
+                        #mso.write(f"u1,-,{u[1]},{u_low[1]},{u_up[1]}\n")
+
+                elif len(filters) > 0:
+                    for fil in filters:
+                        q, q_low, q_up = [], [], []
+                        for param in self.limb_dark_coeffs:
+                            param_ = param+'_'+str(int(fil))
+                            errs = get_quantiles_on_best_val(
+                                samples=self.values[param_], weights=self.values[param_+'_weights'], best_val=self.values[param_+'_best'])
+
+                            q.append(self.values[param_+'_best']),
+                            q_low.append(errs[0])
+                            q_up.append(errs[1])
+
+                        u, u_low, u_up = q_to_u(q, q_low, q_up)
+
+                        for j,p in enumerate(self.limb_dark_coeffs):
+                            mso.write(
+                                f"u{str(j)},{str(int(fil))},{u[j]},{u_low[j]},{u_up[j]}\n")
+                            #mso.write(f"u1,{str(int(fil))},{u[1]},{u_low[1]},{u_up[1]}\n")
 
         print(
             f"Saved results in {self.OUTPUT_PARAMETERS_FOLDER+'/'+self.MODIFIED_SUMMARY_OUTPUT}")
 
         return
```

### Comparing `transitfit-3.0.8/transitfit/io.py` & `transitfit-3.0.9/transitfit/io.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/transitfit/lightcurve.py` & `transitfit-3.0.9/transitfit/lightcurve.py`

 * *Files 0% similar despite different names*

```diff
@@ -513,16 +513,18 @@
 
     def get_phases(self, t0, P):
         '''
         Converts times into phase given t0 and P values, with t0 at phase=0
         '''
         n = (self.times - (t0 - 0.5*P))//P
 
+
         return (self.times-t0)/P - n# + 0.5
 
+
     def bin(self, cadence, residuals=None):
         '''
         Bins the light curve to a given observation cadence
 
         Parameters
         ----------
         cadence : float
```

### Comparing `transitfit-3.0.8/transitfit/output_handler.py` & `transitfit-3.0.9/transitfit/output_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,14 +259,15 @@
                     time_wise_best_curve = self.batman_models[i].light_curve(self.batman_params[i])
 
                     # get model phase:
                     n = (model_times - (self.best_model['t0'][i][0] - 0.5 * self.best_model['P'][i][0]))//self.best_model['P'][i][0]
 
                     lc_model_phase = (model_times - self.best_model['t0'][i][0])/self.best_model['P'][i][0] - n# + 0.5
 
+
                     lc_residuals = lc_flux - time_wise_best_curve
 
                     # Store the values!
                     phase += list(lc_phase)
                     flux += list(lc_flux)
                     flux_err += list(lc_flux_err)
                     residuals += list(lc_residuals)
```

### Comparing `transitfit-3.0.8/transitfit/plotting.py` & `transitfit-3.0.9/transitfit/plotting.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/transitfit/priorinfo.py` & `transitfit-3.0.9/transitfit/priorinfo.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/transitfit/retriever.py` & `transitfit-3.0.9/transitfit/retriever.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,14 +195,22 @@
         else:
             self.filters = parse_filter_list(self._filter_input, filter_delimiter)
 
         # Load in the full LightCurve data and detrending index array
         self.all_lightcurves, self.detrending_index_array = read_input_file(
             data_files, data_skiprows
         )
+
+        if median_normalisation:
+            print("Normalising lightcurves...")
+            #normalise_limits=[0.95,1.05]
+            for i in np.ndindex(self.all_lightcurves.shape):
+                scale=np.median(self.all_lightcurves[i].flux)
+                self.all_lightcurves[i].flux = self.all_lightcurves[i].flux/scale
+                self.all_lightcurves[i].errors = self.all_lightcurves[i].errors/scale
         
         if median_normalisation:
             print("Normalising lightcurves...")
             #normalise_limits=[0.95,1.05]
             for i in np.ndindex(self.all_lightcurves.shape):
                 scale=np.median(self.all_lightcurves[i].flux)
                 self.all_lightcurves[i].flux = self.all_lightcurves[i].flux/scale
```

### Comparing `transitfit-3.0.8/transitfit/time_conversions.py` & `transitfit-3.0.9/transitfit/time_conversions.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.8/transitfit.egg-info/PKG-INFO` & `transitfit-3.0.9/transitfit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transitfit
-Version: 3.0.8
+Version: 3.0.9
 Summary: A package to fit exoplanet transit light curves
 Home-page: https://github.com/SPEARNET/TransitFit
 Author: Joshua Hayes and collaborators
 Author-email: Eamonn.Kerins@manchester.ac.uk
 Project-URL: Documentation, https://transitfit.readthedocs.io/en/latest/index.html
 Keywords: exoplanets,transits,fitting
 Classifier: Programming Language :: Python :: 3
```

### Comparing `transitfit-3.0.8/transitfit.egg-info/SOURCES.txt` & `transitfit-3.0.9/transitfit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

