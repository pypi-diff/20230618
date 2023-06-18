# Comparing `tmp/TrimLog-0.7.3.tar.gz` & `tmp/TrimLog-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TrimLog-0.7.3.tar", last modified: Sat Apr  8 14:55:13 2023, max compression
+gzip compressed data, was "TrimLog-0.8.0.tar", last modified: Sun Jun 18 11:44:05 2023, max compression
```

## Comparing `TrimLog-0.7.3.tar` & `TrimLog-0.8.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 14:55:13.653575 TrimLog-0.7.3/
--rw-rw-rw-   0        0        0    11386 2023-01-27 04:01:21.000000 TrimLog-0.7.3/LICENSE
--rw-rw-rw-   0        0        0     2613 2023-04-08 14:55:13.652575 TrimLog-0.7.3/PKG-INFO
--rw-rw-rw-   0        0        0     1604 2023-04-08 14:52:40.000000 TrimLog-0.7.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 14:55:13.639575 TrimLog-0.7.3/TrimLog/
--rw-rw-rw-   0        0        0     1296 2023-04-08 14:52:40.000000 TrimLog-0.7.3/TrimLog/__init__.py
--rw-rw-rw-   0        0        0      276 2023-02-02 05:01:04.000000 TrimLog-0.7.3/TrimLog/exceptions.py
--rw-rw-rw-   0        0        0     2433 2023-02-02 06:39:46.000000 TrimLog-0.7.3/TrimLog/logger_constants.py
--rw-rw-rw-   0        0        0    28657 2023-04-08 14:39:11.000000 TrimLog-0.7.3/TrimLog/logger_main.py
--rw-rw-rw-   0        0        0     2135 2023-02-03 07:05:46.000000 TrimLog-0.7.3/TrimLog/object_constants.py
--rw-rw-rw-   0        0        0     8283 2023-02-12 07:45:45.000000 TrimLog-0.7.3/TrimLog/pip_manager.py
--rw-rw-rw-   0        0        0     3771 2023-04-08 14:50:47.000000 TrimLog-0.7.3/TrimLog/test.py
-drwxrwxrwx   0        0        0        0 2023-04-08 14:55:13.650575 TrimLog-0.7.3/TrimLog.egg-info/
--rw-rw-rw-   0        0        0     2613 2023-04-08 14:55:13.000000 TrimLog-0.7.3/TrimLog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-04-08 14:55:13.000000 TrimLog-0.7.3/TrimLog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 14:55:13.000000 TrimLog-0.7.3/TrimLog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-08 14:55:13.000000 TrimLog-0.7.3/TrimLog.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-08 14:55:13.000000 TrimLog-0.7.3/TrimLog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-08 14:55:13.653575 TrimLog-0.7.3/setup.cfg
--rw-rw-rw-   0        0        0     1461 2023-04-08 14:54:52.000000 TrimLog-0.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 11:44:05.076604 TrimLog-0.8.0/
+-rw-rw-rw-   0        0        0    11386 2023-01-27 04:01:21.000000 TrimLog-0.8.0/LICENSE
+-rw-rw-rw-   0        0        0     2613 2023-06-18 11:44:05.074612 TrimLog-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1604 2023-06-18 11:43:08.000000 TrimLog-0.8.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 11:44:05.051688 TrimLog-0.8.0/TrimLog/
+-rw-rw-rw-   0        0        0     1296 2023-06-18 11:36:28.000000 TrimLog-0.8.0/TrimLog/__init__.py
+-rw-rw-rw-   0        0        0      276 2023-02-02 05:01:04.000000 TrimLog-0.8.0/TrimLog/exceptions.py
+-rw-rw-rw-   0        0        0     2433 2023-02-02 06:39:46.000000 TrimLog-0.8.0/TrimLog/logger_constants.py
+-rw-rw-rw-   0        0        0    29289 2023-06-18 11:41:05.000000 TrimLog-0.8.0/TrimLog/logger_main.py
+-rw-rw-rw-   0        0        0     2135 2023-02-03 07:05:46.000000 TrimLog-0.8.0/TrimLog/object_constants.py
+-rw-rw-rw-   0        0        0     8463 2023-06-18 11:36:28.000000 TrimLog-0.8.0/TrimLog/pip_manager.py
+-rw-rw-rw-   0        0        0     3771 2023-04-21 13:02:38.000000 TrimLog-0.8.0/TrimLog/test.py
+drwxrwxrwx   0        0        0        0 2023-06-18 11:44:05.070624 TrimLog-0.8.0/TrimLog.egg-info/
+-rw-rw-rw-   0        0        0     2613 2023-06-18 11:44:04.000000 TrimLog-0.8.0/TrimLog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-06-18 11:44:04.000000 TrimLog-0.8.0/TrimLog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 11:44:04.000000 TrimLog-0.8.0/TrimLog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-18 11:44:04.000000 TrimLog-0.8.0/TrimLog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-18 11:44:04.000000 TrimLog-0.8.0/TrimLog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 11:44:05.076604 TrimLog-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     1549 2023-06-18 11:36:28.000000 TrimLog-0.8.0/setup.py
```

### Comparing `TrimLog-0.7.3/LICENSE` & `TrimLog-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TrimLog-0.7.3/PKG-INFO` & `TrimLog-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrimLog
-Version: 0.7.3
+Version: 0.8.0
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
 
 
-### 目前版本 Current version: `v0.7.3`
+### 目前版本 Current version: `v0.8.0`
 
 ### 软件架构 Software architecture
 `__init__.py`: 声明程序
 
 `logger_main.py`: 主要logger对象所在的程序
 
 `logger_constants.py`: logger默认文本数据
