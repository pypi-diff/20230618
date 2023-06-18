# Comparing `tmp/pydatawork-0.1.2.tar.gz` & `tmp/pydatawork-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.1.2.tar", last modified: Sun Jun 18 11:24:34 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.1.3.tar", last modified: Sun Jun 18 14:49:09 2023, max compression
```

## Comparing `pydatawork-0.1.2.tar` & `pydatawork-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 11:24:34.000000 pydatawork-0.1.2/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     2583 2023-06-18 11:24:34.000000 pydatawork-0.1.2/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1523 2023-06-18 11:23:40.000000 pydatawork-0.1.2/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 11:24:34.000000 pydatawork-0.1.2/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     2583 2023-06-18 11:24:34.000000 pydatawork-0.1.2/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-18 11:24:34.000000 pydatawork-0.1.2/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-18 11:24:34.000000 pydatawork-0.1.2/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-18 11:24:34.000000 pydatawork-0.1.2/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     7399 2023-06-18 11:22:38.000000 pydatawork-0.1.2/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-18 11:24:34.000000 pydatawork-0.1.2/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-18 11:23:53.000000 pydatawork-0.1.2/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 14:49:09.000000 pydatawork-0.1.3/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     3158 2023-06-18 14:49:09.000000 pydatawork-0.1.3/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     2026 2023-06-18 14:48:26.000000 pydatawork-0.1.3/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 14:49:09.000000 pydatawork-0.1.3/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     3158 2023-06-18 14:49:09.000000 pydatawork-0.1.3/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-18 14:49:09.000000 pydatawork-0.1.3/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-18 14:49:09.000000 pydatawork-0.1.3/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-18 14:49:09.000000 pydatawork-0.1.3/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     9884 2023-06-18 14:43:00.000000 pydatawork-0.1.3/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-18 14:49:09.000000 pydatawork-0.1.3/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-18 14:45:17.000000 pydatawork-0.1.3/setup.py
```

### Comparing `pydatawork-0.1.2/PKG-INFO` & `pydatawork-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.1.2
+Version: 0.1.3
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         
         
-        ###### Sun Jun 18 17:10:46 CST 2023
+        ###### Sun Jun 18 22:37:01 CST 2023
         
-        #### get_weibo() 微博图片获取（v 0.1.2）
+        #### rename_numeric_serialize() 文件夹从左到右比较，按数值从小到大排序，再从1开始进行序列化重命名（v 0.1.3）
         
-        ```shell
-        get_weibo(path,id,weibo_name)
+        ```python
+        def rename_numeric_serialize(path):
+            """
+            path:文件夹路径。给定一个文件夹路径，获取其中子文件夹的名字，根据子文件夹的名字，从左到右进行比较，按数值从小到大对子文件夹排序，再从1开始对子文件夹进行序列化重命名。
+            """
         ```
         
-        参数说明：
-        ```shell
-        path: 内容存放路径；
-        id: 微博id；
-        weibo_name: 内容存放路径下文件夹的名字。
+        ###### Sun Jun 18 17:10:46 CST 2023
+        
+        #### get_weibo() 微博图片获取（v 0.1.2）
+        
+        ```python
+        def get_weibo(path,id,weibo_name):
+            """
+            path: 内容存放路径；
+            id: 微博id；
+            weibo_name: 内容存放路径下文件夹的名字。
+            """
         ```
         
         示例：获取梅西的微博id，获取其微博内容
         
         ```python
         import pydatawork as dw
```

### Comparing `pydatawork-0.1.2/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.1.3/pydatawork.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.1.2
+Version: 0.1.3
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         
         
-        ###### Sun Jun 18 17:10:46 CST 2023
+        ###### Sun Jun 18 22:37:01 CST 2023
         
-        #### get_weibo() 微博图片获取（v 0.1.2）
+        #### rename_numeric_serialize() 文件夹从左到右比较，按数值从小到大排序，再从1开始进行序列化重命名（v 0.1.3）
         
