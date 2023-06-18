# Comparing `tmp/erniechatbotsdk-0.0.8.tar.gz` & `tmp/erniechatbotsdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erniechatbotsdk-0.0.8.tar", last modified: Sat Jun 17 16:24:01 2023, max compression
+gzip compressed data, was "erniechatbotsdk-0.0.9.tar", last modified: Sat Jun 17 16:29:25 2023, max compression
```

## Comparing `erniechatbotsdk-0.0.8.tar` & `erniechatbotsdk-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 16:24:01.677259 erniechatbotsdk-0.0.8/
--rw-r--r--   0 tk         (501) staff       (20)     1058 2023-06-17 11:06:14.000000 erniechatbotsdk-0.0.8/LICENSE
--rw-r--r--   0 tk         (501) staff       (20)     2167 2023-06-17 16:24:01.676398 erniechatbotsdk-0.0.8/PKG-INFO
--rw-r--r--   0 tk         (501) staff       (20)     1576 2023-06-17 16:08:12.000000 erniechatbotsdk-0.0.8/README.md
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 16:24:01.666574 erniechatbotsdk-0.0.8/erniebotchat/
--rw-r--r--   0 tk         (501) staff       (20)        0 2023-06-17 14:58:33.000000 erniechatbotsdk-0.0.8/erniebotchat/__init__.py
--rw-r--r--   0 tk         (501) staff       (20)      488 2023-06-17 16:20:59.000000 erniechatbotsdk-0.0.8/erniebotchat/erniebot.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 16:24:01.668544 erniechatbotsdk-0.0.8/erniebotchat/error/
--rw-r--r--   0 tk         (501) staff       (20)       36 2023-06-17 10:09:15.000000 erniechatbotsdk-0.0.8/erniebotchat/error/__init__.py
--rw-r--r--   0 tk         (501) staff       (20)      148 2023-06-17 10:04:03.000000 erniechatbotsdk-0.0.8/erniebotchat/error/customerror.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 16:24:01.670342 erniechatbotsdk-0.0.8/erniebotchat/service/
--rw-r--r--   0 tk         (501) staff       (20)       28 2023-06-17 04:04:37.000000 erniechatbotsdk-0.0.8/erniebotchat/service/__init__.py
--rw-r--r--   0 tk         (501) staff       (20)     2710 2023-06-17 16:21:57.000000 erniechatbotsdk-0.0.8/erniebotchat/service/explain.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 16:24:01.675268 erniechatbotsdk-0.0.8/erniechatbotsdk.egg-info/
--rw-r--r--   0 tk         (501) staff       (20)     2167 2023-06-17 16:24:01.000000 erniechatbotsdk-0.0.8/erniechatbotsdk.egg-info/PKG-INFO
--rw-r--r--   0 tk         (501) staff       (20)      400 2023-06-17 16:24:01.000000 erniechatbotsdk-0.0.8/erniechatbotsdk.egg-info/SOURCES.txt
--rw-r--r--   0 tk         (501) staff       (20)        1 2023-06-17 16:24:01.000000 erniechatbotsdk-0.0.8/erniechatbotsdk.egg-info/dependency_links.txt
--rw-r--r--   0 tk         (501) staff       (20)        8 2023-06-17 16:24:01.000000 erniechatbotsdk-0.0.8/erniechatbotsdk.egg-info/requires.txt
--rw-r--r--   0 tk         (501) staff       (20)       13 2023-06-17 16:24:01.000000 erniechatbotsdk-0.0.8/erniechatbotsdk.egg-info/top_level.txt
--rw-r--r--   0 tk         (501) staff       (20)       38 2023-06-17 16:24:01.677501 erniechatbotsdk-0.0.8/setup.cfg
--rw-r--r--   0 tk         (501) staff       (20)      979 2023-06-17 16:13:36.000000 erniechatbotsdk-0.0.8/setup.py
+drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 16:29:25.235597 erniechatbotsdk-0.0.9/
+-rw-r--r--   0 tk         (501) staff       (20)     1058 2023-06-17 11:06:14.000000 erniechatbotsdk-0.0.9/LICENSE
+-rw-r--r--   0 tk         (501) staff       (20)     2174 2023-06-17 16:29:25.234813 erniechatbotsdk-0.0.9/PKG-INFO
+-rw-r--r--   0 tk         (501) staff       (20)     1583 2023-06-17 16:26:25.000000 erniechatbotsdk-0.0.9/README.md
+drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 16:29:25.225820 erniechatbotsdk-0.0.9/erniebotchat/
+-rw-r--r--   0 tk         (501) staff       (20)        0 2023-06-17 14:58:33.000000 erniechatbotsdk-0.0.9/erniebotchat/__init__.py
+-rw-r--r--   0 tk         (501) staff       (20)      488 2023-06-17 16:20:59.000000 erniechatbotsdk-0.0.9/erniebotchat/erniebot.py
+drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 16:29:25.227412 erniechatbotsdk-0.0.9/erniebotchat/error/
+-rw-r--r--   0 tk         (501) staff       (20)       36 2023-06-17 10:09:15.000000 erniechatbotsdk-0.0.9/erniebotchat/error/__init__.py
+-rw-r--r--   0 tk         (501) staff       (20)      148 2023-06-17 10:04:03.000000 erniechatbotsdk-0.0.9/erniebotchat/error/customerror.py
+drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 16:29:25.229048 erniechatbotsdk-0.0.9/erniebotchat/service/
+-rw-r--r--   0 tk         (501) staff       (20)       28 2023-06-17 04:04:37.000000 erniechatbotsdk-0.0.9/erniebotchat/service/__init__.py
+-rw-r--r--   0 tk         (501) staff       (20)     2710 2023-06-17 16:21:57.000000 erniechatbotsdk-0.0.9/erniebotchat/service/explain.py
+drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 16:29:25.233880 erniechatbotsdk-0.0.9/erniechatbotsdk.egg-info/
+-rw-r--r--   0 tk         (501) staff       (20)     2174 2023-06-17 16:29:25.000000 erniechatbotsdk-0.0.9/erniechatbotsdk.egg-info/PKG-INFO
+-rw-r--r--   0 tk         (501) staff       (20)      400 2023-06-17 16:29:25.000000 erniechatbotsdk-0.0.9/erniechatbotsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 tk         (501) staff       (20)        1 2023-06-17 16:29:25.000000 erniechatbotsdk-0.0.9/erniechatbotsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 tk         (501) staff       (20)        8 2023-06-17 16:29:25.000000 erniechatbotsdk-0.0.9/erniechatbotsdk.egg-info/requires.txt
+-rw-r--r--   0 tk         (501) staff       (20)       13 2023-06-17 16:29:25.000000 erniechatbotsdk-0.0.9/erniechatbotsdk.egg-info/top_level.txt
+-rw-r--r--   0 tk         (501) staff       (20)       38 2023-06-17 16:29:25.235864 erniechatbotsdk-0.0.9/setup.cfg
+-rw-r--r--   0 tk         (501) staff       (20)      979 2023-06-17 16:26:50.000000 erniechatbotsdk-0.0.9/setup.py
```

### Comparing `erniechatbotsdk-0.0.8/LICENSE` & `erniechatbotsdk-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `erniechatbotsdk-0.0.8/PKG-INFO` & `erniechatbotsdk-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erniechatbotsdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: Baidu Wenxin word api package
 Author: Tk
 Author-email: tkzhu66@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -21,23 +21,21 @@
 ErnieBot-turbo请求地址： https://aip.baidubce.com/rpc/2.0/ai_custom/v1/wenxinworkshop/chat/eb-instant
 的简单封装
 
 # 安装
 使用pip进行安装
 ```
 pip install erniechatbotsdk
