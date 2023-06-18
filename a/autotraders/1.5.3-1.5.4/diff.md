# Comparing `tmp/autotraders-1.5.3.tar.gz` & `tmp/autotraders-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-1.5.3.tar", last modified: Sun Jun 18 20:49:12 2023, max compression
+gzip compressed data, was "autotraders-1.5.4.tar", last modified: Sun Jun 18 21:54:42 2023, max compression
```

## Comparing `autotraders-1.5.3.tar` & `autotraders-1.5.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:49:12.928164 autotraders-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-18 20:48:57.000000 autotraders-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-18 20:49:12.928164 autotraders-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-18 20:48:57.000000 autotraders-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:49:12.920163 autotraders-1.5.3/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-18 20:48:57.000000 autotraders-1.5.3/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-18 20:48:57.000000 autotraders-1.5.3/autotraders/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:49:12.920163 autotraders-1.5.3/autotraders/faction/
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-18 20:48:57.000000 autotraders-1.5.3/autotraders/faction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-18 20:48:57.000000 autotraders-1.5.3/autotraders/faction/contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:49:12.924164 autotraders-1.5.3/autotraders/map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 20:48:57.000000 autotraders-1.5.3/autotraders/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-18 20:48:57.000000 autotraders-1.5.3/autotraders/map/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-18 20:48:57.000000 autotraders-1.5.3/autotraders/map/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:49:12.924164 autotraders-1.5.3/autotraders/map/waypoint_types/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-18 20:48:57.000000 autotraders-1.5.3/autotraders/map/waypoint_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-18 20:48:57.000000 autotraders-1.5.3/autotraders/map/waypoint_types/jumpgate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-18 20:48:57.000000 autotraders-1.5.3/autotraders/map/waypoint_types/marketplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-18 20:48:57.000000 autotraders-1.5.3/autotraders/map/waypoint_types/shipyard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-18 20:48:57.000000 autotraders-1.5.3/autotraders/paginated_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-18 20:48:57.000000 autotraders-1.5.3/autotraders/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:49:12.924164 autotraders-1.5.3/autotraders/shared_models/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-18 20:48:57.000000 autotraders-1.5.3/autotraders/shared_models/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-18 20:48:57.000000 autotraders-1.5.3/autotraders/shared_models/map_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-18 20:48:57.000000 autotraders-1.5.3/autotraders/shared_models/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-18 20:48:57.000000 autotraders-1.5.3/autotraders/shared_models/trait.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-18 20:48:57.000000 autotraders-1.5.3/autotraders/shared_models/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:49:12.924164 autotraders-1.5.3/autotraders/ship/
--rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-06-18 20:48:57.000000 autotraders-1.5.3/autotraders/ship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-18 20:48:57.000000 autotraders-1.5.3/autotraders/ship/cargo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-18 20:48:57.000000 autotraders-1.5.3/autotraders/ship/nav.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-18 20:48:57.000000 autotraders-1.5.3/autotraders/ship/ship_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-18 20:48:57.000000 autotraders-1.5.3/autotraders/ship/states.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-18 20:48:57.000000 autotraders-1.5.3/autotraders/ship/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-18 20:48:57.000000 autotraders-1.5.3/autotraders/space_traders_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-18 20:48:57.000000 autotraders-1.5.3/autotraders/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-18 20:48:57.000000 autotraders-1.5.3/autotraders/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-18 20:48:57.000000 autotraders-1.5.3/autotraders/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:49:12.920163 autotraders-1.5.3/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-18 20:49:12.000000 autotraders-1.5.3/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-18 20:49:12.000000 autotraders-1.5.3/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 20:49:12.000000 autotraders-1.5.3/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-18 20:49:12.000000 autotraders-1.5.3/autotraders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 20:49:12.000000 autotraders-1.5.3/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-18 20:48:57.000000 autotraders-1.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 20:49:12.928164 autotraders-1.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:49:12.928164 autotraders-1.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-18 20:48:57.000000 autotraders-1.5.3/tests/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-18 20:48:57.000000 autotraders-1.5.3/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-18 20:48:57.000000 autotraders-1.5.3/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-18 20:48:57.000000 autotraders-1.5.3/tests/test_ship.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-18 20:48:57.000000 autotraders-1.5.3/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:54:42.437183 autotraders-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-18 21:54:25.000000 autotraders-1.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-18 21:54:42.437183 autotraders-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-18 21:54:25.000000 autotraders-1.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:54:42.425183 autotraders-1.5.4/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:54:42.429183 autotraders-1.5.4/autotraders/faction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/faction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/faction/contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:54:42.429183 autotraders-1.5.4/autotraders/map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/map/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/map/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:54:42.433183 autotraders-1.5.4/autotraders/map/waypoint_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/map/waypoint_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/map/waypoint_types/jumpgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/map/waypoint_types/marketplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/map/waypoint_types/shipyard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/paginated_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:54:42.433183 autotraders-1.5.4/autotraders/shared_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/shared_models/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/shared_models/map_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/shared_models/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/shared_models/trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/shared_models/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:54:42.437183 autotraders-1.5.4/autotraders/ship/
+-rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/ship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/ship/cargo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/ship/nav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/ship/ship_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/ship/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/ship/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/space_traders_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:54:42.429183 autotraders-1.5.4/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-18 21:54:42.000000 autotraders-1.5.4/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-18 21:54:42.000000 autotraders-1.5.4/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 21:54:42.000000 autotraders-1.5.4/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-18 21:54:42.000000 autotraders-1.5.4/autotraders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 21:54:42.000000 autotraders-1.5.4/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-18 21:54:25.000000 autotraders-1.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 21:54:42.437183 autotraders-1.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:54:42.437183 autotraders-1.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-18 21:54:25.000000 autotraders-1.5.4/tests/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-18 21:54:25.000000 autotraders-1.5.4/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-18 21:54:25.000000 autotraders-1.5.4/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-18 21:54:25.000000 autotraders-1.5.4/tests/test_ship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-18 21:54:25.000000 autotraders-1.5.4/tests/test_util.py
```

### Comparing `autotraders-1.5.3/LICENSE` & `autotraders-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.3/PKG-INFO` & `autotraders-1.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.5.3
+Version: 1.5.4
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.5.3/README.md` & `autotraders-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.3/autotraders/agent.py` & `autotraders-1.5.4/autotraders/agent.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.3/autotraders/faction/__init__.py` & `autotraders-1.5.4/autotraders/faction/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.3/autotraders/faction/contract.py` & `autotraders-1.5.4/autotraders/faction/contract.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.3/autotraders/map/system.py` & `autotraders-1.5.4/autotraders/map/waypoint.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,77 @@
-from typing import Union
+from typing import Optional, Union
 
 from autotraders.paginated_list import PaginatedList
