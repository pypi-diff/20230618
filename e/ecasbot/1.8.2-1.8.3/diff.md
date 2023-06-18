# Comparing `tmp/ecasbot-1.8.2.tar.gz` & `tmp/ecasbot-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecasbot-1.8.2.tar", last modified: Sun Apr 16 13:35:20 2023, max compression
+gzip compressed data, was "ecasbot-1.8.3.tar", last modified: Sun Jun 18 11:45:28 2023, max compression
```

## Comparing `ecasbot-1.8.2.tar` & `ecasbot-1.8.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-04-16 13:35:20.049436 ecasbot-1.8.2/
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      134 2023-01-14 12:46:51.000000 ecasbot-1.8.2/.bandit.yml
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)    35141 2018-08-07 15:49:55.000000 ecasbot-1.8.2/LICENSE
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      178 2023-01-14 12:46:51.000000 ecasbot-1.8.2/MANIFEST.in
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     3068 2023-04-16 13:35:20.049436 ecasbot-1.8.2/PKG-INFO
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     2303 2022-12-25 10:28:05.000000 ecasbot-1.8.2/README.md
-drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-04-16 13:35:20.043436 ecasbot-1.8.2/licenses/
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)    11357 2022-05-07 14:34:35.000000 ecasbot-1.8.2/licenses/noto-emoji.LICENSE.txt
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1240 2023-04-16 13:35:09.000000 ecasbot-1.8.2/pyproject.toml
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)       38 2023-04-16 13:35:20.049436 ecasbot-1.8.2/setup.cfg
-drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-04-16 13:35:20.041436 ecasbot-1.8.2/src/
-drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-04-16 13:35:20.046436 ecasbot-1.8.2/src/ecasbot/
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)    40962 2023-04-16 13:35:09.000000 ecasbot-1.8.2/src/ecasbot/__init__.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     2156 2023-01-14 12:46:51.000000 ecasbot-1.8.2/src/ecasbot/chkmsg.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     2974 2023-01-14 12:46:51.000000 ecasbot-1.8.2/src/ecasbot/chkusr.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      535 2023-02-08 14:20:08.000000 ecasbot-1.8.2/src/ecasbot/exceptions.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      894 2023-01-14 12:46:51.000000 ecasbot-1.8.2/src/ecasbot/extractor.py
-drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-04-16 13:35:20.047436 ecasbot-1.8.2/src/ecasbot/messages/
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      648 2023-01-14 12:46:51.000000 ecasbot-1.8.2/src/ecasbot/messages/__init__.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1023 2023-01-14 12:46:51.000000 ecasbot-1.8.2/src/ecasbot/messages/factory.py
-drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-04-16 13:35:20.048436 ecasbot-1.8.2/src/ecasbot/messages/locales/
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      362 2023-01-14 12:46:51.000000 ecasbot-1.8.2/src/ecasbot/messages/locales/__init__.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     5291 2023-01-26 10:59:39.000000 ecasbot-1.8.2/src/ecasbot/messages/locales/en.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     9686 2023-01-26 10:59:39.000000 ecasbot-1.8.2/src/ecasbot/messages/locales/ru.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     2391 2023-04-16 13:35:09.000000 ecasbot-1.8.2/src/ecasbot/permissions.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1194 2023-02-10 14:49:03.000000 ecasbot-1.8.2/src/ecasbot/ranges.py
-drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-04-16 13:35:20.049436 ecasbot-1.8.2/src/ecasbot/scripts/
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      114 2023-01-14 12:46:51.000000 ecasbot-1.8.2/src/ecasbot/scripts/__init__.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      414 2023-01-14 12:46:51.000000 ecasbot-1.8.2/src/ecasbot/scripts/runbot.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)    12725 2023-02-08 14:20:08.000000 ecasbot-1.8.2/src/ecasbot/settings.py
-drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-04-16 13:35:20.047436 ecasbot-1.8.2/src/ecasbot.egg-info/
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     3068 2023-04-16 13:35:20.000000 ecasbot-1.8.2/src/ecasbot.egg-info/PKG-INFO
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      738 2023-04-16 13:35:20.000000 ecasbot-1.8.2/src/ecasbot.egg-info/SOURCES.txt
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)        1 2023-04-16 13:35:20.000000 ecasbot-1.8.2/src/ecasbot.egg-info/dependency_links.txt
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)       56 2023-04-16 13:35:20.000000 ecasbot-1.8.2/src/ecasbot.egg-info/entry_points.txt
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      104 2023-04-16 13:35:20.000000 ecasbot-1.8.2/src/ecasbot.egg-info/requires.txt
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)        8 2023-04-16 13:35:20.000000 ecasbot-1.8.2/src/ecasbot.egg-info/top_level.txt
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1431 2023-01-26 10:59:39.000000 ecasbot-1.8.2/tox.ini
+drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-06-18 11:45:28.558792 ecasbot-1.8.3/
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      134 2023-01-14 12:46:51.000000 ecasbot-1.8.3/.bandit.yml
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)    35141 2018-08-07 15:49:55.000000 ecasbot-1.8.3/LICENSE
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      178 2023-01-14 12:46:51.000000 ecasbot-1.8.3/MANIFEST.in
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     3079 2023-06-18 11:45:28.558792 ecasbot-1.8.3/PKG-INFO
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     2303 2022-12-25 10:28:05.000000 ecasbot-1.8.3/README.md
+drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-06-18 11:45:28.552792 ecasbot-1.8.3/licenses/
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)    11357 2022-05-07 14:34:35.000000 ecasbot-1.8.3/licenses/noto-emoji.LICENSE.txt
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1258 2023-06-18 11:45:18.000000 ecasbot-1.8.3/pyproject.toml
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)       38 2023-06-18 11:45:28.559792 ecasbot-1.8.3/setup.cfg
+drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-06-18 11:45:28.551792 ecasbot-1.8.3/src/
+drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-06-18 11:45:28.555792 ecasbot-1.8.3/src/ecasbot/
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)    40962 2023-04-16 13:35:09.000000 ecasbot-1.8.3/src/ecasbot/__init__.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     2156 2023-01-14 12:46:51.000000 ecasbot-1.8.3/src/ecasbot/chkmsg.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     2974 2023-01-14 12:46:51.000000 ecasbot-1.8.3/src/ecasbot/chkusr.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      535 2023-02-08 14:20:08.000000 ecasbot-1.8.3/src/ecasbot/exceptions.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      894 2023-01-14 12:46:51.000000 ecasbot-1.8.3/src/ecasbot/extractor.py
+drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-06-18 11:45:28.557793 ecasbot-1.8.3/src/ecasbot/messages/
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      648 2023-01-14 12:46:51.000000 ecasbot-1.8.3/src/ecasbot/messages/__init__.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1023 2023-01-14 12:46:51.000000 ecasbot-1.8.3/src/ecasbot/messages/factory.py
+drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-06-18 11:45:28.557793 ecasbot-1.8.3/src/ecasbot/messages/locales/
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      362 2023-01-14 12:46:51.000000 ecasbot-1.8.3/src/ecasbot/messages/locales/__init__.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     5291 2023-01-26 10:59:39.000000 ecasbot-1.8.3/src/ecasbot/messages/locales/en.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     9686 2023-01-26 10:59:39.000000 ecasbot-1.8.3/src/ecasbot/messages/locales/ru.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     2391 2023-04-16 13:35:09.000000 ecasbot-1.8.3/src/ecasbot/permissions.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1194 2023-02-10 14:49:03.000000 ecasbot-1.8.3/src/ecasbot/ranges.py
+drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-06-18 11:45:28.558792 ecasbot-1.8.3/src/ecasbot/scripts/
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      114 2023-01-14 12:46:51.000000 ecasbot-1.8.3/src/ecasbot/scripts/__init__.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      414 2023-01-14 12:46:51.000000 ecasbot-1.8.3/src/ecasbot/scripts/runbot.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)    12725 2023-02-08 14:20:08.000000 ecasbot-1.8.3/src/ecasbot/settings.py
+drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-06-18 11:45:28.556792 ecasbot-1.8.3/src/ecasbot.egg-info/
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     3079 2023-06-18 11:45:28.000000 ecasbot-1.8.3/src/ecasbot.egg-info/PKG-INFO
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      738 2023-06-18 11:45:28.000000 ecasbot-1.8.3/src/ecasbot.egg-info/SOURCES.txt
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)        1 2023-06-18 11:45:28.000000 ecasbot-1.8.3/src/ecasbot.egg-info/dependency_links.txt
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)       56 2023-06-18 11:45:28.000000 ecasbot-1.8.3/src/ecasbot.egg-info/entry_points.txt
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      104 2023-06-18 11:45:28.000000 ecasbot-1.8.3/src/ecasbot.egg-info/requires.txt
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)        8 2023-06-18 11:45:28.000000 ecasbot-1.8.3/src/ecasbot.egg-info/top_level.txt
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1431 2023-01-26 10:59:39.000000 ecasbot-1.8.3/tox.ini
```

### Comparing `ecasbot-1.8.2/LICENSE` & `ecasbot-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.2/PKG-INFO` & `ecasbot-1.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: ecasbot
-Version: 1.8.2
+Version: 1.8.3
 Summary: EC AntiSpam bot for the Telegram messenger
 Author-email: Vitaly Zaitsev <vitaly@easycoding.org>
 License: GPL-3.0-or-later
 Project-URL: homepage, https://github.com/xvitaly/ecasbot
 Project-URL: documentation, https://github.com/xvitaly/ecasbot/blob/master/docs/README.md
 Project-URL: repository, https://github.com/xvitaly/ecasbot
