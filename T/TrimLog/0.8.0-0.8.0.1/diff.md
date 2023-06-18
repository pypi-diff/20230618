# Comparing `tmp/TrimLog-0.8.0.tar.gz` & `tmp/TrimLog-0.8.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TrimLog-0.8.0.tar", last modified: Sun Jun 18 11:44:05 2023, max compression
+gzip compressed data, was "TrimLog-0.8.0.1.tar", last modified: Sun Jun 18 14:13:21 2023, max compression
```

## Comparing `TrimLog-0.8.0.tar` & `TrimLog-0.8.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 11:44:05.076604 TrimLog-0.8.0/
--rw-rw-rw-   0        0        0    11386 2023-01-27 04:01:21.000000 TrimLog-0.8.0/LICENSE
--rw-rw-rw-   0        0        0     2613 2023-06-18 11:44:05.074612 TrimLog-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     1604 2023-06-18 11:43:08.000000 TrimLog-0.8.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 11:44:05.051688 TrimLog-0.8.0/TrimLog/
--rw-rw-rw-   0        0        0     1296 2023-06-18 11:36:28.000000 TrimLog-0.8.0/TrimLog/__init__.py
--rw-rw-rw-   0        0        0      276 2023-02-02 05:01:04.000000 TrimLog-0.8.0/TrimLog/exceptions.py
--rw-rw-rw-   0        0        0     2433 2023-02-02 06:39:46.000000 TrimLog-0.8.0/TrimLog/logger_constants.py
--rw-rw-rw-   0        0        0    29289 2023-06-18 11:41:05.000000 TrimLog-0.8.0/TrimLog/logger_main.py
--rw-rw-rw-   0        0        0     2135 2023-02-03 07:05:46.000000 TrimLog-0.8.0/TrimLog/object_constants.py
--rw-rw-rw-   0        0        0     8463 2023-06-18 11:36:28.000000 TrimLog-0.8.0/TrimLog/pip_manager.py
--rw-rw-rw-   0        0        0     3771 2023-04-21 13:02:38.000000 TrimLog-0.8.0/TrimLog/test.py
-drwxrwxrwx   0        0        0        0 2023-06-18 11:44:05.070624 TrimLog-0.8.0/TrimLog.egg-info/
--rw-rw-rw-   0        0        0     2613 2023-06-18 11:44:04.000000 TrimLog-0.8.0/TrimLog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-06-18 11:44:04.000000 TrimLog-0.8.0/TrimLog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 11:44:04.000000 TrimLog-0.8.0/TrimLog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-18 11:44:04.000000 TrimLog-0.8.0/TrimLog.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-18 11:44:04.000000 TrimLog-0.8.0/TrimLog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 11:44:05.076604 TrimLog-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1549 2023-06-18 11:36:28.000000 TrimLog-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 14:13:21.619547 TrimLog-0.8.0.1/
+-rw-rw-rw-   0        0        0    11386 2023-01-27 04:01:21.000000 TrimLog-0.8.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2617 2023-06-18 14:13:21.618551 TrimLog-0.8.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1606 2023-06-18 14:13:10.000000 TrimLog-0.8.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 14:13:21.603600 TrimLog-0.8.0.1/TrimLog/
+-rw-rw-rw-   0        0        0     1298 2023-06-18 14:10:17.000000 TrimLog-0.8.0.1/TrimLog/__init__.py
+-rw-rw-rw-   0        0        0      276 2023-02-02 05:01:04.000000 TrimLog-0.8.0.1/TrimLog/exceptions.py
+-rw-rw-rw-   0        0        0     2433 2023-02-02 06:39:46.000000 TrimLog-0.8.0.1/TrimLog/logger_constants.py
+-rw-rw-rw-   0        0        0    29545 2023-06-18 14:10:17.000000 TrimLog-0.8.0.1/TrimLog/logger_main.py
+-rw-rw-rw-   0        0        0     2135 2023-02-03 07:05:46.000000 TrimLog-0.8.0.1/TrimLog/object_constants.py
+-rw-rw-rw-   0        0        0     8463 2023-06-18 11:36:28.000000 TrimLog-0.8.0.1/TrimLog/pip_manager.py
+-rw-rw-rw-   0        0        0     3771 2023-04-21 13:02:38.000000 TrimLog-0.8.0.1/TrimLog/test.py
+drwxrwxrwx   0        0        0        0 2023-06-18 14:13:21.616557 TrimLog-0.8.0.1/TrimLog.egg-info/
+-rw-rw-rw-   0        0        0     2617 2023-06-18 14:13:21.000000 TrimLog-0.8.0.1/TrimLog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-06-18 14:13:21.000000 TrimLog-0.8.0.1/TrimLog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 14:13:21.000000 TrimLog-0.8.0.1/TrimLog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-18 14:13:21.000000 TrimLog-0.8.0.1/TrimLog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-18 14:13:21.000000 TrimLog-0.8.0.1/TrimLog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 14:13:21.619547 TrimLog-0.8.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1549 2023-06-18 11:36:28.000000 TrimLog-0.8.0.1/setup.py
```

### Comparing `TrimLog-0.8.0/LICENSE` & `TrimLog-0.8.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TrimLog-0.8.0/PKG-INFO` & `TrimLog-0.8.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrimLog
-Version: 0.8.0
+Version: 0.8.0.1
 Summary: TriMO组织的python项目log和项目管理框架库。
 Home-page: https://github.com/TriM-Organization/TrimLog
 Author: FedDragon1, Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
