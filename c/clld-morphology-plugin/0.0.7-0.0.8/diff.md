# Comparing `tmp/clld_morphology_plugin-0.0.7.tar.gz` & `tmp/clld_morphology_plugin-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clld_morphology_plugin-0.0.7.tar", last modified: Mon Nov  7 03:24:26 2022, max compression
+gzip compressed data, was "dist/clld_morphology_plugin-0.0.8.tar", last modified: Sun Jun 18 05:56:22 2023, max compression
```

## Comparing `clld_morphology_plugin-0.0.7.tar` & `clld_morphology_plugin-0.0.8.tar`

### file list

```diff
@@ -1,55 +1,65 @@
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-07 03:24:26.000000 clld_morphology_plugin-0.0.7/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      424 2022-11-07 03:24:23.000000 clld_morphology_plugin-0.0.7/CITATION.cff
--rw-rw-r--   0 florianm  (1000) florianm  (1000)    11359 2022-04-12 08:24:53.000000 clld_morphology_plugin-0.0.7/LICENSE
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       96 2022-11-06 02:18:58.000000 clld_morphology_plugin-0.0.7/MANIFEST.in
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     2532 2022-11-07 03:24:26.000000 clld_morphology_plugin-0.0.7/PKG-INFO
--rw-r--r--   0 florianm  (1000) florianm  (1000)     1633 2022-06-07 16:08:01.000000 clld_morphology_plugin-0.0.7/README.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      555 2022-07-17 19:35:04.000000 clld_morphology_plugin-0.0.7/pyproject.toml
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1746 2022-11-07 03:24:26.000000 clld_morphology_plugin-0.0.7/setup.cfg
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       92 2022-04-12 08:24:53.000000 clld_morphology_plugin-0.0.7/setup.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-07 03:24:26.000000 clld_morphology_plugin-0.0.7/src/
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-07 03:24:26.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1440 2022-11-07 03:23:28.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/__init__.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-07 03:24:26.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/cldf/
--rw-r--r--   0 florianm  (1000) florianm  (1000)     1344 2022-05-19 19:10:33.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/cldf/FormSlices-metadata.json
--rw-r--r--   0 florianm  (1000) florianm  (1000)      754 2022-06-06 15:00:19.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/cldf/InflectionTable-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      757 2022-07-17 19:35:04.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/cldf/LexemeLexemeParts-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      762 2022-06-07 22:44:43.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/cldf/LexemeMorphemeParts-metadata.json
--rw-r--r--   0 florianm  (1000) florianm  (1000)     1747 2022-06-07 22:42:00.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/cldf/LexemeTable-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     2247 2022-07-17 19:35:04.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/cldf/MorphTable-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1750 2022-07-17 19:35:04.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/cldf/MorphsetTable-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      813 2022-05-31 19:48:56.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/cldf/POSTable-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      830 2022-07-18 14:48:23.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/cldf/__init__.py
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     4803 2022-07-17 20:03:56.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/datatables.py
--rw-r--r--   0 florianm  (1000) florianm  (1000)      436 2022-06-06 17:33:00.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/interfaces.py
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     5977 2022-07-17 19:35:04.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/models.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-07 03:24:26.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/static/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      108 2022-05-28 17:41:45.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/static/clld-morphology.css
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-07 03:24:26.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/templates/
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-07 03:24:26.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/templates/lexeme/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1737 2022-07-17 19:35:04.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/templates/lexeme/detail_html.mako
--rw-r--r--   0 florianm  (1000) florianm  (1000)      245 2022-06-06 03:10:04.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/templates/lexeme/index_html.mako
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-07 03:24:26.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/templates/meaning/
--rw-r--r--   0 florianm  (1000) florianm  (1000)      727 2022-05-10 14:35:49.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/templates/meaning/detail_html.mako
--rw-r--r--   0 florianm  (1000) florianm  (1000)      288 2021-12-26 08:07:46.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/templates/meaning/index_html.mako
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-07 03:24:26.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/templates/morph/
--rw-r--r--   0 florianm  (1000) florianm  (1000)     5322 2022-06-07 23:07:43.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/templates/morph/detail_html.mako
--rw-r--r--   0 florianm  (1000) florianm  (1000)      243 2022-02-23 14:45:24.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/templates/morph/index_html.mako
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-07 03:24:26.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/templates/morpheme/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     5944 2022-07-17 19:35:04.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/templates/morpheme/detail_html.mako
--rw-r--r--   0 florianm  (1000) florianm  (1000)      249 2022-03-13 15:46:33.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/templates/morpheme/index_html.mako
--rw-r--r--   0 florianm  (1000) florianm  (1000)      783 2022-05-10 14:17:26.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/templates/morphology_util.mako
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-07 03:24:26.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/templates/pos/
--rw-r--r--   0 florianm  (1000) florianm  (1000)      488 2022-05-31 20:59:49.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/templates/pos/detail_html.mako
--rw-r--r--   0 florianm  (1000) florianm  (1000)      249 2022-05-31 20:53:58.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/templates/pos/index_html.mako
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-07 03:24:26.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/templates/wordform/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     2963 2022-11-06 23:35:11.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/templates/wordform/detail_html.mako
--rw-r--r--   0 florianm  (1000) florianm  (1000)      245 2022-04-25 06:19:12.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/templates/wordform/index_html.mako
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     4677 2022-11-07 02:47:47.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/util.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-07 03:24:26.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin.egg-info/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     2532 2022-11-07 03:24:26.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin.egg-info/PKG-INFO
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1930 2022-11-07 03:24:26.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin.egg-info/SOURCES.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2022-11-07 03:24:26.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin.egg-info/dependency_links.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2022-11-07 03:24:26.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin.egg-info/not-zip-safe
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      224 2022-11-07 03:24:26.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin.egg-info/requires.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       23 2022-11-07 03:24:26.000000 clld_morphology_plugin-0.0.7/src/clld_morphology_plugin.egg-info/top_level.txt
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      424 2023-06-18 05:56:14.000000 clld_morphology_plugin-0.0.8/CITATION.cff
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)    11359 2022-04-12 08:24:53.000000 clld_morphology_plugin-0.0.8/LICENSE
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       96 2022-11-06 02:18:58.000000 clld_morphology_plugin-0.0.8/MANIFEST.in
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     5520 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/PKG-INFO
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     4621 2023-02-27 21:55:48.000000 clld_morphology_plugin-0.0.8/README.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      555 2022-07-17 19:35:04.000000 clld_morphology_plugin-0.0.8/pyproject.toml
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1746 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/setup.cfg
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       92 2022-04-12 08:24:53.000000 clld_morphology_plugin-0.0.8/setup.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     3168 2023-06-18 05:55:06.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/__init__.py
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     8511 2023-03-26 15:39:42.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/datatables.py
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      942 2023-02-23 22:32:53.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/interfaces.py
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)    22443 2023-03-26 15:39:42.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/models.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/static/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      108 2022-05-28 17:41:45.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/static/clld-morphology.css
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/derivationalprocess/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1332 2023-03-26 16:41:39.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/derivationalprocess/detail_html.mako
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      258 2023-02-23 00:42:28.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/derivationalprocess/index_html.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/form/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     3400 2023-03-07 22:54:59.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/form/detail_html.mako
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      241 2023-02-23 00:42:28.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/form/index_html.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/gloss/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     2725 2023-03-26 15:38:27.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/gloss/detail_html.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/inflectionalcategory/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      580 2023-03-26 15:36:33.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/inflectionalcategory/detail_html.mako
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      317 2023-03-07 06:12:04.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/inflectionalcategory/index_html.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/inflectionalvalue/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1894 2023-03-07 22:55:28.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/inflectionalvalue/detail_html.mako
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      309 2023-02-23 00:42:28.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/inflectionalvalue/index_html.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/lexeme/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     2719 2023-03-07 22:55:32.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/lexeme/detail_html.mako
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      245 2022-06-06 03:10:04.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/lexeme/index_html.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/meaning/
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      790 2023-03-07 22:55:44.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/meaning/detail_html.mako
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      288 2021-12-26 08:07:46.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/meaning/index_html.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/morph/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     6615 2023-03-07 22:53:56.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/morph/detail_html.mako
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      243 2022-02-23 14:45:24.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/morph/index_html.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/morpheme/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     5737 2023-03-07 22:55:37.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/morpheme/detail_html.mako
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      249 2022-03-13 15:46:33.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/morpheme/index_html.mako
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      783 2022-05-10 14:17:26.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/morphology_util.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/morphophonologicalchange/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      625 2023-03-07 22:55:16.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/morphophonologicalchange/detail_html.mako
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      345 2023-02-23 22:42:05.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/morphophonologicalchange/index_html.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/pos/
+-rw-r--r--   0 florianm  (1000) florianm  (1000)     1172 2023-03-07 22:55:10.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/pos/detail_html.mako
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      249 2022-05-31 20:53:58.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/pos/index_html.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/stem/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     2128 2023-06-14 22:03:57.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/stem/detail_html.mako
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      241 2023-02-23 00:42:28.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/stem/index_html.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/wordform/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     6266 2023-03-07 22:54:21.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/wordform/detail_html.mako
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      249 2023-02-23 00:42:28.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/wordform/index_html.mako
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)    13923 2023-06-09 23:08:57.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/util.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin.egg-info/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     5520 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin.egg-info/PKG-INFO
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     2297 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin.egg-info/SOURCES.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin.egg-info/dependency_links.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin.egg-info/not-zip-safe
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      224 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin.egg-info/requires.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       23 2023-06-18 05:56:22.000000 clld_morphology_plugin-0.0.8/src/clld_morphology_plugin.egg-info/top_level.txt
```

### Comparing `clld_morphology_plugin-0.0.7/LICENSE` & `clld_morphology_plugin-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `clld_morphology_plugin-0.0.7/pyproject.toml` & `clld_morphology_plugin-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `clld_morphology_plugin-0.0.7/setup.cfg` & `clld_morphology_plugin-0.0.8/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 	pylons
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = clld_morphology_plugin
 project_urls = 
 	Bug Tracker = https://github.com/fmatter/clld-morphology-plugin/issues
 url = https://github.com/fmatter/clld-morphology-plugin
