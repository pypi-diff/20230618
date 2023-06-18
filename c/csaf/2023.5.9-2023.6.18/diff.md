# Comparing `tmp/csaf-2023.5.9.tar.gz` & `tmp/csaf-2023.6.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csaf-2023.5.9.tar", last modified: Tue May  9 17:00:04 2023, max compression
+gzip compressed data, was "csaf-2023.6.18.tar", last modified: Sun Jun 18 16:15:04 2023, max compression
```

## Comparing `csaf-2023.5.9.tar` & `csaf-2023.6.18.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-09 17:00:04.037012 csaf-2023.5.9/
--rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 csaf-2023.5.9/LICENSE
--rw-r--r--   0 ruth       (501) staff       (20)       34 2021-05-12 16:52:51.000000 csaf-2023.5.9/MANIFEST.in
--rw-r--r--   0 ruth       (501) staff       (20)     3732 2023-05-09 17:00:04.036798 csaf-2023.5.9/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     2576 2023-05-06 13:23:15.000000 csaf-2023.5.9/README.md
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-09 17:00:03.945976 csaf-2023.5.9/csaf/
--rw-r--r--   0 ruth       (501) staff       (20)     1984 2023-05-09 16:52:48.000000 csaf-2023.5.9/csaf/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)      246 2022-03-13 14:31:06.000000 csaf-2023.5.9/csaf/__main__.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:57.000000 csaf-2023.5.9/csaf/category.py
--rw-r--r--   0 ruth       (501) staff       (20)     4112 2023-01-02 18:40:21.000000 csaf-2023.5.9/csaf/cli.py
--rw-r--r--   0 ruth       (501) staff       (20)      647 2022-12-21 15:07:30.000000 csaf-2023.5.9/csaf/config.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:02.000000 csaf-2023.5.9/csaf/cpe.py
--rw-r--r--   0 ruth       (501) staff       (20)    17012 2023-05-09 16:26:07.000000 csaf-2023.5.9/csaf/csaf.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:06.000000 csaf-2023.5.9/csaf/cve.py
--rw-r--r--   0 ruth       (501) staff       (20)    11239 2023-05-06 14:07:29.000000 csaf-2023.5.9/csaf/cvss.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:10.000000 csaf-2023.5.9/csaf/cwe.py
--rw-r--r--   0 ruth       (501) staff       (20)    12425 2023-05-06 13:11:03.000000 csaf-2023.5.9/csaf/definitions.py
--rw-r--r--   0 ruth       (501) staff       (20)    14924 2022-07-31 13:30:33.000000 csaf-2023.5.9/csaf/document.py
--rw-r--r--   0 ruth       (501) staff       (20)     1284 2022-03-13 20:11:44.000000 csaf-2023.5.9/csaf/env.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:45.000000 csaf-2023.5.9/csaf/hash.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-09 17:00:04.027477 csaf-2023.5.9/csaf/mandatory/
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-02-14 21:10:09.000000 csaf-2023.5.9/csaf/mandatory/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)     1325 2021-12-16 11:48:56.000000 csaf-2023.5.9/csaf/mandatory/acyclic_product_ids.py
--rw-r--r--   0 ruth       (501) staff       (20)     2023 2021-12-16 11:48:42.000000 csaf-2023.5.9/csaf/mandatory/consistent_product_status.py
--rw-r--r--   0 ruth       (501) staff       (20)     1435 2022-02-13 17:11:58.000000 csaf-2023.5.9/csaf/mandatory/defined_group_ids.py
--rw-r--r--   0 ruth       (501) staff       (20)     2548 2022-02-13 17:04:26.000000 csaf-2023.5.9/csaf/mandatory/defined_product_ids.py
--rw-r--r--   0 ruth       (501) staff       (20)     5288 2022-06-19 10:04:43.000000 csaf-2023.5.9/csaf/mandatory/rules.py
--rw-r--r--   0 ruth       (501) staff       (20)      981 2022-02-13 16:48:33.000000 csaf-2023.5.9/csaf/mandatory/translator_and_source_lang.py
--rw-r--r--   0 ruth       (501) staff       (20)     1267 2022-02-13 20:44:51.000000 csaf-2023.5.9/csaf/mandatory/unique_group_ids.py
--rw-r--r--   0 ruth       (501) staff       (20)     1192 2022-02-13 20:40:08.000000 csaf-2023.5.9/csaf/mandatory/unique_product_ids.py
--rw-r--r--   0 ruth       (501) staff       (20)     2390 2022-02-13 16:48:33.000000 csaf-2023.5.9/csaf/mandatory/valid_category_name.py
--rw-r--r--   0 ruth       (501) staff       (20)    16500 2022-07-31 13:32:20.000000 csaf-2023.5.9/csaf/product.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:21.000000 csaf-2023.5.9/csaf/purl.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:33.000000 csaf-2023.5.9/csaf/terminal.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:41.000000 csaf-2023.5.9/csaf/tlp.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:29.000000 csaf-2023.5.9/csaf/version.py
--rw-r--r--   0 ruth       (501) staff       (20)     3354 2022-03-13 16:02:22.000000 csaf-2023.5.9/csaf/vuln_types.py
--rw-r--r--   0 ruth       (501) staff       (20)    13724 2023-05-08 18:30:19.000000 csaf-2023.5.9/csaf/vulnerability.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-09 17:00:04.021664 csaf-2023.5.9/csaf.egg-info/
--rw-r--r--   0 ruth       (501) staff       (20)     3732 2023-05-09 17:00:03.000000 csaf-2023.5.9/csaf.egg-info/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     1204 2023-05-09 17:00:03.000000 csaf-2023.5.9/csaf.egg-info/SOURCES.txt
--rw-r--r--   0 ruth       (501) staff       (20)        1 2023-05-09 17:00:03.000000 csaf-2023.5.9/csaf.egg-info/dependency_links.txt
--rw-r--r--   0 ruth       (501) staff       (20)       38 2023-05-09 17:00:03.000000 csaf-2023.5.9/csaf.egg-info/entry_points.txt
--rw-r--r--   0 ruth       (501) staff       (20)      222 2023-05-09 17:00:03.000000 csaf-2023.5.9/csaf.egg-info/requires.txt
--rw-r--r--   0 ruth       (501) staff       (20)        5 2023-05-09 17:00:03.000000 csaf-2023.5.9/csaf.egg-info/top_level.txt
--rw-r--r--   0 ruth       (501) staff       (20)     3004 2023-05-09 16:28:24.000000 csaf-2023.5.9/pyproject.toml
--rw-r--r--   0 ruth       (501) staff       (20)       38 2023-05-09 17:00:04.037076 csaf-2023.5.9/setup.cfg
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-09 17:00:04.036148 csaf-2023.5.9/test/
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:24.000000 csaf-2023.5.9/test/test_category.py
--rw-r--r--   0 ruth       (501) staff       (20)      544 2023-05-06 14:12:39.000000 csaf-2023.5.9/test/test_cli.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:47.000000 csaf-2023.5.9/test/test_config.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:50.000000 csaf-2023.5.9/test/test_cpe.py
--rw-r--r--   0 ruth       (501) staff       (20)     9011 2023-05-09 16:51:44.000000 csaf-2023.5.9/test/test_csaf.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:20.000000 csaf-2023.5.9/test/test_cve.py
--rw-r--r--   0 ruth       (501) staff       (20)     8678 2023-05-09 16:51:33.000000 csaf-2023.5.9/test/test_cvss.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:26.000000 csaf-2023.5.9/test/test_cwe.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:29.000000 csaf-2023.5.9/test/test_document.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:33:14.000000 csaf-2023.5.9/test/test_env.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:43.000000 csaf-2023.5.9/test/test_product.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:46.000000 csaf-2023.5.9/test/test_purl.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:49.000000 csaf-2023.5.9/test/test_terminal.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:52.000000 csaf-2023.5.9/test/test_tlp.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:55.000000 csaf-2023.5.9/test/test_version.py
--rw-r--r--   0 ruth       (501) staff       (20)     2259 2023-05-08 18:29:00.000000 csaf-2023.5.9/test/test_vulnerability.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 16:15:04.675685 csaf-2023.6.18/
+-rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 csaf-2023.6.18/LICENSE
+-rw-r--r--   0 ruth       (501) staff       (20)       34 2021-05-12 16:52:51.000000 csaf-2023.6.18/MANIFEST.in
+-rw-r--r--   0 ruth       (501) staff       (20)     3784 2023-06-18 16:15:04.675465 csaf-2023.6.18/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     2576 2023-05-06 13:23:15.000000 csaf-2023.6.18/README.md
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 16:15:04.594480 csaf-2023.6.18/csaf/
+-rw-r--r--   0 ruth       (501) staff       (20)     1985 2023-06-18 16:13:18.000000 csaf-2023.6.18/csaf/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)      246 2022-03-13 14:31:06.000000 csaf-2023.6.18/csaf/__main__.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:57.000000 csaf-2023.6.18/csaf/category.py
+-rw-r--r--   0 ruth       (501) staff       (20)     4112 2023-01-02 18:40:21.000000 csaf-2023.6.18/csaf/cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)      647 2022-12-21 15:07:30.000000 csaf-2023.6.18/csaf/config.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:02.000000 csaf-2023.6.18/csaf/cpe.py
+-rw-r--r--   0 ruth       (501) staff       (20)    17012 2023-05-09 16:26:07.000000 csaf-2023.6.18/csaf/csaf.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:06.000000 csaf-2023.6.18/csaf/cve.py
+-rw-r--r--   0 ruth       (501) staff       (20)    11239 2023-05-06 14:07:29.000000 csaf-2023.6.18/csaf/cvss.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:10.000000 csaf-2023.6.18/csaf/cwe.py
+-rw-r--r--   0 ruth       (501) staff       (20)    12425 2023-05-06 13:11:03.000000 csaf-2023.6.18/csaf/definitions.py
+-rw-r--r--   0 ruth       (501) staff       (20)    14924 2022-07-31 13:30:33.000000 csaf-2023.6.18/csaf/document.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1284 2022-03-13 20:11:44.000000 csaf-2023.6.18/csaf/env.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:45.000000 csaf-2023.6.18/csaf/hash.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 16:15:04.617995 csaf-2023.6.18/csaf/mandatory/
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-02-14 21:10:09.000000 csaf-2023.6.18/csaf/mandatory/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1325 2021-12-16 11:48:56.000000 csaf-2023.6.18/csaf/mandatory/acyclic_product_ids.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2023 2021-12-16 11:48:42.000000 csaf-2023.6.18/csaf/mandatory/consistent_product_status.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1435 2022-02-13 17:11:58.000000 csaf-2023.6.18/csaf/mandatory/defined_group_ids.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2548 2022-02-13 17:04:26.000000 csaf-2023.6.18/csaf/mandatory/defined_product_ids.py
+-rw-r--r--   0 ruth       (501) staff       (20)     5288 2022-06-19 10:04:43.000000 csaf-2023.6.18/csaf/mandatory/rules.py
+-rw-r--r--   0 ruth       (501) staff       (20)      981 2022-02-13 16:48:33.000000 csaf-2023.6.18/csaf/mandatory/translator_and_source_lang.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1267 2022-02-13 20:44:51.000000 csaf-2023.6.18/csaf/mandatory/unique_group_ids.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1192 2022-02-13 20:40:08.000000 csaf-2023.6.18/csaf/mandatory/unique_product_ids.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2390 2022-02-13 16:48:33.000000 csaf-2023.6.18/csaf/mandatory/valid_category_name.py
+-rw-r--r--   0 ruth       (501) staff       (20)    16500 2022-07-31 13:32:20.000000 csaf-2023.6.18/csaf/product.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:21.000000 csaf-2023.6.18/csaf/purl.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:33.000000 csaf-2023.6.18/csaf/terminal.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:41.000000 csaf-2023.6.18/csaf/tlp.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:29.000000 csaf-2023.6.18/csaf/version.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3338 2023-06-18 15:51:02.000000 csaf-2023.6.18/csaf/vuln_types.py
+-rw-r--r--   0 ruth       (501) staff       (20)    13724 2023-05-08 18:30:19.000000 csaf-2023.6.18/csaf/vulnerability.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 16:15:04.603863 csaf-2023.6.18/csaf.egg-info/
+-rw-r--r--   0 ruth       (501) staff       (20)     3784 2023-06-18 16:15:04.000000 csaf-2023.6.18/csaf.egg-info/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     1204 2023-06-18 16:15:04.000000 csaf-2023.6.18/csaf.egg-info/SOURCES.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        1 2023-06-18 16:15:04.000000 csaf-2023.6.18/csaf.egg-info/dependency_links.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       38 2023-06-18 16:15:04.000000 csaf-2023.6.18/csaf.egg-info/entry_points.txt
+-rw-r--r--   0 ruth       (501) staff       (20)      222 2023-06-18 16:15:04.000000 csaf-2023.6.18/csaf.egg-info/requires.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        5 2023-06-18 16:15:04.000000 csaf-2023.6.18/csaf.egg-info/top_level.txt
+-rw-r--r--   0 ruth       (501) staff       (20)     3060 2023-06-18 14:46:31.000000 csaf-2023.6.18/pyproject.toml
+-rw-r--r--   0 ruth       (501) staff       (20)       38 2023-06-18 16:15:04.675740 csaf-2023.6.18/setup.cfg
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 16:15:04.675202 csaf-2023.6.18/test/
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:24.000000 csaf-2023.6.18/test/test_category.py
+-rw-r--r--   0 ruth       (501) staff       (20)      544 2023-05-06 14:12:39.000000 csaf-2023.6.18/test/test_cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:47.000000 csaf-2023.6.18/test/test_config.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:50.000000 csaf-2023.6.18/test/test_cpe.py
+-rw-r--r--   0 ruth       (501) staff       (20)     9011 2023-05-09 16:51:44.000000 csaf-2023.6.18/test/test_csaf.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:20.000000 csaf-2023.6.18/test/test_cve.py
+-rw-r--r--   0 ruth       (501) staff       (20)     8670 2023-06-18 16:08:21.000000 csaf-2023.6.18/test/test_cvss.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:26.000000 csaf-2023.6.18/test/test_cwe.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:29.000000 csaf-2023.6.18/test/test_document.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:33:14.000000 csaf-2023.6.18/test/test_env.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:43.000000 csaf-2023.6.18/test/test_product.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:46.000000 csaf-2023.6.18/test/test_purl.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:49.000000 csaf-2023.6.18/test/test_terminal.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:52.000000 csaf-2023.6.18/test/test_tlp.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:55.000000 csaf-2023.6.18/test/test_version.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2259 2023-05-08 18:29:00.000000 csaf-2023.6.18/test/test_vulnerability.py
```

### Comparing `csaf-2023.5.9/LICENSE` & `csaf-2023.6.18/LICENSE`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.9/PKG-INFO` & `csaf-2023.6.18/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: csaf
-Version: 2023.5.9
+Version: 2023.6.18
 Summary: Common Security Advisory Framework (CSAF) Verification, Validation, and Application Programming Interface (API).
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/csaf
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/csaf
 Project-URL: Documentation, https://codes.dilettant.life/docs/csaf
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/csaf
 Project-URL: Test-Coverage, https://codes.dilettant.life/coverage/csaf
 Keywords: code-generation,developer-tools,validation,verification
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `csaf-2023.5.9/README.md` & `csaf-2023.6.18/README.md`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.9/csaf/__init__.py` & `csaf-2023.6.18/csaf/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,13 +47,13 @@
 
 
 init_logger(name=APP_ENV, level=logging.DEBUG if DEBUG else None)
 
 from csaf.csaf import is_valid  # noqa
 
 # [[[fill git_describe()]]]
-__version__ = '2023.5.9+parent.0a298a86'
-# [[[end]]] (checksum: 72eec31730ba0300fcb5d605f8aec1d6)
+__version__ = '2023.6.18+parent.e26b1ac2'
+# [[[end]]] (checksum: 8b0627432c50d24920512d6d5a4eea35)
 __version_info__ = tuple(
     e if '-' not in e else e.split('-')[0] for part in __version__.split('+') for e in part.split('.') if e != 'parent'
 )
 __all__ = ['is_valid', 'log']
```

