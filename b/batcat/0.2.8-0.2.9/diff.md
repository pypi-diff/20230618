# Comparing `tmp/batcat-0.2.8-py3-none-any.whl.zip` & `tmp/batcat-0.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 21427 bytes, number of entries: 18
--rw-r--r--  2.0 unx     1544 b- defN 22-Aug-11 06:04 batcat/Athena.py
+Zip file size: 21434 bytes, number of entries: 18
+-rw-r--r--  2.0 unx     1542 b- defN 22-Aug-11 06:15 batcat/Athena.py
 -rw-r--r--  2.0 unx     3094 b- defN 22-Aug-11 02:47 batcat/Docker.py
 -rw-r--r--  2.0 unx     5443 b- defN 22-Aug-11 06:03 batcat/FileSys.py
 -rw-r--r--  2.0 unx      745 b- defN 22-Aug-11 02:43 batcat/Lambda.py
 -rw-r--r--  2.0 unx     1670 b- defN 22-Aug-11 02:40 batcat/Logging.py
--rw-r--r--  2.0 unx     8304 b- defN 22-Aug-11 06:05 batcat/Redshift.py
+-rw-r--r--  2.0 unx     8302 b- defN 22-Aug-11 06:15 batcat/Redshift.py
 -rw-r--r--  2.0 unx     9991 b- defN 22-Aug-11 02:48 batcat/Stepfunctions.py
 -rw-r--r--  2.0 unx     4027 b- defN 22-Aug-11 06:02 batcat/Storage.py
 -rw-r--r--  2.0 unx      355 b- defN 22-Jun-22 07:23 batcat/__init__.py
--rw-r--r--  2.0 unx      163 b- defN 22-Aug-11 06:05 batcat/__version__.py
+-rw-r--r--  2.0 unx      163 b- defN 22-Aug-11 06:15 batcat/__version__.py
 -rw-r--r--  2.0 unx     1426 b- defN 22-Aug-11 06:04 batcat/core.py
 -rw-r--r--  2.0 unx     3673 b- defN 22-Jan-12 07:02 batcat/s3.py
 -rw-r--r--  2.0 unx     7153 b- defN 22-May-31 07:42 batcat/stepfunction.py
--rw-r--r--  2.0 unx     1066 b- defN 22-Aug-11 06:07 batcat-0.2.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     3510 b- defN 22-Aug-11 06:07 batcat-0.2.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Aug-11 06:07 batcat-0.2.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 22-Aug-11 06:07 batcat-0.2.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1345 b- defN 22-Aug-11 06:07 batcat-0.2.8.dist-info/RECORD
-18 files, 53608 bytes uncompressed, 19275 bytes compressed:  64.0%
+-rw-r--r--  2.0 unx     1066 b- defN 22-Aug-11 06:21 batcat-0.2.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3510 b- defN 22-Aug-11 06:21 batcat-0.2.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Aug-11 06:21 batcat-0.2.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 22-Aug-11 06:21 batcat-0.2.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1345 b- defN 22-Aug-11 06:21 batcat-0.2.9.dist-info/RECORD
+18 files, 53604 bytes uncompressed, 19282 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: batcat/s3.py
 Comment: 
 
 Filename: batcat/stepfunction.py
 Comment: 
 
-Filename: batcat-0.2.8.dist-info/LICENSE
+Filename: batcat-0.2.9.dist-info/LICENSE
 Comment: 
 
-Filename: batcat-0.2.8.dist-info/METADATA
+Filename: batcat-0.2.9.dist-info/METADATA
 Comment: 
 
-Filename: batcat-0.2.8.dist-info/WHEEL
+Filename: batcat-0.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: batcat-0.2.8.dist-info/top_level.txt
+Filename: batcat-0.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: batcat-0.2.8.dist-info/RECORD
+Filename: batcat-0.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## batcat/Athena.py

```diff
@@ -32,15 +32,15 @@
     """Read data as DataFrame from AWS Athena.
 
     Args:
         query (str): Querry to obtain data from Athena.
         region (str): Region of the AWS environment, eg. "cn-northwest-1".
         s3_staging_dir (str): S3 staging directory, eg. "s3://#####-###-###-queryresult/ATHENA_QUERY".
         date_start (str): Date to start, strftime('%Y/%m/%d').
-        date_start (str): Date to end, strftime('%Y/%m/%d').
+        date_end (str): Date to end, strftime('%Y/%m/%d').
     
     Returns:    
         df (pandas.DataFrame): dataframe.
     """
 
     cursor = connect(s3_staging_dir=s3_staging_dir,
                      region_name=region,
```

## batcat/Redshift.py

