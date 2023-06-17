# Comparing `tmp/gpteasy-1.1.1.tar.gz` & `tmp/gpteasy-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpteasy-1.1.1.tar", last modified: Sat Jun 17 22:20:34 2023, max compression
+gzip compressed data, was "gpteasy-1.1.2.tar", last modified: Sat Jun 17 22:40:07 2023, max compression
```

## Comparing `gpteasy-1.1.1.tar` & `gpteasy-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 22:20:34.810096 gpteasy-1.1.1/
--rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 gpteasy-1.1.1/LICENSE
--rw-r--r--   0 hp         (501) staff       (20)     5188 2023-06-17 22:20:34.809817 gpteasy-1.1.1/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)     3335 2023-06-17 22:20:27.000000 gpteasy-1.1.1/README.md
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 22:20:34.807372 gpteasy-1.1.1/gpteasy/
--rw-r--r--   0 hp         (501) staff       (20)      118 2023-06-16 09:28:57.000000 gpteasy-1.1.1/gpteasy/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     4457 2023-06-17 13:35:36.000000 gpteasy-1.1.1/gpteasy/commands.py
--rw-r--r--   0 hp         (501) staff       (20)      572 2023-06-16 09:08:00.000000 gpteasy-1.1.1/gpteasy/display.py
--rw-r--r--   0 hp         (501) staff       (20)    13176 2023-06-17 22:16:40.000000 gpteasy-1.1.1/gpteasy/gpt.py
--rw-r--r--   0 hp         (501) staff       (20)     1193 2023-06-17 13:35:36.000000 gpteasy-1.1.1/gpteasy/repl.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 22:20:34.809457 gpteasy-1.1.1/gpteasy.egg-info/
--rw-r--r--   0 hp         (501) staff       (20)     5188 2023-06-17 22:20:34.000000 gpteasy-1.1.1/gpteasy.egg-info/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)      276 2023-06-17 22:20:34.000000 gpteasy-1.1.1/gpteasy.egg-info/SOURCES.txt
--rw-r--r--   0 hp         (501) staff       (20)        1 2023-06-17 22:20:34.000000 gpteasy-1.1.1/gpteasy.egg-info/dependency_links.txt
--rw-r--r--   0 hp         (501) staff       (20)      105 2023-06-17 22:20:34.000000 gpteasy-1.1.1/gpteasy.egg-info/requires.txt
--rw-r--r--   0 hp         (501) staff       (20)        8 2023-06-17 22:20:34.000000 gpteasy-1.1.1/gpteasy.egg-info/top_level.txt
--rw-r--r--   0 hp         (501) staff       (20)     1146 2023-06-17 22:20:27.000000 gpteasy-1.1.1/pyproject.toml
--rw-r--r--   0 hp         (501) staff       (20)       38 2023-06-17 22:20:34.810176 gpteasy-1.1.1/setup.cfg
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 22:40:07.855403 gpteasy-1.1.2/
+-rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 gpteasy-1.1.2/LICENSE
+-rw-r--r--   0 hp         (501) staff       (20)     5188 2023-06-17 22:40:07.855023 gpteasy-1.1.2/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)     3335 2023-06-17 22:40:00.000000 gpteasy-1.1.2/README.md
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 22:40:07.851307 gpteasy-1.1.2/gpteasy/
+-rw-r--r--   0 hp         (501) staff       (20)      118 2023-06-16 09:28:57.000000 gpteasy-1.1.2/gpteasy/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     4907 2023-06-17 22:38:27.000000 gpteasy-1.1.2/gpteasy/commands.py
+-rw-r--r--   0 hp         (501) staff       (20)      572 2023-06-16 09:08:00.000000 gpteasy-1.1.2/gpteasy/display.py
+-rw-r--r--   0 hp         (501) staff       (20)    13176 2023-06-17 22:16:40.000000 gpteasy-1.1.2/gpteasy/gpt.py
+-rw-r--r--   0 hp         (501) staff       (20)     1193 2023-06-17 13:35:36.000000 gpteasy-1.1.2/gpteasy/repl.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 22:40:07.854556 gpteasy-1.1.2/gpteasy.egg-info/
+-rw-r--r--   0 hp         (501) staff       (20)     5188 2023-06-17 22:40:07.000000 gpteasy-1.1.2/gpteasy.egg-info/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)      276 2023-06-17 22:40:07.000000 gpteasy-1.1.2/gpteasy.egg-info/SOURCES.txt
+-rw-r--r--   0 hp         (501) staff       (20)        1 2023-06-17 22:40:07.000000 gpteasy-1.1.2/gpteasy.egg-info/dependency_links.txt
+-rw-r--r--   0 hp         (501) staff       (20)      105 2023-06-17 22:40:07.000000 gpteasy-1.1.2/gpteasy.egg-info/requires.txt
+-rw-r--r--   0 hp         (501) staff       (20)        8 2023-06-17 22:40:07.000000 gpteasy-1.1.2/gpteasy.egg-info/top_level.txt
+-rw-r--r--   0 hp         (501) staff       (20)     1146 2023-06-17 22:40:00.000000 gpteasy-1.1.2/pyproject.toml
+-rw-r--r--   0 hp         (501) staff       (20)       38 2023-06-17 22:40:07.855534 gpteasy-1.1.2/setup.cfg
```

### Comparing `gpteasy-1.1.1/LICENSE` & `gpteasy-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpteasy-1.1.1/PKG-INFO` & `gpteasy-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpteasy
-Version: 1.1.1
+Version: 1.1.2
 Summary: Makes working with OpenAi's GPT API super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -38,15 +38,15 @@
 License-File: LICENSE
 
 # GPT Easy
 
 Package to make working with the OpenAI GPT API in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 1.1.1
