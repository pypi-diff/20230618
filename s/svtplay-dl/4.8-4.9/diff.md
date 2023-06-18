# Comparing `tmp/svtplay-dl-4.8.tar.gz` & `tmp/svtplay-dl-4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svtplay-dl-4.8.tar", last modified: Wed Oct 27 12:56:48 2021, max compression
+gzip compressed data, was "svtplay-dl-4.9.tar", last modified: Wed Nov  3 21:25:59 2021, max compression
```

## Comparing `svtplay-dl-4.8.tar` & `svtplay-dl-4.9.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 12:56:48.660708 svtplay-dl-4.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2021-10-27 12:56:22.000000 svtplay-dl-4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       94 2021-10-27 12:56:22.000000 svtplay-dl-4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5405 2021-10-27 12:56:48.660708 svtplay-dl-4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4479 2021-10-27 12:56:22.000000 svtplay-dl-4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 12:56:48.648708 svtplay-dl-4.8/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)      180 2021-10-27 12:56:22.000000 svtplay-dl-4.8/bin/svtplay-dl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 12:56:48.648708 svtplay-dl-4.8/lib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 12:56:48.660708 svtplay-dl-4.8/lib/svtplay_dl/
--rw-r--r--   0 runner    (1001) docker     (121)     2259 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      381 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      495 2021-10-27 12:56:48.660708 svtplay-dl-4.8/lib/svtplay_dl/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)      991 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/error.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 12:56:48.652708 svtplay-dl-4.8/lib/svtplay_dl/fetcher/
--rw-r--r--   0 runner    (1001) docker     (121)     1208 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/fetcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15830 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/fetcher/dash.py
--rw-r--r--   0 runner    (1001) docker     (121)    21348 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/fetcher/hls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1321 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/fetcher/http.py
--rw-r--r--   0 runner    (1001) docker     (121)      183 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/log.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 12:56:48.652708 svtplay-dl-4.8/lib/svtplay_dl/postprocess/
--rw-r--r--   0 runner    (1001) docker     (121)     8746 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/postprocess/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 12:56:48.656708 svtplay-dl-4.8/lib/svtplay_dl/service/
--rw-r--r--   0 runner    (1001) docker     (121)     7538 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2287 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/aftonbladet.py
--rw-r--r--   0 runner    (1001) docker     (121)     1343 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/atg.py
--rw-r--r--   0 runner    (1001) docker     (121)     3600 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/barnkanalen.py
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/bigbrother.py
--rw-r--r--   0 runner    (1001) docker     (121)     7073 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/cmore.py
--rw-r--r--   0 runner    (1001) docker     (121)     3990 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/disney.py
--rw-r--r--   0 runner    (1001) docker     (121)    11541 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/dplay.py
--rw-r--r--   0 runner    (1001) docker     (121)     4065 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/dr.py
--rw-r--r--   0 runner    (1001) docker     (121)      576 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/efn.py
--rw-r--r--   0 runner    (1001) docker     (121)     5081 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/eurosport.py
--rw-r--r--   0 runner    (1001) docker     (121)      840 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/expressen.py
--rw-r--r--   0 runner    (1001) docker     (121)     1420 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/facebook.py
--rw-r--r--   0 runner    (1001) docker     (121)      657 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/filmarkivet.py
--rw-r--r--   0 runner    (1001) docker     (121)     1265 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/flowonline.py
--rw-r--r--   0 runner    (1001) docker     (121)     3047 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/koket.py
--rw-r--r--   0 runner    (1001) docker     (121)     1980 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/lemonwhale.py
--rw-r--r--   0 runner    (1001) docker     (121)     6234 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/mtvnn.py
--rw-r--r--   0 runner    (1001) docker     (121)     1220 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/mtvservices.py
--rw-r--r--   0 runner    (1001) docker     (121)     2060 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/nhl.py
--rw-r--r--   0 runner    (1001) docker     (121)     2249 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/npo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1836 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/nrk.py
--rw-r--r--   0 runner    (1001) docker     (121)     5191 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/oppetarkiv.py
--rw-r--r--   0 runner    (1001) docker     (121)     5069 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/picsearch.py
--rw-r--r--   0 runner    (1001) docker     (121)     1546 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/pokemon.py
--rw-r--r--   0 runner    (1001) docker     (121)      737 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/radioplay.py
--rw-r--r--   0 runner    (1001) docker     (121)      606 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/raw.py
--rw-r--r--   0 runner    (1001) docker     (121)      961 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/riksdagen.py
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/ruv.py
--rw-r--r--   0 runner    (1001) docker     (121)     2482 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/services.py
--rw-r--r--   0 runner    (1001) docker     (121)     3363 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/solidtango.py
--rw-r--r--   0 runner    (1001) docker     (121)     2929 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/sportlib.py
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/sr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1574 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/svt.py
--rw-r--r--   0 runner    (1001) docker     (121)    14440 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/svtplay.py
--rw-r--r--   0 runner    (1001) docker     (121)    10769 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/tv4play.py
--rw-r--r--   0 runner    (1001) docker     (121)     5351 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/twitch.py
--rw-r--r--   0 runner    (1001) docker     (121)     4442 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/urplay.py
--rw-r--r--   0 runner    (1001) docker     (121)     1393 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/vg.py
--rw-r--r--   0 runner    (1001) docker     (121)     8728 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/viaplay.py
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/viasatsport.py
--rw-r--r--   0 runner    (1001) docker     (121)     1817 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/vimeo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1692 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/service/youplay.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 12:56:48.656708 svtplay-dl-4.8/lib/svtplay_dl/subtitle/
--rw-r--r--   0 runner    (1001) docker     (121)    15859 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/subtitle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 12:56:48.660708 svtplay-dl-4.8/lib/svtplay_dl/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8529 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/utils/getmedia.py
--rw-r--r--   0 runner    (1001) docker     (121)     2931 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/utils/http.py
--rw-r--r--   0 runner    (1001) docker     (121)     3110 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/utils/nfo.py
--rw-r--r--   0 runner    (1001) docker     (121)     7082 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/utils/output.py
--rw-r--r--   0 runner    (1001) docker     (121)    18824 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/utils/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)      411 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/utils/proc.py
--rw-r--r--   0 runner    (1001) docker     (121)     7406 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/utils/stream.py
--rw-r--r--   0 runner    (1001) docker     (121)     2563 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/utils/terminal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1601 2021-10-27 12:56:22.000000 svtplay-dl-4.8/lib/svtplay_dl/utils/text.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 12:56:48.652708 svtplay-dl-4.8/lib/svtplay_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5405 2021-10-27 12:56:48.000000 svtplay-dl-4.8/lib/svtplay_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2371 2021-10-27 12:56:48.000000 svtplay-dl-4.8/lib/svtplay_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-27 12:56:48.000000 svtplay-dl-4.8/lib/svtplay_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2021-10-27 12:56:48.000000 svtplay-dl-4.8/lib/svtplay_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-10-27 12:56:48.000000 svtplay-dl-4.8/lib/svtplay_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-10-27 12:56:22.000000 svtplay-dl-4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      259 2021-10-27 12:56:48.660708 svtplay-dl-4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2560 2021-10-27 12:56:22.000000 svtplay-dl-4.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    67662 2021-10-27 12:56:22.000000 svtplay-dl-4.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-03 21:25:59.907813 svtplay-dl-4.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1098 2021-11-03 21:25:06.000000 svtplay-dl-4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2021-11-03 21:25:06.000000 svtplay-dl-4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5405 2021-11-03 21:25:59.907813 svtplay-dl-4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4479 2021-11-03 21:25:06.000000 svtplay-dl-4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-03 21:25:59.895813 svtplay-dl-4.9/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      180 2021-11-03 21:25:06.000000 svtplay-dl-4.9/bin/svtplay-dl
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-03 21:25:59.895813 svtplay-dl-4.9/lib/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-03 21:25:59.907813 svtplay-dl-4.9/lib/svtplay_dl/
+-rw-r--r--   0 runner    (1001) docker     (121)     2259 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      381 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      495 2021-11-03 21:25:59.907813 svtplay-dl-4.9/lib/svtplay_dl/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      991 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/error.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-03 21:25:59.899813 svtplay-dl-4.9/lib/svtplay_dl/fetcher/
+-rw-r--r--   0 runner    (1001) docker     (121)     1208 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/fetcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15830 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/fetcher/dash.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21095 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/fetcher/hls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1321 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/fetcher/http.py
+-rw-r--r--   0 runner    (1001) docker     (121)      183 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/log.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-03 21:25:59.899813 svtplay-dl-4.9/lib/svtplay_dl/postprocess/
+-rw-r--r--   0 runner    (1001) docker     (121)     8754 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/postprocess/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-03 21:25:59.907813 svtplay-dl-4.9/lib/svtplay_dl/service/
+-rw-r--r--   0 runner    (1001) docker     (121)     7538 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2287 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/aftonbladet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1343 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/atg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3600 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/barnkanalen.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/bigbrother.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7073 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/cmore.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3990 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/disney.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11541 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/dplay.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4065 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/dr.py
+-rw-r--r--   0 runner    (1001) docker     (121)      576 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/efn.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5081 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/eurosport.py
+-rw-r--r--   0 runner    (1001) docker     (121)      840 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/expressen.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1420 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/facebook.py
+-rw-r--r--   0 runner    (1001) docker     (121)      657 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/filmarkivet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1265 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/flowonline.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3047 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/koket.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1980 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/lemonwhale.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6234 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/mtvnn.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1220 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/mtvservices.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2060 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/nhl.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2249 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/npo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1836 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/nrk.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5191 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/oppetarkiv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5069 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/picsearch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1546 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/pokemon.py
+-rw-r--r--   0 runner    (1001) docker     (121)      737 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/radioplay.py
+-rw-r--r--   0 runner    (1001) docker     (121)      606 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/raw.py
+-rw-r--r--   0 runner    (1001) docker     (121)      961 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/riksdagen.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/ruv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2482 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/services.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3363 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/solidtango.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2929 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/sportlib.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1061 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/sr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1574 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/svt.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14534 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/svtplay.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10769 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/tv4play.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5351 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/twitch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4600 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/urplay.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1393 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/vg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8728 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/viaplay.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1065 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/viasatsport.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1817 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/vimeo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1692 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/service/youplay.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-03 21:25:59.907813 svtplay-dl-4.9/lib/svtplay_dl/subtitle/
+-rw-r--r--   0 runner    (1001) docker     (121)    15859 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/subtitle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-03 21:25:59.907813 svtplay-dl-4.9/lib/svtplay_dl/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8529 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/utils/getmedia.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2931 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/utils/http.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3110 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/utils/nfo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7254 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/utils/output.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18824 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/utils/parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/utils/proc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7406 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/utils/stream.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2563 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/utils/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1601 2021-11-03 21:25:06.000000 svtplay-dl-4.9/lib/svtplay_dl/utils/text.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-03 21:25:59.899813 svtplay-dl-4.9/lib/svtplay_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5405 2021-11-03 21:25:59.000000 svtplay-dl-4.9/lib/svtplay_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2371 2021-11-03 21:25:59.000000 svtplay-dl-4.9/lib/svtplay_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-03 21:25:59.000000 svtplay-dl-4.9/lib/svtplay_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2021-11-03 21:25:59.000000 svtplay-dl-4.9/lib/svtplay_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2021-11-03 21:25:59.000000 svtplay-dl-4.9/lib/svtplay_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2021-11-03 21:25:06.000000 svtplay-dl-4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      259 2021-11-03 21:25:59.907813 svtplay-dl-4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2560 2021-11-03 21:25:06.000000 svtplay-dl-4.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    67662 2021-11-03 21:25:06.000000 svtplay-dl-4.9/versioneer.py
```

### Comparing `svtplay-dl-4.8/LICENSE` & `svtplay-dl-4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/PKG-INFO` & `svtplay-dl-4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svtplay-dl
-Version: 4.8
+Version: 4.9
 Summary: Command-line program to download videos from various video on demand sites
 Home-page: https://svtplay-dl.se
 Author: Johan Andersson
 Author-email: j@i19.se
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `svtplay-dl-4.8/README.md` & `svtplay-dl-4.9/README.md`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/__init__.py` & `svtplay-dl-4.9/lib/svtplay_dl/__init__.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/error.py` & `svtplay-dl-4.9/lib/svtplay_dl/error.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/fetcher/__init__.py` & `svtplay-dl-4.9/lib/svtplay_dl/fetcher/__init__.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/fetcher/dash.py` & `svtplay-dl-4.9/lib/svtplay_dl/fetcher/dash.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/fetcher/hls.py` & `svtplay-dl-4.9/lib/svtplay_dl/fetcher/hls.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,19 +232,14 @@
         if audio:
             self.output["ext"] = "audio.ts"
         else:
             self.output["ext"] = "ts"
         filename = formatname(self.output, self.config)
         file_d = open(filename, "wb")
 
