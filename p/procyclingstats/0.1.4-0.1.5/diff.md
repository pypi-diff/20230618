# Comparing `tmp/procyclingstats-0.1.4.tar.gz` & `tmp/procyclingstats-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "procyclingstats-0.1.4.tar", last modified: Wed Mar  1 15:42:57 2023, max compression
+gzip compressed data, was "procyclingstats-0.1.5.tar", last modified: Sun Jun 18 12:21:46 2023, max compression
```

## Comparing `procyclingstats-0.1.4.tar` & `procyclingstats-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 madzin    (1000) madzin    (1000)        0 2023-03-01 15:42:57.258121 procyclingstats-0.1.4/
--rw-r--r--   0 madzin    (1000) madzin    (1000)     2314 2023-03-01 15:42:57.258121 procyclingstats-0.1.4/PKG-INFO
--rw-r--r--   0 madzin    (1000) madzin    (1000)     1461 2023-03-01 15:40:14.000000 procyclingstats-0.1.4/README.rst
-drwxr-xr-x   0 madzin    (1000) madzin    (1000)        0 2023-03-01 15:42:57.247361 procyclingstats-0.1.4/procyclingstats/
--rw-r--r--   0 madzin    (1000) madzin    (1000)      599 2023-02-26 10:28:41.000000 procyclingstats-0.1.4/procyclingstats/__init__.py
--rw-r--r--   0 madzin    (1000) madzin    (1000)     3744 2023-02-26 10:28:41.000000 procyclingstats-0.1.4/procyclingstats/__main__.py
--rw-r--r--   0 madzin    (1000) madzin    (1000)     1304 2023-02-26 10:28:41.000000 procyclingstats-0.1.4/procyclingstats/errors.py
--rw-r--r--   0 madzin    (1000) madzin    (1000)     4709 2023-02-26 10:28:41.000000 procyclingstats-0.1.4/procyclingstats/race_climbs_scraper.py
--rw-r--r--   0 madzin    (1000) madzin    (1000)     6868 2023-02-26 10:28:41.000000 procyclingstats-0.1.4/procyclingstats/race_scraper.py
--rw-r--r--   0 madzin    (1000) madzin    (1000)     5749 2023-02-26 10:28:41.000000 procyclingstats-0.1.4/procyclingstats/race_startlist_scraper.py
--rw-r--r--   0 madzin    (1000) madzin    (1000)    20338 2023-02-26 10:28:41.000000 procyclingstats-0.1.4/procyclingstats/ranking_scraper.py
--rw-r--r--   0 madzin    (1000) madzin    (1000)     9645 2023-02-28 13:47:45.000000 procyclingstats-0.1.4/procyclingstats/rider_results_scraper.py
--rw-r--r--   0 madzin    (1000) madzin    (1000)     7537 2023-02-26 10:28:41.000000 procyclingstats-0.1.4/procyclingstats/rider_scraper.py
--rw-r--r--   0 madzin    (1000) madzin    (1000)     8183 2023-02-28 13:49:20.000000 procyclingstats-0.1.4/procyclingstats/scraper.py
--rw-r--r--   0 madzin    (1000) madzin    (1000)    24647 2023-03-01 15:29:52.000000 procyclingstats-0.1.4/procyclingstats/stage_scraper.py
--rw-r--r--   0 madzin    (1000) madzin    (1000)    14918 2023-02-26 10:28:41.000000 procyclingstats-0.1.4/procyclingstats/table_parser.py
--rw-r--r--   0 madzin    (1000) madzin    (1000)     9649 2023-02-26 10:28:41.000000 procyclingstats-0.1.4/procyclingstats/team_scraper.py
--rw-r--r--   0 madzin    (1000) madzin    (1000)    10976 2023-02-28 13:37:16.000000 procyclingstats-0.1.4/procyclingstats/utils.py
-drwxr-xr-x   0 madzin    (1000) madzin    (1000)        0 2023-03-01 15:42:57.256774 procyclingstats-0.1.4/procyclingstats.egg-info/
--rw-r--r--   0 madzin    (1000) madzin    (1000)     2314 2023-03-01 15:42:57.000000 procyclingstats-0.1.4/procyclingstats.egg-info/PKG-INFO
--rw-r--r--   0 madzin    (1000) madzin    (1000)      676 2023-03-01 15:42:57.000000 procyclingstats-0.1.4/procyclingstats.egg-info/SOURCES.txt
--rw-r--r--   0 madzin    (1000) madzin    (1000)        1 2023-03-01 15:42:57.000000 procyclingstats-0.1.4/procyclingstats.egg-info/dependency_links.txt
--rw-r--r--   0 madzin    (1000) madzin    (1000)       20 2023-03-01 15:42:57.000000 procyclingstats-0.1.4/procyclingstats.egg-info/requires.txt
--rw-r--r--   0 madzin    (1000) madzin    (1000)       16 2023-03-01 15:42:57.000000 procyclingstats-0.1.4/procyclingstats.egg-info/top_level.txt
--rw-r--r--   0 madzin    (1000) madzin    (1000)      108 2023-03-01 15:42:57.261201 procyclingstats-0.1.4/setup.cfg
--rw-r--r--   0 madzin    (1000) madzin    (1000)      669 2023-03-01 15:42:54.000000 procyclingstats-0.1.4/setup.py
+drwxr-xr-x   0 madzin    (1000) madzin    (1000)        0 2023-06-18 12:21:46.403038 procyclingstats-0.1.5/
+-rw-r--r--   0 madzin    (1000) madzin    (1000)     2991 2023-06-18 12:21:46.404003 procyclingstats-0.1.5/PKG-INFO
+-rw-r--r--   0 madzin    (1000) madzin    (1000)     2042 2023-03-01 16:18:11.000000 procyclingstats-0.1.5/README.rst
+drwxr-xr-x   0 madzin    (1000) madzin    (1000)        0 2023-06-18 12:21:46.394209 procyclingstats-0.1.5/procyclingstats/
+-rw-r--r--   0 madzin    (1000) madzin    (1000)      599 2023-02-26 10:28:41.000000 procyclingstats-0.1.5/procyclingstats/__init__.py
+-rw-r--r--   0 madzin    (1000) madzin    (1000)     4235 2023-06-18 10:18:30.000000 procyclingstats-0.1.5/procyclingstats/__main__.py
+-rw-r--r--   0 madzin    (1000) madzin    (1000)     1304 2023-02-26 10:28:41.000000 procyclingstats-0.1.5/procyclingstats/errors.py
+-rw-r--r--   0 madzin    (1000) madzin    (1000)     3460 2023-06-18 10:26:43.000000 procyclingstats-0.1.5/procyclingstats/race_climbs_scraper.py
+-rw-r--r--   0 madzin    (1000) madzin    (1000)     6604 2023-06-17 19:29:12.000000 procyclingstats-0.1.5/procyclingstats/race_scraper.py
+-rw-r--r--   0 madzin    (1000) madzin    (1000)     4567 2023-06-17 17:21:57.000000 procyclingstats-0.1.5/procyclingstats/race_startlist_scraper.py
+-rw-r--r--   0 madzin    (1000) madzin    (1000)    19273 2023-06-17 17:23:51.000000 procyclingstats-0.1.5/procyclingstats/ranking_scraper.py
+-rw-r--r--   0 madzin    (1000) madzin    (1000)     8398 2023-06-17 17:23:38.000000 procyclingstats-0.1.5/procyclingstats/rider_results_scraper.py
+-rw-r--r--   0 madzin    (1000) madzin    (1000)     6870 2023-06-17 17:25:09.000000 procyclingstats-0.1.5/procyclingstats/rider_scraper.py
+-rw-r--r--   0 madzin    (1000) madzin    (1000)     6517 2023-06-17 17:22:57.000000 procyclingstats-0.1.5/procyclingstats/scraper.py
+-rw-r--r--   0 madzin    (1000) madzin    (1000)    23754 2023-06-18 11:20:14.000000 procyclingstats-0.1.5/procyclingstats/stage_scraper.py
+-rw-r--r--   0 madzin    (1000) madzin    (1000)    15221 2023-06-18 11:09:12.000000 procyclingstats-0.1.5/procyclingstats/table_parser.py
+-rw-r--r--   0 madzin    (1000) madzin    (1000)     9053 2023-06-17 17:24:59.000000 procyclingstats-0.1.5/procyclingstats/team_scraper.py
+-rw-r--r--   0 madzin    (1000) madzin    (1000)     6364 2023-06-17 17:25:32.000000 procyclingstats-0.1.5/procyclingstats/utils.py
+drwxr-xr-x   0 madzin    (1000) madzin    (1000)        0 2023-06-18 12:21:46.401969 procyclingstats-0.1.5/procyclingstats.egg-info/
+-rw-r--r--   0 madzin    (1000) madzin    (1000)     2991 2023-06-18 12:21:46.000000 procyclingstats-0.1.5/procyclingstats.egg-info/PKG-INFO
+-rw-r--r--   0 madzin    (1000) madzin    (1000)      676 2023-06-18 12:21:46.000000 procyclingstats-0.1.5/procyclingstats.egg-info/SOURCES.txt
+-rw-r--r--   0 madzin    (1000) madzin    (1000)        1 2023-06-18 12:21:46.000000 procyclingstats-0.1.5/procyclingstats.egg-info/dependency_links.txt
+-rw-r--r--   0 madzin    (1000) madzin    (1000)       20 2023-06-18 12:21:46.000000 procyclingstats-0.1.5/procyclingstats.egg-info/requires.txt
+-rw-r--r--   0 madzin    (1000) madzin    (1000)       16 2023-06-18 12:21:46.000000 procyclingstats-0.1.5/procyclingstats.egg-info/top_level.txt
+-rw-r--r--   0 madzin    (1000) madzin    (1000)      108 2023-06-18 12:21:46.405004 procyclingstats-0.1.5/setup.cfg
+-rw-r--r--   0 madzin    (1000) madzin    (1000)      669 2023-06-18 12:21:30.000000 procyclingstats-0.1.5/setup.py
```

### Comparing `procyclingstats-0.1.4/PKG-INFO` & `procyclingstats-0.1.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: procyclingstats
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python API wrapper for procyclingstats.com
 Home-page: https://github.com/themm1/procyclingstats
 Author: Martin Madzin
 Author-email: madzin.m@gmail.com
 License: MIT
 Description: procyclingstats
         ===============