### Comparing `csaf-2023.5.9/csaf/cli.py` & `csaf-2023.6.18/csaf/cli.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.9/csaf/config.py` & `csaf-2023.6.18/csaf/config.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.9/csaf/csaf.py` & `csaf-2023.6.18/csaf/csaf.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.9/csaf/cvss.py` & `csaf-2023.6.18/csaf/cvss.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.9/csaf/definitions.py` & `csaf-2023.6.18/csaf/definitions.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.9/csaf/document.py` & `csaf-2023.6.18/csaf/document.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.9/csaf/env.py` & `csaf-2023.6.18/csaf/env.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.9/csaf/mandatory/acyclic_product_ids.py` & `csaf-2023.6.18/csaf/mandatory/acyclic_product_ids.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.9/csaf/mandatory/consistent_product_status.py` & `csaf-2023.6.18/csaf/mandatory/consistent_product_status.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.9/csaf/mandatory/defined_group_ids.py` & `csaf-2023.6.18/csaf/mandatory/defined_group_ids.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.9/csaf/mandatory/defined_product_ids.py` & `csaf-2023.6.18/csaf/mandatory/defined_product_ids.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.9/csaf/mandatory/rules.py` & `csaf-2023.6.18/csaf/mandatory/rules.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.9/csaf/mandatory/translator_and_source_lang.py` & `csaf-2023.6.18/csaf/mandatory/translator_and_source_lang.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.9/csaf/mandatory/unique_group_ids.py` & `csaf-2023.6.18/csaf/mandatory/unique_group_ids.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.9/csaf/mandatory/unique_product_ids.py` & `csaf-2023.6.18/csaf/mandatory/unique_product_ids.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.9/csaf/mandatory/valid_category_name.py` & `csaf-2023.6.18/csaf/mandatory/valid_category_name.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.9/csaf/product.py` & `csaf-2023.6.18/csaf/product.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.9/csaf/vuln_types.py` & `csaf-2023.6.18/csaf/vuln_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     multiple = 'MULTIPLE'
     single = 'SINGLE'
     none = 'NONE'
 
 
 class CiaType(Enum):
     none = 'NONE'
