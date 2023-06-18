# Comparing `tmp/dataskema-1.6.7.tar.gz` & `tmp/dataskema-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataskema-1.6.7.tar", last modified: Wed Jun 15 07:57:18 2022, max compression
+gzip compressed data, was "dist/dataskema-1.7.0.tar", last modified: Sun Jun 18 09:54:19 2023, max compression
```

## Comparing `dataskema-1.6.7.tar` & `dataskema-1.7.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 lagor      (501) staff       (20)        0 2022-06-15 07:57:18.021278 dataskema-1.6.7/
--rw-r--r--   0 lagor      (501) staff       (20)     1080 2022-04-04 16:22:31.000000 dataskema-1.6.7/LICENSE
--rw-r--r--   0 lagor      (501) staff       (20)    25013 2022-06-15 07:57:18.020900 dataskema-1.6.7/PKG-INFO
--rw-r--r--   0 lagor      (501) staff       (20)    20118 2022-06-15 07:55:43.000000 dataskema-1.6.7/README.md
-drwxr-xr-x   0 lagor      (501) staff       (20)        0 2022-06-15 07:57:18.014524 dataskema-1.6.7/dataskema/
--rw-r--r--   0 lagor      (501) staff       (20)      136 2022-06-08 14:00:23.000000 dataskema-1.6.7/dataskema/__init__.py
--rw-r--r--   0 lagor      (501) staff       (20)     3947 2022-04-27 11:52:42.000000 dataskema-1.6.7/dataskema/data_schema.py
--rw-r--r--   0 lagor      (501) staff       (20)    10989 2022-06-07 06:08:56.000000 dataskema-1.6.7/dataskema/data_types.py
-drwxr-xr-x   0 lagor      (501) staff       (20)        0 2022-06-15 07:57:18.019752 dataskema-1.6.7/dataskema/decorators/
--rw-r--r--   0 lagor      (501) staff       (20)        0 2022-04-03 18:14:32.000000 dataskema-1.6.7/dataskema/decorators/__init__.py
--rw-r--r--   0 lagor      (501) staff       (20)      546 2022-06-08 14:36:28.000000 dataskema-1.6.7/dataskema/decorators/args.py
--rw-r--r--   0 lagor      (501) staff       (20)     1855 2022-06-15 07:54:37.000000 dataskema-1.6.7/dataskema/decorators/flask.py
--rw-r--r--   0 lagor      (501) staff       (20)     4178 2022-06-13 15:33:10.000000 dataskema-1.6.7/dataskema/lang.py
--rw-r--r--   0 lagor      (501) staff       (20)     1448 2022-04-20 06:53:20.000000 dataskema-1.6.7/dataskema/util.py
--rw-r--r--   0 lagor      (501) staff       (20)    24170 2022-06-13 15:33:10.000000 dataskema-1.6.7/dataskema/validator.py
-drwxr-xr-x   0 lagor      (501) staff       (20)        0 2022-06-15 07:57:18.018141 dataskema-1.6.7/dataskema.egg-info/
--rw-r--r--   0 lagor      (501) staff       (20)    25013 2022-06-15 07:57:17.000000 dataskema-1.6.7/dataskema.egg-info/PKG-INFO
--rw-r--r--   0 lagor      (501) staff       (20)      444 2022-06-15 07:57:18.000000 dataskema-1.6.7/dataskema.egg-info/SOURCES.txt
--rw-r--r--   0 lagor      (501) staff       (20)        1 2022-06-15 07:57:17.000000 dataskema-1.6.7/dataskema.egg-info/dependency_links.txt
--rw-r--r--   0 lagor      (501) staff       (20)        1 2022-04-17 19:18:28.000000 dataskema-1.6.7/dataskema.egg-info/not-zip-safe
--rw-r--r--   0 lagor      (501) staff       (20)        6 2022-06-15 07:57:17.000000 dataskema-1.6.7/dataskema.egg-info/requires.txt
--rw-r--r--   0 lagor      (501) staff       (20)       10 2022-06-15 07:57:17.000000 dataskema-1.6.7/dataskema.egg-info/top_level.txt
--rw-r--r--   0 lagor      (501) staff       (20)       38 2022-06-15 07:57:18.021395 dataskema-1.6.7/setup.cfg
--rw-r--r--   0 lagor      (501) staff       (20)      961 2022-06-15 07:55:11.000000 dataskema-1.6.7/setup.py
+drwxr-xr-x   0 lagor      (501) staff       (20)        0 2023-06-18 09:54:19.000000 dataskema-1.7.0/
+-rw-r--r--   0 lagor      (501) staff       (20)    25324 2023-06-18 09:54:19.000000 dataskema-1.7.0/PKG-INFO
+-rw-r--r--   0 lagor      (501) staff       (20)     1080 2022-04-04 16:22:31.000000 dataskema-1.7.0/LICENSE
+-rw-r--r--   0 lagor      (501) staff       (20)    20387 2023-06-18 09:52:00.000000 dataskema-1.7.0/README.md
+-rw-r--r--   0 lagor      (501) staff       (20)      955 2023-06-18 09:52:13.000000 dataskema-1.7.0/setup.py
+drwxr-xr-x   0 lagor      (501) staff       (20)        0 2023-06-18 09:54:19.000000 dataskema-1.7.0/dataskema/
+-rw-r--r--   0 lagor      (501) staff       (20)    26776 2023-06-18 09:54:05.000000 dataskema-1.7.0/dataskema/validator.py
+-rw-r--r--   0 lagor      (501) staff       (20)     4137 2023-06-18 09:38:01.000000 dataskema-1.7.0/dataskema/lang.py
+-rw-r--r--   0 lagor      (501) staff       (20)     4008 2023-06-18 09:37:38.000000 dataskema-1.7.0/dataskema/data_schema.py
+drwxr-xr-x   0 lagor      (501) staff       (20)        0 2023-06-18 09:54:19.000000 dataskema-1.7.0/dataskema/decorators/
+-rw-r--r--   0 lagor      (501) staff       (20)     1794 2023-06-18 09:43:11.000000 dataskema-1.7.0/dataskema/decorators/flask.py
+-rw-r--r--   0 lagor      (501) staff       (20)        0 2022-04-03 18:14:32.000000 dataskema-1.7.0/dataskema/decorators/__init__.py
+-rw-r--r--   0 lagor      (501) staff       (20)      546 2022-06-08 14:36:28.000000 dataskema-1.7.0/dataskema/decorators/args.py
+-rw-r--r--   0 lagor      (501) staff       (20)     1448 2022-04-20 06:53:20.000000 dataskema-1.7.0/dataskema/util.py
+-rw-r--r--   0 lagor      (501) staff       (20)      136 2022-06-08 14:00:23.000000 dataskema-1.7.0/dataskema/__init__.py
+-rw-r--r--   0 lagor      (501) staff       (20)    10989 2022-06-07 06:08:56.000000 dataskema-1.7.0/dataskema/data_types.py
+-rw-r--r--   0 lagor      (501) staff       (20)       38 2023-06-18 09:54:19.000000 dataskema-1.7.0/setup.cfg
+drwxr-xr-x   0 lagor      (501) staff       (20)        0 2023-06-18 09:54:19.000000 dataskema-1.7.0/dataskema.egg-info/
+-rw-r--r--   0 lagor      (501) staff       (20)    25324 2023-06-18 09:54:19.000000 dataskema-1.7.0/dataskema.egg-info/PKG-INFO
+-rw-r--r--   0 lagor      (501) staff       (20)        1 2022-04-17 19:18:28.000000 dataskema-1.7.0/dataskema.egg-info/not-zip-safe
+-rw-r--r--   0 lagor      (501) staff       (20)      444 2023-06-18 09:54:19.000000 dataskema-1.7.0/dataskema.egg-info/SOURCES.txt
+-rw-r--r--   0 lagor      (501) staff       (20)        6 2023-06-18 09:54:19.000000 dataskema-1.7.0/dataskema.egg-info/requires.txt
+-rw-r--r--   0 lagor      (501) staff       (20)       10 2023-06-18 09:54:19.000000 dataskema-1.7.0/dataskema.egg-info/top_level.txt
+-rw-r--r--   0 lagor      (501) staff       (20)        1 2023-06-18 09:54:19.000000 dataskema-1.7.0/dataskema.egg-info/dependency_links.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `dataskema-1.6.7/LICENSE` & `dataskema-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dataskema-1.6.7/PKG-INFO` & `dataskema-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 Metadata-Version: 2.1
 Name: dataskema
-Version: 1.6.7
+Version: 1.7.0
 Summary: Data schema to validate parameters easily, quickly and with minimal code
 Home-page: https://github.com/lagor-github/dataskema
-Author: Luis A. González Rivas
+Author: Luis A. González
 Author-email: lagor55@gmail.com
 License: MIT
 Description: # `dataskema`
         Data schema validation for python
         
+        v1.7.0
+        - Now dict types can have schema in its fields using 'schema' keyword
+        - Use 'only-schema-keys' keyword to reject no declareted fields
+        - New 'null-when-zero' keyword that rewrites incoming value to None value when zero (number or string)
+        - Some minor bugs fixed
+        
         v1.6.7
         - Bug fixed in @dataskema.flask_url
         
         v1.6.6
         - Schemas for 'dict' types fields
         - 'max-size' and 'min-size' are valid for 'int' and 'float' types
```

