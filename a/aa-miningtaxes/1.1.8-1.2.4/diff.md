# Comparing `tmp/aa-miningtaxes-1.1.8.tar.gz` & `tmp/aa-miningtaxes-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-miningtaxes-1.1.8.tar", last modified: Wed Dec 21 21:29:49 2022, max compression
+gzip compressed data, was "aa-miningtaxes-1.2.4.tar", last modified: Sun Jun 18 15:07:15 2023, max compression
```

## Comparing `aa-miningtaxes-1.1.8.tar` & `aa-miningtaxes-1.2.4.tar`

### file list

```diff
@@ -1,89 +1,95 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.423578 aa-miningtaxes-1.1.8/
--rw-r--r--   0 root         (0) root         (0)     1070 2022-10-24 20:51:10.000000 aa-miningtaxes-1.1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      183 2022-11-06 18:50:28.000000 aa-miningtaxes-1.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7283 2022-12-21 21:29:49.423578 aa-miningtaxes-1.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5580 2022-12-11 21:19:35.000000 aa-miningtaxes-1.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.415578 aa-miningtaxes-1.1.8/aa_miningtaxes.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7283 2022-12-21 21:29:49.000000 aa-miningtaxes-1.1.8/aa_miningtaxes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2604 2022-12-21 21:29:49.000000 aa-miningtaxes-1.1.8/aa_miningtaxes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-21 21:29:49.000000 aa-miningtaxes-1.1.8/aa_miningtaxes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       75 2022-12-21 21:29:49.000000 aa-miningtaxes-1.1.8/aa_miningtaxes.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2022-12-21 21:29:49.000000 aa-miningtaxes-1.1.8/aa_miningtaxes.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.417578 aa-miningtaxes-1.1.8/miningtaxes/
--rw-r--r--   0 root         (0) root         (0)      108 2022-12-21 21:23:09.000000 aa-miningtaxes-1.1.8/miningtaxes/__init__.py
--rw-r--r--   0 root         (0) root         (0)       84 2022-10-24 20:51:10.000000 aa-miningtaxes-1.1.8/miningtaxes/admin.py
--rw-r--r--   0 root         (0) root         (0)     1546 2022-12-11 21:19:35.000000 aa-miningtaxes-1.1.8/miningtaxes/app_settings.py
--rw-r--r--   0 root         (0) root         (0)      200 2022-10-27 10:33:48.000000 aa-miningtaxes-1.1.8/miningtaxes/apps.py
--rw-r--r--   0 root         (0) root         (0)      912 2022-10-24 21:25:29.000000 aa-miningtaxes-1.1.8/miningtaxes/auth_hooks.py
--rw-r--r--   0 root         (0) root         (0)     3304 2022-11-07 04:47:52.000000 aa-miningtaxes-1.1.8/miningtaxes/decorators.py
--rw-r--r--   0 root         (0) root         (0)      264 2022-11-05 16:57:46.000000 aa-miningtaxes-1.1.8/miningtaxes/forms.py
--rw-r--r--   0 root         (0) root         (0)     2061 2022-11-03 15:03:29.000000 aa-miningtaxes-1.1.8/miningtaxes/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.414578 aa-miningtaxes-1.1.8/miningtaxes/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.417578 aa-miningtaxes-1.1.8/miningtaxes/management/commands/
--rw-r--r--   0 root         (0) root         (0)      102 2022-10-29 09:17:21.000000 aa-miningtaxes-1.1.8/miningtaxes/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)      233 2022-10-29 11:13:21.000000 aa-miningtaxes-1.1.8/miningtaxes/management/commands/miningtaxes_preload_prices.py
--rw-r--r--   0 root         (0) root         (0)      434 2022-11-22 12:21:22.000000 aa-miningtaxes-1.1.8/miningtaxes/management/commands/miningtaxes_zero_all.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.418578 aa-miningtaxes-1.1.8/miningtaxes/migrations/
--rw-r--r--   0 root         (0) root         (0)      902 2022-11-06 17:28:27.000000 aa-miningtaxes-1.1.8/miningtaxes/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)    15700 2022-11-06 17:28:28.000000 aa-miningtaxes-1.1.8/miningtaxes/migrations/0002_all_models.py
--rw-r--r--   0 root         (0) root         (0)      779 2022-11-08 09:05:56.000000 aa-miningtaxes-1.1.8/miningtaxes/migrations/0003_alter_general_options.py
--rw-r--r--   0 root         (0) root         (0)      939 2022-11-12 04:17:36.000000 aa-miningtaxes-1.1.8/miningtaxes/migrations/0004_settings_interest_rate_alter_settings_phrase.py
--rw-r--r--   0 root         (0) root         (0)      737 2022-11-14 03:13:49.000000 aa-miningtaxes-1.1.8/miningtaxes/migrations/0005_oreprices_raw_price_oreprices_refined_price_and_more.py
--rw-r--r--   0 root         (0) root         (0)      452 2022-11-22 12:29:33.000000 aa-miningtaxes-1.1.8/miningtaxes/migrations/0006_charactertaxcredits_credit_type.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 16:52:52.000000 aa-miningtaxes-1.1.8/miningtaxes/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.418578 aa-miningtaxes-1.1.8/miningtaxes/models/
--rw-r--r--   0 root         (0) root         (0)      399 2022-11-20 04:46:19.000000 aa-miningtaxes-1.1.8/miningtaxes/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6754 2022-11-06 19:16:46.000000 aa-miningtaxes-1.1.8/miningtaxes/models/admin.py
--rw-r--r--   0 root         (0) root         (0)    16180 2022-12-08 04:56:42.000000 aa-miningtaxes-1.1.8/miningtaxes/models/character.py
--rw-r--r--   0 root         (0) root         (0)      712 2022-11-08 03:08:01.000000 aa-miningtaxes-1.1.8/miningtaxes/models/general.py
--rw-r--r--   0 root         (0) root         (0)     3366 2022-11-14 17:38:09.000000 aa-miningtaxes-1.1.8/miningtaxes/models/orePrices.py
--rw-r--r--   0 root         (0) root         (0)     2089 2022-11-12 04:17:36.000000 aa-miningtaxes-1.1.8/miningtaxes/models/settings.py
--rw-r--r--   0 root         (0) root         (0)      246 2022-10-27 10:44:31.000000 aa-miningtaxes-1.1.8/miningtaxes/providers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.414578 aa-miningtaxes-1.1.8/miningtaxes/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.414578 aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.419578 aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/css/
--rw-r--r--   0 root         (0) root         (0)     4582 2022-11-05 13:42:07.000000 aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/css/billboards_dark.css
--rw-r--r--   0 root         (0) root         (0)     4558 2022-11-05 13:42:07.000000 aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/css/billboards_light.css
--rw-r--r--   0 root         (0) root         (0)     1538 2022-10-27 12:54:28.000000 aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/css/global.css
--rw-r--r--   0 root         (0) root         (0)     4331 2022-10-27 12:54:28.000000 aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/css/launcher.css
--rw-r--r--   0 root         (0) root         (0)     1363 2022-10-27 12:54:28.000000 aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/css/miningtaxes.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.419578 aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/images/
--rw-r--r--   0 root         (0) root         (0)    34837 2022-11-19 22:22:28.000000 aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/images/faq1.png
--rw-r--r--   0 root         (0) root         (0)   132605 2022-11-19 22:22:28.000000 aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/images/faq2.png
--rw-r--r--   0 root         (0) root         (0)   342376 2022-11-19 22:22:28.000000 aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/images/faq3.png
--rw-r--r--   0 root         (0) root         (0)   881821 2022-10-27 12:49:53.000000 aa-miningtaxes-1.1.8/miningtaxes/swagger.json
--rw-r--r--   0 root         (0) root         (0)    12185 2022-11-23 21:19:21.000000 aa-miningtaxes-1.1.8/miningtaxes/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.414578 aa-miningtaxes-1.1.8/miningtaxes/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.421578 aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/
--rw-r--r--   0 root         (0) root         (0)     5082 2022-12-11 21:49:11.000000 aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/admin_launcher.html
--rw-r--r--   0 root         (0) root         (0)    20176 2022-12-21 21:25:40.000000 aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/admin_tables.html
--rw-r--r--   0 root         (0) root         (0)     2396 2022-11-28 15:03:03.000000 aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/base.html
--rw-r--r--   0 root         (0) root         (0)     2755 2022-11-05 18:05:41.000000 aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/character_viewer.html
--rw-r--r--   0 root         (0) root         (0)     1740 2022-11-21 01:21:27.000000 aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/faq.html
--rw-r--r--   0 root         (0) root         (0)      480 2022-10-24 21:28:14.000000 aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/index.html
--rw-r--r--   0 root         (0) root         (0)     6466 2022-11-01 15:07:04.000000 aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/launcher.html
--rw-r--r--   0 root         (0) root         (0)     2488 2022-11-22 12:28:46.000000 aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/ore_prices.html
--rw-r--r--   0 root         (0) root         (0)     9758 2022-12-08 11:39:36.000000 aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/user_summary.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.421578 aa-miningtaxes-1.1.8/miningtaxes/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-19 22:43:55.000000 aa-miningtaxes-1.1.8/miningtaxes/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.422578 aa-miningtaxes-1.1.8/miningtaxes/tests/models/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-19 23:50:12.000000 aa-miningtaxes-1.1.8/miningtaxes/tests/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2747 2022-11-21 22:33:02.000000 aa-miningtaxes-1.1.8/miningtaxes/tests/models/test_admin_character.py
--rw-r--r--   0 root         (0) root         (0)     7665 2022-11-22 12:24:37.000000 aa-miningtaxes-1.1.8/miningtaxes/tests/models/test_character.py
--rw-r--r--   0 root         (0) root         (0)     4321 2022-11-20 04:46:58.000000 aa-miningtaxes-1.1.8/miningtaxes/tests/models/test_orePrice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.422578 aa-miningtaxes-1.1.8/miningtaxes/tests/testdata/
--rw-r--r--   0 root         (0) root         (0)     1361 2022-11-21 20:39:23.000000 aa-miningtaxes-1.1.8/miningtaxes/tests/testdata/esi_client_stub.py
--rw-r--r--   0 root         (0) root         (0)     3671 2022-11-20 16:09:12.000000 aa-miningtaxes-1.1.8/miningtaxes/tests/testdata/load_entities.py
--rw-r--r--   0 root         (0) root         (0)      434 2022-11-20 04:51:22.000000 aa-miningtaxes-1.1.8/miningtaxes/tests/testdata/load_eveuniverse.py
--rw-r--r--   0 root         (0) root         (0)     3204 2022-11-21 22:30:35.000000 aa-miningtaxes-1.1.8/miningtaxes/tests/utils.py
--rw-r--r--   0 root         (0) root         (0)     2491 2022-12-08 04:56:42.000000 aa-miningtaxes-1.1.8/miningtaxes/urls.py
--rw-r--r--   0 root         (0) root         (0)    33402 2022-12-20 18:08:37.000000 aa-miningtaxes-1.1.8/miningtaxes/views.py
--rw-r--r--   0 root         (0) root         (0)      252 2022-12-21 21:29:49.423578 aa-miningtaxes-1.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1586 2022-11-23 22:55:27.000000 aa-miningtaxes-1.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.423578 aa-miningtaxes-1.1.8/testauth/
--rw-r--r--   0 root         (0) root         (0)       46 2022-10-24 20:51:10.000000 aa-miningtaxes-1.1.8/testauth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      612 2022-10-24 20:51:10.000000 aa-miningtaxes-1.1.8/testauth/celery.py
--rwxr-xr-x   0 root         (0) root         (0)     9919 2022-11-03 12:24:46.000000 aa-miningtaxes-1.1.8/testauth/settingsAA2.py
--rwxr-xr-x   0 root         (0) root         (0)     9932 2022-11-03 12:24:55.000000 aa-miningtaxes-1.1.8/testauth/settingsAA3.py
--rw-r--r--   0 root         (0) root         (0)      174 2022-10-24 20:51:10.000000 aa-miningtaxes-1.1.8/testauth/urls.py
--rw-r--r--   0 root         (0) root         (0)      397 2022-10-24 20:51:10.000000 aa-miningtaxes-1.1.8/testauth/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 15:07:15.870322 aa-miningtaxes-1.2.4/
+-rw-r--r--   0 root         (0) root         (0)     1070 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      183 2022-11-06 18:50:28.000000 aa-miningtaxes-1.2.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7451 2023-06-18 15:07:15.870322 aa-miningtaxes-1.2.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5740 2023-02-21 19:42:26.000000 aa-miningtaxes-1.2.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 15:07:15.863322 aa-miningtaxes-1.2.4/aa_miningtaxes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7451 2023-06-18 15:07:15.000000 aa-miningtaxes-1.2.4/aa_miningtaxes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2941 2023-06-18 15:07:15.000000 aa-miningtaxes-1.2.4/aa_miningtaxes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-18 15:07:15.000000 aa-miningtaxes-1.2.4/aa_miningtaxes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       75 2023-06-18 15:07:15.000000 aa-miningtaxes-1.2.4/aa_miningtaxes.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-18 15:07:15.000000 aa-miningtaxes-1.2.4/aa_miningtaxes.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 15:07:15.865322 aa-miningtaxes-1.2.4/miningtaxes/
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.4/miningtaxes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       84 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.4/miningtaxes/admin.py
+-rw-r--r--   0 root         (0) root         (0)     1582 2023-02-21 19:10:53.000000 aa-miningtaxes-1.2.4/miningtaxes/app_settings.py
+-rw-r--r--   0 root         (0) root         (0)      200 2022-10-27 10:33:48.000000 aa-miningtaxes-1.2.4/miningtaxes/apps.py
+-rw-r--r--   0 root         (0) root         (0)      912 2022-10-24 21:25:29.000000 aa-miningtaxes-1.2.4/miningtaxes/auth_hooks.py
+-rw-r--r--   0 root         (0) root         (0)     3304 2022-11-07 04:47:52.000000 aa-miningtaxes-1.2.4/miningtaxes/decorators.py
+-rw-r--r--   0 root         (0) root         (0)      264 2022-11-05 16:57:46.000000 aa-miningtaxes-1.2.4/miningtaxes/forms.py
+-rw-r--r--   0 root         (0) root         (0)     2274 2023-03-06 16:38:34.000000 aa-miningtaxes-1.2.4/miningtaxes/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 15:07:15.861322 aa-miningtaxes-1.2.4/miningtaxes/management/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 15:07:15.865322 aa-miningtaxes-1.2.4/miningtaxes/management/commands/
+-rw-r--r--   0 root         (0) root         (0)      102 2022-10-29 09:17:21.000000 aa-miningtaxes-1.2.4/miningtaxes/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      233 2023-01-08 17:44:15.000000 aa-miningtaxes-1.2.4/miningtaxes/management/commands/miningtaxes_preload_prices.py
+-rw-r--r--   0 root         (0) root         (0)      221 2023-04-04 18:04:31.000000 aa-miningtaxes-1.2.4/miningtaxes/management/commands/miningtaxes_update_manual.py
+-rw-r--r--   0 root         (0) root         (0)      434 2022-11-22 12:21:22.000000 aa-miningtaxes-1.2.4/miningtaxes/management/commands/miningtaxes_zero_all.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 15:07:15.866322 aa-miningtaxes-1.2.4/miningtaxes/migrations/
+-rw-r--r--   0 root         (0) root         (0)      902 2022-11-06 17:28:27.000000 aa-miningtaxes-1.2.4/miningtaxes/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)    15700 2022-11-06 17:28:28.000000 aa-miningtaxes-1.2.4/miningtaxes/migrations/0002_all_models.py
+-rw-r--r--   0 root         (0) root         (0)      779 2022-11-08 09:05:56.000000 aa-miningtaxes-1.2.4/miningtaxes/migrations/0003_alter_general_options.py
+-rw-r--r--   0 root         (0) root         (0)      939 2022-11-12 04:17:36.000000 aa-miningtaxes-1.2.4/miningtaxes/migrations/0004_settings_interest_rate_alter_settings_phrase.py
+-rw-r--r--   0 root         (0) root         (0)      737 2022-11-14 03:13:49.000000 aa-miningtaxes-1.2.4/miningtaxes/migrations/0005_oreprices_raw_price_oreprices_refined_price_and_more.py
+-rw-r--r--   0 root         (0) root         (0)      452 2022-11-22 12:29:33.000000 aa-miningtaxes-1.2.4/miningtaxes/migrations/0006_charactertaxcredits_credit_type.py
+-rw-r--r--   0 root         (0) root         (0)      566 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.4/miningtaxes/migrations/0007_character_life_credits_character_life_taxes.py
+-rw-r--r--   0 root         (0) root         (0)      793 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.4/miningtaxes/migrations/0008_character_monthly_credits_json_and_more.py
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.4/miningtaxes/migrations/0009_stats.py
+-rw-r--r--   0 root         (0) root         (0)      405 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.4/miningtaxes/migrations/0010_stats_admin_get_all_activity_json.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 16:52:52.000000 aa-miningtaxes-1.2.4/miningtaxes/migrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 15:07:15.867322 aa-miningtaxes-1.2.4/miningtaxes/models/
+-rw-r--r--   0 root         (0) root         (0)      438 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.4/miningtaxes/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6786 2023-04-05 19:59:43.000000 aa-miningtaxes-1.2.4/miningtaxes/models/admin.py
+-rw-r--r--   0 root         (0) root         (0)    18238 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.4/miningtaxes/models/character.py
+-rw-r--r--   0 root         (0) root         (0)      712 2022-11-08 03:08:01.000000 aa-miningtaxes-1.2.4/miningtaxes/models/general.py
+-rw-r--r--   0 root         (0) root         (0)     3420 2023-02-21 19:11:09.000000 aa-miningtaxes-1.2.4/miningtaxes/models/orePrices.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2022-11-12 04:17:36.000000 aa-miningtaxes-1.2.4/miningtaxes/models/settings.py
+-rw-r--r--   0 root         (0) root         (0)    24599 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.4/miningtaxes/models/stats.py
+-rw-r--r--   0 root         (0) root         (0)      246 2022-10-27 10:44:31.000000 aa-miningtaxes-1.2.4/miningtaxes/providers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 15:07:15.861322 aa-miningtaxes-1.2.4/miningtaxes/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 15:07:15.861322 aa-miningtaxes-1.2.4/miningtaxes/static/miningtaxes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 15:07:15.867322 aa-miningtaxes-1.2.4/miningtaxes/static/miningtaxes/css/
+-rw-r--r--   0 root         (0) root         (0)     4582 2022-11-05 13:42:07.000000 aa-miningtaxes-1.2.4/miningtaxes/static/miningtaxes/css/billboards_dark.css
+-rw-r--r--   0 root         (0) root         (0)     4558 2022-11-05 13:42:07.000000 aa-miningtaxes-1.2.4/miningtaxes/static/miningtaxes/css/billboards_light.css
+-rw-r--r--   0 root         (0) root         (0)     1538 2022-10-27 12:54:28.000000 aa-miningtaxes-1.2.4/miningtaxes/static/miningtaxes/css/global.css
+-rw-r--r--   0 root         (0) root         (0)     4331 2022-10-27 12:54:28.000000 aa-miningtaxes-1.2.4/miningtaxes/static/miningtaxes/css/launcher.css
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-01-20 16:20:09.000000 aa-miningtaxes-1.2.4/miningtaxes/static/miningtaxes/css/miningtaxes.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 15:07:15.868322 aa-miningtaxes-1.2.4/miningtaxes/static/miningtaxes/images/
+-rw-r--r--   0 root         (0) root         (0)    34837 2022-11-19 22:22:28.000000 aa-miningtaxes-1.2.4/miningtaxes/static/miningtaxes/images/faq1.png
+-rw-r--r--   0 root         (0) root         (0)   132605 2022-11-19 22:22:28.000000 aa-miningtaxes-1.2.4/miningtaxes/static/miningtaxes/images/faq2.png
+-rw-r--r--   0 root         (0) root         (0)   342376 2022-11-19 22:22:28.000000 aa-miningtaxes-1.2.4/miningtaxes/static/miningtaxes/images/faq3.png
+-rw-r--r--   0 root         (0) root         (0)   881821 2022-10-27 12:49:53.000000 aa-miningtaxes-1.2.4/miningtaxes/swagger.json
+-rw-r--r--   0 root         (0) root         (0)    13269 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.4/miningtaxes/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 15:07:15.861322 aa-miningtaxes-1.2.4/miningtaxes/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 15:07:15.869322 aa-miningtaxes-1.2.4/miningtaxes/templates/miningtaxes/
+-rw-r--r--   0 root         (0) root         (0)     6817 2023-04-06 01:58:02.000000 aa-miningtaxes-1.2.4/miningtaxes/templates/miningtaxes/admin_launcher.html
+-rw-r--r--   0 root         (0) root         (0)    20648 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.4/miningtaxes/templates/miningtaxes/admin_tables.html
+-rw-r--r--   0 root         (0) root         (0)     2396 2022-11-28 15:03:03.000000 aa-miningtaxes-1.2.4/miningtaxes/templates/miningtaxes/base.html
+-rw-r--r--   0 root         (0) root         (0)     2755 2023-01-08 18:57:41.000000 aa-miningtaxes-1.2.4/miningtaxes/templates/miningtaxes/character_viewer.html
+-rw-r--r--   0 root         (0) root         (0)     1740 2022-11-21 01:21:27.000000 aa-miningtaxes-1.2.4/miningtaxes/templates/miningtaxes/faq.html
+-rw-r--r--   0 root         (0) root         (0)      480 2022-10-24 21:28:14.000000 aa-miningtaxes-1.2.4/miningtaxes/templates/miningtaxes/index.html
+-rw-r--r--   0 root         (0) root         (0)     6466 2022-11-01 15:07:04.000000 aa-miningtaxes-1.2.4/miningtaxes/templates/miningtaxes/launcher.html
+-rw-r--r--   0 root         (0) root         (0)     2488 2022-11-22 12:28:46.000000 aa-miningtaxes-1.2.4/miningtaxes/templates/miningtaxes/ore_prices.html
+-rw-r--r--   0 root         (0) root         (0)    11159 2023-02-21 19:12:52.000000 aa-miningtaxes-1.2.4/miningtaxes/templates/miningtaxes/user_summary.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 15:07:15.869322 aa-miningtaxes-1.2.4/miningtaxes/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-19 22:43:55.000000 aa-miningtaxes-1.2.4/miningtaxes/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 15:07:15.869322 aa-miningtaxes-1.2.4/miningtaxes/tests/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-19 23:50:12.000000 aa-miningtaxes-1.2.4/miningtaxes/tests/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2747 2022-11-21 22:33:02.000000 aa-miningtaxes-1.2.4/miningtaxes/tests/models/test_admin_character.py
+-rw-r--r--   0 root         (0) root         (0)     7665 2022-11-22 12:24:37.000000 aa-miningtaxes-1.2.4/miningtaxes/tests/models/test_character.py
+-rw-r--r--   0 root         (0) root         (0)     4321 2022-11-20 04:46:58.000000 aa-miningtaxes-1.2.4/miningtaxes/tests/models/test_orePrice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 15:07:15.870322 aa-miningtaxes-1.2.4/miningtaxes/tests/testdata/
+-rw-r--r--   0 root         (0) root         (0)     1361 2022-11-21 20:39:23.000000 aa-miningtaxes-1.2.4/miningtaxes/tests/testdata/esi_client_stub.py
+-rw-r--r--   0 root         (0) root         (0)     3671 2022-11-20 16:09:12.000000 aa-miningtaxes-1.2.4/miningtaxes/tests/testdata/load_entities.py
+-rw-r--r--   0 root         (0) root         (0)      434 2022-11-20 04:51:22.000000 aa-miningtaxes-1.2.4/miningtaxes/tests/testdata/load_eveuniverse.py
+-rw-r--r--   0 root         (0) root         (0)     3204 2022-11-21 22:30:35.000000 aa-miningtaxes-1.2.4/miningtaxes/tests/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2900 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.4/miningtaxes/urls.py
+-rw-r--r--   0 root         (0) root         (0)    20830 2023-06-18 15:06:16.000000 aa-miningtaxes-1.2.4/miningtaxes/views.py
+-rw-r--r--   0 root         (0) root         (0)      252 2023-06-18 15:07:15.871322 aa-miningtaxes-1.2.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1586 2022-11-23 22:55:27.000000 aa-miningtaxes-1.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 15:07:15.870322 aa-miningtaxes-1.2.4/testauth/
+-rw-r--r--   0 root         (0) root         (0)       46 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.4/testauth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      612 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.4/testauth/celery.py
+-rwxr-xr-x   0 root         (0) root         (0)     9919 2022-11-03 12:24:46.000000 aa-miningtaxes-1.2.4/testauth/settingsAA2.py
+-rwxr-xr-x   0 root         (0) root         (0)     9932 2022-11-03 12:24:55.000000 aa-miningtaxes-1.2.4/testauth/settingsAA3.py
+-rw-r--r--   0 root         (0) root         (0)      174 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.4/testauth/urls.py
+-rw-r--r--   0 root         (0) root         (0)      397 2022-10-24 20:51:10.000000 aa-miningtaxes-1.2.4/testauth/wsgi.py
```

### Comparing `aa-miningtaxes-1.1.8/LICENSE` & `aa-miningtaxes-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/PKG-INFO` & `aa-miningtaxes-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-miningtaxes
-Version: 1.1.8
+Version: 1.2.4
 Summary: An Alliance Auth app that tracks and applies taxes for mining
 Home-page: https://gitlab.com/arctiru/aa-miningtaxes
 Author: Arc Tiru
 Author-email: arcturusstl@gmail.com
 License: MIT
 Description: # Mining Taxes
         
