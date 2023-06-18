# Comparing `tmp/nhl_api_py-0.4.1.tar.gz` & `tmp/nhl_api_py-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhl_api_py-0.4.1.tar", max compression
+gzip compressed data, was "nhl_api_py-0.4.2.tar", max compression
```

## Comparing `nhl_api_py-0.4.1.tar` & `nhl_api_py-0.4.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     4792 2023-06-13 00:47:35.510504 nhl_api_py-0.4.1/README.md
--rw-r--r--   0        0        0       34 2023-06-03 14:07:42.805624 nhl_api_py-0.4.1/nhlpy/__init__.py
--rw-r--r--   0        0        0      315 2023-06-09 15:14:25.320047 nhl_api_py-0.4.1/nhlpy/api/__init__.py
--rw-r--r--   0        0        0      743 2023-06-03 14:07:42.805624 nhl_api_py-0.4.1/nhlpy/api/core.py
--rw-r--r--   0        0        0     4213 2023-06-16 18:35:41.424465 nhl_api_py-0.4.1/nhlpy/api/games.py
--rw-r--r--   0        0        0     6775 2023-06-16 18:35:41.424465 nhl_api_py-0.4.1/nhlpy/api/helpers.py
--rw-r--r--   0        0        0     2035 2023-06-16 18:35:41.424465 nhl_api_py-0.4.1/nhlpy/api/players.py
--rw-r--r--   0        0        0      910 2023-06-16 18:35:41.424465 nhl_api_py-0.4.1/nhlpy/api/schedule.py
--rw-r--r--   0        0        0     1967 2023-06-16 18:35:41.424465 nhl_api_py-0.4.1/nhlpy/api/standings.py
--rw-r--r--   0        0        0     2146 2023-06-16 18:35:41.424465 nhl_api_py-0.4.1/nhlpy/api/teams.py
--rw-r--r--   0        0        0      641 2023-06-13 00:29:30.470493 nhl_api_py-0.4.1/nhlpy/nhl_client.py
--rw-r--r--   0        0        0     1390 2023-06-16 18:35:41.424465 nhl_api_py-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     5957 1970-01-01 00:00:00.000000 nhl_api_py-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     4940 2023-06-18 13:41:39.289397 nhl_api_py-0.4.2/README.md
+-rw-r--r--   0        0        0       34 2023-06-03 14:07:42.805624 nhl_api_py-0.4.2/nhlpy/__init__.py
+-rw-r--r--   0        0        0      315 2023-06-09 15:14:25.320047 nhl_api_py-0.4.2/nhlpy/api/__init__.py
+-rw-r--r--   0        0        0      743 2023-06-03 14:07:42.805624 nhl_api_py-0.4.2/nhlpy/api/core.py
+-rw-r--r--   0        0        0     4213 2023-06-16 18:35:41.424465 nhl_api_py-0.4.2/nhlpy/api/games.py
+-rw-r--r--   0        0        0     6775 2023-06-16 18:35:41.424465 nhl_api_py-0.4.2/nhlpy/api/helpers.py
+-rw-r--r--   0        0        0     2035 2023-06-16 18:35:41.424465 nhl_api_py-0.4.2/nhlpy/api/players.py
+-rw-r--r--   0        0        0      910 2023-06-16 18:35:41.424465 nhl_api_py-0.4.2/nhlpy/api/schedule.py
+-rw-r--r--   0        0        0     1942 2023-06-18 13:41:39.289397 nhl_api_py-0.4.2/nhlpy/api/standings.py
+-rw-r--r--   0        0        0     2146 2023-06-16 18:35:41.424465 nhl_api_py-0.4.2/nhlpy/api/teams.py
+-rw-r--r--   0        0        0      641 2023-06-13 00:29:30.470493 nhl_api_py-0.4.2/nhlpy/nhl_client.py
+-rw-r--r--   0        0        0     1390 2023-06-18 13:41:39.289397 nhl_api_py-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     6105 1970-01-01 00:00:00.000000 nhl_api_py-0.4.2/PKG-INFO
```

### Comparing `nhl_api_py-0.4.1/README.md` & `nhl_api_py-0.4.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -62,19 +62,23 @@
 client.games.get_game_content(game_id=2020020001)
 
 # Players
 client.players.get_player(person_id=8477949)
 client.players.get_player_stats(person_id=8477949, season="20222023", stat_type="statsSingleSeason")
 client.players.get_player_stat_types()
 
-# Helpers - Common use cases, data extraction, etc.  For easier dataframe .  These return data that has been parsed
+# Helpers - Common use cases, data extraction, etc.  For easier dataframe initialization.  
+#  These return data that has been parsed
 # out, with some additional calculations as well.
 standings_list = nhl_client.helpers.league_standings(season="20222023")
 standings_df = pd.DataFrame(standings_list)
 standings_df.head(20)
