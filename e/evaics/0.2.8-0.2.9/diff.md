# Comparing `tmp/evaics-0.2.8.tar.gz` & `tmp/evaics-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evaics-0.2.8.tar", last modified: Fri May 26 14:58:11 2023, max compression
+gzip compressed data, was "evaics-0.2.9.tar", last modified: Fri May 26 15:38:26 2023, max compression
```

## Comparing `evaics-0.2.8.tar` & `evaics-0.2.9.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-26 14:58:11.378689 evaics-0.2.8/
--rw-r--r--   0 divisor   (1000) root         (0)    10639 2022-06-30 23:31:52.000000 evaics-0.2.8/LICENSE
--rw-r--r--   0 divisor   (1000) root         (0)      637 2023-05-26 14:58:11.378689 evaics-0.2.8/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)      141 2022-10-03 20:48:30.000000 evaics-0.2.8/README.md
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-26 14:58:11.378689 evaics-0.2.8/evaics/
--rw-r--r--   0 divisor   (1000) root         (0)        0 2023-05-26 14:57:27.000000 evaics-0.2.8/evaics/__init__.py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-26 14:58:11.378689 evaics-0.2.8/evaics/client/
--rw-r--r--   0 divisor   (1000) root         (0)      131 2023-05-26 14:57:27.000000 evaics-0.2.8/evaics/client/__init__.py
--rw-r--r--   0 divisor   (1000) root         (0)     4559 2023-05-26 14:57:27.000000 evaics-0.2.8/evaics/client/http.py
--rw-r--r--   0 divisor   (1000) root         (0)     1821 2023-05-26 14:57:27.000000 evaics-0.2.8/evaics/exceptions.py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-26 14:58:11.378689 evaics-0.2.8/evaics/sdk/
--rw-r--r--   0 divisor   (1000) root         (0)    27404 2023-05-26 14:57:27.000000 evaics-0.2.8/evaics/sdk/__init__.py
--rw-r--r--   0 divisor   (1000) root         (0)     1116 2023-05-26 14:57:27.000000 evaics-0.2.8/evaics/tools.py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-26 14:58:11.378689 evaics-0.2.8/evaics.egg-info/
--rw-r--r--   0 divisor   (1000) root         (0)      637 2023-05-26 14:58:11.000000 evaics-0.2.8/evaics.egg-info/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)      302 2023-05-26 14:58:11.000000 evaics-0.2.8/evaics.egg-info/SOURCES.txt
--rw-r--r--   0 divisor   (1000) root         (0)        1 2023-05-26 14:58:11.000000 evaics-0.2.8/evaics.egg-info/dependency_links.txt
--rw-r--r--   0 divisor   (1000) root         (0)       28 2023-05-26 14:58:11.000000 evaics-0.2.8/evaics.egg-info/requires.txt
--rw-r--r--   0 divisor   (1000) root         (0)        7 2023-05-26 14:58:11.000000 evaics-0.2.8/evaics.egg-info/top_level.txt
--rw-r--r--   0 divisor   (1000) root         (0)       38 2023-05-26 14:58:11.378689 evaics-0.2.8/setup.cfg
--rw-r--r--   0 divisor   (1000) root         (0)      787 2023-05-26 14:57:27.000000 evaics-0.2.8/setup.py
+drwxrwxr-x   0 divisor   (1000) divisor   (1000)        0 2023-05-26 15:38:26.618934 evaics-0.2.9/
+-rw-rw-r--   0 divisor   (1000) divisor   (1000)      674 2023-05-26 15:38:26.618934 evaics-0.2.9/PKG-INFO
+-rw-rw-r--   0 divisor   (1000) divisor   (1000)      141 2022-10-03 21:34:26.000000 evaics-0.2.9/README.md
+drwxrwxr-x   0 divisor   (1000) divisor   (1000)        0 2023-05-26 15:38:26.618934 evaics-0.2.9/evaics/
+-rw-rw-r--   0 divisor   (1000) divisor   (1000)        0 2023-05-26 15:37:59.000000 evaics-0.2.9/evaics/__init__.py
+drwxrwxr-x   0 divisor   (1000) divisor   (1000)        0 2023-05-26 15:38:26.618934 evaics-0.2.9/evaics/client/
+-rw-rw-r--   0 divisor   (1000) divisor   (1000)      131 2023-05-26 15:37:59.000000 evaics-0.2.9/evaics/client/__init__.py
+-rw-rw-r--   0 divisor   (1000) divisor   (1000)     4559 2023-05-26 15:37:59.000000 evaics-0.2.9/evaics/client/http.py
+-rw-rw-r--   0 divisor   (1000) divisor   (1000)     1821 2023-05-26 15:37:59.000000 evaics-0.2.9/evaics/exceptions.py
+drwxrwxr-x   0 divisor   (1000) divisor   (1000)        0 2023-05-26 15:38:26.618934 evaics-0.2.9/evaics/sdk/
+-rw-rw-r--   0 divisor   (1000) divisor   (1000)    27630 2023-05-26 15:37:59.000000 evaics-0.2.9/evaics/sdk/__init__.py
+-rw-rw-r--   0 divisor   (1000) divisor   (1000)     1116 2023-05-26 15:37:59.000000 evaics-0.2.9/evaics/tools.py
+drwxrwxr-x   0 divisor   (1000) divisor   (1000)        0 2023-05-26 15:38:26.618934 evaics-0.2.9/evaics.egg-info/
+-rw-rw-r--   0 divisor   (1000) divisor   (1000)      674 2023-05-26 15:38:26.000000 evaics-0.2.9/evaics.egg-info/PKG-INFO
+-rw-rw-r--   0 divisor   (1000) divisor   (1000)      294 2023-05-26 15:38:26.000000 evaics-0.2.9/evaics.egg-info/SOURCES.txt
+-rw-rw-r--   0 divisor   (1000) divisor   (1000)        1 2023-05-26 15:38:26.000000 evaics-0.2.9/evaics.egg-info/dependency_links.txt
+-rw-rw-r--   0 divisor   (1000) divisor   (1000)       28 2023-05-26 15:38:26.000000 evaics-0.2.9/evaics.egg-info/requires.txt
+-rw-rw-r--   0 divisor   (1000) divisor   (1000)        7 2023-05-26 15:38:26.000000 evaics-0.2.9/evaics.egg-info/top_level.txt
+-rw-rw-r--   0 divisor   (1000) divisor   (1000)       38 2023-05-26 15:38:26.618934 evaics-0.2.9/setup.cfg
+-rw-rw-r--   0 divisor   (1000) divisor   (1000)      787 2023-05-26 15:37:59.000000 evaics-0.2.9/setup.py
```

### Comparing `evaics-0.2.8/PKG-INFO` & `evaics-0.2.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: evaics
-Version: 0.2.8
+Version: 0.2.9
 Summary: EVA ICS v4 Python SDK
 Home-page: https://github.com/eva-ics/eva4
 Author: Bohemia Automation / Altertech
 Author-email: div@altertech.com
 License: Apache License 2.0