-from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.session import AutoTradersSession
-from autotraders.map.waypoint import Waypoint
+from autotraders.shared_models.trait import Trait
+
 from autotraders.shared_models.map_symbol import MapSymbol
+from autotraders.space_traders_entity import SpaceTradersEntity
 
 
-class System(SpaceTradersEntity):
+class Waypoint(SpaceTradersEntity):
+    waypoint_type: str
+    faction: Optional[str]
+    traits: Optional[list[Trait]]
+    marketplace: bool
+    shipyard: bool
     symbol: MapSymbol
     x: int
     y: int
-    waypoints: list[Waypoint]
-    factions: list[str]
-    star_type: str
-    jump_gate: bool
 
     def __init__(
         self, symbol: Union[str, MapSymbol], session: AutoTradersSession, data=None
     ):
-        self.symbol: MapSymbol = MapSymbol(symbol)
-        super().__init__(session, "systems/" + str(self.symbol) + "/", data)
+        self.symbol = MapSymbol(symbol)
+        super().__init__(
+            session,
+            "systems/" + self.symbol.system + "/waypoints/" + self.symbol.waypoint,
+            data,
+        )
 
     def update(self, data=None):
         if data is None:
             data = self.get()["data"]
-        self.waypoints = [Waypoint(w["symbol"], self.session, w) for w in data["waypoints"]]
+        self.waypoint_type = data["type"]
         self.x = data["x"]
         self.y = data["y"]
