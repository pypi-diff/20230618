# Comparing `tmp/terminal_typing_tutor-0.4.0.tar.gz` & `tmp/terminal_typing_tutor-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminal_typing_tutor-0.4.0.tar", max compression
+gzip compressed data, was "terminal_typing_tutor-0.4.1.tar", max compression
```

## Comparing `terminal_typing_tutor-0.4.0.tar` & `terminal_typing_tutor-0.4.1.tar`

### file list

```diff
@@ -1,124 +1,120 @@
--rw-r--r--   0        0        0    35149 2023-06-11 22:25:13.467755 terminal_typing_tutor-0.4.0/LICENSE
--rw-r--r--   0        0        0     2943 2023-06-13 00:49:15.307992 terminal_typing_tutor-0.4.0/README.md
--rw-r--r--   0        0        0      798 2023-06-18 15:49:04.952861 terminal_typing_tutor-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       69 2023-06-11 21:09:06.071850 terminal_typing_tutor-0.4.0/terminal_typing_tutor/__init__.py
--rw-r--r--   0        0        0       31 2023-06-11 04:25:58.607685 terminal_typing_tutor-0.4.0/terminal_typing_tutor/__main__.py
--rw-r--r--   0        0        0     1669 2023-06-18 15:48:46.384914 terminal_typing_tutor-0.4.0/terminal_typing_tutor/constants.py
--rwxr-xr-x   0        0        0      201 2023-06-11 04:11:52.927703 terminal_typing_tutor-0.4.0/terminal_typing_tutor/main.py
--rw-r--r--   0        0        0     3364 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/M/1/data.yaml
--rw-r--r--   0        0        0     3377 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/M/10/data.yaml
--rw-r--r--   0        0        0     4191 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/M/11/data.yaml
--rw-r--r--   0        0        0     2861 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/M/2/data.yaml
--rw-r--r--   0        0        0     3201 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/M/3/data.yaml
--rw-r--r--   0        0        0     2680 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/M/4/data.yaml
--rw-r--r--   0        0        0     3175 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/M/5/data.yaml
--rw-r--r--   0        0        0     3017 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/M/6/data.yaml
--rw-r--r--   0        0        0     2591 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/M/7/data.yaml
--rw-r--r--   0        0        0     3028 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/M/8/data.yaml
--rw-r--r--   0        0        0     3861 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/M/9/data.yaml
--rw-r--r--   0        0        0        3 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/M/lesson_count
--rw-r--r--   0        0        0    36212 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/M/m.typ
--rw-r--r--   0        0        0      520 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/M/menu.json
--rw-r--r--   0        0        0       14 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/M/title
--rw-r--r--   0        0        0     5885 2023-06-17 03:52:11.279983 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/Q/1/data.yaml
--rw-r--r--   0        0        0     2445 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/Q/2/data.yaml
--rw-r--r--   0        0        0     3099 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/Q/3/data.yaml
--rw-r--r--   0        0        0     3034 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/Q/4/data.yaml
--rw-r--r--   0        0        0     2004 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/Q/5/data.yaml
--rw-r--r--   0        0        0        2 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/Q/lesson_count
--rw-r--r--   0        0        0      293 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/Q/menu.json
--rw-r--r--   0        0        0    16803 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/Q/q.typ
--rw-r--r--   0        0        0       20 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/Q/title
--rw-r--r--   0        0        0     2650 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/1/data.yaml
--rw-r--r--   0        0        0     3389 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/10/data.yaml
--rw-r--r--   0        0        0     2608 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/11/data.yaml
--rw-r--r--   0        0        0     2975 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/12/data.yaml
--rw-r--r--   0        0        0     2659 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/13/data.yaml
--rw-r--r--   0        0        0     3307 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/14/data.yaml
--rw-r--r--   0        0        0     2721 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/2/data.yaml
--rw-r--r--   0        0        0     3181 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/3/data.yaml
--rw-r--r--   0        0        0     2764 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/4/data.yaml
--rw-r--r--   0        0        0     3166 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/5/data.yaml
--rw-r--r--   0        0        0     2920 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/6/data.yaml
--rw-r--r--   0        0        0     2852 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/7/data.yaml
--rw-r--r--   0        0        0     3119 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/8/data.yaml
--rw-r--r--   0        0        0     3491 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/9/data.yaml
--rw-r--r--   0        0        0        3 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/lesson_count
--rw-r--r--   0        0        0      672 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/menu.json
--rw-r--r--   0        0        0    41316 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/r.typ
--rw-r--r--   0        0        0       19 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/title
--rw-r--r--   0        0        0     2762 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/S/1/data.yaml
--rw-r--r--   0        0        0     3364 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/S/2/data.yaml
--rw-r--r--   0        0        0     4005 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/S/3/data.yaml
--rw-r--r--   0        0        0     6793 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/S/4/data.yaml
--rw-r--r--   0        0        0        2 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/S/lesson_count
--rw-r--r--   0        0        0      203 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/S/menu.json
--rw-r--r--   0        0        0    18263 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/S/s.typ
--rw-r--r--   0        0        0       13 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/S/title
--rw-r--r--   0        0        0     4694 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/1/data.yaml
--rw-r--r--   0        0        0     4139 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/10/data.yaml
--rw-r--r--   0        0        0     3081 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/11/data.yaml
--rw-r--r--   0        0        0     3842 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/12/data.yaml
--rw-r--r--   0        0        0      741 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/13/data.yaml
--rw-r--r--   0        0        0     1669 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/14/data.yaml
--rw-r--r--   0        0        0     3331 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/15/data.yaml
--rw-r--r--   0        0        0     3828 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/16/data.yaml
--rw-r--r--   0        0        0     2344 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/2/data.yaml
--rw-r--r--   0        0        0     3296 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/3/data.yaml
--rw-r--r--   0        0        0     2254 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/4/data.yaml
--rw-r--r--   0        0        0     2633 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/5/data.yaml
--rw-r--r--   0        0        0     2227 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/6/data.yaml
--rw-r--r--   0        0        0     3282 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/7/data.yaml
--rw-r--r--   0        0        0     3137 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/8/data.yaml
--rw-r--r--   0        0        0     2791 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/9/data.yaml
--rw-r--r--   0        0        0        3 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/lesson_count
--rw-r--r--   0        0        0      932 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/menu.json
--rw-r--r--   0        0        0    40881 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/t.typ
--rw-r--r--   0        0        0       20 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/title
--rw-r--r--   0        0        0      416 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/1/data.yaml
--rw-r--r--   0        0        0     1376 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/10/data.yaml
--rw-r--r--   0        0        0     1324 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/11/data.yaml
--rw-r--r--   0        0        0     1400 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/12/data.yaml
--rw-r--r--   0        0        0     3117 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/13/data.yaml
--rw-r--r--   0        0        0      996 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/2/data.yaml
--rw-r--r--   0        0        0     1295 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/3/data.yaml
--rw-r--r--   0        0        0      631 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/4/data.yaml
--rw-r--r--   0        0        0     1119 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/5/data.yaml
--rw-r--r--   0        0        0     1166 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/6/data.yaml
--rw-r--r--   0        0        0     1189 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/7/data.yaml
--rw-r--r--   0        0        0     1239 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/8/data.yaml
--rw-r--r--   0        0        0     1343 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/9/data.yaml
--rw-r--r--   0        0        0        3 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/lesson_count
--rw-r--r--   0        0        0     1030 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/menu.json
--rw-r--r--   0        0        0       15 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/title
--rw-r--r--   0        0        0    19159 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/u.typ
--rw-r--r--   0        0        0      581 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/1/data.yaml
--rw-r--r--   0        0        0     2382 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/10/data.yaml
--rw-r--r--   0        0        0     2467 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/11/data.yaml
--rw-r--r--   0        0        0     2535 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/12/data.yaml
--rw-r--r--   0        0        0     2915 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/13/data.yaml
--rw-r--r--   0        0        0     3006 2023-06-11 03:21:12.343766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/14/data.yaml
--rw-r--r--   0        0        0     5525 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/15/data.yaml
--rw-r--r--   0        0        0     3465 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/16/data.yaml
--rw-r--r--   0        0        0     3747 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/17/data.yaml
--rw-r--r--   0        0        0     3711 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/18/data.yaml
--rw-r--r--   0        0        0     2927 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/19/data.yaml
--rw-r--r--   0        0        0     1598 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/2/data.yaml
--rw-r--r--   0        0        0     2077 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/3/data.yaml
--rw-r--r--   0        0        0     1873 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/4/data.yaml
--rw-r--r--   0        0        0     2103 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/5/data.yaml
--rw-r--r--   0        0        0     1831 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/6/data.yaml
--rw-r--r--   0        0        0     2071 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/7/data.yaml
--rw-r--r--   0        0        0     1780 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/8/data.yaml
--rw-r--r--   0        0        0     2053 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/9/data.yaml
--rw-r--r--   0        0        0        3 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/lesson_count
--rw-r--r--   0        0        0     1295 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/menu.json
--rw-r--r--   0        0        0       16 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/title
--rw-r--r--   0        0        0    47250 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/v.typ
--rw-r--r--   0        0        0     7550 2023-06-17 05:15:48.567964 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/W/1/data.yaml
--rw-r--r--   0        0        0        2 2023-06-17 03:14:37.267992 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/W/lesson_count
--rw-r--r--   0        0        0       95 2023-06-17 04:04:04.679981 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/W/menu.json
--rw-r--r--   0        0        0       16 2023-06-17 03:13:54.415992 terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/W/title
--rw-r--r--   0        0        0    18625 2023-06-18 15:41:03.819810 terminal_typing_tutor-0.4.0/terminal_typing_tutor/tutor.py
--rw-r--r--   0        0        0       71 2023-06-18 15:43:39.575877 terminal_typing_tutor-0.4.0/terminal_typing_tutor/update.json
--rw-r--r--   0        0        0     4025 1970-01-01 00:00:00.000000 terminal_typing_tutor-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-11 22:25:13.467755 terminal_typing_tutor-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2943 2023-06-13 00:49:15.307992 terminal_typing_tutor-0.4.1/README.md
+-rw-r--r--   0        0        0      798 2023-06-18 15:54:04.572283 terminal_typing_tutor-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-06-11 21:09:06.071850 terminal_typing_tutor-0.4.1/terminal_typing_tutor/__init__.py
+-rw-r--r--   0        0        0       31 2023-06-11 04:25:58.607685 terminal_typing_tutor-0.4.1/terminal_typing_tutor/__main__.py
+-rw-r--r--   0        0        0     1569 2023-06-18 15:55:23.504370 terminal_typing_tutor-0.4.1/terminal_typing_tutor/constants.py
+-rwxr-xr-x   0        0        0      201 2023-06-18 15:55:19.336366 terminal_typing_tutor-0.4.1/terminal_typing_tutor/main.py
+-rw-r--r--   0        0        0     3364 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/M/1/data.yaml
+-rw-r--r--   0        0        0     3377 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/M/10/data.yaml
+-rw-r--r--   0        0        0     4191 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/M/11/data.yaml
+-rw-r--r--   0        0        0     2861 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/M/2/data.yaml
+-rw-r--r--   0        0        0     3201 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/M/3/data.yaml
+-rw-r--r--   0        0        0     2680 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/M/4/data.yaml
+-rw-r--r--   0        0        0     3175 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/M/5/data.yaml
+-rw-r--r--   0        0        0     3017 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/M/6/data.yaml
+-rw-r--r--   0        0        0     2591 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/M/7/data.yaml
+-rw-r--r--   0        0        0     3028 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/M/8/data.yaml
+-rw-r--r--   0        0        0     3861 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/M/9/data.yaml
+-rw-r--r--   0        0        0        3 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/M/lesson_count
+-rw-r--r--   0        0        0    36212 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/M/m.typ
+-rw-r--r--   0        0        0      520 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/M/menu.json
+-rw-r--r--   0        0        0       14 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/M/title
+-rw-r--r--   0        0        0     5885 2023-06-17 03:52:11.279983 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/Q/1/data.yaml
+-rw-r--r--   0        0        0     2445 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/Q/2/data.yaml
+-rw-r--r--   0        0        0     3099 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/Q/3/data.yaml
+-rw-r--r--   0        0        0     3034 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/Q/4/data.yaml
+-rw-r--r--   0        0        0     2004 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/Q/5/data.yaml
+-rw-r--r--   0        0        0        2 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/Q/lesson_count
+-rw-r--r--   0        0        0      293 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/Q/menu.json
+-rw-r--r--   0        0        0    16803 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/Q/q.typ
+-rw-r--r--   0        0        0       20 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/Q/title
+-rw-r--r--   0        0        0     2650 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/1/data.yaml
+-rw-r--r--   0        0        0     3389 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/10/data.yaml
+-rw-r--r--   0        0        0     2608 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/11/data.yaml
+-rw-r--r--   0        0        0     2975 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/12/data.yaml
+-rw-r--r--   0        0        0     2659 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/13/data.yaml
+-rw-r--r--   0        0        0     3307 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/14/data.yaml
+-rw-r--r--   0        0        0     2721 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/2/data.yaml
+-rw-r--r--   0        0        0     3181 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/3/data.yaml
+-rw-r--r--   0        0        0     2764 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/4/data.yaml
+-rw-r--r--   0        0        0     3166 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/5/data.yaml
+-rw-r--r--   0        0        0     2920 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/6/data.yaml
+-rw-r--r--   0        0        0     2852 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/7/data.yaml
+-rw-r--r--   0        0        0     3119 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/8/data.yaml
+-rw-r--r--   0        0        0     3491 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/9/data.yaml
+-rw-r--r--   0        0        0        3 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/lesson_count
+-rw-r--r--   0        0        0      672 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/menu.json
+-rw-r--r--   0        0        0    41316 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/r.typ
+-rw-r--r--   0        0        0       19 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/title
+-rw-r--r--   0        0        0     2762 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/S/1/data.yaml
+-rw-r--r--   0        0        0     3364 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/S/2/data.yaml
+-rw-r--r--   0        0        0     4005 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/S/3/data.yaml
+-rw-r--r--   0        0        0     6793 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/S/4/data.yaml
+-rw-r--r--   0        0        0        2 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/S/lesson_count
+-rw-r--r--   0        0        0      203 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/S/menu.json
+-rw-r--r--   0        0        0    18263 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/S/s.typ
+-rw-r--r--   0        0        0       13 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/S/title
+-rw-r--r--   0        0        0     4694 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/1/data.yaml
+-rw-r--r--   0        0        0     4139 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/10/data.yaml
+-rw-r--r--   0        0        0     3081 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/11/data.yaml
+-rw-r--r--   0        0        0     3842 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/12/data.yaml
+-rw-r--r--   0        0        0      741 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/13/data.yaml
+-rw-r--r--   0        0        0     1669 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/14/data.yaml
+-rw-r--r--   0        0        0     3331 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/15/data.yaml
+-rw-r--r--   0        0        0     3828 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/16/data.yaml
+-rw-r--r--   0        0        0     2344 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/2/data.yaml
+-rw-r--r--   0        0        0     3296 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/3/data.yaml
+-rw-r--r--   0        0        0     2254 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/4/data.yaml
+-rw-r--r--   0        0        0     2633 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/5/data.yaml
+-rw-r--r--   0        0        0     2227 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/6/data.yaml
+-rw-r--r--   0        0        0     3282 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/7/data.yaml
+-rw-r--r--   0        0        0     3137 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/8/data.yaml
+-rw-r--r--   0        0        0     2791 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/9/data.yaml
+-rw-r--r--   0        0        0        3 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/lesson_count
+-rw-r--r--   0        0        0      932 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/menu.json
+-rw-r--r--   0        0        0    40881 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/t.typ
+-rw-r--r--   0        0        0       20 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/title
+-rw-r--r--   0        0        0      416 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/1/data.yaml
+-rw-r--r--   0        0        0     1376 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/10/data.yaml
+-rw-r--r--   0        0        0     1324 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/11/data.yaml
+-rw-r--r--   0        0        0     1400 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/12/data.yaml
+-rw-r--r--   0        0        0     3117 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/13/data.yaml
+-rw-r--r--   0        0        0      996 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/2/data.yaml
+-rw-r--r--   0        0        0     1295 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/3/data.yaml
+-rw-r--r--   0        0        0      631 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/4/data.yaml
+-rw-r--r--   0        0        0     1119 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/5/data.yaml
+-rw-r--r--   0        0        0     1166 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/6/data.yaml
+-rw-r--r--   0        0        0     1189 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/7/data.yaml
+-rw-r--r--   0        0        0     1239 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/8/data.yaml
+-rw-r--r--   0        0        0     1343 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/9/data.yaml
+-rw-r--r--   0        0        0        3 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/lesson_count
+-rw-r--r--   0        0        0     1030 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/menu.json
+-rw-r--r--   0        0        0       15 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/title
+-rw-r--r--   0        0        0    19159 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/u.typ
+-rw-r--r--   0        0        0      581 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/1/data.yaml
+-rw-r--r--   0        0        0     2382 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/10/data.yaml
+-rw-r--r--   0        0        0     2467 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/11/data.yaml
+-rw-r--r--   0        0        0     2535 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/12/data.yaml
+-rw-r--r--   0        0        0     2915 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/13/data.yaml
+-rw-r--r--   0        0        0     3006 2023-06-11 03:21:12.343766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/14/data.yaml
+-rw-r--r--   0        0        0     5525 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/15/data.yaml
+-rw-r--r--   0        0        0     3465 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/16/data.yaml
+-rw-r--r--   0        0        0     3747 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/17/data.yaml
+-rw-r--r--   0        0        0     3711 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/18/data.yaml
+-rw-r--r--   0        0        0     2927 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/19/data.yaml
+-rw-r--r--   0        0        0     1598 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/2/data.yaml
+-rw-r--r--   0        0        0     2077 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/3/data.yaml
+-rw-r--r--   0        0        0     1873 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/4/data.yaml
+-rw-r--r--   0        0        0     2103 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/5/data.yaml
+-rw-r--r--   0        0        0     1831 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/6/data.yaml
+-rw-r--r--   0        0        0     2071 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/7/data.yaml
+-rw-r--r--   0        0        0     1780 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/8/data.yaml
+-rw-r--r--   0        0        0     2053 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/9/data.yaml
+-rw-r--r--   0        0        0        3 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/lesson_count
+-rw-r--r--   0        0        0     1295 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/menu.json
+-rw-r--r--   0        0        0       16 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/title
+-rw-r--r--   0        0        0    47250 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/v.typ
+-rw-r--r--   0        0        0    18625 2023-06-18 15:41:03.819810 terminal_typing_tutor-0.4.1/terminal_typing_tutor/tutor.py
+-rw-r--r--   0        0        0       80 2023-06-18 15:55:41.304390 terminal_typing_tutor-0.4.1/terminal_typing_tutor/update.json
+-rw-r--r--   0        0        0     4025 1970-01-01 00:00:00.000000 terminal_typing_tutor-0.4.1/PKG-INFO
```

### Comparing `terminal_typing_tutor-0.4.0/LICENSE` & `terminal_typing_tutor-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/README.md` & `terminal_typing_tutor-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/pyproject.toml` & `terminal_typing_tutor-0.4.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "terminal-typing-tutor"
-version = "0.4.0"
+version = "0.4.1"
 description = "Improve your touch-typing skills in the terminal, based on the GNU Typist program"
 authors = ["Justin Angeles <justinaawd@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-only"
 homepage = "https://github.com/justinsgithub/terminal-typing-tutor"
 repository = "https://github.com/justinsgithub/terminal-typing-tutor"
 documentation = "https://github.com/justinsgithub/terminal-typing-tutor"
```

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/constants.py` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from blessed import Terminal
 from typing import Literal, TypedDict
 
-CURRENT_VERSION = "0.4.0"
+CURRENT_VERSION = "0.4.1"
 
 MAIN_MENU_TITLE = "Series selection menu"
 
 MAIN_MENU = [
     {
         "title": "Series Q    Quick QWERTY course  (Q1 - Q5) ",
         "series": "Q",
@@ -29,18 +29,14 @@
     {
         "title": "Series M    Typing drills  (M1 - M11)      ",
         "series": "M",
     },
     {
         "title": "Series S    Speed drills  (S1 - S4)        ",
         "series": "S",
-    },
-    {
-        "title": "Series W    Web Development                ",
-        "series": "W",
     }
 ]
 
 TERM = Terminal()
 HOME = TERM.home
 HEIGHT = TERM.height
 WIDTH = TERM.width
```

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/M/1/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/M/1/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/M/10/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/M/10/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/M/11/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/M/11/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/M/2/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/M/2/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/M/3/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/M/3/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/M/4/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/M/4/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/M/5/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/M/5/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/M/6/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/M/6/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/M/7/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/M/7/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/M/8/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/M/8/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/M/9/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/M/9/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/M/m.typ` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/M/m.typ`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/M/menu.json` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/M/menu.json`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/Q/1/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/Q/1/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/Q/2/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/Q/2/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/Q/3/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/Q/3/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/Q/4/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/Q/4/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/Q/5/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/Q/5/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/Q/q.typ` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/Q/q.typ`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/1/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/1/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/10/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/10/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/11/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/11/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/12/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/12/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/13/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/13/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/14/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/14/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/2/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/2/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/3/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/3/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/4/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/4/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/5/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/5/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/6/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/6/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/7/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/7/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/8/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/8/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/9/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/9/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/menu.json` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/menu.json`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/R/r.typ` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/R/r.typ`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/S/1/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/S/1/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/S/2/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/S/2/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/S/3/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/S/3/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/S/4/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/S/4/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/S/s.typ` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/S/s.typ`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/1/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/1/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/10/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/10/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/11/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/11/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/12/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/12/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/13/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/13/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/14/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/14/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/15/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/15/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/16/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/16/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/2/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/2/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/3/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/3/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/4/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/4/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/5/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/5/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/6/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/6/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/7/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/7/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/8/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/8/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/9/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/9/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/menu.json` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/menu.json`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/T/t.typ` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/T/t.typ`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/10/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/10/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/11/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/11/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/12/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/12/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/13/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/13/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/2/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/2/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/3/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/3/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/4/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/4/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/5/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/5/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/6/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/6/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/7/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/7/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/8/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/8/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/9/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/9/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/menu.json` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/menu.json`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/U/u.typ` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/U/u.typ`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/1/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/1/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/10/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/10/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/11/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/11/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/12/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/12/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/13/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/13/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/14/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/14/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/15/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/15/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/16/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/16/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/17/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/17/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/18/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/18/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/19/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/19/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/2/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/2/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/3/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/3/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/4/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/4/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/5/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/5/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/6/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/6/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/7/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/7/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/8/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/8/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/9/data.yaml` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/9/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/menu.json` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/menu.json`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/series/V/v.typ` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/series/V/v.typ`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/terminal_typing_tutor/tutor.py` & `terminal_typing_tutor-0.4.1/terminal_typing_tutor/tutor.py`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.4.0/PKG-INFO` & `terminal_typing_tutor-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal-typing-tutor
-Version: 0.4.0
+Version: 0.4.1
 Summary: Improve your touch-typing skills in the terminal, based on the GNU Typist program
 Home-page: https://github.com/justinsgithub/terminal-typing-tutor
 License: GPL-3.0-only
 Author: Justin Angeles
 Author-email: justinaawd@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

