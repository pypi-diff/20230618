# Comparing `tmp/tika_client-0.1.0.tar.gz` & `tmp/tika_client-0.1.1.tar.gz`

## Comparing `tika_client-0.1.0.tar` & `tika_client-0.1.1.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 tika_client-0.1.0/.editorconfig
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 tika_client-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 tika_client-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 tika_client-0.1.0/.docker/docker-compose.ci-test.yml
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 tika_client-0.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 tika_client-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 tika_client-0.1.0/.github/workflows/codeql.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tika_client-0.1.0/src/tika_client/__about__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 tika_client-0.1.0/src/tika_client/__init__.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tika_client-0.1.0/src/tika_client/_constants.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 tika_client-0.1.0/src/tika_client/_resource_meta.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 tika_client-0.1.0/src/tika_client/_resource_recursive.py
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 tika_client-0.1.0/src/tika_client/_resource_tika.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 tika_client-0.1.0/src/tika_client/_types.py
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 tika_client-0.1.0/src/tika_client/_utils.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 tika_client-0.1.0/src/tika_client/client.py
--rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 tika_client-0.1.0/src/tika_client/data_models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tika_client-0.1.0/src/tika_client/py.typed
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/test_image_files.py
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/test_resource_metadata.py
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/test_resource_recursive_metadata.py
--rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/test_resource_tika.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/samples/README.md
--rw-r--r--   0        0        0    14164 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/samples/microsoft-sample.docx
--rw-r--r--   0        0        0     8843 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/samples/sample-spreadsheet.ods
--rw-r--r--   0        0        0     4743 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/samples/sample-spreadsheet.xlsx
--rw-r--r--   0        0        0    23552 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/samples/sample.doc
--rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/samples/sample.docx
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/samples/sample.html
--rw-r--r--   0        0        0   189116 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/samples/sample.jpg
--rw-r--r--   0        0        0     8271 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/samples/sample.odt
--rw-r--r--   0        0        0   980209 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/samples/sample.png
--rw-r--r--   0        0        0   936200 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/samples/test-document-images.odt
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 tika_client-0.1.0/.gitignore
--rw-r--r--   0        0        0    34670 2020-02-02 00:00:00.000000 tika_client-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 tika_client-0.1.0/README.md
--rw-r--r--   0        0        0     3920 2020-02-02 00:00:00.000000 tika_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 tika_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 tika_client-0.1.1/.editorconfig
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 tika_client-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 tika_client-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 tika_client-0.1.1/TODO.md
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 tika_client-0.1.1/.docker/docker-compose.ci-test.yml
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 tika_client-0.1.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 tika_client-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 tika_client-0.1.1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tika_client-0.1.1/src/tika_client/__about__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 tika_client-0.1.1/src/tika_client/__init__.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tika_client-0.1.1/src/tika_client/_constants.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 tika_client-0.1.1/src/tika_client/_resource_meta.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 tika_client-0.1.1/src/tika_client/_resource_recursive.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 tika_client-0.1.1/src/tika_client/_resource_tika.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 tika_client-0.1.1/src/tika_client/_types.py
+-rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 tika_client-0.1.1/src/tika_client/_utils.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 tika_client-0.1.1/src/tika_client/client.py
+-rw-r--r--   0        0        0     4251 2020-02-02 00:00:00.000000 tika_client-0.1.1/src/tika_client/data_models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tika_client-0.1.1/src/tika_client/py.typed
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/test_image_files.py
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/test_resource_metadata.py
+-rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/test_resource_recursive_metadata.py
+-rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/test_resource_tika.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/samples/README.md
+-rw-r--r--   0        0        0    14164 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/samples/microsoft-sample.docx
+-rw-r--r--   0        0        0     8843 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/samples/sample-spreadsheet.ods
+-rw-r--r--   0        0        0     4743 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/samples/sample-spreadsheet.xlsx
+-rw-r--r--   0        0        0    23552 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/samples/sample.doc
+-rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/samples/sample.docx
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/samples/sample.html
+-rw-r--r--   0        0        0   189116 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/samples/sample.jpg
+-rw-r--r--   0        0        0     8271 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/samples/sample.odt
+-rw-r--r--   0        0        0   980209 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/samples/sample.png
+-rw-r--r--   0        0        0   936200 2020-02-02 00:00:00.000000 tika_client-0.1.1/tests/samples/test-document-images.odt
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 tika_client-0.1.1/.gitignore
+-rw-r--r--   0        0        0    34670 2020-02-02 00:00:00.000000 tika_client-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 tika_client-0.1.1/README.md
+-rw-r--r--   0        0        0     3920 2020-02-02 00:00:00.000000 tika_client-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 tika_client-0.1.1/PKG-INFO
```

### Comparing `tika_client-0.1.0/.editorconfig` & `tika_client-0.1.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.0/.pre-commit-config.yaml` & `tika_client-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.0/CHANGELOG.md` & `tika_client-0.1.1/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.1.1] - 2023-06-18
+
+### Fixed
+
+- Fixes an incorrect key when parsing new content types
+- Fixed handling of message/rfc822 content type documents
+
 ## [0.1.0] - 2023-06-17
 
 ### Changed
 
 - Further refinements to the Tika response data models
 
 ### Added