@@ -49,22 +49,34 @@
         
         Interface consists from scraping classes which are currently ``Race``,
         ``RaceStartlist``, ``RaceClimbs``, ``Ranking``, ``Rider``, ``RiderResults``,
         ``Stage`` and ``Team``. Usage of all scraping classes is almost the same and
         the only difference among them are parsing methods as is for example
         ``birthdate`` in Rider class usage example.
         
+        Unexpected behaviour and parsing errors
+        ---------------------------------------
+        
+        Since the project is a web scraper which parses HTML, it's difficult to make
+        it reliable and it's common to encounter some HTML parsing problems. After
+        getting some kind of unexpected behaviour or parsing errors, it's recommended
+        to update the package on your system using
+        ``pip install procyclingstats --upgrade``. If the problem proceeds, see the
+        GitHub issues_ page and if the issue hasn't been opened yet, don't hesitate to
+        open one!
+        
         Links
         -----
         
         - GitHub_
         - PyPI_
         - Documentation_
         
         .. _GitHub: https://github.com/themm1/procyclingstats
         .. _PyPI: https://pypi.org/project/procyclingstats
         .. _Documentation: https://procyclingstats.readthedocs.io/en/latest
         .. _procyclingstats.com: https://www.procyclingstats.com
         .. _selectolax: https://github.com/rushter/selectolax
+        .. _issues: https://github.com/themm1/procyclingstats/issues
 Keywords: cycling cycling-stats procyclingstats scraper html-parsing sports-analytics
 Platform: UNKNOWN
 Description-Content-Type: text/x-rst
```

### Comparing `procyclingstats-0.1.4/README.rst` & `procyclingstats-0.1.5/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -41,19 +41,31 @@
 
 Interface consists from scraping classes which are currently ``Race``,
 ``RaceStartlist``, ``RaceClimbs``, ``Ranking``, ``Rider``, ``RiderResults``,
 ``Stage`` and ``Team``. Usage of all scraping classes is almost the same and
 the only difference among them are parsing methods as is for example
 ``birthdate`` in Rider class usage example.
 
