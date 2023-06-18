# Comparing `tmp/libre_fastapi_jwt-0.20.2.tar.gz` & `tmp/libre_fastapi_jwt-0.20.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libre_fastapi_jwt-0.20.2.tar", max compression
+gzip compressed data, was "libre_fastapi_jwt-0.20.3.tar", max compression
```

## Comparing `libre_fastapi_jwt-0.20.2.tar` & `libre_fastapi_jwt-0.20.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-06-18 04:07:22.708806 libre_fastapi_jwt-0.20.2/LICENSE
--rw-r--r--   0        0        0     2095 2023-06-18 04:07:22.708806 libre_fastapi_jwt-0.20.2/README.md
--rw-r--r--   0        0        0      148 2023-06-18 04:07:22.712806 libre_fastapi_jwt-0.20.2/libre_fastapi_jwt/__init__.py
--rw-r--r--   0        0        0     5423 2023-06-18 04:07:22.712806 libre_fastapi_jwt-0.20.2/libre_fastapi_jwt/auth_config.py
--rw-r--r--   0        0        0    41338 2023-06-18 04:07:22.712806 libre_fastapi_jwt-0.20.2/libre_fastapi_jwt/auth_jwt.py
--rw-r--r--   0        0        0     4700 2023-06-18 04:07:22.712806 libre_fastapi_jwt-0.20.2/libre_fastapi_jwt/config.py
--rw-r--r--   0        0        0     3059 2023-06-18 04:07:22.712806 libre_fastapi_jwt-0.20.2/libre_fastapi_jwt/exceptions.py
--rw-r--r--   0        0        0     1077 2023-06-18 04:07:22.712806 libre_fastapi_jwt-0.20.2/pyproject.toml
--rw-r--r--   0        0        0     3176 1970-01-01 00:00:00.000000 libre_fastapi_jwt-0.20.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-18 04:26:14.673616 libre_fastapi_jwt-0.20.3/LICENSE
+-rw-r--r--   0        0        0     2091 2023-06-18 04:26:14.673616 libre_fastapi_jwt-0.20.3/README.md
+-rw-r--r--   0        0        0      148 2023-06-18 04:26:14.673616 libre_fastapi_jwt-0.20.3/libre_fastapi_jwt/__init__.py
+-rw-r--r--   0        0        0     5423 2023-06-18 04:26:14.673616 libre_fastapi_jwt-0.20.3/libre_fastapi_jwt/auth_config.py
+-rw-r--r--   0        0        0    41338 2023-06-18 04:26:14.673616 libre_fastapi_jwt-0.20.3/libre_fastapi_jwt/auth_jwt.py
+-rw-r--r--   0        0        0     4700 2023-06-18 04:26:14.673616 libre_fastapi_jwt-0.20.3/libre_fastapi_jwt/config.py
+-rw-r--r--   0        0        0     3059 2023-06-18 04:26:14.673616 libre_fastapi_jwt-0.20.3/libre_fastapi_jwt/exceptions.py
+-rw-r--r--   0        0        0     1077 2023-06-18 04:26:14.677616 libre_fastapi_jwt-0.20.3/pyproject.toml
+-rw-r--r--   0        0        0     3172 1970-01-01 00:00:00.000000 libre_fastapi_jwt-0.20.3/PKG-INFO
```

### Comparing `libre_fastapi_jwt-0.20.2/LICENSE` & `libre_fastapi_jwt-0.20.3/LICENSE`

 * *Files identical despite different names*

### Comparing `libre_fastapi_jwt-0.20.2/README.md` & `libre_fastapi_jwt-0.20.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <h1 align="left" style="margin-bottom: 20px; font-weight: 500; font-size: 50px; color: black;">
   FastAPI JWT Auth
 </h1>
 