-        if "EXT-X-MAP" in m3u8.media_segment[0]:
-            entry = {"URI": get_full_url(m3u8.media_segment[0]["EXT-X-MAP"]["URI"], url), "EXTINF": {"duration": 0}}
-            if "EXT-X-KEY" in m3u8.media_segment[0]:
-                entry["EXT-X-KEY"] = {"URI": m3u8.media_segment[0]["EXT-X-KEY"]["URI"]}
-            m3u8.media_segment.insert(0, entry)
         hls_time_stamp = self.kwargs.pop("hls_time_stamp", False)
         decryptor = None
         size_media = len(m3u8.media_segment)
         eta = ETA(size_media)
         total_duration = 0
         duration = 0
         max_duration = 0
@@ -426,14 +421,15 @@
                     elif tag == "EXT-X-KEY":
                         self.encrypted = True
                         info = _get_tuple_attribute(attr)
 
                     # 4.3.2.5.  EXT-X-MAP
                     elif tag == "EXT-X-MAP":
                         info = _get_tuple_attribute(attr)
+                        self.media_segment.insert(0, {"URI": info["URI"], "EXTINF": {"duration": 0}})
 
                     # 4.3.2.6.  EXT-X-PROGRAM-DATE-TIME"
                     elif tag == "EXT-X-PROGRAM-DATE-TIME":
                         info = attr
 
                     # 4.3.2.7.  EXT-X-DATERANGE
                     elif tag == "EXT-X-DATERANGE":
