# Comparing `tmp/exp10it-2.8.48.tar.gz` & `tmp/exp10it-2.8.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/exp10it-2.8.48.tar", last modified: Sun Jun 18 16:41:22 2023, max compression
+gzip compressed data, was "dist/exp10it-2.8.49.tar", last modified: Sun Jun 18 16:49:58 2023, max compression
```

## Comparing `exp10it-2.8.48.tar` & `exp10it-2.8.49.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 3xp10it    (502) staff       (20)        0 2023-06-18 16:41:22.000000 exp10it-2.8.48/
--rw-r--r--   0 3xp10it    (502) staff       (20)      617 2023-06-18 16:41:22.000000 exp10it-2.8.48/PKG-INFO
-drwxr-xr-x   0 3xp10it    (502) staff       (20)        0 2023-06-18 16:41:22.000000 exp10it-2.8.48/exp10it.egg-info/
--rw-r--r--   0 3xp10it    (502) staff       (20)      617 2023-06-18 16:41:22.000000 exp10it-2.8.48/exp10it.egg-info/PKG-INFO
--rw-r--r--   0 3xp10it    (502) staff       (20)        1 2018-04-20 11:29:26.000000 exp10it-2.8.48/exp10it.egg-info/zip-safe
--rw-r--r--   0 3xp10it    (502) staff       (20)      262 2023-06-18 16:41:22.000000 exp10it-2.8.48/exp10it.egg-info/SOURCES.txt
--rw-r--r--   0 3xp10it    (502) staff       (20)      113 2023-06-18 16:41:22.000000 exp10it-2.8.48/exp10it.egg-info/requires.txt
--rw-r--r--   0 3xp10it    (502) staff       (20)       18 2023-06-18 16:41:22.000000 exp10it-2.8.48/exp10it.egg-info/top_level.txt
--rw-r--r--   0 3xp10it    (502) staff       (20)        1 2023-06-18 16:41:22.000000 exp10it-2.8.48/exp10it.egg-info/dependency_links.txt
--rwxr-xr-x   0 3xp10it    (502) staff       (20)    18901 2021-08-28 04:50:51.000000 exp10it-2.8.48/api.md
--rw-r--r--   0 3xp10it    (502) staff       (20)   231943 2023-06-18 16:37:35.000000 exp10it-2.8.48/exp10it.py
--rwxr-xr-x   0 3xp10it    (502) staff       (20)       24 2018-01-31 13:35:11.000000 exp10it-2.8.48/MANIFEST.in
--rwxr-xr-x   0 3xp10it    (502) staff       (20)      103 2018-01-31 13:35:11.000000 exp10it-2.8.48/README.md
--rw-r--r--   0 3xp10it    (502) staff       (20)     3167 2023-06-18 16:37:48.000000 exp10it-2.8.48/setup.py
--rw-r--r--   0 3xp10it    (502) staff       (20)      179 2018-01-31 13:35:11.000000 exp10it-2.8.48/updateapi.py
--rw-r--r--   0 3xp10it    (502) staff       (20)       59 2023-06-18 16:41:22.000000 exp10it-2.8.48/setup.cfg
--rwxr-xr-x   0 3xp10it    (502) staff       (20)     1035 2018-01-31 13:35:11.000000 exp10it-2.8.48/README.rst
+drwxr-xr-x   0 3xp10it    (502) staff       (20)        0 2023-06-18 16:49:58.000000 exp10it-2.8.49/
+-rw-r--r--   0 3xp10it    (502) staff       (20)      617 2023-06-18 16:49:58.000000 exp10it-2.8.49/PKG-INFO
+drwxr-xr-x   0 3xp10it    (502) staff       (20)        0 2023-06-18 16:49:58.000000 exp10it-2.8.49/exp10it.egg-info/
+-rw-r--r--   0 3xp10it    (502) staff       (20)      617 2023-06-18 16:49:58.000000 exp10it-2.8.49/exp10it.egg-info/PKG-INFO
+-rw-r--r--   0 3xp10it    (502) staff       (20)        1 2018-04-20 11:29:26.000000 exp10it-2.8.49/exp10it.egg-info/zip-safe
+-rw-r--r--   0 3xp10it    (502) staff       (20)      262 2023-06-18 16:49:58.000000 exp10it-2.8.49/exp10it.egg-info/SOURCES.txt
+-rw-r--r--   0 3xp10it    (502) staff       (20)      121 2023-06-18 16:49:58.000000 exp10it-2.8.49/exp10it.egg-info/requires.txt
+-rw-r--r--   0 3xp10it    (502) staff       (20)       18 2023-06-18 16:49:58.000000 exp10it-2.8.49/exp10it.egg-info/top_level.txt
+-rw-r--r--   0 3xp10it    (502) staff       (20)        1 2023-06-18 16:49:58.000000 exp10it-2.8.49/exp10it.egg-info/dependency_links.txt
+-rwxr-xr-x   0 3xp10it    (502) staff       (20)    18901 2021-08-28 04:50:51.000000 exp10it-2.8.49/api.md
+-rw-r--r--   0 3xp10it    (502) staff       (20)   231958 2023-06-18 16:49:41.000000 exp10it-2.8.49/exp10it.py
+-rwxr-xr-x   0 3xp10it    (502) staff       (20)       24 2018-01-31 13:35:11.000000 exp10it-2.8.49/MANIFEST.in
+-rwxr-xr-x   0 3xp10it    (502) staff       (20)      103 2018-01-31 13:35:11.000000 exp10it-2.8.49/README.md
+-rw-r--r--   0 3xp10it    (502) staff       (20)     3197 2023-06-18 16:49:53.000000 exp10it-2.8.49/setup.py
+-rw-r--r--   0 3xp10it    (502) staff       (20)      179 2018-01-31 13:35:11.000000 exp10it-2.8.49/updateapi.py
+-rw-r--r--   0 3xp10it    (502) staff       (20)       59 2023-06-18 16:49:58.000000 exp10it-2.8.49/setup.cfg
+-rwxr-xr-x   0 3xp10it    (502) staff       (20)     1035 2018-01-31 13:35:11.000000 exp10it-2.8.49/README.rst
```

### Comparing `exp10it-2.8.48/PKG-INFO` & `exp10it-2.8.49/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: exp10it
-Version: 2.8.48
+Version: 2.8.49
 Summary: This is a package about network security
 Home-page: http://3xp10it.cc
 Author: quanyechavshuo
 Author-email: quanyechavshuo@gmail.com
 License: MIT
 Description: ### About
