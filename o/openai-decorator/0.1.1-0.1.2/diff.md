# Comparing `tmp/openai_decorator-0.1.1.tar.gz` & `tmp/openai_decorator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_decorator-0.1.1.tar", max compression
+gzip compressed data, was "openai_decorator-0.1.2.tar", max compression
```

## Comparing `openai_decorator-0.1.1.tar` & `openai_decorator-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-06-18 19:24:44.403092 openai_decorator-0.1.1/LICENSE
--rw-r--r--   0        0        0     5814 2023-06-18 19:24:44.403092 openai_decorator-0.1.1/README.md
--rw-r--r--   0        0        0     1490 2023-06-18 19:24:44.403092 openai_decorator-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       30 2023-06-18 19:24:44.403092 openai_decorator-0.1.1/src/openai_decorator/__init__.py
--rw-r--r--   0        0        0     6813 2023-06-18 19:24:44.403092 openai_decorator-0.1.1/src/openai_decorator/main.py
--rw-r--r--   0        0        0     6954 1970-01-01 00:00:00.000000 openai_decorator-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-18 19:33:11.672235 openai_decorator-0.1.2/LICENSE
+-rw-r--r--   0        0        0     5814 2023-06-18 19:33:11.672235 openai_decorator-0.1.2/README.md
+-rw-r--r--   0        0        0     1650 2023-06-18 19:33:11.672235 openai_decorator-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-06-18 19:33:11.672235 openai_decorator-0.1.2/src/openai_decorator/__init__.py
+-rw-r--r--   0        0        0     6813 2023-06-18 19:33:11.672235 openai_decorator-0.1.2/src/openai_decorator/main.py
+-rw-r--r--   0        0        0     7085 1970-01-01 00:00:00.000000 openai_decorator-0.1.2/PKG-INFO
```

### Comparing `openai_decorator-0.1.1/LICENSE` & `openai_decorator-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_decorator-0.1.1/README.md` & `openai_decorator-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `openai_decorator-0.1.1/pyproject.toml` & `openai_decorator-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tool.poetry]
 name = "openai-decorator"
-version = "0.1.1"
+version = "0.1.2"
 description = "This package allows you to genrate function paramater values by integrating OpenAI's API function capabilities through signature and docstring analysis."
 authors = ["Shruti Patel <shruti222patel@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/shruti222patel/openai-decorator"
 packages = [{include = "openai_decorator", from = "src"}]
+keywords = ["openai", "decorator", "functions", "openai-functions", "openai-decorator", "openai-api", "openai-api-functions", "openai-api-decorator", "openai"]
 classifiers = [
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
```

### Comparing `openai_decorator-0.1.1/src/openai_decorator/main.py` & `openai_decorator-0.1.2/src/openai_decorator/main.py`

 * *Files identical despite different names*

### Comparing `openai_decorator-0.1.1/PKG-INFO` & `openai_decorator-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: openai-decorator
-Version: 0.1.1
+Version: 0.1.2
 Summary: This package allows you to genrate function paramater values by integrating OpenAI's API function capabilities through signature and docstring analysis.
 Home-page: https://github.com/shruti222patel/openai-decorator
 License: MIT
+Keywords: openai,decorator,functions,openai-functions,openai-decorator,openai-api,openai-api-functions,openai-api-decorator,openai
 Author: Shruti Patel
 Author-email: shruti222patel@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

