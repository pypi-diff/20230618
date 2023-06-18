# Comparing `tmp/tekore-4.6.1.tar.gz` & `tmp/tekore-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tekore-4.6.1.tar", last modified: Thu May 25 06:12:13 2023, max compression
+gzip compressed data, was "tekore-5.0.0.tar", last modified: Sun Jun 18 18:59:55 2023, max compression
```

## Comparing `tekore-4.6.1.tar` & `tekore-5.0.0.tar`

### file list

```diff
@@ -1,200 +1,200 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.886470 tekore-4.6.1/
--rw-rw-rw-   0        0        0     1096 2023-01-06 17:05:20.000000 tekore-4.6.1/LICENSE
--rw-rw-rw-   0        0        0      156 2023-01-05 23:44:39.000000 tekore-4.6.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5362 2023-05-25 06:12:13.885970 tekore-4.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     4184 2023-01-05 23:44:39.000000 tekore-4.6.1/contributing.rst
-drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.799455 tekore-4.6.1/docs/
--rw-rw-rw-   0        0        0       89 2022-12-30 08:34:42.000000 tekore-4.6.1/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.806455 tekore-4.6.1/docs/src/
--rw-rw-rw-   0        0        0      311 2020-06-21 19:25:53.000000 tekore-4.6.1/docs/src/404.rst
--rw-rw-rw-   0        0        0     8153 2022-12-30 08:34:42.000000 tekore-4.6.1/docs/src/advanced_usage.rst
--rw-rw-rw-   0        0        0    12443 2022-12-30 08:34:42.000000 tekore-4.6.1/docs/src/auth_guide.rst
--rw-rw-rw-   0        0        0     1082 2023-01-06 17:05:20.000000 tekore-4.6.1/docs/src/conf.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.809956 tekore-4.6.1/docs/src/examples/
--rw-rw-rw-   0        0        0     1648 2020-08-27 18:40:55.000000 tekore-4.6.1/docs/src/examples/artist_follower.rst
--rw-rw-rw-   0        0        0     2177 2020-09-02 16:05:17.000000 tekore-4.6.1/docs/src/examples/async_server.rst
--rw-rw-rw-   0        0        0     7611 2021-09-08 13:22:42.000000 tekore-4.6.1/docs/src/examples/auth_server.rst
--rw-rw-rw-   0        0        0     2070 2020-09-02 16:24:55.000000 tekore-4.6.1/docs/src/examples/creating_scripts.rst
--rw-rw-rw-   0        0        0     2086 2021-01-10 19:32:00.000000 tekore-4.6.1/docs/src/examples/discord_bot.rst
-drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.814957 tekore-4.6.1/docs/src/examples/scripts/
--rw-rw-rw-   0        0        0      685 2020-08-27 18:37:41.000000 tekore-4.6.1/docs/src/examples/scripts/albums_top_artist.rst
--rw-rw-rw-   0        0        0     1073 2020-08-27 18:37:41.000000 tekore-4.6.1/docs/src/examples/scripts/analyse_from_playlist.rst
--rw-rw-rw-   0        0        0      793 2020-08-27 18:37:41.000000 tekore-4.6.1/docs/src/examples/scripts/follow_by_search.rst
--rw-rw-rw-   0        0        0      731 2020-08-27 18:37:41.000000 tekore-4.6.1/docs/src/examples/scripts/follow_category_playlist.rst
--rw-rw-rw-   0        0        0      670 2020-08-27 18:37:41.000000 tekore-4.6.1/docs/src/examples/scripts/play_saved_album.rst
--rw-rw-rw-   0        0        0     1045 2020-08-27 18:37:41.000000 tekore-4.6.1/docs/src/examples/scripts/recommended_playlist.rst
--rw-rw-rw-   0        0        0      976 2020-08-27 18:37:41.000000 tekore-4.6.1/docs/src/examples/scripts/related_artists_top_artist.rst
--rw-rw-rw-   0        0        0     3859 2022-05-02 15:56:27.000000 tekore-4.6.1/docs/src/examples/scripts/scrape_playlists.rst
--rw-rw-rw-   0        0        0      657 2020-08-27 18:37:41.000000 tekore-4.6.1/docs/src/examples/scripts/tracks_new_release.rst
--rw-rw-rw-   0        0        0      262 2020-06-21 19:25:53.000000 tekore-4.6.1/docs/src/examples/scripts.rst
--rw-rw-rw-   0        0        0      183 2020-06-21 19:25:53.000000 tekore-4.6.1/docs/src/examples.rst
--rw-rw-rw-   0        0        0     5076 2021-10-26 07:09:35.000000 tekore-4.6.1/docs/src/getting_started.rst
--rw-rw-rw-   0        0        0     2745 2020-09-02 15:00:17.000000 tekore-4.6.1/docs/src/index.rst
--rw-rw-rw-   0        0        0   143290 2021-01-11 16:43:14.000000 tekore-4.6.1/docs/src/logo.png
--rw-rw-rw-   0        0        0    22000 2021-01-11 16:43:14.000000 tekore-4.6.1/docs/src/logo_small.png
-drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.818957 tekore-4.6.1/docs/src/reference/
--rw-rw-rw-   0        0        0     2435 2021-01-10 19:32:00.000000 tekore-4.6.1/docs/src/reference/auth.rst
--rw-rw-rw-   0        0        0    12495 2022-12-30 08:34:42.000000 tekore-4.6.1/docs/src/reference/client.rst
--rw-rw-rw-   0        0        0     1252 2020-06-21 19:25:53.000000 tekore-4.6.1/docs/src/reference/config.rst
--rw-rw-rw-   0        0        0      823 2020-06-25 21:26:36.000000 tekore-4.6.1/docs/src/reference/conversions.rst
--rw-rw-rw-   0        0        0     1577 2022-12-30 08:34:42.000000 tekore-4.6.1/docs/src/reference/errors.rst
--rw-rw-rw-   0        0        0     7784 2022-12-30 08:34:42.000000 tekore-4.6.1/docs/src/reference/models.rst
--rw-rw-rw-   0        0        0     2003 2020-09-02 14:48:39.000000 tekore-4.6.1/docs/src/reference/senders.rst
--rw-rw-rw-   0        0        0      618 2022-12-30 08:34:42.000000 tekore-4.6.1/docs/src/reference.rst
--rw-rw-rw-   0        0        0    19851 2023-05-25 05:58:59.000000 tekore-4.6.1/docs/src/release_notes.rst
--rw-rw-rw-   0        0        0     1174 2020-09-02 14:48:39.000000 tekore-4.6.1/docs/src/resources.rst
--rw-rw-rw-   0        0        0     2069 2023-04-12 17:36:57.000000 tekore-4.6.1/pyproject.toml
--rw-rw-rw-   0        0        0     2901 2021-09-09 16:40:04.000000 tekore-4.6.1/readme_pypi.rst
-drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.821458 tekore-4.6.1/requirements/
--rw-rw-rw-   0        0        0       14 2023-01-05 23:44:39.000000 tekore-4.6.1/requirements/build
--rw-rw-rw-   0        0        0       72 2023-01-05 23:44:39.000000 tekore-4.6.1/requirements/checks
--rw-rw-rw-   0        0        0       50 2023-01-05 23:44:39.000000 tekore-4.6.1/requirements/dev
--rw-rw-rw-   0        0        0       65 2023-01-05 23:44:39.000000 tekore-4.6.1/requirements/docs
--rw-rw-rw-   0        0        0       54 2023-01-05 23:44:39.000000 tekore-4.6.1/requirements/tests
--rw-rw-rw-   0        0        0       42 2023-05-25 06:12:13.886470 tekore-4.6.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.792954 tekore-4.6.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.823958 tekore-4.6.1/src/tekore/
--rw-rw-rw-   0        0        0     2610 2023-05-25 05:58:59.000000 tekore-4.6.1/src/tekore/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.828959 tekore-4.6.1/src/tekore/_auth/
--rw-rw-rw-   0        0        0      393 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_auth/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.831460 tekore-4.6.1/src/tekore/_auth/expiring/
--rw-rw-rw-   0        0        0       72 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_auth/expiring/__init__.py
--rw-rw-rw-   0        0        0     9619 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_auth/expiring/client.py
--rw-rw-rw-   0        0        0     1603 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_auth/expiring/decor.py
--rw-rw-rw-   0        0        0     2869 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_auth/expiring/token.py
--rw-rw-rw-   0        0        0     9067 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_auth/refreshing.py
--rw-rw-rw-   0        0        0     5817 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_auth/scope.py
--rw-rw-rw-   0        0        0     8596 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_auth/util.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.834461 tekore-4.6.1/src/tekore/_client/
--rw-rw-rw-   0        0        0       27 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.841962 tekore-4.6.1/src/tekore/_client/api/
--rw-rw-rw-   0        0        0      584 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/__init__.py
--rw-rw-rw-   0        0        0     1955 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/album.py
--rw-rw-rw-   0        0        0     3186 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/artist.py
--rw-rw-rw-   0        0        0     2866 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/audiobook.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.842962 tekore-4.6.1/src/tekore/_client/api/browse/
--rw-rw-rw-   0        0        0     7095 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/browse/__init__.py
--rw-rw-rw-   0        0        0      663 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/browse/validate.py
--rw-rw-rw-   0        0        0     1761 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/chapter.py
--rw-rw-rw-   0        0        0     1762 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/episode.py
--rw-rw-rw-   0        0        0     5593 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/follow.py
--rw-rw-rw-   0        0        0     9081 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/library.py
--rw-rw-rw-   0        0        0      503 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/markets.py
--rw-rw-rw-   0        0        0     1853 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/personalisation.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.844462 tekore-4.6.1/src/tekore/_client/api/player/
--rw-rw-rw-   0        0        0      181 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/player/__init__.py
--rw-rw-rw-   0        0        0     7343 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/player/modify.py
--rw-rw-rw-   0        0        0     4091 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/player/view.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.846463 tekore-4.6.1/src/tekore/_client/api/playlist/
--rw-rw-rw-   0        0        0      256 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/playlist/__init__.py
--rw-rw-rw-   0        0        0     6142 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/playlist/items.py
--rw-rw-rw-   0        0        0     2770 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/playlist/modify.py
--rw-rw-rw-   0        0        0     7617 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/playlist/view.py
--rw-rw-rw-   0        0        0     3578 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/search.py
--rw-rw-rw-   0        0        0     2985 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/show.py
--rw-rw-rw-   0        0        0     2469 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/track.py
--rw-rw-rw-   0        0        0      951 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/user.py
--rw-rw-rw-   0        0        0     4407 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/base.py
--rw-rw-rw-   0        0        0     4194 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/chunked.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.847463 tekore-4.6.1/src/tekore/_client/decor/
--rw-rw-rw-   0        0        0     2861 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/decor/__init__.py
--rw-rw-rw-   0        0        0     1068 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/decor/handle.py
--rw-rw-rw-   0        0        0     4129 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/full.py
--rw-rw-rw-   0        0        0     4299 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/paging.py
--rw-rw-rw-   0        0        0     1316 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/process.py
--rw-rw-rw-   0        0        0     5922 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_config.py
--rw-rw-rw-   0        0        0     4051 2023-03-26 09:38:45.000000 tekore-4.6.1/src/tekore/_convert.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.857465 tekore-4.6.1/src/tekore/_model/
--rw-rw-rw-   0        0        0     2394 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.858965 tekore-4.6.1/src/tekore/_model/album/
--rw-rw-rw-   0        0        0     1442 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/album/__init__.py
--rw-rw-rw-   0        0        0      990 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/album/base.py
--rw-rw-rw-   0        0        0     1720 2023-05-25 05:45:42.000000 tekore-4.6.1/src/tekore/_model/album/full.py
--rw-rw-rw-   0        0        0     1369 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/artist.py
--rw-rw-rw-   0        0        0     2336 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/audio_analysis.py
--rw-rw-rw-   0        0        0      518 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/audio_features.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.860465 tekore-4.6.1/src/tekore/_model/audiobook/
--rw-rw-rw-   0        0        0      607 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/audiobook/__init__.py
--rw-rw-rw-   0        0        0     1140 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/audiobook/base.py
--rw-rw-rw-   0        0        0      468 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/audiobook/full.py
--rw-rw-rw-   0        0        0      335 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/base.py
--rw-rw-rw-   0        0        0      679 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/category.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.861966 tekore-4.6.1/src/tekore/_model/chapter/
--rw-rw-rw-   0        0        0      860 2023-03-26 09:38:45.000000 tekore-4.6.1/src/tekore/_model/chapter/__init__.py
--rw-rw-rw-   0        0        0      900 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/chapter/base.py
--rw-rw-rw-   0        0        0      627 2023-03-26 09:38:45.000000 tekore-4.6.1/src/tekore/_model/chapter/full.py
--rw-rw-rw-   0        0        0      522 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/context.py
--rw-rw-rw-   0        0        0     3070 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/currently_playing.py
--rw-rw-rw-   0        0        0      845 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/device.py
--rw-rw-rw-   0        0        0     2563 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/episode.py
--rw-rw-rw-   0        0        0     1747 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/error.py
--rw-rw-rw-   0        0        0     1362 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/local.py
--rw-rw-rw-   0        0        0     1110 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/member.py
--rw-rw-rw-   0        0        0      834 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/paging.py
--rw-rw-rw-   0        0        0     1291 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/play_history.py
--rw-rw-rw-   0        0        0     3789 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/playlist.py
--rw-rw-rw-   0        0        0     1259 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/recommendations.py
--rw-rw-rw-   0        0        0     7555 2023-04-12 17:42:29.000000 tekore-4.6.1/src/tekore/_model/serialise.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.862966 tekore-4.6.1/src/tekore/_model/show/
--rw-rw-rw-   0        0        0     1176 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/show/__init__.py
--rw-rw-rw-   0        0        0      907 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/show/base.py
--rw-rw-rw-   0        0        0      582 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/show/full.py
--rw-rw-rw-   0        0        0     4011 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/track.py
--rw-rw-rw-   0        0        0     1808 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/user.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.866466 tekore-4.6.1/src/tekore/_sender/
--rw-rw-rw-   0        0        0      466 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_sender/__init__.py
--rw-rw-rw-   0        0        0     1311 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_sender/base.py
--rw-rw-rw-   0        0        0     3286 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_sender/client.py
--rw-rw-rw-   0        0        0     3130 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_sender/concrete.py
--rw-rw-rw-   0        0        0     2881 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_sender/error.py
--rw-rw-rw-   0        0        0    10259 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_sender/extending.py
--rw-rw-rw-   0        0        0     4202 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/model.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.826959 tekore-4.6.1/src/tekore.egg-info/
--rw-rw-rw-   0        0        0     5362 2023-05-25 06:12:13.000000 tekore-4.6.1/src/tekore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4979 2023-05-25 06:12:13.000000 tekore-4.6.1/src/tekore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 06:12:13.000000 tekore-4.6.1/src/tekore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-25 06:12:13.000000 tekore-4.6.1/src/tekore.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-25 06:12:13.000000 tekore-4.6.1/src/tekore.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.869467 tekore-4.6.1/tests/
--rw-rw-rw-   0        0        0        0 2020-01-13 21:08:33.000000 tekore-4.6.1/tests/__init__.py
--rw-rw-rw-   0        0        0      407 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/_util.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.871967 tekore-4.6.1/tests/auth/
--rw-rw-rw-   0        0        0        0 2020-05-21 14:45:59.000000 tekore-4.6.1/tests/auth/__init__.py
--rw-rw-rw-   0        0        0     8738 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/auth/expiring.py
--rw-rw-rw-   0        0        0     2880 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/auth/refreshing.py
--rw-rw-rw-   0        0        0     5793 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/auth/scope.py
--rw-rw-rw-   0        0        0     5167 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/auth/util.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.882969 tekore-4.6.1/tests/client/
--rw-rw-rw-   0        0        0        0 2020-01-13 21:08:33.000000 tekore-4.6.1/tests/client/__init__.py
--rw-rw-rw-   0        0        0     2542 2023-05-25 05:51:13.000000 tekore-4.6.1/tests/client/_resources.py
--rw-rw-rw-   0        0        0     2123 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/client/album.py
--rw-rw-rw-   0        0        0     1833 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/client/artist.py
--rw-rw-rw-   0        0        0     1640 2023-03-26 09:38:45.000000 tekore-4.6.1/tests/client/audiobook.py
--rw-rw-rw-   0        0        0     1528 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/client/base.py
--rw-rw-rw-   0        0        0     3444 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/client/browse.py
--rw-rw-rw-   0        0        0     1315 2023-03-26 09:38:45.000000 tekore-4.6.1/tests/client/chapter.py
--rw-rw-rw-   0        0        0     1079 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/client/episode.py
--rw-rw-rw-   0        0        0     2267 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/client/follow.py
--rw-rw-rw-   0        0        0    13417 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/client/full.py
--rw-rw-rw-   0        0        0     3583 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/client/library.py
--rw-rw-rw-   0        0        0      130 2021-04-08 08:00:20.000000 tekore-4.6.1/tests/client/markets.py
--rw-rw-rw-   0        0        0     3652 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/client/paging.py
--rw-rw-rw-   0        0        0      229 2020-05-21 14:45:59.000000 tekore-4.6.1/tests/client/personalisation.py
--rw-rw-rw-   0        0        0     6147 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/client/player.py
--rw-rw-rw-   0        0        0     9110 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/client/playlist.py
--rw-rw-rw-   0        0        0     1103 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/client/search.py
--rw-rw-rw-   0        0        0      866 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/client/show.py
--rw-rw-rw-   0        0        0     3779 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/client/track.py
--rw-rw-rw-   0        0        0      477 2022-01-14 08:24:39.000000 tekore-4.6.1/tests/client/user.py
--rw-rw-rw-   0        0        0     6369 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/config.py
--rw-rw-rw-   0        0        0     3662 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/conftest.py
--rw-rw-rw-   0        0        0     3731 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/convert.py
--rw-rw-rw-   0        0        0      450 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/error.py
--rw-rw-rw-   0        0        0     6902 2023-04-12 17:33:26.000000 tekore-4.6.1/tests/model.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.885470 tekore-4.6.1/tests/sender/
--rw-rw-rw-   0        0        0        0 2020-05-21 14:45:59.000000 tekore-4.6.1/tests/sender/__init__.py
--rw-rw-rw-   0        0        0      296 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/sender/base.py
--rw-rw-rw-   0        0        0    10662 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/sender/caching.py
--rw-rw-rw-   0        0        0     1204 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/sender/client.py
--rw-rw-rw-   0        0        0     5995 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/sender/retrying.py
--rw-rw-rw-   0        0        0     2404 2023-04-12 18:04:45.000000 tekore-4.6.1/tox.ini
+drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.744243 tekore-5.0.0/
+-rw-rw-rw-   0        0        0     1096 2023-01-06 17:05:20.000000 tekore-5.0.0/LICENSE
+-rw-rw-rw-   0        0        0      156 2023-01-05 23:44:39.000000 tekore-5.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5311 2023-06-18 18:59:55.743743 tekore-5.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4184 2023-06-18 12:22:02.000000 tekore-5.0.0/contributing.rst
+drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.655228 tekore-5.0.0/docs/
+-rw-rw-rw-   0        0        0       89 2022-12-30 08:34:42.000000 tekore-5.0.0/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.661728 tekore-5.0.0/docs/src/
+-rw-rw-rw-   0        0        0      311 2020-06-21 19:25:53.000000 tekore-5.0.0/docs/src/404.rst
+-rw-rw-rw-   0        0        0     8153 2022-12-30 08:34:42.000000 tekore-5.0.0/docs/src/advanced_usage.rst
+-rw-rw-rw-   0        0        0    12443 2022-12-30 08:34:42.000000 tekore-5.0.0/docs/src/auth_guide.rst
+-rw-rw-rw-   0        0        0     1082 2023-01-06 17:05:20.000000 tekore-5.0.0/docs/src/conf.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.665229 tekore-5.0.0/docs/src/examples/
+-rw-rw-rw-   0        0        0     1648 2020-08-27 18:40:55.000000 tekore-5.0.0/docs/src/examples/artist_follower.rst
+-rw-rw-rw-   0        0        0     2177 2020-09-02 16:05:17.000000 tekore-5.0.0/docs/src/examples/async_server.rst
+-rw-rw-rw-   0        0        0     7611 2021-09-08 13:22:42.000000 tekore-5.0.0/docs/src/examples/auth_server.rst
+-rw-rw-rw-   0        0        0     2070 2020-09-02 16:24:55.000000 tekore-5.0.0/docs/src/examples/creating_scripts.rst
+-rw-rw-rw-   0        0        0     2086 2021-01-10 19:32:00.000000 tekore-5.0.0/docs/src/examples/discord_bot.rst
+drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.670230 tekore-5.0.0/docs/src/examples/scripts/
+-rw-rw-rw-   0        0        0      685 2020-08-27 18:37:41.000000 tekore-5.0.0/docs/src/examples/scripts/albums_top_artist.rst
+-rw-rw-rw-   0        0        0     1073 2020-08-27 18:37:41.000000 tekore-5.0.0/docs/src/examples/scripts/analyse_from_playlist.rst
+-rw-rw-rw-   0        0        0      793 2020-08-27 18:37:41.000000 tekore-5.0.0/docs/src/examples/scripts/follow_by_search.rst
+-rw-rw-rw-   0        0        0      731 2020-08-27 18:37:41.000000 tekore-5.0.0/docs/src/examples/scripts/follow_category_playlist.rst
+-rw-rw-rw-   0        0        0      670 2020-08-27 18:37:41.000000 tekore-5.0.0/docs/src/examples/scripts/play_saved_album.rst
+-rw-rw-rw-   0        0        0     1045 2020-08-27 18:37:41.000000 tekore-5.0.0/docs/src/examples/scripts/recommended_playlist.rst
+-rw-rw-rw-   0        0        0      976 2020-08-27 18:37:41.000000 tekore-5.0.0/docs/src/examples/scripts/related_artists_top_artist.rst
+-rw-rw-rw-   0        0        0     3859 2022-05-02 15:56:27.000000 tekore-5.0.0/docs/src/examples/scripts/scrape_playlists.rst
+-rw-rw-rw-   0        0        0      657 2020-08-27 18:37:41.000000 tekore-5.0.0/docs/src/examples/scripts/tracks_new_release.rst
+-rw-rw-rw-   0        0        0      262 2020-06-21 19:25:53.000000 tekore-5.0.0/docs/src/examples/scripts.rst
+-rw-rw-rw-   0        0        0      183 2020-06-21 19:25:53.000000 tekore-5.0.0/docs/src/examples.rst
+-rw-rw-rw-   0        0        0     5076 2021-10-26 07:09:35.000000 tekore-5.0.0/docs/src/getting_started.rst
+-rw-rw-rw-   0        0        0     2745 2020-09-02 15:00:17.000000 tekore-5.0.0/docs/src/index.rst
+-rw-rw-rw-   0        0        0   143290 2021-01-11 16:43:14.000000 tekore-5.0.0/docs/src/logo.png
+-rw-rw-rw-   0        0        0    22000 2021-01-11 16:43:14.000000 tekore-5.0.0/docs/src/logo_small.png
+drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.674231 tekore-5.0.0/docs/src/reference/
+-rw-rw-rw-   0        0        0     2435 2021-01-10 19:32:00.000000 tekore-5.0.0/docs/src/reference/auth.rst
+-rw-rw-rw-   0        0        0    12495 2022-12-30 08:34:42.000000 tekore-5.0.0/docs/src/reference/client.rst
+-rw-rw-rw-   0        0        0     1252 2020-06-21 19:25:53.000000 tekore-5.0.0/docs/src/reference/config.rst
+-rw-rw-rw-   0        0        0      823 2020-06-25 21:26:36.000000 tekore-5.0.0/docs/src/reference/conversions.rst
+-rw-rw-rw-   0        0        0     1577 2022-12-30 08:34:42.000000 tekore-5.0.0/docs/src/reference/errors.rst
+-rw-rw-rw-   0        0        0     7553 2023-06-18 17:59:26.000000 tekore-5.0.0/docs/src/reference/models.rst
+-rw-rw-rw-   0        0        0     2003 2020-09-02 14:48:39.000000 tekore-5.0.0/docs/src/reference/senders.rst
+-rw-rw-rw-   0        0        0      618 2022-12-30 08:34:42.000000 tekore-5.0.0/docs/src/reference.rst
+-rw-rw-rw-   0        0        0    20908 2023-06-18 18:36:40.000000 tekore-5.0.0/docs/src/release_notes.rst
+-rw-rw-rw-   0        0        0     1174 2020-09-02 14:48:39.000000 tekore-5.0.0/docs/src/resources.rst
+-rw-rw-rw-   0        0        0     2036 2023-06-18 18:52:59.000000 tekore-5.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0     2901 2021-09-09 16:40:04.000000 tekore-5.0.0/readme_pypi.rst
+drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.676731 tekore-5.0.0/requirements/
+-rw-rw-rw-   0        0        0       14 2023-01-05 23:44:39.000000 tekore-5.0.0/requirements/build
+-rw-rw-rw-   0        0        0       72 2023-01-05 23:44:39.000000 tekore-5.0.0/requirements/checks
+-rw-rw-rw-   0        0        0       50 2023-01-05 23:44:39.000000 tekore-5.0.0/requirements/dev
+-rw-rw-rw-   0        0        0       65 2023-01-05 23:44:39.000000 tekore-5.0.0/requirements/docs
+-rw-rw-rw-   0        0        0       54 2023-01-05 23:44:39.000000 tekore-5.0.0/requirements/tests
+-rw-rw-rw-   0        0        0       42 2023-06-18 18:59:55.744243 tekore-5.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.647226 tekore-5.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.678732 tekore-5.0.0/src/tekore/
+-rw-rw-rw-   0        0        0     2610 2023-06-18 18:37:26.000000 tekore-5.0.0/src/tekore/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.683732 tekore-5.0.0/src/tekore/_auth/
+-rw-rw-rw-   0        0        0      393 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_auth/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.685732 tekore-5.0.0/src/tekore/_auth/expiring/
+-rw-rw-rw-   0        0        0       72 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_auth/expiring/__init__.py
+-rw-rw-rw-   0        0        0     9619 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_auth/expiring/client.py
+-rw-rw-rw-   0        0        0     1603 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_auth/expiring/decor.py
+-rw-rw-rw-   0        0        0     2869 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_auth/expiring/token.py
+-rw-rw-rw-   0        0        0     9067 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_auth/refreshing.py
+-rw-rw-rw-   0        0        0     5817 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_auth/scope.py
+-rw-rw-rw-   0        0        0     8596 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_auth/util.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.688733 tekore-5.0.0/src/tekore/_client/
+-rw-rw-rw-   0        0        0       27 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.696234 tekore-5.0.0/src/tekore/_client/api/
+-rw-rw-rw-   0        0        0      584 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/api/__init__.py
+-rw-rw-rw-   0        0        0     1966 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_client/api/album.py
+-rw-rw-rw-   0        0        0     3160 2023-06-18 17:26:57.000000 tekore-5.0.0/src/tekore/_client/api/artist.py
+-rw-rw-rw-   0        0        0     2877 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_client/api/audiobook.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.697234 tekore-5.0.0/src/tekore/_client/api/browse/
+-rw-rw-rw-   0        0        0     7095 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/api/browse/__init__.py
+-rw-rw-rw-   0        0        0      663 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/api/browse/validate.py
+-rw-rw-rw-   0        0        0     1772 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_client/api/chapter.py
+-rw-rw-rw-   0        0        0     1773 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_client/api/episode.py
+-rw-rw-rw-   0        0        0     5593 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/api/follow.py
+-rw-rw-rw-   0        0        0     9081 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/api/library.py
+-rw-rw-rw-   0        0        0      503 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/api/markets.py
+-rw-rw-rw-   0        0        0     1853 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/api/personalisation.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.698735 tekore-5.0.0/src/tekore/_client/api/player/
+-rw-rw-rw-   0        0        0      181 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/api/player/__init__.py
+-rw-rw-rw-   0        0        0     7343 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/api/player/modify.py
+-rw-rw-rw-   0        0        0     4097 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_client/api/player/view.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.700735 tekore-5.0.0/src/tekore/_client/api/playlist/
+-rw-rw-rw-   0        0        0      256 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/api/playlist/__init__.py
+-rw-rw-rw-   0        0        0     6142 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/api/playlist/items.py
+-rw-rw-rw-   0        0        0     2770 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/api/playlist/modify.py
+-rw-rw-rw-   0        0        0     7576 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_client/api/playlist/view.py
+-rw-rw-rw-   0        0        0     3568 2023-06-18 16:08:44.000000 tekore-5.0.0/src/tekore/_client/api/search.py
+-rw-rw-rw-   0        0        0     2996 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_client/api/show.py
+-rw-rw-rw-   0        0        0     2475 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_client/api/track.py
+-rw-rw-rw-   0        0        0      951 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/api/user.py
+-rw-rw-rw-   0        0        0     4407 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/base.py
+-rw-rw-rw-   0        0        0     4130 2023-06-18 17:26:05.000000 tekore-5.0.0/src/tekore/_client/chunked.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.702235 tekore-5.0.0/src/tekore/_client/decor/
+-rw-rw-rw-   0        0        0     2861 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/decor/__init__.py
+-rw-rw-rw-   0        0        0     1068 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/decor/handle.py
+-rw-rw-rw-   0        0        0     4129 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/full.py
+-rw-rw-rw-   0        0        0     4259 2023-06-18 16:19:25.000000 tekore-5.0.0/src/tekore/_client/paging.py
+-rw-rw-rw-   0        0        0     1276 2023-06-18 17:38:50.000000 tekore-5.0.0/src/tekore/_client/process.py
+-rw-rw-rw-   0        0        0     5922 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_config.py
+-rw-rw-rw-   0        0        0     4051 2023-03-26 09:38:45.000000 tekore-5.0.0/src/tekore/_convert.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.712737 tekore-5.0.0/src/tekore/_model/
+-rw-rw-rw-   0        0        0     2322 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.714237 tekore-5.0.0/src/tekore/_model/album/
+-rw-rw-rw-   0        0        0      857 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_model/album/__init__.py
+-rw-rw-rw-   0        0        0      677 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_model/album/base.py
+-rw-rw-rw-   0        0        0      874 2023-06-18 17:28:56.000000 tekore-5.0.0/src/tekore/_model/album/full.py
+-rw-rw-rw-   0        0        0      707 2023-06-18 17:36:38.000000 tekore-5.0.0/src/tekore/_model/artist.py
+-rw-rw-rw-   0        0        0     1629 2023-06-18 17:27:56.000000 tekore-5.0.0/src/tekore/_model/audio_analysis.py
+-rw-rw-rw-   0        0        0      457 2023-06-18 14:22:16.000000 tekore-5.0.0/src/tekore/_model/audio_features.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.715737 tekore-5.0.0/src/tekore/_model/audiobook/
+-rw-rw-rw-   0        0        0      436 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_model/audiobook/__init__.py
+-rw-rw-rw-   0        0        0      743 2023-06-18 17:29:06.000000 tekore-5.0.0/src/tekore/_model/audiobook/base.py
+-rw-rw-rw-   0        0        0      184 2023-06-18 14:03:09.000000 tekore-5.0.0/src/tekore/_model/audiobook/full.py
+-rw-rw-rw-   0        0        0      250 2023-06-18 13:57:29.000000 tekore-5.0.0/src/tekore/_model/base.py
+-rw-rw-rw-   0        0        0      347 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_model/category.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.717238 tekore-5.0.0/src/tekore/_model/chapter/
+-rw-rw-rw-   0        0        0      320 2023-06-18 17:29:11.000000 tekore-5.0.0/src/tekore/_model/chapter/__init__.py
+-rw-rw-rw-   0        0        0      640 2023-06-18 17:29:14.000000 tekore-5.0.0/src/tekore/_model/chapter/base.py
+-rw-rw-rw-   0        0        0      171 2023-06-18 15:59:39.000000 tekore-5.0.0/src/tekore/_model/chapter/full.py
+-rw-rw-rw-   0        0        0      385 2023-06-18 14:22:16.000000 tekore-5.0.0/src/tekore/_model/context.py
+-rw-rw-rw-   0        0        0     1804 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_model/currently_playing.py
+-rw-rw-rw-   0        0        0      711 2023-06-18 14:22:16.000000 tekore-5.0.0/src/tekore/_model/device.py
+-rw-rw-rw-   0        0        0     1285 2023-06-18 17:28:10.000000 tekore-5.0.0/src/tekore/_model/episode.py
+-rw-rw-rw-   0        0        0     1747 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_model/error.py
+-rw-rw-rw-   0        0        0     1065 2023-06-18 17:28:13.000000 tekore-5.0.0/src/tekore/_model/local.py
+-rw-rw-rw-   0        0        0      941 2023-06-18 16:16:53.000000 tekore-5.0.0/src/tekore/_model/member.py
+-rw-rw-rw-   0        0        0      654 2023-06-18 17:17:07.000000 tekore-5.0.0/src/tekore/_model/paging.py
+-rw-rw-rw-   0        0        0      726 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_model/play_history.py
+-rw-rw-rw-   0        0        0     2308 2023-06-18 18:18:36.000000 tekore-5.0.0/src/tekore/_model/playlist.py
+-rw-rw-rw-   0        0        0      986 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_model/recommendations.py
+-rw-rw-rw-   0        0        0     1812 2023-06-18 17:24:30.000000 tekore-5.0.0/src/tekore/_model/serialise.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.719238 tekore-5.0.0/src/tekore/_model/show/
+-rw-rw-rw-   0        0        0      683 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_model/show/__init__.py
+-rw-rw-rw-   0        0        0      507 2023-06-18 17:29:22.000000 tekore-5.0.0/src/tekore/_model/show/base.py
+-rw-rw-rw-   0        0        0      343 2023-06-18 14:22:16.000000 tekore-5.0.0/src/tekore/_model/show/full.py
+-rw-rw-rw-   0        0        0     2095 2023-06-18 17:28:32.000000 tekore-5.0.0/src/tekore/_model/track.py
+-rw-rw-rw-   0        0        0     1209 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_model/user.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.722239 tekore-5.0.0/src/tekore/_sender/
+-rw-rw-rw-   0        0        0      466 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_sender/__init__.py
+-rw-rw-rw-   0        0        0     1311 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_sender/base.py
+-rw-rw-rw-   0        0        0     3286 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_sender/client.py
+-rw-rw-rw-   0        0        0     3130 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_sender/concrete.py
+-rw-rw-rw-   0        0        0     2881 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_sender/error.py
+-rw-rw-rw-   0        0        0    10259 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_sender/extending.py
+-rw-rw-rw-   0        0        0     4100 2023-06-18 17:26:16.000000 tekore-5.0.0/src/tekore/model.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.681732 tekore-5.0.0/src/tekore.egg-info/
+-rw-rw-rw-   0        0        0     5311 2023-06-18 18:59:55.000000 tekore-5.0.0/src/tekore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4979 2023-06-18 18:59:55.000000 tekore-5.0.0/src/tekore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 18:59:55.000000 tekore-5.0.0/src/tekore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-18 18:59:55.000000 tekore-5.0.0/src/tekore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-18 18:59:55.000000 tekore-5.0.0/src/tekore.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.725739 tekore-5.0.0/tests/
+-rw-rw-rw-   0        0        0        0 2020-01-13 21:08:33.000000 tekore-5.0.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      407 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/_util.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.729740 tekore-5.0.0/tests/auth/
+-rw-rw-rw-   0        0        0        0 2020-05-21 14:45:59.000000 tekore-5.0.0/tests/auth/__init__.py
+-rw-rw-rw-   0        0        0     8738 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/auth/expiring.py
+-rw-rw-rw-   0        0        0     2880 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/auth/refreshing.py
+-rw-rw-rw-   0        0        0     5793 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/auth/scope.py
+-rw-rw-rw-   0        0        0     5167 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/auth/util.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.740742 tekore-5.0.0/tests/client/
+-rw-rw-rw-   0        0        0        0 2020-01-13 21:08:33.000000 tekore-5.0.0/tests/client/__init__.py
+-rw-rw-rw-   0        0        0     2542 2023-05-25 05:51:13.000000 tekore-5.0.0/tests/client/_resources.py
+-rw-rw-rw-   0        0        0     2123 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/client/album.py
+-rw-rw-rw-   0        0        0     1833 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/client/artist.py
+-rw-rw-rw-   0        0        0     1640 2023-03-26 09:38:45.000000 tekore-5.0.0/tests/client/audiobook.py
+-rw-rw-rw-   0        0        0     1528 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/client/base.py
+-rw-rw-rw-   0        0        0     3444 2023-06-18 15:20:59.000000 tekore-5.0.0/tests/client/browse.py
+-rw-rw-rw-   0        0        0     1315 2023-03-26 09:38:45.000000 tekore-5.0.0/tests/client/chapter.py
+-rw-rw-rw-   0        0        0     1079 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/client/episode.py
+-rw-rw-rw-   0        0        0     2267 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/client/follow.py
+-rw-rw-rw-   0        0        0    13150 2023-06-18 17:29:58.000000 tekore-5.0.0/tests/client/full.py
+-rw-rw-rw-   0        0        0     3583 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/client/library.py
+-rw-rw-rw-   0        0        0      130 2021-04-08 08:00:20.000000 tekore-5.0.0/tests/client/markets.py
+-rw-rw-rw-   0        0        0     3619 2023-06-18 17:20:20.000000 tekore-5.0.0/tests/client/paging.py
+-rw-rw-rw-   0        0        0      229 2020-05-21 14:45:59.000000 tekore-5.0.0/tests/client/personalisation.py
+-rw-rw-rw-   0        0        0     6147 2023-06-18 18:52:49.000000 tekore-5.0.0/tests/client/player.py
+-rw-rw-rw-   0        0        0     9110 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/client/playlist.py
+-rw-rw-rw-   0        0        0     1103 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/client/search.py
+-rw-rw-rw-   0        0        0      866 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/client/show.py
+-rw-rw-rw-   0        0        0     3779 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/client/track.py
+-rw-rw-rw-   0        0        0      477 2022-01-14 08:24:39.000000 tekore-5.0.0/tests/client/user.py
+-rw-rw-rw-   0        0        0     6369 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/config.py
+-rw-rw-rw-   0        0        0     3662 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/conftest.py
+-rw-rw-rw-   0        0        0     3731 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/convert.py
+-rw-rw-rw-   0        0        0      450 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/error.py
+-rw-rw-rw-   0        0        0     2202 2023-06-18 17:51:35.000000 tekore-5.0.0/tests/model.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.743242 tekore-5.0.0/tests/sender/
+-rw-rw-rw-   0        0        0        0 2020-05-21 14:45:59.000000 tekore-5.0.0/tests/sender/__init__.py
+-rw-rw-rw-   0        0        0      296 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/sender/base.py
+-rw-rw-rw-   0        0        0    10662 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/sender/caching.py
+-rw-rw-rw-   0        0        0     1204 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/sender/client.py
+-rw-rw-rw-   0        0        0     5995 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/sender/retrying.py
+-rw-rw-rw-   0        0        0     2443 2023-06-18 17:19:58.000000 tekore-5.0.0/tox.ini
```

### Comparing `tekore-4.6.1/LICENSE` & `tekore-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/PKG-INFO` & `tekore-5.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tekore
-Version: 4.6.1
+Version: 5.0.0
 Summary: Client for the Spotify Web API
 Author-email: Felix Hildén <felix.hilden@gmail.com>
 Maintainer-email: Felix Hildén <felix.hilden@gmail.com>
 License: MIT License
         
         Copyright (c) 2019-2023 Felix Hildén
         
