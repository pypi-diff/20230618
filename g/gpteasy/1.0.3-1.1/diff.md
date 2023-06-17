# Comparing `tmp/gpteasy-1.0.3.tar.gz` & `tmp/gpteasy-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpteasy-1.0.3.tar", last modified: Sat Jun 17 14:20:41 2023, max compression
+gzip compressed data, was "gpteasy-1.1.tar", last modified: Sat Jun 17 22:17:59 2023, max compression
```

## Comparing `gpteasy-1.0.3.tar` & `gpteasy-1.1.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 14:20:41.608223 gpteasy-1.0.3/
--rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 gpteasy-1.0.3/LICENSE
--rw-r--r--   0 hp         (501) staff       (20)     5188 2023-06-17 14:20:41.607758 gpteasy-1.0.3/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)     3335 2023-06-17 14:20:31.000000 gpteasy-1.0.3/README.md
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 14:20:41.603302 gpteasy-1.0.3/gpteasy/
--rw-r--r--   0 hp         (501) staff       (20)      118 2023-06-16 09:28:57.000000 gpteasy-1.0.3/gpteasy/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     4457 2023-06-17 13:35:36.000000 gpteasy-1.0.3/gpteasy/commands.py
--rw-r--r--   0 hp         (501) staff       (20)      572 2023-06-16 09:08:00.000000 gpteasy-1.0.3/gpteasy/display.py
--rw-r--r--   0 hp         (501) staff       (20)    12803 2023-06-17 14:19:37.000000 gpteasy-1.0.3/gpteasy/gpt.py
--rw-r--r--   0 hp         (501) staff       (20)     1193 2023-06-17 13:35:36.000000 gpteasy-1.0.3/gpteasy/repl.py
--rw-r--r--   0 hp         (501) staff       (20)     3757 2023-06-16 09:08:00.000000 gpteasy-1.0.3/gpteasy/settings.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 14:20:41.607021 gpteasy-1.0.3/gpteasy.egg-info/
--rw-r--r--   0 hp         (501) staff       (20)     5188 2023-06-17 14:20:41.000000 gpteasy-1.0.3/gpteasy.egg-info/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)      296 2023-06-17 14:20:41.000000 gpteasy-1.0.3/gpteasy.egg-info/SOURCES.txt
--rw-r--r--   0 hp         (501) staff       (20)        1 2023-06-17 14:20:41.000000 gpteasy-1.0.3/gpteasy.egg-info/dependency_links.txt
--rw-r--r--   0 hp         (501) staff       (20)      105 2023-06-17 14:20:41.000000 gpteasy-1.0.3/gpteasy.egg-info/requires.txt
--rw-r--r--   0 hp         (501) staff       (20)        8 2023-06-17 14:20:41.000000 gpteasy-1.0.3/gpteasy.egg-info/top_level.txt
--rw-r--r--   0 hp         (501) staff       (20)     1146 2023-06-17 14:20:31.000000 gpteasy-1.0.3/pyproject.toml
--rw-r--r--   0 hp         (501) staff       (20)       38 2023-06-17 14:20:41.608388 gpteasy-1.0.3/setup.cfg
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 22:17:59.816780 gpteasy-1.1/
+-rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 gpteasy-1.1/LICENSE
+-rw-r--r--   0 hp         (501) staff       (20)     5186 2023-06-17 22:17:59.816355 gpteasy-1.1/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)     3335 2023-06-17 14:20:31.000000 gpteasy-1.1/README.md
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 22:17:59.813550 gpteasy-1.1/gpteasy/
+-rw-r--r--   0 hp         (501) staff       (20)      118 2023-06-16 09:28:57.000000 gpteasy-1.1/gpteasy/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     4457 2023-06-17 13:35:36.000000 gpteasy-1.1/gpteasy/commands.py
+-rw-r--r--   0 hp         (501) staff       (20)      572 2023-06-16 09:08:00.000000 gpteasy-1.1/gpteasy/display.py
+-rw-r--r--   0 hp         (501) staff       (20)    13176 2023-06-17 22:16:40.000000 gpteasy-1.1/gpteasy/gpt.py
+-rw-r--r--   0 hp         (501) staff       (20)     1193 2023-06-17 13:35:36.000000 gpteasy-1.1/gpteasy/repl.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 22:17:59.815839 gpteasy-1.1/gpteasy.egg-info/
+-rw-r--r--   0 hp         (501) staff       (20)     5186 2023-06-17 22:17:59.000000 gpteasy-1.1/gpteasy.egg-info/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)      276 2023-06-17 22:17:59.000000 gpteasy-1.1/gpteasy.egg-info/SOURCES.txt
+-rw-r--r--   0 hp         (501) staff       (20)        1 2023-06-17 22:17:59.000000 gpteasy-1.1/gpteasy.egg-info/dependency_links.txt
+-rw-r--r--   0 hp         (501) staff       (20)      105 2023-06-17 22:17:59.000000 gpteasy-1.1/gpteasy.egg-info/requires.txt
+-rw-r--r--   0 hp         (501) staff       (20)        8 2023-06-17 22:17:59.000000 gpteasy-1.1/gpteasy.egg-info/top_level.txt
+-rw-r--r--   0 hp         (501) staff       (20)     1144 2023-06-17 22:17:06.000000 gpteasy-1.1/pyproject.toml
+-rw-r--r--   0 hp         (501) staff       (20)       38 2023-06-17 22:17:59.816904 gpteasy-1.1/setup.cfg
```

### Comparing `gpteasy-1.0.3/LICENSE` & `gpteasy-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpteasy-1.0.3/PKG-INFO` & `gpteasy-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpteasy
-Version: 1.0.3
+Version: 1.1
 Summary: Makes working with OpenAi's GPT API super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `gpteasy-1.0.3/README.md` & `gpteasy-1.1/README.md`

 * *Files identical despite different names*