-        ```shell
-        get_weibo(path,id,weibo_name)
+        ```python
+        def rename_numeric_serialize(path):
+            """
+            path:文件夹路径。给定一个文件夹路径，获取其中子文件夹的名字，根据子文件夹的名字，从左到右进行比较，按数值从小到大对子文件夹排序，再从1开始对子文件夹进行序列化重命名。
+            """
         ```
         
-        参数说明：
-        ```shell
-        path: 内容存放路径；
-        id: 微博id；
-        weibo_name: 内容存放路径下文件夹的名字。
+        ###### Sun Jun 18 17:10:46 CST 2023
+        
+        #### get_weibo() 微博图片获取（v 0.1.2）
+        
+        ```python
+        def get_weibo(path,id,weibo_name):
+            """
+            path: 内容存放路径；
+            id: 微博id；
+            weibo_name: 内容存放路径下文件夹的名字。
+            """
         ```
         
         示例：获取梅西的微博id，获取其微博内容
         
         ```python
         import pydatawork as dw
```

### Comparing `pydatawork-0.1.2/pydatawork.py` & `pydatawork-0.1.3/pydatawork.py`

 * *Files 24% similar despite different names*

```diff
@@ -167,7 +167,53 @@
         os.mkdir(os.path.join(path,weibo_name))
     file = os.path.join(path, weibo_name, weibo_name + ".txt")
 
     get_userInfo(id)
     get_weibo(id, file)
     print("微博数据获取完毕")
 
+
+
+def rename_numeric_serialize(path):
+    """
+    path:文件夹路径。给定一个文件夹路径，获取其中子文件夹的名字，根据子文件夹的名字，从左到右进行比较，按数值从小到大对子文件夹排序，再从1开始对子文件夹进行序列化重命名。
+    """
+
+    # 定义一个函数，将输入的字符串按照数字和非数字的部分进行分割，并将数字部分转换为整数
+    def split_key(s): # 【一个字符串一个字符串处理】
+        parts = [] # 初始化一个空列表，用于存储分割后的字符串
+        current_part = "" # 初始化一个空字符串，用于存储当前正在处理的部分
+        for c in s: # 遍历字符串中的每个字符
+            if c.isalnum(): # 如果当前字符是字母或数字
+                current_part += c # 将其添加到 current_part 变量中
+            else: # 如果当前字符是非字母和数字的符号
+                if current_part: # 如果 current_part 不为空
+                    if current_part.isdigit(): # 如果 current_part 是数字
+                        current_part = int(current_part) # 将其转换为整数
+                    parts.append(current_part) # 将 current_part 添加到 parts 列表中
+                    current_part = "" # 将 current_part 重置为空字符串
+        if current_part: # 如果 current_part 不为空
+            if current_part.isdigit(): # 如果 current_part 是数字
+                current_part = int(current_part) # 将其转换为整数
+            parts.append(current_part) # 将 current_part 添加到 parts 列表中
+            # print(parts)
+            # exit()
+        return parts # 返回分割后的字符串列表
+
+        
+    # 定义文件夹路径
+    images_path = path
+
+    # 获取images_path下的所有子文件夹
+    subfolders = [f.path for f in os.scandir(images_path) if f.is_dir()]
+
+    # 对子文件夹按名字进行递增排序
+    subfolders.sort(key=split_key)
+
+    # 对排序后的子文件夹从1开始序列化，序列化的值加在原文件名末尾，以_进行拼接
+    for i, folder in enumerate(subfolders, start=1): # 遍历排序后的子文件夹，从1开始序列化
+        new_name = f"{folder}_{i}" # 将序列化的值加在原文件名末尾，以_进行拼接
+        os.rename(folder, new_name) # 重命名文件夹
+        print(os.path.basename(new_name)) # 打印重命名后的文件夹名字，不包括路径
+
+
+
```

### Comparing `pydatawork-0.1.2/setup.py` & `pydatawork-0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.1.2',
+    version='0.1.3',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

