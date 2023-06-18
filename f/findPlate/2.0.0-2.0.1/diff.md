# Comparing `tmp/findPlate-2.0.0.tar.gz` & `tmp/findPlate-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findPlate-2.0.0.tar", last modified: Sun Jun 18 14:08:46 2023, max compression
+gzip compressed data, was "findPlate-2.0.1.tar", last modified: Sun Jun 18 14:13:45 2023, max compression
```

## Comparing `findPlate-2.0.0.tar` & `findPlate-2.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 robo      (1000) robo      (1000)        0 2023-06-18 14:08:46.860562 findPlate-2.0.0/
--rw-rw-r--   0 robo      (1000) robo      (1000)      508 2023-06-18 14:08:46.856562 findPlate-2.0.0/PKG-INFO
--rw-rw-r--   0 robo      (1000) robo      (1000)       16 2023-06-18 13:41:47.000000 findPlate-2.0.0/README.md
-drwxrwxr-x   0 robo      (1000) robo      (1000)        0 2023-06-18 14:08:46.856562 findPlate-2.0.0/findPlate/
--rw-rw-r--   0 robo      (1000) robo      (1000)        0 2023-06-18 13:26:11.000000 findPlate-2.0.0/findPlate/__init__.py
--rw-rw-r--   0 robo      (1000) robo      (1000)      827 2023-06-18 14:07:16.000000 findPlate-2.0.0/findPlate/main.py
-drwxrwxr-x   0 robo      (1000) robo      (1000)        0 2023-06-18 14:08:46.856562 findPlate-2.0.0/findPlate.egg-info/
--rw-rw-r--   0 robo      (1000) robo      (1000)      508 2023-06-18 14:08:46.000000 findPlate-2.0.0/findPlate.egg-info/PKG-INFO
--rw-rw-r--   0 robo      (1000) robo      (1000)      222 2023-06-18 14:08:46.000000 findPlate-2.0.0/findPlate.egg-info/SOURCES.txt
--rw-rw-r--   0 robo      (1000) robo      (1000)        1 2023-06-18 14:08:46.000000 findPlate-2.0.0/findPlate.egg-info/dependency_links.txt
--rw-rw-r--   0 robo      (1000) robo      (1000)       30 2023-06-18 14:08:46.000000 findPlate-2.0.0/findPlate.egg-info/requires.txt
--rw-rw-r--   0 robo      (1000) robo      (1000)       10 2023-06-18 14:08:46.000000 findPlate-2.0.0/findPlate.egg-info/top_level.txt
--rw-rw-r--   0 robo      (1000) robo      (1000)       38 2023-06-18 14:08:46.860562 findPlate-2.0.0/setup.cfg
--rw-rw-r--   0 robo      (1000) robo      (1000)      766 2023-06-18 14:08:33.000000 findPlate-2.0.0/setup.py
+drwxrwxr-x   0 robo      (1000) robo      (1000)        0 2023-06-18 14:13:45.490748 findPlate-2.0.1/
+-rw-rw-r--   0 robo      (1000) robo      (1000)      508 2023-06-18 14:13:45.490748 findPlate-2.0.1/PKG-INFO
+-rw-rw-r--   0 robo      (1000) robo      (1000)       16 2023-06-18 13:41:47.000000 findPlate-2.0.1/README.md
+drwxrwxr-x   0 robo      (1000) robo      (1000)        0 2023-06-18 14:13:45.490748 findPlate-2.0.1/findPlate/
+-rw-rw-r--   0 robo      (1000) robo      (1000)        0 2023-06-18 13:26:11.000000 findPlate-2.0.1/findPlate/__init__.py
+-rw-rw-r--   0 robo      (1000) robo      (1000)      829 2023-06-18 14:13:29.000000 findPlate-2.0.1/findPlate/main.py
+drwxrwxr-x   0 robo      (1000) robo      (1000)        0 2023-06-18 14:13:45.490748 findPlate-2.0.1/findPlate.egg-info/
+-rw-rw-r--   0 robo      (1000) robo      (1000)      508 2023-06-18 14:13:45.000000 findPlate-2.0.1/findPlate.egg-info/PKG-INFO
+-rw-rw-r--   0 robo      (1000) robo      (1000)      222 2023-06-18 14:13:45.000000 findPlate-2.0.1/findPlate.egg-info/SOURCES.txt
+-rw-rw-r--   0 robo      (1000) robo      (1000)        1 2023-06-18 14:13:45.000000 findPlate-2.0.1/findPlate.egg-info/dependency_links.txt
+-rw-rw-r--   0 robo      (1000) robo      (1000)       30 2023-06-18 14:13:45.000000 findPlate-2.0.1/findPlate.egg-info/requires.txt
+-rw-rw-r--   0 robo      (1000) robo      (1000)       10 2023-06-18 14:13:45.000000 findPlate-2.0.1/findPlate.egg-info/top_level.txt
+-rw-rw-r--   0 robo      (1000) robo      (1000)       38 2023-06-18 14:13:45.490748 findPlate-2.0.1/setup.cfg
+-rw-rw-r--   0 robo      (1000) robo      (1000)      766 2023-06-18 14:13:41.000000 findPlate-2.0.1/setup.py
```

### Comparing `findPlate-2.0.0/findPlate/main.py` & `findPlate-2.0.1/findPlate/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,10 +18,10 @@
     df = pd.read_excel(path)
     df = df[(df.emri == emri) & (df.mbiemri == mbiemri)]
     if len(df) > 0:
         mgs = f"""
 Personit {df.iloc[0]['emri']} {df.iloc[0]['mbiemri']} me NID {df.iloc[0]['id']} zoteron targen {df.iloc[0]['targa']}
         """
     else:
-        mgs = "Traga nuk ekziston ne listen e targave"
+        mgs = "Personi nuk ekziston ne listen e targave"
     print(mgs)
```

### Comparing `findPlate-2.0.0/setup.py` & `findPlate-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import codecs
 import os
 
 
 # Setting up
 setup(
     name="findPlate",
-    version='2.0.0',
+    version='2.0.1',
     author="Guido Xhindoli",
     author_email="<mail@gmail.com>",
     description='A package finds the car plate',
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
         "pandas==2.0.2",
```

