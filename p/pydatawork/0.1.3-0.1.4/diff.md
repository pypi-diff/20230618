# Comparing `tmp/pydatawork-0.1.3.tar.gz` & `tmp/pydatawork-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.1.3.tar", last modified: Sun Jun 18 14:49:09 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.1.4.tar", last modified: Sun Jun 18 15:04:16 2023, max compression
```

## Comparing `pydatawork-0.1.3.tar` & `pydatawork-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 14:49:09.000000 pydatawork-0.1.3/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     3158 2023-06-18 14:49:09.000000 pydatawork-0.1.3/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     2026 2023-06-18 14:48:26.000000 pydatawork-0.1.3/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 14:49:09.000000 pydatawork-0.1.3/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     3158 2023-06-18 14:49:09.000000 pydatawork-0.1.3/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-18 14:49:09.000000 pydatawork-0.1.3/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-18 14:49:09.000000 pydatawork-0.1.3/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-18 14:49:09.000000 pydatawork-0.1.3/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     9884 2023-06-18 14:43:00.000000 pydatawork-0.1.3/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-18 14:49:09.000000 pydatawork-0.1.3/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-18 14:45:17.000000 pydatawork-0.1.3/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 15:04:16.000000 pydatawork-0.1.4/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     3158 2023-06-18 15:04:16.000000 pydatawork-0.1.4/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     2026 2023-06-18 15:03:33.000000 pydatawork-0.1.4/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 15:04:16.000000 pydatawork-0.1.4/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     3158 2023-06-18 15:04:16.000000 pydatawork-0.1.4/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-18 15:04:16.000000 pydatawork-0.1.4/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-18 15:04:16.000000 pydatawork-0.1.4/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-18 15:04:16.000000 pydatawork-0.1.4/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    10131 2023-06-18 15:02:04.000000 pydatawork-0.1.4/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-18 15:04:16.000000 pydatawork-0.1.4/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-18 15:03:07.000000 pydatawork-0.1.4/setup.py
```

### Comparing `pydatawork-0.1.3/PKG-INFO` & `pydatawork-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.1.3
+Version: 0.1.4
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         
         
         ###### Sun Jun 18 22:37:01 CST 2023
         
-        #### rename_numeric_serialize() 文件夹从左到右比较，按数值从小到大排序，再从1开始进行序列化重命名（v 0.1.3）
+        #### rename_numeric_serialize() 文件夹从左到右比较，按数值从小到大排序，再从1开始进行序列化重命名（v 0.1.4）
         
         ```python
         def rename_numeric_serialize(path):
             """
             path:文件夹路径。给定一个文件夹路径，获取其中子文件夹的名字，根据子文件夹的名字，从左到右进行比较，按数值从小到大对子文件夹排序，再从1开始对子文件夹进行序列化重命名。
             """
         ```
```

### Comparing `pydatawork-0.1.3/README.md` & `pydatawork-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 
 
 ###### Sun Jun 18 22:37:01 CST 2023
 
-#### rename_numeric_serialize() 文件夹从左到右比较，按数值从小到大排序，再从1开始进行序列化重命名（v 0.1.3）
+#### rename_numeric_serialize() 文件夹从左到右比较，按数值从小到大排序，再从1开始进行序列化重命名（v 0.1.4）
 
 ```python
 def rename_numeric_serialize(path):
     """
     path:文件夹路径。给定一个文件夹路径，获取其中子文件夹的名字，根据子文件夹的名字，从左到右进行比较，按数值从小到大对子文件夹排序，再从1开始对子文件夹进行序列化重命名。
     """
 ```
```

### Comparing `pydatawork-0.1.3/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.1.4/pydatawork.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.1.3
+Version: 0.1.4
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         
         
         ###### Sun Jun 18 22:37:01 CST 2023
         
-        #### rename_numeric_serialize() 文件夹从左到右比较，按数值从小到大排序，再从1开始进行序列化重命名（v 0.1.3）
+        #### rename_numeric_serialize() 文件夹从左到右比较，按数值从小到大排序，再从1开始进行序列化重命名（v 0.1.4）
         
         ```python
         def rename_numeric_serialize(path):
             """
             path:文件夹路径。给定一个文件夹路径，获取其中子文件夹的名字，根据子文件夹的名字，从左到右进行比较，按数值从小到大对子文件夹排序，再从1开始对子文件夹进行序列化重命名。
             """
         ```
```

### Comparing `pydatawork-0.1.3/pydatawork.py` & `pydatawork-0.1.4/pydatawork.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,49 +3,49 @@
 import urllib.request
 import json
 import requests
 import os
 
 
 
