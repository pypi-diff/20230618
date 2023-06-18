# Comparing `tmp/hrbot-0.0.2.tar.gz` & `tmp/hrbot-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hrbot-0.0.2.tar", last modified: Sat Jun 17 14:56:01 2023, max compression
+gzip compressed data, was "hrbot-0.1.0.tar", max compression
```

## Comparing `hrbot-0.0.2.tar` & `hrbot-0.1.0.tar`

### file list

```diff
@@ -1,32 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 14:56:01.027844 hrbot-0.0.2/
--rw-rw-rw-   0        0        0     1331 2023-06-17 14:56:01.025282 hrbot-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      962 2023-06-17 09:59:30.000000 hrbot-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 14:56:00.968553 hrbot-0.0.2/hrbot/
--rw-rw-rw-   0        0        0      158 2023-06-15 08:01:29.000000 hrbot-0.0.2/hrbot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 14:56:00.989816 hrbot-0.0.2/hrbot/bot/
--rw-rw-rw-   0        0        0       31 2023-05-18 14:31:32.000000 hrbot-0.0.2/hrbot/bot/__init__.py
--rw-rw-rw-   0        0        0      988 2023-06-15 08:48:39.000000 hrbot-0.0.2/hrbot/bot/base.py
--rw-rw-rw-   0        0        0     3092 2023-06-14 10:31:36.000000 hrbot-0.0.2/hrbot/bot/bot.py
-drwxrwxrwx   0        0        0        0 2023-06-17 14:56:01.004114 hrbot-0.0.2/hrbot/dispatcher/
--rw-rw-rw-   0        0        0       59 2023-05-18 14:31:32.000000 hrbot-0.0.2/hrbot/dispatcher/__init__.py
--rw-rw-rw-   0        0        0     5690 2023-06-17 09:43:39.000000 hrbot-0.0.2/hrbot/dispatcher/dispatсher.py
--rw-rw-rw-   0        0        0     9399 2023-06-14 10:31:36.000000 hrbot-0.0.2/hrbot/dispatcher/filter.py
-drwxrwxrwx   0        0        0        0 2023-06-17 14:56:01.012449 hrbot-0.0.2/hrbot/dispatcher/fsm/
--rw-rw-rw-   0        0        0       30 2023-05-31 10:19:08.000000 hrbot-0.0.2/hrbot/dispatcher/fsm/__init__.py
--rw-rw-rw-   0        0        0     1972 2023-06-15 09:02:33.000000 hrbot-0.0.2/hrbot/dispatcher/fsm/state.py
--rw-rw-rw-   0        0        0     4675 2023-06-14 06:55:24.000000 hrbot-0.0.2/hrbot/dispatcher/fsm/storage.py
--rw-rw-rw-   0        0        0     1337 2023-06-14 07:07:30.000000 hrbot-0.0.2/hrbot/dispatcher/handler.py
-drwxrwxrwx   0        0        0        0 2023-06-17 14:56:01.021911 hrbot-0.0.2/hrbot/types/
--rw-rw-rw-   0        0        0      284 2023-06-11 09:43:38.000000 hrbot-0.0.2/hrbot/types/__init__.py
--rw-rw-rw-   0        0        0      432 2023-06-14 07:58:57.000000 hrbot-0.0.2/hrbot/types/handler.py
--rw-rw-rw-   0        0        0       31 2023-05-14 15:25:08.000000 hrbot-0.0.2/hrbot/types/hr.py
-drwxrwxrwx   0        0        0        0 2023-06-17 14:56:01.023434 hrbot-0.0.2/hrbot/utils/
--rw-rw-rw-   0        0        0        0 2023-05-14 13:14:36.000000 hrbot-0.0.2/hrbot/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 14:56:00.982941 hrbot-0.0.2/hrbot.egg-info/
--rw-rw-rw-   0        0        0     1331 2023-06-17 14:56:00.000000 hrbot-0.0.2/hrbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      537 2023-06-17 14:56:00.000000 hrbot-0.0.2/hrbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 14:56:00.000000 hrbot-0.0.2/hrbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-17 14:56:00.000000 hrbot-0.0.2/hrbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-17 14:56:00.000000 hrbot-0.0.2/hrbot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 14:56:01.027844 hrbot-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      756 2023-06-17 14:53:50.000000 hrbot-0.0.2/setup.py
+-rw-r--r--   0        0        0      158 2023-06-15 08:01:29.191231 hrbot-0.1.0/hrbot/__init__.py
+-rw-r--r--   0        0        0       31 2023-05-18 14:31:32.146814 hrbot-0.1.0/hrbot/bot/__init__.py
+-rw-r--r--   0        0        0      988 2023-06-15 08:48:39.851385 hrbot-0.1.0/hrbot/bot/base.py
+-rw-r--r--   0        0        0     3092 2023-06-14 10:31:36.453525 hrbot-0.1.0/hrbot/bot/bot.py
+-rw-r--r--   0        0        0       59 2023-05-18 14:31:32.138854 hrbot-0.1.0/hrbot/dispatcher/__init__.py
+-rw-r--r--   0        0        0     8581 2023-06-17 09:43:42.524896 hrbot-0.1.0/hrbot/dispatcher/__pycache__/dispatсher.cpython-311.pyc
+-rw-r--r--   0        0        0     5690 2023-06-17 09:43:39.773391 hrbot-0.1.0/hrbot/dispatcher/dispatсher.py
+-rw-r--r--   0        0        0     9399 2023-06-14 10:31:36.445953 hrbot-0.1.0/hrbot/dispatcher/filter.py
+-rw-r--r--   0        0        0       30 2023-05-31 10:19:08.115326 hrbot-0.1.0/hrbot/dispatcher/fsm/__init__.py
+-rw-r--r--   0        0        0     1972 2023-06-15 09:02:33.436860 hrbot-0.1.0/hrbot/dispatcher/fsm/state.py
+-rw-r--r--   0        0        0     4675 2023-06-14 06:55:24.164338 hrbot-0.1.0/hrbot/dispatcher/fsm/storage.py
+-rw-r--r--   0        0        0     1337 2023-06-14 07:07:30.601511 hrbot-0.1.0/hrbot/dispatcher/handler.py
+-rw-r--r--   0        0        0      284 2023-06-11 09:43:38.740611 hrbot-0.1.0/hrbot/types/__init__.py
+-rw-r--r--   0        0        0      432 2023-06-14 07:58:57.121193 hrbot-0.1.0/hrbot/types/handler.py
+-rw-r--r--   0        0        0       31 2023-05-14 15:25:08.437975 hrbot-0.1.0/hrbot/types/hr.py
+-rw-r--r--   0        0        0        0 2023-05-14 13:14:36.307325 hrbot-0.1.0/hrbot/utils/__init__.py
+-rw-r--r--   0        0        0      494 2023-06-18 07:13:28.726074 hrbot-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      962 2023-06-17 09:59:30.331030 hrbot-0.1.0/README.md
+-rw-r--r--   0        0        0     1513 1970-01-01 00:00:00.000000 hrbot-0.1.0/PKG-INFO
```

### Comparing `hrbot-0.0.2/PKG-INFO` & `hrbot-0.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: hrbot
-Version: 0.0.2
-Summary: The hrbot is a wrapper on top of the HighRise Python Bot SDK that makes it easy to create bots in HighRise.
-Home-page: https://github.com/muodosta/hrbot
-Author: MuoDosta
-Author-email: MuoDostaWork@gmail.com
-License: MIT License
-Requires-Python: >=3.10,<4.0
-Description-Content-Type: text/markdown
-
 # The hrbot
 The hrbot is a wrapper on top of the [HighRise Python Bot SDK](https://github.com/pocketzworld/python-bot-sdk) that makes it easy to create bots in [HighRise](https://highrise.game/).
 
 Install the library:
 ```shell
 pip install hrbot
 ```
@@ -43,8 +32,8 @@
 
 @dp.on_user_leave()
 async def user_leave(user: User):
     await bot.highrise.chat(f'Goodbye, {user.username}')
 
 if __name__ == '__main__':
     bot.start()
-```
+```
```

### Comparing `hrbot-0.0.2/hrbot/bot/base.py` & `hrbot-0.1.0/hrbot/bot/base.py`

 * *Files identical despite different names*

### Comparing `hrbot-0.0.2/hrbot/bot/bot.py` & `hrbot-0.1.0/hrbot/bot/bot.py`

 * *Files identical despite different names*

### Comparing `hrbot-0.0.2/hrbot/dispatcher/dispatсher.py` & `hrbot-0.1.0/hrbot/dispatcher/dispatсher.py`

 * *Files identical despite different names*

### Comparing `hrbot-0.0.2/hrbot/dispatcher/filter.py` & `hrbot-0.1.0/hrbot/dispatcher/filter.py`

 * *Files identical despite different names*

### Comparing `hrbot-0.0.2/hrbot/dispatcher/fsm/state.py` & `hrbot-0.1.0/hrbot/dispatcher/fsm/state.py`

 * *Files identical despite different names*

### Comparing `hrbot-0.0.2/hrbot/dispatcher/fsm/storage.py` & `hrbot-0.1.0/hrbot/dispatcher/fsm/storage.py`

 * *Files identical despite different names*

### Comparing `hrbot-0.0.2/hrbot/dispatcher/handler.py` & `hrbot-0.1.0/hrbot/dispatcher/handler.py`

 * *Files identical despite different names*

### Comparing `hrbot-0.0.2/hrbot.egg-info/PKG-INFO` & `hrbot-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,55 @@
-Metadata-Version: 2.1
-Name: hrbot
-Version: 0.0.2
-Summary: The hrbot is a wrapper on top of the HighRise Python Bot SDK that makes it easy to create bots in HighRise.
-Home-page: https://github.com/muodosta/hrbot
-Author: MuoDosta
-Author-email: MuoDostaWork@gmail.com
-License: MIT License
-Requires-Python: >=3.10,<4.0
-Description-Content-Type: text/markdown
-
-# The hrbot
-The hrbot is a wrapper on top of the [HighRise Python Bot SDK](https://github.com/pocketzworld/python-bot-sdk) that makes it easy to create bots in [HighRise](https://highrise.game/).
-
-Install the library:
-```shell
-pip install hrbot
-```
-
-Example:
-```python
-from hrbot import Bot, Dispatcher  
-from hrbot.types.hr import *
-
-dp = Dispatcher()
-bot = Bot(
-    api_key='',
-    room_id='',
-    dispatcher=dp
-)
-
-@dp.on_user_join()
-async def user_join(user: User):
-    await bot.highrise.chat(f'Hi, {user.username}')
-
-@dp.on_chat(command='help', case_ignore=True, prefix='!')
-async def help_command(user: User, message: str):
-    await bot.highrise.chat('some text')
-
-@dp.on_chat()
-async def echo(user: User, message: str):
-    await bot.highrise.chat(message)
-
-@dp.on_user_leave()
-async def user_leave(user: User):
-    await bot.highrise.chat(f'Goodbye, {user.username}')
-
-if __name__ == '__main__':
-    bot.start()
-```
+Metadata-Version: 2.1
+Name: hrbot
+Version: 0.1.0
+Summary: The hrbot is a wrapper on top of the HighRise Python Bot SDK that makes it easy to create bots in HighRise.
+License: MIT
+Author: MuoDosta
+Author-email: MuoDostaWork@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: highrise-bot-sdk (==23.1.0b12)
+Requires-Dist: redis (>=4.5.5,<5.0.0)
+Description-Content-Type: text/markdown
+
+# The hrbot
+The hrbot is a wrapper on top of the [HighRise Python Bot SDK](https://github.com/pocketzworld/python-bot-sdk) that makes it easy to create bots in [HighRise](https://highrise.game/).
+
+Install the library:
+```shell
+pip install hrbot
+```
+
+Example:
+```python
+from hrbot import Bot, Dispatcher  
+from hrbot.types.hr import *
+
+dp = Dispatcher()
+bot = Bot(
+    api_key='',
+    room_id='',
+    dispatcher=dp
+)
+
+@dp.on_user_join()
+async def user_join(user: User):
+    await bot.highrise.chat(f'Hi, {user.username}')
+
+@dp.on_chat(command='help', case_ignore=True, prefix='!')
+async def help_command(user: User, message: str):
+    await bot.highrise.chat('some text')
+
+@dp.on_chat()
+async def echo(user: User, message: str):
+    await bot.highrise.chat(message)
+
+@dp.on_user_leave()
+async def user_leave(user: User):
+    await bot.highrise.chat(f'Goodbye, {user.username}')
+
+if __name__ == '__main__':
+    bot.start()
+```
```

