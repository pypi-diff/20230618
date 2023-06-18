# Comparing `tmp/tika_client-0.0.3.tar.gz` & `tmp/tika_client-0.1.0.tar.gz`

## Comparing `tika_client-0.0.3.tar` & `tika_client-0.1.0.tar`

### file list

```diff
@@ -1,35 +1,40 @@
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 tika_client-0.0.3/.editorconfig
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 tika_client-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 tika_client-0.0.3/CHANGELOG.md
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 tika_client-0.0.3/.docker/docker-compose.ci-test.yml
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 tika_client-0.0.3/.github/dependabot.yml
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 tika_client-0.0.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 tika_client-0.0.3/.github/workflows/codeql.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tika_client-0.0.3/src/tika_client/__about__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 tika_client-0.0.3/src/tika_client/__init__.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tika_client-0.0.3/src/tika_client/_constants.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 tika_client-0.0.3/src/tika_client/_resource_meta.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 tika_client-0.0.3/src/tika_client/_resource_recursive.py
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 tika_client-0.0.3/src/tika_client/_resource_tika.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 tika_client-0.0.3/src/tika_client/_types.py
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 tika_client-0.0.3/src/tika_client/_utils.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 tika_client-0.0.3/src/tika_client/client.py
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 tika_client-0.0.3/src/tika_client/data_models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tika_client-0.0.3/src/tika_client/py.typed
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 tika_client-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 tika_client-0.0.3/tests/conftest.py
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 tika_client-0.0.3/tests/test_resource_metadata.py
--rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 tika_client-0.0.3/tests/test_resource_recursive_metadata.py
--rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 tika_client-0.0.3/tests/test_resource_tika.py
--rw-r--r--   0        0        0    14164 2020-02-02 00:00:00.000000 tika_client-0.0.3/tests/samples/microsoft-sample.docx
--rw-r--r--   0        0        0     8843 2020-02-02 00:00:00.000000 tika_client-0.0.3/tests/samples/sample-spreadsheet.ods
--rw-r--r--   0        0        0     4743 2020-02-02 00:00:00.000000 tika_client-0.0.3/tests/samples/sample-spreadsheet.xlsx
--rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 tika_client-0.0.3/tests/samples/sample.docx
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 tika_client-0.0.3/tests/samples/sample.html
--rw-r--r--   0        0        0     8271 2020-02-02 00:00:00.000000 tika_client-0.0.3/tests/samples/sample.odt
--rw-r--r--   0        0        0   936200 2020-02-02 00:00:00.000000 tika_client-0.0.3/tests/samples/test-document-images.odt
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 tika_client-0.0.3/.gitignore
--rw-r--r--   0        0        0    34670 2020-02-02 00:00:00.000000 tika_client-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 tika_client-0.0.3/README.md
--rw-r--r--   0        0        0     3920 2020-02-02 00:00:00.000000 tika_client-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4419 2020-02-02 00:00:00.000000 tika_client-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 tika_client-0.1.0/.editorconfig
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 tika_client-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 tika_client-0.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 tika_client-0.1.0/.docker/docker-compose.ci-test.yml
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 tika_client-0.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 tika_client-0.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 tika_client-0.1.0/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tika_client-0.1.0/src/tika_client/__about__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 tika_client-0.1.0/src/tika_client/__init__.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tika_client-0.1.0/src/tika_client/_constants.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 tika_client-0.1.0/src/tika_client/_resource_meta.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 tika_client-0.1.0/src/tika_client/_resource_recursive.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 tika_client-0.1.0/src/tika_client/_resource_tika.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 tika_client-0.1.0/src/tika_client/_types.py
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 tika_client-0.1.0/src/tika_client/_utils.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 tika_client-0.1.0/src/tika_client/client.py
+-rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 tika_client-0.1.0/src/tika_client/data_models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tika_client-0.1.0/src/tika_client/py.typed
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/conftest.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/test_image_files.py
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/test_resource_metadata.py
+-rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/test_resource_recursive_metadata.py
+-rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/test_resource_tika.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/samples/README.md
+-rw-r--r--   0        0        0    14164 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/samples/microsoft-sample.docx
+-rw-r--r--   0        0        0     8843 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/samples/sample-spreadsheet.ods
+-rw-r--r--   0        0        0     4743 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/samples/sample-spreadsheet.xlsx
+-rw-r--r--   0        0        0    23552 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/samples/sample.doc
+-rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/samples/sample.docx
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/samples/sample.html
+-rw-r--r--   0        0        0   189116 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/samples/sample.jpg
+-rw-r--r--   0        0        0     8271 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/samples/sample.odt
+-rw-r--r--   0        0        0   980209 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/samples/sample.png
+-rw-r--r--   0        0        0   936200 2020-02-02 00:00:00.000000 tika_client-0.1.0/tests/samples/test-document-images.odt
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 tika_client-0.1.0/.gitignore
+-rw-r--r--   0        0        0    34670 2020-02-02 00:00:00.000000 tika_client-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 tika_client-0.1.0/README.md
+-rw-r--r--   0        0        0     3920 2020-02-02 00:00:00.000000 tika_client-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 tika_client-0.1.0/PKG-INFO
```

