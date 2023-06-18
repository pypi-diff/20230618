# Comparing `tmp/ipcs-0.1.5.tar.gz` & `tmp/ipcs-0.1.5.post1.tar.gz`

## Comparing `ipcs-0.1.5.tar` & `ipcs-0.1.5.post1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 ipcs-0.1.5/CONTRIBUTING.md
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 ipcs-0.1.5/README.md
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 ipcs-0.1.5/mypy.ini
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 ipcs-0.1.5/test.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ipcs-0.1.5/.github/dependabot.yml
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 ipcs-0.1.5/.venv/.gitignore
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 ipcs-0.1.5/docs/conf.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 ipcs-0.1.5/docs/event_reference.rst
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 ipcs-0.1.5/docs/index.rst
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 ipcs-0.1.5/docs/ipcs.rst
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 ipcs-0.1.5/docs/modules.rst
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ipcs-0.1.5/docs/requirements.txt
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 ipcs-0.1.5/examples/chat.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 ipcs-0.1.5/examples/readme.md
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 ipcs-0.1.5/src/ipcs/__init__.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 ipcs-0.1.5/src/ipcs/__main__.py
--rw-r--r--   0        0        0    19183 2020-02-02 00:00:00.000000 ipcs-0.1.5/src/ipcs/client.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 ipcs-0.1.5/src/ipcs/connection.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 ipcs-0.1.5/src/ipcs/errors.py
--rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 ipcs-0.1.5/src/ipcs/server.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 ipcs-0.1.5/src/ipcs/types_.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 ipcs-0.1.5/src/ipcs/utils.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ipcs-0.1.5/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ipcs-0.1.5/LICENSE
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 ipcs-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 ipcs-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/CONTRIBUTING.md
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/mypy.ini
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/test.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/.venv/.gitignore
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/docs/conf.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/docs/event_reference.rst
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/docs/index.rst
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/docs/ipcs.rst
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/docs/modules.rst
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/docs/requirements.txt
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/examples/chat.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/examples/readme.md
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/src/ipcs/__init__.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/src/ipcs/__main__.py
+-rw-r--r--   0        0        0    19183 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/src/ipcs/client.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/src/ipcs/connection.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/src/ipcs/errors.py
+-rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/src/ipcs/server.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/src/ipcs/types_.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/src/ipcs/utils.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/LICENSE
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/README.md
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/pyproject.toml
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/PKG-INFO
```

### Comparing `ipcs-0.1.5/README.md` & `ipcs-0.1.5.post1/README.md`

 * *Files identical despite different names*

### Comparing `ipcs-0.1.5/test.py` & `ipcs-0.1.5.post1/test.py`

 * *Files identical despite different names*

### Comparing `ipcs-0.1.5/docs/conf.py` & `ipcs-0.1.5.post1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ipcs-0.1.5/docs/event_reference.rst` & `ipcs-0.1.5.post1/docs/event_reference.rst`

 * *Files identical despite different names*

### Comparing `ipcs-0.1.5/docs/index.rst` & `ipcs-0.1.5.post1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ipcs-0.1.5/docs/ipcs.rst` & `ipcs-0.1.5.post1/docs/ipcs.rst`

 * *Files identical despite different names*

### Comparing `ipcs-0.1.5/examples/chat.py` & `ipcs-0.1.5.post1/examples/chat.py`

 * *Files identical despite different names*

### Comparing `ipcs-0.1.5/src/ipcs/__main__.py` & `ipcs-0.1.5.post1/src/ipcs/__main__.py`

 * *Files identical despite different names*

### Comparing `ipcs-0.1.5/src/ipcs/client.py` & `ipcs-0.1.5.post1/src/ipcs/client.py`

 * *Files identical despite different names*

### Comparing `ipcs-0.1.5/src/ipcs/connection.py` & `ipcs-0.1.5.post1/src/ipcs/connection.py`

 * *Files identical despite different names*

### Comparing `ipcs-0.1.5/src/ipcs/errors.py` & `ipcs-0.1.5.post1/src/ipcs/errors.py`

 * *Files identical despite different names*

### Comparing `ipcs-0.1.5/src/ipcs/server.py` & `ipcs-0.1.5.post1/src/ipcs/server.py`

 * *Files identical despite different names*

### Comparing `ipcs-0.1.5/src/ipcs/types_.py` & `ipcs-0.1.5.post1/src/ipcs/types_.py`

 * *Files identical despite different names*

### Comparing `ipcs-0.1.5/src/ipcs/utils.py` & `ipcs-0.1.5.post1/src/ipcs/utils.py`

 * *Files identical despite different names*

### Comparing `ipcs-0.1.5/LICENSE` & `ipcs-0.1.5.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipcs-0.1.5/pyproject.toml` & `ipcs-0.1.5.post1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [project]
 name = "ipcs"
-version = "0.1.5"
+version = "0.1.5.post1"
 description = "Simple IPC server/client"
 keywords = ["ipc", "networking"]
 license = "MIT"
+readme = "README.md"
 license-files = { paths = ["LICENSE"] }
 classifiers = [
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.10",
     "Typing :: Typed"
 ]
 authors = [
```

