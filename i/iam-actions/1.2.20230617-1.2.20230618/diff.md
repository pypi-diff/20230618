# Comparing `tmp/iam_actions-1.2.20230617.tar.gz` & `tmp/iam_actions-1.2.20230618.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230617.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230618.tar", max compression
```

## Comparing `iam_actions-1.2.20230617.tar` & `iam_actions-1.2.20230618.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-06-17 02:31:19.037263 iam_actions-1.2.20230617/LICENSE
--rw-r--r--   0        0        0     2302 2023-06-17 02:31:19.037263 iam_actions-1.2.20230617/README.md
--rw-r--r--   0        0        0      228 2023-06-17 02:31:19.037263 iam_actions-1.2.20230617/iam_actions/__init__.py
--rw-r--r--   0        0        0  4326719 2023-06-17 02:32:44.581665 iam_actions-1.2.20230617/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-06-17 02:31:19.037263 iam_actions-1.2.20230617/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-06-17 02:31:19.037263 iam_actions-1.2.20230617/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-06-17 02:31:19.037263 iam_actions-1.2.20230617/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-06-17 02:31:19.037263 iam_actions-1.2.20230617/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-06-17 02:31:19.037263 iam_actions-1.2.20230617/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-06-17 02:31:19.037263 iam_actions-1.2.20230617/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-06-17 02:31:19.037263 iam_actions-1.2.20230617/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-06-17 02:31:19.037263 iam_actions-1.2.20230617/iam_actions/generate/services.py
--rw-r--r--   0        0        0   556740 2023-06-17 02:32:44.581665 iam_actions-1.2.20230617/iam_actions/policies.json
--rw-r--r--   0        0        0   196395 2023-06-17 02:32:44.581665 iam_actions-1.2.20230617/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   540016 2023-06-17 02:32:44.581665 iam_actions-1.2.20230617/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-06-17 02:32:45.585669 iam_actions-1.2.20230617/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230617/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230617/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-18 02:47:26.429566 iam_actions-1.2.20230618/LICENSE
+-rw-r--r--   0        0        0     2302 2023-06-18 02:47:26.429566 iam_actions-1.2.20230618/README.md
+-rw-r--r--   0        0        0      228 2023-06-18 02:47:26.429566 iam_actions-1.2.20230618/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4326719 2023-06-18 02:49:07.461741 iam_actions-1.2.20230618/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-06-18 02:47:26.429566 iam_actions-1.2.20230618/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-06-18 02:47:26.429566 iam_actions-1.2.20230618/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-06-18 02:47:26.429566 iam_actions-1.2.20230618/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-06-18 02:47:26.429566 iam_actions-1.2.20230618/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-06-18 02:47:26.429566 iam_actions-1.2.20230618/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-06-18 02:47:26.429566 iam_actions-1.2.20230618/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-06-18 02:47:26.429566 iam_actions-1.2.20230618/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-06-18 02:47:26.429566 iam_actions-1.2.20230618/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   556740 2023-06-18 02:49:07.461741 iam_actions-1.2.20230618/iam_actions/policies.json
+-rw-r--r--   0        0        0   196395 2023-06-18 02:49:07.461741 iam_actions-1.2.20230618/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   540016 2023-06-18 02:49:07.461741 iam_actions-1.2.20230618/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-06-18 02:49:08.201741 iam_actions-1.2.20230618/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230618/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230618/PKG-INFO
```

### Comparing `iam_actions-1.2.20230617/LICENSE` & `iam_actions-1.2.20230618/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230617/README.md` & `iam_actions-1.2.20230618/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230617/iam_actions/actions.json` & `iam_actions-1.2.20230618/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -17284,297 +17284,297 @@
             "access_level": "Undocumented",
             "action": "GetSchemaAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "CreateMembership": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "CreateMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartProtectedQuery": {