```

### Comparing `exp10it-2.8.48/exp10it.egg-info/PKG-INFO` & `exp10it-2.8.49/exp10it.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: exp10it
-Version: 2.8.48
+Version: 2.8.49
 Summary: This is a package about network security
 Home-page: http://3xp10it.cc
 Author: quanyechavshuo
 Author-email: quanyechavshuo@gmail.com
 License: MIT
 Description: ### About
```

### Comparing `exp10it-2.8.48/api.md` & `exp10it-2.8.49/api.md`

 * *Files identical despite different names*

### Comparing `exp10it-2.8.48/exp10it.py` & `exp10it-2.8.49/exp10it.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pdb
+import aiohttp
 import chardet
 import platform
 import os
 import re
 import sys
 import random
 import time
```

### Comparing `exp10it-2.8.48/setup.py` & `exp10it-2.8.49/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,32 +29,32 @@
 DESCRIPTION = "This is a package about network security"
 LONG_DESCRIPTION = read("README.md")
 KEYWORDS = "network security package"
 AUTHOR = "quanyechavshuo"
 AUTHOR_EMAIL = "quanyechavshuo@gmail.com"
 URL = "http://3xp10it.cc"
 
-VERSION = "2.8.48"
+VERSION = "2.8.49"
 LICENSE = "MIT"
 #beepy在linux下可能会安装失败,有需要的情况下要手动安装
 require_package_list=['mechanicalsoup', 'bs4', 'selenium', 'colorama', 'requests', 'configparser', 'chardet', 'wget', 'pymysql','pyperclip','html2text']
 system=platform.system()
 if system in ['Windows','Darwin']:
     #require_package_list.append("beepy")
     try:
         #有的windows无法安装beepy
         os.system("pip3 install beepy")
     except:
         pass
 if system=='Windows':
-    require_package_list=['mechanicalsoup', 'bs4', 'selenium', 'colorama', 'requests', 'configparser', 'chardet', 'wget', 'pycryptodome', 'pymysql','pyperclip','html2text','pywin32']
+    require_package_list=['aiohttp','mechanicalsoup', 'bs4', 'selenium', 'colorama', 'requests', 'configparser', 'chardet', 'wget', 'pycryptodome', 'pymysql','pyperclip','html2text','pywin32']
 elif system=='Darwin':
-    require_package_list=['mechanicalsoup', 'bs4', 'selenium', 'colorama', 'requests', 'configparser', 'chardet', 'wget', 'pycryptodome', 'pymysql','pyperclip','html2text']
+    require_package_list=['aiohttp','mechanicalsoup', 'bs4', 'selenium', 'colorama', 'requests', 'configparser', 'chardet', 'wget', 'pycryptodome', 'pymysql','pyperclip','html2text']
 else:
-    require_package_list=['mechanicalsoup', 'bs4', 'selenium', 'colorama', 'requests', 'configparser', 'chardet', 'wget', 'pycrypto', 'pymysql','pyperclip','html2text']
+    require_package_list=['aiohttp','mechanicalsoup', 'bs4', 'selenium', 'colorama', 'requests', 'configparser', 'chardet', 'wget', 'pycrypto', 'pymysql','pyperclip','html2text']
 
 if re.search(r"(centos)|(redhat)|(fedora)",platform.platform(),re.I):
     os.system("echo y | yum install readline")
 if re.search(r"(kali)|(debain)|(ubuntu)", platform.platform(), re.I):
     content=get_string_from_command("apt search libncurses5-dev")
     if "libncurses5-dev" not in content:
         os.system("apt-get update && (echo y | apt-get install libncurses5-dev) && pip3 install readline")
```

### Comparing `exp10it-2.8.48/README.rst` & `exp10it-2.8.49/README.rst`

 * *Files identical despite different names*