### Comparing `dataskema-1.6.7/README.md` & `dataskema-1.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 # `dataskema`
 Data schema validation for python
 
+v1.7.0
+- Now dict types can have schema in its fields using 'schema' keyword
+- Use 'only-schema-keys' keyword to reject no declareted fields
+- New 'null-when-zero' keyword that rewrites incoming value to None value when zero (number or string)
+- Some minor bugs fixed
+
 v1.6.7
 - Bug fixed in @dataskema.flask_url
 
 v1.6.6
 - Schemas for 'dict' types fields
 - 'max-size' and 'min-size' are valid for 'int' and 'float' types
```

### Comparing `dataskema-1.6.7/dataskema/data_schema.py` & `dataskema-1.7.0/dataskema/data_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     def __init__(self, message: str, results: dict):
         idx = message.find('\n')
         line = message[0:idx] if idx >= 0 else message
         line = util.no_acute(line)
         super(SchemaValidationResult, self).__init__(line)
         self.message = message
-        self.results = results if results is not None else {}
+        self.results = results if isinstance(results, dict) else {}  # -- bug fixed 1.6.8: podría no ser un dict
 
     def get_results(self) -> dict:
         return self.results
 
     def get_result_of(self, name: str) -> dict:
         return self.results.get(name)
 
@@ -82,15 +82,15 @@
                 continue
             validator = SchemaValidator(schema)
             try:
                 pvalue = validator.validate(pname, pvalue)
                 self.data[pname] = pvalue
                 _add_is_valid(result, pname)
             except SchemaValidationFailure as ex:
-                _add_is_not_valid(result, pname, ex.get_name(), ex.get_message(True))
+                _add_is_not_valid(result, ex.get_name(), ex.get_label(), ex.get_message(True))
                 if MAX_VALIDATION_MESSAGES <= 0 or len(first_messages) < MAX_VALIDATION_MESSAGES:
                     first_messages.append(ex.get_message(False))
                 valid = False
                 total_errors = total_errors + 1
         if not valid:
             first_message = '\n'.join(first_messages) + '\n' + lang.get_more_messages(total_errors - 1)
             raise SchemaValidationResult(first_message, result)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dataskema-1.6.7/dataskema/data_types.py` & `dataskema-1.7.0/dataskema/data_types.py`

 * *Files identical despite different names*

### Comparing `dataskema-1.6.7/dataskema/decorators/args.py` & `dataskema-1.7.0/dataskema/decorators/args.py`

 * *Files identical despite different names*

### Comparing `dataskema-1.6.7/dataskema/decorators/flask.py` & `dataskema-1.7.0/dataskema/decorators/flask.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # -*- coding: utf-8 -*-
 # pylint: disable=missing-docstring, C0301