-def break_words(stuff):
-    """This function will break up words for us."""
-    words = stuff.split(' ')
-    return words
-
-def sort_words(words):
-    """Sorts the words.""" # 文档字符串，是注释的一种
-    return sorted(words)
-
-def print_first_word(words):
-    """Prints the first word after popping it off."""
-    word = words.pop(0)
-    print(word)
-
-def print_last_word(words):
-    """Print the last word after popping it off."""
-    word = words.pop(-1)
-    print(word)
-
-def sort_sentence(sentence):
-    """Takes in a full sentence and returns the sorted words"""
-    words = break_words(sentence)
-    return sort_words(words)  # 没懂这个函数
-
-def print_first_and_last(sentence):
-    """Prints the first and last words of the sentence."""
-    words = break_words(sentence)
-    print_first_word(words)
-    print_last_word(words)
-
-def print_first_and_last_sorted(sentence):
-    """Sorts the words then prints the first and last one."""
-    words = sort_sentence(sentence)
-    print_first_word(words)
-    print_last_word(words)
+# def break_words(stuff):
+#     """This function will break up words for us."""
+#     words = stuff.split(' ')
+#     return words
+
+# def sort_words(words):
+#     """Sorts the words.""" # 文档字符串，是注释的一种
+#     return sorted(words)
+
+# def print_first_word(words):
+#     """Prints the first word after popping it off."""
+#     word = words.pop(0)
+#     print(word)
+
+# def print_last_word(words):
+#     """Print the last word after popping it off."""
+#     word = words.pop(-1)
+#     print(word)
+
+# def sort_sentence(sentence):
+#     """Takes in a full sentence and returns the sorted words"""
+#     words = break_words(sentence)
+#     return sort_words(words)  # 没懂这个函数
+
+# def print_first_and_last(sentence):
+#     """Prints the first and last words of the sentence."""
+#     words = break_words(sentence)
+#     print_first_word(words)
+#     print_last_word(words)
+
+# def print_first_and_last_sorted(sentence):
+#     """Sorts the words then prints the first and last one."""
+#     words = sort_sentence(sentence)
+#     print_first_word(words)
+#     print_last_word(words)
     
 
 def get_weibo(path,id,weibo_name):
     """
     path: 内容存放路径
     id: 微博id
     weibo_name: 内容存放路径下文件夹的名字
@@ -169,15 +169,15 @@
 
     get_userInfo(id)
     get_weibo(id, file)
     print("微博数据获取完毕")
 
 
 
-def rename_numeric_serialize(path):
+def rename_folder_numeric_serialize(path):
     """
     path:文件夹路径。给定一个文件夹路径，获取其中子文件夹的名字，根据子文件夹的名字，从左到右进行比较，按数值从小到大对子文件夹排序，再从1开始对子文件夹进行序列化重命名。
     """
 
     # 定义一个函数，将输入的字符串按照数字和非数字的部分进行分割，并将数字部分转换为整数
     def split_key(s): # 【一个字符串一个字符串处理】
         parts = [] # 初始化一个空列表，用于存储分割后的字符串
@@ -202,18 +202,18 @@
         
     # 定义文件夹路径
     images_path = path
 
     # 获取images_path下的所有子文件夹
     subfolders = [f.path for f in os.scandir(images_path) if f.is_dir()]
 
-    # 对子文件夹按名字进行递增排序
+    # 对子文件夹按名字进行递增排序 @ 知识卡片 键函数。把subfolders中的每个元素，传给split_key按规则进行处理，并返回一个键，按返回的键进行排序。
     subfolders.sort(key=split_key)
 
     # 对排序后的子文件夹从1开始序列化，序列化的值加在原文件名末尾，以_进行拼接
-    for i, folder in enumerate(subfolders, start=1): # 遍历排序后的子文件夹，从1开始序列化
+    for i, folder in enumerate(subfolders, start=1): # 遍历排序后的子文件夹，从1开始序列化 @ 知识卡片
         new_name = f"{folder}_{i}" # 将序列化的值加在原文件名末尾，以_进行拼接
-        os.rename(folder, new_name) # 重命名文件夹
+        os.rename(folder, new_name) # 重命名文件夹 @ 知识卡片
         print(os.path.basename(new_name)) # 打印重命名后的文件夹名字，不包括路径
```

### Comparing `pydatawork-0.1.3/setup.py` & `pydatawork-0.1.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.1.3',
+    version='0.1.4',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

