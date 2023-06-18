# Comparing `tmp/autotraders-1.5.1.tar.gz` & `tmp/autotraders-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-1.5.1.tar", last modified: Sun Jun 11 00:17:33 2023, max compression
+gzip compressed data, was "autotraders-1.5.2.tar", last modified: Sun Jun 18 20:15:31 2023, max compression
```

## Comparing `autotraders-1.5.1.tar` & `autotraders-1.5.2.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:17:33.579790 autotraders-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-11 00:17:15.000000 autotraders-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-11 00:17:33.579790 autotraders-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-11 00:17:15.000000 autotraders-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:17:33.571790 autotraders-1.5.1/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:17:33.575791 autotraders-1.5.1/autotraders/faction/
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/faction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/faction/contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:17:33.575791 autotraders-1.5.1/autotraders/map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/map/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/map/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:17:33.575791 autotraders-1.5.1/autotraders/map/waypoint_types/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/map/waypoint_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/map/waypoint_types/jumpgate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/map/waypoint_types/marketplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/map/waypoint_types/shipyard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/paginated_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:17:33.575791 autotraders-1.5.1/autotraders/shared_models/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/shared_models/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/shared_models/map_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/shared_models/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/shared_models/trait.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/shared_models/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:17:33.575791 autotraders-1.5.1/autotraders/ship/
--rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/ship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/ship/cargo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/ship/nav.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/ship/ship_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/ship/states.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/ship/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/space_traders_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-11 00:17:15.000000 autotraders-1.5.1/autotraders/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:17:33.571790 autotraders-1.5.1/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-11 00:17:33.000000 autotraders-1.5.1/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-11 00:17:33.000000 autotraders-1.5.1/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 00:17:33.000000 autotraders-1.5.1/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-11 00:17:33.000000 autotraders-1.5.1/autotraders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-11 00:17:33.000000 autotraders-1.5.1/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-11 00:17:15.000000 autotraders-1.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 00:17:33.579790 autotraders-1.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:17:33.579790 autotraders-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-11 00:17:15.000000 autotraders-1.5.1/tests/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-11 00:17:15.000000 autotraders-1.5.1/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-11 00:17:15.000000 autotraders-1.5.1/tests/test_ship.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-11 00:17:15.000000 autotraders-1.5.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:15:31.905657 autotraders-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-18 20:15:17.000000 autotraders-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-18 20:15:31.905657 autotraders-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-18 20:15:17.000000 autotraders-1.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:15:31.901657 autotraders-1.5.2/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-18 20:15:17.000000 autotraders-1.5.2/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-18 20:15:17.000000 autotraders-1.5.2/autotraders/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:15:31.901657 autotraders-1.5.2/autotraders/faction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-18 20:15:17.000000 autotraders-1.5.2/autotraders/faction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-18 20:15:17.000000 autotraders-1.5.2/autotraders/faction/contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:15:31.901657 autotraders-1.5.2/autotraders/map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 20:15:17.000000 autotraders-1.5.2/autotraders/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-18 20:15:17.000000 autotraders-1.5.2/autotraders/map/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-18 20:15:17.000000 autotraders-1.5.2/autotraders/map/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:15:31.901657 autotraders-1.5.2/autotraders/map/waypoint_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-18 20:15:17.000000 autotraders-1.5.2/autotraders/map/waypoint_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-18 20:15:17.000000 autotraders-1.5.2/autotraders/map/waypoint_types/jumpgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-18 20:15:17.000000 autotraders-1.5.2/autotraders/map/waypoint_types/marketplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-18 20:15:17.000000 autotraders-1.5.2/autotraders/map/waypoint_types/shipyard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-18 20:15:17.000000 autotraders-1.5.2/autotraders/paginated_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-18 20:15:17.000000 autotraders-1.5.2/autotraders/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:15:31.901657 autotraders-1.5.2/autotraders/shared_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-18 20:15:17.000000 autotraders-1.5.2/autotraders/shared_models/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-18 20:15:17.000000 autotraders-1.5.2/autotraders/shared_models/map_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-18 20:15:17.000000 autotraders-1.5.2/autotraders/shared_models/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-18 20:15:17.000000 autotraders-1.5.2/autotraders/shared_models/trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-18 20:15:17.000000 autotraders-1.5.2/autotraders/shared_models/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:15:31.901657 autotraders-1.5.2/autotraders/ship/
+-rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-06-18 20:15:17.000000 autotraders-1.5.2/autotraders/ship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-18 20:15:17.000000 autotraders-1.5.2/autotraders/ship/cargo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-18 20:15:17.000000 autotraders-1.5.2/autotraders/ship/nav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-18 20:15:17.000000 autotraders-1.5.2/autotraders/ship/ship_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-18 20:15:17.000000 autotraders-1.5.2/autotraders/ship/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-18 20:15:17.000000 autotraders-1.5.2/autotraders/ship/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-18 20:15:17.000000 autotraders-1.5.2/autotraders/space_traders_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-18 20:15:17.000000 autotraders-1.5.2/autotraders/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-18 20:15:17.000000 autotraders-1.5.2/autotraders/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-18 20:15:17.000000 autotraders-1.5.2/autotraders/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:15:31.901657 autotraders-1.5.2/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-18 20:15:31.000000 autotraders-1.5.2/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-18 20:15:31.000000 autotraders-1.5.2/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 20:15:31.000000 autotraders-1.5.2/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-18 20:15:31.000000 autotraders-1.5.2/autotraders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 20:15:31.000000 autotraders-1.5.2/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-18 20:15:17.000000 autotraders-1.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 20:15:31.905657 autotraders-1.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:15:31.901657 autotraders-1.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-18 20:15:17.000000 autotraders-1.5.2/tests/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-18 20:15:17.000000 autotraders-1.5.2/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-18 20:15:17.000000 autotraders-1.5.2/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-18 20:15:17.000000 autotraders-1.5.2/tests/test_ship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-18 20:15:17.000000 autotraders-1.5.2/tests/test_util.py
```

### Comparing `autotraders-1.5.1/LICENSE` & `autotraders-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.1/PKG-INFO` & `autotraders-1.5.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.5.1
+Version: 1.5.2
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.5.1/README.md` & `autotraders-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.1/autotraders/agent.py` & `autotraders-1.5.2/autotraders/agent.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from typing import Optional
-
 from autotraders.faction.contract import Contract