@@ -33,21 +33,20 @@
 Project-URL: Documentation, https://tekore.rtfd.org
 Keywords: spotify,web,api,client
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Sound/Audio
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 |logo|
 
 |python| |downloads|
```

### Comparing `tekore-4.6.1/contributing.rst` & `tekore-5.0.0/contributing.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/advanced_usage.rst` & `tekore-5.0.0/docs/src/advanced_usage.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/auth_guide.rst` & `tekore-5.0.0/docs/src/auth_guide.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/conf.py` & `tekore-5.0.0/docs/src/conf.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/examples/artist_follower.rst` & `tekore-5.0.0/docs/src/examples/artist_follower.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/examples/async_server.rst` & `tekore-5.0.0/docs/src/examples/async_server.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/examples/auth_server.rst` & `tekore-5.0.0/docs/src/examples/auth_server.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/examples/creating_scripts.rst` & `tekore-5.0.0/docs/src/examples/creating_scripts.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/examples/discord_bot.rst` & `tekore-5.0.0/docs/src/examples/discord_bot.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/examples/scripts/albums_top_artist.rst` & `tekore-5.0.0/docs/src/examples/scripts/albums_top_artist.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/examples/scripts/analyse_from_playlist.rst` & `tekore-5.0.0/docs/src/examples/scripts/analyse_from_playlist.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/examples/scripts/follow_by_search.rst` & `tekore-5.0.0/docs/src/examples/scripts/follow_by_search.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/examples/scripts/follow_category_playlist.rst` & `tekore-5.0.0/docs/src/examples/scripts/follow_category_playlist.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/examples/scripts/play_saved_album.rst` & `tekore-5.0.0/docs/src/examples/scripts/play_saved_album.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/examples/scripts/recommended_playlist.rst` & `tekore-5.0.0/docs/src/examples/scripts/recommended_playlist.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/examples/scripts/related_artists_top_artist.rst` & `tekore-5.0.0/docs/src/examples/scripts/related_artists_top_artist.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/examples/scripts/scrape_playlists.rst` & `tekore-5.0.0/docs/src/examples/scripts/scrape_playlists.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/examples/scripts/tracks_new_release.rst` & `tekore-5.0.0/docs/src/examples/scripts/tracks_new_release.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/getting_started.rst` & `tekore-5.0.0/docs/src/getting_started.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/index.rst` & `tekore-5.0.0/docs/src/index.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/logo.png` & `tekore-5.0.0/docs/src/logo.png`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/logo_small.png` & `tekore-5.0.0/docs/src/logo_small.png`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/reference/auth.rst` & `tekore-5.0.0/docs/src/reference/auth.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/reference/client.rst` & `tekore-5.0.0/docs/src/reference/client.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/reference/config.rst` & `tekore-5.0.0/docs/src/reference/config.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/reference/conversions.rst` & `tekore-5.0.0/docs/src/reference/conversions.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/reference/errors.rst` & `tekore-5.0.0/docs/src/reference/errors.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/reference/models.rst` & `tekore-5.0.0/docs/src/reference/models.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _models:
 .. currentmodule:: tekore.model
 
 Models
 ======
 Response model definitions for :ref:`client <client>`.
 
