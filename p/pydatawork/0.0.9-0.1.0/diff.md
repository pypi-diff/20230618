# Comparing `tmp/pydatawork-0.0.9.tar.gz` & `tmp/pydatawork-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.0.9.tar", last modified: Sun Jun 18 09:50:57 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.1.0.tar", last modified: Sun Jun 18 11:00:14 2023, max compression
```

## Comparing `pydatawork-0.0.9.tar` & `pydatawork-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 09:50:57.000000 pydatawork-0.0.9/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1699 2023-06-18 09:50:57.000000 pydatawork-0.0.9/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      855 2023-06-18 09:13:53.000000 pydatawork-0.0.9/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 09:50:57.000000 pydatawork-0.0.9/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1699 2023-06-18 09:50:57.000000 pydatawork-0.0.9/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-18 09:50:57.000000 pydatawork-0.0.9/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-18 09:50:57.000000 pydatawork-0.0.9/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-18 09:50:57.000000 pydatawork-0.0.9/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     7028 2023-06-18 09:50:17.000000 pydatawork-0.0.9/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-18 09:50:57.000000 pydatawork-0.0.9/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-18 09:50:35.000000 pydatawork-0.0.9/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 11:00:14.000000 pydatawork-0.1.0/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     2322 2023-06-18 11:00:14.000000 pydatawork-0.1.0/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1318 2023-06-18 10:59:25.000000 pydatawork-0.1.0/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 11:00:14.000000 pydatawork-0.1.0/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     2322 2023-06-18 11:00:14.000000 pydatawork-0.1.0/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-18 11:00:14.000000 pydatawork-0.1.0/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-18 11:00:14.000000 pydatawork-0.1.0/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-18 11:00:14.000000 pydatawork-0.1.0/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     7403 2023-06-18 10:53:27.000000 pydatawork-0.1.0/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-18 11:00:14.000000 pydatawork-0.1.0/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-18 10:59:42.000000 pydatawork-0.1.0/setup.py
```

### Comparing `pydatawork-0.0.9/README.md` & `pydatawork-0.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,51 @@
 
 
 
 ###### Sun Jun 18 17:10:46 CST 2023
-v0.0.7：添加了get_weibo()
 
+#### get_weibo() 微博图片获取（v 0.1.0）
+
+```shell
 get_weibo(path,id,weibo_name)
-path:输入存放路径；
-id:微博id；
-weibi_name:存放文件夹的名字。
+```
+参数说明：
+path: 内容存放路径
+id: 微博id
+weibo_name: 内容存放路径下文件夹的名字
+
+
+示例：获取梅西的微博id，获取其微博内容
 
+```python
+import pydatawork as dw 
 
-pypi维护指令：
+path="/home/Desktop/pydatawork"
+id="3543420821" # 梅西的微博id。在网页版上能获得链接，链接中u后面的内容即为id ,梅西微博的id为 3543420821  https://weibo.com/u/3543420821
+weibo_name="mx"
+
+dw.get_weibo(path,id,weibo_name)
+```
+
+#### pypi维护指令
 
 ```shell
 cd 到pydatawork文件夹
 python3 setup.py sdist bdist_wheel # 打包
 twine check dist/* # 检查
 twine upload dist/* # 上传，需要输入帐号密码
 
 ```
 
 
 ###### Sat Jun 17 18:23:38 CST 2023
 要升级使用最新的安装包，比较稳定可靠的一种方式是，先卸载旧的，再重装。
 
+#### pydatawork升级方法
+
 卸载：
 ```shell
 pip3 uninstall pydatawork
 ```
 
 安装：
 ```shell
@@ -39,13 +57,15 @@
 ```shell
 import pydatawork
 ```
 
 ###### Thu Jun 15 13:23:43 CST 2023
 数据工作相关的分享。
 
+#### pydatawork安装
+
 安装：
 ```shell
 pip3 install pydatawork
 ```
```

### Comparing `pydatawork-0.0.9/pydatawork.py` & `pydatawork-0.1.0/pydatawork.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,17 +42,28 @@
     words = sort_sentence(sentence)
     print_first_word(words)
     print_last_word(words)
     
 
 def get_weibo(path,id,weibo_name):
     """
-    path:输入存放路径；
-    id:微博id；
-    weibi_name:存放文件夹的名字。
+    path: 内容存放路径
+    id: 微博id
+    weibo_name: 内容存放路径下文件夹的名字
+
+    示例：获取梅西的微博id，获取其微博内容
+    
+    import pydatawork as dw 
+
+    path="/home/Desktop/pydatawork"
+    id="3543420821" # 梅西的微博id。在网页版上能获得链接，链接中u后面的内容即为id ,梅西微博的id为 3543420821  https://weibo.com/u/3543420821
+    weibo_name="mx"
+
+    dw.get_weibo(path,id,weibo_name)
+
     """
     path = path
     id = id # 在微博上获取
 
     proxy_addr = "122.241.72.191:808"
     weibo_name = weibo_name # 可以自定义名字
```

### Comparing `pydatawork-0.0.9/setup.py` & `pydatawork-0.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.0.9',
+    version='0.1.0',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