@@ -79,14 +79,15 @@
         - When a new user joins your corp and adds their character to the plugin, also consider going into the audit tables and providing a tax credit so that it will zero out their past mining activity.
         
         ## Local settings
         
         
         Name | Description | Default
         -- | -- | --
+        MININGTAXES_UNKNOWN_TAX_RATE | The tax rate when a new type of ore is encountered that has not yet been added to the plugin in float (eg 0.10 means 10%) | 0.10
         MININGTAXES_TAX_ONLY_CORP_MOONS | Only tax corporate moons using moon observers as opposed to all moons appearing in the personal mining ledgers. | True
         MININGTAXES_UPDATE_LEDGER_STALE | Minutes after which a character's mining ledger is considered stale | 240
         MININGTAXES_REFINED_RATE | Refining rate for ores. | 0.9063
         MININGTAXES_PRICE_METHOD | By default Fuzzwork API will be used for pricing, if this is set to "Janice" then the Janice API will be used. | Fuzzwork
         MININGTAXES_PRICE_JANICE_API_KEY | The API key to access Janice API. |
         MININGTAXES_PRICE_SOURCE_ID | Station ID for fetching base prices. Supports IDs listed on [Fuzzworks API](https://market.fuzzwork.co.uk/api/). Does not work with Janice API!| 60003760
         MININGTAXES_TAX_CACHE_VIEW_TIMEOUT | Number of seconds before view cache expires. Default is 6 hours. | 21800
```

### Comparing `aa-miningtaxes-1.1.8/README.md` & `aa-miningtaxes-1.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 - When a new user joins your corp and adds their character to the plugin, also consider going into the audit tables and providing a tax credit so that it will zero out their past mining activity.
 
 ## Local settings
 
 
 Name | Description | Default
 -- | -- | --
+MININGTAXES_UNKNOWN_TAX_RATE | The tax rate when a new type of ore is encountered that has not yet been added to the plugin in float (eg 0.10 means 10%) | 0.10
 MININGTAXES_TAX_ONLY_CORP_MOONS | Only tax corporate moons using moon observers as opposed to all moons appearing in the personal mining ledgers. | True
 MININGTAXES_UPDATE_LEDGER_STALE | Minutes after which a character's mining ledger is considered stale | 240
 MININGTAXES_REFINED_RATE | Refining rate for ores. | 0.9063
 MININGTAXES_PRICE_METHOD | By default Fuzzwork API will be used for pricing, if this is set to "Janice" then the Janice API will be used. | Fuzzwork
 MININGTAXES_PRICE_JANICE_API_KEY | The API key to access Janice API. |
 MININGTAXES_PRICE_SOURCE_ID | Station ID for fetching base prices. Supports IDs listed on [Fuzzworks API](https://market.fuzzwork.co.uk/api/). Does not work with Janice API!| 60003760
 MININGTAXES_TAX_CACHE_VIEW_TIMEOUT | Number of seconds before view cache expires. Default is 6 hours. | 21800
```

### Comparing `aa-miningtaxes-1.1.8/aa_miningtaxes.egg-info/PKG-INFO` & `aa-miningtaxes-1.2.4/aa_miningtaxes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-miningtaxes
-Version: 1.1.8
+Version: 1.2.4
 Summary: An Alliance Auth app that tracks and applies taxes for mining
 Home-page: https://gitlab.com/arctiru/aa-miningtaxes
 Author: Arc Tiru
 Author-email: arcturusstl@gmail.com
 License: MIT
 Description: # Mining Taxes
         
@@ -79,14 +79,15 @@
         - When a new user joins your corp and adds their character to the plugin, also consider going into the audit tables and providing a tax credit so that it will zero out their past mining activity.
         
         ## Local settings
         
         
         Name | Description | Default
         -- | -- | --
+        MININGTAXES_UNKNOWN_TAX_RATE | The tax rate when a new type of ore is encountered that has not yet been added to the plugin in float (eg 0.10 means 10%) | 0.10
         MININGTAXES_TAX_ONLY_CORP_MOONS | Only tax corporate moons using moon observers as opposed to all moons appearing in the personal mining ledgers. | True
         MININGTAXES_UPDATE_LEDGER_STALE | Minutes after which a character's mining ledger is considered stale | 240
         MININGTAXES_REFINED_RATE | Refining rate for ores. | 0.9063
         MININGTAXES_PRICE_METHOD | By default Fuzzwork API will be used for pricing, if this is set to "Janice" then the Janice API will be used. | Fuzzwork
         MININGTAXES_PRICE_JANICE_API_KEY | The API key to access Janice API. |
         MININGTAXES_PRICE_SOURCE_ID | Station ID for fetching base prices. Supports IDs listed on [Fuzzworks API](https://market.fuzzwork.co.uk/api/). Does not work with Janice API!| 60003760
         MININGTAXES_TAX_CACHE_VIEW_TIMEOUT | Number of seconds before view cache expires. Default is 6 hours. | 21800
```

### Comparing `aa-miningtaxes-1.1.8/aa_miningtaxes.egg-info/SOURCES.txt` & `aa-miningtaxes-1.2.4/aa_miningtaxes.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,28 +19,34 @@
 miningtaxes/providers.py
 miningtaxes/swagger.json
 miningtaxes/tasks.py
 miningtaxes/urls.py
 miningtaxes/views.py
 miningtaxes/management/commands/__init__.py
 miningtaxes/management/commands/miningtaxes_preload_prices.py
+miningtaxes/management/commands/miningtaxes_update_manual.py
 miningtaxes/management/commands/miningtaxes_zero_all.py
 miningtaxes/migrations/0001_initial.py
 miningtaxes/migrations/0002_all_models.py
 miningtaxes/migrations/0003_alter_general_options.py
 miningtaxes/migrations/0004_settings_interest_rate_alter_settings_phrase.py
 miningtaxes/migrations/0005_oreprices_raw_price_oreprices_refined_price_and_more.py
 miningtaxes/migrations/0006_charactertaxcredits_credit_type.py
+miningtaxes/migrations/0007_character_life_credits_character_life_taxes.py
+miningtaxes/migrations/0008_character_monthly_credits_json_and_more.py
+miningtaxes/migrations/0009_stats.py
+miningtaxes/migrations/0010_stats_admin_get_all_activity_json.py
 miningtaxes/migrations/__init__.py
 miningtaxes/models/__init__.py
 miningtaxes/models/admin.py
 miningtaxes/models/character.py
 miningtaxes/models/general.py
 miningtaxes/models/orePrices.py
 miningtaxes/models/settings.py
+miningtaxes/models/stats.py
 miningtaxes/static/miningtaxes/css/billboards_dark.css
 miningtaxes/static/miningtaxes/css/billboards_light.css
 miningtaxes/static/miningtaxes/css/global.css
 miningtaxes/static/miningtaxes/css/launcher.css
 miningtaxes/static/miningtaxes/css/miningtaxes.css
 miningtaxes/static/miningtaxes/images/faq1.png
 miningtaxes/static/miningtaxes/images/faq2.png
```

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/app_settings.py` & `aa-miningtaxes-1.2.4/miningtaxes/app_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 MININGTAXES_TASKS_TIME_LIMIT = clean_setting("MININGTAXES_TASKS_TIME_LIMIT", 7200)
 """Global timeout for tasks in seconds to reduce task accumulation during outages."""
 
 MININGTAXES_REFINED_RATE = clean_setting("MININGTAXES_REFINED_RATE", 0.9063)
 """Refining rate for ores."""
 
+MININGTAXES_UNKNOWN_TAX_RATE = 0.10
 
 MININGTAXES_PRICE_SOURCE_ID = clean_setting("MININGTAXES_PRICE_SOURCE_ID", 60003760)
 
 MININGTAXES_PRICE_SOURCE_NAME = clean_setting("MININGTAXES_PRICE_SOURCE_NAME", "Jita")
 
 MININGTAXES_PRICE_METHOD = clean_setting("MININGTAXES_PRICE_METHOD", "Fuzzwork")
```

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/auth_hooks.py` & `aa-miningtaxes-1.2.4/miningtaxes/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/decorators.py` & `aa-miningtaxes-1.2.4/miningtaxes/decorators.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/migrations/0001_initial.py` & `aa-miningtaxes-1.2.4/miningtaxes/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/migrations/0002_all_models.py` & `aa-miningtaxes-1.2.4/miningtaxes/migrations/0002_all_models.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/migrations/0003_alter_general_options.py` & `aa-miningtaxes-1.2.4/miningtaxes/migrations/0003_alter_general_options.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/migrations/0004_settings_interest_rate_alter_settings_phrase.py` & `aa-miningtaxes-1.2.4/miningtaxes/migrations/0004_settings_interest_rate_alter_settings_phrase.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/migrations/0005_oreprices_raw_price_oreprices_refined_price_and_more.py` & `aa-miningtaxes-1.2.4/miningtaxes/migrations/0005_oreprices_raw_price_oreprices_refined_price_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/models/admin.py` & `aa-miningtaxes-1.2.4/miningtaxes/models/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             structinfo = esi.client.Universe.get_universe_structures_structure_id(
                 structure_id=entry["observer_id"],
                 token=token.valid_access_token(),
             ).results()
             structname = ""
             sys = None
             if type(structinfo) == dict:
-                structname = structinfo["name"]
+                structname = structinfo["name"][0:32]  # fix for names too long
                 sys, _ = EveSolarSystem.objects.get_or_create_esi(
                     id=structinfo["solar_system_id"]
                 )
             else:
                 logger.error("Wrong struct info for: %d" % entry["observer_id"])
                 logger.error(structinfo)
                 continue
```

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/models/character.py` & `aa-miningtaxes-1.2.4/miningtaxes/models/character.py`

 * *Files 6% similar despite different names*

```diff
@@ -200,14 +200,20 @@
             return True
 
         deadline = now() - self.update_time_until_stale()
         return update_status.started_at < deadline
 
 
 class Character(CharacterAbstract):
+    life_credits = models.FloatField(default=0.0)
+    life_taxes = models.FloatField(default=0.0)
+    monthly_mining_json = models.JSONField(default=None, null=True)
+    monthly_taxes_json = models.JSONField(default=None, null=True)
+    monthly_credits_json = models.JSONField(default=None, null=True)
+
     @fetch_token_for_character("esi-industry.read_character_mining.v1")
     def update_mining_ledger(self, token: Token):
         """Update mining ledger from ESI for this character."""
         logger.info("%s: Fetching mining ledger from ESI", self)
         entries = esi.client.Industry.get_characters_character_id_mining(
             character_id=self.eve_character.character_id,
             token=token.valid_access_token(),
@@ -225,84 +231,141 @@
             (row, _) = self.mining_ledger.update_or_create(
                 date=entry["date"],
                 eve_solar_system=eve_solar_system,
                 eve_type=eve_type,
                 defaults={"quantity": entry["quantity"]},
             )
             row.calc_prices()
+        self.calc_lifetime_taxes()
+        self.calc_monthly_taxes()
+        self.calc_monthly_mining()
 
     @classmethod
     def get_esi_scopes(cls) -> list:
         return [
             "esi-industry.read_character_mining.v1",
         ]
 
-    def standardize(self, months):
+    def json_standardize(self, months):
         newmonths = {}
         for h in months:
             if type(h["month"]) == dt.datetime:
-                h["month"] = h["month"].date()
+                h["month"] = str(h["month"].date())
+            else:
+                h["month"] = str(h["month"])
             newmonths[h["month"]] = h["total"]
         return newmonths
 
-    def get_lifetime_taxes(self):
+    def standardize(self, months):
+        newmonths = {}
+        for k in months.keys():
+            kn = dt.datetime.strptime(k, "%Y-%m-%d").date()
+            newmonths[kn] = months[k]
+        return newmonths
+
+    def calc_lifetime_taxes(self):
         amount = self.mining_ledger.all().aggregate(Sum("taxes_owed"))[
             "taxes_owed__sum"
         ]
         if amount is None:
             amount = 0.0
-        return round(amount, 2)
+        self.life_taxes = amount
+        self.save()
 
-    def get_lifetime_credits(self):
+    def calc_lifetime_credits(self):
         amount = self.tax_credits.all().aggregate(Sum("credit"))["credit__sum"]
         if amount is None:
             amount = 0.0
-        return round(amount, 2)
+        self.life_credits = amount
+        self.save()
 
-    def get_monthly_taxes(self):
-        return self.standardize(
+    def get_lifetime_taxes(self):
+        if self.life_taxes == 0.0:
+            self.calc_lifetime_taxes()
+        return round(self.life_taxes, 2)
+
+    def get_lifetime_credits(self):
+        if self.life_credits == 0.0:
+            self.calc_lifetime_credits()
+        return round(self.life_credits, 2)
+
+    def calc_monthly_taxes(self):
+        dat = (
             self.mining_ledger.all()
             .annotate(month=TruncMonth("date"))
             .values("month")
             .annotate(total=Sum("taxes_owed"))
             .order_by("month")
         )
 
-    def get_monthly_credits(self):
-        return self.standardize(
+        self.monthly_taxes_json = self.json_standardize(dat)
+        self.save()
+
+    def get_monthly_taxes(self):
+        if self.monthly_taxes_json is None:
+            self.calc_monthly_taxes()
+        return self.standardize(self.monthly_taxes_json)
+
+    def calc_monthly_credits(self):
+        dat = (
             self.tax_credits.all()
             .annotate(month=TruncMonth("date"))
             .values("month")
             .annotate(total=Sum("credit"))
             .order_by("month")
         )
 
-    def get_monthly_mining(self):
-        return self.standardize(
+        self.monthly_credits_json = self.json_standardize(dat)
+        self.save()
+
+    def get_monthly_credits(self):
+        if self.monthly_credits_json is None:
+            self.calc_monthly_credits()
+        return self.standardize(self.monthly_credits_json)
+
+    def calc_monthly_mining(self):
+        dat = (
             self.mining_ledger.all()
             .annotate(month=TruncMonth("date"))
             .values("month")
             .annotate(total=Sum("taxed_value"))
             .order_by("month")
         )
 
+        self.monthly_mining_json = self.json_standardize(dat)
+        self.save()
+
+    def get_monthly_mining(self):
+        if self.monthly_mining_json is None:
+            self.calc_monthly_mining()
+        return self.standardize(self.monthly_mining_json)
+
     def get_90d_mining(self):
         b = now().date() - dt.timedelta(days=90)
         return self.mining_ledger.filter(date__gte=b)
 
     def last_paid(self):
         dt = self.tax_credits.last()
         if dt is None:
             return None
         return dt.date
 
     def give_credit(self, isk, credit_type):
         if credit_type not in ("credit", "paid", "interest"):
             raise Exception("Unknown credit type")
         self.tax_credits.create(date=now(), credit=isk, credit_type=credit_type)
+        self.calc_lifetime_credits()
+        self.calc_monthly_credits()
+
+    def precalc_all(self):
+        self.calc_lifetime_taxes()
+        self.calc_lifetime_credits()
+        self.calc_monthly_taxes()
+        self.calc_monthly_credits()
+        self.calc_monthly_mining()
 
 
 class CharacterTaxCredits(models.Model):
     character = models.ForeignKey(
         Character, on_delete=models.CASCADE, related_name="tax_credits"
     )
     date = models.DateTimeField(db_index=True)
```

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/models/general.py` & `aa-miningtaxes-1.2.4/miningtaxes/models/general.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/models/orePrices.py` & `aa-miningtaxes-1.2.4/miningtaxes/models/orePrices.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 from django.db import models
 from eveuniverse.models import EveType, EveTypeMaterial
 
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.logging import LoggerAddTag
 
 from .. import __title__
-from ..app_settings import MININGTAXES_REFINED_RATE
+from ..app_settings import MININGTAXES_REFINED_RATE, MININGTAXES_UNKNOWN_TAX_RATE
 from ..helpers import PriceGroups
 from .settings import Settings
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
 def get_tax(eve_type):
     settings = Settings.load()
     pg = PriceGroups()
     if eve_type.eve_group_id not in pg.taxgroups:
         logger.debug(
             "Unknown evetype for %s, group: %d" % (eve_type, eve_type.eve_group_id)
         )
-        return 0.10
+        return MININGTAXES_UNKNOWN_TAX_RATE
     group = "tax_" + pg.taxgroups[eve_type.eve_group_id]
     return settings.__dict__[group] / 100.0
 
 
 def ore_calc_prices(eve_type, q):
     try:
         ore = OrePrices.objects.get(eve_type=eve_type)
```

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/models/settings.py` & `aa-miningtaxes-1.2.4/miningtaxes/models/settings.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/css/billboards_dark.css` & `aa-miningtaxes-1.2.4/miningtaxes/static/miningtaxes/css/billboards_dark.css`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/css/billboards_light.css` & `aa-miningtaxes-1.2.4/miningtaxes/static/miningtaxes/css/billboards_light.css`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/css/global.css` & `aa-miningtaxes-1.2.4/miningtaxes/static/miningtaxes/css/global.css`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/css/launcher.css` & `aa-miningtaxes-1.2.4/miningtaxes/static/miningtaxes/css/launcher.css`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/css/miningtaxes.css` & `aa-miningtaxes-1.2.4/miningtaxes/static/miningtaxes/css/miningtaxes.css`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,34 @@
 /* Common styles for all pages of this app */
+
+.item-icon-button{
+  height: 25px;
+}
+.item-icon{
+  top: -10px !important;
+}
+
 @media all {
     .icon-plus-name {
         padding-left: 2em;
         text-indent: -2em;
     }
 
     .text-high-sec {
         color: rgb(0, 128, 0);
     }
 
+    .text-green {
+        color: rgb(50, 154, 50);
+    }
+
+    .text-red {
+        color: rgb(255, 60, 60);
+    }
+
     .text-low-sec {
         color: rgb(255, 165, 0);
     }
 
     .text-null-sec {
         color: rgb(255, 0, 0);
     }
```

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/images/faq1.png` & `aa-miningtaxes-1.2.4/miningtaxes/static/miningtaxes/images/faq1.png`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/images/faq2.png` & `aa-miningtaxes-1.2.4/miningtaxes/static/miningtaxes/images/faq2.png`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/images/faq3.png` & `aa-miningtaxes-1.2.4/miningtaxes/static/miningtaxes/images/faq3.png`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/swagger.json` & `aa-miningtaxes-1.2.4/miningtaxes/swagger.json`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/tasks.py` & `aa-miningtaxes-1.2.4/miningtaxes/tasks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from datetime import date
-
 import requests
 from celery import shared_task
 
 from django.db import Error
+from django.http.response import Http404
 from django.shortcuts import get_object_or_404
 from django.utils import timezone
-from django.utils.timezone import now
+from eveuniverse.models import EveType, EveTypeMaterial
 
 from allianceauth.eveonline.models import EveCharacter
 from allianceauth.notifications import notify
 from allianceauth.services.hooks import get_extension_logger
 
 from .app_settings import (
     MININGTAXES_PRICE_JANICE_API_KEY,
@@ -24,41 +23,24 @@
 from .models import (
     AdminCharacter,
     AdminMiningCorpLedgerEntry,
     AdminMiningObsLog,
     Character,
     OrePrices,
     Settings,
+    Stats,
 )
 
 logger = get_extension_logger(__name__)
 TASK_DEFAULT_KWARGS = {"time_limit": MININGTAXES_TASKS_TIME_LIMIT, "max_retries": 3}
 
 
 def calctaxes():
-    n = now().date()
-    curmonth = date(year=n.year, month=n.month, day=1)
-    user2taxes = {}
-    characters = Character.objects.all()
-    for character in characters:
-        taxes = character.get_monthly_taxes()
-        total = 0.0
-        for k in taxes.keys():
-            if k != curmonth:
-                total += taxes[k]
-        if character.user not in user2taxes:
-            user2taxes[character.user] = [0.0, 0.0, character]
-        user2taxes[character.user][0] += total
-        if total > user2taxes[character.user][1]:
-            user2taxes[character.user][1] = total
-            user2taxes[character.user][2] = character
-        credits = character.get_lifetime_credits()
-        user2taxes[character.user][0] -= credits
-
-    return user2taxes
+    s = Stats.load()
+    return s.calctaxes()
 
 
 @shared_task(**{**TASK_DEFAULT_KWARGS, **{"bind": True}})
 def notify_taxes_due(self):
     user2taxes = calctaxes()
 
     for u in user2taxes.keys():
@@ -97,14 +79,19 @@
     for character in characters:
         update_admin_character(character_pk=character.id, celery=True)
     characters = Character.objects.all()
     for character in characters:
         update_character(character_pk=character.id, celery=True)
     add_corp_moon_taxes()
     add_tax_credits()
+    # precalc all characters
+    for character in characters:
+        character.precalc_all()
+    s = Stats.load()
+    s.precalc_all()
 
 
 def valid_janice_api_key():
     c = requests.get(
         "https://janice.e-351.com/api/rest/v2/markets",
         headers={
             "Content-Type": "text/plain",
@@ -159,14 +146,32 @@
     type_ids = []
     market_data = {}
     api_up = True
 
     # Get all type ids
     prices = PriceGroups().items
 
+    # Update EveUniverse objects
+    matset = set()
+    for item in prices:
+        EveType.objects.update_or_create_esi(
+            id=item.id,
+            enabled_sections=EveType.Section.TYPE_MATERIALS,
+            include_children=True,
+            wait_for_children=True,
+        )
+        EveTypeMaterial.objects.update_or_create_api(eve_type=item)
+
+        materials = EveTypeMaterial.objects.filter(
+            eve_type_id=item.id
+        ).prefetch_related("eve_type")
+        for mat in materials:
+            mat = mat.material_eve_type
+            matset.add(mat.id)
+
     if MININGTAXES_PRICE_METHOD == "Fuzzwork":
         logger.debug(
             "Price setup starting for %s items from Fuzzworks API from station id %s (%s), this may take up to 30 seconds..."
             % (
                 len(prices),
                 MININGTAXES_PRICE_SOURCE_ID,
                 MININGTAXES_PRICE_SOURCE_NAME,
@@ -206,14 +211,16 @@
         existing = OrePrices.objects.all()
         toupdate = []
         tocreate = []
         for price in prices:
             if not str(price.id) in market_data:
                 logger.debug(f"Missing data on {price}")
                 continue
+            if price.id in matset:
+                continue
             buy = int(float(market_data[str(price.id)]["buy"]["max"]))
             sell = int(float(market_data[str(price.id)]["sell"]["min"]))
             now = timezone.now()
 
             found = None
             for e in existing:
                 if price.id == e.eve_type.id:
@@ -224,14 +231,43 @@
                 found.sell = sell
                 found.updated = now
                 toupdate.append(found)
             else:
                 tocreate.append(
                     OrePrices(eve_type_id=price.id, buy=buy, sell=sell, updated=now)
                 )
+
+        # Handling refined material prices
+        logger.debug("Materials price updating...")
+        type_ids = list(matset)
+        market_data = {}
+        market_data.update(get_bulk_prices(type_ids))
+        for mat in matset:
+            if not str(mat) in market_data:
+                logger.debug(f"Missing data on {mat}")
+                continue
+            buy = int(float(market_data[str(mat)]["buy"]["max"]))
+            sell = int(float(market_data[str(mat)]["sell"]["min"]))
+            now = timezone.now()
+
+            found = None
+            for e in existing:
+                if mat == e.eve_type.id:
+                    found = e
+                    break
+            if found is not None:
+                found.buy = buy
+                found.sell = sell
+                found.updated = now
+                toupdate.append(found)
+            else:
+                tocreate.append(
+                    OrePrices(eve_type_id=mat, buy=buy, sell=sell, updated=now)
+                )
+
         logger.debug("Objects to be created: %d" % len(tocreate))
         logger.debug("Objects to be updated: %d" % len(toupdate))
         try:
             OrePrices.objects.bulk_create(tocreate)
             OrePrices.objects.bulk_update(toupdate, ["buy", "sell", "updated"])
             logger.debug("All prices succesfully updated")
         except Error as e:
@@ -283,25 +319,24 @@
     characters = AdminCharacter.objects.all()
     phrase = settings.phrase.lower().strip()
     for character in characters:
         entries = character.corp_ledger.all()
         for entry in entries:
             if phrase != "" and phrase not in entry.reason.lower():
                 continue
-            payee = None
             try:
                 payee = get_object_or_404(
                     Character,
                     eve_character_id=EveCharacter.objects.get(
                         character_id=entry.taxed_id
                     ).pk,
                 )
             except EveCharacter.DoesNotExist:
-                pass
-            if payee is None:
+                continue
+            except Http404:
                 continue
             payee.tax_credits.update_or_create(
                 date=entry.date, credit=entry.amount, defaults={"credit_type": "paid"}
             )
 
 
 def add_tax_credits_by_char(character):
```

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/admin_launcher.html` & `aa-miningtaxes-1.2.4/miningtaxes/templates/miningtaxes/launcher.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,58 @@
 {% extends 'miningtaxes/base.html' %}
 {% load i18n %}
 {% load static %}
 {% load humanize %}
 {% load evelinks %}
-{% load bootstrap %}
 
 {% block details %}
+
     <div class="panel panel-default">
         <div class="panel-heading" style="display:flex;">
-		<h3 class="panel-title">{% translate 'MiningTaxes Settings' %} (v{{ version }})</h3>
-        </div>
-        <div class="panel-body">
-	    <form class="form" action="{{ url }}" method="POST">
-		    {% csrf_token %}
-		    {{ form|bootstrap }}
-		    <button type="submit" class="btn btn-primary">Edit Settings</button>
-	    </form>
-	</div>
-    </div>
-    <div class="panel panel-default">
-        <div class="panel-heading" style="display:flex;">
-            <h3 class="panel-title">{% translate 'Accountant Characters (add only one accountant per corp)' %}</h3>
+            <h3 class="panel-title">{% translate 'Characters' %}</h3>
         </div>
         <div class="panel-body">
             <!-- Characters -->
             <div class="character-cards">
                 <ul class="cards_container">
                     <!-- Add New Character -->
                     <li class="cards_item">
                         <div class="card">
                             <div class="card-header">{% translate 'Register Character' %}</div>
 
                             <div class="card-body card__content">
-                                <a href="{% url 'miningtaxes:add_admin_character' %}">
+                                <a href="{% url 'miningtaxes:add_character' %}">
                                     <img src="{{ 1|character_portrait_url:256 }}" alt="Add character">
                                 </a>
                             </div>
 
                             <div class="card-footer">
-                                <a class="btn btn-primary btn-sm" href="{% url 'miningtaxes:add_admin_character' %}">{% translate 'Register' %}</a>
+                                <a class="btn btn-primary btn-sm" href="{% url 'miningtaxes:add_character' %}">{% translate 'Register' %}</a>
                             </div>
                         </div>
                     </li>
 
                     {% if has_registered_characters %}
                         <!-- Registered Characters -->
                         {% for auth_character in auth_characters|dictsort:"character_name" %}
                             <li class="cards_item">
                                 <div class="card">
                                     <div class="card-header">
                                         {{ auth_character.character_name }}
+                                        {% if auth_character.character_id == main_character_id %}
+                                            &nbsp;<i class="fas fa-crown" title="Main character"></i>
+                                        {% endif %}
+                                        {% if auth_character.character.is_shared %}
+                                            &nbsp;<i class="far fa-eye" title="Currently shared with recruiters"></i>
+                                        {% endif %}
                                     </div>
+
                                     <div class="card-body card__content">
                                         <p>
-					<a href="">
+                                            <a href="{% url 'miningtaxes:character_viewer' auth_character.character.pk %}">
                                                 <span class="aa-miningtaxes-launcher-character-image">
                                                     <img src="{{ auth_character.character_id|character_portrait_url:256 }}" alt="{{ auth_character.character_name }}">
 
                                                     {% if auth_character.alliance_id %}
                                                         <span class="aa-miningtaxes-alliance-logo">
                                                             <img class="" src="{{ auth_character.alliance_id|alliance_logo_url:64 }}" title="{{ auth_character.alliance_name }}">
                                                         </span>
@@ -67,36 +62,60 @@
                                                         <img class="" src="{{ auth_character.corporation_id|corporation_logo_url:64 }}" title="{{ auth_character.corporation_name }}">
                                                     </span>
                                                 </span>
                                             </a>
                                         </p>
 
                                         <div class="text-center">
+                                            <br>
+                                            {% if auth_character.character.wallet_balance %}
+                                                {{ auth_character.character.wallet_balance.total|intword|default_if_none:"-" }} ISK<br>
+                                            {% else %}
+                                                <span class="text-muted">{% translate "(no data yet)" %}</span>
+                                            {% endif %}
+
                                         </div>
                                     </div>
 
                                     <div class="card-footer">
-                                        <a class="btn btn-danger btn-sm" href="{% url 'miningtaxes:remove_admin_character' auth_character.character.pk %}"
+                                        <a class="btn btn-success btn-sm" href="{% url 'miningtaxes:character_viewer' auth_character.character.pk %}"
+                                            role="button" title="{% translate 'View this character.' %}">
+                                            <i class="fas fa-sign-in-alt"></i>
+                                        </a>
+
+                                        <a class="btn btn-danger btn-sm" href="{% url 'miningtaxes:remove_character' auth_character.character.pk %}"
                                             role="button" title="{% translate 'Remove this character.' %}"
                                             onclick="return confirm('Are you sure you want to REMOVE this character?')">
                                             <i class="far fa-trash-alt"></i>
                                         </a>
                                     </div>
                                 </div>
                             </li>
                         {% endfor %}
                     {% endif %}
                 </ul>
             </div>
+
+            {% if unregistered_chars|length > 0 %}
+                <p class="text-warning">
+                    <strong>
+                    <i class="fas fa-exclamation-triangle"></i>
+                    {% translate 'Unregistered character(s):' %}&nbsp;&nbsp;</strong>
+                    {{ unregistered_chars|join:", " }}
+                </p>
+            {% endif %}
+
         </div>
     </div>
 
-
 {% endblock details %}
 
+{% block extra_javascript %}
+{% endblock %}
+
 {% block extra_css %}
     <link rel="stylesheet" href="{% static 'miningtaxes/css/global.css' %}" type="text/css">
     <link rel="stylesheet" href="{% static 'miningtaxes/css/miningtaxes.css' %}" type="text/css">
     <link rel="stylesheet" href="{% static 'miningtaxes/css/launcher.css' %}" type="text/css">
 {% endblock %}
 
 {% block extra_script %}
```

#### html2text {}

```diff
@@ -1,20 +1,30 @@
 {% extends 'miningtaxes/base.html' %} {% load i18n %} {% load static %} {% load
-humanize %} {% load evelinks %} {% load bootstrap %} {% block details %}
-**** {% translate 'MiningTaxes Settings' %} (v{{ version }}) ****
-{% csrf_token %} {{ form|bootstrap }} Edit Settings
-**** {% translate 'Accountant Characters (add only one accountant per corp)' %}
-****
+humanize %} {% load evelinks %} {% block details %}
+**** {% translate 'Characters' %} ****
     * {% translate 'Register Character' %}
       [Add_character]
       {%_translate_'Register'_%}
     * {% if has_registered_characters %}  {% for auth_character in
       auth_characters|dictsort:"character_name" %}
-    * {{ auth_character.character_name }}
-       [{{ auth_character.character_name }}] {% if auth_character.alliance_id
-      %}  [{{ auth_character.alliance_id|alliance_logo_url:64 }}]  {% endif %}
-      [{{ auth_character.corporation_id|corporation_logo_url:64 }}]
+    * {{ auth_character.character_name }} {% if auth_character.character_id ==
+      main_character_id %}   {% endif %} {% if
+      auth_character.character.is_shared %}   {% endif %}
+      _[{{_auth_character.character_name_}}]_{%_if_auth_character.alliance_id
+      %}__[{{_auth_character.alliance_id|alliance_logo_url:64_}}]__{%_endif_%}
+      [{{_auth_character.corporation_id|corporation_logo_url:64_}}]__
+
+      {% if auth_character.character.wallet_balance %} {
+      { auth_character.character.wallet_balance.total|intword|default_if_none:
+      "-" }} ISK
+      {% else %} {% translate "(no data yet)" %} {% endif %}
+
     * {% endfor %} {% endif %}
-{% endblock details %} {% block extra_css %}
+{% if unregistered_chars|length > 0 %}
+ {% translate 'Unregistered character(s):' %}  
+ {{ unregistered_chars|join:", " }}
+{% endif %}
+{% endblock details %} {% block extra_javascript %} {% endblock %} {% block
+extra_css %}
 
 
  {% endblock %} {% block extra_script %} {% endblock %}
```

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/admin_tables.html` & `aa-miningtaxes-1.2.4/miningtaxes/templates/miningtaxes/admin_tables.html`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,16 @@
 			<div class="panel-body">
     <div class="table-responsive">
         <table class="table table-striped table-width-fix" id="mains">
             <thead>
                 <tr>
                     <th>{% translate 'Name' %}</th>
                     <th>{% translate 'Corp' %}</th>
-                    <th>{% translate 'Balance' %}</th>
+                    <th>{% translate 'Taxes Past Due' %}</th>
+                    <th>{% translate 'Current Balance' %}</th>
                     <th>{% translate 'Last Paid' %}</th>
 		    <th>{% translate 'Actions' %}</th>
                 </tr>
             </thead>
             <tbody></tbody>
         </table>
     </div>
@@ -204,17 +205,17 @@
 	</div>
 </div>
 
 <div class="row">
 	<div class="col-md-12">
     		<div class="panel panel-default">
 			<div class="panel-heading" style="display:flex;">
-				<button class="btn btn-default" onclick="prior()"><span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span></button>
+				<button class="btn btn-default item-icon-button" onclick="prior()"><span class="glyphicon glyphicon-chevron-left item-icon" aria-hidden="true"></span></button>
 				<h3 class="panel-title"><span id='sys_month_disp'></span></h3>
-				<button class="btn btn-default" onclick="next()"><span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span></button>
+				<button class="btn btn-default item-icon-button" onclick="next()"><span class="glyphicon glyphicon-chevron-right item-icon" aria-hidden="true"></span></button>
 			</div>
 			<div class="panel-body">
 			    <div class="table-responsive">
 
 				<table class="table table-striped table-width-fix" id="sys_month">
 				    <thead>
 					<tr>
@@ -245,14 +246,15 @@
 			</div>
 			<div class="panel-body">
 			    <div class="table-responsive">
 				<table class="table table-striped table-width-fix" id="unregistered">
 				    <thead>
 					<tr>
 					    <th>{% translate 'Name' %}</th>
+					    <th>{% translate 'System' %}</th>
 					    <th>{% translate 'Approx. ISK' %}</th>
 					    <th>{% translate 'Ore Units' %}</th>
 					    <th>{% translate 'Last Mined' %}</th>
 					</tr>
 				    </thead>
 				    <tbody></tbody>
 				</table>
@@ -267,14 +269,15 @@
 			</div>
 			<div class="panel-body">
 			    <div class="table-responsive">
 				<table class="table table-striped table-width-fix" id="unknown">
 				    <thead>
 					<tr>
 					    <th>{% translate 'Name' %}</th>
+					    <th>{% translate 'System' %}</th>
 					    <th>{% translate 'Approx. ISK' %}</th>
 					    <th>{% translate 'Ore Units' %}</th>
 					    <th>{% translate 'Last Mined' %}</th>
 					</tr>
 				    </thead>
 				    <tbody></tbody>
 				</table>
@@ -351,15 +354,17 @@
 		if (pane == "#sys_stats") { draw_sys_stats(); }
 		if (pane == "#corp_moons") { draw_corp_moons(); }
 		firstdraw[pane] = false;
 	}
 }
 
 function exportsysdata() {
-        exportToCsv("miningtaxes-allactivity.csv", tax_sys_data);
+$.get("{% url 'miningtaxes:admin_get_all_activity_json' %}", function(d) {
+        exportToCsv("miningtaxes-allactivity.csv", d.data);
+});
 }
 
 
 function exporttaxdata() {
         exportToCsv("miningtaxes-revenue.csv", tax_csv_data);
 }
 
@@ -415,40 +420,42 @@
 	$("#creditbox").val(bal);
 }
 function draw_corp_moons() {
 	$.getJSON("{% url 'miningtaxes:admin_corp_mining_history' %}", function (d) {
 		unregistered_table = $('#unregistered').DataTable({
 		    columns: [
 			{ data: 'name' },
+			{ data: 'sys' },
 			{
 			    data: 'isk',
 			    render: $.fn.dataTable.render.number(',', '.', 2)
 			},
 			{
 			    data: 'quantity',
 			    render: $.fn.dataTable.render.number(',', '.', 0)
 			},
 			{ data: 'last' },
 		    ],
-		    order: [[3, "desc"]]
+		    order: [[4, "desc"]]
 		});
 		unknown_table = $('#unknown').DataTable({
 		    columns: [
 			{ data: 'name' },
+			{ data: 'sys' },
 			{
 			    data: 'isk',
 			    render: $.fn.dataTable.render.number(',', '.', 2)
 			},
 			{
 			    data: 'quantity',
 			    render: $.fn.dataTable.render.number(',', '.', 0)
 			},
 			{ data: 'last' },
 		    ],
-		    order: [[3, "desc"]]
+		    order: [[4, "desc"]]
 		});
 		corpmoon_table = $('#corpmoon').DataTable({
 		    columns: [
 			{ data: 'date' },
 			{ data: 'name' },
 			{ data: 'ore' },
 			{
@@ -602,20 +609,19 @@
 						  },
 						  },
 						  bindto:"#sys_avg_q"
 							  });
 							  isk.load({columns: d['anal']['q']});
 
 
-tax_sys_data = d["csv"];
-$("#syscsv").click(exportsysdata);
 			 });
 			 }
 
 $(document).ready(function () {
+	$("#syscsv").click(exportsysdata);
 	$.getJSON("{% url 'miningtaxes:admin_tax_revenue_json' %}", function (d) {
 		var taxrevenue = bb.generate({
 			data: {
 				x: "x",
 				columns: [],
 				axes: { isk: "y"},
 				type: "bar",
@@ -666,14 +672,15 @@
 				},
 			},
 			bindto:"#isk"
 		});
 		for (var i = 0 ; i < d["ydata"].length; i++) {
 			iskchart.load({columns: [d['xdata'], d['ydata'][i]]});
 		}
+		iskchart.focus(["all"]);
 		csv_data = d["csv"];
 		$("#csv").click(exportdata);
 		} );
 	$.getJSON("{% url 'miningtaxes:admin_main_json' %}", function (d) {
 		user_data = d["data"];
 		user_data.forEach( function(row) {
 			user_table.row.add(row);
@@ -681,14 +688,18 @@
 		user_table.draw();
 	});
         user_table = $('#mains').DataTable({
             columns: [
                 { data: 'name' },
                 { data: 'corp' },
                 {
+                    data: 'taxes_due',
+                    render: $.fn.dataTable.render.number(',', '.', 2)
+                },
+                {
                     data: 'balance',
                     render: $.fn.dataTable.render.number(',', '.', 2)
                 },
 		{ data: 'last_paid' },
 		{ data: 'action' },
             ],
             order: [[2, "desc"]]
```

#### html2text {}

```diff
@@ -6,16 +6,17 @@
     * Corp_Moon_Audits
 
 **** Overall Monthly Tax Revenue ****
 Export CSV
 **** Monthly Taxes by Users ****
 Export CSV
 **** Taxes by User ****
-{% translate {% translate 'Corp' {% translate {% translate 'Last {% translate
-'Name' %}    %}                  'Balance' %} Paid' %}           'Actions' %}
+{% translate {% translate {% translate {% translate {% translate   {% translate
+'Name' %}    'Corp' %}    'Taxes Past  'Current     'Last Paid' %} 'Actions' %}
+                          Due' %}      Balance' %}
  ×
 *** Tax Credits ***
 {% csrf_token %}
 Recipient:
 Tax credit amount: [creditbox           ]
  {% translate 'Submit' %}
 **** Corp Ledgers ****
@@ -25,19 +26,19 @@
 **** Average Monthly Units of Ore by System ****
 **** Average Monthly Taxes by System ****
 {% translate {% translate 'Ore {% translate 'Value' {% translate 'Taxes'
 'System' %}  Type' %}          %}                   %}
 
 Export All Mining Activity CSV
 **** Unregistered Characters (Missing from MiningTax) ****
-{% translate 'Name' {% translate 'Approx. {% translate 'Ore {% translate 'Last
-%}                  ISK' %}               Units' %}         Mined' %}
+{% translate {% translate {% translate     {% translate 'Ore {% translate 'Last
+'Name' %}    'System' %}  'Approx. ISK' %} Units' %}         Mined' %}
 **** Unknown Characters (Missing from Auth) ****
-{% translate 'Name' {% translate 'Approx. {% translate 'Ore {% translate 'Last
-%}                  ISK' %}               Units' %}         Mined' %}
+{% translate {% translate {% translate     {% translate 'Ore {% translate 'Last
+'Name' %}    'System' %}  'Approx. ISK' %} Units' %}         Mined' %}
 **** Corp Moon Records ****
 {% translate {% translate 'Name' {% translate 'Ore' {% translate  {% translate
 'Date' %}    %}                  %}                 'Quantity' %} 'Location' %}
 {% endblock details %} {% block extra_javascript %} {% include 'bundles/
 datatables-js.html' %}
  {% endblock %} {% block extra_css %} {% if NIGHT_MODE %}
  {% else %}
@@ -48,15 +49,16 @@
 unregistered_table; var unknown_table; var corpmoon_table; var csv_data; var
 tax_csv_data; var tax_sys_data; var curshown = "#basic"; var firstdraw =
 {"#sys_stats" : true, "#corp_moons" : true, "#basic": false}; var
 sys_stats_data; function switchview(pane) { if (pane == curshown) { return; } $
 (curshown).addClass("hidden"); $(pane).removeClass("hidden"); curshown = pane;
 if (firstdraw[pane]) { if (pane == "#sys_stats") { draw_sys_stats(); } if (pane
 == "#corp_moons") { draw_corp_moons(); } firstdraw[pane] = false; } } function
-exportsysdata() { exportToCsv("miningtaxes-allactivity.csv", tax_sys_data); }
+exportsysdata() { $.get("{% url 'miningtaxes:admin_get_all_activity_json' %}",
+function(d) { exportToCsv("miningtaxes-allactivity.csv", d.data); }); }
 function exporttaxdata() { exportToCsv("miningtaxes-revenue.csv",
 tax_csv_data); } function exportdata() { exportToCsv("miningtaxes-
 usertaxes.csv", csv_data); } function exportToCsv(filename, rows) { var
 processRow = function (row) { var finalVal = ''; for (var j = 0; j <
 row.length; j++) { var innerValue = row[j] === null ? '' : row[j].toString();
 if (row[j] instanceof Date) { innerValue = row[j].toLocaleString(); }; var
 result = innerValue.replace(/"/g, '""'); if (result.search(/("|,|\n)/g) >= 0)
@@ -71,30 +73,31 @@
 ("download", filename); link.style.visibility = 'hidden';
 document.body.appendChild(link); link.click(); document.body.removeChild(link);
 } } } function populate(rowi) { $("#user").html(user_data[rowi].name); $
 ("#userid").val(user_data[rowi].user); const bal = Math.round((user_data
 [rowi].balance + Number.EPSILON) * 100) / 100 $("#creditbox").val(bal); }
 function draw_corp_moons() { $.getJSON("{% url 'miningtaxes:
 admin_corp_mining_history' %}", function (d) { unregistered_table = $
-('#unregistered').DataTable({ columns: [ { data: 'name' }, { data: 'isk',
-render: $.fn.dataTable.render.number(',', '.', 2) }, { data: 'quantity',
-render: $.fn.dataTable.render.number(',', '.', 0) }, { data: 'last' }, ],
-order: [[3, "desc"]] }); unknown_table = $('#unknown').DataTable({ columns: [
-{ data: 'name' }, { data: 'isk', render: $.fn.dataTable.render.number(',', '.',
-2) }, { data: 'quantity', render: $.fn.dataTable.render.number(',', '.', 0) },
-{ data: 'last' }, ], order: [[3, "desc"]] }); corpmoon_table = $
-('#corpmoon').DataTable({ columns: [ { data: 'date' }, { data: 'name' },
-{ data: 'ore' }, { data: 'quantity', render: $.fn.dataTable.render.number(',',
-'.', 0) }, { data: 'location' }, ], order: [[0, "desc"]] }); unknown_data = d
-["unknown_data"]; unknown_data.forEach( function(row) { unknown_table.row.add
-(row); }); unknown_table.draw(); unregistered_data = d["unregistered_data"];
-unregistered_data.forEach( function(row) { unregistered_table.row.add(row); });
-unregistered_table.draw(); mining_data = d["mining_log"]; mining_data.forEach
-( function(row) { corpmoon_table.row.add(row); }); corpmoon_table.draw(); }); }
-var sys_months_data; var sys_months_curi; var sys_months_order; var
+('#unregistered').DataTable({ columns: [ { data: 'name' }, { data: 'sys' },
+{ data: 'isk', render: $.fn.dataTable.render.number(',', '.', 2) }, { data:
+'quantity', render: $.fn.dataTable.render.number(',', '.', 0) }, { data: 'last'
+}, ], order: [[4, "desc"]] }); unknown_table = $('#unknown').DataTable(
+{ columns: [ { data: 'name' }, { data: 'sys' }, { data: 'isk', render:
+$.fn.dataTable.render.number(',', '.', 2) }, { data: 'quantity', render:
+$.fn.dataTable.render.number(',', '.', 0) }, { data: 'last' }, ], order: [[4,
+"desc"]] }); corpmoon_table = $('#corpmoon').DataTable({ columns: [ { data:
+'date' }, { data: 'name' }, { data: 'ore' }, { data: 'quantity', render:
+$.fn.dataTable.render.number(',', '.', 0) }, { data: 'location' }, ], order: [
+[0, "desc"]] }); unknown_data = d["unknown_data"]; unknown_data.forEach
+( function(row) { unknown_table.row.add(row); }); unknown_table.draw();
+unregistered_data = d["unregistered_data"]; unregistered_data.forEach( function
+(row) { unregistered_table.row.add(row); }); unregistered_table.draw();
+mining_data = d["mining_log"]; mining_data.forEach( function(row)
+{ corpmoon_table.row.add(row); }); corpmoon_table.draw(); }); } var
+sys_months_data; var sys_months_curi; var sys_months_order; var
 sys_month_table; function prior() { if (sys_months_curi == 0) { return;}
 sys_months_curi--; render_sys_month_table(); } function next() { if
 (sys_months_curi == sys_months_order.length - 1) { return;} sys_months_curi++;
 render_sys_month_table(); } function render_sys_month_table() { const m =
 sys_months_order[sys_months_curi]; sys_month_table.clear(); $
 ("#sys_month_disp").html(m); Object.keys(sys_months_data[m]).forEach( function
 (s) { Object.keys(sys_months_data[m][s]).forEach( function(g)
@@ -114,39 +117,40 @@
 = bb.generate({ data: { x: "x", columns: [], type: "bar", }, bar: { width:
 { ratio: 0.5 } }, axis: { x: {type: "category"}, y: { tick: { format: function
 (x) { return d3.format(",")(x); } }, label: "ISK" }, }, bindto:"#sys_avg_tax"
 }); isk.load({columns: d['anal']['tax']}); var isk = bb.generate({ data: { x:
 "x", columns: [], type: "bar", }, bar: { width: { ratio: 0.5 } }, axis: { x:
 {type: "category"}, y: { tick: { format: function(x) { return d3.format(",")
 (x); } }, label: "Quantity" }, }, bindto:"#sys_avg_q" }); isk.load({columns: d
-['anal']['q']}); tax_sys_data = d["csv"]; $("#syscsv").click(exportsysdata);
-}); } $(document).ready(function () { $.getJSON("{% url 'miningtaxes:
-admin_tax_revenue_json' %}", function (d) { var taxrevenue = bb.generate(
-{ data: { x: "x", columns: [], axes: { isk: "y"}, type: "bar", }, bar: { width:
-{ ratio: 0.5 } }, legend: { show: false }, axis: { x: { padding: { right:
-5000*60*60*12 }, type: "timeseries", tick: { format: "%Y-%m", rotate: 45 } },
-y: { tick: { format: function(x) { return d3.format(",")(x); } }, label: "ISK"
-}, }, bindto:"#taxrevenue" }); taxrevenue.load({columns: [d['xdata'], d
-['ydata']]}); tax_csv_data = d["csv"]; $("#taxcsv").click(exporttaxdata); } );
-$.getJSON("{% url 'miningtaxes:admin_month_json' %}", function (d) { var
-iskchart = bb.generate({ data: { x: "x", columns: [], axes: { isk: "y"}, },
-axis: { x: { padding: { right: 5000*60*60*12 }, type: "timeseries", tick:
-{ format: "%Y-%m", rotate: 45 } }, y: { tick: { format: function(x) { return
-d3.format(",")(x); } }, label: "ISK" }, }, bindto:"#isk" }); for (var i = 0 ; i
-< d["ydata"].length; i++) { iskchart.load({columns: [d['xdata'], d['ydata']
-[i]]}); } csv_data = d["csv"]; $("#csv").click(exportdata); } ); $.getJSON("{%
-url 'miningtaxes:admin_main_json' %}", function (d) { user_data = d["data"];
-user_data.forEach( function(row) { user_table.row.add(row); }); user_table.draw
-(); }); user_table = $('#mains').DataTable({ columns: [ { data: 'name' },
-{ data: 'corp' }, { data: 'balance', render: $.fn.dataTable.render.number(',',
-'.', 2) }, { data: 'last_paid' }, { data: 'action' }, ], order: [[2, "desc"]]
-}); $('#corp_ledgers').DataTable({ ajax: { url: "{% url 'miningtaxes:
-admin_corp_ledger' %}", dataSrc: 'data', cache: false }, columns: [ { data:
-'date' }, { data: 'name' }, { data: 'amount', render:
-$.fn.dataTable.render.number(',', '.', 2) }, { data: 'reason' }, ], order: [[0,
-"desc"]] }); /* $('#chars').DataTable({ ajax: { url: "{% url 'miningtaxes:
-admin_char_json' %}", dataSrc: 'data', cache: false }, columns: [ { data:
-'name' }, { data: 'corp' }, { data: 'main_name' }, { data: 'taxes', render:
-$.fn.dataTable.render.number(',', '.', 2) }, { data: 'credits', render:
+['anal']['q']}); }); } $(document).ready(function () { $("#syscsv").click
+(exportsysdata); $.getJSON("{% url 'miningtaxes:admin_tax_revenue_json' %}",
+function (d) { var taxrevenue = bb.generate({ data: { x: "x", columns: [],
+axes: { isk: "y"}, type: "bar", }, bar: { width: { ratio: 0.5 } }, legend:
+{ show: false }, axis: { x: { padding: { right: 5000*60*60*12 }, type:
+"timeseries", tick: { format: "%Y-%m", rotate: 45 } }, y: { tick: { format:
+function(x) { return d3.format(",")(x); } }, label: "ISK" }, }, bindto:
+"#taxrevenue" }); taxrevenue.load({columns: [d['xdata'], d['ydata']]});
+tax_csv_data = d["csv"]; $("#taxcsv").click(exporttaxdata); } ); $.getJSON("{%
+url 'miningtaxes:admin_month_json' %}", function (d) { var iskchart =
+bb.generate({ data: { x: "x", columns: [], axes: { isk: "y"}, }, axis: { x:
+{ padding: { right: 5000*60*60*12 }, type: "timeseries", tick: { format: "%Y-
+%m", rotate: 45 } }, y: { tick: { format: function(x) { return d3.format(",")
+(x); } }, label: "ISK" }, }, bindto:"#isk" }); for (var i = 0 ; i < d
+["ydata"].length; i++) { iskchart.load({columns: [d['xdata'], d['ydata'][i]]});
+} iskchart.focus(["all"]); csv_data = d["csv"]; $("#csv").click(exportdata); }
+); $.getJSON("{% url 'miningtaxes:admin_main_json' %}", function (d)
+{ user_data = d["data"]; user_data.forEach( function(row) { user_table.row.add
+(row); }); user_table.draw(); }); user_table = $('#mains').DataTable({ columns:
+[ { data: 'name' }, { data: 'corp' }, { data: 'taxes_due', render:
+$.fn.dataTable.render.number(',', '.', 2) }, { data: 'balance', render:
+$.fn.dataTable.render.number(',', '.', 2) }, { data: 'last_paid' }, { data:
+'action' }, ], order: [[2, "desc"]] }); $('#corp_ledgers').DataTable({ ajax:
+{ url: "{% url 'miningtaxes:admin_corp_ledger' %}", dataSrc: 'data', cache:
+false }, columns: [ { data: 'date' }, { data: 'name' }, { data: 'amount',
+render: $.fn.dataTable.render.number(',', '.', 2) }, { data: 'reason' }, ],
+order: [[0, "desc"]] }); /* $('#chars').DataTable({ ajax: { url: "{% url
+'miningtaxes:admin_char_json' %}", dataSrc: 'data', cache: false }, columns: [
+{ data: 'name' }, { data: 'corp' }, { data: 'main_name' }, { data: 'taxes',
+render: $.fn.dataTable.render.number(',', '.', 2) }, { data: 'credits', render:
 $.fn.dataTable.render.number(',', '.', 2) }, { data: 'balance', render:
 $.fn.dataTable.render.number(',', '.', 2) } ], order: [[5, "desc"]] }); */ });
 {% endblock %}
```

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/base.html` & `aa-miningtaxes-1.2.4/miningtaxes/templates/miningtaxes/base.html`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/character_viewer.html` & `aa-miningtaxes-1.2.4/miningtaxes/templates/miningtaxes/character_viewer.html`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/faq.html` & `aa-miningtaxes-1.2.4/miningtaxes/templates/miningtaxes/faq.html`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/launcher.html` & `aa-miningtaxes-1.2.4/miningtaxes/templates/miningtaxes/admin_launcher.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,64 @@
 {% extends 'miningtaxes/base.html' %}
 {% load i18n %}
 {% load static %}
 {% load humanize %}
 {% load evelinks %}
+{% load bootstrap %}
 
 {% block details %}
+    <div class="panel panel-default">
+        <div class="panel-heading" style="display:flex;">
+		<h3 class="panel-title">{% translate 'MiningTaxes Settings' %} (v{{ version }})</h3>
+        </div>
+        <div class="panel-body">
+	    <form class="form" action="{{ url }}" method="POST">
+		    {% csrf_token %}
+		    {{ form|bootstrap }}
+		    <button type="submit" class="btn btn-primary">Edit Settings</button>
+	    </form>
+	</div>
+    </div>
 
     <div class="panel panel-default">
         <div class="panel-heading" style="display:flex;">
-            <h3 class="panel-title">{% translate 'Characters' %}</h3>
+            <h3 class="panel-title">{% translate 'Accountant Characters (add only one accountant per corp)' %}</h3>
         </div>
         <div class="panel-body">
             <!-- Characters -->
             <div class="character-cards">
                 <ul class="cards_container">
                     <!-- Add New Character -->
                     <li class="cards_item">
                         <div class="card">
                             <div class="card-header">{% translate 'Register Character' %}</div>
 
                             <div class="card-body card__content">
-                                <a href="{% url 'miningtaxes:add_character' %}">
+                                <a href="{% url 'miningtaxes:add_admin_character' %}">
                                     <img src="{{ 1|character_portrait_url:256 }}" alt="Add character">
                                 </a>
                             </div>
 
                             <div class="card-footer">
-                                <a class="btn btn-primary btn-sm" href="{% url 'miningtaxes:add_character' %}">{% translate 'Register' %}</a>
+                                <a class="btn btn-primary btn-sm" href="{% url 'miningtaxes:add_admin_character' %}">{% translate 'Register' %}</a>
                             </div>
                         </div>
                     </li>
 
                     {% if has_registered_characters %}
                         <!-- Registered Characters -->
                         {% for auth_character in auth_characters|dictsort:"character_name" %}
                             <li class="cards_item">
                                 <div class="card">
                                     <div class="card-header">
                                         {{ auth_character.character_name }}
-                                        {% if auth_character.character_id == main_character_id %}
-                                            &nbsp;<i class="fas fa-crown" title="Main character"></i>
-                                        {% endif %}
-                                        {% if auth_character.character.is_shared %}
-                                            &nbsp;<i class="far fa-eye" title="Currently shared with recruiters"></i>
-                                        {% endif %}
                                     </div>
-
                                     <div class="card-body card__content">
                                         <p>
-                                            <a href="{% url 'miningtaxes:character_viewer' auth_character.character.pk %}">
+					<a href="">
                                                 <span class="aa-miningtaxes-launcher-character-image">
                                                     <img src="{{ auth_character.character_id|character_portrait_url:256 }}" alt="{{ auth_character.character_name }}">
 
                                                     {% if auth_character.alliance_id %}
                                                         <span class="aa-miningtaxes-alliance-logo">
                                                             <img class="" src="{{ auth_character.alliance_id|alliance_logo_url:64 }}" title="{{ auth_character.alliance_name }}">
                                                         </span>
@@ -62,59 +68,71 @@
                                                         <img class="" src="{{ auth_character.corporation_id|corporation_logo_url:64 }}" title="{{ auth_character.corporation_name }}">
                                                     </span>
                                                 </span>
                                             </a>
                                         </p>
 
                                         <div class="text-center">
-                                            <br>
-                                            {% if auth_character.character.wallet_balance %}
-                                                {{ auth_character.character.wallet_balance.total|intword|default_if_none:"-" }} ISK<br>
-                                            {% else %}
-                                                <span class="text-muted">{% translate "(no data yet)" %}</span>
-                                            {% endif %}
-
                                         </div>
                                     </div>
 
                                     <div class="card-footer">
-                                        <a class="btn btn-success btn-sm" href="{% url 'miningtaxes:character_viewer' auth_character.character.pk %}"
-                                            role="button" title="{% translate 'View this character.' %}">
-                                            <i class="fas fa-sign-in-alt"></i>
-                                        </a>
-
-                                        <a class="btn btn-danger btn-sm" href="{% url 'miningtaxes:remove_character' auth_character.character.pk %}"
+                                        <a class="btn btn-danger btn-sm" href="{% url 'miningtaxes:remove_admin_character' auth_character.character.pk %}"
                                             role="button" title="{% translate 'Remove this character.' %}"
                                             onclick="return confirm('Are you sure you want to REMOVE this character?')">
                                             <i class="far fa-trash-alt"></i>
                                         </a>
                                     </div>
                                 </div>
                             </li>
                         {% endfor %}
                     {% endif %}
                 </ul>
             </div>
+        </div>
+    </div>
 
-            {% if unregistered_chars|length > 0 %}
-                <p class="text-warning">
-                    <strong>
-                    <i class="fas fa-exclamation-triangle"></i>
-                    {% translate 'Unregistered character(s):' %}&nbsp;&nbsp;</strong>
-                    {{ unregistered_chars|join:", " }}
-                </p>
-            {% endif %}
+    <div class="panel panel-default">
+        <div class="panel-heading" style="display:flex;">
+            <h3 class="panel-title">{% translate 'Registered Characters in plugin' %}</h3>
+        </div>
+        <div class="panel-body">
+            <!-- Characters -->
+            <div class="character-cards">
+                        <!-- Registered Characters -->
+                        {% for auth_character in auth_registered|dictsort:"character_name" %}
+                                        <a class="btn btn-danger btn-sm" href="{% url 'miningtaxes:remove_admin_registered' auth_character.character.pk %}"
+                                            role="button" title="{% translate 'Remove this character.' %}"
+							  onclick="return confirm('Are you sure you want to REMOVE {{auth_character.character_name}}? All mining history and tax history will be erased!')">
+						<i class="far fa-trash-alt"></i> {{auth_character.character_name}}
+                                        </a>
+                        {% endfor %}
+            </div>
+        </div>
+    </div>
 
+    <div class="panel panel-default">
+        <div class="panel-heading" style="display:flex;">
+            <h3 class="panel-title">{% translate 'Admin actions' %}</h3>
+        </div>
+        <div class="panel-body">
+		<ul>
+			<li>
+				<a class="btn btn-danger btn-sm" href="{% url 'miningtaxes:purge_old_corphistory' %}"
+				    role="button" title="{% translate 'Purge corp mining history older than 90 days.' %}"
+				    onclick="return confirm('Are you sure you want to PURGE corp mining history older than 90 days?')">
+				    <i class="far fa-trash-alt"></i> Purge corp history older than 90 days
+				</a>
+			</li>
+		</ul>
         </div>
     </div>
 
-{% endblock details %}
 
-{% block extra_javascript %}
-{% endblock %}
+{% endblock details %}
 
 {% block extra_css %}
     <link rel="stylesheet" href="{% static 'miningtaxes/css/global.css' %}" type="text/css">
     <link rel="stylesheet" href="{% static 'miningtaxes/css/miningtaxes.css' %}" type="text/css">
     <link rel="stylesheet" href="{% static 'miningtaxes/css/launcher.css' %}" type="text/css">
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,30 +1,26 @@
 {% extends 'miningtaxes/base.html' %} {% load i18n %} {% load static %} {% load
-humanize %} {% load evelinks %} {% block details %}
-**** {% translate 'Characters' %} ****
+humanize %} {% load evelinks %} {% load bootstrap %} {% block details %}
+**** {% translate 'MiningTaxes Settings' %} (v{{ version }}) ****
+{% csrf_token %} {{ form|bootstrap }} Edit Settings
+**** {% translate 'Accountant Characters (add only one accountant per corp)' %}
+****
     * {% translate 'Register Character' %}
       [Add_character]
       {%_translate_'Register'_%}
     * {% if has_registered_characters %}  {% for auth_character in
       auth_characters|dictsort:"character_name" %}
-    * {{ auth_character.character_name }} {% if auth_character.character_id ==
-      main_character_id %}   {% endif %} {% if
-      auth_character.character.is_shared %}   {% endif %}
-      _[{{_auth_character.character_name_}}]_{%_if_auth_character.alliance_id
-      %}__[{{_auth_character.alliance_id|alliance_logo_url:64_}}]__{%_endif_%}
-      [{{_auth_character.corporation_id|corporation_logo_url:64_}}]__
-
-      {% if auth_character.character.wallet_balance %} {
-      { auth_character.character.wallet_balance.total|intword|default_if_none:
-      "-" }} ISK
-      {% else %} {% translate "(no data yet)" %} {% endif %}
-
+    * {{ auth_character.character_name }}
+       [{{ auth_character.character_name }}] {% if auth_character.alliance_id
+      %}  [{{ auth_character.alliance_id|alliance_logo_url:64 }}]  {% endif %}
+      [{{ auth_character.corporation_id|corporation_logo_url:64 }}]
     * {% endfor %} {% endif %}
-{% if unregistered_chars|length > 0 %}
- {% translate 'Unregistered character(s):' %}  
- {{ unregistered_chars|join:", " }}
-{% endif %}
-{% endblock details %} {% block extra_javascript %} {% endblock %} {% block
-extra_css %}
+**** {% translate 'Registered Characters in plugin' %} ****
+ {% for auth_character in auth_registered|dictsort:"character_name" %}
+ {{auth_character.character_name}}
+ {% endfor %}
+**** {% translate 'Admin actions' %} ****
+    *  Purge_corp_history_older_than_90_days
+{% endblock details %} {% block extra_css %}
 
 
  {% endblock %} {% block extra_script %} {% endblock %}
```

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/ore_prices.html` & `aa-miningtaxes-1.2.4/miningtaxes/templates/miningtaxes/ore_prices.html`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/user_summary.html` & `aa-miningtaxes-1.2.4/miningtaxes/templates/miningtaxes/user_summary.html`

 * *Files 12% similar despite different names*

```diff
@@ -10,25 +10,44 @@
 	<div class="col-md-6">
     		<div class="panel panel-default">
 			<div class="panel-heading" style="display:flex;">
 			    <h3 class="panel-title">Taxes Summary</h3>
 			</div>
 			<div class="panel-body">
 				<dl class="dl-horizontal">
+					<dt>Taxes past due:</dt>
+					{% if taxes_due > 0 %}
+						<dd class="nowrap text-red">
+					{% else %}
+						<dd class="nowrap text-green">
+					{% endif %}
+					<span data-toggle="tooltip" data-placement="bottom" title="Green means that you do not owe taxes or have overpaid, red means that you owe taxes. Taxes past due refers to the amount needed to be paid currently to avoid interest (frozen at the end of the previous month).">
+						{{ taxes_due|floatformat:2|intcomma }} ISK</span> </dd>
 					<dt>Current Taxes owed:</dt>
-					<dd class="nowrap"> {{ balance }} ISK</dd>
-					<dt>Exact amount:</dt>
-					<dd class="nowrap"> {{ balance_raw }} ISK</dd>
+					{% if balance_raw > 0 %}
+						<dd class="nowrap text-red">
+					{% else %}
+						<dd class="nowrap text-green">
+					{% endif %}
+					<span data-toggle="tooltip" data-placement="bottom" title="Green means that you do not owe taxes or have overpaid, red means that you owe taxes. Current taxes refers to the tax balance taking into consideration the amount of mining performed in the current month.">
+						{{ balance }} ISK</dd>
+					<dt>Current Taxes exact:</dt>
+					{% if balance_raw > 0 %}
+						<dd class="nowrap text-red">
+					{% else %}
+						<dd class="nowrap text-green">
+					{% endif %}
+					<span data-toggle="tooltip" data-placement="bottom" title="Green means that you do not owe taxes or have overpaid, red means that you owe taxes. Current taxes refers to the tax balance taking into consideration the amount of mining performed in the current month.">
+						{{ balance_raw|floatformat:2|intcomma }} ISK</dd>
 					<dt>Last paid:</dt>
 					<dd class="nowrap"> {{ last_paid|timesince }}</dd>
 					<dt>Characters:</dt>
 					{% for char in auth_characters %}
 					<dd class="nowrap"><a href="{% url 'miningtaxes:character_viewer' char.pk %}"> {{ char.name }}</a></dd>
 					{% endfor %}
-
 				</dl>
 			</div>
 		</div>
     <br/>
 
     <div class="panel panel-default">
         <div class="panel-heading" style="display:flex;">
@@ -50,17 +69,17 @@
 
 
 	</div>
 
 	<div class="col-md-6">
     		<div class="panel panel-default">
 			<div class="panel-heading" style="display:flex;">
-				<button class="btn btn-default" onclick="prior()"><span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span></button>
-				<h3 class="panel-title">Leaderboard: <span id='leaderboard-month'></span></h3>
-				<button class="btn btn-default" onclick="next()"><span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span></button>
+				<button class="btn btn-default item-icon-button" onclick="prior()"><span class="glyphicon glyphicon-chevron-left item-icon" aria-hidden="true"></span></button>
+				<h3 class="panel-title"> Leaderboard: <span id='leaderboard-month'></span></h3>
+				<button class="btn btn-default item-icon-button" onclick="next()"><span class="glyphicon glyphicon-chevron-right item-icon" aria-hidden="true"></span></button>
 			</div>
 			<div class="panel-body">
 			    <div class="table-responsive">
 				<table class="table table-striped table-width-fix" id="leaderboard">
 				    <thead>
 					<tr>
 					    <th>{% translate 'Rank' %}</th>
@@ -160,14 +179,15 @@
 	lb_data[lbi]["table"].forEach(function(d) {
 		lb_table.row.add(d);
 	});
 	lb_table.draw();
 }
 
 (function() {
+	$('[data-toggle="tooltip"]').tooltip();
 	$.getJSON("{% url 'miningtaxes:user_mining_ledger_90day' user_pk %}", function (d) {
 		console.log(d);
 		var maxpg = 0;
 		d["polargraph"].forEach(function(arr) { if (maxpg < arr[1]) { maxpg = arr[1]; } });
 		var pgs = [];
 		d["stacked"].forEach(function(arr) { if (arr[0] != "x") { pgs.push(arr[0]); } });
 		console.log(pgs);
```

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/tests/models/test_admin_character.py` & `aa-miningtaxes-1.2.4/miningtaxes/tests/models/test_admin_character.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/tests/models/test_character.py` & `aa-miningtaxes-1.2.4/miningtaxes/tests/models/test_character.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/tests/models/test_orePrice.py` & `aa-miningtaxes-1.2.4/miningtaxes/tests/models/test_orePrice.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/tests/testdata/esi_client_stub.py` & `aa-miningtaxes-1.2.4/miningtaxes/tests/testdata/esi_client_stub.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/tests/testdata/load_entities.py` & `aa-miningtaxes-1.2.4/miningtaxes/tests/testdata/load_entities.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/tests/utils.py` & `aa-miningtaxes-1.2.4/miningtaxes/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/miningtaxes/urls.py` & `aa-miningtaxes-1.2.4/miningtaxes/urls.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,40 +11,55 @@
     path("add_admin_character", views.add_admin_character, name="add_admin_character"),
     path(
         "remove_character/<int:character_pk>/",
         views.remove_character,
         name="remove_character",
     ),
     path(
+        "remove_admin_registered/<int:character_pk>/",
+        views.remove_admin_registered,
+        name="remove_admin_registered",
+    ),
+    path(
         "remove_admin_character/<int:character_pk>/",
         views.remove_admin_character,
         name="remove_admin_character",
     ),
     path(
         "character_viewer/<int:character_pk>/",
         views.character_viewer,
         name="character_viewer",
     ),
     path(
-        "character_mining_ledger_data/<int:character_pk>/",
-        views.character_mining_ledger_data,
+        "purge_old_corphistory",
+        views.purge_old_corphistory,
+        name="purge_old_corphistory",
+    ),
+    path(
+        "char_mining_ledger_data/<int:character_pk>/",
+        views.char_mining_ledger_data,
         name="character_mining_ledger_data",
     ),
     path(
         "user_mining_ledger_90day/<int:user_pk>",
         views.user_mining_ledger_90day,
         name="user_mining_ledger_90day",
     ),
     path("user_summary/<int:user_pk>", views.user_summary, name="user_summary"),
     path(
         "summary_month_json/<int:user_pk>",
         views.summary_month_json,
         name="summary_month_json",
     ),
     path(
+        "admin_get_all_activity_json",
+        views.admin_get_all_activity_json,
+        name="admin_get_all_activity_json",
+    ),
+    path(
         "all_tax_credits/<int:user_pk>",
         views.all_tax_credits,
         name="all_tax_credits",
     ),
     path("faq", views.faq, name="faq"),
     path("ore_prices", views.ore_prices, name="ore_prices"),
     path("ore_prices_json", views.ore_prices_json, name="ore_prices_json"),
```

### Comparing `aa-miningtaxes-1.1.8/setup.py` & `aa-miningtaxes-1.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/testauth/celery.py` & `aa-miningtaxes-1.2.4/testauth/celery.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/testauth/settingsAA2.py` & `aa-miningtaxes-1.2.4/testauth/settingsAA2.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.8/testauth/settingsAA3.py` & `aa-miningtaxes-1.2.4/testauth/settingsAA3.py`

 * *Files identical despite different names*

