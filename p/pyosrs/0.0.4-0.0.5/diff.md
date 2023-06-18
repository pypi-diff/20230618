# Comparing `tmp/pyosrs-0.0.4.tar.gz` & `tmp/pyosrs-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyosrs-0.0.4.tar", max compression
+gzip compressed data, was "pyosrs-0.0.5.tar", max compression
```

## Comparing `pyosrs-0.0.4.tar` & `pyosrs-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     7652 2023-06-17 14:31:37.020271 pyosrs-0.0.4/LICENSE
--rw-r--r--   0        0        0     2473 2023-06-17 14:31:37.020271 pyosrs-0.0.4/README.md
--rw-r--r--   0        0        0        0 2023-06-17 14:31:37.020271 pyosrs-0.0.4/pyosrs/__init__.py
--rw-r--r--   0        0        0     6151 2023-06-17 14:31:37.020271 pyosrs-0.0.4/pyosrs/client.py
--rw-r--r--   0        0        0     4762 2023-06-17 14:31:37.020271 pyosrs-0.0.4/pyosrs/enums.py
--rw-r--r--   0        0        0      410 2023-06-17 14:31:37.020271 pyosrs-0.0.4/pyosrs/exceptions.py
--rw-r--r--   0        0        0     3959 2023-06-17 14:31:37.020271 pyosrs-0.0.4/pyosrs/models.py
--rw-r--r--   0        0        0      901 2023-06-17 14:31:37.020271 pyosrs-0.0.4/pyosrs/utils.py
--rw-r--r--   0        0        0      767 2023-06-17 14:31:37.020271 pyosrs-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3207 1970-01-01 00:00:00.000000 pyosrs-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-06-18 17:03:43.880676 pyosrs-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2473 2023-06-18 17:03:43.884676 pyosrs-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-18 17:03:43.884676 pyosrs-0.0.5/pyosrs/__init__.py
+-rw-r--r--   0        0        0     6423 2023-06-18 17:03:43.884676 pyosrs-0.0.5/pyosrs/client.py
+-rw-r--r--   0        0        0     4835 2023-06-18 17:03:43.884676 pyosrs-0.0.5/pyosrs/enums.py
+-rw-r--r--   0        0        0      410 2023-06-18 17:03:43.884676 pyosrs-0.0.5/pyosrs/exceptions.py
+-rw-r--r--   0        0        0     4002 2023-06-18 17:03:43.884676 pyosrs-0.0.5/pyosrs/models.py
+-rw-r--r--   0        0        0      901 2023-06-18 17:03:43.884676 pyosrs-0.0.5/pyosrs/utils.py
+-rw-r--r--   0        0        0      767 2023-06-18 17:03:43.884676 pyosrs-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3207 1970-01-01 00:00:00.000000 pyosrs-0.0.5/PKG-INFO
```

### Comparing `pyosrs-0.0.4/LICENSE` & `pyosrs-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyosrs-0.0.4/README.md` & `pyosrs-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyosrs-0.0.4/pyosrs/client.py` & `pyosrs-0.0.5/pyosrs/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import asyncio
 from typing import Dict, Tuple
 
 import httpx
 
 from .enums import (
     BOSSES_INDEX,
+    CLUES_INDEX,
     GAME_MODE,
     HISCORE_RESPONSE_LEN,
     MINIGAMES_INDEX,
     SKILLS_INDEX,
 )
 from .exceptions import InvalidAPIResponseException, InvalidUserException
