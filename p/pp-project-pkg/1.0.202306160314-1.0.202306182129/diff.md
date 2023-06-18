# Comparing `tmp/pp_project_pkg-1.0.202306160314-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202306182129-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 7988 bytes, number of entries: 12
+Zip file size: 8590 bytes, number of entries: 13
 -rw-rw-r--  2.0 unx       71 b- defN 23-Jun-07 11:24 pp_project_pkg/__init__.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jun-18 21:29 pp_project_pkg/linear_train.py
 -rw-rw-r--  2.0 unx      577 b- defN 23-Jun-07 11:24 pp_project_pkg/newsvendor.py
 -rw-rw-r--  2.0 unx     7115 b- defN 23-Jun-07 11:24 pp_project_pkg/pp_tables.py
--rw-rw-r--  2.0 unx     3004 b- defN 23-Jun-16 03:14 pp_project_pkg/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jun-16 03:14 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx     4190 b- defN 23-Jun-18 21:13 pp_project_pkg/utils.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jun-18 21:29 pp_project_pkg/version.py
 -rw-rw-r--  2.0 unx     4391 b- defN 23-Jun-16 01:49 pp_project_pkg/wrangling.py
--rwxrwxr-x  2.0 unx       65 b- defN 23-Jun-02 12:43 pp_project_pkg-1.0.202306160314.data/scripts/get_tables.py
--rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-07 11:24 pp_project_pkg-1.0.202306160314.data/scripts/pp_project_run.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jun-16 03:15 pp_project_pkg-1.0.202306160314.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-16 03:15 pp_project_pkg-1.0.202306160314.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-16 03:15 pp_project_pkg-1.0.202306160314.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1095 b- defN 23-Jun-16 03:15 pp_project_pkg-1.0.202306160314.dist-info/RECORD
-12 files, 18328 bytes uncompressed, 6102 bytes compressed:  66.7%
+-rwxrwxr-x  2.0 unx       65 b- defN 23-Jun-02 12:43 pp_project_pkg-1.0.202306182129.data/scripts/get_tables.py
+-rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-07 11:24 pp_project_pkg-1.0.202306182129.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jun-18 21:29 pp_project_pkg-1.0.202306182129.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-18 21:29 pp_project_pkg-1.0.202306182129.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Jun-18 21:29 pp_project_pkg-1.0.202306182129.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1179 b- defN 23-Jun-18 21:29 pp_project_pkg-1.0.202306182129.dist-info/RECORD
+13 files, 19598 bytes uncompressed, 6568 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: pp_project_pkg/__init__.py
 Comment: 
 
+Filename: pp_project_pkg/linear_train.py
+Comment: 
+
 Filename: pp_project_pkg/newsvendor.py
 Comment: 
 
 Filename: pp_project_pkg/pp_tables.py
 Comment: 
 
 Filename: pp_project_pkg/utils.py
@@ -12,26 +15,26 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306160314.data/scripts/get_tables.py
+Filename: pp_project_pkg-1.0.202306182129.data/scripts/get_tables.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306160314.data/scripts/pp_project_run.py
+Filename: pp_project_pkg-1.0.202306182129.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306160314.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202306182129.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306160314.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202306182129.dist-info/WHEEL
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306160314.dist-info/top_level.txt
+Filename: pp_project_pkg-1.0.202306182129.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306160314.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202306182129.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pp_project_pkg/utils.py

```diff
@@ -1,19 +1,20 @@
 import wml.visionml as wv
 import datetime
 import mb.pandas as pd
 
-__all__ = ['site_date_res','check_if_valid_date','check_report_close_date','create_date_table']
+__all__ = ['site_date_res','check_if_valid_date','check_report_close_date','create_date_table',
+           'download_upload_dates_report','compare_report_dates']
 
 
 def site_date_res(site_id= 30607):
     """
     Get the site date report closure data
     Args:
-        site_id : Site id for fetching the date wise result. Site_id : 30607 (Waldof)
+        site_id : Site id for fetching the date wise result. Site_id : 30607 (Waldof Astoria)
     
     Returns:
         pd.DateFrame
     """
     q1 = """
     select s.start_date,s.id,s.meal_service_state, s.closed,s.updated from pp_meal_service.view_current_state cs
                join pp_meal_service.view_service s on s.view_current_state_id = cs.id
@@ -52,15 +53,15 @@
     Args:
         start_date: start date of the date table. format : '2023-06-06'
         end_date: end date of the date table. format : '2023-06-06'
     Output:
         pd.DataFrame
     """    
     date_index = pd.date_range(start=start_date, end=end_date, freq='D')
-    df = pd.DataFrame({'datetime': date_index.date,'closed':None})
+    df = pd.DataFrame({'date': date_index.date,'closed':None})
     return df
 
 def check_report_close_date(site_res,start_date='2023-06-06', end_date='2023-12-31'):
     """
     Check if the dates has closed the report.
 
     Args:
@@ -80,9 +81,40 @@
     for i in range(len(site_res_date_new)):
         k = site_res_date_new.iloc[i]['start_date']
         l = site_res_date_new.iloc[i]['closed']
         if l is not None or l is not pd.NaT:
             l = l.to_pydatetime().date()
         else:
             l = None
-        create_date_table_res.loc[create_date_table_res['datetime']==k,'closed']=l
-    return create_date_table_res
+        create_date_table_res.loc[create_date_table_res['date']==k,'closed']=l
+    return create_date_table_res
+
+def compare_report_dates(rep_new,rep_old = 'site_30607_report_dates'):
+    """
+    Compare two report dates and return the difference in days.
+    Args:
+        rep_new : newly created on todays date
+        rep_old : table on the production project pp_tables schema
+    Returns:
+        df : pd.DataFrame of newly closed report dates
+    """
+    merged_df = pd.merge(rep_new, rep_old, on='date', how='left', indicator=True)
+    result_df = merged_df[merged_df['_merge'] == 'left_only'].drop(columns='_merge')
+    return result_df
+
+def download_upload_dates_report(res_new,logger=None):
+    """
+    Download the report of the dates of the result of the compared report 
+    Args:
+        res_rep : result of the compared report
+    Returns:
+        none
+    """
+    q1 = """ 
+    SELECT * FROM pp_tables.waldorf_data
+    """
+    download_file = wv.read_sql(q1,wv.ml_engine)
+    res_rep = compare_report_dates(res_new,download_file)
+    if logger:
+        logger.info("Uploading records total : {}".format(len(res_rep)))
+    wv.to_sql(res_rep,wv.ml_engine,table_name='waldorf_data',if_exists='replace',index=False)
+
```

