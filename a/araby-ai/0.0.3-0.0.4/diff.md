# Comparing `tmp/araby-ai-0.0.3.tar.gz` & `tmp/araby-ai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "araby-ai-0.0.3.tar", last modified: Sun Jun 11 21:08:49 2023, max compression
+gzip compressed data, was "araby-ai-0.0.4.tar", last modified: Sun Jun 18 19:11:05 2023, max compression
```

## Comparing `araby-ai-0.0.3.tar` & `araby-ai-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-11 21:08:49.331823 araby-ai-0.0.3/
--rw-rw----   0 root         (0) everybody  (9997)       20 2023-06-11 12:12:33.000000 araby-ai-0.0.3/LICENSE.txt
--rw-rw----   0 root         (0) everybody  (9997)      336 2023-06-11 21:08:49.319823 araby-ai-0.0.3/PKG-INFO
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-11 21:08:49.215823 araby-ai-0.0.3/araby_ai/
--rw-rw----   0 root         (0) everybody  (9997)      876 2023-06-11 21:07:59.000000 araby-ai-0.0.3/araby_ai/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     1175 2023-06-11 21:07:29.000000 araby-ai-0.0.3/araby_ai/signup.py
--rw-rw----   0 root         (0) everybody  (9997)     2656 2023-06-11 13:45:51.000000 araby-ai-0.0.3/araby_ai/writenow.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-11 21:08:49.299823 araby-ai-0.0.3/araby_ai.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      336 2023-06-11 21:08:48.000000 araby-ai-0.0.3/araby_ai.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      209 2023-06-11 21:08:48.000000 araby-ai-0.0.3/araby_ai.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-11 21:08:48.000000 araby-ai-0.0.3/araby_ai.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)        9 2023-06-11 21:08:48.000000 araby-ai-0.0.3/araby_ai.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-11 21:08:49.335823 araby-ai-0.0.3/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      377 2023-06-11 21:08:19.000000 araby-ai-0.0.3/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-18 19:11:05.748000 araby-ai-0.0.4/
+-rw-rw----   0 root         (0) everybody  (9997)       20 2023-06-11 12:12:33.000000 araby-ai-0.0.4/LICENSE.txt
+-rw-rw----   0 root         (0) everybody  (9997)      336 2023-06-18 19:11:05.724000 araby-ai-0.0.4/PKG-INFO
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-18 19:11:05.608000 araby-ai-0.0.4/araby_ai/
+-rw-rw----   0 root         (0) everybody  (9997)      700 2023-06-18 19:10:14.000000 araby-ai-0.0.4/araby_ai/ArabyGPT.py
+-rw-rw----   0 root         (0) everybody  (9997)      900 2023-06-14 13:22:58.000000 araby-ai-0.0.4/araby_ai/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     1175 2023-06-11 21:07:29.000000 araby-ai-0.0.4/araby_ai/signup.py
+-rw-rw----   0 root         (0) everybody  (9997)     2656 2023-06-11 13:45:51.000000 araby-ai-0.0.4/araby_ai/writenow.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-18 19:11:05.700000 araby-ai-0.0.4/araby_ai.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      336 2023-06-18 19:11:05.000000 araby-ai-0.0.4/araby_ai.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      230 2023-06-18 19:11:05.000000 araby-ai-0.0.4/araby_ai.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-18 19:11:05.000000 araby-ai-0.0.4/araby_ai.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)        9 2023-06-18 19:11:05.000000 araby-ai-0.0.4/araby_ai.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-18 19:11:05.752000 araby-ai-0.0.4/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      377 2023-06-18 19:10:56.000000 araby-ai-0.0.4/setup.py
```

### Comparing `araby-ai-0.0.3/araby_ai/__init__.py` & `araby-ai-0.0.4/araby_ai/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .writenow import *
 from .signup import *
+from .ArabyGPT import *
 import requests, random, re
 
 class Client:
 	def __init__(self, email, password):
 		headers = {
 			"authority": "v1.prd.socket.araby.ai",
 			"accept": "application/json, text/plain, */*",
```

### Comparing `araby-ai-0.0.3/araby_ai/signup.py` & `araby-ai-0.0.4/araby_ai/signup.py`

 * *Files identical despite different names*

### Comparing `araby-ai-0.0.3/araby_ai/writenow.py` & `araby-ai-0.0.4/araby_ai/writenow.py`

 * *Files identical despite different names*

