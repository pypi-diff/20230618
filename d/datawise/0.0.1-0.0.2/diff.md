# Comparing `tmp/datawise-0.0.1.tar.gz` & `tmp/datawise-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawise-0.0.1.tar", max compression
+gzip compressed data, was "datawise-0.0.2.tar", max compression
```

## Comparing `datawise-0.0.1.tar` & `datawise-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.1/LICENSE
--rw-r--r--   0        0        0     2233 2023-06-18 02:49:30.570947 datawise-0.0.1/datawise/__init__.py
--rw-r--r--   0        0        0      334 2023-06-18 02:49:50.939696 datawise-0.0.1/datawise/exceptions.py
--rw-r--r--   0        0        0      463 2023-06-18 02:48:46.674314 datawise-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      317 1970-01-01 00:00:00.000000 datawise-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2306 2023-06-18 03:27:24.836274 datawise-0.0.2/datawise/__init__.py
+-rw-r--r--   0        0        0      334 2023-06-18 02:49:50.939696 datawise-0.0.2/datawise/exceptions.py
+-rw-r--r--   0        0        0      463 2023-06-18 03:28:26.019065 datawise-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      317 1970-01-01 00:00:00.000000 datawise-0.0.2/PKG-INFO
```

### Comparing `datawise-0.0.1/LICENSE` & `datawise-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datawise-0.0.1/datawise/__init__.py` & `datawise-0.0.2/datawise/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import json
 import os
 import requests
 
 from dotenv import load_dotenv
 from .exceptions import AuthorizationError, DataWiseInternalError
 from requests.exceptions import RequestException
@@ -38,23 +39,23 @@
       }
     )
 
     if (response.status_code == 400): raise AuthorizationError()
     if (response.status_code >= 500): raise DataWiseInternalError()
 
     python_code = response.json()
-    if code: return python_code
     
     import pandas as pd
     globals = { "pd": pd }
     locals = dataframes.copy()
     try:
       exec(python_code, globals, locals)
       if isinstance(locals["return_df"], pd.DataFrame):
         return_df=locals["return_df"].reset_index(drop=True)
+        if code: logging.info(f"Given query: \n{query} \nOutput code: \n{python_code}\n")
       else:
         num_retries += 1
         data["error"] = "Is not a pandas dataframe. Please return dataframe."
         return_df = self.sql(query, dataframes, error=data["error"], code=code, num_retries=num_retries)
     except Exception as e:
       num_retries += 1
       data["error"] = f"Threw exception: `{e}`"
```

