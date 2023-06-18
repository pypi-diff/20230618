# Comparing `tmp/scratchattach-1.2.5.tar.gz` & `tmp/scratchattach-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchattach-1.2.5.tar", last modified: Sun Jun 18 13:54:23 2023, max compression
+gzip compressed data, was "scratchattach-1.2.6.tar", last modified: Sun Jun 18 14:34:21 2023, max compression
```

## Comparing `scratchattach-1.2.5.tar` & `scratchattach-1.2.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 13:54:23.982103 scratchattach-1.2.5/
--rw-rw-rw-   0        0        0    22053 2023-06-18 13:54:23.981105 scratchattach-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0    20730 2023-06-10 15:56:43.000000 scratchattach-1.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 13:54:23.930241 scratchattach-1.2.5/scratchattach/
--rw-rw-rw-   0        0        0      167 2023-06-10 15:02:36.000000 scratchattach-1.2.5/scratchattach/__init__.py
--rw-rw-rw-   0        0        0    13680 2023-06-10 19:50:37.000000 scratchattach-1.2.5/scratchattach/_cloud.py
--rw-rw-rw-   0        0        0    18094 2023-06-18 13:54:00.000000 scratchattach-1.2.5/scratchattach/_cloud_requests.py
--rw-rw-rw-   0        0        0     1797 2023-06-10 15:02:49.000000 scratchattach-1.2.5/scratchattach/_encoder.py
--rw-rw-rw-   0        0        0      888 2023-06-10 15:02:52.000000 scratchattach-1.2.5/scratchattach/_exceptions.py
--rw-rw-rw-   0        0        0     6558 2023-06-10 15:02:54.000000 scratchattach-1.2.5/scratchattach/_forum.py
--rw-rw-rw-   0        0        0    18239 2023-06-10 15:02:57.000000 scratchattach-1.2.5/scratchattach/_project.py
--rw-rw-rw-   0        0        0    17986 2023-06-10 16:04:19.000000 scratchattach-1.2.5/scratchattach/_session.py
--rw-rw-rw-   0        0        0     9728 2023-06-10 15:02:59.000000 scratchattach-1.2.5/scratchattach/_studio.py
--rw-rw-rw-   0        0        0    25434 2023-06-10 15:03:05.000000 scratchattach-1.2.5/scratchattach/_user.py
-drwxrwxrwx   0        0        0        0 2023-06-18 13:54:23.977116 scratchattach-1.2.5/scratchattach.egg-info/
--rw-rw-rw-   0        0        0    22053 2023-06-18 13:54:23.000000 scratchattach-1.2.5/scratchattach.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-06-18 13:54:23.000000 scratchattach-1.2.5/scratchattach.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 13:54:23.000000 scratchattach-1.2.5/scratchattach.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-18 13:54:23.000000 scratchattach-1.2.5/scratchattach.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-18 13:54:23.000000 scratchattach-1.2.5/scratchattach.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 13:54:23.982103 scratchattach-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1112 2023-06-18 13:54:08.000000 scratchattach-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 14:34:21.491949 scratchattach-1.2.6/
+-rw-rw-rw-   0        0        0    21960 2023-06-18 14:34:21.490952 scratchattach-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0    20641 2023-06-18 14:23:06.000000 scratchattach-1.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 14:34:21.438093 scratchattach-1.2.6/scratchattach/
+-rw-rw-rw-   0        0        0      167 2023-06-10 15:02:36.000000 scratchattach-1.2.6/scratchattach/__init__.py
+-rw-rw-rw-   0        0        0    13982 2023-06-18 14:33:57.000000 scratchattach-1.2.6/scratchattach/_cloud.py
+-rw-rw-rw-   0        0        0    18499 2023-06-18 14:33:59.000000 scratchattach-1.2.6/scratchattach/_cloud_requests.py
+-rw-rw-rw-   0        0        0     1797 2023-06-10 15:02:49.000000 scratchattach-1.2.6/scratchattach/_encoder.py
+-rw-rw-rw-   0        0        0      888 2023-06-10 15:02:52.000000 scratchattach-1.2.6/scratchattach/_exceptions.py
+-rw-rw-rw-   0        0        0     6558 2023-06-10 15:02:54.000000 scratchattach-1.2.6/scratchattach/_forum.py
+-rw-rw-rw-   0        0        0    18239 2023-06-10 15:02:57.000000 scratchattach-1.2.6/scratchattach/_project.py
+-rw-rw-rw-   0        0        0    17986 2023-06-10 16:04:19.000000 scratchattach-1.2.6/scratchattach/_session.py
+-rw-rw-rw-   0        0        0     9728 2023-06-10 15:02:59.000000 scratchattach-1.2.6/scratchattach/_studio.py
+-rw-rw-rw-   0        0        0    25434 2023-06-10 15:03:05.000000 scratchattach-1.2.6/scratchattach/_user.py
+drwxrwxrwx   0        0        0        0 2023-06-18 14:34:21.487960 scratchattach-1.2.6/scratchattach.egg-info/
+-rw-rw-rw-   0        0        0    21960 2023-06-18 14:34:21.000000 scratchattach-1.2.6/scratchattach.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-06-18 14:34:21.000000 scratchattach-1.2.6/scratchattach.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 14:34:21.000000 scratchattach-1.2.6/scratchattach.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-18 14:34:21.000000 scratchattach-1.2.6/scratchattach.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-18 14:34:21.000000 scratchattach-1.2.6/scratchattach.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 14:34:21.492946 scratchattach-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1112 2023-06-18 14:23:24.000000 scratchattach-1.2.6/setup.py
```

### Comparing `scratchattach-1.2.5/PKG-INFO` & `scratchattach-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.2.5
+Version: 1.2.6
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timmccool.scratch@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -60,15 +60,15 @@
 
 **Logging in with a sessionId:**
 *You can get your session id from your browser's cookies. [More information](https://github.com/TimMcCool/scratchattach/wiki/Get-your-session-id)*
 
 ```python
 import scratchattach as scratch3
 
-session = scratch3.Session("sessionId", username="username")
+session = scratch3.Session("sessionId", username="username") #The username field is case sensitive
 ```
 
 **Attributes:**
 ```py
 session.session_id #Returns the associated session id
 session.xtoken
 session.email #Returns the email address associated with the account
@@ -117,21 +117,17 @@
 
 ```python
 value = scratch3.get_var("project_id", "variable")
 variables = scratch3.get_cloud("project_id") #Returns a dict with all cloud var values
 logs = scratch3.get_cloud_logs("project_id") #Returns the cloud logs as list
 ```
 
-**Get a Scratch / TurboWarp cloud var from the websocket:** (new in v0.8.0)
+**Get a Scratch / TurboWarp cloud var from the websocket:**
 
-Requires a connection to Scratch or TurboWarp's cloud (a `CloudConnection` / `TwCloudConnection` object).
-
-```python
-value = conn.get_var("variable")
-```
+This feature is not working at the moment.
 
 **Close the cloud connection:**
 
 ```python
 conn.disconnect()
 ```
```

