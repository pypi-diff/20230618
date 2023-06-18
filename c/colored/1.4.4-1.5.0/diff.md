# Comparing `tmp/colored-1.4.4.tar.gz` & `tmp/colored-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, from Unix
+gzip compressed data, was "colored-1.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `colored-1.4.4.tar` & `colored-1.5.0.tar`

### file list

```diff
@@ -1,44 +1,11 @@
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2022-11-11 16:39:51.000000 colored-1.4.4/
--rw-r--r--   0 dslackw   (1000) users      (100)     1070 2022-11-09 15:59:15.000000 colored-1.4.4/LICENSE.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     3665 2022-11-09 15:59:15.000000 colored-1.4.4/CHANGES.md
--rw-r--r--   0 dslackw   (1000) users      (100)      310 2022-11-09 15:59:15.000000 colored-1.4.4/MANIFEST.in
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2022-11-09 15:59:15.000000 colored-1.4.4/docs/
--rw-r--r--   0 dslackw   (1000) users      (100)     6223 2022-11-09 15:59:15.000000 colored-1.4.4/docs/back.COLOR.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     4943 2022-11-09 15:59:15.000000 colored-1.4.4/docs/colors_list.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     6219 2022-11-09 15:59:15.000000 colored-1.4.4/docs/fore.COLOR.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     3855 2022-11-09 15:59:15.000000 colored-1.4.4/docs/hex_list.txt
--rw-r--r--   0 dslackw   (1000) users      (100)      296 2022-11-09 15:59:15.000000 colored-1.4.4/docs/style.COLOR.txt
--rwxr-xr-x   0 dslackw   (1000) users      (100)     1173 2022-11-09 15:59:15.000000 colored-1.4.4/setup.py
--rw-r--r--   0 dslackw   (1000) users      (100)    13489 2022-11-09 15:59:15.000000 colored-1.4.4/README.rst
--rw-r--r--   0 dslackw   (1000) users      (100)       32 2022-11-09 15:59:15.000000 colored-1.4.4/requirements.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2022-11-09 15:59:15.000000 colored-1.4.4/tests/
--rwxr-xr-x   0 dslackw   (1000) users      (100)     6511 2022-11-09 15:59:15.000000 colored-1.4.4/tests/test_2.py
--rwxr-xr-x   0 dslackw   (1000) users      (100)      400 2022-11-09 15:59:15.000000 colored-1.4.4/tests/test_1.py
--rwxr-xr-x   0 dslackw   (1000) users      (100)     3111 2022-11-09 15:59:15.000000 colored-1.4.4/tests/test_hex_1.py
--rwxr-xr-x   0 dslackw   (1000) users      (100)     1006 2022-11-09 15:59:15.000000 colored-1.4.4/tests/test_hex_2.py
--rwxr-xr-x   0 dslackw   (1000) users      (100)     5424 2022-11-09 15:59:15.000000 colored-1.4.4/tests/test_3.py
--rwxr-xr-x   0 dslackw   (1000) users      (100)    32058 2022-11-09 15:59:15.000000 colored-1.4.4/tests/test_4.py
--rwxr-xr-x   0 dslackw   (1000) users      (100)     5424 2022-11-09 15:59:15.000000 colored-1.4.4/tests/test_5.py
--rw-r--r--   0 dslackw   (1000) users      (100)      153 2022-11-09 15:59:15.000000 colored-1.4.4/.travis.yml
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2022-11-11 16:39:47.000000 colored-1.4.4/colored.egg-info/
--rw-r--r--   0 dslackw   (1000) users      (100)        1 2022-11-11 16:39:47.000000 colored-1.4.4/colored.egg-info/dependency_links.txt
--rw-r--r--   0 dslackw   (1000) users      (100)      519 2022-11-11 16:39:47.000000 colored-1.4.4/colored.egg-info/SOURCES.txt
--rw-r--r--   0 dslackw   (1000) users      (100)        8 2022-11-11 16:39:47.000000 colored-1.4.4/colored.egg-info/top_level.txt
--rw-r--r--   0 dslackw   (1000) users      (100)    14472 2022-11-11 16:39:47.000000 colored-1.4.4/colored.egg-info/PKG-INFO
--rw-r--r--   0 dslackw   (1000) users      (100)       83 2022-11-09 15:59:15.000000 colored-1.4.4/.gitignore
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2022-11-11 16:39:47.000000 colored-1.4.4/colored/
--rw-r--r--   0 dslackw   (1000) users      (100)      495 2022-11-09 15:59:15.000000 colored-1.4.4/colored/style.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4991 2022-11-09 15:59:15.000000 colored-1.4.4/colored/colors.py
--rw-r--r--   0 dslackw   (1000) users      (100)    15844 2022-11-09 15:59:15.000000 colored-1.4.4/colored/colored.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2022-11-11 16:39:47.000000 colored-1.4.4/colored/__pycache__/
--rw-r--r--   0 dslackw   (1000) users      (100)      647 2022-11-11 16:39:47.000000 colored-1.4.4/colored/__pycache__/style.cpython-39.pyc
--rw-r--r--   0 dslackw   (1000) users      (100)      362 2022-11-11 16:39:47.000000 colored-1.4.4/colored/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 dslackw   (1000) users      (100)     3555 2022-11-11 16:39:47.000000 colored-1.4.4/colored/__pycache__/colors.cpython-39.pyc
--rw-r--r--   0 dslackw   (1000) users      (100)    10798 2022-11-11 16:39:47.000000 colored-1.4.4/colored/__pycache__/colored.cpython-39.pyc
--rw-r--r--   0 dslackw   (1000) users      (100)     5345 2022-11-11 16:39:47.000000 colored-1.4.4/colored/__pycache__/hex.cpython-39.pyc
--rw-r--r--   0 dslackw   (1000) users      (100)      441 2022-11-11 16:39:47.000000 colored-1.4.4/colored/__pycache__/back.cpython-39.pyc
--rw-r--r--   0 dslackw   (1000) users      (100)      441 2022-11-11 16:39:47.000000 colored-1.4.4/colored/__pycache__/fore.cpython-39.pyc
--rw-r--r--   0 dslackw   (1000) users      (100)      255 2022-11-09 15:59:15.000000 colored-1.4.4/colored/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6742 2022-11-09 15:59:15.000000 colored-1.4.4/colored/hex.py
--rw-r--r--   0 dslackw   (1000) users      (100)      209 2022-11-09 15:59:15.000000 colored-1.4.4/colored/fore.py
--rw-r--r--   0 dslackw   (1000) users      (100)      209 2022-11-09 15:59:15.000000 colored-1.4.4/colored/back.py
+-rw-r--r--   0        0        0     2303 2023-06-18 07:19:35.000000 colored-1.5.0/README.md
+-rw-r--r--   0        0        0      292 2023-06-18 07:19:35.000000 colored-1.5.0/colored/__init__.py
+-rw-r--r--   0        0        0      626 2023-06-18 07:19:35.000000 colored-1.5.0/colored/attributes.py
+-rw-r--r--   0        0        0      672 2023-06-18 07:19:35.000000 colored-1.5.0/colored/background.py
+-rw-r--r--   0        0        0     7416 2023-06-18 07:19:35.000000 colored-1.5.0/colored/colored.py
+-rw-r--r--   0        0        0      844 2023-06-18 07:19:35.000000 colored-1.5.0/colored/exceptions.py
+-rw-r--r--   0        0        0      672 2023-06-18 07:19:35.000000 colored-1.5.0/colored/foreground.py
+-rw-r--r--   0        0        0     1265 2023-06-18 07:19:35.000000 colored-1.5.0/colored/hex.py
+-rw-r--r--   0        0        0    12659 2023-06-18 07:19:35.000000 colored-1.5.0/colored/library.py
+-rw-r--r--   0        0        0     1141 2023-06-18 07:19:35.000000 colored-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3300 1970-01-01 00:00:00.000000 colored-1.5.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