-Responses are parsed into model classes.
+Responses are parsed into `Pydantic <https://docs.pydantic.dev/latest/>`_ models.
 This allows accessing parts of the response directly as attributes.
 Further documentation on specific attribute values can be viewed in the Web API
 `reference <https://developer.spotify.com/documentation/web-api/reference/>`_.
 
 .. code:: python
 
     import tekore as tk
@@ -18,34 +18,32 @@
     spotify = tk.Spotify(token)
     album = spotify.album('3RBULTZJ97bvVzZLpxcB0j')
 
     # Use the response
     for track in album.tracks.items:
         print(track.track_number, track.name)
 
-Response models and lists of models are made easy to work with.
-They provide a readable ``repr`` for quickly inspecting the contents of a model
-and a :meth:`pprint <Serialisable.pprint>` method to view the model in more detail.
-It is also possible to convert models to builtin and JSON representations.
-See :class:`Serialisable` for more details on all available functionality.
+Using Pydantic models means that responses are easy to work with.
+They provide a readable ``repr`` (particularly with `devtools
+<https://docs.pydantic.dev/latest/usage/devtools/>`_) for quick inspection,
+and it is also possible to convert models to builtin and JSON representations:
 
 .. code:: python
 
+    from pprint import pprint
+
     print(album)
