# Comparing `tmp/http3_client-1.0.0.tar.gz` & `tmp/http3_client-1.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "http3_client-1.0.0.tar", last modified: Sun Jun 18 09:16:14 2023, max compression
+gzip compressed data, was "http3_client-1.0.0.1.tar", last modified: Sun Jun 18 09:40:13 2023, max compression
```

## Comparing `http3_client-1.0.0.tar` & `http3_client-1.0.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-18 09:16:14.066868 http3_client-1.0.0/
--rw-r--r--   0 admin      (501) staff       (20)       56 2023-06-18 09:16:14.066506 http3_client-1.0.0/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-06-18 09:16:14.067006 http3_client-1.0.0/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)      120 2023-06-18 09:11:42.000000 http3_client-1.0.0/setup.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-18 09:16:14.063064 http3_client-1.0.0/src/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-18 09:16:14.065829 http3_client-1.0.0/src/http3_client.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)       56 2023-06-18 09:16:14.000000 http3_client-1.0.0/src/http3_client.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      207 2023-06-18 09:16:14.000000 http3_client-1.0.0/src/http3_client.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-06-18 09:16:14.000000 http3_client-1.0.0/src/http3_client.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)        9 2023-06-18 09:16:14.000000 http3_client-1.0.0/src/http3_client.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-06-18 09:16:14.000000 http3_client-1.0.0/src/http3_client.egg-info/top_level.txt
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-18 09:40:13.828208 http3_client-1.0.0.1/
+-rw-r--r--   0 admin      (501) staff       (20)       58 2023-06-18 09:40:13.827500 http3_client-1.0.0.1/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-06-18 09:40:13.828332 http3_client-1.0.0.1/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)      122 2023-06-18 09:34:10.000000 http3_client-1.0.0.1/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-18 09:40:13.822612 http3_client-1.0.0.1/src/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-18 09:40:13.826523 http3_client-1.0.0.1/src/http3_client.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)       58 2023-06-18 09:40:13.000000 http3_client-1.0.0.1/src/http3_client.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      207 2023-06-18 09:40:13.000000 http3_client-1.0.0.1/src/http3_client.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-06-18 09:40:13.000000 http3_client-1.0.0.1/src/http3_client.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)        9 2023-06-18 09:40:13.000000 http3_client-1.0.0.1/src/http3_client.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-06-18 09:40:13.000000 http3_client-1.0.0.1/src/http3_client.egg-info/top_level.txt
```