@@ -26,15 +26,15 @@
 TriMO组织的python项目log和项目管理框架库。
 
 ---
 
 The Python project log and project management framework library for TriM Organization.
 
 
-### 目前版本 Current version: `v0.8.0`
+### 目前版本 Current version: `v0.8.0.1`
 
 ### 软件架构 Software architecture
 `__init__.py`: 声明程序
 
 `logger_main.py`: 主要logger对象所在的程序
 
 `logger_constants.py`: logger默认文本数据
```

### Comparing `TrimLog-0.8.0/README.md` & `TrimLog-0.8.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 TriMO组织的python项目log和项目管理框架库。
 
 ---
 
 The Python project log and project management framework library for TriM Organization.
 
 
-### 目前版本 Current version: `v0.8.0`
+### 目前版本 Current version: `v0.8.0.1`
 
 ### 软件架构 Software architecture
 `__init__.py`: 声明程序
 
 `logger_main.py`: 主要logger对象所在的程序
 
 `logger_constants.py`: logger默认文本数据
```

### Comparing `TrimLog-0.8.0/TrimLog/__init__.py` & `TrimLog-0.8.0.1/TrimLog/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
    You may obtain a copy of the License at
 
        https://www.apache.org/licenses/LICENSE-2.0
 """
 
 from .logger_main import *
 
-__version__: str = "v0.8.0"
+__version__: str = "v0.8.0.1"
 
 set_version(__version__)
 
 
 def get_version() -> str:
     """获取版本号"""
     return __version__
```

### Comparing `TrimLog-0.8.0/TrimLog/logger_constants.py` & `TrimLog-0.8.0.1/TrimLog/logger_constants.py`

 * *Files identical despite different names*

### Comparing `TrimLog-0.8.0/TrimLog/logger_main.py` & `TrimLog-0.8.0.1/TrimLog/logger_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -599,21 +599,24 @@
                         ):
                             print(i["tips"])
                             Logger.instance.log_text += i["tips"] + "\n"
                     except BaseException:
                         pass
 
     @staticmethod
-    def register_traceback(console_width: int = 64, info_show_fun=None) -> None:
+    def register_traceback(console_width: int = 64, info_show_fun=lambda x:None) -> None:
         """
         register traceback function.
         :param console_width: int, the width of traceback console as well the traceback log file's context
         :param info_show_fun: function, there should be a function, which must contains an argument to convery
         a traceback information
         """
+        if not isinstance(info_show_fun, type(lambda x:None)):
+            logger.write('参数 info_show_fun 应该是一个函数。你传入的是 {}: {}'.format(info_show_fun,type(info_show_fun)))
+            info_show_fun = lambda x: None
         if Logger.instance.is_logging:
             traceback_console = Console(file=sys.stderr, width=console_width)
 
             def excepthook(
                 type_: Type[BaseException],
                 value: BaseException,
                 traceback: Optional[TracebackType],
```

### Comparing `TrimLog-0.8.0/TrimLog/object_constants.py` & `TrimLog-0.8.0.1/TrimLog/object_constants.py`

 * *Files identical despite different names*

### Comparing `TrimLog-0.8.0/TrimLog/pip_manager.py` & `TrimLog-0.8.0.1/TrimLog/pip_manager.py`

 * *Files identical despite different names*

### Comparing `TrimLog-0.8.0/TrimLog/test.py` & `TrimLog-0.8.0.1/TrimLog/test.py`

 * *Files identical despite different names*

### Comparing `TrimLog-0.8.0/TrimLog.egg-info/PKG-INFO` & `TrimLog-0.8.0.1/TrimLog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrimLog
-Version: 0.8.0
+Version: 0.8.0.1
 Summary: TriMO组织的python项目log和项目管理框架库。
 Home-page: https://github.com/TriM-Organization/TrimLog
 Author: FedDragon1, Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
@@ -26,15 +26,15 @@
 TriMO组织的python项目log和项目管理框架库。
 
 ---
 
 The Python project log and project management framework library for TriM Organization.
 
 
-### 目前版本 Current version: `v0.8.0`
+### 目前版本 Current version: `v0.8.0.1`
 
 ### 软件架构 Software architecture
 `__init__.py`: 声明程序
 
 `logger_main.py`: 主要logger对象所在的程序
 
 `logger_constants.py`: logger默认文本数据
```

### Comparing `TrimLog-0.8.0/setup.py` & `TrimLog-0.8.0.1/setup.py`

 * *Files identical despite different names*