```diff
@@ -36,15 +36,15 @@
         query (str): Querry to obtain data from Redshift, str.
         host (str): Redshift configuration.
         password (str): Redshift configuration.
         port (str): Redshift configuration.
         database (str): Redshift configuration.
         user (str): Redshift configuration.
         date_start (str): Date to start, strftime('%Y/%m/%d').
-        date_start (str): Date to end, strftime('%Y/%m/%d').
+        date_end (str): Date to end, strftime('%Y/%m/%d').
 
 
     Returns:
         df (pandas.DataFrame): target dataframe
     """
     
     cursor = connect(host=host,
```

## batcat/__version__.py

```diff
@@ -1,8 +1,8 @@
-VERSION = (0, 2, 8)
+VERSION = (0, 2, 9)
 
 __version__ = '.'.join(map(str, VERSION))
 
 # python3 setup.py bdist_wheel
 # python3 -m twine upload dist/*
 
 # pip3 install dist/my-project.whl
```

## Comparing `batcat-0.2.8.dist-info/LICENSE` & `batcat-0.2.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `batcat-0.2.8.dist-info/METADATA` & `batcat-0.2.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batcat
-Version: 0.2.8
+Version: 0.2.9
 Summary: BatCat, A Cat Looks Like A Bat.
 Home-page: https://github.com/Ewen2015/BatCat
 Author: Ewen Wang
 Author-email: wolfgangwong2012@gmail.com
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
```

## Comparing `batcat-0.2.8.dist-info/RECORD` & `batcat-0.2.9.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-batcat/Athena.py,sha256=lgEuogEV-QHCvBREDBUSXT1Gbb_IWlhRbLJejDjVGuA,1544
+batcat/Athena.py,sha256=HIX7_JQVDHOYvDGx6i6zd8myz1G1K5bLSdFshhqS9yQ,1542
 batcat/Docker.py,sha256=eJgP1nJHxjGqLQ9NNFNj2zAozyAsixZ9Ok7WA5jb2kU,3094
 batcat/FileSys.py,sha256=W5wEvAK0V55JsQCEdXt5yVGGzsYjnlRT1KHfmBzj4Fo,5443
 batcat/Lambda.py,sha256=xi34jDpNccMvJJN9yrpJl-dirIgtgAkqd1SkXEoUBd4,745
 batcat/Logging.py,sha256=fEYxm4aGEZvkDH-ZU3KrpFjioLTvp-IkRgTnvjjXQqo,1670
-batcat/Redshift.py,sha256=3rqwIBucVzwT5gW2BMroIWorlJ7fZjBJBmITXCWGDDs,8304
+batcat/Redshift.py,sha256=HbrU4Pz5ncvOvU_yfeJs9PYNHYKljJqg2q7rM8kEblg,8302
 batcat/Stepfunctions.py,sha256=GQ4mnqcYTVNFUnPxnYTf0cK7kad471fvqVpt-IgWZdo,9991
 batcat/Storage.py,sha256=TMVJF8KlnUt8HZSZDiLqH6PxqYYDXyHZFB9UlmGsoSg,4027
 batcat/__init__.py,sha256=jRQ4Yx52di6gj7QKtxzEMJtkm61laaojgYjdBIt9LWY,355
-batcat/__version__.py,sha256=RTXmXFYeu73oS4raLKvzrk2XqIbc_HVJyUL9LVXIIcg,163
+batcat/__version__.py,sha256=NoYNeStAdDgw6H7hcKwWNecVLk2M5P0hjwcKgMnU6wM,163
 batcat/core.py,sha256=XzFr8IJIp4qe4pADQO3gUhkCmsRSkMaw-sJaWp5OIXE,1426
 batcat/s3.py,sha256=XNaQpz3mueUeXX5z0eGU1kT68HwBkulwPiAPZYhZKY8,3673
 batcat/stepfunction.py,sha256=c_V5CeMTl_D3J3Tewo0k2Qlt77ebqM2MkqREKQ5m-68,7153
-batcat-0.2.8.dist-info/LICENSE,sha256=UEwfcb3EiV_u_j5yPgN2mbPCo2LqEWPz2Fw9acB94bw,1066
-batcat-0.2.8.dist-info/METADATA,sha256=PdKXQpuGfp59NCa_KyREOjs7gdvg9Ishy9AYsAyJfWM,3510
-batcat-0.2.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-batcat-0.2.8.dist-info/top_level.txt,sha256=QirwQtE5DF66necyVBGtfrnV2UVWGem_1TFCt1TuZ8Y,7
-batcat-0.2.8.dist-info/RECORD,,
+batcat-0.2.9.dist-info/LICENSE,sha256=UEwfcb3EiV_u_j5yPgN2mbPCo2LqEWPz2Fw9acB94bw,1066
+batcat-0.2.9.dist-info/METADATA,sha256=QViF7tOEN4FtvFkAXBPdDkBWIFONj7QxUbY4y5n1qJg,3510
+batcat-0.2.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+batcat-0.2.9.dist-info/top_level.txt,sha256=QirwQtE5DF66necyVBGtfrnV2UVWGem_1TFCt1TuZ8Y,7
+batcat-0.2.9.dist-info/RECORD,,
```

