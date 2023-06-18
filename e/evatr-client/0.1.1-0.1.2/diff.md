# Comparing `tmp/evatr-client-0.1.1.tar.gz` & `tmp/evatr-client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evatr-client-0.1.1.tar", last modified: Sat Jun 17 17:28:13 2023, max compression
+gzip compressed data, was "evatr-client-0.1.2.tar", last modified: Sun Jun 18 20:33:36 2023, max compression
```

## Comparing `evatr-client-0.1.1.tar` & `evatr-client-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 cedricaltermatt   (501) staff       (20)        0 2023-06-17 17:28:13.710950 evatr-client-0.1.1/
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)     1068 2023-06-16 08:34:10.000000 evatr-client-0.1.1/LICENSE.txt
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)      863 2023-06-17 17:28:13.711135 evatr-client-0.1.1/PKG-INFO
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)     3202 2023-06-16 21:31:12.000000 evatr-client-0.1.1/README.md
-drwxr-xr-x   0 cedricaltermatt   (501) staff       (20)        0 2023-06-17 17:28:13.708111 evatr-client-0.1.1/evatr_client/
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)      171 2023-06-16 17:00:00.000000 evatr-client-0.1.1/evatr_client/__init__.py
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)     6127 2023-06-17 17:26:31.000000 evatr-client-0.1.1/evatr_client/client.py
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)     4532 2023-06-17 16:38:13.000000 evatr-client-0.1.1/evatr_client/status_codes.py
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)     5905 2023-06-17 17:01:59.000000 evatr-client-0.1.1/evatr_client/util.py
-drwxr-xr-x   0 cedricaltermatt   (501) staff       (20)        0 2023-06-17 17:28:13.710505 evatr-client-0.1.1/evatr_client.egg-info/
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)      863 2023-06-17 17:28:13.000000 evatr-client-0.1.1/evatr_client.egg-info/PKG-INFO
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)      317 2023-06-17 17:28:13.000000 evatr-client-0.1.1/evatr_client.egg-info/SOURCES.txt
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)        1 2023-06-17 17:28:13.000000 evatr-client-0.1.1/evatr_client.egg-info/dependency_links.txt
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)       32 2023-06-17 17:28:13.000000 evatr-client-0.1.1/evatr_client.egg-info/requires.txt
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)       13 2023-06-17 17:28:13.000000 evatr-client-0.1.1/evatr_client.egg-info/top_level.txt
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)       79 2023-06-17 17:28:13.711831 evatr-client-0.1.1/setup.cfg
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)     1221 2023-06-17 17:27:11.000000 evatr-client-0.1.1/setup.py
+drwxr-xr-x   0 cedricaltermatt   (501) staff       (20)        0 2023-06-18 20:33:36.533229 evatr-client-0.1.2/
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)     1068 2023-06-16 08:34:10.000000 evatr-client-0.1.2/LICENSE.txt
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)      863 2023-06-18 20:33:36.533398 evatr-client-0.1.2/PKG-INFO
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)     3366 2023-06-18 20:29:03.000000 evatr-client-0.1.2/README.md
+drwxr-xr-x   0 cedricaltermatt   (501) staff       (20)        0 2023-06-18 20:33:36.530634 evatr-client-0.1.2/evatr_client/
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)      171 2023-06-16 17:00:00.000000 evatr-client-0.1.2/evatr_client/__init__.py
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)     6120 2023-06-18 20:21:06.000000 evatr-client-0.1.2/evatr_client/client.py
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)     4532 2023-06-17 16:38:13.000000 evatr-client-0.1.2/evatr_client/status_codes.py
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)     5913 2023-06-18 20:25:16.000000 evatr-client-0.1.2/evatr_client/util.py
+drwxr-xr-x   0 cedricaltermatt   (501) staff       (20)        0 2023-06-18 20:33:36.532921 evatr-client-0.1.2/evatr_client.egg-info/
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)      863 2023-06-18 20:33:36.000000 evatr-client-0.1.2/evatr_client.egg-info/PKG-INFO
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)      317 2023-06-18 20:33:36.000000 evatr-client-0.1.2/evatr_client.egg-info/SOURCES.txt
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)        1 2023-06-18 20:33:36.000000 evatr-client-0.1.2/evatr_client.egg-info/dependency_links.txt
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)       32 2023-06-18 20:33:36.000000 evatr-client-0.1.2/evatr_client.egg-info/requires.txt
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)       13 2023-06-18 20:33:36.000000 evatr-client-0.1.2/evatr_client.egg-info/top_level.txt
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)       79 2023-06-18 20:33:36.534039 evatr-client-0.1.2/setup.cfg
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)     1221 2023-06-18 20:32:26.000000 evatr-client-0.1.2/setup.py
```

### Comparing `evatr-client-0.1.1/LICENSE.txt` & `evatr-client-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evatr-client-0.1.1/PKG-INFO` & `evatr-client-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: evatr-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: A client for: https://evatr.bff-online.de/eVatR/
 Home-page: https://github.com/CeeDiii/evatr-client
