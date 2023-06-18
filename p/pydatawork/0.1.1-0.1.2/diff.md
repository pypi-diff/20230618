# Comparing `tmp/pydatawork-0.1.1.tar.gz` & `tmp/pydatawork-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.1.1.tar", last modified: Sun Jun 18 11:13:15 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.1.2.tar", last modified: Sun Jun 18 11:24:34 2023, max compression
```

## Comparing `pydatawork-0.1.1.tar` & `pydatawork-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 11:13:15.000000 pydatawork-0.1.1/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     2583 2023-06-18 11:13:15.000000 pydatawork-0.1.1/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1523 2023-06-18 11:11:46.000000 pydatawork-0.1.1/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 11:13:15.000000 pydatawork-0.1.1/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     2583 2023-06-18 11:13:15.000000 pydatawork-0.1.1/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-18 11:13:15.000000 pydatawork-0.1.1/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-18 11:13:15.000000 pydatawork-0.1.1/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-18 11:13:15.000000 pydatawork-0.1.1/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     7403 2023-06-18 10:53:27.000000 pydatawork-0.1.1/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-18 11:13:15.000000 pydatawork-0.1.1/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-18 11:13:00.000000 pydatawork-0.1.1/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 11:24:34.000000 pydatawork-0.1.2/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     2583 2023-06-18 11:24:34.000000 pydatawork-0.1.2/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1523 2023-06-18 11:23:40.000000 pydatawork-0.1.2/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 11:24:34.000000 pydatawork-0.1.2/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     2583 2023-06-18 11:24:34.000000 pydatawork-0.1.2/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-18 11:24:34.000000 pydatawork-0.1.2/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-18 11:24:34.000000 pydatawork-0.1.2/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-18 11:24:34.000000 pydatawork-0.1.2/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     7399 2023-06-18 11:22:38.000000 pydatawork-0.1.2/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-18 11:24:34.000000 pydatawork-0.1.2/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-18 11:23:53.000000 pydatawork-0.1.2/setup.py
```

### Comparing `pydatawork-0.1.1/PKG-INFO` & `pydatawork-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.1.1
+Version: 0.1.2
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         
         
         ###### Sun Jun 18 17:10:46 CST 2023
         
-        #### get_weibo() 微博图片获取（v 0.1.1）
+        #### get_weibo() 微博图片获取（v 0.1.2）
         
         ```shell
         get_weibo(path,id,weibo_name)
         ```
+        
         参数说明：
         ```shell
         path: 内容存放路径；
         id: 微博id；
         weibo_name: 内容存放路径下文件夹的名字。
         ```
         
-        
         示例：获取梅西的微博id，获取其微博内容
         
         ```python
         import pydatawork as dw 
         
         path="/home/Desktop/pydatawork"
-        id="3543420821" # 梅西的微博id。在网页版上能获得链接，链接中u后面的内容即为id ,梅西微博的id为 3543420821  https://weibo.com/u/3543420821
+        id="5934019851" # 梅西的微博id。在网页版上能获得链接，链接中u后面的内容即为id ,梅西微博的id为 5934019851  https://weibo.com/u/5934019851
         weibo_name="mx"
         
         dw.get_weibo(path,id,weibo_name)
         ```
         
         #### pypi维护指令
```

### Comparing `pydatawork-0.1.1/README.md` & `pydatawork-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 
 
 
 ###### Sun Jun 18 17:10:46 CST 2023
 
-#### get_weibo() 微博图片获取（v 0.1.1）
+#### get_weibo() 微博图片获取（v 0.1.2）
 
 ```shell
 get_weibo(path,id,weibo_name)
 ```
+
 参数说明：
 ```shell
 path: 内容存放路径；
 id: 微博id；
 weibo_name: 内容存放路径下文件夹的名字。
 ```
 
-
 示例：获取梅西的微博id，获取其微博内容
 
 ```python
 import pydatawork as dw 
 
 path="/home/Desktop/pydatawork"
-id="3543420821" # 梅西的微博id。在网页版上能获得链接，链接中u后面的内容即为id ,梅西微博的id为 3543420821  https://weibo.com/u/3543420821
+id="5934019851" # 梅西的微博id。在网页版上能获得链接，链接中u后面的内容即为id ,梅西微博的id为 5934019851  https://weibo.com/u/5934019851
 weibo_name="mx"
 
 dw.get_weibo(path,id,weibo_name)
 ```
 
 #### pypi维护指令
```

### Comparing `pydatawork-0.1.1/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.1.2/pydatawork.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.1.1
+Version: 0.1.2
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         
         
         ###### Sun Jun 18 17:10:46 CST 2023
         
-        #### get_weibo() 微博图片获取（v 0.1.1）
+        #### get_weibo() 微博图片获取（v 0.1.2）
         
         ```shell
         get_weibo(path,id,weibo_name)
         ```
+        
         参数说明：
         ```shell
         path: 内容存放路径；
         id: 微博id；
         weibo_name: 内容存放路径下文件夹的名字。
         ```
         
-        
         示例：获取梅西的微博id，获取其微博内容
         
         ```python
         import pydatawork as dw 
         
         path="/home/Desktop/pydatawork"
-        id="3543420821" # 梅西的微博id。在网页版上能获得链接，链接中u后面的内容即为id ,梅西微博的id为 3543420821  https://weibo.com/u/3543420821
+        id="5934019851" # 梅西的微博id。在网页版上能获得链接，链接中u后面的内容即为id ,梅西微博的id为 5934019851  https://weibo.com/u/5934019851
         weibo_name="mx"
         
         dw.get_weibo(path,id,weibo_name)
         ```
         
         #### pypi维护指令
```

### Comparing `pydatawork-0.1.1/pydatawork.py` & `pydatawork-0.1.2/pydatawork.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,19 +47,19 @@
 def get_weibo(path,id,weibo_name):
     """
     path: 内容存放路径
     id: 微博id
     weibo_name: 内容存放路径下文件夹的名字
 
     示例：获取梅西的微博id，获取其微博内容
-    
+
     import pydatawork as dw 
 
     path="/home/Desktop/pydatawork"
-    id="3543420821" # 梅西的微博id。在网页版上能获得链接，链接中u后面的内容即为id ,梅西微博的id为 3543420821  https://weibo.com/u/3543420821
+    id="5934019851" # 梅西的微博id。在网页版上能获得链接，链接中u后面的内容即为id ,梅西微博的id为 5934019851  https://weibo.com/u/5934019851
     weibo_name="mx"
 
     dw.get_weibo(path,id,weibo_name)
 
     """
     path = path
     id = id # 在微博上获取
```

### Comparing `pydatawork-0.1.1/setup.py` & `pydatawork-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.1.1',
+    version='0.1.2',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

