# Comparing `tmp/connect_python-0.1.0.dev1.tar.gz` & `tmp/connect_python-0.1.0.dev2.tar.gz`

## Comparing `connect_python-0.1.0.dev1.tar` & `connect_python-0.1.0.dev2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 connect_python-0.1.0.dev1/src/connect/__init__.py
--rw-r--r--   0        0        0     5239 2020-02-02 00:00:00.000000 connect_python-0.1.0.dev1/src/connect/client.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 connect_python-0.1.0.dev1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 connect_python-0.1.0.dev1/LICENSE
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 connect_python-0.1.0.dev1/README.md
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 connect_python-0.1.0.dev1/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 connect_python-0.1.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 connect_python-0.1.0.dev2/src/connect/__init__.py
+-rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 connect_python-0.1.0.dev2/src/connect/client.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 connect_python-0.1.0.dev2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 connect_python-0.1.0.dev2/LICENSE
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 connect_python-0.1.0.dev2/README.md
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 connect_python-0.1.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 connect_python-0.1.0.dev2/PKG-INFO
```

### Comparing `connect_python-0.1.0.dev1/src/connect/client.py` & `connect_python-0.1.0.dev2/src/connect/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,7 +186,13 @@
                     # if EnvelopeFlags.compression in flags:
                     resp = self._response_type()
                     resp.ParseFromString(buffer)
                     yield resp
 
                     buffer = buffer[data_len:]
                     needs_header = True
+
+    def call_client_stream(self, req):
+        raise NotImplementedError("client stream not supported")
+
+    def call_bidi_stream(self, req):
+        raise NotImplementedError("bidi stream not supported")
```

### Comparing `connect_python-0.1.0.dev1/LICENSE` & `connect_python-0.1.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `connect_python-0.1.0.dev1/pyproject.toml` & `connect_python-0.1.0.dev2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "connect-python"
-version = "0.1.0.dev1"
+version = "0.1.0.dev2"
 authors = [{ email = "matt@ydekproductions.com" }]
 description = "Client implementation for the Connect RPC protocol"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `connect_python-0.1.0.dev1/PKG-INFO` & `connect_python-0.1.0.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connect-python
-Version: 0.1.0.dev1
+Version: 0.1.0.dev2
 Summary: Client implementation for the Connect RPC protocol
 Project-URL: Homepage, https://github.com/mattrobenolt/connect-python
 Project-URL: Bug Tracker, https://github.com/mattrobenolt/connect-python/issues
 Author-email: matt@ydekproductions.com
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

