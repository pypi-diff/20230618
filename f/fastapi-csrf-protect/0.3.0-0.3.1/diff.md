# Comparing `tmp/fastapi-csrf-protect-0.3.0.tar.gz` & `tmp/fastapi-csrf-protect-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-csrf-protect-0.3.0.tar", max compression
+gzip compressed data, was "fastapi-csrf-protect-0.3.1.tar", max compression
```

## Comparing `fastapi-csrf-protect-0.3.0.tar` & `fastapi-csrf-protect-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1073 2022-05-16 14:56:34.276540 fastapi-csrf-protect-0.3.0/LICENSE
--rw-r--r--   0        0        0     3647 2023-05-23 13:37:59.268734 fastapi-csrf-protect-0.3.0/README.md
--rw-r--r--   0        0        0      443 2023-05-23 14:09:10.000718 fastapi-csrf-protect-0.3.0/fastapi_csrf_protect/__init__.py
--rw-r--r--   0        0        0     6620 2023-05-23 14:09:10.000696 fastapi-csrf-protect-0.3.0/fastapi_csrf_protect/core.py
--rw-r--r--   0        0        0     1941 2023-05-23 14:09:10.000710 fastapi-csrf-protect-0.3.0/fastapi_csrf_protect/csrf_config.py
--rw-r--r--   0        0        0      825 2023-05-23 14:09:10.000832 fastapi-csrf-protect-0.3.0/fastapi_csrf_protect/exceptions.py
--rw-r--r--   0        0        0     1867 2023-05-23 14:09:10.000763 fastapi-csrf-protect-0.3.0/fastapi_csrf_protect/load_config.py
--rw-r--r--   0        0        0     1768 2023-05-23 14:09:05.224543 fastapi-csrf-protect-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4590 1970-01-01 00:00:00.000000 fastapi-csrf-protect-0.3.0/setup.py
--rw-r--r--   0        0        0     5245 1970-01-01 00:00:00.000000 fastapi-csrf-protect-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-05-16 14:56:34.276540 fastapi-csrf-protect-0.3.1/LICENSE
+-rw-r--r--   0        0        0     4524 2023-06-18 12:43:21.460103 fastapi-csrf-protect-0.3.1/README.md
+-rw-r--r--   0        0        0      443 2023-06-18 12:37:02.455348 fastapi-csrf-protect-0.3.1/fastapi_csrf_protect/__init__.py
+-rw-r--r--   0        0        0     7005 2023-06-18 12:37:02.446608 fastapi-csrf-protect-0.3.1/fastapi_csrf_protect/core.py
+-rw-r--r--   0        0        0     1941 2023-06-18 12:37:02.451374 fastapi-csrf-protect-0.3.1/fastapi_csrf_protect/csrf_config.py
+-rw-r--r--   0        0        0      825 2023-06-18 12:37:02.451249 fastapi-csrf-protect-0.3.1/fastapi_csrf_protect/exceptions.py
+-rw-r--r--   0        0        0     1867 2023-06-18 12:37:02.451264 fastapi-csrf-protect-0.3.1/fastapi_csrf_protect/load_config.py
+-rw-r--r--   0        0        0     1768 2023-06-18 12:37:02.419399 fastapi-csrf-protect-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5481 1970-01-01 00:00:00.000000 fastapi-csrf-protect-0.3.1/setup.py
+-rw-r--r--   0        0        0     6122 1970-01-01 00:00:00.000000 fastapi-csrf-protect-0.3.1/PKG-INFO
```

### Comparing `fastapi-csrf-protect-0.3.0/LICENSE` & `fastapi-csrf-protect-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-csrf-protect-0.3.0/README.md` & `fastapi-csrf-protect-0.3.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,24 @@
 FastAPI extension that provides stateless Cross-Site Request Forgery (XSRF) Protection support.
 Aimed to be easy to use and lightweight, we adopt [Double Submit Cookie](https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet.html#double-submit-cookie) mitigation pattern.
 If you were familiar with `flask-wtf` library this extension suitable for you.
 This extension inspired by `fastapi-jwt-auth` 😀
 
 - Storing `fastapi-csrf-token` in cookies or serve it in template's context
 
+## 🚧 Breaking Changes (0.3.0 -> 0.3.1)
+
+* The `generate_csrf` method has now been marked for deprecation
+* The recommended method is now `generate_csrf_tokens` which returns a tuple of tokens, first unsigned
+  and the latter signed
+* Recommended pattern is for the first token is aimed for returning as part of context
+* Recommended pattern is for the signed token to be set in client's cookie completing [Double Submit Cookie](https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet.html#double-submit-cookie)
+* To prevent token reuse, protected endpoint can unset the signed CSRF Token in client's cookies as
+  per example code and recommended pattern.
+
 ## Installation
 
 The easiest way to start working with this extension with pip
 
 ```bash
 pip install fastapi-csrf-protect
 # or
@@ -51,28 +61,30 @@
   return CsrfSettings()
 
 @app.get("/login")
 def form(request: Request, csrf_protect: CsrfProtect = Depends()):
   """
   Returns form template.
   """
-  csrf_token = csrf_protect.generate_csrf()
+  csrf_token, signed_token = csrf_protect.generate_csrf_tokens()
   response = templates.TemplateResponse(
     "form.html", {"request": request, "csrf_token": csrf_token}
   )
-  csrf_protect.set_csrf_cookie(csrf_token, response)
+  csrf_protect.set_csrf_cookie(signed_token, response)
   return response
 
 @app.post("/login", response_class=JSONResponse)
 def create_post(request: Request, csrf_protect: CsrfProtect = Depends()):
   """
   Creates a new Post
   """
   csrf_protect.validate_csrf(request)
-  # Do stuff
+  response: JSONResponse = JSONResponse(status_code=200, content={"detail": "OK"})
+  csrf_protect.unset_csrf_cookie(response)  # prevent token reuse
+  return response
 
 @app.exception_handler(CsrfProtectError)
 def csrf_protect_exception_handler(request: Request, exc: CsrfProtectError):
   return JSONResponse(status_code=exc.status_code, content={"detail": exc.message})
 
 ```
```

### Comparing `fastapi-csrf-protect-0.3.0/fastapi_csrf_protect/core.py` & `fastapi-csrf-protect-0.3.1/fastapi_csrf_protect/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,62 @@
 #!/usr/bin/env python3
 # Copyright (C) 2021-2023 All rights reserved.
 # FILENAME:  core.py
-# VERSION: 	 0.3.0
+# VERSION: 	 0.3.1
 # CREATED: 	 2020-11-25 14:35
 # AUTHOR: 	 Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
 import re
 from os import urandom
 from hashlib import sha1
-from typing import Optional
+from typing import Optional, Tuple
 from fastapi.requests import Request
 from fastapi.responses import Response
 from starlette.datastructures import Headers
 from itsdangerous import BadData, SignatureExpired, URLSafeTimedSerializer
 from fastapi_csrf_protect.csrf_config import CsrfConfig
 from fastapi_csrf_protect.exceptions import (
     InvalidHeaderError,
     MissingTokenError,
     TokenValidationError,
 )
+from warnings import warn
 
 
 class CsrfProtect(CsrfConfig):
-    def generate_csrf(self, secret_key: Optional[str] = None):
+    def generate_csrf(self, secret_key: Optional[str] = None) -> Tuple[str, str]:
         """
-        Generate a CSRF token.
-        TODO: The token should be cached for a request, so multiple
-        calls to this function will generate the same token.
+        Deprecated. Please use `generate_csrf_tokens` method instead.
 
         ---
-        :param secret_key: (Optional) the secret key used when generating a new token for users
-        :type secret_key: str
+        :param secret_key: (Optional) the secret key used when generating tokens for users
+        :type secret_key: (str | None) Defaults to None.
+        """
+        warn("This is deprecated; version=0.3.1", DeprecationWarning, stacklevel=2)
+        return self.generate_csrf_tokens(secret_key)
+
+    def generate_csrf_tokens(self, secret_key: Optional[str] = None) -> Tuple[str, str]:
+        """
+        Generate a CSRF token and a signed CSRF token using server's secret key to be stored in
+        cookie. R
+
+        ---
+        :param secret_key: (Optional) the secret key used when generating tokens for users
+        :type secret_key: (str | None) Defaults to None.
         """
         secret_key = secret_key or self._secret_key
         if secret_key is None:
             raise RuntimeError("A secret key is required to use CsrfProtect extension.")
         serializer = URLSafeTimedSerializer(secret_key, salt="fastapi-csrf-token")
-        token = serializer.dumps(sha1(urandom(64)).hexdigest())
-        return token
+        token = sha1(urandom(64)).hexdigest()
+        signed = serializer.dumps(token)
+        return token, signed
 
     def get_csrf_from_headers(self, headers: Headers) -> str:
         """
         Get token from the headers
 
         ---
         :param headers: Headers containing header with configured `header_name`
@@ -75,52 +87,47 @@
             ):
                 raise InvalidHeaderError(
                     f'Bad {header_name} header. Expected value "{header_type} <Token>"'
                 )
             token = header_parts[1]
         return token
 
-    def set_csrf_cookie(
-        self, csrf_token: Optional[str] = None, response: Optional[Response] = None
-    ) -> None:
+    def set_csrf_cookie(self, csrf_signed_token: str, response: Response) -> None:
         """
         Sets Csrf Protection token to the response cookies
 
         ---
-        :param csrf_token: (Optional) pre-determined token data
-        :type csrf_token: str
+        :param csrf_signed_token: signed CSRF token from `generate_csrf_token` method
+        :type csrf_signed_token: str
         :param response: The FastAPI response object to sets the access cookies in.
         :type response: fastapi.responses.Response
         """
-        csrf_token = csrf_token or self.generate_csrf(self._secret_key)
-        if response and not isinstance(response, Response):
+        if not isinstance(response, Response):
             raise TypeError("The response must be an object response FastAPI")
-        response = response or self._response
         response.set_cookie(
             self._cookie_key,
-            csrf_token,
+            csrf_signed_token,
             max_age=self._max_age,
             path=self._cookie_path,
             domain=self._cookie_domain,
             secure=self._cookie_secure,
             httponly=self._httponly,
             samesite=self._cookie_samesite,
         )
 
-    def unset_csrf_cookie(self, response: Optional[Response] = None) -> None:
+    def unset_csrf_cookie(self, response: Response) -> None:
         """
         Remove Csrf Protection token from the response cookies
 
         ---
-        :param response: (Optional) The FastAPI response object to delete the access cookies in.
+        :param response: The FastAPI response object to delete the access cookies in.
         :type response: fastapi.responses.Response
         """
-        if response and not isinstance(response, Response):
+        if not isinstance(response, Response):
             raise TypeError("The response must be an object response FastAPI")
-        response = response or self._response
         response.delete_cookie(
             self._cookie_key, path=self._cookie_path, domain=self._cookie_domain
         )
 
     def validate_csrf(
         self,
         request: Request,
@@ -146,21 +153,23 @@
         :type time_limit: int
         :raises TokenValidationError: Contains the reason that validation failed.
         """
         secret_key = secret_key or self._secret_key
         if secret_key is None:
             raise RuntimeError("A secret key is required to use CsrfProtect extension.")
         cookie_key = cookie_key or self._cookie_key
-        cookie_token = request.cookies.get(cookie_key)
-        if cookie_token is None:
+        signed_token = request.cookies.get(cookie_key)
+        if signed_token is None:
             raise MissingTokenError(f"Missing Cookie: `{cookie_key}`.")
         time_limit = time_limit or self._max_age
         token: str = self.get_csrf_from_headers(request.headers)
-        if token != cookie_token:
-            raise TokenValidationError("The CSRF token pair submitted do not match.")
         serializer = URLSafeTimedSerializer(secret_key, salt="fastapi-csrf-token")
         try:
-            serializer.loads(token, max_age=time_limit)
+            signature: str = serializer.loads(signed_token, max_age=time_limit)
+            if token != signature:
+                raise TokenValidationError(
+                    "The CSRF signatures submitted do not match."
+                )
         except SignatureExpired:
             raise TokenValidationError("The CSRF token has expired.")
         except BadData:
             raise TokenValidationError("The CSRF token is invalid.")
```

### Comparing `fastapi-csrf-protect-0.3.0/fastapi_csrf_protect/csrf_config.py` & `fastapi-csrf-protect-0.3.1/fastapi_csrf_protect/csrf_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # Copyright (C) 2021-2023 All rights reserved.
 # FILENAME:  fastapi_csrf_config.py
-# VERSION: 	 0.3.0
+# VERSION: 	 0.3.1
 # CREATED: 	 2020-11-25 14:35
 # AUTHOR: 	 Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
 ### Standard Packages ###
```

### Comparing `fastapi-csrf-protect-0.3.0/fastapi_csrf_protect/exceptions.py` & `fastapi-csrf-protect-0.3.1/fastapi_csrf_protect/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # Copyright (C) 2021-2023 All rights reserved.
 # FILENAME:  exceptions.py
-# VERSION: 	 0.3.0
+# VERSION: 	 0.3.1
 # CREATED: 	 2020-11-25 14:35
 # AUTHOR: 	 Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
 class CsrfProtectError(Exception):
```

### Comparing `fastapi-csrf-protect-0.3.0/fastapi_csrf_protect/load_config.py` & `fastapi-csrf-protect-0.3.1/fastapi_csrf_protect/load_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # Copyright (C) 2021-2023 All rights reserved.
 # FILENAME:  load_config.py
-# VERSION: 	 0.3.0
+# VERSION: 	 0.3.1
 # CREATED: 	 2020-11-25 14:35
 # AUTHOR: 	 Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
 from typing import Optional, Sequence
```

### Comparing `fastapi-csrf-protect-0.3.0/pyproject.toml` & `fastapi-csrf-protect-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-csrf-protect"
-version = "0.3.0"
+version = "0.3.1"
 description = "Stateless implementation of Cross-Site Request Forgery (XSRF) Protection by using Double Submit Cookie mitigation pattern"
 authors = ["Sitt Guruvanich <aekazitt@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/aekasitt/fastapi-csrf-protect"
 repository = "https://github.com/aekasitt/fastapi-csrf-protect"
 keywords = ["starlette", "fastapi", "csrf", "xsrf", "cross-site request forgery", "samesite", "asynchronous"]
```

### Comparing `fastapi-csrf-protect-0.3.0/setup.py` & `fastapi-csrf-protect-0.3.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['fastapi>=0,<1', 'itsdangerous>=2.0.1,<3.0.0', 'pydantic>=1.7.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'fastapi-csrf-protect',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Stateless implementation of Cross-Site Request Forgery (XSRF) Protection by using Double Submit Cookie mitigation pattern',
-    'long_description': '# FastAPI CSRF Protect\n\n[![Build Status](https://travis-ci.com/aekasitt/fastapi-csrf-protect.svg?branch=master)](https://app.travis-ci.com/github/aekasitt/fastapi-csrf-protect)\n[![Package Vesion](https://img.shields.io/pypi/v/fastapi-csrf-protect)](https://pypi.org/project/fastapi-csrf-protect)\n[![Format](https://img.shields.io/pypi/format/fastapi-csrf-protect)](https://pypi.org/project/fastapi-csrf-protect)\n[![Python Version](https://img.shields.io/pypi/pyversions/fastapi-csrf-protect)](https://pypi.org/project/fastapi-csrf-protect)\n[![License](https://img.shields.io/pypi/l/fastapi-csrf-protect)](https://pypi.org/project/fastapi-csrf-protect)\n\n## Features\n\nFastAPI extension that provides stateless Cross-Site Request Forgery (XSRF) Protection support.\nAimed to be easy to use and lightweight, we adopt [Double Submit Cookie](https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet.html#double-submit-cookie) mitigation pattern.\nIf you were familiar with `flask-wtf` library this extension suitable for you.\nThis extension inspired by `fastapi-jwt-auth` 😀\n\n- Storing `fastapi-csrf-token` in cookies or serve it in template\'s context\n\n## Installation\n\nThe easiest way to start working with this extension with pip\n\n```bash\npip install fastapi-csrf-protect\n# or\npoetry add fastapi-csrf-protect\n```\n\n## Getting Started\n\nThe following examples show you how to integrate this extension to a FastAPI App\n\n### Example Login Form\n\n```python\nfrom fastapi import FastAPI, Request, Depends\nfrom fastapi.responses import JSONResponse\nfrom fastapi.templating import Jinja2Templates\nfrom fastapi_csrf_protect import CsrfProtect\nfrom fastapi_csrf_protect.exceptions import CsrfProtectError\nfrom pydantic import BaseModel\n\napp = FastAPI()\ntemplates = Jinja2Templates(directory="templates")\n\nclass CsrfSettings(BaseModel):\n  secret_key: str = "asecrettoeverybody"\n  cookie_samesite: str = "none"\n\n@CsrfProtect.load_config\ndef get_csrf_config():\n  return CsrfSettings()\n\n@app.get("/login")\ndef form(request: Request, csrf_protect: CsrfProtect = Depends()):\n  """\n  Returns form template.\n  """\n  csrf_token = csrf_protect.generate_csrf()\n  response = templates.TemplateResponse(\n    "form.html", {"request": request, "csrf_token": csrf_token}\n  )\n  csrf_protect.set_csrf_cookie(csrf_token, response)\n  return response\n\n@app.post("/login", response_class=JSONResponse)\ndef create_post(request: Request, csrf_protect: CsrfProtect = Depends()):\n  """\n  Creates a new Post\n  """\n  csrf_protect.validate_csrf(request)\n  # Do stuff\n\n@app.exception_handler(CsrfProtectError)\ndef csrf_protect_exception_handler(request: Request, exc: CsrfProtectError):\n  return JSONResponse(status_code=exc.status_code, content={"detail": exc.message})\n\n```\n\n## Contributions\n\nTo contribute to the project, fork the repository and clone to your local device and install preferred testing dependency [pytest](https://github.com/pytest-dev/pytest)\nAlternatively, run the following command on your terminal to do so:\n\n```bash\npip install -U poetry\npoetry install\n```\n\nTesting can be done by the following command post-installation:\n\n```bash\npoetry install --with test\npytest\n```\n\n### Run Examples\n\nTo run the provided examples, first you must install extra dependencies [uvicorn](https://github.com/encode/uvicorn) and [jinja2](https://github.com/pallets/jinja/)\nAlternatively, run the following command on your terminal to do so\n\n```bash\npoetry install --with examples\n```\n\nRunning the example utilizing Context and Headers\n\n```bash\nuvicorn examples.login:app\n```\n\n## License\n\nThis project is licensed under the terms of the MIT license.\n',
+    'long_description': '# FastAPI CSRF Protect\n\n[![Build Status](https://travis-ci.com/aekasitt/fastapi-csrf-protect.svg?branch=master)](https://app.travis-ci.com/github/aekasitt/fastapi-csrf-protect)\n[![Package Vesion](https://img.shields.io/pypi/v/fastapi-csrf-protect)](https://pypi.org/project/fastapi-csrf-protect)\n[![Format](https://img.shields.io/pypi/format/fastapi-csrf-protect)](https://pypi.org/project/fastapi-csrf-protect)\n[![Python Version](https://img.shields.io/pypi/pyversions/fastapi-csrf-protect)](https://pypi.org/project/fastapi-csrf-protect)\n[![License](https://img.shields.io/pypi/l/fastapi-csrf-protect)](https://pypi.org/project/fastapi-csrf-protect)\n\n## Features\n\nFastAPI extension that provides stateless Cross-Site Request Forgery (XSRF) Protection support.\nAimed to be easy to use and lightweight, we adopt [Double Submit Cookie](https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet.html#double-submit-cookie) mitigation pattern.\nIf you were familiar with `flask-wtf` library this extension suitable for you.\nThis extension inspired by `fastapi-jwt-auth` 😀\n\n- Storing `fastapi-csrf-token` in cookies or serve it in template\'s context\n\n## 🚧 Breaking Changes (0.3.0 -> 0.3.1)\n\n* The `generate_csrf` method has now been marked for deprecation\n* The recommended method is now `generate_csrf_tokens` which returns a tuple of tokens, first unsigned\n  and the latter signed\n* Recommended pattern is for the first token is aimed for returning as part of context\n* Recommended pattern is for the signed token to be set in client\'s cookie completing [Double Submit Cookie](https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet.html#double-submit-cookie)\n* To prevent token reuse, protected endpoint can unset the signed CSRF Token in client\'s cookies as\n  per example code and recommended pattern.\n\n## Installation\n\nThe easiest way to start working with this extension with pip\n\n```bash\npip install fastapi-csrf-protect\n# or\npoetry add fastapi-csrf-protect\n```\n\n## Getting Started\n\nThe following examples show you how to integrate this extension to a FastAPI App\n\n### Example Login Form\n\n```python\nfrom fastapi import FastAPI, Request, Depends\nfrom fastapi.responses import JSONResponse\nfrom fastapi.templating import Jinja2Templates\nfrom fastapi_csrf_protect import CsrfProtect\nfrom fastapi_csrf_protect.exceptions import CsrfProtectError\nfrom pydantic import BaseModel\n\napp = FastAPI()\ntemplates = Jinja2Templates(directory="templates")\n\nclass CsrfSettings(BaseModel):\n  secret_key: str = "asecrettoeverybody"\n  cookie_samesite: str = "none"\n\n@CsrfProtect.load_config\ndef get_csrf_config():\n  return CsrfSettings()\n\n@app.get("/login")\ndef form(request: Request, csrf_protect: CsrfProtect = Depends()):\n  """\n  Returns form template.\n  """\n  csrf_token, signed_token = csrf_protect.generate_csrf_tokens()\n  response = templates.TemplateResponse(\n    "form.html", {"request": request, "csrf_token": csrf_token}\n  )\n  csrf_protect.set_csrf_cookie(signed_token, response)\n  return response\n\n@app.post("/login", response_class=JSONResponse)\ndef create_post(request: Request, csrf_protect: CsrfProtect = Depends()):\n  """\n  Creates a new Post\n  """\n  csrf_protect.validate_csrf(request)\n  response: JSONResponse = JSONResponse(status_code=200, content={"detail": "OK"})\n  csrf_protect.unset_csrf_cookie(response)  # prevent token reuse\n  return response\n\n@app.exception_handler(CsrfProtectError)\ndef csrf_protect_exception_handler(request: Request, exc: CsrfProtectError):\n  return JSONResponse(status_code=exc.status_code, content={"detail": exc.message})\n\n```\n\n## Contributions\n\nTo contribute to the project, fork the repository and clone to your local device and install preferred testing dependency [pytest](https://github.com/pytest-dev/pytest)\nAlternatively, run the following command on your terminal to do so:\n\n```bash\npip install -U poetry\npoetry install\n```\n\nTesting can be done by the following command post-installation:\n\n```bash\npoetry install --with test\npytest\n```\n\n### Run Examples\n\nTo run the provided examples, first you must install extra dependencies [uvicorn](https://github.com/encode/uvicorn) and [jinja2](https://github.com/pallets/jinja/)\nAlternatively, run the following command on your terminal to do so\n\n```bash\npoetry install --with examples\n```\n\nRunning the example utilizing Context and Headers\n\n```bash\nuvicorn examples.login:app\n```\n\n## License\n\nThis project is licensed under the terms of the MIT license.\n',
     'author': 'Sitt Guruvanich',
     'author_email': 'aekazitt@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/aekasitt/fastapi-csrf-protect',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `fastapi-csrf-protect-0.3.0/PKG-INFO` & `fastapi-csrf-protect-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-csrf-protect
-Version: 0.3.0
+Version: 0.3.1
 Summary: Stateless implementation of Cross-Site Request Forgery (XSRF) Protection by using Double Submit Cookie mitigation pattern
 Home-page: https://github.com/aekasitt/fastapi-csrf-protect
 License: MIT
 Keywords: starlette,fastapi,csrf,xsrf,cross-site request forgery,samesite,asynchronous
 Author: Sitt Guruvanich
 Author-email: aekazitt@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -45,14 +45,24 @@
 FastAPI extension that provides stateless Cross-Site Request Forgery (XSRF) Protection support.
 Aimed to be easy to use and lightweight, we adopt [Double Submit Cookie](https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet.html#double-submit-cookie) mitigation pattern.
 If you were familiar with `flask-wtf` library this extension suitable for you.
 This extension inspired by `fastapi-jwt-auth` 😀
 
 - Storing `fastapi-csrf-token` in cookies or serve it in template's context
 
+## 🚧 Breaking Changes (0.3.0 -> 0.3.1)
+
+* The `generate_csrf` method has now been marked for deprecation
+* The recommended method is now `generate_csrf_tokens` which returns a tuple of tokens, first unsigned
+  and the latter signed
+* Recommended pattern is for the first token is aimed for returning as part of context
+* Recommended pattern is for the signed token to be set in client's cookie completing [Double Submit Cookie](https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet.html#double-submit-cookie)
+* To prevent token reuse, protected endpoint can unset the signed CSRF Token in client's cookies as
+  per example code and recommended pattern.
+
 ## Installation
 
 The easiest way to start working with this extension with pip
 
 ```bash
 pip install fastapi-csrf-protect
 # or
@@ -85,28 +95,30 @@
   return CsrfSettings()
 
 @app.get("/login")
 def form(request: Request, csrf_protect: CsrfProtect = Depends()):
   """
   Returns form template.
   """
-  csrf_token = csrf_protect.generate_csrf()
+  csrf_token, signed_token = csrf_protect.generate_csrf_tokens()
   response = templates.TemplateResponse(
     "form.html", {"request": request, "csrf_token": csrf_token}
   )
-  csrf_protect.set_csrf_cookie(csrf_token, response)
+  csrf_protect.set_csrf_cookie(signed_token, response)
   return response
 
 @app.post("/login", response_class=JSONResponse)
 def create_post(request: Request, csrf_protect: CsrfProtect = Depends()):
   """
   Creates a new Post
   """
   csrf_protect.validate_csrf(request)
-  # Do stuff
+  response: JSONResponse = JSONResponse(status_code=200, content={"detail": "OK"})
+  csrf_protect.unset_csrf_cookie(response)  # prevent token reuse
+  return response
 
 @app.exception_handler(CsrfProtectError)
 def csrf_protect_exception_handler(request: Request, exc: CsrfProtectError):
   return JSONResponse(status_code=exc.status_code, content={"detail": exc.message})
 
 ```
```

