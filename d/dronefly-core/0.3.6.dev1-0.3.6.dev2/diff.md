# Comparing `tmp/dronefly_core-0.3.6.dev1.tar.gz` & `tmp/dronefly_core-0.3.6.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dronefly_core-0.3.6.dev1.tar", max compression
+gzip compressed data, was "dronefly_core-0.3.6.dev2.tar", max compression
```

## Comparing `dronefly_core-0.3.6.dev1.tar` & `dronefly_core-0.3.6.dev2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    56815 2023-04-16 13:37:18.956988 dronefly_core-0.3.6.dev1/LICENSE
--rw-r--r--   0        0        0      702 2023-01-28 19:16:26.368426 dronefly_core-0.3.6.dev1/README.md
--rw-r--r--   0        0        0       53 2023-01-29 15:27:41.654095 dronefly_core-0.3.6.dev1/dronefly/core/__init__.py
--rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev1/dronefly/core/clients/__init__.py
--rw-r--r--   0        0        0     1028 2023-03-13 15:05:57.725989 dronefly_core-0.3.6.dev1/dronefly/core/clients/inat.py
--rw-r--r--   0        0        0     7532 2023-06-16 17:33:58.906636 dronefly_core-0.3.6.dev1/dronefly/core/commands/__init__.py
--rw-r--r--   0        0        0      635 2023-03-19 08:14:11.111276 dronefly_core-0.3.6.dev1/dronefly/core/constants.py
--rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev1/dronefly/core/formatters/__init__.py
--rw-r--r--   0        0        0      445 2023-04-16 10:53:39.829302 dronefly_core-0.3.6.dev1/dronefly/core/formatters/constants.py
--rw-r--r--   0        0        0    29903 2023-06-03 20:23:10.683148 dronefly_core-0.3.6.dev1/dronefly/core/formatters/generic.py
--rw-r--r--   0        0        0        0 2022-05-23 14:14:52.624333 dronefly_core-0.3.6.dev1/dronefly/core/models/__init__.py
--rw-r--r--   0        0        0     1753 2023-04-09 09:38:32.529718 dronefly_core-0.3.6.dev1/dronefly/core/models/controlled_terms.py
--rw-r--r--   0        0        0      188 2023-03-13 15:15:33.501579 dronefly_core-0.3.6.dev1/dronefly/core/models/user.py
--rw-r--r--   0        0        0       49 2023-01-29 15:28:49.919496 dronefly_core-0.3.6.dev1/dronefly/core/parsers/__init__.py
--rw-r--r--   0        0        0     3721 2023-06-14 15:48:19.092273 dronefly_core-0.3.6.dev1/dronefly/core/parsers/constants.py
--rw-r--r--   0        0        0     9291 2023-02-18 13:51:02.476816 dronefly_core-0.3.6.dev1/dronefly/core/parsers/natural.py
--rw-r--r--   0        0        0     6329 2023-03-19 08:21:31.268129 dronefly_core-0.3.6.dev1/dronefly/core/parsers/unixlike.py
--rw-r--r--   0        0        0     2346 2023-01-29 15:35:29.175688 dronefly_core-0.3.6.dev1/dronefly/core/parsers/url.py
--rw-r--r--   0        0        0       51 2023-01-29 15:27:27.497804 dronefly_core-0.3.6.dev1/dronefly/core/query/__init__.py
--rw-r--r--   0        0        0    19768 2023-06-14 16:36:34.575475 dronefly_core-0.3.6.dev1/dronefly/core/query/query.py
--rw-r--r--   0        0        0      527 2023-06-16 17:08:24.162383 dronefly_core-0.3.6.dev1/dronefly/core/utils/__init__.py
--rw-r--r--   0        0        0      741 2023-06-16 19:09:05.170493 dronefly_core-0.3.6.dev1/pyproject.toml
--rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev1/setup.py
--rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev1/PKG-INFO
+-rw-r--r--   0        0        0    56815 2023-04-16 13:37:18.956988 dronefly_core-0.3.6.dev2/LICENSE
+-rw-r--r--   0        0        0      702 2023-01-28 19:16:26.368426 dronefly_core-0.3.6.dev2/README.md
+-rw-r--r--   0        0        0       53 2023-01-29 15:27:41.654095 dronefly_core-0.3.6.dev2/dronefly/core/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev2/dronefly/core/clients/__init__.py
+-rw-r--r--   0        0        0     1028 2023-03-13 15:05:57.725989 dronefly_core-0.3.6.dev2/dronefly/core/clients/inat.py
+-rw-r--r--   0        0        0     7532 2023-06-16 17:33:58.906636 dronefly_core-0.3.6.dev2/dronefly/core/commands/__init__.py
+-rw-r--r--   0        0        0      635 2023-03-19 08:14:11.111276 dronefly_core-0.3.6.dev2/dronefly/core/constants.py
+-rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev2/dronefly/core/formatters/__init__.py
+-rw-r--r--   0        0        0      445 2023-04-16 10:53:39.829302 dronefly_core-0.3.6.dev2/dronefly/core/formatters/constants.py
+-rw-r--r--   0        0        0    32312 2023-06-18 12:34:06.350900 dronefly_core-0.3.6.dev2/dronefly/core/formatters/generic.py
+-rw-r--r--   0        0        0        0 2022-05-23 14:14:52.624333 dronefly_core-0.3.6.dev2/dronefly/core/models/__init__.py
+-rw-r--r--   0        0        0     1753 2023-04-09 09:38:32.529718 dronefly_core-0.3.6.dev2/dronefly/core/models/controlled_terms.py
+-rw-r--r--   0        0        0      188 2023-03-13 15:15:33.501579 dronefly_core-0.3.6.dev2/dronefly/core/models/user.py
+-rw-r--r--   0        0        0       49 2023-01-29 15:28:49.919496 dronefly_core-0.3.6.dev2/dronefly/core/parsers/__init__.py
+-rw-r--r--   0        0        0     3721 2023-06-14 15:48:19.092273 dronefly_core-0.3.6.dev2/dronefly/core/parsers/constants.py
+-rw-r--r--   0        0        0     9291 2023-02-18 13:51:02.476816 dronefly_core-0.3.6.dev2/dronefly/core/parsers/natural.py
+-rw-r--r--   0        0        0     6329 2023-03-19 08:21:31.268129 dronefly_core-0.3.6.dev2/dronefly/core/parsers/unixlike.py
+-rw-r--r--   0        0        0     2346 2023-01-29 15:35:29.175688 dronefly_core-0.3.6.dev2/dronefly/core/parsers/url.py
+-rw-r--r--   0        0        0       51 2023-01-29 15:27:27.497804 dronefly_core-0.3.6.dev2/dronefly/core/query/__init__.py
+-rw-r--r--   0        0        0    19768 2023-06-17 15:43:08.517165 dronefly_core-0.3.6.dev2/dronefly/core/query/query.py
+-rw-r--r--   0        0        0     1310 2023-06-18 12:34:04.486862 dronefly_core-0.3.6.dev2/dronefly/core/utils/__init__.py
+-rw-r--r--   0        0        0      741 2023-06-18 12:36:24.205752 dronefly_core-0.3.6.dev2/pyproject.toml
+-rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev2/setup.py
+-rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev2/PKG-INFO
```

### Comparing `dronefly_core-0.3.6.dev1/LICENSE` & `dronefly_core-0.3.6.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev1/README.md` & `dronefly_core-0.3.6.dev2/README.md`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev1/dronefly/core/clients/inat.py` & `dronefly_core-0.3.6.dev2/dronefly/core/clients/inat.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev1/dronefly/core/commands/__init__.py` & `dronefly_core-0.3.6.dev2/dronefly/core/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev1/dronefly/core/constants.py` & `dronefly_core-0.3.6.dev2/dronefly/core/constants.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev1/dronefly/core/formatters/generic.py` & `dronefly_core-0.3.6.dev2/dronefly/core/formatters/generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,24 +14,27 @@
 
 import html2markdown
 import inflect
 from pyinaturalist import (
     ConservationStatus,
     EstablishmentMeans,
     JsonResponse,
+    LifeList,
     ListedTaxon,
     Observation,
     Taxon,
     TaxonSummary,
     User,
 )
+from pyinaturalist.constants import COMMON_RANKS
 
 from dronefly.core.constants import (
     TAXON_PRIMARY_RANKS,
     TRINOMIAL_ABBR,
+    RANK_EQUIVALENTS,
     RANK_LEVELS,
 )
 from dronefly.core.formatters.constants import (
     ICONS,
     WWW_BASE_URL,
 )
 from dronefly.core.utils import obs_url_from_v1
@@ -64,14 +67,17 @@
     rf"(?P<markdown>{_MARKDOWN_ESCAPE_SUBREGEX}|{_MARKDOWN_ESCAPE_COMMON})",
     re.MULTILINE,
 )
 _URL_REGEX = r"(?P<url><[^: >]+:\/[^ >]+>|(?:https?|steam):\/\/[^\s<]+[^<.,:;\"\'\]\s])"
 _MARKDOWN_STOCK_REGEX = rf"(?P<markdown>[_\\~|\*`]|{_MARKDOWN_ESCAPE_COMMON})"
 
 p = inflect.engine()