+from autotraders.paginated_list import PaginatedList
 from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.session import AutoTradersSession
 from autotraders.ship import Ship
 
 
 class Agent(SpaceTradersEntity):
+    contracts: PaginatedList
+    starting_faction: str
+    symbol: str
+    account_id: str
+    credits: int
+    ships: PaginatedList
+    headquarters: MapSymbol
+
     def __init__(self, session: AutoTradersSession, data=None):
-        self.contracts: Optional[list[Contract]] = None
-        self.starting_faction: Optional[str] = None
-        self.symbol: Optional[str] = None
-        self.account_id: Optional[str] = None
-        self.credits: Optional[int] = None
-        self.ships: Optional[Ship] = None
-        self.headquarters: Optional[MapSymbol] = None
         super().__init__(session, "my/agent", data)
 
     def update(self, data=None):
         """Uses 3 API requests to get all agent details"""
         if data is None:
             data = self.get()["data"]
         self.account_id = data["accountId"]
```

### Comparing `autotraders-1.5.1/autotraders/faction/__init__.py` & `autotraders-1.5.2/autotraders/faction/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.1/autotraders/faction/contract.py` & `autotraders-1.5.2/autotraders/faction/contract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from datetime import datetime
-from typing import Optional
 
 from autotraders.paginated_list import PaginatedList
 from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.session import AutoTradersSession
 from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.time import parse_time
```

### Comparing `autotraders-1.5.1/autotraders/map/system.py` & `autotraders-1.5.2/autotraders/map/system.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union
+from typing import Union
 
 from autotraders.paginated_list import PaginatedList
 from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.session import AutoTradersSession
 from autotraders.map.waypoint import Waypoint
 from autotraders.shared_models.map_symbol import MapSymbol
 
@@ -10,32 +10,31 @@
 class System(SpaceTradersEntity):
     symbol: MapSymbol
     x: int
     y: int
     waypoints: list[Waypoint]
     factions: list[str]
     star_type: str
+    jump_gate: bool
 
     def __init__(
         self, symbol: Union[str, MapSymbol], session: AutoTradersSession, data=None
     ):
         self.symbol: MapSymbol = MapSymbol(symbol)
         super().__init__(session, "systems/" + str(self.symbol) + "/", data)
 
     def update(self, data=None):
         if data is None:
             data = self.get()["data"]
