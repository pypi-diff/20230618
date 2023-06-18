# Comparing `tmp/pyopnsense-0.3.0.tar.gz` & `tmp/pyopnsense-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyopnsense-0.3.0.tar", last modified: Mon Nov  2 12:33:25 2020, max compression
+gzip compressed data, was "pyopnsense-0.4.0.tar", last modified: Sun Jun 18 19:46:01 2023, max compression
```

## Comparing `pyopnsense-0.3.0.tar` & `pyopnsense-0.4.0.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2020-11-02 12:33:25.425058 pyopnsense-0.3.0/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)       39 2019-11-28 10:15:15.000000 pyopnsense-0.3.0/.stestr.conf
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2020-11-02 12:33:25.421725 pyopnsense-0.3.0/.travis/
--rwxr-xr-x   0 computertreker  (1000) computertreker  (1000)       61 2019-11-28 10:19:20.000000 pyopnsense-0.3.0/.travis/coveralls.sh
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      667 2020-11-02 12:29:06.000000 pyopnsense-0.3.0/.travis.yml
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      187 2020-11-02 12:33:25.000000 pyopnsense-0.3.0/AUTHORS
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1137 2020-11-02 12:33:25.000000 pyopnsense-0.3.0/ChangeLog
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    35147 2019-11-28 10:15:15.000000 pyopnsense-0.3.0/LICENSE
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3365 2020-11-02 12:33:25.425058 pyopnsense-0.3.0/PKG-INFO
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2096 2019-11-28 10:19:20.000000 pyopnsense-0.3.0/README.rst
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      878 2020-11-02 12:29:06.000000 pyopnsense-0.3.0/azure-pipelines.yml
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2020-11-02 12:33:25.421725 pyopnsense-0.3.0/doc/
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2020-11-02 12:33:25.425058 pyopnsense-0.3.0/doc/source/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2098 2020-11-02 12:29:06.000000 pyopnsense-0.3.0/doc/source/api.rst
--rwxr-xr-x   0 computertreker  (1000) computertreker  (1000)     2699 2019-11-28 10:15:15.000000 pyopnsense-0.3.0/doc/source/conf.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)       78 2019-11-28 10:15:15.000000 pyopnsense-0.3.0/doc/source/index.rst
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)       30 2019-11-28 10:15:15.000000 pyopnsense-0.3.0/doc/source/readme.rst
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2020-11-02 12:33:25.425058 pyopnsense-0.3.0/pyopnsense/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)        0 2019-11-28 10:15:15.000000 pyopnsense-0.3.0/pyopnsense/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2234 2019-11-28 10:15:15.000000 pyopnsense-0.3.0/pyopnsense/client.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3780 2019-11-28 10:15:15.000000 pyopnsense-0.3.0/pyopnsense/diagnostics.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1093 2019-11-28 10:15:15.000000 pyopnsense-0.3.0/pyopnsense/exceptions.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1741 2019-11-28 10:15:15.000000 pyopnsense-0.3.0/pyopnsense/firmware.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1262 2020-11-02 12:29:06.000000 pyopnsense-0.3.0/pyopnsense/routes.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2020-11-02 12:33:25.425058 pyopnsense-0.3.0/pyopnsense/tests/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)        0 2019-11-28 10:15:15.000000 pyopnsense-0.3.0/pyopnsense/tests/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1241 2019-11-28 10:15:15.000000 pyopnsense-0.3.0/pyopnsense/tests/base.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2960 2019-11-28 10:15:15.000000 pyopnsense-0.3.0/pyopnsense/tests/test_client.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2020-11-02 12:33:25.425058 pyopnsense-0.3.0/pyopnsense.egg-info/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3365 2020-11-02 12:33:25.000000 pyopnsense-0.3.0/pyopnsense.egg-info/PKG-INFO
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      705 2020-11-02 12:33:25.000000 pyopnsense-0.3.0/pyopnsense.egg-info/SOURCES.txt
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)        1 2020-11-02 12:33:25.000000 pyopnsense-0.3.0/pyopnsense.egg-info/dependency_links.txt
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)        1 2020-11-02 12:33:25.000000 pyopnsense-0.3.0/pyopnsense.egg-info/not-zip-safe
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)       46 2020-11-02 12:33:25.000000 pyopnsense-0.3.0/pyopnsense.egg-info/pbr.json
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)       37 2020-11-02 12:33:25.000000 pyopnsense-0.3.0/pyopnsense.egg-info/requires.txt
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)       11 2020-11-02 12:33:25.000000 pyopnsense-0.3.0/pyopnsense.egg-info/top_level.txt
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      280 2019-11-28 10:15:15.000000 pyopnsense-0.3.0/requirements.txt
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      829 2020-11-02 12:33:25.425058 pyopnsense-0.3.0/setup.cfg
--rwxr-xr-x   0 computertreker  (1000) computertreker  (1000)     1065 2019-11-28 10:15:15.000000 pyopnsense-0.3.0/setup.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      329 2020-11-02 12:29:06.000000 pyopnsense-0.3.0/test-requirements.txt
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      851 2020-11-02 12:29:06.000000 pyopnsense-0.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:46:01.827845 pyopnsense-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:46:01.815844 pyopnsense-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:46:01.819844 pyopnsense-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-18 19:45:51.000000 pyopnsense-0.4.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-18 19:45:51.000000 pyopnsense-0.4.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-18 19:45:51.000000 pyopnsense-0.4.0/.stestr.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-18 19:46:01.000000 pyopnsense-0.4.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-18 19:46:01.000000 pyopnsense-0.4.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-18 19:45:51.000000 pyopnsense-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-18 19:46:01.827845 pyopnsense-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-18 19:45:51.000000 pyopnsense-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:46:01.815844 pyopnsense-0.4.0/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:46:01.823845 pyopnsense-0.4.0/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-18 19:45:51.000000 pyopnsense-0.4.0/doc/source/api.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2699 2023-06-18 19:45:51.000000 pyopnsense-0.4.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-18 19:45:51.000000 pyopnsense-0.4.0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-18 19:45:51.000000 pyopnsense-0.4.0/doc/source/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:46:01.823845 pyopnsense-0.4.0/pyopnsense/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 19:45:51.000000 pyopnsense-0.4.0/pyopnsense/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-18 19:45:51.000000 pyopnsense-0.4.0/pyopnsense/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-18 19:45:51.000000 pyopnsense-0.4.0/pyopnsense/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-18 19:45:51.000000 pyopnsense-0.4.0/pyopnsense/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-18 19:45:51.000000 pyopnsense-0.4.0/pyopnsense/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-18 19:45:51.000000 pyopnsense-0.4.0/pyopnsense/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-18 19:45:51.000000 pyopnsense-0.4.0/pyopnsense/firmware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-18 19:45:51.000000 pyopnsense-0.4.0/pyopnsense/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:46:01.827845 pyopnsense-0.4.0/pyopnsense/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 19:45:51.000000 pyopnsense-0.4.0/pyopnsense/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-18 19:45:51.000000 pyopnsense-0.4.0/pyopnsense/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-18 19:45:51.000000 pyopnsense-0.4.0/pyopnsense/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:46:01.827845 pyopnsense-0.4.0/pyopnsense.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-18 19:46:01.000000 pyopnsense-0.4.0/pyopnsense.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-18 19:46:01.000000 pyopnsense-0.4.0/pyopnsense.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 19:46:01.000000 pyopnsense-0.4.0/pyopnsense.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 19:46:01.000000 pyopnsense-0.4.0/pyopnsense.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-18 19:46:01.000000 pyopnsense-0.4.0/pyopnsense.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-18 19:46:01.000000 pyopnsense-0.4.0/pyopnsense.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-18 19:46:01.000000 pyopnsense-0.4.0/pyopnsense.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-18 19:45:51.000000 pyopnsense-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-18 19:46:01.827845 pyopnsense-0.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1056 2023-06-18 19:45:51.000000 pyopnsense-0.4.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-18 19:45:51.000000 pyopnsense-0.4.0/test-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-18 19:45:51.000000 pyopnsense-0.4.0/tox.ini
```

### Comparing `pyopnsense-0.3.0/LICENSE` & `pyopnsense-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopnsense-0.3.0/PKG-INFO` & `pyopnsense-0.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,86 +1,83 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyopnsense
-Version: 0.3.0
+Version: 0.4.0
 Summary: A python API client for OPNsense