```

### Comparing `TrimLog-0.7.3/README.md` & `TrimLog-0.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 TriMO组织的python项目log和项目管理框架库。
 
 ---
 
 The Python project log and project management framework library for TriM Organization.
 
 
-### 目前版本 Current version: `v0.7.3`
+### 目前版本 Current version: `v0.8.0`
 
 ### 软件架构 Software architecture
 `__init__.py`: 声明程序
 
 `logger_main.py`: 主要logger对象所在的程序
 
 `logger_constants.py`: logger默认文本数据
```

### Comparing `TrimLog-0.7.3/TrimLog/__init__.py` & `TrimLog-0.8.0/TrimLog/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
    You may obtain a copy of the License at
 
        https://www.apache.org/licenses/LICENSE-2.0
 """
 
 from .logger_main import *
 
-__version__: str = "v0.7.3"
+__version__: str = "v0.8.0"
 
 set_version(__version__)
 
 
 def get_version() -> str:
     """获取版本号"""
     return __version__
```

### Comparing `TrimLog-0.7.3/TrimLog/logger_constants.py` & `TrimLog-0.8.0/TrimLog/logger_constants.py`

 * *Files identical despite different names*

### Comparing `TrimLog-0.7.3/TrimLog/logger_main.py` & `TrimLog-0.8.0/TrimLog/logger_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
        https://www.apache.org/licenses/LICENSE-2.0
 """
 
 from __future__ import annotations
 
 import atexit
 import platform
-import sys
 import time
 
 from types import TracebackType
 from typing import Literal, Optional, Type, TypeVar
 
 import rich.traceback
 from rich.console import Console
@@ -70,31 +69,30 @@
     console: Console = Console()
     """
     Logger.console 
     If you want to use rich in OSC, you should use: osc.get_console(logger.console)
     """
 
     def __new__(
-            cls,
-            is_logging: bool = True,
-            is_auto_headline: bool = False,
-            is_tips: bool = True,
-            printing: bool = True,
-            writing: bool = True,
-            include_headline: bool = True,
-            include_license: bool = True,
-            include_release_info: bool = False,
-            print_level: L = "DEBUG",
-            write_level: L = "INFO",
-            headline_level: L = "WARNING",
-            license_level: L = "WARNING",
-            max_log_count: int = 20,
-            show_position: bool = False,
-            in_suffix: str = ".dsl",
-
+        cls,
+        is_logging: bool = True,
+        is_auto_headline: bool = False,
+        is_tips: bool = True,
+        printing: bool = True,
+        writing: bool = True,
+        include_headline: bool = True,
+        include_license: bool = True,
+        include_release_info: bool = False,
+        print_level: L = "DEBUG",
+        write_level: L = "INFO",
+        headline_level: L = "WARNING",
+        license_level: L = "WARNING",
+        max_log_count: int = 20,
+        show_position: bool = False,
+        in_suffix: str = ".dsl",
     ) -> Logger:
         """
         __new__() method. Don't change it unless you need.
         :param is_logging: use logger or not. Notice that this is the main switch of Logger class.
         :param printing: print on the screen or not.
         :param writing: write into file or not.
         :param print_level: a level that's used to limit the print.
@@ -114,31 +112,30 @@
         if cls.instance is not None:
             return cls.instance
         cls.instance = super().__new__(cls)
 
         return cls.instance
 
     def __init__(
-            self,
-            is_logging: bool = True,
-            is_auto_headline: bool = False,
-            is_tips: bool = True,
-            printing: bool = True,
-            writing: bool = True,
-            include_headline: bool = True,
-            include_license: bool = True,
-            include_release_info: bool = False,
-            print_level: L = "DEBUG",
-            write_level: L = "INFO",
-            headline_level: L = "WARNING",
-            license_level: L = "WARNING",
-            max_log_count: int = 20,
-            show_position: bool = False,
-            in_suffix: str = ".dsl",
-
+        self,
+        is_logging: bool = True,
+        is_auto_headline: bool = False,
+        is_tips: bool = True,
+        printing: bool = True,
+        writing: bool = True,
+        include_headline: bool = True,
+        include_license: bool = True,
+        include_release_info: bool = False,
+        print_level: L = "DEBUG",
+        write_level: L = "INFO",
+        headline_level: L = "WARNING",
+        license_level: L = "WARNING",
+        max_log_count: int = 20,
+        show_position: bool = False,
+        in_suffix: str = ".dsl",
     ) -> None:
         """
         __init__() method. Don't change it unless you need.
         :param is_logging: use logger or not. Notice that this is the main switch of Logger class.
         :param is_auto_headline: allow to print headline when the logger is initializing or not.
         The best choice is false.
         :param is_tips: allow to show some tips when the program have errors or not.
