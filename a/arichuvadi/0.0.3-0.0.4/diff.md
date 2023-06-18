# Comparing `tmp/arichuvadi-0.0.3.tar.gz` & `tmp/arichuvadi-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/vanangamudi/agam/projects/code/tamilnlp/arichuvadi/dist/tmpi04gptrl/arichuvadi-0.0.3.tar", last modified: Tue Jul 26 05:43:04 2022, max compression
+gzip compressed data, was "/home/vanangamudi/agam/projects/code/tamilnlp/arichuvadi/dist/.tmp-1r_fyt_2/arichuvadi-0.0.4.tar", last modified: Sun Jun 18 19:48:18 2023, max compression
```

## Comparing `arichuvadi-0.0.3.tar` & `arichuvadi-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2022-07-26 05:43:04.214788 arichuvadi-0.0.3/
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)    35149 2022-07-15 17:10:03.000000 arichuvadi-0.0.3/LICENSE
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)       25 2022-07-26 05:42:53.000000 arichuvadi-0.0.3/MANIFEST.in
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)    42478 2022-07-26 05:43:04.214788 arichuvadi-0.0.3/PKG-INFO
-drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2022-07-26 05:43:04.214788 arichuvadi-0.0.3/mlm/
-drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2022-07-26 05:43:04.214788 arichuvadi-0.0.3/mlm/arichuvadi.egg-info/
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)    42478 2022-07-26 05:43:04.000000 arichuvadi-0.0.3/mlm/arichuvadi.egg-info/PKG-INFO
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)      273 2022-07-26 05:43:04.000000 arichuvadi-0.0.3/mlm/arichuvadi.egg-info/SOURCES.txt
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)        1 2022-07-26 05:43:04.000000 arichuvadi-0.0.3/mlm/arichuvadi.egg-info/dependency_links.txt
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)        8 2022-07-26 05:43:04.000000 arichuvadi-0.0.3/mlm/arichuvadi.egg-info/top_level.txt
-drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2022-07-26 05:43:04.214788 arichuvadi-0.0.3/mlm/tharavu/
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     5615 2022-07-20 07:20:46.000000 arichuvadi-0.0.3/mlm/tharavu/adaiyalamitta-ari.txt
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)      488 2022-07-20 08:12:36.000000 arichuvadi-0.0.3/mlm/tharavu/ari-uni.txt
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     2349 2022-07-20 08:04:19.000000 arichuvadi-0.0.3/mlm/tharavu/ari.txt
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)      813 2022-07-26 05:41:35.000000 arichuvadi-0.0.3/pyproject.toml
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)       38 2022-07-26 05:43:04.214788 arichuvadi-0.0.3/setup.cfg
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)       92 2022-07-20 18:40:03.000000 arichuvadi-0.0.3/setup.py
+drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 19:48:18.181599 arichuvadi-0.0.4/
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)    35149 2022-07-15 17:10:03.000000 arichuvadi-0.0.4/LICENSE.txt
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)       72 2023-06-18 18:27:07.000000 arichuvadi-0.0.4/MANIFEST.in
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     1931 2023-06-18 19:48:18.181599 arichuvadi-0.0.4/PKG-INFO
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     1447 2022-07-20 10:00:04.000000 arichuvadi-0.0.4/README.txt
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     1447 2022-07-20 10:00:04.000000 arichuvadi-0.0.4/YENNAI_PADI.txt
+drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 19:48:18.181599 arichuvadi-0.0.4/mlm/
+drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 19:48:18.181599 arichuvadi-0.0.4/mlm/arichuvadi/
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)       26 2023-06-18 19:08:18.000000 arichuvadi-0.0.4/mlm/arichuvadi/__init__.py
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     5206 2023-06-18 18:39:19.000000 arichuvadi-0.0.4/mlm/arichuvadi/arichuvadi.py
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)      309 2023-06-18 18:41:33.000000 arichuvadi-0.0.4/mlm/arichuvadi/valam.py
+drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 19:48:18.181599 arichuvadi-0.0.4/mlm/arichuvadi.egg-info/
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     1931 2023-06-18 19:48:18.000000 arichuvadi-0.0.4/mlm/arichuvadi.egg-info/PKG-INFO
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)      384 2023-06-18 19:48:18.000000 arichuvadi-0.0.4/mlm/arichuvadi.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)        1 2023-06-18 19:48:18.000000 arichuvadi-0.0.4/mlm/arichuvadi.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)       19 2023-06-18 19:48:18.000000 arichuvadi-0.0.4/mlm/arichuvadi.egg-info/top_level.txt
+drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 19:48:18.181599 arichuvadi-0.0.4/mlm/tharavu/
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     5612 2022-07-29 07:42:40.000000 arichuvadi-0.0.4/mlm/tharavu/adaiyalamitta-ari.txt
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)      488 2022-07-20 08:12:36.000000 arichuvadi-0.0.4/mlm/tharavu/ari-uni.txt
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     2349 2022-07-20 08:04:19.000000 arichuvadi-0.0.4/mlm/tharavu/ari.txt
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)      841 2023-06-18 19:46:28.000000 arichuvadi-0.0.4/pyproject.toml
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)       38 2023-06-18 19:48:18.181599 arichuvadi-0.0.4/setup.cfg
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)       92 2022-07-20 18:40:03.000000 arichuvadi-0.0.4/setup.py
```

### Comparing `arichuvadi-0.0.3/LICENSE` & `arichuvadi-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arichuvadi-0.0.3/mlm/tharavu/adaiyalamitta-ari.txt` & `arichuvadi-0.0.4/mlm/tharavu/adaiyalamitta-ari.txt`

 * *Files 0% similar despite different names*

```diff
@@ -41,21 +41,21 @@
 எழுத்து:உயிர்மெய்:கிரந்தம்		:=	ஸ	ஸா	ஸி	ஸீ	ஸு	ஸூ	ஸெ	ஸே	ஸை	ஸொ	ஸோ	ஸௌ
 எழுத்து:உயிர்மெய்:கிரந்தம்		:=	ஹ	ஹா	ஹி	ஹீ	ஹு	ஹூ	ஹெ	ஹே	ஹை	ஹொ	ஹோ	ஹௌ
 எழுத்து:உயிர்மெய்:கிரந்தம்		:=	க்ஷ	க்ஷா	க்ஷி	க்ஷீ	க்ஷு	க்ஷூ	க்ஷெ	க்ஷே	க்ஷை	க்ஷொ	க்ஷோ	க்ஷௌ	
 
 ஒருங்குறி:உயிர்க்குறி			:=	_	ா	ி	ீ	ு	ூ	ெ	ே	ை	ொ	ோ	ௌ
 
 எண்கள்:தமிழ்			:=	௦	௧	௨	௩	௪	௫	௬	௭	௮	௯	௰
