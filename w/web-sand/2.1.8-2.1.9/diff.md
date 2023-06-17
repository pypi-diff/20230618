# Comparing `tmp/web-sand-2.1.8.tar.gz` & `tmp/web_sand-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web-sand-2.1.8.tar", max compression
+gzip compressed data, was "web_sand-2.1.9.tar", max compression
```

## Comparing `web-sand-2.1.8.tar` & `web_sand-2.1.9.tar`

### file list

```diff
@@ -1,91 +1,91 @@
--rw-r--r--   0        0        0     2210 2022-09-05 01:13:07.794138 web-sand-2.1.8/README.md
--rw-r--r--   0        0        0      785 2022-09-05 01:13:07.806138 web-sand-2.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/__init__.py
--rw-r--r--   0        0        0     2856 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/__main__.py
--rw-r--r--   0        0        0     2003 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/app.py
--rw-r--r--   0        0        0     1740 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/client.py
--rw-r--r--   0        0        0        0 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/commands/__init__.py
--rw-r--r--   0        0        0     1549 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/commands/load.py
--rw-r--r--   0        0        0     2304 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/config.py
--rw-r--r--   0        0        0        0 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/controllers/__init__.py
--rw-r--r--   0        0        0     5590 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/controllers/assistant.py
--rw-r--r--   0        0        0        0 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/controllers/helpers/__init__.py
--rw-r--r--   0        0        0     5290 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/controllers/helpers/upload.py
--rw-r--r--   0        0        0     5374 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/controllers/project.py
--rw-r--r--   0        0        0      612 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/controllers/settings.py
--rw-r--r--   0        0        0     7861 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/controllers/table.py
--rw-r--r--   0        0        0     8201 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/deserializer.py
--rw-r--r--   0        0        0      246 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/models/__init__.py
--rw-r--r--   0        0        0     2120 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/models/base.py
--rw-r--r--   0        0        0     2895 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/models/entity.py
--rw-r--r--   0        0        0     2484 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/models/ontology.py
--rw-r--r--   0        0        0      172 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/models/project.py
--rw-r--r--   0        0        0     1004 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/models/semantic_model.py
--rw-r--r--   0        0        0     3642 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/models/table.py
--rw-r--r--   0        0        0     2413 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/models/uploading_table.py.deprecated
--rw-r--r--   0        0        0       62 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/plugins/__init__.py
--rw-r--r--   0        0        0        0 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/plugins/drepr/__init__.py
--rw-r--r--   0        0        0      697 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/plugins/drepr/raw_transformations/global_coordinate.py
--rw-r--r--   0        0        0      130 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/plugins/drepr/raw_transformations/number.py
--rw-r--r--   0        0        0     4895 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/plugins/drepr/relational2rdf.py
--rw-r--r--   0        0        0     2181 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/plugins/drepr/resources.py
--rw-r--r--   0        0        0     4895 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/plugins/drepr/semanticmodel.py
--rw-r--r--   0        0        0      784 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/plugins/drepr/transformation.py
--rw-r--r--   0        0        0     1940 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/plugins/grams_plugin.py
--rw-r--r--   0        0        0     8008 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/plugins/mtab.py
--rw-r--r--   0        0        0     4959 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/plugins/wikidata.py
--rw-r--r--   0        0        0     4968 2022-09-05 01:13:07.806138 web-sand-2.1.8/sand/serializer.py
--rw-r--r--   0        0        0     3354 2022-09-05 01:17:03.966335 web-sand-2.1.8/sand/www/asset-manifest.json
--rw-r--r--   0        0        0     3180 2022-09-05 01:14:35.303753 web-sand-2.1.8/sand/www/favicon.ico
--rw-r--r--   0        0        0     3066 2022-09-05 01:17:03.898334 web-sand-2.1.8/sand/www/index.html
--rw-r--r--   0        0        0    10442 2022-09-05 01:14:35.303753 web-sand-2.1.8/sand/www/logo192.png
--rw-r--r--   0        0        0    41571 2022-09-05 01:14:35.303753 web-sand-2.1.8/sand/www/logo512.png
--rw-r--r--   0        0        0      485 2022-09-05 01:14:35.303753 web-sand-2.1.8/sand/www/manifest.json
--rw-r--r--   0        0        0       67 2022-09-05 01:14:35.303753 web-sand-2.1.8/sand/www/robots.txt
--rw-r--r--   0        0        0   574958 2022-09-05 01:17:03.962335 web-sand-2.1.8/sand/www/static/css/2.b3380b9b.chunk.css
--rw-r--r--   0        0        0  1590594 2022-09-05 01:17:03.962335 web-sand-2.1.8/sand/www/static/css/2.b3380b9b.chunk.css.map
--rw-r--r--   0        0        0      125 2022-09-05 01:17:03.898334 web-sand-2.1.8/sand/www/static/css/main.8470bb9a.chunk.css
--rw-r--r--   0        0        0      366 2022-09-05 01:17:03.962335 web-sand-2.1.8/sand/www/static/css/main.8470bb9a.chunk.css.map
--rw-r--r--   0        0        0  3614314 2022-09-05 01:17:03.962335 web-sand-2.1.8/sand/www/static/js/2.9bc60325.chunk.js
--rw-r--r--   0        0        0     4181 2022-09-05 01:17:03.962335 web-sand-2.1.8/sand/www/static/js/2.9bc60325.chunk.js.LICENSE.txt
--rw-r--r--   0        0        0 14556928 2022-09-05 01:17:03.966335 web-sand-2.1.8/sand/www/static/js/2.9bc60325.chunk.js.map
--rw-r--r--   0        0        0     4375 2022-09-05 01:17:03.962335 web-sand-2.1.8/sand/www/static/js/3.28cb8f3e.chunk.js
--rw-r--r--   0        0        0     9612 2022-09-05 01:17:03.966335 web-sand-2.1.8/sand/www/static/js/3.28cb8f3e.chunk.js.map
--rw-r--r--   0        0        0   138479 2022-09-05 01:17:03.898334 web-sand-2.1.8/sand/www/static/js/main.6cfd4db2.chunk.js
--rw-r--r--   0        0        0   442424 2022-09-05 01:17:03.962335 web-sand-2.1.8/sand/www/static/js/main.6cfd4db2.chunk.js.map
--rw-r--r--   0        0        0     2350 2022-09-05 01:17:03.962335 web-sand-2.1.8/sand/www/static/js/runtime-main.3b0ba70d.js
--rw-r--r--   0        0        0    12462 2022-09-05 01:17:03.966335 web-sand-2.1.8/sand/www/static/js/runtime-main.3b0ba70d.js.map
--rw-r--r--   0        0        0      134 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/default.003f90b3.less
--rw-r--r--   0        0        0     2074 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.00515a28.less
--rw-r--r--   0        0        0     1289 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.055e5992.less
--rw-r--r--   0        0        0     1434 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.0b3b5180.less
--rw-r--r--   0        0        0      248 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.222b2c74.less
--rw-r--r--   0        0        0      197 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.24d39731.less
--rw-r--r--   0        0        0      488 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.3f817bd9.less
--rw-r--r--   0        0        0     1604 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.42e22abe.less
--rw-r--r--   0        0        0      584 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.4eac1d48.less
--rw-r--r--   0        0        0       56 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.512735b3.less
--rw-r--r--   0        0        0      421 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.5636ef18.less
--rw-r--r--   0        0        0      356 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.57db1704.less
--rw-r--r--   0        0        0      197 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.5c257f6d.less
--rw-r--r--   0        0        0      319 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.67496dda.less
--rw-r--r--   0        0        0      280 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.84840f0d.less
--rw-r--r--   0        0        0      547 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.91905563.less
--rw-r--r--   0        0        0      506 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.a04a827f.less
--rw-r--r--   0        0        0      714 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.a3d92676.less
--rw-r--r--   0        0        0     1638 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.a5dc9231.less
--rw-r--r--   0        0        0      519 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.afe80595.less
--rw-r--r--   0        0        0     1932 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.b81af914.less
--rw-r--r--   0        0        0     1366 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.d53f1fd8.less
--rw-r--r--   0        0        0     1015 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.d58a1f05.less
--rw-r--r--   0        0        0      314 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.d94a7ca0.less
--rw-r--r--   0        0        0      317 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.e16b9e9f.less
--rw-r--r--   0        0        0      998 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.e2b6f656.less
--rw-r--r--   0        0        0      231 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.e7481eae.less
--rw-r--r--   0        0        0     1221 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.e8b6b0c3.less
--rw-r--r--   0        0        0      992 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.f2583e3d.less
--rw-r--r--   0        0        0     1174 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/index.f4067327.less
--rw-r--r--   0        0        0    60181 2022-09-05 01:17:03.894334 web-sand-2.1.8/sand/www/static/media/logo.aa0996dd.png
--rw-r--r--   0        0        0        5 2022-09-05 01:17:04.370342 web-sand-2.1.8/sand/www/version.txt
--rw-r--r--   0        0        0     3535 1970-01-01 00:00:00.000000 web-sand-2.1.8/setup.py
--rw-r--r--   0        0        0     3271 1970-01-01 00:00:00.000000 web-sand-2.1.8/PKG-INFO
+-rw-r--r--   0        0        0     2210 2022-12-24 07:04:40.507134 web_sand-2.1.9/README.md
+-rw-r--r--   0        0        0      784 2022-12-24 07:04:40.523134 web_sand-2.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-24 07:04:40.523134 web_sand-2.1.9/sand/__init__.py
+-rw-r--r--   0        0        0     2856 2022-12-24 07:04:40.523134 web_sand-2.1.9/sand/__main__.py
+-rw-r--r--   0        0        0     2018 2022-12-24 07:04:40.523134 web_sand-2.1.9/sand/app.py
+-rw-r--r--   0        0        0     1740 2022-12-24 07:04:40.523134 web_sand-2.1.9/sand/client.py
+-rw-r--r--   0        0        0        0 2022-12-24 07:04:40.523134 web_sand-2.1.9/sand/commands/__init__.py
+-rw-r--r--   0        0        0     1549 2022-12-24 07:04:40.523134 web_sand-2.1.9/sand/commands/load.py
+-rw-r--r--   0        0        0     2304 2022-12-24 07:04:40.523134 web_sand-2.1.9/sand/config.py
+-rw-r--r--   0        0        0        0 2022-12-24 07:04:40.523134 web_sand-2.1.9/sand/controllers/__init__.py
+-rw-r--r--   0        0        0     5590 2022-12-24 07:04:40.523134 web_sand-2.1.9/sand/controllers/assistant.py
+-rw-r--r--   0        0        0        0 2022-12-24 07:04:40.523134 web_sand-2.1.9/sand/controllers/helpers/__init__.py
+-rw-r--r--   0        0        0     5290 2022-12-24 07:04:40.523134 web_sand-2.1.9/sand/controllers/helpers/upload.py
+-rw-r--r--   0        0        0     4416 2022-12-24 07:04:40.523134 web_sand-2.1.9/sand/controllers/project.py
+-rw-r--r--   0        0        0      612 2022-12-24 07:04:40.523134 web_sand-2.1.9/sand/controllers/settings.py
+-rw-r--r--   0        0        0     7876 2022-12-24 07:04:40.523134 web_sand-2.1.9/sand/controllers/table.py
+-rw-r--r--   0        0        0     8216 2022-12-24 07:04:40.523134 web_sand-2.1.9/sand/deserializer.py
+-rw-r--r--   0        0        0      246 2022-12-24 07:04:40.523134 web_sand-2.1.9/sand/models/__init__.py
+-rw-r--r--   0        0        0     2120 2022-12-24 07:04:40.523134 web_sand-2.1.9/sand/models/base.py
+-rw-r--r--   0        0        0     2895 2022-12-24 07:04:40.523134 web_sand-2.1.9/sand/models/entity.py
+-rw-r--r--   0        0        0     2484 2022-12-24 07:04:40.523134 web_sand-2.1.9/sand/models/ontology.py
+-rw-r--r--   0        0        0      172 2022-12-24 07:04:40.523134 web_sand-2.1.9/sand/models/project.py
+-rw-r--r--   0        0        0     1019 2022-12-24 07:04:40.523134 web_sand-2.1.9/sand/models/semantic_model.py
+-rw-r--r--   0        0        0     3642 2022-12-24 07:04:40.523134 web_sand-2.1.9/sand/models/table.py
+-rw-r--r--   0        0        0     2413 2022-12-24 07:04:40.523134 web_sand-2.1.9/sand/models/uploading_table.py.deprecated
+-rw-r--r--   0        0        0       62 2022-12-24 07:04:40.527134 web_sand-2.1.9/sand/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-24 07:04:40.527134 web_sand-2.1.9/sand/plugins/drepr/__init__.py
+-rw-r--r--   0        0        0      697 2022-12-24 07:04:40.527134 web_sand-2.1.9/sand/plugins/drepr/raw_transformations/global_coordinate.py
+-rw-r--r--   0        0        0      130 2022-12-24 07:04:40.527134 web_sand-2.1.9/sand/plugins/drepr/raw_transformations/number.py
+-rw-r--r--   0        0        0     4910 2022-12-24 07:04:40.527134 web_sand-2.1.9/sand/plugins/drepr/relational2rdf.py
+-rw-r--r--   0        0        0     2125 2022-12-24 07:04:40.527134 web_sand-2.1.9/sand/plugins/drepr/resources.py
+-rw-r--r--   0        0        0     4910 2022-12-24 07:04:40.527134 web_sand-2.1.9/sand/plugins/drepr/semanticmodel.py
+-rw-r--r--   0        0        0      784 2022-12-24 07:04:40.527134 web_sand-2.1.9/sand/plugins/drepr/transformation.py
+-rw-r--r--   0        0        0     1940 2022-12-24 07:04:40.527134 web_sand-2.1.9/sand/plugins/grams_plugin.py
+-rw-r--r--   0        0        0     7782 2022-12-24 07:04:40.527134 web_sand-2.1.9/sand/plugins/mtab.py
+-rw-r--r--   0        0        0     4959 2022-12-24 07:04:40.527134 web_sand-2.1.9/sand/plugins/wikidata.py
+-rw-r--r--   0        0        0     4983 2022-12-24 07:04:40.527134 web_sand-2.1.9/sand/serializer.py
+-rw-r--r--   0        0        0     3354 2022-12-24 07:10:12.729292 web_sand-2.1.9/sand/www/asset-manifest.json
+-rw-r--r--   0        0        0     3180 2022-12-24 07:06:44.640042 web_sand-2.1.9/sand/www/favicon.ico
+-rw-r--r--   0        0        0     3066 2022-12-24 07:10:12.665291 web_sand-2.1.9/sand/www/index.html
+-rw-r--r--   0        0        0    10442 2022-12-24 07:06:44.640042 web_sand-2.1.9/sand/www/logo192.png
+-rw-r--r--   0        0        0    41571 2022-12-24 07:06:44.652042 web_sand-2.1.9/sand/www/logo512.png
+-rw-r--r--   0        0        0      485 2022-12-24 07:06:44.652042 web_sand-2.1.9/sand/www/manifest.json
+-rw-r--r--   0        0        0       67 2022-12-24 07:06:44.652042 web_sand-2.1.9/sand/www/robots.txt
+-rw-r--r--   0        0        0   574958 2022-12-24 07:10:12.721292 web_sand-2.1.9/sand/www/static/css/2.b3380b9b.chunk.css
+-rw-r--r--   0        0        0  1590594 2022-12-24 07:10:12.725292 web_sand-2.1.9/sand/www/static/css/2.b3380b9b.chunk.css.map
+-rw-r--r--   0        0        0      125 2022-12-24 07:10:12.665291 web_sand-2.1.9/sand/www/static/css/main.8470bb9a.chunk.css
+-rw-r--r--   0        0        0      366 2022-12-24 07:10:12.725292 web_sand-2.1.9/sand/www/static/css/main.8470bb9a.chunk.css.map
+-rw-r--r--   0        0        0  3614314 2022-12-24 07:10:12.725292 web_sand-2.1.9/sand/www/static/js/2.9bc60325.chunk.js
+-rw-r--r--   0        0        0     4181 2022-12-24 07:10:12.725292 web_sand-2.1.9/sand/www/static/js/2.9bc60325.chunk.js.LICENSE.txt
+-rw-r--r--   0        0        0 14556928 2022-12-24 07:10:12.725292 web_sand-2.1.9/sand/www/static/js/2.9bc60325.chunk.js.map
+-rw-r--r--   0        0        0     4375 2022-12-24 07:10:12.725292 web_sand-2.1.9/sand/www/static/js/3.28cb8f3e.chunk.js
+-rw-r--r--   0        0        0     9612 2022-12-24 07:10:12.729292 web_sand-2.1.9/sand/www/static/js/3.28cb8f3e.chunk.js.map
+-rw-r--r--   0        0        0   138479 2022-12-24 07:10:12.665291 web_sand-2.1.9/sand/www/static/js/main.6cfd4db2.chunk.js
+-rw-r--r--   0        0        0   442424 2022-12-24 07:10:12.725292 web_sand-2.1.9/sand/www/static/js/main.6cfd4db2.chunk.js.map
+-rw-r--r--   0        0        0     2350 2022-12-24 07:10:12.721292 web_sand-2.1.9/sand/www/static/js/runtime-main.3b0ba70d.js
+-rw-r--r--   0        0        0    12462 2022-12-24 07:10:12.725292 web_sand-2.1.9/sand/www/static/js/runtime-main.3b0ba70d.js.map
+-rw-r--r--   0        0        0      134 2022-12-24 07:10:12.661291 web_sand-2.1.9/sand/www/static/media/default.003f90b3.less
+-rw-r--r--   0        0        0     2074 2022-12-24 07:10:12.661291 web_sand-2.1.9/sand/www/static/media/index.00515a28.less
+-rw-r--r--   0        0        0     1289 2022-12-24 07:10:12.665291 web_sand-2.1.9/sand/www/static/media/index.055e5992.less
+-rw-r--r--   0        0        0     1434 2022-12-24 07:10:12.665291 web_sand-2.1.9/sand/www/static/media/index.0b3b5180.less
+-rw-r--r--   0        0        0      248 2022-12-24 07:10:12.665291 web_sand-2.1.9/sand/www/static/media/index.222b2c74.less
+-rw-r--r--   0        0        0      197 2022-12-24 07:10:12.665291 web_sand-2.1.9/sand/www/static/media/index.24d39731.less
+-rw-r--r--   0        0        0      488 2022-12-24 07:10:12.661291 web_sand-2.1.9/sand/www/static/media/index.3f817bd9.less
+-rw-r--r--   0        0        0     1604 2022-12-24 07:10:12.665291 web_sand-2.1.9/sand/www/static/media/index.42e22abe.less
+-rw-r--r--   0        0        0      584 2022-12-24 07:10:12.661291 web_sand-2.1.9/sand/www/static/media/index.4eac1d48.less
+-rw-r--r--   0        0        0       56 2022-12-24 07:10:12.661291 web_sand-2.1.9/sand/www/static/media/index.512735b3.less
+-rw-r--r--   0        0        0      421 2022-12-24 07:10:12.665291 web_sand-2.1.9/sand/www/static/media/index.5636ef18.less
+-rw-r--r--   0        0        0      356 2022-12-24 07:10:12.661291 web_sand-2.1.9/sand/www/static/media/index.57db1704.less
+-rw-r--r--   0        0        0      197 2022-12-24 07:10:12.661291 web_sand-2.1.9/sand/www/static/media/index.5c257f6d.less
+-rw-r--r--   0        0        0      319 2022-12-24 07:10:12.665291 web_sand-2.1.9/sand/www/static/media/index.67496dda.less
+-rw-r--r--   0        0        0      280 2022-12-24 07:10:12.661291 web_sand-2.1.9/sand/www/static/media/index.84840f0d.less
+-rw-r--r--   0        0        0      547 2022-12-24 07:10:12.661291 web_sand-2.1.9/sand/www/static/media/index.91905563.less
+-rw-r--r--   0        0        0      506 2022-12-24 07:10:12.665291 web_sand-2.1.9/sand/www/static/media/index.a04a827f.less
+-rw-r--r--   0        0        0      714 2022-12-24 07:10:12.661291 web_sand-2.1.9/sand/www/static/media/index.a3d92676.less
+-rw-r--r--   0        0        0     1638 2022-12-24 07:10:12.661291 web_sand-2.1.9/sand/www/static/media/index.a5dc9231.less
+-rw-r--r--   0        0        0      519 2022-12-24 07:10:12.661291 web_sand-2.1.9/sand/www/static/media/index.afe80595.less
+-rw-r--r--   0        0        0     1932 2022-12-24 07:10:12.661291 web_sand-2.1.9/sand/www/static/media/index.b81af914.less
+-rw-r--r--   0        0        0     1366 2022-12-24 07:10:12.661291 web_sand-2.1.9/sand/www/static/media/index.d53f1fd8.less
+-rw-r--r--   0        0        0     1015 2022-12-24 07:10:12.661291 web_sand-2.1.9/sand/www/static/media/index.d58a1f05.less
+-rw-r--r--   0        0        0      314 2022-12-24 07:10:12.665291 web_sand-2.1.9/sand/www/static/media/index.d94a7ca0.less
+-rw-r--r--   0        0        0      317 2022-12-24 07:10:12.665291 web_sand-2.1.9/sand/www/static/media/index.e16b9e9f.less
+-rw-r--r--   0        0        0      998 2022-12-24 07:10:12.665291 web_sand-2.1.9/sand/www/static/media/index.e2b6f656.less
+-rw-r--r--   0        0        0      231 2022-12-24 07:10:12.665291 web_sand-2.1.9/sand/www/static/media/index.e7481eae.less
+-rw-r--r--   0        0        0     1221 2022-12-24 07:10:12.661291 web_sand-2.1.9/sand/www/static/media/index.e8b6b0c3.less
+-rw-r--r--   0        0        0      992 2022-12-24 07:10:12.665291 web_sand-2.1.9/sand/www/static/media/index.f2583e3d.less
+-rw-r--r--   0        0        0     1174 2022-12-24 07:10:12.665291 web_sand-2.1.9/sand/www/static/media/index.f4067327.less
+-rw-r--r--   0        0        0    60181 2022-12-24 07:10:12.665291 web_sand-2.1.9/sand/www/static/media/logo.aa0996dd.png
+-rw-r--r--   0        0        0        5 2022-12-24 07:10:13.169294 web_sand-2.1.9/sand/www/version.txt
+-rw-r--r--   0        0        0     3542 1970-01-01 00:00:00.000000 web_sand-2.1.9/setup.py
+-rw-r--r--   0        0        0     3278 1970-01-01 00:00:00.000000 web_sand-2.1.9/PKG-INFO
```

### Comparing `web-sand-2.1.8/README.md` & `web_sand-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/pyproject.toml` & `web_sand-2.1.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "web-sand"
-version = "2.1.8"
+version = "2.1.9"
 description = "UI for browsing/editing semantic descriptions"
 authors = ["Binh Vu <binh@toan2.com>"]
 repository = "https://github.com/usc-isi-i2/sand"
 license = "MIT"
 packages = [
     { include = "sand" }
 ]