-Home-page: UNKNOWN
 Author: Matthew Treinish
 Author-email: mtreinish@kortar.org
-License: UNKNOWN
-Description: ==========
-        pyopnsense
-        ==========
-        You can see the full rendered docs at: http://pyopnsense.readthedocs.io/en/latest/
-        
-        A python API client for the OPNsense API. This provides a python interface for
-        interacting with the OPNsense API.
-        
-        
-        Installation
-        ============
-        pyopnsense is available via pypi so all you need to do is run::
-        
-           pip install -U pyopnsense
-        
-        to get the latest pyopnsense release on your system. If you need to use a
-        development version of pyopnsense you can clone the repo and install it locally
-        with::
-        
-          git clone https://github.com/mtreinish/pyopnsense && pip install -e pyopnsense
-        
-        which will install pyopnsense in your python environment in editable mode for
-        development.
-        
-        .. _usage:
-        
-        Usage
-        =====
-        
-        To use pyopnsense you need a couple pieces of information, the API key and the
-        API secret. Both can be created/found from the OPNsense web UI by navigating
-        to: `System->Access->Users` under `API keys`.
-        
-        More information on this can be found in the OPNsense documentation:
-        https://docs.opnsense.org/development/how-tos/api.html
-        
-        Once you have the API key and API secret you can use pyopnsense to interact
-        with your OPNsense installation. You can do this by passing your credentials
-        to a client class. For example:
-        
-        .. code-block:: python
-        
-            from pyopnsense import diagnostics
-        
-            api_key = 'XXXXXX'
-            api_secret = 'XXXXXXXXXXXXXXX'
-            opnsense_url = 'http://192.168.1.1/api'
-        
-            netinsight_client = diagnostics.NetworkInsightClient(
-                api_key, api_secret, opnsense_url)
-        
-            print(netinsight_client.get_interfaces())
-        
-        which will print a dictionary mapping physical devices to their interface label.
-        
-        This same formula can be used to access each individual API endpoint you need
-        to access. The basic structure of the library is setup to roughly mirror the
-        endpoint tree of the OPNsense API. Each client module maps to the base endpoint
-        and then there is a client class in those modules for the next level up off
-        that.
-        
-        You can find more detail on how to use the clients in the API reference
-        documentation found here:
-        
-        http://pyopnsense.readthedocs.io/en/latest/api.html
-        
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+License-File: LICENSE
+
+==========
+pyopnsense
+==========
+You can see the full rendered docs at: http://pyopnsense.readthedocs.io/en/latest/
+
+A python API client for the OPNsense API. This provides a python interface for
+interacting with the OPNsense API.
+
+
+Installation
+============
+pyopnsense is available via pypi so all you need to do is run::
+
+   pip install -U pyopnsense
+
+to get the latest pyopnsense release on your system. If you need to use a
+development version of pyopnsense you can clone the repo and install it locally
+with::
+
+  git clone https://github.com/mtreinish/pyopnsense && pip install -e pyopnsense
+
+which will install pyopnsense in your python environment in editable mode for
+development.
+
+.. _usage:
+
+Usage
+=====
+
+To use pyopnsense you need a couple pieces of information, the API key and the
+API secret. Both can be created/found from the OPNsense web UI by navigating
+to: `System->Access->Users` under `API keys`.
+
+More information on this can be found in the OPNsense documentation:
+https://docs.opnsense.org/development/how-tos/api.html
+
+Once you have the API key and API secret you can use pyopnsense to interact
+with your OPNsense installation. You can do this by passing your credentials
+to a client class. For example:
+
+.. code-block:: python
+
+    from pyopnsense import diagnostics
+
+    api_key = 'XXXXXX'
+    api_secret = 'XXXXXXXXXXXXXXX'
+    opnsense_url = 'http://192.168.1.1/api'
+    timeout = 5
+
+    netinsight_client = diagnostics.NetworkInsightClient(
+        api_key, api_secret, opnsense_url, timeout)
+
+    print(netinsight_client.get_interfaces())
+
+which will print a dictionary mapping physical devices to their interface label.
+
+This same formula can be used to access each individual API endpoint you need
+to access. The basic structure of the library is setup to roughly mirror the
+endpoint tree of the OPNsense API. Each client module maps to the base endpoint
+and then there is a client class in those modules for the next level up off
+that.
+
+You can find more detail on how to use the clients in the API reference
+documentation found here:
+
+http://pyopnsense.readthedocs.io/en/latest/api.html
+
```

### Comparing `pyopnsense-0.3.0/README.rst` & `pyopnsense-0.4.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -41,17 +41,18 @@
 .. code-block:: python
 
     from pyopnsense import diagnostics
 
     api_key = 'XXXXXX'
     api_secret = 'XXXXXXXXXXXXXXX'
     opnsense_url = 'http://192.168.1.1/api'
