# Comparing `tmp/rapidocr_api-0.0.2-py3-none-any.whl.zip` & `tmp/rapidocr_api-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4222 bytes, number of entries: 7
--rw-r--r--  2.0 unx       74 b- defN 23-May-27 01:02 rapidocr_api/__init__.py
--rw-r--r--  2.0 unx     2082 b- defN 23-May-27 01:02 rapidocr_api/api.py
--rw-r--r--  2.0 unx     4553 b- defN 23-May-27 01:03 rapidocr_api-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-27 01:03 rapidocr_api-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       56 b- defN 23-May-27 01:03 rapidocr_api-0.0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-May-27 01:03 rapidocr_api-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      573 b- defN 23-May-27 01:03 rapidocr_api-0.0.2.dist-info/RECORD
-7 files, 7443 bytes uncompressed, 3196 bytes compressed:  57.1%
+Zip file size: 4225 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       74 b- defN 23-Jun-18 12:05 rapidocr_api/__init__.py
+-rw-r--r--  2.0 unx     2082 b- defN 23-Jun-18 12:05 rapidocr_api/api.py
+-rw-r--r--  2.0 unx     4652 b- defN 23-Jun-18 12:06 rapidocr_api-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-18 12:06 rapidocr_api-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-18 12:06 rapidocr_api-0.0.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-18 12:06 rapidocr_api-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      573 b- defN 23-Jun-18 12:06 rapidocr_api-0.0.3.dist-info/RECORD
+7 files, 7542 bytes uncompressed, 3199 bytes compressed:  57.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: rapidocr_api/__init__.py
 Comment: 
 
 Filename: rapidocr_api/api.py
 Comment: 
 
-Filename: rapidocr_api-0.0.2.dist-info/METADATA
+Filename: rapidocr_api-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: rapidocr_api-0.0.2.dist-info/WHEEL
+Filename: rapidocr_api-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: rapidocr_api-0.0.2.dist-info/entry_points.txt
+Filename: rapidocr_api-0.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapidocr_api-0.0.2.dist-info/top_level.txt
+Filename: rapidocr_api-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: rapidocr_api-0.0.2.dist-info/RECORD
+Filename: rapidocr_api-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `rapidocr_api-0.0.2.dist-info/METADATA` & `rapidocr_api-0.0.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: rapidocr-api
-Version: 0.0.2
+Version: 0.0.3
 Summary: A cross platform OCR API Library based on OnnxRuntime.
 Home-page: https://github.com/RapidAI/RapidOCR
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Download-URL: https://github.com/RapidAI/RapidOCR.git
 Keywords: ocr,text_detection,text_recognition,db,onnxruntime,paddleocr,openvino,rapidocr
 Platform: Any
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7,<=3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.6,<3.12
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: rapidocr-onnxruntime
 Requires-Dist: fastapi
 Requires-Dist: uvicorn[standard]
 
 ## rapidocr-api
 <p>
-    <a href=""><img src="https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg"></a>
+    <a href=""><img src="https://img.shields.io/badge/Python->=3.6,<3.12-aff.svg"></a>
     <a href=""><img src="https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg"></a>
     <a href="https://pypi.org/project/rapidocr-api/"><img alt="PyPI" src="https://img.shields.io/pypi/v/rapidocr-api"></a>
     <a href="https://pepy.tech/project/rapidocr_api"><img src="https://static.pepy.tech/personalized-badge/rapidocr_api?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads"></a>
 </p>
 
 ### Use
 1. Install`rapidocr_api`
```

### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: rapidocr-api Version: 0.0.2 Summary: A cross
+Metadata-Version: 2.1 Name: rapidocr-api Version: 0.0.3 Summary: A cross
 platform OCR API Library based on OnnxRuntime. Home-page: https://github.com/
 RapidAI/RapidOCR Author: SWHL Author-email: liekkaskono@163.com License:
 Apache-2.0 Download-URL: https://github.com/RapidAI/RapidOCR.git Keywords:
 ocr,text_detection,text_recognition,db,onnxruntime,paddleocr,openvino,rapidocr
-Platform: Any Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Requires-
-Python: >=3.7,<=3.10 Description-Content-Type: text/markdown Requires-Dist:
-requests Requires-Dist: rapidocr-onnxruntime Requires-Dist: fastapi Requires-
-Dist: uvicorn[standard] ## rapidocr-api
-[https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg] [https://
+Platform: Any Classifier: Programming Language :: Python :: 3.6 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Requires-Python: >=3.6,<3.12 Description-Content-Type: text/
+markdown Requires-Dist: requests Requires-Dist: rapidocr-onnxruntime Requires-
+Dist: fastapi Requires-Dist: uvicorn[standard] ## rapidocr-api
+[https://img.shields.io/badge/Python->=3.6,<3.12-aff.svg] [https://
 img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg] [PyPI] [https://
 static.pepy.tech/personalized-badge/
 rapidocr_api?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads]
 ### Use 1. Install`rapidocr_api` ```bash $ pip install rapidocr_api ``` 2. Run
 - Usage: ```bash $ rapidocr_api -h usage: rapidocr_api [-h] [-ip IP] [-p PORT]
 optional arguments: -h, --help show this help message and exit -ip IP, --ip IP
 IP Address -p PORT, --port PORT IP port ``` - Example: ```bash $ rapidocr_api -
```

## Comparing `rapidocr_api-0.0.2.dist-info/RECORD` & `rapidocr_api-0.0.3.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 rapidocr_api/__init__.py,sha256=m-UGKHJ-31qL7pBis4nfoFz5fzb-dXsiTLNqY-xpSoA,74
 rapidocr_api/api.py,sha256=2ja-Sa0F6IB_V1cx0cHLoNv8rFOE_8EEiRD15lguCP8,2082
-rapidocr_api-0.0.2.dist-info/METADATA,sha256=zBXQKP2aPgMruxlFdwrWWzzGcjcEfkRKVy-rbvrjI1M,4553
-rapidocr_api-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rapidocr_api-0.0.2.dist-info/entry_points.txt,sha256=eyebK_Y51FH8A7SUEnvI_vjx5d67TrCbQkYQtaDwc8c,56
-rapidocr_api-0.0.2.dist-info/top_level.txt,sha256=aUFqn9ci2x8Qxo0jzaPUN_zmdk1Sjr_Yfa4gSGEQIpM,13
-rapidocr_api-0.0.2.dist-info/RECORD,,
+rapidocr_api-0.0.3.dist-info/METADATA,sha256=_zDsuE_Y-U4z4PTQOWmGm0J8EntfysDA-FnVpa1HHpk,4652
+rapidocr_api-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rapidocr_api-0.0.3.dist-info/entry_points.txt,sha256=eyebK_Y51FH8A7SUEnvI_vjx5d67TrCbQkYQtaDwc8c,56
+rapidocr_api-0.0.3.dist-info/top_level.txt,sha256=aUFqn9ci2x8Qxo0jzaPUN_zmdk1Sjr_Yfa4gSGEQIpM,13
+rapidocr_api-0.0.3.dist-info/RECORD,,
```

