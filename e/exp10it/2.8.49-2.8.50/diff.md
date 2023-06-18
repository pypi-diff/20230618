# Comparing `tmp/exp10it-2.8.49.tar.gz` & `tmp/exp10it-2.8.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/exp10it-2.8.49.tar", last modified: Sun Jun 18 16:49:58 2023, max compression
+gzip compressed data, was "dist/exp10it-2.8.50.tar", last modified: Sun Jun 18 16:57:46 2023, max compression
```

## Comparing `exp10it-2.8.49.tar` & `exp10it-2.8.50.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 3xp10it    (502) staff       (20)        0 2023-06-18 16:49:58.000000 exp10it-2.8.49/
--rw-r--r--   0 3xp10it    (502) staff       (20)      617 2023-06-18 16:49:58.000000 exp10it-2.8.49/PKG-INFO
-drwxr-xr-x   0 3xp10it    (502) staff       (20)        0 2023-06-18 16:49:58.000000 exp10it-2.8.49/exp10it.egg-info/
--rw-r--r--   0 3xp10it    (502) staff       (20)      617 2023-06-18 16:49:58.000000 exp10it-2.8.49/exp10it.egg-info/PKG-INFO
--rw-r--r--   0 3xp10it    (502) staff       (20)        1 2018-04-20 11:29:26.000000 exp10it-2.8.49/exp10it.egg-info/zip-safe
--rw-r--r--   0 3xp10it    (502) staff       (20)      262 2023-06-18 16:49:58.000000 exp10it-2.8.49/exp10it.egg-info/SOURCES.txt
--rw-r--r--   0 3xp10it    (502) staff       (20)      121 2023-06-18 16:49:58.000000 exp10it-2.8.49/exp10it.egg-info/requires.txt
--rw-r--r--   0 3xp10it    (502) staff       (20)       18 2023-06-18 16:49:58.000000 exp10it-2.8.49/exp10it.egg-info/top_level.txt
--rw-r--r--   0 3xp10it    (502) staff       (20)        1 2023-06-18 16:49:58.000000 exp10it-2.8.49/exp10it.egg-info/dependency_links.txt
--rwxr-xr-x   0 3xp10it    (502) staff       (20)    18901 2021-08-28 04:50:51.000000 exp10it-2.8.49/api.md
--rw-r--r--   0 3xp10it    (502) staff       (20)   231958 2023-06-18 16:49:41.000000 exp10it-2.8.49/exp10it.py
--rwxr-xr-x   0 3xp10it    (502) staff       (20)       24 2018-01-31 13:35:11.000000 exp10it-2.8.49/MANIFEST.in
--rwxr-xr-x   0 3xp10it    (502) staff       (20)      103 2018-01-31 13:35:11.000000 exp10it-2.8.49/README.md
--rw-r--r--   0 3xp10it    (502) staff       (20)     3197 2023-06-18 16:49:53.000000 exp10it-2.8.49/setup.py
--rw-r--r--   0 3xp10it    (502) staff       (20)      179 2018-01-31 13:35:11.000000 exp10it-2.8.49/updateapi.py
--rw-r--r--   0 3xp10it    (502) staff       (20)       59 2023-06-18 16:49:58.000000 exp10it-2.8.49/setup.cfg
--rwxr-xr-x   0 3xp10it    (502) staff       (20)     1035 2018-01-31 13:35:11.000000 exp10it-2.8.49/README.rst
+drwxr-xr-x   0 3xp10it    (502) staff       (20)        0 2023-06-18 16:57:46.000000 exp10it-2.8.50/
+-rw-r--r--   0 3xp10it    (502) staff       (20)      617 2023-06-18 16:57:46.000000 exp10it-2.8.50/PKG-INFO
+drwxr-xr-x   0 3xp10it    (502) staff       (20)        0 2023-06-18 16:57:46.000000 exp10it-2.8.50/exp10it.egg-info/
+-rw-r--r--   0 3xp10it    (502) staff       (20)      617 2023-06-18 16:57:46.000000 exp10it-2.8.50/exp10it.egg-info/PKG-INFO
+-rw-r--r--   0 3xp10it    (502) staff       (20)        1 2018-04-20 11:29:26.000000 exp10it-2.8.50/exp10it.egg-info/zip-safe
+-rw-r--r--   0 3xp10it    (502) staff       (20)      262 2023-06-18 16:57:46.000000 exp10it-2.8.50/exp10it.egg-info/SOURCES.txt
+-rw-r--r--   0 3xp10it    (502) staff       (20)      121 2023-06-18 16:57:46.000000 exp10it-2.8.50/exp10it.egg-info/requires.txt
+-rw-r--r--   0 3xp10it    (502) staff       (20)       18 2023-06-18 16:57:46.000000 exp10it-2.8.50/exp10it.egg-info/top_level.txt
+-rw-r--r--   0 3xp10it    (502) staff       (20)        1 2023-06-18 16:57:46.000000 exp10it-2.8.50/exp10it.egg-info/dependency_links.txt
+-rwxr-xr-x   0 3xp10it    (502) staff       (20)    18901 2021-08-28 04:50:51.000000 exp10it-2.8.50/api.md
+-rw-r--r--   0 3xp10it    (502) staff       (20)   231958 2023-06-18 16:57:37.000000 exp10it-2.8.50/exp10it.py
+-rwxr-xr-x   0 3xp10it    (502) staff       (20)       24 2018-01-31 13:35:11.000000 exp10it-2.8.50/MANIFEST.in
+-rwxr-xr-x   0 3xp10it    (502) staff       (20)      103 2018-01-31 13:35:11.000000 exp10it-2.8.50/README.md
+-rw-r--r--   0 3xp10it    (502) staff       (20)     3197 2023-06-18 16:57:42.000000 exp10it-2.8.50/setup.py
+-rw-r--r--   0 3xp10it    (502) staff       (20)      179 2018-01-31 13:35:11.000000 exp10it-2.8.50/updateapi.py
+-rw-r--r--   0 3xp10it    (502) staff       (20)       59 2023-06-18 16:57:46.000000 exp10it-2.8.50/setup.cfg
+-rwxr-xr-x   0 3xp10it    (502) staff       (20)     1035 2018-01-31 13:35:11.000000 exp10it-2.8.50/README.rst
```

### Comparing `exp10it-2.8.49/PKG-INFO` & `exp10it-2.8.50/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: exp10it
-Version: 2.8.49
+Version: 2.8.50
 Summary: This is a package about network security
 Home-page: http://3xp10it.cc
 Author: quanyechavshuo
 Author-email: quanyechavshuo@gmail.com
 License: MIT
 Description: ### About
