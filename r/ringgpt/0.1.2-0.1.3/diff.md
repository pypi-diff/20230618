# Comparing `tmp/ringgpt-0.1.2.tar.gz` & `tmp/ringgpt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ringgpt-0.1.2.tar", max compression
+gzip compressed data, was "ringgpt-0.1.3.tar", max compression
```

## Comparing `ringgpt-0.1.2.tar` & `ringgpt-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-17 17:22:54.403042 ringgpt-0.1.2/README.md
--rw-r--r--   0        0        0      591 2023-06-18 16:18:52.423688 ringgpt-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       84 2023-06-17 17:25:10.567674 ringgpt-0.1.2/ringgpt/__init__.py
--rw-r--r--   0        0        0     1988 2023-06-18 15:38:01.724785 ringgpt-0.1.2/ringgpt/dataloader.py
--rw-r--r--   0        0        0     5710 2023-06-18 15:36:24.315528 ringgpt-0.1.2/ringgpt/prompt.py
--rw-r--r--   0        0        0    10672 2023-06-18 15:50:57.342661 ringgpt-0.1.2/ringgpt/ring.py
--rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 ringgpt-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-17 17:22:54.403042 ringgpt-0.1.3/README.md
+-rw-r--r--   0        0        0      591 2023-06-18 16:22:56.935048 ringgpt-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       84 2023-06-17 17:25:10.567674 ringgpt-0.1.3/ringgpt/__init__.py
+-rw-r--r--   0        0        0     1988 2023-06-18 15:38:01.724785 ringgpt-0.1.3/ringgpt/dataloader.py
+-rw-r--r--   0        0        0     5710 2023-06-18 15:36:24.315528 ringgpt-0.1.3/ringgpt/prompt.py
+-rw-r--r--   0        0        0    10672 2023-06-18 15:50:57.342661 ringgpt-0.1.3/ringgpt/ring.py
+-rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 ringgpt-0.1.3/PKG-INFO
```

### Comparing `ringgpt-0.1.2/pyproject.toml` & `ringgpt-0.1.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ringgpt"
-version = "0.1.2"
+version = "0.1.3"
 description = "Package enables users to iterate on a corpus to perform single shot completion tasks leveraging GPT-3.5, Bard and Bing Chat"
 authors = ["Avinaash Anand K <avinaash96@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `ringgpt-0.1.2/ringgpt/dataloader.py` & `ringgpt-0.1.3/ringgpt/dataloader.py`

 * *Files identical despite different names*

### Comparing `ringgpt-0.1.2/ringgpt/prompt.py` & `ringgpt-0.1.3/ringgpt/prompt.py`

 * *Files identical despite different names*

### Comparing `ringgpt-0.1.2/ringgpt/ring.py` & `ringgpt-0.1.3/ringgpt/ring.py`

 * *Files identical despite different names*

### Comparing `ringgpt-0.1.2/PKG-INFO` & `ringgpt-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ringgpt
-Version: 0.1.2
+Version: 0.1.3
 Summary: Package enables users to iterate on a corpus to perform single shot completion tasks leveraging GPT-3.5, Bard and Bing Chat
 License: Apache-2.0
 Author: Avinaash Anand K
 Author-email: avinaash96@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