-version = 0.0.7
+version = 0.0.8
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 package_dir = 
 	=src
```

### Comparing `clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/datatables.py` & `clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/datatables.py`

 * *Files 27% similar despite different names*

```diff
@@ -43,74 +43,123 @@
         if qs == "yes":
             return models.Wordform_files.pk != 0
         return True
 
 
 class Wordforms(DataTable):
 
-    __constraints__ = [Language, models.POS, models.Lexeme, models.Inflection]
+    __constraints__ = [
+        Language,
+        models.Lexeme,
+        models.Morph,
+        models.POS,
+        models.Inflection,
+        models.Stem,
+    ]
 
     def base_query(self, query):
         query = query.join(Language).options(joinedload(models.Wordform.language))
 
         query = query.outerjoin(
             models.Wordform_files,
             and_(
                 models.Wordform_files.object_pk == models.Wordform.pk,
                 models.Wordform_files.mime_type.contains("audio/"),
             ),
         ).options(
             joinedload(models.Wordform._files)  # pylint: disable=protected-access
         )
 
+        if self.morph:
+            query = query.join(models.WordformPart).options(
+                joinedload(models.Wordform.slices)
+            )
+            return query.filter(
+                models.Wordform.slices.any(models.WordformPart.morph == self.morph)
+            )
         if self.language:
             return query.filter(models.Wordform.language == self.language)
