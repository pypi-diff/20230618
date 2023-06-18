# Comparing `tmp/nais-processor-0.0.8.tar.gz` & `tmp/nais-processor-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nais-processor-0.0.8.tar", last modified: Wed Oct  5 16:57:29 2022, max compression
+gzip compressed data, was "dist/nais-processor-0.0.9.tar", last modified: Wed Oct  5 22:23:53 2022, max compression
```

## Comparing `nais-processor-0.0.8.tar` & `nais-processor-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 jlam      (1000) jlam      (1000)        0 2022-10-05 16:57:29.000000 nais-processor-0.0.8/
--rw-r--r--   0 jlam      (1000) jlam      (1000)    35149 2020-10-09 14:04:08.000000 nais-processor-0.0.8/LICENSE.txt
--rw-rw-r--   0 jlam      (1000) jlam      (1000)       57 2022-10-04 22:22:33.000000 nais-processor-0.0.8/MANIFEST.in
--rw-rw-r--   0 jlam      (1000) jlam      (1000)     5436 2022-10-05 16:57:29.000000 nais-processor-0.0.8/PKG-INFO
--rw-rw-r--   0 jlam      (1000) jlam      (1000)     5140 2022-10-05 10:01:01.000000 nais-processor-0.0.8/README.md
-drwxrwxr-x   0 jlam      (1000) jlam      (1000)        0 2022-10-05 16:57:29.000000 nais-processor-0.0.8/docs/
--rw-rw-r--   0 jlam      (1000) jlam      (1000)   104420 2022-10-05 16:52:32.000000 nais-processor-0.0.8/docs/index.html
--rw-rw-r--   0 jlam      (1000) jlam      (1000)       38 2022-10-05 16:57:29.000000 nais-processor-0.0.8/setup.cfg
--rw-rw-r--   0 jlam      (1000) jlam      (1000)      673 2022-10-05 16:51:42.000000 nais-processor-0.0.8/setup.py
--rw-rw-r--   0 jlam      (1000) jlam      (1000)   247143 2022-10-04 10:30:43.000000 nais-processor-0.0.8/small_img.png
-drwxrwxr-x   0 jlam      (1000) jlam      (1000)        0 2022-10-05 16:57:29.000000 nais-processor-0.0.8/src/
-drwxrwxr-x   0 jlam      (1000) jlam      (1000)        0 2022-10-05 16:57:29.000000 nais-processor-0.0.8/src/nais_processor.egg-info/
--rw-rw-r--   0 jlam      (1000) jlam      (1000)     5436 2022-10-05 16:57:29.000000 nais-processor-0.0.8/src/nais_processor.egg-info/PKG-INFO
--rw-rw-r--   0 jlam      (1000) jlam      (1000)      303 2022-10-05 16:57:29.000000 nais-processor-0.0.8/src/nais_processor.egg-info/SOURCES.txt
--rw-rw-r--   0 jlam      (1000) jlam      (1000)        1 2022-10-05 16:57:29.000000 nais-processor-0.0.8/src/nais_processor.egg-info/dependency_links.txt
--rw-rw-r--   0 jlam      (1000) jlam      (1000)       74 2022-10-05 16:57:29.000000 nais-processor-0.0.8/src/nais_processor.egg-info/requires.txt
--rw-rw-r--   0 jlam      (1000) jlam      (1000)       15 2022-10-05 16:57:29.000000 nais-processor-0.0.8/src/nais_processor.egg-info/top_level.txt
--rw-rw-r--   0 jlam      (1000) jlam      (1000)    51556 2022-10-05 16:55:49.000000 nais-processor-0.0.8/src/nais_processor.py
+drwxrwxr-x   0 jlam      (1000) jlam      (1000)        0 2022-10-05 22:23:53.000000 nais-processor-0.0.9/
+-rw-r--r--   0 jlam      (1000) jlam      (1000)    35149 2020-10-09 14:04:08.000000 nais-processor-0.0.9/LICENSE.txt
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)       57 2022-10-04 22:22:33.000000 nais-processor-0.0.9/MANIFEST.in
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)     5436 2022-10-05 22:23:53.000000 nais-processor-0.0.9/PKG-INFO
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)     5140 2022-10-05 10:01:01.000000 nais-processor-0.0.9/README.md
+drwxrwxr-x   0 jlam      (1000) jlam      (1000)        0 2022-10-05 22:23:53.000000 nais-processor-0.0.9/docs/
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)   104474 2022-10-05 22:23:14.000000 nais-processor-0.0.9/docs/index.html
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)       38 2022-10-05 22:23:53.000000 nais-processor-0.0.9/setup.cfg
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)      673 2022-10-05 22:23:40.000000 nais-processor-0.0.9/setup.py
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)   247143 2022-10-04 10:30:43.000000 nais-processor-0.0.9/small_img.png
+drwxrwxr-x   0 jlam      (1000) jlam      (1000)        0 2022-10-05 22:23:53.000000 nais-processor-0.0.9/src/
+drwxrwxr-x   0 jlam      (1000) jlam      (1000)        0 2022-10-05 22:23:53.000000 nais-processor-0.0.9/src/nais_processor.egg-info/
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)     5436 2022-10-05 22:23:53.000000 nais-processor-0.0.9/src/nais_processor.egg-info/PKG-INFO
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)      303 2022-10-05 22:23:53.000000 nais-processor-0.0.9/src/nais_processor.egg-info/SOURCES.txt
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)        1 2022-10-05 22:23:53.000000 nais-processor-0.0.9/src/nais_processor.egg-info/dependency_links.txt
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)       74 2022-10-05 22:23:53.000000 nais-processor-0.0.9/src/nais_processor.egg-info/requires.txt
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)       15 2022-10-05 22:23:53.000000 nais-processor-0.0.9/src/nais_processor.egg-info/top_level.txt
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)    51586 2022-10-05 22:19:20.000000 nais-processor-0.0.9/src/nais_processor.py
```

### Comparing `nais-processor-0.0.8/LICENSE.txt` & `nais-processor-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nais-processor-0.0.8/PKG-INFO` & `nais-processor-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nais-processor
-Version: 0.0.8
+Version: 0.0.9
 Summary: Code to process ion spectrometer data files
 Home-page: https://github.com/jlpl/nais-processor
 Author: Janne Lampilahti
 Author-email: janne.lampilahti@helsinki.fi
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `nais-processor-0.0.8/README.md` & `nais-processor-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nais-processor-0.0.8/docs/index.html` & `nais-processor-0.0.9/docs/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -694,24 +694,24 @@
 
             # If all parameters are NaN
             # e.g. sensor is broken
             if (np.all(np.isnan(flow_df)) |
                 np.all(np.isnan(p_df)) |
                 np.all(np.isnan(t_df))):
                 return None
-            
-            # Sanity check the values
-            t_df.where(~((t_df&lt;=223.)|(t_df&gt;=353.)),np.nan)
-            p_df.where(~((p_df&lt;=37000.)|(p_df&gt;=121000.)),np.nan)
-            flow_df.where(~((flow_df&lt;=30.)|(flow_df&gt;=80.)),np.nan)
 
-            # Interpolate out the NaN values using the sane data
-            t_df = t_df.interpolate().values.flatten()
-            p_df = p_df.interpolate().values.flatten()
-            flow_df = flow_df.interpolate().values.flatten()
+            # Interpolate out NaNs
+            t_df = t_df.interpolate(method=&#34;nearest&#34;)
+            p_df = p_df.interpolate(method=&#34;nearest&#34;)
+            flow_df = flow_df.interpolate(method=&#34;nearest&#34;)
+
+            # Sanity check the values
+            t_df = t_df.where(~((t_df&lt;=223.)|(t_df&gt;=353.)),np.nan).values.flatten()
+            p_df = p_df.where(~((p_df&lt;=37000.)|(p_df&gt;=121000.)),np.nan).values.flatten()
+            flow_df = flow_df.where(~((flow_df&lt;=48.)|(flow_df&gt;=60.)),np.nan).values.flatten()
 
             # Correct the number concentrations to standard conditions (optional)
             if (sealevel_corr):
                 stp_corr_df = (pres_ref*t_df)/(temp_ref*p_df)
                 neg_df = (stp_corr_df*neg_df.T).T
                 pos_df = (stp_corr_df*pos_df.T).T
```