-from .models import Bosses, Hiscore, Minigame, Minigames, Skill, Skills
+from .models import Bosses, Clues, Hiscore, Minigame, Minigames, Skill, Skills
 from .utils import calc_combat_level
 
 
 class Pyosrs:
     def __init__(self):
         self.session = httpx.AsyncClient(
             base_url="https://secure.runescape.com/",
@@ -61,48 +62,52 @@
         try:
             response = await self._get_hiscore(username, game_mode)
         except httpx.HTTPStatusError:
             raise InvalidUserException(username)
 
         skills: Dict[str, Skill] = {}
         minigames: Dict[str, Minigame] = {}
+        clues: Dict[str, Minigame] = {}
         bosses: Dict[str, Minigame] = {}
 
         if len(lines := response.text.splitlines()) != HISCORE_RESPONSE_LEN:
             raise InvalidAPIResponseException
 
         for index, line in enumerate(lines):
             if index in SKILLS_INDEX:
                 rank, level, experience = map(int, line.split(","))
                 skills[SKILLS_INDEX[index][0]] = Skill(
                     rank=rank, level=level, experience=experience
                 )
             elif index in MINIGAMES_INDEX:
                 rank, score = map(int, line.split(","))
                 minigames[MINIGAMES_INDEX[index][0]] = Minigame(rank=rank, score=score)
+            elif index in CLUES_INDEX:
+                rank, score = map(int, line.split(","))
+                clues[CLUES_INDEX[index][0]] = Minigame(rank=rank, score=score)
             else:
                 rank, score = map(int, line.split(","))
                 bosses[BOSSES_INDEX[index][0]] = Minigame(rank=rank, score=score)
 
         combat_level = calc_combat_level(
             defence=skills["defence"].level,
             hitpoints=skills["hitpoints"].level,
             prayer=skills["prayer"].level,
             attack=skills["attack"].level,
             strength=skills["strength"].level,
             ranged=skills["ranged"].level,
             magic=skills["magic"].level,
         )
-
         return Hiscore(
             username=username,
             game_mode=game_mode,
             combat_level=combat_level,
             skills=Skills(**skills),
             minigames=Minigames(**minigames),
+            clues=Clues(**clues),
             bosses=Bosses(**bosses),
         )
 
     async def get_game_mode(self, username: str) -> Tuple[GAME_MODE, Hiscore]:
         """
         Determines the game mode of a given username by comparing the experience
         levels across different modes using the hiscore API.
```

### Comparing `pyosrs-0.0.4/pyosrs/enums.py` & `pyosrs-0.0.5/pyosrs/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,25 +42,28 @@
 
 MINIGAMES_INDEX: Final[Dict[int, Tuple[str, str]]] = {
     24: ("league_points", "League Points"),
     25: ("bounty_hunter_hunter", "Bounty Hunter - Hunter"),
     26: ("bounty_hunter_rogue", "Bounty Hunter - Rogue"),
     27: ("bounty_hunter_hunter_legacy", "Bounty Hunter (Legacy) - Hunter"),
     28: ("bounty_hunter_rogue_legacy", "Bounty Hunter (Legacy) - Rogue"),
+    36: ("lms", "LMS"),
+    37: ("pvp_arena", "PvP Arena"),
+    38: ("soul_wars", "Soul Wars Zeal"),
+    39: ("rifts_closed", "Rifts Closed"),
+}
+
+CLUES_INDEX: Final[Dict[int, Tuple[str, str]]] = {
     29: ("clue_scrolls_all", "Clue Scrolls All"),
     30: ("clue_scrolls_beginner", "Clue Scrolls Beginner"),
     31: ("clue_scrolls_easy", "Clue Scrolls Easy"),
     32: ("clue_scrolls_medium", "Clue Scrolls Medium"),
     33: ("clue_scrolls_hard", "Clue Scrolls Hard"),
     34: ("clue_scrolls_elite", "Clue Scrolls Elite"),
     35: ("clue_scrolls_master", "Clue Scrolls Master"),
-    36: ("lms", "LMS"),
-    37: ("pvp_arena", "PvP Arena"),
-    38: ("soul_wars", "Soul Wars Zeal"),
-    39: ("rifts_closed", "Rifts Closed"),
 }
 
 BOSSES_INDEX: Final[Dict[int, Tuple[str, str]]] = {
     40: ("abyssal_sire", "Abyssal Sire"),
     41: ("alchemical_hydra", "Alchemical Hydra"),
     42: ("artio", "Artio"),
     43: ("barrows_chests", "Barrows Chests"),
@@ -116,9 +119,9 @@
     90: ("vorkath", "Vorkath"),
     91: ("wintertodt", "Wintertodt"),
     92: ("zalcano", "Zalcano"),
     93: ("zulrah", "Zulrah"),
 }
 
 HISCORE_RESPONSE_LEN: Final[int] = (
-    len(SKILLS_INDEX) + len(MINIGAMES_INDEX) + len(BOSSES_INDEX)
+    len(SKILLS_INDEX) + len(MINIGAMES_INDEX) + len(CLUES_INDEX) + len(BOSSES_INDEX)
 )
```

### Comparing `pyosrs-0.0.4/pyosrs/models.py` & `pyosrs-0.0.5/pyosrs/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,25 +43,28 @@
 
 class Minigames(BaseModel):
     league_points: Minigame = Minigame()
     bounty_hunter_hunter: Minigame = Minigame()
     bounty_hunter_rogue: Minigame = Minigame()
     bounty_hunter_hunter_legacy: Minigame = Minigame()
     bounty_hunter_rogue_legacy: Minigame = Minigame()
+    lms: Minigame = Minigame()
+    pvp_arena: Minigame = Minigame()
+    soul_wars: Minigame = Minigame()
+    rifts_closed: Minigame = Minigame()
+
+
+class Clues(BaseModel):
     all: Minigame = Minigame()
     beginner: Minigame = Minigame()
     easy: Minigame = Minigame()
     medium: Minigame = Minigame()
     hard: Minigame = Minigame()
     elite: Minigame = Minigame()
     master: Minigame = Minigame()
-    lms: Minigame = Minigame()
-    pvp_arena: Minigame = Minigame()
-    soul_wars: Minigame = Minigame()
-    rifts_closed: Minigame = Minigame()
 
 
 class Bosses(BaseModel):
     alchemical_hydra: Minigame = Minigame()
     artio: Minigame = Minigame()
     barrows_chests: Minigame = Minigame()
     bryophyta: Minigame = Minigame()
@@ -118,8 +121,9 @@
 
 class Hiscore(BaseModel):
     username: str
     game_mode: GAME_MODE
     combat_level: int
     skills: Skills
     minigames: Minigames
+    clues: Clues
     bosses: Bosses
```

### Comparing `pyosrs-0.0.4/pyosrs/utils.py` & `pyosrs-0.0.5/pyosrs/utils.py`

 * *Files identical despite different names*

### Comparing `pyosrs-0.0.4/pyproject.toml` & `pyosrs-0.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyosrs"
-version = "0.0.4"
+version = "0.0.5"
 description = "A Python library for Oldschool RuneScape."
 authors = ["Phong Tran"]
 repository = "https://github.com/phongse/pyosrs"
 license = "LGPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
@@ -21,15 +21,15 @@
 factory-boy = "^3.2.1"
 mypy = "^1.2.0"
 pre-commit = "^3.2.2"
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 pytest-mock = "^3.10.0"
 respx = "^0.20.1"
-ruff = "^0.0.263"
+ruff = "^0.0.272"
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
 exclude = [
     "testing/",
```

### Comparing `pyosrs-0.0.4/PKG-INFO` & `pyosrs-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyosrs
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python library for Oldschool RuneScape.
 Home-page: https://github.com/phongse/pyosrs
 License: LGPL-3.0-only
 Author: Phong Tran
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
```

