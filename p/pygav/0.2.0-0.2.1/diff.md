# Comparing `tmp/pygav-0.2.0.tar.gz` & `tmp/pygav-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygav-0.2.0.tar", last modified: Thu Jun  8 12:26:51 2023, max compression
+gzip compressed data, was "pygav-0.2.1.tar", last modified: Sun Jun 18 16:32:15 2023, max compression
```

## Comparing `pygav-0.2.0.tar` & `pygav-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-08 12:26:51.772113 pygav-0.2.0/
--rw-rw-r--   0 ngav      (1000) ngav      (1000)      483 2022-06-04 21:24:31.000000 pygav-0.2.0/LICENSE
--rw-rw-r--   0 ngav      (1000) ngav      (1000)     1415 2023-06-08 12:26:51.772113 pygav-0.2.0/PKG-INFO
--rw-rw-r--   0 ngav      (1000) ngav      (1000)      447 2023-06-08 12:23:02.000000 pygav-0.2.0/README.md
-drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-08 12:26:51.772113 pygav-0.2.0/pygav/
--rw-rw-r--   0 ngav      (1000) ngav      (1000)        0 2022-06-04 19:41:44.000000 pygav-0.2.0/pygav/__init__.py
--rw-rw-r--   0 ngav      (1000) ngav      (1000)     4679 2023-06-08 12:21:25.000000 pygav-0.2.0/pygav/data.py
--rw-rw-r--   0 ngav      (1000) ngav      (1000)      715 2023-06-07 10:49:39.000000 pygav-0.2.0/pygav/utils.py
-drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-08 12:26:51.772113 pygav-0.2.0/pygav.egg-info/
--rw-rw-r--   0 ngav      (1000) ngav      (1000)     1415 2023-06-08 12:26:51.000000 pygav-0.2.0/pygav.egg-info/PKG-INFO
--rw-rw-r--   0 ngav      (1000) ngav      (1000)      243 2023-06-08 12:26:51.000000 pygav-0.2.0/pygav.egg-info/SOURCES.txt
--rw-rw-r--   0 ngav      (1000) ngav      (1000)        1 2023-06-08 12:26:51.000000 pygav-0.2.0/pygav.egg-info/dependency_links.txt
--rw-rw-r--   0 ngav      (1000) ngav      (1000)       82 2023-06-08 12:26:51.000000 pygav-0.2.0/pygav.egg-info/requires.txt
--rw-rw-r--   0 ngav      (1000) ngav      (1000)        6 2023-06-08 12:26:51.000000 pygav-0.2.0/pygav.egg-info/top_level.txt
--rw-rw-r--   0 ngav      (1000) ngav      (1000)      753 2023-06-08 11:48:59.000000 pygav-0.2.0/pyproject.toml
--rw-rw-r--   0 ngav      (1000) ngav      (1000)       38 2023-06-08 12:26:51.772113 pygav-0.2.0/setup.cfg
-drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-08 12:26:51.772113 pygav-0.2.0/tests/
--rw-rw-r--   0 ngav      (1000) ngav      (1000)      258 2023-06-07 10:51:03.000000 pygav-0.2.0/tests/test_utils.py
+drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-18 16:32:15.815651 pygav-0.2.1/
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)      483 2022-06-04 21:24:31.000000 pygav-0.2.1/LICENSE
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)     1415 2023-06-18 16:32:15.811651 pygav-0.2.1/PKG-INFO
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)      447 2023-06-08 12:23:02.000000 pygav-0.2.1/README.md
+drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-18 16:32:15.811651 pygav-0.2.1/pygav/
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)        0 2022-06-04 19:41:44.000000 pygav-0.2.1/pygav/__init__.py
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)     4681 2023-06-18 16:30:30.000000 pygav-0.2.1/pygav/data.py
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)      715 2023-06-07 10:49:39.000000 pygav-0.2.1/pygav/utils.py
+drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-18 16:32:15.811651 pygav-0.2.1/pygav.egg-info/
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)     1415 2023-06-18 16:32:15.000000 pygav-0.2.1/pygav.egg-info/PKG-INFO
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)      243 2023-06-18 16:32:15.000000 pygav-0.2.1/pygav.egg-info/SOURCES.txt
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)        1 2023-06-18 16:32:15.000000 pygav-0.2.1/pygav.egg-info/dependency_links.txt
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)       82 2023-06-18 16:32:15.000000 pygav-0.2.1/pygav.egg-info/requires.txt
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)        6 2023-06-18 16:32:15.000000 pygav-0.2.1/pygav.egg-info/top_level.txt
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)      753 2023-06-18 16:31:30.000000 pygav-0.2.1/pyproject.toml
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)       38 2023-06-18 16:32:15.815651 pygav-0.2.1/setup.cfg
+drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-18 16:32:15.811651 pygav-0.2.1/tests/
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)      258 2023-06-07 10:51:03.000000 pygav-0.2.1/tests/test_utils.py
```

### Comparing `pygav-0.2.0/PKG-INFO` & `pygav-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygav
-Version: 0.2.0
+Version: 0.2.1
 Summary: Useful stuff
 Author: Nikos Gavalas
 License:             DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
                             Version 2, December 2004
         
          Copyright (C) 2004 Sam Hocevar <sam@hocevar.net>
```

### Comparing `pygav-0.2.0/pygav/data.py` & `pygav-0.2.1/pygav/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,17 +138,17 @@
 
     plot = sns.relplot(data=data, x=x, y=y, col=col, hue=hue, style=style, kind=kind, ax=ax)
 
     if title:
         plot.fig.subplots_adjust(top=0.9)
         plot.fig.suptitle(title)
     if xlabel:
-        plot.set_xlabel(xlabel)
+        plot.set_xlabels(xlabel)
     if ylabel:
-        plot.set_ylabel(ylabel)
+        plot.set_ylabels(ylabel)
 
     if xlim is not None:
         plot.set(xlim=xlim)
     if ylim is not None:
         plot.set(ylim=ylim)
 
     if logx:
```

### Comparing `pygav-0.2.0/pygav/utils.py` & `pygav-0.2.1/pygav/utils.py`

 * *Files identical despite different names*

### Comparing `pygav-0.2.0/pygav.egg-info/PKG-INFO` & `pygav-0.2.1/pygav.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygav
-Version: 0.2.0
+Version: 0.2.1
 Summary: Useful stuff
 Author: Nikos Gavalas
 License:             DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
                             Version 2, December 2004
         
          Copyright (C) 2004 Sam Hocevar <sam@hocevar.net>
```

### Comparing `pygav-0.2.0/pyproject.toml` & `pygav-0.2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygav"
-version = "0.2.0"
+version = "0.2.1"
 description = "Useful stuff"
 readme = "README.md"
 authors = [{ name = "Nikos Gavalas" }]
 license = { file = "LICENSE" }
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
```

