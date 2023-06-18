# Comparing `tmp/mcqq-tool-0.0.6.tar.gz` & `tmp/mcqq-tool-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcqq-tool-0.0.6.tar", last modified: Thu Apr 27 12:29:46 2023, max compression
+gzip compressed data, was "mcqq-tool-0.0.7.tar", last modified: Sun Jun 18 17:08:34 2023, max compression
```

## Comparing `mcqq-tool-0.0.6.tar` & `mcqq-tool-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:29:46.953814 mcqq-tool-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-27 12:29:36.000000 mcqq-tool-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-27 12:29:46.953814 mcqq-tool-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-27 12:29:36.000000 mcqq-tool-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:29:46.953814 mcqq-tool-0.0.6/mcqq_tool/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 12:29:36.000000 mcqq-tool-0.0.6/mcqq_tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-27 12:29:36.000000 mcqq-tool-0.0.6/mcqq_tool/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-27 12:29:36.000000 mcqq-tool-0.0.6/mcqq_tool/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:29:46.953814 mcqq-tool-0.0.6/mcqq_tool/model/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-27 12:29:36.000000 mcqq-tool-0.0.6/mcqq_tool/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-27 12:29:36.000000 mcqq-tool-0.0.6/mcqq_tool/model/basemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-27 12:29:36.000000 mcqq-tool-0.0.6/mcqq_tool/model/minecraft.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 12:29:36.000000 mcqq-tool-0.0.6/mcqq_tool/model/model_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-27 12:29:36.000000 mcqq-tool-0.0.6/mcqq_tool/model/spigot.py
--rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-04-27 12:29:36.000000 mcqq-tool-0.0.6/mcqq_tool/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:29:46.953814 mcqq-tool-0.0.6/mcqq_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-27 12:29:46.000000 mcqq-tool-0.0.6/mcqq_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-27 12:29:46.000000 mcqq-tool-0.0.6/mcqq_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 12:29:46.000000 mcqq-tool-0.0.6/mcqq_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-27 12:29:46.000000 mcqq-tool-0.0.6/mcqq_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 12:29:46.000000 mcqq-tool-0.0.6/mcqq_tool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 12:29:46.953814 mcqq-tool-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-27 12:29:36.000000 mcqq-tool-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:08:34.324747 mcqq-tool-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-18 17:08:19.000000 mcqq-tool-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-18 17:08:34.324747 mcqq-tool-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-18 17:08:19.000000 mcqq-tool-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:08:34.320747 mcqq-tool-0.0.7/mcqq_tool/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 17:08:19.000000 mcqq-tool-0.0.7/mcqq_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-18 17:08:19.000000 mcqq-tool-0.0.7/mcqq_tool/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-18 17:08:19.000000 mcqq-tool-0.0.7/mcqq_tool/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:08:34.324747 mcqq-tool-0.0.7/mcqq_tool/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-18 17:08:19.000000 mcqq-tool-0.0.7/mcqq_tool/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-18 17:08:19.000000 mcqq-tool-0.0.7/mcqq_tool/model/basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-18 17:08:19.000000 mcqq-tool-0.0.7/mcqq_tool/model/minecraft.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 17:08:19.000000 mcqq-tool-0.0.7/mcqq_tool/model/model_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-18 17:08:19.000000 mcqq-tool-0.0.7/mcqq_tool/model/spigot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-06-18 17:08:19.000000 mcqq-tool-0.0.7/mcqq_tool/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:08:34.320747 mcqq-tool-0.0.7/mcqq_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-18 17:08:34.000000 mcqq-tool-0.0.7/mcqq_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-18 17:08:34.000000 mcqq-tool-0.0.7/mcqq_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 17:08:34.000000 mcqq-tool-0.0.7/mcqq_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-18 17:08:34.000000 mcqq-tool-0.0.7/mcqq_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-18 17:08:34.000000 mcqq-tool-0.0.7/mcqq_tool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 17:08:34.324747 mcqq-tool-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-18 17:08:19.000000 mcqq-tool-0.0.7/setup.py
```

### Comparing `mcqq-tool-0.0.6/LICENSE` & `mcqq-tool-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.6/PKG-INFO` & `mcqq-tool-0.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcqq-tool
-Version: 0.0.6
+Version: 0.0.7
 Summary: MC_QQ 工具包
 Home-page: https://github.com/17TheWord/mcqq-tool
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mcqq-tool-0.0.6/mcqq_tool/common.py` & `mcqq-tool-0.0.7/mcqq_tool/common.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.6/mcqq_tool/config.py` & `mcqq-tool-0.0.7/mcqq_tool/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -37,14 +37,16 @@
     server_name: str
     # 服务器群列表
     group_list: Optional[List[int]] = []
     # 服务器频道列表
     guild_list: Optional[List[Guild]] = []
     # 是否开启 Rcon
     rcon_enable: Optional[bool] = False
+    # 该群Bot ID
+    self_id: Optional[int] = None
 
 
 class Config(BaseModel, extra=Extra.ignore):
     """配置"""
     # 服务器地址
     mc_qq_ws_ip: Optional[str] = "127.0.0.1"
     # 服务器端口
```

### Comparing `mcqq-tool-0.0.6/mcqq_tool/model/__init__.py` & `mcqq-tool-0.0.7/mcqq_tool/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.6/mcqq_tool/model/basemodel.py` & `mcqq-tool-0.0.7/mcqq_tool/model/basemodel.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.6/mcqq_tool/model/minecraft.py` & `mcqq-tool-0.0.7/mcqq_tool/model/minecraft.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.6/mcqq_tool/model/spigot.py` & `mcqq-tool-0.0.7/mcqq_tool/model/spigot.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.6/mcqq_tool/utils.py` & `mcqq-tool-0.0.7/mcqq_tool/utils.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.6/mcqq_tool.egg-info/PKG-INFO` & `mcqq-tool-0.0.7/mcqq_tool.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcqq-tool
-Version: 0.0.6
+Version: 0.0.7
 Summary: MC_QQ 工具包
 Home-page: https://github.com/17TheWord/mcqq-tool
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mcqq-tool-0.0.6/setup.py` & `mcqq-tool-0.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="mcqq-tool",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.0.6",  # 程序版本
+    version="0.0.7",  # 程序版本
     author="17TheWord",  # 项目作者
     author_email="17theword@gmail.com",  # 作者邮件
     description="MC_QQ 工具包",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述？
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/17TheWord/mcqq-tool",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
```

