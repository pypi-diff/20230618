# Comparing `tmp/datawise-0.0.2.tar.gz` & `tmp/datawise-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawise-0.0.2.tar", max compression
+gzip compressed data, was "datawise-0.0.3.tar", max compression
```

## Comparing `datawise-0.0.2.tar` & `datawise-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.2/LICENSE
--rw-r--r--   0        0        0     2306 2023-06-18 03:27:24.836274 datawise-0.0.2/datawise/__init__.py
--rw-r--r--   0        0        0      334 2023-06-18 02:49:50.939696 datawise-0.0.2/datawise/exceptions.py
--rw-r--r--   0        0        0      463 2023-06-18 03:28:26.019065 datawise-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      317 1970-01-01 00:00:00.000000 datawise-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2958 2023-06-18 11:33:26.090801 datawise-0.0.3/datawise/__init__.py
+-rw-r--r--   0        0        0      334 2023-06-18 02:49:50.939696 datawise-0.0.3/datawise/exceptions.py
+-rw-r--r--   0        0        0      485 2023-06-18 11:30:59.853996 datawise-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      321 1970-01-01 00:00:00.000000 datawise-0.0.3/PKG-INFO
```

### Comparing `datawise-0.0.2/LICENSE` & `datawise-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datawise-0.0.2/datawise/__init__.py` & `datawise-0.0.3/datawise/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,51 @@
-import logging
 import json
+import logging
 import os
 import requests
 
-from dotenv import load_dotenv
 from .exceptions import AuthorizationError, DataWiseInternalError
+from dotenv import load_dotenv
 from requests.exceptions import RequestException
 from retry import retry
 
 
 class DataWise:
+  """Creates a new DataWise API client."""
   def __init__(
     self, 
     api_base="https://datawise.vercel.app/api",
     api_key=None
   ):
     load_dotenv()
     self.api_base = api_base if api_base else os.getenv("DATAWISE_API_BASE")
     self.api_key = api_key if api_key else os.getenv("DATAWISE_API_KEY")
-    
+
+  
+  def sql(self, query, dataframes, code=False):
+    """
+    Transforms given dataframes based on given SQL query.
+
+    Parameters:
+    -----------
+    query: str
+      SQL query to be executed.
+    dataframes: dict
+      Dictionary of dataframes to be transformed.
+      The key is the dataframe name and the value is the dataframe itself.
+      Example:
+      {"customers_df": customers_df, "employees_df": employees_df}
+    Code: bool
+      Whether to print/log the pandas code used to transformed dataframes or not.
+    """
+    return self._sql(query, dataframes, code=code)
+
+
   @retry(exceptions=(RequestException, DataWiseInternalError), tries=3, delay=2)
-  def sql(self, query, dataframes, error=None, code=False, num_retries=0):
+  def _sql(self, query, dataframes, error=None, code=False, num_retries=0):
     if not (type(dataframes) is dict): raise Exception("dataframes needs to be a dictionary with key being dataframe name and value being the dataframe.")
     if num_retries > 3: raise Exception("We couldn't translate your query. :(")
 
     data = {
       "dataframe": "\n".join([f"{idx+1}. Dataframe named {key} with columns {value.columns.tolist()}" for idx, (key, value) in enumerate(dataframes.items())]),
       "sql": query,
       "error": error
@@ -39,17 +60,18 @@
       }
     )
 
     if (response.status_code == 400): raise AuthorizationError()
     if (response.status_code >= 500): raise DataWiseInternalError()
 
     python_code = response.json()
-    
+
     import pandas as pd
-    globals = { "pd": pd }
+    import numpy as np
+    globals = { "np": np, "pd": pd }
     locals = dataframes.copy()
     try:
       exec(python_code, globals, locals)
       if isinstance(locals["return_df"], pd.DataFrame):
         return_df=locals["return_df"].reset_index(drop=True)
         if code: logging.info(f"Given query: \n{query} \nOutput code: \n{python_code}\n")
       else:
```

