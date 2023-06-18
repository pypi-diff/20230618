# Comparing `tmp/drizzutojr_vapi-0.0.2-py3-none-any.whl.zip` & `tmp/drizzutojr_vapi-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3692 bytes, number of entries: 8
--rw-r--r--  2.0 unx       49 b- defN 23-Jun-13 07:14 vapi/__init__.py
--rw-r--r--  2.0 unx      367 b- defN 23-Jun-13 07:14 vapi/exceptions.py
--rw-r--r--  2.0 unx     4775 b- defN 23-Jun-13 07:14 vapi/vapi.py
--rw-r--r--  2.0 unx     1061 b- defN 23-Jun-13 07:15 drizzutojr_vapi-0.0.2.dist-info/LICENSE.md
--rw-r--r--  2.0 unx      200 b- defN 23-Jun-13 07:15 drizzutojr_vapi-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 07:15 drizzutojr_vapi-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-13 07:15 drizzutojr_vapi-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      641 b- defN 23-Jun-13 07:15 drizzutojr_vapi-0.0.2.dist-info/RECORD
-8 files, 7190 bytes uncompressed, 2566 bytes compressed:  64.3%
+Zip file size: 3986 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-18 21:46 vapi/__init__.py
+-rw-r--r--  2.0 unx     1107 b- defN 23-Jun-18 21:46 vapi/exceptions.py
+-rw-r--r--  2.0 unx     5449 b- defN 23-Jun-18 21:46 vapi/vapi.py
+-rw-r--r--  2.0 unx     1061 b- defN 23-Jun-18 21:48 drizzutojr_vapi-0.0.3.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx      200 b- defN 23-Jun-18 21:48 drizzutojr_vapi-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-18 21:48 drizzutojr_vapi-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-18 21:48 drizzutojr_vapi-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      642 b- defN 23-Jun-18 21:48 drizzutojr_vapi-0.0.3.dist-info/RECORD
+8 files, 8605 bytes uncompressed, 2860 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: vapi/exceptions.py
 Comment: 
 
 Filename: vapi/vapi.py
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.2.dist-info/LICENSE.md
+Filename: drizzutojr_vapi-0.0.3.dist-info/LICENSE.md
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.2.dist-info/METADATA
+Filename: drizzutojr_vapi-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.2.dist-info/WHEEL
+Filename: drizzutojr_vapi-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.2.dist-info/top_level.txt
+Filename: drizzutojr_vapi-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.2.dist-info/RECORD
+Filename: drizzutojr_vapi-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vapi/exceptions.py

```diff
@@ -1,14 +1,41 @@
-class VAPIPermissionDeniedError(Exception):
-    """Vault returned permission denied"""
+DEFAULT_STATUS_CODE = 400
 
 
-class VAPISealedError(Exception):
-    """Vault is sealed"""
+def vapi_exception_handler(exception):
+    return {
+        "message": str(exception.message),
+        "status_code": exception.status_code,
+        "response": exception.response,
+        "errors": exception.errors,
+    }, exception.status_code
 
 
-class VAPIAcceptedStatusCodeError(Exception):
-    """The Status Code returned from Vault does match the accepted status codes set by the user"""
+class VAPIGenericError(Exception):
+    def __init__(self, message: str, details: str = ""):
+        self.message = message
+        self.details = details
+        super().__init__(self.message)
 
 
-class VAPIGenericError(Exception):
+class VAPIConfigError(VAPIGenericError):
     """Vault returned an Error"""
+
+
+class VAPIVaultError(Exception):
+    def __init__(self, message: str, status_code: int, errors: list = []):
+        self.message = message
+        self.errors = errors
+        self.status_code = status_code
+        super().__init__(self.message)
+
+
+class VAPIPermissionDeniedError(VAPIVaultError):
+    """Vault returned permission denied"""
+
+
+class VAPISealedError(VAPIVaultError):
+    """Vault is sealed"""
+
+
+class VAPIAcceptedStatusCodeError(VAPIVaultError):
+    """The Status Code returned from Vault does match the accepted status codes set by the user"""
```

