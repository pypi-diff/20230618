# Comparing `tmp/scratchattach-1.2.4.tar.gz` & `tmp/scratchattach-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchattach-1.2.4.tar", last modified: Sun Jun 11 01:57:25 2023, max compression
+gzip compressed data, was "scratchattach-1.2.5.tar", last modified: Sun Jun 18 13:54:23 2023, max compression
```

## Comparing `scratchattach-1.2.4.tar` & `scratchattach-1.2.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 01:57:25.211477 scratchattach-1.2.4/
--rw-rw-rw-   0        0        0    22094 2023-06-11 01:57:25.211477 scratchattach-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0    20730 2023-06-10 15:56:43.000000 scratchattach-1.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 01:57:25.196781 scratchattach-1.2.4/scratchattach/
--rw-rw-rw-   0        0        0      167 2023-06-10 15:02:36.000000 scratchattach-1.2.4/scratchattach/__init__.py
--rw-rw-rw-   0        0        0    13680 2023-06-10 19:50:37.000000 scratchattach-1.2.4/scratchattach/_cloud.py
--rw-rw-rw-   0        0        0    18072 2023-06-11 01:56:52.000000 scratchattach-1.2.4/scratchattach/_cloud_requests.py
--rw-rw-rw-   0        0        0     1797 2023-06-10 15:02:49.000000 scratchattach-1.2.4/scratchattach/_encoder.py
--rw-rw-rw-   0        0        0      888 2023-06-10 15:02:52.000000 scratchattach-1.2.4/scratchattach/_exceptions.py
--rw-rw-rw-   0        0        0     6558 2023-06-10 15:02:54.000000 scratchattach-1.2.4/scratchattach/_forum.py
--rw-rw-rw-   0        0        0    18239 2023-06-10 15:02:57.000000 scratchattach-1.2.4/scratchattach/_project.py
--rw-rw-rw-   0        0        0    17986 2023-06-10 16:04:19.000000 scratchattach-1.2.4/scratchattach/_session.py
--rw-rw-rw-   0        0        0     9728 2023-06-10 15:02:59.000000 scratchattach-1.2.4/scratchattach/_studio.py
--rw-rw-rw-   0        0        0    25434 2023-06-10 15:03:05.000000 scratchattach-1.2.4/scratchattach/_user.py
-drwxrwxrwx   0        0        0        0 2023-06-11 01:57:25.210476 scratchattach-1.2.4/scratchattach.egg-info/
--rw-rw-rw-   0        0        0    22094 2023-06-11 01:57:25.000000 scratchattach-1.2.4/scratchattach.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-06-11 01:57:25.000000 scratchattach-1.2.4/scratchattach.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 01:57:25.000000 scratchattach-1.2.4/scratchattach.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-11 01:57:25.000000 scratchattach-1.2.4/scratchattach.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-11 01:57:25.000000 scratchattach-1.2.4/scratchattach.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 01:57:25.212477 scratchattach-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1112 2023-06-11 01:56:05.000000 scratchattach-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 13:54:23.982103 scratchattach-1.2.5/
+-rw-rw-rw-   0        0        0    22053 2023-06-18 13:54:23.981105 scratchattach-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0    20730 2023-06-10 15:56:43.000000 scratchattach-1.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 13:54:23.930241 scratchattach-1.2.5/scratchattach/
+-rw-rw-rw-   0        0        0      167 2023-06-10 15:02:36.000000 scratchattach-1.2.5/scratchattach/__init__.py
+-rw-rw-rw-   0        0        0    13680 2023-06-10 19:50:37.000000 scratchattach-1.2.5/scratchattach/_cloud.py
+-rw-rw-rw-   0        0        0    18094 2023-06-18 13:54:00.000000 scratchattach-1.2.5/scratchattach/_cloud_requests.py
+-rw-rw-rw-   0        0        0     1797 2023-06-10 15:02:49.000000 scratchattach-1.2.5/scratchattach/_encoder.py
+-rw-rw-rw-   0        0        0      888 2023-06-10 15:02:52.000000 scratchattach-1.2.5/scratchattach/_exceptions.py
+-rw-rw-rw-   0        0        0     6558 2023-06-10 15:02:54.000000 scratchattach-1.2.5/scratchattach/_forum.py
+-rw-rw-rw-   0        0        0    18239 2023-06-10 15:02:57.000000 scratchattach-1.2.5/scratchattach/_project.py
+-rw-rw-rw-   0        0        0    17986 2023-06-10 16:04:19.000000 scratchattach-1.2.5/scratchattach/_session.py
+-rw-rw-rw-   0        0        0     9728 2023-06-10 15:02:59.000000 scratchattach-1.2.5/scratchattach/_studio.py
+-rw-rw-rw-   0        0        0    25434 2023-06-10 15:03:05.000000 scratchattach-1.2.5/scratchattach/_user.py
+drwxrwxrwx   0        0        0        0 2023-06-18 13:54:23.977116 scratchattach-1.2.5/scratchattach.egg-info/
+-rw-rw-rw-   0        0        0    22053 2023-06-18 13:54:23.000000 scratchattach-1.2.5/scratchattach.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-06-18 13:54:23.000000 scratchattach-1.2.5/scratchattach.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 13:54:23.000000 scratchattach-1.2.5/scratchattach.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-18 13:54:23.000000 scratchattach-1.2.5/scratchattach.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-18 13:54:23.000000 scratchattach-1.2.5/scratchattach.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 13:54:23.982103 scratchattach-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1112 2023-06-18 13:54:08.000000 scratchattach-1.2.5/setup.py
```

### Comparing `scratchattach-1.2.4/PKG-INFO` & `scratchattach-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.2.4
+Version: 1.2.5
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timmccool.scratch@gmail.com
-License: UNKNOWN
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -621,9 +619,7 @@
 - See the GitHub repository for full list of contributors.
 - Create a pull request to contribute code yourself.
 
 # Support
 
 If you need help with your code, leave a comment on TimMcCool's Scratch
 profile (https://scratch.mit.edu/users/TimMcCool/) or open an issue on the github repo
-
-
```

### Comparing `scratchattach-1.2.4/README.md` & `scratchattach-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.4/scratchattach/_cloud.py` & `scratchattach-1.2.5/scratchattach/_cloud.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.4/scratchattach/_cloud_requests.py` & `scratchattach-1.2.5/scratchattach/_cloud_requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -353,33 +353,34 @@
                 ]
 
             if self.ws_data != []:
                 event = self.ws_data.pop()
 
                 try:
                     raw_request, request_id = event.value.split(".")
