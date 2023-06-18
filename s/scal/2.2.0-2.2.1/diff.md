# Comparing `tmp/scal-2.2.0.tar.gz` & `tmp/scal-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scal-2.2.0.tar", last modified: Tue Nov 29 12:36:03 2022, max compression
+gzip compressed data, was "scal-2.2.1.tar", last modified: Sun Jun 18 20:41:03 2023, max compression
```

## Comparing `scal-2.2.0.tar` & `scal-2.2.1.tar`

### file list

```diff
@@ -1,138 +1,34 @@
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-11-29 12:36:03.736000 scal-2.2.0/
--rw-r--r--   0 louis     (1000) louis     (1000)       85 2022-08-15 20:56:54.000000 scal-2.2.0/.gitlab-ci.yml
--rw-r--r--   0 louis     (1000) louis     (1000)      196 2022-11-29 07:14:05.000000 scal-2.2.0/.pre-commit-config.yaml
--rw-r--r--   0 louis     (1000) louis     (1000)       17 2020-06-21 10:57:06.000000 scal-2.2.0/AUTHORS
--rw-r--r--   0 louis     (1000) louis     (1000)     2061 2022-11-29 11:13:12.000000 scal-2.2.0/CHANGELOG.md
--rw-r--r--   0 louis     (1000) louis     (1000)    35147 2020-06-21 10:57:06.000000 scal-2.2.0/LICENSE
--rw-r--r--   0 louis     (1000) louis     (1000)     5021 2022-11-29 12:36:03.736000 scal-2.2.0/PKG-INFO
--rw-r--r--   0 louis     (1000) louis     (1000)     3740 2022-07-16 21:59:39.000000 scal-2.2.0/README.rst
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-11-29 12:36:03.583999 scal-2.2.0/bin/
--rwxr-xr-x   0 louis     (1000) louis     (1000)      129 2020-06-21 10:57:06.000000 scal-2.2.0/bin/autoautoscl
--rwxr-xr-x   0 louis     (1000) louis     (1000)      125 2020-06-21 10:57:06.000000 scal-2.2.0/bin/autoscl
--rwxr-xr-x   0 louis     (1000) louis     (1000)      196 2020-06-21 10:57:06.000000 scal-2.2.0/bin/generate_examples.sh
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-11-29 12:36:03.583999 scal-2.2.0/bin/lib/
--rw-r--r--   0 louis     (1000) louis     (1000)       79 2020-06-21 10:57:06.000000 scal-2.2.0/bin/lib/.pylintrc
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-11-29 12:36:03.583999 scal-2.2.0/bin/lib/autoautoscl/
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:57:06.000000 scal-2.2.0/bin/lib/autoautoscl/__init__.py
--rw-r--r--   0 louis     (1000) louis     (1000)     5009 2021-08-16 11:31:26.000000 scal-2.2.0/bin/lib/autoautoscl/__main__.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-11-29 12:36:03.587999 scal-2.2.0/bin/lib/autoscl/
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:57:06.000000 scal-2.2.0/bin/lib/autoscl/__init__.py
--rw-r--r--   0 louis     (1000) louis     (1000)     9487 2022-07-18 21:11:53.000000 scal-2.2.0/bin/lib/autoscl/__main__.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-11-29 12:36:03.587999 scal-2.2.0/bin/lib/autoscl/templates/
--rw-r--r--   0 louis     (1000) louis     (1000)      348 2022-07-18 20:56:19.000000 scal-2.2.0/bin/lib/autoscl/templates/scl.template
--rwxr-xr-x   0 louis     (1000) louis     (1000)      144 2020-06-21 10:57:06.000000 scal-2.2.0/bin/scal
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-11-29 12:36:03.595999 scal-2.2.0/doc/
--rw-r--r--   0 louis     (1000) louis     (1000)        8 2020-06-21 10:57:06.000000 scal-2.2.0/doc/.gitignore
--rw-r--r--   0 louis     (1000) louis     (1000)     6754 2020-06-21 10:57:06.000000 scal-2.2.0/doc/Makefile
--rw-r--r--   0 louis     (1000) louis     (1000)     8622 2022-11-29 09:47:31.000000 scal-2.2.0/doc/conf.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-11-29 12:36:03.679999 scal-2.2.0/doc/examples/
--rw-r--r--   0 louis     (1000) louis     (1000)        7 2022-08-15 20:56:54.000000 scal-2.2.0/doc/examples/.gitignore
--rw-r--r--   0 louis     (1000) louis     (1000)      341 2022-08-17 08:20:26.000000 scal-2.2.0/doc/examples/Makefile
--rw-r--r--   0 louis     (1000) louis     (1000)    24066 2022-08-17 08:33:59.000000 scal-2.2.0/doc/examples/fr_20142015_A.pdf
--rw-r--r--   0 louis     (1000) louis     (1000)      543 2022-08-17 08:21:34.000000 scal-2.2.0/doc/examples/fr_20142015_A.scl
--rw-r--r--   0 louis     (1000) louis     (1000)    24066 2022-08-17 08:33:59.000000 scal-2.2.0/doc/examples/fr_20142015_B.pdf
--rw-r--r--   0 louis     (1000) louis     (1000)      543 2022-07-18 21:03:36.000000 scal-2.2.0/doc/examples/fr_20142015_B.scl
--rw-r--r--   0 louis     (1000) louis     (1000)    24062 2022-08-17 08:33:59.000000 scal-2.2.0/doc/examples/fr_20142015_C.pdf
--rw-r--r--   0 louis     (1000) louis     (1000)      543 2022-07-18 21:03:59.000000 scal-2.2.0/doc/examples/fr_20142015_C.scl
--rw-r--r--   0 louis     (1000) louis     (1000)    39460 2022-08-17 08:33:59.000000 scal-2.2.0/doc/examples/fr_20152016_A.pdf
--rw-r--r--   0 louis     (1000) louis     (1000)      561 2022-07-18 21:04:21.000000 scal-2.2.0/doc/examples/fr_20152016_A.scl
--rw-r--r--   0 louis     (1000) louis     (1000)    39451 2022-08-17 08:33:59.000000 scal-2.2.0/doc/examples/fr_20152016_B.pdf
--rw-r--r--   0 louis     (1000) louis     (1000)      561 2022-07-18 21:07:47.000000 scal-2.2.0/doc/examples/fr_20152016_B.scl
--rw-r--r--   0 louis     (1000) louis     (1000)    39463 2022-08-17 08:33:59.000000 scal-2.2.0/doc/examples/fr_20152016_C.pdf
--rw-r--r--   0 louis     (1000) louis     (1000)      561 2022-07-18 21:07:52.000000 scal-2.2.0/doc/examples/fr_20152016_C.scl
--rw-r--r--   0 louis     (1000) louis     (1000)    39270 2022-08-17 08:33:59.000000 scal-2.2.0/doc/examples/fr_20162017_A.pdf
--rw-r--r--   0 louis     (1000) louis     (1000)      561 2022-07-18 21:07:54.000000 scal-2.2.0/doc/examples/fr_20162017_A.scl
--rw-r--r--   0 louis     (1000) louis     (1000)    39261 2022-08-17 08:33:59.000000 scal-2.2.0/doc/examples/fr_20162017_B.pdf
--rw-r--r--   0 louis     (1000) louis     (1000)      561 2022-07-18 21:07:55.000000 scal-2.2.0/doc/examples/fr_20162017_B.scl
--rw-r--r--   0 louis     (1000) louis     (1000)    39274 2022-08-17 08:33:59.000000 scal-2.2.0/doc/examples/fr_20162017_C.pdf
--rw-r--r--   0 louis     (1000) louis     (1000)      561 2022-07-18 21:07:58.000000 scal-2.2.0/doc/examples/fr_20162017_C.scl
--rw-r--r--   0 louis     (1000) louis     (1000)    39219 2022-08-17 08:33:59.000000 scal-2.2.0/doc/examples/fr_20172018_A.pdf
--rw-r--r--   0 louis     (1000) louis     (1000)      550 2022-07-18 21:08:13.000000 scal-2.2.0/doc/examples/fr_20172018_A.scl
--rw-r--r--   0 louis     (1000) louis     (1000)    39238 2022-08-17 08:33:59.000000 scal-2.2.0/doc/examples/fr_20172018_B.pdf
--rw-r--r--   0 louis     (1000) louis     (1000)      550 2022-07-18 21:08:41.000000 scal-2.2.0/doc/examples/fr_20172018_B.scl
--rw-r--r--   0 louis     (1000) louis     (1000)    39230 2022-08-17 08:33:59.000000 scal-2.2.0/doc/examples/fr_20172018_C.pdf
--rw-r--r--   0 louis     (1000) louis     (1000)      550 2022-07-18 21:08:33.000000 scal-2.2.0/doc/examples/fr_20172018_C.scl
--rw-r--r--   0 louis     (1000) louis     (1000)    39141 2022-08-17 08:33:59.000000 scal-2.2.0/doc/examples/fr_20182019_A.pdf
--rw-r--r--   0 louis     (1000) louis     (1000)      622 2022-07-18 21:02:09.000000 scal-2.2.0/doc/examples/fr_20182019_A.scl
--rw-r--r--   0 louis     (1000) louis     (1000)    39140 2022-08-17 08:33:59.000000 scal-2.2.0/doc/examples/fr_20182019_B.pdf
--rw-r--r--   0 louis     (1000) louis     (1000)      622 2022-07-18 21:02:15.000000 scal-2.2.0/doc/examples/fr_20182019_B.scl
--rw-r--r--   0 louis     (1000) louis     (1000)    39171 2022-08-17 08:33:59.000000 scal-2.2.0/doc/examples/fr_20182019_C.pdf
--rw-r--r--   0 louis     (1000) louis     (1000)      622 2022-07-18 21:02:21.000000 scal-2.2.0/doc/examples/fr_20182019_C.scl
--rw-r--r--   0 louis     (1000) louis     (1000)    39158 2022-08-17 08:33:59.000000 scal-2.2.0/doc/examples/fr_20192020_A.pdf
--rw-r--r--   0 louis     (1000) louis     (1000)      622 2022-07-18 21:02:27.000000 scal-2.2.0/doc/examples/fr_20192020_A.scl
--rw-r--r--   0 louis     (1000) louis     (1000)    39129 2022-08-17 08:33:59.000000 scal-2.2.0/doc/examples/fr_20192020_B.pdf
--rw-r--r--   0 louis     (1000) louis     (1000)      622 2022-07-18 21:02:33.000000 scal-2.2.0/doc/examples/fr_20192020_B.scl
--rw-r--r--   0 louis     (1000) louis     (1000)    39125 2022-08-17 08:33:59.000000 scal-2.2.0/doc/examples/fr_20192020_C.pdf
--rw-r--r--   0 louis     (1000) louis     (1000)      622 2022-07-18 21:02:39.000000 scal-2.2.0/doc/examples/fr_20192020_C.scl
--rw-r--r--   0 louis     (1000) louis     (1000)    38947 2022-08-17 08:33:59.000000 scal-2.2.0/doc/examples/fr_20202021_A.pdf
--rw-r--r--   0 louis     (1000) louis     (1000)      622 2022-07-18 21:02:44.000000 scal-2.2.0/doc/examples/fr_20202021_A.scl
--rw-r--r--   0 louis     (1000) louis     (1000)    38946 2022-08-17 08:33:59.000000 scal-2.2.0/doc/examples/fr_20202021_B.pdf
--rw-r--r--   0 louis     (1000) louis     (1000)      622 2022-07-18 21:02:50.000000 scal-2.2.0/doc/examples/fr_20202021_B.scl
--rw-r--r--   0 louis     (1000) louis     (1000)    38935 2022-08-17 08:33:59.000000 scal-2.2.0/doc/examples/fr_20202021_C.pdf
--rw-r--r--   0 louis     (1000) louis     (1000)      622 2022-07-18 21:02:56.000000 scal-2.2.0/doc/examples/fr_20202021_C.scl
--rw-r--r--   0 louis     (1000) louis     (1000)    38914 2022-08-17 08:33:59.000000 scal-2.2.0/doc/examples/fr_20212022_A.pdf
--rw-r--r--   0 louis     (1000) louis     (1000)      611 2022-08-17 08:22:43.000000 scal-2.2.0/doc/examples/fr_20212022_A.scl
--rw-r--r--   0 louis     (1000) louis     (1000)    38929 2022-08-17 08:33:59.000000 scal-2.2.0/doc/examples/fr_20212022_B.pdf
--rw-r--r--   0 louis     (1000) louis     (1000)      611 2022-07-18 21:03:08.000000 scal-2.2.0/doc/examples/fr_20212022_B.scl
--rw-r--r--   0 louis     (1000) louis     (1000)    38923 2022-08-17 08:33:59.000000 scal-2.2.0/doc/examples/fr_20212022_C.pdf
--rw-r--r--   0 louis     (1000) louis     (1000)      611 2022-07-18 21:03:13.000000 scal-2.2.0/doc/examples/fr_20212022_C.scl
--rw-r--r--   0 louis     (1000) louis     (1000)     4195 2022-08-18 10:15:44.000000 scal-2.2.0/doc/index.rst
--rw-r--r--   0 louis     (1000) louis     (1000)       70 2022-08-18 09:40:04.000000 scal-2.2.0/doc/requirements.txt
--rw-r--r--   0 louis     (1000) louis     (1000)      257 2022-11-29 09:47:31.000000 scal-2.2.0/pyproject.toml
--rw-r--r--   0 louis     (1000) louis     (1000)       26 2022-08-18 10:22:12.000000 scal-2.2.0/requirements.txt
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-11-29 12:36:03.679999 scal-2.2.0/scal/
--rw-r--r--   0 louis     (1000) louis     (1000)      894 2022-11-29 11:11:40.000000 scal-2.2.0/scal/__init__.py
--rwxr-xr-x   0 louis     (1000) louis     (1000)     4150 2022-08-17 08:03:07.000000 scal-2.2.0/scal/__main__.py
--rw-r--r--   0 louis     (1000) louis     (1000)    11731 2022-08-17 08:03:07.000000 scal-2.2.0/scal/calendar.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-11-29 12:36:03.683999 scal-2.2.0/scal/data/
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:57:07.000000 scal-2.2.0/scal/data/__init__.py
--rw-r--r--   0 louis     (1000) louis     (1000)     1009 2021-08-16 08:51:59.000000 scal-2.2.0/scal/errors.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-11-29 12:36:03.683999 scal-2.2.0/scal/template/
--rw-r--r--   0 louis     (1000) louis     (1000)     2166 2022-08-17 08:03:07.000000 scal-2.2.0/scal/template/__init__.py
--rw-r--r--   0 louis     (1000) louis     (1000)     1290 2022-08-17 08:03:07.000000 scal-2.2.0/scal/template/commands.py
--rw-r--r--   0 louis     (1000) louis     (1000)     1783 2022-08-18 10:26:05.000000 scal-2.2.0/scal/utils.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-11-29 12:36:03.683999 scal-2.2.0/scal.egg-info/
--rw-r--r--   0 louis     (1000) louis     (1000)     5021 2022-11-29 12:36:03.000000 scal-2.2.0/scal.egg-info/PKG-INFO
--rw-r--r--   0 louis     (1000) louis     (1000)     3314 2022-11-29 12:36:03.000000 scal-2.2.0/scal.egg-info/SOURCES.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        1 2022-11-29 12:36:03.000000 scal-2.2.0/scal.egg-info/dependency_links.txt
--rw-r--r--   0 louis     (1000) louis     (1000)       44 2022-11-29 12:36:03.000000 scal-2.2.0/scal.egg-info/entry_points.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        1 2020-12-18 16:34:16.000000 scal-2.2.0/scal.egg-info/not-zip-safe
--rw-r--r--   0 louis     (1000) louis     (1000)       26 2022-11-29 12:36:03.000000 scal-2.2.0/scal.egg-info/requires.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        5 2022-11-29 12:36:03.000000 scal-2.2.0/scal.egg-info/top_level.txt
--rw-r--r--   0 louis     (1000) louis     (1000)     1425 2022-11-29 12:36:03.744000 scal-2.2.0/setup.cfg
--rwxr-xr-x   0 louis     (1000) louis     (1000)       93 2020-12-18 16:33:43.000000 scal-2.2.0/setup.py
--rw-r--r--   0 louis     (1000) louis     (1000)      177 2020-06-21 10:57:07.000000 scal-2.2.0/stdeb.cfg
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-11-29 12:36:03.691999 scal-2.2.0/test/
--rw-r--r--   0 louis     (1000) louis     (1000)     1044 2021-08-16 08:51:59.000000 scal-2.2.0/test/__init__.py
--rw-r--r--   0 louis     (1000) louis     (1000)     1460 2022-02-15 08:55:26.000000 scal-2.2.0/test/doctest_all.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-11-29 12:36:03.736000 scal-2.2.0/test/test_full/
--rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:57:08.000000 scal-2.2.0/test/test_full/.gitignore
--rw-r--r--   0 louis     (1000) louis     (1000)      714 2020-06-21 10:57:08.000000 scal-2.2.0/test/test_full/__init__.py
--rw-r--r--   0 louis     (1000) louis     (1000)       68 2022-07-18 20:49:56.000000 scal-2.2.0/test/test_full/comment.scl
--rw-r--r--   0 louis     (1000) louis     (1000)     3974 2022-08-17 08:03:07.000000 scal-2.2.0/test/test_full/comment.tex
--rw-r--r--   0 louis     (1000) louis     (1000)       48 2022-07-18 20:24:57.000000 scal-2.2.0/test/test_full/empty.scl
--rw-r--r--   0 louis     (1000) louis     (1000)     3974 2022-08-17 08:03:07.000000 scal-2.2.0/test/test_full/empty.tex
--rw-r--r--   0 louis     (1000) louis     (1000)      566 2022-07-18 20:27:07.000000 scal-2.2.0/test/test_full/fr_20142015_A.scl
--rw-r--r--   0 louis     (1000) louis     (1000)     7149 2022-08-17 08:03:07.000000 scal-2.2.0/test/test_full/fr_20142015_A.tex
--rw-r--r--   0 louis     (1000) louis     (1000)       68 2022-07-18 20:35:08.000000 scal-2.2.0/test/test_full/holiday_ignore.scl
--rw-r--r--   0 louis     (1000) louis     (1000)     3974 2022-08-17 08:03:07.000000 scal-2.2.0/test/test_full/holiday_ignore.tex
--rw-r--r--   0 louis     (1000) louis     (1000)       86 2022-07-18 20:35:02.000000 scal-2.2.0/test/test_full/holiday_noyear_name.scl
--rw-r--r--   0 louis     (1000) louis     (1000)     4127 2022-08-17 08:03:07.000000 scal-2.2.0/test/test_full/holiday_noyear_name.tex
--rw-r--r--   0 louis     (1000) louis     (1000)       68 2022-07-18 20:26:22.000000 scal-2.2.0/test/test_full/holiday_noyear_noname.scl
--rw-r--r--   0 louis     (1000) louis     (1000)     4078 2022-08-17 08:03:07.000000 scal-2.2.0/test/test_full/holiday_noyear_noname.tex
--rw-r--r--   0 louis     (1000) louis     (1000)       97 2022-07-18 21:53:18.000000 scal-2.2.0/test/test_full/holiday_year_name.scl
--rw-r--r--   0 louis     (1000) louis     (1000)     4127 2022-08-17 08:03:07.000000 scal-2.2.0/test/test_full/holiday_year_name.tex
--rw-r--r--   0 louis     (1000) louis     (1000)       76 2022-07-18 20:34:14.000000 scal-2.2.0/test/test_full/holiday_year_noname.scl
--rw-r--r--   0 louis     (1000) louis     (1000)     4078 2022-08-17 08:03:07.000000 scal-2.2.0/test/test_full/holiday_year_noname.tex
--rw-r--r--   0 louis     (1000) louis     (1000)       80 2022-07-18 20:34:35.000000 scal-2.2.0/test/test_full/option_language.scl
--rw-r--r--   0 louis     (1000) louis     (1000)     3974 2022-08-17 08:03:07.000000 scal-2.2.0/test/test_full/option_language.tex
--rw-r--r--   0 louis     (1000) louis     (1000)       81 2022-07-18 20:34:44.000000 scal-2.2.0/test/test_full/option_papersize.scl
--rw-r--r--   0 louis     (1000) louis     (1000)     3974 2022-08-17 08:03:07.000000 scal-2.2.0/test/test_full/option_papersize.tex
--rw-r--r--   0 louis     (1000) louis     (1000)     2065 2022-07-18 21:12:52.000000 scal-2.2.0/test/test_full/test_render.py
--rw-r--r--   0 louis     (1000) louis     (1000)       48 2022-07-18 20:34:47.000000 scal-2.2.0/test/test_full/year_1.scl
--rw-r--r--   0 louis     (1000) louis     (1000)     3974 2022-08-17 08:03:07.000000 scal-2.2.0/test/test_full/year_1.tex
--rw-r--r--   0 louis     (1000) louis     (1000)       48 2022-07-18 20:34:49.000000 scal-2.2.0/test/test_full/year_2.scl
--rw-r--r--   0 louis     (1000) louis     (1000)     5514 2022-08-17 08:03:07.000000 scal-2.2.0/test/test_full/year_2.tex
--rw-r--r--   0 louis     (1000) louis     (1000)       48 2022-07-18 20:24:59.000000 scal-2.2.0/test/test_full/year_5.scl
--rw-r--r--   0 louis     (1000) louis     (1000)    10263 2022-08-17 08:03:07.000000 scal-2.2.0/test/test_full/year_5.tex
--rw-r--r--   0 louis     (1000) louis     (1000)      807 2022-11-29 09:47:31.000000 scal-2.2.0/tox.ini
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-06-18 20:41:03.690384 scal-2.2.1/
+-rw-r--r--   0 louis     (1000) louis     (1000)       17 2020-06-21 10:57:06.000000 scal-2.2.1/AUTHORS
+-rw-r--r--   0 louis     (1000) louis     (1000)    35147 2020-06-21 10:57:06.000000 scal-2.2.1/LICENSE
+-rw-r--r--   0 louis     (1000) louis     (1000)       29 2023-01-02 20:22:48.000000 scal-2.2.1/MANIFEST.in
+-rw-r--r--   0 louis     (1000) louis     (1000)     8454 2023-06-18 20:41:03.694384 scal-2.2.1/PKG-INFO
+-rw-r--r--   0 louis     (1000) louis     (1000)     7173 2023-06-18 20:38:03.000000 scal-2.2.1/README.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)      257 2023-01-02 20:15:57.000000 scal-2.2.1/pyproject.toml
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-06-18 20:41:03.690384 scal-2.2.1/scal/
+-rw-r--r--   0 louis     (1000) louis     (1000)      894 2023-06-18 20:38:06.000000 scal-2.2.1/scal/__init__.py
+-rwxr-xr-x   0 louis     (1000) louis     (1000)     4202 2023-01-02 20:31:07.000000 scal-2.2.1/scal/__main__.py
+-rw-r--r--   0 louis     (1000) louis     (1000)    11729 2023-05-03 16:35:03.000000 scal-2.2.1/scal/calendar.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-06-18 20:41:03.690384 scal-2.2.1/scal/data/
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:57:07.000000 scal-2.2.1/scal/data/__init__.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-06-18 20:41:03.690384 scal-2.2.1/scal/data/config/
+-rw-r--r--   0 louis     (1000) louis     (1000)      896 2022-12-31 21:35:27.000000 scal-2.2.1/scal/data/config/calendar.tex
+-rw-r--r--   0 louis     (1000) louis     (1000)      724 2022-08-17 08:03:07.000000 scal-2.2.1/scal/data/config/weekly.tex
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-06-18 20:41:03.690384 scal-2.2.1/scal/data/templates/
+-rw-r--r--   0 louis     (1000) louis     (1000)     4712 2023-06-18 11:11:36.000000 scal-2.2.1/scal/data/templates/calendar.tex
+-rw-r--r--   0 louis     (1000) louis     (1000)    10059 2023-06-18 11:12:50.000000 scal-2.2.1/scal/data/templates/weekly.tex
+-rw-r--r--   0 louis     (1000) louis     (1000)     1009 2021-08-16 08:51:59.000000 scal-2.2.1/scal/errors.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-06-18 20:41:03.690384 scal-2.2.1/scal/template/
+-rw-r--r--   0 louis     (1000) louis     (1000)     2166 2022-08-17 08:03:07.000000 scal-2.2.1/scal/template/__init__.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     1290 2022-08-17 08:03:07.000000 scal-2.2.1/scal/template/commands.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     1783 2022-08-18 10:26:05.000000 scal-2.2.1/scal/utils.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-06-18 20:41:03.690384 scal-2.2.1/scal.egg-info/
+-rw-r--r--   0 louis     (1000) louis     (1000)     8454 2023-06-18 20:41:03.000000 scal-2.2.1/scal.egg-info/PKG-INFO
+-rw-r--r--   0 louis     (1000) louis     (1000)      545 2023-06-18 20:41:03.000000 scal-2.2.1/scal.egg-info/SOURCES.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)        1 2023-06-18 20:41:03.000000 scal-2.2.1/scal.egg-info/dependency_links.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)       44 2023-06-18 20:41:03.000000 scal-2.2.1/scal.egg-info/entry_points.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)        1 2023-01-02 20:29:29.000000 scal-2.2.1/scal.egg-info/not-zip-safe
+-rw-r--r--   0 louis     (1000) louis     (1000)       26 2023-06-18 20:41:03.000000 scal-2.2.1/scal.egg-info/requires.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)        5 2023-06-18 20:41:03.000000 scal-2.2.1/scal.egg-info/top_level.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)     1425 2023-06-18 20:41:03.694384 scal-2.2.1/setup.cfg
+-rwxr-xr-x   0 louis     (1000) louis     (1000)       93 2020-12-18 16:33:43.000000 scal-2.2.1/setup.py
```

### Comparing `scal-2.2.0/LICENSE` & `scal-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scal-2.2.0/scal/__init__.py` & `scal-2.2.1/scal/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright Louis Paternault 2013-2022
+# Copyright Louis Paternault 2013-2023
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -13,11 +13,11 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>. 1
 
 """Calendar producer"""
 
