# Comparing `tmp/readthis-0.0.7.tar.gz` & `tmp/readthis-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readthis-0.0.7.tar", last modified: Sun Jun 18 14:53:09 2023, max compression
+gzip compressed data, was "readthis-0.0.8.tar", last modified: Sun Jun 18 15:11:24 2023, max compression
```

## Comparing `readthis-0.0.7.tar` & `readthis-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:53:09.674030 readthis-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-18 14:52:57.000000 readthis-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-18 14:53:09.674030 readthis-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-18 14:52:57.000000 readthis-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:53:09.674030 readthis-0.0.7/readthis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 14:52:57.000000 readthis-0.0.7/readthis/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2185 2023-06-18 14:52:57.000000 readthis-0.0.7/readthis/readthis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:53:09.674030 readthis-0.0.7/readthis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-18 14:53:09.000000 readthis-0.0.7/readthis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-18 14:53:09.000000 readthis-0.0.7/readthis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 14:53:09.000000 readthis-0.0.7/readthis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-18 14:53:09.000000 readthis-0.0.7/readthis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-18 14:53:09.000000 readthis-0.0.7/readthis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-18 14:53:09.000000 readthis-0.0.7/readthis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 14:53:09.674030 readthis-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-18 14:52:57.000000 readthis-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:11:24.586667 readthis-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-18 15:11:14.000000 readthis-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-18 15:11:24.586667 readthis-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-18 15:11:14.000000 readthis-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:11:24.586667 readthis-0.0.8/readthis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 15:11:14.000000 readthis-0.0.8/readthis/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2185 2023-06-18 15:11:14.000000 readthis-0.0.8/readthis/readthis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:11:24.586667 readthis-0.0.8/readthis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-18 15:11:24.000000 readthis-0.0.8/readthis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-18 15:11:24.000000 readthis-0.0.8/readthis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 15:11:24.000000 readthis-0.0.8/readthis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-18 15:11:24.000000 readthis-0.0.8/readthis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-18 15:11:24.000000 readthis-0.0.8/readthis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-18 15:11:24.000000 readthis-0.0.8/readthis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 15:11:24.586667 readthis-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-18 15:11:14.000000 readthis-0.0.8/setup.py
```

### Comparing `readthis-0.0.7/LICENSE` & `readthis-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `readthis-0.0.7/PKG-INFO` & `readthis-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readthis
-Version: 0.0.7
+Version: 0.0.8
 Summary: readthis - A command line tool to read a text file aloud
 Home-page: https://github.com/entropyqueen/readthis
 Author: Emy Canton
 Author-email: emy.canton@proton.me
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `readthis-0.0.7/README.md` & `readthis-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `readthis-0.0.7/readthis/readthis.py` & `readthis-0.0.8/readthis/readthis.py`

 * *Files identical despite different names*

### Comparing `readthis-0.0.7/readthis.egg-info/PKG-INFO` & `readthis-0.0.8/readthis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readthis
-Version: 0.0.7
+Version: 0.0.8
 Summary: readthis - A command line tool to read a text file aloud
 Home-page: https://github.com/entropyqueen/readthis
 Author: Emy Canton
 Author-email: emy.canton@proton.me
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `readthis-0.0.7/setup.py` & `readthis-0.0.8/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,32 +3,28 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='readthis',
-    version='0.0.7',
+    version='0.0.8',
     description='readthis - A command line tool to read a text file aloud',
     author='Emy Canton',
     author_email='emy.canton@proton.me',
     url='https://github.com/entropyqueen/readthis',
     license='MIT',
     setup_requires=[
         'wheel',
     ],
     install_requires=[
         'gTTS==2.3.2',
         'pydub==0.25.1',
     ],
     packages=['readthis'],
-    package_dir={'readthis': 'readthis'},
-    package_data={
-        'readthis': ['readthis/data/*.txt'],
-    },
     include_package_data=True,
     entry_points={
         'console_scripts': [
             'readthis = readthis.readthis:main',
         ],
     },
     long_description=long_description,
```