+    timeout = 5
 
     netinsight_client = diagnostics.NetworkInsightClient(
-        api_key, api_secret, opnsense_url)
+        api_key, api_secret, opnsense_url, timeout)
 
     print(netinsight_client.get_interfaces())
 
 which will print a dictionary mapping physical devices to their interface label.
 
 This same formula can be used to access each individual API endpoint you need
 to access. The basic structure of the library is setup to roughly mirror the
```

### Comparing `pyopnsense-0.3.0/doc/source/api.rst` & `pyopnsense-0.4.0/doc/source/api.rst`

 * *Files identical despite different names*

### Comparing `pyopnsense-0.3.0/doc/source/conf.py` & `pyopnsense-0.4.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyopnsense-0.3.0/pyopnsense/client.py` & `pyopnsense-0.4.0/pyopnsense/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -27,35 +27,46 @@
 # All the successful HTTP status codes from RFC 7231 & 4918
 HTTP_SUCCESS = (200, 201, 202, 203, 204, 205, 206, 207)
 
 
 class OPNClient(object):
     """Representation of the OPNsense API client."""
 
-    def __init__(self, api_key, api_secret, base_url, verify_cert=False):
+    def __init__(
+        self, api_key, api_secret, base_url, verify_cert=False, timeout=DEFAULT_TIMEOUT
+    ):
         """Initialize the OPNsense API client."""
         self.api_key = api_key
         self.api_secret = api_secret
         self.base_url = base_url
         self.verify_cert = verify_cert
