# Comparing `tmp/nomenklatura-2.9.4.tar.gz` & `tmp/nomenklatura-2.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomenklatura-2.9.4.tar", last modified: Wed Apr 19 19:57:50 2023, max compression
+gzip compressed data, was "nomenklatura-2.9.5.tar", last modified: Tue Apr 25 08:10:40 2023, max compression
```

## Comparing `nomenklatura-2.9.4.tar` & `nomenklatura-2.9.5.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:50.567531 nomenklatura-2.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-19 19:57:50.567531 nomenklatura-2.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:50.563531 nomenklatura-2.9.4/nomenklatura/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:50.563531 nomenklatura-2.9.4/nomenklatura/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/data/match-regression.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:50.563531 nomenklatura-2.9.4/nomenklatura/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/dataset/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/dataset/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/dataset/publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/dataset/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/dataset/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:50.563531 nomenklatura-2.9.4/nomenklatura/enrich/
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/enrich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/enrich/aleph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/enrich/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/enrich/nominatim.py
--rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/enrich/opencorporates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:50.563531 nomenklatura-2.9.4/nomenklatura/enrich/wikidata/
--rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/enrich/wikidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/enrich/wikidata/lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/enrich/wikidata/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/enrich/wikidata/props.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/enrich/wikidata/qualified.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/enrich/wikidata/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/enrich/yente.py
--rw-r--r--   0 runner    (1001) docker     (123)    15759 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:50.563531 nomenklatura-2.9.4/nomenklatura/index/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/index/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/index/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/index/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/judgement.py
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:50.567531 nomenklatura-2.9.4/nomenklatura/matching/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/matching/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:50.567531 nomenklatura-2.9.4/nomenklatura/matching/features/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/matching/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/matching/features/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/matching/features/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/matching/features/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/matching/features/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/matching/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/matching/pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/matching/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/matching/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:50.567531 nomenklatura-2.9.4/nomenklatura/publish/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/publish/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/publish/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/publish/names.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:50.567531 nomenklatura-2.9.4/nomenklatura/resolver/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/resolver/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/resolver/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/resolver/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/resolver/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/senzing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:50.567531 nomenklatura-2.9.4/nomenklatura/statement/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/statement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/statement/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/statement/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:50.567531 nomenklatura-2.9.4/nomenklatura/tui/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/tui/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/tui/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/tui/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/xref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:50.563531 nomenklatura-2.9.4/nomenklatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-19 19:57:50.000000 nomenklatura-2.9.4/nomenklatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-19 19:57:50.000000 nomenklatura-2.9.4/nomenklatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:57:50.000000 nomenklatura-2.9.4/nomenklatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-19 19:57:50.000000 nomenklatura-2.9.4/nomenklatura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:57:50.000000 nomenklatura-2.9.4/nomenklatura.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:57:10.000000 nomenklatura-2.9.4/nomenklatura.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-19 19:57:50.000000 nomenklatura-2.9.4/nomenklatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-19 19:57:50.000000 nomenklatura-2.9.4/nomenklatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 19:57:50.567531 nomenklatura-2.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:10:40.022672 nomenklatura-2.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-04-25 08:10:40.022672 nomenklatura-2.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:10:40.014672 nomenklatura-2.9.5/nomenklatura/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:10:40.018672 nomenklatura-2.9.5/nomenklatura/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/data/match-regression.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:10:40.018672 nomenklatura-2.9.5/nomenklatura/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/dataset/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/dataset/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/dataset/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/dataset/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/dataset/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:10:40.018672 nomenklatura-2.9.5/nomenklatura/enrich/
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/enrich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/enrich/aleph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/enrich/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/enrich/nominatim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/enrich/opencorporates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:10:40.018672 nomenklatura-2.9.5/nomenklatura/enrich/wikidata/
+-rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/enrich/wikidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/enrich/wikidata/lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/enrich/wikidata/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/enrich/wikidata/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/enrich/wikidata/qualified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/enrich/wikidata/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/enrich/yente.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15759 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:10:40.018672 nomenklatura-2.9.5/nomenklatura/index/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/index/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/index/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/index/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/judgement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:10:40.018672 nomenklatura-2.9.5/nomenklatura/matching/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/matching/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:10:40.018672 nomenklatura-2.9.5/nomenklatura/matching/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/matching/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/matching/features/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/matching/features/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/matching/features/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/matching/features/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/matching/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/matching/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/matching/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/matching/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:10:40.018672 nomenklatura-2.9.5/nomenklatura/publish/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/publish/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/publish/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/publish/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:10:40.022672 nomenklatura-2.9.5/nomenklatura/resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/resolver/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/resolver/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/resolver/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/resolver/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/senzing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:10:40.022672 nomenklatura-2.9.5/nomenklatura/statement/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/statement/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/statement/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:10:40.022672 nomenklatura-2.9.5/nomenklatura/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/tui/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/tui/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/tui/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/nomenklatura/xref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:10:40.018672 nomenklatura-2.9.5/nomenklatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-04-25 08:10:39.000000 nomenklatura-2.9.5/nomenklatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-25 08:10:39.000000 nomenklatura-2.9.5/nomenklatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:10:39.000000 nomenklatura-2.9.5/nomenklatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-25 08:10:39.000000 nomenklatura-2.9.5/nomenklatura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:10:39.000000 nomenklatura-2.9.5/nomenklatura.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:09:53.000000 nomenklatura-2.9.5/nomenklatura.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-25 08:10:39.000000 nomenklatura-2.9.5/nomenklatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-25 08:10:39.000000 nomenklatura-2.9.5/nomenklatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 08:10:40.022672 nomenklatura-2.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-25 08:08:18.000000 nomenklatura-2.9.5/setup.py
```

### Comparing `nomenklatura-2.9.4/LICENSE` & `nomenklatura-2.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/PKG-INFO` & `nomenklatura-2.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 2.9.4
+Version: 2.9.5
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # nomenklatura
 
 Nomenklatura de-duplicates and integrates different [Follow the Money](https://followthemoney.rtfd.org/) entities. It serves to clean up messy data and to find links between different datasets.
@@ -90,7 +91,9 @@
 ## Contact, contributions etc.
 
 This codebase is licensed under the terms of an MIT license (see LICENSE).
 
 We're keen for any contributions, bug fixes and feature suggestions, please use the GitHub issue tracker for this repository. 
 
 Nomenklatura is currently developed thanks to a Prototypefund grant for [OpenSanctions](https://opensanctions.org). Previous iterations of the package were developed with support from [Knight-Mozilla OpenNews](http://opennews.org) and the [Open Knowledge Foundation Labs](http://okfnlabs.org).
+
+
```

### Comparing `nomenklatura-2.9.4/README.md` & `nomenklatura-2.9.5/README.md`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/cache.py` & `nomenklatura-2.9.5/nomenklatura/cache.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/cli.py` & `nomenklatura-2.9.5/nomenklatura/cli.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/data/match-regression.pkl` & `nomenklatura-2.9.5/nomenklatura/data/match-regression.pkl`

 * *Files 15% similar despite different names*

```diff
@@ -12,55 +12,55 @@
 000000b0: 0e6e 5f66 6561 7475 7265 735f 696e 5f94  .n_features_in_.
 000000c0: 4b11 8c0f 6e5f 7361 6d70 6c65 735f 7365  K...n_samples_se
 000000d0: 656e 5f94 8c15 6e75 6d70 792e 636f 7265  en_...numpy.core
 000000e0: 2e6d 756c 7469 6172 7261 7994 8c06 7363  .multiarray...sc
 000000f0: 616c 6172 9493 948c 056e 756d 7079 948c  alar.....numpy..
 00000100: 0564 7479 7065 9493 948c 0269 3894 8988  .dtype.....i8...
 00000110: 8794 5294 284b 038c 013c 944e 4e4e 4aff  ..R.(K...<.NNNJ.
-00000120: ffff ff4a ffff ffff 4b00 7494 6243 086a  ...J....K.t.bC.j
-00000130: 1f04 0000 0000 0094 8694 5294 8c05 6d65  ..........R...me
+00000120: ffff ff4a ffff ffff 4b00 7494 6243 08c4  ...J....K.t.bC..
+00000130: 8004 0000 0000 0094 8694 5294 8c05 6d65  ..........R...me
 00000140: 616e 5f94 6814 8c0c 5f72 6563 6f6e 7374  an_.h..._reconst
 00000150: 7275 6374 9493 9468 178c 076e 6461 7272  ruct...h...ndarr
 00000160: 6179 9493 944b 0085 9443 0162 9487 9452  ay...K...C.b...R
 00000170: 9428 4b01 4b11 8594 6819 8c02 6638 9489  .(K.K...h...f8..
 00000180: 8887 9452 9428 4b03 681d 4e4e 4e4a ffff  ...R.(K.h.NNNJ..
-00000190: ffff 4aff ffff ff4b 0074 9462 8943 8855  ..J....K.t.b.C.U
-000001a0: 89e5 78e2 252e 4097 8954 ca1b a1e6 3f74  ..x.%.@..T....?t
-000001b0: a040 a8fc d341 3f9f 26b7 d17c 47e9 3fc2  .@...A?.&..|G.?.
-000001c0: e7b4 1b37 2b4f 3f74 a7ca 7a9a 5065 3f4e  ...7+O?t..z.Pe?N
-000001d0: 5588 1876 5074 3f36 a67d c6db 7bd3 3fa5  U..vPt?6.}..{.?.
-000001e0: b5ed 63d7 9dca 3f6b fcb6 b999 66bd 3f5a  ..c...?k....f.?Z
-000001f0: f636 643c 57b9 3f20 8f34 f3d8 88b8 3f3e  .6d<W.? .4....?>
-00000200: 8161 3a08 2265 3fa4 4f3e 164e 859e 3fd0  .a:."e?.O>.N..?.
-00000210: bc7f f0a3 d0af 3f3e ab4b a353 1db0 3f62  ......?>.K.S..?b
-00000220: 8e80 007b 87a2 bf94 7494 628c 0476 6172  ...{....t.b..var
+00000190: ffff 4aff ffff ff4b 0074 9462 8943 88b4  ..J....K.t.b.C..
+000001a0: cf8e 2ba7 7f2e 40ce d0ea 414b b6e6 3ff9  ..+...@...AK..?.
+000001b0: faf8 96fb a645 3fdb 1928 0a01 81e9 3f70  .....E?..(....?p
+000001c0: 10af acba fa4e 3fd9 8f10 4baf ca64 3f01  .....N?...K..d?.
+000001d0: 02ef f0d5 a87f 3ffa b0d5 701a fcd2 3ff8  ......?...p...?.
+000001e0: a579 6e42 e7c9 3f9b c46c ee18 1fbe 3fd7  .ynB..?..l....?.
+000001f0: e6c2 47e7 13b8 3f76 ea8e 1cbb 70b7 3f97  ..G...?v....p.?.
+00000200: c910 3a42 1262 3f7e 3468 81f2 009f 3f5d  ..:B.b?~4h....?]
+00000210: 8e7c 4846 b1af 3f73 306b 3e49 c5ae 3f56  .|HF..?s0k>I..?V
+00000220: 063e bdd6 e2a3 bf94 7494 628c 0476 6172  .>......t.b..var
 00000230: 5f94 6824 6826 4b00 8594 6828 8794 5294  _.h$h&K...h(..R.
-00000240: 284b 014b 1185 9468 2e89 4388 f5d7 9124  (K.K...h..C....$
-00000250: 99c9 6b40 c431 6fdf a338 c03f 500d 0ffa  ..k@.1o..8.?P...
-00000260: 80d1 413f be09 4b53 9fd3 bc3f fe96 30cf  ..A?..KS...?..0.
-00000270: 200a 6e3f 7102 86f9 e63e 813f adc8 45b9   .n?q....>.?..E.
-00000280: d1ae b03f 75ab 1868 c64f d33f 4b5c 893f  ...?u..h.O.?K\.?
-00000290: f514 c53f 95f6 d938 ba16 c23f 4b24 c870  ...?...8...?K$.p
-000002a0: b76f bd3f 9980 c322 3c6c b13f a4d4 636b  .o.?..."<l.?..ck
-000002b0: 1314 653f 3e9f 6128 6d9c 9d3f 83cc db8a  ..e?>.a(m..?....
-000002c0: 7113 bc3f daa4 d67b 9f6d a73f b563 86d5  q..?...{.m.?.c..
-000002d0: 5b4b d93f 9474 9462 8c06 7363 616c 655f  [K.?.t.b..scale_
+00000240: 284b 014b 1185 9468 2e89 4388 53ab bc30  (K.K...h..C.S..0
+00000250: 9d00 6c40 1694 ddee e6c0 bf3f 8deb 94f2  ..l@.......?....
+00000260: 51a3 453f 3a2b d878 46af bb3f d6de 9ffc  Q.E?:+.xF..?....
+00000270: c42a 6e3f ec84 e7e8 71b4 803f bf2c 1acd  .*n?....q..?.,..
+00000280: 522c b23f 5cc4 3944 720d d33f 1a78 68a9  R,.?\.9Dr..?.xh.
+00000290: 4aa9 c43f ffd9 9e29 728d c23f 7b6d b9d6  J..?...)r..?{m..
+000002a0: 218a bc3f 1f5c f9d2 4aba b03f 4f22 24a5  !..?.\..J..?O"$.
+000002b0: 0d08 623f 6f7f 59d2 a310 9e3f c053 1c8d  ..b?o.Y....?.S..
+000002c0: 82b8 bc3f 9a5f f82c 6854 a63f fb81 184a  ...?._.,hT.?...J
+000002d0: 6217 da3f 9474 9462 8c06 7363 616c 655f  b..?.t.b..scale_
 000002e0: 9468 2468 264b 0085 9468 2887 9452 9428  .h$h&K...h(..R.(
-000002f0: 4b01 4b11 8594 682e 8943 8839 27dc abc7  K.K...h..C.9'...
-00000300: d12d 4089 3b27 2888 c8d6 3fda 0e32 88ec  .-@.;'(...?..2..
-00000310: e097 3f6b 9706 12e7 79d5 3f5c 3526 2c19  ..?k....y.?\5&,.
-00000320: 01af 3ff5 d023 f9e3 7db7 3fbd edb5 0f7f  ..?..#..}.?.....
-00000330: 56d0 3fbf feb4 89f7 93e1 3fa5 9f52 9233  V.?.......?..R.3
-00000340: f9d9 3f7f 2a32 0b22 0fd8 3f0c e057 8cbe  ..?.*2."..?..W..
-00000350: b3d5 3fd0 4234 473d b2d0 3f11 36c9 73a8  ..?.B4G=..?.6.s.
-00000360: f8a9 3f57 60ab 8333 c4c5 3fe2 2a37 b9d7  ..?W`..3..?.*7..
-00000370: 31d5 3f57 bc27 b975 61cb 3fca 8090 260e  1.?W.'.ua.?...&.
-00000380: 1ee4 3f94 7494 628c 105f 736b 6c65 6172  ..?.t.b.._sklear
+000002f0: 4b01 4b11 8594 682e 8943 88fd 7886 163e  K.K...h..C..x..>
+00000300: ef2d 40ec cea3 6344 8ad6 3f67 7b6d e153  .-@...cD..?g{m.S
+00000310: 509a 3f05 d754 b6e6 0bd5 3ffe 950c e0ec  P.?..T....?.....
+00000320: 11af 3f45 9414 65d6 1eb7 3f4c a0bc ee4e  ..?E..e...?L...N
+00000330: 0dd1 3f28 2be8 88ad 75e1 3f79 6f16 1a8b  ..?(+...u.?yo...
+00000340: b6d9 3f9f 4909 a695 5dd8 3f6d 6790 6775  ..?.I...].?mg.gu
+00000350: 5ed5 3f1c 99cc 461c 5cd0 3f4d 117f d45d  ^.?...F.\.?M...]
+00000360: 05a8 3fd5 9c4b 72c0 eec5 3fa1 02a5 36cb  ..?..Kr...?...6.
+00000370: 6fd5 3fd9 73f4 5628 bbca 3f8b f01f 548f  o.?.s.V(..?...T.
+00000380: 6ee4 3f94 7494 628c 105f 736b 6c65 6172  n.?.t.b.._sklear
 00000390: 6e5f 7665 7273 696f 6e94 8c05 312e 322e  n_version...1.2.
-000003a0: 3194 7562 8694 8c12 6c6f 6769 7374 6963  1.ub....logistic
+000003a0: 3294 7562 8694 8c12 6c6f 6769 7374 6963  2.ub....logistic
 000003b0: 7265 6772 6573 7369 6f6e 948c 1e73 6b6c  regression...skl
 000003c0: 6561 726e 2e6c 696e 6561 725f 6d6f 6465  earn.linear_mode
 000003d0: 6c2e 5f6c 6f67 6973 7469 6394 8c12 4c6f  l._logistic...Lo
 000003e0: 6769 7374 6963 5265 6772 6573 7369 6f6e  gisticRegression
 000003f0: 9493 9429 8194 7d94 288c 0770 656e 616c  ...)..}.(..penal
 00000400: 7479 948c 026c 3294 8c04 6475 616c 9489  ty...l2...dual..
 00000410: 8c03 746f 6c94 473f 1a36 e2eb 1c43 2d8c  ..tol.G?.6...C-.
@@ -79,64 +79,64 @@
 000004e0: 7365 735f 9468 2468 264b 0085 9468 2887  ses_.h$h&K...h(.
 000004f0: 9452 9428 4b01 4b02 8594 681c 8943 1000  .R.(K.K...h..C..
 00000500: 0000 0000 0000 0001 0000 0000 0000 0094  ................
 00000510: 7494 628c 076e 5f69 7465 725f 9468 2468  t.b..n_iter_.h$h
 00000520: 264b 0085 9468 2887 9452 9428 4b01 4b01  &K...h(..R.(K.K.
 00000530: 8594 6819 8c02 6934 9489 8887 9452 9428  ..h...i4.....R.(
 00000540: 4b03 681d 4e4e 4e4a ffff ffff 4aff ffff  K.h.NNNJ....J...
-00000550: ff4b 0074 9462 8943 041c 0000 0094 7494  .K.t.b.C......t.
+00000550: ff4b 0074 9462 8943 041f 0000 0094 7494  .K.t.b.C......t.
 00000560: 628c 0563 6f65 665f 9468 2468 264b 0085  b..coef_.h$h&K..
 00000570: 9468 2887 9452 9428 4b01 4b01 4b11 8694  .h(..R.(K.K.K...
-00000580: 682e 8943 884a 338e a74e 8bec 3fc5 c406  h..C.J3..N..?...
-00000590: 4d41 10b6 3fc8 cc42 a935 e0ce bf10 604c  MA..?..B.5....`L
-000005a0: fa76 79eb 3fc6 a223 712b d098 3f1c 893d  .vy.?..#q+..?..=
-000005b0: f83e aaac 3f59 9587 4869 44cb 3fdf 60aa  .>..?Y..HiD.?.`.
-000005c0: 8032 01f2 3f1b 25f4 b59c 6fd1 3f2d 9065  .2..?.%...o.?-.e
-000005d0: b83c 16ab 3fb0 b84c 3b9e ccbe 3f0f 2ef1  .<..?..L;...?...
-000005e0: f492 b8b1 bfee b0be 2ed9 cec5 bf00 ae40  ...............@
-000005f0: 8a82 18d1 bfb7 e868 ff38 29e3 3f1a 99e8  .......h.8).?...
-00000600: 594e d5ee 3ff6 1868 9f8e 2aaf 3f94 7494  YN..?..h..*.?.t.
+00000580: 682e 8943 8835 2e64 3b1b faec 3f00 8e32  h..C.5.d;...?..2
+00000590: c158 45b2 3f0e 7f68 1ce5 e5d0 bfaf 593a  .XE.?..h......Y:
+000005a0: a175 01eb 3ff1 0bc1 2ade cc96 3f69 2abd  .u..?...*...?i*.
+000005b0: 0a33 38a4 3fda c5fb d8b0 c6ca 3f85 d679  .38.?.......?..y
+000005c0: 2fa9 8af1 3f1a 9a9c e0c5 12d1 3fe1 4c75  /...?.......?.Lu
+000005d0: 8dfc d5a4 3f34 b3e1 26b4 68c1 3ff6 cef0  ....?4..&.h.?...
+000005e0: 48bf eaa6 bfe1 09ba 536a 92ce bf9b d957  H.......Sj.....W
+000005f0: 3f35 5bd2 bf9d a7fb a273 14e3 3ff5 21e3  ?5[......s..?.!.
+00000600: ae18 52ed 3ff5 3150 3a3a 40ae 3f94 7494  ..R.?.1P::@.?.t.
 00000610: 628c 0a69 6e74 6572 6365 7074 5f94 6824  b..intercept_.h$
 00000620: 6826 4b00 8594 6828 8794 5294 284b 014b  h&K...h(..R.(K.K
-00000630: 0185 9468 2e89 4308 51d4 ef38 0d09 0240  ...h..C.Q..8...@
+00000630: 0185 9468 2e89 4308 ad0d f310 190a 0240  ...h..C........@
 00000640: 9474 9462 6840 6841 7562 8694 658c 066d  .t.bh@hAub..e..m
 00000650: 656d 6f72 7994 4e68 5789 6840 6841 7562  emory.NhW.h@hAub
 00000660: 8c0c 636f 6566 6669 6369 656e 7473 947d  ..coefficients.}
 00000670: 9428 8c0a 6e61 6d65 5f6d 6174 6368 9468  .(..name_match.h
-00000680: 1668 2e43 084a 338e a74e 8bec 3f94 8694  .h.C.J3..N..?...
+00000680: 1668 2e43 0835 2e64 3b1b faec 3f94 8694  .h.C.5.d;...?...
 00000690: 5294 8c12 6e61 6d65 5f74 6f6b 656e 5f6f  R...name_token_o
-000006a0: 7665 726c 6170 9468 1668 2e43 08c5 c406  verlap.h.h.C....
-000006b0: 4d41 10b6 3f94 8694 5294 8c0c 6e61 6d65  MA..?...R...name
-000006c0: 5f6e 756d 6265 7273 9468 1668 2e43 08c8  _numbers.h.h.C..
-000006d0: cc42 a935 e0ce bf94 8694 5294 8c10 6e61  .B.5......R...na
+000006a0: 7665 726c 6170 9468 1668 2e43 0800 8e32  verlap.h.h.C...2
+000006b0: c158 45b2 3f94 8694 5294 8c0c 6e61 6d65  .XE.?...R...name
+000006c0: 5f6e 756d 6265 7273 9468 1668 2e43 080e  _numbers.h.h.C..
+000006d0: 7f68 1ce5 e5d0 bf94 8694 5294 8c10 6e61  .h........R...na
 000006e0: 6d65 5f6c 6576 656e 7368 7465 696e 9468  me_levenshtein.h
-000006f0: 1668 2e43 0810 604c fa76 79eb 3f94 8694  .h.C..`L.vy.?...
+000006f0: 1668 2e43 08af 593a a175 01eb 3f94 8694  .h.C..Y:.u..?...
 00000700: 5294 8c0b 7068 6f6e 655f 6d61 7463 6894  R...phone_match.
-00000710: 6816 682e 4308 c6a2 2371 2bd0 983f 9486  h.h.C...#q+..?..
+00000710: 6816 682e 4308 f10b c12a decc 963f 9486  h.h.C....*...?..
 00000720: 9452 948c 0b65 6d61 696c 5f6d 6174 6368  .R...email_match
-00000730: 9468 1668 2e43 081c 893d f83e aaac 3f94  .h.h.C...=.>..?.
+00000730: 9468 1668 2e43 0869 2abd 0a33 38a4 3f94  .h.h.C.i*..38.?.
 00000740: 8694 5294 8c10 6964 656e 7469 6669 6572  ..R...identifier
-00000750: 5f6d 6174 6368 9468 1668 2e43 0859 9587  _match.h.h.C.Y..
-00000760: 4869 44cb 3f94 8694 5294 8c0b 646f 625f  HiD.?...R...dob_
-00000770: 6d61 7463 6865 7394 6816 682e 4308 df60  matches.h.h.C..`
-00000780: aa80 3201 f23f 9486 9452 948c 1064 6f62  ..2..?...R...dob
+00000750: 5f6d 6174 6368 9468 1668 2e43 08da c5fb  _match.h.h.C....
+00000760: d8b0 c6ca 3f94 8694 5294 8c0b 646f 625f  ....?...R...dob_
+00000770: 6d61 7463 6865 7394 6816 682e 4308 85d6  matches.h.h.C...
+00000780: 792f a98a f13f 9486 9452 948c 1064 6f62  y/...?...R...dob
 00000790: 5f79 6561 725f 6d61 7463 6865 7394 6816  _year_matches.h.
-000007a0: 682e 4308 1b25 f4b5 9c6f d13f 9486 9452  h.C..%...o.?...R
+000007a0: 682e 4308 1a9a 9ce0 c512 d13f 9486 9452  h.C........?...R
 000007b0: 948c 1066 6972 7374 5f6e 616d 655f 6d61  ...first_name_ma
-000007c0: 7463 6894 6816 682e 4308 2d90 65b8 3c16  tch.h.h.C.-.e.<.
-000007d0: ab3f 9486 9452 948c 1166 616d 696c 795f  .?...R...family_
+000007c0: 7463 6894 6816 682e 4308 e14c 758d fcd5  tch.h.h.C..Lu...
+000007d0: a43f 9486 9452 948c 1166 616d 696c 795f  .?...R...family_
 000007e0: 6e61 6d65 5f6d 6174 6368 9468 1668 2e43  name_match.h.h.C
-000007f0: 08b0 b84c 3b9e ccbe 3f94 8694 5294 8c0b  ...L;...?...R...
+000007f0: 0834 b3e1 26b4 68c1 3f94 8694 5294 8c0b  .4..&.h.?...R...
 00000800: 6269 7274 685f 706c 6163 6594 6816 682e  birth_place.h.h.
-00000810: 4308 0f2e f1f4 92b8 b1bf 9486 9452 948c  C............R..
+00000810: 4308 f6ce f048 bfea a6bf 9486 9452 948c  C....H.......R..
 00000820: 0f67 656e 6465 725f 6d69 736d 6174 6368  .gender_mismatch
-00000830: 9468 1668 2e43 08ee b0be 2ed9 cec5 bf94  .h.h.C..........
+00000830: 9468 1668 2e43 08e1 09ba 536a 92ce bf94  .h.h.C....Sj....
 00000840: 8694 5294 8c10 636f 756e 7472 795f 6d69  ..R...country_mi
-00000850: 736d 6174 6368 9468 1668 2e43 0800 ae40  smatch.h.h.C...@
-00000860: 8a82 18d1 bf94 8694 5294 8c14 6f72 675f  ........R...org_
+00000850: 736d 6174 6368 9468 1668 2e43 089b d957  smatch.h.h.C...W
+00000860: 3f35 5bd2 bf94 8694 5294 8c14 6f72 675f  ?5[.....R...org_
 00000870: 6964 656e 7469 6669 6572 5f6d 6174 6368  identifier_match
-00000880: 9468 1668 2e43 08b7 e868 ff38 29e3 3f94  .h.h.C...h.8).?.
+00000880: 9468 1668 2e43 089d a7fb a273 14e3 3f94  .h.h.C.....s..?.
 00000890: 8694 5294 8c0d 6164 6472 6573 735f 6d61  ..R...address_ma
-000008a0: 7463 6894 6816 682e 4308 1a99 e859 4ed5  tch.h.h.C....YN.
-000008b0: ee3f 9486 9452 948c 0f61 6464 7265 7373  .?...R...address
-000008c0: 5f6e 756d 6265 7273 9468 1668 2e43 08f6  _numbers.h.h.C..
-000008d0: 1868 9f8e 2aaf 3f94 8694 5294 7575 2e    .h..*.?...R.uu.
+000008a0: 7463 6894 6816 682e 4308 f521 e3ae 1852  tch.h.h.C..!...R
+000008b0: ed3f 9486 9452 948c 0f61 6464 7265 7373  .?...R...address
+000008c0: 5f6e 756d 6265 7273 9468 1668 2e43 08f5  _numbers.h.h.C..
+000008d0: 3150 3a3a 40ae 3f94 8694 5294 7575 2e    1P::@.?...R.uu.
```

### Comparing `nomenklatura-2.9.4/nomenklatura/dataset/catalog.py` & `nomenklatura-2.9.5/nomenklatura/dataset/catalog.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/dataset/coverage.py` & `nomenklatura-2.9.5/nomenklatura/dataset/coverage.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/dataset/dataset.py` & `nomenklatura-2.9.5/nomenklatura/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/dataset/publisher.py` & `nomenklatura-2.9.5/nomenklatura/dataset/publisher.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/dataset/resource.py` & `nomenklatura-2.9.5/nomenklatura/dataset/resource.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/dataset/util.py` & `nomenklatura-2.9.5/nomenklatura/dataset/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/db.py` & `nomenklatura-2.9.5/nomenklatura/db.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/enrich/__init__.py` & `nomenklatura-2.9.5/nomenklatura/enrich/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/enrich/aleph.py` & `nomenklatura-2.9.5/nomenklatura/enrich/aleph.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/enrich/common.py` & `nomenklatura-2.9.5/nomenklatura/enrich/common.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/enrich/nominatim.py` & `nomenklatura-2.9.5/nomenklatura/enrich/nominatim.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/enrich/opencorporates.py` & `nomenklatura-2.9.5/nomenklatura/enrich/opencorporates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/enrich/wikidata/__init__.py` & `nomenklatura-2.9.5/nomenklatura/enrich/wikidata/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/enrich/wikidata/lang.py` & `nomenklatura-2.9.5/nomenklatura/enrich/wikidata/lang.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/enrich/wikidata/model.py` & `nomenklatura-2.9.5/nomenklatura/enrich/wikidata/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/enrich/wikidata/props.py` & `nomenklatura-2.9.5/nomenklatura/enrich/wikidata/props.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/enrich/wikidata/qualified.py` & `nomenklatura-2.9.5/nomenklatura/enrich/wikidata/qualified.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/enrich/wikidata/value.py` & `nomenklatura-2.9.5/nomenklatura/enrich/wikidata/value.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/enrich/yente.py` & `nomenklatura-2.9.5/nomenklatura/enrich/yente.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/entity.py` & `nomenklatura-2.9.5/nomenklatura/entity.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/index/entry.py` & `nomenklatura-2.9.5/nomenklatura/index/entry.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 import math
 from typing import Any, Dict, Generator, Tuple, cast
 
+from nomenklatura.resolver import Identifier
+
 
 class Entry(object):
     """A set of entities and a weight associated with a given term in the index."""
 
     __slots__ = "idf", "entities"
 
     def __init__(self) -> None:
         self.idf: float = 0.0
-        self.entities: Dict[str, int] = dict()
+        self.entities: Dict[Identifier, int] = dict()
 
-    def add(self, entity_id: str) -> None:
+    def add(self, entity_id: Identifier) -> None:
         """Mark the given entity as relevant to the entry's token."""
         # This is insane and meant to trade perf for memory:
         try:
             self.entities[entity_id] += 1
         except KeyError:
             self.entities[entity_id] = 1
 
     def compute(self, field: "Field") -> None:
         """Compute weighted term frequency for scoring."""
         self.idf = math.log(field.len / len(self.entities))
 
-    def frequencies(self, field: "Field") -> Generator[Tuple[str, float], None, None]:
+    def frequencies(
+        self, field: "Field"
+    ) -> Generator[Tuple[Identifier, float], None, None]:
         for entity_id, mentions in self.entities.items():
             field_len = max(1, field.entities[entity_id])
             yield entity_id, (mentions / field_len)
 
     def __repr__(self) -> str:
         return "<Entry(%r)>" % len(self.entities)
 
@@ -46,17 +50,17 @@
 
     __slots__ = "len", "avg_len", "tokens", "entities"
 
     def __init__(self) -> None:
         self.len = 0
         self.avg_len = 0.0
         self.tokens: Dict[str, Entry] = {}
-        self.entities: Dict[str, int] = {}
+        self.entities: Dict[Identifier, int] = {}
 
-    def add(self, entity_id: str, token: str) -> None:
+    def add(self, entity_id: Identifier, token: str) -> None:
         if token not in self.tokens:
             self.tokens[token] = Entry()
         self.tokens[token].add(entity_id)
         try:
             self.entities[entity_id] += 1
         except KeyError:
             self.entities[entity_id] = 1
@@ -67,20 +71,22 @@
 
         for entry in self.tokens.values():
             entry.compute(self)
 
     def to_dict(self) -> Dict[str, Any]:
         return {
             "tokens": {t: e.to_dict() for t, e in self.tokens.items()},
-            "entities": self.entities,
+            "entities": {i.id: c for i, c in self.entities.items()},
         }
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "Field":
         obj = cls()
         inverted = data["tokens"].items()
         obj.tokens = {t: Entry.from_dict(i) for t, i in inverted}
-        obj.entities = cast(Dict[str, int], data.get("entities"))
+        # obj.entities = cast(Dict[str, int], data.get("entities"))
+        entities: Dict[str, int] = data.get("entities", {})
+        obj.entities = {Identifier.get(e): c for e, c in entities.items()}
         return obj
 
     def __repr__(self) -> str:
         return "<Field(%d, %.3f)>" % (self.len, self.avg_len)
```

### Comparing `nomenklatura-2.9.4/nomenklatura/index/index.py` & `nomenklatura-2.9.5/nomenklatura/index/index.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,27 +45,28 @@
 
     __slots__ = "loader", "fields", "tokenizer", "entities"
 
     def __init__(self, loader: Loader[DS, CE]):
         self.loader = loader
         self.tokenizer = Tokenizer[DS, CE]()
         self.fields: Dict[str, Field] = {}
-        self.entities: Set[str] = set()
+        self.entities: Set[Identifier] = set()
 
     def index(self, entity: CE, adjacent: bool = True) -> None:
         """Index one entity. This is not idempotent, you need to remove the
         entity before re-indexing it."""
         if not entity.schema.matchable or entity.id is None:
             return
         loader = self.loader if adjacent else None
+        ident = Identifier.get(entity.id)
         for field, token in self.tokenizer.entity(entity, loader=loader):
             if field not in self.fields:
                 self.fields[field] = Field()
-            self.fields[field].add(entity.id, token)
-        self.entities.add(entity.id)
+            self.fields[field].add(ident, token)
+        self.entities.add(ident)
 
     def build(self, adjacent: bool = True) -> None:
         """Index all entities in the dataset."""
         log.info("Building index from: %r...", self.loader)
         self.fields = {}
         self.entities = set()
         for entity in self.loader:
@@ -106,15 +107,15 @@
             except KeyError:
                 continue
             entry = field.tokens.get(token)
             if entry is None or entry.idf is None:
                 continue
             for entity_id, tf in entry.frequencies(field):
                 score = (tf * entry.idf) * self.BOOSTS.get(field_, 1.0)
-                matches[entity_id] += score
+                matches[entity_id.id] += score
 
         results = sorted(matches.items(), key=lambda x: x[1], reverse=True)
         log.debug("Match entity: %r (%d results)", query, len(results))
         returned = 0
         for result_id, score in results:
             if score <= 0.0:
                 break
@@ -162,15 +163,15 @@
                     continue
                 entities = sorted(
                     entry.frequencies(field), key=lambda f: f[1], reverse=True
                 )
                 for (left, lw), (right, rw) in combinations(entities, 2):
                     if lw == 0.0 or rw == 0.0:
                         continue
-                    pair = Identifier.pair(left, right)
+                    pair = (max(left, right), min(left, right))
                     if pair not in pairs:
                         pairs[pair] = 0
                     score = (lw + rw) * boost
                     pairs[pair] += score
 
         return sorted(pairs.items(), key=lambda p: p[1], reverse=True)
 
@@ -194,22 +195,23 @@
         log.debug("Loaded: %r", index)
         return index
 
     def to_dict(self) -> Dict[str, Any]:
         """Prepare an index for pickling."""
         return {
             "fields": {n: f.to_dict() for n, f in self.fields.items()},
-            "entities": self.entities,
+            "entities": [e.id for e in self.entities],
         }
 
     def from_dict(self, state: Dict[str, Any]) -> None:
         """Restore a pickled index."""
         fields = state["fields"].items()
         self.fields = {t: Field.from_dict(i) for t, i in fields}
-        self.entities = set(cast(Set[str], state.get("entities")))
+        entities: List[str] = state.get("entities", [])
+        self.entities = set((Identifier.get(e) for e in entities))
 
     def __len__(self) -> int:
         return len(self.entities)
 
     def __repr__(self) -> str:
         return "<Index(%r, %d, %d)>" % (
             self.loader.dataset.name,
```

### Comparing `nomenklatura-2.9.4/nomenklatura/index/tokenizer.py` & `nomenklatura-2.9.5/nomenklatura/index/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/judgement.py` & `nomenklatura-2.9.5/nomenklatura/judgement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/loader.py` & `nomenklatura-2.9.5/nomenklatura/loader.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/matching/features/__init__.py` & `nomenklatura-2.9.5/nomenklatura/matching/features/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/matching/features/dates.py` & `nomenklatura-2.9.5/nomenklatura/matching/features/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/matching/features/misc.py` & `nomenklatura-2.9.5/nomenklatura/matching/features/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/matching/features/names.py` & `nomenklatura-2.9.5/nomenklatura/matching/features/names.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,33 @@
-import math
 import fingerprints
-from typing import Iterable, Set
+from functools import lru_cache
+from typing import Iterable, Set, Optional
 from followthemoney.types import registry
 
 from nomenklatura.entity import CompositeEntity as Entity
-from nomenklatura.matching.features.util import has_disjoint, has_overlap, has_schema
+from nomenklatura.matching.features.util import has_disjoint, has_overlap
 from nomenklatura.matching.features.util import extract_numbers, compare_sets
 from nomenklatura.matching.features.util import tokenize_pair, props_pair
 from nomenklatura.matching.features.util import type_pair, compare_levenshtein
 
 
+@lru_cache(maxsize=10000)
+def normalize_name(original: str) -> Optional[str]:
+    name = fingerprints.generate(original)
+    if name is None:
+        return None
+    return name[:128]
+
+
 def normalize_names(raws: Iterable[str]) -> Set[str]:
     names = set()
     for raw in raws:
-        name = fingerprints.generate(raw)
-        if name is None:
-            continue
-        names.add(name[:128])
+        name = normalize_name(raw)
+        if name is not None:
+            names.add(name)
     return names
 
 
 def name_levenshtein(left: Entity, right: Entity) -> float:
     """Consider the edit distance (as a fraction of name length) between the two most
     similar names linked to both entities."""
     lv, rv = type_pair(left, right, registry.name)
```

### Comparing `nomenklatura-2.9.4/nomenklatura/matching/features/util.py` & `nomenklatura-2.9.5/nomenklatura/matching/features/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+import math
 import Levenshtein
 from itertools import product
 from normality import slugify
 from functools import lru_cache
 from normality.constants import WS
 from typing import Callable, Iterable, List
 from typing import Optional, Set, Tuple, TypeVar
@@ -54,14 +55,15 @@
     return numbers
 
 
 def compare_levenshtein(left: str, right: str) -> float:
     distance = Levenshtein.distance(left, right)
     base = max((1, len(left), len(right)))
     return 1.0 - (distance / float(base))
+    # return math.sqrt(distance)
 
 
 def props_pair(
     left: Entity, right: Entity, props: List[str]
 ) -> Tuple[Set[str], Set[str]]:
     left_values: Set[str] = set()
     right_values: Set[str] = set()
```

### Comparing `nomenklatura-2.9.4/nomenklatura/matching/model.py` & `nomenklatura-2.9.5/nomenklatura/matching/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/matching/pairs.py` & `nomenklatura-2.9.5/nomenklatura/matching/pairs.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/matching/train.py` & `nomenklatura-2.9.5/nomenklatura/matching/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/publish/dates.py` & `nomenklatura-2.9.5/nomenklatura/publish/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/publish/edges.py` & `nomenklatura-2.9.5/nomenklatura/publish/edges.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/publish/names.py` & `nomenklatura-2.9.5/nomenklatura/publish/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/resolver/edge.py` & `nomenklatura-2.9.5/nomenklatura/resolver/edge.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/resolver/identifier.py` & `nomenklatura-2.9.5/nomenklatura/resolver/identifier.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/resolver/resolver.py` & `nomenklatura-2.9.5/nomenklatura/resolver/resolver.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/senzing.py` & `nomenklatura-2.9.5/nomenklatura/senzing.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/statement/serialize.py` & `nomenklatura-2.9.5/nomenklatura/statement/serialize.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/statement/statement.py` & `nomenklatura-2.9.5/nomenklatura/statement/statement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/tui/app.py` & `nomenklatura-2.9.5/nomenklatura/tui/app.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/tui/comparison.py` & `nomenklatura-2.9.5/nomenklatura/tui/comparison.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/tui/util.py` & `nomenklatura-2.9.5/nomenklatura/tui/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/util.py` & `nomenklatura-2.9.5/nomenklatura/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/nomenklatura/xref.py` & `nomenklatura-2.9.5/nomenklatura/xref.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     loader: Loader[DS, CE],
     resolver: Resolver[CE],
     limit: int = 5000,
     scored: bool = True,
     adjacent: bool = False,
     range: Optional[Schema] = None,
     auto_threshold: Optional[float] = None,
+    focus_dataset: Optional[str] = None,
     user: Optional[str] = None,
 ) -> None:
     log.info("Begin xref: %r, resolver: %s", loader, resolver)
     index = Index(loader)
     index.build(adjacent=adjacent)
     try:
         scores: List[float] = []
@@ -80,24 +81,24 @@
             #         resolver.decide(left_id, right_id, Judgement.POSITIVE)
             #         continue
 
             # Not sure this is globally a good idea.
             if len(left.datasets.intersection(right.datasets)) > 0:
                 score = score * 0.7
 
-            # promote = "us_cia_world_leaders"
-            # if promote in left.datasets and promote not in right.datasets:
-            #     score = (score + 1.0) / 2.0
-            # if promote not in left.datasets and promote in right.datasets:
-            #     score = (score + 1.0) / 2.0
-
             if auto_threshold is not None and score > auto_threshold:
                 log.info("Auto-merge [%.2f]: %s <> %s", score, left, right)
                 resolver.decide(left_id, right_id, Judgement.POSITIVE, user=user)
                 continue
+
+            if focus_dataset in left.datasets and focus_dataset not in right.datasets:
+                score = (score + 1.0) / 2.0
+            if focus_dataset not in left.datasets and focus_dataset in right.datasets:
+                score = (score + 1.0) / 2.0
+
             resolver.suggest(left.id, right.id, score, user=user)
             if suggested > limit:
                 break
             suggested += 1
         _print_stats(idx, suggested, scores)
 
     except KeyboardInterrupt:
```

### Comparing `nomenklatura-2.9.4/nomenklatura.egg-info/PKG-INFO` & `nomenklatura-2.9.5/nomenklatura.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 2.9.4
+Version: 2.9.5
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # nomenklatura
 
 Nomenklatura de-duplicates and integrates different [Follow the Money](https://followthemoney.rtfd.org/) entities. It serves to clean up messy data and to find links between different datasets.
@@ -90,7 +91,9 @@
 ## Contact, contributions etc.
 
 This codebase is licensed under the terms of an MIT license (see LICENSE).
 
 We're keen for any contributions, bug fixes and feature suggestions, please use the GitHub issue tracker for this repository. 
 
 Nomenklatura is currently developed thanks to a Prototypefund grant for [OpenSanctions](https://opensanctions.org). Previous iterations of the package were developed with support from [Knight-Mozilla OpenNews](http://opennews.org) and the [Open Knowledge Foundation Labs](http://okfnlabs.org).
+
+
```

### Comparing `nomenklatura-2.9.4/nomenklatura.egg-info/SOURCES.txt` & `nomenklatura-2.9.5/nomenklatura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.4/setup.py` & `nomenklatura-2.9.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="nomenklatura",
-    version="2.9.4",
+    version="2.9.5",
     description="Make record linkages in followthemoney data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="data mapping identity followthemoney linkage record",
     author="Friedrich Lindenberg",
     author_email="friedrich@pudo.org",
     url="https://github.com/opensanctions/nomenklatura",
@@ -20,16 +20,16 @@
     include_package_data=True,
     package_data={"": ["nomenklatura/data/*", "nomenklatura/py.typed"]},
     zip_safe=False,
     install_requires=[
         "followthemoney >= 3.3.0, < 4.0.0",
         "shortuuid >= 1.0.11, < 2.0.0",
         "rich >= 10.9.0, < 14.0.0",
-        "textual >= 0.19.0, < 0.20.0",
-        "scikit-learn == 1.2.1",
+        "textual >= 0.19.0, < 0.21.0",
+        "scikit-learn == 1.2.2",
         "click >= 8.0.0, < 9.0.0",
     ],
     tests_require=[],
     entry_points={
         "console_scripts": [
             "nk = nomenklatura.cli:cli",
             "nomenklatura = nomenklatura.cli:cli",
```