-VERSION = "2.2.0"
+VERSION = "2.2.1"
 __AUTHOR__ = "Louis Paternault (spalax@gresille.org)"
-__DATE__ = "2011-2022"
+__DATE__ = "2011-2023"
 __COPYRIGHT__ = f"(C) {__DATE__} Louis Paternault. GNU GPL 3 or later."
```

### Comparing `scal-2.2.0/scal/__main__.py` & `scal-2.2.1/scal/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,22 +132,25 @@
 
     for command, function in sorted(SUBCOMMANDS.items()):
         subparser.add_function(function, command=command)
 
     return parser
 
 
-def main(args):
+def main(args=None):
     """Main function."""
     parser = argument_parser()
 
+    if args is None:
+        args = sys.argv[1:]
+
     if not args:
-        return parser.parse_args(args)
-    if args[0] in ("-h", "--help"):
+        return parser.parse_args()
+    if args[0] in ("-h", "--help", "--version"):
         return parser.parse_args(args)
     if args[0] in SUBCOMMANDS:
         return parser.parse_args(args)
     return parser.parse_args([DEFAULT_SUBCOMMAND] + args)
 
 
 if __name__ == "__main__":
-    main(sys.argv[1:])
+    main()
```

### Comparing `scal-2.2.0/scal/calendar.py` & `scal-2.2.1/scal/calendar.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,15 +317,15 @@
                 maybe_workweek = None
             yield wednesday, maybe_workweek, weeknumber(wednesday)
             wednesday += datetime.timedelta(days=7)
 
     def _weeks(self, work, iso):
         """Return the list of weeks, processed by template."""
         weeks = []