+        if self.stem:
+            return query.filter(
+                models.Wordform.formstems.any(models.WordformStem.stem == self.stem)
+            )
         if self.pos:
-            query = query.join(models.POS).options(joinedload(models.Wordform.pos))
             return query.filter(models.Wordform.pos == self.pos)
         if self.lexeme:
-            query = query.join(models.Inflection, models.Lexeme).options(
-                joinedload(models.Wordform.lexemes)
-            )
-            return query.filter(models.Inflection.lexeme == self.lexeme)
+            return query.filter(models.Wordform.lexeme == self.lexeme)
         return query
 
     def col_defs(self):
         cols = [LinkCol(self, "name"), Col(self, "description")]
         if not self.pos:
             cols.append(
                 LinkCol(
                     self,
                     "part of speech",
                     model_col=models.POS.name,
                     get_obj=lambda i: i.pos,
                 )
             )
-        if not self.language and not self.lexeme:
+        if not self.language:
             cols.append(
                 LinkCol(
                     self,
                     "language",
                     model_col=Language.name,
                     get_obj=lambda i: i.language,
                 )
             )
-        if not self.lexeme:
+        cols.append(AudioCol(self, "Audio"))
+        return cols
+
+
+class Wordforms_noPOS(Wordforms):
+    def col_defs(self):
+        cols = [LinkCol(self, "name"), Col(self, "description")]
+        if not self.language:
             cols.append(
                 LinkCol(
                     self,
-                    "lexeme",
-                    model_col=models.Lexeme.name,
-                    get_obj=lambda i: i.lexeme,
+                    "language",
+                    model_col=Language.name,
+                    get_obj=lambda i: i.language,
                 )
             )
         cols.append(AudioCol(self, "Audio"))
         return cols
 
 
+class Forms(DataTable):
+
+    __constraints__ = [Language, models.Wordform]
+
+    def base_query(self, query):
+        query = query.join(Language).options(joinedload(models.Form.language))
+
+        if self.language:
+            return query.filter(models.Form.language == self.language)
+        if self.wordform:
+            query = query.join(models.FormPart).options(
+                joinedload(models.Form.formslices)
+            )
+            return query.filter(
+                models.Form.formslices.any(models.FormPart.wordform == self.wordform)
+            )
+        return query
+
+    def col_defs(self):
+        return [
+            LinkCol(self, "name"),
+            Col(self, "description"),
+            LinkCol(
+                self, "language", model_col=Language.name, get_obj=lambda i: i.language
+            ),
+        ]
+
+
 class Morphs(DataTable):
 
     __constraints__ = [Language]
 
     def base_query(self, query):
         query = query.join(Language).options(joinedload(models.Morph.language))
 
@@ -121,14 +170,15 @@
     def col_defs(self):
         return [
             LinkCol(self, "name"),
             Col(self, "description"),
             LinkCol(
                 self, "language", model_col=Language.name, get_obj=lambda i: i.language
             ),
+            Col(self, "morph_type", choices=["prefix", "suffix", "root", "infix"]),
         ]
 
 
 class Morphemes(DataTable):
     __constraints__ = [Language]
 
     def base_query(self, query):
@@ -144,26 +194,111 @@
             Col(self, "description"),
             LinkCol(
                 self, "language", model_col=Language.name, get_obj=lambda i: i.language
             ),
         ]
 
 
+class Stems(DataTable):
+    __constraints__ = [Language, models.Morph]
+
+    def base_query(self, query):
+        query = query.join(Language).options(joinedload(models.Stem.language))
+        query = query.join(models.StemPart).options(joinedload(models.Stem.slices))
+
+        if self.language:
+            return query.filter(models.Stem.language == self.language)
+        if self.morph:
+            return query.filter(
+                models.Stem.slices.any(models.StemPart.morph == self.morph)
+            )
+        return query
+
+    def col_defs(self):
+        return [
+            LinkCol(self, "name"),
+            Col(self, "description"),
+            LinkCol(
+                self, "language", model_col=Language.name, get_obj=lambda i: i.language
+            ),
+        ]
+
+
 class Meanings(DataTable):
     def col_defs(self):
         return [LinkCol(self, "name")]
 
 
+class DerivationalProcesses(DataTable):
+    def col_defs(self):
+        return [LinkCol(self, "name")]
+
+
 class POS(DataTable):
     def col_defs(self):
+        return [LinkCol(self, "name"), Col(self, "description")]
+
+
+class InflectionalCategories(DataTable):
+    def col_defs(self):
+        return [LinkCol(self, "name"), Col(self, "description")]
+
+
+class InflectionalValues(DataTable):
+    def col_defs(self):
+        return [LinkCol(self, "name")]
+
+
+class Glosses(DataTable):
+    def col_defs(self):
         return [LinkCol(self, "name")]
 
 
 class Lexemes(DataTable):
