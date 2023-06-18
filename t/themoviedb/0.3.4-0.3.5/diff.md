# Comparing `tmp/themoviedb-0.3.4.tar.gz` & `tmp/themoviedb-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "themoviedb-0.3.4.tar", last modified: Sun Jun 18 02:14:26 2023, max compression
+gzip compressed data, was "themoviedb-0.3.5.tar", last modified: Sun Jun 18 02:19:04 2023, max compression
```

## Comparing `themoviedb-0.3.4.tar` & `themoviedb-0.3.5.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxrwxr-x   0 leandro   (1000) leandro   (1000)        0 2023-06-18 02:14:26.171636 themoviedb-0.3.4/
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     7359 2023-06-18 02:14:26.171636 themoviedb-0.3.4/PKG-INFO
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     4920 2023-06-18 02:14:21.000000 themoviedb-0.3.4/README.rst
--rw-rw-r--   0 leandro   (1000) leandro   (1000)       38 2023-06-18 02:14:26.171636 themoviedb-0.3.4/setup.cfg
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     1714 2023-06-18 02:11:06.000000 themoviedb-0.3.4/setup.py
-drwxrwxr-x   0 leandro   (1000) leandro   (1000)        0 2023-06-18 02:14:26.167636 themoviedb-0.3.4/themoviedb/
--rw-rw-r--   0 leandro   (1000) leandro   (1000)       72 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/__init__.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     6027 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/aiotmdb.py
-drwxrwxr-x   0 leandro   (1000) leandro   (1000)        0 2023-06-18 02:14:26.167636 themoviedb-0.3.4/themoviedb/routes_async/
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     1197 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_async/__init__.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     2985 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_async/_base.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     2703 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_async/authentication.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      866 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_async/certifications.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     1279 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_async/collections.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     1232 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_async/companies.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      546 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_async/credit.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     6165 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_async/discover.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      621 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_async/episode_groups.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     2674 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_async/episodes.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     3030 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_async/find.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      700 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_async/genres.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     1516 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_async/guest.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      956 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_async/keywords.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     7019 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_async/movies.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     1231 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_async/network.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     3790 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_async/people.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      557 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_async/reviews.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     3303 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_async/search.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     3043 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_async/seasons.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     2046 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_async/trending.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     7757 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_async/tv.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     1409 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_async/watch_providers.py
-drwxrwxr-x   0 leandro   (1000) leandro   (1000)        0 2023-06-18 02:14:26.171636 themoviedb-0.3.4/themoviedb/routes_sync/
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     1175 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_sync/__init__.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     2956 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_sync/_base.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     2642 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_sync/authentication.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      841 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_sync/certifications.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     1242 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_sync/collections.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     1195 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_sync/companies.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      533 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_sync/credit.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     6140 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_sync/discover.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      608 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_sync/episode_groups.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     2601 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_sync/episodes.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     2933 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_sync/find.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      675 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_sync/genres.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     1479 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_sync/guest.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      931 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_sync/keywords.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     6790 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_sync/movies.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     1194 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_sync/network.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     3669 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_sync/people.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      544 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_sync/reviews.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     3218 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_sync/search.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     2958 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_sync/seasons.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     1973 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_sync/trending.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     7504 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_sync/tv.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     1372 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/routes_sync/watch_providers.py
-drwxrwxr-x   0 leandro   (1000) leandro   (1000)        0 2023-06-18 02:14:26.171636 themoviedb-0.3.4/themoviedb/schemas/
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     2607 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/__init__.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      962 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/_enums.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     6059 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/_partial.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      837 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/_result.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      378 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/alternative_names.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      594 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/alternative_titles.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      738 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/authentication.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      712 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/certifications.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      134 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/changes.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      422 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/collections.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      546 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/companies.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      396 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/content_ratings.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      214 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/countries.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      834 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/credit.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     7860 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/credits.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      887 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/episode_groups.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      617 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/episodes.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     2103 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/external_ids.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      389 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/genres.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     1335 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/images.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      455 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/keywords.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      253 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/languages.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      805 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/list.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     2564 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/movies.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     1131 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/multi.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      236 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/networks.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     1315 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/people.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      724 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/rated.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      398 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/regions.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      645 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/release_date.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     1138 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/reviews.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      783 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/seasons.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      790 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/translations.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     3825 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/tv.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      635 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/videos.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     1499 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/schemas/watch_providers.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     6014 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/tmdb.py
--rw-rw-r--   0 leandro   (1000) leandro   (1000)      918 2023-06-18 02:08:40.000000 themoviedb-0.3.4/themoviedb/utils.py
-drwxrwxr-x   0 leandro   (1000) leandro   (1000)        0 2023-06-18 02:14:26.167636 themoviedb-0.3.4/themoviedb.egg-info/
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     7359 2023-06-18 02:14:26.000000 themoviedb-0.3.4/themoviedb.egg-info/PKG-INFO
--rw-rw-r--   0 leandro   (1000) leandro   (1000)     3087 2023-06-18 02:14:26.000000 themoviedb-0.3.4/themoviedb.egg-info/SOURCES.txt
--rw-rw-r--   0 leandro   (1000) leandro   (1000)        1 2023-06-18 02:14:26.000000 themoviedb-0.3.4/themoviedb.egg-info/dependency_links.txt
--rw-rw-r--   0 leandro   (1000) leandro   (1000)        1 2023-06-18 02:14:26.000000 themoviedb-0.3.4/themoviedb.egg-info/not-zip-safe
--rw-rw-r--   0 leandro   (1000) leandro   (1000)       46 2023-06-18 02:14:26.000000 themoviedb-0.3.4/themoviedb.egg-info/requires.txt
--rw-rw-r--   0 leandro   (1000) leandro   (1000)       11 2023-06-18 02:14:26.000000 themoviedb-0.3.4/themoviedb.egg-info/top_level.txt
+drwxrwxr-x   0 leandro   (1000) leandro   (1000)        0 2023-06-18 02:19:04.564709 themoviedb-0.3.5/
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     7359 2023-06-18 02:19:04.564709 themoviedb-0.3.5/PKG-INFO
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     4920 2023-06-18 02:14:21.000000 themoviedb-0.3.5/README.rst
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)       38 2023-06-18 02:19:04.564709 themoviedb-0.3.5/setup.cfg
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     1952 2023-06-18 02:18:32.000000 themoviedb-0.3.5/setup.py
+drwxrwxr-x   0 leandro   (1000) leandro   (1000)        0 2023-06-18 02:19:04.556709 themoviedb-0.3.5/themoviedb/
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)       72 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/__init__.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     6027 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/aiotmdb.py
+drwxrwxr-x   0 leandro   (1000) leandro   (1000)        0 2023-06-18 02:19:04.556709 themoviedb-0.3.5/themoviedb/routes_async/
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     1197 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_async/__init__.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     2985 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_async/_base.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     2703 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_async/authentication.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      866 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_async/certifications.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     1279 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_async/collections.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     1232 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_async/companies.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      546 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_async/credit.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     6165 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_async/discover.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      621 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_async/episode_groups.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     2674 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_async/episodes.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     3030 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_async/find.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      700 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_async/genres.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     1516 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_async/guest.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      956 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_async/keywords.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     7019 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_async/movies.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     1231 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_async/network.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     3790 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_async/people.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      557 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_async/reviews.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     3303 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_async/search.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     3043 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_async/seasons.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     2046 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_async/trending.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     7757 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_async/tv.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     1409 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_async/watch_providers.py
+drwxrwxr-x   0 leandro   (1000) leandro   (1000)        0 2023-06-18 02:19:04.560709 themoviedb-0.3.5/themoviedb/routes_sync/
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     1175 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_sync/__init__.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     2956 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_sync/_base.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     2642 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_sync/authentication.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      841 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_sync/certifications.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     1242 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_sync/collections.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     1195 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_sync/companies.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      533 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_sync/credit.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     6140 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_sync/discover.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      608 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_sync/episode_groups.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     2601 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_sync/episodes.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     2933 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_sync/find.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      675 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_sync/genres.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     1479 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_sync/guest.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      931 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_sync/keywords.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     6790 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_sync/movies.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     1194 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_sync/network.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     3669 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_sync/people.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      544 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_sync/reviews.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     3218 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_sync/search.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     2958 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_sync/seasons.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     1973 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_sync/trending.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     7504 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_sync/tv.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     1372 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/routes_sync/watch_providers.py
+drwxrwxr-x   0 leandro   (1000) leandro   (1000)        0 2023-06-18 02:19:04.564709 themoviedb-0.3.5/themoviedb/schemas/
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     2607 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/__init__.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      962 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/_enums.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     6059 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/_partial.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      837 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/_result.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      378 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/alternative_names.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      594 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/alternative_titles.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      738 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/authentication.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      712 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/certifications.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      134 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/changes.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      422 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/collections.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      546 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/companies.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      396 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/content_ratings.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      214 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/countries.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      834 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/credit.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     7860 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/credits.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      887 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/episode_groups.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      617 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/episodes.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     2103 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/external_ids.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      389 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/genres.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     1335 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/images.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      455 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/keywords.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      253 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/languages.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      805 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/list.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     2564 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/movies.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     1131 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/multi.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      236 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/networks.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     1315 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/people.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      724 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/rated.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      398 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/regions.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      645 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/release_date.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     1138 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/reviews.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      783 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/seasons.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      790 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/translations.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     3825 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/tv.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      635 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/videos.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     1499 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/schemas/watch_providers.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     6014 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/tmdb.py
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      918 2023-06-18 02:08:40.000000 themoviedb-0.3.5/themoviedb/utils.py
+drwxrwxr-x   0 leandro   (1000) leandro   (1000)        0 2023-06-18 02:19:04.556709 themoviedb-0.3.5/themoviedb.egg-info/
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     7359 2023-06-18 02:19:04.000000 themoviedb-0.3.5/themoviedb.egg-info/PKG-INFO
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)     3087 2023-06-18 02:19:04.000000 themoviedb-0.3.5/themoviedb.egg-info/SOURCES.txt
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)        1 2023-06-18 02:19:04.000000 themoviedb-0.3.5/themoviedb.egg-info/dependency_links.txt
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)        1 2023-06-18 02:19:04.000000 themoviedb-0.3.5/themoviedb.egg-info/not-zip-safe
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)      214 2023-06-18 02:19:04.000000 themoviedb-0.3.5/themoviedb.egg-info/requires.txt
+-rw-rw-r--   0 leandro   (1000) leandro   (1000)       11 2023-06-18 02:19:04.000000 themoviedb-0.3.5/themoviedb.egg-info/top_level.txt
```

### Comparing `themoviedb-0.3.4/PKG-INFO` & `themoviedb-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: themoviedb
-Version: 0.3.4
+Version: 0.3.5
 Summary: A modern and easy to use API wrapper for The Movie Database (TMDb) API v3 written in Python
 Home-page: https://github.com/leandcesar/themoviedb
 Author: Leandro César
 Author-email: ccleandroc@gmail.com
 License: MIT
 Description: |Code Quality Score| |Code Grade| |Code Coverage| |PyPI Version| |Code style: black| |PyPI License|