-    partial = 'PARTIAL'
-    complete = 'COMPLETE'
+    low = 'LOW'
+    high = 'HIGH'
 
 
 class ExploitabilityType(Enum):
     unproven = 'UNPROVEN'
     proof_of_concept = 'PROOF_OF_CONCEPT'
     functional = 'FUNCTIONAL'
     high = 'HIGH'
```

### Comparing `csaf-2023.5.9/csaf/vulnerability.py` & `csaf-2023.6.18/csaf/vulnerability.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.9/csaf.egg-info/PKG-INFO` & `csaf-2023.6.18/csaf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: csaf
-Version: 2023.5.9
+Version: 2023.6.18
 Summary: Common Security Advisory Framework (CSAF) Verification, Validation, and Application Programming Interface (API).
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/csaf
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/csaf
 Project-URL: Documentation, https://codes.dilettant.life/docs/csaf
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/csaf
 Project-URL: Test-Coverage, https://codes.dilettant.life/coverage/csaf
 Keywords: code-generation,developer-tools,validation,verification
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `csaf-2023.5.9/csaf.egg-info/SOURCES.txt` & `csaf-2023.6.18/csaf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.9/pyproject.toml` & `csaf-2023.6.18/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "csaf"
-version = "2023.5.9"
+version = "2023.6.18"
 description = "Common Security Advisory Framework (CSAF) Verification, Validation, and Application Programming Interface (API)."
 readme = "README.md"
 authors = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 maintainers = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.9",
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Libraries",
 ]
 keywords = [
     "code-generation",
     "developer-tools",
@@ -26,18 +27,18 @@
     "verification",
 ]
 dependencies = [
     "jmespath >= 1.0.1",
     "jsonschema >= 4.17.3",
     "langcodes >= 3.3.0",
     "lazr.uri >= 1.0.1",
-    "msgspec >= 0.14.2",
-    "pydantic >= 1.10.7",
+    "msgspec >= 0.16.0",
+    "pydantic >= 1.10.9",
     "scooby >= 0.7.2",
-    "setuptools >= 67.7.2",
+    "setuptools >= 67.8.0",
     "typer >= 0.9.0",
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = ["black", "coverage", "hypothesis", "mypy", "pytest", "pytest-cov", "pytest-flake8", "ruff"]
 
@@ -58,15 +59,15 @@
   "csaf.schema_proxy",
 ]
 exclude = ["test*"]
 
 [tool.black]
 line-length = 120
 skip-string-normalization = true
-target-version = ["py39", "py310", "py311"]
+target-version = ["py39", "py310", "py311", "py312"]
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.report]
 precision = 2
 exclude_lines = [
```