+    __constraints__ = [Language, models.POS]
+
+    def base_query(self, query):
+        if self.pos:
+            return query.filter(models.Lexeme.pos == self.pos)
+        return query
+
+    def col_defs(self):
+        cols = [
+            LinkCol(self, "name"),
+            Col(self, "description"),
+            # FormCountCol(self, "Forms", bSortable=False, bSearchable=False),
+        ]
+        if not self.pos:
+            cols.append(
+                LinkCol(
+                    self,
+                    "part of speech",
+                    # model_col=models.POS.name,
+                    get_obj=lambda i: i.pos,
+                )
+            )
+        return cols
+
+
+class MorphoPhonoChanges(DataTable):
+
     __constraints__ = [Language]
 
+    def base_query(self, query):
+        query = query.join(Language).options(
+            joinedload(models.MorphoPhonologicalChange.language)
+        )
+
+        if self.language:
+            return query.filter(
+                models.MorphoPhonologicalChange.language == self.language
+            )
+        return query
+
     def col_defs(self):
         return [
             LinkCol(self, "name"),
             Col(self, "description"),
-            FormCountCol(self, "Forms", bSortable=False, bSearchable=False),
+            LinkCol(
+                self, "language", model_col=Language.name, get_obj=lambda i: i.language
+            ),
         ]
```

### Comparing `clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/templates/meaning/detail_html.mako` & `clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/meaning/detail_html.mako`

 * *Files 22% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     <ol>
         % for form in ctx.forms:
             <li>${h.link(request, form.form)}</li>
     % endfor
     </ol>
 %endif
 
+<p>${h.text2html(h.Markup(ctx.markup_description or ""))}</p>
+
 % if ctx.morphemes:
     <h3>${_('Morphemes')}</h3>
     <ol>
         % for m in ctx.morphemes:
             <li>${h.link(request, m.morpheme)}</li>
         % endfor
     </ol>
```

### Comparing `clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/templates/morph/detail_html.mako` & `clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/morpheme/detail_html.mako`

 * *Files 22% similar despite different names*