-    album.pprint()
-    album.pprint(depth=2)
+    pprint(album, depth=2)
 
-    album.asbuiltin()
+    album.dict()
     album.json()
 
 Responses will sometimes contain unknown attributes when the API changes.
-They are parsed into the response model,
-but are not included in serialisation and other model transforms.
-An :class:`UnknownModelAttributeWarning` is issued
-when encountering an unknown attribute.
+They are ignored when parsing the response model, but a
+:class:`UnknownModelAttributeWarning` is issued when encountering one.
 Please consider upgrading Tekore if a newer version documents and handles it.
 
 Models are made available in the :mod:`tekore.models` namespace.
 
 Album
 -----
 .. autosummary::
@@ -350,39 +348,34 @@
    :undoc-members:
 
 Model bases
 -----------
 .. autosummary::
    :nosignatures:
 
-   Serialisable
    Model
-   ModelList
    UnknownModelAttributeWarning
 
    Identifiable
    Item
    Paging
    OffsetPaging
    Cursor
    CursorPaging
 
 Functionality
 *************
-.. autoclass:: Serialisable
 .. autoclass:: Model
-.. autoclass:: ModelList
 .. autoclass:: UnknownModelAttributeWarning
 
 Models
 ******
 .. autoclass:: Identifiable
 .. autoclass:: Item
 .. autoclass:: Paging
 .. autoclass:: OffsetPaging
 .. autoclass:: Cursor
 .. autoclass:: CursorPaging
 
 Member types
 ------------
 .. autoclass:: StrEnum
-.. autoclass:: Timestamp
```

### Comparing `tekore-4.6.1/docs/src/reference/senders.rst` & `tekore-5.0.0/docs/src/reference/senders.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/reference.rst` & `tekore-5.0.0/docs/src/reference.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/docs/src/release_notes.rst` & `tekore-5.0.0/docs/src/release_notes.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,35 @@
 .. _release-notes:
 .. currentmodule:: tekore
 
 Release notes
 =============
+5.0.0 (2023-06-18)
+------------------
+Tekore 5 comes with an overhauled response model system based on Pydantic.
+Although the underlying change is major, the primary usage of models remains
+unchanged. The new models are more robust and easier to maintain.
+However, with more careful data validation new issues may arise. Please submit
+them on `GitHub <https://github.com/felix-hilden/tekore/issues>`_.
+
+Changed
+*******
+- Remove support for Python 3.7 (EOL) (:issue:`292`)
+- Use Pydantic in response models (:issue:`279`)
+
+  * Many type hints are fixed and improved.
+  * Instead of retaining unknown response attributes, they are now discarded.
+    However, the same warning message is raised.
+  * ``.json`` and ``.asbuiltin`` methods are replaced by Pydantic models'
+    ``.json`` and ``.dict``.
+  * Models use the builtin ``datetime`` object directly.
+  * ``.pprint`` and custom ``__repr__`` are removed in favor of using
+    Pydantic's own machinery.
+  * The builtin list class is used everywhere instead of the old ``ModelList``.
+
 4.6.1 (2023-05-25)
 ------------------
 Fixed
 *****
 - :class:`FullAlbum <model.FullAlbum>` - remove "album_group" attribute
   introduced in version 4.6.0 (:issue:`291`)
```

### Comparing `tekore-4.6.1/docs/src/resources.rst` & `tekore-5.0.0/docs/src/resources.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/pyproject.toml` & `tekore-5.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [build-system]
-requires = ["setuptools>=61.0", "wheel"]
+requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tekore"
 description = "Client for the Spotify Web API"
 readme = "readme_pypi.rst"
 license = {file = "LICENSE"}
 dynamic = ["version"]
 
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
     "httpx>=0.15,<0.25",
+    "pydantic>=1.8",
 ]
 
 keywords = ["spotify", "web", "api", "client"]
 authors = [{name = "Felix Hildén", email = "felix.hilden@gmail.com"}]
 maintainers = [{name = "Felix Hildén", email = "felix.hilden@gmail.com"}]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Multimedia :: Sound/Audio",
 ]
```

### Comparing `tekore-4.6.1/readme_pypi.rst` & `tekore-5.0.0/readme_pypi.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/__init__.py` & `tekore-5.0.0/src/tekore/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     ServerError,
     ServiceUnavailable,
     SyncSender,
     TooManyRequests,
     Unauthorised,
 )
 
-__version__ = "4.6.1"
+__version__ = "5.0.0"
 
 # Change the module of classes to hide module structure
 # and fix Sphinx base class links
 _classes = [
     Spotify,
     Credentials,
     Token,
```

### Comparing `tekore-4.6.1/src/tekore/_auth/expiring/client.py` & `tekore-5.0.0/src/tekore/_auth/expiring/client.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/_auth/expiring/decor.py` & `tekore-5.0.0/src/tekore/_auth/expiring/decor.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/_auth/expiring/token.py` & `tekore-5.0.0/src/tekore/_auth/expiring/token.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/_auth/refreshing.py` & `tekore-5.0.0/src/tekore/_auth/refreshing.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/_auth/scope.py` & `tekore-5.0.0/src/tekore/_auth/scope.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/_auth/util.py` & `tekore-5.0.0/src/tekore/_auth/util.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/_client/api/__init__.py` & `tekore-5.0.0/src/tekore/_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/_client/api/album.py` & `tekore-5.0.0/src/tekore/_client/api/album.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from tekore.model import FullAlbum, ModelList, SimpleTrackPaging
+from typing import List
+
+from tekore.model import FullAlbum, SimpleTrackPaging
 
 from ..base import SpotifyBase
 from ..chunked import chunked, join_lists
 from ..decor import maximise_limit, scopes, send_and_process
 from ..process import model_list, single
 
 
@@ -47,15 +49,15 @@
         return self._get(
             f"albums/{album_id}/tracks", market=market, limit=limit, offset=offset
         )
 
     @scopes()
     @chunked("album_ids", 1, 20, join_lists)
     @send_and_process(model_list(FullAlbum, "albums"))
-    def albums(self, album_ids: list, market: str = None) -> ModelList[FullAlbum]:
+    def albums(self, album_ids: list, market: str = None) -> List[FullAlbum]:
         """
         Get multiple albums.
 
         Parameters
         ----------
         album_ids
             list of album IDs, max 20 without chunking
```

### Comparing `tekore-4.6.1/src/tekore/_client/api/artist.py` & `tekore-5.0.0/src/tekore/_client/api/artist.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Union
 
-from tekore.model import AlbumGroup, FullArtist, FullTrack, ModelList, SimpleAlbumPaging
+from tekore.model import AlbumGroup, FullArtist, FullTrack, SimpleAlbumPaging
 
 from ..base import SpotifyBase
 from ..chunked import chunked, join_lists
 from ..decor import maximise_limit, scopes, send_and_process
 from ..process import model_list, single
 
 
@@ -23,15 +23,15 @@
             artist ID
         """
         return self._get("artists/" + artist_id)
 
     @scopes()
     @chunked("artist_ids", 1, 50, join_lists)
     @send_and_process(model_list(FullArtist, "artists"))
-    def artists(self, artist_ids: list) -> ModelList[FullArtist]:
+    def artists(self, artist_ids: list) -> List[FullArtist]:
         """
         Get information for multiple artists.
 
         Parameters
         ----------
         artist_ids
             list of artist IDs, max 50 without chunking
@@ -73,30 +73,30 @@
             market=market,
             limit=limit,
             offset=offset,
         )
 
     @scopes()
     @send_and_process(model_list(FullTrack, "tracks"))
-    def artist_top_tracks(self, artist_id: str, market: str) -> ModelList[FullTrack]:
+    def artist_top_tracks(self, artist_id: str, market: str) -> List[FullTrack]:
         """
         Get an artist's top 10 tracks by country.
 
         Parameters
         ----------
         artist_id
             the artist ID
         market
             an ISO 3166-1 alpha-2 country code or 'from_token'
         """
         return self._get(f"artists/{artist_id}/top-tracks", country=market)
 
     @scopes()
     @send_and_process(model_list(FullArtist, "artists"))
-    def artist_related_artists(self, artist_id: str) -> ModelList[FullArtist]:
+    def artist_related_artists(self, artist_id: str) -> List[FullArtist]:
         """
         Get artists similar to an identified artist.
 
         Similarity is based on analysis of
         the Spotify community's listening history.
 
         Parameters
```

### Comparing `tekore-4.6.1/src/tekore/_client/api/audiobook.py` & `tekore-5.0.0/src/tekore/_client/api/audiobook.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from tekore.model import FullAudiobook, ModelList, SimpleChapterPaging
+from typing import List
+
+from tekore.model import FullAudiobook, SimpleChapterPaging
 
 from ..base import SpotifyBase
 from ..chunked import chunked, join_lists
 from ..decor import maximise_limit, scopes, send_and_process
 from ..process import model_list, single
 
 
@@ -29,15 +31,15 @@
         return self._get("audiobooks/" + audiobook_id, market=market)
 
     @scopes()
     @chunked("audiobook_ids", 1, 50, join_lists)
     @send_and_process(model_list(FullAudiobook, "audiobooks"))
     def audiobooks(
         self, audiobook_ids: list, market: str = None
-    ) -> ModelList[FullAudiobook]:
+    ) -> List[FullAudiobook]:
         """
         Get information for multiple audiobooks.
 
         Parameters
         ----------
         audiobook_ids
             the audiobook IDs, max 50 without chunking
```

### Comparing `tekore-4.6.1/src/tekore/_client/api/browse/__init__.py` & `tekore-5.0.0/src/tekore/_client/api/browse/__init__.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/_client/api/browse/validate.py` & `tekore-5.0.0/src/tekore/_client/api/browse/validate.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/_client/api/chapter.py` & `tekore-5.0.0/src/tekore/_client/api/chapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from tekore.model import FullChapter, ModelList
+from typing import List
+
+from tekore.model import FullChapter
 
 from ..base import SpotifyBase
 from ..chunked import chunked, join_lists
 from ..decor import scopes, send_and_process
 from ..process import model_list, single
 
 
@@ -27,15 +29,15 @@
             the episode is considered unavailable.
         """
         return self._get("chapters/" + chapter_id, market=market)
 
     @scopes()
     @chunked("chapter_ids", 1, 50, join_lists)
     @send_and_process(model_list(FullChapter, "chapters"))