+p.defnoun("phylum", "phyla")
+p.defnoun("subphylum", "subphyla")
+p.defnoun("subgenus", "subgenera")
 
 
 def escape_markdown(
     text: str, *, as_needed: bool = False, ignore_links: bool = True
 ) -> str:
     r"""A helper function that escapes Discord's markdown.
 
@@ -134,14 +140,74 @@
             formatted_time = f"{mon}-{year}"
     else:
         wday = time.strftime("%a")
         formatted_time = f"{wday} {mon} {day}, {year} · {hour}:{minute} {am_pm}"
     return formatted_time
 
 
+def format_life_list_summary(life_list: LifeList, per_rank: str, taxon: Taxon):
+    ranks = None
+    rank_totals = {}
+    if per_rank in ["main", "any"]:
+        ranks_to_count = (
+            COMMON_RANKS[-8:] if per_rank == "main" else list(RANK_LEVELS.keys())
+        )
+        if taxon:
+            if per_rank == "main" and taxon.rank not in ranks_to_count:
+                rank_level = RANK_LEVELS[taxon.rank]
+                ranks_to_count = [
+                    rank for rank in ranks_to_count if RANK_LEVELS[rank] < rank_level
+                ]
+                ranks_to_count.append(taxon.rank)
+            else:
+                ranks_to_count = ranks_to_count[: ranks_to_count.index(taxon.rank) + 1]
+        ranks = "main ranks" if per_rank == "main" else "ranks"
+        taxa = [
+            life_list_taxon
+            for life_list_taxon in life_list.data
+            if life_list_taxon.rank in ranks_to_count
+        ]
+        tot = {}
+        for taxon in taxa:
+            rank = taxon.rank
+            tot[rank] = tot.get(taxon.rank, 0) + 1
+        max_digits = len(str(max(tot.values())))
+        rank_totals = {
+            rank: f"`{str(tot[rank]).rjust(max_digits)}` {p.plural_noun(rank, tot[rank])}"
+            for rank in tot
+        }
+    elif per_rank == "leaf":
+        ranks = "leaf taxa"
+        taxa = [
+            life_list_taxon
+            for life_list_taxon in life_list.data
+            if life_list_taxon.direct_obs_count == life_list_taxon.descendant_obs_count
+        ]
+    else:
+        rank = RANK_EQUIVALENTS[per_rank] if per_rank in RANK_EQUIVALENTS else per_rank
+        ranks = p.plural_noun(rank)
+        taxa = [
+            life_list_taxon
+            for life_list_taxon in life_list.data
+            if life_list_taxon.rank == rank
+        ]
+    total = f"Total: {len(taxa)} {ranks}"
+    if rank_totals:
+        rank_keys = reversed(
+            [rank for rank in RANK_LEVELS.keys() if rank != "stateofmatter"]
+        )
+        rank_totals_by_rank = [
+            rank_totals[rank] for rank in rank_keys if rank_totals.get(rank)
+        ]
+        response = "\n\n".join(["\n".join(rank_totals_by_rank), total])
+    else:
+        response = total
+    return response
+
+
 def format_user_name(user: User):
     """Format user's display name with Markdown special characters escaped."""
     if user.name:
         return f"{escape_markdown(user.name)} ({escape_markdown(user.login)})"
     return escape_markdown(user.login)
 
 