-        self.waypoints = []
+        self.waypoints = [Waypoint(w["symbol"], self.session, w) for w in data["waypoints"]]
         self.x = data["x"]
         self.y = data["y"]
         self.factions = data["factions"]
         self.star_type = data["type"]
-        for w in data["waypoints"]:
-            waypoint = Waypoint(w["symbol"], self.session, w)
-            self.waypoints.append(waypoint)
+        self.jump_gate = len([waypoint for waypoint in self.waypoints if waypoint.waypoint_type.lower() == "jump_gate"]) > 0
 
     @staticmethod
     def all(session, page: int = 1) -> PaginatedList:
         def paginated_func(p, num_per_page):
             r = session.get(
                 session.base_url
                 + "systems?limit="
```

### Comparing `autotraders-1.5.1/autotraders/map/waypoint.py` & `autotraders-1.5.2/autotraders/map/waypoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.space_traders_entity import SpaceTradersEntity
 
 
 class Waypoint(SpaceTradersEntity):
     waypoint_type: str
     faction: Optional[str]
-    traits: list[Trait]
+    traits: Optional[list[Trait]]
     marketplace: bool
     shipyard: bool
     symbol: MapSymbol
     x: int
     y: int
 
     def __init__(
@@ -34,16 +34,17 @@
         self.waypoint_type = data["type"]
         self.x = data["x"]
         self.y = data["y"]
         if "faction" in data:
             self.faction = data["faction"]["symbol"]
         else:
             self.faction = None
-        self.traits = []
+        self.traits = None
         if "traits" in data:
+            self.traits = []
             for trait in data["traits"]:
                 self.traits.append(Trait(trait))
         self.marketplace = (
             len([trait for trait in self.traits if trait.symbol == "MARKETPLACE"]) > 0
         )
         self.shipyard = (
             len([trait for trait in self.traits if trait.symbol == "SHIPYARD"]) > 0
```

### Comparing `autotraders-1.5.1/autotraders/map/waypoint_types/__init__.py` & `autotraders-1.5.2/autotraders/map/waypoint_types/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.1/autotraders/map/waypoint_types/marketplace.py` & `autotraders-1.5.2/autotraders/map/waypoint_types/marketplace.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Optional
-
 from autotraders.map.waypoint_types import WaypointType
 from autotraders.session import AutoTradersSession
 from autotraders.shared_models.item import Item
 
 
 class TradeGood(Item):
     def __init__(self, data):
@@ -11,19 +9,20 @@
         self.trade_volume: int = data["tradeVolume"]
         self.supply: str = data["supply"]
         self.purchase_price: int = data["purchasePrice"]
         self.sell_price: int = data["sellPrice"]
 
 
 class Marketplace(WaypointType):
+    imports: list[str]
+    exports: list[str]
+    exchange: list[str]
+    trade_goods: list[TradeGood]
+
     def __init__(self, waypoint: str, session: AutoTradersSession, data=None):
-        self.imports: Optional[list[str]] = None
-        self.exports: Optional[list[str]] = None
-        self.exchange: Optional[list[str]] = None
-        self.trade_goods: Optional[list[TradeGood]] = None
         super().__init__(waypoint, "market", session, data)
 
     def update(self, data: dict = None):
         if data is None:
             data = self.session.get(
                 self.session.base_url
                 + "systems/"
```

### Comparing `autotraders-1.5.1/autotraders/map/waypoint_types/shipyard.py` & `autotraders-1.5.2/autotraders/map/waypoint_types/shipyard.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Optional
-
 from autotraders.map.waypoint_types import WaypointType
 from autotraders.session import AutoTradersSession
 from autotraders.shared_models.transaction import ShipyardTransaction
 from autotraders.ship import Frame, Reactor, Engine, Module, Mount, Ship
 
 
 class ShipyardShip:
@@ -16,17 +14,18 @@
         self.reactor = Reactor(data["reactor"])
         self.engine = Engine(data["engine"])
         self.modules = [Module(d) for d in data["modules"]]
         self.mounts = [Mount(d) for d in data["mounts"]]
 
 
 class Shipyard(WaypointType):
+    ship_types: list[str]
+    ships: list[ShipyardShip]
+
     def __init__(self, waypoint: str, session: AutoTradersSession, data=None):
-        self.ship_types: Optional[list[str]] = None
-        self.ships: Optional[list[ShipyardShip]] = None
         super().__init__(waypoint, "shipyard", session, data)
 
     def update(self, data: dict = None):
         if data is None:
             data = self.get()["data"]
         self.ship_types = []
         for ship_type in data["shipTypes"]:
@@ -38,10 +37,10 @@
                 self.ships.append(ShipyardShip(ship))
 
     def purchase(self, ship_type: str):
         j = self.session.post(
             self.session.base_url + "my/ships",
             data={"shipType": ship_type, "waypointSymbol": self.location},
         ).json()
-        return Ship(j["data"]["ship"], self.session), ShipyardTransaction(
+        return Ship(j["data"]["ship"]["symbol"], self.session, j["data"]["ship"]), ShipyardTransaction(
             j["data"]["transaction"]
         )
```

### Comparing `autotraders-1.5.1/autotraders/paginated_list.py` & `autotraders-1.5.2/autotraders/paginated_list.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.1/autotraders/session.py` & `autotraders-1.5.2/autotraders/session.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,14 @@
         return r
 
 
 class AutoTradersSession(LimiterSession):
     def __init__(self, base_url="https://api.spacetraders.io/v2/"):
         super().__init__(per_second=2, burst_rate=10, limit_statuses=[429, 502])
         self.base_url = base_url
-        self.headers.update({"Prefer": "dynamic=true"})
 
 
 def get_session(token: Optional[str] = None) -> AutoTradersSession:
     """Creates a session with the provided token."""
     s = AutoTradersSession()
     if token is not None:
         s.auth = BearerAuth(token)
```

### Comparing `autotraders-1.5.1/autotraders/shared_models/map_symbol.py` & `autotraders-1.5.2/autotraders/shared_models/map_symbol.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.1/autotraders/shared_models/transaction.py` & `autotraders-1.5.2/autotraders/shared_models/transaction.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.1/autotraders/ship/__init__.py` & `autotraders-1.5.2/autotraders/ship/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import asyncio
+import json
 from typing import Union, Optional
 
 from autotraders.paginated_list import PaginatedList
 from autotraders.shared_models.item import Item
 from autotraders.shared_models.transaction import MarketTransaction, ShipyardTransaction
 from autotraders.ship.cargo import Cargo
 from autotraders.ship.nav import Nav
-from autotraders.ship.nav import Nav
 from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.map.system import System
 from autotraders.session import AutoTradersSession
 from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.ship.ship_components import Frame, Reactor, Engine, Module, Mount
 from autotraders.ship.survey import Survey
 from autotraders.time import parse_time
@@ -24,29 +24,34 @@
 
     def __str__(self):
         return str(self.current) + "/" + str(self.total)
 
 
 class Crew:
     def __init__(self, data):
-        self.current = data["current"]
-        self.required = data["required"]
-        self.capacity = data["capacity"]
+        self.current: int = data["current"]
+        self.required: int = data["required"]
+        self.capacity: int = data["capacity"]
         self.morale = data["morale"]
         self.wages = data["wages"]
 
 
 class Registration:
     def __init__(self, data):
-        self.name = data["name"]
-        self.faction_symbol = data["factionSymbol"]
-        self.role = data["role"]
+        self.name: str = data["name"]
+        self.faction_symbol: str = data["factionSymbol"]
+        self.role: str = data["role"]
 
 
 class Capabilities:
+    """
+    :ivar warp: can the ship warp
+    :ivar jump: can the ship jump without a jump gate
+    :ivar mine: can the ship mine (experimental)
+    """
     def __init__(self, modules, mounts):
         warp_drives = [module for module in modules if "warp" in module.symbol.lower()]
         jump_drives = [module for module in modules if "jump" in module.symbol.lower()]
         mine = [mount for mount in mounts if "mine" in mount.symbol.lower()]
         self.warp = len(warp_drives) > 0
         self.jump = len(jump_drives) > 0
         self.mine = len(mine) > 0
@@ -90,18 +95,16 @@
             self.nav = Nav(self.symbol, self.session, data["nav"])
         if "fuel" in data:
             self.fuel = Fuel(data["fuel"]["current"], data["fuel"]["capacity"])
         if "cargo" in data:
             self.cargo = Cargo(self.symbol, self.session, data["cargo"])
         if "registration" in data:
             self.registration = Registration(data["registration"])
-        try:
+        if self.modules is not None and self.mounts is not None:
             self.capabilities = Capabilities(self.modules, self.mounts)
-        except:
-            pass
 
     async def navigate_async(self, waypoint: Union[str, MapSymbol], interval=1):
         """Attempts to move ship to the provided waypoint.
         If the request succeeds, this function waits for the ship to arrive.
         :param interval: Frequency of updates in seconds (default: 1)
         """
         j = self.post("navigate", data={"waypointSymbol": str(waypoint)})
@@ -135,31 +138,41 @@
             },
         )
         self.update(j["data"])
 
     def patch_navigation(self, new_flight_mode):
         r = self.session.patch(
             self.session.base_url + "my/ships/" + self.symbol + "/nav",
-            data={"flightMode": new_flight_mode},
+            data=json.dumps({"flightMode": new_flight_mode})  # Requests is so dumb I spent 30 minutes debugging this
+            # just to find that its requests fault for sending a body of "flightMode=DRIFT".
         )
         j = r.json()
         if "error" in j:
             raise IOError(j["error"]["message"])
         self.update({"nav": j["data"]})
 
     def dock(self):
         j = self.post("dock")
         self.update(j["data"])
 
     def orbit(self):
         j = self.post("orbit")
         self.update(j["data"])
 
-    def extract(self):
-        j = self.post("extract")
+    def extract(self, survey: Survey = None):
+        if survey is None:
+            j = self.post("extract")
+        else:
+            j = self.post("extract", data={
+                "signature": survey.signature,
+                "symbol": survey.symbol,
+                "deposits": survey.deposits,
+                "expiration": survey.expiration.isoformat(),
+                "size": survey.size
+            })
         self.update(j["data"])
         self.reactor.cooldown = parse_time(j["data"]["cooldown"]["expiration"])
         return Item(
             j["data"]["extraction"]["yield"]["symbol"],
             j["data"]["extraction"]["yield"]["units"],
             None,
         )
```

### Comparing `autotraders-1.5.1/autotraders/ship/cargo.py` & `autotraders-1.5.2/autotraders/ship/cargo.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from typing import Optional
-
 from autotraders import AutoTradersSession
 from autotraders.shared_models.item import Item
 from autotraders.space_traders_entity import SpaceTradersEntity
 
 
 class Cargo(SpaceTradersEntity):
+    capacity: int
+    current: int
+    inventory: list[Item]
+
     def __init__(self, symbol, session: AutoTradersSession, data=None):
-        self.capacity: Optional[int] = None
-        self.current: Optional[int] = None
-        self.inventory: Optional[list[Item]] = None
         super().__init__(session, "my/ships/" + symbol, data)
 
     def update(self, data: dict = None) -> None:
         if data is None:
             data = self.get("cargo")["data"]
         self.capacity = data["capacity"]
         inventory = data["inventory"]
```

### Comparing `autotraders-1.5.1/autotraders/ship/nav.py` & `autotraders-1.5.2/autotraders/ship/nav.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from datetime import datetime, timezone
-from typing import Optional
 
 from autotraders import AutoTradersSession
 from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.time import parse_time
 
 
@@ -13,20 +12,21 @@
         self.departure = MapSymbol(data["departure"]["symbol"])
         self.departure_time = parse_time(data["departureTime"])
         self.arrival = parse_time(data["arrival"])
         self.moving = self.arrival > datetime.now(timezone.utc)
 
 
 class Nav(SpaceTradersEntity):
+    status: str
+    location: MapSymbol
+    flight_mode: str
+    route: Route
+    moving: bool
+
     def __init__(self, symbol, session: AutoTradersSession, data=None):
-        self.status: Optional[str] = None
-        self.location: Optional[MapSymbol] = None
-        self.flight_mode: Optional[str] = None
-        self.route: Optional[Route] = None
-        self.moving: Optional[bool] = None
         super().__init__(session, "my/ships/" + symbol, data)
 
     def update(self, data: dict = None) -> None:
         if data is None:
             data = self.get("nav")["data"]
         self.status = data["status"]
         self.location = MapSymbol(data["waypointSymbol"])
```

### Comparing `autotraders-1.5.1/autotraders/ship/ship_components.py` & `autotraders-1.5.2/autotraders/ship/ship_components.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.1/autotraders/space_traders_entity.py` & `autotraders-1.5.2/autotraders/space_traders_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,11 +37,12 @@
         j = r.json()
         if "error" in j:
             raise IOError(j["error"]["message"])
         return j
 
     def update(self, data: dict = None):
         """
-        :param data: If you have data from an api requests, you can provide it here. If not provided, an API request will be sent.
+        :param data: If you have data from an api requests, you can provide it here. If not provided, an API request
+        will be sent.
         :raise IOException: If the server fails
         """
         pass
```

### Comparing `autotraders-1.5.1/autotraders/status.py` & `autotraders-1.5.2/autotraders/status.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,20 +31,20 @@
     def __init__(self, name: str, url: str):
         self.name = name
         self.url = url
 
 
 class Status:
     """
-    :ivar status: User Readable description of the server status
+    :ivar status: User-Readable description of the server status
     :ivar version: The server version
     :ivar reset_date: A datetime of the last reset date
     :ivar description: A user-readable description of the server
     :ivar stats: A dictionary of stats. The keys are agents, ships, systems, and waypoints
-    :ivar leaderboards:
+    :ivar leaderboards: The list of leaderboards (most credits, most charts)
     :ivar next_reset: A datetime of the next reset
     :ivar reset_frequency: A user-readable description of the server reset frequency
     :ivar announcements: A list of announcements
     :ivar links: A list of useful links
     """
 
     status: str
```

### Comparing `autotraders-1.5.1/autotraders/util.py` & `autotraders-1.5.2/autotraders/util.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.1/autotraders.egg-info/PKG-INFO` & `autotraders-1.5.2/autotraders.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.5.1
+Version: 1.5.2
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.5.1/autotraders.egg-info/SOURCES.txt` & `autotraders-1.5.2/autotraders.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -32,9 +32,10 @@
 autotraders/ship/cargo.py
 autotraders/ship/nav.py
 autotraders/ship/ship_components.py
 autotraders/ship/states.py
 autotraders/ship/survey.py
 tests/test_contract.py
 tests/test_init.py
+tests/test_map.py
 tests/test_ship.py
 tests/test_util.py
```

### Comparing `autotraders-1.5.1/pyproject.toml` & `autotraders-1.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autotraders"
-version = "1.5.1"
+version = "1.5.2"
 authors = [
   { name="Ashwin Naren", email="arihant2math@gmail.com" },
 ]
 description = "A powerful spacetraders API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `autotraders-1.5.1/tests/test_init.py` & `autotraders-1.5.2/tests/test_init.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,45 @@
-import time
+# import time
 
 import pytest
 
 from autotraders import get_status
 from autotraders.agent import Agent
 from autotraders.faction import Faction
 from autotraders.session import get_session
 
 
 @pytest.fixture
 def session():
-    s = get_session(None)
-    s.base_url = "https://stoplight.io/mocks/spacetraders/spacetraders/96627693/"
+    s = get_session("TEST")
+    s.base_url = "https://stoplight.io/mocks/spacetraders/spacetraders/96627693/"  # Use http://127.0.0.1:4010/ for local mocking
+    s.headers.update({"Prefer": "dynamic=true"})
     return s
 
 
 def test_invalid_api_key():
-    s = get_session("TEST")
+    s = get_session("INVALID TOKEN")
     try:
         Agent(s)
         assert False  # shouldn't complete successfully
     except Exception as e:
         assert type(e) is IOError
 
 
 def test_get_status():
     status = get_status()
     assert status.version == "v2"
 
 
-def test_rate_limiter(session):
-    t1 = time.time()
-    for i in range(20):
-        get_status(session)
-    t2 = time.time()
-    assert t2 - t1 < 100
+# def test_rate_limiter(session):
+#     t1 = time.time()
+#     for i in range(20):
+#         get_status()
+#     t2 = time.time()
+#     assert t2 - t1 < 100
 
 
 def test_agent(session):
     Agent(session)
 
 
 def test_faction(session):
```

### Comparing `autotraders-1.5.1/tests/test_ship.py` & `autotraders-1.5.2/tests/test_ship.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.1/tests/test_util.py` & `autotraders-1.5.2/tests/test_util.py`

 * *Files identical despite different names*