+```
 
 ## 请求示例
-```
+```python
 from erniebotchat.erniebot import Erniebot
 
-
 json_str='{"messages": [{"role": "user", "content": "介绍一下自已"},{"role":"assistant","content":"我是百度公司开发的人工智能语言模型，我的中文名是文心一言，英文名是ERNIE Bot，可以协助您完成范围广泛的任务并提供有关各种主题的信息，比如回答问题，提供定义和解释及建议。如果您有任何问题，请随时向我提问。"},{"role":"user","content": "我在上海，周末可以去哪里玩？"}]}'
-
-
 if __name__ == '__main__':
 
     enrniebot = Erniebot("apikey","secretkey")
     resp = enrniebot.chat(json_str,"erniebot")
     print(resp)
 
 ```
```

### Comparing `erniechatbotsdk-0.0.8/README.md` & `erniechatbotsdk-0.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,23 +4,21 @@
 ErnieBot-turbo请求地址： https://aip.baidubce.com/rpc/2.0/ai_custom/v1/wenxinworkshop/chat/eb-instant
 的简单封装
 
 # 安装
 使用pip进行安装
 ```
 pip install erniechatbotsdk
+```
 
 ## 请求示例
-```
+```python
 from erniebotchat.erniebot import Erniebot
 
-
 json_str='{"messages": [{"role": "user", "content": "介绍一下自已"},{"role":"assistant","content":"我是百度公司开发的人工智能语言模型，我的中文名是文心一言，英文名是ERNIE Bot，可以协助您完成范围广泛的任务并提供有关各种主题的信息，比如回答问题，提供定义和解释及建议。如果您有任何问题，请随时向我提问。"},{"role":"user","content": "我在上海，周末可以去哪里玩？"}]}'
