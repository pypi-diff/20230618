# Comparing `tmp/BlizzardWarcraftAPI-0.1.0.tar.gz` & `tmp/BlizzardWarcraftAPI-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlizzardWarcraftAPI-0.1.0.tar", last modified: Tue Jun 13 22:22:03 2023, max compression
+gzip compressed data, was "BlizzardWarcraftAPI-0.1.1.tar", last modified: Sun Jun 18 11:43:46 2023, max compression
```

## Comparing `BlizzardWarcraftAPI-0.1.0.tar` & `BlizzardWarcraftAPI-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:22:03.308914 BlizzardWarcraftAPI-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:22:03.304914 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI/
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-13 22:21:30.000000 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI/BlizzardAuthToken.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-13 22:21:30.000000 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI/BlizzardWarcraftAPI.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-13 22:21:30.000000 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-13 22:21:30.000000 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-13 22:21:30.000000 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:22:03.308914 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-13 22:21:30.000000 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI/modules/AchievementAPI.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-13 22:21:30.000000 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI/modules/BlizzardWarcraftAPI_base.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-13 22:21:30.000000 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-13 22:21:30.000000 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:22:03.308914 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-13 22:22:03.000000 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-13 22:22:03.000000 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 22:22:03.000000 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 22:22:03.000000 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-13 22:22:03.000000 BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-13 22:21:30.000000 BlizzardWarcraftAPI-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-13 22:22:03.308914 BlizzardWarcraftAPI-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-13 22:21:30.000000 BlizzardWarcraftAPI-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-13 22:21:30.000000 BlizzardWarcraftAPI-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 22:22:03.308914 BlizzardWarcraftAPI-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:22:03.308914 BlizzardWarcraftAPI-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-13 22:21:30.000000 BlizzardWarcraftAPI-0.1.0/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:43:46.961266 BlizzardWarcraftAPI-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:43:46.961266 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/BlizzardAuthToken.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/BlizzardWarcraftAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:43:46.961266 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/modules/AchievementAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/modules/AuctionHouseAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/modules/BlizzardWarcraftAPI_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/modules/CharacterAchievementsAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/modules/CharacterAppearanceAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/modules/ConnectedRealmAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:43:46.961266 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-18 11:43:46.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-18 11:43:46.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 11:43:46.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-18 11:43:46.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-18 11:43:46.000000 BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-18 11:43:46.961266 BlizzardWarcraftAPI-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 11:43:46.961266 BlizzardWarcraftAPI-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:43:46.961266 BlizzardWarcraftAPI-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-18 11:43:22.000000 BlizzardWarcraftAPI-0.1.1/tests/test_base.py
```

### Comparing `BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI/BlizzardAuthToken.py` & `BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/BlizzardAuthToken.py`

 * *Files identical despite different names*

### Comparing `BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI/data.py` & `BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/data.py`

 * *Files identical despite different names*

### Comparing `BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI/modules/BlizzardWarcraftAPI_base.py` & `BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI/modules/BlizzardWarcraftAPI_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import requests
 from ..data import region_data, locales_region_data
 from ..exceptions import BlizzardWarcraftApiError
 from ..urls import URL_TOKEN_VALIDATION
 
 
 class BlizzardWarcraftAPI():
+    @staticmethod
+    def response(url, param):
+        resp = requests.get(url, params=param)
+        return resp.json()
 
     @staticmethod
     def __valid_region(region):
         if region in region_data:
             return True
         else:
             text = f"Region must be: {region_data}"
@@ -49,7 +53,12 @@
 
         if self.__valid_locale(self.region, locale):
             self.locale = locale
 
         self.namespace_profile = "profile-" + self.region
         self.namespace_static = "static-" + self.region
         self.namespace_dynamic = "dynamic-" + self.region
+
+        self.param = {
+            "locale": self.locale,
+            "access_token": self.BlizzardAuthToken
+        }
```

### Comparing `BlizzardWarcraftAPI-0.1.0/BlizzardWarcraftAPI.egg-info/PKG-INFO` & `BlizzardWarcraftAPI-0.1.1/BlizzardWarcraftAPI.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BlizzardWarcraftAPI
-Version: 0.1.0
+Version: 0.1.1
 Summary: Warcraft API
 Author-email: Angeloffy <angeloffy.work@gmail.com>
 Project-URL: Homepage, https://github.com/Angeloffy/BlizzardWarcraftAPI/tree/main
 Project-URL: Bug Tracker, https://github.com/Angeloffy/BlizzardWarcraftAPI/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,16 +25,29 @@
 # Installing
 Install and update using <a href="https://pip.pypa.io/en/stable/getting-started/">pip</a>:
 ```shell
 pip install BlizzardWarcraftAPI
 ```
 
 # A Simple Example