-#எண்கள்:அரபி			:=	0	1	2	3	4	5	6	7	8	9	10
+எண்கள்:அரபி			:=	0	1	2	3	4	5	6	7	8	9	10
 
 எண்கள்:தமிழ்			:=	௱
-#எண்கள்:அரபி			:=	100
+எண்கள்:அரபி			:=	100
 
 எண்கள்:தமிழ்			:=	௲
-#எண்கள்:அரபி			:=	1000
+எண்கள்:அரபி			:=	1000
 
 குறி:நாள்				:=	௳
 குறி:மாதம்				:=	௴
 குறி:ஆண்டு				:=	௵
 குறி:செலவு				:=	௶
 குறி:வரவு				:=	௷
 குறி:உருவாய்				:=	௹
```

### Comparing `arichuvadi-0.0.3/mlm/tharavu/ari.txt` & `arichuvadi-0.0.4/mlm/tharavu/ari.txt`

 * *Files identical despite different names*

### Comparing `arichuvadi-0.0.3/pyproject.toml` & `arichuvadi-0.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "arichuvadi"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="vanangamudi", email="selva.developer@gmail.com" },
 ]
 description = "a basic set of tools to work with Tamil text"
 readme = "YENNAI_PADI.txt"
 license = { file="LICENSE" }
 requires-python = ">=3.5"
@@ -19,14 +19,15 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/vanangamudi/arichuvadi"
 "Bug Tracker" = "https://github.com/vanangamudi/arichuvadi/issues"
 
 [tool.setuptools]
+#package-dir = {"" = "mlm"}
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["mlm"]  # ["."] by default
 include = ["*"]  # ["*"] by default
 exclude = []  # empty by default
 namespaces = true  # true by default
```