-import json
 import functools
-from dataskema.data_schema import DataSchema, SchemaValidationResult
-from flask import request, make_response, Response
+from dataskema.data_schema import DataSchema
+from flask import request
 
 
 class JSON(DataSchema):
     def __init__(self):
         super(JSON, self).__init__(request.get_json())
```

### Comparing `dataskema-1.6.7/dataskema/util.py` & `dataskema-1.7.0/dataskema/util.py`

 * *Files identical despite different names*

### Comparing `dataskema-1.6.7/dataskema/validator.py` & `dataskema-1.7.0/dataskema/validator.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,26 +31,28 @@
 KEYWORD_MAX_SIZE = 'max-size'
 KEYWORD_REGEXP = 'regexp'
 KEYWORD_ICASE = 'icase'
 KEYWORD_WHITE_LIST = 'white-list'
 KEYWORD_MAX_LINES = 'max-lines'
 KEYWORD_FORMAT = 'format'
 KEYWORD_JOIN = 'join'
+KEYWORD_NULL_WHEN_ZERO = 'null-when-zero'
 
 KEYWORD_TYPE_INT = 'int'
 KEYWORD_TYPE_FLOAT = 'float'
 KEYWORD_MIN_VALUE = 'min-value'
 KEYWORD_MAX_VALUE = 'max-value'
 
 KEYWORD_TYPE_BOOL = 'bool'
 KEYWORD_BOOL_TRUE = 'true'
 KEYWORD_BOOL_FALSE = 'false'
 
 KEYWORD_TYPE_ANY = 'any'
 KEYWORD_SCHEMA = 'schema'
+KEYWORD_ONLY_SCHEMA_KEYS = 'only-schema-keys'
 
 KEYWORD_TO = 'to'
 KEYWORD_TO_FUNC_LOWER = 'lower'
 KEYWORD_TO_FUNC_UPPER = 'upper'
 KEYWORD_TO_FUNC_NO_TRIM = 'no-trim'
 KEYWORD_TO_FUNC_TRIM = 'trim'
 
@@ -63,14 +65,20 @@
 DEFAULT_TIME_FORMAT = '%H:%M:%S'
 DEFAULT_DATETIME_FORMAT = DEFAULT_DATE_FORMAT + ' ' + DEFAULT_TIME_FORMAT
 
 ERROR_INVALID_TYPE = "'{keyword}' has an invalid value '{itype}'"
 ERROR_INVALID_DEFAULT_TYPE = "Invalid default value type '{def_itype}'. Expected type '{itype}"
 ERROR_UNEXPECTED_TYPE = "Type '{expected_type}' expected. Found '{utype}'"
 ERROR_INVALID_FUNCTION_NAME = "'Invalid '{keyword}' function '{func_name}'"
+ERROR_EXPECTED_FIELD_TYPE = "Expected field '{field_name}' into '{label}'"
+ERROR_SCHEMA_EXPECTED_FOR_FIELD = "Schema expected for field '{field_name}' into '{label}'"
+ERROR_SCHEMA_EXPECTED_FOR_DICT = "Schema expected for '{field_name}'"
+ERROR_SCHEMA_EXPECTED_FOR_ITEM_LIST = "Schema expected for item of '{field_name}'"
+
+KEYWORD_VALUE = 'value'
 
 
 class SchemaFormatError(ValueError):
     def __init__(self, message: dict or str, params: dict):
         super(SchemaFormatError, self).__init__(lang.get_message(message, params))
 
 
@@ -88,14 +96,20 @@
 
     def get_message(self, anonymize: bool or None = False) -> str:
         return lang.get_message(self.message, self.params, anonymize)
 
     def get_name(self) -> str:
         return self.params.get(KEYWORD_NAME)
 
+    def get_label(self) -> str:
+        return self.params.get(KEYWORD_LABEL)
+
+    def get_params(self) -> dict:
+        return self.params
+
 
 class SchemaValidator:
 
     def __init__(self, data_schema: dict):
         """
         """
         self.data_schema = data_schema
@@ -121,48 +135,48 @@
         if itype is not None:
             try:
                 if itype == KEYWORD_TYPE_STR:
                     keyword2 = KEYWORD_FORMAT
                     sformat = self._get_str(keyword2)
                     keyword2 = KEYWORD_JOIN
                     join = self._get_str(keyword2)
-                    value = _get_type_str(label, value, sformat, join)
+                    value = _get_type_str(name, label, value, sformat, join)
                 elif itype == KEYWORD_TYPE_INT:
-                    value = _get_type_int(label, value)
+                    value = _get_type_int(name, label, value)
                 elif itype == KEYWORD_TYPE_FLOAT:
-                    value = _get_type_float(label, value)
+                    value = _get_type_float(name, label, value)
                 elif itype == KEYWORD_TYPE_BOOL:
-                    value = _get_type_bool(label, value)
+                    value = _get_type_bool(name, label, value)
                 elif itype == KEYWORD_TYPE_DATE:
                     keyword2 = KEYWORD_FORMAT
                     date_format = self._get_str(keyword2)
                     date_format = date_format if date_format is not None else DEFAULT_DATE_FORMAT
-                    value = _get_type_date(label, value, date_format)
+                    value = _get_type_date(name, label, value, date_format)
                 elif itype == KEYWORD_TYPE_TIME:
                     keyword2 = KEYWORD_FORMAT
                     time_format = self._get_str(keyword2)
                     time_format = time_format if time_format is not None else DEFAULT_TIME_FORMAT