```

### Comparing `tika_client-0.1.0/.github/dependabot.yml` & `tika_client-0.1.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.0/.github/workflows/ci.yml` & `tika_client-0.1.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.0/.github/workflows/codeql.yml` & `tika_client-0.1.1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.0/src/tika_client/_resource_meta.py` & `tika_client-0.1.1/src/tika_client/_resource_meta.py`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.0/src/tika_client/_resource_recursive.py` & `tika_client-0.1.1/src/tika_client/_resource_recursive.py`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.0/src/tika_client/_resource_tika.py` & `tika_client-0.1.1/src/tika_client/_resource_tika.py`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.0/src/tika_client/_utils.py` & `tika_client-0.1.1/src/tika_client/_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 import logging
 from pathlib import Path
 from typing import Dict
-from typing import Union
 
 from httpx import Client
 
 from tika_client._constants import MIN_COMPRESS_LEN
 from tika_client._types import MimeType
 from tika_client._types import RequestContent
-from tika_client.data_models import DOCUMENT_TYPES
-from tika_client.data_models import IMAGE_TYPES
-from tika_client.data_models import ParsedDocument
-from tika_client.data_models import ParsedImage
+from tika_client.data_models import KNOWN_CONTENT_TYPES
 from tika_client.data_models import TikaKey
 from tika_client.data_models import TikaResponse
 
 logger = logging.getLogger("tika-client.utils")
 
 
 class BaseResource:
@@ -65,20 +61,18 @@
             headers["Content-Type"] = mime_type
 
         resp = self.client.put(endpoint, content=content_bytes, headers=headers)
         resp.raise_for_status()
         return resp.json()
 
     @staticmethod
-    def _decoded_response(resp_json: Dict) -> Union[ParsedDocument, ParsedImage, TikaResponse]:
+    def _decoded_response(resp_json: Dict):
         """
         If possible, returns a more detailed class with properties that appear often in this
         mime type.  Otherwise, it's a basically raw data response, but with some helpers
         for processing fields into Python types
         """
-        if resp_json[TikaKey.ContentType] in IMAGE_TYPES:
-            return ParsedImage(resp_json)
-        elif resp_json[TikaKey.ContentType] in DOCUMENT_TYPES:
-            return ParsedDocument(resp_json)
+        if resp_json[TikaKey.ContentType] in KNOWN_CONTENT_TYPES:
+            return KNOWN_CONTENT_TYPES[resp_json[TikaKey.ContentType]](resp_json)
         else:
-            logger.warning(f"Unknown content-type: {resp_json[TikaKey.ContentLength]}")
+            logger.warning(f"Under-specified content-type: {resp_json[TikaKey.ContentType]}")
             return TikaResponse(resp_json)
```

### Comparing `tika_client-0.1.0/src/tika_client/client.py` & `tika_client-0.1.1/src/tika_client/client.py`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.0/src/tika_client/data_models.py` & `tika_client-0.1.1/src/tika_client/data_models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from datetime import datetime
 from enum import Enum
 from typing import Dict
 from typing import Final
 from typing import List
 from typing import Optional
-from typing import Set
+from typing import Type
 from typing import Union
 
 
 class TikaKey(str, Enum):
     Parsers = "X-TIKA:Parsed-By"
     ContentType = "Content-Type"
     ContentLength = "Content-Length"
     Content = "X-TIKA:content"
     Created = "dcterms:created"
     Modified = "dcterms:modified"