@@ -196,21 +193,21 @@
         self.headline_count = 0
 
         # 初始化展示headline
         if is_auto_headline:
             self.headline_shower()
 
     def log(
-            self,
-            info: T,
-            level: L,
-            mandatory_use: bool = False,
-            frame_file: str = None,
-            frame_name: str = None,
-            frame_lineno: int = None,
+        self,
+        info: T,
+        level: L,
+        mandatory_use: bool = False,
+        frame_file: str = None,
+        frame_name: str = None,
+        frame_lineno: int = None,
     ) -> T:
         """
         log output base function.
         :param info: things you want to output.
         :param level: the log output level.
         :param mandatory_use: allow to use this function while "self.is_logging" is False.
         :param frame_file: initiation program's file name.
@@ -249,21 +246,20 @@
             if self.writing and level_weight >= self.write_default_weight:
                 if self.show_position:
                     e_w = end_with.replace("\n", "")
                     self.log_text += (
                         f"{time.strftime('[%H:%M:%S]')} [{level}] [{e_w}] {info}\n"
                     )
                 else:
-                    self.log_text += (
-                        f"{time.strftime('[%H:%M:%S]')} [{level}] {info}\n"
-                    )
+                    self.log_text += f"{time.strftime('[%H:%M:%S]')} [{level}] {info}\n"
 
             # 打印模块(条件：启用打印；满足打印权重)
-            if (self.printing and level_weight >= self.print_default_weight) or \
-                    mandatory_use:
+            if (
+                self.printing and level_weight >= self.print_default_weight
+            ) or mandatory_use:
                 if self.show_position:
                     e_w = " <" + end_with.replace("\n", "") + "> "
                     add = style + e_w
                     self.console.log(f"{add:<{length}}{info!s:<10}")
                 else:
                     self.console.log(f"{style:<{length}}{info!s:<10}")
 
@@ -318,60 +314,84 @@
         """
         back_frame = sys._getframe().f_back.f_back  # 上一帧=debug/info/..., 上上帧=目标函数
         back_file_name: str = os.path.basename(back_frame.f_code.co_filename)
         back_func_name: str = back_frame.f_code.co_name
         back_line_number: int = back_frame.f_lineno
         return back_file_name, back_func_name, back_line_number
 
-    def debug(self, debug: T, mandatory_use: bool = False, ) -> T:
+    def debug(
+        self,
+        debug: T,
+        mandatory_use: bool = False,
+    ) -> T:
         """
         output log that's "debug" level.
         :param debug: things you want to output.
         :param mandatory_use: allow to use this function while "self.is_logging" is False.
         :return:things you want to output.
         """
         return self.log(debug, "DEBUG", mandatory_use, *self.get_detail_info())
 
