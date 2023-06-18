# Comparing `tmp/pydatawork-0.1.6.tar.gz` & `tmp/pydatawork-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.1.6.tar", last modified: Sun Jun 18 15:25:04 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.1.7.tar", last modified: Sun Jun 18 15:40:36 2023, max compression
```

## Comparing `pydatawork-0.1.6.tar` & `pydatawork-0.1.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 15:25:04.000000 pydatawork-0.1.6/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     3172 2023-06-18 15:25:04.000000 pydatawork-0.1.6/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     2040 2023-06-18 15:24:07.000000 pydatawork-0.1.6/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 15:25:04.000000 pydatawork-0.1.6/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     3172 2023-06-18 15:25:04.000000 pydatawork-0.1.6/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-18 15:25:04.000000 pydatawork-0.1.6/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-18 15:25:04.000000 pydatawork-0.1.6/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-18 15:25:04.000000 pydatawork-0.1.6/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    10131 2023-06-18 15:02:04.000000 pydatawork-0.1.6/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-18 15:25:04.000000 pydatawork-0.1.6/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-18 15:24:46.000000 pydatawork-0.1.6/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 15:40:36.000000 pydatawork-0.1.7/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     3503 2023-06-18 15:40:36.000000 pydatawork-0.1.7/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     2291 2023-06-18 15:38:44.000000 pydatawork-0.1.7/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 15:40:36.000000 pydatawork-0.1.7/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     3503 2023-06-18 15:40:36.000000 pydatawork-0.1.7/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-18 15:40:36.000000 pydatawork-0.1.7/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-18 15:40:36.000000 pydatawork-0.1.7/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-18 15:40:36.000000 pydatawork-0.1.7/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    10277 2023-06-18 15:34:02.000000 pydatawork-0.1.7/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-18 15:40:36.000000 pydatawork-0.1.7/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-18 15:38:52.000000 pydatawork-0.1.7/setup.py
```

### Comparing `pydatawork-0.1.6/PKG-INFO` & `pydatawork-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.1.6
+Version: 0.1.7
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         
         
+        ###### Sun Jun 18 23:34:45 CST 2023
+        
+        #### hello_jkzhou() Always grow together（v 0.1.7）
+        
+        ```python
+        def hello_jkzhou():
+            """If you need help or have a better idea, send me an e-mail."""
+            print("My e-mail is: zhouqiling.bjfu@foxmail.com")
+        ```
+        
         ###### Sun Jun 18 22:37:01 CST 2023
         
         #### rename_folder_numeric_serialize() 文件夹从左到右比较，按数值从小到大排序，再从1开始进行序列化重命名（v 0.1.6）
         
         ```python
         def rename_folder_numeric_serialize(path):
             """
```

### Comparing `pydatawork-0.1.6/README.md` & `pydatawork-0.1.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 
 
 
+###### Sun Jun 18 23:34:45 CST 2023
+
+#### hello_jkzhou() Always grow together（v 0.1.7）
+
+```python
+def hello_jkzhou():
+    """If you need help or have a better idea, send me an e-mail."""
+    print("My e-mail is: zhouqiling.bjfu@foxmail.com")
+```
+
 ###### Sun Jun 18 22:37:01 CST 2023
 
 #### rename_folder_numeric_serialize() 文件夹从左到右比较，按数值从小到大排序，再从1开始进行序列化重命名（v 0.1.6）
 
 ```python
 def rename_folder_numeric_serialize(path):
     """
```

### Comparing `pydatawork-0.1.6/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.1.7/pydatawork.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.1.6
+Version: 0.1.7
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         
         
+        ###### Sun Jun 18 23:34:45 CST 2023
+        
+        #### hello_jkzhou() Always grow together（v 0.1.7）
+        
+        ```python
+        def hello_jkzhou():
+            """If you need help or have a better idea, send me an e-mail."""
+            print("My e-mail is: zhouqiling.bjfu@foxmail.com")
+        ```
+        
         ###### Sun Jun 18 22:37:01 CST 2023
         
         #### rename_folder_numeric_serialize() 文件夹从左到右比较，按数值从小到大排序，再从1开始进行序列化重命名（v 0.1.6）
         
         ```python
         def rename_folder_numeric_serialize(path):
             """
```

### Comparing `pydatawork-0.1.6/pydatawork.py` & `pydatawork-0.1.7/pydatawork.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,19 @@
 #     print_last_word(words)
 
 # def print_first_and_last_sorted(sentence):
 #     """Sorts the words then prints the first and last one."""
 #     words = sort_sentence(sentence)
 #     print_first_word(words)
 #     print_last_word(words)
+
+
+def hello_jkzhou():
+    """If you need help or have a better idea, send me an e-mail."""
+    print("My e-mail is: zhouqiling.bjfu@foxmail.com")
     
 
 def get_weibo(path,id,weibo_name):
     """
     path: 内容存放路径
     id: 微博id
     weibo_name: 内容存放路径下文件夹的名字
```

### Comparing `pydatawork-0.1.6/setup.py` & `pydatawork-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.1.6',
+    version='0.1.7',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