@@ -12,27 +12,27 @@
 include = ["sand/www/**/*"]
 
 [tool.poetry.scripts]
 sand = 'sand.__main__:cli'
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
-kgdata = "^3.0.2"
-sm-grams = "^2.1.3"
-sem-desc = "^3.5.2"
-peewee = "^3.14.4"
-Flask = "^2.0.2"
+kgdata = "^3.3.0"
+sm-grams = "^2.1.7"
+sem-desc = "^4.1.6"
+peewee = "^3.15.2"
+Flask = "^2.2.2"
 python-dotenv = ">=0.19.0"
-tornado = "^6.1"
-gena = "^1.1.2"
-loguru = ">=0.6.0"
-orjson = "^3.6.8"
+tornado = "^6.2"
+gena = "^1.6.4"
+loguru = "^0.6.0"
+orjson = "^3.8.2"
 drepr = "^2.10.0"
 
 lat_lon_parser = "^1.3.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2.5"
+pytest = "^7.1.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `web-sand-2.1.8/sand/__main__.py` & `web_sand-2.1.9/sand/__main__.py`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/app.py` & `web_sand-2.1.9/sand/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-import sm.outputs as O
+import sm.outputs.semantic_model as O
 from gena import generate_api, generate_app, generate_readonly_api_4dict
 from hugedict.chained_mapping import ChainedMapping
 from sm.misc.funcs import import_attr
 
 from sand.config import SETTINGS
 from sand.controllers.assistant import assistant_bp
 from sand.controllers.project import project_bp