### Comparing `scratchattach-1.2.5/README.md` & `scratchattach-1.2.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 **Logging in with a sessionId:**
 *You can get your session id from your browser's cookies. [More information](https://github.com/TimMcCool/scratchattach/wiki/Get-your-session-id)*
 
 ```python
 import scratchattach as scratch3
 
-session = scratch3.Session("sessionId", username="username")
+session = scratch3.Session("sessionId", username="username") #The username field is case sensitive
 ```
 
 **Attributes:**
 ```py
 session.session_id #Returns the associated session id
 session.xtoken
 session.email #Returns the email address associated with the account
@@ -101,21 +101,17 @@
 
 ```python
 value = scratch3.get_var("project_id", "variable")
 variables = scratch3.get_cloud("project_id") #Returns a dict with all cloud var values
 logs = scratch3.get_cloud_logs("project_id") #Returns the cloud logs as list
 ```
 
-**Get a Scratch / TurboWarp cloud var from the websocket:** (new in v0.8.0)
+**Get a Scratch / TurboWarp cloud var from the websocket:**
 
-Requires a connection to Scratch or TurboWarp's cloud (a `CloudConnection` / `TwCloudConnection` object).
-
-```python
-value = conn.get_var("variable")
-```
+This feature is not working at the moment.
 
 **Close the cloud connection:**
 
 ```python
 conn.disconnect()
 ```
```

### Comparing `scratchattach-1.2.5/scratchattach/_cloud.py` & `scratchattach-1.2.6/scratchattach/_cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,16 @@
     def __init__(self, *, project_id, username="python", session_id=None, cloud_host=None, _allow_non_numeric=False, _no_reconnect=False):
         self._session_id = session_id
         self._username = username
         try:
             self.project_id = int(project_id)
         except ValueError: #non-numeric project id (possible on turbowarp's cloud server)
             self.project_id = str(project_id)
-        self._ratelimited_until = 0#deals with the 0.1 second rate limit for cloud variable sets
+        self._ratelimited_until = 0 #deals with the 0.1 second rate limit for cloud variable sets
+        self._connect_timestamp = 0 #timestamp of when the cloud connection was opened
         self.websocket = websocket.WebSocket()
         self._no_reconnect = False
         self._connect(cloud_host=cloud_host)
         self._handshake()
         self._no_reconnect = _no_reconnect
         self.cloud_host = cloud_host
         self.allow_non_numeric = _allow_non_numeric #TurboWarp only. If this is true, turbowarp cloud variables can be set to non-numeric values (if) the cloud_host wss allows it)
