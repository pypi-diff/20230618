# Comparing `tmp/charactergpt-prompts-0.0.15.tar.gz` & `tmp/charactergpt-prompts-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charactergpt-prompts-0.0.15.tar", last modified: Sat Jun 17 22:31:37 2023, max compression
+gzip compressed data, was "charactergpt-prompts-0.1.0.tar", last modified: Sat Jun 17 23:46:03 2023, max compression
```

## Comparing `charactergpt-prompts-0.0.15.tar` & `charactergpt-prompts-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 22:31:37.532662 charactergpt-prompts-0.0.15/
--rw-rw-rw-   0        0        0     1069 2023-06-17 21:13:55.000000 charactergpt-prompts-0.0.15/LICENSE
--rw-rw-rw-   0        0        0      604 2023-06-17 22:31:37.532662 charactergpt-prompts-0.0.15/PKG-INFO
--rw-rw-rw-   0        0        0      113 2023-06-17 21:03:43.000000 charactergpt-prompts-0.0.15/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 22:31:37.519552 charactergpt-prompts-0.0.15/charactergpt_prompts/
--rw-rw-rw-   0        0        0        0 2023-06-17 22:10:30.000000 charactergpt-prompts-0.0.15/charactergpt_prompts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 22:31:37.529662 charactergpt-prompts-0.0.15/charactergpt_prompts/additional_data/
--rw-rw-rw-   0        0        0      262 2023-06-16 21:09:43.000000 charactergpt-prompts-0.0.15/charactergpt_prompts/additional_data/character_gpt_errors.py
--rw-rw-rw-   0        0        0      433 2023-06-17 19:36:19.000000 charactergpt-prompts-0.0.15/charactergpt_prompts/additional_data/debug_mode_prompt
--rw-rw-rw-   0        0        0      237 2023-06-16 22:01:44.000000 charactergpt-prompts-0.0.15/charactergpt_prompts/additional_data/prompt_finish
-drwxrwxrwx   0        0        0        0 2023-06-17 22:31:37.529662 charactergpt-prompts-0.0.15/charactergpt_prompts/jailbreaks/
--rw-rw-rw-   0        0        0      912 2023-06-16 22:26:14.000000 charactergpt-prompts-0.0.15/charactergpt_prompts/jailbreaks/default.txt
--rw-rw-rw-   0        0        0     7755 2023-06-17 22:31:17.000000 charactergpt-prompts-0.0.15/charactergpt_prompts/prompt_generator.py
-drwxrwxrwx   0        0        0        0 2023-06-17 22:31:37.531662 charactergpt-prompts-0.0.15/charactergpt_prompts/ready_to_use_prompts/
--rw-rw-rw-   0        0        0     2675 2023-06-17 19:36:53.000000 charactergpt-prompts-0.0.15/charactergpt_prompts/ready_to_use_prompts/Alys
--rw-rw-rw-   0        0        0     3831 2023-06-17 20:32:06.000000 charactergpt-prompts-0.0.15/charactergpt_prompts/ready_to_use_prompts/Ami
--rw-rw-rw-   0        0        0     3675 2023-06-17 20:57:42.000000 charactergpt-prompts-0.0.15/charactergpt_prompts/ready_to_use_prompts/Sakura
-drwxrwxrwx   0        0        0        0 2023-06-17 22:31:37.527660 charactergpt-prompts-0.0.15/charactergpt_prompts.egg-info/
--rw-rw-rw-   0        0        0      604 2023-06-17 22:31:37.000000 charactergpt-prompts-0.0.15/charactergpt_prompts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      629 2023-06-17 22:31:37.000000 charactergpt-prompts-0.0.15/charactergpt_prompts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 22:31:37.000000 charactergpt-prompts-0.0.15/charactergpt_prompts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-17 22:31:37.000000 charactergpt-prompts-0.0.15/charactergpt_prompts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 22:31:37.532662 charactergpt-prompts-0.0.15/setup.cfg
--rw-rw-rw-   0        0        0      856 2023-06-17 22:31:36.000000 charactergpt-prompts-0.0.15/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 23:46:03.911890 charactergpt-prompts-0.1.0/
+-rw-rw-rw-   0        0        0     1069 2023-06-17 21:13:55.000000 charactergpt-prompts-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3616 2023-06-17 23:46:03.911890 charactergpt-prompts-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3124 2023-06-17 23:44:00.000000 charactergpt-prompts-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 23:46:03.897270 charactergpt-prompts-0.1.0/charactergpt_prompts/
+-rw-rw-rw-   0        0        0        0 2023-06-17 22:10:30.000000 charactergpt-prompts-0.1.0/charactergpt_prompts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 23:46:03.907891 charactergpt-prompts-0.1.0/charactergpt_prompts/additional_data/
+-rw-rw-rw-   0        0        0      262 2023-06-16 21:09:43.000000 charactergpt-prompts-0.1.0/charactergpt_prompts/additional_data/character_gpt_errors.py
+-rw-rw-rw-   0        0        0      433 2023-06-17 19:36:19.000000 charactergpt-prompts-0.1.0/charactergpt_prompts/additional_data/debug_mode_prompt
+-rw-rw-rw-   0        0        0      237 2023-06-16 22:01:44.000000 charactergpt-prompts-0.1.0/charactergpt_prompts/additional_data/prompt_finish
+drwxrwxrwx   0        0        0        0 2023-06-17 23:46:03.910891 charactergpt-prompts-0.1.0/charactergpt_prompts/character_examples/
+-rw-rw-rw-   0        0        0     2675 2023-06-17 19:36:53.000000 charactergpt-prompts-0.1.0/charactergpt_prompts/character_examples/Alys
+-rw-rw-rw-   0        0        0     3831 2023-06-17 20:32:06.000000 charactergpt-prompts-0.1.0/charactergpt_prompts/character_examples/Ami
+-rw-rw-rw-   0        0        0     3675 2023-06-17 20:57:42.000000 charactergpt-prompts-0.1.0/charactergpt_prompts/character_examples/Sakura
+drwxrwxrwx   0        0        0        0 2023-06-17 23:46:03.910891 charactergpt-prompts-0.1.0/charactergpt_prompts/jailbreaks/
+-rw-rw-rw-   0        0        0      912 2023-06-16 22:26:14.000000 charactergpt-prompts-0.1.0/charactergpt_prompts/jailbreaks/default.txt
+-rw-rw-rw-   0        0        0     7767 2023-06-17 23:44:00.000000 charactergpt-prompts-0.1.0/charactergpt_prompts/prompt_generator.py
+drwxrwxrwx   0        0        0        0 2023-06-17 23:46:03.906888 charactergpt-prompts-0.1.0/charactergpt_prompts.egg-info/
+-rw-rw-rw-   0        0        0     3616 2023-06-17 23:46:03.000000 charactergpt-prompts-0.1.0/charactergpt_prompts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      623 2023-06-17 23:46:03.000000 charactergpt-prompts-0.1.0/charactergpt_prompts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 23:46:03.000000 charactergpt-prompts-0.1.0/charactergpt_prompts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-17 23:46:03.000000 charactergpt-prompts-0.1.0/charactergpt_prompts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 23:46:03.912891 charactergpt-prompts-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      853 2023-06-17 23:46:02.000000 charactergpt-prompts-0.1.0/setup.py
```

### Comparing `charactergpt-prompts-0.0.15/LICENSE` & `charactergpt-prompts-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `charactergpt-prompts-0.0.15/charactergpt_prompts/jailbreaks/default.txt` & `charactergpt-prompts-0.1.0/charactergpt_prompts/jailbreaks/default.txt`

 * *Files identical despite different names*

