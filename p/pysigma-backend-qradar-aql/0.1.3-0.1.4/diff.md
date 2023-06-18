# Comparing `tmp/pysigma_backend_qradar_aql-0.1.3.tar.gz` & `tmp/pysigma_backend_qradar_aql-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_backend_qradar_aql-0.1.3.tar", max compression
+gzip compressed data, was "pysigma_backend_qradar_aql-0.1.4.tar", max compression
```

## Comparing `pysigma_backend_qradar_aql-0.1.3.tar` & `pysigma_backend_qradar_aql-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1088 2023-05-11 10:26:27.440460 pysigma_backend_qradar_aql-0.1.3/LICENSE
--rw-r--r--   0        0        0    26893 2023-05-18 15:50:26.457194 pysigma_backend_qradar_aql-0.1.3/README.md
--rw-r--r--   0        0        0      539 2023-05-19 13:59:12.906094 pysigma_backend_qradar_aql-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    18776 2023-05-14 09:29:21.546257 pysigma_backend_qradar_aql-0.1.3/sigma/backends/QRadarAQL/QRadarAQL.py
--rw-r--r--   0        0        0      251 2023-05-18 15:03:35.537046 pysigma_backend_qradar_aql-0.1.3/sigma/backends/QRadarAQL/__init__.py
--rw-r--r--   0        0        0    24281 2023-05-14 09:29:21.547589 pysigma_backend_qradar_aql-0.1.3/sigma/pipelines/QRadarAQL/QRadarAQL.py
--rw-r--r--   0        0        0     1466 2023-05-10 20:46:57.641000 pysigma_backend_qradar_aql-0.1.3/sigma/pipelines/QRadarAQL/QRadarAQL_fields.py
--rw-r--r--   0        0        0     5230 2023-05-14 09:29:21.548462 pysigma_backend_qradar_aql-0.1.3/sigma/pipelines/QRadarAQL/QRadarAQL_payload.py
--rw-r--r--   0        0        0      238 2023-05-15 06:54:27.232430 pysigma_backend_qradar_aql-0.1.3/sigma/pipelines/QRadarAQL/__init__.py
--rw-r--r--   0        0        0    27605 1970-01-01 00:00:00.000000 pysigma_backend_qradar_aql-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-05-11 10:26:27.440460 pysigma_backend_qradar_aql-0.1.4/LICENSE
+-rw-r--r--   0        0        0    26893 2023-05-18 15:50:26.457194 pysigma_backend_qradar_aql-0.1.4/README.md
+-rw-r--r--   0        0        0      539 2023-06-18 11:06:18.002045 pysigma_backend_qradar_aql-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    18776 2023-06-18 09:16:11.240880 pysigma_backend_qradar_aql-0.1.4/sigma/backends/QRadarAQL/QRadarAQL.py
+-rw-r--r--   0        0        0      251 2023-06-12 15:14:20.587205 pysigma_backend_qradar_aql-0.1.4/sigma/backends/QRadarAQL/__init__.py
+-rw-r--r--   0        0        0    24281 2023-06-18 10:45:59.476907 pysigma_backend_qradar_aql-0.1.4/sigma/pipelines/QRadarAQL/QRadarAQL.py
+-rw-r--r--   0        0        0     1466 2023-05-10 20:46:57.641000 pysigma_backend_qradar_aql-0.1.4/sigma/pipelines/QRadarAQL/QRadarAQL_fields.py
+-rw-r--r--   0        0        0     5230 2023-05-14 09:29:21.548462 pysigma_backend_qradar_aql-0.1.4/sigma/pipelines/QRadarAQL/QRadarAQL_payload.py
+-rw-r--r--   0        0        0      238 2023-05-15 06:54:27.232430 pysigma_backend_qradar_aql-0.1.4/sigma/pipelines/QRadarAQL/__init__.py
+-rw-r--r--   0        0        0    27605 1970-01-01 00:00:00.000000 pysigma_backend_qradar_aql-0.1.4/PKG-INFO
```

### Comparing `pysigma_backend_qradar_aql-0.1.3/LICENSE` & `pysigma_backend_qradar_aql-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.1.3/README.md` & `pysigma_backend_qradar_aql-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.1.3/pyproject.toml` & `pysigma_backend_qradar_aql-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pySigma-backend-QRadar-AQL"
-version = "0.1.3"
+version = "0.1.4"
 description = "pySigma QRadarAQL backend"
 authors = ["IBM <noaakless@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/IBM/pySigma-backend-QRadar-AQL"
 packages = [
     { include = "sigma" }
 ]
```

### Comparing `pysigma_backend_qradar_aql-0.1.3/sigma/backends/QRadarAQL/QRadarAQL.py` & `pysigma_backend_qradar_aql-0.1.4/sigma/backends/QRadarAQL/QRadarAQL.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         str] = "="  # Token inserted between field and value (without separator)
 
     # String output
     ## Fields
     ### Quoting
 
     field_quote: ClassVar[
-        str] = "'"  # Character used to quote field characters if field_quote_pattern
+        str] = '"'  # Character used to quote field characters if field_quote_pattern
     # doesn't match
     field_quote_pattern: ClassVar[Pattern] = re.compile(
         "^\S+$|.*\([^()]*\).*")  # Quote field names if this pattern
     # doesn't match- contains spacing or doesn't contain parentheses
     field_quote_pattern_negation: ClassVar[
         bool] = True  # Negate field_quote_pattern result. Field name is quoted if
     # pattern doesn't match if set to True
```

### Comparing `pysigma_backend_qradar_aql-0.1.3/sigma/pipelines/QRadarAQL/QRadarAQL.py` & `pysigma_backend_qradar_aql-0.1.4/sigma/pipelines/QRadarAQL/QRadarAQL.py`

 * *Files 1% similar despite different names*

```diff
@@ -680,15 +680,15 @@
     def apply_field_name(self, field: str) -> Union[str, List[str]]:
         parentheses_and_no_spacing = re.compile(QRadarAQLBackend.field_quote_pattern)
         mappings = copy.deepcopy(self.get_mapping(field)) or []
         if isinstance(mappings, str):
             mappings = [mappings]
         for i, mapping in enumerate(mappings):
             if not parentheses_and_no_spacing.match(mapping):
-                mappings[i] = "'" + mapping + "'"
+                mappings[i] = '"' + mapping + '"'
         return mappings
 
 
 class SetEventSourceTransformation(SetStateTransformation):
     """
     set the logsources values from the field devicetype in state, to use it in the
     backend's finalize query
```

### Comparing `pysigma_backend_qradar_aql-0.1.3/sigma/pipelines/QRadarAQL/QRadarAQL_fields.py` & `pysigma_backend_qradar_aql-0.1.4/sigma/pipelines/QRadarAQL/QRadarAQL_fields.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.1.3/sigma/pipelines/QRadarAQL/QRadarAQL_payload.py` & `pysigma_backend_qradar_aql-0.1.4/sigma/pipelines/QRadarAQL/QRadarAQL_payload.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.1.3/PKG-INFO` & `pysigma_backend_qradar_aql-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysigma-backend-qradar-aql
-Version: 0.1.3
+Version: 0.1.4
 Summary: pySigma QRadarAQL backend
 Home-page: https://github.com/IBM/pySigma-backend-QRadar-AQL
 License: MIT
 Author: IBM
 Author-email: noaakless@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