### Comparing `tika_client-0.0.3/.editorconfig` & `tika_client-0.1.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.3/.pre-commit-config.yaml` & `tika_client-0.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.3/CHANGELOG.md` & `tika_client-0.1.0/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.1.0] - 2023-06-17
+
+### Changed
+
+- Further refinements to the Tika response data models
+
+### Added
+
+- Testing against a .doc format file
+- Testing against JPEG and PNG format files
+
 ## [0.0.3] - 2023-06-01
 
 ### Changed
 
 - The plain text and html versions of the Tika endpoint have been renamed to `as_html` and `as_text`,
   hopefully to make it clearer about the response type
 - The plain text and html versions of the recursive endpoint were renamed to `as_html` and `as_text`
```

### Comparing `tika_client-0.0.3/.github/dependabot.yml` & `tika_client-0.1.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.3/.github/workflows/ci.yml` & `tika_client-0.1.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.3/.github/workflows/codeql.yml` & `tika_client-0.1.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.3/src/tika_client/_resource_meta.py` & `tika_client-0.1.0/src/tika_client/_resource_meta.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 from pathlib import Path
 from typing import Final
-from typing import Union
 
 from tika_client._types import MimeType
 from tika_client._utils import BaseResource
-from tika_client.data_models import BaseResponse
-from tika_client.data_models import DocumentMetadata
 
 
 class Metadata(BaseResource):
     """
     Handles interaction with the /meta endpoint of a Tika
     server REST API.
 
     See documentation:
     https://cwiki.apache.org/confluence/display/TIKA/TikaServer#TikaServer-MetadataResource
     """
 
     ENDPOINT: Final[str] = "/meta"
     MULTI_PART_ENDPOINT = f"{ENDPOINT}/form"
 
-    def from_file(self, filepath: Path, mime_type: MimeType = None) -> Union[BaseResponse, DocumentMetadata]:
+    def from_file(self, filepath: Path, mime_type: MimeType = None):
         """
         PUTs the provided document to the metadata endpoint using multipart
         file encoding.  Optionally can provide the mime type
         """
         resp = self._put_multipart(self.MULTI_PART_ENDPOINT, filepath, mime_type)
-        return DocumentMetadata(resp)
+        return self._decoded_response(resp)
```

### Comparing `tika_client-0.0.3/src/tika_client/_resource_recursive.py` & `tika_client-0.1.0/src/tika_client/_resource_recursive.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,40 +4,34 @@
 from typing import List
 from typing import Union
 
 from httpx import Client
 
 from tika_client._types import MimeType
 from tika_client._utils import BaseResource
-from tika_client.data_models import KNOWN_DATA_TYPES
-from tika_client.data_models import BaseResponse
-from tika_client.data_models import Document
-from tika_client.data_models import Image
+from tika_client.data_models import ParsedDocument
+from tika_client.data_models import ParsedImage
+from tika_client.data_models import TikaResponse
 
 logger = logging.getLogger("tika-client.rmeta")
 
 
 class _TikaRmetaBase(BaseResource):
     def _common_call(
         self,
         endpoint: str,
         filepath: Path,
         mime_type: MimeType = None,
-    ) -> List[Union[Document, Image, BaseResponse]]:
+    ) -> List[Union[ParsedDocument, ParsedImage, TikaResponse]]:
         """
         Given a specific endpoint and a file, do a multipart put to the endpoint
         """
