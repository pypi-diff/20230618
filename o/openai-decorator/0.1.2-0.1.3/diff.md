# Comparing `tmp/openai_decorator-0.1.2.tar.gz` & `tmp/openai_decorator-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_decorator-0.1.2.tar", max compression
+gzip compressed data, was "openai_decorator-0.1.3.tar", max compression
```

## Comparing `openai_decorator-0.1.2.tar` & `openai_decorator-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-06-18 19:33:11.672235 openai_decorator-0.1.2/LICENSE
--rw-r--r--   0        0        0     5814 2023-06-18 19:33:11.672235 openai_decorator-0.1.2/README.md
--rw-r--r--   0        0        0     1650 2023-06-18 19:33:11.672235 openai_decorator-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       30 2023-06-18 19:33:11.672235 openai_decorator-0.1.2/src/openai_decorator/__init__.py
--rw-r--r--   0        0        0     6813 2023-06-18 19:33:11.672235 openai_decorator-0.1.2/src/openai_decorator/main.py
--rw-r--r--   0        0        0     7085 1970-01-01 00:00:00.000000 openai_decorator-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-18 21:03:30.596884 openai_decorator-0.1.3/LICENSE
+-rw-r--r--   0        0        0     5814 2023-06-18 21:03:30.596884 openai_decorator-0.1.3/README.md
+-rw-r--r--   0        0        0     1643 2023-06-18 21:03:30.596884 openai_decorator-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-06-18 21:03:30.596884 openai_decorator-0.1.3/src/openai_decorator/__init__.py
+-rw-r--r--   0        0        0     6813 2023-06-18 21:03:30.596884 openai_decorator-0.1.3/src/openai_decorator/main.py
+-rw-r--r--   0        0        0     7084 1970-01-01 00:00:00.000000 openai_decorator-0.1.3/PKG-INFO
```

### Comparing `openai_decorator-0.1.2/LICENSE` & `openai_decorator-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_decorator-0.1.2/README.md` & `openai_decorator-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `openai_decorator-0.1.2/pyproject.toml` & `openai_decorator-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-decorator"
-version = "0.1.2"
+version = "0.1.3"
 description = "This package allows you to genrate function paramater values by integrating OpenAI's API function capabilities through signature and docstring analysis."
 authors = ["Shruti Patel <shruti222patel@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/shruti222patel/openai-decorator"
 packages = [{include = "openai_decorator", from = "src"}]
 keywords = ["openai", "decorator", "functions", "openai-functions", "openai-decorator", "openai-api", "openai-api-functions", "openai-api-decorator", "openai"]
@@ -17,15 +17,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = "^3.8"
 openai = "^0.27.8"
 docstring-parser = "^0.15"
 requests = "^2.31.0"
 tenacity = "^8.2.2"
 
 [tool.poetry.scripts]
 add-docstring = "openai_decorator.main:main"
```

### Comparing `openai_decorator-0.1.2/src/openai_decorator/main.py` & `openai_decorator-0.1.3/src/openai_decorator/main.py`

 * *Files identical despite different names*

### Comparing `openai_decorator-0.1.2/PKG-INFO` & `openai_decorator-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: openai-decorator
-Version: 0.1.2
+Version: 0.1.3
 Summary: This package allows you to genrate function paramater values by integrating OpenAI's API function capabilities through signature and docstring analysis.
 Home-page: https://github.com/shruti222patel/openai-decorator
 License: MIT
 Keywords: openai,decorator,functions,openai-functions,openai-decorator,openai-api,openai-api-functions,openai-api-decorator,openai
 Author: Shruti Patel
 Author-email: shruti222patel@gmail.com
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