```

### Comparing `exp10it-2.8.49/exp10it.egg-info/PKG-INFO` & `exp10it-2.8.50/exp10it.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: exp10it
-Version: 2.8.49
+Version: 2.8.50
 Summary: This is a package about network security
 Home-page: http://3xp10it.cc
 Author: quanyechavshuo
 Author-email: quanyechavshuo@gmail.com
 License: MIT
 Description: ### About
```

### Comparing `exp10it-2.8.49/api.md` & `exp10it-2.8.50/api.md`

 * *Files identical despite different names*

### Comparing `exp10it-2.8.49/exp10it.py` & `exp10it-2.8.50/exp10it.py`

 * *Files 0% similar despite different names*

```diff
@@ -2682,36 +2682,36 @@
                 1) + re.search(r" (\S+)", uri_line, re.I).group(1)
             if string[:3] == "GET":
                 if proxies == {}:
                     async with aiohttp.ClientSession() as session:
                         async with session.get(url, headers=header_dict, timeout=30, ssl=False) as res:
                             code = res.status
                             headers = res.headers
-                            content = await res.text()
+                            content = await res.read()
                 else:
                     async with aiohttp.ClientSession() as session:
                         async with session.get(url, headers=header_dict, proxy=proxies, timeout=30, ssl=False) as res:
                             code = res.status
                             headers = res.headers
-                            content = await res.text()
+                            content = await res.read()
             elif string[:4] == "POST":
                 post_string = re.search(r"((\r\n\r\n)|(\n\n))(.*)", string).group(4)
                 post_string_bytes = post_string.encode("utf8")
                 if proxies == {}:
                     async with aiohttp.ClientSession() as session:
                         async with session.post(url, headers=header_dict, data=post_string_bytes, timeout=30, ssl=False) as res:
                             code = res.status
                             headers = res.headers
-                            content = await res.text()
+                            content = await res.read()
                 else:
                     async with aiohttp.ClientSession() as session:
                         async with session.post(url, headers=header_dict, data=post_string_bytes, proxy=proxies, timeout=30, ssl=False) as res:
                             code = res.status
                             headers = res.headers
-                            content = await res.text()
+                            content = await res.read()
             if encoding=='chardet':
                 import chardet
                 bytes_encoding = chardet.detect(content)['encoding']
                 if bytes_encoding is None:
                     bytes_encoding="utf8"
             else:
                 bytes_encoding=encoding
```

### Comparing `exp10it-2.8.49/setup.py` & `exp10it-2.8.50/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 DESCRIPTION = "This is a package about network security"
 LONG_DESCRIPTION = read("README.md")
 KEYWORDS = "network security package"
 AUTHOR = "quanyechavshuo"
 AUTHOR_EMAIL = "quanyechavshuo@gmail.com"
 URL = "http://3xp10it.cc"
 
-VERSION = "2.8.49"
+VERSION = "2.8.50"
 LICENSE = "MIT"
 #beepy在linux下可能会安装失败,有需要的情况下要手动安装
 require_package_list=['mechanicalsoup', 'bs4', 'selenium', 'colorama', 'requests', 'configparser', 'chardet', 'wget', 'pymysql','pyperclip','html2text']
 system=platform.system()
 if system in ['Windows','Darwin']:
     #require_package_list.append("beepy")
     try:
```

### Comparing `exp10it-2.8.49/README.rst` & `exp10it-2.8.50/README.rst`

 * *Files identical despite different names*

