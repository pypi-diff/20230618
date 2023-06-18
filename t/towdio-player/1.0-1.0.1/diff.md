# Comparing `tmp/towdio_player-1.0.tar.gz` & `tmp/towdio_player-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "towdio_player-1.0.tar", last modified: Sun Jun 18 11:19:07 2023, max compression
+gzip compressed data, was "towdio_player-1.0.1.tar", last modified: Sun Jun 18 11:33:12 2023, max compression
```

## Comparing `towdio_player-1.0.tar` & `towdio_player-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-18 11:19:07.984026 towdio_player-1.0/
--rw-r--r--   0 thowie     (501) staff       (20)      146 2023-06-18 11:19:07.983906 towdio_player-1.0/PKG-INFO
--rw-r--r--   0 thowie     (501) staff       (20)       38 2023-06-18 11:19:07.984068 towdio_player-1.0/setup.cfg
--rw-r--r--   0 thowie     (501) staff       (20)      297 2023-06-18 11:18:29.000000 towdio_player-1.0/setup.py
-drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-18 11:19:07.982876 towdio_player-1.0/towdio_player/
--rw-r--r--   0 thowie     (501) staff       (20)        0 2023-06-18 11:11:57.000000 towdio_player-1.0/towdio_player/__init__.py
--rw-r--r--   0 thowie     (501) staff       (20)      362 2023-06-18 11:02:22.000000 towdio_player-1.0/towdio_player/script.py
-drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-18 11:19:07.983717 towdio_player-1.0/towdio_player.egg-info/
--rw-r--r--   0 thowie     (501) staff       (20)      146 2023-06-18 11:19:07.000000 towdio_player-1.0/towdio_player.egg-info/PKG-INFO
--rw-r--r--   0 thowie     (501) staff       (20)      242 2023-06-18 11:19:07.000000 towdio_player-1.0/towdio_player.egg-info/SOURCES.txt
--rw-r--r--   0 thowie     (501) staff       (20)        1 2023-06-18 11:19:07.000000 towdio_player-1.0/towdio_player.egg-info/dependency_links.txt
--rw-r--r--   0 thowie     (501) staff       (20)       22 2023-06-18 11:19:07.000000 towdio_player-1.0/towdio_player.egg-info/requires.txt
--rw-r--r--   0 thowie     (501) staff       (20)       14 2023-06-18 11:19:07.000000 towdio_player-1.0/towdio_player.egg-info/top_level.txt
+drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-18 11:33:12.519205 towdio_player-1.0.1/
+-rw-r--r--   0 thowie     (501) staff       (20)      145 2023-06-18 11:33:12.519072 towdio_player-1.0.1/PKG-INFO
+-rw-r--r--   0 thowie     (501) staff       (20)       38 2023-06-18 11:33:12.519258 towdio_player-1.0.1/setup.cfg
+-rw-r--r--   0 thowie     (501) staff       (20)      438 2023-06-18 11:33:09.000000 towdio_player-1.0.1/setup.py
+drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-18 11:33:12.517867 towdio_player-1.0.1/towdio_player/
+-rw-r--r--   0 thowie     (501) staff       (20)        0 2023-06-18 11:11:57.000000 towdio_player-1.0.1/towdio_player/__init__.py
+-rw-r--r--   0 thowie     (501) staff       (20)      435 2023-06-18 11:28:04.000000 towdio_player-1.0.1/towdio_player/towdio_player.py
+drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-18 11:33:12.518883 towdio_player-1.0.1/towdio_player.egg-info/
+-rw-r--r--   0 thowie     (501) staff       (20)      145 2023-06-18 11:33:12.000000 towdio_player-1.0.1/towdio_player.egg-info/PKG-INFO
+-rw-r--r--   0 thowie     (501) staff       (20)      289 2023-06-18 11:33:12.000000 towdio_player-1.0.1/towdio_player.egg-info/SOURCES.txt
+-rw-r--r--   0 thowie     (501) staff       (20)        1 2023-06-18 11:33:12.000000 towdio_player-1.0.1/towdio_player.egg-info/dependency_links.txt
+-rw-r--r--   0 thowie     (501) staff       (20)       67 2023-06-18 11:33:12.000000 towdio_player-1.0.1/towdio_player.egg-info/entry_points.txt
+-rw-r--r--   0 thowie     (501) staff       (20)       22 2023-06-18 11:33:12.000000 towdio_player-1.0.1/towdio_player.egg-info/requires.txt
+-rw-r--r--   0 thowie     (501) staff       (20)       14 2023-06-18 11:33:12.000000 towdio_player-1.0.1/towdio_player.egg-info/top_level.txt
```

