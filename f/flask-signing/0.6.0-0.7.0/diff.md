# Comparing `tmp/flask_signing-0.6.0.tar.gz` & `tmp/flask_signing-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_signing-0.6.0.tar", last modified: Sat Jun 17 03:24:13 2023, max compression
+gzip compressed data, was "flask_signing-0.7.0.tar", last modified: Sun Jun 18 03:34:06 2023, max compression
```

## Comparing `flask_signing-0.6.0.tar` & `flask_signing-0.7.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-17 03:24:13.901771 flask_signing-0.6.0/
--rw-rw-r--   0 sig       (1000) sig       (1000)     1503 2023-06-11 20:13:39.000000 flask_signing-0.6.0/LICENSE
--rw-rw-r--   0 sig       (1000) sig       (1000)       43 2023-06-15 20:25:19.000000 flask_signing-0.6.0/MANIFEST.in
--rw-rw-r--   0 sig       (1000) sig       (1000)     3870 2023-06-17 03:24:13.901771 flask_signing-0.6.0/PKG-INFO
--rw-rw-r--   0 sig       (1000) sig       (1000)     3138 2023-06-17 03:12:27.000000 flask_signing-0.6.0/README.md
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-17 03:24:13.901771 flask_signing-0.6.0/docs/
--rw-rw-r--   0 sig       (1000) sig       (1000)    78889 2023-06-13 00:10:22.000000 flask_signing-0.6.0/docs/combined.png
--rw-rw-r--   0 sig       (1000) sig       (1000)    65777 2023-06-13 00:01:06.000000 flask_signing-0.6.0/docs/logo.png
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-17 03:24:13.901771 flask_signing-0.6.0/flask_signing/
--rw-rw-r--   0 sig       (1000) sig       (1000)    20649 2023-06-17 03:12:34.000000 flask_signing-0.6.0/flask_signing/__init__.py
--rw-rw-r--   0 sig       (1000) sig       (1000)      213 2023-06-17 03:23:40.000000 flask_signing-0.6.0/flask_signing/__metadata__.py
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-17 03:24:13.901771 flask_signing-0.6.0/flask_signing.egg-info/
--rw-rw-r--   0 sig       (1000) sig       (1000)     3870 2023-06-17 03:24:13.000000 flask_signing-0.6.0/flask_signing.egg-info/PKG-INFO
--rw-rw-r--   0 sig       (1000) sig       (1000)      372 2023-06-17 03:24:13.000000 flask_signing-0.6.0/flask_signing.egg-info/SOURCES.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)        1 2023-06-17 03:24:13.000000 flask_signing-0.6.0/flask_signing.egg-info/dependency_links.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       35 2023-06-17 03:24:13.000000 flask_signing-0.6.0/flask_signing.egg-info/requires.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       20 2023-06-17 03:24:13.000000 flask_signing-0.6.0/flask_signing.egg-info/top_level.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       35 2023-06-11 20:04:40.000000 flask_signing-0.6.0/requirements.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       38 2023-06-17 03:24:13.901771 flask_signing-0.6.0/setup.cfg
--rw-rw-r--   0 sig       (1000) sig       (1000)     1587 2023-06-15 20:26:56.000000 flask_signing-0.6.0/setup.py
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-17 03:24:13.901771 flask_signing-0.6.0/tests/
--rw-rw-r--   0 sig       (1000) sig       (1000)    10843 2023-06-17 02:47:54.000000 flask_signing-0.6.0/tests/__init__.py
--rw-rw-r--   0 sig       (1000) sig       (1000)     7995 2023-06-17 03:12:37.000000 flask_signing-0.6.0/tests/performance_tests.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-18 03:34:06.897492 flask_signing-0.7.0/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     1503 2023-06-11 20:13:39.000000 flask_signing-0.7.0/LICENSE
+-rw-rw-r--   0 sig       (1000) sig       (1000)       43 2023-06-15 20:25:19.000000 flask_signing-0.7.0/MANIFEST.in
+-rw-rw-r--   0 sig       (1000) sig       (1000)     4232 2023-06-18 03:34:06.897492 flask_signing-0.7.0/PKG-INFO
+-rw-rw-r--   0 sig       (1000) sig       (1000)     3500 2023-06-17 23:58:12.000000 flask_signing-0.7.0/README.md
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-18 03:34:06.893492 flask_signing-0.7.0/docs/
+-rw-rw-r--   0 sig       (1000) sig       (1000)    78889 2023-06-13 00:10:22.000000 flask_signing-0.7.0/docs/combined.png
+-rw-rw-r--   0 sig       (1000) sig       (1000)    65777 2023-06-13 00:01:06.000000 flask_signing-0.7.0/docs/logo.png
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-18 03:34:06.893492 flask_signing-0.7.0/flask_signing/
+-rw-rw-r--   0 sig       (1000) sig       (1000)    24748 2023-06-18 03:24:58.000000 flask_signing-0.7.0/flask_signing/__init__.py
+-rw-rw-r--   0 sig       (1000) sig       (1000)      213 2023-06-18 03:31:30.000000 flask_signing-0.7.0/flask_signing/__metadata__.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-18 03:34:06.897492 flask_signing-0.7.0/flask_signing.egg-info/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     4232 2023-06-18 03:34:06.000000 flask_signing-0.7.0/flask_signing.egg-info/PKG-INFO
+-rw-rw-r--   0 sig       (1000) sig       (1000)      372 2023-06-18 03:34:06.000000 flask_signing-0.7.0/flask_signing.egg-info/SOURCES.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)        1 2023-06-18 03:34:06.000000 flask_signing-0.7.0/flask_signing.egg-info/dependency_links.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       35 2023-06-18 03:34:06.000000 flask_signing-0.7.0/flask_signing.egg-info/requires.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       20 2023-06-18 03:34:06.000000 flask_signing-0.7.0/flask_signing.egg-info/top_level.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       35 2023-06-11 20:04:40.000000 flask_signing-0.7.0/requirements.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       38 2023-06-18 03:34:06.897492 flask_signing-0.7.0/setup.cfg
+-rw-rw-r--   0 sig       (1000) sig       (1000)     1587 2023-06-15 20:26:56.000000 flask_signing-0.7.0/setup.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-18 03:34:06.897492 flask_signing-0.7.0/tests/
+-rw-rw-r--   0 sig       (1000) sig       (1000)    12354 2023-06-18 03:24:43.000000 flask_signing-0.7.0/tests/__init__.py
+-rw-rw-r--   0 sig       (1000) sig       (1000)     7995 2023-06-17 03:12:37.000000 flask_signing-0.7.0/tests/performance_tests.py
```

### Comparing `flask_signing-0.6.0/LICENSE` & `flask_signing-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_signing-0.6.0/PKG-INFO` & `flask_signing-0.7.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_signing
-Version: 0.6.0
+Version: 0.7.0
 Summary: a signing key extension for flask
 Home-page: https://github.com/signebedi/Flask-Signing
 Author: Sig Janoska-Bedi
 Author-email: signe@atreeus.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -21,14 +21,15 @@
 
 ## Flask-Signing
 
 [![License: BSD-3-Clause](https://img.shields.io/github/license/signebedi/Flask-Signing?color=dark-green)](https://github.com/signebedi/Flask-Signing/blob/master/LICENSE) 
 [![PyPI version](https://badge.fury.io/py/Flask-Signing.svg)](https://pypi.org/project/flask-signing/)
 [![Downloads](https://static.pepy.tech/personalized-badge/flask-signing?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/flask-signing)
 [![Flask-Signing tests](https://github.com/signebedi/Flask-Signing/workflows/tests/badge.svg)](https://github.com/signebedi/Flask-Signing/actions)
+[![Buy me a coffee](https://img.shields.io/badge/Buy%20me%20a%20coffee--brightgreen.svg?logo=buy-me-a-coffee&logoColor=brightgreen)](https://www.buymeacoffee.com/signebedi)
 
 a signing key extension for flask
 
 
 ### About
 
 The Flask-Signing library is a useful tool for Flask applications that require secure and robust management of signing keys. Do you need to generate single-use tokens for one-time actions like email verification or password reset? Flask-Signing can handle that. Are you looking for a simple method for managing API keys? Look no further. 
@@ -37,17 +38,17 @@
 
 First, install the flask_signing package. You can do this with pip:
 
 ```bash
 pip install flask_signing
 ```
 
-### Usage
+### Basic Usage
 
-After you've installed the package, you can use it in your Flask application. Here's an example of how you might do this:
+After you've installed the flask_signing package, you can use it in your Flask application. Here's an example of how you might do this:
 
 ```python
 from flask import Flask
 from flask_sqlalchemy import SQLAlchemy
 from flask_signing import Signatures
 
 app = Flask(__name__)
@@ -75,14 +76,14 @@
     
 @app.route('/all')
 def all():
     all = signatures.get_all()
     return f'Response: {all}'
 ```
 
-In this example, a new signing key is generated and written to the database when you visit the /sign route, and the key is displayed on the page. Then, when you visit the /verify/<key> route (replace <key> with the actual key), the validity of the key is checked and displayed. You can expire a key using the /expire/<key> route, and view all records with the /all route.
+In this basic example, a new signing key is generated and written to the database when you visit the `/sign` route, and the key is displayed on the page. Then, when you visit the `/verify/<key>` route (replace <key> with the actual key), the validity of the key is checked and displayed. You can expire a key using the `/expire/<key>` route, and view all records with the `/all` route.
 
-Please note that this is a very basic example and your actual use of the flask_signing package may be more complex depending on your needs. It's important to secure your signing keys and handle them appropriately according to your application's security requirements.
+This is a rather basic example and your actual use of the flask_signing package may be more complex depending on your needs. It's important to secure your signing keys and handle them appropriately according to your application's security requirements. Further usage examples can be found in the [examples](https://github.com/signebedi/Flask-Signing/tree/master/examples) directory of the Flask-Signing Github repository. 
 
 ### Developers
 
 Contributions are welcome! You can read the developer docs at https://signebedi.github.io/Flask-Signing. If you're interested, review (or add to) the feature ideas at https://github.com/signebedi/Flask-Signing/issues.
```

### Comparing `flask_signing-0.6.0/README.md` & `flask_signing-0.7.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 ## Flask-Signing
 
 [![License: BSD-3-Clause](https://img.shields.io/github/license/signebedi/Flask-Signing?color=dark-green)](https://github.com/signebedi/Flask-Signing/blob/master/LICENSE) 
 [![PyPI version](https://badge.fury.io/py/Flask-Signing.svg)](https://pypi.org/project/flask-signing/)
 [![Downloads](https://static.pepy.tech/personalized-badge/flask-signing?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/flask-signing)
 [![Flask-Signing tests](https://github.com/signebedi/Flask-Signing/workflows/tests/badge.svg)](https://github.com/signebedi/Flask-Signing/actions)
+[![Buy me a coffee](https://img.shields.io/badge/Buy%20me%20a%20coffee--brightgreen.svg?logo=buy-me-a-coffee&logoColor=brightgreen)](https://www.buymeacoffee.com/signebedi)
 
 a signing key extension for flask
 
 
 ### About
 
 The Flask-Signing library is a useful tool for Flask applications that require secure and robust management of signing keys. Do you need to generate single-use tokens for one-time actions like email verification or password reset? Flask-Signing can handle that. Are you looking for a simple method for managing API keys? Look no further. 
@@ -18,17 +19,17 @@
 
 First, install the flask_signing package. You can do this with pip:
 
 ```bash
 pip install flask_signing
 ```
 
-### Usage
+### Basic Usage
 
-After you've installed the package, you can use it in your Flask application. Here's an example of how you might do this:
+After you've installed the flask_signing package, you can use it in your Flask application. Here's an example of how you might do this:
 
 ```python
 from flask import Flask
 from flask_sqlalchemy import SQLAlchemy
 from flask_signing import Signatures
 
 app = Flask(__name__)
@@ -56,14 +57,14 @@
     
 @app.route('/all')
 def all():
     all = signatures.get_all()
     return f'Response: {all}'
 ```
 
-In this example, a new signing key is generated and written to the database when you visit the /sign route, and the key is displayed on the page. Then, when you visit the /verify/<key> route (replace <key> with the actual key), the validity of the key is checked and displayed. You can expire a key using the /expire/<key> route, and view all records with the /all route.
+In this basic example, a new signing key is generated and written to the database when you visit the `/sign` route, and the key is displayed on the page. Then, when you visit the `/verify/<key>` route (replace <key> with the actual key), the validity of the key is checked and displayed. You can expire a key using the `/expire/<key>` route, and view all records with the `/all` route.
 
-Please note that this is a very basic example and your actual use of the flask_signing package may be more complex depending on your needs. It's important to secure your signing keys and handle them appropriately according to your application's security requirements.
+This is a rather basic example and your actual use of the flask_signing package may be more complex depending on your needs. It's important to secure your signing keys and handle them appropriately according to your application's security requirements. Further usage examples can be found in the [examples](https://github.com/signebedi/Flask-Signing/tree/master/examples) directory of the Flask-Signing Github repository. 
 
 ### Developers
 
 Contributions are welcome! You can read the developer docs at https://signebedi.github.io/Flask-Signing. If you're interested, review (or add to) the feature ideas at https://github.com/signebedi/Flask-Signing/issues.
```

### Comparing `flask_signing-0.6.0/docs/combined.png` & `flask_signing-0.7.0/docs/combined.png`

 * *Files identical despite different names*

### Comparing `flask_signing-0.6.0/docs/logo.png` & `flask_signing-0.7.0/docs/logo.png`

 * *Files identical despite different names*

### Comparing `flask_signing-0.6.0/flask_signing/__init__.py` & `flask_signing-0.7.0/flask_signing/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,16 @@
                        __license__, __maintainer__, __email__)
 import datetime, secrets
 from functools import wraps
 from sqlalchemy import func, literal
 from sqlalchemy.exc import SQLAlchemyError
 from flask_sqlalchemy import SQLAlchemy
 from typing import Union, List, Dict, Any
+from itsdangerous import URLSafeTimedSerializer
+
 
 class RateLimitExceeded(Exception):
     """
     An exception that is raised when the request count for a specific signature 
     exceeds the maximum allowed requests within a specified time period in the 
     Signatures class.
 
@@ -21,30 +23,34 @@
 
 class Signatures:
     """
     The Signatures class handles operations related to the creation, management, and validation 
     of signing keys in the database.
     """
     
-    def __init__(self, app, safe_mode:bool=True, byte_len:int=24, rate_limiting=False, rate_limiting_max_requests=10, rate_limiting_period=datetime.timedelta(minutes=1)):
+    def __init__(self, app, db=None, safe_mode:bool=True, byte_len:int=24, rate_limiting=False, rate_limiting_max_requests=10, rate_limiting_period=datetime.timedelta(minutes=1)):
         """
         Initializes a new instance of the Signatures class.
 
         Args:
             app (Flask): A flask object to contain the context for database interactions. 
+            db (SQLAlchemy, optional): An optional SQLAlchemy db object to inherit an app's existing data model. Defaults to False.
             safe_mode (bool, optional): If safe_mode is enabled, we will prevent rotation of disabled or rotated keys. Defaults to True.
             byte_len (int, optional): The length of the generated signing keys. Defaults to 24.
             rate_limiting (bool, optional): If rate_limiting is enabled, we will impose key-by-key rate limits. Defaults to False.
             rate_limiting_max_requests (int, optional): Maximum allowed requests per time period.
             rate_limiting_period (datetime.timedelta, optional): Time period for rate limiting. Defaults to 1 hour.
         """
-
-        self.db = SQLAlchemy(app)
-        self.Signing = self.get_model()
-        self.db.create_all()  # this will create all necessary tables
+        if db is not None:
+            self.db = db
+            self.Signing = self.get_model()
+        else:
+            self.db = SQLAlchemy(app)
+            self.Signing = self.get_model()
+            self.db.create_all()  # this will create all necessary tables
 
         self.byte_len = byte_len
 
         # Set safe mode to prevent disabled/rotated keys from being rotated
         self.safe_mode = safe_mode
 
         # Set rate limiting attributes
@@ -284,17 +290,15 @@
         #     return False
 
         return True
 
     def get_model(self):
 
         """
-        Generate an instance of the Signing class, which represents the Signing table in the database.
-
-        Each instance of this class represents a row of data in the database table.
+        Return a single instance of the Signing class, which represents the Signing table in the database.
 
         Attributes:
             signature (str): The primary key of the Signing table. This field is unique for each entry.
             email (str): The email associated with a specific signing key.
             scope (str): The scope within which the key is valid.
             active (bool): The status of the signing key. If True, the key is active.
             timestamp (datetime): The date and time when the signing key was created.
@@ -492,8 +496,113 @@
             # print(f"An error occurred while rotating the key {key}: {e}")
             return False
 
         except Exception as e:
             # print(f"An unexpected error occurred: {e}")
             return False
 
-        return new_key
+        return new_key
+
+
+class DangerousSignatures(Signatures):
+
+    """
+    The DangerousSignatures class handles operations related to the creation, management, 
+    and validation of signing keys in the database using the itsdangerous library.
+    """
+    
+    def __init__(self, app, secret_key:str=None, salt:str=None, *args, **kwargs):
+        """
+        Initializes a new instance of the DangerousSignatures class.
+
+        Args:
+            app (Flask): A flask object to contain the context for database interactions. 
+            secret_key (str, optional): Value to use as a secret key. Defaults to the app.secret_key.
+            salt (str, optional): Value to use as the salt. Defaults to flask-signing.
+
+        """
+        self.app = app
+        super().__init__(self.app, *args, **kwargs)
+        
+        self.secret_key = secret_key or self.app.secret_key
+        self.salt = salt or 'flask-signing'
+        self.serializer = URLSafeTimedSerializer(self.secret_key)
+
+
+    def generate_key(self, additional_data: dict = None, length:int=None) -> str:
+        """
+        Overrides the parent generate_key method to use itsdangerous for key generation.
+
+        Args:
+            additional_data (dict, optional): Additional data to be included in the token. Defaults to None.
+            length (int, optional): The length of the generated signing key. Defaults to None, in which case the byte_len is used.
+
+        Returns:
+            str: The generated signing key.
+        """
+        if not length: 
+            length = self.byte_len
+
+        data = {"key": secrets.token_urlsafe(length)}
+
+        # If additional_data is provided, update the data dictionary
+        if additional_data is not None:
+            data.update(additional_data)
+
+        return self.serializer.dumps(data)
+
+    # def check_key(self, signature, scope):
+    #     """
+    #     Checks the validity of a given signing key against a specific scope.
+
+    #     This function checks if the signing key exists, if it is active, if it has not expired,
+    #     and if its scope matches the provided scope. If all these conditions are met, the function
+    #     returns True, otherwise, it returns False.
+
+    #     Args:
+    #         signature (str): The signing key to be verified.
+    #         scope (str): The scope against which the signing key will be validated.
+
+    #     Returns:
+    #         bool: True if the signing key is valid and False otherwise.
+    #     """
+
+    #     Signing = self.get_model()
+
+    #     # try to decode the signature using the serializer
+    #     try:
+    #         data = self.serializer.loads(signature)
+
+    #         # if the signature doesn't contain a key, it's invalid
+    #         if "key" not in data:
+    #             return False
+
+    #         signing_key = Signing.query.filter_by(signature=data["key"]).first()
+
+    #     except (itsdangerous.BadSignature, itsdangerous.SignatureExpired):
+    #         return False  # if the signature cannot be decoded or is expired, it's invalid
+    #     except Exception as e:
+    #         print(f"Unexpected error while decoding signature: {e}")
+    #         return False
+
+    #     # if the key doesn't exist
+    #     if not signing_key:
+    #         return False
+
+    #     # if the signing key's expiration time has passed
+    #     if signing_key.expiration < datetime.datetime.utcnow():
+    #         self.expire_key(data["key"])
+    #         return False
+
+    #     # if the signing key is set to inactive
+    #     if not signing_key.active:
+    #         return False
+
+    #     # Convert scope to a list if it's a string
+    #     if isinstance(scope, str):
+    #         scope = [scope]
+
+    #     # if the signing key's scope doesn't match any of the required scopes
+    #     if not set(scope).intersection(set(signing_key.scope)):
+    #         return False
+
+    #     return True
```

### Comparing `flask_signing-0.6.0/flask_signing.egg-info/PKG-INFO` & `flask_signing-0.7.0/flask_signing.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-signing
-Version: 0.6.0
+Version: 0.7.0
 Summary: a signing key extension for flask
 Home-page: https://github.com/signebedi/Flask-Signing
 Author: Sig Janoska-Bedi
 Author-email: signe@atreeus.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -21,14 +21,15 @@
 
 ## Flask-Signing
 
 [![License: BSD-3-Clause](https://img.shields.io/github/license/signebedi/Flask-Signing?color=dark-green)](https://github.com/signebedi/Flask-Signing/blob/master/LICENSE) 
 [![PyPI version](https://badge.fury.io/py/Flask-Signing.svg)](https://pypi.org/project/flask-signing/)
 [![Downloads](https://static.pepy.tech/personalized-badge/flask-signing?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/flask-signing)
 [![Flask-Signing tests](https://github.com/signebedi/Flask-Signing/workflows/tests/badge.svg)](https://github.com/signebedi/Flask-Signing/actions)
+[![Buy me a coffee](https://img.shields.io/badge/Buy%20me%20a%20coffee--brightgreen.svg?logo=buy-me-a-coffee&logoColor=brightgreen)](https://www.buymeacoffee.com/signebedi)
 
 a signing key extension for flask
 
 
 ### About
 
 The Flask-Signing library is a useful tool for Flask applications that require secure and robust management of signing keys. Do you need to generate single-use tokens for one-time actions like email verification or password reset? Flask-Signing can handle that. Are you looking for a simple method for managing API keys? Look no further. 
@@ -37,17 +38,17 @@
 
 First, install the flask_signing package. You can do this with pip:
 
 ```bash
 pip install flask_signing
 ```
 
-### Usage
+### Basic Usage
 
-After you've installed the package, you can use it in your Flask application. Here's an example of how you might do this:
+After you've installed the flask_signing package, you can use it in your Flask application. Here's an example of how you might do this:
 
 ```python
 from flask import Flask
 from flask_sqlalchemy import SQLAlchemy
 from flask_signing import Signatures
 
 app = Flask(__name__)
@@ -75,14 +76,14 @@
     
 @app.route('/all')
 def all():
     all = signatures.get_all()
     return f'Response: {all}'
 ```
 
-In this example, a new signing key is generated and written to the database when you visit the /sign route, and the key is displayed on the page. Then, when you visit the /verify/<key> route (replace <key> with the actual key), the validity of the key is checked and displayed. You can expire a key using the /expire/<key> route, and view all records with the /all route.
+In this basic example, a new signing key is generated and written to the database when you visit the `/sign` route, and the key is displayed on the page. Then, when you visit the `/verify/<key>` route (replace <key> with the actual key), the validity of the key is checked and displayed. You can expire a key using the `/expire/<key>` route, and view all records with the `/all` route.
 
-Please note that this is a very basic example and your actual use of the flask_signing package may be more complex depending on your needs. It's important to secure your signing keys and handle them appropriately according to your application's security requirements.
+This is a rather basic example and your actual use of the flask_signing package may be more complex depending on your needs. It's important to secure your signing keys and handle them appropriately according to your application's security requirements. Further usage examples can be found in the [examples](https://github.com/signebedi/Flask-Signing/tree/master/examples) directory of the Flask-Signing Github repository. 
 
 ### Developers
 
 Contributions are welcome! You can read the developer docs at https://signebedi.github.io/Flask-Signing. If you're interested, review (or add to) the feature ideas at https://github.com/signebedi/Flask-Signing/issues.
```

### Comparing `flask_signing-0.6.0/setup.py` & `flask_signing-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `flask_signing-0.6.0/tests/__init__.py` & `flask_signing-0.7.0/tests/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os, datetime, unittest, time
 from flask import Flask
 from flask_sqlalchemy import SQLAlchemy
-from flask_signing import Signatures, RateLimitExceeded
+from flask_signing import Signatures, DangerousSignatures, RateLimitExceeded
 
 class TestFlaskSigning(unittest.TestCase):
 
     def setUp(self):
         """
         Set up testing environment.
         """
@@ -242,9 +242,54 @@
             # Wait for the rate limit period to pass
             time.sleep(2)
 
             # Validate the key again, should return True
             self.assertTrue(self.signatures.verify_key(signature, scope))
 
 
+class TestDangerousFlaskSigning(TestFlaskSigning):
+
+
+
+    def setUp(self):
+        """
+        Set up testing environment for DangerousSignatures.
+        """
+
+        self.app = Flask(__name__)
+        self.app.config['SQLALCHEMY_DATABASE_URI'] = 'sqlite:///:memory:'
+        self.app.config['SECRET_KEY'] = 'Your_Key_Here'
+        self.app.config['TESTING'] = True
+        
+
+        with self.app.app_context():
+            self.signatures = DangerousSignatures(app=self.app)
+            self.db = self.signatures.db
+            self.db.create_all()
+
+    def test_generate_key(self):
+        """
+        Test if the generate_key method returns a correctly serialized string,
+        for keys of various byte lengths
+        """
+
+        for i in range(10, 256):
+            with self.app.app_context():
+                key = self.signatures.generate_key(length=i)
+                data = self.signatures.serializer.loads(key)
+            # self.assertEqual(len(data['key']), i)
+            self.assertTrue(i < len(data['key']) < 1.6*i)
+            self.assertIsInstance(key, str)
+
+    def test_serializer(self):
+        """
+        Test if the serializer properly serializes and deserializes data
+        """
+
+        with self.app.app_context():
+            data = {'key': 'test_data'}
+            serialized_data = self.signatures.serializer.dumps(data)
+            deserialized_data = self.signatures.serializer.loads(serialized_data)
+        self.assertEqual(data, deserialized_data)
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flask_signing-0.6.0/tests/performance_tests.py` & `flask_signing-0.7.0/tests/performance_tests.py`

 * *Files identical despite different names*

