# Comparing `tmp/fgo_api_types-2023.6.7.4.47.40.tar.gz` & `tmp/fgo_api_types-2023.6.8.15.39.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgo_api_types-2023.6.7.4.47.40.tar", max compression
+gzip compressed data, was "fgo_api_types-2023.6.8.15.39.7.tar", max compression
```

## Comparing `fgo_api_types-2023.6.7.4.47.40.tar` & `fgo_api_types-2023.6.8.15.39.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34523 2023-06-07 04:47:20.334114 fgo_api_types-2023.6.7.4.47.40/LICENSE
--rw-r--r--   0        0        0      449 2023-06-07 04:47:20.334114 fgo_api_types-2023.6.7.4.47.40/README.md
--rw-r--r--   0        0        0        0 2023-06-07 04:47:40.502153 fgo_api_types-2023.6.7.4.47.40/fgo_api_types/__init__.py
--rw-r--r--   0        0        0      434 2023-06-07 04:47:40.502153 fgo_api_types-2023.6.7.4.47.40/fgo_api_types/base.py
--rw-r--r--   0        0        0     4195 2023-06-07 04:47:40.502153 fgo_api_types-2023.6.7.4.47.40/fgo_api_types/basic.py
--rw-r--r--   0        0        0     3631 2023-06-07 04:47:40.502153 fgo_api_types-2023.6.7.4.47.40/fgo_api_types/common.py
--rw-r--r--   0        0        0    38038 2023-06-07 04:47:40.502153 fgo_api_types-2023.6.7.4.47.40/fgo_api_types/enums.py
--rw-r--r--   0        0        0   158848 2023-06-07 04:47:40.502153 fgo_api_types-2023.6.7.4.47.40/fgo_api_types/gameenums.py
--rw-r--r--   0        0        0    76421 2023-06-07 04:47:40.502153 fgo_api_types-2023.6.7.4.47.40/fgo_api_types/nice.py
--rw-r--r--   0        0        0    50619 2023-06-07 04:47:40.502153 fgo_api_types-2023.6.7.4.47.40/fgo_api_types/raw.py
--rw-r--r--   0        0        0     4176 2023-06-07 04:47:40.502153 fgo_api_types-2023.6.7.4.47.40/fgo_api_types/rayshift.py
--rw-r--r--   0        0        0    18670 2023-06-07 04:47:40.502153 fgo_api_types-2023.6.7.4.47.40/fgo_api_types/search.py
--rw-r--r--   0        0        0      520 2023-06-07 04:47:40.826154 fgo_api_types-2023.6.7.4.47.40/pyproject.toml
--rw-r--r--   0        0        0     1221 1970-01-01 00:00:00.000000 fgo_api_types-2023.6.7.4.47.40/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-08 15:38:35.602324 fgo_api_types-2023.6.8.15.39.7/LICENSE
+-rw-r--r--   0        0        0      449 2023-06-08 15:38:35.602324 fgo_api_types-2023.6.8.15.39.7/README.md
+-rw-r--r--   0        0        0        0 2023-06-08 15:39:07.010581 fgo_api_types-2023.6.8.15.39.7/fgo_api_types/__init__.py
+-rw-r--r--   0        0        0      434 2023-06-08 15:39:07.010581 fgo_api_types-2023.6.8.15.39.7/fgo_api_types/base.py
+-rw-r--r--   0        0        0     4195 2023-06-08 15:39:07.010581 fgo_api_types-2023.6.8.15.39.7/fgo_api_types/basic.py
+-rw-r--r--   0        0        0     3631 2023-06-08 15:39:07.010581 fgo_api_types-2023.6.8.15.39.7/fgo_api_types/common.py
+-rw-r--r--   0        0        0    38038 2023-06-08 15:39:07.010581 fgo_api_types-2023.6.8.15.39.7/fgo_api_types/enums.py
+-rw-r--r--   0        0        0   158848 2023-06-08 15:39:07.010581 fgo_api_types-2023.6.8.15.39.7/fgo_api_types/gameenums.py
+-rw-r--r--   0        0        0    76474 2023-06-08 15:39:07.010581 fgo_api_types-2023.6.8.15.39.7/fgo_api_types/nice.py
+-rw-r--r--   0        0        0    50915 2023-06-08 15:39:07.010581 fgo_api_types-2023.6.8.15.39.7/fgo_api_types/raw.py
+-rw-r--r--   0        0        0     4176 2023-06-08 15:39:07.010581 fgo_api_types-2023.6.8.15.39.7/fgo_api_types/rayshift.py
+-rw-r--r--   0        0        0    18670 2023-06-08 15:39:07.010581 fgo_api_types-2023.6.8.15.39.7/fgo_api_types/search.py
+-rw-r--r--   0        0        0      520 2023-06-08 15:39:07.426585 fgo_api_types-2023.6.8.15.39.7/pyproject.toml
+-rw-r--r--   0        0        0     1221 1970-01-01 00:00:00.000000 fgo_api_types-2023.6.8.15.39.7/PKG-INFO
```

### Comparing `fgo_api_types-2023.6.7.4.47.40/LICENSE` & `fgo_api_types-2023.6.8.15.39.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.6.7.4.47.40/fgo_api_types/basic.py` & `fgo_api_types-2023.6.8.15.39.7/fgo_api_types/basic.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.6.7.4.47.40/fgo_api_types/common.py` & `fgo_api_types-2023.6.8.15.39.7/fgo_api_types/common.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.6.7.4.47.40/fgo_api_types/enums.py` & `fgo_api_types-2023.6.8.15.39.7/fgo_api_types/enums.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.6.7.4.47.40/fgo_api_types/gameenums.py` & `fgo_api_types-2023.6.8.15.39.7/fgo_api_types/gameenums.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.6.7.4.47.40/fgo_api_types/nice.py` & `fgo_api_types-2023.6.8.15.39.7/fgo_api_types/nice.py`

 * *Files 0% similar despite different names*

```diff
@@ -2463,14 +2463,15 @@
     condType: NiceCondType
     condTargetId: int
     condNum: int
 
 
 class NiceSpot(BaseModel):
     id: int
