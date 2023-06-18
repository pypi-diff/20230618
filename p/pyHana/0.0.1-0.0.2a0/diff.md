# Comparing `tmp/pyHana-0.0.1-py3-none-any.whl.zip` & `tmp/pyHana-0.0.2a0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 22315 bytes, number of entries: 19
+Zip file size: 22275 bytes, number of entries: 19
 -rw-rw-rw-  2.0 fat       87 b- defN 23-Jun-11 03:47 pyHana/__init__.py
 -rw-rw-rw-  2.0 fat       28 b- defN 23-Jun-04 13:58 pyHana/analysis/__init__.py
 -rw-rw-rw-  2.0 fat    16582 b- defN 23-Jun-18 12:17 pyHana/analysis/stockEcoIndex.py
 -rw-rw-rw-  2.0 fat       48 b- defN 23-Jun-09 22:21 pyHana/common/__init__.py
 -rw-rw-rw-  2.0 fat      516 b- defN 23-Jun-15 13:44 pyHana/common/conf.py
 -rw-rw-rw-  2.0 fat     1121 b- defN 23-Jun-18 12:45 pyHana/common/dataProc.py
 -rw-rw-rw-  2.0 fat     5047 b- defN 23-Jun-08 04:17 pyHana/common/graph.py
@@ -10,12 +10,12 @@
 -rw-rw-rw-  2.0 fat       56 b- defN 23-Jun-09 22:22 pyHana/innerIO/__init__.py
 -rw-rw-rw-  2.0 fat     2144 b- defN 23-Jun-18 12:21 pyHana/innerIO/ecoIndex.py
 -rw-rw-rw-  2.0 fat     6324 b- defN 23-Jun-18 12:21 pyHana/innerIO/stockData.py
 -rw-rw-rw-  2.0 fat       61 b- defN 23-Jun-09 22:22 pyHana/outerIO/__init__.py
 -rw-rw-rw-  2.0 fat    21451 b- defN 23-Jun-07 11:29 pyHana/outerIO/dart.py
 -rw-rw-rw-  2.0 fat    14998 b- defN 23-Jun-18 12:21 pyHana/outerIO/ebest.py
 -rw-rw-rw-  2.0 fat     1840 b- defN 23-Jun-18 12:21 pyHana/outerIO/ecoIndex.py
--rw-rw-rw-  2.0 fat      528 b- defN 23-Jun-18 13:39 pyHana-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-18 13:39 pyHana-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-18 13:39 pyHana-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1508 b- defN 23-Jun-18 13:39 pyHana-0.0.1.dist-info/RECORD
-19 files, 73119 bytes uncompressed, 19861 bytes compressed:  72.8%
+-rw-rw-rw-  2.0 fat      284 b- defN 23-Jun-18 14:16 pyHana-0.0.2a0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-18 14:16 pyHana-0.0.2a0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-18 14:16 pyHana-0.0.2a0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1516 b- defN 23-Jun-18 14:16 pyHana-0.0.2a0.dist-info/RECORD
+19 files, 72883 bytes uncompressed, 19805 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -39,20 +39,20 @@
 
 Filename: pyHana/outerIO/ebest.py
 Comment: 
 
 Filename: pyHana/outerIO/ecoIndex.py
 Comment: 
 
-Filename: pyHana-0.0.1.dist-info/METADATA
+Filename: pyHana-0.0.2a0.dist-info/METADATA
 Comment: 
 
-Filename: pyHana-0.0.1.dist-info/WHEEL
+Filename: pyHana-0.0.2a0.dist-info/WHEEL
 Comment: 
 
-Filename: pyHana-0.0.1.dist-info/top_level.txt
+Filename: pyHana-0.0.2a0.dist-info/top_level.txt
 Comment: 
 
-Filename: pyHana-0.0.1.dist-info/RECORD
+Filename: pyHana-0.0.2a0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pyHana-0.0.1.dist-info/RECORD` & `pyHana-0.0.2a0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 pyHana/innerIO/__init__.py,sha256=_HQnYZsDbczSz6jHKdVMcRnMo6X_rcC55k16fAMEJDs,56
 pyHana/innerIO/ecoIndex.py,sha256=Whf5GEinjaxQSKEHFgiSIaRjIBO9JsC4oTkf5Cppk2I,2144
 pyHana/innerIO/stockData.py,sha256=_Klb7YgfSjwMiKAxHKKqFipUkrCXK1l8HHzfJZF3408,6324
 pyHana/outerIO/__init__.py,sha256=JhxO_Qf0Mlls-Mpw8lZFO-Sf_C09r4Wx4wITxLTi4w0,61
 pyHana/outerIO/dart.py,sha256=d2NXmU6A7MpBEeUv4AdlEKIyTgO7hUGmSdVmp1X627w,21451
 pyHana/outerIO/ebest.py,sha256=dOxOcPgD6Jg_qes9aB1djOme6CsiSqFKpJLX966jneg,14998
 pyHana/outerIO/ecoIndex.py,sha256=Lbu9VrbWYy2Yo57iisfTi6dJlHUkbH1tDcBGeE5xC-c,1840
-pyHana-0.0.1.dist-info/METADATA,sha256=lQlE_Dd2nk_2Wenv4jhN3kbQUkxI6TsF92a7RSK-q0Q,528
-pyHana-0.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyHana-0.0.1.dist-info/top_level.txt,sha256=HB0jmziPuwk5hJlWnvEbaS8QkKv84NPwX8F6le7Tm1Y,7
-pyHana-0.0.1.dist-info/RECORD,,
+pyHana-0.0.2a0.dist-info/METADATA,sha256=VDVRyPKjpBdNkdJXReVgS1PsneiCjmbnz0kQnnxFvoY,284
+pyHana-0.0.2a0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyHana-0.0.2a0.dist-info/top_level.txt,sha256=HB0jmziPuwk5hJlWnvEbaS8QkKv84NPwX8F6le7Tm1Y,7
+pyHana-0.0.2a0.dist-info/RECORD,,
```