### Comparing `charactergpt-prompts-0.0.15/charactergpt_prompts/prompt_generator.py` & `charactergpt-prompts-0.1.0/charactergpt_prompts/prompt_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from .additional_data.character_gpt_errors import *
-from typing import Union
 import json
 import warnings
 import os
 
 jailbreak_dict={
     "default":"default.txt"
 }
@@ -48,36 +47,39 @@
         self._user_name_for_story=import_data.get("user_name")
         self._story_start_context=import_data.get("story_start_context")
         self._model_author=import_data.get("model_author")
 
 
     def generate_prompt(self):
         tokens_limits=self._get_tokens_limitations()
-        response=f"{self.jailbreak_text}{tokens_limits}{self.get_debug_mode_message()}\n"
+        response=f"{self.jailbreak_text}{tokens_limits}{self._get_debug_mode_message()}\n"
         if self.user_name:
             response+=f"User name for current story: {self.user_name}\n"
         else:
             warnings.warn("User name for current story is not specified. All {{user}} will not be replaced by the username")
         if self.character_description:
             response+=self._generate_character_description()
         else:
             warnings.warn("You didn't provide character description")
         if self.initial_message:
-            response+=f"This is your initial message that you need to start story from: (\"{self._initial_message}\")\n"
+            initial_message=self._initial_message
+            if self.user_name:
+                initial_message=initial_message.replace("{{user}}", self.user_name)
+            response+=f"This is your initial message that you need to start story from: (\"{initial_message}\")\n"
         else:
             warnings.warn("You didn't provide story initial message")
         if self.story_start_context:
             story_start_context=self.story_start_context
             if self.user_name:
                 story_start_context=story_start_context.replace("{{user}}", self.user_name)
             response+=f"Story start context: (\"{story_start_context}\")\n"
         response+=self._prompt_end
         return response
 
