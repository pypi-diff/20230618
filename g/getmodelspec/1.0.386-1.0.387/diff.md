# Comparing `tmp/getmodelspec-1.0.386.tar.gz` & `tmp/getmodelspec-1.0.387.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\getmodelspec-1.0.386.tar", last modified: Sat Jun 17 23:29:33 2023, max compression
+gzip compressed data, was "dist\getmodelspec-1.0.387.tar", last modified: Sat Jun 17 23:33:20 2023, max compression
```

## Comparing `getmodelspec-1.0.386.tar` & `getmodelspec-1.0.387.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 23:29:33.000000 getmodelspec-1.0.386/
--rw-rw-rw-   0        0        0      351 2023-06-17 23:29:33.000000 getmodelspec-1.0.386/PKG-INFO
--rw-rw-rw-   0        0        0     3785 2023-06-13 15:33:43.000000 getmodelspec-1.0.386/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 23:29:33.000000 getmodelspec-1.0.386/getmodelspec/
--rw-rw-rw-   0        0        0      253 2023-06-12 12:36:25.000000 getmodelspec-1.0.386/getmodelspec/__init__.py
--rw-rw-rw-   0        0        0      778 2023-06-13 15:30:10.000000 getmodelspec-1.0.386/getmodelspec/lineup.py
-drwxrwxrwx   0        0        0        0 2023-06-17 23:29:33.000000 getmodelspec-1.0.386/getmodelspec/src/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.386/getmodelspec/src/__init__.py
--rw-rw-rw-   0        0        0    11040 2023-06-17 15:28:00.000000 getmodelspec-1.0.386/getmodelspec/src/panasonic.py
--rw-rw-rw-   0        0        0    27921 2023-06-17 23:26:54.000000 getmodelspec-1.0.386/getmodelspec/src/sony.py
--rw-rw-rw-   0        0        0     1817 2023-06-12 11:30:21.000000 getmodelspec-1.0.386/getmodelspec/src/tv_score.py
--rw-rw-rw-   0        0        0     4277 2023-06-10 11:21:39.000000 getmodelspec-1.0.386/getmodelspec/src/tv_spepcifications.py
-drwxrwxrwx   0        0        0        0 2023-06-17 23:29:33.000000 getmodelspec-1.0.386/getmodelspec/tools/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.386/getmodelspec/tools/__init__.py
--rw-rw-rw-   0        0        0     2810 2023-06-14 15:20:39.000000 getmodelspec-1.0.386/getmodelspec/tools/functions.py
--rw-rw-rw-   0        0        0     5315 2023-06-17 15:03:46.000000 getmodelspec-1.0.386/getmodelspec/tools/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-06-17 23:29:33.000000 getmodelspec-1.0.386/getmodelspec.egg-info/
--rw-rw-rw-   0        0        0      351 2023-06-17 23:29:33.000000 getmodelspec-1.0.386/getmodelspec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      531 2023-06-17 23:29:33.000000 getmodelspec-1.0.386/getmodelspec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 23:29:33.000000 getmodelspec-1.0.386/getmodelspec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-17 23:29:33.000000 getmodelspec-1.0.386/getmodelspec.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2023-06-17 23:29:33.000000 getmodelspec-1.0.386/getmodelspec.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-17 23:29:33.000000 getmodelspec-1.0.386/getmodelspec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 23:29:33.000000 getmodelspec-1.0.386/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-06-17 23:29:20.000000 getmodelspec-1.0.386/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 23:33:20.000000 getmodelspec-1.0.387/
+-rw-rw-rw-   0        0        0      351 2023-06-17 23:33:20.000000 getmodelspec-1.0.387/PKG-INFO
+-rw-rw-rw-   0        0        0     3785 2023-06-13 15:33:43.000000 getmodelspec-1.0.387/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 23:33:20.000000 getmodelspec-1.0.387/getmodelspec/
+-rw-rw-rw-   0        0        0      253 2023-06-12 12:36:25.000000 getmodelspec-1.0.387/getmodelspec/__init__.py
+-rw-rw-rw-   0        0        0      778 2023-06-13 15:30:10.000000 getmodelspec-1.0.387/getmodelspec/lineup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 23:33:20.000000 getmodelspec-1.0.387/getmodelspec/src/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.387/getmodelspec/src/__init__.py
+-rw-rw-rw-   0        0        0    11040 2023-06-17 15:28:00.000000 getmodelspec-1.0.387/getmodelspec/src/panasonic.py
+-rw-rw-rw-   0        0        0    28415 2023-06-17 23:33:07.000000 getmodelspec-1.0.387/getmodelspec/src/sony.py
+-rw-rw-rw-   0        0        0     1817 2023-06-12 11:30:21.000000 getmodelspec-1.0.387/getmodelspec/src/tv_score.py
+-rw-rw-rw-   0        0        0     4277 2023-06-10 11:21:39.000000 getmodelspec-1.0.387/getmodelspec/src/tv_spepcifications.py
+drwxrwxrwx   0        0        0        0 2023-06-17 23:33:20.000000 getmodelspec-1.0.387/getmodelspec/tools/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.387/getmodelspec/tools/__init__.py
+-rw-rw-rw-   0        0        0     2810 2023-06-14 15:20:39.000000 getmodelspec-1.0.387/getmodelspec/tools/functions.py
+-rw-rw-rw-   0        0        0     5315 2023-06-17 15:03:46.000000 getmodelspec-1.0.387/getmodelspec/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-06-17 23:33:20.000000 getmodelspec-1.0.387/getmodelspec.egg-info/
+-rw-rw-rw-   0        0        0      351 2023-06-17 23:33:20.000000 getmodelspec-1.0.387/getmodelspec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      531 2023-06-17 23:33:20.000000 getmodelspec-1.0.387/getmodelspec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 23:33:20.000000 getmodelspec-1.0.387/getmodelspec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-17 23:33:20.000000 getmodelspec-1.0.387/getmodelspec.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2023-06-17 23:33:20.000000 getmodelspec-1.0.387/getmodelspec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-17 23:33:20.000000 getmodelspec-1.0.387/getmodelspec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 23:33:20.000000 getmodelspec-1.0.387/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-06-17 23:33:19.000000 getmodelspec-1.0.387/setup.py
```

### Comparing `getmodelspec-1.0.386/README.md` & `getmodelspec-1.0.387/README.md`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.386/getmodelspec/lineup.py` & `getmodelspec-1.0.387/getmodelspec/lineup.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.386/getmodelspec/src/panasonic.py` & `getmodelspec-1.0.387/getmodelspec/src/panasonic.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.386/getmodelspec/src/sony.py` & `getmodelspec-1.0.387/getmodelspec/src/sony.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,43 +17,47 @@
 from getmodelspec.src.tv_score import Score
 from getmodelspec.tools.functions import *
 from getmodelspec.tools.webdriver import WebDriver
 
 
 
 class GetSONY:
-    def __init__(self, fastMode=True, srcfromGlobal=True, toExcel=True):
+    def __init__(self, fastMode=True, srcfromGlobal=True, toExcel=True,trackingLog=False):
         self.waitTime = 10
         self.fastMode = fastMode
         self.srcfromGlobal = srcfromGlobal
         self.toExcel = toExcel
         self.dir_3rd = "sony/log/models"
-        # makeDir(self.dir_3rd)
+        self.trackingLog=trackingLog
+        if self.trackingLog == True:
+            makeDir(self.dir_3rd)
         pass
 
     def getModels(self, toExcel:bool = True) -> dict:
         # 메인 페이지에서 시리즈를 추출
         setUrlSeries = self.__getUrlSeries__()
         print(setUrlSeries)
         # ==========================================================================
-        # backUp(setUrlSeries, "setUrlSeries")
+        if self.trackingLog == True:
+            backUp(setUrlSeries, "setUrlSeries")
         # with open(f"setUrlSeries.pickle", "rb") as file:
         #     setUrlSeries = pickle.load(file)
         # # ==========================================================================
 
         ## 웹페이지의 모든 모델 url을 추출
         dictUrlSeries = {}
         for url in setUrlSeries:
             urlModels = self.__getModels__(url=url)
             print(urlModels)
             dictUrlSeries.update(urlModels)
         print("Number of all Series:", len(dictUrlSeries))
 
         # # # ==========================================================================
-        # backUp(dictUrlSeries, "dictUrlSeries")
+        if self.trackingLog == True:
+            backUp(dictUrlSeries, "dictUrlSeries")
         # with open(f"dictUrlSeries.pickle", "rb") as file:
         #     dictUrlSeries = pickle.load(file)
         # ==========================================================================
     #     # 모델 정보 추출, 모델명/url/가격
         dictModels = {}
         score = Score()
         for key, urlModel in tqdm(dictUrlSeries.items()):
@@ -197,55 +201,60 @@
                 dictSpec = {}
                 wd = WebDriver.getChrome()
                 wd.get(url=url)
 
                 model = getNamefromURL(url)
                 dir_model = f"{self.dir_3rd}/{model}"
                 makeDir(dir_model)
-
-                wd.save_screenshot(f"./{dir_model}/{getNamefromURL(url)}_0_model_{get_today()}.png")  # 스크린 샷
+                if self.trackingLog == True:
+                    wd.save_screenshot(f"./{dir_model}/{getNamefromURL(url)}_0_model_{get_today()}.png")  # 스크린 샷
 
                 elementSpec = wd.find_element(By.ID, "PDPSpecificationsLink")
                 wd = WebDriver.move_element_to_center(wd, elementSpec)
-                wd.save_screenshot(f"./{dir_model}/{getNamefromURL(url)}_1_move_to_spec_{get_today()}.png")  # 스크린 샷
+                if self.trackingLog == True:
+                    wd.save_screenshot(f"./{dir_model}/{getNamefromURL(url)}_1_move_to_spec_{get_today()}.png")  # 스크린 샷
 
                 waitingPage(self.waitTime)  # 페이지 로딩 대기 -
                 elementClickSpec = wd.find_element(By.ID, 'PDPSpecificationsLink')
                 elementClickSpec.click()
                 waitingPage(self.waitTime)  # 페이지 로딩 대기 -
-                wd.save_screenshot(
-                    f"./{dir_model}/{getNamefromURL(url)}_2_after_click_specification_{get_today()}.png")  # 스크린 샷
+                if self.trackingLog == True:
+                    wd.save_screenshot(
+                        f"./{dir_model}/{getNamefromURL(url)}_2_after_click_specification_{get_today()}.png")  # 스크린 샷
 
                 try:
                     element_seeMore = wd.find_element(By.XPATH,
                                                       '//*[@id="PDPOveriewLink"]/div[1]/div/div/div[2]/div/app-product-specification/div/div[2]/div[3]/button')
                     wd = WebDriver.move_element_to_center(wd, element_seeMore)
-                    wd.save_screenshot(
-                        f"./{dir_model}/{getNamefromURL(url)}_3_after_click_see_more_{get_today()}.png")  # 스크린 샷
+                    if self.trackingLog == True:
+                        wd.save_screenshot(
+                            f"./{dir_model}/{getNamefromURL(url)}_3_after_click_see_more_{get_today()}.png")  # 스크린 샷
                     element_seeMore.click()
                 except:
                     element_seeMore = wd.find_element(By.XPATH,
                                                       '//*[@id="PDPOveriewLink"]/div[1]/div/div/div[2]/div/app-product-specification/div/div[2]/div[2]/button')
                     wd = WebDriver.move_element_to_center(wd, element_seeMore)
-                    wd.save_screenshot(
-                        f"./{dir_model}/{getNamefromURL(url)}_3_after_click_see_more_{get_today()}.png")  # 스크린 샷
+                    if self.trackingLog == True:
+                        wd.save_screenshot(
+                            f"./{dir_model}/{getNamefromURL(url)}_3_after_click_see_more_{get_today()}.png")  # 스크린 샷
                     element_seeMore.click()
 
                 # 스펙 팝업 창의 스크롤 선택 후 클릭: 팝업 창으로 이동
                 time.sleep(self.waitTime)  # 페이지 로딩 대기 -
                 wd.find_element(By.ID, "ngb-nav-0-panel").click()
                 # 스펙 팝업 창의 스펙 가져오기
                 for cnt in range(15):
                     elements = wd.find_elements(By.CLASS_NAME,
                                                 "full-specifications__specifications-single-card__sub-list")
                     for element in elements:
                         soup = BeautifulSoup(element.get_attribute("innerHTML"), 'html.parser')
                         dictSpec.update(self.__soupToDict__(soup))
                     ActionChains(wd).key_down(Keys.PAGE_DOWN).perform()
-                wd.save_screenshot(f"./{dir_model}/{getNamefromURL(url)}_4_end_{get_today()}.png")  # 스크린 샷
+                if self.trackingLog == True:
+                    wd.save_screenshot(f"./{dir_model}/{getNamefromURL(url)}_4_end_{get_today()}.png")  # 스크린 샷
 
                 wd.quit()
                 print(f"{model}\n", dictSpec)
                 return dictSpec
 
             except Exception as e:
                 print(f"getPage3rd error: {model} try {cntTry + 1}/{cntTryTotal}")
```

### Comparing `getmodelspec-1.0.386/getmodelspec/src/tv_score.py` & `getmodelspec-1.0.387/getmodelspec/src/tv_score.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.386/getmodelspec/src/tv_spepcifications.py` & `getmodelspec-1.0.387/getmodelspec/src/tv_spepcifications.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.386/getmodelspec/tools/functions.py` & `getmodelspec-1.0.387/getmodelspec/tools/functions.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.386/getmodelspec/tools/webdriver.py` & `getmodelspec-1.0.387/getmodelspec/tools/webdriver.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.386/getmodelspec.egg-info/SOURCES.txt` & `getmodelspec-1.0.387/getmodelspec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.386/setup.py` & `getmodelspec-1.0.387/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='getmodelspec',
-    version='1.0.386',
+    version='1.0.387',
     author='xikest',
     description='get model spec,',
     packages=find_packages(),
     python_requires='>=3.7',
     install_requires=[
         'numpy',
         'pandas',
```

