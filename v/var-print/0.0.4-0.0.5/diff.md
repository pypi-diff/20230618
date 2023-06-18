# Comparing `tmp/var_print-0.0.4.tar.gz` & `tmp/var_print-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "var_print-0.0.4.tar", last modified: Sun May 14 20:12:49 2023, max compression
+gzip compressed data, was "var_print-0.0.5.tar", last modified: Sun Jun 18 17:44:48 2023, max compression
```

## Comparing `var_print-0.0.4.tar` & `var_print-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 20:12:49.165924 var_print-0.0.4/
--rw-rw-rw-   0        0        0     1095 2023-01-07 18:45:09.000000 var_print-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      159 2023-01-07 18:55:43.000000 var_print-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     5750 2023-05-14 20:12:49.165924 var_print-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4986 2023-01-07 18:59:14.000000 var_print-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-14 20:12:49.165924 var_print-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1803 2023-05-14 20:10:20.000000 var_print-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-14 20:12:49.155036 var_print-0.0.4/var_print/
--rw-rw-rw-   0        0        0       63 2023-05-14 20:10:36.000000 var_print-0.0.4/var_print/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 20:12:49.163893 var_print-0.0.4/var_print/data/
--rw-rw-rw-   0        0        0     6221 2023-01-07 18:45:09.000000 var_print-0.0.4/var_print/data/color_schemes.pickle
--rw-rw-rw-   0        0        0    36197 2023-02-14 16:19:16.000000 var_print-0.0.4/var_print/varPrint.py
-drwxrwxrwx   0        0        0        0 2023-05-14 20:12:49.162333 var_print-0.0.4/var_print.egg-info/
--rw-rw-rw-   0        0        0     5750 2023-05-14 20:12:48.000000 var_print-0.0.4/var_print.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-05-14 20:12:49.000000 var_print-0.0.4/var_print.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 20:12:48.000000 var_print-0.0.4/var_print.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-14 20:12:49.000000 var_print-0.0.4/var_print.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-14 20:12:49.000000 var_print-0.0.4/var_print.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 17:44:47.999219 var_print-0.0.5/
+-rw-rw-rw-   0        0        0     1095 2023-01-07 18:45:09.000000 var_print-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      159 2023-01-07 18:55:43.000000 var_print-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     5750 2023-06-18 17:44:47.997969 var_print-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4986 2023-01-07 18:59:14.000000 var_print-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-18 17:44:47.999219 var_print-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1803 2023-06-18 17:43:36.000000 var_print-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:44:47.986747 var_print-0.0.5/var_print/
+-rw-rw-rw-   0        0        0       63 2023-06-18 17:43:37.000000 var_print-0.0.5/var_print/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:44:47.995683 var_print-0.0.5/var_print/data/
+-rw-rw-rw-   0        0        0     6221 2023-01-07 18:45:09.000000 var_print-0.0.5/var_print/data/color_schemes.pickle
+-rw-rw-rw-   0        0        0    35982 2023-06-18 17:42:21.000000 var_print-0.0.5/var_print/varPrint.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:44:47.993496 var_print-0.0.5/var_print.egg-info/
+-rw-rw-rw-   0        0        0     5750 2023-06-18 17:44:47.000000 var_print-0.0.5/var_print.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-06-18 17:44:47.000000 var_print-0.0.5/var_print.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 17:44:47.000000 var_print-0.0.5/var_print.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-18 17:44:47.000000 var_print-0.0.5/var_print.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-18 17:44:47.000000 var_print-0.0.5/var_print.egg-info/top_level.txt
```

### Comparing `var_print-0.0.4/LICENSE` & `var_print-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `var_print-0.0.4/PKG-INFO` & `var_print-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: var_print
-Version: 0.0.4
+Version: 0.0.5
 Summary: Nicer printing with var_print: Colours and structure allow quick reading of the output, at the same time the name of the variable is displayed. 
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `var_print-0.0.4/README.md` & `var_print-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `var_print-0.0.4/setup.py` & `var_print-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.4"
+VERSION = "0.0.5"
 DESCRIPTION = "Nicer printing with var_print: Colours and structure allow quick reading of the output, at the same time the name of the variable is displayed. "
 
 # Setting up
 setup(
     name="var_print",
     version=VERSION,
     author="André Herber",
```

### Comparing `var_print-0.0.4/var_print/data/color_schemes.pickle` & `var_print-0.0.5/var_print/data/color_schemes.pickle`

 * *Files identical despite different names*

### Comparing `var_print-0.0.4/var_print/varPrint.py` & `var_print-0.0.5/var_print/varPrint.py`

 * *Files 2% similar despite different names*

```diff
@@ -514,46 +514,45 @@
                         max_vl,
                         i,
                         len(liste),
                         True,
                     )  # left
                     for (i, v) in enumerate(liste)
                 ]
-                jvs = {jvs[i]: type(v) for (i, v) in enumerate(liste)}
+                jvs = [(jvs[i], type(v)) for (i, v) in enumerate(liste)]
             if self.list_alignment == "right":
                 jvs = [
                     iter_colored_adjustment(
                         self.format_value(v, kide, recursion_level)
                         + iter_comma_if_needed(i, len(liste)),
                         self.format_value(v, kide, recursion_level),
                         max_vl,
                         i,
                         len(liste),
                         False,
                     )  # right
                     for (i, v) in enumerate(liste)
                 ]
-                jvs = {jvs[i]: type(v) for (i, v) in enumerate(liste)}
+                jvs = [(jvs[i], type(v)) for (i, v) in enumerate(liste)]
             else:
                 jvs = [
                     self.format_value(v, kide, recursion_level)
                     + iter_comma_if_needed(i, len(liste))
                     for (i, v) in enumerate(liste)
                 ]
-                jvs = {jvs[i]: type(v) for (i, v) in enumerate(liste)}
+                jvs = [(jvs[i], type(v)) for (i, v) in enumerate(liste)]
 
-            # lstr = self.c_rgb + pref + k_auf + f"".join([f"{self.a_rgb}{v}{iters_new_line_if_needed(i, len(jvs), ide, iipl, k_auf, v_type)}" for (i, (v, v_type)) in enumerate(jvs.items())]) + self.c_rgb + k_zu
             lstr = (
                 self.c_rgb
                 + pref
                 + k_auf
                 + iter_join(
                     [
                         f"{self.a_rgb}{v}{iters_new_line_if_needed(i, len(jvs), ide, iipl, k_auf, v_type)}"
-                        for (i, (v, v_type)) in enumerate(jvs.items())
+                        for (i, (v, v_type)) in enumerate(jvs)
                     ]
                 )
                 + self.c_rgb
                 + k_zu
             )
 
             return lstr
```

### Comparing `var_print-0.0.4/var_print.egg-info/PKG-INFO` & `var_print-0.0.5/var_print.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: var-print
-Version: 0.0.4
+Version: 0.0.5
 Summary: Nicer printing with var_print: Colours and structure allow quick reading of the output, at the same time the name of the variable is displayed. 
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

