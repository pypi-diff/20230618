# Comparing `tmp/pydatawork-0.1.0.tar.gz` & `tmp/pydatawork-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.1.0.tar", last modified: Sun Jun 18 11:00:14 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.1.1.tar", last modified: Sun Jun 18 11:13:15 2023, max compression
```

## Comparing `pydatawork-0.1.0.tar` & `pydatawork-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 11:00:14.000000 pydatawork-0.1.0/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     2322 2023-06-18 11:00:14.000000 pydatawork-0.1.0/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1318 2023-06-18 10:59:25.000000 pydatawork-0.1.0/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 11:00:14.000000 pydatawork-0.1.0/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     2322 2023-06-18 11:00:14.000000 pydatawork-0.1.0/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-18 11:00:14.000000 pydatawork-0.1.0/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-18 11:00:14.000000 pydatawork-0.1.0/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-18 11:00:14.000000 pydatawork-0.1.0/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     7403 2023-06-18 10:53:27.000000 pydatawork-0.1.0/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-18 11:00:14.000000 pydatawork-0.1.0/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-18 10:59:42.000000 pydatawork-0.1.0/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 11:13:15.000000 pydatawork-0.1.1/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     2583 2023-06-18 11:13:15.000000 pydatawork-0.1.1/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1523 2023-06-18 11:11:46.000000 pydatawork-0.1.1/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 11:13:15.000000 pydatawork-0.1.1/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     2583 2023-06-18 11:13:15.000000 pydatawork-0.1.1/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-18 11:13:15.000000 pydatawork-0.1.1/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-18 11:13:15.000000 pydatawork-0.1.1/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-18 11:13:15.000000 pydatawork-0.1.1/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     7403 2023-06-18 10:53:27.000000 pydatawork-0.1.1/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-18 11:13:15.000000 pydatawork-0.1.1/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-18 11:13:00.000000 pydatawork-0.1.1/setup.py
```

### Comparing `pydatawork-0.1.0/PKG-INFO` & `pydatawork-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.1.0
+Version: 0.1.1
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         
         
         ###### Sun Jun 18 17:10:46 CST 2023
         
-        #### get_weibo() 微博图片获取（v 0.1.0）
+        #### get_weibo() 微博图片获取（v 0.1.1）
         
         ```shell
         get_weibo(path,id,weibo_name)
         ```
         参数说明：
-        path: 内容存放路径
-        id: 微博id
-        weibo_name: 内容存放路径下文件夹的名字
+        ```shell
+        path: 内容存放路径；
+        id: 微博id；
+        weibo_name: 内容存放路径下文件夹的名字。
+        ```
         
         
         示例：获取梅西的微博id，获取其微博内容
         
         ```python
         import pydatawork as dw 
         
@@ -40,46 +42,51 @@
         cd 到pydatawork文件夹
         python3 setup.py sdist bdist_wheel # 打包
         twine check dist/* # 检查
         twine upload dist/* # 上传，需要输入帐号密码
         
         ```
         
-        
         ###### Sat Jun 17 18:23:38 CST 2023
-        要升级使用最新的安装包，比较稳定可靠的一种方式是，先卸载旧的，再重装。
         
-        #### pydatawork升级方法
+        #### 查看pydatawork是否有更新
         
-        卸载：
         ```shell
-        pip3 uninstall pydatawork
+        pip3 list --outdated
         ```
         
-        安装：
+        #### pydatawork升级方法（先卸载，再安装）
+        
         ```shell
-        pip3 install pydatawork
+        pip3 uninstall pydatawork # 卸载
+        pip3 install pydatawork # 安装
         ```
         
         ###### Sat Jun 17 17:32:47 CST 2023
-        修改了导入方式，使用下面的导入方式：
+        #### pydatawork 导入方式
         ```shell
-        import pydatawork
+        import pydatawork # 标准导入方式
+        import pydatawork as dw # 推荐使用此方式，更简洁
         ```
         
         ###### Thu Jun 15 13:23:43 CST 2023
-        数据工作相关的分享。
         
         #### pydatawork安装
         
         安装：
         ```shell
         pip3 install pydatawork
         ```
         
+        #### 关于
+        数据工作相关的分享。
+        
+        推荐始终使用最新版。
+        
+        要升级使用最新的安装包，比较稳定可靠的一种方式是，先卸载旧的，再重装。
         
         
 Keywords: datawork
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pydatawork-0.1.0/README.md` & `pydatawork-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 
 
 
 ###### Sun Jun 18 17:10:46 CST 2023
 
-#### get_weibo() 微博图片获取（v 0.1.0）
+#### get_weibo() 微博图片获取（v 0.1.1）
 
 ```shell
 get_weibo(path,id,weibo_name)
 ```
 参数说明：