-Keywords: anti-spam,bot,database-less,telegram,telegram-api,telegram-bot
+Keywords: anti-spam,bot,database-less,protection,telegram,telegram-api,telegram-bot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: deploy
 Provides-Extra: test
```

### Comparing `ecasbot-1.8.2/README.md` & `ecasbot-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.2/licenses/noto-emoji.LICENSE.txt` & `ecasbot-1.8.3/licenses/noto-emoji.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.2/pyproject.toml` & `ecasbot-1.8.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,30 +2,31 @@
 
 # SPDX-FileCopyrightText: 2017-2023 EasyCoding Team
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 [project]
 name = "ecasbot"
-version = "1.8.2"
+version = "1.8.3"
 license = { text = "GPL-3.0-or-later" }
 readme = "README.md"
 dependencies = [
     "requests>=2.28.0",
-    "pytelegrambotapi>=4.11.0",
-    "emoji>=2.2.0"
+    "pytelegrambotapi>=4.12.0",
+    "emoji>=2.5.1"
 ]
 authors = [
     { name = "Vitaly Zaitsev", email="vitaly@easycoding.org" }
 ]
 description = "EC AntiSpam bot for the Telegram messenger"
 keywords = [
     "anti-spam",
     "bot",
     "database-less",
+    "protection",
     "telegram",
     "telegram-api",
     "telegram-bot"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `ecasbot-1.8.2/src/ecasbot/__init__.py` & `ecasbot-1.8.3/src/ecasbot/__init__.py`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.2/src/ecasbot/chkmsg.py` & `ecasbot-1.8.3/src/ecasbot/chkmsg.py`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.2/src/ecasbot/chkusr.py` & `ecasbot-1.8.3/src/ecasbot/chkusr.py`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.2/src/ecasbot/exceptions.py` & `ecasbot-1.8.3/src/ecasbot/exceptions.py`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.2/src/ecasbot/extractor.py` & `ecasbot-1.8.3/src/ecasbot/extractor.py`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.2/src/ecasbot/messages/__init__.py` & `ecasbot-1.8.3/src/ecasbot/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.2/src/ecasbot/messages/factory.py` & `ecasbot-1.8.3/src/ecasbot/messages/factory.py`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.2/src/ecasbot/messages/locales/en.py` & `ecasbot-1.8.3/src/ecasbot/messages/locales/en.py`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.2/src/ecasbot/messages/locales/ru.py` & `ecasbot-1.8.3/src/ecasbot/messages/locales/ru.py`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.2/src/ecasbot/permissions.py` & `ecasbot-1.8.3/src/ecasbot/permissions.py`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.2/src/ecasbot/ranges.py` & `ecasbot-1.8.3/src/ecasbot/ranges.py`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.2/src/ecasbot/settings.py` & `ecasbot-1.8.3/src/ecasbot/settings.py`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.2/src/ecasbot.egg-info/PKG-INFO` & `ecasbot-1.8.3/src/ecasbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: ecasbot
-Version: 1.8.2
+Version: 1.8.3
 Summary: EC AntiSpam bot for the Telegram messenger
 Author-email: Vitaly Zaitsev <vitaly@easycoding.org>
 License: GPL-3.0-or-later
 Project-URL: homepage, https://github.com/xvitaly/ecasbot
 Project-URL: documentation, https://github.com/xvitaly/ecasbot/blob/master/docs/README.md
 Project-URL: repository, https://github.com/xvitaly/ecasbot
-Keywords: anti-spam,bot,database-less,telegram,telegram-api,telegram-bot
+Keywords: anti-spam,bot,database-less,protection,telegram,telegram-api,telegram-bot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: deploy
 Provides-Extra: test
```

### Comparing `ecasbot-1.8.2/src/ecasbot.egg-info/SOURCES.txt` & `ecasbot-1.8.3/src/ecasbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.2/tox.ini` & `ecasbot-1.8.3/tox.ini`

 * *Files identical despite different names*

