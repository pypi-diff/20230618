# Comparing `tmp/readthis-0.0.3.tar.gz` & `tmp/readthis-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readthis-0.0.3.tar", last modified: Sun Jun 18 12:56:02 2023, max compression
+gzip compressed data, was "readthis-0.0.4.tar", last modified: Sun Jun 18 14:09:50 2023, max compression
```

## Comparing `readthis-0.0.3.tar` & `readthis-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:56:02.274182 readthis-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-18 12:55:47.000000 readthis-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-18 12:56:02.274182 readthis-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-18 12:55:47.000000 readthis-0.0.3/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1984 2023-06-18 12:55:47.000000 readthis-0.0.3/readthis
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:56:02.270182 readthis-0.0.3/readthis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-18 12:56:02.000000 readthis-0.0.3/readthis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-18 12:56:02.000000 readthis-0.0.3/readthis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 12:56:02.000000 readthis-0.0.3/readthis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-18 12:56:02.000000 readthis-0.0.3/readthis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 12:56:02.000000 readthis-0.0.3/readthis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 12:56:02.274182 readthis-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-18 12:55:47.000000 readthis-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:09:50.609198 readthis-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-18 14:09:33.000000 readthis-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-18 14:09:50.609198 readthis-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-18 14:09:33.000000 readthis-0.0.4/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2125 2023-06-18 14:09:33.000000 readthis-0.0.4/readthis
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:09:50.609198 readthis-0.0.4/readthis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-18 14:09:50.000000 readthis-0.0.4/readthis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-18 14:09:50.000000 readthis-0.0.4/readthis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 14:09:50.000000 readthis-0.0.4/readthis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-18 14:09:50.000000 readthis-0.0.4/readthis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-18 14:09:50.000000 readthis-0.0.4/readthis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 14:09:50.609198 readthis-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-18 14:09:33.000000 readthis-0.0.4/setup.py
```

### Comparing `readthis-0.0.3/LICENSE` & `readthis-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `readthis-0.0.3/PKG-INFO` & `readthis-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readthis
-Version: 0.0.3
+Version: 0.0.4
 Summary: readthis - A command line tool to read a text file aloud
 Home-page: https://github.com/entropyqueen/readthis
 Author: Emy Canton
 Author-email: emy.canton@proton.me
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `readthis-0.0.3/README.md` & `readthis-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `readthis-0.0.3/readthis` & `readthis-0.0.4/readthis`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 from gtts import gTTS
 from io import BytesIO
 from pydub import AudioSegment
 from pydub.playback import play as pydub_play
 import argparse
-import sys
+import sys, os
 
 import concurrent.futures
 
 
 MAX_GTTS_INPUT = 300 # Max bytes (found 5000 online)
 MAX_GTTS_RQTS = 1000 # Max requests *per minutes* (found 1000 online)
 
@@ -53,29 +53,30 @@
         else:
             i += 1
             fragments.append(token)
     return fragments
 
 if __name__ == '__main__':
 
+    default_text = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'data', 'default_text.txt')
+
     parser = argparse.ArgumentParser(description='reads a text using google API')
     parser.add_argument(
         '--lang', '-l', metavar='LANG', default='en',
         help='Choose language to use for reading.'
     )
     parser.add_argument(
-        'text', metavar='FILE',
+        'text', metavar='FILE', nargs='?', default=default_text,
         help='File to read, or - for stdin'
     )
     args = parser.parse_args()
 
     text = ''
     # Get input from file or stdin
     if args.text == '-':
         text = sys.stdin.read()
     else:
         with open(args.text) as f:
             text = f.read()
 
     fragments = handle_limits(text)
     read_text(fragments, args.lang)
-
```

### Comparing `readthis-0.0.3/readthis.egg-info/PKG-INFO` & `readthis-0.0.4/readthis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readthis
-Version: 0.0.3
+Version: 0.0.4
 Summary: readthis - A command line tool to read a text file aloud
 Home-page: https://github.com/entropyqueen/readthis
 Author: Emy Canton
 Author-email: emy.canton@proton.me
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `readthis-0.0.3/setup.py` & `readthis-0.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,25 +3,28 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='readthis',
-    version='0.0.3',
+    version='0.0.4',
     description='readthis - A command line tool to read a text file aloud',
     author='Emy Canton',
     author_email='emy.canton@proton.me',
     url='https://github.com/entropyqueen/readthis',
     license='MIT',
     scripts=['readthis'],
     setup_requires=[
         'setuptools',
         'wheel',
     ],
     install_requires=[
         'gTTS==2.3.2',
         'pydub==0.25.1',
     ],
+    package_data={
+        'readthis': ['data/*.txt'],
+    },
     long_description=long_description,
     long_description_content_type='text/markdown'
 )
```

