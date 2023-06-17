# Comparing `tmp/charactergpt-prompts-0.0.1.tar.gz` & `tmp/charactergpt-prompts-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charactergpt-prompts-0.0.1.tar", last modified: Sat Jun 17 21:32:29 2023, max compression
+gzip compressed data, was "charactergpt-prompts-0.0.12.tar", last modified: Sat Jun 17 21:57:26 2023, max compression
```

## Comparing `charactergpt-prompts-0.0.1.tar` & `charactergpt-prompts-0.0.12.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 21:32:29.439104 charactergpt-prompts-0.0.1/
--rw-rw-rw-   0        0        0     1069 2023-06-17 21:13:55.000000 charactergpt-prompts-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      603 2023-06-17 21:32:29.438104 charactergpt-prompts-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      113 2023-06-17 21:03:43.000000 charactergpt-prompts-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 21:32:29.437105 charactergpt-prompts-0.0.1/charactergpt_prompts.egg-info/
--rw-rw-rw-   0        0        0      603 2023-06-17 21:32:29.000000 charactergpt-prompts-0.0.1/charactergpt_prompts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-06-17 21:32:29.000000 charactergpt-prompts-0.0.1/charactergpt_prompts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 21:32:29.000000 charactergpt-prompts-0.0.1/charactergpt_prompts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 21:32:29.000000 charactergpt-prompts-0.0.1/charactergpt_prompts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 21:32:29.439104 charactergpt-prompts-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      706 2023-06-17 21:14:13.000000 charactergpt-prompts-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 21:57:26.517873 charactergpt-prompts-0.0.12/
+-rw-rw-rw-   0        0        0     1069 2023-06-17 21:13:55.000000 charactergpt-prompts-0.0.12/LICENSE
+-rw-rw-rw-   0        0        0      604 2023-06-17 21:57:26.516872 charactergpt-prompts-0.0.12/PKG-INFO
+-rw-rw-rw-   0        0        0      113 2023-06-17 21:03:43.000000 charactergpt-prompts-0.0.12/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 21:57:26.515872 charactergpt-prompts-0.0.12/charactergpt_prompts.egg-info/
+-rw-rw-rw-   0        0        0      604 2023-06-17 21:57:26.000000 charactergpt-prompts-0.0.12/charactergpt_prompts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-06-17 21:57:26.000000 charactergpt-prompts-0.0.12/charactergpt_prompts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 21:57:26.000000 charactergpt-prompts-0.0.12/charactergpt_prompts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 21:57:26.000000 charactergpt-prompts-0.0.12/charactergpt_prompts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 21:57:26.517873 charactergpt-prompts-0.0.12/setup.cfg
+-rw-rw-rw-   0        0        0      707 2023-06-17 21:57:06.000000 charactergpt-prompts-0.0.12/setup.py
```

### Comparing `charactergpt-prompts-0.0.1/LICENSE` & `charactergpt-prompts-0.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `charactergpt-prompts-0.0.1/PKG-INFO` & `charactergpt-prompts-0.0.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charactergpt-prompts
-Version: 0.0.1
+Version: 0.0.12
 Summary: This library is designed to make the creation of characters for roll-play in ChatGPT much easier
 Home-page: https://github.com/hikki-e/CharacterGPT
 Author: Hikki-e
 Author-email: zmk383@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `charactergpt-prompts-0.0.1/charactergpt_prompts.egg-info/PKG-INFO` & `charactergpt-prompts-0.0.12/charactergpt_prompts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charactergpt-prompts
-Version: 0.0.1
+Version: 0.0.12
 Summary: This library is designed to make the creation of characters for roll-play in ChatGPT much easier
 Home-page: https://github.com/hikki-e/CharacterGPT
 Author: Hikki-e
 Author-email: zmk383@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `charactergpt-prompts-0.0.1/setup.py` & `charactergpt-prompts-0.0.12/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="charactergpt-prompts",
-    version="0.0.1",
+    version="0.0.12",
     author="Hikki-e",
     author_email="zmk383@gmail.com",
     description="This library is designed to make the creation of characters for roll-play in ChatGPT much easier",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hikki-e/CharacterGPT",
     packages=setuptools.find_packages(),
```

