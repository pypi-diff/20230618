# Comparing `tmp/readthis-0.0.8.tar.gz` & `tmp/readthis-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readthis-0.0.8.tar", last modified: Sun Jun 18 15:11:24 2023, max compression
+gzip compressed data, was "readthis-0.0.9.tar", last modified: Sun Jun 18 16:28:47 2023, max compression
```

## Comparing `readthis-0.0.8.tar` & `readthis-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:11:24.586667 readthis-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-18 15:11:14.000000 readthis-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-18 15:11:24.586667 readthis-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-18 15:11:14.000000 readthis-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:11:24.586667 readthis-0.0.8/readthis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 15:11:14.000000 readthis-0.0.8/readthis/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2185 2023-06-18 15:11:14.000000 readthis-0.0.8/readthis/readthis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:11:24.586667 readthis-0.0.8/readthis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-18 15:11:24.000000 readthis-0.0.8/readthis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-18 15:11:24.000000 readthis-0.0.8/readthis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 15:11:24.000000 readthis-0.0.8/readthis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-18 15:11:24.000000 readthis-0.0.8/readthis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-18 15:11:24.000000 readthis-0.0.8/readthis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-18 15:11:24.000000 readthis-0.0.8/readthis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 15:11:24.586667 readthis-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-18 15:11:14.000000 readthis-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:28:47.885828 readthis-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-18 16:28:33.000000 readthis-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-18 16:28:33.000000 readthis-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-18 16:28:47.885828 readthis-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-18 16:28:33.000000 readthis-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:28:47.885828 readthis-0.0.9/readthis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-18 16:28:47.000000 readthis-0.0.9/readthis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-18 16:28:47.000000 readthis-0.0.9/readthis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 16:28:47.000000 readthis-0.0.9/readthis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-18 16:28:47.000000 readthis-0.0.9/readthis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-18 16:28:47.000000 readthis-0.0.9/readthis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-18 16:28:47.000000 readthis-0.0.9/readthis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 16:28:47.885828 readthis-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-18 16:28:33.000000 readthis-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:28:47.881828 readthis-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:28:47.885828 readthis-0.0.9/src/readthis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 16:28:33.000000 readthis-0.0.9/src/readthis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:28:47.885828 readthis-0.0.9/src/readthis/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-18 16:28:33.000000 readthis-0.0.9/src/readthis/data/default_text.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2185 2023-06-18 16:28:33.000000 readthis-0.0.9/src/readthis/readthis.py
```

### Comparing `readthis-0.0.8/LICENSE` & `readthis-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `readthis-0.0.8/PKG-INFO` & `readthis-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readthis
-Version: 0.0.8
+Version: 0.0.9
 Summary: readthis - A command line tool to read a text file aloud
 Home-page: https://github.com/entropyqueen/readthis
 Author: Emy Canton
 Author-email: emy.canton@proton.me
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `readthis-0.0.8/README.md` & `readthis-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `readthis-0.0.8/readthis/readthis.py` & `readthis-0.0.9/src/readthis/readthis.py`

 * *Files identical despite different names*

### Comparing `readthis-0.0.8/readthis.egg-info/PKG-INFO` & `readthis-0.0.9/readthis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readthis
-Version: 0.0.8
+Version: 0.0.9
 Summary: readthis - A command line tool to read a text file aloud
 Home-page: https://github.com/entropyqueen/readthis
 Author: Emy Canton
 Author-email: emy.canton@proton.me
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `readthis-0.0.8/setup.py` & `readthis-0.0.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,35 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='readthis',
-    version='0.0.8',
+    version='0.0.9',
     description='readthis - A command line tool to read a text file aloud',
     author='Emy Canton',
     author_email='emy.canton@proton.me',
     url='https://github.com/entropyqueen/readthis',
     license='MIT',
     setup_requires=[
+        'setuptools',
         'wheel',
     ],
     install_requires=[
         'gTTS==2.3.2',
         'pydub==0.25.1',
     ],
     packages=['readthis'],
+    package_dir={'readthis': 'src/readthis'},
+    package_data={
+        'readthis': ['data/*.txt'],
+    },
     include_package_data=True,
     entry_points={
         'console_scripts': [
             'readthis = readthis.readthis:main',
         ],
     },
     long_description=long_description,
```