+Unexpected behaviour and parsing errors
+---------------------------------------
+
+Since the project is a web scraper which parses HTML, it's difficult to make
+it reliable and it's common to encounter some HTML parsing problems. After
+getting some kind of unexpected behaviour or parsing errors, it's recommended
+to update the package on your system using
+``pip install procyclingstats --upgrade``. If the problem proceeds, see the
+GitHub issues_ page and if the issue hasn't been opened yet, don't hesitate to
+open one!
+
 Links
 -----
 
 - GitHub_
 - PyPI_
 - Documentation_
 
 .. _GitHub: https://github.com/themm1/procyclingstats
 .. _PyPI: https://pypi.org/project/procyclingstats
 .. _Documentation: https://procyclingstats.readthedocs.io/en/latest
 .. _procyclingstats.com: https://www.procyclingstats.com
-.. _selectolax: https://github.com/rushter/selectolax
+.. _selectolax: https://github.com/rushter/selectolax
+.. _issues: https://github.com/themm1/procyclingstats/issues
```

### Comparing `procyclingstats-0.1.4/procyclingstats/__init__.py` & `procyclingstats-0.1.5/procyclingstats/__init__.py`

 * *Files identical despite different names*

### Comparing `procyclingstats-0.1.4/procyclingstats/errors.py` & `procyclingstats-0.1.5/procyclingstats/errors.py`

 * *Files identical despite different names*

### Comparing `procyclingstats-0.1.4/procyclingstats/race_scraper.py` & `procyclingstats-0.1.5/procyclingstats/race_scraper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,35 @@
 from typing import Any, Dict, List
 
-from .errors import ExpectedParsingError
+from .errors import ExpectedParsingError, UnexpectedParsingError
 from .scraper import Scraper
 from .table_parser import TableParser
-from .utils import (format_regex_str, get_day_month, normalize_race_url,
-                    parse_select, parse_table_fields_args, reg)
+from .utils import get_day_month, parse_select, parse_table_fields_args
 
 
 class Race(Scraper):
     """
     Scraper for race overview HTML page.
 
     Usage:
 
     >>> from procyclingstats import Race
-    >>> race = Race("race/tour-de-france/2022/overview")
+    >>> race = Race("race/tour-de-france/2022")
     >>> race.enddate()
     '2022-07-24'
     >>> race.parse()
     {
         'category': 'Men Elite',
         'edition': 109,
         'enddate': '2022-07-24',
         'is_one_day_race': False,
         ...
     }
 
     """
-    _url_validation_regex = format_regex_str(
-    f"""
-        {reg.base_url}?race{reg.url_str}
-        (({reg.year}{reg.stage}{reg.overview}{reg.anything}?)|
-        ({reg.year}{reg.result}?{reg.overview}{reg.anything}?)|
-        {reg.overview}{reg.anything}?)
-        \\/*
-    """)
-    """Regex for validating race overview URL."""
-
-    def normalized_relative_url(self) -> str:
-        """
-        Creates normalized relative URL. Determines equality of objects (is
-        used in __eq__ method).
-
-        :return: Normalized URL in ``race/{race_id}/{year}/overview`` format.
-            When year isn't contained in user defined URL, year is skipped.
-        """
-        return normalize_race_url(self._decompose_url(), "overview")
-
     def year(self) -> int:
         """
         Parse year when the race occured from HTML.
 
         :return: Year when the race occured.
         """
         return int(self.html.css_first("span.hideIfMobile").text())
@@ -66,16 +45,20 @@
 
     def is_one_day_race(self) -> bool:
         """
         Parses whether race is one day race from HTML.
 
         :return: Whether given race is one day race.
         """
-        one_day_race_html = self.html.css_first("div.sub > span.blue")
-        return "stage" not in one_day_race_html.text().lower()
+        titles = self.html.css("div > div > h3")
+        titles = [] if not titles else titles
+        for title_html in titles:
+            if "Stages" in title_html.text():
+                return False
+        return True
 
     def nationality(self) -> str:
         """
         Parses race nationality from HTML.
 
         :return: 2 chars long country code in uppercase.
         """
@@ -147,55 +130,66 @@
         """
         Parses race stages from HTML (available only on stage races). When
         race is one day race, empty list is returned.
 
         :param args: Fields that should be contained in returned table. When
             no args are passed, all fields are parsed.
 
+            - rider_url: Winner's URL.
+            - rider_name: Winner's name.
+            - nationality: Winner's nationality as 2 chars long country code.
             - date: Date when the stage occured in ``MM-DD`` format.
             - profile_icon: Profile icon of the stage (p1, p2, ... p5).
             - stage_name: Name of the stage, e.g \
                 ``Stage 2 | Roskilde - Nyborg``.
             - stage_url: URL of the stage, e.g. \
                 ``race/tour-de-france/2022/stage-2``.
-            - distance: Stage distance in KMs as float.
 
         :raises ValueError: When one of args is of invalid value.
         :return: Table with wanted fields.
         """
         available_fields = (
             "date",
             "profile_icon",
             "stage_name",
             "stage_url",
-            "distance"
+            "rider_url",
+            "rider_name",
+            "nationality"
         )
         if self.is_one_day_race():
             return []
 
         fields = parse_table_fields_args(args, available_fields)
-        casual_fields = (
-            "profile_icon",
-            "stage_name",
-            "stage_url"
-        )
-        stages_table_html = self.html.css_first("div.mt20 ul.list")
+        stages_table_html = self.html.css_first("div:not(.mg_r2) > div > \
+            span > table.basic")
+        if not stages_table_html:
+            return []
         # remove rest day table rows
-        for stage_e in stages_table_html.css("li"):
-            dist = stage_e.css_first("div:nth-child(5)").text()
-            if not dist:
+        for stage_e in stages_table_html.css("tr"):
+            not_p_icon = stage_e.css_first(".icon.profile.p")
+            if not_p_icon:
                 stage_e.remove()
 
         table_parser = TableParser(stages_table_html)
-        casual_f_to_parse = [f for f in fields if f in casual_fields]
-        if casual_fields:
+        casual_f_to_parse = [f for f in fields if f != "date"]
+        try:
             table_parser.parse(casual_f_to_parse)