-Download-URL: https://github.com/CeeDiii/evatr-client/archive/refs/tags/v0.1.1.tar.gz
+Download-URL: https://github.com/CeeDiii/evatr-client/archive/refs/tags/v0.1.2.tar.gz
 Author: CeeDiii
 License: MIT
 Keywords: python,uid,vat,uid prüfung,vat validation,evatr,evatr client,evatr python client
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `evatr-client-0.1.1/README.md` & `evatr-client-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,21 @@
 
 You can scrape the error codes with the script `scripts/scrape_status_codes.py`. The script has to be executed from the project root directory:
 
 ```shell
 $ python scripts/scrape_status_codes.py
 ```
 
+## Testing 
+To get the actual test results, execute the following command from the root project directory:
+
+```shell
+$ python -m unittest tests/test_client.py
+```
+
 ## Contributing 
 Feel free to open issues and pull requests in this repo.
 
 ## License MIT
 Copyright © 2023 CeeDiii
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `evatr-client-0.1.1/evatr_client/client.py` & `evatr-client-0.1.2/evatr_client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import requests
 
 from dataclasses import asdict
 from typing import Dict
 from urllib.parse import urlencode
 from xml.etree.ElementTree import fromstring
 
-from .util import ISimpleParams, IQualifiedParams, ISimpleResult, IQualifiedResult, _get_error_description, _get_result_description
+from .util import ISimpleParams, IQualifiedParams, ISimpleResult, IQualifiedResult, get_error_description, get_result_description
 
 class EvatrClient:
     '''
     A client for making requests to the eVatR service and parsing the XML responses.
 
     This client provides methods to retrieve XML data from the eVatR RPC-API and parse the responses into simple or qualified result objects.
     
@@ -99,15 +99,15 @@
         result_street = response['Erg_Str']
 
         result = ISimpleResult(
             valid=error_code == 200,
             date=response['Datum'],
             time=response['Uhrzeit'],
             error_code=response['ErrorCode'],
-            error_description=_get_error_description(error_code),
+            error_description=get_error_description(error_code),
             own_vat_number=response['UstId_1'],
             validated_vat_number=response['UstId_2'],
             valid_from=response['Gueltig_ab'],
             valid_until=response['Gueltig_bis'],
             raw_xml=raw_xml if include_raw_xml else None
         )
 
@@ -118,18 +118,18 @@
                 city=response['Ort'],
                 zip=response['PLZ'],
                 street=response['Strasse'],
                 result_name=result_name,
                 result_city=result_city,
                 result_zip=result_zip,
                 result_street=result_street,
-                result_name_description=_get_result_description(result_name),
-                result_city_description=_get_result_description(result_city),
-                result_zip_description=_get_result_description(result_zip),
-                result_street_description=_get_result_description(result_street)
+                result_name_description=get_result_description(result_name),
+                result_city_description=get_result_description(result_city),
+                result_zip_description=get_result_description(result_zip),
+                result_street_description=get_result_description(result_street)
             )
 
         return result
 
 
     def check_simple(self, params: ISimpleParams):
         '''
```

### Comparing `evatr-client-0.1.1/evatr_client/status_codes.py` & `evatr-client-0.1.2/evatr_client/status_codes.py`

 * *Files identical despite different names*

### Comparing `evatr-client-0.1.1/evatr_client/util.py` & `evatr-client-0.1.2/evatr_client/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     result_zip: Optional[ResultType] = ResultType.NOT_QUERIED
     result_street: Optional[ResultType] = ResultType.NOT_QUERIED
     result_name_description: Optional[str] = None
     result_city_description: Optional[str] = None
     result_zip_description: Optional[str] = None
     result_street_description: Optional[str] = None
 
-def _get_result_description(result_type):
+def get_result_description(result_type):
     '''
     Get the description for a specific result type.
 
     Args:
         result_type (ResultType): The result type.
 
     Returns:
@@ -141,21 +141,21 @@
     elif result_type == ResultType.NOT_QUERIED:
         return 'nicht angefragt'
     elif result_type == ResultType.NOT_RETURNED:
         return 'vom EU-Mitgliedsstaat nicht mitgeteilt'
     else:
         return None
     
-def _get_error_description(error_code: int):
+def get_error_description(error_code: int):
     '''
     Get the description for a specific error code.
 
     Args:
         error_code (int): The error code.
 
     Returns:
         str: The description of the error code.
 
     '''
-    if error_code in status_codes:
-       return status_codes[error_code]
+    if str(error_code) in status_codes:
+       return status_codes[str(error_code)]
     return 'Description not found for the given code.'
```

### Comparing `evatr-client-0.1.1/evatr_client.egg-info/PKG-INFO` & `evatr-client-0.1.2/evatr_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: evatr-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: A client for: https://evatr.bff-online.de/eVatR/
 Home-page: https://github.com/CeeDiii/evatr-client
-Download-URL: https://github.com/CeeDiii/evatr-client/archive/refs/tags/v0.1.1.tar.gz
+Download-URL: https://github.com/CeeDiii/evatr-client/archive/refs/tags/v0.1.2.tar.gz
 Author: CeeDiii
 License: MIT
 Keywords: python,uid,vat,uid prüfung,vat validation,evatr,evatr client,evatr python client
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `evatr-client-0.1.1/setup.py` & `evatr-client-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 DESCRIPTION = 'A client for: https://evatr.bff-online.de/eVatR/'
 LONG_DESCRIPTION = 'A client to validate EU-VAT numbers with the official German tool that can be found here: https://evatr.bff-online.de/eVatR/'
 
 # Setting up
 setup(
     name="evatr-client",
     version=VERSION,
     author="CeeDiii",
     description=DESCRIPTION,
     license='MIT',
     url='https://github.com/CeeDiii/evatr-client',
-    download_url='https://github.com/CeeDiii/evatr-client/archive/refs/tags/v0.1.1.tar.gz',
+    download_url='https://github.com/CeeDiii/evatr-client/archive/refs/tags/v0.1.2.tar.gz',
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     keywords=['python', 'uid', 'vat', 'uid prüfung', 'vat validation', 'evatr', 'evatr client', 'evatr python client'],
     python_requires=">=3.10",
     install_requires=[
           'requests',
```

