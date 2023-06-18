# Comparing `tmp/towdio_player-1.0.1.tar.gz` & `tmp/towdio_player-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "towdio_player-1.0.1.tar", last modified: Sun Jun 18 11:33:12 2023, max compression
+gzip compressed data, was "towdio_player-1.0.2.tar", last modified: Sun Jun 18 11:40:15 2023, max compression
```

## Comparing `towdio_player-1.0.1.tar` & `towdio_player-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-18 11:33:12.519205 towdio_player-1.0.1/
--rw-r--r--   0 thowie     (501) staff       (20)      145 2023-06-18 11:33:12.519072 towdio_player-1.0.1/PKG-INFO
--rw-r--r--   0 thowie     (501) staff       (20)       38 2023-06-18 11:33:12.519258 towdio_player-1.0.1/setup.cfg
--rw-r--r--   0 thowie     (501) staff       (20)      438 2023-06-18 11:33:09.000000 towdio_player-1.0.1/setup.py
-drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-18 11:33:12.517867 towdio_player-1.0.1/towdio_player/
--rw-r--r--   0 thowie     (501) staff       (20)        0 2023-06-18 11:11:57.000000 towdio_player-1.0.1/towdio_player/__init__.py
--rw-r--r--   0 thowie     (501) staff       (20)      435 2023-06-18 11:28:04.000000 towdio_player-1.0.1/towdio_player/towdio_player.py
-drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-18 11:33:12.518883 towdio_player-1.0.1/towdio_player.egg-info/
--rw-r--r--   0 thowie     (501) staff       (20)      145 2023-06-18 11:33:12.000000 towdio_player-1.0.1/towdio_player.egg-info/PKG-INFO
--rw-r--r--   0 thowie     (501) staff       (20)      289 2023-06-18 11:33:12.000000 towdio_player-1.0.1/towdio_player.egg-info/SOURCES.txt
--rw-r--r--   0 thowie     (501) staff       (20)        1 2023-06-18 11:33:12.000000 towdio_player-1.0.1/towdio_player.egg-info/dependency_links.txt
--rw-r--r--   0 thowie     (501) staff       (20)       67 2023-06-18 11:33:12.000000 towdio_player-1.0.1/towdio_player.egg-info/entry_points.txt
--rw-r--r--   0 thowie     (501) staff       (20)       22 2023-06-18 11:33:12.000000 towdio_player-1.0.1/towdio_player.egg-info/requires.txt
--rw-r--r--   0 thowie     (501) staff       (20)       14 2023-06-18 11:33:12.000000 towdio_player-1.0.1/towdio_player.egg-info/top_level.txt
+drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-18 11:40:15.380062 towdio_player-1.0.2/
+-rw-r--r--   0 thowie     (501) staff       (20)      145 2023-06-18 11:40:15.379922 towdio_player-1.0.2/PKG-INFO
+-rw-r--r--   0 thowie     (501) staff       (20)       38 2023-06-18 11:40:15.380122 towdio_player-1.0.2/setup.cfg
+-rw-r--r--   0 thowie     (501) staff       (20)      437 2023-06-18 11:40:03.000000 towdio_player-1.0.2/setup.py
+drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-18 11:40:15.378366 towdio_player-1.0.2/towdio_player/
+-rw-r--r--   0 thowie     (501) staff       (20)        0 2023-06-18 11:11:57.000000 towdio_player-1.0.2/towdio_player/__init__.py
+-rw-r--r--   0 thowie     (501) staff       (20)      485 2023-06-18 11:38:49.000000 towdio_player-1.0.2/towdio_player/towdio_player.py
+drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-18 11:40:15.379689 towdio_player-1.0.2/towdio_player.egg-info/
+-rw-r--r--   0 thowie     (501) staff       (20)      145 2023-06-18 11:40:15.000000 towdio_player-1.0.2/towdio_player.egg-info/PKG-INFO
+-rw-r--r--   0 thowie     (501) staff       (20)      289 2023-06-18 11:40:15.000000 towdio_player-1.0.2/towdio_player.egg-info/SOURCES.txt
+-rw-r--r--   0 thowie     (501) staff       (20)        1 2023-06-18 11:40:15.000000 towdio_player-1.0.2/towdio_player.egg-info/dependency_links.txt
+-rw-r--r--   0 thowie     (501) staff       (20)       67 2023-06-18 11:40:15.000000 towdio_player-1.0.2/towdio_player.egg-info/entry_points.txt
+-rw-r--r--   0 thowie     (501) staff       (20)       22 2023-06-18 11:40:15.000000 towdio_player-1.0.2/towdio_player.egg-info/requires.txt
+-rw-r--r--   0 thowie     (501) staff       (20)       14 2023-06-18 11:40:15.000000 towdio_player-1.0.2/towdio_player.egg-info/top_level.txt
```