+        self.timeout = timeout
 
-    def _process_response(self, response):
+    def _process_response(self, response, raw=False):
         """Handle the response."""
         if response.status_code in HTTP_SUCCESS:
-            return json.loads(response.text)
+            return response.text if raw else json.loads(response.text)
         else:
             raise exceptions.APIException(
-                status_code=response.status_code, resp_body=response.text)
+                status_code=response.status_code, resp_body=response.text
+            )
 
-    def _get(self, endpoint):
-        req_url = '{}/{}'.format(self.base_url, endpoint)
-        response = requests.get(req_url, verify=self.verify_cert,
-                                auth=(self.api_key, self.api_secret),
-                                timeout=DEFAULT_TIMEOUT)
-        return self._process_response(response)
-
-    def _post(self, endpoint, body):
-        req_url = '{}/{}'.format(self.base_url, endpoint)
-        response = requests.post(req_url, data=body, verify=self.verify_cert,
-                                 auth=(self.api_key, self.api_secret),
-                                 timeout=DEFAULT_TIMEOUT)
-        return self._process_response(response)
+    def _get(self, endpoint, raw=False):
+        req_url = "{}/{}".format(self.base_url, endpoint)
+        response = requests.get(
+            req_url,
+            verify=self.verify_cert,
+            auth=(self.api_key, self.api_secret),
+            timeout=self.timeout,
+        )
+        return self._process_response(response, raw)
+
+    def _post(self, endpoint, body, raw=False):
+        req_url = "{}/{}".format(self.base_url, endpoint)
+        response = requests.post(
+            req_url,
+            data=body,
+            verify=self.verify_cert,
+            auth=(self.api_key, self.api_secret),
+            timeout=self.timeout,
+        )
+        return self._process_response(response, raw)
```

### Comparing `pyopnsense-0.3.0/pyopnsense/diagnostics.py` & `pyopnsense-0.4.0/pyopnsense/diagnostics.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,97 +11,105 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with pyopnsense. If not, see <http://www.gnu.org/licenses/>.
 
-from six.moves import urllib
+import urllib
 
 from pyopnsense import client
 
 
 class NetFlowClient(client.OPNClient):
     """A client for interacting with the diagnostics/netflow endpoint.
 
     :param str api_key: The API key to use for requests
     :param str api_secret: The API secret to use for requests
     :param str base_url: The base API endpoint for the OPNsense deployment
     """
