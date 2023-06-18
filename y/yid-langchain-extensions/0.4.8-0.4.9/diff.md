# Comparing `tmp/yid_langchain_extensions-0.4.8.tar.gz` & `tmp/yid_langchain_extensions-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yid_langchain_extensions-0.4.8.tar", last modified: Sun Jun 18 07:30:03 2023, max compression
+gzip compressed data, was "yid_langchain_extensions-0.4.9.tar", last modified: Sun Jun 18 08:07:33 2023, max compression
```

## Comparing `yid_langchain_extensions-0.4.8.tar` & `yid_langchain_extensions-0.4.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:30:03.365272 yid_langchain_extensions-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-18 07:29:44.000000 yid_langchain_extensions-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-18 07:30:03.365272 yid_langchain_extensions-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-18 07:29:44.000000 yid_langchain_extensions-0.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 07:30:03.365272 yid_langchain_extensions-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-18 07:29:44.000000 yid_langchain_extensions-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:30:03.365272 yid_langchain_extensions-0.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 07:29:44.000000 yid_langchain_extensions-0.4.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-06-18 07:29:44.000000 yid_langchain_extensions-0.4.8/tests/test_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:30:03.365272 yid_langchain_extensions-0.4.8/yid_langchain_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 07:29:44.000000 yid_langchain_extensions-0.4.8/yid_langchain_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:30:03.365272 yid_langchain_extensions-0.4.8/yid_langchain_extensions/output_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 07:29:44.000000 yid_langchain_extensions-0.4.8/yid_langchain_extensions/output_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-18 07:29:44.000000 yid_langchain_extensions-0.4.8/yid_langchain_extensions/output_parser/action_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-18 07:29:44.000000 yid_langchain_extensions-0.4.8/yid_langchain_extensions/output_parser/class_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-18 07:29:44.000000 yid_langchain_extensions-0.4.8/yid_langchain_extensions/output_parser/direct_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-18 07:29:44.000000 yid_langchain_extensions-0.4.8/yid_langchain_extensions/output_parser/thoughts_json_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:30:03.365272 yid_langchain_extensions-0.4.8/yid_langchain_extensions/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 07:29:44.000000 yid_langchain_extensions-0.4.8/yid_langchain_extensions/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-18 07:29:44.000000 yid_langchain_extensions-0.4.8/yid_langchain_extensions/tools/agent_as_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-18 07:29:44.000000 yid_langchain_extensions-0.4.8/yid_langchain_extensions/tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:30:03.365272 yid_langchain_extensions-0.4.8/yid_langchain_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-18 07:30:03.000000 yid_langchain_extensions-0.4.8/yid_langchain_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-18 07:30:03.000000 yid_langchain_extensions-0.4.8/yid_langchain_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 07:30:03.000000 yid_langchain_extensions-0.4.8/yid_langchain_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-18 07:30:03.000000 yid_langchain_extensions-0.4.8/yid_langchain_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-18 07:30:03.000000 yid_langchain_extensions-0.4.8/yid_langchain_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:07:33.411548 yid_langchain_extensions-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-18 08:07:09.000000 yid_langchain_extensions-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-18 08:07:33.411548 yid_langchain_extensions-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-18 08:07:09.000000 yid_langchain_extensions-0.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 08:07:33.411548 yid_langchain_extensions-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-18 08:07:09.000000 yid_langchain_extensions-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:07:33.411548 yid_langchain_extensions-0.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 08:07:09.000000 yid_langchain_extensions-0.4.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-06-18 08:07:09.000000 yid_langchain_extensions-0.4.9/tests/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:07:33.411548 yid_langchain_extensions-0.4.9/yid_langchain_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 08:07:09.000000 yid_langchain_extensions-0.4.9/yid_langchain_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:07:33.411548 yid_langchain_extensions-0.4.9/yid_langchain_extensions/output_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 08:07:09.000000 yid_langchain_extensions-0.4.9/yid_langchain_extensions/output_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-18 08:07:09.000000 yid_langchain_extensions-0.4.9/yid_langchain_extensions/output_parser/action_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-18 08:07:09.000000 yid_langchain_extensions-0.4.9/yid_langchain_extensions/output_parser/class_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-18 08:07:09.000000 yid_langchain_extensions-0.4.9/yid_langchain_extensions/output_parser/direct_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-18 08:07:09.000000 yid_langchain_extensions-0.4.9/yid_langchain_extensions/output_parser/thoughts_json_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:07:33.411548 yid_langchain_extensions-0.4.9/yid_langchain_extensions/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 08:07:09.000000 yid_langchain_extensions-0.4.9/yid_langchain_extensions/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-18 08:07:09.000000 yid_langchain_extensions-0.4.9/yid_langchain_extensions/tools/agent_as_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-18 08:07:09.000000 yid_langchain_extensions-0.4.9/yid_langchain_extensions/tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:07:33.411548 yid_langchain_extensions-0.4.9/yid_langchain_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-18 08:07:33.000000 yid_langchain_extensions-0.4.9/yid_langchain_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-18 08:07:33.000000 yid_langchain_extensions-0.4.9/yid_langchain_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 08:07:33.000000 yid_langchain_extensions-0.4.9/yid_langchain_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-18 08:07:33.000000 yid_langchain_extensions-0.4.9/yid_langchain_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-18 08:07:33.000000 yid_langchain_extensions-0.4.9/yid_langchain_extensions.egg-info/top_level.txt
```

### Comparing `yid_langchain_extensions-0.4.8/LICENSE` & `yid_langchain_extensions-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yid_langchain_extensions-0.4.8/PKG-INFO` & `yid_langchain_extensions-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yid_langchain_extensions
-Version: 0.4.8
+Version: 0.4.9
 Summary: Useful classes extending langchain library
 Home-page: https://github.com/dimitree54/yid_langchain_extensions
 Author: Dmitrii Rashchenko
 Author-email: dimitree54@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yid_langchain_extensions-0.4.8/setup.py` & `yid_langchain_extensions-0.4.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='yid_langchain_extensions',