```

### Comparing `web-sand-2.1.8/sand/client.py` & `web_sand-2.1.9/sand/client.py`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/commands/load.py` & `web_sand-2.1.9/sand/commands/load.py`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/config.py` & `web_sand-2.1.9/sand/config.py`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/controllers/assistant.py` & `web_sand-2.1.9/sand/controllers/assistant.py`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/controllers/helpers/upload.py` & `web_sand-2.1.9/sand/controllers/helpers/upload.py`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/controllers/project.py` & `web_sand-2.1.9/sand/controllers/project.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,58 +1,27 @@
-import copy
-import csv
 from dataclasses import asdict
-import os
-from functools import partial
-from io import StringIO
-from typing import List, Optional, Union, cast, no_type_check_decorator
+from typing import List
 
 import orjson
-import sm.misc as M
-import sm.outputs as O
 from flask import json, jsonify, request
-from gena import generate_api, generate_app, generate_readonly_api_4dict
+from gena import generate_api
 from gena.deserializer import (
-    deserialize_dict,
-    generate_deserializer,
     get_dataclass_deserializer,
 )
-from grams.inputs.context import Attribute
-from hugedict.chained_mapping import ChainedMapping
-from peewee import DoesNotExist
-from peewee import Model as PeeweeModel
-from peewee import fn
 from sand.controllers.helpers.upload import (
     ALLOWED_EXTENSIONS,
     CSVParserOpts,
-    RawTable,
     UploadingTable,
     get_extension,
     parse_upload,
     save_upload,
 )
-from sand.deserializer import deserialize_graph
 from sand.models import (
-    EntityAR,
     Project,
-    SemanticModel,
-    Table,
-    TableRow,
 )
-from sand.models.entity import Value
-from sand.models.ontology import OntClass, OntClassAR, OntProperty, OntPropertyAR
-from sand.plugins.wikidata import DEFAULT_ONT_CLASSES, DEFAULT_ONT_PROPS
-from sand.serializer import (
-    batch_serialize_sms,
-    get_label,
-    serialize_class,
-    serialize_entity,
-    serialize_property,
-)
-from werkzeug.datastructures import FileStorage
 from werkzeug.exceptions import BadRequest
 from sand.controllers.helpers.upload import CSVParserOpts, JSONParserOpts
 
 project_bp = generate_api(Project)
 
 deser_CSVParserOpts = get_dataclass_deserializer(CSVParserOpts, {})
 deser_JSONParserOpts = get_dataclass_deserializer(JSONParserOpts, {})
```

