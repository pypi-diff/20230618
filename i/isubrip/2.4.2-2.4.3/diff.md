# Comparing `tmp/isubrip-2.4.2.tar.gz` & `tmp/isubrip-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isubrip-2.4.2.tar", last modified: Fri Jun  2 18:34:52 2023, max compression
+gzip compressed data, was "isubrip-2.4.3.tar", last modified: Sun Jun 18 19:33:13 2023, max compression
```

## Comparing `isubrip-2.4.2.tar` & `isubrip-2.4.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 18:34:52.664036 isubrip-2.4.2/
--rw-rw-rw-   0        0        0     1093 2022-01-28 09:13:22.000000 isubrip-2.4.2/LICENSE
--rw-rw-rw-   0        0        0     3536 2023-06-02 18:34:52.663036 isubrip-2.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     2411 2023-06-02 18:33:22.000000 isubrip-2.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 18:34:52.646516 isubrip-2.4.2/isubrip/
--rw-rw-rw-   0        0        0       23 2023-06-02 18:33:22.000000 isubrip-2.4.2/isubrip/__init__.py
--rw-rw-rw-   0        0        0    13093 2023-06-02 18:33:22.000000 isubrip-2.4.2/isubrip/__main__.py
--rw-rw-rw-   0        0        0    11888 2023-06-02 14:55:15.000000 isubrip-2.4.2/isubrip/config.py
--rw-rw-rw-   0        0        0     2175 2023-06-02 18:33:16.000000 isubrip-2.4.2/isubrip/constants.py
--rw-rw-rw-   0        0        0     6053 2023-05-26 11:44:57.000000 isubrip-2.4.2/isubrip/data_structures.py
-drwxrwxrwx   0        0        0        0 2023-06-02 18:34:52.653522 isubrip-2.4.2/isubrip/resources/
--rw-rw-rw-   0        0        0      595 2023-05-23 20:01:27.000000 isubrip-2.4.2/isubrip/resources/default_config.toml
-drwxrwxrwx   0        0        0        0 2023-06-02 18:34:52.656522 isubrip-2.4.2/isubrip/scrapers/
--rw-rw-rw-   0        0        0        0 2023-05-26 10:40:55.000000 isubrip-2.4.2/isubrip/scrapers/__init__.py
--rw-rw-rw-   0        0        0    15845 2023-05-30 20:51:32.000000 isubrip-2.4.2/isubrip/scrapers/appletv_scraper.py
--rw-rw-rw-   0        0        0     4334 2023-06-02 14:55:15.000000 isubrip-2.4.2/isubrip/scrapers/itunes_scraper.py
--rw-rw-rw-   0        0        0    22271 2023-06-02 18:33:16.000000 isubrip-2.4.2/isubrip/scrapers/scraper.py
-drwxrwxrwx   0        0        0        0 2023-06-02 18:34:52.660525 isubrip-2.4.2/isubrip/subtitle_formats/
--rw-rw-rw-   0        0        0        0 2023-05-24 22:34:46.000000 isubrip-2.4.2/isubrip/subtitle_formats/__init__.py
--rw-rw-rw-   0        0        0     1383 2023-05-26 11:44:57.000000 isubrip-2.4.2/isubrip/subtitle_formats/subrip.py
--rw-rw-rw-   0        0        0     7909 2023-05-26 11:44:57.000000 isubrip-2.4.2/isubrip/subtitle_formats/subtitles.py
--rw-rw-rw-   0        0        0     9220 2023-05-26 11:44:57.000000 isubrip-2.4.2/isubrip/subtitle_formats/webvtt.py
--rw-rw-rw-   0        0        0    13341 2023-06-02 14:19:57.000000 isubrip-2.4.2/isubrip/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-02 18:34:52.652525 isubrip-2.4.2/isubrip.egg-info/
--rw-rw-rw-   0        0        0     3536 2023-06-02 18:34:52.000000 isubrip-2.4.2/isubrip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      663 2023-06-02 18:34:52.000000 isubrip-2.4.2/isubrip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 18:34:52.000000 isubrip-2.4.2/isubrip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-02 18:34:52.000000 isubrip-2.4.2/isubrip.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       38 2023-06-02 18:34:52.000000 isubrip-2.4.2/isubrip.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-02 18:34:52.000000 isubrip-2.4.2/isubrip.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       83 2023-05-26 11:45:14.000000 isubrip-2.4.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-02 18:34:52.664036 isubrip-2.4.2/setup.cfg
--rw-rw-rw-   0        0        0     2815 2023-05-26 11:44:57.000000 isubrip-2.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 19:33:13.422226 isubrip-2.4.3/
+-rw-rw-rw-   0        0        0     1093 2022-01-28 09:13:22.000000 isubrip-2.4.3/LICENSE
+-rw-rw-rw-   0        0        0     3536 2023-06-18 19:33:13.421226 isubrip-2.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2411 2023-06-18 19:32:47.000000 isubrip-2.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 19:33:13.408182 isubrip-2.4.3/isubrip/
+-rw-rw-rw-   0        0        0       23 2023-06-18 19:32:47.000000 isubrip-2.4.3/isubrip/__init__.py
+-rw-rw-rw-   0        0        0    13093 2023-06-17 17:48:16.000000 isubrip-2.4.3/isubrip/__main__.py
+-rw-rw-rw-   0        0        0    11888 2023-06-17 17:48:16.000000 isubrip-2.4.3/isubrip/config.py
+-rw-rw-rw-   0        0        0     2175 2023-06-17 17:48:16.000000 isubrip-2.4.3/isubrip/constants.py
+-rw-rw-rw-   0        0        0     6057 2023-06-18 19:30:18.000000 isubrip-2.4.3/isubrip/data_structures.py
+drwxrwxrwx   0        0        0        0 2023-06-18 19:33:13.414182 isubrip-2.4.3/isubrip/resources/
+-rw-rw-rw-   0        0        0      595 2023-05-23 20:01:27.000000 isubrip-2.4.3/isubrip/resources/default_config.toml
+drwxrwxrwx   0        0        0        0 2023-06-18 19:33:13.418225 isubrip-2.4.3/isubrip/scrapers/
+-rw-rw-rw-   0        0        0        0 2023-05-26 10:40:55.000000 isubrip-2.4.3/isubrip/scrapers/__init__.py
+-rw-rw-rw-   0        0        0    15845 2023-06-18 19:30:18.000000 isubrip-2.4.3/isubrip/scrapers/appletv_scraper.py
+-rw-rw-rw-   0        0        0     4334 2023-06-17 17:48:16.000000 isubrip-2.4.3/isubrip/scrapers/itunes_scraper.py
+-rw-rw-rw-   0        0        0    22271 2023-06-17 17:48:16.000000 isubrip-2.4.3/isubrip/scrapers/scraper.py
+drwxrwxrwx   0        0        0        0 2023-06-18 19:33:13.421226 isubrip-2.4.3/isubrip/subtitle_formats/
+-rw-rw-rw-   0        0        0        0 2023-05-24 22:34:46.000000 isubrip-2.4.3/isubrip/subtitle_formats/__init__.py
+-rw-rw-rw-   0        0        0     1383 2023-06-17 17:47:55.000000 isubrip-2.4.3/isubrip/subtitle_formats/subrip.py
+-rw-rw-rw-   0        0        0     7909 2023-06-17 17:47:55.000000 isubrip-2.4.3/isubrip/subtitle_formats/subtitles.py
+-rw-rw-rw-   0        0        0     9220 2023-06-17 17:47:55.000000 isubrip-2.4.3/isubrip/subtitle_formats/webvtt.py
+-rw-rw-rw-   0        0        0    13457 2023-06-18 19:30:18.000000 isubrip-2.4.3/isubrip/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-18 19:33:13.414182 isubrip-2.4.3/isubrip.egg-info/
+-rw-rw-rw-   0        0        0     3536 2023-06-18 19:33:13.000000 isubrip-2.4.3/isubrip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      663 2023-06-18 19:33:13.000000 isubrip-2.4.3/isubrip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 19:33:13.000000 isubrip-2.4.3/isubrip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-18 19:33:13.000000 isubrip-2.4.3/isubrip.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       38 2023-06-18 19:33:13.000000 isubrip-2.4.3/isubrip.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-18 19:33:13.000000 isubrip-2.4.3/isubrip.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       83 2023-06-17 18:04:27.000000 isubrip-2.4.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-18 19:33:13.422226 isubrip-2.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     2815 2023-06-17 17:47:55.000000 isubrip-2.4.3/setup.py
```

### Comparing `isubrip-2.4.2/LICENSE` & `isubrip-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.2/PKG-INFO` & `isubrip-2.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isubrip
-Version: 2.4.2
+Version: 2.4.3
 Summary: A Python package for scraping and downloading subtitles from iTunes movie pages.
 Home-page: https://github.com/MichaelYochpaz/iSubRip
 Author: Michael Yochpaz
 License: MIT
 Project-URL: Bug Reports, https://github.com/MichaelYochpaz/iSubRip/issues
 Project-URL: Source, https://github.com/MichaelYochpaz/iSubRip
 Keywords: iTunes,AppleTV,movies,subtitles,scrape,scraper,download,m3u8
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # iSubRip
 A Python package for scraping and downloading subtitles from AppleTV / iTunes movie pages.  