+Current version: 1.1.2
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install gpteasy
 ~~~~
 2. Create an OpenAI acccount [here](https://platform.openai.com/))
```

### Comparing `gpteasy-1.1.1/README.md` & `gpteasy-1.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # GPT Easy
 
 Package to make working with the OpenAI GPT API in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 1.1.1
+Current version: 1.1.2
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install gpteasy
 ~~~~
 2. Create an OpenAI acccount [here](https://platform.openai.com/))
```

### Comparing `gpteasy-1.1.1/gpteasy/commands.py` & `gpteasy-1.1.2/gpteasy/commands.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     def __init__(self, gpt: GPT):
         self.gpt = gpt
 
         self.commands = {}
         self.add_command('quit', self.handle_quit, ":quit - Quit the program")
         self.add_command('load', self.handle_load, ":load name - loads the saved conversation with the specified name")
         self.add_command('save', self.handle_save, ":save name - saves the conversation under the specified name")
-
+        self.add_command('debug', self.handle_debug, ":debug - set to True displays all prompts and model replies")
         self.add_command('input', self.handle_input, ":input filename - loads an input from the specified file")
         self.add_command('model', self.handle_gpt_attribute, ":model gpt-4 - Sets the AI model")
         self.add_command('max_tokens', self.handle_gpt_attribute,
                          ":max_tokens 800 - The maximum number of tokens to generate in the completion")
         self.add_command('temperature', self.handle_gpt_attribute, ":temperature 0.9 - What sampling temperature to " +
                                                                    "use, between 0 and 2")
         self.add_command('n', self.handle_gpt_attribute, ":n 1 - Specifies the number answers given")
@@ -55,14 +55,22 @@
         return True
 
     def handle_reset(self):
         self.gpt.reset()
         color_print(f"Conversation reset\n", color=SYSTEM_COLOR)
         return True
 
+    def handle_debug(self, debug: str=None):
+        if debug is None:
+            color_print(f'debug is {self.gpt.debug}', color=SYSTEM_COLOR)
+        else:
+            self.gpt.debug = debug.lower() in ['true', '1', 't', 'y', 'yes']
+            color_print(f'debug set to {self.gpt.debug}', color=SYSTEM_COLOR)
+        return True
+
     def handle_bye(self):
         self.gpt.save()
         self.gpt.chat('bye')
         return False
 
     def handle_maxmessages(self, param):
         self.gpt.message_memory = int(param)
```

### Comparing `gpteasy-1.1.1/gpteasy/display.py` & `gpteasy-1.1.2/gpteasy/display.py`

 * *Files identical despite different names*

### Comparing `gpteasy-1.1.1/gpteasy/gpt.py` & `gpteasy-1.1.2/gpteasy/gpt.py`

 * *Files identical despite different names*

### Comparing `gpteasy-1.1.1/gpteasy/repl.py` & `gpteasy-1.1.2/gpteasy/repl.py`

 * *Files identical despite different names*

### Comparing `gpteasy-1.1.1/gpteasy.egg-info/PKG-INFO` & `gpteasy-1.1.2/gpteasy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpteasy
-Version: 1.1.1
+Version: 1.1.2
 Summary: Makes working with OpenAi's GPT API super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -38,15 +38,15 @@
 License-File: LICENSE
 
 # GPT Easy
 
 Package to make working with the OpenAI GPT API in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 1.1.1
+Current version: 1.1.2
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install gpteasy
 ~~~~
 2. Create an OpenAI acccount [here](https://platform.openai.com/))
```

### Comparing `gpteasy-1.1.1/pyproject.toml` & `gpteasy-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gpteasy"
-version = "1.1.1"
+version = "1.1.2"
 description = "Makes working with OpenAi's GPT API super easy"
 readme = "README.md"
 authors = [{ name = "HP Harmsen", email = "hp@harmsen.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

