# Comparing `tmp/info-chunks-to-embeddings-1.0.0.tar.gz` & `tmp/info-chunks-to-embeddings-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "info-chunks-to-embeddings-1.0.0.tar", last modified: Sun Jun 18 01:51:27 2023, max compression
+gzip compressed data, was "info-chunks-to-embeddings-1.0.1.tar", last modified: Sun Jun 18 01:53:56 2023, max compression
```

## Comparing `info-chunks-to-embeddings-1.0.0.tar` & `info-chunks-to-embeddings-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-18 01:51:27.921536 info-chunks-to-embeddings-1.0.0/
--rw-r--r--   0 chiubowen   (501) staff       (20)     4143 2023-06-18 01:51:27.921404 info-chunks-to-embeddings-1.0.0/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     4032 2023-06-18 01:51:27.000000 info-chunks-to-embeddings-1.0.0/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-18 01:51:27.921221 info-chunks-to-embeddings-1.0.0/info_chunks_to_embeddings.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     4143 2023-06-18 01:51:27.000000 info-chunks-to-embeddings-1.0.0/info_chunks_to_embeddings.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      343 2023-06-18 01:51:27.000000 info-chunks-to-embeddings-1.0.0/info_chunks_to_embeddings.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-06-18 01:51:27.000000 info-chunks-to-embeddings-1.0.0/info_chunks_to_embeddings.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       77 2023-06-18 01:51:27.000000 info-chunks-to-embeddings-1.0.0/info_chunks_to_embeddings.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       37 2023-06-18 01:51:27.000000 info-chunks-to-embeddings-1.0.0/info_chunks_to_embeddings.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       26 2023-06-18 01:51:27.000000 info-chunks-to-embeddings-1.0.0/info_chunks_to_embeddings.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     1926 2023-06-18 01:51:27.000000 info-chunks-to-embeddings-1.0.0/info_chunks_to_embeddings.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-06-18 01:51:27.921574 info-chunks-to-embeddings-1.0.0/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      564 2023-06-18 01:51:27.000000 info-chunks-to-embeddings-1.0.0/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-18 01:53:56.867202 info-chunks-to-embeddings-1.0.1/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     4149 2023-06-18 01:53:56.867040 info-chunks-to-embeddings-1.0.1/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     4038 2023-06-18 01:53:56.000000 info-chunks-to-embeddings-1.0.1/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-18 01:53:56.866789 info-chunks-to-embeddings-1.0.1/info_chunks_to_embeddings.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     4149 2023-06-18 01:53:56.000000 info-chunks-to-embeddings-1.0.1/info_chunks_to_embeddings.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      343 2023-06-18 01:53:56.000000 info-chunks-to-embeddings-1.0.1/info_chunks_to_embeddings.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-06-18 01:53:56.000000 info-chunks-to-embeddings-1.0.1/info_chunks_to_embeddings.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       77 2023-06-18 01:53:56.000000 info-chunks-to-embeddings-1.0.1/info_chunks_to_embeddings.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       37 2023-06-18 01:53:56.000000 info-chunks-to-embeddings-1.0.1/info_chunks_to_embeddings.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       26 2023-06-18 01:53:56.000000 info-chunks-to-embeddings-1.0.1/info_chunks_to_embeddings.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     1926 2023-06-18 01:53:56.000000 info-chunks-to-embeddings-1.0.1/info_chunks_to_embeddings.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-06-18 01:53:56.867249 info-chunks-to-embeddings-1.0.1/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      564 2023-06-18 01:53:56.000000 info-chunks-to-embeddings-1.0.1/setup.py
```

### Comparing `info-chunks-to-embeddings-1.0.0/PKG-INFO` & `info-chunks-to-embeddings-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: info-chunks-to-embeddings
-Version: 1.0.0
+Version: 1.0.1
 Description-Content-Type: text/markdown
 
 # info_chunks_to_embeddings.py
 info_chunks_to_embeddings.py 是一個將 JSON 檔案轉換為語句嵌入的工具。它使用 SentenceTransformer 模型將 JSON 文件中的內容轉換為相應的語句嵌入，然後將這些嵌入保存到指定的資料夾中。
 
 ```
 🐔動機: 
@@ -20,16 +20,14 @@
   doc-id_1H0NTLvF0oyURCw_YWBQJ8CkcL7pij5D_8zO_1gXMc5k_sha_0f813133_row_7.json
   doc-id_1H0NTLvF0oyURCw_YWBQJ8CkcL7pij5D_8zO_1gXMc5k_sha_0f813133_row_7.pt
 
 💣地雷: 
 . 要注意 info_chunk.json 裡面必須包含有 content 欄位才能轉 embeddings .pt 檔案
 ```
 