### Comparing `gpteasy-1.0.3/gpteasy/commands.py` & `gpteasy-1.1/gpteasy/commands.py`

 * *Files identical despite different names*

### Comparing `gpteasy-1.0.3/gpteasy/display.py` & `gpteasy-1.1/gpteasy/display.py`

 * *Files identical despite different names*

### Comparing `gpteasy-1.0.3/gpteasy/gpt.py` & `gpteasy-1.1/gpteasy/gpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 from pathlib import Path
 
 import openai
 from tenacity import retry, wait_random_exponential, stop_after_attempt
 from dotenv import load_dotenv
 from openai.error import APIConnectionError, APIError, RateLimitError
 
-from gpteasy.display import print_message, color_print, SYSTEM_COLOR, ERROR_COLOR
-from gpteasy.settings import get_settings
+from gpteasy.display import print_message, color_print, SYSTEM_COLOR, ERROR_COLOR, DEBUG_COLOR2, DEBUG_COLOR1
 
 BASE_SYSTEM = "You are ChatGPT, a large language model trained by OpenAI."
 
 
 class GptFunction:
     def __init__(self, name: str, description: str, callback=None):
         self.function_name = name
@@ -130,14 +129,16 @@
         self.name = ''  # Name of the current conversation
         self.save_dir = Path(__file__).resolve().parent / 'saves'
         self.save_dir.mkdir(exist_ok=True)
 
         self.message_memory = 20  # Number of messages to remember. Limits token usage.
         self.messages = []
 
+        self.debug = False
+
     def system(self):  # This function can be overwritten by child classes to make the system message dynamic
         return self.system_message
 
     def reset(self):
         self.name = ''
         self.messages = []
 
@@ -161,14 +162,18 @@
     def get_functions(self):
         return [f.in_completion_format() for f in self.functions.values()] if self.functions else None
 
     def chat(self, prompt, add_to_messages=True):
 
         @retry(wait=wait_random_exponential(min=1, max=40), stop=stop_after_attempt(3))
         def chat_completion_request():
+            if self.debug:
+                for message in self.messages:
+                    if hasattr(message, 'text'):
+                        color_print(f"{message.role}: {message.text}", color=DEBUG_COLOR1)
             try:
                 if self.functions:
                     completion = openai.ChatCompletion.create(
                         model=self.model,
                         messages=self.get_messages(),
                         temperature=self.temperature,
                         max_tokens=self.max_tokens,
@@ -188,23 +193,25 @@
                         max_tokens=self.max_tokens,
                         n=self.n,
                         top_p=self.top_p,
                         frequency_penalty=self.frequency_penalty,
                         presence_penalty=self.presence_penalty,
                         stop=self.stop
                     )
+                if self.debug and hasattr(completion.choices[0], 'text'):
+                    color_print(f"{completion.choices[0].text}", color=DEBUG_COLOR2)
                 return completion
             except APIConnectionError as e:
                 color_print("Connection error.", color=SYSTEM_COLOR)
                 return e
             except APIError as e:
                 color_print("API error", color=SYSTEM_COLOR)
                 return e
             except RateLimitError as e:
-                color_print(f"{get_settings()['model']} is overloaded", color=SYSTEM_COLOR)
+                color_print(f"{self.model} is overloaded", color=SYSTEM_COLOR)
                 return e
 
         if self.messages and not self.name:
             self.name = re.sub(r'\W+', '', self.messages[0].text).replace(' ', '_')[:20]
         self.messages += [Message('user', prompt)]
 
         completion = chat_completion_request()
```

### Comparing `gpteasy-1.0.3/gpteasy/repl.py` & `gpteasy-1.1/gpteasy/repl.py`

 * *Files identical despite different names*

### Comparing `gpteasy-1.0.3/gpteasy.egg-info/PKG-INFO` & `gpteasy-1.1/gpteasy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpteasy
-Version: 1.0.3
+Version: 1.1
 Summary: Makes working with OpenAi's GPT API super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `gpteasy-1.0.3/pyproject.toml` & `gpteasy-1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gpteasy"
-version = "1.0.3"
+version = "1.1"
 description = "Makes working with OpenAi's GPT API super easy"
 readme = "README.md"
 authors = [{ name = "HP Harmsen", email = "hp@harmsen.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