+
     def status(self):
         """Return the current netflow status.
 
         :returns: A dict representing the current status of netflow
         :rtype: dict
         """
-        return self._get('diagnostics/netflow/status')
+        return self._get("diagnostics/netflow/status")
 
 
 class InterfaceClient(client.OPNClient):
     """A client for interacting with the diagnostics/interface endpoint
 
     :param str api_key: The API key to use for requests
     :param str api_secret: The API secret to use for requests
     :param str base_url: The base API endpoint for the OPNsense deployment
+    :param int timeout: The timeout in seconds for API requests
     """
+
     def get_ndp(self):
         """Get NDP table for router."""
-        return self._get('diagnostics/interface/getNdp')
+        return self._get("diagnostics/interface/getNdp")
 
     def get_arp(self):
         """Get ARP table for router."""
-        return self._get('diagnostics/interface/getArp')
+        return self._get("diagnostics/interface/getArp")
 
 
 class NetworkInsightClient(client.OPNClient):
     """A client for interacting with the diagnostics/networkinsight endpoint.
 
     :param str api_key: The API key to use for requests
     :param str api_secret: The API secret to use for requests
     :param str base_url: The base API endpoint for the OPNsense deployment
+    :param int timeout: The timeout in seconds for API requests
     """
+
     def get_interfaces(self):
         """Return the available interfaces."""
-        return self._get('diagnostics/networkinsight/getinterfaces')
+        return self._get("diagnostics/networkinsight/getinterfaces")
 
     def get_services(self):
         """Return the available services."""
-        return self._get('diagnostics/networkinsight/getservices')
+        return self._get("diagnostics/networkinsight/getservices")
 
     def get_protocols(self):
         """Return the protocols."""
-        return self._get('diagnostics/networkinsight/getprotocols')
+        return self._get("diagnostics/networkinsight/getprotocols")
 
     def get_timeserie(self):
         """Return the time serie."""
-        return self._get('diagnostics/networkinsight/timeserie')
+        return self._get("diagnostics/networkinsight/timeserie")
 
 
 class SystemHealthClient(client.OPNClient):
     """A client for interacting with the diagnostics/systemhealth endpoint.
 
     :param str api_key: The API key to use for requests
     :param str api_secret: The API secret to use for requests
     :param str base_url: The base API endpoint for the OPNsense deployment
+    :param int timeout: The timeout in seconds for API requests
     """
+
     def get_health_list(self):
         """Return the health list."""
-        return self._get('diagnostics/systemhealth/getRRDlist')
+        return self._get("diagnostics/systemhealth/getRRDlist")
 
-    def get_health_data(self, metric, start=0, stop=0, maxitems=1024,
-                        inverse=False, details=False):
+    def get_health_data(
+        self, metric, start=0, stop=0, maxitems=1024, inverse=False, details=False
+    ):
         """Return the health data."""
-        url = ['diagnostics/systemhealth/getSystemHealth']
+        url = ["diagnostics/systemhealth/getSystemHealth"]
         url.append(urllib.parse.quote(metric))
         url.append(start)
         url.append(stop)
         url.append(maxitems)
         if inverse:
-            url.append('true')
+            url.append("true")
         else:
-            url.append('false')
+            url.append("false")
         if details:
-            url.append('true')
+            url.append("true")
         else:
-            url.append('false')
+            url.append("false")
 
-        return self._get('/'.join(url))
+        return self._get("/".join(url))
```

### Comparing `pyopnsense-0.3.0/pyopnsense/exceptions.py` & `pyopnsense-0.4.0/pyopnsense/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,9 +19,9 @@
 class APIException(Exception):
     """Representation of the API exception."""
 
     def __init__(self, status_code=None, resp_body=None, *args, **kwargs):
         """Initialize the API exception."""
         self.resp_body = resp_body
         self.status_code = status_code
-        message = kwargs.get('message', resp_body)
+        message = kwargs.get("message", resp_body)
         super(APIException, self).__init__(message, *args, **kwargs)