+    blankEarth: bool
     joinSpotIds: list[int]
     mapId: int
     name: str
     originalName: str
     image: Optional[HttpUrl] = None
     x: int
     y: int
@@ -2517,14 +2518,15 @@
     originalLongName: str
     flags: list[NiceWarFlag]
     banner: Optional[HttpUrl] = None
     headerImage: Optional[HttpUrl] = None
     priority: int
     parentWarId: int
     materialParentWarId: int
+    parentBlankEarthSpotId: int
     emptyMessage: str
     bgm: NiceBgm
     scriptId: str = Field(..., description='Could be "NONE".')
     script: HttpUrl
     startType: NiceWarStartType
     targetId: int
     eventId: int
```

### Comparing `fgo_api_types-2023.6.7.4.47.40/fgo_api_types/raw.py` & `fgo_api_types-2023.6.8.15.39.7/fgo_api_types/raw.py`

 * *Files 1% similar despite different names*

```diff
@@ -1412,14 +1412,15 @@
     mapImageId: int  # 9046
     mapImageW: int  # 2048
     mapImageH: int  # 2048
     headerImageId: int  # 1000
     priority: int  # 9046
     parentWarId: int  # 0
     materialParentWarId: int = 0  # 0
+    parentBlankEarthSpotId: int = 0
     flag: int  # 32
     emptyMessage: str  # "クエストがありません"
     bgmId: int  # 8
     scriptId: str  # "NONE"
     startType: int  # 0
     targetId: int  # 0
     eventId: int  # 80112
@@ -1508,14 +1509,27 @@
     activeCondType: int  # 1
     activeTargetId: int  # 0
     activeTargetValue: int  # 0
     closedMessage: str  # ""
     flag: int  # 0
 
 
+class MstBlankEarthSpot(BaseModelORJson):
+    id: int
+    warId: int
+    mapId: int
+    name: str
+    objectId: int
+    x: float
+    y: float
+    condTargetType: int
+    condTargetId: int
+    condTargetNum: int
+
+
 class MstSpotAdd(BaseModelORJson):
     spotId: int
     priority: int
     overrideType: int
     targetId: int
     targetText: str | None = None
     condType: int
@@ -2017,14 +2031,15 @@
     mstWar: MstWar
     mstEvent: Optional[MstEvent] = None
     mstWarAdd: list[MstWarAdd]
     mstMap: list[MstMap]
     mstBgm: list[MstBgm]
     mstMapGimmick: list[MstMapGimmick]
     mstSpot: list[MstSpot]
+    mstBlankEarthSpot: list[MstBlankEarthSpot]
     mstSpotAdd: list[MstSpotAdd]
     mstQuest: list[QuestEntity]
     mstSpotRoad: list[MstSpotRoad]
     mstWarQuestSelection: list[MstWarQuestSelection]
 
 
 class ShopEntity(BaseModelORJson):
```

### Comparing `fgo_api_types-2023.6.7.4.47.40/fgo_api_types/rayshift.py` & `fgo_api_types-2023.6.8.15.39.7/fgo_api_types/rayshift.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.6.7.4.47.40/fgo_api_types/search.py` & `fgo_api_types-2023.6.8.15.39.7/fgo_api_types/search.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.6.7.4.47.40/pyproject.toml` & `fgo_api_types-2023.6.8.15.39.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fgo-api-types"
-version = "2023.06.07.04.47.40"
+version = "2023.06.08.15.39.07"
 description = "Provide Pydantic types from FGO API"
 authors = ["squaresmile <squaresmile@protonmail.com>"]
 readme = "README.md"
 homepage = "https://api.atlasacademy.io"
 repository = "https://github.com/atlasacademy/fgo-game-data-api"
 
 [tool.poetry.dependencies]
```

### Comparing `fgo_api_types-2023.6.7.4.47.40/PKG-INFO` & `fgo_api_types-2023.6.8.15.39.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgo-api-types
-Version: 2023.6.7.4.47.40
+Version: 2023.6.8.15.39.7
 Summary: Provide Pydantic types from FGO API
 Home-page: https://api.atlasacademy.io
 Author: squaresmile
 Author-email: squaresmile@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

