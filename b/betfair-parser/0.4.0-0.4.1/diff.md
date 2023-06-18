# Comparing `tmp/betfair_parser-0.4.0.tar.gz` & `tmp/betfair_parser-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betfair_parser-0.4.0.tar", max compression
+gzip compressed data, was "betfair_parser-0.4.1.tar", max compression
```

## Comparing `betfair_parser-0.4.0.tar` & `betfair_parser-0.4.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1286 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0     3277 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/__init__.py
--rw-r--r--   0        0        0     2038 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/client.py
--rw-r--r--   0        0        0     2417 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/endpoints.py
--rw-r--r--   0        0        0      741 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/__init__.py
--rw-r--r--   0        0        0       85 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/accounts/__init__.py
--rw-r--r--   0        0        0     2929 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/accounts/enums.py
--rw-r--r--   0        0        0     3177 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/accounts/operations.py
--rw-r--r--   0        0        0    11161 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/accounts/type_definitions.py
--rw-r--r--   0        0        0       84 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/betting/__init__.py
--rw-r--r--   0        0        0    21951 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/betting/enums.py
--rw-r--r--   0        0        0     9634 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/betting/listings.py
--rw-r--r--   0        0        0      134 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/betting/operations.py
--rw-r--r--   0        0        0     8860 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/betting/orders.py
--rw-r--r--   0        0        0    32688 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/betting/type_definitions.py
--rw-r--r--   0        0        0      238 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/common/__init__.py
--rw-r--r--   0        0        0     9771 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/common/enums.py
--rw-r--r--   0        0        0     4716 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/common/messages.py
--rw-r--r--   0        0        0     1493 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/common/type_definitions.py
--rw-r--r--   0        0        0     2773 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/heartbeat.py
--rw-r--r--   0        0        0     8653 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/identity.py
--rw-r--r--   0        0        0     3645 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/navigation.py
--rw-r--r--   0        0        0     3172 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/race_status.py
--rw-r--r--   0        0        0      399 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/streaming/__init__.py
--rw-r--r--   0        0        0     5989 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/streaming/mcm.py
--rw-r--r--   0        0        0     2247 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/streaming/ocm.py
--rw-r--r--   0        0        0     2507 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/streaming/status.py
--rw-r--r--   0        0        0     2319 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/strenums.py
--rw-r--r--   0        0        0      902 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/util.py
--rw-r--r--   0        0        0     1731 2023-06-16 04:54:28.902370 betfair_parser-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3767 1970-01-01 00:00:00.000000 betfair_parser-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1286 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/LICENSE.txt
+-rw-r--r--   0        0        0     3277 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/__init__.py
+-rw-r--r--   0        0        0     2054 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/client.py
+-rw-r--r--   0        0        0     2417 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/endpoints.py
+-rw-r--r--   0        0        0      741 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/__init__.py
+-rw-r--r--   0        0        0       85 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/accounts/__init__.py
+-rw-r--r--   0        0        0     2929 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/accounts/enums.py
+-rw-r--r--   0        0        0     3177 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/accounts/operations.py
+-rw-r--r--   0        0        0    11161 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/accounts/type_definitions.py
+-rw-r--r--   0        0        0       84 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/betting/__init__.py
+-rw-r--r--   0        0        0    21951 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/betting/enums.py
+-rw-r--r--   0        0        0     9634 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/betting/listings.py
+-rw-r--r--   0        0        0      134 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/betting/operations.py
+-rw-r--r--   0        0        0     8860 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/betting/orders.py
+-rw-r--r--   0        0        0    32923 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/betting/type_definitions.py
+-rw-r--r--   0        0        0      238 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/common/__init__.py
+-rw-r--r--   0        0        0     9771 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/common/enums.py
+-rw-r--r--   0        0        0     4734 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/common/messages.py
+-rw-r--r--   0        0        0     1493 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/common/type_definitions.py
+-rw-r--r--   0        0        0     2773 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/heartbeat.py
+-rw-r--r--   0        0        0     8653 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/identity.py
+-rw-r--r--   0        0        0     3645 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/navigation.py
+-rw-r--r--   0        0        0     3172 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/race_status.py
+-rw-r--r--   0        0        0      399 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/streaming/__init__.py
+-rw-r--r--   0        0        0     5989 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/streaming/mcm.py
+-rw-r--r--   0        0        0     2247 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/streaming/ocm.py
+-rw-r--r--   0        0        0     2507 2023-06-18 09:38:31.226552 betfair_parser-0.4.1/betfair_parser/spec/streaming/status.py
+-rw-r--r--   0        0        0     2319 2023-06-18 09:38:31.226552 betfair_parser-0.4.1/betfair_parser/strenums.py
+-rw-r--r--   0        0        0      902 2023-06-18 09:38:31.226552 betfair_parser-0.4.1/betfair_parser/util.py
+-rw-r--r--   0        0        0     1731 2023-06-18 09:38:46.874497 betfair_parser-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3767 1970-01-01 00:00:00.000000 betfair_parser-0.4.1/PKG-INFO
```

### Comparing `betfair_parser-0.4.0/LICENSE.txt` & `betfair_parser-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.0/README.md` & `betfair_parser-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.0/betfair_parser/client.py` & `betfair_parser-0.4.1/betfair_parser/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 
 def request(session, req: Request, endpoints=ENDPOINTS):
     """Minimalistic client example."""
 
     url = endpoints.url_for_request(req)
     raw_resp = session.post(url, headers=req.headers(), data=req.body())