#### html2text {}

```diff
@@ -701,23 +701,26 @@
             # If all parameters are NaN
             # e.g. sensor is broken
             if (np.all(np.isnan(flow_df)) |
                 np.all(np.isnan(p_df)) |
                 np.all(np.isnan(t_df))):
                 return None
 
-            # Sanity check the values
-            t_df.where(~((t_df<=223.)|(t_df>=353.)),np.nan)
-            p_df.where(~((p_df<=37000.)|(p_df>=121000.)),np.nan)
-            flow_df.where(~((flow_df<=30.)|(flow_df>=80.)),np.nan)
+            # Interpolate out NaNs
+            t_df = t_df.interpolate(method="nearest")
+            p_df = p_df.interpolate(method="nearest")
+            flow_df = flow_df.interpolate(method="nearest")
 
-            # Interpolate out the NaN values using the sane data
-            t_df = t_df.interpolate().values.flatten()
-            p_df = p_df.interpolate().values.flatten()
-            flow_df = flow_df.interpolate().values.flatten()
+            # Sanity check the values
+            t_df = t_df.where(~((t_df<=223.)|
+(t_df>=353.)),np.nan).values.flatten()
+            p_df = p_df.where(~((p_df<=37000.)|
+(p_df>=121000.)),np.nan).values.flatten()
+            flow_df = flow_df.where(~((flow_df<=48.)|
+(flow_df>=60.)),np.nan).values.flatten()
 
             # Correct the number concentrations to standard conditions
 (optional)
             if (sealevel_corr):
                 stp_corr_df = (pres_ref*t_df)/(temp_ref*p_df)
                 neg_df = (stp_corr_df*neg_df.T).T
                 pos_df = (stp_corr_df*pos_df.T).T
```