```diff
@@ -1,135 +1,148 @@
 <%inherit file="../${context.get('request').registry.settings.get('clld.app_template', 'app.mako')}"/>
 <%namespace name="util" file="../util.mako"/>
-<link rel="stylesheet" href="${req.static_url('clld_morphology_plugin:static/clld-morphology.css')}"/>
+<%namespace name="mutil" file="../morphology_util.mako"/>
 
+<link rel="stylesheet" href="${req.static_url('clld_morphology_plugin:static/clld-morphology.css')}"/>
 % try:
     <%from clld_corpus_plugin.util import rendered_sentence%>
 % except:
     <% rendered_sentence = h.rendered_sentence %>
 % endtry 
-<%! active_menu_item = "morphs" %>
 
+<%! active_menu_item = "morphemes" %>
 
-<%doc><h2>${_('Morph')} ${ctx.name} (${h.link(request, ctx.language)})</h2>
-</%doc>
-
-<h3>${_('Morph')} <i>${ctx.name}</i></h3>
+<h3>${_('Morpheme')} <i>${ctx.name}</i> ‘${ctx.description}’</h3>
 
 <table class="table table-nonfluid">
     <tbody>
         <tr>
             <td>Language:</td>
             <td>${h.link(request, ctx.language)}</td>
         </tr>
         <tr>
-            <td> Morpheme:</td>
-            <td>${h.link(request, ctx.morpheme)}</td>
-        </tr>
-        <tr>
-            <td> Meanings:</td>
-            <td>
-                <ol>
-                    % for meaning in ctx.morpheme.meanings:
-                        <li> ‘${h.link(request, meaning.meaning)}’ </li>
-                    % endfor
-                </ol>
-            </td>
-        </tr>
-        % if cognates in dir(ctx):
-        <tr>
-            <td>Cognate set(s):</td>
-            <td>
-              <%
-                cogsets = []
-              %>
-                    % for c in ctx.cognates:
-                        % if c.cognateset not in cogsets:
-                            <%
-                                cogsets.append(c.cognateset)
-                            %>
+            % if ctx.allomorphs:
+                <td> Morphs: </td>
+                <td>
+                    % for i, morph in enumerate(ctx.allomorphs):
+                        % if i < len(ctx.allomorphs)-1:
+                            <% comma = "," %>
+                        % else:
+                            <% comma = "" %>
                         % endif
+                    <i>${h.link(request, morph)}</i>${comma}
                     % endfor
-                    ${h.text2html("*"+"+".join([h.link(request, c) for c in cogsets]))}
-            </td>
-            % for c in ctx.cognates:
-                ${type(c.cognateset)}
-            % endfor
-        </tr>
-        % endif
-        % if contribution in dir(ctx):
-        <tr>
-            <td> Contribution:</td>
-            <td>
-                ${h.link(request, ctx.contribution)} by
-% for contributor in ctx.contribution.primary_contributors:
-${h.link(request, contributor)}
-% endfor
-            </td>
+                </td>
+            %endif
         </tr>
+        % if ctx.glosses:
+            <tr>
+                <td>Glosses:</td>
+                <td>
+                    ${h.text2html(", ".join([".".join([h.link(request, gloss) for gloss in glosslist]) for glosslist in ctx.glosses]))}
+                </td>
+            </tr>
+        %endif
+        % if ctx.inflectionalvalues:
+            <tr>
+                <td> Inflectional values:</td>
+                <td>
+                <ul>
+                  % for val in ctx.inflectionalvalues:
+                     <li>${h.link(request, val, label=val.name)} (${h.link(request, val.category)})</li>
+                  % endfor
+                </ul>
+                </td>
+            </tr>
         % endif
     </tbody>
 </table>
 
+<p>${h.text2html(h.Markup(ctx.markup_description or ""))}</p>
+
 <% meaning_forms = {} %>
-<% meaning_sentences = {} %>
-    % for form_slice in ctx.forms:
-        % if not form_slice.morpheme_meaning:
-            <li> ${h.link(request, form_slice.form)} </li>
-        % else:
-            <% meaning_forms.setdefault(form_slice.morpheme_meaning, []) %>
-            <% meaning_forms[form_slice.morpheme_meaning].append(form_slice.form) %>
-            % if getattr(form_slice.form_meaning, "form_tokens", None):
-                <% meaning_sentences.setdefault(form_slice.morpheme_meaning, []) %>
-                <% meaning_sentences[form_slice.morpheme_meaning].extend(form_slice.form_meaning.form_tokens) %>
-            % endif
+<% gloss_sentences = {} %>
+
+% for fslice in ctx.formslices:
+    % if hasattr(fslice.form, "sentence_assocs") and fslice.form.sentence_assocs:
+        <% gloss = ".".join([str(x.gloss) for x in fslice.glosses]) %>
+        <% gloss_sentences.setdefault(gloss, []) %>
+        % for s in fslice.form.sentence_assocs:
+            <% gloss_sentences[gloss].append(s.sentence) %>
+        % endfor
+    % endif
+% endfor
+
+% for sslice in ctx.stemslices:
+    % for wf in sslice.stem.wordforms:
+        % if hasattr(wf, "sentence_assocs") and wf.sentence_assocs:
+            <% gloss = ".".join([str(x.gloss) for x in sslice.glosses]) %>
+            <% gloss_sentences.setdefault(gloss, []) %>
+            % for s in wf.sentence_assocs:
+                <% gloss_sentences[gloss].append(s.sentence) %>
+            % endfor
         % endif
+    % endfor
 % endfor
 
 <div class="tabbable">
     <ul class="nav nav-tabs">
-        <li class="active"><a href="#corpus" data-toggle="tab"> Corpus tokens </a></li>
-        <li><a href="#forms" data-toggle="tab"> Wordforms </a></li>
+        % if gloss_sentences:
+            <li class=${'active' if gloss_sentences else ''}><a href="#corpus" data-toggle="tab"> Corpus tokens </a></li>
+        % endif
+        % if ctx.formslices:
+            <li class=${'' if gloss_sentences else 'active'}><a href="#forms" data-toggle="tab"> Wordforms </a></li>
+        % endif
+        % if ctx.stemslices:
+            <li class=${'' if gloss_sentences or ctx.formslices else 'active'}><a href="#stems" data-toggle="tab"> Stems </a></li>
+        % endif
     </ul>
 
     <div class="tab-content" style="overflow: visible;">
-        <div id="forms" class="tab-pane">
-            % for meaning, forms in meaning_forms.items():
-                % if len(meaning_forms) > 1:
-                    <h5> As ‘${h.link(request, meaning.meaning)}’: </h5>
-                % endif
-                <ol>
-                    % for form in forms:
-                        <li> ${h.link(request, form)} ${"("+form.pos.id+")" if form.pos else ""} </li>
-                    % endfor
-                </ol>
-            % endfor
+
+        <div id="forms" class="tab-pane ${'' if gloss_sentences else 'active'}">
+            <ul>
+                % for fslice in ctx.formslices:
+                    <li> ${h.link(request, fslice.form)} </li>
+                % endfor
+            </ul>
         </div>
-    
-        <div id="corpus" class="tab-pane active">
-            % for morpheme_meaning, sentences in meaning_sentences.items():
-                <div id=${morpheme_meaning.id}>
-                    % if len(meaning_forms) > 1:
-                        <h5> As ‘${h.link(request, morpheme_meaning.meaning)}’:</h5>
+
+        <div id="stems" class="tab-pane ${'' if gloss_sentences or ctx.formslices else 'active'}">
+            <ul>
+                % for sslice in ctx.stemslices:
+                    <li> ${h.link(request, sslice.stem)} </li>
+                % endfor
+            </ul>
+        </div>
+
+        <div id="corpus" class="tab-pane ${'active' if gloss_sentences else ''}">
+            % for gloss, sentences in gloss_sentences.items():
+                <div id=${gloss}>
+                    % if len(sentences) > 1:
+                        <h5> As ‘${gloss}’:</h5>
                     % endif
-                    <button type="button" class="btn btn-link" onclick="copyIDs('${morpheme_meaning.id}-ids')">Copy sentence IDs</button>
-                    <code class="id_list" id=${morpheme_meaning.id}-ids> ${" ".join([x.sentence.id for x in sentences])} </code>
+                    ## <button type="button" class="btn btn-outline-info" onclick="copyIDs('${gloss}-ids')">Copy sentence IDs</button>
                     <% stc_ids = [] %>
                     <ol class="example">
                         % for sentence in sentences:
-                            % if sentence.sentence.id not in stc_ids:
-                                ${rendered_sentence(request, sentence.sentence, sentence_link=True)}
-                                <% stc_ids.append(sentence.sentence.id) %>
+                            % if sentence.id not in stc_ids:
+                                ${rendered_sentence(request, sentence, sentence_link=True)}
+                                <% stc_ids.append(sentence.id) %>
                             % endif
                         % endfor
                     </ol>
                 </div>
                 <script>
-                    var highlight_div = document.getElementById("${morpheme_meaning.id}");
-                    var highlight_targets = highlight_div.querySelectorAll("*[name='${ctx.id}-${morpheme_meaning.id}']")
+                    var highlight_div = document.getElementById("${gloss}");
+                    var highlight_targets = [];
+                    % for x in ctx.allomorphs:
+                        highlight_targets.push(...highlight_div.querySelectorAll("*[name='${x.id}']"))
+                    % endfor
+                    console.log(highlight_targets)
                     for (index = 0; index < highlight_targets.length; index++) {
                         highlight_targets[index].classList.add("morpho-highlight");
                     }
                 </script>
             % endfor
         </div>
     </div>
```