-        self.factions = data["factions"]
-        self.star_type = data["type"]
-        self.jump_gate = len([waypoint for waypoint in self.waypoints if waypoint.waypoint_type.lower() == "jump_gate"]) > 0
+        if "faction" in data:
+            self.faction = data["faction"]["symbol"]
+        else:
+            self.faction = None
+        self.traits = None
+        if "traits" in data:
+            self.traits = []
+            for trait in data["traits"]:
+                self.traits.append(Trait(trait))
+        self.marketplace = (
+            len([trait for trait in self.traits if trait.symbol == "MARKETPLACE"]) > 0
+        )
+        self.shipyard = (
+            len([trait for trait in self.traits if trait.symbol == "SHIPYARD"]) > 0
+        )
 
     @staticmethod
-    def all(session, page: int = 1) -> PaginatedList:
+    def all(session, system_symbol, page: int = 1) -> PaginatedList:
         def paginated_func(p, num_per_page):
             r = session.get(
                 session.base_url
-                + "systems?limit="
+                + "systems/"
+                + system_symbol
+                + "/waypoints?limit="
                 + str(num_per_page)
                 + "&page="
                 + str(p)
             )
             j = r.json()
             if "error" in j:
                 raise IOError(j["error"]["message"])
-            systems = []
-            for system in j["data"]:
-                s = System(system["symbol"], session, system)
-                systems.append(s)
-            return systems, j["meta"]["total"]
+            waypoints = []
+            for w in j["data"]:
+                waypoint = Waypoint(w["symbol"], session, w)
+                waypoints.append(waypoint)
+            return waypoints, j["meta"]["total"]
 
         return PaginatedList(paginated_func, page)
 
     def __eq__(self, other):
         return self.symbol == other.symbol
```

### Comparing `autotraders-1.5.3/autotraders/map/waypoint.py` & `autotraders-1.5.4/autotraders/map/waypoint_types/shipyard.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,77 +1,46 @@
-from typing import Optional, Union
-
-from autotraders.paginated_list import PaginatedList
+from autotraders.map.waypoint_types import WaypointType
 from autotraders.session import AutoTradersSession
-from autotraders.shared_models.trait import Trait
+from autotraders.shared_models.transaction import ShipyardTransaction
+from autotraders.ship import Frame, Reactor, Engine, Module, Mount, Ship
 
-from autotraders.shared_models.map_symbol import MapSymbol
-from autotraders.space_traders_entity import SpaceTradersEntity
 
+class ShipyardShip:
+    def __init__(self, data):
+        self.ship_type = data["type"]
+        self.name = data["name"]
+        self.description = data["description"]
+        self.purchase_price = data["purchasePrice"]
+        self.frame = Frame(data["frame"])
+        self.reactor = Reactor(data["reactor"])
+        self.engine = Engine(data["engine"])
+        self.modules = [Module(d) for d in data["modules"]]
+        self.mounts = [Mount(d) for d in data["mounts"]]
+
+
+class Shipyard(WaypointType):
+    ship_types: list[str]
+    ships: list[ShipyardShip]
 
-class Waypoint(SpaceTradersEntity):
-    waypoint_type: str
-    faction: Optional[str]
-    traits: Optional[list[Trait]]
-    marketplace: bool
-    shipyard: bool
-    symbol: MapSymbol
-    x: int
-    y: int
-
-    def __init__(
-        self, symbol: Union[str, MapSymbol], session: AutoTradersSession, data=None
-    ):
-        self.symbol = MapSymbol(symbol)
-        super().__init__(
-            session,
-            "systems/" + self.symbol.system + "/waypoints/" + self.symbol.waypoint,
-            data,
-        )
+    def __init__(self, waypoint: str, session: AutoTradersSession, data=None):
+        super().__init__(waypoint, "shipyard", session, data)
 
-    def update(self, data=None):
+    def update(self, data: dict = None):
         if data is None:
             data = self.get()["data"]