+        # if nationalities don't fit stages winners
+        except UnexpectedParsingError:
+            casual_f_to_parse.remove("nationality")
+            table_parser.parse(casual_f_to_parse)
+            nats = table_parser.nationality()
+            j = 0
+            for i in range(len(table_parser.table)):
+                if j < len(nats) and \
+                    table_parser.table[i]['rider_url'].split("/")[1]:
+                    table_parser.table[i]['nationality'] = nats[j]
+                    j += 1
+                else:
+                    table_parser.table[i]['nationality'] = None
+
         # add stages dates to table if neede
         if "date" in fields:
             dates = table_parser.parse_extra_column(0, get_day_month)
             table_parser.extend_table("date", dates)
-        # add distances to table if needed
-        if "distance" in fields:
-            distances = table_parser.parse_extra_column(4, lambda x:
-                float(x.split("k")[0].replace("(", "")) if x else None)
-            table_parser.extend_table("distance", distances)
         return table_parser.table
```

### Comparing `procyclingstats-0.1.4/procyclingstats/race_startlist_scraper.py` & `procyclingstats-0.1.5/procyclingstats/race_startlist_scraper.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Any, Dict, List
 
 from .scraper import Scraper
 from .table_parser import TableParser
-from .utils import (format_regex_str, normalize_race_url,
-                    parse_table_fields_args, reg)
+from .utils import parse_table_fields_args
 
 
 class RaceStartlist(Scraper):
     """
     Scraper for race startlist HTML page.
 
     Usage:
@@ -24,120 +23,92 @@
             'team_name': 'UAE Team Emirates',
             'team_url': 'team/uae-team-emirates-2022'}
         },
         ...
     ]
     >>> race_startlist.parse()
     {
-        'normalized_relative_url': 'race/tour-de-france/2022/startlist',
         'startlist': [
             {
                 'nationality': 'SI',
                 'rider_name': 'POGAČAR Tadej',
                 'rider_number': 1,
                 'rider_url': 'rider/tadej-pogacar',
                 'team_name': 'UAE Team Emirates',
                 'team_url': 'team/uae-team-emirates-2022'}
             },
             ...
         ]
     }
     """
-    _url_validation_regex = format_regex_str(
-    f"""
-        {reg.base_url}?race{reg.url_str}
-        (({reg.year}{reg.stage}{reg.startlist}{reg.anything}?)|
-        ({reg.year}{reg.result}?{reg.startlist}{reg.anything}?)|
-        {reg.startlist}{reg.anything}?)
-        \\/*
-    """)
-    """Regex for validating race startlist URL."""
-
-    def normalized_relative_url(self) -> str:
-        """
-        Creates normalized relative URL. Determines equality of objects (is
-        used in __eq__ method).
-
-        :return: Normalized URL in ``race/{race_id}/{year}/startlist`` format.
-            When year isn't contained in user defined URL, year is skipped.
-        """
-        return normalize_race_url(self._decompose_url(), "startlist")
-
     def startlist(self, *args: str) -> List[Dict[str, Any]]:
         """
         Parses startlist from HTML. When startlist is individual (without
         teams) fields team name, team url and rider nationality are set to
         None.
 
         :param args: Fields that should be contained in returned table. When
             no args are passed, all fields are parsed.
 
             - rider_name:
             - rider_url:
             - team_name:
             - team_url:
             - nationality: Rider's nationality as 2 chars long country code.
-            - rider_number: Rider's ID number in the race.
+            - rider_number: Rider's ID number in the race. For races without
+                numbered participants (e.g. the ones that haven't occured yet)
+                is every rider's ID None.
 
         :raises ValueError: When one of args is of invalid value.
         :return: Table with wanted fields.
         """
         available_fields = (
             "rider_name",
             "rider_url",
             "team_name",
             "team_url",
             "nationality",
             "rider_number"
         )
         fields = parse_table_fields_args(args, available_fields)
-        startlist_html = self.html.css_first(".startlist_v3")
-        # startlist is individual startlist e.g.
-        # race/tour-de-pologne/2009/gc/startlist
-        if startlist_html.css_first("li.team") is None:
-            startlist_html = self.html.css_first(".page-content > div")
-            startlist_table = []
-            for i, rider_a in enumerate(startlist_html.css("a:not([class])")):
-                startlist_table.append({})
-                for field in fields:
-                    startlist_table[-1][field] = None
-
-                if "rider_url" in fields:
-                    startlist_table[-1]['rider_url'] = rider_a.\
-                        attributes['href']
-                if "rider_name" in fields:
-                    startlist_table[-1]['rider_name'] = rider_a.text()
-                if "rider_number" in fields:
-                    startlist_table[-1]['rider_number'] = i + 1
-                if "team_name" in fields:
-                    startlist_table[-1]['team_name'] = None
-                if "team_url" in fields:
-                    startlist_table[-1]['team_url'] = None
-                if "nationality" in fields:
-                    startlist_table[-1]['nationality'] = None
-            return startlist_table
+        startlist_html = self.html.css_first("table.basic")
+
+        # if startlist is a table
+        if startlist_html:
+            startlist_parser = TableParser(startlist_html)
+            casual_fields = [f for f in fields if f != "rider_number"]
+            startlist_parser.parse(casual_fields)
+            # adds rider number to table if needed
+            if "rider_number" in fields:
+                numbers = startlist_parser.parse_extra_column(0,
+                    lambda x: int(x) if x else None)
+                startlist_parser.extend_table("rider_number", numbers)
+            return startlist_parser.table
 
         casual_rider_fields = [
             "rider_name",
             "rider_url",
             "nationality"
         ]
-
         table = []
-        for team_html in startlist_html.css("li.team"):
+        startlist_html = self.html.css_first(".startlist_v4")
+        for team_html in startlist_html.css(".ridersCont"):
             riders_table = team_html.css_first("ul")
             table_parser = TableParser(riders_table)
             rider_f_to_parse = [f for f in casual_rider_fields if f in fields]
             table_parser.parse(rider_f_to_parse)
             # add rider numbers to the table if needed
             if "rider_number" in fields:
                 numbers = []
-                for row in riders_table.css("li"):
+                for row in riders_table.css("li > .bib"):
                     num = row.text(deep=False).split(" ")[0]