```

### Comparing `themoviedb-0.3.4/README.rst` & `themoviedb-0.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/setup.py` & `themoviedb-0.3.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,31 +3,41 @@
 from setuptools import setup, find_packages
 
 with open("README.rst", "r", encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 requirements = [
     "aiohttp==3.8.4",
-    "dacite==1.8.0",
-    "requests==2.28.2",
+    "aiosignal==1.3.1",
+    "async-timeout==4.0.2",
+    "attrs==23.1.0",
+    "certifi==2023.5.7",
+    "charset-normalizer==3.1.0",
+    "dacite==1.8.1",
+    "frozenlist==1.3.3",
+    "idna==3.4",
+    "multidict==6.0.4",
+    "requests==2.31.0",
+    "urllib3==2.0.3",
+    "yarl==1.9.2",
 ]
 
 test_requirements = [
     "pytest",
     "pytest-asyncio",
 ]
 
 setup(
     name="themoviedb",
     description="A modern and easy to use API wrapper for The Movie Database (TMDb) API v3 written in Python",
     long_description=readme,
     author="Leandro César",
     author_email="ccleandroc@gmail.com",
     url="https://github.com/leandcesar/themoviedb",
-    version="0.3.4",
+    version="0.3.5",
     license="MIT",
     python_requires=">=3.7",
     packages=find_packages(include=["themoviedb", "themoviedb.*"]),
     include_package_data=True,
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `themoviedb-0.3.4/themoviedb/aiotmdb.py` & `themoviedb-0.3.5/themoviedb/aiotmdb.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_async/__init__.py` & `themoviedb-0.3.5/themoviedb/routes_async/__init__.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_async/_base.py` & `themoviedb-0.3.5/themoviedb/routes_async/_base.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_async/authentication.py` & `themoviedb-0.3.5/themoviedb/routes_async/authentication.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_async/certifications.py` & `themoviedb-0.3.5/themoviedb/routes_async/certifications.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_async/collections.py` & `themoviedb-0.3.5/themoviedb/routes_async/collections.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_async/companies.py` & `themoviedb-0.3.5/themoviedb/routes_async/companies.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_async/credit.py` & `themoviedb-0.3.5/themoviedb/routes_async/credit.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_async/discover.py` & `themoviedb-0.3.5/themoviedb/routes_async/discover.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_async/episode_groups.py` & `themoviedb-0.3.5/themoviedb/routes_async/episode_groups.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_async/episodes.py` & `themoviedb-0.3.5/themoviedb/routes_async/episodes.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_async/find.py` & `themoviedb-0.3.5/themoviedb/routes_async/find.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_async/genres.py` & `themoviedb-0.3.5/themoviedb/routes_async/genres.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_async/guest.py` & `themoviedb-0.3.5/themoviedb/routes_async/guest.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_async/keywords.py` & `themoviedb-0.3.5/themoviedb/routes_async/keywords.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_async/movies.py` & `themoviedb-0.3.5/themoviedb/routes_async/movies.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_async/network.py` & `themoviedb-0.3.5/themoviedb/routes_async/network.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_async/people.py` & `themoviedb-0.3.5/themoviedb/routes_async/people.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_async/reviews.py` & `themoviedb-0.3.5/themoviedb/routes_async/reviews.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_async/search.py` & `themoviedb-0.3.5/themoviedb/routes_async/search.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_async/seasons.py` & `themoviedb-0.3.5/themoviedb/routes_async/seasons.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_async/trending.py` & `themoviedb-0.3.5/themoviedb/routes_async/trending.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_async/tv.py` & `themoviedb-0.3.5/themoviedb/routes_async/tv.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_async/watch_providers.py` & `themoviedb-0.3.5/themoviedb/routes_async/watch_providers.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_sync/__init__.py` & `themoviedb-0.3.5/themoviedb/routes_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_sync/_base.py` & `themoviedb-0.3.5/themoviedb/routes_sync/_base.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_sync/authentication.py` & `themoviedb-0.3.5/themoviedb/routes_sync/authentication.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_sync/certifications.py` & `themoviedb-0.3.5/themoviedb/routes_sync/certifications.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_sync/collections.py` & `themoviedb-0.3.5/themoviedb/routes_sync/collections.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_sync/companies.py` & `themoviedb-0.3.5/themoviedb/routes_sync/companies.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_sync/credit.py` & `themoviedb-0.3.5/themoviedb/routes_sync/credit.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_sync/discover.py` & `themoviedb-0.3.5/themoviedb/routes_sync/discover.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_sync/episode_groups.py` & `themoviedb-0.3.5/themoviedb/routes_sync/episode_groups.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_sync/episodes.py` & `themoviedb-0.3.5/themoviedb/routes_sync/episodes.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_sync/find.py` & `themoviedb-0.3.5/themoviedb/routes_sync/find.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_sync/genres.py` & `themoviedb-0.3.5/themoviedb/routes_sync/genres.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_sync/guest.py` & `themoviedb-0.3.5/themoviedb/routes_sync/guest.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_sync/keywords.py` & `themoviedb-0.3.5/themoviedb/routes_sync/keywords.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_sync/movies.py` & `themoviedb-0.3.5/themoviedb/routes_sync/movies.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_sync/network.py` & `themoviedb-0.3.5/themoviedb/routes_sync/network.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_sync/people.py` & `themoviedb-0.3.5/themoviedb/routes_sync/people.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_sync/reviews.py` & `themoviedb-0.3.5/themoviedb/routes_sync/reviews.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_sync/search.py` & `themoviedb-0.3.5/themoviedb/routes_sync/search.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_sync/seasons.py` & `themoviedb-0.3.5/themoviedb/routes_sync/seasons.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_sync/trending.py` & `themoviedb-0.3.5/themoviedb/routes_sync/trending.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_sync/tv.py` & `themoviedb-0.3.5/themoviedb/routes_sync/tv.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/routes_sync/watch_providers.py` & `themoviedb-0.3.5/themoviedb/routes_sync/watch_providers.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/schemas/__init__.py` & `themoviedb-0.3.5/themoviedb/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/schemas/_enums.py` & `themoviedb-0.3.5/themoviedb/schemas/_enums.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/schemas/_partial.py` & `themoviedb-0.3.5/themoviedb/schemas/_partial.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/schemas/_result.py` & `themoviedb-0.3.5/themoviedb/schemas/_result.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/schemas/alternative_titles.py` & `themoviedb-0.3.5/themoviedb/schemas/alternative_titles.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/schemas/authentication.py` & `themoviedb-0.3.5/themoviedb/schemas/authentication.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/schemas/certifications.py` & `themoviedb-0.3.5/themoviedb/schemas/certifications.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/schemas/companies.py` & `themoviedb-0.3.5/themoviedb/schemas/companies.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/schemas/credit.py` & `themoviedb-0.3.5/themoviedb/schemas/credit.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/schemas/credits.py` & `themoviedb-0.3.5/themoviedb/schemas/credits.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/schemas/episode_groups.py` & `themoviedb-0.3.5/themoviedb/schemas/episode_groups.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/schemas/episodes.py` & `themoviedb-0.3.5/themoviedb/schemas/episodes.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/schemas/external_ids.py` & `themoviedb-0.3.5/themoviedb/schemas/external_ids.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/schemas/images.py` & `themoviedb-0.3.5/themoviedb/schemas/images.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/schemas/list.py` & `themoviedb-0.3.5/themoviedb/schemas/list.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/schemas/movies.py` & `themoviedb-0.3.5/themoviedb/schemas/movies.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/schemas/multi.py` & `themoviedb-0.3.5/themoviedb/schemas/multi.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/schemas/people.py` & `themoviedb-0.3.5/themoviedb/schemas/people.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/schemas/rated.py` & `themoviedb-0.3.5/themoviedb/schemas/rated.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/schemas/release_date.py` & `themoviedb-0.3.5/themoviedb/schemas/release_date.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/schemas/reviews.py` & `themoviedb-0.3.5/themoviedb/schemas/reviews.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/schemas/seasons.py` & `themoviedb-0.3.5/themoviedb/schemas/seasons.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/schemas/translations.py` & `themoviedb-0.3.5/themoviedb/schemas/translations.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/schemas/tv.py` & `themoviedb-0.3.5/themoviedb/schemas/tv.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/schemas/videos.py` & `themoviedb-0.3.5/themoviedb/schemas/videos.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/schemas/watch_providers.py` & `themoviedb-0.3.5/themoviedb/schemas/watch_providers.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/tmdb.py` & `themoviedb-0.3.5/themoviedb/tmdb.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb/utils.py` & `themoviedb-0.3.5/themoviedb/utils.py`

 * *Files identical despite different names*

### Comparing `themoviedb-0.3.4/themoviedb.egg-info/PKG-INFO` & `themoviedb-0.3.5/themoviedb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: themoviedb
-Version: 0.3.4
+Version: 0.3.5
 Summary: A modern and easy to use API wrapper for The Movie Database (TMDb) API v3 written in Python
 Home-page: https://github.com/leandcesar/themoviedb
 Author: Leandro César
 Author-email: ccleandroc@gmail.com
 License: MIT
 Description: |Code Quality Score| |Code Grade| |Code Coverage| |PyPI Version| |Code style: black| |PyPI License|
```

### Comparing `themoviedb-0.3.4/themoviedb.egg-info/SOURCES.txt` & `themoviedb-0.3.5/themoviedb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

