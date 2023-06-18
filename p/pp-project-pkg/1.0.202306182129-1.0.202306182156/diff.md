# Comparing `tmp/pp_project_pkg-1.0.202306182129-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202306182156-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 8590 bytes, number of entries: 13
+Zip file size: 8641 bytes, number of entries: 13
 -rw-rw-r--  2.0 unx       71 b- defN 23-Jun-07 11:24 pp_project_pkg/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-18 21:29 pp_project_pkg/linear_train.py
 -rw-rw-r--  2.0 unx      577 b- defN 23-Jun-07 11:24 pp_project_pkg/newsvendor.py
 -rw-rw-r--  2.0 unx     7115 b- defN 23-Jun-07 11:24 pp_project_pkg/pp_tables.py
 -rw-rw-r--  2.0 unx     4190 b- defN 23-Jun-18 21:13 pp_project_pkg/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jun-18 21:29 pp_project_pkg/version.py
--rw-rw-r--  2.0 unx     4391 b- defN 23-Jun-16 01:49 pp_project_pkg/wrangling.py
--rwxrwxr-x  2.0 unx       65 b- defN 23-Jun-02 12:43 pp_project_pkg-1.0.202306182129.data/scripts/get_tables.py
--rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-07 11:24 pp_project_pkg-1.0.202306182129.data/scripts/pp_project_run.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jun-18 21:29 pp_project_pkg-1.0.202306182129.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-18 21:29 pp_project_pkg-1.0.202306182129.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-18 21:29 pp_project_pkg-1.0.202306182129.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1179 b- defN 23-Jun-18 21:29 pp_project_pkg-1.0.202306182129.dist-info/RECORD
-13 files, 19598 bytes uncompressed, 6568 bytes compressed:  66.5%
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jun-18 21:56 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx     4595 b- defN 23-Jun-18 21:56 pp_project_pkg/wrangling.py
+-rwxrwxr-x  2.0 unx       65 b- defN 23-Jun-02 12:43 pp_project_pkg-1.0.202306182156.data/scripts/get_tables.py
+-rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-07 11:24 pp_project_pkg-1.0.202306182156.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jun-18 21:56 pp_project_pkg-1.0.202306182156.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-18 21:56 pp_project_pkg-1.0.202306182156.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Jun-18 21:56 pp_project_pkg-1.0.202306182156.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1179 b- defN 23-Jun-18 21:56 pp_project_pkg-1.0.202306182156.dist-info/RECORD
+13 files, 19802 bytes uncompressed, 6619 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306182129.data/scripts/get_tables.py
+Filename: pp_project_pkg-1.0.202306182156.data/scripts/get_tables.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306182129.data/scripts/pp_project_run.py
+Filename: pp_project_pkg-1.0.202306182156.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306182129.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202306182156.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306182129.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202306182156.dist-info/WHEEL
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306182129.dist-info/top_level.txt
+Filename: pp_project_pkg-1.0.202306182156.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306182129.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202306182156.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pp_project_pkg/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('06')
 VERSION_DAY = int('18')
 VERSION_HOUR = int('21')
-VERSION_MINUTE = int('29')
+VERSION_MINUTE = int('56')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202306182129
-version_date = '2023/06/18 21:29'
+PATCH_VERSION = 202306182156
+version_date = '2023/06/18 21:56'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## pp_project_pkg/wrangling.py

```diff
@@ -79,9 +79,14 @@
     meal_service_summary_df['covers'] = cover_count
     meal_service_summary_df['actual_consumption'] = meal_service_summary_df['actual_production'] - meal_service_summary_df['rework_or_reuse'] - meal_service_summary_df['waste']
     meal_service_summary_df['consumption_per_cover'] = meal_service_summary_df['actual_consumption'] / cover_count
     meal_service_summary_df['scaling_factor'] = meal_service_summary_df['actual_consumption'] / (cover_count * 1000)
 
     # Select all columns from the resulting dataframe
     result_df = meal_service_summary_df.loc[:, :]
+    result_df['date'] = site_data['date']
 
+    if logger:
+        logger.info("Added date column to the result_df")
+        logger.info("result_df : {}".format(result_df.head(2)))
+                        
     return result_df
```

## Comparing `pp_project_pkg-1.0.202306182129.data/scripts/pp_project_run.py` & `pp_project_pkg-1.0.202306182156.data/scripts/pp_project_run.py`

 * *Files identical despite different names*

## Comparing `pp_project_pkg-1.0.202306182129.dist-info/RECORD` & `pp_project_pkg-1.0.202306182156.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 pp_project_pkg/__init__.py,sha256=9idX2X6SQKZg--ziGy6Ii9OB-kz9hOX1nEG9a0xEW9g,71
 pp_project_pkg/linear_train.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pp_project_pkg/newsvendor.py,sha256=E6JHp0Vtmq63toKM6bO3xTAdCgwmAZzRua-w10wrc5Y,577
 pp_project_pkg/pp_tables.py,sha256=8rqVp4P9nF13UbBmN_R7vGK7MeY4BkeG2ibDa7jLRpg,7115
 pp_project_pkg/utils.py,sha256=HpFZUMcULReiYvfwOycdy1Xrfyr32qXcAN0gl2xrgnM,4190
-pp_project_pkg/version.py,sha256=a_exhTKKG1k1WtCELjUA4io-ZHLPsG8dCaYkcU7eHOA,396
-pp_project_pkg/wrangling.py,sha256=rTDhW4hNytVSargqNoJlub_wyN37zPElVtKNc2TaRlw,4391
-pp_project_pkg-1.0.202306182129.data/scripts/get_tables.py,sha256=E5FmW2bHAU9NPORQMG85RzGtXOGjjzbATEa5lLGjyk4,65
-pp_project_pkg-1.0.202306182129.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
-pp_project_pkg-1.0.202306182129.dist-info/METADATA,sha256=fcUqHfgViSBkQcrScMyT7gakjiFXg2MrGpV1AHLw21Y,191
-pp_project_pkg-1.0.202306182129.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-pp_project_pkg-1.0.202306182129.dist-info/top_level.txt,sha256=2V1bEC5qsYRo1f2gAotX3L3S5xl1nIUxjITUTeRd8yQ,15
-pp_project_pkg-1.0.202306182129.dist-info/RECORD,,
+pp_project_pkg/version.py,sha256=q9q9h959xm6kb9ytuLGAiq5XFOGCvQjVBBbbEjdKJPo,396
+pp_project_pkg/wrangling.py,sha256=_8pEiN1ktE98SfuAmIUkufgPdtM3NI4j8H1mOY2Zg0c,4595
+pp_project_pkg-1.0.202306182156.data/scripts/get_tables.py,sha256=E5FmW2bHAU9NPORQMG85RzGtXOGjjzbATEa5lLGjyk4,65
+pp_project_pkg-1.0.202306182156.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
+pp_project_pkg-1.0.202306182156.dist-info/METADATA,sha256=0IGHmk6l5pmNef6pEhouJRGS0JebkvxCQFkW81iSOdg,191
+pp_project_pkg-1.0.202306182156.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+pp_project_pkg-1.0.202306182156.dist-info/top_level.txt,sha256=2V1bEC5qsYRo1f2gAotX3L3S5xl1nIUxjITUTeRd8yQ,15
+pp_project_pkg-1.0.202306182156.dist-info/RECORD,,
```