-
-
 if __name__ == '__main__':
 
     enrniebot = Erniebot("apikey","secretkey")
     resp = enrniebot.chat(json_str,"erniebot")
     print(resp)
 
 ```
```

### Comparing `erniechatbotsdk-0.0.8/erniebotchat/service/explain.py` & `erniechatbotsdk-0.0.9/erniebotchat/service/explain.py`

 * *Files identical despite different names*

### Comparing `erniechatbotsdk-0.0.8/erniechatbotsdk.egg-info/PKG-INFO` & `erniechatbotsdk-0.0.9/erniechatbotsdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erniechatbotsdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: Baidu Wenxin word api package
 Author: Tk
 Author-email: tkzhu66@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -21,23 +21,21 @@
 ErnieBot-turbo请求地址： https://aip.baidubce.com/rpc/2.0/ai_custom/v1/wenxinworkshop/chat/eb-instant
 的简单封装
 
 # 安装
 使用pip进行安装
 ```
 pip install erniechatbotsdk
+```
 
 ## 请求示例
-```
+```python
 from erniebotchat.erniebot import Erniebot
 
-
 json_str='{"messages": [{"role": "user", "content": "介绍一下自已"},{"role":"assistant","content":"我是百度公司开发的人工智能语言模型，我的中文名是文心一言，英文名是ERNIE Bot，可以协助您完成范围广泛的任务并提供有关各种主题的信息，比如回答问题，提供定义和解释及建议。如果您有任何问题，请随时向我提问。"},{"role":"user","content": "我在上海，周末可以去哪里玩？"}]}'
-
-
 if __name__ == '__main__':
 
     enrniebot = Erniebot("apikey","secretkey")
     resp = enrniebot.chat(json_str,"erniebot")
     print(resp)
 
 ```
```

### Comparing `erniechatbotsdk-0.0.8/setup.py` & `erniechatbotsdk-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open(os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="erniechatbotsdk",
-    version="0.0.8",
+    version="0.0.9",
     description="Baidu Wenxin word api package",
     author="Tk",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="tkzhu66@gmail.com",
     #packages=find_packages(),
     package_data={
```