#### html2text {}

```diff
@@ -1,48 +1,50 @@
 <%inherit file="../${context.get('request').registry.settings.get
 ('clld.app_template', 'app.mako')}"/> <%namespace name="util" file="../
-util.mako"/>
+util.mako"/> <%namespace name="mutil" file="../morphology_util.mako"/>
  % try: <%from clld_corpus_plugin.util import rendered_sentence%> % except: <%
 rendered_sentence = h.rendered_sentence %> % endtry <%! active_menu_item =
-"morphs" %> <%doc>
-***** ${_('Morph')} ${ctx.name} (${h.link(request, ctx.language)}) *****
-doc>
-**** ${_('Morph')} ${ctx.name} ****
-Language:       ${h.link(request, ctx.language)}
-Morpheme:       ${h.link(request, ctx.morpheme)}
-                   1. % for meaning in ctx.morpheme.meanings:
-Meanings:          2. â${h.link(request, meaning.meaning)}â
-                   3. % endfor
-                <% cogsets = [] %> % for c in ctx.cognates: % if c.cognateset
-Cognate set(s): not in cogsets: <% cogsets.append(c.cognateset) %> % endif %
-                endfor ${h.text2html("*"+"+".join([h.link(request, c) for c in
-                cogsets]))}
-                ${h.link(request, ctx.contribution)} by % for contributor in
-Contribution:   ctx.contribution.primary_contributors: ${h.link(request,
-                contributor)} % endfor
-<% meaning_forms = {} %> <% meaning_sentences = {} %> % for form_slice in
-ctx.forms: % if not form_slice.morpheme_meaning:
-${h.link(request, form_slice.form)}
-% else: <% meaning_forms.setdefault(form_slice.morpheme_meaning, []) %> <%
-meaning_forms[form_slice.morpheme_meaning].append(form_slice.form) %> % if
-getattr(form_slice.form_meaning, "form_tokens", None): <%
-meaning_sentences.setdefault(form_slice.morpheme_meaning, []) %> <%
-meaning_sentences[form_slice.morpheme_meaning].extend
-(form_slice.form_meaning.form_tokens) %> % endif % endif % endfor
-    * Corpus_tokens
-    * Wordforms
-% for meaning, forms in meaning_forms.items(): % if len(meaning_forms) > 1:
-** As â${h.link(request, meaning.meaning)}â: **
+"morphemes" %>
+**** ${_('Morpheme')} ${ctx.name} â${ctx.description}â ****
+Language:            ${h.link(request, ctx.language)}
+                     % for i, morph in enumerate(ctx.allomorphs): % if i < len
+Morphs:              (ctx.allomorphs)-1: <% comma = "," %> % else: <% comma =
+                     "" %> % endif ${h.link(request, morph)}${comma} % endfor
+Glosses:             ${h.text2html(", ".join([".".join([h.link(request, gloss)
+                     for gloss in glosslist]) for glosslist in ctx.glosses]))}
+                         * % for val in ctx.inflectionalvalues:
+Inflectional values:     * ${h.link(request, val, label=val.name)} (${h.link
+                           (request, val.category)})
+                         * % endfor
+${h.text2html(h.Markup(ctx.markup_description or ""))}
+<% meaning_forms = {} %> <% gloss_sentences = {} %> % for fslice in
+ctx.formslices: % if hasattr(fslice.form, "sentence_assocs") and
+fslice.form.sentence_assocs: <% gloss = ".".join([str(x.gloss) for x in
+fslice.glosses]) %> <% gloss_sentences.setdefault(gloss, []) %> % for s in
+fslice.form.sentence_assocs: <% gloss_sentences[gloss].append(s.sentence) %> %
+endfor % endif % endfor % for sslice in ctx.stemslices: % for wf in
+sslice.stem.wordforms: % if hasattr(wf, "sentence_assocs") and
+wf.sentence_assocs: <% gloss = ".".join([str(x.gloss) for x in sslice.glosses])
+%> <% gloss_sentences.setdefault(gloss, []) %> % for s in wf.sentence_assocs:
+<% gloss_sentences[gloss].append(s.sentence) %> % endfor % endif % endfor %
+endfor
+    * % if gloss_sentences:
+    * '}>Corpus_tokens
+% endif % if ctx.formslices:
+active'}>Wordforms
+% endif % if ctx.stemslices:
+formslices else 'active'}>Stems
 % endif
-   1. % for form in forms:
-   2. ${h.link(request, form)} ${"("+form.pos.id+")" if form.pos else ""}
-   3. % endfor
-% endfor
-% for morpheme_meaning, sentences in meaning_sentences.items():
-% if len(meaning_forms) > 1:
-** As â${h.link(request, morpheme_meaning.meaning)}â: **
-% endif Copy sentence IDs ${" ".join([x.sentence.id for x in sentences])} <%
-stc_ids = [] %>
-   1. % for sentence in sentences: % if sentence.sentence.id not in stc_ids: $
-      {rendered_sentence(request, sentence.sentence, sentence_link=True)} <%
-      stc_ids.append(sentence.sentence.id) %> % endif % endfor
+    * % for fslice in ctx.formslices:
+    * ${h.link(request, fslice.form)}
+    * % endfor
+    * % for sslice in ctx.stemslices:
+    * ${h.link(request, sslice.stem)}
+    * % endfor
+% for gloss, sentences in gloss_sentences.items():
+% if len(sentences) > 1:
+** As â${gloss}â: **
+% endif ## Copy sentence IDs <% stc_ids = [] %>
+   1. % for sentence in sentences: % if sentence.id not in stc_ids: $
+      {rendered_sentence(request, sentence, sentence_link=True)} <%
+      stc_ids.append(sentence.id) %> % endif % endfor
  % endfor
```