```

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/fetcher/http.py` & `svtplay-dl-4.9/lib/svtplay_dl/fetcher/http.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/postprocess/__init__.py` & `svtplay-dl-4.9/lib/svtplay_dl/postprocess/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.detect = None
         for i in ["ffmpeg", "avconv"]:
             self.detect = which(i)
             if self.detect:
                 break
         if self.detect is None and platform.system() == "Windows":
             path = pathlib.Path(sys.executable).parent / "ffmpeg.exe"
-            if path.is_file:
+            if os.path.isfile(path):
                 self.detect = path
 
     def merge(self):
         if self.detect is None:
             logging.error("Cant detect ffmpeg or avconv. Cant mux files without it.")
             return
         if self.stream.finished is False:
@@ -120,15 +120,15 @@
             os.remove(orig_filename)
         if (self.stream.audio and self.config.get("only_audio")) or (self.stream.audio and not self.config.get("only_video")):
             os.remove(audio_filename)
 
         if self.config.get("merge_subtitle"):
             if self.subfixes and len(self.subfixes) >= 2:
                 for subfix in self.subfixes:
-                    subfile = orig_filename.parent / (orig_filename.name + "." + subfix + ".srt")
+                    subfile = orig_filename.parent / (orig_filename.stem + "." + subfix + ".srt")
                     os.remove(subfile)
             else:
                 os.remove(subfile)
         os.rename(tempfile, new_name)
 
 
 def _streams(output):
```

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/__init__.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/__init__.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/aftonbladet.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/aftonbladet.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/atg.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/atg.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/barnkanalen.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/barnkanalen.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/bigbrother.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/bigbrother.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/cmore.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/cmore.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/disney.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/disney.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/dplay.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/dplay.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/dr.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/dr.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/efn.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/efn.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/eurosport.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/eurosport.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/expressen.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/expressen.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/facebook.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/facebook.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/filmarkivet.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/filmarkivet.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/flowonline.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/flowonline.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/koket.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/koket.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/lemonwhale.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/lemonwhale.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/mtvnn.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/mtvnn.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/mtvservices.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/mtvservices.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/nhl.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/nhl.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/npo.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/npo.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/nrk.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/nrk.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/oppetarkiv.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/oppetarkiv.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/picsearch.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/picsearch.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/pokemon.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/pokemon.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/radioplay.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/radioplay.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/raw.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/raw.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/riksdagen.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/riksdagen.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/ruv.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/ruv.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/services.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/services.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/solidtango.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/solidtango.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/sportlib.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/sportlib.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/sr.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/sr.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/svt.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/svt.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/svtplay.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/svtplay.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,17 @@
 
         res = self.http.get(URL_VIDEO_API + vid)
         try:
             janson = res.json()
         except json.decoder.JSONDecodeError:
             yield ServiceError(f"Can't decode api request: {res.request.url}")
             return
