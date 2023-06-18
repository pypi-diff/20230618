# Comparing `tmp/getmodelspec-1.0.389.tar.gz` & `tmp/getmodelspec-1.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\getmodelspec-1.0.389.tar", last modified: Sun Jun 18 00:02:34 2023, max compression
+gzip compressed data, was "dist\getmodelspec-1.0.39.tar", last modified: Sun Jun 18 03:39:41 2023, max compression
```

## Comparing `getmodelspec-1.0.389.tar` & `getmodelspec-1.0.39.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 00:02:34.000000 getmodelspec-1.0.389/
--rw-rw-rw-   0        0        0      351 2023-06-18 00:02:34.000000 getmodelspec-1.0.389/PKG-INFO
--rw-rw-rw-   0        0        0     3785 2023-06-13 15:33:43.000000 getmodelspec-1.0.389/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 00:02:34.000000 getmodelspec-1.0.389/getmodelspec/
--rw-rw-rw-   0        0        0      253 2023-06-12 12:36:25.000000 getmodelspec-1.0.389/getmodelspec/__init__.py
--rw-rw-rw-   0        0        0      778 2023-06-13 15:30:10.000000 getmodelspec-1.0.389/getmodelspec/lineup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 00:02:34.000000 getmodelspec-1.0.389/getmodelspec/src/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.389/getmodelspec/src/__init__.py
--rw-rw-rw-   0        0        0    11005 2023-06-18 00:01:42.000000 getmodelspec-1.0.389/getmodelspec/src/panasonic.py
--rw-rw-rw-   0        0        0    28581 2023-06-17 23:38:53.000000 getmodelspec-1.0.389/getmodelspec/src/sony.py
--rw-rw-rw-   0        0        0     1873 2023-06-17 23:37:55.000000 getmodelspec-1.0.389/getmodelspec/src/tv_score.py
--rw-rw-rw-   0        0        0     4277 2023-06-10 11:21:39.000000 getmodelspec-1.0.389/getmodelspec/src/tv_spepcifications.py
-drwxrwxrwx   0        0        0        0 2023-06-18 00:02:34.000000 getmodelspec-1.0.389/getmodelspec/tools/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.389/getmodelspec/tools/__init__.py
--rw-rw-rw-   0        0        0     2810 2023-06-14 15:20:39.000000 getmodelspec-1.0.389/getmodelspec/tools/functions.py
--rw-rw-rw-   0        0        0     5315 2023-06-17 15:03:46.000000 getmodelspec-1.0.389/getmodelspec/tools/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-06-18 00:02:34.000000 getmodelspec-1.0.389/getmodelspec.egg-info/
--rw-rw-rw-   0        0        0      351 2023-06-18 00:02:34.000000 getmodelspec-1.0.389/getmodelspec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      531 2023-06-18 00:02:34.000000 getmodelspec-1.0.389/getmodelspec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 00:02:34.000000 getmodelspec-1.0.389/getmodelspec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-18 00:02:34.000000 getmodelspec-1.0.389/getmodelspec.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2023-06-18 00:02:34.000000 getmodelspec-1.0.389/getmodelspec.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-18 00:02:34.000000 getmodelspec-1.0.389/getmodelspec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 00:02:34.000000 getmodelspec-1.0.389/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-06-18 00:02:22.000000 getmodelspec-1.0.389/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:39:41.000000 getmodelspec-1.0.39/
+-rw-rw-rw-   0        0        0      350 2023-06-18 03:39:41.000000 getmodelspec-1.0.39/PKG-INFO
+-rw-rw-rw-   0        0        0     3785 2023-06-13 15:33:43.000000 getmodelspec-1.0.39/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 03:39:41.000000 getmodelspec-1.0.39/getmodelspec/
+-rw-rw-rw-   0        0        0      253 2023-06-12 12:36:25.000000 getmodelspec-1.0.39/getmodelspec/__init__.py
+-rw-rw-rw-   0        0        0      778 2023-06-13 15:30:10.000000 getmodelspec-1.0.39/getmodelspec/lineup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:39:41.000000 getmodelspec-1.0.39/getmodelspec/src/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.39/getmodelspec/src/__init__.py
+-rw-rw-rw-   0        0        0    11001 2023-06-18 03:38:45.000000 getmodelspec-1.0.39/getmodelspec/src/panasonic.py
+-rw-rw-rw-   0        0        0    28852 2023-06-18 03:38:45.000000 getmodelspec-1.0.39/getmodelspec/src/sony.py
+-rw-rw-rw-   0        0        0     1873 2023-06-17 23:37:55.000000 getmodelspec-1.0.39/getmodelspec/src/tv_score.py
+-rw-rw-rw-   0        0        0     4277 2023-06-10 11:21:39.000000 getmodelspec-1.0.39/getmodelspec/src/tv_spepcifications.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:39:41.000000 getmodelspec-1.0.39/getmodelspec/tools/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.39/getmodelspec/tools/__init__.py
+-rw-rw-rw-   0        0        0     2810 2023-06-14 15:20:39.000000 getmodelspec-1.0.39/getmodelspec/tools/functions.py
+-rw-rw-rw-   0        0        0     5315 2023-06-17 15:03:46.000000 getmodelspec-1.0.39/getmodelspec/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:39:41.000000 getmodelspec-1.0.39/getmodelspec.egg-info/
+-rw-rw-rw-   0        0        0      350 2023-06-18 03:39:41.000000 getmodelspec-1.0.39/getmodelspec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      531 2023-06-18 03:39:41.000000 getmodelspec-1.0.39/getmodelspec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 03:39:41.000000 getmodelspec-1.0.39/getmodelspec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-18 03:39:41.000000 getmodelspec-1.0.39/getmodelspec.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2023-06-18 03:39:41.000000 getmodelspec-1.0.39/getmodelspec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-18 03:39:41.000000 getmodelspec-1.0.39/getmodelspec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 03:39:41.000000 getmodelspec-1.0.39/setup.cfg
+-rw-rw-rw-   0        0        0      810 2023-06-18 03:39:12.000000 getmodelspec-1.0.39/setup.py
```

### Comparing `getmodelspec-1.0.389/README.md` & `getmodelspec-1.0.39/README.md`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.389/getmodelspec/lineup.py` & `getmodelspec-1.0.39/getmodelspec/lineup.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.389/getmodelspec/src/panasonic.py` & `getmodelspec-1.0.39/getmodelspec/src/panasonic.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,18 +97,18 @@
         return results
 
 
     def __getSpecGlobal__(self, url: str) -> dict:
         # print("get", url)
         cntTryTotal = 20
         for cntTry in range(cntTryTotal):
+            model = getNamefromURL(url)
             try:
                 wd = WebDriver.getChrome()
                 wd.get(url=url)
-                model = getNamefromURL(url)
                 # dir_model = f"{self.dir_3rd}/{model}"
                 # makeDir(dir_model)
                 # wd.save_screenshot(f"./{dir_model}/{getNamefromURL(url)}_0_model_{get_today()}.png")  # 스크린 샷
 
                 # Selenium을 사용하여 페이지 소스 가져오기
                 page_source = wd.page_source
```