-    def info(self, info: T, mandatory_use: bool = False, ) -> T:
+    def info(
+        self,
+        info: T,
+        mandatory_use: bool = False,
+    ) -> T:
         """
         output log that's "info" level.
         :param info: things you want to output.
         :param mandatory_use: allow to use this function while "self.is_logging" is False.
         :return: things you want to output.
         """
         return self.log(info, "INFO", mandatory_use, *self.get_detail_info())
 
-    def warning(self, warning: T, mandatory_use: bool = False, ) -> T:
+    def warning(
+        self,
+        warning: T,
+        mandatory_use: bool = False,
+    ) -> T:
         """
         output log that's "warning" level.
         :param warning: things you want to output.
         :param mandatory_use: allow to use this function while "self.is_logging" is False.
         :return: things you want to output.
         """
         return self.log(warning, "WARNING", mandatory_use, *self.get_detail_info())
 
-    def error(self, error: T, mandatory_use: bool = False, ) -> T:
+    def error(
+        self,
+        error: T,
+        mandatory_use: bool = False,
+    ) -> T:
         """
         output log that's "error" level.
         :param error: things you want to output.
         :param mandatory_use: allow to use this function while "self.is_logging" is False.
         :return: things you want to output.
         """
         return self.log(error, "ERROR", mandatory_use, *self.get_detail_info())
 
-    def critical(self, critical: T, mandatory_use: bool = False, ) -> T:
+    def critical(
+        self,
+        critical: T,
+        mandatory_use: bool = False,
+    ) -> T:
         """
         output log that's "critical" level.
         :param critical: things you want to output.
         :param mandatory_use: allow to use this function while "self.is_logging" is False.
         :return: things you want to output.
         """
         return self.log(critical, "CRITICAL", mandatory_use, *self.get_detail_info())
 
-    def write(self, text: str, mandatory_use: bool = False, ) -> None:
+    def write(
+        self,
+        text: str,
+        mandatory_use: bool = False,
+    ) -> None:
         """
         write things into self.log_text.
         :param text: things
         :param mandatory_use: allow to use this function while "self.is_logging" is False.
         """
         if (self.is_logging and self.writing) or mandatory_use:
             self.log_text += text
@@ -379,16 +399,17 @@
     def headline_shower(self, mandatory_use: bool = False) -> None:
         """
         show this library's headline.
         :param mandatory_use: allow to use this function while "self.is_logging" is False and self.headline_count >= 1.
         control
         """
         global __version__, pip_manage_, osc_
-        if (self.include_headline is True and self.headline_count < 1) or \
-                mandatory_use is True:  # 启动两种条件：允许自动包含打印且次数为0；强制打印
+        if (
+            self.include_headline is True and self.headline_count < 1
+        ) or mandatory_use is True:  # 启动两种条件：允许自动包含打印且次数为0；强制打印
             self.console.rule("[bold red]Headline")  # 画线
             self.log(
                 HEADLINE_STRUCTURE.format(osc_.project_name, osc_.version, __version__),
                 self.headline_level,
                 mandatory_use=True,
             )  # 强制log
 
@@ -426,25 +447,25 @@
                     running_path,
                     default_encoding,
                     file_system_encoding,
                     pip_list,
                     pip_check,
                 ),
                 self.headline_level,  # 跟headline同级输出