+
 ```python
 from BlizzardWarcraftAPI import BlizzardWarcraftAPI, BlizzardAuthToken
 
-
 token = BlizzardAuthToken("ClientID", "ClientSecret").get()
 
 warcraft = BlizzardWarcraftAPI(token, region, locale)
-warcraft.get_AchievementCategoriesIndex()
+warcraft.get_AchievementCategoriesIndex
 ```
+
+# [APIs](https://develop.battle.net/documentation/world-of-warcraft)
+
+## [Game Data](https://develop.battle.net/documentation/world-of-warcraft/game-data-apis)
+
+- [x] Achievement
+- [x] Auction House
+- [x] Connected Realm
+
+## [Profile](https://develop.battle.net/documentation/world-of-warcraft/profile-apis)
+
+- [x] Character Achievements
+- [x] Character Appearance
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BlizzardWarcraftAPI Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: BlizzardWarcraftAPI Version: 0.1.1 Summary:
 Warcraft API Author-email: Angeloffy
 work@gmail.com> Project-URL: Homepage, https://github.com/Angeloffy/
 BlizzardWarcraftAPI/tree/main Project-URL: Bug Tracker, https://github.com/
 Angeloffy/BlizzardWarcraftAPI/issues Classifier: Programming Language :: Python
 :: 3.9 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
 markdown License-File: LICENSE # BlizzardWarcraftAPI ![image](https://
@@ -23,8 +23,13 @@
 capabilities and improve its usability. Developers interested in utilizing the
 vast resources offered by the World of Warcraft API will find
 BlizzardWarcraftAPI to be a valuable tool in their projects. # Installing
 Install and update using pip: ```shell pip install BlizzardWarcraftAPI ``` # A
 Simple Example ```python from BlizzardWarcraftAPI import BlizzardWarcraftAPI,
 BlizzardAuthToken token = BlizzardAuthToken("ClientID", "ClientSecret").get()
 warcraft = BlizzardWarcraftAPI(token, region, locale)
-warcraft.get_AchievementCategoriesIndex() ```
+warcraft.get_AchievementCategoriesIndex ``` # [APIs](https://
+develop.battle.net/documentation/world-of-warcraft) ## [Game Data](https://
+develop.battle.net/documentation/world-of-warcraft/game-data-apis) - [x]
+Achievement - [x] Auction House - [x] Connected Realm ## [Profile](https://
+develop.battle.net/documentation/world-of-warcraft/profile-apis) - [x]
+Character Achievements - [x] Character Appearance
```

### Comparing `BlizzardWarcraftAPI-0.1.0/LICENSE` & `BlizzardWarcraftAPI-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `BlizzardWarcraftAPI-0.1.0/PKG-INFO` & `BlizzardWarcraftAPI-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BlizzardWarcraftAPI
-Version: 0.1.0
+Version: 0.1.1
 Summary: Warcraft API
 Author-email: Angeloffy <angeloffy.work@gmail.com>
 Project-URL: Homepage, https://github.com/Angeloffy/BlizzardWarcraftAPI/tree/main
 Project-URL: Bug Tracker, https://github.com/Angeloffy/BlizzardWarcraftAPI/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,16 +25,29 @@
 # Installing
 Install and update using <a href="https://pip.pypa.io/en/stable/getting-started/">pip</a>:
 ```shell
 pip install BlizzardWarcraftAPI
 ```
 
 # A Simple Example
+
 ```python
 from BlizzardWarcraftAPI import BlizzardWarcraftAPI, BlizzardAuthToken
 
-
 token = BlizzardAuthToken("ClientID", "ClientSecret").get()
 
 warcraft = BlizzardWarcraftAPI(token, region, locale)
-warcraft.get_AchievementCategoriesIndex()
+warcraft.get_AchievementCategoriesIndex
 ```
