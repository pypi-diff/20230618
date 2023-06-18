# Comparing `tmp/pydatawork-0.1.4.tar.gz` & `tmp/pydatawork-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.1.4.tar", last modified: Sun Jun 18 15:04:16 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.1.5.tar", last modified: Sun Jun 18 15:22:46 2023, max compression
```

## Comparing `pydatawork-0.1.4.tar` & `pydatawork-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 15:04:16.000000 pydatawork-0.1.4/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     3158 2023-06-18 15:04:16.000000 pydatawork-0.1.4/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     2026 2023-06-18 15:03:33.000000 pydatawork-0.1.4/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 15:04:16.000000 pydatawork-0.1.4/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     3158 2023-06-18 15:04:16.000000 pydatawork-0.1.4/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-18 15:04:16.000000 pydatawork-0.1.4/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-18 15:04:16.000000 pydatawork-0.1.4/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-18 15:04:16.000000 pydatawork-0.1.4/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    10131 2023-06-18 15:02:04.000000 pydatawork-0.1.4/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-18 15:04:16.000000 pydatawork-0.1.4/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-18 15:03:07.000000 pydatawork-0.1.4/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 15:22:46.000000 pydatawork-0.1.5/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     3172 2023-06-18 15:22:46.000000 pydatawork-0.1.5/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     2040 2023-06-18 15:21:45.000000 pydatawork-0.1.5/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 15:22:46.000000 pydatawork-0.1.5/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     3172 2023-06-18 15:22:46.000000 pydatawork-0.1.5/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-18 15:22:46.000000 pydatawork-0.1.5/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-18 15:22:46.000000 pydatawork-0.1.5/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-18 15:22:46.000000 pydatawork-0.1.5/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    10131 2023-06-18 15:02:04.000000 pydatawork-0.1.5/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-18 15:22:46.000000 pydatawork-0.1.5/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-18 15:22:13.000000 pydatawork-0.1.5/setup.py
```

### Comparing `pydatawork-0.1.4/PKG-INFO` & `pydatawork-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.1.4
+Version: 0.1.5
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         
         
         ###### Sun Jun 18 22:37:01 CST 2023
         
-        #### rename_numeric_serialize() 文件夹从左到右比较，按数值从小到大排序，再从1开始进行序列化重命名（v 0.1.4）
+        #### rename_folder_numeric_serialize() 文件夹从左到右比较，按数值从小到大排序，再从1开始进行序列化重命名（v 0.1.4）
         
         ```python
-        def rename_numeric_serialize(path):
+        def rename_folder_numeric_serialize(path):
             """
             path:文件夹路径。给定一个文件夹路径，获取其中子文件夹的名字，根据子文件夹的名字，从左到右进行比较，按数值从小到大对子文件夹排序，再从1开始对子文件夹进行序列化重命名。
             """
         ```
         
         ###### Sun Jun 18 17:10:46 CST 2023
```

### Comparing `pydatawork-0.1.4/README.md` & `pydatawork-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
 
 
 ###### Sun Jun 18 22:37:01 CST 2023
 
-#### rename_numeric_serialize() 文件夹从左到右比较，按数值从小到大排序，再从1开始进行序列化重命名（v 0.1.4）
+#### rename_folder_numeric_serialize() 文件夹从左到右比较，按数值从小到大排序，再从1开始进行序列化重命名（v 0.1.4）
 
 ```python
-def rename_numeric_serialize(path):
+def rename_folder_numeric_serialize(path):
     """
     path:文件夹路径。给定一个文件夹路径，获取其中子文件夹的名字，根据子文件夹的名字，从左到右进行比较，按数值从小到大对子文件夹排序，再从1开始对子文件夹进行序列化重命名。
     """
 ```
 
 ###### Sun Jun 18 17:10:46 CST 2023
```

### Comparing `pydatawork-0.1.4/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.1.5/pydatawork.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.1.4
+Version: 0.1.5
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         
         
         ###### Sun Jun 18 22:37:01 CST 2023
         
-        #### rename_numeric_serialize() 文件夹从左到右比较，按数值从小到大排序，再从1开始进行序列化重命名（v 0.1.4）
+        #### rename_folder_numeric_serialize() 文件夹从左到右比较，按数值从小到大排序，再从1开始进行序列化重命名（v 0.1.4）
         
         ```python
-        def rename_numeric_serialize(path):
+        def rename_folder_numeric_serialize(path):
             """
             path:文件夹路径。给定一个文件夹路径，获取其中子文件夹的名字，根据子文件夹的名字，从左到右进行比较，按数值从小到大对子文件夹排序，再从1开始对子文件夹进行序列化重命名。
             """
         ```
         
         ###### Sun Jun 18 17:10:46 CST 2023
```

### Comparing `pydatawork-0.1.4/pydatawork.py` & `pydatawork-0.1.5/pydatawork.py`

 * *Files identical despite different names*

### Comparing `pydatawork-0.1.4/setup.py` & `pydatawork-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.1.4',
+    version='0.1.5',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