+
+                    if event.value[0] == "-":
+                        if not request_id in self.request_parts:
+                            self.request_parts[request_id] = []
+                        self.request_parts[request_id].append(raw_request[1:])
+                        continue
+
                     if request_id in self.responded_request_ids:
                         continue
                     else:
                         self.responded_request_ids.insert(0, request_id)
                         self.responded_request_ids = self.responded_request_ids[:
                                                                                 15]
                 except Exception:
                     self.last_timestamp = event.timestamp
                     continue
 
                 self.last_requester = event.user
                 self.last_timestamp = event.timestamp
 
-                if event.value[0] == "-":
-                    if not request_id in self.request_parts:
-                        self.request_parts[request_id] = []
-                    self.request_parts[request_id].append(raw_request[1:])
-                    continue
-
                 _raw_request = ""
                 if request_id in self.request_parts:
                     data = self.request_parts[request_id]
                     for i in data:
                         _raw_request += i
                     self.request_parts.pop(request_id)
                 raw_request = _raw_request + raw_request
```

### Comparing `scratchattach-1.2.4/scratchattach/_encoder.py` & `scratchattach-1.2.5/scratchattach/_encoder.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.4/scratchattach/_exceptions.py` & `scratchattach-1.2.5/scratchattach/_exceptions.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.4/scratchattach/_forum.py` & `scratchattach-1.2.5/scratchattach/_forum.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.4/scratchattach/_project.py` & `scratchattach-1.2.5/scratchattach/_project.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.4/scratchattach/_session.py` & `scratchattach-1.2.5/scratchattach/_session.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.4/scratchattach/_studio.py` & `scratchattach-1.2.5/scratchattach/_studio.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.4/scratchattach/_user.py` & `scratchattach-1.2.5/scratchattach/_user.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.4/scratchattach.egg-info/PKG-INFO` & `scratchattach-1.2.5/scratchattach.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.2.4
+Version: 1.2.5
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timmccool.scratch@gmail.com
-License: UNKNOWN
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -621,9 +619,7 @@
 - See the GitHub repository for full list of contributors.
 - Create a pull request to contribute code yourself.
 
 # Support
 
 If you need help with your code, leave a comment on TimMcCool's Scratch
 profile (https://scratch.mit.edu/users/TimMcCool/) or open an issue on the github repo
-
-
```

### Comparing `scratchattach-1.2.4/setup.py` & `scratchattach-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.2.4'
+VERSION = '1.2.5'
 DESCRIPTION = 'An Scratch API Wrapper for scratch.mit.edu'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     name="scratchattach",
     version=VERSION,
```