### Comparing `getmodelspec-1.0.389/getmodelspec/src/sony.py` & `getmodelspec-1.0.39/getmodelspec/src/sony.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,39 +59,43 @@
         # with open(f"dictUrlSeries.pickle", "rb") as file:
         #     dictUrlSeries = pickle.load(file)
         # ==========================================================================
     #     # 모델 정보 추출, 모델명/url/가격
         dictModels = {}
         score = Score()
         for key, urlModel in tqdm(dictUrlSeries.items()):
-            try:
-                dictInfo = self.__getModelInfo__(urlModel)
-                time.sleep(1)
-                dictModels[key] = dictInfo
-                model = dictInfo.get('model')
+            for i in range(5):
+                try:
+                    dictInfo = self.__getModelInfo__(urlModel)
+                    time.sleep(1)
+                    dictModels[key] = dictInfo
+                    model = dictInfo.get('model')
 
-                if self.fastMode == False:
-                    if self.srcfromGlobal == True:
-                        dictSpec = self.__getSpecGlobal__(url=urlModel)
-                        dictModels[key].update(dictSpec)
-                    else:
-                        print("global")
-                        dictSpec = self.__getSpec__(maker="sony", model=model)
-                        dictModels[key].update(dictSpec)
+                    if self.fastMode == False:
+                        if self.srcfromGlobal == True:
+                            dictSpec = self.__getSpecGlobal__(url=urlModel)
+                            dictModels[key].update(dictSpec)
+                        else:
+                            print("global")
+                            dictSpec = self.__getSpec__(maker="sony", model=model)
+                            dictModels[key].update(dictSpec)
 
-                time.sleep(1)
-                series = model.split("-")[1][2:]
-                dictScore = score.getRthinsScore(maker="sony", series=series)
-                if self.trackingLog == True:
-                    print(series,"score:", dictScore)
-                dictModels[key].update(dictScore)
-            except Exception as e:
-                print(f"fail to get info from {key}")
-                print(e)
-                pass
+                    time.sleep(1)
+                    series = model.split("-")[1][2:]
+                    dictScore = score.getRthinsScore(maker="sony", series=series)
+                    if self.trackingLog == True:
+                        print(series,"score:", dictScore)
+                    dictModels[key].update(dictScore)
+                    break
+                except Exception as e:
+                    print(f"fail to get info from {key}")
+                    print(f"try to get info from {key}_{i+1}/5")
+                    if self.trackingLog == True:
+                        print(e)
+                    pass
 
     # ======export====================================================================
         if self.toExcel == True:
             fileName = f"sony_LineUpGlobal_{date.today().strftime('%Y-%m-%d')}"
             dictToexcel(dictModels, fileName=fileName,sheetName="Global")  # 엑셀 파일로 저장
 
         return dictModels
```

### Comparing `getmodelspec-1.0.389/getmodelspec/src/tv_score.py` & `getmodelspec-1.0.39/getmodelspec/src/tv_score.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.389/getmodelspec/src/tv_spepcifications.py` & `getmodelspec-1.0.39/getmodelspec/src/tv_spepcifications.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.389/getmodelspec/tools/functions.py` & `getmodelspec-1.0.39/getmodelspec/tools/functions.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.389/getmodelspec/tools/webdriver.py` & `getmodelspec-1.0.39/getmodelspec/tools/webdriver.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.389/getmodelspec.egg-info/SOURCES.txt` & `getmodelspec-1.0.39/getmodelspec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.389/setup.py` & `getmodelspec-1.0.39/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='getmodelspec',
-    version='1.0.389',
+    version='1.0.39',
     author='xikest',
     description='get model spec,',
     packages=find_packages(),
     python_requires='>=3.7',
     install_requires=[
         'numpy',
         'pandas',
```