### Comparing `web-sand-2.1.8/sand/controllers/settings.py` & `web_sand-2.1.9/sand/controllers/settings.py`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/controllers/table.py` & `web_sand-2.1.9/sand/controllers/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from sand.serializer import (
     get_label,
     serialize_class,
     serialize_entity,
     batch_serialize_sms,
     serialize_property,
 )
-import sm.outputs as O
+import sm.outputs.semantic_model as O
 from sand.plugins.wikidata import DEFAULT_ONT_CLASSES, DEFAULT_ONT_PROPS
 from flask import json, jsonify, request, make_response
 from peewee import Model as PeeweeModel, DoesNotExist, fn
 
 from werkzeug.exceptions import BadRequest, NotFound
 
 table_bp = generate_api(
```

### Comparing `web-sand-2.1.8/sand/deserializer.py` & `web_sand-2.1.9/sand/deserializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from gena.deserializer import get_dataclass_deserializer
-import sm.outputs as O
+import sm.outputs.semantic_model as O
 from sm.outputs.semantic_model import LiteralNodeDataType
 from sand.plugins.wikidata import get_rel_uri
 
 
 def deserialize_graph(value) -> O.SemanticModel:
     if not isinstance(value, dict):
         raise ValueError(f"expect dictionary but get {type(value)}")
```

### Comparing `web-sand-2.1.8/sand/models/base.py` & `web_sand-2.1.9/sand/models/base.py`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/models/entity.py` & `web_sand-2.1.9/sand/models/entity.py`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/models/ontology.py` & `web_sand-2.1.9/sand/models/ontology.py`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/models/semantic_model.py` & `web_sand-2.1.9/sand/models/semantic_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import orjson
-import sm.outputs as O
+import sm.outputs.semantic_model as O
 from peewee import CharField, ForeignKeyField, TextField, IntegerField
 from playhouse.shortcuts import model_to_dict
 from sand.models.base import BaseModel, BlobField
 from sand.models.project import Project
 from sand.models.table import Table
```

### Comparing `web-sand-2.1.8/sand/models/table.py` & `web_sand-2.1.9/sand/models/table.py`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/models/uploading_table.py.deprecated` & `web_sand-2.1.9/sand/models/uploading_table.py.deprecated`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/plugins/drepr/raw_transformations/global_coordinate.py` & `web_sand-2.1.9/sand/plugins/drepr/raw_transformations/global_coordinate.py`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/plugins/drepr/relational2rdf.py` & `web_sand-2.1.9/sand/plugins/drepr/relational2rdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from io import StringIO
 import orjson, csv
 from typing import Dict, List, Set, Tuple, cast
 from sand.config import SETTINGS
 from sand.models.entity import NIL_ENTITY, Entity
 from sand.models.ontology import OntProperty, OntPropertyAR, OntPropertyDataType
 from sand.models.table import Table, TableRow
-import sm.outputs as O
+import sm.outputs.semantic_model as O
 import sm.misc as M
 from hugedict.chained_mapping import ChainedMapping
 from drepr.models import (
     DRepr,
     Attr,
     Resource,
     ResourceType,
```

### Comparing `web-sand-2.1.8/sand/plugins/drepr/resources.py` & `web_sand-2.1.9/sand/plugins/drepr/resources.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from dataclasses import dataclass
 from io import StringIO
 import orjson, csv
 from typing import Dict, List, Set, Tuple
 from sand.config import SETTINGS
 from sand.models.entity import NIL_ENTITY, Entity
-from sand.models.ontology import OntProperty, OntPropertyAR
+from sand.models.ontology import OntPropertyAR
 from sand.models.table import Table, TableRow
-import sm.outputs as O
-import sm.misc as M
 from drepr.models import (
     ResourceDataString,
     ResourceData,
 )
 from uuid import uuid4
```

### Comparing `web-sand-2.1.8/sand/plugins/drepr/semanticmodel.py` & `web_sand-2.1.9/sand/plugins/drepr/semanticmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from io import StringIO
 import orjson, csv
 from typing import Callable, Dict, List, Mapping, Set, Tuple
 from sand.config import SETTINGS
 from sand.models.entity import NIL_ENTITY, Entity
 from sand.models.ontology import OntProperty, OntPropertyAR, OntPropertyDataType
 from sand.models.table import Table, TableRow
-import sm.outputs as O
+import sm.outputs.semantic_model as O
 import sm.misc as M
 from sm.namespaces.wikidata import WikidataNamespace
 import drepr.models.sm as drepr_sm
 
 
 prefixes = WikidataNamespace.create().prefix2ns.copy()
 prefixes.update(drepr_sm.SemanticModel.get_default_prefixes())
```

### Comparing `web-sand-2.1.8/sand/plugins/drepr/transformation.py` & `web_sand-2.1.9/sand/plugins/drepr/transformation.py`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/plugins/grams_plugin.py` & `web_sand-2.1.9/sand/plugins/grams_plugin.py`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/plugins/mtab.py` & `web_sand-2.1.9/sand/plugins/mtab.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,19 @@
 import copy
 from rdflib import RDFS
 import subprocess
-from abc import ABC, abstractmethod
 from pathlib import Path
-import threading
 from typing import Dict, List, Tuple
-from flask.blueprints import Blueprint
-from sm.misc.funcs import V, import_func
-from sm.misc.deser import (
-    deserialize_csv,
-    deserialize_json,
-    deserialize_text,
-    serialize_csv,
-)
+import serde.prelude as serde
 from sm.namespaces.wikidata import WikidataNamespace
-import sm.outputs as O
+import sm.outputs.semantic_model as O
 from sand.controllers.assistant import Assistant
-from sand.models.base import init_db, db
+from sand.models.base import init_db
 
 from sand.models.table import CandidateEntity, Link, Table, TableRow
-from flask import request, jsonify
-from uuid import uuid4
 
 
 class MTabAssistant(Assistant):
     def __init__(self):
         self.cache_dir = Path(f"/tmp/mtab")
         self.cache_dir.mkdir(exist_ok=True)
 
@@ -38,34 +27,36 @@
         cwd = self.cache_dir / f"p{table.project.id}-t:{table.id}-{table.name}"
         cwd.mkdir(exist_ok=True)
         infile = cwd / "infile.csv"
         outfile = cwd / "outfile.json"
 
         rerun = True
         if infile.exists() and outfile.exists():
-            serialize_csv(content, str(infile) + ".tmp")
-            if deserialize_text(infile) == deserialize_text(str(infile) + ".tmp"):
+            serde.csv.ser(content, str(infile) + ".tmp")
+            if serde.textline.deser(infile) == serde.textline.deser(
+                str(infile) + ".tmp"
+            ):
                 rerun = False
 
         if rerun:
-            serialize_csv(content, infile)
+            serde.csv.ser(content, infile)
             subprocess.check_call(
                 [
                     "curl",
                     "-X",
                     "POST",
                     "-F",
                     f"file=@{str(infile)}",
                     "https://mtab.app/api/v1/mtab?limit=1000",
                     "-o",
                     outfile,
                 ]
             )
 
-        record = deserialize_json(outfile)
+        record = serde.json.deser(outfile)
         assert record["status"] == "Success"
 
         semantic = record["tables"][0]["semantic"]
 
         cpa, cta = [], {}
         for item in semantic["cpa"]:
             source, target = item["target"]
```

### Comparing `web-sand-2.1.8/sand/plugins/wikidata.py` & `web_sand-2.1.9/sand/plugins/wikidata.py`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/serializer.py` & `web_sand-2.1.9/sand/serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import asdict
 from functools import partial
 from typing import Callable, Dict, List, Mapping, Optional
 
 from playhouse.shortcuts import model_to_dict
 
-import sm.outputs as O
+import sm.outputs.semantic_model as O
 from sand.models import SemanticModel, Table
 from sand.models.entity import Entity, EntityAR
 from sand.models.ontology import OntProperty, OntClass, OntPropertyAR, OntClassAR
 
 
 def serialize_property(prop: OntProperty):
     return {
```

### Comparing `web-sand-2.1.8/sand/www/asset-manifest.json` & `web_sand-2.1.9/sand/www/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/favicon.ico` & `web_sand-2.1.9/sand/www/favicon.ico`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/index.html` & `web_sand-2.1.9/sand/www/index.html`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/logo192.png` & `web_sand-2.1.9/sand/www/logo192.png`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/logo512.png` & `web_sand-2.1.9/sand/www/logo512.png`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/static/css/2.b3380b9b.chunk.css` & `web_sand-2.1.9/sand/www/static/css/2.b3380b9b.chunk.css`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/static/css/2.b3380b9b.chunk.css.map` & `web_sand-2.1.9/sand/www/static/css/2.b3380b9b.chunk.css.map`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/static/js/2.9bc60325.chunk.js` & `web_sand-2.1.9/sand/www/static/js/2.9bc60325.chunk.js`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/static/js/2.9bc60325.chunk.js.LICENSE.txt` & `web_sand-2.1.9/sand/www/static/js/2.9bc60325.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/static/js/2.9bc60325.chunk.js.map` & `web_sand-2.1.9/sand/www/static/js/2.9bc60325.chunk.js.map`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/static/js/3.28cb8f3e.chunk.js` & `web_sand-2.1.9/sand/www/static/js/3.28cb8f3e.chunk.js`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/static/js/3.28cb8f3e.chunk.js.map` & `web_sand-2.1.9/sand/www/static/js/3.28cb8f3e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/static/js/main.6cfd4db2.chunk.js` & `web_sand-2.1.9/sand/www/static/js/main.6cfd4db2.chunk.js`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/static/js/main.6cfd4db2.chunk.js.map` & `web_sand-2.1.9/sand/www/static/js/main.6cfd4db2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/static/js/runtime-main.3b0ba70d.js` & `web_sand-2.1.9/sand/www/static/js/runtime-main.3b0ba70d.js`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/static/js/runtime-main.3b0ba70d.js.map` & `web_sand-2.1.9/sand/www/static/js/runtime-main.3b0ba70d.js.map`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/static/media/index.00515a28.less` & `web_sand-2.1.9/sand/www/static/media/index.00515a28.less`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/static/media/index.055e5992.less` & `web_sand-2.1.9/sand/www/static/media/index.055e5992.less`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/static/media/index.0b3b5180.less` & `web_sand-2.1.9/sand/www/static/media/index.0b3b5180.less`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/static/media/index.42e22abe.less` & `web_sand-2.1.9/sand/www/static/media/index.42e22abe.less`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/static/media/index.4eac1d48.less` & `web_sand-2.1.9/sand/www/static/media/index.4eac1d48.less`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/static/media/index.91905563.less` & `web_sand-2.1.9/sand/www/static/media/index.91905563.less`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/static/media/index.a3d92676.less` & `web_sand-2.1.9/sand/www/static/media/index.a3d92676.less`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/static/media/index.a5dc9231.less` & `web_sand-2.1.9/sand/www/static/media/index.a5dc9231.less`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/static/media/index.afe80595.less` & `web_sand-2.1.9/sand/www/static/media/index.afe80595.less`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/static/media/index.b81af914.less` & `web_sand-2.1.9/sand/www/static/media/index.b81af914.less`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/static/media/index.d53f1fd8.less` & `web_sand-2.1.9/sand/www/static/media/index.d53f1fd8.less`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/static/media/index.d58a1f05.less` & `web_sand-2.1.9/sand/www/static/media/index.d58a1f05.less`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/static/media/index.e2b6f656.less` & `web_sand-2.1.9/sand/www/static/media/index.e2b6f656.less`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/static/media/index.e8b6b0c3.less` & `web_sand-2.1.9/sand/www/static/media/index.e8b6b0c3.less`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/static/media/index.f2583e3d.less` & `web_sand-2.1.9/sand/www/static/media/index.f2583e3d.less`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/static/media/index.f4067327.less` & `web_sand-2.1.9/sand/www/static/media/index.f4067327.less`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/sand/www/static/media/logo.aa0996dd.png` & `web_sand-2.1.9/sand/www/static/media/logo.aa0996dd.png`

 * *Files identical despite different names*

### Comparing `web-sand-2.1.8/setup.py` & `web_sand-2.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,33 +12,33 @@
  'sand.plugins.drepr.raw_transformations']
 
 package_data = \
 {'': ['*'],
  'sand': ['www/*', 'www/static/css/*', 'www/static/js/*', 'www/static/media/*']}
 
 install_requires = \
-['Flask>=2.0.2,<3.0.0',
+['Flask>=2.2.2,<3.0.0',
  'drepr>=2.10.0,<3.0.0',
- 'gena>=1.1.2,<2.0.0',
- 'kgdata>=3.0.2,<4.0.0',
+ 'gena>=1.6.4,<2.0.0',
+ 'kgdata>=3.3.0,<4.0.0',
  'lat_lon_parser>=1.3.0,<2.0.0',
- 'loguru>=0.6.0',
- 'orjson>=3.6.8,<4.0.0',
- 'peewee>=3.14.4,<4.0.0',
+ 'loguru>=0.6.0,<0.7.0',
+ 'orjson>=3.8.2,<4.0.0',
+ 'peewee>=3.15.2,<4.0.0',
  'python-dotenv>=0.19.0',
- 'sem-desc>=3.5.2,<4.0.0',
- 'sm-grams>=2.1.3,<3.0.0',
- 'tornado>=6.1,<7.0']
+ 'sem-desc>=4.1.6,<5.0.0',
+ 'sm-grams>=2.1.7,<3.0.0',
+ 'tornado>=6.2,<7.0']
 
 entry_points = \
 {'console_scripts': ['sand = sand.__main__:cli']}
 
 setup_kwargs = {
     'name': 'web-sand',
-    'version': '2.1.8',
+    'version': '2.1.9',
     'description': 'UI for browsing/editing semantic descriptions',
     'long_description': '<h1 align="center">SAND</h1>\n\n<div align="center">\n\n![PyPI](https://img.shields.io/pypi/v/web-sand)\n![Python](https://img.shields.io/badge/python-v3.8+-blue.svg)\n[![GitHub Issues](https://img.shields.io/github/issues/usc-isi-i2/sand.svg)](https://github.com/usc-isi-i2/sand/issues)\n![Contributions welcome](https://img.shields.io/badge/contributions-welcome-orange.svg)\n[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)\n\n</div>\n\n## Table of Contents\n\n- [Introduction](#introduction)\n- [Installation](#installation)\n\n## Introduction\n\nSAND is an application to annotate semantic descriptions of tables and (optionally) linked records in tables to a target knowledge graph, then it can automatically export the table data to RDF, JSON-LD, etc. It also does basic data cleaning automatically based on the annotated semantic descriptions. SAND is designed to be customizable: you can plug in a new semantic modeling algorithm (which generates a semantic description automatically) or different knowledge graphs as long as you have a suitable plugin implemented SAND\'s plugin interface.\n\nMoreover, SAND offers an internal KG browsing and table filtering so you can interactively browsing and modeling your tables.\n\nFor a demo, please see: our [demo paper](./docs/paper.pdf), [demo video](https://github.com/usc-isi-i2/sand/wiki/Demo).\n\n<!-- For more documentation, please see [not available yet](). -->\n\n## Installation\n\nInstall from pip: `pip install -U web-sand`\n\n## Usage\n\n1. Initialize database: `sand init -d <dbfile>`. For example: `sand init -d ./data/sand.db`\n2. Start the webserver: `sand start -d <dbfile> --externaldb <folder_of_ent_and_ont_db>`\n3. Open the URL: `http://localhost:5524`\n\nFor example, checkout [server.sh](./server.sh)\n\n## Development\n\n0. cd to `www`\n1. Install `yarn` and [`yalc`](https://github.com/wclr/yalc)\n2. Install dependencies: `yarn install`\n3. Start development server: `yarn start`. Then, access development server at: `http://127.0.0.1:3000`.\n4. Build production files: `yarn build`\n5. Build library files and publish to private index (only if you are released `sand` as a library): `yarn build:lib && yalc public --private`\n',
     'author': 'Binh Vu',
     'author_email': 'binh@toan2.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/usc-isi-i2/sand',
```

### Comparing `web-sand-2.1.8/PKG-INFO` & `web_sand-2.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: web-sand
-Version: 2.1.8
+Version: 2.1.9
 Summary: UI for browsing/editing semantic descriptions
 Home-page: https://github.com/usc-isi-i2/sand
 License: MIT
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: Flask (>=2.0.2,<3.0.0)
+Requires-Dist: Flask (>=2.2.2,<3.0.0)
 Requires-Dist: drepr (>=2.10.0,<3.0.0)
-Requires-Dist: gena (>=1.1.2,<2.0.0)
-Requires-Dist: kgdata (>=3.0.2,<4.0.0)
+Requires-Dist: gena (>=1.6.4,<2.0.0)
+Requires-Dist: kgdata (>=3.3.0,<4.0.0)
 Requires-Dist: lat_lon_parser (>=1.3.0,<2.0.0)
-Requires-Dist: loguru (>=0.6.0)
-Requires-Dist: orjson (>=3.6.8,<4.0.0)
-Requires-Dist: peewee (>=3.14.4,<4.0.0)
+Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: orjson (>=3.8.2,<4.0.0)
+Requires-Dist: peewee (>=3.15.2,<4.0.0)
 Requires-Dist: python-dotenv (>=0.19.0)
-Requires-Dist: sem-desc (>=3.5.2,<4.0.0)
-Requires-Dist: sm-grams (>=2.1.3,<3.0.0)
-Requires-Dist: tornado (>=6.1,<7.0)
+Requires-Dist: sem-desc (>=4.1.6,<5.0.0)
+Requires-Dist: sm-grams (>=2.1.7,<3.0.0)
+Requires-Dist: tornado (>=6.2,<7.0)
 Project-URL: Repository, https://github.com/usc-isi-i2/sand
 Description-Content-Type: text/markdown
 
 <h1 align="center">SAND</h1>
 
 <div align="center">
```