### Comparing `nais-processor-0.0.8/setup.py` & `nais-processor-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md","r") as fh: 
     long_description = fh.read()
 
 setup(
     name="nais-processor",
-    version="0.0.8",
+    version="0.0.9",
     description='Code to process ion spectrometer data files',
     py_modules=["nais_processor"],
     package_dir={'':'src'},
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires = [
         "pandas >= 1.1.0",
```

### Comparing `nais-processor-0.0.8/small_img.png` & `nais-processor-0.0.9/small_img.png`

 * *Files identical despite different names*

### Comparing `nais-processor-0.0.8/src/nais_processor.egg-info/PKG-INFO` & `nais-processor-0.0.9/src/nais_processor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nais-processor
-Version: 0.0.8
+Version: 0.0.9
 Summary: Code to process ion spectrometer data files
 Home-page: https://github.com/jlpl/nais-processor
 Author: Janne Lampilahti
 Author-email: janne.lampilahti@helsinki.fi
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `nais-processor-0.0.8/src/nais_processor.py` & `nais-processor-0.0.9/src/nais_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -666,24 +666,24 @@
 
             # If all parameters are NaN
             # e.g. sensor is broken
             if (np.all(np.isnan(flow_df)) |
                 np.all(np.isnan(p_df)) |
                 np.all(np.isnan(t_df))):
                 return None
-            
-            # Sanity check the values
-            t_df.where(~((t_df<=223.)|(t_df>=353.)),np.nan)
-            p_df.where(~((p_df<=37000.)|(p_df>=121000.)),np.nan)
-            flow_df.where(~((flow_df<=30.)|(flow_df>=80.)),np.nan)
 
-            # Interpolate out the NaN values using the sane data
-            t_df = t_df.interpolate().values.flatten()
-            p_df = p_df.interpolate().values.flatten()
-            flow_df = flow_df.interpolate().values.flatten()
+            # Interpolate out NaNs
+            t_df = t_df.interpolate(method="nearest")
+            p_df = p_df.interpolate(method="nearest")
+            flow_df = flow_df.interpolate(method="nearest")
+
+            # Sanity check the values
+            t_df = t_df.where(~((t_df<=223.)|(t_df>=353.)),np.nan).values.flatten()
+            p_df = p_df.where(~((p_df<=37000.)|(p_df>=121000.)),np.nan).values.flatten()
+            flow_df = flow_df.where(~((flow_df<=48.)|(flow_df>=60.)),np.nan).values.flatten()
 
             # Correct the number concentrations to standard conditions (optional)
             if (sealevel_corr):
                 stp_corr_df = (pres_ref*t_df)/(temp_ref*p_df)
                 neg_df = (stp_corr_df*neg_df.T).T
                 pos_df = (stp_corr_df*pos_df.T).T
```