-                    numbers.append(int(num))
+                    if num.isnumeric():
+                        numbers.append(int(num))
+                    else:
+                        numbers.append(None)
                 table_parser.extend_table("rider_number", numbers)
             # add team names to the table if needed
             if "team_name" in fields:
                 team_name = team_html.css_first("a").text()
                 team_names = [team_name for _ in range(
                     len(table_parser.table))]
                 table_parser.extend_table("team_name", team_names)
```

### Comparing `procyclingstats-0.1.4/procyclingstats/ranking_scraper.py` & `procyclingstats-0.1.5/procyclingstats/ranking_scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Any, Dict, List, Literal, Tuple
 
 from .errors import ExpectedParsingError
 from .scraper import Scraper
 from .table_parser import TableParser
-from .utils import (format_url_filter, parse_select, parse_table_fields_args,
-                    reg, select_menu_by_name)
+from .utils import parse_select, parse_table_fields_args, select_menu_by_name
 
 
 class Ranking(Scraper):
     """
     Scraper for rankings HTML page.
 
     Always only one parsing method that parses ranking is availabe, the others
@@ -56,38 +55,14 @@
             },
             ...
         ],
         'individual_wins_ranking': None,
         ...
     }
     """
-
-    _url_validation_regex = f"{reg.base_url}?rankings.*\\/*"
-    """Regex for validating ranking URL."""
-
-    def normalized_relative_url(self) -> str:
-        """
-        Creates normalized relative URL. Determines equality of objects (is
-        used in `__eq__` method). Ranking objects are equal when both have same
-        URL or filter values are the same (empty filter values don't count).
-
-        :return: Formatted relative URL or filter URL without uneccessary
-            fields e.g. \
-            ``rankings.php?date=2021-12-31&p=we&s=season-individual``.
-        """
-        relative_url = self.relative_url()
-        # returns special normalized ranking filter URL
-        if "?" in relative_url:
-            return format_url_filter(relative_url)
-        decomposed_url = self._decompose_url()
-        # remove .php from rankings URL if it is not a filter URL
-        if "." in decomposed_url[0]:
-            decomposed_url[0] = decomposed_url[0].split(".")[0]
-        return "/".join(decomposed_url)
-
     def individual_ranking(self, *args: str) -> List[Dict[str, Any]]:
         """
         Parses individual ranking from HTML.
 
         :param args: Fields that should be contained in returned table. When
             no args are passed, all fields are parsed.
```

### Comparing `procyclingstats-0.1.4/procyclingstats/rider_results_scraper.py` & `procyclingstats-0.1.5/procyclingstats/rider_results_scraper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Any, Dict, List
 
 from .errors import ExpectedParsingError
 from .scraper import Scraper
 from .table_parser import TableParser
-from .utils import (format_regex_str, format_url_filter, parse_select,
-                    parse_table_fields_args, reg, select_menu_by_name)
+from .utils import parse_select, parse_table_fields_args, select_menu_by_name
 
 
 class RiderResults(Scraper):
     """
     Scraper for rider results HTML page.
 
     Supported is besides of default results table also final 5k results table
@@ -46,30 +45,17 @@
                 'stage_name': 'Vuelta a España | Stage 20',
                 'stage_url': 'race/vuelta-a-espana/2017/stage-20',
                 'vertical_meters': 590},
             },
             ...
         ],
         'nations_select': None,