-                mandatory_use=True  # 强制
+                mandatory_use=True,  # 强制
             )
 
     def license_shower(
-            self,
-            lib_name: str,
-            license_name: str,
-            license_line: str,
-            lib_version: str,
-            addition: str = "",
-            include_startline: bool = True,
+        self,
+        lib_name: str,
+        license_name: str,
+        license_line: str,
+        lib_version: str,
+        addition: str = "",
+        include_startline: bool = True,
     ) -> None:
         """
         show a specified license
         :param lib_name: what's your importing lib's name?
         :param license_name: what's your importing lib's license?
         :param license_line: copy your importing lib's license show information. Be like:
         Copyright 2022-2023 all the developers of Trim Organization.(FedDragon1, Eilles Wan, bgArray)
@@ -501,15 +522,17 @@
             try:
                 list_of_files = os.listdir("logs")
             except FileNotFoundError:
                 os.makedirs("logs")  # 不存在就新建
             else:
                 full_path = ["logs/{0}".format(x) for x in list_of_files]  # 存在就移除最早日志
 
-                if len(list_of_files) >= Logger.instance.max_log_count:  # 用 instance 访问self里的对象
+                if (
+                    len(list_of_files) >= Logger.instance.max_log_count
+                ):  # 用 instance 访问self里的对象
                     oldest_file = min(full_path, key=os.path.getctime)
                     logger.log(f"移除最早的日志：{oldest_file!r}", INFO)
                     os.remove(oldest_file)
 
             # 写入日志
             try:
                 path = os.path.abspath("./logs/")
@@ -522,19 +545,21 @@
                     return
 
                 if Logger.instance.log_text == "":
                     Logger.instance.log(f"日志未保存：空日志文件", "INFO")
                     return
 
                 # 打开文件写入
-                whole_path = "./logs/" + (name := Logger.str_start_time + f"{Logger.instance.suffix}.log")
+                whole_path = "./logs/" + (
+                    name := Logger.str_start_time + f"{Logger.instance.suffix}.log"
+                )
                 with open(
-                        whole_path,
-                        "w",
-                        encoding="UTF-8",
+                    whole_path,
+                    "w",
+                    encoding="UTF-8",
                 ) as f:
                     f.write(Logger.instance.log_text)  # 写入
 
                 Logger.instance.log(f"日志保存至 '{path}\\{name}'", "INFO")
 
             except IOError as e:
                 Logger.instance.log(f'日志保存失败："{e}"', "ERROR")
@@ -546,15 +571,15 @@
         add tips' function.
         """
         global osc_
         if (Logger.instance.is_logging and osc_.isRelease) or Logger.instance.is_tips:
             log_t = Logger.instance.log_text
             tips_d = Logger.instance.tips_list
             del_t = (
-                    "┌" + "─" * 31 + " Traceback (most recent call last) " + "─" * 32 + "┐"
+                "┌" + "─" * 31 + " Traceback (most recent call last) " + "─" * 32 + "┐"
             )
             end_t = "└" + "─" * 98 + "┘"
 
             clean_t = (
                 log_t[log_t.find(del_t) + 100:].replace("│ │", "").replace("│", "")
             )
 
@@ -565,34 +590,37 @@
             error_position = error_position[error_position.rfind("\\") + 1:]
 
             if tips_d is not []:
                 for i in tips_d:
                     # noinspection PyBroadException
                     try:
                         if (
-                                error_position == i["position"]
-                                and end_error_text == i["error_text"]
+                            error_position == i["position"]
+                            and end_error_text == i["error_text"]
                         ):
                             print(i["tips"])
                             Logger.instance.log_text += i["tips"] + "\n"
                     except BaseException:
                         pass
 
     @staticmethod
-    def register_traceback() -> None:
+    def register_traceback(console_width: int = 64, info_show_fun=None) -> None:
         """
         register traceback function.
+        :param console_width: int, the width of traceback console as well the traceback log file's context
+        :param info_show_fun: function, there should be a function, which must contains an argument to convery
+        a traceback information
         """
         if Logger.instance.is_logging:
-            traceback_console = Console(file=sys.stderr, width=100)
+            traceback_console = Console(file=sys.stderr, width=console_width)
 
             def excepthook(
-                    type_: Type[BaseException],
-                    value: BaseException,
-                    traceback: Optional[TracebackType],
+                type_: Type[BaseException],
+                value: BaseException,
+                traceback: Optional[TracebackType],
             ) -> None:
 
                 exception = Traceback.from_exception(
                     type_,
                     value,
                     traceback,
                     width=WIDTH,
@@ -607,14 +635,16 @@
 
                 path = os.path.abspath("./logs/")
                 logger.log(
                     f"出现严重错误，程序崩溃！详情请看 '{path + Logger.str_start_time}{Logger.instance.suffix}.log'",
                     CRITICAL,
                 )
 
+                final_context = ""
+
                 exception_no_local = Traceback.from_exception(
                     type_,
                     value,
                     traceback,
                     width=WIDTH,
                     extra_lines=EXTRA_LINES,
                     theme=THEME,
@@ -623,45 +653,53 @@
                     indent_guides=INDENT_GUIDES,
                     suppress=SUPPRESS,
                     max_frames=MAX_FRAMES,
                 )
 
                 traceback_console.print(exception_no_local)
                 for exc in exception.__rich_console__(
-                        traceback_console, traceback_console.options
+                    traceback_console, traceback_console.options
                 ):
                     if isinstance(exc, rich.traceback.Constrain):
                         panel = exc.renderable
 
                         for thing in panel.__rich_console__(
-                                traceback_console, traceback_console.options
+                            traceback_console, traceback_console.options
                         ):
-                            logger.write(thing.text)
+                            final_context += thing.text
 
                     elif isinstance(exc, rich.traceback.Text):
-                        logger.write(str(exc.copy()) + "\n")
+                        final_context += str(exc.copy()) + "\n"
+
+                logger.write(final_context)
+
+                # 你传入的函数应该包含且仅包含一个必填参数，不然你传啥？
+                try:
+                    info_show_fun(final_context)
+                except TypeError:
+                    pass
 
             sys.excepthook = excepthook
 
 
 # 获取基础信息
 py_version: str = platform.version()
 py_sys_version: str = sys.version
 py_sys_version_info: str = sys.version_info
 py_platform: str = sys.platform
 default_encoding: str = sys.getdefaultencoding()  # 获取系统当前编码
-file_system_encoding: str = (
-    sys.getfilesystemencoding()
-)  # 获取文件系统使用编码方式
+file_system_encoding: str = sys.getfilesystemencoding()  # 获取文件系统使用编码方式
 running_path: str = os.path.abspath("./")  # logger程序目录环境
 pip_list: str = ""
 pip_check: str
 
 
-def log__init__(osc_in: ObjectStateConstant, pip_in: PipManage, is_regenerate: bool = False) -> None:
+def log__init__(
+    osc_in: ObjectStateConstant, pip_in: PipManage, is_regenerate: bool = False
+) -> None:
     """
     to initialize logger.
     :param osc_in: need an OSC class.
     :param pip_in: need a PM class.
     :param is_regenerate: if regenerate the log class, set True.
     """
     # 直接用本地变量
```

### Comparing `TrimLog-0.7.3/TrimLog/object_constants.py` & `TrimLog-0.8.0/TrimLog/object_constants.py`

 * *Files identical despite different names*

### Comparing `TrimLog-0.7.3/TrimLog/pip_manager.py` & `TrimLog-0.8.0/TrimLog/pip_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,18 +21,19 @@
    You may obtain a copy of the License at
 
        https://www.apache.org/licenses/LICENSE-2.0
 
 pip管理类开发者：bgArray
 """
 
-import pkg_resources
 import os
+import sys
+from typing import Dict, List, Tuple, Union
 
-from typing import Union, Tuple, List, Dict
+import pkg_resources
 
 from .exceptions import *
 
 
 # Pip method
 class PipManage:
     """
@@ -203,15 +204,19 @@
         """
         根据self.detect_report安装库
         :return: True/False 表示是否全部安装正确
         """
         if self.is_install_pip:
             if self.detect_report.__len__() == 0:
                 return True
-            for i in self.detect_report:
-                if i["have"] is None:
-                    command = "pip install " + str(i["need"])
-                    os.system(command)
+            libs_in_need = [
+                i["need"] if i["have"] is None else "" for i in self.detect_report
+            ]
+            if libs_in_need:
+                command = (
+                    "pip install " if sys.platform == "win32" else "pip3 install "
+                ) + " ".join(libs_in_need)
+                os.system(command)
             if self.pip_detect():
                 return True
             else:
                 return False
```

### Comparing `TrimLog-0.7.3/TrimLog/test.py` & `TrimLog-0.8.0/TrimLog/test.py`

 * *Files identical despite different names*

### Comparing `TrimLog-0.7.3/TrimLog.egg-info/PKG-INFO` & `TrimLog-0.8.0/TrimLog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrimLog
-Version: 0.7.3
+Version: 0.8.0
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
 
 
-### 目前版本 Current version: `v0.7.3`
+### 目前版本 Current version: `v0.8.0`
 
 ### 软件架构 Software architecture
 `__init__.py`: 声明程序
 
 `logger_main.py`: 主要logger对象所在的程序
 
 `logger_constants.py`: logger默认文本数据
```

### Comparing `TrimLog-0.7.3/setup.py` & `TrimLog-0.8.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="TrimLog",
     version=TrimLog.__version__,
-    author="FedDragon1, Eilles Wan, bgArray",
+    author="FedDragon1, Eilles Wan, bgArray", # 2333 你太谦虚了，你应该放在第一个的 ——EW2BA
     author_email="TriM-Organization@hotmail.com",
     description="TriMO组织的python项目log和项目管理框架库。\n"
     " The Python project log and project management framework library for TriM Organization.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TriM-Organization/TrimLog",
     packages=setuptools.find_packages(),
@@ -31,9 +31,10 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     # 需要安装的依赖
     install_requires=[
         "rich>=10.9.0",
+        "setuptools",
     ],
 )
```