-
-
 ## 安裝
 要安裝 info_chunks_to_embeddings，請使用以下命令：
 ```
 python3 -m pip install info-chunks-to-embeddings
 ```
 
 ## 使用方法
@@ -52,19 +50,21 @@
 ## 示例
 例如，如果您的 JSON 檔案位於 `~/my_json_files` 資料夾中，並希望將生成的嵌入存儲在 `~/my_embeddings` 資料夾中，則可以運行以下命令：
 ```
 python info_chunks_to_embeddings.py --input-folder ~/my_json_files --embeddings-folder ~/my_embeddings
 ```
 
 ## 輸入資料檔案 info_chunk.json 舉例（需要有 content 欄位）
+```
 {
     "uuid4": "f0dd55f0-229b-46d8-92af-e3c5e7275c52",
     "time": "2023-06-18T01:02:35.411700Z",
     "content": "青春痘 青春痘是最常見的皮膚問題，是皮脂腺發炎所致，表面上可能是細菌感染、黴菌感染、蟎蟲寄生，但更深層來看，是性荷爾蒙代謝不良、腸道菌叢失衡、胰島素太高、肝臟代謝受阻造成。12-24歲青少年盛行率80%，25歲以上青年也高達50%，因為此階段的睪固酮和雌激素分泌最多。熬夜、高醣飲食、加工食物（尤其是垃圾食物）、臉部衛生習慣不好或過度清潔，都會引起青春痘。所以，要徹底解決青春痘並不難，但需要探討自己到底是哪個環節出問題。",
     "type": "google_sheet",
     "sheet_id": "1H0NTLvF0oyURCw_YWBQJ8CkcL7pij5D_8zO_1gXMc5k",
     "sheet_name": "健康百科問答知識庫",
     "worksheet_name": "工作表1",
     "download_time": "2023-06-18T00:57:05.222819Z",
     "download_filepath": "./data/users/boh/bohachu_gmail_com/google_sheet_downloader/2023-06-18/doc-id_1H0NTLvF0oyURCw_YWBQJ8CkcL7pij5D_8zO_1gXMc5k_sha_0f813133.csv",
     "row": 13
 }
+```
```

### Comparing `info-chunks-to-embeddings-1.0.0/README.md` & `info-chunks-to-embeddings-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,14 @@
   doc-id_1H0NTLvF0oyURCw_YWBQJ8CkcL7pij5D_8zO_1gXMc5k_sha_0f813133_row_7.json
   doc-id_1H0NTLvF0oyURCw_YWBQJ8CkcL7pij5D_8zO_1gXMc5k_sha_0f813133_row_7.pt
 
 💣地雷: 
 . 要注意 info_chunk.json 裡面必須包含有 content 欄位才能轉 embeddings .pt 檔案
 ```
 
-
-
 ## 安裝
 要安裝 info_chunks_to_embeddings，請使用以下命令：
 ```
 python3 -m pip install info-chunks-to-embeddings
 ```
 
 ## 使用方法
@@ -47,19 +45,21 @@
 ## 示例
 例如，如果您的 JSON 檔案位於 `~/my_json_files` 資料夾中，並希望將生成的嵌入存儲在 `~/my_embeddings` 資料夾中，則可以運行以下命令：
 ```
 python info_chunks_to_embeddings.py --input-folder ~/my_json_files --embeddings-folder ~/my_embeddings
 ```
 
 ## 輸入資料檔案 info_chunk.json 舉例（需要有 content 欄位）
+```
 {
     "uuid4": "f0dd55f0-229b-46d8-92af-e3c5e7275c52",
     "time": "2023-06-18T01:02:35.411700Z",
     "content": "青春痘 青春痘是最常見的皮膚問題，是皮脂腺發炎所致，表面上可能是細菌感染、黴菌感染、蟎蟲寄生，但更深層來看，是性荷爾蒙代謝不良、腸道菌叢失衡、胰島素太高、肝臟代謝受阻造成。12-24歲青少年盛行率80%，25歲以上青年也高達50%，因為此階段的睪固酮和雌激素分泌最多。熬夜、高醣飲食、加工食物（尤其是垃圾食物）、臉部衛生習慣不好或過度清潔，都會引起青春痘。所以，要徹底解決青春痘並不難，但需要探討自己到底是哪個環節出問題。",
     "type": "google_sheet",
     "sheet_id": "1H0NTLvF0oyURCw_YWBQJ8CkcL7pij5D_8zO_1gXMc5k",
     "sheet_name": "健康百科問答知識庫",
     "worksheet_name": "工作表1",
     "download_time": "2023-06-18T00:57:05.222819Z",
     "download_filepath": "./data/users/boh/bohachu_gmail_com/google_sheet_downloader/2023-06-18/doc-id_1H0NTLvF0oyURCw_YWBQJ8CkcL7pij5D_8zO_1gXMc5k_sha_0f813133.csv",
     "row": 13
-}
+}
+```
```