### Comparing `clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/templates/morphology_util.mako` & `clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/morphology_util.mako`

 * *Files identical despite different names*

### Comparing `clld_morphology_plugin-0.0.7/src/clld_morphology_plugin/templates/wordform/detail_html.mako` & `clld_morphology_plugin-0.0.8/src/clld_morphology_plugin/templates/inflectionalvalue/detail_html.mako`

 * *Files 19% similar despite different names*

```diff
@@ -1,99 +1,55 @@
 <%inherit file="../${context.get('request').registry.settings.get('clld.app_template', 'app.mako')}"/>
 <%namespace name="util" file="../util.mako"/>
-<% from clld_morphology_plugin.util import rendered_form %>
 <link rel="stylesheet" href="${req.static_url('clld_morphology_plugin:static/clld-morphology.css')}"/>
-% try:
-    <%from clld_corpus_plugin.util import rendered_sentence%>
-% except:
-    <% rendered_sentence = h.rendered_sentence %>
-% endtry
-<%! active_menu_item = "wordforms" %>
 
+<%! active_menu_item = "inflectionalvalues" %>
 
-
-<h3>${_('Form')} <i>${ctx.name}</i></h3>
+<h3>${_('Inflectional value')} '${ctx.name}'</h3>
 
 <table class="table table-nonfluid">
     <tbody>
-<%doc>        <tr>
-            <td>Form:</td>
-            <td>${ctx.name}</td>
-        </tr></%doc>
-        % if ctx.morphs:
-        <tr>
-            <td>Structure:</td>
-            <td>
-                    ${rendered_form(request, ctx)}
-            </td>
-        </tr>
-        % endif
-        <tr>
-            <td> Meanings:</td>
-            <td>
-                <ol>
-                    % for meaning in ctx.meanings:
-                        <li> ‘${h.link(request, meaning.meaning)}’ </li>
-                    % endfor
-                </ol>
-            </td>
-        </tr>
-        % if ctx.pos:
-        <tr>
-            <td>Part of speech:</td>
-            <td>
-                ${h.link(request, ctx.pos)}
-            </td>
-        </tr>
-        % endif
-        % if ctx.lexeme:
-        <tr>
-            <td>Lexeme:</td>
-            <td>${h.link(request, ctx.lexeme, label=ctx.lexeme.name.upper())}</td>
-        </tr>
-        % endif
-        % if getattr(ctx, "segments", None):
-            <tr>
-                <td>Segments:</td>
-                <td>
-                % for segment in ctx.segments:
-                ${h.link(request, segment.phoneme)}
-                    % endfor</td>
-            </tr>
-        % endif
+    <tr>
+        <td>Category:</td>
+        <td>${h.link(request, ctx.category)}</td>
+    </tr>
+    % if ctx.gloss:
         <tr>
-            <td>Language:</td>
-            <td>${h.link(request, ctx.language)}</td>
+            <td>Gloss:</td>
+            <td>${h.link(request, ctx.gloss)}</td>
         </tr>
-        % if ctx.source:
-            <tr>
-                <td>Source:</td>
-                <td>${h.link(request, ctx.source)}</td>
-            </tr>
-        % endif
-    </tbody>
-</table>
-
-% if ctx.audio:
-    <audio controls="controls"><source src="/audio/${ctx.audio}" type="audio/x-wav"></source></audio>
-% endif 
-
-% if len(ctx.meanings) > 0:
-    % if getattr(ctx.meanings[0], "form_tokens", None):
-        <h3>${_('Sentences')}</h3>
-        % for form_meaning in ctx.meanings:
-            <h4>‘${h.link(request, form_meaning.meaning)}’:</h4>
-            <ol class="example">
-                % for form_token in form_meaning.form_tokens:
-                    ${rendered_sentence(request, form_token.sentence,       sentence_link=True)}
+    % endif
+    % if ctx.exponents:
+    <td> Exponents: </td>
+    <td>
+        <ul>
+            % for morphs, forms in ctx.exponents.items():
+                <% morph_list = [] %>
+                <% label = [] %>
+                % for morph in morphs:
+                    % if morph:
+                        <% morph_list.append(h.link(request, morph)) %>
+                        <% label.append(morph.id) %>
+                    % else:
+                        <% morph_list.append("zero-marked") %>
+                        <% label.append("zero") %>                      
+                    % endif
                 % endfor
-            </ol>
-        % endfor
+                <% label = ",".join(label) %>
+                <li>
+                    ${", ".join(morph_list) |n} (<a data-toggle="collapse" data-target="#${label}">🞃 forms</a>)
+                </li>
+                    <div id="${label}" class="collapse out">
+                        <ul>
+                            % for form in forms:
+                                <li>${h.link(request, form)}</li>
+                            % endfor
+                        </ul>
+                    </div>
+            % endfor
+        </ul>
+    </td>
     % endif
-% endif
+    </tbody>
+</table>
 
-<script>
-var highlight_targets = document.getElementsByName("${ctx.id}");
-for (index = 0; index < highlight_targets.length; index++) {
-    highlight_targets[index].children[0].classList.add("morpho-highlight");
-}
-</script>
+<p>${h.text2html(h.Markup(ctx.markup_description or ""))}</p>
```