-        documents: List[Union[Document, Image, BaseResponse]] = []
+        documents: List[Union[ParsedDocument, ParsedImage, TikaResponse]] = []
         for item in self._put_multipart(endpoint, filepath, mime_type):
-            # If a detailed class exists, use it
-            if item["Content-Type"] in KNOWN_DATA_TYPES:
-                documents.append(KNOWN_DATA_TYPES[item["Content-Type"]](item))
-            else:
-                logger.warning(f"Unknown content-type: {item['Content-Type']}")
-                documents.append(BaseResponse(item))
+            documents.append(self._decoded_response(item))
         return documents
 
 
 class _RecursiveMetaHtml(_TikaRmetaBase):
     ENDPOINT: Final[str] = "/rmeta"
     MULTI_PART_ENDPOINT = "/rmeta/form/html"
```

### Comparing `tika_client-0.0.3/src/tika_client/_resource_tika.py` & `tika_client-0.1.0/src/tika_client/_resource_tika.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 from pathlib import Path
 from typing import Final
-from typing import Union
 
 from httpx import Client
 
 from tika_client._types import MimeType
 from tika_client._types import RequestContent
 from tika_client._utils import BaseResource
-from tika_client.data_models import BaseResponse
-from tika_client.data_models import Document
 
 
 class _TikaHtml(BaseResource):
     ENDPOINT: Final[str] = "/tika"
     MULTI_PART_ENDPOINT = "/tika/form"
 
     def from_file(self, filepath: Path, mime_type: MimeType = None):
         """
         Returns the formatted (as HTML) document data
         """
         return self._decoded_response(self._put_multipart(self.MULTI_PART_ENDPOINT, filepath, mime_type))
 
-    def from_buffer(self, content: RequestContent, mime_type: MimeType = None) -> Union[BaseResponse, Document]:
+    def from_buffer(self, content: RequestContent, mime_type: MimeType = None):
         """
         Returns the HTML formatted document data from a given string of document content
         """
         return self._decoded_response(self._put_content(self.ENDPOINT, content, mime_type))
 
 
 class _TikaPlain(BaseResource):
@@ -34,15 +31,15 @@
 
     def from_file(self, filepath: Path, mime_type: MimeType = None):
         """
         Returns the plain text document data
         """
         return self._decoded_response(self._put_multipart(self.MULTI_PART_PLAIN_TEXT_CONTENT, filepath, mime_type))
 
-    def from_buffer(self, content: RequestContent, mime_type: MimeType = None) -> Union[BaseResponse, Document]:
+    def from_buffer(self, content: RequestContent, mime_type: MimeType = None):
         """
         Returns the plain text document data from a given string of document content
         """
         return self._decoded_response(self._put_content(self.PLAIN_TEXT_CONTENT, content, mime_type))
 
 
 class Tika(BaseResource):
```

### Comparing `tika_client-0.0.3/src/tika_client/_utils.py` & `tika_client-0.1.0/src/tika_client/_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,25 @@
+import logging
 from pathlib import Path
 from typing import Dict
 from typing import Union
 
 from httpx import Client
 
 from tika_client._constants import MIN_COMPRESS_LEN
 from tika_client._types import MimeType
 from tika_client._types import RequestContent
-from tika_client.data_models import KNOWN_DATA_TYPES
-from tika_client.data_models import BaseResponse
-from tika_client.data_models import Document
+from tika_client.data_models import DOCUMENT_TYPES
+from tika_client.data_models import IMAGE_TYPES
+from tika_client.data_models import ParsedDocument
+from tika_client.data_models import ParsedImage
+from tika_client.data_models import TikaKey
+from tika_client.data_models import TikaResponse
+
+logger = logging.getLogger("tika-client.utils")
 
 
 class BaseResource:
     def __init__(self, client: Client, *, compress: bool) -> None:
         self.client = client
         self.compress = compress
 