-                    value = _get_type_time(label, value, time_format)
+                    value = _get_type_time(name, label, value, time_format)
                 elif itype == KEYWORD_TYPE_DATETIME:
                     keyword2 = KEYWORD_FORMAT
                     datetime_format = self._get_str(keyword2)
                     datetime_format = datetime_format if datetime_format is not None else DEFAULT_DATETIME_FORMAT
-                    value = _get_type_datetime(label, value, datetime_format)
+                    value = _get_type_datetime(name, label, value, datetime_format)
                 elif itype == KEYWORD_TYPE_LIST:
                     keyword2 = KEYWORD_SEPARATOR
                     separator = self._get_str(keyword2)
                     separator = separator if separator is not None else DEFAULT_SEPARATOR
-                    value = _get_type_list(label, value, separator)
+                    value = _get_type_list(name, label, value, separator)
                 elif itype == KEYWORD_TYPE_DICT:
-                    value = _get_type_dict(label, value)
+                    value = _get_type_dict(name, label, value)
                 elif itype != KEYWORD_TYPE_ANY:
                     raise SchemaFormatError(ERROR_INVALID_TYPE, {'keyword': keyword, 'itype': itype})
             # -- comprueba si existe un mensaje customizado para un error de tipo
             except SchemaValidationFailure as fail:
-                self._check_error_custom_message(label, fail)
+                self._check_error_custom_message(name, label, fail)
 
         # -- aplica el valor por defecto en su caso
         keyword = KEYWORD_DEFAULT
         defvalue = self._get_obj(keyword)
         if itype is None and defvalue is not None:
             def_itype = util.typeof(defvalue)
             if itype != def_itype:
@@ -170,15 +184,15 @@
         if value is None and defvalue is not None:
             value = defvalue
 
         # -- aplica las funciones de transformación
         keyword = KEYWORD_TO
         tos = self._get_str(keyword)
         if tos is None:
-            tos = 'trim';
+            tos = 'trim'
         tos = tos.split(',')
         for to in tos:
             to = util.trim(to)
             if isinstance(value, str):
                 value = _process_to(keyword, value, to)
             if isinstance(value, list):
                 for (pos, item) in enumerate(value):
@@ -188,58 +202,65 @@
             if isinstance(value, dict):
                 for mkey in value.keys():
                     item = value.get(mkey)
                     if isinstance(item, str):
                         item = _process_to(keyword, item, to)
                         value[mkey] = item
 
+        keyword = KEYWORD_NULL_WHEN_ZERO
+        zero_is_null = self._get_int(keyword)
+        if zero_is_null and ((isinstance(value, str) and str == '0') or
+                             (isinstance(value, int) and value == 0) or
+                             (isinstance(value, float) and value == 0.0)):
+            value = None
+
         # -- comprueba el tipo 'str'
         if isinstance(value, str):
             keyword = KEYWORD_MIN_SIZE
             min_size = self._get_int(keyword)
-            _check_minsize(label, value, min_size)
+            _check_minsize(name, label, value, min_size)
             keyword = KEYWORD_MAX_SIZE
             max_size = self._get_int(keyword)
-            _check_maxsize(label, value, max_size)
+            _check_maxsize(name, label, value, max_size)
             # -- comprueba la cadena en el caso que sea distinta a ''
             if value != '':
                 try:
                     keyword = KEYWORD_REGEXP
                     regexp = self._get_str(keyword)
-                    _check_regexp(label, value, regexp)
+                    _check_regexp(name, label, value, regexp)
                 # -- comprueba si existe un mensaje customizado para un error de formato
                 except SchemaValidationFailure as fail:
-                    self._check_error_custom_message(label, fail)
+                    self._check_error_custom_message(name, label, fail)
 
                 keyword = KEYWORD_WHITE_LIST
                 whitelist = self._get_list(keyword)
                 keyword = KEYWORD_ICASE
                 icase = self._get_bool(keyword)
                 icase = icase if icase is not None else True
-                _check_whitelist(label, value, whitelist, icase)
+                _check_whitelist(name, label, value, whitelist, icase)
                 keyword = KEYWORD_MAX_LINES
                 max_lines = self._get_int(keyword)
-                _check_max_lines(label, value, max_lines)
+                _check_max_lines(name, label, value, max_lines)
             else:
                 value = None
 
         # -- comprueba el tipo 'int' o 'float'
         if isinstance(value, int) or isinstance(value, float):
             keyword = KEYWORD_MIN_SIZE
             min_size = self._get_int(keyword)
-            _check_minsize(label, str(value), min_size)
+            _check_minsize(name, label, str(value), min_size)
             keyword = KEYWORD_MAX_SIZE
             max_size = self._get_int(keyword)
-            _check_maxsize(label, str(value), max_size)
+            _check_maxsize(name, label, str(value), max_size)
             keyword = KEYWORD_MIN_VALUE
             min_value = self._get_int(keyword)
-            _check_minvalue(label, value, min_value)
+            _check_minvalue(name, label, value, min_value)
             keyword = KEYWORD_MAX_VALUE
             max_value = self._get_int(keyword)
-            _check_maxvalue(label, value, max_value)
+            _check_maxvalue(name, label, value, max_value)
 
         # -- comprueba el tipo 'list'
         if isinstance(value, list):
             keyword2 = KEYWORD_IEMPTY
             iempty = self._get_bool(keyword2)
             if iempty:
                 outlist = []
@@ -255,34 +276,63 @@
                 for item in value:
                     if item in outlist:
                         continue
                     outlist.append(item)
                 value = outlist
             keyword = KEYWORD_SCHEMA
             item_schema = self._get_dict(keyword)
-            _check_item_list_schema(label, value, item_schema)
+            if item_schema is not None:
+                schema_validator = SchemaValidator(item_schema)
+                for idx, pitem in enumerate(value):
+                    try:
+                        value[idx] = schema_validator.validate(name, pitem)
+                    except SchemaValidationFailure as ex:
+                        params = ex.get_params()
+                        kname = params.get(KEYWORD_NAME)
+                        params[KEYWORD_NAME] = kname + str(idx)
+                        raise ex
 
         # -- comprueba el tipo 'dict'
         if isinstance(value, dict):
             keyword = KEYWORD_SCHEMA
             item_schema = self._get_dict(keyword)