## pp_project_pkg/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('06')
-VERSION_DAY = int('16')
-VERSION_HOUR = int('03')
-VERSION_MINUTE = int('14')
+VERSION_DAY = int('18')
+VERSION_HOUR = int('21')
+VERSION_MINUTE = int('29')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202306160314
-version_date = '2023/06/16 03:14'
+PATCH_VERSION = 202306182129
+version_date = '2023/06/18 21:29'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `pp_project_pkg-1.0.202306160314.data/scripts/pp_project_run.py` & `pp_project_pkg-1.0.202306182129.data/scripts/pp_project_run.py`

 * *Files identical despite different names*

## Comparing `pp_project_pkg-1.0.202306160314.dist-info/RECORD` & `pp_project_pkg-1.0.202306182129.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 pp_project_pkg/__init__.py,sha256=9idX2X6SQKZg--ziGy6Ii9OB-kz9hOX1nEG9a0xEW9g,71
+pp_project_pkg/linear_train.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pp_project_pkg/newsvendor.py,sha256=E6JHp0Vtmq63toKM6bO3xTAdCgwmAZzRua-w10wrc5Y,577
 pp_project_pkg/pp_tables.py,sha256=8rqVp4P9nF13UbBmN_R7vGK7MeY4BkeG2ibDa7jLRpg,7115
-pp_project_pkg/utils.py,sha256=aRS8ermeFuS_UuJfDMDS5-WB_euxC3pn7eKI8PUgLRY,3004
-pp_project_pkg/version.py,sha256=wIFrj2e1PHhGkpKim9hHp6qbbGpcGnFfm7p2qfMqnaY,396
+pp_project_pkg/utils.py,sha256=HpFZUMcULReiYvfwOycdy1Xrfyr32qXcAN0gl2xrgnM,4190
+pp_project_pkg/version.py,sha256=a_exhTKKG1k1WtCELjUA4io-ZHLPsG8dCaYkcU7eHOA,396
 pp_project_pkg/wrangling.py,sha256=rTDhW4hNytVSargqNoJlub_wyN37zPElVtKNc2TaRlw,4391
-pp_project_pkg-1.0.202306160314.data/scripts/get_tables.py,sha256=E5FmW2bHAU9NPORQMG85RzGtXOGjjzbATEa5lLGjyk4,65
-pp_project_pkg-1.0.202306160314.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
-pp_project_pkg-1.0.202306160314.dist-info/METADATA,sha256=0XoDCt9Jmx0eVX1GuU4F-AuWzMRtrDs1-DxF3PuTV6I,191
-pp_project_pkg-1.0.202306160314.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-pp_project_pkg-1.0.202306160314.dist-info/top_level.txt,sha256=2V1bEC5qsYRo1f2gAotX3L3S5xl1nIUxjITUTeRd8yQ,15
-pp_project_pkg-1.0.202306160314.dist-info/RECORD,,
+pp_project_pkg-1.0.202306182129.data/scripts/get_tables.py,sha256=E5FmW2bHAU9NPORQMG85RzGtXOGjjzbATEa5lLGjyk4,65
+pp_project_pkg-1.0.202306182129.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
+pp_project_pkg-1.0.202306182129.dist-info/METADATA,sha256=fcUqHfgViSBkQcrScMyT7gakjiFXg2MrGpV1AHLw21Y,191
+pp_project_pkg-1.0.202306182129.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+pp_project_pkg-1.0.202306182129.dist-info/top_level.txt,sha256=2V1bEC5qsYRo1f2gAotX3L3S5xl1nIUxjITUTeRd8yQ,15
+pp_project_pkg-1.0.202306182129.dist-info/RECORD,,
```

