# Comparing `tmp/pydatawork-0.0.6.tar.gz` & `tmp/pydatawork-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.0.6.tar", last modified: Sat Jun 17 10:27:33 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.0.7.tar", last modified: Sun Jun 18 09:14:25 2023, max compression
```

## Comparing `pydatawork-0.0.6.tar` & `pydatawork-0.0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-17 10:27:33.000000 pydatawork-0.0.6/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1168 2023-06-17 10:27:33.000000 pydatawork-0.0.6/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      484 2023-06-17 10:26:09.000000 pydatawork-0.0.6/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-17 10:27:33.000000 pydatawork-0.0.6/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1168 2023-06-17 10:27:33.000000 pydatawork-0.0.6/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-17 10:27:33.000000 pydatawork-0.0.6/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-17 10:27:33.000000 pydatawork-0.0.6/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-17 10:27:33.000000 pydatawork-0.0.6/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1056 2023-06-17 10:13:17.000000 pydatawork-0.0.6/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-17 10:27:33.000000 pydatawork-0.0.6/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-17 10:27:03.000000 pydatawork-0.0.6/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 09:14:25.000000 pydatawork-0.0.7/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1699 2023-06-18 09:14:25.000000 pydatawork-0.0.7/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      855 2023-06-18 09:13:53.000000 pydatawork-0.0.7/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 09:14:25.000000 pydatawork-0.0.7/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1699 2023-06-18 09:14:25.000000 pydatawork-0.0.7/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-18 09:14:25.000000 pydatawork-0.0.7/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-18 09:14:25.000000 pydatawork-0.0.7/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-18 09:14:25.000000 pydatawork-0.0.7/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     7054 2023-06-18 09:09:22.000000 pydatawork-0.0.7/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-18 09:14:25.000000 pydatawork-0.0.7/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-18 09:10:31.000000 pydatawork-0.0.7/setup.py
```

### Comparing `pydatawork-0.0.6/PKG-INFO` & `pydatawork-0.0.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,38 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.0.6
+Version: 0.0.7
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         
         
+        ###### Sun Jun 18 17:10:46 CST 2023
+        v0.0.7：添加了get_weibo()
+        
+        get_weibo(path,id,weibo_name)
+        path:输入存放路径；
+        id:微博id；
+        weibi_name:存放文件夹的名字。
+        
+        
+        pypi维护指令：
+        
+        ```shell
+        cd 到pydatawork文件夹
+        python3 setup.py sdist bdist_wheel # 打包
+        twine check dist/* # 检查
+        twine upload dist/* # 上传，需要输入帐号密码
+        
+        ```
+        
+        
         ###### Sat Jun 17 18:23:38 CST 2023
         要升级使用最新的安装包，比较稳定可靠的一种方式是，先卸载旧的，再重装。
         
         卸载：
         ```shell
         pip3 uninstall pydatawork
         ```
```

### Comparing `pydatawork-0.0.6/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.0.7/pydatawork.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,38 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.0.6
+Version: 0.0.7
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         
         
+        ###### Sun Jun 18 17:10:46 CST 2023
+        v0.0.7：添加了get_weibo()
+        
+        get_weibo(path,id,weibo_name)
+        path:输入存放路径；
+        id:微博id；
+        weibi_name:存放文件夹的名字。
+        
+        
+        pypi维护指令：
+        
+        ```shell
+        cd 到pydatawork文件夹
+        python3 setup.py sdist bdist_wheel # 打包
+        twine check dist/* # 检查
+        twine upload dist/* # 上传，需要输入帐号密码
+        
+        ```
+        
+        
         ###### Sat Jun 17 18:23:38 CST 2023
         要升级使用最新的安装包，比较稳定可靠的一种方式是，先卸载旧的，再重装。
         
         卸载：
         ```shell
         pip3 uninstall pydatawork
         ```
```

### Comparing `pydatawork-0.0.6/setup.py` & `pydatawork-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.0.6',
+    version='0.0.7',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