-    def get_debug_mode_message(self):
+    def _get_debug_mode_message(self):
         if not self._debug_mode:
             return ""
         with open(os.path.join(current_dir,"additional_data/debug_mode_prompt"), "r") as f:
             return f.read()
 
     def _get_tokens_limitations(self):
         if self.tokens_limit:
@@ -104,24 +106,21 @@
             if self.user_name:
                 element_data=element_data.replace("{{user}}", self.user_name)
             response+=f"{element}=({element_data})\n"
         if not character_information_found:
             warnings.warn("You didn't provide \"Character information\" field in character description")
         return response
 
-    def add_description_parameter(self, key:str, value:Union[str, dict]):
-        self.character_description[key]=value
-
     def add_description_parameters(self, parameters:dict):
         self.character_description.update(parameters)
 
     @staticmethod
     def import_existing_prompt(prompt_name: str=None, filename: str=None):
         if prompt_name:
-            with open(os.path.join(current_dir,f"ready_to_use_prompts/{prompt_name}"), "r", encoding="utf-8") as f:
+            with open(os.path.join(current_dir,f"character_examples/{prompt_name}"), "r", encoding="utf-8") as f:
                 prompt_data=json.loads(f.read())
         elif filename:
             with open(filename, "r", encoding="utf-8") as f:
                 prompt_data = json.loads(f.read())
         else:
             raise PromptImportError
         return GptPrompt(import_data=prompt_data)
```

### Comparing `charactergpt-prompts-0.0.15/charactergpt_prompts/ready_to_use_prompts/Alys` & `charactergpt-prompts-0.1.0/charactergpt_prompts/character_examples/Alys`

 * *Files identical despite different names*

### Comparing `charactergpt-prompts-0.0.15/charactergpt_prompts/ready_to_use_prompts/Ami` & `charactergpt-prompts-0.1.0/charactergpt_prompts/character_examples/Ami`

 * *Files identical despite different names*

### Comparing `charactergpt-prompts-0.0.15/charactergpt_prompts/ready_to_use_prompts/Sakura` & `charactergpt-prompts-0.1.0/charactergpt_prompts/character_examples/Sakura`

 * *Files identical despite different names*

### Comparing `charactergpt-prompts-0.0.15/charactergpt_prompts.egg-info/SOURCES.txt` & `charactergpt-prompts-0.1.0/charactergpt_prompts.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -6,11 +6,11 @@
 charactergpt_prompts.egg-info/PKG-INFO
 charactergpt_prompts.egg-info/SOURCES.txt
 charactergpt_prompts.egg-info/dependency_links.txt
 charactergpt_prompts.egg-info/top_level.txt
 charactergpt_prompts/additional_data/character_gpt_errors.py
 charactergpt_prompts/additional_data/debug_mode_prompt
 charactergpt_prompts/additional_data/prompt_finish
-charactergpt_prompts/jailbreaks/default.txt
-charactergpt_prompts/ready_to_use_prompts/Alys
-charactergpt_prompts/ready_to_use_prompts/Ami
-charactergpt_prompts/ready_to_use_prompts/Sakura
+charactergpt_prompts/character_examples/Alys
+charactergpt_prompts/character_examples/Ami
+charactergpt_prompts/character_examples/Sakura
+charactergpt_prompts/jailbreaks/default.txt
```

### Comparing `charactergpt-prompts-0.0.15/setup.py` & `charactergpt-prompts-0.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="charactergpt-prompts",
-    version="0.0.15",
+    version="0.1.0",
     author="Hikki-e",
     author_email="zmk383@gmail.com",
     description="This library is designed to make the creation of characters for roll-play in ChatGPT much easier",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hikki-e/CharacterGPT",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 package_data={
-        'charactergpt_prompts': ['additional_data/*', "jailbreaks/*", "ready_to_use_prompts/*"],
+        'charactergpt_prompts': ['additional_data/*', "jailbreaks/*", "character_examples/*"],
     },
 include_package_data=True
 )
```

