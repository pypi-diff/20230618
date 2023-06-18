# Comparing `tmp/classFig-0.0.5.tar.gz` & `tmp/classfig-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/classFig-0.0.5.tar", last modified: Sat May 20 10:45:52 2017, max compression
+gzip compressed data, was "classfig-0.1.4.tar", max compression
```

## Comparing `classFig-0.0.5.tar` & `classfig-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,6 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2017-05-20 10:45:52.000000 classFig-0.0.5/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2017-05-20 10:45:52.000000 classFig-0.0.5/classFig.egg-info/
--rw-r--r--   0 root         (0) staff       (20)        1 2017-05-20 10:45:52.000000 classFig-0.0.5/classFig.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)      430 2017-05-20 10:45:52.000000 classFig-0.0.5/classFig.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)       18 2017-05-20 10:45:52.000000 classFig-0.0.5/classFig.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)      190 2017-05-20 10:45:52.000000 classFig-0.0.5/classFig.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2017-05-20 10:45:52.000000 classFig-0.0.5/classFig.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)    11528 2017-05-18 17:03:28.000000 classFig-0.0.5/classFig.py
--rw-r--r--   0 root         (0) staff       (20)      430 2017-05-20 10:45:52.000000 classFig-0.0.5/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      563 2017-04-27 13:46:12.000000 classFig-0.0.5/README.txt
--rw-r--r--   0 root         (0) staff       (20)       59 2017-05-20 10:45:52.000000 classFig-0.0.5/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     1554 2017-05-20 10:44:46.000000 classFig-0.0.5/setup.py
+-rw-r--r--   0        0        0     1070 2023-05-16 20:11:50.008653 classfig-0.1.4/LICENSE
+-rw-r--r--   0        0        0      904 2023-06-18 05:51:05.134212 classfig-0.1.4/README.md
+-rw-r--r--   0        0        0      192 2023-06-18 06:31:15.537581 classfig-0.1.4/classfig/__init__.py
+-rwxr-xr-x   0        0        0    17612 2023-06-18 06:31:15.538128 classfig-0.1.4/classfig/classfig.py
+-rw-r--r--   0        0        0      641 2023-06-18 06:31:15.538559 classfig-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1611 1970-01-01 00:00:00.000000 classfig-0.1.4/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