@@ -59,12 +65,20 @@
             headers["Content-Type"] = mime_type
 
         resp = self.client.put(endpoint, content=content_bytes, headers=headers)
         resp.raise_for_status()
         return resp.json()
 
     @staticmethod
-    def _decoded_response(resp_json: Dict) -> Union[BaseResponse, Document]:
-        base_resp = BaseResponse(resp_json)
-        if base_resp.type in KNOWN_DATA_TYPES:
-            return KNOWN_DATA_TYPES[base_resp.type](base_resp.data)
-        return base_resp  # pragma: no cover
+    def _decoded_response(resp_json: Dict) -> Union[ParsedDocument, ParsedImage, TikaResponse]:
+        """
+        If possible, returns a more detailed class with properties that appear often in this
+        mime type.  Otherwise, it's a basically raw data response, but with some helpers
+        for processing fields into Python types
+        """
+        if resp_json[TikaKey.ContentType] in IMAGE_TYPES:
+            return ParsedImage(resp_json)
+        elif resp_json[TikaKey.ContentType] in DOCUMENT_TYPES:
+            return ParsedDocument(resp_json)
+        else:
+            logger.warning(f"Unknown content-type: {resp_json[TikaKey.ContentLength]}")
+            return TikaResponse(resp_json)
```

### Comparing `tika_client-0.0.3/src/tika_client/client.py` & `tika_client-0.1.0/src/tika_client/client.py`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.3/tests/conftest.py` & `tika_client-0.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.3/tests/test_resource_metadata.py` & `tika_client-0.1.0/tests/test_resource_metadata.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,52 +5,60 @@
 import magic
 import pytest
 from pytest_httpx import HTTPXMock
 
 from tests.conftest import SAMPLE_DIR
 from tests.conftest import TIKA_URL
 from tika_client.client import TikaClient
-from tika_client.data_models import DocumentMetadata
+from tika_client.data_models import ParsedDocument
 
 
 class TestMetadataResource:
     def test_metadata_from_docx(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.docx"
         resp = tika_client.metadata.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
-        assert isinstance(resp, DocumentMetadata)
+        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
         assert resp.created is None
 
     def test_metadata_from_docx_no_mime(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.docx"
         resp = tika_client.metadata.from_file(test_file)
 
-        assert isinstance(resp, DocumentMetadata)
+        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
         assert resp.created is None
 
     def test_metadata_from_word_docx(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "microsoft-sample.docx"
         resp = tika_client.metadata.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
-        assert isinstance(resp, DocumentMetadata)
+        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
         assert resp.created == datetime(year=2023, month=5, day=17, hour=16, minute=41, tzinfo=timezone.utc)
         assert resp.modified == datetime(year=2023, month=5, day=17, hour=16, minute=44, tzinfo=timezone.utc)
 
     def test_metadata_from_odt(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.odt"
         resp = tika_client.metadata.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
-        assert isinstance(resp, DocumentMetadata)
+        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/vnd.oasis.opendocument.text"
         assert resp.data["generator"] == "LibreOfficeDev/6.0.5.2$Linux_X86_64 LibreOffice_project/"
         assert resp.created is None
 
+    def test_metadata_from_doc(self, tika_client: TikaClient):
+        test_file = SAMPLE_DIR / "sample.doc"
+        resp = tika_client.metadata.from_file(test_file, magic.from_file(str(test_file), mime=True))
+
+        assert isinstance(resp, ParsedDocument)
+        assert resp.type == "application/msword"
+        assert resp.language == "en"
+
     def test_http_error(self, httpx_mock: HTTPXMock):
         test_file = SAMPLE_DIR / "sample.odt"
 
         httpx_mock.add_response(status_code=500)
         with pytest.raises(httpx.HTTPStatusError) as err, TikaClient(tika_url=TIKA_URL) as client:
             client.metadata.from_file(test_file)
         assert err.value.response.status_code == httpx.codes.INTERNAL_SERVER_ERROR
```

### Comparing `tika_client-0.0.3/tests/test_resource_recursive_metadata.py` & `tika_client-0.1.0/tests/test_resource_recursive_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,26 @@
         documents = tika_client.rmeta.as_html.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
         assert len(documents) == 1
         document = documents[0]
 
         assert document.type == "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
         assert "<body><p>This is an DOCX test document, also made September 14, 2022</p>\n</body>" in document.content
