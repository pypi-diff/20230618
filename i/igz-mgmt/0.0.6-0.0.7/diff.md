# Comparing `tmp/igz_mgmt-0.0.6.tar.gz` & `tmp/igz_mgmt-0.0.7.tar.gz`

## Comparing `igz_mgmt-0.0.6.tar` & `igz_mgmt-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/__init__.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/__version__.py
--rw-r--r--   0        0        0    15533 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/client.py
--rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/constants.py
--rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/cruds.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/exceptions.py
--rw-r--r--   0        0        0     9734 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/operations.py
--rw-r--r--   0        0        0    47741 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/resources.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/common/__init__.py
--rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/common/helpers.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/logger/__init__.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/logger/logger.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/schemas/__init__.py
--rw-r--r--   0        0        0    11993 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/schemas/app_services.py
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/igz_mgmt/schemas/manual_events.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/LICENSE
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/README.md
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 igz_mgmt-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/__init__.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/__version__.py
+-rw-r--r--   0        0        0    16097 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/client.py
+-rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/constants.py
+-rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/cruds.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/exceptions.py
+-rw-r--r--   0        0        0    10302 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/operations.py
+-rw-r--r--   0        0        0    47741 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/resources.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/common/__init__.py
+-rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/common/helpers.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/logger/__init__.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/logger/logger.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/schemas/__init__.py
+-rw-r--r--   0        0        0    11993 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/schemas/app_services.py
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/igz_mgmt/schemas/manual_events.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/LICENSE
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/README.md
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 igz_mgmt-0.0.7/PKG-INFO
```

### Comparing `igz_mgmt-0.0.6/igz_mgmt/__init__.py` & `igz_mgmt-0.0.7/igz_mgmt/__init__.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.6/igz_mgmt/__version__.py` & `igz_mgmt-0.0.7/igz_mgmt/__version__.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # limitations under the License.
 #
 
 # version can be either one of the following:
 # x.y.z
 # x.y.z.rcN
 
-__version__ = "0.0.6"
+__version__ = "0.0.7"
```

### Comparing `igz_mgmt-0.0.6/igz_mgmt/client.py` & `igz_mgmt-0.0.7/igz_mgmt/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """The API client used to communicate with the Iguazio backend."""
 import base64
 import copy
 import os
+import typing
 from http import HTTPStatus
 
 import httpx
 import inflection
 import semver
 
 import igz_mgmt.common
@@ -172,14 +173,16 @@
         if password and not username or access_key and not username:
             raise ValueError(
                 "Must provide username when providing password or access key"
             )
 
         self._logger = igz_mgmt.get_or_create_logger(level="INFO", name="apic")
 
+        # TODO: type of Session
+        self._session_obj: typing.Optional[dict] = None
         self._client = _BaseHTTPClient(
             self._logger,
             igz_mgmt.common.helpers.get_endpoint(endpoint, default_scheme="https"),
             timeout=timeout,
             retries=retries,
         )
 
@@ -365,14 +368,15 @@
                     "username": username,
                     "password": password,
                     "plane": igz_mgmt.constants.SessionPlanes.control.value,
                 },
             ),
         )
         self._set_auth(username=username, session=response.cookies.get("session"))
+        self._session_obj = response.json().get("data", {})
 
     def _set_auth(self, username: str, access_key: str = "", session: str = ""):
         if access_key and session:
             raise ValueError("Cannot set both access_key and session")
         self._client._cookies.set(
             "session",
             f'j:{{"sid": "{access_key}"}}' if access_key else session,
@@ -416,14 +420,30 @@
             "Failed to resolve auto detect iguazio external version, use `client.version = x.y.z` for explicitness"
         )
 
         # oldest supported GA version
         return self.__DEFAULT_EXTERNAL_VERSION_NUMBER
 
     @property
+    def tenant_id(self) -> str:
+        """Resolves the tenant id from session.
+
+        Returns:
+            tenant id
+        """
+        if not self._authenticated:
+            raise RuntimeError("Must .login() first")
+        return (
+            self._session_obj.get("relationships", {})
+            .get("tenant", {})
+            .get("data", {})
+            .get("id")
+        )
+
+    @property
     def version(self) -> semver.VersionInfo:
         """Iguazio system version info.
 
         Returns:
             semver.VersionInfo: Iguazio version
         """
         return self._version