```

### Comparing `pyopnsense-0.3.0/pyopnsense/firmware.py` & `pyopnsense-0.4.0/pyopnsense/firmware.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,28 +22,29 @@
 
 class FirmwareClient(client.OPNClient):
     """A client for interacting with the core/firmware endpoint.
 
     :param str api_key: The API key to use for requests
     :param str api_secret: The API secret to use for requests
     :param str base_url: The base API endpoint for the OPNsense deployment
+    :param int timeout: The timeout in seconds for API requests
     """
 
     def status(self):
         """Return the current firmware update status.
 
         :returns: A dict representing the current upgrade status for the
                   OPNsense firmware.
         :rtype: dict
         """
-        return self._get('core/firmware/status')
+        return self._get("core/firmware/status")
 
     def upgrade(self, upgrade_list=None):
         """Issue an upgrade request.
 
         :param list upgrade_list: The list of packages to upgrade. If none are
             specified it will issue a request to upgrade all packages.
         """
         if upgrade_list is None:
-            upgrade_list = 'all'
-        body = json.dumps({'upgrade': upgrade_list})
-        return self._post('core/firmware/upgrade', body)
+            upgrade_list = "all"
+        body = json.dumps({"upgrade": upgrade_list})
+        return self._post("core/firmware/upgrade", body)
```

### Comparing `pyopnsense-0.3.0/pyopnsense/routes.py` & `pyopnsense-0.4.0/pyopnsense/routes.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,16 +20,17 @@
 
 class GatewayClient(client.OPNClient):
     """A client for interacting with the routes/gateway endpoint.
 
     :param str api_key: The API key to use for requests
     :param str api_secret: The API secret to use for requests
     :param str base_url: The base API endpoint for the OPNsense deployment
+    :param int timeout: The timeout in seconds for API requests
     """
 
     def status(self):
         """Return the current gateways status.
 
         :returns: A dict representing the current status of gateways
         :rtype: dict
         """
-        return self._get('routes/gateway/status')
+        return self._get("routes/gateway/status")
```

### Comparing `pyopnsense-0.3.0/pyopnsense/tests/base.py` & `pyopnsense-0.4.0/pyopnsense/tests/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 # along with pyopnsense. If not, see <http://www.gnu.org/licenses/>.
 
 import fixtures
 import testtools
 
 
 class TestCase(testtools.TestCase):
-
     def setUp(self):
         super(TestCase, self).setUp()
-        stdout = self.useFixture(fixtures.StringStream('stdout')).stream
-        self.useFixture(fixtures.MonkeyPatch('sys.stdout', stdout))
-        stderr = self.useFixture(fixtures.StringStream('stderr')).stream
-        self.useFixture(fixtures.MonkeyPatch('sys.stderr', stderr))
-        self.useFixture(fixtures.LoggerFixture(nuke_handlers=False,
-                                               level=None))
+        stdout = self.useFixture(fixtures.StringStream("stdout")).stream
+        self.useFixture(fixtures.MonkeyPatch("sys.stdout", stdout))
+        stderr = self.useFixture(fixtures.StringStream("stderr")).stream
+        self.useFixture(fixtures.MonkeyPatch("sys.stderr", stderr))
+        self.useFixture(fixtures.LoggerFixture(nuke_handlers=False, level=None))
```

### Comparing `pyopnsense-0.3.0/pyopnsense/tests/test_client.py` & `pyopnsense-0.4.0/pyopnsense/tests/test_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,62 +14,64 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with pyopnsense. If not, see <http://www.gnu.org/licenses/>.
 
 
 import json
 
-import mock
+from unittest import mock
 
 from pyopnsense import client
 from pyopnsense import exceptions
 from pyopnsense.tests import base
 
 
 class TestOPNClient(base.TestCase):
-
-    @mock.patch('requests.get')
+    @mock.patch("requests.get")
     def test_get_success(self, request_mock):
         response_mock = mock.MagicMock()
         response_mock.status_code = 200
-        response_mock.text = json.dumps({'a': 'body'})
+        response_mock.text = json.dumps({"a": "body"})
         request_mock.return_value = response_mock
-        opnclient = client.OPNClient('', '', '')
-        resp = opnclient._get('fake_url')
-        self.assertEqual({'a': 'body'}, resp)
+        opnclient = client.OPNClient("", "", "", timeout=10)
+        resp = opnclient._get("fake_url")
+        self.assertEqual({"a": "body"}, resp)
         request_mock.assert_called_once_with(
-            '/fake_url', auth=('', ''), timeout=5, verify=False)
+            "/fake_url", auth=("", ""), timeout=10, verify=False
+        )
 
