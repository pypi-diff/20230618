# Comparing `tmp/readthis-0.0.5.tar.gz` & `tmp/readthis-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readthis-0.0.5.tar", last modified: Sun Jun 18 14:17:31 2023, max compression
+gzip compressed data, was "readthis-0.0.6.tar", last modified: Sun Jun 18 14:40:10 2023, max compression
```

## Comparing `readthis-0.0.5.tar` & `readthis-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:17:31.763868 readthis-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-18 14:17:21.000000 readthis-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-18 14:17:31.763868 readthis-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-18 14:17:21.000000 readthis-0.0.5/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     2170 2023-06-18 14:17:21.000000 readthis-0.0.5/readthis
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:17:31.763868 readthis-0.0.5/readthis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-18 14:17:31.000000 readthis-0.0.5/readthis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-18 14:17:31.000000 readthis-0.0.5/readthis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 14:17:31.000000 readthis-0.0.5/readthis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-18 14:17:31.000000 readthis-0.0.5/readthis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-18 14:17:31.000000 readthis-0.0.5/readthis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 14:17:31.763868 readthis-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-18 14:17:21.000000 readthis-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:40:10.722200 readthis-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-18 14:39:59.000000 readthis-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-18 14:40:10.718200 readthis-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-18 14:39:59.000000 readthis-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:40:10.718200 readthis-0.0.6/readthis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 14:39:59.000000 readthis-0.0.6/readthis/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2185 2023-06-18 14:39:59.000000 readthis-0.0.6/readthis/readthis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:40:10.718200 readthis-0.0.6/readthis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-18 14:40:10.000000 readthis-0.0.6/readthis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-18 14:40:10.000000 readthis-0.0.6/readthis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 14:40:10.000000 readthis-0.0.6/readthis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-18 14:40:10.000000 readthis-0.0.6/readthis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-18 14:40:10.000000 readthis-0.0.6/readthis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-18 14:40:10.000000 readthis-0.0.6/readthis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 14:40:10.722200 readthis-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-18 14:39:59.000000 readthis-0.0.6/setup.py
```

### Comparing `readthis-0.0.5/LICENSE` & `readthis-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `readthis-0.0.5/PKG-INFO` & `readthis-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readthis
-Version: 0.0.5
+Version: 0.0.6
 Summary: readthis - A command line tool to read a text file aloud
 Home-page: https://github.com/entropyqueen/readthis
 Author: Emy Canton
 Author-email: emy.canton@proton.me
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `readthis-0.0.5/README.md` & `readthis-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `readthis-0.0.5/readthis` & `readthis-0.0.6/readthis/readthis.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,23 +26,23 @@
     mp3_fp = BytesIO()
     tts.write_to_fp(mp3_fp)
     mp3_fp.seek(0)
     return mp3_fp
 
 def read_text(fragments, lang):
 
-    mp3_fp = get_audio(fragments[0], args.lang)
+    mp3_fp = get_audio(fragments[0], lang)
     if len(fragments) == 1:
         play_audio(mp3_fp)
 
     for i in range(1, min(MAX_GTTS_RQTS, len(fragments))):
 
         with concurrent.futures.ThreadPoolExecutor() as executor:
             executor.submit(play_audio, mp3_fp)
-            mp3_fp = get_audio(fragments[i], args.lang)
+            mp3_fp = get_audio(fragments[i], lang)
 
 def handle_limits(text):
 
     fragments = []
     i = 0
     d = '.'
     
@@ -53,15 +53,15 @@
         if len(fragments[i]) + len(token) < MAX_GTTS_INPUT:
             fragments[i] += d + token
         else:
             i += 1
             fragments.append(token)
     return fragments
 
-if __name__ == '__main__':
+def main():
 
     default_text = os.path.join(DATA_PATH, 'default_text.txt')
 
     parser = argparse.ArgumentParser(description='reads a text using google API')
     parser.add_argument(
         '--lang', '-l', metavar='LANG', default='en',
         help='Choose language to use for reading.'
@@ -78,7 +78,11 @@
         text = sys.stdin.read()
     else:
         with open(args.text) as f:
             text = f.read()
 
     fragments = handle_limits(text)
     read_text(fragments, args.lang)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `readthis-0.0.5/readthis.egg-info/PKG-INFO` & `readthis-0.0.6/readthis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readthis
-Version: 0.0.5
+Version: 0.0.6
 Summary: readthis - A command line tool to read a text file aloud
 Home-page: https://github.com/entropyqueen/readthis
 Author: Emy Canton
 Author-email: emy.canton@proton.me
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `readthis-0.0.5/setup.py` & `readthis-0.0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,28 +3,33 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='readthis',
-    version='0.0.5',
+    version='0.0.6',
     description='readthis - A command line tool to read a text file aloud',
     author='Emy Canton',
     author_email='emy.canton@proton.me',
     url='https://github.com/entropyqueen/readthis',
     license='MIT',
-    scripts=['readthis'],
     setup_requires=[
-        'setuptools',
         'wheel',
     ],
     install_requires=[
         'gTTS==2.3.2',
         'pydub==0.25.1',
     ],
+    packages=['readthis'],
+    package_dir={'readthis': 'readthis'},
     package_data={
-        'readthis': ['data/*.txt'],
+        'readthis': ['readthis/data/*.txt'],
+    },
+    entry_points={
+        'console_scripts': [
+            'readthis = readthis.readthis:__main__',
+        ],
     },
     long_description=long_description,
     long_description_content_type='text/markdown'
 )
```