+
+game_results = nhl_client.helpers.get_all_game_results(season="20222023", detailed_game_data=True, game_type="R", team_ids=[7])
+
 ```
 
 
 
 - - - 
 
 As mentioned at the top, I created a notebook to go over some of the available methods in more detail.  Below is an export md of that notebook, with out cell executions.
```

### Comparing `nhl_api_py-0.4.1/nhlpy/api/core.py` & `nhl_api_py-0.4.2/nhlpy/api/core.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.4.1/nhlpy/api/games.py` & `nhl_api_py-0.4.2/nhlpy/api/games.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.4.1/nhlpy/api/helpers.py` & `nhl_api_py-0.4.2/nhlpy/api/helpers.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.4.1/nhlpy/api/players.py` & `nhl_api_py-0.4.2/nhlpy/api/players.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.4.1/nhlpy/api/schedule.py` & `nhl_api_py-0.4.2/nhlpy/api/schedule.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.4.1/nhlpy/api/standings.py` & `nhl_api_py-0.4.2/nhlpy/api/standings.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,25 +5,25 @@
     def get_standing_types(self) -> dict:
         """
         Returns a list of standing types that can be used in get_standings_by_standing_type()
         :return: dict of standing types
         """
         return self._get(resource="standingsTypes").json()
 
-    def get_standings(self, season: str = None, detailed_record: bool = False) -> dict:
+    def get_standings(self, season: str, detailed_record: bool = False) -> dict:
         """
         Gets the standings for the season supplied via season: param.
         :param season:
         :param detailed_record: Detailed information for each team including
             home and away records, record in shootouts, last ten games, and split
             head-to-head records against divisions and conferences.
         :return: dict
         """
-        modifier: str = f"season={season}&" if season else ""
-        detailed: str = "expand=standings.record&" if detailed_record else ""
+        modifier: str = f"season={season}"
+        detailed: str = "&expand=standings.record&" if detailed_record else ""
 
         response: dict = self._get(resource=f"standings?{modifier}{detailed}").json()
         return response["records"]
 
     def get_standings_by_standing_type(
         self, season: str, standing_type: str, detailed_records: bool = False
     ) -> dict:
```

### Comparing `nhl_api_py-0.4.1/nhlpy/api/teams.py` & `nhl_api_py-0.4.2/nhlpy/api/teams.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.4.1/nhlpy/nhl_client.py` & `nhl_api_py-0.4.2/nhlpy/nhl_client.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.4.1/pyproject.toml` & `nhl_api_py-0.4.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nhl-api-py"
-version = "0.4.1"
+version = "0.4.2"
 description = "NHL API.  For standings, team stats, outcomes, player information.  Contains each individual API endpoint as well as convience methods for easy data loading in Pandas or any ML applications."
 authors = ["Corey Schaf <cschaf@gmail.com>"]
 readme = "README.md"
 packages = [{include = "nhlpy"}]
 license = "GPL-3.0-or-later"
 homepage = "https://github.com/coreyjs/nhl-api-py"
 repository = "https://github.com/coreyjs/nhl-api-py"
```

### Comparing `nhl_api_py-0.4.1/PKG-INFO` & `nhl_api_py-0.4.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhl-api-py
-Version: 0.4.1
+Version: 0.4.2
 Summary: NHL API.  For standings, team stats, outcomes, player information.  Contains each individual API endpoint as well as convience methods for easy data loading in Pandas or any ML applications.
 Home-page: https://github.com/coreyjs/nhl-api-py
 License: GPL-3.0-or-later
 Keywords: nhl,api,wrapper,hockey,sports
 Author: Corey Schaf
 Author-email: cschaf@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -86,19 +86,23 @@
 client.games.get_game_content(game_id=2020020001)
 
 # Players
 client.players.get_player(person_id=8477949)
 client.players.get_player_stats(person_id=8477949, season="20222023", stat_type="statsSingleSeason")
 client.players.get_player_stat_types()
 
-# Helpers - Common use cases, data extraction, etc.  For easier dataframe .  These return data that has been parsed
+# Helpers - Common use cases, data extraction, etc.  For easier dataframe initialization.  
+#  These return data that has been parsed
 # out, with some additional calculations as well.
 standings_list = nhl_client.helpers.league_standings(season="20222023")
 standings_df = pd.DataFrame(standings_list)
 standings_df.head(20)
+
+game_results = nhl_client.helpers.get_all_game_results(season="20222023", detailed_game_data=True, game_type="R", team_ids=[7])
+
 ```
 
 
 
 - - - 
 
 As mentioned at the top, I created a notebook to go over some of the available methods in more detail.  Below is an export md of that notebook, with out cell executions.
```