@@ -810,30 +876,30 @@
             media_counts += self.format_count("sound", len(self.obs.sounds))
         return media_counts
 
 
 class QualifiedTaxonFormatter(TaxonFormatter):
     def __init__(
         self,
-        query_response: QueryResponse,
+        query_response: "QueryResponse",
         observations: JsonResponse = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.query_response = query_response
         self.observations = observations
         self.obs_count_formatter = self.ObsCountFormatter(
             query_response.taxon, query_response, observations
         )
 
     class ObsCountFormatter(TaxonFormatter.ObsCountFormatter):
         def __init__(
             self,
             taxon: Taxon,
-            query_response: QueryResponse = None,
+            query_response: "QueryResponse" = None,
             observations: JsonResponse = None,
         ):
             super().__init__(taxon)
             self.query_response = query_response
             self.observations = observations
 
         def count(self):
```

### Comparing `dronefly_core-0.3.6.dev1/dronefly/core/models/controlled_terms.py` & `dronefly_core-0.3.6.dev2/dronefly/core/models/controlled_terms.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev1/dronefly/core/parsers/constants.py` & `dronefly_core-0.3.6.dev2/dronefly/core/parsers/constants.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev1/dronefly/core/parsers/natural.py` & `dronefly_core-0.3.6.dev2/dronefly/core/parsers/natural.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev1/dronefly/core/parsers/unixlike.py` & `dronefly_core-0.3.6.dev2/dronefly/core/parsers/unixlike.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev1/dronefly/core/parsers/url.py` & `dronefly_core-0.3.6.dev2/dronefly/core/parsers/url.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev1/dronefly/core/query/query.py` & `dronefly_core-0.3.6.dev2/dronefly/core/query/query.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev1/pyproject.toml` & `dronefly_core-0.3.6.dev2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 exclude_dirs = ["tests"]
 
 [tool.flake8]
 max-line-length = 100
 
 [tool.poetry]
 name = "dronefly-core"
-version = "0.3.6.dev1"
+version = "0.3.6.dev2"
 description = "Core dronefly components"
 authors = ["Ben Armstrong <synrg@debian.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 packages = [
 	{ include = "dronefly/core" },
 ]
```

### Comparing `dronefly_core-0.3.6.dev1/setup.py` & `dronefly_core-0.3.6.dev2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'html2markdown>=0.1.7,<0.2.0',
  'inflect>=5.3.0,<6.0.0',
  'pyinaturalist>=0.19.0.dev2,<0.20',
  'rich>=10.9,<14']
 
 setup_kwargs = {
     'name': 'dronefly-core',
-    'version': '0.3.6.dev1',
+    'version': '0.3.6.dev2',
     'description': 'Core dronefly components',
     'long_description': "# Dronefly core\n\nThis is an incomplete rewrite of [Dronefly](https://dronefly.readthedocs.io)\nDiscord bot's core components. We're not yet making version guarantees until\nit is more usable.\n\n# Related packages\n\n## Dronefly command-line client\n\nThe [dronefly-cli](https://github.com/dronefly-garden/dronefly-cli) command-line\nclient will provide a standalone text user interface that can perform a usable\nsubset of Dronefly Discord bot's capabilities, built solely with Dronefly core.\n\n## Dronefly Discord bot\n\nDronefly Discord bot brings [iNaturalist](https://www.inaturalist.org) taxa,\nobservations, and other data from the site into conversations on the\n[Discord](https://discord.com) chat platform.\n",
     'author': 'Ben Armstrong',
     'author_email': 'synrg@debian.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dronefly_core-0.3.6.dev1/PKG-INFO` & `dronefly_core-0.3.6.dev2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dronefly-core
-Version: 0.3.6.dev1
+Version: 0.3.6.dev2
 Summary: Core dronefly components
 License: AGPL-3.0-or-later
 Author: Ben Armstrong
 Author-email: synrg@debian.org
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

