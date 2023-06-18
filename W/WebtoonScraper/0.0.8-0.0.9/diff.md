# Comparing `tmp/WebtoonScraper-0.0.8.tar.gz` & `tmp/WebtoonScraper-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WebtoonScraper-0.0.8.tar", last modified: Wed May 17 14:19:18 2023, max compression
+gzip compressed data, was "WebtoonScraper-0.0.9.tar", last modified: Wed May 17 14:22:45 2023, max compression
```

## Comparing `WebtoonScraper-0.0.8.tar` & `WebtoonScraper-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 14:19:18.287351 WebtoonScraper-0.0.8/
--rw-rw-rw-   0        0        0     1089 2023-05-15 00:16:47.000000 WebtoonScraper-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       56 2023-05-17 13:57:54.000000 WebtoonScraper-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2134 2023-05-17 14:19:18.286342 WebtoonScraper-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1308 2023-05-15 00:37:37.000000 WebtoonScraper-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 14:19:18.271659 WebtoonScraper-0.0.8/WebtoonScraper/
--rw-rw-rw-   0        0        0      165 2023-05-17 14:15:41.000000 WebtoonScraper-0.0.8/WebtoonScraper/__init__.py
--rw-rw-rw-   0        0        0     9473 2023-05-17 13:49:27.000000 WebtoonScraper-0.0.8/WebtoonScraper/foldermanagement.py
--rw-rw-rw-   0        0        0      682 2023-05-17 13:42:15.000000 WebtoonScraper-0.0.8/WebtoonScraper/getsoup.py
--rw-rw-rw-   0        0        0    11320 2023-05-17 14:19:09.000000 WebtoonScraper-0.0.8/WebtoonScraper/scraper.py
-drwxrwxrwx   0        0        0        0 2023-05-17 14:19:18.284039 WebtoonScraper-0.0.8/WebtoonScraper.egg-info/
--rw-rw-rw-   0        0        0     2134 2023-05-17 14:19:18.000000 WebtoonScraper-0.0.8/WebtoonScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-05-17 14:19:18.000000 WebtoonScraper-0.0.8/WebtoonScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 14:19:18.000000 WebtoonScraper-0.0.8/WebtoonScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-17 14:16:38.000000 WebtoonScraper-0.0.8/WebtoonScraper.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2023-05-17 14:19:18.000000 WebtoonScraper-0.0.8/WebtoonScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-17 14:19:18.000000 WebtoonScraper-0.0.8/WebtoonScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    52914 2023-05-15 00:27:14.000000 WebtoonScraper-0.0.8/example1.png
--rw-rw-rw-   0        0        0       42 2023-05-17 14:19:18.287351 WebtoonScraper-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1326 2023-05-17 14:19:14.000000 WebtoonScraper-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 14:19:18.285301 WebtoonScraper-0.0.8/tests/
--rw-rw-rw-   0        0        0        0 2023-05-17 09:28:57.000000 WebtoonScraper-0.0.8/tests/__init__.py
--rw-rw-rw-   0        0        0      128 2023-05-16 14:18:05.000000 WebtoonScraper-0.0.8/tests/tests.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:22:45.187776 WebtoonScraper-0.0.9/
+-rw-rw-rw-   0        0        0     1089 2023-05-15 00:16:47.000000 WebtoonScraper-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       56 2023-05-17 13:57:54.000000 WebtoonScraper-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2134 2023-05-17 14:22:45.187776 WebtoonScraper-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1308 2023-05-15 00:37:37.000000 WebtoonScraper-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 14:22:45.166747 WebtoonScraper-0.0.9/WebtoonScraper/
+-rw-rw-rw-   0        0        0      165 2023-05-17 14:15:41.000000 WebtoonScraper-0.0.9/WebtoonScraper/__init__.py
+-rw-rw-rw-   0        0        0     9473 2023-05-17 13:49:27.000000 WebtoonScraper-0.0.9/WebtoonScraper/foldermanagement.py
+-rw-rw-rw-   0        0        0      682 2023-05-17 13:42:15.000000 WebtoonScraper-0.0.9/WebtoonScraper/getsoup.py
+-rw-rw-rw-   0        0        0    11337 2023-05-17 14:22:22.000000 WebtoonScraper-0.0.9/WebtoonScraper/scraper.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:22:45.184400 WebtoonScraper-0.0.9/WebtoonScraper.egg-info/
+-rw-rw-rw-   0        0        0     2134 2023-05-17 14:22:45.000000 WebtoonScraper-0.0.9/WebtoonScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-05-17 14:22:45.000000 WebtoonScraper-0.0.9/WebtoonScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 14:22:45.000000 WebtoonScraper-0.0.9/WebtoonScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-17 14:16:38.000000 WebtoonScraper-0.0.9/WebtoonScraper.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       18 2023-05-17 14:22:45.000000 WebtoonScraper-0.0.9/WebtoonScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-17 14:22:45.000000 WebtoonScraper-0.0.9/WebtoonScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    52914 2023-05-15 00:27:14.000000 WebtoonScraper-0.0.9/example1.png
+-rw-rw-rw-   0        0        0       42 2023-05-17 14:22:45.187776 WebtoonScraper-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1326 2023-05-17 14:22:40.000000 WebtoonScraper-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:22:45.186747 WebtoonScraper-0.0.9/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-17 09:28:57.000000 WebtoonScraper-0.0.9/tests/__init__.py
+-rw-rw-rw-   0        0        0      128 2023-05-16 14:18:05.000000 WebtoonScraper-0.0.9/tests/tests.py
```

### Comparing `WebtoonScraper-0.0.8/LICENSE` & `WebtoonScraper-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.0.8/PKG-INFO` & `WebtoonScraper-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebtoonScraper
-Version: 0.0.8
+Version: 0.0.9
 Summary: Scraping webtoons and some utils for it
 Home-page: https://github.com/ilotoki0804/WebtoonScraper
 Author: ilotoki0804
 Author-email: ilotoki0804@gmail.com
 License: MIT
 Keywords: Webtoon,Webtoon Scraper,Never Webtoon,Webtoon Downloader,Download Webtoon
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `WebtoonScraper-0.0.8/README.md` & `WebtoonScraper-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.0.8/WebtoonScraper/foldermanagement.py` & `WebtoonScraper-0.0.9/WebtoonScraper/foldermanagement.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.0.8/WebtoonScraper/getsoup.py` & `WebtoonScraper-0.0.9/WebtoonScraper/getsoup.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.0.8/WebtoonScraper/scraper.py` & `WebtoonScraper-0.0.9/WebtoonScraper/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         self.user_agent = {'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36'}
         self.table = str.maketrans('\\/:*?"<>|\t', '⧵／：＊？＂＜＞∣  ') # for translate filename for forbidden charactor.
         self.loop = asyncio.get_event_loop() # for loop.run_in_executor()
         self.root = 'webtoon'
 
     def get_webtoons(self, *webtoons):
         '''Run crawler in sync function'''
-        asyncio.run(self.get_webtoons_async(*webtoons))
+        self.loop.run_until_complete(self.get_webtoons_async(*webtoons))
 
     async def get_webtoons_async(self, *webtoons):
         '''Get webtoons automatically.\n
         If you want to download webtoon 766648, type like 'get_webtoons_async(76648)'.\n
         If you want to download some part of webtoon, type like 'get_webtoons_async({titleid:76648, range:(1,20)}).\n
         You can use keyword argument down below.\n
             titleid(Required) : webtoon you want to download. int or str required.\n
```

### Comparing `WebtoonScraper-0.0.8/WebtoonScraper.egg-info/PKG-INFO` & `WebtoonScraper-0.0.9/WebtoonScraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebtoonScraper
-Version: 0.0.8
+Version: 0.0.9
 Summary: Scraping webtoons and some utils for it
 Home-page: https://github.com/ilotoki0804/WebtoonScraper
 Author: ilotoki0804
 Author-email: ilotoki0804@gmail.com
 License: MIT
 Keywords: Webtoon,Webtoon Scraper,Never Webtoon,Webtoon Downloader,Download Webtoon
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `WebtoonScraper-0.0.8/example1.png` & `WebtoonScraper-0.0.9/example1.png`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.0.8/setup.py` & `WebtoonScraper-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # long_description = (this_directory / "README.md").read_text()
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='WebtoonScraper',
-    version='0.0.8',
+    version='0.0.9',
     description='Scraping webtoons and some utils for it',
     author='ilotoki0804',
     author_email='ilotoki0804@gmail.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/ilotoki0804/WebtoonScraper',
```