-Latest version: 2.4.2 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
+Latest version: 2.4.3 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
 
 <br/>
   
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/month)](https://python.org/pypi/isubrip)
 [![PyPI - Total Downloads](https://pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/pypi/isubrip)
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: isubrip Version: 2.4.2 Summary: A Python package
+Metadata-Version: 2.1 Name: isubrip Version: 2.4.3 Summary: A Python package
 for scraping and downloading subtitles from iTunes movie pages. Home-page:
 https://github.com/MichaelYochpaz/iSubRip Author: Michael Yochpaz License: MIT
 Project-URL: Bug Reports, https://github.com/MichaelYochpaz/iSubRip/issues
 Project-URL: Source, https://github.com/MichaelYochpaz/iSubRip Keywords:
 iTunes,AppleTV,movies,subtitles,scrape,scraper,download,m3u8 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 End Users/Desktop Classifier: Intended Audience :: Developers Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE # iSubRip A Python package for scraping and
-downloading subtitles from AppleTV / iTunes movie pages. Latest version: 2.4.2
+downloading subtitles from AppleTV / iTunes movie pages. Latest version: 2.4.3
 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))
 
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/
 pypi/isubrip) [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/
 month)](https://python.org/pypi/isubrip) [![PyPI - Total Downloads](https://
 pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip) [![PyPI - Python
 Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/
```

### Comparing `isubrip-2.4.2/README.md` & `isubrip-2.4.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # iSubRip
 A Python package for scraping and downloading subtitles from AppleTV / iTunes movie pages.  
-Latest version: 2.4.2 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
+Latest version: 2.4.3 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
 
 <br/>
   
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/month)](https://python.org/pypi/isubrip)
 [![PyPI - Total Downloads](https://pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/pypi/isubrip)
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # iSubRip A Python package for scraping and downloading subtitles from AppleTV
-/ iTunes movie pages. Latest version: 2.4.2 ([changelog](https://github.com/
+/ iTunes movie pages. Latest version: 2.4.3 ([changelog](https://github.com/
 MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/
 pypi/isubrip) [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/
 month)](https://python.org/pypi/isubrip) [![PyPI - Total Downloads](https://
 pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip) [![PyPI - Python
 Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/
 pypi/isubrip) [![GitHub - License](https://img.shields.io/github/license/
```

### Comparing `isubrip-2.4.2/isubrip/__main__.py` & `isubrip-2.4.3/isubrip/__main__.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.2/isubrip/config.py` & `isubrip-2.4.3/isubrip/config.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.2/isubrip/constants.py` & `isubrip-2.4.3/isubrip/constants.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.2/isubrip/data_structures.py` & `isubrip-2.4.3/isubrip/data_structures.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,16 @@
     scraper: Scraper
     original_scraper: Scraper
     original_data: dict
 
 
 @dataclass
 class MovieData(MediaData):
-    """A named tuple containing movie metadata.
+    """
+    A named tuple containing movie metadata.
 
     Attributes:
         duration (timedelta | None, optional): Duration of the movie. Defaults to None.
         preorder_availability_date (datetime | None, optional): Date when the movie will be available for preorder.
             None if not a preorder. Defaults to None.
     """
     duration: dt.timedelta | None = None
@@ -160,15 +161,14 @@
     episode_name: str
     season_number: int
     episode_release_date: dt.datetime | None = None
     season_name: str | None = None
     duration: dt.timedelta | None = None
 
 
-
 @dataclass
 class SeasonData(MediaData):
     """
     A named tuple containing season metadata.
 
     Attributes:
         season_number (int): Season number.
```

### Comparing `isubrip-2.4.2/isubrip/resources/default_config.toml` & `isubrip-2.4.3/isubrip/resources/default_config.toml`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.2/isubrip/scrapers/appletv_scraper.py` & `isubrip-2.4.3/isubrip/scrapers/appletv_scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 class AppleTVScraper(M3U8Scraper, MovieScraper, SeriesScraper):
     """An Apple TV scraper."""
     id = "appletv"
     name = "Apple TV"  # (iTunes content is redirected to the iTunes scraper)
     abbreviation = "ATV"
-    url_regex = r"(?P<base_url>https?://tv\.apple\.com/(?:(?P<country_code>[a-z]{2})/)?(?P<media_type>movie|episode|season|show)/(?:(?P<media_name>[\w\-%]+)/)?(?P<media_id>umc\.cmc\.[a-z\d]{24,25}))(?:\?(?P<url_params>(?:).*))?"  # noqa: E501
+    url_regex = r"(?P<base_url>https?://tv\.apple\.com/(?:(?P<country_code>[a-z]{2})/)?(?P<media_type>movie|episode|season|show)/(?:(?P<media_name>[\w\-%]+)/)?(?P<media_id>umc\.cmc\.[a-z\d]{23,25}))(?:\?(?P<url_params>(?:).*))?"  # noqa: E501
     subtitles_class = WebVTTSubtitles
     is_movie_scraper = True
     is_series_scraper = True
     uses_scrapers = ["itunes"]
 
     _api_base_url = "https://tv.apple.com/api/uts/v3"
     _api_base_params = {
```

### Comparing `isubrip-2.4.2/isubrip/scrapers/itunes_scraper.py` & `isubrip-2.4.3/isubrip/scrapers/itunes_scraper.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.2/isubrip/scrapers/scraper.py` & `isubrip-2.4.3/isubrip/scrapers/scraper.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.2/isubrip/subtitle_formats/subrip.py` & `isubrip-2.4.3/isubrip/subtitle_formats/subrip.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.2/isubrip/subtitle_formats/subtitles.py` & `isubrip-2.4.3/isubrip/subtitle_formats/subtitles.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.2/isubrip/subtitle_formats/webvtt.py` & `isubrip-2.4.3/isubrip/subtitle_formats/webvtt.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.2/isubrip/utils.py` & `isubrip-2.4.3/isubrip/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import re
 import sys
 
 from abc import ABCMeta
 from os import PathLike
 from pathlib import Path
-from typing import Any, Iterable, Union, get_args, get_origin
+from typing import Any, Union, get_args, get_origin
 
 from isubrip.data_structures import EpisodeData, MovieData, SubtitlesData, SubtitlesFormat, SubtitlesType
 
 
 class SingletonMeta(ABCMeta):
     """
     A metaclass that implements the Singleton pattern.
@@ -277,15 +277,15 @@
 
     Args:
         url_params (str): URL parameters. (e.g. 'param1=value1&param2=value2')
 
     Returns:
         dict: A dictionary containing the URL parameters.
     """
-    url_params = url_params.strip('?').rstrip('&')
+    url_params = url_params.split('?')[-1].rstrip('&')
     params_list = url_params.split('&')
 
     if len(params_list) == 0 or \
             (len(params_list) == 1 and '=' not in params_list[0]):
         return {}
 
     return {key: value for key, value in (param.split('=') for param in params_list)}
@@ -299,20 +299,24 @@
     Args:
         obj: Object to convert.
 
     Returns:
         list: A list containing the object.
             If the object is already an iterable, it will be converted to a list.
     """
-    if isinstance(obj, Iterable) and not isinstance(obj, str):
-        return list(obj)
+    if isinstance(obj, list):
+        return obj
 
     elif obj is None:
         return []
 
+    # tuple (not a namedtuple) or a set
+    elif (isinstance(obj, tuple) and not hasattr(obj, '_fields')) or isinstance(obj, set):
+        return list(obj)
+
     return [obj]
 
 
 def split_subtitles_timestamp(timestamp: str) -> tuple[dt.time, dt.time]:
     """
     Split a subtitles timestamp into start and end.
```

### Comparing `isubrip-2.4.2/isubrip.egg-info/PKG-INFO` & `isubrip-2.4.3/isubrip.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isubrip
-Version: 2.4.2
+Version: 2.4.3
 Summary: A Python package for scraping and downloading subtitles from iTunes movie pages.
 Home-page: https://github.com/MichaelYochpaz/iSubRip
 Author: Michael Yochpaz
 License: MIT
 Project-URL: Bug Reports, https://github.com/MichaelYochpaz/iSubRip/issues
 Project-URL: Source, https://github.com/MichaelYochpaz/iSubRip
 Keywords: iTunes,AppleTV,movies,subtitles,scrape,scraper,download,m3u8
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # iSubRip
 A Python package for scraping and downloading subtitles from AppleTV / iTunes movie pages.  
-Latest version: 2.4.2 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
+Latest version: 2.4.3 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
 
 <br/>
   
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/month)](https://python.org/pypi/isubrip)
 [![PyPI - Total Downloads](https://pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/pypi/isubrip)
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: isubrip Version: 2.4.2 Summary: A Python package
+Metadata-Version: 2.1 Name: isubrip Version: 2.4.3 Summary: A Python package
 for scraping and downloading subtitles from iTunes movie pages. Home-page:
 https://github.com/MichaelYochpaz/iSubRip Author: Michael Yochpaz License: MIT
 Project-URL: Bug Reports, https://github.com/MichaelYochpaz/iSubRip/issues
 Project-URL: Source, https://github.com/MichaelYochpaz/iSubRip Keywords:
 iTunes,AppleTV,movies,subtitles,scrape,scraper,download,m3u8 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 End Users/Desktop Classifier: Intended Audience :: Developers Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE # iSubRip A Python package for scraping and
-downloading subtitles from AppleTV / iTunes movie pages. Latest version: 2.4.2
+downloading subtitles from AppleTV / iTunes movie pages. Latest version: 2.4.3
 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))
 
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/
 pypi/isubrip) [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/
 month)](https://python.org/pypi/isubrip) [![PyPI - Total Downloads](https://
 pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip) [![PyPI - Python
 Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/
```

### Comparing `isubrip-2.4.2/isubrip.egg-info/SOURCES.txt` & `isubrip-2.4.3/isubrip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.2/setup.py` & `isubrip-2.4.3/setup.py`

 * *Files identical despite different names*