## vapi/vapi.py

```diff
@@ -15,48 +15,57 @@
         token_file: str = None,
     ):
         self.addr = addr or os.environ.get("VAULT_ADDR", None)
         self.cacert = cacert or os.environ.get("VAULT_CACERT", None)
         self.namespace = namespace or os.environ.get("VAULT_NAMESPACE", "")
 
         if token and token_file:
-            raise ValueError("May not set token and token_file.  Please choose one.")
+            raise VAPIConfigError(
+                "May not set token and token_file.  Please choose one."
+            )
         elif token:
             self.token = token
         elif token_file:
             with open(token_file, "r") as f:
                 self.token = f.read().strip()
         elif os.environ.get("VAULT_TOKEN", None):
             self.token = os.environ["VAULT_TOKEN"]
         elif os.environ.get("VAULT_TOKEN_FILE", None):
             with open(os.environ["VAULT_TOKEN_FILE"], "r") as f:
                 self.token = f.read().strip()
         else:
-            raise ValueError(
-                "Vault Token not set.  Please check Env variables or pass directly."
+            raise VAPIConfigError(
+                "Vault Token not set", "Please check Env variables or pass directly"
             )
 
         if self.addr is None:
-            raise ValueError("Vault Address not passed or set as environmetn variable")
+            raise VAPIConfigError(
+                "Vault Address not passed or set as environmetn variable",
+                "Please check Env variables or pass directly",
+            )
         if self.token is None:
-            raise ValueError("Vault Token not passed or set as environment variable")
+            raise VAPIConfigError(
+                "Vault Token not passed or set as environment variable",
+                "Please check Env variables or pass directly",
+            )
 
         self.api_version = "v1"
         self.current_path = ""
 
         token_test = self.token_lookup()
 
     def _set_headers(self):
         return {
             "Content-type": "application/json",
             "X-Vault-Token": self.token,
             "X-Vault-Namespace": self.namespace,
         }
 
     def _format_url(self, path):
+        self.current_path = path
         url = f"{self.api_version}/{path}".replace("//", "/")
         url = f"{self.addr.rstrip('/')}/{url}"
         return url
 
     def _format_response(self, response, accepted_status_codes):
         if response.status_code in accepted_status_codes:
             try:
@@ -65,20 +74,29 @@
                     return json_response["data"]
                 else:
                     return json_response
             except ValueError:
                 return {}
         else:
             if response.status_code == 403:
-                raise VAPIPermissionDeniedError(str(response.json()["errors"]))
+                raise VAPIPermissionDeniedError(
+                    f"Vault returned 403 for path {self.current_path}",
+                    response.status_code,
+                    errors=response.json()["errors"],
+                )
             if response.status_code == 503:
-                raise VAPISealedError(str(response.json()["errors"]))
+                raise VAPISealedError(
+                    f"Vault returned 503 for path {self.current_path} and is likely sealed",
+                    response.status_code,
+                    errors=response.json()["errors"],
+                )
             if response.status_code in [200, 204]:
                 raise VAPIAcceptedStatusCodeError(
-                    f"Vault Response Status Code {response.status_code} not in Accepted Range {', '.join(item) for item in accepted_status_codes}"
+                    f"Vault Response Status Code {response.status_code} for path {self.current_path} not in Accepted Range {', '.join(item) for item in accepted_status_codes}",
+                    response.status_code,
                 )
 
             raise VAPIGenericError(response.text)
 
         try:
             return response.json()
         except ValueError:
```

## Comparing `drizzutojr_vapi-0.0.2.dist-info/LICENSE.md` & `drizzutojr_vapi-0.0.3.dist-info/LICENSE.md`

 * *Files identical despite different names*