-    def chapters(self, chapter_ids: list, market: str = None) -> ModelList[FullChapter]:
+    def chapters(self, chapter_ids: list, market: str = None) -> List[FullChapter]:
         """
         Get information for multiple chapters.
 
         Parameters
         ----------
         chapter_ids
             the chapter IDs, max 50 without chunking
```

### Comparing `tekore-4.6.1/src/tekore/_client/api/episode.py` & `tekore-5.0.0/src/tekore/_client/api/episode.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from tekore.model import FullEpisode, ModelList
+from typing import List
+
+from tekore.model import FullEpisode
 
 from ..base import SpotifyBase
 from ..chunked import chunked, join_lists
 from ..decor import scopes, send_and_process
 from ..process import model_list, single
 
 
@@ -27,15 +29,15 @@
             the episode is considered unavailable.
         """
         return self._get("episodes/" + episode_id, market=market)
 
     @scopes()
     @chunked("episode_ids", 1, 50, join_lists)
     @send_and_process(model_list(FullEpisode, "episodes"))
-    def episodes(self, episode_ids: list, market: str = None) -> ModelList[FullEpisode]:
+    def episodes(self, episode_ids: list, market: str = None) -> List[FullEpisode]:
         """
         Get information for multiple episodes.
 
         Parameters
         ----------
         episode_ids
             the episode IDs, max 50 without chunking
```

### Comparing `tekore-4.6.1/src/tekore/_client/api/follow.py` & `tekore-5.0.0/src/tekore/_client/api/follow.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/_client/api/library.py` & `tekore-5.0.0/src/tekore/_client/api/library.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/_client/api/personalisation.py` & `tekore-5.0.0/src/tekore/_client/api/personalisation.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/_client/api/player/modify.py` & `tekore-5.0.0/src/tekore/_client/api/player/modify.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/_client/api/player/view.py` & `tekore-5.0.0/src/tekore/_client/api/player/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+from typing import List
+
 from tekore._auth import scope
 from tekore.model import (
     CurrentlyPlaying,
     CurrentlyPlayingContext,
     Device,
-    ModelList,
     PlayHistoryPaging,
     Queue,
 )
 
 from ...base import SpotifyBase
 from ...decor import maximise_limit, scopes, send_and_process
 from ...process import model_list, single
@@ -103,15 +104,15 @@
         """
         return self._get(
             "me/player/recently-played", limit=limit, after=after, before=before
         )
 
     @scopes([scope.user_read_playback_state])
     @send_and_process(model_list(Device, "devices"))
-    def playback_devices(self) -> ModelList[Device]:
+    def playback_devices(self) -> List[Device]:
         """Get a user's available devices."""
         return self._get("me/player/devices")
 
     @scopes([scope.user_read_playback_state])
     @send_and_process(single(Queue))
     def playback_queue(self) -> Queue:
         """
```

### Comparing `tekore-4.6.1/src/tekore/_client/api/playlist/items.py` & `tekore-5.0.0/src/tekore/_client/api/playlist/items.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/_client/api/playlist/modify.py` & `tekore-5.0.0/src/tekore/_client/api/playlist/modify.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/_client/api/playlist/view.py` & `tekore-5.0.0/src/tekore/_client/api/playlist/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,12 @@
 from functools import wraps
-from typing import Callable, Iterable, Union
+from typing import Callable, Iterable, List, Union
 
 from tekore._auth import scope
-from tekore.model import (
-    FullPlaylist,
-    Image,
-    ModelList,
-    PlaylistTrackPaging,
-    SimplePlaylistPaging,
-)
+from tekore.model import FullPlaylist, Image, PlaylistTrackPaging, SimplePlaylistPaging
 
 from ...base import SpotifyBase
 from ...chunked import _get_arg
 from ...decor import maximise_limit, scopes, send_and_process
 from ...process import model_list, nothing, single
 
 
@@ -155,15 +149,15 @@
             fields=fields,
             market=market,
             additional_types=additional_types,
         )
 
     @scopes()
     @send_and_process(model_list(Image))
-    def playlist_cover_image(self, playlist_id: str) -> ModelList[Image]:
+    def playlist_cover_image(self, playlist_id: str) -> List[Image]:
         """
         Get cover image of a playlist.
 
         .. note:: Returns a list of images.
 
         Parameters
         ----------
```

### Comparing `tekore-4.6.1/src/tekore/_client/api/search.py` & `tekore-5.0.0/src/tekore/_client/api/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "shows": SimpleShowPaging,
     "tracks": FullTrackPaging,
 }
 
 
 def search_result(json: dict):
     """Unpack search result dicts into respective paging type constructors."""
-    return tuple(paging_type[key].from_kwargs(json[key]) for key in json.keys())
+    return tuple(paging_type[key](**json[key]) for key in json.keys())
 
 
 class SpotifySearch(SpotifyBase):
     """Search API endpoints."""
 
     @scopes()
     @send_and_process(search_result)
```

### Comparing `tekore-4.6.1/src/tekore/_client/api/show.py` & `tekore-5.0.0/src/tekore/_client/api/show.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from typing import List
+
 from tekore._auth import scope
-from tekore.model import FullShow, ModelList, SimpleEpisodePaging
+from tekore.model import FullShow, SimpleEpisodePaging
 
 from ..base import SpotifyBase
 from ..chunked import chunked, join_lists
 from ..decor import maximise_limit, scopes, send_and_process
 from ..process import model_list, single
 
 
@@ -31,15 +33,15 @@
             the show is considered unavailable.
         """
         return self._get("shows/" + show_id, market=market)
 
     @scopes(optional=[scope.user_read_playback_position])
     @chunked("show_ids", 1, 50, join_lists)
     @send_and_process(model_list(FullShow, "shows"))
-    def shows(self, show_ids: list, market: str = None) -> ModelList[FullShow]:
+    def shows(self, show_ids: list, market: str = None) -> List[FullShow]:
         """
         Get information for multiple shows.
 
         The user-read-playback-position scope allows
         episode resume points to be returned.
 
         Parameters
```

### Comparing `tekore-4.6.1/src/tekore/_client/api/track.py` & `tekore-5.0.0/src/tekore/_client/api/track.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from tekore.model import AudioAnalysis, AudioFeatures, FullTrack, ModelList
+from typing import List
+
+from tekore.model import AudioAnalysis, AudioFeatures, FullTrack
 
 from ..base import SpotifyBase
 from ..chunked import chunked, join_lists
 from ..decor import scopes, send_and_process
 from ..process import model_list, single
 
 
@@ -23,15 +25,15 @@
             an ISO 3166-1 alpha-2 country code or 'from_token'
         """
         return self._get("tracks/" + track_id, market=market)
 
     @scopes()
     @chunked("track_ids", 1, 50, join_lists)
     @send_and_process(model_list(FullTrack, "tracks"))
-    def tracks(self, track_ids: list, market: str = None) -> ModelList[FullTrack]:
+    def tracks(self, track_ids: list, market: str = None) -> List[FullTrack]:
         """
         Get information for multiple tracks.
 
         Parameters
         ----------
         track_ids
             the track IDs, max 50 without chunking
@@ -56,15 +58,15 @@
     def track_audio_features(self, track_id: str) -> AudioFeatures:
         """Get audio feature information for a track."""
         return self._get("audio-features/" + track_id)
 
     @scopes()
     @chunked("track_ids", 1, 100, join_lists)
     @send_and_process(model_list(AudioFeatures, "audio_features"))
-    def tracks_audio_features(self, track_ids: list) -> ModelList[AudioFeatures]:
+    def tracks_audio_features(self, track_ids: list) -> List[AudioFeatures]:
         """
         Get audio feature information for multiple tracks.
 
         Feature information for a track may be ``None`` if not available.
 
         Parameters
         ----------
```

### Comparing `tekore-4.6.1/src/tekore/_client/api/user.py` & `tekore-5.0.0/src/tekore/_client/api/user.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/_client/base.py` & `tekore-5.0.0/src/tekore/_client/base.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/_client/chunked.py` & `tekore-5.0.0/src/tekore/_client/chunked.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from functools import wraps
 from typing import Callable
 
-from tekore.model import ModelList
-
 
 def _chunks(lst: list, n: int, reverse: bool) -> list:
     """
     Chunk list into length 'n' sublists.
 
     Parameters
     ----------
@@ -132,16 +130,16 @@
 
         return wrapper
 
     return decorator
 
 
 def join_lists(responses):
-    """Join lists of models into ModelList."""
-    return ModelList(sum(responses, []))
+    """Join lists of models."""
+    return sum(responses, [])
 
 
 def return_none(_):
     """Return None always."""
     return None
```

### Comparing `tekore-4.6.1/src/tekore/_client/decor/__init__.py` & `tekore-5.0.0/src/tekore/_client/decor/__init__.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/_client/decor/handle.py` & `tekore-5.0.0/src/tekore/_client/decor/handle.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/_client/full.py` & `tekore-5.0.0/src/tekore/_client/full.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/_client/paging.py` & `tekore-5.0.0/src/tekore/_client/paging.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,25 +42,25 @@
             return self._async_next(page)
 
         if page.next is None:
             return
 
         try:
             next_set = self._get_paging_result(page.next)
-            return type(page).from_kwargs(next_set)
+            return type(page)(**next_set)
         except BadRequest:
             return
 
     async def _async_next(self, page: Paging) -> Optional[Paging]:
         if page.next is None:
             return
 
         try:
             next_set = await self._get_paging_result(page.next)
-            return type(page).from_kwargs(next_set)
+            return type(page)(**next_set)
         except BadRequest:
             return
 
     def previous(self, page: OffsetPaging) -> Optional[OffsetPaging]:
         """
         Retrieve the previous result set of a paging object.
 
@@ -77,22 +77,22 @@
         if self.is_async:
             return self._async_previous(page)
 
         if page.previous is None:
             return
 
         previous_set = self._get_paging_result(page.previous)
-        return type(page).from_kwargs(previous_set)
+        return type(page)(**previous_set)
 
     async def _async_previous(self, page: OffsetPaging) -> Optional[OffsetPaging]:
         if page.previous is None:
             return
 
         previous_set = await self._get_paging_result(page.previous)
-        return type(page).from_kwargs(previous_set)
+        return type(page)(**previous_set)
 
     def all_pages(self, page: Paging) -> Generator[Paging, None, None]:
         """
         Retrieve all pages of a paging.
 
         Request and yield new (next) pages until the end of the paging.
         The paging that was given as an argument is yielded as the first result.
```

### Comparing `tekore-4.6.1/src/tekore/_client/process.py` & `tekore-5.0.0/src/tekore/_client/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Callable
 
-from tekore.model import Model, ModelList
+from tekore.model import Model
 
 
 def nothing(json):
     """Pass value without doing anything."""
     return json
 
 
@@ -22,25 +22,25 @@
     Unpack dict or items in ``from_item`` into single constructor.
 
     If dict or ``from_item`` is None - does nothing and returns None.
     """
 
     def post_func(json: dict):
         json = json if from_item is None else json[from_item]
-        return type_.from_kwargs(json) if json is not None else None
+        return type_(**json) if json is not None else None
 
     return post_func
 
 
 def model_list(type_: Model, from_item: str = None) -> Callable:
     """Unpack items inside ``from_item`` of dict into constructors."""
 
     def post_func(json: dict):
         json = json if from_item is None else json[from_item]
-        return ModelList(type_.from_kwargs(i) if i is not None else None for i in json)
+        return [type_(**i) if i is not None else None for i in json]
 
     return post_func
 
 
 def multiple(*args: Callable):
     """Run json dict through multiple processors."""
```

### Comparing `tekore-4.6.1/src/tekore/_config.py` & `tekore-5.0.0/src/tekore/_config.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/_convert.py` & `tekore-5.0.0/src/tekore/_convert.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/_model/__init__.py` & `tekore-5.0.0/src/tekore/_model/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,22 +64,15 @@
     SimplePlaylistPaging,
 )
 from .recommendations import (
     RecommendationAttribute,
     Recommendations,
     RecommendationSeed,
 )
-from .serialise import (
-    Model,
-    ModelList,
-    Serialisable,
-    StrEnum,
-    Timestamp,
-    UnknownModelAttributeWarning,
-)
+from .serialise import Model, StrEnum, UnknownModelAttributeWarning
 from .show import SavedShow, SavedShowPaging, Show, SimpleShow, SimpleShowPaging
 from .show.full import FullShow
 from .track import (
     FullTrack,
     FullTrackPaging,
     SavedTrack,
     SavedTrackPaging,
```

### Comparing `tekore-4.6.1/src/tekore/_model/album/__init__.py` & `tekore-5.0.0/src/tekore/_model/album/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,34 @@
-from dataclasses import dataclass
 from typing import List, Optional
 
 from ..album.base import Album, AlbumType
 from ..paging import OffsetPaging
-from ..serialise import ModelList, StrEnum
+from ..serialise import StrEnum
 
 
 class AlbumGroup(StrEnum):
     """Relationship between artist and album."""
 
     album = "album"
     appears_on = "appears_on"
     compilation = "compilation"
     single = "single"
 
 
-@dataclass(repr=False)
 class SimpleAlbum(Album):
     """
     Simplified album object.
 
     :attr:`album_group` is available when getting an artist's albums.
     :attr:`available_markets` is available when market is not specified.
 
     The presence of :attr:`is_playable` is undocumented
     and it appears to only be ``True`` when it is present.
     """
 
     album_group: Optional[AlbumGroup] = None
-    available_markets: Optional[List[str]] = None
-    is_playable: Optional[bool] = None
 
-    def __post_init__(self):
-        super().__post_init__()
-        if self.album_group is not None:
-            self.album_group = AlbumGroup[self.album_group]
-        if self.available_markets is not None:
-            self.available_markets = ModelList(self.available_markets)
 
-
-@dataclass(repr=False)
 class SimpleAlbumPaging(OffsetPaging):
     """Paging containing simplified albums."""
 
     items: List[SimpleAlbum]
-
-    def __post_init__(self):
-        self.items = ModelList(SimpleAlbum.from_kwargs(a) for a in self.items)
```

### Comparing `tekore-4.6.1/src/tekore/_model/album/base.py` & `tekore-5.0.0/src/tekore/_model/album/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,29 @@
-from dataclasses import dataclass
-from typing import List
+from typing import List, Optional
 
 from ..artist import SimpleArtist
 from ..base import Item
 from ..member import Image, ReleaseDatePrecision
-from ..serialise import ModelList, StrEnum
+from ..serialise import StrEnum
 
 
 class AlbumType(StrEnum):
     """Type of album."""
 
     album = "album"
     compilation = "compilation"
     single = "single"
 
 
-@dataclass(repr=False)
 class Album(Item):
     """Album base."""
 
     album_type: AlbumType
     artists: List[SimpleArtist]
     external_urls: dict
     images: List[Image]
     name: str
     total_tracks: int
     release_date: str
     release_date_precision: ReleaseDatePrecision
-
-    def __post_init__(self):
-        self.album_type = AlbumType[self.album_type.lower()]
-        self.artists = ModelList(SimpleArtist.from_kwargs(a) for a in self.artists)
-        self.images = ModelList(Image.from_kwargs(i) for i in self.images)
-        self.release_date_precision = ReleaseDatePrecision[self.release_date_precision]
+    available_markets: Optional[List[str]] = None
+    is_playable: Optional[bool] = None
```

### Comparing `tekore-4.6.1/src/tekore/_model/chapter/__init__.py` & `tekore-5.0.0/src/tekore/_model/show/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,34 @@
-from dataclasses import dataclass
-from typing import List, Optional
+from datetime import datetime
+from typing import List
 
-from ..member import Restrictions
 from ..paging import OffsetPaging
-from ..serialise import ModelList
-from .base import Chapter
+from ..serialise import Model
+from ..show.base import Show
 
 
-@dataclass(repr=False)
-class SimpleChapter(Chapter):
-    """Simplified chapter."""
+class SimpleShow(Show):
+    """
+    Simplified show object.
 
