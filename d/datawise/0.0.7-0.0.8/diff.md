# Comparing `tmp/datawise-0.0.7.tar.gz` & `tmp/datawise-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawise-0.0.7.tar", max compression
+gzip compressed data, was "datawise-0.0.8.tar", max compression
```

## Comparing `datawise-0.0.7.tar` & `datawise-0.0.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.7/LICENSE
--rw-r--r--   0        0        0     4287 2023-06-18 13:09:36.174443 datawise-0.0.7/README.md
--rw-r--r--   0        0        0     3133 2023-06-18 12:58:49.702867 datawise-0.0.7/datawise/__init__.py
--rw-r--r--   0        0        0      481 2023-06-18 12:46:33.125357 datawise-0.0.7/datawise/exceptions.py
--rw-r--r--   0        0        0      517 2023-06-18 13:33:56.718918 datawise-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     4813 1970-01-01 00:00:00.000000 datawise-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.8/LICENSE
+-rw-r--r--   0        0        0     4758 2023-06-18 13:38:57.109053 datawise-0.0.8/README.md
+-rw-r--r--   0        0        0     3134 2023-06-18 13:40:56.003231 datawise-0.0.8/datawise/__init__.py
+-rw-r--r--   0        0        0      481 2023-06-18 12:46:33.125357 datawise-0.0.8/datawise/exceptions.py
+-rw-r--r--   0        0        0      517 2023-06-18 13:40:29.606498 datawise-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     5284 1970-01-01 00:00:00.000000 datawise-0.0.8/PKG-INFO
```

### Comparing `datawise-0.0.7/LICENSE` & `datawise-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `datawise-0.0.7/README.md` & `datawise-0.0.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 ```bash
 pip install pandas numpy
 ```
 
 To transform, simply call `sql` function.
 ```python
 import datawise as dw
+import pandas as pd
 
 countries = pd.DataFrame({
     "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain", "Canada", "Australia", "Japan", "China"],
     "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832, 1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440, 14631844184064],
     "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
 })
 
@@ -52,14 +53,15 @@
    NumCountry
 0          10
 ```
 
 You can also do joins of multiple dataframes:
 ```python
 import datawise as dw
+import pandas as pd
 
 countries = pd.DataFrame({
     "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain", "Canada", "Australia", "Japan", "China"],
     "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832, 1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440, 14631844184064],
     "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
 })
 
@@ -91,14 +93,21 @@
 9           China  14631844184064             5.12          10
 ```
 
 ## Error Handling
 Errors could happen if we cannot translate the SQL query. Consider the following example:
 ```python
 import datawise as dw
+import pandas as pd
+
+countries = pd.DataFrame({
+    "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain", "Canada", "Australia", "Japan", "China"],
+    "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832, 1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440, 14631844184064],
+    "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
+})
 
 datawise = dw.DataWise(api_key="you_api_key_here")
 datawise.sql("SELECT bad_column FROM bad_table", {
   "countries": countries
 })
 ```
```

### Comparing `datawise-0.0.7/datawise/__init__.py` & `datawise-0.0.8/datawise/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     """
     return self._sql(query, dataframes, code=code)
 
 
   @retry(exceptions=(RequestException, DataWiseInternalError), tries=3, delay=2)
   def _sql(self, query, dataframes, error=None, code=False, num_retries=0, prev_code=None):
     if not (type(dataframes) is dict): raise Exception("dataframes needs to be a dictionary with key being dataframe name and value being the dataframe.")
-    if num_retries > 3:
+    if num_retries >= 2:
       logging.error(f"We couldn't translate your query. Here is python code we attempted to generate: \n{prev_code}")
       raise TranslationError()
 
     data = {
       "dataframe": "\n".join([f"{idx+1}. Dataframe named {key} with columns {value.columns.tolist()}" for idx, (key, value) in enumerate(dataframes.items())]),
       "sql": query,
       "error": error
```

### Comparing `datawise-0.0.7/pyproject.toml` & `datawise-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datawise"
-version = "0.0.7"
+version = "0.0.8"
 description = "Testing"
 authors = ["DataWise Team"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9.0"
 python-dotenv = "^1.0.0"
```

### Comparing `datawise-0.0.7/PKG-INFO` & `datawise-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawise
-Version: 0.0.7
+Version: 0.0.8
 Summary: Testing
 Author: DataWise Team
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -44,14 +44,15 @@
 ```bash
 pip install pandas numpy
 ```
 
 To transform, simply call `sql` function.
 ```python
 import datawise as dw
+import pandas as pd
 
 countries = pd.DataFrame({
     "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain", "Canada", "Australia", "Japan", "China"],
     "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832, 1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440, 14631844184064],
     "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
 })
 
@@ -68,14 +69,15 @@
    NumCountry
 0          10
 ```
 
 You can also do joins of multiple dataframes:
 ```python
 import datawise as dw
+import pandas as pd
 
 countries = pd.DataFrame({
     "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain", "Canada", "Australia", "Japan", "China"],
     "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832, 1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440, 14631844184064],
     "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
 })
 
@@ -107,14 +109,21 @@
 9           China  14631844184064             5.12          10
 ```
 
 ## Error Handling
 Errors could happen if we cannot translate the SQL query. Consider the following example:
 ```python
 import datawise as dw
+import pandas as pd
+
+countries = pd.DataFrame({
+    "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain", "Canada", "Australia", "Japan", "China"],
+    "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832, 1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440, 14631844184064],
+    "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
+})
 
 datawise = dw.DataWise(api_key="you_api_key_here")
 datawise.sql("SELECT bad_column FROM bad_table", {
   "countries": countries
 })
 ```
```

