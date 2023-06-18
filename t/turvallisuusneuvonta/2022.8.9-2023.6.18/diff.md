# Comparing `tmp/turvallisuusneuvonta-2022.8.9.tar.gz` & `tmp/turvallisuusneuvonta-2023.6.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turvallisuusneuvonta-2022.8.9.tar", last modified: Tue Aug  9 03:17:03 2022, max compression
+gzip compressed data, was "turvallisuusneuvonta-2023.6.18.tar", last modified: Sun Jun 18 19:14:58 2023, max compression
```

## Comparing `turvallisuusneuvonta-2022.8.9.tar` & `turvallisuusneuvonta-2023.6.18.tar`

### file list

```diff
@@ -1,140 +1,54 @@
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-09 03:17:03.142371 turvallisuusneuvonta-2022.8.9/
--rw-r--r--   0 ruth       (501) staff       (20)     1161 2022-04-30 21:02:24.000000 turvallisuusneuvonta-2022.8.9/.editorconfig
--rw-r--r--   0 ruth       (501) staff       (20)       19 2022-06-18 09:14:29.000000 turvallisuusneuvonta-2022.8.9/.gitattributes
--rw-r--r--   0 ruth       (501) staff       (20)     1890 2022-08-01 16:27:50.000000 turvallisuusneuvonta-2022.8.9/.gitignore
--rw-r--r--   0 ruth       (501) staff       (20)     1069 2021-12-08 15:36:04.000000 turvallisuusneuvonta-2022.8.9/LICENSE
--rw-r--r--   0 ruth       (501) staff       (20)       34 2021-05-12 16:52:51.000000 turvallisuusneuvonta-2022.8.9/MANIFEST.in
--rw-r--r--   0 ruth       (501) staff       (20)     2037 2022-08-09 03:09:34.000000 turvallisuusneuvonta-2022.8.9/Makefile
--rw-r--r--   0 ruth       (501) staff       (20)     2526 2022-08-09 03:17:03.142495 turvallisuusneuvonta-2022.8.9/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     1445 2022-08-09 02:59:04.000000 turvallisuusneuvonta-2022.8.9/README.md
--rw-r--r--   0 ruth       (501) staff       (20)     9288 2022-08-09 03:09:40.000000 turvallisuusneuvonta-2022.8.9/baseline-bandit.json
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-09 03:17:03.100771 turvallisuusneuvonta-2022.8.9/docs/
--rw-r--r--   0 ruth       (501) staff       (20)     3168 2022-02-14 21:51:06.000000 turvallisuusneuvonta-2022.8.9/docs/api.md
--rw-r--r--   0 ruth       (501) staff       (20)     1543 2022-08-09 03:08:05.000000 turvallisuusneuvonta-2022.8.9/docs/changes.md
--rw-r--r--   0 ruth       (501) staff       (20)     1240 2022-08-09 02:59:23.000000 turvallisuusneuvonta-2022.8.9/docs/index.md
--rw-r--r--   0 ruth       (501) staff       (20)      263 2022-08-09 03:05:18.000000 turvallisuusneuvonta-2022.8.9/docs/install.md
--rw-r--r--   0 ruth       (501) staff       (20)     4257 2022-08-09 03:05:31.000000 turvallisuusneuvonta-2022.8.9/docs/usage.md
--rw-r--r--   0 ruth       (501) staff       (20)     1093 2022-07-09 20:50:34.000000 turvallisuusneuvonta-2022.8.9/gen_version.py
--rw-r--r--   0 ruth       (501) staff       (20)     1353 2022-07-31 09:34:54.000000 turvallisuusneuvonta-2022.8.9/mkdocs.yml
--rw-r--r--   0 ruth       (501) staff       (20)      200 2022-05-22 10:06:06.000000 turvallisuusneuvonta-2022.8.9/pyproject.toml
--rw-r--r--   0 ruth       (501) staff       (20)       93 2022-07-31 13:23:15.000000 turvallisuusneuvonta-2022.8.9/requirements.txt
--rw-r--r--   0 ruth       (501) staff       (20)     1657 2022-02-20 15:52:47.000000 turvallisuusneuvonta-2022.8.9/sbom.json
--rw-r--r--   0 ruth       (501) staff       (20)     2117 2022-08-09 03:17:03.143609 turvallisuusneuvonta-2022.8.9/setup.cfg
--rw-r--r--   0 ruth       (501) staff       (20)       38 2021-12-08 15:53:54.000000 turvallisuusneuvonta-2022.8.9/setup.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-09 03:17:03.105538 turvallisuusneuvonta-2022.8.9/test/
--rw-r--r--   0 ruth       (501) staff       (20)      130 2021-12-20 19:14:02.000000 turvallisuusneuvonta-2022.8.9/test/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)     4385 2022-07-09 16:06:01.000000 turvallisuusneuvonta-2022.8.9/test/conftest.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2021-12-08 17:11:17.000000 turvallisuusneuvonta-2022.8.9/test/context.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-09 03:17:03.093098 turvallisuusneuvonta-2022.8.9/test/fixtures/
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-09 03:17:03.105844 turvallisuusneuvonta-2022.8.9/test/fixtures/a-b/
--rw-r--r--   0 ruth       (501) staff       (20)      527 2021-12-31 17:39:59.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/a-b/a-b.json
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-09 03:17:03.106151 turvallisuusneuvonta-2022.8.9/test/fixtures/a-game-log4j/
--rw-r--r--   0 ruth       (501) staff       (20)     2892 2021-12-31 17:46:21.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/a-game-log4j/some-vex-csaf-document.json
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-09 03:17:03.106540 turvallisuusneuvonta-2022.8.9/test/fixtures/empty/
--rw-r--r--   0 ruth       (501) staff       (20)        3 2021-12-08 15:36:04.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/empty/advisory.json
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-09 03:17:03.106820 turvallisuusneuvonta-2022.8.9/test/fixtures/example-com/
--rw-r--r--   0 ruth       (501) staff       (20)     1406 2021-12-12 13:18:31.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/example-com/example-com-123.json
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-09 03:17:03.092985 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-09 03:17:03.092918 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-09 03:17:03.124973 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/
--rw-r--r--   0 ruth       (501) staff       (20)      897 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-01-01.json
--rw-r--r--   0 ruth       (501) staff       (20)      926 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-02-01.json
--rw-r--r--   0 ruth       (501) staff       (20)     1143 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-03-01.json
--rw-r--r--   0 ruth       (501) staff       (20)     1107 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-04-01.json
--rw-r--r--   0 ruth       (501) staff       (20)     1344 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-05-01.json
--rw-r--r--   0 ruth       (501) staff       (20)     1046 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-06-01.json
--rw-r--r--   0 ruth       (501) staff       (20)     1510 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-07-01.json
--rw-r--r--   0 ruth       (501) staff       (20)     1142 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-08-01.json
--rw-r--r--   0 ruth       (501) staff       (20)     1188 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-09-01.json
--rw-r--r--   0 ruth       (501) staff       (20)     1501 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-10-01.json
--rw-r--r--   0 ruth       (501) staff       (20)      797 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-11-01.json
--rw-r--r--   0 ruth       (501) staff       (20)      689 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-12-01.json
--rw-r--r--   0 ruth       (501) staff       (20)      902 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-13-01.json
--rw-r--r--   0 ruth       (501) staff       (20)      817 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-14-01.json
--rw-r--r--   0 ruth       (501) staff       (20)      700 2021-11-24 04:47:33.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-15-01.json
--rw-r--r--   0 ruth       (501) staff       (20)      817 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-16-01.json
--rw-r--r--   0 ruth       (501) staff       (20)      698 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-17-01.json
--rw-r--r--   0 ruth       (501) staff       (20)      815 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-18-01.json
--rw-r--r--   0 ruth       (501) staff       (20)      881 2021-11-24 04:47:33.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-19-01.json
--rw-r--r--   0 ruth       (501) staff       (20)      882 2021-11-24 04:47:33.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-19-02.json
--rw-r--r--   0 ruth       (501) staff       (20)      705 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-20-01.json
--rw-r--r--   0 ruth       (501) staff       (20)      830 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-21-01.json
--rw-r--r--   0 ruth       (501) staff       (20)      837 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-22-01.json
--rw-r--r--   0 ruth       (501) staff       (20)      798 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-23-01.json
--rw-r--r--   0 ruth       (501) staff       (20)     1131 2021-11-24 04:47:33.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-24-01.json
--rw-r--r--   0 ruth       (501) staff       (20)     1134 2021-11-24 04:47:33.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-24-02.json
--rw-r--r--   0 ruth       (501) staff       (20)     1390 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-25-01.json
--rw-r--r--   0 ruth       (501) staff       (20)      710 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-26-01.json
--rw-r--r--   0 ruth       (501) staff       (20)      953 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-27-01-01.json
--rw-r--r--   0 ruth       (501) staff       (20)      914 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-27-02-01.json
--rw-r--r--   0 ruth       (501) staff       (20)      790 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-27-03-01.json
--rw-r--r--   0 ruth       (501) staff       (20)      830 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-27-04-01.json
--rw-r--r--   0 ruth       (501) staff       (20)      783 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-27-05-01.json
--rw-r--r--   0 ruth       (501) staff       (20)      788 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-27-06-01.json
--rw-r--r--   0 ruth       (501) staff       (20)     1106 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-27-07-01.json
--rw-r--r--   0 ruth       (501) staff       (20)      771 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-27-08-01.json
--rw-r--r--   0 ruth       (501) staff       (20)     1618 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-27-09-01.json
--rw-r--r--   0 ruth       (501) staff       (20)     1676 2021-07-24 10:58:12.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-27-10-01.json
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-09 03:17:03.125467 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/valid_category_name/
--rw-r--r--   0 ruth       (501) staff       (20)      530 2022-02-06 13:11:44.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/valid_category_name/space_vex.json
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-09 03:17:03.093033 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/valid/
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-09 03:17:03.126007 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/valid/valid_category_name/
--rw-r--r--   0 ruth       (501) staff       (20)      528 2022-02-06 13:12:38.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/rules/valid/valid_category_name/space_vex.json
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-09 03:17:03.126397 turvallisuusneuvonta-2022.8.9/test/fixtures/spam/
--rw-r--r--   0 ruth       (501) staff       (20)     1143 2022-02-14 22:04:32.000000 turvallisuusneuvonta-2022.8.9/test/fixtures/spam/advisory.json
--rw-r--r--   0 ruth       (501) staff       (20)      712 2022-08-08 05:07:26.000000 turvallisuusneuvonta-2022.8.9/test/requirements-dev.txt
--rw-r--r--   0 ruth       (501) staff       (20)      705 2022-08-07 07:18:38.000000 turvallisuusneuvonta-2022.8.9/test/requirements.txt
--rw-r--r--   0 ruth       (501) staff       (20)     1558 2022-07-09 16:07:06.000000 turvallisuusneuvonta-2022.8.9/test/test_cli.py
--rw-r--r--   0 ruth       (501) staff       (20)    13142 2022-07-09 16:08:10.000000 turvallisuusneuvonta-2022.8.9/test/test_csaf_core_rules_mandatory.py
--rw-r--r--   0 ruth       (501) staff       (20)     1318 2022-07-31 09:29:32.000000 turvallisuusneuvonta-2022.8.9/test/test_csaf_document.py
--rw-r--r--   0 ruth       (501) staff       (20)     2865 2022-07-31 09:29:32.000000 turvallisuusneuvonta-2022.8.9/test/test_csaf_meta.py
--rw-r--r--   0 ruth       (501) staff       (20)     2297 2022-07-31 09:33:20.000000 turvallisuusneuvonta-2022.8.9/test/test_csaf_product.py
--rw-r--r--   0 ruth       (501) staff       (20)     8761 2022-07-31 09:32:21.000000 turvallisuusneuvonta-2022.8.9/test/test_csaf_vulnerability.py
--rw-r--r--   0 ruth       (501) staff       (20)     4974 2022-07-31 09:29:32.000000 turvallisuusneuvonta-2022.8.9/test/test_cvss.py
--rw-r--r--   0 ruth       (501) staff       (20)     8481 2022-07-31 09:29:32.000000 turvallisuusneuvonta-2022.8.9/test/test_turvallisuusneuvonta.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-09 03:17:03.128169 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/
--rw-r--r--   0 ruth       (501) staff       (20)      829 2022-08-09 03:15:09.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)      258 2021-12-08 16:02:41.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/__main__.py
--rw-r--r--   0 ruth       (501) staff       (20)     2168 2021-12-08 21:09:34.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/cli.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-09 03:17:03.132771 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/
--rw-r--r--   0 ruth       (501) staff       (20)       42 2021-12-18 16:26:42.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/__init__.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-09 03:17:03.133056 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/core/
--rw-r--r--   0 ruth       (501) staff       (20)        0 2021-12-08 17:12:18.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/core/__init__.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-09 03:17:03.133355 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/core/rules/
--rw-r--r--   0 ruth       (501) staff       (20)        0 2021-12-08 17:10:46.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/core/rules/__init__.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-09 03:17:03.138024 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/core/rules/mandatory/
--rw-r--r--   0 ruth       (501) staff       (20)     4439 2021-12-16 09:26:48.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/core/rules/mandatory/README.md
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-02-14 21:10:09.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/core/rules/mandatory/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)     1325 2021-12-16 11:48:56.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/core/rules/mandatory/acyclic_product_ids.py
--rw-r--r--   0 ruth       (501) staff       (20)     2023 2021-12-16 11:48:42.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/core/rules/mandatory/consistent_product_status.py
--rw-r--r--   0 ruth       (501) staff       (20)     1435 2022-02-13 17:11:58.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/core/rules/mandatory/defined_group_ids.py
--rw-r--r--   0 ruth       (501) staff       (20)     2548 2022-02-13 17:04:26.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/core/rules/mandatory/defined_product_ids.py
--rw-r--r--   0 ruth       (501) staff       (20)     5460 2022-02-14 21:43:11.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/core/rules/mandatory/mandatory.py
--rw-r--r--   0 ruth       (501) staff       (20)      981 2022-02-13 16:48:33.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/core/rules/mandatory/translator_and_source_lang.py
--rw-r--r--   0 ruth       (501) staff       (20)     1267 2022-02-13 20:44:51.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/core/rules/mandatory/unique_group_ids.py
--rw-r--r--   0 ruth       (501) staff       (20)     1192 2022-02-13 20:40:08.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/core/rules/mandatory/unique_product_ids.py
--rw-r--r--   0 ruth       (501) staff       (20)     2390 2022-02-13 16:48:33.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/core/rules/mandatory/valid_category_name.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-09 03:17:03.138336 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/core/schema/
--rw-r--r--   0 ruth       (501) staff       (20)    54123 2021-08-29 08:03:36.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/core/schema/csaf_2_0.json
--rw-r--r--   0 ruth       (501) staff       (20)     1455 2022-07-31 09:27:01.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/csaf.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-09 03:17:03.140154 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/cvss/
--rw-r--r--   0 ruth       (501) staff       (20)        0 2021-12-20 14:13:01.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/cvss/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)    10750 2021-12-20 14:21:58.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/cvss/cvss.py
--rw-r--r--   0 ruth       (501) staff       (20)     3354 2021-12-20 14:21:35.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/cvss/definitions.py
--rw-r--r--   0 ruth       (501) staff       (20)    12422 2022-07-31 09:28:01.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/definitions.py
--rw-r--r--   0 ruth       (501) staff       (20)    14945 2022-07-31 09:28:21.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/document.py
--rw-r--r--   0 ruth       (501) staff       (20)    16542 2022-07-31 09:29:24.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/product.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-09 03:17:03.142218 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/schema_proxy/
--rw-r--r--   0 ruth       (501) staff       (20)    54123 2021-08-29 08:03:36.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/schema_proxy/csaf_2_0.json
--rw-r--r--   0 ruth       (501) staff       (20)     5662 2021-12-18 16:01:59.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/schema_proxy/cvss-v2.0.json
--rw-r--r--   0 ruth       (501) staff       (20)     7591 2021-12-18 16:00:10.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/schema_proxy/cvss-v3.0.json
--rw-r--r--   0 ruth       (501) staff       (20)     7588 2021-12-18 16:00:13.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/schema_proxy/cvss-v3.1.json
--rw-r--r--   0 ruth       (501) staff       (20)    14906 2022-07-31 09:28:43.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/vulnerability.py
--rw-r--r--   0 ruth       (501) staff       (20)    14414 2022-02-14 22:10:02.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/turvallisuusneuvonta.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-08-09 03:17:03.130584 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta.egg-info/
--rw-r--r--   0 ruth       (501) staff       (20)     2526 2022-08-09 03:17:02.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta.egg-info/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     4764 2022-08-09 03:17:03.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta.egg-info/SOURCES.txt
--rw-r--r--   0 ruth       (501) staff       (20)        1 2022-08-09 03:17:02.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta.egg-info/dependency_links.txt
--rw-r--r--   0 ruth       (501) staff       (20)       70 2022-08-09 03:17:02.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta.egg-info/entry_points.txt
--rw-r--r--   0 ruth       (501) staff       (20)      185 2022-08-09 03:17:02.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta.egg-info/requires.txt
--rw-r--r--   0 ruth       (501) staff       (20)       21 2022-08-09 03:17:02.000000 turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta.egg-info/top_level.txt
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 19:14:58.730236 turvallisuusneuvonta-2023.6.18/
+-rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 turvallisuusneuvonta-2023.6.18/LICENSE
+-rw-r--r--   0 ruth       (501) staff       (20)       34 2021-05-12 16:52:51.000000 turvallisuusneuvonta-2023.6.18/MANIFEST.in
+-rw-r--r--   0 ruth       (501) staff       (20)     3500 2023-06-18 19:14:58.730097 turvallisuusneuvonta-2023.6.18/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     2370 2023-03-14 22:47:23.000000 turvallisuusneuvonta-2023.6.18/README.md
+-rw-r--r--   0 ruth       (501) staff       (20)     3200 2023-06-18 16:42:15.000000 turvallisuusneuvonta-2023.6.18/pyproject.toml
+-rw-r--r--   0 ruth       (501) staff       (20)       38 2023-06-18 19:14:58.730272 turvallisuusneuvonta-2023.6.18/setup.cfg
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 19:14:58.718796 turvallisuusneuvonta-2023.6.18/test/
+-rw-r--r--   0 ruth       (501) staff       (20)     1558 2022-07-09 16:07:06.000000 turvallisuusneuvonta-2023.6.18/test/test_cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)    13142 2022-07-09 16:08:10.000000 turvallisuusneuvonta-2023.6.18/test/test_csaf_core_rules_mandatory.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1326 2022-12-21 15:26:14.000000 turvallisuusneuvonta-2023.6.18/test/test_csaf_document.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2873 2022-12-21 15:26:55.000000 turvallisuusneuvonta-2023.6.18/test/test_csaf_meta.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2312 2022-12-21 15:27:33.000000 turvallisuusneuvonta-2023.6.18/test/test_csaf_product.py
+-rw-r--r--   0 ruth       (501) staff       (20)     8932 2023-06-18 19:09:24.000000 turvallisuusneuvonta-2023.6.18/test/test_csaf_vulnerability.py
+-rw-r--r--   0 ruth       (501) staff       (20)    13907 2023-06-18 19:08:16.000000 turvallisuusneuvonta-2023.6.18/test/test_cvss.py
+-rw-r--r--   0 ruth       (501) staff       (20)     8481 2022-07-31 09:29:32.000000 turvallisuusneuvonta-2023.6.18/test/test_turvallisuusneuvonta.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 19:14:58.720270 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/
+-rw-r--r--   0 ruth       (501) staff       (20)      830 2023-06-18 19:12:57.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)      258 2021-12-08 16:02:41.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/__main__.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2168 2021-12-08 21:09:34.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/cli.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 19:14:58.724500 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/
+-rw-r--r--   0 ruth       (501) staff       (20)       42 2021-12-18 16:26:42.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/__init__.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 19:14:58.724840 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/core/
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2021-12-08 17:12:18.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/core/__init__.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 19:14:58.725056 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/core/rules/
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2021-12-08 17:10:46.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/core/rules/__init__.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 19:14:58.729052 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/core/rules/mandatory/
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-02-14 21:10:09.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/core/rules/mandatory/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1325 2021-12-16 11:48:56.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/core/rules/mandatory/acyclic_product_ids.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2023 2021-12-16 11:48:42.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/core/rules/mandatory/consistent_product_status.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1435 2022-02-13 17:11:58.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/core/rules/mandatory/defined_group_ids.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2548 2022-02-13 17:04:26.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/core/rules/mandatory/defined_product_ids.py
+-rw-r--r--   0 ruth       (501) staff       (20)     5460 2022-02-14 21:43:11.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/core/rules/mandatory/mandatory.py
+-rw-r--r--   0 ruth       (501) staff       (20)      981 2022-02-13 16:48:33.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/core/rules/mandatory/translator_and_source_lang.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1267 2022-02-13 20:44:51.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/core/rules/mandatory/unique_group_ids.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1192 2022-02-13 20:40:08.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/core/rules/mandatory/unique_product_ids.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2390 2022-02-13 16:48:33.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/core/rules/mandatory/valid_category_name.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1601 2023-06-18 18:06:02.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/csaf.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 19:14:58.729911 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/cvss/
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2021-12-20 14:13:01.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/cvss/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)    11087 2023-06-18 19:09:24.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/cvss/cvss.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3338 2023-06-18 16:47:29.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/cvss/definitions.py
+-rw-r--r--   0 ruth       (501) staff       (20)    12422 2022-07-31 09:28:01.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/definitions.py
+-rw-r--r--   0 ruth       (501) staff       (20)    14945 2022-07-31 09:28:21.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/document.py
+-rw-r--r--   0 ruth       (501) staff       (20)    16542 2022-07-31 09:29:24.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/product.py
+-rw-r--r--   0 ruth       (501) staff       (20)    15182 2023-06-18 18:04:55.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/vulnerability.py
+-rw-r--r--   0 ruth       (501) staff       (20)    14426 2022-12-21 15:29:28.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/turvallisuusneuvonta.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 19:14:58.722524 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta.egg-info/
+-rw-r--r--   0 ruth       (501) staff       (20)     3500 2023-06-18 19:14:58.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta.egg-info/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     1802 2023-06-18 19:14:58.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta.egg-info/SOURCES.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        1 2023-06-18 19:14:58.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta.egg-info/dependency_links.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       70 2023-06-18 19:14:58.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta.egg-info/entry_points.txt
+-rw-r--r--   0 ruth       (501) staff       (20)      170 2023-06-18 19:14:58.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta.egg-info/requires.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       21 2023-06-18 19:14:58.000000 turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta.egg-info/top_level.txt
```

### Comparing `turvallisuusneuvonta-2022.8.9/PKG-INFO` & `turvallisuusneuvonta-2023.6.18/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,45 @@
-Metadata-Version: 2.1
-Name: turvallisuusneuvonta
-Version: 2022.8.9
-Summary: Security advisory (Finnish: turvallisuusneuvonta) audit tool.
-Home-page: https://git.sr.ht/~sthagen/turvallisuusneuvonta
-Author: Stefan Hagen
-Author-email: stefan@hagen.link
-Maintainer: Stefan Hagen
-Maintainer-email: stefan@hagen.link
-Project-URL: Bug Tracker, https://todo.sr.ht/~sthagen/turvallisuusneuvonta
-Project-URL: Documentation, https://codes.dilettant.life/docs/turvallisuusneuvonta
-Project-URL: Source Code, https://git.sr.ht/~sthagen/turvallisuusneuvonta
-Project-URL: Test Coverage, https://codes.dilettant.life/coverage/turvallisuusneuvonta
-Keywords: csaf,developer-tools,validation,verification
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-# turvallisuusneuvonta
+# Turvallisuusneuvonta
 
 Security advisory (Finnish: turvallisuusneuvonta) audit tool.
 
 [License: MIT](https://git.sr.ht/~sthagen/turvallisuusneuvonta/tree/default/item/LICENSE)
 
+Third party dependencies are documented in the folder [third-party](docs/third-party/README.md).
+
 [![version](https://img.shields.io/pypi/v/turvallisuusneuvonta.svg?style=flat)](https://pypi.python.org/pypi/turvallisuusneuvonta/)
 [![downloads](https://pepy.tech/badge/turvallisuusneuvonta/month)](https://pepy.tech/project/turvallisuusneuvonta)
 [![wheel](https://img.shields.io/pypi/wheel/turvallisuusneuvonta.svg?style=flat)](https://pypi.python.org/pypi/turvallisuusneuvonta/)
 [![supported-versions](https://img.shields.io/pypi/pyversions/turvallisuusneuvonta.svg?style=flat)](https://pypi.python.org/pypi/turvallisuusneuvonta/)
 [![supported-implementations](https://img.shields.io/pypi/implementation/turvallisuusneuvonta.svg?style=flat)](https://pypi.python.org/pypi/turvallisuusneuvonta/)
 
 ## Documentation
 
 User and developer [documentation of turvallisuusneuvonta](https://codes.dilettant.life/docs/turvallisuusneuvonta).
 
 ## Bug Tracker
 
-Feature requests and bug reports are bested entered in the [todos of turvallisuusneuvonta](https://todo.sr.ht/~sthagen/turvallisuusneuvonta).
+Any feature requests or bug reports shall go to the [todos of turvallisuusneuvonta](https://todo.sr.ht/~sthagen/turvallisuusneuvonta).
 
 ## Primary Source repository
 
-The primary source repository of [turvallisuusneuvonta is at sourcehut](https://git.sr.ht/~sthagen/turvallisuusneuvonta)
-a collection of tools useful for software development.
+The main source of `turvallisuusneuvonta` is on a mountain in central Switzerland.
+We use distributed version control (git).
+There is no central hub.
+Every clone can become a new source for the benefit of all.
+The preferred public clones of `turvallisuusneuvonta` are:
+
+* [on codeberg](https://codeberg.org/sthagen/turvallisuusneuvonta) - a democratic community-driven, non-profit software development platform operated by Codeberg e.V.
+* [at sourcehut](https://git.sr.ht/~sthagen/turvallisuusneuvonta) - a collection of tools useful for software development.
+
+## Contributions
+
+Please do not submit "pull requests" (I found no way to disable that "feature" on GitHub).
+If you like to share small changes under the repositories license please kindly do so by sending a patchset.
+You can either send such a patchset per email using [git send-email](https://git-send-email.io) or 
+if you are a sourcehut user by selecting "Prepare a patchset" on the summary page of your fork at [sourcehut](https://git.sr.ht/).
 
 ## Status
 
 Experimental.
 
 **Note**: The default branch is `default`.
```

### Comparing `turvallisuusneuvonta-2022.8.9/test/fixtures/rules/invalid/upstream/6-1-05-01.json` & `turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/core/rules/mandatory/unique_group_ids.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,84 +1,80 @@
-00000000: 7b0a 2020 2264 6f63 756d 656e 7422 3a20  {.  "document": 
-00000010: 7b0a 2020 2020 2263 6174 6567 6f72 7922  {.    "category"
-00000020: 3a20 2267 656e 6572 6963 5f63 7361 6622  : "generic_csaf"
-00000030: 2c0a 2020 2020 2263 7361 665f 7665 7273  ,.    "csaf_vers
-00000040: 696f 6e22 3a20 2232 2e30 222c 0a20 2020  ion": "2.0",.   
-00000050: 2022 7075 626c 6973 6865 7222 3a20 7b0a   "publisher": {.
-00000060: 2020 2020 2020 2263 6174 6567 6f72 7922        "category"
-00000070: 3a20 226f 7468 6572 222c 0a20 2020 2020  : "other",.     
-00000080: 2022 6e61 6d65 223a 2022 4f41 5349 5320   "name": "OASIS 
-00000090: 4353 4146 2054 4322 2c0a 2020 2020 2020  CSAF TC",.      
-000000a0: 226e 616d 6573 7061 6365 223a 2022 6874  "namespace": "ht
-000000b0: 7470 733a 2f2f 6373 6166 2e69 6f22 0a20  tps://csaf.io". 
-000000c0: 2020 207d 2c0a 2020 2020 2274 6974 6c65     },.    "title
-000000d0: 223a 2022 4d61 6e64 6174 6f72 7920 7465  ": "Mandatory te
-000000e0: 7374 3a20 4d75 6c74 6970 6c65 2044 6566  st: Multiple Def
-000000f0: 696e 6974 696f 6e20 6f66 2050 726f 6475  inition of Produ
-00000100: 6374 2047 726f 7570 2049 4420 2866 6169  ct Group ID (fai
-00000110: 6c69 6e67 2065 7861 6d70 6c65 2031 2922  ling example 1)"
-00000120: 2c0a 2020 2020 2274 7261 636b 696e 6722  ,.    "tracking"
-00000130: 3a20 7b0a 2020 2020 2020 2263 7572 7265  : {.      "curre
-00000140: 6e74 5f72 656c 6561 7365 5f64 6174 6522  nt_release_date"
-00000150: 3a20 2232 3032 312d 3037 2d32 3154 3130  : "2021-07-21T10
-00000160: 3a30 303a 3030 2e30 3030 5a22 2c0a 2020  :00:00.000Z",.  
-00000170: 2020 2020 2269 6422 3a20 224f 4153 4953      "id": "OASIS
-00000180: 5f43 5341 465f 5443 2d43 5341 465f 322e  _CSAF_TC-CSAF_2.
-00000190: 302d 3230 3231 2d36 2d31 2d30 352d 3031  0-2021-6-1-05-01
-000001a0: 222c 0a20 2020 2020 2022 696e 6974 6961  ",.      "initia
-000001b0: 6c5f 7265 6c65 6173 655f 6461 7465 223a  l_release_date":
-000001c0: 2022 3230 3231 2d30 372d 3231 5431 303a   "2021-07-21T10:
-000001d0: 3030 3a30 302e 3030 305a 222c 0a20 2020  00:00.000Z",.   
-000001e0: 2020 2022 7265 7669 7369 6f6e 5f68 6973     "revision_his
-000001f0: 746f 7279 223a 205b 0a20 2020 2020 2020  tory": [.       
-00000200: 207b 0a20 2020 2020 2020 2020 2022 6461   {.          "da
-00000210: 7465 223a 2022 3230 3231 2d30 372d 3231  te": "2021-07-21
-00000220: 5431 303a 3030 3a30 302e 3030 305a 222c  T10:00:00.000Z",
-00000230: 0a20 2020 2020 2020 2020 2022 6e75 6d62  .          "numb
-00000240: 6572 223a 2022 3122 2c0a 2020 2020 2020  er": "1",.      
-00000250: 2020 2020 2273 756d 6d61 7279 223a 2022      "summary": "
-00000260: 496e 6974 6961 6c20 7665 7273 696f 6e2e  Initial version.
-00000270: 220a 2020 2020 2020 2020 7d0a 2020 2020  ".        }.    
-00000280: 2020 5d2c 0a20 2020 2020 2022 7374 6174    ],.      "stat
-00000290: 7573 223a 2022 6669 6e61 6c22 2c0a 2020  us": "final",.  
-000002a0: 2020 2020 2276 6572 7369 6f6e 223a 2022      "version": "
-000002b0: 3122 0a20 2020 207d 0a20 207d 2c0a 2020  1".    }.  },.  
-000002c0: 2270 726f 6475 6374 5f74 7265 6522 3a20  "product_tree": 
-000002d0: 7b0a 2020 2020 2266 756c 6c5f 7072 6f64  {.    "full_prod
-000002e0: 7563 745f 6e61 6d65 7322 3a20 5b0a 2020  uct_names": [.  
-000002f0: 2020 2020 7b0a 2020 2020 2020 2020 2270      {.        "p
-00000300: 726f 6475 6374 5f69 6422 3a20 2243 5341  roduct_id": "CSA
-00000310: 4650 4944 2d39 3038 3037 3030 222c 0a20  FPID-9080700",. 
-00000320: 2020 2020 2020 2022 6e61 6d65 223a 2022         "name": "
-00000330: 5072 6f64 7563 7420 4122 0a20 2020 2020  Product A".     
-00000340: 207d 2c0a 2020 2020 2020 7b0a 2020 2020   },.      {.    
-00000350: 2020 2020 2270 726f 6475 6374 5f69 6422      "product_id"
-00000360: 3a20 2243 5341 4650 4944 2d39 3038 3037  : "CSAFPID-90807
-00000370: 3031 222c 0a20 2020 2020 2020 2022 6e61  01",.        "na
-00000380: 6d65 223a 2022 5072 6f64 7563 7420 4222  me": "Product B"
-00000390: 0a20 2020 2020 207d 2c0a 2020 2020 2020  .      },.      
-000003a0: 7b0a 2020 2020 2020 2020 2270 726f 6475  {.        "produ
-000003b0: 6374 5f69 6422 3a20 2243 5341 4650 4944  ct_id": "CSAFPID
-000003c0: 2d39 3038 3037 3032 222c 0a20 2020 2020  -9080702",.     
-000003d0: 2020 2022 6e61 6d65 223a 2022 5072 6f64     "name": "Prod
-000003e0: 7563 7420 4322 0a20 2020 2020 207d 0a20  uct C".      }. 
-000003f0: 2020 205d 2c0a 2020 2020 2270 726f 6475     ],.    "produ
-00000400: 6374 5f67 726f 7570 7322 3a20 5b0a 2020  ct_groups": [.  
-00000410: 2020 2020 7b0a 2020 2020 2020 2020 2267      {.        "g
-00000420: 726f 7570 5f69 6422 3a20 2243 5341 4647  roup_id": "CSAFG
-00000430: 4944 2d31 3032 3033 3030 222c 0a20 2020  ID-1020300",.   
-00000440: 2020 2020 2022 7072 6f64 7563 745f 6964       "product_id
-00000450: 7322 3a20 5b0a 2020 2020 2020 2020 2020  s": [.          
-00000460: 2243 5341 4650 4944 2d39 3038 3037 3030  "CSAFPID-9080700
-00000470: 222c 0a20 2020 2020 2020 2020 2022 4353  ",.          "CS
-00000480: 4146 5049 442d 3930 3830 3730 3122 0a20  AFPID-9080701". 
-00000490: 2020 2020 2020 205d 0a20 2020 2020 207d         ].      }
-000004a0: 2c0a 2020 2020 2020 7b0a 2020 2020 2020  ,.      {.      
-000004b0: 2020 2267 726f 7570 5f69 6422 3a20 2243    "group_id": "C
-000004c0: 5341 4647 4944 2d31 3032 3033 3030 222c  SAFGID-1020300",
-000004d0: 0a20 2020 2020 2020 2022 7072 6f64 7563  .        "produc
-000004e0: 745f 6964 7322 3a20 5b0a 2020 2020 2020  t_ids": [.      
-000004f0: 2020 2020 2243 5341 4650 4944 2d39 3038      "CSAFPID-908
-00000500: 3037 3030 222c 0a20 2020 2020 2020 2020  0700",.         
-00000510: 2022 4353 4146 5049 442d 3930 3830 3730   "CSAFPID-908070
-00000520: 3222 0a20 2020 2020 2020 205d 0a20 2020  2".        ].   
-00000530: 2020 207d 0a20 2020 205d 0a20 207d 0a7d     }.    ].  }.}
+00000000: 2222 2236 2e31 2e35 204d 756c 7469 706c  """6.1.5 Multipl
+00000010: 6520 4465 6669 6e69 7469 6f6e 206f 6620  e Definition of 
+00000020: 5072 6f64 7563 7420 4772 6f75 7020 4944  Product Group ID
+00000030: 0a0a 466f 7220 6561 6368 2050 726f 6475  ..For each Produ
+00000040: 6374 2047 726f 7570 2049 4420 2874 7970  ct Group ID (typ
+00000050: 6520 2f24 6465 6673 2f70 726f 6475 6374  e /$defs/product
+00000060: 5f67 726f 7570 5f69 645f 7429 2050 726f  _group_id_t) Pro
+00000070: 6475 6374 2047 726f 7570 2065 6c65 6d65  duct Group eleme
+00000080: 6e74 7320 282f 7072 6f64 7563 745f 7472  nts (/product_tr
+00000090: 6565 2f70 726f 6475 6374 5f67 726f 7570  ee/product_group
+000000a0: 735b 5d29 0a69 7420 6d75 7374 2062 6520  s[]).it must be 
+000000b0: 7465 7374 6564 2074 6861 7420 7468 6520  tested that the 
+000000c0: 6772 6f75 705f 6964 2077 6173 206e 6f74  group_id was not
+000000d0: 2061 6c72 6561 6479 2064 6566 696e 6564   already defined
+000000e0: 2077 6974 6869 6e20 7468 6520 7361 6d65   within the same
+000000f0: 2064 6f63 756d 656e 742e 0a0a 5468 6520   document...The 
+00000100: 7265 6c65 7661 6e74 2070 6174 6820 666f  relevant path fo
+00000110: 7220 7468 6973 2074 6573 7420 6973 3a0a  r this test is:.
+00000120: 0a20 2020 202f 7072 6f64 7563 745f 7472  .    /product_tr
+00000130: 6565 2f70 726f 6475 6374 5f67 726f 7570  ee/product_group
+00000140: 735b 5d2f 6772 6f75 705f 6964 0a0a 4578  s[]/group_id..Ex
+00000150: 616d 706c 6520 3434 2077 6869 6368 2066  ample 44 which f
+00000160: 6169 6c73 2074 6865 2074 6573 743a 0a0a  ails the test:..
+00000170: 2020 2270 726f 6475 6374 5f74 7265 6522    "product_tree"
+00000180: 3a20 7b0a 2020 2020 2266 756c 6c5f 7072  : {.    "full_pr
+00000190: 6f64 7563 745f 6e61 6d65 7322 3a20 5b0a  oduct_names": [.
+000001a0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+000001b0: 2270 726f 6475 6374 5f69 6422 3a20 2243  "product_id": "C
+000001c0: 5341 4650 4944 2d39 3038 3037 3030 222c  SAFPID-9080700",
+000001d0: 0a20 2020 2020 2020 2022 6e61 6d65 223a  .        "name":
+000001e0: 2022 5072 6f64 7563 7420 4122 0a20 2020   "Product A".   
+000001f0: 2020 207d 2c0a 2020 2020 2020 7b0a 2020     },.      {.  
+00000200: 2020 2020 2020 2270 726f 6475 6374 5f69        "product_i
+00000210: 6422 3a20 2243 5341 4650 4944 2d39 3038  d": "CSAFPID-908
+00000220: 3037 3031 222c 0a20 2020 2020 2020 2022  0701",.        "
+00000230: 6e61 6d65 223a 2022 5072 6f64 7563 7420  name": "Product 
+00000240: 4222 0a20 2020 2020 207d 2c0a 2020 2020  B".      },.    
+00000250: 2020 7b0a 2020 2020 2020 2020 2270 726f    {.        "pro
+00000260: 6475 6374 5f69 6422 3a20 2243 5341 4650  duct_id": "CSAFP
+00000270: 4944 2d39 3038 3037 3032 222c 0a20 2020  ID-9080702",.   
+00000280: 2020 2020 2022 6e61 6d65 223a 2022 5072       "name": "Pr
+00000290: 6f64 7563 7420 4322 0a20 2020 2020 207d  oduct C".      }
+000002a0: 0a20 2020 205d 2c0a 2020 2020 2270 726f  .    ],.    "pro
+000002b0: 6475 6374 5f67 726f 7570 7322 3a20 5b0a  duct_groups": [.
+000002c0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+000002d0: 2267 726f 7570 5f69 6422 3a20 2243 5341  "group_id": "CSA
+000002e0: 4647 4944 2d31 3032 3033 3030 222c 0a20  FGID-1020300",. 
+000002f0: 2020 2020 2020 2022 7072 6f64 7563 745f         "product_
+00000300: 6964 7322 3a20 5b0a 2020 2020 2020 2020  ids": [.        
+00000310: 2020 2243 5341 4650 4944 2d39 3038 3037    "CSAFPID-90807
+00000320: 3030 222c 0a20 2020 2020 2020 2020 2022  00",.          "
+00000330: 4353 4146 5049 442d 3930 3830 3730 3122  CSAFPID-9080701"
+00000340: 0a20 2020 2020 2020 205d 0a20 2020 2020  .        ].     
+00000350: 207d 2c0a 2020 2020 2020 7b0a 2020 2020   },.      {.    
+00000360: 2020 2020 2267 726f 7570 5f69 6422 3a20      "group_id": 
+00000370: 2243 5341 4647 4944 2d31 3032 3033 3030  "CSAFGID-1020300
+00000380: 222c 0a20 2020 2020 2020 2022 7072 6f64  ",.        "prod
+00000390: 7563 745f 6964 7322 3a20 5b0a 2020 2020  uct_ids": [.    
+000003a0: 2020 2020 2020 2243 5341 4650 4944 2d39        "CSAFPID-9
+000003b0: 3038 3037 3030 222c 0a20 2020 2020 2020  080700",.       
+000003c0: 2020 2022 4353 4146 5049 442d 3930 3830     "CSAFPID-9080
+000003d0: 3730 3222 0a20 2020 2020 2020 205d 0a20  702".        ]. 
+000003e0: 2020 2020 207d 0a20 2020 205d 0a20 207d       }.    ].  }
+000003f0: 0a0a 4353 4146 4749 442d 3130 3230 3330  ..CSAFGID-102030
+00000400: 3020 7761 7320 6465 6669 6e65 6420 7477  0 was defined tw
+00000410: 6963 652e 0a22 2222 0a0a 4944 203d 2028  ice.."""..ID = (
+00000420: 362c 2031 2c20 3529 0a54 4f50 4943 203d  6, 1, 5).TOPIC =
+00000430: 2027 4d75 6c74 6970 6c65 2044 6566 696e   'Multiple Defin
+00000440: 6974 696f 6e20 6f66 2050 726f 6475 6374  ition of Product
+00000450: 2047 726f 7570 2049 4427 0a43 4f4e 4449   Group ID'.CONDI
+00000460: 5449 4f4e 5f50 4154 4820 3d20 272f 7072  TION_PATH = '/pr
+00000470: 6f64 7563 745f 7472 6565 2f70 726f 6475  oduct_tree/produ
+00000480: 6374 5f67 726f 7570 735b 5d2f 6772 6f75  ct_groups[]/grou
+00000490: 705f 6964 270a 434f 4e44 4954 494f 4e5f  p_id'.CONDITION_
+000004a0: 4a4d 4553 5f50 4154 4820 3d20 434f 4e44  JMES_PATH = COND
+000004b0: 4954 494f 4e5f 5041 5448 2e6c 7374 7269  ITION_PATH.lstri
+000004c0: 7028 272f 2729 2e72 6570 6c61 6365 2827  p('/').replace('
+000004d0: 2f27 2c20 272e 2729 0a50 4154 4853 203d  /', '.').PATHS =
+000004e0: 2028 434f 4e44 4954 494f 4e5f 5041 5448   (CONDITION_PATH
+000004f0: 2c29 0a                                  ,).
```

### Comparing `turvallisuusneuvonta-2022.8.9/test/test_cli.py` & `turvallisuusneuvonta-2023.6.18/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `turvallisuusneuvonta-2022.8.9/test/test_csaf_core_rules_mandatory.py` & `turvallisuusneuvonta-2023.6.18/test/test_csaf_core_rules_mandatory.py`

 * *Files identical despite different names*

### Comparing `turvallisuusneuvonta-2022.8.9/test/test_csaf_document.py` & `turvallisuusneuvonta-2023.6.18/test/test_csaf_document.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # pylint: disable=line-too-long,missing-docstring,reimported,unused-import,unused-variable
 from test import conftest
 
-import orjson
+import msgspec
 import pytest
 from pydantic.error_wrappers import ValidationError
 
 import turvallisuusneuvonta.csaf.csaf as csaf
 
 
 def _subs(count: int, what: str) -> str:
@@ -22,15 +22,15 @@
     assert '\npublisher\n  field required' in str(err.value)
     assert '\ntitle\n  field required' in str(err.value)
     assert '\ntracking\n  field required' in str(err.value)
 
 
 def test_doc_ok_if_spammy():
     doc = csaf.CSAF(**conftest.DOC_OK)
-    strip_me = orjson.loads(doc.json())
+    strip_me = msgspec.json.decode(doc.json())
     conftest._strip_and_iso_grace(strip_me)
     assert strip_me == conftest.DOC_OK
 
 
 def test_doc_vulnerability_empty():
     with pytest.raises(ValidationError, match=_subs(1, 'CSAF')) as err:
         _ = csaf.CSAF(**conftest.DOC_VULN_EMPTY)
```

### Comparing `turvallisuusneuvonta-2022.8.9/test/test_csaf_meta.py` & `turvallisuusneuvonta-2023.6.18/test/test_csaf_meta.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # pylint: disable=line-too-long,missing-docstring,reimported,unused-import,unused-variable
 from test import conftest
 
-import orjson
+import msgspec
 import pytest
 from pydantic.error_wrappers import ValidationError
 
 import turvallisuusneuvonta.csaf.document as document
 
 
 def _subs(count: int) -> str:
@@ -61,10 +61,10 @@
     host = 'tracking'
     for prop in ('current_release_date', 'id', 'initial_release_date', 'revision_history', 'status', 'version'):
         assert f'\n{host} -> {prop}\n  field required' in str(err.value)
 
 
 def test_meta_doc_ok_if_spammy():
     meta_doc = document.Document(**conftest.META_OK)  # type: ignore
-    strip_me = orjson.loads(meta_doc.json())
+    strip_me = msgspec.json.decode(meta_doc.json())
     conftest._strip_and_iso_grace(strip_me)
     assert strip_me == conftest.META_OK
```

### Comparing `turvallisuusneuvonta-2022.8.9/test/test_csaf_product.py` & `turvallisuusneuvonta-2023.6.18/test/test_csaf_product.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # pylint: disable=line-too-long,missing-docstring,reimported,unused-import,unused-variable
 import re
 from test import conftest
 
-import orjson
+import msgspec
 import pytest
 
 import turvallisuusneuvonta.csaf.definitions as defs
 import turvallisuusneuvonta.csaf.product as product
 
 
 def test_product_empty():
@@ -35,15 +35,15 @@
     }
     rel = product.Relationship(**data)
     assert rel.category == product.RelationshipCategory.installed_with
 
 
 def test_product_relationship_loads():
     rel = product.Relationship(**conftest.PRODUCT_RELATIONSHIP_DATA)
-    assert orjson.loads(rel.json()) == conftest.PRODUCT_RELATIONSHIP_DATA
+    assert msgspec.json.decode(rel.json()) == conftest.PRODUCT_RELATIONSHIP_DATA
 
 
 def test_product_relationship_dumps():
     pr_ref_other = product.ReferenceTokenForProductInstance(value='acme-101')
     pr_ref_self = product.ReferenceTokenForProductInstance(value='acme-112')
     pr_id = pr_ref_self
     pr_ids = product.Products(__root__=['acme-101', 'acme-112'])
@@ -52,8 +52,8 @@
     data = {
         'category': product.RelationshipCategory.installed_with,
         'full_product_name': pr_name,
         'product_reference': pr_ref_self,
         'relates_to_product_reference': pr_ref_other,
     }
     rel = product.Relationship(**data)
-    assert orjson.loads(rel.json()) == conftest.PRODUCT_RELATIONSHIP_DATA
+    assert msgspec.json.decode(rel.json()) == conftest.PRODUCT_RELATIONSHIP_DATA
```

### Comparing `turvallisuusneuvonta-2022.8.9/test/test_csaf_vulnerability.py` & `turvallisuusneuvonta-2023.6.18/test/test_csaf_vulnerability.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # -*- coding: utf-8 -*-
 # pylint: disable=line-too-long,missing-docstring,reimported,unused-import,unused-variable
+import json
 import re
 from test import conftest
 
-import orjson
+import msgspec
 import pytest
 from pydantic.error_wrappers import ValidationError
 
 import turvallisuusneuvonta.csaf.product as product
 import turvallisuusneuvonta.csaf.vulnerability as vulnerability
-from turvallisuusneuvonta.csaf.cvss.cvss import CVSS31, SeverityType, Version as CvssVersion
+from turvallisuusneuvonta.csaf.cvss.cvss import CVSS31
 
-CVSS31_BASE_SEVERITY_LOG4J = SeverityType.critical
+# , SeverityType, Version as CvssVersion
+
+CVSS31_BASE_SEVERITY_LOG4J = 'CRITICAL'  # str(SeverityType.critical)
 
 
 def test_vulnerability_empty():
     assert isinstance(vulnerability.Vulnerability(), vulnerability.Vulnerability)
 
 
 def test_vulnerability_text():
@@ -28,44 +31,46 @@
     message = '__init__() takes exactly 1 positional argument (2 given)'
     with pytest.raises(TypeError, match=re.escape(message)):
         _ = vulnerability.Score('text')  # type: ignore
 
 
 def test_vulnerability_score_cvss31_log4j_cve_2021_44228():
     data = {
-        'version': CvssVersion.three_wun,
-        'vector_string': conftest.CVSS31_VECTOR_STRING_LOG4J,
-        'base_score': conftest.CVSS31_BASE_SCORE_LOG4J,
-        'base_severity': CVSS31_BASE_SEVERITY_LOG4J,
+        'version': '3.1',  # str(CvssVersion.three_wun),
+        'vectorString': conftest.CVSS31_VECTOR_STRING_LOG4J,
+        'baseScore': conftest.CVSS31_BASE_SCORE_LOG4J,
+        'baseSeverity': CVSS31_BASE_SEVERITY_LOG4J,
     }
-    cvss_cve_2021_44228 = CVSS31(**data)
+    as_json = json.dumps(data)
+    cvss_cve_2021_44228 = CVSS31.parse_raw(as_json)
     message = '1 validation error for Score'
     with pytest.raises(ValidationError, match=message) as err:
         _ = vulnerability.Score(cvss_v3=cvss_cve_2021_44228, products=[])  # type: ignore
     assert '\nproducts -> __root__\n  ensure this value has at least 1 items' in str(err.value)
 
 
 def test_vulnerability_score_cvss31_log4j_cve_2021_44228_product_foo():
     data = {
-        'version': CvssVersion.three_wun,
-        'vector_string': conftest.CVSS31_VECTOR_STRING_LOG4J,
-        'base_score': conftest.CVSS31_BASE_SCORE_LOG4J,
-        'base_severity': CVSS31_BASE_SEVERITY_LOG4J,
+        'version': '3.1',  # str(CvssVersion.three_wun),
+        'vectorString': conftest.CVSS31_VECTOR_STRING_LOG4J,
+        'baseScore': conftest.CVSS31_BASE_SCORE_LOG4J,
+        'baseSeverity': CVSS31_BASE_SEVERITY_LOG4J,
     }
     # pr_ref = product.ReferenceTokenForProductInstance(value='log4j-123')
     products = product.Products(__root__=['log4j-123'])
-    cvss_cve_2021_44228 = CVSS31(**data)
+    as_json = json.dumps(data)
+    cvss_cve_2021_44228 = CVSS31.parse_raw(as_json)
     score = vulnerability.Score(cvss_v3=cvss_cve_2021_44228, products=products)
     assert score.cvss_v3 == cvss_cve_2021_44228
     assert score.products == products
 
 
 def test_vulnerability_score_loads_cvss31_log4j_cve_2021_44228_product_foo():
-    score = vulnerability.Score(**conftest.VULNERABILITY_SCORE_LOG4J)
-    assert orjson.loads(score.json()) == conftest.VULNERABILITY_SCORE_LOG4J
+    score = vulnerability.Score.parse_raw(json.dumps(conftest.VULNERABILITY_SCORE_LOG4J))
+    assert msgspec.json.decode(score.json()) == conftest.VULNERABILITY_SCORE_LOG4J
 
 
 def test_vulnerability_cwe_text():
     message = '__init__() takes exactly 1 positional argument (2 given)'
     with pytest.raises(TypeError, match=re.escape(message)):
         _ = vulnerability.Cwe('text')  # type: ignore
```

### Comparing `turvallisuusneuvonta-2022.8.9/test/test_turvallisuusneuvonta.py` & `turvallisuusneuvonta-2023.6.18/test/test_turvallisuusneuvonta.py`

 * *Files identical despite different names*

### Comparing `turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/__init__.py` & `turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Security advisory (Finnish: turvallisuusneuvonta) audit tool."""
 # [[[fill git_describe()]]]
-__version__ = '2022.8.9+parent.3233165e'
-# [[[end]]] (checksum: ec2cc12146ac51673531f0f6ebebef47)
+__version__ = '2023.6.18+parent.dd252054'
+# [[[end]]] (checksum: ed24f138a6c1f4ed1846f228247c7db7)
 __version_info__ = tuple(
     e if '-' not in e else e.split('-')[0] for part in __version__.split('+') for e in part.split('.') if e != 'parent'
 )
 
 from turvallisuusneuvonta.csaf.core.rules.mandatory.mandatory import (
     is_valid,
     is_valid_category,
```

### Comparing `turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/cli.py` & `turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/cli.py`

 * *Files identical despite different names*

### Comparing `turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/core/rules/mandatory/acyclic_product_ids.py` & `turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/core/rules/mandatory/acyclic_product_ids.py`

 * *Files identical despite different names*

### Comparing `turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/core/rules/mandatory/consistent_product_status.py` & `turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/core/rules/mandatory/consistent_product_status.py`

 * *Files identical despite different names*

### Comparing `turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/core/rules/mandatory/defined_group_ids.py` & `turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/core/rules/mandatory/defined_group_ids.py`

 * *Files identical despite different names*

### Comparing `turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/core/rules/mandatory/defined_product_ids.py` & `turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/core/rules/mandatory/defined_product_ids.py`

 * *Files identical despite different names*

### Comparing `turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/core/rules/mandatory/mandatory.py` & `turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/core/rules/mandatory/mandatory.py`

 * *Files identical despite different names*

### Comparing `turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/core/rules/mandatory/translator_and_source_lang.py` & `turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/core/rules/mandatory/translator_and_source_lang.py`

 * *Files identical despite different names*

### Comparing `turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/core/rules/mandatory/unique_product_ids.py` & `turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/core/rules/mandatory/unique_product_ids.py`

 * *Files identical despite different names*

### Comparing `turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/core/rules/mandatory/valid_category_name.py` & `turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/core/rules/mandatory/valid_category_name.py`

 * *Files identical despite different names*

### Comparing `turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/csaf.py` & `turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/csaf.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,13 +37,18 @@
             description='Represents a list of all relevant vulnerability information items.',
             min_items=1,
             title='Vulnerabilities',
         ),
     ]
 
     @no_type_check
+    def json(self, *args, **kwargs):
+        kwargs.setdefault('by_alias', True)
+        return super().json(*args, **kwargs)
+
+    @no_type_check
     @validator('vulnerabilities')
     @classmethod
     def check_len(cls, v):
         if not v:
             raise ValueError('vulnerabilities present but empty')
         return v
```

### Comparing `turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/cvss/cvss.py` & `turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/cvss/cvss.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """CSAF CVSS 2/3.0/3.1 proxy implementation."""
 
 from __future__ import annotations
 
 from enum import Enum
-from typing import Annotated, Optional
+from typing import Annotated, Optional, no_type_check
 
 from pydantic import BaseModel, Field
 
 from turvallisuusneuvonta.csaf.cvss.definitions import (
     AccessComplexityType,
     AccessVectorType,
     AttackComplexityType,
@@ -47,152 +47,163 @@
 
 
 class CVSS2(BaseModel):
     version: Annotated[Version, Field(description='CVSS Version')] = Version.two
     vector_string: Annotated[
         str,
         Field(
-            alias='vector_string',
+            alias='vectorString',
             regex=(
                 '^((AV:[NAL]|AC:[LMH]|Au:[MSN]|[CIA]:[NPC]|E:(U|POC|F|H|ND)|RL:(OF|TF|W|U|ND)|RC:(UC|UR|C|ND)|CDP:'
                 '(N|L|LM|MH|H|ND)|TD:(N|L|M|H|ND)|[CIA]R:(L|M|H|ND))/)*(AV:[NAL]|AC:[LMH]|Au:[MSN]|[CIA]:[NPC]|E:'
                 '(U|POC|F|H|ND)|RL:(OF|TF|W|U|ND)|RC:(UC|UR|C|ND)|CDP:(N|L|LM|MH|H|ND)|TD:(N|L|M|H|ND)|[CIA]R:'
                 '(L|M|H|ND))$'
             ),
         ),
     ]
-    access_vector: Annotated[Optional[AccessVectorType], Field(alias='access_vector')] = None
-    access_complexity: Annotated[Optional[AccessComplexityType], Field(alias='access_complexity')] = None
+    access_vector: Annotated[Optional[AccessVectorType], Field(alias='accessVector')] = None
+    access_complexity: Annotated[Optional[AccessComplexityType], Field(alias='accessComplexity')] = None
     authentication: Optional[AuthenticationType] = None
-    confidentiality_impact: Annotated[Optional[CiaType], Field(alias='confidentiality_impact')] = None
-    integrity_impact: Annotated[Optional[CiaType], Field(alias='integrity_impact')] = None
-    availability_impact: Annotated[Optional[CiaType], Field(alias='availability_impact')] = None
-    base_score: Annotated[ScoreType, Field(alias='base_score')]
+    confidentiality_impact: Annotated[Optional[CiaType], Field(alias='confidentialityImpact')] = None
+    integrity_impact: Annotated[Optional[CiaType], Field(alias='integrityImpact')] = None
+    availability_impact: Annotated[Optional[CiaType], Field(alias='availabilityImpact')] = None
+    base_score: Annotated[ScoreType, Field(alias='baseScore')]
     exploitability: Optional[ExploitabilityType] = None
-    remediation_level: Annotated[Optional[RemediationLevelType], Field(alias='remediation_level')] = None
-    report_confidence: Annotated[Optional[ReportConfidenceType], Field(alias='report_confidence')] = None
-    temporal_score: Annotated[Optional[ScoreType], Field(alias='temporal_score')] = None
+    remediation_level: Annotated[Optional[RemediationLevelType], Field(alias='remediationLevel')] = None
+    report_confidence: Annotated[Optional[ReportConfidenceType], Field(alias='reportConfidence')] = None
+    temporal_score: Annotated[Optional[ScoreType], Field(alias='temporalScore')] = None
     collateral_damage_potential: Annotated[
         Optional[CollateralDamagePotentialType],
-        Field(alias='collateral_damage_potential'),
+        Field(alias='collateralDamagePotential'),
     ] = None
-    target_distribution: Annotated[Optional[TargetDistributionType], Field(alias='target_distribution')] = None
+    target_distribution: Annotated[Optional[TargetDistributionType], Field(alias='targetDistribution')] = None
     confidentiality_requirement: Annotated[
-        Optional[CiaRequirementType], Field(alias='confidentiality_requirement')
+        Optional[CiaRequirementType], Field(alias='confidentialityRequirement')
     ] = None
-    integrity_requirement: Annotated[Optional[CiaRequirementType], Field(alias='integrity_requirement')] = None
-    availability_requirement: Annotated[Optional[CiaRequirementType], Field(alias='availability_requirement')] = None
-    environmental_score: Annotated[Optional[ScoreType], Field(alias='environmental_score')] = None
+    integrity_requirement: Annotated[Optional[CiaRequirementType], Field(alias='integrityRequirement')] = None
+    availability_requirement: Annotated[Optional[CiaRequirementType], Field(alias='availabilityRequirement')] = None
+    environmental_score: Annotated[Optional[ScoreType], Field(alias='environmentalScore')] = None
+
+    @no_type_check
+    def json(self, *args, **kwargs):
+        kwargs.setdefault('by_alias', True)
+        return super().json(*args, **kwargs)
 
 
 class CVSS30(BaseModel):
     version: Annotated[Version, Field(description='CVSS Version')] = Version.three_zero
     vector_string: Annotated[
         str,
         Field(
-            alias='vector_string',
+            alias='vectorString',
             regex=(
                 '^CVSS:3[.]0/((AV:[NALP]|AC:[LH]|PR:[UNLH]|UI:[NR]|S:[UC]|[CIA]:[NLH]|E:[XUPFH]|RL:[XOTWU]|RC:[XURC]|'
                 '[CIA]R:[XLMH]|MAV:[XNALP]|MAC:[XLH]|MPR:[XUNLH]|MUI:[XNR]|MS:[XUC]|M[CIA]:[XNLH])/)*(AV:[NALP]|'
                 'AC:[LH]|PR:[UNLH]|UI:[NR]|S:[UC]|[CIA]:[NLH]|E:[XUPFH]|RL:[XOTWU]|RC:[XURC]|[CIA]R:[XLMH]|'
                 'MAV:[XNALP]|MAC:[XLH]|MPR:[XUNLH]|MUI:[XNR]|MS:[XUC]|M[CIA]:[XNLH])$'
             ),
         ),
     ]
-    attack_vector: Annotated[Optional[AttackVectorType], Field(alias='attack_vector')] = None
-    attack_complexity: Annotated[Optional[AttackComplexityType], Field(alias='attack_complexity')] = None
-    privileges_required: Annotated[Optional[PrivilegesRequiredType], Field(alias='privileges_required')] = None
+    attack_vector: Annotated[Optional[AttackVectorType], Field(alias='attackVector')] = None
+    attack_complexity: Annotated[Optional[AttackComplexityType], Field(alias='attackComplexity')] = None
+    privileges_required: Annotated[Optional[PrivilegesRequiredType], Field(alias='privilegesRequired')] = None
     user_interaction: Annotated[Optional[UserInteractionType], Field(alias='user_interaction')] = None
     scope: Optional[ScopeType] = None
-    confidentiality_impact: Annotated[Optional[CiaType], Field(alias='confidentiality_impact')] = None
-    integrity_impact: Annotated[Optional[CiaType], Field(alias='integrity_impact')] = None
-    availability_impact: Annotated[Optional[CiaType], Field(alias='availability_impact')] = None
-    base_score: Annotated[ScoreType, Field(alias='base_score')]
-    base_severity: Annotated[SeverityType, Field(alias='base_severity')]
-    exploit_code_maturity: Annotated[Optional[ExploitCodeMaturityType], Field(alias='exploit_code_maturity')] = None
-    remediation_level: Annotated[Optional[RemediationLevelType], Field(alias='remediation_level')] = None
-    report_confidence: Annotated[Optional[ConfidenceType], Field(alias='report_confidence')] = None
-    temporal_score: Annotated[Optional[ScoreType], Field(alias='temporal_score')] = None
-    temporal_severity: Annotated[Optional[SeverityType], Field(alias='temporal_severity')] = None
+    confidentiality_impact: Annotated[Optional[CiaType], Field(alias='confidentialityImpact')] = None
+    integrity_impact: Annotated[Optional[CiaType], Field(alias='integrityImpact')] = None
+    availability_impact: Annotated[Optional[CiaType], Field(alias='availabilityImpact')] = None
+    base_score: Annotated[ScoreType, Field(alias='baseScore')]
+    base_severity: Annotated[SeverityType, Field(alias='baseSeverity')]
+    exploit_code_maturity: Annotated[Optional[ExploitCodeMaturityType], Field(alias='exploitCodeMaturity')] = None
+    remediation_level: Annotated[Optional[RemediationLevelType], Field(alias='remediationLevel')] = None
+    report_confidence: Annotated[Optional[ConfidenceType], Field(alias='reportConfidence')] = None
+    temporal_score: Annotated[Optional[ScoreType], Field(alias='temporalScore')] = None
+    temporal_severity: Annotated[Optional[SeverityType], Field(alias='temporalSeverity')] = None
     confidentiality_requirement: Annotated[
-        Optional[CiaRequirementType], Field(alias='confidentiality_requirement')
+        Optional[CiaRequirementType], Field(alias='confidentialityRequirement')
     ] = None
-    integrity_requirement: Annotated[Optional[CiaRequirementType], Field(alias='integrity_requirement')] = None
-    availability_requirement: Annotated[Optional[CiaRequirementType], Field(alias='availability_requirement')] = None
-    modified_attack_vector: Annotated[Optional[ModifiedAttackVectorType], Field(alias='modified_attack_vector')] = None
+    integrity_requirement: Annotated[Optional[CiaRequirementType], Field(alias='integrityRequirement')] = None
+    availability_requirement: Annotated[Optional[CiaRequirementType], Field(alias='availabilityRequirement')] = None
+    modified_attack_vector: Annotated[Optional[ModifiedAttackVectorType], Field(alias='modifiedAttackVector')] = None
     modified_attack_complexity: Annotated[
-        Optional[ModifiedAttackComplexityType], Field(alias='modified_attack_complexity')
+        Optional[ModifiedAttackComplexityType], Field(alias='modifiedAttackComplexity')
     ] = None
     modified_privileges_required: Annotated[
         Optional[ModifiedPrivilegesRequiredType],
-        Field(alias='modified_privileges_required'),
+        Field(alias='modifiedPrivilegesRequired'),
     ] = None
     modified_user_interaction: Annotated[
-        Optional[ModifiedUserInteractionType], Field(alias='modified_user_interaction')
+        Optional[ModifiedUserInteractionType], Field(alias='modifiedUserInteraction')
     ] = None
-    modified_scope: Annotated[Optional[ModifiedScopeType], Field(alias='modified_scope')] = None
+    modified_scope: Annotated[Optional[ModifiedScopeType], Field(alias='modifiedScope')] = None
     modified_confidentiality_impact: Annotated[
-        Optional[ModifiedCiaType], Field(alias='modified_confidentiality_impact')
+        Optional[ModifiedCiaType], Field(alias='modifiedConfidentialityImpact')
     ] = None
-    modified_integrity_impact: Annotated[Optional[ModifiedCiaType], Field(alias='modified_integrity_impact')] = None
-    modified_availability_impact: Annotated[
-        Optional[ModifiedCiaType], Field(alias='modified_availability_impact')
-    ] = None
-    environmental_score: Annotated[Optional[ScoreType], Field(alias='environmental_score')] = None
-    environmental_severity: Annotated[Optional[SeverityType], Field(alias='environmental_severity')] = None
+    modified_integrity_impact: Annotated[Optional[ModifiedCiaType], Field(alias='modifiedIntegrityImpact')] = None
+    modified_availability_impact: Annotated[Optional[ModifiedCiaType], Field(alias='modifiedAvailabilityImpact')] = None
+    environmental_score: Annotated[Optional[ScoreType], Field(alias='environmentalScore')] = None
+    environmental_severity: Annotated[Optional[SeverityType], Field(alias='environmentalSeverity')] = None
+
+    @no_type_check
+    def json(self, *args, **kwargs):
+        kwargs.setdefault('by_alias', True)
+        return super().json(*args, **kwargs)
 
 
 class CVSS31(BaseModel):
     version: Annotated[Version, Field(description='CVSS Version')] = Version.three_wun
     vector_string: Annotated[
         str,
         Field(
-            alias='vector_string',
+            alias='vectorString',
             regex=(
                 '^CVSS:3[.]1/((AV:[NALP]|AC:[LH]|PR:[NLH]|UI:[NR]|S:[UC]|[CIA]:[NLH]|E:[XUPFH]|RL:[XOTWU]|RC:'
                 '[XURC]|[CIA]R:[XLMH]|MAV:[XNALP]|MAC:[XLH]|MPR:[XNLH]|MUI:[XNR]|MS:[XUC]|M[CIA]:[XNLH])/)*'
                 '(AV:[NALP]|AC:[LH]|PR:[NLH]|UI:[NR]|S:[UC]|[CIA]:[NLH]|E:[XUPFH]|RL:[XOTWU]|RC:[XURC]|[CIA]R:'
                 '[XLMH]|MAV:[XNALP]|MAC:[XLH]|MPR:[XNLH]|MUI:[XNR]|MS:[XUC]|M[CIA]:[XNLH])$'
             ),
         ),
     ]
-    attack_vector: Annotated[Optional[AttackVectorType], Field(alias='attack_vector')] = None
-    attack_complexity: Annotated[Optional[AttackComplexityType], Field(alias='attack_complexity')] = None
-    privileges_required: Annotated[Optional[PrivilegesRequiredType], Field(alias='privileges_required')] = None
-    user_interaction: Annotated[Optional[UserInteractionType], Field(alias='user_interaction')] = None
+    attack_vector: Annotated[Optional[AttackVectorType], Field(alias='attackVector')] = None
+    attack_complexity: Annotated[Optional[AttackComplexityType], Field(alias='attackComplexity')] = None
+    privileges_required: Annotated[Optional[PrivilegesRequiredType], Field(alias='privilegesRequired')] = None
+    user_interaction: Annotated[Optional[UserInteractionType], Field(alias='userInteraction')] = None
     scope: Optional[ScopeType] = None
-    confidentiality_impact: Annotated[Optional[CiaType], Field(alias='confidentiality_impact')] = None
-    integrity_impact: Annotated[Optional[CiaType], Field(alias='integrity_impact')] = None
-    availability_impact: Annotated[Optional[CiaType], Field(alias='availability_impact')] = None
-    base_score: Annotated[ScoreType, Field(alias='base_score')]
-    base_severity: Annotated[SeverityType, Field(alias='base_severity')]
-    exploit_code_maturity: Annotated[Optional[ExploitCodeMaturityType], Field(alias='exploit_code_maturity')] = None
-    remediation_level: Annotated[Optional[RemediationLevelType], Field(alias='remediation_level')] = None
-    report_confidence: Annotated[Optional[ConfidenceType], Field(alias='report_confidence')] = None
-    temporal_score: Annotated[Optional[ScoreType], Field(alias='temporal_score')] = None
-    temporal_severity: Annotated[Optional[SeverityType], Field(alias='temporal_severity')] = None
+    confidentiality_impact: Annotated[Optional[CiaType], Field(alias='confidentialityImpact')] = None
+    integrity_impact: Annotated[Optional[CiaType], Field(alias='integrityImpact')] = None
+    availability_impact: Annotated[Optional[CiaType], Field(alias='availabilityImpact')] = None
+    base_score: Annotated[ScoreType, Field(alias='baseScore')]
+    base_severity: Annotated[SeverityType, Field(alias='baseSeverity')]
+    exploit_code_maturity: Annotated[Optional[ExploitCodeMaturityType], Field(alias='exploitCodeMaturity')] = None
+    remediation_level: Annotated[Optional[RemediationLevelType], Field(alias='remediationLevel')] = None
+    report_confidence: Annotated[Optional[ConfidenceType], Field(alias='reportConfidence')] = None
+    temporal_score: Annotated[Optional[ScoreType], Field(alias='temporalScore')] = None
+    temporal_severity: Annotated[Optional[SeverityType], Field(alias='temporalSeverity')] = None
     confidentiality_requirement: Annotated[
-        Optional[CiaRequirementType], Field(alias='confidentiality_requirement')
+        Optional[CiaRequirementType], Field(alias='confidentialityRequirement')
     ] = None
-    integrity_requirement: Annotated[Optional[CiaRequirementType], Field(alias='integrity_requirement')] = None
-    availability_requirement: Annotated[Optional[CiaRequirementType], Field(alias='availability_requirement')] = None
-    modified_attack_vector: Annotated[Optional[ModifiedAttackVectorType], Field(alias='modified_attack_vector')] = None
+    integrity_requirement: Annotated[Optional[CiaRequirementType], Field(alias='integrityRequirement')] = None
+    availability_requirement: Annotated[Optional[CiaRequirementType], Field(alias='availabilityRequirement')] = None
+    modified_attack_vector: Annotated[Optional[ModifiedAttackVectorType], Field(alias='modifiedAttackVector')] = None
     modified_attack_complexity: Annotated[
-        Optional[ModifiedAttackComplexityType], Field(alias='modified_attack_complexity')
+        Optional[ModifiedAttackComplexityType], Field(alias='modifiedAttackComplexity')
     ] = None
     modified_privileges_required: Annotated[
         Optional[ModifiedPrivilegesRequiredType],
-        Field(alias='modified_privileges_required'),
+        Field(alias='modifiedPrivilegesRequired'),
     ] = None
     modified_user_interaction: Annotated[
-        Optional[ModifiedUserInteractionType], Field(alias='modified_user_interaction')
+        Optional[ModifiedUserInteractionType], Field(alias='modifiedUserInteraction')
     ] = None
-    modified_scope: Annotated[Optional[ModifiedScopeType], Field(alias='modified_scope')] = None
+    modified_scope: Annotated[Optional[ModifiedScopeType], Field(alias='modifiedScope')] = None
     modified_confidentiality_impact: Annotated[
-        Optional[ModifiedCiaType], Field(alias='modified_confidentiality_impact')
-    ] = None
-    modified_integrity_impact: Annotated[Optional[ModifiedCiaType], Field(alias='modified_integrity_impact')] = None
-    modified_availability_impact: Annotated[
-        Optional[ModifiedCiaType], Field(alias='modified_availability_impact')
+        Optional[ModifiedCiaType], Field(alias='modifiedConfidentialityImpact')
     ] = None
-    environmental_score: Annotated[Optional[ScoreType], Field(alias='environmental_score')] = None
-    environmental_severity: Annotated[Optional[SeverityType], Field(alias='environmental_severity')] = None
+    modified_integrity_impact: Annotated[Optional[ModifiedCiaType], Field(alias='modifiedIntegrityImpact')] = None
+    modified_availability_impact: Annotated[Optional[ModifiedCiaType], Field(alias='modifiedAvailabilityImpact')] = None
+    environmental_score: Annotated[Optional[ScoreType], Field(alias='environmentalScore')] = None
+    environmental_severity: Annotated[Optional[SeverityType], Field(alias='environmentalSeverity')] = None
+
+    @no_type_check
+    def json(self, *args, **kwargs):
+        kwargs.setdefault('by_alias', True)
+        return super().json(*args, **kwargs)
```

### Comparing `turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/cvss/definitions.py` & `turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/cvss/definitions.py`

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

### Comparing `turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/definitions.py` & `turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/definitions.py`

 * *Files identical despite different names*

### Comparing `turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/document.py` & `turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/document.py`

 * *Files identical despite different names*

### Comparing `turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/product.py` & `turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/product.py`

 * *Files identical despite different names*

### Comparing `turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/csaf/vulnerability.py` & `turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/csaf/vulnerability.py`

 * *Files 6% similar despite different names*

```diff
@@ -192,16 +192,16 @@
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
@@ -448,14 +448,19 @@
     which products the given value applies.
     """
 
     cvss_v2: Optional[CVSS2] = None
     cvss_v3: Optional[Union[CVSS30, CVSS31]] = None
     products: Products
 
+    @no_type_check
+    def json(self, *args, **kwargs):
+        kwargs.setdefault('by_alias', True)
+        return super().json(*args, **kwargs)
+
 
 class Vulnerability(BaseModel):
     """
     Is a container for the aggregation of all fields that are related to a single vulnerability in the document.
     """
 
     acknowledgments: Annotated[
@@ -564,13 +569,18 @@
             ' the vulnerability.',
             min_length=1,
             title='Title',
         ),
     ]
 
     @no_type_check
+    def json(self, *args, **kwargs):
+        kwargs.setdefault('by_alias', True)
+        return super().json(*args, **kwargs)
+
+    @no_type_check
     @validator('involvements', 'remediations', 'scores', 'threats')
     @classmethod
     def check_len(cls, v):
         if not v:
             raise ValueError('optional element present but empty')
         return v
```

### Comparing `turvallisuusneuvonta-2022.8.9/turvallisuusneuvonta/turvallisuusneuvonta.py` & `turvallisuusneuvonta-2023.6.18/turvallisuusneuvonta/turvallisuusneuvonta.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import os
 import pathlib
 import sys
 from itertools import chain
 from typing import Dict, Iterator, List, Optional, Tuple, Union, no_type_check
 
 import jmespath
-import orjson
+import msgspec
 from langcodes import tag_is_valid
 from lazr.uri import URI, InvalidURIError  # type: ignore
 
 from turvallisuusneuvonta.csaf.core.rules.mandatory.mandatory import (
     is_valid,
     is_valid_category,
     is_valid_defined_group_ids,
@@ -339,16 +339,16 @@
 
     return 0, '', argv
 
 
 def verify_json(data: str) -> Tuple[int, str, List[str], Dict[str, object]]:
     """Verify the JSON as CSAF."""
     try:
-        doc = orjson.loads(data)
-    except orjson.JSONDecodeError:
+        doc = msgspec.json.decode(data)
+    except msgspec.DecodeError:
         return 1, 'advisory is no valid JSON', [], {}
 
     error, message = level_zero(doc)
     if error:
         return error, message, [], {}
     return 0, 'OK', [], doc
 
@@ -359,15 +359,15 @@
     if error:
         print(message, file=sys.stderr)
         return error
 
     command, inp, config = strings
 
     with open(config, 'rb') as handle:
-        configuration = orjson.loads(handle.read())
+        configuration = msgspec.json.decode(handle.read())
 
     print(f'using configuration ({configuration})')
     source = sys.stdin if not inp else reader(inp)
     data = ''.join(line for line in source)
 
     guess = peek(data)
```

