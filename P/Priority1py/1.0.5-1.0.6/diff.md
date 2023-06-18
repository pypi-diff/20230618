# Comparing `tmp/Priority1py-1.0.5.tar.gz` & `tmp/Priority1py-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Priority1py-1.0.5.tar", last modified: Sun Jun 18 02:09:06 2023, max compression
+gzip compressed data, was "dist\Priority1py-1.0.6.tar", last modified: Sun Jun 18 02:14:01 2023, max compression
```

## Comparing `Priority1py-1.0.5.tar` & `Priority1py-1.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 02:09:06.000000 Priority1py-1.0.5/
--rw-rw-rw-   0        0        0      769 2023-06-18 02:09:06.000000 Priority1py-1.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-18 02:09:06.000000 Priority1py-1.0.5/Priority1py/
--rw-rw-rw-   0        0        0     4632 2023-06-18 02:03:23.000000 Priority1py-1.0.5/Priority1py/Priority1py.py
--rw-rw-rw-   0        0        0      157 2023-06-18 02:07:51.000000 Priority1py-1.0.5/Priority1py/__init__.py
--rw-rw-rw-   0        0        0     1353 2023-06-15 02:44:19.000000 Priority1py-1.0.5/Priority1py/request.py
--rw-rw-rw-   0        0        0      960 2023-06-17 23:52:34.000000 Priority1py-1.0.5/Priority1py/strings.py
--rw-rw-rw-   0        0        0      246 2023-06-18 01:23:34.000000 Priority1py-1.0.5/Priority1py/test.py
--rw-rw-rw-   0        0        0       42 2023-06-15 00:31:48.000000 Priority1py-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1646 2023-06-18 02:08:24.000000 Priority1py-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 02:14:01.000000 Priority1py-1.0.6/
+-rw-rw-rw-   0        0        0      769 2023-06-18 02:14:01.000000 Priority1py-1.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-18 02:14:01.000000 Priority1py-1.0.6/Priority1py/
+-rw-rw-rw-   0        0        0     4641 2023-06-18 02:12:59.000000 Priority1py-1.0.6/Priority1py/Priority1py.py
+-rw-rw-rw-   0        0        0      157 2023-06-18 02:07:51.000000 Priority1py-1.0.6/Priority1py/__init__.py
+-rw-rw-rw-   0        0        0     1353 2023-06-15 02:44:19.000000 Priority1py-1.0.6/Priority1py/request.py
+-rw-rw-rw-   0        0        0      960 2023-06-17 23:52:34.000000 Priority1py-1.0.6/Priority1py/strings.py
+-rw-rw-rw-   0        0        0      246 2023-06-18 01:23:34.000000 Priority1py-1.0.6/Priority1py/test.py
+-rw-rw-rw-   0        0        0       42 2023-06-15 00:31:48.000000 Priority1py-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1646 2023-06-18 02:13:32.000000 Priority1py-1.0.6/setup.py
```

### Comparing `Priority1py-1.0.5/PKG-INFO` & `Priority1py-1.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: Priority1py
-Version: 1.0.5
+Version: 1.0.6
 Summary: Priority 1 web API python library
 Home-page: https://github.com/reid10305/Priority1py
 Author: Daniel Pifer
 Author-email: UNKNOWN
 License: MIT
-Download-URL: https://github.com/reid10305/Priority1py/archive/refs/tags/v1.0.5.tar.gz
+Download-URL: https://github.com/reid10305/Priority1py/archive/refs/tags/v1.0.6.tar.gz
 Description: UNKNOWN
 Keywords: API,Priority1
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Priority1py-1.0.5/Priority1py/Priority1py.py` & `Priority1py-1.0.6/Priority1py/Priority1py.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from Priority1py.request import req_send
-from Priority1py.strings import Endpoint, Crud, Accessorial, IDType
+from Priority1py.strings import Endpoint, Crud, Accessorial, IDType, Details
 # from request import req_send
 # from strings import Endpoint, Crud, Accessorial, IDType, Details
 import json
 from datetime import datetime
 
 class Priority1py():
     ''' API helper class '''
```

### Comparing `Priority1py-1.0.5/Priority1py/request.py` & `Priority1py-1.0.6/Priority1py/request.py`

 * *Files identical despite different names*

### Comparing `Priority1py-1.0.5/Priority1py/strings.py` & `Priority1py-1.0.6/Priority1py/strings.py`

 * *Files identical despite different names*

### Comparing `Priority1py-1.0.5/setup.py` & `Priority1py-1.0.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 
 from distutils.core import setup
 setup(
   name = 'Priority1py',         # How you named your package folder (MyLib)
   packages = ['Priority1py'],   # Chose the same as "name"
-  version = '1.0.5',      # Start with a small number and increase it with every change you make
+  version = '1.0.6',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Priority 1 web API python library',   # Give a short description about your library
   author = 'Daniel Pifer',                   # Type in your name
   author_email = '',      # Type in your E-Mail
   url = 'https://github.com/reid10305/Priority1py',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/reid10305/Priority1py/archive/refs/tags/v1.0.5.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/reid10305/Priority1py/archive/refs/tags/v1.0.6.tar.gz',    # I explain this later on
   keywords = ['API', 'Priority1'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'requests'
       ],
   classifiers=[
     'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
```