+Description: # EVA ICS v4 SDK (Python)
+        
+        EVA ICS v4 software development kit (Python)
+        
+        Technical documentation: <https://info.bma.ai/en/actual/eva4/sdk/>
+        
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Communications
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# EVA ICS v4 SDK (Python)
-
-EVA ICS v4 software development kit (Python)
-
-Technical documentation: <https://info.bma.ai/en/actual/eva4/sdk/>
-
-
-
```

### Comparing `evaics-0.2.8/evaics/client/http.py` & `evaics-0.2.9/evaics/client/http.py`

 * *Files identical despite different names*

### Comparing `evaics-0.2.8/evaics/exceptions.py` & `evaics-0.2.9/evaics/exceptions.py`

 * *Files identical despite different names*

### Comparing `evaics-0.2.8/evaics/sdk/__init__.py` & `evaics-0.2.9/evaics/sdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.2.8'
+__version__ = '0.2.9'
 
 import busrt
 import sys
 import msgpack
 import logging
 import time
 import signal
@@ -553,27 +553,33 @@
         def log_trace(msg, *args, **kwargs):
             logger.log(1, msg, *args, **kwargs)
 
         logger.trace = log_trace
         self.logger = logger
         return self.logger
 
-    def block(self):
+    def block(self, prepare=True):
         """
         Block the service until terminated
 
         Automatically calls register_signals, mark_ready, mark_terminating
         (after receiving a termination signal/event)
+
+        Optional:
+            prepare: default: True, if False, register_signals, mark_ready and
+                     mark_terminating must be called manually
         """
-        self.register_signals()
-        self.mark_ready()
+        if prepare:
+            self.register_signals()
+            self.mark_ready()
         sleep_step = self.sleep_step
         while self.active and self.bus.is_connected():
             time.sleep(sleep_step)
-        self.mark_terminating()
+        if prepare:
+            self.mark_terminating()
 
     def mark_ready(self):
         """
         Mark the service ready
 
         Automatically logs the service is started if logs are initialized
         """
```

### Comparing `evaics-0.2.8/evaics/tools.py` & `evaics-0.2.9/evaics/tools.py`

 * *Files identical despite different names*

### Comparing `evaics-0.2.8/evaics.egg-info/PKG-INFO` & `evaics-0.2.9/evaics.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: evaics
-Version: 0.2.8
+Version: 0.2.9
 Summary: EVA ICS v4 Python SDK
 Home-page: https://github.com/eva-ics/eva4
 Author: Bohemia Automation / Altertech
 Author-email: div@altertech.com
 License: Apache License 2.0
+Description: # EVA ICS v4 SDK (Python)
+        
+        EVA ICS v4 software development kit (Python)
+        
+        Technical documentation: <https://info.bma.ai/en/actual/eva4/sdk/>
+        
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Communications
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# EVA ICS v4 SDK (Python)
-
-EVA ICS v4 software development kit (Python)
-
-Technical documentation: <https://info.bma.ai/en/actual/eva4/sdk/>
-
-
-
```

### Comparing `evaics-0.2.8/setup.py` & `evaics-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.2.8'
+__version__ = '0.2.9'
 
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
```