@@ -82,14 +83,15 @@
                     "wss://clouddata.scratch.mit.edu",
                     cookie="scratchsessionsid=" + self._session_id + ";",
                     origin="https://scratch.mit.edu",
                     enable_multithread=True,
                 )
             except Exception:
                 raise(_exceptions.ConnectionError)
+        self._connect_timestamp = time.time()
 
     def set_var(self, variable, value):
         variable = variable.replace("☁ ", "")
         if not (value is True or value is False or value in [float('inf'), -float('inf')]):
             value = str(value)
             if len(value) > 256:
                 warnings.warn("invalid cloud var (too long): "+str(value), Warning)
@@ -138,14 +140,15 @@
                 self.cloud_host = "wss://clouddata.turbowarp.org/"
             self.websocket.connect(
                 cloud_host,
                 enable_multithread=True
             )
         except Exception:
             raise(_exceptions.ConnectionError)
+        self._connect_timestamp = time.time()
 
     def get_cloud(self, variable):
         try:
             variable = "☁ " + str(variable)
             self.set_var('@scratchattach','0')
 
             result = []
@@ -314,14 +317,16 @@
         self.connection = connection
         self.__dict__.update(entries)
 
     def _update(self):
         while True:
             try:
                 data = self.connection.websocket.recv().split('\n')
+                if len(data) > 1 and time.time() < self.connection._connect_timestamp + 0.5:
+                    continue
                 result = []
                 for i in data:
                     try:
                         result.append(json.loads(i))
                     except Exception:
                         pass
                 for activity in result:
```

### Comparing `scratchattach-1.2.5/scratchattach/_cloud_requests.py` & `scratchattach-1.2.6/scratchattach/_cloud_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,14 +175,26 @@
 
         return self.last_requester
 
     def get_timestamp(self):
 
         return self.last_timestamp
 
+    def get_exact_timestamp(self):
+
+        logs = _cloud.get_cloud_logs(self.project_id,
+                                     filter_by_var_named="TO_HOST")
+        activity = list(
+            filter(lambda x: "." + self.last_request_id in x["value"],
+                   logs))
+        if len(activity) > 0:
+            return activity[0]["timestamp"]
+        else:
+            return None
+
     def _respond(self, request_id, response, limit, *, validation=2222):
 
         if self.idle_since + 8 < time.time() or self.force_reconnect:
             self.connection._connect(cloud_host=self.connection.cloud_host)
             self.connection._handshake()
 
         remaining_response = str(response)
```

### Comparing `scratchattach-1.2.5/scratchattach/_encoder.py` & `scratchattach-1.2.6/scratchattach/_encoder.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.5/scratchattach/_exceptions.py` & `scratchattach-1.2.6/scratchattach/_exceptions.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.5/scratchattach/_forum.py` & `scratchattach-1.2.6/scratchattach/_forum.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.5/scratchattach/_project.py` & `scratchattach-1.2.6/scratchattach/_project.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.5/scratchattach/_session.py` & `scratchattach-1.2.6/scratchattach/_session.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.5/scratchattach/_studio.py` & `scratchattach-1.2.6/scratchattach/_studio.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.5/scratchattach/_user.py` & `scratchattach-1.2.6/scratchattach/_user.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.5/scratchattach.egg-info/PKG-INFO` & `scratchattach-1.2.6/scratchattach.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.2.5
+Version: 1.2.6
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timmccool.scratch@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -60,15 +60,15 @@
 
 **Logging in with a sessionId:**
 *You can get your session id from your browser's cookies. [More information](https://github.com/TimMcCool/scratchattach/wiki/Get-your-session-id)*
 
 ```python
 import scratchattach as scratch3
 
-session = scratch3.Session("sessionId", username="username")
+session = scratch3.Session("sessionId", username="username") #The username field is case sensitive
 ```
 
 **Attributes:**
 ```py
 session.session_id #Returns the associated session id
 session.xtoken
 session.email #Returns the email address associated with the account
@@ -117,21 +117,17 @@
 
 ```python
 value = scratch3.get_var("project_id", "variable")
 variables = scratch3.get_cloud("project_id") #Returns a dict with all cloud var values
 logs = scratch3.get_cloud_logs("project_id") #Returns the cloud logs as list
 ```
 
-**Get a Scratch / TurboWarp cloud var from the websocket:** (new in v0.8.0)
+**Get a Scratch / TurboWarp cloud var from the websocket:**
 
-Requires a connection to Scratch or TurboWarp's cloud (a `CloudConnection` / `TwCloudConnection` object).
-
-```python
-value = conn.get_var("variable")
-```
+This feature is not working at the moment.
 
 **Close the cloud connection:**
 
 ```python
 conn.disconnect()
 ```
```

### Comparing `scratchattach-1.2.5/setup.py` & `scratchattach-1.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.2.5'
+VERSION = '1.2.6'
 DESCRIPTION = 'An Scratch API Wrapper for scratch.mit.edu'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     name="scratchattach",
     version=VERSION,
```