+        if res.status_code >= 400:
+            yield ServiceError("Can't find any videos. its removed?")
+            return
         videos = self._get_video(janson)
         yield from videos
 
     def _get_video(self, janson):
         if "subtitleReferences" in janson:
             for i in janson["subtitleReferences"]:
                 if i["format"] == "webvtt" and "url" in i:
@@ -102,15 +105,15 @@
 
         if "videoReferences" in janson:
             if len(janson["videoReferences"]) == 0:
                 yield ServiceError("Media doesn't have any associated videos.")
                 return
 
             for i in janson["videoReferences"]:
-                if i["url"].find(".m3u8") > 0 and "hls-cmaf" in i["format"]:
+                if i["url"].find(".m3u8") > 0:
                     yield from hlsparse(self.config, self.http.request("get", i["url"]), i["url"], self.output)
                 elif i["url"].find(".mpd") > 0:
                     yield from dashparse(self.config, self.http.request("get", i["url"]), i["url"], output=self.output)
 
     def _last_chance(self):
         videos = []
         match = re.search(self.info_search_expr, self.get_urldata())
```

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/tv4play.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/tv4play.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/twitch.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/twitch.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/urplay.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/urplay.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 # ex:ts=4:sw=4:sts=4:et
 # -*- tab-width: 4; c-basic-offset: 4; indent-tabs-mode: nil -*-
 import copy
 import json
 import logging
 import re
 from html import unescape
+from urllib.parse import urljoin
 
 from svtplay_dl.error import ServiceError
 from svtplay_dl.fetcher.hls import hlsparse
 from svtplay_dl.service import OpenGraphThumbMixin
 from svtplay_dl.service import Service
 from svtplay_dl.subtitle import subtitle
 
 
 class Urplay(Service, OpenGraphThumbMixin):
     supported_domains = ["urplay.se", "ur.se", "betaplay.ur.se", "urskola.se"]
 
     def get(self):
         urldata = self.get_urldata()
-        key = "currentProduct"
-        match = re.search(r'/Player/Player" data-react-props="([^\"]+)\"', urldata)
+        match = re.search(r"__NEXT_DATA__\" type=\"application\/json\">({.+})<\/script>", urldata)
         if not match:
-            key = "program"
-            match = re.search(r'/ProgramContainer" data-react-props="([^\"]+)\"', self.get_urldata())
-            if not match:
-                yield ServiceError("Can't find json info")
-                return
+            yield ServiceError("Can't find video info.")
+            return
 
         data = unescape(match.group(1))
         jsondata = json.loads(data)
 
         res = self.http.get("https://streaming-loadbalancer.ur.se/loadbalancer.json")
         loadbalancer = res.json()["redirect"]
+        jsondata = jsondata["props"]["pageProps"]["program"]
 
-        self.outputfilename(jsondata[key], urldata)
+        self.outputfilename(jsondata, urldata)
 
-        for streaminfo in jsondata[key]["streamingInfo"].keys():
-            stream = jsondata[key]["streamingInfo"][streaminfo]
+        for streaminfo in jsondata["streamingInfo"].keys():
+            stream = jsondata["streamingInfo"][streaminfo]
 
             if streaminfo == "raw":
                 if "sd" in stream:
                     url = "https://{}/{}playlist.m3u8".format(loadbalancer, stream["sd"]["location"])
                     yield from hlsparse(self.config, self.http.request("get", url), url, output=self.output)
                 if "hd" in stream:
                     url = "https://{}/{}playlist.m3u8".format(loadbalancer, stream["hd"]["location"])
@@ -53,26 +51,30 @@
                 if stream["tt"]["scope"] != "complete":
                     label = "{}-{}".format(label, stream["tt"]["scope"])
                 yield subtitle(copy.copy(self.config), "wrst", stream["tt"]["location"].replace(".tt", ".vtt"), label, output=copy.copy(self.output))
 
     def find_all_episodes(self, config):
         episodes = []
 
-        match = re.search(r'/Player/Player" data-react-props="([^\"]+)\"', self.get_urldata())
+        match = re.search(r"__NEXT_DATA__\" type=\"application\/json\">({.+})<\/script>", self.get_urldata())
         if not match:
-            match = re.search(r'/ProgramContainer" data-react-props="([^\"]+)\"', self.get_urldata())
-            if not match:
-                logging.error("Can't find json info")
-                return
+            logging.error("Can't find video info.")
+            return
 
         data = unescape(match.group(1))
         jsondata = json.loads(data)
-
-        for episode in jsondata["accessibleEpisodes"]:
-            episodes.append("https://urplay.se/program/{}".format(episode["slug"]))
+        seasons = jsondata["props"]["pageProps"]["superSeriesSeasons"]
+        if seasons:
+            for season in seasons:
+                res = self.http.get(f'https://urplay.se/api/v1/series?id={season["id"]}')
+                for episode in res.json()["programs"]:
+                    episodes.append(urljoin("https://urplay.se", episode["link"]))
+        else:
+            for episode in jsondata["props"]["pageProps"]["accessibleEpisodes"]:
+                episodes.append(urljoin("https://urplay.se", episode["link"]))
         episodes_new = []
         n = 0
         for i in episodes:
             if n == config.get("all_last"):
                 break
             if i not in episodes_new:
                 episodes_new.append(i)
@@ -90,12 +92,12 @@
                 self.output["title"] = data["title"]
             else:
                 self.output["episodename"] = data["title"]
         if "id" in data and data["id"]:
             self.output["id"] = str(data["id"])
 
         # Try to match Season info from HTML (not available in json, it seems), e.g.: <button class="SeasonsDropdown-module__seasonButton___25Uyt" type="button"><span>Säsong 6</span>
-        seasonmatch = re.search(r"class..SeasonsDropdown-module__seasonButton.*span.S.song (\d+)..span", urldata)
+        seasonmatch = re.search(r"data-testid=\"season-name-label\">S.song (\d+)...<\/span", urldata)
         if seasonmatch:
             self.output["season"] = seasonmatch.group(1)
         else:
             self.output["season"] = "1"  # No season info - probably show without seasons
```

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/vg.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/vg.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/viaplay.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/viaplay.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/viasatsport.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/viasatsport.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/vimeo.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/vimeo.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/service/youplay.py` & `svtplay-dl-4.9/lib/svtplay_dl/service/youplay.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/subtitle/__init__.py` & `svtplay-dl-4.9/lib/svtplay_dl/subtitle/__init__.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/utils/getmedia.py` & `svtplay-dl-4.9/lib/svtplay_dl/utils/getmedia.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/utils/http.py` & `svtplay-dl-4.9/lib/svtplay_dl/utils/http.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/utils/nfo.py` & `svtplay-dl-4.9/lib/svtplay_dl/utils/nfo.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/utils/output.py` & `svtplay-dl-4.9/lib/svtplay_dl/utils/output.py`

 * *Files 8% similar despite different names*

```diff
@@ -125,37 +125,47 @@
             stream.config.set("output_auto", True)
             title_tag = decode_html_entities(match.group(1))
             stream.output["title"] = filenamify(title_tag)
     return True
 
 
 def formatname(output, config):