-            _check_item_dict_schema(label, value, item_schema)
+            keyword = KEYWORD_ONLY_SCHEMA_KEYS
+            only_schema_keys = self._get_bool(keyword)
+            if item_schema is not None:
+                for key in item_schema.keys():
+                    key_schema = item_schema.get(key)
+                    if key_schema is not None:
+                        if not isinstance(key_schema, dict):
+                            _schema_error_schema_expected_for_field(key, label)
+                        fvalue = value.get(key)
+                        val = SchemaValidator(key_schema)
+                        value[key] = val.validate(key, fvalue)
+                    elif only_schema_keys:
+                        _schema_error_schema_expected_for_field(key, label)
+                if only_schema_keys:
+                    for fkey in value.keys():
+                        key_schema = item_schema.get(fkey)
+                        if key_schema is None:
+                            _schema_error_schema_expected_for_field(fkey, label)
+
+            elif only_schema_keys:
+                _schema_error_schema_expected_for_dict(label)
 
         # -- aplica las funciones de casting
         keyword = KEYWORD_CAST
         cast = self._get_dict(keyword)
         if cast is not None:
             validator = SchemaValidator(cast)
             value = validator.validate(name, value)
 
         # -- comprueba si es mandatorio (fuera de comprobación de mensaje específico)
         keyword = KEYWORD_MANDATORY
         mandatory = self._get_bool(keyword)
         if mandatory:
-            _check_mandatory(label, value)
+            _check_mandatory(name, label, value)
         return value
 
     def _get_obj(self, keyword: str):
         return self.data_schema.get(keyword)
 
     def _get_bool(self, keyword: str) -> bool:
         value = self._get_obj(keyword)
@@ -310,15 +360,15 @@
 
     def _get_list(self, keyword: str):
         value = self._get_obj(keyword)
         if value is not None and not isinstance(value, list):
             _schema_error_unexpected_type(keyword, value, KEYWORD_TYPE_LIST)
         return value
 
-    def _check_error_custom_message(self, label: str, fail: SchemaValidationFailure):
+    def _check_error_custom_message(self, name: str, label: str, fail: SchemaValidationFailure):
         keyword = KEYWORD_MESSAGE
         message_map = self._get_obj(keyword)
         if message_map is None:
             raise fail
         if isinstance(message_map, dict):
             message = message_map.get(lang.DEFAULT)
             if message is None:
@@ -326,54 +376,71 @@
             if message is None:
                 message = fail.message
         elif isinstance(message_map, str):
             message = message_map
         else:
             raise fail
         raise SchemaValidationFailure(message, {
-            KEYWORD_NAME: label,
+            KEYWORD_NAME: name,
+            KEYWORD_LABEL: label,
         })
 
 
 def _schema_error_unexpected_type(keyword: str, found_value: any, expected_type: str):
     utype = util.typeof(found_value)
     raise SchemaFormatError(ERROR_UNEXPECTED_TYPE, {'keyword': keyword, 'utype': utype, 'expected_type': expected_type})
 
 
-def _val_error_unexpected_type(name: str, found_value: any, expected_type: str):
+def _schema_error_expected_field_type(key: str, from_dict_label: str):
+    raise SchemaFormatError(ERROR_EXPECTED_FIELD_TYPE, {'field_name': key, 'label': from_dict_label})
+
+
+def _schema_error_schema_expected_for_field(key: str, from_dict_label: str):
+    raise SchemaFormatError(ERROR_SCHEMA_EXPECTED_FOR_FIELD, {'field_name': key, 'label': from_dict_label})
+
+
+def _schema_error_schema_expected_for_dict(dict_label: str):
+    raise SchemaFormatError(ERROR_SCHEMA_EXPECTED_FOR_DICT, {'label': dict_label})
+
+
+def _schema_error_schema_expected_for_item_list(dict_label: str):
+    raise SchemaFormatError(ERROR_SCHEMA_EXPECTED_FOR_ITEM_LIST, {'label': dict_label})
+
+
+def _val_error_unexpected_type(name: str, label: str, found_value: any, expected_type: str):
     utype = util.typeof(found_value)
-    raise SchemaValidationFailure(lang.VAL_ERROR_PARAM_HAS_INVALID_TYPE, {KEYWORD_NAME: name, 'utype': utype, 'expected_type': expected_type})
+    raise SchemaValidationFailure(lang.VAL_ERROR_PARAM_HAS_INVALID_TYPE, {KEYWORD_NAME: name, KEYWORD_LABEL: label, 'utype': utype, 'expected_type': expected_type})
 
 
-def  _format_datetime_format(dformat: str) -> str:
+def _format_datetime_format(dformat: str) -> str:
     dformat = dformat.replace('%Y', 'YYYY')
     dformat = dformat.replace('%m', 'MM')
     dformat = dformat.replace('%d', 'DD')
     dformat = dformat.replace('%H', 'HH')
     dformat = dformat.replace('%M', 'MM')
     dformat = dformat.replace('%S', 'SS')
     return dformat
 
 
-def _val_error_invalid_date_format(name: str, value: any, date_format: str):
+def _val_error_invalid_date_format(name: str, label: str, date_format: str):
     date_format = _format_datetime_format(date_format)
-    raise SchemaValidationFailure(lang.VAL_ERROR_PARAM_DATE_FORMAT, {KEYWORD_NAME: name, 'date_format': date_format})
+    raise SchemaValidationFailure(lang.VAL_ERROR_PARAM_DATE_FORMAT, {KEYWORD_NAME: name, KEYWORD_LABEL: label, 'date_format': date_format})
 
 
-def _val_error_invalid_time_format(name: str, value: any, time_format: str):
+def _val_error_invalid_time_format(name: str, label: str, time_format: str):
     time_format = _format_datetime_format(time_format)