-    @mock.patch('requests.get')
+    @mock.patch("requests.get")
     def test_get_failures(self, request_mock):
         response_mock = mock.MagicMock()
         response_mock.status_code = 401
-        response_mock.text = json.dumps({'a': 'body'})
+        response_mock.text = json.dumps({"a": "body"})
         request_mock.return_value = response_mock
-        opnclient = client.OPNClient('', '', '')
-        self.assertRaises(exceptions.APIException, opnclient._get, 'fake_url')
+        opnclient = client.OPNClient("", "", "")
+        self.assertRaises(exceptions.APIException, opnclient._get, "fake_url")
         request_mock.assert_called_once_with(
-            '/fake_url', auth=('', ''), timeout=5, verify=False)
+            "/fake_url", auth=("", ""), timeout=5, verify=False
+        )
 
-    @mock.patch('requests.post')
+    @mock.patch("requests.post")
     def test_post_success(self, request_mock):
         response_mock = mock.MagicMock()
         response_mock.status_code = 200
-        response_mock.text = json.dumps({'a': 'body'})
+        response_mock.text = json.dumps({"a": "body"})
         request_mock.return_value = response_mock
-        opnclient = client.OPNClient('', '', '')
-        resp = opnclient._post('fake_url', 'body')
-        self.assertEqual({'a': 'body'}, resp)
+        opnclient = client.OPNClient("", "", "")
+        resp = opnclient._post("fake_url", "body")
+        self.assertEqual({"a": "body"}, resp)
         request_mock.assert_called_once_with(
-            '/fake_url', data='body', auth=('', ''), timeout=5, verify=False)
+            "/fake_url", data="body", auth=("", ""), timeout=5, verify=False
+        )
 
-    @mock.patch('requests.post')
+    @mock.patch("requests.post")
     def test_post_failures(self, request_mock):
         response_mock = mock.MagicMock()
         response_mock.status_code = 401
-        response_mock.text = json.dumps({'a': 'body'})
+        response_mock.text = json.dumps({"a": "body"})
         request_mock.return_value = response_mock
-        opnclient = client.OPNClient('', '', '')
-        self.assertRaises(
-            exceptions.APIException, opnclient._post, 'fake_url', 'body')
+        opnclient = client.OPNClient("", "", "")
+        self.assertRaises(exceptions.APIException, opnclient._post, "fake_url", "body")
         request_mock.assert_called_once_with(
-            '/fake_url', data='body', auth=('', ''), timeout=5, verify=False)
+            "/fake_url", data="body", auth=("", ""), timeout=5, verify=False
+        )
```

### Comparing `pyopnsense-0.3.0/pyopnsense.egg-info/PKG-INFO` & `pyopnsense-0.4.0/pyopnsense.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,86 +1,83 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyopnsense
-Version: 0.3.0
+Version: 0.4.0
 Summary: A python API client for OPNsense
-Home-page: UNKNOWN
 Author: Matthew Treinish
 Author-email: mtreinish@kortar.org