-    name = pathlib.Path(_formatname(output, config)).expanduser().resolve()
+    name = pathlib.Path(_formatname(output, config))
+    subfolder = None
+    dirname = None
+
     if not output.get("basedir", False):
         # If tvshow have not been derived by service do it by if season and episode is set
         if output.get("tvshow", None) is None:
             tvshow = output.get("season", None) is not None and output.get("episode", None) is not None
         else:
             tvshow = output.get("tvshow", False)
         if config.get("subfolder") and "title" in output and tvshow:
             # Add subfolder with name title
-            name = pathlib.Path(output["title"]) / name.name
+            subfolder = pathlib.Path(output["title"])
         elif config.get("subfolder") and not tvshow:
             # Add subfolder with name movies
-            name = pathlib.Path("movies") / name.name
+            subfolder = pathlib.Path("movies")
     if config.get("output") and pathlib.Path(config.get("output")).expanduser().is_dir():
-        name = pathlib.Path(config.get("output")).expanduser() / name.name
+        dirname = pathlib.Path(config.get("output"))
     elif config.get("path") and pathlib.Path(config.get("path")).expanduser().is_dir():
-        name = pathlib.Path(config.get("path")).expanduser() / name.name
+        dirname = pathlib.Path(config.get("path"))
     elif config.get("output"):
         if output["ext"]:
-            name = pathlib.Path(f"{config.get('output')}.{output['ext']}").expanduser()
+            name = pathlib.Path(f"{config.get('output')}.{output['ext']}")
         else:
-            name = pathlib.Path(config.get("output")).expanduser()
-    return name
+            name = pathlib.Path(config.get("output"))
+    if subfolder and dirname:
+        return dirname / subfolder / name.expanduser()
+    elif subfolder:
+        return subfolder / name.expanduser()
+    elif dirname:
+        return dirname / name.expanduser()
+    else:
+        return name.expanduser()
 
 
 def _formatname(output, config):
     name = config.get("filename")
     for key in output:
         if key == "title" and output[key]:
             name = name.replace("{title}", filenamify(output[key]))
```

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/utils/parser.py` & `svtplay-dl-4.9/lib/svtplay_dl/utils/parser.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/utils/stream.py` & `svtplay-dl-4.9/lib/svtplay_dl/utils/stream.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/utils/terminal.py` & `svtplay-dl-4.9/lib/svtplay_dl/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl/utils/text.py` & `svtplay-dl-4.9/lib/svtplay_dl/utils/text.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/lib/svtplay_dl.egg-info/PKG-INFO` & `svtplay-dl-4.9/lib/svtplay_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svtplay-dl
-Version: 4.8
+Version: 4.9
 Summary: Command-line program to download videos from various video on demand sites
 Home-page: https://svtplay-dl.se
 Author: Johan Andersson
 Author-email: j@i19.se
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `svtplay-dl-4.8/lib/svtplay_dl.egg-info/SOURCES.txt` & `svtplay-dl-4.9/lib/svtplay_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/setup.py` & `svtplay-dl-4.9/setup.py`

 * *Files identical despite different names*

### Comparing `svtplay-dl-4.8/versioneer.py` & `svtplay-dl-4.9/versioneer.py`

 * *Files identical despite different names*