+
+# [APIs](https://develop.battle.net/documentation/world-of-warcraft)
+
+## [Game Data](https://develop.battle.net/documentation/world-of-warcraft/game-data-apis)
+
+- [x] Achievement
+- [x] Auction House
+- [x] Connected Realm
+
+## [Profile](https://develop.battle.net/documentation/world-of-warcraft/profile-apis)
+
+- [x] Character Achievements
+- [x] Character Appearance
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BlizzardWarcraftAPI Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: BlizzardWarcraftAPI Version: 0.1.1 Summary:
 Warcraft API Author-email: Angeloffy
 work@gmail.com> Project-URL: Homepage, https://github.com/Angeloffy/
 BlizzardWarcraftAPI/tree/main Project-URL: Bug Tracker, https://github.com/
 Angeloffy/BlizzardWarcraftAPI/issues Classifier: Programming Language :: Python
 :: 3.9 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
 markdown License-File: LICENSE # BlizzardWarcraftAPI ![image](https://
@@ -23,8 +23,13 @@
 capabilities and improve its usability. Developers interested in utilizing the
 vast resources offered by the World of Warcraft API will find
 BlizzardWarcraftAPI to be a valuable tool in their projects. # Installing
 Install and update using pip: ```shell pip install BlizzardWarcraftAPI ``` # A
 Simple Example ```python from BlizzardWarcraftAPI import BlizzardWarcraftAPI,
 BlizzardAuthToken token = BlizzardAuthToken("ClientID", "ClientSecret").get()
 warcraft = BlizzardWarcraftAPI(token, region, locale)
-warcraft.get_AchievementCategoriesIndex() ```
+warcraft.get_AchievementCategoriesIndex ``` # [APIs](https://
+develop.battle.net/documentation/world-of-warcraft) ## [Game Data](https://
+develop.battle.net/documentation/world-of-warcraft/game-data-apis) - [x]
+Achievement - [x] Auction House - [x] Connected Realm ## [Profile](https://
+develop.battle.net/documentation/world-of-warcraft/profile-apis) - [x]
+Character Achievements - [x] Character Appearance
```

### Comparing `BlizzardWarcraftAPI-0.1.0/README.md` & `BlizzardWarcraftAPI-0.1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -11,16 +11,29 @@
 # Installing
 Install and update using <a href="https://pip.pypa.io/en/stable/getting-started/">pip</a>:
 ```shell
 pip install BlizzardWarcraftAPI
 ```
 
 # A Simple Example
+
 ```python
 from BlizzardWarcraftAPI import BlizzardWarcraftAPI, BlizzardAuthToken
 
-
 token = BlizzardAuthToken("ClientID", "ClientSecret").get()
 
 warcraft = BlizzardWarcraftAPI(token, region, locale)
-warcraft.get_AchievementCategoriesIndex()
-```
+warcraft.get_AchievementCategoriesIndex
+```
+
+# [APIs](https://develop.battle.net/documentation/world-of-warcraft)
+
+## [Game Data](https://develop.battle.net/documentation/world-of-warcraft/game-data-apis)
+
+- [x] Achievement
+- [x] Auction House
+- [x] Connected Realm
+
+## [Profile](https://develop.battle.net/documentation/world-of-warcraft/profile-apis)
+
+- [x] Character Achievements
+- [x] Character Appearance
```

#### html2text {}

```diff
@@ -16,8 +16,13 @@
 its usability. Developers interested in utilizing the vast resources offered by
 the World of Warcraft API will find BlizzardWarcraftAPI to be a valuable tool
 in their projects. # Installing Install and update using pip: ```shell pip
 install BlizzardWarcraftAPI ``` # A Simple Example ```python from
 BlizzardWarcraftAPI import BlizzardWarcraftAPI, BlizzardAuthToken token =
 BlizzardAuthToken("ClientID", "ClientSecret").get() warcraft =
 BlizzardWarcraftAPI(token, region, locale)
-warcraft.get_AchievementCategoriesIndex() ```
+warcraft.get_AchievementCategoriesIndex ``` # [APIs](https://
+develop.battle.net/documentation/world-of-warcraft) ## [Game Data](https://
+develop.battle.net/documentation/world-of-warcraft/game-data-apis) - [x]
+Achievement - [x] Auction House - [x] Connected Realm ## [Profile](https://
+develop.battle.net/documentation/world-of-warcraft/profile-apis) - [x]
+Character Achievements - [x] Character Appearance
```

### Comparing `BlizzardWarcraftAPI-0.1.0/pyproject.toml` & `BlizzardWarcraftAPI-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "BlizzardWarcraftAPI"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     {name = "Angeloffy", email = "angeloffy.work@gmail.com"},
 ]
 description = "Warcraft API"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