-        'normalized_relative_url': 'rider/alberto-contador/results/final-5k-analysis',
         ...
     }
     """
-    _url_validation_regex = format_regex_str(
-    f"""
-        {reg.base_url}?
-        (rider.php\\?.*
-        \\/*
-        |
-        rider
-        {reg.url_str}\\/*results{reg.anything}?
-        \\/*)
-    """)
-    """regex for validating rider results url."""
-
     def _html_valid(self) -> bool:
         """
         Extends Scraper method for validating HTMLs.
 
         :return: True if given HTML is valid, otherwise False
         """
         try:
@@ -77,34 +63,14 @@
             page_title = self.html.css_first(".page-content > h2").text()
             assert page_title in ("All results",
                 "Top results final 5k analysis")
             return True
         except AssertionError:
             return False
 
-    def normalized_relative_url(self) -> str:
-        """
-        Creates normalized relative URL. Determines equality of objects (is
-        used in `__eq__` method). Rider results objects are equal when both have
-        same URL or filter values are the same (empty filter values don't
-        count).
-
-        :return: normalized filter URL or URL in ``rider/{rider_id}/results``
-            format
-        """
-        relative_url = self.relative_url()
-        if "?" in relative_url:
-            return format_url_filter(relative_url)
-        decomposed_url = self._decompose_url()
-        rider_id = decomposed_url[1]
-        if (len(decomposed_url) >= 4 and
-                decomposed_url[3] == "final-5k-analysis"):
-            return f"rider/{rider_id}/results/final-5k-analysis"
-        return f"rider/{rider_id}/results"
-
     def _set_up_html(self):
         """Overrides Scraper method. Removes last table row with sum stats."""
         results_table_html = self.html.css_first("table")
         if not results_table_html:
             return
         for row in results_table_html.css("tr"):
             if "class" in row.attributes and row.attributes['class'] == "sum":
```

### Comparing `procyclingstats-0.1.4/procyclingstats/rider_scraper.py` & `procyclingstats-0.1.5/procyclingstats/rider_scraper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import calendar
 from typing import Any, Dict, List
 
 from .scraper import Scraper
 from .table_parser import TableParser
-from .utils import (format_regex_str, get_day_month, parse_table_fields_args,
-                    reg)
+from .utils import get_day_month, parse_table_fields_args
 
 
 class Rider(Scraper):
     """
     Scraper for rider HTML page.
 
     Usage:
@@ -22,34 +21,14 @@
         'birthdate': '1998-9-21',
         'height': 1.76,
         'name': 'Tadej  Pogačar',
         'nationality': 'SI',
         ...
     }
     """
-    _url_validation_regex = format_regex_str(
-    f"""
-        {reg.base_url}?rider
-        {reg.url_str}({reg.overview}{reg.anything}?|
-        {reg.year}{reg.anything}?)?
-        \\/*
-    """)
-    """Regex for validating rider URL."""
-
-    def normalized_relative_url(self) -> str:
-        """
-        Creates normalized relative URL. Determines equality of objects (is
-        used in __eq__ method).
-
-        :return: Normalized URL in ``rider/{rider_id}`` format.
-        """
-        decomposed_url = self._decompose_url()
-        rider_id = decomposed_url[1]
-        return f"rider/{rider_id}"
-
     def birthdate(self) -> str:
         """
         Parses rider's birthdate from HTML.
 
         :return: birthday of the rider in ``YYYY-MM-DD`` format.
         """
         general_info_html = self.html.css_first(".rdr-info-cont")
```

### Comparing `procyclingstats-0.1.4/procyclingstats/scraper.py` & `procyclingstats-0.1.5/procyclingstats/scraper.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,46 @@
 import inspect
 from typing import Any, Callable, Dict, List, Optional, Tuple, Type
 
 import requests
 from selectolax.parser import HTMLParser
 
-from .errors import ExpectedParsingError, ParsedValueInvalidError
-from .utils import validate_string
+from .errors import ExpectedParsingError
 
 
 class Scraper:
     """Base class for all scraping classes."""
     BASE_URL: str = "https://www.procyclingstats.com/"
 
     _public_nonparsing_methods = (
         "update_html",
         "parse",
         "relative_url"
     )
     """Public methods that aren't called by `parse` method."""
 
-    _url_validation_regex = ".*"
-    """Regex for validating URL. Should be overridden by subclass."""
-
     def __init__(self, url: str, html: Optional[str] = None,
-                 update_html: bool = True, validate_url: bool = True) -> None:
+                 update_html: bool = True) -> None:
         """
         Creates scraper object that is by default ready for HTML parsing. Call
         parsing methods to parse data from HTML.
 
         :param url: URL of procyclingstats page to parse. Either absolute or
             relative.
         :param html: HTML to be parsed from, defaults to None. When passing the
             parameter, set `update_html` to False to prevent overriding or
             making useless request.
         :param update_html: Whether to make request to given URL and update
             `self.html`. When False `self.update_html` method has to be called
             manually to make object ready for parsing. Defaults to True.
-        :param validate_url: Whether to validate passed URL by current scraping
-            class regex. Defaults to True and is strongly recomended to leave
-            as is. Setting to False might result in unexpected behaviour of
-            some methods that use the URL or obtaining wrong HTML, which is
-            not possible to parse correctly.
 
-        :raises ValueError: When given URL isn't valid for current scraping
-            class.
         :raises ValueError: When given HTML or HTML from given URL is invalid,
             e.g. 'Page not found' is contained in the HTML.
         """
         # validate given URL
-        try:
-            if validate_url:
-                validate_string(url, regex=self._url_validation_regex)
-        except ParsedValueInvalidError:
-            raise ValueError(f"Given URL is indvalid: '{url}'") \
-                # pylint: disable=raise-missing-from
-
         self._url = self._make_url_absolute(url)
         self._html = None
         if html:
             self._html = HTMLParser(html)
             if not self._html_valid():
                 raise ValueError("Given HTML is invalid.")
             self._set_up_html()
@@ -66,22 +48,15 @@
             self.update_html()
             if not self._html_valid():
                 raise ValueError(
                     f"HTML from given URL is invalid: '{self.url}'")
             self._set_up_html()
 
     def __repr__(self) -> str:
-        return f"{type(self).__name__}(url='{self.normalized_relative_url()}')"
-
-    def __eq__(self, other) -> bool:
-        """Compares two classes based on their `normalized_relative_url`."""
-        if isinstance(type(self), type(other)):
-            return False
-        return (self.normalized_relative_url() ==
-                other.normalized_relative_url())
+        return f"{type(self).__name__}(url='{self.url}')"
 
     @property
     def url(self) -> str:
         """Absolute URL from URL that was passed when constructing."""
         return self._url
 
     @property
@@ -101,25 +76,14 @@
         """
         Makes relative URL from absolute url (cuts `self.BASE_URL` from URL).
 
         :return: Relative URL.
         """
         return "/".join(self._url.split("/")[3:])
 
-    def normalized_relative_url(self) -> str:
-        """
-        Creates normalized relative URL. By default only removes extra slashes
-        from user defined relative URL. Is used for evaluating equality of
-        objects and should be overridden by subclass. In general this method
-        should remove unnecessary information from the URL.
-
-        :return: Normalized URL.
-        """
-        return "/".join(self._decompose_url())
-
     def update_html(self) -> None:
         """
         Calls request to `self.url` and updates `self.html` to HTMLParser
         object created from returned HTML.
         """
         html_str = requests.get(self._url).text \
             # pylint: disable=missing-timeout
```

### Comparing `procyclingstats-0.1.4/procyclingstats/stage_scraper.py` & `procyclingstats-0.1.5/procyclingstats/stage_scraper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Dict, List, Literal, Optional
 
 from selectolax.parser import HTMLParser, Node
 
 from .errors import ExpectedParsingError
 from .scraper import Scraper
 from .table_parser import TableParser
-from .utils import (add_times, convert_date, format_regex_str, format_time,
-                    join_tables, parse_table_fields_args, reg)
+from .utils import (add_times, convert_date, format_time, join_tables,
+                    parse_table_fields_args)
 
 
 class Stage(Scraper):
     """
     Scraper for stage results HTML page.
 
     Usage:
@@ -41,52 +41,16 @@
                 'uci_points': 25.0
             },
             ...
         ],
         ...
     }
     """
-    _url_validation_regex = format_regex_str(
-    f"""
-        {reg.base_url}?race{reg.url_str}
-        ({reg.year}{reg.stage}({reg.result}{reg.anything}?)?|
-        ({reg.year}{reg.result}?({reg.result}{reg.result}{reg.anything})?)|
-        ({reg.result}{reg.anything}))?
-        \\/*
-    """)
-    """Regex for validating stage URL."""
     _tables_path = ".result-cont table"
 
-    def normalized_relative_url(self) -> str:
-        """
-        Creates normalized relative URL. Determines equality of objects (is
-        used in `__eq__` method).
-
-        :return: Normalized URL in ``race/{race_id}/{year}/{stage_id}`` format.
-            When year or stage_id aren't contained in user defined URL, they
-            are skipped.
-        """
-        decomposed_url = self._decompose_url()
-        decomposed_url.extend([""] * (4 - len(decomposed_url)))
-        race_id = decomposed_url[1]
-        if decomposed_url[2].isnumeric() and len(decomposed_url[2]) == 4:
-            year = decomposed_url[2]
-        else:
-            year = None
-        if "stage" in decomposed_url[3] or "prologue" in decomposed_url[3]:
-            stage_id = decomposed_url[3]
-        else:
-            stage_id = None
-        normalized_url = f"race/{race_id}"
-        if year is not None:
-            normalized_url += f"/{year}"
-            if stage_id is not None:
-                normalized_url += f"/{stage_id}"
-        return normalized_url
-
     def _set_up_html(self) -> None:
         """
         Overrides Scraper method. Modifies HTML if stage is TTT by adding team
         ranks to riders.
         """
         # add team ranks to every rider's first td element, so it's possible
         # to map teams to riders based on their rank
@@ -270,14 +234,15 @@
         because they aren't contained in the HTML.
 
         :param args: Fields that should be contained in returned table. When
             no args are passed, all fields are parsed.
 
             - rider_name:
             - rider_url:
+            - rider_number:
             - team_name:
             - team_url:
             - rank: Rider's result in the stage.
             - status: ``DF``, ``DNF``, ``DNS``, ``OTL`` or ``DSQ``.
             - age: Rider's age.
             - nationality: Rider's nationality as 2 chars long country code.
             - time: Rider's time in the stage.
@@ -287,14 +252,15 @@
 
         :raises ValueError: When one of args is of invalid value.
         :return: Table with wanted fields.
         """
         available_fields = (
             "rider_name",
             "rider_url",
+            "rider_number",
             "team_name",
             "team_url",
             "rank",
             "status",
             "age",
             "nationality",
             "time",
@@ -326,18 +292,23 @@
                 table_parser = TableParser(gc_table_html)
                 extra_fields = [f for f in fields
                                 if f in ("nationality", "age", "rider_url")]
                 # add rider_url for table joining purposes
                 extra_fields.append("rider_url")
                 table_parser.parse(extra_fields)
                 table = join_tables(table, table_parser.table, "rider_url")
-            elif "nationality" in fields or "age" in fields:
+            elif "nationality" in fields or "age" in fields or \
+                "rider_number" in fields:
                 for row in table:
-                    row['nationality'] = None
-                    row['age'] = None
+                    if "nationality" in fields:
+                        row['nationality'] = None
+                    if "age" in fields:
+                        row['age'] = None
+                    if "rider_number" in fields:
+                        row['rider_number'] = None
             # remove rider_url from table if isn't needed
             if "rider_url" not in fields:
                 for row in table:
                     row.pop("rider_url")
         else:
             table_parser = TableParser(results_table_html)
             table_parser.parse(fields)
@@ -351,14 +322,15 @@
         is returned.
 
         :param args: Fields that should be contained in returned table. When
             no args are passed, all fields are parsed.
 
             - rider_name:
             - rider_url:
+            - rider_number:
             - team_name:
             - team_url:
             - rank: Rider's GC rank after the stage.
             - prev_rank: Rider's GC rank before the stage.
             - age: Rider's age.
             - nationality: Rider's nationality as 2 chars long country code.
             - time: Rider's GC time after the stage.
@@ -368,14 +340,15 @@
 
         :raises ValueError: When one of args is of invalid value.
         :return: Table with wanted fields.
         """
         available_fields = (
             "rider_name",
             "rider_url",
+            "rider_number",
             "team_name",
             "team_url",
             "rank",
             "prev_rank",
             "age",
             "nationality",
             "time",
@@ -398,14 +371,15 @@
         classif. is unavailable empty list is returned.
 
         :param args: Fields that should be contained in returned table. When
             no args are passed, all fields are parsed.
 
             - rider_name:
             - rider_url:
+            - rider_number:
             - team_name:
             - team_url:
             - rank: Rider's points classif. rank after the stage.
             - prev_rank: Rider's points classif. rank before the stage.
             - points: Rider's points classif. points after the stage.
             - age: Rider's age.
             - nationality: Rider's nationality as 2 chars long country code.
@@ -414,14 +388,15 @@
 
         :raises ValueError: When one of args is of invalid value.
         :return: Table with wanted fields.
         """
         available_fields = (
             "rider_name",
             "rider_url",
+            "rider_number",
             "team_name",
             "team_url",
             "rank",
             "prev_rank",
             "points",
             "age",
             "nationality",
@@ -443,14 +418,15 @@
         unavailable empty list is returned.
 
         :param args: Fields that should be contained in returned table. When
             no args are passed, all fields are parsed.
 
             - rider_name:
             - rider_url:
+            - rider_number:
             - team_name:
             - team_url:
             - rank: Rider's KOM classif. rank after the stage.
             - prev_rank: Rider's KOM classif. rank before the stage.
             - points: Rider's KOM points after the stage.
             - age: Rider's age.
             - nationality: Rider's nationality as 2 chars long country code.
@@ -459,14 +435,15 @@
 
         :raises ValueError: When one of args is of invalid value.
         :return: Table with wanted fields.
         """
         available_fields = (
             "rider_name",
             "rider_url",
+            "rider_number",
             "team_name",
             "team_url",
             "rank",
             "prev_rank",
             "points",
             "age",
             "nationality",
@@ -488,14 +465,15 @@
         is unavailable empty list is returned.
 
         :param args: Fields that should be contained in returned table. When
             no args are passed, all fields are parsed.
 
             - rider_name:
             - rider_url:
+            - rider_number:
             - team_name:
             - team_url:
             - rank: Rider's youth classif. rank after the stage.
             - prev_rank: Rider's youth classif. rank before the stage.
             - time: Rider's GC time after the stage.
             - age: Rider's age.
             - nationality: Rider's nationality as 2 chars long country code.
@@ -504,14 +482,15 @@
 
         :raises ValueError: When one of args is of invalid value.
         :return: Table with wanted fields.
         """
         available_fields = (
             "rider_name",
             "rider_url",
+            "rider_number",
             "team_name",
             "team_url",
             "rank",
             "prev_rank",
             "time",
             "age",
             "nationality",
@@ -598,16 +577,16 @@
     def _ttt_results(results_table_html: Node,
                      fields: List[str]) -> List[Dict[str, Any]]:
         """
         Parses data from TTT results table.
 
         :param results_table_html: TTT results table HTML.
         :param fields: Fields that returned table should have. Available are
-            all `results` table fields with the exception of age and
-            nationality.
+            all `results` table fields with the exception of age,
+            nationality and rider_number.
         :return: Table with wanted fields.
         """
         team_fields = [
             "rank",
             "team_name",
             "team_url",
         ]
```

### Comparing `procyclingstats-0.1.4/procyclingstats/table_parser.py` & `procyclingstats-0.1.5/procyclingstats/table_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
             - nation_name
             - age
             - nationality
             - time
             - bonus
             - profile_icon
             - season
+            - rider_number
 
         :fields options for tables with a header:
             - rank
             - status
             - prev_rank
             - pcs_points
             - uci_points
@@ -279,14 +280,19 @@
         for season_e in seasons_elements:
             season_e_text = season_e.text()
             if season_e_text.isnumeric():
                 seasons.append(int(season_e_text))
             else:
                 seasons.append(None)
         return seasons
+    
+    def rider_number(self) -> List[Optional[int]]:
+        bibs_elements = self.html_table.css(".bibs")
+        return [int(bib_e.text()) if bib_e.text().isnumeric() else None \
+            for bib_e in bibs_elements]
 
     def rank(self) -> List[Optional[int]]:
         possible_columns = ["Rnk", "pos", "Result", "#"]
         for column_name in possible_columns:
             try:
                 return self.parse_extra_column(column_name,
                     lambda x: int(x) if x.isnumeric() else None)
@@ -306,25 +312,25 @@
                 lambda x: int(x) if x else None)
         except ValueError:
             return [None for _ in range(self.table_length)]
 
     def uci_points(self) -> List[Optional[float]]:
         try:
             return self.parse_extra_column("UCI",
-                lambda x: float(x) if x else 0)
+                lambda x: float(x) if x and x.replace('.', '', 1).isdigit() else 0)
         except ValueError:
             return [0 for _ in range(self.table_length)]
 
     def pcs_points(self) -> List[Optional[int]]:
         try:
             return self.parse_extra_column("Pnt", lambda x: int(x) if x else 0)
         except ValueError:
             try:
                 return self.parse_extra_column("PCS points",
-                    lambda x: int(x) if x else 0)
+                    lambda x: int(x) if x  and x.isdigit() else 0)
             except ValueError:
                 return [0 for _ in range(self.table_length)]
 
     def points(self) -> List[int]:
         return self.parse_extra_column("Points", lambda x:
             float(x) if x else 0)
```

### Comparing `procyclingstats-0.1.4/procyclingstats/team_scraper.py` & `procyclingstats-0.1.5/procyclingstats/team_scraper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Dict, List, Optional
 
 from .scraper import Scraper
 from .table_parser import TableParser
-from .utils import (format_regex_str, get_day_month, join_tables, parse_select,
-                    parse_table_fields_args, reg)
+from .utils import (get_day_month, join_tables, parse_select,
+                    parse_table_fields_args)
 
 
 class Team(Scraper):
     """
     Scraper for team HTML page.
 
     Usage:
@@ -27,32 +27,14 @@
             },
             ...
         ],
         'name': 'BORA - hansgrohe',
         ...
     }
     """
-    _url_validation_regex = format_regex_str(
-    f"""
-        {reg.base_url}?team{reg.team_url_str}
-        ({reg.overview}{reg.anything}?)?\\/*
-    """)
-    """Regex for validating team URL."""
-
-    def normalized_relative_url(self) -> str:
-        """
-        Creates normalized relative URL. Determines equality of objects (is
-        used in __eq__ method).
-
-        :return: Normalized URL in ``team/{team_id}`` format.
-        """
-        decomposed_url = self._decompose_url()
-        team_id = decomposed_url[1]
-        return f"team/{team_id}"
-
     def name(self) -> str:
         """
         Parses team display name from HTML.
 
         :return: Display name, e.g. ``BORA - hansgrohe``.
         """
         display_name_html = self.html.css_first(".page-title > .main > h1")
```

### Comparing `procyclingstats-0.1.4/procyclingstats.egg-info/PKG-INFO` & `procyclingstats-0.1.5/procyclingstats.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: procyclingstats
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python API wrapper for procyclingstats.com
 Home-page: https://github.com/themm1/procyclingstats
 Author: Martin Madzin
 Author-email: madzin.m@gmail.com
 License: MIT
 Description: procyclingstats
         ===============
@@ -49,22 +49,34 @@
         
         Interface consists from scraping classes which are currently ``Race``,
         ``RaceStartlist``, ``RaceClimbs``, ``Ranking``, ``Rider``, ``RiderResults``,
         ``Stage`` and ``Team``. Usage of all scraping classes is almost the same and
         the only difference among them are parsing methods as is for example
         ``birthdate`` in Rider class usage example.
         
+        Unexpected behaviour and parsing errors
+        ---------------------------------------
+        
+        Since the project is a web scraper which parses HTML, it's difficult to make
+        it reliable and it's common to encounter some HTML parsing problems. After
+        getting some kind of unexpected behaviour or parsing errors, it's recommended
+        to update the package on your system using
+        ``pip install procyclingstats --upgrade``. If the problem proceeds, see the
+        GitHub issues_ page and if the issue hasn't been opened yet, don't hesitate to
+        open one!
+        
         Links
         -----
         
         - GitHub_
         - PyPI_
         - Documentation_
         
         .. _GitHub: https://github.com/themm1/procyclingstats
         .. _PyPI: https://pypi.org/project/procyclingstats
         .. _Documentation: https://procyclingstats.readthedocs.io/en/latest
         .. _procyclingstats.com: https://www.procyclingstats.com
         .. _selectolax: https://github.com/rushter/selectolax
+        .. _issues: https://github.com/themm1/procyclingstats/issues
 Keywords: cycling cycling-stats procyclingstats scraper html-parsing sports-analytics
 Platform: UNKNOWN
 Description-Content-Type: text/x-rst
```

### Comparing `procyclingstats-0.1.4/procyclingstats.egg-info/SOURCES.txt` & `procyclingstats-0.1.5/procyclingstats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `procyclingstats-0.1.4/setup.py` & `procyclingstats-0.1.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.rst", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="procyclingstats",
-    version="0.1.4",
+    version="0.1.5",
     license="MIT",
     description="A Python API wrapper for procyclingstats.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     author="Martin Madzin",
     author_email="madzin.m@gmail.com",
     packages=["procyclingstats"],
```

