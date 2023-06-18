# Comparing `tmp/rapidocr_web-0.1.6-py3-none-any.whl.zip` & `tmp/rapidocr_web-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 41043 bytes, number of entries: 12
--rw-r--r--  2.0 unx       73 b- defN 23-May-21 13:22 rapidocr_web/__init__.py
--rw-r--r--  2.0 unx     1264 b- defN 23-May-21 13:22 rapidocr_web/ocrweb.py
--rw-r--r--  2.0 unx     3043 b- defN 23-May-21 13:22 rapidocr_web/task.py
--rw-r--r--  2.0 unx    16958 b- defN 23-May-21 13:22 rapidocr_web/static/css/favicon.ico
--rw-r--r--  2.0 unx     2065 b- defN 23-May-21 13:22 rapidocr_web/static/css/main.css
--rw-r--r--  2.0 unx    86341 b- defN 23-May-21 13:22 rapidocr_web/static/js/jquery-3.0.0.min.js
--rw-r--r--  2.0 unx     8202 b- defN 23-May-21 13:22 rapidocr_web/templates/index.html
--rw-r--r--  2.0 unx     1909 b- defN 23-May-21 13:22 rapidocr_web-0.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-21 13:22 rapidocr_web-0.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       59 b- defN 23-May-21 13:22 rapidocr_web-0.1.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-May-21 13:22 rapidocr_web-0.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1025 b- defN 23-May-21 13:22 rapidocr_web-0.1.6.dist-info/RECORD
-12 files, 121044 bytes uncompressed, 39307 bytes compressed:  67.5%
+Zip file size: 41052 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       73 b- defN 23-Jun-18 12:05 rapidocr_web/__init__.py
+-rw-r--r--  2.0 unx     1264 b- defN 23-Jun-18 12:05 rapidocr_web/ocrweb.py
+-rw-r--r--  2.0 unx     3043 b- defN 23-Jun-18 12:05 rapidocr_web/task.py
+-rw-r--r--  2.0 unx    16958 b- defN 23-Jun-18 12:05 rapidocr_web/static/css/favicon.ico
+-rw-r--r--  2.0 unx     2065 b- defN 23-Jun-18 12:05 rapidocr_web/static/css/main.css
+-rw-r--r--  2.0 unx    86341 b- defN 23-Jun-18 12:05 rapidocr_web/static/js/jquery-3.0.0.min.js
+-rw-r--r--  2.0 unx     8202 b- defN 23-Jun-18 12:05 rapidocr_web/templates/index.html
+-rw-r--r--  2.0 unx     2008 b- defN 23-Jun-18 12:05 rapidocr_web-0.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-18 12:05 rapidocr_web-0.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-18 12:05 rapidocr_web-0.1.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-18 12:05 rapidocr_web-0.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1025 b- defN 23-Jun-18 12:05 rapidocr_web-0.1.7.dist-info/RECORD
+12 files, 121143 bytes uncompressed, 39316 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: rapidocr_web/static/js/jquery-3.0.0.min.js
 Comment: 
 
 Filename: rapidocr_web/templates/index.html
 Comment: 
 
-Filename: rapidocr_web-0.1.6.dist-info/METADATA
+Filename: rapidocr_web-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: rapidocr_web-0.1.6.dist-info/WHEEL
+Filename: rapidocr_web-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: rapidocr_web-0.1.6.dist-info/entry_points.txt
+Filename: rapidocr_web-0.1.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapidocr_web-0.1.6.dist-info/top_level.txt
+Filename: rapidocr_web-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: rapidocr_web-0.1.6.dist-info/RECORD
+Filename: rapidocr_web-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `rapidocr_web-0.1.6.dist-info/METADATA` & `rapidocr_web-0.1.7.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: rapidocr-web
-Version: 0.1.6
+Version: 0.1.7
 Summary: A cross platform OCR Library based on OnnxRuntime.
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
 Requires-Dist: Flask (>=2.1.0)
 Requires-Dist: rapidocr-onnxruntime
 
 ## rapidocr-web
 <p>
-    <a href=""><img src="https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg"></a>
+    <a href=""><img src="https://img.shields.io/badge/Python->=3.6,<3.12-aff.svg"></a>
     <a href=""><img src="https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg"></a>
     <a href="https://pypi.org/project/rapidocr-web/"><img alt="PyPI" src="https://img.shields.io/pypi/v/rapidocr-web"></a>
     <a href="https://pepy.tech/project/rapidocr_web"><img src="https://static.pepy.tech/personalized-badge/rapidocr_web?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads"></a>
 </p>
 
 ### use
 1. Install package by pypi.
```

### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: rapidocr-web Version: 0.1.6 Summary: A cross
+Metadata-Version: 2.1 Name: rapidocr-web Version: 0.1.7 Summary: A cross
 platform OCR Library based on OnnxRuntime. Home-page: https://github.com/
 RapidAI/RapidOCR Author: SWHL Author-email: liekkaskono@163.com License:
 Apache-2.0 Download-URL: https://github.com/RapidAI/RapidOCR.git Keywords:
 ocr,text_detection,text_recognition,db,onnxruntime,paddleocr,openvino,rapidocr
-Platform: Any Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Requires-
-Python: >=3.7,<=3.10 Description-Content-Type: text/markdown Requires-Dist:
-requests Requires-Dist: Flask (>=2.1.0) Requires-Dist: rapidocr-onnxruntime ##
-rapidocr-web
-[https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg] [https://
+Platform: Any Classifier: Programming Language :: Python :: 3.6 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Requires-Python: >=3.6,<3.12 Description-Content-Type: text/
+markdown Requires-Dist: requests Requires-Dist: Flask (>=2.1.0) Requires-Dist:
+rapidocr-onnxruntime ## rapidocr-web
+[https://img.shields.io/badge/Python->=3.6,<3.12-aff.svg] [https://
 img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg] [PyPI] [https://
 static.pepy.tech/personalized-badge/
 rapidocr_web?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads]
 ### use 1. Install package by pypi. ```bash $ pip install rapidocr-web ``` 2.
 Run by command line. - Usage: ```bash $ rapidocr_web -h usage: rapidocr_web [-
 h] [-ip IP] [-p PORT] optional arguments: -h, --help show this help message and
 exit -ip IP, --ip IP IP Address -p PORT, --port PORT IP port ``` - Example:
```

## Comparing `rapidocr_web-0.1.6.dist-info/RECORD` & `rapidocr_web-0.1.7.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 rapidocr_web/__init__.py,sha256=JmySAOGOURKrbjdme2lVdTbDKaclr00IBKeVIa0_n30,73
 rapidocr_web/ocrweb.py,sha256=2YUp91COzzuJW5_XKwfng0-9VwtGXeRSOA3Kw_DAyfg,1264
 rapidocr_web/task.py,sha256=UVgdPds1NeZTtBnh_hjZiULUKOs_J1cU_hcQDm1Y5ts,3043
 rapidocr_web/static/css/favicon.ico,sha256=CBE1NF6iiIax8WqZVR-vPRaPTcmWjlTWsk1fzEbSd8c,16958
 rapidocr_web/static/css/main.css,sha256=2HcVvoa5oSQONnuC6IjjmBd127Jv9Y5EFJGy32nTEZk,2065
 rapidocr_web/static/js/jquery-3.0.0.min.js,sha256=JmvOoLtYsmqlsWxa7mDSLMwa6dZ9rrIdtrrVYRnDRH0,86341
 rapidocr_web/templates/index.html,sha256=xUe3Xce289Of4XTfeafPTX5JMRsOTdgv2Md5EQwxm48,8202
-rapidocr_web-0.1.6.dist-info/METADATA,sha256=HHoTfnj004peOoL7lrdjXE7L6R2b232ujIFFU8QGxaY,1909
-rapidocr_web-0.1.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rapidocr_web-0.1.6.dist-info/entry_points.txt,sha256=ivlPn9JP6ziblPQyG6N4H4cXfrJZ9FD5rvSYhnEc8cU,59
-rapidocr_web-0.1.6.dist-info/top_level.txt,sha256=dArjxF38AFvTF1Ae-mGaxBhwnETUJ4sLF_nQ93HC5A4,13
-rapidocr_web-0.1.6.dist-info/RECORD,,
+rapidocr_web-0.1.7.dist-info/METADATA,sha256=h1DtauYNAwI-zqCb9P8zzL46hN9wY1kmT8Dxahb9t34,2008
+rapidocr_web-0.1.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rapidocr_web-0.1.7.dist-info/entry_points.txt,sha256=ivlPn9JP6ziblPQyG6N4H4cXfrJZ9FD5rvSYhnEc8cU,59
+rapidocr_web-0.1.7.dist-info/top_level.txt,sha256=dArjxF38AFvTF1Ae-mGaxBhwnETUJ4sLF_nQ93HC5A4,13
+rapidocr_web-0.1.7.dist-info/RECORD,,
```