+        "GetCollaboration": {
             "access_level": "Undocumented",
-            "action": "StartProtectedQuery",
+            "action": "GetCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMembers": {
+        "GetMembership": {
             "access_level": "Undocumented",
-            "action": "ListMembers",
+            "action": "GetMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProtectedQueries": {
+        "GetConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "ListProtectedQueries",
+            "action": "GetConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTable": {
+        "CreateConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTable",
+            "action": "CreateConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCollaboration": {
+        "UpdateMembership": {
             "access_level": "Undocumented",
-            "action": "DeleteCollaboration",
+            "action": "UpdateMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMembership": {
+        "GetConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "CreateMembership",
+            "action": "GetConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProtectedQuery": {
+        "CreateConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "UpdateProtectedQuery",
+            "action": "CreateConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTable": {
+        "UpdateConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTable",
+            "action": "UpdateConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProtectedQuery": {
+        "DeleteConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "GetProtectedQuery",
+            "action": "DeleteConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTableAssociation": {
+        "UpdateProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTableAssociation",
+            "action": "UpdateProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSchemas": {
+        "CreateConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "ListSchemas",
+            "action": "CreateConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetSchema": {
+        "StartProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "BatchGetSchema",
+            "action": "StartProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborations": {
+        "GetProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "ListCollaborations",
+            "action": "GetProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeleteCollaboration": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeleteCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMembership": {
+        "UpdateConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "UpdateMembership",
+            "action": "UpdateConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTableAssociation": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTableAssociation",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConfiguredTableAssociations": {
+        "GetConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "ListConfiguredTableAssociations",
+            "action": "GetConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMemberships": {
+        "CreateCollaboration": {
             "access_level": "Undocumented",
-            "action": "ListMemberships",
+            "action": "CreateCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTableAnalysisRule": {
+        "DeleteConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTableAnalysisRule",
+            "action": "DeleteConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTableAssociation": {
+        "DeleteMember": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTableAssociation",
+            "action": "DeleteMember",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTable": {
+        "ListMembers": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTable",
+            "action": "ListMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTableAnalysisRule": {
+        "DeleteConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTableAnalysisRule",
+            "action": "DeleteConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTableAssociation": {
+        "BatchGetSchema": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTableAssociation",
+            "action": "BatchGetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConfiguredTables": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListConfiguredTables",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMember": {
+        "UpdateCollaboration": {
             "access_level": "Undocumented",
-            "action": "DeleteMember",
+            "action": "UpdateCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListMemberships": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListMemberships",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateCollaboration": {
+        "ListProtectedQueries": {
             "access_level": "Undocumented",
-            "action": "UpdateCollaboration",
+            "action": "ListProtectedQueries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTableAnalysisRule": {
+        "ListConfiguredTableAssociations": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTableAnalysisRule",
+            "action": "ListConfiguredTableAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateCollaboration": {
+        "DeleteMembership": {
             "access_level": "Undocumented",
-            "action": "CreateCollaboration",
+            "action": "DeleteMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMembership": {
+        "ListConfiguredTables": {
             "access_level": "Undocumented",
-            "action": "GetMembership",
+            "action": "ListConfiguredTables",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTable": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTable",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMembership": {
+        "GetSchema": {
             "access_level": "Undocumented",
-            "action": "DeleteMembership",
+            "action": "GetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchema": {
+        "ListSchemas": {
             "access_level": "Undocumented",
-            "action": "GetSchema",
+            "action": "ListSchemas",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTableAnalysisRule": {
+        "UpdateConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTableAnalysisRule",
+            "action": "UpdateConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCollaboration": {
+        "ListCollaborations": {
             "access_level": "Undocumented",
-            "action": "GetCollaboration",
+            "action": "ListCollaborations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "cloud9": {
@@ -24947,113 +24947,113 @@
             "access_level": "Undocumented",
             "action": "CreateUploadUrl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetScan": {
+        "ListFindingsMetrics": {
             "access_level": "Undocumented",
-            "action": "GetScan",
+            "action": "ListFindingsMetrics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFindings": {
+        "BatchGetFindings": {
             "access_level": "Undocumented",
-            "action": "ListFindings",
+            "action": "BatchGetFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountConfiguration": {
+        "ListScans": {
             "access_level": "Undocumented",
-            "action": "GetAccountConfiguration",
+            "action": "ListScans",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetricsSummary": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetMetricsSummary",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountConfiguration": {
+        "GetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountConfiguration",
+            "action": "GetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetFindings": {
+        "UpdateAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "BatchGetFindings",
+            "action": "UpdateAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateScan": {
+        "GetFindings": {
             "access_level": "Undocumented",
-            "action": "CreateScan",
+            "action": "GetFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListScans": {
+        "GetScan": {
             "access_level": "Undocumented",
-            "action": "ListScans",
+            "action": "GetScan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFindings": {
+        "CreateScan": {
             "access_level": "Undocumented",
-            "action": "GetFindings",
+            "action": "CreateScan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFindingsMetrics": {
+        "GetMetricsSummary": {
             "access_level": "Undocumented",
-            "action": "ListFindingsMetrics",
+            "action": "GetMetricsSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListTagsForResource": {
             "access_level": "Undocumented",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListFindings": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteScansByCategory": {
             "access_level": "Undocumented",
@@ -32622,43 +32622,43 @@
             "orphan": false,
             "resources": [
                 "campaign"
             ]
         }
     },
     "consoleapp": {
-        "GetDeviceIdentity": {
+        "ListDeviceIdentities": {
             "access_level": "Undocumented",
-            "action": "GetDeviceIdentity",
+            "action": "ListDeviceIdentities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceIdentities": {
+        "GetDeviceIdentity": {
             "access_level": "Undocumented",
-            "action": "ListDeviceIdentities",
+            "action": "GetDeviceIdentity",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "consolidatedbilling": {
-        "ListLinkedAccounts": {
+        "GetAccountBillingRole": {
             "access_level": "Undocumented",
-            "action": "ListLinkedAccounts",
+            "action": "GetAccountBillingRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountBillingRole": {
+        "ListLinkedAccounts": {
             "access_level": "Undocumented",
-            "action": "GetAccountBillingRole",
+            "action": "ListLinkedAccounts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "controltower": {
@@ -33092,25 +33092,25 @@
             "access_level": "Undocumented",
             "action": "GetCustomerVerificationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateCustomerVerificationDetails": {
+        "UpdateCustomerVerificationDetails": {
             "access_level": "Undocumented",
-            "action": "CreateCustomerVerificationDetails",
+            "action": "UpdateCustomerVerificationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateCustomerVerificationDetails": {
+        "CreateCustomerVerificationDetails": {
             "access_level": "Undocumented",
-            "action": "UpdateCustomerVerificationDetails",
+            "action": "CreateCustomerVerificationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "databrew": {
@@ -34754,33 +34754,33 @@
             "orphan": false,
             "resources": [
                 "taskexecution"
             ]
         }
     },
     "datazone": {
-        "ListProjects": {
+        "GetProject": {
             "access_level": "Undocumented",
-            "action": "ListProjects",
+            "action": "GetProject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProjectConfiguration": {
+        "ListProjects": {
             "access_level": "Undocumented",
-            "action": "GetProjectConfiguration",
+            "action": "ListProjects",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProject": {
+        "GetProjectConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetProject",
+            "action": "GetProjectConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetProjectCredentials": {
             "access_level": "Undocumented",
@@ -34796,241 +34796,241 @@
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "datazonecontrol": {
-        "UpdateDataSource": {
+        "ListDataSources": {
             "access_level": "Undocumented",
-            "action": "UpdateDataSource",
+            "action": "ListDataSources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReviewAccountAssociationInvitation": {
+        "ListMetadataCollectorRuns": {
             "access_level": "Undocumented",
-            "action": "ReviewAccountAssociationInvitation",
+            "action": "ListMetadataCollectorRuns",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "UpdateEnvironment": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "UpdateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSourcesByEnvironment": {
+        "CreateEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListDataSourcesByEnvironment",
+            "action": "CreateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUserPortalLoginAuthCode": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetUserPortalLoginAuthCode",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDomains": {
+        "CreateAccountAssociationInvitation": {
             "access_level": "Undocumented",
-            "action": "ListDomains",
+            "action": "CreateAccountAssociationInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMetadataCollectorRuns": {
+        "ListDataSourcesByEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListMetadataCollectorRuns",
+            "action": "ListDataSourcesByEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironment": {
+        "CreateDataSource": {
             "access_level": "Undocumented",
-            "action": "ListEnvironment",
+            "action": "CreateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDomain": {
+        "DeleteDataSource": {
             "access_level": "Undocumented",
-            "action": "GetDomain",
+            "action": "DeleteDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironment": {
+        "DeleteEnvironment": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironment",
+            "action": "DeleteEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "UpdateDataSource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "UpdateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAssociatedDomain": {
+        "ListMetadataCollectors": {
             "access_level": "Undocumented",
-            "action": "GetAssociatedDomain",
+            "action": "ListMetadataCollectors",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDataSource": {
+        "GetUserPortalLoginAuthCode": {
             "access_level": "Undocumented",
-            "action": "CreateDataSource",
+            "action": "GetUserPortalLoginAuthCode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccountAssociationInvitations": {
+        "GetAssociatedDomain": {
             "access_level": "Undocumented",
-            "action": "ListAccountAssociationInvitations",
+            "action": "GetAssociatedDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEnvironment": {
+        "GetDomain": {
             "access_level": "Undocumented",
-            "action": "CreateEnvironment",
+            "action": "GetDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAssociatedEnvironments": {
+        "ListProjects": {
             "access_level": "Undocumented",
-            "action": "ListAssociatedEnvironments",
+            "action": "ListProjects",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountAssociationDescription": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountAssociationDescription",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSources": {
+        "ListAccountAssociationInvitations": {
             "access_level": "Undocumented",
-            "action": "ListDataSources",
+            "action": "ListAccountAssociationInvitations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DissociateAccount": {
+        "UpdateAccountAssociationDescription": {
             "access_level": "Undocumented",
-            "action": "DissociateAccount",
+            "action": "UpdateAccountAssociationDescription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetadataCollector": {
+        "ListEnvironment": {
             "access_level": "Undocumented",
-            "action": "GetMetadataCollector",
+            "action": "ListEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMetadataCollectors": {
+        "ListAssociatedEnvironments": {
             "access_level": "Undocumented",
-            "action": "ListMetadataCollectors",
+            "action": "ListAssociatedEnvironments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetDataSourceByEnvironment": {
             "access_level": "Undocumented",
             "action": "GetDataSourceByEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAccountAssociationInvitation": {
+        "GetMetadataCollector": {
             "access_level": "Undocumented",
-            "action": "CreateAccountAssociationInvitation",
+            "action": "GetMetadataCollector",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEnvironment": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteEnvironment",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProjects": {
+        "GetEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListProjects",
+            "action": "GetEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDataSource": {
+        "DissociateAccount": {
             "access_level": "Undocumented",
-            "action": "DeleteDataSource",
+            "action": "DissociateAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListDomains": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListDomains",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironment": {
+        "ListAllAssociatedAccountsForEnvironment": {
             "access_level": "Undocumented",
-            "action": "GetEnvironment",
+            "action": "ListAllAssociatedAccountsForEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAllAssociatedAccountsForEnvironment": {
+        "ReviewAccountAssociationInvitation": {
             "access_level": "Undocumented",
-            "action": "ListAllAssociatedAccountsForEnvironment",
+            "action": "ReviewAccountAssociationInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "dax": {
@@ -56550,225 +56550,225 @@
             ],
             "description": "Grants permission to replace the current set of policies for the specified load balancer port with the specified set of policies",
             "orphan": false,
             "resources": [
                 "loadbalancer"
             ]
         },
-        "RemoveListenerCertificates": {
+        "SetSecurityGroups": {
             "access_level": "Undocumented",
-            "action": "RemoveListenerCertificates",
+            "action": "SetSecurityGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTargetGroupAttributes": {
+        "DescribeTargetHealth": {
             "access_level": "Undocumented",
-            "action": "DescribeTargetGroupAttributes",
+            "action": "DescribeTargetHealth",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetWebAcl": {
+        "DeleteRule": {
             "access_level": "Undocumented",
-            "action": "SetWebAcl",
+            "action": "DeleteRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSecurityGroups": {
+        "CreateRule": {
             "access_level": "Undocumented",
-            "action": "SetSecurityGroups",
+            "action": "CreateRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeSSLPolicies": {
+        "DeleteListener": {
             "access_level": "Undocumented",
-            "action": "DescribeSSLPolicies",
+            "action": "DeleteListener",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddListenerCertificates": {
+        "SetRulePriorities": {
             "access_level": "Undocumented",
-            "action": "AddListenerCertificates",
+            "action": "SetRulePriorities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeRules": {
+        "AddListenerCertificates": {
             "access_level": "Undocumented",
-            "action": "DescribeRules",
+            "action": "AddListenerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyListener": {
+        "ModifyRule": {
             "access_level": "Undocumented",
-            "action": "ModifyListener",
+            "action": "ModifyRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetIpAddressType": {
+        "DescribeAccountLimits": {
             "access_level": "Undocumented",
-            "action": "SetIpAddressType",
+            "action": "DescribeAccountLimits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterTargets": {
+        "SetIpAddressType": {
             "access_level": "Undocumented",
-            "action": "DeregisterTargets",
+            "action": "SetIpAddressType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeListenerCertificates": {
+        "DescribeTargetGroups": {
             "access_level": "Undocumented",
-            "action": "DescribeListenerCertificates",
+            "action": "DescribeTargetGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSubnets": {
+        "RegisterTargets": {
             "access_level": "Undocumented",
-            "action": "SetSubnets",
+            "action": "RegisterTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTargetGroup": {
+        "DeleteTargetGroup": {
             "access_level": "Undocumented",
-            "action": "CreateTargetGroup",
+            "action": "DeleteTargetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTargetHealth": {
+        "ModifyListener": {
             "access_level": "Undocumented",
-            "action": "DescribeTargetHealth",
+            "action": "ModifyListener",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeListeners": {
+        "DescribeListenerCertificates": {
             "access_level": "Undocumented",
-            "action": "DescribeListeners",
+            "action": "DescribeListenerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTargetGroup": {
+        "SetWebAcl": {
             "access_level": "Undocumented",
-            "action": "DeleteTargetGroup",
+            "action": "SetWebAcl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRule": {
+        "DescribeTargetGroupAttributes": {
             "access_level": "Undocumented",
-            "action": "DeleteRule",
+            "action": "DescribeTargetGroupAttributes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyRule": {
+        "ModifyTargetGroup": {
             "access_level": "Undocumented",
-            "action": "ModifyRule",
+            "action": "ModifyTargetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyTargetGroupAttributes": {
+        "RemoveListenerCertificates": {
             "access_level": "Undocumented",
-            "action": "ModifyTargetGroupAttributes",
+            "action": "RemoveListenerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTargetGroups": {
+        "DescribeSSLPolicies": {
             "access_level": "Undocumented",
-            "action": "DescribeTargetGroups",
+            "action": "DescribeSSLPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetRulePriorities": {
+        "ModifyTargetGroupAttributes": {
             "access_level": "Undocumented",
-            "action": "SetRulePriorities",
+            "action": "ModifyTargetGroupAttributes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteListener": {
+        "CreateListener": {
             "access_level": "Undocumented",
-            "action": "DeleteListener",
+            "action": "CreateListener",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterTargets": {
+        "SetSubnets": {
             "access_level": "Undocumented",
-            "action": "RegisterTargets",
+            "action": "SetSubnets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateListener": {
+        "DeregisterTargets": {
             "access_level": "Undocumented",
-            "action": "CreateListener",
+            "action": "DeregisterTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRule": {
+        "DescribeRules": {
             "access_level": "Undocumented",
-            "action": "CreateRule",
+            "action": "DescribeRules",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyTargetGroup": {
+        "CreateTargetGroup": {
             "access_level": "Undocumented",
-            "action": "ModifyTargetGroup",
+            "action": "CreateTargetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAccountLimits": {
+        "DescribeListeners": {
             "access_level": "Undocumented",
-            "action": "DescribeAccountLimits",
+            "action": "DescribeListeners",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "elasticmapreduce": {
@@ -63310,33 +63310,33 @@
             "condition_keys": [],
             "description": "Grants permission to verify the email for FreeRTOS extended maintenance plan (EMP)",
             "orphan": false,
             "resources": []
         }
     },
     "freetier": {
-        "GetFreeTierUsage": {
+        "GetFreeTierAlertPreference": {
             "access_level": "Undocumented",
-            "action": "GetFreeTierUsage",
+            "action": "GetFreeTierAlertPreference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFreeTierAlertPreference": {
+        "PutFreeTierAlertPreference": {
             "access_level": "Undocumented",
-            "action": "GetFreeTierAlertPreference",
+            "action": "PutFreeTierAlertPreference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutFreeTierAlertPreference": {
+        "GetFreeTierUsage": {
             "access_level": "Undocumented",
-            "action": "PutFreeTierAlertPreference",
+            "action": "GetFreeTierUsage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "fsx": {
@@ -71807,1249 +71807,1249 @@
             "condition_keys": [],
             "description": "Grants permission to update an Amazon Honeycode team for your AWS Account",
             "orphan": false,
             "resources": []
         }
     },
     "iam": {
-        "DetachUserPolicy": {
+        "DeleteServiceLinkedRole": {
             "access_level": "Undocumented",
-            "action": "DetachUserPolicy",
+            "action": "DeleteServiceLinkedRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRolePolicy": {
+        "PutRolePolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteRolePolicy",
+            "action": "PutRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicies": {
+        "CreateAccessKey": {
             "access_level": "Undocumented",
-            "action": "ListPolicies",
+            "action": "CreateAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachRolePolicy": {
+        "UploadSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "AttachRolePolicy",
+            "action": "UploadSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOrganizationsAccessReport": {
+        "ListPolicyVersions": {
             "access_level": "Undocumented",
-            "action": "GetOrganizationsAccessReport",
+            "action": "ListPolicyVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddRoleToInstanceProfile": {
+        "UploadSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "AddRoleToInstanceProfile",
+            "action": "UploadSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddClientIDToOpenIDConnectProvider": {
+        "ListSSHPublicKeys": {
             "access_level": "Undocumented",
-            "action": "AddClientIDToOpenIDConnectProvider",
+            "action": "ListSSHPublicKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOpenIDConnectProviders": {
+        "ListServerCertificateTags": {
             "access_level": "Undocumented",
-            "action": "ListOpenIDConnectProviders",
+            "action": "ListServerCertificateTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUser": {
+        "ListUserTags": {
             "access_level": "Undocumented",
-            "action": "CreateUser",
+            "action": "ListUserTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSSHPublicKey": {
+        "CreatePolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteSSHPublicKey",
+            "action": "CreatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagPolicy": {
+        "CreateGroup": {
             "access_level": "Undocumented",
-            "action": "TagPolicy",
+            "action": "CreateGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachGroupPolicy": {
+        "GetSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "DetachGroupPolicy",
+            "action": "GetSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccountAlias": {
+        "GetSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "DeleteAccountAlias",
+            "action": "GetSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLinkedRoleDeletionStatus": {
+        "DeleteRolePolicy": {
             "access_level": "Undocumented",
-            "action": "GetServiceLinkedRoleDeletionStatus",
+            "action": "DeleteRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRole": {
+        "GetAccountSummary": {
             "access_level": "Undocumented",
-            "action": "DeleteRole",
+            "action": "GetAccountSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOpenIDConnectProvider": {
+        "DeleteServerCertificate": {
             "access_level": "Undocumented",
-            "action": "GetOpenIDConnectProvider",
+            "action": "DeleteServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRolePolicy": {
+        "UpdateCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "PutRolePolicy",
+            "action": "UpdateCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SimulateCustomPolicy": {
+        "DeleteGroup": {
             "access_level": "Undocumented",
-            "action": "SimulateCustomPolicy",
+            "action": "DeleteGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceLinkedRole": {
+        "DeleteSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceLinkedRole",
+            "action": "DeleteSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableMFADevice": {
+        "AttachGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "EnableMFADevice",
+            "action": "AttachGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResyncMFADevice": {
+        "GetAccountName": {
             "access_level": "Undocumented",
-            "action": "ResyncMFADevice",
+            "action": "GetAccountName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRoles": {
+        "GetServiceLinkedRoleDeletionStatus": {
             "access_level": "Undocumented",
-            "action": "ListRoles",
+            "action": "GetServiceLinkedRoleDeletionStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEntitiesForPolicy": {
+        "GetContextKeysForCustomPolicy": {
             "access_level": "Undocumented",
-            "action": "ListEntitiesForPolicy",
+            "action": "GetContextKeysForCustomPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagPolicy": {
+        "CreateRole": {
             "access_level": "Undocumented",
-            "action": "UntagPolicy",
+            "action": "CreateRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRolePolicies": {
+        "ListSAMLProviders": {
             "access_level": "Undocumented",
-            "action": "ListRolePolicies",
+            "action": "ListSAMLProviders",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagRole": {
+        "UntagOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "TagRole",
+            "action": "UntagOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagRole": {
+        "DeleteRole": {
             "access_level": "Undocumented",
-            "action": "UntagRole",
+            "action": "DeleteRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountEmailAddress": {
+        "ListSigningCertificates": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountEmailAddress",
+            "action": "ListSigningCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfilesForRole": {
+        "GenerateOrganizationsAccessReport": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfilesForRole",
+            "action": "GenerateOrganizationsAccessReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUserPolicy": {
+        "GetAccountAuthorizationDetails": {
             "access_level": "Undocumented",
-            "action": "GetUserPolicy",
+            "action": "GetAccountAuthorizationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateServerCertificate": {
+        "DeleteGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateServerCertificate",
+            "action": "DeleteGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeactivateMFADevice": {
+        "UpdateAssumeRolePolicy": {
             "access_level": "Undocumented",
-            "action": "DeactivateMFADevice",
+            "action": "UpdateAssumeRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveClientIDFromOpenIDConnectProvider": {
+        "DeletePolicy": {
             "access_level": "Undocumented",
-            "action": "RemoveClientIDFromOpenIDConnectProvider",
+            "action": "DeletePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagOpenIDConnectProvider": {
+        "ListSAMLProviderTags": {
             "access_level": "Undocumented",
-            "action": "TagOpenIDConnectProvider",
+            "action": "ListSAMLProviderTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAssumeRolePolicy": {
+        "ResyncMFADevice": {
             "access_level": "Undocumented",
-            "action": "UpdateAssumeRolePolicy",
+            "action": "ResyncMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccessKeys": {
+        "DeactivateMFADevice": {
             "access_level": "Undocumented",
-            "action": "ListAccessKeys",
+            "action": "DeactivateMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInstanceProfile": {
+        "GetGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "GetInstanceProfile",
+            "action": "GetGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagOpenIDConnectProvider": {
+        "GetInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "UntagOpenIDConnectProvider",
+            "action": "GetInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccountPasswordPolicy": {
+        "UntagInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteAccountPasswordPolicy",
+            "action": "UntagInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedGroupPolicies": {
+        "ListGroups": {
             "access_level": "Undocumented",
-            "action": "ListAttachedGroupPolicies",
+            "action": "ListGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRolePolicy": {
+        "EnableMFADevice": {
             "access_level": "Undocumented",
-            "action": "GetRolePolicy",
+            "action": "EnableMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServerCertificate": {
+        "UpdateOpenIDConnectProviderThumbprint": {
             "access_level": "Undocumented",
-            "action": "GetServerCertificate",
+            "action": "UpdateOpenIDConnectProviderThumbprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagUser": {
+        "ListAttachedRolePolicies": {
             "access_level": "Undocumented",
-            "action": "UntagUser",
+            "action": "ListAttachedRolePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLastAccessedDetails": {
+        "DetachUserPolicy": {
             "access_level": "Undocumented",
-            "action": "GetServiceLastAccessedDetails",
+            "action": "DetachUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddUserToGroup": {
+        "GetUser": {
             "access_level": "Undocumented",
-            "action": "AddUserToGroup",
+            "action": "GetUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSAMLProviders": {
+        "UpdateServerCertificate": {
             "access_level": "Undocumented",
-            "action": "ListSAMLProviders",
+            "action": "UpdateServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserPolicies": {
+        "DeleteOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "ListUserPolicies",
+            "action": "DeleteOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLoginProfile": {
+        "UpdateSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "GetLoginProfile",
+            "action": "UpdateSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagUser": {
+        "ListMFADevices": {
             "access_level": "Undocumented",
-            "action": "TagUser",
+            "action": "ListMFADevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMFADeviceTags": {
+        "DetachGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "ListMFADeviceTags",
+            "action": "DetachGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServerCertificateTags": {
+        "PutGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "ListServerCertificateTags",
+            "action": "PutGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicy": {
+        "CreateUser": {
             "access_level": "Undocumented",
-            "action": "CreatePolicy",
+            "action": "CreateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteOpenIDConnectProvider": {
+        "DeleteCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "DeleteOpenIDConnectProvider",
+            "action": "DeleteCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSTSRegionalEndpointsStatus": {
+        "UpdateSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "ListSTSRegionalEndpointsStatus",
+            "action": "UpdateSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadServerCertificate": {
+        "UpdateGroup": {
             "access_level": "Undocumented",
-            "action": "UploadServerCertificate",
+            "action": "UpdateGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadSigningCertificate": {
+        "GetOrganizationsAccessReport": {
             "access_level": "Undocumented",
-            "action": "UploadSigningCertificate",
+            "action": "GetOrganizationsAccessReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ChangePassword": {
+        "GetCredentialReport": {
             "access_level": "Undocumented",
-            "action": "ChangePassword",
+            "action": "GetCredentialReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountAuthorizationDetails": {
+        "ListAccessKeys": {
             "access_level": "Undocumented",
-            "action": "GetAccountAuthorizationDetails",
+            "action": "ListAccessKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteInstanceProfile": {
+        "GetRole": {
             "access_level": "Undocumented",
-            "action": "DeleteInstanceProfile",
+            "action": "GetRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateOpenIDConnectProviderThumbprint": {
+        "ListPolicies": {
             "access_level": "Undocumented",
-            "action": "UpdateOpenIDConnectProviderThumbprint",
+            "action": "ListPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateServiceLastAccessedDetails": {
+        "GetRolePolicy": {
             "access_level": "Undocumented",
-            "action": "GenerateServiceLastAccessedDetails",
+            "action": "GetRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachRolePolicy": {
+        "GetServiceLastAccessedDetailsWithEntities": {
             "access_level": "Undocumented",
-            "action": "DetachRolePolicy",
+            "action": "GetServiceLastAccessedDetailsWithEntities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSSHPublicKeys": {
+        "ListGroupPolicies": {
             "access_level": "Undocumented",
-            "action": "ListSSHPublicKeys",
+            "action": "ListGroupPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccessKey": {
+        "UntagServerCertificate": {
             "access_level": "Undocumented",
-            "action": "DeleteAccessKey",
+            "action": "UntagServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyVersion": {
+        "ListRoleTags": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyVersion",
+            "action": "ListRoleTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSAMLProvider": {
+        "ListRolePolicies": {
             "access_level": "Undocumented",
-            "action": "GetSAMLProvider",
+            "action": "ListRolePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetDefaultPolicyVersion": {
+        "UpdateLoginProfile": {
             "access_level": "Undocumented",
-            "action": "SetDefaultPolicyVersion",
+            "action": "UpdateLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContextKeysForCustomPolicy": {
+        "UpdateServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "GetContextKeysForCustomPolicy",
+            "action": "UpdateServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRole": {
+        "GetAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "GetRole",
+            "action": "GetAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUserPolicy": {
+        "UpdateRole": {
             "access_level": "Undocumented",
-            "action": "DeleteUserPolicy",
+            "action": "UpdateRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSAMLProviderTags": {
+        "GetPolicy": {
             "access_level": "Undocumented",
-            "action": "ListSAMLProviderTags",
+            "action": "GetPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroups": {
+        "SimulateCustomPolicy": {
             "access_level": "Undocumented",
-            "action": "ListGroups",
+            "action": "SimulateCustomPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetServiceSpecificCredential": {
+        "PutRolePermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "ResetServiceSpecificCredential",
+            "action": "PutRolePermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountName": {
+        "TagSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountName",
+            "action": "TagSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateOpenIDConnectProvider": {
+        "DeleteServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "CreateOpenIDConnectProvider",
+            "action": "DeleteServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateVirtualMFADevice": {
+        "ListSTSRegionalEndpointsStatus": {
             "access_level": "Undocumented",
-            "action": "CreateVirtualMFADevice",
+            "action": "ListSTSRegionalEndpointsStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServerCertificates": {
+        "SetSTSRegionalEndpointStatus": {
             "access_level": "Undocumented",
-            "action": "ListServerCertificates",
+            "action": "SetSTSRegionalEndpointStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccessKeyLastUsed": {
+        "UntagSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "GetAccessKeyLastUsed",
+            "action": "UntagSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGroup": {
+        "AddRoleToInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "CreateGroup",
+            "action": "AddRoleToInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateServiceSpecificCredential": {
+        "CreateAccountAlias": {
             "access_level": "Undocumented",
-            "action": "UpdateServiceSpecificCredential",
+            "action": "CreateAccountAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSAMLProvider": {
+        "DetachRolePolicy": {
             "access_level": "Undocumented",
-            "action": "CreateSAMLProvider",
+            "action": "DetachRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountPasswordPolicy": {
+        "CreateServiceLinkedRole": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountPasswordPolicy",
+            "action": "CreateServiceLinkedRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteVirtualMFADevice": {
+        "GetOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "DeleteVirtualMFADevice",
+            "action": "GetOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagMFADevice": {
+        "RemoveRoleFromInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "TagMFADevice",
+            "action": "RemoveRoleFromInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUser": {
+        "ListAttachedGroupPolicies": {
             "access_level": "Undocumented",
-            "action": "DeleteUser",
+            "action": "ListAttachedGroupPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRolePermissionsBoundary": {
+        "ListInstanceProfileTags": {
             "access_level": "Undocumented",
-            "action": "DeleteRolePermissionsBoundary",
+            "action": "ListInstanceProfileTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAccountAlias": {
+        "RemoveClientIDFromOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "CreateAccountAlias",
+            "action": "RemoveClientIDFromOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateInstanceProfile": {
+        "AddClientIDToOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "CreateInstanceProfile",
+            "action": "AddClientIDToOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyVersions": {
+        "GetPolicyVersion": {
             "access_level": "Undocumented",
-            "action": "ListPolicyVersions",
+            "action": "GetPolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCloudFrontPublicKey": {
+        "TagOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "DeleteCloudFrontPublicKey",
+            "action": "TagOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountName": {
+        "DeleteAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "GetAccountName",
+            "action": "DeleteAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfiles": {
+        "TagUser": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfiles",
+            "action": "TagUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCloudFrontPublicKeys": {
+        "CreateOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "ListCloudFrontPublicKeys",
+            "action": "CreateOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUserPermissionsBoundary": {
+        "TagMFADevice": {
             "access_level": "Undocumented",
-            "action": "DeleteUserPermissionsBoundary",
+            "action": "TagMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccessKey": {
+        "TagInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateAccessKey",
+            "action": "TagInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteLoginProfile": {
+        "ResetServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "DeleteLoginProfile",
+            "action": "ResetServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateLoginProfile": {
+        "CreateVirtualMFADevice": {
             "access_level": "Undocumented",
-            "action": "CreateLoginProfile",
+            "action": "CreateVirtualMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagMFADevice": {
+        "ListMFADeviceTags": {
             "access_level": "Undocumented",
-            "action": "UntagMFADevice",
+            "action": "ListMFADeviceTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSecurityTokenServicePreferences": {
+        "ListUsers": {
             "access_level": "Undocumented",
-            "action": "SetSecurityTokenServicePreferences",
+            "action": "ListUsers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceLinkedRole": {
+        "ListVirtualMFADevices": {
             "access_level": "Undocumented",
-            "action": "CreateServiceLinkedRole",
+            "action": "ListVirtualMFADevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSigningCertificate": {
+        "AttachUserPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteSigningCertificate",
+            "action": "AttachUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicyVersion": {
+        "UntagMFADevice": {
             "access_level": "Undocumented",
-            "action": "CreatePolicyVersion",
+            "action": "UntagMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateUser": {
+        "ListServerCertificates": {
             "access_level": "Undocumented",
-            "action": "UpdateUser",
+            "action": "ListServerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachUserPolicy": {
+        "AddUserToGroup": {
             "access_level": "Undocumented",
-            "action": "AttachUserPolicy",
+            "action": "AddUserToGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGroup": {
+        "GetContextKeysForPrincipalPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateGroup",
+            "action": "GetContextKeysForPrincipalPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountPasswordPolicy": {
+        "PutUserPolicy": {
             "access_level": "Undocumented",
-            "action": "GetAccountPasswordPolicy",
+            "action": "PutUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountSummary": {
+        "DeleteAccessKey": {
             "access_level": "Undocumented",
-            "action": "GetAccountSummary",
+            "action": "DeleteAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroupsForUser": {
+        "GetAccountEmailAddress": {
             "access_level": "Undocumented",
-            "action": "ListGroupsForUser",
+            "action": "GetAccountEmailAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagServerCertificate": {
+        "CreateSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "UntagServerCertificate",
+            "action": "CreateSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicyVersion": {
+        "GetCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "GetPolicyVersion",
+            "action": "GetCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSAMLProvider": {
+        "TagServerCertificate": {
             "access_level": "Undocumented",
-            "action": "UpdateSAMLProvider",
+            "action": "TagServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUsers": {
+        "ListPoliciesGrantingServiceAccess": {
             "access_level": "Undocumented",
-            "action": "ListUsers",
+            "action": "ListPoliciesGrantingServiceAccess",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroup": {
+        "ListUserPolicies": {
             "access_level": "Undocumented",
-            "action": "GetGroup",
+            "action": "ListUserPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceSpecificCredential": {
+        "CreateInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceSpecificCredential",
+            "action": "CreateInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSTSRegionalEndpointStatus": {
+        "SetSecurityTokenServicePreferences": {
             "access_level": "Undocumented",
-            "action": "SetSTSRegionalEndpointStatus",
+            "action": "SetSecurityTokenServicePreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedRolePolicies": {
+        "ListGroupsForUser": {
             "access_level": "Undocumented",
-            "action": "ListAttachedRolePolicies",
+            "action": "ListGroupsForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateOrganizationsAccessReport": {
+        "DeleteUserPermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "GenerateOrganizationsAccessReport",
+            "action": "DeleteUserPermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroupPolicies": {
+        "DeleteLoginProfile": {
             "access_level": "Undocumented",
-            "action": "ListGroupPolicies",
+            "action": "DeleteLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGroupPolicy": {
+        "UntagPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteGroupPolicy",
+            "action": "UntagPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveRoleFromInstanceProfile": {
+        "SetDefaultPolicyVersion": {
             "access_level": "Undocumented",
-            "action": "RemoveRoleFromInstanceProfile",
+            "action": "SetDefaultPolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSAMLProvider": {
+        "UpdateAccountEmailAddress": {
             "access_level": "Undocumented",
-            "action": "DeleteSAMLProvider",
+            "action": "UpdateAccountEmailAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfileTags": {
+        "PutUserPermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfileTags",
+            "action": "PutUserPermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUser": {
+        "CreatePolicyVersion": {
             "access_level": "Undocumented",
-            "action": "GetUser",
+            "action": "CreatePolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSSHPublicKey": {
+        "RemoveUserFromGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateSSHPublicKey",
+            "action": "RemoveUserFromGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroupPolicy": {
+        "ListInstanceProfiles": {
             "access_level": "Undocumented",
-            "action": "GetGroupPolicy",
+            "action": "ListInstanceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRolePermissionsBoundary": {
+        "UpdateAccessKey": {
             "access_level": "Undocumented",
-            "action": "PutRolePermissionsBoundary",
+            "action": "UpdateAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateLoginProfile": {
+        "DeleteVirtualMFADevice": {
             "access_level": "Undocumented",
-            "action": "UpdateLoginProfile",
+            "action": "DeleteVirtualMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagInstanceProfile": {
+        "DeletePolicyVersion": {
             "access_level": "Undocumented",
-            "action": "UntagInstanceProfile",
+            "action": "DeletePolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRole": {
+        "UploadServerCertificate": {
             "access_level": "Undocumented",
-            "action": "UpdateRole",
+            "action": "UploadServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContextKeysForPrincipalPolicy": {
+        "UpdateAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "GetContextKeysForPrincipalPolicy",
+            "action": "UpdateAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountEmailAddress": {
+        "UpdateSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "GetAccountEmailAddress",
+            "action": "UpdateSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPoliciesGrantingServiceAccess": {
+        "GetLoginProfile": {
             "access_level": "Undocumented",
-            "action": "ListPoliciesGrantingServiceAccess",
+            "action": "GetLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRoleTags": {
+        "ListServiceSpecificCredentials": {
             "access_level": "Undocumented",
-            "action": "ListRoleTags",
+            "action": "ListServiceSpecificCredentials",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSigningCertificates": {
+        "PassRole": {
             "access_level": "Undocumented",
-            "action": "ListSigningCertificates",
+            "action": "PassRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserTags": {
+        "UntagUser": {
             "access_level": "Undocumented",
-            "action": "ListUserTags",
+            "action": "UntagUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PassRole": {
+        "ListOpenIDConnectProviders": {
             "access_level": "Undocumented",
-            "action": "PassRole",
+            "action": "ListOpenIDConnectProviders",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachGroupPolicy": {
+        "ListPolicyTags": {
             "access_level": "Undocumented",
-            "action": "AttachGroupPolicy",
+            "action": "ListPolicyTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutUserPolicy": {
+        "DeleteRolePermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "PutUserPolicy",
+            "action": "DeleteRolePermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicy": {
+        "ListOpenIDConnectProviderTags": {
             "access_level": "Undocumented",
-            "action": "GetPolicy",
+            "action": "ListOpenIDConnectProviderTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagSAMLProvider": {
+        "GenerateServiceLastAccessedDetails": {
             "access_level": "Undocumented",
-            "action": "UntagSAMLProvider",
+            "action": "GenerateServiceLastAccessedDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveUserFromGroup": {
+        "ListRoles": {
             "access_level": "Undocumented",
-            "action": "RemoveUserFromGroup",
+            "action": "ListRoles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccountAliases": {
+        "CreateServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "ListAccountAliases",
+            "action": "CreateServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicy": {
+        "GenerateCredentialReport": {
             "access_level": "Undocumented",
-            "action": "DeletePolicy",
+            "action": "GenerateCredentialReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateCloudFrontPublicKey": {
+        "CreateLoginProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateCloudFrontPublicKey",
+            "action": "CreateLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListVirtualMFADevices": {
+        "GetServerCertificate": {
             "access_level": "Undocumented",
-            "action": "ListVirtualMFADevices",
+            "action": "GetServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "SimulatePrincipalPolicy": {
             "access_level": "Undocumented",
             "action": "SimulatePrincipalPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagInstanceProfile": {
+        "TagPolicy": {
             "access_level": "Undocumented",
-            "action": "TagInstanceProfile",
+            "action": "TagPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCredentialReport": {
+        "ListAccountAliases": {
             "access_level": "Undocumented",
-            "action": "GetCredentialReport",
+            "action": "ListAccountAliases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRole": {
+        "UntagRole": {
             "access_level": "Undocumented",
-            "action": "CreateRole",
+            "action": "UntagRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagSAMLProvider": {
+        "UpdateUser": {
             "access_level": "Undocumented",
-            "action": "TagSAMLProvider",
+            "action": "UpdateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadSSHPublicKey": {
+        "GetAccessKeyLastUsed": {
             "access_level": "Undocumented",
-            "action": "UploadSSHPublicKey",
+            "action": "GetAccessKeyLastUsed",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGroup": {
+        "ListCloudFrontPublicKeys": {
             "access_level": "Undocumented",
-            "action": "DeleteGroup",
+            "action": "ListCloudFrontPublicKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLastAccessedDetailsWithEntities": {
+        "GetUserPolicy": {
             "access_level": "Undocumented",
-            "action": "GetServiceLastAccessedDetailsWithEntities",
+            "action": "GetUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutGroupPolicy": {
+        "UpdateAccountName": {
             "access_level": "Undocumented",
-            "action": "PutGroupPolicy",
+            "action": "UpdateAccountName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceSpecificCredential": {
+        "GetServiceLastAccessedDetails": {
             "access_level": "Undocumented",
-            "action": "CreateServiceSpecificCredential",
+            "action": "GetServiceLastAccessedDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListAttachedUserPolicies": {
             "access_level": "Undocumented",
@@ -73063,113 +73063,113 @@
             "access_level": "Undocumented",
             "action": "UploadCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAccessKey": {
+        "DeleteUser": {
             "access_level": "Undocumented",
-            "action": "CreateAccessKey",
+            "action": "DeleteUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagServerCertificate": {
+        "DeleteUserPolicy": {
             "access_level": "Undocumented",
-            "action": "TagServerCertificate",
+            "action": "DeleteUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRoleDescription": {
+        "AttachRolePolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateRoleDescription",
+            "action": "AttachRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutUserPermissionsBoundary": {
+        "DeleteSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "PutUserPermissionsBoundary",
+            "action": "DeleteSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMFADevices": {
+        "GetGroup": {
             "access_level": "Undocumented",
-            "action": "ListMFADevices",
+            "action": "GetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServiceSpecificCredentials": {
+        "ListEntitiesForPolicy": {
             "access_level": "Undocumented",
-            "action": "ListServiceSpecificCredentials",
+            "action": "ListEntitiesForPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOpenIDConnectProviderTags": {
+        "ChangePassword": {
             "access_level": "Undocumented",
-            "action": "ListOpenIDConnectProviderTags",
+            "action": "ChangePassword",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServerCertificate": {
+        "TagRole": {
             "access_level": "Undocumented",
-            "action": "DeleteServerCertificate",
+            "action": "TagRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCloudFrontPublicKey": {
+        "DeleteInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "GetCloudFrontPublicKey",
+            "action": "DeleteInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSigningCertificate": {
+        "DeleteSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "UpdateSigningCertificate",
+            "action": "DeleteSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateCredentialReport": {
+        "UpdateRoleDescription": {
             "access_level": "Undocumented",
-            "action": "GenerateCredentialReport",
+            "action": "UpdateRoleDescription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyTags": {
+        "ListInstanceProfilesForRole": {
             "access_level": "Undocumented",
-            "action": "ListPolicyTags",
+            "action": "ListInstanceProfilesForRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSSHPublicKey": {
+        "DeleteAccountAlias": {
             "access_level": "Undocumented",
-            "action": "GetSSHPublicKey",
+            "action": "DeleteAccountAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "identity-sync": {
@@ -75002,33 +75002,33 @@
             "access_level": "Undocumented",
             "action": "GetInvoicePDF",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutInvoiceEmailDeliveryPreferences": {
+        "GetInvoiceEmailDeliveryPreferences": {
             "access_level": "Undocumented",
-            "action": "PutInvoiceEmailDeliveryPreferences",
+            "action": "GetInvoiceEmailDeliveryPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListInvoiceSummaries": {
             "access_level": "Undocumented",
             "action": "ListInvoiceSummaries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInvoiceEmailDeliveryPreferences": {
+        "PutInvoiceEmailDeliveryPreferences": {
             "access_level": "Undocumented",
-            "action": "GetInvoiceEmailDeliveryPreferences",
+            "action": "PutInvoiceEmailDeliveryPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "iot": {
@@ -80935,889 +80935,889 @@
             "orphan": false,
             "resources": [
                 "workspace"
             ]
         }
     },
     "iotwireless": {
-        "DeleteQueuedMessages": {
+        "UpdateDestination": {
             "access_level": "Undocumented",
-            "action": "DeleteQueuedMessages",
+            "action": "UpdateDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMulticastGroup": {
+        "ListQueuedMessages": {
             "access_level": "Undocumented",
-            "action": "GetMulticastGroup",
+            "action": "ListQueuedMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateAwsAccountWithPartnerAccount": {
+        "DisassociateAwsAccountFromPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "AssociateAwsAccountWithPartnerAccount",
+            "action": "DisassociateAwsAccountFromPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDeviceProfile": {
+        "DisassociateWirelessGatewayFromCertificate": {
             "access_level": "Undocumented",
-            "action": "DeleteDeviceProfile",
+            "action": "DisassociateWirelessGatewayFromCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetWirelessGatewayCertificate": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetWirelessGatewayCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithMulticastGroup": {
+        "CreateNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithMulticastGroup",
+            "action": "CreateNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayFirmwareInformation": {
+        "ListMulticastGroupsByFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayFirmwareInformation",
+            "action": "ListMulticastGroupsByFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePosition": {
+        "ListPositionConfigurations": {
             "access_level": "Undocumented",
-            "action": "UpdatePosition",
+            "action": "ListPositionConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromMulticastGroup": {
+        "UpdateWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromMulticastGroup",
+            "action": "UpdateWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithFuotaTask": {
+        "ListNetworkAnalyzerConfigurations": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithFuotaTask",
+            "action": "ListNetworkAnalyzerConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDeviceImportTask": {
+        "TestWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDeviceImportTask",
+            "action": "TestWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromThing": {
+        "DeleteFuotaTask": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromThing",
+            "action": "DeleteFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceProfile": {
+        "DeleteWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "GetServiceProfile",
+            "action": "DeleteWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartNetworkAnalyzerStream": {
+        "ListEventConfigurations": {
             "access_level": "Undocumented",
-            "action": "StartNetworkAnalyzerStream",
+            "action": "ListEventConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceLogLevel": {
+        "GetPositionConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetResourceLogLevel",
+            "action": "GetPositionConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPartnerAccounts": {
+        "GetPositionEstimate": {
             "access_level": "Undocumented",
-            "action": "ListPartnerAccounts",
+            "action": "GetPositionEstimate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessDeviceImportTask": {
+        "StartFuotaTask": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessDeviceImportTask",
+            "action": "StartFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLogLevelsByResourceTypes": {
+        "DisassociateWirelessDeviceFromThing": {
             "access_level": "Undocumented",
-            "action": "GetLogLevelsByResourceTypes",
+            "action": "DisassociateWirelessDeviceFromThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDeviceStatistics": {
+        "AssociateWirelessDeviceWithMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDeviceStatistics",
+            "action": "AssociateWirelessDeviceWithMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDevicesForWirelessDeviceImportTask": {
+        "StartWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "ListDevicesForWirelessDeviceImportTask",
+            "action": "StartWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromFuotaTask": {
+        "GetLogLevelsByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromFuotaTask",
+            "action": "GetLogLevelsByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessGatewayFromCertificate": {
+        "DisassociateWirelessDeviceFromFuotaTask": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessGatewayFromCertificate",
+            "action": "DisassociateWirelessDeviceFromFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGateway": {
+        "GetPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGateway",
+            "action": "GetPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceProfile": {
+        "ListDestinations": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceProfile",
+            "action": "ListDestinations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGatewayTaskDefinition": {
+        "GetWirelessDeviceStatistics": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGatewayTaskDefinition",
+            "action": "GetWirelessDeviceStatistics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDestination": {
+        "GetFuotaTask": {
             "access_level": "Undocumented",
-            "action": "DeleteDestination",
+            "action": "GetFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueuedMessages": {
+        "ListWirelessGatewayTaskDefinitions": {
             "access_level": "Undocumented",
-            "action": "ListQueuedMessages",
+            "action": "ListWirelessGatewayTaskDefinitions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDestination": {
+        "GetEventConfigurationByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "UpdateDestination",
+            "action": "GetEventConfigurationByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceProfile": {
+        "GetNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "CreateServiceProfile",
+            "action": "GetNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessGatewayTaskDefinitions": {
+        "UpdateMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "ListWirelessGatewayTaskDefinitions",
+            "action": "UpdateMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceProfile": {
+        "PutPositionConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceProfile",
+            "action": "PutPositionConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateNetworkAnalyzerConfiguration": {
+        "UpdateEventConfigurationByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "UpdateNetworkAnalyzerConfiguration",
+            "action": "UpdateEventConfigurationByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartSingleWirelessDeviceImportTask": {
+        "DeregisterWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "StartSingleWirelessDeviceImportTask",
+            "action": "DeregisterWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGateway": {
+        "AssociateMulticastGroupWithFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGateway",
+            "action": "AssociateMulticastGroupWithFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDevice": {
+        "UpdateLogLevelsByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDevice",
+            "action": "UpdateLogLevelsByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFuotaTasks": {
+        "GetDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "ListFuotaTasks",
+            "action": "GetDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "TagResource": {
             "access_level": "Undocumented",
             "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMulticastGroup": {
+        "StartBulkDisassociateWirelessDeviceFromMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteMulticastGroup",
+            "action": "StartBulkDisassociateWirelessDeviceFromMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartFuotaTask": {
+        "SendDataToWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "StartFuotaTask",
+            "action": "SendDataToWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendDataToWirelessDevice": {
+        "DeleteWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "SendDataToWirelessDevice",
+            "action": "DeleteWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateNetworkAnalyzerConfiguration": {
+        "CreateWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "CreateNetworkAnalyzerConfiguration",
+            "action": "CreateWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceEventConfiguration": {
+        "StartNetworkAnalyzerStream": {
             "access_level": "Undocumented",
-            "action": "GetResourceEventConfiguration",
+            "action": "StartNetworkAnalyzerStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNetworkAnalyzerConfigurations": {
+        "UpdatePosition": {
             "access_level": "Undocumented",
-            "action": "ListNetworkAnalyzerConfigurations",
+            "action": "UpdatePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendDataToMulticastGroup": {
+        "AssociateWirelessGatewayWithThing": {
             "access_level": "Undocumented",
-            "action": "SendDataToMulticastGroup",
+            "action": "AssociateWirelessGatewayWithThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMulticastGroup": {
+        "DeleteMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "CreateMulticastGroup",
+            "action": "DeleteMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGatewayTask": {
+        "DisassociateWirelessDeviceFromMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGatewayTask",
+            "action": "DisassociateWirelessDeviceFromMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateLogLevelsByResourceTypes": {
+        "CancelMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "UpdateLogLevelsByResourceTypes",
+            "action": "CancelMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetNetworkAnalyzerConfiguration": {
+        "UpdateWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "GetNetworkAnalyzerConfiguration",
+            "action": "UpdateWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessDeviceImportTask": {
+        "CreateWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessDeviceImportTask",
+            "action": "CreateWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMulticastGroupWithFuotaTask": {
+        "ListMulticastGroups": {
             "access_level": "Undocumented",
-            "action": "AssociateMulticastGroupWithFuotaTask",
+            "action": "ListMulticastGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMulticastGroupsByFuotaTask": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListMulticastGroupsByFuotaTask",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessDevices": {
+        "AssociateAwsAccountWithPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "ListWirelessDevices",
+            "action": "AssociateAwsAccountWithPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGatewayTask": {
+        "DeleteServiceProfile": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGatewayTask",
+            "action": "DeleteServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDestinations": {
+        "GetWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "ListDestinations",
+            "action": "GetWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayTaskDefinition": {
+        "AssociateWirelessDeviceWithThing": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayTaskDefinition",
+            "action": "AssociateWirelessDeviceWithThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFuotaTask": {
+        "DisassociateWirelessGatewayFromThing": {
             "access_level": "Undocumented",
-            "action": "CreateFuotaTask",
+            "action": "DisassociateWirelessGatewayFromThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMulticastGroupSession": {
+        "CreateFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetMulticastGroupSession",
+            "action": "CreateFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetAllResourceLogLevels": {
+        "PutResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "ResetAllResourceLogLevels",
+            "action": "PutResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEventConfigurationByResourceTypes": {
+        "DeleteWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "GetEventConfigurationByResourceTypes",
+            "action": "DeleteWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessGateway": {
+        "GetMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessGateway",
+            "action": "GetMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessGateways": {
+        "ListWirelessDeviceImportTasks": {
             "access_level": "Undocumented",
-            "action": "ListWirelessGateways",
+            "action": "ListWirelessDeviceImportTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateAwsAccountFromPartnerAccount": {
+        "UpdateResourceEventConfiguration": {
             "access_level": "Undocumented",
-            "action": "DisassociateAwsAccountFromPartnerAccount",
+            "action": "UpdateResourceEventConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDestination": {
+        "GetServiceEndpoint": {
             "access_level": "Undocumented",
-            "action": "GetDestination",
+            "action": "GetServiceEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetResourceLogLevel": {
+        "UpdatePartnerAccount": {
             "access_level": "Undocumented",
-            "action": "ResetResourceLogLevel",
+            "action": "UpdatePartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartBulkDisassociateWirelessDeviceFromMulticastGroup": {
+        "ListWirelessDevices": {
             "access_level": "Undocumented",
-            "action": "StartBulkDisassociateWirelessDeviceFromMulticastGroup",
+            "action": "ListWirelessDevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPositionEstimate": {
+        "GetWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "GetPositionEstimate",
+            "action": "GetWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEventConfigurationByResourceTypes": {
+        "GetWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "UpdateEventConfigurationByResourceTypes",
+            "action": "GetWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TestWirelessDevice": {
+        "DeleteWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "TestWirelessDevice",
+            "action": "DeleteWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutResourceLogLevel": {
+        "StartSingleWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "PutResourceLogLevel",
+            "action": "StartSingleWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePartnerAccount": {
+        "ListDevicesForWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "UpdatePartnerAccount",
+            "action": "ListDevicesForWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "CreateWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "CreateWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessDevice": {
+        "GetServiceProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessDevice",
+            "action": "GetServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourceEventConfiguration": {
+        "StartBulkAssociateWirelessDeviceWithMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateResourceEventConfiguration",
+            "action": "StartBulkAssociateWirelessDeviceWithMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMulticastGroups": {
+        "CreateMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "ListMulticastGroups",
+            "action": "CreateMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGatewayTaskDefinition": {
+        "GetPosition": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGatewayTaskDefinition",
+            "action": "GetPosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayTask": {
+        "DeleteDestination": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayTask",
+            "action": "DeleteDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPartnerAccount": {
+        "UpdateNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetPartnerAccount",
+            "action": "UpdateNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteNetworkAnalyzerConfiguration": {
+        "StartMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "DeleteNetworkAnalyzerConfiguration",
+            "action": "StartMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMulticastGroup": {
+        "GetResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "UpdateMulticastGroup",
+            "action": "GetResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEventConfigurations": {
+        "ListDeviceProfiles": {
             "access_level": "Undocumented",
-            "action": "ListEventConfigurations",
+            "action": "ListDeviceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterWirelessDevice": {
+        "AssociateWirelessDeviceWithFuotaTask": {
             "access_level": "Undocumented",
-            "action": "DeregisterWirelessDevice",
+            "action": "AssociateWirelessDeviceWithFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeviceProfile": {
+        "GetResourceEventConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetDeviceProfile",
+            "action": "GetResourceEventConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayStatistics": {
+        "CreateServiceProfile": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayStatistics",
+            "action": "CreateServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPosition": {
+        "GetMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetPosition",
+            "action": "GetMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPositionConfiguration": {
+        "CreateDestination": {
             "access_level": "Undocumented",
-            "action": "GetPositionConfiguration",
+            "action": "CreateDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourcePosition": {
+        "CreateDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "GetResourcePosition",
+            "action": "CreateDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPositionConfigurations": {
+        "ListPartnerAccounts": {
             "access_level": "Undocumented",
-            "action": "ListPositionConfigurations",
+            "action": "ListPartnerAccounts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithThing": {
+        "UpdateResourcePosition": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithThing",
+            "action": "UpdateResourcePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFuotaTask": {
+        "CreateWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "DeleteFuotaTask",
+            "action": "CreateWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServiceProfiles": {
+        "DeleteWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "ListServiceProfiles",
+            "action": "DeleteWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartBulkAssociateWirelessDeviceWithMulticastGroup": {
+        "ResetAllResourceLogLevels": {
             "access_level": "Undocumented",
-            "action": "StartBulkAssociateWirelessDeviceWithMulticastGroup",
+            "action": "ResetAllResourceLogLevels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartMulticastGroupSession": {
+        "GetDestination": {
             "access_level": "Undocumented",
-            "action": "StartMulticastGroupSession",
+            "action": "GetDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFuotaTask": {
+        "AssociateWirelessGatewayWithCertificate": {
             "access_level": "Undocumented",
-            "action": "GetFuotaTask",
+            "action": "AssociateWirelessGatewayWithCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessGatewayWithThing": {
+        "DeleteQueuedMessages": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessGatewayWithThing",
+            "action": "DeleteQueuedMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateFuotaTask": {
+        "ListWirelessGateways": {
             "access_level": "Undocumented",
-            "action": "UpdateFuotaTask",
+            "action": "ListWirelessGateways",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessGatewayWithCertificate": {
+        "ListServiceProfiles": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessGatewayWithCertificate",
+            "action": "ListServiceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceProfiles": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListDeviceProfiles",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessDevice": {
+        "GetResourcePosition": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessDevice",
+            "action": "GetResourcePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessDevice": {
+        "GetWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessDevice",
+            "action": "GetWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMulticastGroupFromFuotaTask": {
+        "DeleteNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "DisassociateMulticastGroupFromFuotaTask",
+            "action": "DeleteNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelMulticastGroupSession": {
+        "GetWirelessGatewayFirmwareInformation": {
             "access_level": "Undocumented",
-            "action": "CancelMulticastGroupSession",
+            "action": "GetWirelessGatewayFirmwareInformation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessGatewayFromThing": {
+        "GetWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessGatewayFromThing",
+            "action": "GetWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayCertificate": {
+        "ResetResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayCertificate",
+            "action": "ResetResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceEndpoint": {
+        "UpdateFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetServiceEndpoint",
+            "action": "UpdateFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutPositionConfiguration": {
+        "ListFuotaTasks": {
             "access_level": "Undocumented",
-            "action": "PutPositionConfiguration",
+            "action": "ListFuotaTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGateway": {
+        "SendDataToMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGateway",
+            "action": "SendDataToMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessDeviceImportTasks": {
+        "UpdateWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "ListWirelessDeviceImportTasks",
+            "action": "UpdateWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartWirelessDeviceImportTask": {
+        "DeleteDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "StartWirelessDeviceImportTask",
+            "action": "DeleteDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDestination": {
+        "GetWirelessGatewayStatistics": {
             "access_level": "Undocumented",
-            "action": "CreateDestination",
+            "action": "GetWirelessGatewayStatistics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourcePosition": {
+        "DisassociateMulticastGroupFromFuotaTask": {
             "access_level": "Undocumented",
-            "action": "UpdateResourcePosition",
+            "action": "DisassociateMulticastGroupFromFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "iq": {
@@ -84452,315 +84452,315 @@
             "resources": [
                 "index",
                 "thesaurus"
             ]
         }
     },
     "kendra-ranking": {
-        "DeleteRescoreExecutionPlan": {
+        "CreateRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "DeleteRescoreExecutionPlan",
+            "action": "CreateRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeRescoreExecutionPlan": {
+        "UpdateRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "DescribeRescoreExecutionPlan",
+            "action": "UpdateRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRescoreExecutionPlans": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListRescoreExecutionPlans",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UntagResource": {
             "access_level": "Undocumented",
             "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Rescore": {
+        "ListRescoreExecutionPlans": {
             "access_level": "Undocumented",
-            "action": "Rescore",
+            "action": "ListRescoreExecutionPlans",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRescoreExecutionPlan": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "CreateRescoreExecutionPlan",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DescribeRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DescribeRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRescoreExecutionPlan": {
+        "Rescore": {
             "access_level": "Undocumented",
-            "action": "UpdateRescoreExecutionPlan",
+            "action": "Rescore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeleteRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeleteRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "kinesis": {
-        "CreateStream": {
+        "PutRecords": {
             "access_level": "Undocumented",
-            "action": "CreateStream",
+            "action": "PutRecords",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterStreamConsumer": {
+        "StopStreamEncryption": {
             "access_level": "Undocumented",
-            "action": "DeregisterStreamConsumer",
+            "action": "StopStreamEncryption",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterStreamConsumer": {
+        "SubscribeToShard": {
             "access_level": "Undocumented",
-            "action": "RegisterStreamConsumer",
+            "action": "SubscribeToShard",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRecords": {
+        "DescribeStream": {
             "access_level": "Undocumented",
-            "action": "PutRecords",
+            "action": "DescribeStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SplitShard": {
+        "StartStreamEncryption": {
             "access_level": "Undocumented",
-            "action": "SplitShard",
+            "action": "StartStreamEncryption",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisableEnhancedMonitoring": {
+        "SplitShard": {
             "access_level": "Undocumented",
-            "action": "DisableEnhancedMonitoring",
+            "action": "SplitShard",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListShards": {
+        "RegisterStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "ListShards",
+            "action": "RegisterStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForStream": {
+        "MergeShards": {
             "access_level": "Undocumented",
-            "action": "ListTagsForStream",
+            "action": "MergeShards",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopStreamEncryption": {
+        "DescribeLimits": {
             "access_level": "Undocumented",
-            "action": "StopStreamEncryption",
+            "action": "DescribeLimits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStreamConsumers": {
+        "ListStreams": {
             "access_level": "Undocumented",
-            "action": "ListStreamConsumers",
+            "action": "ListStreams",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetShardIterator": {
+        "UpdateStreamMode": {
             "access_level": "Undocumented",
-            "action": "GetShardIterator",
+            "action": "UpdateStreamMode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "MergeShards": {
+        "AddTagsToStream": {
             "access_level": "Undocumented",
-            "action": "MergeShards",
+            "action": "AddTagsToStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeLimits": {
+        "PutRecord": {
             "access_level": "Undocumented",
-            "action": "DescribeLimits",
+            "action": "PutRecord",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableEnhancedMonitoring": {
+        "DeregisterStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "EnableEnhancedMonitoring",
+            "action": "DeregisterStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddTagsToStream": {
+        "CreateStream": {
             "access_level": "Undocumented",
-            "action": "AddTagsToStream",
+            "action": "CreateStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRecord": {
+        "DescribeStreamSummary": {
             "access_level": "Undocumented",
-            "action": "PutRecord",
+            "action": "DescribeStreamSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveTagsFromStream": {
+        "ListStreamConsumers": {
             "access_level": "Undocumented",
-            "action": "RemoveTagsFromStream",
+            "action": "ListStreamConsumers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateStreamMode": {
+        "UpdateShardCount": {
             "access_level": "Undocumented",
-            "action": "UpdateStreamMode",
+            "action": "UpdateShardCount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStreamSummary": {
+        "DecreaseStreamRetentionPeriod": {
             "access_level": "Undocumented",
-            "action": "DescribeStreamSummary",
+            "action": "DecreaseStreamRetentionPeriod",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartStreamEncryption": {
+        "DeleteStream": {
             "access_level": "Undocumented",
-            "action": "StartStreamEncryption",
+            "action": "DeleteStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteStream": {
+        "GetRecords": {
             "access_level": "Undocumented",
-            "action": "DeleteStream",
+            "action": "GetRecords",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStreamConsumer": {
+        "EnableEnhancedMonitoring": {
             "access_level": "Undocumented",
-            "action": "DescribeStreamConsumer",
+            "action": "EnableEnhancedMonitoring",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "IncreaseStreamRetentionPeriod": {
+        "DescribeStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "IncreaseStreamRetentionPeriod",
+            "action": "DescribeStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateShardCount": {
+        "IncreaseStreamRetentionPeriod": {
             "access_level": "Undocumented",
-            "action": "UpdateShardCount",
+            "action": "IncreaseStreamRetentionPeriod",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStreams": {
+        "GetShardIterator": {
             "access_level": "Undocumented",
-            "action": "ListStreams",
+            "action": "GetShardIterator",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DecreaseStreamRetentionPeriod": {
+        "DisableEnhancedMonitoring": {
             "access_level": "Undocumented",
-            "action": "DecreaseStreamRetentionPeriod",
+            "action": "DisableEnhancedMonitoring",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SubscribeToShard": {
+        "ListShards": {
             "access_level": "Undocumented",
-            "action": "SubscribeToShard",
+            "action": "ListShards",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStream": {
+        "RemoveTagsFromStream": {
             "access_level": "Undocumented",
-            "action": "DescribeStream",
+            "action": "RemoveTagsFromStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRecords": {
+        "ListTagsForStream": {
             "access_level": "Undocumented",
-            "action": "GetRecords",
+            "action": "ListTagsForStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "kinesisanalytics": {
@@ -87328,169 +87328,169 @@
             "orphan": false,
             "resources": [
                 "function"
             ]
         }
     },
     "launchwizard": {
-        "ListWorkloadDeploymentOptions": {
+        "GetResourceCostEstimate": {
             "access_level": "Undocumented",
-            "action": "ListWorkloadDeploymentOptions",
+            "action": "GetResourceCostEstimate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSettingsSet": {
+        "ListProvisionedApps": {
             "access_level": "Undocumented",
-            "action": "UpdateSettingsSet",
+            "action": "ListProvisionedApps",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSettingsSet": {
+        "DescribeAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "CreateSettingsSet",
+            "action": "DescribeAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteApp": {
+        "UpdateSettingsSet": {
             "access_level": "Undocumented",
-            "action": "DeleteApp",
+            "action": "UpdateSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAdditionalNode": {
+        "DeleteApp": {
             "access_level": "Undocumented",
-            "action": "DeleteAdditionalNode",
+            "action": "DeleteApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceCostEstimate": {
+        "ListWorkloadDeploymentOptions": {
             "access_level": "Undocumented",
-            "action": "GetResourceCostEstimate",
+            "action": "ListWorkloadDeploymentOptions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeSettingsSet": {
+        "DescribeProvisioningEvents": {
             "access_level": "Undocumented",
-            "action": "DescribeSettingsSet",
+            "action": "DescribeProvisioningEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSettingsSets": {
+        "StartProvisioning": {
             "access_level": "Undocumented",
-            "action": "ListSettingsSets",
+            "action": "StartProvisioning",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkloads": {
+        "CreateAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "ListWorkloads",
+            "action": "CreateAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAdditionalNode": {
+        "GetWorkloadAssets": {
             "access_level": "Undocumented",
-            "action": "DescribeAdditionalNode",
+            "action": "GetWorkloadAssets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIpAddress": {
+        "ListWorkloads": {
             "access_level": "Undocumented",
-            "action": "GetIpAddress",
+            "action": "ListWorkloads",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAdditionalNodes": {
+        "DeleteAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "ListAdditionalNodes",
+            "action": "DeleteAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeProvisionedApp": {
+        "ListSettingsSets": {
             "access_level": "Undocumented",
-            "action": "DescribeProvisionedApp",
+            "action": "ListSettingsSets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartProvisioning": {
+        "CreateSettingsSet": {
             "access_level": "Undocumented",
-            "action": "StartProvisioning",
+            "action": "CreateSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProvisionedApps": {
+        "DescribeProvisionedApp": {
             "access_level": "Undocumented",
-            "action": "ListProvisionedApps",
+            "action": "DescribeProvisionedApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteSettingsSet": {
             "access_level": "Undocumented",
             "action": "DeleteSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorkloadAssets": {
+        "GetInfrastructureSuggestion": {
             "access_level": "Undocumented",
-            "action": "GetWorkloadAssets",
+            "action": "GetInfrastructureSuggestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAdditionalNode": {
+        "GetIpAddress": {
             "access_level": "Undocumented",
-            "action": "CreateAdditionalNode",
+            "action": "GetIpAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInfrastructureSuggestion": {
+        "DescribeSettingsSet": {
             "access_level": "Undocumented",
-            "action": "GetInfrastructureSuggestion",
+            "action": "DescribeSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeProvisioningEvents": {
+        "ListAdditionalNodes": {
             "access_level": "Undocumented",
-            "action": "DescribeProvisioningEvents",
+            "action": "ListAdditionalNodes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "lex": {
@@ -95956,225 +95956,225 @@
             "orphan": false,
             "resources": [
                 "packaging-groups"
             ]
         }
     },
     "mediapackagev2": {
-        "DeleteChannelGroup": {
+        "GetHeadObject": {
             "access_level": "Undocumented",
-            "action": "DeleteChannelGroup",
+            "action": "GetHeadObject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateOriginEndpoint": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateOriginEndpoint",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChannelGroup": {
+        "GetObject": {
             "access_level": "Undocumented",
-            "action": "GetChannelGroup",
+            "action": "GetObject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetHeadObject": {
+        "UpdateChannelGroup": {
             "access_level": "Undocumented",
-            "action": "GetHeadObject",
+            "action": "UpdateChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeleteOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetObject": {
+        "DeleteChannelPolicy": {
             "access_level": "Undocumented",
-            "action": "GetObject",
+            "action": "DeleteChannelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteOriginEndpointPolicy": {
             "access_level": "Undocumented",
             "action": "DeleteOriginEndpointPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOriginEndpointPolicy": {
+        "ListChannelGroups": {
             "access_level": "Undocumented",
-            "action": "GetOriginEndpointPolicy",
+            "action": "ListChannelGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChannelPolicy": {
+        "GetOriginEndpointPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteChannelPolicy",
+            "action": "GetOriginEndpointPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutObject": {
+        "CreateChannelGroup": {
             "access_level": "Undocumented",
-            "action": "PutObject",
+            "action": "CreateChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChannelPolicy": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetChannelPolicy",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreateChannel": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOriginEndpoint": {
+        "GetChannel": {
             "access_level": "Undocumented",
-            "action": "GetOriginEndpoint",
+            "action": "GetChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateChannelGroup": {
+        "PutObject": {
             "access_level": "Undocumented",
-            "action": "CreateChannelGroup",
+            "action": "PutObject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOriginEndpoints": {
+        "GetChannelGroup": {
             "access_level": "Undocumented",
-            "action": "ListOriginEndpoints",
+            "action": "GetChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateOriginEndpoint": {
             "access_level": "Undocumented",
             "action": "CreateOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListChannels": {
+        "UpdateChannel": {
             "access_level": "Undocumented",
-            "action": "ListChannels",
+            "action": "UpdateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChannel": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetChannel",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateChannel": {
+        "UpdateOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "CreateChannel",
+            "action": "UpdateOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateChannel": {
+        "DeleteChannelGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateChannel",
+            "action": "DeleteChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "PutChannelPolicy": {
             "access_level": "Undocumented",
             "action": "PutChannelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteOriginEndpoint": {
+        "DeleteChannel": {
             "access_level": "Undocumented",
-            "action": "DeleteOriginEndpoint",
+            "action": "DeleteChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListChannelGroups": {
+        "ListOriginEndpoints": {
             "access_level": "Undocumented",
-            "action": "ListChannelGroups",
+            "action": "ListOriginEndpoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateChannelGroup": {
+        "GetChannelPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateChannelGroup",
+            "action": "GetChannelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "PutOriginEndpointPolicy": {
             "access_level": "Undocumented",
             "action": "PutOriginEndpointPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChannel": {
+        "ListChannels": {
             "access_level": "Undocumented",
-            "action": "DeleteChannel",
+            "action": "ListChannels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "mediastore": {
@@ -103216,251 +103216,251 @@
             "orphan": false,
             "resources": [
                 "studio-component"
             ]
         }
     },
     "notifications": {
-        "DisassociateChannel": {
+        "CreateNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "DisassociateChannel",
+            "action": "CreateNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetNotificationConfiguration": {
+        "UpdateNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetNotificationConfiguration",
+            "action": "UpdateNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEventRule": {
+        "GetNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetEventRule",
+            "action": "GetNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "CreateEventRule": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "CreateEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterNotificationHub": {
+        "DisassociateChannel": {
             "access_level": "Undocumented",
-            "action": "DeregisterNotificationHub",
+            "action": "DisassociateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEventRule": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateEventRule",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateChannel": {
+        "ListEventRules": {
             "access_level": "Undocumented",
-            "action": "AssociateChannel",
+            "action": "ListEventRules",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEventRule": {
+        "GetNotificationEvent": {
             "access_level": "Undocumented",
-            "action": "DeleteEventRule",
+            "action": "GetNotificationEvent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeleteEventRule": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeleteEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateNotificationConfiguration": {
+        "DeregisterNotificationHub": {
             "access_level": "Undocumented",
-            "action": "UpdateNotificationConfiguration",
+            "action": "DeregisterNotificationHub",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetNotificationEvent": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetNotificationEvent",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotificationHubs": {
+        "RegisterNotificationHub": {
             "access_level": "Undocumented",
-            "action": "ListNotificationHubs",
+            "action": "RegisterNotificationHub",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterNotificationHub": {
+        "AssociateChannel": {
             "access_level": "Undocumented",
-            "action": "RegisterNotificationHub",
+            "action": "AssociateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListChannels": {
+        "ListNotificationHubs": {
             "access_level": "Undocumented",
-            "action": "ListChannels",
+            "action": "ListNotificationHubs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEventRule": {
+        "UpdateEventRule": {
             "access_level": "Undocumented",
-            "action": "CreateEventRule",
+            "action": "UpdateEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListNotificationEvents": {
             "access_level": "Undocumented",
             "action": "ListNotificationEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateNotificationConfiguration": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreateNotificationConfiguration",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEventRules": {
+        "DeleteNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListEventRules",
+            "action": "DeleteNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetEventRule": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteNotificationConfiguration": {
+        "ListNotificationConfigurations": {
             "access_level": "Undocumented",
-            "action": "DeleteNotificationConfiguration",
+            "action": "ListNotificationConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotificationConfigurations": {
+        "ListChannels": {
             "access_level": "Undocumented",
-            "action": "ListNotificationConfigurations",
+            "action": "ListChannels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "notifications-contacts": {
-        "UntagResource": {
+        "GetEmailContact": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEmailContact": {
+        "SendActivationCode": {
             "access_level": "Undocumented",
-            "action": "GetEmailContact",
+            "action": "SendActivationCode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEmailContact": {
+        "ActivateEmailContact": {
             "access_level": "Undocumented",
-            "action": "CreateEmailContact",
+            "action": "ActivateEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendActivationCode": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "SendActivationCode",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeleteEmailContact": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeleteEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEmailContacts": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListEmailContacts",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreateEmailContact": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreateEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEmailContact": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteEmailContact",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ActivateEmailContact": {
+        "ListEmailContacts": {
             "access_level": "Undocumented",
-            "action": "ActivateEmailContact",
+            "action": "ListEmailContacts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "oam": {
@@ -105833,129 +105833,129 @@
             "orphan": false,
             "resources": [
                 "policy"
             ]
         }
     },
     "osis": {
-        "TagResource": {
+        "GetPipelineChangeProgress": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetPipelineChangeProgress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPipelineChangeProgress": {
+        "ListPipelines": {
             "access_level": "Undocumented",
-            "action": "GetPipelineChangeProgress",
+            "action": "ListPipelines",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePipeline": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DeletePipeline",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPipelineBlueprints": {
+        "UpdatePipeline": {
             "access_level": "Undocumented",
-            "action": "ListPipelineBlueprints",
+            "action": "UpdatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Ingest": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "Ingest",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetPipeline": {
             "access_level": "Undocumented",
             "action": "GetPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartPipeline": {
+        "CreatePipeline": {
             "access_level": "Undocumented",
-            "action": "StartPipeline",
+            "action": "CreatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "Ingest": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "Ingest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePipeline": {
+        "StopPipeline": {
             "access_level": "Undocumented",
-            "action": "CreatePipeline",
+            "action": "StopPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidatePipeline": {
+        "ListPipelineBlueprints": {
             "access_level": "Undocumented",
-            "action": "ValidatePipeline",
+            "action": "ListPipelineBlueprints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeletePipeline": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeletePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopPipeline": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "StopPipeline",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPipelines": {
+        "StartPipeline": {
             "access_level": "Undocumented",
-            "action": "ListPipelines",
+            "action": "StartPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPipelineBlueprint": {
+        "ValidatePipeline": {
             "access_level": "Undocumented",
-            "action": "GetPipelineBlueprint",
+            "action": "ValidatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePipeline": {
+        "GetPipelineBlueprint": {
             "access_level": "Undocumented",
-            "action": "UpdatePipeline",
+            "action": "GetPipelineBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "outposts": {
@@ -106570,249 +106570,249 @@
             "orphan": false,
             "resources": [
                 "device"
             ]
         }
     },
     "payment-cryptography": {
-        "GetPublicKeyCertificate": {
+        "GenerateCardValidationData": {
             "access_level": "Undocumented",
-            "action": "GetPublicKeyCertificate",
+            "action": "GenerateCardValidationData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "CreateKey": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "CreateKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopKeyUsage": {
+        "VerifyAuthRequestCryptogram": {
             "access_level": "Undocumented",
-            "action": "StopKeyUsage",
+            "action": "VerifyAuthRequestCryptogram",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartKeyUsage": {
+        "ImportKey": {
             "access_level": "Undocumented",
-            "action": "StartKeyUsage",
+            "action": "ImportKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAlias": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "CreateAlias",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAlias": {
+        "DecryptData": {
             "access_level": "Undocumented",
-            "action": "UpdateAlias",
+            "action": "DecryptData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetParametersForExport": {
+        "VerifyCardValidationData": {
             "access_level": "Undocumented",
-            "action": "GetParametersForExport",
+            "action": "VerifyCardValidationData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TranslatePinData": {
+        "GenerateMac": {
             "access_level": "Undocumented",
-            "action": "TranslatePinData",
+            "action": "GenerateMac",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EncryptData": {
+        "ExportKey": {
             "access_level": "Undocumented",
-            "action": "EncryptData",
+            "action": "ExportKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyCardValidationData": {
+        "GetKey": {
             "access_level": "Undocumented",
-            "action": "VerifyCardValidationData",
+            "action": "GetKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateKey": {
+        "StartKeyUsage": {
             "access_level": "Undocumented",
-            "action": "CreateKey",
+            "action": "StartKeyUsage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReEncryptData": {
+        "VerifyMac": {
             "access_level": "Undocumented",
-            "action": "ReEncryptData",
+            "action": "VerifyMac",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ImportKey": {
+        "GetParametersForExport": {
             "access_level": "Undocumented",
-            "action": "ImportKey",
+            "action": "GetParametersForExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateCardValidationData": {
+        "GetParametersForImport": {
             "access_level": "Undocumented",
-            "action": "GenerateCardValidationData",
+            "action": "GetParametersForImport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteKey": {
+        "RestoreKey": {
             "access_level": "Undocumented",
-            "action": "DeleteKey",
+            "action": "RestoreKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GeneratePinData": {
+        "ListKeys": {
             "access_level": "Undocumented",
-            "action": "GeneratePinData",
+            "action": "ListKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateMac": {
+        "VerifyPinData": {
             "access_level": "Undocumented",
-            "action": "GenerateMac",
+            "action": "VerifyPinData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyPinData": {
+        "GetPublicKeyCertificate": {
             "access_level": "Undocumented",
-            "action": "VerifyPinData",
+            "action": "GetPublicKeyCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAlias": {
+        "StopKeyUsage": {
             "access_level": "Undocumented",
-            "action": "GetAlias",
+            "action": "StopKeyUsage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ExportKey": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ExportKey",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DecryptData": {
+        "GeneratePinData": {
             "access_level": "Undocumented",
-            "action": "DecryptData",
+            "action": "GeneratePinData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyAuthRequestCryptogram": {
+        "TranslatePinData": {
             "access_level": "Undocumented",
-            "action": "VerifyAuthRequestCryptogram",
+            "action": "TranslatePinData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetParametersForImport": {
+        "UpdateAlias": {
             "access_level": "Undocumented",
-            "action": "GetParametersForImport",
+            "action": "UpdateAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ReEncryptData": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ReEncryptData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyMac": {
+        "ListAliases": {
             "access_level": "Undocumented",
-            "action": "VerifyMac",
+            "action": "ListAliases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListKeys": {
+        "EncryptData": {
             "access_level": "Undocumented",
-            "action": "ListKeys",
+            "action": "EncryptData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetKey": {
+        "CreateAlias": {
             "access_level": "Undocumented",
-            "action": "GetKey",
+            "action": "CreateAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAliases": {
+        "DeleteKey": {
             "access_level": "Undocumented",
-            "action": "ListAliases",
+            "action": "DeleteKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RestoreKey": {
+        "GetAlias": {
             "access_level": "Undocumented",
-            "action": "RestoreKey",
+            "action": "GetAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteAlias": {
             "access_level": "Undocumented",
@@ -106820,49 +106820,49 @@
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "payments": {
-        "GetPaymentInstrument": {
+        "DeletePaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "GetPaymentInstrument",
+            "action": "DeletePaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePaymentInstrument": {
+        "ListPaymentPreferences": {
             "access_level": "Undocumented",
-            "action": "CreatePaymentInstrument",
+            "action": "ListPaymentPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPaymentPreferences": {
+        "CreatePaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "ListPaymentPreferences",
+            "action": "CreatePaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetPaymentStatus": {
             "access_level": "Undocumented",
             "action": "GetPaymentStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePaymentInstrument": {
+        "GetPaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "DeletePaymentInstrument",
+            "action": "GetPaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "MakePayment": {
             "access_level": "Undocumented",
@@ -112241,281 +112241,281 @@
             "orphan": false,
             "resources": [
                 "vpcconnection"
             ]
         }
     },
     "ram": {
-        "DisassociateResourceShare": {
+        "GetResourcePolicies": {
             "access_level": "Undocumented",
-            "action": "DisassociateResourceShare",
+            "action": "GetResourcePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePermissionVersion": {
+        "CreatePermissionVersion": {
             "access_level": "Undocumented",
-            "action": "DeletePermissionVersion",
+            "action": "CreatePermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissionVersions": {
+        "RejectResourceShareInvitation": {
             "access_level": "Undocumented",
-            "action": "ListPermissionVersions",
+            "action": "RejectResourceShareInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DisassociateResourceSharePermission": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DisassociateResourceSharePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourcePolicies": {
+        "DeleteResourceShare": {
             "access_level": "Undocumented",
-            "action": "GetResourcePolicies",
+            "action": "DeleteResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResources": {
+        "DeletePermissionVersion": {
             "access_level": "Undocumented",
-            "action": "ListResources",
+            "action": "DeletePermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateResourceShare": {
+        "GetResourceShareInvitations": {
             "access_level": "Undocumented",
-            "action": "CreateResourceShare",
+            "action": "GetResourceShareInvitations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "PromoteResourceShareCreatedFromPolicy": {
             "access_level": "Undocumented",
             "action": "PromoteResourceShareCreatedFromPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateResourceSharePermission": {
+        "ListPendingInvitationResources": {
             "access_level": "Undocumented",
-            "action": "AssociateResourceSharePermission",
+            "action": "ListPendingInvitationResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PromotePermissionCreatedFromPolicy": {
+        "ListReplacePermissionAssociationsWork": {
             "access_level": "Undocumented",
-            "action": "PromotePermissionCreatedFromPolicy",
+            "action": "ListReplacePermissionAssociationsWork",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RejectResourceShareInvitation": {
+        "ListResourceTypes": {
             "access_level": "Undocumented",
-            "action": "RejectResourceShareInvitation",
+            "action": "ListResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShareAssociations": {
+        "AcceptResourceShareInvitation": {
             "access_level": "Undocumented",
-            "action": "GetResourceShareAssociations",
+            "action": "AcceptResourceShareInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetDefaultPermissionVersion": {
+        "ListResources": {
             "access_level": "Undocumented",
-            "action": "SetDefaultPermissionVersion",
+            "action": "ListResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateResourceSharePermission": {
+        "DeletePermission": {
             "access_level": "Undocumented",
-            "action": "DisassociateResourceSharePermission",
+            "action": "DeletePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShares": {
+        "AssociateResourceShare": {
             "access_level": "Undocumented",
-            "action": "GetResourceShares",
+            "action": "AssociateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissions": {
+        "ListPermissionVersions": {
             "access_level": "Undocumented",
-            "action": "ListPermissions",
+            "action": "ListPermissionVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReplacePermissionAssociationsWork": {
+        "ListPermissions": {
             "access_level": "Undocumented",
-            "action": "ListReplacePermissionAssociationsWork",
+            "action": "ListPermissions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AcceptResourceShareInvitation": {
+        "PromotePermissionCreatedFromPolicy": {
             "access_level": "Undocumented",
-            "action": "AcceptResourceShareInvitation",
+            "action": "PromotePermissionCreatedFromPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPendingInvitationResources": {
+        "DisassociateResourceShare": {
             "access_level": "Undocumented",
-            "action": "ListPendingInvitationResources",
+            "action": "DisassociateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePermission": {
+        "ReplacePermissionAssociations": {
             "access_level": "Undocumented",
-            "action": "DeletePermission",
+            "action": "ReplacePermissionAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePermissionVersion": {
+        "ListPermissionAssociations": {
             "access_level": "Undocumented",
-            "action": "CreatePermissionVersion",
+            "action": "ListPermissionAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateResourceShare": {
+        "GetResourceShareAssociations": {
             "access_level": "Undocumented",
-            "action": "AssociateResourceShare",
+            "action": "GetResourceShareAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteResourceShare": {
+        "GetPermission": {
             "access_level": "Undocumented",
-            "action": "DeleteResourceShare",
+            "action": "GetPermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePermission": {
+        "AssociateResourceSharePermission": {
             "access_level": "Undocumented",
-            "action": "CreatePermission",
+            "action": "AssociateResourceSharePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourceShare": {
+        "EnableSharingWithAwsOrganization": {
             "access_level": "Undocumented",
-            "action": "UpdateResourceShare",
+            "action": "EnableSharingWithAwsOrganization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPrincipals": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListPrincipals",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "UpdateResourceShare": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "UpdateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissionAssociations": {
+        "SetDefaultPermissionVersion": {
             "access_level": "Undocumented",
-            "action": "ListPermissionAssociations",
+            "action": "SetDefaultPermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShareInvitations": {
+        "CreatePermission": {
             "access_level": "Undocumented",
-            "action": "GetResourceShareInvitations",
+            "action": "CreatePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListResourceSharePermissions": {
             "access_level": "Undocumented",
             "action": "ListResourceSharePermissions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableSharingWithAwsOrganization": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "EnableSharingWithAwsOrganization",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPermission": {
+        "CreateResourceShare": {
             "access_level": "Undocumented",
-            "action": "GetPermission",
+            "action": "CreateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReplacePermissionAssociations": {
+        "GetResourceShares": {
             "access_level": "Undocumented",
-            "action": "ReplacePermissionAssociations",
+            "action": "GetResourceShares",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResourceTypes": {
+        "ListPrincipals": {
             "access_level": "Undocumented",
-            "action": "ListResourceTypes",
+            "action": "ListPrincipals",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "rbin": {
@@ -130054,113 +130054,113 @@
             "orphan": false,
             "resources": [
                 "schema"
             ]
         }
     },
     "scn": {
-        "DescribeInstance": {
+        "DeleteInstance": {
             "access_level": "Undocumented",
-            "action": "DescribeInstance",
+            "action": "DeleteInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSSOApplication": {
+        "CreateSSOApplication": {
             "access_level": "Undocumented",
-            "action": "DeleteSSOApplication",
+            "action": "CreateSSOApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteInstance": {
+        "ListAdminUsers": {
             "access_level": "Undocumented",
-            "action": "DeleteInstance",
+            "action": "ListAdminUsers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstances": {
+        "DescribeInstance": {
             "access_level": "Undocumented",
-            "action": "ListInstances",
+            "action": "DescribeInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateInstance": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreateInstance",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAdminUsers": {
+        "AssignAdminPermissionsToUser": {
             "access_level": "Undocumented",
-            "action": "ListAdminUsers",
+            "action": "AssignAdminPermissionsToUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateInstance": {
+        "DeleteSSOApplication": {
             "access_level": "Undocumented",
-            "action": "UpdateInstance",
+            "action": "DeleteSSOApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssignAdminPermissionsToUser": {
+        "ListInstances": {
             "access_level": "Undocumented",
-            "action": "AssignAdminPermissionsToUser",
+            "action": "ListInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListTagsForResource": {
             "access_level": "Undocumented",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSSOApplication": {
+        "RemoveAdminPermissionsForUser": {
             "access_level": "Undocumented",
-            "action": "CreateSSOApplication",
+            "action": "RemoveAdminPermissionsForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreateInstance": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreateInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveAdminPermissionsForUser": {
+        "UpdateInstance": {
             "access_level": "Undocumented",
-            "action": "RemoveAdminPermissionsForUser",
+            "action": "UpdateInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "sdb": {
@@ -145062,265 +145062,265 @@
             "access_level": "Undocumented",
             "action": "TerminateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolNetworkInstance": {
+        "PutSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "DeleteSolNetworkInstance",
+            "action": "PutSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolNetworkInstance": {
+        "ValidateSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "CreateSolNetworkInstance",
+            "action": "ValidateSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetSolFunctionInstance": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetSolFunctionInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolNetworkPackage": {
+        "ListSolNetworkInstances": {
             "access_level": "Undocumented",
-            "action": "CreateSolNetworkPackage",
+            "action": "ListSolNetworkInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolFunctionPackages": {
+        "GetSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "ListSolFunctionPackages",
+            "action": "GetSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackageDescriptor": {
+        "CreateSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackageDescriptor",
+            "action": "CreateSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolNetworkPackage": {
+        "GetSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "DeleteSolNetworkPackage",
+            "action": "GetSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackageContent": {
+        "GetSolFunctionPackageDescriptor": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackageContent",
+            "action": "GetSolFunctionPackageDescriptor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackageContent": {
+        "ListSolNetworkPackages": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackageContent",
+            "action": "ListSolNetworkPackages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkOperations": {
+        "DeleteSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkOperations",
+            "action": "DeleteSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackage": {
+        "ListSolFunctionInstances": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackage",
+            "action": "ListSolFunctionInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ValidateSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ValidateSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkOperation": {
+        "GetSolNetworkPackageDescriptor": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkOperation",
+            "action": "GetSolNetworkPackageDescriptor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSolNetworkPackage": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateSolNetworkPackage",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkPackages": {
+        "GetSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkPackages",
+            "action": "GetSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolFunctionPackage": {
+        "GetSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "DeleteSolFunctionPackage",
+            "action": "GetSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSolFunctionPackageContent": {
+        "GetSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "PutSolFunctionPackageContent",
+            "action": "GetSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSolFunctionPackage": {
+        "PutSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "UpdateSolFunctionPackage",
+            "action": "PutSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolFunctionPackage": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "CreateSolFunctionPackage",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CancelSolNetworkOperation": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CancelSolNetworkOperation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSolNetworkInstance": {
+        "DeleteSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "UpdateSolNetworkInstance",
+            "action": "DeleteSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackageDescriptor": {
+        "UpdateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackageDescriptor",
+            "action": "UpdateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InstantiateSolNetworkInstance": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "InstantiateSolNetworkInstance",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelSolNetworkOperation": {
+        "DeleteSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "CancelSolNetworkOperation",
+            "action": "DeleteSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkInstance": {
+        "ListSolFunctionPackages": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkInstance",
+            "action": "ListSolFunctionPackages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolFunctionInstances": {
+        "CreateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "ListSolFunctionInstances",
+            "action": "CreateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSolNetworkPackageContent": {
+        "InstantiateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "PutSolNetworkPackageContent",
+            "action": "InstantiateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionInstance": {
+        "GetSolNetworkOperation": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionInstance",
+            "action": "GetSolNetworkOperation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkInstances": {
+        "ListSolNetworkOperations": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkInstances",
+            "action": "ListSolNetworkOperations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidateSolFunctionPackageContent": {
+        "UpdateSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "ValidateSolFunctionPackageContent",
+            "action": "UpdateSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidateSolNetworkPackageContent": {
+        "CreateSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "ValidateSolNetworkPackageContent",
+            "action": "CreateSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackage": {
+        "UpdateSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackage",
+            "action": "UpdateSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "transcribe": {
@@ -147171,185 +147171,185 @@
             "access_level": "Undocumented",
             "action": "GetPolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIdentitySource": {
+        "IsAuthorized": {
             "access_level": "Undocumented",
-            "action": "GetIdentitySource",
+            "action": "IsAuthorized",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSchema": {
+        "ListPolicyStores": {
             "access_level": "Undocumented",
-            "action": "PutSchema",
+            "action": "ListPolicyStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyTemplate": {
+        "UpdatePolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyTemplate",
+            "action": "UpdatePolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyStore": {
+        "UpdatePolicyStore": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyStore",
+            "action": "UpdatePolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyTemplates": {
+        "UpdatePolicy": {
             "access_level": "Undocumented",
-            "action": "ListPolicyTemplates",
+            "action": "UpdatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIdentitySource": {
+        "GetIdentitySource": {
             "access_level": "Undocumented",
-            "action": "CreateIdentitySource",
+            "action": "GetIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicyStore": {
+        "DeletePolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "CreatePolicyStore",
+            "action": "DeletePolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetPolicy": {
             "access_level": "Undocumented",
             "action": "GetPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicyTemplate": {
+        "CreateIdentitySource": {
             "access_level": "Undocumented",
-            "action": "CreatePolicyTemplate",
+            "action": "CreateIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicy": {
+        "CreatePolicyStore": {
             "access_level": "Undocumented",
-            "action": "CreatePolicy",
+            "action": "CreatePolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicy": {
+        "CreatePolicy": {
             "access_level": "Undocumented",
-            "action": "DeletePolicy",
+            "action": "CreatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "IsAuthorizedWithToken": {
+        "DeletePolicyStore": {
             "access_level": "Undocumented",
-            "action": "IsAuthorizedWithToken",
+            "action": "DeletePolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePolicy": {
+        "IsAuthorizedWithToken": {
             "access_level": "Undocumented",
-            "action": "UpdatePolicy",
+            "action": "IsAuthorizedWithToken",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "IsAuthorized": {
+        "CreatePolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "IsAuthorized",
+            "action": "CreatePolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePolicyTemplate": {
+        "ListIdentitySources": {
             "access_level": "Undocumented",
-            "action": "UpdatePolicyTemplate",
+            "action": "ListIdentitySources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIdentitySources": {
+        "PutSchema": {
             "access_level": "Undocumented",
-            "action": "ListIdentitySources",
+            "action": "PutSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePolicyStore": {
+        "UpdateIdentitySource": {
             "access_level": "Undocumented",
-            "action": "UpdatePolicyStore",
+            "action": "UpdateIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchema": {
+        "GetPolicyStore": {
             "access_level": "Undocumented",
-            "action": "GetSchema",
+            "action": "GetPolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyStores": {
+        "DeleteIdentitySource": {
             "access_level": "Undocumented",
-            "action": "ListPolicyStores",
+            "action": "DeleteIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIdentitySource": {
+        "GetSchema": {
             "access_level": "Undocumented",
-            "action": "DeleteIdentitySource",
+            "action": "GetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicyStore": {
+        "DeletePolicy": {
             "access_level": "Undocumented",
-            "action": "GetPolicyStore",
+            "action": "DeletePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIdentitySource": {
+        "ListPolicyTemplates": {
             "access_level": "Undocumented",
-            "action": "UpdateIdentitySource",
+            "action": "ListPolicyTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "voiceid": {
```

### Comparing `iam_actions-1.2.20230617/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230618/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230617/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230618/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230617/iam_actions/generate/generate.py` & `iam_actions-1.2.20230618/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230617/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230618/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230617/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230618/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230617/iam_actions/generate/services.py` & `iam_actions-1.2.20230618/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230617/iam_actions/policies.json` & `iam_actions-1.2.20230618/iam_actions/policies.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230617/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230618/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230617/iam_actions/services.json` & `iam_actions-1.2.20230618/iam_actions/services.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230617/pyproject.toml` & `iam_actions-1.2.20230618/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230617"
+version = "1.2.20230618"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230617/setup.py` & `iam_actions-1.2.20230618/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230617',
+    'version': '1.2.20230618',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230617/PKG-INFO` & `iam_actions-1.2.20230618/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230617
+Version: 1.2.20230618
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