-    raise SchemaValidationFailure(lang.VAL_ERROR_PARAM_TIME_FORMAT, {KEYWORD_NAME: name, 'time_format': time_format})
+    raise SchemaValidationFailure(lang.VAL_ERROR_PARAM_TIME_FORMAT, {KEYWORD_NAME: name, KEYWORD_LABEL: label, 'time_format': time_format})
 
 
-def _val_error_invalid_datetime_format(name: str, value: any, datetime_format: str):
+def _val_error_invalid_datetime_format(name: str, label: str, datetime_format: str):
     datetime_format = _format_datetime_format(datetime_format)
-    raise SchemaValidationFailure(lang.VAL_ERROR_PARAM_DATETIME_FORMAT, {KEYWORD_NAME: name, 'datetime_format': datetime_format})
+    raise SchemaValidationFailure(lang.VAL_ERROR_PARAM_DATETIME_FORMAT, {KEYWORD_NAME: name, KEYWORD_LABEL: label, 'datetime_format': datetime_format})
 
 
-def _get_type_str(name: str, value: any, sformat: str or None, join: str or None) -> str or None:
+def _get_type_str(name: str, label: str, value: any, sformat: str or None, join: str or None) -> str or None:
     if value is None:
         return None
     if isinstance(value, int) or isinstance(value, float) or isinstance(value, bool):
         if sformat is not None:
             return ("{" + sformat + "}").format(value)
         return str(value)
     if isinstance(value, date) or isinstance(value, time) or isinstance(value, datetime):
@@ -385,141 +452,141 @@
             return datetime.combine(datetime.today(), value).strftime(sformat)
         return str(value)
     if isinstance(value, list):
         if join is not None:
             return join.join(value)
         return str(value)
     if not isinstance(value, str):
-        _val_error_unexpected_type(name, value, KEYWORD_TYPE_STR)
+        _val_error_unexpected_type(name, label, value, KEYWORD_TYPE_STR)
     if sformat is not None:
         value = ("{" + sformat + "}").format(value)
     return value
 
 
-def _get_type_int(name: str, value: any) -> int or None:
+def _get_type_int(name: str, label: str, value: any) -> int or None:
     if value is None:
         return None
     if isinstance(value, str):
         value = util.trim(value)
         if value == '':
             return None
         try:
             value = int(value)
         except ValueError:
-            _val_error_unexpected_type(name, value, KEYWORD_TYPE_INT)
+            _val_error_unexpected_type(name, label, value, KEYWORD_TYPE_INT)
     if isinstance(value, float):
         return int(value)
     if not isinstance(value, int):
-        _val_error_unexpected_type(name, value, KEYWORD_TYPE_INT)
+        _val_error_unexpected_type(name, label, value, KEYWORD_TYPE_INT)
     return value
 
 
-def _get_type_float(name: str, value: any) -> int or None:
+def _get_type_float(name: str, label: str, value: any) -> int or None:
     if value is None:
         return None
     if isinstance(value, str):
         value = util.trim(value)
         if value == '':
             return None
         try:
             value = float(value)
         except ValueError:
-            _val_error_unexpected_type(name, value, KEYWORD_TYPE_FLOAT)
+            _val_error_unexpected_type(name, label, value, KEYWORD_TYPE_FLOAT)
     if isinstance(value, int):
         return float(value)
     if not isinstance(value, float):
-        _val_error_unexpected_type(name, value, KEYWORD_TYPE_FLOAT)
+        _val_error_unexpected_type(name, label, value, KEYWORD_TYPE_FLOAT)
     return value
 
 
-def _get_type_bool(name: str, value: any) -> bool or None:
+def _get_type_bool(name: str, label: str, value: any) -> bool or None:
     if value is None:
         return None
     if isinstance(value, str):
         sbool = util.trim(value).lower()
         if sbool == '':
             return None
         if sbool != KEYWORD_BOOL_TRUE and sbool != KEYWORD_BOOL_FALSE:
-            _val_error_unexpected_type(name, value, KEYWORD_TYPE_BOOL)
+            _val_error_unexpected_type(name, label, value, KEYWORD_TYPE_BOOL)
         value = sbool == KEYWORD_BOOL_TRUE
     elif isinstance(value, int) or isinstance(value, float):
         value = value != 0
     elif not isinstance(value, bool):
-        _val_error_unexpected_type(name, value, KEYWORD_TYPE_BOOL)
+        _val_error_unexpected_type(name, label, value, KEYWORD_TYPE_BOOL)
     return value
 
 
-def _get_type_date(name: str, value: any, date_format: str) -> date or None:
+def _get_type_date(name: str, label: str, value: any, date_format: str) -> date or None:
     if value is None:
         return None
     if isinstance(value, date):
         return value
     elif isinstance(value, datetime):
         return value.date()
     elif not isinstance(value, str):
-        _val_error_unexpected_type(name, value, KEYWORD_TYPE_DATE)
+        _val_error_unexpected_type(name, label, value, KEYWORD_TYPE_DATE)
     value = util.trim(value)
     if value == '':
         return None
     try:
         value = datetime.strptime(value, date_format)
     except ValueError:
-        _val_error_invalid_date_format(name, value, date_format)
+        _val_error_invalid_date_format(name, label, date_format)
     return value.date()
 
 
-def _get_type_time(name: str, value: any, time_format: str) -> time or None:
+def _get_type_time(name: str, label: str, value: any, time_format: str) -> time or None:
     if value is None:
         return None
     if isinstance(value, date):
         return value
     elif isinstance(value, datetime):
         return value.time()
     elif not isinstance(value, str):