-License: UNKNOWN
-Description: ==========
-        pyopnsense
-        ==========
-        You can see the full rendered docs at: http://pyopnsense.readthedocs.io/en/latest/
-        
-        A python API client for the OPNsense API. This provides a python interface for
-        interacting with the OPNsense API.
-        
-        
-        Installation
-        ============
-        pyopnsense is available via pypi so all you need to do is run::
-        
-           pip install -U pyopnsense
-        
-        to get the latest pyopnsense release on your system. If you need to use a
-        development version of pyopnsense you can clone the repo and install it locally
-        with::
-        
-          git clone https://github.com/mtreinish/pyopnsense && pip install -e pyopnsense
-        
-        which will install pyopnsense in your python environment in editable mode for
-        development.
-        
-        .. _usage:
-        
-        Usage
-        =====
-        
-        To use pyopnsense you need a couple pieces of information, the API key and the
-        API secret. Both can be created/found from the OPNsense web UI by navigating
-        to: `System->Access->Users` under `API keys`.
-        
-        More information on this can be found in the OPNsense documentation:
-        https://docs.opnsense.org/development/how-tos/api.html
-        
-        Once you have the API key and API secret you can use pyopnsense to interact
-        with your OPNsense installation. You can do this by passing your credentials
-        to a client class. For example:
-        
-        .. code-block:: python
-        
-            from pyopnsense import diagnostics
-        
-            api_key = 'XXXXXX'
-            api_secret = 'XXXXXXXXXXXXXXX'
-            opnsense_url = 'http://192.168.1.1/api'
-        
-            netinsight_client = diagnostics.NetworkInsightClient(
-                api_key, api_secret, opnsense_url)
-        
-            print(netinsight_client.get_interfaces())
-        
-        which will print a dictionary mapping physical devices to their interface label.
-        
-        This same formula can be used to access each individual API endpoint you need
-        to access. The basic structure of the library is setup to roughly mirror the
-        endpoint tree of the OPNsense API. Each client module maps to the base endpoint
-        and then there is a client class in those modules for the next level up off
-        that.
-        
-        You can find more detail on how to use the clients in the API reference
-        documentation found here:
-        
-        http://pyopnsense.readthedocs.io/en/latest/api.html
-        
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+License-File: LICENSE
+
+==========
+pyopnsense
+==========
+You can see the full rendered docs at: http://pyopnsense.readthedocs.io/en/latest/
+
+A python API client for the OPNsense API. This provides a python interface for
+interacting with the OPNsense API.
+
+
+Installation
+============
+pyopnsense is available via pypi so all you need to do is run::
+
+   pip install -U pyopnsense
+
+to get the latest pyopnsense release on your system. If you need to use a
+development version of pyopnsense you can clone the repo and install it locally
+with::
+
+  git clone https://github.com/mtreinish/pyopnsense && pip install -e pyopnsense
+
+which will install pyopnsense in your python environment in editable mode for
+development.
+
+.. _usage:
+
+Usage
+=====
+
+To use pyopnsense you need a couple pieces of information, the API key and the
+API secret. Both can be created/found from the OPNsense web UI by navigating
+to: `System->Access->Users` under `API keys`.
+
+More information on this can be found in the OPNsense documentation:
+https://docs.opnsense.org/development/how-tos/api.html
+
+Once you have the API key and API secret you can use pyopnsense to interact
+with your OPNsense installation. You can do this by passing your credentials
+to a client class. For example:
+
+.. code-block:: python
+
+    from pyopnsense import diagnostics
+
+    api_key = 'XXXXXX'
+    api_secret = 'XXXXXXXXXXXXXXX'
+    opnsense_url = 'http://192.168.1.1/api'
+    timeout = 5
+
+    netinsight_client = diagnostics.NetworkInsightClient(
+        api_key, api_secret, opnsense_url, timeout)
+
+    print(netinsight_client.get_interfaces())
+
+which will print a dictionary mapping physical devices to their interface label.
+
+This same formula can be used to access each individual API endpoint you need
+to access. The basic structure of the library is setup to roughly mirror the
+endpoint tree of the OPNsense API. Each client module maps to the base endpoint
+and then there is a client class in those modules for the next level up off
+that.
+
+You can find more detail on how to use the clients in the API reference
+documentation found here:
+
+http://pyopnsense.readthedocs.io/en/latest/api.html
+
```

### Comparing `pyopnsense-0.3.0/setup.cfg` & `pyopnsense-0.4.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 [metadata]
 name = pyopnsense
 summary = A python API client for OPNsense
 homepage = http://github.com/mtreinish/pyopnsense
-description-file = 
+description_file = 
 	README.rst
 author = Matthew Treinish
-author-email = mtreinish@kortar.org
+author_email = mtreinish@kortar.org
 classifier = 
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Programming Language :: Python
-	Programming Language :: Python :: 2
-	Programming Language :: Python :: 2.7
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.5
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
+python_requires = >=3.8
 
 [files]
 packages = 
 	pyopnsense
 
 [build_sphinx]
 source-dir = doc/source
```

### Comparing `pyopnsense-0.3.0/setup.py` & `pyopnsense-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,10 +22,8 @@
 # setuptools if some other modules registered functions in `atexit`.
 # solution from: http://bugs.python.org/issue15881#msg170215
 try:
     import multiprocessing  # noqa
 except ImportError:
     pass
 
-setuptools.setup(
-    setup_requires=['pbr'],
-    pbr=True)
+setuptools.setup(setup_requires=["pbr"], pbr=True)
```