-    version='0.4.8',
+    version='0.4.9',
     author='Dmitrii Rashchenko',
     author_email='dimitree54@gmail.com',
     packages=find_packages(),
     description='Useful classes extending langchain library',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/dimitree54/yid_langchain_extensions',
```

### Comparing `yid_langchain_extensions-0.4.8/tests/test_parser.py` & `yid_langchain_extensions-0.4.9/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `yid_langchain_extensions-0.4.8/yid_langchain_extensions/output_parser/action_parser.py` & `yid_langchain_extensions-0.4.9/yid_langchain_extensions/output_parser/action_parser.py`

 * *Files identical despite different names*

### Comparing `yid_langchain_extensions-0.4.8/yid_langchain_extensions/output_parser/class_parser.py` & `yid_langchain_extensions-0.4.9/yid_langchain_extensions/output_parser/class_parser.py`

 * *Files identical despite different names*

### Comparing `yid_langchain_extensions-0.4.8/yid_langchain_extensions/tools/agent_as_tool.py` & `yid_langchain_extensions-0.4.9/yid_langchain_extensions/tools/agent_as_tool.py`

 * *Files identical despite different names*

### Comparing `yid_langchain_extensions-0.4.8/yid_langchain_extensions.egg-info/PKG-INFO` & `yid_langchain_extensions-0.4.9/yid_langchain_extensions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yid-langchain-extensions
-Version: 0.4.8
+Version: 0.4.9
 Summary: Useful classes extending langchain library
 Home-page: https://github.com/dimitree54/yid_langchain_extensions
 Author: Dmitrii Rashchenko
 Author-email: dimitree54@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yid_langchain_extensions-0.4.8/yid_langchain_extensions.egg-info/SOURCES.txt` & `yid_langchain_extensions-0.4.9/yid_langchain_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

