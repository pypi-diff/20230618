# Comparing `tmp/odoo_addons_oca_server_backend-16.0.20230411.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_server_backend-16.0.20230617.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1443 bytes, number of entries: 4
--rw-r--r--  2.0 unx      671 b- defN 23-Apr-12 07:49 odoo_addons_oca_server_backend-16.0.20230411.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 07:49 odoo_addons_oca_server_backend-16.0.20230411.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-12 07:49 odoo_addons_oca_server_backend-16.0.20230411.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      428 b- defN 23-Apr-12 07:49 odoo_addons_oca_server_backend-16.0.20230411.0.dist-info/RECORD
-4 files, 1192 bytes uncompressed, 597 bytes compressed:  49.9%
+Zip file size: 1454 bytes, number of entries: 4
+-rw-r--r--  2.0 unx      736 b- defN 23-Jun-18 05:03 odoo_addons_oca_server_backend-16.0.20230617.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-18 05:03 odoo_addons_oca_server_backend-16.0.20230617.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-18 05:03 odoo_addons_oca_server_backend-16.0.20230617.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      428 b- defN 23-Jun-18 05:03 odoo_addons_oca_server_backend-16.0.20230617.0.dist-info/RECORD
+4 files, 1257 bytes uncompressed, 608 bytes compressed:  51.6%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_server_backend-16.0.20230411.0.dist-info/METADATA
+Filename: odoo_addons_oca_server_backend-16.0.20230617.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_server_backend-16.0.20230411.0.dist-info/WHEEL
+Filename: odoo_addons_oca_server_backend-16.0.20230617.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_server_backend-16.0.20230411.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_server_backend-16.0.20230617.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_server_backend-16.0.20230411.0.dist-info/RECORD
+Filename: odoo_addons_oca_server_backend-16.0.20230617.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_server_backend-16.0.20230411.0.dist-info/METADATA` & `odoo_addons_oca_server_backend-16.0.20230617.0.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-server-backend
-Version: 16.0.20230411.0
+Version: 16.0.20230617.0
 Summary: Meta package for oca-server-backend Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
 Requires-Dist: odoo-addon-base-external-dbsource (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-base-external-dbsource-mssql (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-base-external-dbsource-sqlite (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-base-import-match (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-base-user-role (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-base-user-role-history (<16.1dev,>=16.0dev)
 
 UNKNOWN
```