#### html2text {}

```diff
@@ -1,26 +1,8 @@
 <%inherit file="../${context.get('request').registry.settings.get
 ('clld.app_template', 'app.mako')}"/> <%namespace name="util" file="../
-util.mako"/> <% from clld_morphology_plugin.util import rendered_form %>
- % try: <%from clld_corpus_plugin.util import rendered_sentence%> % except: <%
-rendered_sentence = h.rendered_sentence %> % endtry <%! active_menu_item =
-"wordforms" %>
-**** ${_('Form')} ${ctx.name} ****
-Form:           ${ctx.name}
-Structure:      ${rendered_form(request, ctx)}
-                   1. % for meaning in ctx.meanings:
-Meanings:          2. â${h.link(request, meaning.meaning)}â
-                   3. % endfor
-Part of speech: ${h.link(request, ctx.pos)}
-Lexeme:         ${h.link(request, ctx.lexeme, label=ctx.lexeme.name.upper())}
-Segments:       % for segment in ctx.segments: ${h.link(request,
-                segment.phoneme)} % endfor
-Language:       ${h.link(request, ctx.language)}
-Source:         ${h.link(request, ctx.source)}
-% if ctx.audio:  % endif % if len(ctx.meanings) > 0: % if getattr(ctx.meanings
-[0], "form_tokens", None):
-**** ${_('Sentences')} ****
-% for form_meaning in ctx.meanings:
-*** â${h.link(request, form_meaning.meaning)}â: ***
-   1. % for form_token in form_meaning.form_tokens: ${rendered_sentence
-      (request, form_token.sentence, sentence_link=True)} % endfor
-% endfor % endif % endif
+util.mako"/>
+ <%! active_menu_item = "inflectionalvalues" %>
+**** ${_('Inflectional value')} '${ctx.name}' ****
+Category: ${h.link(request, ctx.category)}
+Gloss:    ${h.link(request, ctx.gloss)}
+${h.text2html(h.Markup(ctx.markup_description or ""))}
```

### Comparing `clld_morphology_plugin-0.0.7/src/clld_morphology_plugin.egg-info/SOURCES.txt` & `clld_morphology_plugin-0.0.8/src/clld_morphology_plugin.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -12,30 +12,34 @@
 src/clld_morphology_plugin/util.py
 src/clld_morphology_plugin.egg-info/PKG-INFO
 src/clld_morphology_plugin.egg-info/SOURCES.txt
 src/clld_morphology_plugin.egg-info/dependency_links.txt
 src/clld_morphology_plugin.egg-info/not-zip-safe
 src/clld_morphology_plugin.egg-info/requires.txt
 src/clld_morphology_plugin.egg-info/top_level.txt
-src/clld_morphology_plugin/cldf/FormSlices-metadata.json
-src/clld_morphology_plugin/cldf/InflectionTable-metadata.json
-src/clld_morphology_plugin/cldf/LexemeLexemeParts-metadata.json
-src/clld_morphology_plugin/cldf/LexemeMorphemeParts-metadata.json
-src/clld_morphology_plugin/cldf/LexemeTable-metadata.json
-src/clld_morphology_plugin/cldf/MorphTable-metadata.json
-src/clld_morphology_plugin/cldf/MorphsetTable-metadata.json
-src/clld_morphology_plugin/cldf/POSTable-metadata.json
-src/clld_morphology_plugin/cldf/__init__.py
 src/clld_morphology_plugin/static/clld-morphology.css
 src/clld_morphology_plugin/templates/morphology_util.mako
+src/clld_morphology_plugin/templates/derivationalprocess/detail_html.mako
+src/clld_morphology_plugin/templates/derivationalprocess/index_html.mako
+src/clld_morphology_plugin/templates/form/detail_html.mako
+src/clld_morphology_plugin/templates/form/index_html.mako
+src/clld_morphology_plugin/templates/gloss/detail_html.mako
+src/clld_morphology_plugin/templates/inflectionalcategory/detail_html.mako
+src/clld_morphology_plugin/templates/inflectionalcategory/index_html.mako
+src/clld_morphology_plugin/templates/inflectionalvalue/detail_html.mako
+src/clld_morphology_plugin/templates/inflectionalvalue/index_html.mako
 src/clld_morphology_plugin/templates/lexeme/detail_html.mako
 src/clld_morphology_plugin/templates/lexeme/index_html.mako
 src/clld_morphology_plugin/templates/meaning/detail_html.mako
 src/clld_morphology_plugin/templates/meaning/index_html.mako
 src/clld_morphology_plugin/templates/morph/detail_html.mako
 src/clld_morphology_plugin/templates/morph/index_html.mako
 src/clld_morphology_plugin/templates/morpheme/detail_html.mako
 src/clld_morphology_plugin/templates/morpheme/index_html.mako
+src/clld_morphology_plugin/templates/morphophonologicalchange/detail_html.mako
+src/clld_morphology_plugin/templates/morphophonologicalchange/index_html.mako
 src/clld_morphology_plugin/templates/pos/detail_html.mako
 src/clld_morphology_plugin/templates/pos/index_html.mako
+src/clld_morphology_plugin/templates/stem/detail_html.mako
+src/clld_morphology_plugin/templates/stem/index_html.mako
 src/clld_morphology_plugin/templates/wordform/detail_html.mako
 src/clld_morphology_plugin/templates/wordform/index_html.mako
```