-path: 内容存放路径
-id: 微博id
-weibo_name: 内容存放路径下文件夹的名字
+```shell
+path: 内容存放路径；
+id: 微博id；
+weibo_name: 内容存放路径下文件夹的名字。
+```
 
 
 示例：获取梅西的微博id，获取其微博内容
 
 ```python
 import pydatawork as dw 
 
@@ -32,40 +34,45 @@
 cd 到pydatawork文件夹
 python3 setup.py sdist bdist_wheel # 打包
 twine check dist/* # 检查
 twine upload dist/* # 上传，需要输入帐号密码
 
 ```
 
-
 ###### Sat Jun 17 18:23:38 CST 2023
-要升级使用最新的安装包，比较稳定可靠的一种方式是，先卸载旧的，再重装。
 
-#### pydatawork升级方法
+#### 查看pydatawork是否有更新
 
-卸载：
 ```shell
-pip3 uninstall pydatawork
+pip3 list --outdated
 ```
 
-安装：
+#### pydatawork升级方法（先卸载，再安装）
+
 ```shell
-pip3 install pydatawork
+pip3 uninstall pydatawork # 卸载
+pip3 install pydatawork # 安装
 ```
 
 ###### Sat Jun 17 17:32:47 CST 2023
-修改了导入方式，使用下面的导入方式：
+#### pydatawork 导入方式
 ```shell
-import pydatawork
+import pydatawork # 标准导入方式
+import pydatawork as dw # 推荐使用此方式，更简洁
 ```
 
 ###### Thu Jun 15 13:23:43 CST 2023
-数据工作相关的分享。
 
 #### pydatawork安装
 
 安装：
 ```shell
 pip3 install pydatawork
 ```
 
+#### 关于
+数据工作相关的分享。
+
+推荐始终使用最新版。
+
+要升级使用最新的安装包，比较稳定可靠的一种方式是，先卸载旧的，再重装。
```

### Comparing `pydatawork-0.1.0/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.1.1/pydatawork.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.1.0
+Version: 0.1.1
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         
         
         ###### Sun Jun 18 17:10:46 CST 2023
         
-        #### get_weibo() 微博图片获取（v 0.1.0）
+        #### get_weibo() 微博图片获取（v 0.1.1）
         
         ```shell
         get_weibo(path,id,weibo_name)
         ```
         参数说明：
-        path: 内容存放路径
-        id: 微博id
-        weibo_name: 内容存放路径下文件夹的名字
+        ```shell
+        path: 内容存放路径；
+        id: 微博id；
+        weibo_name: 内容存放路径下文件夹的名字。
+        ```
         
         
         示例：获取梅西的微博id，获取其微博内容
         
         ```python
         import pydatawork as dw 
         
@@ -40,46 +42,51 @@
         cd 到pydatawork文件夹
         python3 setup.py sdist bdist_wheel # 打包
         twine check dist/* # 检查
         twine upload dist/* # 上传，需要输入帐号密码
         
         ```
         
-        
         ###### Sat Jun 17 18:23:38 CST 2023
-        要升级使用最新的安装包，比较稳定可靠的一种方式是，先卸载旧的，再重装。
         
-        #### pydatawork升级方法
+        #### 查看pydatawork是否有更新
         
-        卸载：
         ```shell
-        pip3 uninstall pydatawork
+        pip3 list --outdated
         ```
         
-        安装：
+        #### pydatawork升级方法（先卸载，再安装）
+        
         ```shell
-        pip3 install pydatawork
+        pip3 uninstall pydatawork # 卸载
+        pip3 install pydatawork # 安装
         ```
         
         ###### Sat Jun 17 17:32:47 CST 2023
-        修改了导入方式，使用下面的导入方式：
+        #### pydatawork 导入方式
         ```shell
-        import pydatawork
+        import pydatawork # 标准导入方式
+        import pydatawork as dw # 推荐使用此方式，更简洁
         ```
         
         ###### Thu Jun 15 13:23:43 CST 2023
-        数据工作相关的分享。
         
         #### pydatawork安装
         
         安装：
         ```shell
         pip3 install pydatawork
         ```
         
+        #### 关于
+        数据工作相关的分享。
+        
+        推荐始终使用最新版。
+        
+        要升级使用最新的安装包，比较稳定可靠的一种方式是，先卸载旧的，再重装。
         
         
 Keywords: datawork
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pydatawork-0.1.0/pydatawork.py` & `pydatawork-0.1.1/pydatawork.py`

 * *Files identical despite different names*

### Comparing `pydatawork-0.1.0/setup.py` & `pydatawork-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.1.0',
+    version='0.1.1',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