-        for (day, work_number, iso_number) in self.week_iterator():
+        for day, work_number, iso_number in self.week_iterator():
             week = {"date": day, "work": None, "iso": None}
             if work:
                 week["work"] = work_number
             if iso:
                 week["iso"] = iso_number
             weeks.append(week)
         return weeks
```

### Comparing `scal-2.2.0/scal/errors.py` & `scal-2.2.1/scal/errors.py`

 * *Files identical despite different names*

### Comparing `scal-2.2.0/scal/template/__init__.py` & `scal-2.2.1/scal/template/__init__.py`

 * *Files identical despite different names*

### Comparing `scal-2.2.0/scal/template/commands.py` & `scal-2.2.1/scal/template/commands.py`

 * *Files identical despite different names*

### Comparing `scal-2.2.0/scal/utils.py` & `scal-2.2.1/scal/utils.py`

 * *Files identical despite different names*

### Comparing `scal-2.2.0/setup.cfg` & `scal-2.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = scal
-version = 2.2.0
+version = 2.2.1
 author = Louis Paternault
 author_email = spalax@gresille.org
 license = GPLv3 or any later version
 description = LaTeX generation of school year calendars
 keywords = calendar latex school tikz
 url = http://framagit.org/spalax/scal
 project_urls =
```

### Comparing `scal-2.2.0/test/test_full/comment.tex` & `scal-2.2.1/scal/data/templates/calendar.tex`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
 % Copyright 2012 Robert Krause
-% Copyright @COPYRIGHTDATE@ Louis Paternault
+% Copyright ((copyrightdate)) Louis Paternault
 % License : Creative Commons Attribution License
 %
-% Produced by `scal` version @VERSION@.
+% Produced by ((version)).
 % http://git.framasoft.org/spalax/scal
 %
 % Compile it using `lualatex`
 %
 % History:
 % This file has been posted by original author Robert Krause on TeXample.net [1] on 13 July 2012.
 % I (Louis Paternault) used it as a base for this template.
@@ -20,44 +20,46 @@
 %$ lualatex $basename
 
 \documentclass[10pt]{article}
 
 \IfFileExists{hyperref.sty}{
   \usepackage[
     pdftitle={Calendar for years
-        2014
+      (*for year in years|sort*)
+        ((year))
+      (*endfor*)
     },
-    pdfcreator={LuaLaTeX, using a file generated by `scal` version @VERSION@},
+    pdfcreator={LuaLaTeX, using a file generated by ((version))},
   ]{hyperref}
 }{
   % Hyperref not loaded
 }
 
 \usepackage{fontspec}
 \renewcommand{\familydefault}{\sfdefault}
 
-\usepackage[english]{babel}
-\usepackage[english]{translator} % Internationalized  Month and Day names
+\usepackage[(( variables.language ))]{babel}
+\usepackage[(( variables.language ))]{translator} % Internationalized  Month and Day names
 
 \usepackage{tikz}
 \usetikzlibrary{calc}
 \usetikzlibrary{calendar}
 
-\usepackage[a4paper, landscape, margin=.5cm]{geometry}
+\usepackage[(( variables.papersize )), landscape, margin=.5cm]{geometry}
 
-\newcommand{\cellwidth}{\textwidth/1}
+\newcommand{\cellwidth}{\textwidth/(( count.months ))}
 \newcommand{\cellheight}{\textheight/34}
 \newcommand{\cellsep}{2pt}
 
 % Names of Holidays are inserted by employing this macro. Arguments:
 % - #1: First day of holidays
 % - #2: Holiday name
 \def\printholiday#1#2{
-    \node [anchor=north west, align=right, text width={\cellwidth-\cellsep-7pt}] at
-    ($(cal-#1.north west)$) {\tiny{#2\par}};
+    \node [anchor=west, align=right, text width={\cellwidth-\cellsep-7pt}] at
+    ($(cal-#1.west)$) {\tiny{#2\par}};
 }
 
 % Display weeks
 % - #1 Day in which week is to be written
 % - #2 Week number (as LaTeX code)
 \def\printweek#1#2{
     \node [anchor=east, align=center, color=gray] at
@@ -81,15 +83,15 @@
 \begin{document}
 
 
 \begin{center}
 \begin{tikzpicture}[every day/.style={anchor = north}]
 \pgftransformyshift{\cellheight}
 \calendar[
-  dates=2014-3-01 to 2014-3-last,
+  dates=(( start.year ))-(( start.month ))-01 to (( end.year ))-(( end.month ))-last,
   name=cal,
   day yshift = \cellheight,
   day code=
   {
     \node[name=\pgfcalendarsuggestedname,every day,shape=rectangle,
     minimum height= \cellheight, draw=black, text width = {\cellwidth-\cellsep-7pt}]{};
     \draw ($(\pgfcalendarsuggestedname.west)+(0  em,0)$)           node[anchor=west, color=gray]{\tikzdaytext};
@@ -107,33 +109,47 @@
         {\textbf{\pgfcalendarmonthname{\pgfcalendarcurrentmonth}}};
     }{}
     \ifdate{workday}
     {
       % normal days are white
       \tikzset{every day/.style={fill=white}}
       % Holidays
+      (* for holiday in holidays *)
+      \ifdate{between=((holiday.start)) and ((holiday.end))}{%
+        \tikzset{every day/.style={fill=gray!30}}}{}
+      (* endfor *)
     }{}
     % Saturdays
     \ifdate{Saturday}{\tikzset{every day/.style={fill=red!10}}}{}
     % Sundays
     \ifdate{Sunday}{\tikzset{every day/.style={fill=red!20}}}{}
   },
  execute at begin day scope=
   {
     % each day is shifted down according to the day of month
     \pgftransformyshift{-{\cellheight * \number\pgfcalendarcurrentday}}
   }
 ];
 
-% Print name of Holidays
-
 % Print week numbers
-  \printweek{2014-03-05}{10}
-  \printweek{2014-03-12}{11}
-  \printweek{2014-03-19}{12}
-  \printweek{2014-03-26}{13}
+(* for week in weeks if week.work and week.iso *)
+  \printweek{((week.date))}{((week.work)) / ((week.iso))}
+(* endfor *)
+(* for week in weeks if week.iso and not week.work *)
+  \printweek{((week.date))}{((week.iso))}
+(* endfor *)
+(* for week in weeks if week.work and not week.iso*)
+  \printweek{((week.date))}{((week.work))}
+(* endfor *)
+
+% Print name of Holidays
+(* for holiday in holidays if holiday.name *)
+    \printholiday{((holiday.start))}{((holiday.name))}
+(* endfor *)
 
 % Print years
-  \printyear{2014}{03}{03}
+(* for year, boundaries in years.items() *)
+  \printyear{((year))}{((boundaries[0]))}{((boundaries[1]))}
+(* endfor *)
 \end{tikzpicture}
 \end{center}
 \end{document}
```