-    available_markets: List[str] = None
-    is_playable: Optional[bool] = None
-    restrictions: Optional[Restrictions] = None
+    :attr:`total_episodes` is undocumented by Spotify,
+    so it might be missing or removed in a future version.
+    """
 
-    def __post_init__(self):
-        super().__post_init__()
-        if self.restrictions:
-            self.restrictions = Restrictions.from_kwargs(self.restrictions)
 
+class SimpleShowPaging(OffsetPaging):
+    """Paging of simplified shows."""
 
-@dataclass(repr=False)
-class SimpleChapterPaging(OffsetPaging):
-    """Paging of simplified chapters."""
+    items: List[SimpleShow]
 
-    items = List[SimpleChapter]
 
-    def __post_init__(self):
-        self.items = ModelList(SimpleChapter.from_kwargs(i) for i in self.items)
+class SavedShow(Model):
+    """Show saved in library."""
+
+    added_at: datetime
+    show: SimpleShow
+
+
+class SavedShowPaging(OffsetPaging):
+    """Paging of shows in library."""
+
+    items: List[SavedShow]
```

### Comparing `tekore-4.6.1/src/tekore/_model/chapter/base.py` & `tekore-5.0.0/src/tekore/_model/audiobook/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,37 @@
-from dataclasses import dataclass
 from typing import List, Optional
 
 from ..base import Item
-from ..member import Image, ReleaseDatePrecision, ResumePoint
-from ..serialise import ModelList
+from ..member import Copyright, Image
+from ..serialise import Model
 
 
-@dataclass(repr=False)
-class Chapter(Item):
-    """Audiobook chapter base."""
+class Author(Model):
+    """Audiobook author."""
 
-    audio_preview_url: Optional[str]
-    chapter_number: int
+    name: str
+
+
+class Narrator(Model):
+    """Audiobook narrator."""
+
+    name: str
+
+
+class Audiobook(Item):
+    """Audiobook base."""
+
+    authors: List[Author]
+    available_markets: Optional[List[str]] = None
+    copyrights: List[Copyright]
     description: str
-    duration_ms: int
+    edition: Optional[str]
     explicit: bool
     external_urls: dict
     html_description: str
     images: List[Image]
     languages: List[str]
+    media_type: str
     name: str
-    release_date: str
-    release_date_precision: ReleaseDatePrecision
-    resume_point: ResumePoint
-
-    def __post_init__(self):
-        self.images = ModelList(Image.from_kwargs(i) for i in self.images)
-        self.release_date_precision = ReleaseDatePrecision[self.release_date_precision]
-        self.resume_point = ResumePoint.from_kwargs(self.resume_point)
+    narrators: List[Narrator]
+    publisher: str
+    total_chapters: Optional[int]
```

### Comparing `tekore-4.6.1/src/tekore/_model/device.py` & `tekore-5.0.0/src/tekore/_model/device.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from dataclasses import dataclass
 from typing import Optional
 
 from .base import Identifiable
 from .serialise import StrEnum
 
 
 class DeviceType(StrEnum):
@@ -19,20 +18,16 @@
     GameConsole = "GameConsole"
     CastVideo = "CastVideo"
     CastAudio = "CastAudio"
     Automobile = "Automobile"
     Unknown = "Unknown"
 
 
-@dataclass(repr=False)
 class Device(Identifiable):
     """Playback device."""
 
     is_active: bool
     is_private_session: bool
     is_restricted: bool
     name: str
     type: DeviceType
     volume_percent: Optional[int]
-
-    def __post_init__(self):
-        self.type = DeviceType[self.type]
```

### Comparing `tekore-4.6.1/src/tekore/_model/error.py` & `tekore-5.0.0/src/tekore/_model/error.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/_model/member.py` & `tekore-5.0.0/src/tekore/_model/member.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,56 @@
-from dataclasses import dataclass
 from typing import Optional
 
 from .serialise import Model, StrEnum
 
 
 class ReleaseDatePrecision(StrEnum):
     """Precision of a release date."""
 
     year = "year"
     month = "month"
     day = "day"
     minute = "minute"
 
 
-@dataclass(repr=False)
 class Copyright(Model):
     """Copyright."""
 
     text: str
     type: str
 
 
-@dataclass(repr=False)
 class Followers(Model):
     """
     Followers.
 
     :attr:`href` is always ``None``.
     """
 
     href: None
     total: int
 
 
-@dataclass(repr=False)
 class Image(Model):
     """
     Image link and information.
 
     The Web API documentation reports that :attr:`height` and :attr:`width`
     can be ``None`` or not available in the response.
     """
 
     url: str
-    height: Optional[int] = None
-    width: Optional[int] = None
+    height: Optional[int]
+    width: Optional[int]
 
 
-@dataclass(repr=False)
 class Restrictions(Model):
     """Restrictions on relinked resource."""
 
     reason: str
 
 
-@dataclass(repr=False)
 class ResumePoint(Model):
     """Resume point."""
 
     fully_played: bool
     resume_position_ms: int
```

### Comparing `tekore-4.6.1/src/tekore/_model/recommendations.py` & `tekore-5.0.0/src/tekore/_model/recommendations.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from dataclasses import dataclass
-from typing import List
+from typing import List, Optional
 
 from .base import Identifiable
-from .serialise import Model, ModelList, StrEnum
+from .serialise import Model, StrEnum
 from .track import FullTrack
 
 
 class RecommendationAttribute(StrEnum):
     """Attributes available in recommendations."""
 
     acousticness = "acousticness"
@@ -21,28 +20,22 @@
     popularity = "popularity"
     speechiness = "speechiness"
     tempo = "tempo"
     time_signature = "time_signature"
     valence = "valence"
 
 
-@dataclass(repr=False)
 class RecommendationSeed(Identifiable):
     """Recommendation seeds."""
 
     afterFilteringSize: int
     afterRelinkingSize: int
-    href: str
+    href: Optional[str]
     initialPoolSize: int
     type: str
 
 
-@dataclass(repr=False)
 class Recommendations(Model):
     """Track recommendations."""
 
     seeds: List[RecommendationSeed]
     tracks: List[FullTrack]
-
-    def __post_init__(self):
-        self.seeds = ModelList(RecommendationSeed.from_kwargs(s) for s in self.seeds)
-        self.tracks = ModelList(FullTrack.from_kwargs(t) for t in self.tracks)
```

### Comparing `tekore-4.6.1/src/tekore/_sender/base.py` & `tekore-5.0.0/src/tekore/_sender/base.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/_sender/client.py` & `tekore-5.0.0/src/tekore/_sender/client.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/_sender/concrete.py` & `tekore-5.0.0/src/tekore/_sender/concrete.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/_sender/error.py` & `tekore-5.0.0/src/tekore/_sender/error.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/_sender/extending.py` & `tekore-5.0.0/src/tekore/_sender/extending.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/src/tekore/model.py` & `tekore-5.0.0/src/tekore/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     Item,
     LocalAlbum,
     LocalArtist,
     LocalItem,
     LocalPlaylistTrack,
     LocalTrack,
     Model,
-    ModelList,
     Narrator,
     OffsetPaging,
     Paging,
     PlayerErrorReason,
     PlayHistory,
     PlayHistoryCursor,
     PlayHistoryPaging,
@@ -76,15 +75,14 @@
     SavedEpisodePaging,
     SavedShow,
     SavedShowPaging,
     SavedTrack,
     SavedTrackPaging,
     Section,
     Segment,
-    Serialisable,
     Show,
     SimpleAlbum,
     SimpleAlbumPaging,
     SimpleArtist,
     SimpleAudiobook,
     SimpleAudiobookPaging,
     SimpleChapter,
@@ -95,15 +93,14 @@
     SimplePlaylistPaging,
     SimpleShow,
     SimpleShowPaging,
     SimpleTrack,
     SimpleTrackPaging,
     StrEnum,
     TimeInterval,
-    Timestamp,
     Track,
     TrackLink,
     Tracks,
     UnknownModelAttributeWarning,
     User,
 )
 
@@ -206,15 +203,12 @@
     FullTrackPaging,
     ExplicitContent,
     UnknownModelAttributeWarning,
     User,
     PrivateUser,
     PublicUser,
     Model,
-    ModelList,
-    Serialisable,
     StrEnum,
-    Timestamp,
 ]
 
 for _cls in _classes:
     _cls.__module__ = "tekore.model"
```

### Comparing `tekore-4.6.1/src/tekore.egg-info/PKG-INFO` & `tekore-5.0.0/src/tekore.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tekore
-Version: 4.6.1
+Version: 5.0.0
 Summary: Client for the Spotify Web API
 Author-email: Felix Hildén <felix.hilden@gmail.com>
 Maintainer-email: Felix Hildén <felix.hilden@gmail.com>
 License: MIT License
         
         Copyright (c) 2019-2023 Felix Hildén
         
@@ -33,21 +33,20 @@
 Project-URL: Documentation, https://tekore.rtfd.org
 Keywords: spotify,web,api,client
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Sound/Audio
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 |logo|
 
 |python| |downloads|
```

### Comparing `tekore-4.6.1/src/tekore.egg-info/SOURCES.txt` & `tekore-5.0.0/src/tekore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/tests/auth/expiring.py` & `tekore-5.0.0/tests/auth/expiring.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/tests/auth/refreshing.py` & `tekore-5.0.0/tests/auth/refreshing.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/tests/auth/scope.py` & `tekore-5.0.0/tests/auth/scope.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/tests/auth/util.py` & `tekore-5.0.0/tests/auth/util.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/tests/client/_resources.py` & `tekore-5.0.0/tests/client/_resources.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/tests/client/album.py` & `tekore-5.0.0/tests/client/album.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/tests/client/artist.py` & `tekore-5.0.0/tests/client/artist.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/tests/client/audiobook.py` & `tekore-5.0.0/tests/client/audiobook.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/tests/client/base.py` & `tekore-5.0.0/tests/client/base.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/tests/client/browse.py` & `tekore-5.0.0/tests/client/browse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 
 import tekore as tk
 
 from ._resources import artist_ids, category_id, genres, track_id
 
 
-class TestSpotifyArtist:
+class TestSpotifyBrowse:
     def test_featured_playlists_with_country(self, app_client):
         msg, playlists = app_client.featured_playlists(country="US")
         assert playlists.total > 0
 
     def test_featured_playlists_no_country(self, app_client):
         msg, playlists = app_client.featured_playlists()
         assert playlists.total > 0
```

### Comparing `tekore-4.6.1/tests/client/chapter.py` & `tekore-5.0.0/tests/client/chapter.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/tests/client/episode.py` & `tekore-5.0.0/tests/client/episode.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/tests/client/follow.py` & `tekore-5.0.0/tests/client/follow.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/tests/client/full.py` & `tekore-5.0.0/tests/client/full.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from inspect import getmembers, ismethod
 from unittest.mock import MagicMock
 
 import pytest
 
 from tekore import BadRequest, Scope, Spotify, Unauthorised
 from tekore._client.chunked import chunked, return_last, return_none
-from tekore.model import ModelList
 
 
 @pytest.fixture()
 def client():
     return Spotify("token")
 
 
@@ -292,20 +291,14 @@
     @pytest.mark.asyncio
     async def test_async_too_many_chunked_succeeds(self, app_token, track_ids):
         client = Spotify(app_token, chunked_on=True, asynchronous=True)
         tracks = await client.tracks(track_ids)
         assert len(track_ids) == len(tracks)
         await client.close()
 
-    def test_returns_model_list(self, app_token, track_ids):
-        client = Spotify(app_token, chunked_on=True)
-        tracks = client.tracks(track_ids)
-        assert isinstance(tracks, ModelList)
-        client.close()
-
     def test_chunked_context_enables(self):
         client = Spotify()
         with client.chunked(True):
             assert client.chunked_on is True
         client.close()
 
     def test_chunked_context_disables(self):
```

### Comparing `tekore-4.6.1/tests/client/library.py` & `tekore-5.0.0/tests/client/library.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/tests/client/paging.py` & `tekore-5.0.0/tests/client/paging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import pytest
 
-from tekore import BadRequest
-
 from ._resources import album_id
 
 
 @pytest.fixture(scope="class")
 def tracks(data_client):
     return data_client.album_tracks(album_id, limit=1)
```

### Comparing `tekore-4.6.1/tests/client/player.py` & `tekore-5.0.0/tests/client/player.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/tests/client/playlist.py` & `tekore-5.0.0/tests/client/playlist.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/tests/client/search.py` & `tekore-5.0.0/tests/client/search.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/tests/client/show.py` & `tekore-5.0.0/tests/client/show.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/tests/client/track.py` & `tekore-5.0.0/tests/client/track.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/tests/config.py` & `tekore-5.0.0/tests/config.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/tests/conftest.py` & `tekore-5.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/tests/convert.py` & `tekore-5.0.0/tests/convert.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/tests/sender/caching.py` & `tekore-5.0.0/tests/sender/caching.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/tests/sender/client.py` & `tekore-5.0.0/tests/sender/client.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/tests/sender/retrying.py` & `tekore-5.0.0/tests/sender/retrying.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.1/tox.ini` & `tekore-5.0.0/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -25,127 +25,129 @@
 00000180: 696e 2c6d 6163 2c77 696e 7d0d 0a0d 0a5b  in,mac,win}....[
 00000190: 666c 616b 6538 5d0d 0a6d 6178 2d6c 696e  flake8]..max-lin
 000001a0: 652d 6c65 6e67 7468 203d 2038 300d 0a73  e-length = 80..s
 000001b0: 656c 6563 7420 3d20 432c 452c 462c 572c  elect = C,E,F,W,
 000001c0: 422c 4239 0d0a 6967 6e6f 7265 203d 2042  B,B9..ignore = B
 000001d0: 3330 352c 4239 3032 2c42 3930 352c 4532  305,B902,B905,E2
 000001e0: 3033 2c45 3430 322c 4535 3031 2c45 3732  03,E402,E501,E72
-000001f0: 322c 4634 3031 0d0a 0d0a 5b64 6f63 385d  2,F401....[doc8]
-00000200: 0d0a 6967 6e6f 7265 203d 2044 3030 322c  ..ignore = D002,
-00000210: 4430 3034 0d0a 6d61 782d 6c69 6e65 2d6c  D004..max-line-l
-00000220: 656e 6774 6820 3d20 3830 0d0a 0d0a 5b74  ength = 80....[t
-00000230: 6573 7465 6e76 5d0d 0a64 6573 6372 6970  estenv]..descrip
-00000240: 7469 6f6e 203d 2052 756e 2074 6573 7420  tion = Run test 
-00000250: 7375 6974 6520 7769 7468 2063 6f64 6520  suite with code 
-00000260: 636f 7665 7261 6765 0d0a 706c 6174 666f  coverage..platfo
-00000270: 726d 203d 0d0a 2020 2020 6c69 6e3a 206c  rm =..    lin: l
-00000280: 696e 7578 0d0a 2020 2020 6d61 633a 2064  inux..    mac: d
-00000290: 6172 7769 6e0d 0a20 2020 2077 696e 3a20  arwin..    win: 
-000002a0: 7769 6e33 320d 0a61 6c6c 6f77 6c69 7374  win32..allowlist
-000002b0: 5f65 7874 6572 6e61 6c73 203d 2063 6f76  _externals = cov
-000002c0: 6572 6167 650d 0a70 6173 7365 6e76 203d  erage..passenv =
-000002d0: 2053 504f 5449 4659 2a2c 5445 4b4f 5245   SPOTIFY*,TEKORE
-000002e0: 2a0d 0a63 6f6d 6d61 6e64 7320 3d20 636f  *..commands = co
-000002f0: 7665 7261 6765 2072 756e 0d0a 2020 2020  verage run..    
-00000300: 2020 2020 2020 2063 6f76 6572 6167 6520         coverage 
-00000310: 7265 706f 7274 0d0a 0d0a 5b74 6573 7465  report....[teste
-00000320: 6e76 3a63 6f76 6572 6167 655d 0d0a 3b20  nv:coverage]..; 
-00000330: 496e 6865 7269 7420 6576 6572 7974 6869  Inherit everythi
-00000340: 6e67 2066 726f 6d20 7465 7374 656e 760d  ng from testenv.
-00000350: 0a0d 0a5b 7465 7374 656e 763a 646f 6338  ...[testenv:doc8
-00000360: 5d0d 0a64 6573 6372 6970 7469 6f6e 203d  ]..description =
-00000370: 2043 6865 636b 2064 6f63 756d 656e 7461   Check documenta
-00000380: 7469 6f6e 202e 7273 7420 6669 6c65 730d  tion .rst files.
-00000390: 0a61 6c6c 6f77 6c69 7374 5f65 7874 6572  .allowlist_exter
-000003a0: 6e61 6c73 203d 2064 6f63 380d 0a63 6f6d  nals = doc8..com
-000003b0: 6d61 6e64 7320 3d20 646f 6338 2064 6f63  mands = doc8 doc
-000003c0: 732f 7372 630d 0a0d 0a5b 7465 7374 656e  s/src....[testen
-000003d0: 763a 666c 616b 6538 5d0d 0a64 6573 6372  v:flake8]..descr
-000003e0: 6970 7469 6f6e 203d 2043 6865 636b 2063  iption = Check c
-000003f0: 6f64 6520 7374 796c 650d 0a61 6c6c 6f77  ode style..allow
-00000400: 6c69 7374 5f65 7874 6572 6e61 6c73 203d  list_externals =
-00000410: 2066 6c61 6b65 380d 0a63 6f6d 6d61 6e64   flake8..command
-00000420: 7320 3d20 666c 616b 6538 2073 7263 2074  s = flake8 src t
-00000430: 6573 7473 0d0a 0d0a 5b74 6573 7465 6e76  ests....[testenv
-00000440: 3a70 7964 6f63 7374 796c 655d 0d0a 6465  :pydocstyle]..de
-00000450: 7363 7269 7074 696f 6e20 3d20 4368 6563  scription = Chec
-00000460: 6b20 646f 6375 6d65 6e74 6174 696f 6e20  k documentation 
-00000470: 7374 7269 6e67 2073 7479 6c65 0d0a 616c  string style..al
-00000480: 6c6f 776c 6973 745f 6578 7465 726e 616c  lowlist_external
-00000490: 7320 3d20 7079 646f 6373 7479 6c65 0d0a  s = pydocstyle..
-000004a0: 636f 6d6d 616e 6473 203d 2070 7964 6f63  commands = pydoc
-000004b0: 7374 796c 6520 7372 630d 0a0d 0a5b 7465  style src....[te
-000004c0: 7374 656e 763a 646f 6373 5d0d 0a64 6573  stenv:docs]..des
-000004d0: 6372 6970 7469 6f6e 203d 2042 7569 6c64  cription = Build
-000004e0: 2053 7068 696e 7820 646f 6375 6d65 6e74   Sphinx document
-000004f0: 6174 696f 6e0d 0a61 6c6c 6f77 6c69 7374  ation..allowlist
-00000500: 5f65 7874 6572 6e61 6c73 203d 2073 7068  _externals = sph
-00000510: 696e 782d 6275 696c 640d 0a63 6861 6e67  inx-build..chang
-00000520: 655f 6469 7220 3d20 646f 6373 0d0a 636f  e_dir = docs..co
-00000530: 6d6d 616e 6473 203d 2073 7068 696e 782d  mmands = sphinx-
-00000540: 6275 696c 6420 2d4d 2068 746d 6c20 7372  build -M html sr
-00000550: 6320 6275 696c 640d 0a0d 0a5b 7465 7374  c build....[test
-00000560: 656e 763a 626c 6163 6b2d 6368 6563 6b5d  env:black-check]
-00000570: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
-00000580: 4368 6563 6b20 636f 6465 2066 6f72 6d61  Check code forma
-00000590: 7474 696e 670d 0a61 6c6c 6f77 6c69 7374  tting..allowlist
-000005a0: 5f65 7874 6572 6e61 6c73 203d 2062 6c61  _externals = bla
-000005b0: 636b 0d0a 636f 6d6d 616e 6473 203d 2062  ck..commands = b
-000005c0: 6c61 636b 202e 202d 2d63 6865 636b 0d0a  lack . --check..
-000005d0: 0d0a 5b74 6573 7465 6e76 3a62 6c61 636b  ..[testenv:black
-000005e0: 2d66 6f72 6d61 745d 0d0a 6465 7363 7269  -format]..descri
-000005f0: 7074 696f 6e20 3d20 466f 726d 6174 2063  ption = Format c
-00000600: 6f64 650d 0a61 6c6c 6f77 6c69 7374 5f65  ode..allowlist_e
-00000610: 7874 6572 6e61 6c73 203d 2062 6c61 636b  xternals = black
-00000620: 0d0a 636f 6d6d 616e 6473 203d 2062 6c61  ..commands = bla
-00000630: 636b 202e 0d0a 0d0a 5b74 6573 7465 6e76  ck .....[testenv
-00000640: 3a69 736f 7274 2d63 6865 636b 5d0d 0a64  :isort-check]..d
-00000650: 6573 6372 6970 7469 6f6e 203d 2043 6865  escription = Che
-00000660: 636b 2069 6d70 6f72 7420 736f 7274 696e  ck import sortin
-00000670: 670d 0a61 6c6c 6f77 6c69 7374 5f65 7874  g..allowlist_ext
-00000680: 6572 6e61 6c73 203d 2069 736f 7274 0d0a  ernals = isort..
-00000690: 636f 6d6d 616e 6473 203d 2069 736f 7274  commands = isort
-000006a0: 202e 202d 2d63 6865 636b 2d6f 6e6c 790d   . --check-only.
-000006b0: 0a0d 0a5b 7465 7374 656e 763a 6973 6f72  ...[testenv:isor
-000006c0: 742d 666f 726d 6174 5d0d 0a64 6573 6372  t-format]..descr
-000006d0: 6970 7469 6f6e 203d 2046 6f72 6d61 7420  iption = Format 
-000006e0: 696d 706f 7274 730d 0a61 6c6c 6f77 6c69  imports..allowli
-000006f0: 7374 5f65 7874 6572 6e61 6c73 203d 2069  st_externals = i
-00000700: 736f 7274 0d0a 636f 6d6d 616e 6473 203d  sort..commands =
-00000710: 2069 736f 7274 202e 0d0a 0d0a 5b74 6573   isort .....[tes
-00000720: 7465 6e76 3a62 7569 6c64 2d7b 6c69 6e2c  tenv:build-{lin,
-00000730: 6d61 632c 7769 6e7d 5d0d 0a64 6573 6372  mac,win}]..descr
-00000740: 6970 7469 6f6e 203d 2042 7569 6c64 2061  iption = Build a
-00000750: 6e64 2063 6865 636b 2070 6163 6b61 6765  nd check package
-00000760: 0d0a 6465 7073 203d 202d 7220 7265 7175  ..deps = -r requ
-00000770: 6972 656d 656e 7473 2f62 7569 6c64 0d0a  irements/build..
-00000780: 616c 6c6f 776c 6973 745f 6578 7465 726e  allowlist_extern
-00000790: 616c 7320 3d20 726d 2c20 636d 640d 0a63  als = rm, cmd..c
-000007a0: 6f6d 6d61 6e64 7320 3d0d 0a20 2020 2070  ommands =..    p
-000007b0: 7974 686f 6e20 2d6d 2062 7569 6c64 0d0a  ython -m build..
-000007c0: 2020 2020 7477 696e 6520 6368 6563 6b20      twine check 
-000007d0: 2d2d 7374 7269 6374 2064 6973 742f 2a0d  --strict dist/*.
-000007e0: 0a63 6f6d 6d61 6e64 735f 706f 7374 203d  .commands_post =
-000007f0: 0d0a 2020 2020 6c69 6e2c 6d61 633a 2072  ..    lin,mac: r
-00000800: 6d20 2d72 2064 6973 740d 0a20 2020 2077  m -r dist..    w
-00000810: 696e 3a20 636d 6420 2f63 2072 6d64 6972  in: cmd /c rmdir
-00000820: 202f 7320 2f71 2064 6973 740d 0a0d 0a5b   /s /q dist....[
-00000830: 7465 7374 656e 763a 7075 626c 6973 682d  testenv:publish-
-00000840: 7b6c 696e 2c6d 6163 2c77 696e 7d5d 0d0a  {lin,mac,win}]..
-00000850: 6465 7363 7269 7074 696f 6e20 3d20 4275  description = Bu
-00000860: 696c 642c 2063 6865 636b 2061 6e64 2070  ild, check and p
-00000870: 7562 6c69 7368 2070 6163 6b61 6765 0d0a  ublish package..
-00000880: 6465 7073 203d 202d 7220 7265 7175 6972  deps = -r requir
-00000890: 656d 656e 7473 2f62 7569 6c64 0d0a 616c  ements/build..al
-000008a0: 6c6f 776c 6973 745f 6578 7465 726e 616c  lowlist_external
-000008b0: 7320 3d20 726d 2c20 636d 640d 0a63 6f6d  s = rm, cmd..com
-000008c0: 6d61 6e64 7320 3d0d 0a20 2020 2070 7974  mands =..    pyt
-000008d0: 686f 6e20 2d6d 2062 7569 6c64 0d0a 2020  hon -m build..  
-000008e0: 2020 7477 696e 6520 6368 6563 6b20 2d2d    twine check --
-000008f0: 7374 7269 6374 2064 6973 742f 2a0d 0a20  strict dist/*.. 
-00000900: 2020 2074 7769 6e65 2075 706c 6f61 6420     twine upload 
-00000910: 6469 7374 2f2a 0d0a 636f 6d6d 616e 6473  dist/*..commands
-00000920: 5f70 6f73 7420 3d0d 0a20 2020 206c 696e  _post =..    lin
-00000930: 2c6d 6163 3a20 726d 202d 7220 6469 7374  ,mac: rm -r dist
-00000940: 0d0a 2020 2020 7769 6e3a 2063 6d64 202f  ..    win: cmd /
-00000950: 6320 726d 6469 7220 2f73 202f 7120 6469  c rmdir /s /q di
-00000960: 7374 0d0a                                st..
+000001f0: 320d 0a70 6572 2d66 696c 652d 6967 6e6f  2..per-file-igno
+00000200: 7265 7320 3d20 0d0a 2020 2020 5f5f 696e  res = ..    __in
+00000210: 6974 5f5f 2e70 793a 2046 3430 310d 0a0d  it__.py: F401...
+00000220: 0a5b 646f 6338 5d0d 0a69 676e 6f72 6520  .[doc8]..ignore 
+00000230: 3d20 4430 3032 2c44 3030 340d 0a6d 6178  = D002,D004..max
+00000240: 2d6c 696e 652d 6c65 6e67 7468 203d 2038  -line-length = 8
+00000250: 300d 0a0d 0a5b 7465 7374 656e 765d 0d0a  0....[testenv]..
+00000260: 6465 7363 7269 7074 696f 6e20 3d20 5275  description = Ru
+00000270: 6e20 7465 7374 2073 7569 7465 2077 6974  n test suite wit
+00000280: 6820 636f 6465 2063 6f76 6572 6167 650d  h code coverage.
+00000290: 0a70 6c61 7466 6f72 6d20 3d0d 0a20 2020  .platform =..   
+000002a0: 206c 696e 3a20 6c69 6e75 780d 0a20 2020   lin: linux..   
+000002b0: 206d 6163 3a20 6461 7277 696e 0d0a 2020   mac: darwin..  
+000002c0: 2020 7769 6e3a 2077 696e 3332 0d0a 616c    win: win32..al
+000002d0: 6c6f 776c 6973 745f 6578 7465 726e 616c  lowlist_external
+000002e0: 7320 3d20 636f 7665 7261 6765 0d0a 7061  s = coverage..pa
+000002f0: 7373 656e 7620 3d20 5350 4f54 4946 592a  ssenv = SPOTIFY*
+00000300: 2c54 454b 4f52 452a 0d0a 636f 6d6d 616e  ,TEKORE*..comman
+00000310: 6473 203d 2063 6f76 6572 6167 6520 7275  ds = coverage ru
+00000320: 6e0d 0a20 2020 2020 2020 2020 2020 636f  n..           co
+00000330: 7665 7261 6765 2072 6570 6f72 740d 0a0d  verage report...
+00000340: 0a5b 7465 7374 656e 763a 636f 7665 7261  .[testenv:covera
+00000350: 6765 5d0d 0a3b 2049 6e68 6572 6974 2065  ge]..; Inherit e
+00000360: 7665 7279 7468 696e 6720 6672 6f6d 2074  verything from t
+00000370: 6573 7465 6e76 0d0a 0d0a 5b74 6573 7465  estenv....[teste
+00000380: 6e76 3a64 6f63 385d 0d0a 6465 7363 7269  nv:doc8]..descri
+00000390: 7074 696f 6e20 3d20 4368 6563 6b20 646f  ption = Check do
+000003a0: 6375 6d65 6e74 6174 696f 6e20 2e72 7374  cumentation .rst
+000003b0: 2066 696c 6573 0d0a 616c 6c6f 776c 6973   files..allowlis
+000003c0: 745f 6578 7465 726e 616c 7320 3d20 646f  t_externals = do
+000003d0: 6338 0d0a 636f 6d6d 616e 6473 203d 2064  c8..commands = d
+000003e0: 6f63 3820 646f 6373 2f73 7263 0d0a 0d0a  oc8 docs/src....
+000003f0: 5b74 6573 7465 6e76 3a66 6c61 6b65 385d  [testenv:flake8]
+00000400: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
+00000410: 4368 6563 6b20 636f 6465 2073 7479 6c65  Check code style
+00000420: 0d0a 616c 6c6f 776c 6973 745f 6578 7465  ..allowlist_exte
+00000430: 726e 616c 7320 3d20 666c 616b 6538 0d0a  rnals = flake8..
+00000440: 636f 6d6d 616e 6473 203d 2066 6c61 6b65  commands = flake
+00000450: 3820 7372 6320 7465 7374 730d 0a0d 0a5b  8 src tests....[
+00000460: 7465 7374 656e 763a 7079 646f 6373 7479  testenv:pydocsty
+00000470: 6c65 5d0d 0a64 6573 6372 6970 7469 6f6e  le]..description
+00000480: 203d 2043 6865 636b 2064 6f63 756d 656e   = Check documen
+00000490: 7461 7469 6f6e 2073 7472 696e 6720 7374  tation string st
+000004a0: 796c 650d 0a61 6c6c 6f77 6c69 7374 5f65  yle..allowlist_e
+000004b0: 7874 6572 6e61 6c73 203d 2070 7964 6f63  xternals = pydoc
+000004c0: 7374 796c 650d 0a63 6f6d 6d61 6e64 7320  style..commands 
+000004d0: 3d20 7079 646f 6373 7479 6c65 2073 7263  = pydocstyle src
+000004e0: 0d0a 0d0a 5b74 6573 7465 6e76 3a64 6f63  ....[testenv:doc
+000004f0: 735d 0d0a 6465 7363 7269 7074 696f 6e20  s]..description 
+00000500: 3d20 4275 696c 6420 5370 6869 6e78 2064  = Build Sphinx d
+00000510: 6f63 756d 656e 7461 7469 6f6e 0d0a 616c  ocumentation..al
+00000520: 6c6f 776c 6973 745f 6578 7465 726e 616c  lowlist_external
+00000530: 7320 3d20 7370 6869 6e78 2d62 7569 6c64  s = sphinx-build
+00000540: 0d0a 6368 616e 6765 5f64 6972 203d 2064  ..change_dir = d
+00000550: 6f63 730d 0a63 6f6d 6d61 6e64 7320 3d20  ocs..commands = 
+00000560: 7370 6869 6e78 2d62 7569 6c64 202d 4d20  sphinx-build -M 
+00000570: 6874 6d6c 2073 7263 2062 7569 6c64 0d0a  html src build..
+00000580: 0d0a 5b74 6573 7465 6e76 3a62 6c61 636b  ..[testenv:black
+00000590: 2d63 6865 636b 5d0d 0a64 6573 6372 6970  -check]..descrip
+000005a0: 7469 6f6e 203d 2043 6865 636b 2063 6f64  tion = Check cod
+000005b0: 6520 666f 726d 6174 7469 6e67 0d0a 616c  e formatting..al
+000005c0: 6c6f 776c 6973 745f 6578 7465 726e 616c  lowlist_external
+000005d0: 7320 3d20 626c 6163 6b0d 0a63 6f6d 6d61  s = black..comma
+000005e0: 6e64 7320 3d20 626c 6163 6b20 2e20 2d2d  nds = black . --
+000005f0: 6368 6563 6b0d 0a0d 0a5b 7465 7374 656e  check....[testen
+00000600: 763a 626c 6163 6b2d 666f 726d 6174 5d0d  v:black-format].
+00000610: 0a64 6573 6372 6970 7469 6f6e 203d 2046  .description = F
+00000620: 6f72 6d61 7420 636f 6465 0d0a 616c 6c6f  ormat code..allo
+00000630: 776c 6973 745f 6578 7465 726e 616c 7320  wlist_externals 
+00000640: 3d20 626c 6163 6b0d 0a63 6f6d 6d61 6e64  = black..command
+00000650: 7320 3d20 626c 6163 6b20 2e0d 0a0d 0a5b  s = black .....[
+00000660: 7465 7374 656e 763a 6973 6f72 742d 6368  testenv:isort-ch
+00000670: 6563 6b5d 0d0a 6465 7363 7269 7074 696f  eck]..descriptio
+00000680: 6e20 3d20 4368 6563 6b20 696d 706f 7274  n = Check import
+00000690: 2073 6f72 7469 6e67 0d0a 616c 6c6f 776c   sorting..allowl
+000006a0: 6973 745f 6578 7465 726e 616c 7320 3d20  ist_externals = 
+000006b0: 6973 6f72 740d 0a63 6f6d 6d61 6e64 7320  isort..commands 
+000006c0: 3d20 6973 6f72 7420 2e20 2d2d 6368 6563  = isort . --chec
+000006d0: 6b2d 6f6e 6c79 0d0a 0d0a 5b74 6573 7465  k-only....[teste
+000006e0: 6e76 3a69 736f 7274 2d66 6f72 6d61 745d  nv:isort-format]
+000006f0: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
+00000700: 466f 726d 6174 2069 6d70 6f72 7473 0d0a  Format imports..
+00000710: 616c 6c6f 776c 6973 745f 6578 7465 726e  allowlist_extern
+00000720: 616c 7320 3d20 6973 6f72 740d 0a63 6f6d  als = isort..com
+00000730: 6d61 6e64 7320 3d20 6973 6f72 7420 2e0d  mands = isort ..
+00000740: 0a0d 0a5b 7465 7374 656e 763a 6275 696c  ...[testenv:buil
+00000750: 642d 7b6c 696e 2c6d 6163 2c77 696e 7d5d  d-{lin,mac,win}]
+00000760: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
+00000770: 4275 696c 6420 616e 6420 6368 6563 6b20  Build and check 
+00000780: 7061 636b 6167 650d 0a64 6570 7320 3d20  package..deps = 
+00000790: 2d72 2072 6571 7569 7265 6d65 6e74 732f  -r requirements/
+000007a0: 6275 696c 640d 0a61 6c6c 6f77 6c69 7374  build..allowlist
+000007b0: 5f65 7874 6572 6e61 6c73 203d 2072 6d2c  _externals = rm,
+000007c0: 2063 6d64 0d0a 636f 6d6d 616e 6473 203d   cmd..commands =
+000007d0: 0d0a 2020 2020 7079 7468 6f6e 202d 6d20  ..    python -m 
+000007e0: 6275 696c 640d 0a20 2020 2074 7769 6e65  build..    twine
+000007f0: 2063 6865 636b 202d 2d73 7472 6963 7420   check --strict 
+00000800: 6469 7374 2f2a 0d0a 636f 6d6d 616e 6473  dist/*..commands
+00000810: 5f70 6f73 7420 3d0d 0a20 2020 206c 696e  _post =..    lin
+00000820: 2c6d 6163 3a20 726d 202d 7220 6469 7374  ,mac: rm -r dist
+00000830: 0d0a 2020 2020 7769 6e3a 2063 6d64 202f  ..    win: cmd /
+00000840: 6320 726d 6469 7220 2f73 202f 7120 6469  c rmdir /s /q di
+00000850: 7374 0d0a 0d0a 5b74 6573 7465 6e76 3a70  st....[testenv:p
+00000860: 7562 6c69 7368 2d7b 6c69 6e2c 6d61 632c  ublish-{lin,mac,
+00000870: 7769 6e7d 5d0d 0a64 6573 6372 6970 7469  win}]..descripti
+00000880: 6f6e 203d 2042 7569 6c64 2c20 6368 6563  on = Build, chec
+00000890: 6b20 616e 6420 7075 626c 6973 6820 7061  k and publish pa
+000008a0: 636b 6167 650d 0a64 6570 7320 3d20 2d72  ckage..deps = -r
+000008b0: 2072 6571 7569 7265 6d65 6e74 732f 6275   requirements/bu
+000008c0: 696c 640d 0a61 6c6c 6f77 6c69 7374 5f65  ild..allowlist_e
+000008d0: 7874 6572 6e61 6c73 203d 2072 6d2c 2063  xternals = rm, c
+000008e0: 6d64 0d0a 636f 6d6d 616e 6473 203d 0d0a  md..commands =..
+000008f0: 2020 2020 7079 7468 6f6e 202d 6d20 6275      python -m bu
+00000900: 696c 640d 0a20 2020 2074 7769 6e65 2063  ild..    twine c
+00000910: 6865 636b 202d 2d73 7472 6963 7420 6469  heck --strict di
+00000920: 7374 2f2a 0d0a 2020 2020 7477 696e 6520  st/*..    twine 
+00000930: 7570 6c6f 6164 2064 6973 742f 2a0d 0a63  upload dist/*..c
+00000940: 6f6d 6d61 6e64 735f 706f 7374 203d 0d0a  ommands_post =..
+00000950: 2020 2020 6c69 6e2c 6d61 633a 2072 6d20      lin,mac: rm 
+00000960: 2d72 2064 6973 740d 0a20 2020 2077 696e  -r dist..    win
+00000970: 3a20 636d 6420 2f63 2072 6d64 6972 202f  : cmd /c rmdir /
+00000980: 7320 2f71 2064 6973 740d 0a              s /q dist..
```