-        _val_error_unexpected_type(name, value, KEYWORD_TYPE_TIME)
+        _val_error_unexpected_type(name, label, value, KEYWORD_TYPE_TIME)
     value = util.trim(value)
     if value == '':
         return None
     try:
         value = datetime.strptime(value, time_format)
     except ValueError:
-        _val_error_invalid_time_format(name, value, time_format)
+        _val_error_invalid_time_format(name, label, time_format)
     return value.time()
 
 
-def _get_type_datetime(name: str, value: any, datetime_format: str) -> date or None:
+def _get_type_datetime(name: str, label: str, value: any, datetime_format: str) -> date or None:
     if value is None:
         return None
     if isinstance(value, datetime):
         return value
     elif isinstance(value, date):
         return datetime.combine(value, datetime.min.time())
     elif not isinstance(value, str):
-        _val_error_unexpected_type(name, value, KEYWORD_TYPE_DATETIME)
+        _val_error_unexpected_type(name, label, value, KEYWORD_TYPE_DATETIME)
     value = util.trim(value)
     if value == '':
         return None
     try:
         value = datetime.strptime(value, datetime_format)
     except ValueError:
-        _val_error_invalid_datetime_format(name, value, datetime_format)
+        _val_error_invalid_datetime_format(name, label, datetime_format)
     return value
 
 
-def _get_type_list(name: str, value: any, separator: str) -> list or None:
+def _get_type_list(name: str, label: str, value: any, separator: str) -> list or None:
     if value is None:
         return None
     if isinstance(value, str):
         return value.split(separator)
     elif not isinstance(value, list):
-        _val_error_unexpected_type(name, value, KEYWORD_TYPE_LIST)
+        _val_error_unexpected_type(name, label, value, KEYWORD_TYPE_LIST)
     return value
 
 
-def _get_type_dict(name: str, value: any) -> dict or None:
+def _get_type_dict(name: str, label: str, value: any) -> dict or None:
     if value is None:
         return None
     if isinstance(value, str):
         value = util.trim(value)
         if value == '':
             return None
         try:
@@ -527,17 +594,17 @@
         except json.decoder.JSONDecodeError:
             value = value.replace('\"', '<dquote>')
             value = value.replace('\'', '\"')
             value = value.replace('<dquote>', '\'')
             try:
                 value = json.loads(value)
             except json.decoder.JSONDecodeError:
-                _val_error_unexpected_type(name, value, KEYWORD_TYPE_DICT)
+                _val_error_unexpected_type(name, label, value, KEYWORD_TYPE_DICT)
     if not isinstance(value, dict):
-        _val_error_unexpected_type(name, value, KEYWORD_TYPE_DICT)
+        _val_error_unexpected_type(name, label, value, KEYWORD_TYPE_DICT)
     return value
 
 
 def _process_to(keyword: str, value: any, func_name: str) -> str:
     if func_name == KEYWORD_TO_FUNC_LOWER:
         return value.lower()
     if func_name == KEYWORD_TO_FUNC_UPPER:
@@ -545,88 +612,63 @@
     if func_name == KEYWORD_TO_FUNC_NO_TRIM:
         return value
     if func_name == KEYWORD_TO_FUNC_TRIM:
         return util.trim(value)
     raise SchemaFormatError(ERROR_INVALID_FUNCTION_NAME, {'keyword': keyword, 'func_name': func_name})
 
 
-def _check_mandatory(name: str, value: any):
+def _check_mandatory(name: str, label: str, value: any):
     if value is None or (isinstance(value, str) and len(value) == 0):
-        raise SchemaValidationFailure(lang.VAL_ERROR_PARAM_IS_MANDATORY, {KEYWORD_NAME: name})
+        raise SchemaValidationFailure(lang.VAL_ERROR_PARAM_IS_MANDATORY, {KEYWORD_NAME: name, KEYWORD_LABEL: label})
 
 
-def _check_regexp(name: str, value: str, pattern_to_match: str):
+def _check_regexp(name: str, label: str, value: str, pattern_to_match: str):
     if value is not None and len(value) > 0 and pattern_to_match is not None:
         regex = re.compile(pattern_to_match, re.I)
         match = regex.match(str(value))
         if not bool(match):
-            raise SchemaValidationFailure(lang.VAL_ERROR_PARAM_HAS_INVALID_FORMAT, {KEYWORD_NAME: name})
+            raise SchemaValidationFailure(lang.VAL_ERROR_PARAM_HAS_INVALID_FORMAT, {KEYWORD_NAME: name, KEYWORD_LABEL: label})
 
 
-def _check_minsize(name: str, value: str, minsize: int or None):
+def _check_minsize(name: str, label: str, value: str, minsize: int or None):
     slen = len(util.trim(value))
     if value is not None and minsize is not None and slen < minsize:
-        raise SchemaValidationFailure(lang.VAL_ERROR_PARAM_IS_TOO_SHORT, {KEYWORD_NAME: name, 'minsize': minsize})
+        raise SchemaValidationFailure(lang.VAL_ERROR_PARAM_IS_TOO_SHORT, {KEYWORD_NAME: name, KEYWORD_LABEL: label, 'minsize': minsize})
 
 
-def _check_maxsize(name: str, value: str, maxsize: int or None):
+def _check_maxsize(name: str, label: str, value: str, maxsize: int or None):
     slen = len(util.trim(value))
     if value is not None and maxsize is not None and slen > maxsize:
-        raise SchemaValidationFailure(lang.VAL_ERROR_PARAM_IS_TOO_LARGE, {KEYWORD_NAME: name, 'maxsize': maxsize})
+        raise SchemaValidationFailure(lang.VAL_ERROR_PARAM_IS_TOO_LARGE, {KEYWORD_NAME: name, KEYWORD_LABEL: label, 'maxsize': maxsize})
 
 
-def _check_minvalue(name: str, value: any, minvalue: any):
+def _check_minvalue(name: str, label: str, value: any, minvalue: any):
     if value is not None and minvalue is not None and value < minvalue:
-        raise SchemaValidationFailure(lang.VAL_ERROR_PARAM_IS_TOO_SMALL, {KEYWORD_NAME: name, 'minvalue': minvalue})
+        raise SchemaValidationFailure(lang.VAL_ERROR_PARAM_IS_TOO_SMALL, {KEYWORD_NAME: name, KEYWORD_LABEL: label, 'minvalue': minvalue})
 
 
-def _check_maxvalue(name: str, value: any, maxvalue: any):
+def _check_maxvalue(name: str, label: str, value: any, maxvalue: any):
     if value is not None and maxvalue is not None and value > maxvalue:
-        raise SchemaValidationFailure(lang.VAL_ERROR_PARAM_IS_TOO_BIG, {KEYWORD_NAME: name, 'maxvalue': maxvalue})
-
-
-def _check_item_list_schema(name: str, plist: list, item_schema: dict):
-    if item_schema is not None:
-        schema_validator = SchemaValidator(item_schema)
-        for pitem in plist:
-            try:
-                schema_validator.validate('item list', pitem)
-            except SchemaValidationFailure as ex:
-                raise SchemaValidationFailure(lang.VAL_ERROR_LIST_ITEM_HAS_INVALID_ELEMENT, {KEYWORD_NAME: name, 'message': ex.get_message()})
-
-
-def _check_item_dict_schema(name: str, pdict: dict, item_schema: dict):
-    if item_schema is not None:
-        for pitem in pdict.keys():
-            schema = item_schema.get(pitem)
-            if schema is None:
-                raise SchemaValidationFailure(lang.VAL_ERROR_DICT_ITEM_HAS_NOT_DEFINED_DATA_VALIDATION, {KEYWORD_NAME: name})
-        for pkey, schema in item_schema.items():
-            schema_validator = SchemaValidator(schema)
-            pvalue = pdict.get(pkey)
-            try:
-                schema_validator.validate(pkey, pvalue)
-            except SchemaValidationFailure as ex:
-                raise SchemaValidationFailure(lang.VAL_ERROR_DICT_ITEM_HAS_INVALID_ELEMENT, {KEYWORD_NAME: name, 'message': ex.get_message()})
+        raise SchemaValidationFailure(lang.VAL_ERROR_PARAM_IS_TOO_BIG, {KEYWORD_NAME: name, KEYWORD_LABEL: label, 'maxvalue': maxvalue})
 
 
-def _check_whitelist(name: str, value: any, whitelist: list, icase: bool = True):
+def _check_whitelist(name: str, label: str, value: any, whitelist: list, icase: bool = True):
     if whitelist is None:
         return
     if icase:
-        value = str(value).lower()
+        ivalue = str(value).lower()
         for pitem in whitelist:
-            if str(pitem).lower() == value:
+            if str(pitem).lower() == ivalue:
                 return
     else:
         for pitem in whitelist:
             if pitem == value:
                 return
-    raise SchemaValidationFailure(lang.VAL_ERROR_PARAM_HAS_INVALID_VALUE, {KEYWORD_NAME: name})
+    raise SchemaValidationFailure(lang.VAL_ERROR_PARAM_HAS_INVALID_VALUE, {KEYWORD_NAME: name, KEYWORD_LABEL: label, KEYWORD_VALUE: str(value)})
 
 
-def _check_max_lines(name: str, value: any, max_lines: int):
+def _check_max_lines(name: str, label: str, value: any, max_lines: int):
     if max_lines is not None and max_lines > 0:
         total_nl = util.trim(value).count('\n') + 1
         if total_nl > max_lines:
-            raise SchemaValidationFailure(lang.VAL_ERROR_PARAM_HAS_TOO_MUCH_LINES, {KEYWORD_NAME: name, 'maxlines': max_lines})
+            raise SchemaValidationFailure(lang.VAL_ERROR_PARAM_HAS_TOO_MUCH_LINES, {KEYWORD_NAME: name, KEYWORD_LABEL: label, 'maxlines': max_lines})
```

### Comparing `dataskema-1.6.7/dataskema.egg-info/PKG-INFO` & `dataskema-1.7.0/dataskema.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 Metadata-Version: 2.1
 Name: dataskema
-Version: 1.6.7
+Version: 1.7.0
 Summary: Data schema to validate parameters easily, quickly and with minimal code
 Home-page: https://github.com/lagor-github/dataskema
-Author: Luis A. González Rivas
+Author: Luis A. González
 Author-email: lagor55@gmail.com
 License: MIT
 Description: # `dataskema`
         Data schema validation for python
         
+        v1.7.0
+        - Now dict types can have schema in its fields using 'schema' keyword
+        - Use 'only-schema-keys' keyword to reject no declareted fields
+        - New 'null-when-zero' keyword that rewrites incoming value to None value when zero (number or string)
+        - Some minor bugs fixed
+        
         v1.6.7
         - Bug fixed in @dataskema.flask_url
         
         v1.6.6
         - Schemas for 'dict' types fields
         - 'max-size' and 'min-size' are valid for 'int' and 'float' types
```

### Comparing `dataskema-1.6.7/setup.py` & `dataskema-1.7.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 with open("README.md", "r") as fh:
     readme_description = fh.read()
 
 setup(
     name='dataskema',
     packages=['dataskema', 'dataskema.decorators'],
     include_package_data=True,  # -- para que se incluyan archivos sin extension .py
-    version='1.6.7',
+    version='1.7.0',
     description='Data schema to validate parameters easily, quickly and with minimal code',
     long_description=readme_description,
     long_description_content_type="text/markdown",
     zip_safe=False,
     install_requires=[
         'flask',
     ],
-    author='Luis A. González Rivas',
+    author='Luis A. González',
     author_email="lagor55@gmail.com",
     license="MIT",
     url="https://github.com/lagor-github/dataskema",
     classifiers=["Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Development Status :: 5 - Production/Stable", "Intended Audience :: Developers",
         "Operating System :: OS Independent"],
```