-        self.waypoint_type = data["type"]
-        self.x = data["x"]
-        self.y = data["y"]
-        if "faction" in data:
-            self.faction = data["faction"]["symbol"]
-        else:
-            self.faction = None
-        self.traits = None
-        if "traits" in data:
-            self.traits = []
-            for trait in data["traits"]:
-                self.traits.append(Trait(trait))
-        self.marketplace = (
-            len([trait for trait in self.traits if trait.symbol == "MARKETPLACE"]) > 0
-        )
-        self.shipyard = (
-            len([trait for trait in self.traits if trait.symbol == "SHIPYARD"]) > 0
+        self.ship_types = []
+        for ship_type in data["shipTypes"]:
+            self.ship_types.append(ship_type["type"])
+        self.ships = None
+        if "ships" in data:
+            self.ships = []
+            for ship in data["ships"]:
+                self.ships.append(ShipyardShip(ship))
+
+    def purchase(self, ship_type: str):
+        j = self.session.post(
+            self.session.base_url + "my/ships",
+            data={"shipType": ship_type, "waypointSymbol": self.location},
+        ).json()
+        return Ship(j["data"]["ship"]["symbol"], self.session, j["data"]["ship"]), ShipyardTransaction(
+            j["data"]["transaction"]
         )
-
-    @staticmethod
-    def all(session, system_symbol, page: int = 1) -> PaginatedList:
-        def paginated_func(p, num_per_page):
-            r = session.get(
-                session.base_url
-                + "systems/"
-                + system_symbol
-                + "/waypoints?limit="
-                + str(num_per_page)
-                + "&page="
-                + str(p)
-            )
-            j = r.json()
-            if "error" in j:
-                raise IOError(j["error"]["message"])
-            waypoints = []
-            for w in j["data"]:
-                waypoint = Waypoint(w["symbol"], session, w)
-                waypoints.append(waypoint)
-            return waypoints, j["meta"]["total"]
-
-        return PaginatedList(paginated_func, page)
-
-    def __eq__(self, other):
-        return self.symbol == other.symbol
```

### Comparing `autotraders-1.5.3/autotraders/map/waypoint_types/__init__.py` & `autotraders-1.5.4/autotraders/map/waypoint_types/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.3/autotraders/map/waypoint_types/jumpgate.py` & `autotraders-1.5.4/autotraders/map/waypoint_types/jumpgate.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.3/autotraders/map/waypoint_types/marketplace.py` & `autotraders-1.5.4/autotraders/map/waypoint_types/marketplace.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.3/autotraders/paginated_list.py` & `autotraders-1.5.4/autotraders/paginated_list.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.3/autotraders/session.py` & `autotraders-1.5.4/autotraders/session.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.3/autotraders/shared_models/map_symbol.py` & `autotraders-1.5.4/autotraders/shared_models/map_symbol.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.3/autotraders/shared_models/transaction.py` & `autotraders-1.5.4/autotraders/shared_models/transaction.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.3/autotraders/ship/__init__.py` & `autotraders-1.5.4/autotraders/ship/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.3/autotraders/ship/cargo.py` & `autotraders-1.5.4/autotraders/ship/cargo.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.3/autotraders/ship/nav.py` & `autotraders-1.5.4/autotraders/ship/nav.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.3/autotraders/ship/ship_components.py` & `autotraders-1.5.4/autotraders/ship/ship_components.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.3/autotraders/space_traders_entity.py` & `autotraders-1.5.4/autotraders/space_traders_entity.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.3/autotraders/status.py` & `autotraders-1.5.4/autotraders/status.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.3/autotraders/util.py` & `autotraders-1.5.4/autotraders/util.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.3/autotraders.egg-info/PKG-INFO` & `autotraders-1.5.4/autotraders.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.5.3
+Version: 1.5.4
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.5.3/autotraders.egg-info/SOURCES.txt` & `autotraders-1.5.4/autotraders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.3/pyproject.toml` & `autotraders-1.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autotraders"
-version = "1.5.3"
+version = "1.5.4"
 authors = [
   { name="Ashwin Naren", email="arihant2math@gmail.com" },
 ]
 description = "A powerful spacetraders API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `autotraders-1.5.3/tests/test_init.py` & `autotraders-1.5.4/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.3/tests/test_map.py` & `autotraders-1.5.4/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.3/tests/test_ship.py` & `autotraders-1.5.4/tests/test_ship.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.3/tests/test_util.py` & `autotraders-1.5.4/tests/test_util.py`

 * *Files identical despite different names*

