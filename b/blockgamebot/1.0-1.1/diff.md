# Comparing `tmp/blockgamebot-1.0.tar.gz` & `tmp/blockgamebot-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockgamebot-1.0.tar", last modified: Sun May  7 14:12:04 2023, max compression
+gzip compressed data, was "blockgamebot-1.1.tar", last modified: Sun Jun 18 08:30:35 2023, max compression
```

## Comparing `blockgamebot-1.0.tar` & `blockgamebot-1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 14:12:04.470330 blockgamebot-1.0/
--rw-rw-rw-   0        0        0     1086 2023-05-07 14:09:59.000000 blockgamebot-1.0/LICENSE
--rw-rw-rw-   0        0        0     1976 2023-05-07 14:12:04.469333 blockgamebot-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1362 2023-05-07 14:09:59.000000 blockgamebot-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 14:12:04.443401 blockgamebot-1.0/blockgamebot/
--rw-rw-rw-   0        0        0       37 2023-05-07 14:09:59.000000 blockgamebot-1.0/blockgamebot/__init__.py
--rw-rw-rw-   0        0        0     1788 2023-05-07 14:09:59.000000 blockgamebot-1.0/blockgamebot/api.py
-drwxrwxrwx   0        0        0        0 2023-05-07 14:12:04.468334 blockgamebot-1.0/blockgamebot.egg-info/
--rw-rw-rw-   0        0        0     1976 2023-05-07 14:12:04.000000 blockgamebot-1.0/blockgamebot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-05-07 14:12:04.000000 blockgamebot-1.0/blockgamebot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 14:12:04.000000 blockgamebot-1.0/blockgamebot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-07 14:12:04.000000 blockgamebot-1.0/blockgamebot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-07 14:12:04.000000 blockgamebot-1.0/blockgamebot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      698 2023-05-07 14:11:48.000000 blockgamebot-1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-07 14:12:04.470330 blockgamebot-1.0/setup.cfg
--rw-rw-rw-   0        0        0      879 2023-05-07 14:09:59.000000 blockgamebot-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 08:30:35.649896 blockgamebot-1.1/
+-rw-rw-rw-   0        0        0     1086 2023-06-18 08:25:07.000000 blockgamebot-1.1/LICENSE
+-rw-rw-rw-   0        0        0     1983 2023-06-18 08:30:35.649896 blockgamebot-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1369 2023-06-18 08:25:07.000000 blockgamebot-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 08:30:35.636932 blockgamebot-1.1/blockgamebot/
+-rw-rw-rw-   0        0        0       37 2023-06-18 08:25:07.000000 blockgamebot-1.1/blockgamebot/__init__.py
+-rw-rw-rw-   0        0        0     2407 2023-06-18 08:25:07.000000 blockgamebot-1.1/blockgamebot/api.py
+drwxrwxrwx   0        0        0        0 2023-06-18 08:30:35.648899 blockgamebot-1.1/blockgamebot.egg-info/
+-rw-rw-rw-   0        0        0     1983 2023-06-18 08:30:35.000000 blockgamebot-1.1/blockgamebot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-06-18 08:30:35.000000 blockgamebot-1.1/blockgamebot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 08:30:35.000000 blockgamebot-1.1/blockgamebot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-18 08:30:35.000000 blockgamebot-1.1/blockgamebot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-18 08:30:35.000000 blockgamebot-1.1/blockgamebot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      698 2023-06-18 08:27:52.000000 blockgamebot-1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-18 08:30:35.650894 blockgamebot-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      879 2023-06-18 08:29:47.000000 blockgamebot-1.1/setup.py
```

### Comparing `blockgamebot-1.0/LICENSE` & `blockgamebot-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blockgamebot-1.0/PKG-INFO` & `blockgamebot-1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockgamebot
-Version: 1.0
+Version: 1.1
 Summary: An API Wrapper for the block game bot api
 Author: asov
 Author-email: asov <noemtdev@gmail.com>
 Project-URL: Homepage, https://github.com/noemtdev/api-wrapper
 Project-URL: Bug Tracker, https://github.com/noemtdev/api-wrapper/issues
 Keywords: python,hypixel,skyblock,scammerlist,blockgamebot,blockgamebot
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # block game bot
 
 [![license](https://img.shields.io/badge/license-MIT-green?style=for-the-badge)](LICENSE)
-[![pypi](https://img.shields.io/pypi/v/lilyweight?style=for-the-badge)](https://pypi.org/project/lilyweight/)
+[![pypi](https://img.shields.io/pypi/v/blockgamebot?style=for-the-badge)](https://pypi.org/project/blockgamebot/)
 
 block game bot api Wrapper
 
 ## Information
 
 Written without any external libraries other than `aiohttp` which is used to fetch data from the block game bot API.
 
@@ -49,15 +49,15 @@
     print(all_scammers)
 
     # Lookup a scammer
     scammer = await scammers.lookup("asov")
     print(scammer)
 
     # Get an item image
-    url = await images.get_image("bread", variation="enchanted") 
+    url = await images.get_image("hyperion", variation="enchanted") 
     # variation defaults to "normal" but it can also be "enchanted"
 
     print(url)
 
 
 asyncio.run(main())
 ```
```

### Comparing `blockgamebot-1.0/README.md` & `blockgamebot-1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # block game bot
 
 [![license](https://img.shields.io/badge/license-MIT-green?style=for-the-badge)](LICENSE)
-[![pypi](https://img.shields.io/pypi/v/lilyweight?style=for-the-badge)](https://pypi.org/project/lilyweight/)
+[![pypi](https://img.shields.io/pypi/v/blockgamebot?style=for-the-badge)](https://pypi.org/project/blockgamebot/)
 
 block game bot api Wrapper
 
 ## Information
 
 Written without any external libraries other than `aiohttp` which is used to fetch data from the block game bot API.
 
@@ -33,15 +33,15 @@
     print(all_scammers)
 
     # Lookup a scammer
     scammer = await scammers.lookup("asov")
     print(scammer)
 
     # Get an item image
-    url = await images.get_image("bread", variation="enchanted") 
+    url = await images.get_image("hyperion", variation="enchanted") 
     # variation defaults to "normal" but it can also be "enchanted"
 
     print(url)
 
 
 asyncio.run(main())
 ```
```

### Comparing `blockgamebot-1.0/blockgamebot/api.py` & `blockgamebot-1.1/blockgamebot/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,51 +9,73 @@
         self.urls = {
             "all": f"https://api.nom-nom.link/scammers?key={self.key}",
             "lookup": f"https://api.nom-nom.link/lookup/scammer/ARGUMENTS?key={self.key}",
         }
 
     
     async def get_all(self):
+        close = False
 
         if self.session is None:
+            close = True
             self.session = aiohttp.ClientSession()
         
         async with self.session.get(self.urls["all"]) as resp:
+            
+            if close is True:
+                await self.session.close()
+                
             return await resp.json()
         
     
     async def lookup(self, argument):
+        close = False
 
         if self.session is None:
+            close = True
             self.session = aiohttp.ClientSession()
             
         async with self.session.get(self.urls["lookup"].replace("ARGUMENTS", argument)) as resp:
+            
+            if close is True:
+                await self.session.close()
+                
             return await resp.json()
 
 class itemImages:
     def __init__(self, session:aiohttp.ClientSession=None):
 
         self.session = session
         self.urls = {
             "base": "https://api.nom-nom.link/skyblock/items/{variation}/{item}/"
         }
 
         self.variations = ["normal", "enchanted"]
 
 
     async def get_image(self, item:str, variation="normal"):
-
-        if self.session is None:
-            self.session = aiohttp.ClientSession()
-
+        close = False
+        
         if variation.lower() not in self.variations:
             raise ValueError(f"Variation must be one of the following: {self.variations}")
+            
+        if self.session is None:
+            close = True
+            self.session = aiohttp.ClientSession()
         
         url = self.urls["base"].replace("{variation}", variation).replace("{item}", item.upper())
         async with self.session.get(url) as resp:
+            
             if resp.status == 404:
+                
+                if close is True:
+                    await self.session.close()
+                    
                 raise ValueError(f"Item not found")
             
+            if close is True:
+                    await self.session.close()
+                    
             return url
```

### Comparing `blockgamebot-1.0/blockgamebot.egg-info/PKG-INFO` & `blockgamebot-1.1/blockgamebot.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockgamebot
-Version: 1.0
+Version: 1.1
 Summary: An API Wrapper for the block game bot api
 Author: asov
 Author-email: asov <noemtdev@gmail.com>
 Project-URL: Homepage, https://github.com/noemtdev/api-wrapper
 Project-URL: Bug Tracker, https://github.com/noemtdev/api-wrapper/issues
 Keywords: python,hypixel,skyblock,scammerlist,blockgamebot,blockgamebot
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # block game bot
 
 [![license](https://img.shields.io/badge/license-MIT-green?style=for-the-badge)](LICENSE)
-[![pypi](https://img.shields.io/pypi/v/lilyweight?style=for-the-badge)](https://pypi.org/project/lilyweight/)
+[![pypi](https://img.shields.io/pypi/v/blockgamebot?style=for-the-badge)](https://pypi.org/project/blockgamebot/)
 
 block game bot api Wrapper
 
 ## Information
 
 Written without any external libraries other than `aiohttp` which is used to fetch data from the block game bot API.
 
@@ -49,15 +49,15 @@
     print(all_scammers)
 
     # Lookup a scammer
     scammer = await scammers.lookup("asov")
     print(scammer)
 
     # Get an item image
-    url = await images.get_image("bread", variation="enchanted") 
+    url = await images.get_image("hyperion", variation="enchanted") 
     # variation defaults to "normal" but it can also be "enchanted"
 
     print(url)
 
 
 asyncio.run(main())
 ```
```

### Comparing `blockgamebot-1.0/pyproject.toml` & `blockgamebot-1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "blockgamebot"
-version = "1.0"
+version = "1.1"
 authors = [
   { name="asov", email="noemtdev@gmail.com" },
 ]
 description = "An API Wrapper for the block game bot api"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `blockgamebot-1.0/setup.py` & `blockgamebot-1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0'
+VERSION = '1.1'
 DESCRIPTION = 'Hypixel SkyBlock Scammer List Package'
 
 # Setting up
 setup(
     name="blockgamebot",
     version=VERSION,
     author="asov",
```

