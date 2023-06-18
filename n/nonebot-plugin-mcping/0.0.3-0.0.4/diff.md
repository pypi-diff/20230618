# Comparing `tmp/nonebot-plugin-mcping-0.0.3.tar.gz` & `tmp/nonebot-plugin-mcping-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-mcping-0.0.3.tar", last modified: Sun Jun 18 16:58:33 2023, max compression
+gzip compressed data, was "nonebot-plugin-mcping-0.0.4.tar", last modified: Sun Jun 18 16:58:45 2023, max compression
```

## Comparing `nonebot-plugin-mcping-0.0.3.tar` & `nonebot-plugin-mcping-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:58:33.199365 nonebot-plugin-mcping-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-18 16:58:19.000000 nonebot-plugin-mcping-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-18 16:58:33.199365 nonebot-plugin-mcping-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-18 16:58:19.000000 nonebot-plugin-mcping-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:58:33.187364 nonebot-plugin-mcping-0.0.3/nonebot_plugin_mcping/
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-18 16:58:19.000000 nonebot-plugin-mcping-0.0.3/nonebot_plugin_mcping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-18 16:58:19.000000 nonebot-plugin-mcping-0.0.3/nonebot_plugin_mcping/bg.png
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-06-18 16:58:19.000000 nonebot-plugin-mcping-0.0.3/nonebot_plugin_mcping/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)  9753388 2023-06-18 16:58:19.000000 nonebot-plugin-mcping-0.0.3/nonebot_plugin_mcping/simhei.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:58:33.199365 nonebot-plugin-mcping-0.0.3/nonebot_plugin_mcping.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-18 16:58:33.000000 nonebot-plugin-mcping-0.0.3/nonebot_plugin_mcping.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-18 16:58:33.000000 nonebot-plugin-mcping-0.0.3/nonebot_plugin_mcping.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 16:58:33.000000 nonebot-plugin-mcping-0.0.3/nonebot_plugin_mcping.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-18 16:58:33.000000 nonebot-plugin-mcping-0.0.3/nonebot_plugin_mcping.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-18 16:58:33.000000 nonebot-plugin-mcping-0.0.3/nonebot_plugin_mcping.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 16:58:33.199365 nonebot-plugin-mcping-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-18 16:58:19.000000 nonebot-plugin-mcping-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:58:45.960824 nonebot-plugin-mcping-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-18 16:58:32.000000 nonebot-plugin-mcping-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-18 16:58:45.960824 nonebot-plugin-mcping-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-18 16:58:32.000000 nonebot-plugin-mcping-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:58:45.948824 nonebot-plugin-mcping-0.0.4/nonebot_plugin_mcping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-18 16:58:32.000000 nonebot-plugin-mcping-0.0.4/nonebot_plugin_mcping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-18 16:58:32.000000 nonebot-plugin-mcping-0.0.4/nonebot_plugin_mcping/bg.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-06-18 16:58:32.000000 nonebot-plugin-mcping-0.0.4/nonebot_plugin_mcping/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)  9753388 2023-06-18 16:58:32.000000 nonebot-plugin-mcping-0.0.4/nonebot_plugin_mcping/simhei.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:58:45.960824 nonebot-plugin-mcping-0.0.4/nonebot_plugin_mcping.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-18 16:58:45.000000 nonebot-plugin-mcping-0.0.4/nonebot_plugin_mcping.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-18 16:58:45.000000 nonebot-plugin-mcping-0.0.4/nonebot_plugin_mcping.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 16:58:45.000000 nonebot-plugin-mcping-0.0.4/nonebot_plugin_mcping.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-18 16:58:45.000000 nonebot-plugin-mcping-0.0.4/nonebot_plugin_mcping.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-18 16:58:45.000000 nonebot-plugin-mcping-0.0.4/nonebot_plugin_mcping.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 16:58:45.960824 nonebot-plugin-mcping-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-18 16:58:32.000000 nonebot-plugin-mcping-0.0.4/setup.py
```

### Comparing `nonebot-plugin-mcping-0.0.3/LICENSE` & `nonebot-plugin-mcping-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcping-0.0.3/PKG-INFO` & `nonebot-plugin-mcping-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcping
-Version: 0.0.3
+Version: 0.0.4
 Summary: 基于NoneBot的查询MineCraft服务器状态并返回图片的插件
 Home-page: https://github.com/17TheWord/nonebot-plugin-mcping
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `nonebot-plugin-mcping-0.0.3/README.md` & `nonebot-plugin-mcping-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcping-0.0.3/nonebot_plugin_mcping/__init__.py` & `nonebot-plugin-mcping-0.0.4/nonebot_plugin_mcping/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcping-0.0.3/nonebot_plugin_mcping/bg.png` & `nonebot-plugin-mcping-0.0.4/nonebot_plugin_mcping/bg.png`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcping-0.0.3/nonebot_plugin_mcping/data_source.py` & `nonebot-plugin-mcping-0.0.4/nonebot_plugin_mcping/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcping-0.0.3/nonebot_plugin_mcping/simhei.ttf` & `nonebot-plugin-mcping-0.0.4/nonebot_plugin_mcping/simhei.ttf`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcping-0.0.3/nonebot_plugin_mcping.egg-info/PKG-INFO` & `nonebot-plugin-mcping-0.0.4/nonebot_plugin_mcping.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcping
-Version: 0.0.3
+Version: 0.0.4
 Summary: 基于NoneBot的查询MineCraft服务器状态并返回图片的插件
 Home-page: https://github.com/17TheWord/nonebot-plugin-mcping
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `nonebot-plugin-mcping-0.0.3/setup.py` & `nonebot-plugin-mcping-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot-plugin-mcping",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.0.3",  # 程序版本
+    version="0.0.4",  # 程序版本
     author="17TheWord",  # 项目作者
     author_email="17theword@gmail.com",  # 作者邮件
     description="基于NoneBot的查询MineCraft服务器状态并返回图片的插件",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述？
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/17TheWord/nonebot-plugin-mcping",  # 项目地址
     packages=setuptools.find_packages(),
```

