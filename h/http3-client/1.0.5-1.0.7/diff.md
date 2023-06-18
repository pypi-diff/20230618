# Comparing `tmp/http3_client-1.0.5.tar.gz` & `tmp/http3_client-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "http3_client-1.0.5.tar", last modified: Sun Jun 18 09:47:07 2023, max compression
+gzip compressed data, was "http3_client-1.0.7.tar", last modified: Sun Jun 18 09:54:45 2023, max compression
```

## Comparing `http3_client-1.0.5.tar` & `http3_client-1.0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-18 09:47:07.937886 http3_client-1.0.5/
--rw-r--r--   0 admin      (501) staff       (20)       56 2023-06-18 09:47:07.937602 http3_client-1.0.5/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-06-18 09:47:07.937995 http3_client-1.0.5/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)      286 2023-06-18 09:46:21.000000 http3_client-1.0.5/setup.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-18 09:47:07.935088 http3_client-1.0.5/src/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-18 09:47:07.937044 http3_client-1.0.5/src/http3_client.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)       56 2023-06-18 09:47:07.000000 http3_client-1.0.5/src/http3_client.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      207 2023-06-18 09:47:07.000000 http3_client-1.0.5/src/http3_client.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-06-18 09:47:07.000000 http3_client-1.0.5/src/http3_client.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)        9 2023-06-18 09:47:07.000000 http3_client-1.0.5/src/http3_client.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-06-18 09:47:07.000000 http3_client-1.0.5/src/http3_client.egg-info/top_level.txt
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-18 09:54:45.942025 http3_client-1.0.7/
+-rw-r--r--   0 admin      (501) staff       (20)       56 2023-06-18 09:54:45.941787 http3_client-1.0.7/PKG-INFO
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-18 09:54:45.941399 http3_client-1.0.7/http3_client.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)       56 2023-06-18 09:54:45.000000 http3_client-1.0.7/http3_client.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      226 2023-06-18 09:54:45.000000 http3_client-1.0.7/http3_client.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-06-18 09:54:45.000000 http3_client-1.0.7/http3_client.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       39 2023-06-18 09:54:45.000000 http3_client-1.0.7/http3_client.egg-info/entry_points.txt
+-rw-r--r--   0 admin      (501) staff       (20)        9 2023-06-18 09:54:45.000000 http3_client-1.0.7/http3_client.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-06-18 09:54:45.000000 http3_client-1.0.7/http3_client.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-06-18 09:54:45.942129 http3_client-1.0.7/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)      445 2023-06-18 09:54:44.000000 http3_client-1.0.7/setup.py
```

