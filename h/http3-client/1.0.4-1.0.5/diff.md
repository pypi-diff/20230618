# Comparing `tmp/http3_client-1.0.4.tar.gz` & `tmp/http3_client-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "http3_client-1.0.4.tar", last modified: Sun Jun 18 09:47:02 2023, max compression
+gzip compressed data, was "http3_client-1.0.5.tar", last modified: Sun Jun 18 09:47:07 2023, max compression
```

## Comparing `http3_client-1.0.4.tar` & `http3_client-1.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-18 09:47:02.986424 http3_client-1.0.4/
--rw-r--r--   0 admin      (501) staff       (20)       56 2023-06-18 09:47:02.985977 http3_client-1.0.4/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-06-18 09:47:02.986518 http3_client-1.0.4/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)      286 2023-06-18 09:46:21.000000 http3_client-1.0.4/setup.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-18 09:47:02.980671 http3_client-1.0.4/src/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-18 09:47:02.982958 http3_client-1.0.4/src/http3_client.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)       56 2023-06-18 09:47:02.000000 http3_client-1.0.4/src/http3_client.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      207 2023-06-18 09:47:02.000000 http3_client-1.0.4/src/http3_client.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-06-18 09:47:02.000000 http3_client-1.0.4/src/http3_client.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)        9 2023-06-18 09:47:02.000000 http3_client-1.0.4/src/http3_client.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-06-18 09:47:02.000000 http3_client-1.0.4/src/http3_client.egg-info/top_level.txt
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-18 09:47:07.937886 http3_client-1.0.5/
+-rw-r--r--   0 admin      (501) staff       (20)       56 2023-06-18 09:47:07.937602 http3_client-1.0.5/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-06-18 09:47:07.937995 http3_client-1.0.5/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)      286 2023-06-18 09:46:21.000000 http3_client-1.0.5/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-18 09:47:07.935088 http3_client-1.0.5/src/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-18 09:47:07.937044 http3_client-1.0.5/src/http3_client.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)       56 2023-06-18 09:47:07.000000 http3_client-1.0.5/src/http3_client.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      207 2023-06-18 09:47:07.000000 http3_client-1.0.5/src/http3_client.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-06-18 09:47:07.000000 http3_client-1.0.5/src/http3_client.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)        9 2023-06-18 09:47:07.000000 http3_client-1.0.5/src/http3_client.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-06-18 09:47:07.000000 http3_client-1.0.5/src/http3_client.egg-info/top_level.txt
```