-        assert document.metadata.created is None
+        assert document.created is None
 
     def test_r_metadata_from_docx_plain(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.docx"
         documents = tika_client.rmeta.as_text.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
         assert len(documents) == 1
         document = documents[0]
 
         assert document.type == "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
         assert "This is an DOCX test document, also made September 14, 2022" in document.content
-        assert document.metadata.created is None
+        assert document.created is None
 
     def test_r_meta_microsoft_word_docx(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "microsoft-sample.docx"
         documents = tika_client.rmeta.as_html.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
         assert len(documents) == 1
         document = documents[0]
@@ -45,15 +45,15 @@
         documents = tika_client.rmeta.as_html.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
         assert len(documents) == 2
         document = documents[0]
 
         assert document.type == "application/vnd.oasis.opendocument.text"
         assert "<body><p>This is an ODT test document, created September 14, 2022</p>\n</body>" in document.content
-        assert document.metadata.created is None
+        assert document.created is None
 
     def test_r_metadata_from_odt_plain(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.odt"
         documents = tika_client.rmeta.as_text.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
         assert len(documents) == 2
         document = documents[0]
```

### Comparing `tika_client-0.0.3/tests/test_resource_tika.py` & `tika_client-0.1.0/tests/test_resource_tika.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,99 +1,120 @@
 import magic
 
 from tests.conftest import SAMPLE_DIR
 from tika_client.client import TikaClient
-from tika_client.data_models import Document
+from tika_client.data_models import ParsedDocument
 
 
 class TestParseFormatted:
+    """
+    Test the Tika endpoint for returning HTML formatted content
+    """
+
     def test_parse_docx_from_file_as_html(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.docx"
         resp = tika_client.tika.as_html.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
-        assert isinstance(resp, Document)
+        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
         assert "<body><p>This is an DOCX test document, also made September 14, 2022</p>\n</body>" in resp.content
+        assert resp.content_length == 6424
+
+    def test_parse_doc_from_file_as_html(self, tika_client: TikaClient):
+        test_file = SAMPLE_DIR / "sample.doc"
+        resp = tika_client.tika.as_html.from_file(test_file, magic.from_file(str(test_file), mime=True))
+
+        assert isinstance(resp, ParsedDocument)
+        assert resp.type == "application/msword"
+        assert (
+            "body><p>This is a test document, saved in the older .doc format for Word documents (but created in Google Drive)</p>\n</body>"  # noqa: E501
+            in resp.content
+        )
+        assert resp.content_length == 23739
+        assert resp.character_count == 90
+        assert resp.page_count == 1
+        assert resp.revision == 1
+        assert resp.last_author == "cloudconvert_4"
 
     def test_parse_docx_no_mime_from_file_as_html(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.docx"
         resp = tika_client.tika.as_html.from_file(test_file)
 
-        assert isinstance(resp, Document)
+        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
         assert "<body><p>This is an DOCX test document, also made September 14, 2022</p>\n</body>" in resp.content
 
     def test_parse_microsoft_word_docx_from_file_as_html(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "microsoft-sample.docx"
         resp = tika_client.tika.as_html.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
-        assert isinstance(resp, Document)
+        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
         assert (
             "<body><p>This is a sample document, generated by Microsoft Office on Wednesday, May 17, 2023.</p>\n<p>It is in English.</p>\n</body>"  # noqa: E501
             in resp.content
         )
 
     def test_parse_odt_from_file_as_html(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.odt"
         resp = tika_client.tika.as_html.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
-        assert isinstance(resp, Document)
+        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/vnd.oasis.opendocument.text"
         assert "<body><p>This is an ODT test document, created September 14, 2022</p>\n</body>" in resp.content
 
 
 class TestParsePlain:
     def test_parse_docx_from_file_as_text(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.docx"
 
         resp = tika_client.tika.as_text.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
-        assert isinstance(resp, Document)
+        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
         assert "This is an DOCX test document, also made September 14, 2022" in resp.content
 
     def test_parse_odt_from_file_as_text(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.odt"
 
         resp = tika_client.tika.as_text.from_file(test_file, magic.from_file(str(test_file), mime=True))
 
-        assert isinstance(resp, Document)
+        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/vnd.oasis.opendocument.text"
         assert "This is an ODT test document, created September 14, 2022" in resp.content
 
 
 class TestParseContentPlain:
     def test_parse_docx_from_bytes_buffer(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.docx"
         buffer = test_file.read_bytes()
 
         resp = tika_client.tika.as_text.from_buffer(buffer)
 
-        assert isinstance(resp, Document)
+        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
         assert "This is an DOCX test document, also made September 14, 2022" in resp.content
 
     def test_parse_odt_from_bytes_buffer(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.odt"
         buffer = test_file.read_bytes()
 
         resp = tika_client.tika.as_text.from_buffer(buffer)
 
-        assert isinstance(resp, Document)
+        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/vnd.oasis.opendocument.text"
         assert "This is an ODT test document, created September 14, 2022" in resp.content
 
     def test_parse_odt_from_bytes_buffer_with_mime(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.odt"
         buffer = test_file.read_bytes()
 
         resp = tika_client.tika.as_text.from_buffer(buffer, "application/vnd.oasis.opendocument.text")
 
-        assert isinstance(resp, Document)
+        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/vnd.oasis.opendocument.text"
         assert "This is an ODT test document, created September 14, 2022" in resp.content
 
     def test_html_document_from_string_buffer(self, tika_client: TikaClient):
         test_file = SAMPLE_DIR / "sample.html"
         buffer = test_file.read_text()
 
@@ -109,9 +130,9 @@
 class TestParseContentCompress:
     def test_parse_odt_from_bytes_buffer_compress(self, tika_client_compressed: TikaClient):
         test_file = SAMPLE_DIR / "test-document-images.odt"
         buffer = test_file.read_bytes()
 
         resp = tika_client_compressed.tika.as_text.from_buffer(buffer)
 
-        assert isinstance(resp, Document)
+        assert isinstance(resp, ParsedDocument)
         assert resp.type == "application/vnd.oasis.opendocument.text"
```

### Comparing `tika_client-0.0.3/tests/samples/microsoft-sample.docx` & `tika_client-0.1.0/tests/samples/microsoft-sample.docx`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.3/tests/samples/sample-spreadsheet.ods` & `tika_client-0.1.0/tests/samples/sample-spreadsheet.ods`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.3/tests/samples/sample-spreadsheet.xlsx` & `tika_client-0.1.0/tests/samples/sample-spreadsheet.xlsx`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.3/tests/samples/sample.docx` & `tika_client-0.1.0/tests/samples/sample.docx`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.3/tests/samples/sample.odt` & `tika_client-0.1.0/tests/samples/sample.odt`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.3/tests/samples/test-document-images.odt` & `tika_client-0.1.0/tests/samples/test-document-images.odt`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.3/.gitignore` & `tika_client-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.3/LICENSE.txt` & `tika_client-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.3/README.md` & `tika_client-0.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 ## Features
 
 - Simplified: No need to worry about XML or JSON responses, downloading a Tika jar file or Python 2
 - Support for Tika 2+ only
 - Based on the modern [httpx](https://github.com/encode/httpx) library
 - Full support for type hinting
-- Full test coverage run against an actual Tika server for multiple Python and PyPy versions
+- Nearly full test coverage run against an actual Tika server for multiple Python and PyPy versions
 - Uses HTTP multipart/form-data to stream files to the server (instead of reading into memory)
 - Optional compression for parsing from a file content already in a buffer (as opposed to a file)
 
 ## Installation
 
 ```console
 pip3 install tika-client
@@ -59,31 +59,31 @@
 
 ```
 
 The Tika REST API documentation can be found [here](https://cwiki.apache.org/confluence/display/TIKA/TikaServer).
 At the moment, only the metadata, tika and recursive metadata endpoints are implemented.
 
 Unfortunately, the set of possible return values of the Tika API are not very well documented. The library makes
-a best effort to extract relevant fields into type attributes, including conversion of date strings to
-time zone aware `datetime` objects. The full JSON response is always available to the user under the `.data`
+a best effort to extract relevant fields into type properties where it understands more about the mime type
+of the document (as returned by Tika). This includes information like created/modified information as time zone
+aware `datetime` objects. The full JSON response is always available to the user under the `.data`
 attribute.
 
-In general, requests from the tika and recursive endpoints return a
-`Document` with any metadata available under `document.metadata`.
+When a particular key is not present in the response, all properties will return `None` instead.
 
 ## Why
 
 Only one other library for interfacing with Tika exists that I know of. I find it too complicated, trying to handle
 a lot of differing uses.
 
 The biggest issue I have with the library is its downloading and running of a jar file if needed. To me, an
 API client should only interface to the API and not try to provide functionality to start
 the API as well. The user is responsible for providing the server with the Tika version they desire.
 
 The library also provides a lot of knobs to turn, but I argue most developers will not want to configure XML as
-the response type, they just want the data, already parsed.
+the response type, they just want the data, already parsed to the maximum extend possible.
 
 This library attempts to provide a simpler interface, minimal lines of code and typing of the parsed response.
 
 ## License
 
 `tika-client` is distributed under the terms of the [GPL-3.0-only](https://spdx.org/licenses/GPL-3.0-only.html) license.
```

### Comparing `tika_client-0.0.3/pyproject.toml` & `tika_client-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tika_client-0.0.3/PKG-INFO` & `tika_client-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tika-client
-Version: 0.0.3
+Version: 0.1.0
 Summary: A modern REST client for Apache Tika server
 Project-URL: Documentation, https://github.com/stumpylog/tika-rest-client#readme
 Project-URL: Issues, https://github.com/stumpylog/tika-rest-client/issues
 Project-URL: Source, https://github.com/stumpylog/tika-rest-client
 Author-email: Trenton H <797416+stumpylog@users.noreply.github.com>
 License-Expression: GPL-3.0-only
 License-File: LICENSE.txt
@@ -37,15 +37,15 @@
 
 ## Features
 
 - Simplified: No need to worry about XML or JSON responses, downloading a Tika jar file or Python 2
 - Support for Tika 2+ only
 - Based on the modern [httpx](https://github.com/encode/httpx) library
 - Full support for type hinting
-- Full test coverage run against an actual Tika server for multiple Python and PyPy versions
+- Nearly full test coverage run against an actual Tika server for multiple Python and PyPy versions
 - Uses HTTP multipart/form-data to stream files to the server (instead of reading into memory)
 - Optional compression for parsing from a file content already in a buffer (as opposed to a file)
 
 ## Installation
 
 ```console
 pip3 install tika-client
@@ -81,31 +81,31 @@
 
 ```
 
 The Tika REST API documentation can be found [here](https://cwiki.apache.org/confluence/display/TIKA/TikaServer).
 At the moment, only the metadata, tika and recursive metadata endpoints are implemented.
 
 Unfortunately, the set of possible return values of the Tika API are not very well documented. The library makes
-a best effort to extract relevant fields into type attributes, including conversion of date strings to
-time zone aware `datetime` objects. The full JSON response is always available to the user under the `.data`
+a best effort to extract relevant fields into type properties where it understands more about the mime type
+of the document (as returned by Tika). This includes information like created/modified information as time zone
+aware `datetime` objects. The full JSON response is always available to the user under the `.data`
 attribute.
 
-In general, requests from the tika and recursive endpoints return a
-`Document` with any metadata available under `document.metadata`.
+When a particular key is not present in the response, all properties will return `None` instead.
 
 ## Why
 
 Only one other library for interfacing with Tika exists that I know of. I find it too complicated, trying to handle
 a lot of differing uses.
 
 The biggest issue I have with the library is its downloading and running of a jar file if needed. To me, an
 API client should only interface to the API and not try to provide functionality to start
 the API as well. The user is responsible for providing the server with the Tika version they desire.
 
 The library also provides a lot of knobs to turn, but I argue most developers will not want to configure XML as
-the response type, they just want the data, already parsed.
+the response type, they just want the data, already parsed to the maximum extend possible.
 
 This library attempts to provide a simpler interface, minimal lines of code and typing of the parsed response.
 
 ## License
 
 `tika-client` is distributed under the terms of the [GPL-3.0-only](https://spdx.org/licenses/GPL-3.0-only.html) license.
```

