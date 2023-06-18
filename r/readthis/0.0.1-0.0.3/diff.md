# Comparing `tmp/readthis-0.0.1.tar.gz` & `tmp/readthis-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readthis-0.0.1.tar", last modified: Sun Jun 18 12:33:27 2023, max compression
+gzip compressed data, was "readthis-0.0.3.tar", last modified: Sun Jun 18 12:56:02 2023, max compression
```

## Comparing `readthis-0.0.1.tar` & `readthis-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:33:27.656699 readthis-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-18 12:33:12.000000 readthis-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-18 12:33:27.656699 readthis-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-18 12:33:12.000000 readthis-0.0.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1984 2023-06-18 12:33:12.000000 readthis-0.0.1/readthis
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:33:27.656699 readthis-0.0.1/readthis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-18 12:33:27.000000 readthis-0.0.1/readthis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-18 12:33:27.000000 readthis-0.0.1/readthis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 12:33:27.000000 readthis-0.0.1/readthis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-18 12:33:27.000000 readthis-0.0.1/readthis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 12:33:27.000000 readthis-0.0.1/readthis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 12:33:27.656699 readthis-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-18 12:33:12.000000 readthis-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:56:02.274182 readthis-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-18 12:55:47.000000 readthis-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-18 12:56:02.274182 readthis-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-18 12:55:47.000000 readthis-0.0.3/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1984 2023-06-18 12:55:47.000000 readthis-0.0.3/readthis
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:56:02.270182 readthis-0.0.3/readthis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-18 12:56:02.000000 readthis-0.0.3/readthis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-18 12:56:02.000000 readthis-0.0.3/readthis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 12:56:02.000000 readthis-0.0.3/readthis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-18 12:56:02.000000 readthis-0.0.3/readthis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 12:56:02.000000 readthis-0.0.3/readthis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 12:56:02.274182 readthis-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-18 12:55:47.000000 readthis-0.0.3/setup.py
```

### Comparing `readthis-0.0.1/LICENSE` & `readthis-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `readthis-0.0.1/PKG-INFO` & `readthis-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: readthis
-Version: 0.0.1
+Version: 0.0.3
 Summary: readthis - A command line tool to read a text file aloud
 Home-page: https://github.com/entropyqueen/readthis
 Author: Emy Canton
 Author-email: emy.canton@proton.me
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# ReadIt
+# Readthis
 
-ReadIt is a command line tool that reads aloud a given text file using the gTTS (Google Text-to-Speech) interface.
+Readthis is a command line tool that reads aloud a given text file using the gTTS (Google Text-to-Speech) interface.
 
 ## Usage
 
 ```bash
 $ readthis [OPTIONS] FILE
 ```
 
 ### Positional Arguments
 
 - `FILE`: The file to read aloud. Use - to read from stdin.
 
 ### Options
 
 - `-h, --help`: Show the help message and exit.
-- `--lang LANG, -l LANG`: Choose the language to use for reading. Specify the language using the language code (e.g., en for English).
+- `--lang LANG, -l LANG`: Choose the language to use for reading. Specify the language using the language code (e.g., fr for French). Defaults to English.
 
 ## Installation
 
 ```bash
 $ pip install readthis
 ```
 
@@ -45,9 +45,9 @@
 - Read from stdin in French:
 ```bash
 $ echo "Bonjour, comment ça va ?" | readthis -l fr -
 ```
 
 ## License
 
-This project is licensed under the MIT License.
+This project is licensed under the [MIT License](./LICENCE).
```

### Comparing `readthis-0.0.1/README.md` & `readthis-0.0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# ReadIt
+# Readthis
 
-ReadIt is a command line tool that reads aloud a given text file using the gTTS (Google Text-to-Speech) interface.
+Readthis is a command line tool that reads aloud a given text file using the gTTS (Google Text-to-Speech) interface.
 
 ## Usage
 
 ```bash
 $ readthis [OPTIONS] FILE
 ```
 
 ### Positional Arguments
 
 - `FILE`: The file to read aloud. Use - to read from stdin.
 
 ### Options
 
 - `-h, --help`: Show the help message and exit.
-- `--lang LANG, -l LANG`: Choose the language to use for reading. Specify the language using the language code (e.g., en for English).
+- `--lang LANG, -l LANG`: Choose the language to use for reading. Specify the language using the language code (e.g., fr for French). Defaults to English.
 
 ## Installation
 
 ```bash
 $ pip install readthis
 ```
 
@@ -34,9 +34,9 @@
 - Read from stdin in French:
 ```bash
 $ echo "Bonjour, comment ça va ?" | readthis -l fr -
 ```
 
 ## License
 
-This project is licensed under the MIT License.
+This project is licensed under the [MIT License](./LICENCE).
```

### Comparing `readthis-0.0.1/readthis` & `readthis-0.0.3/readthis`

 * *Files identical despite different names*

### Comparing `readthis-0.0.1/readthis.egg-info/PKG-INFO` & `readthis-0.0.3/readthis.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: readthis
-Version: 0.0.1
+Version: 0.0.3
 Summary: readthis - A command line tool to read a text file aloud
 Home-page: https://github.com/entropyqueen/readthis
 Author: Emy Canton
 Author-email: emy.canton@proton.me
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# ReadIt
+# Readthis
 
-ReadIt is a command line tool that reads aloud a given text file using the gTTS (Google Text-to-Speech) interface.
+Readthis is a command line tool that reads aloud a given text file using the gTTS (Google Text-to-Speech) interface.
 
 ## Usage
 
 ```bash
 $ readthis [OPTIONS] FILE
 ```
 
 ### Positional Arguments
 
 - `FILE`: The file to read aloud. Use - to read from stdin.
 
 ### Options
 
 - `-h, --help`: Show the help message and exit.
-- `--lang LANG, -l LANG`: Choose the language to use for reading. Specify the language using the language code (e.g., en for English).
+- `--lang LANG, -l LANG`: Choose the language to use for reading. Specify the language using the language code (e.g., fr for French). Defaults to English.
 
 ## Installation
 
 ```bash
 $ pip install readthis
 ```
 
@@ -45,9 +45,9 @@
 - Read from stdin in French:
 ```bash
 $ echo "Bonjour, comment ça va ?" | readthis -l fr -
 ```
 
 ## License
 
-This project is licensed under the MIT License.
+This project is licensed under the [MIT License](./LICENCE).
```

### Comparing `readthis-0.0.1/setup.py` & `readthis-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='readthis',
-    version='0.0.1',
+    version='0.0.3',
     description='readthis - A command line tool to read a text file aloud',
     author='Emy Canton',
     author_email='emy.canton@proton.me',
     url='https://github.com/entropyqueen/readthis',
     license='MIT',
     scripts=['readthis'],
     setup_requires=[
```