+    Title = "dc:title"
+    Subject = "dc:subject"
 
 
 class TikaResponse:
     """
     A basic response from the API.  It sets fields which the response
     always appears to have, and some small helpers for getting and converting
     other data types, including handling the chance those don't exist in the response.
@@ -105,15 +107,38 @@
 class ParsedImage(TikaResponse):
     """
     Properties which seem to be returned for image like
     parsing
     """
 
 
-IMAGE_TYPES: Final[Set[str]] = {"image/png", "image/jpeg", "image/webp"}
-DOCUMENT_TYPES: Final[Set[str]] = {
-    "application/vnd.oasis.opendocument.text",
-    "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
-    "application/vnd.oasis.opendocument.spreadsheet",
-    "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet",
-    "application/msword",
+class ParsedEmail(TikaResponse):
+    """
+    Properties for .eml files
+    """
+
+    @property
+    def subject(self):
+        return self.get_optional_string(TikaKey.Subject)
+
+    @property
+    def title(self):
+        return self.get_optional_string(TikaKey.Title)
+
+    @property
+    def content(self) -> Optional[str]:
+        return self.get_optional_string(TikaKey.Content)
+
+
+KNOWN_CONTENT_TYPES: Final[
+    Dict[str, Union[Type[ParsedDocument], Type[ParsedImage], Type[ParsedEmail], Type[TikaResponse]]]
+] = {
+    "application/vnd.oasis.opendocument.text": ParsedDocument,
+    "application/vnd.openxmlformats-officedocument.wordprocessingml.document": ParsedDocument,
+    "application/vnd.oasis.opendocument.spreadsheet": ParsedDocument,
+    "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet": ParsedDocument,
+    "application/msword": ParsedDocument,
+    "image/png": ParsedImage,
+    "image/jpeg": ParsedImage,
+    "image/webp": ParsedImage,
+    "message/rfc822": ParsedEmail,
 }
```

### Comparing `tika_client-0.1.0/tests/conftest.py` & `tika_client-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.0/tests/test_image_files.py` & `tika_client-0.1.1/tests/test_image_files.py`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.0/tests/test_resource_metadata.py` & `tika_client-0.1.1/tests/test_resource_metadata.py`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.0/tests/test_resource_recursive_metadata.py` & `tika_client-0.1.1/tests/test_resource_recursive_metadata.py`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.0/tests/test_resource_tika.py` & `tika_client-0.1.1/tests/test_resource_tika.py`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.0/tests/samples/microsoft-sample.docx` & `tika_client-0.1.1/tests/samples/microsoft-sample.docx`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.0/tests/samples/sample-spreadsheet.ods` & `tika_client-0.1.1/tests/samples/sample-spreadsheet.ods`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.0/tests/samples/sample-spreadsheet.xlsx` & `tika_client-0.1.1/tests/samples/sample-spreadsheet.xlsx`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.0/tests/samples/sample.doc` & `tika_client-0.1.1/tests/samples/sample.doc`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.0/tests/samples/sample.docx` & `tika_client-0.1.1/tests/samples/sample.docx`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.0/tests/samples/sample.jpg` & `tika_client-0.1.1/tests/samples/sample.jpg`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.0/tests/samples/sample.odt` & `tika_client-0.1.1/tests/samples/sample.odt`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.0/tests/samples/sample.png` & `tika_client-0.1.1/tests/samples/sample.png`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.0/tests/samples/test-document-images.odt` & `tika_client-0.1.1/tests/samples/test-document-images.odt`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.0/.gitignore` & `tika_client-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.0/LICENSE.txt` & `tika_client-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.0/README.md` & `tika_client-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 ---
 
 **Table of Contents**
 
 - [Features](#features)
 - [Installation](#installation)
 - [Usage](#usage)
+- [Why](#why)
 - [License](#license)
 
 ## Features
 
 - Simplified: No need to worry about XML or JSON responses, downloading a Tika jar file or Python 2
 - Support for Tika 2+ only
 - Based on the modern [httpx](https://github.com/encode/httpx) library
```

### Comparing `tika_client-0.1.0/pyproject.toml` & `tika_client-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tika_client-0.1.0/PKG-INFO` & `tika_client-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tika-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: A modern REST client for Apache Tika server
 Project-URL: Documentation, https://github.com/stumpylog/tika-rest-client#readme
 Project-URL: Issues, https://github.com/stumpylog/tika-rest-client/issues
 Project-URL: Source, https://github.com/stumpylog/tika-rest-client
 Author-email: Trenton H <797416+stumpylog@users.noreply.github.com>
 License-Expression: GPL-3.0-only
 License-File: LICENSE.txt
@@ -29,14 +29,15 @@
 ---
 
 **Table of Contents**
 
 - [Features](#features)
 - [Installation](#installation)
 - [Usage](#usage)
+- [Why](#why)
 - [License](#license)
 
 ## Features
 
 - Simplified: No need to worry about XML or JSON responses, downloading a Tika jar file or Python 2
 - Support for Tika 2+ only
 - Based on the modern [httpx](https://github.com/encode/httpx) library
```