-[![Tests](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/tests.yml)
-[![CodeQL](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/codeql.yml/badge.svg?branch=master)](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/codeql.yml)
+[![Tests](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/tests.yml)
+[![CodeQL](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/codeql.yml/badge.svg?branch=main)](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/codeql.yml)
 [![PyPI version](https://badge.fury.io/py/libre-fastapi-jwt.svg)](https://badge.fury.io/py/libre-fastapi-jwt)
 [![Downloads](https://static.pepy.tech/personalized-badge/libre-fastapi-jwt?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/libre-fastapi-jwt)
 
 ---
 <h3> BTW - The project is based on <a href="https://pypi.org/project/libre-fastapi-jwt/" target="_blank">Fastapi-jwt-auth</a> that is no longer maintained. </h3> 
 
 **Documentation**: <a href="https://LibreNZ.github.io/libre-fastapi-jwt" target="_blank">https://LibreNZ.github.io/libre-fastapi-jwt</a>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 ****** FastAPI JWT Auth ******
 [![Tests](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/
-tests.yml/badge.svg?branch=master)](https://github.com/LibreNZ/libre-fastapi-
-jwt/actions/workflows/tests.yml) [![CodeQL](https://github.com/LibreNZ/libre-
-fastapi-jwt/actions/workflows/codeql.yml/badge.svg?branch=master)](https://
+tests.yml/badge.svg?branch=main)](https://github.com/LibreNZ/libre-fastapi-jwt/
+actions/workflows/tests.yml) [![CodeQL](https://github.com/LibreNZ/libre-
+fastapi-jwt/actions/workflows/codeql.yml/badge.svg?branch=main)](https://
 github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/codeql.yml) [![PyPI
 version](https://badge.fury.io/py/libre-fastapi-jwt.svg)](https://
 badge.fury.io/py/libre-fastapi-jwt) [![Downloads](https://static.pepy.tech/
 personalized-badge/libre-fastapi-
 jwt?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)]
 (https://pepy.tech/project/libre-fastapi-jwt) ---
 **** BTW - The project is based on Fastapi-jwt-auth that is no longer
```

### Comparing `libre_fastapi_jwt-0.20.2/libre_fastapi_jwt/auth_config.py` & `libre_fastapi_jwt-0.20.3/libre_fastapi_jwt/auth_config.py`

 * *Files identical despite different names*

### Comparing `libre_fastapi_jwt-0.20.2/libre_fastapi_jwt/auth_jwt.py` & `libre_fastapi_jwt-0.20.3/libre_fastapi_jwt/auth_jwt.py`

 * *Files identical despite different names*

### Comparing `libre_fastapi_jwt-0.20.2/libre_fastapi_jwt/config.py` & `libre_fastapi_jwt-0.20.3/libre_fastapi_jwt/config.py`

 * *Files identical despite different names*

### Comparing `libre_fastapi_jwt-0.20.2/libre_fastapi_jwt/exceptions.py` & `libre_fastapi_jwt-0.20.3/libre_fastapi_jwt/exceptions.py`

 * *Files identical despite different names*

### Comparing `libre_fastapi_jwt-0.20.2/pyproject.toml` & `libre_fastapi_jwt-0.20.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "libre-fastapi-jwt"
-version = "0.20.2"
+version = "0.20.3"
 description = "Yet another fork of fast-jwt-auth"
 authors = ["Libre NZ <github-support@libre.nz>"]
 license = "MIT"
 repository = "https://github.com/LibreNZ/libre-fastapi-jwt"
 readme = "README.md"
 classifiers = [
   "Environment :: Web Environment",
```

### Comparing `libre_fastapi_jwt-0.20.2/PKG-INFO` & `libre_fastapi_jwt-0.20.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libre-fastapi-jwt
-Version: 0.20.2
+Version: 0.20.3
 Summary: Yet another fork of fast-jwt-auth
 Home-page: https://github.com/LibreNZ/libre-fastapi-jwt
 License: MIT
 Author: Libre NZ
 Author-email: github-support@libre.nz
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Web Environment
@@ -25,16 +25,16 @@
 Project-URL: Repository, https://github.com/LibreNZ/libre-fastapi-jwt
 Description-Content-Type: text/markdown
 
 <h1 align="left" style="margin-bottom: 20px; font-weight: 500; font-size: 50px; color: black;">
   FastAPI JWT Auth
 </h1>
 
-[![Tests](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/tests.yml)
-[![CodeQL](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/codeql.yml/badge.svg?branch=master)](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/codeql.yml)
+[![Tests](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/tests.yml)
+[![CodeQL](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/codeql.yml/badge.svg?branch=main)](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/codeql.yml)
 [![PyPI version](https://badge.fury.io/py/libre-fastapi-jwt.svg)](https://badge.fury.io/py/libre-fastapi-jwt)
 [![Downloads](https://static.pepy.tech/personalized-badge/libre-fastapi-jwt?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/libre-fastapi-jwt)
 
 ---
 <h3> BTW - The project is based on <a href="https://pypi.org/project/libre-fastapi-jwt/" target="_blank">Fastapi-jwt-auth</a> that is no longer maintained. </h3> 
 
 **Documentation**: <a href="https://LibreNZ.github.io/libre-fastapi-jwt" target="_blank">https://LibreNZ.github.io/libre-fastapi-jwt</a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: libre-fastapi-jwt Version: 0.20.2 Summary: Yet
+Metadata-Version: 2.1 Name: libre-fastapi-jwt Version: 0.20.3 Summary: Yet
 another fork of fast-jwt-auth Home-page: https://github.com/LibreNZ/libre-
 fastapi-jwt License: MIT Author: Libre NZ Author-email: github-support@libre.nz
 Requires-Python: >=3.8,<4.0 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
@@ -11,17 +11,17 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: PyJWT (>=2.6.0,<3.0.0) Requires-Dist: cryptography (>=41.0.0)
 Requires-Dist: fastapi (>=0.95.1) Requires-Dist: httpx (>=0.14.0) Project-URL:
 Repository, https://github.com/LibreNZ/libre-fastapi-jwt Description-Content-
 Type: text/markdown
 ****** FastAPI JWT Auth ******
 [![Tests](https://github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/
-tests.yml/badge.svg?branch=master)](https://github.com/LibreNZ/libre-fastapi-
-jwt/actions/workflows/tests.yml) [![CodeQL](https://github.com/LibreNZ/libre-
-fastapi-jwt/actions/workflows/codeql.yml/badge.svg?branch=master)](https://
+tests.yml/badge.svg?branch=main)](https://github.com/LibreNZ/libre-fastapi-jwt/
+actions/workflows/tests.yml) [![CodeQL](https://github.com/LibreNZ/libre-
+fastapi-jwt/actions/workflows/codeql.yml/badge.svg?branch=main)](https://
 github.com/LibreNZ/libre-fastapi-jwt/actions/workflows/codeql.yml) [![PyPI
 version](https://badge.fury.io/py/libre-fastapi-jwt.svg)](https://
 badge.fury.io/py/libre-fastapi-jwt) [![Downloads](https://static.pepy.tech/
 personalized-badge/libre-fastapi-
 jwt?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)]
 (https://pepy.tech/project/libre-fastapi-jwt) ---
 **** BTW - The project is based on Fastapi-jwt-auth that is no longer
```

