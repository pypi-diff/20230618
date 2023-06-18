# Comparing `tmp/openai_decorator-0.1.0.tar.gz` & `tmp/openai_decorator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_decorator-0.1.0.tar", max compression
+gzip compressed data, was "openai_decorator-0.1.1.tar", max compression
```

## Comparing `openai_decorator-0.1.0.tar` & `openai_decorator-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-06-18 16:16:40.037203 openai_decorator-0.1.0/LICENSE
--rw-r--r--   0        0        0     5814 2023-06-18 16:16:40.037203 openai_decorator-0.1.0/README.md
--rw-r--r--   0        0        0      762 2023-06-18 16:16:40.037203 openai_decorator-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       30 2023-06-18 16:16:40.037203 openai_decorator-0.1.0/src/openai_decorator/__init__.py
--rw-r--r--   0        0        0     6813 2023-06-18 16:16:40.037203 openai_decorator-0.1.0/src/openai_decorator/main.py
--rw-r--r--   0        0        0     6330 1970-01-01 00:00:00.000000 openai_decorator-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-18 19:24:44.403092 openai_decorator-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5814 2023-06-18 19:24:44.403092 openai_decorator-0.1.1/README.md
+-rw-r--r--   0        0        0     1490 2023-06-18 19:24:44.403092 openai_decorator-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-06-18 19:24:44.403092 openai_decorator-0.1.1/src/openai_decorator/__init__.py
+-rw-r--r--   0        0        0     6813 2023-06-18 19:24:44.403092 openai_decorator-0.1.1/src/openai_decorator/main.py
+-rw-r--r--   0        0        0     6954 1970-01-01 00:00:00.000000 openai_decorator-0.1.1/PKG-INFO
```

### Comparing `openai_decorator-0.1.0/LICENSE` & `openai_decorator-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_decorator-0.1.0/README.md` & `openai_decorator-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -167,14 +167,14 @@
 
 - [x] Handle optional parameters.
 - [x] Handle parameters with default values.
 - [ ] Add test to ensure default values are used if OpenAI doesn't return parameters.
 - [ ] Publish the package to PyPI.
 - [ ] Expand test coverage.
 - [ ] Show tests passing & coverage as github badges.
-- [ ] Fix CI/CD -- Address the issue where the pre-release deployment to PyPI fails due to the need for version update.
+- [X] Fix CI/CD -- Address the issue where the pre-release deployment to PyPI fails due to the need for version update.
 - [ ] Add docstrings.
 - [ ] Generate docs (from docstrings).
 
 ## License
 
 This project is under the MIT License. See the [LICENSE](LICENSE) file for more details.
```

### Comparing `openai_decorator-0.1.0/src/openai_decorator/main.py` & `openai_decorator-0.1.1/src/openai_decorator/main.py`

 * *Files identical despite different names*

### Comparing `openai_decorator-0.1.0/PKG-INFO` & `openai_decorator-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 Metadata-Version: 2.1
 Name: openai-decorator
-Version: 0.1.0
-Summary: 
+Version: 0.1.1
+Summary: This package allows you to genrate function paramater values by integrating OpenAI's API function capabilities through signature and docstring analysis.
+Home-page: https://github.com/shruti222patel/openai-decorator
+License: MIT
 Author: Shruti Patel
 Author-email: shruti222patel@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.8,<3.12
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: docstring-parser (>=0.15,<0.16)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
-Requires-Dist: pytest-mock (>=3.11.1,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
+Project-URL: Repository, https://github.com/shruti222patel/openai-decorator
 Description-Content-Type: text/markdown
 
 # OpenAI Decorator
 
 The OpenAI Decorator is a Python package that enriches your Python functions with the capabilities of OpenAI's API. It leverages the function's signature and docstring to generate specifications comprehensible by OpenAI's API, subsequently making a request to the API.
 
 ## Table of Contents
@@ -183,15 +192,15 @@
 
 - [x] Handle optional parameters.
 - [x] Handle parameters with default values.
 - [ ] Add test to ensure default values are used if OpenAI doesn't return parameters.
 - [ ] Publish the package to PyPI.
 - [ ] Expand test coverage.
 - [ ] Show tests passing & coverage as github badges.
-- [ ] Fix CI/CD -- Address the issue where the pre-release deployment to PyPI fails due to the need for version update.
+- [X] Fix CI/CD -- Address the issue where the pre-release deployment to PyPI fails due to the need for version update.
 - [ ] Add docstrings.
 - [ ] Generate docs (from docstrings).
 
 ## License
 
 This project is under the MIT License. See the [LICENSE](LICENSE) file for more details.
```