### Comparing `csaf-2023.5.9/test/test_cli.py` & `csaf-2023.6.18/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.9/test/test_csaf.py` & `csaf-2023.6.18/test/test_csaf.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.9/test/test_cvss.py` & `csaf-2023.6.18/test/test_cvss.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
             },
             'UserInteractionType': {
                 'title': 'UserInteractionType',
                 'description': 'An enumeration.',
                 'enum': ['NONE', 'REQUIRED'],
             },
             'ScopeType': {'title': 'ScopeType', 'description': 'An enumeration.', 'enum': ['UNCHANGED', 'CHANGED']},
-            'CiaType': {'title': 'CiaType', 'description': 'An enumeration.', 'enum': ['NONE', 'PARTIAL', 'COMPLETE']},
+            'CiaType': {'title': 'CiaType', 'description': 'An enumeration.', 'enum': ['NONE', 'LOW', 'HIGH']},
             'ScoreType': {'title': 'ScoreType', 'minimum': 0.0, 'maximum': 10.0, 'type': 'number'},
             'SeverityType': {
                 'title': 'SeverityType',
                 'description': 'An enumeration.',
                 'enum': ['NONE', 'LOW', 'MEDIUM', 'HIGH', 'CRITICAL'],
             },
             'ExploitCodeMaturityType': {
```

### Comparing `csaf-2023.5.9/test/test_vulnerability.py` & `csaf-2023.6.18/test/test_vulnerability.py`

 * *Files identical despite different names*

