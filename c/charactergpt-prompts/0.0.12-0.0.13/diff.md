# Comparing `tmp/charactergpt-prompts-0.0.12.tar.gz` & `tmp/charactergpt-prompts-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charactergpt-prompts-0.0.12.tar", last modified: Sat Jun 17 21:57:26 2023, max compression
+gzip compressed data, was "charactergpt-prompts-0.0.13.tar", last modified: Sat Jun 17 22:22:32 2023, max compression
```

## Comparing `charactergpt-prompts-0.0.12.tar` & `charactergpt-prompts-0.0.13.tar`

### file list

```diff
@@ -1,11 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 21:57:26.517873 charactergpt-prompts-0.0.12/
--rw-rw-rw-   0        0        0     1069 2023-06-17 21:13:55.000000 charactergpt-prompts-0.0.12/LICENSE
--rw-rw-rw-   0        0        0      604 2023-06-17 21:57:26.516872 charactergpt-prompts-0.0.12/PKG-INFO
--rw-rw-rw-   0        0        0      113 2023-06-17 21:03:43.000000 charactergpt-prompts-0.0.12/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 21:57:26.515872 charactergpt-prompts-0.0.12/charactergpt_prompts.egg-info/
--rw-rw-rw-   0        0        0      604 2023-06-17 21:57:26.000000 charactergpt-prompts-0.0.12/charactergpt_prompts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-06-17 21:57:26.000000 charactergpt-prompts-0.0.12/charactergpt_prompts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 21:57:26.000000 charactergpt-prompts-0.0.12/charactergpt_prompts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 21:57:26.000000 charactergpt-prompts-0.0.12/charactergpt_prompts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 21:57:26.517873 charactergpt-prompts-0.0.12/setup.cfg
--rw-rw-rw-   0        0        0      707 2023-06-17 21:57:06.000000 charactergpt-prompts-0.0.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 22:22:32.223116 charactergpt-prompts-0.0.13/
+-rw-rw-rw-   0        0        0     1069 2023-06-17 21:13:55.000000 charactergpt-prompts-0.0.13/LICENSE
+-rw-rw-rw-   0        0        0      604 2023-06-17 22:22:32.223116 charactergpt-prompts-0.0.13/PKG-INFO
+-rw-rw-rw-   0        0        0      113 2023-06-17 21:03:43.000000 charactergpt-prompts-0.0.13/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 22:22:32.213116 charactergpt-prompts-0.0.13/charactergpt_prompts/
+-rw-rw-rw-   0        0        0        0 2023-06-17 22:10:30.000000 charactergpt-prompts-0.0.13/charactergpt_prompts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 22:22:32.219116 charactergpt-prompts-0.0.13/charactergpt_prompts/additional_data/
+-rw-rw-rw-   0        0        0      262 2023-06-16 21:09:43.000000 charactergpt-prompts-0.0.13/charactergpt_prompts/additional_data/character_gpt_errors.py
+-rw-rw-rw-   0        0        0      433 2023-06-17 19:36:19.000000 charactergpt-prompts-0.0.13/charactergpt_prompts/additional_data/debug_mode_prompt
+-rw-rw-rw-   0        0        0      237 2023-06-16 22:01:44.000000 charactergpt-prompts-0.0.13/charactergpt_prompts/additional_data/prompt_finish
+drwxrwxrwx   0        0        0        0 2023-06-17 22:22:32.220116 charactergpt-prompts-0.0.13/charactergpt_prompts/jailbreaks/
+-rw-rw-rw-   0        0        0      912 2023-06-16 22:26:14.000000 charactergpt-prompts-0.0.13/charactergpt_prompts/jailbreaks/default.txt
+-rw-rw-rw-   0        0        0     7754 2023-06-17 21:53:19.000000 charactergpt-prompts-0.0.13/charactergpt_prompts/prompt_generator.py
+drwxrwxrwx   0        0        0        0 2023-06-17 22:22:32.222116 charactergpt-prompts-0.0.13/charactergpt_prompts/ready_to_use_prompts/
+-rw-rw-rw-   0        0        0     2675 2023-06-17 19:36:53.000000 charactergpt-prompts-0.0.13/charactergpt_prompts/ready_to_use_prompts/Alys
+-rw-rw-rw-   0        0        0     3831 2023-06-17 20:32:06.000000 charactergpt-prompts-0.0.13/charactergpt_prompts/ready_to_use_prompts/Ami
+-rw-rw-rw-   0        0        0     3675 2023-06-17 20:57:42.000000 charactergpt-prompts-0.0.13/charactergpt_prompts/ready_to_use_prompts/Sakura
+drwxrwxrwx   0        0        0        0 2023-06-17 22:22:32.217116 charactergpt-prompts-0.0.13/charactergpt_prompts.egg-info/
+-rw-rw-rw-   0        0        0      604 2023-06-17 22:22:32.000000 charactergpt-prompts-0.0.13/charactergpt_prompts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2023-06-17 22:22:32.000000 charactergpt-prompts-0.0.13/charactergpt_prompts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 22:22:32.000000 charactergpt-prompts-0.0.13/charactergpt_prompts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-17 22:22:32.000000 charactergpt-prompts-0.0.13/charactergpt_prompts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 22:22:32.223116 charactergpt-prompts-0.0.13/setup.cfg
+-rw-rw-rw-   0        0        0      829 2023-06-17 22:21:04.000000 charactergpt-prompts-0.0.13/setup.py
```

### Comparing `charactergpt-prompts-0.0.12/LICENSE` & `charactergpt-prompts-0.0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `charactergpt-prompts-0.0.12/PKG-INFO` & `charactergpt-prompts-0.0.13/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charactergpt-prompts
-Version: 0.0.12
+Version: 0.0.13
 Summary: This library is designed to make the creation of characters for roll-play in ChatGPT much easier
 Home-page: https://github.com/hikki-e/CharacterGPT
 Author: Hikki-e
 Author-email: zmk383@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `charactergpt-prompts-0.0.12/charactergpt_prompts.egg-info/PKG-INFO` & `charactergpt-prompts-0.0.13/charactergpt_prompts.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charactergpt-prompts
-Version: 0.0.12
+Version: 0.0.13
 Summary: This library is designed to make the creation of characters for roll-play in ChatGPT much easier
 Home-page: https://github.com/hikki-e/CharacterGPT
 Author: Hikki-e
 Author-email: zmk383@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `charactergpt-prompts-0.0.12/setup.py` & `charactergpt-prompts-0.0.13/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="charactergpt-prompts",
-    version="0.0.12",
+    version="0.0.13",
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
+package_data={
+        'charactergpt_prompts': ['additional_data/*', "jailbreaks/*", "ready_to_use_prompts/*"],
+    },
 )
```