### Comparing `info-chunks-to-embeddings-1.0.0/info_chunks_to_embeddings.egg-info/PKG-INFO` & `info-chunks-to-embeddings-1.0.1/info_chunks_to_embeddings.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: info-chunks-to-embeddings
-Version: 1.0.0
+Version: 1.0.1
 Description-Content-Type: text/markdown
 
 # info_chunks_to_embeddings.py
 info_chunks_to_embeddings.py 是一個將 JSON 檔案轉換為語句嵌入的工具。它使用 SentenceTransformer 模型將 JSON 文件中的內容轉換為相應的語句嵌入，然後將這些嵌入保存到指定的資料夾中。
 
 ```
 🐔動機: 
@@ -20,16 +20,14 @@
   doc-id_1H0NTLvF0oyURCw_YWBQJ8CkcL7pij5D_8zO_1gXMc5k_sha_0f813133_row_7.json
   doc-id_1H0NTLvF0oyURCw_YWBQJ8CkcL7pij5D_8zO_1gXMc5k_sha_0f813133_row_7.pt
 
 💣地雷: 
 . 要注意 info_chunk.json 裡面必須包含有 content 欄位才能轉 embeddings .pt 檔案
 ```
 
-
-
 ## 安裝
 要安裝 info_chunks_to_embeddings，請使用以下命令：
 ```
 python3 -m pip install info-chunks-to-embeddings
 ```
 
 ## 使用方法
@@ -52,19 +50,21 @@
 ## 示例
 例如，如果您的 JSON 檔案位於 `~/my_json_files` 資料夾中，並希望將生成的嵌入存儲在 `~/my_embeddings` 資料夾中，則可以運行以下命令：
 ```
 python info_chunks_to_embeddings.py --input-folder ~/my_json_files --embeddings-folder ~/my_embeddings
 ```
 
 ## 輸入資料檔案 info_chunk.json 舉例（需要有 content 欄位）
+```
 {
     "uuid4": "f0dd55f0-229b-46d8-92af-e3c5e7275c52",
     "time": "2023-06-18T01:02:35.411700Z",
     "content": "青春痘 青春痘是最常見的皮膚問題，是皮脂腺發炎所致，表面上可能是細菌感染、黴菌感染、蟎蟲寄生，但更深層來看，是性荷爾蒙代謝不良、腸道菌叢失衡、胰島素太高、肝臟代謝受阻造成。12-24歲青少年盛行率80%，25歲以上青年也高達50%，因為此階段的睪固酮和雌激素分泌最多。熬夜、高醣飲食、加工食物（尤其是垃圾食物）、臉部衛生習慣不好或過度清潔，都會引起青春痘。所以，要徹底解決青春痘並不難，但需要探討自己到底是哪個環節出問題。",
     "type": "google_sheet",
     "sheet_id": "1H0NTLvF0oyURCw_YWBQJ8CkcL7pij5D_8zO_1gXMc5k",
     "sheet_name": "健康百科問答知識庫",
     "worksheet_name": "工作表1",
     "download_time": "2023-06-18T00:57:05.222819Z",
     "download_filepath": "./data/users/boh/bohachu_gmail_com/google_sheet_downloader/2023-06-18/doc-id_1H0NTLvF0oyURCw_YWBQJ8CkcL7pij5D_8zO_1gXMc5k_sha_0f813133.csv",
     "row": 13
 }
+```
```

### Comparing `info-chunks-to-embeddings-1.0.0/info_chunks_to_embeddings.py` & `info-chunks-to-embeddings-1.0.1/info_chunks_to_embeddings.py`

 * *Files identical despite different names*

### Comparing `info-chunks-to-embeddings-1.0.0/setup.py` & `info-chunks-to-embeddings-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="info-chunks-to-embeddings",
-    version="1.0.0",
+    version="1.0.1",
     packages=find_packages(),
     py_modules=['info_chunks_to_embeddings'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'info_chunks_to_embeddings = info_chunks_to_embeddings:main',
         ],
```

