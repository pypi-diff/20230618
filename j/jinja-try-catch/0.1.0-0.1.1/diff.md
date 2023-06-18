# Comparing `tmp/jinja_try_catch-0.1.0.tar.gz` & `tmp/jinja_try_catch-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinja_try_catch-0.1.0.tar", max compression
+gzip compressed data, was "jinja_try_catch-0.1.1.tar", max compression
```

## Comparing `jinja_try_catch-0.1.0.tar` & `jinja_try_catch-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      362 2023-06-18 08:29:12.367772 jinja_try_catch-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1067 2023-06-18 08:12:00.806186 jinja_try_catch-0.1.0/LICENSE
--rw-r--r--   0        0        0     1300 2023-06-18 08:23:53.589138 jinja_try_catch-0.1.0/README.md
--rw-r--r--   0        0        0       41 2023-06-18 08:14:15.425031 jinja_try_catch-0.1.0/jinja_try_catch/__init__.py
--rw-r--r--   0        0        0     3485 2023-06-18 07:59:10.909400 jinja_try_catch-0.1.0/jinja_try_catch/extension.py
--rw-r--r--   0        0        0     1784 2023-06-18 08:27:46.973997 jinja_try_catch-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-18 07:04:21.004229 jinja_try_catch-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     5808 2023-06-18 08:01:49.112962 jinja_try_catch-0.1.0/tests/test_try_catch.py
--rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 jinja_try_catch-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      524 2023-06-18 17:15:52.809820 jinja_try_catch-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1067 2023-06-18 08:12:00.806186 jinja_try_catch-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1300 2023-06-18 08:23:53.589138 jinja_try_catch-0.1.1/README.md
+-rw-r--r--   0        0        0       41 2023-06-18 08:14:15.425031 jinja_try_catch-0.1.1/jinja_try_catch/__init__.py
+-rw-r--r--   0        0        0     3485 2023-06-18 07:59:10.909400 jinja_try_catch-0.1.1/jinja_try_catch/extension.py
+-rw-r--r--   0        0        0     2219 2023-06-18 17:15:52.537814 jinja_try_catch-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-18 07:04:21.004229 jinja_try_catch-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     5820 2023-06-18 17:02:37.674764 jinja_try_catch-0.1.1/tests/test_try_catch.py
+-rw-r--r--   0        0        0     2403 1970-01-01 00:00:00.000000 jinja_try_catch-0.1.1/PKG-INFO
```

### Comparing `jinja_try_catch-0.1.0/LICENSE` & `jinja_try_catch-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jinja_try_catch-0.1.0/README.md` & `jinja_try_catch-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `jinja_try_catch-0.1.0/jinja_try_catch/extension.py` & `jinja_try_catch-0.1.1/jinja_try_catch/extension.py`

 * *Files identical despite different names*

### Comparing `jinja_try_catch-0.1.0/pyproject.toml` & `jinja_try_catch-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 [tool.poetry]
 name = "jinja-try-catch"
-version = "0.1.0"
+version = "0.1.1"
 description = "Jinja2 extension adding {% try %} {% catch %} exception handling"
 authors = ["Zach Kanzler <zach@rewst.io>"]
+repository = "https://github.com/RewstApp/jinja-try-catch"
+homepage = "https://github.com/RewstApp/jinja-try-catch"
 license = "MIT"
 readme = "README.md"
 packages = [
   { include = "jinja_try_catch" },
   { include = "tests", format = "sdist" },
   { include = "pyproject.toml", format = "sdist" },
   { include = "LICENSE", format = "sdist" },
   { include = "CHANGELOG.md", format = "sdist" },
 ]
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Environment :: Web Environment",
+    "Intended Audience :: Developers",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
+    "Topic :: Text Processing :: Markup :: HTML",
+]
 
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 Jinja2 = ">=3.0.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `jinja_try_catch-0.1.0/tests/test_try_catch.py` & `jinja_try_catch-0.1.1/tests/test_try_catch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Any, Callable
+from typing import Any, Callable, Dict, Type
 
 import jinja2
 import jinja2.ext
 import jinja2.nativetypes
 import pytest
 
 from jinja_try_catch.extension import TryCatchExtension
 
 
 @pytest.fixture
-def env_kwargs() -> dict[str, Any]:
+def env_kwargs() -> Dict[str, Any]:
     return dict(
         extensions=[
             TryCatchExtension,
             jinja2.ext.ExprStmtExtension,
         ],
         undefined=jinja2.StrictUndefined,
     )
@@ -24,15 +24,15 @@
     pytest.param(True, id='native'),
 ])
 def is_native_env(request) -> bool:
     return request.param
 
 
 @pytest.fixture
-def env_class(is_native_env) -> type[jinja2.Environment]:
+def env_class(is_native_env) -> Type[jinja2.Environment]:
     return jinja2.nativetypes.NativeEnvironment if is_native_env else jinja2.Environment
 
 
 @pytest.fixture
 def preprocess_expected(is_native_env) -> Callable[[Any], Any]:
     return (lambda o: o) if is_native_env else str
```

### Comparing `jinja_try_catch-0.1.0/PKG-INFO` & `jinja_try_catch-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 Metadata-Version: 2.1
 Name: jinja-try-catch
-Version: 0.1.0
+Version: 0.1.1
 Summary: Jinja2 extension adding {% try %} {% catch %} exception handling
+Home-page: https://github.com/RewstApp/jinja-try-catch
 License: MIT
 Author: Zach Kanzler
 Author-email: zach@rewst.io
 Requires-Python: >=3.7
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Text Processing :: Markup :: HTML
 Requires-Dist: Jinja2 (>=3.0.0)
+Project-URL: Repository, https://github.com/RewstApp/jinja-try-catch
 Description-Content-Type: text/markdown
 
 # jinja-try-catch
 A Jinja2 extension providing exception handling within templates.
 
 ```jinja
 {%- try -%}
```