```

### Comparing `igz_mgmt-0.0.6/igz_mgmt/constants.py` & `igz_mgmt-0.0.7/igz_mgmt/constants.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.6/igz_mgmt/cruds.py` & `igz_mgmt-0.0.7/igz_mgmt/cruds.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.6/igz_mgmt/exceptions.py` & `igz_mgmt-0.0.7/igz_mgmt/exceptions.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.6/igz_mgmt/operations.py` & `igz_mgmt-0.0.7/igz_mgmt/operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #
 """Below are classes which do not have a corresponding resource in the API but represent operations.
 
 Some endpoints within the management API are considered “operations”,
 which means that the response may not represent a resource.
 Some operations are long-living, which means a background job is created whereas the response will hold its id.
 """
-
+import json
 import typing
 
 import igz_mgmt.client
 import igz_mgmt.constants
 import igz_mgmt.exceptions
 import igz_mgmt.resources
 import igz_mgmt.schemas.app_services
@@ -55,31 +55,46 @@
     """Manual event operations."""
 
     @classmethod
     def emit(
         cls,
         http_client: igz_mgmt.client.APIClient,
         event: igz_mgmt.schemas.manual_events.ManualEventSchema,
+        audit_tenant_id: typing.Optional[str] = None,
     ):
         """Emits a manual event.
 
         This operation requires system-admin role permissions.
 
         Args:
             http_client (APIClient): The client to use.
             event (ManualEventSchema): The event to emit.
+            audit_tenant_id: The assigned tenant id for auditing events (required for audit events).
         """
+        relationships = None
+        if audit_tenant_id:
+            relationships = {
+                "audit_tenant": {
+                    "data": {"type": "tenant", "id": audit_tenant_id},
+                },
+            }
+
         manual_event_request = {
             "data": {
                 **igz_mgmt.schemas.manual_events.ManualEventRequest(
-                    attributes=event
+                    attributes=event,
+                    relationships=relationships,
                 ).dict(exclude_none=True)
             }
         }
-        http_client.request("POST", "manual_events", json=manual_event_request)
+        try:
+            http_client.request("POST", "manual_events", json=manual_event_request)
+        except json.JSONDecodeError:
+            # endpoint is not json on old igz versions
+            pass
 
 
 class AppServices(object):
     """Syntactic sugar to AppServicesManifest class."""
 
     @classmethod
     def get(
```

### Comparing `igz_mgmt-0.0.6/igz_mgmt/resources.py` & `igz_mgmt-0.0.7/igz_mgmt/resources.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.6/igz_mgmt/common/__init__.py` & `igz_mgmt-0.0.7/igz_mgmt/common/__init__.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.6/igz_mgmt/common/helpers.py` & `igz_mgmt-0.0.7/igz_mgmt/common/helpers.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.6/igz_mgmt/logger/__init__.py` & `igz_mgmt-0.0.7/igz_mgmt/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.6/igz_mgmt/logger/logger.py` & `igz_mgmt-0.0.7/igz_mgmt/logger/logger.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.6/igz_mgmt/schemas/__init__.py` & `igz_mgmt-0.0.7/igz_mgmt/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.6/igz_mgmt/schemas/app_services.py` & `igz_mgmt-0.0.7/igz_mgmt/schemas/app_services.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.6/igz_mgmt/schemas/manual_events.py` & `igz_mgmt-0.0.7/igz_mgmt/schemas/manual_events.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,7 +103,8 @@
 
 
 class ManualEventRequest(igz_mgmt.schemas._Base):
     """Manual event request."""
 
     type: str = pydantic.Field("event", const=True)
     attributes: ManualEventSchema
+    relationships: typing.Optional[dict]
```

### Comparing `igz_mgmt-0.0.6/LICENSE` & `igz_mgmt-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.6/pyproject.toml` & `igz_mgmt-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.6/PKG-INFO` & `igz_mgmt-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igz-mgmt
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python SDK For Iguazio Management API
 Project-URL: Homepage, https://github.com/iguazio/igz-mgmt-sdk
 Author-email: Iguazio Platform Team <liranb@iguazio.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

