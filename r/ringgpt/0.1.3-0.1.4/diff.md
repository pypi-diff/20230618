# Comparing `tmp/ringgpt-0.1.3.tar.gz` & `tmp/ringgpt-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ringgpt-0.1.3.tar", max compression
+gzip compressed data, was "ringgpt-0.1.4.tar", max compression
```

## Comparing `ringgpt-0.1.3.tar` & `ringgpt-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-17 17:22:54.403042 ringgpt-0.1.3/README.md
--rw-r--r--   0        0        0      591 2023-06-18 16:22:56.935048 ringgpt-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       84 2023-06-17 17:25:10.567674 ringgpt-0.1.3/ringgpt/__init__.py
--rw-r--r--   0        0        0     1988 2023-06-18 15:38:01.724785 ringgpt-0.1.3/ringgpt/dataloader.py
--rw-r--r--   0        0        0     5710 2023-06-18 15:36:24.315528 ringgpt-0.1.3/ringgpt/prompt.py
--rw-r--r--   0        0        0    10672 2023-06-18 15:50:57.342661 ringgpt-0.1.3/ringgpt/ring.py
--rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 ringgpt-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-17 17:22:54.403042 ringgpt-0.1.4/README.md
+-rw-r--r--   0        0        0      590 2023-06-18 16:33:40.101689 ringgpt-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       84 2023-06-17 17:25:10.567674 ringgpt-0.1.4/ringgpt/__init__.py
+-rw-r--r--   0        0        0     1988 2023-06-18 15:38:01.724785 ringgpt-0.1.4/ringgpt/dataloader.py
+-rw-r--r--   0        0        0     5710 2023-06-18 15:36:24.315528 ringgpt-0.1.4/ringgpt/prompt.py
+-rw-r--r--   0        0        0    10672 2023-06-18 15:50:57.342661 ringgpt-0.1.4/ringgpt/ring.py
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 ringgpt-0.1.4/PKG-INFO
```

### Comparing `ringgpt-0.1.3/pyproject.toml` & `ringgpt-0.1.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "ringgpt"
-version = "0.1.3"
+version = "0.1.4"
 description = "Package enables users to iterate on a corpus to perform single shot completion tasks leveraging GPT-3.5, Bard and Bing Chat"
 authors = ["Avinaash Anand K <avinaash96@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "^2.0.2"
 bard = "^0.1"
 asyncio = "^3.4.3"
-EdgeGPT = "^0.11.1"
+EdgeGPT = "^0.5.0"
 revChatGPT = "^6.3.3"
 requests = "^2.31.0"
 rich = "^13.4.2"
 langchain = "^0.0.202"
 tiktoken = "^0.4.0"
```

### Comparing `ringgpt-0.1.3/ringgpt/dataloader.py` & `ringgpt-0.1.4/ringgpt/dataloader.py`

 * *Files identical despite different names*

### Comparing `ringgpt-0.1.3/ringgpt/prompt.py` & `ringgpt-0.1.4/ringgpt/prompt.py`

 * *Files identical despite different names*

### Comparing `ringgpt-0.1.3/ringgpt/ring.py` & `ringgpt-0.1.4/ringgpt/ring.py`

 * *Files identical despite different names*

### Comparing `ringgpt-0.1.3/PKG-INFO` & `ringgpt-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: ringgpt
-Version: 0.1.3
+Version: 0.1.4
 Summary: Package enables users to iterate on a corpus to perform single shot completion tasks leveraging GPT-3.5, Bard and Bing Chat
 License: Apache-2.0
 Author: Avinaash Anand K
 Author-email: avinaash96@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: EdgeGPT (>=0.11.1,<0.12.0)
+Requires-Dist: EdgeGPT (>=0.5.0,<0.6.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: bard (>=0.1,<0.2)
 Requires-Dist: langchain (>=0.0.202,<0.0.203)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: revChatGPT (>=6.3.3,<7.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
```