-    resp = req.parse_response(raw_resp.content, raise_errors=True)
-    return resp
+    raw_resp.raise_for_status()
+    return req.parse_response(raw_resp.content, raise_errors=True)
 
 
 def login(session, username, password, app_key, two_factor_code="", endpoints=ENDPOINTS):
     """Authenticate a session to betfair."""
 
     session.headers.update({"X-Application": app_key})
     resp = request(
```

### Comparing `betfair_parser-0.4.0/betfair_parser/endpoints.py` & `betfair_parser-0.4.1/betfair_parser/endpoints.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.0/betfair_parser/exceptions.py` & `betfair_parser-0.4.1/betfair_parser/exceptions.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,22 @@
     """Base class for all Exceptions in this package. Allow to hand in custom data with keyword arguments."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args)
         self.__dict__.update(kwargs)
 
 
-class APIError(BetfairError):
-    """Most general API error."""
-
-
 class JSONError(BetfairError):
     """Issue with the data serialization."""
 
 
+class APIError(BetfairError):
+    """Most general API error."""
+
+
 class APINGException(APIError):
     """Errors thrown from a betfair operation."""
 
 
 class AccountAPINGException(APIError):
     """An issue thrown from the accounts API."""
```

### Comparing `betfair_parser-0.4.0/betfair_parser/spec/accounts/enums.py` & `betfair_parser-0.4.1/betfair_parser/spec/accounts/enums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.0/betfair_parser/spec/accounts/operations.py` & `betfair_parser-0.4.1/betfair_parser/spec/accounts/operations.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.0/betfair_parser/spec/accounts/type_definitions.py` & `betfair_parser-0.4.1/betfair_parser/spec/accounts/type_definitions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.0/betfair_parser/spec/betting/enums.py` & `betfair_parser-0.4.1/betfair_parser/spec/betting/enums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.0/betfair_parser/spec/betting/listings.py` & `betfair_parser-0.4.1/betfair_parser/spec/betting/listings.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.0/betfair_parser/spec/betting/orders.py` & `betfair_parser-0.4.1/betfair_parser/spec/betting/orders.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.0/betfair_parser/spec/betting/type_definitions.py` & `betfair_parser-0.4.1/betfair_parser/spec/betting/type_definitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,14 +280,20 @@
     cloth_number_alpha: Optional[str] = None  # The number on the saddle cloth for US paired runners, e.g. "1A"
 
     @property
     def colours_url(self):
         if self.colours_filename:
             return SILKS + self.colours_filename
 
+    @property
+    def forecastprice_decimal(self):
+        if not self.forecastprice_numerator or not self.forecastprice_denominator:
+            return
+        return self.forecastprice_numerator / self.forecastprice_denominator + 1
+
 
 class RunnerCatalog(BaseMessage, frozen=True):
     """Information about the Runners (selections) in a market"""
 
     selection_id: int  # The unique id for the selection
     runner_name: str  # The name of the runner
```

### Comparing `betfair_parser-0.4.0/betfair_parser/spec/common/enums.py` & `betfair_parser-0.4.1/betfair_parser/spec/common/enums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.0/betfair_parser/spec/common/messages.py` & `betfair_parser-0.4.1/betfair_parser/spec/common/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Generic, Literal, Optional, TypeVar
 
 import msgspec
 
-from betfair_parser.exceptions import APINGException, JSONError
+from betfair_parser.exceptions import APIError, APINGException, JSONError
 from betfair_parser.spec.common.enums import (
     AccountAPINGExceptionCode,
     APINGExceptionCode,
     EndpointType,
     JSONExceptionCode,
 )
 
@@ -114,15 +114,15 @@
     method: str = ""
     params: ParamsType = {}  # type: ignore
     return_type = Response  # not to be serialized, so no type definition
     throws = APINGException  # JSON error definition
 
     @classmethod
     def with_params(cls, request_id=1, **kwargs):
-        params_cls = cls.__annotations__["params"]
+        params_cls = cls.__annotations__.get("params", dict)
         return cls(
             params=params_cls(**kwargs),
             method=cls.method,
             id=request_id,
         )
 
     @staticmethod
@@ -136,15 +136,15 @@
 
     def body(self):
         return encode(self)
 
     def parse_response(self, response, raise_errors=True):
         resp = decode(response, type=self.return_type)
         if resp.id != self.id:
-            raise ValueError(f"Response ID ({resp.id}) does not match Request ID ({self.id})")
+            raise APIError(f"Response ID ({resp.id}) does not match Request ID ({self.id})")
         if resp.is_error:
             if raise_errors:
                 exception = self.throws(
                     str(resp.error.exception_code),
                     response=resp,
                     request=self,
                     code=resp.error.exception_code,
```

### Comparing `betfair_parser-0.4.0/betfair_parser/spec/common/type_definitions.py` & `betfair_parser-0.4.1/betfair_parser/spec/common/type_definitions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.0/betfair_parser/spec/heartbeat.py` & `betfair_parser-0.4.1/betfair_parser/spec/heartbeat.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.0/betfair_parser/spec/identity.py` & `betfair_parser-0.4.1/betfair_parser/spec/identity.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.0/betfair_parser/spec/navigation.py` & `betfair_parser-0.4.1/betfair_parser/spec/navigation.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.0/betfair_parser/spec/race_status.py` & `betfair_parser-0.4.1/betfair_parser/spec/race_status.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.0/betfair_parser/spec/streaming/mcm.py` & `betfair_parser-0.4.1/betfair_parser/spec/streaming/mcm.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.0/betfair_parser/spec/streaming/ocm.py` & `betfair_parser-0.4.1/betfair_parser/spec/streaming/ocm.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.0/betfair_parser/spec/streaming/status.py` & `betfair_parser-0.4.1/betfair_parser/spec/streaming/status.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.0/betfair_parser/strenums.py` & `betfair_parser-0.4.1/betfair_parser/strenums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.0/betfair_parser/util.py` & `betfair_parser-0.4.1/betfair_parser/util.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.0/pyproject.toml` & `betfair_parser-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "betfair_parser"
-version = "0.4.0"
+version = "0.4.1"
 description = "A betfair parser"
 readme = "README.md"
 authors = ["Bradley McElroy <bradley.mcelroy@live.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 msgspec = "^0.16.0"
```

### Comparing `betfair_parser-0.4.0/PKG-INFO` & `betfair_parser-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betfair-parser
-Version: 0.4.0
+Version: 0.4.1
 Summary: A betfair parser
 Author: Bradley McElroy
 Author-email: bradley.mcelroy@live.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

